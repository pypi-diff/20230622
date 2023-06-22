# Comparing `tmp/Jord-0.0.7.tar.gz` & `tmp/Jord-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Jord-0.0.7.tar", last modified: Wed Jun 21 08:58:48 2023, max compression
+gzip compressed data, was "Jord-0.0.8.tar", last modified: Thu Jun 22 13:51:21 2023, max compression
```

## Comparing `Jord-0.0.7.tar` & `Jord-0.0.8.tar`

### file list

```diff
@@ -1,137 +1,140 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:58:48.677254 Jord-0.0.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:58:48.645254 Jord-0.0.7/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-06-21 08:58:43.000000 Jord-0.0.7/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-21 08:58:43.000000 Jord-0.0.7/.github/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-21 08:58:43.000000 Jord-0.0.7/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 08:58:43.000000 Jord-0.0.7/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:58:48.649253 Jord-0.0.7/Jord.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-06-21 08:58:48.000000 Jord-0.0.7/Jord.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-06-21 08:58:48.000000 Jord-0.0.7/Jord.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 08:58:48.000000 Jord-0.0.7/Jord.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-21 08:58:48.000000 Jord-0.0.7/Jord.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-21 08:58:48.000000 Jord-0.0.7/Jord.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-21 08:58:43.000000 Jord-0.0.7/KEYWORDS.md
--rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-06-21 08:58:43.000000 Jord-0.0.7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-21 08:58:43.000000 Jord-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-06-21 08:58:48.677254 Jord-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-06-21 08:58:43.000000 Jord-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-21 08:58:43.000000 Jord-0.0.7/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:58:48.649253 Jord-0.0.7/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-21 08:58:43.000000 Jord-0.0.7/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:58:48.649253 Jord-0.0.7/jord/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:58:48.649253 Jord-0.0.7/jord/gdal_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/gdal_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/gdal_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/gdal_utilities/cloning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/gdal_utilities/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/gdal_utilities/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/gdal_utilities/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/gdal_utilities/importing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:58:48.649253 Jord-0.0.7/jord/geojson_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/geojson_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/geojson_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/geojson_utilities/geometry_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:58:48.649253 Jord-0.0.7/jord/geopandas_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/geopandas_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/geopandas_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/geopandas_utilities/geometry_filtering.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:58:48.653254 Jord-0.0.7/jord/pillow_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/pillow_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/pillow_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/pillow_utilities/exif.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/pillow_utilities/tiff.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:58:48.653254 Jord-0.0.7/jord/qgis_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/qgis_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/qgis_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/qgis_utilities/categorisation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:58:48.657254 Jord-0.0.7/jord/qgis_utilities/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/qgis_utilities/configuration/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/qgis_utilities/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/qgis_utilities/configuration/plugin_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/qgis_utilities/configuration/project_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:58:48.657254 Jord-0.0.7/jord/qgis_utilities/conversion/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/qgis_utilities/conversion/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/qgis_utilities/conversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/qgis_utilities/conversion/parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/qgis_utilities/data_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/qgis_utilities/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/qgis_utilities/geometry_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:58:48.661254 Jord-0.0.7/jord/qgis_utilities/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/qgis_utilities/helpers/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/qgis_utilities/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/qgis_utilities/helpers/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/qgis_utilities/helpers/drawing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/qgis_utilities/helpers/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/qgis_utilities/helpers/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/qgis_utilities/helpers/progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/qgis_utilities/helpers/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/qgis_utilities/helpers/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/qgis_utilities/helpers/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/qgis_utilities/importing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:58:48.665254 Jord-0.0.7/jord/qgis_utilities/numpy_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/qgis_utilities/numpy_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/qgis_utilities/numpy_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/qgis_utilities/numpy_utilities/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/qgis_utilities/numpy_utilities/data_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/qgis_utilities/numpy_utilities/numpy_image_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/qgis_utilities/numpy_utilities/rasters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:58:48.665254 Jord-0.0.7/jord/qgis_utilities/qlive_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/qgis_utilities/qlive_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/qgis_utilities/qlive_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/qgis_utilities/qlive_utilities/procedure_implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/qgis_utilities/qlive_utilities/rpc_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:58:48.665254 Jord-0.0.7/jord/qgis_utilities/shapely_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/qgis_utilities/shapely_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/qgis_utilities/shapely_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/qgis_utilities/shapely_utilities/temp_layer_persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/qgis_utilities/styling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:58:48.669254 Jord-0.0.7/jord/qlive_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/qlive_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/qlive_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/qlive_utilities/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12907 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/qlive_utilities/procedures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/qlive_utilities/serialisation.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/qlive_utilities/uri_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:58:48.669254 Jord-0.0.7/jord/qt_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/qt_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19270 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/qt_utilities/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:58:48.669254 Jord-0.0.7/jord/rasterio_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/rasterio_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/rasterio_utilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:58:48.673254 Jord-0.0.7/jord/shapely_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/shapely_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/shapely_utilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:58:48.673254 Jord-0.0.7/jord/shapely_utilities/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/shapely_utilities/analysis/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/shapely_utilities/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/shapely_utilities/analysis/degrees_of_freedom.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/shapely_utilities/analysis/tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/shapely_utilities/clamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/shapely_utilities/geometry_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/shapely_utilities/iteration.py
--rw-r--r--   0 runner    (1001) docker     (123)    14249 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/shapely_utilities/lines.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/shapely_utilities/mirroring.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/shapely_utilities/morphology.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/shapely_utilities/points.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/shapely_utilities/projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     7780 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/shapely_utilities/sanitise_poly.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:58:48.677254 Jord-0.0.7/jord/shapely_utilities/serialisation/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/shapely_utilities/serialisation/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/shapely_utilities/serialisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/shapely_utilities/serialisation/well_known_binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/shapely_utilities/serialisation/well_known_text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:58:48.677254 Jord-0.0.7/jord/torch_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/torch_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/torch_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-21 08:58:43.000000 Jord-0.0.7/jord/torch_utilities/geodata_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-21 08:58:43.000000 Jord-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-21 08:58:43.000000 Jord-0.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-21 08:58:48.677254 Jord-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-06-21 08:58:43.000000 Jord-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:58:48.677254 Jord-0.0.7/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:58:48.677254 Jord-0.0.7/tests/qgis/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-21 08:58:43.000000 Jord-0.0.7/tests/qgis/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-21 08:58:43.000000 Jord-0.0.7/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-21 08:58:43.000000 Jord-0.0.7/tests/test_sanity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:51:21.486913 Jord-0.0.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:51:21.462913 Jord-0.0.8/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-06-22 13:51:10.000000 Jord-0.0.8/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-22 13:51:10.000000 Jord-0.0.8/.github/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-22 13:51:10.000000 Jord-0.0.8/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:51:10.000000 Jord-0.0.8/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:51:21.466913 Jord-0.0.8/Jord.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-06-22 13:51:21.000000 Jord-0.0.8/Jord.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-06-22 13:51:21.000000 Jord-0.0.8/Jord.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 13:51:21.000000 Jord-0.0.8/Jord.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-22 13:51:21.000000 Jord-0.0.8/Jord.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-22 13:51:21.000000 Jord-0.0.8/Jord.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-22 13:51:10.000000 Jord-0.0.8/KEYWORDS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-06-22 13:51:10.000000 Jord-0.0.8/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-22 13:51:10.000000 Jord-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-06-22 13:51:21.486913 Jord-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-06-22 13:51:10.000000 Jord-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-22 13:51:10.000000 Jord-0.0.8/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:51:21.466913 Jord-0.0.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-22 13:51:10.000000 Jord-0.0.8/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:51:21.466913 Jord-0.0.8/jord/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:51:21.466913 Jord-0.0.8/jord/gdal_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/gdal_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/gdal_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/gdal_utilities/cloning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/gdal_utilities/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/gdal_utilities/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/gdal_utilities/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/gdal_utilities/importing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/gdal_utilities/persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/gdal_utilities/spatial_reference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:51:21.466913 Jord-0.0.8/jord/geojson_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/geojson_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/geojson_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/geojson_utilities/geometry_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:51:21.470913 Jord-0.0.8/jord/geopandas_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/geopandas_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/geopandas_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/geopandas_utilities/geometry_filtering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:51:21.470913 Jord-0.0.8/jord/pillow_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/pillow_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/pillow_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/pillow_utilities/exif.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/pillow_utilities/tiff.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:51:21.470913 Jord-0.0.8/jord/qgis_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/categorisation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:51:21.470913 Jord-0.0.8/jord/qgis_utilities/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/configuration/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/configuration/plugin_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/configuration/project_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:51:21.470913 Jord-0.0.8/jord/qgis_utilities/conversion/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/conversion/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/conversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/conversion/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/data_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/geometry_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:51:21.474913 Jord-0.0.8/jord/qgis_utilities/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/helpers/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/helpers/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/helpers/drawing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/helpers/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/helpers/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/helpers/progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/helpers/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/helpers/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/helpers/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/importing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:51:21.474913 Jord-0.0.8/jord/qgis_utilities/numpy_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/numpy_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/numpy_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/numpy_utilities/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/numpy_utilities/data_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/numpy_utilities/numpy_image_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/numpy_utilities/rasters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:51:21.474913 Jord-0.0.8/jord/qgis_utilities/qlive_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/qlive_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/qlive_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/qlive_utilities/procedure_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/qlive_utilities/rpc_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:51:21.478913 Jord-0.0.8/jord/qgis_utilities/shapely_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/shapely_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/shapely_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/shapely_utilities/temp_layer_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/styling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:51:21.478913 Jord-0.0.8/jord/qlive_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qlive_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qlive_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qlive_utilities/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12907 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qlive_utilities/procedures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qlive_utilities/serialisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qlive_utilities/uri_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:51:21.478913 Jord-0.0.8/jord/qt_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qt_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19270 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qt_utilities/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:51:21.478913 Jord-0.0.8/jord/rasterio_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/rasterio_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/rasterio_utilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:51:21.482913 Jord-0.0.8/jord/shapely_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/shapely_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/shapely_utilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:51:21.482913 Jord-0.0.8/jord/shapely_utilities/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/shapely_utilities/analysis/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/shapely_utilities/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/shapely_utilities/analysis/degrees_of_freedom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/shapely_utilities/analysis/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/shapely_utilities/clamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/shapely_utilities/geometry_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/shapely_utilities/iteration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14249 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/shapely_utilities/lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/shapely_utilities/mirroring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/shapely_utilities/morphology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/shapely_utilities/points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/shapely_utilities/projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7780 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/shapely_utilities/sanitise_poly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:51:21.482913 Jord-0.0.8/jord/shapely_utilities/serialisation/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/shapely_utilities/serialisation/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/shapely_utilities/serialisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/shapely_utilities/serialisation/well_known_binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/shapely_utilities/serialisation/well_known_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/shapely_utilities/transformation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:51:21.482913 Jord-0.0.8/jord/torch_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/torch_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/torch_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/torch_utilities/geodata_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-22 13:51:10.000000 Jord-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-22 13:51:10.000000 Jord-0.0.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-22 13:51:21.486913 Jord-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     9613 2023-06-22 13:51:10.000000 Jord-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:51:21.486913 Jord-0.0.8/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:51:21.486913 Jord-0.0.8/tests/qgis/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-22 13:51:10.000000 Jord-0.0.8/tests/qgis/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-22 13:51:10.000000 Jord-0.0.8/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-22 13:51:10.000000 Jord-0.0.8/tests/test_sanity.py
```

### Comparing `Jord-0.0.7/.github/CODE_OF_CONDUCT.md` & `Jord-0.0.8/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `Jord-0.0.7/.github/CONTRIBUTING.md` & `Jord-0.0.8/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `Jord-0.0.7/Jord.egg-info/PKG-INFO` & `Jord-0.0.8/Jord.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jord
-Version: 0.0.7
+Version: 0.0.8
 Home-page: https://github.com/aivclab/jord
 Download-URL: https://github.com/aivclab/jord/releases
 Author: Christian Heider Nielsen
 Author-email: christian.heider@alexandra.dk
 Maintainer: Christian Heider Nielsen
 Maintainer-email: christian.heider@alexandra.dk
 License: Apache License, Version 2.0
