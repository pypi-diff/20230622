# Comparing `tmp/rtt_console-0.2.6.tar.gz` & `tmp/rtt_console-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtt_console-0.2.6.tar", last modified: Sat Oct 29 08:37:37 2022, max compression
+gzip compressed data, was "rtt_console-0.2.7.tar", last modified: Thu Jun 22 14:59:37 2023, max compression
```

## Comparing `rtt_console-0.2.6.tar` & `rtt_console-0.2.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 viacheslav  (1000) viacheslav  (1000)        0 2022-10-29 08:37:37.285219 rtt_console-0.2.6/
--rw-rw-r--   0 viacheslav  (1000) viacheslav  (1000)     1067 2022-06-05 07:08:56.000000 rtt_console-0.2.6/LICENSE
--rw-rw-r--   0 viacheslav  (1000) viacheslav  (1000)      759 2022-10-29 08:37:37.285219 rtt_console-0.2.6/PKG-INFO
--rw-rw-r--   0 viacheslav  (1000) viacheslav  (1000)      330 2022-06-12 15:48:46.000000 rtt_console-0.2.6/README.md
--rw-rw-r--   0 viacheslav  (1000) viacheslav  (1000)      104 2022-06-12 15:48:46.000000 rtt_console-0.2.6/pyproject.toml
--rw-rw-r--   0 viacheslav  (1000) viacheslav  (1000)      767 2022-10-29 08:37:37.285219 rtt_console-0.2.6/setup.cfg
-drwxrwxr-x   0 viacheslav  (1000) viacheslav  (1000)        0 2022-10-29 08:37:37.281218 rtt_console-0.2.6/src/
-drwxrwxr-x   0 viacheslav  (1000) viacheslav  (1000)        0 2022-10-29 08:37:37.281218 rtt_console-0.2.6/src/rtt_console/
--rw-rw-r--   0 viacheslav  (1000) viacheslav  (1000)      147 2022-06-12 15:48:46.000000 rtt_console-0.2.6/src/rtt_console/__init__.py
--rwxrwxr-x   0 viacheslav  (1000) viacheslav  (1000)     4509 2022-06-24 16:55:30.000000 rtt_console-0.2.6/src/rtt_console/console.py
--rw-rw-r--   0 viacheslav  (1000) viacheslav  (1000)      365 2022-06-24 16:55:30.000000 rtt_console-0.2.6/src/rtt_console/default_command.py
--rw-rw-r--   0 viacheslav  (1000) viacheslav  (1000)     4250 2022-10-29 08:32:15.000000 rtt_console-0.2.6/src/rtt_console/jlink_dongle.py
--rw-rw-r--   0 viacheslav  (1000) viacheslav  (1000)       17 2022-10-29 08:32:12.000000 rtt_console-0.2.6/src/rtt_console/version.py
-drwxrwxr-x   0 viacheslav  (1000) viacheslav  (1000)        0 2022-10-29 08:37:37.285219 rtt_console-0.2.6/src/rtt_console.egg-info/
--rw-rw-r--   0 viacheslav  (1000) viacheslav  (1000)      759 2022-10-29 08:37:37.000000 rtt_console-0.2.6/src/rtt_console.egg-info/PKG-INFO
--rw-rw-r--   0 viacheslav  (1000) viacheslav  (1000)      427 2022-10-29 08:37:37.000000 rtt_console-0.2.6/src/rtt_console.egg-info/SOURCES.txt
--rw-rw-r--   0 viacheslav  (1000) viacheslav  (1000)        1 2022-10-29 08:37:37.000000 rtt_console-0.2.6/src/rtt_console.egg-info/dependency_links.txt
--rw-rw-r--   0 viacheslav  (1000) viacheslav  (1000)       57 2022-10-29 08:37:37.000000 rtt_console-0.2.6/src/rtt_console.egg-info/entry_points.txt
--rw-rw-r--   0 viacheslav  (1000) viacheslav  (1000)       75 2022-10-29 08:37:37.000000 rtt_console-0.2.6/src/rtt_console.egg-info/requires.txt
--rw-rw-r--   0 viacheslav  (1000) viacheslav  (1000)       12 2022-10-29 08:37:37.000000 rtt_console-0.2.6/src/rtt_console.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-22 14:59:37.508949 rtt_console-0.2.7/
+-rw-rw-r--   0 user      (1000) user      (1000)     1067 2023-06-22 13:42:36.000000 rtt_console-0.2.7/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)      759 2023-06-22 14:59:37.508949 rtt_console-0.2.7/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      330 2023-06-22 13:42:36.000000 rtt_console-0.2.7/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)      104 2023-06-22 13:42:36.000000 rtt_console-0.2.7/pyproject.toml
+-rw-rw-r--   0 user      (1000) user      (1000)      767 2023-06-22 14:59:37.508949 rtt_console-0.2.7/setup.cfg
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-22 14:59:37.504949 rtt_console-0.2.7/src/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-22 14:59:37.508949 rtt_console-0.2.7/src/rtt_console/
+-rw-rw-r--   0 user      (1000) user      (1000)      147 2023-06-22 13:42:36.000000 rtt_console-0.2.7/src/rtt_console/__init__.py
+-rwxrwxr-x   0 user      (1000) user      (1000)     4530 2023-06-22 14:56:09.000000 rtt_console-0.2.7/src/rtt_console/console.py
+-rw-rw-r--   0 user      (1000) user      (1000)      365 2023-06-22 13:42:36.000000 rtt_console-0.2.7/src/rtt_console/default_command.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4501 2023-06-22 14:56:09.000000 rtt_console-0.2.7/src/rtt_console/jlink_dongle.py
+-rw-rw-r--   0 user      (1000) user      (1000)       17 2023-06-22 14:31:09.000000 rtt_console-0.2.7/src/rtt_console/version.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-22 14:59:37.508949 rtt_console-0.2.7/src/rtt_console.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)      759 2023-06-22 14:59:37.000000 rtt_console-0.2.7/src/rtt_console.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      427 2023-06-22 14:59:37.000000 rtt_console-0.2.7/src/rtt_console.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-22 14:59:37.000000 rtt_console-0.2.7/src/rtt_console.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       57 2023-06-22 14:59:37.000000 rtt_console-0.2.7/src/rtt_console.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       75 2023-06-22 14:59:37.000000 rtt_console-0.2.7/src/rtt_console.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       12 2023-06-22 14:59:37.000000 rtt_console-0.2.7/src/rtt_console.egg-info/top_level.txt
```

### Comparing `rtt_console-0.2.6/LICENSE` & `rtt_console-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `rtt_console-0.2.6/PKG-INFO` & `rtt_console-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtt_console
-Version: 0.2.6
+Version: 0.2.7
 Summary: Simple Segger RTT console.
 Home-page: https://github.com/Mcublog/rtt-console
 Author: Viacheslav
 Author-email: viacheslav@mcublog.xyz
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rtt_console-0.2.6/setup.cfg` & `rtt_console-0.2.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `rtt_console-0.2.6/src/rtt_console/console.py` & `rtt_console-0.2.7/src/rtt_console/console.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,16 +42,15 @@
             return JLinkIsBroken
 
     return wrap
 
 
 @exception_handling
 def connect(jlink: JLinkDongle) -> bool:
-    jlink.connect()
-    return JLinkCmdSuccess
+    return jlink.connect()
 
 
 @exception_handling
 def reconnect(jlink: JLinkDongle) -> bool:
     jlink.reconnect()
     return JLinkCmdSuccess
 
@@ -108,14 +107,17 @@
                         default=False)
 
     args = parser.parse_args()
     args.speed = 'auto' if args.speed == 0 else args.speed
     jlink = JLinkDongle(chip_name=args.target, speed=args.speed, dll_path=args.path, pwr_target=args.power)
     jlink_broken = connect(jlink)
 
+    if not jlink_broken:
+        return
+
     kill_evt = Event()
     input: Thread = Thread(target=reading_input, args=([kill_evt]), daemon=True)
     input.start()
 
     while not kill_evt.wait(0.01):
         # Try to reconnect to JLink
         if jlink_broken == JLinkIsBroken:
```

### Comparing `rtt_console-0.2.6/src/rtt_console/jlink_dongle.py` & `rtt_console-0.2.7/src/rtt_console/jlink_dongle.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 from colorama import Fore as Clr
 from pylink import JLink, JLinkException, JLinkInterfaces, library
 
 CHIP_NAME_DEFAULT = 'STM32F407VE'
 DEFAULT_BUFFER_INDEX = 0
 
