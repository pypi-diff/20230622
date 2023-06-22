# Comparing `tmp/enstools-compression-2023.5.tar.gz` & `tmp/enstools-compression-2023.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enstools-compression-2023.5.tar", last modified: Thu May 11 15:11:19 2023, max compression
+gzip compressed data, was "enstools-compression-2023.6.tar", last modified: Thu Jun 22 14:47:57 2023, max compression
```

## Comparing `enstools-compression-2023.5.tar` & `enstools-compression-2023.6.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:11:19.355095 enstools-compression-2023.5/
--rw-rw-rw-   0 root         (0) root         (0)    10898 2023-01-18 16:33:07.000000 enstools-compression-2023.5/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       15 2023-01-18 16:33:07.000000 enstools-compression-2023.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1660 2023-05-11 15:11:19.354095 enstools-compression-2023.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1412 2023-01-18 16:33:07.000000 enstools-compression-2023.5/README.md
--rw-rw-rw-   0 root         (0) root         (0)        7 2023-05-11 13:20:17.000000 enstools-compression-2023.5/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:11:19.350095 enstools-compression-2023.5/enstools/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:11:19.352095 enstools-compression-2023.5/enstools/compression/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-11 12:10:49.000000 enstools-compression-2023.5/enstools/compression/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:11:19.353095 enstools-compression-2023.5/enstools/compression/analyzer/
--rw-rw-rw-   0 root         (0) root         (0)       53 2023-01-18 16:33:07.000000 enstools-compression-2023.5/enstools/compression/analyzer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4050 2023-05-11 12:10:49.000000 enstools-compression-2023.5/enstools/compression/analyzer/analysis_options.py
--rw-rw-rw-   0 root         (0) root         (0)     6932 2023-05-11 12:10:49.000000 enstools-compression-2023.5/enstools/compression/analyzer/analyze_data_array.py
--rwxrwxrwx   0 root         (0) root         (0)    10707 2023-05-11 12:10:49.000000 enstools-compression-2023.5/enstools/compression/analyzer/analyzer.py
--rw-rw-rw-   0 root         (0) root         (0)    12948 2023-05-11 12:10:49.000000 enstools-compression-2023.5/enstools/compression/analyzer/analyzer_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      617 2023-05-11 12:10:49.000000 enstools-compression-2023.5/enstools/compression/api.py
--rw-rw-rw-   0 root         (0) root         (0)    19012 2023-05-11 12:10:49.000000 enstools-compression-2023.5/enstools/compression/cli.py
--rwxrwxrwx   0 root         (0) root         (0)    11108 2023-05-11 12:10:49.000000 enstools-compression-2023.5/enstools/compression/compressor.py
--rwxrwxrwx   0 root         (0) root         (0)     5492 2023-05-11 12:10:49.000000 enstools-compression-2023.5/enstools/compression/emulation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:11:19.353095 enstools-compression-2023.5/enstools/compression/emulators/
--rw-rw-rw-   0 root         (0) root         (0)      301 2023-05-11 12:10:49.000000 enstools-compression-2023.5/enstools/compression/emulators/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1176 2023-05-11 12:10:49.000000 enstools-compression-2023.5/enstools/compression/emulators/emulator_class.py
--rw-rw-rw-   0 root         (0) root         (0)     3341 2023-05-11 12:10:49.000000 enstools-compression-2023.5/enstools/compression/emulators/filters_emulator.py
--rwxrwxrwx   0 root         (0) root         (0)     4847 2023-05-11 12:10:49.000000 enstools-compression-2023.5/enstools/compression/emulators/libpressio_emulator.py
--rwxrwxrwx   0 root         (0) root         (0)     2959 2023-05-11 12:10:49.000000 enstools-compression-2023.5/enstools/compression/emulators/zfp_emulator.py
--rw-rw-rw-   0 root         (0) root         (0)     2908 2023-05-11 12:10:49.000000 enstools-compression-2023.5/enstools/compression/evaluator.py
--rw-rw-rw-   0 root         (0) root         (0)     5369 2023-05-11 12:10:49.000000 enstools-compression-2023.5/enstools/compression/h5netcdf_compressor.py
--rw-rw-rw-   0 root         (0) root         (0)    12646 2023-05-11 12:10:49.000000 enstools-compression-2023.5/enstools/compression/metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     1185 2023-05-11 12:10:49.000000 enstools-compression-2023.5/enstools/compression/plugins.py
--rw-rw-rw-   0 root         (0) root         (0)     4660 2023-05-11 12:10:49.000000 enstools-compression-2023.5/enstools/compression/pruner.py
--rw-rw-rw-   0 root         (0) root         (0)    19657 2023-05-11 13:20:17.000000 enstools-compression-2023.5/enstools/compression/significant_bits.py
--rw-rw-rw-   0 root         (0) root         (0)     1674 2023-05-11 12:10:49.000000 enstools-compression-2023.5/enstools/compression/size_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     8244 2023-05-11 12:10:49.000000 enstools-compression-2023.5/enstools/compression/slicing.py
--rw-rw-rw-   0 root         (0) root         (0)     6731 2023-05-11 12:10:49.000000 enstools-compression-2023.5/enstools/compression/xr_accessor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:11:19.354095 enstools-compression-2023.5/enstools_compression.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1660 2023-05-11 15:11:19.000000 enstools-compression-2023.5/enstools_compression.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1267 2023-05-11 15:11:19.000000 enstools-compression-2023.5/enstools_compression.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 15:11:19.000000 enstools-compression-2023.5/enstools_compression.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       71 2023-05-11 15:11:19.000000 enstools-compression-2023.5/enstools_compression.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       74 2023-05-11 15:11:19.000000 enstools-compression-2023.5/enstools_compression.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-11 15:11:19.000000 enstools-compression-2023.5/enstools_compression.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-11 15:11:19.355095 enstools-compression-2023.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1366 2023-01-18 16:33:07.000000 enstools-compression-2023.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:47:57.787129 enstools-compression-2023.6/
+-rw-rw-rw-   0 root         (0) root         (0)    10898 2023-01-18 16:33:07.000000 enstools-compression-2023.6/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       15 2023-01-18 16:33:07.000000 enstools-compression-2023.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1706 2023-06-22 14:47:57.787129 enstools-compression-2023.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1412 2023-01-18 16:33:07.000000 enstools-compression-2023.6/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        7 2023-06-22 14:23:00.000000 enstools-compression-2023.6/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:47:57.782129 enstools-compression-2023.6/enstools/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:47:57.785129 enstools-compression-2023.6/enstools/compression/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-11 12:10:49.000000 enstools-compression-2023.6/enstools/compression/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:47:57.785129 enstools-compression-2023.6/enstools/compression/analyzer/
+-rw-rw-rw-   0 root         (0) root         (0)       53 2023-01-18 16:33:07.000000 enstools-compression-2023.6/enstools/compression/analyzer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4050 2023-05-11 12:10:49.000000 enstools-compression-2023.6/enstools/compression/analyzer/analysis_options.py
+-rw-rw-rw-   0 root         (0) root         (0)     7580 2023-06-14 14:12:35.000000 enstools-compression-2023.6/enstools/compression/analyzer/analyze_data_array.py
+-rwxrwxrwx   0 root         (0) root         (0)    11198 2023-06-14 14:12:35.000000 enstools-compression-2023.6/enstools/compression/analyzer/analyzer.py
+-rw-rw-rw-   0 root         (0) root         (0)    13609 2023-06-14 14:12:35.000000 enstools-compression-2023.6/enstools/compression/analyzer/analyzer_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      617 2023-05-11 12:10:49.000000 enstools-compression-2023.6/enstools/compression/api.py
+-rw-rw-rw-   0 root         (0) root         (0)    19012 2023-05-11 12:10:49.000000 enstools-compression-2023.6/enstools/compression/cli.py
+-rwxrwxrwx   0 root         (0) root         (0)    11108 2023-05-11 12:10:49.000000 enstools-compression-2023.6/enstools/compression/compressor.py
+-rwxrwxrwx   0 root         (0) root         (0)     5492 2023-05-11 12:10:49.000000 enstools-compression-2023.6/enstools/compression/emulation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:47:57.786129 enstools-compression-2023.6/enstools/compression/emulators/
+-rw-rw-rw-   0 root         (0) root         (0)      301 2023-05-11 12:10:49.000000 enstools-compression-2023.6/enstools/compression/emulators/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1176 2023-05-11 12:10:49.000000 enstools-compression-2023.6/enstools/compression/emulators/emulator_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     3412 2023-06-14 14:12:35.000000 enstools-compression-2023.6/enstools/compression/emulators/filters_emulator.py
+-rwxrwxrwx   0 root         (0) root         (0)     4847 2023-05-11 12:10:49.000000 enstools-compression-2023.6/enstools/compression/emulators/libpressio_emulator.py
+-rwxrwxrwx   0 root         (0) root         (0)     2959 2023-05-11 12:10:49.000000 enstools-compression-2023.6/enstools/compression/emulators/zfp_emulator.py
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-06-14 14:12:35.000000 enstools-compression-2023.6/enstools/compression/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     2908 2023-05-11 12:10:49.000000 enstools-compression-2023.6/enstools/compression/evaluator.py
+-rw-rw-rw-   0 root         (0) root         (0)     5369 2023-05-11 12:10:49.000000 enstools-compression-2023.6/enstools/compression/h5netcdf_compressor.py
+-rw-rw-rw-   0 root         (0) root         (0)    12646 2023-05-11 12:10:49.000000 enstools-compression-2023.6/enstools/compression/metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     1185 2023-05-11 12:10:49.000000 enstools-compression-2023.6/enstools/compression/plugins.py
+-rw-rw-rw-   0 root         (0) root         (0)     4660 2023-05-11 12:10:49.000000 enstools-compression-2023.6/enstools/compression/pruner.py
+-rw-rw-rw-   0 root         (0) root         (0)    19657 2023-05-11 13:20:17.000000 enstools-compression-2023.6/enstools/compression/significant_bits.py
+-rw-rw-rw-   0 root         (0) root         (0)     1674 2023-05-11 12:10:49.000000 enstools-compression-2023.6/enstools/compression/size_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     8244 2023-05-11 12:10:49.000000 enstools-compression-2023.6/enstools/compression/slicing.py
+-rw-rw-rw-   0 root         (0) root         (0)     6731 2023-05-11 12:10:49.000000 enstools-compression-2023.6/enstools/compression/xr_accessor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:47:57.787129 enstools-compression-2023.6/enstools_compression.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1706 2023-06-22 14:47:57.000000 enstools-compression-2023.6/enstools_compression.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1298 2023-06-22 14:47:57.000000 enstools-compression-2023.6/enstools_compression.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 14:47:57.000000 enstools-compression-2023.6/enstools_compression.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       71 2023-06-22 14:47:57.000000 enstools-compression-2023.6/enstools_compression.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      125 2023-06-22 14:47:57.000000 enstools-compression-2023.6/enstools_compression.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-22 14:47:57.000000 enstools-compression-2023.6/enstools_compression.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 14:47:57.787129 enstools-compression-2023.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1541 2023-06-22 14:23:00.000000 enstools-compression-2023.6/setup.py
```

### Comparing `enstools-compression-2023.5/LICENSE` & `enstools-compression-2023.6/LICENSE`

 * *Files identical despite different names*

### Comparing `enstools-compression-2023.5/PKG-INFO` & `enstools-compression-2023.6/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: enstools-compression
-Version: 2023.5
-Home-page: https://github.com/wavestoweather/enstools-compression
-Author: Oriol Tintó
-Author-email: oriol.tinto@lmu.de
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # enstools-compression [![Documentation Status](https://readthedocs.org/projects/enstools/badge/?version=latest)](https://enstools-compression.readthedocs.io/en/latest/?badge=latest)
 
 
 This package extends [enstools](github.com/wavestoweather/enstools) to enable **lossy** and **lossless** compression 
 by using **HDF5 filters**.
 
 Also, it contains a set of tools to help to find appropriate compression specifications.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `enstools-compression-2023.5/README.md` & `enstools-compression-2023.6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: enstools-compression
+Version: 2023.6
+Home-page: https://github.com/wavestoweather/enstools-compression
+Author: Oriol Tintó
+Author-email: oriol.tinto@lmu.de
+Description-Content-Type: text/markdown
+Provides-Extra: examples
+Provides-Extra: test
+License-File: LICENSE
+
 # enstools-compression [![Documentation Status](https://readthedocs.org/projects/enstools/badge/?version=latest)](https://enstools-compression.readthedocs.io/en/latest/?badge=latest)
 
 
 This package extends [enstools](github.com/wavestoweather/enstools) to enable **lossy** and **lossless** compression 
 by using **HDF5 filters**.
 
 Also, it contains a set of tools to help to find appropriate compression specifications.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `enstools-compression-2023.5/enstools/compression/analyzer/analysis_options.py` & `enstools-compression-2023.6/enstools/compression/analyzer/analysis_options.py`

 * *Files identical despite different names*

### Comparing `enstools-compression-2023.5/enstools/compression/analyzer/analyze_data_array.py` & `enstools-compression-2023.6/enstools/compression/analyzer/analyze_data_array.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,77 +13,89 @@
 import logging
 import warnings
 from typing import Tuple, Callable
 
 import numpy as np
 import xarray
 
