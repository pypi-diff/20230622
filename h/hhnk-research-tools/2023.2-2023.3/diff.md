# Comparing `tmp/hhnk_research_tools-2023.2.tar.gz` & `tmp/hhnk_research_tools-2023.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hhnk_research_tools-2023.2.tar", last modified: Wed May 10 15:40:53 2023, max compression
+gzip compressed data, was "hhnk_research_tools-2023.3.tar", last modified: Thu Jun 22 10:18:28 2023, max compression
```

## Comparing `hhnk_research_tools-2023.2.tar` & `hhnk_research_tools-2023.3.tar`

### file list

```diff
@@ -1,40 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 15:40:52.825994 hhnk_research_tools-2023.2/
--rw-rw-rw-   0        0        0      605 2023-05-10 15:40:53.494100 hhnk_research_tools-2023.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-10 15:40:52.913995 hhnk_research_tools-2023.2/hhnk_research_tools/
--rw-rw-rw-   0        0        0     1825 2023-05-10 15:38:56.000000 hhnk_research_tools-2023.2/hhnk_research_tools/__init__.py
--rw-rw-rw-   0        0        0     5861 2023-05-10 15:38:56.000000 hhnk_research_tools-2023.2/hhnk_research_tools/dataframe_functions.py
-drwxrwxrwx   0        0        0        0 2023-05-10 15:40:53.143999 hhnk_research_tools-2023.2/hhnk_research_tools/folder_file_classes/
--rw-rw-rw-   0        0        0        0 2023-05-10 15:38:56.000000 hhnk_research_tools-2023.2/hhnk_research_tools/folder_file_classes/__init__.py
--rw-rw-rw-   0        0        0     1661 2023-05-10 15:38:56.000000 hhnk_research_tools-2023.2/hhnk_research_tools/folder_file_classes/file_class.py
--rw-rw-rw-   0        0        0     6811 2023-05-10 15:38:56.000000 hhnk_research_tools-2023.2/hhnk_research_tools/folder_file_classes/folder_file_classes.py
--rw-rw-rw-   0        0        0     6168 2023-05-10 15:38:56.000000 hhnk_research_tools-2023.2/hhnk_research_tools/folder_file_classes/sqlite_class.py
--rw-rw-rw-   0        0        0     6527 2023-05-10 15:38:56.000000 hhnk_research_tools-2023.2/hhnk_research_tools/folder_file_classes/threedi_schematisation.py
--rw-rw-rw-   0        0        0     2372 2023-05-10 15:38:56.000000 hhnk_research_tools-2023.2/hhnk_research_tools/general_functions.py
-drwxrwxrwx   0        0        0        0 2023-05-10 15:40:53.229000 hhnk_research_tools-2023.2/hhnk_research_tools/gis/
--rw-rw-rw-   0        0        0     1092 2021-10-25 11:51:58.000000 hhnk_research_tools-2023.2/hhnk_research_tools/gis/__init__.py
--rw-rw-rw-   0        0        0    18341 2023-05-10 15:38:56.000000 hhnk_research_tools-2023.2/hhnk_research_tools/gis/raster.py
--rw-rw-rw-   0        0        0     1427 2022-05-04 07:44:27.000000 hhnk_research_tools-2023.2/hhnk_research_tools/gis/vector.py
--rw-rw-rw-   0        0        0     2097 2023-05-10 15:38:56.000000 hhnk_research_tools-2023.2/hhnk_research_tools/processes.py
--rw-rw-rw-   0        0        0    18110 2023-05-10 15:38:56.000000 hhnk_research_tools-2023.2/hhnk_research_tools/raster_functions.py
--rw-rw-rw-   0        0        0    11573 2023-05-10 15:38:56.000000 hhnk_research_tools-2023.2/hhnk_research_tools/sql_functions.py
-drwxrwxrwx   0        0        0        0 2023-05-10 15:40:53.354002 hhnk_research_tools-2023.2/hhnk_research_tools/threedi/
--rw-rw-rw-   0        0        0      149 2022-07-04 12:41:36.000000 hhnk_research_tools-2023.2/hhnk_research_tools/threedi/__init__.py
--rw-rw-rw-   0        0        0     3603 2021-10-25 11:51:58.000000 hhnk_research_tools-2023.2/hhnk_research_tools/threedi/construct_rain_scenario.py
--rw-rw-rw-   0        0        0     2260 2022-08-17 15:04:24.000000 hhnk_research_tools-2023.2/hhnk_research_tools/threedi/construct_rain_scenario_dataframe.py
--rw-rw-rw-   0        0        0     1997 2023-05-10 15:38:56.000000 hhnk_research_tools-2023.2/hhnk_research_tools/threedi/geometry_functions.py
--rw-rw-rw-   0        0        0    12463 2022-07-04 14:10:34.000000 hhnk_research_tools-2023.2/hhnk_research_tools/threedi/grid.py
--rw-rw-rw-   0        0        0     1722 2022-05-04 07:44:27.000000 hhnk_research_tools-2023.2/hhnk_research_tools/threedi/gridedit.py
-drwxrwxrwx   0        0        0        0 2023-05-10 15:40:53.466004 hhnk_research_tools-2023.2/hhnk_research_tools/threedi/variables/
--rw-rw-rw-   0        0        0        0 2021-10-25 11:51:58.000000 hhnk_research_tools-2023.2/hhnk_research_tools/threedi/variables/__init__.py
--rw-rw-rw-   0        0        0       66 2021-10-25 11:51:58.000000 hhnk_research_tools-2023.2/hhnk_research_tools/threedi/variables/gridadmin.py
--rw-rw-rw-   0        0        0      182 2021-10-25 11:51:58.000000 hhnk_research_tools-2023.2/hhnk_research_tools/threedi/variables/rain_dataframe.py
--rw-rw-rw-   0        0        0       33 2021-10-25 11:51:58.000000 hhnk_research_tools-2023.2/hhnk_research_tools/threedi/variables/results_mapping.py
--rw-rw-rw-   0        0        0      415 2021-10-25 11:51:58.000000 hhnk_research_tools-2023.2/hhnk_research_tools/threedi/variables/variables_container.py
--rw-rw-rw-   0        0        0     1870 2021-10-25 11:51:58.000000 hhnk_research_tools-2023.2/hhnk_research_tools/variables.py
-drwxrwxrwx   0        0        0        0 2023-05-10 15:40:53.004997 hhnk_research_tools-2023.2/hhnk_research_tools.egg-info/
--rw-rw-rw-   0        0        0      605 2023-05-10 15:40:52.000000 hhnk_research_tools-2023.2/hhnk_research_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1395 2023-05-10 15:40:52.000000 hhnk_research_tools-2023.2/hhnk_research_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 15:40:52.000000 hhnk_research_tools-2023.2/hhnk_research_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-05-10 15:40:52.000000 hhnk_research_tools-2023.2/hhnk_research_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 15:40:53.508393 hhnk_research_tools-2023.2/setup.cfg
--rw-rw-rw-   0        0        0     1755 2023-05-10 15:38:56.000000 hhnk_research_tools-2023.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 10:18:27.187326 hhnk_research_tools-2023.3/
+-rw-rw-rw-   0        0        0      596 2023-06-22 10:18:28.756280 hhnk_research_tools-2023.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-22 10:18:27.447330 hhnk_research_tools-2023.3/hhnk_research_tools/
+-rw-rw-rw-   0        0        0     2108 2023-06-21 07:36:30.000000 hhnk_research_tools-2023.3/hhnk_research_tools/__init__.py
+-rw-rw-rw-   0        0        0     5861 2023-05-10 15:38:56.000000 hhnk_research_tools-2023.3/hhnk_research_tools/dataframe_functions.py
+drwxrwxrwx   0        0        0        0 2023-06-22 10:18:27.747334 hhnk_research_tools-2023.3/hhnk_research_tools/folder_file_classes/
+-rw-rw-rw-   0        0        0        0 2023-05-10 15:38:56.000000 hhnk_research_tools-2023.3/hhnk_research_tools/folder_file_classes/__init__.py
+-rw-rw-rw-   0        0        0     1561 2023-06-16 13:27:17.000000 hhnk_research_tools-2023.3/hhnk_research_tools/folder_file_classes/file_class.py
+-rw-rw-rw-   0        0        0     7014 2023-06-22 10:06:15.000000 hhnk_research_tools-2023.3/hhnk_research_tools/folder_file_classes/folder_file_classes.py
+-rw-rw-rw-   0        0        0     6168 2023-05-10 15:38:56.000000 hhnk_research_tools-2023.3/hhnk_research_tools/folder_file_classes/sqlite_class.py
+-rw-rw-rw-   0        0        0     6732 2023-06-16 13:18:13.000000 hhnk_research_tools-2023.3/hhnk_research_tools/folder_file_classes/threedi_schematisation.py
+-rw-rw-rw-   0        0        0     3570 2023-06-16 11:21:37.000000 hhnk_research_tools-2023.3/hhnk_research_tools/general_functions.py
+drwxrwxrwx   0        0        0        0 2023-06-22 10:18:27.821335 hhnk_research_tools-2023.3/hhnk_research_tools/gis/
+-rw-rw-rw-   0        0        0     1092 2021-10-25 11:51:58.000000 hhnk_research_tools-2023.3/hhnk_research_tools/gis/__init__.py
+-rw-rw-rw-   0        0        0    18597 2023-06-16 09:23:36.000000 hhnk_research_tools-2023.3/hhnk_research_tools/gis/raster.py
+-rw-rw-rw-   0        0        0     1427 2022-05-04 07:44:27.000000 hhnk_research_tools-2023.3/hhnk_research_tools/gis/vector.py
+-rw-rw-rw-   0        0        0     2097 2023-05-10 15:38:56.000000 hhnk_research_tools-2023.3/hhnk_research_tools/processes.py
+-rw-rw-rw-   0        0        0    18373 2023-06-16 09:23:36.000000 hhnk_research_tools-2023.3/hhnk_research_tools/raster_functions.py
+-rw-rw-rw-   0        0        0    11573 2023-05-10 15:38:56.000000 hhnk_research_tools-2023.3/hhnk_research_tools/sql_functions.py
+drwxrwxrwx   0        0        0        0 2023-06-22 10:18:28.077339 hhnk_research_tools-2023.3/hhnk_research_tools/threedi/
+-rw-rw-rw-   0        0        0      149 2022-07-04 12:41:36.000000 hhnk_research_tools-2023.3/hhnk_research_tools/threedi/__init__.py
+-rw-rw-rw-   0        0        0     3603 2021-10-25 11:51:58.000000 hhnk_research_tools-2023.3/hhnk_research_tools/threedi/construct_rain_scenario.py
+-rw-rw-rw-   0        0        0     2260 2022-08-17 15:04:24.000000 hhnk_research_tools-2023.3/hhnk_research_tools/threedi/construct_rain_scenario_dataframe.py
+-rw-rw-rw-   0        0        0     1997 2023-05-10 15:38:56.000000 hhnk_research_tools-2023.3/hhnk_research_tools/threedi/geometry_functions.py
+-rw-rw-rw-   0        0        0    12463 2022-07-04 14:10:34.000000 hhnk_research_tools-2023.3/hhnk_research_tools/threedi/grid.py
+-rw-rw-rw-   0        0        0     1722 2022-05-04 07:44:27.000000 hhnk_research_tools-2023.3/hhnk_research_tools/threedi/gridedit.py
+-rw-rw-rw-   0        0        0      343 2023-06-16 09:23:36.000000 hhnk_research_tools-2023.3/hhnk_research_tools/threedi/read_api_file.py
+drwxrwxrwx   0        0        0        0 2023-06-22 10:18:28.465345 hhnk_research_tools-2023.3/hhnk_research_tools/threedi/variables/
+-rw-rw-rw-   0        0        0        0 2021-10-25 11:51:58.000000 hhnk_research_tools-2023.3/hhnk_research_tools/threedi/variables/__init__.py
+-rw-rw-rw-   0        0        0       66 2021-10-25 11:51:58.000000 hhnk_research_tools-2023.3/hhnk_research_tools/threedi/variables/gridadmin.py
+-rw-rw-rw-   0        0        0      182 2021-10-25 11:51:58.000000 hhnk_research_tools-2023.3/hhnk_research_tools/threedi/variables/rain_dataframe.py
+-rw-rw-rw-   0        0        0       33 2021-10-25 11:51:58.000000 hhnk_research_tools-2023.3/hhnk_research_tools/threedi/variables/results_mapping.py
+-rw-rw-rw-   0        0        0      415 2021-10-25 11:51:58.000000 hhnk_research_tools-2023.3/hhnk_research_tools/threedi/variables/variables_container.py
+-rw-rw-rw-   0        0        0     1870 2021-10-25 11:51:58.000000 hhnk_research_tools-2023.3/hhnk_research_tools/variables.py
+drwxrwxrwx   0        0        0        0 2023-06-22 10:18:27.169325 hhnk_research_tools-2023.3/hhnk_research_tools/waterschadeschatter/
+-rw-rw-rw-   0        0        0       80 2023-06-16 11:35:08.000000 hhnk_research_tools-2023.3/hhnk_research_tools/waterschadeschatter/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 10:18:28.706349 hhnk_research_tools-2023.3/hhnk_research_tools/waterschadeschatter/resources/
+-rw-rw-rw-   0        0        0        0 2023-06-16 09:23:36.000000 hhnk_research_tools-2023.3/hhnk_research_tools/waterschadeschatter/resources/__init__.py
+-rw-rw-rw-   0        0        0    70142 2023-06-16 09:23:36.000000 hhnk_research_tools-2023.3/hhnk_research_tools/waterschadeschatter/resources/cfg_hhnk_2020.cfg
+-rw-rw-rw-   0        0        0    64399 2023-06-16 09:23:36.000000 hhnk_research_tools-2023.3/hhnk_research_tools/waterschadeschatter/resources/cfg_lizard.cfg
+-rw-rw-rw-   0        0        0    64209 2023-06-16 09:23:36.000000 hhnk_research_tools-2023.3/hhnk_research_tools/waterschadeschatter/resources/cfg_lizard_servicedesk.cfg
+-rw-rw-rw-   0        0        0    69232 2023-06-16 09:23:36.000000 hhnk_research_tools-2023.3/hhnk_research_tools/waterschadeschatter/resources/cfg_stowa_standaard.cfg
+-rw-rw-rw-   0        0        0     5000 2023-06-16 09:23:36.000000 hhnk_research_tools-2023.3/hhnk_research_tools/waterschadeschatter/wss_calculations.py
+-rw-rw-rw-   0        0        0     4088 2023-06-16 09:23:36.000000 hhnk_research_tools-2023.3/hhnk_research_tools/waterschadeschatter/wss_loading.py
+-rw-rw-rw-   0        0        0     7076 2023-06-16 09:23:36.000000 hhnk_research_tools-2023.3/hhnk_research_tools/waterschadeschatter/wss_main.py
+drwxrwxrwx   0        0        0        0 2023-06-22 10:18:27.576332 hhnk_research_tools-2023.3/hhnk_research_tools.egg-info/
+-rw-rw-rw-   0        0        0      596 2023-06-22 10:18:25.000000 hhnk_research_tools-2023.3/hhnk_research_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2005 2023-06-22 10:18:26.000000 hhnk_research_tools-2023.3/hhnk_research_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 10:18:25.000000 hhnk_research_tools-2023.3/hhnk_research_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-06-22 10:18:25.000000 hhnk_research_tools-2023.3/hhnk_research_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-22 10:18:28.769755 hhnk_research_tools-2023.3/setup.cfg
+-rw-rw-rw-   0        0        0     1902 2023-06-22 10:16:00.000000 hhnk_research_tools-2023.3/setup.py
```

### Comparing `hhnk_research_tools-2023.2/PKG-INFO` & `hhnk_research_tools-2023.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: hhnk_research_tools
-Version: 2023.2
+Version: 2023.3
 Summary: General tools for analysis, data manipulation and threedi interaction for analysis of water systems
 Home-page: https://github.com/HHNK/hhnk-research-tools
 Author: Wietse van Gerwen
 Author-email: w.vangerwen@hhnk.nl
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/HHNK/hhnk-research-tools/issues
-Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
+
+UNKNOWN
+
```

### Comparing `hhnk_research_tools-2023.2/hhnk_research_tools/__init__.py` & `hhnk_research_tools-2023.3/hhnk_research_tools/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 import hhnk_research_tools.variables as variables
 
 from hhnk_research_tools.folder_file_classes.file_class import File
 
