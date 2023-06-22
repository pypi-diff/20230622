# Comparing `tmp/geomappy-0.0.3.tar.gz` & `tmp/geomappy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geomappy-0.0.3.tar", last modified: Wed Jun 21 13:11:02 2023, max compression
+gzip compressed data, was "geomappy-0.0.4.tar", last modified: Thu Jun 22 16:12:55 2023, max compression
```

## Comparing `geomappy-0.0.3.tar` & `geomappy-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,31 @@
-drwxr-xr-x   0 jroebroek   (501) staff       (20)        0 2023-06-21 13:11:02.587903 geomappy-0.0.3/
--rw-r--r--   0 jroebroek   (501) staff       (20)     1072 2021-12-02 09:00:50.000000 geomappy-0.0.3/LICENSE
--rw-r--r--   0 jroebroek   (501) staff       (20)      224 2023-06-21 13:11:02.587593 geomappy-0.0.3/PKG-INFO
--rw-r--r--   0 jroebroek   (501) staff       (20)      384 2022-01-21 17:42:19.000000 geomappy-0.0.3/README.md
-drwxr-xr-x   0 jroebroek   (501) staff       (20)        0 2023-06-21 13:11:02.584528 geomappy-0.0.3/geomappy/
--rw-r--r--   0 jroebroek   (501) staff       (20)      913 2023-03-15 14:34:21.000000 geomappy-0.0.3/geomappy/__init__.py
--rw-r--r--   0 jroebroek   (501) staff       (20)    10988 2022-02-10 08:57:53.000000 geomappy-0.0.3/geomappy/basemap.py
--rw-r--r--   0 jroebroek   (501) staff       (20)     2011 2022-01-24 09:11:22.000000 geomappy-0.0.3/geomappy/bounds.py
--rw-r--r--   0 jroebroek   (501) staff       (20)    14232 2023-03-15 22:07:52.000000 geomappy-0.0.3/geomappy/colors.py
--rw-r--r--   0 jroebroek   (501) staff       (20)    10688 2022-01-24 09:11:22.000000 geomappy-0.0.3/geomappy/geodataframe.py
--rw-r--r--   0 jroebroek   (501) staff       (20)    52096 2022-01-24 09:11:22.000000 geomappy-0.0.3/geomappy/plotting.py
--rw-r--r--   0 jroebroek   (501) staff       (20)     2260 2021-11-27 12:28:51.000000 geomappy-0.0.3/geomappy/utils.py
--rw-r--r--   0 jroebroek   (501) staff       (20)    11158 2023-02-07 17:46:57.000000 geomappy-0.0.3/geomappy/xarray.py
-drwxr-xr-x   0 jroebroek   (501) staff       (20)        0 2023-06-21 13:11:02.586525 geomappy-0.0.3/geomappy.egg-info/
--rw-r--r--   0 jroebroek   (501) staff       (20)      224 2023-06-21 13:11:02.000000 geomappy-0.0.3/geomappy.egg-info/PKG-INFO
--rw-r--r--   0 jroebroek   (501) staff       (20)      370 2023-06-21 13:11:02.000000 geomappy-0.0.3/geomappy.egg-info/SOURCES.txt
--rw-r--r--   0 jroebroek   (501) staff       (20)        1 2023-06-21 13:11:02.000000 geomappy-0.0.3/geomappy.egg-info/dependency_links.txt
--rw-r--r--   0 jroebroek   (501) staff       (20)       93 2023-06-21 13:11:02.000000 geomappy-0.0.3/geomappy.egg-info/requires.txt
--rw-r--r--   0 jroebroek   (501) staff       (20)        9 2023-06-21 13:11:02.000000 geomappy-0.0.3/geomappy.egg-info/top_level.txt
--rw-r--r--   0 jroebroek   (501) staff       (20)       38 2023-06-21 13:11:02.587991 geomappy-0.0.3/setup.cfg
--rw-r--r--   0 jroebroek   (501) staff       (20)      456 2023-06-21 13:03:26.000000 geomappy-0.0.3/setup.py
-drwxr-xr-x   0 jroebroek   (501) staff       (20)        0 2023-06-21 13:11:02.586857 geomappy-0.0.3/tests/
--rw-r--r--   0 jroebroek   (501) staff       (20)     3144 2022-01-20 15:44:19.000000 geomappy-0.0.3/tests/test_plotting.py
+drwxr-xr-x   0 jroebroek   (501) staff       (20)        0 2023-06-22 16:12:55.948612 geomappy-0.0.4/
+-rw-r--r--   0 jroebroek   (501) staff       (20)     1072 2021-12-02 09:00:50.000000 geomappy-0.0.4/LICENSE
+-rw-r--r--   0 jroebroek   (501) staff       (20)      224 2023-06-22 16:12:55.948319 geomappy-0.0.4/PKG-INFO
+-rw-r--r--   0 jroebroek   (501) staff       (20)      384 2022-01-21 17:42:19.000000 geomappy-0.0.4/README.md
+drwxr-xr-x   0 jroebroek   (501) staff       (20)        0 2023-06-22 16:12:55.946246 geomappy-0.0.4/geomappy/
+-rw-r--r--   0 jroebroek   (501) staff       (20)      964 2023-06-22 10:10:42.000000 geomappy-0.0.4/geomappy/__init__.py
+-rw-r--r--   0 jroebroek   (501) staff       (20)     4929 2023-06-22 13:12:44.000000 geomappy-0.0.4/geomappy/axes_decoration.py
+-rw-r--r--   0 jroebroek   (501) staff       (20)     7013 2023-06-22 15:02:54.000000 geomappy-0.0.4/geomappy/basemap.py
+-rw-r--r--   0 jroebroek   (501) staff       (20)     1205 2023-06-22 14:35:59.000000 geomappy-0.0.4/geomappy/bounds.py
+-rw-r--r--   0 jroebroek   (501) staff       (20)     1613 2023-06-22 13:12:44.000000 geomappy-0.0.4/geomappy/classified.py
+-rw-r--r--   0 jroebroek   (501) staff       (20)     9838 2023-06-22 13:12:44.000000 geomappy-0.0.4/geomappy/colors.py
+-rw-r--r--   0 jroebroek   (501) staff       (20)     7938 2023-06-22 15:54:39.000000 geomappy-0.0.4/geomappy/geodataframe.py
+-rw-r--r--   0 jroebroek   (501) staff       (20)     3030 2023-06-22 13:12:44.000000 geomappy-0.0.4/geomappy/legends.py
+-rw-r--r--   0 jroebroek   (501) staff       (20)    52229 2023-06-22 11:39:25.000000 geomappy-0.0.4/geomappy/plotting__.py
+-rw-r--r--   0 jroebroek   (501) staff       (20)     6985 2023-06-22 11:29:51.000000 geomappy-0.0.4/geomappy/raster.py
+-rw-r--r--   0 jroebroek   (501) staff       (20)     2389 2023-06-22 10:33:01.000000 geomappy-0.0.4/geomappy/scalar.py
+-rw-r--r--   0 jroebroek   (501) staff       (20)    17944 2023-06-22 15:38:54.000000 geomappy-0.0.4/geomappy/shapes.py
+-rw-r--r--   0 jroebroek   (501) staff       (20)      498 2023-06-22 13:12:44.000000 geomappy-0.0.4/geomappy/types.py
+-rw-r--r--   0 jroebroek   (501) staff       (20)     2184 2023-06-22 13:36:54.000000 geomappy-0.0.4/geomappy/utils.py
+-rw-r--r--   0 jroebroek   (501) staff       (20)     1993 2023-06-22 15:34:00.000000 geomappy-0.0.4/geomappy/world.py
+-rw-r--r--   0 jroebroek   (501) staff       (20)     8104 2023-06-22 15:29:23.000000 geomappy-0.0.4/geomappy/xarray.py
+drwxr-xr-x   0 jroebroek   (501) staff       (20)        0 2023-06-22 16:12:55.947677 geomappy-0.0.4/geomappy.egg-info/
+-rw-r--r--   0 jroebroek   (501) staff       (20)      224 2023-06-22 16:12:55.000000 geomappy-0.0.4/geomappy.egg-info/PKG-INFO
+-rw-r--r--   0 jroebroek   (501) staff       (20)      536 2023-06-22 16:12:55.000000 geomappy-0.0.4/geomappy.egg-info/SOURCES.txt
+-rw-r--r--   0 jroebroek   (501) staff       (20)        1 2023-06-22 16:12:55.000000 geomappy-0.0.4/geomappy.egg-info/dependency_links.txt
+-rw-r--r--   0 jroebroek   (501) staff       (20)       93 2023-06-22 16:12:55.000000 geomappy-0.0.4/geomappy.egg-info/requires.txt
+-rw-r--r--   0 jroebroek   (501) staff       (20)        9 2023-06-22 16:12:55.000000 geomappy-0.0.4/geomappy.egg-info/top_level.txt
+-rw-r--r--   0 jroebroek   (501) staff       (20)       38 2023-06-22 16:12:55.948703 geomappy-0.0.4/setup.cfg
+-rw-r--r--   0 jroebroek   (501) staff       (20)      456 2023-06-22 16:00:12.000000 geomappy-0.0.4/setup.py
+drwxr-xr-x   0 jroebroek   (501) staff       (20)        0 2023-06-22 16:12:55.947975 geomappy-0.0.4/tests/
+-rw-r--r--   0 jroebroek   (501) staff       (20)     3178 2023-06-22 10:29:09.000000 geomappy-0.0.4/tests/test_plotting.py
```

### Comparing `geomappy-0.0.3/LICENSE` & `geomappy-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `geomappy-0.0.3/geomappy/__init__.py` & `geomappy-0.0.4/geomappy/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from geomappy.geodataframe import gpd_plot_shapes, gpd_plot_classified_shapes, gpd_plot_world, gpd_plot_file
 from geomappy.xarray import xarray_plot_raster, xarray_plot_classified_raster, xarray_plot_world, xarray_plot_file
-from geomappy.basemap import basemap
-from geomappy.plotting import plot_raster, plot_classified_raster, plot_shapes, plot_classified_shapes
+from geomappy.basemap import basemap, add_ticks, add_gridlines
+from geomappy.raster import plot_raster, plot_classified_raster
+from geomappy.shapes import plot_shapes, plot_classified_shapes
 
 import matplotlib
 import warnings
 
 # Import 'show' and 'savefig' for convenience. This should be avoided in production code.
 show = matplotlib.pyplot.show
 savefig = matplotlib.pyplot.savefig
```

