# Comparing `tmp/pytak-5.6.1.tar.gz` & `tmp/pytak-5.7.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytak-5.6.1.tar", last modified: Sat Jan 28 07:27:52 2023, max compression
+gzip compressed data, was "pytak-5.7.0b3.tar", last modified: Thu Jun 22 04:26:37 2023, max compression
```

## Comparing `pytak-5.6.1.tar` & `pytak-5.7.0b3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 07:27:52.357394 pytak-5.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-01-28 07:27:40.000000 pytak-5.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-01-28 07:27:40.000000 pytak-5.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14757 2023-01-28 07:27:52.357394 pytak-5.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14215 2023-01-28 07:27:40.000000 pytak-5.6.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 07:27:52.353394 pytak-5.6.1/pytak/
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-01-28 07:27:40.000000 pytak-5.6.1/pytak/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 07:27:52.353394 pytak-5.6.1/pytak/asyncio_dgram/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-01-28 07:27:40.000000 pytak-5.6.1/pytak/asyncio_dgram/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-28 07:27:40.000000 pytak-5.6.1/pytak/asyncio_dgram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9784 2023-01-28 07:27:40.000000 pytak-5.6.1/pytak/asyncio_dgram/aio.py
--rw-r--r--   0 runner    (1001) docker     (123)    10168 2023-01-28 07:27:40.000000 pytak-5.6.1/pytak/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    13730 2023-01-28 07:27:40.000000 pytak-5.6.1/pytak/client_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-01-28 07:27:40.000000 pytak-5.6.1/pytak/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-01-28 07:27:40.000000 pytak-5.6.1/pytak/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-01-28 07:27:40.000000 pytak-5.6.1/pytak/crypto_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-01-28 07:27:40.000000 pytak-5.6.1/pytak/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 07:27:52.353394 pytak-5.6.1/pytak.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14757 2023-01-28 07:27:52.000000 pytak-5.6.1/pytak.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-01-28 07:27:52.000000 pytak-5.6.1/pytak.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-28 07:27:52.000000 pytak-5.6.1/pytak.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-28 07:27:52.000000 pytak-5.6.1/pytak.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-01-28 07:27:52.000000 pytak-5.6.1/pytak.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-28 07:27:52.000000 pytak-5.6.1/pytak.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-01-28 07:27:52.357394 pytak-5.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-01-28 07:27:40.000000 pytak-5.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 04:26:37.221131 pytak-5.7.0b3/
+-rw-r--r--   0 runner    (1001) docker     (122)      557 2023-06-22 04:26:28.000000 pytak-5.7.0b3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      115 2023-06-22 04:26:28.000000 pytak-5.7.0b3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2970 2023-06-22 04:26:37.221131 pytak-5.7.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1463 2023-06-22 04:26:28.000000 pytak-5.7.0b3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      210 2023-06-22 04:26:28.000000 pytak-5.7.0b3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 04:26:37.221131 pytak-5.7.0b3/pytak/
+-rw-r--r--   0 runner    (1001) docker     (122)     1820 2023-06-22 04:26:28.000000 pytak-5.7.0b3/pytak/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 04:26:37.221131 pytak-5.7.0b3/pytak/asyncio_dgram/
+-rw-r--r--   0 runner    (1001) docker     (122)     1071 2023-06-22 04:26:28.000000 pytak-5.7.0b3/pytak/asyncio_dgram/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-06-22 04:26:28.000000 pytak-5.7.0b3/pytak/asyncio_dgram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9911 2023-06-22 04:26:28.000000 pytak-5.7.0b3/pytak/asyncio_dgram/aio.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13143 2023-06-22 04:26:28.000000 pytak-5.7.0b3/pytak/classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15504 2023-06-22 04:26:28.000000 pytak-5.7.0b3/pytak/client_functions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      998 2023-06-22 04:26:28.000000 pytak-5.7.0b3/pytak/commands.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2938 2023-06-22 04:26:28.000000 pytak-5.7.0b3/pytak/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3207 2023-06-22 04:26:28.000000 pytak-5.7.0b3/pytak/crypto_functions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5263 2023-06-22 04:26:28.000000 pytak-5.7.0b3/pytak/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 04:26:37.221131 pytak-5.7.0b3/pytak.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2970 2023-06-22 04:26:37.000000 pytak-5.7.0b3/pytak.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      438 2023-06-22 04:26:37.000000 pytak-5.7.0b3/pytak.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-22 04:26:37.000000 pytak-5.7.0b3/pytak.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      136 2023-06-22 04:26:37.000000 pytak-5.7.0b3/pytak.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-06-22 04:26:37.000000 pytak-5.7.0b3/pytak.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1490 2023-06-22 04:26:37.221131 pytak-5.7.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      806 2023-06-22 04:26:28.000000 pytak-5.7.0b3/setup.py
```

### Comparing `pytak-5.6.1/LICENSE` & `pytak-5.7.0b3/LICENSE`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright 2023 Greg Albrecht <oss@undef.net>
+Copyright 2023 Sensors & Signals LLC
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
```

### Comparing `pytak-5.6.1/pytak/__init__.py` & `pytak-5.7.0b3/pytak/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #
-# Copyright 2023 Greg Albrecht <oss@undef.net>
+# Copyright 2023 Sensors & Signals LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-# Author:: Greg Albrecht W2GMD <oss@undef.net>
-#
 
 """Python Team Awareness Kit (PyTAK) Module.
 
-:author: Greg Albrecht W2GMD <oss@undef.net>
-:copyright: Copyright 2023 Greg Albrecht
-:license: Apache License, Version 2.0
-:source: <https://github.com/ampledata/pytak>
+:source: <https://github.com/snstac/pytak>
 """
 
