# Comparing `tmp/universal-silabs-flasher-0.0.8.tar.gz` & `tmp/universal-silabs-flasher-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "universal-silabs-flasher-0.0.8.tar", last modified: Mon Dec  5 21:42:58 2022, max compression
+gzip compressed data, was "universal-silabs-flasher-0.0.9.tar", last modified: Wed Feb  8 07:47:31 2023, max compression
```

## Comparing `universal-silabs-flasher-0.0.8.tar` & `universal-silabs-flasher-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 21:42:58.382435 universal-silabs-flasher-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2022-12-05 21:42:55.000000 universal-silabs-flasher-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2022-12-05 21:42:58.382435 universal-silabs-flasher-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2022-12-05 21:42:55.000000 universal-silabs-flasher-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2022-12-05 21:42:55.000000 universal-silabs-flasher-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2022-12-05 21:42:58.382435 universal-silabs-flasher-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2022-12-05 21:42:55.000000 universal-silabs-flasher-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 21:42:58.382435 universal-silabs-flasher-0.0.8/universal_silabs_flasher/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2022-12-05 21:42:55.000000 universal-silabs-flasher-0.0.8/universal_silabs_flasher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2022-12-05 21:42:55.000000 universal-silabs-flasher-0.0.8/universal_silabs_flasher/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2022-12-05 21:42:55.000000 universal-silabs-flasher-0.0.8/universal_silabs_flasher/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    11697 2022-12-05 21:42:55.000000 universal-silabs-flasher-0.0.8/universal_silabs_flasher/cpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11483 2022-12-05 21:42:55.000000 universal-silabs-flasher-0.0.8/universal_silabs_flasher/cpc_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2022-12-05 21:42:55.000000 universal-silabs-flasher-0.0.8/universal_silabs_flasher/emberznet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7300 2022-12-05 21:42:55.000000 universal-silabs-flasher-0.0.8/universal_silabs_flasher/flash.py
--rw-r--r--   0 runner    (1001) docker     (123)     9120 2022-12-05 21:42:55.000000 universal-silabs-flasher-0.0.8/universal_silabs_flasher/flasher.py
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2022-12-05 21:42:55.000000 universal-silabs-flasher-0.0.8/universal_silabs_flasher/gbl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5383 2022-12-05 21:42:55.000000 universal-silabs-flasher-0.0.8/universal_silabs_flasher/gecko_bootloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2022-12-05 21:42:55.000000 universal-silabs-flasher-0.0.8/universal_silabs_flasher/xmodemcrc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 21:42:58.382435 universal-silabs-flasher-0.0.8/universal_silabs_flasher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2022-12-05 21:42:58.000000 universal-silabs-flasher-0.0.8/universal_silabs_flasher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      743 2022-12-05 21:42:58.000000 universal-silabs-flasher-0.0.8/universal_silabs_flasher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-05 21:42:58.000000 universal-silabs-flasher-0.0.8/universal_silabs_flasher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2022-12-05 21:42:58.000000 universal-silabs-flasher-0.0.8/universal_silabs_flasher.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      255 2022-12-05 21:42:58.000000 universal-silabs-flasher-0.0.8/universal_silabs_flasher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-05 21:42:58.000000 universal-silabs-flasher-0.0.8/universal_silabs_flasher.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 07:47:31.014967 universal-silabs-flasher-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-02-08 07:47:25.000000 universal-silabs-flasher-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-02-08 07:47:31.014967 universal-silabs-flasher-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-02-08 07:47:25.000000 universal-silabs-flasher-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-02-08 07:47:25.000000 universal-silabs-flasher-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-02-08 07:47:31.014967 universal-silabs-flasher-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-02-08 07:47:25.000000 universal-silabs-flasher-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 07:47:31.010967 universal-silabs-flasher-0.0.9/universal_silabs_flasher/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-02-08 07:47:25.000000 universal-silabs-flasher-0.0.9/universal_silabs_flasher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-02-08 07:47:25.000000 universal-silabs-flasher-0.0.9/universal_silabs_flasher/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-02-08 07:47:25.000000 universal-silabs-flasher-0.0.9/universal_silabs_flasher/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11697 2023-02-08 07:47:25.000000 universal-silabs-flasher-0.0.9/universal_silabs_flasher/cpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11483 2023-02-08 07:47:25.000000 universal-silabs-flasher-0.0.9/universal_silabs_flasher/cpc_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-02-08 07:47:25.000000 universal-silabs-flasher-0.0.9/universal_silabs_flasher/emberznet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-02-08 07:47:25.000000 universal-silabs-flasher-0.0.9/universal_silabs_flasher/flash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9516 2023-02-08 07:47:25.000000 universal-silabs-flasher-0.0.9/universal_silabs_flasher/flasher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-02-08 07:47:25.000000 universal-silabs-flasher-0.0.9/universal_silabs_flasher/gbl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-02-08 07:47:25.000000 universal-silabs-flasher-0.0.9/universal_silabs_flasher/gecko_bootloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-02-08 07:47:25.000000 universal-silabs-flasher-0.0.9/universal_silabs_flasher/xmodemcrc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 07:47:31.014967 universal-silabs-flasher-0.0.9/universal_silabs_flasher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-02-08 07:47:30.000000 universal-silabs-flasher-0.0.9/universal_silabs_flasher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-02-08 07:47:30.000000 universal-silabs-flasher-0.0.9/universal_silabs_flasher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 07:47:30.000000 universal-silabs-flasher-0.0.9/universal_silabs_flasher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-02-08 07:47:30.000000 universal-silabs-flasher-0.0.9/universal_silabs_flasher.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-02-08 07:47:30.000000 universal-silabs-flasher-0.0.9/universal_silabs_flasher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-08 07:47:30.000000 universal-silabs-flasher-0.0.9/universal_silabs_flasher.egg-info/top_level.txt
```

### Comparing `universal-silabs-flasher-0.0.8/LICENSE` & `universal-silabs-flasher-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `universal-silabs-flasher-0.0.8/PKG-INFO` & `universal-silabs-flasher-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: universal-silabs-flasher
-Version: 0.0.8
+Version: 0.0.9
 Summary: Tool to flash firmware onto any Silicon Labs radio running EmberZNet, CPC multi-PAN, or just a bare Gecko Bootloader
 Home-page: https://github.com/puddly/universal-silabs-flasher/
 Author: Puddly
 Author-email: puddly3@gmail.com
 License: GPL-3.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8
```

