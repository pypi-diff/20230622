# Comparing `tmp/meow-sim-0.6.6.tar.gz` & `tmp/meow-sim-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meow-sim-0.6.6.tar", last modified: Thu Jun 22 19:10:01 2023, max compression
+gzip compressed data, was "meow-sim-0.6.7.tar", last modified: Thu Jun 22 19:10:35 2023, max compression
```

## Comparing `meow-sim-0.6.6.tar` & `meow-sim-0.6.7.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 19:10:01.489985 meow-sim-0.6.6/
--rw-r--r--   0 root         (0) root         (0)    11347 2023-06-22 19:09:57.000000 meow-sim-0.6.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3241 2023-06-22 19:10:01.489985 meow-sim-0.6.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2223 2023-06-22 19:09:57.000000 meow-sim-0.6.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 19:10:01.489985 meow-sim-0.6.6/meow/
--rw-r--r--   0 root         (0) root         (0)     1414 2023-06-22 19:09:57.000000 meow-sim-0.6.6/meow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 19:10:01.489985 meow-sim-0.6.6/meow/assets/
--rw-r--r--   0 root         (0) root         (0)    10307 2023-06-22 19:09:57.000000 meow-sim-0.6.6/meow/assets/silicon.csv
--rw-r--r--   0 root         (0) root         (0)     8535 2023-06-22 19:09:57.000000 meow-sim-0.6.6/meow/assets/silicon_oxide.csv
--rw-r--r--   0 root         (0) root         (0)     8378 2023-06-22 19:09:57.000000 meow-sim-0.6.6/meow/base_model.py
--rw-r--r--   0 root         (0) root         (0)     1189 2023-06-22 19:09:57.000000 meow-sim-0.6.6/meow/cache.py
--rw-r--r--   0 root         (0) root         (0)     3855 2023-06-22 19:09:57.000000 meow-sim-0.6.6/meow/cell.py
--rw-r--r--   0 root         (0) root         (0)     6615 2023-06-22 19:09:57.000000 meow-sim-0.6.6/meow/cross_section.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 19:10:01.489985 meow-sim-0.6.6/meow/eme/
--rw-r--r--   0 root         (0) root         (0)      623 2023-06-22 19:09:57.000000 meow-sim-0.6.6/meow/eme/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6066 2023-06-22 19:09:57.000000 meow-sim-0.6.6/meow/eme/common.py
--rw-r--r--   0 root         (0) root         (0)     3889 2023-06-22 19:09:57.000000 meow-sim-0.6.6/meow/eme/sax.py
--rw-r--r--   0 root         (0) root         (0)      551 2023-06-22 19:09:57.000000 meow-sim-0.6.6/meow/environment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 19:10:01.489985 meow-sim-0.6.6/meow/fde/
--rw-r--r--   0 root         (0) root         (0)      324 2023-06-22 19:09:57.000000 meow-sim-0.6.6/meow/fde/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4913 2023-06-22 19:09:57.000000 meow-sim-0.6.6/meow/fde/lumerical.py
--rw-r--r--   0 root         (0) root         (0)     3290 2023-06-22 19:09:57.000000 meow-sim-0.6.6/meow/fde/tidy3d.py
--rw-r--r--   0 root         (0) root         (0)     2318 2023-06-22 19:09:57.000000 meow-sim-0.6.6/meow/gds_structures.py
--rw-r--r--   0 root         (0) root         (0)    10400 2023-06-22 19:09:57.000000 meow-sim-0.6.6/meow/geometries.py
--rw-r--r--   0 root         (0) root         (0)      960 2023-06-22 19:09:57.000000 meow-sim-0.6.6/meow/integrate.py
--rw-r--r--   0 root         (0) root         (0)    12794 2023-06-22 19:09:57.000000 meow-sim-0.6.6/meow/materials.py
--rw-r--r--   0 root         (0) root         (0)     4786 2023-06-22 19:09:57.000000 meow-sim-0.6.6/meow/mesh.py
--rw-r--r--   0 root         (0) root         (0)    17355 2023-06-22 19:09:57.000000 meow-sim-0.6.6/meow/mode.py
--rw-r--r--   0 root         (0) root         (0)     1751 2023-06-22 19:09:57.000000 meow-sim-0.6.6/meow/structures.py
--rw-r--r--   0 root         (0) root         (0)     8099 2023-06-22 19:09:57.000000 meow-sim-0.6.6/meow/visualize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 19:10:01.489985 meow-sim-0.6.6/meow_sim.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3241 2023-06-22 19:10:01.000000 meow-sim-0.6.6/meow_sim.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      686 2023-06-22 19:10:01.000000 meow-sim-0.6.6/meow_sim.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 19:10:01.000000 meow-sim-0.6.6/meow_sim.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      444 2023-06-22 19:10:01.000000 meow-sim-0.6.6/meow_sim.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-22 19:10:01.000000 meow-sim-0.6.6/meow_sim.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1864 2023-06-22 19:09:57.000000 meow-sim-0.6.6/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 19:10:01.489985 meow-sim-0.6.6/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 19:10:01.489985 meow-sim-0.6.6/tests/
--rw-r--r--   0 root         (0) root         (0)     3931 2023-06-22 19:09:57.000000 meow-sim-0.6.6/tests/test_deserialization.py
--rw-r--r--   0 root         (0) root         (0)     3767 2023-06-22 19:09:57.000000 meow-sim-0.6.6/tests/test_mode_operators.py
--rw-r--r--   0 root         (0) root         (0)     1322 2023-06-22 19:09:57.000000 meow-sim-0.6.6/tests/test_nbs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 19:10:35.713666 meow-sim-0.6.7/
+-rw-r--r--   0 root         (0) root         (0)    11347 2023-06-22 19:10:31.000000 meow-sim-0.6.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3241 2023-06-22 19:10:35.713666 meow-sim-0.6.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2223 2023-06-22 19:10:31.000000 meow-sim-0.6.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 19:10:35.713666 meow-sim-0.6.7/meow/
+-rw-r--r--   0 root         (0) root         (0)     1414 2023-06-22 19:10:31.000000 meow-sim-0.6.7/meow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 19:10:35.713666 meow-sim-0.6.7/meow/assets/
+-rw-r--r--   0 root         (0) root         (0)    10307 2023-06-22 19:10:31.000000 meow-sim-0.6.7/meow/assets/silicon.csv
+-rw-r--r--   0 root         (0) root         (0)     8535 2023-06-22 19:10:31.000000 meow-sim-0.6.7/meow/assets/silicon_oxide.csv
+-rw-r--r--   0 root         (0) root         (0)     8378 2023-06-22 19:10:31.000000 meow-sim-0.6.7/meow/base_model.py
+-rw-r--r--   0 root         (0) root         (0)     1189 2023-06-22 19:10:31.000000 meow-sim-0.6.7/meow/cache.py
+-rw-r--r--   0 root         (0) root         (0)     3855 2023-06-22 19:10:31.000000 meow-sim-0.6.7/meow/cell.py
+-rw-r--r--   0 root         (0) root         (0)     6615 2023-06-22 19:10:31.000000 meow-sim-0.6.7/meow/cross_section.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 19:10:35.713666 meow-sim-0.6.7/meow/eme/
+-rw-r--r--   0 root         (0) root         (0)      623 2023-06-22 19:10:31.000000 meow-sim-0.6.7/meow/eme/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6063 2023-06-22 19:10:31.000000 meow-sim-0.6.7/meow/eme/common.py
+-rw-r--r--   0 root         (0) root         (0)     4924 2023-06-22 19:10:31.000000 meow-sim-0.6.7/meow/eme/propagate.py
+-rw-r--r--   0 root         (0) root         (0)     3889 2023-06-22 19:10:31.000000 meow-sim-0.6.7/meow/eme/sax.py
+-rw-r--r--   0 root         (0) root         (0)      551 2023-06-22 19:10:31.000000 meow-sim-0.6.7/meow/environment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 19:10:35.713666 meow-sim-0.6.7/meow/fde/
+-rw-r--r--   0 root         (0) root         (0)      324 2023-06-22 19:10:31.000000 meow-sim-0.6.7/meow/fde/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4913 2023-06-22 19:10:31.000000 meow-sim-0.6.7/meow/fde/lumerical.py
+-rw-r--r--   0 root         (0) root         (0)     3290 2023-06-22 19:10:31.000000 meow-sim-0.6.7/meow/fde/tidy3d.py
+-rw-r--r--   0 root         (0) root         (0)     2318 2023-06-22 19:10:31.000000 meow-sim-0.6.7/meow/gds_structures.py
+-rw-r--r--   0 root         (0) root         (0)    10400 2023-06-22 19:10:31.000000 meow-sim-0.6.7/meow/geometries.py
+-rw-r--r--   0 root         (0) root         (0)      960 2023-06-22 19:10:31.000000 meow-sim-0.6.7/meow/integrate.py
+-rw-r--r--   0 root         (0) root         (0)    12794 2023-06-22 19:10:31.000000 meow-sim-0.6.7/meow/materials.py
+-rw-r--r--   0 root         (0) root         (0)     4786 2023-06-22 19:10:31.000000 meow-sim-0.6.7/meow/mesh.py
+-rw-r--r--   0 root         (0) root         (0)    17355 2023-06-22 19:10:31.000000 meow-sim-0.6.7/meow/mode.py
+-rw-r--r--   0 root         (0) root         (0)     1751 2023-06-22 19:10:31.000000 meow-sim-0.6.7/meow/structures.py
+-rw-r--r--   0 root         (0) root         (0)     8099 2023-06-22 19:10:31.000000 meow-sim-0.6.7/meow/visualize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 19:10:35.713666 meow-sim-0.6.7/meow_sim.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3241 2023-06-22 19:10:35.000000 meow-sim-0.6.7/meow_sim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      708 2023-06-22 19:10:35.000000 meow-sim-0.6.7/meow_sim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 19:10:35.000000 meow-sim-0.6.7/meow_sim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      444 2023-06-22 19:10:35.000000 meow-sim-0.6.7/meow_sim.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-22 19:10:35.000000 meow-sim-0.6.7/meow_sim.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1864 2023-06-22 19:10:31.000000 meow-sim-0.6.7/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 19:10:35.713666 meow-sim-0.6.7/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 19:10:35.713666 meow-sim-0.6.7/tests/
+-rw-r--r--   0 root         (0) root         (0)     3931 2023-06-22 19:10:31.000000 meow-sim-0.6.7/tests/test_deserialization.py
+-rw-r--r--   0 root         (0) root         (0)     3767 2023-06-22 19:10:31.000000 meow-sim-0.6.7/tests/test_mode_operators.py
+-rw-r--r--   0 root         (0) root         (0)     1322 2023-06-22 19:10:31.000000 meow-sim-0.6.7/tests/test_nbs.py
```

### Comparing `meow-sim-0.6.6/LICENSE` & `meow-sim-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.6/PKG-INFO` & `meow-sim-0.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.6.6
+Version: 0.6.7
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `meow-sim-0.6.6/README.md` & `meow-sim-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.6/meow/__init__.py` & `meow-sim-0.6.7/meow/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ MEOW: Modeling of Eigenmodes and Overlaps in Waveguides """
 
 __author__ = "Floris Laporte"
-__version__ = "0.6.6"
+__version__ = "0.6.7"
 
 import warnings
 
 # Silence Excessive Logging...
 
 try:
     from loguru import logger
```