### Comparing `geomappy-0.0.3/geomappy/geodataframe.py` & `geomappy-0.0.4/geomappy/geodataframe.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,71 +1,51 @@
-import geopandas as gpd
-import cartopy.crs as ccrs
-import numpy as np
-from shapely.geometry import Polygon
-
-from geomappy.bounds import bounds_to_polygons
-from geomappy.plotting import plot_shapes as plot_shapes, plot_classified_shapes
-from geomappy.basemap import basemap as basemap_function
-from geomappy.utils import add_method
-
-# TODO; geo_clip
+from typing import Optional, Union, Tuple
 
+import cartopy.crs as ccrs
+import geopandas as gpd
+from cartopy.mpl.geoaxes import GeoAxes
+from matplotlib import pyplot as plt
 
-def _plot_combined_shapes(classified, *, df=None, basemap=False, figsize=(10, 10), ax=None, projection=None, xticks=30,
-                          yticks=30, fontsize=10, extent=None, basemap_kwargs=None, **kwargs):
-    if df is None:
-        raise TypeError("Internal error: df not received")
-
-    if not isinstance(fontsize, (tuple, list)):
-        fontsize = (fontsize, fontsize)
-    kwargs.update({'fontsize': fontsize[1]})
+from geomappy.basemap import basemap as basemap_function, add_gridlines, add_ticks
+from geomappy.shapes import plot_shapes, plot_classified_shapes
+from geomappy.types import Number, OptionalLegend
+from geomappy.utils import add_method, change_between_bounds_and_extent
+from geomappy.world import plot_world
+
+
+def _plot_combined_shapes(classified, df, *,
+                          figsize: Tuple[int, int] = (8, 8), ax: Optional[plt.Axes] = None, basemap: bool = True,
+                          lines: Union[Number, Tuple[Number, Number], Tuple[Tuple[Number], Tuple[Number]]] = 30,
+                          ticks: Union[Number, Tuple[Number, Number], Tuple[Tuple[Number], Tuple[Number]]] = 30,
+                          fontsize: int = 10, **kwargs) -> Tuple[plt.Axes, OptionalLegend]:
+    if isinstance(ax, GeoAxes):
+        basemap = True
 
     if basemap:
-        if isinstance(basemap_kwargs, type(None)):
-            basemap_kwargs = {}
-
-        if 'xticks' not in basemap_kwargs:
-            basemap_kwargs.update({'xticks': xticks})
-        if 'yticks' not in basemap_kwargs:
-            basemap_kwargs.update({'yticks': yticks})
-        if 'fontsize' not in basemap_kwargs:
-            basemap_kwargs.update({'fontsize': fontsize[0]})
-
-        if hasattr(ax, 'projection'):
-            projection = ax.projection
-        elif projection is not None:
-            pass
-        elif df.crs is not None:
-            projection = df.get_cartopy_projection()
-        else:
-            raise ValueError("No projection is provided, which is necessary when plotting a basemap. Search order is "
-                             "a projection set on a provided Axes, the projection parameter, the CRS of the dataframe.")
-
-        if extent is None:
-            extent = df.total_bounds.tolist()
-            basemap_kwargs.update({"extent_projection": df.get_cartopy_projection()})
-
-        ax = basemap_function(extent, ax=ax, projection=projection, figsize=figsize, **basemap_kwargs)
-        kwargs.update({'transform': projection})
-
-        crs_proj4 = projection.proj4_init
-        extent = ax.get_extent()
-        df = df.to_crs(crs_proj4).clip(Polygon(
-            ((extent[0], extent[2]), (extent[0], extent[3]), (extent[1], extent[3]), (extent[1], extent[2]))
-        ))
+        projection = df.get_cartopy_projection()
+        ax = basemap_function(ax=ax, projection=projection, figsize=figsize)
+        ax.set_extent(df.get_extent(), crs=projection)
+        ax.coastlines()
+        add_gridlines(ax, lines)
+        add_ticks(ax, ticks, fontsize=fontsize)
+        kwargs['transform'] = projection
 
     if classified:
         return plot_classified_shapes(df=df, ax=ax, figsize=figsize, **kwargs)
     else:
         return plot_shapes(df=df, ax=ax, figsize=figsize, **kwargs)
 
 
+@add_method("get_extent", gpd.GeoDataFrame, gpd.GeoSeries)
+def gpd_get_extent(self):
+    return change_between_bounds_and_extent(self.total_bounds)
+
+
 @add_method("get_cartopy_projection", gpd.GeoDataFrame, gpd.GeoSeries)
-def gpd_get_cartopy_projection(self=None):
+def gpd_get_cartopy_projection(self):
     if self.crs is None:
         raise ValueError("No projection is set on the DataArray")
 
     crs = self.crs
 
     if crs.to_epsg() == 4326:
         return ccrs.PlateCarree()
@@ -74,51 +54,38 @@
     elif crs.to_epsg() is not None:
         return ccrs.epsg(crs.to_epsg())
     else:
         return ccrs.Projection(crs)
 
 
 @add_method("plot_shapes", gpd.GeoDataFrame, gpd.GeoSeries)
