# Comparing `tmp/ocsmesh-1.3.3.tar.gz` & `tmp/ocsmesh-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocsmesh-1.3.3.tar", last modified: Tue Jun 20 14:25:19 2023, max compression
+gzip compressed data, was "ocsmesh-1.3.4.tar", last modified: Thu Jun 22 19:24:45 2023, max compression
```

## Comparing `ocsmesh-1.3.3.tar` & `ocsmesh-1.3.4.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:19.101632 ocsmesh-1.3.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:19.085631 ocsmesh-1.3.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:19.089631 ocsmesh-1.3.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/.github/workflows/documentation.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/.github/workflows/functional_test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/.github/workflows/functional_test_2.yml
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/.github/workflows/pylint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10967 2023-06-20 14:25:19.101632 ocsmesh-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:19.089631 ocsmesh-1.3.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)  2851126 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/docs/noaa_33879_DS1.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:19.093632 ocsmesh-1.3.3/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/docs/source/ocsmesh.command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/docs/source/ocsmesh.geometry.rst
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/docs/source/ocsmesh.mesh.rst
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/docs/source/ocsmesh.size_function.rst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/docs/source/ocsmesh.utilities.rst
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/docs/source/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:19.093632 ocsmesh-1.3.3/ocsmesh/
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:19.093632 ocsmesh-1.3.3/ocsmesh/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/cli/mesh_upgrader.py
--rw-r--r--   0 runner    (1001) docker     (123)    13271 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/cli/remesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    11179 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/cli/remesh_by_shape_factor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23645 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/cli/subset_n_combine.py
--rw-r--r--   0 runner    (1001) docker     (123)    17544 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/crs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:19.097632 ocsmesh-1.3.3/ocsmesh/features/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/features/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)    11129 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/features/constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/features/contour.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/features/linefeature.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/features/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/figures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:19.097632 ocsmesh-1.3.3/ocsmesh/geom/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/geom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/geom/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    26034 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/geom/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/geom/geom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/geom/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/geom/raster.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/geom/shapely.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:19.097632 ocsmesh-1.3.3/ocsmesh/hfun/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/hfun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/hfun/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    81400 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/hfun/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/hfun/hfun.py
--rw-r--r--   0 runner    (1001) docker     (123)    22004 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/hfun/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    59651 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/hfun/raster.py
--rw-r--r--   0 runner    (1001) docker     (123)    15388 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/interp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:19.097632 ocsmesh-1.3.3/ocsmesh/mesh/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/mesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/mesh/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    74313 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/mesh/mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:19.097632 ocsmesh-1.3.3/ocsmesh/mesh/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/mesh/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7362 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/mesh/parsers/grd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/mesh/parsers/sms2dm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:19.097632 ocsmesh-1.3.3/ocsmesh/ops/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21111 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/ops/combine_geom.py
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/ops/combine_hfun.py
--rw-r--r--   0 runner    (1001) docker     (123)    64799 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/raster.py
--rw-r--r--   0 runner    (1001) docker     (123)    68014 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/ocsmesh/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:19.093632 ocsmesh-1.3.3/ocsmesh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10967 2023-06-20 14:25:19.000000 ocsmesh-1.3.3/ocsmesh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-06-20 14:25:19.000000 ocsmesh-1.3.3/ocsmesh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 14:25:19.000000 ocsmesh-1.3.3/ocsmesh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-20 14:25:19.000000 ocsmesh-1.3.3/ocsmesh.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-20 14:25:19.000000 ocsmesh-1.3.3/ocsmesh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-20 14:25:19.000000 ocsmesh-1.3.3/ocsmesh.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 14:25:19.101632 ocsmesh-1.3.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3046 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:19.085631 ocsmesh-1.3.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:19.101632 ocsmesh-1.3.3/tests/api/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/tests/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/tests/api/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/tests/api/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    13728 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/tests/api/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     7931 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/tests/api/geom.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    30865 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/tests/api/hfun.py
--rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/tests/api/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    16260 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/tests/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:19.101632 ocsmesh-1.3.3/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/tests/cli/build_geom.sh
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/tests/cli/build_hfun.sh
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-20 14:25:05.000000 ocsmesh-1.3.3/tests/cli/remesh_by_dem.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:24:45.394126 ocsmesh-1.3.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:24:45.374125 ocsmesh-1.3.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:24:45.378125 ocsmesh-1.3.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/.github/workflows/documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/.github/workflows/functional_test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/.github/workflows/functional_test_2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/.github/workflows/pylint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10967 2023-06-22 19:24:45.394126 ocsmesh-1.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:24:45.378125 ocsmesh-1.3.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)  2851126 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/docs/noaa_33879_DS1.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:24:45.382125 ocsmesh-1.3.4/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/docs/source/ocsmesh.command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/docs/source/ocsmesh.geometry.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/docs/source/ocsmesh.mesh.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/docs/source/ocsmesh.size_function.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/docs/source/ocsmesh.utilities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/docs/source/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:24:45.386125 ocsmesh-1.3.4/ocsmesh/
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:24:45.386125 ocsmesh-1.3.4/ocsmesh/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/cli/mesh_upgrader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13271 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/cli/remesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11179 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/cli/remesh_by_shape_factor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23645 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/cli/subset_n_combine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17544 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/crs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:24:45.390125 ocsmesh-1.3.4/ocsmesh/features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/features/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11129 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/features/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/features/contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/features/linefeature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/features/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/figures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:24:45.390125 ocsmesh-1.3.4/ocsmesh/geom/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/geom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/geom/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26034 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/geom/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/geom/geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/geom/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/geom/raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/geom/shapely.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:24:45.390125 ocsmesh-1.3.4/ocsmesh/hfun/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/hfun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/hfun/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81400 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/hfun/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/hfun/hfun.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22004 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/hfun/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59651 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/hfun/raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15388 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/interp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:24:45.390125 ocsmesh-1.3.4/ocsmesh/mesh/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/mesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/mesh/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74313 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/mesh/mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:24:45.390125 ocsmesh-1.3.4/ocsmesh/mesh/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/mesh/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7362 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/mesh/parsers/grd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/mesh/parsers/sms2dm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:24:45.390125 ocsmesh-1.3.4/ocsmesh/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21111 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/ops/combine_geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/ops/combine_hfun.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64867 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68014 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/ocsmesh/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:24:45.386125 ocsmesh-1.3.4/ocsmesh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10967 2023-06-22 19:24:45.000000 ocsmesh-1.3.4/ocsmesh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-06-22 19:24:45.000000 ocsmesh-1.3.4/ocsmesh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 19:24:45.000000 ocsmesh-1.3.4/ocsmesh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-22 19:24:45.000000 ocsmesh-1.3.4/ocsmesh.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-22 19:24:45.000000 ocsmesh-1.3.4/ocsmesh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-22 19:24:45.000000 ocsmesh-1.3.4/ocsmesh.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 19:24:45.394126 ocsmesh-1.3.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3082 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:24:45.378125 ocsmesh-1.3.4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:24:45.394126 ocsmesh-1.3.4/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/tests/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/tests/api/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/tests/api/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13728 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/tests/api/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7931 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/tests/api/geom.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31570 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/tests/api/hfun.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/tests/api/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17159 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/tests/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:24:45.394126 ocsmesh-1.3.4/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/tests/cli/build_geom.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/tests/cli/build_hfun.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-22 19:24:30.000000 ocsmesh-1.3.4/tests/cli/remesh_by_dem.sh
```

### Comparing `ocsmesh-1.3.3/.github/workflows/documentation.yml` & `ocsmesh-1.3.4/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.3/.github/workflows/functional_test.yml` & `ocsmesh-1.3.4/.github/workflows/functional_test.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,26 @@
 name: Functional
 
