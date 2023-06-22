# Comparing `tmp/arivo-settings_models-0.0.1rc0.tar.gz` & `tmp/arivo-settings_models-0.0.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/arivo-settings_models-0.0.1rc0.tar", last modified: Wed Jun 14 09:15:51 2023, max compression
+gzip compressed data, was "dist/arivo-settings_models-0.0.1rc1.tar", last modified: Thu Jun 22 11:56:04 2023, max compression
```

## Comparing `arivo-settings_models-0.0.1rc0.tar` & `arivo-settings_models-0.0.1rc1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:15:51.000000 arivo-settings_models-0.0.1rc0/
--rw-rw-rw-   0 root         (0) root         (0)      183 2023-06-14 09:15:36.000000 arivo-settings_models-0.0.1rc0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      445 2023-06-14 09:15:36.000000 arivo-settings_models-0.0.1rc0/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      360 2023-06-14 09:15:36.000000 arivo-settings_models-0.0.1rc0/tox.ini
--rw-rw-rw-   0 root         (0) root         (0)      569 2023-06-14 09:15:51.000000 arivo-settings_models-0.0.1rc0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1061 2023-06-14 09:15:51.000000 arivo-settings_models-0.0.1rc0/ChangeLog
--rw-rw-rw-   0 root         (0) root         (0)     1353 2023-06-14 09:15:36.000000 arivo-settings_models-0.0.1rc0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-06-14 09:15:36.000000 arivo-settings_models-0.0.1rc0/.coveragerc
--rw-r--r--   0 root         (0) root         (0)      707 2023-06-14 09:15:51.000000 arivo-settings_models-0.0.1rc0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-06-14 09:15:36.000000 arivo-settings_models-0.0.1rc0/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:15:51.000000 arivo-settings_models-0.0.1rc0/tests/
--rw-rw-rw-   0 root         (0) root         (0)      873 2023-06-14 09:15:36.000000 arivo-settings_models-0.0.1rc0/tests/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    11070 2023-06-14 09:15:36.000000 arivo-settings_models-0.0.1rc0/tests/test_models.py
--rw-rw-rw-   0 root         (0) root         (0)     3417 2023-06-14 09:15:36.000000 arivo-settings_models-0.0.1rc0/tests/test_serialization.py
--rw-rw-rw-   0 root         (0) root         (0)    32787 2023-06-14 09:15:36.000000 arivo-settings_models-0.0.1rc0/tests/test_validation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:15:51.000000 arivo-settings_models-0.0.1rc0/docs/
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-06-14 09:15:36.000000 arivo-settings_models-0.0.1rc0/docs/migrations.md
--rw-rw-rw-   0 root         (0) root         (0)       18 2023-06-14 09:15:36.000000 arivo-settings_models-0.0.1rc0/test-requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:15:51.000000 arivo-settings_models-0.0.1rc0/arivo_settings_models.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 09:15:51.000000 arivo-settings_models-0.0.1rc0/arivo_settings_models.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 09:15:51.000000 arivo-settings_models-0.0.1rc0/arivo_settings_models.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      707 2023-06-14 09:15:51.000000 arivo-settings_models-0.0.1rc0/arivo_settings_models.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       57 2023-06-14 09:15:51.000000 arivo-settings_models-0.0.1rc0/arivo_settings_models.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       46 2023-06-14 09:15:51.000000 arivo-settings_models-0.0.1rc0/arivo_settings_models.egg-info/pbr.json
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-14 09:15:51.000000 arivo-settings_models-0.0.1rc0/arivo_settings_models.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      922 2023-06-14 09:15:51.000000 arivo-settings_models-0.0.1rc0/arivo_settings_models.egg-info/SOURCES.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:15:51.000000 arivo-settings_models-0.0.1rc0/tools/
--rw-rw-rw-   0 root         (0) root         (0)      439 2023-06-14 09:15:36.000000 arivo-settings_models-0.0.1rc0/tools/pages.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:15:51.000000 arivo-settings_models-0.0.1rc0/settings_models/
--rw-rw-rw-   0 root         (0) root         (0)      163 2023-06-14 09:15:36.000000 arivo-settings_models-0.0.1rc0/settings_models/_combat.py
--rw-rw-rw-   0 root         (0) root         (0)     1977 2023-06-14 09:15:36.000000 arivo-settings_models-0.0.1rc0/settings_models/validators.py
--rw-rw-rw-   0 root         (0) root         (0)      372 2023-06-14 09:15:36.000000 arivo-settings_models-0.0.1rc0/settings_models/doc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:15:51.000000 arivo-settings_models-0.0.1rc0/settings_models/settings/
--rw-rw-rw-   0 root         (0) root         (0)      749 2023-06-14 09:15:36.000000 arivo-settings_models-0.0.1rc0/settings_models/settings/gate_control.py
--rw-rw-rw-   0 root         (0) root         (0)    17036 2023-06-14 09:15:36.000000 arivo-settings_models-0.0.1rc0/settings_models/settings/common.py
--rw-rw-rw-   0 root         (0) root         (0)      524 2023-06-14 09:15:36.000000 arivo-settings_models-0.0.1rc0/settings_models/settings/device_keys.py
--rw-rw-rw-   0 root         (0) root         (0)      332 2023-06-14 09:15:36.000000 arivo-settings_models-0.0.1rc0/settings_models/settings/intercom.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-14 09:15:36.000000 arivo-settings_models-0.0.1rc0/settings_models/settings/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      477 2023-06-14 09:15:36.000000 arivo-settings_models-0.0.1rc0/settings_models/settings/enforcement.py
--rw-rw-rw-   0 root         (0) root         (0)     6650 2023-06-14 09:15:36.000000 arivo-settings_models-0.0.1rc0/settings_models/serialization.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-14 09:15:36.000000 arivo-settings_models-0.0.1rc0/settings_models/__init__.py
--rw-r--r--   0 root         (0) root         (0)      111 2023-06-14 09:15:51.000000 arivo-settings_models-0.0.1rc0/AUTHORS
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 11:56:04.000000 arivo-settings_models-0.0.1rc1/
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-05-11 10:22:52.000000 arivo-settings_models-0.0.1rc1/.coveragerc
+-rw-r--r--   0 root         (0) root         (0)      111 2023-06-22 11:56:04.000000 arivo-settings_models-0.0.1rc1/AUTHORS
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 11:56:04.000000 arivo-settings_models-0.0.1rc1/settings_models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 11:55:45.000000 arivo-settings_models-0.0.1rc1/settings_models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1977 2023-06-13 13:58:32.000000 arivo-settings_models-0.0.1rc1/settings_models/validators.py
+-rw-rw-rw-   0 root         (0) root         (0)      372 2023-06-13 13:58:32.000000 arivo-settings_models-0.0.1rc1/settings_models/doc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 11:56:04.000000 arivo-settings_models-0.0.1rc1/settings_models/settings/
+-rw-rw-rw-   0 root         (0) root         (0)      749 2023-06-13 13:58:32.000000 arivo-settings_models-0.0.1rc1/settings_models/settings/gate_control.py
+-rw-rw-rw-   0 root         (0) root         (0)      332 2023-06-13 13:58:32.000000 arivo-settings_models-0.0.1rc1/settings_models/settings/intercom.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 11:55:45.000000 arivo-settings_models-0.0.1rc1/settings_models/settings/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      477 2023-06-13 13:58:32.000000 arivo-settings_models-0.0.1rc1/settings_models/settings/enforcement.py
+-rw-rw-rw-   0 root         (0) root         (0)    17036 2023-06-13 13:58:32.000000 arivo-settings_models-0.0.1rc1/settings_models/settings/common.py
+-rw-rw-rw-   0 root         (0) root         (0)      524 2023-06-13 13:58:32.000000 arivo-settings_models-0.0.1rc1/settings_models/settings/device_keys.py
+-rw-rw-rw-   0 root         (0) root         (0)      163 2023-06-13 13:58:32.000000 arivo-settings_models-0.0.1rc1/settings_models/_combat.py
+-rw-rw-rw-   0 root         (0) root         (0)     6637 2023-06-22 11:55:45.000000 arivo-settings_models-0.0.1rc1/settings_models/serialization.py
+-rw-rw-rw-   0 root         (0) root         (0)      360 2023-05-17 14:33:24.000000 arivo-settings_models-0.0.1rc1/tox.ini
+-rw-rw-rw-   0 root         (0) root         (0)      445 2023-05-11 10:22:52.000000 arivo-settings_models-0.0.1rc1/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-05-17 14:33:24.000000 arivo-settings_models-0.0.1rc1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)      707 2023-06-22 11:56:04.000000 arivo-settings_models-0.0.1rc1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1353 2023-06-22 11:55:45.000000 arivo-settings_models-0.0.1rc1/.gitlab-ci.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 11:56:04.000000 arivo-settings_models-0.0.1rc1/tools/
+-rw-rw-rw-   0 root         (0) root         (0)      439 2023-05-17 14:33:24.000000 arivo-settings_models-0.0.1rc1/tools/pages.py
+-rw-rw-rw-   0 root         (0) root         (0)      569 2023-06-22 11:56:04.000000 arivo-settings_models-0.0.1rc1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 11:56:04.000000 arivo-settings_models-0.0.1rc1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     3417 2023-06-13 13:58:32.000000 arivo-settings_models-0.0.1rc1/tests/test_serialization.py
+-rw-rw-rw-   0 root         (0) root         (0)    32787 2023-06-13 13:58:32.000000 arivo-settings_models-0.0.1rc1/tests/test_validation.py
+-rw-rw-rw-   0 root         (0) root         (0)    11070 2023-06-13 13:58:32.000000 arivo-settings_models-0.0.1rc1/tests/test_models.py
+-rw-rw-rw-   0 root         (0) root         (0)      873 2023-06-13 13:58:32.000000 arivo-settings_models-0.0.1rc1/tests/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      183 2023-05-11 10:22:52.000000 arivo-settings_models-0.0.1rc1/README.md
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-06-22 11:56:04.000000 arivo-settings_models-0.0.1rc1/ChangeLog
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-05-11 10:22:52.000000 arivo-settings_models-0.0.1rc1/test-requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 11:56:04.000000 arivo-settings_models-0.0.1rc1/docs/
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-05-11 10:22:52.000000 arivo-settings_models-0.0.1rc1/docs/migrations.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 11:56:04.000000 arivo-settings_models-0.0.1rc1/arivo_settings_models.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      707 2023-06-22 11:56:04.000000 arivo-settings_models-0.0.1rc1/arivo_settings_models.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       57 2023-06-22 11:56:04.000000 arivo-settings_models-0.0.1rc1/arivo_settings_models.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 11:56:04.000000 arivo-settings_models-0.0.1rc1/arivo_settings_models.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 11:56:04.000000 arivo-settings_models-0.0.1rc1/arivo_settings_models.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       47 2023-06-22 11:56:04.000000 arivo-settings_models-0.0.1rc1/arivo_settings_models.egg-info/pbr.json
+-rw-r--r--   0 root         (0) root         (0)      922 2023-06-22 11:56:04.000000 arivo-settings_models-0.0.1rc1/arivo_settings_models.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-22 11:56:04.000000 arivo-settings_models-0.0.1rc1/arivo_settings_models.egg-info/top_level.txt
```

### Comparing `arivo-settings_models-0.0.1rc0/setup.cfg` & `arivo-settings_models-0.0.1rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-0.0.1rc0/ChangeLog` & `arivo-settings_models-0.0.1rc1/ChangeLog`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 CHANGES
 =======
 
+v0.0.1rc1
+---------
+
+* marked gate\_control/day\_mode as unscoped
+
 v0.0.1rc0
 ---------
 
 * push package on pypi
 
 v0.0.0rc5
 ---------
```

