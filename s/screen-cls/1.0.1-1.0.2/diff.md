# Comparing `tmp/screen_cls-1.0.1.tar.gz` & `tmp/screen_cls-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "screen_cls-1.0.1.tar", last modified: Thu Jun 22 18:48:42 2023, max compression
+gzip compressed data, was "screen_cls-1.0.2.tar", last modified: Thu Jun 22 19:24:04 2023, max compression
```

## Comparing `screen_cls-1.0.1.tar` & `screen_cls-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 18:48:42.743242 screen_cls-1.0.1/
--rw-rw-rw-   0        0        0     1101 2023-06-22 11:49:23.000000 screen_cls-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      912 2023-06-22 18:48:42.744243 screen_cls-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      276 2023-06-22 18:44:10.000000 screen_cls-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 18:48:42.705244 screen_cls-1.0.1/screen_cls/
--rw-rw-rw-   0        0        0        0 2023-06-22 12:24:08.000000 screen_cls-1.0.1/screen_cls/_init_.py
--rw-rw-rw-   0        0        0       99 2023-06-22 12:51:35.000000 screen_cls-1.0.1/screen_cls/example.py
--rw-rw-rw-   0        0        0      189 2023-06-22 12:49:42.000000 screen_cls-1.0.1/screen_cls/screen_cls.py
-drwxrwxrwx   0        0        0        0 2023-06-22 18:48:42.741244 screen_cls-1.0.1/screen_cls.egg-info/
--rw-rw-rw-   0        0        0      912 2023-06-22 18:48:42.000000 screen_cls-1.0.1/screen_cls.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2023-06-22 18:48:42.000000 screen_cls-1.0.1/screen_cls.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 18:48:42.000000 screen_cls-1.0.1/screen_cls.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-22 18:48:42.000000 screen_cls-1.0.1/screen_cls.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-22 18:48:42.761247 screen_cls-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      787 2023-06-22 18:47:53.000000 screen_cls-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 19:24:04.267793 screen_cls-1.0.2/
+-rw-rw-rw-   0        0        0     1101 2023-06-22 11:49:23.000000 screen_cls-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      914 2023-06-22 19:24:04.268793 screen_cls-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2023-06-22 19:22:26.000000 screen_cls-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 19:24:04.214801 screen_cls-1.0.2/screen_cls/
+-rw-rw-rw-   0        0        0        0 2023-06-22 12:24:08.000000 screen_cls-1.0.2/screen_cls/_init_.py
+-rw-rw-rw-   0        0        0       99 2023-06-22 12:51:35.000000 screen_cls-1.0.2/screen_cls/example.py
+-rw-rw-rw-   0        0        0      189 2023-06-22 12:49:42.000000 screen_cls-1.0.2/screen_cls/main.py
+drwxrwxrwx   0        0        0        0 2023-06-22 19:24:04.261804 screen_cls-1.0.2/screen_cls.egg-info/
+-rw-rw-rw-   0        0        0      914 2023-06-22 19:24:03.000000 screen_cls-1.0.2/screen_cls.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-06-22 19:24:03.000000 screen_cls-1.0.2/screen_cls.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 19:24:03.000000 screen_cls-1.0.2/screen_cls.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-22 19:24:03.000000 screen_cls-1.0.2/screen_cls.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-22 19:24:04.271797 screen_cls-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      787 2023-06-22 19:23:47.000000 screen_cls-1.0.2/setup.py
```

### Comparing `screen_cls-1.0.1/LICENSE` & `screen_cls-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `screen_cls-1.0.1/PKG-INFO` & `screen_cls-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: screen_cls
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python script for clearing screen for any OS's: Windows, MAC, Linux
 Home-page: https://github.com/IgorMan2005/screen_cls
 Author: IgorMan (IgorMan2005)
 Author-email: igorman2005@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://best-itpro.ru/news/screen_cls/
 Keywords: python screen cls
@@ -12,23 +12,24 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# CLS_Screen
+# Screen_CLS
 Python script for clearing screen for any OS's: Windows, MAC, Linux
 
 ## Setup
 https://pypi.org/project/screen-cls/
 
 **pip install screen-cls**
 
 ## Example:
 import screen_cls
+
 screen_cls.cls()
 
 ### Documentation
 https://best-itpro.ru/news/screen_cls/
```

### Comparing `screen_cls-1.0.1/screen_cls.egg-info/PKG-INFO` & `screen_cls-1.0.2/screen_cls.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: screen-cls
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python script for clearing screen for any OS's: Windows, MAC, Linux
 Home-page: https://github.com/IgorMan2005/screen_cls
 Author: IgorMan (IgorMan2005)
 Author-email: igorman2005@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://best-itpro.ru/news/screen_cls/
 Keywords: python screen cls
@@ -12,23 +12,24 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# CLS_Screen
+# Screen_CLS
 Python script for clearing screen for any OS's: Windows, MAC, Linux
 
 ## Setup
 https://pypi.org/project/screen-cls/
 
 **pip install screen-cls**
 
 ## Example:
 import screen_cls
+
 screen_cls.cls()
 
 ### Documentation
 https://best-itpro.ru/news/screen_cls/
```

### Comparing `screen_cls-1.0.1/setup.py` & `screen_cls-1.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 setup(
   name='screen_cls',
-  version='1.0.1',
+  version='1.0.2',
   author='IgorMan (IgorMan2005)',
   author_email='igorman2005@gmail.com',
   description='Python script for clearing screen for any OS\'s: Windows, MAC, Linux',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/IgorMan2005/screen_cls',
   packages=['screen_cls'],
```

