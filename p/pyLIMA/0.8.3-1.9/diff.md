# Comparing `tmp/pyLIMA-0.8.3.tar.gz` & `tmp/pyLIMA-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyLIMA-0.8.3.tar", last modified: Fri May 15 21:58:02 2020, max compression
+gzip compressed data, was "pyLIMA-1.9.tar", last modified: Wed Jun 21 23:00:15 2023, max compression
```

## Comparing `pyLIMA-0.8.3.tar` & `pyLIMA-1.9.tar`

### file list

```diff
@@ -1,34 +1,109 @@
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2020-05-15 21:58:02.624229 pyLIMA-0.8.3/
--rw-rw-r--   0 etienne   (1000) etienne   (1000)       22 2020-03-26 00:34:53.000000 pyLIMA-0.8.3/MANIFEST.in
--rw-r--r--   0 etienne   (1000) etienne   (1000)      671 2020-05-15 21:58:02.624229 pyLIMA-0.8.3/PKG-INFO
--rw-rw-r--   0 etienne   (1000) etienne   (1000)     3765 2020-03-26 00:34:53.000000 pyLIMA-0.8.3/README.md
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2020-05-15 21:58:02.608229 pyLIMA-0.8.3/pyLIMA/
--rw-rw-r--   0 etienne   (1000) etienne   (1000)       27 2020-03-26 00:34:53.000000 pyLIMA-0.8.3/pyLIMA/__init__.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2020-05-15 21:58:02.624229 pyLIMA-0.8.3/pyLIMA/data/
--rw-rw-r--   0 etienne   (1000) etienne   (1000) 21637440 2020-03-26 00:34:53.000000 pyLIMA-0.8.3/pyLIMA/data/Claret2011.fits
--rwxrwxr-x   0 etienne   (1000) etienne   (1000)   301577 2020-03-26 00:34:53.000000 pyLIMA-0.8.3/pyLIMA/data/Yoo_B0B1.dat
--rw-rw-r--   0 etienne   (1000) etienne   (1000)     8049 2020-03-26 00:34:53.000000 pyLIMA-0.8.3/pyLIMA/event.py
--rw-rw-r--   0 etienne   (1000) etienne   (1000)    19830 2020-03-26 00:34:53.000000 pyLIMA-0.8.3/pyLIMA/microlcaustics.py
--rw-rw-r--   0 etienne   (1000) etienne   (1000)    39924 2020-05-07 01:16:30.000000 pyLIMA-0.8.3/pyLIMA/microlfits.py
--rw-rw-r--   0 etienne   (1000) etienne   (1000)    17249 2020-05-07 01:01:06.000000 pyLIMA-0.8.3/pyLIMA/microlguess.py
--rw-rw-r--   0 etienne   (1000) etienne   (1000)     1410 2020-03-26 00:34:53.000000 pyLIMA-0.8.3/pyLIMA/microllimb_darkening.py
--rw-rw-r--   0 etienne   (1000) etienne   (1000)    18331 2020-03-26 00:34:53.000000 pyLIMA-0.8.3/pyLIMA/microlmagnification.py
--rw-rw-r--   0 etienne   (1000) etienne   (1000)    56777 2020-03-26 00:34:53.000000 pyLIMA-0.8.3/pyLIMA/microlmodels.py
--rw-rw-r--   0 etienne   (1000) etienne   (1000)    12900 2020-03-26 00:34:53.000000 pyLIMA-0.8.3/pyLIMA/microlorbitalmotion.py
--rw-rw-r--   0 etienne   (1000) etienne   (1000)    54452 2020-05-09 00:32:08.000000 pyLIMA-0.8.3/pyLIMA/microloutputs.py
--rw-rw-r--   0 etienne   (1000) etienne   (1000)    27819 2020-04-09 20:09:47.000000 pyLIMA-0.8.3/pyLIMA/microlparallax.py
--rw-rw-r--   0 etienne   (1000) etienne   (1000)     2892 2020-03-26 00:34:53.000000 pyLIMA-0.8.3/pyLIMA/microlpriors.py
--rw-rw-r--   0 etienne   (1000) etienne   (1000)    13901 2020-03-26 00:34:53.000000 pyLIMA-0.8.3/pyLIMA/microlsimulator.py
--rw-rw-r--   0 etienne   (1000) etienne   (1000)     4184 2020-03-26 00:34:53.000000 pyLIMA-0.8.3/pyLIMA/microlstats.py
--rw-rw-r--   0 etienne   (1000) etienne   (1000)     5191 2020-03-26 00:34:53.000000 pyLIMA-0.8.3/pyLIMA/microltoolbox.py
--rw-rw-r--   0 etienne   (1000) etienne   (1000)     6293 2020-03-26 00:34:53.000000 pyLIMA-0.8.3/pyLIMA/microlxallarap.py
--rw-rw-r--   0 etienne   (1000) etienne   (1000)     3357 2020-03-26 00:34:53.000000 pyLIMA-0.8.3/pyLIMA/stars.py
--rw-rw-r--   0 etienne   (1000) etienne   (1000)    12827 2020-05-15 21:54:00.000000 pyLIMA-0.8.3/pyLIMA/telescopes.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2020-05-15 21:58:02.612229 pyLIMA-0.8.3/pyLIMA.egg-info/
--rw-rw-r--   0 etienne   (1000) etienne   (1000)      671 2020-05-15 21:58:02.000000 pyLIMA-0.8.3/pyLIMA.egg-info/PKG-INFO
--rw-rw-r--   0 etienne   (1000) etienne   (1000)      655 2020-05-15 21:58:02.000000 pyLIMA-0.8.3/pyLIMA.egg-info/SOURCES.txt
--rw-rw-r--   0 etienne   (1000) etienne   (1000)        1 2020-05-15 21:58:02.000000 pyLIMA-0.8.3/pyLIMA.egg-info/dependency_links.txt
--rw-rw-r--   0 etienne   (1000) etienne   (1000)       84 2020-05-15 21:58:02.000000 pyLIMA-0.8.3/pyLIMA.egg-info/requires.txt
--rw-rw-r--   0 etienne   (1000) etienne   (1000)        7 2020-05-15 21:58:02.000000 pyLIMA-0.8.3/pyLIMA.egg-info/top_level.txt
--rw-r--r--   0 etienne   (1000) etienne   (1000)       38 2020-05-15 21:58:02.624229 pyLIMA-0.8.3/setup.cfg
--rw-rw-r--   0 etienne   (1000) etienne   (1000)     1036 2020-05-15 21:55:14.000000 pyLIMA-0.8.3/setup.py
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-06-21 23:00:15.478150 pyLIMA-1.9/
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)    35141 2022-11-22 10:52:02.000000 pyLIMA-1.9/LICENSE
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)       22 2022-11-22 10:52:02.000000 pyLIMA-1.9/MANIFEST.in
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     2598 2023-06-21 23:00:15.478150 pyLIMA-1.9/PKG-INFO
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     1900 2023-06-21 22:36:32.000000 pyLIMA-1.9/README.md
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-06-21 23:00:15.454149 pyLIMA-1.9/pyLIMA/
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)      113 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/__init__.py
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-06-21 23:00:15.454149 pyLIMA-1.9/pyLIMA/astrometry/
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)        0 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/astrometry/__init__.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     5426 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/astrometry/astrometric_positions.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     1524 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/astrometry/astrometric_shifts.py
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-06-21 23:00:15.454149 pyLIMA-1.9/pyLIMA/caustics/
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)        0 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/caustics/__init__.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)    17278 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/caustics/binary_caustics.py
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-06-21 23:00:15.470149 pyLIMA-1.9/pyLIMA/data/
+-rw-rw-r--   0 etienne   (1000) etienne   (1000) 21637440 2022-11-22 10:52:02.000000 pyLIMA-1.9/pyLIMA/data/Claret2011.fits
+-rwxrwxr-x   0 etienne   (1000) etienne   (1000)   301577 2022-11-22 10:52:02.000000 pyLIMA-1.9/pyLIMA/data/Yoo_B0B1.dat
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     5739 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/event.py
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-06-21 23:00:15.470149 pyLIMA-1.9/pyLIMA/fits/
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     3608 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/fits/BOOTSTRAP_fit.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     5446 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/fits/DEMC_fit.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     7338 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/fits/DE_fit.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)    13782 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/fits/DREAM_fit.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     5678 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/fits/GRIDS_fit.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     4097 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/fits/LM_fit.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     6360 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/fits/MCMC_fit.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     2864 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/fits/MINIMIZE_fit.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)    41444 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/fits/ML_fit.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     2726 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/fits/NGSA2_fit.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     2549 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/fits/TRF_fit.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)      463 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/fits/__init__.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     1006 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/fits/fit_metrics.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     6860 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/fits/objective_functions.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     4201 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/fits/stats.py
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-06-21 23:00:15.470149 pyLIMA-1.9/pyLIMA/magnification/
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)        0 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/magnification/__init__.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)      419 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/magnification/impact_parameter.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     3120 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/magnification/magnification_FSPL.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     6034 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/magnification/magnification_Jacobian.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     1203 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/magnification/magnification_PSPL.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     4919 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/magnification/magnification_VBB.py
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-06-21 23:00:15.474149 pyLIMA-1.9/pyLIMA/models/
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     2424 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/models/DFSPL_model.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     3452 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/models/DSPL_model.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     1591 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/models/FSBL_model.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     2667 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/models/FSPL_model.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     1455 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/models/FSPLarge_model.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)    30033 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/models/ML_model.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     1520 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/models/PSBL_model.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     4509 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/models/PSPL_model.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     4634 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/models/USBL_model.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)      414 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/models/__init__.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)      974 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/models/generate_model.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     1889 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/models/pyLIMA_fancy_parameters.py
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-06-21 23:00:15.474149 pyLIMA-1.9/pyLIMA/orbitalmotion/
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)        0 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/orbitalmotion/__init__.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     1796 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/orbitalmotion/orbital_motion.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     1127 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/orbitalmotion/orbital_motion_2D.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     8753 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/orbitalmotion/orbital_motion_3D.py
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-06-21 23:00:15.474149 pyLIMA-1.9/pyLIMA/outputs/
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)        0 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/outputs/__init__.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     3072 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/outputs/file_outputs.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)    53436 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/outputs/pyLIMA_plots.py
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-06-21 23:00:15.474149 pyLIMA-1.9/pyLIMA/parallax/
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     3161 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/parallax/JPL_ephemerides.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)        0 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/parallax/__init__.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)      516 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/parallax/astropy_ephemerides.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     8892 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/parallax/parallax.py
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-06-21 23:00:15.474149 pyLIMA-1.9/pyLIMA/priors/
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)        0 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/priors/__init__.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     9448 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/priors/guess.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     6026 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/priors/parameters_boundaries.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     1624 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/priors/parameters_priors.py
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-06-21 23:00:15.474149 pyLIMA-1.9/pyLIMA/simulations/
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)        0 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/simulations/__init__.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)    14022 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/simulations/simulator.py
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-06-21 23:00:15.474149 pyLIMA-1.9/pyLIMA/stars/
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)        0 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/stars/__init__.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     1433 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/stars/limb_darkening.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     3636 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/stars/stars.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)    16536 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/telescopes.py
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-06-21 23:00:15.478150 pyLIMA-1.9/pyLIMA/tests/
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     8923 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/tests/test_astrometry.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     6827 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/tests/test_caustics.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     1655 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/tests/test_event.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)    53228 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/tests/test_fits.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     5838 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/tests/test_magnification.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)    11882 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/tests/test_model.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     5161 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/tests/test_orbital_motion.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     9143 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/tests/test_parallax.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     3999 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/tests/test_priors.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)    14053 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/tests/test_simulations.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     5932 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/tests/test_telescopes.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)      937 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/tests/test_toolbox.py
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-06-21 23:00:15.478150 pyLIMA-1.9/pyLIMA/toolbox/
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)        0 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/toolbox/__init__.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     2342 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/toolbox/brightness_transformation.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     1238 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/toolbox/fake_telescopes.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     1347 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/toolbox/limb_darkening_table.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     1473 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/toolbox/plots.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     1675 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyLIMA/toolbox/time_series.py
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-06-21 23:00:15.454149 pyLIMA-1.9/pyLIMA.egg-info/
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     2598 2023-06-21 23:00:15.000000 pyLIMA-1.9/pyLIMA.egg-info/PKG-INFO
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     2659 2023-06-21 23:00:15.000000 pyLIMA-1.9/pyLIMA.egg-info/SOURCES.txt
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)        1 2023-06-21 23:00:15.000000 pyLIMA-1.9/pyLIMA.egg-info/dependency_links.txt
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)      127 2023-06-21 23:00:15.000000 pyLIMA-1.9/pyLIMA.egg-info/requires.txt
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)        7 2023-06-21 23:00:15.000000 pyLIMA-1.9/pyLIMA.egg-info/top_level.txt
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     1090 2023-06-21 22:36:32.000000 pyLIMA-1.9/pyproject.toml
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)       38 2023-06-21 23:00:15.478150 pyLIMA-1.9/setup.cfg
```

### Comparing `pyLIMA-0.8.3/pyLIMA/data/Claret2011.fits` & `pyLIMA-1.9/pyLIMA/data/Claret2011.fits`

 * *Files identical despite different names*

### Comparing `pyLIMA-0.8.3/pyLIMA/data/Yoo_B0B1.dat` & `pyLIMA-1.9/pyLIMA/data/Yoo_B0B1.dat`

 * *Files identical despite different names*

### Comparing `pyLIMA-0.8.3/pyLIMA/microllimb_darkening.py` & `pyLIMA-1.9/pyLIMA/stars/limb_darkening.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 """
 Created on Thu Aug 27 16:39:32 2015
 
 @author: ebachelet
 """
 import collections
 import contextlib
+
 try:
     import StringIO
 except ImportError:
     import io as StringIO
 
-
-_CLARET_COLUMNS = 'log_g, Teff, metallicity, microturbulent_velocity, linear_limb_darkening, ' \
+_CLARET_COLUMNS = 'log_g, Teff, metallicity, microturbulent_velocity, ' \
+                  'linear_limb_darkening, ' \
                   'filter, method, model'
 _ClaretType = collections.namedtuple('ClaretType', _CLARET_COLUMNS)
 
 
 def read_claret_data(file_name, camera_filter):
     """
     Read in claret data from file.
```

### Comparing `pyLIMA-0.8.3/pyLIMA/microloutputs.py` & `pyLIMA-1.9/pyLIMA/outputs/pyLIMA_plots.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,1334 +1,1261 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Mon Nov  9 16:38:14 2015
-
-@author: ebachelet
-"""
-from __future__ import division
-from datetime import datetime
-from collections import OrderedDict
-import collections
-import copy
-import json
+import sys
+
 import cycler
 import matplotlib
 import matplotlib.pyplot as plt
-from matplotlib.ticker import MaxNLocator, MultipleLocator
-from matplotlib.ticker import FormatStrFormatter
-from matplotlib.colors import LogNorm
-from matplotlib.font_manager import FontProperties
-
-from bokeh.io import output_file, show
-from bokeh.layouts import gridplot, grid, layout, row
-from bokeh.plotting import figure, curdoc
-from bokeh.transform import linear_cmap, log_cmap
-from bokeh.util.hex import hexbin
-from bokeh.models import BasicTickFormatter
-from bokeh.models.widgets import DataTable, DateFormatter, TableColumn
-from bokeh.models import ColumnDataSource
-from bokeh.models import Arrow, OpenHead
-from bokeh.models.markers import Circle
-
 import numpy as np
-from astropy.time import Time
-from scipy.stats.distributions import t as student
-import os
-import json
-
-from pyLIMA import microltoolbox
-from pyLIMA import microlstats
-from pyLIMA import microlcaustics
+import pyLIMA.fits.objective_functions
+import pygtc
+from bokeh.layouts import gridplot
+from bokeh.models import Arrow, OpenHead
+from bokeh.models import BasicTickFormatter
+from bokeh.plotting import figure
+from matplotlib.ticker import MaxNLocator
+from pyLIMA.astrometry import astrometric_positions
+from pyLIMA.parallax import parallax
+from pyLIMA.toolbox import fake_telescopes, plots
 
 plot_lightcurve_windows = 0.2
 plot_residuals_windows = 0.21
 MAX_PLOT_TICKS = 2
