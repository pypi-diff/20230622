# Comparing `tmp/datamatrix-1.0.2.tar.gz` & `tmp/datamatrix-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamatrix-1.0.2.tar", last modified: Wed Mar 29 14:49:49 2023, max compression
+gzip compressed data, was "datamatrix-1.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `datamatrix-1.0.2.tar` & `datamatrix-1.0.4.tar`

### file list

```diff
@@ -1,43 +1,44 @@
--rw-r--r--   0        0        0    35147 2023-03-29 14:49:33.670452 datamatrix-1.0.2/COPYING
--rw-r--r--   0        0        0     1281 2023-03-29 14:49:33.670452 datamatrix-1.0.2/datamatrix/__init__.py
--rw-r--r--   0        0        0     1952 2023-03-29 14:49:33.670452 datamatrix-1.0.2/datamatrix/_config.py
--rw-r--r--   0        0        0      673 2023-03-29 14:49:33.670452 datamatrix-1.0.2/datamatrix/_datamatrix/__init__.py
--rw-r--r--   0        0        0    28220 2023-03-29 14:49:33.670452 datamatrix-1.0.2/datamatrix/_datamatrix/_basecolumn.py
--rw-r--r--   0        0        0     6556 2023-03-29 14:49:33.670452 datamatrix-1.0.2/datamatrix/_datamatrix/_blinkreconstruct.py
--rw-r--r--   0        0        0      878 2023-03-29 14:49:33.670452 datamatrix-1.0.2/datamatrix/_datamatrix/_callable_values.py
--rw-r--r--   0        0        0    25440 2023-03-29 14:49:33.670452 datamatrix-1.0.2/datamatrix/_datamatrix/_datamatrix.py
--rw-r--r--   0        0        0     4167 2023-03-29 14:49:33.670452 datamatrix-1.0.2/datamatrix/_datamatrix/_index.py
--rw-r--r--   0        0        0      898 2023-03-29 14:49:33.670452 datamatrix-1.0.2/datamatrix/_datamatrix/_mixedcolumn.py
--rw-r--r--   0        0        0    25682 2023-03-29 14:49:33.670452 datamatrix-1.0.2/datamatrix/_datamatrix/_multidimensionalcolumn.py
--rw-r--r--   0        0        0     4005 2023-03-29 14:49:33.670452 datamatrix-1.0.2/datamatrix/_datamatrix/_nifticolumn.py
--rw-r--r--   0        0        0    12828 2023-03-29 14:49:33.670452 datamatrix-1.0.2/datamatrix/_datamatrix/_numericcolumn.py
--rw-r--r--   0        0        0     3028 2023-03-29 14:49:33.670452 datamatrix-1.0.2/datamatrix/_datamatrix/_row.py
--rw-r--r--   0        0        0     1552 2023-03-29 14:49:33.670452 datamatrix-1.0.2/datamatrix/_datamatrix/_seriescolumn.py
--rw-r--r--   0        0        0     2922 2023-03-29 14:49:33.670452 datamatrix-1.0.2/datamatrix/_datamatrix/_sort.py
--rw-r--r--   0        0        0      673 2023-03-29 14:49:33.670452 datamatrix-1.0.2/datamatrix/_functional/__init__.py
--rw-r--r--   0        0        0    13219 2023-03-29 14:49:33.670452 datamatrix-1.0.2/datamatrix/_functional/_memoize.py
--rw-r--r--   0        0        0     1672 2023-03-29 14:49:33.670452 datamatrix-1.0.2/datamatrix/_ordered_state.py
--rw-r--r--   0        0        0      673 2023-03-29 14:49:33.670452 datamatrix-1.0.2/datamatrix/colors/__init__.py
--rw-r--r--   0        0        0     1415 2023-03-29 14:49:33.670452 datamatrix-1.0.2/datamatrix/colors/tango.py
--rw-r--r--   0        0        0      990 2023-03-29 14:49:33.670452 datamatrix-1.0.2/datamatrix/convert/__init__.py
--rw-r--r--   0        0        0     3978 2023-03-29 14:49:33.670452 datamatrix-1.0.2/datamatrix/convert/_html.py
--rw-r--r--   0        0        0     2348 2023-03-29 14:49:33.670452 datamatrix-1.0.2/datamatrix/convert/_json.py
--rw-r--r--   0        0        0     8604 2023-03-29 14:49:33.670452 datamatrix-1.0.2/datamatrix/convert/_mne.py
--rw-r--r--   0        0        0     3849 2023-03-29 14:49:33.670452 datamatrix-1.0.2/datamatrix/convert/_pandas.py
--rw-r--r--   0        0        0    13532 2023-03-29 14:49:33.670452 datamatrix-1.0.2/datamatrix/functional.py
--rw-r--r--   0        0        0     1003 2023-03-29 14:49:33.670452 datamatrix-1.0.2/datamatrix/io/__init__.py
--rw-r--r--   0        0        0     5191 2023-03-29 14:49:33.670452 datamatrix-1.0.2/datamatrix/io/_bin.py
--rw-r--r--   0        0        0     4565 2023-03-29 14:49:33.670452 datamatrix-1.0.2/datamatrix/io/_excel.py
--rw-r--r--   0        0        0     2807 2023-03-29 14:49:33.670452 datamatrix-1.0.2/datamatrix/io/_pickle.py
--rw-r--r--   0        0        0     3318 2023-03-29 14:49:33.674452 datamatrix-1.0.2/datamatrix/io/_text.py
--rw-r--r--   0        0        0     1412 2023-03-29 14:49:33.674452 datamatrix-1.0.2/datamatrix/monkeypatch.py
--rw-r--r--   0        0        0     7822 2023-03-29 14:49:33.674452 datamatrix-1.0.2/datamatrix/multidimensional.py
--rw-r--r--   0        0        0    29160 2023-03-29 14:49:33.674452 datamatrix-1.0.2/datamatrix/operations.py
--rw-r--r--   0        0        0     4205 2023-03-29 14:49:33.674452 datamatrix-1.0.2/datamatrix/plot.py
--rw-r--r--   0        0        0     3125 2023-03-29 14:49:33.674452 datamatrix-1.0.2/datamatrix/py3compat.py
--rw-r--r--   0        0        0     1059 2023-03-29 14:49:33.674452 datamatrix-1.0.2/datamatrix/rbridge/__init__.py
--rw-r--r--   0        0        0     4422 2023-03-29 14:49:33.674452 datamatrix-1.0.2/datamatrix/rbridge/lme4.py
--rw-r--r--   0        0        0    53892 2023-03-29 14:49:33.674452 datamatrix-1.0.2/datamatrix/series.py
--rw-r--r--   0        0        0      834 2023-03-29 14:49:34.082454 datamatrix-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     5859 2023-03-29 14:49:34.082454 datamatrix-1.0.2/readme.md
--rw-r--r--   0        0        0     6410 1970-01-01 00:00:00.000000 datamatrix-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    35147 2023-06-22 15:35:41.970158 datamatrix-1.0.4/COPYING
+-rw-r--r--   0        0        0     1281 2023-06-22 15:35:41.970158 datamatrix-1.0.4/datamatrix/__init__.py
+-rw-r--r--   0        0        0     1952 2023-06-22 15:35:41.970158 datamatrix-1.0.4/datamatrix/_config.py
+-rw-r--r--   0        0        0      673 2023-06-22 15:35:41.970158 datamatrix-1.0.4/datamatrix/_datamatrix/__init__.py
+-rw-r--r--   0        0        0    28244 2023-06-22 15:35:41.970158 datamatrix-1.0.4/datamatrix/_datamatrix/_basecolumn.py
+-rw-r--r--   0        0        0     6556 2023-06-22 15:35:41.970158 datamatrix-1.0.4/datamatrix/_datamatrix/_blinkreconstruct.py
+-rw-r--r--   0        0        0      878 2023-06-22 15:35:41.970158 datamatrix-1.0.4/datamatrix/_datamatrix/_callable_values.py
+-rw-r--r--   0        0        0    27063 2023-06-22 15:35:41.970158 datamatrix-1.0.4/datamatrix/_datamatrix/_datamatrix.py
+-rw-r--r--   0        0        0     4167 2023-06-22 15:35:41.970158 datamatrix-1.0.4/datamatrix/_datamatrix/_index.py
+-rw-r--r--   0        0        0      898 2023-06-22 15:35:41.970158 datamatrix-1.0.4/datamatrix/_datamatrix/_mixedcolumn.py
+-rw-r--r--   0        0        0    25682 2023-06-22 15:35:41.970158 datamatrix-1.0.4/datamatrix/_datamatrix/_multidimensionalcolumn.py
+-rw-r--r--   0        0        0     4005 2023-06-22 15:35:41.970158 datamatrix-1.0.4/datamatrix/_datamatrix/_nifticolumn.py
+-rw-r--r--   0        0        0    12861 2023-06-22 15:35:41.970158 datamatrix-1.0.4/datamatrix/_datamatrix/_numericcolumn.py
+-rw-r--r--   0        0        0     3028 2023-06-22 15:35:41.970158 datamatrix-1.0.4/datamatrix/_datamatrix/_row.py
+-rw-r--r--   0        0        0     1552 2023-06-22 15:35:41.970158 datamatrix-1.0.4/datamatrix/_datamatrix/_seriescolumn.py
+-rw-r--r--   0        0        0     2922 2023-06-22 15:35:41.970158 datamatrix-1.0.4/datamatrix/_datamatrix/_sort.py
+-rw-r--r--   0        0        0     1568 2023-06-22 15:35:41.970158 datamatrix-1.0.4/datamatrix/_datamatrix/_uninstantiatedcolumn.py
+-rw-r--r--   0        0        0      673 2023-06-22 15:35:41.970158 datamatrix-1.0.4/datamatrix/_functional/__init__.py
+-rw-r--r--   0        0        0    13219 2023-06-22 15:35:41.970158 datamatrix-1.0.4/datamatrix/_functional/_memoize.py
+-rw-r--r--   0        0        0     1672 2023-06-22 15:35:41.970158 datamatrix-1.0.4/datamatrix/_ordered_state.py
+-rw-r--r--   0        0        0      673 2023-06-22 15:35:41.970158 datamatrix-1.0.4/datamatrix/colors/__init__.py
+-rw-r--r--   0        0        0     1415 2023-06-22 15:35:41.970158 datamatrix-1.0.4/datamatrix/colors/tango.py
+-rw-r--r--   0        0        0      990 2023-06-22 15:35:41.970158 datamatrix-1.0.4/datamatrix/convert/__init__.py
+-rw-r--r--   0        0        0     3978 2023-06-22 15:35:41.970158 datamatrix-1.0.4/datamatrix/convert/_html.py
+-rw-r--r--   0        0        0     2348 2023-06-22 15:35:41.974158 datamatrix-1.0.4/datamatrix/convert/_json.py
+-rw-r--r--   0        0        0     8604 2023-06-22 15:35:41.974158 datamatrix-1.0.4/datamatrix/convert/_mne.py
+-rw-r--r--   0        0        0     3849 2023-06-22 15:35:41.974158 datamatrix-1.0.4/datamatrix/convert/_pandas.py
+-rw-r--r--   0        0        0    13989 2023-06-22 15:35:41.974158 datamatrix-1.0.4/datamatrix/functional.py
+-rw-r--r--   0        0        0     1003 2023-06-22 15:35:41.974158 datamatrix-1.0.4/datamatrix/io/__init__.py
+-rw-r--r--   0        0        0     5510 2023-06-22 15:35:41.974158 datamatrix-1.0.4/datamatrix/io/_bin.py
+-rw-r--r--   0        0        0     4565 2023-06-22 15:35:41.974158 datamatrix-1.0.4/datamatrix/io/_excel.py
+-rw-r--r--   0        0        0     2807 2023-06-22 15:35:41.974158 datamatrix-1.0.4/datamatrix/io/_pickle.py
+-rw-r--r--   0        0        0     3318 2023-06-22 15:35:41.974158 datamatrix-1.0.4/datamatrix/io/_text.py
+-rw-r--r--   0        0        0     1412 2023-06-22 15:35:41.974158 datamatrix-1.0.4/datamatrix/monkeypatch.py
+-rw-r--r--   0        0        0     7822 2023-06-22 15:35:41.974158 datamatrix-1.0.4/datamatrix/multidimensional.py
+-rw-r--r--   0        0        0    29729 2023-06-22 15:35:41.974158 datamatrix-1.0.4/datamatrix/operations.py
+-rw-r--r--   0        0        0     4205 2023-06-22 15:35:41.974158 datamatrix-1.0.4/datamatrix/plot.py
+-rw-r--r--   0        0        0     3125 2023-06-22 15:35:41.974158 datamatrix-1.0.4/datamatrix/py3compat.py
+-rw-r--r--   0        0        0     1059 2023-06-22 15:35:41.974158 datamatrix-1.0.4/datamatrix/rbridge/__init__.py
+-rw-r--r--   0        0        0     4422 2023-06-22 15:35:41.974158 datamatrix-1.0.4/datamatrix/rbridge/lme4.py
+-rw-r--r--   0        0        0    53892 2023-06-22 15:35:41.974158 datamatrix-1.0.4/datamatrix/series.py
+-rw-r--r--   0        0        0      834 2023-06-22 15:35:42.406161 datamatrix-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     5859 2023-06-22 15:35:42.406161 datamatrix-1.0.4/readme.md
+-rw-r--r--   0        0        0     6410 1970-01-01 00:00:00.000000 datamatrix-1.0.4/PKG-INFO
```

