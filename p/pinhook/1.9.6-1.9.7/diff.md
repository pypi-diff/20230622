# Comparing `tmp/pinhook-1.9.6.tar.gz` & `tmp/pinhook-1.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinhook-1.9.6.tar", last modified: Fri Dec 18 16:47:04 2020, max compression
+gzip compressed data, was "pinhook-1.9.7.tar", last modified: Tue Dec 29 02:52:36 2020, max compression
```

## Comparing `pinhook-1.9.6.tar` & `pinhook-1.9.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-18 16:47:04.213005 pinhook-1.9.6/
--rw-r--r--   0 runner    (1001) docker     (116)       18 2020-12-18 16:46:51.000000 pinhook-1.9.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     9087 2020-12-18 16:47:04.213005 pinhook-1.9.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     6839 2020-12-18 16:46:51.000000 pinhook-1.9.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-18 16:47:04.213005 pinhook-1.9.6/pinhook/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-18 16:46:51.000000 pinhook-1.9.6/pinhook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)       22 2020-12-18 16:46:51.000000 pinhook-1.9.6/pinhook/__version__.py
--rw-r--r--   0 runner    (1001) docker     (116)    14558 2020-12-18 16:46:51.000000 pinhook-1.9.6/pinhook/bot.py
--rw-r--r--   0 runner    (1001) docker     (116)     2096 2020-12-18 16:46:51.000000 pinhook-1.9.6/pinhook/cli.py
--rw-r--r--   0 runner    (1001) docker     (116)      443 2020-12-18 16:46:51.000000 pinhook-1.9.6/pinhook/log.py
--rw-r--r--   0 runner    (1001) docker     (116)     4945 2020-12-18 16:46:51.000000 pinhook-1.9.6/pinhook/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-18 16:47:04.213005 pinhook-1.9.6/pinhook.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     9087 2020-12-18 16:47:04.000000 pinhook-1.9.6/pinhook.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      324 2020-12-18 16:47:04.000000 pinhook-1.9.6/pinhook.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-18 16:47:04.000000 pinhook-1.9.6/pinhook.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       45 2020-12-18 16:47:04.000000 pinhook-1.9.6/pinhook.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)       57 2020-12-18 16:47:04.000000 pinhook-1.9.6/pinhook.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        8 2020-12-18 16:47:04.000000 pinhook-1.9.6/pinhook.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-12-18 16:47:04.213005 pinhook-1.9.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (116)     3416 2020-12-18 16:46:51.000000 pinhook-1.9.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-29 02:52:36.277414 pinhook-1.9.7/
+-rw-r--r--   0 runner    (1001) docker     (116)       18 2020-12-29 02:52:23.000000 pinhook-1.9.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     9087 2020-12-29 02:52:36.277414 pinhook-1.9.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     6839 2020-12-29 02:52:23.000000 pinhook-1.9.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-29 02:52:36.277414 pinhook-1.9.7/pinhook/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-29 02:52:23.000000 pinhook-1.9.7/pinhook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)       22 2020-12-29 02:52:23.000000 pinhook-1.9.7/pinhook/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14578 2020-12-29 02:52:23.000000 pinhook-1.9.7/pinhook/bot.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2096 2020-12-29 02:52:23.000000 pinhook-1.9.7/pinhook/cli.py
+-rw-r--r--   0 runner    (1001) docker     (116)      443 2020-12-29 02:52:23.000000 pinhook-1.9.7/pinhook/log.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4945 2020-12-29 02:52:23.000000 pinhook-1.9.7/pinhook/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-29 02:52:36.277414 pinhook-1.9.7/pinhook.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     9087 2020-12-29 02:52:36.000000 pinhook-1.9.7/pinhook.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      324 2020-12-29 02:52:36.000000 pinhook-1.9.7/pinhook.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-29 02:52:36.000000 pinhook-1.9.7/pinhook.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       45 2020-12-29 02:52:36.000000 pinhook-1.9.7/pinhook.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       57 2020-12-29 02:52:36.000000 pinhook-1.9.7/pinhook.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        8 2020-12-29 02:52:36.000000 pinhook-1.9.7/pinhook.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2020-12-29 02:52:36.277414 pinhook-1.9.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (116)     3416 2020-12-29 02:52:23.000000 pinhook-1.9.7/setup.py
```

### Comparing `pinhook-1.9.6/PKG-INFO` & `pinhook-1.9.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinhook
-Version: 1.9.6
+Version: 1.9.7
 Summary: a pluggable irc bot framework in python
 Home-page: https://github.com/archangelic/pinhook
 Author: M. Hancock
 Author-email: mhancock@archangelic.space
 License: MIT
 Description: 
         # pinhook
```

### Comparing `pinhook-1.9.6/README.md` & `pinhook-1.9.7/README.md`

 * *Files identical despite different names*

### Comparing `pinhook-1.9.6/pinhook/bot.py` & `pinhook-1.9.7/pinhook/bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,17 +67,17 @@
             self.action = action
             self.privmsg = privmsg
             self.notice = notice
             self.msg_type = msg_type
             if cmd:
                 self.cmd = cmd
                 self.arg = arg
-            if text:
+            if text != None:
                 self.text = text
-            if not (cmd or text):
+            if not (cmd==None or text==None):
                 raise TypeError('missing cmd or text parameter')
 
     def start_logging(self):
         self.logger = log.logger
         if self.log_file:
             log.set_log_file(self.log_file)
         else:
```

### Comparing `pinhook-1.9.6/pinhook/cli.py` & `pinhook-1.9.7/pinhook/cli.py`

 * *Files identical despite different names*

### Comparing `pinhook-1.9.6/pinhook/plugin.py` & `pinhook-1.9.7/pinhook/plugin.py`

 * *Files identical despite different names*

### Comparing `pinhook-1.9.6/pinhook.egg-info/PKG-INFO` & `pinhook-1.9.7/pinhook.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinhook
-Version: 1.9.6
+Version: 1.9.7
 Summary: a pluggable irc bot framework in python
 Home-page: https://github.com/archangelic/pinhook
 Author: M. Hancock
 Author-email: mhancock@archangelic.space
 License: MIT
 Description: 
         # pinhook
```

### Comparing `pinhook-1.9.6/setup.py` & `pinhook-1.9.7/setup.py`

 * *Files identical despite different names*

