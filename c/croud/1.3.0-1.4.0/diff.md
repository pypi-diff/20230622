# Comparing `tmp/croud-1.3.0.tar.gz` & `tmp/croud-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "croud-1.3.0.tar", last modified: Tue Mar 14 10:02:32 2023, max compression
+gzip compressed data, was "croud-1.4.0.tar", last modified: Thu Jun 22 13:31:19 2023, max compression
```

## Comparing `croud-1.3.0.tar` & `croud-1.4.0.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:02:32.104761 croud-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    12601 2023-03-14 10:02:25.000000 croud-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-03-14 10:02:32.104761 croud-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-03-14 10:02:25.000000 croud-1.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:02:32.092760 croud-1.3.0/croud/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-14 10:02:25.000000 croud-1.3.0/croud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44512 2023-03-14 10:02:25.000000 croud-1.3.0/croud/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-03-14 10:02:25.000000 croud-1.3.0/croud/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:02:32.096760 croud-1.3.0/croud/apikeys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 10:02:25.000000 croud-1.3.0/croud/apikeys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-03-14 10:02:25.000000 croud-1.3.0/croud/apikeys/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:02:32.096760 croud-1.3.0/croud/clusters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 10:02:25.000000 croud-1.3.0/croud/clusters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20928 2023-03-14 10:02:25.000000 croud-1.3.0/croud/clusters/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-03-14 10:02:25.000000 croud-1.3.0/croud/clusters/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:02:32.096760 croud-1.3.0/croud/config/
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-03-14 10:02:25.000000 croud-1.3.0/croud/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-03-14 10:02:25.000000 croud-1.3.0/croud/config/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-03-14 10:02:25.000000 croud-1.3.0/croud/config/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-03-14 10:02:25.000000 croud-1.3.0/croud/config/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-03-14 10:02:25.000000 croud-1.3.0/croud/config/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-03-14 10:02:25.000000 croud-1.3.0/croud/config/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-03-14 10:02:25.000000 croud-1.3.0/croud/config/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:02:32.096760 croud-1.3.0/croud/consumers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 10:02:25.000000 croud-1.3.0/croud/consumers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-03-14 10:02:25.000000 croud-1.3.0/croud/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-03-14 10:02:25.000000 croud-1.3.0/croud/logout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-03-14 10:02:25.000000 croud-1.3.0/croud/me.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:02:32.096760 croud-1.3.0/croud/organizations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 10:02:25.000000 croud-1.3.0/croud/organizations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:02:32.096760 croud-1.3.0/croud/organizations/auditlogs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 10:02:25.000000 croud-1.3.0/croud/organizations/auditlogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-03-14 10:02:25.000000 croud-1.3.0/croud/organizations/auditlogs/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-03-14 10:02:25.000000 croud-1.3.0/croud/organizations/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:02:32.096760 croud-1.3.0/croud/organizations/users/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 10:02:25.000000 croud-1.3.0/croud/organizations/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-03-14 10:02:25.000000 croud-1.3.0/croud/organizations/users/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-03-14 10:02:25.000000 croud-1.3.0/croud/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-03-14 10:02:25.000000 croud-1.3.0/croud/printer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:02:32.096760 croud-1.3.0/croud/products/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 10:02:25.000000 croud-1.3.0/croud/products/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-03-14 10:02:25.000000 croud-1.3.0/croud/products/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:02:32.100761 croud-1.3.0/croud/projects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 10:02:25.000000 croud-1.3.0/croud/projects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-03-14 10:02:25.000000 croud-1.3.0/croud/projects/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:02:32.100761 croud-1.3.0/croud/projects/users/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 10:02:25.000000 croud-1.3.0/croud/projects/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-03-14 10:02:25.000000 croud-1.3.0/croud/projects/users/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:02:32.100761 croud-1.3.0/croud/regions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 10:02:25.000000 croud-1.3.0/croud/regions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-03-14 10:02:25.000000 croud-1.3.0/croud/regions/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-03-14 10:02:25.000000 croud-1.3.0/croud/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:02:32.100761 croud-1.3.0/croud/subscriptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 10:02:25.000000 croud-1.3.0/croud/subscriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-03-14 10:02:25.000000 croud-1.3.0/croud/subscriptions/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:02:32.100761 croud-1.3.0/croud/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 10:02:25.000000 croud-1.3.0/croud/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-03-14 10:02:25.000000 croud-1.3.0/croud/tools/spinner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-03-14 10:02:25.000000 croud-1.3.0/croud/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:02:32.100761 croud-1.3.0/croud/users/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 10:02:25.000000 croud-1.3.0/croud/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-03-14 10:02:25.000000 croud-1.3.0/croud/users/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:02:32.100761 croud-1.3.0/croud/users/roles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 10:02:25.000000 croud-1.3.0/croud/users/roles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-03-14 10:02:25.000000 croud-1.3.0/croud/users/roles/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-03-14 10:02:25.000000 croud-1.3.0/croud/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:02:32.096760 croud-1.3.0/croud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-03-14 10:02:32.000000 croud-1.3.0/croud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-03-14 10:02:32.000000 croud-1.3.0/croud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 10:02:32.000000 croud-1.3.0/croud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-14 10:02:32.000000 croud-1.3.0/croud.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-14 10:02:32.000000 croud-1.3.0/croud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-14 10:02:32.000000 croud-1.3.0/croud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-03-14 10:02:32.104761 croud-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-03-14 10:02:25.000000 croud-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:02:32.100761 croud-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 10:02:25.000000 croud-1.3.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:02:32.104761 croud-1.3.0/tests/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 10:02:25.000000 croud-1.3.0/tests/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-03-14 10:02:25.000000 croud-1.3.0/tests/commands/test_api_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)    41091 2023-03-14 10:02:25.000000 croud-1.3.0/tests/commands/test_clusters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-03-14 10:02:25.000000 croud-1.3.0/tests/commands/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-03-14 10:02:25.000000 croud-1.3.0/tests/commands/test_login.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-03-14 10:02:25.000000 croud-1.3.0/tests/commands/test_logout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-03-14 10:02:25.000000 croud-1.3.0/tests/commands/test_me.py
--rw-r--r--   0 runner    (1001) docker     (123)    11702 2023-03-14 10:02:25.000000 croud-1.3.0/tests/commands/test_organizations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-03-14 10:02:25.000000 croud-1.3.0/tests/commands/test_products.py
--rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-03-14 10:02:25.000000 croud-1.3.0/tests/commands/test_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)    10493 2023-03-14 10:02:25.000000 croud-1.3.0/tests/commands/test_regions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-03-14 10:02:25.000000 croud-1.3.0/tests/commands/test_subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-03-14 10:02:25.000000 croud-1.3.0/tests/commands/test_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-03-14 10:02:25.000000 croud-1.3.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-03-14 10:02:25.000000 croud-1.3.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-03-14 10:02:25.000000 croud-1.3.0/tests/test_config_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-03-14 10:02:25.000000 croud-1.3.0/tests/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-03-14 10:02:25.000000 croud-1.3.0/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8140 2023-03-14 10:02:25.000000 croud-1.3.0/tests/test_printer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-03-14 10:02:25.000000 croud-1.3.0/tests/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-03-14 10:02:25.000000 croud-1.3.0/tests/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:02:32.104761 croud-1.3.0/tests/util/
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-03-14 10:02:25.000000 croud-1.3.0/tests/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-03-14 10:02:25.000000 croud-1.3.0/tests/util/fake_cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:19.125494 croud-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    12601 2023-06-22 13:31:14.000000 croud-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-22 13:31:19.125494 croud-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-22 13:31:14.000000 croud-1.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:19.117494 croud-1.4.0/croud/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-22 13:31:14.000000 croud-1.4.0/croud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48294 2023-06-22 13:31:14.000000 croud-1.4.0/croud/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-06-22 13:31:14.000000 croud-1.4.0/croud/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:19.117494 croud-1.4.0/croud/apikeys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:14.000000 croud-1.4.0/croud/apikeys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-06-22 13:31:14.000000 croud-1.4.0/croud/apikeys/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:19.117494 croud-1.4.0/croud/clusters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:14.000000 croud-1.4.0/croud/clusters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22712 2023-06-22 13:31:14.000000 croud-1.4.0/croud/clusters/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-22 13:31:14.000000 croud-1.4.0/croud/clusters/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:19.121494 croud-1.4.0/croud/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-06-22 13:31:14.000000 croud-1.4.0/croud/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-06-22 13:31:14.000000 croud-1.4.0/croud/config/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-06-22 13:31:14.000000 croud-1.4.0/croud/config/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-22 13:31:14.000000 croud-1.4.0/croud/config/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-06-22 13:31:14.000000 croud-1.4.0/croud/config/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-22 13:31:14.000000 croud-1.4.0/croud/config/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-22 13:31:14.000000 croud-1.4.0/croud/config/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:19.121494 croud-1.4.0/croud/consumers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:14.000000 croud-1.4.0/croud/consumers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-06-22 13:31:14.000000 croud-1.4.0/croud/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-22 13:31:14.000000 croud-1.4.0/croud/logout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-22 13:31:14.000000 croud-1.4.0/croud/me.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:19.121494 croud-1.4.0/croud/organizations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:14.000000 croud-1.4.0/croud/organizations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:19.121494 croud-1.4.0/croud/organizations/auditlogs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:14.000000 croud-1.4.0/croud/organizations/auditlogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-06-22 13:31:14.000000 croud-1.4.0/croud/organizations/auditlogs/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6741 2023-06-22 13:31:14.000000 croud-1.4.0/croud/organizations/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:19.121494 croud-1.4.0/croud/organizations/users/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:14.000000 croud-1.4.0/croud/organizations/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-06-22 13:31:14.000000 croud-1.4.0/croud/organizations/users/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-06-22 13:31:14.000000 croud-1.4.0/croud/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-06-22 13:31:14.000000 croud-1.4.0/croud/printer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:19.121494 croud-1.4.0/croud/products/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:14.000000 croud-1.4.0/croud/products/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-22 13:31:14.000000 croud-1.4.0/croud/products/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:19.121494 croud-1.4.0/croud/projects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:14.000000 croud-1.4.0/croud/projects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-06-22 13:31:14.000000 croud-1.4.0/croud/projects/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:19.121494 croud-1.4.0/croud/projects/users/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:14.000000 croud-1.4.0/croud/projects/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-06-22 13:31:14.000000 croud-1.4.0/croud/projects/users/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:19.121494 croud-1.4.0/croud/regions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:14.000000 croud-1.4.0/croud/regions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-06-22 13:31:14.000000 croud-1.4.0/croud/regions/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-06-22 13:31:14.000000 croud-1.4.0/croud/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:19.121494 croud-1.4.0/croud/subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:14.000000 croud-1.4.0/croud/subscriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-06-22 13:31:14.000000 croud-1.4.0/croud/subscriptions/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:19.121494 croud-1.4.0/croud/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:14.000000 croud-1.4.0/croud/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-22 13:31:14.000000 croud-1.4.0/croud/tools/spinner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-22 13:31:14.000000 croud-1.4.0/croud/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:19.121494 croud-1.4.0/croud/users/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:14.000000 croud-1.4.0/croud/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-22 13:31:14.000000 croud-1.4.0/croud/users/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:19.121494 croud-1.4.0/croud/users/roles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:14.000000 croud-1.4.0/croud/users/roles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-06-22 13:31:14.000000 croud-1.4.0/croud/users/roles/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-06-22 13:31:14.000000 croud-1.4.0/croud/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:19.117494 croud-1.4.0/croud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-22 13:31:19.000000 croud-1.4.0/croud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-06-22 13:31:19.000000 croud-1.4.0/croud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 13:31:19.000000 croud-1.4.0/croud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-22 13:31:19.000000 croud-1.4.0/croud.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-22 13:31:19.000000 croud-1.4.0/croud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-22 13:31:19.000000 croud-1.4.0/croud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-22 13:31:19.125494 croud-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-06-22 13:31:14.000000 croud-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:19.125494 croud-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:14.000000 croud-1.4.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:19.125494 croud-1.4.0/tests/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:14.000000 croud-1.4.0/tests/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-22 13:31:14.000000 croud-1.4.0/tests/commands/test_api_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43174 2023-06-22 13:31:14.000000 croud-1.4.0/tests/commands/test_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-06-22 13:31:14.000000 croud-1.4.0/tests/commands/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-06-22 13:31:14.000000 croud-1.4.0/tests/commands/test_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-06-22 13:31:14.000000 croud-1.4.0/tests/commands/test_logout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-22 13:31:14.000000 croud-1.4.0/tests/commands/test_me.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13172 2023-06-22 13:31:14.000000 croud-1.4.0/tests/commands/test_organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-06-22 13:31:14.000000 croud-1.4.0/tests/commands/test_products.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-06-22 13:31:14.000000 croud-1.4.0/tests/commands/test_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10493 2023-06-22 13:31:14.000000 croud-1.4.0/tests/commands/test_regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-06-22 13:31:14.000000 croud-1.4.0/tests/commands/test_subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-06-22 13:31:14.000000 croud-1.4.0/tests/commands/test_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-06-22 13:31:14.000000 croud-1.4.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-06-22 13:31:14.000000 croud-1.4.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-06-22 13:31:14.000000 croud-1.4.0/tests/test_config_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-06-22 13:31:14.000000 croud-1.4.0/tests/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-06-22 13:31:14.000000 croud-1.4.0/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8140 2023-06-22 13:31:14.000000 croud-1.4.0/tests/test_printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-22 13:31:14.000000 croud-1.4.0/tests/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-06-22 13:31:14.000000 croud-1.4.0/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:19.125494 croud-1.4.0/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-06-22 13:31:14.000000 croud-1.4.0/tests/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-06-22 13:31:14.000000 croud-1.4.0/tests/util/fake_cloud.py
```

### Comparing `croud-1.3.0/LICENSE` & `croud-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `croud-1.3.0/PKG-INFO` & `croud-1.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: croud
-Version: 1.3.0
+Version: 1.4.0
 Summary: A command line interface for CrateDB Cloud
 Home-page: https://github.com/crate/croud
 Author: Crate.io
 Author-email: office@crate.io
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `croud-1.3.0/README.rst` & `croud-1.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `croud-1.3.0/croud/__init__.py` & `croud-1.4.0/croud/__init__.py`

 * *Files identical despite different names*

