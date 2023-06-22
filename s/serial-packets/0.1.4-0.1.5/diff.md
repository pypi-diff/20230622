# Comparing `tmp/serial_packets-0.1.4.tar.gz` & `tmp/serial_packets-0.1.5.tar.gz`

## Comparing `serial_packets-0.1.4.tar` & `serial_packets-0.1.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 serial_packets-0.1.4/src/serial_packets/__init__.py
--rw-r--r--   0        0        0     6692 2020-02-02 00:00:00.000000 serial_packets-0.1.4/src/serial_packets/_packet_decoder.py
--rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 serial_packets-0.1.4/src/serial_packets/_packet_encoder.py
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 serial_packets-0.1.4/src/serial_packets/_packets.py
--rw-r--r--   0        0        0    17831 2020-02-02 00:00:00.000000 serial_packets-0.1.4/src/serial_packets/client.py
--rw-r--r--   0        0        0     7691 2020-02-02 00:00:00.000000 serial_packets-0.1.4/src/serial_packets/packets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 serial_packets-0.1.4/src/serial_packets/py.typed
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 serial_packets-0.1.4/.gitignore
--rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 serial_packets-0.1.4/LICENSE
--rw-r--r--   0        0        0    16147 2020-02-02 00:00:00.000000 serial_packets-0.1.4/README.md
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 serial_packets-0.1.4/pyproject.toml
--rw-r--r--   0        0        0    16419 2020-02-02 00:00:00.000000 serial_packets-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 serial_packets-0.1.5/src/serial_packets/__init__.py
+-rw-r--r--   0        0        0     7105 2020-02-02 00:00:00.000000 serial_packets-0.1.5/src/serial_packets/_packet_decoder.py
+-rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 serial_packets-0.1.5/src/serial_packets/_packet_encoder.py
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 serial_packets-0.1.5/src/serial_packets/_packets.py
+-rw-r--r--   0        0        0    18184 2020-02-02 00:00:00.000000 serial_packets-0.1.5/src/serial_packets/client.py
+-rw-r--r--   0        0        0     7691 2020-02-02 00:00:00.000000 serial_packets-0.1.5/src/serial_packets/packets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 serial_packets-0.1.5/src/serial_packets/py.typed
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 serial_packets-0.1.5/.gitignore
+-rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 serial_packets-0.1.5/LICENSE
+-rw-r--r--   0        0        0    16147 2020-02-02 00:00:00.000000 serial_packets-0.1.5/README.md
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 serial_packets-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0    16419 2020-02-02 00:00:00.000000 serial_packets-0.1.5/PKG-INFO
```

### Comparing `serial_packets-0.1.4/src/serial_packets/_packet_decoder.py` & `serial_packets-0.1.5/src/serial_packets/_packet_decoder.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import logging
 import asyncio
 from PyCRC.CRCCCITT import CRCCCITT
-from typing import Optional, Callable
+from typing import Optional
 
 from ._packets import PacketType, PACKET_START_FLAG, PACKET_END_FLAG, PACKET_ESC, MIN_PACKET_LEN, MAX_PACKET_LEN
 from .packets import PacketData, MAX_DATA_LEN
 # from .packets import  PACKET_MAX_LEN
 
 logger = logging.getLogger(__name__)
 
@@ -42,117 +42,128 @@
 
     def __str__(self):
         return f"Message packet: {self.endpoint}, {self.data.size()}"
 
 
 class PacketDecoder:
 
-    def __init__(self, decoded_packet_callback: Callable[
-        [DecodedCommandPacket | DecodedResponsePacket | DecodedMessagePacket], None]):
-        assert (decoded_packet_callback is not None)
+    def __init__(self):
+        # assert (decoded_packet_callback is not None)
         self.__crc_calc = CRCCCITT("FFFF")
         self.__packet_bfr = bytearray()
         self.__in_packet = False
         self.__pending_escape = False
-        self.__decoded_packet_callback = decoded_packet_callback
+        # self.__decoded_packet_callback = decoded_packet_callback
 
     def __str__(self):
         return f"In_packet ={self.__in_packet}, pending_escape={self.__pending_escape}, len={len(self.__packet_bytes)}"
 
     def __reset_packet(self, in_packet: bool):
         self.__in_packet = in_packet
         self.__pending_escape = False
         self.__packet_bfr.clear()
 
     # async def get_next_packet(self):
     #     """Blocking asyncio fetch of next pending packet."""
     #     return await self.__packets_queue.get()
 
-    def receive(self, data: bytes):
-        for b in data:
-            self.__receive_byte(b)
-
-    def __receive_byte(self, b: int):
+    # def receive(self, data: bytes):
+    #     for b in data:
+    #         self.__receive_byte(b)
+
+    def receive_byte(
+        self, b: int
+    ) -> Optional(DecodedCommandPacket | DecodedResponsePacket
+                  | DecodedMessagePacket):
+        """ Returns a decoded packet or None."""
         # If not already in a packet, wait for next flag.
         if not self.__in_packet:
             if b == PACKET_START_FLAG:
                 # Start collecting a packet.
                 self.__reset_packet(True)
             else:
                 # Here we drop bytes until next packet start. Should not
                 # happen in normal operation.
                 logger.error(f"Dropping byte {b:02x}")
                 pass
