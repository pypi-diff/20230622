# Comparing `tmp/hdcms-0.1.26.tar.gz` & `tmp/hdcms-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdcms-0.1.26.tar", last modified: Thu Jun 22 01:41:46 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `hdcms-0.1.26.tar` & `hdcms-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,16 @@
-drwxr-xr-x   0 jason      (502) staff       (20)        0 2023-06-22 01:41:46.612337 hdcms-0.1.26/
--rw-r--r--   0 jason      (502) staff       (20)     1830 2023-01-22 19:56:46.000000 hdcms-0.1.26/LICENSE.txt
--rw-r--r--   0 jason      (502) staff       (20)     4287 2023-06-22 01:41:46.612208 hdcms-0.1.26/PKG-INFO
--rw-r--r--   0 jason      (502) staff       (20)     1795 2023-06-22 01:41:41.000000 hdcms-0.1.26/README.md
--rw-r--r--   0 jason      (502) staff       (20)      597 2023-06-22 01:41:41.000000 hdcms-0.1.26/pyproject.toml
--rw-r--r--   0 jason      (502) staff       (20)       38 2023-06-22 01:41:46.612385 hdcms-0.1.26/setup.cfg
-drwxr-xr-x   0 jason      (502) staff       (20)        0 2023-06-22 01:41:46.610376 hdcms-0.1.26/src/
-drwxr-xr-x   0 jason      (502) staff       (20)        0 2023-06-22 01:41:46.611401 hdcms-0.1.26/src/hdcms/
--rw-r--r--   0 jason      (502) staff       (20)      339 2023-06-20 09:00:01.000000 hdcms-0.1.26/src/hdcms/__init__.py
--rw-r--r--   0 jason      (502) staff       (20)     2120 2023-02-18 19:52:59.000000 hdcms-0.1.26/src/hdcms/gen.py
--rw-r--r--   0 jason      (502) staff       (20)     5793 2023-06-22 00:43:12.000000 hdcms-0.1.26/src/hdcms/stats.py
--rw-r--r--   0 jason      (502) staff       (20)      951 2023-06-20 09:00:01.000000 hdcms-0.1.26/src/hdcms/verify.py
--rw-r--r--   0 jason      (502) staff       (20)     7616 2023-06-22 01:41:40.000000 hdcms-0.1.26/src/hdcms/visualize.py
-drwxr-xr-x   0 jason      (502) staff       (20)        0 2023-06-22 01:41:46.612041 hdcms-0.1.26/src/hdcms.egg-info/
--rw-r--r--   0 jason      (502) staff       (20)     4287 2023-06-22 01:41:46.000000 hdcms-0.1.26/src/hdcms.egg-info/PKG-INFO
--rw-r--r--   0 jason      (502) staff       (20)      301 2023-06-22 01:41:46.000000 hdcms-0.1.26/src/hdcms.egg-info/SOURCES.txt
--rw-r--r--   0 jason      (502) staff       (20)        1 2023-06-22 01:41:46.000000 hdcms-0.1.26/src/hdcms.egg-info/dependency_links.txt
--rw-r--r--   0 jason      (502) staff       (20)       52 2023-06-22 01:41:46.000000 hdcms-0.1.26/src/hdcms.egg-info/requires.txt
--rw-r--r--   0 jason      (502) staff       (20)        6 2023-06-22 01:41:46.000000 hdcms-0.1.26/src/hdcms.egg-info/top_level.txt
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 hdcms-0.1.9/out/hdcms_helper/__init__.pyi
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 hdcms-0.1.9/out/hdcms_helper/clean.pyi
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 hdcms-0.1.9/out/hdcms_helper/gen.pyi
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 hdcms-0.1.9/out/hdcms_helper/stats.pyi
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 hdcms-0.1.9/out/hdcms_helper/visualize.pyi
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 hdcms-0.1.9/src/hdcms_helper/__init__.py
+-rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 hdcms-0.1.9/src/hdcms_helper/clean.py
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 hdcms-0.1.9/src/hdcms_helper/gen.py
+-rw-r--r--   0        0        0     5206 2020-02-02 00:00:00.000000 hdcms-0.1.9/src/hdcms_helper/stats.py
+-rw-r--r--   0        0        0     6508 2020-02-02 00:00:00.000000 hdcms-0.1.9/src/hdcms_helper/visualize.py
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 hdcms-0.1.9/test/.DS_Store
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 hdcms-0.1.9/.gitignore
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 hdcms-0.1.9/LICENSE.txt
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 hdcms-0.1.9/README.md
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 hdcms-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     4768 2020-02-02 00:00:00.000000 hdcms-0.1.9/PKG-INFO
```

### Comparing `hdcms-0.1.26/LICENSE.txt` & `hdcms-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hdcms-0.1.26/PKG-INFO` & `hdcms-0.1.9/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 Metadata-Version: 2.1
 Name: hdcms
