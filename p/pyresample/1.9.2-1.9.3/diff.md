# Comparing `tmp/pyresample-1.9.2.tar.gz` & `tmp/pyresample-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyresample-1.9.2.tar", last modified: Sun May 13 19:08:11 2018, max compression
+gzip compressed data, was "dist/pyresample-1.9.3.tar", last modified: Fri Jun  8 20:46:00 2018, max compression
```

## Comparing `pyresample-1.9.2.tar` & `pyresample-1.9.3.tar`

### file list

```diff
@@ -1,85 +1,86 @@
-drwxrwxr-x   0 a001673  (62310) smhiprimgrp  (2000)        0 2018-05-13 19:08:11.000000 pyresample-1.9.2/
-drwxrwxr-x   0 a001673  (62310) smhiprimgrp  (2000)        0 2018-05-13 19:08:11.000000 pyresample-1.9.2/docs/
-drwxrwxr-x   0 a001673  (62310) smhiprimgrp  (2000)        0 2018-05-13 19:08:11.000000 pyresample-1.9.2/docs/source/
-drwxrwxr-x   0 a001673  (62310) smhiprimgrp  (2000)        0 2018-05-13 19:08:11.000000 pyresample-1.9.2/docs/source/_static/
-drwxrwxr-x   0 a001673  (62310) smhiprimgrp  (2000)        0 2018-05-13 19:08:11.000000 pyresample-1.9.2/docs/source/_static/images/
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)  1152178 2017-02-07 08:08:35.000000 pyresample-1.9.2/docs/source/_static/images/bilinear_overview.png
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)   801023 2017-02-07 08:08:35.000000 pyresample-1.9.2/docs/source/_static/images/nearest_overview.png
--rw-r--r--   0 a001673  (62310) smhiprimgrp  (2000)   244656 2011-11-28 13:37:41.000000 pyresample-1.9.2/docs/source/_static/images/tb37_multi.png
--rw-r--r--   0 a001673  (62310) smhiprimgrp  (2000)   345622 2011-11-28 13:37:41.000000 pyresample-1.9.2/docs/source/_static/images/tb37v_bmng.png
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)    69084 2013-06-12 09:02:21.000000 pyresample-1.9.2/docs/source/_static/images/tb37v_ortho.png
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)   110843 2012-07-18 08:35:01.000000 pyresample-1.9.2/docs/source/_static/images/tb37v_pc.png
--rw-r--r--   0 a001673  (62310) smhiprimgrp  (2000)   174265 2011-11-28 13:37:41.000000 pyresample-1.9.2/docs/source/_static/images/tb37v_quick.png
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)    35330 2015-03-29 20:36:04.000000 pyresample-1.9.2/docs/source/_static/images/time_vs_nproc_1-12.png
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)   193508 2014-03-03 08:24:40.000000 pyresample-1.9.2/docs/source/_static/images/uncert_conc_nh.png
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)   217710 2014-03-03 08:24:40.000000 pyresample-1.9.2/docs/source/_static/images/uncert_count_nh.png
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)   201293 2014-03-03 08:24:40.000000 pyresample-1.9.2/docs/source/_static/images/uncert_stddev_nh.png
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)    64392 2018-04-27 12:34:10.000000 pyresample-1.9.2/docs/source/_static/images/viirs_i04_cartopy.png
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)      812 2017-02-07 08:08:35.000000 pyresample-1.9.2/docs/source/API.rst
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)     7723 2016-06-21 09:38:56.000000 pyresample-1.9.2/docs/source/conf.py
--rw-r--r--   0 a001673  (62310) smhiprimgrp  (2000)     2587 2011-11-28 13:37:41.000000 pyresample-1.9.2/docs/source/data_reduce.rst
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)    14293 2017-09-18 13:37:53.000000 pyresample-1.9.2/docs/source/geo_def.rst
--rw-r--r--   0 a001673  (62310) smhiprimgrp  (2000)     1648 2011-11-28 13:37:41.000000 pyresample-1.9.2/docs/source/geo_filter.rst
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)     7863 2013-06-12 09:02:21.000000 pyresample-1.9.2/docs/source/grid.rst
--rw-r--r--   0 a001673  (62310) smhiprimgrp  (2000)      759 2011-11-28 13:37:41.000000 pyresample-1.9.2/docs/source/index.rst
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)     2393 2014-03-03 08:24:41.000000 pyresample-1.9.2/docs/source/installation.rst
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)     1919 2015-03-29 20:36:04.000000 pyresample-1.9.2/docs/source/multi.rst
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)     6879 2018-04-27 12:34:10.000000 pyresample-1.9.2/docs/source/plot.rst
--rw-r--r--   0 a001673  (62310) smhiprimgrp  (2000)     2365 2011-11-28 13:37:41.000000 pyresample-1.9.2/docs/source/preproc.rst
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)    23448 2018-02-02 12:17:02.000000 pyresample-1.9.2/docs/source/swath.rst
--rw-r--r--   0 a001673  (62310) smhiprimgrp  (2000)     3141 2011-11-28 13:37:40.000000 pyresample-1.9.2/docs/Makefile
-drwxrwxr-x   0 a001673  (62310) smhiprimgrp  (2000)        0 2018-05-13 19:08:11.000000 pyresample-1.9.2/pyresample/
-drwxrwxr-x   0 a001673  (62310) smhiprimgrp  (2000)        0 2018-05-13 19:08:11.000000 pyresample-1.9.2/pyresample/bilinear/
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)    18895 2017-10-13 09:25:58.000000 pyresample-1.9.2/pyresample/bilinear/__init__.py
-drwxrwxr-x   0 a001673  (62310) smhiprimgrp  (2000)        0 2018-05-13 19:08:11.000000 pyresample-1.9.2/pyresample/ewa/
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)    10878 2017-05-02 08:25:13.000000 pyresample-1.9.2/pyresample/ewa/__init__.py
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)  1303908 2017-10-13 09:22:37.000000 pyresample-1.9.2/pyresample/ewa/_fornav.cpp
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)    14213 2016-07-21 20:43:46.000000 pyresample-1.9.2/pyresample/ewa/_fornav_templates.cpp
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)     2211 2016-06-17 10:33:22.000000 pyresample-1.9.2/pyresample/ewa/_fornav_templates.h
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)  1054157 2017-10-13 09:22:37.000000 pyresample-1.9.2/pyresample/ewa/_ll2cr.c
-drwxrwxr-x   0 a001673  (62310) smhiprimgrp  (2000)        0 2018-05-13 19:08:11.000000 pyresample-1.9.2/pyresample/test/
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)     1889 2018-05-13 18:54:47.000000 pyresample-1.9.2/pyresample/test/__init__.py
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)    10709 2018-02-02 12:15:27.000000 pyresample-1.9.2/pyresample/test/test_bilinear.py
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)     7576 2018-02-22 07:47:29.000000 pyresample-1.9.2/pyresample/test/test_data_reduce.py
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)     7126 2017-05-02 08:25:13.000000 pyresample-1.9.2/pyresample/test/test_ewa_fornav.py
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)     8978 2017-10-04 13:18:41.000000 pyresample-1.9.2/pyresample/test/test_ewa_ll2cr.py
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)    63933 2018-05-13 18:54:47.000000 pyresample-1.9.2/pyresample/test/test_geometry.py
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)     9792 2018-02-02 12:15:27.000000 pyresample-1.9.2/pyresample/test/test_grid.py
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)    12347 2017-10-13 09:25:58.000000 pyresample-1.9.2/pyresample/test/test_image.py
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)    40222 2018-04-27 12:34:10.000000 pyresample-1.9.2/pyresample/test/test_kd_tree.py
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)     4506 2018-04-27 12:34:10.000000 pyresample-1.9.2/pyresample/test/test_plot.py
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)     3086 2018-02-02 12:15:27.000000 pyresample-1.9.2/pyresample/test/test_rotation.py
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)    21876 2018-05-13 18:54:47.000000 pyresample-1.9.2/pyresample/test/test_spherical.py
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)    14656 2016-11-15 16:27:42.000000 pyresample-1.9.2/pyresample/test/test_spherical_geometry.py
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)     3308 2016-07-21 20:43:46.000000 pyresample-1.9.2/pyresample/test/test_swath.py
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)    10594 2018-02-02 12:17:02.000000 pyresample-1.9.2/pyresample/test/test_utils.py
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)     6458 2018-05-13 18:54:47.000000 pyresample-1.9.2/pyresample/test/utils.py
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)     1948 2018-04-27 12:34:10.000000 pyresample-1.9.2/pyresample/__init__.py
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)     3482 2018-04-27 12:34:10.000000 pyresample-1.9.2/pyresample/_cartopy.py
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)     3482 2016-04-29 13:05:57.000000 pyresample-1.9.2/pyresample/_multi_proc.py
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)    10163 2016-04-29 13:05:57.000000 pyresample-1.9.2/pyresample/_spatial_mp.py
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)     3636 2018-05-13 18:54:47.000000 pyresample-1.9.2/pyresample/boundary.py
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)    10723 2018-02-22 07:47:29.000000 pyresample-1.9.2/pyresample/data_reduce.py
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)     2751 2015-03-29 20:36:04.000000 pyresample-1.9.2/pyresample/geo_filter.py
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)    59555 2018-05-13 18:54:47.000000 pyresample-1.9.2/pyresample/geometry.py
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)     8691 2018-02-02 12:15:27.000000 pyresample-1.9.2/pyresample/grid.py
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)    15530 2018-02-02 12:15:27.000000 pyresample-1.9.2/pyresample/image.py
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)    45080 2018-05-13 18:54:47.000000 pyresample-1.9.2/pyresample/kd_tree.py
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)    11973 2018-04-27 12:34:10.000000 pyresample-1.9.2/pyresample/plot.py
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)    17545 2018-05-13 18:59:14.000000 pyresample-1.9.2/pyresample/spherical.py
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)    14389 2018-05-13 18:54:47.000000 pyresample-1.9.2/pyresample/spherical_geometry.py
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)    17496 2018-02-02 12:17:02.000000 pyresample-1.9.2/pyresample/utils.py
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)      835 2018-05-13 19:05:41.000000 pyresample-1.9.2/pyresample/version.py
-drwxrwxr-x   0 a001673  (62310) smhiprimgrp  (2000)        0 2018-05-13 19:08:11.000000 pyresample-1.9.2/pyresample.egg-info/
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)      607 2018-05-13 19:08:11.000000 pyresample-1.9.2/pyresample.egg-info/PKG-INFO
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)     2162 2018-05-13 19:08:11.000000 pyresample-1.9.2/pyresample.egg-info/SOURCES.txt
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)        1 2018-05-13 19:08:11.000000 pyresample-1.9.2/pyresample.egg-info/dependency_links.txt
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)        1 2014-12-10 21:39:06.000000 pyresample-1.9.2/pyresample.egg-info/not-zip-safe
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)      190 2018-05-13 19:08:11.000000 pyresample-1.9.2/pyresample.egg-info/requires.txt
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)       11 2018-05-13 19:08:11.000000 pyresample-1.9.2/pyresample.egg-info/top_level.txt
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)     7657 2016-04-29 13:05:57.000000 pyresample-1.9.2/LICENSE.txt
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)      147 2016-06-21 09:58:03.000000 pyresample-1.9.2/MANIFEST.in
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)     1406 2018-05-13 18:54:47.000000 pyresample-1.9.2/README
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)      173 2018-05-13 19:08:11.000000 pyresample-1.9.2/setup.cfg
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)     4925 2018-05-12 18:47:54.000000 pyresample-1.9.2/setup.py
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)      607 2018-05-13 19:08:11.000000 pyresample-1.9.2/PKG-INFO
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-06-08 20:46:00.000000 pyresample-1.9.3/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7657 2018-06-08 20:39:15.000000 pyresample-1.9.3/LICENSE.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-06-08 20:46:00.000000 pyresample-1.9.3/docs/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3141 2018-06-08 20:39:15.000000 pyresample-1.9.3/docs/Makefile
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-06-08 20:46:00.000000 pyresample-1.9.3/docs/source/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1648 2018-06-08 20:39:15.000000 pyresample-1.9.3/docs/source/geo_filter.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      759 2018-06-08 20:39:15.000000 pyresample-1.9.3/docs/source/index.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14293 2018-06-08 20:39:15.000000 pyresample-1.9.3/docs/source/geo_def.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6879 2018-06-08 20:39:15.000000 pyresample-1.9.3/docs/source/plot.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2365 2018-06-08 20:39:15.000000 pyresample-1.9.3/docs/source/preproc.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-06-08 20:46:00.000000 pyresample-1.9.3/docs/source/_static/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-06-08 20:46:00.000000 pyresample-1.9.3/docs/source/_static/images/
+-rw-rw-r--   0 travis    (2000) travis    (2000)   345622 2018-06-08 20:39:15.000000 pyresample-1.9.3/docs/source/_static/images/tb37v_bmng.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)   244656 2018-06-08 20:39:15.000000 pyresample-1.9.3/docs/source/_static/images/tb37_multi.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35330 2018-06-08 20:39:15.000000 pyresample-1.9.3/docs/source/_static/images/time_vs_nproc_1-12.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)   201293 2018-06-08 20:39:15.000000 pyresample-1.9.3/docs/source/_static/images/uncert_stddev_nh.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)    69084 2018-06-08 20:39:15.000000 pyresample-1.9.3/docs/source/_static/images/tb37v_ortho.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)    64392 2018-06-08 20:39:15.000000 pyresample-1.9.3/docs/source/_static/images/viirs_i04_cartopy.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)   193508 2018-06-08 20:39:15.000000 pyresample-1.9.3/docs/source/_static/images/uncert_conc_nh.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)   110843 2018-06-08 20:39:15.000000 pyresample-1.9.3/docs/source/_static/images/tb37v_pc.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)   217710 2018-06-08 20:39:15.000000 pyresample-1.9.3/docs/source/_static/images/uncert_count_nh.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1152178 2018-06-08 20:39:15.000000 pyresample-1.9.3/docs/source/_static/images/bilinear_overview.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)   801023 2018-06-08 20:39:15.000000 pyresample-1.9.3/docs/source/_static/images/nearest_overview.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)   174265 2018-06-08 20:39:15.000000 pyresample-1.9.3/docs/source/_static/images/tb37v_quick.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1919 2018-06-08 20:39:15.000000 pyresample-1.9.3/docs/source/multi.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2393 2018-06-08 20:39:15.000000 pyresample-1.9.3/docs/source/installation.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23444 2018-06-08 20:39:15.000000 pyresample-1.9.3/docs/source/swath.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      812 2018-06-08 20:39:15.000000 pyresample-1.9.3/docs/source/API.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7863 2018-06-08 20:39:15.000000 pyresample-1.9.3/docs/source/grid.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2587 2018-06-08 20:39:15.000000 pyresample-1.9.3/docs/source/data_reduce.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7723 2018-06-08 20:39:15.000000 pyresample-1.9.3/docs/source/conf.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-06-08 20:46:00.000000 pyresample-1.9.3/pyresample/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10163 2018-06-08 20:39:15.000000 pyresample-1.9.3/pyresample/_spatial_mp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15531 2018-06-08 20:39:15.000000 pyresample-1.9.3/pyresample/image.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14389 2018-06-08 20:39:15.000000 pyresample-1.9.3/pyresample/spherical_geometry.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2751 2018-06-08 20:39:15.000000 pyresample-1.9.3/pyresample/geo_filter.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3633 2018-06-08 20:39:15.000000 pyresample-1.9.3/pyresample/boundary.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11973 2018-06-08 20:39:15.000000 pyresample-1.9.3/pyresample/plot.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-06-08 20:46:00.000000 pyresample-1.9.3/pyresample/ewa/
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1054157 2018-06-08 20:39:15.000000 pyresample-1.9.3/pyresample/ewa/_ll2cr.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10874 2018-06-08 20:39:15.000000 pyresample-1.9.3/pyresample/ewa/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2211 2018-06-08 20:39:15.000000 pyresample-1.9.3/pyresample/ewa/_fornav_templates.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1303908 2018-06-08 20:39:15.000000 pyresample-1.9.3/pyresample/ewa/_fornav.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14213 2018-06-08 20:39:15.000000 pyresample-1.9.3/pyresample/ewa/_fornav_templates.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1949 2018-06-08 20:39:15.000000 pyresample-1.9.3/pyresample/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    45080 2018-06-08 20:39:15.000000 pyresample-1.9.3/pyresample/kd_tree.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17545 2018-06-08 20:39:15.000000 pyresample-1.9.3/pyresample/spherical.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      835 2018-06-08 20:39:15.000000 pyresample-1.9.3/pyresample/version.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-06-08 20:46:00.000000 pyresample-1.9.3/pyresample/test/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9788 2018-06-08 20:39:15.000000 pyresample-1.9.3/pyresample/test/test_grid.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11348 2018-06-08 20:39:15.000000 pyresample-1.9.3/pyresample/test/test_image.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8978 2018-06-08 20:39:15.000000 pyresample-1.9.3/pyresample/test/test_ewa_ll2cr.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7126 2018-06-08 20:39:15.000000 pyresample-1.9.3/pyresample/test/test_ewa_fornav.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3308 2018-06-08 20:39:15.000000 pyresample-1.9.3/pyresample/test/test_swath.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1889 2018-06-08 20:39:15.000000 pyresample-1.9.3/pyresample/test/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21876 2018-06-08 20:39:15.000000 pyresample-1.9.3/pyresample/test/test_spherical.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7375 2018-06-08 20:39:15.000000 pyresample-1.9.3/pyresample/test/test_data_reduce.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12581 2018-06-08 20:39:15.000000 pyresample-1.9.3/pyresample/test/test_bilinear.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34968 2018-06-08 20:39:15.000000 pyresample-1.9.3/pyresample/test/test_kd_tree.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10594 2018-06-08 20:39:15.000000 pyresample-1.9.3/pyresample/test/test_utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3086 2018-06-08 20:39:15.000000 pyresample-1.9.3/pyresample/test/test_rotation.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14656 2018-06-08 20:39:15.000000 pyresample-1.9.3/pyresample/test/test_spherical_geometry.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6458 2018-06-08 20:39:15.000000 pyresample-1.9.3/pyresample/test/utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    66945 2018-06-08 20:39:15.000000 pyresample-1.9.3/pyresample/test/test_geometry.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4504 2018-06-08 20:39:15.000000 pyresample-1.9.3/pyresample/test/test_plot.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8691 2018-06-08 20:39:15.000000 pyresample-1.9.3/pyresample/grid.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10793 2018-06-08 20:39:15.000000 pyresample-1.9.3/pyresample/data_reduce.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    60627 2018-06-08 20:39:15.000000 pyresample-1.9.3/pyresample/geometry.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17370 2018-06-08 20:39:15.000000 pyresample-1.9.3/pyresample/utils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-06-08 20:46:00.000000 pyresample-1.9.3/pyresample/bilinear/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24613 2018-06-08 20:39:15.000000 pyresample-1.9.3/pyresample/bilinear/xarr.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19058 2018-06-08 20:39:15.000000 pyresample-1.9.3/pyresample/bilinear/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3483 2018-06-08 20:39:15.000000 pyresample-1.9.3/pyresample/_cartopy.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3482 2018-06-08 20:39:15.000000 pyresample-1.9.3/pyresample/_multi_proc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4992 2018-06-08 20:39:15.000000 pyresample-1.9.3/setup.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      173 2018-06-08 20:46:00.000000 pyresample-1.9.3/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1405 2018-06-08 20:39:15.000000 pyresample-1.9.3/README
+-rw-rw-r--   0 travis    (2000) travis    (2000)      127 2018-06-08 20:39:15.000000 pyresample-1.9.3/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)      724 2018-06-08 20:46:00.000000 pyresample-1.9.3/PKG-INFO
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-06-08 20:46:00.000000 pyresample-1.9.3/pyresample.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       11 2018-06-08 20:46:00.000000 pyresample-1.9.3/pyresample.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2018-06-08 20:46:00.000000 pyresample-1.9.3/pyresample.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)      190 2018-06-08 20:46:00.000000 pyresample-1.9.3/pyresample.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      724 2018-06-08 20:46:00.000000 pyresample-1.9.3/pyresample.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2018-06-08 20:46:00.000000 pyresample-1.9.3/pyresample.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2190 2018-06-08 20:46:00.000000 pyresample-1.9.3/pyresample.egg-info/SOURCES.txt
```

### Comparing `pyresample-1.9.2/docs/source/_static/images/bilinear_overview.png` & `pyresample-1.9.3/docs/source/_static/images/bilinear_overview.png`

 * *Files identical despite different names*

### Comparing `pyresample-1.9.2/docs/source/_static/images/nearest_overview.png` & `pyresample-1.9.3/docs/source/_static/images/nearest_overview.png`

 * *Files identical despite different names*

### Comparing `pyresample-1.9.2/docs/source/_static/images/tb37_multi.png` & `pyresample-1.9.3/docs/source/_static/images/tb37_multi.png`

 * *Files identical despite different names*

### Comparing `pyresample-1.9.2/docs/source/_static/images/tb37v_bmng.png` & `pyresample-1.9.3/docs/source/_static/images/tb37v_bmng.png`

 * *Files identical despite different names*

### Comparing `pyresample-1.9.2/docs/source/_static/images/tb37v_ortho.png` & `pyresample-1.9.3/docs/source/_static/images/tb37v_ortho.png`

 * *Files identical despite different names*

### Comparing `pyresample-1.9.2/docs/source/_static/images/tb37v_pc.png` & `pyresample-1.9.3/docs/source/_static/images/tb37v_pc.png`

 * *Files identical despite different names*

### Comparing `pyresample-1.9.2/docs/source/_static/images/tb37v_quick.png` & `pyresample-1.9.3/docs/source/_static/images/tb37v_quick.png`

 * *Files identical despite different names*

### Comparing `pyresample-1.9.2/docs/source/_static/images/time_vs_nproc_1-12.png` & `pyresample-1.9.3/docs/source/_static/images/time_vs_nproc_1-12.png`

 * *Files identical despite different names*

### Comparing `pyresample-1.9.2/docs/source/_static/images/uncert_conc_nh.png` & `pyresample-1.9.3/docs/source/_static/images/uncert_conc_nh.png`

 * *Files identical despite different names*

### Comparing `pyresample-1.9.2/docs/source/_static/images/uncert_count_nh.png` & `pyresample-1.9.3/docs/source/_static/images/uncert_count_nh.png`

 * *Files identical despite different names*

### Comparing `pyresample-1.9.2/docs/source/_static/images/uncert_stddev_nh.png` & `pyresample-1.9.3/docs/source/_static/images/uncert_stddev_nh.png`

 * *Files identical despite different names*

### Comparing `pyresample-1.9.2/docs/source/_static/images/viirs_i04_cartopy.png` & `pyresample-1.9.3/docs/source/_static/images/viirs_i04_cartopy.png`

 * *Files identical despite different names*

### Comparing `pyresample-1.9.2/docs/source/API.rst` & `pyresample-1.9.3/docs/source/API.rst`

 * *Files identical despite different names*

### Comparing `pyresample-1.9.2/docs/source/conf.py` & `pyresample-1.9.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pyresample-1.9.2/docs/source/data_reduce.rst` & `pyresample-1.9.3/docs/source/data_reduce.rst`

 * *Files identical despite different names*

### Comparing `pyresample-1.9.2/docs/source/geo_def.rst` & `pyresample-1.9.3/docs/source/geo_def.rst`

 * *Files identical despite different names*

### Comparing `pyresample-1.9.2/docs/source/geo_filter.rst` & `pyresample-1.9.3/docs/source/geo_filter.rst`

 * *Files identical despite different names*

### Comparing `pyresample-1.9.2/docs/source/grid.rst` & `pyresample-1.9.3/docs/source/grid.rst`

 * *Files identical despite different names*

### Comparing `pyresample-1.9.2/docs/source/index.rst` & `pyresample-1.9.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pyresample-1.9.2/docs/source/installation.rst` & `pyresample-1.9.3/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `pyresample-1.9.2/docs/source/multi.rst` & `pyresample-1.9.3/docs/source/multi.rst`

 * *Files identical despite different names*

