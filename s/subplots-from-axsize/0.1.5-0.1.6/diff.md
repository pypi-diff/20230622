# Comparing `tmp/subplots_from_axsize-0.1.5.tar.gz` & `tmp/subplots_from_axsize-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subplots_from_axsize-0.1.5.tar", max compression
+gzip compressed data, was "subplots_from_axsize-0.1.6.tar", max compression
```

## Comparing `subplots_from_axsize-0.1.5.tar` & `subplots_from_axsize-0.1.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1505 2023-06-15 13:41:52.549659 subplots_from_axsize-0.1.5/LICENSE
--rw-r--r--   0        0        0     1934 2023-06-22 13:28:27.287169 subplots_from_axsize-0.1.5/README.md
--rw-r--r--   0        0        0      432 2023-06-22 13:28:39.733960 subplots_from_axsize-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       76 2023-06-15 14:07:27.491712 subplots_from_axsize-0.1.5/src/subplots_from_axsize/__init__.py
--rw-r--r--   0        0        0     3229 2023-06-20 21:35:21.638348 subplots_from_axsize-0.1.5/src/subplots_from_axsize/_subplots_from_axsize.py
--rw-r--r--   0        0        0     2437 1970-01-01 00:00:00.000000 subplots_from_axsize-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1505 2023-06-15 13:41:52.549659 subplots_from_axsize-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1934 2023-06-22 13:28:27.287169 subplots_from_axsize-0.1.6/README.md
+-rw-r--r--   0        0        0      474 2023-06-22 13:43:49.615052 subplots_from_axsize-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0       76 2023-06-15 14:07:27.491712 subplots_from_axsize-0.1.6/src/subplots_from_axsize/__init__.py
+-rw-r--r--   0        0        0     4156 2023-06-22 13:46:07.676267 subplots_from_axsize-0.1.6/src/subplots_from_axsize/_subplots_from_axsize.py
+-rw-r--r--   0        0        0     2437 1970-01-01 00:00:00.000000 subplots_from_axsize-0.1.6/PKG-INFO
```

### Comparing `subplots_from_axsize-0.1.5/LICENSE` & `subplots_from_axsize-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `subplots_from_axsize-0.1.5/README.md` & `subplots_from_axsize-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `subplots_from_axsize-0.1.5/src/subplots_from_axsize/_subplots_from_axsize.py` & `subplots_from_axsize-0.1.6/src/subplots_from_axsize/_subplots_from_axsize.py`

 * *Files 17% similar despite different names*

```diff
@@ -71,21 +71,48 @@
     right: float = 0.2,
     top: float = 0.1,
     wspace: Union[float, list[float]] = 0.75,
     hspace: Union[float, list[float]] = 0.5,
     squeeze: bool = True,
 ):
     """
-    Similar to plt.subplots() but uses fixed instead of relative sizes.
+    Similar to plt.subplots() but uses fixed sizes (inches) instead of fractions.
     This allows for more control over the final axes sizes.
 
-    Examples:
+    Parameters
+    ----------
+    nrows, ncols : int, optional, default: None
+        Number of rows/columns of the subplot grid.
+
+    axsize : tuple of sizes, default: (3, 4)
+        Each size can be either a float or list of floats (inches).
+        If either entry is a list, it will be used to determine `nrows`/`ncols`.
+
+    left, bottom, right, top : floats, defaults: 0.6, 0.5, 0.2, 0.1
+        Specify figure margins (in inches).
+
+    wspace, hspace : sizes, defaults: 0.75, 0.5
+        Each size can be either a float or list of floats (inches).
+        If either entry is a list, it will be used to determine `nrows`/`ncols`.
+
+    squeeze : bool, default: True
+        If True, returns `axs` like subplots, by removing array axes with length 1.
+        If False, always returns an array of axes with shape ``(nrows, ncols)`.
+
+    Returns
+    -------
+        fig, axs : same as plt.subplots()
+
+    Examples
+    --------
     fig, axs = subplots_from_axsize(axsize=(3, 2), nrows=2) creates a figure with two axes of size (3, 2)
     fig, axs = subplots_from_axsize(axsize=(3, [2, 1])) creates a figure with two axes: (3, 2) and (3, 1)
+
     """
+
     axx, axy = axsize
 
     # standardize types
     axx = _list_or_float(axx)
     axy = _list_or_float(axy)
     wspace = _list_or_float(wspace)
     hspace = _list_or_float(hspace)
```

### Comparing `subplots_from_axsize-0.1.5/PKG-INFO` & `subplots_from_axsize-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: subplots-from-axsize
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: Frederic Grabowski
 Author-email: grabowski.frederic@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