+__version__ = "5.7.0-beta3"
+
+
 from .constants import (  # NOQA
     LOG_LEVEL,
     LOG_FORMAT,
     DEFAULT_COT_PORT,
     DEFAULT_BACKOFF,
     DEFAULT_SLEEP,
     DEFAULT_ATAK_PORT,
@@ -39,14 +37,16 @@
     DEFAULT_COT_URL,
     DEFAULT_TLS_PARAMS_OPT,
     DEFAULT_TLS_PARAMS_REQ,
     DEFAULT_HOST_ID,
     BOOLEAN_TRUTH,
     DEFAULT_MIN_ASYNC_SLEEP,
     DEFAULT_XML_DECLARATION,
+    DEFAULT_IMPORT_OTHER_CONFIGS,
+    DEFAULT_TAK_PROTO,
 )
 
 from .classes import (  # NOQA
     Worker,
     TXWorker,
     RXWorker,
     QueueWorker,
@@ -64,10 +64,10 @@
     read_pref_package,
 )
 
 from . import asyncio_dgram  # NOQA
 
 # from .crypto_functions import *
 
-__author__ = "Greg Albrecht W2GMD <oss@undef.net>"
-__copyright__ = "Copyright 2023 Greg Albrecht"
+__author__ = "Greg Albrecht <gba@snstac.com>"
+__copyright__ = "Copyright 2023 Sensors & Signals LLC"
 __license__ = "Apache License, Version 2.0"
```

### Comparing `pytak-5.6.1/pytak/asyncio_dgram/LICENSE` & `pytak-5.7.0b3/pytak/asyncio_dgram/LICENSE`

 * *Files identical despite different names*

### Comparing `pytak-5.6.1/pytak/asyncio_dgram/aio.py` & `pytak-5.7.0b3/pytak/asyncio_dgram/aio.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import sys
 import asyncio
 import pathlib
 import socket
 import warnings
 
 __all__ = ("TransportClosed", "bind", "connect", "from_socket", "DatagramClient")
 
@@ -238,15 +239,15 @@
         local_addr=addr,
         family=family,
     )
 
     return DatagramServer(transport, recvq, excq, drained)
 
 
-async def connect(addr):
+async def connect(addr, local_addr=None):
     """
     Connect a socket to a remote address for datagrams.  The socket will be
     either AF_INET, AF_INET6 or AF_UNIX depending upon the type of host
     specified.
 
     @param addr - For AF_INET or AF_INET6, a tuple with the the host and port to
                   to connect to.
@@ -266,14 +267,15 @@
     else:
         family = 0
 
     transport, protocol = await loop.create_datagram_endpoint(
         lambda: Protocol(recvq, excq, drained),
         remote_addr=addr,
         family=family,
+        local_addr=local_addr,
     )
 
     return DatagramClient(transport, recvq, excq, drained)
 
 
 async def from_socket(sock):
     """
