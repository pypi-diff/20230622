# Comparing `tmp/vtable-0.1.5.tar.gz` & `tmp/vtable-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vtable-0.1.5.tar", max compression
+gzip compressed data, was "vtable-0.1.6.tar", max compression
```

## Comparing `vtable-0.1.5.tar` & `vtable-0.1.6.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0    35149 2023-06-16 17:21:26.072295 vtable-0.1.5/LICENSE
--rw-r--r--   0        0        0       46 2023-06-16 17:21:26.072295 vtable-0.1.5/README.md
--rw-r--r--   0        0        0      415 2023-06-16 21:31:00.156846 vtable-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      197 2023-06-16 20:54:07.044765 vtable-0.1.5/vtable/__init__.py
--rw-r--r--   0        0        0     4316 2023-06-16 17:58:42.164378 vtable-0.1.5/vtable/checkablecombo.py
--rw-r--r--   0        0        0     6853 2023-06-16 21:16:00.984813 vtable-0.1.5/vtable/colfilters.py
--rw-r--r--   0        0        0     1287 2023-06-16 21:27:24.744838 vtable-0.1.5/vtable/loaders.py
--rw-r--r--   0        0        0     2100 2023-06-16 21:29:32.852843 vtable-0.1.5/vtable/main.py
--rw-r--r--   0        0        0     3610 2023-06-16 17:59:08.676379 vtable-0.1.5/vtable/newtable.py
--rw-r--r--   0        0        0     1704 2023-06-16 17:59:18.176379 vtable-0.1.5/vtable/selector.py
--rw-r--r--   0        0        0     2219 2023-06-16 20:40:52.680735 vtable-0.1.5/vtable/supertable.py
--rw-r--r--   0        0        0      709 1970-01-01 00:00:00.000000 vtable-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-17 21:16:27.103208 vtable-0.1.6/LICENSE
+-rw-r--r--   0        0        0       46 2023-06-17 21:16:27.103208 vtable-0.1.6/README.md
+-rw-r--r--   0        0        0      415 2023-06-21 12:49:41.605234 vtable-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      196 2023-06-18 18:50:07.090783 vtable-0.1.6/vtable/__init__.py
+-rw-r--r--   0        0        0     4316 2023-06-17 21:16:27.103208 vtable-0.1.6/vtable/checkablecombo.py
+-rw-r--r--   0        0        0     7409 2023-06-21 02:55:20.296310 vtable-0.1.6/vtable/colfilters.py
+-rwxr-xr-x   0        0        0     4709 2023-06-21 02:55:27.572551 vtable-0.1.6/vtable/filteredtablemodel.py
+-rw-r--r--   0        0        0     1539 2023-06-21 12:47:17.613028 vtable-0.1.6/vtable/loaders.py
+-rw-r--r--   0        0        0     2621 2023-06-22 01:04:45.867760 vtable-0.1.6/vtable/main.py
+-rw-r--r--   0        0        0     3645 2023-06-21 02:55:30.712656 vtable-0.1.6/vtable/newtable.py
+-rw-r--r--   0        0        0     1706 2023-06-21 02:55:43.093075 vtable-0.1.6/vtable/selector.py
+-rw-r--r--   0        0        0     3194 2023-06-21 12:30:33.060104 vtable-0.1.6/vtable/supertable.py
+-rw-r--r--   0        0        0      770 2023-06-22 01:29:00.599243 vtable-0.1.6/setup.py
+-rw-r--r--   0        0        0      658 2023-06-22 01:29:00.599577 vtable-0.1.6/PKG-INFO
```

### Comparing `vtable-0.1.5/LICENSE` & `vtable-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vtable-0.1.5/vtable/checkablecombo.py` & `vtable-0.1.6/vtable/checkablecombo.py`

 * *Files identical despite different names*

### Comparing `vtable-0.1.5/vtable/colfilters.py` & `vtable-0.1.6/vtable/colfilters.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from ipdb import set_trace as idebug
+# from ipdb import set_trace as idebug
 import numpy as np
 import re
 
 
 import PyQt5.QtWidgets as QtWidget
 import PyQt5.QtCore as QtCore
 
 from .checkablecombo import CheckableComboBox
 
 QtCore.Signal = QtCore.pyqtSignal
 """
-Abstract and concreate column filter classes. 
+Abstract and concreate column filter classes.
 
-These are QWidget objects that also encode the logic of which rows should be filtered in and out 
+These are QWidget objects that also encode the logic of which rows should be filtered in and out
 """
 
 
 class AbstractColumnFilter(QtWidget.QWidget):
     changed = QtCore.Signal()
 
     def __init__(self, parent=None):