### Comparing `arivo-settings_models-0.0.1rc0/.gitlab-ci.yml` & `arivo-settings_models-0.0.1rc1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-0.0.1rc0/PKG-INFO` & `arivo-settings_models-0.0.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: arivo-settings_models
-Version: 0.0.1rc0
+Version: 0.0.1rc1
 Summary: Library for arivo parking system settings definitions and models
 Home-page: https://gitlab.com/accessio/onegate/settings-models
 Author: ARIVO
 Author-email: support@arivo.co
 License: "GPL-3",
 Description: # Settings Models
```

### Comparing `arivo-settings_models-0.0.1rc0/tests/utils.py` & `arivo-settings_models-0.0.1rc1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-0.0.1rc0/tests/test_models.py` & `arivo-settings_models-0.0.1rc1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-0.0.1rc0/tests/test_serialization.py` & `arivo-settings_models-0.0.1rc1/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-0.0.1rc0/tests/test_validation.py` & `arivo-settings_models-0.0.1rc1/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-0.0.1rc0/arivo_settings_models.egg-info/PKG-INFO` & `arivo-settings_models-0.0.1rc1/arivo_settings_models.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: arivo-settings-models
-Version: 0.0.1rc0
+Version: 0.0.1rc1
 Summary: Library for arivo parking system settings definitions and models
 Home-page: https://gitlab.com/accessio/onegate/settings-models
 Author: ARIVO
 Author-email: support@arivo.co
 License: "GPL-3",
 Description: # Settings Models