-MARKER_SYMBOLS = np.array([['o', '.', '*', 'v', '^', '<', '>', 's', 'p', 'd', 'x'] * 10])
-
-
-# plt.style.use('ggplot')
-
-def json_output(fit, output_directory):
-
-    errors = fit_errors(fit, fit.fit_covariance)
-
-    fit_results = {}
-    source_fluxes = {}	
-    source_fluxes['value'] = {}	
-    blend_fluxes = {}
-    blend_fluxes['value'] = {}	
-    for index, key in enumerate(fit.model.model_dictionnary):
-
-        value = fit.fit_results[index]
-        param_dic = {}
-        param_dic['value'] = value
-        param_dic['comment'] = ''
-        param_dic['format'] = 'float'
-        param_dic['unit'] = ''
-        
-        if index < len(fit.model.parameters_boundaries):
-    
-            fit_results[key] = param_dic
-        else:
-            
-            if key[:3] == 'fs_':
-                 
-               source_fluxes['value'][key]=value 
-
-            else:
-
-                blend_fluxes['value'][key]=value 
-    
-
-    fit_results['source_fluxes'] = source_fluxes
-    fit_results['blend_fluxes'] = blend_fluxes
-
-    source_fluxes_errors = {}
-    source_fluxes_errors['value'] = {}
-    blend_fluxes_errors = {}
-    blend_fluxes_errors['value'] = {}
-    for index, key in enumerate(fit.model.model_dictionnary):
-        
-        value = getattr(errors,'err_'+key)
-
-        error_dic = {}
-        error_dic['value'] = value
-        error_dic['comment'] = ''
-        error_dic['format'] = 'float'
-        error_dic['unit'] = ''
-
-        if index < len(fit.model.parameters_boundaries):
-    
-            fit_results['sig_'+key] = param_dic
-        else:
-            
-            if key[:3] == 'fs_':
-                 
-               source_fluxes_errors['value'][key]=value 
-
-            else:
-
-               blend_fluxes_errors['value'][key]=value 
-
-    fit_results['sig_source_fluxes'] = source_fluxes_errors
-    fit_results['sig_blend_fluxes'] = blend_fluxes_errors
-    with open( output_directory+fit.event.name+'_.json', 'w') as outfile:
-        json.dump(fit_results, outfile)
-
-def latex_output(fit, output_directory):
-    """Function to output a LaTeX format table of the fit parameters"""
-
-    event_name = fit.event.name
-    fit_type = fit.method
-
-    file_path = os.path.join(output_directory, event_name + '_' + fit_type + '_results.tex')
-
-    t = open(file_path, 'w')
-
-    t.write('\\begin{table}[h!]\n')
-    t.write('\\centering\n')
-    t.write(
-        '\\caption{Best model parameters} \label{tab:fitparams}\n')
-    t.write('\\begin{tabular}{lll}\n')
-    t.write('\\hline\n')
-    t.write('\\hline\n')
+MARKER_SYMBOLS = np.array(
+    [['o', '.', '*', 'v', '^', '<', '>', 's', 'p', 'd', 'x'] * 10])
 
-    if fit_type == 'MCMC':
-        t.write('Parameters&Value(best model)&Errors([16,50,84] range)')
-        t.write('\\hline\n')
+# this is a pointer to the module object instance itself.
+thismodule = sys.modules[__name__]
 
-        mcmc_chains = fit.MCMC_chains
-        best_model_index = np.argmax(mcmc_chains[:, -1])
+thismodule.list_of_fake_telescopes = []
+thismodule.saved_model = None
 
-        for index, key in enumerate(fit.model.model_dictionnary):
-            best_param = mcmc_chains[best_model_index, index]
-            percent_34 = np.percentile(mcmc_chains[:, index], 16)
-            percent_50 = np.percentile(mcmc_chains[:, index], 50)
-            percent_84 = np.percentile(mcmc_chains[:, index], 84)
 
-            t.write(
-                key + '&' + str(best_param) + '&[' + str(percent_34) + ',' + str(percent_50) + ',' + str(
-                    percent_84) + ']\\\\\n')
+def create_telescopes_to_plot_model(microlensing_model, pyLIMA_parameters):
+    if microlensing_model == thismodule.saved_model:
 
-        t.write('Chi2&' + str(-2 * mcmc_chains[best_model_index, -1]) + '&0\\\\\n')
+        list_of_fake_telescopes = thismodule.list_of_fake_telescopes
 
     else:
-        t.write('Parameters&Value&Errors')
-        t.write('\\hline\n')
 
-        for index, key in enumerate(fit.model.model_dictionnary):
-            t.write(key + '&' + str(fit.fit_results[index]) + '&' + str(
-                fit.fit_covariance.diagonal()[index] ** 0.5) + '\\\\\n')
+        list_of_fake_telescopes = []
 
-        t.write('Chi2&' + str(fit.fit_results[-1]) + '&0\\\\\n')
+    if len(list_of_fake_telescopes) == 0:
 
-    t.write('\\hline\n')
-    t.write('\\end{tabular}\n')
-    t.write('\\end{table}\n')
+        # Photometry first
+        Earth = True
 
-    t.close()
+        for tel in microlensing_model.event.telescopes:
 
+            if tel.lightcurve_flux is not None:
 
-def pdf_output(fit, output_directory):
-    from matplotlib.backends.backend_pdf import PdfPages
-    with PdfPages(output_directory + fit.event.name + '.pdf') as pdf:
-        figure_1 = fit.outputs.figure_lightcurve
-        pdf.savefig(figure_1)
+                if tel.location == 'Space':
+                    model_time = np.arange(
+                        np.min(tel.lightcurve_magnitude['time'].value),
+                        np.max(tel.lightcurve_magnitude['time'].value),
+                        0.1).round(2)
 
-        figure_2 = fit.outputs.figure_geometry
-        pdf.savefig(figure_2)
+                    model_time = np.r_[
+                        model_time, tel.lightcurve_magnitude['time'].value]
 
-        if 'figure_distributions' in fit.outputs._fields:
-            figure_3 = fit.outputs.figure_distributions
-            pdf.savefig(figure_3)
-        pdf_details = pdf.infodict()
-        pdf_details['Title'] = fit.event.name + '_pyLIMA'
-        pdf_details['Author'] = 'Produced by pyLIMA'
-        pdf_details['Subject'] = 'A microlensing fit'
+                    model_time.sort()
 
-        pdf_details['CreationDate'] = datetime.today()
+                if Earth and tel.location == 'Earth':
 
+                    model_time1 = np.arange(np.min((np.min(
+                        tel.lightcurve_magnitude['time'].value),
+                                                    pyLIMA_parameters.t0 - 5 *
+                                                    pyLIMA_parameters.tE)),
+                        np.max((np.max(
+                            tel.lightcurve_magnitude['time'].value),
+                                pyLIMA_parameters.t0 + 5 *
+                                pyLIMA_parameters.tE)),
+                        1).round(2)
 
-def statistical_outputs(fit):
-    """Compute statistics to estimate the fit quality
+                    model_time2 = np.arange(
+                        pyLIMA_parameters.t0 - 1 * pyLIMA_parameters.tE,
+                        pyLIMA_parameters.t0 + 1 * pyLIMA_parameters.tE,
+                        1).round(2)
 
-        :param object fit: a fit object. See the microlfits for more details.
+                    model_time = np.r_[model_time1, model_time2]
 
-        :return: a namedtuple containing the following attributes :
+                    for telescope in microlensing_model.event.telescopes:
 
-                  fit_parameters : an namedtuple object containing all the fitted parameters
+                        if telescope.location == 'Earth':
+                            model_time = np.r_[
+                                model_time, telescope.lightcurve_magnitude[
+                                    'time'].value]
 
-                  fit_errors : an namedtuple object containing all the fitted parameters errors
+                            symmetric = 2 * pyLIMA_parameters.t0 - \
+                                        telescope.lightcurve_magnitude['time'].value
+                            model_time = np.r_[model_time, symmetric]
 
-                  fit_correlation_matrix : a numpy array representing the fitted parameters
-                  correlation matrix
+                    model_time.sort()
 
-                  figure_lightcurve : a two matplotlib figure showing the data and model and the
-                  correspoding residuals
+                if (tel.location == 'Space') | (Earth and tel.location == 'Earth'):
 
-        :rtype: object
-    """
-    fig_size = [15, 5]
-    figure_stats = plt.figure(figsize=(fig_size[0], fig_size[1]))
-
-    best_parameters = fit.fit_results
-    best_model_pyLIMA_parameters = fit.model.compute_pyLIMA_parameters(best_parameters)
+                    model_time = np.unique(model_time)
 
-    telescope_residuals = fit.all_telescope_residuals(best_model_pyLIMA_parameters)
+                    model_lightcurve = np.c_[
+                        model_time, [0] * len(model_time), [0.1] * len(model_time)]
+                    model_telescope = fake_telescopes.create_a_fake_telescope(
+                        light_curve=model_lightcurve)
 
-    telescope_Kolmogorv_Smirnov_residuals_test = []
-    telescope_Anderson_Darling_residuals_test = []
-    telescope_Shapiro_Wilk_residuals_test = []
+                    model_telescope.name = tel.name
+                    model_telescope.filter = tel.filter
+                    model_telescope.location = tel.location
+                    model_telescope.ld_gamma = tel.ld_gamma
+                    model_telescope.ld_sigma = tel.ld_sigma
+                    model_telescope.ld_a1 = tel.ld_a1
+                    model_telescope.ld_a2 = tel.ld_a2
+                    model_telescope.location = tel.location
 
-    telescope_chi2 = []
-    telescope_chi2_sur_dof = []
-    telescope_BIC = []
-    telescope_AIC = []
-    count = 0
-    for telescope in fit.event.telescopes:
-        residuals = telescope_residuals[count]
+                    if tel.location == 'Space':
+                        model_telescope.spacecraft_name = tel.spacecraft_name
+                        model_telescope.spacecraft_positions = tel.spacecraft_positions
 
-        telescope_residuals.append(residuals)
+                    if microlensing_model.parallax_model[0] != 'None':
+                        model_telescope.initialize_positions()
 
-        Kolmogorov_Smirnov = microlstats.normal_Kolmogorov_Smirnov(residuals)
+                        model_telescope.compute_parallax(
+                            microlensing_model.parallax_model,
+                            microlensing_model.event.North
+                            ,
+                            microlensing_model.event.East)  # ,
+                        # microlensing_model.event.ra/180*np.pi)
 
-        Anderson_Darling = microlstats.normal_Anderson_Darling(residuals)
+                    list_of_fake_telescopes.append(model_telescope)
 
-        Shapiro_Wilk = microlstats.normal_Shapiro_Wilk(residuals)
+                    if tel.location == 'Earth' and Earth:
+                        Earth = False
 
-        telescope_Kolmogorv_Smirnov_residuals_test.append(Kolmogorov_Smirnov)
-        telescope_Anderson_Darling_residuals_test.append(Anderson_Darling)
-        telescope_Shapiro_Wilk_residuals_test.append(Shapiro_Wilk)
+        # Astrometry
 
-        chi2_sur_dof = microlstats.normalized_chi2((residuals ** 2).sum(), len(residuals),
-                                                   len(fit.model.parameters_boundaries) + 2)
-        BIC = 0.0
-        AIC = 0.0
+        for tel in microlensing_model.event.telescopes:
 
-        telescope_chi2.append((residuals ** 2).sum())
-        telescope_chi2_sur_dof.append(chi2_sur_dof)
-        telescope_BIC.append(BIC)
-        telescope_AIC.append(AIC)
-        count += 1
-    total_residuals = fit.residuals_LM(best_parameters)
+            if tel.astrometry is not None:
 
-    Kolmogorov_Smirnov = microlstats.normal_Kolmogorov_Smirnov(total_residuals)
+                if tel.location == 'Space':
 
-    Anderson_Darling = microlstats.normal_Anderson_Darling(total_residuals)
+                    model_time = np.arange(np.min(tel.astrometry['time'].value),
+                                           np.max(tel.astrometry['time'].value),
+                                           0.1).round(2)
+                else:
 
-    Shapiro_Wilk = microlstats.normal_Shapiro_Wilk(total_residuals)
+                    model_time1 = np.arange(
+                        np.min((np.min(tel.lightcurve_magnitude['time'].value),
+                                pyLIMA_parameters.t0 - 5 * pyLIMA_parameters.tE)),
+                        np.max((np.max(tel.lightcurve_magnitude['time'].value),
+                                pyLIMA_parameters.t0 + 5 * pyLIMA_parameters.tE)),
+                        1).round(2)
 
-    telescope_Kolmogorv_Smirnov_residuals_test.append(Kolmogorov_Smirnov)
-    telescope_Anderson_Darling_residuals_test.append(Anderson_Darling)
-    telescope_Shapiro_Wilk_residuals_test.append(Shapiro_Wilk)
+                    model_time2 = np.arange(
+                        pyLIMA_parameters.t0 - 1 * pyLIMA_parameters.tE,
+                        pyLIMA_parameters.t0 + 1 * pyLIMA_parameters.tE,
+                        0.1).round(2)
 
-    chi2_sur_dof = microlstats.normalized_chi2(best_parameters[-1], len(total_residuals),
-                                               len(fit.model.parameters_boundaries) + 2)
-    BIC = microlstats.Bayesian_Information_Criterion(best_parameters[-1], len(total_residuals),
-                                                     len(fit.model.parameters_boundaries) + 2)
-    AIC = microlstats.Akaike_Information_Criterion(best_parameters[-1], len(fit.model.parameters_boundaries) + 2)
+                    model_time = np.r_[model_time1, model_time2]
 
-    telescope_chi2.append(best_parameters[-1])
-    telescope_chi2_sur_dof.append(chi2_sur_dof)
-    telescope_BIC.append(BIC)
-    telescope_AIC.append(AIC)
+                    model_time = np.r_[model_time, telescope.astrometry['time'].value]
 
-    raw_labels = [i.name for i in fit.event.telescopes]
-    raw_labels += ['All site']
-    column_labels = ['Kolmogorov-Smirnov\n(KS_stat,p_value)', 'Anderson-Darling\n(AD_stat,p value)',
-                     'Shapiro-Wilk\n(SW_stat,p_value)', 'chi2', 'chi2_dof', 'BIC', 'AIC']
-    table_val = []
-    table_colors = []
-    colors_dictionary = {0: 'r', 1: 'y', 2: 'g'}
+                    symmetric = 2 * pyLIMA_parameters.t0 - telescope.astrometry[
+                        'time'].value
+                    model_time = np.r_[model_time, symmetric]
+                    model_time.sort()
 
-    for i in range(len(raw_labels)):
-        table_val.append([np.round(telescope_Kolmogorv_Smirnov_residuals_test[i][:2], 3),
-                          np.round(telescope_Anderson_Darling_residuals_test[i][:2], 3),
-                          np.round(telescope_Shapiro_Wilk_residuals_test[i][:2], 3),
-                          np.round(telescope_chi2[i], 3), np.round(telescope_chi2_sur_dof[i][0], 3),
-                          np.round(telescope_BIC[i], 3), np.round(telescope_AIC[i], 3)])
-
-        table_colors.append([colors_dictionary[telescope_Kolmogorv_Smirnov_residuals_test[i][2]],
-                             colors_dictionary[telescope_Anderson_Darling_residuals_test[i][2]],
-                             colors_dictionary[telescope_Shapiro_Wilk_residuals_test[i][2]],
-                             'w',
-                             colors_dictionary[telescope_chi2_sur_dof[i][1]],
-                             'w',
-                             'w',
-                             ])
-
-    # table_val = np.round(table_val, 5).tolist()
-
-    table_axes = figure_stats.add_subplot(111, frameon=False)
-
-    the_table = table_axes.table(cellText=table_val,
-                                 rowLabels=raw_labels, cellColours=table_colors,
-                                 colLabels=column_labels, loc='center left')
-    table_axes.get_yaxis().set_visible(False)
-    table_axes.get_xaxis().set_visible(False)
-    the_table.auto_set_font_size(False)
-    the_table.set_fontsize(fig_size[0] * 3 / 4.0 / np.log10(len(fit.model.model_dictionnary.keys())))
-    the_table.scale(0.75, 0.75)
-    title = fit.model.event.name + ' : ' + fit.model.model_type
-    figure_stats.suptitle(title, fontsize=30 * fig_size[0] / len(title))
+                model_time = np.unique(model_time)
+                model_astrometry = np.c_[
+                    model_time, [0] * len(model_time), [0.1] * len(model_time), [
+                        0] * len(model_time), [0.1] * len(model_time)]
+                model_telescope = fake_telescopes.create_a_fake_telescope(
+                    astrometry_curve=model_astrometry,
+                    astrometry_unit=tel.astrometry['ra'].unit)
 
+                model_telescope.name = tel.name
+                model_telescope.filter = tel.filter
+                model_telescope.location = tel.location
+                model_telescope.ld_gamma = tel.ld_gamma
+                model_telescope.ld_sigma = tel.ld_sigma
+                model_telescope.ld_a1 = tel.ld_a1
+                model_telescope.ld_a2 = tel.ld_a2
+                model_telescope.pixel_scale = tel.pixel_scale
 