@@ -55,36 +55,36 @@
         layout = QtWidget.QVBoxLayout()
         layout.addWidget(self.label)
         layout.addWidget(self.combo)
         self.setLayout(layout)
 
 
     def getFilteredIn(self) -> np.ndarray:
-        print('Debug GFI', self.col.name, np.sum(self.idx))
+        # print('Debug GFI', self.col.name, np.sum(self.idx))
         return self.idx.copy()
 
     def onChange(self):
         print("Getting selection for CatFilter for ", self.col.name)
         selected = self.combo.getSelectedItems()
-        print(selected)
-        print(self.col.astype(str).values[:10])
-        print(self.col.astype(str).values[-10:])
+        # print(selected)
+        # print(self.col.astype(str).values[:10])
+        # print(self.col.astype(str).values[-10:])
         idx = self.col.astype(str).isin(selected)
 
-        print( np.all(self.col.astype(str) == '0'))
-        print(np.sum(self.col.astype(str) == '0'))
-        print(np.sum(self.col.astype(str) == '1'))
-        print(np.where(idx == False))
-        print(idx)
+        # print( np.all(self.col.astype(str) == '0'))
+        # print(np.sum(self.col.astype(str) == '0'))
+        # print(np.sum(self.col.astype(str) == '1'))
+        # print(np.where(idx == False))
+        # print(idx)
 
         try:
             self.idx = idx.values
         except AttributeError:
             self.idx = idx
-        print('Debug', self.col.name, np.sum(idx))
+        # print('Debug', self.col.name, np.sum(idx))
         self.changed.emit()
 
     def setWidth(self, width):
         self.combo.setMaximumWidth(width)
 
 
 class NumericFilter(AbstractColumnFilter):
@@ -101,14 +101,24 @@
         layout = QtWidget.QVBoxLayout()
         layout.addWidget(self.label)
         layout.addWidget(self.edit)
         self.setLayout(layout)
         self.show()
 
     def onChange(self):
+        """
+
+        o fail(?) on semi-colons
+        o Split on '&' and '|', maybe a special xor character?
+        o parse seach subsection independently
+        o Look for nan and ~nan
+        o Wrap in brackets
+        o join
+        o eval
+        """
         # print(f"Change detected in {self.col}: {self}")
         text = self.edit.text()
         cmd = self.parseText(text)
 
         if cmd == "":
             self.idx = np.ones(len(self.col), dtype=bool)   # No filter
             self.changed.emit()
@@ -132,15 +142,15 @@
             return
         # print("idx is numpy array")
 
         if len(idx) != len(self.col):
             return
         # print("idx is correct length")
         self.idx = idx
-        # print("Emiting")
+        # print(f"Emiting: Indices are {np.where(idx)[0]}")
         self.changed.emit()
 
 
     def parseText(self, text):
         if text == "":
             return text
 
@@ -181,17 +191,22 @@
         self.setLayout(layout)
         self.show()
 
     def onChange(self):
         # print(f"Change detected in {self.col}: {self}")
 
         text = self.edit.text()
-        num_char = len(text)
-        self.idx = text == self.col.str[:num_char]
-        # print(f"string: {np.sum(self.idx)} of {len(self.idx)} are true")
+        # num_char = len(text)
+        # self.idx = text == self.col.str[:num_char]
+
+        #Works around an edge case of Nans appearing in a text field
+        self.idx = self.col.str.contains(text).values.astype(bool)
+        # self.idx[~np.isfinite(self.idx)] = False 
+        
+        # print("In string filter: ", self.idx)
         self.changed.emit()
 
     def getFilteredIn(self):
         try:
             return self.idx.values.copy()
         except AttributeError:
             return self.idx.copy()
@@ -231,15 +246,16 @@
         # print("   ---    ")
         # print(f0.col.name,  np.sum(idx), " of ", len(f0.col))
         for i in range(0, self.layout.count()):
             f = self.layout.itemAt(i).widget()
             idx2 = f.getFilteredIn()
             # print(f.col.name, np.sum(idx2), " of ", len(idx2))
             # print("Idx is now:", np.sum(idx))
