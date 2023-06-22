# Comparing `tmp/odb-plotter-0.6.0.tar.gz` & `tmp/odb-plotter-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odb-plotter-0.6.0.tar", last modified: Wed Jun 21 18:29:22 2023, max compression
+gzip compressed data, was "odb-plotter-0.6.1.tar", last modified: Thu Jun 22 16:07:13 2023, max compression
```

## Comparing `odb-plotter-0.6.0.tar` & `odb-plotter-0.6.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-21 18:29:22.109733 odb-plotter-0.6.0/
--rw-r--r--   0 clark     (1000) clark     (1000)     1074 2023-06-02 13:55:59.000000 odb-plotter-0.6.0/LICENSE
--rw-r--r--   0 clark     (1000) clark     (1000)     3667 2023-06-21 18:29:22.109733 odb-plotter-0.6.0/PKG-INFO
--rw-r--r--   0 clark     (1000) clark     (1000)     1742 2023-06-21 18:29:07.000000 odb-plotter-0.6.0/README.md
--rw-r--r--   0 clark     (1000) clark     (1000)     1221 2023-06-21 18:29:07.000000 odb-plotter-0.6.0/pyproject.toml
--rw-r--r--   0 clark     (1000) clark     (1000)       38 2023-06-21 18:29:22.109733 odb-plotter-0.6.0/setup.cfg
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-21 18:29:22.103066 odb-plotter-0.6.0/src/
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-21 18:29:22.103066 odb-plotter-0.6.0/src/odb_plotter.egg-info/
--rw-r--r--   0 clark     (1000) clark     (1000)     3667 2023-06-21 18:29:22.000000 odb-plotter-0.6.0/src/odb_plotter.egg-info/PKG-INFO
--rw-r--r--   0 clark     (1000) clark     (1000)      559 2023-06-21 18:29:22.000000 odb-plotter-0.6.0/src/odb_plotter.egg-info/SOURCES.txt
--rw-r--r--   0 clark     (1000) clark     (1000)        1 2023-06-21 18:29:22.000000 odb-plotter-0.6.0/src/odb_plotter.egg-info/dependency_links.txt
--rw-r--r--   0 clark     (1000) clark     (1000)      133 2023-06-21 18:29:22.000000 odb-plotter-0.6.0/src/odb_plotter.egg-info/requires.txt
--rw-r--r--   0 clark     (1000) clark     (1000)        5 2023-06-21 18:29:22.000000 odb-plotter-0.6.0/src/odb_plotter.egg-info/top_level.txt
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-21 18:29:22.109733 odb-plotter-0.6.0/src/odbp/
--rw-r--r--   0 clark     (1000) clark     (1000)       85 2023-06-21 18:29:07.000000 odb-plotter-0.6.0/src/odbp/__init__.py
--rw-r--r--   0 clark     (1000) clark     (1000)       59 2023-05-25 14:12:43.000000 odb-plotter-0.6.0/src/odbp/__main__.py
--rw-r--r--   0 clark     (1000) clark     (1000)    24792 2023-06-21 18:29:07.000000 odb-plotter-0.6.0/src/odbp/cli.py
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-21 18:29:22.109733 odb-plotter-0.6.0/src/odbp/data/
--rw-r--r--   0 clark     (1000) clark     (1000)     4872 2023-06-01 00:43:21.000000 odb-plotter-0.6.0/src/odbp/data/config.toml
--rw-r--r--   0 clark     (1000) clark     (1000)      456 2023-05-25 14:12:43.000000 odb-plotter-0.6.0/src/odbp/data/views.toml
--rw-r--r--   0 clark     (1000) clark     (1000)    36497 2023-06-21 18:29:07.000000 odb-plotter-0.6.0/src/odbp/odb.py
--rw-r--r--   0 clark     (1000) clark     (1000)     4851 2023-06-12 22:11:39.000000 odb-plotter-0.6.0/src/odbp/odb_visualizer.py
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-21 18:29:22.109733 odb-plotter-0.6.0/src/odbp/py2_scripts/
--rw-r--r--   0 clark     (1000) clark     (1000)     9751 2023-06-21 18:29:07.000000 odb-plotter-0.6.0/src/odbp/py2_scripts/converter.py
--rw-r--r--   0 clark     (1000) clark     (1000)     5298 2023-06-21 18:29:07.000000 odb-plotter-0.6.0/src/odbp/py2_scripts/extractor.py
--rw-r--r--   0 clark     (1000) clark     (1000)     3079 2023-06-21 18:29:07.000000 odb-plotter-0.6.0/src/odbp/py2_scripts/state_collector.py
--rw-r--r--   0 clark     (1000) clark     (1000)     2336 2023-06-21 18:29:07.000000 odb-plotter-0.6.0/src/odbp/reader.py
--rw-r--r--   0 clark     (1000) clark     (1000)    26816 2023-06-21 18:29:07.000000 odb-plotter-0.6.0/src/odbp/state.py
--rw-r--r--   0 clark     (1000) clark     (1000)     2242 2023-06-21 18:29:07.000000 odb-plotter-0.6.0/src/odbp/util.py
--rw-r--r--   0 clark     (1000) clark     (1000)     3938 2023-06-21 18:29:07.000000 odb-plotter-0.6.0/src/odbp/writer.py
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-22 16:07:13.933123 odb-plotter-0.6.1/
+-rw-r--r--   0 clark     (1000) clark     (1000)     1074 2023-06-02 13:55:59.000000 odb-plotter-0.6.1/LICENSE
+-rw-r--r--   0 clark     (1000) clark     (1000)     3859 2023-06-22 16:07:13.929790 odb-plotter-0.6.1/PKG-INFO
+-rw-r--r--   0 clark     (1000) clark     (1000)     1893 2023-06-22 16:06:55.000000 odb-plotter-0.6.1/README.md
+-rw-r--r--   0 clark     (1000) clark     (1000)     1294 2023-06-22 16:06:55.000000 odb-plotter-0.6.1/pyproject.toml
+-rw-r--r--   0 clark     (1000) clark     (1000)       38 2023-06-22 16:07:13.933123 odb-plotter-0.6.1/setup.cfg
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-22 16:07:13.926457 odb-plotter-0.6.1/src/
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-22 16:07:13.926457 odb-plotter-0.6.1/src/odb_plotter.egg-info/
+-rw-r--r--   0 clark     (1000) clark     (1000)     3859 2023-06-22 16:07:13.000000 odb-plotter-0.6.1/src/odb_plotter.egg-info/PKG-INFO
+-rw-r--r--   0 clark     (1000) clark     (1000)      559 2023-06-22 16:07:13.000000 odb-plotter-0.6.1/src/odb_plotter.egg-info/SOURCES.txt
+-rw-r--r--   0 clark     (1000) clark     (1000)        1 2023-06-22 16:07:13.000000 odb-plotter-0.6.1/src/odb_plotter.egg-info/dependency_links.txt
+-rw-r--r--   0 clark     (1000) clark     (1000)      156 2023-06-22 16:07:13.000000 odb-plotter-0.6.1/src/odb_plotter.egg-info/requires.txt
+-rw-r--r--   0 clark     (1000) clark     (1000)        5 2023-06-22 16:07:13.000000 odb-plotter-0.6.1/src/odb_plotter.egg-info/top_level.txt
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-22 16:07:13.929790 odb-plotter-0.6.1/src/odbp/
+-rw-r--r--   0 clark     (1000) clark     (1000)       85 2023-06-22 16:06:55.000000 odb-plotter-0.6.1/src/odbp/__init__.py
+-rw-r--r--   0 clark     (1000) clark     (1000)       59 2023-05-25 14:12:43.000000 odb-plotter-0.6.1/src/odbp/__main__.py
+-rw-r--r--   0 clark     (1000) clark     (1000)    24792 2023-06-21 18:29:07.000000 odb-plotter-0.6.1/src/odbp/cli.py
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-22 16:07:13.929790 odb-plotter-0.6.1/src/odbp/data/
+-rw-r--r--   0 clark     (1000) clark     (1000)     4872 2023-06-01 00:43:21.000000 odb-plotter-0.6.1/src/odbp/data/config.toml
+-rw-r--r--   0 clark     (1000) clark     (1000)      456 2023-05-25 14:12:43.000000 odb-plotter-0.6.1/src/odbp/data/views.toml
+-rw-r--r--   0 clark     (1000) clark     (1000)    36679 2023-06-22 16:06:55.000000 odb-plotter-0.6.1/src/odbp/odb.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     4851 2023-06-12 22:11:39.000000 odb-plotter-0.6.1/src/odbp/odb_visualizer.py
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-22 16:07:13.929790 odb-plotter-0.6.1/src/odbp/py2_scripts/
+-rw-r--r--   0 clark     (1000) clark     (1000)     9751 2023-06-21 18:29:07.000000 odb-plotter-0.6.1/src/odbp/py2_scripts/converter.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     5298 2023-06-21 18:29:07.000000 odb-plotter-0.6.1/src/odbp/py2_scripts/extractor.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     3079 2023-06-21 18:29:07.000000 odb-plotter-0.6.1/src/odbp/py2_scripts/state_collector.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     2336 2023-06-21 18:29:07.000000 odb-plotter-0.6.1/src/odbp/reader.py
+-rw-r--r--   0 clark     (1000) clark     (1000)    26816 2023-06-21 18:29:07.000000 odb-plotter-0.6.1/src/odbp/state.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     2242 2023-06-21 18:29:07.000000 odb-plotter-0.6.1/src/odbp/util.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     3938 2023-06-21 18:29:07.000000 odb-plotter-0.6.1/src/odbp/writer.py
```

### Comparing `odb-plotter-0.6.0/LICENSE` & `odb-plotter-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.0/PKG-INFO` & `odb-plotter-0.6.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odb-plotter
-Version: 0.6.0
+Version: 0.6.1
 Summary: Python3 API for Abaqus .odb Files and related Command Line Visualization Tool. Focused on Additive Manufacturing Thermal Transfer
 Author-email: Clark Hensley <clarkhensley@duck.com>
 Maintainer-email: Clark Hensley <clarkhensley@duck.com>
 License: MIT License
         
         Copyright (c) 2023 Matthew W. Priddy
         