### Comparing `datamatrix-1.0.2/COPYING` & `datamatrix-1.0.4/COPYING`

 * *Files identical despite different names*

### Comparing `datamatrix-1.0.2/datamatrix/__init__.py` & `datamatrix-1.0.4/datamatrix/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,10 +24,10 @@
 from datamatrix._datamatrix._numericcolumn import FloatColumn, IntColumn
 from datamatrix._datamatrix._seriescolumn import SeriesColumn
 from datamatrix._datamatrix._multidimensionalcolumn import \
     MultiDimensionalColumn
 from datamatrix._datamatrix._nifticolumn import NiftiColumn
 from datamatrix._datamatrix._datamatrix import DataMatrix
 
-__version__ = '1.0.2'
+__version__ = '1.0.4'
 NAN = float('nan')
 INF = float('inf')
```

### Comparing `datamatrix-1.0.2/datamatrix/_config.py` & `datamatrix-1.0.4/datamatrix/_config.py`

 * *Files identical despite different names*

### Comparing `datamatrix-1.0.2/datamatrix/_datamatrix/__init__.py` & `datamatrix-1.0.4/datamatrix/_datamatrix/__init__.py`

 * *Files identical despite different names*

### Comparing `datamatrix-1.0.2/datamatrix/_datamatrix/_basecolumn.py` & `datamatrix-1.0.4/datamatrix/_datamatrix/_basecolumn.py`

 * *Files 0% similar despite different names*

```diff
@@ -580,30 +580,30 @@
             key:	A DataMatrix
         """
 
         if key != self._datamatrix:
             raise ValueError('Cannot slice column with a different DataMatrix')
         return self[[self._rowid.index(_rowid) for _rowid in key._rowid]]
 
-    def _getrowidkey(self, key):
+    def _getrowidkey(self, key, dm=None):
 
         """
         visible: False
 
         desc:
             Gets a slice of this column by a list of row ids.
 
         arguments:
             key:	A list of row ids.
 
         returns:
             BaseColunn
         """
         seq = [self._seq[self._rowid.index(_rowid)] for _rowid in key]
-        return self._empty_col(rowid=key, seq=seq)
+        return self._empty_col(rowid=key, seq=seq, datamatrix=dm)
         
     def _sortedrowid(self):
 
         """
         visible: False
 
         desc:
```

### Comparing `datamatrix-1.0.2/datamatrix/_datamatrix/_blinkreconstruct.py` & `datamatrix-1.0.4/datamatrix/_datamatrix/_blinkreconstruct.py`

 * *Files identical despite different names*

### Comparing `datamatrix-1.0.2/datamatrix/_datamatrix/_callable_values.py` & `datamatrix-1.0.4/datamatrix/_datamatrix/_callable_values.py`

 * *Files identical despite different names*

### Comparing `datamatrix-1.0.2/datamatrix/_datamatrix/_datamatrix.py` & `datamatrix-1.0.4/datamatrix/_datamatrix/_datamatrix.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 """
 
 from datamatrix.py3compat import *
 from datamatrix import Row
 from datamatrix._datamatrix._basecolumn import BaseColumn
 from datamatrix._datamatrix._mixedcolumn import MixedColumn
 from datamatrix._datamatrix._index import Index
+from datamatrix._datamatrix._uninstantiatedcolumn import UninstantiatedColumn
 from datamatrix._ordered_state import OrderedState
 try:
     from collections.abc import Sequence  # Python 3.3 and later
 except ImportError:
     from collections import Sequence
 try:
     import numpy as np
@@ -127,14 +128,15 @@
         elif default_col_type == int:
             from datamatrix import IntColumn
             default_col_type = IntColumn
         object.__setattr__(self, u'_default_col_type', default_col_type)
         object.__setattr__(self, u'_id', _id)
         object.__setattr__(self, u'_sorted', True)
         object.__setattr__(self, u'metadata', metadata)
+        object.__setattr__(self, u'_instantiate_on_select', True)
         _id += 1
         for column_name, val in columns.items():
             self[column_name] = val
         # If a dict was provided, initialize the datamatrix
         if init_dict is not None:
             self._fromdict(init_dict)
 
@@ -147,14 +149,15 @@
     def empty(self):
         
         return not len(self) or not len(self._cols)
 
     @property
     def columns(self):
 
+        self._instantiate()
         return self._to_list(self._cols.items(), key=lambda col: col[0])
 
     @property
     def column_names(self):
 
         return self._to_list(self._cols.keys())
 
@@ -301,15 +304,25 @@
             type:	DataMatrix.
         """
 
         dm = DataMatrix(len(_rowid))
         object.__setattr__(dm, u'_rowid', _rowid)
         object.__setattr__(dm, u'_id', self._id)
         for name, col in self._cols.items():