@@ -288,15 +290,17 @@
                   DatagramServer.
     """
     loop = asyncio.get_event_loop()
     recvq = asyncio.Queue()
     excq = asyncio.Queue()
     drained = asyncio.Event()
 
-    supported_families = tuple((socket.AF_INET, socket.AF_INET6, socket.AF_UNIX))
+    supported_families = tuple((socket.AF_INET, socket.AF_INET6))
+    if not sys.platform == "win32":
+        supported_families += (socket.AF_UNIX,)
 
     if sock.family not in supported_families:
         raise TypeError(
             "socket family not one of %s"
             % (", ".join(str(f) for f in supported_families))
         )
```

### Comparing `pytak-5.6.1/pytak/classes.py` & `pytak-5.7.0b3/pytak/classes.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,46 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #
-# Copyright 2023 Greg Albrecht <oss@undef.net>
+# Copyright 2023 Sensors & Signals LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-# Author:: Greg Albrecht W2GMD <oss@undef.net>
-#
 
 """PyTAK Class Definitions."""
 
 import asyncio
+import importlib.util
+import ipaddress
 import logging
 import multiprocessing as mp
 import queue as _queue
 import random
 
 from typing import Set, Union
 
 from configparser import ConfigParser
 
 import pytak
 
-__author__ = "Greg Albrecht W2GMD <oss@undef.net>"
-__copyright__ = "Copyright 2023 Greg Albrecht"
+try:
+    import takproto
+except ImportError:
+    pass
+
+__author__ = "Greg Albrecht <gba@snstac.com>"
+__copyright__ = "Copyright 2023 Sensors & Signals LLC"
 __license__ = "Apache License, Version 2.0"
 
 
 class Worker:  # pylint: disable=too-few-public-methods
     """Meta class for all other Worker Classes."""
 
     _logger = logging.getLogger(__name__)
@@ -45,31 +50,46 @@
         _console_handler.setLevel(pytak.LOG_LEVEL)
         _console_handler.setFormatter(pytak.LOG_FORMAT)
         _logger.addHandler(_console_handler)
         _logger.propagate = False
     logging.getLogger("asyncio").setLevel(pytak.LOG_LEVEL)
 
     def __init__(
-        self,
-        queue: Union[asyncio.Queue, mp.Queue], 
-        config: ConfigParser = None
+        self, queue: Union[asyncio.Queue, mp.Queue], config: ConfigParser = None
     ) -> None:
         """Initialize a Worker instance."""
         self.queue: Union[asyncio.Queue, mp.Queue] = queue
         if config:
             self.config = config
         else:
             config_p = ConfigParser({})
             config_p.add_section("pytak")
             self.config = config_p["pytak"]
         if self.config.getboolean("DEBUG", False):
             _ = [x.setLevel(logging.DEBUG) for x in self._logger.handlers]
 
         self.min_period = pytak.DEFAULT_MIN_ASYNC_SLEEP
 
+        tak_proto_version = config.getint("TAK_PROTO", pytak.DEFAULT_TAK_PROTO)
+
+        if tak_proto_version > 0 and importlib.util.find_spec("takproto") is None:
+            self._logger.error(
+                "Failed to use takproto for parsing CoT serialized with protobuf.\n Try: pip install pytak[with_takproto]"
+            )
+
+        self.use_protobuf = tak_proto_version > 0 and importlib.util.find_spec(
+            "takproto"
+        )
+        self._parse_proto = None
+        self._xml2proto = None
+
+        if self.use_protobuf:
+            self._parse_proto = lambda cot: takproto.parse_proto(cot)
+            self._xml2proto = lambda cot: takproto.xml2proto(cot)
+
     async def fts_compat(self) -> None:
         """Apply FreeTAKServer (FTS) compatibility.
 
         If the FTS_COMPAT (or PYTAK_SLEEP) config options are set, will async sleep for
         either a given (PYTAK_SLEEP) or random (FTS_COMPAT) time.
         """
         pytak_sleep: int = self.config.get("PYTAK_SLEEP", 0)
@@ -78,16 +98,15 @@
                 pytak_sleep or (pytak.DEFAULT_SLEEP * random.random())
             )
             self._logger.debug("COMPAT: Sleeping for %ss", sleep_period)
             await asyncio.sleep(sleep_period)
 
     async def handle_data(self, data: bytes) -> None:
         """Handle data (placeholder method, please override)."""
-        del data
-        self._logger.warning("Override this method!")
+        raise NotImplementedError("Subclasses need to override this method")
 
     async def run(self, number_of_iterations=-1):
         """Run this Thread, reads Data from Queue & passes data to next Handler."""
         self._logger.info("Run: %s", self.__class__)
 
         # We're instantiating the while loop this way, and using get_nowait(),
         # to allow unit testing of at least one call of this loop.
@@ -124,34 +143,49 @@
     ) -> None:
         """Initialize a TXWorker instance."""
         super().__init__(queue, config)
         self.writer: asyncio.Protocol = writer
 
     async def handle_data(self, data: bytes) -> None:
         """Accept CoT event from CoT event queue and process for writing."""
-        self._logger.debug("TX: %s", data)
+        self._logger.debug("TX (%s): %s", self.config.name, data)
         await self.send_data(data)
 
     async def send_data(self, data: bytes) -> None:
         """Send Data using the appropriate Protocol method."""
+        if self.use_protobuf:
+            host, _ = pytak.parse_url(self.config.get("COT_URL"))
+            is_multicast: bool = False
+
+            try:
+                is_multicast = ipaddress.ip_address(host).is_multicast
+            except ValueError:
+                # It's probably not an ip address...
+                pass
+
+            if is_multicast:
+                data = self._xml2proto(data, takproto.TAKProtoVer.MESH)
+            else:
+                data = self._xml2proto(data, takproto.TAKProtoVer.STREAM)
+
         if hasattr(self.writer, "send"):
             await self.writer.send(data)
         else:
             self.writer.write(data)
             if hasattr(self.writer, "drain"):
                 await self.writer.drain()
             if hasattr(self.writer, "flush"):
                 # FIXME: This should be an asyncio.Future?:
                 self.writer.flush()
 
 
 class RXWorker(Worker):  # pylint: disable=too-few-public-methods
     """Async receive (input) queue worker.
-    
-    Reads events from a `pytak.protocol_factory()` reader and adds them to 
+
+    Reads events from a `pytak.protocol_factory()` reader and adds them to
     an `rx_queue`.
 
     Most implementations use this to drain an RX buffer on a socket.
 
     pytak([asyncio.Protocol]->[pytak.EventReceiver]->[queue.Queue])
     """
 
@@ -160,29 +194,38 @@
     ) -> None:
         """Initialize a RXWorker instance."""
         super().__init__(queue, config)
         self.reader: asyncio.Protocol = reader
         self.reader_queue: asyncio.Queue = asyncio.Queue
 
     async def readcot(self):
-        if hasattr(self.reader, 'readuntil'):
-            return await self.reader.readuntil("</event>".encode("UTF-8"))
-        elif hasattr(self.reader, 'recv'):
-            buf, _ = await self.reader.recv()
-            return buf
+        try:
+            if hasattr(self.reader, "readuntil"):
+                cot = await self.reader.readuntil("</event>".encode("UTF-8"))
+            elif hasattr(self.reader, "recv"):
+                cot, src = await self.reader.recv()
+
+            if self.use_protobuf and self._parse_proto:
+                tak_v1 = self._parse_proto(cot)
+                if tak_v1 != -1:
+                    cot = tak_v1  # .SerializeToString()
+            return cot
+        except asyncio.exceptions.IncompleteReadError:
+            return None
 
     async def run(self, number_of_iterations=-1) -> None:
         self._logger.info("Run: %s", self.__class__)
 
         while 1:
             await asyncio.sleep(self.min_period)
             if self.reader:
                 data: bytes = await self.readcot()
-                self._logger.debug("RX: %s", data)
-                self.queue.put_nowait(data)
+                if data:
+                    self._logger.debug("RX: %s", data)
+                    self.queue.put_nowait(data)
 
 
 class QueueWorker(Worker):  # pylint: disable=too-few-public-methods
     """Read non-CoT Messages from an async network client.
 
     (`asyncio.Protocol` or similar async network client)
     Serializes it as COT, and puts it onto an `asyncio.Queue`.