### Comparing `pyresample-1.9.2/docs/source/plot.rst` & `pyresample-1.9.3/docs/source/plot.rst`

 * *Files identical despite different names*

### Comparing `pyresample-1.9.2/docs/source/preproc.rst` & `pyresample-1.9.3/docs/source/preproc.rst`

 * *Files identical despite different names*

### Comparing `pyresample-1.9.2/docs/source/swath.rst` & `pyresample-1.9.3/docs/source/swath.rst`

 * *Files 1% similar despite different names*

```diff
@@ -297,15 +297,15 @@
  >>> source_def = geometry.SwathDefinition(lons=lons, lats=lats)
  >>> result = bilinear.resample_bilinear(data, source_def, target_def,
  ...                                     radius=50e3, neighbours=32,
  ...                                     nprocs=1, fill_value=0,
  ...                                     reduce_data=True, segments=None,
  ...                                     epsilon=0)
 
-The **target_area** needs to be an area definition with **proj4_string**
+The **target_area** needs to be an area definition with **proj_str**
 attribute.
 
 ..
     The **source_def** can be either an area definition as above,
     or a 2-tuple of (lons, lats).
 
 Keyword arguments which are passed to **kd_tree**:
```

### Comparing `pyresample-1.9.2/docs/Makefile` & `pyresample-1.9.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyresample-1.9.2/pyresample/bilinear/__init__.py` & `pyresample-1.9.3/pyresample/bilinear/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,16 +131,18 @@
     -------
     result : numpy array
         Source data resampled to target geometry
     """
 
     # Reduce data
     new_data = data[input_idxs]
-    data_min = np.nanmin(new_data)
-    data_max = np.nanmax(new_data)
+    # Add a small "machine epsilon" so that tiny variations are not discarded
+    epsilon = 1e-6
+    data_min = np.nanmin(new_data) - epsilon
+    data_max = np.nanmax(new_data) + epsilon
 
     new_data = new_data[idx_arr]
 
     # Get neighbour data to separate variables
     p_1 = new_data[:, 0]
     p_2 = new_data[:, 1]
     p_3 = new_data[:, 2]
@@ -229,30 +231,30 @@
 
     # Reduce index reference
     input_size = input_idxs.sum()
     index_mask = (idx_ref == input_size)
     idx_ref = np.where(index_mask, 0, idx_ref)
 
     # Get output projection as pyproj object
-    proj = Proj(target_area_def.proj4_string)
+    proj = Proj(target_area_def.proj_str)
 
     # Get output x/y coordinates
     out_x, out_y = _get_output_xy(target_area_def, proj)
 
-    # Get input x/ycoordinates
+    # Get input x/y coordinates
     in_x, in_y = _get_input_xy(source_geo_def, proj, input_idxs, idx_ref)
 
     # Get the four closest corner points around each output location
     pt_1, pt_2, pt_3, pt_4, idx_ref = \
         _get_bounding_corners(in_x, in_y, out_x, out_y, neighbours, idx_ref)
 
     # Calculate vertical and horizontal fractional distances t and s
     t__, s__ = _get_ts(pt_1, pt_2, pt_3, pt_4, out_x, out_y)
 
-    # Remove mask and put np.nan at the masked locations instead
+    # Mask NaN values
     if masked:
         mask = np.isnan(t__) | np.isnan(s__)
         t__ = np.ma.masked_where(mask, t__)
         s__ = np.ma.masked_where(mask, s__)
 
     return t__, s__, input_idxs, idx_ref
 
@@ -408,16 +410,19 @@
         lats[idxs] = np.nan
 
     return lons, lats
 
 
 def _get_corner(stride, valid, in_x, in_y, idx_ref):
     """Get closest set of coordinates from the *valid* locations"""
+    # Find the closest valid pixels, if any
     idxs = np.argmax(valid, axis=1)
+    # Check which of these were actually valid
     invalid = np.invert(np.max(valid, axis=1))
+
     # Replace invalid points with np.nan
     x__ = in_x[stride, idxs]
     x__[invalid] = np.nan
     y__ = in_y[stride, idxs]
     y__[invalid] = np.nan
     idx = idx_ref[stride, idxs]
```

### Comparing `pyresample-1.9.2/pyresample/ewa/__init__.py` & `pyresample-1.9.3/pyresample/ewa/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
         lons = lons.astype(np.float64, copy=copy)
         lats = lats.astype(np.float64, copy=copy)
     except TypeError:
         lons = lons.astype(np.float64)
         lats = lats.astype(np.float64)
 
     # Break the input area up in to the expected parameters for ll2cr
-    p = area_def.proj4_string
+    p = area_def.proj_str
     cw = area_def.pixel_size_x
     # cell height must be negative for this to work as expected
     ch = -abs(area_def.pixel_size_y)
     w = area_def.x_size
     h = area_def.y_size
     ox = area_def.area_extent[0] + cw / 2.
     oy = area_def.area_extent[3] + ch / 2.
```

### Comparing `pyresample-1.9.2/pyresample/ewa/_fornav.cpp` & `pyresample-1.9.3/pyresample/ewa/_fornav.cpp`

 * *Files identical despite different names*

### Comparing `pyresample-1.9.2/pyresample/ewa/_fornav_templates.cpp` & `pyresample-1.9.3/pyresample/ewa/_fornav_templates.cpp`

 * *Files identical despite different names*

### Comparing `pyresample-1.9.2/pyresample/ewa/_fornav_templates.h` & `pyresample-1.9.3/pyresample/ewa/_fornav_templates.h`

 * *Files identical despite different names*

### Comparing `pyresample-1.9.2/pyresample/ewa/_ll2cr.c` & `pyresample-1.9.3/pyresample/ewa/_ll2cr.c`

 * *Files identical despite different names*

### Comparing `pyresample-1.9.2/pyresample/test/__init__.py` & `pyresample-1.9.3/pyresample/test/__init__.py`

 * *Files identical despite different names*

### Comparing `pyresample-1.9.2/pyresample/test/test_bilinear.py` & `pyresample-1.9.3/pyresample/test/test_bilinear.py`

 * *Files 16% similar despite different names*

```diff
@@ -40,16 +40,17 @@
                                               1029087.28,
                                               1490031.3600000001])
 
         # Input data around the target pixel at 0.63388324, 55.08234642,
         in_shape = (100, 100)
         cls.data1 = np.ones((in_shape[0], in_shape[1]))
         cls.data2 = 2. * cls.data1
-        lons, lats = np.meshgrid(np.linspace(-5., 5., num=in_shape[0]),
-                                 np.linspace(50., 60., num=in_shape[1]))
+        cls.data3 = cls.data1 + 9.5
+        lons, lats = np.meshgrid(np.linspace(-25., 40., num=in_shape[0]),
+                                 np.linspace(45., 75., num=in_shape[1]))
         cls.swath_def = geometry.SwathDefinition(lons=lons, lats=lats)
 
         radius = 50e3
         cls.neighbours = 32
         input_idxs, output_idxs, idx_ref, dists = \
             kd_tree.get_neighbour_info(cls.swath_def, target_def,
                                        radius, neighbours=cls.neighbours,
@@ -58,15 +59,14 @@
         index_mask = (idx_ref == input_size)
         idx_ref = np.where(index_mask, 0, idx_ref)
 
         cls.input_idxs = input_idxs
         cls.target_def = target_def
         cls.idx_ref = idx_ref
 
-
     def test_calc_abc(self):
         # No np.nan inputs
         pt_1, pt_2, pt_3, pt_4 = self.pts_irregular
         res = bil._calc_abc(pt_1, pt_2, pt_3, pt_4, 0.0, 0.0)
         self.assertFalse(np.isnan(res[0]))
         self.assertFalse(np.isnan(res[1]))
         self.assertFalse(np.isnan(res[2]))
@@ -150,53 +150,75 @@
         res = bil._solve_quadratic(res[0], res[1], res[2])
         self.assertAlmostEqual(res[0], 0.5, 5)
         res = bil._calc_abc(pt_1, pt_3, pt_2, pt_4, 0.0, 0.0)
         res = bil._solve_quadratic(res[0], res[1], res[2])
         self.assertAlmostEqual(res[0], 0.5, 5)
 
     def test_get_output_xy(self):
-        proj = Proj(self.target_def.proj4_string)
+        proj = Proj(self.target_def.proj_str)
         out_x, out_y = bil._get_output_xy(self.target_def, proj)
         self.assertTrue(out_x.all())
         self.assertTrue(out_y.all())
 
     def test_get_input_xy(self):
-        proj = Proj(self.target_def.proj4_string)
+        proj = Proj(self.target_def.proj_str)
         in_x, in_y = bil._get_output_xy(self.swath_def, proj)
         self.assertTrue(in_x.all())
         self.assertTrue(in_y.all())
 
     def test_get_bounding_corners(self):
-        proj = Proj(self.target_def.proj4_string)
+        proj = Proj(self.target_def.proj_str)
         out_x, out_y = bil._get_output_xy(self.target_def, proj)
         in_x, in_y = bil._get_input_xy(self.swath_def, proj,
                                        self.input_idxs, self.idx_ref)
         res = bil._get_bounding_corners(in_x, in_y, out_x, out_y,
                                         self.neighbours, self.idx_ref)
         for i in range(len(res) - 1):
             pt_ = res[i]
             for j in range(2):
                 # Only the sixth output location has four valid corners
                 self.assertTrue(np.isfinite(pt_[5, j]))
 
     def test_get_bil_info(self):
+        def _check_ts(t__, s__):
+            for i in range(len(t__)):
+                # Just check the exact value for one pixel
+                if i == 5:
+                    self.assertAlmostEqual(t__[i], 0.730659147133, 5)
+                    self.assertAlmostEqual(s__[i], 0.310314173004, 5)
+                # These pixels are outside the area
+                elif i in [12, 13, 14, 15]:
+                    self.assertTrue(np.isnan(t__[i]))
+                    self.assertTrue(np.isnan(s__[i]))
+                # All the others should have values between 0.0 and 1.0
+                else:
+                    self.assertTrue(t__[i] >= 0.0)
+                    self.assertTrue(s__[i] >= 0.0)
+                    self.assertTrue(t__[i] <= 1.0)
+                    self.assertTrue(s__[i] <= 1.0)
+
+        t__, s__, input_idxs, idx_arr = bil.get_bil_info(self.swath_def,
+                                                         self.target_def,
+                                                         50e5, neighbours=32,
+                                                         nprocs=1,
+                                                         reduce_data=False)
+        _check_ts(t__, s__)
+
         t__, s__, input_idxs, idx_arr = bil.get_bil_info(self.swath_def,
-                                                         self.target_def)
-        # Only 6th index should have valid values
-        for i in range(len(t__)):
-            if i == 5:
-                self.assertAlmostEqual(t__[i], 0.684850870155, 5)
-                self.assertAlmostEqual(s__[i], 0.775433912393, 5)
-            else:
-                self.assertTrue(np.isnan(t__[i]))
-                self.assertTrue(np.isnan(s__[i]))
+                                                         self.target_def,
+                                                         50e5, neighbours=32,
+                                                         nprocs=1,
+                                                         reduce_data=True)
+        _check_ts(t__, s__)
 
     def test_get_sample_from_bil_info(self):
         t__, s__, input_idxs, idx_arr = bil.get_bil_info(self.swath_def,
-                                                         self.target_def)
+                                                         self.target_def,
+                                                         50e5, neighbours=32,
+                                                         nprocs=1)
         # Sample from data1
         res = bil.get_sample_from_bil_info(self.data1.ravel(), t__, s__,
                                            input_idxs, idx_arr)
         self.assertEqual(res[5], 1.)
         # Sample from data2
         res = bil.get_sample_from_bil_info(self.data2.ravel(), t__, s__,
                                            input_idxs, idx_arr)
@@ -205,30 +227,42 @@
         res = bil.get_sample_from_bil_info(self.data2.ravel(), t__, s__,
                                            input_idxs, idx_arr,
                                            output_shape=self.target_def.shape)
         res = res.shape
         self.assertEqual(res[0], self.target_def.shape[0])
         self.assertEqual(res[1], self.target_def.shape[1])
 
+        # Test rounding that is happening for certain values
+        res = bil.get_sample_from_bil_info(self.data3.ravel(), t__, s__,
+                                           input_idxs, idx_arr,
+                                           output_shape=self.target_def.shape)
+        # Four pixels are outside of the data
+        self.assertEqual(np.isnan(res).sum(), 4)
+
     def test_resample_bilinear(self):
         # Single array
         res = bil.resample_bilinear(self.data1,
                                     self.swath_def,
-                                    self.target_def)
+                                    self.target_def,
+                                    50e5, neighbours=32,
+                                    nprocs=1)
         self.assertEqual(res.shape, self.target_def.shape)
-        # There should be only one pixel with value 1, all others are 0
-        self.assertEqual(res.sum(), 1)
+        # There are 12 pixels with value 1, all others are zero
+        self.assertEqual(res.sum(), 12)
+        self.assertEqual((res == 0).sum(), 4)
 
         # Single array with masked output
         res = bil.resample_bilinear(self.data1,
                                     self.swath_def,
-                                    self.target_def, fill_value=None)
+                                    self.target_def,
+                                    50e5, neighbours=32,
+                                    nprocs=1, fill_value=None)
         self.assertTrue(hasattr(res, 'mask'))
-        # There should be only one valid pixel
-        self.assertEqual(self.target_def.size - res.mask.sum(), 1)
+        # There should be 12 valid pixels
+        self.assertEqual(self.target_def.size - res.mask.sum(), 12)
 
         # Two stacked arrays
         data = np.dstack((self.data1, self.data2))
         res = bil.resample_bilinear(data,
                                     self.swath_def,
                                     self.target_def)
         shp = res.shape
```

### Comparing `pyresample-1.9.2/pyresample/test/test_data_reduce.py` & `pyresample-1.9.3/pyresample/test/test_data_reduce.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,14 +23,15 @@
                                     swath_from_lonlat_grid,
                                     swath_from_lonlat_boundaries,
                                     swath_from_cartesian_grid,
                                     get_valid_index_from_lonlat_grid)
 
 
 class Test(unittest.TestCase):
+
     """Unit testing the data_reduce module."""
 
     @classmethod
     def setUpClass(cls):
         """Get ready for testing."""
         cls.area_def = geometry.AreaDefinition('areaD',
                                                'Europe (3km, HRV, VTC)',
@@ -55,73 +56,71 @@
         lats = np.fromfunction(
             lambda y, x: -90 + (180.0 / 1000) * y, (1000, 1000))
         grid_lons, grid_lats = self.area_def.get_lonlats()
         lons, lats, data = swath_from_lonlat_grid(grid_lons, grid_lats,
                                                   lons, lats, data,
                                                   7000)
         cross_sum = data.sum()
-        expected = 20514375.0
-        self.assertAlmostEqual(cross_sum, expected, msg='Reduce data failed')
+        expected = 20685125.0
+        self.assertAlmostEqual(cross_sum, expected)
 
     def test_reduce_boundary(self):
         data = np.fromfunction(lambda y, x: (y + x), (1000, 1000))
         lons = np.fromfunction(
             lambda y, x: -180 + (360.0 / 1000) * x, (1000, 1000))
         lats = np.fromfunction(
             lambda y, x: -90 + (180.0 / 1000) * y, (1000, 1000))
         boundary_lonlats = self.area_def.get_boundary_lonlats()
         lons, lats, data = swath_from_lonlat_boundaries(boundary_lonlats[0],
                                                         boundary_lonlats[1],
                                                         lons, lats, data, 7000)
         cross_sum = data.sum()
-        expected = 20514375.0
-        self.assertAlmostEqual(cross_sum, expected, msg='Reduce data failed')
+        expected = 20685125.0
+        self.assertAlmostEqual(cross_sum, expected)
 
     def test_cartesian_reduce(self):
         data = np.fromfunction(lambda y, x: (y + x), (1000, 1000))
         lons = np.fromfunction(
             lambda y, x: -180 + (360.0 / 1000) * x, (1000, 1000))
         lats = np.fromfunction(
             lambda y, x: -90 + (180.0 / 1000) * y, (1000, 1000))
         grid = self.area_def.get_cartesian_coords()
         lons, lats, data = swath_from_cartesian_grid(grid, lons, lats, data,
                                                      7000)
         cross_sum = data.sum()
-        expected = 20514375.0
-        self.assertAlmostEqual(
-            cross_sum, expected, msg='Cartesian reduce data failed')
+        expected = 20685125.0
+        self.assertAlmostEqual(cross_sum, expected)
 
     def test_area_con_reduce(self):
         data = np.fromfunction(lambda y, x: (y + x), (1000, 1000))
         lons = np.fromfunction(
             lambda y, x: -180 + (360.0 / 1000) * x, (1000, 1000))
         lats = np.fromfunction(
             lambda y, x: -90 + (180.0 / 1000) * y, (1000, 1000))
         grid_lons, grid_lats = self.area_def.get_lonlats()
         valid_index = get_valid_index_from_lonlat_grid(grid_lons, grid_lats,
                                                        lons, lats, 7000)
         data = data[valid_index]
         cross_sum = data.sum()
-        expected = 20514375.0
-        self.assertAlmostEqual(cross_sum, expected, msg='Reduce data failed')
+        expected = 20685125.0
+        self.assertAlmostEqual(cross_sum, expected)
 
     def test_area_con_cartesian_reduce(self):
         data = np.fromfunction(lambda y, x: (y + x), (1000, 1000))
         lons = np.fromfunction(
             lambda y, x: -180 + (360.0 / 1000) * x, (1000, 1000))
         lats = np.fromfunction(
             lambda y, x: -90 + (180.0 / 1000) * y, (1000, 1000))
         cart_grid = self.area_def.get_cartesian_coords()
         valid_index = get_valid_index_from_cartesian_grid(cart_grid,
                                                           lons, lats, 7000)
         data = data[valid_index]
         cross_sum = data.sum()
-        expected = 20514375.0
-        self.assertAlmostEqual(
-            cross_sum, expected, msg='Cartesian reduce data failed')
+        expected = 20685125.0
+        self.assertAlmostEqual(cross_sum, expected)
 
     def test_reduce_north_pole(self):
         """Test reducing around the poles."""
 
         from pyresample import utils
         area_id = 'ease_sh'
         description = 'Antarctic EASE grid'
@@ -151,15 +150,15 @@
         lons, lats = smaller_area_def.get_lonlats()
 
         lons, lats, data = swath_from_lonlat_grid(grid_lons, grid_lats,
                                                   lons, lats, data, 7000)
 
         cross_sum = data.sum()
         expected = 999000000.0
-        self.assertAlmostEqual(cross_sum, expected, msg='Reduce data failed')
+        self.assertAlmostEqual(cross_sum, expected)
 
 
 def suite():
     """The test suite.
     """
     loader = unittest.TestLoader()
     mysuite = unittest.TestSuite()
```

### Comparing `pyresample-1.9.2/pyresample/test/test_ewa_fornav.py` & `pyresample-1.9.3/pyresample/test/test_ewa_fornav.py`

 * *Files identical despite different names*

### Comparing `pyresample-1.9.2/pyresample/test/test_ewa_ll2cr.py` & `pyresample-1.9.3/pyresample/test/test_ewa_ll2cr.py`

 * *Files identical despite different names*

### Comparing `pyresample-1.9.2/pyresample/test/test_geometry.py` & `pyresample-1.9.3/pyresample/test/test_geometry.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,24 +23,14 @@
     import unittest
 
 
 class Test(unittest.TestCase):
 
     """Unit testing the geometry and geo_filter modules"""
 
-    def assert_raises(self, exception, call_able, *args):
-        """assertRaises() has changed from py2.6 to 2.7! Here is an attempt to
-        cover both"""
-        import sys
-        if sys.version_info < (2, 7):
-            self.assertRaises(exception, call_able, *args)
-        else:
-            with self.assertRaises(exception):
-                call_able(*args)
-
     def test_lonlat_precomp(self):
         area_def = geometry.AreaDefinition('areaD', 'Europe (3km, HRV, VTC)', 'areaD',
                                            {'a': '6378144.0',
                                             'b': '6356759.0',
                                             'lat_0': '50.00',
                                             'lat_ts': '50.00',
                                             'lon_0': '8.00',
@@ -726,46 +716,32 @@
 
         lon, lat = p__(1025000 + eps_meters, 25000 + eps_meters, inverse=True)
         x__, y__ = area_def.get_xy_from_lonlat(lon, lat)
         self.assertEqual(x__, 1)
         self.assertEqual(y__, 0)
 
         lon, lat = p__(999000, -10, inverse=True)
-        self.assert_raises(ValueError, area_def.get_xy_from_lonlat, lon, lat)
-        self.assert_raises(ValueError, area_def.get_xy_from_lonlat, 0., 0.)
+        self.assertRaises(ValueError, area_def.get_xy_from_lonlat, lon, lat)
+        self.assertRaises(ValueError, area_def.get_xy_from_lonlat, 0., 0.)
 
         # Test getting arrays back:
         lons = [lon_ll + eps_lonlat, lon_ur - eps_lonlat]
         lats = [lat_ll + eps_lonlat, lat_ur - eps_lonlat]
         x__, y__ = area_def.get_xy_from_lonlat(lons, lats)
 
         x_expects = np.array([0, 1])
         y_expects = np.array([1, 0])
         self.assertTrue((x__.data == x_expects).all())
         self.assertTrue((y__.data == y_expects).all())
 
     def test_get_area_slices(self):
         """Check area slicing."""
         from pyresample import utils
-        area_id = 'cover'
-        area_name = 'Area to cover'
-        proj_id = 'test'
-        x_size = 3712
-        y_size = 3712
-        area_extent = (-5570248.477339261, -5567248.074173444, 5567248.074173444, 5570248.477339261)
-        proj_dict = {'a': 6378169.5, 'b': 6356583.8, 'h': 35785831.0,
-                     'lon_0': 0.0, 'proj': 'geos', 'units': 'm'}
-
-        area_to_cover = utils.get_area_def(area_id,
-                                           area_name,
-                                           proj_id,
-                                           proj_dict,
-                                           x_size, y_size,
-                                           area_extent)
 
+        # The area of our source data
         area_id = 'orig'
         area_name = 'Test area'
         proj_id = 'test'
         x_size = 3712
         y_size = 3712
         area_extent = (-5570248.477339745, -5561247.267842293, 5567248.074173927, 5570248.477339745)
         proj_dict = {'a': 6378169.0, 'b': 6356583.8, 'h': 35785831.0,
@@ -773,17 +749,49 @@
         area_def = utils.get_area_def(area_id,
                                       area_name,
                                       proj_id,
                                       proj_dict,
                                       x_size, y_size,
                                       area_extent)
 
+        # An area that is a subset of the original one
+        area_to_cover = utils.get_area_def(
+            'cover_subset',
+            'Area to cover',
+            'test',
+            proj_dict,
+            1000, 1000,
+            area_extent=(area_extent[0] + 10000,
+                         area_extent[1] + 10000,
+                         area_extent[2] - 10000,
+                         area_extent[3] - 10000))
         slice_x, slice_y = area_def.get_area_slices(area_to_cover)
-        self.assertEqual(slice_x, slice(0, 3712))
-        self.assertEqual(slice_y, slice(0, 3712))
+        self.assertEqual(slice(3, 3709, None), slice_x)
+        self.assertEqual(slice(3, 3709, None), slice_y)
+
+        # An area similar to the source data but not the same
+        area_id = 'cover'
+        area_name = 'Area to cover'
+        proj_id = 'test'
+        x_size = 3712
+        y_size = 3712
+        area_extent = (-5570248.477339261, -5567248.074173444, 5567248.074173444, 5570248.477339261)
+        proj_dict = {'a': 6378169.5, 'b': 6356583.8, 'h': 35785831.0,
+                     'lon_0': 0.0, 'proj': 'geos', 'units': 'm'}
+
+        area_to_cover = utils.get_area_def(area_id,
+                                           area_name,
+                                           proj_id,
+                                           proj_dict,
+                                           x_size, y_size,
+                                           area_extent)
+        slice_x, slice_y = area_def.get_area_slices(area_to_cover)
+        self.assertEqual(slice(46, 3667, None), slice_x)
+        self.assertEqual(slice(52, 3663, None), slice_y)
+
 
         area_to_cover = geometry.AreaDefinition('areaD', 'Europe (3km, HRV, VTC)', 'areaD',
                                                 {'a': 6378144.0,
                                                  'b': 6356759.0,
                                                  'lat_0': 50.00,
                                                  'lat_ts': 50.00,
                                                  'lon_0': 8.00,
@@ -794,40 +802,106 @@
                                                  -909968.64,
                                                  1029087.28,
                                                  1490031.36])
         slice_x, slice_y = area_def.get_area_slices(area_to_cover)
         self.assertEqual(slice_x, slice(1610, 2343))
         self.assertEqual(slice_y, slice(158, 515, None))
 
+    def test_get_area_slices_nongeos(self):
+        """Check area slicing for non-geos projections."""
+        from pyresample import utils
+
+        # The area of our source data
+        area_id = 'orig'
+        area_name = 'Test area'
+        proj_id = 'test'
+        x_size = 3712
+        y_size = 3712
+        area_extent = (-5570248.477339745, -5561247.267842293, 5567248.074173927, 5570248.477339745)
+        proj_dict = {'a': 6378169.0, 'b': 6356583.8, 'lat_1': 25.,
+                     'lat_2': 25., 'lon_0': 0.0, 'proj': 'lcc', 'units': 'm'}
+        area_def = utils.get_area_def(area_id,
+                                      area_name,
+                                      proj_id,
+                                      proj_dict,
+                                      x_size, y_size,
+                                      area_extent)
+
+        # An area that is a subset of the original one
+        area_to_cover = utils.get_area_def(
+            'cover_subset',
+            'Area to cover',
+            'test',
+            proj_dict,
+            1000, 1000,
+            area_extent=(area_extent[0] + 10000,
+                         area_extent[1] + 10000,
+                         area_extent[2] - 10000,
+                         area_extent[3] - 10000))
+        slice_x, slice_y = area_def.get_area_slices(area_to_cover)
+        self.assertEqual(slice(3, 3709, None), slice_x)
+        self.assertEqual(slice(3, 3709, None), slice_y)
+
+    def test_proj_str(self):
+        from collections import OrderedDict
+        proj_dict = OrderedDict()
+        proj_dict['proj'] = 'stere'
+        proj_dict['a'] = 6378144.0
+        proj_dict['b'] = 6356759.0
+        proj_dict['lat_0'] = 50.00
+        proj_dict['lat_ts'] = 50.00
+        proj_dict['lon_0'] = 8.00
+        area = geometry.AreaDefinition('areaD', 'Europe (3km, HRV, VTC)', 'areaD',
+                                       proj_dict, 10, 10,
+                                       [-1370912.72, -909968.64, 1029087.28,
+                                        1490031.36])
+        self.assertEquals(area.proj_str,
+                          '+a=6378144.0 +b=6356759.0 +lat_0=50.0 +lat_ts=50.0 +lon_0=8.0 +proj=stere')
+        proj_dict['no_rot'] = ''
+        self.assertEquals(area.proj_str,
+                          '+a=6378144.0 +b=6356759.0 +lat_0=50.0 +lat_ts=50.0 +lon_0=8.0 +no_rot +proj=stere')
+
 
 def assert_np_dict_allclose(dict1, dict2):
 
     assert set(dict1.keys()) == set(dict2.keys())
     for key, val in dict1.items():
         try:
             np.testing.assert_allclose(val, dict2[key])
         except TypeError:
             assert(val == dict2[key])
 
 
 class TestSwathDefinition(unittest.TestCase):
+
     """Test the SwathDefinition."""
 
     def test_swath(self):
         lons1 = np.fromfunction(lambda y, x: 3 + (10.0 / 100) * x, (5000, 100))
         lats1 = np.fromfunction(
             lambda y, x: 75 - (50.0 / 5000) * y, (5000, 100))
 
         swath_def = geometry.SwathDefinition(lons1, lats1)
 
         lons2, lats2 = swath_def.get_lonlats()
 
         self.assertFalse(id(lons1) != id(lons2) or id(lats1) != id(lats2),
                          msg='Caching of swath coordinates failed')
 
+    def test_slice(self):
+        """Test that SwathDefinitions can be sliced."""
+        lons1 = np.fromfunction(lambda y, x: 3 + (10.0 / 100) * x, (5000, 100))
+        lats1 = np.fromfunction(
+            lambda y, x: 75 - (50.0 / 5000) * y, (5000, 100))
+
+        swath_def = geometry.SwathDefinition(lons1, lats1)
+        new_swath_def = swath_def[1000:4000, 20:40]
+        self.assertTupleEqual(new_swath_def.lons.shape, (3000, 20))
+        self.assertTupleEqual(new_swath_def.lats.shape, (3000, 20))
+
     def test_concat_1d(self):
         lons1 = np.array([1, 2, 3])
         lats1 = np.array([1, 2, 3])
         lons2 = np.array([4, 5, 6])
         lats2 = np.array([4, 5, 6])
         swath_def1 = geometry.SwathDefinition(lons1, lats1)
         swath_def2 = geometry.SwathDefinition(lons2, lats2)
@@ -957,17 +1031,17 @@
                          [67.07600402832031, 54.147003173828125, 30.547000885009766]]).T
 
         lons = np.array([[-90.67900085449219, -21.565000534057617, -21.525001525878906],
                          [79.11000061035156, 7.284000396728516, -5.107000350952148],
                          [81.26400756835938, 29.672000885009766, 10.260000228881836]]).T
 
         area = geometry.SwathDefinition(lons, lats)
-        proj_dict = {'no_rot': True, 'lonc': -11.391744043133668,
-                     'ellps': 'WGS84', 'proj': 'omerc',
-                     'alpha': 9.185764390923012, 'lat_0': -0.2821013754097188}
+        proj_dict = {'lonc': -11.391744043133668, 'ellps': 'WGS84',
+                     'proj': 'omerc', 'alpha': 9.185764390923012,
+                     'gamma': 0, 'lat_0': -0.2821013754097188}
         assert_np_dict_allclose(area._compute_omerc_parameters('WGS84'),
                                 proj_dict)
 
     def test_get_edge_lonlats(self):
         """Test the `get_edge_lonlats` functionality."""
         lats = np.array([[85.23900604248047, 62.256004333496094, 35.58000183105469],
                          [80.84000396728516, 60.74200439453125, 34.08500289916992],
@@ -1015,26 +1089,25 @@
                          [79.11000061035156, 7.284000396728516, -5.107000350952148],
                          [81.26400756835938, 29.672000885009766, 10.260000228881836]]).T
 
         area = geometry.SwathDefinition(lons, lats)
 
         res = area.compute_optimal_bb_area({'proj': 'omerc', 'ellps': 'WGS84'})
 
-        np.testing.assert_allclose(res.area_extent, [2253027.149539,
-                                                     -2348379.728104,
-                                                     11687636.846985,
-                                                     2432121.058435])
-        proj_dict = {'no_rot': True, 'lonc': -11.391744043133668,
+        np.testing.assert_allclose(res.area_extent, [-2348379.728104, 2284625.526467,
+                                                     2432121.058435, 11719235.223912])
+        proj_dict = {'gamma': 0.0, 'lonc': -11.391744043133668,
                      'ellps': 'WGS84', 'proj': 'omerc',
                      'alpha': 9.185764390923012, 'lat_0': -0.2821013754097188}
         assert_np_dict_allclose(res.proj_dict, proj_dict)
         self.assertEqual(res.shape, (3, 3))
 
 
 class TestStackedAreaDefinition(unittest.TestCase):
+
     """Test the StackedAreaDefition."""
 
     def test_append(self):
         """Appending new definitions."""
         area1 = geometry.AreaDefinition("area1", 'area1', "geosmsg",
                                         {'a': '6378169.0', 'b': '6356583.8',
                                          'h': '35785831.0', 'lon_0': '0.0',
@@ -1185,14 +1258,15 @@
         y_size = area1.y_size + area2.y_size
         adef.assert_called_once_with(area1.area_id, area1.name, area1.proj_id,
                                      area1.proj_dict, area1.x_size, y_size,
                                      area_extent)
 
 
 class TestDynamicAreaDefinition(unittest.TestCase):
+
     """Test the DynamicAreaDefinition class."""
 
     def test_freeze(self):
         """Test freezing the area."""
         area = geometry.DynamicAreaDefinition('test_area', 'A test area',
                                               {'proj': 'laea'})
         lons = [10, 10, 22, 22]
@@ -1220,20 +1294,19 @@
                 [10, 11.9, 13.8, 15.7]]
         lats = [[66, 67, 68, 69.],
                 [58, 59, 60, 61],
                 [50, 51, 52, 53]]
         sdef = geometry.SwathDefinition(lons, lats)
         result = area.freeze(sdef,
                              resolution=1000)
-        np.testing.assert_allclose(result.area_extent, [5016583.682258,
-                                                        -336277.698941,
-                                                        8184964.697984,
-                                                        192456.651909])
-        self.assertEqual(result.x_size, 3)
-        self.assertEqual(result.y_size, 4)
+        np.testing.assert_allclose(result.area_extent,
+                                   [-336277.698941, 5047207.008079,
+                                    192456.651909, 8215588.023806])
+        self.assertEqual(result.x_size, 4)
+        self.assertEqual(result.y_size, 3)
 
     def test_compute_domain(self):
         """Test computing size and area extent."""
         area = geometry.DynamicAreaDefinition('test_area', 'A test area',
                                               {'proj': 'laea'})
         corners = [1, 1, 9, 9]
         self.assertRaises(ValueError, area.compute_domain, corners, 1, 1)
@@ -1246,14 +1319,15 @@
         area_extent, x_size, y_size = area.compute_domain(corners, resolution=2)
         self.assertTupleEqual(area_extent, (0, 0, 10, 10))
         self.assertEqual(x_size, 5)
         self.assertEqual(y_size, 5)
 
 
 class TestCrop(unittest.TestCase):
+
     """Test the area helpers."""
 
     def test_get_geostationary_bbox(self):
         """Get the geostationary bbox."""
 
         geos_area = MagicMock()
         lon_0 = 0
```

### Comparing `pyresample-1.9.2/pyresample/test/test_grid.py` & `pyresample-1.9.3/pyresample/test/test_grid.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,15 +197,15 @@
         lon, lat = self.area_def.get_lonlat(400, 400)
         self.assertAlmostEqual(
             lon, 5.5028467120975835, msg='Resampling of single lon failed')
         self.assertAlmostEqual(
             lat, 52.566998432390619, msg='Resampling of single lat failed')
 
     def test_proj4_string(self):
-        proj4_string = self.area_def.proj4_string
+        proj4_string = self.area_def.proj_str
         expected_string = '+a=6378144.0 +b=6356759.0 +lat_ts=50.00 +lon_0=8.00 +proj=stere +lat_0=50.00'
         self.assertEqual(
             frozenset(proj4_string.split()), frozenset(expected_string.split()))
 
 
 def suite():
     """The test suite.
