# Comparing `tmp/pycatsearch-5.1.6.tar.gz` & `tmp/pycatsearch-5.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycatsearch-5.1.6.tar", last modified: Tue Jun 20 15:18:17 2023, max compression
+gzip compressed data, was "pycatsearch-5.1.7.tar", last modified: Thu Jun 22 09:24:14 2023, max compression
```

## Comparing `pycatsearch-5.1.6.tar` & `pycatsearch-5.1.7.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:18:17.160011 pycatsearch-5.1.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:18:17.152011 pycatsearch-5.1.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:18:17.156011 pycatsearch-5.1.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    10610 2023-06-20 15:18:17.160011 pycatsearch-5.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9070 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     1230 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 15:18:17.160011 pycatsearch-5.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:18:17.156011 pycatsearch-5.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:18:17.156011 pycatsearch-5.1.6/src/pycatsearch/
--rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/src/pycatsearch/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      109 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/src/pycatsearch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-20 15:18:17.000000 pycatsearch-5.1.6/src/pycatsearch/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    11022 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/src/pycatsearch/async_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    18859 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/src/pycatsearch/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/src/pycatsearch/catalog_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/src/pycatsearch/downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:18:17.160011 pycatsearch-5.1.6/src/pycatsearch/gui/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/src/pycatsearch/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6578 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/src/pycatsearch/gui/catalog_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/src/pycatsearch/gui/download_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/src/pycatsearch/gui/float_spinbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     7984 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/src/pycatsearch/gui/frequency_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/src/pycatsearch/gui/menu_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)     7688 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/src/pycatsearch/gui/preferences.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/src/pycatsearch/gui/selectable_label.py
--rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/src/pycatsearch/gui/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/src/pycatsearch/gui/substance_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/src/pycatsearch/gui/substances_box.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/src/pycatsearch/gui/titled_list_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    45208 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/src/pycatsearch/gui/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/src/pycatsearch/gui/waiting_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)    24947 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/src/pycatsearch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:18:17.160011 pycatsearch-5.1.6/src/pycatsearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10610 2023-06-20 15:18:17.000000 pycatsearch-5.1.6/src/pycatsearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-20 15:18:17.000000 pycatsearch-5.1.6/src/pycatsearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:18:17.000000 pycatsearch-5.1.6/src/pycatsearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-20 15:18:17.000000 pycatsearch-5.1.6/src/pycatsearch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 15:18:17.000000 pycatsearch-5.1.6/src/pycatsearch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-20 15:18:17.000000 pycatsearch-5.1.6/src/pycatsearch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:24:14.940382 pycatsearch-5.1.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:24:14.936382 pycatsearch-5.1.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:24:14.936382 pycatsearch-5.1.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10610 2023-06-22 09:24:14.940382 pycatsearch-5.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9070 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1230 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 09:24:14.940382 pycatsearch-5.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:24:14.936382 pycatsearch-5.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:24:14.936382 pycatsearch-5.1.7/src/pycatsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/src/pycatsearch/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      109 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/src/pycatsearch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-22 09:24:14.000000 pycatsearch-5.1.7/src/pycatsearch/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11022 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/src/pycatsearch/async_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18859 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/src/pycatsearch/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/src/pycatsearch/catalog_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/src/pycatsearch/downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:24:14.940382 pycatsearch-5.1.7/src/pycatsearch/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/src/pycatsearch/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6578 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/src/pycatsearch/gui/catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/src/pycatsearch/gui/download_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/src/pycatsearch/gui/float_spinbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7984 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/src/pycatsearch/gui/frequency_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/src/pycatsearch/gui/menu_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7688 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/src/pycatsearch/gui/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/src/pycatsearch/gui/selectable_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/src/pycatsearch/gui/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/src/pycatsearch/gui/substance_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/src/pycatsearch/gui/substances_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/src/pycatsearch/gui/titled_list_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45337 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/src/pycatsearch/gui/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/src/pycatsearch/gui/waiting_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25354 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/src/pycatsearch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:24:14.940382 pycatsearch-5.1.7/src/pycatsearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10610 2023-06-22 09:24:14.000000 pycatsearch-5.1.7/src/pycatsearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-22 09:24:14.000000 pycatsearch-5.1.7/src/pycatsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 09:24:14.000000 pycatsearch-5.1.7/src/pycatsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-22 09:24:14.000000 pycatsearch-5.1.7/src/pycatsearch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 09:24:14.000000 pycatsearch-5.1.7/src/pycatsearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-22 09:24:14.000000 pycatsearch-5.1.7/src/pycatsearch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-06-22 09:24:04.000000 pycatsearch-5.1.7/updater.py
```

### Comparing `pycatsearch-5.1.6/.github/workflows/publish-to-pypi.yml` & `pycatsearch-5.1.7/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.6/LICENSE.md` & `pycatsearch-5.1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.6/PKG-INFO` & `pycatsearch-5.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycatsearch
-Version: 5.1.6
+Version: 5.1.7
 Summary: Yet another implementation of JPL and CDMS spectroscopy catalogs offline search
 Author-email: StSav012 <stsav012@gmail.com>
 License: LGPL-3.0-only
 Project-URL: Source Code, https://github.com/StSav012/pycatsearch
 Project-URL: Bug Tracker, https://github.com/StSav012/pycatsearch/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Win32 (MS Windows)
