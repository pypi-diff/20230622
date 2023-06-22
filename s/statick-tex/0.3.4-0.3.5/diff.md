# Comparing `tmp/statick-tex-0.3.4.tar.gz` & `tmp/statick-tex-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statick-tex-0.3.4.tar", last modified: Thu Jun 22 01:14:02 2023, max compression
+gzip compressed data, was "statick-tex-0.3.5.tar", last modified: Thu Jun 22 01:44:41 2023, max compression
```

## Comparing `statick-tex-0.3.4.tar` & `statick-tex-0.3.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:14:02.412473 statick-tex-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-06-22 01:13:57.000000 statick-tex-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-06-22 01:14:02.412473 statick-tex-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-06-22 01:13:57.000000 statick-tex-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:14:02.408473 statick-tex-0.3.4/rsc/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-22 01:13:57.000000 statick-tex-0.3.4/rsc/tex-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-22 01:13:57.000000 statick-tex-0.3.4/rsc/tex-profile.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 01:14:02.412473 statick-tex-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-22 01:13:57.000000 statick-tex-0.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:14:02.408473 statick-tex-0.3.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:14:02.408473 statick-tex-0.3.4/src/statick_tex/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:14:02.408473 statick-tex-0.3.4/src/statick_tex/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:14:02.412473 statick-tex-0.3.4/src/statick_tex/plugins/discovery/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-22 01:13:57.000000 statick-tex-0.3.4/src/statick_tex/plugins/discovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-06-22 01:13:57.000000 statick-tex-0.3.4/src/statick_tex/plugins/discovery/tex_discovery_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-22 01:13:57.000000 statick-tex-0.3.4/src/statick_tex/plugins/discovery/tex_discovery_plugin.yapsy-plugin
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:14:02.412473 statick-tex-0.3.4/src/statick_tex/plugins/tool/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-22 01:13:57.000000 statick-tex-0.3.4/src/statick_tex/plugins/tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-06-22 01:13:57.000000 statick-tex-0.3.4/src/statick_tex/plugins/tool/chktex_tool_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-22 01:13:57.000000 statick-tex-0.3.4/src/statick_tex/plugins/tool/chktex_tool_plugin.yapsy-plugin
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-06-22 01:13:57.000000 statick-tex-0.3.4/src/statick_tex/plugins/tool/lacheck_tool_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-22 01:13:57.000000 statick-tex-0.3.4/src/statick_tex/plugins/tool/lacheck_tool_plugin.yapsy-plugin
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:14:02.412473 statick-tex-0.3.4/statick_tex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-06-22 01:14:02.000000 statick-tex-0.3.4/statick_tex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-22 01:14:02.000000 statick-tex-0.3.4/statick_tex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 01:14:02.000000 statick-tex-0.3.4/statick_tex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-22 01:14:02.000000 statick-tex-0.3.4/statick_tex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-22 01:14:02.000000 statick-tex-0.3.4/statick_tex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:44:41.886996 statick-tex-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-06-22 01:44:37.000000 statick-tex-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-06-22 01:44:41.886996 statick-tex-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-06-22 01:44:37.000000 statick-tex-0.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:44:41.882996 statick-tex-0.3.5/rsc/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-22 01:44:37.000000 statick-tex-0.3.5/rsc/tex-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-22 01:44:37.000000 statick-tex-0.3.5/rsc/tex-profile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 01:44:41.886996 statick-tex-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-22 01:44:37.000000 statick-tex-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:44:41.882996 statick-tex-0.3.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:44:41.882996 statick-tex-0.3.5/src/statick_tex/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:44:41.882996 statick-tex-0.3.5/src/statick_tex/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:44:41.882996 statick-tex-0.3.5/src/statick_tex/plugins/discovery/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-22 01:44:37.000000 statick-tex-0.3.5/src/statick_tex/plugins/discovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-06-22 01:44:37.000000 statick-tex-0.3.5/src/statick_tex/plugins/discovery/tex_discovery_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-22 01:44:37.000000 statick-tex-0.3.5/src/statick_tex/plugins/discovery/tex_discovery_plugin.yapsy-plugin
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:44:41.886996 statick-tex-0.3.5/src/statick_tex/plugins/tool/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-22 01:44:37.000000 statick-tex-0.3.5/src/statick_tex/plugins/tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-06-22 01:44:37.000000 statick-tex-0.3.5/src/statick_tex/plugins/tool/chktex_tool_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-22 01:44:37.000000 statick-tex-0.3.5/src/statick_tex/plugins/tool/chktex_tool_plugin.yapsy-plugin
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-06-22 01:44:37.000000 statick-tex-0.3.5/src/statick_tex/plugins/tool/lacheck_tool_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-22 01:44:37.000000 statick-tex-0.3.5/src/statick_tex/plugins/tool/lacheck_tool_plugin.yapsy-plugin
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:44:41.886996 statick-tex-0.3.5/statick_tex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-06-22 01:44:41.000000 statick-tex-0.3.5/statick_tex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-22 01:44:41.000000 statick-tex-0.3.5/statick_tex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 01:44:41.000000 statick-tex-0.3.5/statick_tex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-22 01:44:41.000000 statick-tex-0.3.5/statick_tex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-22 01:44:41.000000 statick-tex-0.3.5/statick_tex.egg-info/top_level.txt
```

### Comparing `statick-tex-0.3.4/LICENSE` & `statick-tex-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `statick-tex-0.3.4/PKG-INFO` & `statick-tex-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statick-tex
-Version: 0.3.4
+Version: 0.3.5
 Summary: Statick analysis plugins for TeX/LaTeX files and projects.
 Home-page: https://github.com/tdenewiler/statick-tex
 Author: Thomas Denewiler
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `statick-tex-0.3.4/README.md` & `statick-tex-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `statick-tex-0.3.4/setup.py` & `statick-tex-0.3.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     "test": TEST_DEPS,
 }
 
 setup(
     author="Thomas Denewiler",
     name="statick-tex",
     description="Statick analysis plugins for TeX/LaTeX files and projects.",
-    version="0.3.4",
+    version="0.3.5",
     packages=[
         "statick_tool",
         "statick_tool.plugins.discovery",
         "statick_tool.plugins.tool",
     ],
     package_dir={
         "statick_tool": ".",
```

### Comparing `statick-tex-0.3.4/src/statick_tex/plugins/discovery/tex_discovery_plugin.py` & `statick-tex-0.3.5/src/statick_tex/plugins/discovery/tex_discovery_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-tex-0.3.4/src/statick_tex/plugins/tool/chktex_tool_plugin.py` & `statick-tex-0.3.5/src/statick_tex/plugins/tool/chktex_tool_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-tex-0.3.4/src/statick_tex/plugins/tool/lacheck_tool_plugin.py` & `statick-tex-0.3.5/src/statick_tex/plugins/tool/lacheck_tool_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-tex-0.3.4/statick_tex.egg-info/PKG-INFO` & `statick-tex-0.3.5/statick_tex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statick-tex
-Version: 0.3.4
+Version: 0.3.5
 Summary: Statick analysis plugins for TeX/LaTeX files and projects.
 Home-page: https://github.com/tdenewiler/statick-tex
 Author: Thomas Denewiler
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `statick-tex-0.3.4/statick_tex.egg-info/SOURCES.txt` & `statick-tex-0.3.5/statick_tex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