### Comparing `meow-sim-0.6.6/meow/assets/silicon.csv` & `meow-sim-0.6.7/meow/assets/silicon.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.6/meow/assets/silicon_oxide.csv` & `meow-sim-0.6.7/meow/assets/silicon_oxide.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.6/meow/base_model.py` & `meow-sim-0.6.7/meow/base_model.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.6/meow/cache.py` & `meow-sim-0.6.7/meow/cache.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.6/meow/cell.py` & `meow-sim-0.6.7/meow/cell.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.6/meow/cross_section.py` & `meow-sim-0.6.7/meow/cross_section.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.6/meow/eme/__init__.py` & `meow-sim-0.6.7/meow/eme/__init__.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.6/meow/eme/common.py` & `meow-sim-0.6.7/meow/eme/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     if conjugate:
         O_LL = np.real(O_LL)
         O_RR = np.real(O_RR)
 
     # ignoring the phase seems to corresponds best with lumerical.
 
     # alternative phase correction (probably worth testing this out)
-    # Question: is this not just a conjugation?
+    # Question: is this not just an abs ;) ?
     # O_LL = O_LL*np.exp(-1j*np.angle(O_LL))
     # O_RR = O_RR*np.exp(-1j*np.angle(O_RR))
 
     # yet another alternative phase correction (probably worth testing this out too)
     # O_LR = O_LR*np.diag(np.exp(-1j*np.angle(np.diag(O_LR))))
     # O_RL = O_RL*np.diag(np.exp(-1j*np.angle(np.diag(O_RL))))
