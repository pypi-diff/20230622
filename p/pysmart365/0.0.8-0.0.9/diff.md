# Comparing `tmp/pysmart365-0.0.8.tar.gz` & `tmp/pysmart365-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysmart365-0.0.8.tar", last modified: Thu Jun 15 10:38:07 2023, max compression
+gzip compressed data, was "pysmart365-0.0.9.tar", last modified: Thu Jun 22 20:40:35 2023, max compression
```

## Comparing `pysmart365-0.0.8.tar` & `pysmart365-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 10:38:07.081788 pysmart365-0.0.8/
--rw-rw-rw-   0        0        0    35803 2023-06-02 13:24:19.000000 pysmart365-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      353 2023-06-15 10:38:07.081788 pysmart365-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      583 2023-06-02 13:24:19.000000 pysmart365-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 10:38:07.059729 pysmart365-0.0.8/pysmart365/
--rw-rw-rw-   0        0        0     3561 2023-06-15 10:27:55.000000 pysmart365-0.0.8/pysmart365/MicroSoftware.py
--rw-rw-rw-   0        0        0     1822 2023-06-15 10:30:41.000000 pysmart365-0.0.8/pysmart365/__init__.py
--rw-rw-rw-   0        0        0      633 2023-06-15 10:28:22.000000 pysmart365-0.0.8/pysmart365/modules.py
-drwxrwxrwx   0        0        0        0 2023-06-15 10:38:07.080829 pysmart365-0.0.8/pysmart365.egg-info/
--rw-rw-rw-   0        0        0      353 2023-06-15 10:38:06.000000 pysmart365-0.0.8/pysmart365.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2023-06-15 10:38:06.000000 pysmart365-0.0.8/pysmart365.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 10:38:06.000000 pysmart365-0.0.8/pysmart365.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      122 2023-06-15 10:38:06.000000 pysmart365-0.0.8/pysmart365.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-15 10:38:06.000000 pysmart365-0.0.8/pysmart365.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 10:38:07.082786 pysmart365-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      734 2023-06-15 10:31:55.000000 pysmart365-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 20:40:35.681004 pysmart365-0.0.9/
+-rw-rw-rw-   0        0        0    35803 2023-06-02 13:24:19.000000 pysmart365-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      353 2023-06-22 20:40:35.680007 pysmart365-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      554 2023-06-15 10:39:32.000000 pysmart365-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 20:40:35.670034 pysmart365-0.0.9/pysmart365/
+-rw-rw-rw-   0        0        0     3489 2023-06-22 20:38:13.000000 pysmart365-0.0.9/pysmart365/MicroSoftware.py
+-rw-rw-rw-   0        0        0     1822 2023-06-15 10:30:41.000000 pysmart365-0.0.9/pysmart365/__init__.py
+-rw-rw-rw-   0        0        0      635 2023-06-22 20:38:31.000000 pysmart365-0.0.9/pysmart365/modules.py
+drwxrwxrwx   0        0        0        0 2023-06-22 20:40:35.680007 pysmart365-0.0.9/pysmart365.egg-info/
+-rw-rw-rw-   0        0        0      353 2023-06-22 20:40:35.000000 pysmart365-0.0.9/pysmart365.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2023-06-22 20:40:35.000000 pysmart365-0.0.9/pysmart365.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 20:40:35.000000 pysmart365-0.0.9/pysmart365.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      133 2023-06-22 20:40:35.000000 pysmart365-0.0.9/pysmart365.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-22 20:40:35.000000 pysmart365-0.0.9/pysmart365.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-22 20:40:35.681004 pysmart365-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      757 2023-06-22 20:40:33.000000 pysmart365-0.0.9/setup.py
```

### Comparing `pysmart365-0.0.8/LICENSE` & `pysmart365-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pysmart365-0.0.8/pysmart365/MicroSoftware.py` & `pysmart365-0.0.9/pysmart365/MicroSoftware.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,109 +1,114 @@
-from datetime import *
-import datetime
-from datetime import *
-import subprocess
-from pywinauto import Application
+from datetime import datetime
 import os
 import sys
 import time
-from tkinter import messagebox
-
+from tkinter import messagebox, Tk
+from pywinauto import Application
 import pyautogui
-from screeninfo import get_monitors
+
 def view_time():
     view_time = datetime.now().strftime("%H:%M:%S")
     return view_time
+
 def view_date():
     view_date = datetime.now().strftime("%d/%m/%Y")
     return view_date
+
 def sleep(delay):
-    if delay == '0' or None:
-        sleep = time.sleep(0)
-        return sleep
+    if delay == '0' or delay is None:
+        time.sleep(0)
     elif delay:
-        sleep1 = time.sleep(delay)
-        return sleep1
+        time.sleep(delay)
     else:
         print("Error")
-def center_screen(width, height):
-    try:
-        monitors = get_monitors()
-        if monitors:
-            monitor = monitors[0]
-            screen_width = monitor.width
-            screen_height = monitor.height
-            sw = (screen_width - width) // 2
-            sh = (screen_height - height) // 2
-            text = f'{width}x{height}+{sw}+{sh}'
-            return text
-        else:
-            return None
-    except Exception as error:
-        print('Error: ', error)
+
+class center_screen():
+    def __init__(self, width: int = None, height: int = None):
+        screen_width = Tk().winfo_screenwidth()
+        screen_height = Tk().winfo_screenheight()
+        x = (screen_width - width) // 2
+        y = (screen_height - height) // 2
+        self.geometry = f"{width}x{height}+{x}+{y}"
 
 class EXIT():
     def __init__(self):
         sys.exit()
