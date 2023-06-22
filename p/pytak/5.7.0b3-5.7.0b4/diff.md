# Comparing `tmp/pytak-5.7.0b3.tar.gz` & `tmp/pytak-5.7.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytak-5.7.0b3.tar", last modified: Thu Jun 22 04:26:37 2023, max compression
+gzip compressed data, was "pytak-5.7.0b4.tar", last modified: Thu Jun 22 05:06:18 2023, max compression
```

## Comparing `pytak-5.7.0b3.tar` & `pytak-5.7.0b4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 04:26:37.221131 pytak-5.7.0b3/
--rw-r--r--   0 runner    (1001) docker     (122)      557 2023-06-22 04:26:28.000000 pytak-5.7.0b3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      115 2023-06-22 04:26:28.000000 pytak-5.7.0b3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2970 2023-06-22 04:26:37.221131 pytak-5.7.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1463 2023-06-22 04:26:28.000000 pytak-5.7.0b3/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      210 2023-06-22 04:26:28.000000 pytak-5.7.0b3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 04:26:37.221131 pytak-5.7.0b3/pytak/
--rw-r--r--   0 runner    (1001) docker     (122)     1820 2023-06-22 04:26:28.000000 pytak-5.7.0b3/pytak/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 04:26:37.221131 pytak-5.7.0b3/pytak/asyncio_dgram/
--rw-r--r--   0 runner    (1001) docker     (122)     1071 2023-06-22 04:26:28.000000 pytak-5.7.0b3/pytak/asyncio_dgram/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-06-22 04:26:28.000000 pytak-5.7.0b3/pytak/asyncio_dgram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9911 2023-06-22 04:26:28.000000 pytak-5.7.0b3/pytak/asyncio_dgram/aio.py
--rw-r--r--   0 runner    (1001) docker     (122)    13143 2023-06-22 04:26:28.000000 pytak-5.7.0b3/pytak/classes.py
--rw-r--r--   0 runner    (1001) docker     (122)    15504 2023-06-22 04:26:28.000000 pytak-5.7.0b3/pytak/client_functions.py
--rw-r--r--   0 runner    (1001) docker     (122)      998 2023-06-22 04:26:28.000000 pytak-5.7.0b3/pytak/commands.py
--rw-r--r--   0 runner    (1001) docker     (122)     2938 2023-06-22 04:26:28.000000 pytak-5.7.0b3/pytak/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     3207 2023-06-22 04:26:28.000000 pytak-5.7.0b3/pytak/crypto_functions.py
--rw-r--r--   0 runner    (1001) docker     (122)     5263 2023-06-22 04:26:28.000000 pytak-5.7.0b3/pytak/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 04:26:37.221131 pytak-5.7.0b3/pytak.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2970 2023-06-22 04:26:37.000000 pytak-5.7.0b3/pytak.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      438 2023-06-22 04:26:37.000000 pytak-5.7.0b3/pytak.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-22 04:26:37.000000 pytak-5.7.0b3/pytak.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      136 2023-06-22 04:26:37.000000 pytak-5.7.0b3/pytak.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-06-22 04:26:37.000000 pytak-5.7.0b3/pytak.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1490 2023-06-22 04:26:37.221131 pytak-5.7.0b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      806 2023-06-22 04:26:28.000000 pytak-5.7.0b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 05:06:18.041940 pytak-5.7.0b4/
+-rw-r--r--   0 runner    (1001) docker     (122)      557 2023-06-22 05:06:05.000000 pytak-5.7.0b4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      115 2023-06-22 05:06:05.000000 pytak-5.7.0b4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2970 2023-06-22 05:06:18.045940 pytak-5.7.0b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1463 2023-06-22 05:06:05.000000 pytak-5.7.0b4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      210 2023-06-22 05:06:05.000000 pytak-5.7.0b4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 05:06:18.041940 pytak-5.7.0b4/pytak/
+-rw-r--r--   0 runner    (1001) docker     (122)     1820 2023-06-22 05:06:05.000000 pytak-5.7.0b4/pytak/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 05:06:18.041940 pytak-5.7.0b4/pytak/asyncio_dgram/
+-rw-r--r--   0 runner    (1001) docker     (122)     1071 2023-06-22 05:06:05.000000 pytak-5.7.0b4/pytak/asyncio_dgram/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-06-22 05:06:05.000000 pytak-5.7.0b4/pytak/asyncio_dgram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9911 2023-06-22 05:06:05.000000 pytak-5.7.0b4/pytak/asyncio_dgram/aio.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13463 2023-06-22 05:06:05.000000 pytak-5.7.0b4/pytak/classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15504 2023-06-22 05:06:05.000000 pytak-5.7.0b4/pytak/client_functions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      998 2023-06-22 05:06:05.000000 pytak-5.7.0b4/pytak/commands.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2938 2023-06-22 05:06:05.000000 pytak-5.7.0b4/pytak/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3207 2023-06-22 05:06:05.000000 pytak-5.7.0b4/pytak/crypto_functions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5263 2023-06-22 05:06:05.000000 pytak-5.7.0b4/pytak/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 05:06:18.041940 pytak-5.7.0b4/pytak.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2970 2023-06-22 05:06:17.000000 pytak-5.7.0b4/pytak.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      438 2023-06-22 05:06:18.000000 pytak-5.7.0b4/pytak.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-22 05:06:17.000000 pytak-5.7.0b4/pytak.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      136 2023-06-22 05:06:17.000000 pytak-5.7.0b4/pytak.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-06-22 05:06:17.000000 pytak-5.7.0b4/pytak.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1490 2023-06-22 05:06:18.045940 pytak-5.7.0b4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      806 2023-06-22 05:06:05.000000 pytak-5.7.0b4/setup.py
```

### Comparing `pytak-5.7.0b3/LICENSE` & `pytak-5.7.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytak-5.7.0b3/PKG-INFO` & `pytak-5.7.0b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytak
-Version: 5.7.0b3
+Version: 5.7.0b4
 Summary: PyTAK: Python Team Awareness Kit Module
 Home-page: https://github.com/snstac/pytak
 Author-email: Greg Albrecht <oss@undef.net>
 Maintainer: Greg Albrecht <oss@undef.net>
 Maintainer-email: oss@undef.net
 License: Apache 2.0
 Project-URL: CI: GitHub Actions, https://github.com/snstac/pytak/actions
