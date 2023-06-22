# Comparing `tmp/pybox-toolkit-0.1.9.dev81.tar.gz` & `tmp/pybox-toolkit-0.1.9.dev82.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybox-toolkit-0.1.9.dev81.tar", last modified: Thu Jun 22 16:51:10 2023, max compression
+gzip compressed data, was "pybox-toolkit-0.1.9.dev82.tar", last modified: Thu Jun 22 17:31:30 2023, max compression
```

## Comparing `pybox-toolkit-0.1.9.dev81.tar` & `pybox-toolkit-0.1.9.dev82.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 16:51:10.283623 pybox-toolkit-0.1.9.dev81/
--rw-r--r--   0 root         (0) root         (0)      480 2023-06-22 16:51:10.283623 pybox-toolkit-0.1.9.dev81/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      857 2023-06-22 16:50:30.000000 pybox-toolkit-0.1.9.dev81/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       11 2023-06-22 16:50:30.000000 pybox-toolkit-0.1.9.dev81/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 16:51:10.287623 pybox-toolkit-0.1.9.dev81/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 16:51:10.279623 pybox-toolkit-0.1.9.dev81/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 16:51:10.283623 pybox-toolkit-0.1.9.dev81/src/pybox_toolkit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      480 2023-06-22 16:51:10.000000 pybox-toolkit-0.1.9.dev81/src/pybox_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      419 2023-06-22 16:51:10.000000 pybox-toolkit-0.1.9.dev81/src/pybox_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 16:51:10.000000 pybox-toolkit-0.1.9.dev81/src/pybox_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-06-22 16:51:10.000000 pybox-toolkit-0.1.9.dev81/src/pybox_toolkit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-22 16:51:10.000000 pybox-toolkit-0.1.9.dev81/src/pybox_toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 16:51:10.283623 pybox-toolkit-0.1.9.dev81/src/toolkit/
--rw-rw-rw-   0 root         (0) root         (0)    15423 2023-06-22 16:50:30.000000 pybox-toolkit-0.1.9.dev81/src/toolkit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 16:51:10.283623 pybox-toolkit-0.1.9.dev81/src/toolkit/graphing/
--rw-rw-rw-   0 root         (0) root         (0)     1724 2023-06-22 07:36:20.000000 pybox-toolkit-0.1.9.dev81/src/toolkit/graphing/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 16:50:30.000000 pybox-toolkit-0.1.9.dev81/src/toolkit/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 16:51:10.283623 pybox-toolkit-0.1.9.dev81/src/toolkit/test/
--rw-rw-rw-   0 root         (0) root         (0)     5113 2023-06-22 16:50:30.000000 pybox-toolkit-0.1.9.dev81/src/toolkit/test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 16:51:10.283623 pybox-toolkit-0.1.9.dev81/src/toolkit/typing/
--rw-rw-rw-   0 root         (0) root         (0)     9875 2023-06-22 07:36:20.000000 pybox-toolkit-0.1.9.dev81/src/toolkit/typing/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      839 2023-06-22 07:36:20.000000 pybox-toolkit-0.1.9.dev81/src/toolkit/typing/si.py
--rw-rw-rw-   0 root         (0) root         (0)     7997 2023-06-22 16:50:30.000000 pybox-toolkit-0.1.9.dev81/src/toolkit/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 17:31:30.533342 pybox-toolkit-0.1.9.dev82/
+-rw-r--r--   0 root         (0) root         (0)      480 2023-06-22 17:31:30.529343 pybox-toolkit-0.1.9.dev82/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      857 2023-06-22 17:30:54.000000 pybox-toolkit-0.1.9.dev82/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       11 2023-06-22 17:30:54.000000 pybox-toolkit-0.1.9.dev82/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 17:31:30.533342 pybox-toolkit-0.1.9.dev82/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 17:31:30.525342 pybox-toolkit-0.1.9.dev82/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 17:31:30.529343 pybox-toolkit-0.1.9.dev82/src/pybox_toolkit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      480 2023-06-22 17:31:30.000000 pybox-toolkit-0.1.9.dev82/src/pybox_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      419 2023-06-22 17:31:30.000000 pybox-toolkit-0.1.9.dev82/src/pybox_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 17:31:30.000000 pybox-toolkit-0.1.9.dev82/src/pybox_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-22 17:31:30.000000 pybox-toolkit-0.1.9.dev82/src/pybox_toolkit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-22 17:31:30.000000 pybox-toolkit-0.1.9.dev82/src/pybox_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 17:31:30.529343 pybox-toolkit-0.1.9.dev82/src/toolkit/
+-rw-rw-rw-   0 root         (0) root         (0)    15423 2023-06-22 17:30:54.000000 pybox-toolkit-0.1.9.dev82/src/toolkit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 17:31:30.529343 pybox-toolkit-0.1.9.dev82/src/toolkit/graphing/
+-rw-rw-rw-   0 root         (0) root         (0)     1724 2023-06-22 07:36:20.000000 pybox-toolkit-0.1.9.dev82/src/toolkit/graphing/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 17:30:54.000000 pybox-toolkit-0.1.9.dev82/src/toolkit/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 17:31:30.529343 pybox-toolkit-0.1.9.dev82/src/toolkit/test/
+-rw-rw-rw-   0 root         (0) root         (0)     5113 2023-06-22 17:30:54.000000 pybox-toolkit-0.1.9.dev82/src/toolkit/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 17:31:30.529343 pybox-toolkit-0.1.9.dev82/src/toolkit/typing/
+-rw-rw-rw-   0 root         (0) root         (0)     9875 2023-06-22 07:36:20.000000 pybox-toolkit-0.1.9.dev82/src/toolkit/typing/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      839 2023-06-22 07:36:20.000000 pybox-toolkit-0.1.9.dev82/src/toolkit/typing/si.py
+-rw-rw-rw-   0 root         (0) root         (0)     8004 2023-06-22 17:30:54.000000 pybox-toolkit-0.1.9.dev82/src/toolkit/utils.py
```

### Comparing `pybox-toolkit-0.1.9.dev81/pyproject.toml` & `pybox-toolkit-0.1.9.dev82/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pybox-toolkit-0.1.9.dev81/src/toolkit/__init__.py` & `pybox-toolkit-0.1.9.dev82/src/toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `pybox-toolkit-0.1.9.dev81/src/toolkit/graphing/__init__.py` & `pybox-toolkit-0.1.9.dev82/src/toolkit/graphing/__init__.py`

 * *Files identical despite different names*