-
 from hhnk_research_tools.gis.raster import Raster, RasterMetadata
 
 import hhnk_research_tools.threedi as threedi
 
+from hhnk_research_tools.threedi.read_api_file import (
+    read_api_file
+) 
+
+from hhnk_research_tools.waterschadeschatter.wss_main import Waterschadeschatter
+
+import hhnk_research_tools.waterschadeschatter.resources
 
 from hhnk_research_tools.sql_functions import (
     sql_create_update_case_statement,
     sql_construct_select_query,
     create_sqlite_connection,
     sql_table_exists,
     execute_sql_selection,
@@ -27,14 +33,17 @@
     gdf_write_to_csv,
 )
 
 from hhnk_research_tools.general_functions import (
     ensure_file_path,
     convert_gdb_to_gpkg,
     check_create_new_file,
+    load_source,
+    get_uuid,
+    get_pkg_resource_path,
 )
 
 from hhnk_research_tools.raster_functions import (
     load_gdal_raster,
     gdf_to_raster,
     create_new_raster_file,
     save_raster_array_to_tiff,
@@ -60,12 +69,12 @@
     ThreediResult,
     RevisionsDir,
 )
 
 # TODO how does this versioning work?
 # Threedigrid version number is automatic updated with zest.releaser. Geopandas uses versioneer.py.
 # the version number in setup.py is updated using the find_version()
