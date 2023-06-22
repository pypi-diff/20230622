# Comparing `tmp/odb-plotter-0.6.1.tar.gz` & `tmp/odb-plotter-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odb-plotter-0.6.1.tar", last modified: Thu Jun 22 16:07:13 2023, max compression
+gzip compressed data, was "odb-plotter-0.6.2.tar", last modified: Thu Jun 22 18:34:47 2023, max compression
```

## Comparing `odb-plotter-0.6.1.tar` & `odb-plotter-0.6.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-22 16:07:13.933123 odb-plotter-0.6.1/
--rw-r--r--   0 clark     (1000) clark     (1000)     1074 2023-06-02 13:55:59.000000 odb-plotter-0.6.1/LICENSE
--rw-r--r--   0 clark     (1000) clark     (1000)     3859 2023-06-22 16:07:13.929790 odb-plotter-0.6.1/PKG-INFO
--rw-r--r--   0 clark     (1000) clark     (1000)     1893 2023-06-22 16:06:55.000000 odb-plotter-0.6.1/README.md
--rw-r--r--   0 clark     (1000) clark     (1000)     1294 2023-06-22 16:06:55.000000 odb-plotter-0.6.1/pyproject.toml
--rw-r--r--   0 clark     (1000) clark     (1000)       38 2023-06-22 16:07:13.933123 odb-plotter-0.6.1/setup.cfg
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-22 16:07:13.926457 odb-plotter-0.6.1/src/
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-22 16:07:13.926457 odb-plotter-0.6.1/src/odb_plotter.egg-info/
--rw-r--r--   0 clark     (1000) clark     (1000)     3859 2023-06-22 16:07:13.000000 odb-plotter-0.6.1/src/odb_plotter.egg-info/PKG-INFO
--rw-r--r--   0 clark     (1000) clark     (1000)      559 2023-06-22 16:07:13.000000 odb-plotter-0.6.1/src/odb_plotter.egg-info/SOURCES.txt
--rw-r--r--   0 clark     (1000) clark     (1000)        1 2023-06-22 16:07:13.000000 odb-plotter-0.6.1/src/odb_plotter.egg-info/dependency_links.txt
--rw-r--r--   0 clark     (1000) clark     (1000)      156 2023-06-22 16:07:13.000000 odb-plotter-0.6.1/src/odb_plotter.egg-info/requires.txt
--rw-r--r--   0 clark     (1000) clark     (1000)        5 2023-06-22 16:07:13.000000 odb-plotter-0.6.1/src/odb_plotter.egg-info/top_level.txt
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-22 16:07:13.929790 odb-plotter-0.6.1/src/odbp/
--rw-r--r--   0 clark     (1000) clark     (1000)       85 2023-06-22 16:06:55.000000 odb-plotter-0.6.1/src/odbp/__init__.py
--rw-r--r--   0 clark     (1000) clark     (1000)       59 2023-05-25 14:12:43.000000 odb-plotter-0.6.1/src/odbp/__main__.py
--rw-r--r--   0 clark     (1000) clark     (1000)    24792 2023-06-21 18:29:07.000000 odb-plotter-0.6.1/src/odbp/cli.py
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-22 16:07:13.929790 odb-plotter-0.6.1/src/odbp/data/
--rw-r--r--   0 clark     (1000) clark     (1000)     4872 2023-06-01 00:43:21.000000 odb-plotter-0.6.1/src/odbp/data/config.toml
--rw-r--r--   0 clark     (1000) clark     (1000)      456 2023-05-25 14:12:43.000000 odb-plotter-0.6.1/src/odbp/data/views.toml
--rw-r--r--   0 clark     (1000) clark     (1000)    36679 2023-06-22 16:06:55.000000 odb-plotter-0.6.1/src/odbp/odb.py
--rw-r--r--   0 clark     (1000) clark     (1000)     4851 2023-06-12 22:11:39.000000 odb-plotter-0.6.1/src/odbp/odb_visualizer.py
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-22 16:07:13.929790 odb-plotter-0.6.1/src/odbp/py2_scripts/
--rw-r--r--   0 clark     (1000) clark     (1000)     9751 2023-06-21 18:29:07.000000 odb-plotter-0.6.1/src/odbp/py2_scripts/converter.py
--rw-r--r--   0 clark     (1000) clark     (1000)     5298 2023-06-21 18:29:07.000000 odb-plotter-0.6.1/src/odbp/py2_scripts/extractor.py
--rw-r--r--   0 clark     (1000) clark     (1000)     3079 2023-06-21 18:29:07.000000 odb-plotter-0.6.1/src/odbp/py2_scripts/state_collector.py
--rw-r--r--   0 clark     (1000) clark     (1000)     2336 2023-06-21 18:29:07.000000 odb-plotter-0.6.1/src/odbp/reader.py
--rw-r--r--   0 clark     (1000) clark     (1000)    26816 2023-06-21 18:29:07.000000 odb-plotter-0.6.1/src/odbp/state.py
--rw-r--r--   0 clark     (1000) clark     (1000)     2242 2023-06-21 18:29:07.000000 odb-plotter-0.6.1/src/odbp/util.py
--rw-r--r--   0 clark     (1000) clark     (1000)     3938 2023-06-21 18:29:07.000000 odb-plotter-0.6.1/src/odbp/writer.py
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-22 18:34:47.514384 odb-plotter-0.6.2/
+-rw-r--r--   0 clark     (1000) clark     (1000)     1074 2023-06-02 13:55:59.000000 odb-plotter-0.6.2/LICENSE
+-rw-r--r--   0 clark     (1000) clark     (1000)     3949 2023-06-22 18:34:47.514384 odb-plotter-0.6.2/PKG-INFO
+-rw-r--r--   0 clark     (1000) clark     (1000)     1983 2023-06-22 18:34:28.000000 odb-plotter-0.6.2/README.md
+-rw-r--r--   0 clark     (1000) clark     (1000)     1294 2023-06-22 16:06:55.000000 odb-plotter-0.6.2/pyproject.toml
+-rw-r--r--   0 clark     (1000) clark     (1000)       38 2023-06-22 18:34:47.514384 odb-plotter-0.6.2/setup.cfg
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-22 18:34:47.511051 odb-plotter-0.6.2/src/
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-22 18:34:47.511051 odb-plotter-0.6.2/src/odb_plotter.egg-info/
+-rw-r--r--   0 clark     (1000) clark     (1000)     3949 2023-06-22 18:34:47.000000 odb-plotter-0.6.2/src/odb_plotter.egg-info/PKG-INFO
+-rw-r--r--   0 clark     (1000) clark     (1000)      559 2023-06-22 18:34:47.000000 odb-plotter-0.6.2/src/odb_plotter.egg-info/SOURCES.txt
+-rw-r--r--   0 clark     (1000) clark     (1000)        1 2023-06-22 18:34:47.000000 odb-plotter-0.6.2/src/odb_plotter.egg-info/dependency_links.txt
+-rw-r--r--   0 clark     (1000) clark     (1000)      156 2023-06-22 18:34:47.000000 odb-plotter-0.6.2/src/odb_plotter.egg-info/requires.txt
+-rw-r--r--   0 clark     (1000) clark     (1000)        5 2023-06-22 18:34:47.000000 odb-plotter-0.6.2/src/odb_plotter.egg-info/top_level.txt
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-22 18:34:47.514384 odb-plotter-0.6.2/src/odbp/
+-rw-r--r--   0 clark     (1000) clark     (1000)       85 2023-06-22 18:34:28.000000 odb-plotter-0.6.2/src/odbp/__init__.py
+-rw-r--r--   0 clark     (1000) clark     (1000)       59 2023-05-25 14:12:43.000000 odb-plotter-0.6.2/src/odbp/__main__.py
+-rw-r--r--   0 clark     (1000) clark     (1000)    24792 2023-06-21 18:29:07.000000 odb-plotter-0.6.2/src/odbp/cli.py
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-22 18:34:47.514384 odb-plotter-0.6.2/src/odbp/data/
+-rw-r--r--   0 clark     (1000) clark     (1000)     4872 2023-06-01 00:43:21.000000 odb-plotter-0.6.2/src/odbp/data/config.toml
+-rw-r--r--   0 clark     (1000) clark     (1000)      456 2023-05-25 14:12:43.000000 odb-plotter-0.6.2/src/odbp/data/views.toml
+-rw-r--r--   0 clark     (1000) clark     (1000)    36534 2023-06-22 18:34:28.000000 odb-plotter-0.6.2/src/odbp/odb.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     4851 2023-06-12 22:11:39.000000 odb-plotter-0.6.2/src/odbp/odb_visualizer.py
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-22 18:34:47.514384 odb-plotter-0.6.2/src/odbp/py2_scripts/
+-rw-r--r--   0 clark     (1000) clark     (1000)     9751 2023-06-21 18:29:07.000000 odb-plotter-0.6.2/src/odbp/py2_scripts/converter.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     5298 2023-06-21 18:29:07.000000 odb-plotter-0.6.2/src/odbp/py2_scripts/extractor.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     3079 2023-06-21 18:29:07.000000 odb-plotter-0.6.2/src/odbp/py2_scripts/state_collector.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     2336 2023-06-21 18:29:07.000000 odb-plotter-0.6.2/src/odbp/reader.py
+-rw-r--r--   0 clark     (1000) clark     (1000)    26816 2023-06-21 18:29:07.000000 odb-plotter-0.6.2/src/odbp/state.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     2242 2023-06-21 18:29:07.000000 odb-plotter-0.6.2/src/odbp/util.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     3938 2023-06-21 18:29:07.000000 odb-plotter-0.6.2/src/odbp/writer.py
```

### Comparing `odb-plotter-0.6.1/LICENSE` & `odb-plotter-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.1/PKG-INFO` & `odb-plotter-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odb-plotter
-Version: 0.6.1
+Version: 0.6.2
 Summary: Python3 API for Abaqus .odb Files and related Command Line Visualization Tool. Focused on Additive Manufacturing Thermal Transfer
 Author-email: Clark Hensley <clarkhensley@duck.com>
 Maintainer-email: Clark Hensley <clarkhensley@duck.com>
 License: MIT License
         
         Copyright (c) 2023 Matthew W. Priddy
         
