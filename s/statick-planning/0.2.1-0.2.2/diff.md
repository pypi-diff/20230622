# Comparing `tmp/statick-planning-0.2.1.tar.gz` & `tmp/statick-planning-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statick-planning-0.2.1.tar", last modified: Mon Oct 10 20:53:52 2022, max compression
+gzip compressed data, was "statick-planning-0.2.2.tar", last modified: Thu Jun 22 03:02:58 2023, max compression
```

## Comparing `statick-planning-0.2.1.tar` & `statick-planning-0.2.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-10 20:53:52.328226 statick-planning-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (116)     6401 2022-10-10 20:53:48.000000 statick-planning-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     5903 2022-10-10 20:53:52.328226 statick-planning-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     5292 2022-10-10 20:53:48.000000 statick-planning-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-10 20:53:52.324226 statick-planning-0.2.1/rsc/
--rw-r--r--   0 runner    (1001) docker     (116)      172 2022-10-10 20:53:48.000000 statick-planning-0.2.1/rsc/planning-config.yaml
--rw-r--r--   0 runner    (1001) docker     (116)       18 2022-10-10 20:53:48.000000 statick-planning-0.2.1/rsc/planning-profile.yaml
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-10-10 20:53:52.328226 statick-planning-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1517 2022-10-10 20:53:48.000000 statick-planning-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-10 20:53:52.324226 statick-planning-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-10 20:53:52.324226 statick-planning-0.2.1/src/statick_planning/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-10 20:53:52.324226 statick-planning-0.2.1/src/statick_planning/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-10 20:53:52.324226 statick-planning-0.2.1/src/statick_planning/plugins/discovery/
--rw-r--r--   0 runner    (1001) docker     (116)       34 2022-10-10 20:53:48.000000 statick-planning-0.2.1/src/statick_planning/plugins/discovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2042 2022-10-10 20:53:48.000000 statick-planning-0.2.1/src/statick_planning/plugins/discovery/pddl_discovery_plugin.py
--rw-r--r--   0 runner    (1001) docker     (116)       67 2022-10-10 20:53:48.000000 statick-planning-0.2.1/src/statick_planning/plugins/discovery/pddl_discovery_plugin.yapsy-plugin
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-10 20:53:52.324226 statick-planning-0.2.1/src/statick_planning/plugins/tool/
--rw-r--r--   0 runner    (1001) docker     (116)       29 2022-10-10 20:53:48.000000 statick-planning-0.2.1/src/statick_planning/plugins/tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3990 2022-10-10 20:53:48.000000 statick-planning-0.2.1/src/statick_planning/plugins/tool/val_parser_tool_plugin.py
--rw-r--r--   0 runner    (1001) docker     (116)       69 2022-10-10 20:53:48.000000 statick-planning-0.2.1/src/statick_planning/plugins/tool/val_parser_tool_plugin.yapsy-plugin
--rw-r--r--   0 runner    (1001) docker     (116)     3803 2022-10-10 20:53:48.000000 statick-planning-0.2.1/src/statick_planning/plugins/tool/val_validate_tool_plugin.py
--rw-r--r--   0 runner    (1001) docker     (116)       73 2022-10-10 20:53:48.000000 statick-planning-0.2.1/src/statick_planning/plugins/tool/val_validate_tool_plugin.yapsy-plugin
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-10 20:53:52.328226 statick-planning-0.2.1/statick_planning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     5903 2022-10-10 20:53:52.000000 statick-planning-0.2.1/statick_planning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      779 2022-10-10 20:53:52.000000 statick-planning-0.2.1/statick_planning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-10-10 20:53:52.000000 statick-planning-0.2.1/statick_planning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       39 2022-10-10 20:53:52.000000 statick-planning-0.2.1/statick_planning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       13 2022-10-10 20:53:52.000000 statick-planning-0.2.1/statick_planning.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:02:58.614670 statick-planning-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-06-22 03:02:54.000000 statick-planning-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-06-22 03:02:58.614670 statick-planning-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-06-22 03:02:54.000000 statick-planning-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:02:58.610670 statick-planning-0.2.2/rsc/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-22 03:02:54.000000 statick-planning-0.2.2/rsc/planning-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-22 03:02:54.000000 statick-planning-0.2.2/rsc/planning-profile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 03:02:58.614670 statick-planning-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-22 03:02:54.000000 statick-planning-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:02:58.610670 statick-planning-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:02:58.610670 statick-planning-0.2.2/src/statick_planning/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:02:58.610670 statick-planning-0.2.2/src/statick_planning/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:02:58.610670 statick-planning-0.2.2/src/statick_planning/plugins/discovery/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-22 03:02:54.000000 statick-planning-0.2.2/src/statick_planning/plugins/discovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-22 03:02:54.000000 statick-planning-0.2.2/src/statick_planning/plugins/discovery/pddl_discovery_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-22 03:02:54.000000 statick-planning-0.2.2/src/statick_planning/plugins/discovery/pddl_discovery_plugin.yapsy-plugin
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:02:58.610670 statick-planning-0.2.2/src/statick_planning/plugins/tool/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-22 03:02:54.000000 statick-planning-0.2.2/src/statick_planning/plugins/tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-06-22 03:02:54.000000 statick-planning-0.2.2/src/statick_planning/plugins/tool/val_parser_tool_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-22 03:02:54.000000 statick-planning-0.2.2/src/statick_planning/plugins/tool/val_parser_tool_plugin.yapsy-plugin
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-06-22 03:02:54.000000 statick-planning-0.2.2/src/statick_planning/plugins/tool/val_validate_tool_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-22 03:02:54.000000 statick-planning-0.2.2/src/statick_planning/plugins/tool/val_validate_tool_plugin.yapsy-plugin
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:02:58.614670 statick-planning-0.2.2/statick_planning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-06-22 03:02:58.000000 statick-planning-0.2.2/statick_planning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-22 03:02:58.000000 statick-planning-0.2.2/statick_planning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 03:02:58.000000 statick-planning-0.2.2/statick_planning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-22 03:02:58.000000 statick-planning-0.2.2/statick_planning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-22 03:02:58.000000 statick-planning-0.2.2/statick_planning.egg-info/top_level.txt
```

### Comparing `statick-planning-0.2.1/LICENSE` & `statick-planning-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `statick-planning-0.2.1/PKG-INFO` & `statick-planning-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: statick-planning
-Version: 0.2.1
+Version: 0.2.2
 Summary: Statick analysis plugins for planning files.
 Home-page: https://github.com/tdenewiler/statick-planning
 Author: Thomas Denewiler
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Testing
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # Statick Planning Plugins
```