@@ -195,18 +238,21 @@
     pytak([asyncio.Protocol]->[pytak.MessageWorker]->[asyncio.Queue])
     """
 
     def __init__(self, queue: asyncio.Queue, config: dict) -> None:
         super().__init__(queue, config)
         self._logger.info("CoT_URL Dest: %s", self.config.get("COT_URL"))
 
-    async def put_queue(self, data: bytes) -> None:
+    async def put_queue(self, data: bytes, queue_arg: asyncio.Queue = None) -> None:
         """Put Data onto the Queue."""
         try:
-            await self.queue.put(data)
+            if queue_arg == None:
+                await self.queue.put(data)
+            else:
+                await queue_arg.put(data)
         except asyncio.QueueFull:
             self._logger.warning("Lost Data (queue full): '%s'", data)
 
 
 class CLITool:
     """Wrapper Object for CLITools."""
 
@@ -225,23 +271,56 @@
         config: ConfigParser,
         tx_queue: Union[asyncio.Queue, mp.Queue, None] = None,
         rx_queue: Union[asyncio.Queue, mp.Queue, None] = None,
     ) -> None:
         """Initialize CLITool instance."""
         self.tasks: Set = set()
         self.running_tasks: Set = set()
-
-        self.config = config
+        self._config = config
+        self.queues = {}
         self.tx_queue: Union[asyncio.Queue, mp.Queue] = tx_queue or asyncio.Queue()
         self.rx_queue: Union[asyncio.Queue, mp.Queue] = rx_queue or asyncio.Queue()
 
-        if self.config.getboolean("DEBUG", False):
+        if self._config.getboolean("DEBUG", False):
             for handler in self._logger.handlers:
                 handler.setLevel(logging.DEBUG)
 
+    @property
+    def config(self):
+        return self._config
+
+    @config.setter
+    def config(self, v):
+        self._config = v
+
+    async def create_workers(self, i_config):
+        """Creates and runs queue workers with specified config parameter.
+
+        Parameters
+        ----------
+        i_config : `configparser.SectionProxy`
+            Configuration options & values.
+        """
+        try:
+            reader, writer = await pytak.protocol_factory(i_config)
+            tx_queue = asyncio.Queue()
+            rx_queue = asyncio.Queue()
+            if len(self.queues) == 0:
+                # If the queue list is empty, make this the default.
+                self.tx_queue = tx_queue
+                self.rx_queue = rx_queue
+            write_worker = pytak.TXWorker(tx_queue, i_config, writer)
+            read_worker = pytak.RXWorker(rx_queue, i_config, reader)
+            self.queues[i_config.name] = {"tx_queue": tx_queue, "rx_queue": rx_queue}
+            self.add_task(write_worker)
+            self.add_task(read_worker)
+        except Exception as exc:
+            self._logger.warn(f"Unable to create workers from {i_config.name}")
+            self._logger.exception(exc)
+
     async def setup(self) -> None:
         """Set up CLITool.
 
         Creates protocols, queue workers and adds them to our task list.
         """
         # Create our TX & RX Protocol Worker
         reader, writer = await pytak.protocol_factory(self.config)
@@ -272,14 +351,15 @@
         self.running_tasks.add(asyncio.ensure_future(task.run()))
 
     def run_tasks(self, tasks=None):
         """Run the given list or set of couroutine tasks."""
         tasks = tasks or self.tasks
         for task in tasks:
             self.run_task(task)
+        self.tasks.clear()
 
     async def run(self):
         """Run this Thread and its associated coroutine tasks."""
         self._logger.info("Run: %s", self.__class__)
 
         await self.hello_event()
         self.run_tasks()
```

### Comparing `pytak-5.6.1/pytak/client_functions.py` & `pytak-5.7.0b3/pytak/client_functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #
-# Copyright 2023 Greg Albrecht <oss@undef.net>
+# Copyright 2023 Sensors & Signals LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-# Author:: Greg Albrecht W2GMD <oss@undef.net>
-#
 
 """PyTAK Client & CLI Functions."""
 
 import argparse
 import asyncio
 import importlib
 import ipaddress
@@ -39,71 +37,88 @@
 import pytak
 
 from pytak.functions import unzip_file, find_file, load_preferences, cs2url
 
 from pytak.asyncio_dgram import (
     DatagramClient,
     connect as dgconnect,
-    bind as dgbind
+    bind as dgbind,
+    from_socket,
 )
 
+from pytak.crypto_functions import convert_cert
+
 # Python 3.6 support:
 if sys.version_info[:2] >= (3, 7):
     from asyncio import get_running_loop
 else:
     warnings.warn("Using Python < 3.7, consider upgrading Python.")
     from asyncio import get_event_loop as get_running_loop
 
-__author__ = "Greg Albrecht W2GMD <oss@undef.net>"
-__copyright__ = "Copyright 2023 Greg Albrecht"
+__author__ = "Greg Albrecht <gba@snstac.com>"
+__copyright__ = "Copyright 2023 Sensors & Signals LLC"
 __license__ = "Apache License, Version 2.0"
 
 
-async def create_udp_client(url: ParseResult) -> Tuple[Union[DatagramClient, None], DatagramClient]:
+async def create_udp_client(
+    url: ParseResult, iface: str = None, local_addr=None
+) -> Tuple[Union[DatagramClient, None], DatagramClient]:
     """Create an AsyncIO UDP network client for Unicast, Broadcast & Multicast.
 
     Parameters
     ----------
     url : `ParseResult`
         A parsed fully-qualified URL parsed with `urllib.parse.urlparse()`.
         For example: udp://tak.example.com:4242
 
     Returns
     -------
     `DatagramClient`
         An AsyncIO UDP network stream client.
     """
     host, port = pytak.parse_url(url)
-    write_only: bool = "+wo" in url.scheme
-
+    is_write_only: bool = "+wo" in url.scheme
+    is_broadcast = "broadcast" in url.scheme
+    is_multicast: bool = False
     reader: Union[DatagramClient, None] = None
-    if not write_only:
-        reader = await dgbind((host, port))
-    writer: DatagramClient = await dgconnect((host, port))
-
-    if reader and "broadcast" in url.scheme:
-        wsock = writer.socket
-        wsock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
-        wsock.setsockopt(socket.SOL_SOCKET, socket.SO_BROADCAST, 1)
-        rsock = reader.socket
-        rsock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
-        rsock.setsockopt(socket.SOL_SOCKET, socket.SO_BROADCAST, 1)
 
-    is_multicast: bool = False
     try:
         is_multicast = ipaddress.ip_address(host).is_multicast
     except ValueError:
         # It's probably not an ip address...
         pass
 
-    if reader and is_multicast and not write_only:
-        rsock = reader.socket
+    rsock: Union[DatagramClient, None] = None
+    if not is_write_only:
+        rsock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
+        bindall = True if sys.platform == "win32" else False
+        rsock.bind(("" if bindall else host, port))
+        reader = await from_socket(rsock)
+    writer: DatagramClient = await dgconnect((host, port), local_addr=local_addr)
+
+    if is_broadcast:
+        writer.socket.setsockopt(socket.SOL_SOCKET, socket.SO_BROADCAST, 1)
+        # writer.socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+        if reader:
+            reader.socket.setsockopt(socket.SOL_SOCKET, socket.SO_BROADCAST, 1)
+
+    if reader and (is_broadcast or is_multicast):
+        reader.socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+        try:
+            reader.socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEPORT, 1)
+        except AttributeError:
+            pass  # Some systems don't support SO_REUSEPORT
+
+    if reader and is_multicast:
         group = socket.inet_aton(host)
         mreq = struct.pack("4sL", group, socket.INADDR_ANY)
-        rsock.setsockopt(socket.IPPROTO_IP, socket.IP_ADD_MEMBERSHIP, mreq)
+        reader.socket.setsockopt(socket.IPPROTO_IP, socket.IP_ADD_MEMBERSHIP, mreq)
+        reader.socket.setsockopt(
+            socket.IPPROTO_IP, socket.IP_MULTICAST_TTL, struct.pack("b", 1)
+        )
 
     return reader, writer
 
 
 def get_tls_config(config: SectionProxy) -> SectionProxy:
     """Get the TLS config and ensures required TLS params are set.
 