-__version__ = '2023.2'
+__version__ = '2023.3'
 
 __doc__ = """
 General toolbox for loading, converting and saving serval datatypes.
 """
```

### Comparing `hhnk_research_tools-2023.2/hhnk_research_tools/dataframe_functions.py` & `hhnk_research_tools-2023.3/hhnk_research_tools/dataframe_functions.py`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-2023.2/hhnk_research_tools/folder_file_classes/file_class.py` & `hhnk_research_tools-2023.3/hhnk_research_tools/folder_file_classes/file_class.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,20 +43,18 @@
         if self.exists:
             self.pl.unlink(missing_ok=False)
 
     def __str__(self):
         return self.base
 
     def __repr__(self):
-        if self.exists:
-            exists = "exists"
-        else:
-            exists = "doesn't exist"
         funcs = '.'+' .'.join([i for i in dir(self) if not i.startswith('__') and hasattr(inspect.getattr_static(self,i)
         , '__call__')])
         variables = '.'+' .'.join([i for i in dir(self) if not i.startswith('__') and not hasattr(inspect.getattr_static(self,i)
         , '__call__')])
-        repr_str = f"""type: {type(self)}
+        repr_str = \
+f"""{self.pl.name} @ {self.base}
+exists: {self.exists}
+type: {type(self)}
 functions: {funcs}
 variables: {variables}"""
-        return f"""{self.name} @ {self.base} ({exists})
-{repr_str}"""
+        return repr_str
```

