# Comparing `tmp/motley_cue-0.5.1.tar.gz` & `tmp/motley_cue-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motley_cue-0.5.1.tar", last modified: Thu Dec  8 13:26:52 2022, max compression
+gzip compressed data, was "motley_cue-0.5.3.tar", last modified: Wed Jun 21 22:37:36 2023, max compression
```

## Comparing `motley_cue-0.5.1.tar` & `motley_cue-0.5.3.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 13:26:52.050867 motley_cue-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2022-12-08 13:26:52.050867 motley_cue-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2022-12-08 13:26:41.000000 motley_cue-0.5.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 13:26:52.046867 motley_cue-0.5.1/etc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 13:26:52.046867 motley_cue-0.5.1/etc/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      264 2022-12-08 13:26:41.000000 motley_cue-0.5.1/etc/bin/motley-cue
--rw-r--r--   0 runner    (1001) docker     (123)    12637 2022-12-08 13:26:41.000000 motley_cue-0.5.1/etc/feudal_adapter.conf
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2022-12-08 13:26:41.000000 motley_cue-0.5.1/etc/gunicorn.conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 13:26:52.046867 motley_cue-0.5.1/etc/init.d/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2365 2022-12-08 13:26:41.000000 motley_cue-0.5.1/etc/init.d/motley-cue
--rw-r--r--   0 runner    (1001) docker     (123)      448 2022-12-08 13:26:41.000000 motley_cue-0.5.1/etc/motley-cue.service
--rw-r--r--   0 runner    (1001) docker     (123)    10018 2022-12-08 13:26:41.000000 motley_cue-0.5.1/etc/motley_cue.conf
--rw-r--r--   0 runner    (1001) docker     (123)      279 2022-12-08 13:26:41.000000 motley_cue-0.5.1/etc/motley_cue.env
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2022-12-08 13:26:41.000000 motley_cue-0.5.1/etc/nginx.motley_cue
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2022-12-08 13:26:41.000000 motley_cue-0.5.1/etc/privacystatement.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 13:26:52.050867 motley_cue-0.5.1/etc/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2022-12-08 13:26:41.000000 motley_cue-0.5.1/etc/templates/admin.deploy.template
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2022-12-08 13:26:41.000000 motley_cue-0.5.1/etc/templates/admin.deploy.update.template
--rw-r--r--   0 runner    (1001) docker     (123)      302 2022-12-08 13:26:41.000000 motley_cue-0.5.1/etc/templates/admin.test.template
--rw-r--r--   0 runner    (1001) docker     (123)      991 2022-12-08 13:26:41.000000 motley_cue-0.5.1/etc/templates/admin.update.template
--rw-r--r--   0 runner    (1001) docker     (123)      255 2022-12-08 13:26:41.000000 motley_cue-0.5.1/etc/templates/unknown.template
--rw-r--r--   0 runner    (1001) docker     (123)      380 2022-12-08 13:26:41.000000 motley_cue-0.5.1/etc/templates/user.deploy.template
--rw-r--r--   0 runner    (1001) docker     (123)      417 2022-12-08 13:26:41.000000 motley_cue-0.5.1/etc/templates/user.deploy.update.template
--rw-r--r--   0 runner    (1001) docker     (123)      395 2022-12-08 13:26:41.000000 motley_cue-0.5.1/etc/templates/user.update.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 13:26:52.042867 motley_cue-0.5.1/motley_cue/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2022-12-08 13:26:41.000000 motley_cue-0.5.1/motley_cue/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 13:26:41.000000 motley_cue-0.5.1/motley_cue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2022-12-08 13:26:41.000000 motley_cue-0.5.1/motley_cue/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2022-12-08 13:26:41.000000 motley_cue-0.5.1/motley_cue/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4696 2022-12-08 13:26:41.000000 motley_cue-0.5.1/motley_cue/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2022-12-08 13:26:41.000000 motley_cue-0.5.1/motley_cue/dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 13:26:52.046867 motley_cue-0.5.1/motley_cue/mapper/
--rw-r--r--   0 runner    (1001) docker     (123)     7719 2022-12-08 13:26:41.000000 motley_cue-0.5.1/motley_cue/mapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9913 2022-12-08 13:26:41.000000 motley_cue-0.5.1/motley_cue/mapper/authorisation.py
--rw-r--r--   0 runner    (1001) docker     (123)    14405 2022-12-08 13:26:41.000000 motley_cue-0.5.1/motley_cue/mapper/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2022-12-08 13:26:41.000000 motley_cue-0.5.1/motley_cue/mapper/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6865 2022-12-08 13:26:41.000000 motley_cue-0.5.1/motley_cue/mapper/local_user_management.py
--rw-r--r--   0 runner    (1001) docker     (123)    18697 2022-12-08 13:26:41.000000 motley_cue-0.5.1/motley_cue/mapper/token_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2022-12-08 13:26:41.000000 motley_cue-0.5.1/motley_cue/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 13:26:52.046867 motley_cue-0.5.1/motley_cue/routers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 13:26:41.000000 motley_cue-0.5.1/motley_cue/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2022-12-08 13:26:41.000000 motley_cue-0.5.1/motley_cue/routers/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2022-12-08 13:26:41.000000 motley_cue-0.5.1/motley_cue/routers/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2022-12-08 13:26:41.000000 motley_cue-0.5.1/motley_cue/static.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 13:26:52.050867 motley_cue-0.5.1/motley_cue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2022-12-08 13:26:52.000000 motley_cue-0.5.1/motley_cue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2022-12-08 13:26:52.000000 motley_cue-0.5.1/motley_cue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-08 13:26:52.000000 motley_cue-0.5.1/motley_cue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2022-12-08 13:26:52.000000 motley_cue-0.5.1/motley_cue.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2022-12-08 13:26:52.000000 motley_cue-0.5.1/motley_cue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2022-12-08 13:26:52.000000 motley_cue-0.5.1/motley_cue.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2022-12-08 13:26:41.000000 motley_cue-0.5.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 13:26:52.050867 motley_cue-0.5.1/selinux/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2022-12-08 13:26:41.000000 motley_cue-0.5.1/selinux/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      547 2022-12-08 13:26:41.000000 motley_cue-0.5.1/selinux/motley-cue-gunicorn.te
--rw-r--r--   0 runner    (1001) docker     (123)      399 2022-12-08 13:26:41.000000 motley_cue-0.5.1/selinux/motley-cue-nginx.te
--rw-r--r--   0 runner    (1001) docker     (123)      207 2022-12-08 13:26:41.000000 motley_cue-0.5.1/selinux/motley-cue-sshd.te
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2022-12-08 13:26:52.050867 motley_cue-0.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 13:26:52.046867 motley_cue-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 13:26:41.000000 motley_cue-0.5.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2022-12-08 13:26:41.000000 motley_cue-0.5.1/tests/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5239 2022-12-08 13:26:41.000000 motley_cue-0.5.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2022-12-08 13:26:41.000000 motley_cue-0.5.1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5680 2022-12-08 13:26:41.000000 motley_cue-0.5.1/tests/test_authorisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2022-12-08 13:26:41.000000 motley_cue-0.5.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6730 2022-12-08 13:26:41.000000 motley_cue-0.5.1/tests/test_local_user_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6586 2022-12-08 13:26:41.000000 motley_cue-0.5.1/tests/test_token_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8213 2022-12-08 13:26:41.000000 motley_cue-0.5.1/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:37:36.995091 motley_cue-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-06-21 22:37:36.995091 motley_cue-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-06-21 22:37:26.000000 motley_cue-0.5.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:37:36.991091 motley_cue-0.5.3/etc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:37:36.991091 motley_cue-0.5.3/etc/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-06-21 22:37:26.000000 motley_cue-0.5.3/etc/bin/motley-cue
+-rw-r--r--   0 runner    (1001) docker     (123)    12637 2023-06-21 22:37:26.000000 motley_cue-0.5.3/etc/feudal_adapter.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-06-21 22:37:26.000000 motley_cue-0.5.3/etc/gunicorn.conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:37:36.991091 motley_cue-0.5.3/etc/init.d/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2365 2023-06-21 22:37:26.000000 motley_cue-0.5.3/etc/init.d/motley-cue
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-21 22:37:26.000000 motley_cue-0.5.3/etc/motley-cue.service
+-rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-06-21 22:37:26.000000 motley_cue-0.5.3/etc/motley_cue.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-21 22:37:26.000000 motley_cue-0.5.3/etc/motley_cue.env
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-21 22:37:26.000000 motley_cue-0.5.3/etc/nginx.motley_cue
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-06-21 22:37:26.000000 motley_cue-0.5.3/etc/privacystatement.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:37:36.995091 motley_cue-0.5.3/etc/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-21 22:37:26.000000 motley_cue-0.5.3/etc/templates/admin.deploy.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-21 22:37:26.000000 motley_cue-0.5.3/etc/templates/admin.deploy.update.template
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-21 22:37:26.000000 motley_cue-0.5.3/etc/templates/admin.test.template
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-21 22:37:26.000000 motley_cue-0.5.3/etc/templates/admin.update.template
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-21 22:37:26.000000 motley_cue-0.5.3/etc/templates/unknown.template
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-21 22:37:26.000000 motley_cue-0.5.3/etc/templates/user.deploy.template
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-21 22:37:26.000000 motley_cue-0.5.3/etc/templates/user.deploy.update.template
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-21 22:37:26.000000 motley_cue-0.5.3/etc/templates/user.update.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:37:36.991091 motley_cue-0.5.3/motley_cue/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-21 22:37:26.000000 motley_cue-0.5.3/motley_cue/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:37:26.000000 motley_cue-0.5.3/motley_cue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-21 22:37:26.000000 motley_cue-0.5.3/motley_cue/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-21 22:37:26.000000 motley_cue-0.5.3/motley_cue/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-06-21 22:37:26.000000 motley_cue-0.5.3/motley_cue/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-21 22:37:26.000000 motley_cue-0.5.3/motley_cue/dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:37:36.991091 motley_cue-0.5.3/motley_cue/mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-06-21 22:37:26.000000 motley_cue-0.5.3/motley_cue/mapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9914 2023-06-21 22:37:26.000000 motley_cue-0.5.3/motley_cue/mapper/authorisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14574 2023-06-21 22:37:26.000000 motley_cue-0.5.3/motley_cue/mapper/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-21 22:37:26.000000 motley_cue-0.5.3/motley_cue/mapper/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6865 2023-06-21 22:37:26.000000 motley_cue-0.5.3/motley_cue/mapper/local_user_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18745 2023-06-21 22:37:26.000000 motley_cue-0.5.3/motley_cue/mapper/token_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-06-21 22:37:26.000000 motley_cue-0.5.3/motley_cue/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:37:36.991091 motley_cue-0.5.3/motley_cue/routers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:37:26.000000 motley_cue-0.5.3/motley_cue/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-06-21 22:37:26.000000 motley_cue-0.5.3/motley_cue/routers/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-06-21 22:37:26.000000 motley_cue-0.5.3/motley_cue/routers/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-21 22:37:26.000000 motley_cue-0.5.3/motley_cue/static.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:37:36.995091 motley_cue-0.5.3/motley_cue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-06-21 22:37:36.000000 motley_cue-0.5.3/motley_cue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-21 22:37:36.000000 motley_cue-0.5.3/motley_cue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 22:37:36.000000 motley_cue-0.5.3/motley_cue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-21 22:37:36.000000 motley_cue-0.5.3/motley_cue.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-21 22:37:36.000000 motley_cue-0.5.3/motley_cue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-21 22:37:36.000000 motley_cue-0.5.3/motley_cue.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-21 22:37:26.000000 motley_cue-0.5.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:37:36.995091 motley_cue-0.5.3/selinux/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-21 22:37:26.000000 motley_cue-0.5.3/selinux/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-21 22:37:26.000000 motley_cue-0.5.3/selinux/motley-cue-gunicorn.te
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-21 22:37:26.000000 motley_cue-0.5.3/selinux/motley-cue-nginx.te
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-21 22:37:26.000000 motley_cue-0.5.3/selinux/motley-cue-sshd.te
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-06-21 22:37:36.995091 motley_cue-0.5.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:37:36.991091 motley_cue-0.5.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:37:26.000000 motley_cue-0.5.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-06-21 22:37:26.000000 motley_cue-0.5.3/tests/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-06-21 22:37:26.000000 motley_cue-0.5.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-06-21 22:37:26.000000 motley_cue-0.5.3/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-06-21 22:37:26.000000 motley_cue-0.5.3/tests/test_authorisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-06-21 22:37:26.000000 motley_cue-0.5.3/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6782 2023-06-21 22:37:26.000000 motley_cue-0.5.3/tests/test_local_user_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6586 2023-06-21 22:37:26.000000 motley_cue-0.5.3/tests/test_token_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8235 2023-06-21 22:37:26.000000 motley_cue-0.5.3/tests/utils.py
```

### Comparing `motley_cue-0.5.1/PKG-INFO` & `motley_cue-0.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motley_cue
-Version: 0.5.1
+Version: 0.5.3
 Summary: Mapper Oidc To Local idEntitY with loCal User managEment
 Home-page: https://github.com/dianagudu/motley_cue
 Author: Diana Gudu
 Author-email: gudu@kit.edu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/dianagudu/motley_cue/issues
 Project-URL: Documentation, https://motley-cue.readthedocs.io
