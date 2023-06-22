# Comparing `tmp/yaqd-adafruit-2022.6.0.tar.gz` & `tmp/yaqd_adafruit-2023.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaqd-adafruit-2022.6.0.tar", last modified: Wed Jun 15 21:03:36 2022, max compression
+gzip compressed data, was "yaqd_adafruit-2023.6.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `yaqd-adafruit-2022.6.0.tar` & `yaqd_adafruit-2023.6.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0      429 2022-06-15 21:03:29.183697 yaqd-adafruit-2022.6.0/.github/workflows/python-mypy.yml
--rw-r--r--   0        0        0      793 2022-06-15 21:03:29.183697 yaqd-adafruit-2022.6.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      707 2022-06-15 21:03:29.183697 yaqd-adafruit-2022.6.0/.github/workflows/run-entry-points.yml
--rw-r--r--   0        0        0      446 2022-06-15 21:03:29.183697 yaqd-adafruit-2022.6.0/.gitignore
--rw-r--r--   0        0        0      647 2022-06-15 21:03:29.183697 yaqd-adafruit-2022.6.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      553 2022-06-15 21:03:29.183697 yaqd-adafruit-2022.6.0/CHANGELOG.md
--rw-r--r--   0        0        0     7633 2022-06-15 21:03:29.183697 yaqd-adafruit-2022.6.0/LICENSE
--rw-r--r--   0        0        0      732 2022-06-15 21:03:29.183697 yaqd-adafruit-2022.6.0/README.md
--rw-r--r--   0        0        0     1328 2022-06-15 21:03:29.183697 yaqd-adafruit-2022.6.0/pyproject.toml
--rw-r--r--   0        0        0        9 2022-06-15 21:03:29.183697 yaqd-adafruit-2022.6.0/yaqd_adafruit/VERSION
--rw-r--r--   0        0        0       69 2022-06-15 21:03:29.183697 yaqd-adafruit-2022.6.0/yaqd_adafruit/__init__.py
--rw-r--r--   0        0        0      493 2022-06-15 21:03:29.183697 yaqd-adafruit-2022.6.0/yaqd_adafruit/__version__.py
--rw-r--r--   0        0        0     3699 2022-06-15 21:03:29.183697 yaqd-adafruit-2022.6.0/yaqd_adafruit/_adafruit_stepper_motor_hat.py
--rw-r--r--   0        0        0    11116 2022-06-15 21:03:29.183697 yaqd-adafruit-2022.6.0/yaqd_adafruit/adafruit-stepper-motor-hat.avpr
--rw-r--r--   0        0        0      997 2022-06-15 21:03:29.183697 yaqd-adafruit-2022.6.0/yaqd_adafruit/adafruit-stepper-motor-hat.toml
--rw-r--r--   0        0        0     1756 1970-01-01 00:00:00.000000 yaqd-adafruit-2022.6.0/PKG-INFO
+-rw-r--r--   0        0        0      429 2023-06-22 18:13:17.169432 yaqd_adafruit-2023.6.0/.github/workflows/python-mypy.yml
+-rw-r--r--   0        0        0      793 2023-06-22 18:13:17.169432 yaqd_adafruit-2023.6.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      707 2023-06-22 18:13:17.169432 yaqd_adafruit-2023.6.0/.github/workflows/run-entry-points.yml
+-rw-r--r--   0        0        0      446 2023-06-22 18:13:17.169432 yaqd_adafruit-2023.6.0/.gitignore
+-rw-r--r--   0        0        0      656 2023-06-22 18:13:17.169432 yaqd_adafruit-2023.6.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      726 2023-06-22 18:13:17.169432 yaqd_adafruit-2023.6.0/CHANGELOG.md
+-rw-r--r--   0        0        0     7633 2023-06-22 18:13:17.169432 yaqd_adafruit-2023.6.0/LICENSE
+-rw-r--r--   0        0        0      732 2023-06-22 18:13:17.169432 yaqd_adafruit-2023.6.0/README.md
+-rw-r--r--   0        0        0      287 2023-06-22 18:13:17.169432 yaqd_adafruit-2023.6.0/example-yaq-configs/adafruit-stepper-motor-hat/opa4-delays.toml
+-rw-r--r--   0        0        0     1328 2023-06-22 18:13:17.169432 yaqd_adafruit-2023.6.0/pyproject.toml
+-rw-r--r--   0        0        0        9 2023-06-22 18:13:17.169432 yaqd_adafruit-2023.6.0/yaqd_adafruit/VERSION
+-rw-r--r--   0        0        0       69 2023-06-22 18:13:17.169432 yaqd_adafruit-2023.6.0/yaqd_adafruit/__init__.py
+-rw-r--r--   0        0        0      493 2023-06-22 18:13:17.173432 yaqd_adafruit-2023.6.0/yaqd_adafruit/__version__.py
+-rw-r--r--   0        0        0     4246 2023-06-22 18:13:17.173432 yaqd_adafruit-2023.6.0/yaqd_adafruit/_adafruit_stepper_motor_hat.py
+-rw-r--r--   0        0        0    11728 2023-06-22 18:13:17.173432 yaqd_adafruit-2023.6.0/yaqd_adafruit/adafruit-stepper-motor-hat.avpr
+-rw-r--r--   0        0        0     1395 2023-06-22 18:13:17.173432 yaqd_adafruit-2023.6.0/yaqd_adafruit/adafruit-stepper-motor-hat.toml
+-rw-r--r--   0        0        0     1756 1970-01-01 00:00:00.000000 yaqd_adafruit-2023.6.0/PKG-INFO
```

### Comparing `yaqd-adafruit-2022.6.0/.github/workflows/python-publish.yml` & `yaqd_adafruit-2023.6.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `yaqd-adafruit-2022.6.0/.github/workflows/run-entry-points.yml` & `yaqd_adafruit-2023.6.0/.github/workflows/run-entry-points.yml`

 * *Files identical despite different names*