+import enstools.encoding.chunk_size
 from enstools.compression.emulators import DefaultEmulator
+from enstools.compression.errors import ConditionsNotFulfilledError
+from enstools.compression.slicing import MultiDimensionalSliceCollection
 from enstools.encoding.api import VariableEncoding
+from enstools.encoding.dataset_encoding import find_chunk_sizes, convert_to_bytes
 from enstools.encoding.rules import COMPRESSION_SPECIFICATION_SEPARATOR
 from .analysis_options import AnalysisOptions
 from .analyzer_utils import get_metrics, get_parameter_range, bisection_method
 
 # These metrics will be used to select within the different encodings when aiming at a certain compression ratio.
 ANALYSIS_DIAGNOSTIC_METRICS = ["correlation_I", "ssim_I"]
 COMPRESSION_RATIO_LABEL = "compression_ratio"
 
 COUNTER = 0
 
 
 def find_direct_relation(parameter_range, function_to_nullify):
     """Return whether the nullified function has a direct relation between the parameter and the nullified value."""
     min_val, max_val = parameter_range
-    first_q = min_val + (max_val - min_val) / 10
-    third_q = min_val + 9 * (max_val - min_val) / 10
+    first_percentile = min_val + (max_val - min_val) / 100
+    last_percentile = min_val + 99 * (max_val - min_val) / 100
+
+    eval_first_percentile = function_to_nullify(first_percentile)
+    eval_last_percentile = function_to_nullify(last_percentile)
+    return eval_last_percentile > eval_first_percentile
+
+
+def  get_one_slice(data_array: xarray.DataArray, chunk_size: str = "100KB"):
+    chunk_memory_size = convert_to_bytes(chunk_size)
+    chunk_sizes = find_chunk_sizes(data_array, chunk_memory_size)
+    chunk_sizes = [chunk_sizes[dim] for dim in data_array.dims]
+    multi_dimensional_slice = MultiDimensionalSliceCollection(shape=data_array.shape, chunk_sizes=chunk_sizes)
+    big_chunk_size = max(set([s.size for s in multi_dimensional_slice.objects.ravel()]))
+    big_chunks = [s for s in multi_dimensional_slice.objects.ravel() if s.size == big_chunk_size]
+
+    return {dim: size for dim, size in zip(data_array.dims, big_chunks[0].slices)}
 
