# Comparing `tmp/signialib-2.3.0.tar.gz` & `tmp/signialib-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signialib-2.3.0.tar", max compression
+gzip compressed data, was "signialib-2.4.0.tar", max compression
```

## Comparing `signialib-2.3.0.tar` & `signialib-2.4.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1073 2023-04-14 11:54:46.848297 signialib-2.3.0/LICENSE
--rw-r--r--   0        0        0     1805 2023-04-14 11:54:46.852297 signialib-2.3.0/pyproject.toml
--rw-r--r--   0        0        0      584 2023-04-14 11:54:46.852297 signialib-2.3.0/signialib/__init__.py
--rw-r--r--   0        0        0     3998 2023-04-14 11:54:46.852297 signialib-2.3.0/signialib/_session_base.py
--rw-r--r--   0        0        0     2113 2023-04-14 11:54:46.852297 signialib-2.3.0/signialib/calibrations/001/Ferraris/2022-07-24_16-00/001_2022-01-10_10-48.json
--rw-r--r--   0        0        0     2117 2023-04-14 11:54:46.852297 signialib-2.3.0/signialib/calibrations/002/Ferraris/2022-07-24_16-00/002_2022-01-10_10-48.json
--rw-r--r--   0        0        0      600 2023-04-14 11:54:46.852297 signialib-2.3.0/signialib/consts.py
--rwxr-xr-x   0        0        0    28466 2023-04-14 11:54:46.852297 signialib-2.3.0/signialib/dataset.py
--rw-r--r--   0        0        0      265 2023-04-14 11:54:46.852297 signialib-2.3.0/signialib/exceptions.py
--rw-r--r--   0        0        0    11384 2023-04-14 11:54:46.852297 signialib-2.3.0/signialib/header.py
--rwxr-xr-x   0        0        0    10263 2023-04-14 11:54:46.852297 signialib-2.3.0/signialib/session.py
--rwxr-xr-x   0        0        0     1695 2023-04-14 11:54:46.852297 signialib-2.3.0/signialib/utils.py
--rw-r--r--   0        0        0      647 1970-01-01 00:00:00.000000 signialib-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-22 15:35:38.235663 signialib-2.4.0/LICENSE
+-rw-r--r--   0        0        0     1849 2023-06-22 15:35:38.239663 signialib-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0      584 2023-06-22 15:35:38.239663 signialib-2.4.0/signialib/__init__.py
+-rw-r--r--   0        0        0     3998 2023-06-22 15:35:38.239663 signialib-2.4.0/signialib/_session_base.py
+-rw-r--r--   0        0        0     2113 2023-06-22 15:35:38.239663 signialib-2.4.0/signialib/calibrations/001/Ferraris/2022-07-24_16-00/001_2022-01-10_10-48.json
+-rw-r--r--   0        0        0     2117 2023-06-22 15:35:38.239663 signialib-2.4.0/signialib/calibrations/002/Ferraris/2022-07-24_16-00/002_2022-01-10_10-48.json
+-rw-r--r--   0        0        0      600 2023-06-22 15:35:38.239663 signialib-2.4.0/signialib/consts.py
+-rwxr-xr-x   0        0        0    29120 2023-06-22 15:35:38.239663 signialib-2.4.0/signialib/dataset.py
+-rw-r--r--   0        0        0     3244 2023-06-22 15:35:38.239663 signialib-2.4.0/signialib/datastream.py
+-rw-r--r--   0        0        0      265 2023-06-22 15:35:38.239663 signialib-2.4.0/signialib/exceptions.py
+-rw-r--r--   0        0        0    11384 2023-06-22 15:35:38.239663 signialib-2.4.0/signialib/header.py
+-rwxr-xr-x   0        0        0    10565 2023-06-22 15:35:38.239663 signialib-2.4.0/signialib/session.py
+-rwxr-xr-x   0        0        0     1695 2023-06-22 15:35:38.239663 signialib-2.4.0/signialib/utils.py
+-rw-r--r--   0        0        0      733 1970-01-01 00:00:00.000000 signialib-2.4.0/PKG-INFO
```

### Comparing `signialib-2.3.0/LICENSE` & `signialib-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `signialib-2.3.0/pyproject.toml` & `signialib-2.4.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 [tool.poetry]
 name = "signialib"
-version = "2.3.0"
+version = "2.4.0"
 description = "Data handling of the IMUs integrated into Signia hearing aids"
 authors = ["Ann-Kristin Seifer <ann-kristin.seifer@fau.de>", 
         "Arne Küderle <arne.kuederle@fau.de>",
         "Nils Roth <nils.roth@fau.de>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 pandas = "^1"
 scipy = ">=1.6.1,<2.0.0"
 numpy = ">=1"
 joblib = "^1.0.0"
 nilspodlib = "^3.2.2"
+matplotlib = "^3.7.1"
+fau-colors = "^1.6.0"
 
 [tool.poetry.dev-dependencies]
 prospector = "^1.7.7"
 black = "^22.3.0"
 isort = "^5.10.1"
 doit = "^0.32.0"
 poethepoet = "^0.10.0"
```