-
+            # print(i, idx.dtype)
+            # print(i, f, idx2.dtype)
             idx &= idx2
         return idx
 
     def showColumn(self, i):
         self.filter_list[i].show()
 
     def hideColumn(self, i):
```

### Comparing `vtable-0.1.5/vtable/loaders.py` & `vtable-0.1.6/vtable/loaders.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,54 @@
 from importlib import import_module
+import pandas as pd
+
+def fits_to_pandas(fits):
+    df = pd.DataFrame(fits.tolist())
+    df.columns = fits.columns.names
+    return df 
+
+
 class Loader:
     """A class to load data from filse of different formats, that doesn't fail when
     modules to load those files don't exist
 
-    THIS IS UNTESTED
     """
 
     def __init__(self):
         self.opts = {
-            'csv': 'pandas.read_csv',
-            'csv.gz': 'pandas.read_csv',
-            'parquet': 'pandas.read_parquet',
-            'fits': 'pyfits.io.fits.getdata',
+            'csv': ('pandas.read_csv', None),
+            'csv.gz': ('pandas.read_csv', None),
+            'parquet': ('pandas.read_parquet', None),
+            'fits': ('astropy.io.fits.getdata', fits_to_pandas),
         }
 
     def load(self, path):
         filetype = get_filetype(path)
 
         try:
-            importstr = self.opts[filetype]
+            importstr, convertor = self.opts[filetype]
         except KeyError:
             raise ValueError(f"No loader defined for files of type {filetype}")
 
         package = ".".join(importstr.split('.')[:-1])
         func = importstr.split('.')[-1]
         pkg = import_module(package)
         # print(pkg)
         # func = eval(importstr)
         # func = eval(f"{pkg}.{func}")
 
         try:
             func = pkg.__dict__[func]
         except KeyError:
             raise ValueError(f"Package {package} has no function called {func}")
-        return func(path)
 
+        df = func(path)
+        if convertor is not None:
+            df = convertor(df)
+        return df 
 
 
 def get_filetype(path):
     tokens = path.split('.')
 
     # If the suffix is gz, include previous suffix
     if tokens[-1] in "gz bz2".split():
```

### Comparing `vtable-0.1.5/vtable/newtable.py` & `vtable-0.1.6/vtable/newtable.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import PyQt5.QtWidgets as QtWidget
 import PyQt5.QtCore as QtCore
 import PyQt5.QtGui as QtGui
 import PyQt5.QtWidgets
 
-from ipdb import set_trace as idebug
+# from ipdb import set_trace as idebug
 import numpy as np
 
 
 class TableWidget(PyQt5.QtWidgets.QTableWidget):
     def __init__(self, df, num=1000, parent=None):
         self.df = df
         self.num = num
 
         self.include_row = np.ones(len(self.df), dtype=bool)
-        self.max_width = 1000
+        self.max_width = 10000
 
         self.nrow = len(self.df)
         self.ncol = len(self.df.columns)
         super().__init__(self.nrow, self.ncol, parent=parent)
 
 
         # PyQt5.QtWidgets.QTableWidget(self.nrow, self.ncol)
@@ -64,27 +64,28 @@
                     item = QItem(str(elt))
                 # Mark item as readonly
                 item.setFlags( item.flags() & ~QtCore.Qt.EditRole)
                 self.setItem(j, i, item)
 
         self.resizeColumnsToContents()
         self.resizeRowsToContents()
+        self.set_size_policy()
 
     def resetTable(self):
         """Clear data from the table"""
         row_count = self.rowCount()
         self.setRowCount(0)
 
     def set_size_policy(self):
-        width_pix = self.horizontalHeader().length() + self.verticalHeader().width() + 20
+        width_pix = self.horizontalHeader().length() + self.verticalHeader().width() + 200
         height_pix = self.verticalHeader().length() + self.horizontalHeader().width()
         self.setMaximumSize(width_pix, height_pix)
         self.max_width = width_pix
 
-        width_pix = min(width_pix, 1000)
+        width_pix = min(width_pix, 2000)
         height_pix = min(height_pix, 1000)
         self.resize(width_pix, height_pix)
 
     def getMaxWidth(self):
         return self.max_width
 
     def draw_row_guides(self):