```

### Comparing `pyresample-1.9.2/pyresample/test/test_image.py` & `pyresample-1.9.3/pyresample/test/test_image.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,35 +67,32 @@
     def test_image(self):
         data = numpy.fromfunction(lambda y, x: y * x * 10 ** -6, (3712, 3712))
         msg_con = image.ImageContainerQuick(data, self.msg_area, segments=1)
         area_con = msg_con.resample(self.area_def)
         res = area_con.image_data
         cross_sum = res.sum()
         expected = 399936.39392500359
-        self.assertAlmostEqual(
-            cross_sum, expected, msg='ImageContainer resampling quick failed')
+        self.assertAlmostEqual(cross_sum, expected)
 
     @tmp
     def test_image_segments(self):
         data = numpy.fromfunction(lambda y, x: y * x * 10 ** -6, (3712, 3712))
         msg_con = image.ImageContainerQuick(data, self.msg_area, segments=8)
         area_con = msg_con.resample(self.area_def)
         res = area_con.image_data
         cross_sum = res.sum()
         expected = 399936.39392500359
-        self.assertAlmostEqual(
-            cross_sum, expected, msg='ImageContainer resampling quick segments failed')
+        self.assertAlmostEqual(cross_sum, expected)
 
     def test_return_type(self):
         data = numpy.ones((3712, 3712)).astype('int')
         msg_con = image.ImageContainerQuick(data, self.msg_area, segments=1)
         area_con = msg_con.resample(self.area_def)
         res = area_con.image_data