### Comparing `hhnk_research_tools-2023.2/hhnk_research_tools/folder_file_classes/folder_file_classes.py` & `hhnk_research_tools-2023.3/hhnk_research_tools/folder_file_classes/folder_file_classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,15 +124,18 @@
     def unlink_contents(self, names=[], rmfiles=True, rmdirs=False):
         """unlink all content when names is an empty list. Otherwise just remove the names."""
         if not names:
             names=self.content
         for name in names:
             pathname = self.pl / name
             try:
-                if pathname.exists:
+                if pathname.exists():
+                    #FIXME rmdir is only allowed for empty dirs
+                    #can use shutil.rmtree, but this can be dangerous, 
+                    #not sure if we should support that here.
                     if pathname.is_dir():
                         if rmdirs:
                             pathname.rmdir()
                     else:
                         if rmfiles:
                             pathname.unlink()
             except Exception as e:
```

### Comparing `hhnk_research_tools-2023.2/hhnk_research_tools/folder_file_classes/sqlite_class.py` & `hhnk_research_tools-2023.3/hhnk_research_tools/folder_file_classes/sqlite_class.py`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-2023.2/hhnk_research_tools/folder_file_classes/threedi_schematisation.py` & `hhnk_research_tools-2023.3/hhnk_research_tools/folder_file_classes/threedi_schematisation.py`

 * *Files 6% similar despite different names*

