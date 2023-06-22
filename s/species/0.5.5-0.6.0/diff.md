# Comparing `tmp/species-0.5.5.tar.gz` & `tmp/species-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "species-0.5.5.tar", last modified: Fri Feb  3 12:01:53 2023, max compression
+gzip compressed data, was "species-0.6.0.tar", last modified: Thu Jun 22 07:22:21 2023, max compression
```

## Comparing `species-0.5.5.tar` & `species-0.6.0.tar`

### file list

```diff
@@ -1,76 +1,77 @@
-drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2023-02-03 12:01:53.778542 species-0.5.5/
--rw-r--r--   0 tomasstolker   (501) staff       (20)     1075 2022-05-29 12:41:46.000000 species-0.5.5/LICENSE
--rw-r--r--   0 tomasstolker   (501) staff       (20)     3940 2023-02-03 12:01:53.778350 species-0.5.5/PKG-INFO
--rw-r--r--   0 tomasstolker   (501) staff       (20)     3133 2022-12-15 20:50:46.000000 species-0.5.5/README.rst
--rw-r--r--   0 tomasstolker   (501) staff       (20)       38 2023-02-03 12:01:53.778590 species-0.5.5/setup.cfg
--rw-r--r--   0 tomasstolker   (501) staff       (20)     1323 2023-02-03 10:24:04.000000 species-0.5.5/setup.py
-drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2023-02-03 12:01:53.736320 species-0.5.5/species/
--rw-r--r--   0 tomasstolker   (501) staff       (20)     2017 2023-02-03 10:24:11.000000 species-0.5.5/species/__init__.py
-drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2023-02-03 12:01:53.741881 species-0.5.5/species/analysis/
--rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2021-02-06 22:03:48.000000 species-0.5.5/species/analysis/__init__.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    22982 2022-08-24 12:16:37.000000 species-0.5.5/species/analysis/compare_spectra.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    43944 2023-01-02 10:50:47.000000 species-0.5.5/species/analysis/emission_line.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    74425 2022-11-09 14:05:33.000000 species-0.5.5/species/analysis/fit_model.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     6386 2022-07-21 11:40:43.000000 species-0.5.5/species/analysis/fit_spectrum.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    16952 2022-06-26 09:54:50.000000 species-0.5.5/species/analysis/photometry.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)   130234 2023-02-02 16:23:45.000000 species-0.5.5/species/analysis/retrieval.py
-drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2023-02-03 12:01:53.744152 species-0.5.5/species/core/
--rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2021-02-06 22:03:48.000000 species-0.5.5/species/core/__init__.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    14252 2022-11-25 15:06:19.000000 species-0.5.5/species/core/box.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)      743 2022-11-09 14:03:32.000000 species-0.5.5/species/core/constants.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     4109 2022-07-12 21:00:15.000000 species-0.5.5/species/core/init.py
-drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2023-02-03 12:01:53.754828 species-0.5.5/species/data/
--rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2021-02-06 22:03:48.000000 species-0.5.5/species/data/__init__.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     4078 2023-01-02 11:36:48.000000 species-0.5.5/species/data/accretion.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     5200 2022-12-15 12:34:30.000000 species-0.5.5/species/data/allers2013.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     4199 2022-12-15 12:39:38.000000 species-0.5.5/species/data/bonnefoy2014.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    51846 2023-01-31 11:08:46.000000 species-0.5.5/species/data/companion_data.json
--rw-r--r--   0 tomasstolker   (501) staff       (20)     1948 2022-12-23 10:17:11.000000 species-0.5.5/species/data/companion_spectra.json
--rw-r--r--   0 tomasstolker   (501) staff       (20)     2525 2022-12-23 10:17:11.000000 species-0.5.5/species/data/companion_spectra.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)   143755 2023-02-02 19:13:40.000000 species-0.5.5/species/data/database.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     6308 2022-05-29 12:41:46.000000 species-0.5.5/species/data/dust.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     6703 2022-06-26 07:25:19.000000 species-0.5.5/species/data/filters.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     6226 2022-12-23 10:17:11.000000 species-0.5.5/species/data/irtf.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    14343 2022-12-15 12:17:09.000000 species-0.5.5/species/data/isochrones.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     2878 2022-12-15 12:48:41.000000 species-0.5.5/species/data/kesseli2017.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     6258 2022-12-15 12:40:56.000000 species-0.5.5/species/data/leggett.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     7528 2023-01-13 12:30:04.000000 species-0.5.5/species/data/model_data.json
--rw-r--r--   0 tomasstolker   (501) staff       (20)     9697 2023-01-13 12:28:28.000000 species-0.5.5/species/data/model_spectra.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     8386 2022-09-24 12:24:11.000000 species-0.5.5/species/data/spex.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     1873 2022-05-29 12:41:46.000000 species-0.5.5/species/data/vega.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     3449 2023-01-02 10:50:47.000000 species-0.5.5/species/data/vlm_plx.py
-drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2023-02-03 12:01:53.759225 species-0.5.5/species/plot/
--rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2021-02-06 22:03:48.000000 species-0.5.5/species/plot/__init__.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    58221 2022-12-23 10:17:11.000000 species-0.5.5/species/plot/plot_color.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    22045 2022-12-23 10:17:11.000000 species-0.5.5/species/plot/plot_comparison.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    45973 2022-12-23 10:17:11.000000 species-0.5.5/species/plot/plot_mcmc.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    42502 2023-02-02 16:21:26.000000 species-0.5.5/species/plot/plot_retrieval.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    47725 2023-01-26 13:53:56.000000 species-0.5.5/species/plot/plot_spectrum.py
-drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2023-02-03 12:01:53.771353 species-0.5.5/species/read/
--rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2021-02-06 22:03:48.000000 species-0.5.5/species/read/__init__.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    12507 2022-07-14 13:37:28.000000 species-0.5.5/species/read/read_calibration.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    13069 2022-05-29 12:41:46.000000 species-0.5.5/species/read/read_color.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     5296 2022-11-25 10:55:33.000000 species-0.5.5/species/read/read_filter.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    33326 2023-01-02 13:29:10.000000 species-0.5.5/species/read/read_isochrone.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    61351 2023-01-12 12:02:52.000000 species-0.5.5/species/read/read_model.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     8390 2022-07-13 13:25:56.000000 species-0.5.5/species/read/read_object.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    15518 2022-10-13 14:09:49.000000 species-0.5.5/species/read/read_planck.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    44687 2022-12-05 07:06:36.000000 species-0.5.5/species/read/read_radtrans.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    11238 2022-09-24 08:55:45.000000 species-0.5.5/species/read/read_spectrum.py
-drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2023-02-03 12:01:53.778010 species-0.5.5/species/util/
--rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2021-02-06 22:03:48.000000 species-0.5.5/species/util/__init__.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    36034 2023-01-12 13:15:01.000000 species-0.5.5/species/util/data_util.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    20237 2023-01-02 10:50:47.000000 species-0.5.5/species/util/dust_util.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    16733 2022-08-22 10:12:45.000000 species-0.5.5/species/util/phot_util.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    28048 2023-01-26 13:53:49.000000 species-0.5.5/species/util/plot_util.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     8130 2022-05-29 12:41:46.000000 species-0.5.5/species/util/query_util.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    22045 2022-11-09 14:05:33.000000 species-0.5.5/species/util/read_util.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    87152 2023-02-02 16:20:42.000000 species-0.5.5/species/util/retrieval_util.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)      770 2022-06-25 07:27:57.000000 species-0.5.5/species/util/test_util.py
-drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2023-02-03 12:01:53.737610 species-0.5.5/species.egg-info/
--rw-r--r--   0 tomasstolker   (501) staff       (20)     3940 2023-02-03 12:01:53.000000 species-0.5.5/species.egg-info/PKG-INFO
--rw-r--r--   0 tomasstolker   (501) staff       (20)     1748 2023-02-03 12:01:53.000000 species-0.5.5/species.egg-info/SOURCES.txt
--rw-r--r--   0 tomasstolker   (501) staff       (20)        1 2023-02-03 12:01:53.000000 species-0.5.5/species.egg-info/dependency_links.txt
--rw-r--r--   0 tomasstolker   (501) staff       (20)        1 2023-02-03 12:01:53.000000 species-0.5.5/species.egg-info/not-zip-safe
--rw-r--r--   0 tomasstolker   (501) staff       (20)      341 2023-02-03 12:01:53.000000 species-0.5.5/species.egg-info/requires.txt
--rw-r--r--   0 tomasstolker   (501) staff       (20)        8 2023-02-03 12:01:53.000000 species-0.5.5/species.egg-info/top_level.txt
+drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2023-06-22 07:22:21.191058 species-0.6.0/
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     1075 2022-05-29 12:41:46.000000 species-0.6.0/LICENSE
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     4015 2023-06-22 07:22:21.190853 species-0.6.0/PKG-INFO
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     3208 2023-03-19 14:40:07.000000 species-0.6.0/README.rst
+-rw-r--r--   0 tomasstolker   (501) staff       (20)       38 2023-06-22 07:22:21.191111 species-0.6.0/setup.cfg
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     1323 2023-06-22 05:51:33.000000 species-0.6.0/setup.py
+drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2023-06-22 07:22:21.161066 species-0.6.0/species/
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     2017 2023-06-22 05:51:20.000000 species-0.6.0/species/__init__.py
+drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2023-06-22 07:22:21.167252 species-0.6.0/species/analysis/
+-rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2021-02-06 22:03:48.000000 species-0.6.0/species/analysis/__init__.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    26961 2023-06-05 15:59:19.000000 species-0.6.0/species/analysis/compare_spectra.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    43756 2023-04-17 14:50:32.000000 species-0.6.0/species/analysis/emission_line.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    80996 2023-06-20 18:54:02.000000 species-0.6.0/species/analysis/fit_model.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     6386 2022-07-21 11:40:43.000000 species-0.6.0/species/analysis/fit_spectrum.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    23668 2023-06-16 13:27:39.000000 species-0.6.0/species/analysis/photometry.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)   130234 2023-03-16 14:00:31.000000 species-0.6.0/species/analysis/retrieval.py
+drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2023-06-22 07:22:21.169160 species-0.6.0/species/core/
+-rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2021-02-06 22:03:48.000000 species-0.6.0/species/core/__init__.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    14876 2023-04-21 08:36:46.000000 species-0.6.0/species/core/box.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)      743 2023-03-16 14:00:31.000000 species-0.6.0/species/core/constants.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     4562 2023-06-16 10:36:58.000000 species-0.6.0/species/core/init.py
+drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2023-06-22 07:22:21.175402 species-0.6.0/species/data/
+-rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2021-02-06 22:03:48.000000 species-0.6.0/species/data/__init__.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     4078 2023-03-16 14:00:31.000000 species-0.6.0/species/data/accretion.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     5200 2023-03-16 14:00:31.000000 species-0.6.0/species/data/allers2013.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     4199 2023-03-16 14:00:31.000000 species-0.6.0/species/data/bonnefoy2014.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    52815 2023-06-22 05:50:45.000000 species-0.6.0/species/data/companion_data.json
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     1948 2023-03-16 14:00:31.000000 species-0.6.0/species/data/companion_spectra.json
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     2525 2023-03-16 14:00:31.000000 species-0.6.0/species/data/companion_spectra.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     9202 2023-03-16 14:00:31.000000 species-0.6.0/species/data/custom_model.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)   148669 2023-06-12 10:22:15.000000 species-0.6.0/species/data/database.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     6308 2022-05-29 12:41:46.000000 species-0.6.0/species/data/dust.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     6703 2023-05-08 16:54:49.000000 species-0.6.0/species/data/filters.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     6273 2023-03-16 14:00:31.000000 species-0.6.0/species/data/irtf.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    20923 2023-03-16 14:15:42.000000 species-0.6.0/species/data/isochrones.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     2878 2023-03-16 14:00:31.000000 species-0.6.0/species/data/kesseli2017.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     6258 2023-03-16 14:00:31.000000 species-0.6.0/species/data/leggett.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     8626 2023-06-19 10:01:20.000000 species-0.6.0/species/data/model_data.json
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     9684 2023-06-19 10:02:32.000000 species-0.6.0/species/data/model_spectra.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     8386 2023-05-12 10:02:35.000000 species-0.6.0/species/data/spex.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     2740 2023-06-16 12:46:44.000000 species-0.6.0/species/data/vega.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     3449 2023-03-16 14:00:31.000000 species-0.6.0/species/data/vlm_plx.py
+drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2023-06-22 07:22:21.179049 species-0.6.0/species/plot/
+-rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2021-02-06 22:03:48.000000 species-0.6.0/species/plot/__init__.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    60439 2023-06-21 08:40:35.000000 species-0.6.0/species/plot/plot_color.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    24103 2023-06-04 08:00:13.000000 species-0.6.0/species/plot/plot_comparison.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    46122 2023-04-17 08:43:33.000000 species-0.6.0/species/plot/plot_mcmc.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    42647 2023-04-17 15:27:47.000000 species-0.6.0/species/plot/plot_retrieval.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    49153 2023-06-12 19:35:57.000000 species-0.6.0/species/plot/plot_spectrum.py
+drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2023-06-22 07:22:21.185854 species-0.6.0/species/read/
+-rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2021-02-06 22:03:48.000000 species-0.6.0/species/read/__init__.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    12507 2023-03-26 10:33:11.000000 species-0.6.0/species/read/read_calibration.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    13069 2022-05-29 12:41:46.000000 species-0.6.0/species/read/read_color.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     6638 2023-03-26 11:37:54.000000 species-0.6.0/species/read/read_filter.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    54599 2023-05-04 10:42:41.000000 species-0.6.0/species/read/read_isochrone.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    68123 2023-05-08 16:54:49.000000 species-0.6.0/species/read/read_model.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     8390 2022-07-13 13:25:56.000000 species-0.6.0/species/read/read_object.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    15518 2022-10-13 14:09:49.000000 species-0.6.0/species/read/read_planck.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    44622 2023-04-17 15:27:32.000000 species-0.6.0/species/read/read_radtrans.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    11148 2023-06-07 11:14:31.000000 species-0.6.0/species/read/read_spectrum.py
+drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2023-06-22 07:22:21.190464 species-0.6.0/species/util/
+-rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2021-02-06 22:03:48.000000 species-0.6.0/species/util/__init__.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    36034 2023-03-16 14:00:31.000000 species-0.6.0/species/util/data_util.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    21688 2023-03-26 20:37:58.000000 species-0.6.0/species/util/dust_util.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    18476 2023-05-08 15:45:51.000000 species-0.6.0/species/util/phot_util.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    36146 2023-06-21 07:57:22.000000 species-0.6.0/species/util/plot_util.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     8130 2022-05-29 12:41:46.000000 species-0.6.0/species/util/query_util.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    22808 2023-03-16 14:34:00.000000 species-0.6.0/species/util/read_util.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    87152 2023-03-16 14:00:31.000000 species-0.6.0/species/util/retrieval_util.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)      770 2022-06-25 07:27:57.000000 species-0.6.0/species/util/test_util.py
+drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2023-06-22 07:22:21.162951 species-0.6.0/species.egg-info/
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     4015 2023-06-22 07:22:20.000000 species-0.6.0/species.egg-info/PKG-INFO
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     1777 2023-06-22 07:22:21.000000 species-0.6.0/species.egg-info/SOURCES.txt
+-rw-r--r--   0 tomasstolker   (501) staff       (20)        1 2023-06-22 07:22:20.000000 species-0.6.0/species.egg-info/dependency_links.txt
+-rw-r--r--   0 tomasstolker   (501) staff       (20)        1 2023-06-22 07:22:20.000000 species-0.6.0/species.egg-info/not-zip-safe
+-rw-r--r--   0 tomasstolker   (501) staff       (20)      373 2023-06-22 07:22:20.000000 species-0.6.0/species.egg-info/requires.txt
+-rw-r--r--   0 tomasstolker   (501) staff       (20)        8 2023-06-22 07:22:20.000000 species-0.6.0/species.egg-info/top_level.txt
```

### Comparing `species-0.5.5/LICENSE` & `species-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `species-0.5.5/PKG-INFO` & `species-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: species
-Version: 0.5.5
+Version: 0.6.0
 Summary: Toolkit for atmospheric characterization of directly imaged exoplanets
 Home-page: https://github.com/tomasstolker/species
 Author: Tomas Stolker
 Author-email: stolker@strw.leidenuniv.nl
 License: MIT
 Project-URL: Documentation, https://species.readthedocs.io
 Keywords: species
@@ -45,15 +45,17 @@
 
 .. image:: https://img.shields.io/github/license/tomasstolker/species
    :target: https://github.com/tomasstolker/species/blob/main/LICENSE
 
 .. image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/tomasstolker/species/HEAD
 
-*species* is a toolkit for atmospheric characterization of directly imaged exoplanets. It provides a coherent framework for spectral and photometric analysis which builds on publicly-available data and models from various resources. There are tools available for both grid retrievals and free retrievals with Bayesian inference, color-magnitude and color-color diagrams, a variety of model grids, empirical spectral analysis, spectral and photometric calibration, analysis of emission lines, and synthetic photometry. The package has been released on `PyPI <https://pypi.org/project/species/>`_ and is actively developed and maintained on Github.
+*species* is a toolkit for atmospheric characterization of directly imaged exoplanets. It provides a coherent framework for spectral and photometric analysis which builds on publicly-available data and models from various resources.
+
+There are tools available for grid and free retrievals using Bayesian inference, synthetic photometry, interpolating a variety atmospheric and evolutionary model grids (including the possibility to add a custom grid), color-magnitude and color-color diagrams, empirical spectral analysis, spectral and photometric calibration, and analysis of emission lines. The package has been released on `PyPI <https://pypi.org/project/species/>`_ and is actively developed and maintained on Github.
 
 Documentation
 -------------
 
 Documentation can be found at `http://species.readthedocs.io <http://species.readthedocs.io>`_.
 
 Tutorials
@@ -70,12 +72,12 @@
 ------------
 
 Contributions are welcome so please consider `forking <https://help.github.com/en/articles/fork-a-repo>`_ the repository and creating a `pull request <https://github.com/tomasstolker/pycrires/pulls>`_. Bug reports and feature requests can be provided by creating an `issue <https://github.com/tomasstolker/pycrires/issues>`_ on the Github page.
 
 License
 -------
 
-Copyright 2018-2022 Tomas Stolker
+Copyright 2018-2023 Tomas Stolker
 
 *species* is distributed under the MIT License. See `LICENSE <https://github.com/tomasstolker/pycrires/blob/main/LICENSE>`_ for the terms and conditions.
```

### Comparing `species-0.5.5/README.rst` & `species-0.6.0/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -23,15 +23,17 @@
 
 .. image:: https://img.shields.io/github/license/tomasstolker/species
    :target: https://github.com/tomasstolker/species/blob/main/LICENSE
 
 .. image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/tomasstolker/species/HEAD
 
-*species* is a toolkit for atmospheric characterization of directly imaged exoplanets. It provides a coherent framework for spectral and photometric analysis which builds on publicly-available data and models from various resources. There are tools available for both grid retrievals and free retrievals with Bayesian inference, color-magnitude and color-color diagrams, a variety of model grids, empirical spectral analysis, spectral and photometric calibration, analysis of emission lines, and synthetic photometry. The package has been released on `PyPI <https://pypi.org/project/species/>`_ and is actively developed and maintained on Github.
+*species* is a toolkit for atmospheric characterization of directly imaged exoplanets. It provides a coherent framework for spectral and photometric analysis which builds on publicly-available data and models from various resources.
+
+There are tools available for grid and free retrievals using Bayesian inference, synthetic photometry, interpolating a variety atmospheric and evolutionary model grids (including the possibility to add a custom grid), color-magnitude and color-color diagrams, empirical spectral analysis, spectral and photometric calibration, and analysis of emission lines. The package has been released on `PyPI <https://pypi.org/project/species/>`_ and is actively developed and maintained on Github.
 
 Documentation
 -------------
 
 Documentation can be found at `http://species.readthedocs.io <http://species.readthedocs.io>`_.
 
 Tutorials
@@ -48,10 +50,10 @@
 ------------
 
 Contributions are welcome so please consider `forking <https://help.github.com/en/articles/fork-a-repo>`_ the repository and creating a `pull request <https://github.com/tomasstolker/pycrires/pulls>`_. Bug reports and feature requests can be provided by creating an `issue <https://github.com/tomasstolker/pycrires/issues>`_ on the Github page.
 
 License
 -------
 
-Copyright 2018-2022 Tomas Stolker
+Copyright 2018-2023 Tomas Stolker
 
 *species* is distributed under the MIT License. See `LICENSE <https://github.com/tomasstolker/pycrires/blob/main/LICENSE>`_ for the terms and conditions.
```

### Comparing `species-0.5.5/setup.py` & `species-0.6.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open('requirements.txt') as req_txt:
     parse_req = pkg_resources.parse_requirements(req_txt)
     install_requires = [str(req) for req in parse_req]
 
 setuptools.setup(
     name='species',
-    version='0.5.5',
+    version='0.6.0',
     description='Toolkit for atmospheric characterization of directly imaged exoplanets',
     long_description=open('README.rst').read(),
     long_description_content_type='text/x-rst',
     author='Tomas Stolker',
     author_email='stolker@strw.leidenuniv.nl',
     url='https://github.com/tomasstolker/species',
     project_urls={'Documentation': 'https://species.readthedocs.io'},
```

### Comparing `species-0.5.5/species/__init__.py` & `species-0.6.0/species/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,11 +74,11 @@
     update_objectbox,
     update_spectra,
 )
 
 
 __author__ = "Tomas Stolker"
 __license__ = "MIT"
-__version__ = "0.5.5"
+__version__ = "0.6.0"
 __maintainer__ = "Tomas Stolker"
 __email__ = "stolker@strw.leidenuniv.nl"
 __status__ = "Development"
```

### Comparing `species-0.5.5/species/analysis/compare_spectra.py` & `species-0.6.0/species/analysis/compare_spectra.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,110 +20,104 @@
 from species.data import database
 from species.read import read_filter, read_model, read_object
 from species.util import dust_util, read_util
 
 
 class CompareSpectra:
     """
-    Class for comparing a spectrum of an object with a
-    library of empirical or model spectra.
+    Class for comparing the spectrum of an object with
+    a library of empirical or model spectra.
     """
 
     @typechecked
     def __init__(
         self,
         object_name: str,
         spec_name: Union[str, List[str]],
-        spec_library: Optional[str] = None,
     ) -> None:
         """
         Parameters
         ----------
         object_name : str
             Object name as stored in the database with
             :func:`~species.data.database.Database.add_object` or
             :func:`~species.data.database.Database.add_companion`.
         spec_name : str, list(str)
             Name of the spectrum or list with spectrum names that
             are stored at the object data of ``object_name``. The
             argument can be either a string or a list of strings.
-        spec_library : str, None
-            DEPRECATED: Name of the spectral library
-            ('irtf', 'spex', or 'kesseli+2017).
 
         Returns
         -------
         NoneType
             None
         """
 
         self.object_name = object_name
         self.spec_name = spec_name
 
         if isinstance(self.spec_name, str):
             self.spec_name = [self.spec_name]
 
-        if spec_library is not None:
-            warnings.warn(
-                "The 'spec_library' parameter is no longer used "
-                "by the constructor of CompareSpectra and will "
-                "be removed in a future release.",
-                DeprecationWarning,
-            )
-
         self.object = read_object.ReadObject(object_name)
 
         config_file = os.path.join(os.getcwd(), "species_config.ini")
 
         config = configparser.ConfigParser()
         config.read(config_file)
 
         self.database = config["species"]["database"]
 
     @typechecked
     def spectral_type(
         self,
         tag: str,
-        spec_library,
+        spec_library: str,
         wavel_range: Optional[Tuple[Optional[float], Optional[float]]] = None,
         sptypes: Optional[List[str]] = None,
-        av_ext: Optional[Union[List[float], np.array]] = None,
-        rad_vel: Optional[Union[List[float], np.array]] = None,
+        av_ext: Optional[Union[List[float], np.ndarray]] = None,
+        rad_vel: Optional[Union[List[float], np.ndarray]] = None,
     ) -> None:
         """
         Method for finding the best fitting empirical spectra
         from a selected library by evaluating the goodness-of-fit
-        statistic from Cushing et al. (2008).
+        statistic from `Cushing et al. (2008) <https://ui.adsabs.
+        harvard.edu/abs/2008ApJ...678.1372C/abstract>`_.
 
         Parameters
         ----------
         tag : str
             Database tag where for each spectrum from the spectral
             library the best-fit parameters will be stored. So when
             testing a range of values for ``av_ext`` and ``rad_vel``,
             only the parameters that minimize the goodness-of-fit
             statistic will be stored.
         spec_library : str
-            Name of the spectral library ('irtf', 'spex',
+            Name of the spectral library (e.g. 'irtf', 'spex',
             'kesseli+2017', 'bonnefoy+2014').
         wavel_range : tuple(float, float), None
-            Wavelength range (um) that is used for the empirical
-            comparison.
+            Wavelength range (:math:`\\mu\\mathrm{m}`) that
+            is evaluated.
         sptypes : list(str), None
-            List with spectral types to compare with. The list should
-            only contains types, for example ``sptypes=['M', 'L']``.
-            All available spectral types in the ``spec_library``
-            are compared with if set to ``None``.
-        av_ext : list(float), np.array, None
+            List with spectral types to compare with, for example
+            ``sptypes=['M', 'L']``. All available spectral types
+            in the ``spec_library`` are compared with if the
+            argument is set to ``None``.
+        av_ext : list(float), np.ndarray, None
             List of :math:`A_V` for which the goodness-of-fit
             statistic is tested. The extinction is calculated with
-            the empirical relation from Cardelli et al. (1989).
-        rad_vel : list(float), np.array, None
+            the empirical relation from `Cardelli et al. (1989)
+            <https://ui.adsabs.harvard.edu/abs/1989ApJ...345..245C/
+            abstract>`_. The extinction is not varied if the argument
+            is set to ``None``.
+        rad_vel : list(float), np.ndarray, None
             List of radial velocities (km s-1) for which the
-            goodness-of-fit statistic is tested.
+            goodness-of-fit statistic is tested. The radial
+            velocity is not varied if the argument is set
+            to ``None``.
 
         Returns
         -------
         NoneType
             None
         """
 
@@ -207,17 +201,15 @@
                         raise ValueError(
                             "The selected wavelength range does not "
                             "cover any wavelength points of the input "
                             "spectrum. Please use a broader range as "
                             "argument of 'wavel_range'."
                         )
 
-                    spectrum = spectrum[
-                        indices,
-                    ]
+                    spectrum = spectrum[indices,]
 
                 empty_message = len(print_message) * " "
                 print(f"\r{empty_message}", end="")
 
                 print_message = f"Processing spectra... {item}"
                 print(f"\r{print_message}", end="")
 
@@ -374,59 +366,60 @@
         )
 
     @typechecked
     def compare_model(
         self,
         tag: str,
         model: str,
-        av_points: Optional[Union[List[float], np.array]] = None,
+        av_points: Optional[Union[List[float], np.ndarray]] = None,
         fix_logg: Optional[float] = None,
         scale_spec: Optional[List[str]] = None,
         weights: bool = True,
         inc_phot: Optional[List[str]] = None,
     ) -> None:
         """
         Method for finding the best fitting spectrum from a grid of
         atmospheric model spectra by evaluating the goodness-of-fit
-        statistic from Cushing et al. (2008). Currently, this method
-        only supports model grids with only :math:`T_\\mathrm{eff}`
-        and :math:`\\log(g)` as free parameters (e.g. BT-Settl).
-        Please create an issue on Github if support for models with
-        more than two parameters is required.
+        statistic from `Cushing et al. (2008) <https://ui.adsabs.
+        harvard.edu/abs/2008ApJ...678.1372C/abstract>`_.
 
         Parameters
         ----------
         tag : str
             Database tag where for each spectrum from the spectral
             library the best-fit parameters will be stored. So when
             testing a range of values for ``av_ext`` and ``rad_vel``,
             only the parameters that minimize the goodness-of-fit
             statistic will be stored.
         model : str
             Name of the atmospheric model grid with synthetic spectra.
         av_points : list(float), np.array, None
             List of :math:`A_V` extinction values for which the
             goodness-of-fit statistic will be tested. The extinction is
-            calculated with the relation from Cardelli et al. (1989).
+            calculated with the relation from `Cardelli et al. (1989)
+            <https://ui.adsabs.harvard.edu/abs/1989ApJ...345..245C/
+            abstract>`_.
         fix_logg : float, None
             Fix the value of :math:`\\log(g)`, for example if estimated
             from gravity-sensitive spectral features. Typically,
             :math:`\\log(g)` can not be accurately determined when
             comparing the spectra over a broad wavelength range.
         scale_spec : list(str), None
-            List with names of observed spectra to which a flux scaling
-            is applied to best match the spectral templates.
+            List with names of observed spectra to which an additional
+            flux scaling is applied to best match the spectral
+            templates. This can be used to account for a difference in
+            absolute calibration between spectra.
         weights : bool
             Apply a weighting based on the widths of the
             wavelengths bins.
         inc_phot : list(str), None
             Filter names of the photometry to include in the
-            comparison. Photometry points are weighted by the FWHM of
-            the filter profile. No photometric fluxes will be used if
-            the argument is set to ``None``.
+            comparison. Photometry points are weighted by the FWHM
+            of the filter profile. No photometric fluxes will be
+            used if the argument is set to ``None``.
 
         Returns
         -------
         NoneType
             None
         """
 
@@ -453,24 +446,18 @@
         phot_wavel = {}
 
         for phot_item in inc_phot:
             read_filt = read_filter.ReadFilter(phot_item)
             w_i[phot_item] = read_filt.filter_fwhm()
             phot_wavel[phot_item] = read_filt.mean_wavelength()
 
-        if av_points is None:
-            av_points = np.array([0.0])
-
-        elif isinstance(av_points, list):
-            av_points = np.array(av_points)
-
-        readmodel = read_model.ReadModel(model)
+        model_reader = read_model.ReadModel(model)
 
-        model_param = readmodel.get_parameters()
-        grid_points = readmodel.get_points()
+        model_param = model_reader.get_parameters()
+        grid_points = model_reader.get_points()
 
         coord_points = []
         for key, value in grid_points.items():
             if key == "logg" and fix_logg is not None:
                 if fix_logg in value:
                     coord_points.append(np.array([fix_logg]))
 
@@ -486,143 +473,221 @@
                 coord_points.append(value)
 
         if av_points is not None:
             model_param.append("ism_ext")
             coord_points.append(av_points)
 
         grid_shape = []
-
         for item in coord_points:
             grid_shape.append(len(item))
 
+        for _ in range(len(coord_points), 6):
+            model_param.append(None)
+            coord_points.append([None])
+            grid_shape.append(1)
+
         fit_stat = np.zeros(grid_shape)
         flux_scaling = np.zeros(grid_shape)
 
         if len(scale_spec) == 0:
             extra_scaling = None
 
         else:
             grid_shape.append(len(scale_spec))
             extra_scaling = np.zeros(grid_shape)
 
+        n_iter = 1
+        for item in coord_points:
+            if len(item) > 0:
+                n_iter *= len(item)
+
         count = 1
 
-        if len(coord_points) == 3:
-            n_iter = len(coord_points[0]) * len(coord_points[1]) * len(coord_points[2])
+        for coord_0_idx, coord_0_item in enumerate(coord_points[0]):
+            for coord_1_idx, coord_1_item in enumerate(coord_points[1]):
+                for coord_2_idx, coord_2_item in enumerate(coord_points[2]):
+                    for coord_3_idx, coord_3_item in enumerate(coord_points[3]):
+                        for coord_4_idx, coord_4_item in enumerate(coord_points[4]):
+                            for coord_5_idx, coord_5_item in enumerate(coord_points[5]):
+                                print(
+                                    f"\rProcessing model spectrum {count}/{n_iter}...",
+                                    end="",
+                                )
 
-            for i, item_i in enumerate(coord_points[0]):
-                for j, item_j in enumerate(coord_points[1]):
-                    for k, item_k in enumerate(coord_points[2]):
-                        print(
-                            f"\rProcessing model spectrum {count}/{n_iter}...", end=""
-                        )
+                                model_spec = {}
+                                model_phot = {}
 
-                        model_spec = {}
-                        model_phot = {}
+                                param_dict = {}
 
-                        for spec_item in self.spec_name:
-                            obj_spec = self.object.get_spectrum()[spec_item][0]
-                            obj_res = self.object.get_spectrum()[spec_item][3]
-
-                            param_dict = {
-                                model_param[0]: item_i,
-                                model_param[1]: item_j,
-                                model_param[2]: item_k,
-                            }
-
-                            wavel_range = (0.9 * obj_spec[0, 0], 1.1 * obj_spec[-1, 0])
-                            readmodel = read_model.ReadModel(
-                                model, wavel_range=wavel_range
-                            )
+                                if model_param[0] is not None:
+                                    param_dict[model_param[0]] = coord_0_item
 
-                            model_box = readmodel.get_data(
-                                param_dict,
-                                spec_res=obj_res,
-                                wavel_resample=obj_spec[:, 0],
-                            )
+                                if model_param[1] is not None:
+                                    param_dict[model_param[1]] = coord_1_item
 
-                            model_spec[spec_item] = model_box.flux
+                                if model_param[2] is not None:
+                                    param_dict[model_param[2]] = coord_2_item
 
-                        for phot_item in inc_phot:
-                            readmodel = read_model.ReadModel(
-                                model, filter_name=phot_item
-                            )
+                                if model_param[3] is not None:
+                                    param_dict[model_param[3]] = coord_3_item
 
-                            model_phot[phot_item] = readmodel.get_flux(param_dict)[0]
+                                if model_param[4] is not None:
+                                    param_dict[model_param[4]] = coord_4_item
 
-                        def g_fit(x, scaling):
-                            g_stat = 0.0
+                                if model_param[5] is not None:
+                                    param_dict[model_param[5]] = coord_5_item
 
-                            for spec_item in self.spec_name:
-                                obs_spec = self.object.get_spectrum()[spec_item][0]
+                                for spec_item in self.spec_name:
+                                    obj_spec = self.object.get_spectrum()[spec_item][0]
+                                    obj_res = self.object.get_spectrum()[spec_item][3]
 