-            return
+            return None
 
         # Here collecting packet bytes.
         assert (self.__in_packet)
 
         if b == PACKET_START_FLAG:
             # Abort current packet and start a new one.
-            logger.error(f"Dropping partial packet of size {len(self.__packet_bfr)}.")
+            logger.error(
+                f"Dropping partial packet of size {len(self.__packet_bfr)}.")
             self.__reset_packet(True)
-            return
+            return None
 
         if b == PACKET_END_FLAG:
             # Process current packet.
             if self.__pending_escape:
                 logger.error("Packet has a pending escape, dropping.")
+                decoded_packet = None
             else:
-                self.__process_packet()
+                # Returns None or a packet.
+                decoded_packet = self.__process_packet()
             self.__reset_packet(False)
-            return
+            return decoded_packet
 
         # Check for size overrun. At this point, we know that the packet will
         # have at least one more additional byte, either normal or escaped.
         if len(self.__packet_bfr) >= MAX_PACKET_LEN:
-            logger.error("Packet is too long (%d), dropping", len(self.__packet_bfr))
+            logger.error("Packet is too long (%d), dropping",
+                         len(self.__packet_bfr))
             self.__reset_packet(False)
-            return
+            return None
 
         # Handle escape byte.
         if b == PACKET_ESC:
             if self.__pending_escape:
                 logger.error("Two consecutive escape chars, dropping packet")
                 self.__reset_packet(False)
             else:
                 self.__pending_escape = True
-            return
+            return None
 
         # Handle an escaped byte.
         if self.__pending_escape:
             # Flip back for 5x to 7x.
             b1 = b ^ 0x20
             if b1 != PACKET_START_FLAG and b1 != PACKET_END_FLAG and b1 != PACKET_ESC:
-                logger.error(f"Invalid escaped byte ({b1:02x}, {b:02x}), dropping packet")
+                logger.error(
+                    f"Invalid escaped byte ({b1:02x}, {b:02x}), dropping packet"
+                )
                 self.__reset_packet(False)
             else:
                 self.__packet_bfr.append(b1)
                 self.__pending_escape = False
-            return
+            return None
 
         # Handle a normal byte
         self.__packet_bfr.append(b)
 
     def __process_packet(self):
+        """Returns a packet or None."""
         rx_bfr = self.__packet_bfr
 
         # Check for minimum length. A minimum we should
         # have a type byte and two CRC bytes.
         n = len(rx_bfr)
         if n < MIN_PACKET_LEN:
             logger.error("Packet too short (%d), dropping", n)
-            return
+            return None
 
         # Check CRC
         packet_crc = int.from_bytes(rx_bfr[-2:], byteorder='big', signed=False)
         computed_crc = self.__crc_calc.calculate(bytes(rx_bfr[:-2]))
         if computed_crc != packet_crc:
-            logger.error("Packet CRC error %04x vs %04x, dropping", packet_crc, computed_crc)
-            return
+            logger.error("Packet CRC error %04x vs %04x, dropping", packet_crc,
+                         computed_crc)
+            return None
 
         # Construct decoded packet
         type_value = rx_bfr[0]
         if type_value == PacketType.COMMAND.value:
             cmd_id = int.from_bytes(rx_bfr[1:5], byteorder='big', signed=False)
             endpoint = rx_bfr[5]
             data = PacketData().add_bytes(rx_bfr[6:-2])
@@ -163,19 +174,21 @@
             data = PacketData().add_bytes(rx_bfr[6:-2])
             decoded_packet = DecodedResponsePacket(cmd_id, status, data)
         elif type_value == PacketType.MESSAGE.value:
             endpoint = rx_bfr[1]
             data = PacketData().add_bytes(rx_bfr[2:-2])
             decoded_packet = DecodedMessagePacket(endpoint, data)
         else:
-            logger.error("Invalid packet type %02x, dropping packet", type.value)
-            return
+            logger.error("Invalid packet type %02x, dropping packet",
+                         type.value)
+            return None
 
         if data.size() > MAX_DATA_LEN:
-            logger.error("Packet data too long (type=%d, len=%d), dropping", type_value,
-                         data.size())
-            return
+            logger.error("Packet data too long (type=%d, len=%d), dropping",
+                         type_value, data.size())
+            return None
 
         # Inform the user about the new packet.
-        self.__decoded_packet_callback(decoded_packet)
+        # self.__decoded_packet_callback(decoded_packet)
+        return decoded_packet
 
         # self.__packets_queue.put_nowait(decoded_packet)
```

### Comparing `serial_packets-0.1.4/src/serial_packets/_packet_encoder.py` & `serial_packets-0.1.5/src/serial_packets/_packet_encoder.py`

 * *Files identical despite different names*

### Comparing `serial_packets-0.1.4/src/serial_packets/_packets.py` & `serial_packets-0.1.5/src/serial_packets/_packets.py`

 * *Files identical despite different names*

### Comparing `serial_packets-0.1.4/src/serial_packets/client.py` & `serial_packets-0.1.5/src/serial_packets/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,31 +44,37 @@
 class _SerialProtocol(asyncio.Protocol):
     """Callbacks for the asyncio serial client."""
 
     def __init__(self):
         self.__client: SerialPacketsClient = None
         self.__port: str = None
         self.__packet_decoder: PacketDecoder = None