-def fit_outputs(fit):
-    """Standard outputs.
+                if tel.location == 'Space':
+                    model_telescope.spacecraft_name = tel.spacecraft_name
+                    model_telescope.spacecraft_positions = tel.spacecraft_positions
 
-    :param object fit: a fit object. See the microlfits for more details.
+                if microlensing_model.parallax_model[0] != 'None':
+                    model_telescope.initialize_positions()
 
-    :return: a namedtuple containing the following attributes :
+                    model_telescope.compute_parallax(microlensing_model.parallax_model,
+                                                     microlensing_model.event.North
+                                                     ,
+                                                     microlensing_model.event.East)  # ,
+                    # microlensing_model.event.ra / 180)# * np.pi)
 
-              fit_parameters : an namedtuple object containing all the fitted parameters
+                list_of_fake_telescopes.append(model_telescope)
 
-              fit_errors : an namedtuple object containing all the fitted parameters errors
+        thismodule.saved_model = microlensing_model
+        thismodule.list_of_fake_telescopes = list_of_fake_telescopes
 
-              fit_correlation_matrix : a numpy array representing the fitted parameters
-              correlation matrix
+    return list_of_fake_telescopes
 
-              figure_lightcurve : a two matplotlib figure showing the data and model and the
-              correspoding residuals
 
-    :rtype: object
+def plot_geometry(microlensing_model, model_parameters, bokeh_plot=None):
+    """Plot the lensing geometry (i.e source trajectory) and the table of best
+    parameters.
+    :param object fit: a fit object. See the microlfits for more details.
+    :param list best_parameters: a list containing the model you want to plot the
+    trajectory
     """
+
     # Change matplotlib default colors
-    n = len(fit.event.telescopes)
-    color = plt.cm.jet(np.linspace(0.01, 0.99, n))  # This returns RGBA; convert:
-    # hexcolor = map(lambda rgb: '#%02x%02x%02x' % (rgb[0] * 255, rgb[1] * 255, rgb[2] * 255),
+    n_telescopes = len(microlensing_model.event.telescopes)
+    color = plt.cm.jet(
+        np.linspace(0.01, 0.99, n_telescopes))  # This returns RGBA; convert:
+    # hexcolor = map(lambda rgb: '#%02x%02x%02x' % (rgb[0] * 255, rgb[1] * 255,
+    # rgb[2] * 255),
     #                tuple(color[:, 0:-1]))
-    hexcolor = ['#' + format(int(i[0] * 255), 'x').zfill(2) + format(int(i[1] * 255), 'x').zfill(2) +
+    hexcolor = ['#' + format(int(i[0] * 255), 'x').zfill(2) + format(int(i[1] * 255),
+                                                                     'x').zfill(2) +
                 format(int(i[2] * 255), 'x').zfill(2) for i in color]
 
     matplotlib.rcParams['axes.prop_cycle'] = cycler.cycler(color=hexcolor)
-    # hexcolor[0] = '#000000'
 
-    if (fit.method == 'LM') or (fit.method == 'TRF'):
-        # prepare a list of fake telescopes
-        create_the_fake_telescopes(fit, fit.fit_results)
-
-        results = parameters_result(fit)
-
-        figure_trajectory, bokeh_trajectory = plot_geometry(fit)
-        figure_table, bokeh_table = parameters_table(fit)
-        covariance_matrix = fit.fit_covariance
-        errors = fit_errors(fit)
-        figure_lightcurve, bokeh_lightcurve = LM_plot_lightcurves(fit)
-
-        key_outputs = ['fit_parameters', 'fit_errors', 'fit_correlation_matrix', 'figure_lightcurve', 'figure_geometry',
-                       'figure_table']
-        values_outputs = [results, errors, covariance_matrix, figure_lightcurve, figure_trajectory, figure_table]
-        bokeh_grid = gridplot(
-            [[row([bokeh_lightcurve, gridplot([[bokeh_trajectory], [bokeh_table]], toolbar_location=None)])]],
-            toolbar_location="above")
-
-    if fit.method == 'DE':
-        # prepare a list of fake telescopes
-        create_the_fake_telescopes(fit, fit.fit_results)
-
-        results = parameters_result(fit)
-        figure_trajectory, bokeh_trajectory = plot_geometry(fit)
-        figure_table, bokeh_table = parameters_table(fit)
-        covariance_matrix = fit.fit_covariance
-        errors = fit_errors(fit)
-
-        figure_lightcurve, bokeh_lightcurve = LM_plot_lightcurves(fit)
-
-        figure_distributions, bokeh_distributions = plot_distributions(fit, fit.DE_population)
-        key_outputs = ['fit_parameters', 'fit_errors', 'fit_correlation_matrix', 'figure_lightcurve', 'figure_geometry',
-                       'figure_table', 'figure_distributions']
-        values_outputs = [results, errors, covariance_matrix, figure_lightcurve, figure_trajectory, figure_table,
-                          figure_distributions]
-
-        bokeh_grid = gridplot(
-            [[row([bokeh_lightcurve, gridplot([[bokeh_trajectory], [bokeh_table]], toolbar_location=None)])]
-                , [row([bokeh_distributions])]],
-            toolbar_location="above")
-
-    if fit.method == 'MCMC':
-        mcmc_chains = fit.MCMC_chains
-
-        best_chain = copy.copy(mcmc_chains[np.argmax(mcmc_chains[:, -1])])
-        best_chain[-1] *= -2  # likelihood to chi2
-        # prepare a list of fake telescopes
-        create_the_fake_telescopes(fit, best_chain)
-
-        results = parameters_result(fit, best_chain)
-        covariance_matrix = MCMC_covariance(mcmc_chains)
-        errors = fit_errors(fit, covariance_matrix)
-
-        index = np.random.choice(range(len(mcmc_chains)), 12)
-        index = np.r_[index, np.argmax(mcmc_chains[:, -1])]
-
-        best_chains = mcmc_chains[index]
-        best_chains = best_chains[best_chains[:, -1].argsort(),]
-
-        figure_lightcurve, bokeh_lightcurve = MCMC_plot_lightcurves(fit, best_chains)
-        figure_trajectory, bokeh_trajectory = plot_geometry(fit)
-        figure_table, bokeh_table = parameters_table(fit)
-
-        figure_distributions, bokeh_distributions = plot_distributions(fit, mcmc_chains)
-
-        key_outputs = ['fit_parameters', 'fit_errors', 'fit_correlation_matrix', 'figure_lightcurve', 'figure_geometry',
-                       'figure_table', 'figure_distributions']
-        values_outputs = [results, errors, covariance_matrix, figure_lightcurve, figure_trajectory, figure_table,
-                          figure_distributions]
-
-        bokeh_grid = gridplot([[row([bokeh_lightcurve, gridplot([[bokeh_trajectory], [bokeh_table]], toolbar_location=None)])]
-                , [row([bokeh_distributions])]],
-            toolbar_location="above")
-    outputs = collections.namedtuple('Fit_outputs', key_outputs)
-
-    count = 0
-    for key in key_outputs:
-        setattr(outputs, key, values_outputs[count])
-        count += 1
-    
-    show(bokeh_grid)
-    return outputs
-
-
-def complete_MCMC_parameters(fit, parameters):
-    pyLIMA_parameters = fit.model.compute_pyLIMA_parameters(parameters)
-    chichi = parameters[-1]
-    parameters = parameters[:-1].tolist()
-    for index, telescope in enumerate(fit.event.telescopes):
-        _, fs, fb = fit.model.compute_the_microlensing_model(telescope, pyLIMA_parameters)
-        parameters.append(fs)
-        parameters.append(fb)
-
-    return parameters + [chichi]
-
-
-def create_the_fake_telescopes(fit, parameters):
-    fit.event.fake_telescopes = []
-    pyLIMA_parameters = fit.model.compute_pyLIMA_parameters(parameters)
+    pyLIMA_parameters = microlensing_model.compute_pyLIMA_parameters(model_parameters)
 
-    telescopes_ground = np.array([[i, fit.event.telescopes[i].n_data()] for i
-                                  in range(len(fit.event.telescopes)) if fit.event.telescopes[i].location == 'Earth'])
+    faketelescopes = create_telescopes_to_plot_model(microlensing_model,
+                                                     pyLIMA_parameters)
 
-    try:
+    fig_size = [10, 10]
+    figure_trajectory = plt.figure(figsize=(fig_size[0], fig_size[1]), dpi=75)
 
-        telescopes_index = [telescopes_ground[0, 0]]
-    except:
-        telescopes_index = []
-   
-    telescopes_space = [i for i in range(len(fit.event.telescopes)) if fit.event.telescopes[i].location == 'Space']
+    figure_axes = figure_trajectory.add_subplot(111, aspect=1)
+    figure_axes.set_aspect('equal', adjustable='box')
+    plt.subplots_adjust(top=0.8, bottom=0.1, left=0.2, right=0.9, wspace=0.1,
+                        hspace=0.1)
 
+    if bokeh_plot is not None:
 
-    telescopes_index += telescopes_space
+        bokeh_geometry = figure(width=600, height=600, x_range=(-3, 3), y_range=(-3, 3),
+                                x_axis_label=r'$$x [\theta_E]$$',
+                                y_axis_label=r'$$y [\theta_E]$$')
 
-    if 0 not in telescopes_index:
-        telescopes_index = np.r_[0, telescopes_index].astype(int)
+    else:
 
-    telescopes_index = np.sort(telescopes_index)
+        bokeh_geometry = None
 
-    for telescope_index in telescopes_index:
+    for telescope in faketelescopes:
 
-        reference_telescope = copy.copy(fit.event.telescopes[telescope_index])
-        telescope_time = fit.event.telescopes[telescope_index].lightcurve_flux[:, 0]
+        if telescope.lightcurve_flux is not None:
 
-        if fit.event.telescopes[telescope_index].location == 'Space':
-		
-            if np.min(telescope_time)>np.min(reference_telescope.spacecraft_positions[:,0]):
-               time_minimum = np.min(reference_telescope.spacecraft_positions[:,0])
-            else:
-               time_minimum = np.min(telescope_time)
+            platform = 'Earth'
+
+            if telescope.location == 'Space':
+
+                platform = telescope.name
+                linestyle = '--'
 
-            if np.max(telescope_time)<np.max(reference_telescope.spacecraft_positions[:,0]):
-               time_maximum = np.max(reference_telescope.spacecraft_positions[:,0])
             else:
-               time_maximum = np.max(telescope_time)
 
+                linestyle = '-'
 
-            time = np.linspace( time_minimum, time_maximum, 5000)
-        else:
-            time = np.linspace(np.min([np.min(telescope_time), pyLIMA_parameters.to - 3 * pyLIMA_parameters.tE]),
-                             np.max([np.max(telescope_time), pyLIMA_parameters.to + 3 * pyLIMA_parameters.tE]), 5000)
+            reference_telescope = telescope
 
-        reference_telescope.lightcurve_magnitude = np.array([time, [0] * len(time), [0] * len(time)]).T
-        reference_telescope.lightcurve_flux = reference_telescope.lightcurve_in_flux()
+            telescope_index = \
+                [i for i in range(len(microlensing_model.event.telescopes)) if
+                 microlensing_model.event.telescopes[i].name == telescope.name][0]
 
-        if fit.model.parallax_model[0] != 'None':
+            trajectory_x, trajectory_y, dseparation, dalpha = \
+                microlensing_model.source_trajectory(
+                    telescope, pyLIMA_parameters,
+                    data_type='photometry')
 
-            reference_telescope.compute_parallax(fit.event, fit.model.parallax_model)
+            color = plt.rcParams["axes.prop_cycle"].by_key()["color"][telescope_index]
+            figure_axes.plot(trajectory_x, trajectory_y,
+                             c=color,
+                             label=platform, linestyle=linestyle)
 
-        fit.event.fake_telescopes.append(reference_telescope)
+            if bokeh_geometry is not None:
+                bokeh_geometry.line(trajectory_x, trajectory_y,
+                                    color=color,
+                                    legend_label=platform)
 
+            for ind in [-2, -1, 0, 1, 2]:
 
-def plot_distributions(fit, mcmc_chains):
-    """ Plot the fit parameters distributions.
-        Only plot the best mcmc_chains are plotted.
-        :param fit: a fit object. See the microlfits for more details.
-        :param mcmc_best: a numpy array representing the best (<= 6 sigma) mcmc chains.
-        :return: a multiple matplotlib subplot representing the parameters distributions (2D slice +
-        histogram)
-        :rtype: matplotlib_figure
-    """
+                try:
 
-    fig_size = [10, 10]
+                    index = np.argmin(
+                        np.abs(telescope.lightcurve_magnitude['time'].value -
+                               (pyLIMA_parameters.t0 + ind * pyLIMA_parameters.tE)))
+                    sign = np.sign(trajectory_x[index + 1] - trajectory_x[index])
+                    derivative = (trajectory_y[index - 1] - trajectory_y[index + 1]) / (
+                            trajectory_x[index - 1] - trajectory_x[index + 1])
+
+                    figure_axes.annotate('',
+                                         xy=(trajectory_x[index], trajectory_y[index]),
+                                         xytext=(trajectory_x[index] - (
+                                                 trajectory_x[index + 1] -
+                                                 trajectory_x[index]) * 0.001,
+                                                 trajectory_y[index] - (
+                                                         trajectory_x[index + 1] -
+                                                         trajectory_x[
+                                                             index]) * 0.001 *
+                                                 derivative),
+                                         arrowprops=dict(arrowstyle="->",
+                                                         mutation_scale=35,
+                                                         color=color))
+
+                    if bokeh_geometry is not None:
+                        oh = OpenHead(line_color=color, line_width=1)
+
+                        bokeh_geometry.add_layout(Arrow(end=oh,
+                                                        x_start=trajectory_x[index],
+                                                        y_start=trajectory_y[index],
+                                                        x_end=trajectory_x[
+                                                                  index] + sign * 0.001,
+                                                        y_end=trajectory_y[
+                                                                  index] + sign *
+                                                              0.001 * derivative))
 
-    max_plot_ticks = MAX_PLOT_TICKS
-    dimensions = len(mcmc_chains[0]) - 1
+                except IndexError:
 
-    figure_distributions, axes = plt.subplots(dimensions, dimensions, figsize=(fig_size[0], fig_size[1]))
-    keys = list(fit.model.model_dictionnary)
+                    pass
 
-    chains = np.copy(mcmc_chains)
-    chains[:, 0] -= 2450000
+            if microlensing_model.model_type == 'DSPL':
 
-    bokeh_figs = []
-    for i in range(len(chains[0]) - 1):
-        figs_row = []
-        chain_i = chains[:, i]
-        for j in range(len(chains[0]) - 1):
-
-            chain_j = chains[:, j]
-            hex = None
-
-            if j == i:
-
-                axes[j, i].hist(chain_i, 50, histtype='step')
-                H, edges = np.histogram(chain_i, bins=50)
-                hex = figure(toolbar_location=None, width=250, height=250)
-                hex.quad(top=H, bottom=0, left=edges[:-1], right=edges[1:])
+                _, _, trajectory_x, trajectory_y = \
+                    microlensing_model.sources_trajectory(
+                        reference_telescope,
+                        pyLIMA_parameters)
+
+                figure_axes.plot(trajectory_x, trajectory_y,
+                                 c=color, alpha=0.5)
+
+                if bokeh_geometry is not None:
+                    bokeh_geometry.line(trajectory_x, trajectory_y,
+                                        color=color, alpha=0.5)
+
+    if 'BL' in microlensing_model.model_type():
+
+        from pyLIMA.caustics import binary_caustics
+
+        regime, caustics, cc = \
+            binary_caustics.find_2_lenses_caustics_and_critical_curves(
+                pyLIMA_parameters.separation,
+                pyLIMA_parameters.mass_ratio,
+                resolution=5000)
+
+        center_of_mass = pyLIMA_parameters.separation * pyLIMA_parameters.mass_ratio / (
+                1 + pyLIMA_parameters.mass_ratio)
+        plt.scatter(-center_of_mass, 0, s=10, c='k')
+        plt.scatter(-center_of_mass + pyLIMA_parameters.separation, 0, s=10, c='k')
 
-            else:
+        for count, caustic in enumerate(caustics):
 
-                axes[j, i].hist2d(chain_i, chain_j, 50, norm=LogNorm())
+            try:
+                figure_axes.plot(caustic.real, caustic.imag, lw=3, c='r')
+                figure_axes.plot(cc[count].real, cc[count].imag, '--k')
 
-            axes[j, i].yaxis.set_major_formatter(FormatStrFormatter('%.3f'))
-            axes[j, i].xaxis.set_major_formatter(FormatStrFormatter('%.3f'))
-            axes[j, i].xaxis.set_major_locator(MaxNLocator(2))
-            axes[j, i].yaxis.set_major_locator(MaxNLocator(2))
-            # axes[j, i].set_xticks([np.percentile(chain_i, 1), np.percentile(chain_i, 99)])
-            # axes[j, i].set_yticks([np.percentile(chain_j, 99), np.percentile(chain_j, 99)])
-
-            if j > i:
-                figure_distributions.delaxes(axes[i, j])
-
-            if (i == 0):
-
-                if j != len(chains[0]) - 2:
-                    axes[j, i].set_xticks([])
-
-                axes[j, i].set_ylabel(keys[j])
-
-            if j == len(chains[0]) - 2:
-
-                if i != 0:
-                    axes[j, i].set_yticks([])
-                axes[j, i].set_xlabel(keys[i])
-
-            if (i != 0) and (j != len(chains[0]) - 2):
-                axes[j, i].set_xticks([])
-                axes[j, i].set_yticks([])
-
-            if (i == 0) and (j == 0):
-                axes[j, i].set_xticks([])
-                axes[j, i].set_yticks([])
-                axes[j, i].set_ylabel(None)
-
-            if j < i:
-                H, ye, xe = np.histogram2d(chain_i, chain_j, bins=50)
-                hex = figure(x_range=(min(xe), max(xe)), y_range=(min(ye), max(ye)), toolbar_location=None, width=250,
-                             height=250)
-                hex.image(image=[np.log10(H)], x=xe[0], y=ye[0], dw=xe[-1] - xe[0], dh=ye[-1] - ye[0],
-                          color_mapper=log_cmap('counts', 'Viridis256', 0.1, np.max(np.log10(H)))['transform'])
-                # bins = hexbin(chain_i, chain_j, 0.1)
-                # hex = figure(title="Hexbin", match_aspect=True)
-                # hex.hex_tile(q="q", r="r", size=0.1, line_color=None, source=bins,
-                # fill_color=log_cmap('counts', 'Viridis256', 0, max(bins.counts)))
+                if bokeh_geometry is not None:
+                    bokeh_geometry.line(caustic.real, caustic.imag,
+                                        color='red', line_width=3)
+                    bokeh_geometry.line(cc[count].real, cc[count].imag,
+                                        line_dash='dashed',
+                                        color='black')
 
-            if (j == 0) and (i != 0):
+            except AttributeError:
 
-                try:
-                    hex.yaxis.axis_label = keys[i]
-                except:
-                    pass
-            if i == (len(chains[0]) - 2):
-                try:
-                    hex.xaxis.axis_label = keys[j]
-                except:
-                    pass
-            try:
-                hex.xaxis.major_label_orientation = np.pi / 4
-            except:
                 pass
 
-            figs_row.append(hex)
-        bokeh_figs.append(figs_row)
-    figure_distributions.subplots_adjust(hspace=0.1, wspace=0.1)
+    else:
 
-    bokeh_grid = gridplot(bokeh_figs)
+        figure_axes.scatter(0, 0, s=10, c='r')
 
-    return figure_distributions, bokeh_grid
+        einstein_ring = plt.Circle((0, 0), 1, fill=False, color='k', linestyle='--')
+        figure_axes.add_artist(einstein_ring)
 
+        if bokeh_geometry is not None:
+            bokeh_geometry.scatter(0, 0, color='red')
+            bokeh_geometry.circle(0, 0, radius=1, line_dash='dashed',
+                                  line_color='black', fill_color=None)
 
-def parameters_result(fit, parameters=None):
-    """ Produce a namedtuple object containing the fitted parameters in the fit.fit_results.
+    for telescope_index, telescope in enumerate(microlensing_model.event.telescopes):
 