-                                if spec_item in scale_spec:
-                                    spec_idx = scale_spec.index(spec_item)
-
-                                    c_numer = (
-                                        w_i[spec_item]
-                                        * obs_spec[:, 1]
-                                        * model_spec[spec_item]
-                                        / obs_spec[:, 2] ** 2
+                                    wavel_range = (
+                                        0.9 * obj_spec[0, 0],
+                                        1.1 * obj_spec[-1, 0],
                                     )
 
-                                    c_denom = (
-                                        w_i[spec_item]
-                                        * model_spec[spec_item] ** 2
-                                        / obs_spec[:, 2] ** 2
+                                    model_reader = read_model.ReadModel(
+                                        model, wavel_range=wavel_range
                                     )
 
-                                    extra_scaling[i, j, k, spec_idx] = np.sum(
-                                        c_numer
-                                    ) / np.sum(c_denom)
-
-                                    g_stat += np.sum(
-                                        w_i[spec_item]
-                                        * (
-                                            obs_spec[:, 1]
-                                            - extra_scaling[i, j, k, spec_idx]
-                                            * model_spec[spec_item]
-                                        )
-                                        ** 2
-                                        / obs_spec[:, 2] ** 2
+                                    model_box = model_reader.get_data(
+                                        param_dict,
+                                        spec_res=obj_res,
+                                        wavel_resample=obj_spec[:, 0],
                                     )
 
-                                else:
-                                    g_stat += np.sum(
-                                        w_i[spec_item]
-                                        * (
-                                            obs_spec[:, 1]
-                                            - scaling * model_spec[spec_item]
-                                        )
-                                        ** 2
-                                        / obs_spec[:, 2] ** 2
-                                    )
+                                    model_spec[spec_item] = model_box.flux
 
-                            for phot_item in inc_phot:
-                                obs_phot = self.object.get_photometry(phot_item)
+                                for phot_item in inc_phot:
+                                    model_reader = read_model.ReadModel(
+                                        model, filter_name=phot_item
+                                    )
 
-                                g_stat += (
-                                    w_i[phot_item]
-                                    * (obs_phot[2] - scaling * model_phot[phot_item])
-                                    ** 2
-                                    / obs_phot[3] ** 2
-                                )
+                                    model_phot[phot_item] = model_reader.get_flux(
+                                        param_dict
+                                    )[0]
+
+                                def g_fit(x, scaling):
+                                    g_stat = 0.0
+
+                                    for spec_item in self.spec_name:
+                                        obs_spec = self.object.get_spectrum()[
+                                            spec_item
+                                        ][0]
+
+                                        if spec_item in scale_spec:
+                                            spec_idx = scale_spec.index(spec_item)
+
+                                            c_numer = (
+                                                w_i[spec_item]
+                                                * obs_spec[:, 1]
+                                                * model_spec[spec_item]
+                                                / obs_spec[:, 2] ** 2
+                                            )
+
+                                            c_denom = (
+                                                w_i[spec_item]
+                                                * model_spec[spec_item] ** 2
+                                                / obs_spec[:, 2] ** 2
+                                            )
+
+                                            extra_scaling[
+                                                coord_0_idx,
+                                                coord_1_idx,
+                                                coord_2_idx,
+                                                coord_3_idx,
+                                                coord_4_idx,
+                                                coord_5_idx,
+                                                spec_idx,
+                                            ] = np.sum(c_numer) / np.sum(c_denom)
+
+                                            g_stat += np.sum(
+                                                w_i[spec_item]
+                                                * (
+                                                    obs_spec[:, 1]
+                                                    - extra_scaling[
+                                                        coord_0_idx,
+                                                        coord_1_idx,
+                                                        coord_2_idx,
+                                                        coord_3_idx,
+                                                        coord_4_idx,
+                                                        coord_5_idx,
+                                                        spec_idx,
+                                                    ]
+                                                    * model_spec[spec_item]
+                                                )
+                                                ** 2
+                                                / obs_spec[:, 2] ** 2
+                                            )
+
+                                        else:
+                                            g_stat += np.sum(
+                                                w_i[spec_item]
+                                                * (
+                                                    obs_spec[:, 1]
+                                                    - scaling * model_spec[spec_item]
+                                                )
+                                                ** 2
+                                                / obs_spec[:, 2] ** 2
+                                            )
+
+                                    for phot_item in inc_phot:
+                                        obs_phot = self.object.get_photometry(phot_item)
+
+                                        g_stat += (
+                                            w_i[phot_item]
+                                            * (
+                                                obs_phot[2]
+                                                - scaling * model_phot[phot_item]
+                                            )
+                                            ** 2
+                                            / obs_phot[3] ** 2
+                                        )
 
-                            return g_stat
+                                    return g_stat
 
-                        popt, _ = curve_fit(g_fit, xdata=[0.0], ydata=[0.0])
-                        scaling = popt[0]
+                                popt, _ = curve_fit(g_fit, xdata=[0.0], ydata=[0.0])
+                                scaling = popt[0]
 
-                        flux_scaling[i, j, k] = scaling
-                        fit_stat[i, j, k] = g_fit(0.0, scaling)
+                                flux_scaling[
+                                    coord_0_idx,
+                                    coord_1_idx,
+                                    coord_2_idx,
+                                    coord_3_idx,
+                                    coord_4_idx,
+                                    coord_5_idx,
+                                ] = scaling
+                                fit_stat[
+                                    coord_0_idx,
+                                    coord_1_idx,
+                                    coord_2_idx,
+                                    coord_3_idx,
+                                    coord_4_idx,
+                                    coord_5_idx,
+                                ] = g_fit(0.0, scaling)
 
-                        count += 1
+                                count += 1
 
         print(" [DONE]")
 
+        for param_idx, param_item in enumerate(model_param):
+            if param_item is None:
+                model_param = model_param[:param_idx]
+                coord_points = coord_points[:param_idx]
+                grid_shape = grid_shape[:param_idx]
+                break
+
+        for dim_idx in range(fit_stat.ndim, 0, -1):
+            if dim_idx > len(model_param):
+                fit_stat = fit_stat[..., 0]
+                flux_scaling = flux_scaling[..., 0]
+
+                if extra_scaling is not None:
+                    extra_scaling = extra_scaling[..., 0, :]
+
         species_db = database.Database()
 
         species_db.add_comparison(
             tag=tag,
             goodness_of_fit=fit_stat,
             flux_scaling=flux_scaling,
             model_param=model_param,
```

### Comparing `species-0.5.5/species/analysis/emission_line.py` & `species-0.6.0/species/analysis/emission_line.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,21 +264,19 @@
         # Create plot
 
         if plot_filename is None:
             print("Plotting continuum fit...", end="", flush=True)
         else:
             print(f"Plotting continuum fit: {plot_filename}...", end="", flush=True)
 
-        mpl.rcParams["font.serif"] = ["Bitstream Vera Serif"]
-        mpl.rcParams["font.family"] = "serif"
-
-        plt.rc("axes", edgecolor="black", linewidth=2)
+        plt.rcParams["font.family"] = "serif"
+        plt.rcParams["mathtext.fontset"] = "dejavuserif"
         plt.rcParams["axes.axisbelow"] = False
 
-        plt.figure(1, figsize=(6, 6))
+        plt.figure(figsize=(6, 6))
         gs = mpl.gridspec.GridSpec(2, 1)
         gs.update(wspace=0, hspace=0.1, left=0, right=1, bottom=0, top=1)
 
         ax1 = plt.subplot(gs[0, 0])
         ax2 = plt.subplot(gs[1, 0])
         ax3 = ax1.twiny()
         ax4 = ax2.twiny()
@@ -517,21 +515,19 @@
 
         n_samples = 1000
 
         wavel_high_res = read_util.create_wavelengths(wavel_int, 1e5)
 
         # Creating plot
 
-        mpl.rcParams["font.serif"] = ["Bitstream Vera Serif"]
-        mpl.rcParams["font.family"] = "serif"
-
-        plt.rc("axes", edgecolor="black", linewidth=2)
+        plt.rcParams["font.family"] = "serif"
+        plt.rcParams["mathtext.fontset"] = "dejavuserif"
         plt.rcParams["axes.axisbelow"] = False
 
-        plt.figure(1, figsize=(6, 3))
+        plt.figure(figsize=(6, 3))
         gs = mpl.gridspec.GridSpec(1, 1)
         gs.update(wspace=0, hspace=0, left=0, right=1, bottom=0, top=1)
 
         ax1 = plt.subplot(gs[0, 0])
         ax2 = ax1.twiny()
 
         ax1.tick_params(
@@ -625,29 +621,29 @@
                 self.spectrum[:, 0], spec_rand, kind=interp_kind, bounds_error=False
             )
 
             # Resample to high-resolution wavelengths
             flux_rand = spec_interp(wavel_high_res)
 
             # Integrate line flux (W m-2)
-            flux_sample[i] = np.trapz(flux_rand, wavel_high_res)
+            flux_sample[i] = np.trapz(flux_rand, x=wavel_high_res)
 
             # Line luminosity (Lsun)
             lum_sample[i] = (
                 4.0
                 * np.pi
                 * (1e3 * constants.PARSEC / self.parallax) ** 2
                 * flux_sample[i]
             )
             lum_sample[i] /= constants.L_SUN  # (Lsun)
 
             # Weighted (with flux) mean wavelength (um)
             mean_sample[i] = np.trapz(
-                wavel_high_res * flux_rand, wavel_high_res
-            ) / np.trapz(flux_rand, wavel_high_res)
+                wavel_high_res * flux_rand, x=wavel_high_res
+            ) / np.trapz(flux_rand, x=wavel_high_res)
 
             # Radial velocity (km s-1)
             vrad_sample[i] = (
                 1e-3
                 * constants.LIGHT
                 * (mean_sample[i] - self.lambda_rest)
                 / self.lambda_rest
@@ -692,15 +688,15 @@
             self.spectrum[:, 1],
             kind=interp_kind,
             bounds_error=False,
         )
 
         flux_high_res = spec_interp(wavel_high_res)
 
-        line_flux = np.trapz(flux_high_res, wavel_high_res)
+        line_flux = np.trapz(flux_high_res, x=wavel_high_res)
 
         ax1.plot(
             wavel_high_res, flux_high_res, color="tab:blue", label="High resolution"
         )
 
         ax1.legend(loc="upper right", frameon=False, fontsize=12.0)
 
@@ -741,15 +737,15 @@
 
             log_acc_mean = np.mean(log_acc_sample)
             log_acc_std = np.std(log_acc_sample)
 
             print(
                 "Inflating the uncertainty on the "
                 "accretion luminosity by 0.3 dex\n to "
-                "account for the the model uncertainty "
+                "account for the model uncertainty "
                 "(see Aoyama et al. 2021)..."
             )
 
             log_acc_std = np.sqrt(log_acc_std**2 + 0.3**2)
 
             print(
                 "Accretion luminosity log10(L/Lsun) = "
@@ -1072,15 +1068,15 @@
             model_box = read_util.gaussian_spectrum(
                 self.wavel_range,
                 model_param,
                 spec_res=high_spec_res,
                 double_gaussian=double_gaussian,
             )
 
-            line_flux[i] = np.trapz(model_box.flux, model_box.wavelength)  # (W m-2)
+            line_flux[i] = np.trapz(model_box.flux, x=model_box.wavelength)  # (W m-2)
 
             line_lum[i] = (
                 4.0
                 * np.pi
                 * (1e3 * constants.PARSEC / self.parallax) ** 2
                 * line_flux[i]
             )  # (W)
@@ -1090,15 +1086,15 @@
                 # Normalize the spectrum to the continuum
                 spec_norm = (model_box.flux + cont_high_res) / cont_high_res
 
                 # Check if the flux is NaN (due to interpolation errors at the spectrum edge)
                 indices = ~np.isnan(spec_norm)
 
                 eq_width[i] = np.trapz(
-                    1.0 - spec_norm[indices], model_box.wavelength[indices]
+                    1.0 - spec_norm[indices], x=model_box.wavelength[indices]
                 )  # (um)
                 eq_width[i] *= 1e4  # (A)
 
         print(" [DONE]")
 
         line_flux = line_flux[..., np.newaxis]
         samples = np.append(samples, line_flux, axis=1)
@@ -1108,15 +1104,15 @@
 
         if self.hydrogen_line is not None:
             log_acc_lum = np.log10(self.accretion_luminosity(line_lum[:, 0]))
 
             print(
                 "Inflating the uncertainty on the "
                 "accretion luminosity by 0.3 dex\n to "
-                "account for the the model uncertainty "
+                "account for the model uncertainty "
                 "(see Aoyama et al. 2021)..."
             )
 
             log_acc_lum += np.random.normal(0.0, 0.3, size=log_acc_lum.size)
             log_acc_lum = log_acc_lum[..., np.newaxis]
             samples = np.append(samples, log_acc_lum, axis=1)
 
@@ -1197,21 +1193,19 @@
         else:
             print(
                 f"Plotting best-fit line profile: {plot_filename}...",
                 end="",
                 flush=True,
             )
 
-        mpl.rcParams["font.serif"] = ["Bitstream Vera Serif"]
-        mpl.rcParams["font.family"] = "serif"
-
-        plt.rc("axes", edgecolor="black", linewidth=2)
+        plt.rcParams["font.family"] = "serif"
+        plt.rcParams["mathtext.fontset"] = "dejavuserif"
         plt.rcParams["axes.axisbelow"] = False
 
-        plt.figure(1, figsize=(6, 6))
+        plt.figure(figsize=(6, 6))
         gs = mpl.gridspec.GridSpec(2, 1)
         gs.update(wspace=0, hspace=0.1, left=0, right=1, bottom=0, top=1)
 
         ax1 = plt.subplot(gs[0, 0])
         ax2 = plt.subplot(gs[1, 0])
         ax3 = ax1.twiny()
         ax4 = ax2.twiny()
```

### Comparing `species-0.5.5/species/analysis/fit_model.py` & `species-0.6.0/species/analysis/fit_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 import warnings
 
 from typing import Optional, Union, List, Tuple, Dict
 
 import numpy as np
 import spectres
 
-from scipy import stats
+from PyAstronomy.pyasl import fastRotBroad
+from scipy import interpolate, stats
 
 try:
     import ultranest
 except:
     warnings.warn(
         "UltraNest could not be imported. Perhaps "
         "because cython was not correctly compiled?"
@@ -62,23 +63,30 @@
         object_name: str,
         model: str,
         bounds: Optional[
             Dict[
                 str,
                 Union[
                     Tuple[float, float],
+                    Tuple[Optional[Tuple[float, float]]],
                     Tuple[Optional[Tuple[float, float]], Optional[Tuple[float, float]]],
+                    Tuple[
+                        Optional[Tuple[float, float]],
+                        Optional[Tuple[float, float]],
+                        Optional[Tuple[float, float]],
+                    ],
                     List[Tuple[float, float]],
                 ],
             ]
         ] = None,
         inc_phot: Union[bool, List[str]] = True,
         inc_spec: Union[bool, List[str]] = True,
         fit_corr: Optional[List[str]] = None,
         weights: Optional[Dict[str, float]] = None,
+        ext_filter: Optional[str] = None,
     ) -> None:
         """
         Parameters
         ----------
         object_name : str
             Object name of the companion as stored in the database with
             :func:`~species.data.database.Database.add_object` or
@@ -92,15 +100,15 @@
             providing the same value as lower and upper boundary
             of the parameter (e.g. ``bounds={'logg': (4., 4.)``.
             An explanation of the various parameters can be found
             below.
 
             Atmospheric model parameters (e.g. with
             ``model='bt-settl-cifist'``; see docstring of
-            :meth:`~species.data.database.Database.add_model`
+            :func:`~species.data.database.Database.add_model`
             for the available model grids):
 
                - Boundaries are provided as tuple of two floats. For example,
                  ``bounds={'teff': (1000, 1500.), 'logg': (3.5, 5.)}``.
 
                - The grid boundaries (i.e. the maximum range) are
                  adopted as priors if a parameter range is set to
@@ -108,14 +116,34 @@
                  in the dictionary of ``bounds``. For example,
                  ``bounds={'teff': (1000., 1500.), 'logg': None}``.
                  The default range for the radius is
                  :math:`0.5-5.0~R_\\mathrm{J}`. With ``bounds=None``,
                  automatic priors will be set for all mandatory
                  parameters.
 
+               - Rotational broadening can be fitted by including the
+                 ``vsini`` parameter (km/s). This parameter will only
+                 be relevant if the rotational broadening is stronger
+                 than or comparable to the instrumental broadening,
+                 so typically when the data has a high spectral
+                 resolution. The resolution is set when adding a
+                 spectrum to the database with
+                 :func:`~species.data.database.Database.add_object`.
+                 Note that the broadening is applied with the
+                 `fastRotBroad <https://pyastronomy.readthedocs.io/
+                 en/latest/pyaslDoc/aslDoc/rotBroad.html#PyAstronomy.
+                 pyasl.fastRotBroad>`_ function from ``PyAstronomy``.
+                 The rotational broadening is only accurate if the
+                 wavelength range of the data is somewhat narrow.
+                 For example, when fitting a medium- or
+                 high-resolution spectrum across multiple bands
+                 (e.g. $JHK$ bands) then it is best to split up the
+                 data into the separate bands when adding them with
+                 :func:`~species.data.database.Database.add_object`.
+
                - It is possible to fit a weighted combination of two
                  atmospheric parameters from the same model. This
                  can be useful to fit data of a spectroscopic binary
                  or to account for atmospheric asymmetries of a single
                  object. For each atmospheric parameter, a tuple of
                  two tuples can be provided, for example
                  ``bounds={'teff': ((1000., 1500.), (1300., 1800.))}``.
@@ -175,34 +203,39 @@
                - The :func:`~species.plot.plot_mcmc.plot_mag_posterior`
                  function can be used for calculating synthetic
                  photometry and error bars from the posterior
                  distributions.
 
             Calibration parameters:
 
-                 - For each spectrum/instrument, two optional
+                 - For each spectrum/instrument, three optional
                    parameters can be fitted to account for biases in
-                   the calibration: a scaling of the flux and a
-                   relative inflation of the uncertainties.
+                   the calibration: a scaling of the flux, a
+                   relative inflation of the uncertainties, and a
+                   radial velocity (RV) shift. The last parameter can
+                   account for an actual RV shift by the source or
+                   an inaccuracy in the wavelength solution.
 
                  - For example, ``bounds={'SPHERE': ((0.8, 1.2),
-                   (0., 1.))}`` if the scaling is
-                   fitted between 0.8 and 1.2, and the error is
+                   (0., 1.), (-50., 50.))}`` if the scaling is
+                   fitted between 0.8 and 1.2, the error is
                    inflated (relative to the sampled model fluxes)
-                   with a value between 0 and 1.
+                   with a value between 0 and 1, and the RV is
+                   fitted between -50 and 50 km/s.
 
                  - The dictionary key should be the same as the
                    database tag of the spectrum. For example,
-                   ``{'SPHERE': ((0.8, 1.2), (0., 1.))}`` if the
-                   spectrum is stored as ``'SPHERE'`` with
+                   ``{'SPHERE': ((0.8, 1.2), (0., 1.), (-50., 50.))}``
+                   if the spectrum is stored as ``'SPHERE'`` with
                    :func:`~species.data.database.Database.add_object`.
 
-                 - Each of the two calibration parameters can be set to
+                 - Each of the three calibration parameters can be set to
                    ``None`` in which case the parameter is not used. For
-                   example, ``bounds={'SPHERE': ((0.8, 1.2), None)}``.
+                   example,
+                   ``bounds={'SPHERE': ((0.8, 1.2), None, None)}``.
 
                  - The errors of the photometric fluxes can be inflated
                    to account for underestimated error bars. The error
                    inflation is relative to the actual flux and is
                    either fitted separately for a filter, or a single
                    error inflation is applied to all filters from an
                    instrument. For the first case, the keyword in the
@@ -334,14 +367,23 @@
         weights : dict(str, float), None
             Weights to be applied to the log-likelihood components of
             the different spectroscopic and photometric data that are
             provided with ``inc_spec`` and ``inc_phot``. This parameter
             can for example be used to bias the weighting of the
             photometric data points. An equal weighting is applied if
             the argument is set to ``None``.
+        ext_filter : str, None
+            Filter that is associated with the (optional) extinction
+            parameter, ``ism_ext``. When the argument of ``ext_filter``
+            is set to ``None``, the extinction is defined in the visual
+            (i.e. :math:`A_V`). By providing a filter name from the
+            `SVO Filter Profile Service <http://svo2.cab.inta-csic.es/
+            svo/theory/fps/>`_ as argument then the extinction
+            ``ism_ext`` is fitted in that filter instead of the
+            $V$ band.
 
         Returns
         -------
         NoneType
             None
         """
 
@@ -352,14 +394,15 @@
             raise ValueError(
                 "The 'bounds' dictionary should contain 'teff' and 'radius'."
             )
 
         self.object = read_object.ReadObject(object_name)
         self.parallax = self.object.get_parallax()
         self.binary = False
+        self.ext_filter = ext_filter
 
         if fit_corr is None:
             self.fit_corr = []
         else:
             self.fit_corr = fit_corr
 
         self.model = model
@@ -407,15 +450,14 @@
         else:
             # Fitting self-consistent atmospheric models
             if self.bounds is not None:
                 readmodel = read_model.ReadModel(self.model)
                 bounds_grid = readmodel.get_bounds()
 
                 for key, value in bounds_grid.items():
-
                     if key not in self.bounds:
                         # Set the parameter boundaries to the grid
                         # boundaries if set to None or not found
                         self.bounds[key] = bounds_grid[key]
 
                     elif isinstance(self.bounds[key][0], tuple):
                         self.binary = True
@@ -504,14 +546,21 @@
                 readmodel = read_model.ReadModel(self.model, None, None)
                 self.bounds = readmodel.get_bounds()
 
             self.modelpar = readmodel.get_parameters()
             self.modelpar.append("radius")
             self.modelpar.append("parallax")
 
+            # Optional rotational broading
+
+            if "vsini" in bounds:
+                # Add vsin(i) parameter (km s-1)
+                self.modelpar.append("vsini")
+                self.bounds["vsini"] = (bounds["vsini"][0], bounds["vsini"][1])
+
             if self.binary:
                 if "radius" in self.bounds:
                     if isinstance(self.bounds["radius"][0], tuple):
                         self.bounds["radius_0"] = self.bounds["radius"][0]
                         self.bounds["radius_1"] = self.bounds["radius"][1]
                         del self.bounds["radius"]
 
@@ -674,15 +723,14 @@
                             self.bounds[f"corr_amp_{item}"] = (0.0, 1.0)
 
                         self.n_corr_par += 2
 
             self.modelspec = []
 
             if self.model != "planck":
-
                 for key, value in self.spectrum.items():
                     print(f"\rInterpolating {key}...", end="", flush=True)
 
                     wavel_range = (0.9 * value[0][0, 0], 1.1 * value[0][-1, 0])
 
                     readmodel = read_model.ReadModel(
                         self.model, wavel_range=wavel_range
@@ -754,24 +802,23 @@
 
                 self.diskspec.append(readmodel)
 
                 print(" [DONE]")
 
         for item in self.spectrum:
             if bounds is not None and item in bounds:
-
                 if bounds[item][0] is not None:
                     # Add the flux scaling parameter
                     self.modelpar.append(f"scaling_{item}")
                     self.bounds[f"scaling_{item}"] = (
                         bounds[item][0][0],
                         bounds[item][0][1],
                     )
 
-                if bounds[item][1] is not None:
+                if len(bounds[item]) > 1 and bounds[item][1] is not None:
                     # Add the error inflation parameters
                     self.modelpar.append(f"error_{item}")
                     self.bounds[f"error_{item}"] = (
                         bounds[item][1][0],
                         bounds[item][1][1],
                     )
 
@@ -799,23 +846,30 @@
                     if self.bounds[f"error_{item}"][1] > 1.0:
                         warnings.warn(
                             f"The upper bound of 'error_{item}' is larger than 1. The "
                             f"error inflation should be given relative to the model "
                             f"fluxes so the boundaries are typically between 0 and 1."
                         )
 
+                if len(bounds[item]) > 2 and bounds[item][2] is not None:
+                    # Add radial velocity parameter (km s-1)
+                    self.modelpar.append(f"radvel_{item}")
+                    self.bounds[f"radvel_{item}"] = (
+                        bounds[item][2][0],
+                        bounds[item][2][1],
+                    )
+
                 if item in self.bounds:
                     del self.bounds[item]
 
         if (
             "lognorm_radius" in self.bounds
             and "lognorm_sigma" in self.bounds
             and "lognorm_ext" in self.bounds
         ):
-
             self.cross_sections, _, _ = dust_util.interp_lognorm(
                 inc_phot, inc_spec, self.spectrum
             )
 
             self.modelpar.append("lognorm_radius")
             self.modelpar.append("lognorm_sigma")
             self.modelpar.append("lognorm_ext")
@@ -826,15 +880,14 @@
             )
 
         elif (
             "powerlaw_max" in self.bounds
             and "powerlaw_exp" in self.bounds
             and "powerlaw_ext" in self.bounds
         ):
-
             self.cross_sections, _, _ = dust_util.interp_powerlaw(
                 inc_phot, inc_spec, self.spectrum
             )
 
             self.modelpar.append("powerlaw_max")
             self.modelpar.append("powerlaw_exp")
             self.modelpar.append("powerlaw_ext")
@@ -844,15 +897,21 @@
                 np.log10(self.bounds["powerlaw_max"][1]),
             )
 
         else:
             self.cross_sections = None
 
         if "ism_ext" in self.bounds:
-            self.modelpar.append("ism_ext")
+            if self.ext_filter is not None:
+                self.modelpar.append(f"phot_ext_{self.ext_filter}")
+                self.bounds[f"phot_ext_{self.ext_filter}"] = self.bounds["ism_ext"]
+                del self.bounds["ism_ext"]
+
+            else:
+                self.modelpar.append("ism_ext")
 
         if "ism_red" in self.bounds:
             self.modelpar.append("ism_red")
 
         if "veil_a" in self.bounds:
             self.modelpar.append("veil_a")
 
@@ -915,15 +974,15 @@
                 self.weights[item] = 1.0
 
             print(f"   - {item} = {self.weights[item]:.2e}")
 
     @typechecked
     def lnlike_func(
         self, params, prior: Optional[Dict[str, Tuple[float, float]]]
-    ) -> np.float64:
+    ) -> Union[np.float64, float]:
         """
         Function for calculating the log-likelihood for the sampled
         parameter cube.
 
         Parameters
         ----------
         params : np.ndarray, pymultinest.run.LP_c_double
@@ -950,24 +1009,28 @@
         err_scaling = {}
         corr_len = {}
         corr_amp = {}
         dust_param = {}
         disk_param = {}
         veil_param = {}
         param_dict = {}
+        rad_vel = {}
 
         for item in self.bounds:
             # Add the parameters from the params to their dictionaries
 
             if item[:8] == "scaling_" and item[8:] in self.spectrum:
                 spec_scaling[item[8:]] = params[self.cube_index[item]]
 
             elif item[:6] == "error_" and item[6:] in self.spectrum:
                 err_scaling[item[6:]] = params[self.cube_index[item]]
 
+            elif item[:7] == "radvel_":
+                rad_vel[item[7:]] = params[self.cube_index[item]]
+
             elif item[:9] == "corr_len_" and item[9:] in self.spectrum:
                 corr_len[item[9:]] = 10.0 ** params[self.cube_index[item]]  # (um)
 
             elif item[:9] == "corr_amp_" and item[9:] in self.spectrum:
                 corr_amp[item[9:]] = params[self.cube_index[item]]
 
             elif item[-6:] == "_error" and item[:-6] in self.filter_name:
@@ -981,14 +1044,17 @@
 
             elif item[:9] == "powerlaw_":
                 dust_param[item] = params[self.cube_index[item]]
 
             elif item[:4] == "ism_":
                 dust_param[item] = params[self.cube_index[item]]
 
+            elif self.ext_filter is not None and item == f"phot_ext_{self.ext_filter}":
+                dust_param[item] = params[self.cube_index[item]]
+
             elif item == "disk_teff":
                 disk_param["teff"] = params[self.cube_index[item]]
 
             elif item == "disk_radius":
                 disk_param["radius"] = params[self.cube_index[item]]
 
             elif item == "veil_a":
@@ -1017,14 +1083,17 @@
 
             if item[:8] == "scaling_" and item[8:] in self.spectrum:
                 spec_scaling[item[8:]] = self.fix_param[item]
 
             elif item[:6] == "error_" and item[6:] in self.spectrum:
                 err_scaling[item[6:]] = self.fix_param[item]
 
+            elif item[:7] == "radvel_" and item[7:] in self.spectrum:
+                rad_vel[item[7:]] = self.fix_param[item]
+
             elif item[:9] == "corr_len_" and item[9:] in self.spectrum:
                 corr_len[item[9:]] = self.fix_param[item]  # (um)
 
             elif item[:9] == "corr_amp_" and item[9:] in self.spectrum:
                 corr_amp[item[9:]] = self.fix_param[item]
 
             elif item[:8] == "lognorm_":
@@ -1032,14 +1101,17 @@
 
             elif item[:9] == "powerlaw_":
                 dust_param[item] = self.fix_param[item]
 
             elif item[:4] == "ism_":
                 dust_param[item] = self.fix_param[item]
 
+            elif item[:9] == "phot_ext_":
+                dust_param[item] = self.fix_param[item]
+
             elif item == "disk_teff":
                 disk_param["teff"] = self.fix_param[item]
 
             elif item == "disk_radius":
                 disk_param["radius"] = self.fix_param[item]
 
             elif item == "spec_weight":
@@ -1123,17 +1195,19 @@
                         params[self.cube_index["logg"]],
                         params[self.cube_index["radius"]],
                     )
 
                     ln_like += -0.5 * (mass - value[0]) ** 2 / value[1] ** 2
 
                 else:
-                    warnings.warn(f"The log(g) parameter is not used "
-                                  f"by the {self.model} model so the "
-                                  f"mass prior can not be applied.")
+                    warnings.warn(
+                        f"The log(g) parameter is not used "
+                        f"by the {self.model} model so the "
+                        f"mass prior can not be applied."
+                    )
 
             else:
                 ln_like += (
                     -0.5
                     * (params[self.cube_index[key]] - value[0]) ** 2
                     / value[1] ** 2
                 )
@@ -1247,24 +1321,36 @@
                     dust_param["powerlaw_exp"], 10.0 ** dust_param["powerlaw_max"]
                 )[0]
 
                 phot_flux *= np.exp(-cross_tmp * n_grains)
 
             elif "ism_ext" in dust_param:
                 read_filt = read_filter.ReadFilter(phot_filter)
-                filt_wavel = np.array([read_filt.mean_wavelength()])
+                phot_wavel = np.array([read_filt.mean_wavelength()])
 
                 ism_reddening = dust_param.get("ism_red", 3.1)
 
                 ext_filt = dust_util.ism_extinction(
-                    dust_param["ism_ext"], ism_reddening, filt_wavel
+                    dust_param["ism_ext"], ism_reddening, phot_wavel
                 )
 
                 phot_flux *= 10.0 ** (-0.4 * ext_filt[0])
 
+            elif self.ext_filter is not None:
+                readmodel = read_model.ReadModel(self.model, filter_name=phot_filter)
+
+                param_dict[f"phot_ext_{self.ext_filter}"] = dust_param[f"phot_ext_{self.ext_filter}"]
+                param_dict["ism_red"] = dust_param.get("ism_red", 3.1)
+
+                phot_flux = readmodel.get_flux(param_dict)[0]
+                phot_flux *= flux_scaling
+
+                del param_dict[f"phot_ext_{self.ext_filter}"]
+                del param_dict["ism_red"]
+
             if obj_item.ndim == 1:
                 phot_var = obj_item[1] ** 2
 
                 # Get the telescope/instrument name
                 instr_check = phot_filter.split(".")[0]
 
                 if phot_filter in phot_scaling:
@@ -1387,14 +1473,52 @@
                     )
 
                     model_flux = veil_param["veil_a"] * model_flux + veil_flux
 
             # Scale the spectrum data
             data_flux = spec_scaling[item] * self.spectrum[item][0][:, 1]
 
+            # Apply radial velocity shift
+
+            if item in rad_vel:
+                wavel_shift = (
+                    rad_vel[item] * 1e3 * self.spectrum[item][0][:, 0] / constants.LIGHT
+                )
+                spec_interp = interpolate.interp1d(
+                    self.spectrum[item][0][:, 0] + wavel_shift,
+                    model_flux,
+                    fill_value="extrapolate",
+                )
+                model_flux = spec_interp(self.spectrum[item][0][:, 0])
+
+            # Apply rotational broadening
+
+            if "vsini" in self.modelpar:
+                spec_interp = interpolate.interp1d(
+                    self.spectrum[item][0][:, 0], model_flux
+                )
+
+                wavel_new = np.linspace(
+                    self.spectrum[item][0][0, 0],
+                    self.spectrum[item][0][-1, 0],
+                    2 * self.spectrum[item][0].shape[0],
+                )
+
+                flux_broad = fastRotBroad(
+                    wvl=wavel_new,
+                    flux=spec_interp(wavel_new),
+                    epsilon=0.0,
+                    vsini=params[self.cube_index["vsini"]],
+                    effWvl=None,
+                )
+
+                spec_interp = interpolate.interp1d(wavel_new, flux_broad)
+
+                model_flux = spec_interp(self.spectrum[item][0][:, 0])
+
             if err_scaling[item] is None:
                 # Variance without error inflation
                 data_var = self.spectrum[item][0][:, 2] ** 2
 
             else:
                 # Variance with error inflation (see Piette & Madhusudhan 2020)
                 data_var = (
@@ -1445,19 +1569,34 @@
                     )[0]
 
                     model_flux[j] *= np.exp(-cross_tmp * n_grains)
 
             elif "ism_ext" in dust_param:
                 ism_reddening = dust_param.get("ism_red", 3.1)
 
-                ext_filt = dust_util.ism_extinction(
+                ext_spec = dust_util.ism_extinction(
                     dust_param["ism_ext"], ism_reddening, self.spectrum[item][0][:, 0]
                 )
 
-                model_flux *= 10.0 ** (-0.4 * ext_filt)
+                model_flux *= 10.0 ** (-0.4 * ext_spec)
+
+            elif self.ext_filter is not None:
+                ism_reddening = dust_param.get("ism_red", 3.1)
+
+                av_required = dust_util.convert_to_av(
+                    filter_name=self.ext_filter,
+                    filter_ext=dust_param[f"phot_ext_{self.ext_filter}"],
+                    v_band_red=ism_reddening,
+                )
+
+                ext_spec = dust_util.ism_extinction(
+                    av_required, ism_reddening, self.spectrum[item][0][:, 0]
+                )
+
+                model_flux *= 10.0 ** (-0.4 * ext_spec)
 
             if self.spectrum[item][2] is not None:
                 # Use the inverted covariance matrix
                 ln_like += (
                     -0.5
                     * weight
                     * np.dot(
@@ -1719,14 +1858,17 @@
         attr_dict = {
             "spec_type": "model",
             "spec_name": self.model,
             "ln_evidence": (ln_z, ln_z_error),
             "parallax": self.parallax[0],
         }
 
+        if self.ext_filter is not None:
+            attr_dict["ext_filter"] = self.ext_filter
+
         # Add samples to the database
 
         if mpi_rank == 0:
             # Writing the samples to the database is only possible when using a single process
             species_db = database.Database()
 
             species_db.add_samples(
@@ -1944,14 +2086,17 @@
         attr_dict = {
             "spec_type": "model",
             "spec_name": self.model,
             "ln_evidence": (ln_z, ln_z_error),
             "parallax": self.parallax[0],
         }
 
+        if self.ext_filter is not None:
+            attr_dict["ext_filter"] = self.ext_filter
+
         # Add samples to the database
 
         if mpi_rank == 0:
             # Writing the samples to the database is only
             # possible when using a single process
             species_db = database.Database()
```

### Comparing `species-0.5.5/species/analysis/fit_spectrum.py` & `species-0.6.0/species/analysis/fit_spectrum.py`

 * *Files identical despite different names*

### Comparing `species-0.5.5/species/analysis/retrieval.py` & `species-0.6.0/species/analysis/retrieval.py`

 * *Files identical despite different names*

### Comparing `species-0.5.5/species/core/box.py` & `species-0.6.0/species/core/box.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,35 +60,44 @@
         if "iso_tag" in kwargs:
             box.iso_tag = kwargs["iso_tag"]
 
     elif boxtype == "cooling":
         box = CoolingBox()
         box.model = kwargs["model"]
         box.mass = kwargs["mass"]
-        box.filters_color = kwargs["filters_color"]
-        box.filter_mag = kwargs["filter_mag"]
-        box.color = kwargs["color"]
-        box.magnitude = kwargs["magnitude"]
-        box.ages = kwargs["ages"]
-        box.log_lum = kwargs["log_lum"]
+        if "age" in kwargs:
+            box.age = kwargs["age"]
+        else:
+            box.age = kwargs["ages"]
         box.teff = kwargs["teff"]
+        box.log_lum = kwargs["log_lum"]
         box.logg = kwargs["logg"]
+        box.radius = kwargs["radius"]
+        box.filter_mag = kwargs["filter_mag"]
+        box.magnitude = kwargs["magnitude"]
+        box.filters_color = kwargs["filters_color"]
+        box.color = kwargs["color"]
+
 
     elif boxtype == "isochrone":
         box = IsochroneBox()
         box.model = kwargs["model"]
         box.age = kwargs["age"]
-        box.filters_color = kwargs["filters_color"]
-        box.filter_mag = kwargs["filter_mag"]
-        box.color = kwargs["color"]
-        box.magnitude = kwargs["magnitude"]
-        box.log_lum = kwargs["log_lum"]
+        if "mass" in kwargs:
+            box.mass = kwargs["mass"]
+        else:
+            box.mass = kwargs["masses"]
         box.teff = kwargs["teff"]
+        box.log_lum = kwargs["log_lum"]
         box.logg = kwargs["logg"]
-        box.masses = kwargs["masses"]
+        box.radius = kwargs["radius"]
+        box.filter_mag = kwargs["filter_mag"]
+        box.magnitude = kwargs["magnitude"]
+        box.filters_color = kwargs["filters_color"]
+        box.color = kwargs["color"]
 
     elif boxtype == "model":
         box = ModelBox()
         box.model = kwargs["model"]
         box.wavelength = kwargs["wavelength"]
         box.flux = kwargs["flux"]
         box.parameters = kwargs["parameters"]
@@ -165,14 +174,20 @@
         if "spec_res" in kwargs:
             box.spec_res = kwargs["spec_res"]
 
     elif boxtype == "synphot":
         box = SynphotBox()
         box.name = kwargs["name"]
         box.flux = kwargs["flux"]
+        if "wavelength" in kwargs:
+            box.wavelength = kwargs["wavelength"]
+        if "app_mag" in kwargs:
+            box.app_mag = kwargs["app_mag"]
+        if "abs_mag" in kwargs:
+            box.abs_mag = kwargs["abs_mag"]
 
     return box
 
 
 class Box:
     """
     Class for generic methods that can be applied on all `Box` object.
@@ -267,22 +282,23 @@
         -------
         NoneType
             None
         """
 
         self.model = None
         self.mass = None
-        self.filters_color = None
-        self.filter_mag = None
-        self.color = None
-        self.magnitude = None
-        self.ages = None
-        self.log_lum = None
+        self.age = None
         self.teff = None
+        self.log_lum = None
         self.logg = None
+        self.radius = None
+        self.filter_mag = None
+        self.magnitude = None
+        self.filters_color = None
+        self.color = None
 
 
 class IsochroneBox(Box):
     """
     Class for storing isochrone data in a
     :class:`~species.core.box.Box`.
     """
@@ -293,22 +309,23 @@
         -------
         NoneType
             None
         """
 
         self.model = None
         self.age = None
-        self.filters_color = None
-        self.filter_mag = None
-        self.color = None
-        self.magnitude = None
-        self.log_lum = None
+        self.mass = None
         self.teff = None
+        self.log_lum = None
         self.logg = None
-        self.masses = None
+        self.radius = None
+        self.filter_mag = None
+        self.magnitude = None
+        self.filters_color = None
+        self.color = None
 
 
 class PhotometryBox(Box):
     """
     Class for storing photometric data in a
     :class:`~species.core.box.Box`.
     """
@@ -564,8 +581,11 @@
         Returns
         -------
         NoneType
             None
         """
 
         self.name = None
+        self.wavelength = None
         self.flux = None
+        self.app_mag = None
+        self.abs_mag = None
```

### Comparing `species-0.5.5/species/core/constants.py` & `species-0.6.0/species/core/constants.py`

 * *Files identical despite different names*

### Comparing `species-0.5.5/species/core/init.py` & `species-0.6.0/species/core/init.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,92 +23,111 @@
         """
         Returns
         -------
         NoneType
             None
         """
 
-        print(f"Initiating species v{species.__version__}...", end="", flush=True)
+        species_msg = f"species v{species.__version__}"
+        print(len(species_msg) * "=")
+        print(species_msg)
+        print(len(species_msg) * "=")
 
         working_folder = os.path.abspath(os.getcwd())
+        print(f"Working folder: {working_folder}")
 
         config_file = os.path.join(working_folder, "species_config.ini")
 
-        print(" [DONE]")
-
         try:
             contents = urllib.request.urlopen(
                 "https://pypi.org/pypi/species/json", timeout=1.0
             ).read()
 
             data = json.loads(contents)
             latest_version = data["info"]["version"]
 
         except (urllib.error.URLError, socket.timeout):
             latest_version = None
 
         if latest_version is not None and species.__version__ != latest_version:
             print(f"A new version ({latest_version}) is available!")
-            print("Want to stay informed about updates?")
-            print("Please have a look at the Github page:")
-            print("https://github.com/tomasstolker/species")
+            print("It is recommended to update to the latest version, "
+                  "see https://github.com/tomasstolker/species.")
 
         if not os.path.isfile(config_file):
-
             print("Creating species_config.ini...", end="", flush=True)
 
             with open(config_file, "w") as file_obj:
                 file_obj.write("[species]\n\n")
 
                 file_obj.write("; File with the HDF5 database\n")
                 file_obj.write("database = species_database.hdf5\n\n")
 
                 file_obj.write("; Folder where data will be downloaded\n")
                 file_obj.write("data_folder = ./data/\n\n")
 
                 file_obj.write("; Method for the grid interpolation\n")
-                file_obj.write("; Options: linear, nearest, slinear, "
-                               "cubic, quintic, pchip\n")
+                file_obj.write(
+                    "; Options: linear, nearest, slinear, " "cubic, quintic, pchip\n"
+                )
                 file_obj.write("interp_method = linear\n")
 
             print(" [DONE]")
 
         config = configparser.ConfigParser()
         config.read(config_file)
 
         if "database" in config["species"]:
             database_file = os.path.abspath(config["species"]["database"])
+
         else:
             database_file = "species_database.hdf5"
+
             with open(config_file, "a") as file_obj:
                 file_obj.write("\n; File with the HDF5 database\n")
                 file_obj.write("database = species_database.hdf5\n")
 
         if "data_folder" in config["species"]:
             data_folder = os.path.abspath(config["species"]["data_folder"])
+
         else:
             data_folder = "./data/"
+
             with open(config_file, "a") as file_obj:
                 file_obj.write("\n; Folder where data will be downloaded\n")
                 file_obj.write("data_folder = ./data/\n")
 
         if "interp_method" in config["species"]:
             interp_method = config["species"]["interp_method"]
+
         else:
             interp_method = "linear"
+
             with open(config_file, "a") as file_obj:
                 file_obj.write("\n; Method for the grid interpolation\n")
-                file_obj.write("; Options: linear, nearest, slinear, "
-                               "cubic, quintic, pchip\n")
+                file_obj.write(
+                    "; Options: linear, nearest, slinear, " "cubic, quintic, pchip\n"
+                )
                 file_obj.write("interp_method = linear\n")
 
-        print(f"Database: {database_file}")
-        print(f"Data folder: {data_folder}")
-        print(f"Working folder: {working_folder}")
-        print(f"Grid interpolation method: {interp_method}")
+        if "vega_mag" in config["species"]:
+            vega_mag = config["species"]["vega_mag"]
+
+        else:
+            vega_mag = 0.03
+
+            with open(config_file, "a") as file_obj:
+                file_obj.write("\n; Magnitude of Vega for all filters\n")
+                file_obj.write("vega_mag = 0.03\n")
+
+        print("Configuration settings:")
+        print(f"   - Database: {database_file}")
+        print(f"   - Data folder: {data_folder}")
+        print(f"   - Interpolation method: {interp_method}")
+        print(f"   - Magnitude of Vega: {vega_mag}")
 
         if not os.path.isfile(database_file):
             print("Creating species_database.hdf5...", end="", flush=True)
             h5_file = h5py.File(database_file, "w")
             h5_file.close()
             print(" [DONE]")
```

### Comparing `species-0.5.5/species/data/accretion.py` & `species-0.6.0/species/data/accretion.py`

 * *Files identical despite different names*

### Comparing `species-0.5.5/species/data/allers2013.py` & `species-0.6.0/species/data/allers2013.py`

 * *Files identical despite different names*

### Comparing `species-0.5.5/species/data/bonnefoy2014.py` & `species-0.6.0/species/data/bonnefoy2014.py`

 * *Files identical despite different names*

### Comparing `species-0.5.5/species/data/companion_data.json` & `species-0.6.0/species/data/companion_data.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9763750461424879%*

 * *Differences: {"'SR 12 C'": "{'references': {insert: [(3, 'Santamaría-Miranda et al. 2018'), (4, "*

 * *              "'Santamaría-Miranda et al. 2019 (erratum)')], delete: [4, 3]}}",*

 * * "'VHS 1256 B'": "OrderedDict([('simbad', 'SIPS J1256-1257'), ('parallax', [47.2733, 0.4731]), "*

 * *                 "('app_mag', OrderedDict([('2MASS/2MASS.J', [16.662, 0.287]), ('2MASS/2MASS.H', "*

 * *                 "[15.595, 0.209]), ('2MASS/2MASS.Ks', [14.568, 0.121]), ('WISE/WISE.W1', [13.6, "*

 * *                 "0.5]), ('WISE/WISE.W2', [12.8, 0.5 […]*

```diff
@@ -1943,23 +1943,69 @@
             8.9034,
             0.4288
         ],
         "references": [
             "Bowler et al. 2014",
             "Gaia Data Release 2",
             "Kuzuhara et al. 2011",
-            "Santamar\u00eda-Miranda et al. 2017",
-            "Santamar\u00eda-Miranda et al. 2017 (erratum)"
+            "Santamar\u00eda-Miranda et al. 2018",
+            "Santamar\u00eda-Miranda et al. 2019 (erratum)"
         ],
         "semi_major": [
             1100.0,
             0.0
         ],
         "simbad": "2MASS J16271951-2441403"
     },
+    "VHS 1256 B": {
+        "accretion": false,
+        "app_mag": {
+            "2MASS/2MASS.H": [
+                15.595,
+                0.209
+            ],
+            "2MASS/2MASS.J": [
+                16.662,
+                0.287
+            ],
+            "2MASS/2MASS.Ks": [
+                14.568,
+                0.121
+            ],
+            "WISE/WISE.W1": [
+                13.6,
+                0.5
+            ],
+            "WISE/WISE.W2": [
+                12.8,
+                0.5
+            ]
+        },
+        "mass_companion": [
+            11.2,
+            10.0
+        ],
+        "mass_star": [
+            0.07,
+            0.02
+        ],
+        "parallax": [
+            47.2733,
+            0.4731
+        ],
+        "references": [
+            "Gaia Early Data Release 3",
+            "Gauza et al. 2015"
+        ],
+        "semi_major": [
+            150.0,
+            150.0
+        ],
+        "simbad": "SIPS J1256-1257"
+    },
     "YSES 1 b": {
         "accretion": true,
         "app_mag": {
             "Paranal/NACO.Lp": [
                 13.3,
                 0.08
             ],
```

### Comparing `species-0.5.5/species/data/companion_spectra.json` & `species-0.6.0/species/data/companion_spectra.json`

 * *Files identical despite different names*

### Comparing `species-0.5.5/species/data/companion_spectra.py` & `species-0.6.0/species/data/companion_spectra.py`

 * *Files identical despite different names*

### Comparing `species-0.5.5/species/data/database.py` & `species-0.6.0/species/data/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,36 +3,39 @@
 """
 
 import configparser
 import json
 import os
 import pathlib
 import sys
+
 # import urllib.error
 import warnings
 
 from typing import Dict, List, Optional, Tuple, Union
 
 import emcee
 import h5py
 import numpy as np
 
 from astropy.io import fits
+
 # from astroquery.simbad import Simbad
 from scipy.integrate import simps
 from tqdm.auto import tqdm
 from typeguard import typechecked
 
 from species.analysis import photometry
 from species.core import box, constants
 from species.data import (
     accretion,
     allers2013,
     bonnefoy2014,
     companion_spectra,
+    custom_model,
     dust,
     filters,
     irtf,
     isochrones,
     kesseli2017,
     leggett,
     model_spectra,
@@ -308,15 +311,15 @@
 
         data_file = pathlib.Path(__file__).parent.resolve() / "companion_data.json"
 
         with open(data_file, "r", encoding="utf-8") as json_file:
             comp_data = json.load(json_file)
 
         if name is None:
-            name = comp_data.keys()
+            name = list(comp_data.keys())
 
         for item in name:
             spec_dict = companion_spectra.companion_spectra(
                 self.input_path, item, verbose=verbose
             )
 
             parallax = None
@@ -535,22 +538,22 @@
     ) -> None:
         """
         Function for adding isochrone data to the database.
 
         Parameters
         ----------
         model : str
-            Evolutionary model ('ames', 'bt-settl', 'sonora',
-            'saumon2008', 'nextgen', 'baraffe2015', or 'manual').
-            Isochrones will be automatically downloaded.
-            Alternatively, isochrone data can be downloaded from
-            https://phoenix.ens-lyon.fr/Grids/ or
-            https://perso.ens-lyon.fr/isabelle.baraffe/, and can be
-            manually added by setting the ``filename`` and ``tag``
-            arguments, and setting ``model='manual'``.
+            Evolutionary model ('ames', 'atmo', 'baraffe2015',
+            'bt-settl', 'nextgen', 'saumon2008', 'sonora',
+            or 'manual'). Isochrones will be automatically
+            downloaded. Alternatively, isochrone data can be
+            downloaded from https://phoenix.ens-lyon.fr/Grids/ or
+            https://perso.ens-lyon.fr/isabelle.baraffe/, and can
+            be manually added by setting the ``filename`` and
+            ``tag`` arguments, and setting ``model='manual'``.
         filename : str, None
             Filename with the isochrone data. Only required with
             ``model='manual'`` and can be set to ``None`` otherwise.
         tag : str
             Database tag name where the isochrone that will be stored.
             Only required with ``model='manual'`` and can be set to
             ``None`` otherwise.
@@ -558,89 +561,111 @@
         Returns
         -------
         NoneType
             None
         """
 
         if model == "phoenix":
-            warnings.warn("Please set model='manual' instead of "
-                          "model='phoenix' when using the filename "
-                          "parameter for adding isochrone data.",
-                          DeprecationWarning)
+            warnings.warn(
+                "Please set model='manual' instead of "
+                "model='phoenix' when using the filename "
+                "parameter for adding isochrone data.",
+                DeprecationWarning,
+            )
 
         h5_file = h5py.File(self.database, "a")
 
         if "isochrones" not in h5_file:
             h5_file.create_group("isochrones")
 
-        if model in ["phoenix", "marleau", "manual"]:
+        if model in ["manual", "marleau", "phoenix"]:
             if f"isochrones/{tag}" in h5_file:
                 del h5_file[f"isochrones/{tag}"]
 
         elif model == "ames":
             if "isochrones/ames-cond" in h5_file:
                 del h5_file["isochrones/ames-cond"]
             if "isochrones/ames-dusty" in h5_file:
                 del h5_file["isochrones/ames-dusty"]
 
+        elif model == "atmo":
+            if "isochrones/atmo-ceq" in h5_file:
+                del h5_file["isochrones/atmo-ceq"]
+            if "isochrones/atmo-neq-weak" in h5_file:
+                del h5_file["isochrones/atmo-neq-weak"]
+            if "isochrones/atmo-neq-strong" in h5_file:
+                del h5_file["isochrones/atmo-neq-strong"]
+
+        elif model == "baraffe2015":
+            if "isochrones/baraffe2015" in h5_file:
+                del h5_file["isochrones/baraffe2015"]
+
         elif model == "bt-settl":
             if "isochrones/bt-settl" in h5_file:
                 del h5_file["isochrones/bt-settl"]
 
-        elif model == "sonora":
-            if "isochrones/sonora+0.0" in h5_file:
-                del h5_file["isochrones/sonora+0.0"]
-            if "isochrones/sonora+0.5" in h5_file:
-                del h5_file["isochrones/sonora+0.5"]
-            if "isochrones/sonora-0.5" in h5_file:
-                del h5_file["isochrones/sonora-0.5"]
+        elif model == "nextgen":
+            if "isochrones/nextgen" in h5_file:
+                del h5_file["isochrones/nextgen"]
 
         elif model == "saumon2008":
             if "isochrones/saumon2008-nc_solar" in h5_file:
                 del h5_file["isochrones/saumon2008-nc_solar"]
             if "isochrones/saumon2008-nc_-0.3" in h5_file:
                 del h5_file["isochrones/saumon2008-nc_-0.3"]
             if "isochrones/saumon2008-nc_+0.3" in h5_file:
                 del h5_file["isochrones/saumon2008-nc_+0.3"]
             if "isochrones/saumon2008-f2_solar" in h5_file:
                 del h5_file["isochrones/saumon2008-f2_solar"]
             if "isochrones/saumon2008-hybrid_solar" in h5_file:
                 del h5_file["isochrones/saumon2008-hybrid_solar"]
 
-        elif model == "nextgen":
-            if "isochrones/nextgen" in h5_file:
-                del h5_file["isochrones/nextgen"]
+        elif model == "sonora":
+            if "isochrones/sonora+0.0" in h5_file:
+                del h5_file["isochrones/sonora+0.0"]
+            if "isochrones/sonora+0.5" in h5_file:
+                del h5_file["isochrones/sonora+0.5"]
+            if "isochrones/sonora-0.5" in h5_file:
+                del h5_file["isochrones/sonora-0.5"]
+
+        if model == "ames":
+            isochrones.add_ames(h5_file, self.input_path)
+
+        elif model == "atmo":
+            isochrones.add_atmo(h5_file, self.input_path)
 
         elif model == "baraffe2015":
-            if "isochrones/baraffe2015" in h5_file:
-                del h5_file["isochrones/baraffe2015"]
+            isochrones.add_baraffe2015(h5_file, self.input_path)
+
+        elif model == "bt-settl":
+            isochrones.add_btsettl(h5_file, self.input_path)
 
-        if model == "manual":
+        elif model == "manual":
             isochrones.add_manual(h5_file, tag, filename)
 
         elif model == "marleau":
             isochrones.add_marleau(h5_file, tag, filename)
 
-        elif model == "ames":
-            isochrones.add_ames(h5_file, self.input_path)
-
-        elif model == "bt-settl":
-            isochrones.add_btsettl(h5_file, self.input_path)
-
-        elif model == "sonora":
-            isochrones.add_sonora(h5_file, self.input_path)
+        elif model == "nextgen":
+            isochrones.add_nextgen(h5_file, self.input_path)
 
         elif model == "saumon2008":
             isochrones.add_saumon(h5_file, self.input_path)
 
-        elif model == "nextgen":
-            isochrones.add_nextgen(h5_file, self.input_path)
+        elif model == "sonora":
+            isochrones.add_sonora(h5_file, self.input_path)
 
-        elif model == "baraffe2015":
-            isochrones.add_baraffe2015(h5_file, self.input_path)
+        else:
+            raise ValueError(
+                f"The evolutionary model '{model}' is "
+                "not supported. Please choose another "
+                "argument for 'model'. Have a look "
+                "at the documentation of add_isochrones "
+                "for details on the supported models."
+            )
 
         h5_file.close()
 
     @typechecked
     def add_model(
         self,
         model: str,
@@ -659,15 +684,16 @@
         calculated with a constant step size in wavenumber,
         so the original spectral resolution decreased from short
         to long wavelengths.
 
         Parameters
         ----------
         model : str
-            Model name ('ames-cond', 'ames-dusty', 'atmo', 'bt-settl',
+            Model name ('ames-cond', 'ames-dusty', 'atmo-ceq',
+            'atmo-neq-weak', 'atmo-neq-strong', 'bt-settl',
             'bt-settl-cifist', 'bt-nextgen', 'drift-phoenix',
             'petitcode-cool-clear', 'petitcode-cool-cloudy',
             'petitcode-hot-clear', 'petitcode-hot-cloudy', 'exo-rem',
             'blackbody', bt-cond', 'bt-cond-feh, 'morley-2012',
             'sonora-cholla', 'sonora-bobcat', 'sonora-bobcat-co',
             'koester-wd', 'saumon2008-clear', 'saumon2008-cloudy',
             'petrus2023').
@@ -697,14 +723,96 @@
                 h5_file.create_group("models")
 
             model_spectra.add_model_grid(
                 model, self.input_path, h5_file, wavel_range, teff_range, spec_res
             )
 
     @typechecked
+    def add_custom_model(
+        self,
+        model: str,
+        data_path: str,
+        parameters: List[str],
+        wavel_range: Optional[Tuple[float, float]] = None,
+        spec_res: Optional[float] = None,
+        teff_range: Optional[Tuple[float, float]] = None,
+    ) -> None:
+        """
+        Function for adding a custom grid of model spectra to the
+        database. The spectra are read from the ``data_path`` and
+        should contain the ``model_name`` and ``parameters`` in
+        the filenames in the following format example:
+        `model-name_teff_1000_logg_4.0_feh_0.0_spec.dat`. The
+        list with ``parameters`` should contain the same parameters
+        as are included in the filename. Each datafile should contain
+        two columns with the wavelengths in :math:`\\mu\\text{m}`
+        and the fluxes in
+        :math:`\\text{W} \\text{m}^{-2} \\mu\\text{m}^{-1}`. Each file
+        should contain the same number and values of wavelengths. The
+        wavelengths should be logarithmically sampled, so at a constant
+        resolution, :math:`\\lambda/\\Delta\\lambda`. If not, then the
+        ``wavel_range`` and ``spec_res`` parameters should be used
+        such that the wavelengths are resampled when reading the data
+        into the ``species`` database.
+
+        Parameters
+        ----------
+        model : str
+            Name of the model grid. Should be identical to the model
+            name that is used in the filenames.
+        data_path : str
+            Path where the files with the model spectra are located.
+            It is best to provide an absolute path to the folder.
+        parameters : list(str)
+            List with the model parameters. The following parameters
+            are supported: ``teff`` (for :math:`T_\\mathrm{eff}`),
+            ``logg`` (for :math:`\\log\\,g`), ``feh`` (for [Fe/H]),
+            ``c_o_ratio`` (for C/O), ``fsed`` (for
+            :math:`f_\\mathrm{sed}`), ``log_kzz`` (for
+            :math:`\\log\\,K_\\mathrm{zz}`), and ``ad_index`` (for
+            :math:`\\gamma_\\mathrm{ad}`). Please contact the code
+            maintainer if support for other parameters should be added.
+        wavel_range : tuple(float, float), None
+            Wavelength range (:math:`\\mu\\text{m}`) for adding a
+            subset of the spectra. The full wavelength range is
+            used if the argument is set to ``None``.
+        spec_res : float, None
+            Spectral resolution to which the spectra will be resampled.
+            This parameter should be used in combination with
+            ``wavel_range`` if the input spectra at ``data_path``
+            are not sampled at a constant
+            :math:`\\lambda/\\Delta\\lambda`. The argument is
+            only used if ``wavel_range`` is not ``None`` and it is
+            not used if set to ``None``.
+        teff_range : tuple(float, float), None
+            Effective temperature range (K) for adding a subset of the
+            model grid. The full parameter grid will be added if the
+            argument is set to ``None``.
+
+        Returns
+        -------
+        NoneType
+            None
+        """
+
+        with h5py.File(self.database, "a") as h5_file:
+            if "models" not in h5_file:
+                h5_file.create_group("models")
+
+            custom_model.add_custom_model_grid(
+                model,
+                data_path,
+                parameters,
+                h5_file,
+                wavel_range,
+                teff_range,
+                spec_res,
+            )
+
+    @typechecked
     def add_object(
         self,
         object_name: str,
         parallax: Optional[Tuple[float, float]] = None,
         distance: Optional[Tuple[float, float]] = None,
         app_mag: Optional[
             Dict[str, Union[Tuple[float, float], List[Tuple[float, float]]]]
@@ -880,15 +988,14 @@
                         filter_profile[:, 0], 10.0 ** (0.4 * ext_mag)
                     )
 
                 else:
                     dered_phot[mag_item] = 1.0
 
                 if isinstance(app_mag[mag_item], tuple):
-
                     try:
                         synphot = photometry.SyntheticPhotometry(mag_item)
 
                         flux[mag_item], error[mag_item] = synphot.magnitude_to_flux(
                             app_mag[mag_item][0], app_mag[mag_item][1]
                         )
 
@@ -907,15 +1014,14 @@
                         flux[mag_item], error[mag_item] = np.nan, np.nan
 
                 elif isinstance(app_mag[mag_item], list):
                     flux_list = []
                     error_list = []
 
                     for i, dupl_item in enumerate(app_mag[mag_item]):
-
                         try:
                             synphot = photometry.SyntheticPhotometry(mag_item)
 
                             flux_dupl, error_dupl = synphot.magnitude_to_flux(
                                 dupl_item[0], dupl_item[1]
                             )
 
@@ -1161,25 +1267,25 @@
                         f"Transposing the data of {key} because "
                         f"the first instead of the second axis "
                         f"has a length of 3."
                     )
 
                     read_spec[key] = read_spec[key].transpose()
 
-                nan_index = np.isnan(read_spec[key][:, 1])
+                nan_idx = np.isnan(read_spec[key][:, 1])
 
                 # Add NaN booleans to dictionary for adjusting
                 # the covariance matrix later on
-                spec_nan[key] = nan_index
+                spec_nan[key] = nan_idx
 
-                if sum(nan_index) != 0:
-                    read_spec[key] = read_spec[key][~nan_index, :]
+                if np.sum(nan_idx) != 0:
+                    read_spec[key] = read_spec[key][~nan_idx, :]
 
                     warnings.warn(
-                        f"Found {sum(nan_index)} fluxes with NaN in "
+                        f"Found {np.sum(nan_idx)} fluxes with NaN in "
                         f"the data of {key}. Removing the spectral "
                         f"fluxes that contain a NaN."
                     )
 
                 wavelength = read_spec[key][:, 0]
                 flux = read_spec[key][:, 1]
                 error = read_spec[key][:, 2]
@@ -1306,15 +1412,14 @@
                     print(f"      - Filename: {value[1]}")
                     print(f"      - Data shape: {read_cov[key].shape}")
 
             if verbose:
                 print("   - Spectral resolution:")
 
             for key, value in spectrum.items():
-
                 h5_file.create_dataset(
                     f"objects/{object_name}/spectrum/{key}/spectrum",
                     data=read_spec[key],
                 )
 
                 if read_cov[key] is not None:
                     h5_file.create_dataset(
@@ -1457,21 +1562,21 @@
                     )
 
                     data = np.transpose(data)
 
             else:
                 data = np.loadtxt(filename)
 
-        nan_index = np.isnan(data[:, 1])
+        nan_idx = np.isnan(data[:, 1])
 
-        if sum(nan_index) != 0:
-            data = data[~nan_index, :]
+        if np.sum(nan_idx) != 0:
+            data = data[~nan_idx, :]
 
             warnings.warn(
-                f"Found {sum(nan_index)} fluxes with NaN in "
+                f"Found {np.sum(nan_idx)} fluxes with NaN in "
                 f"the data of {filename}. Removing the "
                 f"spectral fluxes that contain a NaN."
             )
 
         if units is None:
             wavelength = scaling[0] * data[:, 0]  # (um)
             flux = scaling[1] * data[:, 1]  # (W m-2 um-1)
@@ -1501,23 +1606,23 @@
                 elif units["flux"] == "w m-2":
                     if units["wavelength"] == "um":
                         error = scaling[1] * data[:, 2] / wavelength  # (W m-2 um-1)
 
         else:
             error = np.repeat(0.0, wavelength.size)
 
-        # nan_index = np.isnan(flux)
+        # nan_idx = np.isnan(flux)
         #
-        # if sum(nan_index) != 0:
-        #     wavelength = wavelength[~nan_index]
-        #     flux = flux[~nan_index]
-        #     error = error[~nan_index]
+        # if np.sum(nan_idx) != 0:
+        #     wavelength = wavelength[~nan_idx]
+        #     flux = flux[~nan_idx]
+        #     error = error[~nan_idx]
         #
         #     warnings.warn(
-        #         f"Found {sum(nan_index)} fluxes with NaN in "
+        #         f"Found {np.sum(nan_idx)} fluxes with NaN in "
         #         f"the calibration spectrum. Removing the "
         #         f"spectral fluxes that contain a NaN."
         #     )
 
         print(f"Adding calibration spectrum: {tag}...", end="", flush=True)
 
         h5_file.create_dataset(
@@ -1587,15 +1692,15 @@
         h5_file.close()
 
     @typechecked
     def add_spectra(
         self, spec_library: str, sptypes: Optional[List[str]] = None
     ) -> None:
         """
-        Function for adding an empirical spectral library to the
+        Function for adding empirical spectral libraries to the
         database. The spectra are stored together with several
         attributes such as spectral type, parallax, and Simbad ID.
         The spectra can be read with the functionalities of
         :class:`~species.read.read_spectrum.ReadSpectrum`.
 
         Parameters
         ----------
@@ -1613,15 +1718,15 @@
         """
 
         h5_file = h5py.File(self.database, "a")
 
         if "spectra" not in h5_file:
             h5_file.create_group("spectra")
 
-        if "spectra/" + spec_library in h5_file:
+        if f"spectra/{spec_library}" in h5_file:
             del h5_file["spectra/" + spec_library]
 
         if spec_library[0:5] == "vega":
             vega.add_vega(self.input_path, h5_file)
 
         elif spec_library[0:5] == "irtf":
             irtf.add_irtf(self.input_path, h5_file, sptypes)
@@ -2038,14 +2143,19 @@
             n_error = 0
 
         if "binary" in dset.attrs:
             binary = dset.attrs["binary"]
         else:
             binary = False
 
+        if "ext_filter" in dset.attrs:
+            ext_filter = dset.attrs["ext_filter"]
+        else:
+            ext_filter = None
+
         ignore_param = []
 
         for i in range(n_scaling):
             ignore_param.append(dset.attrs[f"scaling{i}"])
 
         for i in range(n_error):
             ignore_param.append(dset.attrs[f"error{i}"])
@@ -2074,18 +2184,16 @@
             distance = None
 
         samples = np.asarray(dset)
 
         # samples = samples[samples[:, 2] > 100., ]
 
         if samples.ndim == 2:
-            ran_index = np.random.randint(samples.shape[0], size=random)
-            samples = samples[
-                ran_index,
-            ]
+            rand_index = np.random.randint(samples.shape[0], size=random)
+            samples = samples[rand_index, ]
 
         elif samples.ndim == 3:
             if burnin > samples.shape[0]:
                 raise ValueError(
                     f"The 'burnin' value is larger than the number of steps "
                     f"({samples.shape[1]}) that are made by the walkers."
                 )
@@ -2152,23 +2260,25 @@
                         param_0 = read_util.binary_to_single(model_param, 0)
 
                         specbox_0 = readmodel.get_model(
                             param_0,
                             spec_res=spec_res,
                             wavel_resample=wavel_resample,
                             smooth=True,
+                            ext_filter=ext_filter,
                         )
 
                         param_1 = read_util.binary_to_single(model_param, 1)
 
                         specbox_1 = readmodel.get_model(
                             param_1,
                             spec_res=spec_res,
                             wavel_resample=wavel_resample,
                             smooth=True,
+                            ext_filter=ext_filter,
                         )
 
                         flux_comb = (
                             model_param["spec_weight"] * specbox_0.flux
                             + (1.0 - model_param["spec_weight"]) * specbox_1.flux
                         )
 
@@ -2183,14 +2293,15 @@
 
                     else:
                         specbox = readmodel.get_model(
                             model_param,
                             spec_res=spec_res,
                             wavel_resample=wavel_resample,
                             smooth=True,
+                            ext_filter=ext_filter,
                         )
 
             elif spectrum_type == "calibration":
                 specbox = readcalib.get_spectrum(model_param)
 
             boxes.append(specbox)
 
@@ -2413,15 +2524,14 @@
 
         if "distance" in dset:
             distance = np.asarray(dset["distance"])
         else:
             distance = None
 
         if inc_phot:
-
             magnitude = {}
             flux = {}
             mean_wavel = {}
 
             for observatory in dset.keys():
                 if observatory not in ["parallax", "distance", "spectrum"]:
                     for filter_name in dset[observatory]:
@@ -2433,28 +2543,26 @@
 
                             filter_trans = read_filter.ReadFilter(name)
                             mean_wavel[name] = filter_trans.mean_wavelength()
 
             phot_filters = list(magnitude.keys())
 
         else:
-
             magnitude = None
             flux = None
             phot_filters = None
             mean_wavel = None
 
         if inc_spec and f"objects/{object_name}/spectrum" in h5_file:
             spectrum = {}
 
             for item in h5_file[f"objects/{object_name}/spectrum"]:
                 data_group = f"objects/{object_name}/spectrum/{item}"
 
                 if isinstance(inc_spec, bool) or item in inc_spec:
-
                     if f"{data_group}/covariance" not in h5_file:
                         spectrum[item] = (
                             np.asarray(h5_file[f"{data_group}/spectrum"]),
                             None,
                             None,
                             h5_file[f"{data_group}"].attrs["specres"],
                         )
@@ -2754,15 +2862,17 @@
 
             elif pt_profile in ["free", "monotonic"]:
                 if "pt_smooth" in param_index:
                     pt_smooth = item[param_index["pt_smooth"]]
                 else:
                     pt_smooth = 0.0
 
-                knot_press = np.logspace(np.log10(press[0]), np.log10(press[-1]), temp_nodes)
+                knot_press = np.logspace(
+                    np.log10(press[0]), np.log10(press[-1]), temp_nodes
+                )
 
                 knot_temp = []
                 for k in range(temp_nodes):
                     knot_temp.append(item[param_index[f"t{k}"]])
 
                 knot_temp = np.asarray(knot_temp)
 
@@ -2825,15 +2935,14 @@
         Returns
         -------
         NoneType
             None
         """
 
         with h5py.File(self.database, "a") as h5_file:
-
             if "results" not in h5_file:
                 h5_file.create_group("results")
 
             if "results/empirical" not in h5_file:
                 h5_file.create_group("results/empirical")
 
             if f"results/empirical/{tag}" in h5_file:
@@ -2880,51 +2989,59 @@
         object_name: str,
         spec_name: List[str],
         model: str,
         scale_spec: List[str],
         extra_scaling: Optional[np.ndarray],
     ) -> None:
         """
+        Function for adding results obtained with
+        :class:`~species.analysis.compare_spectra.CompareSpectra`
+        to the HDF5 database.
+
         Parameters
         ----------
         tag : str
             Database tag where the results will be stored.
         goodness_of_fit : np.ndarray
             Array with the goodness-of-fit values.
         flux_scaling : np.ndarray
-            Array with the best-fit scaling values to match the model spectra with the data.
+            Array with the best-fit scaling values to match the model
+            spectra with the data.
         model_param : list(str)
             List with the names of the model parameters.
         coord_points : list(np.ndarray)
-            List with 1D arrays of the model grid points, in the same order as ``model_param``.
+            List with 1D arrays of the model grid points, in the same
+            order as ``model_param``.
         object_name : str
             Object name as stored in the database with
             :func:`~species.data.database.Database.add_object` or
             :func:`~species.data.database.Database.add_companion`.
         spec_name : list(str)
-            List with spectrum names that are stored at the object data of ``object_name``.
+            List with spectrum names that are stored at the object
+            data of ``object_name``.
         model : str
             Atmospheric model grid that is used for the comparison.
         scale_spec : list(str)
-            List with spectrum names to which an additional scaling has been applied.
+            List with spectrum names to which an additional scaling
+            has been applied.
         extra_scaling : np.ndarray. None
-            Array with extra scalings that have been applied to the spectra of ``scale_spec``.
-            The argument can be set to ``None`` if no extra scalings have been applied.
+            Array with extra scalings that have been applied to the
+            spectra of ``scale_spec``. The argument can be set to
+            ``None`` if no extra scalings have been applied.
 
         Returns
         -------
         NoneType
             None
         """
 
         read_obj = read_object.ReadObject(object_name)
         parallax = read_obj.get_parallax()[0]  # (mas)
 
         with h5py.File(self.database, "a") as h5_file:
-
             if "results" not in h5_file:
                 h5_file.create_group("results")
 
             if "results/comparison" not in h5_file:
                 h5_file.create_group("results/comparison")
 
             if f"results/comparison/{tag}" in h5_file:
@@ -2974,30 +3091,28 @@
             print(f"   - Goodness-of-fit = {goodness_of_fit[best_index]:.2e}")
 
             for i, item in enumerate(model_param):
                 best_param = coord_points[i][best_index[i]]
                 dset.attrs[f"best_param{i}"] = best_param
                 print(f"   - {item} = {best_param}")
 
-            scaling = flux_scaling[best_index[0], best_index[1], best_index[2]]
+            scaling = flux_scaling[best_index]
 
             radius = np.sqrt(scaling * (1e3 * constants.PARSEC / parallax) ** 2)  # (m)
             radius /= constants.R_JUP  # (Rjup)
 
             dset.attrs["radius"] = radius
             print(f"   - Radius (Rjup) = {radius:.2f}")
 
             dset.attrs["scaling"] = scaling
             print(f"   - Scaling = {scaling:.2e}")
 
             for i, item in enumerate(scale_spec):
-                scale_tmp = (
-                    scaling
-                    / extra_scaling[best_index[0], best_index[1], best_index[2], i]
-                )
+                scaling_idx = list(best_index).append(i)
+                scale_tmp = scaling / extra_scaling[tuple(scaling_idx)]
                 print(f"   - {item} scaling = {scale_tmp:.2e}")
                 dset.attrs[f"scaling_{item}"] = scale_tmp
 
     def add_retrieval(
         self, tag: str, output_folder: str, inc_teff: bool = False
     ) -> None:
         """
@@ -3054,20 +3169,17 @@
 
         if samples.ndim == 1:
             warnings.warn(
                 f"Only 1 sample found in post_equal_weights.dat "
                 f"of the '{output_folder}' folder."
             )
 
-            samples = samples[
-                np.newaxis,
-            ]
+            samples = samples[np.newaxis, ]
 
         with h5py.File(self.database, "a") as h5_file:
-
             if "results" not in h5_file:
                 h5_file.create_group("results")
 
             if "results/fit" not in h5_file:
                 h5_file.create_group("results/fit")
 
             if f"results/fit/{tag}" in h5_file:
@@ -3170,17 +3282,21 @@
                     print("Importing petitRADTRANS...", end="", flush=True)
                     from petitRADTRANS.radtrans import Radtrans
 
                     print(" [DONE]")
 
                     print("Importing chemistry module...", end="", flush=True)
                     if "poor_mans_nonequ_chem" in sys.modules:
-                        from poor_mans_nonequ_chem.poor_mans_nonequ_chem import interpol_abundances
+                        from poor_mans_nonequ_chem.poor_mans_nonequ_chem import (
+                            interpol_abundances,
+                        )
                     else:
-                        from petitRADTRANS.poor_mans_nonequ_chem.poor_mans_nonequ_chem import interpol_abundances
+                        from petitRADTRANS.poor_mans_nonequ_chem.poor_mans_nonequ_chem import (
+                            interpol_abundances,
+                        )
                     print(" [DONE]")
 
                     rt_object = Radtrans(
                         line_species=radtrans["line_species"],
                         rayleigh_species=["H2", "He"],
                         cloud_species=radtrans["cloud_species"].copy(),
                         continuum_opacities=["H2-H2", "H2-He"],
@@ -3200,17 +3316,15 @@
                         rt_object.setup_opa_structure(pressure[::24])
 
                 desc = f"Calculating mass fractions of {cloud_item[:-6]}"
 
                 for j in tqdm(range(samples.shape[0]), desc=desc):
                     sample_dict = retrieval_util.list_to_dict(
                         parameters,
-                        samples[
-                            j,
-                        ],
+                        samples[j, ],
                     )
 
                     if radtrans["pt_profile"] == "molliere":
                         upper_temp = np.array(
                             [sample_dict["t1"], sample_dict["t2"], sample_dict["t3"]]
                         )
 
@@ -3300,17 +3414,15 @@
 
             desc = "Calculating quenching pressures"
 
             for i in tqdm(range(samples.shape[0]), desc=desc):
                 # Convert list of parameters and samples into dictionary
                 sample_dict = retrieval_util.list_to_dict(
                     parameters,
-                    samples[
-                        i,
-                    ],
+                    samples[i, ],
                 )
 
                 # Recalculate the P-T profile from the sampled parameters
 
                 pressure = np.logspace(-6, 3, n_pressures)  # (bar)
 
                 if radtrans["pt_profile"] == "molliere":
@@ -3890,15 +4002,17 @@
                 model_param["tint"],
                 pressure,
                 model_param["metallicity"],
                 model_param["c_o_ratio"],
             )
 
         else:
-            knot_press = np.logspace(np.log10(pressure[0]), np.log10(pressure[-1]), temp_nodes)
+            knot_press = np.logspace(
+                np.log10(pressure[0]), np.log10(pressure[-1]), temp_nodes
+            )
 
             knot_temp = []
             for i in range(temp_nodes):
                 knot_temp.append(model_param[f"t{i}"])
 
             knot_temp = np.asarray(knot_temp)
 
@@ -3910,15 +4024,17 @@
             temperature = retrieval_util.pt_spline_interp(
                 knot_press, knot_temp, pressure, pt_smooth=pt_smooth
             )
 
         if "poor_mans_nonequ_chem" in sys.modules:
             from poor_mans_nonequ_chem.poor_mans_nonequ_chem import interpol_abundances
         else:
-            from petitRADTRANS.poor_mans_nonequ_chem.poor_mans_nonequ_chem import interpol_abundances
+            from petitRADTRANS.poor_mans_nonequ_chem.poor_mans_nonequ_chem import (
+                interpol_abundances,
+            )
 
         # Interpolate the abundances, following chemical equilibrium
         abund_in = interpol_abundances(
             np.full(pressure.shape, model_param["c_o_ratio"]),
             np.full(pressure.shape, model_param["metallicity"]),
             temperature,
             pressure,
```

### Comparing `species-0.5.5/species/data/dust.py` & `species-0.6.0/species/data/dust.py`

 * *Files identical despite different names*

### Comparing `species-0.5.5/species/data/filters.py` & `species-0.6.0/species/data/filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,17 @@
     """
     Function for downloading filter profile data
     from the SVO Filter Profile Service.
 
     Parameters
     ----------
     filter_id : str
-        Filter name as listed on the website of the SVO
-        Filter Profile Service (see
-        http://svo2.cab.inta-csic.es/svo/theory/fps/).
+        Filter name as listed on the website of the `SVO
+        Filter Profile Service
+        <http://svo2.cab.inta-csic.es/svo/theory/fps/>`_.
 
     Returns
     -------
     np.ndarray
         Wavelength (um).
     np.ndarray
         Fractional transmission.
@@ -138,15 +138,15 @@
         except IndexError:
             wavelength = None
             transmission = None
             det_type = None
 
             warnings.warn(
                 f"Filter '{filter_id}' is not available "
-                f"on the SVO Filter ProfileService."
+                f"on the SVO Filter Profile Service."
             )
 
         except:
             os.remove("filter.xml")
 
             raise ValueError(
                 f"The filter data of '{filter_id}' could not "
```

### Comparing `species-0.5.5/species/data/irtf.py` & `species-0.6.0/species/data/irtf.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,16 @@
         "G": os.path.join(input_path, "irtf/G_fits_091201"),
         "K": os.path.join(input_path, "irtf/K_fits_091201"),
         "M": os.path.join(input_path, "irtf/M_fits_091201"),
         "L": os.path.join(input_path, "irtf/L_fits_091201"),
         "T": os.path.join(input_path, "irtf/T_fits_091201"),
     }
 
+    main_folder = os.path.join(input_path, "irtf/")
+
     data_type = {
         "F": "F stars (4.4 MB)",
         "G": "G stars (5.6 MB)",
         "K": "K stars (5.5 MB)",
         "M": "M stars (7.5 MB)",
         "L": "L dwarfs (850 kB)",
         "T": "T dwarfs (100 kB)",
@@ -109,15 +111,15 @@
             )
             urllib.request.urlretrieve(url[item], data_file[item])
             print(" [DONE]")
 
     print("Unpacking IRTF Spectral Library...", end="", flush=True)
 
     for item in sptypes:
-        data_util.extract_tarfile(data_file[item], data_folder[item])
+        data_util.extract_tarfile(data_file[item], main_folder)
 
     print(" [DONE]")
 
     database.create_group("spectra/irtf")
 
     print_message = ""
```

### Comparing `species-0.5.5/species/data/kesseli2017.py` & `species-0.6.0/species/data/kesseli2017.py`

 * *Files identical despite different names*

### Comparing `species-0.5.5/species/data/leggett.py` & `species-0.6.0/species/data/leggett.py`

 * *Files identical despite different names*

### Comparing `species-0.5.5/species/data/model_data.json` & `species-0.6.0/species/data/model_data.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8873456790123456%*

 * *Differences: {"'ames-dusty'": "{'file size': '58 MB'}",*

 * * "'atmo-ceq'": "OrderedDict([('parameters', ['teff', 'logg']), ('name', 'ATMO CEQ'), ('file size', "*

 * *               "'455 MB'), ('wavelength range', [0.2, 6000]), ('resolution', 10000), ('teff "*

 * *               "range', [200, 3000]), ('reference', 'Phillips et al. (2020)'), ('url', "*

 * *               "'https://ui.adsabs.harvard.edu/abs/2020A%26A...637A..38P/abstract')])",*

 * * "'atmo-neq-strong'": "OrderedDict([('parameters', ['teff', 'logg']), ('name', 'ATMO NEQ strong') […]*

```diff
@@ -13,15 +13,15 @@
         ],
         "wavelength range": [
             0.5,
             40
         ]
     },
     "ames-dusty": {
-        "file size": "59 MB",
+        "file size": "58 MB",
         "name": "AMES-Dusty",
         "parameters": [
             "teff",
             "logg"
         ],
         "resolution": 4000,
         "teff range": [
@@ -48,14 +48,71 @@
         ],
         "url": "https://ui.adsabs.harvard.edu/abs/2020A%26A...637A..38P/abstract",
         "wavelength range": [
             0.4,
             6000
         ]
     },
+    "atmo-ceq": {
+        "file size": "455 MB",
+        "name": "ATMO CEQ",
+        "parameters": [
+            "teff",
+            "logg"
+        ],
+        "reference": "Phillips et al. (2020)",
+        "resolution": 10000,
+        "teff range": [
+            200,
+            3000
+        ],
+        "url": "https://ui.adsabs.harvard.edu/abs/2020A%26A...637A..38P/abstract",
+        "wavelength range": [
+            0.2,
+            6000
+        ]
+    },
+    "atmo-neq-strong": {
+        "file size": "274 MB",
+        "name": "ATMO NEQ strong",
+        "parameters": [
+            "teff",
+            "logg"
+        ],
+        "reference": "Phillips et al. (2020)",
+        "resolution": 10000,
+        "teff range": [
+            200,
+            1800
+        ],
+        "url": "https://ui.adsabs.harvard.edu/abs/2020A%26A...637A..38P/abstract",
+        "wavelength range": [
+            0.2,
+            6000
+        ]
+    },
+    "atmo-neq-weak": {
+        "file size": "276 MB",
+        "name": "ATMO NEQ weak",
+        "parameters": [
+            "teff",
+            "logg"
+        ],
+        "reference": "Phillips et al. (2020)",
+        "resolution": 10000,
+        "teff range": [
+            200,
+            1800
+        ],
+        "url": "https://ui.adsabs.harvard.edu/abs/2020A%26A...637A..38P/abstract",
+        "wavelength range": [
+            0.2,
+            6000
+        ]
+    },
     "blackbody": {
         "file size": "56 MB",
         "name": "blackbody",
         "parameters": [
             "teff"
         ],
         "resolution": 1000,
```

### Comparing `species-0.5.5/species/data/model_spectra.py` & `species-0.6.0/species/data/model_spectra.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """
 Module for adding a grid of model spectra to the database.
 """
 
 import json
 import os
 import pathlib
-import urllib.request
 import warnings
 
 from typing import Optional, Tuple
 
 import h5py
-import spectres
 import numpy as np
+import pooch
+import spectres
 
 from typeguard import typechecked
 
 from species.util import data_util, read_util
 
 
 @typechecked
@@ -79,19 +79,21 @@
             f"'petitcode-hot-cloudy', 'exo-rem', 'bt-settl-cifist', "
             f"'bt-cond', 'bt-cond-feh', 'blackbody', 'sonora-cholla', "
             f"'sonora-bobcat', 'sonora-bobcat-co', 'koester-wd', "
             f"'saumon2008-clear', 'saumon2008-cloudy', 'petrus2023' "
         )
 
     if model_name == "bt-settl":
-        warnings.warn("It is recommended to use the CIFIST "
-                      "grid of the BT-Settl, because it is "
-                      "a newer version. In that case, set "
-                      "model='bt-settl-cifist' when using "
-                      "add_model of Database.")
+        warnings.warn(
+            "It is recommended to use the CIFIST "
+            "grid of the BT-Settl, because it is "
+            "a newer version. In that case, set "
+            "model='bt-settl-cifist' when using "
+            "add_model of Database."
+        )
 
     if not os.path.exists(input_path):
         os.makedirs(input_path)
 
     input_file = f"{model_name}.tgz"
 
     data_folder = os.path.join(input_path, model_name)
@@ -99,38 +101,37 @@
 
     if not os.path.exists(data_folder):
         os.makedirs(data_folder)
 
     url = f"https://home.strw.leidenuniv.nl/~stolker/species/{model_name}.tgz"
 
     if not os.path.isfile(data_file):
-        print(
-            f"Downloading {model_info['name']} model "
-            f"spectra ({model_info['file size']})...",
-            end="",
-            flush=True,
-        )
-        urllib.request.urlretrieve(url, data_file)
-        print(" [DONE]")
+        pooch.retrieve(url=url,
+                       known_hash=None,
+                       fname=input_file,
+                       path=input_path,
+                       progressbar=True)
 
     print(
         f"Unpacking {model_info['name']} model "
         f"spectra ({model_info['file size']})...",
         end="",
         flush=True,
     )
     data_util.extract_tarfile(data_file, data_folder)
     print(" [DONE]")
 
     if "information" in model_info:
         print(f"Model information: {model_info['information']}")
 
     if "reference" in model_info:
-        print(f"Please cite {model_info['reference']} when "
-              f"using {model_info['name']} in a publication")
+        print(
+            f"Please cite {model_info['reference']} when "
+            f"using {model_info['name']} in a publication"
+        )
 
     if "url" in model_info:
         print(f"Reference URL: {model_info['url']}")
 
     teff = []
 
     if "logg" in model_info["parameters"]:
@@ -168,29 +169,32 @@
     if wavel_range is not None and spec_res is not None:
         wavelength = read_util.create_wavelengths(wavel_range, spec_res)
         print(f"Wavelength range (um) = {wavel_range[0]} - {wavel_range[1]}")
         print(f"Spectral resolution = {spec_res}")
 
     else:
         wavelength = None
-        print(f"Wavelength range (um) = "
-              f"{model_info['wavelength range'][0]} - "
-              f"{model_info['wavelength range'][1]}")
+        print(
+            f"Wavelength range (um) = "
+            f"{model_info['wavelength range'][0]} - "
+            f"{model_info['wavelength range'][1]}"
+        )
         print(f"Spectral resolution = {model_info['resolution']}")
 
     if teff_range is None:
-        print(f"Teff range (K) = {model_info['teff range'][0]} - {model_info['teff range'][1]}")
+        print(
+            f"Teff range (K) = {model_info['teff range'][0]} - {model_info['teff range'][1]}"
+        )
     else:
         print(f"Teff range (K) = {teff_range[0]} - {teff_range[1]}")
 
     print_message = ""
 
     for _, _, file_list in os.walk(data_folder):
         for filename in sorted(file_list):
-
             if filename[: len(model_name)] == model_name:
                 file_split = filename.split("_")
 
                 param_index = file_split.index("teff") + 1
                 teff_val = float(file_split[param_index])
 
                 if teff_range is not None:
@@ -235,18 +239,18 @@
                     os.path.join(data_folder, filename), unpack=True
                 )
 
                 if wavel_range is None or spec_res is None:
                     if wavelength is None:
                         wavelength = np.copy(data_wavel)  # (um)
 
-                    if np.all(np.diff(wavelength) < 0):
-                        raise ValueError(
-                            "The wavelengths are not all sorted by increasing value."
-                        )
+                        if np.all(np.diff(wavelength) < 0):
+                            raise ValueError(
+                                "The wavelengths are not all sorted by increasing value."
+                            )
 
                     flux.append(data_flux)  # (W m-2 um-1)
 
                 else:
                     flux_resample = spectres.spectres(
                         wavelength,
                         data_wavel,
```

### Comparing `species-0.5.5/species/data/spex.py` & `species-0.6.0/species/data/spex.py`

 * *Files identical despite different names*

### Comparing `species-0.5.5/species/data/vlm_plx.py` & `species-0.6.0/species/data/vlm_plx.py`

 * *Files identical despite different names*

### Comparing `species-0.5.5/species/plot/plot_color.py` & `species-0.6.0/species/plot/plot_color.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
-Module with functions for creating plots with color-magnitude
-diagrams and color-color diagrams.
+Module with functions for creating plots of
+color-magnitude  color-color diagrams.
 """
 
 import json
+import os
 import pathlib
 import warnings
 
 from typing import Dict, List, Optional, Tuple, Union
 
 import matplotlib as mpl
 import matplotlib.pyplot as plt
@@ -46,16 +47,16 @@
     label_x: str = "Color",
     label_y: str = "Absolute magnitude",
     xlim: Optional[Tuple[float, float]] = None,
     ylim: Optional[Tuple[float, float]] = None,
     offset: Optional[Tuple[float, float]] = None,
     legend: Optional[Union[str, dict, Tuple[float, float]]] = "upper left",
     figsize: Optional[Tuple[float, float]] = (4.0, 4.8),
-    output: Optional[str] = "color-magnitude.pdf",
-) -> None:
+    output: Optional[str] = None,
+) -> mpl.figure.Figure:
     """
     Function for creating a color-magnitude diagram.
 
     Parameters
     ----------
     boxes : list(species.core.box.ColorMagBox, species.core.box.IsochroneBox)
         Boxes with the color-magnitude and isochrone data from
@@ -81,20 +82,22 @@
         mass in :math:`M_\\mathrm{J}` and the position of the label
         ('left' or 'right), for
         example ``{'sonora+0.5': [(10., 'left'), (20., 'right')]}``.
         No labels will be shown if the argument is set to ``None`` or
         if an isochrone tag is not included in the dictionary. The
         tags are stored as the ``iso_tag`` attribute of each
         :class:`~species.core.box.ColorColorBox`.
-    teff_labels : list(float), list(tuple(float, str)), None
-        Plot labels with temperatures (K) next to the synthetic Planck
-        photometry. Alternatively, a list of tuples can be provided
-        with the planet mass and position of the label ('left' or
-        'right), for example ``[(1000., 'left'), (1200., 'right')]``.
-        No labels are shown if set to ``None``.
+    teff_labels : dict(str, list(tuple(float, str))), None
+        Plot labels with temperatures (K) next to the isochrones. The
+        argument is a dictionary with the names of the models and a
+        list with tuples that contain the effective temperatures and
+        'left' or 'right' to indicate the position of the label (so
+        similar to the use of mass_labels``). For example,
+        ``{'planck': [(1000., 'left'), (1200., 'right')]``. No labels
+        are shown if the argument is set to ``None``.
     companion_labels : bool
         Plot labels with the names of the directly imaged companions.
     accretion : bool
         Plot accreting, directly imaged objects with a different symbol
         than the regular, directly imaged objects. The object names
         from ``objects`` will be compared with the data from
         `data/companion_data.json` to check if a companion is
@@ -119,18 +122,21 @@
         list is a tuple that itself contain a tuple with the filter
         names for the color, the filter name of the magnitude, the
         visual extinction, and the start position (color, mag) of the
         arrow in the plot, so ``((filter_color_1, filter_color_2),
         filter_mag, A_V, (x_pos, y_pos))``. The parameter is not used
         if the argument is set to ``None``.
     field_range : tuple(str, str), None
-        Range of the discrete colorbar for the field dwarfs. The tuple
-        should contain the lower and upper value ('early M', 'late M',
-        'early L', 'late L', 'early T', 'late T', 'early Y). The full
-        range is used if set to ``None``.
+        Range of spectral types for which the field objects will be
+        plotted and labeled at the discrete colorbar. The tuple
+        should contain the lower and upper value of either the classes,
+        for example ('K', 'T'), or as subclasses by including
+        early/late, for example ('late K', 'early T'). The range is
+        set to the default of 'early M' to 'early Y' if the
+        argument is set to ``None``.
     label_x : str
         Label for the x-axis.
     label_y : str
         Label for the y-axis.
     xlim : tuple(float, float), None
         Limits for the x-axis. Not used if set to None.
     ylim : tuple(float, float), None
@@ -138,29 +144,27 @@
     offset : tuple(float, float), None
         Offset of the x- and y-axis label.
     legend : str, tuple(float, float), dict, None
         Legend position or keyword arguments. No legend
         is shown if set to ``None``.
     figsize : tuple(float, float)
         Figure size.
-    output : str
+    output : str, None
         Output filename for the plot. The plot is shown in an
         interface window if the argument is set to ``None``.
 
     Returns
     -------
-    NoneType
-        None
-
+    matplotlib.figure.Figure
+        The ``Figure`` object that can be used for further
+        customization of the plot.
     """
 
-    mpl.rcParams["font.family"] = "serif"
-    mpl.rcParams["mathtext.fontset"] = "dejavuserif"
-
-    plt.rc("axes", edgecolor="black", linewidth=2.2)
+    plt.rcParams["font.family"] = "serif"
+    plt.rcParams["mathtext.fontset"] = "dejavuserif"
 
     # model_color = ("#234398", "#f6a432", "black")
 
     model_color = (
         "tab:blue",
         "tab:orange",
         "tab:green",
@@ -170,14 +174,34 @@
         "tab:pink",
         "tab:olive",
         "tab:cyan",
     )
 
     model_linestyle = ("-", "--", ":", "-.")
 
+    if field_range is None:
+        field_range = ("early M", "early Y")
+
+    if (len(field_range[0]) == 1 and len(field_range[1]) != 1) or (
+        len(field_range[0]) != 1 and len(field_range[1]) == 1
+    ):
+        raise ValueError(
+            "The argument of 'field_range' should "
+            "be a tuple with either the range of "
+            "spectral type classes, for example "
+            "('A', 'M'), or a tuple with the range "
+            "of subclasses, for example ('early K', "
+            "'late L')."
+        )
+
+    if len(field_range[0]) == 1 and len(field_range[1]) == 1:
+        check_subclass = False
+    else:
+        check_subclass = True
+
     isochrones = []
     planck = []
     models = []
     empirical = []
 
     for item in boxes:
         if isinstance(item, box.IsochroneBox):
@@ -196,23 +220,23 @@
         else:
             raise ValueError(
                 f"Found a {type(item)} while only ColorMagBox and IsochroneBox "
                 f"objects can be provided to 'boxes'."
             )
 
     if empirical:
-        plt.figure(1, figsize=figsize)
+        fig = plt.figure(figsize=figsize)
         gridsp = mpl.gridspec.GridSpec(3, 1, height_ratios=[0.2, 0.1, 4.5])
         gridsp.update(wspace=0.0, hspace=0.0, left=0, right=1, bottom=0, top=1)
 
         ax1 = plt.subplot(gridsp[2, 0])
         ax2 = plt.subplot(gridsp[0, 0])
 
     else:
-        plt.figure(1, figsize=figsize)
+        fig = plt.figure(figsize=figsize)
         gridsp = mpl.gridspec.GridSpec(1, 1)
         gridsp.update(wspace=0.0, hspace=0.0, left=0, right=1, bottom=0, top=1)
 
         ax1 = plt.subplot(gridsp[0, 0])
 
     ax1.tick_params(
         axis="both",
@@ -340,16 +364,16 @@
                         lw=1.0,
                         color=model_color[model_count[0]],
                         label=label,
                         zorder=0,
                     )
 
                     if mass_labels is not None:
-                        interp_magnitude = interp1d(item.sptype, item.magnitude)
-                        interp_color = interp1d(item.sptype, item.color)
+                        interp_magnitude = interp1d(item.mass, item.magnitude)
+                        interp_color = interp1d(item.mass, item.color)
 
                         if item.iso_tag in mass_labels:
                             label_select = mass_labels[item.iso_tag]
                         else:
                             label_select = []
 
                         for i, mass_item in enumerate(label_select):
@@ -381,15 +405,14 @@
                             xlim = ax1.get_xlim()
                             ylim = ax1.get_ylim()
 
                             if (
                                 xlim[0] + 0.2 < pos_color < xlim[1] - 0.2
                                 and ylim[1] + 0.2 < pos_mag < ylim[0] - 0.2
                             ):
-
                                 ax1.scatter(
                                     pos_color,
                                     pos_mag,
                                     c=model_color[model_count[0]],
                                     s=15,
                                     edgecolor="none",
                                     zorder=0,
@@ -470,15 +493,14 @@
                         xlim = ax1.get_xlim()
                         ylim = ax1.get_ylim()
 
                         if (
                             xlim[0] + 0.2 < pos_color < xlim[1] - 0.2
                             and ylim[1] + 0.2 < pos_mag < ylim[0] - 0.2
                         ):
-
                             ax1.scatter(
                                 pos_color, pos_mag, c="gray", s=15, ec="none", zorder=0
                             )
 
                             if planck_count == 0:
                                 ax1.annotate(
                                     teff_label,
@@ -492,15 +514,17 @@
                                 )
 
             planck_count += 1
 
     if empirical:
         cmap = plt.cm.viridis
 
-        bounds, ticks, ticklabels = plot_util.field_bounds_ticks(field_range)
+        bounds, ticks, ticklabels = plot_util.field_bounds_ticks(
+            field_range, check_subclass
+        )
         norm = mpl.colors.BoundaryNorm(bounds, cmap.N)
 
         for item in empirical:
             sptype = item.sptype
             color = item.color
             magnitude = item.magnitude
             names = item.names
@@ -511,15 +535,17 @@
             if item.object_type in ["field", None]:
                 indices = np.where(sptype != "None")[0]
 
                 sptype = sptype[indices]
                 color = color[indices]
                 magnitude = magnitude[indices]
 
-                spt_disc = plot_util.sptype_substellar(sptype, color.shape)
+                spt_disc = plot_util.sptype_to_index(
+                    field_range, sptype, check_subclass
+                )
 
                 _, unique = np.unique(color, return_index=True)
 
                 sptype = sptype[unique]
                 color = color[unique]
                 magnitude = magnitude[unique]
                 spt_disc = spt_disc[unique]
@@ -748,30 +774,31 @@
             if isinstance(abs_mag, np.ndarray):
                 abs_mag = abs_mag[0]
                 abs_err = abs_err[0]
 
             colorerr = np.sqrt(objcolor1[1] ** 2 + objcolor2[1] ** 2)
             x_color = objcolor1[0] - objcolor2[0]
 
-            data_file = pathlib.Path(__file__).parent.resolve() / "companion_data.json"
+            species_folder = str(pathlib.Path(__file__).parent.resolve())[:-4]
+            data_file = os.path.join(species_folder, "data/companion_data.json")
 
             with open(data_file, "r", encoding="utf-8") as json_file:
                 comp_data = json.load(json_file)
 
             if len(item) > 4 and item[4] is not None:
                 kwargs = item[4]
 
             else:
                 kwargs = {
                     "marker": "o",
                     "ms": 5.0,
                     "color": "black",
                     "mfc": "white",
                     "mec": "black",
-                    "label": "Direct imaging",
+                    "label": "Companions",
                 }
 
                 if (
                     accretion
                     and item[0] in comp_data
                     and comp_data[item[0]]["accretion"]
                 ):
@@ -830,19 +857,18 @@
                 ax1.legend(by_label.values(), by_label.keys(), **legend)
 
     if output is None:
         plt.show()
     else:
         plt.savefig(output, bbox_inches="tight")
 
-    plt.clf()
-    plt.close()
-
     print(" [DONE]")
 
+    return fig
+
 
 @typechecked
 def plot_color_color(
     boxes: list,
     objects: Optional[
         Union[
             List[Tuple[str, Tuple[str, str], Tuple[str, str]]],
@@ -876,16 +902,16 @@
     label_x: str = "Color",
     label_y: str = "Color",
     xlim: Optional[Tuple[float, float]] = None,
     ylim: Optional[Tuple[float, float]] = None,
     offset: Optional[Tuple[float, float]] = None,
     legend: Optional[Union[str, dict, Tuple[float, float]]] = "upper left",
     figsize: Optional[Tuple[float, float]] = (4.0, 4.3),
-    output: Optional[str] = "color-color.pdf",
-) -> None:
+    output: Optional[str] = None,
+) -> mpl.figure.Figure:
     """
     Function for creating a color-color diagram.
 
     Parameters
     ----------
     boxes : list(species.core.box.ColorColorBox, species.core.box.IsochroneBox)
         Boxes with the color-color from photometric libraries,
@@ -907,37 +933,42 @@
         mass in :math:`M_\\mathrm{J}` and the position of the label
         ('left' or 'right), for
         example ``{'sonora+0.5': [(10., 'left'), (20., 'right')]}``.
         No labels will be shown if the argument is set to ``None`` or
         if an isochrone tag is not included in the dictionary. The
         tags are stored as the ``iso_tag`` attribute of each
         :class:`~species.core.box.ColorColorBox`.
-    teff_labels : list(float), list(tuple(float, str)), None
-        Plot labels with temperatures (K) next to the synthetic Planck
-        photometry. Alternatively, a list of tuples can be provided
-        with the planet mass and position of the label ('left' or
-        'right), for example ``[(1000., 'left'), (1200., 'right')]``.
-        No labels are shown if the argument is set to ``None``.
+    teff_labels : dict(str, list(tuple(float, str))), None
+        Plot labels with temperatures (K) next to the isochrones. The
+        argument is a dictionary with the names of the models and a
+        list with tuples that contain the effective temperatures and
+        'left' or 'right' to indicate the position of the label (so
+        similar to the use of mass_labels``). For example,
+        ``{'planck': [(1000., 'left'), (1200., 'right')]``. No labels
+        are shown if the argument is set to ``None``.
     companion_labels : bool
         Plot labels with the names of the directly imaged companions.
     reddening : list(tuple(tuple(str, str), tuple(str, str),
             tuple(str, float), str, float, tuple(float, float)), None
         Include reddening arrows by providing a list with tuples.
         Each tuple contains the filter names for the color, the filter
         name for the magnitude, the particle radius (um), and the start
         position (color, mag) of the arrow in the plot, so
         (filter_color_1, filter_color_2, filter_mag, composition,
         radius, (x_pos, y_pos)). The composition can be either 'Fe' or
         'MgSiO3' (both with crystalline structure). The parameter is
         not used if set to ``None``.
     field_range : tuple(str, str), None
-        Range of the discrete colorbar for the field dwarfs. The tuple
-        should contain the lower and upper value ('early M', 'late M',
-        'early L', 'late L', 'early T', 'late T', 'early Y).
-        The full range is used if the argument is set to ``None``.
+        Range of spectral types for which the field objects will be
+        plotted and labeled at the discrete colorbar. The tuple
+        should contain the lower and upper value of either the classes,
+        for example ('K', 'T'), or as subclasses by including
+        early/late, for example ('late K', 'early T'). The range is
+        set to the default of 'early M' to 'early Y' if the
+        argument is set to ``None``.
     label_x : str
         Label for the x-axis.
     label_y : str
         Label for the y-axis.
     xlim : tuple(float, float)
         Limits for the x-axis.
     ylim : tuple(float, float)
@@ -945,28 +976,27 @@
     offset : tuple(float, float), None
         Offset of the x- and y-axis label.
     legend : str, tuple(float, float), dict, None
         Legend position or dictionary with keyword arguments.
         No legend is shown if the argument is set to ``None``.
     figsize : tuple(float, float)
         Figure size.
-    output : str
+    output : str, None
         Output filename for the plot. The plot is shown in an
         interface window if the argument is set to ``None``.
 
     Returns
     -------
-    NoneType
-        None
+    matplotlib.figure.Figure
+        The ``Figure`` object that can be used for further
+        customization of the plot.
     """
 
-    mpl.rcParams["font.family"] = "serif"
-    mpl.rcParams["mathtext.fontset"] = "dejavuserif"
-
-    plt.rc("axes", edgecolor="black", linewidth=2.2)
+    plt.rcParams["font.family"] = "serif"
+    plt.rcParams["mathtext.fontset"] = "dejavuserif"
 
     # model_color = ("#234398", "#f6a432", "black")
 
     model_color = (
         "tab:blue",
         "tab:orange",
         "tab:green",
@@ -976,14 +1006,34 @@
         "tab:pink",
         "tab:olive",
         "tab:cyan",
     )
 
     model_linestyle = ("-", "--", ":", "-.")
 
+    if field_range is None:
+        field_range = ("early M", "early Y")
+
+    if (len(field_range[0]) == 1 and len(field_range[1]) != 1) or (
+        len(field_range[0]) != 1 and len(field_range[1]) == 1
+    ):
+        raise ValueError(
+            "The argument of 'field_range' should "
+            "be a tuple with either the range of "
+            "spectral type classes, for example "
+            "('A', 'M'), or a tuple with the range "
+            "of subclasses, for example ('early K', "
+            "'late L')."
+        )
+
+    if len(field_range[0]) == 1 and len(field_range[1]) == 1:
+        check_subclass = False
+    else:
+        check_subclass = True
+
     isochrones = []
     planck = []
     models = []
     empirical = []
     spectra = []
 
     for item in boxes:
@@ -1005,15 +1055,15 @@
 
         else:
             raise ValueError(
                 f"Found a {type(item)} while only ColorColorBox and "
                 f"IsochroneBox objects can be provided to 'boxes'."
             )
 
-    plt.figure(1, figsize=figsize)
+    fig = plt.figure(figsize=figsize)
 
     if empirical:
         gridsp = mpl.gridspec.GridSpec(3, 1, height_ratios=[0.2, 0.1, 4.0])
     else:
         gridsp = mpl.gridspec.GridSpec(1, 1)
 
     gridsp.update(wspace=0.0, hspace=0.0, left=0, right=1, bottom=0, top=1)
@@ -1148,16 +1198,16 @@
                         lw=1.0,
                         color=model_color[model_count[0]],
                         label=label,
                         zorder=0,
                     )
 
                     if mass_labels is not None:
-                        interp_color1 = interp1d(item.sptype, item.color1)
-                        interp_color2 = interp1d(item.sptype, item.color2)
+                        interp_color1 = interp1d(item.mass, item.color1)
+                        interp_color2 = interp1d(item.mass, item.color2)
 
                         if item.iso_tag in mass_labels:
                             label_select = mass_labels[item.iso_tag]
                         else:
                             label_select = []
 
                         for i, mass_item in enumerate(label_select):
@@ -1180,15 +1230,14 @@
                             xlim = ax1.get_xlim()
                             ylim = ax1.get_ylim()
 
                             if (
                                 xlim[0] + 0.2 < pos_color1 < xlim[1] - 0.2
                                 and ylim[0] + 0.2 < pos_color2 < ylim[1] - 0.2
                             ):
-
                                 ax1.scatter(
                                     pos_color1,
                                     pos_color2,
                                     c=model_color[model_count[0]],
                                     s=15,
                                     edgecolor="none",
                                     zorder=0,
@@ -1223,15 +1272,14 @@
                     zorder=0,
                 )
 
     if planck is not None:
         planck_count = 0
 
         for j, item in enumerate(planck):
-
             if planck_count == 0:
                 label = plot_util.model_name(item.library)
 
                 ax1.plot(
                     item.color1,
                     item.color2,
                     ls="--",
@@ -1276,15 +1324,14 @@
                             xlim = ax1.get_xlim()
                             ylim = ax1.get_ylim()
 
                             if (
                                 xlim[0] + 0.2 < pos_color1 < xlim[1] - 0.2
                                 and ylim[0] + 0.2 < pos_color2 < ylim[1] - 0.2
                             ):
-
                                 ax1.scatter(
                                     pos_color1,
                                     pos_color2,
                                     c="gray",
                                     s=15,
                                     edgecolor="none",
                                     zorder=0,
@@ -1308,15 +1355,14 @@
 
             planck_count += 1
 
     if spectra is not None:
         spectra_count = 0
 
         for j, item in enumerate(spectra):
-
             if spectra_count == 0:
                 label = plot_util.model_name(item.library)
 
                 ax1.plot(
                     item.color1,
                     item.color2,
                     ls="--",
@@ -1361,15 +1407,14 @@
                             xlim = ax1.get_xlim()
                             ylim = ax1.get_ylim()
 
                             if (
                                 xlim[0] + 0.2 < pos_color1 < xlim[1] - 0.2
                                 and ylim[0] + 0.2 < pos_color2 < ylim[1] - 0.2
                             ):
-
                                 ax1.scatter(
                                     pos_color1,
                                     pos_color2,
                                     c="tomato",
                                     s=15,
                                     edgecolor="none",
                                     zorder=0,
@@ -1392,15 +1437,17 @@
                 )
 
             spectra_count += 1
 
     if empirical:
         cmap = plt.cm.viridis
 
-        bounds, ticks, ticklabels = plot_util.field_bounds_ticks(field_range)
+        bounds, ticks, ticklabels = plot_util.field_bounds_ticks(
+            field_range, check_subclass
+        )
         norm = mpl.colors.BoundaryNorm(bounds, cmap.N)
 
         for item in empirical:
             sptype = item.sptype
             names = item.names
             color1 = item.color1
             color2 = item.color2
@@ -1411,15 +1458,17 @@
             if item.object_type in ["field", None]:
                 indices = np.where(sptype != "None")[0]
 
                 sptype = sptype[indices]
                 color1 = color1[indices]
                 color2 = color2[indices]
 
-                spt_disc = plot_util.sptype_substellar(sptype, color1.shape)
+                spt_disc = plot_util.sptype_to_index(
+                    field_range, sptype, check_subclass
+                )
                 _, unique = np.unique(color1, return_index=True)
 
                 sptype = sptype[unique]
                 color1 = color1[unique]
                 color2 = color2[unique]
                 spt_disc = spt_disc[unique]
 
@@ -1617,15 +1666,15 @@
             else:
                 kwargs = {
                     "marker": "o",
                     "ms": 5.0,
                     "color": "black",
                     "mfc": "white",
                     "mec": "black",
-                    "label": "Direct imaging",
+                    "label": "Companions",
                 }
 
             ax1.errorbar(color1, color2, xerr=error1, yerr=error2, zorder=3, **kwargs)
 
             if companion_labels:
                 if len(item) > 3 and item[4] is not None:
                     kwargs = item[4]
@@ -1675,11 +1724,10 @@
                 ax1.legend(by_label.values(), by_label.keys(), **legend)
 
     if output is None:
         plt.show()
     else:
         plt.savefig(output, bbox_inches="tight")
 
-    plt.clf()
-    plt.close()
-
     print(" [DONE]")
+
+    return fig
```

### Comparing `species-0.5.5/species/plot/plot_comparison.py` & `species-0.6.0/species/plot/plot_comparison.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """
-Module with a function for plotting results from the empirical spectral analysis.
+Module with functions for plotting results from a spectral
+analysis that compares data with a library of empirical
+spectra or a grid of model spectra
 """
 
 import configparser
 import os
 
 from typing import Optional, Tuple
 
@@ -14,46 +16,51 @@
 
 from matplotlib.ticker import AutoMinorLocator
 from scipy.interpolate import interp1d, RegularGridInterpolator
 from typeguard import typechecked
 
 from species.core import constants
 from species.read import read_object
-from species.util import dust_util, read_util
+from species.util import dust_util, plot_util, read_util
 
 
 @typechecked
 def plot_statistic(
     tag: str,
     xlim: Optional[Tuple[float, float]] = None,
     ylim: Optional[Tuple[float, float]] = None,
     title: Optional[str] = None,
     offset: Optional[Tuple[float, float]] = None,
     figsize: Optional[Tuple[float, float]] = (4.0, 2.5),
-    output: Optional[str] = "statistic.pdf",
-):
+    output: Optional[str] = None,
+) -> mpl.figure.Figure:
     """
-    Function for plotting the goodness-of-fit statistic of the empirical spectral comparison.
+    Function for plotting the goodness-of-fit statistic from a
+    comparison with an empirical spectral library with
+    :class:`~species.analysis.empirical.CompareSpectra.spectral_type`
+    that enables a determination of the spectral type
 
     Parameters
     ----------
     tag : str
         Database tag where the results from the empirical comparison with
-        :class:`~species.analysis.empirical.CompareSpectra.spectral_type` are stored.
+        :class:`~species.analysis.empirical.CompareSpectra.spectral_type`
+        are stored.
     xlim : tuple(float, float)
-        Limits of the spectral type axis in numbers (i.e. 0=M0, 5=M5, 10=L0, etc.).
+        Limits of the spectral type axis in numbers (i.e.
+        0=M0, 5=M5, 10=L0, etc.).
     ylim : tuple(float, float)
         Limits of the goodness-of-fit axis.
     title : str
         Plot title.
     offset : tuple(float, float)
         Offset for the label of the x- and y-axis.
     figsize : tuple(float, float)
         Figure size.
-    output : str
+    output : str, None
         Output filename for the plot. The plot is shown in an
         interface window if the argument is set to ``None``.
 
     Returns
     -------
     NoneType
         None
@@ -75,21 +82,19 @@
 
     dset = h5_file[f"results/empirical/{tag}/names"]
 
     names = np.array(dset)
     sptypes = np.array(h5_file[f"results/empirical/{tag}/sptypes"])
     g_fit = np.array(h5_file[f"results/empirical/{tag}/goodness_of_fit"])
 
-    mpl.rcParams["font.family"] = "serif"
-    mpl.rcParams["mathtext.fontset"] = "dejavuserif"
-
-    plt.rc("axes", edgecolor="black", linewidth=2.2)
+    plt.rcParams["font.family"] = "serif"
+    plt.rcParams["mathtext.fontset"] = "dejavuserif"
     plt.rcParams["axes.axisbelow"] = False
 
-    plt.figure(1, figsize=figsize)
+    fig = plt.figure(figsize=figsize)
     gridsp = mpl.gridspec.GridSpec(1, 1)
     gridsp.update(wspace=0, hspace=0, left=0, right=1, bottom=0, top=1)
 
     ax = plt.subplot(gridsp[0, 0])
 
     ax.tick_params(
         axis="both",
@@ -176,35 +181,34 @@
     )
 
     if output is None:
         plt.show()
     else:
         plt.savefig(output, bbox_inches="tight")
 
-    plt.clf()
-    plt.close()
-
     h5_file.close()
 
     print(" [DONE]")
 
+    return fig
+
 
 @typechecked
 def plot_empirical_spectra(
     tag: str,
     n_spectra: Optional[int] = None,
     flux_offset: Optional[float] = None,
     label_pos: Optional[Tuple[float, float]] = None,
     xlim: Optional[Tuple[float, float]] = None,
     ylim: Optional[Tuple[float, float]] = None,
     title: Optional[str] = None,
     offset: Optional[Tuple[float, float]] = None,
     figsize: Optional[Tuple[float, float]] = (4.0, 2.5),
-    output: Optional[str] = "empirical.pdf",
-):
+    output: Optional[str] = None,
+) -> mpl.figure.Figure:
     """
     Function for plotting the results from the empirical
     spectrum comparison.
 
     Parameters
     ----------
     tag : str
@@ -231,22 +235,23 @@
         Limits of the goodness-of-fit axis.
     title : str
         Plot title.
     offset : tuple(float, float)
         Offset for the label of the x- and y-axis.
     figsize : tuple(float, float)
         Figure size.
-    output : str
+    output : str, None
         Output filename for the plot. The plot is shown in an
         interface window if the argument is set to ``None``.
 
     Returns
     -------
-    NoneType
-        None
+    matplotlib.figure.Figure
+        The ``Figure`` object that can be used for further
+        customization of the plot.
     """
 
     if output is None:
         print("Plotting empirical spectra comparison...", end="")
     else:
         print(f"Plotting empirical spectra comparison: {output}...", end="")
 
@@ -278,21 +283,19 @@
 
     rad_vel = np.array(h5_file[f"results/empirical/{tag}/rad_vel"])
     rad_vel *= 1e3  # (m s-1)
 
     if n_spectra is None:
         n_spectra = names.size
 
-    mpl.rcParams["font.family"] = "serif"
-    mpl.rcParams["mathtext.fontset"] = "dejavuserif"
-
-    plt.rc("axes", edgecolor="black", linewidth=2.2)
+    plt.rcParams["font.family"] = "serif"
+    plt.rcParams["mathtext.fontset"] = "dejavuserif"
     plt.rcParams["axes.axisbelow"] = False
 
-    plt.figure(1, figsize=figsize)
+    fig = plt.figure(figsize=figsize)
     gridsp = mpl.gridspec.GridSpec(1, 1)
     gridsp.update(wspace=0, hspace=0, left=0, right=1, bottom=0, top=1)
 
     ax = plt.subplot(gridsp[0, 0])
 
     ax.tick_params(
         axis="both",
@@ -434,61 +437,69 @@
             )
 
     if output is None:
         plt.show()
     else:
         plt.savefig(output, bbox_inches="tight")
 
-    plt.clf()
-    plt.close()
-
     h5_file.close()
 
     print(" [DONE]")
 
+    return fig
+
 
 @typechecked
 def plot_grid_statistic(
     tag: str,
     upsample: bool = False,
     xlim: Optional[Tuple[float, float]] = None,
     ylim: Optional[Tuple[float, float]] = None,
     title: Optional[str] = None,
     offset: Optional[Tuple[float, float]] = None,
     figsize: Optional[Tuple[float, float]] = (4.0, 2.5),
-    output: Optional[str] = "grid_statistic.pdf",
-):
+    output: Optional[str] = None,
+    nlevels_main: int = 20,
+    nlevels_extra: int = 10,
+) -> mpl.figure.Figure:
     """
-    Function for plotting the results from the empirical spectrum comparison.
+    Function for plotting the results from the comparison with
+    a grid of empirical or model spectra
 
     Parameters
     ----------
     tag : str
-        Database tag where the results from the empirical comparison with
-        :class:`~species.analysis.empirical.CompareSpectra.spectral_type` are stored.
+        Database tag where the results from the comparison with
+        :class:`~species.analysis.empirical.CompareSpectra` are stored.
     upsample : bool
-        Upsample the goodness-of-fit grid to a higher resolution for a smoother appearance.
-    xlim : tuple(float, float)
-        Limits of the spectral type axis.
-    ylim : tuple(float, float)
-        Limits of the goodness-of-fit axis.
-    title : str
-        Plot title.
-    offset : tuple(float, float)
-        Offset for the label of the x- and y-axis.
-    figsize : tuple(float, float)
+        Upsample the goodness-of-fit grid to a higher resolution
+        for a smoother appearance.
+    xlim : tuple(float, float), None
+        Limits of the x-axis (spectral type or effective temperature).
+    ylim : tuple(float, float), None
+        Limits of the y-axis.
+    title : str, None
+        Title that is shown above the plot.
+    offset : tuple(float, float), None
+        Offset for the label for the x- and y-axis.
+    figsize : tuple(float, float), None
         Figure size.
-    output : str
+    output : str, None
         Output filename for the plot. The plot is shown in an
         interface window if the argument is set to ``None``.
+    nlevels_main : int
+        Number of contour levels for the main plot.
+    nlevels_extra : int
+        Number of contour levels for the optional extra parameter.
 
     Returns
     -------
-    NoneType
-        None
+    matplotlib.figure.Figure
+        The ``Figure`` object that can be used for further
+        customization of the plot.
     """
 
     if output is None:
         print("Plotting goodness-of-fit of model grid...", end="")
     else:
         print(f"Plotting goodness-of-fit of model grid: {output}...", end="")
 
@@ -526,29 +537,28 @@
     for i in range(n_param):
         model_param.append(dset.attrs[f"parameter{i}"])
         coord_points.append(
             np.array(h5_file[f"results/comparison/{tag}/coord_points{i}"])
         )
 
     coord_x = coord_points[0]
+    coord_y = None
+    param_y = None
 
-    if len(coord_points[1]) > 1:
-        coord_y = coord_points[1]
-    elif len(coord_points[2]) > 1:
-        coord_y = coord_points[2]
-    else:
-        coord_y = None
-
-    mpl.rcParams["font.family"] = "serif"
-    mpl.rcParams["mathtext.fontset"] = "dejavuserif"
+    for i, item in enumerate(coord_points[1:]):
+        if len(item) > 1:
+            coord_y = item
+            param_y = model_param[i+1]
+            break
 
-    plt.rc("axes", edgecolor="black", linewidth=2.2)
+    plt.rcParams["font.family"] = "serif"
+    plt.rcParams["mathtext.fontset"] = "dejavuserif"
     plt.rcParams["axes.axisbelow"] = False
 
-    plt.figure(1, figsize=figsize)
+    fig = plt.figure(figsize=figsize)
 
     if coord_y is None:
         gridsp = mpl.gridspec.GridSpec(1, 1)
         gridsp.update(wspace=0, hspace=0, left=0, right=1, bottom=0, top=1)
 
         ax = plt.subplot(gridsp[0, 0])
 
@@ -590,25 +600,34 @@
         right=True,
         pad=5,
     )
 
     ax.xaxis.set_minor_locator(AutoMinorLocator(5))
     ax.yaxis.set_minor_locator(AutoMinorLocator(5))
 
-    ax.set_xlabel(r"T$_\mathregular{eff}$ (K)", fontsize=13.0)
-
-    if coord_y is None:
-        ax.set_ylabel(r"$\Delta\mathregular{log}\,\mathregular{G}$", fontsize=13.0)
+    ax.set_xlabel(r"$T_\mathregular{eff}$ (K)", fontsize=13.0)
 
-    elif len(coord_points[1]) > 1:
-        ax.set_ylabel(r"$\mathregular{log}\,\mathregular{g}$", fontsize=13.0)
+    if param_y is None:
+        ax.set_ylabel(r"$\Delta\mathregular{log}\,G$", fontsize=13.0)
 
-    elif len(coord_points[2]) > 1:
+    elif param_y == "ism_ext":
         ax.set_ylabel(r"$\mathregular{A}_\mathregular{V}$", fontsize=13.0)
 
+    elif param_y == "logg":
+        ax.set_ylabel(r"$\mathregular{log}\,g$", fontsize=13.0)
+
+    elif param_y == "feh":
+        ax.set_ylabel("[Fe/H]", fontsize=13.0)
+
+    elif param_y == "c_o_ratio":
+        ax.set_ylabel("C/O", fontsize=13.0)
+
+    elif param_y == "fsed":
+        ax.set_ylabel(r"$f_\mathregular{sed}$", fontsize=13.0)
+
     if xlim is not None:
         ax.set_xlim(xlim[0], xlim[1])
 
     if ylim is not None:
         ax.set_ylim(ylim[0], ylim[1])
 
     if offset is not None:
@@ -618,36 +637,71 @@
     else:
         ax.get_xaxis().set_label_coords(0.5, -0.11)
         ax.get_yaxis().set_label_coords(-0.1, 0.5)
 
     if title is not None:
         ax.set_title(title, y=1.02, fontsize=14.0)
 
-    # Sum/collapse over log(g) if it contains a single value
-    if len(coord_points[1]) == 1:
-        goodness_fit = np.sum(goodness_fit, axis=1)
+    # Sum/collapse over parameters with a single value
+    for i, item in enumerate(coord_points):
+        if len(item) == 1:
+            goodness_fit = np.sum(goodness_fit, axis=i)
 
     # Indices of the best-fit model
     best_index = np.unravel_index(goodness_fit.argmin(), goodness_fit.shape)
 
-    # Make Teff the x axis and log(g) the y axis
-    goodness_fit = np.transpose(goodness_fit)
+    extra_param = None
+
+    if len(model_param) > 2:
+        n_collapse = len(coord_points) - 3
+
+        if "ism_ext" in model_param:
+            extra_param = "ism_ext"
+            extra_idx = model_param.index("ism_ext")
+
+            if extra_idx != 2:
+                goodness_fit = np.swapaxes(goodness_fit, extra_idx, 2)
+                coord_points = [coord_points[0], coord_points[1], coord_points[extra_idx]]
+                extra_idx = 2
 
-    if len(coord_points[1]) > 1 and len(coord_points[2]) > 1:
-        # Indices with the minimum G_k for the tested A_V values
-        indices = np.argmin(goodness_fit, axis=0)
+        else:
+            extra_param = model_param[2]
+            extra_idx = 2
+
+        if len(model_param) > 3:
+            # Select minimum G_k for tested A_V values
+            axis = []
+            for i in range(n_collapse):
+                axis.append(3+i)
+
+            goodness_fit = np.amin(goodness_fit, axis=tuple(axis))
+
+        # Indices with the minimum G_k for the tested
+        # values of A_V or the 3rd axis otherwise
+        indices = np.argmin(goodness_fit, axis=extra_idx)
 
         # Select minimum G_k for tested A_V values
-        goodness_fit = np.amin(goodness_fit, axis=0)
+        # or the values of the 3rd otherwise
+        goodness_fit = np.amin(goodness_fit, axis=extra_idx)
 
         extra_map = np.zeros(goodness_fit.shape)
 
         for i in range(extra_map.shape[0]):
             for j in range(extra_map.shape[1]):
-                extra_map[i, j] = coord_points[2][indices[i, j]]
+                extra_map[i, j] = coord_points[extra_idx][indices[i, j]]
+
+    else:
+        extra_map = None
+
+    # Transpose for plot so make Teff the x axis
+
+    goodness_fit = np.transpose(goodness_fit)
+
+    if extra_map is not None:
+        extra_map = np.transpose(extra_map)
 
     if coord_y is not None:
         if upsample:
             fit_interp = RegularGridInterpolator((coord_y, coord_x), goodness_fit)
 
             x_new = np.linspace(coord_x[0], coord_x[-1], 50)
             y_new = np.linspace(coord_y[0], coord_y[-1], 50)
@@ -667,15 +721,15 @@
             coord_x,
             goodness_fit[
                 0,
             ],
         )
 
     else:
-        c = ax.contourf(x_grid, y_grid, goodness_fit, levels=20)
+        c = ax.contourf(x_grid, y_grid, goodness_fit, levels=nlevels_main)
 
         cb = mpl.colorbar.Colorbar(
             ax=ax_cb,
             mappable=c,
             orientation="vertical",
             ticklocation="right",
             format="%.1f",
@@ -704,42 +758,42 @@
         cb.ax.set_ylabel(
             r"$\Delta\mathregular{log}\,\mathregular{G}$",
             rotation=270,
             labelpad=22,
             fontsize=13.0,
         )
 
-        if len(coord_points[1]) > 1 and len(coord_points[2]) > 1:
+        if extra_map is not None:
             if upsample:
                 extra_interp = RegularGridInterpolator((coord_y, coord_x), extra_map)
                 extra_map = extra_interp((y_grid, x_grid))
 
                 cs = ax.contour(
-                    x_grid, y_grid, extra_map, levels=10, colors="white", linewidths=0.7
+                    x_grid, y_grid, extra_map, levels=nlevels_extra, colors="white", linewidths=0.7
                 )
 
             else:
                 cs = ax.contour(
                     coord_x,
                     coord_y,
                     extra_map,
-                    levels=10,
+                    levels=nlevels_extra,
                     colors="white",
                     linewidths=0.7,
                 )
 
             # manual = [(2350, 0.8), (2500, 0.8), (2600, 0.8), (2700, 0.8),
             #           (2800, 0.8), (2950, 0.8), (3100, 0.8), (3300, 0.8)]
 
             ax.clabel(cs, cs.levels, inline=True, fontsize=8, fmt="%1.1f")
 
         # if extra_scaling is not None and len(coord_points[2]) > 1:
         #     ratio = np.transpose(flux_scaling[:, 0, :])/np.transpose(extra_scaling[:, 0, :, 0])
         #
-        #     cs = ax.contour(coord_x, coord_y, ratio, levels=10, colors='white',
+        #     cs = ax.contour(coord_x, coord_y, ratio, levels=nlevels_extra, colors='white',
         #                     linestyles='-', linewidths=0.7)
         #
         #     ax.clabel(cs, cs.levels, inline=True, fontsize=8, fmt='%1.1f')
 
         ax.plot(
             coord_x[best_index[0]],
             coord_y[best_index[1]],
@@ -756,18 +810,22 @@
         #
         # par_text = f'{par_label[0]} = {best_param[0]:.0f} {par_unit[0]}\n' \
         #            f'{par_label[1]} = {best_param[1]:.1f}'
         #
         # ax.annotate(par_text, (best_param[0]+50., best_param[1]), ha='left', va='center',
         #             color='white', fontsize=12.)
 
+    if extra_param is not None:
+        extra_label = plot_util.update_labels([extra_param])[0]
+        ax.plot([], [], ls='-', lw=1.2, color='white', label=extra_label)
+        ax.legend(loc='best', frameon=False, labelcolor='linecolor', fontsize=12.)
+
     if output is None:
         plt.show()
     else:
         plt.savefig(output, bbox_inches="tight")
 
-    plt.clf()
-    plt.close()
-
     h5_file.close()
 
     print(" [DONE]")
+
+    return fig
```

### Comparing `species-0.5.5/species/plot/plot_mcmc.py` & `species-0.6.0/species/plot/plot_mcmc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """
 Module for plotting MCMC results.
 """
 
-import os
 import warnings
 
 from typing import List, Optional, Tuple, Union
 
 import h5py
 import corner
 import numpy as np
@@ -23,48 +22,47 @@
 
 
 @typechecked
 def plot_walkers(
     tag: str,
     nsteps: Optional[int] = None,
     offset: Optional[Tuple[float, float]] = None,
-    output: Optional[str] = "walkers.pdf",
-) -> None:
+    output: Optional[str] = None,
+) -> mpl.figure.Figure:
     """
     Function to plot the step history of the walkers.
 
     Parameters
     ----------
     tag : str
         Database tag with the samples.
     nsteps : int, None
         Number of steps that are plotted. All steps are
         plotted if the argument is set to ``None``.
     offset : tuple(float, float), None
         Offset of the x- and y-axis label. Default values
         are used if the arguments is set to ``None``.
-    output : str
+    output : str, None
         Output filename for the plot. The plot is shown in an
         interface window if the argument is set to ``None``.
 
     Returns
     -------
-    NoneType
-        None
+    matplotlib.figure.Figure
+        The ``Figure`` object that can be used for further
+        customization of the plot.
     """
 
     if output is None:
         print("Plotting walkers...", end="", flush=True)
     else:
         print(f"Plotting walkers: {output}...", end="", flush=True)
 
-    mpl.rcParams["font.family"] = "serif"
-    mpl.rcParams["mathtext.fontset"] = "dejavuserif"
-
-    plt.rc("axes", edgecolor="black", linewidth=2.2)
+    plt.rcParams["font.family"] = "serif"
+    plt.rcParams["mathtext.fontset"] = "dejavuserif"
 
     species_db = database.Database()
     box = species_db.get_samples(tag)
 
     samples = box.samples
     labels = plot_util.update_labels(box.parameters)
 
@@ -75,15 +73,15 @@
             f"The plot_walkers function can only be used after "
             "running the MCMC with run_mcmc and not after "
             f"running run_ultranest or run_multinest."
         )
 
     ndim = samples.shape[-1]
 
-    plt.figure(1, figsize=(6, ndim * 1.5))
+    fig = plt.figure(figsize=(6, ndim * 1.5))
     gridsp = mpl.gridspec.GridSpec(ndim, 1)
     gridsp.update(wspace=0, hspace=0.1, left=0, right=1, bottom=0, top=1)
 
     for i in range(ndim):
         ax = plt.subplot(gridsp[i, 0])
 
         if i == ndim - 1:
@@ -174,19 +172,18 @@
             ax.plot(samples[j, :, i], ls="-", lw=0.5, color="black", alpha=0.5)
 
     if output is None:
         plt.show()
     else:
         plt.savefig(output, bbox_inches="tight")
 
-    plt.clf()
-    plt.close()
-
     print(" [DONE]")
 
+    return fig
+
 
 @typechecked
 def plot_posterior(
     tag: str,
     burnin: Optional[int] = None,
     title: Optional[str] = None,
     offset: Optional[Tuple[float, float]] = None,
@@ -195,18 +192,18 @@
     max_prob: bool = False,
     vmr: bool = False,
     inc_luminosity: bool = False,
     inc_mass: bool = False,
     inc_log_mass: bool = False,
     inc_pt_param: bool = False,
     inc_loglike: bool = False,
-    output: Optional[str] = "posterior.pdf",
+    output: Optional[str] = None,
     object_type: str = "planet",
     param_inc: Optional[List[str]] = None,
-) -> None:
+) -> mpl.figure.Figure:
     """
     Function to plot the posterior distribution
     of the fitted parameters.
 
     Parameters
     ----------
     tag : str
@@ -248,37 +245,36 @@
     inc_pt_param : bool
         Include the parameters of the pressure-temperature profile.
         Only used if the ``tag`` contains samples obtained with
         :class:`~species.analysis.retrieval.AtmosphericRetrieval`.
     inc_loglike : bool
         Include the log10 of the likelihood as additional
         parameter in the corner plot.
-    output : str
+    output : str, None
         Output filename for the plot. The plot is shown in an
         interface window if the argument is set to ``None``.
     object_type : str
         Object type ('planet' or 'star'). With 'planet', the radius
         and mass are expressed in Jupiter units. With 'star', the
         radius and mass are expressed in solar units.
     param_inc : list(str), None
         List with subset of parameters that will be included in the
         posterior plot. This parameter can also be used to change the
         order of the parameters in the posterior plot. All parameters
         will be included if the argument is set to ``None``.
 
     Returns
     -------
-    NoneType
-        None
+    matplotlib.figure.Figure
+        The ``Figure`` object that can be used for further
+        customization of the plot.
     """
 
-    mpl.rcParams["font.family"] = "serif"
-    mpl.rcParams["mathtext.fontset"] = "dejavuserif"
-
-    plt.rc("axes", edgecolor="black", linewidth=2.2)
+    plt.rcParams["font.family"] = "serif"
+    plt.rcParams["mathtext.fontset"] = "dejavuserif"
 
     if burnin is None:
         burnin = 0
 
     species_db = database.Database()
 
     box = species_db.get_samples(tag, burnin=burnin)
@@ -491,17 +487,15 @@
 
                     # Overwrite the sample with the log10 number fraction
                     samples_item[param_index] = np.log10(
                         10.0 ** samples_item[param_index] * mmw / masses[param_item]
                     )
 
             # Store the updated sample to the array
-            updated_samples[
-                i,
-            ] = samples_item
+            updated_samples[i,] = samples_item
 
         # Overwrite the samples in the SamplesBox
         box.samples = updated_samples
 
     print("Median sample:")
     for key, value in box.median_sample.items():
         print(f"   - {key} = {value:.2e}")
@@ -703,48 +697,49 @@
             )
 
     # Change from Jupiter to solar units if star
 
     if "radius" in box.parameters:
         radius_index = np.argwhere(np.array(box.parameters) == "radius")[0]
         if object_type == "star":
-            samples[:, radius_index] *= constants.R_JUP/constants.R_SUN
+            samples[:, radius_index] *= constants.R_JUP / constants.R_SUN
 
     if "mass" in box.parameters:
         mass_index = np.argwhere(np.array(box.parameters) == "mass")[0]
         if object_type == "star":
-            samples[:, mass_index] *= constants.M_JUP/constants.M_SUN
+            samples[:, mass_index] *= constants.M_JUP / constants.M_SUN
 
     if "log_mass" in box.parameters:
         mass_index = np.argwhere(np.array(box.parameters) == "log_mass")[0]
         if object_type == "star":
-            samples[:, mass_index] = np.log10(10.**samples[:, mass_index]*constants.M_JUP/constants.M_SUN)
+            samples[:, mass_index] = np.log10(
+                10.0 ** samples[:, mass_index] * constants.M_JUP / constants.M_SUN
+            )
 
     if inc_loglike:
         # Get ln(L) of the samples
         ln_prob = box.ln_prob[..., np.newaxis]
 
         # Normalized by the maximum ln(L)
         ln_prob -= np.amax(ln_prob)
 
         # Convert ln(L) to log10(L)
         log_prob = ln_prob * np.exp(1.0)
 
         # Convert log10(L) to L
-        prob = 10.0 ** log_prob
+        prob = 10.0**log_prob
 
         # Normalize to an integrated probability of 1
         prob /= np.sum(prob)
 
         samples = np.append(samples, np.log10(prob), axis=-1)
         box.parameters.append("log_prob")
         ndim += 1
 
-    labels = plot_util.update_labels(
-        box.parameters, object_type=object_type)
+    labels = plot_util.update_labels(box.parameters, object_type=object_type)
 
     # Check if parameter values were fixed
 
     index_sel = []
     index_del = []
 
     for i in range(ndim):
@@ -776,15 +771,15 @@
         if unit_start == -1:
             param_label = item
             unit_label = None
 
         else:
             param_label = item[:unit_start]
             # Remove parenthesis from the units
-            unit_label = item[unit_start + 1: -1]
+            unit_label = item[unit_start + 1 : -1]
 
         q_16, q_50, q_84 = corner.quantile(samples[:, i], [0.16, 0.5, 0.84])
         q_minus, q_plus = q_50 - q_16, q_84 - q_50
 
         if isinstance(title_fmt, str):
             fmt = "{{0:{0}}}".format(title_fmt).format
 
@@ -890,28 +885,27 @@
         fig.suptitle(title, y=1.02, fontsize=16)
 
     if output is None:
         plt.show()
     else:
         plt.savefig(output, bbox_inches="tight")
 
-    plt.clf()
-    plt.close()
-
     print(" [DONE]")
 
+    return fig
+
 
 @typechecked
 def plot_mag_posterior(
     tag: str,
     filter_name: str,
     burnin: int = None,
     xlim: Tuple[float, float] = None,
-    output: Optional[str] = "mag_posterior.pdf",
-) -> np.ndarray:
+    output: Optional[str] = None,
+) -> Tuple[np.ndarray, mpl.figure.Figure]:
     """
     Function to plot the posterior distribution of the synthetic
     magnitudes. The posterior samples are also returned.
 
     Parameters
     ----------
     tag : str
@@ -920,28 +914,29 @@
         Filter name.
     burnin : int, None
         Number of burnin steps to exclude. All samples are
         used if the argument is set to ``None``.
     xlim : tuple(float, float), None
         Axis limits. Automatically set if the argument is
         set to ``None``.
-    output : str
+    output : str, None
         Output filename for the plot. The plot is shown in an
         interface window if the argument is set to ``None``.
 
     Returns
     -------
     np.ndarray
         Array with the posterior samples of the magnitude.
+    matplotlib.figure.Figure
+        The ``Figure`` object that can be used for further
+        customization of the plot.
     """
 
-    mpl.rcParams["font.family"] = "serif"
-    mpl.rcParams["mathtext.fontset"] = "dejavuserif"
-
-    plt.rc("axes", edgecolor="black", linewidth=2.2)
+    plt.rcParams["font.family"] = "serif"
+    plt.rcParams["mathtext.fontset"] = "dejavuserif"
 
     species_db = database.Database()
 
     samples = species_db.get_mcmc_photometry(tag, filter_name, burnin)
 
     if output is None:
         print("Plotting photometry samples...", end="", flush=True)
@@ -998,30 +993,27 @@
     ax.get_xaxis().set_label_coords(0.5, -0.26)
 
     if output is None:
         plt.show()
     else:
         plt.savefig(output, bbox_inches="tight")
 
-    plt.clf()
-    plt.close()
-
     print(" [DONE]")
 
-    return samples
+    return samples, fig
 
 
 @typechecked
 def plot_size_distributions(
     tag: str,
     burnin: Optional[int] = None,
     random: Optional[int] = None,
     offset: Optional[Tuple[float, float]] = None,
-    output: Optional[str] = "size_distributions.pdf",
-) -> None:
+    output: Optional[str] = None,
+) -> mpl.figure.Figure:
     """
     Function to plot random samples of the log-normal
     or power-law size distributions.
 
     Parameters
     ----------
     tag : str
@@ -1032,53 +1024,50 @@
         with :func:`~species.analysis.fit_model.FitModel.run_mcmc`.
     random : int, None
         Number of randomly selected samples. All samples are used
         if the argument set to ``None``.
     offset : tuple(float, float), None
         Offset of the x- and y-axis label. Default values are used
         if the argument set to ``None``.
-    output : str
+    output : str, None
         Output filename for the plot. The plot is shown in an
         interface window if the argument is set to ``None``.
 
     Returns
     -------
-    NoneType
-        None
+    matplotlib.figure.Figure
+        The ``Figure`` object that can be used for further
+        customization of the plot.
     """
 
     if output is None:
         print("Plotting size distributions...", end="", flush=True)
     else:
         print(f"Plotting size distributions: {output}...", end="", flush=True)
 
     if burnin is None:
         burnin = 0
 
-    mpl.rcParams["font.family"] = "serif"
-    mpl.rcParams["mathtext.fontset"] = "dejavuserif"
-
-    plt.rc("axes", edgecolor="black", linewidth=2.2)
+    plt.rcParams["font.family"] = "serif"
+    plt.rcParams["mathtext.fontset"] = "dejavuserif"
 
     species_db = database.Database()
     box = species_db.get_samples(tag)
 
     if "lognorm_radius" not in box.parameters and "powerlaw_max" not in box.parameters:
         raise ValueError(
             "The SamplesBox does not contain extinction parameter for a log-normal "
             "or power-law size distribution."
         )
 
     samples = box.samples
 
     if samples.ndim == 2 and random is not None:
         ran_index = np.random.randint(samples.shape[0], size=random)
-        samples = samples[
-            ran_index,
-        ]
+        samples = samples[ran_index,]
 
     elif samples.ndim == 3:
         if burnin > samples.shape[1]:
             raise ValueError(
                 f"The 'burnin' value is larger than the number of steps "
                 f"({samples.shape[1]}) that are made by the walkers."
             )
@@ -1099,15 +1088,15 @@
     if "powerlaw_max" in box.parameters:
         r_max_index = box.parameters.index("powerlaw_max")
         exponent_index = box.parameters.index("powerlaw_exp")
 
         r_max = samples[:, r_max_index]
         exponent = samples[:, exponent_index]
 
-    plt.figure(1, figsize=(6, 3))
+    fig = plt.figure(figsize=(6, 3))
     gridsp = mpl.gridspec.GridSpec(1, 1)
     gridsp.update(wspace=0, hspace=0, left=0, right=1, bottom=0, top=1)
 
     ax = plt.subplot(gridsp[0, 0])
 
     ax.tick_params(
         axis="both",
@@ -1178,31 +1167,30 @@
         ax.plot(radii, dn_grains / r_width, ls="-", lw=0.5, color="black", alpha=0.5)
 
     if output is None:
         plt.show()
     else:
         plt.savefig(output, bbox_inches="tight")
 
-    plt.clf()
-    plt.close()
-
     print(" [DONE]")
 
+    return fig
+
 
 @typechecked
 def plot_extinction(
     tag: str,
     burnin: Optional[int] = None,
     random: Optional[int] = None,
     wavel_range: Optional[Tuple[float, float]] = None,
     xlim: Optional[Tuple[float, float]] = None,
     ylim: Optional[Tuple[float, float]] = None,
     offset: Optional[Tuple[float, float]] = None,
-    output: Optional[str] = "extinction.pdf",
-) -> None:
+    output: Optional[str] = None,
+) -> mpl.figure.Figure:
     """
     Function to plot random samples of the extinction, either from
     fitting a size distribution of enstatite grains (``dust_radius``,
     ``dust_sigma``, and ``dust_ext``), or from fitting ISM extinction
     (``ism_ext`` and optionally ``ism_red``).
 
     Parameters
@@ -1225,60 +1213,57 @@
         if the argument is set to ``None``.
     ylim : tuple(float, float)
         Limits of the extinction axis. The range is set automatically
         if the argument is set to ``None``.
     offset : tuple(float, float), None
         Offset of the x- and y-axis label. Default values are used
         if the argument is set to ``None``.
-    output : str
+    output : str, None
         Output filename for the plot. The plot is shown in an
         interface window if the argument is set to ``None``.
 
     Returns
     -------
-    NoneType
-        None
+    matplotlib.figure.Figure
+        The ``Figure`` object that can be used for further
+        customization of the plot.
     """
 
     if burnin is None:
         burnin = 0
 
     if wavel_range is None:
         wavel_range = (0.4, 10.0)
 
-    mpl.rcParams["font.family"] = "serif"
-    mpl.rcParams["mathtext.fontset"] = "dejavuserif"
-
-    plt.rc("axes", edgecolor="black", linewidth=2.2)
+    plt.rcParams["font.family"] = "serif"
+    plt.rcParams["mathtext.fontset"] = "dejavuserif"
 
     species_db = database.Database()
     box = species_db.get_samples(tag)
 
     samples = box.samples
 
     if samples.ndim == 2 and random is not None:
         ran_index = np.random.randint(samples.shape[0], size=random)
-        samples = samples[
-            ran_index,
-        ]
+        samples = samples[ran_index,]
 
     elif samples.ndim == 3:
         if burnin > samples.shape[1]:
             raise ValueError(
                 f"The 'burnin' value is larger than the number of steps "
                 f"({samples.shape[1]}) that are made by the walkers."
             )
 
         samples = samples[:, burnin:, :]
 
         ran_walker = np.random.randint(samples.shape[0], size=random)
         ran_step = np.random.randint(samples.shape[1], size=random)
         samples = samples[ran_walker, ran_step, :]
 
-    plt.figure(1, figsize=(6, 3))
+    fig = plt.figure(figsize=(6, 3))
     gridsp = mpl.gridspec.GridSpec(1, 1)
     gridsp.update(wspace=0, hspace=0, left=0, right=1, bottom=0, top=1)
 
     ax = plt.subplot(gridsp[0, 0])
 
     ax.tick_params(
         axis="both",
@@ -1332,15 +1317,14 @@
     sample_wavel = np.linspace(wavel_range[0], wavel_range[1], 100)
 
     if (
         "lognorm_radius" in box.parameters
         and "lognorm_sigma" in box.parameters
         and "lognorm_ext" in box.parameters
     ):
-
         cross_optical, dust_radius, dust_sigma = dust_util.interp_lognorm([], [], None)
 
         log_r_index = box.parameters.index("lognorm_radius")
         sigma_index = box.parameters.index("lognorm_sigma")
         ext_index = box.parameters.index("lognorm_ext")
 
         log_r_g = samples[:, log_r_index]
@@ -1378,15 +1362,14 @@
             ax.plot(sample_wavel, sample_ext, ls="-", lw=0.5, color="black", alpha=0.5)
 
     elif (
         "powerlaw_max" in box.parameters
         and "powerlaw_exp" in box.parameters
         and "powerlaw_ext" in box.parameters
     ):
-
         cross_optical, dust_max, dust_exp = dust_util.interp_powerlaw([], [], None)
 
         r_max_index = box.parameters.index("powerlaw_max")
         exp_index = box.parameters.index("powerlaw_exp")
         ext_index = box.parameters.index("powerlaw_ext")
 
         r_max = samples[:, r_max_index]
@@ -1420,15 +1403,14 @@
                 sample_cross[j] = cross_interp((item, 10.0 ** r_max[i], exponent[i]))
 
             sample_ext = 2.5 * np.log10(np.exp(1.0)) * sample_cross * n_grains
 
             ax.plot(sample_wavel, sample_ext, ls="-", lw=0.5, color="black", alpha=0.5)
 
     elif "ism_ext" in box.parameters:
-
         ext_index = box.parameters.index("ism_ext")
         ism_ext = samples[:, ext_index]
 
         if "ism_red" in box.parameters:
             red_index = box.parameters.index("ism_red")
             ism_red = samples[:, red_index]
 
@@ -1450,11 +1432,10 @@
         print(f"Plotting extinction: {output}...", end="", flush=True)
 
     if output is None:
         plt.show()
     else:
         plt.savefig(output, bbox_inches="tight")
 
-    plt.clf()
-    plt.close()
-
     print(" [DONE]")
+
+    return fig
```

### Comparing `species-0.5.5/species/plot/plot_retrieval.py` & `species-0.6.0/species/plot/plot_retrieval.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 Module for plotting atmospheric retrieval results.
 """
 
 # import copy
-import os
 import sys
 import warnings
 
 from typing import Optional, Tuple
 
 import matplotlib as mpl
 import matplotlib.pyplot as plt
@@ -29,19 +28,19 @@
 def plot_pt_profile(
     tag: str,
     random: Optional[int] = 100,
     envelope: bool = False,
     xlim: Optional[Tuple[float, float]] = None,
     ylim: Optional[Tuple[float, float]] = None,
     offset: Optional[Tuple[float, float]] = None,
-    output: Optional[str] = "pt_profile.pdf",
+    output: Optional[str] = None,
     radtrans: Optional[read_radtrans.ReadRadtrans] = None,
     extra_axis: Optional[str] = None,
     rad_conv_bound: bool = False,
-) -> None:
+) -> mpl.figure.Figure:
     """
     Function to plot the posterior distribution.
 
     Parameters
     ----------
     tag : str
         Database tag with the posterior samples.
@@ -58,15 +57,15 @@
         set to ``None``.
     ylim : tuple(float, float), None
         Limits of the pressure axis. Default values are used if set
         to ``None``.
     offset : tuple(float, float), None
         Offset of the x- and y-axis label. Default values are used
         if set to ``None``.
-    output : str
+    output : str, None
         Output filename for the plot. The plot is shown in an
         interface window if the argument is set to ``None``.
     radtrans : read_radtrans.ReadRadtrans, None
         Instance of :class:`~species.read.read_radtrans.ReadRadtrans`.
         Not used if set to ``None``.
     extra_axis : str, None
         The quantify that is plotted at the top axis ('photosphere',
@@ -74,16 +73,17 @@
         to ``None``.
     rad_conv_bound : bool
         Plot the range of pressures (:math:`\\pm 1\\sigma`) of the
         radiative-convective boundary.
 
     Returns
     -------
-    NoneType
-        None
+    matplotlib.figure.Figure
+        The ``Figure`` object that can be used for further
+        customization of the plot.
     """
 
     if output is None:
         print("Plotting the P-T profiles...", end="", flush=True)
     else:
         print(f"Plotting the P-T profiles: {output}...", end="", flush=True)
 
@@ -114,20 +114,18 @@
             indices,
         ]
 
     param_index = {}
     for item in parameters:
         param_index[item] = np.argwhere(parameters == item)[0][0]
 
-    mpl.rcParams["font.family"] = "serif"
-    mpl.rcParams["mathtext.fontset"] = "dejavuserif"
-
-    plt.rc("axes", edgecolor="black", linewidth=2.5)
+    plt.rcParams["font.family"] = "serif"
+    plt.rcParams["mathtext.fontset"] = "dejavuserif"
 
-    plt.figure(1, figsize=(4.0, 5.0))
+    fig = plt.figure(figsize=(4.0, 5.0))
     gridsp = mpl.gridspec.GridSpec(1, 1)
     gridsp.update(wspace=0, hspace=0, left=0, right=1, bottom=0, top=1)
 
     ax = plt.subplot(gridsp[0, 0])
 
     ax.tick_params(
         axis="both",
@@ -756,27 +754,26 @@
             )
 
     if output is None:
         plt.show()
     else:
         plt.savefig(output, bbox_inches="tight")
 
-    plt.clf()
-    plt.close()
-
     print(" [DONE]")
 
+    return fig
+
 
 @typechecked
 def plot_opacities(
     tag: str,
     radtrans: read_radtrans.ReadRadtrans,
     offset: Optional[Tuple[float, float]] = None,
-    output: Optional[str] = "opacities.pdf",
-) -> None:
+    output: Optional[str] = None,
+) -> mpl.figure.Figure:
     """
     Function to plot the line and continuum opacity
     structure from the median posterior samples.
 
     Parameters
     ----------
     tag : str
@@ -789,33 +786,32 @@
         if set to ``None``.
     output : str, None
         Output filename for the plot. The plot is shown in an
         interface window if the argument is set to ``None``.
 
     Returns
     -------
-    NoneType
-        None
+    matplotlib.figure.Figure
+        The ``Figure`` object that can be used for further
+        customization of the plot.
     """
 
     if output is None:
         print("Plotting opacities...", end="", flush=True)
     else:
         print(f"Plotting opacities: {output}...", end="", flush=True)
 
     species_db = database.Database()
     box = species_db.get_samples(tag)
     median = box.median_sample
 
-    mpl.rcParams["font.family"] = "serif"
-    mpl.rcParams["mathtext.fontset"] = "dejavuserif"
+    plt.rcParams["font.family"] = "serif"
+    plt.rcParams["mathtext.fontset"] = "dejavuserif"
 
-    plt.rc("axes", edgecolor="black", linewidth=2.5)
-
-    plt.figure(1, figsize=(10.0, 6.0))
+    fig = plt.figure(figsize=(10.0, 6.0))
     gridsp = mpl.gridspec.GridSpec(2, 5, width_ratios=[4, 0.25, 1.5, 4, 0.25])
     gridsp.update(wspace=0.1, hspace=0.1, left=0, right=1, bottom=0, top=1)
 
     ax1 = plt.subplot(gridsp[0, 0])
     ax2 = plt.subplot(gridsp[1, 0])
     ax3 = plt.subplot(gridsp[0, 1])
     ax4 = plt.subplot(gridsp[1, 1])
@@ -1118,66 +1114,66 @@
     # ax1.yaxis.set_minor_locator(LogLocator(base=1.))
     # ax2.yaxis.set_minor_locator(LogLocator(base=1.))
     # ax3.yaxis.set_minor_locator(LogLocator(base=1.))
     # ax4.yaxis.set_minor_locator(LogLocator(base=1.))
 
     xx_grid, yy_grid = np.meshgrid(wavelength, 1e-6 * radtrans.rt_object.press)
 
-    fig = ax1.pcolormesh(
+    fig_1 = ax1.pcolormesh(
         xx_grid,
         yy_grid,
         np.transpose(opacity_line),
         cmap="viridis",
         shading="gouraud",
         norm=LogNorm(vmin=1e-6 * np.amax(opacity_line), vmax=np.amax(opacity_line)),
     )
 
-    cb = Colorbar(ax=ax3, mappable=fig, orientation="vertical", ticklocation="right")
+    cb = Colorbar(ax=ax3, mappable=fig_1, orientation="vertical", ticklocation="right")
     cb.ax.set_ylabel("Line opacity (cm$^2$/g)", rotation=270, labelpad=20, fontsize=11)
 
-    fig = ax2.pcolormesh(
+    fig_2 = ax2.pcolormesh(
         xx_grid,
         yy_grid,
         np.transpose(albedo),
         cmap="viridis",
         shading="gouraud",
         norm=LogNorm(vmin=1e-4 * np.amax(albedo), vmax=np.amax(albedo)),
     )
 
-    cb = Colorbar(ax=ax4, mappable=fig, orientation="vertical", ticklocation="right")
+    cb = Colorbar(ax=ax4, mappable=fig_2, orientation="vertical", ticklocation="right")
     cb.ax.set_ylabel("Single scattering albedo", rotation=270, labelpad=20, fontsize=11)
 
-    fig = ax5.pcolormesh(
+    fig_3 = ax5.pcolormesh(
         xx_grid,
         yy_grid,
         np.transpose(opacity_cont_abs),
         cmap="viridis",
         shading="gouraud",
         norm=LogNorm(
             vmin=1e-6 * np.amax(opacity_cont_abs), vmax=np.amax(opacity_cont_abs)
         ),
     )
 
-    cb = Colorbar(ax=ax7, mappable=fig, orientation="vertical", ticklocation="right")
+    cb = Colorbar(ax=ax7, mappable=fig_3, orientation="vertical", ticklocation="right")
     cb.ax.set_ylabel(
         "Continuum absorption (cm$^2$/g)", rotation=270, labelpad=20, fontsize=11
     )
 
-    fig = ax6.pcolormesh(
+    fig_4 = ax6.pcolormesh(
         xx_grid,
         yy_grid,
         np.transpose(opacity_cont_scat),
         cmap="viridis",
         shading="gouraud",
         norm=LogNorm(
             vmin=1e-6 * np.amax(opacity_cont_scat), vmax=np.amax(opacity_cont_scat)
         ),
     )
 
-    cb = Colorbar(ax=ax8, mappable=fig, orientation="vertical", ticklocation="right")
+    cb = Colorbar(ax=ax8, mappable=fig_4, orientation="vertical", ticklocation="right")
     cb.ax.set_ylabel(
         "Continuum scattering (cm$^2$/g)", rotation=270, labelpad=20, fontsize=11
     )
 
     ax1.set_ylabel("Pressure (bar)", fontsize=13)
 
     ax2.set_xlabel("Wavelength (\N{GREEK SMALL LETTER MU}m)", fontsize=13)
@@ -1245,51 +1241,53 @@
     ax8.set_yscale("log")
 
     if output is None:
         plt.show()
     else:
         plt.savefig(output, bbox_inches="tight")
 
-    plt.clf()
-    plt.close()
-
     print(" [DONE]")
 
+    return fig
+
 
 @typechecked
 def plot_clouds(
     tag: str,
     offset: Optional[Tuple[float, float]] = None,
-    output: Optional[str] = "clouds.pdf",
+    output: Optional[str] = None,
     radtrans: Optional[read_radtrans.ReadRadtrans] = None,
     composition: str = "MgSiO3",
-) -> None:
+) -> mpl.figure.Figure:
     """
     Function to plot the size distributions for a given cloud composition as function as pressure.
     The size distributions are calculated for the median sample by using the radius_g (as function
     of pressure) and sigma_g.
 
     Parameters
     ----------
     tag : str
         Database tag with the posterior samples.
     offset : tuple(float, float), None
-        Offset of the x- and y-axis label. Default values are used if set to ``None``.
-    output : str
+        Offset of the x- and y-axis label. Default values are
+        used if set to ``None``.
+    output : str, None
         Output filename for the plot. The plot is shown in an
         interface window if the argument is set to ``None``.
     radtrans : read_radtrans.ReadRadtrans, None
-        Instance of :class:`~species.read.read_radtrans.ReadRadtrans`. Not used if set to ``None``.
+        Instance of :class:`~species.read.read_radtrans.ReadRadtrans`.
+        Not used if set to ``None``.
     composition : str
         Cloud composition (e.g. 'MgSiO3', 'Fe', 'Al2O3', 'Na2S', 'KCl').
 
     Returns
     -------
-    NoneType
-        None
+    matplotlib.figure.Figure
+        The ``Figure`` object that can be used for
+        further customization of the plot.
     """
 
     species_db = database.Database()
     box = species_db.get_samples(tag)
     median = box.median_sample
 
     if (
@@ -1304,20 +1302,18 @@
         )
 
     if output is None:
         print(f"Plotting {composition} clouds...", end="", flush=True)
     else:
         print(f"Plotting {composition} clouds: {output}...", end="", flush=True)
 
-    mpl.rcParams["font.family"] = "serif"
-    mpl.rcParams["mathtext.fontset"] = "dejavuserif"
+    plt.rcParams["font.family"] = "serif"
+    plt.rcParams["mathtext.fontset"] = "dejavuserif"
 
-    plt.rc("axes", edgecolor="black", linewidth=2.5)
-
-    plt.figure(1, figsize=(4.0, 3.0))
+    fig = plt.figure(figsize=(4.0, 3.0))
     gridsp = mpl.gridspec.GridSpec(1, 2, width_ratios=[4, 0.25])
     gridsp.update(wspace=0.1, hspace=0.0, left=0, right=1, bottom=0, top=1)
 
     ax1 = plt.subplot(gridsp[0, 0])
     ax2 = plt.subplot(gridsp[0, 1])
 
     radtrans.get_model(median)
@@ -1396,24 +1392,24 @@
         bottom=True,
         left=True,
         right=True,
     )
 
     xx_grid, yy_grid = np.meshgrid(radii, 1e-6 * radtrans.rt_object.press)
 
-    fig = ax1.pcolormesh(
+    mesh_fig = ax1.pcolormesh(
         xx_grid,
         yy_grid,
         dn_dr,
         cmap="viridis",
         shading="auto",
         norm=LogNorm(vmin=1e-10 * np.amax(dn_dr), vmax=np.amax(dn_dr)),
     )
 
-    cb = Colorbar(ax=ax2, mappable=fig, orientation="vertical", ticklocation="right")
+    cb = Colorbar(ax=ax2, mappable=mesh_fig, orientation="vertical", ticklocation="right")
     cb.ax.set_ylabel("dn/dr", rotation=270, labelpad=20, fontsize=11)
 
     for item in radtrans.rt_object.press * 1e-6:  # (bar)
         ax1.axhline(item, ls="-", lw=0.1, color="white")
 
     for item in radtrans.rt_object.cloud_radii * 1e4:  # (um)
         ax1.axvline(item, ls="-", lw=0.1, color="white")
@@ -1450,11 +1446,10 @@
     ax2.set_yscale("log")
 
     if output is None:
         plt.show()
     else:
         plt.savefig(output, bbox_inches="tight")
 
-    plt.clf()
-    plt.close()
-
     print(" [DONE]")
+
+    return fig
```

### Comparing `species-0.5.5/species/plot/plot_spectrum.py` & `species-0.6.0/species/plot/plot_spectrum.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from typing import Optional, Union, Tuple, List
 
 import numpy as np
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 
 from typeguard import typechecked
-from matplotlib.ticker import AutoMinorLocator, ScalarFormatter
+from matplotlib.ticker import AutoMinorLocator, ScalarFormatter, MaxNLocator
 
 from species.core import box, constants
 from species.read import read_filter
 from species.util import plot_util
 
 
 @typechecked
@@ -41,19 +41,19 @@
             Tuple[float, float],
             List[Optional[Union[dict, str, Tuple[float, float]]]],
         ]
     ] = None,
     figsize: Optional[Tuple[float, float]] = (10.0, 5.0),
     object_type: str = "planet",
     quantity: str = "flux density",
-    output: Optional[str] = "spectrum.pdf",
+    output: Optional[str] = None,
     leg_param: Optional[List[str]] = None,
     grid_hspace: float = 0.1,
     inc_model_name: bool = False,
-):
+) -> mpl.figure.Figure:
     """
     Function for plotting a spectral energy distribution and combining
     various data such as spectra, photometric fluxes, model spectra,
     synthetic photometry, fit residuals, and filter profiles.
 
     Parameters
     ----------
@@ -130,15 +130,15 @@
     object_type : str
         Object type ('planet' or 'star'). With 'planet', the radius
         and mass are expressed in Jupiter units. With 'star', the
         radius and mass are expressed in solar units.
     quantity: str
         The quantity of the y-axis ('flux density', 'flux',
         or 'magnitude').
-    output : str
+    output : str, None
         Output filename for the plot. The plot is shown in an
         interface window if the argument is set to ``None``.
     leg_param : list(str), None
         List with the parameters to include in the legend of the
         model spectra. Apart from atmospheric parameters (e.g.
         'teff', 'logg', 'radius') also parameters such as 'mass'
         and 'luminosity' can be included. The default atmospheric
@@ -150,62 +150,61 @@
         value is set to 0.1.
     inc_model_name : bool
         Include the model name in the legend of any
         :class:`~species.core.box.ModelBox`.
 
     Returns
     -------
-    NoneType
-        None
+    matplotlib.figure.Figure
+        The ``Figure`` object that can be used for further
+        customization of the plot.
     """
 
-    mpl.rcParams["font.family"] = "serif"
-    mpl.rcParams["mathtext.fontset"] = "dejavuserif"
-
-    plt.rc("axes", edgecolor="black", linewidth=2.2)
+    plt.rcParams["font.family"] = "serif"
+    plt.rcParams["mathtext.fontset"] = "dejavuserif"
     plt.rcParams["axes.axisbelow"] = False
 
     if plot_kwargs is None:
         plot_kwargs = []
 
     elif plot_kwargs is not None and len(boxes) != len(plot_kwargs):
         raise ValueError(
             f"The number of 'boxes' ({len(boxes)}) should be equal to the "
             f"number of items in 'plot_kwargs' ({len(plot_kwargs)})."
         )
 
     if residuals is not None and filters is not None:
-        plt.figure(1, figsize=figsize)
+        fig = plt.figure(figsize=figsize)
         grid_sp = mpl.gridspec.GridSpec(3, 1, height_ratios=[1, 3, 1])
         grid_sp.update(wspace=0, hspace=grid_hspace, left=0, right=1, bottom=0, top=1)
 
         ax1 = plt.subplot(grid_sp[1, 0])
         ax2 = plt.subplot(grid_sp[0, 0])
         ax3 = plt.subplot(grid_sp[2, 0])
 
     elif residuals is not None:
-        plt.figure(1, figsize=figsize)
+        fig = plt.figure(figsize=figsize)
         grid_sp = mpl.gridspec.GridSpec(2, 1, height_ratios=[4, 1])
         grid_sp.update(wspace=0, hspace=grid_hspace, left=0, right=1, bottom=0, top=1)
 
         ax1 = plt.subplot(grid_sp[0, 0])
         ax2 = None
         ax3 = plt.subplot(grid_sp[1, 0])
 
     elif filters is not None:
-        plt.figure(1, figsize=figsize)
+        fig = plt.figure(figsize=figsize)
         grid_sp = mpl.gridspec.GridSpec(2, 1, height_ratios=[1, 4])
         grid_sp.update(wspace=0, hspace=grid_hspace, left=0, right=1, bottom=0, top=1)
 
         ax1 = plt.subplot(grid_sp[1, 0])
         ax2 = plt.subplot(grid_sp[0, 0])
         ax3 = None
 
     else:
-        plt.figure(1, figsize=figsize)
+        fig = plt.figure(figsize=figsize)
         grid_sp = mpl.gridspec.GridSpec(1, 1)
         grid_sp.update(wspace=0, hspace=grid_hspace, left=0, right=1, bottom=0, top=1)
 
         ax1 = plt.subplot(grid_sp[0, 0])
         ax2 = None
         ax3 = None
 
@@ -379,38 +378,62 @@
 
     else:
         if ylim:
             ax1.set_ylim(ylim[0], ylim[1])
 
             ylim = ax1.get_ylim()
 
-            exponent = math.floor(math.log10(ylim[1]))
-            scaling = 10.0**exponent
+            if scale[1] == "linear":
+                exponent = math.floor(math.log10(ylim[1]))
+                scaling = 10.0**exponent
+
+            else:
+                exponent = None
+                scaling = 1.0
 
             if quantity == "flux density":
-                ylabel = (
-                    r"$F_\lambda$ (10$^{" + str(exponent) + r"}$" +" W m$^{-2}$ \N{GREEK SMALL LETTER MU}m$^{-1}$)"
-                )
+                if exponent is None:
+                    ylabel = (
+                        r"$F_\lambda$ (W m$^{-2}$ "
+                        + "\N{GREEK SMALL LETTER MU}m$^{-1}$)"
+                    )
+
+                else:
+                    ylabel = (
+                        r"$F_\lambda$ (10$^{"
+                        + str(exponent)
+                        + r"}$"
+                        + " W m$^{-2}$ \N{GREEK SMALL LETTER MU}m$^{-1}$)"
+                    )
 
             elif quantity == "flux":
-                ylabel = (
-                    r"$\lambda$$F_\lambda$ (10$^{" + str(exponent) + r"}$ W m$^{-2}$)"
-                )
+                if exponent is None:
+                    ylabel = (
+                        r"$\lambda$$F_\lambda$ (W m$^{-2}$)"
+                    )
+
+                else:
+                    ylabel = (
+                        r"$\lambda$$F_\lambda$ (10$^{" + str(exponent) + r"}$ W m$^{-2}$)"
+                    )
 
             ax1.set_ylabel(ylabel, fontsize=11)
             ax1.set_ylim(ylim[0] / scaling, ylim[1] / scaling)
 
             if ylim[0] < 0.0:
                 ax1.axhline(
                     0.0, ls="--", lw=0.7, color="gray", dashes=(2, 4), zorder=0.5
                 )
 
         else:
             if quantity == "flux density":
-                ax1.set_ylabel(r"$F_\lambda$"+ " (W m$^{-2}$ \N{GREEK SMALL LETTER MU}m$^{-1}$)", fontsize=11)
+                ax1.set_ylabel(
+                    r"$F_\lambda$" + " (W m$^{-2}$ \N{GREEK SMALL LETTER MU}m$^{-1}$)",
+                    fontsize=11,
+                )
 
             elif quantity == "flux":
                 ax1.set_ylabel(r"$\lambda$$F_\lambda$ (W m$^{-2}$)", fontsize=11)
 
             scaling = 1.0
 
     xlim = ax1.get_xlim()
@@ -479,31 +502,29 @@
                         param=list(param.keys()), object_type=object_type
                     )
 
                     label = ""
                     # newline = False
 
                     for i, item in enumerate(par_key):
-
                         if item[:4] == "teff":
                             value = f"{param[item]:.0f}"
 
                         elif item in [
                             "logg",
                             "feh",
                             "metallicity",
+                            "fsed",
                             "lognorm_ext",
                             "powerlaw_ext",
                             "ism_ext",
                         ]:
-
                             value = f"{param[item]:.1f}"
 
                         elif item in ["co", "c_o_ratio"]:
-
                             value = f"{param[item]:.2f}"
 
                         elif item[:6] == "radius":
                             if object_type == "planet":
                                 value = f"{param[item]:.1f}"
 
                                 # if item == 'radius_1':
@@ -866,28 +887,26 @@
                         if quantity == "flux":
                             flux_scaling = wavelength
 
                         scale_tmp = flux_scaling / scaling
 
                         if isinstance(box_item.flux[item][0], np.ndarray):
                             for i in range(box_item.flux[item].shape[1]):
-
                                 plot_obj = ax1.errorbar(
                                     wavelength,
                                     scale_tmp * box_item.flux[item][0, i],
                                     xerr=fwhm / 2.0,
                                     yerr=scale_tmp * box_item.flux[item][1, i],
                                     marker="s",
                                     ms=5,
                                     zorder=3,
                                     color="black",
                                 )
 
                         else:
-
                             plot_obj = ax1.errorbar(
                                 wavelength,
                                 scale_tmp * box_item.flux[item][0],
                                 xerr=fwhm / 2.0,
                                 yerr=scale_tmp * box_item.flux[item][1],
                                 marker="s",
                                 ms=5,
@@ -958,28 +977,44 @@
                                     yerr=flux_scaling
                                     * box_item.flux[item][1]
                                     / scaling,
                                     **plot_kwargs[j][item],
                                 )
 
         elif isinstance(box_item, box.SynphotBox):
+            obj_index = None
+
             for i, find_item in enumerate(boxes):
                 if isinstance(find_item, box.ObjectBox):
                     obj_index = i
                     break
 
             for item in box_item.flux:
                 transmission = read_filter.ReadFilter(item)
                 wavelength = transmission.mean_wavelength()
                 fwhm = transmission.filter_fwhm()
 
                 if quantity == "flux":
                     flux_scaling = wavelength
 
-                if not plot_kwargs[obj_index] or item not in plot_kwargs[obj_index]:
+                if plot_kwargs[j] is not None and item in plot_kwargs[j]:
+                    kwargs_copy = plot_kwargs[j][item].copy()
+
+                    if "zorder" not in kwargs_copy:
+                        kwargs_copy["zorder"] = 4.0
+
+                    ax1.errorbar(
+                        wavelength,
+                        flux_scaling * box_item.flux[item] / scaling,
+                        xerr=fwhm / 2.0,
+                        yerr=None,
+                        **kwargs_copy,
+                    )
+
+                elif obj_index is None or not plot_kwargs[obj_index] or item not in plot_kwargs[obj_index]:
                     ax1.errorbar(
                         wavelength,
                         flux_scaling * box_item.flux[item] / scaling,
                         xerr=fwhm / 2.0,
                         yerr=None,
                         alpha=0.7,
                         marker="s",
@@ -1223,14 +1258,17 @@
 
         if ax2 is not None:
             ax2.xaxis.set_major_formatter(ScalarFormatter())
 
         if ax3 is not None:
             ax3.xaxis.set_major_formatter(ScalarFormatter())
 
+    # if scale[1] == "log":
+    #     ax1.yaxis.set_major_locator()
+
     # filters = ['Paranal/SPHERE.ZIMPOL_N_Ha',
     #            'MUSE/Hbeta',
     #            'ALMA/855']
     #
     # filters = ['Paranal/SPHERE.IRDIS_B_Y',
     #            'MKO/NSFCam.J',
     #            'Paranal/SPHERE.IRDIS_D_H23_2',
@@ -1281,11 +1319,10 @@
     # ax1.text(2.5, 1.28, 'VLT/SINFONI', ha='left', va='center', fontsize=8., color='darkgray')
 
     if output is None:
         plt.show()
     else:
         plt.savefig(output, bbox_inches="tight")
 
-    plt.clf()
-    plt.close()
-
     print(" [DONE]")
+
+    return fig
```

### Comparing `species-0.5.5/species/read/read_calibration.py` & `species-0.6.0/species/read/read_calibration.py`

 * *Files identical despite different names*

### Comparing `species-0.5.5/species/read/read_color.py` & `species-0.6.0/species/read/read_color.py`

 * *Files identical despite different names*

### Comparing `species-0.5.5/species/read/read_model.py` & `species-0.6.0/species/read/read_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 """
 
 import os
 import math
 import warnings
 import configparser
 
-from typing import Dict, List, Optional, Tuple
+from typing import Dict, List, Optional, Tuple, Union
 
 import h5py
 import spectres
 import numpy as np
 
+from PyAstronomy.pyasl import rotBroad, fastRotBroad
 from typeguard import typechecked
 from scipy.integrate import simps
 from scipy.interpolate import interp1d, interp2d, RegularGridInterpolator
 
 from species.analysis import photometry
 from species.core import box, constants
 from species.data import database
@@ -104,14 +105,15 @@
             "powerlaw_exp",
             "powerlaw_ext",
             "disk_teff",
             "disk_radius",
             "veil_a",
             "veil_b",
             "veil_ref",
+            "vsini",
         ]
 
         # Test if the spectra are present in the database
         self.open_database()
 
     @typechecked
     def open_database(self) -> h5py._hl.files.File:
@@ -135,18 +137,28 @@
 
         try:
             h5_file[f"models/{self.model}"]
 
         except KeyError:
             h5_file.close()
 
-            raise ValueError(
-                f"The '{self.model}' model spectra are not present in the database."
+            warnings.warn(
+                f"The '{self.model}' model spectra are not present "
+                "in the database. Will try to add the model grid. "
+                "If this does not work (e.g. currently without an "
+                "internet connection) then please use the "
+                "'add_model' method of 'Database' to add the "
+                "grid of spectra yourself."
             )
 
+            species_db = database.Database()
+            species_db.add_model(self.model)
+
+            h5_file = h5py.File(database_path, "r")
+
         return h5_file
 
     @typechecked
     def wavelength_points(
         self, hdf5_file: h5py._hl.files.File
     ) -> Tuple[np.ndarray, np.ndarray]:
         """
@@ -472,16 +484,16 @@
             for j in range(dust_sigma.shape[0]):
                 cross_interp = interp1d(
                     dust_wavel, dust_cross[:, i, j], kind="linear", bounds_error=True
                 )
 
                 cross_tmp = cross_interp(filt_trans[:, 0])
 
-                integral1 = np.trapz(filt_trans[:, 1] * cross_tmp, filt_trans[:, 0])
-                integral2 = np.trapz(filt_trans[:, 1], filt_trans[:, 0])
+                integral1 = np.trapz(filt_trans[:, 1] * cross_tmp, x=filt_trans[:, 0])
+                integral2 = np.trapz(filt_trans[:, 1], x=filt_trans[:, 0])
 
                 # Filter-weighted average of the extinction cross section
                 cross_phot[i, j] = integral1 / integral2
 
         cross_interp = interp2d(
             dust_sigma, dust_radius, cross_phot, kind="linear", bounds_error=True
         )
@@ -572,16 +584,16 @@
             for j in range(dust_exp.shape[0]):
                 cross_interp = interp1d(
                     dust_wavel, dust_cross[:, i, j], kind="linear", bounds_error=True
                 )
 
                 cross_tmp = cross_interp(filt_trans[:, 0])
 
-                integral1 = np.trapz(filt_trans[:, 1] * cross_tmp, filt_trans[:, 0])
-                integral2 = np.trapz(filt_trans[:, 1], filt_trans[:, 0])
+                integral1 = np.trapz(filt_trans[:, 1] * cross_tmp, x=filt_trans[:, 0])
+                integral2 = np.trapz(filt_trans[:, 1], x=filt_trans[:, 0])
 
                 # Filter-weighted average of the extinction cross section
                 cross_phot[i, j] = integral1 / integral2
 
         cross_interp = interp2d(
             dust_exp, dust_r_max, cross_phot, kind="linear", bounds_error=True
         )
@@ -630,14 +642,16 @@
     def get_model(
         self,
         model_param: Dict[str, float],
         spec_res: Optional[float] = None,
         wavel_resample: Optional[np.ndarray] = None,
         magnitude: bool = False,
         smooth: bool = False,
+        fast_rot_broad: bool = True,
+        ext_filter: Optional[str] = None,
     ) -> box.ModelBox:
         """
         Function for extracting a model spectrum by linearly
         interpolating the model grid.
 
         Parameters
         ----------
@@ -663,14 +677,31 @@
             Vega and return the magnitude instead of flux density.
         smooth : bool
             If ``True``, the spectrum is smoothed with a Gaussian
             kernel to the spectral resolution of ``spec_res``. This
             requires either a uniform spectral resolution of the input
             spectra (fast) or a uniform wavelength spacing of the input
             spectra (slow).
+        fast_rot_broad : bool
+            Apply fast algorithm for the rotational broadening if set
+            to ``True``, otherwise a slow but more accurate broadening
+            is applied if set to ``False``. The fast algorithm will
+            only provide an accurate broadening if the wavelength range
+            of the spectrum is somewhat narrow (e.g. only the :math:`K`
+            band). The argument is only used if the ``vsini`` parameter
+            is included in the ``model_param`` dictionary.
+        ext_filter : str, None
+            Filter that is associated with the (optional) extinction
+            parameter, ``ism_ext``. When the argument of ``ext_filter``
+            is set to ``None``, the extinction is defined in the visual
+            as usual (i.e. :math:`A_V`). By providing a filter name
+            from the `SVO Filter Profile Service <http://svo2.cab.
+            inta-csic.es/svo/theory/fps/>`_ as argument then the
+            extinction ``ism_ext`` is defined in that filter instead
+            of the $V$ band.
 
         Returns
         -------
         species.core.box.ModelBox
             Box with the model spectrum.
         """
 
@@ -702,15 +733,19 @@
                 )
 
         # Print a warning if redundant parameters are included in the dictionary
 
         ignore_param = []
 
         for key in model_param.keys():
-            if key not in self.get_parameters() and key not in self.extra_param:
+            if (
+                key not in self.get_parameters()
+                and key not in self.extra_param
+                and not key.startswith("phot_ext_")
+            ):
                 warnings.warn(
                     f"The '{key}' parameter is not required by "
                     f"'{self.model}' so the parameter will be "
                     f"ignored. The mandatory parameters are "
                     f"{self.get_parameters()}."
                 )
 
@@ -740,14 +775,23 @@
         ]
 
         parameters = []
         for item in check_param:
             if item in model_param and item not in ignore_param:
                 parameters.append(model_param[item])
 
+        # Check if the ext_filter should be adjusted
+        # to the name that is extracted from the
+        # phot_ext_{ext_filter} parameter
+
+        if ext_filter is None:
+            for param_item in model_param:
+                if param_item.startswith("phot_ext_"):
+                    ext_filter = param_item[9:]
+
         # Interpolate the spectrum from the grid
 
         flux = self.spectrum_interp(parameters)[0]
 
         # Add the radius to the parameter dictionary if the mass if given
 
         if "mass" in model_param and "radius" not in model_param:
@@ -808,14 +852,47 @@
             model=self.model,
             wavelength=self.wl_points,
             flux=flux,
             parameters=model_param,
             quantity="flux",
         )
 