-on: [push]
+on:
+  push:
+    branches:
+      - 'main'
+    paths:
+      - '**.py'
+      - '.github/workflows/*.yml'
+      - 'pyproject.toml'
+      - 'setup.py'
+      - 'setup.cfg'
+  pull_request:
+    paths:
+      - '**.py'
+      - '.github/workflows/*.yml'
+      - 'pyproject.toml'
+      - 'setup.py'
+      - 'setup.cfg'
 
 jobs:
   basic-functional-tests:
 
     name: Python ${{ matrix.python-version }} on ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
```

### Comparing `ocsmesh-1.3.3/.github/workflows/functional_test_2.yml` & `ocsmesh-1.3.4/.github/workflows/functional_test_2.yml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,26 @@
 name: Functional (pip)
 
-on: [push]
+on:
+  push:
+    branches:
+      - 'main'
+    paths:
+      - '**.py'
+      - '.github/workflows/*.yml'
+      - 'pyproject.toml'
+      - 'setup.py'
+      - 'setup.cfg'
+  pull_request:
+    paths:
+      - '**.py'
+      - '.github/workflows/*.yml'
+      - 'pyproject.toml'
+      - 'setup.py'
+      - 'setup.cfg'
 
 jobs:
   basic-functional-tests-using-pip:
 
     name: Python ${{ matrix.python-version }} on ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