```

### Comparing `meow-sim-0.6.6/meow/eme/sax.py` & `meow-sim-0.6.7/meow/eme/sax.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.6/meow/environment.py` & `meow-sim-0.6.7/meow/environment.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.6/meow/fde/lumerical.py` & `meow-sim-0.6.7/meow/fde/lumerical.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.6/meow/fde/tidy3d.py` & `meow-sim-0.6.7/meow/fde/tidy3d.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.6/meow/gds_structures.py` & `meow-sim-0.6.7/meow/gds_structures.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.6/meow/geometries.py` & `meow-sim-0.6.7/meow/geometries.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.6/meow/integrate.py` & `meow-sim-0.6.7/meow/integrate.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.6/meow/materials.py` & `meow-sim-0.6.7/meow/materials.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.6/meow/mesh.py` & `meow-sim-0.6.7/meow/mesh.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.6/meow/mode.py` & `meow-sim-0.6.7/meow/mode.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.6/meow/structures.py` & `meow-sim-0.6.7/meow/structures.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.6/meow/visualize.py` & `meow-sim-0.6.7/meow/visualize.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.6/meow_sim.egg-info/PKG-INFO` & `meow-sim-0.6.7/meow_sim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.6.6
+Version: 0.6.7
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `meow-sim-0.6.6/meow_sim.egg-info/SOURCES.txt` & `meow-sim-0.6.7/meow_sim.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 meow/mode.py
 meow/structures.py
 meow/visualize.py
 meow/assets/silicon.csv
 meow/assets/silicon_oxide.csv
 meow/eme/__init__.py
 meow/eme/common.py
+meow/eme/propagate.py
 meow/eme/sax.py
 meow/fde/__init__.py
 meow/fde/lumerical.py
 meow/fde/tidy3d.py
 meow_sim.egg-info/PKG-INFO
 meow_sim.egg-info/SOURCES.txt
 meow_sim.egg-info/dependency_links.txt
```

### Comparing `meow-sim-0.6.6/pyproject.toml` & `meow-sim-0.6.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["build", "pip", "setuptools", "wheel", "pybind11"]
 
 [project]
 name = "meow-sim"
-version = "0.6.6"
+version = "0.6.7"
 authors = [
 { name = "Rockley Photonics" },
 { name = "Floris Laporte", email = "floris.laporte@rockleyphotonics.com" },
 ]
 description = "Modeling of Eigenmodes and Overlaps in Waveguide Structures"
 requires-python = ">=3.8"
 keywords = [
```

### Comparing `meow-sim-0.6.6/tests/test_deserialization.py` & `meow-sim-0.6.7/tests/test_deserialization.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.6/tests/test_mode_operators.py` & `meow-sim-0.6.7/tests/test_mode_operators.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.6/tests/test_nbs.py` & `meow-sim-0.6.7/tests/test_nbs.py`

 * *Files identical despite different names*