@@ -120,18 +135,18 @@
     tls_config_req: dict = dict(
         zip(
             pytak.DEFAULT_TLS_PARAMS_REQ,
             [config.get(x) for x in pytak.DEFAULT_TLS_PARAMS_REQ],
         )
     )
 
-
     if not all(tls_config_req.values()):
         raise Exception(
-            f"Not all required TLS Params specified: {pytak.DEFAULT_TLS_PARAMS_REQ}")
+            f"Not all required TLS Params specified: {pytak.DEFAULT_TLS_PARAMS_REQ}"
+        )
 
     tls_config_opt: dict = dict(
         zip(
             pytak.DEFAULT_TLS_PARAMS_OPT,
             [config.get(x) for x in pytak.DEFAULT_TLS_PARAMS_OPT],
         )
     )
@@ -157,15 +172,15 @@
     -------
     `Any`
         Return value depends on the network protocol.
     """
     reader: Any = None
     writer: Any = None
 
-    _cot_url: str = config.get("COT_URL", "")
+    _cot_url: str = config.get("COT_URL", pytak.DEFAULT_COT_URL)
 
     if "://" not in _cot_url:
         warnings.warn(f"Invalid COT_URL: '{_cot_url}'", SyntaxWarning)
         raise Exception(
             "Please specify COT_URL as a full URL, including '://', for "
             "example: tcp://tak.example.com:1234"
         )
@@ -179,14 +194,15 @@
     elif scheme in ["tls", "ssl"]:
         host, port = pytak.parse_url(cot_url)
         tls_config: SectionProxy = get_tls_config(config)
 
         client_cert = tls_config.get("PYTAK_TLS_CLIENT_CERT")
         client_key = tls_config.get("PYTAK_TLS_CLIENT_KEY")
         client_cafile = tls_config.get("PYTAK_TLS_CLIENT_CAFILE")
+        client_password = tls_config.get("PYTAK_TLS_CLIENT_PASSWORD")
 
         # Default cipher suite: ALL.
         #  Also available in FIPS: DEFAULT_FIPS_CIPHERS
         client_ciphers = tls_config.get("PYTAK_TLS_CLIENT_CIPHERS") or "ALL"
 
         # If the cert's CA isn't in our trust chain, set this:
         dont_verify = tls_config.getboolean("PYTAK_TLS_DONT_VERIFY")
@@ -200,40 +216,54 @@
         ssl_ctx = ssl.SSLContext(ssl.PROTOCOL_TLS_CLIENT)
         ssl_ctx.options |= ssl.OP_NO_TLSv1
         ssl_ctx.options |= ssl.OP_NO_TLSv1_1
         ssl_ctx.set_ciphers(client_ciphers)
         ssl_ctx.check_hostname = True
         ssl_ctx.verify_mode = ssl.VerifyMode.CERT_REQUIRED
 
+        if client_cert.endswith(".p12"):
+            cert_paths = convert_cert(client_cert, client_password)
+            client_cert = cert_paths["cert_pem_path"]
+            client_key = cert_paths["pk_pem_path"]
+
         if client_key:
             ssl_ctx.load_cert_chain(client_cert, keyfile=client_key)
         else:
             ssl_ctx.load_cert_chain(client_cert)
 
         if client_cafile:
             ssl_ctx.load_verify_locations(cafile=client_cafile)
 
         # Default to checking hostnames:
         if dont_check_hostname:
             warnings.warn(
-                "TLS CN/Hostname Check DISABLED by PYTAK_TLS_DONT_CHECK_HOSTNAME.")
+                "TLS CN/Hostname Check DISABLED by PYTAK_TLS_DONT_CHECK_HOSTNAME."
+            )
             ssl_ctx.check_hostname = False
 
         # Default to verifying cert:
         if dont_verify:
             warnings.warn(
-                "TLS Certificate Verification DISABLED by PYTAK_TLS_DONT_VERIFY.")
+                "TLS Certificate Verification DISABLED by PYTAK_TLS_DONT_VERIFY."
+            )
             ssl_ctx.verify_mode = ssl.CERT_NONE
 
         try:
             reader, writer = await asyncio.open_connection(host, port, ssl=ssl_ctx)
         except ssl.SSLCertVerificationError as exc:
-            raise Exception("Consider setting PYTAK_TLS_DONT_CHECK_HOSTNAME=1 ?") from exc
+            raise Exception(
+                "Consider setting PYTAK_TLS_DONT_CHECK_HOSTNAME=1 ?"
+            ) from exc
     elif "udp" in scheme:
-        reader, writer = await pytak.create_udp_client(cot_url)
+        iface = config.get("PYTAK_MULTICAST_IFACE")
+        local_addr = (
+            config.get("PYTAK_MULTICAST_LOCAL_ADDR"),
+            0,
+        )
+        reader, writer = await pytak.create_udp_client(cot_url, iface, local_addr)
     elif "http" in scheme:
         raise Exception("TeamConnect / Sit(x) Support comming soon.")
         # writer = await pytak.create_tc_client(cot_url)
     elif "log" in scheme:
         if cot_url.hostname:
             dest: str = cot_url.hostname.lower()
             if "stderr" in dest:
@@ -271,40 +301,49 @@
     :param event_queue: asyncio.Queue worker to get events from.
     :return: EventWorker or asyncio Protocol
     """
     reader, _ = await protocol_factory(config)
     return pytak.RXWorker(queue, config, reader)
 
 