```

### Comparing `ocsmesh-1.3.3/.github/workflows/release.yml` & `ocsmesh-1.3.4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.3/.gitignore` & `ocsmesh-1.3.4/.gitignore`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.3/.pylintrc` & `ocsmesh-1.3.4/.pylintrc`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.3/LICENSE` & `ocsmesh-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.3/PKG-INFO` & `ocsmesh-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocsmesh
-Version: 1.3.3
+Version: 1.3.4
 Summary: Package to generate computational unstructured meshes from planetary modeling.
 Author-email: Jaime R Calzada <jreniel@gmail.com>, Soroosh Mani <soroosh.mani@noaa.gov>
 Maintainer-email: Soroosh Mani <soroosh.mani@noaa.gov>
 License: Creative Commons Legal Code
         
         CC0 1.0 Universal
```

### Comparing `ocsmesh-1.3.3/README.md` & `ocsmesh-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.3/docs/Makefile` & `ocsmesh-1.3.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.3/docs/make.bat` & `ocsmesh-1.3.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.3/docs/noaa_33879_DS1.pdf` & `ocsmesh-1.3.4/docs/noaa_33879_DS1.pdf`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.3/docs/source/conf.py` & `ocsmesh-1.3.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.3/ocsmesh/__init__.py` & `ocsmesh-1.3.4/ocsmesh/__init__.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.3/ocsmesh/__main__.py` & `ocsmesh-1.3.4/ocsmesh/__main__.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.3/ocsmesh/cli/cli.py` & `ocsmesh-1.3.4/ocsmesh/cli/cli.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.3/ocsmesh/cli/mesh_upgrader.py` & `ocsmesh-1.3.4/ocsmesh/cli/mesh_upgrader.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.3/ocsmesh/cli/remesh.py` & `ocsmesh-1.3.4/ocsmesh/cli/remesh.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.3/ocsmesh/cli/remesh_by_shape_factor.py` & `ocsmesh-1.3.4/ocsmesh/cli/remesh_by_shape_factor.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.3/ocsmesh/cli/subset_n_combine.py` & `ocsmesh-1.3.4/ocsmesh/cli/subset_n_combine.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.3/ocsmesh/cmd.py` & `ocsmesh-1.3.4/ocsmesh/cmd.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.3/ocsmesh/db.py` & `ocsmesh-1.3.4/ocsmesh/db.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.3/ocsmesh/driver.py` & `ocsmesh-1.3.4/ocsmesh/driver.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.3/ocsmesh/features/channel.py` & `ocsmesh-1.3.4/ocsmesh/features/channel.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.3/ocsmesh/features/constraint.py` & `ocsmesh-1.3.4/ocsmesh/features/constraint.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.3/ocsmesh/features/contour.py` & `ocsmesh-1.3.4/ocsmesh/features/contour.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.3/ocsmesh/features/linefeature.py` & `ocsmesh-1.3.4/ocsmesh/features/linefeature.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.3/ocsmesh/features/patch.py` & `ocsmesh-1.3.4/ocsmesh/features/patch.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.3/ocsmesh/figures.py` & `ocsmesh-1.3.4/ocsmesh/figures.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.3/ocsmesh/geom/base.py` & `ocsmesh-1.3.4/ocsmesh/geom/base.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.3/ocsmesh/geom/collector.py` & `ocsmesh-1.3.4/ocsmesh/geom/collector.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.3/ocsmesh/geom/geom.py` & `ocsmesh-1.3.4/ocsmesh/geom/geom.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.3/ocsmesh/geom/mesh.py` & `ocsmesh-1.3.4/ocsmesh/geom/mesh.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.3/ocsmesh/geom/raster.py` & `ocsmesh-1.3.4/ocsmesh/geom/raster.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.3/ocsmesh/geom/shapely.py` & `ocsmesh-1.3.4/ocsmesh/geom/shapely.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.3/ocsmesh/hfun/base.py` & `ocsmesh-1.3.4/ocsmesh/hfun/base.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.3/ocsmesh/hfun/collector.py` & `ocsmesh-1.3.4/ocsmesh/hfun/collector.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.3/ocsmesh/hfun/hfun.py` & `ocsmesh-1.3.4/ocsmesh/hfun/hfun.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.3/ocsmesh/hfun/mesh.py` & `ocsmesh-1.3.4/ocsmesh/hfun/mesh.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.3/ocsmesh/hfun/raster.py` & `ocsmesh-1.3.4/ocsmesh/hfun/raster.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.3/ocsmesh/interp.py` & `ocsmesh-1.3.4/ocsmesh/interp.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.3/ocsmesh/mesh/base.py` & `ocsmesh-1.3.4/ocsmesh/mesh/base.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.3/ocsmesh/mesh/mesh.py` & `ocsmesh-1.3.4/ocsmesh/mesh/mesh.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.3/ocsmesh/mesh/parsers/grd.py` & `ocsmesh-1.3.4/ocsmesh/mesh/parsers/grd.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.3/ocsmesh/mesh/parsers/sms2dm.py` & `ocsmesh-1.3.4/ocsmesh/mesh/parsers/sms2dm.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.3/ocsmesh/ops/combine_geom.py` & `ocsmesh-1.3.4/ocsmesh/ops/combine_geom.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.3/ocsmesh/ops/combine_hfun.py` & `ocsmesh-1.3.4/ocsmesh/ops/combine_hfun.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.3/ocsmesh/raster.py` & `ocsmesh-1.3.4/ocsmesh/raster.py`

 * *Files 0% similar despite different names*