@@ -20,14 +20,15 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: System :: Systems Administration :: Authentication/Directory
 Classifier: Topic :: Utilities
 Description-Content-Type: text/x-rst
 
 .. image:: https://readthedocs.org/projects/motley-cue/badge/?version=latest
     :target: https://motley-cue.readthedocs.io/
```

### Comparing `motley_cue-0.5.1/README.rst` & `motley_cue-0.5.3/README.rst`

 * *Files identical despite different names*

### Comparing `motley_cue-0.5.1/etc/feudal_adapter.conf` & `motley_cue-0.5.3/etc/feudal_adapter.conf`

 * *Files identical despite different names*

### Comparing `motley_cue-0.5.1/etc/gunicorn.conf.py` & `motley_cue-0.5.3/etc/gunicorn.conf.py`

 * *Files identical despite different names*

### Comparing `motley_cue-0.5.1/etc/init.d/motley-cue` & `motley_cue-0.5.3/etc/init.d/motley-cue`

 * *Files identical despite different names*

### Comparing `motley_cue-0.5.1/etc/motley_cue.conf` & `motley_cue-0.5.3/etc/motley_cue.conf`

 * *Files identical despite different names*

### Comparing `motley_cue-0.5.1/etc/nginx.motley_cue` & `motley_cue-0.5.3/etc/nginx.motley_cue`

 * *Files identical despite different names*

### Comparing `motley_cue-0.5.1/etc/privacystatement.md` & `motley_cue-0.5.3/etc/privacystatement.md`

 * *Files identical despite different names*

### Comparing `motley_cue-0.5.1/etc/templates/admin.deploy.template` & `motley_cue-0.5.3/etc/templates/admin.deploy.template`

 * *Files identical despite different names*

### Comparing `motley_cue-0.5.1/etc/templates/admin.deploy.update.template` & `motley_cue-0.5.3/etc/templates/admin.deploy.update.template`

 * *Files identical despite different names*

### Comparing `motley_cue-0.5.1/etc/templates/admin.update.template` & `motley_cue-0.5.3/etc/templates/admin.update.template`

 * *Files identical despite different names*

### Comparing `motley_cue-0.5.1/motley_cue/api.py` & `motley_cue-0.5.3/motley_cue/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,27 +64,25 @@
 
 @api.get("/info", response_model=Info, response_model_exclude_unset=True)
 async def info():
     """Retrieve service-specific information:
 
     * login info
     * supported OPs
+    * ops_info per OP information, such as scopes, audience, etc.
     """
     return mapper.info()
 
 
 @api.get(
     "/info/authorisation",
     dependencies=[Depends(mapper.user_security)],
     response_model=InfoAuthorisation,
     response_model_exclude_unset=True,
-    responses={
-        200: {"model": InfoAuthorisation},
-        404: {"model": ClientError},
-    },
+    responses={**responses, 200: {"model": InfoAuthorisation}},
 )
 @mapper.authenticated_user_required
 async def info_authorisation(
     request: Request,
     header: str = Header(..., alias="Authorization", description="OIDC Access Token"),
 ):  # pylint: disable=unused-argument
     """Retrieve authorisation information for specific OP.
```

### Comparing `motley_cue-0.5.1/motley_cue/dependencies.py` & `motley_cue-0.5.3/motley_cue/dependencies.py`

 * *Files identical despite different names*

### Comparing `motley_cue-0.5.1/motley_cue/mapper/__init__.py` & `motley_cue-0.5.3/motley_cue/mapper/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,18 +70,23 @@
         """Admin security for FastAPI"""
         return self.__admin_security
 
     def info(self):
         """Return information about the local service:
         * supported OPs
         * login information
