# Comparing `tmp/ARIclicker-0.1.7.tar.gz` & `tmp/ARIclicker-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ARIclicker-0.1.7.tar", last modified: Thu Jun 22 03:51:46 2023, max compression
+gzip compressed data, was "ARIclicker-0.1.8.tar", last modified: Thu Jun 22 04:13:47 2023, max compression
```

## Comparing `ARIclicker-0.1.7.tar` & `ARIclicker-0.1.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 03:51:46.464848 ARIclicker-0.1.7/
-drwxrwxrwx   0        0        0        0 2023-06-22 03:51:46.417977 ARIclicker-0.1.7/ARIclicker/
--rw-rw-rw-   0        0        0     3031 2023-06-18 10:40:37.000000 ARIclicker-0.1.7/ARIclicker/__init__.py
--rw-rw-rw-   0        0        0        2 2023-05-03 11:07:38.000000 ARIclicker-0.1.7/ARIclicker/file.py
-drwxrwxrwx   0        0        0        0 2023-06-22 03:51:46.449226 ARIclicker-0.1.7/ARIclicker.egg-info/
--rw-rw-rw-   0        0        0     1184 2023-06-22 03:51:46.000000 ARIclicker-0.1.7/ARIclicker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-06-22 03:51:46.000000 ARIclicker-0.1.7/ARIclicker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 03:51:46.000000 ARIclicker-0.1.7/ARIclicker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-22 03:51:46.000000 ARIclicker-0.1.7/ARIclicker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-22 03:51:46.000000 ARIclicker-0.1.7/ARIclicker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1184 2023-06-22 03:51:46.464848 ARIclicker-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0      828 2023-05-07 10:02:54.000000 ARIclicker-0.1.7/README.md
--rw-rw-rw-   0        0        0     1093 2023-05-03 01:46:26.000000 ARIclicker-0.1.7/license.txt
--rw-rw-rw-   0        0        0       42 2023-06-22 03:51:46.464848 ARIclicker-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      673 2023-06-22 03:47:56.000000 ARIclicker-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 04:13:47.187869 ARIclicker-0.1.8/
+drwxrwxrwx   0        0        0        0 2023-06-22 04:13:47.140980 ARIclicker-0.1.8/ARIclicker/
+-rw-rw-rw-   0        0        0     3031 2023-06-18 10:40:37.000000 ARIclicker-0.1.8/ARIclicker/__init__.py
+-rw-rw-rw-   0        0        0        2 2023-05-03 11:07:38.000000 ARIclicker-0.1.8/ARIclicker/file.py
+drwxrwxrwx   0        0        0        0 2023-06-22 04:13:47.172238 ARIclicker-0.1.8/ARIclicker.egg-info/
+-rw-rw-rw-   0        0        0     1601 2023-06-22 04:13:47.000000 ARIclicker-0.1.8/ARIclicker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-06-22 04:13:47.000000 ARIclicker-0.1.8/ARIclicker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 04:13:47.000000 ARIclicker-0.1.8/ARIclicker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-22 04:13:47.000000 ARIclicker-0.1.8/ARIclicker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-22 04:13:47.000000 ARIclicker-0.1.8/ARIclicker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1601 2023-06-22 04:13:47.172238 ARIclicker-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1245 2023-06-22 04:08:21.000000 ARIclicker-0.1.8/README.md
+-rw-rw-rw-   0        0        0     1093 2023-06-22 03:55:50.000000 ARIclicker-0.1.8/license.txt
+-rw-rw-rw-   0        0        0       42 2023-06-22 04:13:47.187869 ARIclicker-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      673 2023-06-22 04:13:37.000000 ARIclicker-0.1.8/setup.py
```

### Comparing `ARIclicker-0.1.7/ARIclicker/__init__.py` & `ARIclicker-0.1.8/ARIclicker/__init__.py`

 * *Files identical despite different names*

### Comparing `ARIclicker-0.1.7/ARIclicker.egg-info/PKG-INFO` & `ARIclicker-0.1.8/ARIclicker.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ARIclicker
-Version: 0.1.7
+Version: 0.1.8
 Summary: AutoRandomIntervalClicker
 Home-page: UNKNOWN
 Author: lin_zhe
 Author-email: 2081812728@qq.com
 Maintainer: lin_zhe
 License: MIT License
 Keywords: AutoRandomIntervalClicker
