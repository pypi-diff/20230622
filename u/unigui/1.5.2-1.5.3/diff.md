# Comparing `tmp/unigui-1.5.2.tar.gz` & `tmp/unigui-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/unigui-1.5.2.tar", last modified: Mon Jun 12 23:33:15 2023, max compression
+gzip compressed data, was "dist/unigui-1.5.3.tar", last modified: Wed Jun 21 23:53:28 2023, max compression
```

## Comparing `unigui-1.5.2.tar` & `unigui-1.5.3.tar`

### file list

```diff
@@ -1,48 +1,47 @@
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-06-12 23:33:15.000000 unigui-1.5.2/
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-06-12 23:33:15.000000 unigui-1.5.2/unigui/
--rw-r--r--   0 george    (1000) george    (1000)    13618 2022-05-05 16:57:28.000000 unigui-1.5.2/unigui/manager.py
--rw-rw-r--   0 george    (1000) george    (1000)     9068 2023-06-12 23:28:53.000000 unigui-1.5.2/unigui/guielements.py
--rw-rw-r--   0 george    (1000) george    (1000)       43 2020-12-07 05:58:08.000000 unigui-1.5.2/unigui/userset.py
--rw-rw-r--   0 george    (1000) george    (1000)     3654 2023-06-11 14:56:41.000000 unigui-1.5.2/unigui/server.py
--rw-rw-r--   0 george    (1000) george    (1000)      132 2022-02-12 20:42:49.000000 unigui-1.5.2/unigui/__init__.py
--rw-r--r--   0 george    (1000) george    (1000)     2579 2021-11-25 07:29:21.000000 unigui-1.5.2/unigui/utils.py
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-06-12 23:33:15.000000 unigui-1.5.2/unigui/web/
--rw-rw-r--   0 george    (1000) george    (1000)    64483 2023-06-12 23:10:20.000000 unigui-1.5.2/unigui/web/favicon.ico
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-06-12 23:33:15.000000 unigui-1.5.2/unigui/web/css/
--rw-rw-r--   0 george    (1000) george    (1000)        0 2023-06-12 23:10:20.000000 unigui-1.5.2/unigui/web/css/app.31d6cfe0.css
--rw-rw-r--   0 george    (1000) george    (1000)   219590 2023-06-12 23:10:20.000000 unigui-1.5.2/unigui/web/css/vendor.49a52e8f.css
--rw-rw-r--   0 george    (1000) george    (1000)     3267 2023-06-12 23:10:20.000000 unigui-1.5.2/unigui/web/css/361.c9159919.css
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-06-12 23:33:15.000000 unigui-1.5.2/unigui/web/icons/
--rw-rw-r--   0 george    (1000) george    (1000)     9643 2023-06-12 23:10:20.000000 unigui-1.5.2/unigui/web/icons/favicon-96x96.png
--rw-rw-r--   0 george    (1000) george    (1000)      859 2023-06-12 23:10:20.000000 unigui-1.5.2/unigui/web/icons/favicon-16x16.png
--rw-rw-r--   0 george    (1000) george    (1000)     2039 2023-06-12 23:10:20.000000 unigui-1.5.2/unigui/web/icons/favicon-32x32.png
--rw-rw-r--   0 george    (1000) george    (1000)    12324 2023-06-12 23:10:20.000000 unigui-1.5.2/unigui/web/icons/favicon-128x128.png
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-06-12 23:33:15.000000 unigui-1.5.2/unigui/web/fonts/
--rw-rw-r--   0 george    (1000) george    (1000)   164912 2023-06-12 23:10:20.000000 unigui-1.5.2/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20344 2023-06-12 23:10:20.000000 unigui-1.5.2/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20416 2023-06-12 23:10:20.000000 unigui-1.5.2/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20408 2023-06-12 23:10:20.000000 unigui-1.5.2/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20424 2023-06-12 23:10:20.000000 unigui-1.5.2/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20544 2023-06-12 23:10:20.000000 unigui-1.5.2/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
--rw-rw-r--   0 george    (1000) george    (1000)   128360 2023-06-12 23:10:20.000000 unigui-1.5.2/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
--rw-rw-r--   0 george    (1000) george    (1000)    20436 2023-06-12 23:10:20.000000 unigui-1.5.2/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-06-12 23:33:15.000000 unigui-1.5.2/unigui/web/js/
--rw-rw-r--   0 george    (1000) george    (1000)    43129 2023-06-12 23:10:20.000000 unigui-1.5.2/unigui/web/js/361.78add75c.js
--rw-rw-r--   0 george    (1000) george    (1000)     6560 2023-06-12 23:10:20.000000 unigui-1.5.2/unigui/web/js/430.591e9a73.js
--rw-rw-r--   0 george    (1000) george    (1000)     5867 2023-06-12 23:10:20.000000 unigui-1.5.2/unigui/web/js/app.6ab35062.js
--rw-rw-r--   0 george    (1000) george    (1000)      763 2023-06-12 23:10:20.000000 unigui-1.5.2/unigui/web/js/193.283445be.js
--rw-rw-r--   0 george    (1000) george    (1000)  1431597 2023-06-12 23:10:20.000000 unigui-1.5.2/unigui/web/js/vendor.3e8714c2.js
--rw-rw-r--   0 george    (1000) george    (1000)      907 2023-06-12 23:10:20.000000 unigui-1.5.2/unigui/web/index.html
--rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.5.2/LICENSE
--rw-rw-r--   0 george    (1000) george    (1000)      585 2023-06-12 23:31:04.000000 unigui-1.5.2/setup.py
--rw-rw-r--   0 george    (1000) george    (1000)    19452 2023-06-12 23:33:15.000000 unigui-1.5.2/PKG-INFO
--rw-rw-r--   0 george    (1000) george    (1000)       38 2023-06-12 23:33:15.000000 unigui-1.5.2/setup.cfg
--rw-rw-r--   0 george    (1000) george    (1000)    19162 2023-05-24 11:05:25.000000 unigui-1.5.2/README.md
--rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.5.2/MANIFEST.in
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-06-12 23:33:15.000000 unigui-1.5.2/unigui.egg-info/
--rw-rw-r--   0 george    (1000) george    (1000)       30 2023-06-12 23:33:15.000000 unigui-1.5.2/unigui.egg-info/requires.txt
--rw-r--r--   0 george    (1000) george    (1000)        1 2023-06-12 23:33:15.000000 unigui-1.5.2/unigui.egg-info/dependency_links.txt
--rw-r--r--   0 george    (1000) george    (1000)    19452 2023-06-12 23:33:15.000000 unigui-1.5.2/unigui.egg-info/PKG-INFO
--rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.5.2/unigui.egg-info/not-zip-safe
--rw-r--r--   0 george    (1000) george    (1000)     1223 2023-06-12 23:33:15.000000 unigui-1.5.2/unigui.egg-info/SOURCES.txt
--rw-r--r--   0 george    (1000) george    (1000)        7 2023-06-12 23:33:15.000000 unigui-1.5.2/unigui.egg-info/top_level.txt
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-06-21 23:53:28.000000 unigui-1.5.3/
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-06-21 23:53:28.000000 unigui-1.5.3/unigui/
+-rw-r--r--   0 george    (1000) george    (1000)    13651 2023-06-21 23:43:02.000000 unigui-1.5.3/unigui/manager.py
+-rw-rw-r--   0 george    (1000) george    (1000)     9068 2023-06-12 23:28:53.000000 unigui-1.5.3/unigui/guielements.py
+-rw-rw-r--   0 george    (1000) george    (1000)     3654 2023-06-11 14:56:41.000000 unigui-1.5.3/unigui/server.py
+-rw-rw-r--   0 george    (1000) george    (1000)      102 2023-06-21 23:42:45.000000 unigui-1.5.3/unigui/__init__.py
+-rw-r--r--   0 george    (1000) george    (1000)     2579 2021-11-25 07:29:21.000000 unigui-1.5.3/unigui/utils.py
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-06-21 23:53:28.000000 unigui-1.5.3/unigui/web/
+-rw-rw-r--   0 george    (1000) george    (1000)    64483 2023-06-12 23:10:20.000000 unigui-1.5.3/unigui/web/favicon.ico
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-06-21 23:53:28.000000 unigui-1.5.3/unigui/web/css/
+-rw-rw-r--   0 george    (1000) george    (1000)        0 2023-06-12 23:10:20.000000 unigui-1.5.3/unigui/web/css/app.31d6cfe0.css
+-rw-rw-r--   0 george    (1000) george    (1000)   219590 2023-06-12 23:10:20.000000 unigui-1.5.3/unigui/web/css/vendor.49a52e8f.css
+-rw-rw-r--   0 george    (1000) george    (1000)     3267 2023-06-12 23:10:20.000000 unigui-1.5.3/unigui/web/css/361.c9159919.css
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-06-21 23:53:28.000000 unigui-1.5.3/unigui/web/icons/
+-rw-rw-r--   0 george    (1000) george    (1000)     9643 2023-06-12 23:10:20.000000 unigui-1.5.3/unigui/web/icons/favicon-96x96.png
+-rw-rw-r--   0 george    (1000) george    (1000)      859 2023-06-12 23:10:20.000000 unigui-1.5.3/unigui/web/icons/favicon-16x16.png
+-rw-rw-r--   0 george    (1000) george    (1000)     2039 2023-06-12 23:10:20.000000 unigui-1.5.3/unigui/web/icons/favicon-32x32.png
+-rw-rw-r--   0 george    (1000) george    (1000)    12324 2023-06-12 23:10:20.000000 unigui-1.5.3/unigui/web/icons/favicon-128x128.png
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-06-21 23:53:28.000000 unigui-1.5.3/unigui/web/fonts/
+-rw-rw-r--   0 george    (1000) george    (1000)   164912 2023-06-12 23:10:20.000000 unigui-1.5.3/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20344 2023-06-12 23:10:20.000000 unigui-1.5.3/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20416 2023-06-12 23:10:20.000000 unigui-1.5.3/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20408 2023-06-12 23:10:20.000000 unigui-1.5.3/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20424 2023-06-12 23:10:20.000000 unigui-1.5.3/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20544 2023-06-12 23:10:20.000000 unigui-1.5.3/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
+-rw-rw-r--   0 george    (1000) george    (1000)   128360 2023-06-12 23:10:20.000000 unigui-1.5.3/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
+-rw-rw-r--   0 george    (1000) george    (1000)    20436 2023-06-12 23:10:20.000000 unigui-1.5.3/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-06-21 23:53:28.000000 unigui-1.5.3/unigui/web/js/
+-rw-rw-r--   0 george    (1000) george    (1000)    43129 2023-06-12 23:10:20.000000 unigui-1.5.3/unigui/web/js/361.78add75c.js
+-rw-rw-r--   0 george    (1000) george    (1000)     6560 2023-06-12 23:10:20.000000 unigui-1.5.3/unigui/web/js/430.591e9a73.js
+-rw-rw-r--   0 george    (1000) george    (1000)     5867 2023-06-12 23:10:20.000000 unigui-1.5.3/unigui/web/js/app.6ab35062.js
+-rw-rw-r--   0 george    (1000) george    (1000)      763 2023-06-12 23:10:20.000000 unigui-1.5.3/unigui/web/js/193.283445be.js
+-rw-rw-r--   0 george    (1000) george    (1000)  1431597 2023-06-12 23:10:20.000000 unigui-1.5.3/unigui/web/js/vendor.3e8714c2.js
+-rw-rw-r--   0 george    (1000) george    (1000)      907 2023-06-12 23:10:20.000000 unigui-1.5.3/unigui/web/index.html
+-rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.5.3/LICENSE
+-rw-rw-r--   0 george    (1000) george    (1000)      600 2023-06-21 23:51:38.000000 unigui-1.5.3/setup.py
+-rw-rw-r--   0 george    (1000) george    (1000)    19442 2023-06-21 23:53:28.000000 unigui-1.5.3/PKG-INFO
+-rw-rw-r--   0 george    (1000) george    (1000)       38 2023-06-21 23:53:28.000000 unigui-1.5.3/setup.cfg
+-rw-rw-r--   0 george    (1000) george    (1000)    19137 2023-06-21 23:49:27.000000 unigui-1.5.3/README.md
+-rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.5.3/MANIFEST.in
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-06-21 23:53:28.000000 unigui-1.5.3/unigui.egg-info/
+-rw-rw-r--   0 george    (1000) george    (1000)       30 2023-06-21 23:53:28.000000 unigui-1.5.3/unigui.egg-info/requires.txt
+-rw-r--r--   0 george    (1000) george    (1000)        1 2023-06-21 23:53:28.000000 unigui-1.5.3/unigui.egg-info/dependency_links.txt
+-rw-r--r--   0 george    (1000) george    (1000)    19442 2023-06-21 23:53:28.000000 unigui-1.5.3/unigui.egg-info/PKG-INFO
+-rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.5.3/unigui.egg-info/not-zip-safe
+-rw-r--r--   0 george    (1000) george    (1000)     1205 2023-06-21 23:53:28.000000 unigui-1.5.3/unigui.egg-info/SOURCES.txt
+-rw-r--r--   0 george    (1000) george    (1000)        7 2023-06-21 23:53:28.000000 unigui-1.5.3/unigui.egg-info/top_level.txt
```

### Comparing `unigui-1.5.2/unigui/manager.py` & `unigui-1.5.3/unigui/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import importlib
 from .utils import *
 from . import utils
 import itertools
 import time
 from .guielements import *
 import sys