-async def main(app_name: str, config: SectionProxy) -> None:
+async def main(app_name: str, config: SectionProxy, full_config: ConfigParser) -> None:
     """
     Abstract implementation of an async main function.
 
     Parameters
     ----------
     app_name : `str`
         Name of the app calling this function.
     config : `SectionProxy`
         A dict of configuration parameters & values.
+    full_config : `ConfigParser`
+        A full dict of configuration parameters & values.
     """
     app = importlib.__import__(app_name)
     clitool: pytak.CLITool = pytak.CLITool(config)
     create_tasks = getattr(app, "create_tasks")
-    await clitool.setup()
+    await clitool.create_workers(config)
+    if config.get("IMPORT_OTHER_CONFIGS", pytak.DEFAULT_IMPORT_OTHER_CONFIGS):
+        try:
+            for i in full_config.sections()[1:]:
+                await clitool.create_workers(full_config[i])
+        except:
+            logging.warn("No more configs to create workers for!")
+    # await clitool.setup()
     clitool.add_tasks(create_tasks(config, clitool))
     await clitool.run()
 
 
 def read_pref_package(pref_package: str) -> dict:
     """Read a pref package / data package of preferences."""
     pref_config = {
         "COT_URL": None,
         "PYTAK_TLS_CLIENT_CERT": None,
         "PYTAK_TLS_CLIENT_KEY": None,
-        "PYTAK_TLS_CLIENT_CAFILE": None
+        "PYTAK_TLS_CLIENT_CAFILE": None,
     }
 
     dp_path: str = unzip_file(pref_package)
     pref_file: str = find_file(dp_path, "*.pref")
     prefs: dict = load_preferences(pref_file, dp_path)
 
     connect_string: str = prefs.get("connect_string", "")
@@ -314,15 +353,18 @@
     cert_location: str = prefs.get("certificate_location", "")
     assert os.path.exists(cert_location)
 
     client_password: str = prefs.get("client_password", "")
     assert client_password
 
     import pytak.crypto_functions
-    pem_certs: dict = pytak.crypto_functions.convert_cert(cert_location, client_password)
+
+    pem_certs: dict = pytak.crypto_functions.convert_cert(
+        cert_location, client_password
+    )
     pref_config["PYTAK_TLS_CLIENT_CERT"] = pem_certs.get("cert_pem_path")
     pref_config["PYTAK_TLS_CLIENT_KEY"] = pem_certs.get("pk_pem_path")
     pref_config["PYTAK_TLS_CLIENT_CAFILE"] = pem_certs.get("ca_pem_path")
 
     assert all(pref_config)
     return pref_config
 
@@ -357,50 +399,51 @@
     namespace = parser.parse_args()
     cli_args = {k: v for k, v in vars(namespace).items() if v is not None}
 
     # Read config:
     env_vars = os.environ
 
     # Remove env vars that contain '%', which ConfigParser or pprint barf on:
-    env_vars = {key: val for key,
-                val in env_vars.items() if "%" not in val}
+    env_vars = {key: val for key, val in env_vars.items() if "%" not in val}
 
     env_vars["COT_URL"] = env_vars.get("COT_URL", pytak.DEFAULT_COT_URL)
     env_vars["COT_HOST_ID"] = f"{app_name}@{platform.node()}"
     env_vars["COT_STALE"] = getattr(app, "DEFAULT_COT_STALE", pytak.DEFAULT_COT_STALE)
+    env_vars["TAK_PROTO"] = env_vars.get("TAK_PROTO", pytak.DEFAULT_TAK_PROTO)
 
     orig_config: ConfigParser = ConfigParser(env_vars)
 
     config_file = cli_args.get("CONFIG_FILE", "")
     if os.path.exists(config_file):
         logging.info("Reading configuration from %s", config_file)
         orig_config.read(config_file)
     else:
         orig_config.add_section(app_name)
 
     config: SectionProxy = orig_config[app_name]