@@ -72,12 +72,13 @@
 * 0.5.0: API Updates and better dataframe filtering
     * 0.5.1: Implement new system information (pypi tags, this changelog)
     * 0.5.2: Returning support to Python 3.8+ (type hinting)
     * 0.5.3: Patching conversion bugs
     * 0.5.4: Parametrize number of cpus for testing
 * 0.6.0: Extractor improvements, ODB interface tools (iteration, receiving ODB data), re-implementation of basic 3D plots over time (including melt-pool plots). Created two-dimensional plotting capabilities
     * 0.6.1: Update notices if pyvista isn't installed
+    * 0.6.2: Improve data extraction for plotting. Ensure that plotting doesn't fork-bomb
 * Upcoming:
     * 0.7.0: Improve user settings, parameterization, metadata. Let users select plotting colors, keep metadata of nodesets or spatial, thermal, temporal bounds within the .hdf5.
     * 0.8.0: Improve pyvista functionality: views, gifs, non-interactive image saving, leave the viewer.
     * 0.9.0: Rewrite CLI to use python's cmd module and pyreadline/GNU readline.
     * 1.0.0: Final bug-fixing, type checking, bounds checking, etc. Hopefully coinciding with (or following) a publication.
```

### Comparing `odb-plotter-0.6.1/README.md` & `odb-plotter-0.6.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -35,12 +35,13 @@
 * 0.5.0: API Updates and better dataframe filtering
     * 0.5.1: Implement new system information (pypi tags, this changelog)
     * 0.5.2: Returning support to Python 3.8+ (type hinting)
     * 0.5.3: Patching conversion bugs
     * 0.5.4: Parametrize number of cpus for testing
 * 0.6.0: Extractor improvements, ODB interface tools (iteration, receiving ODB data), re-implementation of basic 3D plots over time (including melt-pool plots). Created two-dimensional plotting capabilities
     * 0.6.1: Update notices if pyvista isn't installed