-    eval_first_q = function_to_nullify(first_q)
-    eval_third_q = function_to_nullify(third_q)
-    return eval_third_q > eval_first_q
 
 
 def analyze_data_array(data_array: xarray.DataArray, options: AnalysisOptions) -> Tuple[str, dict]:
     """
     Find the compression specification corresponding to a certain data array and a given set of compression options.
     """
-    # In case there is a time dimension, select the last element.
-    # There are accumulative variables (like total precipitation) which have mostly 0 on the first time step.
-    # Using the last time-step can represent an advantage somehow.
-    if "time" in data_array.dims:
-        data_array = data_array.isel(time=-1)
+
+    slices = get_one_slice(data_array,
+                           chunk_size=enstools.encoding.chunk_size.analysis_chunk_size)
+    data_array = data_array.isel(**slices)
     # Check if the array contains any nan
     contains_nan = np.isnan(data_array.values).any()
     if contains_nan:
         logging.warning("The variable %scontains NaN. Falling to 'lossless'.\n"
                         "It is possible to prevent that replacing the NaN values using the parameter --fill-na",
                         data_array.name)
         return "lossless", {**{COMPRESSION_RATIO_LABEL: 1.0}, **{met: 0. for met in ANALYSIS_DIAGNOSTIC_METRICS}}
 
     # Define the functions that will be used to find optimal parameters
     get_metric_from_parameter, function_to_nullify, constrain = define_functions_to_optimize(data_array, options)
 
     # Define parameter range
     parameter_range = get_parameter_range(data_array, options)
 