+        # Apply rotational broadening vsin(i) in km/s
+
+        if "vsini" in model_param:
+            spec_interp = interp1d(model_box.wavelength, model_box.flux)
+
+            wavel_new = np.linspace(
+                model_box.wavelength[0],
+                model_box.wavelength[-1],
+                2 * model_box.wavelength.size,
+            )
+
+            if fast_rot_broad:
+                flux_broad = fastRotBroad(
+                    wvl=wavel_new,
+                    flux=spec_interp(wavel_new),
+                    epsilon=0.0,
+                    vsini=model_param["vsini"],
+                    effWvl=None,
+                )
+
+            else:
+                flux_broad = rotBroad(
+                    wvl=wavel_new,
+                    flux=spec_interp(wavel_new),
+                    epsilon=0.0,
+                    vsini=model_param["vsini"],
+                    edgeHandling="firstlast",
+                )
+
+            spec_interp = interp1d(wavel_new, flux_broad)
+
+            model_box.flux = spec_interp(model_box.wavelength)
+
         # Apply veiling
 
         if (
             "veil_a" in model_param
             and "veil_b" in model_param
             and "veil_ref" in model_param
         ):
@@ -830,44 +907,52 @@
         # Apply extinction
 
         if (
             "lognorm_radius" in model_param
             and "lognorm_sigma" in model_param
             and "lognorm_ext" in model_param
         ):