```

### Comparing `pycatsearch-5.1.6/README.md` & `pycatsearch-5.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.6/main.py` & `pycatsearch-5.1.7/main.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.6/pyproject.toml` & `pycatsearch-5.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.6/setup.py` & `pycatsearch-5.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.6/src/pycatsearch/__init__.py` & `pycatsearch-5.1.7/src/pycatsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.6/src/pycatsearch/async_downloader.py` & `pycatsearch-5.1.7/src/pycatsearch/async_downloader.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.6/src/pycatsearch/catalog.py` & `pycatsearch-5.1.7/src/pycatsearch/catalog.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.6/src/pycatsearch/catalog_entry.py` & `pycatsearch-5.1.7/src/pycatsearch/catalog_entry.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.6/src/pycatsearch/downloader.py` & `pycatsearch-5.1.7/src/pycatsearch/downloader.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.6/src/pycatsearch/gui/__init__.py` & `pycatsearch-5.1.7/src/pycatsearch/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.6/src/pycatsearch/gui/catalog_info.py` & `pycatsearch-5.1.7/src/pycatsearch/gui/catalog_info.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.6/src/pycatsearch/gui/download_dialog.py` & `pycatsearch-5.1.7/src/pycatsearch/gui/download_dialog.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.6/src/pycatsearch/gui/float_spinbox.py` & `pycatsearch-5.1.7/src/pycatsearch/gui/float_spinbox.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.6/src/pycatsearch/gui/frequency_box.py` & `pycatsearch-5.1.7/src/pycatsearch/gui/frequency_box.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.6/src/pycatsearch/gui/menu_bar.py` & `pycatsearch-5.1.7/src/pycatsearch/gui/menu_bar.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.6/src/pycatsearch/gui/preferences.py` & `pycatsearch-5.1.7/src/pycatsearch/gui/preferences.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.6/src/pycatsearch/gui/settings.py` & `pycatsearch-5.1.7/src/pycatsearch/gui/settings.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.6/src/pycatsearch/gui/substance_info.py` & `pycatsearch-5.1.7/src/pycatsearch/gui/substance_info.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.6/src/pycatsearch/gui/substances_box.py` & `pycatsearch-5.1.7/src/pycatsearch/gui/substances_box.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.6/src/pycatsearch/gui/titled_list_widget.py` & `pycatsearch-5.1.7/src/pycatsearch/gui/titled_list_widget.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.6/src/pycatsearch/gui/ui.py` & `pycatsearch-5.1.7/src/pycatsearch/gui/ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
 import math
 from typing import Any, Callable, Final, final
 
-from qtpy.QtCore import QAbstractTableModel, QByteArray, QMimeData, QModelIndex, QPoint, QPointF, QRect, QSize, Qt, Slot
+from qtpy.QtCore import (QAbstractTableModel, QByteArray, QItemSelection, QMimeData, QModelIndex, QPoint, QPointF,
+                         QRect, QSize, Qt, Slot)
 from qtpy.QtGui import (QAbstractTextDocumentLayout, QClipboard, QCloseEvent, QCursor, QIcon, QPainter, QPixmap,
                         QScreen, QTextDocument)
 from qtpy.QtWidgets import (QAbstractItemView, QAbstractSpinBox, QApplication, QDoubleSpinBox, QFormLayout, QHeaderView,
                             QMainWindow, QMessageBox, QPushButton, QSplitter, QStatusBar, QStyle, QStyleOptionViewItem,
                             QStyledItemDelegate, QTableView, QVBoxLayout, QWidget)
 from qtpy.compat import getopenfilenames
 
@@ -486,16 +487,16 @@
         if self.results_shown:
             self.fill_table()
 
     @Slot(QPoint)
     def _on_table_context_menu_requested(self, pos: QPoint) -> None:
         self.menu_bar.menu_edit.popup(self.results_table.viewport().mapToGlobal(pos))
 
