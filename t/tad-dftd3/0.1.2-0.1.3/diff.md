# Comparing `tmp/tad_dftd3-0.1.2.tar.gz` & `tmp/tad_dftd3-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tad_dftd3-0.1.2.tar", last modified: Tue May 30 06:48:13 2023, max compression
+gzip compressed data, was "tad_dftd3-0.1.3.tar", last modified: Thu Jun 22 14:13:53 2023, max compression
```

## Comparing `tad_dftd3-0.1.2.tar` & `tad_dftd3-0.1.3.tar`

### file list

```diff
@@ -1,38 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:48:13.358463 tad_dftd3-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-30 06:48:02.000000 tad_dftd3-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10231 2023-05-30 06:48:13.358463 tad_dftd3-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9443 2023-05-30 06:48:02.000000 tad_dftd3-0.1.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-30 06:48:02.000000 tad_dftd3-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-30 06:48:13.358463 tad_dftd3-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-30 06:48:02.000000 tad_dftd3-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:48:13.350463 tad_dftd3-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:48:13.358463 tad_dftd3-0.1.2/src/tad_dftd3/
--rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-05-30 06:48:02.000000 tad_dftd3-0.1.2/src/tad_dftd3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-30 06:48:02.000000 tad_dftd3-0.1.2/src/tad_dftd3/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-30 06:48:02.000000 tad_dftd3-0.1.2/src/tad_dftd3/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:48:13.358463 tad_dftd3-0.1.2/src/tad_dftd3/damping/
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-30 06:48:02.000000 tad_dftd3-0.1.2/src/tad_dftd3/damping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-05-30 06:48:02.000000 tad_dftd3-0.1.2/src/tad_dftd3/damping/atm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-05-30 06:48:02.000000 tad_dftd3-0.1.2/src/tad_dftd3/damping/rational.py
--rw-r--r--   0 runner    (1001) docker     (123)    75725 2023-05-30 06:48:02.000000 tad_dftd3-0.1.2/src/tad_dftd3/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-30 06:48:02.000000 tad_dftd3-0.1.2/src/tad_dftd3/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     7610 2023-05-30 06:48:02.000000 tad_dftd3-0.1.2/src/tad_dftd3/disp.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-30 06:48:02.000000 tad_dftd3-0.1.2/src/tad_dftd3/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-05-30 06:48:02.000000 tad_dftd3-0.1.2/src/tad_dftd3/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-05-30 06:48:02.000000 tad_dftd3-0.1.2/src/tad_dftd3/ncoord.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 06:48:02.000000 tad_dftd3-0.1.2/src/tad_dftd3/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   893128 2023-05-30 06:48:02.000000 tad_dftd3-0.1.2/src/tad_dftd3/reference-c6.npy
--rw-r--r--   0 runner    (1001) docker     (123)    12169 2023-05-30 06:48:02.000000 tad_dftd3-0.1.2/src/tad_dftd3/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-05-30 06:48:02.000000 tad_dftd3-0.1.2/src/tad_dftd3/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)    10832 2023-05-30 06:48:02.000000 tad_dftd3-0.1.2/src/tad_dftd3/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:48:13.358463 tad_dftd3-0.1.2/src/tad_dftd3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10231 2023-05-30 06:48:13.000000 tad_dftd3-0.1.2/src/tad_dftd3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-30 06:48:13.000000 tad_dftd3-0.1.2/src/tad_dftd3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 06:48:13.000000 tad_dftd3-0.1.2/src/tad_dftd3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-30 06:48:13.000000 tad_dftd3-0.1.2/src/tad_dftd3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-30 06:48:13.000000 tad_dftd3-0.1.2/src/tad_dftd3.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:48:13.358463 tad_dftd3-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-05-30 06:48:02.000000 tad_dftd3-0.1.2/tests/test_dftd3.py
--rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-05-30 06:48:02.000000 tad_dftd3-0.1.2/tests/test_disp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-05-30 06:48:02.000000 tad_dftd3-0.1.2/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-05-30 06:48:02.000000 tad_dftd3-0.1.2/tests/test_ncoord.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:13:53.497841 tad_dftd3-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-22 14:13:44.000000 tad_dftd3-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10231 2023-06-22 14:13:53.497841 tad_dftd3-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9443 2023-06-22 14:13:44.000000 tad_dftd3-0.1.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-22 14:13:44.000000 tad_dftd3-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-22 14:13:53.501841 tad_dftd3-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-22 14:13:44.000000 tad_dftd3-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:13:53.493842 tad_dftd3-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:13:53.497841 tad_dftd3-0.1.3/src/tad_dftd3/
+-rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-06-22 14:13:44.000000 tad_dftd3-0.1.3/src/tad_dftd3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-22 14:13:44.000000 tad_dftd3-0.1.3/src/tad_dftd3/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-22 14:13:44.000000 tad_dftd3-0.1.3/src/tad_dftd3/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:13:53.497841 tad_dftd3-0.1.3/src/tad_dftd3/damping/
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-22 14:13:44.000000 tad_dftd3-0.1.3/src/tad_dftd3/damping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-06-22 14:13:44.000000 tad_dftd3-0.1.3/src/tad_dftd3/damping/atm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-06-22 14:13:44.000000 tad_dftd3-0.1.3/src/tad_dftd3/damping/rational.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75725 2023-06-22 14:13:44.000000 tad_dftd3-0.1.3/src/tad_dftd3/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-22 14:13:44.000000 tad_dftd3-0.1.3/src/tad_dftd3/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7610 2023-06-22 14:13:44.000000 tad_dftd3-0.1.3/src/tad_dftd3/disp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-22 14:13:44.000000 tad_dftd3-0.1.3/src/tad_dftd3/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-06-22 14:13:44.000000 tad_dftd3-0.1.3/src/tad_dftd3/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-06-22 14:13:44.000000 tad_dftd3-0.1.3/src/tad_dftd3/ncoord.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 14:13:44.000000 tad_dftd3-0.1.3/src/tad_dftd3/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   893128 2023-06-22 14:13:44.000000 tad_dftd3-0.1.3/src/tad_dftd3/reference-c6.npy
+-rw-r--r--   0 runner    (1001) docker     (123)    12169 2023-06-22 14:13:44.000000 tad_dftd3-0.1.3/src/tad_dftd3/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-06-22 14:13:44.000000 tad_dftd3-0.1.3/src/tad_dftd3/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:13:53.497841 tad_dftd3-0.1.3/src/tad_dftd3/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-22 14:13:44.000000 tad_dftd3-0.1.3/src/tad_dftd3/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-06-22 14:13:44.000000 tad_dftd3-0.1.3/src/tad_dftd3/util/distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-06-22 14:13:44.000000 tad_dftd3-0.1.3/src/tad_dftd3/util/grad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-06-22 14:13:44.000000 tad_dftd3-0.1.3/src/tad_dftd3/util/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:13:53.497841 tad_dftd3-0.1.3/src/tad_dftd3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10231 2023-06-22 14:13:53.000000 tad_dftd3-0.1.3/src/tad_dftd3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-22 14:13:53.000000 tad_dftd3-0.1.3/src/tad_dftd3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 14:13:53.000000 tad_dftd3-0.1.3/src/tad_dftd3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-22 14:13:53.000000 tad_dftd3-0.1.3/src/tad_dftd3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-22 14:13:53.000000 tad_dftd3-0.1.3/src/tad_dftd3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:13:53.497841 tad_dftd3-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-06-22 14:13:44.000000 tad_dftd3-0.1.3/tests/test_dftd3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-06-22 14:13:44.000000 tad_dftd3-0.1.3/tests/test_disp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-06-22 14:13:44.000000 tad_dftd3-0.1.3/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-06-22 14:13:44.000000 tad_dftd3-0.1.3/tests/test_ncoord.py
```

### Comparing `tad_dftd3-0.1.2/LICENSE` & `tad_dftd3-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.1.2/PKG-INFO` & `tad_dftd3-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tad_dftd3
-Version: 0.1.2
+Version: 0.1.3
 Summary: Torch autodiff DFT-D3 implementation
 License: Apache-2.0
 Project-URL: Documentation, https://tad-dftd3.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/dftd3/tad-dftd3
 Project-URL: Tracker, https://github.com/dftd3/tad-dftd3/issues
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tad_dftd3-0.1.2/README.rst` & `tad_dftd3-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.1.2/pyproject.toml` & `tad_dftd3-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.1.2/setup.cfg` & `tad_dftd3-0.1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.1.2/setup.py` & `tad_dftd3-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.1.2/src/tad_dftd3/__init__.py` & `tad_dftd3-0.1.3/src/tad_dftd3/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,16 @@
 This module allows to process a single structure or a batch of structures for
 the calculation of atom-resolved dispersion energies.
 
 .. note::
 
    This project is still in early development and the API is subject to change.
    Contributions are welcome, please checkout our