-        self.assertTrue(
-            data.dtype is res.dtype, msg='Failed to maintain input data type')
+        self.assertTrue(data.dtype is res.dtype)
 
     @mask
     def test_masked_image(self):
         data = numpy.zeros((3712, 3712))
         mask = numpy.zeros((3712, 3712))
         mask[:, 1865:] = 1
         data_masked = numpy.ma.array(data, mask=mask)
@@ -103,16 +100,15 @@
             data_masked, self.msg_area, segments=1)
         area_con = msg_con.resample(self.area_def)
         res = area_con.image_data
         resampled_mask = res.mask.astype('int')
         expected = numpy.fromfile(os.path.join(os.path.dirname(__file__),
                                                'test_files', 'mask_grid.dat'),
                                   sep=' ').reshape((800, 800))
-        self.assertTrue(numpy.array_equal(
-            resampled_mask, expected), msg='Failed to resample masked array')
+        self.assertTrue(numpy.array_equal(resampled_mask, expected))
 
     @mask
     def test_masked_image_fill(self):
         data = numpy.zeros((3712, 3712))
         mask = numpy.zeros((3712, 3712))
         mask[:, 1865:] = 1
         data_masked = numpy.ma.array(data, mask=mask)
@@ -121,56 +117,52 @@
         area_con = msg_con.resample(self.area_def)
         res = area_con.image_data
         resampled_mask = res.mask.astype('int')
         expected = numpy.fromfile(os.path.join(os.path.dirname(__file__),
                                                'test_files',
                                                'mask_grid.dat'),
                                   sep=' ').reshape((800, 800))
-        self.assertTrue(numpy.array_equal(
-            resampled_mask, expected), msg='Failed to resample masked array')
+        self.assertTrue(numpy.array_equal(resampled_mask, expected))
 
     def test_nearest_neighbour(self):
         data = numpy.fromfunction(lambda y, x: y * x * 10 ** -6, (3712, 3712))
         msg_con = image.ImageContainerNearest(
             data, self.msg_area, 50000, segments=1)
         area_con = msg_con.resample(self.area_def)
         res = area_con.image_data
         cross_sum = res.sum()
-        expected = 399936.783062
-        self.assertAlmostEqual(cross_sum, expected,
-                               msg='ImageContainer resampling nearest neighbour failed')
+        expected = 399936.70287099993
+        self.assertAlmostEqual(cross_sum, expected)
 
     def test_nearest_resize(self):
         data = numpy.fromfunction(lambda y, x: y * x * 10 ** -6, (3712, 3712))
         msg_con = image.ImageContainerNearest(
             data, self.msg_area, 50000, segments=1)
         area_con = msg_con.resample(self.msg_area_resize)
         res = area_con.image_data
         cross_sum = res.sum()
         expected = 2212023.0175830
-        self.assertAlmostEqual(cross_sum, expected,
-                               msg='ImageContainer resampling nearest neighbour failed')
+        self.assertAlmostEqual(cross_sum, expected)
 
     def test_nearest_neighbour_multi(self):
         data1 = numpy.fromfunction(lambda y, x: y * x * 10 ** -6, (3712, 3712))
         data2 = numpy.fromfunction(
             lambda y, x: y * x * 10 ** -6, (3712, 3712)) * 2
         data = numpy.dstack((data1, data2))
         msg_con = image.ImageContainerNearest(
             data, self.msg_area, 50000, segments=1)
         area_con = msg_con.resample(self.area_def)
         res = area_con.image_data
         cross_sum1 = res[:, :, 0].sum()
-        expected1 = 399936.783062
-        self.assertAlmostEqual(cross_sum1, expected1,
-                               msg='ImageContainer resampling nearest neighbour multi failed')
+        expected1 = 399936.70287099993
+        self.assertAlmostEqual(cross_sum1, expected1)
+
         cross_sum2 = res[:, :, 1].sum()
-        expected2 = 399936.783062 * 2
-        self.assertAlmostEqual(cross_sum2, expected2,
-                               msg='ImageContainer resampling nearest neighbour multi failed')
+        expected2 = 399936.70287099993 * 2
+        self.assertAlmostEqual(cross_sum2, expected2)
 
     def test_nearest_neighbour_multi_preproc(self):
         data1 = numpy.fromfunction(lambda y, x: y * x * 10 ** -6, (3712, 3712))
         data2 = numpy.fromfunction(
             lambda y, x: y * x * 10 ** -6, (3712, 3712)) * 2
         data = numpy.dstack((data1, data2))
         msg_con = image.ImageContainer(data, self.msg_area)