### Comparing `croud-1.3.0/croud/__main__.py` & `croud-1.4.0/croud/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,16 @@
     clusters_set_deletion_protection,
     clusters_set_ip_whitelist,
     clusters_set_product,
     clusters_set_suspended,
     clusters_snapshots_list,
     clusters_snapshots_restore,
     clusters_upgrade,
-    import_jobs_create,
+    import_jobs_create_from_file,
+    import_jobs_create_from_url,
     import_jobs_delete,
     import_jobs_list,
 )
 from croud.config import CONFIG
 from croud.config.commands import (
     config_add_profile,
     config_current_profile,
@@ -60,14 +61,17 @@
     config_show,
 )
 from croud.login import login
 from croud.logout import logout
 from croud.me import me, me_edit
 from croud.organizations.auditlogs.commands import auditlogs_list
 from croud.organizations.commands import (
+    org_files_create,
+    org_files_delete,
+    org_files_list,
     organizations_create,
     organizations_delete,
     organizations_edit,
     organizations_get,
     organizations_list,
 )
 from croud.organizations.users.commands import (
@@ -97,14 +101,51 @@
     subscriptions_get,
     subscriptions_list,
 )
 from croud.tools.spinner import HALO
 from croud.users.commands import users_list
 from croud.users.roles.commands import roles_list
 
