# Comparing `tmp/aspect_ratio_too-0.1.0-py2.py3-none-any.whl.zip` & `tmp/aspect_ratio_too-0.1.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 3953 bytes, number of entries: 9
--rw-r--r--  2.0 unx      111 b- defN 22-Nov-07 14:58 aspect_ratio_too/__init__.py
--rw-r--r--  2.0 unx     1145 b- defN 22-Nov-07 16:02 aspect_ratio_too/aspect_ratio.py
--rw-r--r--  2.0 unx      804 b- defN 22-Nov-07 16:20 aspect_ratio_too/utils.py
--rw-r--r--  2.0 unx     1749 b- defN 22-Nov-07 16:00 tests/test_aspect_ratio.py
--rw-r--r--  2.0 unx      199 b- defN 22-Nov-07 16:30 aspect_ratio_too-0.1.0.dist-info/AUTHORS.md
--rw-r--r--  2.0 unx     2054 b- defN 22-Nov-07 16:30 aspect_ratio_too-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 22-Nov-07 16:30 aspect_ratio_too-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       23 b- defN 22-Nov-07 16:30 aspect_ratio_too-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      771 b- defN 22-Nov-07 16:30 aspect_ratio_too-0.1.0.dist-info/RECORD
-9 files, 6966 bytes uncompressed, 2611 bytes compressed:  62.5%
+Zip file size: 4360 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      128 b- defN 23-Jun-22 14:03 aspect_ratio_too/__init__.py
+-rw-r--r--  2.0 unx     1146 b- defN 23-Jun-22 14:03 aspect_ratio_too/aspect_ratio.py
+-rw-r--r--  2.0 unx      732 b- defN 22-Nov-07 18:51 aspect_ratio_too/utils.py
+-rw-r--r--  2.0 unx      199 b- defN 23-Jun-22 14:11 aspect_ratio_too-0.1.1.dist-info/AUTHORS.md
+-rw-r--r--  2.0 unx     1084 b- defN 23-Jun-22 14:11 aspect_ratio_too-0.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1969 b- defN 23-Jun-22 14:11 aspect_ratio_too-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-22 14:11 aspect_ratio_too-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-Jun-22 14:11 aspect_ratio_too-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      785 b- defN 23-Jun-22 14:11 aspect_ratio_too-0.1.1.dist-info/RECORD
+9 files, 6170 bytes uncompressed, 2990 bytes compressed:  51.5%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: aspect_ratio_too/aspect_ratio.py
 Comment: 
 
 Filename: aspect_ratio_too/utils.py
 Comment: 
 
-Filename: tests/test_aspect_ratio.py
+Filename: aspect_ratio_too-0.1.1.dist-info/AUTHORS.md
 Comment: 
 
-Filename: aspect_ratio_too-0.1.0.dist-info/AUTHORS.md
+Filename: aspect_ratio_too-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: aspect_ratio_too-0.1.0.dist-info/METADATA
+Filename: aspect_ratio_too-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: aspect_ratio_too-0.1.0.dist-info/WHEEL
+Filename: aspect_ratio_too-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: aspect_ratio_too-0.1.0.dist-info/top_level.txt
+Filename: aspect_ratio_too-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: aspect_ratio_too-0.1.0.dist-info/RECORD
+Filename: aspect_ratio_too-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aspect_ratio_too/__init__.py

```diff
@@ -1,3 +1,7 @@
-from .aspect_ratio import AspectRatioCalculator, aspect_ratio_str, aspect_ratio  # noqa
+from .aspect_ratio import (  # noqa
+    AspectRatioCalculator,
+    aspect_ratio,
+    aspect_ratio_str,
+)
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
```

## aspect_ratio_too/aspect_ratio.py

```diff
@@ -1,8 +1,9 @@
 import math
+
 from aspect_ratio_too.utils import closest_number
 
 
 def aspect_ratio_str(width: int, height: int) -> str:
     """ "Given a pixel width/height return a string ratio (eg - 16:9)."""
     r = math.gcd(width, height)
     x = int(width / r)
```

## aspect_ratio_too/utils.py

```diff
@@ -13,13 +13,12 @@
     n2 = multiple * (q + 1) if (number * multiple) > 0 else multiple * (q - 1)
 
     # if true, then n1 is the required closest number
     return n1 if abs(number - n1) < abs(number - n2) else n2
 
 
 def round_to_multiple(number, multiple, direction="nearest"):
-    if direction == "nearest" or direction not in ["up", "down"]:
-        return multiple * round(number / multiple)
-    elif direction == "up":
+    if direction == "up":
         return multiple * ceil(number / multiple)
     elif direction == "down":
         return multiple * floor(number / multiple)
+    return multiple * round(number / multiple)
```

## Comparing `aspect_ratio_too-0.1.0.dist-info/METADATA` & `aspect_ratio_too-0.1.1.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,64 +1,64 @@
 Metadata-Version: 2.1
 Name: aspect-ratio-too
-Version: 0.1.0
+Version: 0.1.1
 Summary: Aspect ratio calculations.
 Author-email: Tim Santor <tsantor@xstudios.com>
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.6
-Description-Content-Type: text/x-rst
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
 License-File: AUTHORS.md
 Provides-Extra: dev
 Requires-Dist: black ; extra == 'dev'
 Requires-Dist: pre-commit ; extra == 'dev'
-Requires-Dist: flake8 ; extra == 'dev'
-Requires-Dist: pylint ; extra == 'dev'
-Requires-Dist: wheel ; extra == 'dev'
-Requires-Dist: build ; extra == 'dev'
 
 # Aspect Ratio Too
 
 
 ## Overview
 Aspect ratio calculations.
 
+## Installation
+
+    pip install aspect-ratio-too
+
+
 
 ## Development
 
     make env
     make reqs
     pip install -e .
 
+## Testing
 
-## Installation
-
-    pip install aspect-ratio-too
+    pytest
 
 
 ## Usage
 Know the aspect ratio you want but don't know the corresponding width/height? Try this:
 
     from aspect_ratio_too import AspectRatioCalculator
 
     arc = AspectRatioCalculator(16, 9)
 
     # Get (width/height) tuple
     arc.width_to_dimensions(1920)  # (1920, 1080)
     arc.height_to_dimensions(1080)  # (1920, 1080)
 
-    arc.width_to_height(1920)  # 1920
-    arc.height_to_width(1080)  # 1080
+    arc.width_to_height(1920)  # 1080
+    arc.height_to_width(1080)  # 1920
 
 Or calculate the aspect ratio given know pixel dimensions:
 
     from aspect_ratio_too import aspect_ratio, aspect_ratio_str
 
     aspect_ratio(1920, 1080)  # 1.7777777777777777
 
@@ -68,9 +68,12 @@
 ## Issues
 
 If you experience any issues, please create an [issue](https://bitbucket.org/xstudios/aspect-ratio-too/issues) on Bitbucket.
 
 # History
 All notable changes to this project will be documented in this file. This project adheres to [Semantic Versioning](http://semver.org/).
 
+## 0.1.1 (2023-06-22)
+* Update packaging method to `pyproject.toml`.
+
 ## 0.0.1 (2022-11-07)
 * First release
```