@@ -178,90 +170,87 @@
         # 50000)
         row_indices, col_indices = \
             utils.generate_nearest_neighbour_linesample_arrays(self.msg_area,
                                                                self.area_def,
                                                                50000)
         res = msg_con.get_array_from_linesample(row_indices, col_indices)
         cross_sum1 = res[:, :, 0].sum()
-        expected1 = 399936.783062
-        self.assertAlmostEqual(cross_sum1, expected1,
-                               msg='ImageContainer resampling nearest neighbour multi preproc failed')
+        expected1 = 399936.70287099993
+        self.assertAlmostEqual(cross_sum1, expected1)
+
         cross_sum2 = res[:, :, 1].sum()
-        expected2 = 399936.783062 * 2
-        self.assertAlmostEqual(cross_sum2, expected2,
-                               msg='ImageContainer resampling nearest neighbour multi preproc failed')
+        expected2 = 399936.70287099993 * 2
+        self.assertAlmostEqual(cross_sum2, expected2)
 
     def test_nearest_swath(self):
         data = numpy.fromfunction(lambda y, x: y * x, (50, 10))
         lons = numpy.fromfunction(lambda y, x: 3 + x, (50, 10))
         lats = numpy.fromfunction(lambda y, x: 75 - y, (50, 10))
         swath_def = geometry.SwathDefinition(lons=lons, lats=lats)
         swath_con = image.ImageContainerNearest(
             data, swath_def, 50000, segments=1)
         area_con = swath_con.resample(self.area_def)
         res = area_con.image_data
         cross_sum = res.sum()
         expected = 15874591.0
-        self.assertEqual(cross_sum, expected,
-                         msg='ImageContainer swath resampling nearest failed')
+        self.assertEqual(cross_sum, expected)
 
     def test_nearest_swath_segments(self):
         data = numpy.fromfunction(lambda y, x: y * x, (50, 10))
         data = numpy.dstack(3 * (data,))
         lons = numpy.fromfunction(lambda y, x: 3 + x, (50, 10))
         lats = numpy.fromfunction(lambda y, x: 75 - y, (50, 10))
         swath_def = geometry.SwathDefinition(lons=lons, lats=lats)
         swath_con = image.ImageContainerNearest(
             data, swath_def, 50000, segments=2)
         area_con = swath_con.resample(self.area_def)
         res = area_con.image_data
         cross_sum = res.sum()
         expected = 3 * 15874591.0
-        self.assertEqual(cross_sum, expected,
-                         msg='ImageContainer swath segments resampling nearest failed')
+        self.assertEqual(cross_sum, expected)
 
     def test_bilinear(self):
         data = numpy.fromfunction(lambda y, x: y * x * 10 ** -6, (928, 928))
         msg_con = image.ImageContainerBilinear(data, self.msg_area_resize,
                                                50000, segments=1,
                                                neighbours=8)
         area_con = msg_con.resample(self.area_def)
         res = area_con.image_data
         cross_sum = res.sum()
-        expected = 24690.127073654239
+        expected = 24712.589910252744
         self.assertAlmostEqual(cross_sum, expected)
 
     def test_bilinear_multi(self):
         data1 = numpy.fromfunction(lambda y, x: y * x * 10 ** -6, (928, 928))
         data2 = numpy.fromfunction(lambda y, x: y * x * 10 ** -6,
                                    (928, 928)) * 2
         data = numpy.dstack((data1, data2))
         msg_con = image.ImageContainerBilinear(data, self.msg_area_resize,
                                                50000, segments=1,
                                                neighbours=8)
         area_con = msg_con.resample(self.area_def)
         res = area_con.image_data
         cross_sum1 = res[:, :, 0].sum()
-        expected1 = 24690.127073654239
+        expected1 = 24712.589910252744
         self.assertAlmostEqual(cross_sum1, expected1)
         cross_sum2 = res[:, :, 1].sum()
-        expected2 = 24690.127073654239 * 2
+        expected2 = 24712.589910252744 * 2
         self.assertAlmostEqual(cross_sum2, expected2)
 
     def test_bilinear_swath(self):
         data = numpy.fromfunction(lambda y, x: y * x, (50, 10))
         lons = numpy.fromfunction(lambda y, x: 3 + x, (50, 10))
         lats = numpy.fromfunction(lambda y, x: 75 - y, (50, 10))
         swath_def = geometry.SwathDefinition(lons=lons, lats=lats)
         swath_con = image.ImageContainerBilinear(data, swath_def, 500000,
                                                  segments=1, neighbours=8)
         area_con = swath_con.resample(self.area_def)
         res = area_con.image_data
         cross_sum = res.sum()
-        expected = 16762584.12441789
+        expected = 16852120.789503865
         self.assertAlmostEqual(cross_sum, expected)
 
 
 def suite():
     """The test suite.
     """
     loader = unittest.TestLoader()
```

### Comparing `pyresample-1.9.2/pyresample/test/test_kd_tree.py` & `pyresample-1.9.3/pyresample/test/test_kd_tree.py`

 * *Files 17% similar despite different names*

```diff
@@ -41,95 +41,78 @@
         cls.tgrid = geometry.CoordinateDefinition(
             lons=numpy.array([12.562036]), lats=numpy.array([55.715613]))
 
     def test_nearest_base(self):
         res = kd_tree.resample_nearest(self.tswath,
                                        self.tdata.ravel(), self.tgrid,
                                        100000, reduce_data=False, segments=1)
-        self.assertTrue(res[0] == 2, 'Failed to calculate nearest neighbour')
+        self.assertTrue(res[0] == 2)
 
     def test_gauss_base(self):
         with catch_warnings() as w:
             res = kd_tree.resample_gauss(self.tswath,
                                          self.tdata.ravel(), self.tgrid,
                                          50000, 25000, reduce_data=False, segments=1)
-            self.assertFalse(
-                len(w) != 1, 'Failed to create neighbour warning')
-            self.assertFalse(('Searching' not in str(
-                w[0].message)), 'Failed to create correct neighbour warning')
-        self.assertAlmostEqual(res[0], 2.2020729, 5,
-                               'Failed to calculate gaussian weighting')
+            self.assertFalse(len(w) != 1)
+            self.assertFalse(('Searching' not in str(w[0].message)))
+        self.assertAlmostEqual(res[0], 2.2020729, 5)
 
     def test_custom_base(self):
         def wf(dist):
             return 1 - dist / 100000.0
 
         with catch_warnings() as w:
             res = kd_tree.resample_custom(self.tswath,
                                           self.tdata.ravel(), self.tgrid,
                                           50000, wf, reduce_data=False, segments=1)
-            self.assertFalse(
-                len(w) != 1, 'Failed to create neighbour warning')
-            self.assertFalse(('Searching' not in str(
-                w[0].message)), 'Failed to create correct neighbour warning')
-        self.assertAlmostEqual(res[0], 2.4356757, 5,
-                               'Failed to calculate custom weighting')
+            self.assertFalse(len(w) != 1)
+            self.assertFalse(('Searching' not in str(w[0].message)))
+        self.assertAlmostEqual(res[0], 2.4356757, 5)
 
     def test_gauss_uncert(self):
         sigma = utils.fwhm2sigma(41627.730557884883)
         with catch_warnings() as w:
             res, stddev, count = kd_tree.resample_gauss(self.tswath, self.tdata,
                                                         self.tgrid, 100000, sigma,
                                                         with_uncert=True)
-            self.assertTrue(
-                len(w) > 0, 'Failed to create neighbour warning')
-            self.assertTrue((any('Searching' in str(_w.message) for _w in w)),
-                            'Failed to create correct neighbour warning')
+            self.assertTrue(len(w) > 0)
+            self.assertTrue((any('Searching' in str(_w.message) for _w in w)))
 
         expected_res = 2.20206560694
         expected_stddev = 0.707115076173
         expected_count = 3
-        self.assertAlmostEqual(res[0], expected_res, 5,
-                               'Failed to calculate gaussian weighting with uncertainty')
-        self.assertAlmostEqual(stddev[0], expected_stddev, 5,
-                               'Failed to calculate uncertainty for gaussian weighting')
-        self.assertEqual(
-            count[0], expected_count, 'Wrong data point count for gaussian weighting with uncertainty')
+        self.assertAlmostEqual(res[0], expected_res, 5)
+        self.assertAlmostEqual(stddev[0], expected_stddev, 5)
+        self.assertEqual(count[0], expected_count)
 
     def test_custom_uncert(self):
         def wf(dist):
             return 1 - dist / 100000.0
 
         with catch_warnings() as w:
             res, stddev, counts = kd_tree.resample_custom(self.tswath,
                                                           self.tdata, self.tgrid,
                                                           100000, wf, with_uncert=True)
-            self.assertTrue(
-                len(w) > 0, 'Failed to create neighbour warning')
-            self.assertTrue((any('Searching' in str(_w.message) for _w in w)),
-                            'Failed to create correct neighbour warning')
-
-        self.assertAlmostEqual(res[0], 2.32193149, 5,
-                               'Failed to calculate custom weighting with uncertainty')
-        self.assertAlmostEqual(stddev[0], 0.81817972, 5,
-                               'Failed to calculate custom for gaussian weighting')
-        self.assertEqual(
-            counts[0], 3, 'Wrong data point count for custom weighting with uncertainty')
+            self.assertTrue(len(w) > 0)
+            self.assertTrue((any('Searching' in str(_w.message) for _w in w)))
+
+        self.assertAlmostEqual(res[0], 2.32193149, 5)
+        self.assertAlmostEqual(stddev[0], 0.81817972, 5)
+        self.assertEqual(counts[0], 3)
 
     def test_nearest(self):
         data = numpy.fromfunction(lambda y, x: y * x, (50, 10))
         lons = numpy.fromfunction(lambda y, x: 3 + x, (50, 10))
         lats = numpy.fromfunction(lambda y, x: 75 - y, (50, 10))
         swath_def = geometry.SwathDefinition(lons=lons, lats=lats)
         res = kd_tree.resample_nearest(swath_def, data.ravel(),
                                        self.area_def, 50000, segments=1)
         cross_sum = res.sum()
         expected = 15874591.0
-        self.assertEqual(cross_sum, expected,
-                         msg='Swath resampling nearest failed')
+        self.assertEqual(cross_sum, expected)
 
     def test_nearest_masked_swath_target(self):
         """Test that a masked array works as a target."""
         data = numpy.fromfunction(lambda y, x: y * x, (50, 10))
         lons = numpy.fromfunction(lambda y, x: 3 + x, (50, 10))
         lats = numpy.fromfunction(lambda y, x: 75 - y, (50, 10))
         mask = numpy.ones_like(lons, dtype=numpy.bool)
@@ -139,42 +122,38 @@
             lats=numpy.ma.masked_array(lats, mask=False)
         )
         res = kd_tree.resample_nearest(swath_def, data.ravel(),
                                        swath_def, 50000, segments=3)
         cross_sum = res.sum()
         # expected = 12716  # if masks aren't respected
         expected = 12000
-        self.assertEqual(cross_sum, expected,
-                         msg='Swath resampling masked nearest failed')
+        self.assertEqual(cross_sum, expected)
 
     def test_nearest_1d(self):
         data = numpy.fromfunction(lambda x, y: x * y, (800, 800))
         lons = numpy.fromfunction(lambda x: 3 + x / 100., (500,))
         lats = numpy.fromfunction(lambda x: 75 - x / 10., (500,))
         swath_def = geometry.SwathDefinition(lons=lons, lats=lats)
         res = kd_tree.resample_nearest(self.area_def, data.ravel(),
                                        swath_def, 50000, segments=1)
         cross_sum = res.sum()
         expected = 35821299.0
-        self.assertEqual(res.shape, (500,),
-                         msg='Swath resampling nearest 1d failed')
-        self.assertEqual(cross_sum, expected,
-                         msg='Swath resampling nearest 1d failed')
+        self.assertEqual(res.shape, (500,))
+        self.assertEqual(cross_sum, expected)
 
     def test_nearest_empty(self):
         data = numpy.fromfunction(lambda y, x: y * x, (50, 10))
         lons = numpy.fromfunction(lambda y, x: 165 + x, (50, 10))
         lats = numpy.fromfunction(lambda y, x: 75 - y, (50, 10))
         swath_def = geometry.SwathDefinition(lons=lons, lats=lats)
         res = kd_tree.resample_nearest(swath_def, data.ravel(),
                                        self.area_def, 50000, segments=1)
         cross_sum = res.sum()
         expected = 0
-        self.assertEqual(cross_sum, expected,
-                         msg='Swath resampling nearest empty failed')
+        self.assertEqual(cross_sum, expected)
 
     def test_nearest_empty_multi(self):
         data = numpy.fromfunction(lambda y, x: y * x, (50, 10))
         lons = numpy.fromfunction(lambda y, x: 165 + x, (50, 10))
         lats = numpy.fromfunction(lambda y, x: 75 - y, (50, 10))
         data_multi = numpy.column_stack((data.ravel(), data.ravel(),
                                          data.ravel()))
@@ -190,165 +169,148 @@
         lats = numpy.fromfunction(lambda y, x: 75 - y, (50, 10))
         data_multi = numpy.column_stack((data.ravel(), data.ravel(),
                                          data.ravel()))
         swath_def = geometry.SwathDefinition(lons=lons, lats=lats)
         res = kd_tree.resample_nearest(swath_def, data_multi,
                                        self.area_def, 50000, segments=1,
                                        fill_value=None)
-        self.assertEqual(res.shape, (800, 800, 3),
-                         msg='Swath resampling nearest empty multi masked failed')
+        self.assertEqual(res.shape, (800, 800, 3))
 
     def test_nearest_empty_masked(self):
         data = numpy.fromfunction(lambda y, x: y * x, (50, 10))
         lons = numpy.fromfunction(lambda y, x: 165 + x, (50, 10))
         lats = numpy.fromfunction(lambda y, x: 75 - y, (50, 10))
         swath_def = geometry.SwathDefinition(lons=lons, lats=lats)
         res = kd_tree.resample_nearest(swath_def, data.ravel(),
                                        self.area_def, 50000, segments=1,
                                        fill_value=None)
         cross_sum = res.mask.sum()
         expected = res.size
-        self.assertTrue(cross_sum == expected,
-                        msg='Swath resampling nearest empty masked failed')
+        self.assertTrue(cross_sum == expected)
 
     def test_nearest_segments(self):
         data = numpy.fromfunction(lambda y, x: y * x, (50, 10))
         lons = numpy.fromfunction(lambda y, x: 3 + x, (50, 10))
         lats = numpy.fromfunction(lambda y, x: 75 - y, (50, 10))
         swath_def = geometry.SwathDefinition(lons=lons, lats=lats)
         res = kd_tree.resample_nearest(swath_def, data.ravel(),
                                        self.area_def, 50000, segments=2)
         cross_sum = res.sum()
         expected = 15874591.0
-        self.assertEqual(cross_sum, expected,
-                         msg='Swath resampling nearest segments failed')
+        self.assertEqual(cross_sum, expected)
 
     def test_nearest_remap(self):
         data = numpy.fromfunction(lambda y, x: y * x, (50, 10))
         lons = numpy.fromfunction(lambda y, x: 3 + x, (50, 10))
         lats = numpy.fromfunction(lambda y, x: 75 - y, (50, 10))
         swath_def = geometry.SwathDefinition(lons=lons, lats=lats)
         res = kd_tree.resample_nearest(swath_def, data.ravel(),
                                        self.area_def, 50000, segments=1)
         remap = kd_tree.resample_nearest(self.area_def, res.ravel(),
                                          swath_def, 5000, segments=1)
         cross_sum = remap.sum()
         expected = 22275.0
-        self.assertEqual(cross_sum, expected,
-                         msg='Grid remapping nearest failed')
+        self.assertEqual(cross_sum, expected)
 
     def test_nearest_mp(self):
         data = numpy.fromfunction(lambda y, x: y * x, (50, 10))
         lons = numpy.fromfunction(lambda y, x: 3 + x, (50, 10))
         lats = numpy.fromfunction(lambda y, x: 75 - y, (50, 10))
         swath_def = geometry.SwathDefinition(lons=lons, lats=lats)
         res = kd_tree.resample_nearest(swath_def, data.ravel(),
                                        self.area_def, 50000, nprocs=2, segments=1)
         cross_sum = res.sum()
         expected = 15874591.0
