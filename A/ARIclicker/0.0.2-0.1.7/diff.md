# Comparing `tmp/ARIclicker-0.0.2.tar.gz` & `tmp/ARIclicker-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ARIclicker-0.0.2.tar", last modified: Sun May  7 03:51:12 2023, max compression
+gzip compressed data, was "ARIclicker-0.1.7.tar", last modified: Thu Jun 22 03:51:46 2023, max compression
```

## Comparing `ARIclicker-0.0.2.tar` & `ARIclicker-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 03:51:12.813392 ARIclicker-0.0.2/
-drwxrwxrwx   0        0        0        0 2023-05-07 03:51:11.816975 ARIclicker-0.0.2/ARIclicker/
--rw-rw-rw-   0        0        0     1725 2023-05-03 11:07:38.000000 ARIclicker-0.0.2/ARIclicker/__init__.py
--rw-rw-rw-   0        0        0        2 2023-05-03 11:07:38.000000 ARIclicker-0.0.2/ARIclicker/file.py
-drwxrwxrwx   0        0        0        0 2023-05-07 03:51:12.686466 ARIclicker-0.0.2/ARIclicker.egg-info/
--rw-rw-rw-   0        0        0     1198 2023-05-07 03:51:10.000000 ARIclicker-0.0.2/ARIclicker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-05-07 03:51:10.000000 ARIclicker-0.0.2/ARIclicker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 03:51:10.000000 ARIclicker-0.0.2/ARIclicker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-07 03:51:10.000000 ARIclicker-0.0.2/ARIclicker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-07 03:51:10.000000 ARIclicker-0.0.2/ARIclicker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1198 2023-05-07 03:51:12.783410 ARIclicker-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      845 2023-05-07 03:40:28.000000 ARIclicker-0.0.2/README.md
--rw-rw-rw-   0        0        0     1093 2023-05-03 01:46:26.000000 ARIclicker-0.0.2/license.txt
--rw-rw-rw-   0        0        0       42 2023-05-07 03:51:12.857367 ARIclicker-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      581 2023-05-07 03:50:10.000000 ARIclicker-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 03:51:46.464848 ARIclicker-0.1.7/
+drwxrwxrwx   0        0        0        0 2023-06-22 03:51:46.417977 ARIclicker-0.1.7/ARIclicker/
+-rw-rw-rw-   0        0        0     3031 2023-06-18 10:40:37.000000 ARIclicker-0.1.7/ARIclicker/__init__.py
+-rw-rw-rw-   0        0        0        2 2023-05-03 11:07:38.000000 ARIclicker-0.1.7/ARIclicker/file.py
+drwxrwxrwx   0        0        0        0 2023-06-22 03:51:46.449226 ARIclicker-0.1.7/ARIclicker.egg-info/
+-rw-rw-rw-   0        0        0     1184 2023-06-22 03:51:46.000000 ARIclicker-0.1.7/ARIclicker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-06-22 03:51:46.000000 ARIclicker-0.1.7/ARIclicker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 03:51:46.000000 ARIclicker-0.1.7/ARIclicker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-22 03:51:46.000000 ARIclicker-0.1.7/ARIclicker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-22 03:51:46.000000 ARIclicker-0.1.7/ARIclicker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1184 2023-06-22 03:51:46.464848 ARIclicker-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      828 2023-05-07 10:02:54.000000 ARIclicker-0.1.7/README.md
+-rw-rw-rw-   0        0        0     1093 2023-05-03 01:46:26.000000 ARIclicker-0.1.7/license.txt
+-rw-rw-rw-   0        0        0       42 2023-06-22 03:51:46.464848 ARIclicker-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      673 2023-06-22 03:47:56.000000 ARIclicker-0.1.7/setup.py
```

### Comparing `ARIclicker-0.0.2/ARIclicker.egg-info/PKG-INFO` & `ARIclicker-0.1.7/ARIclicker.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,48 @@
 Metadata-Version: 2.1
 Name: ARIclicker
-Version: 0.0.2
-Summary: A random interval clicker who can DIY:AutoRandomIntervalClicker
+Version: 0.1.7
+Summary: AutoRandomIntervalClicker
 Home-page: UNKNOWN
 Author: lin_zhe
 Author-email: 2081812728@qq.com
 Maintainer: lin_zhe
 License: MIT License
 Keywords: AutoRandomIntervalClicker
 Platform: any
 Requires-Python: >=3.0
+Description-Content-Type: text/markdown
 License-File: license.txt
 
-## How to use the ARIclicker? ##
+## How to use the ARIclicker? 
 
-**explanation:** "ARIclicker" is "Auto Random Interval clicker".
-<br> This is a very good autoclicker, easy to use and intelligent.
+**explanation:** 
+"ARIclicker" is "Auto Random Interval clicker".
 
-#### First of all ####
+ This is a very good autoclicker, easy to use and intelligent.
 
-You need to install **ARIclicker**: Open `cmd` and type ```pip install ARIclicker```
 
-####Function####
-**syntax:** `
-ARIclicker.autoclick("start_pause_key","end_key","min_interval(sec)","max_interval(sec)","button")`
+#### First of all 
 