-def gpd_plot_shapes(self=None, *, ax=None, **kwargs):
+def gpd_plot_shapes(self, *, ax: Optional[plt.Axes] = None, **kwargs):
     """
     Plot data from a GeoDataFrame. This function is exposed as ``plot_shapes`` in a ``GeoDataFrame``.
 
     Parameters
     ----------
-    self : GeoDataFrame
-        This is not supposed to be used directly, but as the self parameter when called from a GeoDataFrame directly
     basemap : bool, optional
         Plot a basemap behind the data.
     figsize : tuple, optional
         Matplotlib figsize parameter
     ax : Axes, optional
         Matplotlib axes/ Cartopy GeoAxes where plot is drawn on. If not provided, it will be created on the fly,
         based on the 'basemap' and 'projection' parameters.
-    projection : cartopy CRS, optional
-        A basemap will be drawn to this projection. If ax already contains a Cartopy GeoAxes, this parameter will be
-        ignored.
-    xticks : float or list, optional
-        parameter that describes the distance between two gridlines in PlateCarree coordinate terms. The default 30
-        means that every 30 degrees a gridline gets drawn. If a list is passed, the procedure is skipped and the
-        coordinates in the list are used.
-    yticks : float or list, optional
-        parameter that describes the distance between two gridlines in PlateCarree coordinate terms. The default 30
-        means that every 30 degrees a gridline gets drawn. If a list is passed, the procedure is skipped and the
-        coordinates in the list are used.
+    lines : int, tuple of ints, or tuple of tuples of ints, optional
+        parameter that describes the distance between two gridlines in lat-lon terms. The default 30
+        means that every 30 degrees a gridline gets drawn. See add_gridlines
+    ticks : int, tuple of ints, or tuple of tuples of ints, optional
+        parameter that describes the distance between two tick labels in lat-lon terms. The default 30
+        means that every 30 degrees a tick gets placed. see add_ticks
     fontsize : float/tuple, optional
         fontsize for both the lon/lat ticks and the ticks on the colorbar if one number, if a list of is passed it
         represents the basemap fontsize and the colorbar fontsize.
-    extent : list or string, optional
-        Extent of the plot, if not provided it will plot the extent belonging to dataframe. If the string "global" is
-        used, the maximum extent of the projection is set. Is only active with basemap switched on. Extent is defined
-        in lotlan by default, but can be switched to something different by passing extent_projection to basemap_kwargs.
-    basemap_kwargs : dict, optional
-        kwargs going to the basemap function
     kwargs
-        kwargs going to the plot_shapes() command
+        kwargs going to the plot_classified_shapes() command
 
     Returns
     -------
     (:obj:`~matplotlib.axes.Axes`, legend)
         Axes and legend. The legend depends on the `legend` parameter and can be None.
     """
     if isinstance(self, type(None)):
@@ -128,49 +95,36 @@
     elif isinstance(self, gpd.GeoSeries):
         return _plot_combined_shapes(classified=False, ax=ax, df=gpd.GeoDataFrame(self, crs=self.crs), **kwargs)
     else:
         raise TypeError("This method does not support positional arguments")
 
 
 @add_method("plot_classified_shapes", gpd.GeoDataFrame, gpd.GeoSeries)
-def gpd_plot_classified_shapes(self=None, *, ax=None, **kwargs):
+def gpd_plot_classified_shapes(self, *, ax: Optional[plt.Axes] = None, **kwargs):
     """
     Plot data from a GeoDataFrame. This function is exposed as ``plot_classified_shapes`` in a ``GeoDataFrame``.
 
     Parameters
     ----------
-    self : GeoDataFrame
-        This is not supposed to be used directly, but as the self parameter when called from a GeoDataFrame directly
     basemap : bool, optional
         Plot a basemap behind the data.
     figsize : tuple, optional
         Matplotlib figsize parameter
     ax : Axes, optional
         Matplotlib axes/ Cartopy GeoAxes where plot is drawn on. If not provided, it will be created on the fly,
         based on the 'basemap' and 'projection' parameters.
-    projection : cartopy CRS, optional
-        A basemap will be drawn to this projection. If ax already contains a Cartopy GeoAxes, this parameter will be
-        ignored.
-    xticks : float or list, optional
-        parameter that describes the distance between two gridlines in PlateCarree coordinate terms. The default 30
-        means that every 30 degrees a gridline gets drawn. If a list is passed, the procedure is skipped and the
-        coordinates in the list are used.
-    yticks : float or list, optional
-        parameter that describes the distance between two gridlines in PlateCarree coordinate terms. The default 30
-        means that every 30 degrees a gridline gets drawn. If a list is passed, the procedure is skipped and the
-        coordinates in the list are used.
+    lines : int, tuple of ints, or tuple of tuples of ints, optional
+        parameter that describes the distance between two gridlines in lat-lon terms. The default 30
+        means that every 30 degrees a gridline gets drawn. See add_gridlines
+    ticks : int, tuple of ints, or tuple of tuples of ints, optional
+        parameter that describes the distance between two tick labels in lat-lon terms. The default 30
+        means that every 30 degrees a tick gets placed. see add_ticks
     fontsize : float/tuple, optional
         fontsize for both the lon/lat ticks and the ticks on the colorbar if one number, if a list of is passed it
         represents the basemap fontsize and the colorbar fontsize.
-    extent : list or string, optional
-        Extent of the plot, if not provided it will plot the extent belonging to dataframe. If the string "global" is
-        used, the maximum extent of the projection is set. Is only active with basemap switched on. Extent is defined
-        in lotlan by default, but can be switched to something different by passing extent_projection to basemap_kwargs.
-    basemap_kwargs : dict, optional
-        kwargs going to the basemap function
     kwargs
         kwargs going to the plot_classified_shapes() command
 
     Returns
     -------
     (:obj:`~matplotlib.axes.Axes`, legend)
         Axes and legend. The legend depends on the `legend` parameter and can be None.
@@ -182,63 +136,52 @@
     elif isinstance(self, gpd.GeoSeries):
         return _plot_combined_shapes(classified=True, ax=ax, df=gpd.GeoDataFrame(self, crs=self.crs), **kwargs)
     else:
         raise TypeError("This method does not support positional arguments")
 
 
 @add_method("plot_world", gpd.GeoDataFrame, gpd.GeoSeries)
-def gpd_plot_world(self=None, projection=None, ax=None, extent="global", **kwargs):
+def gpd_plot_world(self, ax: Optional[plt.Axes] = None, extent: Union[Tuple[int, int, int, int], str] = 'global',
+                   projection: ccrs.Projection = ccrs.PlateCarree(),
+                   extent_projection: ccrs.Projection = ccrs.PlateCarree(), **kwargs) -> GeoAxes:
     """
     Plots the outer bounds of a GeoDataFrame on a world map.
 
     Parameters
     ----------
-    self : GeoDataFrame
-        This is not supposed to be used directly, but as the self parameter when called from a GeoDataFrame directly
     ax : :obj:`~matplotlib.axes.Axes`, optional
         Axes on which to plot the figure
     extent : list, optional
         Takes a four number list, or rasterio bounds object. It constrains the world view
         to a specific view. If not lat-lon, the extent_projection needs to be specified
+    extent_projection: cartopy.CRS
+        Projection of the extent. The default ccrs.PlateCarree().
     projection : cartopy.CRS
-        Projection of the plot. The default is None, which yields ccrs.PlateCarree(). It accepts
-        'native', which plots the map on the projection of the data.
+        Projection of the plot. The default ccrs.PlateCarree().
     kwargs
         arguments for the Basemap function
 
     Returns
     -------