@@ -18,22 +18,22 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: docs
-Provides-Extra: gdal
-Provides-Extra: samples
-Provides-Extra: dev
 Provides-Extra: extra
+Provides-Extra: samples
 Provides-Extra: pil
+Provides-Extra: gdal
+Provides-Extra: dev
 Provides-Extra: tests
 Provides-Extra: setup
+Provides-Extra: docs
 Provides-Extra: all
 License-File: LICENSE.md
 
 <!--![header](.github/images/header.png)-->
 
 <p align="center">
   <img src=".github/images/header.svg" alt='header' />
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: Jord Version: 0.0.7 Home-page: https://github.com/
+Metadata-Version: 2.1 Name: Jord Version: 0.0.8 Home-page: https://github.com/
 aivclab/jord Download-URL: https://github.com/aivclab/jord/releases Author:
 Christian Heider Nielsen Author-email: christian.heider@alexandra.dk
 Maintainer: Christian Heider Nielsen Maintainer-email:
 christian.heider@alexandra.dk License: Apache License, Version 2.0 Keywords:
 python computer vision neo droid Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console Classifier: Intended Audience :: End Users/
 Desktop Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: MacOS ::
 MacOS X Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: POSIX Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Natural Language ::
 English Requires-Python: >=3.6 Description-Content-Type: text/markdown