-    :param fit: a fit object. See the microlfits for more details.
-    :param fit_parameters: a namedtuple object containing the fitted parameters.
-    :rtype: object
-    """
+        if telescope.lightcurve_flux is not None:
 
-    fit_parameters = collections.namedtuple('Parameters', fit.model.model_dictionnary.keys())
+            trajectory_x, trajectory_y, dseparation, dalpha = \
+                microlensing_model.source_trajectory(
+                    telescope,
+                    pyLIMA_parameters,
+                    data_type='photometry')
 
-    if parameters is not None:
+            if 'rho' in microlensing_model.pyLIMA_standards_dictionnary.keys():
 
-        pass
+                rho = pyLIMA_parameters.rho
 
-    else:
+            else:
 
-        parameters = fit.fit_results
+                rho = 10 ** -5
 
-    for parameter in fit.model.model_dictionnary.keys():
+            color = plt.rcParams["axes.prop_cycle"].by_key()["color"][telescope_index]
 
-        try:
-            setattr(fit_parameters, parameter, parameters[fit.model.model_dictionnary[parameter]])
-        except:
-            pass
+            patches = [plt.Circle((x, y), rho, color=color,
+                                  alpha=0.2) for x, y in
+                       zip(trajectory_x, trajectory_y)]
+            coll = matplotlib.collections.PatchCollection(patches, match_original=True)
 
-    setattr(fit_parameters, 'chichi', parameters[-1])
-    return fit_parameters
+            figure_axes.scatter(trajectory_x, trajectory_y,
+                                c=color,
+                                alpha=0.5, label=telescope.name, s=0.1)
 
+            figure_axes.add_collection(coll)
 
-def MCMC_covariance(mcmc_chains):
-    """ Estimate the covariance matrix from the mcmc_chains
+            if bokeh_geometry is not None:
+                bokeh_geometry.circle(trajectory_x, trajectory_y, radius=rho,
+                                      color=color,
+                                      radius_dimension='max', fill_alpha=0.5)
 
-    :param mcmc_chains: a numpy array representing the mcmc chains.
-    :return : a numpy array representing the covariance matrix of your MCMC sampling.
-    :rtype: array_like
-    """
-    esperances = []
-    for i in range(mcmc_chains.shape[1] - 1):
-        esperances.append(mcmc_chains[:, i] - np.median(mcmc_chains[:, i]))
+    if microlensing_model.parallax_model[0] != 'None':
 
-    covariance_matrix = np.zeros((mcmc_chains.shape[1] - 1, mcmc_chains.shape[1] - 1))
+        origin_t0par_index = np.argmin(
+            np.abs(telescope.lightcurve_magnitude['time'].value -
+                   microlensing_model.parallax_model[1]))
 
-    for i in range(mcmc_chains.shape[1] - 1):
-        for j in np.arange(i, mcmc_chains.shape[1] - 1):
-            covariance_matrix[i, j] = 1 / (len(mcmc_chains) - 1) * np.sum(
-                esperances[i] * esperances[j])
-            covariance_matrix[j, i] = 1 / (len(mcmc_chains) - 1) * np.sum(
-                esperances[i] * esperances[j])
+        origin_t0par = np.array(
+            (trajectory_x[origin_t0par_index], trajectory_y[origin_t0par_index]))
+        # origin_t0par += 0.1
 
-    return covariance_matrix
+        piEN = pyLIMA_parameters.piEN
+        piEE = pyLIMA_parameters.piEE
 
+        EN_trajectory_angle = parallax.EN_trajectory_angle(piEN, piEE)
 
-def fit_errors(fit, covariance_matrix=None):
-    """ Estimate the parameters errors from the covariance matrix.
+        plot_angle = -EN_trajectory_angle
 
-    :param fit: a fit object. See the microlfits for more details.
-    :return: a namedtuple object containing the square roots of parameters variance.
-    :rtype: object
-    """
+        try:
 
-    if covariance_matrix is not None:
+            plot_angle += pyLIMA_parameters.alpha
 
-        pass
+        except AttributeError:
 
-    else:
+            pass
 
-        covariance_matrix = fit.fit_covariance
+        north = [0.1, 0]
+        east = [0, 0.1]
 
-    keys = ['err_' + parameter for parameter in fit.model.model_dictionnary.keys()]
-    parameters_errors = collections.namedtuple('Errors_Parameters', keys)
-    errors = covariance_matrix.diagonal() ** 0.5
+        North = [0.105, 0]
+        East = [0, 0.105]
+
+        rota_mat = np.array([[np.cos(plot_angle), -np.sin(plot_angle)],
+                             [np.sin(plot_angle), np.cos(plot_angle)]])
+
+        east = np.dot(rota_mat, east)
+        north = np.dot(rota_mat, north)
+        East = np.dot(rota_mat, East)
+        North = np.dot(rota_mat, North)
+
+        plt.annotate('',
+                     xy=(origin_t0par[0] + east[0], origin_t0par[1] + east[1]),
+                     xytext=(origin_t0par[0], origin_t0par[1]),
+                     arrowprops=dict(arrowstyle="->", lw=3, alpha=0.5))
+        plt.annotate('E', xy=(origin_t0par[0] + East[0], origin_t0par[1] + East[1]),
+                     xytext=(origin_t0par[0] + East[0], origin_t0par[1] + East[1]),
+                     weight='bold', alpha=0.5, ha='center', va='center',
+                     rotation=np.rad2deg(plot_angle))
+
+        plt.annotate('', xy=(
+            origin_t0par[0] + north[0], origin_t0par[1] + north[1]),
+                     xytext=(origin_t0par[0], origin_t0par[1]),
+                     arrowprops=dict(arrowstyle="->", lw=3, alpha=0.5))
+        plt.annotate('N',
+                     xy=(origin_t0par[0] + North[0], origin_t0par[1] + North[1]),
+                     xytext=(
+                         origin_t0par[0] + North[0], origin_t0par[1] + North[1]),
+                     weight='bold', alpha=0.5, ha='center', va='center',
+                     rotation=np.rad2deg(plot_angle))
+
+        if bokeh_geometry is not None:
+            bokeh_geometry.add_layout(
+                Arrow(end=OpenHead(line_color="grey", line_width=1),
+                      x_start=origin_t0par[0], y_start=origin_t0par[1],
+                      x_end=origin_t0par[0] + North[0],
+                      y_end=origin_t0par[1] + North[1]))
+            bokeh_geometry.add_layout(
+                Arrow(end=OpenHead(line_color="grey", line_width=1),
+                      x_start=origin_t0par[0], y_start=origin_t0par[1],
+                      x_end=origin_t0par[0] + East[0],
+                      y_end=origin_t0par[1] + East[1]))
+    # legend = figure_axes.legend(numpoints=1, loc='best', fancybox=True,
+    # framealpha=0.5)
+    legend = figure_axes.legend(shadow=True, fontsize='large',
+                                bbox_to_anchor=(0, 1.02, 1, 0.2), loc="lower left",
+                                mode="expand", borderaxespad=0, ncol=3, numpoints=1)
+
+    for handle in legend.legendHandles:
 
-    for i in fit.model.model_dictionnary.keys():
         try:
-            setattr(parameters_errors, 'err_' + i, errors[fit.model.model_dictionnary[i]])
-        except:
-            pass
-    return parameters_errors
 
+            handle.set_sizes([100])
 
-def cov2corr(covariance_matrix):
-    """Covariance matrix to correlation matrix.
+        except AttributeError:
 
-    :param array_like covariance_matrix: a (square) numpy array representing the covariance matrix
+            pass
 
-    :return: a (square) numpy array representing the correlation matrix
-    :rtype: array_like
+    figure_axes.xaxis.set_major_locator(MaxNLocator(5))
+    figure_axes.yaxis.set_major_locator(MaxNLocator(5))
+    figure_axes.xaxis.get_major_ticks()[0].draw = lambda *args: None
+    figure_axes.yaxis.get_major_ticks()[0].draw = lambda *args: None
+    figure_axes.xaxis.get_major_ticks()[-1].draw = lambda *args: None
+    figure_axes.yaxis.get_major_ticks()[-1].draw = lambda *args: None
 
-    """
+    figure_axes.set_xlabel(r'$x(\theta_E)$', fontsize=25)
+    figure_axes.set_ylabel(r'$y(\theta_E)$', fontsize=25)
+    figure_axes.tick_params(axis='x', labelsize=15)
+    figure_axes.tick_params(axis='y', labelsize=15)
 
-    covariance_diagonal = np.sqrt(covariance_matrix.diagonal())
-    correlation_matrix = ((covariance_matrix.T / covariance_diagonal).T) / covariance_diagonal
+    figure_axes.axis([-2, 2, -2, 2])
+    # figure_axes.axis('scaled')
+    # title = microlensing_model.event.name + ' : ' + microlensing_model.model_type
+    # figure_trajectory.suptitle(title, fontsize=30 * fig_size[0] / len(title))
 
-    return correlation_matrix
+    return figure_trajectory, bokeh_geometry
 
 
-def MCMC_plot_lightcurves(fit, mcmc_best):
-    """Plot 35 models from the mcmc_best sample. This is made to have  35 models equally spaced
-    in term of objective funtion (~chichi)
+def plot_astrometry(microlensing_model, model_parameters, bokeh_plot=None):
+    # Change matplotlib default colors
+    n_telescopes = len(microlensing_model.event.telescopes)
+    color = plt.cm.jet(
+        np.linspace(0.01, 0.99, n_telescopes))  # This returns RGBA; convert:
+    # hexcolor = map(lambda rgb: '#%02x%02x%02x' % (rgb[0] * 255, rgb[1] * 255,
+    # rgb[2] * 255),
+    #                tuple(color[:, 0:-1]))
+    hexcolor = ['#' + format(int(i[0] * 255), 'x').zfill(2) + format(int(i[1] * 255),
+                                                                     'x').zfill(2) +
+                format(int(i[2] * 255), 'x').zfill(2) for i in color]
 