-
             model_box.flux = self.apply_lognorm_ext(
                 model_box.wavelength,
                 model_box.flux,
                 model_param["lognorm_radius"],
                 model_param["lognorm_sigma"],
                 model_param["lognorm_ext"],
             )
 
         if (
             "powerlaw_max" in model_param
             and "powerlaw_exp" in model_param
             and "powerlaw_ext" in model_param
         ):
-
             model_box.flux = self.apply_powerlaw_ext(
                 model_box.wavelength,
                 model_box.flux,
                 model_param["powerlaw_max"],
                 model_param["powerlaw_exp"],
                 model_param["powerlaw_ext"],
             )
 
-        if "ism_ext" in model_param:
+        if "ism_ext" in model_param or ext_filter is not None:
             ism_reddening = model_param.get("ism_red", 3.1)
 
+            if ext_filter is not None:
+                ism_ext_av = dust_util.convert_to_av(
+                    filter_name=ext_filter,
+                    filter_ext=model_param[f"phot_ext_{ext_filter}"],
+                    v_band_red=ism_reddening,
+                )
+
+            else:
+                ism_ext_av = model_param["ism_ext"]
+
             model_box.flux, ext_mag = self.apply_ext_ism(
                 model_box.wavelength,
                 model_box.flux,
-                model_param["ism_ext"],
+                ism_ext_av,
                 ism_reddening,
             )
 
             idx_select = ext_mag >= 0.0
             model_box.wavelength = model_box.wavelength[idx_select]
             model_box.flux = model_box.flux[idx_select]
 
