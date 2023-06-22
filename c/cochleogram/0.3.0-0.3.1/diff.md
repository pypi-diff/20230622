# Comparing `tmp/cochleogram-0.3.0.tar.gz` & `tmp/cochleogram-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cochleogram-0.3.0.tar", last modified: Wed May 17 22:04:44 2023, max compression
+gzip compressed data, was "cochleogram-0.3.1.tar", last modified: Thu Jun 22 19:50:03 2023, max compression
```

## Comparing `cochleogram-0.3.0.tar` & `cochleogram-0.3.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:04:44.484983 cochleogram-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:04:44.480983 cochleogram-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:04:44.480983 cochleogram-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-17 22:04:31.000000 cochleogram-0.3.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-17 22:04:31.000000 cochleogram-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-05-17 22:04:44.484983 cochleogram-0.3.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:04:44.480983 cochleogram-0.3.0/cochleogram/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:04:31.000000 cochleogram-0.3.0/cochleogram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23363 2023-05-17 22:04:31.000000 cochleogram-0.3.0/cochleogram/gui.enaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:04:44.484983 cochleogram-0.3.0/cochleogram/icons/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:04:31.000000 cochleogram-0.3.0/cochleogram/icons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-17 22:04:31.000000 cochleogram-0.3.0/cochleogram/icons/cells.png
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-17 22:04:31.000000 cochleogram-0.3.0/cochleogram/icons/exclude.png
--rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-05-17 22:04:31.000000 cochleogram-0.3.0/cochleogram/icons/main-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-05-17 22:04:31.000000 cochleogram-0.3.0/cochleogram/icons/make_icons.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-05-17 22:04:31.000000 cochleogram-0.3.0/cochleogram/icons/spiral.png
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-17 22:04:31.000000 cochleogram-0.3.0/cochleogram/icons/tile.png
--rw-r--r--   0 runner    (1001) docker     (123)    23257 2023-05-17 22:04:31.000000 cochleogram-0.3.0/cochleogram/instructions.html
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-05-17 22:04:31.000000 cochleogram-0.3.0/cochleogram/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    23013 2023-05-17 22:04:31.000000 cochleogram-0.3.0/cochleogram/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-05-17 22:04:31.000000 cochleogram-0.3.0/cochleogram/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    27793 2023-05-17 22:04:31.000000 cochleogram-0.3.0/cochleogram/presenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-05-17 22:04:31.000000 cochleogram-0.3.0/cochleogram/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14237 2023-05-17 22:04:31.000000 cochleogram-0.3.0/cochleogram/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-17 22:04:44.000000 cochleogram-0.3.0/cochleogram/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:04:44.484983 cochleogram-0.3.0/cochleogram.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-05-17 22:04:44.000000 cochleogram-0.3.0/cochleogram.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-17 22:04:44.000000 cochleogram-0.3.0/cochleogram.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 22:04:44.000000 cochleogram-0.3.0/cochleogram.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-17 22:04:44.000000 cochleogram-0.3.0/cochleogram.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-17 22:04:44.000000 cochleogram-0.3.0/cochleogram.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-17 22:04:44.000000 cochleogram-0.3.0/cochleogram.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-17 22:04:31.000000 cochleogram-0.3.0/development.rst
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-17 22:04:31.000000 cochleogram-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-05-17 22:04:31.000000 cochleogram-0.3.0/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 22:04:44.484983 cochleogram-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:50:03.889881 cochleogram-0.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:50:03.885881 cochleogram-0.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:50:03.885881 cochleogram-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-22 19:49:52.000000 cochleogram-0.3.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-06-22 19:49:52.000000 cochleogram-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-06-22 19:50:03.889881 cochleogram-0.3.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:50:03.889881 cochleogram-0.3.1/cochleogram/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 19:49:52.000000 cochleogram-0.3.1/cochleogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23682 2023-06-22 19:49:52.000000 cochleogram-0.3.1/cochleogram/gui.enaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:50:03.889881 cochleogram-0.3.1/cochleogram/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 19:49:52.000000 cochleogram-0.3.1/cochleogram/icons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-22 19:49:52.000000 cochleogram-0.3.1/cochleogram/icons/cells.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-22 19:49:52.000000 cochleogram-0.3.1/cochleogram/icons/exclude.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-06-22 19:49:52.000000 cochleogram-0.3.1/cochleogram/icons/main-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-06-22 19:49:52.000000 cochleogram-0.3.1/cochleogram/icons/make_icons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-06-22 19:49:52.000000 cochleogram-0.3.1/cochleogram/icons/spiral.png
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-22 19:49:52.000000 cochleogram-0.3.1/cochleogram/icons/tile.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23257 2023-06-22 19:49:52.000000 cochleogram-0.3.1/cochleogram/instructions.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-06-22 19:49:52.000000 cochleogram-0.3.1/cochleogram/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23013 2023-06-22 19:49:52.000000 cochleogram-0.3.1/cochleogram/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-06-22 19:49:52.000000 cochleogram-0.3.1/cochleogram/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28052 2023-06-22 19:49:52.000000 cochleogram-0.3.1/cochleogram/presenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-06-22 19:49:52.000000 cochleogram-0.3.1/cochleogram/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14237 2023-06-22 19:49:52.000000 cochleogram-0.3.1/cochleogram/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-22 19:50:03.000000 cochleogram-0.3.1/cochleogram/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:50:03.889881 cochleogram-0.3.1/cochleogram.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-06-22 19:50:03.000000 cochleogram-0.3.1/cochleogram.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-22 19:50:03.000000 cochleogram-0.3.1/cochleogram.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 19:50:03.000000 cochleogram-0.3.1/cochleogram.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-22 19:50:03.000000 cochleogram-0.3.1/cochleogram.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-22 19:50:03.000000 cochleogram-0.3.1/cochleogram.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-22 19:50:03.000000 cochleogram-0.3.1/cochleogram.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-22 19:49:52.000000 cochleogram-0.3.1/development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-22 19:49:52.000000 cochleogram-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-06-22 19:49:52.000000 cochleogram-0.3.1/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 19:50:03.889881 cochleogram-0.3.1/setup.cfg
```

### Comparing `cochleogram-0.3.0/.github/workflows/publish-to-pypi.yml` & `cochleogram-0.3.1/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `cochleogram-0.3.0/.gitignore` & `cochleogram-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `cochleogram-0.3.0/PKG-INFO` & `cochleogram-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cochleogram
-Version: 0.3.0
+Version: 0.3.1
 Summary: Module for creating cochleograms from confocal images
 Author-email: Brad Buran <buran@ohsu.edu>
 Maintainer-email: Brad Buran <buran@ohsu.edu>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: czi
 Provides-Extra: lif