-        self.assertEqual(cross_sum, expected,
-                         msg='Swath resampling mp nearest failed')
+        self.assertEqual(cross_sum, expected)
 
     def test_nearest_multi(self):
         data = numpy.fromfunction(lambda y, x: y * x, (50, 10))
         lons = numpy.fromfunction(lambda y, x: 3 + x, (50, 10))
         lats = numpy.fromfunction(lambda y, x: 75 - y, (50, 10))
         swath_def = geometry.SwathDefinition(lons=lons, lats=lats)
         data_multi = numpy.column_stack((data.ravel(), data.ravel(),
                                          data.ravel()))
         res = kd_tree.resample_nearest(swath_def, data_multi,
                                        self.area_def, 50000, segments=1)
         cross_sum = res.sum()
         expected = 3 * 15874591.0
-        self.assertEqual(cross_sum, expected,
-                         msg='Swath multi channel resampling nearest failed')
+        self.assertEqual(cross_sum, expected)
 
     def test_nearest_multi_unraveled(self):
         data = numpy.fromfunction(lambda y, x: y * x, (50, 10))
         lons = numpy.fromfunction(lambda y, x: 3 + x, (50, 10))
         lats = numpy.fromfunction(lambda y, x: 75 - y, (50, 10))
         swath_def = geometry.SwathDefinition(lons=lons, lats=lats)
         data_multi = numpy.dstack((data, data, data))
         res = kd_tree.resample_nearest(swath_def, data_multi,
                                        self.area_def, 50000, segments=1)
         cross_sum = res.sum()
         expected = 3 * 15874591.0
-        self.assertEqual(cross_sum, expected,
-                         msg='Swath multi channel resampling nearest failed')
+        self.assertEqual(cross_sum, expected)
 
     def test_gauss_sparse(self):
         data = numpy.fromfunction(lambda y, x: y * x, (50, 10))
         lons = numpy.fromfunction(lambda y, x: 3 + x, (50, 10))
         lats = numpy.fromfunction(lambda y, x: 75 - y, (50, 10))
         swath_def = geometry.SwathDefinition(lons=lons, lats=lats)
         res = kd_tree.resample_gauss(swath_def, data.ravel(),
                                      self.area_def, 50000, 25000, fill_value=-1, segments=1)
         cross_sum = res.sum()
         expected = 15387753.9852
-        self.assertAlmostEqual(cross_sum, expected, places=3,
-                               msg='Swath gauss sparse nearest failed')
+        self.assertAlmostEqual(cross_sum, expected, places=3)
 
     def test_gauss(self):
         data = numpy.fromfunction(lambda y, x: (y + x) * 10 ** -5, (5000, 100))
         lons = numpy.fromfunction(
             lambda y, x: 3 + (10.0 / 100) * x, (5000, 100))
         lats = numpy.fromfunction(
             lambda y, x: 75 - (50.0 / 5000) * y, (5000, 100))
         swath_def = geometry.SwathDefinition(lons=lons, lats=lats)
         with catch_warnings() as w:
             res = kd_tree.resample_gauss(swath_def, data.ravel(),
                                          self.area_def, 50000, 25000, segments=1)
-            self.assertFalse(
-                len(w) != 1, 'Failed to create neighbour radius warning')
-            self.assertFalse(('Possible more' not in str(
-                w[0].message)), 'Failed to create correct neighbour radius warning')
-        cross_sum = res.sum()
-        expected = 4872.81050892
-        self.assertAlmostEqual(cross_sum, expected,
-                               msg='Swath resampling gauss failed')
+            self.assertFalse(len(w) != 1)
+            self.assertFalse(('Possible more' not in str(w[0].message)))
+        cross_sum = res.sum()
+        expected = 4872.8100353517921
+        self.assertAlmostEqual(cross_sum, expected)
 
     def test_gauss_fwhm(self):
         data = numpy.fromfunction(lambda y, x: (y + x) * 10 ** -5, (5000, 100))
         lons = numpy.fromfunction(
             lambda y, x: 3 + (10.0 / 100) * x, (5000, 100))
         lats = numpy.fromfunction(
             lambda y, x: 75 - (50.0 / 5000) * y, (5000, 100))
         swath_def = geometry.SwathDefinition(lons=lons, lats=lats)
         with catch_warnings() as w:
             res = kd_tree.resample_gauss(swath_def, data.ravel(),
                                          self.area_def, 50000, utils.fwhm2sigma(41627.730557884883), segments=1)
-            self.assertFalse(
-                len(w) != 1, 'Failed to create neighbour radius warning')
-            self.assertFalse(('Possible more' not in str(
-                w[0].message)), 'Failed to create correct neighbour radius warning')
-        cross_sum = res.sum()
-        expected = 4872.81050892
-        self.assertAlmostEqual(cross_sum, expected,
-                               msg='Swath resampling gauss failed')
+            self.assertFalse(len(w) != 1)
+            self.assertFalse(('Possible more' not in str(w[0].message)))
+        cross_sum = res.sum()
+        expected = 4872.8100353517921
+        self.assertAlmostEqual(cross_sum, expected)
 
     def test_gauss_multi(self):
         data = numpy.fromfunction(lambda y, x: (y + x) * 10 ** -6, (5000, 100))
         lons = numpy.fromfunction(
             lambda y, x: 3 + (10.0 / 100) * x, (5000, 100))
         lats = numpy.fromfunction(
             lambda y, x: 75 - (50.0 / 5000) * y, (5000, 100))
         swath_def = geometry.SwathDefinition(lons=lons, lats=lats)
         data_multi = numpy.column_stack((data.ravel(), data.ravel(),
                                          data.ravel()))
         with catch_warnings() as w:
             res = kd_tree.resample_gauss(swath_def, data_multi,
                                          self.area_def, 50000, [25000, 15000, 10000], segments=1)
-            self.assertFalse(
-                len(w) != 1, 'Failed to create neighbour radius warning')
-            self.assertFalse(('Possible more' not in str(
-                w[0].message)), 'Failed to create correct neighbour radius warning')
-        cross_sum = res.sum()
-        expected = 1461.84313918
-        self.assertAlmostEqual(cross_sum, expected,
-                               msg='Swath multi channel resampling gauss failed')
+            self.assertFalse(len(w) != 1)
+            self.assertFalse(('Possible more' not in str(w[0].message)))
+        cross_sum = res.sum()
+        expected = 1461.8429990248171
+        self.assertAlmostEqual(cross_sum, expected)
 
     def test_gauss_multi_uncert(self):
         data = numpy.fromfunction(lambda y, x: (y + x) * 10 ** -6, (5000, 100))
         lons = numpy.fromfunction(
             lambda y, x: 3 + (10.0 / 100) * x, (5000, 100))
         lats = numpy.fromfunction(
             lambda y, x: 75 - (50.0 / 5000) * y, (5000, 100))
@@ -360,33 +322,31 @@
             # and whether it contains a specific message from pyresample
             # On python 2.7.9+ the resample_gauss method raises multiple deprecation warnings
             # that cause to fail, so we ignore the unrelated warnings.
             res, stddev, counts = kd_tree.resample_gauss(swath_def, data_multi,
                                                          self.area_def, 50000, [
                                                              25000, 15000, 10000],
                                                          segments=1, with_uncert=True)
+            self.assertTrue(len(w) >= 1)
             self.assertTrue(
-                len(w) >= 1, 'Failed to create neighbour radius warning')
-            self.assertTrue(any(['Possible more' in str(
-                x.message) for x in w]), 'Failed to create correct neighbour radius warning')
+                any(['Possible more' in str(x.message) for x in w]))
         cross_sum = res.sum()
         cross_sum_counts = counts.sum()
-        expected = 1461.84313918
-        expected_stddev = [0.446193170875, 0.443606880035, 0.438586349519]
+        expected = 1461.8429990248171
+        expected_stddev = [0.44621800779801657, 0.44363137712896705,
+                           0.43861019464274459]
         expected_counts = 4934802.0
         self.assertTrue(res.shape == stddev.shape and stddev.shape ==
                         counts.shape and counts.shape == (800, 800, 3))
-        self.assertAlmostEqual(cross_sum, expected,
-                               msg='Swath multi channel resampling gauss failed on data')
+        self.assertAlmostEqual(cross_sum, expected)
+
         for i, e_stddev in enumerate(expected_stddev):
             cross_sum_stddev = stddev[:, :, i].sum()
-            self.assertAlmostEqual(cross_sum_stddev, e_stddev,
-                                   msg='Swath multi channel resampling gauss failed on stddev (channel {})'.format(i))
-        self.assertAlmostEqual(cross_sum_counts, expected_counts,
-                               msg='Swath multi channel resampling gauss failed on counts')
+            self.assertAlmostEqual(cross_sum_stddev, e_stddev)
+        self.assertAlmostEqual(cross_sum_counts, expected_counts)
 
     def test_gauss_multi_mp(self):
         data = numpy.fromfunction(lambda y, x: (y + x) * 10 ** -6, (5000, 100))
         lons = numpy.fromfunction(
             lambda y, x: 3 + (10.0 / 100) * x, (5000, 100))
         lats = numpy.fromfunction(
             lambda y, x: 75 - (50.0 / 5000) * y, (5000, 100))
@@ -394,22 +354,19 @@
         data_multi = numpy.column_stack((data.ravel(), data.ravel(),
                                          data.ravel()))
         with catch_warnings() as w:
             res = kd_tree.resample_gauss(swath_def, data_multi,
                                          self.area_def, 50000, [
                                              25000, 15000, 10000],
                                          nprocs=2, segments=1)
-            self.assertFalse(
-                len(w) != 1, 'Failed to create neighbour radius warning')
-            self.assertFalse(('Possible more' not in str(
-                w[0].message)), 'Failed to create correct neighbour radius warning')
-        cross_sum = res.sum()
-        expected = 1461.84313918
-        self.assertAlmostEqual(cross_sum, expected,
-                               msg='Swath multi channel resampling gauss failed')
+            self.assertFalse(len(w) != 1)
+            self.assertFalse(('Possible more' not in str(w[0].message)))
+        cross_sum = res.sum()
+        expected = 1461.8429990248171
+        self.assertAlmostEqual(cross_sum, expected)
 
     def test_gauss_multi_mp_segments(self):
         data = numpy.fromfunction(lambda y, x: (y + x) * 10 ** -6, (5000, 100))
         lons = numpy.fromfunction(
             lambda y, x: 3 + (10.0 / 100) * x, (5000, 100))
         lats = numpy.fromfunction(
             lambda y, x: 75 - (50.0 / 5000) * y, (5000, 100))
@@ -417,22 +374,19 @@
         data_multi = numpy.column_stack((data.ravel(), data.ravel(),
                                          data.ravel()))
         with catch_warnings() as w:
             res = kd_tree.resample_gauss(swath_def, data_multi,
                                          self.area_def, 50000, [
                                              25000, 15000, 10000],
                                          nprocs=2, segments=1)
-            self.assertFalse(
-                len(w) != 1, 'Failed to create neighbour radius warning')
-            self.assertFalse(('Possible more' not in str(
-                w[0].message)), 'Failed to create correct neighbour radius warning')
-        cross_sum = res.sum()
-        expected = 1461.84313918
-        self.assertAlmostEqual(cross_sum, expected,
-                               msg='Swath multi channel segments resampling gauss failed')
+            self.assertFalse(len(w) != 1)
+            self.assertFalse('Possible more' not in str(w[0].message))
+        cross_sum = res.sum()
+        expected = 1461.8429990248171
+        self.assertAlmostEqual(cross_sum, expected)
 
     def test_gauss_multi_mp_segments_empty(self):
         data = numpy.fromfunction(lambda y, x: (y + x) * 10 ** -6, (5000, 100))
         lons = numpy.fromfunction(
             lambda y, x: 165 + (10.0 / 100) * x, (5000, 100))
         lats = numpy.fromfunction(
             lambda y, x: 75 - (50.0 / 5000) * y, (5000, 100))
@@ -440,39 +394,34 @@
         data_multi = numpy.column_stack((data.ravel(), data.ravel(),
                                          data.ravel()))
         res = kd_tree.resample_gauss(swath_def, data_multi,
                                      self.area_def, 50000, [
                                          25000, 15000, 10000],
                                      nprocs=2, segments=1)
         cross_sum = res.sum()
-        self.assertTrue(cross_sum == 0,
-                        msg=('Swath multi channel segments empty '
-                             'resampling gauss failed'))
+        self.assertTrue(cross_sum == 0)
 
     def test_custom(self):
         def wf(dist):
             return 1 - dist / 100000.0
 
         data = numpy.fromfunction(lambda y, x: (y + x) * 10 ** -5, (5000, 100))
         lons = numpy.fromfunction(
             lambda y, x: 3 + (10.0 / 100) * x, (5000, 100))
         lats = numpy.fromfunction(
             lambda y, x: 75 - (50.0 / 5000) * y, (5000, 100))
         swath_def = geometry.SwathDefinition(lons=lons, lats=lats)
         with catch_warnings() as w:
             res = kd_tree.resample_custom(swath_def, data.ravel(),
                                           self.area_def, 50000, wf, segments=1)
-            self.assertFalse(
-                len(w) != 1, 'Failed to create neighbour radius warning')
-            self.assertFalse(('Possible more' not in str(
-                w[0].message)), 'Failed to create correct neighbour radius warning')
-        cross_sum = res.sum()
-        expected = 4872.81050729
-        self.assertAlmostEqual(cross_sum, expected,
-                               msg='Swath custom resampling failed')
+            self.assertFalse(len(w) != 1)
+            self.assertFalse(('Possible more' not in str(w[0].message)))
+        cross_sum = res.sum()
+        expected = 4872.8100347930776
+        self.assertAlmostEqual(cross_sum, expected)
 
     def test_custom_multi(self):
         def wf1(dist):
             return 1 - dist / 100000.0
 
         def wf2(dist):
             return 1
@@ -487,22 +436,19 @@
             lambda y, x: 75 - (50.0 / 5000) * y, (5000, 100))
         swath_def = geometry.SwathDefinition(lons=lons, lats=lats)
         data_multi = numpy.column_stack((data.ravel(), data.ravel(),
                                          data.ravel()))
         with catch_warnings() as w:
             res = kd_tree.resample_custom(swath_def, data_multi,
                                           self.area_def, 50000, [wf1, wf2, wf3], segments=1)
-            self.assertFalse(
-                len(w) != 1, 'Failed to create neighbour radius warning')
-            self.assertFalse(('Possible more' not in str(
-                w[0].message)), 'Failed to create correct neighbour radius warning')
-        cross_sum = res.sum()
-        expected = 1461.842980746
-        self.assertAlmostEqual(cross_sum, expected,
-                               msg='Swath multi channel custom resampling failed')
+            self.assertFalse(len(w) != 1)
+            self.assertFalse('Possible more' not in str(w[0].message))
+        cross_sum = res.sum()
+        expected = 1461.8428378742638
+        self.assertAlmostEqual(cross_sum, expected)
 
     def test_masked_nearest(self):
         data = numpy.ones((50, 10))
         data[:, 5:] = 2
         lons = numpy.fromfunction(lambda y, x: 3 + x, (50, 10))
         lats = numpy.fromfunction(lambda y, x: 75 - y, (50, 10))
         swath_def = geometry.SwathDefinition(lons=lons, lats=lats)
@@ -515,32 +461,29 @@
                                                     'test_files',
                                                     'mask_test_nearest_mask.dat'),
                                        sep=' ').reshape((800, 800))
         expected_data = numpy.fromfile(os.path.join(os.path.dirname(__file__),
                                                     'test_files',
                                                     'mask_test_nearest_data.dat'),
                                        sep=' ').reshape((800, 800))
-        self.assertTrue(numpy.array_equal(expected_mask, res.mask),
-                        msg='Resampling of swath mask failed')
-        self.assertTrue(numpy.array_equal(expected_data, res.data),
-                        msg='Resampling of swath masked data failed')
+        self.assertTrue(numpy.array_equal(expected_mask, res.mask))
+        self.assertTrue(numpy.array_equal(expected_data, res.data))
 
     def test_masked_nearest_1d(self):
         data = numpy.ones((800, 800))
         data[:400, :] = 2
         lons = numpy.fromfunction(lambda x: 3 + x / 100., (500,))
         lats = numpy.fromfunction(lambda x: 75 - x / 10., (500,))
         swath_def = geometry.SwathDefinition(lons=lons, lats=lats)
         mask = numpy.ones((800, 800))
         mask[400:, :] = 0
         masked_data = numpy.ma.array(data, mask=mask)
         res = kd_tree.resample_nearest(self.area_def, masked_data.ravel(),
                                        swath_def, 50000, segments=1)