@@ -929,23 +1014,23 @@
             )
 
             model_box.wavelength = wavel_resample
 
         # Convert flux to magnitude
 
         if magnitude:
-            with h5py.File(self.database, "r") as h5_file:
-                try:
-                    h5_file["spectra/calibration/vega"]
-
-                except KeyError:
-                    h5_file.close()
-                    species_db = database.Database()
-                    species_db.add_spectra("vega")
-                    h5_file = h5py.File(self.database, "r")
+            h5_file = h5py.File(self.database, "r")
+
+            if "spectra/calibration/vega" not in h5_file:
+                h5_file.close()
+                species_db = database.Database()
+                species_db.add_spectra("vega")
+
+            else:
+                h5_file.close()
 
             readcalib = read_calibration.ReadCalibration("vega", filter_name=None)
             calibbox = readcalib.get_spectrum()
 
             flux_vega, _ = spectres.spectres(
                 model_box.wavelength,
                 calibbox.wavelength,
@@ -1006,14 +1091,15 @@
 
     @typechecked
     def get_data(
         self,
         model_param: Dict[str, float],
         spec_res: Optional[float] = None,
         wavel_resample: Optional[np.ndarray] = None,
+        ext_filter: Optional[str] = None,
     ) -> box.ModelBox:
         """
         Function for selecting a model spectrum (without interpolation)
         for a set of parameter values that coincide with the grid
         points. The stored grid points can be inspected with
         :func:`~species.read.read_model.ReadModel.get_points`.
 
@@ -1029,14 +1115,23 @@
             spectrum if the argument is set to ``None``.
         wavel_resample : np.ndarray, None
             Wavelength points (um) to which the spectrum will be
             resampled. In that case, ``spec_res`` can still be used for
             smoothing the spectrum with a Gaussian kernel. The original
             wavelength points are used if the argument is set to
             ``None``.
+        ext_filter : str, None
+            Filter that is associated with the (optional) extinction
+            parameter, ``ism_ext``. When the argument of ``ext_filter``
+            is set to ``None``, the extinction is defined in the visual
+            as usual (i.e. :math:`A_V`). By providing a filter name
+            from the `SVO Filter Profile Service <http://svo2.cab.
+            inta-csic.es/svo/theory/fps/>`_ as argument then the
+            extinction ``ism_ext`` is defined in that filter instead
+            of the $V$ band.
 
         Returns
         -------
         species.core.box.ModelBox
             Box with the model spectrum.
         """
 
@@ -1082,14 +1177,23 @@
         param_val = []
 
         for item in check_param:
             if item in model_param and item not in ignore_param:
                 param_key.append(item)
                 param_val.append(model_param[item])
 
+        # Check if the ext_filter should be adjusted
+        # to the name that is extracted from the
+        # phot_ext_{ext_filter} parameter
+
+        if ext_filter is None:
+            for param_item in model_param:
+                if param_item.startswith("phot_ext_"):
+                    ext_filter = param_item[9:]
+
         # Read the grid of fluxes from the database
 
         flux = np.asarray(h5_file[f"models/{self.model}/flux"])
 
         # Find the indices of the grid points for which the spectrum will be extracted
 
         indices = []
@@ -1181,44 +1285,52 @@
         # Apply extinction
 
         if (
             "lognorm_radius" in model_param
             and "lognorm_sigma" in model_param
             and "lognorm_ext" in model_param
         ):
-
             model_box.flux = self.apply_lognorm_ext(
                 model_box.wavelength,
                 model_box.flux,
                 model_param["lognorm_radius"],
                 model_param["lognorm_sigma"],
                 model_param["lognorm_ext"],
             )
 
         if (
             "powerlaw_max" in model_param
             and "powerlaw_exp" in model_param
             and "powerlaw_ext" in model_param
         ):
-
             model_box.flux = self.apply_powerlaw_ext(
                 model_box.wavelength,
                 model_box.flux,
                 model_param["powerlaw_max"],
                 model_param["powerlaw_exp"],
                 model_param["powerlaw_ext"],
             )
 
-        if "ism_ext" in model_param:
+        if "ism_ext" in model_param or ext_filter is not None:
             ism_reddening = model_param.get("ism_red", 3.1)
 
+            if ext_filter is not None:
+                ism_ext_av = dust_util.convert_to_av(
+                    filter_name=ext_filter,
+                    filter_ext=model_param[f"phot_ext_{ext_filter}"],
+                    v_band_red=ism_reddening,
+                )
+
+            else:
+                ism_ext_av = model_param["ism_ext"]
+
             model_box.flux, ext_mag = self.apply_ext_ism(
                 model_box.wavelength,
                 model_box.flux,
-                model_param["ism_ext"],
+                ism_ext_av,
                 ism_reddening,
             )
 
             idx_select = ext_mag >= 0.0
             model_box.wavelength = model_box.wavelength[idx_select]
             model_box.flux = model_box.flux[idx_select]
 
@@ -1269,26 +1381,37 @@
                 * model_box.parameters["disk_teff"] ** 4.0
                 / constants.L_SUN
             )  # (Lsun)
 
         return model_box
 
     @typechecked