```diff
@@ -96,14 +96,19 @@
             self.friction = self.get_raster_path(
                 table_name="v2_global_settings", col_name="frict_coef_file"
             )
             self.infiltration = self.get_raster_path(
                 table_name="v2_simple_infiltration", col_name="infiltration_rate_file"
             )
 
+            landuse = [i for i in self.pl.glob("landuse_*.tif")]
+            if len(landuse)==0:
+                landuse = [""]
+            self.landuse = File(landuse[0])
+
 
         def get_raster_path(self, table_name, col_name):
             """Read the sqlite to check which rasters are used in the model.
             This only works for models from Klondike release onwards, where we only have
             one global settings row."""
 
             if self.caller.database.exists:
@@ -128,15 +133,16 @@
 
         def __repr__(self):
             return f"""  
     dem - {self.dem.name}
     storage - {self.storage.name}
     friction - {self.friction.name}
     infiltration - {self.infiltration.name}
-        """
+    landuse - {self.landuse.name}
+"""
 
 
 class ThreediResult(Folder):
     """Result of threedi simulation. Base files are .nc and .h5.
     Use .grid to access GridH5ResultAdmin and .admin to access GridH5Admin"""
 
     def __init__(self, base):
```

### Comparing `hhnk_research_tools-2023.2/hhnk_research_tools/gis/__init__.py` & `hhnk_research_tools-2023.3/hhnk_research_tools/gis/__init__.py`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-2023.2/hhnk_research_tools/gis/raster.py` & `hhnk_research_tools-2023.3/hhnk_research_tools/gis/raster.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,14 +148,22 @@
     def open_gdal_source_write(self):
         """
         open source with write access
         """
         return gdal.Open(str(self.source_path), gdal.GA_Update)
 
 