-        self.assertEqual(res.mask.sum(), 108,
-                         msg='Swath resampling masked nearest 1d failed')
+        self.assertEqual(res.mask.sum(), 112)
 
     def test_masked_gauss(self):
         data = numpy.ones((50, 10))
         data[:, 5:] = 2
         lons = numpy.fromfunction(lambda y, x: 3 + x, (50, 10))
         lats = numpy.fromfunction(lambda y, x: 75 - y, (50, 10))
         swath_def = geometry.SwathDefinition(lons=lons, lats=lats)
@@ -556,48 +499,44 @@
         expected_data = numpy.fromfile(os.path.join(os.path.dirname(__file__),
                                                     'test_files',
                                                     'mask_test_data.dat'),
                                        sep=' ').reshape((800, 800))
         expected = expected_data.sum()
         cross_sum = res.data.sum()
 
-        self.assertTrue(numpy.array_equal(expected_mask, res.mask),
-                        msg='Gauss resampling of swath mask failed')
-        self.assertAlmostEqual(cross_sum, expected, places=3,
-                               msg='Gauss resampling of swath masked data failed')
+        self.assertTrue(numpy.array_equal(expected_mask, res.mask))
+        self.assertAlmostEqual(cross_sum, expected, places=3)
 
     def test_masked_fill_float(self):
         data = numpy.ones((50, 10))
         lons = numpy.fromfunction(lambda y, x: 3 + x, (50, 10))
         lats = numpy.fromfunction(lambda y, x: 75 - y, (50, 10))
         swath_def = geometry.SwathDefinition(lons=lons, lats=lats)
         res = kd_tree.resample_nearest(swath_def, data.ravel(),
                                        self.area_def, 50000, fill_value=None, segments=1)
         expected_fill_mask = numpy.fromfile(os.path.join(os.path.dirname(__file__),
                                                          'test_files',
                                                          'mask_test_fill_value.dat'),
                                             sep=' ').reshape((800, 800))
         fill_mask = res.mask
-        self.assertTrue(numpy.array_equal(fill_mask, expected_fill_mask),
-                        msg='Failed to create fill mask on float data')
+        self.assertTrue(numpy.array_equal(fill_mask, expected_fill_mask))
 
     def test_masked_fill_int(self):
         data = numpy.ones((50, 10)).astype('int')
         lons = numpy.fromfunction(lambda y, x: 3 + x, (50, 10))
         lats = numpy.fromfunction(lambda y, x: 75 - y, (50, 10))
         swath_def = geometry.SwathDefinition(lons=lons, lats=lats)
         res = kd_tree.resample_nearest(swath_def, data.ravel(),
                                        self.area_def, 50000, fill_value=None, segments=1)
         expected_fill_mask = numpy.fromfile(os.path.join(os.path.dirname(__file__),
                                                          'test_files',
                                                          'mask_test_fill_value.dat'),
                                             sep=' ').reshape((800, 800))
         fill_mask = res.mask
-        self.assertTrue(numpy.array_equal(fill_mask, expected_fill_mask),
-                        msg='Failed to create fill mask on integer data')
+        self.assertTrue(numpy.array_equal(fill_mask, expected_fill_mask))
 
     def test_masked_full(self):
         data = numpy.ones((50, 10))
         data[:, 5:] = 2
         mask = numpy.ones((50, 10))
         mask[:, :5] = 0
         masked_data = numpy.ma.array(data, mask=mask)
@@ -610,16 +549,15 @@
                                        fill_value=None, segments=1)
         expected_fill_mask = numpy.fromfile(os.path.join(os.path.dirname(__file__),
                                                          'test_files',
                                                          'mask_test_full_fill.dat'),
                                             sep=' ').reshape((800, 800))
         fill_mask = res.mask
 
-        self.assertTrue(numpy.array_equal(fill_mask, expected_fill_mask),
-                        msg='Failed to create fill mask on masked data')
+        self.assertTrue(numpy.array_equal(fill_mask, expected_fill_mask))
 
     def test_masked_full_multi(self):
         data = numpy.ones((50, 10))
         data[:, 5:] = 2
         mask1 = numpy.ones((50, 10))
         mask1[:, :5] = 0
         mask2 = numpy.ones((50, 10))
@@ -640,18 +578,16 @@
         expected_fill_mask = numpy.fromfile(os.path.join(os.path.dirname(__file__),
                                                          'test_files',
                                                          'mask_test_full_fill_multi.dat'),
                                             sep=' ').reshape((800, 800, 3))
         fill_mask = res.mask
         cross_sum = res.sum()
         expected = 357140.0
-        self.assertAlmostEqual(cross_sum, expected,
-                               msg='Failed to resample masked data')
-        self.assertTrue(numpy.array_equal(fill_mask, expected_fill_mask),
-                        msg='Failed to create fill mask on masked data')
+        self.assertAlmostEqual(cross_sum, expected)
+        self.assertTrue(numpy.array_equal(fill_mask, expected_fill_mask))
 
     def test_dtype(self):
         lons = numpy.fromfunction(lambda y, x: 3 + x, (50, 10))
         lats = numpy.fromfunction(lambda y, x: 75 - y, (50, 10))
         grid_def = geometry.GridDefinition(lons, lats)
         lons = numpy.asarray(lons, dtype='f4')
         lats = numpy.asarray(lats, dtype='f4')
@@ -671,16 +607,15 @@
                                        self.area_def,
                                        50000, neighbours=1, segments=1)
         res = kd_tree.get_sample_from_neighbour_info('nn', (800, 800), data.ravel(),
                                                      valid_input_index, valid_output_index,
                                                      index_array)
         cross_sum = res.sum()
         expected = 15874591.0
-        self.assertEqual(cross_sum, expected,
-                         msg='Swath resampling from neighbour info nearest failed')
+        self.assertEqual(cross_sum, expected)
 
     def test_custom_multi_from_sample(self):
         def wf1(dist):
             return 1 - dist / 100000.0
 
         def wf2(dist):
             return 1
@@ -698,41 +633,37 @@
                                          data.ravel()))
 
         with catch_warnings() as w:
             valid_input_index, valid_output_index, index_array, distance_array = \
                 kd_tree.get_neighbour_info(swath_def,
                                            self.area_def,
                                            50000, segments=1)
-            self.assertFalse(
-                len(w) != 1, 'Failed to create neighbour radius warning')
-            self.assertFalse(('Possible more' not in str(
-                w[0].message)), 'Failed to create correct neighbour radius warning')
+            self.assertFalse(len(w) != 1)
+            self.assertFalse(('Possible more' not in str(w[0].message)))
 
         res = kd_tree.get_sample_from_neighbour_info('custom', (800, 800),
                                                      data_multi,
                                                      valid_input_index, valid_output_index,
                                                      index_array, distance_array,
                                                      weight_funcs=[wf1, wf2, wf3])
 
         cross_sum = res.sum()
 
-        expected = 1461.842980746
-        self.assertAlmostEqual(cross_sum, expected,
-                               msg='Swath multi channel custom resampling from neighbour info failed 1')
+        expected = 1461.8428378742638
+        self.assertAlmostEqual(cross_sum, expected)
         res = kd_tree.get_sample_from_neighbour_info('custom', (800, 800),
                                                      data_multi,
                                                      valid_input_index, valid_output_index,
                                                      index_array, distance_array,
                                                      weight_funcs=[wf1, wf2, wf3])
 
         # Look for error where input data has been manipulated
         cross_sum = res.sum()
-        expected = 1461.842980746
-        self.assertAlmostEqual(cross_sum, expected,
-                               msg='Swath multi channel custom resampling from neighbour info failed 2')
+        expected = 1461.8428378742638
+        self.assertAlmostEqual(cross_sum, expected)
 
     def test_masked_multi_from_sample(self):
         data = numpy.ones((50, 10))
         data[:, 5:] = 2
         mask1 = numpy.ones((50, 10))
         mask1[:, :5] = 0
         mask2 = numpy.ones((50, 10))
@@ -757,16 +688,15 @@
                                                      valid_output_index, index_array,
                                                      fill_value=None)
         expected_fill_mask = numpy.fromfile(os.path.join(os.path.dirname(__file__),
                                                          'test_files',
                                                          'mask_test_full_fill_multi.dat'),
                                             sep=' ').reshape((800, 800, 3))
         fill_mask = res.mask
-        self.assertTrue(numpy.array_equal(fill_mask, expected_fill_mask),
-                        msg='Failed to create fill mask on masked data')
+        self.assertTrue(numpy.array_equal(fill_mask, expected_fill_mask))
 
 
 def suite():
     """The test suite.
     """
     loader = unittest.TestLoader()
     mysuite = unittest.TestSuite()
```

### Comparing `pyresample-1.9.2/pyresample/test/test_plot.py` & `pyresample-1.9.3/pyresample/test/test_plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,17 +42,17 @@
     lats = data[:, 1].astype(np.float64)
     tb37v = data[:, 2].astype(np.float64)
 
     # screen out the fill values
     fvalue = -10000000000.0
     valid_fov = (lons != fvalue) * (lats != fvalue) * (tb37v != fvalue)
     lons = lons[valid_fov]
-    lats = lats[valid_fov] 
+    lats = lats[valid_fov]
     tb37v = tb37v[valid_fov]
- 
+
     def test_ellps2axis(self):
         from pyresample import plot
         a, b = plot.ellps2axis('WGS84')
         self.assertAlmostEqual(a, 6378137.0,
                                msg='Failed to get semi-major axis of ellipsis')
         self.assertAlmostEqual(b, 6356752.3142451793,
                                msg='Failed to get semi-minor axis of ellipsis')
```

### Comparing `pyresample-1.9.2/pyresample/test/test_rotation.py` & `pyresample-1.9.3/pyresample/test/test_rotation.py`

 * *Files identical despite different names*

### Comparing `pyresample-1.9.2/pyresample/test/test_spherical.py` & `pyresample-1.9.3/pyresample/test/test_spherical.py`

 * *Files identical despite different names*

### Comparing `pyresample-1.9.2/pyresample/test/test_spherical_geometry.py` & `pyresample-1.9.3/pyresample/test/test_spherical_geometry.py`

 * *Files identical despite different names*

### Comparing `pyresample-1.9.2/pyresample/test/test_swath.py` & `pyresample-1.9.3/pyresample/test/test_swath.py`

 * *Files identical despite different names*

### Comparing `pyresample-1.9.2/pyresample/test/test_utils.py` & `pyresample-1.9.3/pyresample/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `pyresample-1.9.2/pyresample/test/utils.py` & `pyresample-1.9.3/pyresample/test/utils.py`

 * *Files identical despite different names*

### Comparing `pyresample-1.9.2/pyresample/__init__.py` & `pyresample-1.9.3/pyresample/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 # with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import os
 
 CHUNK_SIZE = int(os.getenv('PYTROLL_CHUNK_SIZE', 4096))
 
 from pyresample.version import __version__  # noqa
+
 # Backwards compatibility
 from pyresample import geometry  # noqa
 from pyresample import grid  # noqa
 from pyresample import image  # noqa
 from pyresample import kd_tree  # noqa
 from pyresample import utils  # noqa
 from pyresample import plot  # noqa
```

### Comparing `pyresample-1.9.2/pyresample/_cartopy.py` & `pyresample-1.9.3/pyresample/_cartopy.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,14 +56,15 @@
     globe = ccrs.Globe(**{_GLOBE_PARAMS[name]: value for name, value in
                           globe_terms})
     return globe
 
 
 # copy of class in cartopy (before it was released)
 class _PROJ4Projection(ccrs.Projection):
+
     def __init__(self, proj4_terms, globe=None, bounds=None):
         terms = proj4_str_to_dict(proj4_terms)
         globe = _globe_from_proj4(terms) if globe is None else globe
 
         other_terms = []
         for term in terms.items():
             if term[0] not in _GLOBE_PARAMS:
```

### Comparing `pyresample-1.9.2/pyresample/_multi_proc.py` & `pyresample-1.9.3/pyresample/_multi_proc.py`

 * *Files identical despite different names*

### Comparing `pyresample-1.9.2/pyresample/_spatial_mp.py` & `pyresample-1.9.3/pyresample/_spatial_mp.py`

 * *Files identical despite different names*

### Comparing `pyresample-1.9.2/pyresample/boundary.py` & `pyresample-1.9.3/pyresample/boundary.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 class AreaDefBoundary(AreaBoundary):
     """Boundaries for area definitions (pyresample).
     """
 
     def __init__(self, area, frequency=1):
         lons, lats = area.get_bbox_lonlats()
         AreaBoundary.__init__(self,
-                              *zip(*(lons, lats)))
+                              *zip(lons, lats))
 
         if frequency != 1:
             self.decimate(frequency)
 
 
 class SimpleBoundary(object):
     """Container for geometry boundary.
```

### Comparing `pyresample-1.9.2/pyresample/data_reduce.py` & `pyresample-1.9.3/pyresample/data_reduce.py`

 * *Files 3% similar despite different names*

```diff
@@ -268,28 +268,28 @@
                 angle_sum += delta
                 side_sum += delta
             prev = lon
 
     # Buffer min and max lon and lat of interest with radius of interest
     lat_min = min(lats_side1.min(), lats_side2.min(), lats_side3.min(),
                   lats_side4.min())
-    lat_min_buffered = lat_min - float(radius_of_influence) / R
+    lat_min_buffered = lat_min - np.degrees(float(radius_of_influence) / R)
     lat_max = max(lats_side1.max(), lats_side2.max(), lats_side3.max(),
                   lats_side4.max())
-    lat_max_buffered = lat_max + float(radius_of_influence) / R
+    lat_max_buffered = lat_max + np.degrees(float(radius_of_influence) / R)
 
     max_angle_s2 = max(abs(lats_side2.max()), abs(lats_side2.min()))
     max_angle_s4 = max(abs(lats_side4.max()), abs(lats_side4.min()))
     lon_min_buffered = (lons_side4.min() -
-                        float(radius_of_influence) /
-                        (np.sin(np.radians(max_angle_s4)) * R))
+                        np.degrees(float(radius_of_influence) /
+                                   (np.sin(np.radians(max_angle_s4)) * R)))
 
     lon_max_buffered = (lons_side2.max() +
-                        float(radius_of_influence) /
-                        (np.sin(np.radians(max_angle_s2)) * R))
+                        np.degrees(float(radius_of_influence) /
+                                   (np.sin(np.radians(max_angle_s2)) * R)))
 
     # From the winding number theorem follows:
     # angle_sum possiblilities:
     # -360: area covers north pole
     # 360: area covers south pole
     #   0: area covers no poles
     # else: area covers both poles
```

### Comparing `pyresample-1.9.2/pyresample/geo_filter.py` & `pyresample-1.9.3/pyresample/geo_filter.py`

 * *Files identical despite different names*

### Comparing `pyresample-1.9.2/pyresample/geometry.py` & `pyresample-1.9.3/pyresample/geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,14 +77,23 @@
         self.nprocs = nprocs
         self.lats = lats
         self.lons = lons
         self.ndim = None
         self.cartesian_coords = None
         self.hash = None
 
+    def __getitem__(self, key):
+        """Slice a 2D geographic definition."""
+        y_slice, x_slice = key
+        return self.__class__(
+            lons=self.lons[y_slice, x_slice],
+            lats=self.lats[y_slice, x_slice],
+            nprocs=self.nprocs
+        )
+
     def __hash__(self):
         """Compute the hash of this object."""
         if self.hash is None:
             self.hash = int(self.update_hash().hexdigest(), 16)
         return self.hash
 
     def __eq__(self, other):
@@ -539,38 +548,39 @@
         lines, cols = self.lons.shape
         lon1, lon2 = np.asanyarray(self.lons[[0, -1], int(cols / 2)])
         lat1, lat, lat2 = np.asanyarray(
             self.lats[[0, int(lines / 2), -1], int(cols / 2)])
 
         proj_dict2points = {'proj': 'omerc', 'lat_0': lat, 'ellps': ellipsoid,
                             'lat_1': lat1, 'lon_1': lon1,
-                            'lat_2': lat2, 'lon_2': lon2, 'no_rot': True}
+                            'lat_2': lat2, 'lon_2': lon2,
+                            'no_rot': True
+                            }
 
-        # return proj_dict2points
         # We need to compute alpha-based omerc for geotiff support
         lonc, lat0 = Proj(**proj_dict2points)(0, 0, inverse=True)
         az1, az2, dist = Geod(**proj_dict2points).inv(lonc, lat0, lon2, lat2)
         azimuth = az1
         az1, az2, dist = Geod(**proj_dict2points).inv(lonc, lat0, lon1, lat1)
         if abs(az1 - azimuth) > 1:
             if abs(az2 - azimuth) > 1:
                 logger.warning("Can't find appropriate azimuth.")
             else:
                 azimuth += az2
                 azimuth /= 2
         else:
             azimuth += az1
             azimuth /= 2
-
         if abs(azimuth) > 90:
             azimuth = 180 + azimuth
 
         prj_params = {'proj': 'omerc', 'alpha': float(azimuth),
                       'lat_0': float(lat0),  'lonc': float(lonc),
-                      'no_rot': True, 'ellps': ellipsoid}
+                      'gamma': 0,
+                      'ellps': ellipsoid}
 
         return prj_params
 
     def _compute_generic_parameters(self, projection, ellipsoid):
         """Compute the projection bb parameters for most projections."""
         lines, cols = self.lons.shape
         lat_0 = self.lats[int(lines / 2), int(cols / 2)]
@@ -610,17 +620,14 @@
         description = 'On-the-fly ' + projection + ' area'
         lines, cols = self.lons.shape
         x_size = int(cols * 1.1)
         y_size = int(lines * 1.1)
 
         proj_dict = self.compute_bb_proj_params(proj_dict)
 
-        if projection == 'omerc':
-            x_size, y_size = y_size, x_size
-
         area = DynamicAreaDefinition(area_id, description, proj_dict)
         lons, lats = self.get_edge_lonlats()
         return area.freeze((lons, lats), size=(x_size, y_size))
 
 
 class DynamicAreaDefinition(object):
     """An AreaDefintion containing just a subset of the needed parameters.