```

### Comparing `pytak-5.7.0b3/README.rst` & `pytak-5.7.0b4/README.rst`

 * *Files identical despite different names*

### Comparing `pytak-5.7.0b3/pytak/__init__.py` & `pytak-5.7.0b4/pytak/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 #
 
 """Python Team Awareness Kit (PyTAK) Module.
 
 :source: <https://github.com/snstac/pytak>
 """
 
-__version__ = "5.7.0-beta3"
+__version__ = "5.7.0-beta4"
 
 
 from .constants import (  # NOQA
     LOG_LEVEL,
     LOG_FORMAT,
     DEFAULT_COT_PORT,
     DEFAULT_BACKOFF,
```

### Comparing `pytak-5.7.0b3/pytak/asyncio_dgram/LICENSE` & `pytak-5.7.0b4/pytak/asyncio_dgram/LICENSE`

 * *Files identical despite different names*

### Comparing `pytak-5.7.0b3/pytak/asyncio_dgram/aio.py` & `pytak-5.7.0b4/pytak/asyncio_dgram/aio.py`

 * *Files identical despite different names*

### Comparing `pytak-5.7.0b3/pytak/classes.py` & `pytak-5.7.0b4/pytak/classes.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 import importlib.util
 import ipaddress
 import logging
 import multiprocessing as mp
 import queue as _queue
 import random
 
-from typing import Set, Union
+from typing import Optional, Set, Union
 
-from configparser import ConfigParser
+from configparser import ConfigParser, SectionProxy
 
 import pytak
 
 try:
     import takproto
 except ImportError:
     pass
@@ -50,54 +50,53 @@
         _console_handler.setLevel(pytak.LOG_LEVEL)
         _console_handler.setFormatter(pytak.LOG_FORMAT)
         _logger.addHandler(_console_handler)
         _logger.propagate = False
     logging.getLogger("asyncio").setLevel(pytak.LOG_LEVEL)
 
     def __init__(
-        self, queue: Union[asyncio.Queue, mp.Queue], config: ConfigParser = None
+        self,
+        queue: Union[asyncio.Queue, mp.Queue],
+        config: Union[None, SectionProxy, dict] = None,
     ) -> None:
         """Initialize a Worker instance."""
         self.queue: Union[asyncio.Queue, mp.Queue] = queue
         if config:
             self.config = config
         else:
             config_p = ConfigParser({})
             config_p.add_section("pytak")
-            self.config = config_p["pytak"]
-        if self.config.getboolean("DEBUG", False):
-            _ = [x.setLevel(logging.DEBUG) for x in self._logger.handlers]
+            self.config = config_p["pytak"] or {}
+
+        if bool(self.config.get("DEBUG")):
+            for handler in self._logger.handlers:
+                handler.setLevel(logging.DEBUG)
 
         self.min_period = pytak.DEFAULT_MIN_ASYNC_SLEEP
 
-        tak_proto_version = config.getint("TAK_PROTO", pytak.DEFAULT_TAK_PROTO)
+        tak_proto_version = int(self.config.get("TAK_PROTO") or pytak.DEFAULT_TAK_PROTO)
 
         if tak_proto_version > 0 and importlib.util.find_spec("takproto") is None:
             self._logger.error(
-                "Failed to use takproto for parsing CoT serialized with protobuf.\n Try: pip install pytak[with_takproto]"
+                "Failed to use takproto for parsing CoT serialized with protobuf.\n"
+                "Try: pip install pytak[with_takproto]"
             )
 
         self.use_protobuf = tak_proto_version > 0 and importlib.util.find_spec(
             "takproto"
         )
-        self._parse_proto = None
-        self._xml2proto = None
-
-        if self.use_protobuf:
-            self._parse_proto = lambda cot: takproto.parse_proto(cot)
-            self._xml2proto = lambda cot: takproto.xml2proto(cot)
 
     async def fts_compat(self) -> None:
         """Apply FreeTAKServer (FTS) compatibility.
 
         If the FTS_COMPAT (or PYTAK_SLEEP) config options are set, will async sleep for
         either a given (PYTAK_SLEEP) or random (FTS_COMPAT) time.
         """
-        pytak_sleep: int = self.config.get("PYTAK_SLEEP", 0)
-        if self.config.getboolean("FTS_COMPAT") or pytak_sleep:
+        pytak_sleep: int = int(self.config.get("PYTAK_SLEEP") or 0)
+        if bool(self.config.get("FTS_COMPAT") or pytak_sleep):
             sleep_period: int = int(
                 pytak_sleep or (pytak.DEFAULT_SLEEP * random.random())
             )
             self._logger.debug("COMPAT: Sleeping for %ss", sleep_period)
             await asyncio.sleep(sleep_period)
 
     async def handle_data(self, data: bytes) -> None:
@@ -135,46 +134,52 @@
     You should create an TXWorker Instance using the `pytak.txworker_factory()`
     Function.
 
     Data is put onto the Queue using a `pytak.QueueWorker()` instance.
     """
 
     def __init__(
-        self, queue: asyncio.Queue, config: ConfigParser, writer: asyncio.Protocol
+        self,
+        queue: Union[asyncio.Queue, mp.Queue],
+        config: Union[None, SectionProxy, dict],
+        writer: asyncio.Protocol,
     ) -> None:
         """Initialize a TXWorker instance."""
         super().__init__(queue, config)
         self.writer: asyncio.Protocol = writer
 
     async def handle_data(self, data: bytes) -> None:
         """Accept CoT event from CoT event queue and process for writing."""
-        self._logger.debug("TX (%s): %s", self.config.name, data)
+        # self._logger.debug("TX (%s): %s", self.config.get('name'), data)
         await self.send_data(data)
 
     async def send_data(self, data: bytes) -> None:
         """Send Data using the appropriate Protocol method."""
         if self.use_protobuf:
-            host, _ = pytak.parse_url(self.config.get("COT_URL"))
+            host, _ = pytak.parse_url(self.config.get("COT_URL", pytak.DEFAULT_COT_URL))
             is_multicast: bool = False
 
             try:
                 is_multicast = ipaddress.ip_address(host).is_multicast
             except ValueError:
                 # It's probably not an ip address...
                 pass
 
             if is_multicast:
-                data = self._xml2proto(data, takproto.TAKProtoVer.MESH)
+                proto = takproto.TAKProtoVer.MESH
             else:
-                data = self._xml2proto(data, takproto.TAKProtoVer.STREAM)
+                proto = takproto.TAKProtoVer.STREAM
+
+            data = takproto.xml2proto(data, proto)
 
         if hasattr(self.writer, "send"):
             await self.writer.send(data)
         else:
-            self.writer.write(data)
+            if hasattr(self.writer, "write"):
+                self.writer.write(data)
             if hasattr(self.writer, "drain"):
                 await self.writer.drain()
             if hasattr(self.writer, "flush"):
                 # FIXME: This should be an asyncio.Future?:
                 self.writer.flush()
 
 
@@ -186,37 +191,42 @@
 
     Most implementations use this to drain an RX buffer on a socket.
 
     pytak([asyncio.Protocol]->[pytak.EventReceiver]->[queue.Queue])
     """
 
     def __init__(
-        self, queue: asyncio.Queue, config: dict, reader: asyncio.Protocol
+        self,
+        queue: Union[asyncio.Queue, mp.Queue],
+        config: Union[None, SectionProxy, dict],
+        reader: asyncio.Protocol,
     ) -> None:
         """Initialize a RXWorker instance."""
         super().__init__(queue, config)
         self.reader: asyncio.Protocol = reader
-        self.reader_queue: asyncio.Queue = asyncio.Queue
+        self.reader_queue = None
 
     async def readcot(self):
+        """Read CoT from the wire until we hit an event boundary."""
         try:
             if hasattr(self.reader, "readuntil"):
                 cot = await self.reader.readuntil("</event>".encode("UTF-8"))
             elif hasattr(self.reader, "recv"):
-                cot, src = await self.reader.recv()
+                cot, _ = await self.reader.recv()
 
-            if self.use_protobuf and self._parse_proto:
-                tak_v1 = self._parse_proto(cot)
+            if self.use_protobuf:
+                tak_v1 = takproto.parse_proto(cot)
                 if tak_v1 != -1:
                     cot = tak_v1  # .SerializeToString()
             return cot
         except asyncio.exceptions.IncompleteReadError:
             return None
 
     async def run(self, number_of_iterations=-1) -> None:
+        """Run this worker."""
         self._logger.info("Run: %s", self.__class__)
 
         while 1:
             await asyncio.sleep(self.min_period)
             if self.reader:
                 data: bytes = await self.readcot()
                 if data:
@@ -234,25 +244,32 @@
     putting them onto the `event_queue`.
 
     The `event_queue` is handled by the `pytak.EventWorker` Class.
 
     pytak([asyncio.Protocol]->[pytak.MessageWorker]->[asyncio.Queue])
     """
 
-    def __init__(self, queue: asyncio.Queue, config: dict) -> None:
+    def __init__(
+        self,
+        queue: Union[asyncio.Queue, mp.Queue],
+        config: Union[None, SectionProxy, dict],
+    ) -> None:
         super().__init__(queue, config)
-        self._logger.info("CoT_URL Dest: %s", self.config.get("COT_URL"))
+        self._logger.info("COT_URL: %s", self.config.get("COT_URL"))
 
-    async def put_queue(self, data: bytes, queue_arg: asyncio.Queue = None) -> None:
+    async def put_queue(
+        self, data: bytes, queue_arg: Union[asyncio.Queue, mp.Queue, None] = None
+    ) -> None:
         """Put Data onto the Queue."""
+        _queue = queue_arg or self.queue
         try:
-            if queue_arg == None:
-                await self.queue.put(data)
+            if isinstance(_queue, asyncio.Queue):
+                await _queue.put(data)
             else:
-                await queue_arg.put(data)
+                _queue.put(data)
         except asyncio.QueueFull:
             self._logger.warning("Lost Data (queue full): '%s'", data)
 
 
 class CLITool:
     """Wrapper Object for CLITools."""
 
@@ -272,29 +289,29 @@
         tx_queue: Union[asyncio.Queue, mp.Queue, None] = None,
         rx_queue: Union[asyncio.Queue, mp.Queue, None] = None,
     ) -> None:
         """Initialize CLITool instance."""
         self.tasks: Set = set()
         self.running_tasks: Set = set()
         self._config = config
-        self.queues = {}
+        self.queues: dict = {}
         self.tx_queue: Union[asyncio.Queue, mp.Queue] = tx_queue or asyncio.Queue()
         self.rx_queue: Union[asyncio.Queue, mp.Queue] = rx_queue or asyncio.Queue()
 
-        if self._config.getboolean("DEBUG", False):
+        if bool(self._config.get("DEBUG") or 0):
             for handler in self._logger.handlers:
                 handler.setLevel(logging.DEBUG)
 
     @property
     def config(self):
         return self._config
 
     @config.setter
-    def config(self, v):
-        self._config = v
+    def config(self, val):
+        self._config = val
 
     async def create_workers(self, i_config):
         """Creates and runs queue workers with specified config parameter.
 
         Parameters
         ----------
         i_config : `configparser.SectionProxy`
@@ -310,15 +327,15 @@
                 self.rx_queue = rx_queue
             write_worker = pytak.TXWorker(tx_queue, i_config, writer)
             read_worker = pytak.RXWorker(rx_queue, i_config, reader)
             self.queues[i_config.name] = {"tx_queue": tx_queue, "rx_queue": rx_queue}
             self.add_task(write_worker)
             self.add_task(read_worker)
         except Exception as exc:
-            self._logger.warn(f"Unable to create workers from {i_config.name}")
+            self._logger.warning(f"Unable to create workers from {i_config.name}")
             self._logger.exception(exc)
 
     async def setup(self) -> None:
         """Set up CLITool.
 
         Creates protocols, queue workers and adds them to our task list.
         """
```

### Comparing `pytak-5.7.0b3/pytak/client_functions.py` & `pytak-5.7.0b4/pytak/client_functions.py`

 * *Files identical despite different names*

### Comparing `pytak-5.7.0b3/pytak/commands.py` & `pytak-5.7.0b4/pytak/commands.py`

 * *Files identical despite different names*

### Comparing `pytak-5.7.0b3/pytak/constants.py` & `pytak-5.7.0b4/pytak/constants.py`

 * *Files identical despite different names*

### Comparing `pytak-5.7.0b3/pytak/crypto_functions.py` & `pytak-5.7.0b4/pytak/crypto_functions.py`

 * *Files identical despite different names*

### Comparing `pytak-5.7.0b3/pytak/functions.py` & `pytak-5.7.0b4/pytak/functions.py`

 * *Files identical despite different names*

### Comparing `pytak-5.7.0b3/pytak.egg-info/PKG-INFO` & `pytak-5.7.0b4/pytak.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytak
-Version: 5.7.0b3
+Version: 5.7.0b4
 Summary: PyTAK: Python Team Awareness Kit Module
 Home-page: https://github.com/snstac/pytak
 Author-email: Greg Albrecht <oss@undef.net>
 Maintainer: Greg Albrecht <oss@undef.net>
 Maintainer-email: oss@undef.net
 License: Apache 2.0
 Project-URL: CI: GitHub Actions, https://github.com/snstac/pytak/actions
```

### Comparing `pytak-5.7.0b3/setup.cfg` & `pytak-5.7.0b4/setup.cfg`

 * *Files identical despite different names*

### Comparing `pytak-5.7.0b3/setup.py` & `pytak-5.7.0b4/setup.py`

 * *Files identical despite different names*

