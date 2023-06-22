# Comparing `tmp/ssh_remote_control-0.1.3.tar.gz` & `tmp/ssh_remote_control-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssh_remote_control-0.1.3.tar", last modified: Tue Jun 20 10:53:44 2023, max compression
+gzip compressed data, was "ssh_remote_control-0.1.4.tar", last modified: Thu Jun 22 08:15:17 2023, max compression
```

## Comparing `ssh_remote_control-0.1.3.tar` & `ssh_remote_control-0.1.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 10:53:44.490080 ssh_remote_control-0.1.3/
--rw-rw-rw-   0        0        0     1084 2023-06-19 04:51:08.000000 ssh_remote_control-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     1569 2023-06-20 10:53:44.489081 ssh_remote_control-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      973 2023-06-20 06:12:24.000000 ssh_remote_control-0.1.3/README.md
--rw-rw-rw-   0        0        0      846 2023-06-20 10:52:31.000000 ssh_remote_control-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-20 10:53:44.491079 ssh_remote_control-0.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-20 10:53:44.414083 ssh_remote_control-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-20 10:53:44.447080 ssh_remote_control-0.1.3/src/ssh_remote_control/
--rw-rw-rw-   0        0        0    10675 2023-06-20 10:48:44.000000 ssh_remote_control-0.1.3/src/ssh_remote_control/__init__.py
--rw-rw-rw-   0        0        0     6576 2023-06-20 10:48:44.000000 ssh_remote_control-0.1.3/src/ssh_remote_control/command.py
--rw-rw-rw-   0        0        0     2882 2023-06-20 10:48:44.000000 ssh_remote_control-0.1.3/src/ssh_remote_control/command_set.py
-drwxrwxrwx   0        0        0        0 2023-06-20 10:53:44.487084 ssh_remote_control-0.1.3/src/ssh_remote_control/default_command_sets/
--rw-rw-rw-   0        0        0      163 2023-06-20 10:48:45.000000 ssh_remote_control-0.1.3/src/ssh_remote_control/default_command_sets/__init__.py
--rw-rw-rw-   0        0        0     1006 2023-06-20 10:48:45.000000 ssh_remote_control-0.1.3/src/ssh_remote_control/default_command_sets/const.py
--rw-rw-rw-   0        0        0     3987 2023-06-20 10:51:23.000000 ssh_remote_control-0.1.3/src/ssh_remote_control/default_command_sets/linux.py
--rw-rw-rw-   0        0        0     3822 2023-06-20 10:48:45.000000 ssh_remote_control-0.1.3/src/ssh_remote_control/default_command_sets/windows_cmd.py
--rw-rw-rw-   0        0        0     4087 2023-06-20 10:48:45.000000 ssh_remote_control-0.1.3/src/ssh_remote_control/default_command_sets/windows_ps.py
--rw-rw-rw-   0        0        0      645 2023-06-20 10:48:44.000000 ssh_remote_control-0.1.3/src/ssh_remote_control/event.py
--rw-rw-rw-   0        0        0      159 2023-06-20 10:48:44.000000 ssh_remote_control-0.1.3/src/ssh_remote_control/helpers.py
--rw-rw-rw-   0        0        0     1313 2023-06-20 10:48:44.000000 ssh_remote_control-0.1.3/src/ssh_remote_control/locker.py
--rw-rw-rw-   0        0        0     3885 2023-06-20 10:48:44.000000 ssh_remote_control-0.1.3/src/ssh_remote_control/manager.py
--rw-rw-rw-   0        0        0     6074 2023-06-20 10:48:44.000000 ssh_remote_control-0.1.3/src/ssh_remote_control/sensor.py
-drwxrwxrwx   0        0        0        0 2023-06-20 10:53:44.474080 ssh_remote_control-0.1.3/src/ssh_remote_control.egg-info/
--rw-rw-rw-   0        0        0     1569 2023-06-20 10:53:44.000000 ssh_remote_control-0.1.3/src/ssh_remote_control.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      813 2023-06-20 10:53:44.000000 ssh_remote_control-0.1.3/src/ssh_remote_control.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 10:53:44.000000 ssh_remote_control-0.1.3/src/ssh_remote_control.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2023-06-20 10:53:44.000000 ssh_remote_control-0.1.3/src/ssh_remote_control.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-20 10:53:44.000000 ssh_remote_control-0.1.3/src/ssh_remote_control.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-22 08:15:17.497905 ssh_remote_control-0.1.4/
+-rw-rw-rw-   0        0        0     1084 2023-06-19 04:51:08.000000 ssh_remote_control-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     1569 2023-06-22 08:15:17.495635 ssh_remote_control-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      973 2023-06-20 06:12:24.000000 ssh_remote_control-0.1.4/README.md
+-rw-rw-rw-   0        0        0      846 2023-06-22 08:13:58.000000 ssh_remote_control-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-22 08:15:17.498638 ssh_remote_control-0.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-22 08:15:17.332215 ssh_remote_control-0.1.4/src/
+drwxrwxrwx   0        0        0        0 2023-06-22 08:15:17.395080 ssh_remote_control-0.1.4/src/ssh_remote_control/
+-rw-rw-rw-   0        0        0    10675 2023-06-22 08:11:21.000000 ssh_remote_control-0.1.4/src/ssh_remote_control/__init__.py
+-rw-rw-rw-   0        0        0     6576 2023-06-22 08:11:21.000000 ssh_remote_control-0.1.4/src/ssh_remote_control/command.py
+-rw-rw-rw-   0        0        0     2882 2023-06-22 08:11:21.000000 ssh_remote_control-0.1.4/src/ssh_remote_control/command_set.py
+drwxrwxrwx   0        0        0        0 2023-06-22 08:15:17.492650 ssh_remote_control-0.1.4/src/ssh_remote_control/default_command_sets/
+-rw-rw-rw-   0        0        0      163 2023-06-22 08:11:22.000000 ssh_remote_control-0.1.4/src/ssh_remote_control/default_command_sets/__init__.py
+-rw-rw-rw-   0        0        0     1006 2023-06-22 08:11:22.000000 ssh_remote_control-0.1.4/src/ssh_remote_control/default_command_sets/const.py
+-rw-rw-rw-   0        0        0     3987 2023-06-22 08:11:22.000000 ssh_remote_control-0.1.4/src/ssh_remote_control/default_command_sets/linux.py
+-rw-rw-rw-   0        0        0     3822 2023-06-22 08:11:22.000000 ssh_remote_control-0.1.4/src/ssh_remote_control/default_command_sets/windows_cmd.py
+-rw-rw-rw-   0        0        0     4087 2023-06-22 08:11:22.000000 ssh_remote_control-0.1.4/src/ssh_remote_control/default_command_sets/windows_ps.py
+-rw-rw-rw-   0        0        0      645 2023-06-22 08:11:21.000000 ssh_remote_control-0.1.4/src/ssh_remote_control/event.py
+-rw-rw-rw-   0        0        0      159 2023-06-22 08:11:21.000000 ssh_remote_control-0.1.4/src/ssh_remote_control/helpers.py
+-rw-rw-rw-   0        0        0     1313 2023-06-22 08:11:21.000000 ssh_remote_control-0.1.4/src/ssh_remote_control/locker.py
+-rw-rw-rw-   0        0        0     3885 2023-06-22 08:11:21.000000 ssh_remote_control-0.1.4/src/ssh_remote_control/manager.py
+-rw-rw-rw-   0        0        0     6667 2023-06-22 08:11:21.000000 ssh_remote_control-0.1.4/src/ssh_remote_control/sensor.py
+drwxrwxrwx   0        0        0        0 2023-06-22 08:15:17.465634 ssh_remote_control-0.1.4/src/ssh_remote_control.egg-info/
+-rw-rw-rw-   0        0        0     1569 2023-06-22 08:15:17.000000 ssh_remote_control-0.1.4/src/ssh_remote_control.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      813 2023-06-22 08:15:17.000000 ssh_remote_control-0.1.4/src/ssh_remote_control.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 08:15:17.000000 ssh_remote_control-0.1.4/src/ssh_remote_control.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       89 2023-06-22 08:15:17.000000 ssh_remote_control-0.1.4/src/ssh_remote_control.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-22 08:15:17.000000 ssh_remote_control-0.1.4/src/ssh_remote_control.egg-info/top_level.txt
```

### Comparing `ssh_remote_control-0.1.3/LICENSE` & `ssh_remote_control-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.1.3/PKG-INFO` & `ssh_remote_control-0.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssh_remote_control
-Version: 0.1.3
+Version: 0.1.4
 Summary: Control and monitor remote devices through SSH
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Project-URL: Homepage, https://github.com/zhbjsh/ssh-remote-control
 Project-URL: Bug Tracker, https://github.com/zhbjsh/ssh-remote-control/issues
 Keywords: ssh,command line,remote control
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ssh_remote_control-0.1.3/README.md` & `ssh_remote_control-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.1.3/pyproject.toml` & `ssh_remote_control-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ssh_remote_control"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="zhbjsh", email="zhbjsh@outlook.com" },
 ]
 description = "Control and monitor remote devices through SSH"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `ssh_remote_control-0.1.3/src/ssh_remote_control/__init__.py` & `ssh_remote_control-0.1.4/src/ssh_remote_control/__init__.py`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.1.3/src/ssh_remote_control/command.py` & `ssh_remote_control-0.1.4/src/ssh_remote_control/command.py`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.1.3/src/ssh_remote_control/command_set.py` & `ssh_remote_control-0.1.4/src/ssh_remote_control/command_set.py`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.1.3/src/ssh_remote_control/default_command_sets/const.py` & `ssh_remote_control-0.1.4/src/ssh_remote_control/default_command_sets/const.py`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.1.3/src/ssh_remote_control/default_command_sets/linux.py` & `ssh_remote_control-0.1.4/src/ssh_remote_control/default_command_sets/linux.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
                     value_type=int,
                     value_unit="MB",
                 )
             ],
             interval=30,
         ),
         SensorCommand(
-            "df -m | awk '/^\\/dev\\// {{print $6 \"|\" $4}}'",
+            "df -m | awk '/^\\/dev\\// {{print $4 \"|\" $6}}'",
             [
                 DynamicSensor(
                     SensorName.FREE_DISK_SPACE,
                     SensorKey.FREE_DISK_SPACE,
                     value_type=int,
                     value_unit="MB",
                     separator="|",
```