-Provides-Extra: docs Provides-Extra: gdal Provides-Extra: samples Provides-
-Extra: dev Provides-Extra: extra Provides-Extra: pil Provides-Extra: tests
-Provides-Extra: setup Provides-Extra: all License-File: LICENSE.md
+Provides-Extra: extra Provides-Extra: samples Provides-Extra: pil Provides-
+Extra: gdal Provides-Extra: dev Provides-Extra: tests Provides-Extra: setup
+Provides-Extra: docs Provides-Extra: all License-File: LICENSE.md
                                    [header]
                               ****** Jord ******
  | [![Build Status](https://travis-ci.org/aivclab/jord.svg?branch=master)]
 (https://travis-ci.org/aivclab/jord) | [![Coverage Status](https://
 coveralls.io/repos/github/aivclab/vision/badge.svg?branch=master)](https://
 coveralls.io/github/aivclab/vision?branch=master) | [![GitHub Issues](https://
 img.shields.io/github/issues/aivclab/vision.svg?style=flat)](https://
```

### Comparing `Jord-0.0.7/Jord.egg-info/SOURCES.txt` & `Jord-0.0.8/Jord.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 jord/gdal_utilities/README.md
 jord/gdal_utilities/__init__.py
 jord/gdal_utilities/cloning.py
 jord/gdal_utilities/context.py
 jord/gdal_utilities/conversion.py
 jord/gdal_utilities/enums.py
 jord/gdal_utilities/importing.py
+jord/gdal_utilities/persistence.py
+jord/gdal_utilities/spatial_reference.py
 jord/geojson_utilities/README.md
 jord/geojson_utilities/__init__.py
 jord/geojson_utilities/geometry_types.py
 jord/geopandas_utilities/README.md
 jord/geopandas_utilities/__init__.py
 jord/geopandas_utilities/geometry_filtering.py
 jord/pillow_utilities/README.md
@@ -91,14 +93,15 @@
 jord/shapely_utilities/iteration.py
 jord/shapely_utilities/lines.py
 jord/shapely_utilities/mirroring.py
 jord/shapely_utilities/morphology.py
 jord/shapely_utilities/points.py
 jord/shapely_utilities/projection.py
 jord/shapely_utilities/sanitise_poly.py
+jord/shapely_utilities/transformation.py
 jord/shapely_utilities/analysis/README.md
 jord/shapely_utilities/analysis/__init__.py
 jord/shapely_utilities/analysis/degrees_of_freedom.py
 jord/shapely_utilities/analysis/tracing.py
 jord/shapely_utilities/serialisation/README.md
 jord/shapely_utilities/serialisation/__init__.py
 jord/shapely_utilities/serialisation/well_known_binary.py
```

### Comparing `Jord-0.0.7/Jord.egg-info/requires.txt` & `Jord-0.0.8/Jord.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,58 +1,58 @@
 numpy>=1.20.2
 warg>=1.1.6
 apppath>=1.0.2
 sorcery
 pyzmq
 
 [all]
-warg>=1.1.6
-sorcery
 pip>=22.1.2
+coveralls>=1.6.0
+pytest>=4.3.0
 pytest>=4.4.1
-black[jupyter]>=21.5b0
+pytest-cov>=2.11.1
 sphinx>=4.0.1
-sphinxcontrib-programoutput
-coveralls>=1.6.0
-pre-commit>=2.17.0
-pyzmq
+warg>=1.1.6
 Pillow
-pytest-cov>=2.11.1
-numpy>=1.20.2
 mock
-twine>=1.13.0
-pytest>=4.3.0
+pyzmq
 wheel>=0.33.0
-apppath>=1.0.2
+sphinxcontrib-programoutput
+numpy>=1.20.2
 furo
+twine>=1.13.0
+apppath>=1.0.2
+pre-commit>=2.17.0
+black[jupyter]>=21.5b0
+sorcery
 
 [dev]
-pytest>=4.3.0
-sphinx>=4.0.1
-warg>=1.1.6
-sorcery
-pytest-cov>=2.11.1
-coveralls>=1.6.0
-sphinxcontrib-programoutput
-wheel>=0.33.0
-numpy>=1.20.2
+furo
+twine>=1.13.0
 pip>=22.1.2
 mock
-apppath>=1.0.2
-twine>=1.13.0
+coveralls>=1.6.0
+wheel>=0.33.0
+warg>=1.1.6
+pyzmq
+pytest-cov>=2.11.1
+pytest>=4.3.0
 pytest>=4.4.1
+apppath>=1.0.2
 pre-commit>=2.17.0
-pyzmq
+sphinxcontrib-programoutput
+sorcery
+sphinx>=4.0.1
 black[jupyter]>=21.5b0
-furo
+numpy>=1.20.2
 
 [docs]
+sphinxcontrib-programoutput
 sphinx>=4.0.1
 furo
-sphinxcontrib-programoutput
 
 [extra]
 
 [gdal]
 
 [pil]
 Pillow
```

### Comparing `Jord-0.0.7/LICENSE.md` & `Jord-0.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Jord-0.0.7/PKG-INFO` & `Jord-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jord
-Version: 0.0.7
+Version: 0.0.8
 Home-page: https://github.com/aivclab/jord
 Download-URL: https://github.com/aivclab/jord/releases
 Author: Christian Heider Nielsen
 Author-email: christian.heider@alexandra.dk
 Maintainer: Christian Heider Nielsen
 Maintainer-email: christian.heider@alexandra.dk
 License: Apache License, Version 2.0
@@ -18,22 +18,22 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: docs
-Provides-Extra: gdal
-Provides-Extra: samples
-Provides-Extra: dev
 Provides-Extra: extra
+Provides-Extra: samples
 Provides-Extra: pil
+Provides-Extra: gdal
+Provides-Extra: dev
 Provides-Extra: tests
 Provides-Extra: setup
+Provides-Extra: docs
 Provides-Extra: all
 License-File: LICENSE.md
 
 <!--![header](.github/images/header.png)-->
 
 <p align="center">
   <img src=".github/images/header.svg" alt='header' />
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: Jord Version: 0.0.7 Home-page: https://github.com/
+Metadata-Version: 2.1 Name: Jord Version: 0.0.8 Home-page: https://github.com/
 aivclab/jord Download-URL: https://github.com/aivclab/jord/releases Author:
 Christian Heider Nielsen Author-email: christian.heider@alexandra.dk
 Maintainer: Christian Heider Nielsen Maintainer-email:
 christian.heider@alexandra.dk License: Apache License, Version 2.0 Keywords:
 python computer vision neo droid Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console Classifier: Intended Audience :: End Users/
 Desktop Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: MacOS ::
 MacOS X Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: POSIX Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Natural Language ::
 English Requires-Python: >=3.6 Description-Content-Type: text/markdown
-Provides-Extra: docs Provides-Extra: gdal Provides-Extra: samples Provides-
-Extra: dev Provides-Extra: extra Provides-Extra: pil Provides-Extra: tests
-Provides-Extra: setup Provides-Extra: all License-File: LICENSE.md
+Provides-Extra: extra Provides-Extra: samples Provides-Extra: pil Provides-
+Extra: gdal Provides-Extra: dev Provides-Extra: tests Provides-Extra: setup
+Provides-Extra: docs Provides-Extra: all License-File: LICENSE.md
                                    [header]
                               ****** Jord ******
  | [![Build Status](https://travis-ci.org/aivclab/jord.svg?branch=master)]
 (https://travis-ci.org/aivclab/jord) | [![Coverage Status](https://
 coveralls.io/repos/github/aivclab/vision/badge.svg?branch=master)](https://
 coveralls.io/github/aivclab/vision?branch=master) | [![GitHub Issues](https://
 img.shields.io/github/issues/aivclab/vision.svg?style=flat)](https://
```

### Comparing `Jord-0.0.7/README.md` & `Jord-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `Jord-0.0.7/SECURITY.md` & `Jord-0.0.8/SECURITY.md`

 * *Files identical despite different names*

### Comparing `Jord-0.0.7/jord/__init__.py` & `Jord-0.0.8/jord/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 import pkg_resources
 from apppath import AppPath
 from warg import dist_is_editable
 
 __project__ = "Jord"
 __author__ = "Christian Heider Nielsen"
-__version__ = "0.0.7"
+__version__ = "0.0.8"
 __doc__ = r"""
 .. module:: jord
    :platform: Unix, Windows
    :synopsis: A set of general tools build for geo data.
 
 .. moduleauthor:: Christian Heider Nielsen <christian.heider@alexandra.dk>
```

### Comparing `Jord-0.0.7/jord/gdal_utilities/__init__.py` & `Jord-0.0.8/jord/gdal_utilities/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,11 +14,13 @@
 
 try:
     from .conversion import *
     from .enums import *
     from .importing import *
     from .context import *
     from .cloning import *
+    from .persistence import *
+    from .spatial_reference import *
 except ImportError as ix:
     this_package_name = Path(__file__).parent.name
     print(f"Make sure gdal module is available for {this_package_name}")
     raise ix
```

### Comparing `Jord-0.0.7/jord/gdal_utilities/cloning.py` & `Jord-0.0.8/jord/gdal_utilities/cloning.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.7/jord/gdal_utilities/context.py` & `Jord-0.0.8/jord/gdal_utilities/context.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.7/jord/gdal_utilities/conversion.py` & `Jord-0.0.8/jord/gdal_utilities/conversion.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.7/jord/gdal_utilities/importing.py` & `Jord-0.0.8/jord/gdal_utilities/importing.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.7/jord/geojson_utilities/geometry_types.py` & `Jord-0.0.8/jord/geojson_utilities/geometry_types.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.7/jord/geopandas_utilities/geometry_filtering.py` & `Jord-0.0.8/jord/geopandas_utilities/geometry_filtering.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.7/jord/qgis_utilities/__init__.py` & `Jord-0.0.8/jord/qgis_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.7/jord/qgis_utilities/categorisation.py` & `Jord-0.0.8/jord/qgis_utilities/categorisation.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.7/jord/qgis_utilities/configuration/plugin_settings.py` & `Jord-0.0.8/jord/qgis_utilities/configuration/plugin_settings.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.7/jord/qgis_utilities/configuration/project_settings.py` & `Jord-0.0.8/jord/qgis_utilities/configuration/project_settings.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.7/jord/qgis_utilities/enums.py` & `Jord-0.0.8/jord/qgis_utilities/enums.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.7/jord/qgis_utilities/geometry_types.py` & `Jord-0.0.8/jord/qgis_utilities/geometry_types.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.7/jord/qgis_utilities/helpers/actions.py` & `Jord-0.0.8/jord/qgis_utilities/helpers/actions.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.7/jord/qgis_utilities/helpers/drawing.py` & `Jord-0.0.8/jord/qgis_utilities/helpers/drawing.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.7/jord/qgis_utilities/helpers/environment.py` & `Jord-0.0.8/jord/qgis_utilities/helpers/environment.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.7/jord/qgis_utilities/helpers/models.py` & `Jord-0.0.8/jord/qgis_utilities/helpers/models.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.7/jord/qgis_utilities/helpers/progress_bar.py` & `Jord-0.0.8/jord/qgis_utilities/helpers/progress_bar.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.7/jord/qgis_utilities/helpers/signals.py` & `Jord-0.0.8/jord/qgis_utilities/helpers/signals.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.7/jord/qgis_utilities/helpers/timestamp.py` & `Jord-0.0.8/jord/qgis_utilities/helpers/timestamp.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.7/jord/qgis_utilities/numpy_utilities/conversion.py` & `Jord-0.0.8/jord/qgis_utilities/numpy_utilities/conversion.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.7/jord/qgis_utilities/numpy_utilities/data_type.py` & `Jord-0.0.8/jord/qgis_utilities/numpy_utilities/data_type.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.7/jord/qgis_utilities/numpy_utilities/numpy_image_widget.py` & `Jord-0.0.8/jord/qgis_utilities/numpy_utilities/numpy_image_widget.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.7/jord/qgis_utilities/shapely_utilities/temp_layer_persistence.py` & `Jord-0.0.8/jord/qgis_utilities/shapely_utilities/temp_layer_persistence.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.7/jord/qgis_utilities/styling.py` & `Jord-0.0.8/jord/qgis_utilities/styling.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.7/jord/qlive_utilities/client.py` & `Jord-0.0.8/jord/qlive_utilities/client.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.7/jord/qlive_utilities/procedures.py` & `Jord-0.0.8/jord/qlive_utilities/procedures.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.7/jord/qlive_utilities/serialisation.py` & `Jord-0.0.8/jord/qlive_utilities/serialisation.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.7/jord/qlive_utilities/uri_utilities.py` & `Jord-0.0.8/jord/qlive_utilities/uri_utilities.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.7/jord/qt_utilities/enums.py` & `Jord-0.0.8/jord/qt_utilities/enums.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.7/jord/shapely_utilities/__init__.py` & `Jord-0.0.8/jord/shapely_utilities/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,7 +18,8 @@
 from .morphology import *
 from .points import *
 from .sanitise_poly import *
 from .serialisation import *
 from .geometry_types import *
 from .iteration import *
 from .projection import *
+from .transformation import *
```

### Comparing `Jord-0.0.7/jord/shapely_utilities/clamp.py` & `Jord-0.0.8/jord/shapely_utilities/clamp.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.7/jord/shapely_utilities/geometry_types.py` & `Jord-0.0.8/jord/shapely_utilities/geometry_types.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.7/jord/shapely_utilities/iteration.py` & `Jord-0.0.8/jord/shapely_utilities/iteration.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.7/jord/shapely_utilities/lines.py` & `Jord-0.0.8/jord/shapely_utilities/lines.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.7/jord/shapely_utilities/mirroring.py` & `Jord-0.0.8/jord/shapely_utilities/mirroring.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.7/jord/shapely_utilities/morphology.py` & `Jord-0.0.8/jord/shapely_utilities/morphology.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.7/jord/shapely_utilities/points.py` & `Jord-0.0.8/jord/shapely_utilities/points.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.7/jord/shapely_utilities/projection.py` & `Jord-0.0.8/jord/shapely_utilities/projection.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.7/jord/shapely_utilities/sanitise_poly.py` & `Jord-0.0.8/jord/shapely_utilities/sanitise_poly.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.7/jord/shapely_utilities/serialisation/well_known_binary.py` & `Jord-0.0.8/jord/shapely_utilities/serialisation/well_known_binary.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.7/jord/shapely_utilities/serialisation/well_known_text.py` & `Jord-0.0.8/jord/shapely_utilities/serialisation/well_known_text.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.7/setup.py` & `Jord-0.0.8/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -344,7 +344,48 @@
         long_description_content_type=pkg.readme_type,
         long_description=pkg.readme,
         tests_require=pkg.test_dependencies,
         setup_requires=pkg.setup_dependencies,
         include_package_data=True,
         python_requires=">=3.6",
     )
+
+    """
+    name: str = ...,
+          version: str = ...,
+          description: str = ...,
+          long_description: str = ...,
+          author: str = ...,
+          author_email: str = ...,
+          maintainer: str = ...,
+          maintainer_email: str = ...,
+          url: str = ...,
+          download_url: str = ...,
+          packages: list[str] = ...,
+          py_modules: list[str] = ...,
+          scripts: list[str] = ...,
+          ext_modules: list[Extension] = ...,
+          classifiers: list[str] = ...,
+          distclass: Type[Distribution] = ...,
+          script_name: str = ...,
+          script_args: list[str] = ...,
+          options: Mapping[str, Any] = ...,
+          license: str = ...,
+          keywords: list[str] | str = ...,
+          platforms: list[str] | str = ...,
+          cmdclass: Mapping[str, Type[Command]] = ...,
+          data_files: list[tuple[str, list[str]]] = ...,
+          package_dir: Mapping[str, str] = ...,
+          obsoletes: list[str] = ...,
+          provides: list[str] = ...,
+          requires: list[str] = ...,
+          command_packages: list[str] = ...,
+          command_options: Mapping[str, Mapping[str, tuple[Any, Any]]] = ...,
+          package_data: Mapping[str, list[str]] = ...,
+          include_package_data: bool = ...,
+          libraries: list[str] = ...,
+          headers: list[str] = ...,
+          ext_package: str = ...,
+          include_dirs: list[str] = ...,
+          password: str = ...,
+          fullname: str = ...,
+    """
```

### Comparing `Jord-0.0.7/tests/test_import.py` & `Jord-0.0.8/tests/test_import.py`

 * *Files identical despite different names*