-            dm._cols[name] = self._cols[name]._getrowidkey(_rowid)
+            # By default we create new columns with a copy of the selected data 
+            if not hasattr(self, '_instantiate_on_select') or \
+                    self._instantiate_on_select:
+                self._instantiate_column(name)
+                dm._cols[name] = self._cols[name]._getrowidkey(_rowid, dm)
+            # Except when _instatiate_on_select is set to False, in which case
+            # we create an UninstantiatedColumn object which can be turned into
+            # an actual column when it is requested in _getcolbyname()
+            else:
+                dm._cols[name] = UninstantiatedColumn(
+                    name, self._cols[name], _rowid, dm)
             dm._cols[name]._datamatrix = dm
         return dm
 
     def _slice(self, key):
 
         """
         visible: False
@@ -321,14 +334,15 @@
         arguments:
             key:		A slice object, or a list of indices.
 
         returns:
             type:	DataMatrix.
         """
 
+        self._instantiate()
         # A tuple of length two is interpreted by a SeriesColumn as a sample
         # and row. Therefore, we turn tuples into lists.
         if isinstance(key, tuple):
             key = list(key)
         _rowid = self._rowid[key]
         dm = DataMatrix(len(_rowid))
         object.__setattr__(dm, u'_rowid', _rowid)
@@ -357,15 +371,15 @@
             ~~~
 
         arguments:
             value:
                 desc:	The new length.
                 type:	int
         """
-
+        self._instantiate()
         if value < len(self):
             object.__setattr__(self, u'_rowid', self._rowid[:value])
             for name, col in self._cols.items():
                 self._cols[name] = self._cols[name][:value]
         else:
             startid = 0 if not len(self) else self._rowid.max+1
             rowid = Index([i+startid for i in range(value-len(self))])
@@ -405,15 +419,15 @@
         arguments:
             other:	Another DataMatrix.
             _rowid:	A list of row ids.
 
         returns:
             type:	DataMatrix.
         """