-    GeoAxis
+    GeoAxes
     """
-    if projection == "native":
-        projection = self.get_cartopy_projection()
-
-    ax = basemap_function(extent, ax=ax, projection=projection, **kwargs)
-
     bounds = self.total_bounds
-    gdf = bounds_to_polygons([bounds])
-    gdf.crs = self.crs
-    gdf.plot(ax=ax, edgecolor="green", facecolor="none", transform=self.get_cartopy_projection(), zorder=2)
-
-    return ax
+    plot_world(bounds, ax=ax, extent=extent, projection=projection, extent_projection=extent_projection,
+               bounds_projection=self.get_cartopy_projection(), **kwargs)
 
 
 @add_method("plot_file", gpd.GeoDataFrame, gpd.GeoSeries)
-def gpd_plot_file(self=None, **kwargs):
+def gpd_plot_file(self, **kwargs) -> GeoAxes:
     """
     Plots a map of the outer bounds of GeoDataFrame.
 
     Parameters
     ----------
-    self : GeoDataFrame
-        This is not supposed to be used directly, but as the self parameter when called from a GeoDataFrame directly
     kwargs
         arguments for the :func:`geomappy.gpd_plot_world` function
 
     Returns
     -------
-    GeoAxis
+    GeoAxes
     """
-    ax = self.plot_world(extent=self.total_bounds, projection=self.get_cartopy_projection(),
-                         extent_projection=self.get_cartopy_projection(), **kwargs)
-
-    return ax
+    return self.plot_world(extent=self.get_extent(), projection=self.get_cartopy_projection(),
+                           extent_projection=self.get_cartopy_projection(), **kwargs)
```

### Comparing `geomappy-0.0.3/geomappy/plotting.py` & `geomappy-0.0.4/geomappy/plotting__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 import copy
+
 import cartopy
 import cartopy.crs as ccrs
-import matplotlib.pyplot as plt
 import geopandas as gpd
-import pandas as pd
+import matplotlib.pyplot as plt
 import numpy as np
-from geopandas.plotting import plot_polygon_collection, plot_linestring_collection, plot_point_collection
+import pandas as pd
+from geopandas.plotting import _plot_polygon_collection, _plot_linestring_collection, _plot_point_collection
 from matplotlib.cm import ScalarMappable
 from matplotlib.colors import Colormap, BoundaryNorm, Normalize, ListedColormap, NoNorm
 from shapely.geometry import Point
 
-from geomappy.colors import cmap_discrete, create_colorbar_axes, add_colorbar, legend_patches
+from geomappy.axes_decoration import create_colorbar_axes, add_colorbar, legend_patches
+from geomappy.colors import cmap_discrete
 
 
 # PLOTTING
 class Plot:
     """
     Plot object. Handles the creation of the Axes if none is provided, stores the parameters for plotting and deals
     with the Axes makeup when the plot is drawn.
     """
+
     def __init__(self, ax, figsize, legend, params, **kwargs):
         """Sets the parameters and creates the Axes if not provided"""
         if ax is None:
             _, ax = plt.subplots(figsize=figsize)
 
         self.ax = ax
         self.kwargs = kwargs
@@ -44,14 +47,15 @@
 
 
 class PlotRaster(Plot):
     """
     Plot object for raster data. If a GeoAxes is provided the `extent` and `transform` will be inferred if not provided.
     If this leads to the wrong result they can be passed in directly as keyword arguments.
     """
+
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         if isinstance(self.ax, cartopy.mpl.geoaxes.GeoAxes):
             if 'extent' not in kwargs:
                 self.kwargs['extent'] = self.ax.get_extent()
             if 'transform' not in kwargs:
                 self.kwargs["transform"] = self.ax.projection
@@ -61,14 +65,15 @@
 
 
 class PlotShapes(Plot):
     """
     Plot object for polygon/point data. If a GeoAxes is provided the `transform` will be inferred if not provided.
     If this leads to the wrong result it can be passed in directly as keyword argument.
     """
+
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         if isinstance(self.ax, cartopy.mpl.geoaxes.GeoAxes):
             if 'transform' not in kwargs:
                 self.kwargs["transform"] = ccrs.PlateCarree()
 
     @staticmethod
@@ -183,30 +188,30 @@
             facecolor = pd.Series([facecolor] * df.shape[0])
         if not isinstance(edgecolor, np.ndarray):
             edgecolor = pd.Series([edgecolor] * df.shape[0])
 
         # plot all Polygons and all MultiPolygon components in the same collection
         polys = df.geometry[poly_idx]
         if not polys.empty:
-            plot_polygon_collection(ax, polys, facecolor=facecolor[poly_idx], edgecolor=edgecolor[poly_idx],
-                                    linewidth=linewidth, **kwargs)
+            _plot_polygon_collection(ax, polys, facecolor=facecolor[poly_idx], edgecolor=edgecolor[poly_idx],
+                                     linewidth=linewidth, **kwargs)
 
         # plot all LineStrings and MultiLineString components in same collection
         lines = df.geometry[line_idx]
         if not lines.empty:
-            plot_linestring_collection(ax, lines, facecolor=facecolor[line_idx], edgecolor=edgecolor[line_idx],
-                                       linewidth=linewidth, **kwargs)
+            _plot_linestring_collection(ax, lines, facecolor=facecolor[line_idx], edgecolor=edgecolor[line_idx],
+                                        linewidth=linewidth, **kwargs)
 
         # plot all Points in the same collection
         points = df.geometry[point_idx]
         if not points.empty:
             if isinstance(markersize, np.ndarray):
                 markersize = markersize[point_idx]
-            plot_point_collection(ax, points, facecolor=facecolor[point_idx], edgecolor=edgecolor[point_idx],
-                                  markersize=markersize, linewidth=linewidth, **kwargs)
+            _plot_point_collection(ax, points, facecolor=facecolor[point_idx], edgecolor=edgecolor[point_idx],
+                                   markersize=markersize, linewidth=linewidth, **kwargs)
 
     def _draw(self, geometry, markersize, linewidth):
         """Sets the colors that will be passed on to `PlotShapes._plot_geometries`"""
         values = self.params.values
         colors = pd.Series(self.params.cmap(self.params.norm(values)).tolist())
         colors[np.isnan(values)] = self.params._nan_color
         self._plot_geometries(self.ax, geometry, colors, linewidth, markersize, **self.kwargs)
@@ -236,14 +241,15 @@
     colors : array-like, optional
         Colors for `LegendPatches`. The default is None, in which case the legend will silently not be drawn.
     nan_color : matplotlib color, optionl
         Color for NaN values. It is both set in the property, as well as in the cmap instance
     extend : {"both", "neither", "max", "min"}, optional
         Extend for the colorbar. The default is 'neither'
     """
+
     def __init__(self, cmap="viridis", norm=None, colors=None, nan_color="White", bins=None, labels=None, extend=None,
                  values=None, labels_overwritten=False):
         if isinstance(cmap, type(None)):
             self._cmap = plt.cm.get_cmap("viridis")
         elif isinstance(cmap, str):
             self._cmap = plt.cm.get_cmap(cmap)
         elif isinstance(cmap, Colormap):
@@ -353,14 +359,15 @@
         Matplotlib colormap to color the data, or a string that represents one.
     nan_color : matplotlib color, optional
         Color for NaN values, the default is white
     clip_legend : bool, optional
         If bins are provided that are outside the range of data they will be clipped. The default is False. An Error
         wil be raised if all bins are clipped.
     """
+
     def __init__(self, values, bins=None, labels=None, vmin=None, vmax=None, cmap=None, nan_color='White',
                  clip_legend=False):
         super().__init__(cmap=cmap)
         cmap = self._cmap
 
         values = np.array(values)
         if np.issubdtype(values.dtype, np.floating):
@@ -468,14 +475,15 @@
         Color for NaN values, the default is white
     clip_legend : bool, optional
         If bins are provided that are outside the range of data they will be clipped. The default is False. An Error
         wil be raised if all bins are clipped.
     suppress_warnings : bool, optional
         Only 9 bins will be drawn by default. Set this parameter to True to avoid this limitation
     """
