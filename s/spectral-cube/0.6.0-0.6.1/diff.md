# Comparing `tmp/spectral-cube-0.6.0.tar.gz` & `tmp/spectral-cube-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectral-cube-0.6.0.tar", last modified: Thu Sep 30 16:04:24 2021, max compression
+gzip compressed data, was "spectral-cube-0.6.1.tar", last modified: Thu Jun 22 19:58:09 2023, max compression
```

## Comparing `spectral-cube-0.6.0.tar` & `spectral-cube-0.6.1.tar`

### file list

```diff
@@ -1,168 +1,174 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 16:04:24.745030 spectral-cube-0.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 16:04:24.721030 spectral-cube-0.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 16:04:24.725030 spectral-cube-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2622 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (121)      983 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)      624 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      175 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)    14152 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1494 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (121)      316 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2161 2021-09-30 16:04:24.745030 spectral-cube-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1718 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 16:04:24.729030 spectral-cube-0.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     6786 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 16:04:24.721030 spectral-cube-0.6.0/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 16:04:24.729030 spectral-cube-0.6.0/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (121)       42 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/docs/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (121)       43 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (121)       44 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/docs/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2944 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/docs/accessing.rst
--rw-r--r--   0 runner    (1001) docker     (121)      701 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      959 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/docs/arithmetic.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3004 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/docs/beam_handling.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5621 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/docs/big_data.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7218 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     2166 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/docs/continuum_subtraction.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3091 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/docs/creating_reading.rst
--rw-r--r--   0 runner    (1001) docker     (121)    17879 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/docs/dask.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5064 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/docs/errors.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6633 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3006 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3384 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7672 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/docs/manipulating.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8707 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/docs/masking.rst
--rw-r--r--   0 runner    (1001) docker     (121)      999 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/docs/metadata.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6895 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/docs/moments.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1280 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/docs/nitpick-exceptions
--rw-r--r--   0 runner    (1001) docker     (121)      631 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/docs/quick_looks.rst
--rw-r--r--   0 runner    (1001) docker     (121)      215 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/docs/rtd-pip-requirements
--rw-r--r--   0 runner    (1001) docker     (121)     7109 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/docs/smoothing.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3275 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/docs/spectral_extraction.rst
--rw-r--r--   0 runner    (1001) docker     (121)      258 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/docs/stokes.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1815 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/docs/visualization.rst
--rw-r--r--   0 runner    (1001) docker     (121)      256 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/docs/writing.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6824 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/docs/yt_example.rst
--rw-r--r--   0 runner    (1001) docker     (121)      132 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     2004 2021-09-30 16:04:24.749030 spectral-cube-0.6.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     1102 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 16:04:24.733030 spectral-cube-0.6.0/spectral_cube/
--rw-r--r--   0 runner    (1001) docker     (121)     1147 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1491 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/_astropy_init.py
--rw-r--r--   0 runner    (1001) docker     (121)     4789 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/_moments.py
--rw-r--r--   0 runner    (1001) docker     (121)    13241 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/analysis_utilities.py
--rw-r--r--   0 runner    (1001) docker     (121)    29830 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/base_class.py
--rw-r--r--   0 runner    (1001) docker     (121)    17148 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)    24471 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/cube_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    63167 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/dask_spectral_cube.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 16:04:24.737030 spectral-cube-0.6.0/spectral_cube/io/
--rw-r--r--   0 runner    (1001) docker     (121)       65 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8831 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/io/casa_image.py
--rw-r--r--   0 runner    (1001) docker     (121)     3685 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/io/casa_masks.py
--rw-r--r--   0 runner    (1001) docker     (121)    29674 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/io/class_lmv.py
--rw-r--r--   0 runner    (1001) docker     (121)     7086 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/io/core.py
--rw-r--r--   0 runner    (1001) docker     (121)    11232 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/io/fits.py
--rw-r--r--   0 runner    (1001) docker     (121)    40798 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/lower_dimensional_structures.py
--rw-r--r--   0 runner    (1001) docker     (121)    30770 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/masks.py
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/np_compat.py
--rw-r--r--   0 runner    (1001) docker     (121)    18043 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/spectral_axis.py
--rw-r--r--   0 runner    (1001) docker     (121)   166748 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/spectral_cube.py
--rw-r--r--   0 runner    (1001) docker     (121)     5893 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/stokes_spectral_cube.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 16:04:24.737030 spectral-cube-0.6.0/spectral_cube/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      167 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 16:04:24.741030 spectral-cube-0.6.0/spectral_cube/tests/data/
--rw-r--r--   0 runner    (1001) docker     (121)      233 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/data/255-fk5.reg
--rw-r--r--   0 runner    (1001) docker     (121)      232 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/data/255-pixel.reg
--rw-r--r--   0 runner    (1001) docker     (121)      128 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/data/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 16:04:24.741030 spectral-cube-0.6.0/spectral_cube/tests/data/basic.image/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 16:04:24.741030 spectral-cube-0.6.0/spectral_cube/tests/data/basic.image/logtable/
--rw-r--r--   0 runner    (1001) docker     (121)     1392 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/data/basic.image/logtable/table.dat
--rw-r--r--   0 runner    (1001) docker     (121)    98816 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/data/basic.image/logtable/table.f0
--rw-r--r--   0 runner    (1001) docker     (121)       82 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/data/basic.image/logtable/table.info
--rw-r--r--   0 runner    (1001) docker     (121)      325 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/data/basic.image/logtable/table.lock
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 16:04:24.741030 spectral-cube-0.6.0/spectral_cube/tests/data/basic.image/mask0/
--rw-r--r--   0 runner    (1001) docker     (121)      844 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/data/basic.image/mask0/table.dat
--rw-r--r--   0 runner    (1001) docker     (121)      300 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/data/basic.image/mask0/table.f0
--rw-r--r--   0 runner    (1001) docker     (121)       15 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/data/basic.image/mask0/table.f0_TSM0
--rw-r--r--   0 runner    (1001) docker     (121)       31 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/data/basic.image/mask0/table.info
--rw-r--r--   0 runner    (1001) docker     (121)      325 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/data/basic.image/mask0/table.lock
--rw-r--r--   0 runner    (1001) docker     (121)     8753 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/data/basic.image/table.dat
--rw-r--r--   0 runner    (1001) docker     (121)      293 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/data/basic.image/table.f0
--rw-r--r--   0 runner    (1001) docker     (121)      480 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/data/basic.image/table.f0_TSM0
--rw-r--r--   0 runner    (1001) docker     (121)       25 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/data/basic.image/table.info
--rw-r--r--   0 runner    (1001) docker     (121)      325 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/data/basic.image/table.lock
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 16:04:24.745030 spectral-cube-0.6.0/spectral_cube/tests/data/basic_bigendian.image/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 16:04:24.745030 spectral-cube-0.6.0/spectral_cube/tests/data/basic_bigendian.image/logtable/
--rw-r--r--   0 runner    (1001) docker     (121)     1392 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/data/basic_bigendian.image/logtable/table.dat
--rw-r--r--   0 runner    (1001) docker     (121)    98816 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/data/basic_bigendian.image/logtable/table.f0
--rw-r--r--   0 runner    (1001) docker     (121)       82 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/data/basic_bigendian.image/logtable/table.info
--rw-r--r--   0 runner    (1001) docker     (121)      325 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/data/basic_bigendian.image/logtable/table.lock
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 16:04:24.745030 spectral-cube-0.6.0/spectral_cube/tests/data/basic_bigendian.image/mask0/
--rw-r--r--   0 runner    (1001) docker     (121)      844 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/data/basic_bigendian.image/mask0/table.dat
--rw-r--r--   0 runner    (1001) docker     (121)      300 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/data/basic_bigendian.image/mask0/table.f0
--rw-r--r--   0 runner    (1001) docker     (121)       15 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/data/basic_bigendian.image/mask0/table.f0_TSM0
--rw-r--r--   0 runner    (1001) docker     (121)       31 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/data/basic_bigendian.image/mask0/table.info
--rw-r--r--   0 runner    (1001) docker     (121)      325 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/data/basic_bigendian.image/mask0/table.lock
--rw-r--r--   0 runner    (1001) docker     (121)     8753 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/data/basic_bigendian.image/table.dat
--rw-r--r--   0 runner    (1001) docker     (121)      293 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/data/basic_bigendian.image/table.f0
--rw-r--r--   0 runner    (1001) docker     (121)      480 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/data/basic_bigendian.image/table.f0_TSM0
--rw-r--r--   0 runner    (1001) docker     (121)       25 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/data/basic_bigendian.image/table.info
--rw-r--r--   0 runner    (1001) docker     (121)      325 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/data/basic_bigendian.image/table.lock
--rw-r--r--   0 runner    (1001) docker     (121)     2605 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/data/cubewcs1.hdr
--rw-r--r--   0 runner    (1001) docker     (121)     2605 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/data/cubewcs2.hdr
--rw-r--r--   0 runner    (1001) docker     (121)     8640 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/data/example_cube.fits
--rw-r--r--   0 runner    (1001) docker     (121)     8192 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/data/example_cube.lmv
--rw-r--r--   0 runner    (1001) docker     (121)      248 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/data/fk5.reg
--rw-r--r--   0 runner    (1001) docker     (121)      298 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/data/fk5_twoboxes.reg
--rw-r--r--   0 runner    (1001) docker     (121)     2265 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/data/greisen2006.hdr
--rw-r--r--   0 runner    (1001) docker     (121)     3520 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/data/header_jybeam.hdr
--rw-r--r--   0 runner    (1001) docker     (121)      211 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/data/image.reg
--rw-r--r--   0 runner    (1001) docker     (121)      234 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/data/no_overlap_fk5.reg
--rw-r--r--   0 runner    (1001) docker     (121)      217 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/data/no_overlap_image.reg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 16:04:24.745030 spectral-cube-0.6.0/spectral_cube/tests/data/nomask.image/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 16:04:24.745030 spectral-cube-0.6.0/spectral_cube/tests/data/nomask.image/logtable/
--rw-r--r--   0 runner    (1001) docker     (121)     1392 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/data/nomask.image/logtable/table.dat
--rw-r--r--   0 runner    (1001) docker     (121)    98816 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/data/nomask.image/logtable/table.f0
--rw-r--r--   0 runner    (1001) docker     (121)       82 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/data/nomask.image/logtable/table.info
--rw-r--r--   0 runner    (1001) docker     (121)      325 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/data/nomask.image/logtable/table.lock
--rw-r--r--   0 runner    (1001) docker     (121)     8753 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/data/nomask.image/table.dat
--rw-r--r--   0 runner    (1001) docker     (121)      293 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/data/nomask.image/table.f0
--rw-r--r--   0 runner    (1001) docker     (121)      480 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/data/nomask.image/table.f0_TSM0
--rw-r--r--   0 runner    (1001) docker     (121)       25 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/data/nomask.image/table.info
--rw-r--r--   0 runner    (1001) docker     (121)      325 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/data/nomask.image/table.lock
--rw-r--r--   0 runner    (1001) docker     (121)      234 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/data/partial_overlap_fk5.reg
--rw-r--r--   0 runner    (1001) docker     (121)      211 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/data/partial_overlap_image.reg
--rw-r--r--   0 runner    (1001) docker     (121)      673 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)      223 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/setup_package.py
--rw-r--r--   0 runner    (1001) docker     (121)    12009 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/test_analysis_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     9896 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/test_casafuncs.py
--rw-r--r--   0 runner    (1001) docker     (121)     1226 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/test_cube_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     7592 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/test_dask.py
--rw-r--r--   0 runner    (1001) docker     (121)     4860 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (121)    20247 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/test_masks.py
--rw-r--r--   0 runner    (1001) docker     (121)     7235 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/test_moments.py
--rw-r--r--   0 runner    (1001) docker     (121)     7845 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/test_performance.py
--rw-r--r--   0 runner    (1001) docker     (121)    26608 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/test_projection.py
--rw-r--r--   0 runner    (1001) docker     (121)    18594 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/test_regrid.py
--rw-r--r--   0 runner    (1001) docker     (121)    25767 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/test_spectral_axis.py
--rw-r--r--   0 runner    (1001) docker     (121)    93608 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/test_spectral_cube.py
--rw-r--r--   0 runner    (1001) docker     (121)     8462 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/test_stokes_spectral_cube.py
--rw-r--r--   0 runner    (1001) docker     (121)     7614 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/test_subcubes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1885 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/test_visualization.py
--rw-r--r--   0 runner    (1001) docker     (121)     7413 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/test_wcs_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3585 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/tests/utilities.py
--rw-r--r--   0 runner    (1001) docker     (121)     3232 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      142 2021-09-30 16:04:24.000000 spectral-cube-0.6.0/spectral_cube/version.py
--rw-r--r--   0 runner    (1001) docker     (121)     5243 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/visualization-tools.py
--rw-r--r--   0 runner    (1001) docker     (121)    24639 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/wcs_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    11170 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/spectral_cube/ytcube.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 16:04:24.733030 spectral-cube-0.6.0/spectral_cube.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2161 2021-09-30 16:04:24.000000 spectral-cube-0.6.0/spectral_cube.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5319 2021-09-30 16:04:24.000000 spectral-cube-0.6.0/spectral_cube.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-30 16:04:24.000000 spectral-cube-0.6.0/spectral_cube.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-30 16:04:24.000000 spectral-cube-0.6.0/spectral_cube.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      346 2021-09-30 16:04:24.000000 spectral-cube-0.6.0/spectral_cube.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2021-09-30 16:04:24.000000 spectral-cube-0.6.0/spectral_cube.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1357 2021-09-30 16:04:12.000000 spectral-cube-0.6.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:58:09.036659 spectral-cube-0.6.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:58:09.004658 spectral-cube-0.6.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:58:09.008658 spectral-cube-0.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    14437 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-22 19:58:09.040659 spectral-cube-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:58:09.016658 spectral-cube-0.6.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6786 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:58:09.016658 spectral-cube-0.6.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    19682 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/_static/radiosnakes_nostruts2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/_static/spectralcube.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:58:09.016658 spectral-cube-0.6.1/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:58:09.016658 spectral-cube-0.6.1/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/accessing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/arithmetic.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/beam_handling.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/big_data.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/continuum_subtraction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/creating_reading.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    18082 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/dask.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/developing_with_spectralcube.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/errors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/manipulating.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/masking.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/metadata.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/moments.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/nitpick-exceptions
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/quick_looks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/reprojection.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/rtd-pip-requirements
+-rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/smoothing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/spectral_extraction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/stokes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/visualization.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/writing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/yt_example.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-06-22 19:58:09.040659 spectral-cube-0.6.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1102 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:58:09.020658 spectral-cube-0.6.1/spectral_cube/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/_astropy_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/_moments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15352 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/analysis_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30075 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/base_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19734 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28876 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/cube_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65594 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/dask_spectral_cube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:58:09.020658 spectral-cube-0.6.1/spectral_cube/io/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8928 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/io/casa_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/io/casa_masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29671 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/io/class_lmv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/io/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11693 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/io/fits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41710 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/lower_dimensional_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30758 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/np_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18043 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/spectral_axis.py
+-rw-r--r--   0 runner    (1001) docker     (123)   173469 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/spectral_cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12286 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/stokes_spectral_cube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:58:09.028658 spectral-cube-0.6.1/spectral_cube/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:58:09.028658 spectral-cube-0.6.1/spectral_cube/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/255-fk5.reg
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/255-pixel.reg
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:58:09.032659 spectral-cube-0.6.1/spectral_cube/tests/data/basic.image/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:58:09.032659 spectral-cube-0.6.1/spectral_cube/tests/data/basic.image/logtable/
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/basic.image/logtable/table.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    98816 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/basic.image/logtable/table.f0
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/basic.image/logtable/table.info
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/basic.image/logtable/table.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:58:09.032659 spectral-cube-0.6.1/spectral_cube/tests/data/basic.image/mask0/
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/basic.image/mask0/table.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/basic.image/mask0/table.f0
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/basic.image/mask0/table.f0_TSM0
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/basic.image/mask0/table.info
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/basic.image/mask0/table.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/basic.image/table.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/basic.image/table.f0
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/basic.image/table.f0_TSM0
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/basic.image/table.info
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/basic.image/table.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:58:09.032659 spectral-cube-0.6.1/spectral_cube/tests/data/basic_bigendian.image/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:58:09.036659 spectral-cube-0.6.1/spectral_cube/tests/data/basic_bigendian.image/logtable/
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/basic_bigendian.image/logtable/table.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    98816 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/basic_bigendian.image/logtable/table.f0
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/basic_bigendian.image/logtable/table.info
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/basic_bigendian.image/logtable/table.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:58:09.036659 spectral-cube-0.6.1/spectral_cube/tests/data/basic_bigendian.image/mask0/
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/basic_bigendian.image/mask0/table.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/basic_bigendian.image/mask0/table.f0
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/basic_bigendian.image/mask0/table.f0_TSM0
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/basic_bigendian.image/mask0/table.info
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/basic_bigendian.image/mask0/table.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/basic_bigendian.image/table.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/basic_bigendian.image/table.f0
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/basic_bigendian.image/table.f0_TSM0
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/basic_bigendian.image/table.info
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/basic_bigendian.image/table.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/cubewcs1.hdr
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/cubewcs2.hdr
+-rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/example_cube.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/example_cube.lmv
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/fk5.reg
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/fk5_twoboxes.reg
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/greisen2006.hdr
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/header_jybeam.hdr
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/image.reg
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/no_overlap_fk5.reg
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/no_overlap_image.reg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:58:09.036659 spectral-cube-0.6.1/spectral_cube/tests/data/nomask.image/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:58:09.036659 spectral-cube-0.6.1/spectral_cube/tests/data/nomask.image/logtable/
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/nomask.image/logtable/table.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    98816 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/nomask.image/logtable/table.f0
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/nomask.image/logtable/table.info
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/nomask.image/logtable/table.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/nomask.image/table.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/nomask.image/table.f0
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/nomask.image/table.f0_TSM0
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/nomask.image/table.info
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/nomask.image/table.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/partial_overlap_fk5.reg
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/partial_overlap_image.reg
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/setup_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13651 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/test_analysis_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12356 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/test_casafuncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/test_cube_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10364 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/test_dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20247 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/test_masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/test_moments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/test_performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27709 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/test_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23136 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/test_regrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25767 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/test_spectral_axis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98333 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/test_spectral_cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10977 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/test_stokes_spectral_cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/test_subcubes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/test_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/test_wcs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-22 19:58:08.000000 spectral-cube-0.6.1/spectral_cube/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/visualization-tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24639 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/wcs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/ytcube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:58:09.020658 spectral-cube-0.6.1/spectral_cube.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-22 19:58:08.000000 spectral-cube-0.6.1/spectral_cube.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5476 2023-06-22 19:58:09.000000 spectral-cube-0.6.1/spectral_cube.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 19:58:08.000000 spectral-cube-0.6.1/spectral_cube.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 19:58:08.000000 spectral-cube-0.6.1/spectral_cube.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-22 19:58:08.000000 spectral-cube-0.6.1/spectral_cube.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-22 19:58:08.000000 spectral-cube-0.6.1/spectral_cube.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/tox.ini
```

### Comparing `spectral-cube-0.6.0/.gitignore` & `spectral-cube-0.6.1/.gitignore`

 * *Files 26% similar despite different names*

```diff
@@ -56,7 +56,8 @@
 *.fits
 
 # Other generated stuff
 */version.py
 */cython_version.py
 
 .tmp
+.ipynb_checkpoints
```

### Comparing `spectral-cube-0.6.0/CHANGES.rst` & `spectral-cube-0.6.1/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+0.6.1.dev (2023-06-22)
+----------------------
+- Fix memory issue when calling statistics() on FITS cubes. #752
+- Cube mosaicing implemented #829, #844
+- Varied bugfixes for numpy compatibility #858, #865, #883
+- Many other small fixes & improvements that didn't get changelog entries
+
 0.6 (2021-09-30)
 ----------------
 - Fix `convolve_to` when units are in Jy/beam. Add error/warnings for operations
   for all operations that change the spatial resolution for Jy/beam cubes.
 - Add ``argmax_world`` and ``argmin_world`` to return the argmin/max position
   in WCS coordinates. This is ONLY defined for independent WCS axes
   (e.g., spectral) #680
```

### Comparing `spectral-cube-0.6.0/LICENSE.rst` & `spectral-cube-0.6.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.0/PKG-INFO` & `spectral-cube-0.6.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: spectral-cube
-Version: 0.6.0
+Version: 0.6.1
 Summary: A package for interaction with spectral cubes
 Home-page: http://spectral-cube.readthedocs.org
 Author: Adam Ginsburg, Tom Robitaille,  Chris Beaumont, Adam Leroy, Erik Rosolowsky, and Eric Koch
 Author-email: adam.g.ginsburg@gmail.com
 License: BSD
-Platform: UNKNOWN
 Provides-Extra: test
 Provides-Extra: docs
-Provides-Extra: novis
-Provides-Extra: all
+Provides-Extra: noviz
+Provides-Extra: viz
+Provides-Extra: viz_extra
+Provides-Extra: dev
 License-File: LICENSE.rst
 
 About
 =====
 
 |Join the chat at https://gitter.im/radio-astro-tools/spectral-cube|
 
@@ -29,29 +30,27 @@
    Powered by Astropy Badge
 
 Credits
 =======
 
 This package is developed by:
 
--  Chris Beaumont (`@ChrisBeaumont <http://github.com/ChrisBeaumont>`__)
+-  Eric Koch (`@e-koch <https://github.com/e-koch>`__)
 -  Adam Ginsburg (`@keflavich <http://github.com/keflavich>`__)
--  Adam Leroy (`@akleroy <http://github.com/akleroy>`__)
 -  Thomas Robitaille (`@astrofrog <http://github.com/astrofrog>`__)
 -  Erik Rosolowsky (`@low-sky <http://github.com/low-sky>`__)
--  Eric Koch (`@e-koch <https://github.com/e-koch>`__)
+
+Original development included substantial contributions from:
+-  Adam Leroy (`@akleroy <http://github.com/akleroy>`__)
+-  Chris Beaumont (`@ChrisBeaumont <http://github.com/ChrisBeaumont>`__)
 
 Build and coverage status
 =========================
 
-|Build Status| |Coverage Status| |DOI|
+|Coverage Status| |DOI|
 
 .. |Join the chat at https://gitter.im/radio-astro-tools/spectral-cube| image:: https://badges.gitter.im/Join%20Chat.svg
    :target: https://gitter.im/radio-astro-tools/spectral-cube?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
-.. |Build Status| image:: https://travis-ci.org/radio-astro-tools/spectral-cube.png?branch=master
-   :target: https://travis-ci.org/radio-astro-tools/spectral-cube
 .. |Coverage Status| image:: https://coveralls.io/repos/radio-astro-tools/spectral-cube/badge.svg?branch=master
    :target: https://coveralls.io/r/radio-astro-tools/spectral-cube?branch=master
 .. |DOI| image:: https://zenodo.org/badge/doi/10.5281/zenodo.11485.svg
    :target: http://dx.doi.org/10.5281/zenodo.11485
-
-
```

### Comparing `spectral-cube-0.6.0/README.rst` & `spectral-cube-0.6.1/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -14,27 +14,27 @@
    Powered by Astropy Badge
 
 Credits
 =======
 
 This package is developed by:
 