-
+        self._instantiate()
         if self != other:
             raise Exception('Can only merge related datamatrices')
         dm = DataMatrix(len(_rowid))
         object.__setattr__(dm, u'_rowid', _rowid)
         object.__setattr__(dm, u'_id', self._id)
         for name, col in self._cols.items():
             dm._cols[name] = self._cols[name]._merge(other._cols[name], _rowid)
@@ -476,15 +490,15 @@
         arguments:
             key:
                 type:	BaseColumn
 
         returns:
             type:	BaseColumn
         """
-
+        self._instantiate()
         for col in self._cols.values():
             if col is key:
                 return col
         raise Exception('Column not found')
 
     def _getcolbyname(self, key):
 
@@ -503,15 +517,15 @@
         """
 
         if isinstance(key, bytes):
             key = safe_decode(key)
         col = self._cols.get(key, None)
         if col is None:
             raise AttributeError(u'No column named "%s"' % key)
-        return col
+        return self._instantiate_column(key, col)
 
     def _getrow(self, key):
 
         """
         visible: False
 
         desc:
@@ -790,14 +804,15 @@
             return self._slice(key)
         if isinstance(key, DataMatrix):
             return self._where(key)
         raise KeyError('Invalid key, index, or slice: %s' % key)
 
     def __str__(self):
 
+        self._instantiate()
         if len(self) > PRINT_MAX_ROWS:
             return str(self[:PRINT_MAX_ROWS]) + u'\n(+ %d rows not shown)' \
                 % (len(self) - PRINT_MAX_ROWS)
         import prettytable
         t = prettytable.PrettyTable()
         t.add_column('#', self._rowid)
         for name, col in list(self.columns)[:PRINT_MAX_COLUMNS]:
@@ -851,14 +866,15 @@
             Use by numpy to convert the DataMatrix to an array where the first
             axis corresponds to the rows and the second axis to the columns.
             The dtype of the array is object, float, or int, depending on which
             dtype fits best.
         """
         
         import numpy as np
+        self._instantiate()
         a = np.empty((len(self), len(self.columns)), dtype=object)
         for i, col in enumerate(self._cols.values()):
             if hasattr(col, 'depth'):
                 for j, row in enumerate(col):
                     a[j, i] = row
             else:
                 a[:, i] = col
@@ -872,7 +888,26 @@
         return a
 
     def __dataframe__(self):
         
         from datamatrix import convert as cnv
         
         return cnv.to_pandas(self)
+
+    def _instantiate(self):
+        """Instantiates all uninstantiated columns"""
+        for name, col in self._cols.items():
+            if isinstance(col, UninstantiatedColumn):
+                col = col.instantiate()
+                self._cols[name] = col
+
+    def _instantiate_column(self, key, col=None):
+        """Makes sure that a specific column is instantiated, and returns the
+        instantiated column.
+        """
+        if col is None:
+            col = self._cols[key]
+        if not isinstance(col, UninstantiatedColumn):
+            return col
+        col = col.instantiate()
+        self._cols[key] = col
+        return col
```

### Comparing `datamatrix-1.0.2/datamatrix/_datamatrix/_index.py` & `datamatrix-1.0.4/datamatrix/_datamatrix/_index.py`

 * *Files identical despite different names*

### Comparing `datamatrix-1.0.2/datamatrix/_datamatrix/_mixedcolumn.py` & `datamatrix-1.0.4/datamatrix/_datamatrix/_mixedcolumn.py`

 * *Files identical despite different names*

### Comparing `datamatrix-1.0.2/datamatrix/_datamatrix/_multidimensionalcolumn.py` & `datamatrix-1.0.4/datamatrix/_datamatrix/_multidimensionalcolumn.py`

 * *Files identical despite different names*

### Comparing `datamatrix-1.0.2/datamatrix/_datamatrix/_nifticolumn.py` & `datamatrix-1.0.4/datamatrix/_datamatrix/_nifticolumn.py`

 * *Files identical despite different names*

### Comparing `datamatrix-1.0.2/datamatrix/_datamatrix/_numericcolumn.py` & `datamatrix-1.0.4/datamatrix/_datamatrix/_numericcolumn.py`

 * *Files 0% similar despite different names*

```diff
@@ -220,15 +220,15 @@
             raise ValueError('Cannot slice column with a different DataMatrix')
         return self._getrowidkey(key._rowid)
 
     def _getintkey(self, key):
 
         return self.dtype(self._seq[key])
 
-    def _getrowidkey(self, key):
+    def _getrowidkey(self, key, dm=None):
 
         if isinstance(key, Index):
             key = key._a
         # argsort and searchsorted are fairly time-consuming operations which
         # need to be performed very often. Therefore we implement a crude
         # but fast caching mechanism.
         global rowid_argsort_cache, selected_indices_cache