```

### Comparing `cochleogram-0.3.0/cochleogram/gui.enaml` & `cochleogram-0.3.1/cochleogram/gui.enaml`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 from enaml.stdlib.fields import FloatField
 from enaml.stdlib.message_box import critical, information, question
 from enaml.qt.QtCore import Qt
 from enaml.widgets.api import (Action, ButtonGroup, CheckBox, Container,
                                DockArea, DockItem, DualSlider, Feature,
                                FileDialogEx, Form, HGroup, Html, Label,
                                MainWindow, Menu, MenuBar, MPLCanvas,
-                               ObjectCombo, ProgressBar, PushButton, Slider,
-                               VGroup, Window)
+                               ObjectCombo, PopupView, ProgressBar, PushButton,
+                               Slider, VGroup, Window)
 
 from cochleogram import plot, util
 from cochleogram.model import Cochlea
 from cochleogram.presenter import Presenter
 from cochleogram import readers
 
 
@@ -44,28 +44,28 @@
     # Check for unsaved changes
     if any(p.unsaved_changes for p in window.presenters):
         q = 'There are unsaved changes. Your current analysis will be lost. Are you sure?'
         button = question(None, 'Confirm action', q)
         if button is None or button.text == 'No':
             return
 
-    path = FileDialogEx.get_existing_directory(window, current_path=window.current_path)
+    path = FileDialogEx.get_existing_directory(window, current_path=str(window.current_path))
     if path:
         load_dataset(path, window, readers.ProcessedReader)
 
 
 def open_20x_lif_file(window):
     # Check for unsaved changes
     if any(p.unsaved_changes for p in window.presenters):
         q = 'There are unsaved changes. Your current analysis will be lost. Are you sure?'
         button = question(None, 'Confirm action', q)
         if button is None or button.text == 'No':
             return
 
-    path = FileDialogEx.get_open_file_name(window, current_path=window.current_path)
+    path = FileDialogEx.get_open_file_name(window, current_path=str(window.current_path))
     if path:
         load_dataset(path, window, readers.LIFReader)
 
 
 def load_dataset(path, window, reader_class=None):
     path = Path(path)
     if reader_class is None:
@@ -149,41 +149,78 @@
         for o in observe:
             if hasattr(item, o):
                 item.observe(o, cb)
         if getattr(item, 'children', []):
             bind_focus(item.children, cb)
 
 
-enamldef MPLDockItem(DockItem):
+enamldef ChannelConfigPopup(PopupView):
+    attr presenter
+    attr display_apply
+
+    anchor = (0.5, 0.0)
+    parent_anchor = (0.5, 1.0)
+    arrow_size = 20
+
+    Container:
+        layout_constraints => ():
+            widgets = self.visible_widgets()
+            cb = widgets[::2]
+            slider = widgets[1::2]
+            constraints = [vbox(*[hbox(c, s) for c, s in zip(cb, slider)])]
+            constraints.append(align('left', *slider))
+            constraints.append(align('left', *cb))
+            return constraints
+
+        Looper:
+            iterable << presenter.current_artist.channel_config.items() \
+                if presenter.current_artist is not None else {}
+
+            CheckBox:
+                text = loop_item[0]
+                checked << loop_item[1].visible
+                checked ::
+                    presenter.set_channel_visible(loop_item[0], checked, display_apply)
+            DualSlider:
+                minimum = 0
+                maximum = 100
+                low_value << int(loop_item[1].min_value * 100)
+                high_value << int(loop_item[1].max_value * 100)
+                low_value ::
+                    presenter.set_channel_min_value(loop_item[0], low_value / 100, display_apply)
+                high_value ::
+                    presenter.set_channel_max_value(loop_item[0], high_value / 100, display_apply)
+
+
+enamldef MPLDockItem(DockItem): dock_item:
 
     attr presenter
     closable = False
 
     title << 'Piece {}{}'.format(presenter.piece.piece, '*' if presenter.unsaved_changes else '')
 
     initialized ::
         bind_focus(container.children, canvas.set_focus)
         deferred_call(canvas.set_focus)
 
     Container: container:
         constraints = [
             vbox(
-                channel_config,
-                hbox(display_label, display_as_label,
-                     display_mode, z_slice_number_label, z_slice,
-                     display_apply, highlight_selected),
+                hbox(display_label, channels, display_as_label, display_mode,
+                     z_slice_number_label, z_slice, display_apply,
+                     highlight_selected),
                 hbox(tool_label, mode_buttons, spacer, load_analysis, save_analysis),
                 hbox(action_label, action_clear_spiral, action_clear_cells,
                      action_simplify_exclusions, action_merge_ohc_exclusions,
                      spacer, spacing=0),
                 action_guess_cells,
                 action_copy_exclusion,
                 canvas,
             ),
-            align('v_center', display_label, display_as_label,
+            align('v_center', display_label, channels, display_as_label,
                   display_mode, z_slice_number_label, z_slice, display_apply,
                   highlight_selected),
             align('v_center', tool_label, mode_buttons),
             align('v_center', action_label, action_clear_spiral,
                   action_clear_cells, action_simplify_exclusions,
                   action_merge_ohc_exclusions),
             align('left', display_label, tool_label, action_label),
@@ -192,42 +229,20 @@
             guess_width.width == 50,
             guess_spacing.width == 50,
         ]
 
         Label: display_label:
             text = 'Display'
 
-        Container: channel_config:
-            layout_constraints => ():
-                widgets = self.visible_widgets()
-                cb = widgets[::2]
-                slider = widgets[1::2]
-                constraints = [vbox(*[hbox(c, s) for c, s in zip(cb, slider)])]
-                constraints.append(align('left', *slider))
-                constraints.append(align('left', *cb))
-                return constraints
-
-            Looper:
-                iterable << presenter.current_artist.channel_config.items() \
-                    if presenter.current_artist is not None else {}
-
-                CheckBox:
-                    text = loop_item[0]
-                    checked << loop_item[1].visible
-                    checked ::
-                        presenter.set_channel_visible(loop_item[0], checked, display_apply.checked)
-                DualSlider:
-                    minimum = 0
-                    maximum = 100
-                    low_value << int(loop_item[1].min_value * 100)
-                    high_value << int(loop_item[1].max_value * 100)
-                    low_value ::
-                        presenter.set_channel_min_value(loop_item[0], low_value / 100, display_apply.checked)
-                    high_value ::
-                        presenter.set_channel_max_value(loop_item[0], high_value / 100, display_apply.checked)
+        PushButton: channels:
+            text = 'Channels'
+            clicked ::
+                popup = ChannelConfigPopup(self, presenter=dock_item.presenter,
+                                           display_apply=display_apply.checked)
+                popup.show()
 
         Label: display_as_label:
             text = 'as'
 
         ObjectCombo: display_mode:
             items = ['projection', 'slice']
             selected << 'projection' if presenter.current_artist is None else presenter.current_artist.display_mode
@@ -530,25 +545,25 @@
 
             Action:
                 separator = True
 
             Action:
                 text = 'Process 20x LIF file\tCtrl+P'
                 triggered ::
-                    path = FileDialogEx.get_open_file_name(window, current_path=window.current_path)
+                    path = FileDialogEx.get_open_file_name(window, current_path=str(window.current_path))
                     if path:
                         pp = ProgressWindow()
                         pp.show()
                         cb = lambda x, pp=pp: setattr(pp, 'progress', x)
                         deferred_call(util.process_lif, path, reprocess=True, cb=cb)
 
             Action:
                 text = 'Process 63x LIF file\tCtrl+P'
                 triggered ::
-                    path = FileDialogEx.get_open_file_name(window, current_path=window.current_path)
+                    path = FileDialogEx.get_open_file_name(window, current_path=str(window.current_path))
                     if path:
                         pp = ProgressWindow()
                         pp.show()
                         cb = lambda x, pp=pp: setattr(pp, 'progress', x)
                         deferred_call(util.lif_to_ims, path, reprocess=True, cb=cb)
 
             Action:
```