-    @Slot()
-    def _on_table_item_selection_changed(self) -> None:
+    @Slot(QItemSelection, QItemSelection)
+    def _on_table_item_selection_changed(self, _selected: QItemSelection, _deselected: QItemSelection) -> None:
         self.menu_bar.action_copy.setEnabled(bool(self.results_table.selectionModel().selectedRows()))
         self.menu_bar.action_substance_info.setEnabled(bool(self.results_table.selectionModel().selectedRows()))
 
     def get_open_file_names(self, formats: dict[tuple[str, ...], str],
                             caption: str = '', directory: str = '') -> tuple[list[str], str]:
 
         def join_file_dialog_formats(_formats: dict[tuple[str, ...], str]) -> str:
```

### Comparing `pycatsearch-5.1.6/src/pycatsearch/gui/waiting_screen.py` & `pycatsearch-5.1.7/src/pycatsearch/gui/waiting_screen.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.6/src/pycatsearch/utils.py` & `pycatsearch-5.1.7/src/pycatsearch/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
+import builtins
 import html
 import html.entities
 import itertools
 import math
 import os
+import sys
 from numbers import Real
 from pathlib import Path
-from typing import Callable, Final, Iterator, Protocol, Sequence, TypeVar, cast, overload
+from typing import Any, Callable, Final, Iterable, Iterator, Protocol, Sequence, TypeVar, cast, overload
 
 __all__ = ['M_LOG10E',
            'T0', 'c', 'h', 'k', 'e',
            'CATALOG', 'BUILD_TIME', 'LINES', 'FREQUENCY', 'INTENSITY', 'ID', 'STRUCTURAL_FORMULA',
            'STOICHIOMETRIC_FORMULA', 'MOLECULE', 'MOLECULE_SYMBOL', 'SPECIES_TAG', 'NAME', 'TRIVIAL_NAME', 'ISOTOPOLOG',
            'STATE', 'STATE_HTML', 'INCHI_KEY', 'DEGREES_OF_FREEDOM', 'LOWER_STATE_ENERGY', 'CONTRIBUTOR', 'VERSION',
            'DATE_OF_ENTRY', 'HUMAN_READABLE',
@@ -27,15 +29,16 @@
            'sq_nm_mhz_to_log10_sq_nm_mhz',
            'log10_cm_per_molecule_to_log10_sq_nm_mhz',
            'cm_per_molecule_to_log10_sq_nm_mhz',
            'sort_unique', 'merge_sorted', 'search_sorted',
            'within', 'chem_html', 'best_name', 'remove_html', 'wrap_in_html',
            'ensure_prefix', 'all_cases',
            'save_catalog_to_file',
-           'ReleaseInfo', 'latest_release', 'update_with_pip']
+           'ReleaseInfo', 'latest_release', 'update_with_pip',
+           'zip']
 
 M_LOG10E: Final[float] = math.log10(math.e)
 
 T0: Final[float] = 300.00  # [K], see https://spec.jpl.nasa.gov/ftp/pub/catalog/doc/catdoc.pdf
 k: Final[float] = 1.380649000e-23  # [J/K],  see https://physics.nist.gov/cgi-bin/cuu/Value?k
 h: Final[float] = 6.626070150e-34  # [J/Hz], see https://physics.nist.gov/cgi-bin/cuu/Value?h
 e: Final[float] = 1.602176634e-19  # [C],    see https://physics.nist.gov/cgi-bin/cuu/Value?e
@@ -681,7 +684,16 @@
 
     subprocess.Popen(args=[
         sys.executable, '-c',
         f'''import sys, subprocess, time; time.sleep(2);\
         subprocess.run(args=[sys.executable, '-m', 'pip', 'install', '-U', {__original_name__!r}]);\
         subprocess.Popen(args=[sys.executable, '-m', {__original_name__!r}])'''])
     sys.exit(0)
+
+
+# noinspection PyShadowingBuiltins
+def zip(*iterables: Iterable[Any], strict: bool = False) -> builtins.zip:
+    """ Intentionally override `builtins.zip` to ignore `strict` parameter in Python < 3.10 """
+    if sys.version_info < (3, 10):
+        return builtins.zip(*iterables)
+    else:
+        return builtins.zip(*iterables, strict=strict)
```

### Comparing `pycatsearch-5.1.6/src/pycatsearch.egg-info/PKG-INFO` & `pycatsearch-5.1.7/src/pycatsearch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycatsearch
-Version: 5.1.6
+Version: 5.1.7
 Summary: Yet another implementation of JPL and CDMS spectroscopy catalogs offline search
 Author-email: StSav012 <stsav012@gmail.com>
 License: LGPL-3.0-only
 Project-URL: Source Code, https://github.com/StSav012/pycatsearch
 Project-URL: Bug Tracker, https://github.com/StSav012/pycatsearch/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Win32 (MS Windows)
```

### Comparing `pycatsearch-5.1.6/src/pycatsearch.egg-info/SOURCES.txt` & `pycatsearch-5.1.7/src/pycatsearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.6/updater.py` & `pycatsearch-5.1.7/updater.py`

 * *Files identical despite different names*