@@ -245,17 +245,16 @@
         if key_hash != selected_indices_cache[0]:
             matching_indices = np.searchsorted(self._rowid[orig_indices], key)
             selected_indices = orig_indices[matching_indices]
             selected_indices_cache = key_hash, selected_indices
         else:
             selected_indices = selected_indices_cache[1]
         return self._empty_col(rowid=self._rowid[selected_indices],
-                               seq=self._seq[selected_indices])
-            
-        
+                               seq=self._seq[selected_indices],
+                               datamatrix=dm)
 
     def _setdatamatrixkey(self, key, val):
 
         if key != self._datamatrix:
             raise ValueError('Cannot slice column with a different DataMatrix')
         self._seq[np.searchsorted(self._rowid, key._rowid)] = val
```

### Comparing `datamatrix-1.0.2/datamatrix/_datamatrix/_row.py` & `datamatrix-1.0.4/datamatrix/_datamatrix/_row.py`

 * *Files identical despite different names*

### Comparing `datamatrix-1.0.2/datamatrix/_datamatrix/_seriescolumn.py` & `datamatrix-1.0.4/datamatrix/_datamatrix/_seriescolumn.py`

 * *Files identical despite different names*

### Comparing `datamatrix-1.0.2/datamatrix/_datamatrix/_sort.py` & `datamatrix-1.0.4/datamatrix/_datamatrix/_sort.py`

 * *Files identical despite different names*

### Comparing `datamatrix-1.0.2/datamatrix/_functional/__init__.py` & `datamatrix-1.0.4/datamatrix/_functional/__init__.py`

 * *Files identical despite different names*

### Comparing `datamatrix-1.0.2/datamatrix/_functional/_memoize.py` & `datamatrix-1.0.4/datamatrix/_functional/_memoize.py`

 * *Files identical despite different names*

### Comparing `datamatrix-1.0.2/datamatrix/_ordered_state.py` & `datamatrix-1.0.4/datamatrix/_ordered_state.py`

 * *Files identical despite different names*

### Comparing `datamatrix-1.0.2/datamatrix/colors/__init__.py` & `datamatrix-1.0.4/datamatrix/colors/__init__.py`

 * *Files identical despite different names*

### Comparing `datamatrix-1.0.2/datamatrix/colors/tango.py` & `datamatrix-1.0.4/datamatrix/colors/tango.py`

 * *Files identical despite different names*

### Comparing `datamatrix-1.0.2/datamatrix/convert/__init__.py` & `datamatrix-1.0.4/datamatrix/convert/__init__.py`

 * *Files identical despite different names*

### Comparing `datamatrix-1.0.2/datamatrix/convert/_html.py` & `datamatrix-1.0.4/datamatrix/convert/_html.py`

 * *Files identical despite different names*

### Comparing `datamatrix-1.0.2/datamatrix/convert/_json.py` & `datamatrix-1.0.4/datamatrix/convert/_json.py`

 * *Files identical despite different names*

### Comparing `datamatrix-1.0.2/datamatrix/convert/_mne.py` & `datamatrix-1.0.4/datamatrix/convert/_mne.py`

 * *Files identical despite different names*

### Comparing `datamatrix-1.0.2/datamatrix/convert/_pandas.py` & `datamatrix-1.0.4/datamatrix/convert/_pandas.py`

 * *Files identical despite different names*

### Comparing `datamatrix-1.0.2/datamatrix/functional.py` & `datamatrix-1.0.4/datamatrix/functional.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 try:
     from inspect import getfullargspec as getargspec  # Python 3.0 and later
 except ImportError:
     from inspect import getargspec
 import functools
 import logging
+import os
 from contextlib import contextmanager
 from datamatrix.py3compat import *
 from datamatrix import DataMatrix, cfg
 from datamatrix._datamatrix._basecolumn import BaseColumn
 from datamatrix._datamatrix._index import Index
 from datamatrix._functional._memoize import memoize
 logger = logging.getLogger('datamatrix')
@@ -97,14 +98,17 @@
         
         See also:
         
         - <https://docs.python.org/3/library/multiprocessing.html>
         - %link:operations%#function-stack
         
         *Version note:* New in 1.0.0.