+        * ops_info per OP information, such as scopes, audience, etc.
         """
         return {
             "login_info": self.__lum.login_info(),
             "supported_OPs": self.__authorisation.trusted_op_list,
+            "ops_info": dict(
+                (op, self.__config.get_op_info(op))
+                for op in self.__authorisation.trusted_op_list
+            ),
         }
 
     def info_op(self, url: str):
         """Return information about a given OP"""
         info = self.__config.get_op_info(url)
         if info is None:
             raise NotFound(message="OP not supported")
```

### Comparing `motley_cue-0.5.1/motley_cue/mapper/authorisation.py` & `motley_cue-0.5.3/motley_cue/mapper/authorisation.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 from .config import Config, ConfigAuthorisation, canonical_url
 from .exceptions import Unauthorised
 
 
 logger = logging.getLogger(__name__)
 
+
 # We dynamically load the requirement in is_satisfied_by
 class AuthRequirement(Requirement):
     """Base class for authorisation requirements corresponding to an OP."""
 
     # pylint: disable=too-few-public-methods
     def __init__(self, authorisation: ConfigAuthorisation):
         self.authorisation = authorisation
```

### Comparing `motley_cue-0.5.1/motley_cue/mapper/config.py` & `motley_cue-0.5.3/motley_cue/mapper/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -332,19 +332,21 @@
     audience: str = ""
     # admin authorisation
     authorised_admins: list = field(default_factory=list)
     authorise_admins_for_all_ops: bool = False
 
     def get_info(self) -> dict:
         """Returns a dict with the info for this OP"""
-        return {
+        op_info = {
             "op_url": self.op_url,
             "scopes": self.scopes,
-            "audience": self.audience,
         }
+        if self.audience and self.audience != "":
+            op_info["audience"] = self.audience
+        return op_info
 
     # methods used in conjunction with flaat
     def get_user_requirement(self) -> Requirement:
         """Creates a (flaat) Requirement object from this authorisation configuration,
         for API users.
         """
         req = OneOf()
@@ -426,18 +428,18 @@
         return self.all_op_authz.get(canonical_url(user_infos.issuer), None)
 
 
 @dataclass
 class Configuration:
     """All configuration settings for motley_cue."""
 
-    mapper: ConfigMapper = ConfigMapper()
-    otp: ConfigOTP = ConfigOTP()
-    privacy: ConfigPrivacy = ConfigPrivacy()
-    authorisation: ConfigAuthorisation = ConfigAuthorisation()
+    mapper: ConfigMapper = field(default_factory=ConfigMapper)
+    otp: ConfigOTP = field(default_factory=ConfigOTP)
+    privacy: ConfigPrivacy = field(default_factory=ConfigPrivacy)
+    authorisation: ConfigAuthorisation = field(default_factory=ConfigAuthorisation)
 
     @classmethod
     def load(cls, config: ConfigParser):
         """Loads all config settings from the given config parser"""
         return cls(**{f.name: f.type.load(config) for f in fields(cls)})
 
     def to_dict(self) -> dict:
```

### Comparing `motley_cue-0.5.1/motley_cue/mapper/exceptions.py` & `motley_cue-0.5.3/motley_cue/mapper/exceptions.py`

 * *Files identical despite different names*

### Comparing `motley_cue-0.5.1/motley_cue/mapper/local_user_management.py` & `motley_cue-0.5.3/motley_cue/mapper/local_user_management.py`

 * *Files identical despite different names*

### Comparing `motley_cue-0.5.1/motley_cue/mapper/token_manager.py` & `motley_cue-0.5.3/motley_cue/mapper/token_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -303,18 +303,18 @@
             tablename="tokenmap",
             flag="c",
             encode=self._encrypted_encode,
             decode=self._encrypted_decode,
         )
 
     def _encrypted_encode(self, obj):
-        return self.encryption.encrypt(json.dumps(obj))
+        return sqlite3.Binary(self.encryption.encrypt(json.dumps(obj)).encode("utf-8"))
 
     def _encrypted_decode(self, obj):
-        return json.loads(self.encryption.decrypt(obj))
+        return json.loads(self.encryption.decrypt(obj.decode("utf-8")))
 
     def pop(self, otp: str) -> Optional[str]:
         token = None
         if otp in self.database:
             token = str(self.database[otp])
             del self.database[otp]
         self.database.commit()
```

### Comparing `motley_cue-0.5.1/motley_cue/models.py` & `motley_cue-0.5.3/motley_cue/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 """Definitions of API response models
 """
-from typing import Optional, Union, List
+from typing import Optional, Union, List, Dict
 from pydantic.dataclasses import dataclass
 from pydantic import Field
 
 from .mapper.authorisation import AuthorisationType
 
 
 @dataclass
+class InfoOp:
+    """Data model for responses on the /info/op endpoint."""
+
+    scopes: Optional[List[str]] = Field([], example=["openid", "profile", "email"])
+    audience: Optional[Union[str, List[str]]] = Field("", example="ssh_localhost")
+
+
+@dataclass
 class Info:
     """Data model for responses on the /info endpoint."""
 
     login_info: dict = Field(
         ...,
         example={
             "description": "Local SSH Test Service",
@@ -22,14 +30,27 @@
     supported_OPs: list = Field(  # pylint: disable=invalid-name
         ...,
         example=[
             "https://aai.egi.eu/oidc",
             "https://login.helmholtz.de/oauth2",
         ],
     )
+    ops_info: Dict[str, InfoOp] = Field(
+        {},
+        example={
+            "https://aai.egi.eu/oidc": {
+                "scopes": ["openid", "profile", "email"],
+                "audience": "ssh_localhost",
+            },
+            "https://login.helmholtz.de/oauth2": {
+                "scopes": ["openid", "profile", "email"],
+                "audience": "ssh_localhost",
+            },
+        },
+    )
 
 
 @dataclass
 class InfoAuthorisation:
     """Data model for responses on the /info/authorisation endpoint."""
 
     OP: str = Field(
@@ -44,22 +65,14 @@
     supported_VOs: Optional[list] = Field(
         [], example=["/wlcg"]
     )  # pylint: disable=invalid-name
     audience: Optional[Union[str, List[str]]] = Field("", example="ssh_localhost")
 
 
 @dataclass
-class InfoOp:
-    """Data model for responses on the /info/op endpoint."""
-
-    scopes: Optional[List[str]] = Field([], example=["openid", "profile", "email"])
-    audience: Optional[Union[str, List[str]]] = Field("", example="ssh_localhost")
-
-
-@dataclass
 class VerifyUser:
     """Data model for responses on the /verify_user endpoint."""
 
     state: str = Field(..., example="deployed")
     verified: bool = Field(..., example=True)
```

### Comparing `motley_cue-0.5.1/motley_cue/routers/admin.py` & `motley_cue-0.5.3/motley_cue/routers/admin.py`

 * *Files identical despite different names*

### Comparing `motley_cue-0.5.1/motley_cue/routers/user.py` & `motley_cue-0.5.3/motley_cue/routers/user.py`

 * *Files identical despite different names*

### Comparing `motley_cue-0.5.1/motley_cue/static.py` & `motley_cue-0.5.3/motley_cue/static.py`

 * *Files identical despite different names*

### Comparing `motley_cue-0.5.1/motley_cue.egg-info/PKG-INFO` & `motley_cue-0.5.3/motley_cue.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motley-cue
-Version: 0.5.1
+Version: 0.5.3
 Summary: Mapper Oidc To Local idEntitY with loCal User managEment
 Home-page: https://github.com/dianagudu/motley_cue
 Author: Diana Gudu
 Author-email: gudu@kit.edu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/dianagudu/motley_cue/issues
 Project-URL: Documentation, https://motley-cue.readthedocs.io
@@ -20,14 +20,15 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: System :: Systems Administration :: Authentication/Directory
 Classifier: Topic :: Utilities
 Description-Content-Type: text/x-rst
 
 .. image:: https://readthedocs.org/projects/motley-cue/badge/?version=latest
     :target: https://motley-cue.readthedocs.io/
```

### Comparing `motley_cue-0.5.1/motley_cue.egg-info/SOURCES.txt` & `motley_cue-0.5.3/motley_cue.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -40,17 +40,23 @@
 etc/templates/admin.deploy.update.template
 etc/templates/admin.test.template
 etc/templates/admin.update.template
 etc/templates/unknown.template
 etc/templates/user.deploy.template
 etc/templates/user.deploy.update.template
 etc/templates/user.update.template
+motley_cue/VERSION
 motley_cue.egg-info/PKG-INFO
 motley_cue.egg-info/SOURCES.txt
 motley_cue.egg-info/dependency_links.txt
 motley_cue.egg-info/entry_points.txt
 motley_cue.egg-info/requires.txt
 motley_cue.egg-info/top_level.txt
 selinux/README.md
 selinux/motley-cue-gunicorn.te
 selinux/motley-cue-nginx.te
-selinux/motley-cue-sshd.te
+selinux/motley-cue-sshd.te
+tests/test_api.py
+tests/test_authorisation.py
+tests/test_config.py
+tests/test_local_user_manager.py
+tests/test_token_manager.py
```

### Comparing `motley_cue-0.5.1/selinux/motley-cue-gunicorn.te` & `motley_cue-0.5.3/selinux/motley-cue-gunicorn.te`

 * *Files identical despite different names*

### Comparing `motley_cue-0.5.1/setup.cfg` & `motley_cue-0.5.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 	Natural Language :: English
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: System :: Systems Administration
 	Topic :: System :: Systems Administration :: Authentication/Directory
 	Topic :: Utilities
 
 [options.entry_points]
 console_scripts = 
 	motley_cue_uvicorn = motley_cue.__main__:main
```

### Comparing `motley_cue-0.5.1/tests/configs.py` & `motley_cue-0.5.3/tests/configs.py`

 * *Files identical despite different names*

### Comparing `motley_cue-0.5.1/tests/conftest.py` & `motley_cue-0.5.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `motley_cue-0.5.1/tests/test_api.py` & `motley_cue-0.5.3/tests/test_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,17 @@
         (CONFIG_NOT_SUPPORTED, []),
     ],
     ids=[*CONFIGS_AUTHENTICATED_USERS.keys(), "NOT_SUPPORTED"],
 )
 @pytest.mark.parametrize("method_to_patch,callback", [("", Info.callback_valid)])
 def test_info_endpoint(test_api, supported_ops):
     response = test_api.get(Info.url)
-    assert [url.rstrip("/") for url in response.json()["supported_OPs"]] == supported_ops
+    assert [
+        url.rstrip("/") for url in response.json()["supported_OPs"]
+    ] == supported_ops
 
 
 @pytest.mark.parametrize(
     "config_file",
     [
         *CONFIGS_AUTHENTICATED_USERS.values(),
         CONFIG_NOT_SUPPORTED,
```

### Comparing `motley_cue-0.5.1/tests/test_authorisation.py` & `motley_cue-0.5.3/tests/test_authorisation.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,41 +27,45 @@
     ids=CONFIGS_AUTHENTICATED_USERS.keys(),
 )
 def test_info_authorisation(test_authorisation):
     response = test_authorisation.info(MOCK_REQUEST)
     assert set(InfoAuthorisation.valid_response.keys()) <= set(response.keys())
 
 
-@pytest.mark.parametrize("config_file", [CONFIGS["NOT_SUPPORTED"]], ids=["NOT_SUPPORTED"])
+@pytest.mark.parametrize(
+    "config_file", [CONFIGS["NOT_SUPPORTED"]], ids=["NOT_SUPPORTED"]
+)
 def test_info_authorisation_not_supported(test_authorisation, test_unauthorised):
     with pytest.raises(test_unauthorised):
         test_authorisation.info(MOCK_REQUEST)
 
 
 @pytest.mark.parametrize(
     "config_file",
     CONFIGS_AUTHORISED_USERS.values(),
     ids=CONFIGS_AUTHORISED_USERS.keys(),
 )
 async def test_require_authorised_user_success(test_authorisation):
-    assert await test_authorisation.authorised_user_required(view_func)(request=MOCK_REQUEST) == {
-        "message": "Success"
-    }
+    assert await test_authorisation.authorised_user_required(view_func)(
+        request=MOCK_REQUEST
+    ) == {"message": "Success"}
 
 
 @pytest.mark.parametrize(
     "config_file,status_code",
     [
         (CONFIGS["SUPPORTED_NOT_AUTHORISED"], 403),
         (CONFIGS["NOT_SUPPORTED"], 401),
     ],
     ids=["SUPPORTED_NOT_AUTHORISED", "NOT_SUPPORTED"],
 )
 async def test_require_authorised_user_fail(test_authorisation, status_code):
-    response = await test_authorisation.authorised_user_required(view_func)(request=MOCK_REQUEST)
+    response = await test_authorisation.authorised_user_required(view_func)(
+        request=MOCK_REQUEST
+    )
     assert response.status_code == status_code
 
 
 @pytest.mark.parametrize("config_file", CONFIGS.values(), ids=CONFIGS.keys())
 async def test_require_authorised_user_bad_request(test_authorisation):
     response = await test_authorisation.authorised_user_required(view_func)(
         request=MOCK_BAD_REQUEST
@@ -118,17 +122,21 @@
 )
 async def test_require_authenticated_user_success(test_authorisation):
     assert await test_authorisation.authenticated_user_required(view_func)(
         request=MOCK_REQUEST
     ) == {"message": "Success"}
 
 
-@pytest.mark.parametrize("config_file", [CONFIGS["NOT_SUPPORTED"]], ids=["NOT_SUPPORTED"])
+@pytest.mark.parametrize(
+    "config_file", [CONFIGS["NOT_SUPPORTED"]], ids=["NOT_SUPPORTED"]
+)
 async def test_require_authenticated_user_fail(test_authorisation):
-    response = await test_authorisation.authenticated_user_required(view_func)(request=MOCK_REQUEST)
+    response = await test_authorisation.authenticated_user_required(view_func)(
+        request=MOCK_REQUEST
+    )
     assert response.status_code == 401
 
 
 @pytest.mark.parametrize("config_file", CONFIGS.values(), ids=CONFIGS.keys())
 async def test_require_authenticated_user_bad_request(test_authorisation):
     response = await test_authorisation.authenticated_user_required(view_func)(
         request=MOCK_BAD_REQUEST
@@ -138,23 +146,30 @@
 
 @pytest.mark.parametrize(
     "config_file",
     CONFIGS_AUTHENTICATED_USERS.values(),
     ids=CONFIGS_AUTHENTICATED_USERS.keys(),
 )
 def test_get_user_infos_from_access_token_success(test_authorisation):
-    response = test_authorisation.get_user_infos_from_access_token(access_token=MOCK_TOKEN)
+    response = test_authorisation.get_user_infos_from_access_token(
+        access_token=MOCK_TOKEN
+    )
     assert response.subject == MOCK_SUB
     assert response.issuer == MOCK_ISS
 
 
 @pytest.mark.parametrize("config_file", CONFIGS.values(), ids=CONFIGS.keys())
 def test_get_user_infos_from_access_token_fail(test_authorisation):
-    assert test_authorisation.get_user_infos_from_access_token(access_token="bad token") == None
-    assert test_authorisation.get_user_infos_from_access_token(access_token=None) == None
+    assert (
+        test_authorisation.get_user_infos_from_access_token(access_token="bad token")
+        == None
+    )
+    assert (
+        test_authorisation.get_user_infos_from_access_token(access_token=None) == None
+    )
 
 
 @pytest.mark.parametrize(
     "config_file",
     CONFIGS_AUTHENTICATED_USERS.values(),
     ids=CONFIGS_AUTHENTICATED_USERS.keys(),
 )
```

### Comparing `motley_cue-0.5.1/tests/test_config.py` & `motley_cue-0.5.3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `motley_cue-0.5.1/tests/test_local_user_manager.py` & `motley_cue-0.5.3/tests/test_local_user_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,17 @@
 )
 def test_admin_suspend_success(test_local_user_manager_patched):
     response = test_local_user_manager_patched.admin_suspend(sub=MOCK_SUB, iss=MOCK_ISS)
     assert set(response.keys()) == set(["state", "message"])
 
 
 @pytest.mark.parametrize("mocker", [mock_exception()])
-def test_admin_suspend_fail(test_local_user_manager_patched, test_internal_server_error):
+def test_admin_suspend_fail(
+    test_local_user_manager_patched, test_internal_server_error
+):
     with pytest.raises(test_internal_server_error):
         test_local_user_manager_patched.admin_suspend(sub=MOCK_SUB, iss=MOCK_ISS)
 
 
 @pytest.mark.parametrize(
     "mocker",
     [
@@ -144,26 +146,31 @@
             for state in ["deployed", "suspended", "limited", "pending"]
         ],
         *[
             (mock_status_result(state=state, username="same_user"), username, False)
             for state in ["deployed", "suspended", "limited", "pending"]
             for username in ["not_same_user", "", None]
         ],
-        *[(mock_not_deployed_result(), username, False) for username in ["user", "", None]],
+        *[
+            (mock_not_deployed_result(), username, False)
+            for username in ["user", "", None]
+        ],
         *[
             (mock_status_result(state="rejected"), username, False)
             for username in ["user", "", None]
         ],
         *[
             (mock_status_result(state="unknown"), username, False)
             for username in ["user", "", None]
         ],
     ],
 )
-def test_verify_user_success(test_local_user_manager_patched, username: str, verified: bool):
+def test_verify_user_success(
+    test_local_user_manager_patched, username: str, verified: bool
+):
     response = test_local_user_manager_patched.verify_user({}, username)
     assert set(response.keys()) == set(["state", "verified"])
     assert response["verified"] == verified
 
 
 @pytest.mark.parametrize(
     "mocker,username",
@@ -198,11 +205,13 @@
             ]
         ],
         mock_failure(),
         mock_rejection(),
         mock_exception(),
     ],
 )
-def test_reach_state_no_userinfo(test_local_user_manager_patched, test_internal_server_error):
+def test_reach_state_no_userinfo(
+    test_local_user_manager_patched, test_internal_server_error
+):
     with pytest.raises(test_internal_server_error):
         state = 0  # any number (of State type)
         test_local_user_manager_patched._reach_state(None, state)
```

### Comparing `motley_cue-0.5.1/tests/test_token_manager.py` & `motley_cue-0.5.3/tests/test_token_manager.py`

 * *Files identical despite different names*

### Comparing `motley_cue-0.5.1/tests/utils.py` & `motley_cue-0.5.3/tests/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         self.mapper_method = mapper_method
         self.valid_response = valid_response
         self.callback_valid = lambda *x: valid_response
 
 
 Info = Endpoint(
     url="/info",
-    valid_response={"login_info": "", "supported_OPs": []},
+    valid_response={"login_info": "", "supported_OPs": [], "ops_info": {}},
     mapper_method="info",
 )
 
 InfoAuthorisation = Endpoint(
     url="/info/authorisation",
     valid_response={"OP": "", "authorisation_type": "", "authorisation_info": ""},
     mapper_method="info_authorisation",
@@ -109,15 +109,17 @@
 Root = Endpoint(
     url="/",
     valid_response={"description": "", "endpoints": {}, "usage": ""},
     children=[Info, InfoAuthorisation, InfoOp, User, Admin, VerifyUser],
 )
 
 
-def getListOfEndpoints(endpoint: Endpoint, condition: Callable[[Endpoint], bool]) -> List[Endpoint]:
+def getListOfEndpoints(
+    endpoint: Endpoint, condition: Callable[[Endpoint], bool]
+) -> List[Endpoint]:
     """Returns a list of endpoints that satisfy a given condition,
     from the subtree starting at the given endpoint"""
     endpoints = []
     if condition(endpoint):
         endpoints += [endpoint]
     if endpoint.children:
         for child in endpoint.children:
```