### Comparing `ssh_remote_control-0.1.3/src/ssh_remote_control/default_command_sets/windows_cmd.py` & `ssh_remote_control-0.1.4/src/ssh_remote_control/default_command_sets/windows_cmd.py`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.1.3/src/ssh_remote_control/default_command_sets/windows_ps.py` & `ssh_remote_control-0.1.4/src/ssh_remote_control/default_command_sets/windows_ps.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
                 )
             ],
             interval=30,
         ),
         SensorCommand(
             "Get-CimInstance Win32_LogicalDisk | "
             + "Select DeviceID, FreeSpace | ForEach-Object "
-            + '{{$_.DeviceID+"|"+[math]::Round($_.FreeSpace/1MB)}}',
+            + '{{[math]::Round($_.FreeSpace/1MB)+"|"+$_.DeviceID}}',
             [
                 DynamicSensor(
                     SensorName.FREE_DISK_SPACE,
                     SensorKey.FREE_DISK_SPACE,
                     value_type=int,
                     value_unit="MB",
                     separator="|",
```

### Comparing `ssh_remote_control-0.1.3/src/ssh_remote_control/event.py` & `ssh_remote_control-0.1.4/src/ssh_remote_control/event.py`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.1.3/src/ssh_remote_control/locker.py` & `ssh_remote_control-0.1.4/src/ssh_remote_control/locker.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import asyncio
-import inspect
 from collections.abc import Coroutine
 from functools import wraps
+import inspect
 
 
 def locked(coro: Coroutine):
     @wraps(coro)
     async def wrapper(instance: Locker, *args, **kwargs):
         async with instance.lock:
             return await coro(instance, *args, **kwargs)
```

### Comparing `ssh_remote_control-0.1.3/src/ssh_remote_control/manager.py` & `ssh_remote_control-0.1.4/src/ssh_remote_control/manager.py`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.1.3/src/ssh_remote_control/sensor.py` & `ssh_remote_control-0.1.4/src/ssh_remote_control/sensor.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,14 +35,32 @@
     if string.lower() in TRUE_STRINGS:
         return True
 
     if string.lower() in FALSE_STRINGS:
         return False
 
 
+class DynamicData:
+    """The DynamicData class"""
+
+    def __init__(
+        self,
+        sensor_name: str,
+        sensor_key: str,
+        data_value: str,
+        data_name: str,
+        data_id: str | None = None,
+    ) -> None:
+        data_key = name_to_key(data_name)
+        self.value_string = data_value
+        self.child_name = f"{sensor_name} {data_name}"
+        self.child_key = f"{sensor_key}_{data_key}"
+        self.child_id = data_id or data_key
+
+
 class Sensor:
     """The Sensor class."""
 
     value: Any | None = None
     last_known_value: Any | None = None
 
     def __init__(
@@ -58,18 +76,18 @@
         switch_off: Command | None = None,
         payload_on: str | None = None,
         payload_off: str | None = None,
         options: dict | None = None,
     ) -> None:
         self.name = name
         self.key = key or name_to_key(name)
+        self.child_id = child_id
         self.value_type = value_type or str
         self.value_unit = value_unit
         self.value_renderer = value_renderer
-        self.child_id = child_id
         self.switch_on = switch_on
         self.switch_off = switch_off
         self.payload_on = payload_on
         self.payload_off = payload_off
         self.options = options or {}
         self.on_update = Event()
 
@@ -154,41 +172,43 @@
         if data is None:
             for child in self.value:
                 child.set_value(None)
 
             self.on_update.notify(self)
             return
 
-        lines = [line.split(self.separator, 1) for line in data]
-        pairs = [pair for pair in lines if len(pair) == 2]
+        dynamic_data_list = [
+            DynamicData(self.name, self.key, *data_items)
+            for data_items in [line.split(self.separator, 2) for line in data]
+            if len(data_items) >= 2
+        ]
 
-        data_by_key = {
-            f"{self.key}_{name_to_key(child_id)}": (child_id, value_string)
-            for child_id, value_string in pairs
+        dynamic_data_by_key = {
+            dynamic_data.child_key: dynamic_data for dynamic_data in dynamic_data_list
         }
 
-        for key, (child_id, _) in data_by_key.items():
+        for key, dynamic_data in dynamic_data_by_key.items():
             if key not in self.children_by_key:
-                self.add_child(key, child_id)
+                self.add_child(dynamic_data)
 
         for child in self.value:
-            if child.key in data_by_key:
-                _, value_string = data_by_key[child.key]
-                child.set_value(value_string)
+            if child.key in dynamic_data_by_key:
+                dynamic_data = dynamic_data_by_key[child.key]
+                child.set_value(dynamic_data.value_string)
             else:
                 self.remove_child(child)
 
         self.on_update.notify(self)
 
-    def add_child(self, key: str, child_id: str) -> None:
+    def add_child(self, dynamic_data: DynamicData) -> None:
         """Add a child."""
         child = Sensor(
-            f"{self.name} {child_id}",
-            key,
-            child_id,
+            dynamic_data.child_name,
+            dynamic_data.child_key,
+            dynamic_data.child_id,
             value_type=self.value_type,
             value_unit=self.value_unit,
             value_renderer=self.value_renderer,
             switch_on=self.switch_on,
             switch_off=self.switch_off,
             options=self.options,
         )
```

### Comparing `ssh_remote_control-0.1.3/src/ssh_remote_control.egg-info/PKG-INFO` & `ssh_remote_control-0.1.4/src/ssh_remote_control.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssh-remote-control
-Version: 0.1.3
+Version: 0.1.4
 Summary: Control and monitor remote devices through SSH
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Project-URL: Homepage, https://github.com/zhbjsh/ssh-remote-control
 Project-URL: Bug Tracker, https://github.com/zhbjsh/ssh-remote-control/issues
 Keywords: ssh,command line,remote control
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ssh_remote_control-0.1.3/src/ssh_remote_control.egg-info/SOURCES.txt` & `ssh_remote_control-0.1.4/src/ssh_remote_control.egg-info/SOURCES.txt`

 * *Files identical despite different names*