+        
+        *Version note:* As of 1.0.4, if one of the processes crashes, and error
+        is shown with the Exception, but the main process doesn't crash.
 
         __Example:__
 
         ```python
         from datamatrix import DataMatrix, functional as fnc
         
         def get_dm(i):
@@ -135,27 +139,35 @@
         returns:
             type: `DataMatrix`
     """
     import multiprocessing as mp
     from datamatrix import io, operations as ops
     
     logger.debug('starting multiprocessing')
-    with mp.Pool(processes) as pool:
-        results = pool.map(functools.partial(_stack_multiprocess_inner, fnc),
-                           args)
-        logger.debug('received {} DataMatrix objects'.format(len(results)))
+    pool = mp.Pool(processes)
+    fnc = functools.partial(_stack_multiprocess_inner, fnc)
+    results = [pool.apply_async(fnc, (arg,)) for arg in args]
+    paths = []
+    for result in results:
+        try:
+            path = result.get()
+        except Exception as e:
+            logger.error(f'a process failed with the following exception: {e}')
+        else:
+            paths.append(path)
+    logger.debug('received {} DataMatrix objects'.format(len(paths)))
     # The return values consist of path objects that refer to temporary
     # binary datamatrix files. We read these files, stack them, and then
     # delete them.
     try:
-        dm = ops.stack([io.readbin(path) for path in results])
+        dm = ops.stack([io.readbin(path) for path in paths])
     except Exception as e:
         raise
     finally:
-        for path in results:
+        for path in paths:
             try:
                 path.unlink()
             except Exception as e:
                 logger.warning(
                     'failed to remove temporary file: {}'.format(path))
     return dm
 
@@ -413,16 +425,19 @@
 def _stack_multiprocess_inner(fnc, arg):
     """A helper function for stack_multiprocess that calls another function,
     ensures that the result value is a DataMatrix, saves the DataMatrix to 
     disk, and then returns the path to the saved file.
     """
     from pathlib import Path
     from datamatrix import io
+    import gc
     
     dm = fnc(arg)
     if not isinstance(dm, DataMatrix):
         raise ValueError('function should return DataMatrix, not {}'
                          .format(type(dm)))
-    path = Path(cfg.tmp_dir) / Path('.{}.dm'.format(id(dm)))
+    path = Path(cfg.tmp_dir) / Path(f'.{id(dm)}-{os.getpid()}.dm')
     logger.info('writing process result to temporary file {}'.format(path))
     io.writebin(dm, path)
+    del dm
+    gc.collect()
     return path
```

### Comparing `datamatrix-1.0.2/datamatrix/io/__init__.py` & `datamatrix-1.0.4/datamatrix/io/__init__.py`

 * *Files identical despite different names*

### Comparing `datamatrix-1.0.2/datamatrix/io/_bin.py` & `datamatrix-1.0.4/datamatrix/io/_bin.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 """
 
 from datamatrix.py3compat import *
 from datamatrix import cfg
 from datamatrix._datamatrix._multidimensionalcolumn import \
     _MultiDimensionalColumn
 from datamatrix.io._pickle import readpickle, writepickle
+import os
 import logging
 import tarfile
 from pathlib import Path
 try:
     import numpy as np
 except ImportError:
     np = None
@@ -56,38 +57,45 @@
     if np is None:
         raise Exception(
             'NumPy and SciPy are required, but not installed.')
     if not isinstance(path, Path):
         path = Path(path)
     logger.debug('reading binary file from {}'.format(path))
     tar = tarfile.open(path, 'r:gz')
+    # Extracte to a temporary folder that is based on the pid of the current
+    # process. This avoids races conditions if multiple processes are reading
+    # from the same file
+    tmp_dir = Path(cfg.tmp_dir) / f'.{os.getpid()}'
+    if not tmp_dir.exists():
+        tmp_dir.mkdir()
     for member in tar.getmembers():
-        dm_path = Path(member.name)
+        dm_path = tmp_dir / Path(member.name)
         if dm_path.suffix == '.datamatrix':
             logger.debug('reading datamatrix pickle from {}'.format(dm_path))
-            tar.extract(member, path=cfg.tmp_dir)
-            dm = readpickle(Path(cfg.tmp_dir) / dm_path)
+            tar.extract(member, path=str(tmp_dir))
+            dm = readpickle(tmp_dir / dm_path)
             dm_path.unlink()
             break
     else:
         raise TypeError('{} is not a binary datamatrix file'.format(path))
     for col in dm._cols.values():
         if not isinstance(col, _MultiDimensionalColumn) or col.loaded:
             continue
         aux_path = col._seq
         logger.debug('reading auxiliary file: {}'.format(aux_path))
-        tar.extract(tar.getmember(str(aux_path)), path=cfg.tmp_dir)
+        tar.extract(tar.getmember(str(aux_path)), path=str(tmp_dir))
         col._init_seq()
         chunk_slice = int(cfg.save_chunk_size / col._memory_size() * len(col))
-        tmp_path = Path(cfg.tmp_dir) / aux_path
+        tmp_path = tmp_dir / aux_path
         with tmp_path.open('rb+') as fd:
             a = np.memmap(fd, mode='r', shape=col.shape, dtype=col.dtype)
             for i in range(0, len(col), chunk_slice):
                 col._seq[i:i + chunk_slice] = a[i:i + chunk_slice]
         tmp_path.unlink()
