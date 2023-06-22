# Comparing `tmp/pyManson-1.2.0.tar.gz` & `tmp/pyManson-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyManson-1.2.0.tar", last modified: Thu Mar 31 09:41:31 2022, max compression
+gzip compressed data, was "pyManson-1.2.1.tar", last modified: Thu Jun 22 15:32:10 2023, max compression
```

## Comparing `pyManson-1.2.0.tar` & `pyManson-1.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 niehaus   (1000) niehaus   (1000)        0 2022-03-31 09:41:31.346974 pyManson-1.2.0/
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)     1076 2022-03-24 20:31:18.000000 pyManson-1.2.0/LICENSE
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      118 2022-03-09 07:44:44.000000 pyManson-1.2.0/MANIFEST.in
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      728 2022-03-31 09:41:31.346974 pyManson-1.2.0/PKG-INFO
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)     1093 2022-03-24 17:36:57.000000 pyManson-1.2.0/README.md
-drwxrwxr-x   0 niehaus   (1000) niehaus   (1000)        0 2022-03-31 09:41:31.346974 pyManson-1.2.0/pyManson/
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      149 2022-03-31 09:41:17.000000 pyManson-1.2.0/pyManson/__init__.py
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)     8042 2022-03-29 21:01:14.000000 pyManson-1.2.0/pyManson/mansonClass.py
-drwxrwxr-x   0 niehaus   (1000) niehaus   (1000)        0 2022-03-31 09:41:31.346974 pyManson-1.2.0/pyManson.egg-info/
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      728 2022-03-31 09:41:31.000000 pyManson-1.2.0/pyManson.egg-info/PKG-INFO
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      283 2022-03-31 09:41:31.000000 pyManson-1.2.0/pyManson.egg-info/SOURCES.txt
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)        1 2022-03-31 09:41:31.000000 pyManson-1.2.0/pyManson.egg-info/dependency_links.txt
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)        1 2022-03-24 20:39:14.000000 pyManson-1.2.0/pyManson.egg-info/not-zip-safe
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)        9 2022-03-31 09:41:31.000000 pyManson-1.2.0/pyManson.egg-info/requires.txt
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)        9 2022-03-31 09:41:31.000000 pyManson-1.2.0/pyManson.egg-info/top_level.txt
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      448 2022-03-31 09:41:31.346974 pyManson-1.2.0/setup.cfg
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      936 2022-03-31 09:41:17.000000 pyManson-1.2.0/setup.py
+drwxrwxr-x   0 niehaus   (1000) niehaus   (1000)        0 2023-06-22 15:32:10.509248 pyManson-1.2.1/
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)     1076 2022-03-24 20:31:18.000000 pyManson-1.2.1/LICENSE
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      118 2022-03-09 07:44:44.000000 pyManson-1.2.1/MANIFEST.in
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      709 2023-06-22 15:32:10.509248 pyManson-1.2.1/PKG-INFO
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)     1093 2022-03-24 17:36:57.000000 pyManson-1.2.1/README.md
+drwxrwxr-x   0 niehaus   (1000) niehaus   (1000)        0 2023-06-22 15:32:10.509248 pyManson-1.2.1/pyManson/
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      149 2023-06-22 14:43:07.000000 pyManson-1.2.1/pyManson/__init__.py
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)     8168 2023-06-22 14:43:07.000000 pyManson-1.2.1/pyManson/mansonClass.py
+drwxrwxr-x   0 niehaus   (1000) niehaus   (1000)        0 2023-06-22 15:32:10.509248 pyManson-1.2.1/pyManson.egg-info/
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      709 2023-06-22 15:32:10.000000 pyManson-1.2.1/pyManson.egg-info/PKG-INFO
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      283 2023-06-22 15:32:10.000000 pyManson-1.2.1/pyManson.egg-info/SOURCES.txt
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)        1 2023-06-22 15:32:10.000000 pyManson-1.2.1/pyManson.egg-info/dependency_links.txt
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)        1 2022-03-24 20:39:14.000000 pyManson-1.2.1/pyManson.egg-info/not-zip-safe
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)        9 2023-06-22 15:32:10.000000 pyManson-1.2.1/pyManson.egg-info/requires.txt
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)        9 2023-06-22 15:32:10.000000 pyManson-1.2.1/pyManson.egg-info/top_level.txt
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      448 2023-06-22 15:32:10.509248 pyManson-1.2.1/setup.cfg
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      938 2023-06-22 15:25:03.000000 pyManson-1.2.1/setup.py
```

### Comparing `pyManson-1.2.0/LICENSE` & `pyManson-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyManson-1.2.0/PKG-INFO` & `pyManson-1.2.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: pyManson
-Version: 1.2.0
+Version: 1.2.1
 Summary: Communcation package for Manson power supply
 Author: Konstantin Niehaus
 Author-email: konstantin+pypi@niehaus-web.com
 License: MIT
 Keywords: power supply,manson,serial
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: System :: Hardware
 Classifier: Topic :: System :: Hardware :: Hardware Drivers
 Classifier: Topic :: Scientific/Engineering
 License-File: LICENSE
 
 Serial communication to Manson power supply is initialized. All commands mentioned in the device manual can be used. Convenience functions for setting current, voltage, locking the device screen, ... have been implemented