+        self.__work_queue: asyncio.Queue = None
         self.__is_connected = False
 
-    def set(self, client: SerialPacketsClient, port: str, packet_decoder: PacketDecoder):
+    def set(self, client: SerialPacketsClient, port: str, packet_decoder: PacketDecoder, work_queue: asyncio.Queue):
         self.__client = client
         self.__port = port
         self.__packet_decoder = packet_decoder
+        self.__work_queue = work_queue
 
     def is_connected(self):
         return self.__is_connected
 
     def connection_made(self, transport: BaseTransport):
         self.__is_connected = True
         self.__client._post_event(
             PacketsEvent(PacketsEventType.CONNECTED, f"Connected to {self.__port}"))
 
     def data_received(self, data: bytes):
-        self.__packet_decoder.receive(data)
+        for b in data:
+          decoded_packet =  self.__packet_decoder.receive_byte(b)
+          if decoded_packet:
+            logger.debug("Queuing incoming packet of type [%s.]", type(decoded_packet).__name__)
+            self.__work_queue.put_nowait(decoded_packet)
 
     def connection_lost(self, exc):
         self.__is_connected = False
         self.__client._post_event(
             PacketsEvent(PacketsEventType.DISCONNECTED, f"Disconnected from {self.__port}"))
 
     def pause_writing(self):
@@ -127,15 +133,15 @@
         self.__baudrate = baudrate
         self.__command_async_callback = command_async_callback
         self.__message_async_callback = message_async_callback
         self.__event_async_callback = event_async_callback
         self.__transport = None
         self.__protocol = None
         self.__packet_encoder = PacketEncoder()
-        self.__packet_decoder = PacketDecoder(self.__on_decoded_packet)
+        self.__packet_decoder = PacketDecoder()
         self.__command_id_counter = 0
         # self.__interval_tracker = IntervalTracker(PRE_FLAG_TIMEOUT)
         self.__tx_cmd_contexts: Dict[int, _TxCommandContext] = {}
         # Work items types:
         # * PacketsEvent: call user's event handler.
         # * DecodedCommandPacket: handle incoming command packet.
         # * DecodedResponsePacket: handle incoming response packet.
@@ -169,22 +175,22 @@
             self.__transport, self.__protocol = await serial_asyncio.create_serial_connection(
                 asyncio.get_event_loop(), _SerialProtocol, self.__port, baudrate=self.__baudrate)
         except Exception as e:
             logger.error("%s", e)
             if logging.DEBUG >= logger.getEffectiveLevel():
                 traceback.print_exception(e)
             return False
-        self.__protocol.set(self, self.__port, self.__packet_decoder)
+        self.__protocol.set(self, self.__port, self.__packet_decoder, self.__work_queue)
         return True
 
-    def __on_decoded_packet(self, decoded_packet: DecodedCommandPacket | DecodedResponsePacket |
-                            DecodedMessagePacket):
-        """Called from the packet decoder on each receive packet"""
-        logger.debug("Queuing incoming packet of type [%s.]", type(decoded_packet).__name__)
-        self.__work_queue.put_nowait(decoded_packet)
+    # def __on_decoded_packet(self, decoded_packet: DecodedCommandPacket | DecodedResponsePacket |
+    #                         DecodedMessagePacket):
+    #     """Called from the packet decoder on each receive packet"""
+    #     logger.debug("Queuing incoming packet of type [%s.]", type(decoded_packet).__name__)
+    #     self.__work_queue.put_nowait(decoded_packet)
 
     def __create_loop_runner_task(self, task_loop, name):
         logger.debug("Creating task '%s'", name)
         task = asyncio.create_task(self.__loop_runner_task(task_loop), name=name)
         self.__background_tasks.append(task)
 
     async def __loop_runner_task(self, task_loop):
```

### Comparing `serial_packets-0.1.4/src/serial_packets/packets.py` & `serial_packets-0.1.5/src/serial_packets/packets.py`

 * *Files identical despite different names*

### Comparing `serial_packets-0.1.4/LICENSE` & `serial_packets-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `serial_packets-0.1.4/README.md` & `serial_packets-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `serial_packets-0.1.4/pyproject.toml` & `serial_packets-0.1.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "serial_packets"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="Zapta", email="zapta@zapta.com" },
 ]
 description = "A Python impelementation of the Serial Packets protocol"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `serial_packets-0.1.4/PKG-INFO` & `serial_packets-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serial_packets
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python impelementation of the Serial Packets protocol
 Project-URL: Homepage, https://github.com/zapta/serial_packets_py
 Project-URL: Bug Tracker, https://github.com/zapta/serial_packets_py/issues
 Author-email: Zapta <zapta@zapta.com>
 License-File: LICENSE
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Operating System :: OS Independent
```