+
     def __init__(self, values, bins=None, labels=None, colors=None, cmap=None, nan_color="White", clip_legend=False,
                  suppress_warnings=False):
         data = values[~np.isnan(values)]
 
         if isinstance(bins, type(None)):
             bins = np.unique(data)
         else:
@@ -512,15 +520,15 @@
 
         if clip_legend:
             present = np.isin(bins, classes)
             bins = bins[present]
             labels = labels[present]
             colors = colors[present]
 
-        boundaries = np.hstack((bins[0]-1, [(bins[i]+bins[i-1])/2 for i in range(1, len(bins))], bins[-1]+1))
+        boundaries = np.hstack((bins[0] - 1, [(bins[i] + bins[i - 1]) / 2 for i in range(1, len(bins))], bins[-1] + 1))
         self._norm = BoundaryNorm(boundaries, len(bins))
         self._cmap = ListedColormap(colors)
         self._nan_color = nan_color
         self._cmap.set_bad(nan_color)
         self._colors = colors
         self._labels = labels
         self._labels_overwritten = True
@@ -528,16 +536,17 @@
         self._values = values
 
 
 # LEGEND OBJECTS (both colorbar and legend_patches)
 class Legend:
     """Parent object for the legends. It contains a method `create` to create a Colorbar or LegendPatches object.
     A custom Legend object can be created, it only needs to expose a `draw` method with parameters `ax` and `params`"""
+
     @staticmethod
-    def create(legend, aspect=30, pad_fraction=0.6, legend_ax=None, fontsize=None,  legend_kwargs=None):
+    def create(legend, aspect=30, pad_fraction=0.6, legend_ax=None, fontsize=None, legend_kwargs=None):
         """
         Creates a Legend object of type Colorbar or LegendPatches
 
         Parameters
         ----------
         legend : {'colorbar', 'legend'} or Legend or None
             Switch for the creation of a legend. `colorbar` will create a ``Colorbar`` object while `legend` will
@@ -587,14 +596,15 @@
     fontsize : numeric, optional
         Fontsize for the legend
     kwargs : dict
         Keyword arguments for ``cbar_decorater function``
 
     todo; move all parameters from cbar_decorator to __init__
     """
+
     def __init__(self, aspect=30, pad_fraction=0.6, legend_ax=None, fontsize=None, **kwargs):
         self._aspect = aspect
         self._pad_fraction = pad_fraction
         self._legend_ax = legend_ax
         self._fontsize = kwargs.pop('fontsize', fontsize)
         self._kwargs = kwargs
 
@@ -694,14 +704,15 @@
         Align the title of the legend box to the left. The default is True
     handles_kwargs : dict, optional
         # todo; move this function here
         Keyword arguments for the `legend_patches` function
     kwargs
         Keyword arguments for the `ax.legend` function call.
     """
+
     def __init__(self, legend_ax=None, facecolor='white', edgecolor='lightgrey', fontsize=None, patch_type="patch",
                  patch_edgecolor="lightgrey", title=None, align_left=True, handles_kwargs=None, **kwargs):
         self._facecolor = facecolor
         self._edgecolor = edgecolor
         self._patch_edgecolor = patch_edgecolor
         self._patch_type = patch_type
         self._title = title
@@ -841,15 +852,16 @@
     else:
         # Case of boolean raster
         plot_params = ClassifiedPlotParams(values=m, bins=[0, 1], labels=["False", "True"], colors=['Lightgrey', 'Red'])
 
     legend = Legend.create(legend, aspect=aspect, pad_fraction=pad_fraction, legend_ax=legend_ax, fontsize=fontsize,
                            legend_kwargs=legend_kwargs)
 
-    ax, legend = PlotRaster(ax=ax, figsize=figsize, fontsize=fontsize, params=plot_params, legend=legend, **kwargs).draw()
+    ax, legend = PlotRaster(ax=ax, figsize=figsize, fontsize=fontsize, params=plot_params, legend=legend,
+                            **kwargs).draw()
 
     if force_equal_figsize and legend != 'colorbar':
         if isinstance(legend_kwargs, type(None)):
             legend_kwargs = {}
         create_colorbar_axes(ax=ax, aspect=aspect, pad_fraction=pad_fraction,
                              position=legend_kwargs.get("position", "right")).axis("off")
 
@@ -916,20 +928,21 @@
 
     Returns
     -------
     (:obj:`~matplotlib.axes.Axes`, legend)
         Axes and legend. The legend depends on the `legend` parameter and can be None.
     """
     plot_params = ClassifiedPlotParams(values=m, bins=bins, labels=labels, colors=colors, cmap=cmap,
-                                       nan_color=nan_color, clip_legend=clip_legend, suppress_warnings=suppress_warnings)
+                                       nan_color=nan_color, clip_legend=clip_legend,
+                                       suppress_warnings=suppress_warnings)
 
     legend = Legend.create(legend, aspect=aspect, pad_fraction=pad_fraction, legend_ax=legend_ax, fontsize=fontsize,
                            legend_kwargs=legend_kwargs)
 
-    ax, legend = PlotRaster(ax=ax, figsize=figsize, fontsize=fontsize, params=plot_params, legend=legend, **kwargs)\
+    ax, legend = PlotRaster(ax=ax, figsize=figsize, fontsize=fontsize, params=plot_params, legend=legend, **kwargs) \
         .draw()
 
     if force_equal_figsize and legend != 'colorbar':
         if isinstance(legend_kwargs, type(None)):
             legend_kwargs = {}
         create_colorbar_axes(ax=ax, aspect=aspect, pad_fraction=pad_fraction,
                              position=legend_kwargs.get("position", "right")).axis("off")
@@ -1039,15 +1052,15 @@
         # Case of boolean raster
         plot_params = ClassifiedPlotParams(values=values, bins=[0, 1], labels=['False', 'True'],
                                            colors=['Lightgrey', 'Red'])
 
     legend = Legend.create(legend, aspect=aspect, pad_fraction=pad_fraction, legend_ax=legend_ax, fontsize=fontsize,
                            legend_kwargs=legend_kwargs)
 
-    ax, legend = PlotShapes(ax=ax, figsize=figsize, fontsize=fontsize, params=plot_params, legend=legend, **kwargs)\
+    ax, legend = PlotShapes(ax=ax, figsize=figsize, fontsize=fontsize, params=plot_params, legend=legend, **kwargs) \
         .draw(geometry=geometry, markersize=markersize, linewidth=linewidth)
 
     if force_equal_figsize and legend != 'colorbar':
         if isinstance(legend_kwargs, type(None)):
             legend_kwargs = {}
         create_colorbar_axes(ax=ax, aspect=aspect, pad_fraction=pad_fraction,
                              position=legend_kwargs.get("position", "right")).axis("off")
```

### Comparing `geomappy-0.0.3/geomappy/utils.py` & `geomappy-0.0.4/geomappy/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,41 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 Utilities used in geomappy. Interesting functions to use outside the internal scope are
 progress_bar and reproject_map_like
 """
 from functools import wraps
+from numbers import Number
+from typing import Tuple, Union
+
 import numpy as np
+from numpy import ndarray
+from rasterio.coords import BoundingBox
 
 
-def grid_from_corners(v, shape):
+def _grid_from_corners(v: Tuple[Union[Number, ndarray]], shape: Tuple[int, int]):
     """
     function returns an linearly interpolated grid from values at the corners
 
     Parameters
     ----------