+# Arguments common to all import-job create commands
+import_job_create_common_args = [
+    Argument(
+        "--cluster-id",
+        type=str,
+        required=True,
+        help="The cluster the data will be imported into.",
+    ),
+    Argument(
+        "--file-format",
+        type=str,
+        required=True,
+        choices=["csv", "json", "parquet"],
+        help="The format of the structured data in the file.",
+    ),
+    Argument(
+        "--compression",
+        type=str,
+        required=False,
+        choices=["gzip"],
+        help="The compression method the file uses.",
+    ),
+    Argument(
+        "--table",
+        type=str,
+        required=True,
+        help="The table the data will be imported into.",
+    ),
+    Argument(
+        "--create-table",
+        type=lambda x: bool(strtobool(str(x))),  # noqa
+        required=False,
+        help="Whether the table should be created automatically"
+        " if it does not exist.",
+    ),
+]
+
 # fmt: off
 command_tree = {
     "me": {
         "help": "Print information about the current logged in user.",
         "resolver": me,
         "commands": {
             "edit": {
@@ -621,15 +662,15 @@
                                 help="The repository that contains the snapshot to be "
                                      "restored.",
                             ),
                             Argument(
                                 "--source-cluster-id", type=str, required=False,
                                 help="The CrateDB cluster ID of the snapshot to be "
                                      "used belongs to. Must belong to the same "
-                                     "organization as the target cluster."
+                                     "organization as the target cluster. "
                                      "If not specified the ``--cluster-id`` CrateDB"
                                      " cluster will be used as the source.",
                             ),
                             Argument(
                                 "--tables", type=str, required=False,
                                 help="The list of tables to restore, comma separated. "
                                      "If not specified all tables will be restored.",
@@ -669,50 +710,53 @@
                                 help="The cluster the import jobs belong to."
                             ),
                         ],
                         "resolver": import_jobs_list,
                     },
                     "create": {
                         "help": "Create a data import job for the specified cluster.",
-                        "extra_args": [
-                            Argument(
-                                "--cluster-id", type=str, required=True,
-                                help="The cluster the data will be imported into."
-                            ),
-                            Argument(
-                                "--type", type=str, required=True, choices=["url"],
-                                help="The type of import job that will be created."
-                            ),
-                            Argument(
-                                "--url", type=str, required=True,
-                                help="When type is URL, the URL the import file will "
-                                     "be read from."
-                            ),
-                            Argument(
-                                "--file-format", type=str, required=True,
-                                choices=["csv", "json", "parquet"],
-                                help="The format of the structured data in the file."
-                            ),
-                            Argument(
-                                "--compression", type=str, required=False,
-                                choices=["gzip"],
-                                help="The compression method the file uses."
-                            ),
-                            Argument(
-                                "--table", type=str, required=True,
-                                help="The table the data will be imported into."
-                            ),
-                            Argument(
-                                "--create-table", type=lambda x: bool(strtobool(str(x))),  # noqa
-                                required=False,
-                                help="Whether the table should be created automatically"
-                                     " if it does not exist."
-                            )
-                        ],
-                        "resolver": import_jobs_create,
+                        "commands" : {
+                            "from-url": {
+                                "help": "Create a data import job on the specified "
+                                        "cluster from a url.",
+                                "extra_args": [
+                                    # Type URL params
+                                    Argument(
+                                        "--url", type=str, required=True,
+                                        help="The URL the import file will be read "
+                                             "from."
+                                    ),
+                                ] + import_job_create_common_args,
+                                "resolver": import_jobs_create_from_url,
+                            },
+                            "from-file": {
+                                "help": "Create a data import job on the specified "
+                                        "cluster from a file.",
+                                "extra_args": [
+                                    # Type file params
+                                    Argument(
+                                        "--file-id", type=str, required=False,
+                                        help="The file ID that will be used for the "
+                                             "import. If not specified then --file-path"
+                                             " must be specified. "
+                                             "Please refer to `croud organizations "
+                                             "files` for more info."
+                                    ),
+                                    Argument(
+                                        "--file-path", type=str, required=False,
+                                        help="The file in your local filesystem that "
+                                             "will be used. If not specified then "
+                                             "--file-id must be specified. "
+                                             "Please note the file will become visible "
+                                             "under `croud organizations files list`."
+                                    ),
+                                ] + import_job_create_common_args,
+                                "resolver": import_jobs_create_from_file,
+                            },
+                        },
                     },
                 },
             },
         },
     },
     "products": {
         "help": "Manage Products.",
@@ -867,14 +911,63 @@
                                 help="The organization ID to use.",
                             ),
                         ],
                         "resolver": org_users_remove,
                     },
                 },
             },