--  Chris Beaumont (`@ChrisBeaumont <http://github.com/ChrisBeaumont>`__)
+-  Eric Koch (`@e-koch <https://github.com/e-koch>`__)
 -  Adam Ginsburg (`@keflavich <http://github.com/keflavich>`__)
--  Adam Leroy (`@akleroy <http://github.com/akleroy>`__)
 -  Thomas Robitaille (`@astrofrog <http://github.com/astrofrog>`__)
 -  Erik Rosolowsky (`@low-sky <http://github.com/low-sky>`__)
--  Eric Koch (`@e-koch <https://github.com/e-koch>`__)
+
+Original development included substantial contributions from:
+-  Adam Leroy (`@akleroy <http://github.com/akleroy>`__)
+-  Chris Beaumont (`@ChrisBeaumont <http://github.com/ChrisBeaumont>`__)
 
 Build and coverage status
 =========================
 
-|Build Status| |Coverage Status| |DOI|
+|Coverage Status| |DOI|
 
 .. |Join the chat at https://gitter.im/radio-astro-tools/spectral-cube| image:: https://badges.gitter.im/Join%20Chat.svg
    :target: https://gitter.im/radio-astro-tools/spectral-cube?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
-.. |Build Status| image:: https://travis-ci.org/radio-astro-tools/spectral-cube.png?branch=master
-   :target: https://travis-ci.org/radio-astro-tools/spectral-cube
 .. |Coverage Status| image:: https://coveralls.io/repos/radio-astro-tools/spectral-cube/badge.svg?branch=master
    :target: https://coveralls.io/r/radio-astro-tools/spectral-cube?branch=master
 .. |DOI| image:: https://zenodo.org/badge/doi/10.5281/zenodo.11485.svg
    :target: http://dx.doi.org/10.5281/zenodo.11485
```

### Comparing `spectral-cube-0.6.0/docs/Makefile` & `spectral-cube-0.6.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.0/docs/accessing.rst` & `spectral-cube-0.6.1/docs/accessing.rst`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.0/docs/api.rst` & `spectral-cube-0.6.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.0/docs/arithmetic.rst` & `spectral-cube-0.6.1/docs/arithmetic.rst`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.0/docs/beam_handling.rst` & `spectral-cube-0.6.1/docs/beam_handling.rst`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.0/docs/big_data.rst` & `spectral-cube-0.6.1/docs/big_data.rst`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.0/docs/conf.py` & `spectral-cube-0.6.1/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,19 @@
 
 
 # Custom sidebar templates, maps document names to template names.
 #html_sidebars = {}
 
 # The name of an image file (relative to this directory) to place at the top
 # of the sidebar.
-#html_logo = ''
+# html_logo = 'radiosnakes_nostruts2.svg'
+
+# Static files to copy after template files
+html_static_path = ['_static']
+html_style = 'spectralcube.css'
 
 # The name of an image file (within the static path) to use as favicon of the
 # docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
 # pixels large.
 #html_favicon = ''
 
 # If not '', a 'Last updated on:' timestamp is inserted at every page bottom,
```

### Comparing `spectral-cube-0.6.0/docs/continuum_subtraction.rst` & `spectral-cube-0.6.1/docs/continuum_subtraction.rst`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.0/docs/dask.rst` & `spectral-cube-0.6.1/docs/dask.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+.. _doc_dask:
+
 Integration with dask
 =====================
 
 Getting started
 ---------------
 
 When loading a cube with the :class:`~spectral_cube.SpectralCube` class, it is possible to optionally
@@ -21,14 +23,18 @@
      n_x:      3  type_x: RA---ARC  unit_x: deg    range:    52.231466 deg:   52.231544 deg
      n_y:      4  type_y: DEC--ARC  unit_y: deg    range:    31.243639 deg:   31.243739 deg
      n_s:      7  type_s: VRAD      unit_s: m / s  range:    14322.821 m / s:   14944.909 m / s
 
 Most of the properties and methods that normally work with :class:`~spectral_cube.SpectralCube`
 should continue to work with :class:`~spectral_cube.DaskSpectralCube`.
 
+For an interactive demonstration, see the `Guide to Dask Optimization <https://github.com/radio-astro-tools/tutorials/pull/21>`_.
+
+..
+    TODO: UPDATE THE LINK TO THE TUTORIAL once merged
 
 Schedulers and parallel computations
 ------------------------------------
 
 By default, we use the ``'synchronous'`` `dask scheduler <https://docs.dask.org/en/latest/scheduler-overview.html>`_
 which means that calculations are run in a single process/thread. However, you can control this using the
 :meth:`~spectral_cube.DaskSpectralCube.use_dask_scheduler` method:
```

### Comparing `spectral-cube-0.6.0/docs/errors.rst` & `spectral-cube-0.6.1/docs/errors.rst`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.0/docs/examples.rst` & `spectral-cube-0.6.1/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.0/docs/index.rst` & `spectral-cube-0.6.1/docs/index.rst`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,17 @@
   wide range of conventions of axis order, spatial projections,
   and spectral units that exist in the wild.
 - Easy extraction of cube sub-regions using physical coordinates.
 - Ability to easily create, combine, and apply masks to datasets.
 - Basic summary statistic methods like moments and array aggregates.
 - Designed to work with datasets too large to load into memory.
 
+You can find the latest version and the issue tracker on `github
+<https://github.com/radio-astro-tools/spectral-cube>`_.
+
 Quick start
 -----------
 
 Here's a simple script demonstrating the spectral-cube package::
 
     >>> import astropy.units as u
     >>> from astropy.utils import data
@@ -69,14 +72,15 @@
    errors.rst
    writing.rst
    beam_handling.rst
    masking.rst
    arithmetic.rst
    metadata.rst
    smoothing.rst
+   reprojection.rst
 
 Subsets
 ^^^^^^^
 
 .. toctree::
    :maxdepth: 2
 
@@ -111,8 +115,9 @@
 
 .. toctree::
    :maxdepth: 1
 
    dask.rst
    yt_example.rst
    big_data.rst
+   developing_with_spectralcube.rst
    api.rst
```

### Comparing `spectral-cube-0.6.0/docs/installing.rst` & `spectral-cube-0.6.1/docs/installing.rst`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 Installation
 ------------
 
 To install the latest stable release, you can type::
 
     pip install spectral-cube
 
+(you may need to add ``--upgrade`` if you already have an older version installed) 
 or you can download the latest tar file from
 `PyPI <https://pypi.python.org/pypi/spectral-cube>`_ and install it using::
 
     python setup.py install
 
 If you are using python2.7 (e.g., if you are using CASA version 5 or earlier),
 the latest spectral-cube version that is compatible is v0.4.4. Note that `Astropy v2.0 <https://docs.astropy.org/en/v2.0.16/install.html>__` is the last version to support python2.7.
```

### Comparing `spectral-cube-0.6.0/docs/manipulating.rst` & `spectral-cube-0.6.1/docs/manipulating.rst`

 * *Files 7% similar despite different names*

```diff
@@ -89,32 +89,32 @@
 <https://casaguides.nrao.edu/index.php/CASA_Region_Format>`_ regions to extract
 subcubes. The minimal enclosing subcube will be extracted with a two-dimensional
 mask corresponding to the DS9/CRTF region.  `Regions
 <https://astropy-regions.readthedocs.io/en/latest/>`_ is required for region
 parsing.  CRTF regions may also contain spectral cutout information.
 
 This example shows extraction of a subcube from a ds9 region file ``file.reg``.
-`~regions.read_ds9` parses the ds9 file and converts it to a list of
+`~regions.Regions.read` parses the ds9 file and converts it to a list of
 `~regions.Region` objects::
 
     >>> import regions # doctest: +SKIP
-    >>> region_list = regions.read_ds9('file.reg')  # doctest: +SKIP
+    >>> region_list = regions.Regions.read('file.reg')  # doctest: +SKIP
     >>> sub_cube = cube.subcube_from_regions(region_list)  # doctest: +SKIP
 
 This one shows extraction of a subcube from a CRTF region file ``file.crtf``,
 parsed using `~regions.read_crtf`::
 
     >>> import regions # doctest: +SKIP
     >>> region_list = regions.read_crtf('file.reg')  # doctest: +SKIP
     >>> sub_cube = cube.subcube_from_regions(region_list)  # doctest: +SKIP
 
 If you want to loop over individual regions with a single region file, you need
 to convert the individual regions to lists of that region::
 
-    >>> region_list = regions.read_ds9('file.reg')  #doctest: +SKIP
+    >>> region_list = regions.Regions.read('file.reg')  #doctest: +SKIP
     >>> for region in region_list: #doctest: +SKIP
     >>>     sub_cube = cube.subcube_from_regions([region]) #doctest: +SKIP
     
 You can also directly use a ds9 region string.  This example extracts a 0.1
 degree circle around the Galactic Center::
 
     >>> region_str = "galactic; circle(0, 0, 0.1)"  # doctest: +SKIP
@@ -151,14 +151,24 @@
 
     >>> sub_cube = cube.minimal_subcube()  # doctest: +SKIP
 
 You can also shrink any cube by this mechanism::
 
     >>> sub_cube = cube.with_mask(smaller_region).minimal_subcube()  # doctest: +SKIP
 
+If you have many cubes that are the same shape, and you want to cut them out in
+the same way (e.g., for CASA image, model, residual, and other cubes), you can
+get the slice to make the cutout and reuse it.  It can also be helpful to cut
+only in the spatial dimensions::
+
+    >>> subcube_slice = cube.subcube_slices_from_mask(cube.mask, spatial_only=True)
+    >>> mod_subcube = modcube[subcube_slice]
+    >>> resid_subcube = residcube[subcube_slice]
+    >>> subcube = cube[subcube_slice]
+
 
 Extract a spatial and spectral subcube
 --------------------------------------
 There is a generic subcube function that allows slices in the spatial and
 spectral axes simultaneously, as long as the spatial axes are aligned with the
 pixel axes.  An arbitrary example looks like this::
```

### Comparing `spectral-cube-0.6.0/docs/masking.rst` & `spectral-cube-0.6.1/docs/masking.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+.. _doc_masking:
+
 Masking
 =======
 
 Getting started
 ---------------
 
 In addition to supporting the representation of data and associated WCS, it
@@ -60,15 +62,15 @@
 Any boolean area that can be `broadcast
 <http://docs.scipy.org/doc/numpy/user/basics.broadcasting.html>`_ to the cube
 shape can be used as a boolean array mask.
 
 Accessing masked data
 ---------------------
 
-As mention in :doc:`accessing`, the raw and unmasked data can be accessed with
+As mentioned in :doc:`accessing`, the raw and unmasked data can be accessed with
 the `spectral_cube.spectral_cube.BaseSpectralCube.unmasked_data`
 attribute.  You can access the masked data using ``filled_data``. This array is
 a copy of the original data with any masked value replaced by a fill value
 (which is ``np.nan`` by default but can be changed using the ``fill_value``
 option in the :class:`~spectral_cube.SpectralCube` initializer). The 'filled'
 data is accessed with e.g.::
```

### Comparing `spectral-cube-0.6.0/docs/metadata.rst` & `spectral-cube-0.6.1/docs/metadata.rst`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.0/docs/moments.rst` & `spectral-cube-0.6.1/docs/moments.rst`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.0/docs/nitpick-exceptions` & `spectral-cube-0.6.1/docs/nitpick-exceptions`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.0/docs/quick_looks.rst` & `spectral-cube-0.6.1/docs/quick_looks.rst`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.0/docs/smoothing.rst` & `spectral-cube-0.6.1/docs/smoothing.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+=========
 Smoothing
----------
+=========
 
 There are two types of smoothing routine available in ``spectral_cube``:
 spatial and spectral.
 
 Spatial Smoothing
 =================
 
@@ -87,14 +88,16 @@
     new_cube = cube.spatial_smooth(kernel)
     new_cube.write('/some_path/some_other_file.fits')
 
 ``x_stddev`` specifies the width of the `Gaussian kernel <http://docs.astropy.org/en/stable/api/astropy.convolution.Gaussian2DKernel.html>`_.
 Any `astropy convolution <kernel http://docs.astropy.org/en/stable/convolution/kernels.html>`_
 is acceptable.
 
+.. _Spectral-Smoothing:
+
 Spectral Smoothing
 ==================
 
 Only :class:`~spectral_cube.SpectralCube` instances with a consistent beam can
 be spectrally smoothed, so if you have a
 :class:`~spectral_cube.VaryingResolutionSpectralCube`, you must convolve each
 slice in it to a common resolution before spectrally smoothing.
```

### Comparing `spectral-cube-0.6.0/docs/spectral_extraction.rst` & `spectral-cube-0.6.1/docs/spectral_extraction.rst`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.0/docs/visualization.rst` & `spectral-cube-0.6.1/docs/visualization.rst`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.0/docs/yt_example.rst` & `spectral-cube-0.6.1/docs/yt_example.rst`

 * *Files 3% similar despite different names*

```diff
@@ -54,26 +54,26 @@
 .. note::
 
     The :meth:`~spectral_cube.SpectralCube.to_yt` method and its associated
     coordinate methods are compatible with both yt v. 2.x and v. 3.0 and
     following, but use of version 3.0 or later is recommended due to
     substantial improvements in support for FITS data. For more information on
     how yt handles FITS datasets, see `the yt docs
-    <http://yt-project.org/docs/3.0/examining/loading_data.html#fits-data>`_.
+    <http://yt-project.org/doc/examining/loading_data.html#fits-data>`_.
 
 Visualization example
 ---------------------
 
 This section shows an example of a rendering script that can be used to
 produce a 3-d isocontour visualization using an object returned by
 :meth:`~spectral_cube.SpectralCube.to_yt`::
 
     import numpy as np
     from spectral_cube import SpectralCube
-    from yt.mods import ColorTransferFunction, write_bitmap
+    import yt
     import astropy.units as u
 
     # Read in spectral cube
     cube = SpectralCube.read('L1448_13CO.fits', format='fits')
 
     # Extract the yt object from the SpectralCube instance
     ytcube = cube.to_yt(spectral_factor=0.75)
@@ -83,15 +83,15 @@
     # of the isocontours
     n_v = 10
     vmin = 0.05
     vmax = 4.0
     dv = 0.02
 
     # Set up color transfer function