-    v : list
+    v : tuple
         List of four numeric values that will be interpolated. Order of the values is clockwise; starting from the upper
         left corner.
-    shape : list
+    shape : tuple
         List of two integers, determining the shape of the array that will be returned
 
     Returns
     -------
     :obj:`~numpy.ndarray`
         Interpolated array
     """
-    if type(v) not in (tuple, list, np.ndarray):
-        raise TypeError("corner values need to be supplied in a list")
-    else:
-        if len(v) != 4:
-            raise ValueError("Four corner values need to be given")
-    if type(shape) not in (tuple, list):
-        raise TypeError("shape needs to be a list")
-    else:
-        if len(shape) != 2:
-            raise ValueError("shape needs to contain 2 integers")
-        if type(shape[0]) not in (float, int) or type(shape[1]) not in (float, int):
-            raise TypeError("shape needs to be provided as integers")
-
-    grid = np.linspace(np.linspace(v[0], v[1], shape[1]),
+    return np.linspace(np.linspace(v[0], v[1], shape[1]),
                        np.linspace(v[3], v[2], shape[1]), shape[0])
-    return grid
 
 
 def add_method(name, *cls):
     """
     Decorator to add functions to existing classes
 
     Parameters
@@ -54,16 +45,29 @@
     cls : class or list of classes
         class or classes that the function that the wrapper is placed around will be added to
 
     Notes
     -----
     https://medium.com/@mgarod/dynamically-add-a-method-to-a-class-in-python-c49204b85bd6
     """
+
     def decorator(func):
         @wraps(func)
         def wrapper(self, *args, **kwargs):
             return func(self, *args, **kwargs)
+
         for c in cls:
             setattr(c, name, wrapper)
         # Note we are not binding func, but wrapper which accepts self but does exactly the same as func
-        return func # returning func means func can still be used normally
+        return func  # returning func means func can still be used normally
+
     return decorator
+
+
+def check_increasing_and_unique(v: np.ndarray) -> None:
+    vs = np.sort(np.unique(v))
+    if not np.array_equal(v, vs):
+        raise ValueError("Levels are not sorted or contain double entries")
+
+
+def change_between_bounds_and_extent(x: Union[BoundingBox, Tuple[Number, Number, Number, Number]]):
+    return x[0], x[2], x[1], x[3]
```

### Comparing `geomappy-0.0.3/geomappy/xarray.py` & `geomappy-0.0.4/geomappy/xarray.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,86 +1,55 @@
-import pyproj
-import xarray as xr
+from typing import Optional, Union, Tuple
+
 import cartopy.crs as ccrs
-import numpy as np
-from rasterio.enums import Resampling
-from geomappy.bounds import bounds_to_polygons
-from geomappy.plotting import plot_raster
-from geomappy.plotting import plot_classified_raster
-from geomappy.basemap import basemap as basemap_function
-from geomappy.utils import add_method
-
-# TODO; make a geo_clip function supporting lon_lat
-# TODO; clip -> reproject -> clip (Transformer().transform_bounds())
-# TODO; automatically switch basemap on when a geoaxes is provided
-
-def _plot_combined_raster(classified, *, da=None, basemap=False, figsize=(10, 10), ax=None, projection=None, xticks=30,
-                          yticks=30, fontsize=10, extent=None, basemap_kwargs=None, resampling=Resampling.nearest,
-                          **kwargs):
-    if da.ndim == 2:
-        pass
-    elif da.ndim == 3:
-        if da.shape[0] == 1:
-            da = da[0]
-        elif da.shape[0] == 3:
-            # todo; this does not work
-            da = da.transpose(da.rio.y_dim, da.rio.x_dim, '...')
-        else:
-            raise IndexError("Bands can only be 1 or 3, corresponding to values or RGB")
-    else:
+import xarray as xr
+from cartopy.mpl.geoaxes import GeoAxes
+from matplotlib import pyplot as plt
+
+from geomappy.basemap import basemap as basemap_function, add_gridlines, add_ticks
+from geomappy.raster import plot_classified_raster, plot_raster
+from geomappy.types import Number, OptionalLegend
+from geomappy.utils import add_method, change_between_bounds_and_extent
+from geomappy.world import plot_world
+
+
+def _plot_combined_raster(classified: bool, *, da: xr.DataArray, basemap: bool = True,
+                          figsize: Tuple[int, int] = (8, 8), ax: Optional[plt.Axes] = None,
+                          lines: Union[Number, Tuple[Number, Number], Tuple[Tuple[Number], Tuple[Number]]] = 30,
+                          ticks: Union[Number, Tuple[Number, Number], Tuple[Tuple[Number], Tuple[Number]]] = 30,
+                          fontsize: int = 10, **kwargs) -> Tuple[plt.Axes, OptionalLegend]:
+    if da.ndim == 3 and da.shape[0] == 1:
+        da = da[0]
+
+    if da.ndim != 2:
         raise IndexError("Only 2 or 3 dimensional DataArrays are accepted")
 
-    if not isinstance(fontsize, (tuple, list)):
-        fontsize = (fontsize, fontsize)
-    kwargs.update({'fontsize': fontsize[1]})
+    if isinstance(ax, GeoAxes):
+        basemap = True
 
     if basemap:
-        if isinstance(basemap_kwargs, type(None)):
-            basemap_kwargs = {}
-
-        if 'xticks' not in basemap_kwargs:
-            basemap_kwargs.update({'xticks': xticks})
-        if 'yticks' not in basemap_kwargs:
-            basemap_kwargs.update({'yticks': yticks})
-        if 'fontsize' not in basemap_kwargs:
-            basemap_kwargs.update({'fontsize': fontsize[0]})
-
-        if hasattr(ax, 'projection'):
-            projection = ax.projection
-        elif projection is not None:
-            pass
-        elif da.rio.crs is not None:
-            projection = da.get_cartopy_projection()
-        else:
-            raise ValueError("No projection is provided, which is necessary when plotting a basemap. Search order is "
-                             "a projection set on a provided Axes, the projection parameter, the CRS of the dataframe.")
-
-        if extent is None:
-            extent = da.rio._internal_bounds()
-            basemap_kwargs.update({"extent_projection": da.get_cartopy_projection()})
-
-        ax = basemap_function(extent, ax=ax, projection=projection, figsize=figsize, **basemap_kwargs)
-
-        minx, maxx, miny, maxy = ax.get_extent()
-
-        da = (
-            da.rio.reproject(projection, resampling=resampling)
-              .rio.clip_box(minx=minx, miny=miny, maxx=maxx, maxy=maxy)
-        )
+        projection = da.get_cartopy_projection()
+        ax = basemap_function(ax=ax, projection=projection, figsize=figsize)
+        ax.set_extent(da.get_extent(), crs=projection)
+        ax.coastlines()
+        add_gridlines(ax, lines)
+        add_ticks(ax, ticks, fontsize=fontsize)
+        kwargs['extent'] = da.get_extent()
+        kwargs['transform'] = projection
 
     a = da.to_masked_array()
 
     if classified:
         return plot_classified_raster(a, ax=ax, figsize=figsize, **kwargs)
     else:
         return plot_raster(a, ax=ax, figsize=figsize, **kwargs)
 
 
 @add_method("get_cartopy_projection", xr.core.dataarray.DataArray)
-def xarray_get_cartopy_projection(self=None):
+def xarray_get_cartopy_projection(self):
     if self.rio.crs is None:
         raise ValueError("No projection is set on the DataArray")
 
     crs = self.rio.crs
 
     if crs.to_epsg() == 4326:
         return ccrs.PlateCarree()
@@ -88,56 +57,46 @@
         return ccrs.Mercator()
     elif crs.to_epsg() is not None:
         return ccrs.epsg(crs.to_epsg())
     else:
         return ccrs.Projection(crs)
 
 
+@add_method("get_extent", xr.core.dataarray.DataArray)
+def xarray_get_extent(self):
+    return change_between_bounds_and_extent(self.rio._internal_bounds())
+
+
 @add_method("plot_raster", xr.core.dataarray.DataArray)
-def xarray_plot_raster(self=None, *, ax=None, **kwargs):
+def xarray_plot_raster(self, *, ax: Optional[plt.Axes] = None, **kwargs):
     """
     Plot data from an DataArray. This function is exposed as ``plot_raster`` in a ``DataArray``.
 
     Parameters
     ----------
     self : DataArray
         This is not supposed to be used directly, but as the self parameter when called from a DataArray directly