-    :param fit: a fit object. See the microlfits for more details.
-    :param mcmc_best: a numpy array representing the best (<= 6 sigma) mcmc chains.
-    :return: a two matplotlib subplot showing the data and 35 models and the residuals
-    corresponding to the best model.
-    :rtype: matplotlib_figure
-    """
+    matplotlib.rcParams['axes.prop_cycle'] = cycler.cycler(color=hexcolor)
 
-    figure_lightcurves, figure_axes = initialize_plot_lightcurve(fit)
-    bokeh_lightcurves = figure(width=800, height=600, toolbar_location=None, y_axis_label='m [mag]')
-    bokeh_residuals = figure(width=bokeh_lightcurves.plot_width, plot_height=200, x_range=bokeh_lightcurves.x_range,
-                             y_range=(0.18, -0.18), toolbar_location=None,
-                             x_axis_label='JD', y_axis_label=u'\u0394m [mag]')
+    # Set up the geometry of the three plots
+    main_plot = [0.12, 0.12, 0.48, 0.48]
+    residuals_x = [0.12, 0.83, 0.83, 0.15]
+    residuals_y = [0.12, 0.65, 0.83, 0.15]
+
+    # Set up the size of the figure
+    fig_size = (9.5, 9.5)
+    ast_figure = plt.figure(figsize=fig_size)
+
+    # Make the three plots
+    ax_main = ast_figure.add_axes(main_plot)
+    ax_res_x = ast_figure.add_axes(residuals_x)
+    ax_res_y = ast_figure.add_axes(residuals_y)
+
+    ax_main.xaxis.grid(True)
+    ax_main.yaxis.grid(True)
+    ax_res_x.xaxis.grid(True)
+    ax_res_x.yaxis.grid(True)
+    ax_res_y.xaxis.grid(True)
+    ax_res_y.yaxis.grid(True)
+
+    ax_res_x.get_shared_x_axes().join(ax_res_x, ax_res_y)
+    # ax_main.get_shared_y_axes().join(ax_main, ax_res_y)
+    ax_res_y.xaxis.set_major_locator(MaxNLocator(4))
+    ax_res_x.xaxis.set_major_locator(MaxNLocator(4))
 
-    telescope_index = 0
-    telescope_reference_name = fit.event.telescopes[telescope_index].name
+    ax_res_y.ticklabel_format(useOffset=False, style='plain')
 
-    for telescope_index, telescope in enumerate(fit.event.fake_telescopes):
+    unit = 'deg'
+    for tel in microlensing_model.event.telescopes:
 
-        telescope_index_color = [i for i in range(len(fit.event.telescopes)) if
-                                 fit.event.telescopes[i].name == telescope.name][0]
+        if tel.astrometry is not None:
+            unit = tel.astrometry['ra'].unit
 
-        for idx, parameters in enumerate(mcmc_best):
+    if bokeh_plot is not None:
 
-            if len(parameters[:-1]) < len(fit.model.model_dictionnary):
-                parameters = complete_MCMC_parameters(fit, parameters)
+        bokeh_main = figure(width=800, height=800, toolbar_location=None,
+                            x_axis_label=r'$$E~[' + str(unit) + ']$$',
+                            y_axis_label=r'$$N~[' + str(unit) + ']$$')
+
+        bokeh_res_x = figure(width=bokeh_main.width, height=200,
+                             y_range=(-0.1, 0.1), toolbar_location=None,
+                             y_axis_label=r'$$\Delta_N$$')
+        bokeh_res_y = figure(width=bokeh_main.width, height=200,
+                             y_range=(-0.1, 0.1), toolbar_location=None,
+                             y_axis_label=r'$$\Delta_E$$')
+
+        bokeh_main.x_range.flipped = True
+        bokeh_res_y.xaxis.formatter = BasicTickFormatter(use_scientific=False)
+        bokeh_res_x.xaxis.minor_tick_line_color = None
+        bokeh_res_x.xaxis.major_tick_line_color = None
+        bokeh_res_x.xaxis.major_label_text_font_size = '0pt'
 
-            pyLIMA_parameters = fit.model.compute_pyLIMA_parameters(parameters)
-            parameters_to_plot = copy.copy(parameters)
+    else:
 
-            # put all flux parameters to the telescope 0 scale
+        bokeh_main = None
+        bokeh_res_x = None
+        bokeh_res_y = None
 
-            for index, telescope in enumerate(fit.event.telescopes):
+    if len(model_parameters) != len(microlensing_model.model_dictionnary):
+        telescopes_fluxes = microlensing_model.find_telescopes_fluxes(model_parameters)
 
-                telescope_name = telescope.name
-                parameters_to_change = [(i, name) for i, name in enumerate(pyLIMA_parameters._fields) if
-                                        telescope_name in name]
+        model_parameters = np.r_[model_parameters, telescopes_fluxes]
 
-                for parameter in parameters_to_change:
-                    parameters_to_plot[parameter[0]] = getattr(pyLIMA_parameters, parameter[1].replace(telescope_name,
-                                                                                                       telescope_reference_name))
+    plot_astrometric_data(ax_main, microlensing_model, bokeh_plot=bokeh_main)
 
-            plot_model(figure_axes[0], fit,
-                       parameters=parameters_to_plot, telescope_index=telescope_index, model_color='grey',
-                       model_alpha=0.25, label=False, bokeh_plot=bokeh_lightcurves)
+    plot_astrometric_models([ax_main, ax_res_x, ax_res_y], microlensing_model,
+                            model_parameters,
+                            bokeh_plots=[bokeh_main, bokeh_res_x, bokeh_res_y])
 
-        if telescope_index == 0:
+    ax_main.legend(shadow=True, fontsize='large', bbox_to_anchor=(1.05, 0.25),
+                   loc="center left", borderaxespad=0, ncol=2)
 
-            plot_model(figure_axes[0], fit,
-                       parameters=parameters_to_plot, telescope_index=telescope_index,
-                       model_color=plt.rcParams["axes.prop_cycle"].by_key()["color"][telescope_index_color],
-                       bokeh_plot=bokeh_lightcurves)
-        else:
+    ax_main.invert_xaxis()
+    ax_res_x.set_xticklabels([])
 
-            plot_model(figure_axes[0], fit,
-                       parameters=parameters_to_plot, telescope_index=telescope_index,
-                       model_color=plt.rcParams["axes.prop_cycle"].by_key()["color"][telescope_index_color],
-                       label=False, bokeh_plot=bokeh_lightcurves)
+    ax_main.set_xlabel(r'$E~[' + str(unit) + ']$', fontsize=4 * fig_size[0] * 3 / 4.0)
+    ax_main.set_ylabel(r'$N~[' + str(unit) + ']$', fontsize=4 * fig_size[0] * 3 / 4.0)
 
-    plot_align_data(figure_axes[0], fit, telescope_index=0, parameters=parameters, bokeh_plot=bokeh_lightcurves)
+    ax_res_y.set_ylabel(r'$\Delta E~[' + str(unit) + ']$',
+                        fontsize=4 * fig_size[0] * 3 / 4.0)
+    ax_res_y.set_xlabel('$JD$',  x=0.75,fontsize=4 * fig_size[0] * 3 / 4.0)
 
-    plot_residuals(figure_axes[1], fit, parameters=parameters, bokeh_plot=bokeh_residuals)
+    ax_res_x.set_ylabel(r'$\Delta N~[' + str(unit) + ']$',
+                        fontsize=4 * fig_size[0] * 3 / 4.0)
 
-    figure_axes[0].legend(numpoints=1, loc='best',
-                          fancybox=True, framealpha=0.5)
+    figure_bokeh = gridplot([[bokeh_res_x], [bokeh_res_y], [bokeh_main]],
+                            toolbar_location='above')
 
-    bokeh_lightcurves.xaxis.minor_tick_line_color = None
-    bokeh_lightcurves.xaxis.major_tick_line_color = None
-    bokeh_lightcurves.xaxis.major_label_text_font_size = '0pt'
-    bokeh_lightcurves.y_range.flipped = True
-    bokeh_lightcurves.xaxis.formatter = BasicTickFormatter(use_scientific=False)
-    bokeh_lightcurves.legend.click_policy = "mute"
+    return ast_figure, figure_bokeh
 
-    legend = bokeh_lightcurves.legend[0]
 
-    bokeh_lightcurves.add_layout(legend, 'right')
+def plot_astrometric_models(figure_axes, microlensing_model, model_parameters,
+                            bokeh_plots=None):
+    pyLIMA_parameters = microlensing_model.compute_pyLIMA_parameters(model_parameters)
 
-    bokeh_residuals.xaxis.formatter = BasicTickFormatter(use_scientific=False)
-    bokeh_residuals.xaxis.major_label_orientation = np.pi / 4
-    bokeh_residuals.xaxis.minor_tick_line_color = None
+    list_of_telescopes = create_telescopes_to_plot_model(microlensing_model,
+                                                         pyLIMA_parameters)
+    telescopes_names = np.array([i.name for i in microlensing_model.event.telescopes])
 
-    figure_bokeh = gridplot([[bokeh_lightcurves], [bokeh_residuals]], toolbar_location=None)
+    # plot models
+    Earth = True
 
-    return figure_lightcurves, figure_bokeh
+    for tel in list_of_telescopes:
 
+        if tel.astrometry is not None:
 
-def LM_plot_lightcurves(fit):
-    """Plot the aligned datasets and the best fit on the first subplot figure_axes[0] and residuals
-    on the second subplot figure_axes[1].
+            model = microlensing_model.compute_the_microlensing_model(tel,
+                                                                      pyLIMA_parameters)
 
-    :param object fit: a fit object. See the microlfits for more details.
-    :return: a figure representing data+model and residuals.
-    :rtype: matplotlib_figure
+            astrometric_model = model['astrometry']
+            lens_E, lens_N = astrometric_positions.lens_astrometric_positions(
+                microlensing_model, tel, pyLIMA_parameters)
+            name = tel.name
 
-    """
+            index_color = np.where(name == telescopes_names)[0][0]
+            color = plt.rcParams["axes.prop_cycle"].by_key()["color"][index_color]
 
-    figure_lightcurves, figure_axes = initialize_plot_lightcurve(fit)
-    bokeh_lightcurves = figure(width=800, height=600, toolbar_location=None, y_axis_label='m [mag]')
-    bokeh_residuals = figure(width=bokeh_lightcurves.plot_width, plot_height=200, x_range=bokeh_lightcurves.x_range,
-                             y_range=(0.18, -0.18), toolbar_location=None,
-                             x_axis_label='JD', y_axis_label=u'\u0394m [mag]')
+            figure_axes[0].plot(astrometric_model[0], astrometric_model[1], c=color)
 
-    try:
-        best_parameters = fit.fit_results
-    except:
-        best_parameters = fit.MCMC_chains[np.argmax(fit.MCMC_chains[:, -1])]
+            if bokeh_plots[0] is not None:
+                bokeh_plots[0].line(astrometric_model[0], astrometric_model[1],
+                                    color=color)
 
-    pyLIMA_parameters = fit.model.compute_pyLIMA_parameters(best_parameters)
+            if Earth is True:
 
-    telescope_index = 0
-    telescope_reference_name = fit.event.telescopes[telescope_index].name
+                source_E, source_N = \
+                    astrometric_positions.astrometric_positions_of_the_source(
+                        tel, pyLIMA_parameters)
+                figure_axes[0].plot(source_E, source_N, c='k', label='Source')
+                figure_axes[0].plot(lens_E, lens_N, c='k', linestyle='--', label='Lens')
 
-    parameters_to_plot = copy.copy(best_parameters)
+                if bokeh_plots[0] is not None:
+                    bokeh_plots[0].line(source_E, source_N, color='black',
+                                        legend_label='Source')
+                    bokeh_plots[0].line(lens_E, lens_N, color='black',
+                                        line_dash='dotted', legend_label='Lens')
 
-    # put all flux parameters to the telescope 0 scale
+                for index in [-2, -1, 0, 1, 2]:
 
-    for index, telescope in enumerate(fit.event.telescopes):
+                    try:
 
-        telescope_name = telescope.name
-        parameters_to_change = [(i, name) for i, name in enumerate(pyLIMA_parameters._fields) if telescope_name in name]
+                        index_time = np.argmin(np.abs(tel.astrometry['time'].value -
+                                                      (
+                                                              pyLIMA_parameters.t0 +
+                                                              index *
+                                                              pyLIMA_parameters.tE)))
+                        derivative = (source_N[index_time - 1] - source_N[
+                            index_time + 1]) / (
+                                             source_E[index_time - 1] - source_E[
+                                         index_time + 1])
 
-        for parameter in parameters_to_change:
-            parameters_to_plot[parameter[0]] = getattr(pyLIMA_parameters, parameter[1].replace(telescope_name,
-                                                                                               telescope_reference_name))
- 
-    for telescope_index, telescope in enumerate(fit.event.fake_telescopes):
+                        figure_axes[0].annotate('', xy=(
+                            source_E[index_time], source_N[index_time]),
+                                                xytext=(source_E[index_time] - 0.001 * (
+                                                        source_E[index_time + 1] -
+                                                        source_E[index_time]),
+                                                        source_N[index_time] - 0.001 * (
+                                                                source_E[
+                                                                    index_time +
+                                                                    1] -
+                                                                source_E[
+                                                                    index_time])
+                                                        * derivative),
+                                                arrowprops=dict(arrowstyle="->",
+                                                                mutation_scale=35,
+                                                                color='k'))
 
-        telescope_index_color = [i for i in range(len(fit.event.telescopes)) if
-                                 fit.event.telescopes[i].name == telescope.name][0]
+                        index_time = np.argmin(np.abs(tel.astrometry['time'].value -
+                                                      (
+                                                              pyLIMA_parameters.t0 +
+                                                              index *
+                                                              pyLIMA_parameters.tE)))
+                        derivative = (lens_N[index_time - 1] - lens_N[
+                            index_time + 1]) / (
+                                             lens_E[index_time - 1] - lens_E[
+                                         index_time + 1])
 
-        if telescope_index == 0:
+                        figure_axes[0].annotate('', xy=(
+                            lens_E[index_time], lens_N[index_time]),
+                                                xytext=(lens_E[index_time] - 0.001 * (
+                                                        lens_E[index_time + 1] -
+                                                        lens_E[index_time]),
+                                                        lens_N[index_time] - 0.001 * (
+                                                                lens_E[
+                                                                    index_time +
+                                                                    1] -
+                                                                lens_E[
+                                                                    index_time])
+                                                        * derivative),
+                                                arrowprops=dict(arrowstyle="->",
+                                                                mutation_scale=35,
+                                                                color='k'))
 
-            plot_model(figure_axes[0], fit, parameters=parameters_to_plot, telescope_index=telescope_index,
-                       model_color=plt.rcParams["axes.prop_cycle"].by_key()["color"][telescope_index_color],
-                       bokeh_plot=bokeh_lightcurves)
+                        if bokeh_plots[0] is not None:
+                            oh = OpenHead(line_color='black', line_width=1)
 
-        else:
-            plot_model(figure_axes[0], fit, parameters=parameters_to_plot, telescope_index=telescope_index,
-                       model_color=plt.rcParams["axes.prop_cycle"].by_key()["color"][telescope_index_color],
-                       label=False, bokeh_plot=bokeh_lightcurves)
+                            bokeh_plots[0].add_layout(Arrow(end=oh,
+                                                            x_start=source_E[
+                                                                index_time],
+                                                            y_start=source_N[
+                                                                index_time],
+                                                            x_end=source_E[
+                                                                index_time + 1],
+                                                            y_end=source_N[
+                                                                index_time + 1]))
 
-    plot_align_data(figure_axes[0], fit, telescope_index=0, parameters=best_parameters, bokeh_plot=bokeh_lightcurves)
+                            bokeh_plots[0].add_layout(Arrow(end=oh,
+                                                            x_start=lens_E[index_time],
+                                                            y_start=lens_N[index_time],
+                                                            x_end=lens_E[
+                                                                index_time + 1],
+                                                            y_end=lens_N[
+                                                                index_time + 1]))
 
-    plot_residuals(figure_axes[1], fit, parameters=best_parameters, bokeh_plot=bokeh_residuals)
-    figure_axes[0].legend(numpoints=1, loc='best',
-                          fancybox=True, framealpha=0.5)
+                    except ValueError:
 
-    bokeh_lightcurves.xaxis.minor_tick_line_color = None
-    bokeh_lightcurves.xaxis.major_tick_line_color = None
-    bokeh_lightcurves.xaxis.major_label_text_font_size = '0pt'
-    bokeh_lightcurves.y_range.flipped = True
-    bokeh_lightcurves.xaxis.formatter = BasicTickFormatter(use_scientific=False)
-    bokeh_lightcurves.legend.click_policy = "mute"
+                        pass
 
-    legend = bokeh_lightcurves.legend[0]
-    # legend.visible = None
+                Earth = False
 
-    # bokeh_lightcurves.legend.visible = False
-    # legend.orientation = 'horizontal'
-    bokeh_lightcurves.add_layout(legend, 'right')
-    # bokeh_legend = figure()
-    # bokeh_lightcurves.add_layout(legend,'above')
+    # plot residuals
 
-    bokeh_residuals.xaxis.formatter = BasicTickFormatter(use_scientific=False)
-    bokeh_residuals.xaxis.major_label_orientation = np.pi / 4
-    bokeh_residuals.xaxis.minor_tick_line_color = None
+    for ind, tel in enumerate(microlensing_model.event.telescopes):
 
-    figure_bokeh = gridplot([[bokeh_lightcurves], [bokeh_residuals]], toolbar_location=None)
+        if tel.astrometry is not None:
 
-    return figure_lightcurves, figure_bokeh
+            delta_ra = tel.astrometry['ra'].value
+            err_ra = tel.astrometry['err_ra'].value
 
+            delta_dec = tel.astrometry['dec'].value
+            err_dec = tel.astrometry['err_dec'].value
 
-def initialize_plot_lightcurve(fit):
-    """Initialize the lightcurve plot.
+            color = plt.rcParams["axes.prop_cycle"].by_key()["color"][ind]
 
-    :param object fit: a fit object. See the microlfits for more details.
+            model = microlensing_model.compute_the_microlensing_model(tel,
+                                                                      pyLIMA_parameters)
 
-    :return: a matplotlib figure  and the corresponding matplotlib axes
-    :rtype: matplotlib_figure,matplotlib_axes
+            astrometric_model = model['astrometry']
 
-    """
-    fig_size = [10, 10]
-    figure, figure_axes = plt.subplots(2, 1, sharex=True, gridspec_kw={'height_ratios': [3, 1]},
-                                       figsize=(fig_size[0], fig_size[1]), dpi=75)
-    plt.subplots_adjust(top=0.9, bottom=0.15, left=0.15, right=0.99, wspace=0.2, hspace=0.1)
-    figure_axes[0].grid()
-    figure_axes[1].grid()
-    # fig_size = plt.rcParams["figure.figsize"]
-    figure.suptitle(fit.event.name, fontsize=30 * fig_size[0] / len(fit.event.name))
-
-    figure_axes[0].set_ylabel('Mag', fontsize=5 * fig_size[1] * 3 / 4.0)
-    figure_axes[0].yaxis.set_major_locator(MaxNLocator(4))
-    figure_axes[0].tick_params(axis='y', labelsize=3.5 * fig_size[1] * 3 / 4.0)
-
-    figure_axes[0].text(0.01, 0.96, 'provided by pyLIMA', style='italic', fontsize=10,
-                        transform=figure_axes[0].transAxes)
-
-    figure_axes[1].set_xlabel('HJD', fontsize=5 * fig_size[0] * 3 / 4.0)
-    figure_axes[1].xaxis.set_major_locator(MaxNLocator(3))
-    figure_axes[1].yaxis.set_major_locator(MaxNLocator(4, min_n_ticks=3))
-
-    figure_axes[1].ticklabel_format(useOffset=False, style='plain')
-    figure_axes[1].set_ylabel('Residuals', fontsize=5 * fig_size[1] * 2 / 4.0)
-    figure_axes[1].tick_params(axis='x', labelsize=3.5 * fig_size[0] * 3 / 4.0)
-    figure_axes[1].tick_params(axis='y', labelsize=3.5 * fig_size[1] * 3 / 4.0)
-
-    return figure, figure_axes
-
-
-def plot_model(figure_axe, fit, parameters=None, telescope_index=0, model_color='b', model_alpha=1.0, label=True,
-               bokeh_plot=None):
-    """Plot the microlensing model corresponding to parameters, time and with the same properties as  telescope,  the best fit and first telescope.
+            figure_axes[1].errorbar(tel.astrometry['time'].value,
+                                    delta_ra - astrometric_model[0], yerr=err_ra,
+                                    fmt='.', ecolor=color, color=color,
+                                    label=tel.name, alpha=0.5)
 
