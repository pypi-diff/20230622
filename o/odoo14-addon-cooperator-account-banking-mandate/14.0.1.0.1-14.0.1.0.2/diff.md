# Comparing `tmp/odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.1.tar.gz` & `tmp/odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.1.tar", last modified: Wed Jun 14 08:27:00 2023, max compression
+gzip compressed data, was "dist/odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.2.tar", last modified: Thu Jun 22 11:53:02 2023, max compression
```

## Comparing `odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.1.tar` & `odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-14 08:27:00.945082 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.1/
--rw-rw-r--   0 daniil    (1000) daniil    (1000)      433 2023-06-14 08:27:00.945082 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.1/PKG-INFO
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-14 08:27:00.941082 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.1/odoo/
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-14 08:27:00.941082 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.1/odoo/addons/
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-14 08:27:00.941082 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.1/odoo/addons/cooperator_account_banking_mandate/
--rw-rw-r--   0 daniil    (1000) daniil    (1000)       46 2023-06-14 08:22:58.000000 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.1/odoo/addons/cooperator_account_banking_mandate/__init__.py
--rw-rw-r--   0 daniil    (1000) daniil    (1000)      543 2023-06-14 08:23:37.000000 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.1/odoo/addons/cooperator_account_banking_mandate/__manifest__.py
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-14 08:27:00.941082 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.1/odoo/addons/cooperator_account_banking_mandate/models/
--rw-rw-r--   0 daniil    (1000) daniil    (1000)       60 2023-06-14 08:22:58.000000 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.1/odoo/addons/cooperator_account_banking_mandate/models/__init__.py
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     2409 2023-06-14 08:22:58.000000 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.1/odoo/addons/cooperator_account_banking_mandate/models/subscription_request.py
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-14 08:27:00.941082 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.1/odoo/addons/cooperator_account_banking_mandate/views/
--rw-rw-r--   0 daniil    (1000) daniil    (1000)      956 2023-06-14 08:22:58.000000 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.1/odoo/addons/cooperator_account_banking_mandate/views/subscription_request_views.xml
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-14 08:27:00.945082 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.1/odoo14_addon_cooperator_account_banking_mandate.egg-info/
--rw-rw-r--   0 daniil    (1000) daniil    (1000)      433 2023-06-14 08:27:00.000000 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.1/odoo14_addon_cooperator_account_banking_mandate.egg-info/PKG-INFO
--rw-rw-r--   0 daniil    (1000) daniil    (1000)      782 2023-06-14 08:27:00.000000 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.1/odoo14_addon_cooperator_account_banking_mandate.egg-info/SOURCES.txt
--rw-rw-r--   0 daniil    (1000) daniil    (1000)        1 2023-06-14 08:27:00.000000 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.1/odoo14_addon_cooperator_account_banking_mandate.egg-info/dependency_links.txt
--rw-rw-r--   0 daniil    (1000) daniil    (1000)        1 2023-06-14 08:27:00.000000 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.1/odoo14_addon_cooperator_account_banking_mandate.egg-info/not-zip-safe
--rw-rw-r--   0 daniil    (1000) daniil    (1000)      169 2023-06-14 08:27:00.000000 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.1/odoo14_addon_cooperator_account_banking_mandate.egg-info/requires.txt
--rw-rw-r--   0 daniil    (1000) daniil    (1000)        5 2023-06-14 08:27:00.000000 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.1/odoo14_addon_cooperator_account_banking_mandate.egg-info/top_level.txt
--rw-rw-r--   0 daniil    (1000) daniil    (1000)       38 2023-06-14 08:27:00.945082 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.1/setup.cfg
--rw-rw-r--   0 daniil    (1000) daniil    (1000)      240 2023-06-14 08:26:18.000000 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.1/setup.py
+drwxr-xr-x   0 enrico    (1000) enrico    (1000)        0 2023-06-22 11:53:02.958712 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.2/
+-rw-r--r--   0 enrico    (1000) enrico    (1000)      491 2023-06-22 11:53:02.958712 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.2/PKG-INFO
+drwxr-xr-x   0 enrico    (1000) enrico    (1000)        0 2023-06-22 11:53:02.952045 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.2/odoo/
+drwxr-xr-x   0 enrico    (1000) enrico    (1000)        0 2023-06-22 11:53:02.952045 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.2/odoo/addons/
+drwxr-xr-x   0 enrico    (1000) enrico    (1000)        0 2023-06-22 11:53:02.955378 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.2/odoo/addons/cooperator_account_banking_mandate/
+-rw-r--r--   0 enrico    (1000) enrico    (1000)       46 2023-06-19 10:18:40.000000 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.2/odoo/addons/cooperator_account_banking_mandate/__init__.py
+-rw-r--r--   0 enrico    (1000) enrico    (1000)      543 2023-06-22 11:44:42.000000 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.2/odoo/addons/cooperator_account_banking_mandate/__manifest__.py
+drwxr-xr-x   0 enrico    (1000) enrico    (1000)        0 2023-06-22 11:53:02.955378 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.2/odoo/addons/cooperator_account_banking_mandate/models/
+-rw-r--r--   0 enrico    (1000) enrico    (1000)       60 2023-06-19 10:18:40.000000 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.2/odoo/addons/cooperator_account_banking_mandate/models/__init__.py
+-rw-r--r--   0 enrico    (1000) enrico    (1000)     2409 2023-06-19 10:18:40.000000 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.2/odoo/addons/cooperator_account_banking_mandate/models/subscription_request.py
+drwxr-xr-x   0 enrico    (1000) enrico    (1000)        0 2023-06-22 11:53:02.955378 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.2/odoo/addons/cooperator_account_banking_mandate/views/
+-rw-r--r--   0 enrico    (1000) enrico    (1000)      956 2023-06-19 10:18:40.000000 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.2/odoo/addons/cooperator_account_banking_mandate/views/subscription_request_views.xml
+drwxr-xr-x   0 enrico    (1000) enrico    (1000)        0 2023-06-22 11:53:02.958712 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.2/odoo14_addon_cooperator_account_banking_mandate.egg-info/
+-rw-r--r--   0 enrico    (1000) enrico    (1000)      491 2023-06-22 11:53:02.000000 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.2/odoo14_addon_cooperator_account_banking_mandate.egg-info/PKG-INFO
+-rw-r--r--   0 enrico    (1000) enrico    (1000)      782 2023-06-22 11:53:02.000000 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.2/odoo14_addon_cooperator_account_banking_mandate.egg-info/SOURCES.txt
+-rw-r--r--   0 enrico    (1000) enrico    (1000)        1 2023-06-22 11:53:02.000000 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.2/odoo14_addon_cooperator_account_banking_mandate.egg-info/dependency_links.txt
+-rw-r--r--   0 enrico    (1000) enrico    (1000)        1 2023-06-22 11:53:02.000000 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.2/odoo14_addon_cooperator_account_banking_mandate.egg-info/not-zip-safe
+-rw-r--r--   0 enrico    (1000) enrico    (1000)      169 2023-06-22 11:53:02.000000 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.2/odoo14_addon_cooperator_account_banking_mandate.egg-info/requires.txt
+-rw-r--r--   0 enrico    (1000) enrico    (1000)        5 2023-06-22 11:53:02.000000 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.2/odoo14_addon_cooperator_account_banking_mandate.egg-info/top_level.txt
+-rw-r--r--   0 enrico    (1000) enrico    (1000)       38 2023-06-22 11:53:02.958712 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.2/setup.cfg
+-rw-r--r--   0 enrico    (1000) enrico    (1000)      240 2023-06-19 10:18:40.000000 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.2/setup.py
```

### Comparing `odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.1/odoo/addons/cooperator_account_banking_mandate/__manifest__.py` & `odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.2/odoo/addons/cooperator_account_banking_mandate/__manifest__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 {
     "name": "Cooperator Account Banking Mandate",
-    "version": "14.0.1.0.1",
+    "version": "14.0.1.0.2",
     "license": "AGPL-3",
     "summary": """
         This module adds mandate selection to cooperator subscription request.""",
     "author": "Som IT Cooperatiu SCCL",
     "category": "Banking addons",
     "depends": ["cooperator", "account_payment_cooperator", "account_banking_mandate",
                 "account_banking_sepa_direct_debit"],
```

### Comparing `odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.1/odoo/addons/cooperator_account_banking_mandate/models/subscription_request.py` & `odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.2/odoo/addons/cooperator_account_banking_mandate/models/subscription_request.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.1/odoo/addons/cooperator_account_banking_mandate/views/subscription_request_views.xml` & `odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.2/odoo/addons/cooperator_account_banking_mandate/views/subscription_request_views.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.1/odoo14_addon_cooperator_account_banking_mandate.egg-info/SOURCES.txt` & `odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.2/odoo14_addon_cooperator_account_banking_mandate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

