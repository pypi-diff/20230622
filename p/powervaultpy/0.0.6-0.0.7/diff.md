# Comparing `tmp/powervaultpy-0.0.6.tar.gz` & `tmp/powervaultpy-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "powervaultpy-0.0.6.tar", last modified: Tue Jun 20 22:37:03 2023, max compression
+gzip compressed data, was "powervaultpy-0.0.7.tar", last modified: Wed Jun 21 23:05:04 2023, max compression
```

## Comparing `powervaultpy-0.0.6.tar` & `powervaultpy-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-20 22:37:03.463086 powervaultpy-0.0.6/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      701 2023-06-20 22:37:03.463086 powervaultpy-0.0.6/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1478 2023-06-20 22:37:00.000000 powervaultpy-0.0.6/pyproject.toml
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-06-20 22:37:03.463086 powervaultpy-0.0.6/setup.cfg
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-20 22:37:03.462086 powervaultpy-0.0.6/src/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-20 22:37:03.463086 powervaultpy-0.0.6/src/powervaultpy/
--rw-r--r--   0 vscode    (1000) vscode    (1000)       47 2023-06-20 22:25:16.000000 powervaultpy-0.0.6/src/powervaultpy/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7710 2023-06-20 22:36:50.000000 powervaultpy-0.0.6/src/powervaultpy/powervault.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-20 22:37:03.463086 powervaultpy-0.0.6/src/powervaultpy.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      701 2023-06-20 22:37:03.000000 powervaultpy-0.0.6/src/powervaultpy.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      273 2023-06-20 22:37:03.000000 powervaultpy-0.0.6/src/powervaultpy.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-06-20 22:37:03.000000 powervaultpy-0.0.6/src/powervaultpy.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       99 2023-06-20 22:37:03.000000 powervaultpy-0.0.6/src/powervaultpy.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       13 2023-06-20 22:37:03.000000 powervaultpy-0.0.6/src/powervaultpy.egg-info/top_level.txt
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-21 23:05:04.324443 powervaultpy-0.0.7/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      701 2023-06-21 23:05:04.324443 powervaultpy-0.0.7/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1478 2023-06-21 23:04:45.000000 powervaultpy-0.0.7/pyproject.toml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-06-21 23:05:04.324443 powervaultpy-0.0.7/setup.cfg
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-21 23:05:04.323443 powervaultpy-0.0.7/src/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-21 23:05:04.323443 powervaultpy-0.0.7/src/powervaultpy/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       63 2023-06-21 22:09:08.000000 powervaultpy-0.0.7/src/powervaultpy/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9040 2023-06-21 23:03:12.000000 powervaultpy-0.0.7/src/powervaultpy/powervault.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-21 23:05:04.324443 powervaultpy-0.0.7/src/powervaultpy.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      701 2023-06-21 23:05:04.000000 powervaultpy-0.0.7/src/powervaultpy.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      273 2023-06-21 23:05:04.000000 powervaultpy-0.0.7/src/powervaultpy.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-06-21 23:05:04.000000 powervaultpy-0.0.7/src/powervaultpy.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       99 2023-06-21 23:05:04.000000 powervaultpy-0.0.7/src/powervaultpy.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       13 2023-06-21 23:05:04.000000 powervaultpy-0.0.7/src/powervaultpy.egg-info/top_level.txt
```

### Comparing `powervaultpy-0.0.6/PKG-INFO` & `powervaultpy-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powervaultpy
-Version: 0.0.6
+Version: 0.0.7
 Summary: An integration to control the Powervault battery
 Author-email: Adam McDonagh <adam@elitemonkey.net>
 License: GPLv3
 Project-URL: Homepage, https://github.com/adammcdonagh/powervaultpy
 Project-URL: Bug Tracker, https://github.com/adammcdonagh/powervaultpy/issues
 Project-URL: Changelog, https://github.com/adammcdonagh/powervaultpy/blob/main/CHANGELOG.md
 Keywords: powervault,home,automation