### Comparing `statick-planning-0.2.1/README.md` & `statick-planning-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `statick-planning-0.2.1/setup.py` & `statick-planning-0.2.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     "test": TEST_DEPS,
 }
 
 setup(
     author="Thomas Denewiler",
     name="statick-planning",
     description="Statick analysis plugins for planning files.",
-    version="0.2.1",
+    version="0.2.2",
     packages=[
         "statick_tool",
         "statick_tool.plugins.discovery",
         "statick_tool.plugins.tool",
     ],
     package_dir={
         "statick_tool.plugins.discovery": "src/statick_planning/plugins/discovery",
@@ -40,14 +40,14 @@
     long_description_content_type="text/markdown",
     install_requires=["statick"],
     tests_require=TEST_DEPS,
     extras_require=EXTRAS,
     url="https://github.com/tdenewiler/statick-planning",
     classifiers=[
         "License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Software Development :: Testing",
     ],
 )
```

### Comparing `statick-planning-0.2.1/src/statick_planning/plugins/discovery/pddl_discovery_plugin.py` & `statick-planning-0.2.2/src/statick_planning/plugins/discovery/pddl_discovery_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-planning-0.2.1/src/statick_planning/plugins/tool/val_parser_tool_plugin.py` & `statick-planning-0.2.2/src/statick_planning/plugins/tool/val_parser_tool_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-planning-0.2.1/src/statick_planning/plugins/tool/val_validate_tool_plugin.py` & `statick-planning-0.2.2/src/statick_planning/plugins/tool/val_validate_tool_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-planning-0.2.1/statick_planning.egg-info/PKG-INFO` & `statick-planning-0.2.2/statick_planning.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: statick-planning
-Version: 0.2.1
+Version: 0.2.2
 Summary: Statick analysis plugins for planning files.
 Home-page: https://github.com/tdenewiler/statick-planning
 Author: Thomas Denewiler
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Testing
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # Statick Planning Plugins
```

### Comparing `statick-planning-0.2.1/statick_planning.egg-info/SOURCES.txt` & `statick-planning-0.2.2/statick_planning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