+    full_config: ConfigParser = orig_config
 
     pref_package: str = config.get("PREF_PACKAGE", cli_args.get("PREF_PACKAGE"))
     if pref_package and os.path.exists(pref_package):
         pref_config = read_pref_package(pref_package)
         config.update(pref_config)
 
     debug = config.getboolean("DEBUG")
     if debug:
         print(f"Showing Config: {config_file}")
         print("=" * 10)
         pprint.pprint(dict(config))
         print("=" * 10)
 
     if sys.version_info[:2] >= (3, 7):
-        asyncio.run(main(app_name, config), debug=debug)
+        asyncio.run(main(app_name, config, full_config), debug=debug)
     else:
         loop = get_running_loop()
         try:
-            loop.run_until_complete(main(app_name, config))
+            loop.run_until_complete(main(app_name, config, full_config))
         finally:
             loop.close()
 
 
 # TeamConnect / Sit(x) Support TK:
 #
 # def tc_get_auth(
```

### Comparing `pytak-5.6.1/pytak/commands.py` & `pytak-5.7.0b3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,25 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #
-# Copyright 2023 Greg Albrecht <oss@undef.net>
+# Copyright 2023 Sensors & Signals LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-# Author:: Greg Albrecht W2GMD <oss@undef.net>
-#
-
-"""PyTAK Command Line."""
-
-import pytak
-
-__author__ = "Greg Albrecht W2GMD <oss@undef.net>"
-__copyright__ = "Copyright 2023 Greg Albrecht"
-__license__ = "Apache License, Version 2.0"
 
+"""Setup for the Python Team Awareness Kit (PyTAK) Module.
 
-def main() -> None:
-    """Boilerplate main function."""
-    # PyTAK CLI tool boilerplate:
-    pytak.cli(__name__.split(".", maxsplit=1)[0])
+:source: <https://github.com/snstac/pytak>
+"""
 
+from setuptools import setup
 
 if __name__ == "__main__":
-    main()
+    setup()
```

### Comparing `pytak-5.6.1/pytak/constants.py` & `pytak-5.7.0b3/pytak/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #
-# Copyright 2023 Greg Albrecht <oss@undef.net>
+# Copyright 2023 Sensors & Signals LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-# Author:: Greg Albrecht W2GMD <oss@undef.net>
-#
 
 """PyTAK Constants."""
 
 import logging
 import os
 import platform
 
 
-__author__ = "Greg Albrecht W2GMD <oss@undef.net>"
-__copyright__ = "Copyright 2023 Greg Albrecht"
+__author__ = "Greg Albrecht <gba@snstac.com>"
+__copyright__ = "Copyright 2023 Sensors & Signals LLC"
 __license__ = "Apache License, Version 2.0"
 
 
 LOG_LEVEL: int = logging.INFO
 LOG_FORMAT: logging.Formatter = logging.Formatter(
     ("%(asctime)s pytak %(levelname)s - %(message)s")
 )
@@ -39,21 +37,21 @@
         (
             "%(asctime)s pytak %(levelname)s %(name)s.%(funcName)s:%(lineno)d - "
             "%(message)s"
         )
     )
     logging.debug("pytak Debugging Enabled via DEBUG Environment Variable.")
 
-DEFAULT_COT_URL: str = "udp://239.2.3.1:6969"  # ATAK Default multicast
+DEFAULT_COT_URL: str = "udp+wo://239.2.3.1:6969"  # ATAK Default multicast
 DEFAULT_COT_STALE: str = "120"  # Config wants all values as strings, we'll cast later.
 DEFAULT_HOST_ID: str = f"pytak@{platform.node()}"
-
 DEFAULT_COT_PORT: int = 8087
 DEFAULT_ATAK_PORT: int = 4242
 DEFAULT_BROADCAST_PORT: int = 6969
+DEFAULT_TAK_PROTO: int = 1
 
 DEFAULT_BACKOFF: int = 120
 DEFAULT_SLEEP: int = 5
 DEFAULT_FIPS_CIPHERS: str = (
     "ECDHE-ECDSA-AES256-GCM-SHA384:ECDHE-ECDSA-AES256-GCM-SHA384"
 )
 ISO_8601_UTC = "%Y-%m-%dT%H:%M:%S.%fZ"
@@ -67,21 +65,27 @@
 
 DEFAULT_TLS_PARAMS_OPT: list = [
     "PYTAK_TLS_CLIENT_KEY",
     "PYTAK_TLS_CLIENT_CAFILE",
     "PYTAK_TLS_CLIENT_CIPHERS",
     "PYTAK_TLS_DONT_CHECK_HOSTNAME",
     "PYTAK_TLS_DONT_VERIFY",
+    "PYTAK_TLS_CLIENT_PASSWORD",  # used for encrypted PEM such as P12
 ]
 
+DEFAULT_IMPORT_OTHER_CONFIGS: bool = False
+
 BOOLEAN_TRUTH: list = ["true", "yes", "y", "on", "1"]
 DEFAULT_COT_VAL: str = "9999999.0"
 
 # await asyncio.sleep(0) should allow co-routines to yield, but they end up
 # eating 100% CPU. @PeterQFR found bumping this to 0.1 solved the high CPU
-# issue. See: https://github.com/ampledata/pytak/pull/22
+# issue. See: https://github.com/snstac/pytak/pull/22
 DEFAULT_MIN_ASYNC_SLEEP: float = 0.1
 
+# TAK Protocol to use for CoT output, one of: 0 (XML, default), 2 (Mesh), 2 (Stream).
+DEFAULT_TAK_PROTO = 0
+
 # Python <3.8 has no way of including XML Declaration in ET.tostring():
 DEFAULT_XML_DECLARATION: bytes = (
     b'<?xml version="1.0" encoding="UTF-8" standalone="yes" ?>'
 )
