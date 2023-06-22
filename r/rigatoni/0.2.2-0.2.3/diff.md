# Comparing `tmp/rigatoni-0.2.2.tar.gz` & `tmp/rigatoni-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rigatoni-0.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "rigatoni-0.2.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `rigatoni-0.2.2.tar` & `rigatoni-0.2.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1905 2023-06-15 00:16:12.422002 rigatoni-0.2.2/README.md
--rw-r--r--   0        0        0      780 2023-06-15 00:16:12.422002 rigatoni-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      930 2023-06-15 00:16:12.426002 rigatoni-0.2.2/rigatoni/__init__.py
--rw-r--r--   0        0        0    41908 2023-06-15 00:16:12.426002 rigatoni-0.2.2/rigatoni/core.py
--rw-r--r--   0        0        0      522 2023-06-15 00:16:12.426002 rigatoni-0.2.2/rigatoni/geometry/__init__.py
--rw-r--r--   0        0        0     4452 2023-06-15 00:16:12.426002 rigatoni-0.2.2/rigatoni/geometry/byte_server.py
--rw-r--r--   0        0        0    24399 2023-06-15 00:16:12.426002 rigatoni-0.2.2/rigatoni/geometry/geometry_creation.py
--rw-r--r--   0        0        0      837 2023-06-15 00:16:12.426002 rigatoni-0.2.2/rigatoni/geometry/geometry_objects.py
--rw-r--r--   0        0        0    20787 2023-06-15 00:16:12.426002 rigatoni-0.2.2/rigatoni/noodle_objects.py
--rw-r--r--   0        0        0     2755 1970-01-01 00:00:00.000000 rigatoni-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1945 2023-06-22 21:54:00.405660 rigatoni-0.2.3/README.md
+-rw-r--r--   0        0        0      942 2023-06-22 21:54:00.405660 rigatoni-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      956 2023-06-22 21:54:00.405660 rigatoni-0.2.3/rigatoni/__init__.py
+-rw-r--r--   0        0        0    43438 2023-06-22 21:54:00.405660 rigatoni-0.2.3/rigatoni/core.py
+-rw-r--r--   0        0        0      503 2023-06-22 21:54:00.405660 rigatoni-0.2.3/rigatoni/geometry/__init__.py
+-rw-r--r--   0        0        0     4804 2023-06-22 21:54:00.405660 rigatoni-0.2.3/rigatoni/geometry/byte_server.py
+-rw-r--r--   0        0        0    31856 2023-06-22 21:54:00.405660 rigatoni-0.2.3/rigatoni/geometry/methods.py
+-rw-r--r--   0        0        0     1498 2023-06-22 21:54:00.405660 rigatoni-0.2.3/rigatoni/geometry/objects.py
+-rw-r--r--   0        0        0    29937 2023-06-22 21:54:00.405660 rigatoni-0.2.3/rigatoni/noodle_objects.py
+-rw-r--r--   0        0        0     2961 1970-01-01 00:00:00.000000 rigatoni-0.2.3/PKG-INFO
```

### Comparing `rigatoni-0.2.2/README.md` & `rigatoni-0.2.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
+
 # Rigatoni
 
 ![Build Status](https://github.com/InsightCenterNoodles/Rigatoni/workflows/CI/badge.svg)
 ![PyPI](https://img.shields.io/pypi/v/Rigatoni)
-[![Coverage badge](https://raw.githubusercontent.com/InsightCenterNoodles/Rigatoni/python-coverage-comment-action-data/badge.svg)](https://htmlpreview.github.io/?https://github.com/InsightCenterNoodles/Rigatoni/blob/python-coverage-comment-action-data/htmlcov/index.html)
-
+[![Coverage badge](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/InsightCenterNoodles/Rigatoni/python-coverage-comment-action-data/endpoint.json&color=brightgreen)](https://htmlpreview.github.io/?https://github.com/InsightCenterNoodles/Rigatoni/blob/python-coverage-comment-action-data/htmlcov/index.html)
 
 Python Server Library for NOODLES Protocol
 
 ## Description
 This server library implements the NOODLES messaging protocol and provides objects for maintaining a scene in state. 
 The server uses a websocket connection to send CBOR encoded messages. To customize its implementation, the library 
 provides convenient interface methods to assist the user in writing their own methods for the server. The user can
 also add custom delegates to add additional functionality to any of the standard components.
 
 ## Documentation
 
-For more information and documentation, check out [the documentation](https://insightcenternoodles.github.io/Rigatoni/).
+For more information, check out [the documentation](https://insightcenternoodles.github.io/Rigatoni/).
 
 ## Installation
 
 Installation is as simple as:
 
 ```bash
 pip install rigatoni
@@ -56,8 +56,8 @@
 
 with rig.Server(50000, starting_state) as server:
     # do stuff
     pass
 ```
 
 ## Hungry for more NOODLES?
-For more information and other related repositories check out [this repository](https://github.com/InsightCenterNoodles)
+For more information and other related repositories check out [this collection](https://github.com/InsightCenterNoodles)
```

### Comparing `rigatoni-0.2.2/pyproject.toml` & `rigatoni-0.2.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -28,12 +28,19 @@
     "numpy",
     "meshio"
 ]
 testing = [
     "pytest",
     "penne",
     "pandas",
-    "matplotlib"
+    "matplotlib",
+    "meshio",
+    "pymeshlab"
 ]
 
+[tool.pytest.ini_options]
+testpaths = ["tests"]
+log_cli = true
+
 [project.urls]
-Source = "https://github.com/InsightCenterNoodles/Rigatoni"
+Source = "https://github.com/InsightCenterNoodles/Rigatoni"
+Documentation = "https://insightcenternoodles.github.io/Rigatoni/"
```

### Comparing `rigatoni-0.2.2/rigatoni/__init__.py` & `rigatoni-0.2.3/rigatoni/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,26 +5,27 @@
 messages. To customize its implementation, the library provides convenient interface 
 methods to assist the user in writing their own methods for the server. The user can also 
 add custom delegates to add additionally functionality to any of the standard components.
 
 Modules:
     core.py
     geometry/
-        geometry_creation.py
-        geometry_objects.py
+        methods.py
+        objects.py
     delegates.py
     noodle_objects.py
     server.py
 """
 
 
-__version__ = "0.2.2"
+__version__ = "0.2.3"
 
 from .core import Server
 from .noodle_objects import *
+from .geometry.byte_server import ByteServer
 
 # Ensure that dependencies are installed for optional module
 try:
     import numpy
     import meshio
     optionals = True
 except ImportError:
```

### Comparing `rigatoni-0.2.2/rigatoni/core.py` & `rigatoni-0.2.3/rigatoni/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,17 @@
 
 
 class Server(object):
     """Overarching object for managing the state of a NOODLES session
 
     Handles communication and multiple client connections. The server provides several
     methods for interacting with and creating delegates. These are especially useful for
-    defining custom methods that the server will expose to clients.
+    defining custom methods that the server will expose to clients. Can be instatiated normally,
+    or it can be used as a context manager to automatically start and stop the server while running
+    in a new thread.
     
     Attributes:
         port (int):
             port server is running on
         clients (set):
             client connections
         ids (dict): 
@@ -46,14 +48,16 @@
             components that are referenced but have been requested to be deleted
         ready (threading.Event):
             event to signal when server is ready to accept connections
         shutdown_event (asyncio.Event):
             event to signal when server is shutting down
         thread (threading.Thread):
             thread server is running on if using context manager
+        byte_server (ByteServer):
+            slot to store reference to server that serves uri bytes
         json_output (str):
             path to json file to output message logs
         custom_delegates (dict):
             maps component type to delegate class
         id_map (dict):
             maps component type to ID type
         id_decoder (dict):
@@ -86,14 +90,15 @@
         self.state = {}
         self.client_state = {}
         self.references = {}
         self.delete_queue = set()
         self.ready = threading.Event()
         self.shutdown_event = asyncio.Event()
         self.thread = None
+        self.byte_server = None
         self.json_output = json_output
         if json_output:
             with open(json_output, "w") as outfile:  # Clear out old contents
                 outfile.write("JSON Log\n")
 
         # Set up id's and custom delegates
         self.custom_delegates = delegate_map if delegate_map else {}
@@ -292,15 +297,15 @@
 
     def get_delegate(self, identifier: Union[ID, str, Dict[str, ID]]):
         """Access components in state
 
         Can be called with an ID, name, or context of the delegate
 
         Args:
-            identifier (Union[ID, str, Dict[str, ID]]): identifier for component
+            identifier (ID | str| Dict[str, ID]]): identifier for component
 
         Returns:
             delegate: delegate with specified identifier
 
         Raises:
             TypeError: if identifier is not of type ID, str, or dict
             ValueError: if no component with specified identifier is found or context is invalid
@@ -313,16 +318,19 @@
             return self.get_delegate_by_context(identifier)
         else:
             raise TypeError(f"Invalid type for identifier: {type(identifier)}")
 
     def get_delegate_by_context(self, context: dict):
         """Get a component using a context object
 
-        This is especially useful in methods that are invoked in a certain context. Note contexts
-        are only used when working with entities, tables, and plots.
+        This is especially useful in methods that are invoked in a certain context.
+
+        !!! note
+
+            Contexts are only used when working with entities, tables, and plots.
 
         Args:
             context (dict): context of the form {str: ID}
 
         Returns:
             delegate: delegate from specified context
 
@@ -451,15 +459,15 @@
         try:
             self._invoke_method(message, reply_obj)
 
         except Exception as e:
             if type(e) is MethodException:
                 reply_obj.method_exception = e
             else:
-                logging.error(f"\033[91mServerside Error: {e}\033[0m")
+                logging.error(f"\033[91mServerside Error from Method: {e}\033[0m")
                 reply_obj.method_exception = MethodException(code=-32603, message="Internal Error")
 
         return self._prepare_message("reply", reply_obj)
 
     def _invoke_method(self, message: dict, reply: Reply):
         """Invoke method and build out reply object
         
@@ -468,19 +476,20 @@
         Args:
             message (dict): Invoke message in dict form
             reply (Reply): Practically empty reply object to be updated 
         """
 
         # Parse message
         try:
+            invoke_id = message["invoke_id"]
+            reply.invoke_id = invoke_id  # Process invoke id first so it can be sent in reply with exception
             method_id = MethodID(slot=message["method"][0], gen=message["method"][1])
             context = message.get("context")
-            invoke_id = message["invoke_id"]
             args: list = message["args"]
-            reply.invoke_id = invoke_id
+
         except Exception:
             raise MethodException(code=-32700, message="Parse Error")
 
         # Locate method
         try:
             method_name = self.state[method_id].name
             method = getattr(self, method_name)
@@ -562,24 +571,26 @@
     def create_component(self, comp_type: Type[T], **kwargs) -> T:
         """Officially create new component in state
         
         This method updates state, updates references, and broadcasts msg to clients.
         It also handles the acquisition of a valid ID. This is a general creator method, but
         more specific versions exist for each component type. Keyword arguments should be
         used for specifying the attributes of the component. Any deviation from the spec will
-        raise a validation exception. Note that since this method
-        handles the ID, it should not be specified as one of the keyword arguments.
+        raise a validation exception.
+
+        !!! note
+
+            Since this method handles the ID, it should not be specified as one of the keyword arguments.
         
         Args:
             comp_type (Component Type): type of component to be created
             **kwargs: the user should specify the attributes of the component using 
                 keyword arguments. Refer to the noodle objects to see which attributes
                 are required and optional. Any deviation from the spec will raise a 
-                validation exception. Note that since this method handles the ID, it 
-                should not be specified as one of the keyword arguments.
+                validation exception.
 
         Returns:
             Delegate: delegate for the newly created component
 
         Raises:
             ValueError: if the user specifies an invalid attribute for the component
         """
@@ -602,24 +613,42 @@
         # Create message and broadcast
         message = self._prepare_message("create", new_delegate)
         self.broadcast(message)
 
         # Return component or delegate instance if applicable
         return new_delegate
 
-    def delete_component(self, delegate: Union[Delegate, ID]):
+    def _get_referenced(self, delegate: Delegate) -> list:
+        """Get all components referenced by this one
+
+        Args:
+            delegate (Delegate): component to get references for
+
+        Returns:
+            list: list of all components referenced by this one
+        """
+
+        referenced = []
+        for id, referred_by in self.references.items():
+            if delegate.id in referred_by:
+                referenced.append(self.state[id])
+        return referenced
+
+    def delete_component(self, delegate: Union[Delegate, ID], recursive: bool = False):
         """Delete object in state and update clients
         
         This method excepts a delegate, or component ID, and will attempt
         to delete the component as long as it is not referenced by any other component.
         If this component is still being used by another, it will be added to a queue so that
-        it can be deleted later once that reference is no longer being used.
+        it can be deleted later once that reference is no longer being used. If recursive flag
+        is set, then all components referenced by this one will also be deleted or at least
+        queued to be deleted.
 
         Args:
-            delegate (Component, Delegate, or ID): component / delegate to be deleted
+            delegate (Component | Delegate | ID): component / delegate to be deleted
 
         Raises:
             TypeError: if the user specifies an invalid input type
         """
 
         # Handle cases so can except different input types - cast to ID
         if isinstance(delegate, Delegate):
@@ -627,14 +656,20 @@
             del_id = delegate.id
         elif isinstance(delegate, ID):
             delegate = self.state[delegate]
             del_id = delegate.id
         else:
             raise TypeError(f"Invalid type for delegate when deleting: {type(delegate)}")
 
+        # Delete all referenced components if recursive flag is set
+        if recursive:
+            referenced = self._get_referenced(delegate)
+            for ref in referenced:
+                self.delete_component(ref, recursive=recursive)
+
         # Delete if no references, or else queue it up for later
         if not self.references.get(del_id):
             self.broadcast(self._prepare_message("delete", delegate))
             del self.state[del_id]
             del self.client_state[del_id]
 
             # Free up the ID
@@ -651,15 +686,16 @@
                     self.delete_queue.remove(comp_id)
                     self.delete_component(comp_id)
 
         else:
             logging.warning(f"Couldn't delete {delegate}, referenced by {self.references[del_id]}, added to queue")
             self.delete_queue.add(del_id)
 
-    def _find_delta(self, state, edited):
+    @staticmethod
+    def _find_delta(state, edited):
         """Helper to find differences between two objects
         
         Also checks to find recursive cases and cases where references
         should be updated, Does this get recursive deltas tho? should it?
         """
 
         delta = set()
@@ -693,42 +729,54 @@
         self.client_state[current.id] = current.copy()
 
         # Form message and broadcast
         try:
             message = self._prepare_message("update", current, delta)
             self.broadcast(message)
         except Exception as e:
-            raise Exception(f"This obj can not be updated: {e}")
+            raise ValueError(f"This obj can not be updated: {e}")
 
-    def invoke_signal(self, signal: SignalID, on_component: Delegate, signal_data: list):
+    def invoke_signal(self, signal: Union[SignalID, Signal], on_component: Delegate, signal_data: list = None):
         """Send signal to target component
         
         Args:
-            signal (ID): signal to be invoked
+            signal (SignalID | Signal): signal to be invoked
             on_component (Delegate): component to receive the signal
             signal_data (dict): data to be sent with the signal
 
+        Returns:
+            message: message to be broadcast
+
         Raises:
             ValueError: if the user specifies an invalid on_component type
         """
 
+        # Cast signal to ID if needed
+        if isinstance(signal, Signal):
+            signal = signal.id
+
+        # Fill in default signal data if not specified
+        if signal_data is None:
+            signal_data = []
+
         # Get context from on_component
         if isinstance(on_component, Entity):
             context = InvokeIDType(entity=on_component.id)
         elif isinstance(on_component, Table):
             context = InvokeIDType(table=on_component.id)
         elif isinstance(on_component, Plot):
             context = InvokeIDType(plot=on_component.id)
         else:
             raise ValueError(f"Invalid on_component type: {type(on_component)}")
 
         # Create invoke object and broadcast message
         invoke = Invoke(id=signal, context=context, signal_data=signal_data)
         message = self._prepare_message("invoke", invoke)
         self.broadcast(message)
+        return message
 
     def create_method(self, name: str,
                       arg_doc: list[MethodArg],
                       doc: Optional[str] = None,
                       return_doc: Optional[str] = None) -> Method:
         """Add a Method object to the scene and return it. Will use a custom delegate if applicable.
```

### Comparing `rigatoni-0.2.2/rigatoni/geometry/byte_server.py` & `rigatoni-0.2.3/rigatoni/geometry/byte_server.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 import socket
 import re
 import threading
+import logging
 
 
 class ByteServer(object):
     """Server to Host URI Bytes.
 
     This is helpful for large meshes and images that would
     otherwise be too large to send using CBOR and the websocket connection. The server maps
     a tag to a buffer, and the client can request the buffer using the url that includes the
     tag.
+
+    !!! note
+
+        The server is start up automatically in a new thread when the class is instantiated, and
+        `shutdown` must be called to clean up this thread.
     
     Attributes:
         host (str): IP address for server
         port (int): port server is listening on
         socket (socket): socket connection 
         buffers (dict): mapping tag to buffer
         _next_tag (int): next available tag for a buffer
@@ -37,17 +43,19 @@
 
         self.port = port
         self.socket = None
         self.buffers = {}
         self._next_tag = 0
         self.url = f"http://{self.host}:{port}"
 
-        self.thread = threading.Thread(target=self.run, args=())
+        self.thread = threading.Thread(target=self._run, args=())
         self.running = True
+        self.ready = threading.Event()
         self.thread.start()
+        self.ready.wait()
 
     def _get_tag(self):
         """Helper to get next tag for a buffer"""
 
         tag = self._next_tag
         self._next_tag += 1
         return str(tag)
@@ -63,85 +71,77 @@
 
         m = re.search(f'(?<={self.port}/).+\Z', uri)
         if m:
             tag = m.group(0)
             buffer_bytes = self.buffers[tag]
             return buffer_bytes
         else:
-            raise Exception("Invalid HTTP Request")
+            raise ValueError("Invalid HTTP Request")
 
-    def run(self):
+    def _run(self):
         """Main loop to run in thread
         
         Runs the server and listens for byte requests using HTTP protocol
         """
 
         # Create socket
         server_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         server_socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
         server_socket.bind((self.host, self.port))
 
-        print(f"IP Address: {server_socket.getsockname()}")
+        logging.info(f"IP Address for Byte Server: {server_socket.getsockname()}")
 
         self.socket = server_socket
 
+        server_socket.settimeout(.5)  # timeout to check if still running
         server_socket.listen(1)
-        print(f'Listening on port {self.port} ...')
-
+        logging.info(f'Byte server listening on port {self.port}...')
+        self.ready.set()
         while self.running:
-            # Wait for client connections
-            print("Waiting for connection...")
-            client_connection, client_address = server_socket.accept()
-
-            # Get the client request
-            request = client_connection.recv(1024).decode()
-            print(f"Request: {request}")
-
-            # Try to get tag from request with regex
-            m = re.search('(?<=GET /)(.+?)(?= HTTP)', request)
-            if m:
-                tag = m.group(0)
-                select_bytes = self.buffers[tag]
-                header = f'HTTP/1.0 200 OK\r\nContent-Type: application/octet-stream\r\nContent-Length: {len(select_bytes)}\n\n'
-                response = bytearray(header.encode()) + select_bytes
-            else:
-                header = f'HTTP/1.0 500 FAIL'
-                response = header.encode()
-
-            # Send HTTP response
-            client_connection.sendall(response)
-            client_connection.close()
+            try:
+                # Wait for client connections - this is blocking
+                client_connection, client_address = server_socket.accept()
+
+                # Get the client request
+                request = client_connection.recv(1024).decode()
+                logging.info(f"Request: {request}")
+
+                # Try to get tag from request with regex
+                m = re.search('(?<=GET /)(.+?)(?= HTTP)', request)
+                try:
+                    tag = m.group(0)
+                    select_bytes = self.buffers[tag]
+                    header = f'HTTP/1.0 200 OK\r\nContent-Type: application/octet-stream\r\n' \
+                             f'Content-Length: {len(select_bytes)}\n\n'
+                    response = bytearray(header.encode()) + select_bytes
+                except Exception:
+                    header = f'HTTP/1.0 500 FAIL'
+                    response = header.encode()
+
+                # Send HTTP response
+                client_connection.sendall(response)
+                client_connection.close()
 
+            except socket.timeout:
+                pass
         # Clean up and close socket
         self.socket.close()
 
     def add_buffer(self, buffer) -> str:
         """Add buffer to server and return url to reach it
         
         Args:
             buffer (bytes): bytes to add as buffer
         """
 
         tag = self._get_tag()
         self.buffers[tag] = buffer
         url = f"{self.url}/{tag}"
-        print(f"Adding Buffer: {url}")
+        logging.info(f"Adding buffer to byte server: {url}")
 
         return url
 
     def shutdown(self):
         """Stop running thread"""
 
         self.running = False
         self.thread.join()
-
-
-def main():
-    """Main method for testing"""
-
-    server = ByteServer(port=60000)
-    server.add_buffer('HTTP/1.0 200 OK\n\nTEST TEST TEST'.encode())
-    server.add_buffer(b'TESTING BYTES')
-
-
-if __name__ == "__main__":
-    main()
```

### Comparing `rigatoni-0.2.2/rigatoni/geometry/geometry_creation.py` & `rigatoni-0.2.3/rigatoni/geometry/methods.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-"""Module for assisting with the creation of geometry objects"""
+"""Helpful methods for assisting with the creation of geometry objects"""
 from math import sqrt
 from collections import deque
 from statistics import mean
 from typing import Optional, Tuple
+import logging
+
 import numpy as np
 import meshio
 
 from .. import noodle_objects as nooobs
 from ..core import Server
 
-from .geometry_objects import AttributeInput, GeometryPatchInput
+from .objects import AttributeInput, GeometryPatchInput
 from .byte_server import ByteServer
 
 INLINE_LIMIT = 10000
 
 SIZES = {
     # in bytes
     "U8": 1,
@@ -43,61 +45,101 @@
 
 DEFAULT_POSITION = [0.0, 0.0, 0.0, 1.0]
 DEFAULT_COLOR = [1.0, 1.0, 1.0, 1.0]
 DEFAULT_ROTATION = [0.0, 0.0, 0.0, 1.0]
 DEFAULT_SCALE = [1.0, 1.0, 1.0, 1.0]
 
 
-def get_format(num_vertices: int) -> str:
+def _get_format(num_vertices: int) -> str:
     """Helper to get format that can accommodate number of vertices
     
     Args:
         num_vertices (int): number of vertices needed to store in mesh
     """
 
     if num_vertices < 256:
         return 'U8'
     elif num_vertices < 65536:
         return 'U16'
     else:
         return 'U32'
 
 
-def set_up_attributes(patch_input: GeometryPatchInput, generate_normals: bool):
-    """Constructs attribute info from input type
-    
-    Takes list input and constructs objects 
-    that can be used in build_geometry_patch
+def _convert_to_rgba(colors: list):
+    """Convert list of arbitrary colors to list of RGBA colors
+
+    Used to ensure geometry patch input colors are valid RGBA colors
+
+    Args:
+        colors (list): list of colors, each color is a list of 3 or 4 elements
+
+    Returns:
+        list: list of RGBA colors
+
+    Raises:
+        ValueError: if color does not have 3 or 4 elements
+    """
+    rgba_colors = []
+    for color in colors:
+        if len(color) == 3:
+            color = list(color) + [1.0]  # Append 1 to represent alpha channel
+        elif len(color) != 4:
+            raise ValueError("Color must have 3 or 4 elements")
+
+        # Normalize values if they are in the range 0-255
+        normalized_color = [c / 255.0 if c > 1.0 else c for c in color]
+        rgba_colors.append(normalized_color)
+
+    return rgba_colors
+
+
+def _set_up_attributes(patch_input: GeometryPatchInput, generate_normals: bool, ordered=True):
+    """Constructs attribute info from input type, not used by users
+    
+    Takes list input and constructs objects that can be used in build_geometry_patch.
+    Specifically, it returns a list of AttributeInput objects that have attributes:
+    semantic: nooobs.AttributeSemantic
+    format: nooobs.Format
+    normalized: bool
+    offset: Optional[int]
+    stride: Optional[int]
 
     Args:
         patch_input (GeometryPatchInput): stores lists of vertices, indices
             index type, material, and possibly normals, tangents,
             textures, and colors
         generate_normals (bool): calculate normals for mesh or not
+
+    Returns:
+        list: list of AttributeInput objects
     """
 
     # Generate normals if not indicated in input
     if not patch_input.normals and generate_normals:
-        patch_input.normals = calculate_normals(patch_input.vertices, patch_input.indices)
+        if len(patch_input.vertices) > 1024:
+            raise ValueError("Mesh is too large to generate normals. Either provide normals as input or set "
+                             "generate_normals to False.")
+        patch_input.normals = calculate_normals(patch_input.vertices, patch_input.indices, ordered=ordered)
 
     # Add attribute info based on the input lists
     attribute_info = []
     position = AttributeInput(
         semantic="POSITION",
         format="VEC3",
         normalized=False,
     )
     attribute_info.append(position)
 
-    normal = AttributeInput(
-        semantic="NORMAL",
-        format="VEC3",
-        normalized=False,
-    )
-    attribute_info.append(normal)
+    if patch_input.normals:
+        normal = AttributeInput(
+            semantic="NORMAL",
+            format="VEC3",
+            normalized=False,
+        )
+        attribute_info.append(normal)
 
     if patch_input.tangents:
         tangent = AttributeInput(
             semantic="TANGENT",
             format="VEC3",
             normalized=False,
         )
@@ -115,104 +157,115 @@
         color = AttributeInput(
             semantic="COLOR",
             format="U8VEC4",
             normalized=True,
         )
         attribute_info.append(color)
 
-        # Check color format and correct
-        if any(i > 1 for i in patch_input.colors[0]):
-            for i in range(len(patch_input.colors)):
-                patch_input.colors[i] = [x / 255 for x in patch_input.colors[i]]
+        # Check color format and correct, values greater than 1 are assumed to be 0-255, default alpha to 1
+        patch_input.colors = _convert_to_rgba(patch_input.colors)
 
-    # Use input to get offsets
+    # Use input to get offsets for each attribute
     offset = 0
     for attribute in attribute_info:
         attribute.offset = offset
         offset += SIZES[attribute.format]
 
     # Use final offset to get stride
     for attribute in attribute_info:
         attribute.stride = offset
 
     return attribute_info
 
 
-def build_geometry_buffer(server: Server, name, patch_input: GeometryPatchInput, index_format: str,
-                          attribute_info: list[AttributeInput],
-                          byte_server: ByteServer = None) -> Tuple[nooobs.Buffer, int]:
-    """Builds a buffer component
+def _build_geometry_buffer(server: Server, name, patch_input: GeometryPatchInput, index_format: str,
+                           attribute_info: list[AttributeInput],
+                           byte_server: ByteServer = None) -> Tuple[nooobs.Buffer, int]:
+    """Builds a buffer component from attributes and data from geometry input
+
+    Structures bytes by interleaving attributes grouped by vertex, then indices are added to the end.
 
     Args:
         server (Server): server to create component on
         name (str): name to give component
         patch_input (GeometryPatchInput): lists of attributes and point data
         index_format (str): format the indices should take
         attribute_info (list[AttributeInput]): Info on the attributes, mostly used for formatting
         byte_server (ByteServer): byte server to use if needed
     """
 
     # Filter out inputs unspecified by user, and group attributes by point
-    data = [x for x in
-            [patch_input.vertices, patch_input.normals, patch_input.tangents, patch_input.textures, patch_input.colors]
-            if x]
+    fields = [patch_input.vertices, patch_input.normals, patch_input.tangents, patch_input.textures, patch_input.colors]
+    data = [x for x in fields if x]
     points = zip(*data)
 
     # Build byte array by iterating through points and their attributes
     buffer_bytes = bytearray(0)
     for point in points:
         for info, attr in zip(point, attribute_info):
             attr_size = FORMAT_MAP[attr.format]
             new_bytes = np.array(info, dtype=attr_size).tobytes(order='C')
             buffer_bytes.extend(new_bytes)
 
     # Add index bytes to byte array
     index_offset = len(buffer_bytes)
-    index_bytes = np.array(patch_input.indices, dtype=FORMAT_MAP[index_format]).tobytes(order='C')
+    index_bytes = np.array(patch_input.indices).astype(FORMAT_MAP[index_format]).tobytes(order='C')
     buffer_bytes.extend(index_bytes)
 
     # Create buffer component using uri bytes if needed
     size = len(buffer_bytes)
     if size > INLINE_LIMIT:
-        print(f"Large Mesh: Using URI Bytes")
+        logging.info(f"Large Mesh: Using URI Bytes")
         uri = byte_server.add_buffer(buffer_bytes)
         buffer = server.create_buffer(name=name, size=size, uri_bytes=uri)
         return buffer, index_offset
     else:
         buffer = server.create_buffer(
             name=name,
             size=size,
             inline_bytes=buffer_bytes
         )
         return buffer, index_offset
 
 
 def build_geometry_patch(server: Server, name: str, patch_input: GeometryPatchInput,
-                         byte_server: ByteServer = None, generate_normals: bool = True) -> nooobs.GeometryPatch:
+                         byte_server: ByteServer = None, generate_normals: bool = True,
+                         ordered_indices: bool = True) -> nooobs.GeometryPatch:
     """Build a Geometry Patch with related buffers and views
+
+    Buffer bytes are structured by interleaving attributes grouped by vertex, then indices are added to the end.
+    Normals are generated by default if they are not provided. If indices are not oriented consistently, ordered_indices
+    should be set to False, slowing down the calculation of normals.
+
+    !!! note
+
+        If the mesh is larger than 10Kb, the buffer will attempt to use URI bytes, and an exception will be raised if
+        one is not provided.
     
     Args:
         server (Server): server to create components on
         name (str): name for the components
         patch_input (GeometryPatch): input lists with data to create the patch
         byte_server (ByteServer): optional server to use if mesh is larger than 10Kb
         generate_normals (bool): whether to calculate normals for this mesh
+        ordered_indices (bool): whether indices are ordered or not, could be clockwise or counter-clockwise, used when
+            calculating normals
     """
 
     # Set up some constants
     vert_count = len(patch_input.vertices)
     index_count = len(patch_input.indices) * len(patch_input.indices[0])
-    index_format = get_format(vert_count)
+    index_format = _get_format(vert_count)
 
     # Set up attributes with given lists
-    attribute_info = set_up_attributes(patch_input, generate_normals=generate_normals)
+    attribute_info = _set_up_attributes(patch_input, generate_normals=generate_normals, ordered=ordered_indices)
 
     # Build buffer with given lists
     buffer: nooobs.Buffer
-    buffer, index_offset = build_geometry_buffer(server, name, patch_input, index_format, attribute_info, byte_server)
+    buffer, index_offset = _build_geometry_buffer(server, name, patch_input, index_format, attribute_info, byte_server)
 
     # Make buffer view component
     buffer_view: nooobs.BufferView = server.create_component(
         nooobs.BufferView,
         name=name,
         source_buffer=buffer.id,
         type="GEOMETRY",
@@ -265,14 +318,16 @@
     )
 
     return buffer
 
 
 def build_entity(server: Server, geometry: nooobs.Geometry, instances: list[list] = None):
     """Build Entity from Geometry
+
+    Helps format buffers for instances. Can get instance matrices easily with create_instances.
     
     Args:
         server (Server): server to build entity component on
         geometry (Geometry): geometry to link entity to
         instances (Mat4): optional instance matrix, can use create_instances to generate
 
     Returns:
@@ -305,28 +360,35 @@
 
 
 def create_instances(
         positions: list[list] = None,
         colors: list[list] = None,
         rotations: list[list] = None,
         scales: list[list] = None) -> list[list]:
-    """Create new instances for an entity
+    """Create new instance matrices for an entity
     
     All lists are optional and will be filled with defaults.
     By default, one instance is created at least.
-    Lists are padded out to 4 values.
+    Lists are padded out to 4 values. Each matrix is of the form below
+
+    | position | color | rotation | scale |
+    |----------|-------|----------|-------|
+    | x        | r     | x        | x     |
+    | y        | g     | y        | y     |
+    | z        | b     | z        | z     |
+    | 1        | a     | w        | 1     |
 
     Args:
         positions (list[Vec3]): positions for each instance
         colors (list[Vec4]): Colors for each instance
         rotations (list[Vec4]): Rotations for each instance
         scales (list[Vec3]): Scales for each instance
 
     Returns:
-        list[list]: 2d array representing instance data
+        list: list of instance matrices
     """
 
     def padded(lst: list, default_val: float = 1.0):
         """Helper to pad the lists"""
 
         lst = list(lst)
         if len(lst) < 4:
@@ -364,84 +426,92 @@
     """Update an entity with new instances or geometry
     
     Args:
         server (Server): server with entity to update
         entity (Entity): Entity to be updated
         geometry (Geometry): Optional new geometry if that is being changed
         instances (list[Mat4]): Optional new instances if that is changed
+
+    Returns:
+        Entity: updated entity
+
+    Raises:
+        ValueError: If no geometry is specified and entity has no geometry
     """
 
     # Get name from entity if applicable
     name = entity.name if entity.name else None
 
-    # Get render rep and ensure entity is working with geometry
-    old_rep = entity.render_rep
-    if not old_rep:
-        raise Exception("Entity isn't renderable")
-
     # Set geometry id based on whether there is new geometry or not
+    old_rep = entity.render_rep
     if geometry:
         mesh = geometry.id
-    else:
+    elif old_rep and old_rep.mesh:
         mesh = old_rep.mesh
+    else:
+        raise ValueError("No geometry specified and entity has no geometry")
 
     # Build new buffer / view for instances or use existing instances
     if instances:
         buffer = build_instance_buffer(server, name, instances)
         buffer_view = server.create_component(
             nooobs.BufferView,
             name=f"Instance View for {name}",
             source_buffer=buffer.id,
             type="UNK",
             offset=0,
             length=buffer.size
         )
         instance = nooobs.InstanceSource(view=buffer_view.id, stride=0, bb=None)
     else:
-        instance = old_rep.instances
+        instance = old_rep.instances if old_rep else None
 
     # Create new render rep for entity and update entity
     rep = nooobs.RenderRepresentation(mesh=mesh, instances=instance)
     entity.render_rep = rep
-    entity = server.update_component(entity)
+    server.update_component(entity)
 
     # Clean up old components with deletes
-    if instances:
-        server.delete_component(server.state[old_rep.instances.view].source_buffer)
-        server.delete_component(old_rep.instances.view)
-    elif geometry:
-        server.delete_component(old_rep.mesh)
+    if instances and old_rep and old_rep.instances:
+        old_instance_buffer = server.get_delegate(old_rep.instances.view).source_buffer
+        old_instance_view = old_rep.instances.view
+        server.delete_component(old_instance_buffer)
+        server.delete_component(old_instance_view)
+    if geometry and old_rep:
+        server.delete_component(old_rep.mesh, recursive=True)
 
     return entity
 
 
 def add_instances(server: Server, entity: nooobs.Entity, instances: list):
-    """Add instances to an existing entity
+    """Adds instances or merges them into existing instances for an entity
     
     Args:
         server (Server): server with entity to update
         entity (Entity): entity to be updated
         instances (list[Mat4]): new instances to be added, can be generated using 
             create_instances()
     """
 
     # Ensure we're working with an entity that can be rendered
-    try:
-        rep = entity.render_rep
+    if not entity.render_rep:
+        raise ValueError(f"Entity {entity} has no render representation - could not add instances")
 
-        # Get old instance buffer from entity's render rep
+    # Get old instance buffer from entity's render rep
+    rep = entity.render_rep
+    if rep.instances:  # Need to combine / merge with old instances
         old_view: nooobs.BufferView = server.state[rep.instances.view]
         old_buffer: nooobs.Buffer = server.state[old_view.source_buffer]
         old_instances = np.frombuffer(old_buffer.inline_bytes, dtype=np.single)
 
         # Combine new and old instances
-        combined = np.append(old_instances, instances)
-        update_entity(server, entity, instances=combined.tolist())
-    except:
-        raise Exception("Entity isn't renderable")
+        combined = np.append(old_instances, instances).tolist()
+        instances = combined
+
+    update_entity(server, entity, instances=instances)
 
 
 # ---------------------------------- Mesh Importing ----------------------------------#
 
 def convert(color: int):
     """Helper to convert decimal pymesh values to RGBA array"""
 
@@ -452,15 +522,16 @@
 
     alpha = rgb.pop(0)
     rgb.append(alpha)
     return rgb
 
 
 def meshlab_load(server: Server, byte_server: ByteServer, file,
-                 material: nooobs.Material, mesh_name: Optional[str] = None, generate_normals: bool = True):
+                 material: nooobs.Material, mesh_name: Optional[str] = None,
+                 generate_normals: bool = True, ordered: bool = False):
     """Use pymeshlab to load types unsupported by meshio
 
     This method is only called from geometry_from_mesh if needed
     
     Args:   
         server (Server): server to load geometry onto
         byte_server (ByteServer): server to support URI bytes if needed
@@ -471,15 +542,15 @@
     """
     import pymeshlab
 
     ms = pymeshlab.MeshSet()
     ms.load_new_mesh(file)
     mesh = ms.current_mesh()
     # mesh.compute_normal_per_vertex("Simple Average")
-    print(f"Finished Loading Mesh...")
+    logging.info(f"Finished Loading Mesh...")
 
     # Extract data from mesh set structure
     vertices = mesh.vertex_matrix().tolist()
     indices = mesh.face_matrix().tolist()
     # normals = mesh.vertex_normal_matrix().tolist() # Look like they could be off
     normals = None
     tangents = None  # TBD
@@ -493,61 +564,82 @@
         indices=indices,
         index_type="TRIANGLES",
         material=material.id,
         normals=normals,
         tangents=tangents,
         textures=textures,
         colors=colors)
-    patches.append(build_geometry_patch(server, mesh_name, patch_info, byte_server, generate_normals=generate_normals))
+    patches.append(build_geometry_patch(server, mesh_name, patch_info, byte_server, generate_normals=generate_normals,
+                                        ordered_indices=ordered))
     geometry = server.create_component(nooobs.Geometry, name=mesh_name, patches=patches)
 
     return geometry
 
 
 def geometry_from_mesh(server: Server, file, material: nooobs.Material,
-                       mesh_name: Optional[str] = None, byte_server: ByteServer = None, generate_normals: bool = True):
+                       mesh_name: Optional[str] = None, byte_server: ByteServer = None,
+                       generate_normals: bool = True, ordered_indices: bool = True):
     """Construct geometry from mesh file
     
-    Can specify byte server if it is a big mesh and needs uri bytes
+    Can specify byte server if it is a big mesh and needs uri bytes. By default, uses meshio to avoid
+    importing pymeshlab if possible. If meshio fails, pymeshlab is used to load the mesh. Meshio supports
+    .inp, .msh, .avs, .cgns, .xml, .e, .exo, .f3grid, .h5m, .mdpa, .mesh, .meshb, .med, .bdf, .fem, .nas,
+    .vol, .vol.gz, .post, .post.gz, .dato, .dato.gz, .ply, .stl, .svg, .su2, .ugrid, .vtk, .vtu, .wkt, .xdmf,
+    and .xmf. If you are looking to use another format, you will have to install pymeshlab.
+
+    By default, this method will calculate normals for the mesh if they are not provided. This can be a relatively
+    intense step that will slow down an application. To turn this off, set generate_normals to False. If indices
+    are oriented consistently, set ordered_indices to True to improve performance.
+
+    !!! note
+
+        If the mesh is too large (> 1024 vertices) and calculating the normals would be too intense, this method
+        will raise an exception, and you should either provide normals or set generate_normals to False.
+
+    !!! note
+
+        If the mesh is larger than 10Kb, the buffer will attempt to use URI bytes, and an exception will be raised if
+        one is not provided.
 
     Args:
         server (Server): server to load geometry onto
         file (str, path): file to load mesh from
         material (Material): material to use in geometry
         mesh_name (str): optional name
         byte_server (ByteServer): server to support URI bytes if needed
         generate_normals (bool): whether to calculate normals for the mesh
+        ordered_indices (bool): whether indices are oriented consistently (clockwise or counterclockwise)
 
     Returns:
         Geometry: newly created geometry delegate
     """
 
     # Create meshio mesh object to extract data from file, if unsupported file type use meshlab
     try:
         mesh = meshio.read(file)
     except Exception as e:
-        return meshlab_load(server, byte_server, file, material, mesh_name, generate_normals=generate_normals)
+        return meshlab_load(server, byte_server, file, material, mesh_name, generate_normals=generate_normals,
+                            ordered=ordered_indices)
 
     # Define Meshio helper functions
     def get_point_attr(mesh_obj, attr: str):
         """Helper to get attribute from mesh object"""
 
         data = mesh_obj.point_data.get(attr)
         try:
             return data.tolist()
-        except:
+        except Exception:
             return data
 
     def get_triangles(mesh_obj):
         """Helper to get triangles from mesh object"""
 
         for cell in mesh_obj.cells:
             if cell.type == "triangle":
                 return cell.data.tolist()
-        return None
 
     vertices = mesh.points.tolist()
     indices = get_triangles(mesh)
 
     # I think attribute name is going to be specific to mesh - how to map to right attribute?
     normals = get_point_attr(mesh, "NORMAL")
     tangents = get_point_attr(mesh, "TANGENT")
@@ -561,15 +653,16 @@
         indices=indices,
         index_type="TRIANGLES",
         material=material.id,
         normals=normals,
         tangents=tangents,
         textures=textures,
         colors=colors)
-    patches.append(build_geometry_patch(server, mesh_name, patch_info, byte_server, generate_normals=generate_normals))
+    patches.append(build_geometry_patch(server, mesh_name, patch_info, byte_server,
+                                        generate_normals=generate_normals, ordered_indices=ordered_indices))
     geometry = server.create_component(nooobs.Geometry, name=mesh_name, patches=patches)
 
     return geometry
 
 
 def export_mesh(server: Server, geometry: nooobs.Geometry, new_file_name: str, byte_server: ByteServer = None):
     """Export noodles geometry to mesh file
@@ -592,16 +685,16 @@
         buffer = server.get_delegate(view.source_buffer)
         inline, uri = buffer.inline_bytes, buffer.uri_bytes
         if inline:
             geo_bytes = inline
         else:
             try:
                 geo_bytes = byte_server.get_buffer(uri)
-            except:
-                raise Exception("No byte server specified for uri byte mesh")
+            except Exception as e:
+                raise ValueError(f"No byte server specified for uri byte mesh: {e}")
 
         # Reconstruct indices from buffer
         raw_indices = np.frombuffer(geo_bytes, dtype=FORMAT_MAP[index.format], count=index.count, offset=index.offset)
         grouped = [list(x) for x in zip(*(iter(raw_indices),) * 3)]
         indices.extend(grouped)
 
         # Reconstruct points and attributes from buffer
@@ -623,26 +716,40 @@
         points,
         [("triangle", indices)],
         point_data=point_data)
     mesh.write(new_file_name)
 
 
 def dot_product(v1, v2):
-    """Helper to take dot product"""
+    """Helper to take dot product used in thorough normal calculation"""
     product = 0
     for c1, c2 in zip(v1, v2):
         product += (round(c1, 5) * round(c2, 5))
     return product
 
 
-def calculate_normals(vertices: list[list], indices: list[list]):
-    """TODO"""
+# Old slow version, uses BFS to orient the normals in the same direction
+def calculate_normals_thorough(vertices: list[list], indices: list[list]):
+    """Calculate normals for a mesh
+
+    This method should be used if indices in the mesh are not oriented in the same direction. Normals are calculated
+    using the average of face normals for each vertex. Then BFS is used to orient the normals in the same direction.
 
+    !!! note
+        This method is slow for larger meshes and should be used sparingly.
+
+    Args:
+        vertices (list[list]): list of vertices
+        indices (list[list]): list of indices
+
+    Returns:
+        list[list]: list of normals
+    """
     # Idea: go through all the triangles, and calculate normal for each one and attach average to each vertex
-    print(f"Generating normals for {len(vertices)} vertices")
+    logging.info(f"Generating normals for {len(vertices)} vertices")
     normals = {}
     adjacents = {}
     for triangle in indices:
 
         # Calculate the normal
         v1, v2, v3 = triangle
         p1, p2, p3 = vertices[v1], vertices[v2], vertices[v3]
@@ -651,44 +758,45 @@
         normal = np.cross(vector1, vector2)
 
         # Attach normal to each vertex
         for vertex in triangle:
 
             existing_normals = normals.get(vertex)
 
-            # Add in new normals with matching orientation
+            # Add in new normals with matching orientation,
+            # Assumes normals will be in same direction for adjacent triangles (no sharp points)
             if existing_normals:
                 if dot_product(existing_normals[0], normal) < 0:
                     existing_normals.append([-x for x in normal])
-                    print(f"Mismatching triangle normals @ {vertex}")
+                    logging.info(f"Mismatching triangle normals @ {vertex}")
                 else:
                     existing_normals.append(normal)
             else:
                 normals[vertex] = [normal]
 
             # Mark other vertices in triangle as adjacent
             other_vert = [x for x in triangle if x != vertex]
             adjacents.setdefault(vertex, set()).update(other_vert)
 
-    print(f"Vertices {len(vertices)} vs. Normals {len(normals)}")
+    logging.info(f"Vertices {len(vertices)} vs. Normals {len(normals)}")
 
     # Find averages
     for vertex, normal_list in normals.items():
 
         # Calculate average
         average_normal = []
         for component in zip(*normal_list):
             average_normal.append(mean(component))
 
-        # Normalize and set normal to keep track of final average 
+        # Normalize and set normal to keep track of final average
         length = sqrt((average_normal[0] ** 2) + (average_normal[1] ** 2) + (average_normal[2] ** 2))
         normals[vertex] = [x / length for x in average_normal]
 
     # Orient normals to match
-    print(f"Vertices {len(vertices)} vs. Normals {len(normals)}")
+    logging.info(f"Vertices {len(vertices)} vs. Normals {len(normals)}")
 
     center = [mean(x) for x in zip(*vertices)]
     visited = set()
     starting_index = indices[0][0]
     discovered = deque()  # (index, neighbor)
     discovered.append((starting_index, starting_index))
     while discovered:
@@ -701,23 +809,79 @@
 
         for adjacent in adjacents[current_index]:
             if adjacent not in visited and (adjacent, current_index) not in discovered:
                 discovered.append((adjacent, current_index))
 
         visited.add(current_index)
 
-    print(f"Vertices {len(vertices)} vs. Normals {len(normals)}")
+    logging.info(f"Vertices {len(vertices)} vs. Normals {len(normals)}")
     # Find number pointing towards center
     num_inward = 0
     for index, normal in normals.items():
         center_vector = [x - y for x, y in zip(vertices[index], center)]
         if np.dot(normal, center_vector) < 0:
             num_inward += 1
 
     # If majority are inward invert
     if num_inward > (len(vertices) / 2):
         for key, normal in normals.items():
             normals[key] = [-x for x in normal]
 
-    print(f"Finished getting normals...\nNum Inward: {num_inward}")
-    print(f"Vertices {len(vertices)} vs. Normals {len(normals)}")
+    logging.info(f"Finished getting normals...\nNum Inward: {num_inward}")
+    logging.info(f"Vertices {len(vertices)} vs. Normals {len(normals)}")
     return [normals.get(i, [0, 0, 0]) for i in range(len(vertices))]
+
+
+def calculate_normals(vertices, indices, ordered=True):
+    """Calculate normals for a mesh
+
+    By default, assumes indices are oriented in the same direction. If not, normals will be calculated incorrectly.
+    If the ordered flag is set to false, a slower more intense method for calculating normals will be used.
+
+    !!! note
+        If you are using `build_geometry_patch` or `geometry_from_mesh`, normals will calculated automatically if
+        they are not provided
+
+    Args:
+        vertices (list[list]): list of vertices
+        indices (list[list]): list of indices
+        ordered (bool): whether indices are ordered in the same direction
+
+    Returns:
+        list[list]: list of normals
+    """
+
+    # If indices are not ordered in any way, hand off to thorough method
+    if not ordered:
+        return calculate_normals_thorough(vertices, indices)
+
+    # Cast vertices and indices to numpy arrays
+    vertices = np.array(vertices).astype(np.float64)
+    indices = np.array(indices)
+
+    # Initialize an empty array for vertex normals
+    vertex_normals = np.zeros_like(vertices)
+
+    # Iterate over each face
+    for face_indices in indices:
+        # Get the vertices of the face
+        face_vertices = vertices[face_indices]
+
+        # Calculate the face normal using cross product
+        edge1 = face_vertices[1] - face_vertices[0]
+        edge2 = face_vertices[2] - face_vertices[0]
+        face_normal = np.cross(edge1, edge2)
+
+        # Add the face normal to each vertex normal adjacent to the face
+        vertex_normals[face_indices] += face_normal
+
+    # Normalize the vertex normals
+    magnitudes = np.linalg.norm(vertex_normals, axis=1)
+    vertex_normals /= magnitudes[:, np.newaxis]
+
+    # Check how many are facing center and flip if majority is inward
+    dot_prods = np.sum(vertex_normals * vertices, axis=1)
+    num_inward = np.sum(dot_prods < 0)
+    if num_inward > (len(vertices) / 2):
+        vertex_normals = -vertex_normals
+
+    return vertex_normals.tolist()
```

### Comparing `rigatoni-0.2.2/PKG-INFO` & `rigatoni-0.2.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rigatoni
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python Server Library for NOODLES Protocol
 Keywords: noodles,cbor,Websockets,server,NOODLES
 Author: Alex Racapé
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
@@ -14,36 +14,39 @@
 Requires-Dist: pydantic
 Requires-Dist: numpy ; extra == "geometry"
 Requires-Dist: meshio ; extra == "geometry"
 Requires-Dist: pytest ; extra == "testing"
 Requires-Dist: penne ; extra == "testing"
 Requires-Dist: pandas ; extra == "testing"
 Requires-Dist: matplotlib ; extra == "testing"
+Requires-Dist: meshio ; extra == "testing"
+Requires-Dist: pymeshlab ; extra == "testing"
+Project-URL: Documentation, https://insightcenternoodles.github.io/Rigatoni/
 Project-URL: Source, https://github.com/InsightCenterNoodles/Rigatoni
 Provides-Extra: geometry
 Provides-Extra: testing
 
+
 # Rigatoni
 
 ![Build Status](https://github.com/InsightCenterNoodles/Rigatoni/workflows/CI/badge.svg)
 ![PyPI](https://img.shields.io/pypi/v/Rigatoni)
-[![Coverage badge](https://raw.githubusercontent.com/InsightCenterNoodles/Rigatoni/python-coverage-comment-action-data/badge.svg)](https://htmlpreview.github.io/?https://github.com/InsightCenterNoodles/Rigatoni/blob/python-coverage-comment-action-data/htmlcov/index.html)
-
+[![Coverage badge](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/InsightCenterNoodles/Rigatoni/python-coverage-comment-action-data/endpoint.json&color=brightgreen)](https://htmlpreview.github.io/?https://github.com/InsightCenterNoodles/Rigatoni/blob/python-coverage-comment-action-data/htmlcov/index.html)
 
 Python Server Library for NOODLES Protocol
 
 ## Description
 This server library implements the NOODLES messaging protocol and provides objects for maintaining a scene in state. 
 The server uses a websocket connection to send CBOR encoded messages. To customize its implementation, the library 
 provides convenient interface methods to assist the user in writing their own methods for the server. The user can
 also add custom delegates to add additional functionality to any of the standard components.
 
 ## Documentation
 
-For more information and documentation, check out [the documentation](https://insightcenternoodles.github.io/Rigatoni/).
+For more information, check out [the documentation](https://insightcenternoodles.github.io/Rigatoni/).
 
 ## Installation
 
 Installation is as simple as:
 
 ```bash
 pip install rigatoni
@@ -80,9 +83,9 @@
 
 with rig.Server(50000, starting_state) as server:
     # do stuff
     pass
 ```
 
 ## Hungry for more NOODLES?
-For more information and other related repositories check out [this repository](https://github.com/InsightCenterNoodles)
+For more information and other related repositories check out [this collection](https://github.com/InsightCenterNoodles)
```

