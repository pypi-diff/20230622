# Comparing `tmp/bmw-lobster-tool-json-0.9.6.tar.gz` & `tmp/bmw-lobster-tool-json-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmw-lobster-tool-json-0.9.6.tar", last modified: Tue Jun 20 07:30:14 2023, max compression
+gzip compressed data, was "bmw-lobster-tool-json-0.9.7.tar", last modified: Thu Jun 22 14:54:05 2023, max compression
```

## Comparing `bmw-lobster-tool-json-0.9.6.tar` & `bmw-lobster-tool-json-0.9.7.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-20 07:30:14.720900 bmw-lobster-tool-json-0.9.6/
--rw-r--r--   0 florian   (1000) florian   (1000)     1818 2023-06-20 07:30:14.720900 bmw-lobster-tool-json-0.9.6/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)      890 2023-06-13 09:17:37.000000 bmw-lobster-tool-json-0.9.6/README.md
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-20 07:30:14.720900 bmw-lobster-tool-json-0.9.6/bmw_lobster_tool_json.egg-info/
--rw-r--r--   0 florian   (1000) florian   (1000)     1818 2023-06-20 07:30:14.000000 bmw-lobster-tool-json-0.9.6/bmw_lobster_tool_json.egg-info/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)      317 2023-06-20 07:30:14.000000 bmw-lobster-tool-json-0.9.6/bmw_lobster_tool_json.egg-info/SOURCES.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-06-20 07:30:14.000000 bmw-lobster-tool-json-0.9.6/bmw_lobster_tool_json.egg-info/dependency_links.txt
--rw-r--r--   0 florian   (1000) florian   (1000)       62 2023-06-20 07:30:14.000000 bmw-lobster-tool-json-0.9.6/bmw_lobster_tool_json.egg-info/entry_points.txt
--rw-r--r--   0 florian   (1000) florian   (1000)       24 2023-06-20 07:30:14.000000 bmw-lobster-tool-json-0.9.6/bmw_lobster_tool_json.egg-info/requires.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        8 2023-06-20 07:30:14.000000 bmw-lobster-tool-json-0.9.6/bmw_lobster_tool_json.egg-info/top_level.txt
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-20 07:30:14.720900 bmw-lobster-tool-json-0.9.6/lobster/
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-20 07:30:14.720900 bmw-lobster-tool-json-0.9.6/lobster/tools/
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-20 07:30:14.720900 bmw-lobster-tool-json-0.9.6/lobster/tools/json/
--rwxr-xr-x   0 florian   (1000) florian   (1000)     6914 2023-06-20 07:30:14.000000 bmw-lobster-tool-json-0.9.6/lobster/tools/json/json.py
--rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-06-20 07:30:14.720900 bmw-lobster-tool-json-0.9.6/setup.cfg
--rw-r--r--   0 florian   (1000) florian   (1000)     2234 2023-05-08 15:03:18.000000 bmw-lobster-tool-json-0.9.6/setup.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-22 14:54:05.341267 bmw-lobster-tool-json-0.9.7/
+-rw-r--r--   0 florian   (1000) florian   (1000)     1818 2023-06-22 14:54:05.341267 bmw-lobster-tool-json-0.9.7/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)      890 2023-06-13 09:17:37.000000 bmw-lobster-tool-json-0.9.7/README.md
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-22 14:54:05.341267 bmw-lobster-tool-json-0.9.7/bmw_lobster_tool_json.egg-info/
+-rw-r--r--   0 florian   (1000) florian   (1000)     1818 2023-06-22 14:54:05.000000 bmw-lobster-tool-json-0.9.7/bmw_lobster_tool_json.egg-info/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)      348 2023-06-22 14:54:05.000000 bmw-lobster-tool-json-0.9.7/bmw_lobster_tool_json.egg-info/SOURCES.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-06-22 14:54:05.000000 bmw-lobster-tool-json-0.9.7/bmw_lobster_tool_json.egg-info/dependency_links.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)       62 2023-06-22 14:54:05.000000 bmw-lobster-tool-json-0.9.7/bmw_lobster_tool_json.egg-info/entry_points.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)       24 2023-06-22 14:54:05.000000 bmw-lobster-tool-json-0.9.7/bmw_lobster_tool_json.egg-info/requires.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        8 2023-06-22 14:54:05.000000 bmw-lobster-tool-json-0.9.7/bmw_lobster_tool_json.egg-info/top_level.txt
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-22 14:54:05.341267 bmw-lobster-tool-json-0.9.7/lobster/
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-22 14:54:05.341267 bmw-lobster-tool-json-0.9.7/lobster/tools/
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-22 14:54:05.341267 bmw-lobster-tool-json-0.9.7/lobster/tools/json/
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-06-22 14:54:05.000000 bmw-lobster-tool-json-0.9.7/lobster/tools/json/__init__.py
+-rwxr-xr-x   0 florian   (1000) florian   (1000)     6914 2023-06-22 14:54:05.000000 bmw-lobster-tool-json-0.9.7/lobster/tools/json/json.py
+-rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-06-22 14:54:05.341267 bmw-lobster-tool-json-0.9.7/setup.cfg
+-rw-r--r--   0 florian   (1000) florian   (1000)     2234 2023-05-08 15:03:18.000000 bmw-lobster-tool-json-0.9.7/setup.py
```

### Comparing `bmw-lobster-tool-json-0.9.6/PKG-INFO` & `bmw-lobster-tool-json-0.9.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmw-lobster-tool-json
-Version: 0.9.6
+Version: 0.9.7
 Summary: LOBSTER Tool for JSON
 Home-page: https://github.com/bmw-software-engineering/lobster
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU Affero General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/lobster/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/lobster/
```

### Comparing `bmw-lobster-tool-json-0.9.6/README.md` & `bmw-lobster-tool-json-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `bmw-lobster-tool-json-0.9.6/bmw_lobster_tool_json.egg-info/PKG-INFO` & `bmw-lobster-tool-json-0.9.7/bmw_lobster_tool_json.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmw-lobster-tool-json
-Version: 0.9.6
+Version: 0.9.7
 Summary: LOBSTER Tool for JSON
 Home-page: https://github.com/bmw-software-engineering/lobster
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU Affero General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/lobster/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/lobster/
```

### Comparing `bmw-lobster-tool-json-0.9.6/lobster/tools/json/json.py` & `bmw-lobster-tool-json-0.9.7/lobster/tools/json/json.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-tool-json-0.9.6/setup.py` & `bmw-lobster-tool-json-0.9.7/setup.py`

 * *Files identical despite different names*

