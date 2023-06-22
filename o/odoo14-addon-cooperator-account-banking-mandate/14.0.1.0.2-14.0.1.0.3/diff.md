# Comparing `tmp/odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.2.tar.gz` & `tmp/odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.2.tar", last modified: Thu Jun 22 11:53:02 2023, max compression
+gzip compressed data, was "dist/odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.3.tar", last modified: Thu Jun 22 15:44:27 2023, max compression
```

## Comparing `odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.2.tar` & `odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 enrico    (1000) enrico    (1000)        0 2023-06-22 11:53:02.958712 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.2/
--rw-r--r--   0 enrico    (1000) enrico    (1000)      491 2023-06-22 11:53:02.958712 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.2/PKG-INFO
-drwxr-xr-x   0 enrico    (1000) enrico    (1000)        0 2023-06-22 11:53:02.952045 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.2/odoo/
-drwxr-xr-x   0 enrico    (1000) enrico    (1000)        0 2023-06-22 11:53:02.952045 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.2/odoo/addons/
-drwxr-xr-x   0 enrico    (1000) enrico    (1000)        0 2023-06-22 11:53:02.955378 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.2/odoo/addons/cooperator_account_banking_mandate/
--rw-r--r--   0 enrico    (1000) enrico    (1000)       46 2023-06-19 10:18:40.000000 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.2/odoo/addons/cooperator_account_banking_mandate/__init__.py
--rw-r--r--   0 enrico    (1000) enrico    (1000)      543 2023-06-22 11:44:42.000000 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.2/odoo/addons/cooperator_account_banking_mandate/__manifest__.py
-drwxr-xr-x   0 enrico    (1000) enrico    (1000)        0 2023-06-22 11:53:02.955378 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.2/odoo/addons/cooperator_account_banking_mandate/models/
--rw-r--r--   0 enrico    (1000) enrico    (1000)       60 2023-06-19 10:18:40.000000 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.2/odoo/addons/cooperator_account_banking_mandate/models/__init__.py
--rw-r--r--   0 enrico    (1000) enrico    (1000)     2409 2023-06-19 10:18:40.000000 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.2/odoo/addons/cooperator_account_banking_mandate/models/subscription_request.py
-drwxr-xr-x   0 enrico    (1000) enrico    (1000)        0 2023-06-22 11:53:02.955378 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.2/odoo/addons/cooperator_account_banking_mandate/views/
--rw-r--r--   0 enrico    (1000) enrico    (1000)      956 2023-06-19 10:18:40.000000 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.2/odoo/addons/cooperator_account_banking_mandate/views/subscription_request_views.xml
-drwxr-xr-x   0 enrico    (1000) enrico    (1000)        0 2023-06-22 11:53:02.958712 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.2/odoo14_addon_cooperator_account_banking_mandate.egg-info/
--rw-r--r--   0 enrico    (1000) enrico    (1000)      491 2023-06-22 11:53:02.000000 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.2/odoo14_addon_cooperator_account_banking_mandate.egg-info/PKG-INFO
--rw-r--r--   0 enrico    (1000) enrico    (1000)      782 2023-06-22 11:53:02.000000 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.2/odoo14_addon_cooperator_account_banking_mandate.egg-info/SOURCES.txt
--rw-r--r--   0 enrico    (1000) enrico    (1000)        1 2023-06-22 11:53:02.000000 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.2/odoo14_addon_cooperator_account_banking_mandate.egg-info/dependency_links.txt
--rw-r--r--   0 enrico    (1000) enrico    (1000)        1 2023-06-22 11:53:02.000000 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.2/odoo14_addon_cooperator_account_banking_mandate.egg-info/not-zip-safe
--rw-r--r--   0 enrico    (1000) enrico    (1000)      169 2023-06-22 11:53:02.000000 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.2/odoo14_addon_cooperator_account_banking_mandate.egg-info/requires.txt
--rw-r--r--   0 enrico    (1000) enrico    (1000)        5 2023-06-22 11:53:02.000000 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.2/odoo14_addon_cooperator_account_banking_mandate.egg-info/top_level.txt
--rw-r--r--   0 enrico    (1000) enrico    (1000)       38 2023-06-22 11:53:02.958712 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.2/setup.cfg
--rw-r--r--   0 enrico    (1000) enrico    (1000)      240 2023-06-19 10:18:40.000000 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.2/setup.py
+drwxr-xr-x   0 enrico    (1000) enrico    (1000)        0 2023-06-22 15:44:27.464319 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.3/
+-rw-r--r--   0 enrico    (1000) enrico    (1000)      491 2023-06-22 15:44:27.464319 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.3/PKG-INFO
+drwxr-xr-x   0 enrico    (1000) enrico    (1000)        0 2023-06-22 15:44:27.460986 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.3/odoo/
+drwxr-xr-x   0 enrico    (1000) enrico    (1000)        0 2023-06-22 15:44:27.460986 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.3/odoo/addons/
+drwxr-xr-x   0 enrico    (1000) enrico    (1000)        0 2023-06-22 15:44:27.460986 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.3/odoo/addons/cooperator_account_banking_mandate/
+-rw-r--r--   0 enrico    (1000) enrico    (1000)       46 2023-06-19 10:18:40.000000 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.3/odoo/addons/cooperator_account_banking_mandate/__init__.py
+-rw-r--r--   0 enrico    (1000) enrico    (1000)      543 2023-06-22 15:43:05.000000 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.3/odoo/addons/cooperator_account_banking_mandate/__manifest__.py
+drwxr-xr-x   0 enrico    (1000) enrico    (1000)        0 2023-06-22 15:44:27.464319 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.3/odoo/addons/cooperator_account_banking_mandate/models/
+-rw-r--r--   0 enrico    (1000) enrico    (1000)       60 2023-06-19 10:18:40.000000 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.3/odoo/addons/cooperator_account_banking_mandate/models/__init__.py
+-rw-r--r--   0 enrico    (1000) enrico    (1000)     2409 2023-06-19 10:18:40.000000 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.3/odoo/addons/cooperator_account_banking_mandate/models/subscription_request.py
+drwxr-xr-x   0 enrico    (1000) enrico    (1000)        0 2023-06-22 15:44:27.464319 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.3/odoo/addons/cooperator_account_banking_mandate/views/
+-rw-r--r--   0 enrico    (1000) enrico    (1000)      956 2023-06-19 10:18:40.000000 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.3/odoo/addons/cooperator_account_banking_mandate/views/subscription_request_views.xml
+drwxr-xr-x   0 enrico    (1000) enrico    (1000)        0 2023-06-22 15:44:27.464319 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.3/odoo14_addon_cooperator_account_banking_mandate.egg-info/
+-rw-r--r--   0 enrico    (1000) enrico    (1000)      491 2023-06-22 15:44:27.000000 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.3/odoo14_addon_cooperator_account_banking_mandate.egg-info/PKG-INFO
+-rw-r--r--   0 enrico    (1000) enrico    (1000)      782 2023-06-22 15:44:27.000000 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.3/odoo14_addon_cooperator_account_banking_mandate.egg-info/SOURCES.txt
+-rw-r--r--   0 enrico    (1000) enrico    (1000)        1 2023-06-22 15:44:27.000000 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.3/odoo14_addon_cooperator_account_banking_mandate.egg-info/dependency_links.txt
+-rw-r--r--   0 enrico    (1000) enrico    (1000)        1 2023-06-22 11:53:02.000000 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.3/odoo14_addon_cooperator_account_banking_mandate.egg-info/not-zip-safe
+-rw-r--r--   0 enrico    (1000) enrico    (1000)      181 2023-06-22 15:44:27.000000 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.3/odoo14_addon_cooperator_account_banking_mandate.egg-info/requires.txt
+-rw-r--r--   0 enrico    (1000) enrico    (1000)        5 2023-06-22 15:44:27.000000 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.3/odoo14_addon_cooperator_account_banking_mandate.egg-info/top_level.txt
+-rw-r--r--   0 enrico    (1000) enrico    (1000)       38 2023-06-22 15:44:27.464319 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.3/setup.cfg
+-rw-r--r--   0 enrico    (1000) enrico    (1000)      240 2023-06-19 10:18:40.000000 odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.3/setup.py
```

### Comparing `odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.2/odoo/addons/cooperator_account_banking_mandate/__manifest__.py` & `odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.3/odoo/addons/cooperator_account_banking_mandate/__manifest__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
 {
     "name": "Cooperator Account Banking Mandate",
-    "version": "14.0.1.0.2",
+    "version": "14.0.1.0.3",
     "license": "AGPL-3",
     "summary": """
         This module adds mandate selection to cooperator subscription request.""",
     "author": "Som IT Cooperatiu SCCL",
     "category": "Banking addons",
-    "depends": ["cooperator", "account_payment_cooperator", "account_banking_mandate",
+    "depends": ["cooperator", "cooperator_account_payment", "account_banking_mandate",
                 "account_banking_sepa_direct_debit"],
     "data": [
         "views/subscription_request_views.xml",
     ],
     "installable": True,
 }
```

### Comparing `odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.2/odoo/addons/cooperator_account_banking_mandate/models/subscription_request.py` & `odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.3/odoo/addons/cooperator_account_banking_mandate/models/subscription_request.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.2/odoo/addons/cooperator_account_banking_mandate/views/subscription_request_views.xml` & `odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.3/odoo/addons/cooperator_account_banking_mandate/views/subscription_request_views.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.2/odoo14_addon_cooperator_account_banking_mandate.egg-info/SOURCES.txt` & `odoo14-addon-cooperator_account_banking_mandate-14.0.1.0.3/odoo14_addon_cooperator_account_banking_mandate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