-Version: 0.1.26
+Version: 0.1.9
 Summary: This package creates useful helper functions for python API
+Project-URL: Homepage, https://github.com/jasoneveleth/pyhdcms-helper
+Project-URL: Bug Tracker, https://github.com/jasoneveleth/pyhdcms-helper/issues
 Author: Arun Moorthy
 Author-email: Jason Eveleth <hdcms-helper@jasoneveleth.com>
 License: NIST-developed software is provided by NIST as a public service. You may use,
         copy, and distribute copies of the software in any medium, provided that you
         keep intact this entire notice. You may improve, modify, and create derivative
         works of the software or any portion of the software, and you may copy and
         distribute such modifications or works. Modified works should carry a notice
@@ -27,64 +29,65 @@
         distributing the software and you assume all risks associated with its use,
         including but not limited to the risks and costs of program errors, compliance
         with applicable laws, damage to or loss of data, programs or equipment, and the
         unavailability or interruption of operation. This software is not intended to
         be used in any situation where a failure could cause risk of injury or damage
         to property. The software developed by NIST employees is not subject to
         copyright protection within the United States.
-        
-Project-URL: Homepage, https://github.com/jasoneveleth/hdcms-python
-Project-URL: Bug Tracker, https://github.com/jasoneveleth/hdcms-python/issues
+License-File: LICENSE.txt
 Requires-Python: >=3.7
+Requires-Dist: hdcms
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: opencv-python
+Requires-Dist: scipy
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
 