### Comparing `universal-silabs-flasher-0.0.8/README.md` & `universal-silabs-flasher-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `universal-silabs-flasher-0.0.8/pyproject.toml` & `universal-silabs-flasher-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `universal-silabs-flasher-0.0.8/setup.cfg` & `universal-silabs-flasher-0.0.9/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 [options]
 packages = find:
 python_requires = >=3.8
 install_requires = 
 	click
 	zigpy
 	bellows>=0.34.3
-	gpiod; platform_system!="Windows"
+	gpiod; platform_system=="Linux"
 	coloredlogs
 	async_timeout
 	awesomeversion
 
 [options.entry_points]
 console_scripts = 
 	universal-silabs-flasher = universal_silabs_flasher.__main__:main
```

### Comparing `universal-silabs-flasher-0.0.8/universal_silabs_flasher/common.py` & `universal-silabs-flasher-0.0.9/universal_silabs_flasher/common.py`

 * *Files identical despite different names*

### Comparing `universal-silabs-flasher-0.0.8/universal_silabs_flasher/cpc.py` & `universal-silabs-flasher-0.0.9/universal_silabs_flasher/cpc.py`

 * *Files identical despite different names*

### Comparing `universal-silabs-flasher-0.0.8/universal_silabs_flasher/cpc_types.py` & `universal-silabs-flasher-0.0.9/universal_silabs_flasher/cpc_types.py`

 * *Files identical despite different names*

### Comparing `universal-silabs-flasher-0.0.8/universal_silabs_flasher/emberznet.py` & `universal-silabs-flasher-0.0.9/universal_silabs_flasher/emberznet.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,14 +29,15 @@
                 "CONFIG_TRUST_CENTER_ADDRESS_CACHE_SIZE": None,
                 "CONFIG_SOURCE_ROUTE_TABLE_SIZE": None,
                 "CONFIG_MULTICAST_TABLE_SIZE": None,
                 "CONFIG_ADDRESS_TABLE_SIZE": None,
                 "CONFIG_PACKET_BUFFER_COUNT": None,
                 "CONFIG_STACK_PROFILE": None,
             },
