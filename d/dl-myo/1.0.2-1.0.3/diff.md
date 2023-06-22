# Comparing `tmp/dl_myo-1.0.2.tar.gz` & `tmp/dl_myo-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dl_myo-1.0.2.tar", max compression
+gzip compressed data, was "dl_myo-1.0.3.tar", max compression
```

## Comparing `dl_myo-1.0.2.tar` & `dl_myo-1.0.3.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0    35123 2023-06-20 18:42:20.173442 dl_myo-1.0.2/LICENSE
--rw-r--r--   0        0        0     3837 2023-06-20 18:42:20.173442 dl_myo-1.0.2/README.md
--rw-r--r--   0        0        0      770 2023-06-20 18:42:20.173442 dl_myo-1.0.2/myo/__init__.py
--rw-r--r--   0        0        0    10915 2023-06-20 18:42:20.173442 dl_myo-1.0.2/myo/client.py
--rw-r--r--   0        0        0     3293 2023-06-20 18:42:20.173442 dl_myo-1.0.2/myo/commands.py
--rw-r--r--   0        0        0      504 2023-06-20 18:42:20.173442 dl_myo-1.0.2/myo/constants.py
--rw-r--r--   0        0        0     4331 2023-06-20 18:42:20.173442 dl_myo-1.0.2/myo/core.py
--rw-r--r--   0        0        0     5805 2023-06-20 18:42:20.173442 dl_myo-1.0.2/myo/profile.py
--rw-r--r--   0        0        0     9074 2023-06-20 18:42:20.177442 dl_myo-1.0.2/myo/types.py
--rw-r--r--   0        0        0       22 2023-06-20 18:42:20.177442 dl_myo-1.0.2/myo/version.py
--rw-r--r--   0        0        0     3164 2023-06-20 18:42:45.717558 dl_myo-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     4423 1970-01-01 00:00:00.000000 dl_myo-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    35123 2023-06-22 16:31:30.630862 dl_myo-1.0.3/LICENSE
+-rw-r--r--   0        0        0     3837 2023-06-22 16:31:30.630862 dl_myo-1.0.3/README.md
+-rw-r--r--   0        0        0      751 2023-06-22 16:31:30.630862 dl_myo-1.0.3/myo/__init__.py
+-rw-r--r--   0        0        0     3293 2023-06-22 16:31:30.630862 dl_myo-1.0.3/myo/commands.py
+-rw-r--r--   0        0        0      504 2023-06-22 16:31:30.630862 dl_myo-1.0.3/myo/constants.py
+-rw-r--r--   0        0        0    15170 2023-06-22 16:31:30.630862 dl_myo-1.0.3/myo/core.py
+-rw-r--r--   0        0        0     5805 2023-06-22 16:31:30.630862 dl_myo-1.0.3/myo/profile.py
+-rw-r--r--   0        0        0     9074 2023-06-22 16:31:30.630862 dl_myo-1.0.3/myo/types.py
+-rw-r--r--   0        0        0       22 2023-06-22 16:31:30.630862 dl_myo-1.0.3/myo/version.py
+-rw-r--r--   0        0        0     3210 2023-06-22 16:31:50.235024 dl_myo-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4423 1970-01-01 00:00:00.000000 dl_myo-1.0.3/PKG-INFO
```

### Comparing `dl_myo-1.0.2/LICENSE` & `dl_myo-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dl_myo-1.0.2/README.md` & `dl_myo-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `dl_myo-1.0.2/myo/__init__.py` & `dl_myo-1.0.3/myo/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """
     dl-myo
     ------
     Yet another MyoConnect alternative without dongles.
 """
 from __future__ import absolute_import, annotations
 
-from .client import MyoClient
-from .core import Myo
+from .core import Myo, MyoClient
 from .profile import Handle
 from .types import (
     ClassifierEvent,
     ClassifierMode,
     EMGData,
     EMGMode,
     FVData,
```

### Comparing `dl_myo-1.0.2/myo/client.py` & `dl_myo-1.0.3/myo/core.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,45 @@
 """
-    myo.client
+    myo.core
     ----------------
-    MyoClient is a wrapper class to handle the connection to Myo devices.
+    The core Myo BLE device manager (Myo) and
+    a wrapper class (MyoClient) to handle the connection to Myo devices
+
 """
 import asyncio
 import binascii
 import logging
 import json
-
-from bleak import BleakClient
+from bleak import BleakClient, BleakScanner
 from bleak.backends.characteristic import BleakGATTCharacteristic
+from bleak.backends.device import BLEDevice
+from bleak.backends.scanner import AdvertisementData
+
 
 from .constants import (
     RGB_CYAN,
     RGB_PINK,
     RGB_YELLOW,
     RGB_GREEN,
 )