### Comparing `cochleogram-0.3.0/cochleogram/icons/cells.png` & `cochleogram-0.3.1/cochleogram/icons/cells.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.3.0/cochleogram/icons/exclude.png` & `cochleogram-0.3.1/cochleogram/icons/exclude.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.3.0/cochleogram/icons/main-icon.png` & `cochleogram-0.3.1/cochleogram/icons/main-icon.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.3.0/cochleogram/icons/make_icons.py` & `cochleogram-0.3.1/cochleogram/icons/make_icons.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.3.0/cochleogram/icons/spiral.png` & `cochleogram-0.3.1/cochleogram/icons/spiral.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.3.0/cochleogram/icons/tile.png` & `cochleogram-0.3.1/cochleogram/icons/tile.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.3.0/cochleogram/instructions.html` & `cochleogram-0.3.1/cochleogram/instructions.html`

 * *Files identical despite different names*

### Comparing `cochleogram-0.3.0/cochleogram/main.py` & `cochleogram-0.3.1/cochleogram/main.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.3.0/cochleogram/model.py` & `cochleogram-0.3.1/cochleogram/model.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.3.0/cochleogram/plot.py` & `cochleogram-0.3.1/cochleogram/plot.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.3.0/cochleogram/presenter.py` & `cochleogram-0.3.1/cochleogram/presenter.py`

 * *Files 2% similar despite different names*