-    :param object fit: a fit object. See the microlfits for more details.
-    :param matplotlib_axes figure_axe: a matplotlib axes correpsonding to the figure.
-    :param list parameters : a list of model parameters.
-    :param np.array time : the time stamps for the model.
-    :param int telescope_index : which telescope you want a model (depends on filter, location etc...)
-    :param str model_color : the model color
-    :param float model_alpha : the intensity of the model line
+            figure_axes[2].errorbar(tel.astrometry['time'].value,
+                                    delta_dec - astrometric_model[1], yerr=err_dec,
+                                    fmt='.', ecolor=color,
+                                    color=color,
+                                    label=tel.name, alpha=0.5)
 
-    """
+            if bokeh_plots[1] is not None:
 
-    if parameters is not None:
+                res_ra = delta_ra - astrometric_model[0]
+                res_dec = delta_dec - astrometric_model[1]
 
-        pyLIMA_parameters = fit.model.compute_pyLIMA_parameters(parameters)
+                time = []
 
-    else:
+                err_xs = []
+                err_ys = []
 
-        pyLIMA_parameters = fit.model.compute_pyLIMA_parameters(fit.fit_results)
+                for t, rex, rey, xerr, yerr in zip(tel.astrometry['time'].value, res_ra,
+                                                   res_dec, err_ra, err_dec):
+                    time.append((t, t))
 
-    telescope = fit.event.fake_telescopes[telescope_index]
+                    err_xs.append((rex - xerr, rex + xerr))
+                    err_ys.append((rey - yerr, rey + yerr))
 
-    time = telescope.lightcurve_flux[:, 0]
-    flux_model = fit.model.compute_the_microlensing_model(telescope, pyLIMA_parameters)[0]
-    magnitude = microltoolbox.flux_to_magnitude(flux_model)
+                bokeh_plots[1].scatter(tel.astrometry['time'].value,
+                                       delta_ra - astrometric_model[0],
+                                       color=color,
+                                       size=5,
+                                       muted_color=color,
+                                       muted_alpha=0.2)
 
-    if label == True:
+                bokeh_plots[1].multi_line(time, err_xs, color=color,
+                                          muted_color=color,
+                                          muted_alpha=0.2)
 
-        figure_axe.plot(time, magnitude, c=model_color, label=fit.model.model_type, lw=3, alpha=model_alpha)
+                bokeh_plots[2].scatter(tel.astrometry['time'].value,
+                                       delta_dec - astrometric_model[1],
+                                       color=color,
+                                       size=5,
+                                       muted_color=color,
+                                       muted_alpha=0.2)
 
-    else:
+                bokeh_plots[2].multi_line(time, err_ys, color=color,
+                                          muted_color=color,
+                                          muted_alpha=0.2)
 
-        figure_axe.plot(time, magnitude, c=model_color, lw=3, alpha=model_alpha)
 
-    if telescope_index == 0:
-        figure_axe.set_ylim(
-            [min(magnitude) - plot_lightcurve_windows, max(magnitude) + plot_lightcurve_windows])
-        figure_axe.set_xlim(
-            [pyLIMA_parameters.to - 2 * np.abs(pyLIMA_parameters.tE),
-             pyLIMA_parameters.to + 2 * np.abs(pyLIMA_parameters.tE)])
+def plot_astrometric_data(figure_ax, microlensing_model, bokeh_plot=None):
+    # plot data
+    for ind, tel in enumerate(microlensing_model.event.telescopes):
 
-        figure_axe.invert_yaxis()
+        if tel.astrometry is not None:
 
-    if bokeh_plot is not None:
+            delta_ra = tel.astrometry['ra'].value
+            err_ra = tel.astrometry['err_ra'].value
 
-        if label == True:
-            bokeh_plot.line(time, magnitude, color=model_color, alpha=model_alpha, legend=fit.model.model_type)
-        else:
-            bokeh_plot.line(time, magnitude, color=model_color, alpha=model_alpha)
+            delta_dec = tel.astrometry['dec'].value
+            err_dec = tel.astrometry['err_dec'].value
 
+            color = plt.rcParams["axes.prop_cycle"].by_key()["color"][ind]
+            # marker = str(MARKER_SYMBOLS[0][ind])
 
-def plot_residuals(figure_axe, fit, parameters=None, bokeh_plot=None):
-    """Plot the residuals from the fit.
+            figure_ax.errorbar(delta_ra, delta_dec, xerr=err_ra, yerr=err_dec, fmt='.',
+                               ecolor=color, color=color,
+                               label=tel.name, alpha=0.5)
 
-    :param object fit: a fit object. See the microlfits for more details.
-    :param matplotlib_axes figure_axe: a matplotlib axes correpsonding to the figure.
-    """
+            if bokeh_plot is not None:
 
-    if parameters is not None:
+                bokeh_plot.scatter(delta_ra, delta_dec,
+                                   color=color,
+                                   size=5, legend_label=tel.name,
+                                   muted_color=color,
+                                   muted_alpha=0.2)
 
-        pyLIMA_parameters = fit.model.compute_pyLIMA_parameters(parameters)
+                X = []
+                Y = []
 
-    else:
-        pyLIMA_parameters = fit.model.compute_pyLIMA_parameters(fit.fit_results)
+                err_xs = []
+                err_ys = []
 
-    for index, telescope in enumerate(fit.event.telescopes):
-        time = telescope.lightcurve_flux[:, 0]
-        flux = telescope.lightcurve_flux[:, 1]
-        err_mag = telescope.lightcurve_magnitude[:, 2]
+                for x, y, xerr, yerr in zip(delta_ra, delta_dec, err_ra, err_dec):
+                    X.append((x, x))
+                    Y.append((y, y))
 
-        flux_model = fit.model.compute_the_microlensing_model(telescope, pyLIMA_parameters)[0]
+                    err_xs.append((x - xerr, x + xerr))
+                    err_ys.append((y - yerr, y + yerr))
 
-        residuals = 2.5 * np.log10(flux_model / flux)
+                bokeh_plot.multi_line(err_xs, Y, color=color,
+                                      muted_color=color,
+                                      muted_alpha=0.2)
 
-        figure_axe.errorbar(time, residuals, yerr=err_mag, ls='None', markersize=7.5,
-                            marker=str(MARKER_SYMBOLS[0][index]), capsize=0.0)
+                bokeh_plot.multi_line(X, err_ys, color=color,
+                                      muted_color=color,
+                                      muted_alpha=0.2)
 
-        if bokeh_plot is not None:
 
-            bokeh_plot.scatter(time, residuals,
-                               color=plt.rcParams["axes.prop_cycle"].by_key()["color"][index]
-                               , size=5)
+def plot_lightcurves(microlensing_model, model_parameters, bokeh_plot=None):
+    # Change matplotlib default colors
+    n_telescopes = len(microlensing_model.event.telescopes)
+    color = plt.cm.jet(
+        np.linspace(0.01, 0.99, n_telescopes))  # This returns RGBA; convert:
+    # hexcolor = map(lambda rgb: '#%02x%02x%02x' % (rgb[0] * 255, rgb[1] * 255,
+    # rgb[2] * 255),
+    #                tuple(color[:, 0:-1]))
+    hexcolor = ['#' + format(int(i[0] * 255), 'x').zfill(2) + format(int(i[1] * 255),
+                                                                     'x').zfill(2) +
+                format(int(i[2] * 255), 'x').zfill(2) for i in color]
 
-            err_xs = []
-            err_ys = []
+    matplotlib.rcParams['axes.prop_cycle'] = cycler.cycler(color=hexcolor)
 
-            for x, y, yerr in zip(time, residuals, err_mag):
-                err_xs.append((x, x))
-                err_ys.append((y - yerr, y + yerr))
+    mat_figure, mat_figure_axes = initialize_light_curves_plot(
+        event_name=microlensing_model.event.name)
 
-            bokeh_plot.multi_line(err_xs, err_ys, color=plt.rcParams["axes.prop_cycle"].by_key()["color"][index])
+    if bokeh_plot is not None:
 
-    figure_axe.set_ylim([-plot_residuals_windows, plot_residuals_windows])
-    figure_axe.invert_yaxis()
-    figure_axe.yaxis.get_major_ticks()[-1].draw = lambda *args: None
+        bokeh_lightcurves = figure(width=800, height=600, toolbar_location=None,
+                                   y_axis_label=r'$$m [mag]$$')
+        bokeh_residuals = figure(width=bokeh_lightcurves.width, height=200,
+                                 x_range=bokeh_lightcurves.x_range,
+                                 y_range=(0.18, -0.18), toolbar_location=None,
+                                 x_axis_label='JD', y_axis_label=r'$$\Delta m [mag]$$')
+
+        bokeh_lightcurves.xaxis.minor_tick_line_color = None
+        bokeh_lightcurves.xaxis.major_tick_line_color = None
+        bokeh_lightcurves.xaxis.major_label_text_font_size = '0pt'
+        bokeh_lightcurves.y_range.flipped = True
+        bokeh_lightcurves.xaxis.formatter = BasicTickFormatter(use_scientific=False)
+
+        bokeh_residuals.xaxis.formatter = BasicTickFormatter(use_scientific=False)
+        bokeh_residuals.xaxis.major_label_orientation = np.pi / 4
+        bokeh_residuals.xaxis.minor_tick_line_color = None
 
+    else:
 
-def plot_align_data(figure_axe, fit, telescope_index=0, parameters=None, bokeh_plot=None):
-    """Plot the aligned data.
+        bokeh_lightcurves = None
+        bokeh_residuals = None
 
-    :param matplotlib_axes figure_axe: a matplotlib axes correpsonding to the figure.
-    :param object fit: a fit object. See the microlfits for more details.
-    :param int telescope_index : the telescope to align data to.
+    if len(model_parameters) != len(microlensing_model.model_dictionnary):
+        telescopes_fluxes = microlensing_model.find_telescopes_fluxes(model_parameters)
+        telescopes_fluxes = [getattr(telescopes_fluxes, key) for key in
+                             telescopes_fluxes._fields]
+
+        model_parameters = np.r_[model_parameters, telescopes_fluxes]
+
+    plot_photometric_models(mat_figure_axes[0], microlensing_model, model_parameters,
+                            plot_unit='Mag',
+                            bokeh_plot=bokeh_lightcurves)
+
+    plot_aligned_data(mat_figure_axes[0], microlensing_model, model_parameters,
+                      plot_unit='Mag',
+                      bokeh_plot=bokeh_lightcurves)
+
+    plot_residuals(mat_figure_axes[1], microlensing_model, model_parameters,
+                   plot_unit='Mag',
+                   bokeh_plot=bokeh_residuals)
+
+    mat_figure_axes[0].invert_yaxis()
+    mat_figure_axes[1].invert_yaxis()
+    mat_figure_axes[0].legend(shadow=True, fontsize='large',
+                              bbox_to_anchor=(0, 1.02, 1, 0.2),
+                              loc="lower left",
+                              mode="expand", borderaxespad=0, ncol=3)
 
-    """
+    try:
+        bokeh_lightcurves.legend.click_policy = "mute"
+        # legend = bokeh_lightcurves.legend[0]
 
-    normalised_lightcurves = microltoolbox.align_the_data_to_the_reference_telescope(fit, telescope_index, parameters)
+    except AttributeError:
 
-    for index, telescope in enumerate(fit.event.telescopes):
-        lightcurve = normalised_lightcurves[index]
+        pass
 
-        figure_axe.errorbar(lightcurve[:, 0], lightcurve[:, 1], yerr=lightcurve[:, 2], ls='None',
-                            marker=str(MARKER_SYMBOLS[0][index]), markersize=7.5, capsize=0.0,
-                            label=telescope.name)
+    figure_bokeh = gridplot([[bokeh_lightcurves], [bokeh_residuals]],
+                            toolbar_location=None)
 
-        if bokeh_plot is not None:
+    return mat_figure, figure_bokeh
 
-            bokeh_plot.scatter(lightcurve[:, 0], lightcurve[:, 1],
-                               color=plt.rcParams["axes.prop_cycle"].by_key()["color"][index]
-                               , size=5, legend=telescope.name,
-                               muted_color=plt.rcParams["axes.prop_cycle"].by_key()["color"][index],
-                               muted_alpha=0.2)
 
-            err_xs = []
-            err_ys = []
+def initialize_light_curves_plot(plot_unit='Mag', event_name='A microlensing event'):
+    fig_size = [10, 10]
+    mat_figure, mat_figure_axes = plt.subplots(2, 1, sharex=True,
+                                               gridspec_kw={'height_ratios': [3, 1]},
+                                               figsize=(fig_size[0], fig_size[1]),
+                                               dpi=75)
+    plt.subplots_adjust(top=0.8, bottom=0.15, left=0.2, right=0.9, wspace=0.1,
+                        hspace=0.1)
+    mat_figure_axes[0].grid()
+    mat_figure_axes[1].grid()
+    # mat_figure.suptitle(event_name, fontsize=30 * fig_size[0] / len(event_name))
 
-            for x, y, yerr in zip(lightcurve[:, 0], lightcurve[:, 1], lightcurve[:, 2]):
-                err_xs.append((x, x))
-                err_ys.append((y - yerr, y + yerr))
+    mat_figure_axes[0].set_ylabel(r'$' + plot_unit + '$',
+                                  fontsize=5 * fig_size[1] * 3 / 4.0)
+    mat_figure_axes[0].yaxis.set_major_locator(MaxNLocator(4))
+    mat_figure_axes[0].tick_params(axis='y', labelsize=3.5 * fig_size[1] * 3 / 4.0)
 
-            bokeh_plot.multi_line(err_xs, err_ys, color=plt.rcParams["axes.prop_cycle"].by_key()["color"][index],
-                                  legend=telescope.name,
-                                  muted_color=plt.rcParams["axes.prop_cycle"].by_key()["color"][index],
-                                  muted_alpha=0.2)
+    mat_figure_axes[0].text(0.01, 0.96, 'provided by pyLIMA', style='italic',
+                            fontsize=10,
+                            transform=mat_figure_axes[0].transAxes)
 
+    mat_figure_axes[1].set_xlabel(r'$JD$', fontsize=5 * fig_size[0] * 3 / 4.0)
+    mat_figure_axes[1].xaxis.set_major_locator(MaxNLocator(3))
+    mat_figure_axes[1].yaxis.set_major_locator(MaxNLocator(4, min_n_ticks=3))
 
-def align_telescope_lightcurve(lightcurve_telescope_flux, model_ghost, model_telescope):
-    """Align data to the survey telescope (i.e telescope 0).
+    mat_figure_axes[1].ticklabel_format(useOffset=False, style='plain')
+    mat_figure_axes[1].set_ylabel(r'$\Delta M$', fontsize=5 * fig_size[1] * 2 / 4.0)
+    mat_figure_axes[1].tick_params(axis='x', labelsize=3.5 * fig_size[0] * 3 / 4.0)
+    mat_figure_axes[1].tick_params(axis='y', labelsize=3.5 * fig_size[1] * 3 / 4.0)
 
-    :param array_like lightcurve_telescope_mag: the survey telescope in magnitude
-    :param float fs_reference: thce survey telescope reference source flux (i.e the fitted value)
-    :param float g_reference: the survey telescope reference blending parameter (i.e the fitted
-    value)
-    :param float fs_telescope: the telescope source flux (i.e the fitted value)
-    :param float g_reference: the telescope blending parameter (i.e the fitted value)
+    return mat_figure, mat_figure_axes
 