```

### Comparing `vtable-0.1.5/vtable/selector.py` & `vtable-0.1.6/vtable/selector.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ipdb import set_trace as idebug
+# from ipdb import set_trace as idebug
 
 import PyQt5.QtWidgets as QtWidget
 import PyQt5.QtWidgets
 
 
 class ColumnSelector(PyQt5.QtWidgets.QDialog):
     def __init__(self, table, parent=None):
```

### Comparing `vtable-0.1.5/vtable/supertable.py` & `vtable-0.1.6/vtable/supertable.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,72 +1,99 @@
 import PyQt5.QtWidgets as QtWidget
+import PyQt5.QtCore as QtCore
+
 
 import numpy as np
 from . import colfilters
 from . import newtable
+from .filteredtablemodel import FilteredTableModel
 
 class SuperTableWidget(QtWidget.QDialog):
     def __init__(self, df, num=1000, parent=None):
         QtWidget.QMainWindow.__init__(self, parent)
         self.df = df
         self.ncol = len(df.columns)
+        self.max_width  = 1000
 
         self.collection = create_filter_collection(df)
         self.collection.changed.connect(self.updateFilters)
 
-        self.table = newtable.TableWidget(df, num=num)
+        self.tableModel = FilteredTableModel(df)
+        self.tableView = QtWidget.QTableView()
+        self.tableView.setModel(self.tableModel)
+        self.tableView.setSortingEnabled(True)
+        # self.tableView.setHorizontalHeaderLabels(df.columns)
+        self.tableView.resizeColumnsToContents()
+        
+        # self.table = newtable.TableWidget(df, num=num)
         layout = QtWidget.QVBoxLayout()
         layout.addWidget(self.collection)
-        layout.addWidget(self.table)
+        layout.addWidget(self.tableView)
         self.setLayout(layout)
         self.show()
 
     def updateFilters(self):
         idx = self.collection.getFilteredIn()
-        # print("In main window: ", np.sum(idx), " of ", len(idx))
-        self.table.drawFiltered(idx)
+        # print("In Supertable.updateFilters: ", np.sum(idx), " of ", len(idx))
+        self.tableModel.setFiltered(idx)
 
     def toggleColumn(self, sender_label, state):
-        cols = self.table.df.columns
+        #cols = self.table.df.columns
+        cols = self.tableModel.getColumns()
         for i in range(self.ncol):
             if cols[i] == sender_label:
                 if state:
-                    self.table.showColumn(i)
+                    self.tableView.showColumn(i)
                     self.collection.showColumn(i)
                 else:
-                    self.table.hideColumn(i)
+                    self.tableView.hideColumn(i)
                     self.collection.hideColumn(i)
 
     def showAll(self):
         for i in range(self.ncol):
             self.table.showColumn(i)
             self.collection.showColumn(i)
 
     def hideAll(self):
         for i in range(self.ncol):
             self.table.hideColumn(i)
             self.collection.hideColumn(i)
 
+
+    def set_size_policy(self):
+        tv = self.tableView
+        width_pix = tv.horizontalHeader().length() + tv.verticalHeader().width() + 20
+        height_pix = tv.verticalHeader().length() + tv.horizontalHeader().width()
+        tv.setMaximumSize(width_pix, height_pix)
+        self.max_width = width_pix
+
+        width_pix = min(width_pix, 1000)
+        height_pix = min(height_pix, 1000)
+        self.resize(width_pix, height_pix)
+
     def getMaxWidth(self):
-        return self.table.max_width
+        return self.max_width
+
+
 
 
 def create_filter_collection(df):
     cols = df.columns
 
     filter_list = []
     for c in cols:
         filter_list.append(create_column_filter(df, c))
-        print(c, filter_list[-1])
+        # print(c, filter_list[-1])
 
     collection = colfilters.FilterCollection(filter_list)
     return collection
 
 
 def create_column_filter(df, c):
+    # import pdb; pdb.set_trace()
     col = df[c]
     num_values = len(set(col))
     if num_values < 10:
         return colfilters.CategoricalFilter(col)
 
     # idebug()
     dtype = col.dtype
```

### Comparing `vtable-0.1.5/PKG-INFO` & `vtable-0.1.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: vtable
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Qt based table viewer for Python
 License: GPL 3.0
 Author: fergal
 Author-email: fergal.mullally@gmail.com
 Requires-Python: >3.6
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyQt5
 Requires-Dist: ipdb
 Requires-Dist: numpy
 Requires-Dist: pandas
 Description-Content-Type: text/markdown
 
 # qtable
```