+    def unlink_if_exists(self):
+        """Remove file if it exists
+        overwrites function from File class"""
+        super().unlink_if_exists()
+        if not self.pl.exists():
+            self.source_set=False
+
+
     @property
     def exists(self):
         if self.source_set: #check this first for speed.
             return True
         else:
             path_exists = os.path.exists(self.source_path)
             if not self.source_set:
@@ -260,20 +268,21 @@
         minx += window[0] *self.metadata.pixel_width
         maxy += window[1] * self.metadata.pixel_height
         maxx = minx + window[2] *self.metadata.pixel_width
         miny = maxy + window[3] * self.metadata.pixel_height
         
         return geometry.box(minx=minx, miny=miny, maxx=maxx, maxy=maxy)
     
+
     def generate_blocks_geometry(self) -> gpd.GeoDataFrame:
         """Create blocks with shapely geometry"""
-        self.generate_blocks()
-        blocks_df =gpd.GeoDataFrame(self.blocks, geometry=self.blocks["window_readarray"].apply(self._generate_blocks_geometry_row), crs=self.metadata.projection)
-        self.blocks = blocks_df
-        return blocks_df
+        self.blocks = self.generate_blocks()
+        self.blocks =gpd.GeoDataFrame(self.blocks, geometry=self.blocks["window_readarray"].apply(self._generate_blocks_geometry_row), crs=self.metadata.projection)
+        return self.blocks
+
 
     def sum_labels(self, labels_raster, labels_index):
         """Calculate the sum of the rastervalues per label."""
         if labels_raster.shape != self.shape:
             raise Exception(f'label raster shape {labels_raster.shape} does not match the raster shape {self.shape}')
 
         accum = None
@@ -294,27 +303,29 @@
             else:
                 accum += result
         return accum
 
 
     def iter_window(self, min_block_size=None):
         """Iterate of the raster using blocks, only returning the window, not the values."""
-        if not hasattr(self,'blocks'):
+        if not hasattr(self,'blocks') or min_block_size is not None:
             if min_block_size is not None:
                  self.min_block_size = min_block_size
                 
             _ = self.generate_blocks_geometry()
 
         for idx, block_row in self.blocks.iterrows():
             window=block_row['window_readarray']
             yield idx, window, block_row
 
+
     def to_file(self):
         pass
 
+
     def __iter__(self):
         if not hasattr(self,'blocks'):
             _ = self.generate_blocks()
 
         for idx, block_row in self.blocks.iterrows():
             window=block_row['window_readarray']
             block = self._read_array(window=window)