-   `contributing guidelines <https://github.com/dftd3/tad-dftd3/blob/main/CONTRIBUTING.md>`_.
+   `contributing guidelines <https://github.com/dftd3/tad-dftd3/blob/main/\
+    CONTRIBUTING.md>`_.
 
 
 Example
 -------
 >>> import torch
 >>> import tad_dftd3 as d3
 >>> numbers = d3.util.pack((  # S22 system 4: formamide dimer
@@ -69,24 +70,25 @@
 >>> print(energy)  # Energies in Hartree
 tensor([-0.0124292, -0.0045002])
 >>> print(energy[0] - 2*energy[1])
 tensor(-0.0034288)
 """
 import torch
 
-from . import damping, data, disp, model, ncoord, reference, util
+from . import damping, data, disp, model, ncoord, reference
 from .typing import (
     DD,
     CountingFunction,
     DampingFunction,
     Dict,
     Optional,
     Tensor,
     WeightingFunction,
 )
+from .util import misc
 
 
 def dftd3(
     numbers: Tensor,
     positions: Tensor,
     param: Dict[str, Tensor],
     *,
```

### Comparing `tad_dftd3-0.1.2/src/tad_dftd3/__version__.py` & `tad_dftd3-0.1.3/src/tad_dftd3/exception.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,16 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
-Version module for tad_dftd3.
+Possible exceptions which can be raised by this module.
 """
-import torch
 
-__version__ = "0.1.2"
 
-__torch_version__ = tuple(
-    int(x) for x in torch.__version__.split("+", maxsplit=1)[0].split(".")
-)
+class DFTD3Error(Exception):
+    """Base class for exceptions raised by this module."""
+
+    pass
```

### Comparing `tad_dftd3-0.1.2/src/tad_dftd3/constants.py` & `tad_dftd3-0.1.3/src/tad_dftd3/constants.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.1.2/src/tad_dftd3/damping/__init__.py` & `tad_dftd3-0.1.3/src/tad_dftd3/damping/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.1.2/src/tad_dftd3/damping/atm.py` & `tad_dftd3-0.1.3/src/tad_dftd3/damping/atm.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.1.2/src/tad_dftd3/damping/rational.py` & `tad_dftd3-0.1.3/src/tad_dftd3/damping/rational.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.1.2/src/tad_dftd3/data.py` & `tad_dftd3-0.1.3/src/tad_dftd3/data.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.1.2/src/tad_dftd3/defaults.py` & `tad_dftd3-0.1.3/src/tad_dftd3/defaults.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.1.2/src/tad_dftd3/disp.py` & `tad_dftd3-0.1.3/src/tad_dftd3/disp.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.1.2/src/tad_dftd3/exception.py` & `tad_dftd3-0.1.3/src/tad_dftd3/__version__.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
-Possible exceptions which can be raised by this module.
+Version module for tad_dftd3.
 """
+import torch
 
+__version__ = "0.1.3"
 
-class DFTD3Error(Exception):
-    """Base class for exceptions raised by this module."""
-
-    pass
+__torch_version__ = torch.__version__
```

### Comparing `tad_dftd3-0.1.2/src/tad_dftd3/model.py` & `tad_dftd3-0.1.3/src/tad_dftd3/model.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.1.2/src/tad_dftd3/ncoord.py` & `tad_dftd3-0.1.3/src/tad_dftd3/ncoord.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.1.2/src/tad_dftd3/reference-c6.npy` & `tad_dftd3-0.1.3/src/tad_dftd3/reference-c6.npy`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.1.2/src/tad_dftd3/reference.py` & `tad_dftd3-0.1.3/src/tad_dftd3/reference.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.1.2/src/tad_dftd3/typing.py` & `tad_dftd3-0.1.3/src/tad_dftd3/typing.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.1.2/src/tad_dftd3.egg-info/PKG-INFO` & `tad_dftd3-0.1.3/src/tad_dftd3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tad-dftd3
-Version: 0.1.2
+Version: 0.1.3
 Summary: Torch autodiff DFT-D3 implementation
 License: Apache-2.0
 Project-URL: Documentation, https://tad-dftd3.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/dftd3/tad-dftd3
 Project-URL: Tracker, https://github.com/dftd3/tad-dftd3/issues
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tad_dftd3-0.1.2/src/tad_dftd3.egg-info/SOURCES.txt` & `tad_dftd3-0.1.3/src/tad_dftd3.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -12,20 +12,23 @@
 src/tad_dftd3/exception.py
 src/tad_dftd3/model.py
 src/tad_dftd3/ncoord.py
 src/tad_dftd3/py.typed
 src/tad_dftd3/reference-c6.npy
 src/tad_dftd3/reference.py
 src/tad_dftd3/typing.py
-src/tad_dftd3/util.py
 src/tad_dftd3.egg-info/PKG-INFO
 src/tad_dftd3.egg-info/SOURCES.txt
 src/tad_dftd3.egg-info/dependency_links.txt
 src/tad_dftd3.egg-info/requires.txt
 src/tad_dftd3.egg-info/top_level.txt
 src/tad_dftd3/damping/__init__.py
 src/tad_dftd3/damping/atm.py
 src/tad_dftd3/damping/rational.py
+src/tad_dftd3/util/__init__.py
+src/tad_dftd3/util/distance.py
+src/tad_dftd3/util/grad.py
+src/tad_dftd3/util/misc.py
 tests/test_dftd3.py
 tests/test_disp.py
 tests/test_model.py
 tests/test_ncoord.py
```

### Comparing `tad_dftd3-0.1.2/tests/test_dftd3.py` & `tad_dftd3-0.1.3/tests/test_dftd3.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.1.2/tests/test_disp.py` & `tad_dftd3-0.1.3/tests/test_disp.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.1.2/tests/test_model.py` & `tad_dftd3-0.1.3/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.1.2/tests/test_ncoord.py` & `tad_dftd3-0.1.3/tests/test_ncoord.py`

 * *Files identical despite different names*