+    * 0.6.2: Improve data extraction for plotting. Ensure that plotting doesn't fork-bomb
 * Upcoming:
     * 0.7.0: Improve user settings, parameterization, metadata. Let users select plotting colors, keep metadata of nodesets or spatial, thermal, temporal bounds within the .hdf5.
     * 0.8.0: Improve pyvista functionality: views, gifs, non-interactive image saving, leave the viewer.
     * 0.9.0: Rewrite CLI to use python's cmd module and pyreadline/GNU readline.
     * 1.0.0: Final bug-fixing, type checking, bounds checking, etc. Hopefully coinciding with (or following) a publication.
```

### Comparing `odb-plotter-0.6.1/pyproject.toml` & `odb-plotter-0.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.1/src/odb_plotter.egg-info/PKG-INFO` & `odb-plotter-0.6.2/src/odb_plotter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odb-plotter
-Version: 0.6.1
+Version: 0.6.2
 Summary: Python3 API for Abaqus .odb Files and related Command Line Visualization Tool. Focused on Additive Manufacturing Thermal Transfer
 Author-email: Clark Hensley <clarkhensley@duck.com>
 Maintainer-email: Clark Hensley <clarkhensley@duck.com>
 License: MIT License
         
         Copyright (c) 2023 Matthew W. Priddy
         
