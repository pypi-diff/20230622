# Comparing `tmp/bmw-lobster-tool-codebeamer-0.9.6.tar.gz` & `tmp/bmw-lobster-tool-codebeamer-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmw-lobster-tool-codebeamer-0.9.6.tar", last modified: Tue Jun 20 07:30:13 2023, max compression
+gzip compressed data, was "bmw-lobster-tool-codebeamer-0.9.7.tar", last modified: Thu Jun 22 14:54:04 2023, max compression
```

## Comparing `bmw-lobster-tool-codebeamer-0.9.6.tar` & `bmw-lobster-tool-codebeamer-0.9.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-20 07:30:13.836885 bmw-lobster-tool-codebeamer-0.9.6/
--rw-r--r--   0 florian   (1000) florian   (1000)     2181 2023-06-20 07:30:13.836885 bmw-lobster-tool-codebeamer-0.9.6/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)     1241 2023-06-14 14:03:10.000000 bmw-lobster-tool-codebeamer-0.9.6/README.md
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-20 07:30:13.836885 bmw-lobster-tool-codebeamer-0.9.6/bmw_lobster_tool_codebeamer.egg-info/
--rw-r--r--   0 florian   (1000) florian   (1000)     2181 2023-06-20 07:30:13.000000 bmw-lobster-tool-codebeamer-0.9.6/bmw_lobster_tool_codebeamer.egg-info/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)      402 2023-06-20 07:30:13.000000 bmw-lobster-tool-codebeamer-0.9.6/bmw_lobster_tool_codebeamer.egg-info/SOURCES.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-06-20 07:30:13.000000 bmw-lobster-tool-codebeamer-0.9.6/bmw_lobster_tool_codebeamer.egg-info/dependency_links.txt
--rw-r--r--   0 florian   (1000) florian   (1000)       80 2023-06-20 07:30:13.000000 bmw-lobster-tool-codebeamer-0.9.6/bmw_lobster_tool_codebeamer.egg-info/entry_points.txt
--rw-r--r--   0 florian   (1000) florian   (1000)       39 2023-06-20 07:30:13.000000 bmw-lobster-tool-codebeamer-0.9.6/bmw_lobster_tool_codebeamer.egg-info/requires.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        8 2023-06-20 07:30:13.000000 bmw-lobster-tool-codebeamer-0.9.6/bmw_lobster_tool_codebeamer.egg-info/top_level.txt
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-20 07:30:13.836885 bmw-lobster-tool-codebeamer-0.9.6/lobster/
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-20 07:30:13.836885 bmw-lobster-tool-codebeamer-0.9.6/lobster/tools/
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-20 07:30:13.836885 bmw-lobster-tool-codebeamer-0.9.6/lobster/tools/codebeamer/
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-06-20 07:30:13.000000 bmw-lobster-tool-codebeamer-0.9.6/lobster/tools/codebeamer/__init__.py
--rwxr-xr-x   0 florian   (1000) florian   (1000)     9763 2023-06-20 07:30:13.000000 bmw-lobster-tool-codebeamer-0.9.6/lobster/tools/codebeamer/codebeamer.py
--rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-06-20 07:30:13.836885 bmw-lobster-tool-codebeamer-0.9.6/setup.cfg
--rw-r--r--   0 florian   (1000) florian   (1000)     2296 2023-05-08 15:03:18.000000 bmw-lobster-tool-codebeamer-0.9.6/setup.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-22 14:54:04.441251 bmw-lobster-tool-codebeamer-0.9.7/
+-rw-r--r--   0 florian   (1000) florian   (1000)     2181 2023-06-22 14:54:04.441251 bmw-lobster-tool-codebeamer-0.9.7/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)     1241 2023-06-14 14:03:10.000000 bmw-lobster-tool-codebeamer-0.9.7/README.md
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-22 14:54:04.441251 bmw-lobster-tool-codebeamer-0.9.7/bmw_lobster_tool_codebeamer.egg-info/
+-rw-r--r--   0 florian   (1000) florian   (1000)     2181 2023-06-22 14:54:04.000000 bmw-lobster-tool-codebeamer-0.9.7/bmw_lobster_tool_codebeamer.egg-info/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)      402 2023-06-22 14:54:04.000000 bmw-lobster-tool-codebeamer-0.9.7/bmw_lobster_tool_codebeamer.egg-info/SOURCES.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-06-22 14:54:04.000000 bmw-lobster-tool-codebeamer-0.9.7/bmw_lobster_tool_codebeamer.egg-info/dependency_links.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)       80 2023-06-22 14:54:04.000000 bmw-lobster-tool-codebeamer-0.9.7/bmw_lobster_tool_codebeamer.egg-info/entry_points.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)       39 2023-06-22 14:54:04.000000 bmw-lobster-tool-codebeamer-0.9.7/bmw_lobster_tool_codebeamer.egg-info/requires.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        8 2023-06-22 14:54:04.000000 bmw-lobster-tool-codebeamer-0.9.7/bmw_lobster_tool_codebeamer.egg-info/top_level.txt
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-22 14:54:04.441251 bmw-lobster-tool-codebeamer-0.9.7/lobster/
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-22 14:54:04.441251 bmw-lobster-tool-codebeamer-0.9.7/lobster/tools/
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-22 14:54:04.441251 bmw-lobster-tool-codebeamer-0.9.7/lobster/tools/codebeamer/
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-06-22 14:54:04.000000 bmw-lobster-tool-codebeamer-0.9.7/lobster/tools/codebeamer/__init__.py
+-rwxr-xr-x   0 florian   (1000) florian   (1000)    10398 2023-06-22 14:54:04.000000 bmw-lobster-tool-codebeamer-0.9.7/lobster/tools/codebeamer/codebeamer.py
+-rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-06-22 14:54:04.441251 bmw-lobster-tool-codebeamer-0.9.7/setup.cfg
+-rw-r--r--   0 florian   (1000) florian   (1000)     2296 2023-05-08 15:03:18.000000 bmw-lobster-tool-codebeamer-0.9.7/setup.py
```

### Comparing `bmw-lobster-tool-codebeamer-0.9.6/PKG-INFO` & `bmw-lobster-tool-codebeamer-0.9.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmw-lobster-tool-codebeamer
-Version: 0.9.6
+Version: 0.9.7
 Summary: LOBSTER Tool for Codebeamer
 Home-page: https://github.com/bmw-software-engineering/lobster
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU Affero General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/lobster/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/lobster/
```

### Comparing `bmw-lobster-tool-codebeamer-0.9.6/README.md` & `bmw-lobster-tool-codebeamer-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `bmw-lobster-tool-codebeamer-0.9.6/bmw_lobster_tool_codebeamer.egg-info/PKG-INFO` & `bmw-lobster-tool-codebeamer-0.9.7/bmw_lobster_tool_codebeamer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmw-lobster-tool-codebeamer
-Version: 0.9.6
+Version: 0.9.7
 Summary: LOBSTER Tool for Codebeamer
 Home-page: https://github.com/bmw-software-engineering/lobster
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU Affero General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/lobster/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/lobster/
```

