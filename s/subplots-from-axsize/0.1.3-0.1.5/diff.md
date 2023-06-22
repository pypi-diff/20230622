# Comparing `tmp/subplots_from_axsize-0.1.3.tar.gz` & `tmp/subplots_from_axsize-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subplots_from_axsize-0.1.3.tar", max compression
+gzip compressed data, was "subplots_from_axsize-0.1.5.tar", max compression
```

## Comparing `subplots_from_axsize-0.1.3.tar` & `subplots_from_axsize-0.1.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1505 2023-06-15 13:41:52.549659 subplots_from_axsize-0.1.3/LICENSE
--rw-r--r--   0        0        0       77 2023-06-17 17:56:09.932773 subplots_from_axsize-0.1.3/README.md
--rw-r--r--   0        0        0      394 2023-06-20 21:28:01.922554 subplots_from_axsize-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       76 2023-06-15 14:07:27.491712 subplots_from_axsize-0.1.3/src/subplots_from_axsize/__init__.py
--rw-r--r--   0        0        0     3221 2023-06-20 21:28:49.176177 subplots_from_axsize-0.1.3/src/subplots_from_axsize/_subplots_from_axsize.py
--rw-r--r--   0        0        0      619 1970-01-01 00:00:00.000000 subplots_from_axsize-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1505 2023-06-15 13:41:52.549659 subplots_from_axsize-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1934 2023-06-22 13:28:27.287169 subplots_from_axsize-0.1.5/README.md
+-rw-r--r--   0        0        0      432 2023-06-22 13:28:39.733960 subplots_from_axsize-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       76 2023-06-15 14:07:27.491712 subplots_from_axsize-0.1.5/src/subplots_from_axsize/__init__.py
+-rw-r--r--   0        0        0     3229 2023-06-20 21:35:21.638348 subplots_from_axsize-0.1.5/src/subplots_from_axsize/_subplots_from_axsize.py
+-rw-r--r--   0        0        0     2437 1970-01-01 00:00:00.000000 subplots_from_axsize-0.1.5/PKG-INFO
```

### Comparing `subplots_from_axsize-0.1.3/LICENSE` & `subplots_from_axsize-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `subplots_from_axsize-0.1.3/src/subplots_from_axsize/_subplots_from_axsize.py` & `subplots_from_axsize-0.1.5/src/subplots_from_axsize/_subplots_from_axsize.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,20 +61,21 @@
     return sizes, sum(ds)
 
 
 def subplots_from_axsize(
     nrows: Optional[int] = None,
     ncols: Optional[int] = None,
     axsize: Tuple[Union[float, list[float]], Union[float, list[float]]] = (4, 3),
-    top: float = 0.1,
-    bottom: float = 0.5,
+    *,
     left: float = 0.6,
+    bottom: float = 0.5,
     right: float = 0.2,
+    top: float = 0.1,
+    wspace: Union[float, list[float]] = 0.75,
     hspace: Union[float, list[float]] = 0.5,
-    wspace: Union[float, list[float]] = 0.5,
     squeeze: bool = True,
 ):
     """
     Similar to plt.subplots() but uses fixed instead of relative sizes.
     This allows for more control over the final axes sizes.
 
     Examples:
@@ -82,16 +83,16 @@
     fig, axs = subplots_from_axsize(axsize=(3, [2, 1])) creates a figure with two axes: (3, 2) and (3, 1)
     """
     axx, axy = axsize
 
     # standardize types
     axx = _list_or_float(axx)
     axy = _list_or_float(axy)
-    hspace = _list_or_float(hspace)
     wspace = _list_or_float(wspace)
+    hspace = _list_or_float(hspace)
 
     # make sure counts agree and convert to lists
     ncols, axx, wspace = _sync_counts(ncols, axx, wspace, "col")
     nrows, axy, hspace = _sync_counts(nrows, axy, hspace, "row")
 
     w_sizes, total_w = _make_sizes(left, axx, right, wspace)
     h_sizes, total_h = _make_sizes(top, axy, bottom, hspace)
```