@@ -328,15 +339,14 @@
     Shape: {self.metadata.shape}
     Pixelsize: {self.metadata.pixel_width}"""
         else:
             return f"""{self.__class__}
     Source: {self.source_path}, exists:{self.exists}"""
 
 
-
     def create(self, metadata, nodata, verbose=False, overwrite=False):
         """Create empty raster
         metadata : RasterMetadata instance
         nodata: int
         """
         #Check if function should continue.
         if verbose:
@@ -371,15 +381,15 @@
     
     Metadata can be created by supplying either: 
     1. gdal_src
     2. res, bounds
     """
     def __init__(self, gdal_src=None, res=None, bounds_dict=None, proj='epsg:28992'):
         """gdal_src = gdal.Open(raster_source)
-        bounds = {minx:, maxx:, miny:, maxy:}
+        bounds = {"minx":, "maxx":, "miny":, "maxy":}
         Projection only implemented for epsg:28992"""
 
         if gdal_src is not None:
             self.proj = gdal_src.GetProjection()
             self.georef = gdal_src.GetGeoTransform()
 
             self.x_res = gdal_src.RasterXSize
```

### Comparing `hhnk_research_tools-2023.2/hhnk_research_tools/gis/vector.py` & `hhnk_research_tools-2023.3/hhnk_research_tools/gis/vector.py`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-2023.2/hhnk_research_tools/processes.py` & `hhnk_research_tools-2023.3/hhnk_research_tools/processes.py`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-2023.2/hhnk_research_tools/raster_functions.py` & `hhnk_research_tools-2023.3/hhnk_research_tools/raster_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import os
 import types
 
 
 DEFAULT_CREATE_OPTIONS = [f"COMPRESS=ZSTD", f"TILED=YES", "PREDICTOR=2", "ZSTD_LEVEL=1"]
 
 # Loading