@@ -72,12 +72,13 @@
 * 0.5.0: API Updates and better dataframe filtering
     * 0.5.1: Implement new system information (pypi tags, this changelog)
     * 0.5.2: Returning support to Python 3.8+ (type hinting)
     * 0.5.3: Patching conversion bugs
     * 0.5.4: Parametrize number of cpus for testing
 * 0.6.0: Extractor improvements, ODB interface tools (iteration, receiving ODB data), re-implementation of basic 3D plots over time (including melt-pool plots). Created two-dimensional plotting capabilities
     * 0.6.1: Update notices if pyvista isn't installed
+    * 0.6.2: Improve data extraction for plotting. Ensure that plotting doesn't fork-bomb
 * Upcoming:
     * 0.7.0: Improve user settings, parameterization, metadata. Let users select plotting colors, keep metadata of nodesets or spatial, thermal, temporal bounds within the .hdf5.
     * 0.8.0: Improve pyvista functionality: views, gifs, non-interactive image saving, leave the viewer.
     * 0.9.0: Rewrite CLI to use python's cmd module and pyreadline/GNU readline.
     * 1.0.0: Final bug-fixing, type checking, bounds checking, etc. Hopefully coinciding with (or following) a publication.
```

### Comparing `odb-plotter-0.6.1/src/odb_plotter.egg-info/SOURCES.txt` & `odb-plotter-0.6.2/src/odb_plotter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.1/src/odbp/cli.py` & `odb-plotter-0.6.2/src/odbp/cli.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.1/src/odbp/data/config.toml` & `odb-plotter-0.6.2/src/odbp/data/config.toml`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.1/src/odbp/odb.py` & `odb-plotter-0.6.2/src/odbp/odb.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,15 @@
         "_frame_range",
         "_step_names",
         "_frame_ranges_per_step",
         "_nodeset_names",
         "_part_names",
         "_node_range",
         "_node_ranges_per_part",
+        "_extracted_nodes",
 
         # User-defined components
         # TODO turn these into a subclass member, overload
         # __getattr__/__setattr__ on this object
         "_x_low",
         "_x_high",
         "_y_low",
@@ -211,14 +212,16 @@
         self._cpus = multiprocessing.cpu_count()
 
         self._interactive: bool = False
         self._colormap: str = "turbo"
         self._save_format: str = ".png"
         self._save: bool = True
 
+        self._extracted_nodes: DataFrameType
+
         # TODO
         self._angle = Union[str, Tuple[float, float, float]]
 
         self._iterator_ind: int = 0
         self._times: NDArrayType
 
 
@@ -876,17 +879,23 @@
         elif cls.ensure_magic(path, ODB_MAGIC_NUM):
             # extract from .odb
             return cls.extract_from_odb(path)
 
 
     def extract(self) -> DataFrameType:
         if hasattr(self, "hdf_path") or hasattr(self, "odb"):
-            return self.extract_from_hdf()
+            result: DataFrameType = self.extract_from_hdf()
+            self._extracted_nodes = result
+            return result
+
         elif hasattr(self, "odb_path"):
-            return self.extract_from_odb()
+            result: DataFrameType = self.extract_from_odb()
+            self._extracted_nodes = result
+            return result
+
         else:
             raise AttributeError("This Odb object does not have")
 
 
     def extract_from_odb(
         self,
         target_file: Optional[pathlib.Path] = None
@@ -1088,34 +1097,36 @@
         if not PYVISTA_AVAILABLE:
             raise Exception("Plotting cabailities are not included."
                 ' Please install pyvista via pip install odb-plotter["plot"]'
                 ' or odb-plotter["all"] rather than pip install odb-plotter'
                 " Or export the data from Odb.extract() to another tool,"
                 " such as matplotlib or bokeh.")
 
-        data_to_plot: DataFrameType = self.extract()
-        time_data: List[float] = list(data_to_plot.index)
+        if not hasattr(self, "_extracted_nodes"):
+            _ = self.extract()
+
+        time_data: List[float] = list(self._extracted_nodes.index)
 
         title: str = self.hdf_path.stem if hasattr(self, "hdf_path") else self.odb_path.stem
         title += " Temperature versus Time"
 
         temp_v_time: pv.Chart2D = pv.Chart2D(x_label="Time (seconds)", y_label="Temperature (Kelvin)")
         temp_v_time.title = title
 
         if mean_max_both.lower() in ("mean", "both"):
             temp_v_time.line(
                 time_data,
-                data_to_plot["mean"].values,
+                self._extracted_nodes["mean"].values,
                 color="#FF7F00",
                 label="Mean Temperature")
 
         if mean_max_both.lower() in ("max", "both"):
             temp_v_time.line(
                 time_data,
-                data_to_plot["max"].values,
+                self._extracted_nodes["max"].values,
                 color="#FF0000",
                 label="Mean Temperature")
 
         if self.save:
             save_path: pathlib.Path = self.result_dir / f"{title}.png"
             # Returns a numpy array of pixels
             # But we don't need that.
@@ -1133,14 +1144,15 @@
                 off_screen=False,
                 screenshot=False)
 
 
     # 3D Plotting
     def plot_3d_all_times(
             self,
+            *,
             label: Optional[str] = None,
             target_nodes: Optional[DataFrameType] = None
             ) -> "List[pathlib.Path]":
         """
 
         """
         if not PYVISTA_AVAILABLE:
@@ -1148,38 +1160,25 @@
                 ' Please install pyvista via pip install odb-plotter["plot"]'
                 ' or odb-plotter["all"] rather than pip install odb-plotter'
                 " Or export the data from Odb.extract() to another tool,"
                 " such as matplotlib or bokeh.")
 
         label = self.hdf_path.stem if label is None else label
 
-        target_nodes = self.odb if target_nodes is None else target_nodes
-
-        if self.interactive:
-            results: List[pathlib.Path] = list()
-            frame: DataFrameType
-            for frame in self:
-                time: float = frame["Time"].values[0]
-                results.append(self._plot_3d_single(time, label, target_nodes))
+        if target_nodes is None:
+            if not hasattr(self, "odb"):
+                self.load_hdf()
 
-        else:
-            # TODO dataclass
-            single_plot_args: List[Tuple[float, str, str]] = [
-                (frame["Time"].values[0],
-                label,
-                target_nodes,
-                ) for frame in self
-            ]
+            target_nodes = self.odb
 
-            pool: MultiprocessingPoolType
-            with multiprocessing.Pool(processes=self.cpus) as pool:
-                results: List[pathlib.Path] = pool.starmap(
-                    self._plot_3d_single,
-                    single_plot_args,
-                    )
+        results: List[pathlib.Path] = list()
+        frame: DataFrameType
+        for frame in self:
+            time: float = frame["Time"].values[0]
+            results.append(self._plot_3d_single(time, label, target_nodes))
 
         return results
 
 
     def _plot_3d_single(
         self,
         time: float,
@@ -1196,15 +1195,16 @@
                 " Or export the data from Odb.extract() to another tool,"
                 " such as matplotlib or bokeh.")
 
         dims_columns: set[str] = {"X", "Y", "Z"}
         combined_label: str = f"{label}-{round(time, 2):.2f}"
 
         plotter: pv.Plotter = pv.Plotter(
-            off_screen=(not self._interactive),
+            interactive=self.interactive,
+            off_screen=(not self.interactive),
             window_size=(1920, 1080),
             lighting="three lights"
             )
 
         plotter.add_text(
             combined_label,
             position="upper_edge",
```

### Comparing `odb-plotter-0.6.1/src/odbp/odb_visualizer.py` & `odb-plotter-0.6.2/src/odbp/odb_visualizer.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.1/src/odbp/py2_scripts/converter.py` & `odb-plotter-0.6.2/src/odbp/py2_scripts/converter.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.1/src/odbp/py2_scripts/extractor.py` & `odb-plotter-0.6.2/src/odbp/py2_scripts/extractor.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.1/src/odbp/py2_scripts/state_collector.py` & `odb-plotter-0.6.2/src/odbp/py2_scripts/state_collector.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.1/src/odbp/reader.py` & `odb-plotter-0.6.2/src/odbp/reader.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.1/src/odbp/state.py` & `odb-plotter-0.6.2/src/odbp/state.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.1/src/odbp/util.py` & `odb-plotter-0.6.2/src/odbp/util.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.1/src/odbp/writer.py` & `odb-plotter-0.6.2/src/odbp/writer.py`

 * *Files identical despite different names*