-    def get_flux(self, model_param: Dict[str, float], synphot=None):
+    def get_flux(
+        self, model_param: Dict[str, float], synphot=None, return_box: bool = False
+    ) -> Union[Tuple[Optional[float], Optional[float]], box.PhotometryBox]:
         """
         Function for calculating the average flux density for the
         ``filter_name``.
 
         Parameters
         ----------
         model_param : dict
             Model parameters and values.
         synphot : species.analysis.photometry.SyntheticPhotometry, None
             Synthetic photometry object. The object is created if set
             to ``None``.
+        return_box : bool
+            Return a :class:`~species.core.box.PhotometryBox`
+            if set to ``True`` or return the two values that are
+            specified below if set to ``False``. By default, the
+            argument is set to ``False``. The advantage of
+            returning the output in a
+            :class:`~species.core.box.PhotometryBox` is that it can
+            directly be provided as input to
+            :func:`~species.plot.plot_spectrum.plot_spectrum`.
 
         Returns
         -------
         float
             Average flux (W m-2 um-1).
         float, None
             Uncertainty (W m-2 um-1), which is set to ``None``.
@@ -1305,32 +1428,60 @@
             self.interpolate_model()
 
         spectrum = self.get_model(model_param)
 
         if synphot is None:
             synphot = photometry.SyntheticPhotometry(self.filter_name)
 
-        return synphot.spectrum_to_flux(spectrum.wavelength, spectrum.flux)
+        model_flux = synphot.spectrum_to_flux(spectrum.wavelength, spectrum.flux)
+
+        if return_box:
+            model_mag = self.get_magnitude(model_param)
+
+            phot_box = box.create_box(
+                boxtype="photometry",
+                name=self.model,
+                wavelength=[self.mean_wavelength],
+                flux=[model_flux],
+                app_mag=[(model_mag[0], None)],
+                abs_mag=[(model_mag[1], None)],
+                filter_name=[self.filter_name],
+            )
+
+            return phot_box
+
+        return model_flux
 
     @typechecked
     def get_magnitude(
-        self, model_param: Dict[str, float]
-    ) -> Tuple[Optional[float], Optional[float]]:
+        self,
+        model_param: Dict[str, float],
+        return_box: bool = False,
+    ) -> Union[Tuple[Optional[float], Optional[float]], box.PhotometryBox]:
         """
         Function for calculating the apparent and absolute magnitudes
         for the ``filter_name``.
 
         Parameters
         ----------
         model_param : dict
             Dictionary with the model parameters. A ``radius`` (Rjup),
             and ``parallax`` (mas) or ``distance`` (pc) are required
             for the apparent magnitude (i.e. to scale the flux from
             the planet to the observer). Only a ``radius`` is
             required for the absolute magnitude.