```

### Comparing `powervaultpy-0.0.6/pyproject.toml` & `powervaultpy-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "powervaultpy"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Adam McDonagh", email="adam@elitemonkey.net" },
 ]
 license = { text = "GPLv3" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

### Comparing `powervaultpy-0.0.6/src/powervaultpy/powervault.py` & `powervaultpy-0.0.7/src/powervaultpy/powervault.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,26 @@
 """Sample API Client."""
 
 import json
 import logging
-from datetime import datetime
+from datetime import datetime, timedelta
 
 import pytz
 import requests
 
+VALID_STATUSES = [
+    "normal",
+    "only-charge",
+    "only-discharge",
+    "force-charge",
+    "force-discharge",
+    "disable",
+    "dormant",
+]
+
 _LOGGER = logging.getLogger(__name__)
 _LOGGER.setLevel(logging.DEBUG)
 
 class PowerVaultApiClientError(Exception):
     """Exception to indicate a general API error."""
 
 
@@ -130,28 +140,58 @@
         _LOGGER.debug("Data: %s", data_response)
 
         if (data_response is not None) and ("data" in data_response):
             return data_response["data"]
 
         _LOGGER.error("Failed to retrieve data")
 
+    def set_battery_state(self, unit_id: str, battery_state) -> bool:
+        """Override the current battery status with the provided one."""
+        url = f"{self._base_url}/unit/{unit_id}/stateOverride"
+
+        start_time = datetime.now(pytz.timezone('UTC')).strftime("%Y-%m-%d %H:%M:%S")
+        end_time = (datetime.now(pytz.timezone('UTC')) + timedelta(hours=24)).strftime("%Y-%m-%d %H:%M:%S")
+
+        payload = {
+            "stateOverrides": [
+                {
+                    "start": start_time,
+                    "end": end_time,
+                    "state": battery_state
+                }
+            ]
+        }
+
+        _LOGGER.debug("Payload: %s", payload)
+
+        state_override_response = self._read_response(
+            self._session.post(url, json=payload), url)
+        
+        _LOGGER.debug("State Override: %s", state_override_response)
+
+        if (state_override_response is not None) and ("stateOverrides" in state_override_response) and "message" in state_override_response and state_override_response["message"] == "success":
+            return True
+        else:
+            return False
+        
+
     def get_battery_state(self, unit_id: str) -> any:
         """Query the schedule and overrides to determine the current battery state."""
         url = f"{self._base_url}/unit/{unit_id}/schedule"
 
         schedule_response = self._read_response(self._session.get(url), url)
         _LOGGER.debug("Schedule: %s", schedule_response)
 
         url = f"{self._base_url}/unit/{unit_id}/stateOverride"
 
         state_override_response = self._read_response(self._session.get(url), url)
         _LOGGER.debug("State Override: %s", state_override_response)
 
         # Get the current local datetime
-        current_dow = datetime.now().strftime("%A").lower()
+        current_dow = datetime.now(pytz.timezone("Europe/London")).strftime("%A").lower()
 
         # Log the current day of the week
         _LOGGER.debug("Current day of the week: %s", current_dow)
 
         # Get the current time
         current_time = datetime.now(pytz.timezone('Europe/London'))
```

### Comparing `powervaultpy-0.0.6/src/powervaultpy.egg-info/PKG-INFO` & `powervaultpy-0.0.7/src/powervaultpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powervaultpy
-Version: 0.0.6
+Version: 0.0.7
 Summary: An integration to control the Powervault battery
 Author-email: Adam McDonagh <adam@elitemonkey.net>
 License: GPLv3
 Project-URL: Homepage, https://github.com/adammcdonagh/powervaultpy
 Project-URL: Bug Tracker, https://github.com/adammcdonagh/powervaultpy/issues
 Project-URL: Changelog, https://github.com/adammcdonagh/powervaultpy/blob/main/CHANGELOG.md
 Keywords: powervault,home,automation
```