-    # If the aim is a specific compression ratio, the parameter range needs to be reversed
-    # because the relation between compression ratio and quality is inverse.
-    # if COMPRESSION_RATIO_LABEL in options.thresholds:
-    #     parameter_range = tuple(reversed(parameter_range))
-
     #  Ignore warnings
     with warnings.catch_warnings():
         warnings.simplefilter("ignore")
         direct_relation = find_direct_relation(parameter_range=parameter_range, function_to_nullify=function_to_nullify)
         # Use bisection method to find optimal compression parameter.
         parameter = bisection_method(
             parameter_range,
             constrain=constrain,
             fun=function_to_nullify,
             direct_relation=direct_relation)
 
+        if not constrain(parameter):
+            raise ConditionsNotFulfilledError("Condition not fulfilled!")
         # Compute metrics
         # When aiming for a compression ratio some other metrics need to be provided too.
         if COMPRESSION_RATIO_LABEL not in options.thresholds:
             metrics = get_metric_from_parameter(parameter)
         else:
             new_options = copy.deepcopy(options)
             for metric in ANALYSIS_DIAGNOSTIC_METRICS:
```

### Comparing `enstools-compression-2023.5/enstools/compression/analyzer/analyzer.py` & `enstools-compression-2023.6/enstools/compression/analyzer/analyzer.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import xarray
 import yaml
 
 from enstools.compression.compressor import drop_variables
 from enstools.io import read
 from .analysis_options import AnalysisOptions, AnalysisParameters
 from .analyze_data_array import analyze_data_array, ANALYSIS_DIAGNOSTIC_METRICS, COMPRESSION_RATIO_LABEL