```

### Comparing `arivo-settings_models-0.0.1rc0/arivo_settings_models.egg-info/SOURCES.txt` & `arivo-settings_models-0.0.1rc1/arivo_settings_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-0.0.1rc0/settings_models/validators.py` & `arivo-settings_models-0.0.1rc1/settings_models/validators.py`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-0.0.1rc0/settings_models/settings/gate_control.py` & `arivo-settings_models-0.0.1rc1/settings_models/settings/gate_control.py`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-0.0.1rc0/settings_models/settings/common.py` & `arivo-settings_models-0.0.1rc1/settings_models/settings/common.py`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-0.0.1rc0/settings_models/settings/device_keys.py` & `arivo-settings_models-0.0.1rc1/settings_models/settings/device_keys.py`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-0.0.1rc0/settings_models/serialization.py` & `arivo-settings_models-0.0.1rc1/settings_models/serialization.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     "common/garage_settings": Setting(GarageSettings),
     "common/location": Setting(Location),
     "common/billing": Setting(BillingSettings),
     "common/support": Setting(SupportSettings),
     "common/garage_name": Setting(GarageName),
     "common/urls": Setting(Urls),
     "gate_control/mode": Setting(GateMode, scoped=True),
-    "gate_control/day_mode": Setting(DayMode, scoped=True),
+    "gate_control/day_mode": Setting(DayMode),
     "enforcement/basic_settings": Setting(EnforcementSettings),
     "intercom/basic_settings": Setting(IntercomSettings),
     "device_keys/pairing": Setting(PairingKey),
     "feature_flags": Setting(dict, "A dictionary of custom values that can be used to enable or "
                                    "disable features in various places."),
 }
```