+CODEPAGES = ('utf-8', 'cp866', 'cp1251')
+
 class JLinkDongleException(Exception):
 
     def __init__(self, message):
         self.message = message
         super().__init__(self.message)
 
 @dataclass
@@ -32,25 +34,29 @@
                 if func.__name__ in {self.read_rtt.__name__, self.write_rtt.__name__}:  # type: ignore
                     raise JLinkDongleException(f"Do not read/write from RTT Terminal")
                 raise JLinkDongleException(
                     f"{Clr.RED}ERROR:{Clr.RESET} method name: {Clr.YELLOW}{func.__name__}{Clr.RESET} : {e}")  # type: ignore
         return wrap
 
     @check_exception # type: ignore
-    def connect(self):
+    def connect(self) -> bool:
         jlinkdll = None
         if self.dll_path:
             jlinkdll = library.Library()
             try:
                 print(f"Using path to DLL: {self.dll_path}")
                 jlinkdll.load(self.dll_path)
             except:
                 print(f"ERROR: check path: {self.dll_path}")
-                return
-        self.jlink = JLink(lib=jlinkdll)
+                return False
+        try:
+            self.jlink = JLink(lib=jlinkdll)
+        except Exception as e:
+            print(f"ERROR: JLink libs not found: {e}")
+            return False
         self.jlink.disable_dialog_boxes()
         self.jlink.open()
         self.jlink.power_on() if self.pwr_target else self.jlink.power_off()
         self.jlink.rtt_stop()
         self.jlink.set_tif(JLinkInterfaces.SWD)
         self.jlink.connect(chip_name=self.chip_name, speed=self.speed, verbose=True) # type: ignore
         self.jlink.rtt_start()
@@ -80,20 +86,23 @@
                 break
             cnt += self.jlink.rtt_write(terminal_number, data[cnt:])
         if cnt == 0 or cnt != len(data):
             print(f"Write error: sent {cnt} from {len(data)} bytes")
 
     def read_rtt_string(self, terminal_number: int = DEFAULT_BUFFER_INDEX) -> str:
         data = self.read_rtt(terminal_number=terminal_number)
-        if data:
+        if not data:
+            return ""
+        for coding in CODEPAGES:
             try:
-                return bytes(data).decode('utf-8')
+                return bytes(data).decode(coding)
             except:
-                print(f"Do not decode: {data}")
-                return ""
+                continue
+        else:
+            print(f"Do not decode: {data}")
         return ""
 
     def write_rtt_sring(self, data: str, terminal_number: int = DEFAULT_BUFFER_INDEX) -> None:
         self.write_rtt(str.encode(data, 'utf-8'), terminal_number)
 
     @check_exception # type: ignore
     def reconnect(self):
```

### Comparing `rtt_console-0.2.6/src/rtt_console.egg-info/PKG-INFO` & `rtt_console-0.2.7/src/rtt_console.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtt-console
-Version: 0.2.6
+Version: 0.2.7
 Summary: Simple Segger RTT console.
 Home-page: https://github.com/Mcublog/rtt-console
 Author: Viacheslav
 Author-email: viacheslav@mcublog.xyz
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