```

### Comparing `pytak-5.6.1/pytak/crypto_functions.py` & `pytak-5.7.0b3/pytak/crypto_functions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #
-# Copyright 2023 Greg Albrecht <oss@undef.net>
+# Copyright 2023 Greg Albrecht <gba@snstac.com>
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-# Author:: Greg Albrecht W2GMD <oss@undef.net>
-#
 
 """PyTAK Crypto (as in cryptography) Functions."""
 
 import os
 import tempfile
 import warnings
 
@@ -38,16 +36,16 @@
     from cryptography.x509 import Certificate
 
     USE_CRYPTOGRAPHY = True
 except ImportError:
     warnings.warn(INSTALL_MSG)
 
 
-__author__ = "Greg Albrecht W2GMD <oss@undef.net>"
-__copyright__ = "Copyright 2023 Greg Albrecht"
+__author__ = "Greg Albrecht <gba@snstac.com>"
+__copyright__ = "Copyright 2023 Sensors & Signals LLC"
 __license__ = "Apache License, Version 2.0"
 
 
 def save_pem(pem: bytes, dest: Union[str, None] = None) -> str:
     """Save PEM data to dest."""
     if dest:
         with open(dest, "wb+") as dest_fd:
@@ -58,15 +56,17 @@
         with os.fdopen(pem_fd, "wb+") as pfd:
             pfd.write(pem)
 
     assert os.path.exists(pem_path)
     return pem_path
 
 
-def load_cert(cert_path: str, cert_pass: str): # -> Set[_RSAPrivateKey, Certificate, Certificate]:
+def load_cert(
+    cert_path: str, cert_pass: str
+):  # -> Set[_RSAPrivateKey, Certificate, Certificate]:
     """Load RSA Keys & Certs from a pkcs12 ().p12) file."""
     if not USE_CRYPTOGRAPHY:
         raise Exception(INSTALL_MSG)
 
     with open(cert_path, "br+") as cp_fd:
         p12_data = cp_fd.read()
 
@@ -82,29 +82,26 @@
 
     cert_paths = {
         "pk_pem_path": None,
         "cert_pem_path": None,
         "ca_pem_path": None,
     }
 
-    res = load_cert(cert_path, cert_pass)
-
-    private_key: _RSAPrivateKey = res[0]
-    cert: Certificate = res[1]
-    ca_cert: Certificate = res[2][0]
+    private_key, cert, additional_certificates = load_cert(cert_path, cert_pass)
 
     # Load privkey
     pk_pem = private_key.private_bytes(
         encoding=serialization.Encoding.PEM,
         format=serialization.PrivateFormat.PKCS8,
         encryption_algorithm=serialization.NoEncryption(),
     )
     cert_paths["pk_pem_path"] = save_pem(pk_pem)
 
     cert_pem = cert.public_bytes(encoding=serialization.Encoding.PEM)
     cert_paths["cert_pem_path"] = save_pem(cert_pem)
 
+    ca_cert: Certificate = additional_certificates[0]
     ca_pem = ca_cert.public_bytes(encoding=serialization.Encoding.PEM)
     cert_paths["ca_pem_path"] = save_pem(ca_pem)
 
     assert all(cert_paths)
     return cert_paths
```

### Comparing `pytak-5.6.1/pytak/functions.py` & `pytak-5.7.0b3/pytak/functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #
-# Copyright 2023 Greg Albrecht <oss@undef.net>
+# Copyright 2023 Sensors & Signals LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-# Author:: Greg Albrecht W2GMD <oss@undef.net>
-#
 
 """PyTAK Functions."""
 
 import datetime
 import warnings
 import xml.etree.ElementTree as ET
 import tempfile
@@ -27,16 +25,16 @@
 
 from pathlib import Path
 from typing import Tuple, Union
 from urllib.parse import ParseResult, urlparse
 
 import pytak  # pylint: disable=cyclic-import
 
-__author__ = "Greg Albrecht W2GMD <oss@undef.net>"
-__copyright__ = "Copyright 2023 Greg Albrecht"
+__author__ = "Greg Albrecht <gba@snstac.com>"
+__copyright__ = "Copyright 2023 Sensors & Signals LLC"
 __license__ = "Apache License, Version 2.0"
 
 
 def split_host(host: str, port: Union[int, None] = None) -> Tuple[str, int]:
     """Split a host:port string or host, port params into a host,port tuple."""
     if ":" in host:
         addr, _port = host.split(":")
@@ -66,15 +64,15 @@
         host, port = _url.netloc.split(":")
     else:
         if "broadcast" in _url.scheme:
             port = pytak.DEFAULT_BROADCAST_PORT
         elif "multicast" in _url.scheme:
             warnings.warn(
                 "You no longer need to specify '+multicast' in the COT_URL.",
-                DeprecationWarning
+                DeprecationWarning,
             )
             port = pytak.DEFAULT_BROADCAST_PORT
         else:
             port = pytak.DEFAULT_COT_PORT
 
     return host, int(port)
 
@@ -148,15 +146,15 @@
 
     root = ET.fromstring(pref_data)
     entries = root.findall(".//entry")
 
     prefs = {
         "connect_string": None,
         "client_password": None,
-        "certificate_location": None
+        "certificate_location": None,
     }
 
     # Determine the COT URL, client certificate and password
     for entry in entries:
         if entry.attrib["key"] == "connectString0":
             prefs["connect_string"] = entry.text
         if entry.attrib["key"] == "clientPassword":
@@ -167,9 +165,7 @@
     return prefs
 
 
 def cs2url(conn_str: str) -> str:
     """Convert a TAK-style connectString into a URL."""
     uri_parts = conn_str.split(":")
     return f"{uri_parts[2]}://{uri_parts[0]}:{uri_parts[1]}"
-
-
```