-from .core import Myo
-from .profile import Handle
+from .commands import (
+    Command,
+    SetMode,
+    Vibrate,
+    DeepSleep,
+    LED,
+    Vibrate2,
+    SetSleepMode,
+    Unlock,
+    UserAction,
+)
+from .profile import (
+    GATTProfile,
+    Handle,
+)
 from .types import (
     ClassifierEvent,
     ClassifierMode,
     EMGData,
     EMGMode,
     FVData,
     FirmwareInfo,
@@ -30,20 +47,148 @@
     IMUData,
     IMUMode,
     MotionEvent,
     SleepMode,
     VibrationType,
 )
 
+
 logger = logging.getLogger(__name__)
 
 
+class Myo:
+    __slots__ = "_device"
+
+    def __init__(self):
+        pass
+
+    @property
+    def device(self) -> BLEDevice:
+        return self._device
+
+    @classmethod
+    async def with_mac(cls, mac: str):
+        def match_myo_mac(device: BLEDevice, _: AdvertisementData):
+            if mac.lower() == device.address.lower():
+                return True
+            return False
+
+        self = cls()
+        try:
+            # scan the device
+            self._device = await BleakScanner.find_device_by_filter(match_myo_mac, cb=dict(use_bdaddr=True))
+            if self.device is None:
+                logger.error(f"could not find device with address {mac}")
+                return None
+        except Exception as e:
+            logger.error("the mac address may be invalid", e)
+            return None
+
+        return self
+
+    @classmethod
+    async def with_uuid(cls):
+        def match_myo_uuid(_: BLEDevice, adv: AdvertisementData):
+            if str(GATTProfile.MYO_SERVICE).lower() in adv.service_uuids:
+                return True
+            return False
+
+        self = cls()
+        # scan the device
+        self._device = await BleakScanner.find_device_by_filter(match_myo_uuid, cb=dict(use_bdaddr=True))
+        if self.device is None:
+            logger.error(f"could not find device with service UUID {GATTProfile.MYO_SERVICE}")
+            return None
+
+        return self
+
+    async def battery_level(self, client: BleakClient):
+        """
+        Battery Level Characteristic
+        """
+        val = await client.read_gatt_char(Handle.BATTERY_LEVEL.value)
+        return ord(val)
+
+    async def command(self, client: BleakClient, cmd: Command):
+        """
+        Command Characteristic
+        """
+        await client.write_gatt_char(Handle.COMMAND.value, cmd.data, True)
+
+    async def deep_sleep(self, client: BleakClient):
+        """
+        Deep Sleep Command
+        """
+        await self.command(client, DeepSleep())
+
+    async def led(self, client: BleakClient, *args):
+        """
+        LED Command
+            - set leds color
+
+        *args: [logoR, logoG, logoB], [lineR, lineG, lineB]
+        """
+
+        if not isinstance(args, tuple) or len(args) != 2:
+            raise Exception(f"Unknown payload for LEDs: {args}")
+
+        for lst in args:
+            if any(not isinstance(v, int) for v in lst):
+                raise Exception(f"Values must be int 0-255: {lst}")
+
+        await self.command(client, LED(args[0], args[1]))
+
+    async def set_mode(self, client: BleakClient, emg_mode, imu_mode, classifier_mode):
+        """
+        Set Mode Command
+            - configures EMG, IMU, and Classifier modes
+        """
+        await self.command(client, SetMode(emg_mode, imu_mode, classifier_mode))
+
+    async def set_sleep_mode(self, client: BleakClient, sleep_mode):
+        """
+        Set Sleep Mode Command
+        """
+        await self.command(client, SetSleepMode(sleep_mode))
+
+    async def unlock(self, client: BleakClient, unlock_type):
+        """
+        Unlock Command
+        """
+        await self.command(client, Unlock(unlock_type))
+
+    async def user_action(self, client: BleakClient, user_action_type):
+        """
+        User Action Command
+        """
+        await self.command(client, UserAction(user_action_type))
+
+    async def vibrate(self, client: BleakClient, vibration_type):
+        """
+        Vibrate Command
+        """
+        await self.command(client, Vibrate(vibration_type))
+
+    async def vibrate2(self, client: BleakClient, duration, strength):
+        """
+        Vibrate2 Command
+        """
+        await self.command(client, Vibrate2(duration, strength))
+
+    async def write(self, client: BleakClient, handle, value):
+        """
+        Write characteristic
+        """
+        await client.write_gatt_char(handle, value, True)
+
+
 class MyoClient:
     def __init__(self):
         self.m = None
+        self.aggregate_emg = False
         self.classifier_mode = None
         self.emg_mode = None
         self.imu_mode = None
         self._client = None
 
     @classmethod
     async def with_device(cls, mac=None):