-    classified : bool
-        Switch between `plot_raster` and `plot_classified_raster`
     basemap : bool, optional
         Plot a basemap behind the data.
     figsize : tuple, optional
         Matplotlib figsize parameter
     ax : Axes, optional
         Matplotlib axes/ Cartopy GeoAxes where plot is drawn on. If not provided, it will be created on the fly,
         based on the 'basemap' and 'projection' parameters.
-    projection : cartopy CRS, optional
-        A basemap will be drawn to this projection. If ax already contains a Cartopy GeoAxes, this parameter will be
-        ignored.
-    xticks : float or list, optional
-        parameter that describes the distance between two gridlines in PlateCarree coordinate terms. The default 30
-        means that every 30 degrees a gridline gets drawn. If a list is passed, the procedure is skipped and the
-        coordinates in the list are used.
-    yticks : float or list, optional
-        parameter that describes the distance between two gridlines in PlateCarree coordinate terms. The default 30
-        means that every 30 degrees a gridline gets drawn. If a list is passed, the procedure is skipped and the
-        coordinates in the list are used.
+    lines : int, tuple of ints, or tuple of tuples of ints, optional
+        parameter that describes the distance between two gridlines in lat-lon terms. The default 30
+        means that every 30 degrees a gridline gets drawn. See add_gridlines
+    ticks : int, tuple of ints, or tuple of tuples of ints, optional
+        parameter that describes the distance between two tick labels in lat-lon terms. The default 30
+        means that every 30 degrees a tick gets placed. see add_ticks
     fontsize : float/tuple, optional
         fontsize for both the lon/lat ticks and the ticks on the colorbar if one number, if a list of is passed it
         represents the basemap fontsize and the colorbar fontsize.
-    extent : list or string, optional
-        Extent of the plot, if not provided it will plot the extent belonging to dataframe. If the string "global" is
-        used, the maximum extent of the projection is set. Is only active with basemap switched on. Extent is defined
-        in lotlan by default, but can be switched to something different by passing extent_projection to basemap_kwargs.
-    basemap_kwargs : dict, optional
-        kwargs going to the basemap function
-    resampling: Resampling method, optional
-            See rasterio.warp.reproject for more details.
     kwargs
-        kwargs going to the plot_raster() command
+        kwargs going to the plot_classified_raster() command
 
     Returns
     -------
     (:obj:`~matplotlib.axes.Axes`, legend)
         Axes and legend. The legend depends on the `legend` parameter and can be None.
     """
     if self is None:
@@ -145,51 +104,38 @@
     elif isinstance(self, xr.DataArray):
         return _plot_combined_raster(classified=False, ax=ax, da=self, **kwargs)
     else:
         raise TypeError("This method does not support positional arguments")
 
 
 @add_method("plot_classified_raster", xr.core.dataarray.DataArray)
-def xarray_plot_classified_raster(self=None, *, ax=None, **kwargs):
+def xarray_plot_classified_raster(self, *, ax: Optional[plt.Axes] = None, **kwargs):
     """
     Plot data from an DataArray. This function is exposed as ``plot_classified_raster`` in a ``DataArray``.
 
     Parameters
     ----------
     self : DataArray
         This is not supposed to be used directly, but as the self parameter when called from a DataArray directly
     basemap : bool, optional
         Plot a basemap behind the data.
     figsize : tuple, optional
         Matplotlib figsize parameter
     ax : Axes, optional
         Matplotlib axes/ Cartopy GeoAxes where plot is drawn on. If not provided, it will be created on the fly,
         based on the 'basemap' and 'projection' parameters.
-    projection : cartopy CRS, optional
-        A basemap will be drawn to this projection. If ax already contains a Cartopy GeoAxes, this parameter will be
-        ignored.
-    xticks : float or list, optional
-        parameter that describes the distance between two gridlines in PlateCarree coordinate terms. The default 30
-        means that every 30 degrees a gridline gets drawn. If a list is passed, the procedure is skipped and the
-        coordinates in the list are used.
-    yticks : float or list, optional
-        parameter that describes the distance between two gridlines in PlateCarree coordinate terms. The default 30
-        means that every 30 degrees a gridline gets drawn. If a list is passed, the procedure is skipped and the
-        coordinates in the list are used.
+    lines : int, tuple of ints, or tuple of tuples of ints, optional
+        parameter that describes the distance between two gridlines in lat-lon terms. The default 30
+        means that every 30 degrees a gridline gets drawn. See add_gridlines
+    ticks : int, tuple of ints, or tuple of tuples of ints, optional
+        parameter that describes the distance between two tick labels in lat-lon terms. The default 30
+        means that every 30 degrees a tick gets placed. see add_ticks
     fontsize : float/tuple, optional
         fontsize for both the lon/lat ticks and the ticks on the colorbar if one number, if a list of is passed it
         represents the basemap fontsize and the colorbar fontsize.
-    extent : list or string, optional
-        Extent of the plot, if not provided it will plot the extent belonging to dataframe. If the string "global" is
-        used, the maximum extent of the projection is set. Is only active with basemap switched on. Extent is defined
-        in lotlan by default, but can be switched to something different by passing extent_projection to basemap_kwargs.
-    basemap_kwargs : dict, optional
-        kwargs going to the basemap function
-    resampling: Resampling method, optional
-        See rasterio.warp.reproject for more details.
     kwargs
         kwargs going to the plot_classified_raster() command
 
     Returns
     -------
     (:obj:`~matplotlib.axes.Axes`, legend)
         Axes and legend. The legend depends on the `legend` parameter and can be None.
@@ -199,63 +145,52 @@
     elif isinstance(self, xr.DataArray):
         return _plot_combined_raster(classified=True, ax=ax, da=self, **kwargs)
     else:
         raise TypeError("This method does not support positional arguments")
 
 
 @add_method("plot_world", xr.core.dataarray.DataArray)
-def xarray_plot_world(self=None, projection=None, ax=None, extent="global", **kwargs):
+def xarray_plot_world(self, ax: Optional[plt.Axes] = None, extent: Union[Tuple[int, int, int, int], str] = 'global',
+                      projection: ccrs.Projection = ccrs.PlateCarree(),
+                      extent_projection: ccrs.Projection = ccrs.PlateCarree(), **kwargs) -> GeoAxes:
     """
     Plots the outer bounds of a DataArray on a world map.
 
     Parameters
     ----------
-    self : DataArray
-        This is not supposed to be used directly, but as the self parameter when called from a DataArray directly
     ax : :obj:`~matplotlib.axes.Axes`, optional
         Axes on which to plot the figure
     extent : list, optional
         Takes a four number list, or rasterio bounds object. It constrains the world view
         to a specific view. If not lat-lon, the extent_projection needs to be specified
+    extent_projection: cartopy.CRS
+        Projection of the extent. The default ccrs.PlateCarree().
     projection : cartopy.CRS
-        Projection of the plot. The default is None, which yields ccrs.PlateCarree(). It accepts
-        'native', which plots the map on the projection of the data.
+        Projection of the plot. The default ccrs.PlateCarree().
     kwargs
         arguments for the Basemap function
 
     Returns
     -------
-    GeoAxis
+    GeoAxes
     """
