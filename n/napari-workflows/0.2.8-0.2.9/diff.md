# Comparing `tmp/napari-workflows-0.2.8.tar.gz` & `tmp/napari-workflows-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-workflows-0.2.8.tar", last modified: Thu Nov 24 14:26:54 2022, max compression
+gzip compressed data, was "napari-workflows-0.2.9.tar", last modified: Thu Jun 22 14:27:05 2023, max compression
```

## Comparing `napari-workflows-0.2.8.tar` & `napari-workflows-0.2.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2022-11-24 14:26:54.556126 napari-workflows-0.2.8/
--rw-rw-rw-   0        0        0     1515 2022-11-24 12:06:47.000000 napari-workflows-0.2.8/LICENSE
--rw-rw-rw-   0        0        0      127 2022-11-24 12:06:47.000000 napari-workflows-0.2.8/MANIFEST.in
--rw-rw-rw-   0        0        0     5645 2022-11-24 14:26:54.556126 napari-workflows-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     4418 2022-11-24 12:06:47.000000 napari-workflows-0.2.8/README.md
--rw-rw-rw-   0        0        0      229 2022-11-24 12:06:47.000000 napari-workflows-0.2.8/requirements.txt
--rw-rw-rw-   0        0        0     1312 2022-11-24 14:26:54.557129 napari-workflows-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0       89 2022-11-24 12:06:47.000000 napari-workflows-0.2.8/setup.py
-drwxrwxrwx   0        0        0        0 2022-11-24 14:26:54.516501 napari-workflows-0.2.8/src/
-drwxrwxrwx   0        0        0        0 2022-11-24 14:26:54.539794 napari-workflows-0.2.8/src/napari_workflows/
--rw-rw-rw-   0        0        0      133 2022-11-24 14:25:39.000000 napari-workflows-0.2.8/src/napari_workflows/__init__.py
--rw-rw-rw-   0        0        0      932 2022-11-24 12:06:47.000000 napari-workflows-0.2.8/src/napari_workflows/_io_yaml_v1.py
-drwxrwxrwx   0        0        0        0 2022-11-24 14:26:54.555124 napari-workflows-0.2.8/src/napari_workflows/_tests/
--rw-rw-rw-   0        0        0        0 2022-11-24 12:06:47.000000 napari-workflows-0.2.8/src/napari_workflows/_tests/__init__.py
--rw-rw-rw-   0        0        0     6068 2022-11-24 12:06:47.000000 napari-workflows-0.2.8/src/napari_workflows/_tests/test_function.py
--rw-rw-rw-   0        0        0     4547 2022-11-24 12:06:47.000000 napari-workflows-0.2.8/src/napari_workflows/_undo_redo_functionality.py
--rw-rw-rw-   0        0        0    27724 2022-11-24 14:24:13.000000 napari-workflows-0.2.8/src/napari_workflows/_workflow.py
-drwxrwxrwx   0        0        0        0 2022-11-24 14:26:54.553119 napari-workflows-0.2.8/src/napari_workflows.egg-info/
--rw-rw-rw-   0        0        0     5645 2022-11-24 14:26:54.000000 napari-workflows-0.2.8/src/napari_workflows.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      521 2022-11-24 14:26:54.000000 napari-workflows-0.2.8/src/napari_workflows.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-24 14:26:54.000000 napari-workflows-0.2.8/src/napari_workflows.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2022-11-24 14:26:54.000000 napari-workflows-0.2.8/src/napari_workflows.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2022-11-24 14:26:54.000000 napari-workflows-0.2.8/src/napari_workflows.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-22 14:27:05.686961 napari-workflows-0.2.9/
+-rw-rw-rw-   0        0        0     1515 2022-11-24 12:06:47.000000 napari-workflows-0.2.9/LICENSE
+-rw-rw-rw-   0        0        0      127 2022-11-24 12:06:47.000000 napari-workflows-0.2.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     5645 2023-06-22 14:27:05.687963 napari-workflows-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4418 2022-11-24 12:06:47.000000 napari-workflows-0.2.9/README.md
+-rw-rw-rw-   0        0        0      229 2022-11-24 12:06:47.000000 napari-workflows-0.2.9/requirements.txt
+-rw-rw-rw-   0        0        0     1312 2023-06-22 14:27:05.699995 napari-workflows-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0       89 2022-11-24 12:06:47.000000 napari-workflows-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 14:27:05.587700 napari-workflows-0.2.9/src/
+drwxrwxrwx   0        0        0        0 2023-06-22 14:27:05.641842 napari-workflows-0.2.9/src/napari_workflows/
+-rw-rw-rw-   0        0        0      133 2023-06-22 14:26:08.000000 napari-workflows-0.2.9/src/napari_workflows/__init__.py
+-rw-rw-rw-   0        0        0      932 2022-11-24 12:06:47.000000 napari-workflows-0.2.9/src/napari_workflows/_io_yaml_v1.py
+drwxrwxrwx   0        0        0        0 2023-06-22 14:27:05.685958 napari-workflows-0.2.9/src/napari_workflows/_tests/
+-rw-rw-rw-   0        0        0        0 2022-11-24 12:06:47.000000 napari-workflows-0.2.9/src/napari_workflows/_tests/__init__.py
+-rw-rw-rw-   0        0        0     6056 2023-06-22 14:23:31.000000 napari-workflows-0.2.9/src/napari_workflows/_tests/test_function.py
+-rw-rw-rw-   0        0        0     4547 2022-11-24 12:06:47.000000 napari-workflows-0.2.9/src/napari_workflows/_undo_redo_functionality.py
+-rw-rw-rw-   0        0        0    27735 2023-06-22 14:23:31.000000 napari-workflows-0.2.9/src/napari_workflows/_workflow.py
+drwxrwxrwx   0        0        0        0 2023-06-22 14:27:05.681949 napari-workflows-0.2.9/src/napari_workflows.egg-info/
+-rw-rw-rw-   0        0        0     5645 2023-06-22 14:27:05.000000 napari-workflows-0.2.9/src/napari_workflows.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      521 2023-06-22 14:27:05.000000 napari-workflows-0.2.9/src/napari_workflows.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 14:27:05.000000 napari-workflows-0.2.9/src/napari_workflows.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-06-22 14:27:05.000000 napari-workflows-0.2.9/src/napari_workflows.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-22 14:27:05.000000 napari-workflows-0.2.9/src/napari_workflows.egg-info/top_level.txt
```

### Comparing `napari-workflows-0.2.8/LICENSE` & `napari-workflows-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-workflows-0.2.8/PKG-INFO` & `napari-workflows-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-workflows
-Version: 0.2.8
+Version: 0.2.9
 Summary: Data structures for managing image processing workflows in napari
 Home-page: https://github.com/haesleinhuepf/napari-workflows
 Author: Robert Haase, Ryan Savill
 Author-email: robert.haase@tu-dresden.de
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/haesleinhuepf/napari-workflows/issues
 Project-URL: Documentation, https://github.com/haesleinhuepf/napari-workflows#README.md