```diff
@@ -608,14 +608,21 @@
                 self.point_artists[self.cells, 'spiral'].add_point(event.xdata, event.ydata)
             elif self.tool == 'exclude':
                 if self.drag_event is None:
                     self.start_drag_exclude(event)
                 else:
                     self.end_drag_exclude(event, keep=True)
 
+    @observe('tool', 'cells')
+    def _reset_drag(self, event):
+        self.drag_event = None
+        if self.current_spiral_artist is not None:
+            self.current_spiral_artist.start_drag = None
+            self.current_spiral_artist.end_drag = None
+
     def button_release(self, event):
         if event.button == MouseButton.LEFT:
             if not self.pan_performed:
                 self.button_release_tile(event)
             self.end_pan(event)
         elif event.button == MouseButton.RIGHT:
             if self.tool == 'tile':
```

### Comparing `cochleogram-0.3.0/cochleogram/readers.py` & `cochleogram-0.3.1/cochleogram/readers.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.3.0/cochleogram/util.py` & `cochleogram-0.3.1/cochleogram/util.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.3.0/cochleogram.egg-info/PKG-INFO` & `cochleogram-0.3.1/cochleogram.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cochleogram
-Version: 0.3.0
+Version: 0.3.1
 Summary: Module for creating cochleograms from confocal images
 Author-email: Brad Buran <buran@ohsu.edu>
 Maintainer-email: Brad Buran <buran@ohsu.edu>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: czi
 Provides-Extra: lif
```

### Comparing `cochleogram-0.3.0/cochleogram.egg-info/SOURCES.txt` & `cochleogram-0.3.1/cochleogram.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cochleogram-0.3.0/pyproject.toml` & `cochleogram-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cochleogram-0.3.0/readme.rst` & `cochleogram-0.3.1/readme.rst`

 * *Files identical despite different names*