@@ -975,15 +982,15 @@
     def colrow2lonlat(self, cols, rows):
         """
         Return longitudes and latitudes for the given image columns
         and rows. Both scalars and arrays are supported.
         To be used with scarse data points instead of slices
         (see get_lonlats).
         """
-        p = Proj(self.proj4_string)
+        p = Proj(self.proj_str)
         x = self.projection_x_coords
         y = self.projection_y_coords
         return p(y[y.size - cols], x[x.size - rows], inverse=True)
 
     def lonlat2colrow(self, lons, lats):
         """
         Return image columns and rows for the given longitudes
@@ -1021,15 +1028,15 @@
             raise ValueError("Both lon and lat needs to be of " +
                              "the same type and have the same dimensions!")
 
         if isinstance(lon, np.ndarray) and isinstance(lat, np.ndarray):
             if lon.shape != lat.shape:
                 raise ValueError("lon and lat is not of the same shape!")
 
-        pobj = Proj(self.proj4_string)
+        pobj = Proj(self.proj_str)
         xm_, ym_ = pobj(lon, lat)
 
         return self.get_xy_from_proj_coords(xm_, ym_)
 
     def get_xy_from_proj_coords(self, xm, ym):
         """Find closest grid cell index for a specified projection coordinate.
 
@@ -1075,23 +1082,23 @@
         yscale = (self.area_extent[1] -
                   self.area_extent[3]) / float(self.y_size)
 
         x__ = (xm - upl_x) / xscale
         y__ = (ym - upl_y) / yscale
 
         if isinstance(x__, np.ndarray) and isinstance(y__, np.ndarray):
-            mask = (((x__ < 0) | (x__ > self.x_size)) |
-                    ((y__ < 0) | (y__ > self.y_size)))
+            mask = (((x__ < 0) | (x__ >= self.x_size)) |
+                    ((y__ < 0) | (y__ >= self.y_size)))
             return (np.ma.masked_array(x__.astype('int'), mask=mask,
                                        fill_value=-1, copy=False),
                     np.ma.masked_array(y__.astype('int'), mask=mask,
                                        fill_value=-1, copy=False))
         else:
-            if ((x__ < 0 or x__ > self.x_size) or
-                    (y__ < 0 or y__ > self.y_size)):
+            if ((x__ < 0 or x__ >= self.x_size) or
+                    (y__ < 0 or y__ >= self.y_size)):
                 raise ValueError('Point outside area:( %f %f)' % (x__, y__))
             return int(x__), int(y__)
 
     def get_lonlat(self, row, col):
         """Retrieves lon and lat values of single point in area grid
 
         Parameters
@@ -1320,54 +1327,61 @@
                 lons = self.lons[data_slice]
                 lats = self.lats[data_slice]
 
         return lons, lats
 
     @property
     def proj4_string(self):
-        """Returns projection definition as Proj.4 string"""
-
-        items = self.proj_dict.items()
-        return '+' + ' +'.join([t[0] + '=' + str(t[1]) for t in items])
+        """Return projection definition as Proj.4 string."""
+        warnings.warn("'proj4_string' is deprecated, please use 'proj_str' "
+                      "instead.", DeprecationWarning)
+        return utils.proj4_dict_to_str(self.proj_dict)
 
     def get_area_slices(self, area_to_cover):
         """Compute the slice to read based on an `area_to_cover`."""
         if not isinstance(area_to_cover, AreaDefinition):
             raise NotImplementedError('Only AreaDefinitions can be used')
 
-        if self.proj_dict['proj'] != 'geos':
-            raise NotImplementedError('Only geos supported')
-
         # Intersection only required for two different projections
-        if area_to_cover.proj_dict.get('proj') == self.proj_dict['proj']:
+        if area_to_cover.proj_str == self.proj_str:
             logger.debug('Projections for data and slice areas are'
                          ' identical: %s', area_to_cover.proj_dict['proj'])
             # Get xy coordinates
             llx, lly, urx, ury = area_to_cover.area_extent
             x, y = self.get_xy_from_proj_coords([llx, urx], [lly, ury])
 
             xstart = 0 if x[0] is np.ma.masked else x[0]
             ystart = 0 if y[1] is np.ma.masked else y[1]
             xstop = self.x_size if x[1] is np.ma.masked else x[1] + 1
             ystop = self.y_size if y[0] is np.ma.masked else y[0] + 1
 
             return slice(xstart, xstop), slice(ystart, ystop)
 
+        if self.proj_dict.get('proj') != 'geos':
+            raise NotImplementedError("Source projection must be 'geos' if "
+                                      "source/target projections are not "
+                                      "equal.")
+
         data_boundary = Boundary(*get_geostationary_bounding_box(self))
+        if area_to_cover.proj_dict['proj'] == 'geos':
+            area_boundary = Boundary(
+                *get_geostationary_bounding_box(area_to_cover))
+        else:
+            area_boundary = AreaDefBoundary(area_to_cover, 100)
 
-        area_boundary = AreaDefBoundary(area_to_cover, 100)
         intersection = data_boundary.contour_poly.intersection(
             area_boundary.contour_poly)
         if intersection is None:
             logger.debug('Cannot determine appropriate slicing.')
             raise NotImplementedError
         x, y = self.get_xy_from_lonlat(np.rad2deg(intersection.lon),
                                        np.rad2deg(intersection.lat))
 
-        return slice(min(x), max(x) + 1), slice(min(y), max(y) + 1)
+        return (slice(np.ma.min(x), np.ma.max(x) + 1),
+                slice(np.ma.min(y), np.ma.max(y) + 1))
 
     def crop_around(self, other_area):
         """Crop this area around `other_area`."""
         xslice, yslice = self.get_area_slices(other_area)
         return self[yslice, xslice]
 
     def __getitem__(self, key):
@@ -1417,16 +1431,16 @@
     Args:
       nb_points: Number of points on the polygon
     """
     xmax, ymax = get_geostationary_angle_extent(geos_area)
 
     # generate points around the north hemisphere in satellite projection
     # make it a bit smaller so that we stay inside the valid area
-    x = np.cos(np.linspace(-np.pi, 0, nb_points / 2)) * (xmax - 0.0001)
-    y = -np.sin(np.linspace(-np.pi, 0, nb_points / 2)) * (ymax - 0.0001)
+    x = np.cos(np.linspace(-np.pi, 0, int(nb_points / 2))) * (xmax - 0.0001)
+    y = -np.sin(np.linspace(-np.pi, 0, int(nb_points / 2))) * (ymax - 0.0001)
 
     ll_x, ll_y, ur_x, ur_y = geos_area.area_extent
 
     x *= geos_area.proj_dict['h']
     y *= geos_area.proj_dict['h']
 
     x = np.clip(np.concatenate([x, x[::-1]]), min(ll_x, ur_x), max(ll_x, ur_x))
@@ -1576,15 +1590,27 @@
             return self.defs[0]
         else:
             return self
 
     @property
     def proj4_string(self):
         """Returns projection definition as Proj.4 string"""
-        return self.defs[0].proj4_string
+        warnings.warn("'proj4_string' is deprecated, please use 'proj_str' "
+                      "instead.", DeprecationWarning)
+        return self.defs[0].proj_str
+
+    @property
+    def proj_str(self):
+        """Returns projection definition as Proj.4 string"""
+        return self.defs[0].proj_str
+
+    def update_hash(self, the_hash=None):
+        for areadef in self.defs:
+            the_hash = areadef.update_hash(the_hash)
+        return the_hash
 
 
 def _get_slice(segments, shape):
     """Generator for segmenting a 1D or 2D array"""
 
     if not (1 <= len(shape) <= 2):
         raise ValueError('Cannot segment array of shape: %s' % str(shape))
```

### Comparing `pyresample-1.9.2/pyresample/grid.py` & `pyresample-1.9.3/pyresample/grid.py`

 * *Files identical despite different names*

### Comparing `pyresample-1.9.2/pyresample/image.py` & `pyresample-1.9.3/pyresample/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -348,15 +348,15 @@
     nprocs : int
         Number of processor cores to be used
     segments : int or None
         Number of segments to use when resampling
     """
 
     def __init__(self, image_data, geo_def, radius_of_influence, epsilon=0,
-                 fill_value=0, reduce_data=True, nprocs=1, segments=None,
+                 fill_value=0, reduce_data=False, nprocs=1, segments=None,
                  neighbours=32):
         super(ImageContainerBilinear, self).__init__(image_data, geo_def,
                                                      fill_value=fill_value,
                                                      nprocs=nprocs)
         self.radius_of_influence = radius_of_influence
         self.epsilon = epsilon
         self.reduce_data = reduce_data
```

### Comparing `pyresample-1.9.2/pyresample/kd_tree.py` & `pyresample-1.9.3/pyresample/kd_tree.py`

 * *Files identical despite different names*

### Comparing `pyresample-1.9.2/pyresample/plot.py` & `pyresample-1.9.3/pyresample/plot.py`

 * *Files identical despite different names*

### Comparing `pyresample-1.9.2/pyresample/spherical.py` & `pyresample-1.9.3/pyresample/spherical.py`

 * *Files identical despite different names*

### Comparing `pyresample-1.9.2/pyresample/spherical_geometry.py` & `pyresample-1.9.3/pyresample/spherical_geometry.py`

 * *Files identical despite different names*

### Comparing `pyresample-1.9.2/pyresample/utils.py` & `pyresample-1.9.3/pyresample/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -426,29 +426,24 @@
     """
     pairs = (x.split('=', 1) for x in proj4_str.replace('+', '').split(" "))
     return dict((x[0], (x[1] if len(x) == 2 else True)) for x in pairs)
 
 
 def proj4_dict_to_str(proj4_dict, sort=False):
     """Convert a dictionary of PROJ.4 parameters to a valid PROJ.4 string"""
-    keys = proj4_dict.keys()
+    items = proj4_dict.items()
     if sort:
-        keys = sorted(keys)
+        items = sorted(items)
     params = []
-    for key in keys:
-        val = proj4_dict[key]
+    for key, val in items:
         key = str(key) if key.startswith('+') else '+' + str(key)
-        if str(val) in ['True', 'False']:
-            # could be string or boolean object
-            val = ''
-        if val:
-            param = '{}={}'.format(key, val)
-        else:
-            # example "+no_defs"
+        if key in ['+no_defs', '+no_off', '+no_rot']:
             param = key
+        else:
+            param = '{}={}'.format(key, val)
         params.append(param)
     return ' '.join(params)
 
 
 def proj4_radius_parameters(proj4_dict):
     """Calculate 'a' and 'b' radius parameters.
```

### Comparing `pyresample-1.9.2/pyresample/version.py` & `pyresample-1.9.3/pyresample/version.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-__version__ = '1.9.2'
+__version__ = '1.9.3'
```

### Comparing `pyresample-1.9.2/pyresample.egg-info/PKG-INFO` & `pyresample-1.9.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,21 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pyresample
-Version: 1.9.2
+Version: 1.9.3
 Summary: Resampling of remote sensing data in Python
 Home-page: UNKNOWN
 Author: Thomas Lavergne
 Author-email: t.lavergne@met.no
 License: UNKNOWN
-Description-Content-Type: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*
+Provides-Extra: numexpr
+Provides-Extra: dask
+Provides-Extra: pykdtree
+Provides-Extra: quicklook
```

### Comparing `pyresample-1.9.2/pyresample.egg-info/SOURCES.txt` & `pyresample-1.9.3/pyresample.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 pyresample.egg-info/PKG-INFO
 pyresample.egg-info/SOURCES.txt
 pyresample.egg-info/dependency_links.txt
 pyresample.egg-info/not-zip-safe
 pyresample.egg-info/requires.txt
 pyresample.egg-info/top_level.txt
 pyresample/bilinear/__init__.py
+pyresample/bilinear/xarr.py
 pyresample/ewa/__init__.py
 pyresample/ewa/_fornav.cpp
 pyresample/ewa/_fornav_templates.cpp
 pyresample/ewa/_fornav_templates.h
 pyresample/ewa/_ll2cr.c
 pyresample/test/__init__.py
 pyresample/test/test_bilinear.py
```

### Comparing `pyresample-1.9.2/LICENSE.txt` & `pyresample-1.9.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyresample-1.9.2/README` & `pyresample-1.9.3/README`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 [![Build Status](https://travis-ci.org/pytroll/pyresample.svg?branch=master)](https://travis-ci.org/pytroll/pyresample)
 [![Build status](https://ci.appveyor.com/api/projects/status/a34o4utf8dqjsob1/branch/master?svg=true)](https://ci.appveyor.com/project/pytroll/pyresample/branch/master)
 [![codebeat badge](https://codebeat.co/badges/2b9f14bc-758c-4fe1-967d-85b11e934983)](https://codebeat.co/projects/github-com-pytroll-pyresample-master)
 
-
 Python package for geospatial resampling
 ----------------------------------------
 
 Resampling (reprojection) of geospatial image data in Python.
 Pyresample uses a kd-tree approach for resampling.
 Pyresample is designed for resampling of remote sensing data and supports resampling from both fixed grids and geolocated swath data.
 Several types of resampling are supported including nearest neighbour, gaussian weighting and weighting with a user defined radial function.
```

### Comparing `pyresample-1.9.2/setup.py` & `pyresample-1.9.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -109,14 +109,15 @@
     setup(name='pyresample',
           version=version.__version__,
           description='Resampling of remote sensing data in Python',
           author='Thomas Lavergne',
           author_email='t.lavergne@met.no',
           package_dir={'pyresample': 'pyresample'},
           packages=find_packages(),
+          python_requires='>=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*',
           setup_requires=['numpy'],
           install_requires=requirements,
           extras_require=extras_require,
           tests_require=test_requires,
           cmdclass={'build_ext': build_ext},
           ext_modules=cythonize(extensions),
           test_suite='pyresample.test.suite',
```

### Comparing `pyresample-1.9.2/PKG-INFO` & `pyresample-1.9.3/pyresample.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,21 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pyresample
-Version: 1.9.2
+Version: 1.9.3
 Summary: Resampling of remote sensing data in Python
 Home-page: UNKNOWN
 Author: Thomas Lavergne
 Author-email: t.lavergne@met.no
 License: UNKNOWN
-Description-Content-Type: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*
+Provides-Extra: numexpr
+Provides-Extra: dask
+Provides-Extra: pykdtree
+Provides-Extra: quicklook
```