```

### Comparing `napari-workflows-0.2.8/README.md` & `napari-workflows-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `napari-workflows-0.2.8/setup.cfg` & `napari-workflows-0.2.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206e 6170 6172 692d 776f 726b 666c   = napari-workfl
 00000020: 6f77 730d 0a76 6572 7369 6f6e 203d 2030  ows..version = 0
-00000030: 2e32 2e38 0d0a 6175 7468 6f72 203d 2052  .2.8..author = R
+00000030: 2e32 2e39 0d0a 6175 7468 6f72 203d 2052  .2.9..author = R
 00000040: 6f62 6572 7420 4861 6173 652c 2052 7961  obert Haase, Rya
 00000050: 6e20 5361 7669 6c6c 0d0a 6175 7468 6f72  n Savill..author
 00000060: 5f65 6d61 696c 203d 2072 6f62 6572 742e  _email = robert.
 00000070: 6861 6173 6540 7475 2d64 7265 7364 656e  haase@tu-dresden
 00000080: 2e64 650d 0a75 726c 203d 2068 7474 7073  .de..url = https
 00000090: 3a2f 2f67 6974 6875 622e 636f 6d2f 6861  ://github.com/ha
 000000a0: 6573 6c65 696e 6875 6570 662f 6e61 7061  esleinhuepf/napa
```