-    :return: the aligned to survey lightcurve in magnitude
-    :rtype: array_like
-    """
-    time = lightcurve_telescope_flux[:, 0]
-    flux = lightcurve_telescope_flux[:, 1]
-    error_flux = lightcurve_telescope_flux[:, 2]
-    err_mag = microltoolbox.error_flux_to_error_magnitude(error_flux, flux)
 
-    residuals = 2.5 * np.log10(model_telescope / flux)
+def plot_photometric_models(figure_axe, microlensing_model, model_parameters,
+                            bokeh_plot=None, plot_unit='Mag'):
+    pyLIMA_parameters = microlensing_model.compute_pyLIMA_parameters(model_parameters)
 
-    magnitude_normalised = microltoolbox.flux_to_magnitude(model_ghost) + residuals
+    list_of_telescopes = create_telescopes_to_plot_model(microlensing_model,
+                                                         pyLIMA_parameters)
+    telescopes_names = np.array([i.name for i in microlensing_model.event.telescopes])
 
-    lightcurve_normalised = [time, magnitude_normalised, err_mag]
+    # plot models
+    index = 0
 
-    lightcurve_mag_normalised = np.array(lightcurve_normalised).T
+    for tel in list_of_telescopes:
 
-    return lightcurve_mag_normalised
+        if tel.lightcurve_flux is not None:
 
+            magni = microlensing_model.model_magnification(tel, pyLIMA_parameters)
+            microlensing_model.derive_telescope_flux(tel, pyLIMA_parameters, magni)
 
-def parameters_table(fit):
-    """Plot the fit parameters and errors.
-        :param object fit: a fit object. See the microlfits for more details.
-        :param list best_parameters: a list containing the model you want to plot the trajectory
-    """
+            f_source = getattr(pyLIMA_parameters, 'fsource_' + tel.name)
+            f_blend = getattr(pyLIMA_parameters, 'fblend_' + tel.name)
 
-    column_labels = ['Parameters', 'Errors']
+            if index == 0:
+                ref_source = f_source
+                ref_blend = f_blend
+                index += 1
 
-    try:
-        # DE or LM
-        table_val = [fit.fit_results, (fit.fit_covariance.diagonal() ** 0.5).tolist() + [0.0]]
-        raw_labels = list(fit.model.model_dictionnary.keys()) + ['Chi^2']
+            magnitude = pyLIMA.toolbox.brightness_transformation.ZERO_POINT - 2.5 * \
+                        np.log10(ref_source * magni + ref_blend)
 
+            # delta_mag = -2.5 * np.log10(f_source + f_blend) + 2.5 * np.log10(
+            ##     ref_source + ref_blend)
+            # magnitude -= delta_mag
 
-    except:
-        # MCMC
-        best_chain = np.argmax(fit.MCMC_chains[:, -1])
+            name = tel.name
 
-        table_val = [(fit.MCMC_chains[best_chain, :-1]).tolist() + [fit.MCMC_chains[best_chain, -1] * -2],
-                     ((np.percentile(fit.MCMC_chains[:, :-1], 84, axis=0) - np.percentile(fit.MCMC_chains[:, :-1],
-                                                                                          16,
-                                                                                          axis=0)) / 2).tolist()
-                     + [0.0]]
+            index_color = np.where(name == telescopes_names)[0][0]
+            color = plt.rcParams["axes.prop_cycle"].by_key()["color"][index_color]
 
-        raw_labels = list(fit.model.model_dictionnary.keys())[:len(table_val[0]) - 1] + ['Chi^2']
+            if tel.location == 'Earth':
 
-    table_val = np.round(table_val, 5).tolist()
-    table_val = np.array(table_val).T.tolist()
+                name = tel.location
+                linestyle = '-'
 
-    table_colors = []
-    raw_colors = []
-    last_color = 'dodgerblue'
-    for i in range(len(table_val)):
-        table_colors.append([last_color, last_color])
-        raw_colors.append(last_color)
+            else:
 
-        if last_color == 'dodgerblue':
+                linestyle = '--'
 
-            last_color = 'white'
+            plots.plot_light_curve_magnitude(tel.lightcurve_magnitude['time'].value,
+                                             magnitude, figure_axe=figure_axe,
+                                             name=name, color=color,
+                                             linestyle=linestyle)
 
-        else:
+            if bokeh_plot is not None:
+                bokeh_plot.line(tel.lightcurve_magnitude['time'].value, magnitude,
+                                legend_label=name, color=color)
 
-            last_color = 'dodgerblue'
 
-    fig_size = [10, 7.5]
-    figure_table = plt.figure(figsize=(fig_size[0], fig_size[1]), dpi=75)
-    table_axes = figure_table.add_subplot(111, aspect=1)
+def plot_aligned_data(figure_axe, microlensing_model, model_parameters, bokeh_plot=None,
+                      plot_unit='Mag'):
+    pyLIMA_parameters = microlensing_model.compute_pyLIMA_parameters(model_parameters)
 
-    the_table = table_axes.table(cellText=table_val, cellColours=table_colors, rowColours=raw_colors,
-                                 rowLabels=raw_labels,
-                                 colLabels=column_labels, loc='center left',
-                                 rowLoc='left', colLoc='center',
-                                 bbox=[0.0, -0.0, 1.0, 1.0]
-                                 )
-    table_axes.get_yaxis().set_visible(False)
-    table_axes.get_xaxis().set_visible(False)
-
-    for (row, col), cell in the_table.get_celld().items():
-
-        if (row == 0) or (col == -1):
-            cell.set_text_props(fontproperties=FontProperties(weight='bold'))
-
-    for cell in the_table._cells:
-        the_table._cells[cell].set_alpha(.5)
-
-    title = fit.model.event.name + ' : ' + fit.model.model_type
-    figure_table.suptitle(title, fontsize=30 * fig_size[0] / len(title))
-
-    bokeh_data = dict(names=raw_labels,
-                      values=np.array(table_val)[:, 0],
-                      errors=np.array(table_val)[:, 1]
-                      )
-    source = ColumnDataSource(bokeh_data)
-    columns = [TableColumn(field="names", title="Parameters"),
-               TableColumn(field="values", title="Values"),
-               TableColumn(field="errors", title="Errors")]
-
-    bokeh_table = DataTable(source=source, columns=columns,
-                            reorderable=True, scroll_to_selection=True,
-                            width=350, height=350,
-                            )
+    # plot aligned data
+    index = 0
 
-    return figure_table, bokeh_table
+    list_of_telescopes = create_telescopes_to_plot_model(microlensing_model,
+                                                         pyLIMA_parameters)
 
+    ref_names = []
+    ref_locations = []
+    ref_magnification = []
+    ref_fluxes = []
 
-def plot_geometry(fit):
-    """Plot the lensing geometry (i.e source trajectory) and the table of best parameters.
-    :param object fit: a fit object. See the microlfits for more details.
-    :param list best_parameters: a list containing the model you want to plot the trajectory
-    """
+    for ref_tel in list_of_telescopes:
+        model_magnification = microlensing_model.model_magnification(ref_tel,
+                                                                     pyLIMA_parameters)
 
-    bokeh_geometry = figure(width=350, height=350, x_range=(-3, 3), y_range=(-3, 3), toolbar_location=None,
-                            x_axis_label='x [' + u'\u03B8\u2091'']', y_axis_label='y [' + u'\u03B8\u2091'']'
-                            )
+        microlensing_model.derive_telescope_flux(ref_tel, pyLIMA_parameters,
+                                                 model_magnification)
 
-    if len(fit.fit_results) != 0:
-        best_parameters = fit.fit_results
-    else:
-        best_parameters = fit.MCMC_chains[np.argmax(fit.MCMC_chains[:, -1])]
+        f_source = getattr(pyLIMA_parameters, 'fsource_' + ref_tel.name)
+        f_blend = getattr(pyLIMA_parameters, 'fblend_' + ref_tel.name)
 
-    pyLIMA_parameters = fit.model.compute_pyLIMA_parameters(best_parameters)
+        # model_magnification = (model['photometry']-f_blend)/f_source
 
-    fig_size = [10, 10]
-    figure_trajectory = plt.figure(figsize=(fig_size[0], fig_size[1]), dpi=75)
+        ref_names.append(ref_tel.name)
+        ref_locations.append(ref_tel.location)
+        ref_magnification.append(model_magnification)
+        ref_fluxes.append([f_source, f_blend])
 
-    figure_axes = figure_trajectory.add_subplot(111, aspect=1)
-    plt.subplots_adjust(top=0.9, bottom=0.1, wspace=0.1, hspace=0.1)
+    for ind, tel in enumerate(microlensing_model.event.telescopes):
 
-    for telescope in fit.event.fake_telescopes:
+        if tel.lightcurve_flux is not None:
 
-        platform = 'Earth'
-        if telescope.location == 'Space':
-            platform = telescope.name
+            if tel.location == 'Earth':
 
-        reference_telescope = telescope
+                ref_index = np.where(np.array(ref_locations) == 'Earth')[0][0]
 
-        telescope_index = [i for i in range(len(fit.event.telescopes)) if
-                           fit.event.telescopes[i].name == telescope.name][0]
+            else:
 
-        fit.model.find_origin(pyLIMA_parameters)
-        to, uo = fit.model.uo_to_from_uc_tc(pyLIMA_parameters)
+                ref_index = np.where(np.array(ref_names) == tel.name)[0][0]
 
-        trajectory_x, trajectory_y, separation = fit.model.source_trajectory(reference_telescope,
-                                                                             to, uo,
-                                                                             pyLIMA_parameters.tE,
-                                                                             pyLIMA_parameters)
+            residus_in_mag = \
+                pyLIMA.fits.objective_functions.photometric_residuals_in_magnitude(
+                    tel, microlensing_model,
+                    pyLIMA_parameters)
+            if ind == 0:
+                reference_source = ref_fluxes[ind][0]
+                reference_blend = ref_fluxes[ind][1]
+                index += 1
+
+            # time_mask = [False for i in range(len(ref_magnification[ref_index]))]
+            time_mask = []
+            for time in tel.lightcurve_flux['time'].value:
+                time_index = np.where(list_of_telescopes[ref_index].lightcurve_flux[
+                                          'time'].value == time)[0][0]
+                time_mask.append(time_index)
+
+            # model_flux = ref_fluxes[ref_index][0] * ref_magnification[ref_index][
+            #    time_mask] + ref_fluxes[ref_index][1]
+            model_flux = reference_source * ref_magnification[ref_index][
+                time_mask] + reference_blend
+            magnitude = pyLIMA.toolbox.brightness_transformation.ZERO_POINT - 2.5 * \
+                        np.log10(model_flux)
+
+            color = plt.rcParams["axes.prop_cycle"].by_key()["color"][ind]
+            marker = str(MARKER_SYMBOLS[0][ind])
+
+            plots.plot_light_curve_magnitude(tel.lightcurve_magnitude['time'].value,
+                                             magnitude + residus_in_mag,
+                                             tel.lightcurve_magnitude['err_mag'].value,
+                                             figure_axe=figure_axe, color=color,
+                                             marker=marker, name=tel.name)
+
+            if bokeh_plot is not None:
+
+                bokeh_plot.scatter(tel.lightcurve_magnitude['time'].value,
+                                   magnitude + residus_in_mag,
+                                   color=color,
+                                   size=5, legend_label=tel.name,
+                                   muted_color=color,
+                                   muted_alpha=0.2)
+
+                err_xs = []
+                err_ys = []
+
+                for x, y, yerr in zip(tel.lightcurve_magnitude['time'].value,
+                                      magnitude + residus_in_mag,
+                                      tel.lightcurve_magnitude['err_mag'].value):
+                    err_xs.append((x, x))
+                    err_ys.append((y - yerr, y + yerr))
+
+                bokeh_plot.multi_line(err_xs, err_ys, color=color,
+                                      legend_label=tel.name,
+                                      muted_color=color,
+                                      muted_alpha=0.2)
+
+
+def plot_residuals(figure_axe, microlensing_model, model_parameters, bokeh_plot=None,
+                   plot_unit='Mag'):
+    pyLIMA_parameters = microlensing_model.compute_pyLIMA_parameters(model_parameters)
+
+    # plot residuals
+
+    for ind, tel in enumerate(microlensing_model.event.telescopes):
+
+        if tel.lightcurve_flux is not None:
+            residus_in_mag = \
+                pyLIMA.fits.objective_functions.photometric_residuals_in_magnitude(
+                    tel, microlensing_model, pyLIMA_parameters)
+
+            color = plt.rcParams["axes.prop_cycle"].by_key()["color"][ind]
+            marker = str(MARKER_SYMBOLS[0][ind])
+
+            plots.plot_light_curve_magnitude(tel.lightcurve_magnitude['time'].value,
+                                             residus_in_mag,
+                                             tel.lightcurve_magnitude['err_mag'].value,
+                                             figure_axe=figure_axe, color=color,
+                                             marker=marker, name=tel.name)
 
-        figure_axes.plot(trajectory_x, trajectory_y,
-                         c=plt.rcParams["axes.prop_cycle"].by_key()["color"][telescope_index],
-                         label=platform)
-        bokeh_geometry.line(trajectory_x, trajectory_y,
-                            color=plt.rcParams["axes.prop_cycle"].by_key()["color"][telescope_index],
-                            legend=platform)
+        if bokeh_plot is not None:
 
-        for index in [-1, 0, 1]:
+            bokeh_plot.scatter(tel.lightcurve_magnitude['time'].value,
+                               residus_in_mag,
+                               color=color,
+                               size=5,
+                               muted_color=color,
+                               muted_alpha=0.2)
 
-            try:
-                index = np.argmin(np.abs(telescope.lightcurve_magnitude[:, 0] -
-                                         (pyLIMA_parameters.to + index * pyLIMA_parameters.tE)))
-                sign = np.sign(trajectory_x[index+1]-trajectory_x[index])
-                derivative = (trajectory_y[index - 1] - trajectory_y[index + 1]) / (
-                        trajectory_x[index - 1] - trajectory_x[index + 1])
-
-                figure_axes.annotate('', xy=(trajectory_x[index], trajectory_y[index]),
-                                     xytext=(trajectory_x[index] - sign* 0.001, trajectory_y[index] - sign* 0.001 * derivative),
-                                     arrowprops=dict(arrowstyle="->", mutation_scale=35,
-                                                     color=plt.rcParams["axes.prop_cycle"].by_key()["color"][
-                                                         telescope_index]))
-
-                bokeh_geometry.add_layout(Arrow(end=OpenHead(line_color=
-                                                             plt.rcParams["axes.prop_cycle"].by_key()["color"][
-                                                                 telescope_index]),
-                                                x_start=trajectory_x[index], y_start=trajectory_y[index],
-                                                x_end=trajectory_x[index] + sign*0.001,
-                                                y_end=trajectory_y[index] + sign*0.001 * derivative
-                                                ))
-            except:
-                pass
-        if fit.model.model_type == 'DSPL':
-            trajectory_x, trajectory_y, separation = fit.model.source_trajectory(reference_telescope,
-                                                                                 pyLIMA_parameters.to + pyLIMA_parameters.delta_to,
-                                                                                 pyLIMA_parameters.uo + pyLIMA_parameters.delta_uo,
-                                                                                 pyLIMA_parameters.tE,
-                                                                                 pyLIMA_parameters)
+            err_xs = []
+            err_ys = []
 
-            figure_axes.plot(trajectory_x, trajectory_y,
-                             c=plt.rcParams["axes.prop_cycle"].by_key()["color"][telescope_index], alpha=0.5)
+            for x, y, yerr in zip(tel.lightcurve_magnitude['time'].value,
+                                  residus_in_mag,
+                                  tel.lightcurve_magnitude['err_mag'].value):
+                err_xs.append((x, x))
+                err_ys.append((y - yerr, y + yerr))
 
-            bokeh_geometry.line(trajectory_x, trajectory_y,
-                                color=plt.rcParams["axes.prop_cycle"].by_key()["color"][telescope_index], alpha=0.5,
-                                legend=platform)
-
-    if 'BL' in fit.model.model_type:
-        regime, caustics, cc = microlcaustics.find_2_lenses_caustics_and_critical_curves(
-            10 ** pyLIMA_parameters.logs,
-            10 ** pyLIMA_parameters.logq,
-            resolution=5000)
-        for count, caustic in enumerate(caustics):
+            bokeh_plot.multi_line(err_xs, err_ys, color=color,
+                                  muted_color=color,
+                                  muted_alpha=0.2)
 
-            try:
-                figure_axes.plot(caustic.real, caustic.imag, lw=3, c='r')
-                figure_axes.plot(cc[count].real, cc[count].imag, '--k')
+    figure_axe.set_ylim([-0.1, 0.1])
 
-                bokeh_geometry.line(caustic.real, caustic.imag,
-                                    color='red', line_width=3)
-                bokeh_geometry.line(cc[count].real, cc[count].imag, line_dash='dashed',
-                                    color='black')
-            except AttributeError:
-                pass
 
-    else:
+def plot_distribution(samples, parameters_names=None, bokeh_plot=None):
+    names = [str(i) for i in range(len(parameters_names))]
 
-        figure_axes.scatter(0, 0, s=10, c='r')
-        bokeh_geometry.scatter(0, 0, color='red')
+    GTC = pygtc.plotGTC(chains=[samples], sigmaContourLevels=True, paramNames=names,
+                        customLabelFont={'family': 'serif', 'size': 14},
+                        customLegendFont={'family': 'serif', 'size': 14},
+                        customTickFont={'family': 'serif', 'size': 7}, nContourLevels=3)
 
-        einstein_ring = plt.Circle((0, 0), 1, fill=False, color='k', linestyle='--')
-        figure_axes.add_artist(einstein_ring)
+    text = [names[i] + ' : ' + parameters_names[i] + '\n' for i in
+            range(len(parameters_names))]
+    GTC.text(0.71, .41, ''.join(text), size=15)
 
-        bokeh_geometry.circle(0, 0, radius=1, line_dash='dashed', line_color='black', fill_color=None)
+    if bokeh_plot is not None:
+        # Not implemented yet
+        pass
 
-    for telescope_index, telescope in enumerate(fit.event.telescopes):
+    return GTC, bokeh_plot
 
-        fit.model.find_origin(pyLIMA_parameters)
-        to, uo = fit.model.uo_to_from_uc_tc(pyLIMA_parameters)
 
-        trajectory_x, trajectory_y, separation = fit.model.source_trajectory(telescope,
-                                                                             to, uo,
-                                                                             pyLIMA_parameters.tE,
-                                                                             pyLIMA_parameters)
+def plot_parameters_table(samples, parameters_names=None, bokeh_plot=None):
+    percentiles = np.percentile(samples, [16, 50, 84], axis=0)
 
-        if 'rho' in pyLIMA_parameters._fields:
+    table_val = [[r'$' + str(percentiles[1][i]) + '^{+' + str(
+        percentiles[2][i] - percentiles[1][i]) + '}_{-' + str(
+        percentiles[1][i] - percentiles[0][i]) + '}$'] for i in
+                 range(len(percentiles[0]))]
+    raw_labels = parameters_names
 
-            rho = pyLIMA_parameters.rho
-        else:
-            rho = 10 ** -3
+    table_colors = []
+    raw_colors = []
+    last_color = 'dodgerblue'
 
-        patches = [plt.Circle((x, y), rho, color=plt.rcParams["axes.prop_cycle"].by_key()["color"][telescope_index],
-                              alpha=0.2) for x, y in zip(trajectory_x, trajectory_y)]
-        coll = matplotlib.collections.PatchCollection(patches, match_original=True)
+    for i in range(len(table_val)):
+        table_colors.append([last_color])
+        raw_colors.append(last_color)
 
-        figure_axes.scatter(trajectory_x, trajectory_y,
-                            c=plt.rcParams["axes.prop_cycle"].by_key()["color"][telescope_index],
-                            alpha=0.5, label=telescope.name, s=0.1)
+        if last_color == 'dodgerblue':
 
-        figure_axes.add_collection(coll)
+            last_color = 'white'
 
-        bokeh_geometry.circle(trajectory_x, trajectory_y, radius=rho,
-                              color=plt.rcParams["axes.prop_cycle"].by_key()["color"][telescope_index],
-                              radius_dimension = 'max',fill_alpha=0.5)
+        else:
 
-    legend = figure_axes.legend(numpoints=1, loc='best', fancybox=True, framealpha=0.5)
-    for handle in legend.legendHandles:
-        try:
-            handle.set_sizes([100])
-        except:
-            pass
+            last_color = 'dodgerblue'
 
-    figure_axes.xaxis.set_major_locator(MaxNLocator(5))
-    figure_axes.yaxis.set_major_locator(MaxNLocator(5))
-    figure_axes.xaxis.get_major_ticks()[0].draw = lambda *args: None
-    figure_axes.yaxis.get_major_ticks()[0].draw = lambda *args: None
-    figure_axes.xaxis.get_major_ticks()[-1].draw = lambda *args: None
-    figure_axes.yaxis.get_major_ticks()[-1].draw = lambda *args: None
+    # column_labels = ['Parameters', 'Values']
 
-    figure_axes.set_xlabel(r'$x(\theta_E)$', fontsize=25)
-    figure_axes.set_ylabel(r'$y(\theta_E)$', fontsize=25)
-    figure_axes.tick_params(axis='x', labelsize=15)
-    figure_axes.tick_params(axis='y', labelsize=15)
+    fig_size = [10, 7.5]
+    figure_table = plt.figure(figsize=(fig_size[0], fig_size[1]), dpi=75)
+    table_axes = figure_table.add_subplot(111, aspect=1)
+    ax = plt.gca()
+    ax.get_xaxis().set_visible(False)
+    ax.get_yaxis().set_visible(False)
+    plt.box(on=None)
+    the_table = table_axes.table(cellText=table_val, loc='center', rowLabels=raw_labels,
+                                 cellColours=table_colors, rowColours=raw_colors,
+                                 colWidths=[.5] * 2)
+    the_table.set_fontsize(25)
+    breakpoint()
+
+    # the_table = table_axes.table(cellText=table_val, cellColours=table_colors,
+    # rowColours=raw_colors,
+    #                             rowLabels=raw_labels,
+    ##                             colLabels=column_labels, loc='center left',
+    #                            rowLoc='left', colLoc='center',
+    #                            bbox=[0.0, -0.0, 1.0, 1.0]
+    #                            )
 
-    figure_axes.axis([-3, 3, -3, 3])
-    title = fit.model.event.name + ' : ' + fit.model.model_type
-    figure_trajectory.suptitle(title, fontsize=30 * fig_size[0] / len(title))
-    return figure_trajectory, bokeh_geometry
+    return figure_table
```

### Comparing `pyLIMA-0.8.3/pyLIMA/microlstats.py` & `pyLIMA-1.9/pyLIMA/fits/stats.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-import scipy.stats as ss
 import numpy as np
-#import statsmodels.api as sm
-
-### Tests on residuals
+import scipy.stats as ss
 
 
 def normal_Kolmogorov_Smirnov(sample):
     """The moon illumination expressed as a percentage.
 
                 :param astropy sun: the sun ephemeris
                 :param astropy moon: the moon ephemeris