### Comparing `yaqd-adafruit-2022.6.0/CHANGELOG.md` & `yaqd_adafruit-2023.6.0/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/).
 
 ## [Unreleased]
 
+## [2023.6.0]
+
+### added
+- example config file for adafruit-stepper-motor-hat daemon
+
 ## [2022.6.0]
 
 ### Changed
 - migrated to Github
 
 ### Fixed
 - document known hardware
 
 ## [2022.2.0]
 
 ### Added
 - initial release
 
-[Unreleased]: https://github.com/yaq-project/yaqd-adafruit/compare/v2022.6.0...main
+[Unreleased]: https://github.com/yaq-project/yaqd-adafruit/compare/v2023.6.0...main
+[2023.6.0]: https://github.com/yaq-project/yaqd-adafruit/compare/v2022.6.0...v2023.6.0
 [2022.6.0]: https://github.com/yaq-project/yaqd-adafruit/compare/v2022.2.0...v2022.6.0
 [2022.2.0]: https://github.com/yaq-project/yaqd-adafruit/releases/tag/v2022.2.0
```

### Comparing `yaqd-adafruit-2022.6.0/LICENSE` & `yaqd_adafruit-2023.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yaqd-adafruit-2022.6.0/README.md` & `yaqd_adafruit-2023.6.0/README.md`

 * *Files identical despite different names*

### Comparing `yaqd-adafruit-2022.6.0/pyproject.toml` & `yaqd_adafruit-2023.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yaqd-adafruit-2022.6.0/yaqd_adafruit/_adafruit_stepper_motor_hat.py` & `yaqd_adafruit-2023.6.0/yaqd_adafruit/_adafruit_stepper_motor_hat.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,59 +1,76 @@
 import asyncio
 from typing import Dict, Any
 
 import gpiozero  # type: ignore
 from yaqd_core import UsesI2C, UsesSerial, HasLimits, HasPosition, IsHomeable, IsDaemon
+from adafruit_motor import stepper  # type: ignore
+
+
+styles = {
+    "DOUBLE": stepper.DOUBLE,
+    "SINGLE": stepper.SINGLE,
+    "INTERLEAVE": stepper.INTERLEAVE,
+    "MICROSTEP": stepper.MICROSTEP,
+}
 
 
 class AdafruitStepperMotorHat(UsesI2C, UsesSerial, IsHomeable, HasLimits, HasPosition, IsDaemon):
     _kind = "adafruit-stepper-motor-hat"
 
     def __init__(self, name, config, config_filepath):
         # adafruit_motorkit raises an exception if not rpi
         from adafruit_motorkit import MotorKit  # type: ignore
 
         super().__init__(name, config, config_filepath)
-        self._kit = MotorKit(address=config["i2c_addr"], steppers_microsteps=config["microsteps"])
+        self.microsteps = config["microsteps"]
+        self._kit = MotorKit(
+            address=config["i2c_addr"],
+            steppers_microsteps=self.microsteps,
+        )
         self._stepper = getattr(self._kit, f"stepper{config['stepper_index']}")
