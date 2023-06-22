# Comparing `tmp/ARIclicker-0.1.8.tar.gz` & `tmp/ARIclicker-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ARIclicker-0.1.8.tar", last modified: Thu Jun 22 04:13:47 2023, max compression
+gzip compressed data, was "ARIclicker-0.1.9.tar", last modified: Thu Jun 22 07:33:51 2023, max compression
```

## Comparing `ARIclicker-0.1.8.tar` & `ARIclicker-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 04:13:47.187869 ARIclicker-0.1.8/
-drwxrwxrwx   0        0        0        0 2023-06-22 04:13:47.140980 ARIclicker-0.1.8/ARIclicker/
--rw-rw-rw-   0        0        0     3031 2023-06-18 10:40:37.000000 ARIclicker-0.1.8/ARIclicker/__init__.py
--rw-rw-rw-   0        0        0        2 2023-05-03 11:07:38.000000 ARIclicker-0.1.8/ARIclicker/file.py
-drwxrwxrwx   0        0        0        0 2023-06-22 04:13:47.172238 ARIclicker-0.1.8/ARIclicker.egg-info/
--rw-rw-rw-   0        0        0     1601 2023-06-22 04:13:47.000000 ARIclicker-0.1.8/ARIclicker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-06-22 04:13:47.000000 ARIclicker-0.1.8/ARIclicker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 04:13:47.000000 ARIclicker-0.1.8/ARIclicker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-22 04:13:47.000000 ARIclicker-0.1.8/ARIclicker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-22 04:13:47.000000 ARIclicker-0.1.8/ARIclicker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1601 2023-06-22 04:13:47.172238 ARIclicker-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     1245 2023-06-22 04:08:21.000000 ARIclicker-0.1.8/README.md
--rw-rw-rw-   0        0        0     1093 2023-06-22 03:55:50.000000 ARIclicker-0.1.8/license.txt
--rw-rw-rw-   0        0        0       42 2023-06-22 04:13:47.187869 ARIclicker-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      673 2023-06-22 04:13:37.000000 ARIclicker-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 07:33:51.473695 ARIclicker-0.1.9/
+drwxrwxrwx   0        0        0        0 2023-06-22 07:33:51.426823 ARIclicker-0.1.9/ARIclicker/
+-rw-rw-rw-   0        0        0     3099 2023-06-22 07:32:37.000000 ARIclicker-0.1.9/ARIclicker/__init__.py
+-rw-rw-rw-   0        0        0     1530 2023-06-22 07:29:28.000000 ARIclicker-0.1.9/ARIclicker/a.py
+-rw-rw-rw-   0        0        0        2 2023-05-03 11:07:38.000000 ARIclicker-0.1.9/ARIclicker/file.py
+drwxrwxrwx   0        0        0        0 2023-06-22 07:33:51.458072 ARIclicker-0.1.9/ARIclicker.egg-info/
+-rw-rw-rw-   0        0        0     1601 2023-06-22 07:33:51.000000 ARIclicker-0.1.9/ARIclicker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2023-06-22 07:33:51.000000 ARIclicker-0.1.9/ARIclicker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 07:33:51.000000 ARIclicker-0.1.9/ARIclicker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-22 07:33:51.000000 ARIclicker-0.1.9/ARIclicker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-22 07:33:51.000000 ARIclicker-0.1.9/ARIclicker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1601 2023-06-22 07:33:51.473695 ARIclicker-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1245 2023-06-22 04:08:21.000000 ARIclicker-0.1.9/README.md
+-rw-rw-rw-   0        0        0     1093 2023-06-22 03:55:50.000000 ARIclicker-0.1.9/license.txt
+-rw-rw-rw-   0        0        0       42 2023-06-22 07:33:51.473695 ARIclicker-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      673 2023-06-22 07:33:45.000000 ARIclicker-0.1.9/setup.py
```

### Comparing `ARIclicker-0.1.8/ARIclicker/__init__.py` & `ARIclicker-0.1.9/ARIclicker/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import time
 import threading
 from pynput.mouse import Button, Controller
 from pynput.keyboard import Listener, KeyCode
+import pynput
 import random
 
 
 class ClickMouse(threading.Thread):
     def __init__(self, delay_min, delay_max, button):
         super(ClickMouse, self).__init__()
         self.delay_min = delay_min
@@ -35,15 +36,15 @@
 def autoclick(start_stop_key_character, end_key_character, delay_min, delay_max, button):
     if button == "left":
         button = Button.left
     if button == "right":
         button = Button.right
     start_stop_key = KeyCode(char=start_stop_key_character)
     stop_key = KeyCode(char=end_key_character)
-    mouse = Controller()
+    mouse = pynput.mouse.Controller()
     click_thread = ClickMouse(delay_min, delay_max, button)
     click_thread.start()
 
     def on_press(key):
         if key == start_stop_key:
             if click_thread.running:
                 click_thread.stop_clicking()
@@ -74,15 +75,15 @@
             self.running = False
 
         def exit(self):
             self.stop_pressing()
             self.program_running = False
 
         def run(self):
-            key = Controller()
+            key = pynput.keyboard.Controller()
             while self.program_running:
                 while self.running:
                     key.press(button)
 
     start_stop_key = KeyCode(char=start_stop_key_character)
     stop_key = KeyCode(char=end_key_character)
     press_thread = PressKey(button)
@@ -96,7 +97,8 @@
                 press_thread.start_pressing()
         elif key == stop_key:
             press_thread.exit()
             listener.stop()
     with Listener(on_press=on_press) as listener:
         listener.join()
 
+autopress("q","w","e")
```

### Comparing `ARIclicker-0.1.8/ARIclicker.egg-info/PKG-INFO` & `ARIclicker-0.1.9/ARIclicker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ARIclicker
-Version: 0.1.8
+Version: 0.1.9
 Summary: AutoRandomIntervalClicker
 Home-page: UNKNOWN
 Author: lin_zhe
 Author-email: 2081812728@qq.com
 Maintainer: lin_zhe
 License: MIT License
 Keywords: AutoRandomIntervalClicker
```

### Comparing `ARIclicker-0.1.8/PKG-INFO` & `ARIclicker-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ARIclicker
-Version: 0.1.8
+Version: 0.1.9
 Summary: AutoRandomIntervalClicker
 Home-page: UNKNOWN
 Author: lin_zhe
 Author-email: 2081812728@qq.com
 Maintainer: lin_zhe
 License: MIT License
 Keywords: AutoRandomIntervalClicker
```

### Comparing `ARIclicker-0.1.8/README.md` & `ARIclicker-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `ARIclicker-0.1.8/license.txt` & `ARIclicker-0.1.9/license.txt`

 * *Files identical despite different names*

### Comparing `ARIclicker-0.1.8/setup.py` & `ARIclicker-0.1.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 setup(
     name = 'ARIclicker',
-    version = '0.1.8',
+    version = '0.1.9',
     maintainer='lin_zhe',
     keywords='AutoRandomIntervalClicker',
     description = 'AutoRandomIntervalClicker',
     long_description_content_type='text/markdown',
     long_description=long_description,
     license = 'MIT License',
     author = 'lin_zhe',
```