+        return_box : bool
+            Return a :class:`~species.core.box.PhotometryBox`
+            if set to ``True`` or return the two values that are
+            specified below if set to ``False``. By default, the
+            argument is set to ``False``. The advantage of
+            returning the output in a
+            :class:`~species.core.box.PhotometryBox` is that it can
+            directly be provided as input to
+            :func:`~species.plot.plot_spectrum.plot_spectrum`.
 
         Returns
         -------
         float
             Apparent magnitude. A ``None`` is returned if the
             dictionary of ``model_param`` does not contain a
             ``radius``, and ``parallax`` or ``distance``.
@@ -1392,14 +1543,29 @@
                     spectrum.flux *= (model_param["radius"] * constants.R_JUP) ** 2
                     spectrum.flux /= (distance * constants.PARSEC) ** 2
 
                     _, abs_mag = synphot.spectrum_to_magnitude(
                         spectrum.wavelength, spectrum.flux, distance=(distance, None)
                     )
 
+        if return_box:
+            model_flux = self.get_flux(model_param)
+
+            phot_box = box.create_box(
+                boxtype="photometry",
+                name=self.model,
+                wavelength=[self.mean_wavelength],
+                flux=[model_flux],
+                app_mag=[(app_mag[0], None)],
+                abs_mag=[(abs_mag[0], None)],
+                filter_name=[self.filter_name],
+            )
+
+            return phot_box
+
         return app_mag[0], abs_mag[0]
 
     @typechecked
     def get_bounds(self) -> Dict[str, Tuple[float, float]]:
         """
         Function for extracting the grid boundaries.
```

### Comparing `species-0.5.5/species/read/read_object.py` & `species-0.6.0/species/read/read_object.py`

 * *Files identical despite different names*

### Comparing `species-0.5.5/species/read/read_planck.py` & `species-0.6.0/species/read/read_planck.py`

 * *Files identical despite different names*

### Comparing `species-0.5.5/species/read/read_radtrans.py` & `species-0.6.0/species/read/read_radtrans.py`

 * *Files 1% similar despite different names*

```diff
@@ -941,20 +941,18 @@
                 optical_depth = np.sum(
                     w_gauss * self.rt_object.total_tau[:, :, :, :], axis=0
                 )
 
                 # Sum over all species
                 optical_depth = np.sum(optical_depth, axis=1)
 
-            mpl.rcParams["font.family"] = "serif"
-            mpl.rcParams["mathtext.fontset"] = "dejavuserif"
+            plt.rcParams["font.family"] = "serif"
+            plt.rcParams["mathtext.fontset"] = "dejavuserif"
 
-            plt.rc("axes", edgecolor="black", linewidth=2.5)
-
-            plt.figure(1, figsize=(8.0, 4.0))
+            plt.figure(figsize=(8.0, 4.0))
             gridsp = mpl.gridspec.GridSpec(1, 1)
             gridsp.update(wspace=0, hspace=0, left=0, right=1, bottom=0, top=1)
 
             ax = plt.subplot(gridsp[0, 0])
 
             ax.tick_params(
                 axis="both",
```

### Comparing `species-0.5.5/species/read/read_spectrum.py` & `species-0.6.0/species/read/read_spectrum.py`

 * *Files 7% similar despite different names*

```diff
@@ -82,18 +82,15 @@
         -------
         species.core.box.SpectrumBox
             Box with the spectra.
         """
 
         h5_file = h5py.File(self.database, "r")
 
-        try:
-            h5_file[f"spectra/{self.spec_library}"]
-
-        except KeyError:
+        if self.spec_library not in h5_file[f"spectra"]:
             h5_file.close()
             species_db = database.Database()
             species_db.add_spectra(self.spec_library, sptypes)
             h5_file = h5py.File(self.database, "r")
 
         list_wavelength = []
         list_flux = []
@@ -108,21 +105,19 @@
             dset = h5_file[f"spectra/{self.spec_library}/{item}"]
 
             wavelength = dset[:, 0]  # (um)
             flux = dset[:, 1]  # (W m-2 um-1)
             error = dset[:, 2]  # (W m-2 um-1)
 
             if exclude_nan:
-                indices = np.isnan(flux)
-                indices = np.logical_not(indices)
-                indices = np.where(indices)[0]
-
-                wavelength = wavelength[indices]
-                flux = flux[indices]
-                error = error[indices]
+                nan_index = np.isnan(flux)
+
+                wavelength = wavelength[~nan_index]
+                flux = flux[~nan_index]
+                error = error[~nan_index]
 
             if self.wavel_range is None:
                 wl_index = np.arange(0, len(wavelength), 1)
 
             else:
                 wl_index = (
                     (flux > 0.0)
@@ -177,65 +172,63 @@
                     )
                 else:
                     list_parallax.append((np.nan, np.nan))
 
                 if "spec_res" in attrs:
                     list_spec_res.append(dset.attrs["spec_res"])
                 else:
-                    list_parallax.append(np.nan)
+                    list_spec_res.append(np.nan)
 
             else:
                 list_wavelength.append(np.array([]))
                 list_flux.append(np.array([]))
                 list_error.append(np.array([]))
                 list_name.append("")
                 list_simbad.append("")
                 list_sptype.append("None")
                 list_parallax.append((np.nan, np.nan))
                 list_spec_res.append(np.nan)
 
-        specbox = box.SpectrumBox()
-        specbox.spec_library = self.spec_library
+        spec_box = box.SpectrumBox()
+        spec_box.spec_library = self.spec_library
 
         if sptypes is not None:
-            indices = []
-
-            specbox.wavelength = []
-            specbox.flux = []
-            specbox.error = []
-            specbox.name = []
-            specbox.simbad = []
-            specbox.sptype = []
-            specbox.parallax = []
-            specbox.spec_res = []
+            spec_box.wavelength = []
+            spec_box.flux = []
+            spec_box.error = []
+            spec_box.name = []
+            spec_box.simbad = []
+            spec_box.sptype = []
+            spec_box.parallax = []
+            spec_box.spec_res = []
 
             for item in sptypes:
 
                 for i, spec_item in enumerate(list_sptype):
                     if item == spec_item[:2]:
-                        specbox.wavelength.append(list_wavelength[i])
-                        specbox.flux.append(list_flux[i])
-                        specbox.error.append(list_error[i])
-                        specbox.name.append(list_name[i])
-                        specbox.simbad.append(list_simbad[i])
-                        specbox.sptype.append(list_sptype[i])
-                        specbox.parallax.append(list_parallax[i])
-                        specbox.spec_res.append(list_spec_res[i])
+                        spec_box.wavelength.append(list_wavelength[i])
+                        spec_box.flux.append(list_flux[i])
+                        spec_box.error.append(list_error[i])
+                        spec_box.name.append(list_name[i])
+                        spec_box.simbad.append(list_simbad[i])
+                        spec_box.sptype.append(list_sptype[i])
+                        spec_box.parallax.append(list_parallax[i])
+                        spec_box.spec_res.append(list_spec_res[i])
 
         else:
-            specbox.wavelength = list_wavelength
-            specbox.flux = list_flux
-            specbox.error = list_error
-            specbox.name = list_name
-            specbox.simbad = list_simbad
-            specbox.sptype = list_sptype
-            specbox.parallax = list_parallax
-            specbox.spec_res = list_spec_res
+            spec_box.wavelength = list_wavelength
+            spec_box.flux = list_flux
+            spec_box.error = list_error
+            spec_box.name = list_name
+            spec_box.simbad = list_simbad
+            spec_box.sptype = list_sptype
+            spec_box.parallax = list_parallax
+            spec_box.spec_res = list_spec_res
 
-        return specbox
+        return spec_box
 
     @typechecked
     def get_flux(self, sptypes: List[str] = None) -> box.PhotometryBox:
         """
         Function for calculating the average flux density for the
         ``filter_name``.
 
@@ -248,108 +241,108 @@
 
         Returns
         -------
         species.core.box.PhotometryBox
             Box with the synthetic photometry.
         """
 
-        specbox = self.get_spectrum(sptypes=sptypes, exclude_nan=True)
+        spec_box = self.get_spectrum(sptypes=sptypes, exclude_nan=True)
 
-        n_spectra = len(specbox.wavelength)
+        n_spectra = len(spec_box.wavelength)
 
         filter_profile = read_filter.ReadFilter(filter_name=self.filter_name)
         mean_wavel = filter_profile.mean_wavelength()
 
         wavelengths = np.full(n_spectra, mean_wavel)
         filters = np.full(n_spectra, self.filter_name)
 
         synphot = photometry.SyntheticPhotometry(filter_name=self.filter_name)
 
         phot_flux = []
 
         for i in range(n_spectra):
             flux = synphot.spectrum_to_flux(
-                wavelength=specbox.wavelength[i],
-                flux=specbox.flux[i],
-                error=specbox.error[i],
+                wavelength=spec_box.wavelength[i],
+                flux=spec_box.flux[i],
+                error=spec_box.error[i],
             )
 
             phot_flux.append(flux)
 
         phot_flux = np.asarray(phot_flux)
 
         return box.create_box(
             boxtype="photometry",
-            name=specbox.name,
-            sptype=specbox.sptype,
+            name=spec_box.name,
+            sptype=spec_box.sptype,
             wavelength=wavelengths,
             flux=phot_flux,
             app_mag=None,
             abs_mag=None,
             filter_name=filters,
         )
 
     @typechecked
     def get_magnitude(self, sptypes: List[str] = None) -> box.PhotometryBox:
         """
         Function for calculating the apparent magnitude for the
-        ``filter_name``.
+        specified ``filter_name``.
 
         Parameters
         ----------
         sptypes : list(str)
-            Spectral types to select from a library. The spectral types
-            should be indicated with two characters (e.g. 'M5', 'L2',
-            'T3'). All spectra are selected if set to ``None``.
+            Spectral types to select from the library. The spectral
+            types should be indicated with two characters (e.g. 'M5',
+            'L2', 'T3'). All spectra are selected if set to ``None``.
 
         Returns
         -------
         species.core.box.PhotometryBox
             Box with the synthetic photometry.
         """
 
-        specbox = self.get_spectrum(sptypes=sptypes, exclude_nan=True)
+        spec_box = self.get_spectrum(sptypes=sptypes, exclude_nan=True)
 
-        n_spectra = len(specbox.wavelength)
+        n_spectra = len(spec_box.wavelength)
 
         filter_profile = read_filter.ReadFilter(filter_name=self.filter_name)
         mean_wavel = filter_profile.mean_wavelength()
 
         wavelengths = np.full(n_spectra, mean_wavel)
         filters = np.full(n_spectra, self.filter_name)
 
         synphot = photometry.SyntheticPhotometry(filter_name=self.filter_name)
 
         app_mag = []
         abs_mag = []
 
         for i in range(n_spectra):
 
-            if np.isnan(specbox.parallax[i][0]):
+            if np.isnan(spec_box.parallax[i][0]):
                 app_tmp = (np.nan, np.nan)
                 abs_tmp = (np.nan, np.nan)
 
             else:
 
                 app_tmp, abs_tmp = synphot.spectrum_to_magnitude(
-                    specbox.wavelength[i],
-                    specbox.flux[i],
-                    error=specbox.error[i],
+                    spec_box.wavelength[i],
+                    spec_box.flux[i],
+                    error=spec_box.error[i],
                     parallax=(
-                        float(specbox.parallax[i][0]),
-                        float(specbox.parallax[i][1]),
+                        float(spec_box.parallax[i][0]),
+                        float(spec_box.parallax[i][1]),
                     ),
                 )
 
             app_mag.append(app_tmp)
             abs_mag.append(abs_tmp)
 
         return box.create_box(
             boxtype="photometry",
-            name=specbox.name,
-            sptype=specbox.sptype,
+            name=spec_box.name,
+            sptype=spec_box.sptype,
             wavelength=wavelengths,
             flux=None,
             app_mag=np.asarray(app_mag),
             abs_mag=np.asarray(abs_mag),
             filter_name=filters,
         )
```

### Comparing `species-0.5.5/species/util/data_util.py` & `species-0.6.0/species/util/data_util.py`

 * *Files identical despite different names*

### Comparing `species-0.5.5/species/util/dust_util.py` & `species-0.6.0/species/util/dust_util.py`

 * *Files 8% similar despite different names*

```diff
@@ -404,16 +404,16 @@
             for j in range(sigma_g.shape[0]):
                 cross_interp = interp1d(
                     wavelength, cross_section[:, i, j], kind="linear", bounds_error=True
                 )
 
                 cross_tmp = cross_interp(filt_trans[:, 0])
 
-                integral1 = np.trapz(filt_trans[:, 1] * cross_tmp, filt_trans[:, 0])
-                integral2 = np.trapz(filt_trans[:, 1], filt_trans[:, 0])
+                integral1 = np.trapz(filt_trans[:, 1] * cross_tmp, x=filt_trans[:, 0])
+                integral2 = np.trapz(filt_trans[:, 1], x=filt_trans[:, 0])
 
                 # Filter-weighted average of the extinction cross section
                 cross_phot[i, j] = integral1 / integral2
 
         cross_sections[phot_item] = interp2d(
             sigma_g, radius_g, cross_phot, kind="linear", bounds_error=True
         )
@@ -514,16 +514,16 @@
             for j in range(exponent.shape[0]):
                 cross_interp = interp1d(
                     wavelength, cross_section[:, i, j], kind="linear", bounds_error=True
                 )
 
                 cross_tmp = cross_interp(filt_trans[:, 0])
 
-                integral1 = np.trapz(filt_trans[:, 1] * cross_tmp, filt_trans[:, 0])
-                integral2 = np.trapz(filt_trans[:, 1], filt_trans[:, 0])
+                integral1 = np.trapz(filt_trans[:, 1] * cross_tmp, x=filt_trans[:, 0])
+                integral2 = np.trapz(filt_trans[:, 1], x=filt_trans[:, 0])
 
                 # Filter-weighted average of the extinction cross section
                 cross_phot[i, j] = integral1 / integral2
 
         cross_sections[phot_item] = interp2d(
             exponent, radius_max, cross_phot, kind="linear", bounds_error=True
         )
@@ -544,15 +544,14 @@
                 )
 
                 cross_spec[:, i, j] = cross_interp(wavel_spec)
 
         cross_sections[spec_item] = []
 
         for i in range(wavel_spec.shape[0]):
-
             cross_tmp = interp2d(
                 exponent,
                 radius_max,
                 cross_spec[i, :, :],
                 kind="linear",
                 bounds_error=True,
             )
@@ -656,7 +655,53 @@
     np.ndarray
         Fluxes (W m-2 um-1) with the extinction applied.
     """
 
     ext_mag = ism_extinction(v_band_ext, v_band_red, wavelengths)
 
     return flux * 10.0 ** (-0.4 * ext_mag)
+
+
+@typechecked
+def convert_to_av(
+    filter_name: str, filter_ext: float, v_band_red: float = 3.1
+) -> float:
+    """
+    Function for converting the extinction in any filter from
+    the `SVO Filter Profile Service <http://svo2.cab.inta-csic.
+    es/svo/theory/fps/>`_ to a visual extinction, :math:`A_V`.
+    This is done by simply scaling the extinction so at the
+    mean wavelength of the filter.
+
+    filter_name : str
+        Filter name for which the extinction will be
+        converted to a visual extinction (i.e. :math:`A_V`).
+    filter_ext : float
+        Extinction (mag) for the ``filter_name``.
+    v_band_red : float
+        Reddening in the $V$ band.
+
+    Returns
+    -------
+    float
+        Visual extinction (i.e. :math:`A_V`) for which the
+        extinction in the ``filter_name`` band is ``filter_ext``.
+    """
+
+    av_test = 1.0
+
+    # Mean wavelength for filter_name
+    read_filt = read_filter.ReadFilter(filter_name)
+    filt_wavel = np.array([read_filt.mean_wavelength()])
+
+    # Calculate test extinction for A_V = 1.0
+    # at mean wavelength of filter_name
+    ext_ref = ism_extinction(av_test, v_band_red, filt_wavel)[0]
+
+    # Scaling for A_V = 1.0 to the A_V for which
+    # extinction of filter_name is filter_ext
+    scaling = filter_ext / ext_ref
+
+    # Should be the same as filter_ext
+    # filter_ext_test = ism_extinction(scaling * av_test, v_band_red, filt_wavel)[0]
+
+    return scaling * av_test
```

### Comparing `species-0.5.5/species/util/phot_util.py` & `species-0.6.0/species/util/phot_util.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,49 +29,61 @@
     datatype: str,
     spectrum: str,
     filters: List[str],
     parameters: Dict[str, float],
     radtrans: Optional[read_radtrans.ReadRadtrans] = None,
 ) -> box.SynphotBox:
     """
+    Function for calculating synthetic photometry for a list of
+    filters and a specified atmosphere model and related parameters.
+    This function can for example be used for calculating the
+    synthetic photometry from a best-fit model spectrum. It returns
+    a :class:`~species.core.box.SynphotBox` that can be provided
+    as input to :func:`~species.plot.plot_spectrum.plot_spectrum`.
+
     Parameters
     ----------
     datatype : str
         Data type ('model' or 'calibration').
     spectrum : str