```diff
@@ -1421,18 +1421,20 @@
             start = time()
             fig, ax = plt.subplots()
             ax.contour(x, y, values, levels=[level])
             _logger.debug(f'Took {time()-start}...')
             plt.close(fig)
         for path_collection in ax.collections:
             for path in path_collection.get_paths():
+                # LineStrings must have at least 2 coordinate tuples
+                if len(path.vertices) < 2:
+                    continue
                 try:
                     features.append(LineString(path.vertices))
                 except ValueError:
-                    # LineStrings must have at least 2 coordinate tuples
                     pass
         return ops.linemerge(features)
 
     def _get_raster_contour_feathered(
             self,
             level : float,
             iter_windows : Iterable[windows.Window]
```

### Comparing `ocsmesh-1.3.3/ocsmesh/utils.py` & `ocsmesh-1.3.4/ocsmesh/utils.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.3/ocsmesh.egg-info/PKG-INFO` & `ocsmesh-1.3.4/ocsmesh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocsmesh
-Version: 1.3.3
+Version: 1.3.4
 Summary: Package to generate computational unstructured meshes from planetary modeling.
 Author-email: Jaime R Calzada <jreniel@gmail.com>, Soroosh Mani <soroosh.mani@noaa.gov>
 Maintainer-email: Soroosh Mani <soroosh.mani@noaa.gov>
 License: Creative Commons Legal Code
         
         CC0 1.0 Universal