-    transfer = ColorTransferFunction((vmin, vmax))
+    transfer = yt.ColorTransferFunction((vmin, vmax))
     transfer.add_layers(n_v, dv, colormap='RdBu_r')
 
     # Set up the camera parameters
 
     # Derive the pixel coordinate of the desired center
     # from the corresponding world coordinate
     center = ytcube.world2yt([51.424522,
@@ -102,18 +102,18 @@
     size = 1024
 
     camera = ds.camera(center, direction, width, size, transfer,
                        fields=['flux'])
 
     # Take a snapshot and save to a file
     snapshot = camera.snapshot()
-    write_bitmap(snapshot, 'cube_rendering.png', transpose=True)
+    yt.write_bitmap(snapshot, 'cube_rendering.png', transpose=True)
 
 You can move the camera around; see the `yt camera docs
-<http://yt-project.org/docs/dev/reference/api/generated/yt.visualization.volume_rendering.camera.Camera.html>`_.
+<https://yt-project.org/doc/reference/api/yt.visualization.volume_rendering.camera.html>`_.
 
 Movie Making
 ------------
 
 There is a simple utility for quick movie making.  The default movie is a rotation
 of the cube around one of the spatial axes, going from PP -> PV space and back.::
```

### Comparing `spectral-cube-0.6.0/setup.cfg` & `spectral-cube-0.6.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -21,37 +21,40 @@
 	joblib
 	casa-formats-io
 
 [options.extras_require]
 test = 
 	pytest-astropy
 	pytest-cov
+	regions>=0.7
+	numpy>=1.24.0
+	astropy>=5.2.1
 docs = 
 	sphinx-astropy
 	matplotlib
-novis = 
+noviz = 
 	zarr
 	fsspec
 	distributed
 	pvextractor
-	regions
-	reproject
+	reproject>=0.9.1
 	scipy
-all = 
-	zarr
-	fsspec
-	distributed
+viz = 
 	aplpy
-	glue-core[qt]
 	matplotlib
-	pvextractor
-	regions
 	reproject
-	scipy
+	pvextractor
+viz_extra = 
+	glue-core[qt]
 	yt ; python_version<'3.8'
+dev = 
+	pvextractor
+	radio-beam
+	reproject
+	regions
 
 [options.package_data]
 spectral_cube.tests = 
 	data/*
 	data/*/*
 spectral_cube.io.tests = data/*/*
```

### Comparing `spectral-cube-0.6.0/setup.py` & `spectral-cube-0.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.0/spectral_cube/__init__.py` & `spectral-cube-0.6.1/spectral_cube/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 # Licensed under a 3-clause BSD style license - see LICENSE.rst
 
 from ._astropy_init import __version__, test
 
-from pkg_resources import get_distribution, DistributionNotFound
-
 from .spectral_cube import (SpectralCube, VaryingResolutionSpectralCube)
 from .dask_spectral_cube import (DaskSpectralCube, DaskVaryingResolutionSpectralCube)
 from .stokes_spectral_cube import StokesSpectralCube
 from .masks import (MaskBase, InvertedMask, CompositeMask,
                     BooleanArrayMask, LazyMask, LazyComparisonMask,
                     FunctionMask)
 from .lower_dimensional_structures import (OneDSpectrum, Projection, Slice)
```

### Comparing `spectral-cube-0.6.0/spectral_cube/_astropy_init.py` & `spectral-cube-0.6.1/spectral_cube/_astropy_init.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.0/spectral_cube/_moments.py` & `spectral-cube-0.6.1/spectral_cube/_moments.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     moment0 : array
     """
     shp = _moment_shp(cube, axis)
     result = np.zeros(shp)
 
     view = [slice(None)] * 3
 
-    valid = np.zeros(shp, dtype=np.bool)
+    valid = np.zeros(shp, dtype=bool)
     for i in range(cube.shape[axis]):
         view[axis] = i
         plane = cube._get_filled_data(fill=np.nan, view=tuple(view))
         valid |= np.isfinite(plane)
         result += np.nan_to_num(plane) * cube._pix_size_slice(axis)
     result[~valid] = np.nan
     return result
```

### Comparing `spectral-cube-0.6.0/spectral_cube/analysis_utilities.py` & `spectral-cube-0.6.1/spectral_cube/analysis_utilities.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import numpy as np
 
 from astropy import units as u
 from six.moves import zip, range
 from astropy.wcs import WCS
 from astropy.utils.console import ProgressBar
+from astropy import log
 import warnings
 
 from .utils import BadVelocitiesWarning
 from .cube_utils import _map_context
 from .lower_dimensional_structures import VaryingResolutionOneDSpectrum, OneDSpectrum
-from .spectral_cube import VaryingResolutionSpectralCube
+from .spectral_cube import VaryingResolutionSpectralCube, SpectralCube
 
 
 def fourier_shift(x, shift, axis=0, add_pad=False, pad_size=None):
     '''
     Shift a spectrum in the Fourier plane.
 
     Parameters
@@ -200,15 +201,15 @@
         v0 = cube.spectral_axis.mean()
     else:
         if not isinstance(v0, u.Quantity):
             raise u.UnitsError("v0 must be a quantity.")
         spec_unit = cube.spectral_axis.unit
         if not v0.unit.is_equivalent(spec_unit):
             raise u.UnitsError("v0 must have units equivalent to the cube's"
-                               " spectral unit ().".format(spec_unit))
+                               f" spectral unit {spec_unit}.")
 
         v0 = v0.to(spec_unit)
 
         if v0 < cube.spectral_axis.min() or v0 > cube.spectral_axis.max():
             raise ValueError("v0 must be within the range of the spectral "
                              "axis of the cube.")
 
@@ -240,15 +241,15 @@
             (velocity_surface > vmin),
             velocity_surface.value, np.nan)
         velocity_surface = u.Quantity(masked_velocities, velocity_surface.unit)
 
     pix_shifts = vdiff_sign * ((velocity_surface.to(vel_unit) -
                                 v0.to(vel_unit)) / vdiff).value[xy_posns]
 
-    # May a header copy so we can start altering
+    # Make a header copy so we can start altering
     new_header = cube[:, 0, 0].header.copy()
 
     if pad_edges:
         # Enables padding the whole cube such that no spectrum will wrap around
         # This is critical if a low-SB component is far off of the bright
         # component that the velocity surface is derived from.
 
@@ -315,65 +316,119 @@
         stack_spec = OneDSpectrum(stacked, unit=cube.unit, wcs=WCS(new_header),
                                   header=new_header, meta=cube.meta,
                                   spectral_unit=vel_unit, beam=cube.beam)
 
     return stack_spec
 
 
-def stack_cube(cube, linelist, vmin, vmax, average=np.nanmean, convolve_beam=None):
+def stack_cube(cube, linelist, vmin, vmax, average=np.nanmean,
+               convolve_beam=None, return_hdu=False,
+               return_cutouts=False):
     """
     Create a stacked cube by averaging on a common velocity grid.
 
+    If the input cubes have varying resolution, this will trigger potentially
+    expensive convolutions.
+
     Parameters
     ----------
     cube : SpectralCube
-        The cube
+        The cube (or a list of cubes)
     linelist : list of Quantities
         An iterable of Quantities representing line rest frequencies
     vmin / vmax : Quantity
         Velocity-equivalent quantities specifying the velocity range to average
         over
     average : function
         A function that can operate over a list of numpy arrays (and accepts
         ``axis=0``) to average the spectra.  `numpy.nanmean` is the default,
         though one might consider `numpy.mean` or `numpy.median` as other
         options.
     convolve_beam : None
         If the cube is a VaryingResolutionSpectralCube, a convolution beam is
         required to put the cube onto a common grid prior to spectral
         interpolation.
+    return_hdu : bool
+        Return an HDU instead of a spectral-cube
+    return_cutouts : bool
+        Also return the individual cube cutouts?
+
+    Returns
+    =======
+    cube : SpectralCube
+        The SpectralCube object containing the reprojected cube.  Its header
+        will be based on the first cube but will have no reference frequency.
+        Its spectral axis will be in velocity units.
+    cutout_cubes : list
+        A list of cube cutouts projected into the same space (optional; see
+        ``return_cutouts``)
     """
 
-    line_cube = cube.with_spectral_unit(u.km/u.s,
-                                        velocity_convention='radio',
-                                        rest_value=linelist[0])
-    if isinstance(line_cube, VaryingResolutionSpectralCube):
-        if convolve_beam is None:
-            raise ValueError("When stacking VaryingResolutionSpectralCubes, "
-                             "you must specify a target beam size with the "
-                             "keyword `convolve_beam`")
-        reference_cube = line_cube.spectral_slab(vmin, vmax).convolve_to(convolve_beam)
+    if isinstance(cube, list):
+        cubes = cube
+        cube = cubes[0]
+        for cb in cubes[1:]:
+            if cb.shape[1:] != cube.shape[1:]:
+                raise ValueError("If you pass multiple cubes, they must have the "
+                                 "same spatial shape.")
+        if convolve_beam is None and (any(hasattr(cb, 'beams') for cb in cubes) or
+                                      not all([cb.beam == cube.beam for cb in cubes[1:]])):
+            raise ValueError("If the cubes have different resolution, `convolve_beam` must be specified.")
     else:
-        reference_cube = line_cube.spectral_slab(vmin, vmax)
+        cubes = [cube]
 
-    cutout_cubes = [reference_cube.filled_data[:].value]
-
-    for restval in linelist[1:]:
-        line_cube = cube.with_spectral_unit(u.km/u.s,
-                                            velocity_convention='radio',
-                                            rest_value=restval)
-        line_cutout = line_cube.spectral_slab(vmin, vmax)
+    slabs = []
+    included_lines = []
 
-        if isinstance(line_cube, VaryingResolutionSpectralCube):
-            line_cutout = line_cutout.convolve_to(convolve_beam)
+    # loop over linelist first to keep the cutouts in the same order as the
+    # input line frequencies
+    for restval in linelist:
+        for cube in cubes:
+            line_cube = cube.with_spectral_unit(u.km/u.s,
+                                                velocity_convention='radio',
+                                                rest_value=restval)
+            line_cutout = line_cube.spectral_slab(vmin, vmax)
+            if line_cutout.shape[0] <= 1:
+                log.debug(f"Skipped line {restval} for cube {cube} because it resulted"
+                          "in a size-1 spectral axis")
+                continue
+            else:
+                included_lines.append(restval)
+
+            assert line_cutout.shape[0] > 1
+
+            if isinstance(line_cutout, VaryingResolutionSpectralCube):
+                if convolve_beam is None:
+                    raise ValueError("If any of the input cubes have varyin resolution, "
+                                     "a target `common_beam` must be specified.")
+                line_cutout = line_cutout.convolve_to(convolve_beam)
 
-        regridded = line_cutout.spectral_interpolate(reference_cube.spectral_axis)
+            assert not isinstance(line_cutout, VaryingResolutionSpectralCube)
+            slabs.append(line_cutout)
 
+    reference_cube = slabs[0]
+    cutout_cubes = [reference_cube.filled_data[:].value]
+    for slab in slabs[1:]:
+        regridded = slab.spectral_interpolate(reference_cube.spectral_axis)
         cutout_cubes.append(regridded.filled_data[:].value)
 
     stacked_cube = average(cutout_cubes, axis=0)
 
-    hdu = reference_cube.hdu
+    ww = reference_cube.wcs.copy()
+    # set restfreq to zero: it is not defined any more.
+    ww.wcs.restfrq = 0.0
+    meta = reference_cube.meta
+    meta.update({'stacked_lines': included_lines})
+    result_cube = SpectralCube(data=stacked_cube,
+                               wcs=ww,
+                               meta=meta,
+                               header=reference_cube.header)
 
-    hdu.data = stacked_cube
+    if return_hdu:
+        retval = result_cube.hdu
+    else:
+        retval = result_cube
 
-    return hdu
+    if return_cutouts:
+        return retval, cutout_cubes
+    else:
+        return retval
```

### Comparing `spectral-cube-0.6.0/spectral_cube/base_class.py` & `spectral-cube-0.6.1/spectral_cube/base_class.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,19 @@
     def meta(self):
         return self._meta
 
     @property
     def mask(self):
         return self._mask
 
+    @mask.setter
+    def mask(self, value):
+        self._mask = value
+
+
 class HeaderMixinClass(object):
     """
     A mixin class to provide header updating from WCS objects.
     The parent object must have a WCS.
     """
 
     def wcs(self):
@@ -110,15 +115,15 @@
         when smoothing will affect brightness in Jy/beam operations.
 
         This is also true for using the `with_beam` and `with_beams` methods, including 1D spectra with
         Jy/beam units.
 
         Parameters
         ----------
-        raise_error_jybeam : bool, optional
+        raise_error_jybm : bool, optional
             Raises a `~spectral_cube.utils.BeamUnitsError` when True (default). When False, it triggers a
             `~spectral_cube.utils.BeamWarning`.
 
             .. note: This is a reminder to expose raise_error_jybm to top-level functions.
 
         '''
 
@@ -632,14 +637,18 @@
                 beam_mask = self.goodbeams_mask
         else:
             if mask.ndim > 1:
                 beam_mask = np.logical_and(mask, self.goodbeams_mask[:, None, None])
             else:
                 beam_mask = np.logical_and(mask, self.goodbeams_mask)
 
+        if not any(beam_mask):
+            raise ValueError("All beams were excluded using threshold {threshold}"
+                             .format(threshold=threshold))
+
         # use private _beams here because the public one excludes the bad beams
         # by default
         new_beam = self._beams.average_beam(includemask=beam_mask)
 
         if np.isnan(new_beam):
             raise ValueError("Beam was not finite after averaging.  "
                              "This either indicates that there was a problem "
```

### Comparing `spectral-cube-0.6.0/spectral_cube/conftest.py` & `spectral-cube-0.6.1/spectral_cube/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -77,27 +77,81 @@
     beams.header['TUNIT2'] = 'arcsec'
     beams.header['TTYPE3'] = 'BPA'
     beams.header['TUNIT3'] = 'deg'
 
     return beams
 
 
+def prepare_4_beams_withfullpol():
+
+    nchan = 4
+    npol = 4
+
+    beams = np.recarray(nchan*npol, dtype=[('BMAJ', '>f4'), ('BMIN', '>f4'),
+                                           ('BPA', '>f4'), ('CHAN', '>i4'),
+                                           ('POL', '>i4')])
+    beams['BMAJ'] = [0.4,0.3,0.3,0.4] * npol # arcseconds
+    beams['BMIN'] = [0.1,0.2,0.2,0.1] * npol
+    beams['BPA'] = [0,45,60,30] * npol # degrees
+    beams['CHAN'] = [0,1,2,3] * npol
+
+    pol_codes = []
+    for i in range(npol):
+        pol_codes.extend([i] * nchan)
+
+    beams['POL'] = pol_codes
+
+    beams = fits.BinTableHDU(beams)
+
+    beams.header['TTYPE1'] = 'BMAJ'
+    beams.header['TUNIT1'] = 'arcsec'
+    beams.header['TTYPE2'] = 'BMIN'
+    beams.header['TUNIT2'] = 'arcsec'
+    beams.header['TTYPE3'] = 'BPA'
+    beams.header['TUNIT3'] = 'deg'
+    beams.header['TTYPE4'] = 'CHAN'
+    beams.header['TTYPE5'] = 'POL'
+
+    return beams
+
+
 def prepare_advs_data():
     # Single Stokes
     h = fits.header.Header.fromtextfile(HEADER_FILENAME)
     h['BUNIT'] = 'K' # Kelvins are a valid unit, JY/BEAM are not: they should be tested separately
     h['NAXIS1'] = 2
     h['NAXIS2'] = 3
     h['NAXIS3'] = 4
     h['NAXIS4'] = 1
     np.random.seed(42)
     d = np.random.random((1, 2, 3, 4))
     return d, h
 
 
+def prepare_advs_fullstokes_data():
+    # Full Stokes
+    h = fits.header.Header.fromtextfile(HEADER_FILENAME)
+    h['BUNIT'] = 'K' # Kelvins are a valid unit, JY/BEAM are not: they should be tested separately
+    h['NAXIS1'] = 2
+    h['NAXIS2'] = 3
+    h['NAXIS3'] = 4
+    h['NAXIS4'] = 4
+
+    # Add the most basic stokes information to the header
+    h['CTYPE4'] = 'STOKES'
+    h['CRVAL4'] = 1.0
+    h['CDELT4'] = 1.0
+    h['CRPIX4'] = 1.0
+    h['CUNIT4'] = ''
+
+    np.random.seed(42)
+    d = np.random.random((4, 4, 3, 2))
+    return d, h
+
+
 @pytest.fixture
 def data_advs(tmp_path):
     d, h = prepare_advs_data()
     fits.writeto(tmp_path / 'advs.fits', d, h)
     return tmp_path / 'advs.fits'
 
 
@@ -134,14 +188,38 @@
     d, h = transpose(d, h, [1, 2, 3, 0])
     d, h = transpose(d, h, [0, 2, 1, 3])
     fits.writeto(tmp_path / 'sdav.fits', d, h)
     return tmp_path / 'sdav.fits'
 
 
 @pytest.fixture
+def data_sdav_beams_nounits(tmp_path):
+    """
+    For testing io when units are not specified
+    (they should be arcsec by default
+    """
+    d, h = prepare_advs_data()
+    d, h = transpose(d, h, [1, 2, 3, 0])
+    d, h = transpose(d, h, [1, 2, 3, 0])
+    d, h = transpose(d, h, [1, 2, 3, 0])
+    d, h = transpose(d, h, [0, 2, 1, 3])
+    del h['BMAJ'], h['BMIN'], h['BPA']
+    # want 4 spectral channels
+    np.random.seed(42)
+    d = np.random.random((4, 3, 2, 1))
+    beams = prepare_4_beams()
+    for ii in (1,2,3):
+        del beams.header[f'TUNIT{ii}']
+    hdul = fits.HDUList([fits.PrimaryHDU(data=d, header=h),
+                         beams])
+    hdul.writeto(tmp_path / 'sdav_beams_nounits.fits')
+    return tmp_path / 'sdav_beams_nounits.fits'
+
+
+@pytest.fixture
 def data_sdav_beams(tmp_path):
     d, h = prepare_advs_data()
     d, h = transpose(d, h, [1, 2, 3, 0])
     d, h = transpose(d, h, [1, 2, 3, 0])
     d, h = transpose(d, h, [1, 2, 3, 0])
     d, h = transpose(d, h, [0, 2, 1, 3])
     del h['BMAJ'], h['BMIN'], h['BPA']
@@ -161,14 +239,29 @@
     del h['BMAJ']
     del h['BMIN']
     del h['BPA']
     fits.writeto(tmp_path / 'advs_nobeam.fits', d, h)
     return tmp_path / 'advs_nobeam.fits'
 
 
+@pytest.fixture
+def data_advs_beams_fullstokes(tmp_path):
+    d, h = prepare_advs_fullstokes_data()
+
+    beams = prepare_4_beams_withfullpol()
+
+    hdu = fits.HDUList()
+    hdu.append(fits.PrimaryHDU(d, h))
+    hdu.append(beams)
+
+    hdu.writeto(tmp_path / 'advs_beams_fullstokes.fits')
+
+    return tmp_path / 'advs_beams_fullstokes.fits'
+
+
 def prepare_adv_data():
     h = fits.header.Header.fromtextfile(HEADER_FILENAME)
     h['BUNIT'] = 'K' # Kelvins are a valid unit, JY/BEAM are not: they should be tested separately
     h['NAXIS1'] = 2
     h['NAXIS2'] = 3
     h['NAXIS3'] = 4
     h['NAXIS'] = 3
```

### Comparing `spectral-cube-0.6.0/spectral_cube/cube_utils.py` & `spectral-cube-0.6.1/spectral_cube/cube_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     # python2
     import __builtin__ as builtins
 
 import dask.array as da
 import numpy as np
 from astropy.wcs.utils import proj_plane_pixel_area
 from astropy.wcs import (WCSSUB_SPECTRAL, WCSSUB_LONGITUDE, WCSSUB_LATITUDE)
+from astropy.wcs import WCS
 from . import wcs_utils
 from .utils import FITSWarning, AstropyUserWarning, WCSCelestialError
 from astropy import log
 from astropy.io import fits
 from astropy.wcs.utils import is_proj_plane_distorted
 from astropy.io.fits import BinTableHDU, Column
 from astropy import units as u
@@ -47,27 +48,31 @@
         for ind,tp in enumerate(types):
             if tp not in ('celestial','stokes'):
                 if wcs.wcs.ctype[ind] in wcs_utils.bad_spectypes_mapping:
                     wcs.wcs.ctype[ind] = wcs_utils.bad_spectypes_mapping[wcs.wcs.ctype[ind]]
 
     return wcs
 
-def _split_stokes(array, wcs):
+def _split_stokes(array, wcs, beam_table=None):
     """
     Given a 4-d data cube with 4-d WCS (spectral cube + stokes) return a
     dictionary of data and WCS objects for each Stokes component
 
     Parameters
     ----------
     array : `~numpy.ndarray`
         The input 3-d array with two position dimensions, one spectral
         dimension, and a Stokes dimension.
     wcs : `~astropy.wcs.WCS`
         The input 3-d WCS with two position dimensions, one spectral
         dimension, and a Stokes dimension.
+    beam_table : `~astropy.io.fits.hdu.table.BinTableHDU`
+        When multiple beams are present, a FITS table with the beam information
+        can be given to be split into the polarization components, consistent with
+        `array`.
     """
 
     if array.ndim not in (3,4):
         raise ValueError("Input array must be 3- or 4-dimensional for a"
                          " STOKES cube")
 
     if wcs.wcs.naxis != 4:
@@ -105,28 +110,42 @@
                           "axis could be identified")
 
     # TODO: make the stokes names more general
     stokes_names = ["I", "Q", "U", "V"]
 
     stokes_arrays = {}
 
+    if beam_table is not None:
+        beam_tables = {}
+
     wcs_slice = wcs_utils.drop_axis(wcs, wcs.naxis - 1 - stokes_index)
 
     if array.ndim == 4:
         for i_stokes in range(array.shape[stokes_index]):
 
             array_slice = [i_stokes if idim == stokes_index else slice(None)
                            for idim in range(array.ndim)]
 
             stokes_arrays[stokes_names[i_stokes]] = array[tuple(array_slice)]
+
+            if beam_table is not None:
+                beam_pol_idx = beam_table['POL'] == i_stokes
+                beam_tables[stokes_names[i_stokes]] = beam_table[beam_pol_idx]
+
     else:
         # 3D array with STOKES as a 4th header parameter
         stokes_arrays['I'] = array
 
-    return stokes_arrays, wcs_slice
+        if beam_table is not None:
+            beam_tables['I'] = beam_table
+
+    if beam_table is not None:
+        return stokes_arrays, wcs_slice, beam_tables
+    else:
+        return stokes_arrays, wcs_slice
 
 
 def _orient(array, wcs):
     """
     Given a 3-d spectral cube and WCS, swap around the axes so that the
     spectral axis cube is the first in Numpy notation, and the last in WCS
     notation.
@@ -481,15 +500,17 @@
     bunit_lower = re.sub(r"\s", "", bunit.lower())
     if bunit_lower == 'jy/beam':
         unit = u.Jy / u.beam
     else:
         try:
             unit = u.Unit(bunit)
         except ValueError:
-            warnings.warn("Could not parse unit {0}".format(bunit),
+            warnings.warn("Could not parse unit {0}. "
+                    "If you know the correct unit, try "
+                    "u.add_enabled_units(u.def_unit(['{0}'], represents=u.<correct_unit>))".format(bunit),
                           AstropyUserWarning)
             unit = None
 
     return unit
 
 
 def world_take_along_axis(cube, position_plane, axis):
@@ -654,18 +675,15 @@
         # Equivalencies for Jy per ang area.
         if has_perangarea:
             bmequiv_angarea = u.brightness_temperature(thisfreq)
 
             this_equivalencies = list(this_equivalencies) + bmequiv_angarea
 
         # Beam area equivalencies for Jy per beam and/or Jy per ang area
-        if has_perbeam or has_perangarea:
-            if not has_beam:
-                raise ValueError("To convert cubes with Jy/beam units, "
-                                "the cube needs to have a beam defined.")
+        if has_perbeam:
 
             # create a beam equivalency for brightness temperature
             bmequiv = beam.jtok_equiv(thisfreq)
 
             # NOTE: `beamarea_equiv` was included in the radio-beam v0.3.3 release
             # The if/else here handles potential cases where earlier releases are installed.
             if hasattr(beam, 'beamarea_equiv'):
@@ -731,7 +749,114 @@
         factors.append(factor)
 
     if has_beams:
         return factors
     else:
         # Slice along first axis to return a 1D array.
         return factors[0]
+
+def combine_headers(header1, header2, **kwargs):
+    '''
+    Given two Header objects, this function returns a fits Header of the optimal wcs.
+
+    Parameters
+    ----------
+    header1 : astropy.io.fits.Header
+        A Header.
+    header2 : astropy.io.fits.Header
+        A Header.
+
+    Returns
+    -------
+    header : astropy.io.fits.Header
+        A header object of a field containing both initial headers.
+
+    '''
+
+    from reproject.mosaicking import find_optimal_celestial_wcs
+
+    # Get wcs and shape of both headers
+    w1 = WCS(header1).celestial
+    s1 = w1.array_shape
+    w2 = WCS(header2).celestial
+    s2 = w2.array_shape
+
+    # Get the optimal wcs and shape for both fields together
+    wcs_opt, shape_opt = find_optimal_celestial_wcs([(s1, w1), (s2, w2)], auto_rotate=False,
+                                                    **kwargs)
+
+    # Make a new header using the optimal wcs and information from cubes
+    header = header1.copy()
+    header['NAXIS'] = 3
+    header['NAXIS1'] = shape_opt[1]
+    header['NAXIS2'] = shape_opt[0]
+    header['NAXIS3'] = header1['NAXIS3']
+    header.update(wcs_opt.to_header())
+    header['WCSAXES'] = 3
+    return header
+
+def mosaic_cubes(cubes, spectral_block_size=100, combine_header_kwargs={}, **kwargs):
+    '''
+    This function reprojects cubes onto a common grid and combines them to a single field.
+
+    Parameters
+    ----------
+    cubes : iterable
+        Iterable list of SpectralCube objects to reproject and add together.
+    spectral_block_size : int
+        Block size so that reproject does not run out of memory.
+    combine_header_kwargs : dict
+        Keywords passed to `~reproject.mosaicking.find_optimal_celestial_wcs`
+        via `combine_headers`.
+    Outputs
+    -------
+    cube : SpectralCube
+        A spectral cube with the list of cubes mosaicked together.
+    '''
+
+    cube1 = cubes[0]
+    header = cube1.header
+
+    # Create a header for a field containing all cubes
+    for cu in cubes[1:]:
+        header = combine_headers(header, cu.header, **combine_header_kwargs)
+
+    # Prepare an array and mask for the final cube
+    shape_opt = (header['NAXIS3'], header['NAXIS2'], header['NAXIS1'])
+    final_array = np.zeros(shape_opt)
+    mask_opt = np.zeros(shape_opt[1:])
+
+    for cube in cubes:
+        # Reproject cubes to the header
+        try:
+            if spectral_block_size is not None:
+                cube_repr = cube.reproject(header,
+                                           block_size=[spectral_block_size,
+                                                       cube.shape[1],
+                                                       cube.shape[2]],
+                                           **kwargs)
+            else:
+                cube_repr = cube.reproject(header, **kwargs)
+        except TypeError:
+            warnings.warn("The block_size argument is not accepted by `reproject`.  "
+                          "A more recent version may be needed.")
+            cube_repr = cube.reproject(header, **kwargs)
+
+        # Create weighting mask (2D)
+        mask = (cube_repr[0:1].get_mask_array()[0])
+        mask_opt += mask.astype(float)
+
+        # Go through each slice of the cube, add it to the final array
+        for ii in range(final_array.shape[0]):
+            slice1 = np.nan_to_num(cube_repr.unitless_filled_data[ii])
+            final_array[ii] = final_array[ii] + slice1
+
+    # Dividing by the mask throws errors where it is zero
+    with np.errstate(divide='ignore'):
+
+        # Use weighting mask to average where cubes overlap
+        for ss in range(final_array.shape[0]):
+            final_array[ss] /= mask_opt
+
+    # Create Cube
+    cube = cube1.__class__(data=final_array * cube1.unit, wcs=WCS(header))
+    return cube
```

### Comparing `spectral-cube-0.6.0/spectral_cube/dask_spectral_cube.py` & `spectral-cube-0.6.1/spectral_cube/dask_spectral_cube.py`

 * *Files 2% similar despite different names*

```diff
@@ -316,14 +316,21 @@
 
     def __repr__(self):
         default_repr = super().__repr__()
         lines = default_repr.splitlines()
         lines[0] = lines[0][:-1] + ' and chunk size {0}:'.format(self._data.chunksize)
         return '\n'.join(lines)
 
+    def display_dask_array(self):
+        try:
+            from IPython.display import display
+            return display(self._data)
+        except ImportError:
+            warnings.warn("Requires IPython to display.")
+
     @add_save_to_tmp_dir_option
     def rechunk(self, chunks='auto', threshold=None, block_size_limit=None,
                 **kwargs):
         """
         Rechunk the underlying dask array and return a new cube.
 
         For more details about the parameters below, see the dask documentation
@@ -598,22 +605,21 @@
 
         else:
             data = self._get_filled_data(fill=self._fill_value)
             # apply_along_axis returns an array with a single chunk, but we
             # need to rechunk here to avoid issues when writing out the data
             # even if it results in a poorer performance.
             data = data.rechunk((-1, 'auto', 'auto'))
-            newdata = da.apply_along_axis(wrapper, 0, data, shape=(self.shape[0],))
+            newdata = da.apply_along_axis(wrapper, 0, data, shape=(self.shape[0],),
+                                          **kwargs)
 
             if return_new_cube:
-                return self._new_cube_with(data=newdata,
-                                        wcs=self.wcs,
-                                        mask=self.mask,
-                                        meta=self.meta,
-                                        fill_value=self.fill_value)
+                return self._new_cube_with(data=newdata, wcs=self.wcs,
+                                           mask=self.mask, meta=self.meta,
+                                           fill_value=self.fill_value)
             else:
                 return newdata
 
 
     @projection_if_needed
     @ignore_warnings
     def sum(self, axis=None, **kwargs):
@@ -756,28 +762,26 @@
 
         The names for each statistic are adopted from CASA's ia.statistics
         (see https://casa.nrao.edu/Release4.1.0/doc/CasaRef/image.statistics.html)
         """
 
         data = self._get_filled_data(fill=np.nan)
 
-        try:
-            from bottleneck import nanmin, nanmax, nansum
-        except ImportError:
-            from numpy import nanmin, nanmax, nansum
-
         def compute_stats(chunk, *args):
-            return np.array([np.sum(~np.isnan(chunk)),
-                             nanmin(chunk),
-                             nanmax(chunk),
-                             nansum(chunk),
-                             nansum(chunk * chunk)])
+            # NOTE: we used to but do not use bottleneck here anymore, as it
+            # does not seem to provide any performance improvements and also
+            # has a memory leak when dealing with >f4 dtypes.
+            return np.array([[[[np.sum(~np.isnan(chunk)),
+                                np.nanmin(chunk),
+                                np.nanmax(chunk),
+                                np.nansum(chunk),
+                                np.nansum(chunk * chunk)]]]])
 
         with dask.config.set(**self._scheduler_kwargs):
-            results = da.map_blocks(compute_stats, data.reshape(-1)).compute()
+            results = da.map_blocks(compute_stats, data, new_axis=3).compute()
 
         count_values, min_values, max_values, sum_values, ssum_values = results.reshape((-1, 5)).T
 
         stats = {'npts': count_values.sum(),
                  'min': min_values.min() * self._unit,
                  'max': max_values.max() * self._unit,
                  'sum': sum_values.sum() * self._unit,
@@ -893,22 +897,32 @@
             kernel_3d = kernel.array.reshape((len(kernel.array), 1, 1))
             return convolve(array, kernel_3d, normalize_kernel=True)
 
         return self.apply_function_parallel_spectral(spectral_smooth,
                                                      accepts_chunks=True)
 
     @add_save_to_tmp_dir_option
-    def spectral_smooth_median(self, ksize, raise_error_jybm=True, **kwargs):
+    def spectral_smooth_median(self, ksize, raise_error_jybm=True,
+                               filter=ndimage.median_filter, **kwargs):
+        return self.spectral_filter(ksize, filter=filter,
+                                    raise_error_jybm=raise_error_jybm,
+                                    **kwargs)
+
+    @add_save_to_tmp_dir_option
+    def spectral_filter(self, ksize, filter, raise_error_jybm=True,
+                        **kwargs):
         """
-        Smooth the cube along the spectral dimension
+        Smooth the cube along the spectral dimension using a scipy.ndimage filter.
 
         Parameters
         ----------
         ksize : int
-            Size of the median filter (scipy.ndimage.filters.median_filter)
+            Size of the median filter in spectral channels (scipy.ndimage.median_filter).
+        filter : function
+            A filter from `scipy.ndimage <https://docs.scipy.org/doc/scipy/reference/ndimage.html#filters>`_.
         save_to_tmp_dir : bool
             If `True`, the computation will be carried out straight away and
             saved to a temporary directory. This can improve performance,
             especially if carrying out several operations sequentially. If
             `False`, the computation is only carried out when accessing
             specific parts of the data or writing to disk.
         kwargs : dict
@@ -920,15 +934,15 @@
 
         if float(ksize).is_integer():
             ksize = int(ksize)
         else:
             raise TypeError('ksize should be an integer (got {0})'.format(ksize))
 
         def median_filter_wrapper(img, **kwargs):
-            return ndimage.median_filter(img, (ksize, 1, 1), **kwargs)
+            return filter(img, (ksize, 1, 1), **kwargs)
 
         return self.apply_function_parallel_spectral(median_filter_wrapper,
                                                      accepts_chunks=True)
 
     @add_save_to_tmp_dir_option
     def spatial_smooth(self, kernel, convolve=convolution.convolve, raise_error_jybm=True, **kwargs):
         """
@@ -959,39 +973,49 @@
 
         def convolve_wrapper(data, kernel=None, **kwargs):
             return convolve(data, kernel, normalize_kernel=True, **kwargs)
 
         return self.apply_function_parallel_spatial(convolve_wrapper, kernel=kernel.array)
 
     @add_save_to_tmp_dir_option
-    def spatial_smooth_median(self, ksize, raise_error_jybm=True, **kwargs):
+    def spatial_filter(self, ksize, filter, raise_error_jybm=True, **kwargs):
         """
         Smooth the image in each spatial-spatial plane of the cube using a median filter.
 
         Parameters
         ----------
         ksize : int
-            Size of the median filter (scipy.ndimage.filters.median_filter)
+            Size of the filter in pixels.
+        filter : function
+            A filter from `scipy.ndimage <https://docs.scipy.org/doc/scipy/reference/ndimage.html#filters>`_.
         raise_error_jybm : bool, optional
             Raises a `~spectral_cube.utils.BeamUnitsError` when smoothing a cube in Jy/beam units,
             since the brightness is dependent on the spatial resolution.
         kwargs : dict
             Passed to the median_filter function
         """
 
         if not SCIPY_INSTALLED:
             raise ImportError("Scipy could not be imported: this function won't work.")
 
         self.check_jybeam_smoothing(raise_error_jybm=raise_error_jybm)
 
         def median_filter_wrapper(data, ksize=None, **kwargs):
-            return ndimage.median_filter(data, ksize, **kwargs)
+            return filter(data, ksize, **kwargs)
 
         return self.apply_function_parallel_spatial(median_filter_wrapper, ksize=ksize)
 
+    def spatial_smooth_median(self, ksize, raise_error_jybm=True,
+            filter=ndimage.median_filter, **kwargs):
+        """
+        Smooth the image in each spatial-spatial plane of the cube using a median filter.
+        """
+        return self.spatial_filter(ksize=ksize, filter=filter,
+                raise_error_jybm=raise_error_jybm, **kwargs)
+
     def moment(self, order=0, axis=0, **kwargs):
         """
         Compute moments along the spectral axis.
 
         Moments are defined as follows:
 
         Moment 0:
@@ -1206,15 +1230,16 @@
 
         return self._new_cube_with(data=data, wcs=newwcs,
                                    mask=BooleanArrayMask(mask, wcs=newwcs))
 
     @add_save_to_tmp_dir_option
     def spectral_interpolate(self, spectral_grid,
                              suppress_smooth_warning=False,
-                             fill_value=None):
+                             fill_value=None,
+                             force_rechunk=True):
         """Resample the cube spectrally onto a specific grid
 
         Parameters
         ----------
         spectral_grid : array
             An array of the spectral positions to regrid onto
         suppress_smooth_warning : bool
@@ -1228,14 +1253,19 @@
             cube.
         save_to_tmp_dir : bool
             If `True`, the computation will be carried out straight away and
             saved to a temporary directory. This can improve performance,
             especially if carrying out several operations sequentially. If
             `False`, the computation is only carried out when accessing
             specific parts of the data or writing to disk.
+        force_rechunk : bool
+            If `True`, forces rechunking of the dask array to have a single chunk
+            along the spectral axis. If `False`, the data will not be rechunked, but
+            a ValueError is raised if rechunking is required to have a single chunk
+            along the spectral axis.
 
         Returns
         -------
         cube : SpectralCube
 
         """
 
@@ -1275,16 +1305,27 @@
         if outdiff > 2 * indiff and not suppress_smooth_warning:
             warnings.warn("Input grid has too small a spacing. The data should "
                           "be smoothed prior to resampling.", SmoothingWarning)
 
         if reverse_in:
             cubedata = cubedata[::-1, :, :]
 
-        cubedata = cubedata.rechunk((-1, 'auto', 'auto'))
-        chunkshape = (len(spectral_grid),) + cubedata.chunksize[1:]
+        if force_rechunk:
+            cubedata = cubedata.rechunk((-1, 'auto', 'auto'))
+        else:
+            # There should be one chunk size along the spectral
+            # axis if there is only 1 chunk already defined.
+            # Otherwise, the data needs to be rechunked.
+            if len(cubedata.chunks[0]) > 1:
+                raise ValueError(f"The cube currently has {len(cubedata.chunks[0])} chunks along"
+                                 " the spectral axis but DaskSpectralCube.spectral_interpolate"
+                                 " requires one. Rechunk the data first or enable"
+                                 " `force_rechunk=True`.")
+
+        chunkshape = (len(spectral_grid),) + cubedata.chunks[1:]
 
         def interp_wrapper(y, args):
             if y.size == 1:
                 return y
             else:
                 interp = scipy.interpolate.interp1d(args[1], y.T,
                                                     fill_value=fill_value,
@@ -1395,14 +1436,17 @@
         else:
             beam_ratio_factor = 1.
 
         # See #631: kwargs get passed within self.apply_function_parallel_spatial
         def convfunc(img, **kwargs):
             return convolve(img, kernel, normalize_kernel=True, **kwargs).reshape(img.shape) * beam_ratio_factor
 
+        if convolve is convolution.convolve_fft and 'allow_huge' not in kwargs:
+            kwargs['allow_huge'] = self.allow_huge_operations
+
         return self.apply_function_parallel_spatial(convfunc,
                                                     accepts_chunks=True,
                                                     **kwargs).with_beam(beam, raise_error_jybm=False)
 
 
 class DaskVaryingResolutionSpectralCube(DaskSpectralCubeMixin, VaryingResolutionSpectralCube):
 
@@ -1524,15 +1568,15 @@
                     beams.append(None)
                     beam_ratio_factors.append(None)
                 else:
                     raise
 
         # We need to pass in the beams to dask, so we hide them inside an object array
         # that can then be chunked like the data.
-        beams = da.from_array(np.array(beams, dtype=np.object)
+        beams = da.from_array(np.array(beams, dtype=object)
                               .reshape((len(beams), 1, 1)), chunks=(-1, -1, -1))
 
         needs_beam_ratio = self.unit.is_equivalent(u.Jy / u.beam)
 
         # See #631: kwargs get passed within self.apply_function_parallel_spatial
         def convfunc(img, beam, **kwargs):
             if img.size > 0:
@@ -1540,15 +1584,15 @@
                 for index in range(img.shape[0]):
                     if beam[index, 0, 0] is None:
                         out[index] = img[index]
                     else:
                         kernel = beam[index, 0, 0].as_kernel(pixscale)
                         out[index] = convolve(img[index], kernel, normalize_kernel=True, **kwargs)
 
-                        if needs_beam_ratio:
+                        if needs_beam_ratio and beam_ratio_factors[index] is not None:
                             out[index] *= beam_ratio_factors[index]
 
                 return out
             else:
                 return img
 
         # Rechunk so that there is only one chunk in the image plane
```

### Comparing `spectral-cube-0.6.0/spectral_cube/io/casa_image.py` & `spectral-cube-0.6.1/spectral_cube/io/casa_image.py`

 * *Files 10% similar despite different names*

```diff
@@ -84,15 +84,14 @@
 
     imageinfo = desc['_keywords_']['imageinfo']
 
     if 'perplanebeams' in imageinfo:
         beam_ = {'beams': imageinfo['perplanebeams']}
         beam_['nStokes'] = beam_['beams'].pop('nStokes')
         beam_['nChannels'] = beam_['beams'].pop('nChannels')
-        beam_['beams'] = {key: {'*0': value} for key, value in list(beam_['beams'].items())}
     elif 'restoringbeam' in imageinfo:
         beam_ = imageinfo['restoringbeam']
     else:
         beam_ = {}
 
     wcs = coordsys_to_astropy_wcs(casa_cs)
 
@@ -101,30 +100,35 @@
     if 'major' in beam_:
         beam = Beam(major=u.Quantity(beam_['major']['value'], unit=beam_['major']['unit']),
                     minor=u.Quantity(beam_['minor']['value'], unit=beam_['minor']['unit']),
                     pa=u.Quantity(beam_['positionangle']['value'], unit=beam_['positionangle']['unit']),
                    )
     elif 'beams' in beam_:
         bdict = beam_['beams']
-        if beam_['nStokes'] > 1:
-            raise NotImplementedError()
+
+        stokes_params = desc['_keywords_']['coords']['stokes1']['stokes']
+
         nbeams = len(bdict)
-        assert nbeams == beam_['nChannels']
-        stokesidx = '*0'
+        nchan = beam_['nChannels']
+        assert nbeams == nchan * beam_['nStokes']
+
+        beams = {}
+
+        for ii, stokes_name in enumerate(stokes_params):
 
-        majors = [u.Quantity(bdict['*{0}'.format(ii)][stokesidx]['major']['value'],
-                             bdict['*{0}'.format(ii)][stokesidx]['major']['unit']) for ii in range(nbeams)]
-        minors = [u.Quantity(bdict['*{0}'.format(ii)][stokesidx]['minor']['value'],
-                             bdict['*{0}'.format(ii)][stokesidx]['minor']['unit']) for ii in range(nbeams)]
-        pas = [u.Quantity(bdict['*{0}'.format(ii)][stokesidx]['positionangle']['value'],
-                          bdict['*{0}'.format(ii)][stokesidx]['positionangle']['unit']) for ii in range(nbeams)]
-
-        beams = Beams(major=u.Quantity(majors),
-                      minor=u.Quantity(minors),
-                      pa=u.Quantity(pas))
+            majors = [u.Quantity(bdict[f"*{ii*nchan+chan}"]['major']['value'],
+                                 bdict[f"*{ii*nchan+chan}"]['major']['unit']) for chan in range(nchan)]
+            minors = [u.Quantity(bdict[f"*{ii*nchan+chan}"]['minor']['value'],
+                                 bdict[f"*{ii*nchan+chan}"]['minor']['unit']) for chan in range(nchan)]
+            pas = [u.Quantity(bdict[f"*{ii*nchan+chan}"]['positionangle']['value'],
+                              bdict[f"*{ii*nchan+chan}"]['positionangle']['unit']) for chan in range(nchan)]
+
+            beams[stokes_name] = Beams(major=u.Quantity(majors),
+                                       minor=u.Quantity(minors),
+                                       pa=u.Quantity(pas))
     else:
         warnings.warn("No beam information found in CASA image.",
                       BeamWarning)
 
 
     # don't need this yet
     # stokes = get_casa_axis(temp_cs, wanttype="Stokes", skipdeg=False,)
@@ -162,15 +166,16 @@
             mask = BooleanArrayMask(valid, wcs_slice)
         else:
             mask = None
 
         if 'beam' in locals():
             cube = DaskSpectralCube(data, wcs_slice, mask, meta=meta, beam=beam)
         elif 'beams' in locals():
-            cube = DaskVaryingResolutionSpectralCube(data, wcs_slice, mask, meta=meta, beams=beams)
+            cube = DaskVaryingResolutionSpectralCube(data, wcs_slice, mask, meta=meta,
+                                                     beams=beams['I'])
         else:
             cube = DaskSpectralCube(data, wcs_slice, mask, meta=meta)
         # with #592, this is no longer true
         # we've already loaded the cube into memory because of CASA
         # limitations, so there's no reason to disallow operations
         # cube.allow_huge_operations = True
         if mask is not None:
@@ -193,15 +198,15 @@
                 data[component] = DaskSpectralCube(data_, wcs_slice, mask[component],
                                                    meta=meta, beam=beam)
             elif 'beams' in locals():
                 data[component] = DaskVaryingResolutionSpectralCube(data_,
                                                                     wcs_slice,
                                                                     mask[component],
                                                                     meta=meta,
-                                                                    beams=beams)
+                                                                    beams=beams[component])
             else:
                 data[component] = DaskSpectralCube(data_, wcs_slice, mask[component],
                                                    meta=meta)
 
             data[component].allow_huge_operations = True
```

### Comparing `spectral-cube-0.6.0/spectral_cube/io/casa_masks.py` & `spectral-cube-0.6.1/spectral_cube/io/casa_masks.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.0/spectral_cube/io/class_lmv.py` & `spectral-cube-0.6.1/spectral_cube/io/class_lmv.py`

 * *Files 1% similar despite different names*

```diff
@@ -659,15 +659,15 @@
      #!
      #real(kind=8), pointer :: ref(:) => null()
      #real(kind=8), pointer :: val(:) => null()
      #real(kind=8), pointer :: inc(:) => null()
 
     lf.seek(1024)
     real_dims = dims[:ndim]
-    data = np.fromfile(lf, count=np.product(real_dims),
+    data = np.fromfile(lf, count=np.prod(real_dims),
                        dtype='float32').reshape(real_dims[::-1])
     data[data==bval] = np.nan
 
     return data,header
 
 
 io_registry.register_reader('lmv', BaseSpectralCube, load_lmv_cube)
```

### Comparing `spectral-cube-0.6.0/spectral_cube/io/core.py` & `spectral-cube-0.6.1/spectral_cube/io/core.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.0/spectral_cube/io/fits.py` & `spectral-cube-0.6.1/spectral_cube/io/fits.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     SPECTRAL_CUBE_VERSION = 'dev'
 
 from .. import SpectralCube, StokesSpectralCube, LazyMask, VaryingResolutionSpectralCube
 from ..dask_spectral_cube import DaskSpectralCube, DaskVaryingResolutionSpectralCube
 from ..lower_dimensional_structures import LowerDimensionalObject
 from ..spectral_cube import BaseSpectralCube
 from .. import cube_utils
-from ..utils import BeamUnitsError, FITSWarning, FITSReadError, StokesWarning
+from ..utils import FITSWarning, FITSReadError, StokesWarning, BeamWarning
 
 
 def first(iterable):
     return next(iter(iterable))
 
 
 def is_fits(origin, filepath, fileobj, *args, **kwargs):
@@ -98,25 +98,31 @@
             elif isinstance(hdu_item, fits.BinTableHDU):
                 if 'BPA' in hdu_item.data.names:
                     beam_table = hdu_item.data
 
                     # Check that the table has the expected form for beam units:
                     # 1: BMAJ 2: BMIN 3: BPA
                     for i in range(1, 4):
-                        if not f"TUNIT{i}" in hdu_item.header:
-                            raise BeamUnitsError(f"Missing beam units keyword {key}{i}"
-                                                    " in the header.")
+                        key = f"TUNIT{i}"
+                        if key not in hdu_item.header:
+                            warnings.warn(BeamWarning(f"Missing beam units keyword {key}"
+                                                      " in the header."))
 
                     # Read the bmaj/bmin units from the header
                     # (we still assume BPA is degrees because we've never seen an exceptional case)
                     # this will crash if there is no appropriate header info
                     maj_kw = [kw for kw, val in hdu_item.header.items() if val == 'BMAJ'][0]
                     min_kw = [kw for kw, val in hdu_item.header.items() if val == 'BMIN'][0]
-                    maj_unit = hdu_item.header[maj_kw.replace('TTYPE', 'TUNIT')]
-                    min_unit = hdu_item.header[min_kw.replace('TTYPE', 'TUNIT')]
+                    try:
+                        maj_unit = hdu_item.header[maj_kw.replace('TTYPE', 'TUNIT')]
+                        min_unit = hdu_item.header[min_kw.replace('TTYPE', 'TUNIT')]
+                    except KeyError:
+                        # the default units, if unspecified (as from CASA <= 4.7.2, we think), are arcseconds
+                        maj_unit = u.arcsec
+                        min_unit = u.arcsec
 
                     # AIPS uses non-FITS-standard unit names; this catches the
                     # only case we've seen so far
                     if maj_unit == 'DEGREES':
                         maj_unit = 'degree'
                     if min_unit == 'DEGREES':
                         min_unit = 'degree'
@@ -220,29 +226,32 @@
             # check that the shape matches if there is a shape
             # it is possible that VaryingResolution cubes will have a composite
             # mask instead
             assert cube._data.shape == cube._mask._data.shape
 
     elif wcs.wcs.naxis == 4:
 
-        data, wcs = cube_utils._split_stokes(data, wcs)
+        if beam_table is None:
+            data, wcs = cube_utils._split_stokes(data, wcs)
+        else:
+            data, wcs, beam_tables = cube_utils._split_stokes(data, wcs, beam_table=beam_table)
 
         stokes_data = {}
         for component in data:
             comp_data, comp_wcs = cube_utils._orient(data[component], wcs)
             comp_mask = LazyMask(np.isfinite, data=comp_data, wcs=comp_wcs)
             if beam_table is None:
                 stokes_data[component] = SC(comp_data, wcs=comp_wcs,
                                             mask=comp_mask, meta=meta,
                                             header=header)
             else:
                 stokes_data[component] = VRSC(comp_data, wcs=comp_wcs,
                                               mask=comp_mask, meta=meta,
                                               header=header,
-                                              beam_table=beam_table,
+                                              beam_table=beam_tables[component],
                                               major_unit=beam_units[0],
                                               minor_unit=beam_units[1]
                                              )
 
         cube = StokesSpectralCube(stokes_data)
 
     else:
```

### Comparing `spectral-cube-0.6.0/spectral_cube/lower_dimensional_structures.py` & `spectral-cube-0.6.1/spectral_cube/lower_dimensional_structures.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,23 +29,30 @@
 
 __all__ = ['LowerDimensionalObject', 'Projection', 'Slice', 'OneDSpectrum']
 class LowerDimensionalObject(u.Quantity, BaseNDClass, HeaderMixinClass):
     """
     Generic class for 1D and 2D objects.
     """
 
+    def _new_view(self, obj=None, unit=None, finalize=True):
+        # FORCE finalization to hack around https://github.com/astropy/astropy/issues/14514#issuecomment-1463935711
+        try:
+            return super(LowerDimensionalObject, self)._new_view(obj=obj, unit=unit, finalize=True)
+        except TypeError:
+            return super(LowerDimensionalObject, self)._new_view(obj=obj, unit=unit)
+
     @property
     def hdu(self):
         if self.wcs is None:
             hdu = PrimaryHDU(self.value)
         else:
             hdu = PrimaryHDU(self.value, header=self.header)
         hdu.header['BUNIT'] = self.unit.to_string(format='fits')
 
-        if 'beam' in self.meta:
+        if self.meta is not None and 'beam' in self.meta:
             hdu.header.update(self.meta['beam'].to_header_keywords())
 
         return hdu
 
     def read(self, *args, **kwargs):
         raise NotImplementedError()
 
@@ -242,15 +249,15 @@
                 meta=None, mask=None, header=None, beam=None,
                 fill_value=np.nan, read_beam=False, wcs_tolerance=0.0):
 
         if np.asarray(value).ndim != 2:
             raise ValueError("value should be a 2-d array")
 
         if wcs is not None and wcs.wcs.naxis != 2:
-            raise ValueError("wcs should have two dimension")
+            raise ValueError("wcs should have two dimensions")
 
         self = u.Quantity.__new__(cls, value, unit=unit, dtype=dtype,
                                   copy=copy).view(cls)
         self._wcs = wcs
         self._meta = {} if meta is None else meta
         self._wcs_tolerance = wcs_tolerance
 
@@ -363,21 +370,28 @@
                                  wcs_tolerance=wcs_tolerance or self._wcs_tolerance,
                                  beam=beam,
                                  **kwargs)
 
         return newproj
 
     @staticmethod
-    def from_hdu(hdu):
+    def from_hdu(hdu, ext=0):
         '''
         Return a projection from a FITS HDU.
+
+        Parameters
+        -----------
+        ext : int
+            The integer index to load when given an :class:`astropy.io.fits.HDUList`.
+            Default is 0 (the first HDU in the list.
+
         '''
         if isinstance(hdu, HDUList):
             hdul = hdu
-            hdu = hdul[0]
+            hdu = hdul[ext]
 
         if not len(hdu.data.shape) == 2:
             raise ValueError("HDU must contain two-dimensional data.")
 
         meta = {}
 
         mywcs = wcs.WCS(hdu.header)
@@ -588,15 +602,15 @@
 
         #log.debug("Creating a OneDSpectrum with __new__")
 
         if np.asarray(value).ndim != 1:
             raise ValueError("value should be a 1-d array")
 
         if wcs is not None and wcs.wcs.naxis != 1:
-            raise ValueError("wcs should have two dimension")
+            raise ValueError("wcs should have one dimension")
 
         self = u.Quantity.__new__(cls, value, unit=unit, dtype=dtype,
                                   copy=copy).view(cls)
         self._wcs = wcs
         self._meta = {} if meta is None else meta
         self._wcs_tolerance = wcs_tolerance
 
@@ -621,22 +635,29 @@
     def __repr__(self):
         prefixstr = '<' + self.__class__.__name__ + ' '
         arrstr = np.array2string(self.filled_data[:].value, separator=',',
                                  prefix=prefixstr)
         return '{0}{1}{2:s}>'.format(prefixstr, arrstr, self._unitstr)
 
     @staticmethod
-    def from_hdu(hdu):
+    def from_hdu(hdu, ext=0):
         '''
         Return a OneDSpectrum from a FITS HDU or HDU list.
+
+        Parameters
+        -----------
+        ext : int
+            The integer index to load when given an :class:`astropy.io.fits.HDUList`.
+            Default is 0 (the first HDU in the list.
+
         '''
 
         if isinstance(hdu, HDUList):
             hdul = hdu
-            hdu = hdul[0]
+            hdu = hdul[ext]
         else:
             hdul = HDUList([hdu])
 
         if not len(hdu.data.shape) == 1:
             raise ValueError("HDU must contain one-dimensional data.")
 
         meta = {}
@@ -648,17 +669,19 @@
             meta["BUNIT"] = hdu.header["BUNIT"]
         else:
             unit = None
 
         with warnings.catch_warnings():
             warnings.filterwarnings('ignore', category=FITSWarning)
             beam = cube_utils.try_load_beams(hdul)
-            if hasattr(beam, '__len__'):
+            try:
                 beams = beam
-            else:
+                _ = len(beams)
+            except TypeError:
+                # beam is scalar and has no len()
                 beams = None
 
         if beams is not None:
             self = VaryingResolutionOneDSpectrum(hdu.data, unit=unit,
                                                  wcs=mywcs, meta=meta,
                                                  header=hdu.header,
                                                  beams=beams)
```

### Comparing `spectral-cube-0.6.0/spectral_cube/masks.py` & `spectral-cube-0.6.1/spectral_cube/masks.py`

 * *Files 0% similar despite different names*

```diff
@@ -221,15 +221,15 @@
         Notes
         -----
         This is an internal method used by :class:`SpectralCube`.
         Users should use the property :meth:`MaskBase.filled_data`
         """
         # Must convert to floating point, but should not change from inherited
         # type otherwise
-        dt = np.find_common_type([data.dtype], [float])
+        dt = np.result_type([data.dtype, 0.0])
 
         if use_memmap and data.size > 0:
             ntf = tempfile.NamedTemporaryFile()
             sliced_data = np.memmap(ntf, mode='w+', shape=data[view].shape,
                                     dtype=dt)
             sliced_data[:] = data[view]
         else:
@@ -258,15 +258,15 @@
 
     @property
     def ndim(self):
         return len(self.shape)
 
     @property
     def size(self):
-        return np.product(self.shape)
+        return np.prod(self.shape)
 
     @property
     def dtype(self):
         return np.dtype('bool')
 
     def __getitem__(self):
         raise NotImplementedError("Slicing not supported by mask class {0}"
```

### Comparing `spectral-cube-0.6.0/spectral_cube/np_compat.py` & `spectral-cube-0.6.1/spectral_cube/np_compat.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.0/spectral_cube/spectral_axis.py` & `spectral-cube-0.6.1/spectral_cube/spectral_axis.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.0/spectral_cube/spectral_cube.py` & `spectral-cube-0.6.1/spectral_cube/spectral_cube.py`

 * *Files 1% similar despite different names*

```diff
@@ -254,16 +254,14 @@
                 unit = u.Unit(unit)
 
             if hasattr(data, 'unit'):
                 if u.Unit(unit) != data.unit:
                     raise u.UnitsError("The specified new cube unit '{0}' "
                                        "does not match the input unit '{1}'."
                                        .format(unit, data.unit))
-            else:
-                data = u.Quantity(data, unit=unit, copy=False)
         elif self._unit is not None:
             unit = self.unit
 
         wcs = self._wcs if wcs is None else wcs
         mask = self._mask if mask is None else mask
         if meta is None:
             meta = {}
@@ -899,38 +897,60 @@
         # x,y are defined as first,second dim to iterate over
         # (not x,y in pixel space...)
         nx = self.shape[iteraxes[0]]
         ny = self.shape[iteraxes[1]]
         return nx, ny
 
     @warn_slow
-    def _apply_everywhere(self, function, *args):
+    def _apply_everywhere(self, function, *args, check_units=True):
         """
         Return a new cube with ``function`` applied to all pixels
 
         Private because this doesn't have an obvious and easy-to-use API
 
+        Parameters
+        ----------
+        function : function
+            An operator that takes the data (self) and any number of additional
+            arguments
+        check_units : bool
+            When doing the initial test before running the full operation,
+            should units be included on the 'fake' test quantity?  This is
+            specifically added as an option to enable using the subtraction and
+            addition operators without checking unit compatibility here because
+            they _already_ enforce unit compatibility.
+
         Examples
         --------
         >>> newcube = cube.apply_everywhere(np.add, 0.5*u.Jy)
         """
 
         try:
-            test_result = function(np.ones([1,1,1])*self.unit, *args)
+            if check_units:
+                test_result = function(np.ones([1,1,1])*self.unit, *args)
+                new_unit = test_result.unit
+            else:
+                test_result = function(np.ones([1,1,1]), *args)
+                new_unit = self.unit
             # First, check that function returns same # of dims?
             assert test_result.ndim == 3,"Output is not 3-dimensional"
         except Exception as ex:
             raise AssertionError("Function could not be applied to a simple "
                                  "cube.  The error was: {0}".format(ex))
 
-        data = function(u.Quantity(self._get_filled_data(fill=self._fill_value),
-                                   self.unit, copy=False),
-                        *args)
+        # We don't need to convert to a quantity here because the shape check
+        data_in = self._get_filled_data(fill=self._fill_value)
+        data = function(data_in, *args)
+
+        # strip the unit because data_in does not have a unit
+        # (we calculate the appropriate unit above and pass it on below)
+        if hasattr(data, 'unit'):
+            data = data.value
 
-        return self._new_cube_with(data=data, unit=data.unit)
+        return self._new_cube_with(data=data, unit=new_unit)
 
     @warn_slow
     def _cube_on_cube_operation(self, function, cube, equivalencies=[], **kwargs):
         """
         Apply an operation between two cubes.  Inherits the metadata of the
         left cube.
 
@@ -1016,14 +1036,15 @@
             ``unit``.  If ``axis`` is None, the return will be a scalar with or
             without units.  If axis is an integer, the return will be a
             :class:`~spectral_cube.lower_dimensional_structures.Projection` if ``projection`` is set
         """
         if axis is None:
             out = function(self.flattened(), **kwargs)
             if unit is not None:
+                # return is scalar
                 return u.Quantity(out, unit=unit)
             else:
                 return out
         if hasattr(axis, '__len__'):
             raise NotImplementedError("`apply_function` does not support "
                                       "function application across multiple "
                                       "axes.  Try `apply_numpy_function`.")
@@ -1788,14 +1809,20 @@
             to convert the units of the spectral axis.
         """
 
         # Find range of values for spectral axis
         ilo = self.closest_spectral_channel(lo)
         ihi = self.closest_spectral_channel(hi)
 
+        if ilo == ihi:
+            warnings.warn("The maxmimum and minimum spectral channel in the spectral"
+                          "slab are identical; this indicates that one or both are "
+                          "likely incorrect and/or out of range.",
+                          SliceWarning)
+
         if ilo > ihi:
             ilo, ihi = ihi, ilo
         ihi += 1
 
         # Create WCS slab
         wcs_slab = self._wcs.deepcopy()
         wcs_slab.wcs.crpix[2] -= ilo
@@ -1992,15 +2019,18 @@
         allow_empty: bool
             If this is False, an exception will be raised if the region
             contains no overlap with the cube
         """
         import regions
 
         if isinstance(ds9_region, six.string_types):
-            region_list = regions.DS9Parser(ds9_region).shapes.to_regions()
+            if hasattr(regions, 'DS9Parser'):
+                region_list = regions.DS9Parser(ds9_region).shapes.to_regions()
+            else:
+                region_list = regions.Regions.read(ds9_region)
         else:
             raise TypeError("{0} should be a DS9 string".format(ds9_region))
 
         return self.subcube_from_regions(region_list, allow_empty)
 
     def subcube_from_crtfregion(self, crtf_region, allow_empty=False):
         """
@@ -2019,26 +2049,33 @@
         if isinstance(crtf_region, six.string_types):
             region_list = regions.CRTFParser(crtf_region).shapes.to_regions()
         else:
             raise TypeError("{0} should be a CRTF string".format(crtf_region))
 
         return self.subcube_from_regions(region_list, allow_empty)
 
-    def subcube_from_regions(self, region_list, allow_empty=False):
+    def subcube_from_regions(self, region_list, allow_empty=False,
+                             minimize=True):
         """
         Extract a masked subcube from a list of ``regions.Region`` object
         (only functions on celestial dimensions)
 
         Parameters
         ----------
         region_list: ``regions.Region`` list
             The region(s) to extract
         allow_empty: bool, optional
             If this is False, an exception will be raised if the region
             contains no overlap with the cube. Default is False.
+        minimize : bool
+            Run :meth:`~SpectralCube.minimal_subcube`.  This is mostly redundant, since the
+            bounding box of the region is already used, but it will sometimes
+            slice off a one-pixel rind depending on the details of the region
+            shape.  If minimize is disabled, there will potentially be a ring
+            of NaN values around the outside.
         """
         import regions
 
         # Convert every region to a `regions.PixelRegion` object.
         regs = []
         for x in region_list:
             if isinstance(x, regions.SkyRegion):
@@ -2086,21 +2123,28 @@
             if allow_empty:
                 warnings.warn("The derived subset is empty: the region does not"
                               " overlap with the cube (but allow_empty=True).")
             else:
                 raise ValueError("The derived subset is empty: the region does not"
                                  " overlap with the cube.")
 
-        # cropping the mask from top left corner so that it fits the subcube.
-        maskarray = mask.data[:subcube.shape[1], :subcube.shape[2]].astype('bool')
+        shp = self.shape[1:]
+        _, slices_small = mask.get_overlap_slices(shp)
+
+        maskarray = np.zeros(subcube.shape[1:], dtype='bool')
+        maskarray[:] = mask.data[slices_small]
 
-        masked_subcube = subcube.with_mask(BooleanArrayMask(maskarray, subcube.wcs, shape=subcube.shape))
+        BAM = BooleanArrayMask(maskarray, subcube.wcs, shape=subcube.shape)
+        masked_subcube = subcube.with_mask(BAM)
         # by using ceil / floor above, we potentially introduced a NaN buffer
         # that we can now crop out
-        return masked_subcube.minimal_subcube(spatial_only=True)
+        if minimize:
+            return masked_subcube.minimal_subcube(spatial_only=True)
+        else:
+            return masked_subcube
 
     def _velocity_freq_conversion_regions(self, ranges, veltypes, restfreqs):
         """
         Makes the spectral range of the regions compatible with the spectral
         convention of the cube.
 
         ranges: `~astropy.units.Quantity` object
@@ -2161,24 +2205,28 @@
 
     def _val_to_own_unit(self, value, operation='compare', tofrom='to',
                          keepunit=False):
         """
         Given a value, check if it has a unit.  If it does, convert to the
         cube's unit.  If it doesn't, raise an exception.
         """
-        if isinstance(value, SpectralCube):
+        if isinstance(value, BaseSpectralCube):
             if self.unit.is_equivalent(value.unit):
                 return value
             else:
                 return value.to(self.unit)
         elif hasattr(value, 'unit'):
             if keepunit:
                 return value.to(self.unit)
             else:
                 return value.to(self.unit).value
+        elif self.unit.is_equivalent(u.dimensionless_unscaled):
+            # if the value is a numpy array or scalar, and the cube has no
+            # unit, no additional conversion is needed
+            return value
         else:
             raise ValueError("Can only {operation} cube objects {tofrom}"
                              " SpectralCubes or Quantities with "
                              "a unit attribute."
                              .format(operation=operation, tofrom=tofrom))
 
     def __gt__(self, value):
@@ -2213,46 +2261,67 @@
         return id(self)
 
     def __ne__(self, value):
         value = self._val_to_own_unit(value)
         return LazyComparisonMask(operator.ne, value, data=self._data, wcs=self._wcs)
 
     def __add__(self, value):
-        if isinstance(value, SpectralCube):
+        if isinstance(value, BaseSpectralCube):
             return self._cube_on_cube_operation(operator.add, value)
         else:
             value = self._val_to_own_unit(value, operation='add', tofrom='from',
-                                          keepunit=True)
-            return self._apply_everywhere(operator.add, value)
+                                          keepunit=False)
+            return self._apply_everywhere(operator.add, value, check_units=False)
 
     def __sub__(self, value):
-        if isinstance(value, SpectralCube):
+        if isinstance(value, BaseSpectralCube):
             return self._cube_on_cube_operation(operator.sub, value)
         else:
             value = self._val_to_own_unit(value, operation='subtract',
-                                          tofrom='from', keepunit=True)
-            return self._apply_everywhere(operator.sub, value)
+                                          tofrom='from', keepunit=False)
+            return self._apply_everywhere(operator.sub, value, check_units=False)
 
     def __mul__(self, value):
-        if isinstance(value, SpectralCube):
+        if isinstance(value, BaseSpectralCube):
             return self._cube_on_cube_operation(operator.mul, value)
         else:
             return self._apply_everywhere(operator.mul, value)
 
     def __truediv__(self, value):
         return self.__div__(value)
 
     def __div__(self, value):
-        if isinstance(value, SpectralCube):
+        if isinstance(value, BaseSpectralCube):
             return self._cube_on_cube_operation(operator.truediv, value)
         else:
             return self._apply_everywhere(operator.truediv, value)
 
+    def __floordiv__(self, value):
+        raise NotImplementedError("Floor-division (division with truncation) "
+                                  "is not supported.")
+        #if isinstance(value, BaseSpectralCube):
+        #    # (Pdb) operator.floordiv(u.K, u.K)
+        #    # *** TypeError: unsupported operand type(s) for //: 'IrreducibleUnit' and 'IrreducibleUnit'
+        #    return self._cube_on_cube_operation(operator.floordiv, value)
+        #else:
+        #    # only cube-on-cube division allowed
+        #    #
+        #    # we don't support this:
+        #    # (Pdb) np.array([5,5,5])*u.K // (2*u.K)
+        #    # <Quantity [2., 2., 2.]>
+        #    # astropy doesn't support this:
+        #    # >>> np.array([5,5,5])*u.K // (2*u.Jy)
+        #    # astropy.units.core.UnitConversionError: Can only apply 'floor_divide' function to quantities with compatible dimensions
+        #    # >>> np.array([5,5,5])*u.K // (np.array([2])*u.Jy)
+        #    # astropy.units.core.UnitConversionError: Can only apply 'floor_divide' function to quantities with compatible dimensions
+        #    raise NotImplementedError("Floor-division (division with truncation) "
+        #                              "is not supported.")
+
     def __pow__(self, value):
-        if isinstance(value, SpectralCube):
+        if isinstance(value, BaseSpectralCube):
             return self._cube_on_cube_operation(operator.pow, value)
         else:
             return self._apply_everywhere(operator.pow, value)
 
     def to_yt(self, spectral_factor=1.0, nprocs=None, **kwargs):
         """
         Convert a spectral cube to a yt object that can be further analyzed in
@@ -2263,15 +2332,15 @@
         spectral_factor : float, optional
             Factor by which to stretch the spectral axis. If set to 1, one pixel
             in spectral coordinates is equivalent to one pixel in spatial
             coordinates.
 
         If using yt 3.0 or later, additional keyword arguments will be passed
         onto yt's ``FITSDataset`` constructor. See the yt documentation
-        (http://yt-project.org/docs/3.0/examining/loading_data.html?#fits-data)
+        (http://yt-project.org/doc/examining/loading_data.html?#fits-data)
         for details on options for reading FITS data.
         """
 
         import yt
 
         if (('dev' in yt.__version__) or
             (LooseVersion(yt.__version__) >= LooseVersion('3.0'))):
@@ -2308,15 +2377,15 @@
                 ds.quan(1.0,units)
             except UnitParseError:
                 raise RuntimeError("The unit %s was not parsed by yt. " % units+
                                    "Check to make sure it is correct.")
 
         else:
 
-            from yt.mods import load_uniform_grid
+            from yt import load_uniform_grid
 
             data = {'flux': self._get_filled_data(fill=0.).transpose()}
 
             nz, ny, nx = self.shape
 
             if nprocs is None:
                 nprocs = 1
@@ -2455,15 +2524,15 @@
 
     @property
     def hdu(self):
         """
         HDU version of self
         """
         log.debug("Creating HDU")
-        hdu = PrimaryHDU(self.filled_data[:].value, header=self.header)
+        hdu = PrimaryHDU(self.unitless_filled_data[:], header=self.header)
         return hdu
 
     @property
     def hdulist(self):
         return HDUList(self.hdu)
 
     @warn_slow
@@ -2537,15 +2606,15 @@
 
         result = Splatalogue.query_lines(numin, numax, **kwargs)
 
         return result
 
     @warn_slow
     def reproject(self, header, order='bilinear', use_memmap=False,
-                  filled=True):
+                  filled=True, **kwargs):
         """
         Spatially reproject the cube into a new header.  Fills the data with
         the cube's ``fill_value`` to replace bad values before reprojection.
 
         If you want to reproject a cube both spatially and spectrally, you need
         to use `spectral_interpolate` as well.
 
@@ -2574,31 +2643,34 @@
             If specified, a memory mapped temporary file on disk will be
             written to rather than storing the intermediate spectra in memory.
         filled : bool
             Fill the masked values with the cube's fill value before
             reprojection?  Note that setting ``filled=False`` will use the raw
             data array, which can be a workaround that prevents loading large
             data into memory.
+        kwargs : dict
+            Passed to `reproject.reproject_interp`.
         """
 
         try:
             from reproject.version import version
         except ImportError:
             raise ImportError("Requires the reproject package to be"
                               " installed.")
 
+        reproj_kwargs = kwargs
         # Need version > 0.2 to work with cubes, >= 0.5 for memmap
         from distutils.version import LooseVersion
         if LooseVersion(version) < "0.5":
             raise Warning("Requires version >=0.5 of reproject. The current "
                           "version is: {}".format(version))
         elif LooseVersion(version) >= "0.6":
-            reproj_kwargs = {}
+            pass # no additional kwargs, no warning either
         else:
-            reproj_kwargs = {'independent_celestial_slices': True}
+            reproj_kwargs['independent_celestial_slices'] = True
 
         from reproject import reproject_interp
 
         # TODO: Find the minimal subcube that contains the header and only reproject that
         # (see FITS_tools.regrid_cube for a guide on how to do this)
 
         newwcs = wcs.WCS(header)
@@ -2625,32 +2697,67 @@
         newcube, newcube_valid = reproject_interp((data,
                                                    self.header),
                                                   newwcs,
                                                   output_array=outarray,
                                                   shape_out=shape_out,
                                                   order=order,
                                                   **reproj_kwargs)
+        if np.all(np.isnan(newcube)):
+            raise ValueError("All values in reprojected cube are nan.  This can be caused"
+                             " by an error in which coordinates do not 'round-trip'.  Try "
+                             "setting ``roundtrip_coords=False``.  You might also check "
+                             "whether the WCS transformation produces valid pixel->world "
+                             "and world->pixel coordinates in each axis."
+                             )
 
         return self._new_cube_with(data=newcube,
                                    wcs=newwcs,
                                    mask=BooleanArrayMask(newcube_valid.astype('bool'),
                                                          newwcs),
                                    meta=self.meta,
                                   )
 
 
     @parallel_docstring
-    def spatial_smooth_median(self, ksize, update_function=None, raise_error_jybm=True, **kwargs):
+    def spatial_smooth_median(self, ksize, update_function=None, raise_error_jybm=True,
+                              filter=ndimage.median_filter, **kwargs):
         """
         Smooth the image in each spatial-spatial plane of the cube using a median filter.
 
         Parameters
         ----------
         ksize : int
-            Size of the median filter (scipy.ndimage.filters.median_filter)
+            Size of the median filter in pixels (scipy.ndimage.median_filter)
+        filter : function
+            A filter from scipy.ndimage. The default is the median filter.
+        update_function : method
+            Method that is called to update an external progressbar
+            If provided, it disables the default `astropy.utils.console.ProgressBar`
+        raise_error_jybm : bool, optional
+            Raises a `~spectral_cube.utils.BeamUnitsError` when smoothing a cube in Jy/beam units,
+            since the brightness is dependent on the spatial resolution.
+        kwargs : dict
+            Passed to the convolve function
+        """
+        return self.spatial_filter(ksize=ksize, filter=filter,
+                                   update_function=update_function,
+                                   raise_error_jybm=raise_error_jybm, **kwargs)
+
+
+    @parallel_docstring
+    def spatial_filter(self, ksize, filter, update_function=None, raise_error_jybm=True, **kwargs):
+        """
+        Smooth the image in each spatial-spatial plane of the cube using a scipy.ndimage filter.
+
+        Parameters
+        ----------
+        ksize : int
+            Size of the filter in pixels (scipy.ndimage.*_filter).
+        filter : function
+            A filter from `scipy.ndimage <https://docs.scipy.org/doc/scipy/reference/ndimage.html#filters>`_.
         update_function : method
             Method that is called to update an external progressbar
             If provided, it disables the default `astropy.utils.console.ProgressBar`
         raise_error_jybm : bool, optional
             Raises a `~spectral_cube.utils.BeamUnitsError` when smoothing a cube in Jy/beam units,
             since the brightness is dependent on the spatial resolution.
         kwargs : dict
@@ -2658,15 +2765,15 @@
         """
         if not scipyOK:
             raise ImportError("Scipy could not be imported: this function won't work.")
 
         self.check_jybeam_smoothing(raise_error_jybm=raise_error_jybm)
 
         def _msmooth_image(im, **kwargs):
-            return ndimage.filters.median_filter(im, size=ksize, **kwargs)
+            return filter(im, size=ksize, **kwargs)
 
         newcube = self.apply_function_parallel_spatial(_msmooth_image,
                                                        **kwargs)
 
         return newcube
 
     @parallel_docstring
@@ -2702,36 +2809,63 @@
 
         newcube = self.apply_function_parallel_spatial(_gsmooth_image,
                                                        **kwargs)
 
         return newcube
 
     @parallel_docstring
+    def spectral_filter(self, ksize, filter, use_memmap=True, verbose=0,
+            num_cores=None, **kwargs):
+        """
+        Smooth the cube along the spectral dimension using a scipy.ndimage filter.
+
+        Parameters
+        ----------
+        ksize : int
+            Size of the filter in spectral channels.
+        filter : function
+            A filter from `scipy.ndimage <https://docs.scipy.org/doc/scipy/reference/ndimage.html#filters>`_.
+        """
+        # note: same body as spectral_smooth_median right now, but `filter`
+        # is a required kwarg
+
+        if not scipyOK:
+            raise ImportError("Scipy could not be imported: this function won't work.")
+
+        return self.apply_function_parallel_spectral(function=filter,
+                                                     size=ksize,
+                                                     verbose=verbose,
+                                                     num_cores=num_cores,
+                                                     use_memmap=use_memmap,
+                                                     **kwargs)
+
+    @parallel_docstring
     def spectral_smooth_median(self, ksize,
                                use_memmap=True,
                                verbose=0,
                                num_cores=None,
+                               filter=ndimage.median_filter,
                                **kwargs):
         """
         Smooth the cube along the spectral dimension
 
         Parameters
         ----------
         ksize : int
-            Size of the median filter (scipy.ndimage.filters.median_filter)
+            Size of the median filter (scipy.ndimage.median_filter)
         verbose : int
             Verbosity level to pass to joblib
         kwargs : dict
             Not used at the moment.
         """
 
         if not scipyOK:
             raise ImportError("Scipy could not be imported: this function won't work.")
 
-        return self.apply_function_parallel_spectral(ndimage.filters.median_filter,
+        return self.apply_function_parallel_spectral(function=filter,
                                                      size=ksize,
                                                      verbose=verbose,
                                                      num_cores=num_cores,
                                                      use_memmap=use_memmap,
                                                      **kwargs)
 
     def _apply_function_parallel_base(self,
@@ -2783,25 +2917,25 @@
             report.  The function *must* be picklable if ``parallel==True``.
         kwargs : dict
             Passed to ``function``
         """
 
         if use_memmap:
             ntf = tempfile.NamedTemporaryFile(dir=memmap_dir)
-            outcube = np.memmap(ntf, mode='w+', shape=self.shape, dtype=np.float)
+            outcube = np.memmap(ntf, mode='w+', shape=self.shape, dtype=float)
         else:
             if self._is_huge and not self.allow_huge_operations:
                 raise ValueError("Applying a function without ``use_memmap`` "
                                  "requires loading the whole array into "
                                  "memory *twice*, which can overload the "
                                  "machine's memory for large cubes.  Either "
                                  "set ``use_memmap=True`` or set "
                                  "``cube.allow_huge_operations=True`` to "
                                  "override this restriction.")
-            outcube = np.empty(shape=self.shape, dtype=np.float)
+            outcube = np.empty(shape=self.shape, dtype=float)
 
         if num_cores == 1 and parallel:
             warnings.warn("parallel=True was specified but num_cores=1. "
                           "Joblib will be used to run the task with a "
                           "single thread.")
         elif num_cores is not None and num_cores > 1 and not parallel:
             raise ValueError("parallel execution was not requested, but "
@@ -3209,14 +3343,17 @@
             beam_ratio_factor = 1.
 
         # See #631: kwargs get passed within self.apply_function_parallel_spatial
         def convfunc(img, **kwargs):
             return convolve(img, convolution_kernel, normalize_kernel=True,
                             **kwargs) * beam_ratio_factor
 
+        if convolve is convolution.convolve_fft and 'allow_huge' not in kwargs:
+            kwargs['allow_huge'] = self.allow_huge_operations
+
         newcube = self.apply_function_parallel_spatial(convfunc,
                                                        **kwargs).with_beam(beam, raise_error_jybm=False)
 
 
         return newcube
 
     def mask_channels(self, goodchannels):
@@ -3348,17 +3485,17 @@
 
             # Create a view that will add a blank newaxis at the right spot
             view_newaxis = [slice(None) for ii in range(self.ndim)]
             view_newaxis[axis] = None
             view_newaxis = tuple(view_newaxis)
 
             ntf = tempfile.NamedTemporaryFile()
-            dsarr = np.memmap(ntf, mode='w+', shape=newshape, dtype=np.float)
+            dsarr = np.memmap(ntf, mode='w+', shape=newshape, dtype=float)
             ntf2 = tempfile.NamedTemporaryFile()
-            mask = np.memmap(ntf2, mode='w+', shape=newshape, dtype=np.bool)
+            mask = np.memmap(ntf2, mode='w+', shape=newshape, dtype=bool)
             for ii in progressbar(range(newshape[axis])):
                 view_fulldata = makeslice_local(ii*factor)
                 view_newdata = makeslice_local(ii, nsteps=1)
 
                 to_average = self.unitless_filled_data[view_fulldata]
                 to_anyfy = self.mask[view_fulldata].include()
```

### Comparing `spectral-cube-0.6.0/spectral_cube/tests/data/basic.image/logtable/table.dat` & `spectral-cube-0.6.1/spectral_cube/tests/data/basic.image/logtable/table.dat`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.0/spectral_cube/tests/data/basic.image/logtable/table.f0` & `spectral-cube-0.6.1/spectral_cube/tests/data/basic.image/logtable/table.f0`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.0/spectral_cube/tests/data/basic.image/mask0/table.dat` & `spectral-cube-0.6.1/spectral_cube/tests/data/basic.image/mask0/table.dat`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.0/spectral_cube/tests/data/basic.image/table.dat` & `spectral-cube-0.6.1/spectral_cube/tests/data/basic.image/table.dat`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.0/spectral_cube/tests/data/basic_bigendian.image/logtable/table.dat` & `spectral-cube-0.6.1/spectral_cube/tests/data/basic_bigendian.image/logtable/table.dat`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.0/spectral_cube/tests/data/basic_bigendian.image/logtable/table.f0` & `spectral-cube-0.6.1/spectral_cube/tests/data/basic_bigendian.image/logtable/table.f0`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.0/spectral_cube/tests/data/basic_bigendian.image/mask0/table.dat` & `spectral-cube-0.6.1/spectral_cube/tests/data/basic_bigendian.image/mask0/table.dat`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.0/spectral_cube/tests/data/basic_bigendian.image/table.dat` & `spectral-cube-0.6.1/spectral_cube/tests/data/basic_bigendian.image/table.dat`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.0/spectral_cube/tests/data/cubewcs1.hdr` & `spectral-cube-0.6.1/spectral_cube/tests/data/cubewcs1.hdr`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.0/spectral_cube/tests/data/cubewcs2.hdr` & `spectral-cube-0.6.1/spectral_cube/tests/data/cubewcs2.hdr`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.0/spectral_cube/tests/data/example_cube.fits` & `spectral-cube-0.6.1/spectral_cube/tests/data/example_cube.fits`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.0/spectral_cube/tests/data/example_cube.lmv` & `spectral-cube-0.6.1/spectral_cube/tests/data/example_cube.lmv`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.0/spectral_cube/tests/data/greisen2006.hdr` & `spectral-cube-0.6.1/spectral_cube/tests/data/greisen2006.hdr`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.0/spectral_cube/tests/data/header_jybeam.hdr` & `spectral-cube-0.6.1/spectral_cube/tests/data/header_jybeam.hdr`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.0/spectral_cube/tests/data/nomask.image/logtable/table.dat` & `spectral-cube-0.6.1/spectral_cube/tests/data/nomask.image/logtable/table.dat`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.0/spectral_cube/tests/data/nomask.image/logtable/table.f0` & `spectral-cube-0.6.1/spectral_cube/tests/data/nomask.image/logtable/table.f0`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.0/spectral_cube/tests/data/nomask.image/table.dat` & `spectral-cube-0.6.1/spectral_cube/tests/data/nomask.image/table.dat`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.0/spectral_cube/tests/helpers.py` & `spectral-cube-0.6.1/spectral_cube/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.0/spectral_cube/tests/test_analysis_functions.py` & `spectral-cube-0.6.1/spectral_cube/tests/test_analysis_functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 import pytest
 import warnings
 import numpy as np
 import astropy.units as u
 # from astropy.modeling import models, fitting
 
-from ..analysis_utilities import stack_spectra, fourier_shift
+from ..analysis_utilities import stack_spectra, fourier_shift, stack_cube
 from .utilities import generate_gaussian_cube, gaussian
 from ..utils import BadVelocitiesWarning
 
 def test_shift():
 
     amp = 1
     v0 = 0 * u.m / u.s
@@ -82,14 +82,60 @@
     #                            atol=1e-3)
 
     # The stacked spectrum should have the same spectral axis
     np.testing.assert_allclose(stacked.spectral_axis.value,
                                test_cube.spectral_axis.value)
 
 
+def test_cube_stacking(use_dask):
+    '''
+    Test passing a list of cubes
+
+    This test simply averages two copies of the same thing.
+
+    A more thorough test might be to verify that cubes with different frequency
+    supports also yield good results.
+    '''
+
+    amp = 1.
+    sigma = 8.
+    noise = None
+    shape = (100, 25, 25)
+
+    test_cube, test_vels = \
+        generate_gaussian_cube(amp=amp, sigma=sigma, noise=noise,
+                               shape=shape, use_dask=use_dask)
+
+    test_cube1 = test_cube.with_spectral_unit(u.GHz, rest_value=1*u.GHz, velocity_convention='radio')
+    test_cube2 = test_cube.with_spectral_unit(u.GHz, rest_value=2*u.GHz, velocity_convention='radio')
+
+    vmin = -10*u.km/u.s
+    vmax = 10*u.km/u.s
+
+    # Stack two cubes
+    stacked = stack_cube([test_cube1, test_cube2], linelist=[1.,2.]*u.GHz,
+                         vmin=vmin, vmax=vmax, average=np.nanmean,
+                         convolve_beam=None, return_cutouts=False)
+
+    np.testing.assert_allclose(stacked.filled_data[:],
+                               test_cube.spectral_slab(vmin, vmax).filled_data[:])
+
+    # Stack one cube with two frequencies, one that's out of band
+    stacked = stack_cube(test_cube1, linelist=[1.,2.]*u.GHz,
+                         vmin=vmin, vmax=vmax, average=np.nanmean,
+                         convolve_beam=None, return_cutouts=False)
+
+    np.testing.assert_allclose(stacked.filled_data[:],
+                               test_cube.spectral_slab(vmin, vmax).filled_data[:])
+
+    # TODO: add tests of multiple lines in the same cube
+    # (this requires a different test cube setup)
+
+
+
 def test_stacking_badvels(use_dask):
     '''
     Regression test for #493: don't include bad velocities when stacking
     '''
 
     amp = 1.
     v0 = 0. * u.km / u.s
```

### Comparing `spectral-cube-0.6.0/spectral_cube/tests/test_casafuncs.py` & `spectral-cube-0.6.1/spectral_cube/tests/test_casafuncs.py`

 * *Files 19% similar despite different names*

```diff
@@ -64,14 +64,51 @@
                         }
             ia.setrestoringbeam(beam=casabdict, channel=channum, polarization=0)
 
         ia.unlock()
         ia.close()
         ia.done()
 
+def make_casa_stokes_testimage(infile, outname):
+
+    infile = str(infile)
+    outname = str(outname)
+
+    if not CASA_INSTALLED:
+        raise Exception("Attempted to make a CASA test image in a non-CASA "
+                        "environment")
+
+    ia = image()
+
+    ia.fromfits(infile=infile, outfile=outname, overwrite=True)
+    ia.unlock()
+    ia.close()
+    ia.done()
+
+    cube = StokesSpectralCube.read(infile)
+    if isinstance(cube.I, VaryingResolutionSpectralCube):
+        ia.open(outname)
+
+        # populate restoring beam emptily
+        ia.setrestoringbeam(remove=True)
+
+        for polnum, comp in enumerate(cube.components):
+
+            for channum, beam in enumerate(cube[comp].beams):
+                casabdict = {'major': {'value':beam.major.to(u.deg).value, 'unit':'deg'},
+                            'minor': {'value':beam.minor.to(u.deg).value, 'unit':'deg'},
+                            'positionangle': {'value':beam.pa.to(u.deg).value, 'unit':'deg'}
+                            }
+
+                ia.setrestoringbeam(beam=casabdict, channel=channum, polarization=polnum)
+
+        ia.unlock()
+        ia.close()
+        ia.done()
+
 
 @pytest.fixture
 def filename(request):
     return request.getfixturevalue(request.param)
 
 
 @pytest.mark.parametrize(('memmap', 'bigendian'), product((False, True), (False, True)))
@@ -277,7 +314,41 @@
 
     assert hasattr(cube, 'beam')
 
     cube_beams = SpectralCube.read(tmp_path / 'casa_adv_beams.image', format='casa_image')
 
     assert hasattr(cube_beams, 'beams')
     assert isinstance(cube_beams, VaryingResolutionSpectralCube)
+
+
+@pytest.mark.skipif(not CASA_INSTALLED, reason='CASA tests must be run in a CASA environment.')
+def test_casa_beams_stokes(data_advs_beams_fullstokes, tmp_path):
+    '''
+    Varying resolution spectral-cube with full Stokes.
+    '''
+
+    # Test both make_casa_testimage and the beam reading tools using casa's
+    # image reader
+
+    cube = StokesSpectralCube.read(data_advs_beams_fullstokes)
+
+    make_casa_stokes_testimage(data_advs_beams_fullstokes,
+                               tmp_path / 'casa_adv_beams_stokes.image')
+
+    casacube = StokesSpectralCube.read(tmp_path / 'casa_adv_beams_stokes.image', format='casa_image')
+
+    for component in 'IQUV':
+
+        cube_component = getattr(cube, component)
+        casacube_component = getattr(casacube, component)
+
+        assert casacube_component.shape == cube_component.shape
+        assert_allclose(casacube_component.unmasked_data[:].value,
+                        cube_component.unmasked_data[:].value)
+
+        assert casacube_component.shape == cube_component.shape
+        assert_allclose(casacube_component.unmasked_data[:].value,
+                        cube_component.unmasked_data[:].value)
+
+        assert casacube_component.beams == cube_component.beams
+
+        assert isinstance(casacube_component, VaryingResolutionSpectralCube)
```

### Comparing `spectral-cube-0.6.0/spectral_cube/tests/test_cube_utils.py` & `spectral-cube-0.6.1/spectral_cube/tests/test_cube_utils.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.0/spectral_cube/tests/test_dask.py` & `spectral-cube-0.6.1/spectral_cube/tests/test_dask.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 # Tests specific to the dask class
 
 import os
 from numpy.core.shape_base import block
 import pytest
 import numpy as np
+from unittest.mock import patch
 
 from numpy.testing import assert_allclose
 from astropy.tests.helper import assert_quantity_allclose
 from astropy import units as u
+from astropy.utils import data
 
 try:
-    from distributed.utils_test import client, loop, cluster_fixture  # noqa
+    from distributed.utils_test import client, loop, cluster_fixture, cleanup, loop_in_thread  # noqa
+    # zarr & fsspec required for writing to disk w/dask
+    import zarr, fsspec  # noqa
     DISTRIBUTED_INSTALLED = True
 except ImportError:
     DISTRIBUTED_INSTALLED = False
 
-from spectral_cube import DaskSpectralCube
+from spectral_cube import DaskSpectralCube, SpectralCube, DaskVaryingResolutionSpectralCube
 from .test_casafuncs import make_casa_testimage
 
 try:
     import casatools
     from casatools import image
     CASA_INSTALLED = True
 except ImportError:
@@ -202,14 +206,77 @@
     # The total shape of test should be the (1,) + cube.shape[1:]
     assert test.shape == cube.shape[1:]
 
     # Test all True
     assert np.all(test.compute())
 
 
+@pytest.mark.parametrize(('accepts_chunks'),
+                         ((True, False)))
+def test_apply_function_parallel_shape(accepts_chunks):
+    # regression test for #772
+
+    def func(x, add=None):
+        if add is not None:
+            y = x + add
+        else:
+            raise ValueError("This test is supposed to have add=1")
+        return y
+
+
+    fn = data.get_pkg_data_filename('tests/data/example_cube.fits', 'spectral_cube')
+    cube = SpectralCube.read(fn, use_dask=True)
+    cube2 = SpectralCube.read(fn, use_dask=False)
+
+    # Check dask w/both threaded and unthreaded
+    rslt3 = cube.apply_function_parallel_spectral(func, add=1,
+                                                  accepts_chunks=accepts_chunks)
+    with cube.use_dask_scheduler('threads', num_workers=4):
+        rslt = cube.apply_function_parallel_spectral(func, add=1,
+                                                     accepts_chunks=accepts_chunks)
+    rslt2 = cube2.apply_function_parallel_spectral(func, add=1)
+
+    np.testing.assert_almost_equal(cube.filled_data[:].value,
+                                   cube2.filled_data[:].value)
+    np.testing.assert_almost_equal(rslt.filled_data[:].value,
+                                   rslt2.filled_data[:].value)
+    np.testing.assert_almost_equal(rslt.filled_data[:].value,
+                                   rslt3.filled_data[:].value)
+
+
+@pytest.mark.parametrize('filename', ('data_adv', 'data_adv_beams',
+    'data_vda_beams', 'data_vda_beams_image'))
+def test_cube_on_cube(filename, request):
+    if 'image' in filename and not CASA_INSTALLED:
+        pytest.skip('Requires CASA to be installed')
+    dataname = request.getfixturevalue(filename)
+
+    # regression test for #782
+    # the regression applies only to VaryingResolutionSpectralCubes
+    # since they are not SpectralCube subclasses
+    cube = DaskSpectralCube.read(dataname)
+    assert isinstance(cube, (DaskSpectralCube, DaskVaryingResolutionSpectralCube))
+    cube2 = SpectralCube.read(dataname, use_dask=False)
+    if 'image' not in filename:
+        # 'image' would be CASA and must be dask
+        assert not isinstance(cube2, (DaskSpectralCube, DaskVaryingResolutionSpectralCube))
+
+    with patch.object(cube, '_cube_on_cube_operation') as mock:
+        cube * cube
+    mock.assert_called_once()
+
+    with patch.object(cube, '_cube_on_cube_operation') as mock:
+        cube * cube2
+    mock.assert_called_once()
+
+    with patch.object(cube2, '_cube_on_cube_operation') as mock:
+        cube2 * cube
+    mock.assert_called_once()
+
+
 if DISTRIBUTED_INSTALLED:
 
     def test_dask_distributed(client, tmpdir):  # noqa
 
         # Make sure that we can use dask distributed. This is a regression test for
         # a bug caused by FilledArrayHandler not being serializable.
```

### Comparing `spectral-cube-0.6.0/spectral_cube/tests/test_io.py` & `spectral-cube-0.6.1/spectral_cube/tests/test_io.py`

 * *Files 13% similar despite different names*

```diff
@@ -71,27 +71,37 @@
 
 def test_4d_beams(data_sdav_beams, use_dask):
     c = SpectralCube.read(data_sdav_beams, use_dask=use_dask)
     np.testing.assert_almost_equal(c.beams[0].major.value, 0.4)
     np.testing.assert_almost_equal(c.beams[0].minor.value, 0.1)
 
 
+def test_4d_beams_nounits(data_sdav_beams_nounits, use_dask):
+    c = SpectralCube.read(data_sdav_beams_nounits, use_dask=use_dask)
+    np.testing.assert_almost_equal(c.beams[0].major.value, 0.4)
+    np.testing.assert_almost_equal(c.beams[0].minor.value, 0.1)
+    assert c.beams[0].major.unit == u.arcsec
+    assert c.beams[0].minor.unit == u.arcsec
+
+
 def test_3d_beams_roundtrip(tmpdir, data_vda_beams, use_dask):
     c = SpectralCube.read(data_vda_beams, use_dask=use_dask)
     np.testing.assert_almost_equal(c.beams[0].major.value, 0.4)
     np.testing.assert_almost_equal(c.beams[0].minor.value, 0.1)
     c.write(tmpdir.join('vda_beams_out.fits').strpath)
     c2 = SpectralCube.read(tmpdir.join('vda_beams_out.fits').strpath, use_dask=use_dask)
 
     # assert c==c2 # this is not implemented?
     assert np.all(c.filled_data[:] == c2.filled_data[:])
     #assert c.wcs == c2.wcs # not implemented correctly?
 
     np.testing.assert_almost_equal(c2.beams[0].major.value, 0.4)
     np.testing.assert_almost_equal(c2.beams[0].minor.value, 0.1)
+    assert c2.beams[0].major.unit == u.arcsec
+    assert c2.beams[0].minor.unit == u.arcsec
 
 
 def test_4d_beams_roundtrip(tmpdir, data_sdav_beams, use_dask):
     # not sure if 4d can round-trip...
     c = SpectralCube.read(data_sdav_beams, use_dask=use_dask)
     np.testing.assert_almost_equal(c.beams[0].major.value, 0.4)
     np.testing.assert_almost_equal(c.beams[0].minor.value, 0.1)
@@ -100,14 +110,17 @@
 
     # assert c==c2 # this is not implemented?
     assert np.all(c.filled_data[:] == c2.filled_data[:])
     #assert c.wcs == c2.wcs # not implemented correctly?
 
     np.testing.assert_almost_equal(c2.beams[0].major.value, 0.4)
     np.testing.assert_almost_equal(c2.beams[0].minor.value, 0.1)
+    assert c2.beams[0].major.unit == u.arcsec
+    assert c2.beams[0].minor.unit == u.arcsec
+
 
 def test_1d(data_5_spectral):
     hdul = pyfits.open(data_5_spectral)
     hdu = hdul[0]
     spec = OneDSpectrum.from_hdu(hdu)
 
     np.testing.assert_almost_equal(spec, np.arange(5, dtype='float'))
@@ -130,7 +143,19 @@
     regression test for #737, AIPS beam unit specs (degrees)
     """
     c = SpectralCube.read(data_455_degree_beams, use_dask=use_dask)
     np.testing.assert_almost_equal(c.beams[0].major.value, 0.4/3600)
     np.testing.assert_almost_equal(c.beams[0].minor.value, 0.1/3600)
     np.testing.assert_almost_equal(c.beams[0].major.to(u.arcsec).value, 0.4)
     np.testing.assert_almost_equal(c.beams[0].minor.to(u.arcsec).value, 0.1)
+
+
+
+def test_vrsc_fullstokes_read_fits(data_advs_beams_fullstokes):
+    '''
+    Test reading a spectral line data cube with full stokes and a beam table.
+    '''
+    c = StokesSpectralCube.read(data_advs_beams_fullstokes)
+
+    for component in ['I', 'Q', 'U', 'V']:
+        assert isinstance(c[component], VaryingResolutionSpectralCube)
+        assert hasattr(c[component], 'beams')
```

### Comparing `spectral-cube-0.6.0/spectral_cube/tests/test_masks.py` & `spectral-cube-0.6.1/spectral_cube/tests/test_masks.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.0/spectral_cube/tests/test_moments.py` & `spectral-cube-0.6.1/spectral_cube/tests/test_moments.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 # In issue 184, the cubes were corrected such that they all have valid units
 # Therefore, no separate tests are needed for moments-with-units and those
 # without
 MOMENTSu = MOMENTS
 
 
 def moment_cube():
-    cube = np.arange(27).reshape([3, 3, 3]).astype(np.float)
+    cube = np.arange(27).reshape([3, 3, 3]).astype(float)
     wcs = WCS(naxis=3)
     wcs.wcs.ctype = ['RA---TAN', 'DEC--TAN', 'VELO']
     # choose values to minimize spherical distortions
     wcs.wcs.cdelt = np.array([-1, 2, 3], dtype='float32') / 1e5
     wcs.wcs.crpix = np.array([1, 1, 1], dtype='float32')
     wcs.wcs.crval = np.array([0, 1e-3, 2e-3], dtype='float32')
     wcs.wcs.cunit = ['deg', 'deg', 'km/s']
```

### Comparing `spectral-cube-0.6.0/spectral_cube/tests/test_performance.py` & `spectral-cube-0.6.1/spectral_cube/tests/test_performance.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.0/spectral_cube/tests/test_projection.py` & `spectral-cube-0.6.1/spectral_cube/tests/test_projection.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,23 @@
 from ..spectral_cube import SpectralCube
 from ..masks import BooleanArrayMask
 from ..lower_dimensional_structures import (Projection, Slice, OneDSpectrum,
                                             VaryingResolutionOneDSpectrum)
 from ..utils import SliceWarning, WCSCelestialError, BeamUnitsError
 from . import path
 
+# needed for regression in numpy
+import sys
+try:
+    from astropy.utils.compat import NUMPY_LT_1_22
+except ImportError:
+    # if astropy is an old version, we'll just skip the test
+    # (this is only used in one place)
+    NUMPY_LT_1_22 = False
+
 # set up for parametrization
 LDOs = (Projection, Slice, OneDSpectrum)
 LDOs_2d = (Projection, Slice,)
 
 two_qty_2d = np.ones((2,2)) * u.Jy
 twelve_qty_2d = np.ones((12,12)) * u.Jy
 two_qty_1d = np.ones((2,)) * u.Jy
@@ -124,15 +133,17 @@
     assert not hasattr(mask, 'unit')
 
 @pytest.mark.parametrize(('LDO', 'data'),
                          zip(LDOs, data_twelve))
 def test_self_arith(LDO, data):
 
     image = data
-    p = LDO(image, copy=False)
+    p = LDO(image, copy=False, wcs=WCS(naxis=image.ndim))
+    assert hasattr(p, '_wcs')
+    assert p.wcs is not None
 
     p2 = p + p
 
     assert hasattr(p2, '_wcs')
     assert p2.wcs == p.wcs
     assert np.all(p2.value==2)
 
@@ -146,29 +157,34 @@
 @pytest.mark.parametrize(('LDO', 'data'),
                          zip(LDOs, data_twelve))
 def test_self_arith_with_beam(LDO, data):
 
     exp_beam = Beam(1.0 * u.arcsec)
 
     image = data
-    p = LDO(image, copy=False)
+    p = LDO(image, copy=False, wcs=WCS(naxis=image.ndim))
     p = p.with_beam(exp_beam)
+    assert hasattr(p, 'beam')
+    assert hasattr(p, '_wcs')
+    assert p.wcs is not None
 
     p2 = p + p
 
     assert hasattr(p2, '_wcs')
     assert p2.wcs == p.wcs
     assert np.all(p2.value==2)
+    assert hasattr(p2, 'beam')
     assert p2.beam == exp_beam
 
     p2 = p - p
 
     assert hasattr(p2, '_wcs')
     assert p2.wcs == p.wcs
     assert np.all(p2.value==0)
+    assert hasattr(p2, 'beam')
     assert p2.beam == exp_beam
 
 
 @pytest.mark.xfail(raises=ValueError, strict=True)
 def test_VRODS_wrong_beams_shape():
     '''
     Check that passing Beams with a different shape than the data
@@ -693,28 +709,34 @@
 
     sp = cube[:-1,0,0]
 
     assert sp.max() == cube[:-1,:,:].max(axis=0)[0,0]
     assert not isinstance(sp.max(), OneDSpectrum)
 
 
+# TODO: Unpin when Numpy bug is resolved.
+@pytest.mark.skipif(not NUMPY_LT_1_22 and sys.platform == 'win32',
+                    reason='https://github.com/numpy/numpy/issues/20699')
 @pytest.mark.parametrize('method',
                          ('min', 'max', 'std', 'mean', 'sum', 'cumsum',
                           'nansum', 'ptp', 'var'),
                         )
 def test_1d_slice_reductions(method, data_255_delta, use_dask):
 
     cube, data = cube_and_raw(data_255_delta, use_dask=use_dask)
 
     sp = cube[:,0,0]
 
     if hasattr(cube, method):
-        assert getattr(sp, method)() == getattr(cube, method)(axis=0)[0,0]
+        spmethod = getattr(sp, method)
+        cubemethod = getattr(cube, method)
+        assert spmethod() == cubemethod(axis=0)[0,0]
     else:
-        getattr(sp, method)()
+        method = getattr(sp, method)
+        result = method()
 
     assert hasattr(sp, '_fill_value')
 
     assert 'OneDSpectrum' in sp.__repr__()
     assert 'OneDSpectrum' in sp[1:-1].__repr__()
 
 
@@ -724,16 +746,19 @@
     sp = cube[:,0,0]
 
     assert all(sp.value.round() == sp.round().value)
 
     assert hasattr(sp, '_fill_value')
     assert hasattr(sp.round(), '_fill_value')
 
-    assert 'OneDSpectrum' in sp.round().__repr__()
-    assert 'OneDSpectrum' in sp[1:-1].round().__repr__()
+    rnd = sp.round()
+    assert 'OneDSpectrum' in rnd.__repr__()
+
+    rndslc = sp[1:-1].round()
+    assert 'OneDSpectrum' in rndslc.__repr__()
 
 
 def test_LDO_arithmetic(data_vda, use_dask):
     cube, data = cube_and_raw(data_vda, use_dask=use_dask)
 
     sp = cube[:,0,0]
 
@@ -909,7 +934,20 @@
 
     # Test world_flattened here, too
     # TODO: Enable once 2D masking is a thing
     w2_flat = plane.flattened_world(view=view)
     for result, expected in zip(w2_flat, world):
         print(result.shape, expected.flatten().shape)
         assert_allclose(result, expected.flatten())
+
+@pytest.mark.parametrize(('LDO', 'data'),
+                         zip(LDOs, data_twelve))
+def test_unit_division(LDO, data):
+    # regression: 871
+
+    image = data
+    p = LDO(image, copy=False)
+
+    p._meta = None
+
+    # check that this does not raise an Exception
+    p.hdu
```

### Comparing `spectral-cube-0.6.0/spectral_cube/tests/test_regrid.py` & `spectral-cube-0.6.1/spectral_cube/tests/test_regrid.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import sys
 import pytest
 import tempfile
 import numpy as np
+import os
 
-from astropy import units as u
+from astropy import constants, units as u
 from astropy import convolution
 from astropy.wcs import WCS
 from astropy import wcs
 from astropy.io import fits
 
 try:
     import tracemalloc
@@ -20,25 +21,30 @@
 from distutils.version import LooseVersion
 
 NPY_VERSION_CHECK = LooseVersion(np.version.version) >= "1.13"
 
 from radio_beam import beam, Beam
 
 from .. import SpectralCube
+from ..masks import BooleanArrayMask
 from ..utils import WCSCelestialError
+from ..cube_utils import mosaic_cubes, combine_headers
 from .test_spectral_cube import cube_and_raw
 from .test_projection import load_projection
 from . import path, utilities
 
 WINDOWS = sys.platform == "win32"
 
 
-def test_convolution(data_255_delta, use_dask):
+@pytest.mark.parametrize('allow_huge_operations', (True, False))
+def test_convolution(data_255_delta, allow_huge_operations, use_dask):
     cube, data = cube_and_raw(data_255_delta, use_dask=use_dask)
 
+    cube.allow_huge_operations = allow_huge_operations
+
     # 1" convolved with 1.5" -> 1.8027....
     target_beam = Beam(1.802775637731995*u.arcsec, 1.802775637731995*u.arcsec,
                        0*u.deg)
 
     conv_cube = cube.convolve_to(target_beam)
 
     expected = convolution.Gaussian2DKernel((1.5*u.arcsec /
@@ -52,17 +58,20 @@
     np.testing.assert_almost_equal(expected.array,
                                    conv_cube.filled_data[0,:,:].value)
 
     # 2nd layer is all zeros
     assert np.all(conv_cube.filled_data[1,:,:] == 0.0)
 
 
-def test_beams_convolution(data_455_delta_beams, use_dask):
+@pytest.mark.parametrize('allow_huge_operations', (True, False))
+def test_beams_convolution(data_455_delta_beams, allow_huge_operations, use_dask):
     cube, data = cube_and_raw(data_455_delta_beams, use_dask=use_dask)
 
+    cube.allow_huge_operations = allow_huge_operations
+
     # 1" convolved with 1.5" -> 1.8027....
     target_beam = Beam(1.802775637731995*u.arcsec, 1.802775637731995*u.arcsec,
                        0*u.deg)
 
     conv_cube = cube.convolve_to(target_beam)
 
     pixscale = wcs.utils.proj_plane_pixel_area(cube.wcs.celestial)**0.5*u.deg
@@ -102,46 +111,74 @@
 
     wcs_in = WCS(cube.header)
     wcs_out = wcs_in.deepcopy()
     wcs_out.wcs.ctype = ['GLON-SIN', 'GLAT-SIN', wcs_in.wcs.ctype[2]]
     wcs_out.wcs.crval = [134.37608, -31.939241, wcs_in.wcs.crval[2]]
     wcs_out.wcs.crpix = [2., 2., wcs_in.wcs.crpix[2]]
 
+    # cube is doppler-optical by default, which uses the rest wavelength,
+    # which isn't auto-computed, resulting in nan pixels in the WCS transform
+    wcs_out.wcs.restwav = 0.21106114549833
+    cube._wcs.wcs.restwav = 0.21106114549833
+
     header_out = cube.header
     header_out['NAXIS1'] = 4
     header_out['NAXIS2'] = 5
     header_out['NAXIS3'] = cube.shape[0]
     header_out.update(wcs_out.to_header())
 
     result = cube.reproject(header_out, use_memmap=use_memmap)
 
     assert result.shape == (cube.shape[0], 5, 4)
+    
+    # empirically, this is how close we can get after https://github.com/astropy/astropy/pull/14508
+    tolerance = 1e-12
+
+    assert wcs_out.wcs.compare(WCS(header_out).wcs, tolerance=tolerance)
     # Check WCS in reprojected matches wcs_out
-    assert wcs_out.wcs.compare(result.wcs.wcs)
+    assert wcs_out.wcs.compare(result.wcs.wcs, tolerance=tolerance)
     # And that the headers have equivalent WCS info.
     result_wcs_from_header = WCS(result.header)
-    assert result_wcs_from_header.wcs.compare(wcs_out.wcs)
+    assert result_wcs_from_header.wcs.compare(wcs_out.wcs, tolerance=tolerance)
 
 
 def test_spectral_smooth(data_522_delta, use_dask):
 
     cube, data = cube_and_raw(data_522_delta, use_dask=use_dask)
 
-    result = cube.spectral_smooth(kernel=convolution.Gaussian1DKernel(1.0), use_memmap=False)
+    kernel = convolution.Gaussian1DKernel(1.0)
+
+    result = cube.spectral_smooth(kernel=kernel, use_memmap=False)
+
+    # check that all values come out right from the cube creation
+    np.testing.assert_almost_equal(cube[2,:,:].value, 1.0)
+    np.testing.assert_almost_equal(cube.unitless_filled_data[:2,:,:], 0.0)
+    np.testing.assert_almost_equal(cube.unitless_filled_data[3:,:,:], 0.0)
+
+    # make sure the kernel comes out right; the convolution test will fail if this is wrong
+    assert kernel.array.size == 9
+    # this was the old astropy normalization
+    # We don't actually need the kernel to match these values, but I'm leaving this here
+    # as a note for future us:
+    # https://github.com/astropy/astropy/pull/13299
+    # the error came about because we were using two different kernel sizes, which resulted in
+    # two different normalizations after the correction in 13299
+    # Before 13299, normalization was not guaranteed.
+    #np.testing.assert_almost_equal(kernel.array[2:-2],
+    #                               np.array([0.05399097, 0.24197072, 0.39894228, 0.24197072, 0.05399097]))
 
     np.testing.assert_almost_equal(result[:,0,0].value,
-                                   convolution.Gaussian1DKernel(1.0,
-                                                                x_size=5).array,
+                                   kernel.array[2:-2],
                                    4)
 
-    result = cube.spectral_smooth(kernel=convolution.Gaussian1DKernel(1.0), use_memmap=True)
+    # second test with memmap=True
+    result = cube.spectral_smooth(kernel=kernel, use_memmap=True)
 
     np.testing.assert_almost_equal(result[:,0,0].value,
-                                   convolution.Gaussian1DKernel(1.0,
-                                                                x_size=5).array,
+                                   kernel.array[2:-2],
                                    4)
 
 def test_catch_kernel_with_units(data_522_delta, use_dask):
     # Passing a kernel with a unit should raise a u.UnitsError
 
     cube, data = cube_and_raw(data_522_delta, use_dask=use_dask)
 
@@ -154,42 +191,41 @@
 @pytest.mark.skipif('WINDOWS')
 def test_spectral_smooth_4cores(data_522_delta):
 
     pytest.importorskip('joblib')
 
     cube, data = cube_and_raw(data_522_delta, use_dask=False)
 
-    result = cube.spectral_smooth(kernel=convolution.Gaussian1DKernel(1.0), num_cores=4, use_memmap=True)
+    kernel = convolution.Gaussian1DKernel(1.0)
+    result = cube.spectral_smooth(kernel=kernel, num_cores=4, use_memmap=True)
 
+    assert kernel.array.size == 9
     np.testing.assert_almost_equal(result[:,0,0].value,
-                                   convolution.Gaussian1DKernel(1.0,
-                                                                x_size=5).array,
+                                   kernel.array[2:-2],
                                    4)
 
     # this is one way to test non-parallel mode
-    result = cube.spectral_smooth(kernel=convolution.Gaussian1DKernel(1.0), num_cores=4, use_memmap=False)
+    result = cube.spectral_smooth(kernel=kernel, num_cores=4, use_memmap=False)
 
     np.testing.assert_almost_equal(result[:,0,0].value,
-                                   convolution.Gaussian1DKernel(1.0,
-                                                                x_size=5).array,
+                                   kernel.array[2:-2],
                                    4)
 
     # num_cores = 4 is a contradiction with parallel=False, so we want to make
     # sure it fails
     with pytest.raises(ValueError,
                        match=("parallel execution was not requested, but "
                                  "multiple cores were: these are incompatible "
                                  "options.  Either specify num_cores=1 or "
                                  "parallel=True")):
-        result = cube.spectral_smooth(kernel=convolution.Gaussian1DKernel(1.0),
+        result = cube.spectral_smooth(kernel=kernel,
                                       num_cores=4, parallel=False)
 
     np.testing.assert_almost_equal(result[:,0,0].value,
-                                   convolution.Gaussian1DKernel(1.0,
-                                                                x_size=5).array,
+                                   kernel.array[2:-2],
                                    4)
 
 
 def test_spectral_smooth_fail(data_522_delta_beams, use_dask):
 
     cube, data = cube_and_raw(data_522_delta_beams, use_dask=use_dask)
 
@@ -214,14 +250,55 @@
 
     np.testing.assert_almost_equal(result[:,0,0].value,
                                    [0.0, 0.5, 0.5, 0.0])
 
     assert cube.wcs.wcs.compare(orig_wcs.wcs)
 
 
+def test_spectral_interpolate_varying_chunksize(data_255_delta):
+
+    cube, data = cube_and_raw(data_255_delta, use_dask=True)
+
+    orig_wcs = cube.wcs.deepcopy()
+
+    # midpoint between each position
+    sg = (cube.spectral_axis[1:] + cube.spectral_axis[:-1])/2.
+
+    # Force unequal chunks
+    cube = cube.rechunk((-1, 2, 2))
+
+    result = cube.spectral_interpolate(spectral_grid=sg, force_rechunk=False)
+
+    np.testing.assert_almost_equal(result[:,2,2].value,
+                                   [0.5])
+
+    assert cube.wcs.wcs.compare(orig_wcs.wcs)
+
+    # Ensure the spatial chunk sizes vary
+    assert cube._data.chunks[1] == (2, 2, 1)
+    assert result._data.chunks[1] == (2, 2, 1)
+
+
+def test_spectral_interpolate_rechunk_fail(data_255_delta):
+
+    cube, data = cube_and_raw(data_255_delta, use_dask=True)
+
+    orig_wcs = cube.wcs.deepcopy()
+
+    # midpoint between each position
+    sg = (cube.spectral_axis[1:] + cube.spectral_axis[:-1])/2.
+
+    # Force >1 chunk in spectral dimension
+    cube = cube.rechunk((1, -1, -1))
+
+    with pytest.raises(ValueError,
+                       match=("The cube currently has 2 chunks along")):
+        cube.spectral_interpolate(spectral_grid=sg, force_rechunk=False)
+
+
 def test_spectral_interpolate_with_fillvalue(data_522_delta, use_dask):
 
     cube, data = cube_and_raw(data_522_delta, use_dask=use_dask)
 
     # Step one channel out of bounds.
     sg = ((cube.spectral_axis[0]) -
           (cube.spectral_axis[1] - cube.spectral_axis[0]) *
@@ -516,7 +593,48 @@
     assert diffvals.max()*u.B <= 1*u.MB #>= 200**3*sz*u.B
     # the peak memory usage *during* reprojection will have that duplicate,
     # but the memory gets cleaned up afterward
     assert (peak_aftr-peak_b4)*u.B >= (200**3*sz*u.B + 200*100**2*sz*u.B)
 
     assert result.wcs.wcs.crval[0] == 0.001
     assert result.wcs.wcs.crpix[0] == 2.
+
+@pytest.mark.parametrize('spectral_block_size,use_memmap', ((None, False),
+                                                            (100, False),
+                                                            (None, True),
+                                                            (100, False),
+                                                            (1, True),
+                                                            (1, False),
+                                                            ))
+def test_mosaic_cubes(use_memmap, data_adv, use_dask, spectral_block_size):
+
+    pytest.importorskip('reproject')
+
+    # Read in data to use
+    cube, data = cube_and_raw(data_adv, use_dask=use_dask)
+
+    # cube is doppler-optical by default, which uses the rest wavelength,
+    # which isn't auto-computed, resulting in nan pixels in the WCS transform
+    cube._wcs.wcs.restwav = constants.c.to(u.m/u.s).value / cube.wcs.wcs.restfrq
+
+    expected_wcs = WCS(combine_headers(cube.header, cube.header)).celestial
+
+    # Make two overlapping cubes of the data
+    part1 = cube[:, :round(cube.shape[1]*2./3.), :]
+    part2 = cube[:, round(cube.shape[1]/3.):, :]
+
+    assert part1.wcs.wcs.restwav != 0
+    assert part2.wcs.wcs.restwav != 0
+
+    result = mosaic_cubes([part1, part2], order='nearest-neighbor',
+                          roundtrip_coords=False,
+                          spectral_block_size=spectral_block_size)
+
+    # Check that the shapes are the same
+    assert result.shape == cube.shape
+
+    # Check WCS in reprojected matches wcs_out
+    # (comparing WCS failed for no reason we could discern)
+    assert repr(expected_wcs) == repr(result.wcs.celestial)
+    # Check that values of original and result are comparable
+    np.testing.assert_almost_equal(result.filled_data[:].value, cube.filled_data[:].value, decimal=3)
+    # only good to 3 decimal places is not amazing...
```

### Comparing `spectral-cube-0.6.0/spectral_cube/tests/test_spectral_axis.py` & `spectral-cube-0.6.1/spectral_cube/tests/test_spectral_axis.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.0/spectral_cube/tests/test_spectral_cube.py` & `spectral-cube-0.6.1/spectral_cube/tests/test_spectral_cube.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from astropy import stats
 from astropy.io import fits
 from astropy import units as u
 from astropy.wcs import WCS
 from astropy.wcs import _wcs
 from astropy.tests.helper import assert_quantity_allclose
 from astropy.convolution import Gaussian2DKernel, Tophat2DKernel
+from astropy.utils.exceptions import AstropyWarning
 import numpy as np
 
 from .. import (BooleanArrayMask,
                 FunctionMask, LazyMask, CompositeMask)
 from ..spectral_cube import (OneDSpectrum, Projection,
                              VaryingResolutionOneDSpectrum,
                              LowerDimensionalObject)
@@ -72,16 +73,14 @@
 try:
     import scipy
     scipyOK = True
 except ImportError:
     scipyOK = False
 
 import os
-# if ON_TRAVIS is set, we're on travis.
-on_travis = bool(os.environ.get('ON_TRAVIS'))
 
 from radio_beam import Beam, Beams
 from radio_beam.utils import BeamError
 
 NUMPY_LT_19 = LooseVersion(np.__version__) < LooseVersion('1.9.0')
 
 
@@ -323,31 +322,56 @@
         assert_allclose(cube_masked_freq._wcs.wcs.crval[cube_masked_freq._wcs.wcs.spec],
                         outcv.to(u.Hz).value)
         assert_allclose(cube_masked_freq._mask._wcs.wcs.crval[cube_masked_freq._mask._wcs.wcs.spec],
                         outcv.to(u.Hz).value)
 
 
     @pytest.mark.parametrize(('operation', 'value'),
-                             ((operator.add, 0.5*u.K),
-                              (operator.sub, 0.5*u.K),
-                              (operator.mul, 0.5*u.K),
+                             ((operator.mul, 0.5*u.K),
                               (operator.truediv, 0.5*u.K),
-                              (operator.div if hasattr(operator,'div') else operator.floordiv, 0.5*u.K),
                              ))
     def test_apply_everywhere(self, operation, value, data_advs, use_dask):
         c1, d1 = cube_and_raw(data_advs, use_dask=use_dask)
 
         # append 'o' to indicate that it has been operated on
-        c1o = c1._apply_everywhere(operation, value)
+        c1o = c1._apply_everywhere(operation, value, check_units=True)
         d1o = operation(u.Quantity(d1, u.K), value)
 
         assert np.all(d1o == c1o.filled_data[:])
         # allclose fails on identical data?
         #assert_allclose(d1o, c1o.filled_data[:])
 
+
+    @pytest.mark.parametrize(('operation', 'value'), ((operator.add, 0.5*u.K),
+                                                      (operator.sub, 0.5*u.K),))
+    def test_apply_everywhere_plusminus(self, operation, value, data_advs, use_dask):
+        c1, d1 = cube_and_raw(data_advs, use_dask=use_dask)
+
+        assert c1.unit == value.unit
+
+        # append 'o' to indicate that it has been operated on
+        # value.value: the __add__ function explicitly drops the units
+        c1o = c1._apply_everywhere(operation, value.value, check_units=False)
+        d1o = operation(u.Quantity(d1, u.K), value)
+        assert c1o.unit == c1.unit
+        assert c1o.unit == value.unit
+
+        assert np.all(d1o == c1o.filled_data[:])
+
+
+    @pytest.mark.parametrize(('operation', 'value'),
+                             ((operator.div if hasattr(operator,'div') else operator.floordiv, 0.5*u.K),))
+    def test_apply_everywhere_floordivide(self, operation, value, data_advs, use_dask):
+        c1, d1 = cube_and_raw(data_advs, use_dask=use_dask)
+        try:
+            c1o = c1._apply_everywhere(operation, value)
+        except Exception as ex:
+            isinstance(ex, (NotImplementedError, TypeError, u.UnitConversionError))
+
+
     @pytest.mark.parametrize(('filename', 'trans'), translist, indirect=['filename'])
     def test_getitem(self, filename, trans, use_dask):
         c, d = cube_and_raw(filename, use_dask=use_dask)
 
         expected = np.squeeze(d.transpose(trans))
 
         assert_allclose(c[0,:,:].value, expected[0,:,:])
@@ -439,14 +463,26 @@
 
     @pytest.mark.parametrize(('value'),(1,1.0,2,2.0))
     def test_add(self,value):
         d2 = self.d1 + value
         c2 = self.c1 + value*u.K
         assert np.all(d2 == c2.filled_data[:].value)
         assert c2.unit == u.K
+
+        with pytest.raises(ValueError,
+                           match="Can only add cube objects from SpectralCubes or Quantities with a unit attribute."):
+            # c1 is something with Kelvin units, but you can't add a scalar
+            _ = self.c1 + value
+
+        with pytest.raises(u.UnitConversionError,
+                           match=re.escape("'Jy' (spectral flux density) and 'K' (temperature) are not convertible")):
+            # c1 is something with Kelvin units, but you can't add a scalar
+            _ = self.c1 + value*u.Jy
+
+        # cleanup
         self.c1 = self.d1 = None
 
     def test_add_cubes(self):
         d2 = self.d1 + self.d1
         c2 = self.c1 + self.c1
         assert np.all(d2 == c2.filled_data[:].value)
         assert c2.unit == u.K
@@ -503,14 +539,37 @@
         d2 = self.d1 / self.d1
         c2 = self.c1 / self.c1
         assert np.all((d2 == c2.filled_data[:].value) | (np.isnan(c2.filled_data[:])))
         assert np.all((c2.filled_data[:] == 1) | (np.isnan(c2.filled_data[:])))
         assert c2.unit == u.one
         self.c1 = self.d1 = None
 
+    @pytest.mark.parametrize(('value'),(1,1.0,2,2.0))
+    def test_floordiv(self, value):
+        with pytest.raises(NotImplementedError,
+                           match=re.escape("Floor-division (division with truncation) "
+                                           "is not supported.")):
+            c2 = self.c1 // value
+        self.c1 = self.d1 = None
+
+    @pytest.mark.parametrize(('value'),(1,1.0,2,2.0)*u.K)
+    def test_floordiv_fails(self, value):
+        with pytest.raises(NotImplementedError,
+                           match=re.escape("Floor-division (division with truncation) "
+                                           "is not supported.")):
+            c2 = self.c1 // value
+        self.c1 = self.d1 = None
+
+    def test_floordiv_cubes(self):
+        with pytest.raises(NotImplementedError,
+                           match=re.escape("Floor-division (division with truncation) "
+                                           "is not supported.")):
+            c2 = self.c1 // self.c1
+        self.c1 = self.d1 = None
+
     @pytest.mark.parametrize(('value'),
                              (1,1.0,2,2.0))
     def test_pow(self, value):
         d2 = self.d1 ** value
         c2 = self.c1 ** value
         assert np.all(d2 == c2.filled_data[:].value)
         assert c2.unit == u.K**value
@@ -633,22 +692,15 @@
         # this is a test for manually-applied numpy medians, which are different
         # from the cube.median method that does "the right thing"
         #
         # for regular median, we expect a failure, which is why we don't use
         # regular median.
 
         scmed = self.c.apply_numpy_function(np.median, axis=0)
-        # this checks whether numpy <=1.9.3 has a bug?
-        # as far as I can tell, np==1.9.3 no longer has this bug/feature
-        #if LooseVersion(np.__version__) <= LooseVersion('1.9.3'):
-        #    # print statements added so we get more info in the travis builds
-        #    print("Numpy version is: {0}".format(LooseVersion(np.__version__)))
-        #    assert np.count_nonzero(np.isnan(scmed)) == 5
-        #else:
-        #    print("Numpy version is: {0}".format(LooseVersion(np.__version__)))
+
         assert np.count_nonzero(np.isnan(scmed)) == 6
 
         scmed = self.c.apply_numpy_function(np.nanmedian, axis=0)
         assert np.count_nonzero(np.isnan(scmed)) == 0
 
         # use a more aggressive mask to force there to be some all-nan axes
         m2 = self.c>0.74*self.c.unit
@@ -987,23 +1039,23 @@
     assert isinstance(cube2._mask, BooleanArrayMask)
     assert cube2._mask._wcs is cube._wcs
     assert cube2._mask._mask is mask
 
 
 def test_with_mask_with_good_array_shape(use_dask):
     cube = _dummy_cube(use_dask)
-    mask = np.zeros((1, 5), dtype=np.bool)
+    mask = np.zeros((1, 5), dtype=bool)
     cube2 = cube.with_mask(mask, inherit_mask=False)
     assert isinstance(cube2._mask, BooleanArrayMask)
     np.testing.assert_equal(cube2._mask._mask, mask.reshape((1, 1, 5)))
 
 
 def test_with_mask_with_bad_array_shape(use_dask):
     cube = _dummy_cube(use_dask)
-    mask = np.zeros((5, 5), dtype=np.bool)
+    mask = np.zeros((5, 5), dtype=bool)
     with pytest.raises(ValueError) as exc:
         cube.with_mask(mask)
     assert exc.value.args[0] == ("Mask shape is not broadcastable to data shape: "
                                  "(5, 5) vs (1, 1, 5)")
 
 
 class TestMasks(BaseTest):
@@ -1265,25 +1317,25 @@
                                            ('data_advs', 'data_advs_nobeam'),
                                           ), indirect=['filename'])
 def test_twod_numpy(func, how, axis, filename, use_dask):
     # Check that a numpy function returns the correct result when applied along
     # one axis
     # This is partly a regression test for #211
 
+    if use_dask and how != 'cube':
+        pytest.skip()
+
     cube, data = cube_and_raw(filename, use_dask=use_dask)
     cube._meta['BUNIT'] = 'K'
     cube._unit = u.K
 
     if use_dask:
-        if how != 'cube':
-            pytest.skip()
-        else:
-            proj = getattr(cube,func)(axis=axis)
+        proj = getattr(cube, func)(axis=axis)
     else:
-        proj = getattr(cube,func)(axis=axis, how=how)
+        proj = getattr(cube, func)(axis=axis, how=how)
 
     # data has a redundant 1st axis
     dproj = getattr(data,func)(axis=(0,axis+1)).squeeze()
     assert isinstance(proj, Projection)
     np.testing.assert_equal(proj.value, dproj)
     assert cube.unit == proj.unit
 
@@ -1294,26 +1346,26 @@
                                            ('data_advs', 'data_advs_nobeam'),
                                           ), indirect=['filename'])
 def test_twod_numpy_twoaxes(func, how, axis, filename, use_dask):
     # Check that a numpy function returns the correct result when applied along
     # one axis
     # This is partly a regression test for #211
 
+    if use_dask and how != 'cube':
+        pytest.skip()
+
     cube, data = cube_and_raw(filename, use_dask=use_dask)
     cube._meta['BUNIT'] = 'K'
     cube._unit = u.K
 
     with warnings.catch_warnings(record=True) as wrn:
         if use_dask:
-            if how != 'cube':
-                pytest.skip()
-            else:
-                spec = getattr(cube,func)(axis=axis)
+            spec = getattr(cube, func)(axis=axis)
         else:
-             spec = getattr(cube,func)(axis=axis, how=how)
+            spec = getattr(cube, func)(axis=axis, how=how)
 
     if func == 'mean' and axis != (1,2):
         assert 'Averaging over a spatial and a spectral' in str(wrn[-1].message)
 
     # data has a redundant 1st axis
     dspec = getattr(data.squeeze(),func)(axis=axis)
 
@@ -1443,33 +1495,32 @@
 # collapsing to one dimension raywise doesn't make sense and is therefore
 # not supported.
 @pytest.mark.parametrize('how', ('auto', 'cube', 'slice'))
 def test_oned_collapse(how, data_advs, use_dask):
     # Check that an operation along the spatial dims returns an appropriate
     # spectrum
 
+    if use_dask and how != 'cube':
+        pytest.skip()
+
     cube, data = cube_and_raw(data_advs, use_dask=use_dask)
     cube._meta['BUNIT'] = 'K'
     cube._unit = u.K
 
     if use_dask:
-        if how != 'cube':
-            pytest.skip()
-        else:
-            spec = cube.mean(axis=(1,2))
+        spec = cube.mean(axis=(1,2))
     else:
         spec = cube.mean(axis=(1,2), how=how)
 
     assert isinstance(spec, OneDSpectrum)
     # data has a redundant 1st axis
     np.testing.assert_equal(spec.value, data.mean(axis=(0,2,3)))
     assert cube.unit == spec.unit
     assert spec.header['BUNIT'] == cube.header['BUNIT']
 
-
 def test_oned_collapse_beams(data_sdav_beams, use_dask):
     # Check that an operation along the spatial dims returns an appropriate
     # spectrum
 
     cube, data = cube_and_raw(data_sdav_beams, use_dask=use_dask)
     cube._meta['BUNIT'] = 'K'
     cube._unit = u.K
@@ -1700,14 +1751,37 @@
 
     mKcube = cube.to(u.mK)
 
     np.testing.assert_almost_equal(mKcube.filled_data[:].value,
                                    (cube.filled_data[:].value *
                                     1e3))
 
+def test_unit_conversion_brightness_temperature_without_beam(data_adv, use_dask):
+    cube, data = cube_and_raw(data_adv, use_dask=use_dask)
+    cube = SpectralCube(data, wcs=cube.wcs)
+    cube._unit = u.Jy / u.sr
+    cube._meta['BUNIT'] = 'sr-1 Jy'
+
+    # Make sure unit is correct and no beam is defined
+    assert cube.unit == u.Jy / u.sr
+    assert cube._beam is None
+    with pytest.raises(utils.NoBeamError):
+        cube.beam
+
+    brightness_t_cube = cube.to(u.K)
+    np.testing.assert_almost_equal(brightness_t_cube.filled_data[:].value,
+                                   (cube.filled_data[:].value *
+                                    1.60980084e-05))
+
+    # And convert back
+    cube_jy_angle = brightness_t_cube.to(u.Jy / u.arcsec**2)
+    np.testing.assert_almost_equal(cube_jy_angle.filled_data[:].value,
+                                   (cube.filled_data[:].value /
+                                    4.25451703e+10))
+
 
 bunits_list = [u.Jy / u.beam, u.K, u.Jy / u.sr, u.Jy / u.pix, u.Jy / u.arcsec**2,
                u.mJy / u.beam, u.mK]
 
 @pytest.mark.parametrize(('init_unit'), bunits_list)
 def test_unit_conversions_general(data_advs, use_dask, init_unit):
 
@@ -2405,14 +2479,50 @@
                         [0.303744 , 0.3038468],
                         [0.1431722, 0.303744 ]])
 
     np.testing.assert_almost_equal(cube_median[2].value, result2)
 
 
 @pytest.mark.parametrize('num_cores', (None, 1))
+def test_spatial_smooth_maxfilter(num_cores, data_adv, use_dask):
+
+    pytest.importorskip('scipy.ndimage')
+    from scipy import ndimage
+
+    cube, data = cube_and_raw(data_adv, use_dask=use_dask)
+
+    cube_spatial_max = cube.spatial_filter([3, 3],
+            filter=ndimage.filters.maximum_filter, num_cores=num_cores)
+
+    # Check first slice
+    result = np.array([[0.90950237, 0.90950237],
+                       [0.90950237, 0.90950237],
+                       [0.90388047, 0.90388047]])
+
+    np.testing.assert_almost_equal(cube_spatial_max[0, :, :].value, result)
+
+
+@pytest.mark.parametrize('num_cores', (None, 1))
+def test_spectral_smooth_maxfilter(num_cores, data_adv, use_dask):
+
+    pytest.importorskip('scipy.ndimage')
+    from scipy import ndimage
+
+    cube, data = cube_and_raw(data_adv, use_dask=use_dask)
+
+    cube_spectral_max = cube.spectral_filter(3,
+            filter=ndimage.filters.maximum_filter, num_cores=num_cores)
+
+    # Check first slice
+    result = np.array([0.90388047, 0.90388047, 0.96629004, 0.96629004])
+
+    np.testing.assert_almost_equal(cube_spectral_max[:,1,1].value, result)
+
+
+@pytest.mark.parametrize('num_cores', (None, 1))
 def test_spectral_smooth_median(num_cores, data_adv, use_dask):
 
     pytest.importorskip('scipy.ndimage')
 
     cube, data = cube_and_raw(data_adv, use_dask=use_dask)
 
     cube_spectral_median = cube.spectral_smooth_median(3, num_cores=num_cores)
@@ -2487,18 +2597,22 @@
     cube, data = cube_and_raw(data_adv, use_dask=False)
 
     with pytest.raises(ValueError,
                        match=("parallel execution was not requested, but "
                               "multiple cores were: these are incompatible "
                               "options.  Either specify num_cores=1 or "
                               "parallel=True")):
-        cube.spectral_smooth_median(3, num_cores=2, parallel=False,
-                                    update_function=update_function)
+        with warnings.catch_warnings():
+            # FITSFixed warnings can pop up here and break the raises check
+            warnings.simplefilter('ignore', AstropyWarning)
+            cube.spectral_smooth_median(3, num_cores=2, parallel=False,
+                                        update_function=update_function)
 
     with warnings.catch_warnings(record=True) as wrn:
+        warnings.simplefilter('ignore', AstropyWarning)
         cube.spectral_smooth_median(3, num_cores=1, parallel=True,
                                     update_function=update_function)
 
     assert ("parallel=True was specified but num_cores=1. "
             "Joblib will be used to run the task with a "
             "single thread.") in str(wrn[-1].message)
 
@@ -2693,7 +2807,20 @@
     beam = cube.beam
     cfrq = 100*u.GHz
 
     # This should not raise an exception
     mx_K = (mx*u.beam).to(u.K,
                           u.brightness_temperature(beam_area=beam,
                                                    frequency=cfrq))
+
+
+def test_unitless_comparison(data_adv, use_dask):
+    """
+    Issue 819: unitless cubes should be comparable to numbers
+    """
+    cube, data = cube_and_raw(data_adv, use_dask=use_dask)
+
+    # force unit for use below
+    cube._unit = u.dimensionless_unscaled
+
+    # do a comparison to verify that no error occurs
+    mask = cube > 1
```

### Comparing `spectral-cube-0.6.0/spectral_cube/tests/test_subcubes.py` & `spectral-cube-0.6.1/spectral_cube/tests/test_subcubes.py`

 * *Files 3% similar despite different names*

```diff
@@ -103,44 +103,53 @@
 @pytest.mark.parametrize('regfile',
                          ('255-fk5.reg', '255-pixel.reg'),
                         )
 def test_ds9region_255(regfile, data_255, use_dask):
     # specific test for correctness
     cube, data = cube_and_raw(data_255, use_dask=use_dask)
 
-    shapelist = regions.read_ds9(path(regfile))
+    shapelist = regions.Regions.read(path(regfile))
 
     subcube = cube.subcube_from_regions(shapelist)
     assert_array_equal(subcube[0, :, :].value,
                            np.array([11, 12, 16, 17]).reshape((2, 2)))
 
 
 @pytest.mark.skipif('not scipyOK', reason='Could not import scipy')
 @pytest.mark.skipif('not regionsOK', reason='Could not import regions')
 @pytest.mark.skipif('not REGIONS_GT_03', reason='regions version should be >= 0.3')
 @pytest.mark.parametrize(('regfile', 'result'),
-                             (('fk5.reg', (slice(None), 1, 1)),
-                              ('fk5_twoboxes.reg', (slice(None), 1, 1)),
+                             (('fk5.reg', (slice(None), 1, slice(None))),
+                              ('fk5_twoboxes.reg', (slice(None), 1, slice(None))),
                               ('image.reg', (slice(None), 1, slice(None))),
                               (
                               'partial_overlap_image.reg', (slice(None), 1, 1)),
                               ('no_overlap_image.reg', ValueError),
                               ('partial_overlap_fk5.reg', (slice(None), 1, 1)),
                               ('no_overlap_fk5.reg', ValueError),
                               ))
 def test_ds9region_new(regfile, result, data_adv, use_dask):
     cube, data = cube_and_raw(data_adv, use_dask=use_dask)
 
-    regionlist = regions.read_ds9(path(regfile))
+    regionlist = regions.Regions.read(path(regfile))
 
     if isinstance(result, type) and issubclass(result, Exception):
         with pytest.raises(result):
             sc = cube.subcube_from_regions(regionlist)
     else:
         sc = cube.subcube_from_regions(regionlist)
+
+        # Shapes and size should be the same.
+        # squeeze on the cube is b/c is retains dimensions of size 1
+        assert sc.size == data[result].size
+        assert sc.filled_data[:].squeeze().shape == data[result].shape
+
+        # If sizes are the same, values should then be the same.
+        assert (sc.unitless_filled_data[:].squeeze() == data[result]).all()
+
         scsum = sc.sum()
         dsum = data[result].sum()
         assert_allclose(scsum, dsum)
 
     #region = 'fk5\ncircle(29.9346557, 24.0623827, 0.11111)'
     #subcube = cube.subcube_from_ds9region(region)
     # THIS TEST FAILS!
```

### Comparing `spectral-cube-0.6.0/spectral_cube/tests/test_visualization.py` & `spectral-cube-0.6.1/spectral_cube/tests/test_visualization.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.0/spectral_cube/tests/test_wcs_utils.py` & `spectral-cube-0.6.1/spectral_cube/tests/test_wcs_utils.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.0/spectral_cube/tests/utilities.py` & `spectral-cube-0.6.1/spectral_cube/tests/utilities.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.0/spectral_cube/utils.py` & `spectral-cube-0.6.1/spectral_cube/utils.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.0/spectral_cube/visualization-tools.py` & `spectral-cube-0.6.1/spectral_cube/visualization-tools.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.0/spectral_cube/wcs_utils.py` & `spectral-cube-0.6.1/spectral_cube/wcs_utils.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.0/spectral_cube/ytcube.py` & `spectral-cube-0.6.1/spectral_cube/ytcube.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.0/spectral_cube.egg-info/PKG-INFO` & `spectral-cube-0.6.1/spectral_cube.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: spectral-cube
-Version: 0.6.0
+Version: 0.6.1
 Summary: A package for interaction with spectral cubes
 Home-page: http://spectral-cube.readthedocs.org
 Author: Adam Ginsburg, Tom Robitaille,  Chris Beaumont, Adam Leroy, Erik Rosolowsky, and Eric Koch
 Author-email: adam.g.ginsburg@gmail.com
 License: BSD
-Platform: UNKNOWN
 Provides-Extra: test
 Provides-Extra: docs
-Provides-Extra: novis
-Provides-Extra: all
+Provides-Extra: noviz
+Provides-Extra: viz
+Provides-Extra: viz_extra
+Provides-Extra: dev
 License-File: LICENSE.rst
 
 About
 =====
 
 |Join the chat at https://gitter.im/radio-astro-tools/spectral-cube|
 
@@ -29,29 +30,27 @@
    Powered by Astropy Badge
 
 Credits
 =======
 
 This package is developed by:
 
--  Chris Beaumont (`@ChrisBeaumont <http://github.com/ChrisBeaumont>`__)
+-  Eric Koch (`@e-koch <https://github.com/e-koch>`__)
 -  Adam Ginsburg (`@keflavich <http://github.com/keflavich>`__)
--  Adam Leroy (`@akleroy <http://github.com/akleroy>`__)
 -  Thomas Robitaille (`@astrofrog <http://github.com/astrofrog>`__)
 -  Erik Rosolowsky (`@low-sky <http://github.com/low-sky>`__)
--  Eric Koch (`@e-koch <https://github.com/e-koch>`__)
+
+Original development included substantial contributions from:
+-  Adam Leroy (`@akleroy <http://github.com/akleroy>`__)
+-  Chris Beaumont (`@ChrisBeaumont <http://github.com/ChrisBeaumont>`__)
 
 Build and coverage status
 =========================
 
-|Build Status| |Coverage Status| |DOI|
+|Coverage Status| |DOI|
 
 .. |Join the chat at https://gitter.im/radio-astro-tools/spectral-cube| image:: https://badges.gitter.im/Join%20Chat.svg
    :target: https://gitter.im/radio-astro-tools/spectral-cube?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
-.. |Build Status| image:: https://travis-ci.org/radio-astro-tools/spectral-cube.png?branch=master
-   :target: https://travis-ci.org/radio-astro-tools/spectral-cube
 .. |Coverage Status| image:: https://coveralls.io/repos/radio-astro-tools/spectral-cube/badge.svg?branch=master
    :target: https://coveralls.io/r/radio-astro-tools/spectral-cube?branch=master
 .. |DOI| image:: https://zenodo.org/badge/doi/10.5281/zenodo.11485.svg
    :target: http://dx.doi.org/10.5281/zenodo.11485
-
-
```

### Comparing `spectral-cube-0.6.0/spectral_cube.egg-info/SOURCES.txt` & `spectral-cube-0.6.1/spectral_cube.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -17,31 +17,36 @@
 docs/arithmetic.rst
 docs/beam_handling.rst
 docs/big_data.rst
 docs/conf.py
 docs/continuum_subtraction.rst
 docs/creating_reading.rst
 docs/dask.rst
+docs/developing_with_spectralcube.rst
 docs/errors.rst
 docs/examples.rst
 docs/index.rst
 docs/installing.rst
 docs/manipulating.rst
 docs/masking.rst
 docs/metadata.rst
 docs/moments.rst
 docs/nitpick-exceptions
 docs/quick_looks.rst
+docs/reprojection.rst
 docs/rtd-pip-requirements
 docs/smoothing.rst
 docs/spectral_extraction.rst
 docs/stokes.rst
 docs/visualization.rst
 docs/writing.rst
 docs/yt_example.rst
+docs/_static/radiosnakes_nostruts2.svg
+docs/_static/spectralcube.css
+docs/_templates/layout.html
 docs/_templates/autosummary/base.rst
 docs/_templates/autosummary/class.rst
 docs/_templates/autosummary/module.rst
 spectral_cube/__init__.py
 spectral_cube/_astropy_init.py
 spectral_cube/_moments.py
 spectral_cube/analysis_utilities.py
```

### Comparing `spectral-cube-0.6.0/tox.ini` & `spectral-cube-0.6.1/tox.ini`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,42 @@
 [tox]
 envlist =
-    py{36,37,38,39}-test{,-all,-dev,-novis,-cov}
+    py{38,39,310,311}-test{,-dev,-noviz,-viz,-viz_extra,-cov,-noopenfiles}
     build_docs
     codestyle
 requires =
     setuptools >= 30.3.0
     pip >= 19.3.1
-isolated_build = true
-indexserver =
-    NRAO = https://casa-pip.nrao.edu/repository/pypi-group/simple
+set_env =
+    casa: PIP_EXTRA_INDEX_URL = {env:PIP_EXTRA_INDEX_URL:https://casa-pip.nrao.edu/repository/pypi-group/simple}
 
 [testenv]
-passenv =
-    HOME
-    DISPLAY
-    LC_ALL
-    LC_CTYPE
-    ON_TRAVIS
-changedir =
-    .tmp/{envname}
-description =
-    run tests with pytest
+passenv = HOME,DISPLAY,LC_ALL,LC_CTYPE,ON_TRAVIS
+changedir = .tmp/{envname}
+description = run tests with pytest
 deps =
-    dev: git+https://github.com/radio-astro-tools/pvextractor#egg=pvextractor
-    dev: git+https://github.com/radio-astro-tools/radio-beam#egg=radio-beam
-    dev: git+https://github.com/astropy/astropy#egg=astropy
-    dev: git+https://github.com/astropy/reproject#egg=reproject
-    casa: :NRAO:casatools
-    casa: :NRAO:casatasks
+    casa: numpy
+    casa: scipy
+    casa: matplotlib
+    casa: casatools
+    casa: casatasks
 extras =
     test
-    all: all
+    dev: dev
+    viz: viz
+    viz_extra: viz_extra
+    noviz: noviz
+    cov: cov
+    latest: latest
 commands =
+    dev: pip install -U -i https://pypi.anaconda.org/astropy/simple astropy --pre
     pip freeze
-    !cov: pytest --open-files --pyargs spectral_cube {toxinidir}/docs {posargs}
-    cov: pytest --open-files --pyargs spectral_cube {toxinidir}/docs --cov spectral_cube --cov-config={toxinidir}/setup.cfg {posargs}
+    !cov-!noopenfiles: pytest --pyargs spectral_cube {toxinidir}/docs {posargs}
+    noopenfiles: pytest --pyargs spectral_cube {toxinidir}/docs {posargs}
+    cov: pytest --pyargs spectral_cube {toxinidir}/docs --cov spectral_cube --cov-config={toxinidir}/setup.cfg {posargs}
     cov: coverage xml -o {toxinidir}/coverage.xml
 
 [testenv:build_docs]
 changedir =
     docs
 description =
     invoke sphinx-build to build the HTML docs
```