-For instance:<pre><code>import ARIclicker 
-ARIclicker.autoclick("a","b","0.1","1","left")</code></pre>
+You need to install **ARIclicker**: Open `cmd` and type `pip install ARIclicker`
+
+####Function
+**syntax:**
+`
+ARIclicker.autoclick("start_pause_key","end_key","min_interval(sec)","max_interval(sec)","button")
+`
+
+For instance:
+<pre>
+	import ARIclicker 
+	ARIclicker.autoclick("a","b","0.1","1","left")
+</pre>
 
 **explanation:** If you press the "a" key, clicking will start. When you press the "a" key again, clicking will pause. When you press the "b" key, the program will exit. The range of click intervals is between 0.1 and 1 second, and the left mouse button is the key clicked.
-###**have fun~**###
+###**have fun~**
```

### Comparing `ARIclicker-0.0.2/PKG-INFO` & `ARIclicker-0.1.7/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,48 @@
 Metadata-Version: 2.1
 Name: ARIclicker
-Version: 0.0.2
-Summary: A random interval clicker who can DIY:AutoRandomIntervalClicker
+Version: 0.1.7
+Summary: AutoRandomIntervalClicker
 Home-page: UNKNOWN
 Author: lin_zhe
 Author-email: 2081812728@qq.com
 Maintainer: lin_zhe
 License: MIT License
 Keywords: AutoRandomIntervalClicker
 Platform: any
 Requires-Python: >=3.0
+Description-Content-Type: text/markdown
 License-File: license.txt
 
-## How to use the ARIclicker? ##
+## How to use the ARIclicker? 
 
-**explanation:** "ARIclicker" is "Auto Random Interval clicker".
-<br> This is a very good autoclicker, easy to use and intelligent.
+**explanation:** 
+"ARIclicker" is "Auto Random Interval clicker".
 
-#### First of all ####
+ This is a very good autoclicker, easy to use and intelligent.
 
-You need to install **ARIclicker**: Open `cmd` and type ```pip install ARIclicker```
 
-####Function####
-**syntax:** `
-ARIclicker.autoclick("start_pause_key","end_key","min_interval(sec)","max_interval(sec)","button")`
+#### First of all 
 
-For instance:<pre><code>import ARIclicker 
-ARIclicker.autoclick("a","b","0.1","1","left")</code></pre>
+You need to install **ARIclicker**: Open `cmd` and type `pip install ARIclicker`
+
+####Function
+**syntax:**
+`
+ARIclicker.autoclick("start_pause_key","end_key","min_interval(sec)","max_interval(sec)","button")
+`
+
+For instance:
+<pre>
+	import ARIclicker 
+	ARIclicker.autoclick("a","b","0.1","1","left")
+</pre>
 
 **explanation:** If you press the "a" key, clicking will start. When you press the "a" key again, clicking will pause. When you press the "b" key, the program will exit. The range of click intervals is between 0.1 and 1 second, and the left mouse button is the key clicked.
-###**have fun~**###
+###**have fun~**
```

### Comparing `ARIclicker-0.0.2/README.md` & `ARIclicker-0.1.7/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,33 @@
-## How to use the ARIclicker? ##
+## How to use the ARIclicker? 
 
-**explanation:** "ARIclicker" is "Auto Random Interval clicker".
-<br> This is a very good autoclicker, easy to use and intelligent.
+**explanation:** 
+"ARIclicker" is "Auto Random Interval clicker".
 
-#### First of all ####
+ This is a very good autoclicker, easy to use and intelligent.
 
-You need to install **ARIclicker**: Open `cmd` and type ```pip install ARIclicker```
 
-####Function####
-**syntax:** `
-ARIclicker.autoclick("start_pause_key","end_key","min_interval(sec)","max_interval(sec)","button")`
+#### First of all 
 
-For instance:<pre><code>import ARIclicker 
-ARIclicker.autoclick("a","b","0.1","1","left")</code></pre>
+You need to install **ARIclicker**: Open `cmd` and type `pip install ARIclicker`
+
+####Function
+**syntax:**
+`
+ARIclicker.autoclick("start_pause_key","end_key","min_interval(sec)","max_interval(sec)","button")
+`
+
+For instance:
+<pre>
+	import ARIclicker 
+	ARIclicker.autoclick("a","b","0.1","1","left")
+</pre>
 
 **explanation:** If you press the "a" key, clicking will start. When you press the "a" key again, clicking will pause. When you press the "b" key, the program will exit. The range of click intervals is between 0.1 and 1 second, and the left mouse button is the key clicked.
-###**have fun~**###
+###**have fun~**
```

### Comparing `ARIclicker-0.0.2/license.txt` & `ARIclicker-0.1.7/license.txt`

 * *Files identical despite different names*

### Comparing `ARIclicker-0.0.2/setup.py` & `ARIclicker-0.1.7/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from setuptools import setup, find_packages
-
+with open("README.md", "r", encoding='utf-8') as fh:
+    long_description = fh.read()
 setup(
     name = 'ARIclicker',
-    version = '0.0.2',
+    version = '0.1.7',
     maintainer='lin_zhe',
     keywords='AutoRandomIntervalClicker',
-    description = 'A random interval clicker who can DIY:AutoRandomIntervalClicker',
-    long_description=open('README.md').read(),
+    description = 'AutoRandomIntervalClicker',
+    long_description_content_type='text/markdown',
+    long_description=long_description,
     license = 'MIT License',
     author = 'lin_zhe',
     author_email = '2081812728@qq.com',
     packages = find_packages(),
     include_package_data = True,
     python_requires='>=3.0',
     platforms = 'any',
```