+            config.CONF_USE_THREAD: False,
         }
     )
 
     ezsp = await bellows.ezsp.EZSP.initialize(app_config)
 
     try:
         yield ezsp
```

### Comparing `universal-silabs-flasher-0.0.8/universal_silabs_flasher/flash.py` & `universal-silabs-flasher-0.0.9/universal_silabs_flasher/flash.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import re
 import enum
 import typing
 import asyncio
 import logging
 import os.path
 import pathlib
 import functools
@@ -68,16 +69,16 @@
 
         # File
         path = pathlib.Path(value)
 
         if path.exists():
             return value
 
-        # Windows COM port
-        if value.startswith("COM") and value[3:].isdigit():
+        # Windows COM port (COM10+ uses a different syntax)
+        if re.match(r"^COM[0-9]$|\\\\\.\\COM[0-9]+$", str(path)):
             return value
 
         # Socket URI
         try:
             parsed = urllib.parse.urlparse(value)
         except ValueError:
             self.fail(f"Invalid URI: {path}", param, ctx)
@@ -179,22 +180,26 @@
         "Detected running firmware %s, version %s",
         flasher.app_type,
         flasher.app_version,
     )
 
     if flasher.app_type == ApplicationType.EZSP:
         running_image_type = FirmwareImageType.NCP_UART_HW
+    elif flasher.app_type == ApplicationType.GECKO_BOOTLOADER:
+        running_image_type = None
     else:
         # TODO: how do you distinguish RCP_UART_802154 from ZIGBEE_NCP_RCP_UART_802154?
         running_image_type = FirmwareImageType.ZIGBEE_NCP_RCP_UART_802154
 
     # Ensure the firmware versions and image types are consistent
     if not force and flasher.app_version is not None and metadata is not None:
         is_cross_flashing = (
-            metadata.fw_type is not None and metadata.fw_type != running_image_type
+            metadata.fw_type is not None
+            and running_image_type is not None
+            and metadata.fw_type != running_image_type
         )
 
         if is_cross_flashing and not allow_cross_flashing:
             raise click.ClickException(
                 f"Running image type {running_image_type}"
                 f" does not match firmware image type {metadata.fw_type}"
             )
```

### Comparing `universal-silabs-flasher-0.0.8/universal_silabs_flasher/flasher.py` & `universal-silabs-flasher-0.0.9/universal_silabs_flasher/flasher.py`

 * *Files 3% similar despite different names*

```diff
@@ -119,24 +119,28 @@
 
     def _connect_cpc(self):
         return connect_protocol(self._device, self._app_baudrate, CPCProtocol)
 
     def _connect_ezsp(self):
         return connect_ezsp(self._device, self._app_baudrate)
 
-    async def probe_gecko_bootloader(self) -> ProbeResult:
+    async def probe_gecko_bootloader(self, *, run_firmware: bool = True) -> ProbeResult:
         try:
             async with self._connect_gecko_bootloader() as gecko:
                 bootloader_version = await gecko.probe()
-                await gecko.run_firmware()
+
+                if run_firmware:
+                    await gecko.run_firmware()
         except NoFirmwareError:
             _LOGGER.warning("No application can be launched")
             return ProbeResult(version=bootloader_version, continue_probing=False)
         else:
-            return ProbeResult(version=bootloader_version, continue_probing=True)
+            return ProbeResult(
+                version=bootloader_version, continue_probing=run_firmware
+            )
 
     async def probe_cpc(self) -> ProbeResult:
         async with self._connect_cpc() as cpc:
             version = await cpc.probe()
 
         return ProbeResult(version=version, continue_probing=False)
 
@@ -154,17 +158,22 @@
             await self.enter_yellow_bootloader()
 
         self._app_type = None
         self._app_version = None
 
         bootloader_version = None
 