-# hdcms
+# hdcms-helper
 
 This library is available on pypi [here](https://pypi.org/project/hdcms/). Install using `pip install hdcms`.
 
-A very simple example:
+How to use
 
 ```python
 import hdcms as hdc
 
 hdc.generate_examples(visualize=True)
 gaussian_sum_stat = hdc.regex2stats1d(r"gaus_\d+.txt")
 laplacian_sum_stat = hdc.regex2stats1d(r"laplace_\d+\.txt")
 
+# data in another directory for example:
+# regex2stats2d(r"CM1_11_\d+.txt", dir="~/src/hdcms/data/")
+
 print(hdc.compare(gaussian_sum_stat, laplacian_sum_stat))
 hdc.write_image(gaussian_sum_stat, "tmp.png")
 ```
 
-For more documentation: see [`examples/` directory](https://github.com/jasoneveleth/hdcms-python/tree/main/examples).
+This library is built on top of the [`hdcms-bindings` package](https://pypi.org/project/hdcms-bindings/), which exposes python bindings to a C library. That bindings package contains only a few functions and lacks a nice user experience. But, if you are only interested in that, check it out.
+
+# Summary of provided functions
+
+`regex2stats1d`, `regex2stats2d` - takes regex and converts to summary statistic
+`array2stats1d`, `array2stats2d` - takes a varargs list of numpy arrays and converts them into 1d summary statistic
+`file2stats1d`, `file2stats2d` - takes filename and converts it to a summary stat. it is expected that the file contents are a list of filenames on separate lines
+`filenames2stats1d`, `filenames2stats2d` - takes list of filenames and converts it to a summary stat
+`compare` - compares two summary statistics
+`write_image` - visualizes a summary statistic
+`clean` - takes list of filenames and shows you what changes need to be made
+`generate_examples` - generate synthetic data as an example
 
 ## Dependencies
 
-This library is built on top of the [`hdcms-bindings` package](https://pypi.org/project/hdcms-bindings/), which exposes python bindings to a C library. 
+Numpy is a necessary dependency for every function. 
+Matplotlib and scipy are needed for \verb|generate_example()|, which will generate a raondom synthetic data set. 
+opencv is required for \verb|write_image()|, which will visualize summary statistics. 
+You can see a complete list of functions (and where they are located) by running the following code.
+Look at the output of \verb|help(hdc)| to get the right filename.
 
-`numpy` is a necessary dependency for every function. 
+## TODO
 
-`matplotlib` and scipy are needed for `generate_example()`, which will generate a random synthetic data set. 
+filter function for 2d spectra to filter out peaks with large x variation
 
 ## Change Log
 
-```
-0.1.26 Bug fix: npeaks for y-hdc for visualization was possible
-0.1.25 Added missing optional args for filenames2stats*
-0.1.24 Add npeaks for visualization
-0.1.23 Add xtol
-0.1.22 Fix new colors for write_image
-0.1.21 New colors for write_image
-0.1.20 Change name from ms_valid_data_format to is_valid_ms_data_format + scaling, start, end, num_bins
-0.1.19 Return image from write_image
-0.1.18 Add labels to visualization configuration options
-0.1.17 Use matplotlib axes rather than my own
-0.1.16 Bug fixes (text for x axis, names for regex2filenames)
-0.1.15 Return image from write_image, rather than writing to file
-0.1.14 Add new params to write_image
-0.1.13 Add new params to write_image
-0.1.12 Add params to write_image
-0.1.11 Fix problems introduced by rename
-0.1.10 Really rename (broken)
-0.1.9 Rename, performance for visulize in 1D case (broken)
+0.1.9 Rename, performance for visulize in 1D case
 0.1.8 Add documentation
-```
```

### Comparing `hdcms-0.1.26/README.md` & `hdcms-0.1.9/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,49 @@
-# hdcms
+# hdcms-helper
 
 This library is available on pypi [here](https://pypi.org/project/hdcms/). Install using `pip install hdcms`.
 
-A very simple example:
+How to use
 
 ```python
 import hdcms as hdc
 
 hdc.generate_examples(visualize=True)
 gaussian_sum_stat = hdc.regex2stats1d(r"gaus_\d+.txt")
 laplacian_sum_stat = hdc.regex2stats1d(r"laplace_\d+\.txt")
 
+# data in another directory for example:
+# regex2stats2d(r"CM1_11_\d+.txt", dir="~/src/hdcms/data/")
+
 print(hdc.compare(gaussian_sum_stat, laplacian_sum_stat))
 hdc.write_image(gaussian_sum_stat, "tmp.png")
 ```
 
-For more documentation: see [`examples/` directory](https://github.com/jasoneveleth/hdcms-python/tree/main/examples).
+This library is built on top of the [`hdcms-bindings` package](https://pypi.org/project/hdcms-bindings/), which exposes python bindings to a C library. That bindings package contains only a few functions and lacks a nice user experience. But, if you are only interested in that, check it out.
+
+# Summary of provided functions
+
+`regex2stats1d`, `regex2stats2d` - takes regex and converts to summary statistic
+`array2stats1d`, `array2stats2d` - takes a varargs list of numpy arrays and converts them into 1d summary statistic
+`file2stats1d`, `file2stats2d` - takes filename and converts it to a summary stat. it is expected that the file contents are a list of filenames on separate lines
+`filenames2stats1d`, `filenames2stats2d` - takes list of filenames and converts it to a summary stat
+`compare` - compares two summary statistics
+`write_image` - visualizes a summary statistic
+`clean` - takes list of filenames and shows you what changes need to be made
+`generate_examples` - generate synthetic data as an example
 
 ## Dependencies
 
-This library is built on top of the [`hdcms-bindings` package](https://pypi.org/project/hdcms-bindings/), which exposes python bindings to a C library. 
+Numpy is a necessary dependency for every function. 
+Matplotlib and scipy are needed for \verb|generate_example()|, which will generate a raondom synthetic data set. 
+opencv is required for \verb|write_image()|, which will visualize summary statistics. 
+You can see a complete list of functions (and where they are located) by running the following code.
+Look at the output of \verb|help(hdc)| to get the right filename.
 
-`numpy` is a necessary dependency for every function. 
+## TODO
 
-`matplotlib` and scipy are needed for `generate_example()`, which will generate a random synthetic data set. 
+filter function for 2d spectra to filter out peaks with large x variation
 
 ## Change Log
 
-```
-0.1.26 Bug fix: npeaks for y-hdc for visualization was possible
-0.1.25 Added missing optional args for filenames2stats*
-0.1.24 Add npeaks for visualization
-0.1.23 Add xtol
-0.1.22 Fix new colors for write_image
-0.1.21 New colors for write_image
-0.1.20 Change name from ms_valid_data_format to is_valid_ms_data_format + scaling, start, end, num_bins
-0.1.19 Return image from write_image
-0.1.18 Add labels to visualization configuration options
-0.1.17 Use matplotlib axes rather than my own
-0.1.16 Bug fixes (text for x axis, names for regex2filenames)
-0.1.15 Return image from write_image, rather than writing to file
-0.1.14 Add new params to write_image
-0.1.13 Add new params to write_image
-0.1.12 Add params to write_image
-0.1.11 Fix problems introduced by rename
-0.1.10 Really rename (broken)
-0.1.9 Rename, performance for visulize in 1D case (broken)
+0.1.9 Rename, performance for visulize in 1D case
 0.1.8 Add documentation
-```
```

### Comparing `hdcms-0.1.26/pyproject.toml` & `hdcms-0.1.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
+[build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "hdcms"
-version = "0.1.26"
+version = "0.1.9"
 description = "This package creates useful helper functions for python API"
 authors = [
     {name="Jason Eveleth", email="hdcms-helper@jasoneveleth.com"},
     {name="Arun Moorthy"},
 ]
 readme = "README.md"
 requires-python = ">=3.7"
-dependencies = ["hdcms-bindings", "opencv-python", "numpy", "matplotlib", "scipy"]
+dependencies = ["hdcms", "opencv-python", "numpy", "matplotlib", "scipy"]
 license = { file="LICENSE.txt" }
 
 [project.urls]
-"Homepage" = "https://github.com/jasoneveleth/hdcms-python"
-"Bug Tracker" = "https://github.com/jasoneveleth/hdcms-python/issues"
+"Homepage" = "https://github.com/jasoneveleth/pyhdcms-helper"
+"Bug Tracker" = "https://github.com/jasoneveleth/pyhdcms-helper/issues"
```

### Comparing `hdcms-0.1.26/src/hdcms/gen.py` & `hdcms-0.1.9/src/hdcms_helper/gen.py`

 * *Files identical despite different names*

### Comparing `hdcms-0.1.26/src/hdcms/stats.py` & `hdcms-0.1.9/src/hdcms_helper/stats.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,100 +1,100 @@
-import hdcms_bindings
+import hdcms
 import re
 import os
 import sys
 import numpy as np
 
 def file_ok(fname):
     """ensure that fname is a file"""
     if not (os.path.isfile(fname) and os.access(fname, os.R_OK)):
         raise RuntimeError(f"File {fname} doesn't exist or isn't readable")
 
-def filenames2stats1d(filenames, start=0, end=900, num_bins=9000, scaling='n'):
+def filenames2stats1d(filenames):
     """take filenames and convert them into a 1d summary statistic"""
     for f in filenames.split(","):
         file_ok(f)
-    return hdcms_bindings.filenames_to_stats_1d(filenames, start=start, end=end, num_bins=num_bins, scaling=scaling)
+    return hdcms.filenames_to_stats_1d(filenames)
 
-def filenames2stats2d(filenames, scaling='n', xtol=float('inf')):
+def filenames2stats2d(filenames):
     """take filenames and convert them into a 2d summary statistic"""
     for f in filenames.split(","):
         if not (os.path.isfile(f) and os.access(f, os.R_OK)):
             raise RuntimeError(f"File {f} doesn't exist or isn't readable")
-    return hdcms_bindings.filenames_to_stats_2d(filenames, scaling=scaling, xtol=xtol)
+    return hdcms.filenames_to_stats_2d(filenames)
 
 def regex2filenames(regex, dir="."):
     """takes regex, finds all files that match and convert them into list of filenames"""
     files = [f for f in os.listdir(dir) if os.path.isfile(os.path.join(dir, f))]
 
     r = re.compile(regex)
     matches = []
     for f in files:
         match = r.match(f)
         if match:
-            matches.append(f)
+            matches.append(match.group())
 
     if len(matches) == 0:
         raise RuntimeError(f"No matches for {regex} in directory {dir}")
 
     full_paths = list(map(lambda f: os.path.join(dir, f), matches))
     return ','.join(full_paths)
 
-def regex2stats1d(regex, dir=".", start=0, end=900, num_bins=9000, scaling='m'):
+def regex2stats1d(regex, dir="."):
     """takes regex, converts list of filenames that match into 1d summary stat"""
     filenames = regex2filenames(regex, dir)
-    return filenames2stats1d(filenames, start, end, num_bins, scaling)
+    return filenames2stats1d(filenames)
 
-def regex2stats2d(regex, dir=".", scaling='m', xtol=float('inf')):
+def regex2stats2d(regex, dir="."):
     """takes regex, converts list of filenames that match into 2d summary stat
-       example: regex2stats2d(r"CM1_2_\\d.txt", dir="../data")"""
+       example: regex2stats1d(r"CM1_2_\\d.txt", dir="../data")"""
     filenames = regex2filenames(regex, dir)
-    return filenames2stats2d(filenames, scaling, xtol)
+    return filenames2stats2d(filenames)
 
 def file2filenames(filename):
     """takes file with filenames on separate lines and joins them into a string of filenames separated by commas"""
     with open(filename) as f:
         return ",".join(f.readlines())
 
-def file2stats1d(filename, start=0, end=900, num_bins=9000, scaling='m'):
+def file2stats1d(filename):
     """takes file with filenames on separate lines converts them into a 1d summary statistic"""
-    return filenames2stats1d(file2filenames(filename), start, end, num_bins, scaling)
+    return filenames2stats1d(file2filenames(filename))
 
-def file2stats2d(filename, scaling='m', xtol=float('inf')):
+def file2stats2d(filename):
     """takes file with filenames on separate lines converts them into a 2d summary statistic
        example: file2stats2d("./compound1_high_res.txt")"""
-    return filenames2stats2d(file2filenames(filename), scaling, xtol)
+    return filenames2stats2d(file2filenames(filename))
 
 def get_unique_tmpdir(name="hdcms-numpy-tmp"):
     """creates a unique temporary directory, in unix it's /tmp, on windows its C:\\Users\\AppData\\Local\\Temp"""
     dir = f"/tmp" if sys.platform != "win32" else f"C:\\Users\\AppData\\Local\\Temp"
     _, existing_dirs, _ = next(os.walk(dir))
     while name in existing_dirs:
         name += "0"
     return os.path.join(dir, name)
 
-def array2stats1d(*args, start=0, end=900, num_bins=9000, scaling='m'):
+def array2stats1d(*args):
     """takes a varargs list of numpy arrays and converts them into 1d summary statistic"""
     dir = get_unique_tmpdir()
     lst = []
     for i, arr in args:
         filename = os.path.join(dir, f"{i}-numpy-array.txt")
         np.savetxt(filename, arr)
         lst.append(filename)
-    return filenames2stats1d(",".join(lst), start, end, num_bins, scaling)
+    return filenames2stats1d(",".join(lst))
 
-def array2stats2d(*args, scaling='m', xtol=float('inf')):
+def array2stats2d(*args):
     """takes a varargs list of numpy arrays and converts them into 2d summary statistic"""
     dir = get_unique_tmpdir()
     lst = []
     for i, arr in args:
         filename = os.path.join(dir, f"{i}-numpy-array.txt")
         np.savetxt(filename, arr)
         lst.append(filename)
-    return filenames2stats2d(",".join(lst), scaling, xtol)
+    return filenames2stats2d(",".join(lst))
 
 # figures out the comparison function needed and checks that the input is valid size
 def compare(*args, npeaks=None):
     """takes varargs list of summary statistic and computes the similarity according to its arguments,
        so if all arrays are 1d summary stats it will compare them using 1d similarity, same with 2d, if
        anything doesn't match it will raise a helpful error message"""
     is_using_2d = (npeaks != None)
@@ -116,16 +116,16 @@
     # verify they all have the same length of second dimension
     for arr in args:
         if arr.shape[1] != len_of_dim_2:
             raise RuntimeError(f"Mismatch dimension: recieved {arr.shape} and {args[0].shape}, they must be the same and either (_, 2) or (_, 4)")
 
     if len(args) == 2:
         if is_using_2d:
-            return hdcms_bindings.compare_compound_2d(args[0], args[1])
+            return hdcms.compare_compound_2d(args[0], args[1])
         else:
-            return hdcms_bindings.compare_compound_1d(args[0], args[1])
+            return hdcms.compare_compound_1d(args[0], args[1])
     else:
         if is_using_2d:
-            return hdcms_bindings.compare_all_2d(args)
+            return hdcms.compare_all_2d(args)
         else:
-            return hdcms_bindings.compare_all_1d(args)
+            return hdcms.compare_all_1d(args)
```