+#TODO deprecate? replaced by hrt.Raster
 def _get_array_from_bands(gdal_file, band_count, window, raster_source):
     try:
         if band_count == 1:
             band = gdal_file.GetRasterBand(1)
             if window is not None:
                 raster_array = band.ReadAsArray(
                     xoff=window[0],
@@ -59,14 +60,15 @@
             raise ValueError(
                 f"Unexpected number of bands in raster {raster_source} (expect 1 or 3)"
             )
     except Exception as e:
         raise e
 
 
+#TODO deprecate? replaced by hrt.Raster
 def load_gdal_raster(raster_source, window=None, return_array=True, band_count=None):
     """
     Loads a raster (tif) and returns an array of its values, its no_data value and
     dict containing associated metadata
     returns raster_array, no_data, metadata
     """
     try:
@@ -213,16 +215,21 @@
             # elif datatype==gdal.GDT_Int16:
             # options=[f"COMPRESS=LERC_ZSTD", f"TILED=YES", "PREDICTOR=2", "ZSTD_LEVEL=1", "MAX_Z_ERROR=0.001"]
             create_options=DEFAULT_CREATE_OPTIONS
 
             # else:
             #     options = [f"COMPRESS=DEFLATE", f"TILED=YES", "PREDICTOR=2", "ZSTD_LEVEL=1"]
 
+        if driver=="MEM":
+            allow_emptypath=True
+        else:
+            allow_emptypath=False
         if check_create_new_file(output_file=file_name, 
-                                    overwrite=overwrite) or driver == "MEM":
+                                    overwrite=overwrite,
+                                    allow_emptypath=allow_emptypath) or driver == "MEM":
 
             target_ds = gdal.GetDriverByName(driver).Create(
                 str(file_name),
                 meta.x_res,
                 meta.y_res,
                 num_bands,
                 datatype,
```

### Comparing `hhnk_research_tools-2023.2/hhnk_research_tools/sql_functions.py` & `hhnk_research_tools-2023.3/hhnk_research_tools/sql_functions.py`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-2023.2/hhnk_research_tools/threedi/construct_rain_scenario.py` & `hhnk_research_tools-2023.3/hhnk_research_tools/threedi/construct_rain_scenario.py`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-2023.2/hhnk_research_tools/threedi/construct_rain_scenario_dataframe.py` & `hhnk_research_tools-2023.3/hhnk_research_tools/threedi/construct_rain_scenario_dataframe.py`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-2023.2/hhnk_research_tools/threedi/geometry_functions.py` & `hhnk_research_tools-2023.3/hhnk_research_tools/threedi/geometry_functions.py`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-2023.2/hhnk_research_tools/threedi/grid.py` & `hhnk_research_tools-2023.3/hhnk_research_tools/threedi/grid.py`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-2023.2/hhnk_research_tools/threedi/gridedit.py` & `hhnk_research_tools-2023.3/hhnk_research_tools/threedi/gridedit.py`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-2023.2/hhnk_research_tools/variables.py` & `hhnk_research_tools-2023.3/hhnk_research_tools/variables.py`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-2023.2/hhnk_research_tools.egg-info/PKG-INFO` & `hhnk_research_tools-2023.3/hhnk_research_tools.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: hhnk-research-tools
-Version: 2023.2
+Version: 2023.3
 Summary: General tools for analysis, data manipulation and threedi interaction for analysis of water systems
 Home-page: https://github.com/HHNK/hhnk-research-tools
 Author: Wietse van Gerwen
 Author-email: w.vangerwen@hhnk.nl
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/HHNK/hhnk-research-tools/issues
-Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
+
+UNKNOWN
+
```

### Comparing `hhnk_research_tools-2023.2/hhnk_research_tools.egg-info/SOURCES.txt` & `hhnk_research_tools-2023.3/hhnk_research_tools.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -20,12 +20,22 @@
 hhnk_research_tools/gis/vector.py
 hhnk_research_tools/threedi/__init__.py
 hhnk_research_tools/threedi/construct_rain_scenario.py
 hhnk_research_tools/threedi/construct_rain_scenario_dataframe.py
 hhnk_research_tools/threedi/geometry_functions.py
 hhnk_research_tools/threedi/grid.py
 hhnk_research_tools/threedi/gridedit.py
+hhnk_research_tools/threedi/read_api_file.py
 hhnk_research_tools/threedi/variables/__init__.py
 hhnk_research_tools/threedi/variables/gridadmin.py
 hhnk_research_tools/threedi/variables/rain_dataframe.py
 hhnk_research_tools/threedi/variables/results_mapping.py
-hhnk_research_tools/threedi/variables/variables_container.py
+hhnk_research_tools/threedi/variables/variables_container.py
+hhnk_research_tools/waterschadeschatter/__init__.py
+hhnk_research_tools/waterschadeschatter/wss_calculations.py
+hhnk_research_tools/waterschadeschatter/wss_loading.py
+hhnk_research_tools/waterschadeschatter/wss_main.py
+hhnk_research_tools/waterschadeschatter/resources/__init__.py
+hhnk_research_tools/waterschadeschatter/resources/cfg_hhnk_2020.cfg
+hhnk_research_tools/waterschadeschatter/resources/cfg_lizard.cfg
+hhnk_research_tools/waterschadeschatter/resources/cfg_lizard_servicedesk.cfg
+hhnk_research_tools/waterschadeschatter/resources/cfg_stowa_standaard.cfg
```

### Comparing `hhnk_research_tools-2023.2/setup.py` & `hhnk_research_tools-2023.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 import codecs
 import re
 import os
 
-here = os.path.abspath(os.path.dirname(__file__))
 
 
 def read(*parts):
+    here = os.path.abspath(os.path.dirname(__file__))
     with codecs.open(os.path.join(here, *parts), "r") as fp:
         return fp.read()
 
 
 def find_version(*file_paths):
     """
     Search the file for a version string.
@@ -36,20 +36,23 @@
         "Bug Tracker": "https://github.com/HHNK/hhnk-research-tools/issues",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    packages=find_packages(),
+    packages=find_packages(exclude=["tests"]),
     python_requires=">=3.7",
     install_requires=[
         # "numpy>=1.17.0",  # Was 1.19.1
         # "Shapely>=1.6.4",  # Was 1.7.0
         # "gdal>=2.4.0",  # Was 3.1.4
         # "pandas>=0.25.3",  # Was 1.0.1
         # "geopandas>=0.6.0",  # Was 0.7.0
         # "threedigrid>=1.0.16",  # Was 1.0.25
         # "xarray",
         # "threedigrid_builder",
     ],
+    # package_dir={"": r"waterschadeschatter/resources"},
+    package_data={"": ["*.cfg"]},
+    include_package_data=True,
 )
```