-    if projection == "native":
-        projection = self.get_cartopy_projection()
-
-    ax = basemap_function(extent, ax=ax, projection=projection, **kwargs)
-
     bounds = self.rio._internal_bounds()
-    gdf = bounds_to_polygons([bounds])
-    gdf.crs = self.rio.crs
-    gdf.plot(ax=ax, edgecolor="green", facecolor="none", transform=self.get_cartopy_projection(), zorder=2)
-
-    return ax
+    plot_world(bounds, ax=ax, extent=extent, projection=projection, extent_projection=extent_projection,
+               bounds_projection=self.get_cartopy_projection(), **kwargs)
 
 
 @add_method("plot_file", xr.core.dataarray.DataArray)
-def xarray_plot_file(self=None, **kwargs):
+def xarray_plot_file(self, **kwargs) -> GeoAxes:
     """
     Plots a map of the outer bounds of DataArray.
 
     Parameters
     ----------
-    self : DataArray
-        This is not supposed to be used directly, but as the self parameter when called from a DataArray directly
     kwargs
         arguments for the :func:`geomappy.xarray_plot_world` function
 
     Returns
     -------
-    GeoAxis
+    GeoAxes
     """
-    ax = self.plot_world(extent=self.rio._internal_bounds(), projection=self.get_cartopy_projection(),
-                         extent_projection=self.get_cartopy_projection(), **kwargs)
-
-    return ax
+    return self.plot_world(extent=self.get_extent(), projection=self.get_cartopy_projection(),
+                           extent_projection=self.get_cartopy_projection(), **kwargs)
```

### Comparing `geomappy-0.0.3/tests/test_plotting.py` & `geomappy-0.0.4/tests/test_plotting.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from matplotlib.colors import ListedColormap, BoundaryNorm, from_levels_and_colors
+from matplotlib.colors import ListedColormap, from_levels_and_colors
 import geomappy as mp
 import matplotlib.pyplot as plt
 import matplotlib.testing.compare
 import numpy as np
 import os
 import shutil
 import pytest
@@ -10,101 +10,100 @@
 
 def imshow(*args, **kwargs):
     f, ax = plt.subplots()
     ax.imshow(*args, **kwargs)
     return ax
 
 
-# todo; port to fixture
 def compare_images(ax1, ax2):
     try:
         os.mkdir("_test_figures")
     except FileExistsError:
         pass
 
     ax1.get_figure().savefig("_test_figures/ax_geomappy.png")
     ax2.get_figure().savefig("_test_figures/ax_matplotlib.png")
     r = matplotlib.testing.compare.compare_images("_test_figures/ax_geomappy.png", "_test_figures/ax_matplotlib.png", tol=0)
 
     shutil.rmtree("_test_figures")
 
     if r is not None:
-        raise ValueError("Images not equal")
+        return False
+
+    return True
 
 
 def test_figure_base():
     # 3D image data
     x = np.random.rand(10, 10, 3)
-    ax1, cbar = mp.plot_raster(x)
+    ax1, l = mp.plot_raster(x, legend=None)
     ax2 = imshow(x)
-    compare_images(ax1, ax2)
+    assert compare_images(ax1, ax2)
 
     # 2D image data
     x = np.random.rand(10, 10)
-    ax1, cbar = mp.plot_raster(x, legend=None)
+    ax1, l = mp.plot_raster(x, legend=None)
     ax2 = imshow(x)
-    compare_images(ax1, ax2)
+    assert compare_images(ax1, ax2)
 
 
 def test_figure_vmax():
     x = np.random.rand(10, 10)
-    ax1, cbar = mp.plot_raster(x, vmax=0.5, legend=None)
+    ax1, l = mp.plot_raster(x, vmax=0.5, legend=None)
     ax2 = imshow(x, vmax=0.5)
-    compare_images(ax1, ax2)
+    assert compare_images(ax1, ax2)
 
 
 def test_figure_vmin():
     x = np.random.rand(10, 10)
-    ax1, cbar = mp.plot_raster(x, vmin=0.5, legend=None)
+    ax1, l = mp.plot_raster(x, vmin=0.5, legend=None)
     ax2 = imshow(x, vmin=0.5)
-    compare_images(ax1, ax2)
+    assert compare_images(ax1, ax2)
 
 
 def test_figure_binary():
     x = np.random.rand(10, 10)
-    ax1, cbar = mp.plot_raster(x, bins=[0.5], legend=None)
+    ax1, l = mp.plot_raster(x, bins=(0.5,), legend=None)
     ax2 = imshow(x > 0.5, cmap=ListedColormap(["Lightgrey", "Red"]))
-    compare_images(ax1, ax2)
+    assert compare_images(ax1, ax2)
 
 
 def test_figure_classified():
     x = np.ones((10, 10))
     x[4, 4] = 2
     x[5, 5] = 5
-    ax1, cbar = mp.plot_classified_raster(x, [1, 2, 5], ['Red', "Green", "Blue"], legend=None)
-    cmap, norm = from_levels_and_colors([1, 2, 5, 6], ['Red', "Green", "Blue"])
+    ax1, l = mp.plot_classified_raster(x, levels=(1, 2, 5), colors=('Red', "Green", "Blue"), legend=None)
+    cmap, norm = from_levels_and_colors((1, 2, 5, 6), ['Red', "Green", "Blue"])
     ax2 = imshow(x, cmap=cmap, norm=norm)
-    compare_images(ax1, ax2)
+    assert compare_images(ax1, ax2)
 
 
 def test_figure_legend_patches():
     # 3D image data
     # no legend should be plotted
     x = np.random.rand(10, 10, 3)
-    ax1, cbar = mp.plot_raster(x, legend='legend')
-    ax2 = imshow(x)
-    compare_images(ax1, ax2)
+    with pytest.raises(TypeError):
+        ax1, l = mp.plot_raster(x, legend="legend")
 
     # 2D image data, without bins
     # no legend should be plotted
     x = np.random.rand(10, 10)
-    ax1, cbar = mp.plot_raster(x, legend='legend')
-    ax2 = imshow(x)
-    compare_images(ax1, ax2)
+    with pytest.raises(TypeError):
+        ax1, l = mp.plot_raster(x, legend="legend")
 
     # 2D image data, with bins
     # no legend should be plotted, which should raise an error when comparing images
     x = np.random.rand(10, 10)
-    ax1, cbar = mp.plot_raster(x, bins=[0.5], legend='legend')
+    ax1, l = mp.plot_raster(x, bins=(0.5,), legend="legend")
     ax2 = imshow(x > 0.5, cmap=ListedColormap(["Lightgrey", "Red"]))
-    with pytest.raises(ValueError):
-        compare_images(ax1, ax2)
+    assert not compare_images(ax1, ax2)
 
 
-def test_figure_colorbar():
-    # 2D image data, with bins
-    # Legend and colorbar should be different
+def test_figure_legend_and_colorbar_difference():
     x = np.random.rand(10, 10)
-    ax1, cbar = mp.plot_raster(x, bins=[0.5], legend='legend')
-    ax2, cbar = mp.plot_raster(x, bins=[0.5], legend='colorbar')
-    with pytest.raises(ValueError):
-        compare_images(ax1, ax2)
+    ax1, l = mp.plot_raster(x, bins=(0.5,), legend="legend")
+    ax2, l = mp.plot_raster(x, bins=(0.5,), legend="colorbar")
+    assert not compare_images(ax1, ax2)
+
+    ax1, l = mp.plot_raster(x, bins=(0.5, 0.8), legend="legend")
+    ax2, l = mp.plot_raster(x, bins=(0.5, 0.8), legend="colorbar")
+    assert not compare_images(ax1, ax2)
```