### Comparing `napari-workflows-0.2.8/src/napari_workflows/_io_yaml_v1.py` & `napari-workflows-0.2.9/src/napari_workflows/_io_yaml_v1.py`

 * *Files identical despite different names*

### Comparing `napari-workflows-0.2.8/src/napari_workflows/_tests/test_function.py` & `napari-workflows-0.2.9/src/napari_workflows/_tests/test_function.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     from napari_workflows import WorkflowManager
     manager = WorkflowManager.install(viewer, _for_testing=True)
 
     from napari_tools_menu import make_gui
     gui = make_gui(segment, viewer, auto_call=True)
     viewer.window.add_dock_widget(gui)
     # invoke execution / workflow update
-    gui.sigma.value = gui.sigma.value
+    gui.sigma.value = 5.1
 
     workflow = manager.workflow
 
     print(workflow)
     print(viewer.layers)
 
     test_key_root = image_layer.name
@@ -95,15 +95,15 @@
     manager.update(list(viewer.layers)[1], segment, "Image", 2)
     undo_state_check = copy_workflow_state(manager.workflow)
     manager._update_invalid_layer()
 
     # test code generation
     code = manager.to_python_code()
     print(code)
-    assert len(code.split("\n")) == 19
+    assert len(code.split("\n")) == 16
 
     # test event handling
     image_layer.data = image
     class FakeEvent():
         def __init__(self, value):
             self.value = value
     manager._slider_updated(FakeEvent(viewer.dims.current_step))
```

### Comparing `napari-workflows-0.2.8/src/napari_workflows/_undo_redo_functionality.py` & `napari-workflows-0.2.9/src/napari_workflows/_undo_redo_functionality.py`

 * *Files identical despite different names*

### Comparing `napari-workflows-0.2.8/src/napari_workflows/_workflow.py` & `napari-workflows-0.2.9/src/napari_workflows/_workflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -496,15 +496,15 @@
         if isinstance(value, str):
             if value not in image_variable_names:
                 # Make a short and readable variable name, e.g. turn a layer
                 # "Resut of Gaussian blur" into "image1_gb".
                 temp = value
                 temp = temp.replace("Result of ", "")
                 temp = temp.replace(" result", "")
-                temp = "".join([t[0] for t in temp.split("_")])
+                temp = "".join([t[0] for t in temp.split("_") if t != ""])
                 new_name = "image" + str(len(image_variable_names)) + "_" + temp
                 image_variable_names[value] = new_name
 
             return image_variable_names[value]
         else:
             return str(value)
```

### Comparing `napari-workflows-0.2.8/src/napari_workflows.egg-info/PKG-INFO` & `napari-workflows-0.2.9/src/napari_workflows.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-workflows
-Version: 0.2.8
+Version: 0.2.9
 Summary: Data structures for managing image processing workflows in napari
 Home-page: https://github.com/haesleinhuepf/napari-workflows
 Author: Robert Haase, Ryan Savill
 Author-email: robert.haase@tu-dresden.de
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/haesleinhuepf/napari-workflows/issues
 Project-URL: Documentation, https://github.com/haesleinhuepf/napari-workflows#README.md
```

### Comparing `napari-workflows-0.2.8/src/napari_workflows.egg-info/SOURCES.txt` & `napari-workflows-0.2.9/src/napari_workflows.egg-info/SOURCES.txt`

 * *Files identical despite different names*