### Comparing `pybox-toolkit-0.1.9.dev81/src/toolkit/test/__init__.py` & `pybox-toolkit-0.1.9.dev82/src/toolkit/test/__init__.py`

 * *Files identical despite different names*

### Comparing `pybox-toolkit-0.1.9.dev81/src/toolkit/typing/__init__.py` & `pybox-toolkit-0.1.9.dev82/src/toolkit/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `pybox-toolkit-0.1.9.dev81/src/toolkit/typing/si.py` & `pybox-toolkit-0.1.9.dev82/src/toolkit/typing/si.py`

 * *Files identical despite different names*

### Comparing `pybox-toolkit-0.1.9.dev81/src/toolkit/utils.py` & `pybox-toolkit-0.1.9.dev82/src/toolkit/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,14 +87,15 @@
 
     return interval
 
 
 def stringify_interval(interval: tuple[float, float]) -> str:
     """
     Turns a physical range back into its string representation.
+
     Args:
         interval (tuple[float, float]): interval in tuple form
 
     Returns:
         str: interval in string form
     """
     # We try to undo the epsilon for clarity, but this will not work if the original input was non-integral
@@ -118,14 +119,15 @@
 
     return bottom_range + top_range
 
 
 def _safe_div(dividend: float, divisor: float) -> float:
     """
     Float division, with infinity returned if dividing by 0
+
     Args:
         dividend (float): float being divided
         divisor (float): float dividing
 
     Returns:
         float: Result of regular division, or infinity if the divisor is 0
     """
@@ -133,14 +135,15 @@
         return copysign(float("inf"), dividend)
     return dividend / divisor
 
 
 def _safe_min(args: Iterable[float]) -> float:
     """
     Calculate the minimum of an iterable, without returning nan
+
     Args:
         args (Iterable[float]): iterable for which to find a minimum
 
     Returns:
         float: minimum of args, ignoring nan
     """
     filtered_args = (arg for arg in args if not isnan(arg))
@@ -162,14 +165,15 @@
 
 def physical_range_division(
     prange_a: tuple[float, float], prange_b: tuple[float, float]
 ) -> tuple[float, float]:
     """
     Calculate the maximum physical range possible from the equation:
         a / b
+
     Args:
         prange_a (tuple[float, float]): physical range of 'a'
         prange_b (tuple[float, float]): physical range of 'b'
 
     Returns:
         tuple[float, float]: physical range of 'a / b'
     """
@@ -190,14 +194,15 @@
 
 def physical_range_multiplication(
     prange_a: tuple[float, float], prange_b: tuple[float, float]
 ) -> tuple[float, float]:
     """
     Calculate the maximum physical range possible from the equation:
         a * b
+
     Args:
         prange_a (tuple[float, float]): physical range of 'a'
         prange_b (tuple[float, float]): physical range of 'b'
 
     Returns:
         tuple[float, float]: physical range of 'a * b'
     """
@@ -212,14 +217,15 @@
 
 def physical_range_power(
     prange: tuple[float, float], power: int
 ) -> tuple[float, float]:
     """
     Calculate the maximum physical range possible from the equation:
         a ** n
+
     Args:
         prange (tuple[float, float]): physical range of 'a'
         power (int): exponentiating power
 
     Returns:
         tuple[float, float]: physical range of 'a ** n'
     """
@@ -246,14 +252,15 @@
     # prange[0] >= 0 here
     return (prange[0] ** power, prange[1] ** power)
 
 
 def exponent_unicode(exponent: int) -> str:
     """
     Get the unicode superscript of an integer
+
     Args:
         exponent (int): integer exponent
 
     Returns:
         str: exponent unicode
     """
     return "".join(_UNICODE_DIGITS[digit] for digit in str(exponent))
```