```

### Comparing `ocsmesh-1.3.3/ocsmesh.egg-info/SOURCES.txt` & `ocsmesh-1.3.4/ocsmesh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.3/pyproject.toml` & `ocsmesh-1.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.3/setup.py` & `ocsmesh-1.3.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 import setuptools
 import subprocess
 import distutils.cmd
 import shutil
 import platform
 from multiprocessing import cpu_count
 from pathlib import Path
+import site
 import sys
 import os
+import re
 
 PARENT = Path(__file__).parent.absolute()
-PYENV_PREFIX = Path("/".join(sys.executable.split('/')[:-2]))
+PYENV_PREFIX = Path(site.PREFIXES[0])
 SYSLIB = {
     "Windows": "jigsaw.dll",
     "Linux": "libjigsaw.so",
     "Darwin": "libjigsaw.dylib"}
 
 if "install_jigsaw" not in sys.argv:
     if "develop" not in sys.argv:
@@ -62,28 +64,27 @@
              ])
         subprocess.check_call(["make", f"-j{cpu_count()}", "install"])
         libsaw_prefix = list(PYENV_PREFIX.glob("**/*jigsawpy*")).pop() / '_lib'
         os.makedirs(libsaw_prefix, exist_ok=True)
         envlib = PYENV_PREFIX / 'lib' / SYSLIB[platform.system()]
         os.symlink(envlib, libsaw_prefix / envlib.name)
         os.chdir(PARENT)
-        subprocess.check_call(
-          ["git", "submodule", "deinit", "-f", "submodules/jigsaw-python"])
+        subprocess.check_call(["git", "submodule", "deinit", "-f", "submodules/jigsaw-python"])
 
     def _check_gcc_version(self):
         cpp = shutil.which("c++")
-        major, minor, patch = subprocess.check_output(
-            [cpp, "--version"]
-            ).decode('utf-8').split('\n')[0].split()[-1].split('.')
+        line = subprocess.check_output([cpp, "--version"]).decode('utf-8').split('\n')[0]
+        m = re.search('(\d+\.)(\d+\.)(\d+)', line)
+        major, minor, patch = line[m.start(): m.end()].split('.')
         current_version = float(f"{major}.{minor}")
         if current_version < 7.:
             raise Exception(
                 'JIGSAW requires GCC version 7 or later, got '
                 f'{major}.{minor}.{patch} from {cpp}')
         return shutil.which("gcc"), cpp
 
 
 setuptools.setup(
     cmdclass={
         'install_jigsaw': InstallJigsawCommand,
-        },
+    },
 )
```

### Comparing `ocsmesh-1.3.3/tests/api/common.py` & `ocsmesh-1.3.4/tests/api/common.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.3/tests/api/driver.py` & `ocsmesh-1.3.4/tests/api/driver.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.3/tests/api/features.py` & `ocsmesh-1.3.4/tests/api/features.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.3/tests/api/geom.py` & `ocsmesh-1.3.4/tests/api/geom.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.3/tests/api/hfun.py` & `ocsmesh-1.3.4/tests/api/hfun.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 import shutil
 import tempfile
 import warnings
 
 from jigsawpy import jigsaw_msh_t
 import geopandas as gpd
 import numpy as np
-import rasterio as rio
-import requests
 from shapely import geometry
 
 import ocsmesh
 
 from tests.api.common import (
     topo_2rast_1mesh,
 )
@@ -77,18 +75,17 @@
     # all the other types as it is currently calling all the underlying
     # size functions to apply each feature or constraint in "exact" mode
 
     def setUp(self):
         self.tdir = Path(tempfile.mkdtemp())
         self.rast1 = self.tdir / 'rast_1.tif'
         self.rast2 = self.tdir / 'rast_2.tif'
-        self.mesh1 = self.tdir / 'mesh_1.gr3'
+        self.mesh1 = self.tdir / 'mesh_1.grd'
         topo_2rast_1mesh(self.rast1, self.rast2, self.mesh1)
 