+        # Only run firmware from the bootloader if we have other probe methods
+        run_firmware = self._probe_methods != [ApplicationType.GECKO_BOOTLOADER]
+
         for probe_method in self._probe_methods:
             func = {
-                ApplicationType.GECKO_BOOTLOADER: self.probe_gecko_bootloader,
+                ApplicationType.GECKO_BOOTLOADER: lambda: self.probe_gecko_bootloader(
+                    run_firmware=run_firmware
+                ),
                 ApplicationType.CPC: self.probe_cpc,
                 ApplicationType.EZSP: self.probe_ezsp,
             }[probe_method]
 
             _LOGGER.info("Probing %s", probe_method)
 
             try:
@@ -182,21 +191,23 @@
 
             self._app_type = probe_method
             self._app_version = result.version
             break
         else:
             if bootloader_version is None:
                 raise RuntimeError("Failed to probe running application type")
-            elif not yellow_gpio_reset:
+            elif not yellow_gpio_reset and run_firmware:
                 raise RuntimeError(
                     "Cannot reboot back into bootloader from unknown application"
                 )
 
             # We have no valid application image but can still enter the bootloader
-            await self.enter_yellow_bootloader()
+            if yellow_gpio_reset:
+                await self.enter_yellow_bootloader()
+
             self._app_type = ApplicationType.GECKO_BOOTLOADER
             self._app_version = bootloader_version
             _LOGGER.warning("Bootloader did not launch a valid application")
 
         _LOGGER.info("Detected %s, version %s", self._app_type, self._app_version)
 
     async def enter_bootloader(self) -> None:
```

### Comparing `universal-silabs-flasher-0.0.8/universal_silabs_flasher/gbl.py` & `universal-silabs-flasher-0.0.9/universal_silabs_flasher/gbl.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,14 +102,17 @@
 
 @dataclasses.dataclass(frozen=True)
 class GBLImage:
     tags: list[tuple[TagId, bytes]]
 
     @classmethod
     def from_bytes(cls, data: bytes) -> GBLImage:
+        if isinstance(data, memoryview):
+            data = data.tobytes()
+
         tags = []
 
         for tag_bytes, value in parse_silabs_gbl(data):
             tag, _ = TagId.deserialize(tag_bytes)
             tags.append((tag, value))
 
         return cls(tags=tags)
@@ -127,8 +130,8 @@
             return next(v for t, v in self.tags if t == tag_id)
         except StopIteration:
             raise KeyError(f"No tag with id {tag_id!r} exists")
 
     def get_nabucasa_metadata(self) -> NabuCasaMetadata:
         metadata = self.get_first_tag(TagId.METADATA)
 
-        return NabuCasaMetadata.from_json(json.loads(metadata.decode("utf-8")))
+        return NabuCasaMetadata.from_json(json.loads(metadata))
```

### Comparing `universal-silabs-flasher-0.0.8/universal_silabs_flasher/gecko_bootloader.py` & `universal-silabs-flasher-0.0.9/universal_silabs_flasher/gecko_bootloader.py`

 * *Files identical despite different names*

### Comparing `universal-silabs-flasher-0.0.8/universal_silabs_flasher/xmodemcrc.py` & `universal-silabs-flasher-0.0.9/universal_silabs_flasher/xmodemcrc.py`

 * *Files identical despite different names*

### Comparing `universal-silabs-flasher-0.0.8/universal_silabs_flasher.egg-info/PKG-INFO` & `universal-silabs-flasher-0.0.9/universal_silabs_flasher.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: universal-silabs-flasher
-Version: 0.0.8
+Version: 0.0.9
 Summary: Tool to flash firmware onto any Silicon Labs radio running EmberZNet, CPC multi-PAN, or just a bare Gecko Bootloader
 Home-page: https://github.com/puddly/universal-silabs-flasher/
 Author: Puddly
 Author-email: puddly3@gmail.com
 License: GPL-3.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8
```

### Comparing `universal-silabs-flasher-0.0.8/universal_silabs_flasher.egg-info/SOURCES.txt` & `universal-silabs-flasher-0.0.9/universal_silabs_flasher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

