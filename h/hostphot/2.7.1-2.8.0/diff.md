# Comparing `tmp/hostphot-2.7.1.tar.gz` & `tmp/hostphot-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hostphot-2.7.1.tar", last modified: Fri May 12 03:55:03 2023, max compression
+gzip compressed data, was "hostphot-2.8.0.tar", last modified: Thu Jun 22 14:21:35 2023, max compression
```

## Comparing `hostphot-2.7.1.tar` & `hostphot-2.8.0.tar`

### file list

```diff
@@ -1,331 +1,356 @@
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-12 03:55:03.700277 hostphot-2.7.1/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1065 2022-05-31 09:22:42.000000 hostphot-2.7.1/LICENSE
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       53 2022-05-31 09:22:42.000000 hostphot-2.7.1/MANIFEST.in
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9525 2023-05-12 03:55:03.700277 hostphot-2.7.1/PKG-INFO
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     8993 2023-05-12 03:49:47.000000 hostphot-2.7.1/README.md
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      187 2022-05-31 09:22:42.000000 hostphot-2.7.1/pyproject.toml
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      190 2023-05-11 02:29:33.000000 hostphot-2.7.1/requirements.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       38 2023-05-12 03:55:03.700277 hostphot-2.7.1/setup.cfg
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1251 2023-04-28 09:57:11.000000 hostphot-2.7.1/setup.py
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-12 03:55:03.680278 hostphot-2.7.1/src/
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-12 03:55:03.684277 hostphot-2.7.1/src/hostphot/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      439 2023-05-12 03:49:47.000000 hostphot-2.7.1/src/hostphot/__init__.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      386 2023-05-11 09:42:22.000000 hostphot-2.7.1/src/hostphot/_constants.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       47 2023-05-12 03:49:47.000000 hostphot-2.7.1/src/hostphot/_version.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1762 2022-11-14 14:06:00.000000 hostphot-2.7.1/src/hostphot/coadd.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    45897 2023-05-11 02:29:33.000000 hostphot-2.7.1/src/hostphot/cutouts.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6006 2023-05-05 10:39:56.000000 hostphot-2.7.1/src/hostphot/dust.py
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-12 03:55:03.684277 hostphot-2.7.1/src/hostphot/filters/
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-12 03:55:03.684277 hostphot-2.7.1/src/hostphot/filters/2MASS/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1218 2022-07-28 14:32:41.000000 hostphot-2.7.1/src/hostphot/filters/2MASS/2MASS_H.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2247 2022-07-28 14:32:41.000000 hostphot-2.7.1/src/hostphot/filters/2MASS/2MASS_J.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1596 2022-11-14 14:06:00.000000 hostphot-2.7.1/src/hostphot/filters/2MASS/2MASS_Ks.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       15 2022-07-28 14:32:41.000000 hostphot-2.7.1/src/hostphot/filters/2MASS/AAA_README
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1549 2022-07-28 14:32:41.000000 hostphot-2.7.1/src/hostphot/filters/AAA_README
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-12 03:55:03.684277 hostphot-2.7.1/src/hostphot/filters/DES/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       53 2022-05-31 09:22:42.000000 hostphot-2.7.1/src/hostphot/filters/DES/AAA_README
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3387 2022-07-28 14:32:41.000000 hostphot-2.7.1/src/hostphot/filters/DES/DES_Y.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4281 2022-07-28 14:32:41.000000 hostphot-2.7.1/src/hostphot/filters/DES/DES_g.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4515 2022-07-28 14:32:41.000000 hostphot-2.7.1/src/hostphot/filters/DES/DES_i.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4516 2022-07-28 14:32:41.000000 hostphot-2.7.1/src/hostphot/filters/DES/DES_r.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4338 2022-07-28 14:32:41.000000 hostphot-2.7.1/src/hostphot/filters/DES/DES_z.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-12 03:55:03.684277 hostphot-2.7.1/src/hostphot/filters/GALEX/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       15 2022-07-28 14:32:41.000000 hostphot-2.7.1/src/hostphot/filters/GALEX/AAA_README
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6777 2022-07-28 14:32:41.000000 hostphot-2.7.1/src/hostphot/filters/GALEX/GALEX_FUV.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    18911 2022-07-28 14:32:41.000000 hostphot-2.7.1/src/hostphot/filters/GALEX/GALEX_NUV.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-12 03:55:03.684277 hostphot-2.7.1/src/hostphot/filters/HST/
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-12 03:55:03.688277 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    23838 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F435W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    32416 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F475W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4110 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F502N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    15624 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F550M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    31966 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F555W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    43735 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F606W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    29858 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F625W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5234 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F658N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3236 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F660N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    37258 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F775W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)   103143 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F814W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    53451 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F850LP.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7990 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F892N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21666 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR1016N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9107 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR388N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9858 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR423N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    36616 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR459M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    10646 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR462N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11519 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR505N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    12578 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR551N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    13680 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR601N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    53850 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR647M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    14675 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR656N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    15873 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR716N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    17289 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR782N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    18750 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR853N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    61170 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR914M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    19635 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR931N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1264 2023-05-05 10:39:56.000000 hostphot-2.7.1/src/hostphot/filters/HST/IR_err.txt
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-12 03:55:03.688277 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9747 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F090M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2486 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F095N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2874 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F097N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3264 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F108N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    12445 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F110M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    24500 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F110W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3077 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F113N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    33411 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F140W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    13978 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F145M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21021 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F160W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4877 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F164N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11680 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F165M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5199 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F166N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    12148 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F170M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6879 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F187N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7831 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F190N.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-12 03:55:03.688277 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    24275 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F110W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    20849 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F160W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    12018 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F165M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    18588 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F171M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    17947 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F180M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6506 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F187N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    41358 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F187W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5506 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F190N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21662 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F204M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    30947 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F205W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    20965 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F207M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11516 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F212N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7894 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F215N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7479 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F216N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    30813 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F222M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    26323 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F237M.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-12 03:55:03.688277 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3240 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F108N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    24427 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F110W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3363 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F113N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    35249 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F150W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    20994 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F160W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4858 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F164N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4820 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F166N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    43711 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F175W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6876 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F187N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5510 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F190N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7212 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F196N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9291 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F200N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11541 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F212N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7906 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F215N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    30812 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F222M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    13019 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F240M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3503 2023-05-05 10:39:56.000000 hostphot-2.7.1/src/hostphot/filters/HST/UVIS1_err.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3503 2023-05-05 10:39:56.000000 hostphot-2.7.1/src/hostphot/filters/HST/UVIS2_err.txt
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-12 03:55:03.692277 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     8959 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F098M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9826 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F105W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21512 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F110W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    22426 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F125W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4121 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F126N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5064 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F127M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6580 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F128N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3261 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F130N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3792 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F132N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5421 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F139M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    13977 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F140W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6752 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F153M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    10046 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F160W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4738 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F164N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6887 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F167N.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-12 03:55:03.696277 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)   156254 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F200LP.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21978 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F218W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    29976 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F225W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21591 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F275W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7558 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F280N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    56436 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F300X.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    15547 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F336W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    19356 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F343N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)   146819 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F350LP.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4504 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F373N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9638 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F390M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    26406 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F390W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7035 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F395N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9314 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F410M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    18697 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F438W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9833 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F467M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3637 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F469N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    32782 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F475W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    72677 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F475X.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5098 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F487N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5804 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F502N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    38578 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F547M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    63538 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F555W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    97333 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F600LP.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    51442 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F606W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21890 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F621M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    34917 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F625W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4204 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F631N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3675 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F645N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2150 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F656N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11299 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F657N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3236 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F658N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11865 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F665N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11991 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F673N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    13792 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F680N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    20007 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F689M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    19898 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F763M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    36590 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F775W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    54378 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F814W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    33733 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F845M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    57316 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F850LP.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    12497 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F953N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    13422 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ232N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    13900 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ243N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21137 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ378N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6727 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ387N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    39729 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ422M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11393 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ436N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1548 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ437N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    22828 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ492N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    26635 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ508N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4658 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ575N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    19283 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ619N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    20492 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ634N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4687 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ672N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4387 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ674N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    24973 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ727N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    25138 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ750N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2950 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ889N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2948 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ906N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3346 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ924N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3461 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ937N.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-12 03:55:03.700277 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)   156503 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F200LP.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    20752 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F218W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    29190 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F225W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21479 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F275W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7566 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F280N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    55542 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F300X.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    15542 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F336W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    19332 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F343N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)   147032 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F350LP.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4495 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F373N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9640 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F390M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    26441 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F390W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7031 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F395N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9300 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F410M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    18727 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F438W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9871 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F467M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3641 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F469N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    32751 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F475W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    72732 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F475X.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5104 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F487N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5798 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F502N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    38608 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F547M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    63493 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F555W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    97494 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F600LP.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    51384 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F606W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21858 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F621M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    34960 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F625W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4209 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F631N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3686 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F645N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2154 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F656N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11309 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F657N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3233 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F658N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11857 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F665N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11991 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F673N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    13805 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F680N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    20019 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F689M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    19919 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F763M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    36600 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F775W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    54473 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F814W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    33739 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F845M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    57507 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F850LP.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    12507 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F953N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    13422 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ232N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    13900 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ243N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21137 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ378N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6727 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ387N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    39729 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ422M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11393 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ436N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1548 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ437N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    22828 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ492N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    26635 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ508N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4658 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ575N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    19283 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ619N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    20492 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ634N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4687 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ672N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4387 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ674N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    24973 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ727N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    25138 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ750N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2950 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ889N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2948 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ906N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3346 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ924N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3461 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ937N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2012 2023-05-05 10:39:56.000000 hostphot-2.7.1/src/hostphot/filters/HST/ir_aper_corrections.csv
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    18667 2023-05-05 10:39:56.000000 hostphot-2.7.1/src/hostphot/filters/HST/wfc3uvis1_aper_007_syn.csv
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    18635 2023-05-05 10:39:56.000000 hostphot-2.7.1/src/hostphot/filters/HST/wfc3uvis2_aper_007_syn.csv
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-12 03:55:03.700277 hostphot-2.7.1/src/hostphot/filters/LegacySurvey/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2281 2022-11-14 14:06:00.000000 hostphot-2.7.1/src/hostphot/filters/LegacySurvey/BASS_g.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3180 2022-11-14 14:06:00.000000 hostphot-2.7.1/src/hostphot/filters/LegacySurvey/BASS_r.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21743 2022-11-14 14:06:00.000000 hostphot-2.7.1/src/hostphot/filters/LegacySurvey/DECAM_g.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21744 2022-11-14 14:06:00.000000 hostphot-2.7.1/src/hostphot/filters/LegacySurvey/DECAM_r.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21744 2022-11-14 14:06:00.000000 hostphot-2.7.1/src/hostphot/filters/LegacySurvey/DECAM_z.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7028 2022-11-14 14:06:00.000000 hostphot-2.7.1/src/hostphot/filters/LegacySurvey/MzLS_z.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      300 2022-11-14 14:06:00.000000 hostphot-2.7.1/src/hostphot/filters/LegacySurvey/README.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4275 2022-11-14 14:06:00.000000 hostphot-2.7.1/src/hostphot/filters/LegacySurvey/init_BASS_g.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5840 2022-11-14 14:06:00.000000 hostphot-2.7.1/src/hostphot/filters/LegacySurvey/init_BASS_r.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-12 03:55:03.700277 hostphot-2.7.1/src/hostphot/filters/PS1/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      136 2022-05-31 09:22:42.000000 hostphot-2.7.1/src/hostphot/filters/PS1/AAA_README.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3717 2022-07-28 14:32:41.000000 hostphot-2.7.1/src/hostphot/filters/PS1/PS1_g.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3759 2022-07-28 14:32:41.000000 hostphot-2.7.1/src/hostphot/filters/PS1/PS1_i.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3885 2022-07-28 14:32:41.000000 hostphot-2.7.1/src/hostphot/filters/PS1/PS1_r.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4385 2022-07-28 14:32:41.000000 hostphot-2.7.1/src/hostphot/filters/PS1/PS1_y.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3486 2022-07-28 14:32:41.000000 hostphot-2.7.1/src/hostphot/filters/PS1/PS1_z.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-12 03:55:03.700277 hostphot-2.7.1/src/hostphot/filters/SDSS/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       72 2022-05-31 09:22:42.000000 hostphot-2.7.1/src/hostphot/filters/SDSS/AAA_README
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1414 2022-07-28 14:32:41.000000 hostphot-2.7.1/src/hostphot/filters/SDSS/SDSS_g.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1260 2022-07-28 14:32:41.000000 hostphot-2.7.1/src/hostphot/filters/SDSS/SDSS_i.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1176 2022-07-28 14:32:41.000000 hostphot-2.7.1/src/hostphot/filters/SDSS/SDSS_r.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4718 2022-07-28 14:32:41.000000 hostphot-2.7.1/src/hostphot/filters/SDSS/SDSS_u.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2509 2022-07-28 14:32:41.000000 hostphot-2.7.1/src/hostphot/filters/SDSS/SDSS_z.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-12 03:55:03.700277 hostphot-2.7.1/src/hostphot/filters/Spitzer/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      189 2022-11-14 14:06:00.000000 hostphot-2.7.1/src/hostphot/filters/Spitzer/README.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     8211 2022-11-14 14:06:00.000000 hostphot-2.7.1/src/hostphot/filters/Spitzer/Spitzer_IRAC.1.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     8421 2022-11-14 14:06:00.000000 hostphot-2.7.1/src/hostphot/filters/Spitzer/Spitzer_IRAC.2.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6531 2022-11-14 14:06:00.000000 hostphot-2.7.1/src/hostphot/filters/Spitzer/Spitzer_IRAC.3.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7375 2022-11-14 14:06:00.000000 hostphot-2.7.1/src/hostphot/filters/Spitzer/Spitzer_IRAC.4.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2816 2022-11-14 14:06:00.000000 hostphot-2.7.1/src/hostphot/filters/Spitzer/Spitzer_MIPS.1.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-12 03:55:03.700277 hostphot-2.7.1/src/hostphot/filters/VISTA/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       84 2022-11-14 14:06:00.000000 hostphot-2.7.1/src/hostphot/filters/VISTA/README.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    39168 2022-11-14 14:06:00.000000 hostphot-2.7.1/src/hostphot/filters/VISTA/VISTA_H.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    50048 2022-11-14 14:06:00.000000 hostphot-2.7.1/src/hostphot/filters/VISTA/VISTA_J.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    41344 2022-11-14 14:06:00.000000 hostphot-2.7.1/src/hostphot/filters/VISTA/VISTA_Ks.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    46341 2022-11-14 14:06:00.000000 hostphot-2.7.1/src/hostphot/filters/VISTA/VISTA_Y.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)   176418 2022-11-14 14:06:00.000000 hostphot-2.7.1/src/hostphot/filters/VISTA/VISTA_Z.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-12 03:55:03.700277 hostphot-2.7.1/src/hostphot/filters/WISE/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       15 2022-07-28 14:32:41.000000 hostphot-2.7.1/src/hostphot/filters/WISE/AAA_README
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2961 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/WISE/WISE_W1.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3528 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/WISE/WISE_W2.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    24404 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/WISE/WISE_W3.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    19734 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/filters/WISE/WISE_W4.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      739 2023-04-24 13:20:08.000000 hostphot-2.7.1/src/hostphot/filters/config.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    22710 2023-05-12 03:49:47.000000 hostphot-2.7.1/src/hostphot/global_photometry.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2488 2023-05-11 02:29:33.000000 hostphot-2.7.1/src/hostphot/image_cleaning.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    12647 2023-05-12 03:49:47.000000 hostphot-2.7.1/src/hostphot/image_masking.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    12493 2023-04-25 09:34:42.000000 hostphot-2.7.1/src/hostphot/interactive_aperture.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    13859 2023-05-11 02:29:33.000000 hostphot-2.7.1/src/hostphot/local_photometry.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9169 2023-05-11 09:42:22.000000 hostphot-2.7.1/src/hostphot/objects_detect.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    10706 2022-08-15 08:03:30.000000 hostphot-2.7.1/src/hostphot/rgb_images.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4805 2023-05-12 03:49:47.000000 hostphot-2.7.1/src/hostphot/sed_plotting.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    30315 2023-05-12 03:03:08.000000 hostphot-2.7.1/src/hostphot/utils.py
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-12 03:55:03.684277 hostphot-2.7.1/src/hostphot.egg-info/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9525 2023-05-12 03:55:03.000000 hostphot-2.7.1/src/hostphot.egg-info/PKG-INFO
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    14971 2023-05-12 03:55:03.000000 hostphot-2.7.1/src/hostphot.egg-info/SOURCES.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)        1 2023-05-12 03:55:03.000000 hostphot-2.7.1/src/hostphot.egg-info/dependency_links.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      193 2023-05-12 03:55:03.000000 hostphot-2.7.1/src/hostphot.egg-info/requires.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)        9 2023-05-12 03:55:03.000000 hostphot-2.7.1/src/hostphot.egg-info/top_level.txt
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-12 03:55:03.700277 hostphot-2.7.1/tests/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2771 2023-04-25 09:34:42.000000 hostphot-2.7.1/tests/test_cutouts.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1074 2023-05-11 02:29:33.000000 hostphot-2.7.1/tests/test_global_phot.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      460 2022-07-28 14:32:41.000000 hostphot-2.7.1/tests/test_interactivity.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1089 2023-05-11 02:29:33.000000 hostphot-2.7.1/tests/test_local_phot.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1095 2022-07-28 14:32:41.000000 hostphot-2.7.1/tests/test_preprocessing.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      861 2023-05-11 02:29:33.000000 hostphot-2.7.1/tests/test_rgb_images.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-06-22 14:21:35.867258 hostphot-2.8.0/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1065 2022-05-31 09:22:42.000000 hostphot-2.8.0/LICENSE
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       53 2022-05-31 09:22:42.000000 hostphot-2.8.0/MANIFEST.in
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    10496 2023-06-22 14:21:35.867258 hostphot-2.8.0/PKG-INFO
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9964 2023-06-22 08:14:12.000000 hostphot-2.8.0/README.md
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      187 2022-05-31 09:22:42.000000 hostphot-2.8.0/pyproject.toml
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      190 2023-05-11 02:29:33.000000 hostphot-2.8.0/requirements.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       38 2023-06-22 14:21:35.867258 hostphot-2.8.0/setup.cfg
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1251 2023-04-28 09:57:11.000000 hostphot-2.8.0/setup.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-06-22 14:21:35.811259 hostphot-2.8.0/src/
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-06-22 14:21:35.815259 hostphot-2.8.0/src/hostphot/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      439 2023-05-12 03:49:47.000000 hostphot-2.8.0/src/hostphot/__init__.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      386 2023-05-11 09:42:22.000000 hostphot-2.8.0/src/hostphot/_constants.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       47 2023-06-21 08:43:09.000000 hostphot-2.8.0/src/hostphot/_version.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1762 2022-11-14 14:06:00.000000 hostphot-2.8.0/src/hostphot/coadd.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    57543 2023-06-20 14:04:12.000000 hostphot-2.8.0/src/hostphot/cutouts.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6006 2023-05-05 10:39:56.000000 hostphot-2.8.0/src/hostphot/dust.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-06-22 14:21:35.815259 hostphot-2.8.0/src/hostphot/filters/
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-06-22 14:21:35.815259 hostphot-2.8.0/src/hostphot/filters/2MASS/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1218 2022-07-28 14:32:41.000000 hostphot-2.8.0/src/hostphot/filters/2MASS/2MASS_H.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2247 2022-07-28 14:32:41.000000 hostphot-2.8.0/src/hostphot/filters/2MASS/2MASS_J.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1596 2022-11-14 14:06:00.000000 hostphot-2.8.0/src/hostphot/filters/2MASS/2MASS_Ks.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       15 2022-07-28 14:32:41.000000 hostphot-2.8.0/src/hostphot/filters/2MASS/AAA_README
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1549 2022-07-28 14:32:41.000000 hostphot-2.8.0/src/hostphot/filters/AAA_README
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-06-22 14:21:35.815259 hostphot-2.8.0/src/hostphot/filters/DES/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       53 2022-05-31 09:22:42.000000 hostphot-2.8.0/src/hostphot/filters/DES/AAA_README
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3387 2022-07-28 14:32:41.000000 hostphot-2.8.0/src/hostphot/filters/DES/DES_Y.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4281 2022-07-28 14:32:41.000000 hostphot-2.8.0/src/hostphot/filters/DES/DES_g.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4515 2022-07-28 14:32:41.000000 hostphot-2.8.0/src/hostphot/filters/DES/DES_i.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4516 2022-07-28 14:32:41.000000 hostphot-2.8.0/src/hostphot/filters/DES/DES_r.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4338 2022-07-28 14:32:41.000000 hostphot-2.8.0/src/hostphot/filters/DES/DES_z.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-06-22 14:21:35.815259 hostphot-2.8.0/src/hostphot/filters/GALEX/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       15 2022-07-28 14:32:41.000000 hostphot-2.8.0/src/hostphot/filters/GALEX/AAA_README
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6777 2022-07-28 14:32:41.000000 hostphot-2.8.0/src/hostphot/filters/GALEX/GALEX_FUV.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    18911 2022-07-28 14:32:41.000000 hostphot-2.8.0/src/hostphot/filters/GALEX/GALEX_NUV.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-06-22 14:21:35.819259 hostphot-2.8.0/src/hostphot/filters/HST/
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-06-22 14:21:35.823259 hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    23838 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F435W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    32416 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F475W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4110 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F502N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    15624 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F550M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    31966 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F555W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    43735 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F606W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    29858 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F625W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5234 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F658N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3236 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F660N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    37258 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F775W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)   103143 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F814W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    53451 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F850LP.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7990 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F892N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21666 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR1016N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9107 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR388N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9858 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR423N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    36616 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR459M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    10646 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR462N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11519 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR505N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    12578 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR551N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    13680 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR601N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    53850 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR647M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    14675 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR656N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    15873 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR716N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    17289 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR782N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    18750 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR853N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    61170 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR914M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    19635 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR931N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1264 2023-05-05 10:39:56.000000 hostphot-2.8.0/src/hostphot/filters/HST/IR_err.txt
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-06-22 14:21:35.827259 hostphot-2.8.0/src/hostphot/filters/HST/NICMOS1/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9747 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F090M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2486 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F095N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2874 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F097N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3264 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F108N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    12445 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F110M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    24500 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F110W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3077 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F113N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    33411 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F140W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    13978 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F145M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21021 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F160W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4877 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F164N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11680 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F165M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5199 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F166N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    12148 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F170M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6879 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F187N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7831 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F190N.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-06-22 14:21:35.827259 hostphot-2.8.0/src/hostphot/filters/HST/NICMOS2/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    24275 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F110W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    20849 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F160W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    12018 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F165M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    18588 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F171M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    17947 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F180M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6506 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F187N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    41358 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F187W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5506 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F190N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21662 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F204M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    30947 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F205W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    20965 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F207M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11516 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F212N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7894 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F215N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7479 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F216N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    30813 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F222M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    26323 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F237M.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-06-22 14:21:35.831259 hostphot-2.8.0/src/hostphot/filters/HST/NICMOS3/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3240 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F108N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    24427 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F110W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3363 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F113N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    35249 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F150W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    20994 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F160W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4858 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F164N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4820 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F166N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    43711 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F175W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6876 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F187N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5510 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F190N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7212 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F196N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9291 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F200N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11541 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F212N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7906 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F215N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    30812 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F222M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    13019 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F240M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3503 2023-05-05 10:39:56.000000 hostphot-2.8.0/src/hostphot/filters/HST/UVIS1_err.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3503 2023-05-05 10:39:56.000000 hostphot-2.8.0/src/hostphot/filters/HST/UVIS2_err.txt
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-06-22 14:21:35.835259 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_IR/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     8959 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F098M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9826 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F105W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21512 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F110W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    22426 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F125W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4121 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F126N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5064 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F127M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6580 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F128N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3261 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F130N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3792 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F132N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5421 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F139M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    13977 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F140W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6752 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F153M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    10046 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F160W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4738 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F164N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6887 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F167N.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-06-22 14:21:35.847259 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)   156254 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F200LP.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21978 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F218W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    29976 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F225W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21591 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F275W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7558 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F280N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    56436 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F300X.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    15547 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F336W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    19356 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F343N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)   146819 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F350LP.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4504 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F373N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9638 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F390M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    26406 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F390W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7035 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F395N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9314 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F410M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    18697 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F438W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9833 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F467M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3637 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F469N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    32782 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F475W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    72677 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F475X.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5098 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F487N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5804 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F502N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    38578 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F547M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    63538 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F555W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    97333 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F600LP.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    51442 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F606W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21890 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F621M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    34917 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F625W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4204 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F631N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3675 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F645N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2150 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F656N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11299 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F657N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3236 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F658N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11865 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F665N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11991 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F673N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    13792 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F680N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    20007 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F689M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    19898 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F763M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    36590 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F775W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    54378 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F814W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    33733 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F845M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    57316 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F850LP.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    12497 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F953N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    13422 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ232N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    13900 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ243N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21137 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ378N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6727 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ387N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    39729 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ422M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11393 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ436N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1548 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ437N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    22828 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ492N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    26635 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ508N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4658 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ575N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    19283 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ619N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    20492 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ634N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4687 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ672N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4387 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ674N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    24973 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ727N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    25138 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ750N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2950 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ889N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2948 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ906N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3346 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ924N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3461 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ937N.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-06-22 14:21:35.859259 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)   156503 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F200LP.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    20752 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F218W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    29190 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F225W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21479 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F275W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7566 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F280N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    55542 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F300X.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    15542 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F336W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    19332 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F343N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)   147032 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F350LP.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4495 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F373N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9640 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F390M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    26441 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F390W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7031 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F395N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9300 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F410M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    18727 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F438W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9871 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F467M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3641 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F469N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    32751 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F475W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    72732 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F475X.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5104 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F487N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5798 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F502N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    38608 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F547M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    63493 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F555W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    97494 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F600LP.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    51384 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F606W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21858 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F621M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    34960 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F625W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4209 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F631N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3686 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F645N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2154 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F656N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11309 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F657N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3233 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F658N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11857 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F665N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11991 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F673N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    13805 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F680N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    20019 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F689M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    19919 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F763M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    36600 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F775W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    54473 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F814W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    33739 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F845M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    57507 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F850LP.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    12507 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F953N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    13422 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ232N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    13900 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ243N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21137 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ378N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6727 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ387N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    39729 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ422M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11393 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ436N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1548 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ437N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    22828 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ492N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    26635 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ508N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4658 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ575N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    19283 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ619N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    20492 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ634N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4687 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ672N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4387 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ674N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    24973 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ727N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    25138 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ750N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2950 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ889N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2948 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ906N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3346 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ924N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3461 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ937N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2012 2023-05-05 10:39:56.000000 hostphot-2.8.0/src/hostphot/filters/HST/ir_aper_corrections.csv
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    18667 2023-05-05 10:39:56.000000 hostphot-2.8.0/src/hostphot/filters/HST/wfc3uvis1_aper_007_syn.csv
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    18635 2023-05-05 10:39:56.000000 hostphot-2.8.0/src/hostphot/filters/HST/wfc3uvis2_aper_007_syn.csv
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-06-22 14:21:35.859259 hostphot-2.8.0/src/hostphot/filters/LegacySurvey/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2281 2022-11-14 14:06:00.000000 hostphot-2.8.0/src/hostphot/filters/LegacySurvey/BASS_g.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3180 2022-11-14 14:06:00.000000 hostphot-2.8.0/src/hostphot/filters/LegacySurvey/BASS_r.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21743 2022-11-14 14:06:00.000000 hostphot-2.8.0/src/hostphot/filters/LegacySurvey/DECAM_g.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21627 2023-05-19 13:15:53.000000 hostphot-2.8.0/src/hostphot/filters/LegacySurvey/DECAM_r.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21627 2023-05-19 13:15:45.000000 hostphot-2.8.0/src/hostphot/filters/LegacySurvey/DECAM_z.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7028 2022-11-14 14:06:00.000000 hostphot-2.8.0/src/hostphot/filters/LegacySurvey/MzLS_z.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      300 2022-11-14 14:06:00.000000 hostphot-2.8.0/src/hostphot/filters/LegacySurvey/README.txt
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-06-22 14:21:35.863258 hostphot-2.8.0/src/hostphot/filters/PS1/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      136 2022-05-31 09:22:42.000000 hostphot-2.8.0/src/hostphot/filters/PS1/AAA_README.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3717 2022-07-28 14:32:41.000000 hostphot-2.8.0/src/hostphot/filters/PS1/PS1_g.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3759 2022-07-28 14:32:41.000000 hostphot-2.8.0/src/hostphot/filters/PS1/PS1_i.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3885 2022-07-28 14:32:41.000000 hostphot-2.8.0/src/hostphot/filters/PS1/PS1_r.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4385 2022-07-28 14:32:41.000000 hostphot-2.8.0/src/hostphot/filters/PS1/PS1_y.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3486 2022-07-28 14:32:41.000000 hostphot-2.8.0/src/hostphot/filters/PS1/PS1_z.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-06-22 14:21:35.863258 hostphot-2.8.0/src/hostphot/filters/SDSS/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       72 2022-05-31 09:22:42.000000 hostphot-2.8.0/src/hostphot/filters/SDSS/AAA_README
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1414 2022-07-28 14:32:41.000000 hostphot-2.8.0/src/hostphot/filters/SDSS/SDSS_g.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1260 2022-07-28 14:32:41.000000 hostphot-2.8.0/src/hostphot/filters/SDSS/SDSS_i.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1176 2022-07-28 14:32:41.000000 hostphot-2.8.0/src/hostphot/filters/SDSS/SDSS_r.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4718 2022-07-28 14:32:41.000000 hostphot-2.8.0/src/hostphot/filters/SDSS/SDSS_u.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2509 2022-07-28 14:32:41.000000 hostphot-2.8.0/src/hostphot/filters/SDSS/SDSS_z.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-06-22 14:21:35.863258 hostphot-2.8.0/src/hostphot/filters/SPLUS/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      733 2023-05-17 13:41:13.000000 hostphot-2.8.0/src/hostphot/filters/SPLUS/SPLUS_F378.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      514 2023-05-17 13:41:17.000000 hostphot-2.8.0/src/hostphot/filters/SPLUS/SPLUS_F395.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      915 2023-05-17 13:41:20.000000 hostphot-2.8.0/src/hostphot/filters/SPLUS/SPLUS_F410.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      967 2023-05-17 13:41:23.000000 hostphot-2.8.0/src/hostphot/filters/SPLUS/SPLUS_F430.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      823 2023-05-17 13:41:27.000000 hostphot-2.8.0/src/hostphot/filters/SPLUS/SPLUS_F515.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      666 2023-05-17 13:41:31.000000 hostphot-2.8.0/src/hostphot/filters/SPLUS/SPLUS_F660.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1790 2023-05-17 13:41:36.000000 hostphot-2.8.0/src/hostphot/filters/SPLUS/SPLUS_F861.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4729 2023-05-17 13:41:25.000000 hostphot-2.8.0/src/hostphot/filters/SPLUS/SPLUS_g.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5987 2023-05-17 13:41:33.000000 hostphot-2.8.0/src/hostphot/filters/SPLUS/SPLUS_i.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4933 2023-05-17 13:41:29.000000 hostphot-2.8.0/src/hostphot/filters/SPLUS/SPLUS_r.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2942 2023-05-17 13:41:10.000000 hostphot-2.8.0/src/hostphot/filters/SPLUS/SPLUS_u.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7675 2023-05-17 13:41:37.000000 hostphot-2.8.0/src/hostphot/filters/SPLUS/SPLUS_z.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    92457 2023-06-14 11:39:11.000000 hostphot-2.8.0/src/hostphot/filters/SPLUS/iDR3_zps.cat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-06-22 14:21:35.863258 hostphot-2.8.0/src/hostphot/filters/SkyMapper/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      605 2023-05-17 13:38:06.000000 hostphot-2.8.0/src/hostphot/filters/SkyMapper/SkyMapper_g.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      451 2023-05-17 13:38:11.000000 hostphot-2.8.0/src/hostphot/filters/SkyMapper/SkyMapper_i.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      561 2023-05-17 13:38:09.000000 hostphot-2.8.0/src/hostphot/filters/SkyMapper/SkyMapper_r.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      209 2023-05-17 13:37:58.000000 hostphot-2.8.0/src/hostphot/filters/SkyMapper/SkyMapper_u.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      176 2023-05-17 13:38:02.000000 hostphot-2.8.0/src/hostphot/filters/SkyMapper/SkyMapper_v.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      574 2023-05-17 13:38:14.000000 hostphot-2.8.0/src/hostphot/filters/SkyMapper/SkyMapper_z.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-06-22 14:21:35.867258 hostphot-2.8.0/src/hostphot/filters/Spitzer/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      189 2022-11-14 14:06:00.000000 hostphot-2.8.0/src/hostphot/filters/Spitzer/README.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     8211 2022-11-14 14:06:00.000000 hostphot-2.8.0/src/hostphot/filters/Spitzer/Spitzer_IRAC.1.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     8421 2022-11-14 14:06:00.000000 hostphot-2.8.0/src/hostphot/filters/Spitzer/Spitzer_IRAC.2.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6531 2022-11-14 14:06:00.000000 hostphot-2.8.0/src/hostphot/filters/Spitzer/Spitzer_IRAC.3.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7375 2022-11-14 14:06:00.000000 hostphot-2.8.0/src/hostphot/filters/Spitzer/Spitzer_IRAC.4.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2816 2022-11-14 14:06:00.000000 hostphot-2.8.0/src/hostphot/filters/Spitzer/Spitzer_MIPS.1.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-06-22 14:21:35.867258 hostphot-2.8.0/src/hostphot/filters/UKIDSS/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    16346 2023-05-17 13:39:56.000000 hostphot-2.8.0/src/hostphot/filters/UKIDSS/UKIDSS_H.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     8998 2023-05-17 13:39:53.000000 hostphot-2.8.0/src/hostphot/filters/UKIDSS/UKIDSS_J.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    20900 2023-05-17 13:39:59.000000 hostphot-2.8.0/src/hostphot/filters/UKIDSS/UKIDSS_K.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6065 2023-05-17 13:39:51.000000 hostphot-2.8.0/src/hostphot/filters/UKIDSS/UKIDSS_Y.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5166 2023-05-17 13:39:48.000000 hostphot-2.8.0/src/hostphot/filters/UKIDSS/UKIDSS_Z.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-06-22 14:21:35.867258 hostphot-2.8.0/src/hostphot/filters/VISTA/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       52 2023-05-19 13:51:07.000000 hostphot-2.8.0/src/hostphot/filters/VISTA/README.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11368 2023-05-19 13:49:59.000000 hostphot-2.8.0/src/hostphot/filters/VISTA/VISTA_H.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7550 2023-05-19 13:49:54.000000 hostphot-2.8.0/src/hostphot/filters/VISTA/VISTA_J.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    13156 2023-05-19 13:50:03.000000 hostphot-2.8.0/src/hostphot/filters/VISTA/VISTA_Ks.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5530 2023-05-19 13:49:46.000000 hostphot-2.8.0/src/hostphot/filters/VISTA/VISTA_Y.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3880 2023-05-19 13:49:32.000000 hostphot-2.8.0/src/hostphot/filters/VISTA/VISTA_Z.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-06-22 14:21:35.867258 hostphot-2.8.0/src/hostphot/filters/WISE/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       15 2022-07-28 14:32:41.000000 hostphot-2.8.0/src/hostphot/filters/WISE/AAA_README
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2961 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/WISE/WISE_W1.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3528 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/WISE/WISE_W2.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    24404 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/WISE/WISE_W3.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    19734 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/filters/WISE/WISE_W4.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1023 2023-06-14 11:36:52.000000 hostphot-2.8.0/src/hostphot/filters/config.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    24238 2023-06-22 11:23:39.000000 hostphot-2.8.0/src/hostphot/global_photometry.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2488 2023-05-11 02:29:33.000000 hostphot-2.8.0/src/hostphot/image_cleaning.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    13402 2023-06-07 14:05:26.000000 hostphot-2.8.0/src/hostphot/image_masking.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    12493 2023-04-25 09:34:42.000000 hostphot-2.8.0/src/hostphot/interactive_aperture.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    15066 2023-06-22 11:22:57.000000 hostphot-2.8.0/src/hostphot/local_photometry.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9169 2023-06-07 14:06:07.000000 hostphot-2.8.0/src/hostphot/objects_detect.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    10706 2022-08-15 08:03:30.000000 hostphot-2.8.0/src/hostphot/rgb_images.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7550 2023-06-22 13:15:47.000000 hostphot-2.8.0/src/hostphot/sed_plotting.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    32580 2023-06-22 12:42:45.000000 hostphot-2.8.0/src/hostphot/utils.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-06-22 14:21:35.815259 hostphot-2.8.0/src/hostphot.egg-info/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    10496 2023-06-22 14:21:35.000000 hostphot-2.8.0/src/hostphot.egg-info/PKG-INFO
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    15887 2023-06-22 14:21:35.000000 hostphot-2.8.0/src/hostphot.egg-info/SOURCES.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)        1 2023-06-22 14:21:35.000000 hostphot-2.8.0/src/hostphot.egg-info/dependency_links.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      193 2023-06-22 14:21:35.000000 hostphot-2.8.0/src/hostphot.egg-info/requires.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)        9 2023-06-22 14:21:35.000000 hostphot-2.8.0/src/hostphot.egg-info/top_level.txt
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-06-22 14:21:35.867258 hostphot-2.8.0/tests/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3327 2023-06-22 09:06:14.000000 hostphot-2.8.0/tests/test_cutouts.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1074 2023-05-11 02:29:33.000000 hostphot-2.8.0/tests/test_global_phot.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      460 2022-07-28 14:32:41.000000 hostphot-2.8.0/tests/test_interactivity.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1089 2023-05-11 02:29:33.000000 hostphot-2.8.0/tests/test_local_phot.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1095 2022-07-28 14:32:41.000000 hostphot-2.8.0/tests/test_preprocessing.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      861 2023-05-11 02:29:33.000000 hostphot-2.8.0/tests/test_rgb_images.py
```

### Comparing `hostphot-2.7.1/LICENSE` & `hostphot-2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/PKG-INFO` & `hostphot-2.8.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: hostphot
-Version: 2.7.1
-Summary: Global and local photometry of galaxies hosting supernovae or other transients
-Home-page: https://github.com/temuller/hostphot
-Author: Tomás Enrique Müller-Bravo and Lluís Galbany
-Author-email: t.e.muller-bravo@ice.csic.es
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <p align="center">
 	<img src="docs/hostphot_logo.png" alt="drawing" width="300"/>
 </p>
 
 Global and local photometry of galaxies hosting supernovae or other transients
 
 [![repo](https://img.shields.io/badge/GitHub-temuller%2Fhostphot-blue.svg?style=flat)](https://github.com/temuller/hostphot)
@@ -192,14 +177,27 @@
   number = {76}, 
   pages = {4508},  
   journal = {Journal of Open Source Software} 
 } 
 ```
 
 ## What's new!
+v2.8.0
+* Fix SED plotting with negative or too large values/errors, and improve plotting aesthetics
+* Fix problem downloading some 2MASS images giving internal server error (no image overlap)
+* Adding UKIDSS, SPLUS and SkyMapper surveys. WARNINGS: SkyMapper photometry (DR2) is not very accurate with extended sources!
+* The marker showing the galaxy position on images has changed colour for better visualization
+* Adding functions to easily load previously saved parameteres from pickle files
+* Adding missing extinction correction for flux (not magnitudes)
+* Including exposure time into flux for PS1, VISTA and UKIDSS surveys
+* Adding SDSS ZP offsets into flux
+* Output zeropoint together with the photometry
+* Updating LegacySurvey errors, taken from inverse-variance maps and ZP uncertainty
+* Adding missing offsets to unWISE W1 and W2 bands into fluxes
+* Kron radius is no longer "optimized", just the scale, which doesn't have any effect in practice for the user
 v2.7.1
 * Adding SED plotting
 * Fixed plotting angle of masked object 
 v2.7.0
 * MAJOR BUG: Convertion factor between different pixel scales fixed (it was previously inverted). This affects the common aperture photometry between different surveys!
 * Moving font family to `_constant.py` file
 v2.6.2
```

### Comparing `hostphot-2.7.1/README.md` & `hostphot-2.8.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: hostphot
+Version: 2.8.0
+Summary: Global and local photometry of galaxies hosting supernovae or other transients
+Home-page: https://github.com/temuller/hostphot
+Author: Tomás Enrique Müller-Bravo and Lluís Galbany
+Author-email: t.e.muller-bravo@ice.csic.es
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <p align="center">
 	<img src="docs/hostphot_logo.png" alt="drawing" width="300"/>
 </p>
 
 Global and local photometry of galaxies hosting supernovae or other transients
 
 [![repo](https://img.shields.io/badge/GitHub-temuller%2Fhostphot-blue.svg?style=flat)](https://github.com/temuller/hostphot)
@@ -177,14 +192,27 @@
   number = {76}, 
   pages = {4508},  
   journal = {Journal of Open Source Software} 
 } 
 ```
 
 ## What's new!
+v2.8.0
+* Fix SED plotting with negative or too large values/errors, and improve plotting aesthetics
+* Fix problem downloading some 2MASS images giving internal server error (no image overlap)
+* Adding UKIDSS, SPLUS and SkyMapper surveys. WARNINGS: SkyMapper photometry (DR2) is not very accurate with extended sources!
+* The marker showing the galaxy position on images has changed colour for better visualization
+* Adding functions to easily load previously saved parameteres from pickle files
+* Adding missing extinction correction for flux (not magnitudes)
+* Including exposure time into flux for PS1, VISTA and UKIDSS surveys
+* Adding SDSS ZP offsets into flux
+* Output zeropoint together with the photometry
+* Updating LegacySurvey errors, taken from inverse-variance maps and ZP uncertainty
+* Adding missing offsets to unWISE W1 and W2 bands into fluxes
+* Kron radius is no longer "optimized", just the scale, which doesn't have any effect in practice for the user
 v2.7.1
 * Adding SED plotting
 * Fixed plotting angle of masked object 
 v2.7.0
 * MAJOR BUG: Convertion factor between different pixel scales fixed (it was previously inverted). This affects the common aperture photometry between different surveys!
 * Moving font family to `_constant.py` file
 v2.6.2
```

### Comparing `hostphot-2.7.1/setup.py` & `hostphot-2.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/coadd.py` & `hostphot-2.8.0/src/hostphot/coadd.py`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/cutouts.py` & `hostphot-2.8.0/src/hostphot/cutouts.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,20 +15,21 @@
 from astropy.io import fits
 from astropy.table import Table
 from astropy import wcs, units as u
 from astropy.coordinates import SkyCoord
 from astropy.nddata import Cutout2D
 
 import pyvo  # 2MASS
-from pyvo.dal import sia  # DES, DELVE
+from pyvo.dal import sia  # DES, SkyMapper, S-Plus
 from astroquery.sdss import SDSS
+from astroquery.ukidss import Ukidss
 from astroquery.skyview import SkyView  # other surveys
 from astroquery.mast import Observations  # for GALEX
 
-from astroquery.esa.hubble import ESAHubble
+from astroquery.esa.hubble import ESAHubble  # HST
 
 esahubble = ESAHubble()
 
 from reproject import reproject_interp
 
 from hostphot._constants import workdir
 from hostphot.utils import (
@@ -36,14 +37,16 @@
     clean_dir,
     check_work_dir,
     check_survey_validity,
     check_filters_validity,
     check_HST_filters,
     survey_pixel_scale,
 )
+import hostphot
+hostphot_path = hostphot.__path__[0]
 
 import warnings
 from astropy.utils.exceptions import AstropyWarning
 
 
 # PS1
 # ----------------------------------------
@@ -778,21 +781,30 @@
                 tile_url = os.path.join(f"{ordate}{hemisphere}", f"s{scanno}")
                 fits_url = os.path.join("image", f"{fname}.gz")
                 params_url = f"center={ra},{dec}&size={size_degree}degree&gzip=0"  # center and size of the image
 
                 url = os.path.join(
                     base_url, tile_url, fits_url + "?" + params_url
                 )
-                hdu = fits.open(url)
-                ny, nx = hdu[0].data.shape
-                sizes.append(nx * ny)
-                tmp_hdu_list.append(hdu)
+                try:
+                    hdu = fits.open(url)
+                    ny, nx = hdu[0].data.shape
+                    sizes.append(nx * ny)
+                    tmp_hdu_list.append(hdu)
+                except:
+                    # some images might give 500 Internal Server Error
+                    # because the cutout does not overlap the image
+                    pass
 
-            i = np.argmax(sizes)
-            hdu_list.append(tmp_hdu_list[i])
+            if len(tmp_hdu_list)==0:
+                hdu_list.append(None)
+            else:
+                # pick largest image, which usually is the best
+                i = np.argmax(sizes)
+                hdu_list.append(tmp_hdu_list[i])
 
     return hdu_list
 
 
 # Legacy Survey
 def get_LegacySurvey_images(ra, dec, size=3, filters=None, version="dr10"):
     """Gets Legacy Survey fits images for the given coordinates and
@@ -828,25 +840,35 @@
         size_arcsec = size.to(u.arcsec).value
     size_pixels = int(size_arcsec / pixel_scale)
 
     if version is None:
         version = "dr10"  # latest data release
 
     base_url = "https://www.legacysurvey.org/viewer/fits-cutout?"
-    params = f"ra={ra}&dec={dec}&layer=ls-{version}&pixscale={pixel_scale}&bands={filters}&size={size_pixels}"
+    params = f"ra={ra}&dec={dec}&layer=ls-{version}&pixscale={pixel_scale}&bands={filters}&size={size_pixels}&invvar"
     url = base_url + params
+
     master_hdu = fits.open(url)
-    header = master_hdu[0].header
+    master_header = master_hdu[0].header
+    master_header_invvar = master_hdu[1].header
 
     hdu_list = []
-    # assuming order grz of the filters
     for i, filt in enumerate(filters):
         data = master_hdu[0].data[i]
+        header = master_header.copy()
+        header.append(('BAND', filt, ' Band - added by HostPhot'), end=True)
         hdu = fits.PrimaryHDU(data=data, header=header)
-        hdu_list.append(hdu)
+        
+        header_invvar = master_header_invvar.copy()
+        header_invvar.append(('BAND', filt, ' Band - added by HostPhot'), end=True)
+        data_invvar = master_hdu[1].data[i]
+        hdu_invvar = fits.ImageHDU(data=data_invvar, 
+                                header=header_invvar)
+
+        hdu_list.append(fits.HDUList([hdu, hdu_invvar]))
 
     return hdu_list
 
 
 # Spitzer
 def get_Spitzer_images(ra, dec, size=3, filters=None):
     """Gets Spitzer fits images for the given coordinates and
@@ -1014,17 +1036,35 @@
                 urls_dict[filt] = url
                 break
 
     hdu_list = []
     for filt, url in urls_dict.items():
         if url is not None:
             hdu = fits.open(url)
-            # to be consistent with the naming of other surveys
-            hdu[1].header["MAGZP"] = hdu[1].header["MAGZPT"]
-            hdu_list.append(hdu[1])  # extension 1
+
+            hdu[0].data = hdu[1].data
+            with warnings.catch_warnings():
+                warnings.simplefilter("ignore", AstropyWarning)
+                img_wcs = wcs.WCS(hdu[1].header)
+                hdu[0].header.update(img_wcs.to_header())
+                
+                # add some keywords to the PHU
+                hdu[0].header['EXPTIME'] = hdu[1].header['EXPTIME']
+                hdu[0].header['MAGZRR'] = hdu[1].header['MAGZRR']
+
+                # calculate effective ZP (considering atmospheric extinction)
+                # calculate extinction first
+                airmass = (hdu[1].header['HIERARCH ESO TEL AIRM START'] + hdu[1].header['HIERARCH ESO TEL AIRM END'])/2
+                ext_coeff = hdu[1].header['EXTINCT']
+                extinction = ext_coeff*(airmass - 1)
+                # calculate effective ZP
+                zp = hdu[1].header['MAGZPT']
+                hdu[0].header['MAGZP'] = zp - extinction
+
+            hdu_list.append(hdu)
         else:
             hdu_list.append(None)
 
     return hdu_list
 
 
 # HST
@@ -1210,15 +1250,15 @@
 
     update_HST_header(hdu)
     hdu_list = [hdu]
 
     return hdu_list
 
 
-def get_HST_images_OLD(ra, dec, size=3, filt=None, instrument=None):
+def _get_HST_images_OLD(ra, dec, size=3, filt=None, instrument=None):
     """Downloads a set of HST fits images for a given set
     of coordinates and filters using the MAST archive.
 
     Parameters
     ----------
     ra: str or float
         Right ascension in degrees.
@@ -1316,14 +1356,295 @@
 
         trimmed_data = Cutout2D(hdu[0].data, pos, size_pixels, img_wcs)
         hdu[0].data = trimmed_data.data
         hdu[0].header.update(trimmed_data.wcs.to_header())
 
     return hdu_list
 
+# SkyMapper
+def get_SkyMapper_urls(ra, dec, fov, filters="uvgriz"):
+    """Obtains the URLs of the SkyMapper images.
+    
+    The images closest to the given coordinates are retrieved 
+
+    Parameters
+    ----------
+    ra: float
+        Right ascension in degrees.
+    dec: float
+        Declination in degrees.
+    fov: float
+        Field of view in degrees.
+    filters: str, default ``None``
+        Filters to use. If ``None``, uses ``uvgriz``.
+
+    Returns
+    -------
+    url_list: list
+        List of URLs with SkyMapper images.
+    """
+    sm_url = "https://api.skymapper.nci.org.au/public/siap/dr2/query"
+    svc = sia.SIAService(sm_url)
+    imgs_table = svc.search(
+        (ra, dec), (fov / np.cos(dec * np.pi / 180), fov), verbosity=2
+    )
+    if len(imgs_table) == 0:
+        print(("Warning: empty table returned for " f"ra={ra}, dec={dec}"))
+        return None
+
+    imgs_df = pd.DataFrame(imgs_table)
+    imgs_df = imgs_df[imgs_df.format.str.endswith('fits')]
+    if len(imgs_df) == 0:
+        return None
+
+    url_list = []
+    for filt in filters:
+        filt_df = imgs_df[imgs_df.band==filt]
+        # obtain the images with largest exposure times and file size
+        # and lowest mean FWHM, as suggested by Christopher Onken, from the SkyMapper Team
+        filt_df = filt_df[filt_df.exptime==filt_df.exptime.max()]
+        filt_df = filt_df[filt_df.filesize==filt_df.filesize.max()]
+        filt_df = filt_df[filt_df.mean_fwhm==filt_df.mean_fwhm.min()]
+        if len(filt_df) == 0:
+            url_list.append(None)
+        else:
+            fits_url = filt_df.get_fits.values[0]
+            url_list.append(fits_url)
+            
+    return url_list
+
+def get_SkyMapper_images(ra, dec, size=3, filters=None):
+    """Gets SkyMapper fits images for the given coordinates and
+    filters.
+
+    Parameters
+    ----------
+    ra: float
+        Right Ascension in degrees.
+    dec: float
+        Declination in degrees.
+    size: float or ~astropy.units.Quantity, default ``3``
+        Image size. If a float is given, the units are assumed to be arcmin.
+    filters: str, default ``None``
+        Filters to use. If ``None``, uses ``uvgriz``.
+
+    Returns
+    -------
+    hdu_list: list
+        List of fits images.
+    """
+    survey = "SkyMapper"
+    if filters is None:
+        filters = get_survey_filters(survey)
+    check_filters_validity(filters, survey)
+
+    if isinstance(size, (float, int)):
+        fov = (size * u.arcmin).to(u.degree).value
+    else:
+        fov = size.to(u.degree).value
+
+    url_list = get_SkyMapper_urls(ra, dec, fov, filters)
+
+    if url_list is None:
+        return None
+
+    hdu_list = []
+    for url in url_list:
+        if url is None:
+            hdu_list.append(None)
+        else:
+            hdu = fits.open(url)
+            # add zeropoint
+            hdu[0].header['MAGZP'] = hdu[0].header['ZPAPPROX']
+            hdu_list.append(hdu)
+
+    return hdu_list
+
+# S-Plus
+def get_SPlus_urls(ra, dec, fov, filters=None):
+    """Obtains the URLs of the S-Plus images.
+    
+    The available filters are: 'F378', 'F395', 'F410', 'F430', 
+    'F515', 'F660', 'F861', 'G', 'I', 'R', 'U', 'Z'.
+
+    Parameters
+    ----------
+    ra: float
+        Right ascension in degrees.
+    dec: float
+        Declination in degrees.
+    fov: float
+        Field of view in degrees.
+    filters: str, default ``None``
+        Filters to use. If ``None``, uses all available filters.
+
+    Returns
+    -------
+    url_list: list
+        List of URLs with S-Plus images.
+    """
+    splus_url = "https://datalab.noirlab.edu/sia/splus_dr1"
+    svc = sia.SIAService(splus_url)
+    imgs_table = svc.search(
+        (ra, dec), (fov / np.cos(dec * np.pi / 180), fov), verbosity=2
+    )
+    if len(imgs_table) == 0:
+        print(("Warning: empty table returned for " f"ra={ra}, dec={dec}"))
+        return None
+
+    imgs_df = pd.DataFrame(imgs_table)
+    imgs_df = imgs_df[imgs_df.access_format.str.endswith('fits')]
+    if len(imgs_df) == 0:
+        return None
+
+    url_list = []
+    for filt in filters:
+        filt_df = imgs_df[imgs_df.obs_bandpass==filt]
+        if len(filt_df) == 0:
+            url_list.append(None)
+        else:
+            fits_url = filt_df.access_url.values[0]  # first image
+            url_list.append(fits_url)
+            
+    return url_list
+
+def get_SPLUS_images(ra, dec, size=3, filters=None):
+    """Gets S-Plus fits images for the given coordinates and
+    filters.
+
+    The available filters are: 'F378', 'F395', 'F410', 'F430', 
+    'F515', 'F660', 'F861', 'G', 'I', 'R', 'U', 'Z'.
+
+    Parameters
+    ----------
+    ra: float
+        Right Ascension in degrees.
+    dec: float
+        Declination in degrees.
+    size: float or ~astropy.units.Quantity, default ``3``
+        Image size. If a float is given, the units are assumed to be arcmin.
+    filters: str, default ``None``
+        Filters to use. If ``None``, uses all available filters.
+
+    Returns
+    -------
+    hdu_list: list
+        List of fits images.
+    """
+    global hostphot_path
+    survey = "SPLUS"
+    if filters is None:
+        filters = get_survey_filters(survey)
+    check_filters_validity(filters, survey)
+
+    if isinstance(size, (float, int)):
+        fov = (size * u.arcmin).to(u.degree).value
+    else:
+        fov = size.to(u.degree).value
+
+    url_list = get_SPlus_urls(ra, dec, fov, filters)
+
+    if url_list is None:
+        return None
+
+    hdu_list = []
+    for url in url_list:
+        if url is None:
+            hdu_list.append(None)
+        else:
+            hdu = fits.open(url)
+
+            # add zeropoint
+            # file from https://splus.cloud/documentation/dr2_3
+            zps_file = os.path.join(hostphot_path, 'filters', 'SPLUS', 'iDR3_zps.cat')
+            zps_df = pd.read_csv(zps_file, delim_whitespace=True)
+
+            field = hdu[0].header['OBJECT'].replace('_', '-')
+            field_df = zps_df[zps_df['#field']==field]
+            img_filt = hdu[0].header['FILTER']
+            zp = field_df[img_filt].values[0]
+            hdu[0].header['MAGZP'] = zp
+
+            # initial EXPTIME is normalised, so it doesn't help
+            hdu[0].header['EXPTIME'] = hdu[0].header['TEXPOSED']
+
+            hdu_list.append(hdu)
+
+    return hdu_list
+
+# UKIDSS
+def get_UKIDSS_images(ra, dec, size=3, filters='ZYJHK'):
+    """Gets UKIDSS fits images for the given coordinates and
+    filters.
+
+    Parameters
+    ----------
+    ra: float
+        Right Ascension in degrees.
+    dec: float
+        Declination in degrees.
+    size: float or ~astropy.units.Quantity, default ``3``
+        Image size. If a float is given, the units are assumed to be arcmin.
+    filters: str, default ``None``
+        Filters to use. If ``None``, uses ``ZYJHK``.
+
+    Returns
+    -------
+    fits_files: list
+        List of fits images.
+    """
+    survey = "UKIDSS"
+    if filters is None:
+        filters = get_survey_filters(survey)
+    check_filters_validity(filters, survey)
+    
+    database = 'UKIDSSDR11PLUS'
+    # programme = 'LAS'  # ['UDS', 'GCS', 'GPS', 'DXS', 'LAS']
+    
+    survey_pixel_scale(survey)
+    if isinstance(size, (float, int)):
+        size = (size * u.arcmin)
+
+    u_obj = Ukidss(database=database)
+    pos = SkyCoord(ra, dec, unit="deg")
+    urls = u_obj.get_image_list(pos, waveband='all', frame_type="stack", image_width=size)
+
+    hdu_dict = {filt:None for filt in filters}
+    for filt in filters:
+        for url in urls:
+            # pick the first FITS image only (is this correct?)
+            if f'band={filt}' in url:
+                hdu = fits.open(url)
+
+                # update first extension with data and WCS
+                hdu[0].data = hdu[1].data
+                with warnings.catch_warnings():
+                    warnings.simplefilter("ignore", AstropyWarning)
+                    img_wcs = wcs.WCS(hdu[1].header)
+                    hdu[0].header.update(img_wcs.to_header())
+                # add some of the keywords to the PHU
+                hdu[0].header['MAGZRR'] = hdu[1].header['MAGZRR']
+                hdu[0].header['GAIN'] = hdu[1].header['GAIN']
+                hdu[0].header['READNOIS'] = hdu[1].header['READNOIS']
+
+                # calculate effective ZP (considering atmospheric extinction)
+                # calculate extinction first
+                airmass = (hdu[0].header['AMSTART'] + hdu[0].header['AMEND'])/2
+                ext_coeff = hdu[1].header['EXTINCT']
+                extinction = ext_coeff*(airmass - 1)
+                # calculate effective ZP
+                zp = hdu[1].header['MAGZPT']
+                hdu[0].header['MAGZP'] = zp - extinction
+
+                hdu_dict[filt] = hdu
+                break                
+
+    hdu_list = list(hdu_dict.values())
+    
+    return hdu_list
 
 # Check orientation
 # ------------------
 def match_wcs(fits_files):
     """Matches the WCS of all the images, taking the first ones as
     a reference.
 
@@ -1347,14 +1668,44 @@
         for hdu in matched_fits_files[1:]:
             data, footprint = reproject_interp(hdu[0], hdu0.header)
             hdu[0].data = data
             hdu[0].header.update(wcs0.to_header())
 
     return matched_fits_files
 
+def check_existing_images(name, filters, survey):
+    """Checks if images exist for the given filters+survey
+    combination, for the given object.
+
+    Parameters
+    ----------
+    name : str
+        Name of the object.
+    filters : str or list
+        Filters to use.
+    survey : str
+        Survey name.
+
+    Returns
+    -------
+    filters_without_image: list
+        Filters without images.
+    """
+    check_survey_validity(survey)
+
+    check_work_dir(workdir)
+    obj_dir = os.path.join(workdir, name) 
+    
+    filters_without_image = []
+    for filt in filters:
+        filt_image = os.path.join(obj_dir, f'{survey}_{filt}.fits')
+        if os.path.isfile(filt_image) is False:
+            filters_without_image.append(filt)
+
+    return filters_without_image
 
 # Master Function
 # ----------------------------------------
 def download_images(
     name,
     ra,
     dec,
@@ -1403,14 +1754,20 @@
     check_survey_validity(survey)
 
     check_work_dir(workdir)
     obj_dir = os.path.join(workdir, name)
     if not os.path.isdir(obj_dir):
         os.mkdir(obj_dir)
 
+    if filters is None:
+        filters = get_survey_filters(survey)
+
+    if overwrite is False:
+        filters = check_existing_images(name, filters, survey)
+    
     # download fits files
     if survey == "PS1":
         hdu_list = get_PS1_images(ra, dec, size, filters)
     elif survey == "DES":
         hdu_list = get_DES_images(ra, dec, size, filters)
     elif survey == "SDSS":
         hdu_list = get_SDSS_images(ra, dec, size, filters, version)
@@ -1418,30 +1775,33 @@
         hdu_list = get_GALEX_images(ra, dec, size, filters, version)
     elif survey == "WISE":
         hdu_list = get_WISE_images(ra, dec, size, filters)
     elif survey == "unWISE":
         hdu_list = get_unWISE_images(ra, dec, size, filters, version)
     elif survey == "2MASS":
         hdu_list = get_2MASS_images(ra, dec, size, filters)
-    elif survey == "HST":
-        hdu_list = get_HST_images(ra, dec, size, filters)
     elif survey == "LegacySurvey":
         hdu_list = get_LegacySurvey_images(ra, dec, size, filters, version)
     elif survey == "Spitzer":
         hdu_list = get_Spitzer_images(ra, dec, size, filters)
     elif survey == "VISTA":
         hdu_list = get_VISTA_images(ra, dec, size, filters, version)
+    elif survey == "HST":
+        hdu_list = get_HST_images(ra, dec, size, filters)
+    elif survey == "SkyMapper":
+        hdu_list = get_SkyMapper_images(ra, dec, size, filters)
+    elif survey == "SPLUS":
+        hdu_list = get_SPLUS_images(ra, dec, size, filters)
+    elif survey == "UKIDSS":
+        hdu_list = get_UKIDSS_images(ra, dec, size, filters)
     else:
         raise ValueError(
             "The given survey is not properly added to HostPhot..."
         )
-
-    if filters is None:
-        filters = get_survey_filters(survey)
-
+    
     if hdu_list:
         for hdu, filt in zip(hdu_list, filters):
             if hdu is None:
                 continue  # skip missing filter/image
 
             if survey == "HST":
                 inst = version.replace("/", "-")
```

### Comparing `hostphot-2.7.1/src/hostphot/dust.py` & `hostphot-2.8.0/src/hostphot/dust.py`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/2MASS/2MASS_H.dat` & `hostphot-2.8.0/src/hostphot/filters/2MASS/2MASS_H.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/2MASS/2MASS_J.dat` & `hostphot-2.8.0/src/hostphot/filters/2MASS/2MASS_J.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/2MASS/2MASS_Ks.dat` & `hostphot-2.8.0/src/hostphot/filters/2MASS/2MASS_Ks.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/AAA_README` & `hostphot-2.8.0/src/hostphot/filters/AAA_README`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/DES/DES_Y.dat` & `hostphot-2.8.0/src/hostphot/filters/DES/DES_Y.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/DES/DES_g.dat` & `hostphot-2.8.0/src/hostphot/filters/DES/DES_g.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/DES/DES_i.dat` & `hostphot-2.8.0/src/hostphot/filters/DES/DES_i.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/DES/DES_r.dat` & `hostphot-2.8.0/src/hostphot/filters/DES/DES_r.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/DES/DES_z.dat` & `hostphot-2.8.0/src/hostphot/filters/DES/DES_z.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/GALEX/GALEX_FUV.dat` & `hostphot-2.8.0/src/hostphot/filters/GALEX/GALEX_FUV.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/GALEX/GALEX_NUV.dat` & `hostphot-2.8.0/src/hostphot/filters/GALEX/GALEX_NUV.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F435W.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F435W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F475W.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F475W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F502N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F502N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F550M.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F550M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F555W.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F555W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F606W.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F606W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F625W.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F625W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F658N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F658N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F660N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F660N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F775W.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F775W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F814W.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F814W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F850LP.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F850LP.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F892N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F892N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR1016N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR1016N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR388N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR388N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR423N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR423N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR459M.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR459M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR462N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR462N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR505N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR505N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR551N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR551N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR601N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR601N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR647M.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR647M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR656N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR656N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR716N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR716N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR782N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR782N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR853N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR853N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR914M.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR914M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR931N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR931N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/IR_err.txt` & `hostphot-2.8.0/src/hostphot/filters/HST/IR_err.txt`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F090M.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F090M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F095N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F095N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F097N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F097N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F108N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F108N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F110M.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F110M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F110W.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F110W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F113N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F113N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F140W.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F140W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F145M.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F145M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F160W.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F160W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F164N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F164N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F165M.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F165M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F166N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F166N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F170M.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F170M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F187N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F187N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F190N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F190N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F110W.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F110W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F160W.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F160W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F165M.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F165M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F171M.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F171M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F180M.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F180M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F187N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F187N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F187W.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F187W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F190N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F190N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F204M.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F204M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F205W.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F205W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F207M.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F207M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F212N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F212N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F215N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F215N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F216N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F216N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F222M.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F222M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F237M.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F237M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F108N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F108N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F110W.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F110W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F113N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F113N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F150W.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F150W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F160W.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F160W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F164N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F164N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F166N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F166N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F175W.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F175W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F187N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F187N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F190N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F190N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F196N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F196N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F200N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F200N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F212N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F212N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F215N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F215N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F222M.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F222M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F240M.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F240M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/UVIS1_err.txt` & `hostphot-2.8.0/src/hostphot/filters/HST/UVIS1_err.txt`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/UVIS2_err.txt` & `hostphot-2.8.0/src/hostphot/filters/HST/UVIS2_err.txt`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F098M.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F098M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F105W.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F105W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F110W.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F110W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F125W.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F125W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F126N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F126N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F127M.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F127M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F128N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F128N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F130N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F130N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F132N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F132N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F139M.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F139M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F140W.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F140W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F153M.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F153M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F160W.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F160W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F164N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F164N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F167N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F167N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F200LP.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F200LP.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F218W.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F218W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F225W.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F225W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F275W.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F275W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F280N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F280N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F300X.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F300X.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F336W.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F336W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F343N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F343N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F350LP.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F350LP.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F373N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F373N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F390M.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F390M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F390W.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F390W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F395N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F395N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F410M.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F410M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F438W.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F438W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F467M.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F467M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F469N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F469N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F475W.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F475W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F475X.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F475X.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F487N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F487N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F502N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F502N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F547M.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F547M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F555W.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F555W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F600LP.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F600LP.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F606W.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F606W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F621M.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F621M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F625W.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F625W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F631N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F631N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F645N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F645N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F656N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F656N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F657N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F657N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F658N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F658N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F665N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F665N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F673N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F673N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F680N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F680N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F689M.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F689M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F763M.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F763M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F775W.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F775W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F814W.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F814W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F845M.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F845M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F850LP.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F850LP.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F953N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F953N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ232N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ232N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ243N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ243N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ378N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ378N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ387N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ387N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ422M.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ422M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ436N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ436N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ437N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ437N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ492N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ492N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ508N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ508N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ575N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ575N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ619N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ619N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ634N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ634N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ672N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ672N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ674N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ674N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ727N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ727N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ750N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ750N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ889N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ889N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ906N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ906N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ924N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ924N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ937N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ937N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F200LP.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F200LP.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F218W.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F218W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F225W.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F225W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F275W.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F275W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F280N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F280N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F300X.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F300X.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F336W.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F336W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F343N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F343N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F350LP.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F350LP.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F373N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F373N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F390M.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F390M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F390W.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F390W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F395N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F395N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F410M.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F410M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F438W.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F438W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F467M.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F467M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F469N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F469N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F475W.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F475W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F475X.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F475X.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F487N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F487N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F502N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F502N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F547M.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F547M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F555W.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F555W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F600LP.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F600LP.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F606W.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F606W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F621M.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F621M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F625W.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F625W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F631N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F631N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F645N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F645N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F656N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F656N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F657N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F657N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F658N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F658N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F665N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F665N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F673N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F673N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F680N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F680N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F689M.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F689M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F763M.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F763M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F775W.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F775W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F814W.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F814W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F845M.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F845M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F850LP.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F850LP.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F953N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F953N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ232N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ232N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ243N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ243N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ378N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ378N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ387N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ387N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ422M.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ422M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ436N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ436N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ437N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ437N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ492N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ492N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ508N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ508N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ575N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ575N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ619N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ619N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ634N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ634N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ672N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ672N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ674N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ674N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ727N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ727N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ750N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ750N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ889N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ889N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ906N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ906N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ924N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ924N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ937N.dat` & `hostphot-2.8.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ937N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/ir_aper_corrections.csv` & `hostphot-2.8.0/src/hostphot/filters/HST/ir_aper_corrections.csv`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/wfc3uvis1_aper_007_syn.csv` & `hostphot-2.8.0/src/hostphot/filters/HST/wfc3uvis1_aper_007_syn.csv`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/HST/wfc3uvis2_aper_007_syn.csv` & `hostphot-2.8.0/src/hostphot/filters/HST/wfc3uvis2_aper_007_syn.csv`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/LegacySurvey/BASS_g.dat` & `hostphot-2.8.0/src/hostphot/filters/LegacySurvey/BASS_g.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/LegacySurvey/BASS_r.dat` & `hostphot-2.8.0/src/hostphot/filters/LegacySurvey/BASS_r.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/LegacySurvey/DECAM_g.dat` & `hostphot-2.8.0/src/hostphot/filters/LegacySurvey/DECAM_g.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/LegacySurvey/DECAM_r.dat` & `hostphot-2.8.0/src/hostphot/filters/LegacySurvey/DECAM_r.dat`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-# DECam system throughput, from DECaLS wiki, 
-# source: DECamFilters-14apr18.xslx
-# airmass:       1.40000
-# r band
-
       3000.00      0.00000
       3010.00      0.00000
       3020.00      0.00000
       3030.00      0.00000
       3040.00      0.00000
       3050.00      0.00000
       3060.00      0.00000
```

### Comparing `hostphot-2.7.1/src/hostphot/filters/LegacySurvey/DECAM_z.dat` & `hostphot-2.8.0/src/hostphot/filters/LegacySurvey/DECAM_z.dat`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-# DECam system throughput, from DECaLS wiki, 
-# source: DECamFilters-14apr18.xslx
-# airmass:       1.40000
-# z band
-
       3000.00      0.00000
       3010.00      0.00000
       3020.00      0.00000
       3030.00      0.00000
       3040.00      0.00000
       3050.00      0.00000
       3060.00      0.00000
```

### Comparing `hostphot-2.7.1/src/hostphot/filters/LegacySurvey/MzLS_z.dat` & `hostphot-2.8.0/src/hostphot/filters/LegacySurvey/MzLS_z.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/PS1/PS1_g.dat` & `hostphot-2.8.0/src/hostphot/filters/PS1/PS1_g.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/PS1/PS1_i.dat` & `hostphot-2.8.0/src/hostphot/filters/PS1/PS1_i.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/PS1/PS1_r.dat` & `hostphot-2.8.0/src/hostphot/filters/PS1/PS1_r.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/PS1/PS1_y.dat` & `hostphot-2.8.0/src/hostphot/filters/PS1/PS1_y.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/PS1/PS1_z.dat` & `hostphot-2.8.0/src/hostphot/filters/PS1/PS1_z.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/SDSS/SDSS_g.dat` & `hostphot-2.8.0/src/hostphot/filters/SDSS/SDSS_g.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/SDSS/SDSS_i.dat` & `hostphot-2.8.0/src/hostphot/filters/SDSS/SDSS_i.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/SDSS/SDSS_r.dat` & `hostphot-2.8.0/src/hostphot/filters/SDSS/SDSS_r.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/SDSS/SDSS_u.dat` & `hostphot-2.8.0/src/hostphot/filters/SDSS/SDSS_u.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/SDSS/SDSS_z.dat` & `hostphot-2.8.0/src/hostphot/filters/SDSS/SDSS_z.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/Spitzer/Spitzer_IRAC.1.dat` & `hostphot-2.8.0/src/hostphot/filters/Spitzer/Spitzer_IRAC.1.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/Spitzer/Spitzer_IRAC.2.dat` & `hostphot-2.8.0/src/hostphot/filters/Spitzer/Spitzer_IRAC.2.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/Spitzer/Spitzer_IRAC.3.dat` & `hostphot-2.8.0/src/hostphot/filters/Spitzer/Spitzer_IRAC.3.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/Spitzer/Spitzer_IRAC.4.dat` & `hostphot-2.8.0/src/hostphot/filters/Spitzer/Spitzer_IRAC.4.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/Spitzer/Spitzer_MIPS.1.dat` & `hostphot-2.8.0/src/hostphot/filters/Spitzer/Spitzer_MIPS.1.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/WISE/WISE_W1.dat` & `hostphot-2.8.0/src/hostphot/filters/WISE/WISE_W1.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/WISE/WISE_W2.dat` & `hostphot-2.8.0/src/hostphot/filters/WISE/WISE_W2.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/WISE/WISE_W3.dat` & `hostphot-2.8.0/src/hostphot/filters/WISE/WISE_W3.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/WISE/WISE_W4.dat` & `hostphot-2.8.0/src/hostphot/filters/WISE/WISE_W4.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/filters/config.txt` & `hostphot-2.8.0/src/hostphot/filters/config.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,15 @@
-survey		filters					zp		pixel_scale		mag_sys		mag_sys_conv
-DES		grizY					30		0.263			AB		0.0
-PS1		grizy					25		0.25			AB		0.0
-SDSS		ugriz					22.5		0.396			AB		0.0
-GALEX		FUV,NUV					18.82,20.08	1.5			AB		0.0
-2MASS		J,H,Ks	        			header		1.0		    	Vega		0.91,1.39,1.85
-WISE		W1,W2,W3,W4				header		1.375			Vega		2.699,3.339,5.174,6.620
-unWISE		W1,W2,W3,W4				22.5		2.75			Vega		2.699,3.339,5.174,6.620
-HST		UVIS,WFC,IR,NIC				header		0.06			AB		0.0
-LegacySurvey    grz             			22.5    	0.262       		AB          	0.0
-Spitzer         IRAC.1,IRAC.2,IRAC.3,IRAC.4,MIPS.1      header    	0.6,0.6,0.6,0.6,2.45    AB          	0.0
-VISTA           Z,Y,J,H,Ks      			header  	0.339       		VEGA        	0.502,0.600,0.916,1.366,1.827
+survey		filters						zp		pixel_scale		mag_sys		mag_sys_conv
+DES		grizY						30		0.263			AB		0.0
+PS1		grizy						25		0.25			AB		0.0
+SDSS		ugriz						22.5		0.396			AB		0.0
+GALEX		FUV,NUV						18.82,20.08	1.5			AB		0.0
+2MASS		J,H,Ks	        				header		1.0		    	Vega		0.91,1.39,1.85
+WISE		W1,W2,W3,W4					header		1.375			Vega		2.699,3.339,5.174,6.620
+unWISE		W1,W2,W3,W4					22.5		2.75			Vega		2.699,3.339,5.174,6.620
+LegacySurvey    grz             				22.5    	0.262       		AB          	0.0
+Spitzer         IRAC.1,IRAC.2,IRAC.3,IRAC.4,MIPS.1      	header    	0.6,0.6,0.6,0.6,2.45    AB          	0.0
+VISTA           Z,Y,J,H,Ks      				header  	0.339       		Vega        	0.502,0.600,0.916,1.366,1.827
+HST		WFC3/UVIS,WFC3/IR				header		0.04,0.13		AB		0.0
+SkyMapper       uvgriz		      				header  	0.5       		AB        	0.0
+SPLUS           u,F378,F395,F410,F430,g,F515,r,F660,i,F861,z    header  	0.55       		AB        	0.0
+UKIDSS          ZYJHK      					header  	0.4       		Vega        	0.528,0.634,0.938,1.379,1.900
```

### Comparing `hostphot-2.7.1/src/hostphot/global_photometry.py` & `hostphot-2.8.0/src/hostphot/global_photometry.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     check_survey_validity,
     check_filters_validity,
     get_image_gain,
     check_work_dir,
     magnitude_calculation,
     adapt_aperture,
     bkg_surveys,
+    load_pickle
 )
 from hostphot.objects_detect import extract_objects, plot_detected_objects
 from hostphot.image_cleaning import remove_nan
 from hostphot.dust import calc_extinction
 
 import warnings
 from astropy.utils.exceptions import AstropyWarning
@@ -89,16 +90,18 @@
         gain=gain,
     )
 
     return flux, flux_err
 
 
 def optimize_kron_flux(data, err, gain, objects, eps=0.0001):
-    """Optimizes the Kron flux by iteration over different values.
-    The stop condition is met when the change in flux is less that ``eps``.
+    """Optimizes the Kron flux by iteration over different scales.
+
+    The stop condition is met when the change in flux between iterations 
+    is less that ``eps``.
 
     Parameters
     ----------
     data: ndarray
         Data of an image.
     err: float or ndarray
         Background error of the images.
@@ -111,60 +114,51 @@
 
     Returns
     -------
     opt_flux: float
         Optimized Kron flux.
     opt_flux_err: float
         Optimized Kron flux error.
-    opt_kronrad: float
-        Optimized Kron radius.
+    kronrad: float
+        Kron radius.
     opt_scale: float
-        Optimized scale of the Kron radius.
+        Optimized scale for the Kron radius.
     """
-    # iterate over kron radii
-    for r in np.arange(1, 6.05, 0.05)[::-1]:
-        kronrad, _ = sep.kron_radius(
+    kronrad, _ = sep.kron_radius(
             data,
             objects["x"],
             objects["y"],
             objects["a"],
             objects["b"],
             objects["theta"],
-            r,
-        )
-        opt_kronrad = kronrad
-        if ~np.isnan(opt_kronrad):
-            break
-
-    if np.isnan(opt_kronrad):
-        raise ValueError(
-            "The Kron radius cannot be calculated. The image might have NaNs or the aperture is too close to the edge."
+            r=6.0,  # following sep docs
         )
-
+    kronrad = kronrad[0]
+    
     opt_flux = 0.0
     # iterate over scale
     scales = np.arange(1, 10, 0.01)
     for scale in scales:
         flux, flux_err = kron_flux(
-            data, err, gain, objects, opt_kronrad, scale
+            data, err, gain, objects, kronrad, scale
         )
         flux, flux_err = flux[0], flux_err[0]
 
         calc_eps = np.abs(opt_flux - flux) / flux
         opt_flux, opt_flux_err = flux, flux_err
         opt_scale = scale
         if calc_eps < eps:
             opt_scale = scale
             break
         elif np.isnan(calc_eps):
             opt_scale = scales[-2]
             warnings.warn("Warning: the aperture might not fit in the image!")
             break
 
-    return opt_flux, opt_flux_err, opt_kronrad[0], opt_scale
+    return opt_flux, opt_flux_err, kronrad, opt_scale
 
 
 def extract_kronparams(
     name,
     host_ra,
     host_dec,
     filt,
@@ -204,16 +198,16 @@
         VISTA).
     threshold: float, default `10`
         Threshold used by `sep.extract()` to extract objects.
     use_mask: bool, default `True`
         If `True`, the masked fits files are used. These must have
         been created beforehand.
     optimize_kronrad: bool, default `True`
-        If `True`, the Kron radius is optimized, increasing the
-        aperture size until the flux does not increase.
+        If `True`, the Kron-radius scale is optimized, increasing the
+        aperture size until the change in flux is less than ``eps``.
     eps: float, default ``0.0001``
         The Kron radius is increased until the change in flux is lower than ``eps``.
         A value of 0.0001 means 0.01% change in flux.
     gal_dist_thresh: float, default ``-1``.
         Distance in arcsec to crossmatch the galaxy coordinates with a detected object,
         where the object nearest to the galaxy position is considered as the galaxy (within
         the given threshold). If no objects are found within the given distance threshold,
@@ -233,15 +227,15 @@
         Image's WCS.
     kronrad: float
         Kron radius.
     scale: float
         Scale for the Kron radius.
     flip: bool
         Whether to flip the orientation of the
-        aperture. Only used for DES images.
+        aperture.
     """
     check_survey_validity(survey)
     check_work_dir(workdir)
     obj_dir = os.path.join(workdir, name)
     if use_mask:
         suffix = "masked_"
     else:
@@ -304,29 +298,54 @@
             dec,
             host_ra,
             host_dec,
             title,
             outfile,
         )
 
