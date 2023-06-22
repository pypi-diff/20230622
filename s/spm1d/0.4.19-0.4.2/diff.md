# Comparing `tmp/spm1d-0.4.19.tar.gz` & `tmp/spm1d-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spm1d-0.4.19.tar", last modified: Thu Jun 22 05:30:02 2023, max compression
+gzip compressed data, was "dist/spm1d-0.4.2.tar", last modified: Thu Aug 22 08:58:12 2019, max compression
```

## Comparing `spm1d-0.4.19.tar` & `spm1d-0.4.2.tar`

### file list

```diff
@@ -1,492 +1,487 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:30:02.094641 spm1d-0.4.19/
--rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-06-22 05:29:52.000000 spm1d-0.4.19/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-22 05:29:52.000000 spm1d-0.4.19/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-22 05:30:02.094641 spm1d-0.4.19/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-06-22 05:29:52.000000 spm1d-0.4.19/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-22 05:30:02.094641 spm1d-0.4.19/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-22 05:29:52.000000 spm1d-0.4.19/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:30:02.042640 spm1d-0.4.19/spm1d/
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10320 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:30:02.046640 spm1d-0.4.19/spm1d/data/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8227 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:30:02.062640 spm1d-0.4.19/spm1d/data/datafiles/
--rw-r--r--   0 runner    (1001) docker     (123)    29533 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/Besier2009kneeflexion.npz
--rw-r--r--   0 runner    (1001) docker     (123)   282313 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/Besier2009muscleforces.npz
--rw-r--r--   0 runner    (1001) docker     (123)    44022 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/Dorn2012.npz
--rw-r--r--   0 runner    (1001) docker     (123)    37636 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/Neptune1999kneekin.npz
--rw-r--r--   0 runner    (1001) docker     (123)    30624 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/Pataky2014cop.npz
--rw-r--r--   0 runner    (1001) docker     (123)    23431 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/ex_grf_means.npz
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/ex_grf_speeds.npy
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/ex_grf_speeds_cond.npy
--rw-r--r--   0 runner    (1001) docker     (123)    48560 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/ex_grf_subj000.npy
--rw-r--r--   0 runner    (1001) docker     (123)    48560 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/ex_grf_subj001.npy
--rw-r--r--   0 runner    (1001) docker     (123)    48560 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/ex_grf_subj002.npy
--rw-r--r--   0 runner    (1001) docker     (123)    48560 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/ex_grf_subj003.npy
--rw-r--r--   0 runner    (1001) docker     (123)    48560 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/ex_grf_subj004.npy
--rw-r--r--   0 runner    (1001) docker     (123)    48560 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/ex_grf_subj005.npy
--rw-r--r--   0 runner    (1001) docker     (123)    48560 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/ex_grf_subj006.npy
--rw-r--r--   0 runner    (1001) docker     (123)    48560 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/ex_grf_subj007.npy
--rw-r--r--   0 runner    (1001) docker     (123)    48560 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/ex_grf_subj008.npy
--rw-r--r--   0 runner    (1001) docker     (123)    48560 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/ex_grf_subj009.npy
--rw-r--r--   0 runner    (1001) docker     (123)    24320 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/ex_kinematics.npy
--rw-r--r--   0 runner    (1001) docker     (123)    29875 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/ex_kinematics_for_interpolation.npy
--rw-r--r--   0 runner    (1001) docker     (123)     9776 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/ex_sim_twolocalmax.npy
--rw-r--r--   0 runner    (1001) docker     (123)    11291 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/my_spmT.npz
--rw-r--r--   0 runner    (1001) docker     (123)    12770 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/my_spmTi.npz
--rw-r--r--   0 runner    (1001) docker     (123)     9776 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/normality_dataset_A1.npy
--rw-r--r--   0 runner    (1001) docker     (123)     8160 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/normality_dataset_A10.npy
--rw-r--r--   0 runner    (1001) docker     (123)    80880 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/normality_dataset_A11.npy
--rw-r--r--   0 runner    (1001) docker     (123)   808080 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/normality_dataset_A12.npy
--rw-r--r--   0 runner    (1001) docker     (123)   808080 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/normality_dataset_A13.npy
--rw-r--r--   0 runner    (1001) docker     (123)   808080 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/normality_dataset_A14.npy
--rw-r--r--   0 runner    (1001) docker     (123)   404080 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/normality_dataset_A15.npy
--rw-r--r--   0 runner    (1001) docker     (123)   404080 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/normality_dataset_A16.npy
--rw-r--r--   0 runner    (1001) docker     (123)   404080 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/normality_dataset_A17.npy
--rw-r--r--   0 runner    (1001) docker     (123)     9776 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/normality_dataset_A2.npy
--rw-r--r--   0 runner    (1001) docker     (123)     9776 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/normality_dataset_A3.npy
--rw-r--r--   0 runner    (1001) docker     (123)     8160 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/normality_dataset_A4.npy
--rw-r--r--   0 runner    (1001) docker     (123)    32400 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/normality_dataset_A5.npy
--rw-r--r--   0 runner    (1001) docker     (123)   404080 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/normality_dataset_A6.npy
--rw-r--r--   0 runner    (1001) docker     (123)    16240 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/normality_dataset_A7.npy
--rw-r--r--   0 runner    (1001) docker     (123)    16240 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/normality_dataset_A8.npy
--rw-r--r--   0 runner    (1001) docker     (123)    16240 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/normality_dataset_A9.npy
--rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/random.npy
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/random_rough.npy
--rw-r--r--   0 runner    (1001) docker     (123)     8160 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/simscalar_datasetA.npy
--rw-r--r--   0 runner    (1001) docker     (123)     8160 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/simscalar_datasetB.npy
--rw-r--r--   0 runner    (1001) docker     (123)     8160 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/simscalar_datasetC.npy
--rw-r--r--   0 runner    (1001) docker     (123)    17000 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova2_2x2.npz
--rw-r--r--   0 runner    (1001) docker     (123)    49960 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova2_2x3.npz
--rw-r--r--   0 runner    (1001) docker     (123)    59848 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova2_3x3.npz
--rw-r--r--   0 runner    (1001) docker     (123)   119176 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova2_3x4.npz
--rw-r--r--   0 runner    (1001) docker     (123)    87040 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova2_3x5.npz
--rw-r--r--   0 runner    (1001) docker     (123)   105992 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova2_4x4.npz
--rw-r--r--   0 runner    (1001) docker     (123)   198280 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova2_4x5.npz
--rw-r--r--   0 runner    (1001) docker     (123)    17000 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova2nested_2x2.npz
--rw-r--r--   0 runner    (1001) docker     (123)    49960 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova2nested_2x3.npz
--rw-r--r--   0 runner    (1001) docker     (123)    37600 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova2nested_3x3.npz
--rw-r--r--   0 runner    (1001) docker     (123)    89512 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova2nested_3x4.npz
--rw-r--r--   0 runner    (1001) docker     (123)   185920 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova2nested_3x5.npz
--rw-r--r--   0 runner    (1001) docker     (123)    66440 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova2nested_4x4.npz
--rw-r--r--   0 runner    (1001) docker     (123)   115880 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova2nested_4x5.npz
--rw-r--r--   0 runner    (1001) docker     (123)    17332 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova2onerm_2x2.npz
--rw-r--r--   0 runner    (1001) docker     (123)    45620 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova2onerm_2x3.npz
--rw-r--r--   0 runner    (1001) docker     (123)    38132 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova2onerm_3x3.npz
--rw-r--r--   0 runner    (1001) docker     (123)    90548 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova2onerm_3x4.npz
--rw-r--r--   0 runner    (1001) docker     (123)   187892 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova2onerm_3x5.npz
--rw-r--r--   0 runner    (1001) docker     (123)    67252 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova2onerm_4x4.npz
--rw-r--r--   0 runner    (1001) docker     (123)   117172 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova2onerm_4x5.npz
--rw-r--r--   0 runner    (1001) docker     (123)    23988 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova2rm_2x2.npz
--rw-r--r--   0 runner    (1001) docker     (123)    60596 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova2rm_2x3.npz
--rw-r--r--   0 runner    (1001) docker     (123)    38132 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova2rm_3x3.npz
--rw-r--r--   0 runner    (1001) docker     (123)    90548 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova2rm_3x4.npz
--rw-r--r--   0 runner    (1001) docker     (123)    88052 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova2rm_3x5.npz
--rw-r--r--   0 runner    (1001) docker     (123)    67252 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova2rm_4x4.npz
--rw-r--r--   0 runner    (1001) docker     (123)   133812 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova2rm_4x5.npz
--rw-r--r--   0 runner    (1001) docker     (123)    33966 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova3_2x2x2.npz
--rw-r--r--   0 runner    (1001) docker     (123)   100526 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova3_2x3x4.npz
--rw-r--r--   0 runner    (1001) docker     (123)    53934 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova3nested_2x2x2.npz
--rw-r--r--   0 runner    (1001) docker     (123)   133806 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova3nested_2x4x2.npz
--rw-r--r--   0 runner    (1001) docker     (123)    34458 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova3onerm_2x2x2.npz
--rw-r--r--   0 runner    (1001) docker     (123)   101658 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova3onerm_2x3x4.npz
--rw-r--r--   0 runner    (1001) docker     (123)    34458 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova3rm_2x2x2.npz
--rw-r--r--   0 runner    (1001) docker     (123)   101658 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova3rm_2x3x4.npz
--rw-r--r--   0 runner    (1001) docker     (123)    34458 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova3tworm_2x2x2.npz
--rw-r--r--   0 runner    (1001) docker     (123)   101658 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova3tworm_2x3x4.npz
--rw-r--r--   0 runner    (1001) docker     (123)    98728 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/datafiles/weather.npz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:30:02.062640 spm1d-0.4.19/spm1d/data/mv0d/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/mv0d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/mv0d/cca.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/mv0d/hotellings1.py
--rw-r--r--   0 runner    (1001) docker     (123)    17491 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/mv0d/hotellings2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/mv0d/hotellings_paired.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/mv0d/manova1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:30:02.062640 spm1d-0.4.19/spm1d/data/mv1d/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/mv1d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/mv1d/cca.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/mv1d/hotellings2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/mv1d/hotellings_paired.py
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/mv1d/manova1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:30:02.066640 spm1d-0.4.19/spm1d/data/uv0d/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/uv0d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/uv0d/anova1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/uv0d/anova1rm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7115 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/uv0d/anova2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/uv0d/anova2nested.py
--rw-r--r--   0 runner    (1001) docker     (123)    11566 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/uv0d/anova2onerm.py
--rw-r--r--   0 runner    (1001) docker     (123)     8115 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/uv0d/anova2rm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/uv0d/anova3.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/uv0d/anova3nested.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/uv0d/anova3onerm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/uv0d/anova3rm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/uv0d/anova3tworm.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/uv0d/ci1.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/uv0d/ci2.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/uv0d/cipaired.py
--rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/uv0d/normality.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/uv0d/regress.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/uv0d/t1.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/uv0d/t2.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/uv0d/t2nonspher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/uv0d/tpaired.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:30:02.066640 spm1d-0.4.19/spm1d/data/uv1d/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/uv1d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/uv1d/anova1.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/uv1d/anova1rm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/uv1d/anova2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/uv1d/anova2nested.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/uv1d/anova2onerm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/uv1d/anova2rm.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/uv1d/anova3.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/uv1d/anova3nested.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/uv1d/anova3onerm.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/uv1d/anova3rm.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/uv1d/anova3tworm.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/uv1d/normality.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/uv1d/regress.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/uv1d/t1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/uv1d/t2.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/data/uv1d/tpaired.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:30:02.042640 spm1d-0.4.19/spm1d/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:30:02.066640 spm1d-0.4.19/spm1d/examples/io/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:30:02.066640 spm1d-0.4.19/spm1d/examples/io/data/
--rw-r--r--   0 runner    (1001) docker     (123)    24424 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/io/data/ex_kinematics.mat
--rw-r--r--   0 runner    (1001) docker     (123)    24755 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/io/data/ex_kinematics.txt
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/io/ex_import_mat.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/io/ex_import_txt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:30:02.042640 spm1d-0.4.19/spm1d/examples/nonparam/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:30:02.070640 spm1d-0.4.19/spm1d/examples/nonparam/0d/
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/0d/ex_anova1.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/0d/ex_anova1rm.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/0d/ex_anova2.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/0d/ex_anova2nested.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/0d/ex_anova2onerm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/0d/ex_anova2rm.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/0d/ex_anova3.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/0d/ex_anova3nested.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/0d/ex_anova3onerm.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/0d/ex_anova3rm.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/0d/ex_anova3tworm.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/0d/ex_cca.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/0d/ex_ci_onesample.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/0d/ex_ci_pairedsample.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/0d/ex_ci_twosample.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/0d/ex_hotellings.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/0d/ex_hotellings2.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/0d/ex_hotellings_paired.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/0d/ex_manova1.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/0d/ex_regress.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/0d/ex_ttest.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/0d/ex_ttest2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/0d/ex_ttest2_standalone.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/0d/ex_ttest_paired.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/0d/ex_ttest_standalone.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:30:02.070640 spm1d-0.4.19/spm1d/examples/nonparam/1d/
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/1d/ex_anova1.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/1d/ex_anova1rm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/1d/ex_anova2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/1d/ex_anova2nested.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/1d/ex_anova2onerm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/1d/ex_anova2rm.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/1d/ex_anova3.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/1d/ex_anova3nested.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/1d/ex_anova3onerm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/1d/ex_anova3rm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/1d/ex_anova3tworm.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/1d/ex_cca.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/1d/ex_ci_onesample.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/1d/ex_ci_pairedsample.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/1d/ex_ci_twosample.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/1d/ex_hotellings.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/1d/ex_hotellings2.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/1d/ex_hotellings_paired.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/1d/ex_manova1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/1d/ex_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/1d/ex_ttest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/1d/ex_ttest2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/1d/ex_ttest2_circular.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/1d/ex_ttest_other_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/1d/ex_ttest_paired.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:30:02.074640 spm1d-0.4.19/spm1d/examples/nonparam/1d/roi/
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/1d/roi/ex_anova1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/1d/roi/ex_anova1rm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/1d/roi/ex_anova2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/1d/roi/ex_anova2nested.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/1d/roi/ex_anova2onerm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/1d/roi/ex_anova2rm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/1d/roi/ex_anova3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/1d/roi/ex_anova3nested.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/1d/roi/ex_anova3onerm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/1d/roi/ex_anova3rm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/1d/roi/ex_anova3tworm.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/1d/roi/ex_cca.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/1d/roi/ex_hotellings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/1d/roi/ex_hotellings2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/1d/roi/ex_hotellings_paired.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/1d/roi/ex_manova1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/1d/roi/ex_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/1d/roi/ex_ttest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/1d/roi/ex_ttest2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/nonparam/1d/roi/ex_ttest_paired.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:30:02.042640 spm1d-0.4.19/spm1d/examples/normality/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:30:02.074640 spm1d-0.4.19/spm1d/examples/normality/0d/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/normality/0d/ex_anova1.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/normality/0d/ex_anova1rm.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/normality/0d/ex_anova2.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/normality/0d/ex_anova2nested.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/normality/0d/ex_anova2onerm.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/normality/0d/ex_anova2rm.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/normality/0d/ex_anova3.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/normality/0d/ex_anova3nested.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/normality/0d/ex_anova3onerm.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/normality/0d/ex_anova3rm.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/normality/0d/ex_anova3tworm.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/normality/0d/ex_regress.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/normality/0d/ex_ttest.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/normality/0d/ex_ttest2.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/normality/0d/ex_ttest_paired.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:30:02.074640 spm1d-0.4.19/spm1d/examples/normality/1d/
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/normality/1d/ex_anova1.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/normality/1d/ex_anova1rm.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/normality/1d/ex_anova2.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/normality/1d/ex_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/normality/1d/ex_ttest.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/normality/1d/ex_ttest2.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/normality/1d/ex_ttest_paired.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:30:02.074640 spm1d-0.4.19/spm1d/examples/normality/paper/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1897 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/normality/paper/appendix_FigA1.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/normality/paper/appendix_FigA2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1968 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/normality/paper/appendix_FigA3.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1887 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/normality/paper/appendix_FigA4.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1626 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/normality/paper/appendix_FigA5.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1927 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/normality/paper/appendix_FigA6.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1932 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/normality/paper/appendix_FigA7.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:30:02.074640 spm1d-0.4.19/spm1d/examples/processing/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:30:02.074640 spm1d-0.4.19/spm1d/examples/processing/data/
--rw-r--r--   0 runner    (1001) docker     (123)    29875 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/processing/data/ex_kinematics_for_interpolation.npy
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/processing/ex_interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/processing/ex_smooth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:30:02.078641 spm1d-0.4.19/spm1d/examples/scipy/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/scipy/ex_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/scipy/ex_ttest_normality.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/scipy/ex_ttest_onesample.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/scipy/ex_ttest_paired.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/scipy/ex_ttest_twosample.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/scipy/ex_ttest_twosample_unequalvar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:30:02.078641 spm1d-0.4.19/spm1d/examples/stats0d/
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats0d/ex_anova1.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats0d/ex_anova1rm.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats0d/ex_anova2.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats0d/ex_anova2nested.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats0d/ex_anova2onerm.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats0d/ex_anova2onermub.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats0d/ex_anova2rm.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats0d/ex_anova3.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats0d/ex_anova3nested.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats0d/ex_anova3onerm.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats0d/ex_anova3rm.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats0d/ex_anova3tworm.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats0d/ex_cca.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats0d/ex_ci_onesample.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats0d/ex_ci_onesample_standalone.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats0d/ex_ci_pairedsample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats0d/ex_ci_twosample.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats0d/ex_hotellings1.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats0d/ex_hotellings2.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats0d/ex_hotellings_paired.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats0d/ex_manova1.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats0d/ex_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats0d/ex_ttest_onesample.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats0d/ex_ttest_paired.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats0d/ex_ttest_twosample.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats0d/ex_ttest_twosample_unequalvar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:30:02.082641 spm1d-0.4.19/spm1d/examples/stats1d/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats1d/ex_anova1.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats1d/ex_anova1_circular_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats1d/ex_anova1_posthoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats1d/ex_anova1rm.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats1d/ex_anova2.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats1d/ex_anova2nested.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats1d/ex_anova2onerm.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats1d/ex_anova2rm.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats1d/ex_anova3.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats1d/ex_anova3nested.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats1d/ex_anova3onerm.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats1d/ex_anova3rm.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats1d/ex_anova3tworm.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats1d/ex_cca_Dorn2012.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats1d/ex_ci_onesample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats1d/ex_ci_onesample_standalone.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats1d/ex_ci_pairedsample.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats1d/ex_ci_twosample.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats1d/ex_eqvartest.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats1d/ex_glm.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats1d/ex_hotellings2_Besier2009muscleforces.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats1d/ex_hotellings_paired_Neptune1999.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats1d/ex_hotellings_paired_Pataky2014.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats1d/ex_manova1_Dorn2012.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats1d/ex_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats1d/ex_ttest.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats1d/ex_ttest2.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats1d/ex_ttest_paired.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats1d/ex_ttest_roi.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats1d/rfx_0_means.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats1d/rfx_1_level1.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats1d/rfx_2_level2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:30:02.082641 spm1d-0.4.19/spm1d/examples/stats1d_roi/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats1d_roi/ex_anova1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats1d_roi/ex_anova1rm.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats1d_roi/ex_anova2.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats1d_roi/ex_anova2nested.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats1d_roi/ex_anova2onerm.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats1d_roi/ex_anova2rm.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats1d_roi/ex_anova3.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats1d_roi/ex_anova3nested.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats1d_roi/ex_anova3onerm.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats1d_roi/ex_anova3rm.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats1d_roi/ex_anova3tworm.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats1d_roi/ex_cca_Dorn2012.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats1d_roi/ex_glm.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats1d_roi/ex_hotellings2_Besier2009muscleforces.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats1d_roi/ex_hotellings_paired_Neptune1999.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats1d_roi/ex_hotellings_paired_Pataky2014.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats1d_roi/ex_manova1_Dorn2012.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats1d_roi/ex_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats1d_roi/ex_regression_directional.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats1d_roi/ex_ttest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats1d_roi/ex_ttest2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats1d_roi/ex_ttest_paired.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:30:02.082641 spm1d-0.4.19/spm1d/examples/stats2d/
--rw-r--r--   0 runner    (1001) docker     (123)   307328 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats2d/data2d.npy
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/stats2d/ex2d_ttest2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:30:02.082641 spm1d-0.4.19/spm1d/examples/summarystats/
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/summarystats/ex_plot_errorcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/summarystats/ex_plot_meansd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:30:02.082641 spm1d-0.4.19/spm1d/examples/validation/
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/examples/validation/val_eqvartest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    13176 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:30:02.086641 spm1d-0.4.19/spm1d/rft1d/
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:30:02.042640 spm1d-0.4.19/spm1d/rft1d/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:30:02.086641 spm1d-0.4.19/spm1d/rft1d/data/weather/
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/data/weather/README.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    31982 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/data/weather/daily.m
--rwxr-xr-x   0 runner    (1001) docker     (123)    44170 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/data/weather/daily.mat
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    17791 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/distributions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:30:02.090641 spm1d-0.4.19/spm1d/rft1d/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:30:02.090641 spm1d-0.4.19/spm1d/rft1d/examples/paper/
--rw-r--r--   0 runner    (1001) docker     (123)    39888 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/paper/all_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/paper/fig01_fields1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/paper/fig02_EC_HC.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/paper/fig03_EC.py
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/paper/fig04_fields1d_broken.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/paper/fig05_EC_broken.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/paper/fig06_sf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/paper/fig07_bonf_sf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/paper/fig08_bonf_isf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/paper/fig09_val_maxima.py
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/paper/fig10_upcrossing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/paper/fig11_val_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/paper/fig12_val_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/paper/fig13_weather_0_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/paper/fig14_fwhm_estimation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/paper/fig15_weather_1_rft.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/paper/fig16_weather_2_wrapped.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/paper/fig17_weather_3_nonparam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/random_fields_0.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/random_fields_1.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/random_fields_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/random_fields_broken_0.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/random_fields_broken_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/random_fields_broken_2.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/smoothness_estimation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/smoothness_estimation_broken.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/val_broken_0_gauss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/val_broken_1_t.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/val_broken_2_F.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/val_broken_3_T2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/val_broken_4_X2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/val_conj_0_gauss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/val_conj_1_t.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/val_conj_2_F.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/val_conj_3_T2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/val_conj_4_X2.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/val_max_0_gaussian_0d.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/val_max_0_gaussian_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/val_max_1_onesample_t_0d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/val_max_1_onesample_t_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/val_max_2_twosample_t_0d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/val_max_2_twosample_t_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/val_max_3_regress_0d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/val_max_3_regress_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/val_max_4_anova1_0d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/val_max_4_anova1_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/val_max_5_onesample_T2_0d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/val_max_5_onesample_T2_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/val_max_6_twosample_T2_0d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/val_max_6_twosample_T2_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/val_max_7_cca_0d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/val_max_7_cca_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/val_max_8_manova1_0d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/val_max_8_manova1_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/val_upx_0_gauss_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/val_upx_0_gauss_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/val_upx_1_t_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/val_upx_1_t_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/val_upx_2_F_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/val_upx_2_F_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/val_upx_3_T2_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/val_upx_3_T2_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/val_upx_4_X2_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/val_upx_4_X2_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/weather_0_plotdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/weather_1_rft.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/weather_2_nonparam.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/examples/weather_3_wrapped.py
--rw-r--r--   0 runner    (1001) docker     (123)    23509 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/geom.py
--rw-r--r--   0 runner    (1001) docker     (123)    21886 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/prob.py
--rw-r--r--   0 runner    (1001) docker     (123)     8036 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/rft1d/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:30:02.094641 spm1d-0.4.19/spm1d/stats/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/stats/_clusters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/stats/_datachecks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/stats/_mvbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     7192 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/stats/_reml.py
--rw-r--r--   0 runner    (1001) docker     (123)    21596 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/stats/_spm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/stats/_spmlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:30:02.094641 spm1d-0.4.19/spm1d/stats/anova/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/stats/anova/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25111 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/stats/anova/designs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7763 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/stats/anova/factors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/stats/anova/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    15183 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/stats/anova/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/stats/cca.py
--rw-r--r--   0 runner    (1001) docker     (123)    12671 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/stats/ci.py
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/stats/hotellings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/stats/manova.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:30:02.094641 spm1d-0.4.19/spm1d/stats/nonparam/
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/stats/nonparam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12244 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/stats/nonparam/_snpm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/stats/nonparam/_snpmlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     9867 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/stats/nonparam/calculators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/stats/nonparam/ci.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/stats/nonparam/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    17874 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/stats/nonparam/permuters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/stats/nonparam/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:30:02.094641 spm1d-0.4.19/spm1d/stats/normality/
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/stats/normality/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/stats/normality/k2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/stats/normality/sw.py
--rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/stats/t.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/stats/var.py
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-06-22 05:29:52.000000 spm1d-0.4.19/spm1d/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:30:02.046640 spm1d-0.4.19/spm1d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-22 05:30:01.000000 spm1d-0.4.19/spm1d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18106 2023-06-22 05:30:02.000000 spm1d-0.4.19/spm1d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 05:30:01.000000 spm1d-0.4.19/spm1d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-22 05:30:01.000000 spm1d-0.4.19/spm1d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-22 05:30:01.000000 spm1d-0.4.19/spm1d.egg-info/top_level.txt
+drwxr-xr-x   0 todd       (501) staff       (20)        0 2019-08-22 08:58:12.000000 spm1d-0.4.2/
+-rw-r--r--   0 todd       (501) staff       (20)      691 2019-08-22 08:58:12.000000 spm1d-0.4.2/PKG-INFO
+drwxr-xr-x   0 todd       (501) staff       (20)        0 2019-08-22 08:58:12.000000 spm1d-0.4.2/spm1d/
+-rw-r--r--   0 todd       (501) staff       (20)    12987 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/plot.py
+-rw-r--r--   0 todd       (501) staff       (20)     3262 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/util.py
+-rw-r--r--   0 todd       (501) staff       (20)     1075 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/io.py
+-rw-r--r--   0 todd       (501) staff       (20)      774 2019-08-22 08:37:56.000000 spm1d-0.4.2/spm1d/__init__.py
+drwxr-xr-x   0 todd       (501) staff       (20)        0 2019-08-22 08:58:12.000000 spm1d-0.4.2/spm1d/examples/
+drwxr-xr-x   0 todd       (501) staff       (20)        0 2019-08-22 08:58:12.000000 spm1d-0.4.2/spm1d/examples/summarystats/
+-rw-r--r--   0 todd       (501) staff       (20)      504 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/examples/summarystats/ex_plot_errorcloud.py
+-rw-r--r--   0 todd       (501) staff       (20)      602 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/examples/summarystats/ex_plot_meansd.py
+drwxr-xr-x   0 todd       (501) staff       (20)        0 2019-08-22 08:58:12.000000 spm1d-0.4.2/spm1d/examples/stats1d/
+-rw-r--r--   0 todd       (501) staff       (20)     2777 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats1d/ex_ci_onesample.py
+-rw-r--r--   0 todd       (501) staff       (20)      831 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats1d/ex_anova2rm.py
+-rw-r--r--   0 todd       (501) staff       (20)      884 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats1d/ex_ttest_roi.py
+-rw-r--r--   0 todd       (501) staff       (20)      649 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats1d/ex_hotellings_paired_Pataky2014.py
+-rw-r--r--   0 todd       (501) staff       (20)      385 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats1d/ex_cca_Dorn2012.py
+-rw-r--r--   0 todd       (501) staff       (20)      882 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats1d/ex_anova2nested.py
+-rw-r--r--   0 todd       (501) staff       (20)      554 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats1d/ex_anova3nested.py
+-rw-r--r--   0 todd       (501) staff       (20)      538 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats1d/ex_anova3rm.py
+-rw-r--r--   0 todd       (501) staff       (20)      371 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats1d/ex_anova1_circular_field.py
+-rw-r--r--   0 todd       (501) staff       (20)      713 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats1d/rfx_1_level1.py
+-rw-r--r--   0 todd       (501) staff       (20)      782 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats1d/rfx_2_level2.py
+-rw-r--r--   0 todd       (501) staff       (20)      743 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats1d/ex_anova3tworm.py
+-rw-r--r--   0 todd       (501) staff       (20)     2417 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats1d/ex_ci_twosample.py
+-rw-r--r--   0 todd       (501) staff       (20)      782 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats1d/ex_anova1.py
+-rw-r--r--   0 todd       (501) staff       (20)     2426 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats1d/ex_ci_pairedsample.py
+-rw-r--r--   0 todd       (501) staff       (20)      856 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats1d/ex_ttest_paired.py
+-rw-r--r--   0 todd       (501) staff       (20)      379 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats1d/ex_manova1_Dorn2012.py
+-rw-r--r--   0 todd       (501) staff       (20)      786 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats1d/ex_hotellings_paired_Neptune1999.py
+-rw-r--r--   0 todd       (501) staff       (20)      795 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats1d/ex_anova2.py
+-rw-r--r--   0 todd       (501) staff       (20)      553 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats1d/ex_anova3onerm.py
+-rw-r--r--   0 todd       (501) staff       (20)      873 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats1d/ex_anova2onerm.py
+-rw-r--r--   0 todd       (501) staff       (20)      522 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats1d/ex_anova3.py
+-rw-r--r--   0 todd       (501) staff       (20)      546 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats1d/ex_regression.py
+-rw-r--r--   0 todd       (501) staff       (20)      908 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats1d/ex_glm.py
+-rw-r--r--   0 todd       (501) staff       (20)     1583 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats1d/ex_ci_onesample_standalone.py
+-rw-r--r--   0 todd       (501) staff       (20)      920 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats1d/ex_ttest2.py
+-rw-r--r--   0 todd       (501) staff       (20)      913 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats1d/ex_ttest.py
+-rw-r--r--   0 todd       (501) staff       (20)      869 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats1d/rfx_0_means.py
+-rw-r--r--   0 todd       (501) staff       (20)     1021 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats1d/ex_anova1rm.py
+-rw-r--r--   0 todd       (501) staff       (20)     1296 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats1d/ex_anova1_posthoc.py
+-rw-r--r--   0 todd       (501) staff       (20)      396 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats1d/ex_hotellings2_Besier2009muscleforces.py
+drwxr-xr-x   0 todd       (501) staff       (20)        0 2019-08-22 08:58:12.000000 spm1d-0.4.2/spm1d/examples/stats2d/
+-rw-r--r--   0 todd       (501) staff       (20)     1223 2019-08-22 08:44:49.000000 spm1d-0.4.2/spm1d/examples/stats2d/ex2d_ttest2.py
+drwxr-xr-x   0 todd       (501) staff       (20)        0 2019-08-22 08:58:12.000000 spm1d-0.4.2/spm1d/examples/processing/
+-rw-r--r--   0 todd       (501) staff       (20)      581 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/processing/ex_smooth.py
+-rw-r--r--   0 todd       (501) staff       (20)      780 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/processing/ex_interpolate.py
+drwxr-xr-x   0 todd       (501) staff       (20)        0 2019-08-22 08:58:12.000000 spm1d-0.4.2/spm1d/examples/processing/data/
+-rw-r--r--   0 todd       (501) staff       (20)    29875 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/processing/data/ex_kinematics_for_interpolation.npy
+drwxr-xr-x   0 todd       (501) staff       (20)        0 2019-08-22 08:58:12.000000 spm1d-0.4.2/spm1d/examples/stats1d_roi/
+-rw-r--r--   0 todd       (501) staff       (20)      731 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/examples/stats1d_roi/ex_anova2rm.py
+-rw-r--r--   0 todd       (501) staff       (20)      769 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/examples/stats1d_roi/ex_hotellings_paired_Pataky2014.py
+-rw-r--r--   0 todd       (501) staff       (20)      545 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/examples/stats1d_roi/ex_cca_Dorn2012.py
+-rw-r--r--   0 todd       (501) staff       (20)      662 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/examples/stats1d_roi/ex_anova2nested.py
+-rw-r--r--   0 todd       (501) staff       (20)      755 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/examples/stats1d_roi/ex_anova3nested.py
+-rw-r--r--   0 todd       (501) staff       (20)      868 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/examples/stats1d_roi/ex_anova3rm.py
+-rw-r--r--   0 todd       (501) staff       (20)      661 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/examples/stats1d_roi/ex_regression_directional.py
+-rw-r--r--   0 todd       (501) staff       (20)      877 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/examples/stats1d_roi/ex_anova3tworm.py
+-rw-r--r--   0 todd       (501) staff       (20)      716 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats1d_roi/ex_anova1.py
+-rw-r--r--   0 todd       (501) staff       (20)     1038 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/examples/stats1d_roi/ex_ttest_paired.py
+-rw-r--r--   0 todd       (501) staff       (20)      520 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/examples/stats1d_roi/ex_manova1_Dorn2012.py
+-rw-r--r--   0 todd       (501) staff       (20)      927 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/examples/stats1d_roi/ex_hotellings_paired_Neptune1999.py
+-rw-r--r--   0 todd       (501) staff       (20)      707 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/examples/stats1d_roi/ex_anova2.py
+-rw-r--r--   0 todd       (501) staff       (20)      878 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/examples/stats1d_roi/ex_anova3onerm.py
+-rw-r--r--   0 todd       (501) staff       (20)      741 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/examples/stats1d_roi/ex_anova2onerm.py
+-rw-r--r--   0 todd       (501) staff       (20)      857 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/examples/stats1d_roi/ex_anova3.py
+-rw-r--r--   0 todd       (501) staff       (20)      613 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/examples/stats1d_roi/ex_regression.py
+-rw-r--r--   0 todd       (501) staff       (20)     1008 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/examples/stats1d_roi/ex_glm.py
+-rw-r--r--   0 todd       (501) staff       (20)     1033 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/examples/stats1d_roi/ex_ttest2.py
+-rw-r--r--   0 todd       (501) staff       (20)      923 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/examples/stats1d_roi/ex_ttest.py
+-rw-r--r--   0 todd       (501) staff       (20)     1020 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats1d_roi/ex_anova1rm.py
+-rw-r--r--   0 todd       (501) staff       (20)      525 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/examples/stats1d_roi/ex_hotellings2_Besier2009muscleforces.py
+drwxr-xr-x   0 todd       (501) staff       (20)        0 2019-08-22 08:58:12.000000 spm1d-0.4.2/spm1d/examples/nonparam/
+drwxr-xr-x   0 todd       (501) staff       (20)        0 2019-08-22 08:58:12.000000 spm1d-0.4.2/spm1d/examples/nonparam/0d/
+-rw-r--r--   0 todd       (501) staff       (20)      820 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/0d/ex_ci_onesample.py
+-rw-r--r--   0 todd       (501) staff       (20)     1008 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/0d/ex_anova2rm.py
+-rw-r--r--   0 todd       (501) staff       (20)     1090 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/0d/ex_ttest_standalone.py
+-rw-r--r--   0 todd       (501) staff       (20)      769 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/0d/ex_regress.py
+-rw-r--r--   0 todd       (501) staff       (20)      645 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/0d/ex_anova2nested.py
+-rw-r--r--   0 todd       (501) staff       (20)      599 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/0d/ex_anova3nested.py
+-rw-r--r--   0 todd       (501) staff       (20)      960 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/0d/ex_anova3rm.py
+-rw-r--r--   0 todd       (501) staff       (20)      744 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/0d/ex_hotellings.py
+-rw-r--r--   0 todd       (501) staff       (20)      773 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/0d/ex_hotellings2.py
+-rw-r--r--   0 todd       (501) staff       (20)      713 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/0d/ex_cca.py
+-rw-r--r--   0 todd       (501) staff       (20)     1524 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/0d/ex_ttest2_standalone.py
+-rw-r--r--   0 todd       (501) staff       (20)      676 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/0d/ex_anova3tworm.py
+-rw-r--r--   0 todd       (501) staff       (20)      778 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/0d/ex_ci_twosample.py
+-rw-r--r--   0 todd       (501) staff       (20)      870 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/0d/ex_anova1.py
+-rw-r--r--   0 todd       (501) staff       (20)      768 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/0d/ex_hotellings_paired.py
+-rw-r--r--   0 todd       (501) staff       (20)      861 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/0d/ex_ci_pairedsample.py
+-rw-r--r--   0 todd       (501) staff       (20)      561 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/0d/ex_ttest_paired.py
+-rw-r--r--   0 todd       (501) staff       (20)      989 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/0d/ex_anova2.py
+-rw-r--r--   0 todd       (501) staff       (20)      669 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/0d/ex_anova3onerm.py
+-rw-r--r--   0 todd       (501) staff       (20)     1031 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/0d/ex_anova2onerm.py
+-rw-r--r--   0 todd       (501) staff       (20)      633 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/0d/ex_anova3.py
+-rw-r--r--   0 todd       (501) staff       (20)      774 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/0d/ex_ttest2.py
+-rw-r--r--   0 todd       (501) staff       (20)      548 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/0d/ex_ttest.py
+-rw-r--r--   0 todd       (501) staff       (20)      556 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/0d/ex_manova1.py
+-rw-r--r--   0 todd       (501) staff       (20)      834 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/0d/ex_anova1rm.py
+drwxr-xr-x   0 todd       (501) staff       (20)        0 2019-08-22 08:58:12.000000 spm1d-0.4.2/spm1d/examples/nonparam/1d/
+-rw-r--r--   0 todd       (501) staff       (20)      890 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/1d/ex_ci_onesample.py
+drwxr-xr-x   0 todd       (501) staff       (20)        0 2019-08-22 08:58:12.000000 spm1d-0.4.2/spm1d/examples/nonparam/1d/roi/
+-rw-r--r--   0 todd       (501) staff       (20)     1521 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/1d/roi/ex_anova2rm.py
+-rw-r--r--   0 todd       (501) staff       (20)     1574 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/1d/roi/ex_anova2nested.py
+-rw-r--r--   0 todd       (501) staff       (20)     1228 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/1d/roi/ex_anova3nested.py
+-rw-r--r--   0 todd       (501) staff       (20)     1216 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/1d/roi/ex_anova3rm.py
+-rw-r--r--   0 todd       (501) staff       (20)     1103 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/1d/roi/ex_hotellings.py
+-rw-r--r--   0 todd       (501) staff       (20)      998 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/1d/roi/ex_hotellings2.py
+-rw-r--r--   0 todd       (501) staff       (20)      975 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/1d/roi/ex_cca.py
+-rw-r--r--   0 todd       (501) staff       (20)     1234 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/1d/roi/ex_anova3tworm.py
+-rw-r--r--   0 todd       (501) staff       (20)     1017 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/1d/roi/ex_anova1.py
+-rw-r--r--   0 todd       (501) staff       (20)     1081 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/1d/roi/ex_hotellings_paired.py
+-rw-r--r--   0 todd       (501) staff       (20)     1058 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/1d/roi/ex_ttest_paired.py
+-rw-r--r--   0 todd       (501) staff       (20)     1477 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/1d/roi/ex_anova2.py
+-rw-r--r--   0 todd       (501) staff       (20)     1234 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/1d/roi/ex_anova3onerm.py
+-rw-r--r--   0 todd       (501) staff       (20)     1571 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/1d/roi/ex_anova2onerm.py
+-rw-r--r--   0 todd       (501) staff       (20)     1192 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/1d/roi/ex_anova3.py
+-rw-r--r--   0 todd       (501) staff       (20)     1071 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/1d/roi/ex_regression.py
+-rw-r--r--   0 todd       (501) staff       (20)     1107 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/1d/roi/ex_ttest2.py
+-rw-r--r--   0 todd       (501) staff       (20)     1118 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/1d/roi/ex_ttest.py
+-rw-r--r--   0 todd       (501) staff       (20)     1320 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/1d/roi/ex_manova1.py
+-rw-r--r--   0 todd       (501) staff       (20)      994 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/1d/roi/ex_anova1rm.py
+-rw-r--r--   0 todd       (501) staff       (20)     1252 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/1d/ex_anova2rm.py
+-rw-r--r--   0 todd       (501) staff       (20)     1304 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/1d/ex_anova2nested.py
+-rw-r--r--   0 todd       (501) staff       (20)     1453 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/1d/ex_anova3nested.py
+-rw-r--r--   0 todd       (501) staff       (20)     1099 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/1d/ex_anova3rm.py
+-rw-r--r--   0 todd       (501) staff       (20)      984 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/1d/ex_hotellings.py
+-rw-r--r--   0 todd       (501) staff       (20)      879 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/1d/ex_hotellings2.py
+-rw-r--r--   0 todd       (501) staff       (20)      854 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/1d/ex_cca.py
+-rw-r--r--   0 todd       (501) staff       (20)     1117 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/1d/ex_anova3tworm.py
+-rw-r--r--   0 todd       (501) staff       (20)      869 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/1d/ex_ci_twosample.py
+-rw-r--r--   0 todd       (501) staff       (20)      906 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/1d/ex_anova1.py
+-rw-r--r--   0 todd       (501) staff       (20)      960 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/1d/ex_hotellings_paired.py
+-rw-r--r--   0 todd       (501) staff       (20)      845 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/1d/ex_ci_pairedsample.py
+-rw-r--r--   0 todd       (501) staff       (20)      984 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/1d/ex_ttest_paired.py
+-rw-r--r--   0 todd       (501) staff       (20)     1210 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/1d/ex_anova2.py
+-rw-r--r--   0 todd       (501) staff       (20)     1117 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/1d/ex_anova3onerm.py
+-rw-r--r--   0 todd       (501) staff       (20)     1301 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/1d/ex_anova2onerm.py
+-rw-r--r--   0 todd       (501) staff       (20)      932 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/1d/ex_anova3.py
+-rw-r--r--   0 todd       (501) staff       (20)      999 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/1d/ex_regression.py
+-rw-r--r--   0 todd       (501) staff       (20)     1039 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/1d/ex_ttest2_circular.py
+-rw-r--r--   0 todd       (501) staff       (20)     1174 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/1d/ex_ttest_other_metrics.py
+-rw-r--r--   0 todd       (501) staff       (20)     1032 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/1d/ex_ttest2.py
+-rw-r--r--   0 todd       (501) staff       (20)     1044 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/1d/ex_ttest.py
+-rw-r--r--   0 todd       (501) staff       (20)     1202 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/1d/ex_manova1.py
+-rw-r--r--   0 todd       (501) staff       (20)      877 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/nonparam/1d/ex_anova1rm.py
+drwxr-xr-x   0 todd       (501) staff       (20)        0 2019-08-22 08:58:12.000000 spm1d-0.4.2/spm1d/examples/io/
+-rw-r--r--   0 todd       (501) staff       (20)      421 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/io/ex_import_txt.py
+drwxr-xr-x   0 todd       (501) staff       (20)        0 2019-08-22 08:58:12.000000 spm1d-0.4.2/spm1d/examples/io/data/
+-rw-r--r--   0 todd       (501) staff       (20)    24755 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/io/data/ex_kinematics.txt
+-rw-r--r--   0 todd       (501) staff       (20)    24424 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/io/data/ex_kinematics.mat
+-rw-r--r--   0 todd       (501) staff       (20)      402 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/io/ex_import_mat.py
+drwxr-xr-x   0 todd       (501) staff       (20)        0 2019-08-22 08:58:12.000000 spm1d-0.4.2/spm1d/examples/stats0d/
+-rw-r--r--   0 todd       (501) staff       (20)     1497 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats0d/ex_ci_onesample.py
+-rw-r--r--   0 todd       (501) staff       (20)      685 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats0d/ex_anova2rm.py
+-rw-r--r--   0 todd       (501) staff       (20)      351 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats0d/ex_anova2onermub.py
+-rw-r--r--   0 todd       (501) staff       (20)      465 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats0d/ex_anova2nested.py
+-rw-r--r--   0 todd       (501) staff       (20)      256 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats0d/ex_anova3nested.py
+-rw-r--r--   0 todd       (501) staff       (20)      384 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats0d/ex_anova3rm.py
+-rw-r--r--   0 todd       (501) staff       (20)      324 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats0d/ex_hotellings2.py
+-rw-r--r--   0 todd       (501) staff       (20)      292 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats0d/ex_cca.py
+-rw-r--r--   0 todd       (501) staff       (20)      359 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats0d/ex_anova3tworm.py
+-rw-r--r--   0 todd       (501) staff       (20)     1434 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats0d/ex_ci_twosample.py
+-rw-r--r--   0 todd       (501) staff       (20)      443 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats0d/ex_anova1.py
+-rw-r--r--   0 todd       (501) staff       (20)      350 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats0d/ex_hotellings_paired.py
+-rw-r--r--   0 todd       (501) staff       (20)     1479 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats0d/ex_ci_pairedsample.py
+-rw-r--r--   0 todd       (501) staff       (20)      349 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats0d/ex_ttest_paired.py
+-rw-r--r--   0 todd       (501) staff       (20)      678 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats0d/ex_anova2.py
+-rw-r--r--   0 todd       (501) staff       (20)      364 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats0d/ex_ttest_twosample_unequalvar.py
+-rw-r--r--   0 todd       (501) staff       (20)      342 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats0d/ex_anova3onerm.py
+-rw-r--r--   0 todd       (501) staff       (20)      308 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats0d/ex_hotellings1.py
+-rw-r--r--   0 todd       (501) staff       (20)      693 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats0d/ex_anova2onerm.py
+-rw-r--r--   0 todd       (501) staff       (20)      322 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats0d/ex_anova3.py
+-rw-r--r--   0 todd       (501) staff       (20)      347 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats0d/ex_regression.py
+-rw-r--r--   0 todd       (501) staff       (20)      824 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats0d/ex_ci_onesample_standalone.py
+-rw-r--r--   0 todd       (501) staff       (20)      344 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats0d/ex_ttest_twosample.py
+-rw-r--r--   0 todd       (501) staff       (20)      339 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats0d/ex_ttest_onesample.py
+-rw-r--r--   0 todd       (501) staff       (20)      306 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats0d/ex_manova1.py
+-rw-r--r--   0 todd       (501) staff       (20)      400 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/stats0d/ex_anova1rm.py
+drwxr-xr-x   0 todd       (501) staff       (20)        0 2019-08-22 08:58:12.000000 spm1d-0.4.2/spm1d/examples/scipy/
+-rw-r--r--   0 todd       (501) staff       (20)      693 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/scipy/ex_ttest_normality.py
+-rw-r--r--   0 todd       (501) staff       (20)      548 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/scipy/ex_ttest_paired.py
+-rw-r--r--   0 todd       (501) staff       (20)      578 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/scipy/ex_ttest_twosample_unequalvar.py
+-rw-r--r--   0 todd       (501) staff       (20)      577 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/scipy/ex_regression.py
+-rw-r--r--   0 todd       (501) staff       (20)      560 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/scipy/ex_ttest_twosample.py
+-rw-r--r--   0 todd       (501) staff       (20)      544 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/scipy/ex_ttest_onesample.py
+drwxr-xr-x   0 todd       (501) staff       (20)        0 2019-08-22 08:58:12.000000 spm1d-0.4.2/spm1d/examples/normality/
+drwxr-xr-x   0 todd       (501) staff       (20)        0 2019-08-22 08:58:12.000000 spm1d-0.4.2/spm1d/examples/normality/0d/
+-rw-r--r--   0 todd       (501) staff       (20)      446 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/normality/0d/ex_anova2rm.py
+-rw-r--r--   0 todd       (501) staff       (20)      311 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/normality/0d/ex_regress.py
+-rw-r--r--   0 todd       (501) staff       (20)      348 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/normality/0d/ex_anova2nested.py
+-rw-r--r--   0 todd       (501) staff       (20)      293 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/normality/0d/ex_anova3nested.py
+-rw-r--r--   0 todd       (501) staff       (20)      345 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/normality/0d/ex_anova3rm.py
+-rw-r--r--   0 todd       (501) staff       (20)      367 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/normality/0d/ex_anova3tworm.py
+-rw-r--r--   0 todd       (501) staff       (20)      458 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/normality/0d/ex_anova1.py
+-rw-r--r--   0 todd       (501) staff       (20)      313 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/normality/0d/ex_ttest_paired.py
+-rw-r--r--   0 todd       (501) staff       (20)      455 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/normality/0d/ex_anova2.py
+-rw-r--r--   0 todd       (501) staff       (20)      360 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/normality/0d/ex_anova3onerm.py
+-rw-r--r--   0 todd       (501) staff       (20)      401 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/normality/0d/ex_anova2onerm.py
+-rw-r--r--   0 todd       (501) staff       (20)      335 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/normality/0d/ex_anova3.py
+-rw-r--r--   0 todd       (501) staff       (20)      679 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/normality/0d/ex_ttest2.py
+-rw-r--r--   0 todd       (501) staff       (20)      801 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/normality/0d/ex_ttest.py
+-rw-r--r--   0 todd       (501) staff       (20)      412 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/normality/0d/ex_anova1rm.py
+drwxr-xr-x   0 todd       (501) staff       (20)        0 2019-08-22 08:58:12.000000 spm1d-0.4.2/spm1d/examples/normality/paper/
+-rwxr-xr-x   0 todd       (501) staff       (20)     1787 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/normality/paper/appendix_FigA2.py
+-rwxr-xr-x   0 todd       (501) staff       (20)     1955 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/normality/paper/appendix_FigA6.py
+-rwxr-xr-x   0 todd       (501) staff       (20)     1960 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/normality/paper/appendix_FigA7.py
+-rwxr-xr-x   0 todd       (501) staff       (20)     1996 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/normality/paper/appendix_FigA3.py
+-rwxr-xr-x   0 todd       (501) staff       (20)     1915 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/normality/paper/appendix_FigA4.py
+-rwxr-xr-x   0 todd       (501) staff       (20)     1925 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/normality/paper/appendix_FigA1.py
+-rwxr-xr-x   0 todd       (501) staff       (20)     1654 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/normality/paper/appendix_FigA5.py
+drwxr-xr-x   0 todd       (501) staff       (20)        0 2019-08-22 08:58:12.000000 spm1d-0.4.2/spm1d/examples/normality/1d/
+-rw-r--r--   0 todd       (501) staff       (20)      743 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/normality/1d/ex_anova1.py
+-rw-r--r--   0 todd       (501) staff       (20)      750 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/normality/1d/ex_ttest_paired.py
+-rw-r--r--   0 todd       (501) staff       (20)      749 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/normality/1d/ex_anova2.py
+-rw-r--r--   0 todd       (501) staff       (20)      742 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/normality/1d/ex_regression.py
+-rw-r--r--   0 todd       (501) staff       (20)      779 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/normality/1d/ex_ttest2.py
+-rw-r--r--   0 todd       (501) staff       (20)      739 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/normality/1d/ex_ttest.py
+-rw-r--r--   0 todd       (501) staff       (20)      707 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/examples/normality/1d/ex_anova1rm.py
+-rw-r--r--   0 todd       (501) staff       (20)    10019 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/_plot.py
+drwxr-xr-x   0 todd       (501) staff       (20)        0 2019-08-22 08:58:12.000000 spm1d-0.4.2/spm1d/rft1d/
+-rw-r--r--   0 todd       (501) staff       (20)    21850 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/prob.py
+-rw-r--r--   0 todd       (501) staff       (20)    23473 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/geom.py
+-rw-r--r--   0 todd       (501) staff       (20)      779 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/__init__.py
+-rw-r--r--   0 todd       (501) staff       (20)     8036 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/random.py
+-rw-r--r--   0 todd       (501) staff       (20)    17791 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/distributions.py
+drwxr-xr-x   0 todd       (501) staff       (20)        0 2019-08-22 08:58:12.000000 spm1d-0.4.2/spm1d/rft1d/examples/
+drwxr-xr-x   0 todd       (501) staff       (20)        0 2019-08-22 08:58:12.000000 spm1d-0.4.2/spm1d/rft1d/examples/paper/
+-rw-r--r--   0 todd       (501) staff       (20)     2775 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/paper/fig16_weather_2_wrapped.py
+-rw-r--r--   0 todd       (501) staff       (20)     2030 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/paper/fig11_val_cluster.py
+-rw-r--r--   0 todd       (501) staff       (20)     1697 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/paper/fig14_fwhm_estimation.py
+-rw-r--r--   0 todd       (501) staff       (20)     2208 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/paper/fig08_bonf_isf.py
+-rw-r--r--   0 todd       (501) staff       (20)     4448 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/paper/fig10_upcrossing.py
+-rw-r--r--   0 todd       (501) staff       (20)     2125 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/paper/fig12_val_set.py
+-rw-r--r--   0 todd       (501) staff       (20)     2618 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/paper/fig04_fields1d_broken.py
+-rw-r--r--   0 todd       (501) staff       (20)    39888 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/paper/all_results.py
+-rw-r--r--   0 todd       (501) staff       (20)     2751 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/paper/fig15_weather_1_rft.py
+-rw-r--r--   0 todd       (501) staff       (20)     3951 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/paper/fig02_EC_HC.py
+-rw-r--r--   0 todd       (501) staff       (20)     1901 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/paper/fig06_sf.py
+-rw-r--r--   0 todd       (501) staff       (20)     2997 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/paper/fig17_weather_3_nonparam.py
+-rw-r--r--   0 todd       (501) staff       (20)     3709 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/paper/fig05_EC_broken.py
+-rw-r--r--   0 todd       (501) staff       (20)     2655 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/paper/fig03_EC.py
+-rw-r--r--   0 todd       (501) staff       (20)     2341 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/paper/fig09_val_maxima.py
+-rw-r--r--   0 todd       (501) staff       (20)     2388 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/paper/fig01_fields1d.py
+-rw-r--r--   0 todd       (501) staff       (20)     1627 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/paper/fig13_weather_0_data.py
+-rw-r--r--   0 todd       (501) staff       (20)     1981 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/paper/fig07_bonf_sf.py
+-rw-r--r--   0 todd       (501) staff       (20)     1698 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/val_upx_1_t_set.py
+-rw-r--r--   0 todd       (501) staff       (20)     2452 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/weather_2_nonparam.py
+-rw-r--r--   0 todd       (501) staff       (20)      880 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/smoothness_estimation.py
+-rw-r--r--   0 todd       (501) staff       (20)     1075 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/random_fields_broken_2.py
+-rw-r--r--   0 todd       (501) staff       (20)     2570 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/val_upx_2_F_cluster.py
+-rw-r--r--   0 todd       (501) staff       (20)     1838 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/val_max_3_regress_1d.py
+-rw-r--r--   0 todd       (501) staff       (20)     1265 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/val_max_5_onesample_T2_0d.py
+-rw-r--r--   0 todd       (501) staff       (20)      714 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/val_max_0_gaussian_0d.py
+-rw-r--r--   0 todd       (501) staff       (20)      956 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/val_max_0_gaussian_1d.py
+-rw-r--r--   0 todd       (501) staff       (20)     1663 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/val_max_5_onesample_T2_1d.py
+-rw-r--r--   0 todd       (501) staff       (20)     1728 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/val_max_3_regress_0d.py
+-rw-r--r--   0 todd       (501) staff       (20)     2089 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/val_upx_3_T2_set.py
+-rw-r--r--   0 todd       (501) staff       (20)     1337 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/val_upx_0_gauss_set.py
+-rw-r--r--   0 todd       (501) staff       (20)     2351 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/val_broken_2_F.py
+-rw-r--r--   0 todd       (501) staff       (20)     2865 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/val_upx_4_X2_cluster.py
+-rw-r--r--   0 todd       (501) staff       (20)     1863 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/val_max_4_anova1_0d.py
+-rw-r--r--   0 todd       (501) staff       (20)     1113 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/val_max_1_onesample_t_0d.py
+-rw-r--r--   0 todd       (501) staff       (20)     2122 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/val_upx_3_T2_cluster.py
+-rw-r--r--   0 todd       (501) staff       (20)     1246 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/val_max_1_onesample_t_1d.py
+-rw-r--r--   0 todd       (501) staff       (20)     2121 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/val_max_4_anova1_1d.py
+-rw-r--r--   0 todd       (501) staff       (20)     1748 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/val_upx_1_t_cluster.py
+-rw-r--r--   0 todd       (501) staff       (20)     2617 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/val_conj_4_X2.py
+-rw-r--r--   0 todd       (501) staff       (20)      909 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/random_fields_2.py
+-rw-r--r--   0 todd       (501) staff       (20)     1887 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/val_broken_3_T2.py
+-rw-r--r--   0 todd       (501) staff       (20)     1445 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/val_conj_1_t.py
+-rw-r--r--   0 todd       (501) staff       (20)     1497 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/val_broken_0_gauss.py
+-rw-r--r--   0 todd       (501) staff       (20)      635 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/random_fields_1.py
+-rw-r--r--   0 todd       (501) staff       (20)     2199 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/weather_1_rft.py
+-rw-r--r--   0 todd       (501) staff       (20)     1077 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/smoothness_estimation_broken.py
+-rw-r--r--   0 todd       (501) staff       (20)     1327 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/val_max_2_twosample_t_0d.py
+-rw-r--r--   0 todd       (501) staff       (20)     1413 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/val_max_2_twosample_t_1d.py
+-rw-r--r--   0 todd       (501) staff       (20)     2569 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/weather_3_wrapped.py
+-rw-r--r--   0 todd       (501) staff       (20)     1383 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/val_upx_0_gauss_cluster.py
+-rw-r--r--   0 todd       (501) staff       (20)     1440 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/random_fields_0.py
+-rw-r--r--   0 todd       (501) staff       (20)     1064 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/weather_0_plotdata.py
+-rw-r--r--   0 todd       (501) staff       (20)     2269 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/val_conj_2_F.py
+-rw-r--r--   0 todd       (501) staff       (20)     1937 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/val_max_7_cca_0d.py
+-rw-r--r--   0 todd       (501) staff       (20)     2436 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/val_max_7_cca_1d.py
+-rw-r--r--   0 todd       (501) staff       (20)     2833 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/val_upx_4_X2_set.py
+-rw-r--r--   0 todd       (501) staff       (20)     1728 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/random_fields_broken_0.py
+-rw-r--r--   0 todd       (501) staff       (20)     2070 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/val_max_8_manova1_0d.py
+-rw-r--r--   0 todd       (501) staff       (20)     2552 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/val_max_8_manova1_1d.py
+-rw-r--r--   0 todd       (501) staff       (20)     1807 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/val_conj_3_T2.py
+-rw-r--r--   0 todd       (501) staff       (20)     1512 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/val_max_6_twosample_T2_0d.py
+-rw-r--r--   0 todd       (501) staff       (20)     2524 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/val_upx_2_F_set.py
+-rw-r--r--   0 todd       (501) staff       (20)     2060 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/val_max_6_twosample_T2_1d.py
+-rw-r--r--   0 todd       (501) staff       (20)     1170 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/val_conj_0_gauss.py
+-rw-r--r--   0 todd       (501) staff       (20)     1468 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/val_broken_1_t.py
+-rw-r--r--   0 todd       (501) staff       (20)     2813 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/val_broken_4_X2.py
+-rw-r--r--   0 todd       (501) staff       (20)      873 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/examples/random_fields_broken_1.py
+drwxr-xr-x   0 todd       (501) staff       (20)        0 2019-08-22 08:58:12.000000 spm1d-0.4.2/spm1d/rft1d/data/
+drwxr-xr-x   0 todd       (501) staff       (20)        0 2019-08-22 08:58:12.000000 spm1d-0.4.2/spm1d/rft1d/data/weather/
+-rwxr-xr-x   0 todd       (501) staff       (20)    44170 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/data/weather/daily.mat
+-rwxr-xr-x   0 todd       (501) staff       (20)    31982 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/data/weather/daily.m
+-rw-r--r--   0 todd       (501) staff       (20)      674 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/data/weather/README.txt
+-rw-r--r--   0 todd       (501) staff       (20)     2017 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/rft1d/data.py
+drwxr-xr-x   0 todd       (501) staff       (20)        0 2019-08-22 08:58:12.000000 spm1d-0.4.2/spm1d/data/
+-rw-r--r--   0 todd       (501) staff       (20)     8227 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/_base.py
+drwxr-xr-x   0 todd       (501) staff       (20)        0 2019-08-22 08:58:12.000000 spm1d-0.4.2/spm1d/data/mv0d/
+-rw-r--r--   0 todd       (501) staff       (20)     1541 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/mv0d/manova1.py
+-rw-r--r--   0 todd       (501) staff       (20)    17491 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/mv0d/hotellings2.py
+-rw-r--r--   0 todd       (501) staff       (20)       99 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/mv0d/__init__.py
+-rw-r--r--   0 todd       (501) staff       (20)     1953 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/mv0d/hotellings_paired.py
+-rw-r--r--   0 todd       (501) staff       (20)     1671 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/mv0d/hotellings1.py
+-rw-r--r--   0 todd       (501) staff       (20)     2619 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/mv0d/cca.py
+-rw-r--r--   0 todd       (501) staff       (20)       56 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/__init__.py
+drwxr-xr-x   0 todd       (501) staff       (20)        0 2019-08-22 08:58:12.000000 spm1d-0.4.2/spm1d/data/uv0d/
+-rw-r--r--   0 todd       (501) staff       (20)     8115 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/uv0d/anova2rm.py
+-rw-r--r--   0 todd       (501) staff       (20)     2247 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/uv0d/anova3.py
+-rw-r--r--   0 todd       (501) staff       (20)      865 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/uv0d/t2nonspher.py
+-rw-r--r--   0 todd       (501) staff       (20)     3255 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/uv0d/anova3tworm.py
+-rw-r--r--   0 todd       (501) staff       (20)      680 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/uv0d/ci2.py
+-rw-r--r--   0 todd       (501) staff       (20)      724 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/uv0d/t1.py
+-rw-r--r--   0 todd       (501) staff       (20)     7115 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/uv0d/anova2.py
+-rw-r--r--   0 todd       (501) staff       (20)     4909 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/uv0d/anova3rm.py
+-rw-r--r--   0 todd       (501) staff       (20)     1013 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/uv0d/tpaired.py
+-rw-r--r--   0 todd       (501) staff       (20)      272 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/uv0d/__init__.py
+-rw-r--r--   0 todd       (501) staff       (20)     4812 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/uv0d/normality.py
+-rw-r--r--   0 todd       (501) staff       (20)     1275 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/uv0d/anova2nested.py
+-rw-r--r--   0 todd       (501) staff       (20)      923 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/uv0d/anova3nested.py
+-rw-r--r--   0 todd       (501) staff       (20)      695 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/uv0d/cipaired.py
+-rw-r--r--   0 todd       (501) staff       (20)      867 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/uv0d/t2.py
+-rw-r--r--   0 todd       (501) staff       (20)      950 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/uv0d/ci1.py
+-rw-r--r--   0 todd       (501) staff       (20)    11566 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/uv0d/anova2onerm.py
+-rw-r--r--   0 todd       (501) staff       (20)     2982 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/uv0d/anova1.py
+-rw-r--r--   0 todd       (501) staff       (20)      921 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/uv0d/regress.py
+-rw-r--r--   0 todd       (501) staff       (20)     3091 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/uv0d/anova3onerm.py
+-rw-r--r--   0 todd       (501) staff       (20)     2786 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/uv0d/anova1rm.py
+drwxr-xr-x   0 todd       (501) staff       (20)        0 2019-08-22 08:58:12.000000 spm1d-0.4.2/spm1d/data/mv1d/
+-rw-r--r--   0 todd       (501) staff       (20)     1037 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/mv1d/manova1.py
+-rw-r--r--   0 todd       (501) staff       (20)      984 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/mv1d/hotellings2.py
+-rw-r--r--   0 todd       (501) staff       (20)       87 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/mv1d/__init__.py
+-rw-r--r--   0 todd       (501) staff       (20)     1593 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/mv1d/hotellings_paired.py
+-rw-r--r--   0 todd       (501) staff       (20)     1030 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/mv1d/cca.py
+drwxr-xr-x   0 todd       (501) staff       (20)        0 2019-08-22 08:58:12.000000 spm1d-0.4.2/spm1d/data/uv1d/
+-rw-r--r--   0 todd       (501) staff       (20)     1797 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/uv1d/anova2rm.py
+-rw-r--r--   0 todd       (501) staff       (20)      604 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/uv1d/anova3.py
+-rw-r--r--   0 todd       (501) staff       (20)      662 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/uv1d/anova3tworm.py
+-rw-r--r--   0 todd       (501) staff       (20)     1894 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/uv1d/t1.py
+-rw-r--r--   0 todd       (501) staff       (20)     3378 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/uv1d/anova2.py
+-rw-r--r--   0 todd       (501) staff       (20)      641 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/uv1d/anova3rm.py
+-rw-r--r--   0 todd       (501) staff       (20)      689 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/uv1d/tpaired.py
+-rw-r--r--   0 todd       (501) staff       (20)      229 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/uv1d/__init__.py
+-rw-r--r--   0 todd       (501) staff       (20)      641 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/uv1d/normality.py
+-rw-r--r--   0 todd       (501) staff       (20)     1488 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/uv1d/anova2nested.py
+-rw-r--r--   0 todd       (501) staff       (20)      652 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/uv1d/anova3nested.py
+-rw-r--r--   0 todd       (501) staff       (20)     1022 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/uv1d/t2.py
+-rw-r--r--   0 todd       (501) staff       (20)     1484 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/uv1d/anova2onerm.py
+-rw-r--r--   0 todd       (501) staff       (20)     1592 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/uv1d/anova1.py
+-rw-r--r--   0 todd       (501) staff       (20)     1594 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/uv1d/regress.py
+-rw-r--r--   0 todd       (501) staff       (20)      662 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/uv1d/anova3onerm.py
+-rw-r--r--   0 todd       (501) staff       (20)      748 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/uv1d/anova1rm.py
+drwxr-xr-x   0 todd       (501) staff       (20)        0 2019-08-22 08:58:12.000000 spm1d-0.4.2/spm1d/data/datafiles/
+-rw-r--r--   0 todd       (501) staff       (20)   404080 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/normality_dataset_A6.npy
+-rw-r--r--   0 todd       (501) staff       (20)    48560 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/ex_grf_subj000.npy
+-rw-r--r--   0 todd       (501) staff       (20)     8160 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/normality_dataset_A10.npy
+-rw-r--r--   0 todd       (501) staff       (20)    59848 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova2_3x3.npz
+-rw-r--r--   0 todd       (501) staff       (20)    80880 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/normality_dataset_A11.npy
+-rw-r--r--   0 todd       (501) staff       (20)    48560 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/ex_grf_subj001.npy
+-rw-r--r--   0 todd       (501) staff       (20)    16240 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/normality_dataset_A7.npy
+-rw-r--r--   0 todd       (501) staff       (20)    32400 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/normality_dataset_A5.npy
+-rw-r--r--   0 todd       (501) staff       (20)    48560 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/ex_grf_subj003.npy
+-rw-r--r--   0 todd       (501) staff       (20)   187892 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova2onerm_3x5.npz
+-rw-r--r--   0 todd       (501) staff       (20)   808080 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/normality_dataset_A13.npy
+-rw-r--r--   0 todd       (501) staff       (20)   808080 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/normality_dataset_A12.npy
+-rw-r--r--   0 todd       (501) staff       (20)    24320 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/ex_kinematics.npy
+-rw-r--r--   0 todd       (501) staff       (20)    90548 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova2onerm_3x4.npz
+-rw-r--r--   0 todd       (501) staff       (20)    48560 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/ex_grf_subj002.npy
+-rw-r--r--   0 todd       (501) staff       (20)     8160 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/normality_dataset_A4.npy
+-rw-r--r--   0 todd       (501) staff       (20)    37600 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova2nested_3x3.npz
+-rw-r--r--   0 todd       (501) staff       (20)     8080 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/random.npy
+-rw-r--r--   0 todd       (501) staff       (20)    48560 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/ex_grf_subj006.npy
+-rw-r--r--   0 todd       (501) staff       (20)    29875 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/ex_kinematics_for_interpolation.npy
+-rw-r--r--   0 todd       (501) staff       (20)    12770 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/my_spmTi.npz
+-rw-r--r--   0 todd       (501) staff       (20)    87040 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova2_3x5.npz
+-rw-r--r--   0 todd       (501) staff       (20)   404080 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/normality_dataset_A16.npy
+-rw-r--r--   0 todd       (501) staff       (20)   404080 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/normality_dataset_A17.npy
+-rw-r--r--   0 todd       (501) staff       (20)   119176 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova2_3x4.npz
+-rw-r--r--   0 todd       (501) staff       (20)    48560 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/ex_grf_subj007.npy
+-rw-r--r--   0 todd       (501) staff       (20)     8160 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/simscalar_datasetA.npy
+-rw-r--r--   0 todd       (501) staff       (20)     9776 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/normality_dataset_A1.npy
+-rw-r--r--   0 todd       (501) staff       (20)     9776 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/normality_dataset_A3.npy
+-rw-r--r--   0 todd       (501) staff       (20)    89512 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova2nested_3x4.npz
+-rw-r--r--   0 todd       (501) staff       (20)    48560 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/ex_grf_subj005.npy
+-rw-r--r--   0 todd       (501) staff       (20)     8160 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/simscalar_datasetC.npy
+-rw-r--r--   0 todd       (501) staff       (20)    38132 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova2onerm_3x3.npz
+-rw-r--r--   0 todd       (501) staff       (20)   404080 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/normality_dataset_A15.npy
+-rw-r--r--   0 todd       (501) staff       (20)   808080 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/normality_dataset_A14.npy
+-rw-r--r--   0 todd       (501) staff       (20)    34458 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova3rm_2x2x2.npz
+-rw-r--r--   0 todd       (501) staff       (20)     8160 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/simscalar_datasetB.npy
+-rw-r--r--   0 todd       (501) staff       (20)    48560 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/ex_grf_subj004.npy
+-rw-r--r--   0 todd       (501) staff       (20)   185920 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova2nested_3x5.npz
+-rw-r--r--   0 todd       (501) staff       (20)     9776 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/normality_dataset_A2.npy
+-rw-r--r--   0 todd       (501) staff       (20)     4880 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/ex_grf_speeds.npy
+-rw-r--r--   0 todd       (501) staff       (20)    66440 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova2nested_4x4.npz
+-rw-r--r--   0 todd       (501) staff       (20)    17000 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova2nested_2x2.npz
+-rw-r--r--   0 todd       (501) staff       (20)   282313 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/Besier2009muscleforces.npz
+-rw-r--r--   0 todd       (501) staff       (20)   133806 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova3nested_2x4x2.npz
+-rw-r--r--   0 todd       (501) staff       (20)    49960 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova2nested_2x3.npz
+-rw-r--r--   0 todd       (501) staff       (20)   115880 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova2nested_4x5.npz
+-rw-r--r--   0 todd       (501) staff       (20)   101658 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova3rm_2x3x4.npz
+-rw-r--r--   0 todd       (501) staff       (20)    49960 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova2_2x3.npz
+-rw-r--r--   0 todd       (501) staff       (20)   198280 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova2_4x5.npz
+-rw-r--r--   0 todd       (501) staff       (20)   105992 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova2_4x4.npz
+-rw-r--r--   0 todd       (501) staff       (20)    30624 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/Pataky2014cop.npz
+-rw-r--r--   0 todd       (501) staff       (20)    17000 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova2_2x2.npz
+-rw-r--r--   0 todd       (501) staff       (20)    45620 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova2onerm_2x3.npz
+-rw-r--r--   0 todd       (501) staff       (20)   117172 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova2onerm_4x5.npz
+-rw-r--r--   0 todd       (501) staff       (20)    37636 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/Neptune1999kneekin.npz
+-rw-r--r--   0 todd       (501) staff       (20)    67252 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova2onerm_4x4.npz
+-rw-r--r--   0 todd       (501) staff       (20)    53934 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova3nested_2x2x2.npz
+-rw-r--r--   0 todd       (501) staff       (20)    17332 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova2onerm_2x2.npz
+-rw-r--r--   0 todd       (501) staff       (20)    29533 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/Besier2009kneeflexion.npz
+-rw-r--r--   0 todd       (501) staff       (20)    23431 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/ex_grf_means.npz
+-rw-r--r--   0 todd       (501) staff       (20)    98728 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/weather.npz
+-rw-r--r--   0 todd       (501) staff       (20)    90548 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova2rm_3x4.npz
+-rw-r--r--   0 todd       (501) staff       (20)    44022 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/Dorn2012.npz
+-rw-r--r--   0 todd       (501) staff       (20)      680 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/ex_grf_speeds_cond.npy
+-rw-r--r--   0 todd       (501) staff       (20)    33966 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova3_2x2x2.npz
+-rw-r--r--   0 todd       (501) staff       (20)    34458 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova3tworm_2x2x2.npz
+-rw-r--r--   0 todd       (501) staff       (20)    88052 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova2rm_3x5.npz
+-rw-r--r--   0 todd       (501) staff       (20)    34458 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova3onerm_2x2x2.npz
+-rw-r--r--   0 todd       (501) staff       (20)     9776 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/ex_sim_twolocalmax.npy
+-rw-r--r--   0 todd       (501) staff       (20)    38132 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova2rm_3x3.npz
+-rw-r--r--   0 todd       (501) staff       (20)     4928 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/random_rough.npy
+-rw-r--r--   0 todd       (501) staff       (20)    48560 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/ex_grf_subj009.npy
+-rw-r--r--   0 todd       (501) staff       (20)    48560 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/ex_grf_subj008.npy
+-rw-r--r--   0 todd       (501) staff       (20)    11291 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/my_spmT.npz
+-rw-r--r--   0 todd       (501) staff       (20)   101658 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova3onerm_2x3x4.npz
+-rw-r--r--   0 todd       (501) staff       (20)    67252 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova2rm_4x4.npz
+-rw-r--r--   0 todd       (501) staff       (20)    16240 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/normality_dataset_A9.npy
+-rw-r--r--   0 todd       (501) staff       (20)   100526 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova3_2x3x4.npz
+-rw-r--r--   0 todd       (501) staff       (20)    23988 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova2rm_2x2.npz
+-rw-r--r--   0 todd       (501) staff       (20)    60596 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova2rm_2x3.npz
+-rw-r--r--   0 todd       (501) staff       (20)   101658 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova3tworm_2x3x4.npz
+-rw-r--r--   0 todd       (501) staff       (20)    16240 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/normality_dataset_A8.npy
+-rw-r--r--   0 todd       (501) staff       (20)   133812 2019-08-22 08:37:03.000000 spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova2rm_4x5.npz
+drwxr-xr-x   0 todd       (501) staff       (20)        0 2019-08-22 08:58:12.000000 spm1d-0.4.2/spm1d/stats/
+-rw-r--r--   0 todd       (501) staff       (20)     2612 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/stats/_spmlist.py
+-rw-r--r--   0 todd       (501) staff       (20)     3642 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/stats/manova.py
+-rw-r--r--   0 todd       (501) staff       (20)    21139 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/stats/_spm.py
+-rw-r--r--   0 todd       (501) staff       (20)    12671 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/stats/ci.py
+-rw-r--r--   0 todd       (501) staff       (20)     5415 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/stats/_datachecks.py
+drwxr-xr-x   0 todd       (501) staff       (20)        0 2019-08-22 08:58:12.000000 spm1d-0.4.2/spm1d/stats/nonparam/
+-rw-r--r--   0 todd       (501) staff       (20)     2058 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/stats/nonparam/metrics.py
+-rw-r--r--   0 todd       (501) staff       (20)     4974 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/stats/nonparam/_snpmlist.py
+-rw-r--r--   0 todd       (501) staff       (20)     3633 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/stats/nonparam/ci.py
+-rw-r--r--   0 todd       (501) staff       (20)      543 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/stats/nonparam/__init__.py
+-rw-r--r--   0 todd       (501) staff       (20)     5069 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/stats/nonparam/stats.py
+-rw-r--r--   0 todd       (501) staff       (20)    12244 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/stats/nonparam/_snpm.py
+-rw-r--r--   0 todd       (501) staff       (20)     9885 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/stats/nonparam/calculators.py
+-rw-r--r--   0 todd       (501) staff       (20)    17874 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/stats/nonparam/permuters.py
+-rw-r--r--   0 todd       (501) staff       (20)     1048 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/stats/__init__.py
+-rw-r--r--   0 todd       (501) staff       (20)     2097 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/stats/_mvbase.py
+-rw-r--r--   0 todd       (501) staff       (20)     6242 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/stats/_clusters.py
+-rw-r--r--   0 todd       (501) staff       (20)     7192 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/stats/_reml.py
+-rw-r--r--   0 todd       (501) staff       (20)     3661 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/stats/hotellings.py
+drwxr-xr-x   0 todd       (501) staff       (20)        0 2019-08-22 08:58:12.000000 spm1d-0.4.2/spm1d/stats/anova/
+-rw-r--r--   0 todd       (501) staff       (20)     3338 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/stats/anova/models.py
+-rw-r--r--   0 todd       (501) staff       (20)     7763 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/stats/anova/factors.py
+-rw-r--r--   0 todd       (501) staff       (20)    15183 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/stats/anova/ui.py
+-rw-r--r--   0 todd       (501) staff       (20)    25111 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/stats/anova/designs.py
+-rw-r--r--   0 todd       (501) staff       (20)      238 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/stats/anova/__init__.py
+-rw-r--r--   0 todd       (501) staff       (20)     4036 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/stats/cca.py
+-rw-r--r--   0 todd       (501) staff       (20)     5992 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/stats/t.py
+drwxr-xr-x   0 todd       (501) staff       (20)        0 2019-08-22 08:58:12.000000 spm1d-0.4.2/spm1d/stats/normality/
+-rw-r--r--   0 todd       (501) staff       (20)     6814 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/stats/normality/k2.py
+-rw-r--r--   0 todd       (501) staff       (20)      183 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/stats/normality/__init__.py
+-rw-r--r--   0 todd       (501) staff       (20)     2649 2019-08-22 08:37:04.000000 spm1d-0.4.2/spm1d/stats/normality/sw.py
+-rw-r--r--   0 todd       (501) staff       (20)      114 2019-08-22 08:37:03.000000 spm1d-0.4.2/MANIFEST.in
+-rw-r--r--   0 todd       (501) staff       (20)     1530 2019-08-22 08:50:16.000000 spm1d-0.4.2/README.md
+-rw-r--r--   0 todd       (501) staff       (20)      995 2019-08-22 08:49:20.000000 spm1d-0.4.2/setup.py
+-rw-r--r--   0 todd       (501) staff       (20)       79 2019-08-22 08:58:12.000000 spm1d-0.4.2/setup.cfg
+-rw-r--r--   0 todd       (501) staff       (20)    35121 2019-08-22 08:37:03.000000 spm1d-0.4.2/LICENSE.txt
+drwxr-xr-x   0 todd       (501) staff       (20)        0 2019-08-22 08:58:12.000000 spm1d-0.4.2/spm1d.egg-info/
+-rw-r--r--   0 todd       (501) staff       (20)      691 2019-08-22 08:58:12.000000 spm1d-0.4.2/spm1d.egg-info/PKG-INFO
+-rw-r--r--   0 todd       (501) staff       (20)    17971 2019-08-22 08:58:12.000000 spm1d-0.4.2/spm1d.egg-info/SOURCES.txt
+-rw-r--r--   0 todd       (501) staff       (20)       23 2019-08-22 08:58:12.000000 spm1d-0.4.2/spm1d.egg-info/requires.txt
+-rw-r--r--   0 todd       (501) staff       (20)        6 2019-08-22 08:58:12.000000 spm1d-0.4.2/spm1d.egg-info/top_level.txt
+-rw-r--r--   0 todd       (501) staff       (20)        1 2019-08-22 08:58:12.000000 spm1d-0.4.2/spm1d.egg-info/dependency_links.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `spm1d-0.4.19/LICENSE.txt` & `spm1d-0.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/README.md` & `spm1d-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/setup.py` & `spm1d-0.4.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 spm1d uses <b>Random Field Theory</b> expectations regarding the behavior of smooth,
 one-dimensional Gaussian fields to make statistical inferences regarding a set of
 one-dimensional measurements.
 '''
 
 setup(
 	name             = 'spm1d',
-	version          = '0.4.19',
+	version          = '0.4.2',
 	description      = 'One-Dimensional Statistical Parametric Mapping',
 	author           = 'Todd Pataky',
 	author_email     = 'spm1d.mail@gmail.com',
 	url              = 'https://github.com/0todd0000/spm1d',
 	download_url     = 'https://github.com/0todd0000/spm1d/archive/master.zip',
 	packages         = ['spm1d'],
 	package_data     = {'spm1d' : ['examples/*.*', 'data/*.*'] },
```

### Comparing `spm1d-0.4.19/spm1d/__init__.py` & `spm1d-0.4.2/spm1d/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,19 +12,20 @@
 [2] Wellcome Trust Centre for Neuroimaging SPM homepage:
 www.fil.ion.ucl.ac.uk/spm/
 
 [3] Pataky TC (2016). RFT1D: Smooth one-dimensional random field upcrossing
 probabilities in Python, Journal of Statistical Software, in press.
 
 
-Copyright (C) 2023  Todd Pataky
+Copyright (C) 2019  Todd Pataky
+Version: 0.4.2 (2019/08/22)
 '''
 
 
-__version__ = '0.4.19 (2023-06-22)'
+__version__ = '0.4.2 (2019/08/22)'
 
 
 __all__ = ['data', 'io', 'plot', 'rft1d', 'stats', 'util']
 
 from . import data
 from . import io
 from . import plot
```

### Comparing `spm1d-0.4.19/spm1d/_plot.py` & `spm1d-0.4.2/spm1d/_plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,19 +69,15 @@
 			y0,y1   = ax.transData.inverted().transform(bbox)[:,1]
 			ymin    = min(y0, ymin)
 			ymax    = max(y1, ymax)
 		dy = 0.075*(ymax-ymin)
 		ax.set_ylim(ymin-dy, ymax+dy)
 	
 	def plot(self, *args, **kwdargs):
-		if self.x is None:
-			h = self.ax.plot(*args, **kwdargs)
-		else:
-			h = self.ax.plot(self.x, *args, **kwdargs)
-		return h
+		return self.ax.plot(*args, **kwdargs)
 
 	# def plot(self, y, **kwdargs):
 	# 	return self.ax.plot(y, **kwdargs)
 	
 	def plot_cloud(self, Y, facecolor='0.8', edgecolor='0.8', alpha=0.5, edgelinestyle='-'):
 		### create patches:
 		y0,y1       = Y
@@ -167,18 +163,14 @@
 	
 	def plot_field(self, **kwdargs):
 		keys   = kwdargs.keys()
 		if 'color' not in keys:
 			kwdargs.update( dict(color='k') )
 		if ('lw' not in keys) and ('linewidth' not in keys):
 			kwdargs.update( dict(lw=2) )
-		if ('ls' not in keys) and ('linestyle' not in keys):
-			kwdargs.update( dict(ls='-') )
-		if 'marker' not in keys:
-			kwdargs.update( dict(marker=' ') )
 		ax,x    = self.ax, self.x
 		if self.ismasked:
 			ax.plot(x, self.zma, **kwdargs)
 		else:
 			ax.plot(x, self.z, **kwdargs)
 	
 	def plot_ylabel(self):
@@ -199,16 +191,16 @@
 
 
 
 class SPMiPlotter(SPMPlotter):
 	def __init__(self, spmi, ax=None):
 		super(SPMiPlotter, self).__init__(spmi, ax)
 	
-	def plot(self, color='k', lw=3, linestyle='-', marker=' ', facecolor='0.7', thresh_color='k', label=None):
-		self.plot_field(color=color, lw=lw, linestyle=linestyle, marker=marker, label=label)
+	def plot(self, color='k', lw=3, facecolor='0.7', thresh_color='k', label=None):
+		self.plot_field(color=color, lw=lw, label=label)
 		self.plot_datum()
 		self.plot_threshold(color=thresh_color)
 		self.plot_cluster_patches(facecolor=facecolor)
 		self._set_ylim()
 
 	def plot_cluster_patches(self, facecolor='0.8'):
 		if self.spm.nClusters > 0:
```

### Comparing `spm1d-0.4.19/spm1d/data/_base.py` & `spm1d-0.4.2/spm1d/data/_base.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/Besier2009kneeflexion.npz` & `spm1d-0.4.2/spm1d/data/datafiles/Besier2009kneeflexion.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/Besier2009muscleforces.npz` & `spm1d-0.4.2/spm1d/data/datafiles/Besier2009muscleforces.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/Dorn2012.npz` & `spm1d-0.4.2/spm1d/data/datafiles/Dorn2012.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/Neptune1999kneekin.npz` & `spm1d-0.4.2/spm1d/data/datafiles/Neptune1999kneekin.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/Pataky2014cop.npz` & `spm1d-0.4.2/spm1d/data/datafiles/Pataky2014cop.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/ex_grf_means.npz` & `spm1d-0.4.2/spm1d/data/datafiles/ex_grf_means.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/ex_grf_speeds.npy` & `spm1d-0.4.2/spm1d/data/datafiles/ex_grf_speeds.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/ex_grf_speeds_cond.npy` & `spm1d-0.4.2/spm1d/data/datafiles/ex_grf_speeds_cond.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/ex_grf_subj000.npy` & `spm1d-0.4.2/spm1d/data/datafiles/ex_grf_subj000.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/ex_grf_subj001.npy` & `spm1d-0.4.2/spm1d/data/datafiles/ex_grf_subj001.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/ex_grf_subj002.npy` & `spm1d-0.4.2/spm1d/data/datafiles/ex_grf_subj002.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/ex_grf_subj003.npy` & `spm1d-0.4.2/spm1d/data/datafiles/ex_grf_subj003.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/ex_grf_subj004.npy` & `spm1d-0.4.2/spm1d/data/datafiles/ex_grf_subj004.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/ex_grf_subj005.npy` & `spm1d-0.4.2/spm1d/data/datafiles/ex_grf_subj005.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/ex_grf_subj006.npy` & `spm1d-0.4.2/spm1d/data/datafiles/ex_grf_subj006.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/ex_grf_subj007.npy` & `spm1d-0.4.2/spm1d/data/datafiles/ex_grf_subj007.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/ex_grf_subj008.npy` & `spm1d-0.4.2/spm1d/data/datafiles/ex_grf_subj008.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/ex_grf_subj009.npy` & `spm1d-0.4.2/spm1d/data/datafiles/ex_grf_subj009.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/ex_kinematics.npy` & `spm1d-0.4.2/spm1d/data/datafiles/ex_kinematics.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/ex_kinematics_for_interpolation.npy` & `spm1d-0.4.2/spm1d/data/datafiles/ex_kinematics_for_interpolation.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/ex_sim_twolocalmax.npy` & `spm1d-0.4.2/spm1d/data/datafiles/ex_sim_twolocalmax.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/my_spmT.npz` & `spm1d-0.4.2/spm1d/data/datafiles/my_spmT.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/my_spmTi.npz` & `spm1d-0.4.2/spm1d/data/datafiles/my_spmTi.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/normality_dataset_A1.npy` & `spm1d-0.4.2/spm1d/data/datafiles/normality_dataset_A1.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/normality_dataset_A10.npy` & `spm1d-0.4.2/spm1d/data/datafiles/normality_dataset_A10.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/normality_dataset_A11.npy` & `spm1d-0.4.2/spm1d/data/datafiles/normality_dataset_A11.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/normality_dataset_A12.npy` & `spm1d-0.4.2/spm1d/data/datafiles/normality_dataset_A12.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/normality_dataset_A13.npy` & `spm1d-0.4.2/spm1d/data/datafiles/normality_dataset_A13.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/normality_dataset_A14.npy` & `spm1d-0.4.2/spm1d/data/datafiles/normality_dataset_A14.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/normality_dataset_A15.npy` & `spm1d-0.4.2/spm1d/data/datafiles/normality_dataset_A15.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/normality_dataset_A16.npy` & `spm1d-0.4.2/spm1d/data/datafiles/normality_dataset_A16.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/normality_dataset_A17.npy` & `spm1d-0.4.2/spm1d/data/datafiles/normality_dataset_A17.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/normality_dataset_A2.npy` & `spm1d-0.4.2/spm1d/data/datafiles/normality_dataset_A2.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/normality_dataset_A3.npy` & `spm1d-0.4.2/spm1d/data/datafiles/normality_dataset_A3.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/normality_dataset_A4.npy` & `spm1d-0.4.2/spm1d/data/datafiles/normality_dataset_A4.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/normality_dataset_A5.npy` & `spm1d-0.4.2/spm1d/data/datafiles/normality_dataset_A5.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/normality_dataset_A6.npy` & `spm1d-0.4.2/spm1d/data/datafiles/normality_dataset_A6.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/normality_dataset_A7.npy` & `spm1d-0.4.2/spm1d/data/datafiles/normality_dataset_A7.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/normality_dataset_A8.npy` & `spm1d-0.4.2/spm1d/data/datafiles/normality_dataset_A8.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/normality_dataset_A9.npy` & `spm1d-0.4.2/spm1d/data/datafiles/normality_dataset_A9.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/random.npy` & `spm1d-0.4.2/spm1d/data/datafiles/random.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/random_rough.npy` & `spm1d-0.4.2/spm1d/data/datafiles/random_rough.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/simscalar_datasetA.npy` & `spm1d-0.4.2/spm1d/data/datafiles/simscalar_datasetA.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/simscalar_datasetB.npy` & `spm1d-0.4.2/spm1d/data/datafiles/simscalar_datasetB.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/simscalar_datasetC.npy` & `spm1d-0.4.2/spm1d/data/datafiles/simscalar_datasetC.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova2_2x2.npz` & `spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova2_2x2.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova2_2x3.npz` & `spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova2_2x3.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova2_3x3.npz` & `spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova2_3x3.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova2_3x4.npz` & `spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova2_3x4.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova2_3x5.npz` & `spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova2_3x5.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova2_4x4.npz` & `spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova2_4x4.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova2_4x5.npz` & `spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova2_4x5.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova2nested_2x2.npz` & `spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova2nested_2x2.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova2nested_2x3.npz` & `spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova2nested_2x3.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova2nested_3x3.npz` & `spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova2nested_3x3.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova2nested_3x4.npz` & `spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova2nested_3x4.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova2nested_3x5.npz` & `spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova2nested_3x5.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova2nested_4x4.npz` & `spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova2nested_4x4.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova2nested_4x5.npz` & `spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova2nested_4x5.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova2onerm_2x2.npz` & `spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova2onerm_2x2.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova2onerm_2x3.npz` & `spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova2onerm_2x3.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova2onerm_3x3.npz` & `spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova2onerm_3x3.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova2onerm_3x4.npz` & `spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova2onerm_3x4.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova2onerm_3x5.npz` & `spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova2onerm_3x5.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova2onerm_4x4.npz` & `spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova2onerm_4x4.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova2onerm_4x5.npz` & `spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova2onerm_4x5.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova2rm_2x2.npz` & `spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova2rm_2x2.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova2rm_2x3.npz` & `spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova2rm_2x3.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova2rm_3x3.npz` & `spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova2rm_3x3.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova2rm_3x4.npz` & `spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova2rm_3x4.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova2rm_3x5.npz` & `spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova2rm_3x5.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova2rm_4x4.npz` & `spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova2rm_4x4.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova2rm_4x5.npz` & `spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova2rm_4x5.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova3_2x2x2.npz` & `spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova3_2x2x2.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova3_2x3x4.npz` & `spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova3_2x3x4.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova3nested_2x2x2.npz` & `spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova3nested_2x2x2.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova3nested_2x4x2.npz` & `spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova3nested_2x4x2.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova3onerm_2x2x2.npz` & `spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova3onerm_2x2x2.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova3onerm_2x3x4.npz` & `spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova3onerm_2x3x4.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova3rm_2x2x2.npz` & `spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova3rm_2x2x2.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova3rm_2x3x4.npz` & `spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova3rm_2x3x4.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova3tworm_2x2x2.npz` & `spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova3tworm_2x2x2.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/spm1d_anova3tworm_2x3x4.npz` & `spm1d-0.4.2/spm1d/data/datafiles/spm1d_anova3tworm_2x3x4.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/datafiles/weather.npz` & `spm1d-0.4.2/spm1d/data/datafiles/weather.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/mv0d/cca.py` & `spm1d-0.4.2/spm1d/data/mv0d/cca.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/mv0d/hotellings1.py` & `spm1d-0.4.2/spm1d/data/mv0d/hotellings1.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/mv0d/hotellings2.py` & `spm1d-0.4.2/spm1d/data/mv0d/hotellings2.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/mv0d/hotellings_paired.py` & `spm1d-0.4.2/spm1d/data/mv0d/hotellings_paired.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/mv0d/manova1.py` & `spm1d-0.4.2/spm1d/data/mv0d/manova1.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/mv1d/cca.py` & `spm1d-0.4.2/spm1d/data/mv1d/cca.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/mv1d/hotellings2.py` & `spm1d-0.4.2/spm1d/data/mv1d/hotellings2.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/mv1d/hotellings_paired.py` & `spm1d-0.4.2/spm1d/data/mv1d/hotellings_paired.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/mv1d/manova1.py` & `spm1d-0.4.2/spm1d/data/mv1d/manova1.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/uv0d/anova1.py` & `spm1d-0.4.2/spm1d/data/uv0d/anova1.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/uv0d/anova1rm.py` & `spm1d-0.4.2/spm1d/data/uv0d/anova1rm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/uv0d/anova2.py` & `spm1d-0.4.2/spm1d/data/uv0d/anova2.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/uv0d/anova2nested.py` & `spm1d-0.4.2/spm1d/data/uv0d/anova2nested.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/uv0d/anova2onerm.py` & `spm1d-0.4.2/spm1d/data/uv0d/anova2onerm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/uv0d/anova2rm.py` & `spm1d-0.4.2/spm1d/data/uv0d/anova2rm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/uv0d/anova3.py` & `spm1d-0.4.2/spm1d/data/uv0d/anova3.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/uv0d/anova3nested.py` & `spm1d-0.4.2/spm1d/data/uv0d/anova3nested.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/uv0d/anova3onerm.py` & `spm1d-0.4.2/spm1d/data/uv0d/anova3onerm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/uv0d/anova3rm.py` & `spm1d-0.4.2/spm1d/data/uv0d/anova3rm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/uv0d/anova3tworm.py` & `spm1d-0.4.2/spm1d/data/uv0d/anova3tworm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/uv0d/ci1.py` & `spm1d-0.4.2/spm1d/data/uv0d/ci1.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/uv0d/ci2.py` & `spm1d-0.4.2/spm1d/data/uv0d/ci2.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/uv0d/cipaired.py` & `spm1d-0.4.2/spm1d/data/uv0d/cipaired.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/uv0d/normality.py` & `spm1d-0.4.2/spm1d/data/uv0d/normality.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/uv0d/regress.py` & `spm1d-0.4.2/spm1d/data/uv0d/regress.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/uv0d/t1.py` & `spm1d-0.4.2/spm1d/data/uv0d/t1.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/uv0d/t2.py` & `spm1d-0.4.2/spm1d/data/uv0d/t2.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/uv0d/t2nonspher.py` & `spm1d-0.4.2/spm1d/data/uv0d/t2nonspher.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/uv0d/tpaired.py` & `spm1d-0.4.2/spm1d/data/uv0d/tpaired.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/uv1d/anova1.py` & `spm1d-0.4.2/spm1d/data/uv1d/anova1.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/uv1d/anova1rm.py` & `spm1d-0.4.2/spm1d/data/uv1d/anova1rm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/uv1d/anova2.py` & `spm1d-0.4.2/spm1d/data/uv1d/anova2.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/uv1d/anova2nested.py` & `spm1d-0.4.2/spm1d/data/uv1d/anova2nested.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/uv1d/anova2onerm.py` & `spm1d-0.4.2/spm1d/data/uv1d/anova2onerm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/uv1d/anova2rm.py` & `spm1d-0.4.2/spm1d/data/uv1d/anova2rm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/uv1d/anova3.py` & `spm1d-0.4.2/spm1d/data/uv1d/anova3.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/uv1d/anova3nested.py` & `spm1d-0.4.2/spm1d/data/uv1d/anova3nested.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/uv1d/anova3onerm.py` & `spm1d-0.4.2/spm1d/data/uv1d/anova3onerm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/uv1d/anova3rm.py` & `spm1d-0.4.2/spm1d/data/uv1d/anova3rm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/uv1d/anova3tworm.py` & `spm1d-0.4.2/spm1d/data/uv1d/anova3tworm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/uv1d/normality.py` & `spm1d-0.4.2/spm1d/data/uv1d/normality.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/uv1d/regress.py` & `spm1d-0.4.2/spm1d/data/uv1d/regress.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/uv1d/t1.py` & `spm1d-0.4.2/spm1d/data/uv1d/t1.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/uv1d/t2.py` & `spm1d-0.4.2/spm1d/data/uv1d/t2.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/data/uv1d/tpaired.py` & `spm1d-0.4.2/spm1d/data/uv1d/tpaired.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/examples/io/data/ex_kinematics.mat` & `spm1d-0.4.2/spm1d/examples/io/data/ex_kinematics.mat`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/examples/io/data/ex_kinematics.txt` & `spm1d-0.4.2/spm1d/examples/io/data/ex_kinematics.txt`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/0d/ex_anova1.py` & `spm1d-0.4.2/spm1d/examples/nonparam/0d/ex_anova1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 
 import numpy as np
 import spm1d
 
 
 
 #(0) Load dataset:
-# dataset = spm1d.data.uv0d.anova1.Cars()
-# dataset = spm1d.data.uv0d.anova1.Sound()
+dataset = spm1d.data.uv0d.anova1.Cars()
+dataset = spm1d.data.uv0d.anova1.Sound()
 # dataset = spm1d.data.uv0d.anova1.Southampton1()
 # dataset = spm1d.data.uv0d.anova1.ConstructionUnequalSampleSizes()
-dataset = spm1d.data.uv0d.anova1.RSUnequalSampleSizes()
+# dataset = spm1d.data.uv0d.anova1.RSUnequalSampleSizes()
 y,A     = dataset.get_data()
 print( dataset )
 
 
 
 
 #(1) Conduct non-parametric test:
```

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/0d/ex_anova1rm.py` & `spm1d-0.4.2/spm1d/examples/nonparam/0d/ex_anova3rm.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 
 import numpy as np
 import spm1d
 
 
 
 #(0) Load dataset:
-dataset  = spm1d.data.uv0d.anova1rm.Abdi2010()
-# dataset  = spm1d.data.uv0d.anova1rm.Groceries()
-# dataset  = spm1d.data.uv0d.anova1rm.Imacelebrity()
-# dataset  = spm1d.data.uv0d.anova1rm.Southampton1rm()
-y,A,SUBJ = dataset.get_data()
+dataset      = spm1d.data.uv0d.anova3rm.SPM1D2x2x2()
+# dataset      = spm1d.data.uv0d.anova3rm.SPM1D2x3x5()
+# dataset      = spm1d.data.uv0d.anova3rm.SPM1D3x3x3()
+y,A,B,C,SUBJ = dataset.get_data()
 print( dataset )
 
 
 
 
 #(1) Conduct non-parametric test:
 np.random.seed(0)
 alpha      = 0.05
-F          = spm1d.stats.nonparam.anova1rm(y, A, SUBJ)
-Fi         = F.inference(alpha, iterations=1000)
-print(Fi)
+snpmlist   = spm1d.stats.nonparam.anova3rm(y, A, B, C, SUBJ)
+snpmilist  = snpmlist.inference(alpha, iterations=100)
+F,p        = np.array(   [(s.z, s.p)  for s in snpmilist]   ).T
 
 
-#(2) Compare to parametric test:
-Fparam     = spm1d.stats.anova1rm(y, A, SUBJ, equal_var=True)
-Fparami    = Fparam.inference(alpha)
 
+#(1) Conduct non-parametric test:
+np.random.seed(0)
+alpha      = 0.05
+snpmlist   = spm1d.stats.nonparam.anova3rm(y, A, B, C, SUBJ)
+snpmilist  = snpmlist.inference(alpha, iterations=200)
+print( 'Non-parametric results:')
+print( snpmilist )
 
 
-#(3) Print results:
-print
-print( 'Non-parametric results:' )
-print( '   t=%.3f, p=%.5f' %(Fi.z, Fi.p) )
-print
-print( 'Parametric results:' )
-print( '   t=%.3f, p=%.5f' %(Fparami.z, Fparami.p) )
-print
 
+#(2) Compare to parametric test:
+spmlist    = spm1d.stats.anova3rm(y, A, B, C, SUBJ, equal_var=True)
+spmilist   = spmlist.inference(alpha)
+print( 'Parametric results:')
+print( spmilist )
```

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/0d/ex_anova2.py` & `spm1d-0.4.2/spm1d/examples/nonparam/0d/ex_anova2.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 
 
 #(1) Conduct non-parametric test:
 np.random.seed(0)
 alpha      = 0.05
 snpmlist   = spm1d.stats.nonparam.anova2(y, A, B)
-snpmilist  = snpmlist.inference(alpha, iterations=1000)
+snpmilist  = snpmlist.inference(alpha, iterations=200)
 print( 'Non-parametric results:')
 print( snpmilist )
 
 
 #(2) Compare to parametric test:
 spmlist    = spm1d.stats.anova2(y, A, B, equal_var=True)
 spmilist   = spmlist.inference(alpha)
```

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/0d/ex_anova2nested.py` & `spm1d-0.4.2/spm1d/examples/nonparam/0d/ex_anova2nested.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 print( dataset )
 
 
 #(1) Conduct non-parametric test:
 np.random.seed(0)
 alpha      = 0.05
 snpmlist   = spm1d.stats.nonparam.anova2nested(y, A, B)
-snpmilist  = snpmlist.inference(alpha, iterations=1000)
+snpmilist  = snpmlist.inference(alpha, iterations=200)
 print( 'Non-parametric results:')
 print( snpmilist )
 
 
 #(2) Compare to parametric test:
 spmlist    = spm1d.stats.anova2nested(y, A, B, equal_var=True)
 spmilist   = spmlist.inference(alpha)
```

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/0d/ex_anova2onerm.py` & `spm1d-0.4.2/spm1d/examples/nonparam/0d/ex_anova2onerm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/0d/ex_anova2rm.py` & `spm1d-0.4.2/spm1d/examples/nonparam/0d/ex_anova2rm.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import numpy as np
 import spm1d
 
 
 
 #(0) Load dataset:
 dataset    = spm1d.data.uv0d.anova2rm.Antidepressant()
-# dataset    = spm1d.data.uv0d.anova2rm.RSXLTraining()
-# dataset    = spm1d.data.uv0d.anova2rm.SocialNetworks()
-# dataset    = spm1d.data.uv0d.anova2rm.Southampton2rm()
+dataset    = spm1d.data.uv0d.anova2rm.RSXLTraining()
+dataset    = spm1d.data.uv0d.anova2rm.SocialNetworks()
+dataset    = spm1d.data.uv0d.anova2rm.Southampton2rm()
 # dataset    = spm1d.data.uv0d.anova2rm.SPM1D3x3()
 # dataset    = spm1d.data.uv0d.anova2rm.SPM1D3x4()
 # dataset    = spm1d.data.uv0d.anova2rm.SPM1D3x5()
 # dataset    = spm1d.data.uv0d.anova2rm.SPM1D4x4()
 # dataset    = spm1d.data.uv0d.anova2rm.SPM1D4x5()
 y,A,B,SUBJ = dataset.get_data()
 print( dataset )
@@ -21,15 +21,15 @@
 
 
 
 #(1) Conduct non-parametric test:
 np.random.seed(0)
 alpha      = 0.05
 snpmlist   = spm1d.stats.nonparam.anova2rm(y, A, B, SUBJ)
-snpmilist  = snpmlist.inference(alpha, iterations=1000)
+snpmilist  = snpmlist.inference(alpha, iterations=200)
 print( 'Non-parametric results:')
 print( snpmilist )
 
 
 
 #(2) Compare to parametric test:
 spmlist    = spm1d.stats.anova2rm(y, A, B, SUBJ, equal_var=True)
```

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/0d/ex_anova3.py` & `spm1d-0.4.2/spm1d/examples/nonparam/0d/ex_anova3.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 import numpy as np
 import spm1d
 
 
 
 #(0) Load dataset:
-# dataset   = spm1d.data.uv0d.anova3.RSItalian()
+dataset   = spm1d.data.uv0d.anova3.RSItalian()
 dataset   = spm1d.data.uv0d.anova3.SouthamptonFullyCrossedMixed()
 y,A,B,C   = dataset.get_data()
 print( dataset )
 
 
 
 #(1) Conduct non-parametric test:
```

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/0d/ex_anova3nested.py` & `spm1d-0.4.2/spm1d/examples/nonparam/0d/ex_anova3nested.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/0d/ex_anova3onerm.py` & `spm1d-0.4.2/spm1d/examples/nonparam/0d/ex_anova3tworm.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 
 import numpy as np
 import spm1d
 
 
 
 #(0) Load dataset:
-# dataset      = spm1d.data.uv0d.anova3onerm.NYUCaffeine()
-dataset      = spm1d.data.uv0d.anova3onerm.Southampton3onerm()
+dataset      = spm1d.data.uv0d.anova3tworm.NYUHiringExperience()
+dataset      = spm1d.data.uv0d.anova3tworm.Southampton3tworm()
 y,A,B,C,SUBJ = dataset.get_data()
 print( dataset )
 
 
 
-
 #(1) Conduct non-parametric test:
 np.random.seed(0)
 alpha      = 0.05
-snpmlist   = spm1d.stats.nonparam.anova3onerm(y, A, B, C, SUBJ)
+snpmlist   = spm1d.stats.nonparam.anova3tworm(y, A, B, C, SUBJ)
 snpmilist  = snpmlist.inference(alpha, iterations=500)
 print( 'Non-parametric results:')
 print( snpmilist )
 
 
 
 #(2) Compare to parametric test:
-spmlist    = spm1d.stats.anova3onerm(y, A, B, C, SUBJ, equal_var=True)
+spmlist    = spm1d.stats.anova3tworm(y, A, B, C, SUBJ, equal_var=True)
 spmilist   = spmlist.inference(alpha)
 print( 'Parametric results:')
 print( spmilist )
```

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/0d/ex_anova3rm.py` & `spm1d-0.4.2/spm1d/examples/nonparam/0d/ex_anova3onerm.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,34 @@
 
 import numpy as np
 import spm1d
 
 
 
 #(0) Load dataset:
-dataset      = spm1d.data.uv0d.anova3rm.SPM1D2x2x2()
-# dataset      = spm1d.data.uv0d.anova3rm.SPM1D2x3x5()
-# dataset      = spm1d.data.uv0d.anova3rm.SPM1D3x3x3()
+dataset      = spm1d.data.uv0d.anova3onerm.NYUCaffeine()
+dataset      = spm1d.data.uv0d.anova3onerm.Southampton3onerm()
 y,A,B,C,SUBJ = dataset.get_data()
 print( dataset )
 
 
 
 
 #(1) Conduct non-parametric test:
 np.random.seed(0)
 alpha      = 0.05
-snpmlist   = spm1d.stats.nonparam.anova3rm(y, A, B, C, SUBJ)
-snpmilist  = snpmlist.inference(alpha, iterations=1000)
-F,p        = np.array(   [(s.z, s.p)  for s in snpmilist]   ).T
-
-
-
-#(1) Conduct non-parametric test:
-np.random.seed(0)
-alpha      = 0.05
-snpmlist   = spm1d.stats.nonparam.anova3rm(y, A, B, C, SUBJ)
-snpmilist  = snpmlist.inference(alpha, iterations=200)
+snpmlist   = spm1d.stats.nonparam.anova3onerm(y, A, B, C, SUBJ)
+snpmilist  = snpmlist.inference(alpha, iterations=500)
 print( 'Non-parametric results:')
 print( snpmilist )
 
 
 
 #(2) Compare to parametric test:
-spmlist    = spm1d.stats.anova3rm(y, A, B, C, SUBJ, equal_var=True)
+spmlist    = spm1d.stats.anova3onerm(y, A, B, C, SUBJ, equal_var=True)
 spmilist   = spmlist.inference(alpha)
 print( 'Parametric results:')
 print( spmilist )
 
 
 
 
-
```

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/0d/ex_anova3tworm.py` & `spm1d-0.4.2/spm1d/examples/nonparam/0d/ex_anova1rm.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,45 @@
 
 import numpy as np
 import spm1d
 
 
 
 #(0) Load dataset:
-# dataset      = spm1d.data.uv0d.anova3tworm.NYUHiringExperience()
-dataset      = spm1d.data.uv0d.anova3tworm.Southampton3tworm()
-y,A,B,C,SUBJ = dataset.get_data()
+dataset  = spm1d.data.uv0d.anova1rm.Abdi2010()
+dataset  = spm1d.data.uv0d.anova1rm.Groceries()
+dataset  = spm1d.data.uv0d.anova1rm.Imacelebrity()
+# dataset  = spm1d.data.uv0d.anova1rm.Southampton1rm()
+y,A,SUBJ = dataset.get_data()
 print( dataset )
 
 
 
+
 #(1) Conduct non-parametric test:
 np.random.seed(0)
 alpha      = 0.05
-snpmlist   = spm1d.stats.nonparam.anova3tworm(y, A, B, C, SUBJ)
-snpmilist  = snpmlist.inference(alpha, iterations=500)
-print( 'Non-parametric results:')
-print( snpmilist )
-
+F          = spm1d.stats.nonparam.anova1rm(y, A, SUBJ)
+Fi         = F.inference(alpha, iterations=1000)
+print(Fi)
 
 
 #(2) Compare to parametric test:
-spmlist    = spm1d.stats.anova3tworm(y, A, B, C, SUBJ, equal_var=True)
-spmilist   = spmlist.inference(alpha)
-print( 'Parametric results:')
-print( spmilist )
+Fparam     = spm1d.stats.anova1rm(y, A, SUBJ, equal_var=True)
+Fparami    = Fparam.inference(alpha)
+
+
+
+#(3) Print results:
+print
+print( 'Non-parametric results:' )
+print( '   t=%.3f, p=%.5f' %(Fi.z, Fi.p) )
+print
+print( 'Parametric results:' )
+print( '   t=%.3f, p=%.5f' %(Fparami.z, Fparami.p) )
+print
+
+
```

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/0d/ex_cca.py` & `spm1d-0.4.2/spm1d/examples/nonparam/0d/ex_cca.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/0d/ex_ci_onesample.py` & `spm1d-0.4.2/spm1d/examples/nonparam/0d/ex_ci_onesample.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 #(0) Load dataset:
-# dataset = spm1d.data.uv0d.ci1.MinnesotaGeyerRate()
+dataset = spm1d.data.uv0d.ci1.MinnesotaGeyerRate()
 dataset = spm1d.data.uv0d.ci1.WebsterSleep()
 y,mu    = dataset.get_data()
 print( dataset )
 
 
 
 #(1) Compare parametric and non-parametric confidence intervals:
@@ -22,15 +22,14 @@
 cinp       = spm1d.stats.nonparam.ci_onesample(y, alpha, mu=mu, iterations=iterations)
 print( ci )
 print( cinp )
 
 
 
 #(2) Plot the CIs:
-plt.close('all')
-plt.figure(figsize=(8,4))
+pyplot.close('all')
+pyplot.figure(figsize=(8,4))
 
-ax0 = plt.subplot(121);  ci.plot(ax0);    ax0.set_title('Parametric', size=10)
-ax1 = plt.subplot(122);  cinp.plot(ax1);  ax1.set_title('Non-parametric', size=10)
-plt.suptitle('One-sample CIs')
-plt.tight_layout()
-plt.show()
+ax0 = pyplot.subplot(121);  ci.plot(ax0);    ax0.set_title('Parametric', size=10)
+ax1 = pyplot.subplot(122);  cinp.plot(ax1);  ax1.set_title('Non-parametric', size=10)
+pyplot.suptitle('One-sample CIs')
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/0d/ex_ci_pairedsample.py` & `spm1d-0.4.2/spm1d/examples/nonparam/1d/ex_regression.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,49 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
+
 #(0) Load dataset:
-dataset = spm1d.data.uv0d.cipaired.FraminghamSystolicBloodPressure()
-yA,yB   = dataset.get_data()
-print( dataset )
-# yB += 1.9
+dataset    = spm1d.data.uv1d.regress.SimulatedPataky2015c()
+dataset    = spm1d.data.uv1d.regress.SpeedGRF()
+y,x        = dataset.get_data()
 
 
 
-#(1) Compute parametric and non-parametric confidence intervals:
+#(1) Conduct non-parametric test:
 np.random.seed(0)
 alpha      = 0.05
-mu         = 0
-iterations = 1000
-ci         = spm1d.stats.ci_pairedsample(yA, yB, alpha, datum='meanA', mu='meanB')
-cinp       = spm1d.stats.nonparam.ci_pairedsample(yA, yB, alpha, datum='meanA', mu='meanB', iterations=iterations)
-print( ci )
-print( cinp )
+two_tailed = False
+snpm       = spm1d.stats.nonparam.regress(y, x)
+snpmi      = snpm.inference(alpha, two_tailed=two_tailed, iterations=500)
+print( snpmi )
+print( snpmi.clusters )
+
+
+
+#(2) Compare with parametric result:
+spm        = spm1d.stats.regress(y, x)
+spmi       = spm.inference(alpha, two_tailed=two_tailed)
+print( spmi )
+print( snpmi.clusters )
+
+
 
+#(3) Plot
+pyplot.close('all')
+pyplot.figure(figsize=(12,4))
+
+ax0 = pyplot.subplot(121)
+ax1 = pyplot.subplot(122)
+labels = 'Parametric', 'Non-parametric'
+for ax,zi,label in zip([ax0,ax1], [spmi,snpmi], labels):
+	zi.plot(ax=ax)
+	zi.plot_threshold_label(ax=ax, fontsize=8)
+	zi.plot_p_values(ax=ax, size=10)
+	ax.set_title( label )
+pyplot.show()
 
 
-#(2) Plot the CIs:
-plt.close('all')
-plt.figure(figsize=(8,4))
-
-ax0 = plt.subplot(121);  ci.plot(ax0);    ax0.set_title('Parametric', size=10)
-ax1 = plt.subplot(122);  cinp.plot(ax1);  ax1.set_title('Non-parametric', size=10)
-plt.suptitle('One-sample CIs')
-plt.tight_layout()
-plt.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/0d/ex_ci_twosample.py` & `spm1d-0.4.2/spm1d/examples/nonparam/0d/ex_ci_twosample.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 #(0) Load dataset:
 dataset = spm1d.data.uv0d.ci2.AnimalsInResearch()
 yA,yB   = dataset.get_data()
@@ -20,15 +20,14 @@
 cinp       = spm1d.stats.nonparam.ci_twosample(yA, yB, alpha, datum='meanA', mu='meanB', iterations=iterations)
 print( ci )
 print( cinp )
 
 
 
 #(2) Plot the CIs:
-plt.close('all')
-plt.figure(figsize=(8,4))
+pyplot.close('all')
+pyplot.figure(figsize=(8,4))
 
-ax0 = plt.subplot(121);  ci.plot(ax0);    ax0.set_title('Parametric', size=10)
-ax1 = plt.subplot(122);  cinp.plot(ax1);  ax1.set_title('Non-parametric', size=10)
-plt.suptitle('Two-sample CIs')
-plt.tight_layout()
-plt.show()
+ax0 = pyplot.subplot(121);  ci.plot(ax0);    ax0.set_title('Parametric', size=10)
+ax1 = pyplot.subplot(122);  cinp.plot(ax1);  ax1.set_title('Non-parametric', size=10)
+pyplot.suptitle('Two-sample CIs')
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/0d/ex_hotellings.py` & `spm1d-0.4.2/spm1d/examples/nonparam/0d/ex_hotellings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 
 import numpy as np
 import spm1d
 
 
 
 #(0) Load dataset:
-# dataset = spm1d.data.mv0d.hotellings1.RSXLHotellings1()
-dataset = spm1d.data.mv0d.hotellings1.Sweat()
+dataset = spm1d.data.mv0d.hotellings1.RSXLHotellings1()
+# dataset = spm1d.data.mv0d.hotellings1.Sweat()
 y,mu    = dataset.Y, dataset.mu
 # y       = y[:10]
 
 
 #(1) Conduct non-parametric test:
 np.random.seed(10)
 alpha      = 0.05
```

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/0d/ex_hotellings2.py` & `spm1d-0.4.2/spm1d/examples/nonparam/0d/ex_hotellings2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 
 import numpy as np
 import spm1d
 
 
 
 #(0) Load dataset:
-# dataset = spm1d.data.mv0d.hotellings2.RSXLHotellings2()
-dataset = spm1d.data.mv0d.hotellings2.HELPHomeless()
+dataset = spm1d.data.mv0d.hotellings2.RSXLHotellings2()
+# dataset = spm1d.data.mv0d.hotellings2.HELPHomeless()
 yA,yB   = dataset.get_data()
 # yA,yB   = [y[:10]  for y in [yA,yB]]
 
 
 
 #(1) Conduct non-parametric test:
 np.random.seed(0)
```

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/0d/ex_hotellings_paired.py` & `spm1d-0.4.2/spm1d/examples/nonparam/0d/ex_hotellings_paired.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/0d/ex_manova1.py` & `spm1d-0.4.2/spm1d/examples/nonparam/0d/ex_manova1.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import spm1d
 
 
 
 
 #(0) Load dataset:
 dataset = spm1d.data.mv0d.manova1.AnimalDepression()
-# dataset = spm1d.data.mv0d.manova1.Stevens2002()
+dataset = spm1d.data.mv0d.manova1.Stevens2002()
 y,A     = dataset.Y, dataset.A
 print( dataset )
 
 
 
 #(1) Conduct non-parametric test:
 np.random.seed(0)
```

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/0d/ex_regress.py` & `spm1d-0.4.2/spm1d/examples/nonparam/0d/ex_regress.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/0d/ex_ttest.py` & `spm1d-0.4.2/spm1d/examples/nonparam/0d/ex_ttest.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/0d/ex_ttest2.py` & `spm1d-0.4.2/spm1d/examples/nonparam/0d/ex_ttest2.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/0d/ex_ttest2_standalone.py` & `spm1d-0.4.2/spm1d/examples/nonparam/0d/ex_ttest2_standalone.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/0d/ex_ttest_paired.py` & `spm1d-0.4.2/spm1d/examples/nonparam/0d/ex_ttest_paired.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/0d/ex_ttest_standalone.py` & `spm1d-0.4.2/spm1d/examples/nonparam/0d/ex_ttest_standalone.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/1d/ex_anova1.py` & `spm1d-0.4.2/spm1d/examples/nonparam/1d/roi/ex_anova1.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,50 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 
 #(0) Load dataset:
-dataset      = spm1d.data.uv1d.anova1.SpeedGRFcategorical()
-# dataset      = spm1d.data.uv1d.anova1.Weather()
-y,A          = dataset.get_data()
-
-
+dataset    = spm1d.data.uv1d.anova1.SpeedGRFcategorical()
+# dataset    = spm1d.data.uv1d.anova1.Weather()
+y,A        = dataset.get_data()
+
+#(0a) Create region of interest(ROI):
+roi        = np.array( [False]*y.shape[1] )
+roi[15:75] = True
 
 
 #(1) Conduct non-parametric test:
 np.random.seed(0)
 alpha      = 0.05
-snpm       = spm1d.stats.nonparam.anova1(y, A)
-snpmi      = snpm.inference(alpha, iterations=500)
+snpm       = spm1d.stats.nonparam.anova1(y, A, roi=roi)
+snpmi      = snpm.inference(alpha, iterations=200)
 print( snpmi )
 
 
 
 
 #(2) Compare with parametric result:
-spm        = spm1d.stats.anova1(y, A, equal_var=True)
+spm        = spm1d.stats.anova1(y, A, equal_var=True, roi=roi)
 spmi       = spm.inference(alpha)
 print( spmi )
 
 
 
 
 #(3) Plot
-plt.close('all')
-plt.figure(figsize=(10,4))
+pyplot.close('all')
+pyplot.figure(figsize=(12,4))
 
-ax0 = plt.subplot(121)
-ax1 = plt.subplot(122)
+ax0 = pyplot.subplot(121)
+ax1 = pyplot.subplot(122)
 labels = 'Parametric', 'Non-parametric'
 for ax,zi,label in zip([ax0,ax1], [spmi,snpmi], labels):
 	zi.plot(ax=ax)
 	zi.plot_threshold_label(ax=ax, fontsize=8)
 	zi.plot_p_values(ax=ax, size=10)
 	ax.set_title( label )
-plt.tight_layout()
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/1d/ex_anova1rm.py` & `spm1d-0.4.2/spm1d/examples/nonparam/1d/ex_anova1rm.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 
 #(0) Load dataset:
 dataset      = spm1d.data.uv1d.anova1rm.SpeedGRFcategoricalRM()
@@ -28,22 +28,21 @@
 spmi       = spm.inference(alpha)
 print( spmi )
 
 
 
 
 #(3) Plot
-plt.close('all')
-plt.figure(figsize=(10,4))
+pyplot.close('all')
+pyplot.figure(figsize=(12,4))
 
-ax0 = plt.subplot(121)
-ax1 = plt.subplot(122)
+ax0 = pyplot.subplot(121)
+ax1 = pyplot.subplot(122)
 labels = 'Parametric', 'Non-parametric'
 for ax,zi,label in zip([ax0,ax1], [spmi,snpmi], labels):
 	zi.plot(ax=ax)
 	zi.plot_threshold_label(ax=ax, fontsize=8)
 	zi.plot_p_values(ax=ax, size=10)
 	ax.set_title( label )
-plt.tight_layout()
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/1d/ex_anova2.py` & `spm1d-0.4.2/spm1d/examples/nonparam/1d/ex_anova2.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 
 #(0) Load dataset:
 dataset      = spm1d.data.uv1d.anova2.SPM1D_ANOVA2_2x2()
@@ -18,33 +18,31 @@
 
 
 
 #(1) Conduct non-parametric test:
 np.random.seed(0)
 alpha      = 0.05
 FFn        = spm1d.stats.nonparam.anova2(y, A, B)
-FFni       = FFn.inference(alpha, iterations=500)
+FFni       = FFn.inference(alpha, iterations=200)
 print( FFni )
 
 
 
 #(2) Compare with parametric result:
 FF         = spm1d.stats.anova2(y, A, B, equal_var=True)
 FFi        = FF.inference(alpha)
 print( FFi )
 
 
 
 #(3) Plot results:
-plt.close('all')
-plt.figure( figsize=(10,6) )
+pyplot.close('all')
 FFni.plot(plot_threshold_label=True, plot_p_values=True, autoset_ylim=True)
 ### optionally plot parametric thresholds for comparison:
 for i,Fi in enumerate(FFi):
-	ax = plt.subplot(2,2,i+1)
+	ax = pyplot.subplot(2,2,i+1)
 	ax.axhline( Fi.zstar, color='c', linestyle='--' )
 	ax.text(2, Fi.zstar, 'Parametric', color='c')
-plt.tight_layout()
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/1d/ex_anova2nested.py` & `spm1d-0.4.2/spm1d/examples/nonparam/1d/ex_anova2nested.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 
 #(0) Load dataset:
 # dataset      = spm1d.data.uv1d.anova2nested.SPM1D_ANOVA2NESTED_2x2()
@@ -31,18 +31,16 @@
 FF         = spm1d.stats.anova2nested(y, A, B, equal_var=True)
 FFi        = FF.inference(alpha)
 print( FFi )
 
 
 
 #(3) Plot results:
-plt.close('all')
-plt.figure( figsize=(10,6) )
+pyplot.close('all')
 FFni.plot(plot_threshold_label=True, plot_p_values=True, autoset_ylim=True)
 ### optionally plot parametric thresholds for comparison:
 for i,Fi in enumerate(FFi):
-	ax = plt.subplot(2,2,i+1)
+	ax = pyplot.subplot(2,2,i+1)
 	ax.axhline( Fi.zstar, color='c', linestyle='--' )
 	ax.text(2, Fi.zstar, 'Parametric', color='c')
-plt.tight_layout()
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/1d/ex_anova2onerm.py` & `spm1d-0.4.2/spm1d/examples/nonparam/1d/ex_anova2rm.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,46 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 
 #(0) Load dataset:
-dataset      = spm1d.data.uv1d.anova2onerm.SPM1D_ANOVA2ONERM_2x2()
-# dataset      = spm1d.data.uv1d.anova2onerm.SPM1D_ANOVA2ONERM_2x3()
-# dataset      = spm1d.data.uv1d.anova2onerm.SPM1D_ANOVA2ONERM_3x3()
-# dataset      = spm1d.data.uv1d.anova2onerm.SPM1D_ANOVA2ONERM_3x4()
-# dataset      = spm1d.data.uv1d.anova2onerm.SPM1D_ANOVA2ONERM_3x5()
-# dataset      = spm1d.data.uv1d.anova2onerm.SPM1D_ANOVA2ONERM_4x4()
-# dataset      = spm1d.data.uv1d.anova2onerm.SPM1D_ANOVA2ONERM_4x5()
+dataset      = spm1d.data.uv1d.anova2rm.SPM1D_ANOVA2RM_2x2()
+# dataset      = spm1d.data.uv1d.anova2rm.SPM1D_ANOVA2RM_2x3()
+# dataset      = spm1d.data.uv1d.anova2rm.SPM1D_ANOVA2RM_3x3()
+# dataset      = spm1d.data.uv1d.anova2rm.SPM1D_ANOVA2RM_3x4()
+# dataset      = spm1d.data.uv1d.anova2rm.SPM1D_ANOVA2RM_3x5()
+# dataset      = spm1d.data.uv1d.anova2rm.SPM1D_ANOVA2RM_4x4()
+# dataset      = spm1d.data.uv1d.anova2rm.SPM1D_ANOVA2RM_4x5()
 y,A,B,SUBJ   = dataset.get_data()
 
 
 
 #(1) Conduct non-parametric test:
 np.random.seed(0)
 alpha      = 0.05
-FFn        = spm1d.stats.nonparam.anova2onerm(y, A, B, SUBJ)
+FFn        = spm1d.stats.nonparam.anova2rm(y, A, B, SUBJ)
 FFni       = FFn.inference(alpha, iterations=500)
 print( FFni )
 
 
 
 #(2) Compare with parametric result:
-FF         = spm1d.stats.anova2onerm(y, A, B, SUBJ, equal_var=True)
+FF         = spm1d.stats.anova2rm(y, A, B, SUBJ, equal_var=True)
 FFi        = FF.inference(alpha)
 print( FFi )
 
 
 
 #(3) Plot results:
-plt.close('all')
-plt.figure( figsize=(10,6) )
+pyplot.close('all')
 FFni.plot(plot_threshold_label=True, plot_p_values=True, autoset_ylim=True)
 ### optionally plot parametric thresholds for comparison:
 for i,Fi in enumerate(FFi):
-	ax = plt.subplot(2,2,i+1)
+	ax = pyplot.subplot(2,2,i+1)
 	ax.axhline( Fi.zstar, color='c', linestyle='--' )
 	ax.text(2, Fi.zstar, 'Parametric', color='c')
-plt.tight_layout()
-plt.show()
-
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/1d/ex_anova2rm.py` & `spm1d-0.4.2/spm1d/examples/nonparam/1d/roi/ex_anova2rm.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 
 #(0) Load dataset:
 dataset      = spm1d.data.uv1d.anova2rm.SPM1D_ANOVA2RM_2x2()
@@ -12,37 +12,48 @@
 # dataset      = spm1d.data.uv1d.anova2rm.SPM1D_ANOVA2RM_3x3()
 # dataset      = spm1d.data.uv1d.anova2rm.SPM1D_ANOVA2RM_3x4()
 # dataset      = spm1d.data.uv1d.anova2rm.SPM1D_ANOVA2RM_3x5()
 # dataset      = spm1d.data.uv1d.anova2rm.SPM1D_ANOVA2RM_4x4()
 # dataset      = spm1d.data.uv1d.anova2rm.SPM1D_ANOVA2RM_4x5()
 y,A,B,SUBJ   = dataset.get_data()
 
+#(0a) Create region of interest(ROI):
+roi        = np.array( [False]*y.shape[1] )
+roi[25:45] = True
 
 
 #(1) Conduct non-parametric test:
 np.random.seed(0)
 alpha      = 0.05
-FFn        = spm1d.stats.nonparam.anova2rm(y, A, B, SUBJ)
+FFn        = spm1d.stats.nonparam.anova2rm(y, A, B, SUBJ, roi=roi)
 FFni       = FFn.inference(alpha, iterations=500)
 print( FFni )
 
 
 
 #(2) Compare with parametric result:
-FF         = spm1d.stats.anova2rm(y, A, B, SUBJ, equal_var=True)
+FF         = spm1d.stats.anova2rm(y, A, B, SUBJ, equal_var=True, roi=roi)
 FFi        = FF.inference(alpha)
 print( FFi )
 
 
 
-#(3) Plot results:
-plt.close('all')
-plt.figure( figsize=(10,6) )
-FFni.plot(plot_threshold_label=True, plot_p_values=True, autoset_ylim=True)
-### optionally plot parametric thresholds for comparison:
-for i,Fi in enumerate(FFi):
-	ax = plt.subplot(2,2,i+1)
-	ax.axhline( Fi.zstar, color='c', linestyle='--' )
-	ax.text(2, Fi.zstar, 'Parametric', color='c')
-plt.tight_layout()
-plt.show()
+#(3) Plot
+pyplot.close('all')
+pyplot.figure(figsize=(15,4))
+
+for i,(Fi,Fni) in enumerate( zip(FFi,FFni) ):
+	ax = pyplot.subplot(1,3,i+1)
+	Fni.plot(ax=ax)
+	Fni.plot_threshold_label(ax=ax, fontsize=8)
+	Fni.plot_p_values(ax=ax, size=10)
+	ax.axhline( Fi.zstar, color='orange', linestyle='--', label='Parametric threshold')
+	if (Fi.zstar > Fi.z.max()) and (Fi.zstar>Fni.zstar):
+		ax.set_ylim(0, Fi.zstar+1)
+	if i==0:
+		ax.legend(fontsize=10, loc='best')
+	ax.set_title( Fni.effect )
+pyplot.show()
+
+
+
```

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/1d/ex_anova3.py` & `spm1d-0.4.2/spm1d/examples/nonparam/1d/ex_anova3.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 
 #(0) Load dataset:
 dataset      = spm1d.data.uv1d.anova3.SPM1D_ANOVA3_2x2x2()
@@ -13,30 +13,28 @@
 
 
 
 #(1) Conduct non-parametric test:
 np.random.seed(0)
 alpha      = 0.05
 FFn        = spm1d.stats.nonparam.anova3(y, A, B, C)
-FFni       = FFn.inference(alpha, iterations=500)
+FFni       = FFn.inference(alpha, iterations=200)
 print( FFni )
 
 
 
 #(2) Compare with parametric result:
 FF         = spm1d.stats.anova3(y, A, B, C, equal_var=True)
 FFi        = FF.inference(alpha)
 print( FFi )
 
 
 
 #(3) Plot results:
-plt.close('all')
-plt.figure( figsize=(10,6) )
+pyplot.close('all')
 FFni.plot(plot_threshold_label=False, plot_p_values=True, autoset_ylim=True)
-### optionally plot parametric thresholds for comparison:
-for i,Fi in enumerate(FFi):
-	ax = plt.subplot(3,3,i+1)
-	ax.axhline( Fi.zstar, color='c', linestyle='--' )
-	ax.text(2, Fi.zstar, 'Parametric', color='c')
-plt.tight_layout()
-plt.show()
+# ### optionally plot parametric thresholds for comparison:
+# for i,Fi in enumerate(FFi):
+# 	ax = pyplot.subplot(3,3,i+1)
+# 	ax.axhline( Fi.zstar, color='c', linestyle='--' )
+# 	ax.text(2, Fi.zstar, 'Parametric', color='c')
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/1d/ex_anova3nested.py` & `spm1d-0.4.2/spm1d/examples/nonparam/1d/roi/ex_anova3.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,54 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 
 #(0) Load dataset:
-# dataset      = spm1d.data.uv1d.anova3nested.SPM1D_ANOVA3NESTED_2x2x2()
-dataset      = spm1d.data.uv1d.anova3nested.SPM1D_ANOVA3NESTED_2x4x2()
+dataset      = spm1d.data.uv1d.anova3.SPM1D_ANOVA3_2x2x2()
+# dataset      = spm1d.data.uv1d.anova3.SPM1D_ANOVA3_2x3x4()
 y,A,B,C      = dataset.get_data()
 
+#(0a) Create region of interest(ROI):
+roi        = np.array( [False]*y.shape[1] )
+roi[25:45] = True
+
 
 #(1) Conduct non-parametric test:
 np.random.seed(0)
 alpha      = 0.05
-FFn        = spm1d.stats.nonparam.anova3nested(y, A, B, C)
+FFn        = spm1d.stats.nonparam.anova3(y, A, B, C, roi=roi)
 FFni       = FFn.inference(alpha, iterations=200)
 print( FFni )
 
 
 
 #(2) Compare with parametric result:
-FF         = spm1d.stats.anova3nested(y, A, B, C, equal_var=True)
+FF         = spm1d.stats.anova3(y, A, B, C, equal_var=True, roi=roi)
 FFi        = FF.inference(alpha)
 print( FFi )
 
 
 
-#(3) Plot results:
-plt.close('all')
-plt.figure(figsize=(12,8))
-FFni.plot(plot_threshold_label=False, plot_p_values=True, autoset_ylim=True)
-### optionally plot parametric thresholds for comparison:
-for i,Fi in enumerate(FFi):
-	ax = plt.subplot(3,3,i+1)
-	ax.axhline( Fi.zstar, color='c', linestyle='--' )
-	ax.text(2, Fi.zstar, 'Parametric', color='c')
-plt.tight_layout()
-plt.show()
+#(3) Plot
+pyplot.close('all')
+pyplot.figure(figsize=(15,8))
+
+for i,(Fi,Fni) in enumerate( zip(FFi,FFni) ):
+	ax = pyplot.subplot(3,3,i+1)
+	Fni.plot(ax=ax)
+	Fni.plot_threshold_label(ax=ax, fontsize=8)
+	Fni.plot_p_values(ax=ax, size=10)
+	ax.axhline( Fi.zstar, color='orange', linestyle='--', label='Parametric threshold')
+	if (Fi.zstar > Fi.z.max()) and (Fi.zstar>Fni.zstar):
+		ax.set_ylim(0, Fi.zstar+1)
+	if i==0:
+		ax.legend(fontsize=10, loc='best')
+	ax.set_title( Fni.effect )
+pyplot.show()
+
+
+
+
```

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/1d/ex_anova3onerm.py` & `spm1d-0.4.2/spm1d/examples/nonparam/1d/roi/ex_anova3onerm.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,54 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 
 #(0) Load dataset:
 dataset      = spm1d.data.uv1d.anova3onerm.SPM1D_ANOVA3ONERM_2x2x2()
 # dataset      = spm1d.data.uv1d.anova3onerm.SPM1D_ANOVA3ONERM_2x3x4()
 y,A,B,C,SUBJ = dataset.get_data()
 
+#(0a) Create region of interest(ROI):
+roi        = np.array( [False]*y.shape[1] )
+roi[25:45] = True
 
 
 #(1) Conduct non-parametric test:
 np.random.seed(0)
 alpha      = 0.05
-FFn        = spm1d.stats.nonparam.anova3onerm(y, A, B, C, SUBJ)
+FFn        = spm1d.stats.nonparam.anova3onerm(y, A, B, C, SUBJ, roi=roi)
 FFni       = FFn.inference(alpha, iterations=200)
 print( FFni )
 
 
 
 #(2) Compare with parametric result:
-FF         = spm1d.stats.anova3onerm(y, A, B, C, SUBJ, equal_var=True)
+FF         = spm1d.stats.anova3onerm(y, A, B, C, SUBJ, equal_var=True, roi=roi)
 FFi        = FF.inference(alpha)
 print( FFi )
 
 
 
 #(3) Plot
-plt.close('all')
-plt.figure(figsize=(12,8))
+pyplot.close('all')
+pyplot.figure(figsize=(15,8))
 
 for i,(Fi,Fni) in enumerate( zip(FFi,FFni) ):
-	ax = plt.subplot(3,3,i+1)
+	ax = pyplot.subplot(3,3,i+1)
 	Fni.plot(ax=ax)
 	Fni.plot_threshold_label(ax=ax, fontsize=8)
 	Fni.plot_p_values(ax=ax, size=10)
 	ax.axhline( Fi.zstar, color='orange', linestyle='--', label='Parametric threshold')
 	if (Fi.zstar > Fi.z.max()) and (Fi.zstar>Fni.zstar):
 		ax.set_ylim(0, Fi.zstar+1)
 	if i==0:
 		ax.legend(fontsize=10, loc='best')
 	ax.set_title( Fni.effect )
-plt.tight_layout()
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/1d/ex_anova3rm.py` & `spm1d-0.4.2/spm1d/examples/nonparam/1d/roi/ex_anova3rm.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,54 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 
 #(0) Load dataset:
 dataset      = spm1d.data.uv1d.anova3rm.SPM1D_ANOVA3RM_2x2x2()
 # dataset      = spm1d.data.uv1d.anova3rm.SPM1D_ANOVA3RM_2x3x4()
 y,A,B,C,SUBJ = dataset.get_data()
 
+#(0a) Create region of interest(ROI):
+roi        = np.array( [False]*y.shape[1] )
+roi[25:45] = True
 
 
 #(1) Conduct non-parametric test:
 np.random.seed(0)
 alpha      = 0.05
-FFn        = spm1d.stats.nonparam.anova3rm(y, A, B, C, SUBJ)
+FFn        = spm1d.stats.nonparam.anova3rm(y, A, B, C, SUBJ, roi=roi)
 FFni       = FFn.inference(alpha, iterations=200)
 print( FFni )
 
 
 
 #(2) Compare with parametric result:
-FF         = spm1d.stats.anova3rm(y, A, B, C, SUBJ, equal_var=True)
+FF         = spm1d.stats.anova3rm(y, A, B, C, SUBJ, equal_var=True, roi=roi)
 FFi        = FF.inference(alpha)
 print( FFi )
 
 
 
 #(3) Plot
-plt.close('all')
-plt.figure(figsize=(12,8))
+pyplot.close('all')
+pyplot.figure(figsize=(15,8))
 
 for i,(Fi,Fni) in enumerate( zip(FFi,FFni) ):
-	ax = plt.subplot(3,3,i+1)
+	ax = pyplot.subplot(3,3,i+1)
 	Fni.plot(ax=ax)
 	Fni.plot_threshold_label(ax=ax, fontsize=8)
 	Fni.plot_p_values(ax=ax, size=10)
 	ax.axhline( Fi.zstar, color='orange', linestyle='--', label='Parametric threshold')
 	if (Fi.zstar > Fi.z.max()) and (Fi.zstar>Fni.zstar):
 		ax.set_ylim(0, Fi.zstar+1)
 	if i==0:
 		ax.legend(fontsize=10, loc='best')
 	ax.set_title( Fni.effect )
-plt.tight_layout()
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/1d/ex_anova3tworm.py` & `spm1d-0.4.2/spm1d/examples/nonparam/1d/ex_anova3onerm.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,51 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 
 #(0) Load dataset:
-dataset      = spm1d.data.uv1d.anova3tworm.SPM1D_ANOVA3TWORM_2x2x2()
-# dataset      = spm1d.data.uv1d.anova3tworm.SPM1D_ANOVA3TWORM_2x3x4()
+dataset      = spm1d.data.uv1d.anova3onerm.SPM1D_ANOVA3ONERM_2x2x2()
+# dataset      = spm1d.data.uv1d.anova3onerm.SPM1D_ANOVA3ONERM_2x3x4()
 y,A,B,C,SUBJ = dataset.get_data()
 
 
 
 #(1) Conduct non-parametric test:
 np.random.seed(0)
 alpha      = 0.05
-FFn        = spm1d.stats.nonparam.anova3tworm(y, A, B, C, SUBJ)
+FFn        = spm1d.stats.nonparam.anova3onerm(y, A, B, C, SUBJ)
 FFni       = FFn.inference(alpha, iterations=200)
 print( FFni )
 
 
 
 #(2) Compare with parametric result:
-FF         = spm1d.stats.anova3tworm(y, A, B, C, SUBJ, equal_var=True)
+FF         = spm1d.stats.anova3onerm(y, A, B, C, SUBJ, equal_var=True)
 FFi        = FF.inference(alpha)
 print( FFi )
 
 
 
 #(3) Plot
-plt.close('all')
-plt.figure(figsize=(12,8))
+pyplot.close('all')
+pyplot.figure(figsize=(15,10))
 
 for i,(Fi,Fni) in enumerate( zip(FFi,FFni) ):
-	ax = plt.subplot(3,3,i+1)
+	ax = pyplot.subplot(3,3,i+1)
 	Fni.plot(ax=ax)
 	Fni.plot_threshold_label(ax=ax, fontsize=8)
 	Fni.plot_p_values(ax=ax, size=10)
 	ax.axhline( Fi.zstar, color='orange', linestyle='--', label='Parametric threshold')
 	if (Fi.zstar > Fi.z.max()) and (Fi.zstar>Fni.zstar):
 		ax.set_ylim(0, Fi.zstar+1)
 	if i==0:
 		ax.legend(fontsize=10, loc='best')
 	ax.set_title( Fni.effect )
-plt.tight_layout()
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/1d/ex_cca.py` & `spm1d-0.4.2/spm1d/examples/nonparam/1d/roi/ex_regression.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,52 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 
 #(0) Load dataset:
-dataset      = spm1d.data.mv1d.cca.Dorn2012()
-y,x          = dataset.get_data()  #A:slow, B:fast
-
+dataset    = spm1d.data.uv1d.regress.SimulatedPataky2015c()
+dataset    = spm1d.data.uv1d.regress.SpeedGRF()
+y,x        = dataset.get_data()
+
+#(0a) Create region of interest(ROI):
+roi        = np.array( [False]*y.shape[1] )
+roi[70:80] = True
 
 
 #(1) Conduct non-parametric test:
 np.random.seed(0)
 alpha      = 0.05
 two_tailed = False
-snpm       = spm1d.stats.nonparam.cca(y, x)
-snpmi      = snpm.inference(alpha, iterations=100)
+snpm       = spm1d.stats.nonparam.regress(y, x, roi=roi)
+snpmi      = snpm.inference(alpha, two_tailed=two_tailed, iterations=500)
 print( snpmi )
 
 
 
+
 #(2) Compare with parametric result:
-spm        = spm1d.stats.cca(y, x)
-spmi       = spm.inference(alpha)
+spm        = spm1d.stats.regress(y, x, roi=roi)
+spmi       = spm.inference(alpha, two_tailed=two_tailed)
 print( spmi )
 
 
 
+
 #(3) Plot
-plt.close('all')
-plt.figure(figsize=(10,4))
+pyplot.close('all')
+pyplot.figure(figsize=(12,4))
 
-ax0 = plt.subplot(121)
-ax1 = plt.subplot(122)
+ax0 = pyplot.subplot(121)
+ax1 = pyplot.subplot(122)
 labels = 'Parametric', 'Non-parametric'
 for ax,zi,label in zip([ax0,ax1], [spmi,snpmi], labels):
 	zi.plot(ax=ax)
 	zi.plot_threshold_label(ax=ax, fontsize=8)
 	zi.plot_p_values(ax=ax, size=10)
 	ax.set_title( label )
-plt.tight_layout()
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/1d/ex_ci_onesample.py` & `spm1d-0.4.2/spm1d/examples/nonparam/1d/ex_ci_pairedsample.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,47 +1,41 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 #(0) Load dataset:
-dataset    = spm1d.data.uv1d.t1.Random()
-# dataset    = spm1d.data.uv1d.t1.SimulatedPataky2015a()
-# dataset    = spm1d.data.uv1d.t1.SimulatedPataky2015b()
-y,mu       = dataset.get_data()
+dataset      = spm1d.data.uv1d.t2.PlantarArchAngle()
+yA,yB        = dataset.get_data()  #normal and fast walking
 
 
 
 
-#(1) Compare parametric and non-parametric CIs:
+
+#(1) Compute confidence intervals:
 np.random.seed(0)
 alpha      = 0.05
-mu         = 0
 iterations = -1
-ci         = spm1d.stats.ci_onesample(y, alpha, mu=mu)
-cinp       = spm1d.stats.nonparam.ci_onesample(y, alpha, mu=mu, iterations=iterations)
+ci         = spm1d.stats.ci_pairedsample(yA, yB, alpha, datum='meanA', mu='meanB')
+cinp       = spm1d.stats.nonparam.ci_pairedsample(yA, yB, alpha, datum='meanA', mu='meanB', iterations=iterations)
 print( ci )
 print( cinp )
 
 
 
-
 #(2) Plot the CIs:
-plt.close('all')
-plt.figure(figsize=(10,4))
+pyplot.close('all')
+pyplot.figure(figsize=(10,4))
 
 ### plot parametric CI:
-ax = plt.subplot(121)
+ax = pyplot.subplot(121)
 ci.plot(ax)
 ax.set_title('Parametric CI', size=10)
 ### plot parametric CI:
-ax = plt.subplot(122)
+ax = pyplot.subplot(122)
 cinp.plot(ax)
 ax.set_title('Non-parametric CI', size=10)
-plt.suptitle('One-sample CIs')
-plt.tight_layout()
-plt.show()
-
-
+pyplot.suptitle('Paired-sample CIs')
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/1d/ex_ci_twosample.py` & `spm1d-0.4.2/spm1d/examples/nonparam/1d/ex_ci_twosample.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 #(0) Load dataset:
 # dataset      = spm1d.data.uv1d.t2.PlantarArchAngle()
 dataset      = spm1d.data.uv1d.t2.SimulatedTwoLocalMax()
@@ -20,24 +20,23 @@
 cinp       = spm1d.stats.nonparam.ci_twosample(yA, yB, alpha, datum='meanA', mu='meanB', iterations=iterations)
 print( ci )
 print( cinp )
 
 
 
 #(2) Plot the CIs:
-plt.close('all')
-plt.figure(figsize=(10,4))
+pyplot.close('all')
+pyplot.figure(figsize=(10,4))
 
 ### plot parametric CI:
-ax = plt.subplot(121)
+ax = pyplot.subplot(121)
 ci.plot(ax)
 ax.set_title('Parametric CI', size=10)
 ### plot parametric CI:
-ax = plt.subplot(122)
+ax = pyplot.subplot(122)
 cinp.plot(ax)
 ax.set_title('Non-parametric CI', size=10)
-plt.suptitle('Two-sample CIs')
-plt.tight_layout()
-plt.show()
+pyplot.suptitle('Two-sample CIs')
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/1d/ex_hotellings.py` & `spm1d-0.4.2/spm1d/examples/nonparam/1d/roi/ex_hotellings.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,53 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 
 #(0) Load dataset:
 # dataset      = spm1d.data.mv1d.hotellings_paired.Neptune1999kneekin()
 dataset      = spm1d.data.mv1d.hotellings_paired.Pataky2014cop()
 yA,yB        = dataset.get_data()  #A:slow, B:fast
 y            = yA - yB
 mu           = 0
 
+#(0a) Create region of interest(ROI):
+roi        = np.array( [False]*yA.shape[1] )
+roi[70:80] = True
 
 
 #(1) Conduct non-parametric test:
 np.random.seed(0)
 alpha      = 0.05
-snpm       = spm1d.stats.nonparam.hotellings(y, mu)
+snpm       = spm1d.stats.nonparam.hotellings(y, mu, roi=roi)
 snpmi      = snpm.inference(alpha, iterations=100)
 print( snpmi )
 
 
 
 
 #(2) Compare with parametric result:
-spm        = spm1d.stats.hotellings(y, mu)
+spm        = spm1d.stats.hotellings(y, mu, roi=roi)
 spmi       = spm.inference(alpha)
 print( spmi )
 
 
 
 
 #(3) Plot
-plt.close('all')
-plt.figure(figsize=(10,4))
+pyplot.close('all')
+pyplot.figure(figsize=(12,4))
 
-ax0 = plt.subplot(121)
-ax1 = plt.subplot(122)
+ax0 = pyplot.subplot(121)
+ax1 = pyplot.subplot(122)
 labels = 'Parametric', 'Non-parametric'
 for ax,zi,label in zip([ax0,ax1], [spmi,snpmi], labels):
 	zi.plot(ax=ax)
 	zi.plot_threshold_label(ax=ax, fontsize=8)
 	zi.plot_p_values(ax=ax, size=10)
 	ax.set_title( label )
-plt.tight_layout()
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/1d/ex_hotellings2.py` & `spm1d-0.4.2/spm1d/examples/nonparam/1d/ex_hotellings2.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 
 #(0) Load dataset:
 dataset      = spm1d.data.mv1d.hotellings2.Besier2009muscleforces()
@@ -12,37 +12,36 @@
 
 
 
 #(1) Conduct non-parametric test:
 np.random.seed(0)
 alpha      = 0.05
 snpm       = spm1d.stats.nonparam.hotellings2(yA, yB)
-snpmi      = snpm.inference(alpha, iterations=1000)
+snpmi      = snpm.inference(alpha, iterations=100)
 print( snpmi )
 
 
 
 
 #(2) Compare with parametric result:
 spm        = spm1d.stats.hotellings2(yA, yB)
 spmi       = spm.inference(alpha)
 print( spmi )
 
 
 
 
 #(3) Plot
-plt.close('all')
-plt.figure(figsize=(10,4))
+pyplot.close('all')
+pyplot.figure(figsize=(12,4))
 
-ax0 = plt.subplot(121)
-ax1 = plt.subplot(122)
+ax0 = pyplot.subplot(121)
+ax1 = pyplot.subplot(122)
 labels = 'Parametric', 'Non-parametric'
 for ax,zi,label in zip([ax0,ax1], [spmi,snpmi], labels):
 	zi.plot(ax=ax)
 	zi.plot_threshold_label(ax=ax, fontsize=8)
 	zi.plot_p_values(ax=ax, size=10)
 	ax.set_title( label )
-plt.tight_layout()
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/1d/ex_hotellings_paired.py` & `spm1d-0.4.2/spm1d/examples/nonparam/1d/ex_hotellings_paired.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 
 #(0) Load dataset:
 # dataset      = spm1d.data.mv1d.hotellings_paired.Neptune1999kneekin()
@@ -13,37 +13,36 @@
 
 
 
 #(1) Conduct non-parametric test:
 np.random.seed(0)
 alpha      = 0.05
 snpm       = spm1d.stats.nonparam.hotellings_paired(yA, yB)
-snpmi      = snpm.inference(alpha, iterations=500)
+snpmi      = snpm.inference(alpha, iterations=100)
 print( snpmi )
 
 
 
 
 #(2) Compare with parametric result:
 spm        = spm1d.stats.hotellings_paired(yA, yB)
 spmi       = spm.inference(alpha)
 print( spmi )
 
 
 
 
 #(3) Plot
-plt.close('all')
-plt.figure(figsize=(10,4))
+pyplot.close('all')
+pyplot.figure(figsize=(12,4))
 
-ax0 = plt.subplot(121)
-ax1 = plt.subplot(122)
+ax0 = pyplot.subplot(121)
+ax1 = pyplot.subplot(122)
 labels = 'Parametric', 'Non-parametric'
 for ax,zi,label in zip([ax0,ax1], [spmi,snpmi], labels):
 	zi.plot(ax=ax)
 	zi.plot_threshold_label(ax=ax, fontsize=8)
 	zi.plot_p_values(ax=ax, size=10)
 	ax.set_title( label )
-plt.tight_layout()
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/1d/ex_manova1.py` & `spm1d-0.4.2/spm1d/examples/nonparam/1d/ex_manova1.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 #(0) Load data:
 dataset      = spm1d.data.mv1d.manova1.Dorn2012()
 y,A          = dataset.get_data()  #A:slow, B:fast
@@ -21,34 +21,33 @@
 '''
 
 
 
 #(1) Conduct non-parametric test:
 np.random.seed(0)
 X2n     = spm1d.stats.nonparam.manova1(y, A)
-X2ni    = X2n.inference(alpha=0.05, iterations=500)
+X2ni    = X2n.inference(alpha=0.05, iterations=200)
 print( 'Non-parametric test:')
 print( X2ni)
 
 
 
 #(2) Compare to parametric test:
 alpha        = 0.05
 X2           = spm1d.stats.manova1(y, A)
 X2i          = X2.inference(0.05)
 
 
 
 #(3) Plot
-plt.close('all')
-plt.figure(figsize=(10,4))
+pyplot.close('all')
+pyplot.figure(figsize=(12,4))
 
-ax0 = plt.subplot(121)
-ax1 = plt.subplot(122)
+ax0 = pyplot.subplot(121)
+ax1 = pyplot.subplot(122)
 labels = 'Parametric', 'Non-parametric'
 for ax,zi,label in zip([ax0,ax1], [X2i,X2ni], labels):
 	zi.plot(ax=ax)
 	zi.plot_threshold_label(ax=ax, fontsize=8)
 	zi.plot_p_values(ax=ax, size=10)
 	ax.set_title( label )
-plt.tight_layout()
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/1d/ex_regression.py` & `spm1d-0.4.2/spm1d/examples/nonparam/1d/ex_anova1.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,48 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 
 #(0) Load dataset:
-# dataset    = spm1d.data.uv1d.regress.SimulatedPataky2015c()
-dataset    = spm1d.data.uv1d.regress.SpeedGRF()
-y,x        = dataset.get_data()
+dataset      = spm1d.data.uv1d.anova1.SpeedGRFcategorical()
+# dataset      = spm1d.data.uv1d.anova1.Weather()
+y,A          = dataset.get_data()
+
 
 
 
 #(1) Conduct non-parametric test:
 np.random.seed(0)
 alpha      = 0.05
-two_tailed = True
-snpm       = spm1d.stats.nonparam.regress(y, x)
-snpmi      = snpm.inference(alpha, two_tailed=two_tailed, iterations=500)
+snpm       = spm1d.stats.nonparam.anova1(y, A)
+snpmi      = snpm.inference(alpha, iterations=500)
 print( snpmi )
-print( snpmi.clusters )
+
 
 
 
 #(2) Compare with parametric result:
-spm        = spm1d.stats.regress(y, x)
-spmi       = spm.inference(alpha, two_tailed=two_tailed)
+spm        = spm1d.stats.anova1(y, A, equal_var=True)
+spmi       = spm.inference(alpha)
 print( spmi )
-print( snpmi.clusters )
+
 
 
 
 #(3) Plot
-plt.close('all')
-plt.figure(figsize=(10,4))
+pyplot.close('all')
+pyplot.figure(figsize=(12,4))
 
-ax0 = plt.subplot(121)
-ax1 = plt.subplot(122)
+ax0 = pyplot.subplot(121)
+ax1 = pyplot.subplot(122)
 labels = 'Parametric', 'Non-parametric'
 for ax,zi,label in zip([ax0,ax1], [spmi,snpmi], labels):
 	zi.plot(ax=ax)
 	zi.plot_threshold_label(ax=ax, fontsize=8)
 	zi.plot_p_values(ax=ax, size=10)
 	ax.set_title( label )
-plt.tight_layout()
-plt.show()
-
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/1d/ex_ttest.py` & `spm1d-0.4.2/spm1d/examples/nonparam/1d/ex_ttest.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 
 #(0) Load dataset:
 # dataset    = spm1d.data.uv1d.t1.Random()
@@ -31,22 +31,21 @@
 spmi       = spm.inference(alpha, two_tailed=two_tailed)
 print( spmi )
 print( snpmi.clusters )
 
 
 
 #(3) Plot
-plt.close('all')
-plt.figure(figsize=(10,4))
+pyplot.close('all')
+pyplot.figure(figsize=(12,4))
 
-ax0 = plt.subplot(121)
-ax1 = plt.subplot(122)
+ax0 = pyplot.subplot(121)
+ax1 = pyplot.subplot(122)
 labels = 'Parametric', 'Non-parametric'
 for ax,zi,label in zip([ax0,ax1], [spmi,snpmi], labels):
 	zi.plot(ax=ax)
 	zi.plot_threshold_label(ax=ax, fontsize=8)
 	zi.plot_p_values(ax=ax, size=10)
 	ax.set_title( label )
-plt.tight_layout()
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/1d/ex_ttest2.py` & `spm1d-0.4.2/spm1d/examples/nonparam/1d/ex_ttest2.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 
 #(0) Load dataset:
 dataset      = spm1d.data.uv1d.t2.PlantarArchAngle()
@@ -29,22 +29,21 @@
 spmi       = spm.inference(alpha, two_tailed=two_tailed)
 print( spmi )
 print( snpmi.clusters )
 
 
 
 #(3) Plot
-plt.close('all')
-plt.figure(figsize=(10,4))
+pyplot.close('all')
+pyplot.figure(figsize=(12,4))
 
-ax0 = plt.subplot(121)
-ax1 = plt.subplot(122)
+ax0 = pyplot.subplot(121)
+ax1 = pyplot.subplot(122)
 labels = 'Parametric', 'Non-parametric'
 for ax,zi,label in zip([ax0,ax1], [spmi,snpmi], labels):
 	zi.plot(ax=ax)
 	zi.plot_threshold_label(ax=ax, fontsize=8)
 	zi.plot_p_values(ax=ax, size=10)
 	ax.set_title( label )
-plt.tight_layout()
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/1d/ex_ttest2_circular.py` & `spm1d-0.4.2/spm1d/examples/nonparam/1d/ex_cca.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,46 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
-#(0) Load a dataset containing a circular field:
-dataset  = spm1d.data.uv1d.anova1.Weather()
-Y,A      = dataset.get_data()
-yA,yB    = Y[A==0], Y[A==2]  #Atlantic and Contintental regions
+
+#(0) Load dataset:
+dataset      = spm1d.data.mv1d.cca.Dorn2012()
+y,x          = dataset.get_data()  #A:slow, B:fast
 
 
 
 #(1) Conduct non-parametric test:
 np.random.seed(0)
 alpha      = 0.05
 two_tailed = False
-circular   = True
-snpm       = spm1d.stats.nonparam.ttest2(yA, yB)
-snpmi      = snpm.inference(alpha, two_tailed=two_tailed, iterations=1000, circular=circular)
+snpm       = spm1d.stats.nonparam.cca(y, x)
+snpmi      = snpm.inference(alpha, iterations=100)
 print( snpmi )
 
 
 
-
 #(2) Compare with parametric result:
-spm        = spm1d.stats.ttest2(yA, yB)
-spmi       = spm.inference(alpha, two_tailed=two_tailed, circular=circular)
+spm        = spm1d.stats.cca(y, x)
+spmi       = spm.inference(alpha)
 print( spmi )
 
 
 
-
 #(3) Plot
-plt.close('all')
-plt.figure(figsize=(10,4))
+pyplot.close('all')
+pyplot.figure(figsize=(12,4))
 
-ax0 = plt.subplot(121)
-ax1 = plt.subplot(122)
+ax0 = pyplot.subplot(121)
+ax1 = pyplot.subplot(122)
 labels = 'Parametric', 'Non-parametric'
 for ax,zi,label in zip([ax0,ax1], [spmi,snpmi], labels):
 	zi.plot(ax=ax)
 	zi.plot_threshold_label(ax=ax, fontsize=8)
 	zi.plot_p_values(ax=ax, size=10)
 	ax.set_title( label )
-plt.tight_layout()
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/1d/ex_ttest_other_metrics.py` & `spm1d-0.4.2/spm1d/examples/nonparam/1d/ex_ttest_other_metrics.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 
 #(0) Load dataset:
 # dataset    = spm1d.data.uv1d.t1.Random()
@@ -34,22 +34,21 @@
 spmi       = spm.inference(alpha, two_tailed=two_tailed)
 print( spmi )
 print( spmi.clusters )
 
 
 
 #(3) Plot
-plt.close('all')
-plt.figure(figsize=(10,4))
+pyplot.close('all')
+pyplot.figure(figsize=(12,4))
 
-ax0 = plt.subplot(121)
-ax1 = plt.subplot(122)
+ax0 = pyplot.subplot(121)
+ax1 = pyplot.subplot(122)
 labels = 'Parametric', 'Non-parametric'
 for ax,zi,label in zip([ax0,ax1], [spmi,snpmi], labels):
 	zi.plot(ax=ax)
 	zi.plot_threshold_label(ax=ax, fontsize=8)
 	zi.plot_p_values(ax=ax, size=10)
 	ax.set_title( label )
-plt.tight_layout()
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/1d/ex_ttest_paired.py` & `spm1d-0.4.2/spm1d/examples/nonparam/1d/roi/ex_ttest2.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,54 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 
 #(0) Load dataset:
 dataset      = spm1d.data.uv1d.t2.PlantarArchAngle()
-yA,yB        = dataset.get_data()  #normal and fast walking
+# dataset      = spm1d.data.uv1d.t2.SimulatedTwoLocalMax()
+yB,yA        = dataset.get_data()  #normal and fast walking
+
+
+#(0a) Create region of interest(ROI):
+roi        = np.array( [False]*yA.shape[1] )
+roi[70:80] = True
 
 
 
 #(1) Conduct non-parametric test:
 np.random.seed(0)
 alpha      = 0.05
-two_tailed = False
-snpm       = spm1d.stats.nonparam.ttest_paired(yA, yB)
-snpmi      = snpm.inference(alpha, two_tailed=two_tailed, iterations=-1)
+two_tailed = True
+snpm       = spm1d.stats.nonparam.ttest2(yA, yB, roi=roi)
+snpmi      = snpm.inference(alpha, two_tailed=two_tailed, iterations=500)
 print( snpmi )
-print( snpmi.clusters )
+
 
 
 
 #(2) Compare with parametric result:
-spm        = spm1d.stats.ttest_paired(yA, yB)
+spm        = spm1d.stats.ttest2(yA, yB, roi=roi)
 spmi       = spm.inference(alpha, two_tailed=two_tailed)
 print( spmi )
-print( spmi.clusters )
+
 
 
 
 #(3) Plot
-plt.close('all')
-plt.figure(figsize=(10,4))
+pyplot.close('all')
+pyplot.figure(figsize=(12,4))
 
-ax0 = plt.subplot(121)
-ax1 = plt.subplot(122)
+ax0 = pyplot.subplot(121)
+ax1 = pyplot.subplot(122)
 labels = 'Parametric', 'Non-parametric'
 for ax,zi,label in zip([ax0,ax1], [spmi,snpmi], labels):
 	zi.plot(ax=ax)
 	zi.plot_threshold_label(ax=ax, fontsize=8)
 	zi.plot_p_values(ax=ax, size=10)
 	ax.set_title( label )
-plt.tight_layout()
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/1d/roi/ex_anova1.py` & `spm1d-0.4.2/spm1d/examples/nonparam/1d/roi/ex_anova1rm.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,51 +1,50 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 
 #(0) Load dataset:
-dataset    = spm1d.data.uv1d.anova1.SpeedGRFcategorical()
-# dataset    = spm1d.data.uv1d.anova1.Weather()
-y,A        = dataset.get_data()
+dataset      = spm1d.data.uv1d.anova1rm.SpeedGRFcategoricalRM()
+y,A,SUBJ     = dataset.get_data()
 
 #(0a) Create region of interest(ROI):
 roi        = np.array( [False]*y.shape[1] )
-roi[15:75] = True
+roi[25:45] = True
 
 
 #(1) Conduct non-parametric test:
 np.random.seed(0)
 alpha      = 0.05
-snpm       = spm1d.stats.nonparam.anova1(y, A, roi=roi)
-snpmi      = snpm.inference(alpha, iterations=200)
+snpm       = spm1d.stats.nonparam.anova1rm(y, A, SUBJ, roi=roi)
+snpmi      = snpm.inference(alpha, iterations=500)
 print( snpmi )
 
 
 
 
 #(2) Compare with parametric result:
-spm        = spm1d.stats.anova1(y, A, equal_var=True, roi=roi)
+spm        = spm1d.stats.anova1rm(y, A, SUBJ, equal_var=True, roi=roi)
 spmi       = spm.inference(alpha)
 print( spmi )
 
 
 
 
 #(3) Plot
-plt.close('all')
-plt.figure(figsize=(10,4))
+pyplot.close('all')
+pyplot.figure(figsize=(12,4))
 
-ax0 = plt.subplot(121)
-ax1 = plt.subplot(122)
+ax0 = pyplot.subplot(121)
+ax1 = pyplot.subplot(122)
 labels = 'Parametric', 'Non-parametric'
 for ax,zi,label in zip([ax0,ax1], [spmi,snpmi], labels):
 	zi.plot(ax=ax)
 	zi.plot_threshold_label(ax=ax, fontsize=8)
 	zi.plot_p_values(ax=ax, size=10)
 	ax.set_title( label )
-plt.tight_layout()
-plt.show()
+pyplot.show()
+
```

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/1d/roi/ex_anova1rm.py` & `spm1d-0.4.2/spm1d/examples/nonparam/1d/roi/ex_hotellings_paired.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,53 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 
 #(0) Load dataset:
-dataset      = spm1d.data.uv1d.anova1rm.SpeedGRFcategoricalRM()
-y,A,SUBJ     = dataset.get_data()
+# dataset      = spm1d.data.mv1d.hotellings_paired.Neptune1999kneekin()
+dataset      = spm1d.data.mv1d.hotellings_paired.Pataky2014cop()
+yA,yB        = dataset.get_data()  #A:slow, B:fast
+
 
 #(0a) Create region of interest(ROI):
-roi        = np.array( [False]*y.shape[1] )
-roi[25:45] = True
+roi        = np.array( [False]*yA.shape[1] )
+roi[70:80] = True
+
 
 
 #(1) Conduct non-parametric test:
 np.random.seed(0)
 alpha      = 0.05
-snpm       = spm1d.stats.nonparam.anova1rm(y, A, SUBJ, roi=roi)
-snpmi      = snpm.inference(alpha, iterations=500)
+snpm       = spm1d.stats.nonparam.hotellings_paired(yA, yB, roi=roi)
+snpmi      = snpm.inference(alpha, iterations=100)
 print( snpmi )
 
 
 
 
 #(2) Compare with parametric result:
-spm        = spm1d.stats.anova1rm(y, A, SUBJ, equal_var=True, roi=roi)
+spm        = spm1d.stats.hotellings_paired(yA, yB, roi=roi)
 spmi       = spm.inference(alpha)
 print( spmi )
 
 
 
 
 #(3) Plot
-plt.close('all')
-plt.figure(figsize=(10,4))
+pyplot.close('all')
+pyplot.figure(figsize=(12,4))
 
-ax0 = plt.subplot(121)
-ax1 = plt.subplot(122)
+ax0 = pyplot.subplot(121)
+ax1 = pyplot.subplot(122)
 labels = 'Parametric', 'Non-parametric'
 for ax,zi,label in zip([ax0,ax1], [spmi,snpmi], labels):
 	zi.plot(ax=ax)
 	zi.plot_threshold_label(ax=ax, fontsize=8)
 	zi.plot_p_values(ax=ax, size=10)
 	ax.set_title( label )
-plt.tight_layout()
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/1d/roi/ex_anova2.py` & `spm1d-0.4.2/spm1d/examples/nonparam/1d/roi/ex_anova2.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 
 #(0) Load dataset:
 dataset      = spm1d.data.uv1d.anova2.SPM1D_ANOVA2_2x2()
@@ -34,27 +34,26 @@
 FF         = spm1d.stats.anova2(y, A, B, equal_var=True, roi=roi)
 FFi        = FF.inference(alpha)
 print( FFi )
 
 
 
 #(3) Plot
-plt.close('all')
-plt.figure(figsize=(12,4))
+pyplot.close('all')
+pyplot.figure(figsize=(15,4))
 
 for i,(Fi,Fni) in enumerate( zip(FFi,FFni) ):
-	ax = plt.subplot(1,3,i+1)
+	ax = pyplot.subplot(1,3,i+1)
 	Fni.plot(ax=ax)
 	Fni.plot_threshold_label(ax=ax, fontsize=8)
 	Fni.plot_p_values(ax=ax, size=10)
 	ax.axhline( Fi.zstar, color='orange', linestyle='--', label='Parametric threshold')
 	if (Fi.zstar > Fi.z.max()) and (Fi.zstar>Fni.zstar):
 		ax.set_ylim(0, Fi.zstar+1)
 	if i==0:
 		ax.legend(fontsize=10, loc='best')
 	ax.set_title( Fni.effect )
-plt.tight_layout()
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/1d/roi/ex_anova2nested.py` & `spm1d-0.4.2/spm1d/examples/nonparam/1d/roi/ex_anova2nested.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 
 #(0) Load dataset:
 dataset      = spm1d.data.uv1d.anova2nested.SPM1D_ANOVA2NESTED_2x2()
@@ -35,27 +35,26 @@
 FF         = spm1d.stats.anova2nested(y, A, B, equal_var=True, roi=roi)
 FFi        = FF.inference(alpha)
 print( FFi )
 
 
 
 #(3) Plot
-plt.close('all')
-plt.figure(figsize=(12,4))
+pyplot.close('all')
+pyplot.figure(figsize=(15,4))
 
 for i,(Fi,Fni) in enumerate( zip(FFi,FFni) ):
-	ax = plt.subplot(1,3,i+1)
+	ax = pyplot.subplot(1,3,i+1)
 	Fni.plot(ax=ax)
 	Fni.plot_threshold_label(ax=ax, fontsize=8)
 	Fni.plot_p_values(ax=ax, size=10)
 	ax.axhline( Fi.zstar, color='orange', linestyle='--', label='Parametric threshold')
 	if (Fi.zstar > Fi.z.max()) and (Fi.zstar>Fni.zstar):
 		ax.set_ylim(0, Fi.zstar+1)
 	if i==0:
 		ax.legend(fontsize=10, loc='best')
 	ax.set_title( Fni.effect )
-plt.tight_layout()
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/1d/roi/ex_anova2onerm.py` & `spm1d-0.4.2/spm1d/examples/nonparam/1d/roi/ex_anova2onerm.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 
 #(0) Load dataset:
 dataset      = spm1d.data.uv1d.anova2onerm.SPM1D_ANOVA2ONERM_2x2()
@@ -36,27 +36,26 @@
 FF         = spm1d.stats.anova2onerm(y, A, B, SUBJ, equal_var=True, roi=roi)
 FFi        = FF.inference(alpha)
 print( FFi )
 
 
 
 #(3) Plot
-plt.close('all')
-plt.figure(figsize=(12,3))
+pyplot.close('all')
+pyplot.figure(figsize=(15,4))
 
 for i,(Fi,Fni) in enumerate( zip(FFi,FFni) ):
-	ax = plt.subplot(1,3,i+1)
+	ax = pyplot.subplot(1,3,i+1)
 	Fni.plot(ax=ax)
 	Fni.plot_threshold_label(ax=ax, fontsize=8)
 	Fni.plot_p_values(ax=ax, size=10)
 	ax.axhline( Fi.zstar, color='orange', linestyle='--', label='Parametric threshold')
 	if (Fi.zstar > Fi.z.max()) and (Fi.zstar>Fni.zstar):
 		ax.set_ylim(0, Fi.zstar+1)
 	if i==0:
 		ax.legend(fontsize=10, loc='best')
 	ax.set_title( Fni.effect )
-plt.tight_layout()
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/1d/roi/ex_anova3.py` & `spm1d-0.4.2/spm1d/examples/nonparam/1d/ex_anova3tworm.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,55 +1,51 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 
 #(0) Load dataset:
-dataset      = spm1d.data.uv1d.anova3.SPM1D_ANOVA3_2x2x2()
-# dataset      = spm1d.data.uv1d.anova3.SPM1D_ANOVA3_2x3x4()
-y,A,B,C      = dataset.get_data()
-
-#(0a) Create region of interest(ROI):
-roi        = np.array( [False]*y.shape[1] )
-roi[25:45] = True
+dataset      = spm1d.data.uv1d.anova3tworm.SPM1D_ANOVA3TWORM_2x2x2()
+# dataset      = spm1d.data.uv1d.anova3tworm.SPM1D_ANOVA3TWORM_2x3x4()
+y,A,B,C,SUBJ = dataset.get_data()
+
 
 
 #(1) Conduct non-parametric test:
 np.random.seed(0)
 alpha      = 0.05
-FFn        = spm1d.stats.nonparam.anova3(y, A, B, C, roi=roi)
+FFn        = spm1d.stats.nonparam.anova3tworm(y, A, B, C, SUBJ)
 FFni       = FFn.inference(alpha, iterations=200)
 print( FFni )
 
 
 
 #(2) Compare with parametric result:
-FF         = spm1d.stats.anova3(y, A, B, C, equal_var=True, roi=roi)
+FF         = spm1d.stats.anova3tworm(y, A, B, C, SUBJ, equal_var=True)
 FFi        = FF.inference(alpha)
 print( FFi )
 
 
 
 #(3) Plot
-plt.close('all')
-plt.figure(figsize=(12,8))
+pyplot.close('all')
+pyplot.figure(figsize=(15,10))
 
 for i,(Fi,Fni) in enumerate( zip(FFi,FFni) ):
-	ax = plt.subplot(3,3,i+1)
+	ax = pyplot.subplot(3,3,i+1)
 	Fni.plot(ax=ax)
 	Fni.plot_threshold_label(ax=ax, fontsize=8)
 	Fni.plot_p_values(ax=ax, size=10)
 	ax.axhline( Fi.zstar, color='orange', linestyle='--', label='Parametric threshold')
 	if (Fi.zstar > Fi.z.max()) and (Fi.zstar>Fni.zstar):
 		ax.set_ylim(0, Fi.zstar+1)
 	if i==0:
 		ax.legend(fontsize=10, loc='best')
 	ax.set_title( Fni.effect )
-plt.tight_layout()
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/1d/roi/ex_anova3nested.py` & `spm1d-0.4.2/spm1d/examples/nonparam/1d/roi/ex_anova3nested.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 
 #(0) Load dataset:
 dataset      = spm1d.data.uv1d.anova3nested.SPM1D_ANOVA3NESTED_2x2x2()
@@ -29,27 +29,26 @@
 FF         = spm1d.stats.anova3nested(y, A, B, C, equal_var=True, roi=roi)
 FFi        = FF.inference(alpha)
 print( FFi )
 
 
 
 #(3) Plot
-plt.close('all')
-plt.figure(figsize=(12,8))
+pyplot.close('all')
+pyplot.figure(figsize=(15,8))
 
 for i,(Fi,Fni) in enumerate( zip(FFi,FFni) ):
-	ax = plt.subplot(3,3,i+1)
+	ax = pyplot.subplot(3,3,i+1)
 	Fni.plot(ax=ax)
 	Fni.plot_threshold_label(ax=ax, fontsize=8)
 	Fni.plot_p_values(ax=ax, size=10)
 	ax.axhline( Fi.zstar, color='orange', linestyle='--', label='Parametric threshold')
 	if (Fi.zstar > Fi.z.max()) and (Fi.zstar>Fni.zstar):
 		ax.set_ylim(0, Fi.zstar+1)
 	if i==0:
 		ax.legend(fontsize=10, loc='best')
 	ax.set_title( Fni.effect )
-plt.tight_layout()
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/1d/roi/ex_anova3onerm.py` & `spm1d-0.4.2/spm1d/examples/nonparam/1d/roi/ex_anova3tworm.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,55 +1,54 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 
 #(0) Load dataset:
-dataset      = spm1d.data.uv1d.anova3onerm.SPM1D_ANOVA3ONERM_2x2x2()
-# dataset      = spm1d.data.uv1d.anova3onerm.SPM1D_ANOVA3ONERM_2x3x4()
+dataset      = spm1d.data.uv1d.anova3tworm.SPM1D_ANOVA3TWORM_2x2x2()
+# dataset      = spm1d.data.uv1d.anova3tworm.SPM1D_ANOVA3TWORM_2x3x4()
 y,A,B,C,SUBJ = dataset.get_data()
 
 #(0a) Create region of interest(ROI):
 roi        = np.array( [False]*y.shape[1] )
 roi[25:45] = True
 
 
 #(1) Conduct non-parametric test:
 np.random.seed(0)
 alpha      = 0.05
-FFn        = spm1d.stats.nonparam.anova3onerm(y, A, B, C, SUBJ, roi=roi)
+FFn        = spm1d.stats.nonparam.anova3tworm(y, A, B, C, SUBJ, roi=roi)
 FFni       = FFn.inference(alpha, iterations=200)
 print( FFni )
 
 
 
 #(2) Compare with parametric result:
-FF         = spm1d.stats.anova3onerm(y, A, B, C, SUBJ, equal_var=True, roi=roi)
+FF         = spm1d.stats.anova3tworm(y, A, B, C, SUBJ, equal_var=True, roi=roi)
 FFi        = FF.inference(alpha)
 print( FFi )
 
 
 
 #(3) Plot
-plt.close('all')
-plt.figure(figsize=(12,8))
+pyplot.close('all')
+pyplot.figure(figsize=(15,8))
 
 for i,(Fi,Fni) in enumerate( zip(FFi,FFni) ):
-	ax = plt.subplot(3,3,i+1)
+	ax = pyplot.subplot(3,3,i+1)
 	Fni.plot(ax=ax)
 	Fni.plot_threshold_label(ax=ax, fontsize=8)
 	Fni.plot_p_values(ax=ax, size=10)
 	ax.axhline( Fi.zstar, color='orange', linestyle='--', label='Parametric threshold')
 	if (Fi.zstar > Fi.z.max()) and (Fi.zstar>Fni.zstar):
 		ax.set_ylim(0, Fi.zstar+1)
 	if i==0:
 		ax.legend(fontsize=10, loc='best')
 	ax.set_title( Fni.effect )
-plt.tight_layout()
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/1d/roi/ex_anova3rm.py` & `spm1d-0.4.2/spm1d/examples/nonparam/1d/ex_anova3nested.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,55 +1,58 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 
 #(0) Load dataset:
-dataset      = spm1d.data.uv1d.anova3rm.SPM1D_ANOVA3RM_2x2x2()
-# dataset      = spm1d.data.uv1d.anova3rm.SPM1D_ANOVA3RM_2x3x4()
-y,A,B,C,SUBJ = dataset.get_data()
-
-#(0a) Create region of interest(ROI):
-roi        = np.array( [False]*y.shape[1] )
-roi[25:45] = True
+# dataset      = spm1d.data.uv1d.anova3nested.SPM1D_ANOVA3NESTED_2x2x2()
+dataset      = spm1d.data.uv1d.anova3nested.SPM1D_ANOVA3NESTED_2x4x2()
+y,A,B,C      = dataset.get_data()
 
 
 #(1) Conduct non-parametric test:
 np.random.seed(0)
 alpha      = 0.05
-FFn        = spm1d.stats.nonparam.anova3rm(y, A, B, C, SUBJ, roi=roi)
+FFn        = spm1d.stats.nonparam.anova3nested(y, A, B, C)
 FFni       = FFn.inference(alpha, iterations=200)
 print( FFni )
 
 
 
 #(2) Compare with parametric result:
-FF         = spm1d.stats.anova3rm(y, A, B, C, SUBJ, equal_var=True, roi=roi)
+FF         = spm1d.stats.anova3nested(y, A, B, C, equal_var=True)
 FFi        = FF.inference(alpha)
 print( FFi )
 
 
 
 #(3) Plot
-plt.close('all')
-plt.figure(figsize=(12,8))
+pyplot.close('all')
+pyplot.figure(figsize=(15,10))
 
 for i,(Fi,Fni) in enumerate( zip(FFi,FFni) ):
-	ax = plt.subplot(3,3,i+1)
+	ax = pyplot.subplot(3,3,i+1)
 	Fni.plot(ax=ax)
 	Fni.plot_threshold_label(ax=ax, fontsize=8)
 	Fni.plot_p_values(ax=ax, size=10)
 	ax.axhline( Fi.zstar, color='orange', linestyle='--', label='Parametric threshold')
 	if (Fi.zstar > Fi.z.max()) and (Fi.zstar>Fni.zstar):
 		ax.set_ylim(0, Fi.zstar+1)
 	if i==0:
 		ax.legend(fontsize=10, loc='best')
 	ax.set_title( Fni.effect )
-plt.tight_layout()
-plt.show()
-
+pyplot.show()
 
 
 
+#(3) Plot results:
+pyplot.close('all')
+FFni.plot(plot_threshold_label=False, plot_p_values=True, autoset_ylim=True)
+### optionally plot parametric thresholds for comparison:
+for i,Fi in enumerate(FFi):
+	ax = pyplot.subplot(3,3,i+1)
+	ax.axhline( Fi.zstar, color='c', linestyle='--' )
+	ax.text(2, Fi.zstar, 'Parametric', color='c')
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/1d/roi/ex_anova3tworm.py` & `spm1d-0.4.2/spm1d/examples/nonparam/1d/ex_anova3rm.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,51 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 
 #(0) Load dataset:
-dataset      = spm1d.data.uv1d.anova3tworm.SPM1D_ANOVA3TWORM_2x2x2()
-# dataset      = spm1d.data.uv1d.anova3tworm.SPM1D_ANOVA3TWORM_2x3x4()
+dataset      = spm1d.data.uv1d.anova3rm.SPM1D_ANOVA3RM_2x2x2()
+# dataset      = spm1d.data.uv1d.anova3rm.SPM1D_ANOVA3RM_2x3x4()
 y,A,B,C,SUBJ = dataset.get_data()
 
-#(0a) Create region of interest(ROI):
-roi        = np.array( [False]*y.shape[1] )
-roi[25:45] = True
 
 
 #(1) Conduct non-parametric test:
 np.random.seed(0)
 alpha      = 0.05
-FFn        = spm1d.stats.nonparam.anova3tworm(y, A, B, C, SUBJ, roi=roi)
+FFn        = spm1d.stats.nonparam.anova3rm(y, A, B, C, SUBJ)
 FFni       = FFn.inference(alpha, iterations=200)
 print( FFni )
 
 
 
 #(2) Compare with parametric result:
-FF         = spm1d.stats.anova3tworm(y, A, B, C, SUBJ, equal_var=True, roi=roi)
+FF         = spm1d.stats.anova3rm(y, A, B, C, SUBJ, equal_var=True)
 FFi        = FF.inference(alpha)
 print( FFi )
 
 
 
 #(3) Plot
-plt.close('all')
-plt.figure(figsize=(12,8))
+pyplot.close('all')
+pyplot.figure(figsize=(15,10))
 
 for i,(Fi,Fni) in enumerate( zip(FFi,FFni) ):
-	ax = plt.subplot(3,3,i+1)
+	ax = pyplot.subplot(3,3,i+1)
 	Fni.plot(ax=ax)
 	Fni.plot_threshold_label(ax=ax, fontsize=8)
 	Fni.plot_p_values(ax=ax, size=10)
 	ax.axhline( Fi.zstar, color='orange', linestyle='--', label='Parametric threshold')
 	if (Fi.zstar > Fi.z.max()) and (Fi.zstar>Fni.zstar):
 		ax.set_ylim(0, Fi.zstar+1)
 	if i==0:
 		ax.legend(fontsize=10, loc='best')
 	ax.set_title( Fni.effect )
-plt.tight_layout()
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/1d/roi/ex_cca.py` & `spm1d-0.4.2/spm1d/examples/nonparam/1d/roi/ex_hotellings2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,53 +1,50 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 
 #(0) Load dataset:
-dataset      = spm1d.data.mv1d.cca.Dorn2012()
-y,x          = dataset.get_data()  #A:slow, B:fast
-
+dataset      = spm1d.data.mv1d.hotellings2.Besier2009muscleforces()
+yA,yB        = dataset.get_data()  #A:slow, B:fast
 
 #(0a) Create region of interest(ROI):
-roi        = np.array( [False]*y.shape[1] )
-roi[50:80] = True
+roi        = np.array( [False]*yA.shape[1] )
+roi[70:80] = True
 
 
 #(1) Conduct non-parametric test:
 np.random.seed(0)
 alpha      = 0.05
-two_tailed = False
-snpm       = spm1d.stats.nonparam.cca(y, x, roi=roi)
+snpm       = spm1d.stats.nonparam.hotellings2(yA, yB, roi=roi)
 snpmi      = snpm.inference(alpha, iterations=100)
 print( snpmi )
 
 
 
 
 #(2) Compare with parametric result:
-spm        = spm1d.stats.cca(y, x, roi=roi)
+spm        = spm1d.stats.hotellings2(yA, yB, roi=roi)
 spmi       = spm.inference(alpha)
 print( spmi )
 
 
 
 
 #(3) Plot
-plt.close('all')
-plt.figure(figsize=(12,4))
+pyplot.close('all')
+pyplot.figure(figsize=(12,4))
 
-ax0 = plt.subplot(121)
-ax1 = plt.subplot(122)
+ax0 = pyplot.subplot(121)
+ax1 = pyplot.subplot(122)
 labels = 'Parametric', 'Non-parametric'
 for ax,zi,label in zip([ax0,ax1], [spmi,snpmi], labels):
 	zi.plot(ax=ax)
 	zi.plot_threshold_label(ax=ax, fontsize=8)
 	zi.plot_p_values(ax=ax, size=10)
 	ax.set_title( label )
-plt.tight_layout()
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/1d/roi/ex_hotellings2.py` & `spm1d-0.4.2/spm1d/examples/nonparam/1d/roi/ex_ttest_paired.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 
 #(0) Load dataset:
-dataset      = spm1d.data.mv1d.hotellings2.Besier2009muscleforces()
-yA,yB        = dataset.get_data()  #A:slow, B:fast
+dataset      = spm1d.data.uv1d.t2.PlantarArchAngle()
+yA,yB        = dataset.get_data()  #normal and fast walking
 
 #(0a) Create region of interest(ROI):
 roi        = np.array( [False]*yA.shape[1] )
 roi[70:80] = True
 
 
 #(1) Conduct non-parametric test:
 np.random.seed(0)
 alpha      = 0.05
-snpm       = spm1d.stats.nonparam.hotellings2(yA, yB, roi=roi)
-snpmi      = snpm.inference(alpha, iterations=100)
+two_tailed = False
+snpm       = spm1d.stats.nonparam.ttest_paired(yA, yB, roi=roi)
+snpmi      = snpm.inference(alpha, two_tailed=two_tailed, iterations=-1)
 print( snpmi )
 
 
 
 
 #(2) Compare with parametric result:
-spm        = spm1d.stats.hotellings2(yA, yB, roi=roi)
-spmi       = spm.inference(alpha)
+spm        = spm1d.stats.ttest_paired(yA, yB, roi=roi)
+spmi       = spm.inference(alpha, two_tailed=two_tailed)
 print( spmi )
 
 
 
 
 #(3) Plot
-plt.close('all')
-plt.figure(figsize=(12,4))
+pyplot.close('all')
+pyplot.figure(figsize=(12,4))
 
-ax0 = plt.subplot(121)
-ax1 = plt.subplot(122)
+ax0 = pyplot.subplot(121)
+ax1 = pyplot.subplot(122)
 labels = 'Parametric', 'Non-parametric'
 for ax,zi,label in zip([ax0,ax1], [spmi,snpmi], labels):
 	zi.plot(ax=ax)
 	zi.plot_threshold_label(ax=ax, fontsize=8)
 	zi.plot_p_values(ax=ax, size=10)
 	ax.set_title( label )
-plt.tight_layout()
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/1d/roi/ex_hotellings_paired.py` & `spm1d-0.4.2/spm1d/examples/nonparam/1d/ex_ttest_paired.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,54 +1,48 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 
 #(0) Load dataset:
-# dataset      = spm1d.data.mv1d.hotellings_paired.Neptune1999kneekin()
-dataset      = spm1d.data.mv1d.hotellings_paired.Pataky2014cop()
-yA,yB        = dataset.get_data()  #A:slow, B:fast
-
-
-#(0a) Create region of interest(ROI):
-roi        = np.array( [False]*yA.shape[1] )
-roi[70:80] = True
+dataset      = spm1d.data.uv1d.t2.PlantarArchAngle()
+yA,yB        = dataset.get_data()  #normal and fast walking
 
 
 
 #(1) Conduct non-parametric test:
 np.random.seed(0)
 alpha      = 0.05
-snpm       = spm1d.stats.nonparam.hotellings_paired(yA, yB, roi=roi)
-snpmi      = snpm.inference(alpha, iterations=100)
+two_tailed = False
+snpm       = spm1d.stats.nonparam.ttest_paired(yA, yB)
+snpmi      = snpm.inference(alpha, two_tailed=two_tailed, iterations=-1)
 print( snpmi )
-
+print( snpmi.clusters )
 
 
 
 #(2) Compare with parametric result:
-spm        = spm1d.stats.hotellings_paired(yA, yB, roi=roi)
-spmi       = spm.inference(alpha)
+spm        = spm1d.stats.ttest_paired(yA, yB)
+spmi       = spm.inference(alpha, two_tailed=two_tailed)
 print( spmi )
-
+print( spmi.clusters )
 
 
 
 #(3) Plot
-plt.close('all')
-plt.figure(figsize=(12,4))
+pyplot.close('all')
+pyplot.figure(figsize=(12,4))
 
-ax0 = plt.subplot(121)
-ax1 = plt.subplot(122)
+ax0 = pyplot.subplot(121)
+ax1 = pyplot.subplot(122)
 labels = 'Parametric', 'Non-parametric'
 for ax,zi,label in zip([ax0,ax1], [spmi,snpmi], labels):
 	zi.plot(ax=ax)
 	zi.plot_threshold_label(ax=ax, fontsize=8)
 	zi.plot_p_values(ax=ax, size=10)
 	ax.set_title( label )
-plt.tight_layout()
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/1d/roi/ex_manova1.py` & `spm1d-0.4.2/spm1d/examples/nonparam/1d/roi/ex_manova1.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 #(0) Load data:
 dataset      = spm1d.data.mv1d.manova1.Dorn2012()
 y,A          = dataset.get_data()  #A:slow, B:fast
@@ -40,20 +40,19 @@
 alpha        = 0.05
 X2           = spm1d.stats.manova1(y, A, roi=roi)
 X2i          = X2.inference(0.05)
 
 
 
 #(3) Plot
-plt.close('all')
-plt.figure(figsize=(12,4))
+pyplot.close('all')
+pyplot.figure(figsize=(12,4))
 
-ax0 = plt.subplot(121)
-ax1 = plt.subplot(122)
+ax0 = pyplot.subplot(121)
+ax1 = pyplot.subplot(122)
 labels = 'Parametric', 'Non-parametric'
 for ax,zi,label in zip([ax0,ax1], [X2i,X2ni], labels):
 	zi.plot(ax=ax)
 	zi.plot_threshold_label(ax=ax, fontsize=8)
 	zi.plot_p_values(ax=ax, size=10)
 	ax.set_title( label )
-plt.tight_layout()
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/1d/roi/ex_regression.py` & `spm1d-0.4.2/spm1d/examples/nonparam/1d/roi/ex_ttest.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,53 +1,56 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 
 #(0) Load dataset:
-dataset    = spm1d.data.uv1d.regress.SimulatedPataky2015c()
-dataset    = spm1d.data.uv1d.regress.SpeedGRF()
-y,x        = dataset.get_data()
+# dataset    = spm1d.data.uv1d.t1.Random()
+# dataset    = spm1d.data.uv1d.t1.SimulatedPataky2015a()
+dataset    = spm1d.data.uv1d.t1.SimulatedPataky2015b()
+y,mu       = dataset.get_data()
+
+
 
 #(0a) Create region of interest(ROI):
 roi        = np.array( [False]*y.shape[1] )
 roi[70:80] = True
 
 
+
 #(1) Conduct non-parametric test:
 np.random.seed(0)
 alpha      = 0.05
 two_tailed = False
-snpm       = spm1d.stats.nonparam.regress(y, x, roi=roi)
-snpmi      = snpm.inference(alpha, two_tailed=two_tailed, iterations=500)
+snpm       = spm1d.stats.nonparam.ttest(y, mu, roi=roi)
+snpmi      = snpm.inference(alpha, two_tailed=two_tailed, iterations=-1)
 print( snpmi )
 
 
 
 
 #(2) Compare with parametric result:
-spm        = spm1d.stats.regress(y, x, roi=roi)
+spm        = spm1d.stats.ttest(y, mu, roi=roi)
 spmi       = spm.inference(alpha, two_tailed=two_tailed)
 print( spmi )
 
 
 
 
 #(3) Plot
-plt.close('all')
-plt.figure(figsize=(12,4))
+pyplot.close('all')
+pyplot.figure(figsize=(12,4))
 
-ax0 = plt.subplot(121)
-ax1 = plt.subplot(122)
+ax0 = pyplot.subplot(121)
+ax1 = pyplot.subplot(122)
 labels = 'Parametric', 'Non-parametric'
 for ax,zi,label in zip([ax0,ax1], [spmi,snpmi], labels):
 	zi.plot(ax=ax)
 	zi.plot_threshold_label(ax=ax, fontsize=8)
 	zi.plot_p_values(ax=ax, size=10)
 	ax.set_title( label )
-plt.tight_layout()
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/1d/roi/ex_ttest.py` & `spm1d-0.4.2/spm1d/examples/nonparam/1d/ex_ttest2_circular.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,49 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
-
-#(0) Load dataset:
-# dataset    = spm1d.data.uv1d.t1.Random()
-# dataset    = spm1d.data.uv1d.t1.SimulatedPataky2015a()
-dataset    = spm1d.data.uv1d.t1.SimulatedPataky2015b()
-y,mu       = dataset.get_data()
-
-
-
-#(0a) Create region of interest(ROI):
-roi        = np.array( [False]*y.shape[1] )
-roi[70:80] = True
+#(0) Load a dataset containing a circular field:
+dataset  = spm1d.data.uv1d.anova1.Weather()
+Y,A      = dataset.get_data()
+yA,yB    = Y[A==0], Y[A==2]  #Atlantic and Contintental regions
 
 
 
 #(1) Conduct non-parametric test:
 np.random.seed(0)
 alpha      = 0.05
 two_tailed = False
-snpm       = spm1d.stats.nonparam.ttest(y, mu, roi=roi)
-snpmi      = snpm.inference(alpha, two_tailed=two_tailed, iterations=-1)
+circular   = True
+snpm       = spm1d.stats.nonparam.ttest2(yA, yB)
+snpmi      = snpm.inference(alpha, two_tailed=two_tailed, iterations=1000, circular=circular)
 print( snpmi )
 
 
 
 
 #(2) Compare with parametric result:
-spm        = spm1d.stats.ttest(y, mu, roi=roi)
-spmi       = spm.inference(alpha, two_tailed=two_tailed)
+spm        = spm1d.stats.ttest2(yA, yB)
+spmi       = spm.inference(alpha, two_tailed=two_tailed, circular=circular)
 print( spmi )
 
 
 
 
 #(3) Plot
-plt.close('all')
-plt.figure(figsize=(12,4))
+pyplot.close('all')
+pyplot.figure(figsize=(12,4))
 
-ax0 = plt.subplot(121)
-ax1 = plt.subplot(122)
+ax0 = pyplot.subplot(121)
+ax1 = pyplot.subplot(122)
 labels = 'Parametric', 'Non-parametric'
 for ax,zi,label in zip([ax0,ax1], [spmi,snpmi], labels):
 	zi.plot(ax=ax)
 	zi.plot_threshold_label(ax=ax, fontsize=8)
 	zi.plot_p_values(ax=ax, size=10)
 	ax.set_title( label )
-plt.tight_layout()
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/nonparam/1d/roi/ex_ttest_paired.py` & `spm1d-0.4.2/spm1d/examples/nonparam/1d/roi/ex_cca.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 
 #(0) Load dataset:
-dataset      = spm1d.data.uv1d.t2.PlantarArchAngle()
-yA,yB        = dataset.get_data()  #normal and fast walking
+dataset      = spm1d.data.mv1d.cca.Dorn2012()
+y,x          = dataset.get_data()  #A:slow, B:fast
+
 
 #(0a) Create region of interest(ROI):
-roi        = np.array( [False]*yA.shape[1] )
-roi[70:80] = True
+roi        = np.array( [False]*y.shape[1] )
+roi[50:80] = True
 
 
 #(1) Conduct non-parametric test:
 np.random.seed(0)
 alpha      = 0.05
 two_tailed = False
-snpm       = spm1d.stats.nonparam.ttest_paired(yA, yB, roi=roi)
-snpmi      = snpm.inference(alpha, two_tailed=two_tailed, iterations=-1)
+snpm       = spm1d.stats.nonparam.cca(y, x, roi=roi)
+snpmi      = snpm.inference(alpha, iterations=100)
 print( snpmi )
 
 
 
 
 #(2) Compare with parametric result:
-spm        = spm1d.stats.ttest_paired(yA, yB, roi=roi)
-spmi       = spm.inference(alpha, two_tailed=two_tailed)
+spm        = spm1d.stats.cca(y, x, roi=roi)
+spmi       = spm.inference(alpha)
 print( spmi )
 
 
 
 
 #(3) Plot
-plt.close('all')
-plt.figure(figsize=(12,4))
+pyplot.close('all')
+pyplot.figure(figsize=(12,4))
 
-ax0 = plt.subplot(121)
-ax1 = plt.subplot(122)
+ax0 = pyplot.subplot(121)
+ax1 = pyplot.subplot(122)
 labels = 'Parametric', 'Non-parametric'
 for ax,zi,label in zip([ax0,ax1], [spmi,snpmi], labels):
 	zi.plot(ax=ax)
 	zi.plot_threshold_label(ax=ax, fontsize=8)
 	zi.plot_p_values(ax=ax, size=10)
 	ax.set_title( label )
-plt.tight_layout()
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/normality/0d/ex_ttest.py` & `spm1d-0.4.2/spm1d/examples/normality/0d/ex_ttest.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/examples/normality/0d/ex_ttest2.py` & `spm1d-0.4.2/spm1d/examples/normality/0d/ex_ttest2.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/examples/normality/1d/ex_anova1.py` & `spm1d-0.4.2/spm1d/examples/normality/1d/ex_regression.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 
 #(0) Load dataset:
-dataset      = spm1d.data.uv1d.anova1.SpeedGRFcategorical()
-dataset      = spm1d.data.uv1d.anova1.Weather()
-y,A          = dataset.get_data()
-
+dataset    = spm1d.data.uv1d.regress.SimulatedPataky2015c()
+# dataset    = spm1d.data.uv1d.regress.SpeedGRF()
+y,x        = dataset.get_data()
 
 
 
 #(1) Conduct normality test:
 np.random.seed(0)
 alpha      = 0.05
-spmi       = spm1d.stats.normality.anova1(y, A).inference(alpha)
+spmi       = spm1d.stats.normality.k2.regress(y, x).inference(alpha)
 print( spmi )
 
 
 
 #(2) Plot
-plt.close('all')
-plt.figure(figsize=(14,4))
-ax = plt.subplot(131);  ax.plot(y.T, 'k', lw=0.5);   ax.set_title('Data')
-ax = plt.subplot(132);  ax.plot(spmi.residuals.T, 'k', lw=0.5);   ax.set_title('Residuals')
-ax = plt.subplot(133);  spmi.plot(ax=ax);   spmi.plot_threshold_label(ax=ax); ax.set_title('Normality test')
-plt.tight_layout()
-plt.show()
-
+pyplot.close('all')
+pyplot.figure(figsize=(14,4))
 
+ax = pyplot.subplot(131);  ax.plot(y.T, 'k', lw=0.5);   ax.set_title('Data')
+ax = pyplot.subplot(132);  ax.plot(spmi.residuals.T, 'k', lw=0.5);   ax.set_title('Residuals')
+ax = pyplot.subplot(133);  spmi.plot(ax=ax);   spmi.plot_threshold_label(ax=ax); ax.set_title('Normality test')
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/normality/1d/ex_anova1rm.py` & `spm1d-0.4.2/spm1d/examples/normality/1d/ex_anova1rm.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 
 #(0) Load dataset:
 dataset      = spm1d.data.uv1d.anova1rm.SpeedGRFcategoricalRM()
@@ -12,23 +12,22 @@
 
 
 
 
 #(1) Conduct normality test:
 np.random.seed(0)
 alpha      = 0.05
-spmi       = spm1d.stats.normality.anova1rm(y, A, SUBJ).inference(alpha)
+spmi       = spm1d.stats.normality.k2.anova1rm(y, A, SUBJ).inference(alpha)
 print( spmi )
 
 
 
 #(2) Plot
-plt.close('all')
-plt.figure(figsize=(14,4))
-ax = plt.subplot(131);  ax.plot(y.T, 'k', lw=0.5);   ax.set_title('Data')
-ax = plt.subplot(132);  ax.plot(spmi.residuals.T, 'k', lw=0.5);   ax.set_title('Residuals')
-ax = plt.subplot(133);  spmi.plot(ax=ax);   spmi.plot_threshold_label(ax=ax); ax.set_title('Normality test')
-plt.tight_layout()
-plt.show()
+pyplot.close('all')
+pyplot.figure(figsize=(14,4))
+ax = pyplot.subplot(131);  ax.plot(y.T, 'k', lw=0.5);   ax.set_title('Data')
+ax = pyplot.subplot(132);  ax.plot(spmi.residuals.T, 'k', lw=0.5);   ax.set_title('Residuals')
+ax = pyplot.subplot(133);  spmi.plot(ax=ax);   spmi.plot_threshold_label(ax=ax); ax.set_title('Normality test')
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/normality/1d/ex_ttest.py` & `spm1d-0.4.2/spm1d/examples/normality/1d/ex_ttest.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 
 #(0) Load dataset:
-dataset    = spm1d.data.uv1d.t1.Random()
 # dataset    = spm1d.data.uv1d.t1.SimulatedPataky2015a()
 dataset    = spm1d.data.uv1d.t1.SimulatedPataky2015b()
 y,mu       = dataset.get_data()
 
 
 
 #(1) Conduct normality test:
+np.random.seed(0)
 alpha      = 0.05
-spmi       = spm1d.stats.normality.ttest(y-mu).inference(alpha)
+spmi       = spm1d.stats.normality.k2.ttest(y).inference(alpha)
 print( spmi )
 
 
 
 #(2) Plot
-plt.close('all')
-plt.figure(figsize=(14,4))
-ax = plt.subplot(131);  ax.plot(y.T, 'k', lw=0.5);   ax.set_title('Data')
-ax = plt.subplot(132);  ax.plot(spmi.residuals.T, 'k', lw=0.5);   ax.set_title('Residuals')
-ax = plt.subplot(133);  spmi.plot(ax=ax);   spmi.plot_threshold_label(ax=ax); ax.set_title('Normality test')
-plt.tight_layout()
-plt.show()
+pyplot.close('all')
+pyplot.figure(figsize=(14,4))
+ax = pyplot.subplot(131);  ax.plot(y.T, 'k', lw=0.5);   ax.set_title('Data')
+ax = pyplot.subplot(132);  ax.plot(spmi.residuals.T, 'k', lw=0.5);   ax.set_title('Residuals')
+ax = pyplot.subplot(133);  spmi.plot(ax=ax);   spmi.plot_threshold_label(ax=ax); ax.set_title('Normality test')
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/normality/1d/ex_ttest2.py` & `spm1d-0.4.2/spm1d/examples/normality/1d/ex_ttest_paired.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 
 #(0) Load dataset:
 dataset      = spm1d.data.uv1d.t2.PlantarArchAngle()
-# dataset      = spm1d.data.uv1d.t2.SimulatedTwoLocalMax()
-yA,yB        = dataset.get_data()
+yA,yB        = dataset.get_data()  #normal and fast walking
 
 
 
 #(1) Conduct normality test:
 np.random.seed(0)
 alpha      = 0.05
-spmi       = spm1d.stats.normality.ttest2(yA, yB).inference(alpha)
+spmi       = spm1d.stats.normality.k2.ttest_paired(yA, yB).inference(alpha)
 print( spmi )
 
 
 
 #(2) Plot
-plt.close('all')
-plt.figure(figsize=(14,4))
-ax = plt.subplot(131);  ax.plot(yA.T, 'k', lw=0.5);   ax.plot(yB.T, 'r', lw=0.5);   ax.set_title('Data')
-ax = plt.subplot(132);  ax.plot(spmi.residuals.T, 'k', lw=0.5);   ax.set_title('Residuals')
-ax = plt.subplot(133);  spmi.plot(ax=ax);   spmi.plot_threshold_label(ax=ax); ax.set_title('Normality test')
-plt.tight_layout()
-plt.show()
-
+pyplot.close('all')
+pyplot.figure(figsize=(14,4))
 
+ax = pyplot.subplot(131);  ax.plot(yA.T, 'k', lw=0.5);   ax.plot(yB.T, 'r', lw=0.5);   ax.set_title('Data')
+ax = pyplot.subplot(132);  ax.plot(spmi.residuals.T, 'k', lw=0.5);   ax.set_title('Residuals')
+ax = pyplot.subplot(133);  spmi.plot(ax=ax);   spmi.plot_threshold_label(ax=ax); ax.set_title('Normality test')
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/normality/1d/ex_ttest_paired.py` & `spm1d-0.4.2/spm1d/examples/normality/1d/ex_ttest2.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 
 #(0) Load dataset:
 dataset      = spm1d.data.uv1d.t2.PlantarArchAngle()
-yA,yB        = dataset.get_data()  #normal and fast walking
+# dataset      = spm1d.data.uv1d.t2.SimulatedTwoLocalMax()
+yA,yB        = dataset.get_data()
 
 
 
 #(1) Conduct normality test:
 np.random.seed(0)
 alpha      = 0.05
-spmi       = spm1d.stats.normality.ttest_paired(yA, yB).inference(alpha)
+spmi       = spm1d.stats.normality.k2.ttest2(yA, yB).inference(alpha)
 print( spmi )
 
 
 
 #(2) Plot
-plt.close('all')
-plt.figure(figsize=(14,4))
-ax = plt.subplot(131);  ax.plot(yA.T, 'k', lw=0.5);   ax.plot(yB.T, 'r', lw=0.5);   ax.set_title('Data')
-ax = plt.subplot(132);  ax.plot(spmi.residuals.T, 'k', lw=0.5);   ax.set_title('Residuals')
-ax = plt.subplot(133);  spmi.plot(ax=ax);   spmi.plot_threshold_label(ax=ax); ax.set_title('Normality test')
-plt.tight_layout()
-plt.show()
+pyplot.close('all')
+pyplot.figure(figsize=(14,4))
+
+ax = pyplot.subplot(131);  ax.plot(yA.T, 'k', lw=0.5);   ax.plot(yB.T, 'r', lw=0.5);   ax.set_title('Data')
+ax = pyplot.subplot(132);  ax.plot(spmi.residuals.T, 'k', lw=0.5);   ax.set_title('Residuals')
+ax = pyplot.subplot(133);  spmi.plot(ax=ax);   spmi.plot_threshold_label(ax=ax); ax.set_title('Normality test')
+pyplot.show()
+
+
```

### Comparing `spm1d-0.4.19/spm1d/examples/normality/paper/appendix_FigA1.py` & `spm1d-0.4.2/spm1d/examples/normality/paper/appendix_FigA1.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 #(0) Load data:
 np.random.seed(1)
 y0         = spm1d.data.uv1d.normality.NormalityAppendixDataset('A1').Y
@@ -16,46 +16,46 @@
 K2         = [spm1d.stats.normality.dagostinoK2(yy)  for yy in [y0,y1,y2]]
 P          = [spm1d.stats.normality.shapirowilk(yy)[1]  for yy in [y0,y1,y2]]
 logP       = -np.log10(P)
 
 
 
 #(2) Plot:
-plt.close('all')
+pyplot.close('all')
 figw       = 8
 figh       = figw / 1.6
-plt.figure(figsize=(figw,figh))
+pyplot.figure(figsize=(figw,figh))
 ### create axes:
 axw = axh  = 0.27
 axx,axy    = np.linspace(0.07, 0.71, 3), np.linspace(0.72, 0.09, 3)
-AX         = np.array(  [[plt.axes([xx, yy, axw, axh])  for xx in axx]  for yy in axy]  )
+AX         = np.array(  [[pyplot.axes([xx, yy, axw, axh])  for xx in axx]  for yy in axy]  )
 ### plot datasets:
 [ax.plot(yy.T, 'k', lw=0.5)   for ax,yy in zip(AX[0], [y0,y1,y2])]
 ### plot K2 stats:
 [ax.plot(k2.z, 'b', lw=2)   for ax,k2 in zip(AX[1], K2)]
 ### plot Shapiro-Wilk p values:
 [ax.plot(p, 'g', lw=2)   for ax,p in zip(AX[2], logP)]
 ### adjust axis tick labels:
-[plt.setp(ax.get_xticklabels() + ax.get_yticklabels(), size=8 )   for ax in AX.flatten()]
-plt.setp(AX[0], ylim=(-3.9,3.9))
-plt.setp(AX[1], ylim=(0, 20))
-plt.setp(AX[2], ylim=(0, 2.8))
-plt.setp(AX[:2],   xticklabels=[])
-plt.setp(AX[:,1:], yticklabels=[])
+[pyplot.setp(ax.get_xticklabels() + ax.get_yticklabels(), size=8 )   for ax in AX.flatten()]
+pyplot.setp(AX[0], ylim=(-3.9,3.9))
+pyplot.setp(AX[1], ylim=(0, 20))
+pyplot.setp(AX[2], ylim=(0, 2.8))
+pyplot.setp(AX[:2],   xticklabels=[])
+pyplot.setp(AX[:,1:], yticklabels=[])
 ### p values:
 [AX[2,0].axhline(yy, color='g', ls=':')  for yy in [1,2]]
 [AX[2,0].text(75, yy+0.1, 'p = %s'%pp, color='g', size=8)  for yy,pp in zip([1,2],[0.1,0.01])]
 
 ### axis labels:
 [ax.set_xlabel('Time  (%)', size=14)   for ax in AX[2]]
 ylabels   = '', r'$K^2$', r'$-\log_{10}(p)$'
 [ax.set_ylabel(label, size=14)   for ax,label in zip(AX[:,0], ylabels)]
 ### dataset labels
 [ax.text(0.5, 0.85, 'Dataset A%d'%(i+1), size=10, ha='center', bbox=dict(color='0.85'), transform=ax.transAxes)  for  i,ax in enumerate(AX[0])]
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/normality/paper/appendix_FigA2.py` & `spm1d-0.4.2/spm1d/examples/normality/paper/appendix_FigA4.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,60 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 #(0) Load data:
 np.random.seed(1)
-y0         = spm1d.data.uv1d.normality.NormalityAppendixDataset('A1').Y
-y1         = spm1d.data.uv1d.normality.NormalityAppendixDataset('A2').Y
-y2         = spm1d.data.uv1d.normality.NormalityAppendixDataset('A3').Y
+y0         = spm1d.data.uv1d.normality.NormalityAppendixDataset('A7').Y
+y1         = spm1d.data.uv1d.normality.NormalityAppendixDataset('A8').Y
+y2         = spm1d.data.uv1d.normality.NormalityAppendixDataset('A9').Y
+WW         = [10, 25, 50]
+
 
 
 #(1) Compute normality metrics:
-K2         = [spm1d.stats.normality.dagostinoK2(yy).inference(0.05)  for yy in [y0,y1,y2]]
+K2         = [spm1d.stats.normality.dagostinoK2(yy)  for yy in [y0,y1,y2]]
 P          = [spm1d.stats.normality.shapirowilk(yy)[1]  for yy in [y0,y1,y2]]
 logP       = -np.log10(P)
 
 
 
 #(2) Plot:
-plt.close('all')
+pyplot.close('all')
 figw       = 8
 figh       = figw / 1.6
-plt.figure(figsize=(figw,figh))
+pyplot.figure(figsize=(figw,figh))
 ### create axes:
 axw = axh  = 0.27
 axx,axy    = np.linspace(0.07, 0.71, 3), np.linspace(0.72, 0.09, 3)
-AX         = np.array(  [[plt.axes([xx, yy, axw, axh])  for xx in axx]  for yy in axy]  )
+AX         = np.array(  [[pyplot.axes([xx, yy, axw, axh])  for xx in axx]  for yy in axy]  )
 ### plot datasets:
-[ax.plot(yy.T, 'k', lw=0.5)   for ax,yy in zip(AX[0], [y0,y1,y2])]
+[ax.plot(yy.T, 'k', lw=0.2)   for ax,yy in zip(AX[0], [y0,y1,y2])]
 ### plot K2 stats:
-[k2i.plot(ax=ax, color='b')   for ax,k2i in zip(AX[1], K2)]
+[ax.plot(k2.z, color='b', lw=3)   for ax,k2 in zip(AX[1], K2)]
 ### plot Shapiro-Wilk p values:
 [ax.plot(p, 'g', lw=2)   for ax,p in zip(AX[2], logP)]
 ### adjust axis tick labels:
-[plt.setp(ax.get_xticklabels() + ax.get_yticklabels(), size=8 )   for ax in AX.flatten()]
-plt.setp(AX[0], ylim=(-3.9,3.9))
-plt.setp(AX[1], ylim=(0, 20))
-plt.setp(AX[2], ylim=(0, 2.8))
-plt.setp(AX[:2],   xticklabels=[])
-plt.setp(AX[:,1:], yticklabels=[], ylabel='')
+[pyplot.setp(ax.get_xticklabels() + ax.get_yticklabels(), size=8 )   for ax in AX.flatten()]
+pyplot.setp(AX[0], ylim=(-4.9,4.9))
+pyplot.setp(AX[1], ylim=(0, 15))
+pyplot.setp(AX[2], ylim=(0, 2.8))
+pyplot.setp(AX[:2],   xticklabels=[])
+pyplot.setp(AX[:,1:], yticklabels=[])
 ### axis labels:
 [ax.set_xlabel('Time  (%)', size=14)   for ax in AX[2]]
 ylabels   = '', r'$K^2$', r'$-\log_{10}(p)$'
 [ax.set_ylabel(label, size=14)   for ax,label in zip(AX[:,0], ylabels)]
 ### dataset labels
-[ax.text(0.5, 0.85, 'Dataset A%d'%(i+1), size=10, ha='center', bbox=dict(color='0.85'), transform=ax.transAxes)  for  i,ax in enumerate(AX[0])]
-plt.show()
+[ax.text(0.25, 0.85, 'Dataset A%d'%(i+7), size=10, ha='center', bbox=dict(color='0.85'), transform=ax.transAxes)  for  i,ax in enumerate(AX[0])]
+[ax.text(0.55, 0.85, 'FWHM = %d'%w, size=10, ha='left', transform=ax.transAxes)  for  i,(ax,w) in enumerate(zip(AX[0],WW))]
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/normality/paper/appendix_FigA3.py` & `spm1d-0.4.2/spm1d/examples/normality/paper/appendix_FigA3.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 #(0) Load data:
 np.random.seed(1)
 y0         = spm1d.data.uv1d.normality.NormalityAppendixDataset('A4').Y
@@ -16,44 +16,44 @@
 K2         = [spm1d.stats.normality.dagostinoK2(yy)  for yy in [y0,y1,y2]]
 P          = [spm1d.stats.normality.shapirowilk(yy)[1]  for yy in [y0,y1,y2]]
 logP       = -np.log10(P)
 
 
 
 #(2) Plot:
-plt.close('all')
+pyplot.close('all')
 figw       = 8
 figh       = figw / 1.6
-plt.figure(figsize=(figw,figh))
+pyplot.figure(figsize=(figw,figh))
 ### create axes:
 axw = axh  = 0.27
 axx,axy    = np.linspace(0.07, 0.71, 3), np.linspace(0.72, 0.09, 3)
-AX         = np.array(  [[plt.axes([xx, yy, axw, axh])  for xx in axx]  for yy in axy]  )
+AX         = np.array(  [[pyplot.axes([xx, yy, axw, axh])  for xx in axx]  for yy in axy]  )
 ### plot datasets:
 [ax.plot(yy.T, 'k', lw=0.2)   for ax,yy in zip(AX[0], [y0,y1,y2])]
 ### plot K2 stats:
 # [k2i.plot(ax=ax, color='b')   for ax,k2i in zip(AX[1], K2i)]
 [ax.plot(k2.z, color='b', lw=3)   for ax,k2 in zip(AX[1], K2)]
 ### plot Shapiro-Wilk p values:
 [ax.plot(p, 'g', lw=2)   for ax,p in zip(AX[2], logP)]
 ### adjust axis tick labels:
-[plt.setp(ax.get_xticklabels() + ax.get_yticklabels(), size=8 )   for ax in AX.flatten()]
-plt.setp(AX[0], ylim=(-4.9,4.9))
-plt.setp(AX[1], ylim=(0, 15))
-plt.setp(AX[2], ylim=(0, 2.8))
-plt.setp(AX[:2],   xticklabels=[])
-plt.setp(AX[:,1:], yticklabels=[])
+[pyplot.setp(ax.get_xticklabels() + ax.get_yticklabels(), size=8 )   for ax in AX.flatten()]
+pyplot.setp(AX[0], ylim=(-4.9,4.9))
+pyplot.setp(AX[1], ylim=(0, 15))
+pyplot.setp(AX[2], ylim=(0, 2.8))
+pyplot.setp(AX[:2],   xticklabels=[])
+pyplot.setp(AX[:,1:], yticklabels=[])
 ### axis labels:
 [ax.set_xlabel('Time  (%)', size=14)   for ax in AX[2]]
 ylabels   = '', r'$K^2$', r'$-\log_{10}(p)$'
 [ax.set_ylabel(label, size=14)   for ax,label in zip(AX[:,0], ylabels)]
 ### dataset labels
 [ax.text(0.45, 0.85, 'Dataset A%d'%(i+4), size=10, ha='center', bbox=dict(color='0.85'), transform=ax.transAxes)  for  i,ax in enumerate(AX[0])]
 [ax.text(0.75, 0.85, 'J = %d'%j, size=10, ha='left', transform=ax.transAxes)  for  i,(ax,j) in enumerate(zip(AX[0],JJ))]
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/normality/paper/appendix_FigA4.py` & `spm1d-0.4.2/spm1d/examples/normality/paper/appendix_FigA7.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,60 +1,62 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 #(0) Load data:
 np.random.seed(1)
-y0         = spm1d.data.uv1d.normality.NormalityAppendixDataset('A7').Y
-y1         = spm1d.data.uv1d.normality.NormalityAppendixDataset('A8').Y
-y2         = spm1d.data.uv1d.normality.NormalityAppendixDataset('A9').Y
-WW         = [10, 25, 50]
-
+y0         = spm1d.data.uv1d.normality.NormalityAppendixDataset('A15').Y
+y1         = spm1d.data.uv1d.normality.NormalityAppendixDataset('A16').Y
+y2         = spm1d.data.uv1d.normality.NormalityAppendixDataset('A17').Y
 
 
 #(1) Compute normality metrics:
 K2         = [spm1d.stats.normality.dagostinoK2(yy)  for yy in [y0,y1,y2]]
 P          = [spm1d.stats.normality.shapirowilk(yy)[1]  for yy in [y0,y1,y2]]
 logP       = -np.log10(P)
 
 
 
 #(2) Plot:
-plt.close('all')
+pyplot.close('all')
 figw       = 8
 figh       = figw / 1.6
-plt.figure(figsize=(figw,figh))
+pyplot.figure(figsize=(figw,figh))
 ### create axes:
 axw = axh  = 0.27
-axx,axy    = np.linspace(0.07, 0.71, 3), np.linspace(0.72, 0.09, 3)
-AX         = np.array(  [[plt.axes([xx, yy, axw, axh])  for xx in axx]  for yy in axy]  )
+axx,axy    = np.linspace(0.08, 0.71, 3), [0.72, 0.42, 0.04]
+AX         = np.array(  [[pyplot.axes([xx, yy, axw, axh])  for xx in axx]  for yy in axy]  )
 ### plot datasets:
 [ax.plot(yy.T, 'k', lw=0.2)   for ax,yy in zip(AX[0], [y0,y1,y2])]
 ### plot K2 stats:
-[ax.plot(k2.z, color='b', lw=3)   for ax,k2 in zip(AX[1], K2)]
-### plot Shapiro-Wilk p values:
-[ax.plot(p, 'g', lw=2)   for ax,p in zip(AX[2], logP)]
+[k2.plot(ax=ax, color='b')   for ax,k2 in zip(AX[1], K2)]
+### plot histograms:
+bins       = 17
+rng        = -12, 12
+ind        = 50
+[ax.hist(yy[:,ind], bins=bins, range=rng, facecolor='c')   for ax,yy in zip(AX[2], [y0,y1,y2])]
 ### adjust axis tick labels:
-[plt.setp(ax.get_xticklabels() + ax.get_yticklabels(), size=8 )   for ax in AX.flatten()]
-plt.setp(AX[0], ylim=(-4.9,4.9))
-plt.setp(AX[1], ylim=(0, 15))
-plt.setp(AX[2], ylim=(0, 2.8))
-plt.setp(AX[:2],   xticklabels=[])
-plt.setp(AX[:,1:], yticklabels=[])
+[pyplot.setp(ax.get_xticklabels() + ax.get_yticklabels(), size=8 )   for ax in AX.flatten()]
+pyplot.setp(AX[0], ylim=(-14,14))
+pyplot.setp(AX[1], ylim=(-50, 500), ylabel='')
+pyplot.setp(AX[2], ylim=(0, 80))
+pyplot.setp(AX[:2],   xticklabels=[])
+pyplot.setp(AX[:,1:], yticklabels=[])
 ### axis labels:
-[ax.set_xlabel('Time  (%)', size=14)   for ax in AX[2]]
-ylabels   = '', r'$K^2$', r'$-\log_{10}(p)$'
+[ax.set_xlabel('Time  (%)', size=14)   for ax in AX[1]]
+ylabels   = '', r'$K^2$', 'Frequency'
 [ax.set_ylabel(label, size=14)   for ax,label in zip(AX[:,0], ylabels)]
+### time instant labels:
+[ax.text(0.1, 0.8, 'Time = %d%s'%(ind,'%'), size=9, transform=ax.transAxes)  for ax in AX[2]]
 ### dataset labels
-[ax.text(0.25, 0.85, 'Dataset A%d'%(i+7), size=10, ha='center', bbox=dict(color='0.85'), transform=ax.transAxes)  for  i,ax in enumerate(AX[0])]
-[ax.text(0.55, 0.85, 'FWHM = %d'%w, size=10, ha='left', transform=ax.transAxes)  for  i,(ax,w) in enumerate(zip(AX[0],WW))]
-plt.show()
+[ax.text(0.5, 0.85, 'Dataset A%d'%(i+15), size=10, ha='center', bbox=dict(color='0.85'), transform=ax.transAxes)  for  i,ax in enumerate(AX[0])]
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/normality/paper/appendix_FigA5.py` & `spm1d-0.4.2/spm1d/examples/normality/paper/appendix_FigA2.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,56 +1,57 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 #(0) Load data:
 np.random.seed(1)
-y0         = spm1d.data.uv1d.normality.NormalityAppendixDataset('A10').Y
-y1         = spm1d.data.uv1d.normality.NormalityAppendixDataset('A11').Y
-
+y0         = spm1d.data.uv1d.normality.NormalityAppendixDataset('A1').Y
+y1         = spm1d.data.uv1d.normality.NormalityAppendixDataset('A2').Y
+y2         = spm1d.data.uv1d.normality.NormalityAppendixDataset('A3').Y
 
 
 #(1) Compute normality metrics:
-K2i        = [spm1d.stats.normality.dagostinoK2(yy).inference(0.05)  for yy in [y0,y1]]
-P          = [spm1d.stats.normality.shapirowilk(yy)[1]  for yy in [y0,y1]]
+K2         = [spm1d.stats.normality.dagostinoK2(yy).inference(0.05)  for yy in [y0,y1,y2]]
+P          = [spm1d.stats.normality.shapirowilk(yy)[1]  for yy in [y0,y1,y2]]
 logP       = -np.log10(P)
 
 
 
 #(2) Plot:
-plt.close('all')
-plt.figure(figsize=(6,6))
+pyplot.close('all')
+figw       = 8
+figh       = figw / 1.6
+pyplot.figure(figsize=(figw,figh))
 ### create axes:
-axw,axh    = 0.42, 0.27
-axx,axy    = [0.10,0.56], np.linspace(0.72, 0.09, 3)
-AX         = np.array(  [[plt.axes([xx, yy, axw, axh])  for xx in axx]  for yy in axy]  )
+axw = axh  = 0.27
+axx,axy    = np.linspace(0.07, 0.71, 3), np.linspace(0.72, 0.09, 3)
+AX         = np.array(  [[pyplot.axes([xx, yy, axw, axh])  for xx in axx]  for yy in axy]  )
 ### plot datasets:
-[ax.plot(yy.T, 'k', lw=0.5)   for ax,yy in zip(AX[0], [y0,y1])]
+[ax.plot(yy.T, 'k', lw=0.5)   for ax,yy in zip(AX[0], [y0,y1,y2])]
 ### plot K2 stats:
-[k2i.plot(ax=ax, color='b')   for ax,k2i in zip(AX[1], K2i)]
+[k2i.plot(ax=ax, color='b')   for ax,k2i in zip(AX[1], K2)]
 ### plot Shapiro-Wilk p values:
 [ax.plot(p, 'g', lw=2)   for ax,p in zip(AX[2], logP)]
 ### adjust axis tick labels:
-[plt.setp(ax.get_xticklabels() + ax.get_yticklabels(), size=8 )   for ax in AX.flatten()]
-plt.setp(AX[0], ylim=(-3,9))
-plt.setp(AX[1], ylim=(0, 20), ylabel='')
-plt.setp(AX[2], ylim=(0, 2.8))
-plt.setp(AX[:2],   xticklabels=[])
-plt.setp(AX[:,1:], yticklabels=[])
+[pyplot.setp(ax.get_xticklabels() + ax.get_yticklabels(), size=8 )   for ax in AX.flatten()]
+pyplot.setp(AX[0], ylim=(-3.9,3.9))
+pyplot.setp(AX[1], ylim=(0, 20))
+pyplot.setp(AX[2], ylim=(0, 2.8))
+pyplot.setp(AX[:2],   xticklabels=[])
+pyplot.setp(AX[:,1:], yticklabels=[], ylabel='')
 ### axis labels:
 [ax.set_xlabel('Time  (%)', size=14)   for ax in AX[2]]
 ylabels   = '', r'$K^2$', r'$-\log_{10}(p)$'
 [ax.set_ylabel(label, size=14)   for ax,label in zip(AX[:,0], ylabels)]
 ### dataset labels
-[ax.text(0.5, 0.85, 'Dataset A%d'%(i+10), size=10, ha='center', bbox=dict(color='0.85'), transform=ax.transAxes)  for  i,ax in enumerate(AX[0])]
-plt.show()
-
+[ax.text(0.5, 0.85, 'Dataset A%d'%(i+1), size=10, ha='center', bbox=dict(color='0.85'), transform=ax.transAxes)  for  i,ax in enumerate(AX[0])]
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/normality/paper/appendix_FigA6.py` & `spm1d-0.4.2/spm1d/examples/normality/paper/appendix_FigA6.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 #(0) Load data:
 np.random.seed(1)
 y0         = spm1d.data.uv1d.normality.NormalityAppendixDataset('A12').Y
@@ -16,47 +16,47 @@
 K2         = [spm1d.stats.normality.dagostinoK2(yy)  for yy in [y0,y1,y2]]
 P          = [spm1d.stats.normality.shapirowilk(yy)[1]  for yy in [y0,y1,y2]]
 logP       = -np.log10(P)
 
 
 
 #(2) Plot:
-plt.close('all')
+pyplot.close('all')
 figw       = 8
 figh       = figw / 1.6
-plt.figure(figsize=(figw,figh))
+pyplot.figure(figsize=(figw,figh))
 ### create axes:
 axw = axh  = 0.27
 axx,axy    = np.linspace(0.08, 0.71, 3), [0.72, 0.42, 0.04]
-AX         = np.array(  [[plt.axes([xx, yy, axw, axh])  for xx in axx]  for yy in axy]  )
+AX         = np.array(  [[pyplot.axes([xx, yy, axw, axh])  for xx in axx]  for yy in axy]  )
 ### plot datasets:
 [ax.plot(yy.T, 'k', lw=0.2)   for ax,yy in zip(AX[0], [y0,y1,y2])]
 ### plot K2 stats:
 [k2.plot(ax=ax, color='b')   for ax,k2 in zip(AX[1], K2)]
 ### plot histograms:
 bins       = 17
 rng        = -7, 7
 ind        = 50
 [ax.hist(yy[:,ind], bins=bins, range=rng, facecolor='c')   for ax,yy in zip(AX[2], [y0,y1,y2])]
 ### adjust axis tick labels:
-[plt.setp(ax.get_xticklabels() + ax.get_yticklabels(), size=8 )   for ax in AX.flatten()]
-plt.setp(AX[0], ylim=(-7,7))
-plt.setp(AX[1], ylim=(0, 55), ylabel='')
-plt.setp(AX[2], ylim=(0, 220))
-plt.setp(AX[:2],   xticklabels=[])
-plt.setp(AX[:,1:], yticklabels=[])
+[pyplot.setp(ax.get_xticklabels() + ax.get_yticklabels(), size=8 )   for ax in AX.flatten()]
+pyplot.setp(AX[0], ylim=(-7,7))
+pyplot.setp(AX[1], ylim=(0, 55), ylabel='')
+pyplot.setp(AX[2], ylim=(0, 220))
+pyplot.setp(AX[:2],   xticklabels=[])
+pyplot.setp(AX[:,1:], yticklabels=[])
 ### axis labels:
 [ax.set_xlabel('Time  (%)', size=14)   for ax in AX[1]]
 ylabels   = '', r'$K^2$', 'Frequency'
 [ax.set_ylabel(label, size=14)   for ax,label in zip(AX[:,0], ylabels)]
 ### time instant labels:
 [ax.text(0.05, 0.8, 'Time = %d%s'%(ind,'%'), size=9, transform=ax.transAxes)  for ax in AX[2]]
 ### dataset labels
 [ax.text(0.5, 0.85, 'Dataset A%d'%(i+12), size=10, ha='center', bbox=dict(color='0.85'), transform=ax.transAxes)  for  i,ax in enumerate(AX[0])]
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/processing/data/ex_kinematics_for_interpolation.npy` & `spm1d-0.4.2/spm1d/examples/processing/data/ex_kinematics_for_interpolation.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/examples/processing/ex_smooth.py` & `spm1d-0.4.2/spm1d/examples/processing/ex_smooth.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 # create random data:
 np.random.seed(0)
 Y0           = np.random.randn(5,101)
 
 # smooth:
 Y           = spm1d.util.smooth(Y0, fwhm=5.0)
 
 # plot:
-plt.close('all')
-fig,(ax0,ax1) = plt.subplots(1, 2, figsize=(8,3.5))
+pyplot.close('all')
+pyplot.figure(figsize=(8,3.5))
+ax0          = pyplot.axes((0.1,0.15,0.35,0.8))
+ax1          = pyplot.axes((0.55,0.15,0.35,0.8))
 ax0.plot(Y0.T, 'k')
 ax1.plot(Y.T, 'k')
 ax0.text(0.5, 0.9, 'Before smoothing', size=14, transform=ax0.transAxes, ha='center')
 ax1.text(0.5, 0.9, 'After smoothing', size=14, transform=ax1.transAxes, ha='center')
-plt.tight_layout()
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/scipy/ex_regression.py` & `spm1d-0.4.2/spm1d/examples/scipy/ex_regression.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/examples/scipy/ex_ttest_normality.py` & `spm1d-0.4.2/spm1d/examples/scipy/ex_ttest_normality.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/examples/scipy/ex_ttest_onesample.py` & `spm1d-0.4.2/spm1d/examples/scipy/ex_ttest_onesample.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/examples/scipy/ex_ttest_paired.py` & `spm1d-0.4.2/spm1d/examples/scipy/ex_ttest_paired.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/examples/scipy/ex_ttest_twosample.py` & `spm1d-0.4.2/spm1d/examples/scipy/ex_ttest_twosample.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/examples/scipy/ex_ttest_twosample_unequalvar.py` & `spm1d-0.4.2/spm1d/examples/scipy/ex_ttest_twosample_unequalvar.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/examples/stats0d/ex_anova2.py` & `spm1d-0.4.2/spm1d/examples/stats0d/ex_anova2.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 
 
 
 
 
 
 #(0) Load dataset:
-# dataset   = spm1d.data.uv0d.anova2.Mouse()       #2x2
+dataset   = spm1d.data.uv0d.anova2.Mouse()       #2x2
 dataset   = spm1d.data.uv0d.anova2.Detergent()     #2x3
-# dataset   = spm1d.data.uv0d.anova2.Satisfaction()  #2x3
-# dataset   = spm1d.data.uv0d.anova2.SouthamptonCrossed1()  #2x3
+dataset   = spm1d.data.uv0d.anova2.Satisfaction()  #2x3
+dataset   = spm1d.data.uv0d.anova2.SouthamptonCrossed1()  #2x3
 # dataset   = spm1d.data.uv0d.anova2.SPM1D3x3()
 # dataset   = spm1d.data.uv0d.anova2.SPM1D3x4()
 # dataset   = spm1d.data.uv0d.anova2.SPM1D3x5()
 # dataset   = spm1d.data.uv0d.anova2.SPM1D4x4()
 # dataset   = spm1d.data.uv0d.anova2.SPM1D4x5()
 y,A,B     = dataset.get_data()
 print( dataset )
```

### Comparing `spm1d-0.4.19/spm1d/examples/stats0d/ex_anova2onerm.py` & `spm1d-0.4.2/spm1d/examples/stats0d/ex_anova2onerm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 
 import spm1d
 
 
 
 
 #(0) Load dataset:
-dataset    = spm1d.data.uv0d.anova2onerm.RSXLDrug()
 dataset    = spm1d.data.uv0d.anova2onerm.Santa23()
-# dataset    = spm1d.data.uv0d.anova2onerm.Southampton2onerm()
+dataset    = spm1d.data.uv0d.anova2onerm.Southampton2onerm()
+# dataset    = spm1d.data.uv0d.anova2onerm.RSXLDrug()
 # dataset    = spm1d.data.uv0d.anova2onerm.SPM1D3x3()
 # dataset    = spm1d.data.uv0d.anova2onerm.SPM1D3x4()
 # dataset    = spm1d.data.uv0d.anova2onerm.SPM1D3x4A()
 # dataset    = spm1d.data.uv0d.anova2onerm.SPM1D3x5()
 # dataset    = spm1d.data.uv0d.anova2onerm.SPM1D4x4()
 # dataset    = spm1d.data.uv0d.anova2onerm.SPM1D4x5()
 y,A,B,SUBJ = dataset.get_data()
```

### Comparing `spm1d-0.4.19/spm1d/examples/stats0d/ex_anova2rm.py` & `spm1d-0.4.2/spm1d/examples/stats0d/ex_anova2rm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/examples/stats0d/ex_ci_onesample.py` & `spm1d-0.4.2/spm1d/examples/stats0d/ex_ci_onesample.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 - explicit null hypothesis testing is conducted
 - the null hypothesis is rejected if mu lies outside the CI
 '''
 
 
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 #(0) Load dataset:
-# dataset = spm1d.data.uv0d.ci1.MinnesotaGeyerRate()
+dataset = spm1d.data.uv0d.ci1.MinnesotaGeyerRate()
 dataset = spm1d.data.uv0d.ci1.WebsterSleep()
 y,mu    = dataset.get_data()
 print( dataset )
 
 
 
 #(1) Compute confidence intervals:
@@ -37,13 +37,13 @@
 ci1        = spm1d.stats.ci_onesample(y, alpha, mu=mu)    #hypothesis test regarding a specific population mean "mu=9"
 print( ci0 )
 print( ci1 )
 
 
 
 #(2) Plot the CIs:
-plt.close('all')
-plt.figure(figsize=(8,4))
-ax0 = plt.subplot(121);  ci0.plot(ax0);  ax0.set_title('mu=None', size=10)
-ax1 = plt.subplot(122);  ci1.plot(ax1);  ax1.set_title('mu=%.5f'%mu, size=10)
-plt.suptitle('One-sample CIs')
-plt.show()
+pyplot.close('all')
+pyplot.figure(figsize=(8,4))
+ax0 = pyplot.subplot(121);  ci0.plot(ax0);  ax0.set_title('mu=None', size=10)
+ax1 = pyplot.subplot(122);  ci1.plot(ax1);  ax1.set_title('mu=%.5f'%mu, size=10)
+pyplot.suptitle('One-sample CIs')
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/stats0d/ex_ci_onesample_standalone.py` & `spm1d-0.4.2/spm1d/examples/stats0d/ex_ci_onesample_standalone.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/examples/stats0d/ex_ci_pairedsample.py` & `spm1d-0.4.2/spm1d/examples/stats0d/ex_ci_pairedsample.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 #(0) Load dataset:
 dataset = spm1d.data.uv0d.cipaired.FraminghamSystolicBloodPressure()
 yA,yB   = dataset.get_data()
@@ -24,16 +24,16 @@
 print( ci1 )
 print( ci2 )
 print( ci3 )
 
 
 
 #(2) Plot the CIs:
-plt.close('all')
-plt.figure(figsize=(8,8))
-ax0 = plt.subplot(221);  ci0.plot(ax0);  ax0.set_title('datum="difference", mu=None', size=10)
-ax1 = plt.subplot(222);  ci1.plot(ax1);  ax1.set_title('datum="difference", mu=%.5f'%mu, size=10)
-ax2 = plt.subplot(223);  ci2.plot(ax2);  ax2.set_title('datum="meanA", mu="meanB"', size=10)
-ax3 = plt.subplot(224);  ci3.plot(ax3);  ax3.set_title('datum="meanA", mu="tailB"', size=10)
-plt.suptitle('Paired sample CIs')
-plt.show()
+pyplot.close('all')
+pyplot.figure(figsize=(8,8))
+ax0 = pyplot.subplot(221);  ci0.plot(ax0);  ax0.set_title('datum="difference", mu=None', size=10)
+ax1 = pyplot.subplot(222);  ci1.plot(ax1);  ax1.set_title('datum="difference", mu=%.5f'%mu, size=10)
+ax2 = pyplot.subplot(223);  ci2.plot(ax2);  ax2.set_title('datum="meanA", mu="meanB"', size=10)
+ax3 = pyplot.subplot(224);  ci3.plot(ax3);  ax3.set_title('datum="meanA", mu="tailB"', size=10)
+pyplot.suptitle('Paired sample CIs')
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/stats0d/ex_ci_twosample.py` & `spm1d-0.4.2/spm1d/examples/stats0d/ex_ci_twosample.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 #(0) Load dataset:
 dataset = spm1d.data.uv0d.ci2.AnimalsInResearch()
 yA,yB   = dataset.get_data()
@@ -23,15 +23,15 @@
 print( ci1 )
 print( ci2 )
 print( ci3 )
 
 
 
 #(2) Plot the CIs:
-plt.close('all')
-plt.figure(figsize=(8,8))
-ax0 = plt.subplot(221);  ci0.plot(ax0);  ax0.set_title('datum="difference", mu=None', size=10)
-ax1 = plt.subplot(222);  ci1.plot(ax1);  ax1.set_title('datum="difference", mu=%.5f'%mu, size=10)
-ax2 = plt.subplot(223);  ci2.plot(ax2);  ax2.set_title('datum="meanA", mu="meanB"', size=10)
-ax3 = plt.subplot(224);  ci3.plot(ax3);  ax3.set_title('datum="meanA", mu="tailsAB"', size=10)
-plt.suptitle('Paired sample CIs')
-plt.show()
+pyplot.close('all')
+pyplot.figure(figsize=(8,8))
+ax0 = pyplot.subplot(221);  ci0.plot(ax0);  ax0.set_title('datum="difference", mu=None', size=10)
+ax1 = pyplot.subplot(222);  ci1.plot(ax1);  ax1.set_title('datum="difference", mu=%.5f'%mu, size=10)
+ax2 = pyplot.subplot(223);  ci2.plot(ax2);  ax2.set_title('datum="meanA", mu="meanB"', size=10)
+ax3 = pyplot.subplot(224);  ci3.plot(ax3);  ax3.set_title('datum="meanA", mu="tailsAB"', size=10)
+pyplot.suptitle('Paired sample CIs')
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/stats1d/ex_anova1.py` & `spm1d-0.4.2/spm1d/examples/stats1d_roi/ex_anova1.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 
-import matplotlib.pyplot as plt
+import numpy as np
+from matplotlib import pyplot
 import spm1d
 
 
 
 #(0) Load dataset:
 dataset      = spm1d.data.uv1d.anova1.SpeedGRFcategorical()
-dataset      = spm1d.data.uv1d.anova1.Weather()
 Y,A          = dataset.get_data()
 
 
+#(0a) Create region of interest(ROI):
+roi        = np.array([False]*Y.shape[1])
+roi[85:]   = True
+
 
 #(1) Run ANOVA:
 alpha        = 0.05
-F            = spm1d.stats.anova1(Y, A, equal_var=False)
-Fi           = F.inference(alpha, interp=True, circular=False)
+F            = spm1d.stats.anova1(Y, A, equal_var=True, roi=roi)
+Fi           = F.inference(alpha, interp=True)
 print( Fi )
-### alternative syntax:
-# Y0,Y1,Y2     = [Y[A==u] for u in np.unique(A)]
-# F            = spm1d.stats.anova1((Y0,Y1,Y2), equal_var=False)
+
 
 
 #(2) Plot results:
-plt.close('all')
+pyplot.close('all')
+# F.plot()
 Fi.plot()
 Fi.plot_threshold_label(bbox=dict(facecolor='w'))
-# plt.ylim(-1, 500)
-plt.xlabel('Time (%)', size=20)
-plt.title(r'Critical threshold at $\alpha$=%.2f:  $F^*$=%.3f' %(alpha, Fi.zstar))
-plt.show()
+# pyplot.ylim(-1, 500)
+pyplot.xlabel('Time (%)', size=20)
+pyplot.title(r'Critical threshold at $\alpha$=%.2f:  $F^*$=%.3f' %(alpha, Fi.zstar))
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/stats1d/ex_anova1rm.py` & `spm1d-0.4.2/spm1d/examples/stats1d/ex_anova1rm.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 #(0) Load dataset:
 dataset      = spm1d.data.uv1d.anova1rm.SpeedGRFcategoricalRM()
 Y,A,SUBJ     = dataset.get_data()
@@ -13,33 +13,33 @@
 
 
 
 #(1) Run ANOVA (compare between- and within-subjects models):
 alpha        = 0.05
 equal_var    = True
 F            = spm1d.stats.anova1(Y, A, equal_var)  #between-subjects
-Frm          = spm1d.stats.anova1rm(Y, A, SUBJ, equal_var)  #within-subjects (repeated-measures)
+Frm          = spm1d.stats.anova1rm(Y, A, SUBJ, equal_var)  #withing-subjects (repeated-measures)
 Fi           = F.inference(alpha)
 Firm         = Frm.inference(alpha)
 
 
 
 
 #(2) Plot:
-plt.close('all')
-plt.figure( figsize=(8, 3.5) )
-ax0     = plt.axes( (0.1, 0.15, 0.35, 0.8) )
-ax1     = plt.axes((0.55,0.15,0.35,0.8))
+pyplot.close('all')
+pyplot.figure( figsize=(8, 3.5) )
+ax0     = pyplot.axes( (0.1, 0.15, 0.35, 0.8) )
+ax1     = pyplot.axes((0.55,0.15,0.35,0.8))
 ### plot mean subject trajectories:
 ax0.plot(Y[A==0].T, 'b')
 ax0.plot(Y[A==1].T, 'k')
 ax0.plot(Y[A==2].T, 'r')
 ### plot SPM results:
 Firm.plot(ax=ax1, color='r', thresh_color='r', facecolor=(0.8,0.3,0.3), label='Within-subjects analysis')
 Fi.plot(ax=ax1, label='Between-subjects analysis')
 ax1.legend(fontsize=8)
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/stats1d/ex_anova2.py` & `spm1d-0.4.2/spm1d/examples/stats1d/ex_anova2onerm.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 
 #(0) Load data:
-# dataset      = spm1d.data.uv1d.anova2.SPM1D_ANOVA2_2x2()
-dataset      = spm1d.data.uv1d.anova2.SPM1D_ANOVA2_2x3()
-# dataset      = spm1d.data.uv1d.anova2.SPM1D_ANOVA2_3x3()
-# dataset      = spm1d.data.uv1d.anova2.SPM1D_ANOVA2_3x4()
-# dataset      = spm1d.data.uv1d.anova2.SPM1D_ANOVA2_3x5()
-# dataset      = spm1d.data.uv1d.anova2.SPM1D_ANOVA2_4x4()
-# dataset      = spm1d.data.uv1d.anova2.SPM1D_ANOVA2_4x5()
-Y,A,B        = dataset.get_data()
+dataset      = spm1d.data.uv1d.anova2onerm.SPM1D_ANOVA2ONERM_2x2()
+# dataset      = spm1d.data.uv1d.anova2onerm.SPM1D_ANOVA2ONERM_2x3()
+# dataset      = spm1d.data.uv1d.anova2onerm.SPM1D_ANOVA2ONERM_3x3()
+# dataset      = spm1d.data.uv1d.anova2onerm.SPM1D_ANOVA2ONERM_3x4()
+# dataset      = spm1d.data.uv1d.anova2onerm.SPM1D_ANOVA2ONERM_3x5()
+# dataset      = spm1d.data.uv1d.anova2onerm.SPM1D_ANOVA2ONERM_4x4()
+# dataset      = spm1d.data.uv1d.anova2onerm.SPM1D_ANOVA2ONERM_4x5()
+Y,A,B,SUBJ   = dataset.get_data()
 
 
 
 #(1) Conduct ANOVA:
 alpha        = 0.05
-FF           = spm1d.stats.anova2(Y, A, B, equal_var=True)
-FFi          = FF.inference(alpha)
+FF           = spm1d.stats.anova2onerm(Y, A, B, SUBJ, equal_var=True)
+FFi          = FF.inference(0.05)
 print( FFi )
 
 
 
 #(2) Plot results:
-plt.close('all')
+pyplot.close('all')
 FFi.plot(plot_threshold_label=True, plot_p_values=True)
-plt.show()
-
-
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/stats1d/ex_anova2nested.py` & `spm1d-0.4.2/spm1d/examples/stats1d/ex_anova2nested.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 
 #(0) Load data:
 # dataset      = spm1d.data.uv1d.anova2nested.SPM1D_ANOVA2NESTED_2x2()
@@ -22,14 +22,14 @@
 alpha        = 0.05
 FF           = spm1d.stats.anova2nested(Y, A, B, equal_var=True)
 FFi          = FF.inference(0.05)
 print( FFi )
 
 
 #(2) Plot results:
-plt.close('all')
+pyplot.close('all')
 FFi.plot(plot_threshold_label=True, plot_p_values=True)
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/stats1d/ex_anova2onerm.py` & `spm1d-0.4.2/spm1d/examples/stats1d/ex_anova2rm.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 
 #(0) Load data:
-dataset      = spm1d.data.uv1d.anova2onerm.SPM1D_ANOVA2ONERM_2x2()
-# dataset      = spm1d.data.uv1d.anova2onerm.SPM1D_ANOVA2ONERM_2x3()
-# dataset      = spm1d.data.uv1d.anova2onerm.SPM1D_ANOVA2ONERM_3x3()
-# dataset      = spm1d.data.uv1d.anova2onerm.SPM1D_ANOVA2ONERM_3x4()
-# dataset      = spm1d.data.uv1d.anova2onerm.SPM1D_ANOVA2ONERM_3x5()
-# dataset      = spm1d.data.uv1d.anova2onerm.SPM1D_ANOVA2ONERM_4x4()
-# dataset      = spm1d.data.uv1d.anova2onerm.SPM1D_ANOVA2ONERM_4x5()
+dataset      = spm1d.data.uv1d.anova2rm.SPM1D_ANOVA2RM_2x2()
+# dataset      = spm1d.data.uv1d.anova2rm.SPM1D_ANOVA2RM_2x3()
+# dataset      = spm1d.data.uv1d.anova2rm.SPM1D_ANOVA2RM_3x3()
+# dataset      = spm1d.data.uv1d.anova2rm.SPM1D_ANOVA2RM_3x4()
+# dataset      = spm1d.data.uv1d.anova2rm.SPM1D_ANOVA2RM_3x5()
+# dataset      = spm1d.data.uv1d.anova2rm.SPM1D_ANOVA2RM_4x4()
+# dataset      = spm1d.data.uv1d.anova2rm.SPM1D_ANOVA2RM_4x5()
 Y,A,B,SUBJ   = dataset.get_data()
 
 
 
 #(1) Conduct ANOVA:
 alpha        = 0.05
-FF           = spm1d.stats.anova2onerm(Y, A, B, SUBJ, equal_var=True)
+FF           = spm1d.stats.anova2rm(Y, A, B, SUBJ, equal_var=True)
 FFi          = FF.inference(0.05)
 print( FFi )
 
 
 
 #(2) Plot results:
-plt.close('all')
+pyplot.close('all')
 FFi.plot(plot_threshold_label=True, plot_p_values=True)
-plt.show()
+pyplot.show()
+
+
+
```

### Comparing `spm1d-0.4.19/spm1d/examples/stats1d/ex_anova3.py` & `spm1d-0.4.2/spm1d/examples/stats1d/ex_anova3nested.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 
 #(0) Load data:
-dataset      = spm1d.data.uv1d.anova3.SPM1D_ANOVA3_2x2x2()
-# dataset      = spm1d.data.uv1d.anova3.SPM1D_ANOVA3_2x3x4()
+# dataset      = spm1d.data.uv1d.anova3nested.SPM1D_ANOVA3NESTED_2x2x2()
+dataset      = spm1d.data.uv1d.anova3nested.SPM1D_ANOVA3NESTED_2x4x2()
 Y,A,B,C      = dataset.get_data()
 
 
 
 #(1) Conduct ANOVA:
 alpha        = 0.05
-FF           = spm1d.stats.anova3(Y, A, B, C, equal_var=True)
+FF           = spm1d.stats.anova3nested(Y, A, B, C, equal_var=True)
 FFi          = FF.inference(0.05)
 print( FFi )
 
 
 
 #(2) Plot results:
-plt.close('all')
+pyplot.close('all')
 FFi.plot(plot_threshold_label=True, plot_p_values=True, autoset_ylim=True)
-plt.show()
+pyplot.show()
+
+
```

### Comparing `spm1d-0.4.19/spm1d/examples/stats1d/ex_anova3onerm.py` & `spm1d-0.4.2/spm1d/examples/stats1d/ex_anova2.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,37 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 
 #(0) Load data:
-dataset      = spm1d.data.uv1d.anova3onerm.SPM1D_ANOVA3ONERM_2x2x2()
-# dataset      = spm1d.data.uv1d.anova3onerm.SPM1D_ANOVA3ONERM_2x3x4()
-Y,A,B,C,SUBJ = dataset.get_data()
+dataset      = spm1d.data.uv1d.anova2.SPM1D_ANOVA2_2x2()
+# dataset      = spm1d.data.uv1d.anova2.SPM1D_ANOVA2_2x3()
+# dataset      = spm1d.data.uv1d.anova2.SPM1D_ANOVA2_3x3()
+# dataset      = spm1d.data.uv1d.anova2.SPM1D_ANOVA2_3x4()
+# dataset      = spm1d.data.uv1d.anova2.SPM1D_ANOVA2_3x5()
+# dataset      = spm1d.data.uv1d.anova2.SPM1D_ANOVA2_4x4()
+# dataset      = spm1d.data.uv1d.anova2.SPM1D_ANOVA2_4x5()
+Y,A,B        = dataset.get_data()
 
 
 
 #(1) Conduct ANOVA:
 alpha        = 0.05
-FF           = spm1d.stats.anova3onerm(Y, A, B, C, SUBJ, equal_var=True)
-FFi          = FF.inference(0.05)
+FF           = spm1d.stats.anova2(Y, A, B, equal_var=True)
+FFi          = FF.inference(alpha)
 print( FFi )
 
 
 
 #(2) Plot results:
-plt.close('all')
-FFi.plot(plot_threshold_label=True, plot_p_values=True, autoset_ylim=True)
-plt.show()
+pyplot.close('all')
+FFi.plot(plot_threshold_label=True, plot_p_values=True)
+pyplot.show()
+
+
+
```

### Comparing `spm1d-0.4.19/spm1d/examples/stats1d/ex_anova3rm.py` & `spm1d-0.4.2/spm1d/examples/stats1d/ex_anova1.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 
-import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
+#(0) Load dataset:
+dataset      = spm1d.data.uv1d.anova1.SpeedGRFcategorical()
+dataset      = spm1d.data.uv1d.anova1.Weather()
+Y,A          = dataset.get_data()
 
-#(0) Load data:
-dataset      = spm1d.data.uv1d.anova3rm.SPM1D_ANOVA3RM_2x2x2()
-# dataset      = spm1d.data.uv1d.anova3rm.SPM1D_ANOVA3RM_2x3x4()
-Y,A,B,C,SUBJ = dataset.get_data()
 
 
+#(1) Run ANOVA:
+alpha        = 0.0005
+F            = spm1d.stats.anova1(Y, A, equal_var=False)
+Fi           = F.inference(alpha, interp=True, circular=False)
+print( Fi )
+### alternative syntax:
+# Y0,Y1,Y2     = [Y[A==u] for u in np.unique(A)]
+# F            = spm1d.stats.anova1((Y0,Y1,Y2), equal_var=False)
 
-#(1) Conduct ANOVA:
-alpha        = 0.05
-FF           = spm1d.stats.anova3rm(Y, A, B, C, SUBJ, equal_var=True)
-FFi          = FF.inference(0.05)
-print( FFi )
+
+#(2) Plot results:
+pyplot.close('all')
+Fi.plot()
+Fi.plot_threshold_label(bbox=dict(facecolor='w'))
+# pyplot.ylim(-1, 500)
+pyplot.xlabel('Time (%)', size=20)
+pyplot.title(r'Critical threshold at $\alpha$=%.2f:  $F^*$=%.3f' %(alpha, Fi.zstar))
+pyplot.show()
 
 
 
-#(2) Plot results:
-plt.close('all')
-FFi.plot(plot_threshold_label=True, plot_p_values=True, autoset_ylim=True)
-plt.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/stats1d/ex_anova3tworm.py` & `spm1d-0.4.2/spm1d/examples/stats1d/ex_anova3tworm.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 
 #(0) Load data:
 dataset      = spm1d.data.uv1d.anova3tworm.SPM1D_ANOVA3TWORM_2x2x2()
-#dataset      = spm1d.data.uv1d.anova3tworm.SPM1D_ANOVA3TWORM_2x3x4()
+dataset      = spm1d.data.uv1d.anova3tworm.SPM1D_ANOVA3TWORM_2x3x4()
 Y,A,B,C,SUBJ = dataset.get_data()
 
 
 
 #(1) Conduct ANOVA:
 alpha        = 0.05
 FF           = spm1d.stats.anova3tworm(Y, A, B, C, SUBJ, equal_var=True)
 FFi          = FF.inference(0.05)
 print( FFi )
 
 
 # #(2) Plot results:
-# plt.close('all')
+# pyplot.close('all')
 # for i,Fi in enumerate(FFi):
-# 	ax = plt.subplot(3,3,i+1)
+# 	ax = pyplot.subplot(3,3,i+1)
 # 	Fi.plot()
 # 	ax.text(0.1, 0.85, Fi.effect, transform=ax.transAxes)
-# plt.show()
+# pyplot.show()
 
 
 #(2) Plot results:
-plt.close('all')
+pyplot.close('all')
 FFi.plot(plot_threshold_label=True, plot_p_values=True, autoset_ylim=True)
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/stats1d/ex_ci_onesample.py` & `spm1d-0.4.2/spm1d/examples/stats1d/ex_ci_onesample.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 - Explicit null hypothesis testing is conducted
 - The null hypothesis is rejected if mu lies outside the CI at any point in the 1D field
 - A 0D scalar value for mu represents a constant 1D field
 '''
 
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 #(0) Load dataset:
 # dataset    = spm1d.data.uv1d.t1.Random()
 # dataset    = spm1d.data.uv1d.t1.SimulatedPataky2015a()
@@ -40,58 +40,58 @@
 ci1        = spm1d.stats.ci_onesample(y, alpha, mu=mu1)
 print( ci0 )
 print( ci1 )
 
 
 
 #(2) Plot the CIs:
-plt.close('all')
-plt.figure(figsize=(14,7))
+pyplot.close('all')
+pyplot.figure(figsize=(14,7))
 
 
 ### FIRST POPULATION MEAN
 
 ### plot means and SD:
-ax = plt.subplot(231)
+ax = pyplot.subplot(231)
 spm1d.plot.plot_mean_sd(y-mu0, ax=ax)
 ax.set_title('Mean and SD', size=10)
 spm1d.plot.legend_manual(ax, labels=['Mean', 'SD'], colors=['k','0.85'], linestyles=['-', '-'], linewidths=[3, 10], loc='upper left', fontsize=10)
 
 ### plot hypothesis test results:
-ax = plt.subplot(232)
+ax = pyplot.subplot(232)
 spmi = spm1d.stats.ttest(y, mu0).inference(alpha, two_tailed=True)
 spmi.plot(ax=ax)
 spmi.plot_p_values()
 ax.set_title('Hypothesis test', size=10)
 
 ### plot CIs:
-ax = plt.subplot(233)
+ax = pyplot.subplot(233)
 ci0.plot(ax)
 ax.set_title('CI  (criterion: mu=0)', size=10)
 spm1d.plot.legend_manual(ax, labels=['Mean', 'CI', 'Criterion'], colors=['k','0.85','r'], linestyles=['-', '-','--'], linewidths=[3, 10, 1], loc='upper left', fontsize=10)
 
 
 ### SECOND POPULATION MEAN
 
 ### plot means and SD:
-ax = plt.subplot(234)
+ax = pyplot.subplot(234)
 spm1d.plot.plot_mean_sd(y-mu1, ax=ax)
 ax.set_title('Mean and SD  (y - mu1)', size=10)
 
 ### plot hypothesis test results:
-ax = plt.subplot(235)
+ax = pyplot.subplot(235)
 spmi = spm1d.stats.ttest(y, mu1).inference(alpha, two_tailed=True)
 spmi.plot(ax=ax)
 spmi.plot_p_values()
 ax.set_title('Hypothesis test (y - mu1)', size=10)
 
 ### plot CIs:
-ax = plt.subplot(236)
+ax = pyplot.subplot(236)
 ci1.plot(ax)
 ax.set_title('CI  (criterion: mu1)', size=10)
 
 
-plt.suptitle('One-sample analysis')
-plt.show()
+pyplot.suptitle('One-sample analysis')
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/stats1d/ex_ci_onesample_standalone.py` & `spm1d-0.4.2/spm1d/examples/stats1d/ex_ci_onesample_standalone.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 from spm1d import rft1d
 
 
 
 
 
@@ -31,25 +31,25 @@
 
 #(2) Compare to spm1d result:
 ci_spm1d   = spm1d.stats.ci_onesample(y, alpha, mu)
 
 
 
 #(3) Plot the CIs:
-plt.close('all')
-plt.figure(figsize=(10,4))
+pyplot.close('all')
+pyplot.figure(figsize=(10,4))
 
 ### plot parametric CI:
-ax = plt.subplot(121)
+ax = pyplot.subplot(121)
 ax.plot(m, color='b', lw=3)
 ax.plot(ci[0], color='b', lw=1, linestyle=':')
 ax.plot(ci[1], color='b', lw=1, linestyle=':')
 ax.axhline(0, color='k', linestyle='--')
 ax.set_title('Manually computed CI', size=10)
 ax.set_ylim(-7, 13)
 ### plot parametric CI:
-ax = plt.subplot(122)
+ax = pyplot.subplot(122)
 ci_spm1d.plot(ax)
 ax.set_title('spm1d result', size=10)
-plt.suptitle('One-sample CIs')
+pyplot.suptitle('One-sample CIs')
 ax.set_ylim(-7, 13)
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/stats1d/ex_ci_pairedsample.py` & `spm1d-0.4.2/spm1d/examples/stats1d/ex_ci_pairedsample.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 #(0) Load dataset:
 dataset      = spm1d.data.uv1d.t2.PlantarArchAngle()
 yA,yB        = dataset.get_data()  #normal and fast walking
@@ -25,69 +25,69 @@
 ciA_bad    = spm1d.stats.ci_onesample(yA, alpha)
 ciB_bad    = spm1d.stats.ci_onesample(yB, alpha)
 
 
 
 
 #(2) Plot:
-plt.close('all')
-plt.figure(figsize=(14,7))
+pyplot.close('all')
+pyplot.figure(figsize=(14,7))
 
 
 
 ### plot means and standard deviations:
-ax     = plt.subplot(231)
+ax     = pyplot.subplot(231)
 spm1d.plot.plot_mean_sd(yA)
 spm1d.plot.plot_mean_sd(yB, linecolor='r', facecolor='r', edgecolor='r')
 spm1d.plot.legend_manual(ax, labels=['Group A', 'Group B', 'Mean', 'SD'], colors=['0.3', 'r', 'k','0.85'], linestyles=['-']*4, linewidths=[10, 10, 3, 10], loc='lower left', fontsize=10)
 ax.set_title('Means and SDs')
 
 
 
 ### plot hypothesis test results:
-ax     = plt.subplot(232)
+ax     = pyplot.subplot(232)
 spmi   = spm1d.stats.ttest_paired(yA, yB).inference(alpha, two_tailed=True)
 spmi.plot(ax=ax)
 spmi.plot_threshold_label()
 ax.set_title('Hypothesis test')
 ax.text(0.6, 0.2, 'Datum: zero\nCriterion:  $t ^*$', transform=ax.transAxes)
 
 
 
 
 ### plot confidence interval for mean paired difference:
-ax     = plt.subplot(233)
+ax     = pyplot.subplot(233)
 ci0.plot(ax=ax)
 ax.set_title('CI  (possibility 1)')
 ax.text(0.1, 0.8, 'Datum: difference\nCriterion: mu=0', transform=ax.transAxes)
 
 
 
 ### plot confidence interval for mean paired difference:
-ax     = plt.subplot(234)
+ax     = pyplot.subplot(234)
 ci1.plot(ax=ax)
 ax.set_title('CI  (possibility 2)')
 ax.text(0.1, 0.4, 'Datum: meanA\nCriterion: meanB', transform=ax.transAxes)
 
 
 ### plot confidence interval for mean paired difference:
-ax     = plt.subplot(235)
+ax     = pyplot.subplot(235)
 ci2.plot(ax=ax)
 ax.set_title('CI  (possibility 3)')
 ax.text(0.1, 0.4, 'Datum: meanA\nCriterion: tailsAB', transform=ax.transAxes)
 
 
 ### plot CIs computed separately for the means (INCORRECT!!!)
-ax     = plt.subplot(236)
+ax     = pyplot.subplot(236)
 ciA_bad.plot(ax=ax)
 ciB_bad.plot(ax=ax, linecolor='r', facecolor='r', edgecolor='r', alpha=0.3)
 ax.set_title('CIs computed separately for each group', size=10)
 ax.text(0.1, 0.4, 'INCORRECT!!!', transform=ax.transAxes)
 
 
 
 
 
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/stats1d/ex_ci_twosample.py` & `spm1d-0.4.2/spm1d/examples/stats1d/ex_ci_twosample.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 #(0) Load dataset:
 # dataset      = spm1d.data.uv1d.t2.PlantarArchAngle()
 dataset      = spm1d.data.uv1d.t2.SimulatedTwoLocalMax()
@@ -26,65 +26,65 @@
 
 
 
 
 
 
 #(2) Plot:
-plt.close('all')
-plt.figure(figsize=(14,7))
+pyplot.close('all')
+pyplot.figure(figsize=(14,7))
 
 
 
 ### plot means and standard deviations:
-ax     = plt.subplot(231)
+ax     = pyplot.subplot(231)
 spm1d.plot.plot_mean_sd(yA)
 spm1d.plot.plot_mean_sd(yB, linecolor='r', facecolor='r', edgecolor='r')
 ax.set_title('Means and SDs')
 
 
 
 ### plot hypothesis test results:
-ax     = plt.subplot(232)
+ax     = pyplot.subplot(232)
 spmi   = spm1d.stats.ttest2(yA, yB).inference(alpha, two_tailed=True)
 spmi.plot(ax=ax)
 spmi.plot_threshold_label()
 ax.set_title('Hypothesis test')
 ax.text(0.1, 0.2, 'Datum: zero\nCriterion:  $t ^*$', transform=ax.transAxes, bbox=dict(color='w', alpha=0.8))
 
 
 
 
 ### plot confidence interval for mean paired difference:
-ax     = plt.subplot(233)
+ax     = pyplot.subplot(233)
 ci0.plot(ax=ax)
 ax.set_title('CI  (possibility 1)')
 ax.text(0.1, 0.2, 'Datum: difference\nCriterion: mu=0', transform=ax.transAxes, bbox=dict(color='w', alpha=0.8))
 
 
 
 ### plot confidence interval for mean paired difference:
-ax     = plt.subplot(234)
+ax     = pyplot.subplot(234)
 ci1.plot(ax=ax)
 ax.set_title('CI  (possibility 2)')
 ax.text(0.1, 0.2, 'Datum: meanA\nCriterion: meanB', transform=ax.transAxes, bbox=dict(color='w', alpha=0.8))
 
 
 ### plot confidence interval for mean paired difference:
-ax     = plt.subplot(235)
+ax     = pyplot.subplot(235)
 ci2.plot(ax=ax)
 ax.set_title('CI  (possibility 3)')
 ax.text(0.1, 0.2, 'Datum: meanA\nCriterion: tailB', transform=ax.transAxes, bbox=dict(color='w', alpha=0.8))
 
 
 ### plot CIs computed separately for the means (INCORRECT!!!)
-ax     = plt.subplot(236)
+ax     = pyplot.subplot(236)
 ciA_bad.plot(ax=ax)
 ciB_bad.plot(ax=ax, linecolor='r', facecolor='r', edgecolor='r', alpha=0.3)
 ax.set_title('CIs computed separately for each group', size=10)
 ax.text(0.1, 0.2, 'INCORRECT!!!', transform=ax.transAxes, bbox=dict(color='w', alpha=0.8))
 
 
 
 
 
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/stats1d/ex_glm.py` & `spm1d-0.4.2/spm1d/examples/stats1d_roi/ex_glm.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 #(0) Load dataset:
 dataset    = spm1d.data.uv1d.regress.SpeedGRF()
 Y,x        = dataset.get_data()
 # specify design matrix:
@@ -15,23 +15,29 @@
 X[:,1]     = 1       #intercept
 X[:,2]     = np.linspace(0,1,nCurves)   #linear drift
 X[:,3]     = np.sin(np.linspace(0,np.pi,nCurves))  #sinusoidal drift
 # specify a contrast vector:
 c          = [1,0,0,0]  #speed (not the three other factors)
 
 
+#(0a) Create region of interest(ROI):
+roi        = np.array([False]*Y.shape[1])
+roi[60:]   = True
+
+
 
 #(1) Conduct general linear test:
 alpha      = 0.05
-t          = spm1d.stats.glm(Y, X, c)
+t          = spm1d.stats.glm(Y, X, c, roi=roi)
 ti         = t.inference(alpha, two_tailed=False, interp=True)
+print(ti)
 
 
 
 #(2) Plot:
-plt.close('all')
-ax     = plt.axes()
+pyplot.close('all')
+ax     = pyplot.axes()
 ti.plot()
 ti.plot_threshold_label(fontsize=8)
-ti.plot_p_values(size=10, offsets=[(0,0.3)])
+ti.plot_p_values(size=10)
 ax.set_xlabel('Time (%)')
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/stats1d/ex_hotellings_paired_Neptune1999.py` & `spm1d-0.4.2/spm1d/examples/stats1d_roi/ex_hotellings_paired_Pataky2014.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 
-import matplotlib.pyplot as plt
+import numpy as np
+from matplotlib import pyplot
 import spm1d
 
 
 
 #(0) Load data:
-dataset      = spm1d.data.mv1d.hotellings_paired.Neptune1999kneekin()
-YA,YB        = dataset.get_data()  #A:foot, B:speed
+dataset      = spm1d.data.mv1d.hotellings_paired.Pataky2014cop()
+YA,YB        = dataset.get_data()  #A:slow, B:fast
 print( dataset )
 
 
 
+#(0a) Create region of interest(ROI):
+roi        = np.array([False]*YA.shape[1])
+roi[50:80] = True
+
+
+
 #(1) Conduct test:
 alpha        = 0.05
-T2           = spm1d.stats.hotellings_paired(YA, YB)
+T2           = spm1d.stats.hotellings_paired(YA, YB, roi=roi)
 T2i          = T2.inference(0.05)
 
 
 
 #(2) Plot:
-plt.close('all')
-ax0     = plt.subplot(221)
-ax1     = plt.subplot(222)
-ax2     = plt.subplot(223)
-ax3     = plt.subplot(224)
-### plot SPM results:
-h=ax0.plot(YA[:,:,0].T, 'k'); h[0].set_label('side-shuffle')
-h=ax0.plot(YB[:,:,0].T, 'r'); h[0].set_label('v-cut')
+pyplot.close('all')
+ax0     = pyplot.subplot(221)
+ax1     = pyplot.subplot(222)
+ax3     = pyplot.subplot(224)
+## plot SPM results:
+ax0.plot(YA[:,:,0].T, 'k', label='slow')
+ax0.plot(YB[:,:,0].T, 'r', label='fast')
 ax1.plot(YA[:,:,1].T, 'k')
 ax1.plot(YB[:,:,1].T, 'r')
-ax2.plot(YA[:,:,2].T, 'k')
-ax2.plot(YB[:,:,2].T, 'r')
 T2i.plot(ax=ax3)
-ax0.legend(fontsize=9)
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/stats1d/ex_hotellings_paired_Pataky2014.py` & `spm1d-0.4.2/spm1d/examples/stats1d/ex_hotellings_paired_Pataky2014.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 #(0) Load data:
 dataset      = spm1d.data.mv1d.hotellings_paired.Pataky2014cop()
 YA,YB        = dataset.get_data()  #A:slow, B:fast
@@ -15,20 +15,20 @@
 alpha        = 0.05
 T2           = spm1d.stats.hotellings_paired(YA, YB)
 T2i          = T2.inference(0.05)
 print(T2i)
 
 
 #(2) Plot:
-plt.close('all')
-ax0     = plt.subplot(221)
-ax1     = plt.subplot(222)
-ax3     = plt.subplot(224)
+pyplot.close('all')
+ax0     = pyplot.subplot(221)
+ax1     = pyplot.subplot(222)
+ax3     = pyplot.subplot(224)
 ## plot SPM results:
 ax0.plot(YA[:,:,0].T, 'k', label='slow')
 ax0.plot(YB[:,:,0].T, 'r', label='fast')
 ax1.plot(YA[:,:,1].T, 'k')
 ax1.plot(YB[:,:,1].T, 'r')
 T2i.plot(ax=ax3)
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/stats1d/ex_regression.py` & `spm1d-0.4.2/spm1d/examples/stats1d/ex_regression.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 #(0) Load dataset:
-# dataset    = spm1d.data.uv1d.regress.SimulatedPataky2015c()
-dataset    = spm1d.data.uv1d.regress.SpeedGRF()
+dataset    = spm1d.data.uv1d.regress.SimulatedPataky2015c()
+# dataset    = spm1d.data.uv1d.regress.SpeedGRF()
 Y,x        = dataset.get_data()
 
 
 
 #(1) Conduct regression:
 alpha      = 0.05
 t          = spm1d.stats.regress(Y, x)
 ti         = t.inference(alpha, two_tailed=False, interp=True)
 
 
 
 #(2) Plot:
-plt.close('all')
-ax     = plt.axes()
+pyplot.close('all')
+ax     = pyplot.axes()
 ti.plot()
 ti.plot_threshold_label(fontsize=8)
 ti.plot_p_values(size=10, offsets=[(0,0.3)])
 ax.set_xlabel('Time (%)')
-plt.tight_layout()
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/stats1d/ex_ttest.py` & `spm1d-0.4.2/spm1d/examples/stats1d/ex_ttest.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,36 @@
 
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 #(0) Load dataset:
-dataset    = spm1d.data.uv1d.t1.Random()
+# dataset    = spm1d.data.uv1d.t1.Random()
 # dataset    = spm1d.data.uv1d.t1.SimulatedPataky2015a()
-# dataset    = spm1d.data.uv1d.t1.SimulatedPataky2015b()
+dataset    = spm1d.data.uv1d.t1.SimulatedPataky2015b()
 Y,mu       = dataset.get_data()
 
 
 #(1) Conduct t test:
 alpha      = 0.05
-spm        = spm1d.stats.ttest(Y, mu)
-spmi       = spm.inference(alpha, two_tailed=False, interp=True, circular=False)
-print( spmi )
+t          = spm1d.stats.ttest(Y, mu)
+ti         = t.inference(alpha, two_tailed=False, interp=True, circular=False)
+print( ti )
 
 
 
 #(2) Plot:
-plt.close('all')
+pyplot.close('all')
 ### plot mean and SD:
-fig,AX = plt.subplots( 1, 2, figsize=(8, 3.5) )
-ax     = AX[0]
-plt.sca(ax)
+pyplot.figure( figsize=(8, 3.5) )
+ax     = pyplot.axes( (0.1, 0.15, 0.35, 0.8) )
 spm1d.plot.plot_mean_sd(Y)
 ax.axhline(y=0, color='k', linestyle=':')
 ax.set_xlabel('Measurement domain (%)')
 ax.set_ylabel('Dependent Variable')
 ### plot SPM results:
-ax     = AX[1]
-plt.sca(ax)
-spmi.plot()
-spmi.plot_threshold_label(fontsize=8)
-spmi.plot_p_values(size=10, offsets=[(0,0.3)])
+ax     = pyplot.axes((0.55,0.15,0.35,0.8))
+ti.plot()
+ti.plot_threshold_label(fontsize=8)
+ti.plot_p_values(size=10, offsets=[(0,0.3)])
 ax.set_xlabel('Measurement domain (%)')
-plt.tight_layout()
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/stats1d/ex_ttest2.py` & `spm1d-0.4.2/spm1d/examples/stats1d/ex_ttest2.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,38 @@
 
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 #(0) Load data:
 dataset      = spm1d.data.uv1d.t2.PlantarArchAngle()
-# dataset      = spm1d.data.uv1d.t2.SimulatedTwoLocalMax()
+dataset      = spm1d.data.uv1d.t2.SimulatedTwoLocalMax()
 YA,YB        = dataset.get_data()
 
 
 
 #(1) Conduct t test:
 alpha      = 0.05
 t          = spm1d.stats.ttest2(YB, YA, equal_var=True)
-ti         = t.inference(alpha, two_tailed=True, interp=True)
+ti         = t.inference(alpha, two_tailed=False, interp=True)
 print( ti )
 
 
 
 #(2) Plot:
-plt.close('all')
+pyplot.close('all')
 ### plot mean and SD:
-fig,AX = plt.subplots( 1, 2, figsize=(8, 3.5) )
-ax     = AX[0]
-plt.sca(ax)
+pyplot.figure( figsize=(8, 3.5) )
+ax     = pyplot.axes( (0.1, 0.15, 0.35, 0.8) )
 spm1d.plot.plot_mean_sd(YA)
 spm1d.plot.plot_mean_sd(YB, linecolor='r', facecolor='r')
 ax.axhline(y=0, color='k', linestyle=':')
 ax.set_xlabel('Time (%)')
 ax.set_ylabel('Plantar arch angle  (deg)')
 ### plot SPM results:
-ax     = AX[1]
-plt.sca(ax)
+ax     = pyplot.axes((0.55,0.15,0.35,0.8))
 ti.plot()
 ti.plot_threshold_label(fontsize=8)
 ti.plot_p_values(size=10, offset_all_clusters=(0,0.9))
 ax.set_xlabel('Time (%)')
-plt.tight_layout()
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/stats1d/ex_ttest_paired.py` & `spm1d-0.4.2/spm1d/examples/stats1d_roi/ex_ttest_paired.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,44 @@
 
-import matplotlib.pyplot as plt
+import numpy as np
+from matplotlib import pyplot
 import spm1d
 
 
 
 #(0) Load data:
-dataset    = spm1d.data.uv1d.t2.PlantarArchAngle()
-YA,YB      = dataset.get_data()  #normal and fast walking
+dataset      = spm1d.data.uv1d.t2.PlantarArchAngle()
+YA,YB        = dataset.get_data()  #normal and fast walking
+
+
+#(0a) Create region of interest(ROI):
+roi        = np.array([False]*YA.shape[1])
+roi[0:10]  = True
+
 
 
 
 #(1) Conduct t test:
-spm        = spm1d.stats.ttest_paired(YA, YB)
-spmi       = spm.inference(0.05, two_tailed=False, interp=True)
-print( spmi )
+alpha      = 0.05
+t          = spm1d.stats.ttest_paired(YA, YB, roi=roi)
+ti         = t.inference(alpha, two_tailed=False, interp=True)
 
 
 
 #(2) Plot:
-plt.close('all')
+pyplot.close('all')
 ### plot mean and SD:
-fig,AX = plt.subplots( 1, 2, figsize=(8, 3.5) )
-ax     = AX[0]
-plt.sca(ax)
+pyplot.figure( figsize=(8, 3.5) )
+ax     = pyplot.axes( (0.1, 0.15, 0.35, 0.8) )
 spm1d.plot.plot_mean_sd(YA)
 spm1d.plot.plot_mean_sd(YB, linecolor='r', facecolor='r')
+spm1d.plot.plot_roi(roi, facecolor='b', alpha=0.3)
 ax.axhline(y=0, color='k', linestyle=':')
 ax.set_xlabel('Time (%)')
 ax.set_ylabel('Plantar arch angle  (deg)')
 ### plot SPM results:
-ax     = AX[1]
-plt.sca(ax)
-spmi.plot()
-spmi.plot_threshold_label(fontsize=8)
-spmi.plot_p_values(size=10, offsets=[(0,0.3)])
+ax     = pyplot.axes((0.55,0.15,0.35,0.8))
+ti.plot()
+ti.plot_threshold_label(fontsize=8)
+ti.plot_p_values(size=10, offsets=[(0,0.3)])
 ax.set_xlabel('Time (%)')
-plt.tight_layout()
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/stats1d/ex_ttest_roi.py` & `spm1d-0.4.2/spm1d/examples/stats1d/ex_ttest_roi.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 #(0) Load dataset:
 dataset    = spm1d.data.uv1d.t1.Random()
 dataset    = spm1d.data.uv1d.t1.SimulatedPataky2015a()
 # dataset    = spm1d.data.uv1d.t1.SimulatedPataky2015b()
@@ -15,25 +15,22 @@
 t          = spm1d.stats.ttest(Y, mu)
 ti         = t.inference(alpha, two_tailed=False, interp=True)
 
 
 
 
 #(2) Plot:
-plt.close('all')
+pyplot.close('all')
 ### plot mean and SD:
-fig,AX = plt.subplots( 1, 2, figsize=(8, 3.5) )
-ax     = AX[0]
-plt.sca(ax)
+pyplot.figure( figsize=(8, 3.5) )
+ax     = pyplot.axes( (0.1, 0.15, 0.35, 0.8) )
 spm1d.plot.plot_mean_sd(Y)
 ax.axhline(y=0, color='k', linestyle=':')
 ax.set_xlabel('Measurement domain (%)')
 ax.set_ylabel('Dependent Variable')
 ### plot SPM results:
-ax     = AX[1]
-plt.sca(ax)
+ax     = pyplot.axes((0.55,0.15,0.35,0.8))
 ti.plot()
 ti.plot_threshold_label(fontsize=8)
 ti.plot_p_values(size=10, offsets=[(0,0.3)])
 ax.set_xlabel('Measurement domain (%)')
-plt.tight_layout()
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/stats1d/rfx_0_means.py` & `spm1d-0.4.2/spm1d/examples/stats1d/rfx_0_means.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 # compute within-speed means for each subject:
 nSubj        = 10
 Y1,Y2,Y3     = [], [], []
@@ -17,19 +17,18 @@
 	Y1.append(  y1.mean(axis=0)  )
 	Y2.append(  y2.mean(axis=0)  )
 	Y3.append(  y3.mean(axis=0)  )
 Y1,Y2,Y3     = np.asarray(Y1), np.asarray(Y2), np.asarray(Y3)
 
 
 # plot:
-plt.close('all')
-h1 = plt.plot(Y1.T, color='b')
-h2 = plt.plot(Y2.T, color='k')
-h3 = plt.plot(Y3.T, color='r')
+pyplot.close('all')
+h1 = pyplot.plot(Y1.T, color='b')
+h2 = pyplot.plot(Y2.T, color='k')
+h3 = pyplot.plot(Y3.T, color='r')
 h1[0].set_label('Slow')
 h2[0].set_label('Normal')
 h3[0].set_label('Fast')
-plt.legend(loc='lower center', fontsize=12)
-plt.xlabel('Time (% stance)')
-plt.ylabel('GRF (BW)')
-plt.tight_layout()
-plt.show()
+pyplot.legend(loc='lower center', fontsize=12)
+pyplot.xlabel('Time (% stance)')
+pyplot.ylabel('GRF (BW)')
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/stats1d/rfx_1_level1.py` & `spm1d-0.4.2/spm1d/examples/stats1d/rfx_1_level1.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 
 
 
@@ -16,16 +16,15 @@
 	Y,x       = dataset.get_data()
 	t         = spm1d.stats.regress(Y, x) #conduct linear regression
 	BETA.append( t.beta[0] )  #retrieve the regression slope
 BETA          = np.array(BETA)
 
 
 #plot:
-plt.close('all')
-ax            = plt.axes( (0.15, 0.15, 0.8, 0.8) )
-plt.plot(BETA.T, color='k')
+pyplot.close('all')
+ax            = pyplot.axes( (0.15, 0.15, 0.8, 0.8) )
+pyplot.plot(BETA.T, color='k')
 ax.axhline(y=0, color='k', linewidth=1, linestyle=':')
 ax.set_xlabel('Time (% stance)')
 ax.set_ylabel(r'$\beta_0$   $(BW / ms^{-1})$')
-plt.tight_layout()
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/stats1d/rfx_2_level2.py` & `spm1d-0.4.2/spm1d/examples/stats1d/rfx_2_level2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 #first-level SPM analysis: (within-subject effects)
 nSubj         = 10
 BETA          = []  #regression slopes
@@ -19,14 +19,13 @@
 #second-level SPM analysis:  (between-subject random effects)
 alpha         = 0.05
 t             = spm1d.stats.ttest(BETA)
 ti            = t.inference(alpha, two_tailed=True)
 
 
 #plot:
-plt.close('all')
+pyplot.close('all')
 ti.plot()
 ti.plot_threshold_label(fontsize=12)
 ti.plot_p_values()
-plt.xlabel('Time (% stance)', size=16)
-plt.tight_layout()
-plt.show()
+pyplot.xlabel('Time (% stance)', size=16)
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/stats1d_roi/ex_anova1rm.py` & `spm1d-0.4.2/spm1d/examples/stats1d_roi/ex_anova1rm.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 #(0) Load dataset:
 dataset      = spm1d.data.uv1d.anova1rm.SpeedGRFcategoricalRM()
 Y,A,SUBJ     = dataset.get_data()
@@ -25,25 +25,25 @@
 Fi           = F.inference(alpha)
 Firm         = Frm.inference(alpha)
 
 
 
 
 #(2) Plot:
-plt.close('all')
-plt.figure( figsize=(8, 3.5) )
-ax0     = plt.axes( (0.1, 0.15, 0.35, 0.8) )
-ax1     = plt.axes((0.55,0.15,0.35,0.8))
+pyplot.close('all')
+pyplot.figure( figsize=(8, 3.5) )
+ax0     = pyplot.axes( (0.1, 0.15, 0.35, 0.8) )
+ax1     = pyplot.axes((0.55,0.15,0.35,0.8))
 ### plot mean subject trajectories:
 ax0.plot(Y[A==0].T, 'b')
 ax0.plot(Y[A==1].T, 'k')
 ax0.plot(Y[A==2].T, 'r')
 ### plot SPM results:
 Firm.plot(ax=ax1, color='r', facecolor=(0.8,0.3,0.3), label='Within-subjects analysis')
 Fi.plot(ax=ax1, label='Between-subjects analysis')
 ax1.legend(fontsize=8)
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/stats1d_roi/ex_anova2.py` & `spm1d-0.4.2/spm1d/examples/stats1d_roi/ex_anova2onerm.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 
 #(0) Load data:
-dataset      = spm1d.data.uv1d.anova2.SPM1D_ANOVA2_2x2()
-Y,A,B        = dataset.get_data()
+dataset      = spm1d.data.uv1d.anova2onerm.SPM1D_ANOVA2ONERM_2x3()
+Y,A,B,SUBJ   = dataset.get_data()
 
 
 #(0a) Create region of interest(ROI):
 roi        = np.array([False]*Y.shape[1])
-roi[60:80] = True
+roi[60:]   = True
 
 
 
 #(1) Conduct ANOVA:
 alpha        = 0.05
-FF           = spm1d.stats.anova2(Y, A, B, equal_var=True, roi=roi)
-FFi          = [F.inference(alpha)   for F in FF]
+FF           = spm1d.stats.anova2onerm(Y, A, B, SUBJ, equal_var=True, roi=roi)
+FFi          = [F.inference(alpha, interp=True)   for F in FF]
 
 
 #(2) Plot results:
-plt.close('all')
-plt.subplot(221);  FFi[0].plot();  plt.title('Main effect A')
-plt.subplot(222);  FFi[1].plot();  plt.title('Main effect B')
-plt.subplot(223);  FFi[2].plot();  plt.title('Interaction effect AB')
-plt.show()
+pyplot.close('all')
+pyplot.subplot(221);  FFi[0].plot();  pyplot.title('Main effect A')
+pyplot.subplot(222);  FFi[1].plot();  pyplot.title('Main effect B')
+pyplot.subplot(223);  FFi[2].plot();  pyplot.title('Interaction effect AB')
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/stats1d_roi/ex_anova2nested.py` & `spm1d-0.4.2/spm1d/examples/stats1d_roi/ex_anova2nested.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 
 #(0) Load data:
 dataset      = spm1d.data.uv1d.anova2nested.SPM1D_ANOVA2NESTED_2x2()
@@ -20,16 +20,16 @@
 #(1) Conduct ANOVA:
 alpha        = 0.05
 FF           = spm1d.stats.anova2nested(Y, A, B, equal_var=True, roi=roi)
 FFi          = [F.inference(alpha, interp=True)   for F in FF]
 
 
 #(2) Plot results:
-plt.close('all')
-plt.subplot(221);  FFi[0].plot();  plt.title('Main effect A')
-plt.subplot(222);  FFi[1].plot();  plt.title('Main effect B')
-plt.show()
+pyplot.close('all')
+pyplot.subplot(221);  FFi[0].plot();  pyplot.title('Main effect A')
+pyplot.subplot(222);  FFi[1].plot();  pyplot.title('Main effect B')
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/stats1d_roi/ex_anova2onerm.py` & `spm1d-0.4.2/spm1d/examples/stats1d_roi/ex_anova2rm.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 
 #(0) Load data:
-dataset      = spm1d.data.uv1d.anova2onerm.SPM1D_ANOVA2ONERM_2x3()
+dataset      = spm1d.data.uv1d.anova2rm.SPM1D_ANOVA2RM_2x2()
 Y,A,B,SUBJ   = dataset.get_data()
 
 
 #(0a) Create region of interest(ROI):
 roi        = np.array([False]*Y.shape[1])
-roi[60:]   = True
-
+roi[:20]   = True
 
 
 #(1) Conduct ANOVA:
 alpha        = 0.05
-FF           = spm1d.stats.anova2onerm(Y, A, B, SUBJ, equal_var=True, roi=roi)
+FF           = spm1d.stats.anova2rm(Y, A, B, SUBJ, equal_var=True, roi=roi)
 FFi          = [F.inference(alpha, interp=True)   for F in FF]
 
 
 #(2) Plot results:
-plt.close('all')
-plt.subplot(221);  FFi[0].plot();  plt.title('Main effect A')
-plt.subplot(222);  FFi[1].plot();  plt.title('Main effect B')
-plt.subplot(223);  FFi[2].plot();  plt.title('Interaction effect AB')
-plt.show()
+pyplot.close('all')
+pyplot.subplot(221);  FFi[0].plot();  pyplot.title('Main effect A')
+pyplot.subplot(222);  FFi[1].plot();  pyplot.title('Main effect B')
+pyplot.subplot(223);  FFi[2].plot();  pyplot.title('Interaction effect AB')
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/stats1d_roi/ex_anova3.py` & `spm1d-0.4.2/spm1d/examples/stats1d_roi/ex_anova3rm.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,45 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 
 #(0) Load data:
-dataset      = spm1d.data.uv1d.anova3.SPM1D_ANOVA3_2x2x2()
-Y,A,B,C      = dataset.get_data()
+dataset      = spm1d.data.uv1d.anova3rm.SPM1D_ANOVA3RM_2x2x2()
+Y,A,B,C,SUBJ = dataset.get_data()
 
 
 
 #(0a) Create region of interest(ROI):
 roi        = np.array([False]*Y.shape[1])
-roi[60:]   = True
-
+roi[40:75] = True
 
 
 #(1) Conduct ANOVA:
 alpha        = 0.05
-FF           = spm1d.stats.anova3(Y, A, B, C, equal_var=True, roi=roi)
+FF           = spm1d.stats.anova3rm(Y, A, B, C, SUBJ, equal_var=True, roi=roi)
 FFi          = [F.inference(alpha)   for F in FF]
 
 
 #(2) Plot results:
-plt.close('all')
-plt.figure(figsize=(12,8))
+pyplot.close('all')
 titles       = ['Main effect A',
                'Main effect B',
                'Main effect C',
                'Interaction AB',
                'Interaction AC',
                'Interaction BC',
                'Interaction ABC',
 ]
 for i,Fi in enumerate(FFi):
-	ax = plt.subplot(3,3,i+1)
+	ax = pyplot.subplot(3,3,i+1)
 	Fi.plot()
 	ax.text(0.1, 0.85, titles[i], transform=ax.transAxes)
-plt.tight_layout()
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/stats1d_roi/ex_anova3nested.py` & `spm1d-0.4.2/spm1d/examples/stats1d_roi/ex_anova3nested.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 
 #(0) Load data:
 dataset      = spm1d.data.uv1d.anova3nested.SPM1D_ANOVA3NESTED_2x2x2()
@@ -21,23 +21,22 @@
 #(1) Conduct ANOVA:
 alpha        = 0.05
 FF           = spm1d.stats.anova3nested(Y, A, B, C, equal_var=True, roi=roi)
 FFi          = [F.inference(alpha, interp=True)   for F in FF]
 
 
 #(2) Plot results:
-plt.close('all')
+pyplot.close('all')
 titles       = ['Main effect A',
                'Main effect B',
                'Main effect C',
 ]
 for i,Fi in enumerate(FFi):
-	ax = plt.subplot(2,2,i+1)
+	ax = pyplot.subplot(2,2,i+1)
 	Fi.plot()
 	ax.text(0.1, 0.85, titles[i], transform=ax.transAxes)
-plt.tight_layout()
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/stats1d_roi/ex_anova3onerm.py` & `spm1d-0.4.2/spm1d/examples/stats1d_roi/ex_anova3onerm.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 
 #(0) Load data:
 dataset      = spm1d.data.uv1d.anova3onerm.SPM1D_ANOVA3ONERM_2x2x2()
@@ -21,28 +21,26 @@
 #(1) Conduct ANOVA:
 alpha        = 0.05
 FF           = spm1d.stats.anova3onerm(Y, A, B, C, SUBJ, equal_var=True, roi=roi)
 FFi          = [F.inference(alpha)   for F in FF]
 
 
 #(2) Plot results:
-plt.close('all')
-plt.figure(figsize=(12,8))
+pyplot.close('all')
 titles       = ['Main effect A',
                'Main effect B',
                'Main effect C',
                'Interaction AB',
                'Interaction AC',
                'Interaction BC',
                'Interaction ABC',
 ]
 for i,Fi in enumerate(FFi):
-	ax = plt.subplot(3,3,i+1)
+	ax = pyplot.subplot(3,3,i+1)
 	Fi.plot()
 	ax.text(0.1, 0.85, titles[i], transform=ax.transAxes)
-plt.tight_layout()
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/stats1d_roi/ex_anova3rm.py` & `spm1d-0.4.2/spm1d/examples/stats1d_roi/ex_anova3tworm.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,47 +1,45 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 
 #(0) Load data:
-dataset      = spm1d.data.uv1d.anova3rm.SPM1D_ANOVA3RM_2x2x2()
+dataset      = spm1d.data.uv1d.anova3tworm.SPM1D_ANOVA3TWORM_2x2x2()
 Y,A,B,C,SUBJ = dataset.get_data()
 
 
 
 #(0a) Create region of interest(ROI):
 roi        = np.array([False]*Y.shape[1])
-roi[40:75] = True
+roi[40:]   = True
 
 
 #(1) Conduct ANOVA:
 alpha        = 0.05
-FF           = spm1d.stats.anova3rm(Y, A, B, C, SUBJ, equal_var=True, roi=roi)
+FF           = spm1d.stats.anova3tworm(Y, A, B, C, SUBJ, equal_var=True, roi=roi)
 FFi          = [F.inference(alpha)   for F in FF]
 
 
 #(2) Plot results:
-plt.close('all')
-plt.figure(figsize=(12,8))
+pyplot.close('all')
 titles       = ['Main effect A',
                'Main effect B',
                'Main effect C',
                'Interaction AB',
                'Interaction AC',
                'Interaction BC',
                'Interaction ABC',
 ]
 for i,Fi in enumerate(FFi):
-	ax = plt.subplot(3,3,i+1)
+	ax = pyplot.subplot(3,3,i+1)
 	Fi.plot()
 	ax.text(0.1, 0.85, titles[i], transform=ax.transAxes)
-plt.tight_layout()
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/stats1d_roi/ex_anova3tworm.py` & `spm1d-0.4.2/spm1d/examples/stats1d_roi/ex_anova3.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,46 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 
 #(0) Load data:
-dataset      = spm1d.data.uv1d.anova3tworm.SPM1D_ANOVA3TWORM_2x2x2()
-Y,A,B,C,SUBJ = dataset.get_data()
+dataset      = spm1d.data.uv1d.anova3.SPM1D_ANOVA3_2x2x2()
+Y,A,B,C      = dataset.get_data()
 
 
 
 #(0a) Create region of interest(ROI):
 roi        = np.array([False]*Y.shape[1])
-roi[40:]   = True
+roi[60:]   = True
+
 
 
 #(1) Conduct ANOVA:
 alpha        = 0.05
-FF           = spm1d.stats.anova3tworm(Y, A, B, C, SUBJ, equal_var=True, roi=roi)
+FF           = spm1d.stats.anova3(Y, A, B, C, equal_var=True, roi=roi)
 FFi          = [F.inference(alpha)   for F in FF]
 
 
 #(2) Plot results:
-plt.close('all')
-plt.figure(figsize=(12,8))
+pyplot.close('all')
 titles       = ['Main effect A',
                'Main effect B',
                'Main effect C',
                'Interaction AB',
                'Interaction AC',
                'Interaction BC',
                'Interaction ABC',
 ]
 for i,Fi in enumerate(FFi):
-	ax = plt.subplot(3,3,i+1)
+	ax = pyplot.subplot(3,3,i+1)
 	Fi.plot()
 	ax.text(0.1, 0.85, titles[i], transform=ax.transAxes)
-plt.tight_layout()
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/stats1d_roi/ex_cca_Dorn2012.py` & `spm1d-0.4.2/spm1d/examples/stats1d_roi/ex_cca_Dorn2012.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 #(0) Load dataset:
 dataset      = spm1d.data.mv1d.cca.Dorn2012()
 Y,x          = dataset.get_data()  #A:slow, B:fast
@@ -23,14 +23,14 @@
 alpha        = 0.05
 X2           = spm1d.stats.cca(Y, x, roi=roi)
 X2i          = X2.inference(0.05)
 print( X2i )
 
 
 #(2) Plot:
-plt.close('all')
+pyplot.close('all')
 # X2.plot()
 X2i.plot()
 X2i.plot_p_values()
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/stats1d_roi/ex_glm.py` & `spm1d-0.4.2/spm1d/examples/stats1d/ex_glm.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 #(0) Load dataset:
 dataset    = spm1d.data.uv1d.regress.SpeedGRF()
 Y,x        = dataset.get_data()
 # specify design matrix:
@@ -15,29 +15,23 @@
 X[:,1]     = 1       #intercept
 X[:,2]     = np.linspace(0,1,nCurves)   #linear drift
 X[:,3]     = np.sin(np.linspace(0,np.pi,nCurves))  #sinusoidal drift
 # specify a contrast vector:
 c          = [1,0,0,0]  #speed (not the three other factors)
 
 
-#(0a) Create region of interest(ROI):
-roi        = np.array([False]*Y.shape[1])
-roi[60:]   = True
-
-
 
 #(1) Conduct general linear test:
 alpha      = 0.05
-t          = spm1d.stats.glm(Y, X, c, roi=roi)
+t          = spm1d.stats.glm(Y, X, c)
 ti         = t.inference(alpha, two_tailed=False, interp=True)
-print(ti)
 
 
 
 #(2) Plot:
-plt.close('all')
-ax     = plt.axes()
+pyplot.close('all')
+ax     = pyplot.axes()
 ti.plot()
 ti.plot_threshold_label(fontsize=8)
-ti.plot_p_values(size=10)
+ti.plot_p_values(size=10, offsets=[(0,0.3)])
 ax.set_xlabel('Time (%)')
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/stats1d_roi/ex_hotellings_paired_Neptune1999.py` & `spm1d-0.4.2/spm1d/examples/stats1d_roi/ex_hotellings_paired_Neptune1999.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 #(0) Load data:
 dataset      = spm1d.data.mv1d.hotellings_paired.Neptune1999kneekin()
 YA,YB        = dataset.get_data()  #A:foot, B:speed
@@ -23,24 +23,24 @@
 T2           = spm1d.stats.hotellings_paired(YA, YB, roi=roi)
 T2i          = T2.inference(0.05)
 print(T2i)
 
 
 
 #(2) Plot:
-plt.close('all')
-ax0     = plt.subplot(221)
-ax1     = plt.subplot(222)
-ax2     = plt.subplot(223)
-ax3     = plt.subplot(224)
+pyplot.close('all')
+ax0     = pyplot.subplot(221)
+ax1     = pyplot.subplot(222)
+ax2     = pyplot.subplot(223)
+ax3     = pyplot.subplot(224)
 ### plot SPM results:
 h=ax0.plot(YA[:,:,0].T, 'k'); h[0].set_label('side-shuffle')
 h=ax0.plot(YB[:,:,0].T, 'r'); h[0].set_label('v-cut')
 ax1.plot(YA[:,:,1].T, 'k')
 ax1.plot(YB[:,:,1].T, 'r')
 ax2.plot(YA[:,:,2].T, 'k')
 ax2.plot(YB[:,:,2].T, 'r')
 T2i.plot(ax=ax3)
 ax0.legend(fontsize=9)
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/stats1d_roi/ex_ttest.py` & `spm1d-0.4.2/spm1d/examples/stats1d_roi/ex_ttest.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 #(0) Load dataset:
 dataset    = spm1d.data.uv1d.t1.SimulatedPataky2015a()
 Y,mu       = dataset.get_data()
 
@@ -18,22 +18,22 @@
 #(1) Conduct t test:
 alpha      = 0.05
 t          = spm1d.stats.ttest(Y, mu, roi=roi)
 ti         = t.inference(alpha, two_tailed=False, interp=True)
 
 
 #(2) Plot:
-plt.close('all')
-plt.figure( figsize=(8, 3.5) )
+pyplot.close('all')
+pyplot.figure( figsize=(8, 3.5) )
 ### plot mean and SD:
-ax     = plt.axes( (0.1, 0.15, 0.35, 0.8) )
+ax     = pyplot.axes( (0.1, 0.15, 0.35, 0.8) )
 spm1d.plot.plot_mean_sd(Y, roi=roi)
 ax.axhline(y=0, color='k', linestyle=':')
 ax.set_xlabel('Measurement domain (%)')
 ax.set_ylabel('Dependent Variable')
 ### plot SPM results:
-ax     = plt.axes((0.55,0.15,0.35,0.8))
+ax     = pyplot.axes((0.55,0.15,0.35,0.8))
 ti.plot()
 ti.plot_threshold_label(fontsize=8)
 ti.plot_p_values(size=10, offsets=[(0,0.3)])	
 ax.set_xlabel('Measurement domain (%)')
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/stats1d_roi/ex_ttest2.py` & `spm1d-0.4.2/spm1d/examples/stats1d_roi/ex_ttest2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 #(0) Load data:
 dataset      = spm1d.data.uv1d.t2.SimulatedTwoLocalMax()
 YA,YB        = dataset.get_data()
@@ -23,23 +23,23 @@
 t          = spm1d.stats.ttest2(YB, YA, equal_var=True, roi=roi)
 ti         = t.inference(alpha, two_tailed=False, interp=True)
 print( ti )
 
 
 
 #(2) Plot:
-plt.close('all')
+pyplot.close('all')
 ### plot mean and SD:
-plt.figure( figsize=(8, 3.5) )
-ax     = plt.axes( (0.1, 0.15, 0.35, 0.8) )
+pyplot.figure( figsize=(8, 3.5) )
+ax     = pyplot.axes( (0.1, 0.15, 0.35, 0.8) )
 spm1d.plot.plot_mean_sd(YA, roi=roi)
 spm1d.plot.plot_mean_sd(YB, linecolor='r', facecolor='r', roi=roi)
 ax.axhline(y=0, color='k', linestyle=':')
 ax.set_xlabel('Time (%)')
 ax.set_ylabel('Plantar arch angle  (deg)')
 ### plot SPM results:
-ax     = plt.axes((0.55,0.15,0.35,0.8))
+ax     = pyplot.axes((0.55,0.15,0.35,0.8))
 ti.plot()
 ti.plot_threshold_label(fontsize=8)
 ti.plot_p_values(size=10, offset_all_clusters=(0,0.9))
 ax.set_xlabel('Time (%)')
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/stats1d_roi/ex_ttest_paired.py` & `spm1d-0.4.2/spm1d/examples/stats1d/ex_ttest_paired.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,44 +1,36 @@
 
-import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 #(0) Load data:
 dataset      = spm1d.data.uv1d.t2.PlantarArchAngle()
 YA,YB        = dataset.get_data()  #normal and fast walking
 
 
-#(0a) Create region of interest(ROI):
-roi        = np.array([False]*YA.shape[1])
-roi[0:10]  = True
-
-
-
 
 #(1) Conduct t test:
 alpha      = 0.05
-t          = spm1d.stats.ttest_paired(YA, YB, roi=roi)
-ti         = t.inference(alpha, two_tailed=False, interp=True)
+t          = spm1d.stats.ttest_paired(YA, YB)
+ti         = t.inference(alpha, two_tailed=True, interp=True)
 
 
 
 #(2) Plot:
-plt.close('all')
+pyplot.close('all')
 ### plot mean and SD:
-plt.figure( figsize=(8, 3.5) )
-ax     = plt.axes( (0.1, 0.15, 0.35, 0.8) )
+pyplot.figure( figsize=(8, 3.5) )
+ax     = pyplot.axes( (0.1, 0.15, 0.35, 0.8) )
 spm1d.plot.plot_mean_sd(YA)
 spm1d.plot.plot_mean_sd(YB, linecolor='r', facecolor='r')
-spm1d.plot.plot_roi(roi, facecolor='b', alpha=0.3)
 ax.axhline(y=0, color='k', linestyle=':')
 ax.set_xlabel('Time (%)')
 ax.set_ylabel('Plantar arch angle  (deg)')
 ### plot SPM results:
-ax     = plt.axes((0.55,0.15,0.35,0.8))
+ax     = pyplot.axes((0.55,0.15,0.35,0.8))
 ti.plot()
 ti.plot_threshold_label(fontsize=8)
 ti.plot_p_values(size=10, offsets=[(0,0.3)])
 ax.set_xlabel('Time (%)')
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/stats2d/ex2d_ttest2.py` & `spm1d-0.4.2/spm1d/examples/stats2d/ex2d_ttest2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 
-import os
 import numpy as np
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 eps     = np.finfo(float).eps 
 
 
 #(0) Load data:
-dir0    = os.path.dirname(__file__)
-fname   = os.path.join(dir0, 'data2d.npy')
+dir0    = '/Users/todd/Dropbox/2019Sync/Documents/Projects/projectsOngoing/spm1d/ex2d/'
+fname   = dir0 + 'data2d.npy'
 Y0      = np.load(fname)
 y0      = np.array([yy.flatten() for yy in Y0])
 J,Q     = y0.shape
 
 
 
 #(1) Remove zero-variance nodes:
@@ -42,20 +41,19 @@
 z0[i]   = z
 Z0      = np.reshape(z0, Y0.shape[1:])
 Z0i     = Z0.copy()
 Z0i[np.abs(Z0i)<zstar] = 0
 ZZ      = np.hstack( [Z0, Z0i] )
 
 
-plt.close('all')
-plt.figure()
-ax = plt.axes()
+pyplot.close('all')
+pyplot.figure()
+ax = pyplot.axes()
 ax.imshow(np.ma.masked_array(ZZ, ZZ==0), origin='lower', cmap='jet', vmin=-15, vmax=15)
 ax.set_title('SPM results')
 ax.text(16, 10, 'Raw SPM', ha='center')
 ax.text(48, 10, 'Inference', ha='center')
-cb = plt.colorbar(mappable=ax.images[0])
+cb = pyplot.colorbar(mappable=ax.images[0])
 cb.set_label('t value')
-plt.tight_layout()
-plt.show()
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/examples/summarystats/ex_plot_meansd.py` & `spm1d-0.4.2/spm1d/examples/summarystats/ex_plot_meansd.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 
-import matplotlib.pyplot as plt
+from matplotlib import pyplot
 import spm1d
 
 
 
 # load dataset:
 dataset = spm1d.data.uv1d.anova1.SpeedGRFcategorical()
 Y,A     = dataset.get_data()
 Y0      = Y[A==1]
 Y1      = Y[A==2]
 Y2      = Y[A==3]
 
 
 # plot:
-plt.close('all')
+pyplot.close('all')
 spm1d.plot.plot_mean_sd(Y0, linecolor='b', facecolor=(0.7,0.7,1), edgecolor='b', label='Slow')
 spm1d.plot.plot_mean_sd(Y1, label='Normal')
 spm1d.plot.plot_mean_sd(Y2, linecolor='r', facecolor=(1,0.7,0.7), edgecolor='r', label='Fast')
-plt.xlim(0, 100)
-plt.xlabel('Time (%)', size=20)
-plt.ylabel('VGRF  (BW)', size=20)
-plt.legend(loc='lower left')
-plt.show()
+pyplot.xlim(0, 100)
+pyplot.xlabel('Time (%)', size=20)
+pyplot.ylabel('VGRF  (BW)', size=20)
+pyplot.legend(loc='lower left')
+pyplot.show()
```

### Comparing `spm1d-0.4.19/spm1d/io.py` & `spm1d-0.4.2/spm1d/io.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/plot.py` & `spm1d-0.4.2/spm1d/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,26 +273,28 @@
 	
 	None
 	'''
 	plotter = SPMPlotter(spm, ax=ax)
 	plotter.plot_design(factor_labels, fontsize)
 
 
-def plot_spmi(spmi, ax=None, color='k', linestyle='-', marker='', facecolor='0.8', lw=2, plot_thresh=True,
-			  plot_ylabel=True, thresh_color='k', autoset_xlim=True, autoset_ylim=True, label=None):
+
+
+
+
+
+def plot_spmi(spmi, ax=None, color='k', facecolor='0.8', lw=2, plot_thresh=True, plot_ylabel=True, thresh_color='k', autoset_xlim=True, autoset_ylim=True, label=None):
 	'''
 	Plot an **spm1d** SPM inference object as a line.
 	
 	:Parameters:
 	
 	- *spmi* --- an **spm1d** SPM object
 	- *ax* --- optional matplotlib.axes object  [default: matplotlib.pyplot.gca()]
 	- *color* --- optional line color specifier (for the raw SPM)
-	- *linestyle* --- optional line style specifier (for the raw SPM)
-	- *marker* --- optional marker specifier (for the raw SPM)
 	- *facecolor* --- optional face color (for suprathreshold clusters)
 	- *plot_thresh* --- if *True*, one or two horizontal threshold lines will be plotted (for one- or two-tailed inference)
 	- *plot_ylabel* --- if *True*, an "SPM{t}" or "SPM{F}" label will automatically be added to the y axis
 	- *autoset_ylim* --- if True (default), will set the y axis limits so that all text, line and patch objects are visible inside the axes
 	
 	:Returns:
 	
@@ -301,15 +303,15 @@
 	:Example:
 	
 	>>> t     = spm1d.stats.ttest(Y)
 	>>> ti    = t.inference(0.05)
 	>>> ti.plot()   # equivalent to "spm1d.plot.plot_spmi(ti)"
 	'''
 	plotter = SPMiPlotter(spmi, ax=ax)
-	plotter.plot(color=color, lw=lw, linestyle=linestyle, marker= marker, facecolor=facecolor, label=label, thresh_color=thresh_color)
+	plotter.plot(color=color, lw=lw, facecolor=facecolor, label=label, thresh_color=thresh_color)
 	if plot_ylabel:
 		plotter.plot_ylabel()
 	if autoset_xlim:
 		plotter._set_xlim()
 	if autoset_ylim:
 		plotter._set_ylim()
 
@@ -374,12 +376,12 @@
 	:Example:
 	
 	>>> t     = spm1d.stats.ttest(Y)
 	>>> ti    = t.inference(0.05)
 	>>> ti.plot_threshold_label(pos=(50,3.0))   # equivalent to "spm1d.plot.plot_spmi_threshold_label(ti, pos=(50,3.0))"
 	'''
 	plotter = SPMiPlotter(spmi, ax=ax)
-	h       = plotter.plot_threshold_label(lower=False, pos=pos, **kwdargs)
+	h       = plotter.plot_threshold_label(lower=False, pos=None, **kwdargs)
 	if autoset_ylim:
 		plotter._set_ylim(ax)
 	return h
```

### Comparing `spm1d-0.4.19/spm1d/rft1d/__init__.py` & `spm1d-0.4.2/spm1d/rft1d/__init__.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/data/weather/README.txt` & `spm1d-0.4.2/spm1d/rft1d/data/weather/README.txt`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/data/weather/daily.m` & `spm1d-0.4.2/spm1d/rft1d/data/weather/daily.m`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/data/weather/daily.mat` & `spm1d-0.4.2/spm1d/rft1d/data/weather/daily.mat`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/data.py` & `spm1d-0.4.2/spm1d/rft1d/data.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/distributions.py` & `spm1d-0.4.2/spm1d/rft1d/distributions.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/paper/all_results.py` & `spm1d-0.4.2/spm1d/rft1d/examples/paper/all_results.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/paper/fig01_fields1d.py` & `spm1d-0.4.2/spm1d/rft1d/examples/paper/fig01_fields1d.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/paper/fig02_EC_HC.py` & `spm1d-0.4.2/spm1d/rft1d/examples/paper/fig02_EC_HC.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/paper/fig03_EC.py` & `spm1d-0.4.2/spm1d/rft1d/examples/paper/fig03_EC.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/paper/fig04_fields1d_broken.py` & `spm1d-0.4.2/spm1d/rft1d/examples/paper/fig04_fields1d_broken.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/paper/fig05_EC_broken.py` & `spm1d-0.4.2/spm1d/rft1d/examples/paper/fig05_EC_broken.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/paper/fig06_sf.py` & `spm1d-0.4.2/spm1d/rft1d/examples/paper/fig06_sf.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/paper/fig07_bonf_sf.py` & `spm1d-0.4.2/spm1d/rft1d/examples/paper/fig07_bonf_sf.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/paper/fig08_bonf_isf.py` & `spm1d-0.4.2/spm1d/rft1d/examples/paper/fig08_bonf_isf.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/paper/fig09_val_maxima.py` & `spm1d-0.4.2/spm1d/rft1d/examples/paper/fig09_val_maxima.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/paper/fig10_upcrossing.py` & `spm1d-0.4.2/spm1d/rft1d/examples/paper/fig10_upcrossing.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/paper/fig11_val_cluster.py` & `spm1d-0.4.2/spm1d/rft1d/examples/paper/fig11_val_cluster.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/paper/fig12_val_set.py` & `spm1d-0.4.2/spm1d/rft1d/examples/paper/fig12_val_set.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/paper/fig13_weather_0_data.py` & `spm1d-0.4.2/spm1d/rft1d/examples/paper/fig13_weather_0_data.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/paper/fig14_fwhm_estimation.py` & `spm1d-0.4.2/spm1d/rft1d/examples/paper/fig14_fwhm_estimation.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/paper/fig15_weather_1_rft.py` & `spm1d-0.4.2/spm1d/rft1d/examples/paper/fig15_weather_1_rft.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/paper/fig16_weather_2_wrapped.py` & `spm1d-0.4.2/spm1d/rft1d/examples/paper/fig16_weather_2_wrapped.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/paper/fig17_weather_3_nonparam.py` & `spm1d-0.4.2/spm1d/rft1d/examples/paper/fig17_weather_3_nonparam.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/random_fields_0.py` & `spm1d-0.4.2/spm1d/rft1d/examples/random_fields_0.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/random_fields_1.py` & `spm1d-0.4.2/spm1d/rft1d/examples/random_fields_1.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/random_fields_2.py` & `spm1d-0.4.2/spm1d/rft1d/examples/random_fields_2.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/random_fields_broken_0.py` & `spm1d-0.4.2/spm1d/rft1d/examples/random_fields_broken_0.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/random_fields_broken_1.py` & `spm1d-0.4.2/spm1d/rft1d/examples/random_fields_broken_1.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/random_fields_broken_2.py` & `spm1d-0.4.2/spm1d/rft1d/examples/random_fields_broken_2.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/smoothness_estimation.py` & `spm1d-0.4.2/spm1d/rft1d/examples/smoothness_estimation.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/smoothness_estimation_broken.py` & `spm1d-0.4.2/spm1d/rft1d/examples/smoothness_estimation_broken.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/val_broken_0_gauss.py` & `spm1d-0.4.2/spm1d/rft1d/examples/val_broken_0_gauss.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/val_broken_1_t.py` & `spm1d-0.4.2/spm1d/rft1d/examples/val_broken_1_t.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/val_broken_2_F.py` & `spm1d-0.4.2/spm1d/rft1d/examples/val_broken_2_F.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/val_broken_3_T2.py` & `spm1d-0.4.2/spm1d/rft1d/examples/val_broken_3_T2.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/val_broken_4_X2.py` & `spm1d-0.4.2/spm1d/rft1d/examples/val_broken_4_X2.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/val_conj_0_gauss.py` & `spm1d-0.4.2/spm1d/rft1d/examples/val_conj_0_gauss.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/val_conj_1_t.py` & `spm1d-0.4.2/spm1d/rft1d/examples/val_conj_1_t.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/val_conj_2_F.py` & `spm1d-0.4.2/spm1d/rft1d/examples/val_conj_2_F.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/val_conj_3_T2.py` & `spm1d-0.4.2/spm1d/rft1d/examples/val_conj_3_T2.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/val_conj_4_X2.py` & `spm1d-0.4.2/spm1d/rft1d/examples/val_conj_4_X2.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/val_max_0_gaussian_0d.py` & `spm1d-0.4.2/spm1d/rft1d/examples/val_max_0_gaussian_0d.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/val_max_0_gaussian_1d.py` & `spm1d-0.4.2/spm1d/rft1d/examples/val_max_0_gaussian_1d.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/val_max_1_onesample_t_0d.py` & `spm1d-0.4.2/spm1d/rft1d/examples/val_max_1_onesample_t_0d.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/val_max_1_onesample_t_1d.py` & `spm1d-0.4.2/spm1d/rft1d/examples/val_max_1_onesample_t_1d.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/val_max_2_twosample_t_0d.py` & `spm1d-0.4.2/spm1d/rft1d/examples/val_max_2_twosample_t_0d.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/val_max_2_twosample_t_1d.py` & `spm1d-0.4.2/spm1d/rft1d/examples/val_max_2_twosample_t_1d.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/val_max_3_regress_0d.py` & `spm1d-0.4.2/spm1d/rft1d/examples/val_max_3_regress_0d.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/val_max_3_regress_1d.py` & `spm1d-0.4.2/spm1d/rft1d/examples/val_max_3_regress_1d.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/val_max_4_anova1_0d.py` & `spm1d-0.4.2/spm1d/rft1d/examples/val_max_4_anova1_0d.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/val_max_4_anova1_1d.py` & `spm1d-0.4.2/spm1d/rft1d/examples/val_max_4_anova1_1d.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/val_max_5_onesample_T2_0d.py` & `spm1d-0.4.2/spm1d/rft1d/examples/val_max_5_onesample_T2_0d.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/val_max_5_onesample_T2_1d.py` & `spm1d-0.4.2/spm1d/rft1d/examples/val_max_5_onesample_T2_1d.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/val_max_6_twosample_T2_0d.py` & `spm1d-0.4.2/spm1d/rft1d/examples/val_max_6_twosample_T2_0d.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/val_max_6_twosample_T2_1d.py` & `spm1d-0.4.2/spm1d/rft1d/examples/val_max_6_twosample_T2_1d.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/val_max_7_cca_0d.py` & `spm1d-0.4.2/spm1d/rft1d/examples/val_max_7_cca_0d.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/val_max_7_cca_1d.py` & `spm1d-0.4.2/spm1d/rft1d/examples/val_max_7_cca_1d.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/val_max_8_manova1_0d.py` & `spm1d-0.4.2/spm1d/rft1d/examples/val_max_8_manova1_0d.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/val_max_8_manova1_1d.py` & `spm1d-0.4.2/spm1d/rft1d/examples/val_max_8_manova1_1d.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/val_upx_0_gauss_cluster.py` & `spm1d-0.4.2/spm1d/rft1d/examples/val_upx_0_gauss_cluster.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/val_upx_0_gauss_set.py` & `spm1d-0.4.2/spm1d/rft1d/examples/val_upx_0_gauss_set.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/val_upx_1_t_cluster.py` & `spm1d-0.4.2/spm1d/rft1d/examples/val_upx_1_t_cluster.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/val_upx_1_t_set.py` & `spm1d-0.4.2/spm1d/rft1d/examples/val_upx_1_t_set.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/val_upx_2_F_cluster.py` & `spm1d-0.4.2/spm1d/rft1d/examples/val_upx_2_F_cluster.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/val_upx_2_F_set.py` & `spm1d-0.4.2/spm1d/rft1d/examples/val_upx_2_F_set.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/val_upx_3_T2_cluster.py` & `spm1d-0.4.2/spm1d/rft1d/examples/val_upx_3_T2_cluster.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/val_upx_3_T2_set.py` & `spm1d-0.4.2/spm1d/rft1d/examples/val_upx_3_T2_set.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/val_upx_4_X2_cluster.py` & `spm1d-0.4.2/spm1d/rft1d/examples/val_upx_4_X2_cluster.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/val_upx_4_X2_set.py` & `spm1d-0.4.2/spm1d/rft1d/examples/val_upx_4_X2_set.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/weather_0_plotdata.py` & `spm1d-0.4.2/spm1d/rft1d/examples/weather_0_plotdata.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/weather_1_rft.py` & `spm1d-0.4.2/spm1d/rft1d/examples/weather_1_rft.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/weather_2_nonparam.py` & `spm1d-0.4.2/spm1d/rft1d/examples/weather_2_nonparam.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/examples/weather_3_wrapped.py` & `spm1d-0.4.2/spm1d/rft1d/examples/weather_3_wrapped.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/rft1d/geom.py` & `spm1d-0.4.2/spm1d/rft1d/geom.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 '''
 Geometry module
 
 This module contains functions for computing various geomtric characteristics
 of 1D fields and upcrossings.
 '''
 
-# Copyright (C) 2022  Todd Pataky
+# Copyright (C) 2016  Todd Pataky
 
 
 from math import log
 import numpy as np
 
 
-# eps         = np.finfo(np.float).eps
-eps         = np.finfo(float).eps
+eps         = np.finfo(np.float).eps
 
 
 
 class Upcrossing(object):
 	'''
 	A class for computing upcrossing extents.
 	Computing upcrossing extents is simple if the upcrossing extent is to be
```

### Comparing `spm1d-0.4.19/spm1d/rft1d/prob.py` & `spm1d-0.4.2/spm1d/rft1d/prob.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 
 '''
 Random Field Theory expectations and probabilities.
 The core RFT computations are conducted inside **prob.rft**, and the 
 **RFTCalculator** class serves as a high-level interface to **prob.rft**
 '''
 
-# Copyright (C) 2022  Todd Pataky
+# Copyright (C) 2016  Todd Pataky
 
 
 
 from math import pi,log,sqrt,exp
 import numpy as np
 from scipy import stats,optimize
 from scipy.special import gammaln,gamma
 from . import geom
 
 # CONSTANTS:
 FOUR_LOG2   = 4*log(2)
 SQRT_4LOG2  = sqrt(4*log(2))
 SQRT_2      = sqrt(2)
 TWO_PI      = 2*pi
-# eps         = np.finfo(np.float).eps
-eps         = np.finfo(float).eps
+eps         = np.finfo(np.float).eps
 
 
 
 def p_bonferroni(STAT, z, df, Q, n=1):
 	'''
 	Bonferroni correction.
```

### Comparing `spm1d-0.4.19/spm1d/rft1d/random.py` & `spm1d-0.4.2/spm1d/rft1d/random.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/stats/__init__.py` & `spm1d-0.4.2/spm1d/stats/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 * Univariate 0D tests:  **Y** should be ( J x 1 )
 * Multivariate 0D tests:  **Y** should be ( J x I )
 * Univariate 1D tests:  **Y** should be ( J x Q )
 * Multivariate 1D tests:  **Y** should be ( J x Q x I )
 
 '''
 
-# Copyright (C) 2021  Todd Pataky
+# Copyright (C) 2016  Todd Pataky
 
 
 
 from . import _spm
 
 from . t import ttest, ttest_paired, ttest2, regress, glm
 from . ci import ci_onesample, ci_pairedsample, ci_twosample
@@ -30,11 +30,10 @@
 from . anova import anova1,anova1rm
 from . anova import anova2,anova2nested,anova2rm,anova2onerm
 from . anova import anova3,anova3nested,anova3rm,anova3tworm,anova3onerm
 
 from . hotellings import hotellings, hotellings_paired, hotellings2
 from . cca import cca
 from . manova import manova1
-from . var import eqvartest
 
 from . import nonparam
 from . import normality
```

### Comparing `spm1d-0.4.19/spm1d/stats/_clusters.py` & `spm1d-0.4.2/spm1d/stats/_clusters.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 '''
 Clusters module
 
 This module contains class definitions for raw SPMs (raw test statistic continua)
 and inference SPMs (thresholded test statistic).
 '''
 
-# Copyright (C) 2020  Todd Pataky
+# Copyright (C) 2016  Todd Pataky
 
 
 
 from math import floor,ceil
 import numpy as np
 from .. import rft1d
 
@@ -184,15 +184,14 @@
 		### compute metric value:
 		x                  = metric.get_single_cluster_metric_xz(self._X, self._Z, self.threshold, two_tailed)
 		if self.iswrapped:
 			x             += metric.get_single_cluster_metric_xz(self._other._X, self._other._Z, self.threshold, two_tailed)
 		self.metric_value  = x
 
 	def inference(self, pdf, two_tailed):
-		pdf      = np.asarray(pdf, dtype=float)  # fix for ragged nested sequences
-		self.P   = (pdf >= self.metric_value).mean()
+		self.P             = (pdf >= self.metric_value).mean()
 		# self.P             = max( self.P,  1.0/self.nPermUnique )
```

### Comparing `spm1d-0.4.19/spm1d/stats/_datachecks.py` & `spm1d-0.4.2/spm1d/stats/_datachecks.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/stats/_mvbase.py` & `spm1d-0.4.2/spm1d/stats/_mvbase.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/stats/_reml.py` & `spm1d-0.4.2/spm1d/stats/_reml.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/stats/_spm.py` & `spm1d-0.4.2/spm1d/stats/_spm.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 (This and all modules whose names start with underscores
 are not meant to be accessed directly by the user.)
 
 This module contains class definitions for raw SPMs (raw test statistic continua)
 and inference SPMs (thresholded test statistic).
 '''
 
-# Copyright (C) 2022  Todd Pataky
+# Copyright (C) 2016  Todd Pataky
 
 
 import sys
 import numpy as np
 from scipy import stats
 from .. import rft1d
 from .. plot import plot_spm, plot_spm_design
@@ -266,31 +266,19 @@
 		if stat == 'T':
 			stat = 't'
 		s        = ''
 		s       += 'SPM{%s}\n' %stat
 		if self.isanova:
 			s   += '   SPM.effect :   %s\n' %self.effect
 		s       += '   SPM.z      :  %s\n' %self._repr_teststat()
-		if self.isregress:
-			s   += '   SPM.r      :  %s\n' %self._repr_corrcoeff()
 		s       += '   SPM.df     :  %s\n' %dflist2str(self.df)
 		s       += '   SPM.fwhm   :  %.5f\n' %self.fwhm
 		s       += '   SPM.resels :  (%d, %.5f)\n\n\n' %tuple(self.resels)
 		return s
 	
-	@property
-	def R(self):
-		return self.residuals
-	@property
-	def nNodes(self):
-		return self.Q
-	
-	
-	def _repr_corrcoeff(self):
-		return '(1x%d) correlation coefficient field' %self.Q
 	def _repr_teststat(self):
 		return '(1x%d) test stat field' %self.Q
 	def _repr_teststat_short(self):
 		return '(1x%d) array' %self.Q
 		# return '(1x%d) %s field' %(self.Q, self.STAT)
 	
 
@@ -594,34 +582,29 @@
 	isinference = True
 	
 	def __init__(self, spm, alpha, zstar, clusters, p_set, p, two_tailed=False):
 		_SPM.__init__(self, spm.STAT, spm.z, spm.df, spm.fwhm, spm.resels, X=spm.X, beta=spm.beta, residuals=spm.residuals, sigma2=spm.sigma2, roi=spm.roi)
 		self.alpha       = alpha               #Type I error rate
 		self.zstar       = zstar               #critical threshold
 		self.clusters    = clusters            #supra-threshold cluster information
-		self.isregress   = spm.isregress       #propagate regression flag
 		self.nClusters   = len(clusters)       #number of supra-threshold clusters
 		self.h0reject    = self.nClusters > 0  #null hypothesis rejection decision
 		self.p_set       = p_set               #set-level p value
 		self.p           = p                   #cluster-level p values
 		self.two_tailed  = two_tailed          #two-tailed test boolean
-		if self.isregress:
-			self.r       = spm.r
 		if self.isanova:
 			self.set_effect_label( spm.effect )
 
 	def __repr__(self):
 		stat     = 't' if self.STAT == 'T' else self.STAT
 		s        = ''
 		s       += 'SPM{%s} inference field\n' %stat
 		if self.isanova:
 			s   += '   SPM.effect    :   %s\n' %self.effect
 		s       += '   SPM.z         :  (1x%d) raw test stat field\n' %self.Q
-		if self.isregress:
-			s   += '   SPM.r         :  %s\n' %self._repr_corrcoeff()
 		s       += '   SPM.df        :  %s\n' %dflist2str(self.df)
 		s       += '   SPM.fwhm      :  %.5f\n' %self.fwhm
 		s       += '   SPM.resels    :  (%d, %.5f)\n' %tuple(self.resels)
 		s       += 'Inference:\n'
 		s       += '   SPM.alpha     :  %.3f\n' %self.alpha
 		s       += '   SPM.zstar     :  %.5f\n' %self.zstar
 		s       += '   SPM.h0reject  :  %s\n' %self.h0reject
```

### Comparing `spm1d-0.4.19/spm1d/stats/_spmlist.py` & `spm1d-0.4.2/spm1d/stats/_spmlist.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,16 +60,16 @@
 	
 	def get_df_values(self):
 		return [f.df for f in self]
 	def get_effect_labels(self):
 		return tuple( [f.effect for f in self] )
 	def get_f_values(self):
 		return tuple( [f.z for f in self] )
-	def inference(self, alpha=0.05, **kwargs):
-		FFi               = SPMFiList(  [f.inference(alpha=alpha, **kwargs)   for f in self]  )
+	def inference(self, alpha=0.05):
+		FFi               = SPMFiList(  [f.inference(alpha=alpha)   for f in self]  )
 		FFi.set_design_label( self.design )
 		FFi.effect_labels = self.effect_labels
 		FFi.nFactors      = self.nFactors
 		return FFi
 	def plot(self, plot_threshold_label=True, plot_p_values=True, autoset_ylim=True):
 		_plot_F_list(self, plot_threshold_label, plot_p_values, autoset_ylim)
 	def print_summary(self):
```

### Comparing `spm1d-0.4.19/spm1d/stats/anova/designs.py` & `spm1d-0.4.2/spm1d/stats/anova/designs.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/stats/anova/factors.py` & `spm1d-0.4.2/spm1d/stats/anova/factors.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/stats/anova/models.py` & `spm1d-0.4.2/spm1d/stats/anova/models.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/stats/anova/ui.py` & `spm1d-0.4.2/spm1d/stats/anova/ui.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/stats/cca.py` & `spm1d-0.4.2/spm1d/stats/cca.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/stats/ci.py` & `spm1d-0.4.2/spm1d/stats/ci.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/stats/hotellings.py` & `spm1d-0.4.2/spm1d/stats/hotellings.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/stats/manova.py` & `spm1d-0.4.2/spm1d/stats/manova.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/stats/nonparam/__init__.py` & `spm1d-0.4.2/spm1d/stats/nonparam/__init__.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/stats/nonparam/_snpm.py` & `spm1d-0.4.2/spm1d/stats/nonparam/_snpm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-# Copyright (C) 2022  Todd Pataky
+# Copyright (C) 2016  Todd Pataky
 
 from math import ceil
 import numpy as np
 from . metrics import metric_dict
 from .. import _spm
 from .. _spm import p2string, plist2string, _SPMF
 from .. _clusters import ClusterNonparam
```

### Comparing `spm1d-0.4.19/spm1d/stats/nonparam/_snpmlist.py` & `spm1d-0.4.2/spm1d/stats/nonparam/_snpmlist.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/stats/nonparam/calculators.py` & `spm1d-0.4.2/spm1d/stats/nonparam/calculators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
-# Copyright (C) 2023  Todd Pataky
+# Copyright (C) 2016  Todd Pataky
 
 from math import log
 import numpy as np
-from .. anova import designs,models
-from .. anova.ui import aov
+from spm1d.stats.anova import designs,models
+from spm1d.stats.anova.ui import aov
 
 
 
 eps    = np.finfo(float).eps   #smallest float, used to avoid divide-by-zero errors
```

### Comparing `spm1d-0.4.19/spm1d/stats/nonparam/ci.py` & `spm1d-0.4.2/spm1d/stats/nonparam/ci.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/stats/nonparam/metrics.py` & `spm1d-0.4.2/spm1d/stats/nonparam/metrics.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/stats/nonparam/permuters.py` & `spm1d-0.4.2/spm1d/stats/nonparam/permuters.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/stats/nonparam/stats.py` & `spm1d-0.4.2/spm1d/stats/nonparam/stats.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/stats/normality/k2.py` & `spm1d-0.4.2/spm1d/stats/normality/k2.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/stats/normality/sw.py` & `spm1d-0.4.2/spm1d/stats/normality/sw.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/stats/t.py` & `spm1d-0.4.2/spm1d/stats/t.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.19/spm1d/util.py` & `spm1d-0.4.2/spm1d/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,24 +8,23 @@
 - get_dataset
 - interp
 - p_corrected_bonf
 - p_critical_bonf
 - smooth
 '''
 
-# Copyright (C) 2022  Todd Pataky
-# updated (2022/02/06) todd
+# Copyright (C) 2016  Todd Pataky
+# updated (2016/10/01) todd
 
 
 
 from math import sqrt,log
 import numpy as np
 from . stats._spm import plist2string as p2s
-# from scipy.ndimage.filters import gaussian_filter1d
-from scipy.ndimage import gaussian_filter1d
+from scipy.ndimage.filters import gaussian_filter1d
 
 
 
 
 
 
 def plist2stringlist(pList):
```

### Comparing `spm1d-0.4.19/spm1d.egg-info/SOURCES.txt` & `spm1d-0.4.2/spm1d.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -300,15 +300,14 @@
 spm1d/examples/stats1d/ex_anova3rm.py
 spm1d/examples/stats1d/ex_anova3tworm.py
 spm1d/examples/stats1d/ex_cca_Dorn2012.py
 spm1d/examples/stats1d/ex_ci_onesample.py
 spm1d/examples/stats1d/ex_ci_onesample_standalone.py
 spm1d/examples/stats1d/ex_ci_pairedsample.py
 spm1d/examples/stats1d/ex_ci_twosample.py
-spm1d/examples/stats1d/ex_eqvartest.py
 spm1d/examples/stats1d/ex_glm.py
 spm1d/examples/stats1d/ex_hotellings2_Besier2009muscleforces.py
 spm1d/examples/stats1d/ex_hotellings_paired_Neptune1999.py
 spm1d/examples/stats1d/ex_hotellings_paired_Pataky2014.py
 spm1d/examples/stats1d/ex_manova1_Dorn2012.py
 spm1d/examples/stats1d/ex_regression.py
 spm1d/examples/stats1d/ex_ttest.py
@@ -336,19 +335,17 @@
 spm1d/examples/stats1d_roi/ex_hotellings_paired_Pataky2014.py
 spm1d/examples/stats1d_roi/ex_manova1_Dorn2012.py
 spm1d/examples/stats1d_roi/ex_regression.py
 spm1d/examples/stats1d_roi/ex_regression_directional.py
 spm1d/examples/stats1d_roi/ex_ttest.py
 spm1d/examples/stats1d_roi/ex_ttest2.py
 spm1d/examples/stats1d_roi/ex_ttest_paired.py
-spm1d/examples/stats2d/data2d.npy
 spm1d/examples/stats2d/ex2d_ttest2.py
 spm1d/examples/summarystats/ex_plot_errorcloud.py
 spm1d/examples/summarystats/ex_plot_meansd.py
-spm1d/examples/validation/val_eqvartest.py
 spm1d/rft1d/__init__.py
 spm1d/rft1d/data.py
 spm1d/rft1d/distributions.py
 spm1d/rft1d/geom.py
 spm1d/rft1d/prob.py
 spm1d/rft1d/random.py
 spm1d/rft1d/data/weather/README.txt
@@ -430,15 +427,14 @@
 spm1d/stats/_spm.py
 spm1d/stats/_spmlist.py
 spm1d/stats/cca.py
 spm1d/stats/ci.py
 spm1d/stats/hotellings.py
 spm1d/stats/manova.py
 spm1d/stats/t.py
-spm1d/stats/var.py
 spm1d/stats/anova/__init__.py
 spm1d/stats/anova/designs.py
 spm1d/stats/anova/factors.py
 spm1d/stats/anova/models.py
 spm1d/stats/anova/ui.py
 spm1d/stats/nonparam/__init__.py
 spm1d/stats/nonparam/_snpm.py
```