+            "files": {
+                "help": "Manage organization's files.",
+                "commands": {
+                    "list": {
+                        "help": "List all files uploaded to this organization.",
+                        "extra_args": [
+                            Argument(
+                                "--org-id", type=str, required=True,
+                                help="The organization ID to use.",
+                            ),
+                        ],
+                        "resolver": org_files_list,
+                    },
+                    "create": {
+                        "help": "Uploads a new file to the organization.",
+                        "extra_args": [
+                            Argument(
+                                "--org-id", type=str, required=True,
+                                help="The organization ID to use.",
+                            ),
+                            Argument(
+                                "--file-path", type=str, required=True,
+                                help="The local file to be uploaded.",
+                            ),
+                            Argument(
+                                "--name", type=str, required=False,
+                                help="The name that will be displayed when listing the "
+                                     "file. If not provided, the file name will be "
+                                     "used.",
+                            ),
+                        ],
+                        "resolver": org_files_create,
+                    },
+                    "delete": {
+                        "help": "Deletes a previously uploaded file.",
+                        "extra_args": [
+                            Argument(
+                                "--org-id", type=str, required=True,
+                                help="The organization ID to use.",
+                            ),
+                            Argument(
+                                "--file-id", type=str, required=True,
+                                help="The ID of the file.",
+                            ),
+                        ],
+                        "resolver": org_files_delete,
+                    },
+                }
+            }
         },
     },
     "users": {
         "help": "Manage users.",
         "commands": {
             "list": {
                 "help": "List all users.",
```

### Comparing `croud-1.3.0/croud/api.py` & `croud-1.4.0/croud/api.py`

 * *Files identical despite different names*

### Comparing `croud-1.3.0/croud/apikeys/commands.py` & `croud-1.4.0/croud/apikeys/commands.py`

 * *Files identical despite different names*

### Comparing `croud-1.3.0/croud/clusters/commands.py` & `croud-1.4.0/croud/clusters/commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,21 +15,22 @@
 #
 # However, if you have executed another commercial license agreement
 # with Crate these terms will supersede the license and you may use the
 # software solely pursuant to the terms of the relevant commercial agreement.
 import time
 from argparse import Namespace
 from datetime import datetime, timedelta, timezone
-from typing import Dict, Optional
+from typing import Any, Dict, Optional
 
 import bitmath
 
 from croud.api import Client
 from croud.clusters.exceptions import AsyncOperationNotFound
 from croud.config import get_output_format
+from croud.organizations.commands import op_upload_file_to_org
 from croud.printer import print_error, print_info, print_response, print_success
 from croud.tools.spinner import HALO
 from croud.util import require_confirmation
 
 
 def clusters_get(args: Namespace) -> None:
     client = Client.from_args(args)
@@ -155,32 +156,85 @@
         data=data,
         errors=errors,
         keys=["id", "name", "num_nodes"],
         output_fmt=get_output_format(args),
     )
 
 
-def import_jobs_create(args: Namespace) -> None:
-    body = {
-        "type": args.type,
+def import_jobs_create_from_url(args: Namespace) -> None:
+    extra_body = {
         "url": {
             "url": args.url,
-        },
+        }
+    }
+    args.type = "url"
+    import_jobs_create(args, extra_payload=extra_body)
+
+
+def _get_org_id_from_cluster_id(client, cluster_id: str) -> Optional[str]:
+    data, errors = client.get(f"/api/v2/clusters/{cluster_id}/")
+    if errors or not data:
+        return None
+
+    project_id = data["project_id"]
+
+    data, errors = client.get(f"/api/v2/projects/{project_id}/")
+    if errors or not data:
+        return None
+
+    return data["organization_id"]
+
+
+def import_jobs_create_from_file(args: Namespace) -> None:
+    file_id = args.file_id
+
+    if not args.file_path and not args.file_id:
+        print_error("Please specify either --file-id or --file-path")
+        return
+
+    if args.file_path:
+        client = Client.from_args(args)
+        org_id = _get_org_id_from_cluster_id(client, args.cluster_id)
+        if not org_id:
+            print_error("Could not find the organization related to the cluster.")
+            return
+
+        data, errors = op_upload_file_to_org(client, org_id, args.file_path)
+        if errors or not data:
+            print_error("Aborted import job creation.")
+            return
+        file_id = data["id"]
+
+    extra_body = {
+        "file": {
+            "id": file_id,
+        }
+    }
+    args.type = "file"
+    import_jobs_create(args, extra_payload=extra_body)
+
+
+def import_jobs_create(args: Namespace, extra_payload: Dict[str, Any]) -> None:
+    body = {
+        "type": args.type,
         "format": args.file_format,
         "destination": {
             "table": args.table,
         },
     }
 
     if args.compression:
         body["compression"] = args.compression
 
     if args.create_table is not None:
         body["destination"]["create_table"] = args.create_table
 
+    if extra_payload:
+        body.update(extra_payload)
+
     client = Client.from_args(args)
     data, errors = client.post(
         f"/api/v2/clusters/{args.cluster_id}/import-jobs/", body=body
     )
     print_response(
         data=data,
         errors=errors,
@@ -234,16 +288,20 @@
 
 def import_jobs_list(args: Namespace) -> None:
     client = Client.from_args(args)
     data, errors = client.get(f"/api/v2/clusters/{args.cluster_id}/import-jobs/")
     print_response(
         data=data,
         errors=errors,
-        keys=["id", "cluster_id", "status", "type", "destination"],
+        keys=["id", "cluster_id", "status", "type", "url", "destination"],
         output_fmt=get_output_format(args),
+        transforms={
+            "url": lambda field: field.get("url"),
+            "destination": lambda field: field.get("table"),
+        },
     )
 
 
 def clusters_upgrade(args: Namespace) -> None:
     body = {"crate_version": args.version}
     client = Client.from_args(args)
     data, errors = client.put(f"/api/v2/clusters/{args.cluster_id}/upgrade/", body=body)
@@ -681,18 +739,21 @@
             feedback_func(status, feedback)
 
         # Final statuses
         if status == "SUCCEEDED":
             print_success("Operation completed.")
             break
         if status == "FAILED":
-            print_error(
-                "Your cluster operation has failed. "
-                "Our operations team is investigating the issue."
-            )
+            if msg:
+                print_error(msg)
+            else:
+                print_error(
+                    "Your cluster operation has failed. "
+                    "Our operations team is investigating the issue."
+                )
             break
 
         with HALO:
             time.sleep(10)
 
 
 def _lookup_organization_id_for_project(
```

### Comparing `croud-1.3.0/croud/clusters/exceptions.py` & `croud-1.4.0/croud/clusters/exceptions.py`

 * *Files identical despite different names*

### Comparing `croud-1.3.0/croud/config/__init__.py` & `croud-1.4.0/croud/config/__init__.py`

 * *Files identical despite different names*

### Comparing `croud-1.3.0/croud/config/commands.py` & `croud-1.4.0/croud/config/commands.py`

 * *Files identical despite different names*

### Comparing `croud-1.3.0/croud/config/configuration.py` & `croud-1.4.0/croud/config/configuration.py`

 * *Files identical despite different names*

### Comparing `croud-1.3.0/croud/config/exceptions.py` & `croud-1.4.0/croud/config/exceptions.py`

 * *Files identical despite different names*

### Comparing `croud-1.3.0/croud/config/schemas.py` & `croud-1.4.0/croud/config/schemas.py`

 * *Files identical despite different names*

### Comparing `croud-1.3.0/croud/config/types.py` & `croud-1.4.0/croud/config/types.py`

 * *Files identical despite different names*

### Comparing `croud-1.3.0/croud/config/util.py` & `croud-1.4.0/croud/config/util.py`

 * *Files identical despite different names*

### Comparing `croud-1.3.0/croud/login.py` & `croud-1.4.0/croud/login.py`

 * *Files identical despite different names*

### Comparing `croud-1.3.0/croud/logout.py` & `croud-1.4.0/croud/logout.py`

 * *Files identical despite different names*

### Comparing `croud-1.3.0/croud/me.py` & `croud-1.4.0/croud/me.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     """
 
     client = Client.from_args(args)
     data, errors = client.get("/api/v2/users/me/")
     print_response(
         data=data,
         errors=errors,
-        keys=["email", "username"],
+        keys=["email", "username", "idp"],
         output_fmt=get_output_format(args),
     )
 
 
 def me_edit(args: Namespace) -> None:
     """
     Lets the user edit their data
```

### Comparing `croud-1.3.0/croud/organizations/auditlogs/commands.py` & `croud-1.4.0/croud/organizations/auditlogs/commands.py`

 * *Files identical despite different names*

### Comparing `croud-1.3.0/croud/organizations/users/commands.py` & `croud-1.4.0/croud/organizations/users/commands.py`

 * *Files identical despite different names*

### Comparing `croud-1.3.0/croud/parser.py` & `croud-1.4.0/croud/parser.py`

 * *Files identical despite different names*

### Comparing `croud-1.3.0/croud/printer.py` & `croud-1.4.0/croud/printer.py`

 * *Files identical despite different names*

### Comparing `croud-1.3.0/croud/products/commands.py` & `croud-1.4.0/croud/products/commands.py`

 * *Files identical despite different names*

### Comparing `croud-1.3.0/croud/projects/commands.py` & `croud-1.4.0/croud/projects/commands.py`

 * *Files identical despite different names*

### Comparing `croud-1.3.0/croud/projects/users/commands.py` & `croud-1.4.0/croud/projects/users/commands.py`

 * *Files identical despite different names*

### Comparing `croud-1.3.0/croud/regions/commands.py` & `croud-1.4.0/croud/regions/commands.py`

 * *Files identical despite different names*

### Comparing `croud-1.3.0/croud/server.py` & `croud-1.4.0/croud/server.py`

 * *Files identical despite different names*

### Comparing `croud-1.3.0/croud/subscriptions/commands.py` & `croud-1.4.0/croud/subscriptions/commands.py`

 * *Files identical despite different names*

### Comparing `croud-1.3.0/croud/typing.py` & `croud-1.4.0/croud/typing.py`

 * *Files identical despite different names*

### Comparing `croud-1.3.0/croud/users/commands.py` & `croud-1.4.0/croud/users/commands.py`

 * *Files identical despite different names*

### Comparing `croud-1.3.0/croud/users/roles/commands.py` & `croud-1.4.0/croud/users/roles/commands.py`

 * *Files identical despite different names*

### Comparing `croud-1.3.0/croud/util.py` & `croud-1.4.0/croud/util.py`

 * *Files identical despite different names*

### Comparing `croud-1.3.0/croud.egg-info/PKG-INFO` & `croud-1.4.0/croud.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: croud
-Version: 1.3.0
+Version: 1.4.0
 Summary: A command line interface for CrateDB Cloud
 Home-page: https://github.com/crate/croud
 Author: Crate.io
 Author-email: office@crate.io
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `croud-1.3.0/croud.egg-info/SOURCES.txt` & `croud-1.4.0/croud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `croud-1.3.0/setup.py` & `croud-1.4.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # However, if you have executed another commercial license agreement
 # with Crate these terms will supersede the license and you may use the
 # software solely pursuant to the terms of the relevant commercial agreement.
 
 from pkg_resources.extern.packaging.version import Version
 from setuptools import find_packages, setup
 
-__version__ = Version("1.3.0")
+__version__ = Version("1.4.0")
 
 try:
     with open("README.rst", "r", encoding="utf-8") as f:
         readme = f.read()
 except IOError:
     readme = ""
 
@@ -46,25 +46,26 @@
         "bitmath==1.3.3.1",
         "certifi",
         "colorama==0.4.6",
         "marshmallow==3.19.0",
         "pyyaml==6.0",
         "requests==2.28.2",
         "tabulate>=0.8,<1.0",
-        "yarl==1.8.2",
+        "yarl==1.9.2",
         "halo==0.0.31",
-        "shtab==1.5.8",
+        "shtab==1.6.1",
+        "tqdm==4.65.0",
     ],
     extras_require={
         "testing": [
             "tox==3.14.2",
             "pytest-freezegun==0.4.2",
         ],
         "development": [
-            "black==23.1.0",
+            "black==23.3.0",
             "flake8==3.8.4",
             "isort==5.12.0",
             "mypy==0.812",
         ],
     },
     python_requires=">=3.7",
     classifiers=[
```

### Comparing `croud-1.3.0/tests/commands/test_api_keys.py` & `croud-1.4.0/tests/commands/test_api_keys.py`

 * *Files identical despite different names*

### Comparing `croud-1.3.0/tests/commands/test_clusters.py` & `croud-1.4.0/tests/commands/test_clusters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1385,25 +1385,24 @@
         f"/api/v2/clusters/{cluster_id}/import-jobs/{import_job_id}/",
     )
 
 
 @mock.patch.object(
     Client, "request", return_value=({"id": "1", "status": "SUCCEEDED"}, None)
 )
-def test_import_job_create(mock_request):
+def test_import_job_create_from_url(mock_request):
     cluster_id = gen_uuid()
     call_command(
         "croud",
         "clusters",
         "import-jobs",
         "create",
+        "from-url",
         "--cluster-id",
         cluster_id,
-        "--type",
-        "url",
         "--url",
         "http://download-url.com/csv-file.csv.gz",
         "--file-format",
         "csv",
         "--compression",
         "gzip",
         "--table",
@@ -1423,7 +1422,88 @@
     assert_rest(
         mock_request,
         RequestMethod.POST,
         f"/api/v2/clusters/{cluster_id}/import-jobs/",
         body=body,
         any_times=True,
     )
+
+
+@mock.patch.object(
+    Client, "request", return_value=({"id": "1", "status": "SUCCEEDED"}, None)
+)
+def test_import_job_create_from_file(mock_request):
+    cluster_id = gen_uuid()
+    file_uuid = gen_uuid()
+    call_command(
+        "croud",
+        "clusters",
+        "import-jobs",
+        "create",
+        "from-file",
+        "--cluster-id",
+        cluster_id,
+        "--file-id",
+        file_uuid,
+        "--file-format",
+        "csv",
+        "--compression",
+        "gzip",
+        "--table",
+        "my-table",
+        "--create-table",
+        "false",
+    )
+    body = {
+        "type": "file",
+        "file": {
+            "id": file_uuid,
+        },
+        "format": "csv",
+        "destination": {"table": "my-table", "create_table": False},
+        "compression": "gzip",
+    }
+    assert_rest(
+        mock_request,
+        RequestMethod.POST,
+        f"/api/v2/clusters/{cluster_id}/import-jobs/",
+        body=body,
+        any_times=True,
+    )
+
+
+@mock.patch.object(
+    Client,
+    "request",
+    return_value=(
+        [
+            {
+                "cluster_id": "123",
+                "compression": "gzip",
+                "dc": {
+                    "created": "2023-03-14T10:12:29.763000+00:00",
+                    "modified": "2023-03-14T10:12:29.763000+00:00",
+                },
+                "destination": {"create_table": True, "table": "croud-csv-import-two"},
+                "format": "csv",
+                "id": "a95e5a20-61f7-415f-b128-1e21ddf17513",
+                "progress": {
+                    "bytes": 0,
+                    "message": "Failed",
+                    "records": 0,
+                },
+                "status": "FAILED",
+                "type": "url",
+                "url": {"url": "https://some"},
+            }
+        ],
+        None,
+    ),
+)
+def test_import_job_list(mock_request):
+    call_command("croud", "clusters", "import-jobs", "list", "--cluster-id", "123")
+    assert_rest(
+        mock_request,
+        RequestMethod.GET,
+        "/api/v2/clusters/123/import-jobs/",
+        params=None,
+    )
```

### Comparing `croud-1.3.0/tests/commands/test_config.py` & `croud-1.4.0/tests/commands/test_config.py`

 * *Files identical despite different names*

### Comparing `croud-1.3.0/tests/commands/test_login.py` & `croud-1.4.0/tests/commands/test_login.py`

 * *Files identical despite different names*

### Comparing `croud-1.3.0/tests/commands/test_logout.py` & `croud-1.4.0/tests/commands/test_logout.py`

 * *Files identical despite different names*

### Comparing `croud-1.3.0/tests/commands/test_me.py` & `croud-1.4.0/tests/commands/test_me.py`

 * *Files identical despite different names*

### Comparing `croud-1.3.0/tests/commands/test_organizations.py` & `croud-1.4.0/tests/commands/test_organizations.py`

 * *Files 2% similar despite different names*

```diff
@@ -367,7 +367,65 @@
             {"organization_id": "org-1", "role_fqn": "organization_admin"},
             {"organization_id": "org-2", "role_fqn": "organization_member"},
             {"organization_id": "org-3", "role_fqn": "organization_member"},
         ]
     }
     response = organization_role_fqn_transform(user["organization_roles"])
     assert response == "organization_admin"
+
+
+@mock.patch.object(Client, "request", return_value=({}, None))
+def test_organizations_files_list(mock_request):
+    org_id = gen_uuid()
+
+    call_command("croud", "organizations", "files", "list", "--org-id", org_id)
+    assert_rest(
+        mock_request, RequestMethod.GET, f"/api/v2/organizations/{org_id}/files/"
+    )
+
+
+@mock.patch.object(Client, "request", return_value=({}, None))
+def test_organizations_files_delete(mock_request):
+    org_id = gen_uuid()
+    file_id = gen_uuid()
+
+    call_command(
+        "croud",
+        "organizations",
+        "files",
+        "delete",
+        "--org-id",
+        org_id,
+        "--file-id",
+        file_id,
+    )
+    assert_rest(
+        mock_request,
+        RequestMethod.DELETE,
+        f"/api/v2/organizations/{org_id}/files/{file_id}/",
+    )
+
+
+@mock.patch("croud.organizations.commands.os.path.isfile", return_value=True)
+@mock.patch.object(Client, "request", return_value=({}, None))
+def test_organizations_files_create(mock_request, mock_isfile):
+    org_id = gen_uuid()
+    file_path = "/path/to/file.json.gz"
+    file_name = "my-file"
+    call_command(
+        "croud",
+        "organizations",
+        "files",
+        "create",
+        "--org-id",
+        org_id,
+        "--file-path",
+        file_path,
+        "--name",
+        file_name,
+    )
+    assert_rest(
+        mock_request,
+        RequestMethod.POST,
+        f"/api/v2/organizations/{org_id}/files/",
+        body={"name": file_name},
+    )
```

### Comparing `croud-1.3.0/tests/commands/test_products.py` & `croud-1.4.0/tests/commands/test_products.py`

 * *Files identical despite different names*

### Comparing `croud-1.3.0/tests/commands/test_projects.py` & `croud-1.4.0/tests/commands/test_projects.py`

 * *Files identical despite different names*

### Comparing `croud-1.3.0/tests/commands/test_regions.py` & `croud-1.4.0/tests/commands/test_regions.py`

 * *Files identical despite different names*

### Comparing `croud-1.3.0/tests/commands/test_subscriptions.py` & `croud-1.4.0/tests/commands/test_subscriptions.py`

 * *Files identical despite different names*

### Comparing `croud-1.3.0/tests/commands/test_users.py` & `croud-1.4.0/tests/commands/test_users.py`

 * *Files identical despite different names*

### Comparing `croud-1.3.0/tests/conftest.py` & `croud-1.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `croud-1.3.0/tests/test_api.py` & `croud-1.4.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `croud-1.3.0/tests/test_config_schemas.py` & `croud-1.4.0/tests/test_config_schemas.py`

 * *Files identical despite different names*

### Comparing `croud-1.3.0/tests/test_configuration.py` & `croud-1.4.0/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `croud-1.3.0/tests/test_parser.py` & `croud-1.4.0/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `croud-1.3.0/tests/test_printer.py` & `croud-1.4.0/tests/test_printer.py`

 * *Files identical despite different names*

### Comparing `croud-1.3.0/tests/test_server.py` & `croud-1.4.0/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `croud-1.3.0/tests/test_util.py` & `croud-1.4.0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `croud-1.3.0/tests/util/__init__.py` & `croud-1.4.0/tests/util/__init__.py`

 * *Files identical despite different names*

### Comparing `croud-1.3.0/tests/util/fake_cloud.py` & `croud-1.4.0/tests/util/fake_cloud.py`

 * *Files identical despite different names*