-    if survey == "DES":
+    if survey in ["DES", "VISTA", "UKIDSS"]:
         flip = True
     else:
         flip = False
 
     if save_aperture_params is True:
         outfile = os.path.join(
             obj_dir, f"{survey}_{filt}_aperture_parameters.pickle"
         )
         with open(outfile, "wb") as fp:
             aperture_parameters = gal_obj, img_wcs, kronrad, scale, flip
             pickle.dump(aperture_parameters, fp, protocol=4)
 
     return gal_obj, img_wcs, kronrad, scale, flip
 
+def load_aperture_params(name, filt, survey):
+    """Loads previously saved aperture parameters.
+    
+    Parameters
+    ----------
+    name: str
+        Name of the object to find the path of the aperture-parameters file.
+    filt: str
+        Name of the filter used for the aperture parameters. Coadds are
+        also valid.
+    survey: str
+        Survey name to be used.
+        
+    Returns
+    -------
+    aperture_params: tuple
+        Aperture paremeters with the same format as the output of the
+        ``extract_kronparams`` function.
+    """
+    inputfile = os.path.join(workdir, name, 
+                             f'{survey}_{filt}_aperture_parameters.pickle')
+    
+    aperture_params = load_pickle(inputfile)
+    
+    return aperture_params
 
 def photometry(
     name,
     host_ra,
     host_dec,
     filt,
     survey,
@@ -376,16 +395,16 @@
         If `True`, corrects for Milky-Way extinction using the recalibrated dust maps
         by Schlafly & Finkbeiner (2011) and the extinction law from Fitzpatrick (1999).
     aperture_params: tuple, default `None`
         Tuple with objects info and Kron parameters. Used for
         common aperture. If given, the Kron parameters are not
         re-calculated
     optimize_kronrad: bool, default `True`
-        If `True`, the Kron radius is optimized, increasing the
-        aperture size until the flux does not increase.
+        If `True`, the Kron-radius scale is optimized, increasing the
+        aperture size until the change in flux is less than ``eps``.
     eps: float, default ``0.0001``
         The Kron radius is increased until the change in flux is lower than ``eps``.
         A value of 0.0001 means 0.01% change in flux.
     gal_dist_thresh: float, default ``-1``.
         Distance in arcsec to crossmatch the galaxy coordinates with a detected object,
         where the object nearest to the galaxy position is considered as the galaxy (within
         the given threshold). If no objects are found within the given distance threshold,
@@ -401,15 +420,21 @@
         Aperture magnitude.
     mag_err: float
         Error on the aperture magnitude.
     flux: float
         Aperture flux.
     total_flux_err: float
         Total flux error on the aperture flux.
+    zp: float
+        Zeropoint.
     """
+    if survey == 'SkyMapper':
+        warnings.warn(("SkyMapper photometry is not completely trustworthy due to imprecision in "
+                       "the zeropoint for extended sources, which might be solved in a future data release."))
+
     check_survey_validity(survey)
     check_work_dir(workdir)
     obj_dir = os.path.join(workdir, name)
     if use_mask:
         suffix = "masked_"
     else:
         suffix = ""
@@ -433,15 +458,15 @@
         data_sub = np.copy(data - bkg)
     else:
         data_sub = np.copy(data)
 
     if aperture_params is not None:
         gal_obj, master_img_wcs, kronrad, scale, flip2 = aperture_params
 
-        if survey == "DES":
+        if survey in ["DES", "VISTA", "UKIDSS"]:
             flip = True
         else:
             flip = False
         if flip == flip2:
             flip_ = False
         else:
             flip_ = True
@@ -485,27 +510,40 @@
             flux, flux_err = kron_flux(
                 data_sub, bkg_rms, gain, gal_obj, kronrad, scale
             )
             flux, flux_err = flux[0], flux_err[0]
 
     ap_area = np.pi * gal_obj["a"][0] * gal_obj["b"][0]
 
-    mag, mag_err, flux, flux_err = magnitude_calculation(
+    mag, mag_err, flux, flux_err, zp = magnitude_calculation(
         flux,
         flux_err,
         survey,
         filt,
         ap_area,
         header,
         bkg_rms,
     )
 
+    if survey in ["LegacySurvey"]:
+        invvar_map = hdu[1].data
+        var_map = 1/invvar_map
+        sum_var, _ = kron_flux(
+                var_map, bkg_rms, gain, gal_obj, kronrad, scale
+            )
+        extra_flux_err = np.sqrt(sum_var[0]) 
+        flux_err = np.sqrt(flux_err**2 + extra_flux_err**2)
+
+        extra_err = np.abs(2.5 * flux_err / (flux * np.log(10)))
+        mag_err = np.sqrt(mag_err**2 + extra_err**2)
+
     if correct_extinction is True:
         A_ext = calc_extinction(filt, survey, host_ra, host_dec)
         mag -= A_ext
+        flux *= 10**(0.4*A_ext)
 
     if save_plots is True:
         outfile = os.path.join(obj_dir, f"global_{survey}_{filt}.jpg")
         title = f"{name}: {survey}-${filt}$"
         plot_detected_objects(
             hdu,
             gal_obj,
@@ -514,15 +552,15 @@
             dec,
             host_ra,
             host_dec,
             title,
             outfile,
         )
 
-    return mag, mag_err, flux, flux_err
+    return mag, mag_err, flux, flux_err, zp
 
 
 def multi_band_phot(
     name,
     host_ra,
     host_dec,
     filters=None,
@@ -580,16 +618,16 @@
         coadds for common aperture (``common_aperture`` parameter).
     common_aperture: bool, default ``True``
         If ``True``, use a coadd image for common aperture photometry. This is not used
         if ``aperture_params`` is given.
     coadd_filters: str, default ``riz``
         Filters of the coadd image. Used for common aperture photometry.
     optimize_kronrad: bool, default ``True``
-        If ``True``, the Kron radius is optimized, increasing the
-        aperture size until the flux does not increase.
+        If `True`, the Kron-radius scale is optimized, increasing the
+        aperture size until the change in flux is less than ``eps``.
     eps: float, default ``0.0001``
         The Kron radius is increased until the change in flux is lower than ``eps``.
         A value of 0.0001 means 0.01% change in flux.
         when optimizing the Kron radius.
     gal_dist_thresh: float, default ``-1``.
         Distance in arcsec to crossmatch the galaxy coordinates with a detected object,
         where the object nearest to the galaxy position is considered as the galaxy (within
@@ -653,15 +691,15 @@
             eps=eps,
             gal_dist_thresh=gal_dist_thresh,
             save_plots=save_plots,
         )
 
     for filt in filters:
         try:
-            mag, mag_err, flux, flux_err = photometry(
+            mag, mag_err, flux, flux_err, zp = photometry(
                 name,
                 host_ra,
                 host_dec,
                 filt,
                 survey,
                 ra=ra,
                 dec=dec,
@@ -675,20 +713,24 @@
                 gal_dist_thresh=gal_dist_thresh,
                 save_plots=save_plots,
             )
             results_dict[filt] = mag
             results_dict[f"{filt}_err"] = mag_err
             results_dict[f"{filt}_flux"] = flux
             results_dict[f"{filt}_flux_err"] = flux_err
+            results_dict[f"{filt}_zeropoint"] = zp
         except Exception as exc:
             if raise_exception is True:
                 raise Exception(f"{filt}-band: {exc}")
             else:
                 results_dict[filt] = np.nan
                 results_dict[f"{filt}_err"] = np.nan
+                results_dict[f"{filt}_flux"] = np.nan
+                results_dict[f"{filt}_flux_err"] = np.nan
+                results_dict[f"{filt}_zeropoint"] = np.nan
 
     if save_results is True:
         outfile = os.path.join(workdir, name, f"{survey}_global.csv")
         phot_df = pd.DataFrame(
             {key: [val] for key, val in results_dict.items()}
         )
         phot_df.to_csv(outfile, index=False)
```

### Comparing `hostphot-2.7.1/src/hostphot/image_cleaning.py` & `hostphot-2.8.0/src/hostphot/image_cleaning.py`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/image_masking.py` & `hostphot-2.8.0/src/hostphot/image_masking.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     cross_match,
 )
 from hostphot.utils import (
     check_survey_validity,
     bkg_surveys,
     adapt_aperture,
     suppress_stdout,
+    load_pickle
 )
 
 import warnings
 from astropy.utils.exceptions import AstropyWarning
 
 
 # ----------------------------------------
@@ -158,15 +159,15 @@
         Galaxy object.
     nogal_obj: array
         Non-galaxy objects.
     img_wcs: WCS
         Image's WCS.
     flip: bool
         Whether to flip the orientation of the
-        aperture. Only used for DES images.
+        aperture. 
     """
     check_survey_validity(survey)
     if isinstance(filt, list):
         filt = "".join(f for f in filt)
 
     obj_dir = os.path.join(workdir, name)
     fits_file = os.path.join(obj_dir, f"{survey}_{filt}.fits")
@@ -207,15 +208,15 @@
             cat_coord = concatenate([cat_coord1, cat_coord2])
             nogal_objs = cross_match(nogal_objs, img_wcs, cat_coord)
     else:
         # use objects previously extracted
         # the aperture/ellipse parameters are updated accordingly
         gal_obj, nogal_objs, master_img_wcs, flip2 = common_params
 
-        if survey == "DES":
+        if survey in ["DES", "VISTA", "UKIDSS"]:
             flip = True
         else:
             flip = False
         if flip == flip2:
             flip_ = False
         else:
             flip_ = True
@@ -225,14 +226,27 @@
 
     masked_data = mask_image(data_sub, nogal_objs, r=r, sigma=sigma)
     masked_hdu = deepcopy(hdu)
     masked_hdu[0].data = masked_data
     outfile = os.path.join(obj_dir, f"masked_{survey}_{filt}.fits")
     masked_hdu.writeto(outfile, overwrite=True)
 
+    if survey in ["DES", "VISTA", "UKIDSS"]:
+        flip = True
+    else:
+        flip = False
+
+    if save_mask_params is True:
+        outfile = os.path.join(
+            obj_dir, f"{survey}_{filt}_mask_parameters.pickle"
+        )
+        with open(outfile, "wb") as fp:
+            mask_parameters = gal_obj, nogal_objs, img_wcs, flip
+            pickle.dump(mask_parameters, fp, protocol=4)
+
     if save_plots:
         outfile = os.path.join(obj_dir, f"masked_{survey}_{filt}.jpg")
         title = f"{name}: {survey}-${filt}$"
         plot_masked_image(
             hdu,
             masked_hdu,
             nogal_objs,
@@ -242,30 +256,42 @@
             host_dec,
             ra,
             dec,
             title,
             outfile,
         )
 
-    if survey == "DES":
-        flip = True
-    else:
-        flip = False
-
-    if save_mask_params is True:
-        outfile = os.path.join(
-            obj_dir, f"{survey}_{filt}_mask_parameters.pickle"
-        )
-        with open(outfile, "wb") as fp:
-            mask_parameters = gal_obj, nogal_objs, img_wcs, flip
-            pickle.dump(mask_parameters, fp, protocol=4)
-
     if extract_params:
         return gal_obj, nogal_objs, img_wcs, flip
 
+def load_mask_params(name, filt, survey):
+    """Loads previously saved mask parameters.
+    
+    Parameters
+    ----------
+    name: str
+        Name of the object to find the path of the mask-parameters file.
+    filt: str
+        Name of the filter used to create the mask parameters. Coadds are
+        also valid.
+    survey: str
+        Survey name to be used.
+        
+    Returns
+    -------
+    mask_params: tuple
+        Mask paremeters with the same format as the output of the
+        ``create_mask`` function.
+    """
+    inputfile = os.path.join(workdir, name, 
+                             f'{survey}_{filt}_mask_parameters.pickle')
+    
+    mask_params = load_pickle(inputfile)
+    
+    return mask_params
 
 def plot_masked_image(
     hdu,
     masked_hdu,
     objects,
     gal_obj=None,
     r=6,
@@ -335,15 +361,15 @@
         fig.axis_labels.set_font(**{"family": font_family, "size": 18})
 
     # galaxy markers
     fig2.show_markers(
         host_ra,
         host_dec,
         edgecolor="k",
-        facecolor="r",
+        facecolor="m",
         alpha=0.7,
         marker="P",
         s=200,
         label="Given galaxy",
     )
     fig2.show_markers(
         gal_obj["x"][0],
```

### Comparing `hostphot-2.7.1/src/hostphot/interactive_aperture.py` & `hostphot-2.8.0/src/hostphot/interactive_aperture.py`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/local_photometry.py` & `hostphot-2.8.0/src/hostphot/local_photometry.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,25 +16,24 @@
 
 import os
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 import aplpy
 
-font = "GFS Artemisia"
-plt.rcParams["mathtext.fontset"] = "cm"
+plt.rcParams['mathtext.fontset'] = "cm"
 
 import sep
 from photutils.aperture import aperture_photometry, CircularAperture
 
 from astropy.io import fits
 from astropy import units as u, wcs
 from astropy.cosmology import FlatLambdaCDM
 
-from hostphot._constants import workdir
+from hostphot._constants import workdir, font_family
 from hostphot.utils import (
     get_survey_filters,
     check_survey_validity,
     check_filters_validity,
     calc_sky_unc,
     get_image_exptime,
     survey_pixel_scale,
@@ -144,60 +143,47 @@
     title: str
         Title of the figure.
     outfile: str, default ``None``
         If given, path where to save the output figure.
     """
 
     figure = plt.figure(figsize=(10, 10))
-    title, label = title.split("|")
+    title, label = title.split('|')
 
     with warnings.catch_warnings():
         warnings.simplefilter("ignore", AstropyWarning)
         fig = aplpy.FITSFigure(hdu, figure=figure)
 
     with suppress_stdout():
-        fig.show_grayscale(stretch="arcsinh")
+        fig.show_grayscale(stretch='arcsinh')
 
     # plot SN and aperture
-    fig.show_markers(
-        px,
-        py,
-        edgecolor="k",
-        facecolor="aqua",
-        marker="*",
-        s=200,
-        label="SN",
-        coords_frame="pixel",
-    )
-    fig.show_circles(
-        px, py, radius_pix, coords_frame="pixel", linewidth=2, edgecolor="r"
-    )
-    fig.show_lines([], [], color="r", lw=3, label=label)  # for the legend only
-
-    # ticks
-    fig.tick_labels.set_font(**{"family": font, "size": 18})
-    fig.tick_labels.set_xformat("dd.dd")
-    fig.tick_labels.set_yformat("dd.dd")
+    fig.show_markers(px, py, edgecolor='k', facecolor='aqua', 
+                     marker='*', s=200, label='SN', coords_frame='pixel')
+    fig.show_circles(px, py, radius_pix, coords_frame='pixel', linewidth=3, edgecolor='r')
+    fig.show_lines([], [], color='r', lw=3, label=label)  # for the legend only
+
+    #ticks
+    fig.tick_labels.set_font(**{'family':font_family, 'size':18})
+    fig.tick_labels.set_xformat('dd.dd')
+    fig.tick_labels.set_yformat('dd.dd')
     fig.ticks.set_length(6)
 
-    fig.axis_labels.set_font(**{"family": font, "size": 18})
+    fig.axis_labels.set_font(**{'family':font_family, 'size':18})
 
-    fig.set_title(title, **{"family": font, "size": 24})
-    fig.set_theme("publication")
-    fig.ax.legend(
-        fancybox=True, framealpha=1, prop={"size": 20, "family": font}
-    )
+    fig.set_title(title, **{'family':font_family, 'size':24})
+    fig.set_theme('publication')
+    fig.ax.legend(fancybox=True, framealpha=1, prop={'size':20, 'family':font_family})
 
     if outfile:
         plt.savefig(outfile, bbox_inches="tight")
         plt.close(figure)
     else:
         plt.show()
 
-
 def photometry(
     name,
     ra,
     dec,
     z,
     filt,
     survey,
@@ -245,15 +231,21 @@
         Aperture magnitudes for the given aperture radii.
     mags_err: list
         Aperture magnitude errors for the given aperture radii.
     fluxes: list
         Aperture flux for the given aperture radii.
     fluxes_err: list
         Aperture flux errors for the given aperture radii.
+    zp: float
+        Zeropoint.
     """
+    if survey == 'SkyMapper':
+        warnings.warn(("SkyMapper photometry is not completely trustworthy due to imprecision in "
+                       "the zeropoint for extended sources, which might be solved in a future data release."))
+        
     check_survey_validity(survey)
     check_work_dir(workdir)
     obj_dir = os.path.join(workdir, name)
     if use_mask:
         suffix = "masked_"
     else:
         suffix = ""
@@ -282,54 +274,73 @@
     if isinstance(ap_radii, (float, int)):
         ap_radii = [ap_radii]
 
     mags, mags_err = [], []
     fluxes, fluxes_err = [], []
     px, py = img_wcs.wcs_world2pix(ra, dec, 1)
     pixel_scale = survey_pixel_scale(survey, filt)
+    if survey == 'UKIDSS' and filt == 'J':
+        if 'LAS' in header['PROJECT'].split('/')[-1]:
+            # if the J comes from the LAS then the observations were micro-stepped
+            # in the J-band so the pixel size is smaller.
+            nustep = header['NUSTEP']
+            pixel_scale /= nustep/2  # divided by 2 for the two dimensions (x and y)
     error = calc_sky_unc(data_sub, exptime)
 
     for ap_radius in ap_radii:
         # aperture photometry
         radius_arcsec = calc_aperture_size(z, ap_radius)
         radius_pix = radius_arcsec / pixel_scale
 
         flux, flux_err = extract_aperture_flux(
             data_sub, error, px, py, radius_pix
         )
 
-        ap_area = 2 * np.pi * (radius_pix**2)
-        mag, mag_err, flux, flux_err = magnitude_calculation(
+        ap_area = np.pi * (radius_pix**2)
+        mag, mag_err, flux, flux_err, zp = magnitude_calculation(
             flux,
             flux_err,
             survey,
             filt,
             ap_area,
             header,
             bkg_rms,
         )
 
+        if survey in ["LegacySurvey"]:
+            invvar_map = hdu[1].data
+            var_map = 1/invvar_map
+            sum_var, _ = extract_aperture_flux(
+                        var_map, error, px, py, radius_pix
+                    )
+            extra_flux_err = np.sqrt(sum_var) 
+            flux_err = np.sqrt(flux_err**2 + extra_flux_err**2)
+
+            extra_err = np.abs(2.5 * flux_err / (flux * np.log(10)))
+            mag_err = np.sqrt(mag_err**2 + extra_err**2)
+
         # extinction correction is optional
         if correct_extinction:
             A_ext = calc_extinction(filt, survey, ra, dec)
             mag -= A_ext
+            flux *= 10**(0.4*A_ext)
 
         mags.append(mag)
         mags_err.append(mag_err)
         fluxes.append(flux)
         fluxes_err.append(flux_err)
 
         if save_plots:
             outfile = os.path.join(
                 obj_dir, f"local_{survey}_{filt}_{ap_radius}kpc.jpg"
             )
-            title = f"{name}: {survey}-${filt}$|r$={ap_radius}$ kpc @ $z={z}$"
+            title = f'{name}: {survey}-${filt}$|r$={ap_radius}$ kpc @ $z={z}$'
             plot_aperture(hdu, px, py, radius_pix, title, outfile)
 
-    return mags, mags_err, fluxes, fluxes_err
+    return mags, mags_err, fluxes, fluxes_err, zp
 
 
 def multi_band_phot(
     name,
     ra,
     dec,
     z,
@@ -394,37 +405,37 @@
     >>> survey = 'PS1'
     >>> results = lp.multi_band_phot(name, ra, dec, z,
                             survey=survey, ap_radii=ap_radii,
                             use_mask=True, save_plots=True)
     """
     check_survey_validity(survey)
     if filters is None:
-        if survey == "HST":
+        if survey=='HST':
             raise ValueError("For HST, the filter needs to be specified!")
         filters = get_survey_filters(survey)
     else:
         check_filters_validity(filters, survey)
-    if survey == "HST":
+    if survey=='HST':
         filters = [filters]
 
     # turn float into a list
     if isinstance(ap_radii, (float, int)):
         ap_radii = [ap_radii]
 
     results_dict = {
         "name": name,
         "ra": ra,
         "dec": dec,
         "redshift": z,
         "survey": survey,
     }
-
+    
     for filt in filters:
         try:
-            mags, mags_err, fluxes, fluxes_err = photometry(
+            mags, mags_err, fluxes, fluxes_err, zp = photometry(
                 name,
                 ra,
                 dec,
                 z,
                 filt,
                 survey,
                 ap_radii,
@@ -436,23 +447,25 @@
             for radius, mag, mag_err, flux, flux_err in zip(
                 ap_radii, mags, mags_err, fluxes, fluxes_err
             ):
                 results_dict[f"{filt}_{radius}"] = mag
                 results_dict[f"{filt}_{radius}_err"] = mag_err
                 results_dict[f"{filt}_{radius}_flux"] = flux
                 results_dict[f"{filt}_{radius}_flux_err"] = flux_err
+            results_dict[f"{filt}_zeropoint"] = zp
         except Exception as exc:
             if raise_exception is True:
                 raise Exception(exc)
             else:
                 for radius in ap_radii:
                     results_dict[f"{filt}_{radius}"] = np.nan
                     results_dict[f"{filt}_{radius}_err"] = np.nan
                     results_dict[f"{filt}_{radius}_flux"] = np.nan
                     results_dict[f"{filt}_{radius}_flux_err"] = np.nan
+                results_dict[f"{filt}_zeropoint"] = np.nan
 
     if save_results is True:
         outfile = os.path.join(workdir, name, f"{survey}_local.csv")
         phot_df = pd.DataFrame(
             {key: [val] for key, val in results_dict.items()}
         )
         phot_df.to_csv(outfile, index=False)
```

### Comparing `hostphot-2.7.1/src/hostphot/objects_detect.py` & `hostphot-2.8.0/src/hostphot/objects_detect.py`

 * *Files 0% similar despite different names*

```diff
@@ -261,15 +261,15 @@
 
     # plot galaxy marker and aperture
     if (host_ra is not None) and (host_dec is not None):
         fig.show_markers(
             host_ra,
             host_dec,
             edgecolor="k",
-            facecolor="r",
+            facecolor="m",
             alpha=0.7,
             marker="P",
             s=200,
             label="Galaxy position",
         )
     fig.show_ellipses(
         objects["x"][0],
```

### Comparing `hostphot-2.7.1/src/hostphot/rgb_images.py` & `hostphot-2.8.0/src/hostphot/rgb_images.py`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/src/hostphot/utils.py` & `hostphot-2.8.0/src/hostphot/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import os
 import sys
 import glob
+import pickle
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
+import matplotlib.image as img
 
 import aplpy
 from contextlib import contextmanager
 
 plt.rcParams["mathtext.fontset"] = "cm"
 
 from astropy.stats import sigma_clipped_stats
@@ -21,15 +23,15 @@
 from hostphot._constants import font_family
 
 hostphot_path = hostphot.__path__[0]
 config_file = os.path.join(hostphot_path, "filters", "config.txt")
 config_df = pd.read_csv(config_file, delim_whitespace=True)
 
 # surveys that need background subtraction
-bkg_surveys = ["2MASS", "WISE", "VISTA"]
+bkg_surveys = ["2MASS", "WISE", "VISTA", "SkyMapper", "UKIDSS"]
 
 
 def calc_sky_unc(image, exptime):
     """Calculates the uncertainty of the image from the
     sky standard deviation, sigma-clipped STD.
 
     Parameters
@@ -128,20 +130,14 @@
 
     if zps == "header":
         return zps
 
     if "," in zps:
         zps = zps.split(",")
         zp_dict = {filt: float(zp) for filt, zp in zip(filters, zps)}
-    elif survey == "SDSS":
-        # SDSS zero-points are not exactly in AB:
-        # https://www.sdss4.org/dr12/algorithms/fluxcal/#SDSStoAB
-        zp_dict = {filt: float(zps) for filt in filters}
-        zp_dict["u"] -= 0.04
-        zp_dict["z"] += 0.02
     else:
         zp_dict = {filt: float(zps) for filt in filters}
 
     return zp_dict
 
 
 def get_image_gain(header, survey):
@@ -171,29 +167,35 @@
         gain = 1.0
     elif survey == "2MASS":
         # the value comes from https://wise2.ipac.caltech.edu/staff/jarrett/2mass/3chan/noise/
         # Note that it is different from the value of
         # https://iopscience.iop.org/article/10.1086/498708/pdf (8 e ADU^-1)
         gain = 10.0
     elif survey == "LegacySurvey":
-        gain = 30  # assumed similar to DES
+        gain = 1  # not used
     elif survey == "Spitzer":
         # also in the "EXPGAIN" keyword
         if header["INSTRUME"] == "IRAC":
             # Table 2.4 of IRAC Instrument Handbook
             gain = 3.8  # all filters have similar gain
             gain *= header["EFCONV"]  # convert DN/s to MJy/sr
         elif header["INSTRUME"] == "MIPS":
             # Table 2.4 of MIPS Instrument Handbook
             gain = 5.0
     elif survey == "VISTA":
         # use median from http://casu.ast.cam.ac.uk/surveys-projects/vista/technical/vista-gain
         gain = 4.19
     elif survey == "HST":
         gain = header["CCDGAIN"]
+    elif survey=='SkyMapper':
+        gain = header["GAIN"]
+    elif survey=='SPLUS':
+        gain = header["GAIN"]
+    elif survey=='UKIDSS':
+        gain = header["GAIN"]
     else:
         gain = 1.0
 
     return gain
 
 
 def get_image_readnoise(header, survey):
@@ -224,15 +226,15 @@
     elif survey == "SDSS":
         readnoise = 0.0
     elif survey == "2MASS":
         # https://iopscience.iop.org/article/10.1086/498708/pdf
         # 6 combined images
         readnoise = 4.5 * np.sqrt(6)  # not used
     elif survey == "LegacySurvey":
-        readnoise = 7.0  # assumed similar to DES
+        readnoise = 1.0  # not used
     elif survey == "Spitzer":
         if header["INSTRUME"] == "IRAC":
             # Table 2.3 of IRAC Instrument Handbook
             # very rough average
             readnoise_dict = {1: 16.0, 2: 12.0, 3: 10.0, 4: 8.0}
             channel = header["CHNLNUM"]
             readnoise = readnoise_dict[channel]
@@ -242,14 +244,21 @@
     elif survey == "VISTA":
         # very rough average for all filters in
         # http://casu.ast.cam.ac.uk/surveys-projects/vista/technical/vista-gain
         readnoise = 24.0
     elif survey == "HST":
         # tipically 0.0
         readnoise = header["PCTERNOI"]
+    elif survey=='SkyMapper':
+        # https://rsaa.anu.edu.au/observatories/instruments/skymapper-instrument
+        readnoise = 5  # electrons
+    elif survey=='SPLUS':
+        readnoise = header["HIERARCH OAJ QC NCNOISE"]
+    elif survey=='UKIDSS':
+        readnoise = header["READNOIS"]
     else:
         readnoise = 0.0
 
     return readnoise
 
 
 def get_image_exptime(header, survey):
@@ -264,28 +273,32 @@
 
     Returns
     -------
     exptime: float
         Exposure time in seconds.
     """
     check_survey_validity(survey)
-    if survey in ["PS1", "DES", "GALEX", "VISTA", "Spitzer", "HST"]:
+    if survey in ["PS1", "DES", "GALEX", "VISTA", "Spitzer", "HST", "SkyMapper"]:
         exptime = float(header["EXPTIME"])
     elif survey == "WISE":
         # see: https://wise2.ipac.caltech.edu/docs/release/allsky/
         # and https://wise2.ipac.caltech.edu/docs/release/allsky/expsup/sec1_1.html
         if header["BAND"] in [1, 2]:
             exptime = 7.7
         elif header["BAND"] in [3, 4]:
             exptime = 8.8
     elif survey == "2MASS":
         # https://iopscience.iop.org/article/10.1086/498708/pdf
         exptime = 7.8
     elif survey == "LegacySurvey":
-        exptime = 900.0  # assumed similar to DES
+        exptime = 1.0  # Not used
+    elif survey=="SPLUS":
+        exptime = header['TEXPOSED']
+    elif survey=="UKIDSS":
+        exptime = header['EXP_TIME']*header['NEXP']
     else:
         exptime = 1.0
 
     return exptime
 
 
 def correct_HST_aperture(filt, ap_area, header):
@@ -351,110 +364,143 @@
     filt=None,
     ap_area=0.0,
     header=None,
     bkg_rms=0.0,
 ):
     """Calculates the calibrated magnitudes and errors.
 
+    Error propagation is included here, both for magnitudes
+    and fluxes.
+
     Parameters
     ----------
     flux: float
         Aperture flux.
     survey: str
         Survey name: e.g. ``PS1``, ``GALEX``.
     filt: str, default ``None``
         Survey-specific filter.
     ap_area: float, default ``0.0``
         Aperture area.
     header: fits header, default ``None``
         Header of an image.
     bkg_rms: float, default ``0.0``
         Background noise.
+    invvar_map: ndarray
 
     Returns
     -------
     mag: float
         Apparent magnitude.
     mag_err: float
         Apparent magnitude uncertainty.
     flux: float
         Total flux.
-    flux_error: float
+    flux_err: float
         Total uncertainty in flux.
+    zp: float
+        Zeropoint.
     """
     # get zeropoint
     zp_dict = survey_zp(survey)
     if zp_dict == "header":
         zp = header["MAGZP"]
     else:
         zp = zp_dict[filt]
-    if survey == "PS1":
-        exptime = get_image_exptime(header, survey)
-        zp += 2.5 * np.log10(exptime)
+
+    if survey == "SDSS":
+        # SDSS zero-points are not exactly in AB:
+        # https://www.sdss4.org/dr12/algorithms/fluxcal/#SDSStoAB
+        if filt=='u':
+            offset = -0.04  # mag
+        elif filt=='z':
+            offset = 0.02  # mag
+        else:
+            offset = 0
+        flux *= 10**(-0.4*offset)
+        flux_err *= 10**(-0.4*offset)
+
+    if survey == "unWISE":
+        # To improve the agreement between unWISE and AllWISE fluxes,
+        # these offsets need to be applied: https://catalog.unwise.me/catalogs.html#absolute
+        if filt=='W1':
+            offset = -4e-3  # 4 mmag
+        elif filt=='W2':
+            offset = -32e-3  # 32 mmag
+        else:
+            offset = 0
+        flux *= 10**(-0.4*offset)
+        flux_err *= 10**(-0.4*offset)
+
+    if survey == "HST":
+        # HST needs and aperture correction for the flux
+        # see, e.g. https://www.stsci.edu/hst/instrumentation/acs/data-analysis/aperture-corrections
+        ap_corr = correct_HST_aperture(filt, ap_area, header)
+        flux = flux * ap_corr
 
     # error propagation
-    mag_err, flux_err = uncertainty_calculation(
+    flux_err = uncertainty_calculation(
         flux,
         flux_err,
         survey,
         filt,
         ap_area,
         header,
         bkg_rms,
     )
 
-    if survey == "HST":
-        # HST needs and aperture correction for the flux
-        # see, e.g. https://www.stsci.edu/hst/instrumentation/acs/data-analysis/aperture-corrections
-        ap_corr = correct_HST_aperture(filt, ap_area, header)
-        flux = flux * ap_corr
+    if survey in ["PS1", "VISTA", "UKIDSS"]:
+        # flux needs to be in units of counts per second
+        # but only after the error propagation
+        exptime = get_image_exptime(header, survey)
+        flux /= exptime
+        flux_err /= exptime
 
     mag = -2.5 * np.log10(flux) + zp
+    mag_err = np.abs(2.5 * flux_err / (flux * np.log(10)))
 
-    return mag, mag_err, flux, flux_err
+    return mag, mag_err, flux, flux_err, zp
 
 
 def get_HST_err(filt, header):
     """Obtaines the error propagation from the zeropoint.
 
     Parameters
     ----------
     filt : str
         HST filter, e.g. ``WFC3_UVIS_F225W``.
     header: fits header
         Header of an image.
 
     Returns
     -------
-    flux_err: float
-        Error on PHOTFLAM.
     mag_err: float
         Magnitude error on PHOTFLAM.
     """
     # split instrument and filter
     filt_split = filt.split("_")
     filt = filt_split[-1]
     instrument = filt_split[-2]
 
     if instrument == "UVIS":
-        # APERTURE usually point to UVIS2
+        # APERTURE usually points to UVIS2
         instrument = header["APERTURE"]
 
     # get uncertainty file
     err_file = os.path.join(
         hostphot_path, "filters/HST/", f"{instrument}_err.txt"
     )
     err_df = pd.read_csv(err_file, delim_whitespace=True)
     filt_err_df = err_df[err_df.Filter == filt]
 
     flux = filt_err_df.PHOTFLAM.values[0]
     flux_err = filt_err_df.ERR_PHOTFLAM.values[0]
     mag_err = np.abs(2.5 * flux_err / (flux * np.log(10)))
 
-    return flux_err, mag_err
+    return mag_err
 
 
 def uncertainty_calculation(
     flux, flux_err, survey, filt=None, ap_area=0.0, header=None, bkg_rms=0.0
 ):
     """Calculates the uncertainty propagation.
 
@@ -473,37 +519,34 @@
     header: fits header, default ``None``
         Header of an image.
     bkg_rms: float, default ``0.0``
         Background noise.
 
     Returns
     -------
-    mag_err: float
-        Extra uncertainty in magnitudes.
     flux_err: float
         Total uncertainty in flux units.
     """
     exptime = get_image_exptime(header, survey)
     gain = get_image_gain(header, survey)
     readnoise = get_image_readnoise(header, survey)
 
-    mag_err = 2.5 / np.log(10) * flux_err / flux
+    # 1.0857 = 2.5/ln(10)
+    mag_err = 1.0857 * flux_err / flux
 
-    if survey in ["PS1", "DES", "LegacySurvey", "Spitzer", "VISTA"]:
+    if survey in ["PS1", "DES", "LegacySurvey", "Spitzer", "VISTA",
+                  "SkyMapper", "SPLUS", "UKIDSS"]:
         if survey == "Spitzer":
             flux /= header["EFCONV"]  # conv. factor (MJy/sr)/(DN/s)
-        # 1.0857 = 2.5/ln(10)
+        
         extra_err = (
             1.0857 * np.sqrt(ap_area * (readnoise**2) + flux / gain) / flux
         )
         mag_err = np.sqrt(mag_err**2 + extra_err**2)
 
-        extra_flux_err = np.sqrt(ap_area * (readnoise**2) + flux / gain)
-        flux_err = np.sqrt(flux_err**2 + extra_flux_err**2)
-
     if survey == "DES":
         # see the photometry section in https://des.ncsa.illinois.edu/releases/dr1/dr1-docs/quality
         # statistical uncertainties on the AB magnitud system zeropoints
         unc_dict = {
             "g": 2.6e-3,
             "r": 2.9e-3,
             "i": 3.4e-3,
@@ -520,33 +563,27 @@
             "i": 5e-3,
             "z": 6e-3,
             "Y": 5e-3,
         }
         extra_err = unc_dict[filt]
         mag_err = np.sqrt(mag_err**2 + extra_err**2)
 
-        extra_flux_err = np.abs(flux * 0.4 * np.log(10) * extra_err)
-        flux_err = np.sqrt(flux_err**2 + extra_flux_err**2)
-
     elif survey == "PS1":
         # add floor systematic error from:
         # https://iopscience.iop.org/article/10.3847/1538-4365/abb82a/pdf
         unc_dict = {
             "g": 14e-3,
             "r": 14e-3,
             "i": 15e-3,
             "z": 15e-3,
             "y": 18e-3,
         }
         floor_err = unc_dict[filt]
         mag_err = np.sqrt(mag_err**2 + floor_err**2)
 
-        extra_flux_err = np.abs(flux * 0.4 * np.log(10) * floor_err)
-        flux_err = np.sqrt(flux_err**2 + extra_flux_err**2)
-
     elif survey == "SDSS":
         # https://data.sdss.org/datamodel/files/BOSS_PHOTOOBJ/frames/RERUN/RUN/CAMCOL/frame.html
         camcol = header["CAMCOL"]
         run = header["RUN"]
 
         gain_dict = {
             "u": {1: 1.62, 2: 1.595, 3: 1.59, 4: 1.6, 5: 1.47, 6: 2.17},
@@ -599,17 +636,14 @@
                 dark_variance = 12.6025
             if camcol == 5:
                 dark_variance = 2.1025
 
         extra_err = 1.0857 * np.sqrt(dark_variance + flux / gain) / flux
         mag_err = np.sqrt(mag_err**2 + extra_err**2)
 
-        extra_flux_err = np.sqrt(dark_variance + flux / gain)
-        flux_err = np.sqrt(flux_err**2 + extra_flux_err**2)
-
     elif survey == "GALEX":
         # https://asd.gsfc.nasa.gov/archive/galex/FAQ/counts_background.html
         CPS = flux
         if filt == "FUV":
             uv_err = -2.5 * (
                 np.log10(CPS)
                 - np.log10(
@@ -632,16 +666,14 @@
             )
             flux_uv_err = (
                 np.sqrt(CPS * exptime + (0.027 * CPS * exptime) ** 2) / exptime
             )
 
         mag_err = np.sqrt(mag_err**2 + uv_err**2)
 
-        flux_err = np.sqrt(flux_err**2 + flux_uv_err**2)
-
     elif survey == "2MASS":
         # see: https://wise2.ipac.caltech.edu/staff/jarrett/2mass/3chan/noise/
         S = flux
         N_c = 6  # number of coadd pixels
         k_z = 1.7  # kernel smoothing factor
         n_f = ap_area  # number of frame pixels in the aperture; aprox. as aperture area
         n_c = 4 * n_f  # number of coadd pixels in the aperture
@@ -651,17 +683,14 @@
             S / (gain * N_c)
             + n_c * (2 * k_z * sigma_c) ** 2
             + (n_c * 0.024 * sigma_c) ** 2
         )
 
         mag_err = 1.0857 / SNR
 
-        extra_flux_err = flux / SNR
-        flux_err = np.sqrt(flux_err**2 + extra_flux_err**2)
-
     elif "WISE" in survey:
         # see: https://wise2.ipac.caltech.edu/docs/release/allsky/expsup/sec2_3f.html
         # see Table 5 of
         # https://wise2.ipac.caltech.edu/docs/release/allsky/expsup/sec4_4c.html#wpro
         # correction assumed to be 0 mags as PSF fitting is not used.
         m_apcor = 0.0
         f_apcor = 10 ** (-0.4 * m_apcor)
@@ -683,54 +712,79 @@
             * F_corr
             * (flux_err**2 + k * (N_A**2) / N_B * bkg_rms**2)
             + sigma_conf**2
         )
 
         mag_err = np.sqrt(1.179 * sigma_src**2 / F_src**2)
 
-        flux_err = f_apcor**2
-
         # add uncertainty from the ZP
         if survey == "unWISE":
             # These values are the same for all Atlas Images of a given band...
             # see: https://wise2.ipac.caltech.edu/docs/release/allsky/expsup/sec2_3f.html
             unc_dict = {"W1": 0.006, "W2": 0.007, "W3": 0.012, "W4": 0.012}
             zp_unc = unc_dict[filt]
         elif survey == "WISE":
             zp_unc = header["MAGZPUNC"]
 
         mag_err = np.sqrt(mag_err**2 + zp_unc**2)
 
-        extra_flux_err = np.abs(flux * 0.4 * np.log(10) * zp_unc)
-        flux_err = np.sqrt(flux_err**2 + extra_flux_err**2)
-
     elif survey == "LegacySurvey":
-        # already added at the beginning
-        pass
+        # photometry uncertainties for DR10 from https://ui.adsabs.harvard.edu/abs/2023RNAAS...7..105Z/abstract
+        # LS also includes uncertainties from inverse-variance maps
+        # (calculated outside this function), as mentioned by Dustin Lang
+        unc_dict = {
+            "g": 5.0e-3,
+            "r": 3.9e-3,
+            "i": 4.3e-3,
+            "z": 5.5e-3,
+        }
+        extra_err = unc_dict[filt]
+        mag_err = np.sqrt(mag_err**2 + extra_err**2)
+
     elif survey == "Spitzer":
         # already added at the beginning
         pass
     elif survey == "VISTA":
         # add uncertainty from the ZP
         zp_unc = header["MAGZRR"]
         mag_err = np.sqrt(mag_err**2 + zp_unc**2)
 
-        extra_flux_err = np.abs(flux * 0.4 * np.log(10) * zp_unc)
-        flux_err = np.sqrt(flux_err**2 + extra_flux_err**2)
     elif survey == "HST":
-        flux_zp_unc, zp_unc = get_HST_err(filt, header)
+        zp_unc = get_HST_err(filt, header)
+        mag_err = np.sqrt(mag_err**2 + zp_unc**2)
 
+    elif survey == "SkyMapper":
+        zp_unc = header["ZPTERR"]
+        mag_err = np.sqrt(mag_err**2 + zp_unc**2)
+
+    elif survey == "SPLUS":
+        # following Section 4.4 of Almeida-Fernandes et al. (2022)
+        zp_uncs = {'U':25e-3,
+           'F395':25e-3,
+           'F378':15e-3,
+          }
+        if filt in zp_uncs.keys():
+            zp_unc = zp_uncs[filt]
+        else:
+            zp_unc = 1e-3
         mag_err = np.sqrt(mag_err**2 + zp_unc**2)
-        flux_err = np.sqrt(flux_err**2 + flux_zp_unc**2)
+
+    elif survey == "UKIDSS":
+        # nightly ZPs rms
+        zp_unc = header["MAGZRR"]
+        mag_err = np.sqrt(mag_err**2 + zp_unc**2)
+
     else:
         raise Exception(
             f"Survey {survey} has not been added for error propagation."
         )
 
-    return mag_err, flux_err
+    flux_err = np.abs(flux * 0.4 * np.log(10) * mag_err)
+
+    return flux_err
 
 
 def survey_pixel_scale(survey, filt=None):
     """Returns the pixel scale for a given survey.
 
     Parameters
     ----------
@@ -1030,14 +1084,53 @@
     fig.axis_labels.set_font(**{"family": font_family, "size": 18})
 
     fig.set_title(title, **{"family": font_family, "size": 24})
     fig.set_theme("publication")
 
     plt.show()
 
+def plot_image(image_file):
+    """Plots an image file.
+
+    E.g. '.png' and '.jpg' files.
+
+    Parameters
+    ----------
+    image_file: str
+        Path to an image file.
+    """
+    fig, ax = plt.subplots(figsize=(16, 8))
+
+    im = img.imread(image_file)
+    ax.imshow(im)
+    plt.axis('off')
+
+    plt.show()
+
+
+def load_pickle(inputfile):
+    """Loads a pickle file.
+    
+    Parameters
+    ----------
+    inputfile: str
+        Pickle file to load.
+        
+    Returns
+    -------
+    content: any
+        The content of the pickle file
+    """
+    if os.path.isfile(inputfile) is True:
+        with open(inputfile, 'rb') as fp:
+            content = pickle.load(fp)
+    else:
+        raise FileNotFoundError(f"The input file does not exist: {inputfile}")
+        
+    return content
 
 @contextmanager
 def suppress_stdout():
     """Suppresses annoying outputs.
 
     Useful with astroquery and aplpy packages.
     """
```

### Comparing `hostphot-2.7.1/src/hostphot.egg-info/PKG-INFO` & `hostphot-2.8.0/src/hostphot.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hostphot
-Version: 2.7.1
+Version: 2.8.0
 Summary: Global and local photometry of galaxies hosting supernovae or other transients
 Home-page: https://github.com/temuller/hostphot
 Author: Tomás Enrique Müller-Bravo and Lluís Galbany
 Author-email: t.e.muller-bravo@ice.csic.es
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -192,14 +192,27 @@
   number = {76}, 
   pages = {4508},  
   journal = {Journal of Open Source Software} 
 } 
 ```
 
 ## What's new!
+v2.8.0
+* Fix SED plotting with negative or too large values/errors, and improve plotting aesthetics
+* Fix problem downloading some 2MASS images giving internal server error (no image overlap)
+* Adding UKIDSS, SPLUS and SkyMapper surveys. WARNINGS: SkyMapper photometry (DR2) is not very accurate with extended sources!
+* The marker showing the galaxy position on images has changed colour for better visualization
+* Adding functions to easily load previously saved parameteres from pickle files
+* Adding missing extinction correction for flux (not magnitudes)
+* Including exposure time into flux for PS1, VISTA and UKIDSS surveys
+* Adding SDSS ZP offsets into flux
+* Output zeropoint together with the photometry
+* Updating LegacySurvey errors, taken from inverse-variance maps and ZP uncertainty
+* Adding missing offsets to unWISE W1 and W2 bands into fluxes
+* Kron radius is no longer "optimized", just the scale, which doesn't have any effect in practice for the user
 v2.7.1
 * Adding SED plotting
 * Fixed plotting angle of masked object 
 v2.7.0
 * MAJOR BUG: Convertion factor between different pixel scales fixed (it was previously inverted). This affects the common aperture photometry between different surveys!
 * Moving font family to `_constant.py` file
 v2.6.2
```

### Comparing `hostphot-2.7.1/src/hostphot.egg-info/SOURCES.txt` & `hostphot-2.8.0/src/hostphot.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -263,34 +263,56 @@
 src/hostphot/filters/LegacySurvey/BASS_g.dat
 src/hostphot/filters/LegacySurvey/BASS_r.dat
 src/hostphot/filters/LegacySurvey/DECAM_g.dat
 src/hostphot/filters/LegacySurvey/DECAM_r.dat
 src/hostphot/filters/LegacySurvey/DECAM_z.dat
 src/hostphot/filters/LegacySurvey/MzLS_z.dat
 src/hostphot/filters/LegacySurvey/README.txt
-src/hostphot/filters/LegacySurvey/init_BASS_g.dat
-src/hostphot/filters/LegacySurvey/init_BASS_r.dat
 src/hostphot/filters/PS1/AAA_README.dat
 src/hostphot/filters/PS1/PS1_g.dat
 src/hostphot/filters/PS1/PS1_i.dat
 src/hostphot/filters/PS1/PS1_r.dat
 src/hostphot/filters/PS1/PS1_y.dat
 src/hostphot/filters/PS1/PS1_z.dat
 src/hostphot/filters/SDSS/AAA_README
 src/hostphot/filters/SDSS/SDSS_g.dat
 src/hostphot/filters/SDSS/SDSS_i.dat
 src/hostphot/filters/SDSS/SDSS_r.dat
 src/hostphot/filters/SDSS/SDSS_u.dat
 src/hostphot/filters/SDSS/SDSS_z.dat
+src/hostphot/filters/SPLUS/SPLUS_F378.dat
+src/hostphot/filters/SPLUS/SPLUS_F395.dat
+src/hostphot/filters/SPLUS/SPLUS_F410.dat
+src/hostphot/filters/SPLUS/SPLUS_F430.dat
+src/hostphot/filters/SPLUS/SPLUS_F515.dat
+src/hostphot/filters/SPLUS/SPLUS_F660.dat
+src/hostphot/filters/SPLUS/SPLUS_F861.dat
+src/hostphot/filters/SPLUS/SPLUS_g.dat
+src/hostphot/filters/SPLUS/SPLUS_i.dat
+src/hostphot/filters/SPLUS/SPLUS_r.dat
+src/hostphot/filters/SPLUS/SPLUS_u.dat
+src/hostphot/filters/SPLUS/SPLUS_z.dat
+src/hostphot/filters/SPLUS/iDR3_zps.cat
+src/hostphot/filters/SkyMapper/SkyMapper_g.dat
+src/hostphot/filters/SkyMapper/SkyMapper_i.dat
+src/hostphot/filters/SkyMapper/SkyMapper_r.dat
+src/hostphot/filters/SkyMapper/SkyMapper_u.dat
+src/hostphot/filters/SkyMapper/SkyMapper_v.dat
+src/hostphot/filters/SkyMapper/SkyMapper_z.dat
 src/hostphot/filters/Spitzer/README.txt
 src/hostphot/filters/Spitzer/Spitzer_IRAC.1.dat
 src/hostphot/filters/Spitzer/Spitzer_IRAC.2.dat
 src/hostphot/filters/Spitzer/Spitzer_IRAC.3.dat
 src/hostphot/filters/Spitzer/Spitzer_IRAC.4.dat
 src/hostphot/filters/Spitzer/Spitzer_MIPS.1.dat
+src/hostphot/filters/UKIDSS/UKIDSS_H.dat
+src/hostphot/filters/UKIDSS/UKIDSS_J.dat
+src/hostphot/filters/UKIDSS/UKIDSS_K.dat
+src/hostphot/filters/UKIDSS/UKIDSS_Y.dat
+src/hostphot/filters/UKIDSS/UKIDSS_Z.dat
 src/hostphot/filters/VISTA/README.txt
 src/hostphot/filters/VISTA/VISTA_H.dat
 src/hostphot/filters/VISTA/VISTA_J.dat
 src/hostphot/filters/VISTA/VISTA_Ks.dat
 src/hostphot/filters/VISTA/VISTA_Y.dat
 src/hostphot/filters/VISTA/VISTA_Z.dat
 src/hostphot/filters/WISE/AAA_README
```

### Comparing `hostphot-2.7.1/tests/test_cutouts.py` & `hostphot-2.8.0/tests/test_cutouts.py`

 * *Files 13% similar despite different names*

```diff
@@ -89,10 +89,29 @@
         except Exception as exc:
             warnings.warn(
                 "The VISTA SCIENCE ARCHIVE might be having issues..."
             )
             print("Skipping this test...")
             print(exc)
 
+    def test_cutouts_SkyMapper(self):
+        download_images(
+            self.sn_name,
+            self.ra,
+            self.dec,
+            overwrite=True,
+            survey="SkyMapper",
+        )
+
+    def test_cutouts_SPLUS(self):
+        name = "SPLUS_test"
+        ra, dec = 0.6564206, -0.3740297
+        download_images(name, ra, dec, overwrite=True, survey="SPLUS")
+
+    def test_cutouts_UKIDSS(self):
+        name = "UNIDSS_test"
+        ra, dec = 359.5918320, +0.1964120
+        download_images(name, ra, dec, overwrite=True, survey="UKIDSS")
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `hostphot-2.7.1/tests/test_global_phot.py` & `hostphot-2.8.0/tests/test_global_phot.py`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/tests/test_local_phot.py` & `hostphot-2.8.0/tests/test_local_phot.py`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/tests/test_preprocessing.py` & `hostphot-2.8.0/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `hostphot-2.7.1/tests/test_rgb_images.py` & `hostphot-2.8.0/tests/test_rgb_images.py`

 * *Files identical despite different names*