### Comparing `signialib-2.3.0/signialib/__init__.py` & `signialib-2.4.0/signialib/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 
 from .dataset import Dataset  # noqa: F401
 from .session import Session  # noqa: F401
 
 SIGNIA_CAL_PATH = Path(__file__).parent / "calibrations"
 
 __all__ = ["Dataset", "Session", "SIGNIA_CAL_PATH"]
-__version__ = "2.3.0"
+__version__ = "2.4.0"
```

### Comparing `signialib-2.3.0/signialib/_session_base.py` & `signialib-2.4.0/signialib/_session_base.py`

 * *Files identical despite different names*

### Comparing `signialib-2.3.0/signialib/calibrations/001/Ferraris/2022-07-24_16-00/001_2022-01-10_10-48.json` & `signialib-2.4.0/signialib/calibrations/001/Ferraris/2022-07-24_16-00/001_2022-01-10_10-48.json`

 * *Files identical despite different names*

### Comparing `signialib-2.3.0/signialib/calibrations/002/Ferraris/2022-07-24_16-00/002_2022-01-10_10-48.json` & `signialib-2.4.0/signialib/calibrations/002/Ferraris/2022-07-24_16-00/002_2022-01-10_10-48.json`

 * *Files identical despite different names*

### Comparing `signialib-2.3.0/signialib/consts.py` & `signialib-2.4.0/signialib/consts.py`

 * *Files identical despite different names*

### Comparing `signialib-2.3.0/signialib/dataset.py` & `signialib-2.4.0/signialib/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # -*- coding: utf-8 -*-
 """Dataset represents a measurement session of a single sensor_type."""
 import datetime
 import warnings
 from pathlib import Path
 from typing import TYPE_CHECKING, Dict, Iterable, Optional, Sequence, Tuple, Type, TypeVar, Union
 
+import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from nilspodlib.calibration_utils import find_closest_calibration_to_date, load_and_check_cal_info
-from nilspodlib.datastream import Datastream
 from nilspodlib.exceptions import RepeatedCalibrationError, datastream_does_not_exist_warning
 from nilspodlib.utils import inplace_or_copy, path_t
 
 from signialib.consts import GRAV, SENSOR_MAPPINGS
+from signialib.datastream import Datastream
 from signialib.header import Header
 from signialib.utils import load_matlab
 
 if TYPE_CHECKING:
     from imucal import CalibrationInfo  # noqa: F401
 
 T = TypeVar("T")
@@ -505,14 +506,34 @@
             recursive=recursive,
             filter_cal_type=filter_cal_type,
             before_after=before_after,
             warn_thres=warn_thres,
             ignore_file_not_found=ignore_file_not_found,
         )
 
+    def plot(self, index: str = None):
+        """Plot data.
+
+        Parameters
+        ----------
+        index: {None, "local_datetime"}
+            Defines x axis label ticks of plot. Default is None, i.e. samples.
+
+        """
+        fig = plt.figure()
+        if index == "local_datetime":
+            x_axis = self.local_datetime_counter
+        else:
+            x_axis = self.counter
+        for plot_id, stream in enumerate(self.datastreams):
+            ax = fig.add_subplot(len(self.active_sensors), 1, plot_id + 1)
+            stream[1].plot(ax=ax, x_axis=x_axis)
+            plot_id += 1
+        plt.show()
+
 
 def parse_mat(path: path_t) -> Tuple[Dict[str, np.ndarray], np.ndarray, Header]:
     """Parse a *.mat file and read the header and the data.
 
     Parameters
     ----------
     path :
```

### Comparing `signialib-2.3.0/signialib/header.py` & `signialib-2.4.0/signialib/header.py`

 * *Files identical despite different names*

### Comparing `signialib-2.3.0/signialib/session.py` & `signialib-2.4.0/signialib/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -290,7 +290,18 @@
         if skip_calibration is False:
             s = s.calibrate_imu(
                 self.find_closest_calibration(calib_path, warn_thres=datetime.timedelta(days=60))  # noqa
             )  # noqa
         if resample_rate_hz is not None:
             s = s.resample(resample_rate_hz)
         return s
+
+    def plot(self, index: str = None):
+        """Plot data.
+
+        Parameters
+        ----------
+        index: {None, "local_datetime"}
+            Defines x axis label ticks of plot. Default is None, i.e. samples.
+
+        """
+        self.datasets = [d.plot(index=index) for d in self.datasets]
```

### Comparing `signialib-2.3.0/signialib/utils.py` & `signialib-2.4.0/signialib/utils.py`

 * *Files identical despite different names*

### Comparing `signialib-2.3.0/PKG-INFO` & `signialib-2.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: signialib
-Version: 2.3.0
+Version: 2.4.0
 Summary: Data handling of the IMUs integrated into Signia hearing aids
 Author: Ann-Kristin Seifer
 Author-email: ann-kristin.seifer@fau.de
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: fau-colors (>=1.6.0,<2.0.0)
 Requires-Dist: joblib (>=1.0.0,<2.0.0)
+Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: nilspodlib (>=3.2.2,<4.0.0)
 Requires-Dist: numpy (>=1)
 Requires-Dist: pandas (>=1,<2)
 Requires-Dist: scipy (>=1.6.1,<2.0.0)
```