@@ -27,23 +27,30 @@
         SOFTWARE.
         
 Project-URL: Homepage, https://www.cmml.me.msstate.edu
 Project-URL: Bug Reports, https://www.github.com/Computational-Mechanics-Materials-Lab/ODBPlotter/issues
 Project-URL: Source, https://www.github.com/Computational-Mechanics-Materials-Lab/ODBPlotter
 Keywords: abaqus,abq,fea,odb,waam,wa-ded,visualization
 Description-Content-Type: text/markdown
+Provides-Extra: plot
+Provides-Extra: all
 License-File: LICENSE
 
 # ODB Plotter
 
 ## Constraints:
 ODB Plotter is being developed by [CMML](https://www.cmml.me.msstate.edu), and as such has a focus on Additive Manufacturing and Temperature Data.
 
 ## Install with pip
 ```shell
+pip install odb-plotter["all"]
+```
+
+## Install in headless mode (data processing only)
+```shell
 pip install odb-plotter
 ```
 
 ## Run the cli with python
 ```shell
 python -m odbp
 ```
@@ -64,12 +71,13 @@
 * Before 0.5.0: Did not have the Changelog here.
 * 0.5.0: API Updates and better dataframe filtering
     * 0.5.1: Implement new system information (pypi tags, this changelog)
     * 0.5.2: Returning support to Python 3.8+ (type hinting)
     * 0.5.3: Patching conversion bugs
     * 0.5.4: Parametrize number of cpus for testing
 * 0.6.0: Extractor improvements, ODB interface tools (iteration, receiving ODB data), re-implementation of basic 3D plots over time (including melt-pool plots). Created two-dimensional plotting capabilities
+    * 0.6.1: Update notices if pyvista isn't installed
 * Upcoming:
     * 0.7.0: Improve user settings, parameterization, metadata. Let users select plotting colors, keep metadata of nodesets or spatial, thermal, temporal bounds within the .hdf5.
     * 0.8.0: Improve pyvista functionality: views, gifs, non-interactive image saving, leave the viewer.
     * 0.9.0: Rewrite CLI to use python's cmd module and pyreadline/GNU readline.
     * 1.0.0: Final bug-fixing, type checking, bounds checking, etc. Hopefully coinciding with (or following) a publication.
```

### Comparing `odb-plotter-0.6.0/README.md` & `odb-plotter-0.6.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 # ODB Plotter
 
 ## Constraints:
 ODB Plotter is being developed by [CMML](https://www.cmml.me.msstate.edu), and as such has a focus on Additive Manufacturing and Temperature Data.
 
 ## Install with pip
 ```shell
+pip install odb-plotter["all"]
+```
+
+## Install in headless mode (data processing only)
+```shell
 pip install odb-plotter
 ```
 
 ## Run the cli with python
 ```shell
 python -m odbp
 ```
@@ -29,12 +34,13 @@
 * Before 0.5.0: Did not have the Changelog here.
 * 0.5.0: API Updates and better dataframe filtering
     * 0.5.1: Implement new system information (pypi tags, this changelog)
     * 0.5.2: Returning support to Python 3.8+ (type hinting)
     * 0.5.3: Patching conversion bugs
     * 0.5.4: Parametrize number of cpus for testing
 * 0.6.0: Extractor improvements, ODB interface tools (iteration, receiving ODB data), re-implementation of basic 3D plots over time (including melt-pool plots). Created two-dimensional plotting capabilities
+    * 0.6.1: Update notices if pyvista isn't installed
 * Upcoming:
     * 0.7.0: Improve user settings, parameterization, metadata. Let users select plotting colors, keep metadata of nodesets or spatial, thermal, temporal bounds within the .hdf5.
     * 0.8.0: Improve pyvista functionality: views, gifs, non-interactive image saving, leave the viewer.
     * 0.9.0: Rewrite CLI to use python's cmd module and pyreadline/GNU readline.
     * 1.0.0: Final bug-fixing, type checking, bounds checking, etc. Hopefully coinciding with (or following) a publication.
```

### Comparing `odb-plotter-0.6.0/pyproject.toml` & `odb-plotter-0.6.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -9,19 +9,26 @@
 dependencies = [
 "platformdirs",
 "h5py",
 "numpy",
 "tomli>=1.1.0; python_version < '3.11'",
 "tomli_w",
 "pandas",
-"pyvista",
 "pyreadline3; platform_system == 'Windows'",
 ]
 dynamic = ["version",]
 
+[project.optional-dependencies]
+plot = [
+    'pyvista',
+]
+all = [
+    'pyvista',
+]
+
 [project.urls]
 "Homepage" = "https://www.cmml.me.msstate.edu"
 "Bug Reports" = "https://www.github.com/Computational-Mechanics-Materials-Lab/ODBPlotter/issues"
 "Source" = "https://www.github.com/Computational-Mechanics-Materials-Lab/ODBPlotter"
 
 [tool.setuptools]
 package-data = {odbp = ["data/views.toml", "data/config.toml", "py2_scripts/converter.py", "py2_scripts/extractor.py", "py2_scripts/state_collector.py",]}
```

### Comparing `odb-plotter-0.6.0/src/odb_plotter.egg-info/PKG-INFO` & `odb-plotter-0.6.1/src/odb_plotter.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odb-plotter
-Version: 0.6.0
+Version: 0.6.1
 Summary: Python3 API for Abaqus .odb Files and related Command Line Visualization Tool. Focused on Additive Manufacturing Thermal Transfer
 Author-email: Clark Hensley <clarkhensley@duck.com>
 Maintainer-email: Clark Hensley <clarkhensley@duck.com>
 License: MIT License
         
         Copyright (c) 2023 Matthew W. Priddy
         
@@ -27,23 +27,30 @@
         SOFTWARE.
         
 Project-URL: Homepage, https://www.cmml.me.msstate.edu
 Project-URL: Bug Reports, https://www.github.com/Computational-Mechanics-Materials-Lab/ODBPlotter/issues
 Project-URL: Source, https://www.github.com/Computational-Mechanics-Materials-Lab/ODBPlotter
 Keywords: abaqus,abq,fea,odb,waam,wa-ded,visualization
 Description-Content-Type: text/markdown
+Provides-Extra: plot
+Provides-Extra: all
 License-File: LICENSE
 
 # ODB Plotter
 
 ## Constraints:
 ODB Plotter is being developed by [CMML](https://www.cmml.me.msstate.edu), and as such has a focus on Additive Manufacturing and Temperature Data.
 
 ## Install with pip
 ```shell
+pip install odb-plotter["all"]
+```
+
+## Install in headless mode (data processing only)
+```shell
 pip install odb-plotter
 ```
 
 ## Run the cli with python
 ```shell
 python -m odbp
 ```
@@ -64,12 +71,13 @@
 * Before 0.5.0: Did not have the Changelog here.
 * 0.5.0: API Updates and better dataframe filtering
     * 0.5.1: Implement new system information (pypi tags, this changelog)
     * 0.5.2: Returning support to Python 3.8+ (type hinting)
     * 0.5.3: Patching conversion bugs
     * 0.5.4: Parametrize number of cpus for testing
 * 0.6.0: Extractor improvements, ODB interface tools (iteration, receiving ODB data), re-implementation of basic 3D plots over time (including melt-pool plots). Created two-dimensional plotting capabilities
+    * 0.6.1: Update notices if pyvista isn't installed
 * Upcoming:
     * 0.7.0: Improve user settings, parameterization, metadata. Let users select plotting colors, keep metadata of nodesets or spatial, thermal, temporal bounds within the .hdf5.
     * 0.8.0: Improve pyvista functionality: views, gifs, non-interactive image saving, leave the viewer.
     * 0.9.0: Rewrite CLI to use python's cmd module and pyreadline/GNU readline.
     * 1.0.0: Final bug-fixing, type checking, bounds checking, etc. Hopefully coinciding with (or following) a publication.
```

### Comparing `odb-plotter-0.6.0/src/odb_plotter.egg-info/SOURCES.txt` & `odb-plotter-0.6.1/src/odb_plotter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.0/src/odbp/cli.py` & `odb-plotter-0.6.1/src/odbp/cli.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.0/src/odbp/data/config.toml` & `odb-plotter-0.6.1/src/odbp/data/config.toml`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.0/src/odbp/odb.py` & `odb-plotter-0.6.1/src/odbp/odb.py`

 * *Files 1% similar despite different names*

```diff
@@ -1083,16 +1083,16 @@
         mean_max_both: str = "both"
         ) -> Optional[pathlib.Path]:
         # TODO What if I want to 2d-plot only 1 nodeset, but I extractor more stuff
         # or DIDN'T extract the nodeset at all. Same w/ 3D. Metadata?
 
         if not PYVISTA_AVAILABLE:
             raise Exception("Plotting cabailities are not included."
-                " Please install pyvista via pip install odb-plotter"
-                ' rather than pip install odb-plotter["headless"]'
+                ' Please install pyvista via pip install odb-plotter["plot"]'
+                ' or odb-plotter["all"] rather than pip install odb-plotter'
                 " Or export the data from Odb.extract() to another tool,"
                 " such as matplotlib or bokeh.")
 
         data_to_plot: DataFrameType = self.extract()
         time_data: List[float] = list(data_to_plot.index)
 
         title: str = self.hdf_path.stem if hasattr(self, "hdf_path") else self.odb_path.stem
@@ -1140,18 +1140,19 @@
             label: Optional[str] = None,
             target_nodes: Optional[DataFrameType] = None
             ) -> "List[pathlib.Path]":
         """
 
         """
         if not PYVISTA_AVAILABLE:
-            raise Exception("3D Plotting capabilities are not included."
-                            'Please pip install odb-plotter'
-                            'rather than odb-plotter["headless"] to use'
-                            "three-dimensional plotting")
+            raise Exception("Plotting cabailities are not included."
+                ' Please install pyvista via pip install odb-plotter["plot"]'
+                ' or odb-plotter["all"] rather than pip install odb-plotter'
+                " Or export the data from Odb.extract() to another tool,"
+                " such as matplotlib or bokeh.")
 
         label = self.hdf_path.stem if label is None else label
 
         target_nodes = self.odb if target_nodes is None else target_nodes
 
         if self.interactive:
             results: List[pathlib.Path] = list()
@@ -1185,18 +1186,19 @@
         label: str,
         target_nodes: DataFrameType,
         )-> Optional[pathlib.Path]:
         """
         """
 
         if not PYVISTA_AVAILABLE:
-            raise Exception("3D Plotting capabilities are not included."
-                            'Please pip install odb-plotter'
-                            'rather than odb-plotter["headless"] to use'
-                            "three-dimensional plotting")
+            raise Exception("Plotting cabailities are not included."
+                ' Please install pyvista via pip install odb-plotter["plot"]'
+                ' or odb-plotter["all"] rather than pip install odb-plotter'
+                " Or export the data from Odb.extract() to another tool,"
+                " such as matplotlib or bokeh.")
 
         dims_columns: set[str] = {"X", "Y", "Z"}
         combined_label: str = f"{label}-{round(time, 2):.2f}"
 
         plotter: pv.Plotter = pv.Plotter(
             off_screen=(not self._interactive),
             window_size=(1920, 1080),
```

### Comparing `odb-plotter-0.6.0/src/odbp/odb_visualizer.py` & `odb-plotter-0.6.1/src/odbp/odb_visualizer.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.0/src/odbp/py2_scripts/converter.py` & `odb-plotter-0.6.1/src/odbp/py2_scripts/converter.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.0/src/odbp/py2_scripts/extractor.py` & `odb-plotter-0.6.1/src/odbp/py2_scripts/extractor.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.0/src/odbp/py2_scripts/state_collector.py` & `odb-plotter-0.6.1/src/odbp/py2_scripts/state_collector.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.0/src/odbp/reader.py` & `odb-plotter-0.6.1/src/odbp/reader.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.0/src/odbp/state.py` & `odb-plotter-0.6.1/src/odbp/state.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.0/src/odbp/util.py` & `odb-plotter-0.6.1/src/odbp/util.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.0/src/odbp/writer.py` & `odb-plotter-0.6.1/src/odbp/writer.py`

 * *Files identical despite different names*