@@ -94,27 +239,14 @@
             logger.error("connection is already closed")
 
         # disconnect from the device
         await self._client.disconnect()
         self._client = None
         logger.info(f"disconnected from {self.device.name}")
 
-    async def emg_data_aggregate(self, handle, emg_data: EMGData):
-        """
-        <> aggregate the raw EMG data channels
-        """
-        if handle in [
-            Handle.EMG0_DATA,
-            Handle.EMG1_DATA,
-            Handle.EMG2_DATA,
-            Handle.EMG3_DATA,
-        ]:
-            await self.on_emg_data(emg_data.sample1)
-            await self.on_emg_data(emg_data.sample2)
-
     async def get_services(self, indent=1) -> str:
         """
         <> fetch available services as dict
         """
         sd = {}
         for service in self._client.services:  # BleakGATTServiceCollection
             try:
@@ -145,15 +277,21 @@
             - color: myo.constants.RGB_*
         """
         await self.m.led(self._client, color, color)
 
     async def on_classifier_event(self, ce: ClassifierEvent):
         raise NotImplementedError()
 
-    async def on_emg_data(self, emg):  # data: list of 8 8-bit unsigned short
+    async def on_emg_data(self, emg: EMGData):  # data: list of 8 8-bit unsigned short
+        raise NotImplementedError()
+
+    async def on_emg_data_aggregated(self, data):
+        """
+        <> aggregate the raw EMG data channels
+        """
         raise NotImplementedError()
 
     async def on_fv_data(self, fvd: FVData):
         raise NotImplementedError()
 
     async def on_imu_data(self, imu: IMUData):
         raise NotImplementedError()
@@ -171,16 +309,26 @@
             await self.on_classifier_event(ClassifierEvent(data))
         elif handle == Handle.FV_DATA:
             await self.on_fv_data(FVData(data))
         elif handle == Handle.IMU_DATA:
             await self.on_imu_data(IMUData(data))
         elif handle == Handle.MOTION_EVENT:
             await self.on_motion_event(MotionEvent(data))
-        else:  # on EMG[0-3]_DATA handle
-            await self.emg_data_aggregate(handle, EMGData(data))
+        elif handle in [
+            Handle.EMG0_DATA,
+            Handle.EMG1_DATA,
+            Handle.EMG2_DATA,
+            Handle.EMG3_DATA,
+        ]:
+            emg = EMGData(data)
+            if self.aggregate_emg:
+                await self.on_emg_data_aggregated(emg.sample1)
+                await self.on_emg_data_aggregated(emg.sample2)
+            else:
+                await self.on_emg_data(emg)
 
     async def set_mode(self, emg_mode, imu_mode, classifier_mode):
         """
         Set Mode Command
             - configures EMG, IMU, and Classifier modes
         """
         await self.m.set_mode(self._client, emg_mode, imu_mode, classifier_mode)
```

### Comparing `dl_myo-1.0.2/myo/commands.py` & `dl_myo-1.0.3/myo/commands.py`

 * *Files identical despite different names*

### Comparing `dl_myo-1.0.2/myo/profile.py` & `dl_myo-1.0.3/myo/profile.py`

 * *Files identical despite different names*

### Comparing `dl_myo-1.0.2/myo/types.py` & `dl_myo-1.0.3/myo/types.py`

 * *Files identical despite different names*

### Comparing `dl_myo-1.0.2/pyproject.toml` & `dl_myo-1.0.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -79,40 +79,43 @@
 [tool.ruff.per-file-ignores]
 # Tests can use magic values, assertions, and relative imports
 "tests/**/*" = ["PLR2004", "S101", "TID252"]
 "myo/__init__.py" = ["F401"]
 
 [tool.coverage.run]
 branch = true
-omit = []
+omit = [
+    "myo/core.py"
+]
 
 [tool.coverage.report]
 exclude_lines = [
   "no cov",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
 ]
 
 [tool.poetry]
 name = "dl-myo"
-version = "1.0.2"
+version = "1.0.3"
 description = "Yet another MyoConnect alternative without dongles"
 authors = ["Iori Mizutani <iomz@sazanka.io>"]
 license = "GPLv3"
 readme = "README.md"
 packages = [{include = "myo"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 bleak = "^0.20.2"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pytest = "^7.3.2"
 pytest-cov = "^4.1.0"
+pytest-asyncio = "^0.21.0"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "semver"
 
 [build-system]
```

### Comparing `dl_myo-1.0.2/PKG-INFO` & `dl_myo-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dl-myo
-Version: 1.0.2
+Version: 1.0.3
 Summary: Yet another MyoConnect alternative without dongles
 License: GPLv3
 Author: Iori Mizutani
 Author-email: iomz@sazanka.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