+from ..errors import ConditionsNotFulfilledError
 
 logger = logging.getLogger("enstools.compression.analysis")
 
 
 def find_optimal_encoding(dataset: xarray.Dataset, options: AnalysisOptions):
     """
     Given a dataset, find the optimal compression parameters.
@@ -63,15 +64,16 @@
     combinations = [*encodings]
     variables = [*encodings[combinations[0]]]
 
     best_combination = {}
     for variable in variables:
         best_compression_ratio = 0
         for combination in combinations:
-            if metrics[combination][variable][COMPRESSION_RATIO_LABEL] > best_compression_ratio:
+            if variable in metrics[combination] and \
+                    metrics[combination][variable][COMPRESSION_RATIO_LABEL] > best_compression_ratio:
                 best_compression_ratio = metrics[combination][variable][COMPRESSION_RATIO_LABEL]
                 best_combination[variable] = combination
 
     selected_encodings = {variable: encodings[combination][variable] for variable, combination in
                           best_combination.items()}
     selected_metrics = {variable: metrics[combination][variable] for variable, combination in
                         best_combination.items()}
@@ -89,15 +91,15 @@
 
     best_combination = {}
 
     for variable in variables:
         best_metrics = {met: -1.0 for met in ANALYSIS_DIAGNOSTIC_METRICS}
         for combination in combinations:
             for metric in ANALYSIS_DIAGNOSTIC_METRICS:
-                if metric in metrics[combination][variable]:
+                if variable in metrics[combination] and metric in metrics[combination][variable]:
                     if metrics[combination][variable][metric] > best_metrics[metric]:
                         best_metrics[metric] = metrics[combination][variable][metric]
                         best_combination[variable] = combination
     selected_encodings = {variable: encodings[combination][variable] for variable, combination in
                           best_combination.items()}
     selected_metrics = {variable: metrics[combination][variable] for variable, combination in
                         best_combination.items()}
@@ -141,26 +143,29 @@
                 continue
             if not np.issubdtype(dataset[var].dtype, np.floating):
                 logger.debug("Variable %s is not a float, it is %s. Going with lossless.", var, dataset[var].dtype)
                 combination_encoding[var] = "lossless"
                 combination_metrics[var] = {COMPRESSION_RATIO_LABEL: 1.0}
                 continue
 
-            variable_encoding, variable_metrics = analyze_data_array(
-                data_array=dataset[var],
-                options=AnalysisOptions(compressor, mode, thresholds=options.thresholds)
-            )
-            combination_encoding[var] = variable_encoding
-            combination_metrics[var] = variable_metrics
-            # (dataset, variable_name, thresholds, compressor_name, mode)
-            logger.debug("%s %s  CR:%.1f",
-                         var,
-                         variable_encoding,
-                         variable_metrics[COMPRESSION_RATIO_LABEL],
-                         )
+            try:
+                variable_encoding, variable_metrics = analyze_data_array(
+                    data_array=dataset[var],
+                    options=AnalysisOptions(compressor, mode, thresholds=options.thresholds)
+                )
+                combination_encoding[var] = variable_encoding
+                combination_metrics[var] = variable_metrics
+                # (dataset, variable_name, thresholds, compressor_name, mode)
+                logger.debug("%s %s  CR:%.1f",
+                             var,
+                             variable_encoding,
+                             variable_metrics[COMPRESSION_RATIO_LABEL],
+                             )
+            except ConditionsNotFulfilledError:
+                ...
         encodings[combination] = combination_encoding
         metrics[combination] = combination_metrics
 
     return encodings, metrics
 
 
 def analyze_files(file_paths: Union[Path, List[Path]],
@@ -236,15 +241,20 @@
     if variables is not None:
         dataset = drop_variables(dataset, variables)
 
     if fill_na is not False:
         dataset = dataset.fillna(fill_na)
 
     options = AnalysisOptions(compressor=compressor, mode=mode, constrains=constrains)
-    return find_optimal_encoding(dataset, options)
+    encodings, metrics = find_optimal_encoding(dataset, options)
+    if not encodings:
+        raise ConditionsNotFulfilledError(
+            "It was not possible to find a combination that fulfills the constrains provided"
+        )
+    return encodings, metrics
 
 
 def save_encoding(encoding: dict, output_file: Union[Path, str, None] = None, file_format: str = "yaml"):
     """
     Output the encoding dictionary to a file or to the stdout.
     :param encoding:
     :param output_file:
```

### Comparing `enstools-compression-2023.5/enstools/compression/analyzer/analyzer_utils.py` & `enstools-compression-2023.6/enstools/compression/analyzer/analyzer_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 This module contains some helper functions that are used in analyzer.
 """
 
 import logging
 from typing import List, Dict
 
 import xarray
+import numpy as np
 
 from enstools.compression.analyzer.analysis_options import AnalysisOptions
 from enstools.compression.metrics import DataArrayMetrics
 from enstools.core.errors import EnstoolsError
 from enstools.encoding.definitions import lossy_compressors_and_modes
 
 
@@ -19,15 +20,16 @@
     Calculates the requested metrics for a given pair of reference and recovered data arrays.
     :param reference_data: the reference data array
     :param recovered_data: the recovered data array
     :param metric_names: a list of metric names to calculate
     :return: a dictionary with the requested metrics
     """
     metrics = DataArrayMetrics(reference_data, recovered_data)
-    return {metric: float(metrics[metric]) for metric in metric_names if metric != "compression_ratio"}
+    # TODO: Is the average the proper thing to use here?
+    return {metric: float(np.average(metrics[metric])) for metric in metric_names if metric != "compression_ratio"}
 
 
 def check_compression_ratio(compression_ratio: float, thresholds: dict):
     """
     Checks whether the given compression ratio is above the given threshold.
     :param compression_ratio: the compression ratio to check
     :param thresholds: a dictionary containing the threshold values
@@ -144,14 +146,15 @@
                                 constrain: callable = None,
                                 depth: int = 0,
                                 max_depth: int = 50,
                                 last_value=None,
                                 retry_repeated=5,
                                 threshold=0.1,
                                 direct_relation=True,
+                                results=None,
                                 ):
     """
     Recursively refine a parameter range by evaluating the parameter that lies in the middle of the range.
     If the evaluation of the middle parameter returns a value greater than zero,
     the looser half of the parameter range is rejected.
     Otherwise, the tighter half of the parameter range is rejected.
     This way the bisection is iterated until the exit conditions are met.
@@ -164,74 +167,80 @@
     :param max_depth: The maximum allowed depth of the recursion.
     :param last_value: The result of the previous call to fun.
     :param retry_repeated: The number of times the function will retry if the result is repeated (e.g., is 0.0 twice).
     :param threshold: The threshold that will stop the bisection if a value less than the threshold is obtained.
     :param direct_relation: If True, the relation between the function and the parameter is direct, that is,
                             increasing the parameter will increase the function value. If False, the relation is
                             inverse, that is, increasing the parameter will decrease the function value.
+    :param results: A dictionary that stores the function values for each parameter that has been evaluated.
+
     :return: The best value of the parameter that meets the exit conditions.
     """
+
+    if results is None:
+        results = {}
     # Get start and end from parameter range
     start, end = parameter_range
 
     # Get the middle point
     middle = (start + end) / 2
 
     def comparison(value_at_middle: float, direct_relation: bool = True):
         return (value_at_middle > 0.0) == direct_relation
 
     # Evaluate at the middle point
     value_at_middle = fun(middle)
     # TODO: use logging and a debug mode to print this kind of things
     logging.debug("start=%.2e,end=%.2e value_at_middle=%f", start, end, float(value_at_middle))
 
-    # If the value at the middle is positive (all thresholds are fulfilled) we can return the parameter at the middle,
-    # otherwise select the safer one.
-    parameter_to_return = middle if value_at_middle > 0.0 else end
+    # Save result
+    results[middle] = value_at_middle
 
     # In case the accuracy exit condition is reached, return the parameter value at that point
-    if 0.0 <= value_at_middle < threshold:
-        return parameter_to_return
+    if 0.0 <= value_at_middle < threshold or depth >= max_depth or\
+            (value_at_middle == last_value and retry_repeated == 0):
+        positive_results = {k: v for k,v in results.items() if v > 0}
+        if positive_results:
+            return min(positive_results, key=positive_results.get)
+        else:
+            return middle
+
 
     # If the value is the same that the last try, we can retry few times
     if value_at_middle == last_value:
-        if retry_repeated == 0:
-            return parameter_to_return
         retry_repeated -= 1
 
-    # In case having reached the maximum depth, return the proper value
-    if depth >= max_depth:
-        return parameter_to_return
-
     # # Otherwise, set new parameter range and call the function again
     if comparison(value_at_middle, direct_relation=direct_relation):
         new_start, new_end = start, middle
     else:
         new_start, new_end = middle, end
 
     return continuous_bisection_method((new_start, new_end),
                                        fun=fun,
                                        constrain=constrain,
                                        depth=depth + 1,
                                        last_value=value_at_middle,
                                        retry_repeated=retry_repeated,
                                        threshold=threshold,
                                        direct_relation=direct_relation,
+                                       results=results
                                        )
 
 
 def discrete_bisection_method(parameters_list: list,
                               fun: callable = None,
                               constrain: callable = None,
                               depth: int = 0,
                               max_depth: int = 50,
                               last_value=None,
                               retry_repeated=5,
                               threshold=0.1,
                               direct_relation=True,
+                              results=None,
                               ):
     """
     Apply the bisection method on a set of discrete parameters.
 
     :param parameters_list: List of discrete parameters.
     :param fun: Callable function to apply the method.
     :param constrain: Callable function that will return a boolean indicating if a parameter is within the defined