@@ -14,124 +11,132 @@
                 :return: a numpy array like indicated the moon illumination.
 
                 :rtype: array_like
 
     """
 
     mu, sigma = ss.norm.fit(sample)
-    #use mu sigma for anomaly, 0,1 for rescaling???
+    # use mu sigma for anomaly, 0,1 for rescaling???
     KS_stat, KS_pvalue = ss.kstest(sample, 'norm', args=(0, 1))
 
-    # the sample is likely Gaussian-like if KS_stat (~ maximum distance between sample and theoritical distribution) -> 0
-    # the null hypothesis can not be rejected ( i.e the distribution of sample come from a Gaussian) if KS_pvalue -> 1
+    # the sample is likely Gaussian-like if KS_stat (~ maximum distance between
+    # sample and theoritical distribution) -> 0
+    # the null hypothesis can not be rejected ( i.e the distribution of sample come
+    # from a Gaussian) if KS_pvalue -> 1
 
     KS_judgement = 0
 
     if KS_pvalue > 0.01:
-
         KS_judgement = 1
 
     if KS_pvalue > 0.05:
-
         KS_judgement = 2
 
     return KS_stat, KS_pvalue, KS_judgement
 
+
 def normal_Anderson_Darling(sample):
-    """Compute a Anderson-Darling test on the sample versus a normal distribution with mu = 0, sigma = 1
+    """Compute a Anderson-Darling tests on the sample versus a normal distribution
+    with mu = 0, sigma = 1
 
             :param array_like sample: the sample you want to check the "Gaussianity"
-            :returns: the Anderson-Darling statistic, the Anderson-Darling critical values associated to the significance
+            :returns: the Anderson-Darling statistic, the Anderson-Darling critical
+            values associated to the significance
             level of 15 % and the Anderson-Darling judgement
             :rtype: float, array_like, array_like
     """
 
     AD_stat, AD_critical_values, AD_significance_levels = ss.anderson(sample)
 
-    # the sample is likely Gaussian-like if AD_stat (~ maximum distance between sample and theoritical distribution) -> 0
-    # the null hypothesis can not be rejected ( i.e the distribution of sample come from a Gaussian) if AD_pvalue -> 1
-
+    # the sample is likely Gaussian-like if AD_stat (~ maximum distance between
+    # sample and theoritical distribution) -> 0
+    # the null hypothesis can not be rejected ( i.e the distribution of sample come
+    # from a Gaussian) if AD_pvalue -> 1
 
     AD_judgement = 0
 
-    if AD_stat < 2*AD_critical_values[-1]:
+    if AD_stat < 2 * AD_critical_values[-1]:
         AD_judgement = 1
 
     if AD_stat < AD_critical_values[-1]:
         AD_judgement = 2
-    return  AD_stat, AD_critical_values[-1], AD_judgement
+    return AD_stat, AD_critical_values[-1], AD_judgement
+
 
 def normal_Shapiro_Wilk(sample):
-    """Compute a Shapiro-Wilk test on the sample versus a normal distribution with mu = 0, sigma = 1
+    """Compute a Shapiro-Wilk tests on the sample versus a normal distribution with
+    mu = 0, sigma = 1
 
             :param array_like sample: the sample you want to check the "Gaussianity"
             :returns: the Shapiro-Wilk statistic and its related p_value
             :rtype: float, float
     """
 
     SW_stat, SW_pvalue = ss.shapiro(sample)
 
-    # the null hypothesis can not be rejected ( i.e the distribution of sample come from a Gaussian) if SW_stat -> 1
-    # the null hypothesis can not be rejected ( i.e the distribution of sample come from a Gaussian) if SW_pvalue -> 1
+    # the null hypothesis can not be rejected ( i.e the distribution of sample come
+    # from a Gaussian) if SW_stat -> 1
+    # the null hypothesis can not be rejected ( i.e the distribution of sample come
+    # from a Gaussian) if SW_pvalue -> 1
 
-    # Judegement made on the STATISTIC because 'W test statistic is accurate but the p-value may not be" (see scipy doc)
+    # Judegement made on the STATISTIC because 'W tests statistic is accurate but the
+    # p-value may not be" (see scipy doc)
     SW_judgement = 0
 
     if SW_pvalue > 0.01:
         SW_judgement = 1
 
     if SW_pvalue > 0.05:
         SW_judgement = 2
 
-
-    return  SW_stat, SW_pvalue, SW_judgement
+    return SW_stat, SW_pvalue, SW_judgement
 
 
 ### Statistics fit quality metrics
 
-def normalized_chi2(chi2, n_data, n_parameters) :
+def normalized_chi2(chi2, n_data, n_parameters):
     """Compute the chi^2/dof
 
             :param float chi2: the chi^2
             :param int n_data: the number of data_points
             :param int n_parameters: the number of model parameters
 
             :returns: the chi^2/dof and the chi2dof_judgement
             :rtype: float
     """
 
-    chi2_sur_dof = chi2/(n_data-n_parameters)
+    chi2_sur_dof = chi2 / (n_data - n_parameters)
 
     chi2dof_judgement = 0
-    if chi2_sur_dof < 2 :
+    if chi2_sur_dof < 2:
         chi2dof_judgement = 2
 
-    return chi2_sur_dof,chi2dof_judgement
+    return chi2_sur_dof, chi2dof_judgement
+
 
 def Bayesian_Information_Criterion(chi2, n_data, n_parameters):
     """Compute the BIC statistic.
 
             :param float chi2: the chi^2
             :param int n_data: the number of data_points
             :param int n_parameters: the number of model parameters
 
             :returns: the chi^2/dof
             :rtype: float
     """
-    BIC = chi2 + n_parameters*np.log(n_data)
+    BIC = chi2 + n_parameters * np.log(n_data)
 
     return BIC
 
+
 def Akaike_Information_Criterion(chi2, n_parameters):
     """Compute the BIC statistic.
 
             :param float chi2: the chi^2
             :param int n_parameters: the number of model parameters
 
             :returns: the chi^2/dof
             :rtype: float
     """
-    AIC = chi2 + 2*n_parameters
+    AIC = chi2 + 2 * n_parameters
 
     return AIC
-
-
```

### Comparing `pyLIMA-0.8.3/pyLIMA/stars.py` & `pyLIMA-1.9/pyLIMA/stars/stars.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,24 +2,25 @@
 """
 Created on Thu March 03 12:51:19 2017
 
 @author: ebachelet
 """
 
 from __future__ import division
-import pkg_resources
 
-import numpy as np
-import os
 import astropy.io.fits as fits
+import numpy as np
+import pkg_resources
 import scipy.interpolate as si
-resource_package = __name__
-resource_path = '/'.join(('data', 'Claret2011.fits'))
-template = pkg_resources.resource_filename(resource_package, resource_path)
 
+resource_path = '/'.join(('data', 'Yoo_B0B1.dat'))
+template = pkg_resources.resource_filename('pyLIMA', resource_path)
+
+resource_path = '/'.join(('data', 'Claret2011.fits'))
+template = pkg_resources.resource_filename('pyLIMA', resource_path)
 
 CLARET_PATH = template
 
 
 class Star(object):
     """
        ######## Star module ########
@@ -36,70 +37,74 @@
 
         metallicity : The star metallicity in solar unit. Default is 0.0.
 
         mass : the mass in solar unit.
 
         gammas : (Microlensing covention) List of limb darkening coefficient
                  :math:`\\Gamma` associated to all filters.
-                 The classical (Milne definition) linear limb darkening coefficient can be found using:
+                 The classical (Milne definition) linear limb darkening coefficient
+                 can be found using:
                  u=(3*gamma)/(2+gamma).
                  Default is an empty list.
     """
 
     def __init__(self):
-
         self.name = 'Random star'
         self.T_eff = 5000  # Kelvins
         self.log_g = 4
         self.metallicity = 0.0  # Sun metallicity by default
-        self.turbulent_velocity = 2.0 # km/s
+        self.turbulent_velocity = 2.0  # km/s
         self.mass = 1.0  # Solar mass unit
         self.gammas = []  # microlensing limb-darkening coefficient
 
         claret_path = CLARET_PATH
         claret_table = fits.open(claret_path)
 
-        self.claret_table = np.array([claret_table[1].data['log g'], claret_table[1].data['Teff (K)'],
-                             claret_table[1].data['Z (Sun)'], claret_table[1].data['Xi (km/s)'],
-                             claret_table[1].data['u'], claret_table[1].data['filter']]).T
+        self.claret_table = np.array(
+            [claret_table[1].data['log g'], claret_table[1].data['Teff (K)'],
+             claret_table[1].data['Z (Sun)'], claret_table[1].data['Xi (km/s)'],
+             claret_table[1].data['u'], claret_table[1].data['filter']]).T
 
         self.define_claret_filter_tables()
 
     def define_claret_filter_tables(self):
         """
-            Define the filter_claret table. For more details, see " Gravity and limb-darkening coefficients for
+            Define the filter_claret table. For more details, see " Gravity and
+            limb-darkening coefficients for
             the Kepler, CoRoT,
             Spitzer, uvby,   UBVRIJHK,
             and Sloan photometric systems"
             Claret, A. and Bloemen, S. 2011A&A...529A..75C.
         """
-        all_filters = np.unique(self.claret_table[:,-1])
+        all_filters = np.unique(self.claret_table[:, -1])
         self.filter_claret_table = {}
 
         for filter in all_filters:
+            good_filter = np.where(self.claret_table[:, -1] == filter)[0]
 
-            good_filter  = np.where(self.claret_table[:,-1] == filter)[0]
-
-            subclaret = self.claret_table[good_filter,:-1].astype(float)
+            subclaret = self.claret_table[good_filter, :-1].astype(float)
 
-            grid_interpolation = si.NearestNDInterpolator(subclaret[:,:-1],subclaret[:,-1])
+            grid_interpolation = si.NearestNDInterpolator(subclaret[:, :-1],
+                                                          subclaret[:, -1])
 
             self.filter_claret_table[filter] = grid_interpolation
 
     def find_gamma(self, filter):
         """
-        Set the associated :math:`\\Gamma` linear limb-darkening coefficient associated to the filter.
+        Set the associated :math:`\\Gamma` linear limb-darkening coefficient
+        associated to the filter.
 
         :param str filter: the observation filter. Need to match Claret definitions.
         :return: the (microlensing) gamma coefficient
         :rtype: float
         """
 
         good_table = self.filter_claret_table[filter]
 
+        linear_limb_darkening_coefficient = good_table(self.log_g, self.T_eff,
+                                                       self.metallicity,
+                                                       self.turbulent_velocity)
 
-
-        linear_limb_darkening_coefficient = good_table(self.log_g, self.T_eff, self.metallicity, self.turbulent_velocity)
-
-        gamma = 2 * linear_limb_darkening_coefficient / (3 - linear_limb_darkening_coefficient)
+        gamma = 2 * linear_limb_darkening_coefficient / (
+                3 - linear_limb_darkening_coefficient)
 
         return gamma
```