-
     def tearDown(self):
         shutil.rmtree(self.tdir)
 
     def test_multi_path_input(self):
         hfun_coll = ocsmesh.Hfun(
             [self.rast1, self.rast2, self.mesh1],
             hmin=500,
@@ -172,15 +169,15 @@
             value_type='min',
         )
 
         hfun_msht = hfun_coll.msh_t()
         
         self.assertTrue(isinstance(hfun_msht, jigsaw_msh_t))
 
-    def test_add_contor_exact(self):
+    def test_add_contour_exact(self):
         # TODO: Improve this test (added for upgrade to shapely2)
         hfun_coll = ocsmesh.Hfun(
             [self.rast1, self.rast2, self.mesh1],
             hmin=500,
             hmax=5000,
             method='exact'
         )
@@ -189,14 +186,42 @@
             target_size=1000,
             )
 
         hfun_msht = hfun_coll.msh_t()
         
         self.assertTrue(isinstance(hfun_msht, jigsaw_msh_t))
 
+
+    def test_add_contour_single_vertex(self):
+        rast3 = self.tdir / 'rast_3.tif'
+        rast_xy_3 = np.mgrid[-1:0.1:0.1, -0.7:0.1:0.1]
+        rast_z_3 = np.ones_like(rast_xy_3[0]) * 2.0
+        rast_z_3[0, 0] = 1
+        rast_z_3[-1, -1] = 3
+
+        ocsmesh.utils.raster_from_numpy(
+            rast3, rast_z_3, rast_xy_3, 4326
+        )
+
+        # regression test for single point contours
+        hfun_coll = ocsmesh.Hfun(
+            [rast3],
+            hmin=500,
+            hmax=5000,
+            method='exact'
+        )
+        hfun_coll.add_contour(
+            level=1,
+            target_size=1000,
+            )
+
+        hfun_msht = hfun_coll.msh_t()
+        
+        self.assertTrue(isinstance(hfun_msht, jigsaw_msh_t))
+
 
     def test_add_channel_exact(self):
         # TODO: Improve this test (added for upgrade to shapely2)
         hfun_coll = ocsmesh.Hfun(
             [self.rast1, self.rast2, self.mesh1],
             hmin=500,
             hmax=5000,
```

### Comparing `ocsmesh-1.3.3/tests/api/mesh.py` & `ocsmesh-1.3.4/tests/api/mesh.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.3/tests/api/utils.py` & `ocsmesh-1.3.4/tests/api/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,26 +2,49 @@
 import unittest
 import tempfile
 from copy import deepcopy
 
 import numpy as np
 from jigsawpy import jigsaw_msh_t
 from pyproj import CRS
+import re
 from shapely.geometry import (
     Point,
     LineString,
     box,
     Polygon,
     MultiPolygon,
     GeometryCollection,
 )
 
 from ocsmesh import Raster, utils
 
 
+class SetUp(unittest.TestCase):
+
+    def test_cpp_version_parsing(self):
+        # inline copy of code in setup.py.
+        def _cpp_version(line):
+            m = re.search('(\d+\.)(\d+\.)(\d+)', line)
+            return line[m.start(): m.end()].split('.')
+
+        _test_data = [
+            ('c++ (GCC) 11.3.1 20221121 (Red Hat 11.3.1-4)', '11', '3', '1'),
+            ('c++ (GCC) 7.3.1 20180712 (Red Hat 7.3.1-15)', '7', '3', '1'),
+            ('Apple clang version 12.0.0 (clang-1200.0.32.29)', '12', '0', '0'),
+            ('Apple clang version 14.0.3 (clang-1403.0.22.14.1)', '14', '0', '3'),
+            ('cpp (MacPorts gcc12 12.2.0_2+stdlib_flag) 12.2.0', '12', '2', '0')
+        ]
+        for line in _test_data:
+            major, minor, patch = _cpp_version(line[0])
+            assert major == line[1]
+            assert minor == line[2]
+            assert patch == line[3]
+
+
 class FinalizeMesh(unittest.TestCase):
 
     def test_cleanup_mesh_and_generate_valid_mesh(self):
         msh_t1 = utils.create_rectangle_mesh(
             nx=40, ny=40,
             holes=[50, 51],
             quads=np.hstack((
```

