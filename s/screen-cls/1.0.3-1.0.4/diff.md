# Comparing `tmp/screen_cls-1.0.3.tar.gz` & `tmp/screen_cls-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "screen_cls-1.0.3.tar", last modified: Thu Jun 22 19:33:54 2023, max compression
+gzip compressed data, was "screen_cls-1.0.4.tar", last modified: Thu Jun 22 19:37:19 2023, max compression
```

## Comparing `screen_cls-1.0.3.tar` & `screen_cls-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 19:33:54.708783 screen_cls-1.0.3/
--rw-rw-rw-   0        0        0     1101 2023-06-22 11:49:23.000000 screen_cls-1.0.3/LICENSE
--rw-rw-rw-   0        0        0      914 2023-06-22 19:33:54.708783 screen_cls-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      278 2023-06-22 19:22:26.000000 screen_cls-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 19:33:54.576781 screen_cls-1.0.3/screen_cls/
--rw-rw-rw-   0        0        0        0 2023-06-22 12:24:08.000000 screen_cls-1.0.3/screen_cls/_init_.py
--rw-rw-rw-   0        0        0       99 2023-06-22 12:51:35.000000 screen_cls-1.0.3/screen_cls/example.py
--rw-rw-rw-   0        0        0      189 2023-06-22 12:49:42.000000 screen_cls-1.0.3/screen_cls/main.py
-drwxrwxrwx   0        0        0        0 2023-06-22 19:33:54.697784 screen_cls-1.0.3/screen_cls.egg-info/
--rw-rw-rw-   0        0        0      914 2023-06-22 19:33:54.000000 screen_cls-1.0.3/screen_cls.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-06-22 19:33:54.000000 screen_cls-1.0.3/screen_cls.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 19:33:54.000000 screen_cls-1.0.3/screen_cls.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-22 19:33:54.000000 screen_cls-1.0.3/screen_cls.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-22 19:33:54.754782 screen_cls-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      787 2023-06-22 19:33:48.000000 screen_cls-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 19:37:19.441943 screen_cls-1.0.4/
+-rw-rw-rw-   0        0        0     1101 2023-06-22 11:49:23.000000 screen_cls-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0      914 2023-06-22 19:37:19.442943 screen_cls-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2023-06-22 19:22:26.000000 screen_cls-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 19:37:19.400946 screen_cls-1.0.4/screen_cls/
+-rw-rw-rw-   0        0        0        0 2023-06-22 12:24:08.000000 screen_cls-1.0.4/screen_cls/_init_.py
+-rw-rw-rw-   0        0        0       99 2023-06-22 12:51:35.000000 screen_cls-1.0.4/screen_cls/example.py
+-rw-rw-rw-   0        0        0      147 2023-06-22 19:37:05.000000 screen_cls-1.0.4/screen_cls/main.py
+drwxrwxrwx   0        0        0        0 2023-06-22 19:37:19.437946 screen_cls-1.0.4/screen_cls.egg-info/
+-rw-rw-rw-   0        0        0      914 2023-06-22 19:37:19.000000 screen_cls-1.0.4/screen_cls.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-06-22 19:37:19.000000 screen_cls-1.0.4/screen_cls.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 19:37:19.000000 screen_cls-1.0.4/screen_cls.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-22 19:37:19.000000 screen_cls-1.0.4/screen_cls.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-22 19:37:19.445945 screen_cls-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      787 2023-06-22 19:37:14.000000 screen_cls-1.0.4/setup.py
```

### Comparing `screen_cls-1.0.3/LICENSE` & `screen_cls-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `screen_cls-1.0.3/PKG-INFO` & `screen_cls-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: screen_cls
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python script for clearing screen for any OS's: Windows, MAC, Linux
 Home-page: https://github.com/IgorMan2005/screen_cls
 Author: IgorMan (IgorMan2005)
 Author-email: igorman2005@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://best-itpro.ru/news/screen_cls/
 Keywords: python screen cls
```

### Comparing `screen_cls-1.0.3/screen_cls.egg-info/PKG-INFO` & `screen_cls-1.0.4/screen_cls.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: screen-cls
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python script for clearing screen for any OS's: Windows, MAC, Linux
 Home-page: https://github.com/IgorMan2005/screen_cls
 Author: IgorMan (IgorMan2005)
 Author-email: igorman2005@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://best-itpro.ru/news/screen_cls/
 Keywords: python screen cls
```

### Comparing `screen_cls-1.0.3/setup.py` & `screen_cls-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 setup(
   name='screen_cls',
-  version='1.0.3',
+  version='1.0.4',
   author='IgorMan (IgorMan2005)',
   author_email='igorman2005@gmail.com',
   description='Python script for clearing screen for any OS\'s: Windows, MAC, Linux',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/IgorMan2005/screen_cls',
   packages=['screen_cls'],
```