### Comparing `bmw-lobster-tool-codebeamer-0.9.6/lobster/tools/codebeamer/codebeamer.py` & `bmw-lobster-tool-codebeamer-0.9.7/lobster/tools/codebeamer/codebeamer.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 #
 # However you _can_ import all the items referenced from another
 # lobster artefact.
 
 import os
 import sys
 import argparse
+import netrc
 
 from copy import copy
 
 import requests
 
 from lobster.items import Tracing_Tag, Requirement
 from lobster.location import Codebeamer_Reference
@@ -208,15 +209,15 @@
 
     return rv
 
 
 def main():
     ap = argparse.ArgumentParser()
 
-    modes = ap.add_mutually_exclusive_group()
+    modes = ap.add_mutually_exclusive_group(required=True)
     modes.add_argument("--import-tagged",
                        metavar="LOBSTER_FILE",
                        default=None)
     modes.add_argument("--import-query",
                        metavar="CB_QUERY_ID",
                        default=None)
 
@@ -224,19 +225,40 @@
     ap.add_argument("--cb-user", default=os.environ.get("CB_USERNAME", None))
     ap.add_argument("--cb-pass", default=os.environ.get("CB_PASSWORD", None))
     ap.add_argument("--out", default=None)
     options = ap.parse_args()
 
     mh = Message_Handler()
 
-    if options.cb_root is None:
+    cb_config = {
+        "root" : options.cb_root,
+        "base" : "%s/cb/rest" % options.cb_root,
+        "user" : options.cb_user,
+        "pass" : options.cb_pass,
+    }
+
+    if cb_config["root"] is None:
         ap.error("please set CB_ROOT or use --cb-root")
-    if options.cb_user is None:
+
+    if not cb_config["root"].startswith("https://"):
+        ap.error("codebeamer root %s must start with https://")
+
+    if cb_config["user"] is None or cb_config["pass"] is None:
+        netrc_file = os.path.join(os.path.expanduser("~"),
+                                  ".netrc")
+        if os.path.isfile(netrc_file):
+            netrc_config = netrc.netrc()
+            auth = netrc_config.authenticators(cb_config["root"][8:])
+            if auth is not None:
+                print("using .netrc login for %s" % cb_config["root"])
+                cb_config["user"], _, cb_config["pass"] = auth
+
+    if cb_config["user"] is None:
         ap.error("please set CB_USERNAME or use --cb-user")
-    if options.cb_pass is None:
+    if cb_config["pass"] is None:
         ap.error("please set CB_PASSWORD or use --cb-pass")
 
     items_to_import = set()
 
     if options.import_tagged:
         if not os.path.isfile(options.import_tagged):
             ap.error("%s is not a file" % options.import_tagged)
@@ -267,21 +289,14 @@
         try:
             query_id = int(options.import_query)
         except ValueError:
             ap.error("query-id must be an integer")
         if query_id < 1:
             ap.error("query-id must be a positive")
 
-    cb_config = {
-        "root" : options.cb_root,
-        "base" : "%s/cb/rest" % options.cb_root,
-        "user" : options.cb_user,
-        "pass" : options.cb_pass,
-    }
-
     try:
         if options.import_tagged:
             items = import_tagged(mh, cb_config, items_to_import)
         elif options.import_query:
             items = get_query(mh, cb_config, query_id)
     except LOBSTER_Error:
         return 1
```

### Comparing `bmw-lobster-tool-codebeamer-0.9.6/setup.py` & `bmw-lobster-tool-codebeamer-0.9.7/setup.py`

 * *Files identical despite different names*