@@ -17,32 +17,51 @@
 
 **explanation:** 
 "ARIclicker" is "Auto Random Interval clicker".
 
  This is a very good autoclicker, easy to use and intelligent.
 
 
-#### First of all 
+### **First of all** 
 
 You need to install **ARIclicker**: Open `cmd` and type `pip install ARIclicker`
 
-####Function
+### Function:
+
 **syntax:**
+
+clicker:
 `
 ARIclicker.autoclick("start_pause_key","end_key","min_interval(sec)","max_interval(sec)","button")
 `
 
-For instance:
+presser:
+`
+ARIclicker.autopress("start_pause_key","end_key","pressed_button")
+`
+
+example 1:
 <pre>
 	import ARIclicker 
 	ARIclicker.autoclick("a","b","0.1","1","left")
+	
 </pre>
 
 **explanation:** If you press the "a" key, clicking will start. When you press the "a" key again, clicking will pause. When you press the "b" key, the program will exit. The range of click intervals is between 0.1 and 1 second, and the left mouse button is the key clicked.
-###**have fun~**
+
+example 2:
+<pre>
+	import ARIclicker
+	ARIclicker.autopress("a","b","c")
+</pre>
+
+**explanation:** If you press the "a" key,pressing will start.When you press the "a" key again, pressing will pause.When you press the "b" key, the program will exit.The 'c' key represents the key that will be pressed.
+
+
+ ### **have fun~**
```

### Comparing `ARIclicker-0.1.7/PKG-INFO` & `ARIclicker-0.1.8/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ARIclicker
-Version: 0.1.7
+Version: 0.1.8
 Summary: AutoRandomIntervalClicker
 Home-page: UNKNOWN
 Author: lin_zhe
 Author-email: 2081812728@qq.com
 Maintainer: lin_zhe
 License: MIT License
 Keywords: AutoRandomIntervalClicker
@@ -17,32 +17,51 @@
 
 **explanation:** 
 "ARIclicker" is "Auto Random Interval clicker".
 
  This is a very good autoclicker, easy to use and intelligent.
 
 
-#### First of all 
+### **First of all** 
 
 You need to install **ARIclicker**: Open `cmd` and type `pip install ARIclicker`
 
-####Function
+### Function:
+
 **syntax:**
+
+clicker:
 `
 ARIclicker.autoclick("start_pause_key","end_key","min_interval(sec)","max_interval(sec)","button")
 `
 
-For instance:
+presser:
+`
+ARIclicker.autopress("start_pause_key","end_key","pressed_button")
+`
+
+example 1:
 <pre>
 	import ARIclicker 
 	ARIclicker.autoclick("a","b","0.1","1","left")
+	
 </pre>
 
 **explanation:** If you press the "a" key, clicking will start. When you press the "a" key again, clicking will pause. When you press the "b" key, the program will exit. The range of click intervals is between 0.1 and 1 second, and the left mouse button is the key clicked.
-###**have fun~**
+
+example 2:
+<pre>
+	import ARIclicker
+	ARIclicker.autopress("a","b","c")
+</pre>
+
+**explanation:** If you press the "a" key,pressing will start.When you press the "a" key again, pressing will pause.When you press the "b" key, the program will exit.The 'c' key represents the key that will be pressed.
+
+
+ ### **have fun~**
```

### Comparing `ARIclicker-0.1.7/license.txt` & `ARIclicker-0.1.8/license.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2018 The Python Packaging Authority
+Copyright (c) 2023 The Python Packaging Authority
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `ARIclicker-0.1.7/setup.py` & `ARIclicker-0.1.8/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 setup(
     name = 'ARIclicker',
-    version = '0.1.7',
+    version = '0.1.8',
     maintainer='lin_zhe',
     keywords='AutoRandomIntervalClicker',
     description = 'AutoRandomIntervalClicker',
     long_description_content_type='text/markdown',
     long_description=long_description,
     license = 'MIT License',
     author = 'lin_zhe',
```