-from . import userset
 import asyncio
 import requests
 from threading import Thread
 
 users = {}
 
 sing2method = {'=':'changed', '->':'update','?':'complete','+':'append', '-':'delete', '!':'editing', '#':'modify'}    
@@ -153,16 +152,15 @@
             'prepare' : None,
             'dispatch' : None,
             'blocks' : [],
             'header' : utils.appname,            
             'save' : self.save_changes,
             'toolbar' : None
         }     
-
-        userset.user = self    
+         
         blocks_dir = 'blocks'        
         screens_dir =  'screens'
         modules = {}
         for file in os.listdir(screens_dir):
             if file.endswith(".py") and file != '__init__.py':
                 name = file[0:-3]
 
@@ -174,15 +172,16 @@
                 #else:
                 #    module, spec = modules[name]
                 
                 utils.clean_handlers()
                 spec.loader.exec_module(module)            
                 
                 screen = Screen(module.name)
-                module.screen = screen                
+                module.screen = screen 
+                module.user = self               
                 self.screens.append(module)
                 #set system vars
                 for var in screen_vars:                                            
                     setattr(screen, var, getattr(module,var,screen_vars[var])) 
                 screen.handlers__ = utils.handlers__
                 
                 if not screen.toolbar:
@@ -200,15 +199,16 @@
         self.menu = [[s.name,s.icon] for s in self.screens]        
 
         #remove user modules from sys for repeating loading for new users
         for file in os.listdir(blocks_dir):
             if file.endswith(".py") and file != '__init__.py':
                 name = f'{blocks_dir}.{file[0:-3]}'
                 if name in sys.modules:
-                    del sys.modules[name]       
+                    sys.modules[name].user = self
+                    del sys.modules[name]
                 
     @property
     def screen(self):        
         return  self.screen_module.screen 
 
     def set_screen(self,name):
         return self.process(['root', name])
```

### Comparing `unigui-1.5.2/unigui/guielements.py` & `unigui-1.5.3/unigui/guielements.py`

 * *Files identical despite different names*

### Comparing `unigui-1.5.2/unigui/server.py` & `unigui-1.5.3/unigui/server.py`

 * *Files identical despite different names*

### Comparing `unigui-1.5.2/unigui/utils.py` & `unigui-1.5.3/unigui/utils.py`

 * *Files identical despite different names*

### Comparing `unigui-1.5.2/unigui/web/favicon.ico` & `unigui-1.5.3/unigui/web/favicon.ico`

 * *Files identical despite different names*

### Comparing `unigui-1.5.2/unigui/web/css/vendor.49a52e8f.css` & `unigui-1.5.3/unigui/web/css/vendor.49a52e8f.css`

 * *Files identical despite different names*

### Comparing `unigui-1.5.2/unigui/web/css/361.c9159919.css` & `unigui-1.5.3/unigui/web/css/361.c9159919.css`

 * *Files identical despite different names*

### Comparing `unigui-1.5.2/unigui/web/icons/favicon-96x96.png` & `unigui-1.5.3/unigui/web/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `unigui-1.5.2/unigui/web/icons/favicon-16x16.png` & `unigui-1.5.3/unigui/web/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `unigui-1.5.2/unigui/web/icons/favicon-32x32.png` & `unigui-1.5.3/unigui/web/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `unigui-1.5.2/unigui/web/icons/favicon-128x128.png` & `unigui-1.5.3/unigui/web/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `unigui-1.5.2/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff` & `unigui-1.5.3/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.5.2/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff` & `unigui-1.5.3/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.5.2/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff` & `unigui-1.5.3/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.5.2/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff` & `unigui-1.5.3/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.5.2/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff` & `unigui-1.5.3/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.5.2/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff` & `unigui-1.5.3/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.5.2/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2` & `unigui-1.5.3/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2`

 * *Files identical despite different names*

### Comparing `unigui-1.5.2/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff` & `unigui-1.5.3/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.5.2/unigui/web/js/361.78add75c.js` & `unigui-1.5.3/unigui/web/js/361.78add75c.js`

 * *Files identical despite different names*

### Comparing `unigui-1.5.2/unigui/web/js/430.591e9a73.js` & `unigui-1.5.3/unigui/web/js/430.591e9a73.js`

 * *Files identical despite different names*

### Comparing `unigui-1.5.2/unigui/web/js/app.6ab35062.js` & `unigui-1.5.3/unigui/web/js/app.6ab35062.js`

 * *Files identical despite different names*

### Comparing `unigui-1.5.2/unigui/web/js/193.283445be.js` & `unigui-1.5.3/unigui/web/js/193.283445be.js`

 * *Files identical despite different names*

### Comparing `unigui-1.5.2/unigui/web/js/vendor.3e8714c2.js` & `unigui-1.5.3/unigui/web/js/vendor.3e8714c2.js`

 * *Files identical despite different names*

### Comparing `unigui-1.5.2/unigui/web/index.html` & `unigui-1.5.3/unigui/web/index.html`

 * *Files identical despite different names*

### Comparing `unigui-1.5.2/LICENSE` & `unigui-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `unigui-1.5.2/setup.py` & `unigui-1.5.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
  
 setup(name='unigui',
-      version='1.5.2',      
+      version='1.5.3',      
       license='MIT',
       author='Georgii Dernovyi',
       author_email='g.dernovoy@gmail.com',
-      description='Unigui - Universal app browser',
+      description='Unigui - Universal GUI Framework and protocol',
       packages=find_packages(exclude=['tests']),
       long_description=open('README.md').read(),
       long_description_content_type="text/markdown",
       url="https://github.com/Claus1/unigui" ,      
       include_package_data=True,
       install_requires=[
           'websockets','jsonpickle', 'aiohttp'
```