+        if config["style"] in ["DOUBLE", "SINGLE"]:  # full steps only
+            self.step_size = self.microsteps
+        elif config["style"] == "INTERLEAVE":  # half stepping
+            self.step_size = self.microsteps // 2
+        elif config["style"] == "MICROSTEP":  # microstepping
+            self.step_size = 1
+        self.style = styles[config["style"]]
         self.steps_per_unit = config["steps_per_unit"]
         self._units = config["units"]
-        self.microsteps = config["microsteps"]
         self._lock = asyncio.Lock()
         self._lower_pin = gpiozero.InputDevice(config["lower_limit_switch"]["pin"], pull_up=True)
         if config.get("upper_limit_switch"):
             self._upper_pin = gpiozero.InputDevice(
                 config["upper_limit_switch"]["pin"], pull_up=True
             )
 
-    async def _do_step(self, backward=False):
-        from adafruit_motor import stepper  # type: ignore
-
-        steps = self.to_steps(self._state["position"])
+    def _do_step(self, backward=False):
+        steps = self.to_usteps(self._state["position"])
         direction = stepper.BACKWARD if backward else stepper.FORWARD
-        if direction == stepper.BACKWARD and await self._get_lower_limit_switch():
+        if direction == stepper.BACKWARD and self._get_lower_limit_switch():
             return
-        elif direction == stepper.FORWARD and await self._get_upper_limit_switch():
+        elif direction == stepper.FORWARD and self._get_upper_limit_switch():
             return
-        self._stepper.onestep(direction=direction, style=stepper.MICROSTEP)
-        steps += 1 if direction == stepper.FORWARD else -1
+        self._stepper.onestep(direction=direction, style=self.style)
+        steps += self.step_size if direction == stepper.FORWARD else -self.step_size
         self._state["position"] = self.to_units(steps)
         self.logger.debug(f"{self._state['position']}")
 
     def to_units(self, usteps):
         return usteps / self.steps_per_unit / self.microsteps
 
-    def to_steps(self, units):
+    def to_usteps(self, units):
         return round(units * self.steps_per_unit * self.microsteps)
 
-    async def _get_lower_limit_switch(self):
+    def _get_lower_limit_switch(self):
         # TODO: invert
         return self._lower_pin.value
 
-    async def _get_upper_limit_switch(self):
+    def _get_upper_limit_switch(self):
         if not self._config.get("upper_limit_switch"):
             return False
         # TODO: invert
         return self._upper_pin.value
 
     def home(self):
         self._busy = True
@@ -61,38 +78,38 @@
 
     async def _home(self):
         prev_position = self._state["position"]
         async with self._lock:
             self._busy = True
             while True:
                 await asyncio.sleep(0)
-                await self._do_step(backward=True)
+                self._do_step(backward=True)
                 if self._state["position"] == prev_position:
                     break
                 prev_position = self._state["position"]
             self._state["position"] = 0
 
     def _set_position(self, position):
         # destination gets set by parent
         # update state actually steps motor
         pass
 
     async def update_state(self):
         while True:
             async with self._lock:
-                while self.to_steps(self._state["position"]) != self.to_steps(
-                    self._state["destination"]
+                while (
+                    abs(self.to_usteps(self._state["position"] - self._state["destination"]))
+                    >= self.step_size
                 ):
                     self._busy = True
                     await asyncio.sleep(0)
-                    await self._do_step(
-                        self.to_steps(self._state["position"])
-                        > self.to_steps(self._state["destination"])
+                    self._do_step(
+                        self.to_usteps(self._state["position"])
+                        > self.to_usteps(self._state["destination"])
                     )
-
                 self._busy = False
             await self._busy_sig.wait()
 
     def direct_serial_write(self, msg):
         pass
 
     def close(self):
```

### Comparing `yaqd-adafruit-2022.6.0/yaqd_adafruit/adafruit-stepper-motor-hat.avpr` & `yaqd_adafruit-2023.6.0/yaqd_adafruit/adafruit-stepper-motor-hat.avpr`

 * *Files 6% similar despite different names*

```diff
@@ -56,14 +56,15 @@
             "type": [
                 "null",
                 "string"
             ]
         },
         "microsteps": {
             "default": 16,
+            "doc": "Number of microsteps between full steps. Default is 16.",
             "type": "int"
         },
         "model": {
             "default": null,
             "origin": "is-daemon",
             "type": [
                 "null",
@@ -99,14 +100,19 @@
         "stepper_index": {
             "type": "int"
         },
         "steps_per_unit": {
             "default": 0.5555555555556,
             "type": "double"
         },
+        "style": {
+            "default": "DOUBLE",
+            "doc": "Style of step to take. Default is 'DOUBLE'.",
+            "type": "step_style"
+        },
         "units": {
             "default": "deg",
             "type": "string"
         },
         "upper_limit_port": {
             "default": null,
             "type": [
@@ -121,14 +127,15 @@
         "raspberry-pi:4b"
     ],
     "installation": {
         "PyPI": "https://pypi.org/project/yaqd-adafruit/"
     },
     "links": {
         "bugtracker": "https://github.com/yaq-project/yaqd-adafruit/-/issues",
+        "example-configs": "https://github.com/yaq-project/yaqd-adafruit/tree/main/example-yaq-configs/adafruit-stepper-motor-hat",
         "source": "https://github.com/yaq-project/yaqd-adafruit"
     },
     "messages": {
         "busy": {
             "doc": "Returns true if daemon is currently busy.",
             "origin": "is-daemon",
             "request": [],
@@ -255,32 +262,32 @@
                 }
             ],
             "response": "null"
         }
     },
     "properties": {
         "destination": {
-            "control_kind": "normal",
+            "control_kind": "hinted",
             "dynamic": true,
             "getter": "get_destination",
-            "limits_getter": null,
+            "limits_getter": "get_limits",
             "options_getter": null,
             "record_kind": "data",
-            "setter": null,
+            "setter": "set_position",
             "type": "double",
             "units_getter": "get_units"
         },
         "position": {
             "control_kind": "hinted",
             "dynamic": true,
             "getter": "get_position",
             "limits_getter": "get_limits",
             "options_getter": null,
             "record_kind": "data",
-            "setter": "set_position",
+            "setter": null,
             "type": "double",
             "units_getter": "get_units"
         }
     },
     "protocol": "adafruit-stepper-motor-hat",
     "requires": [],
     "state": {
@@ -326,14 +333,24 @@
                     "type": "boolean"
                 }
             ],
             "name": "limit_switch",
             "type": "record"
         },
         {
+            "name": "step_style",
+            "symbols": [
+                "DOUBLE",
+                "SINGLE",
+                "INTERLEAVE",
+                "MICROSTEP"
+            ],
+            "type": "enum"
+        },
+        {
             "fields": [
                 {
                     "name": "shape",
                     "type": {
                         "items": "int",
                         "type": "array"
                     }
```

### Comparing `yaqd-adafruit-2022.6.0/yaqd_adafruit/adafruit-stepper-motor-hat.toml` & `yaqd_adafruit-2023.6.0/yaqd_adafruit/adafruit-stepper-motor-hat.toml`

 * *Files 25% similar despite different names*

```diff
@@ -2,24 +2,30 @@
 doc = ""
 traits = ["uses-i2c", "uses-serial", "has-limits", "has-position", "is-homeable", "is-daemon"]
 hardware = ["adafruit:2348", "raspberry-pi:4b"]
 
 [links]
 source = "https://github.com/yaq-project/yaqd-adafruit"
 bugtracker = "https://github.com/yaq-project/yaqd-adafruit/-/issues"
+example-configs = "https://github.com/yaq-project/yaqd-adafruit/tree/main/example-yaq-configs/adafruit-stepper-motor-hat"
 
 [installation]
 PyPI = "https://pypi.org/project/yaqd-adafruit/"
 
 [[types]]
 name = "limit_switch"
 type = "record"
 fields = [{"name"="pin", "type"="int", "doc"="GPIO Pin"},
 	  {"name"="invert", "type"="boolean", "default"=false}]
 
+[[types]]
+name = "step_style"
+type = "enum"
+symbols = ["DOUBLE", "SINGLE", "INTERLEAVE", "MICROSTEP"]
+
 [config]
 
 [config.i2c_addr]
 default = 0x60
 
 [config.steps_per_unit]
 type = "double"
@@ -30,21 +36,27 @@
 default = "deg"
 
 [config.lower_limit_switch]
 type = "limit_switch"
 
 [config.microsteps]
 type = "int"
+doc = "Number of microsteps between full steps. Default is 16."
 default = 16
 
+[config.style]
+type = "step_style"
+doc = "Style of step to take. Default is 'DOUBLE'."
+default = "DOUBLE"
+
 [config.stepper_index]
 type = "int"
 
 [config.upper_limit_port]
 type = ["null", "limit_switch"]
 default = "__null__"
 
 [state]
 [state.position]
 default = 0
 [state.destination]
-default=0
+default = 0
```

### Comparing `yaqd-adafruit-2022.6.0/PKG-INFO` & `yaqd_adafruit-2023.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaqd-adafruit
-Version: 2022.6.0
+Version: 2023.6.0
 Summary: yaq daemons for Adafruit products
 Home-page: https://yaq.fyi
 Author: yaq developers
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
```

