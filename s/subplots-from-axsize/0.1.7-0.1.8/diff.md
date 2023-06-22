# Comparing `tmp/subplots_from_axsize-0.1.7.tar.gz` & `tmp/subplots_from_axsize-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subplots_from_axsize-0.1.7.tar", max compression
+gzip compressed data, was "subplots_from_axsize-0.1.8.tar", max compression
```

## Comparing `subplots_from_axsize-0.1.7.tar` & `subplots_from_axsize-0.1.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1505 2023-06-15 13:41:52.549659 subplots_from_axsize-0.1.7/LICENSE
--rw-r--r--   0        0        0     1934 2023-06-22 13:28:27.287169 subplots_from_axsize-0.1.7/README.md
--rw-r--r--   0        0        0      474 2023-06-22 14:03:27.055953 subplots_from_axsize-0.1.7/pyproject.toml
--rw-r--r--   0        0        0       76 2023-06-15 14:07:27.491712 subplots_from_axsize-0.1.7/src/subplots_from_axsize/__init__.py
--rw-r--r--   0        0        0     4505 2023-06-22 14:03:18.152535 subplots_from_axsize-0.1.7/src/subplots_from_axsize/_subplots_from_axsize.py
--rw-r--r--   0        0        0     2437 1970-01-01 00:00:00.000000 subplots_from_axsize-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1505 2023-06-15 13:41:52.549659 subplots_from_axsize-0.1.8/LICENSE
+-rw-r--r--   0        0        0     2367 2023-06-22 18:00:31.269873 subplots_from_axsize-0.1.8/README.md
+-rw-r--r--   0        0        0      474 2023-06-22 18:03:21.920053 subplots_from_axsize-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0       76 2023-06-15 14:07:27.491712 subplots_from_axsize-0.1.8/src/subplots_from_axsize/__init__.py
+-rw-r--r--   0        0        0     4583 2023-06-22 18:02:49.932706 subplots_from_axsize-0.1.8/src/subplots_from_axsize/_subplots_from_axsize.py
+-rw-r--r--   0        0        0     2870 1970-01-01 00:00:00.000000 subplots_from_axsize-0.1.8/PKG-INFO
```

### Comparing `subplots_from_axsize-0.1.7/LICENSE` & `subplots_from_axsize-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `subplots_from_axsize-0.1.7/README.md` & `subplots_from_axsize-0.1.8/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 ## subplots_from_axsize
 This package provides a single function, `subplots_from_axsize()`, which is based on matplotlib's `subplots()` and `adjust_subplots()` functions, but:
 * `figsize` is replaced by `axsize`
 * `left`, `bottom`, `right`, `top` use inches instead of fractions
 * `wspace`, `hspace` use inches instead of fractions
 * `axsize`, `wspace`, `hspace` can take lists as arguments (see example #2 below)
 
+## rationale
+Specifying sizes directly makes it easier to achieve consistent ax sizes across figures. Suppose you're plotting various time series data and you would like consistent inches / week on your x axis. Or you carefully crafted your figures but suddenly you need a little extra space for you labels. Or you would want to move the axes a little bit apart and *not* rescale everything else in the whole world simultaneously. 
+
 ## getting started
 The package is available on [PyPi](https://pypi.org/project/subplots-from-axsize/).
 
 ## example #1
 ```
 import matplotlib.pyplot as plt
 from subplots_from_axsize import subplots_from_axsize
```

### Comparing `subplots_from_axsize-0.1.7/src/subplots_from_axsize/_subplots_from_axsize.py` & `subplots_from_axsize-0.1.8/src/subplots_from_axsize/_subplots_from_axsize.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,14 +89,15 @@
         If either entry is a list, it will be used to determine `nrows`/`ncols`.
 
     left, bottom, right, top : floats, defaults: 0.6, 0.5, 0.2, 0.1
         Specify figure margins (in inches).
 
     wspace, hspace : sizes, defaults: 0.75, 0.5
         Each size can be either a float or list of floats (inches).
+        `wspace` (`hspace`) specifies the distance(s) between columns (rows).
         If either entry is a list, it will be used to determine `nrows`/`ncols`.
 
     squeeze : bool, default: True
         If True, extra dimensions (with length 1) are removed from `axs`.
         If False, always returns an array of axes with shape ``(nrows, ncols)`.
 
     **fig_kw
```

### Comparing `subplots_from_axsize-0.1.7/PKG-INFO` & `subplots_from_axsize-0.1.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: subplots-from-axsize
-Version: 0.1.7
+Version: 0.1.8
 Summary: 
 Author: Frederic Grabowski
 Author-email: grabowski.frederic@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -16,14 +16,17 @@
 ## subplots_from_axsize
 This package provides a single function, `subplots_from_axsize()`, which is based on matplotlib's `subplots()` and `adjust_subplots()` functions, but:
 * `figsize` is replaced by `axsize`
 * `left`, `bottom`, `right`, `top` use inches instead of fractions
 * `wspace`, `hspace` use inches instead of fractions
 * `axsize`, `wspace`, `hspace` can take lists as arguments (see example #2 below)
 
+## rationale
+Specifying sizes directly makes it easier to achieve consistent ax sizes across figures. Suppose you're plotting various time series data and you would like consistent inches / week on your x axis. Or you carefully crafted your figures but suddenly you need a little extra space for you labels. Or you would want to move the axes a little bit apart and *not* rescale everything else in the whole world simultaneously. 
+
 ## getting started
 The package is available on [PyPi](https://pypi.org/project/subplots-from-axsize/).
 
 ## example #1
 ```
 import matplotlib.pyplot as plt
 from subplots_from_axsize import subplots_from_axsize
```