### Comparing `unigui-1.5.2/PKG-INFO` & `unigui-1.5.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.5.2
-Summary: Unigui - Universal app browser
+Version: 1.5.3
+Summary: Unigui - Universal GUI Framework and protocol
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # unigui #
-Universal GUI and App Browser
-    Python connector
+Universal GUI Framework and Protocol (Python)
 
 ### Purpose ###
 Provide a programming technology that does not require front-end programming, for a server written in any language, for displaying on any device, in any resolution, without any tuning. 
 
 ### Installing ###
 ```
 pip install unigui
@@ -35,16 +34,15 @@
 Screen example tests/screens/main.py
 ```
 name = "Main" #name of screen to show
 icon = 'blur_linear' #MD icon of screen to show
 order = 0 #order in the program menu
 blocks = [block] #what to show on the screen
 ```
-
-The block example with a table and 2 selectors
+The block example with a table and a selector
 ```
 table = Table('Videos', 0, headers = ['Video', 'Duration',  'Links', 'Mine'],rows = [
     ['opt_sync1_3_0.mp4', '30 seconds',  '@Refer to signal1', True],
     ['opt_sync1_3_0.mp4', '37 seconds',  '@Refer to signal8', False]    
 ])
 #widgets are groped in blocks (complex widgets with logic)
 block = Block('X Block',
@@ -62,15 +60,15 @@
 import unigui
 #app name, the others server setting in config.py like port, upload_dir, ..
 unigui.start('Test app') 
 ```
 Unigui builds the interactive app for the code above.
 Connect a browser to localhast:8000 which are by default and will see:
 
-![image](https://github.com/Claus1/unigui/assets/1247062/5afcf4ac-b388-4237-98ff-3a92e802d44a)
+![image](https://github.com/Claus1/unigui/assets/1247062/62caca12-86fc-4dcd-99b4-26845963b5cf)
 
 ### Handling events ###
 All handlers are functions which have a signature
 ```
 def handler_x(gui_object, value_x)
 ```
 where gui_object is a Python object the user interacted with and value for the event.
@@ -405,17 +403,16 @@
         if http_link(ref[1:]):
             open_inbrowser()
         else:
             return Warning(f'What to do with {ref}?') 
 
 unigui.start('Hello app', user_type = Hello_user)
 ```
-In screens and blocks sources we can access the user by call get_user()
+In screens and blocks sources we can access the user by 'user' variable
 ```
-user = get_user()
 print(isinstance(user, Hello_user))
 ```
 
 More info about User class methods you can find in manager.py in the souce dir.
 
 Examples are in tests folder.
```

### Comparing `unigui-1.5.2/README.md` & `unigui-1.5.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # unigui #
-Universal GUI and App Browser
-    Python connector
+Universal GUI Framework and Protocol (Python)
 
 ### Purpose ###
 Provide a programming technology that does not require front-end programming, for a server written in any language, for displaying on any device, in any resolution, without any tuning. 
 
 ### Installing ###
 ```
 pip install unigui
@@ -23,16 +22,15 @@
 Screen example tests/screens/main.py
 ```
 name = "Main" #name of screen to show
 icon = 'blur_linear' #MD icon of screen to show
 order = 0 #order in the program menu
 blocks = [block] #what to show on the screen
 ```
-
-The block example with a table and 2 selectors
+The block example with a table and a selector
 ```
 table = Table('Videos', 0, headers = ['Video', 'Duration',  'Links', 'Mine'],rows = [
     ['opt_sync1_3_0.mp4', '30 seconds',  '@Refer to signal1', True],
     ['opt_sync1_3_0.mp4', '37 seconds',  '@Refer to signal8', False]    
 ])
 #widgets are groped in blocks (complex widgets with logic)
 block = Block('X Block',
@@ -50,15 +48,15 @@
 import unigui
 #app name, the others server setting in config.py like port, upload_dir, ..
 unigui.start('Test app') 
 ```
 Unigui builds the interactive app for the code above.
 Connect a browser to localhast:8000 which are by default and will see:
 
-![image](https://github.com/Claus1/unigui/assets/1247062/5afcf4ac-b388-4237-98ff-3a92e802d44a)
+![image](https://github.com/Claus1/unigui/assets/1247062/62caca12-86fc-4dcd-99b4-26845963b5cf)
 
 ### Handling events ###
 All handlers are functions which have a signature
 ```
 def handler_x(gui_object, value_x)
 ```
 where gui_object is a Python object the user interacted with and value for the event.
@@ -393,16 +391,15 @@
         if http_link(ref[1:]):
             open_inbrowser()
         else:
             return Warning(f'What to do with {ref}?') 
 
 unigui.start('Hello app', user_type = Hello_user)
 ```
-In screens and blocks sources we can access the user by call get_user()
+In screens and blocks sources we can access the user by 'user' variable
 ```
-user = get_user()
 print(isinstance(user, Hello_user))
 ```
 
 More info about User class methods you can find in manager.py in the souce dir.
 
 Examples are in tests folder.
```

### Comparing `unigui-1.5.2/unigui.egg-info/PKG-INFO` & `unigui-1.5.3/unigui.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.5.2
-Summary: Unigui - Universal app browser
+Version: 1.5.3
+Summary: Unigui - Universal GUI Framework and protocol
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # unigui #
-Universal GUI and App Browser
-    Python connector
+Universal GUI Framework and Protocol (Python)
 
 ### Purpose ###
 Provide a programming technology that does not require front-end programming, for a server written in any language, for displaying on any device, in any resolution, without any tuning. 
 
 ### Installing ###
 ```
 pip install unigui
@@ -35,16 +34,15 @@
 Screen example tests/screens/main.py
 ```
 name = "Main" #name of screen to show
 icon = 'blur_linear' #MD icon of screen to show
 order = 0 #order in the program menu
 blocks = [block] #what to show on the screen
 ```
-
-The block example with a table and 2 selectors
+The block example with a table and a selector
 ```
 table = Table('Videos', 0, headers = ['Video', 'Duration',  'Links', 'Mine'],rows = [
     ['opt_sync1_3_0.mp4', '30 seconds',  '@Refer to signal1', True],
     ['opt_sync1_3_0.mp4', '37 seconds',  '@Refer to signal8', False]    
 ])
 #widgets are groped in blocks (complex widgets with logic)
 block = Block('X Block',
@@ -62,15 +60,15 @@
 import unigui
 #app name, the others server setting in config.py like port, upload_dir, ..
 unigui.start('Test app') 
 ```
 Unigui builds the interactive app for the code above.
 Connect a browser to localhast:8000 which are by default and will see:
 
-![image](https://github.com/Claus1/unigui/assets/1247062/5afcf4ac-b388-4237-98ff-3a92e802d44a)
+![image](https://github.com/Claus1/unigui/assets/1247062/62caca12-86fc-4dcd-99b4-26845963b5cf)
 
 ### Handling events ###
 All handlers are functions which have a signature
 ```
 def handler_x(gui_object, value_x)
 ```
 where gui_object is a Python object the user interacted with and value for the event.
@@ -405,17 +403,16 @@
         if http_link(ref[1:]):
             open_inbrowser()
         else:
             return Warning(f'What to do with {ref}?') 
 
 unigui.start('Hello app', user_type = Hello_user)
 ```
-In screens and blocks sources we can access the user by call get_user()
+In screens and blocks sources we can access the user by 'user' variable
 ```
-user = get_user()
 print(isinstance(user, Hello_user))
 ```
 
 More info about User class methods you can find in manager.py in the souce dir.
 
 Examples are in tests folder.
```

### Comparing `unigui-1.5.2/unigui.egg-info/SOURCES.txt` & `unigui-1.5.3/unigui.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 MANIFEST.in
 README.md
 setup.py
 unigui/__init__.py
 unigui/guielements.py
 unigui/manager.py
 unigui/server.py
-unigui/userset.py
 unigui/utils.py
 unigui.egg-info/PKG-INFO
 unigui.egg-info/SOURCES.txt
 unigui.egg-info/dependency_links.txt
 unigui.egg-info/not-zip-safe
 unigui.egg-info/requires.txt
 unigui.egg-info/top_level.txt
```