-
```

### Comparing `pyManson-1.2.0/README.md` & `pyManson-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pyManson-1.2.0/pyManson/mansonClass.py` & `pyManson-1.2.1/pyManson/mansonClass.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,25 +26,33 @@
         # GMAX Return value: ["Device ID", "Max. supply voltage", "Max. current", "Current scale factor"]
         "605160": ["HCS-3404", 60, 16, 0.1],
         "362120": ["HCS-3202", 36, 10, 0.1],
         "402502": ["SDP-2405", 40, 5, 0.01],
     }
     device_type = ""
     current_factor = 1
-    __logger = logging.getLogger(__name__)
-    __logger.setLevel(logging.DEBUG)
 
-    def __init__(self, port: str, mode: int = 232, channel: int = -1, sp=None):
+    def __init__(
+        self,
+        port: str,
+        mode: int = 232,
+        channel: int = -1,
+        sp=None,
+        loglvl=logging.INFO,
+    ):
         """
         Open Manson Device HCS or SDP at ``port`` or Channel and clear both input and
         output buffer. The serial interface can be accessed via ``self.sp``.
 
         :param port: path to port (default */dev/ttyUSB0*)
         :param serial.Serial sp: parse serial interface directly
         """
+        self.__logger = logging.getLogger(__name__ + "@" + port)
+        self.__logger.setLevel(loglvl)
+
         if mode not in self.supported_modes:
             msg = f"Interface {mode} is not supported only {self.supported_modes}"
             raise ValueError(msg)
         if mode == 232 and channel != -1:
             channel = -1
             self.__logger.warning("Channel information is ignored in RS232 mode.")
         elif mode == 485 and (channel < 0 or channel > 255):
@@ -54,15 +62,15 @@
         self.mode = mode
         self.port = port  # Open serial port.
         self.get_serial()  # open serial port
         self.channel = channel
         self.sp.flushInput()  # Clears input buffer.
         self.sp.flushOutput()  # Clears output buffer.
 
-    def test(self):
+    def test(self) -> bool:
         self.init_serial()
         return True
 
     def get_serial(self):
         """
         Initialize serial interface
 
@@ -78,22 +86,23 @@
         )
         # sp = serial.Serial(self.port, baudrate=9600, parity='N', bytesize=8, stopbits=1, timeout=0.1, inter_byte_timeout=0.02)
         if sp.isOpen():
             sp.close()
         sp.open()
         self.sp = sp
 
-    def readline(self):
+    def readline(self) -> str:
         """
         Read data from ``port``.
         """
         n = 0
         line = self.sp.read_until(b"\rOK\r")
         while len(line) == 0 and n < 100:
             line = self.sp.read_until(b"\rOK\r")
+
         if n == 100:
             raise
         line = line.replace(b"\r", b"")
         line = line.replace(b"OK", b"")
         line = line.decode("utf-8")
         return line
```

### Comparing `pyManson-1.2.0/pyManson.egg-info/PKG-INFO` & `pyManson-1.2.1/pyManson.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: pyManson
-Version: 1.2.0
+Version: 1.2.1
 Summary: Communcation package for Manson power supply
 Author: Konstantin Niehaus
 Author-email: konstantin+pypi@niehaus-web.com
 License: MIT
 Keywords: power supply,manson,serial
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: System :: Hardware
 Classifier: Topic :: System :: Hardware :: Hardware Drivers
 Classifier: Topic :: Scientific/Engineering
 License-File: LICENSE
 
 Serial communication to Manson power supply is initialized. All commands mentioned in the device manual can be used. Convenience functions for setting current, voltage, locking the device screen, ... have been implemented
-
```

### Comparing `pyManson-1.2.0/setup.py` & `pyManson-1.2.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 name = "pyManson"
-version='1.2.0'
+version = "1.2.1"
 setup(
     name=name,
     version=version,
     description="Communcation package for Manson power supply",
     author="Konstantin Niehaus",
     author_email="konstantin+pypi@niehaus-web.com",
     license="MIT",
```