-        Spectrum name (e.g., 'drift-phoenix', 'planck', 'powerlaw',
-        'petitradtrans').
+        Spectrum name (e.g., 'drift-phoenix', 'bt-settl-cifist',
+        planck', 'powerlaw', 'petitradtrans').
     filters : list(str)
         List with the filter names.
     parameters : dict
         Dictionary with the model parameters.
     radtrans : read_radtrans.ReadRadtrans, None
         Instance of :class:`~species.read.read_radtrans.ReadRadtrans`.
         Only required with ``spectrum='petitradtrans'`. Make sure that
         the ``wavel_range`` of the ``ReadRadtrans`` instance is
-        sufficiently broad to cover all the ``filters``. Not used if
-        set to `None`.
+        sufficiently broad to cover all the ``filters``. The argument
+        can be set to ``None`` for any other model than petitRADTRANS.
 
     Returns
     -------
     species.core.box.SynphotBox
         Box with synthetic photometry.
     """
 
     print("Calculating synthetic photometry...", end="", flush=True)
 
+    mean_wavel = {}
+
+    for item in filters:
+        read_filt = read_filter.ReadFilter(item)
+        mean_wavel[item] = read_filt.mean_wavelength
+
     flux = {}
 
     if datatype == "model":
         if spectrum == "petitradtrans":
             # Calculate the petitRADTRANS spectrum only once
             radtrans_box = radtrans.get_model(parameters)
 
         for item in filters:
-
             if spectrum == "petitradtrans":
                 # Use an instance of SyntheticPhotometry instead
                 # of get_flux from ReadRadtrans in order to not
                 # recalculate the spectrum
                 syn_phot = photometry.SyntheticPhotometry(item)
 
                 flux[item], _ = syn_phot.spectrum_to_flux(
@@ -128,17 +140,44 @@
                     )
 
     elif datatype == "calibration":
         for item in filters:
             readcalib = read_calibration.ReadCalibration(spectrum, filter_name=item)
             flux[item] = readcalib.get_flux(parameters)[0]
 
+    app_mag = {}
+    abs_mag = {}
+
+    for key, value in flux.items():
+        syn_phot = photometry.SyntheticPhotometry(key)
+        if "parallax" in parameters:
+            app_mag[key], abs_mag[key] = syn_phot.flux_to_magnitude(
+                flux=value, error=None, parallax=(parameters["parallax"], None)
+            )
+
+        elif "distance" in parameters:
+            app_mag[key], abs_mag[key] = syn_phot.flux_to_magnitude(
+                flux=value, error=None, distance=(parameters["distance"], None)
+            )
+
+        else:
+            app_mag[key], abs_mag[key] = syn_phot.flux_to_magnitude(
+                flux=value, error=None
+            )
+
     print(" [DONE]")
 
-    return box.create_box("synphot", name="synphot", flux=flux)
+    return box.create_box(
+        "synphot",
+        name="synphot",
+        flux=flux,
+        wavelength=mean_wavel,
+        app_mag=app_mag,
+        abs_mag=abs_mag,
+    )
 
 
 @typechecked
 def apparent_to_absolute(
     app_mag: Union[
         Tuple[float, Optional[float]], Tuple[np.ndarray, Optional[np.ndarray]]
     ],
@@ -187,29 +226,35 @@
 
 
 @typechecked
 def absolute_to_apparent(
     abs_mag: Union[
         Tuple[float, Optional[float]], Tuple[np.ndarray, Optional[np.ndarray]]
     ],
-    distance: Union[Tuple[float, Optional[float]], Tuple[np.ndarray, Optional[np.ndarray]]],
+    distance: Union[
+        Tuple[float, Optional[float]], Tuple[np.ndarray, Optional[np.ndarray]]
+    ],
 ) -> Union[Tuple[float, Optional[float]], Tuple[np.ndarray, Optional[np.ndarray]]]:
     """
     Function for converting an absolute magnitude
     into an apparent magnitude.
 
     Parameters
     ----------
     abs_mag : tuple(float, float), tuple(np.ndarray, np.ndarray)
-        Absolute magnitude and uncertainty (mag). The same uncertainty
-        is used for the apparent magnitude.
+        Tuple with the absolute magnitude and uncertainty (mag).
+        The uncertainty on the returned apparent magnitude is
+        simply adopted from the absolute magnitude. Providing the
+        uncertainty is optional and can be set to ``None``.
     distance : tuple(float, float), tuple(np.ndarray, np.ndarray)
-        Distance and uncertainty (pc). The uncertainty is optional
-        and actually not used by this function but included for
-        redundancy.
+        Tuple with the distance and uncertainty (pc). The uncertainty
+        is optional and can be set to ``None``. The distance
+        uncertainty is currently not used by this function but
+        included so it can be implemented at some point into the
+        error budget.
 
     Returns
     -------
     float, np.ndarray
         Apparent magnitude (mag).
     float, np.ndarray, None
         Uncertainty (mag).
@@ -226,15 +271,14 @@
     spectrum: str,
     parameters: Dict[str, float],
     objectbox: box.ObjectBox,
     inc_phot: Union[bool, List[str]] = True,
     inc_spec: Union[bool, List[str]] = True,
     radtrans: Optional[read_radtrans.ReadRadtrans] = None,
 ) -> box.ResidualsBox:
-
     """
     Function for calculating the residuals from fitting model or
     calibration spectra to a set of spectra and/or photometry.
 
     Parameters
     ----------
     datatype : str
@@ -242,15 +286,15 @@
     spectrum : str
         Name of the atmospheric model or calibration spectrum.
     parameters : dict
         Parameters and values for the spectrum
     objectbox : species.core.box.ObjectBox
         Box with the photometry and/or spectra of an object. A scaling
         and/or error inflation of the spectra should be applied with
-        :func:`~species.util.read_util.update_spectra` beforehand.
+        :func:`~species.util.read_util.update_objectbox` beforehand.
     inc_phot : bool, list(str)
         Include photometric data in the fit. If a boolean, either all
         (``True``) or none (``False``) of the data are selected. If a
         list, a subset of filter names (as stored in the database) can
         be provided.
     inc_spec : bool, list(str)
         Include spectroscopic data in the fit. If a boolean, either all
@@ -268,18 +312,18 @@
 
     Returns
     -------
     species.core.box.ResidualsBox
         Box with the residuals.
     """
 
-    if isinstance(inc_phot, bool) and inc_phot:
-        inc_phot = objectbox.filters
+    if inc_phot and objectbox.filters is not None:
+        if isinstance(inc_phot, bool) and inc_phot:
+            inc_phot = objectbox.filters
 
-    if inc_phot:
         model_phot = multi_photometry(
             datatype=datatype,
             spectrum=spectrum,
             filters=inc_phot,
             parameters=parameters,
             radtrans=radtrans,
         )
@@ -302,23 +346,22 @@
                     res_phot[item][1, j] = (
                         objectbox.flux[item][0, j] - model_phot.flux[item]
                     ) / objectbox.flux[item][1, j]
 
     else:
         res_phot = None
 
-    if inc_spec:
+    if inc_spec and objectbox.spectrum is not None:
         res_spec = {}
 
         if spectrum == "petitradtrans":
             # Calculate the petitRADTRANS spectrum only once
             model = radtrans.get_model(parameters)
 
         for key in objectbox.spectrum:
-
             if isinstance(inc_spec, bool) or key in inc_spec:
                 wavel_range = (
                     0.9 * objectbox.spectrum[key][0][0, 0],
                     1.1 * objectbox.spectrum[key][0][-1, 0],
                 )
 
                 wl_new = objectbox.spectrum[key][0][:, 0]
@@ -470,16 +513,17 @@
         spectrum=res_spec,
         chi2_red=chi2_red,
     )
 
 
 @typechecked
 def parallax_to_distance(
-    parallax: Union[Tuple[float, Optional[float]],
-                    Tuple[np.ndarray, Optional[np.ndarray]]],
+    parallax: Union[
+        Tuple[float, Optional[float]], Tuple[np.ndarray, Optional[np.ndarray]]
+    ],
 ) -> Union[Tuple[float, Optional[float]], Tuple[np.ndarray, Optional[np.ndarray]]]:
     """
     Function for converting from parallax to distance.
 
     Parameters
     ----------
     parallax : tuple(float, float), tuple(np.ndarray, np.ndarray)
```

### Comparing `species-0.5.5/species/util/plot_util.py` & `species-0.6.0/species/util/plot_util.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,131 +1,190 @@
 """
 Utility functions for plotting data.
 """
 
+import warnings
+
 from typing import Optional, Tuple, List
 
 import numpy as np
 
 from typeguard import typechecked
 
 
 @typechecked
-def sptype_substellar(sptype: np.ndarray, shape: Tuple[int]) -> np.ndarray:
+def sptype_to_index(
+    field_range: Tuple[str, str], spec_types: np.ndarray, check_subclass: bool
+) -> np.ndarray:
     """
-    Function for mapping the spectral types of substellar objects
-    (M, L, T, and Y) to numbers.
+    Function for mapping the spectral types of stellar and
+    substellar objects to indices that corresponds with the
+    discrete colorbar of a color-magnitude or color-color
+    diagram.
 
     Parameters
     ----------
-    sptype : np.ndarray
-        Array with spectral types.
-    shape : tuple(int)
-        Shape (1D) of the output array
+    field_range : tuple(str, str)
+        Range of the discrete colorbar for the field objects. The tuple
+        should contain the lower and upper value ('early M', 'late M',
+        'early L', 'late L', 'early T', 'late T', 'early Y). Also
+        stellar spectral types can be specified.
+    spec_types : np.ndarray
+        Array with the spectral types.
+    check_subclass : bool
+        Set to ``True`` if the discrete colorbar should distinguish
+        early and late spectral types with different colors or set
+        to ``False`` if subclasses should not be distinguished.
 
     Returns
     -------
     np.ndarray
-        Array with spectral types mapped to numbers.
+        Array with spectral types mapped to indices. Spectral types
+        that are not within the range specified with ``field_range``
+        will be set to NaN.
     """
 
-    spt_disc = np.zeros(shape)
+    spt_discrete = np.zeros(spec_types.size)
 
-    for i, item in enumerate(sptype):
-        if item[0:2] in ["M0", "M1", "M2", "M3", "M4"]:
-            spt_disc[i] = 0.5
+    if check_subclass:
+        spt_check = [
+            ("early O", "late O"),
+            ("early B", "late B"),
+            ("early A", "late A"),
+            ("early F", "late F"),
+            ("early G", "late G"),
+            ("early K", "late K"),
+            ("early M", "late M"),
+            ("early L", "late L"),
+            ("early T", "late T"),
+            ("early Y", "late Y"),
+        ]
 
-        elif item[0:2] in ["M5", "M6", "M7", "M8", "M9"]:
-            spt_disc[i] = 1.5
+        for i, item in enumerate(spec_types):
+            if item[0:2] in ["O0", "O1", "O2", "O3", "O4"]:
+                spt_discrete[i] = 0.5
 
-        elif item[0:2] in ["L0", "L1", "L2", "L3", "L4"]:
-            spt_disc[i] = 2.5
+            elif item[0:2] in ["O5", "O6", "O7", "O8", "O9"]:
+                spt_discrete[i] = 1.5
 
-        elif item[0:2] in ["L5", "L6", "L7", "L8", "L9"]:
-            spt_disc[i] = 3.5
+            elif item[0:2] in ["B0", "B1", "B2", "B3", "B4"]:
+                spt_discrete[i] = 2.5
 
-        elif item[0:2] in ["T0", "T1", "T2", "T3", "T4"]:
-            spt_disc[i] = 4.5
+            elif item[0:2] in ["B5", "B6", "B7", "B8", "B9"]:
+                spt_discrete[i] = 3.5
 
-        elif item[0:2] in ["T5", "T6", "T7", "T8", "T9"]:
-            spt_disc[i] = 5.5
+            elif item[0:2] in ["A0", "A1", "A2", "A3", "A4"]:
+                spt_discrete[i] = 4.5
 
-        elif "Y" in item:
-            spt_disc[i] = 6.5
+            elif item[0:2] in ["A5", "A6", "A7", "A8", "A9"]:
+                spt_discrete[i] = 5.5
 
-        else:
-            spt_disc[i] = np.nan
-            continue
+            elif item[0:2] in ["F0", "F1", "F2", "F3", "F4"]:
+                spt_discrete[i] = 6.5
 
-    return spt_disc
+            elif item[0:2] in ["F5", "F6", "F7", "F8", "F9"]:
+                spt_discrete[i] = 7.5
 
+            elif item[0:2] in ["G0", "G1", "G2", "G3", "G4"]:
+                spt_discrete[i] = 8.5
 
-@typechecked
-def sptype_stellar(sptype: np.ndarray, shape: Tuple[int]) -> np.ndarray:
-    """
-    Function for mapping all spectral types (O through Y) to numbers.
+            elif item[0:2] in ["G5", "G6", "G7", "G8", "G9"]:
+                spt_discrete[i] = 9.5
 
-    Parameters
-    ----------
-    sptype : np.ndarray
-        Array with spectral types.
-    shape : tuple(int)
-        Shape (1D) of the output array
+            elif item[0:2] in ["K0", "K1", "K2", "K3", "K4"]:
+                spt_discrete[i] = 10.5
 
-    Returns
-    -------
-    np.ndarray
-        Array with spectral types mapped to numbers.
-    """
+            elif item[0:2] in ["K5", "K6", "K7", "K8", "K9"]:
+                spt_discrete[i] = 11.5
 
-    spt_disc = np.zeros(shape)
+            elif item[0:2] in ["M0", "M1", "M2", "M3", "M4"]:
+                spt_discrete[i] = 12.5
 
-    for i, item in enumerate(sptype):
-        if item[0] == "O":
-            spt_disc[i] = 0.5
+            elif item[0:2] in ["M5", "M6", "M7", "M8", "M9"]:
+                spt_discrete[i] = 13.5
 
-        elif item[0] == "B":
-            spt_disc[i] = 1.5
+            elif item[0:2] in ["L0", "L1", "L2", "L3", "L4"]:
+                spt_discrete[i] = 14.5
 
-        elif item[0] == "A":
-            spt_disc[i] = 2.5
+            elif item[0:2] in ["L5", "L6", "L7", "L8", "L9"]:
+                spt_discrete[i] = 15.5
 
-        elif item[0] == "F":
-            spt_disc[i] = 3.5
+            elif item[0:2] in ["T0", "T1", "T2", "T3", "T4"]:
+                spt_discrete[i] = 16.5
 
-        elif item[0] == "G":
-            spt_disc[i] = 4.5
+            elif item[0:2] in ["T5", "T6", "T7", "T8", "T9"]:
+                spt_discrete[i] = 17.5
 
-        elif item[0] == "K":
-            spt_disc[i] = 5.5
+            elif "Y" in item:
+                spt_discrete[i] = 18.5
 
-        elif item[0] == "M":
-            spt_disc[i] = 6.5
+            else:
+                spt_discrete[i] = np.nan
 
-        elif item[0] == "L":
-            spt_disc[i] = 7.5
+        count = 0
+        for i, item in enumerate(spt_check):
+            for j in range(2):
+                if field_range[0] == item[j]:
+                    spt_discrete -= float(count)
+                    break
+                count += 1
 
-        elif item[0] == "T":
-            spt_disc[i] = 8.5
+    else:
+        spt_check = ["O", "B", "A", "F", "G", "K", "M", "L", "T", "Y"]
 
-        elif item[0] == "Y":
-            spt_disc[i] = 9.5
+        for i, item in enumerate(spec_types):
+            if item[0] == "O":
+                spt_discrete[i] = 0.5
 
-        else:
-            spt_disc[i] = np.nan
-            continue
+            elif item[0] == "B":
+                spt_discrete[i] = 1.5
+
+            elif item[0] == "A":
+                spt_discrete[i] = 2.5
+
+            elif item[0] == "F":
+                spt_discrete[i] = 3.5
+
+            elif item[0] == "G":
+                spt_discrete[i] = 4.5
+
+            elif item[0] == "K":
+                spt_discrete[i] = 5.5
 
-    return spt_disc
+            elif item[0] == "M":
+                spt_discrete[i] = 6.5
+
+            elif item[0] == "L":
+                spt_discrete[i] = 7.5
+
+            elif item[0] == "T":
+                spt_discrete[i] = 8.5
+
+            elif item[0] == "Y":
+                spt_discrete[i] = 9.5
+
+            else:
+                spt_discrete[i] = np.nan
+
+        for i, item in enumerate(spt_check):
+            if field_range[0] == item:
+                spt_discrete -= float(i)
+                break
+
+    set_to_nan = spt_discrete < 0.0
+    spt_discrete[set_to_nan] = np.nan
+
+    return spt_discrete
 
 
 @typechecked
 def update_labels(param: List[str], object_type: str = "planet") -> List[str]:
     """
-    Function for formatting the model parameters to use them as labels
-    in the posterior plot.
+    Function for formatting the model parameters to use them
+    as labels in the posterior plot.
 
     Parameters
     ----------
     param : list
         List with names of the model parameters.
     object_type : str
         Object type ('planet' or 'star'). With 'planet', the radius
@@ -263,37 +322,41 @@
         param[index] = r"C/O"
 
     if "radius" in param:
         index = param.index("radius")
         if object_type == "planet":
             param[index] = r"$R$ ($R_\mathrm{J}$)"
         elif object_type == "star":
-            param[index] = r"$R$ ($R_\mathrm{\odot}$)"
+            param[index] = r"$R_\ast$ ($R_\mathrm{\odot}$)"
 
     if "distance" in param:
         index = param.index("distance")
         param[index] = "$d$ (pc)"
 
     if "parallax" in param:
         index = param.index("parallax")
         param[index] = r"$\varpi$ (mas)"
 
+    if "vsini" in param:
+        index = param.index("vsini")
+        param[index] = r"$v\,\sin\,i$ (km s$^{-1}$)"
+
     if "mass" in param:
         index = param.index("mass")
         if object_type == "planet":
             param[index] = r"$M$ ($M_\mathrm{J}$)"
         elif object_type == "star":
-            param[index] = r"$M$ ($M_\mathrm{\odot}$)"
+            param[index] = r"$M_\ast$ ($M_\mathrm{\odot}$)"
 
     if "log_mass" in param:
         index = param.index("log_mass")
         if object_type == "planet":
             param[index] = r"$\log\,M/M_\mathrm{J}$"
         elif object_type == "star":
-            param[index] = r"$\log\,M/M_\mathrm{\odot}$"
+            param[index] = r"$\log\,M_\ast/M_\mathrm{\odot}$"
 
     if "age" in param:
         index = param.index("age")
         param[index] = "Age (Myr)"
 
     if "mass_1" in param:
         index = param.index("mass_1")
@@ -341,15 +404,18 @@
 
     if "mcore_2" in param:
         index = param.index("mcore_2")
         param[index] = r"$M_\mathrm{core,c}$ ($M_\mathrm{E}$)"
 
     if "luminosity" in param:
         index = param.index("luminosity")
-        param[index] = r"$\log\,L/L_\mathrm{\odot}$"
+        if object_type == "planet":
+            param[index] = r"$\log\,L/L_\mathrm{\odot}$"
+        elif object_type == "star":
+            param[index] = r"$\log\,L_\ast/L_\mathrm{\odot}$"
 
     if "luminosity_ratio" in param:
         index = param.index("luminosity_ratio")
         param[index] = r"$\log\,L_\mathrm{1}/L_\mathrm{2}$"
 
     if "luminosity_disk_planet" in param:
         index = param.index("luminosity_disk_planet")
@@ -387,14 +453,21 @@
         index = param.index("ism_ext")
         param[index] = r"$A_V$"
 
     if "ism_red" in param:
         index = param.index("ism_red")
         param[index] = r"$R_V$"
 
+    for item in param:
+        if item.startswith("phot_ext_"):
+            index = param.index(item)
+            filter_name = item[9:].split("/")[1]
+            param[index] = rf"$A_\mathrm{{{filter_name}}}$"
+            break
+
     if "tint" in param:
         index = param.index("tint")
         param[index] = r"$T_\mathrm{int}$ (K)"
 
     for i in range(15):
         if f"t{i}" in param:
             index = param.index(f"t{i}")
@@ -429,16 +502,15 @@
         index = param.index("kzz")
         param[index] = r"$\log\,K_\mathrm{zz}$"
 
     for i, item in enumerate(cloud_species):
         if f"{item}_fraction" in param:
             index = param.index(f"{item}_fraction")
             param[index] = (
-                rf"$\log\,\tilde{{\mathrm{{X}}}}"
-                rf"_\mathrm{{{cloud_labels[i]}}}$"
+                rf"$\log\,\tilde{{\mathrm{{X}}}}" rf"_\mathrm{{{cloud_labels[i]}}}$"
             )
 
         if f"{item}_tau" in param:
             index = param.index(f"{item}_tau")
             param[index] = rf"$\bar{{\tau}}_\mathrm{{{cloud_labels[i]}}}$"
 
     for i, item_i in enumerate(cloud_species):
@@ -465,14 +537,20 @@
 
         elif item[0:6] == "error_":
             item_name = item[6:]
             if item_name.find("\\_") == -1 and item_name.find("_") > 0:
                 item_name = item_name.replace("_", "\\_")
             param[i] = rf"$b_\mathrm{{{item_name}}}$"
 
+        elif item[0:7] == "radvel_":
+            item_name = item[7:]
+            if item_name.find("\\_") == -1 and item_name.find("_") > 0:
+                item_name = item_name.replace("_", "\\_")
+            param[i] = rf"RV$_\mathrm{{{item_name}}}$ (km s$^{{-1}}$)"
+
         elif item[0:11] == "wavelength_":
             item_name = item[11:]
             if item_name.find("\\_") == -1 and item_name.find("_") > 0:
                 item_name = item_name.replace("_", "\\_")
             param[i] = rf"$c_\mathrm{{{item_name}}}$ (nm)"
 
         elif item[-6:] == "_error":
@@ -716,14 +794,23 @@
 
     elif in_name == "ames-dusty":
         out_name = "AMES-Dusty"
 
     elif in_name == "atmo":
         out_name = "ATMO"
 
+    elif in_name == "atmo-ceq":
+        out_name = "ATMO CEQ"
+
+    elif in_name == "atmo-neq-weak":
+        out_name = "ATMO NEQ weak"
+
+    elif in_name == "atmo-neq-strong":
+        out_name = "ATMO NEQ strong"
+
     elif in_name == "bt-cond":
         out_name = "BT-Cond"
 
     elif in_name == "bt-cond-feh":
         out_name = "BT-Cond"
 
     elif in_name == "bt-settl":
@@ -765,15 +852,21 @@
     elif in_name == "sonora-bobcat-co":
         out_name = "Sonora Bobcat C/O"
 
     elif in_name == "petitradtrans":
         out_name = "petitRADTRANS"
 
     else:
-        raise ValueError(f"The model name '{in_name}' is not known.")
+        out_name = in_name
+
+        warnings.warn(
+            f"The model name '{in_name}' is not known "
+            "so the output name will not get adjusted "
+            "for plot purposes"
+        )
 
     return out_name
 
 
 @typechecked
 def quantity_unit(
     param: List[str], object_type: str
@@ -835,19 +928,19 @@
             label.append("C/O")
 
         if item == "radius":
             quantity.append("radius")
 
             if object_type == "planet":
                 unit.append(r"$R_\mathrm{J}$")
+                label.append(r"$R$")
 
             elif object_type == "star":
                 unit.append(r"$R_\mathrm{\odot}$")
-
-            label.append(r"$R$")
+                label.append(r"$R_\ast$")
 
         for i in range(100):
             if item == f"teff_{i}":
                 quantity.append(f"teff_{i}")
                 unit.append("K")
                 label.append(rf"$T_\mathrm{{{i+1}}}$")
 
@@ -875,19 +968,19 @@
             label.append(r"$d$")
 
         if item == "mass":
             quantity.append("mass")
 
             if object_type == "planet":
                 unit.append(r"$M_\mathrm{J}$")
+                label.append(r"$M$")
 
             elif object_type == "star":
                 unit.append(r"$M_\mathrm{\odot}$")
-
-            label.append("M")
+                label.append(r"$M_\ast$")
 
         if item == "luminosity":
             quantity.append("luminosity")
             unit.append(None)
             label.append(r"$\log\,L/L_\mathrm{\odot}$")
 
         if item == "ism_ext":
@@ -901,82 +994,216 @@
             label.append(r"$A_V$")
 
         if item == "powerlaw_ext":
             quantity.append("powerlaw_ext")
             unit.append(None)
             label.append(r"$A_V$")
 
+        if item.startswith("phot_ext_"):
+            quantity.append(item)
+            unit.append(None)
+            filter_name = item[9:].split("/")[1]
+            label.append(rf"$A_\mathrm{{{filter_name}}}$")
+
         if item == "pt_smooth":
             quantity.append("pt_smooth")
             unit.append(None)
             label.append(r"$\sigma_\mathrm{P-T}$")
 
     return quantity, unit, label
 
 
-def field_bounds_ticks(field_range):
+@typechecked
+def field_bounds_ticks(
+    field_range: Tuple[str, str],
+    check_subclass: bool,
+) -> Tuple[np.ndarray, np.ndarray, List[str]]:
     """
+    Function for converting the specified field range into boundaries
+    and labels for the discrete colorbar that is plotted with a
+    color-magnitude or color-color diagram.
+
     Parameters
     ----------
-    field_range : tuple(str, str), None
-        Range of the discrete colorbar for the field dwarfs. The tuple
+    field_range : tuple(str, str)
+        Range of the discrete colorbar for the field objects. The tuple
         should contain the lower and upper value ('early M', 'late M',
-        'early L', 'late L', 'early T', 'late T', 'early Y). The full
-        range is used if set to None.
+        'early L', 'late L', 'early T', 'late T', 'early Y). Also
+        stellar spectral types can be specified.
+    check_subclass : bool
+        Set to ``True`` if the discrete colorbar should distinguish
+        early and late spectral types with different colors or set
+        to ``False`` if subclasses should not be distinguished.
 
     Returns
     -------
     np.ndarray
+        Array with the boundaries for the discrete colorbar.
     np.ndarray
-    list(str, )
+        Array with the midpoints for the discrete colorbar.
+    list(str)
+        List with the tick labels for the discrete colorbar.
     """
 
-    spectral_ranges = ["M0-M4", "M5-M9", "L0-L4", "L5-L9", "T0-T4", "T5-T9", "Y1-Y2"]
+    if check_subclass:
+        spectral_ranges = [
+            "O0-O4",
+            "O5-O9",
+            "B0-B4",
+            "B5-B9",
+            "A0-A4",
+            "A5-A9",
+            "F0-F4",
+            "F5-F9",
+            "G0-G4",
+            "G5-G9",
+            "K0-K4",
+            "K5-K9",
+            "M0-M4",
+            "M5-M9",
+            "L0-L4",
+            "L5-L9",
+            "T0-T4",
+            "T5-T9",
+            "Y1-Y2",
+        ]
+
+        if field_range[0] == "early O":
+            index_start = 0
+        elif field_range[0] == "late O":
+            index_start = 1
+        elif field_range[0] == "early B":
+            index_start = 2
+        elif field_range[0] == "late B":
+            index_start = 3
+        elif field_range[0] == "early A":
+            index_start = 4
+        elif field_range[0] == "late A":
+            index_start = 5
+        elif field_range[0] == "early F":
+            index_start = 6
+        elif field_range[0] == "late F":
+            index_start = 7
+        elif field_range[0] == "early G":
+            index_start = 8
+        elif field_range[0] == "late G":
+            index_start = 9
+        elif field_range[0] == "early K":
+            index_start = 10
+        elif field_range[0] == "late K":
+            index_start = 11
+        elif field_range[0] == "early M":
+            index_start = 12
+        elif field_range[0] == "late M":
+            index_start = 13
+        elif field_range[0] == "early L":
+            index_start = 14
+        elif field_range[0] == "late L":
+            index_start = 15
+        elif field_range[0] == "early T":
+            index_start = 16
+        elif field_range[0] == "late T":
+            index_start = 17
+        elif field_range[0] == "early Y":
+            index_start = 18
 
-    if field_range is None:
-        index_start = 0
-        index_end = 7
+        if field_range[1] == "early O":
+            index_end = 1
+        elif field_range[1] == "late O":
+            index_end = 2
+        elif field_range[1] == "early B":
+            index_end = 3
+        elif field_range[1] == "late B":
+            index_end = 4
+        elif field_range[1] == "early A":
+            index_end = 5
+        elif field_range[1] == "late A":
+            index_end = 6
+        elif field_range[1] == "early F":
+            index_end = 7
+        elif field_range[1] == "late F":
+            index_end = 8
+        elif field_range[1] == "early G":
+            index_end = 9
+        elif field_range[1] == "late G":
+            index_end = 10
+        elif field_range[1] == "early K":
+            index_end = 11
+        elif field_range[1] == "late K":
+            index_end = 12
+        elif field_range[1] == "early M":
+            index_end = 13
+        elif field_range[1] == "late M":
+            index_end = 14
+        elif field_range[1] == "early L":
+            index_end = 15
+        elif field_range[1] == "late L":
+            index_end = 16
+        elif field_range[1] == "early T":
+            index_end = 17
+        elif field_range[1] == "late T":
+            index_end = 18
+        elif field_range[1] == "early Y":
+            index_end = 19
 
     else:
-        if field_range[0] == "early M":
+        spectral_ranges = ["O", "B", "A", "F", "G", "K", "M", "L", "T", "Y"]
+
+        if field_range[0] == "O":
             index_start = 0
-        elif field_range[0] == "late M":
+        elif field_range[0] == "B":
             index_start = 1
-        elif field_range[0] == "early L":
+        elif field_range[0] == "A":
             index_start = 2
-        elif field_range[0] == "late L":
+        elif field_range[0] == "F":
             index_start = 3
-        elif field_range[0] == "early T":
+        elif field_range[0] == "G":
             index_start = 4
-        elif field_range[0] == "late T":
+        elif field_range[0] == "K":
             index_start = 5
-        elif field_range[0] == "early Y":
+        elif field_range[0] == "M":
             index_start = 6
+        elif field_range[0] == "L":
+            index_start = 7
+        elif field_range[0] == "T":
+            index_start = 8
+        elif field_range[0] == "Y":
+            index_start = 9
 
-        if field_range[1] == "early M":
+        if field_range[1] == "O":
             index_end = 1
-        elif field_range[1] == "late M":
+        elif field_range[1] == "B":
             index_end = 2
-        elif field_range[1] == "early L":
+        elif field_range[1] == "A":
             index_end = 3
-        elif field_range[1] == "late L":
+        elif field_range[1] == "F":
             index_end = 4
-        elif field_range[1] == "early T":
+        elif field_range[1] == "G":
             index_end = 5
-        elif field_range[1] == "late T":
+        elif field_range[1] == "K":
             index_end = 6
-        elif field_range[1] == "early Y":
+        elif field_range[1] == "M":
             index_end = 7
+        elif field_range[1] == "L":
+            index_end = 8
+        elif field_range[1] == "T":
+            index_end = 9
+        elif field_range[1] == "Y":
+            index_end = 10
 
     index_range = index_end - index_start + 1
 
     bounds = np.linspace(index_start, index_end, index_range)
     ticks = np.linspace(index_start + 0.5, index_end - 0.5, index_range - 1)
+
     labels = spectral_ranges[index_start:index_end]
 
+    ticks -= bounds[0]
+    bounds -= bounds[0]
+
     return bounds, ticks, labels
 
 
 @typechecked
 def remove_color_duplicates(
     object_names: List[str], empirical_names: np.ndarray
 ) -> List[int]:
```

### Comparing `species-0.5.5/species/util/query_util.py` & `species-0.6.0/species/util/query_util.py`

 * *Files identical despite different names*

### Comparing `species-0.5.5/species/util/read_util.py` & `species-0.6.0/species/util/read_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,16 +63,16 @@
     Returns
     -------
     float, np.ndarray
         Radius (Rjup).
     """
 
     surface_grav = 1e-2 * 10.0**logg  # (m s-2)
-    mass *= constants.M_JUP  # (kg)
-    radius = np.sqrt(mass * constants.GRAVITY / surface_grav)  # (m)
+    mass_kg = mass * constants.M_JUP  # (kg)
+    radius = np.sqrt(mass_kg * constants.GRAVITY / surface_grav)  # (m)
 
     return radius / constants.R_JUP
 
 
 def add_luminosity(modelbox):
     """
     Function to add the luminosity of a model spectrum to the parameter
@@ -177,15 +177,14 @@
         "The update_spectra function is deprecated and "
         "will be removed in a future release. Please use "
         "the update_objectbox function instead.",
         DeprecationWarning,
     )
 
     if objectbox.flux is not None:
-
         for key, value in objectbox.flux.items():
             if f"{key}_error" in model_param:
                 var_add = model_param[f"{key}_error"] ** 2 * value[0] ** 2
 
                 message = (
                     f"Inflating the error of {key} "
                     + f"(W m-2 um-1): {np.sqrt(var_add):.2e}..."
@@ -294,15 +293,14 @@
     -------
     species.core.box.ObjectBox
         The input box which includes the spectra with the scaled fluxes
         and/or inflated errors.
     """
 
     if objectbox.flux is not None:
-
         for key, value in objectbox.flux.items():
             instr_name = key.split(".")[0]
 
             if f"{key}_error" in model_param:
                 # Inflate photometric error of filter
                 var_add = model_param[f"{key}_error"] ** 2 * value[0] ** 2
 
@@ -382,14 +380,32 @@
 
                     print(log_msg, end="", flush=True)
                     spec_tmp[:, 2] = np.sqrt(
                         spec_tmp[:, 2] ** 2 + (err_scaling * model_box.flux) ** 2
                     )
                     print(" [DONE]")
 
+            if f"radvel_{key}" in model_param:
+                # Shift the wavelengths of the data by
+                # the radial velocity in opposite direction
+                wavel_shift = (
+                    -1.
+                    * model_param[f"radvel_{key}"]
+                    * 1e3
+                    * spec_tmp[:, 0]
+                    / constants.LIGHT
+                )
+                print(
+                    f"Mean wavelength shift (nm) for {key}: {np.mean(wavel_shift)*1e3:.2f}...",
+                    end="",
+                    flush=True,
+                )
+                spec_tmp[:, 0] += wavel_shift
+                print(" [DONE]")
+
             # Store the spectra with the scaled fluxes and/or errors
             # The other three elements (i.e. the covariance matrix,
             # the inverted covariance matrix, and the spectral
             # resolution) remain unaffected
             objectbox.spectrum[key] = (spec_tmp, value[1], value[2], value[3])
 
     return objectbox
@@ -570,15 +586,15 @@
         + model_param["log_powerlaw_b"]
         * np.log10(wavel) ** model_param["log_powerlaw_c"]
     )
 
     model_box = box.create_box(
         boxtype="model",
         model="powerlaw",
-        wavelength=1e-3*wavel,  # (um)
+        wavelength=1e-3 * wavel,  # (um)
         flux=10.0**log_flux,  # (W m-2 um-1)
         parameters=model_param,
         quantity="flux",
     )
 
     return model_box
 
@@ -678,12 +694,20 @@
     for key, value in param_dict.items():
         if star_index == 0 and key[-1] == "0":
             new_dict[key[:-2]] = value
 
         elif star_index == 1 and key[-1] == "1":
             new_dict[key[:-2]] = value
 
-        elif key in ["teff", "logg", "feh", "c_o_ratio", "fsed",
-                     "radius", "distance", "parallax"]:
+        elif key in [
+            "teff",
+            "logg",
+            "feh",
+            "c_o_ratio",
+            "fsed",
+            "radius",
+            "distance",
+            "parallax",
+        ]:
             new_dict[key] = value
 
     return new_dict
```

### Comparing `species-0.5.5/species/util/retrieval_util.py` & `species-0.6.0/species/util/retrieval_util.py`

 * *Files identical despite different names*

### Comparing `species-0.5.5/species/util/test_util.py` & `species-0.6.0/species/util/test_util.py`

 * *Files identical despite different names*

### Comparing `species-0.5.5/species.egg-info/PKG-INFO` & `species-0.6.0/species.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: species
-Version: 0.5.5
+Version: 0.6.0
 Summary: Toolkit for atmospheric characterization of directly imaged exoplanets
 Home-page: https://github.com/tomasstolker/species
 Author: Tomas Stolker
 Author-email: stolker@strw.leidenuniv.nl
 License: MIT
 Project-URL: Documentation, https://species.readthedocs.io
 Keywords: species
@@ -45,15 +45,17 @@
 
 .. image:: https://img.shields.io/github/license/tomasstolker/species
    :target: https://github.com/tomasstolker/species/blob/main/LICENSE
 
 .. image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/tomasstolker/species/HEAD
 
-*species* is a toolkit for atmospheric characterization of directly imaged exoplanets. It provides a coherent framework for spectral and photometric analysis which builds on publicly-available data and models from various resources. There are tools available for both grid retrievals and free retrievals with Bayesian inference, color-magnitude and color-color diagrams, a variety of model grids, empirical spectral analysis, spectral and photometric calibration, analysis of emission lines, and synthetic photometry. The package has been released on `PyPI <https://pypi.org/project/species/>`_ and is actively developed and maintained on Github.
+*species* is a toolkit for atmospheric characterization of directly imaged exoplanets. It provides a coherent framework for spectral and photometric analysis which builds on publicly-available data and models from various resources.
+
+There are tools available for grid and free retrievals using Bayesian inference, synthetic photometry, interpolating a variety atmospheric and evolutionary model grids (including the possibility to add a custom grid), color-magnitude and color-color diagrams, empirical spectral analysis, spectral and photometric calibration, and analysis of emission lines. The package has been released on `PyPI <https://pypi.org/project/species/>`_ and is actively developed and maintained on Github.
 
 Documentation
 -------------
 
 Documentation can be found at `http://species.readthedocs.io <http://species.readthedocs.io>`_.
 
 Tutorials
@@ -70,12 +72,12 @@
 ------------
 
 Contributions are welcome so please consider `forking <https://help.github.com/en/articles/fork-a-repo>`_ the repository and creating a `pull request <https://github.com/tomasstolker/pycrires/pulls>`_. Bug reports and feature requests can be provided by creating an `issue <https://github.com/tomasstolker/pycrires/issues>`_ on the Github page.
 
 License
 -------
 
-Copyright 2018-2022 Tomas Stolker
+Copyright 2018-2023 Tomas Stolker
 
 *species* is distributed under the MIT License. See `LICENSE <https://github.com/tomasstolker/pycrires/blob/main/LICENSE>`_ for the terms and conditions.
```

### Comparing `species-0.5.5/species.egg-info/SOURCES.txt` & `species-0.6.0/species.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 species/data/__init__.py
 species/data/accretion.py
 species/data/allers2013.py
 species/data/bonnefoy2014.py
 species/data/companion_data.json
 species/data/companion_spectra.json
 species/data/companion_spectra.py
+species/data/custom_model.py
 species/data/database.py
 species/data/dust.py
 species/data/filters.py
 species/data/irtf.py
 species/data/isochrones.py
 species/data/kesseli2017.py
 species/data/leggett.py
```