+
 class wintools():
-    def mrt(secs: float) -> None:
-        if os.path.exists(f'C:\Windows\System32\mrt.exe'):
+    def mrt(self, secs: float) -> None:
+        if os.path.exists(r"C:\Windows\System32\mrt.exe"):
             pyautogui.hotkey("winleft", "r")
             pyautogui.typewrite("mrt.exe")
             sleep(0.5)
             pyautogui.press("Enter")
         else:
-            messagebox.showerror("Error not found", f"Programm `mrt.exe` not found.")
-    def diskmgmt(secs: float) -> None:
+            messagebox.showerror("Error not found", f"Program `mrt.exe` not found.")
+
+    def diskmgmt(self, secs: float) -> None:
         pyautogui.hotkey("winleft", "r")
         pyautogui.typewrite("diskmgmt.msc")
-        time.sleep(secs)
+        sleep(secs)
         pyautogui.press("Enter")
-    def computermgmt(secs: float) -> None:
+
+    def computermgmt(self, secs: float) -> None:
         pyautogui.hotkey("winleft", "r")
         pyautogui.typewrite("compmgmt.msc")
         sleep(secs)
         pyautogui.press("Enter")
-    def notepad(secs: float) -> None:
+
+    def notepad(self, secs: float) -> None:
         pyautogui.hotkey("winleft", "r")
         pyautogui.typewrite("notepad.exe")
-        time.sleep(secs)
+        sleep(secs)
         pyautogui.press("Enter")
-    def calculator(secs: float) -> None:
+
+    def calculator(self, secs: float) -> None:
         pyautogui.hotkey("winleft", "r")
         pyautogui.typewrite("calc.exe")
-        time.sleep(secs)
+        sleep(secs)
         pyautogui.press("Enter")
-    def paint(secs: float) -> None:
+
+    def paint(self, secs: float) -> None:
         pyautogui.hotkey("winleft", "r")
         pyautogui.typewrite("mspaint.exe")
-        time.sleep(secs)
-    def taskmgr() -> None:
+        sleep(secs)
+
+    def taskmgr(self) -> None:
         pyautogui.hotkey("ctrl", "shift", "esc")
-    def explorer() -> None:
+
+    def explorer(self) -> None:
         pyautogui.hotkey("winleft", "e")
-    def cmd(secs: float) -> None:
+
+    def cmd(self, secs: float) -> None:
         pyautogui.hotkey("winleft", "r")
         pyautogui.typewrite("cmd.exe")
-        time.sleep(secs)
+        sleep(secs)
         pyautogui.press("Enter")
-    def settings(secs: float) -> None:
+
+    def settings(self, secs: float) -> None:
         pyautogui.hotkey("winleft", "r")
         pyautogui.typewrite("ms-settings:")
         sleep(0.5)
         pyautogui.press("Enter")
-    def ms_store(secs: float) -> None:
+
+    def ms_store(self, secs: float) -> None:
         def check_microsoft_store():
             try:
                 app = Application(backend='uia').start("ms-windows-store://")
                 app.kill()
                 return True
             except Exception:
                 return False
 
         if check_microsoft_store():
             pyautogui.hotkey("winleft", "r")
             pyautogui.typewrite("ms-windows-store://")
             sleep(0.5)
             pyautogui.press("Enter")
         else:
-            messagebox.showerror("Error not found", "Microsoft store not found.")
+            messagebox.showerror("Error not found", "Microsoft Store not found.")
+    def runner(command) -> None:
+        pyautogui.hotkey("winleft", "r")
+        pyautogui.typewrite(command)
+        time.sleep(0.5)
+        pyautogui.press("Enter")
```

### Comparing `pysmart365-0.0.8/pysmart365/__init__.py` & `pysmart365-0.0.9/pysmart365/__init__.py`

 * *Files identical despite different names*

### Comparing `pysmart365-0.0.8/pysmart365/modules.py` & `pysmart365-0.0.9/pysmart365/modules.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 import flask
 from flask import Flask, views, app, config, globals, helpers, logging, cli, ctx, sessions, debughelpers, testing, wrappers, blueprints, scaffold
 from ttkbootstrap import *
 from flask import *
 import random
 import string
 from customtkinter import *
-import pywinauto
+import pywinauto
```

### Comparing `pysmart365-0.0.8/setup.py` & `pysmart365-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from setuptools import *
 setup(
     author="Runkang",
     author_email="informatic3650@gmail.com",
     name="pysmart365",
     packages=['pysmart365'],
-    version='0.0.8',
+    version='0.0.9',
     long_description='''This module is to simplify the functions of MicroSoftware and SmartSoft.''',
     description='This module is to simplify the functions of MicroSoftware and SmartSoft.',
     install_requires=[
         'screeninfo',
         'pandas',
         'pyautogui',
         'pytube',
         'pytube3',
         'firebase_admin',
         'customtkinter',
         'requests',
         'flask',
         'ttkbootstrap',
         'configparse',
-        'pywinauto'
+        'pywinauto',
+        'jsonschema'
         ],
     url="https://github.com/informatic365/PySmart365/"
 )
```