+    tmp_dir.rmdir()
     return dm
 
 
 def writebin(dm, path):
     """
     desc: |
         Reads a DataMatrix to a binary file. This format allows you to read
@@ -117,28 +125,28 @@
     # We first write all data from unloaded MultiDimensionalColumns to
     # separate files. The _seq and _fd properties are temporarily removed from
     # the columns so that the datamatrix can be pickled.
     tmp = {}
     for col in dm._cols.values():
         if not isinstance(col, _MultiDimensionalColumn) or col.loaded:
             continue
-        aux_path = path.parent / Path('.{}.memmap'.format(id(col)))
+        aux_path = path.parent / Path(f'.{id(col)}-{os.getpid()}.memmap')
         logger.debug('writing auxiliary file: {}'.format(aux_path))
         chunk_slice = int(cfg.save_chunk_size / col._memory_size() * len(col))
         with aux_path.open('wb+') as fd:
             a = np.memmap(fd, mode='w+', shape=col.shape, dtype=col.dtype)
             for i in range(0, len(col), chunk_slice):
                 a[i:i + chunk_slice] = col._seq[i:i + chunk_slice]
         tmp[id(col)] = col._fd, col._seq
         col._fd = None
         object.__setattr__(col, '_seq' , aux_path.name)
         tar.add(aux_path, arcname=aux_path.name)
         aux_path.unlink()
     # The datamatrix can now be safely pickled
-    dm_path = path.parent / Path('.{}.datamatrix'.format(id(dm)))
+    dm_path = path.parent / Path(f'.{id(dm)}-{os.getpid()}.datamatrix')
     logger.debug('writing datamatrix pickle to {}'.format(dm_path))
     writepickle(dm, dm_path)
     tar.add(dm_path, arcname=dm_path.name)
     tar.close()
     dm_path.unlink()
     # The _seq and _fd properties can be restored again
     for col in dm._cols.values():
```

### Comparing `datamatrix-1.0.2/datamatrix/io/_excel.py` & `datamatrix-1.0.4/datamatrix/io/_excel.py`

 * *Files identical despite different names*

### Comparing `datamatrix-1.0.2/datamatrix/io/_pickle.py` & `datamatrix-1.0.4/datamatrix/io/_pickle.py`

 * *Files identical despite different names*

### Comparing `datamatrix-1.0.2/datamatrix/io/_text.py` & `datamatrix-1.0.4/datamatrix/io/_text.py`

 * *Files identical despite different names*

### Comparing `datamatrix-1.0.2/datamatrix/monkeypatch.py` & `datamatrix-1.0.4/datamatrix/monkeypatch.py`

 * *Files identical despite different names*

### Comparing `datamatrix-1.0.2/datamatrix/multidimensional.py` & `datamatrix-1.0.4/datamatrix/multidimensional.py`

 * *Files identical despite different names*

### Comparing `datamatrix-1.0.2/datamatrix/operations.py` & `datamatrix-1.0.4/datamatrix/operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,14 +101,15 @@
         elif not isinstance(dm, DataMatrix):
             raise TypeError(
                 'Expecting DataMatrix, dict, or Row, not {}'.format(type(dm)))
         new_length += len(dms[i])
     start_index = 0
     dm = DataMatrix(length=new_length)
     for stackdm in dms:
+        stackdm._instantiate()
         for name, col in stackdm._cols.items():
             if name not in dm._cols:
                 if isinstance(col, _MultiDimensionalColumn):
                     dm[name] = col.__class__(dm, shape=col._orig_shape,
                                              defaultnan=col.defaultnan,
                                              metadata=col.metadata)
                 else:
@@ -423,15 +424,22 @@
             for val_sdm in split(*[dm[col.name] for col in values]):
                 yield (val1,) + tuple(val_sdm)
         return
     # Otherwise we determine the number of unique values, or use the values
     # that are passed to the function
     _values = values if values else col.unique
     for val in _values:
+        # Setting this flag tells the datamatrix to not copy all columns, but
+        # rather to create UninstiatedColumn objects which are turned into
+        # actual columns only when they are requested. This is much faster and
+        # saves memory in cases where a large datamatrix is split but most
+        # columns are never actually used in the splitted datamatrix objects.
+        object.__setattr__(col._datamatrix, '_instantiate_on_select', False)
         dm = col == val
+        object.__setattr__(col._datamatrix, '_instantiate_on_select', True)
         if not dm:
             warn(u'No matching rows for %s' % val)
         if values:
             yield dm
         else:
             yield val, dm
```

### Comparing `datamatrix-1.0.2/datamatrix/plot.py` & `datamatrix-1.0.4/datamatrix/plot.py`

 * *Files identical despite different names*

### Comparing `datamatrix-1.0.2/datamatrix/py3compat.py` & `datamatrix-1.0.4/datamatrix/py3compat.py`

 * *Files identical despite different names*

### Comparing `datamatrix-1.0.2/datamatrix/rbridge/__init__.py` & `datamatrix-1.0.4/datamatrix/rbridge/__init__.py`

 * *Files identical despite different names*

### Comparing `datamatrix-1.0.2/datamatrix/rbridge/lme4.py` & `datamatrix-1.0.4/datamatrix/rbridge/lme4.py`

 * *Files identical despite different names*

### Comparing `datamatrix-1.0.2/datamatrix/series.py` & `datamatrix-1.0.4/datamatrix/series.py`

 * *Files identical despite different names*

### Comparing `datamatrix-1.0.2/pyproject.toml` & `datamatrix-1.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datamatrix-1.0.2/readme.md` & `datamatrix-1.0.4/readme.md`

 * *Files identical despite different names*

### Comparing `datamatrix-1.0.2/PKG-INFO` & `datamatrix-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamatrix
-Version: 1.0.2
+Version: 1.0.4
 Summary: This file is part of datamatrix.
 Keywords: data analysis,scientific software,time series
 Author-email: Sebastiaan Mathôt <s.mathot@cogsci.nl>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: scipy
```