@@ -239,48 +248,57 @@
     :param depth: Current depth of the recursive call.
     :param max_depth: Maximum depth of the recursive call.
     :param last_value: The last value tried by the method.
     :param retry_repeated: Number of times to retry when the value is repeated.
     :param threshold: The threshold for the method exit condition.
     :param direct_relation: Boolean indicating whether the relation between the parameter and the function value is
     direct or inverse.
+    :param results: A dictionary that stores the function values for each parameter that has been evaluated.
 
     :return: The parameter value that satisfies the constrain function.
 
     :raises: Exception if the maximum depth is reached.
     """
+
+    if results is None:
+        results = {}
+
     middle_index = len(parameters_list) // 2
     middle = parameters_list[middle_index]
 
     def comparison(value_at_middle: float, direct_relation: bool = True):
         return (value_at_middle > 0.0) == direct_relation
 
     # Evaluate at the middle point
     value_at_middle = fun(middle)
     logging.debug("middle: %f value_at_middle: %f",
                   middle,
                   float(value_at_middle))
 
+    results[middle] = value_at_middle
+
     # If the value at the middle is positive (all thresholds are fulfilled) we can return the parameter at the middle,
     # otherwise select the safer one.
     parameter_to_return = middle if value_at_middle > 0.0 else parameters_list[-1]
 
     # In case the accuracy exit condition is reached, return the parameter value at that point
-    if 0.0 <= value_at_middle < threshold:
-        return parameter_to_return
+    if 0.0 <= value_at_middle < threshold or depth >= max_depth or\
+            (value_at_middle == last_value and retry_repeated == 0):
+        positive_results = {k: v for k,v in results.items() if v > 0}
+        if positive_results:
+            return min(positive_results, key=positive_results.get)
+        else:
+            return middle
 
     # If the value is the same that the last try, we can retry few times
     if value_at_middle == last_value:
         if retry_repeated == 0:
             return parameter_to_return
         retry_repeated -= 1
 
-    # In case having reached the maximum depth, return the proper value
-    if depth >= max_depth:
-        return parameter_to_return
 
     # # Otherwise, set new parameter range and call the function again
     if comparison(value_at_middle, direct_relation=direct_relation):
         new_parameters_list = parameters_list[:middle_index]
 
     else:
         new_parameters_list = parameters_list[middle_index:]
@@ -289,8 +307,9 @@
                                      fun=fun,
                                      constrain=constrain,
                                      depth=depth + 1,
                                      last_value=value_at_middle,
                                      retry_repeated=retry_repeated,
                                      threshold=threshold,
                                      direct_relation=direct_relation,
+                                     results=results,
                                      )
```

### Comparing `enstools-compression-2023.5/enstools/compression/api.py` & `enstools-compression-2023.6/enstools/compression/api.py`

 * *Files identical despite different names*

### Comparing `enstools-compression-2023.5/enstools/compression/cli.py` & `enstools-compression-2023.6/enstools/compression/cli.py`

 * *Files identical despite different names*

### Comparing `enstools-compression-2023.5/enstools/compression/compressor.py` & `enstools-compression-2023.6/enstools/compression/compressor.py`

 * *Files identical despite different names*

### Comparing `enstools-compression-2023.5/enstools/compression/emulation.py` & `enstools-compression-2023.6/enstools/compression/emulation.py`

 * *Files identical despite different names*

### Comparing `enstools-compression-2023.5/enstools/compression/emulators/emulator_class.py` & `enstools-compression-2023.6/enstools/compression/emulators/emulator_class.py`

 * *Files identical despite different names*

### Comparing `enstools-compression-2023.5/enstools/compression/emulators/filters_emulator.py` & `enstools-compression-2023.6/enstools/compression/emulators/filters_emulator.py`

 * *Files 6% similar despite different names*

```diff
@@ -82,14 +82,16 @@
         # Calculate uncompressed size
         uncompressed_size = uncompressed_data.dtype.itemsize * uncompressed_data.size
 
         # If the key "chunksizes" is inside the encoding, we need to rename it.
         encoding = dict(self.compression)
         if "chunksizes" in encoding:
             encoding["chunks"] = encoding.pop("chunksizes")
+        else:
+            encoding["chunks"] = uncompressed_data.shape
 
         # Initialize file object
         with io.BytesIO() as bio:
 
             # Compress data
             with h5py.File(bio, mode='w') as temporary_file:
                 temporary_file.create_dataset(dummy_var, data=uncompressed_data, **encoding)
```

### Comparing `enstools-compression-2023.5/enstools/compression/emulators/libpressio_emulator.py` & `enstools-compression-2023.6/enstools/compression/emulators/libpressio_emulator.py`

 * *Files identical despite different names*

### Comparing `enstools-compression-2023.5/enstools/compression/emulators/zfp_emulator.py` & `enstools-compression-2023.6/enstools/compression/emulators/zfp_emulator.py`

 * *Files identical despite different names*

### Comparing `enstools-compression-2023.5/enstools/compression/evaluator.py` & `enstools-compression-2023.6/enstools/compression/evaluator.py`

 * *Files identical despite different names*

### Comparing `enstools-compression-2023.5/enstools/compression/h5netcdf_compressor.py` & `enstools-compression-2023.6/enstools/compression/h5netcdf_compressor.py`

 * *Files identical despite different names*

### Comparing `enstools-compression-2023.5/enstools/compression/metrics.py` & `enstools-compression-2023.6/enstools/compression/metrics.py`

 * *Files identical despite different names*

### Comparing `enstools-compression-2023.5/enstools/compression/plugins.py` & `enstools-compression-2023.6/enstools/compression/plugins.py`

 * *Files identical despite different names*

### Comparing `enstools-compression-2023.5/enstools/compression/pruner.py` & `enstools-compression-2023.6/enstools/compression/pruner.py`

 * *Files identical despite different names*

### Comparing `enstools-compression-2023.5/enstools/compression/significant_bits.py` & `enstools-compression-2023.6/enstools/compression/significant_bits.py`

 * *Files identical despite different names*

### Comparing `enstools-compression-2023.5/enstools/compression/size_metrics.py` & `enstools-compression-2023.6/enstools/compression/size_metrics.py`

 * *Files identical despite different names*

### Comparing `enstools-compression-2023.5/enstools/compression/slicing.py` & `enstools-compression-2023.6/enstools/compression/slicing.py`

 * *Files identical despite different names*

### Comparing `enstools-compression-2023.5/enstools/compression/xr_accessor.py` & `enstools-compression-2023.6/enstools/compression/xr_accessor.py`

 * *Files identical despite different names*

### Comparing `enstools-compression-2023.5/enstools_compression.egg-info/PKG-INFO` & `enstools-compression-2023.6/enstools_compression.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: enstools-compression
-Version: 2023.5
+Version: 2023.6
 Home-page: https://github.com/wavestoweather/enstools-compression
 Author: Oriol Tintó
 Author-email: oriol.tinto@lmu.de
 Description-Content-Type: text/markdown
+Provides-Extra: examples
+Provides-Extra: test
 License-File: LICENSE
 
 # enstools-compression [![Documentation Status](https://readthedocs.org/projects/enstools/badge/?version=latest)](https://enstools-compression.readthedocs.io/en/latest/?badge=latest)
 
 
 This package extends [enstools](github.com/wavestoweather/enstools) to enable **lossy** and **lossless** compression 
 by using **HDF5 filters**.
```

### Comparing `enstools-compression-2023.5/enstools_compression.egg-info/SOURCES.txt` & `enstools-compression-2023.6/enstools_compression.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 VERSION
 setup.py
 enstools/compression/__init__.py
 enstools/compression/api.py
 enstools/compression/cli.py
 enstools/compression/compressor.py
 enstools/compression/emulation.py
+enstools/compression/errors.py
 enstools/compression/evaluator.py
 enstools/compression/h5netcdf_compressor.py
 enstools/compression/metrics.py
 enstools/compression/plugins.py
 enstools/compression/pruner.py
 enstools/compression/significant_bits.py
 enstools/compression/size_metrics.py
```

### Comparing `enstools-compression-2023.5/setup.py` & `enstools-compression-2023.6/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -36,18 +36,27 @@
       long_description_content_type='text/markdown',
       url="https://github.com/wavestoweather/enstools-compression",
 
       packages=find_enstools_packages(),
 
       install_requires=[
           "enstools>=2023.1",
-          "enstools-encoding>=2023.1",
+          "enstools-encoding>=2023.6",
           "zfpy",
-          "hdf5plugin>=4.0.0",
+          "hdf5plugin>=4.1.3",
           "netCDF4",
       ],
+      extras_require={
+          'examples': ['pooch'],
+          'test': [
+              "pytest",
+              "pytest-mock",
+              "pooch",
+          ],
+      },
+
       entry_points={
           'console_scripts': [
               'enstools-compression=enstools.compression.cli:main'
           ],
       },
       )
```

