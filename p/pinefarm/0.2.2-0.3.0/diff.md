# Comparing `tmp/pinefarm-0.2.2.tar.gz` & `tmp/pinefarm-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinefarm-0.2.2.tar", max compression
+gzip compressed data, was "pinefarm-0.3.0.tar", max compression
```

## Comparing `pinefarm-0.2.2.tar` & `pinefarm-0.3.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0      827 2023-02-15 16:34:06.275544 pinefarm-0.2.2/README.md
--rw-r--r--   0        0        0     3187 2023-02-15 16:34:57.524012 pinefarm-0.2.2/pyproject.toml
--rw-r--r--   0        0        0       49 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/__init__.py
--rw-r--r--   0        0        0       90 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/cli/__init__.py
--rw-r--r--   0        0        0     1215 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/cli/_base.py
--rw-r--r--   0        0        0      207 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/cli/configs.py
--rw-r--r--   0        0        0     1534 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/cli/info.py
--rw-r--r--   0        0        0      826 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/cli/install.py
--rw-r--r--   0        0        0     1101 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/cli/list.py
--rw-r--r--   0        0        0     2784 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/cli/merge.py
--rw-r--r--   0        0        0     3404 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/cli/run.py
--rw-r--r--   0        0        0     1015 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/cli/update.py
--rw-r--r--   0        0        0     7251 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/configs.py
--rw-r--r--   0        0        0      220 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/confs/lhapdf.conf
--rw-r--r--   0        0        0       29 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/external/__init__.py
--rw-r--r--   0        0        0     3285 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/external/integrability.py
--rw-r--r--   0        0        0     4458 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/external/interface.py
--rw-r--r--   0        0        0    10263 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/external/mg5/__init__.py
--rw-r--r--   0        0        0     1425 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/external/mg5/cuts_code/abscoscsmax.f
--rw-r--r--   0        0        0     1425 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/external/mg5/cuts_code/abscoscsmin.f
--rw-r--r--   0        0        0     1103 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/external/mg5/cuts_code/atlas_1jet_8tev_r06.f
--rw-r--r--   0        0        0      504 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/external/mg5/cuts_code/atlas_2jet_7tev_r06_0005.f
--rw-r--r--   0        0        0      524 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/external/mg5/cuts_code/atlas_2jet_7tev_r06_0510.f
--rw-r--r--   0        0        0      524 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/external/mg5/cuts_code/atlas_2jet_7tev_r06_1015.f
--rw-r--r--   0        0        0      524 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/external/mg5/cuts_code/atlas_2jet_7tev_r06_1520.f
--rw-r--r--   0        0        0      525 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/external/mg5/cuts_code/atlas_2jet_7tev_r06_2025.f
--rw-r--r--   0        0        0      525 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/external/mg5/cuts_code/atlas_2jet_7tev_r06_2530.f
--rw-r--r--   0        0        0     3827 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/external/mg5/cuts_code/atlas_dy3d_8tev.f
--rw-r--r--   0        0        0      911 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/external/mg5/cuts_code/atlas_wzrap11_cf.f
--rw-r--r--   0        0        0     1854 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/external/mg5/cuts_code/cms_2jet_3d_8tev.f
--rw-r--r--   0        0        0      507 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/external/mg5/cuts_code/cms_2jets_7tev_0005.f
--rw-r--r--   0        0        0      526 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/external/mg5/cuts_code/cms_2jets_7tev_0510.f
--rw-r--r--   0        0        0      526 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/external/mg5/cuts_code/cms_2jets_7tev_1015.f
--rw-r--r--   0        0        0      526 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/external/mg5/cuts_code/cms_2jets_7tev_1520.f
--rw-r--r--   0        0        0      527 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/external/mg5/cuts_code/cms_2jets_7tev_2025.f
--rw-r--r--   0        0        0      230 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/external/mg5/cuts_code/dyjj.f
--rw-r--r--   0        0        0      344 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/external/mg5/cuts_code/minetal.f
--rw-r--r--   0        0        0      172 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/external/mg5/cuts_code/mjj.f
--rw-r--r--   0        0        0      409 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/external/mg5/cuts_code/mmllmax.f
--rw-r--r--   0        0        0      625 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/external/mg5/cuts_code/mtw.f
--rw-r--r--   0        0        0      131 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/external/mg5/cuts_code/ptj1min.f
--rw-r--r--   0        0        0      352 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/external/mg5/cuts_code/ptl1min.f
--rw-r--r--   0        0        0      451 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/external/mg5/cuts_code/ptmiss.f
--rw-r--r--   0        0        0      449 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/external/mg5/cuts_code/ptzmax.f
--rw-r--r--   0        0        0      449 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/external/mg5/cuts_code/ptzmin.f
--rw-r--r--   0        0        0      264 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/external/mg5/cuts_code/yh.f
--rw-r--r--   0        0        0      977 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/external/mg5/cuts_code/yll.f
--rw-r--r--   0        0        0      283 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/external/mg5/cuts_code/yt.f
--rw-r--r--   0        0        0      456 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/external/mg5/cuts_code/yz.f
--rw-r--r--   0        0        0      456 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/external/mg5/cuts_code/yzmin.f
--rw-r--r--   0        0        0      178 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/external/mg5/cuts_variables/abscoscs.f
--rw-r--r--   0        0        0       86 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/external/mg5/cuts_variables/atlas_1jet_8tev_r06.f
--rw-r--r--   0        0        0      143 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/external/mg5/cuts_variables/atlas_dy3d_8tev.f
--rw-r--r--   0        0        0       99 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/external/mg5/cuts_variables/atlas_wzrap11_cf.f
--rw-r--r--   0        0        0       37 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/external/mg5/cuts_variables/cms_2jet_3d_8tev.f
--rw-r--r--   0        0        0       45 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/external/mg5/cuts_variables/mtw.f
--rw-r--r--   0        0        0       53 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/external/mg5/cuts_variables/ptmiss.f
--rw-r--r--   0        0        0     2144 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/external/mg5/patches/change_etaj_to_rapj.patch
--rw-r--r--   0        0        0      380 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/external/mg5/patches/no_pole_cancellation_checks.patch
--rw-r--r--   0        0        0     9504 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/external/mg5/patches/set_tau_min.patch
--rw-r--r--   0        0        0      172 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/external/mg5/paths.py
--rw-r--r--   0        0        0     3654 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/external/positivity.py
--rw-r--r--   0        0        0     8001 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/external/vrap.py
--rw-r--r--   0        0        0     3338 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/external/yad.py
--rw-r--r--   0        0        0     1016 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/info.py
--rw-r--r--   0        0        0    10268 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/install.py
--rw-r--r--   0        0        0     3453 2023-02-15 16:34:06.279544 pinefarm-0.2.2/src/pinefarm/log.py
--rw-r--r--   0        0        0     3437 2023-02-15 16:34:06.283544 pinefarm-0.2.2/src/pinefarm/table.py
--rw-r--r--   0        0        0     6926 2023-02-15 16:34:06.283544 pinefarm-0.2.2/src/pinefarm/tools.py
--rw-r--r--   0        0        0      174 2023-02-15 16:34:06.283544 pinefarm-0.2.2/src/pinefarm/variables.json
--rw-r--r--   0        0        0     2280 1970-01-01 00:00:00.000000 pinefarm-0.2.2/setup.py
--rw-r--r--   0        0        0     2359 1970-01-01 00:00:00.000000 pinefarm-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-22 16:35:23.769981 pinefarm-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1539 2023-06-22 16:35:23.769981 pinefarm-0.3.0/README.md
+-rw-r--r--   0        0        0     2889 2023-06-22 16:36:15.954454 pinefarm-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      106 2023-06-22 16:35:23.769981 pinefarm-0.3.0/src/pinefarm/__init__.py
+-rw-r--r--   0        0        0      109 2023-06-22 16:35:23.769981 pinefarm-0.3.0/src/pinefarm/cli/__init__.py
+-rw-r--r--   0        0        0     1327 2023-06-22 16:35:23.769981 pinefarm-0.3.0/src/pinefarm/cli/_base.py
+-rw-r--r--   0        0        0      281 2023-06-22 16:35:23.769981 pinefarm-0.3.0/src/pinefarm/cli/configs.py
+-rw-r--r--   0        0        0     1557 2023-06-22 16:35:23.769981 pinefarm-0.3.0/src/pinefarm/cli/info.py
+-rw-r--r--   0        0        0      851 2023-06-22 16:35:23.769981 pinefarm-0.3.0/src/pinefarm/cli/install.py
+-rw-r--r--   0        0        0     1169 2023-06-22 16:35:23.769981 pinefarm-0.3.0/src/pinefarm/cli/list.py
+-rw-r--r--   0        0        0     2902 2023-06-22 16:35:23.769981 pinefarm-0.3.0/src/pinefarm/cli/merge.py
+-rw-r--r--   0        0        0     3459 2023-06-22 16:35:23.769981 pinefarm-0.3.0/src/pinefarm/cli/run.py
+-rw-r--r--   0        0        0     1093 2023-06-22 16:35:23.769981 pinefarm-0.3.0/src/pinefarm/cli/update.py
+-rw-r--r--   0        0        0     7285 2023-06-22 16:35:23.769981 pinefarm-0.3.0/src/pinefarm/configs.py
+-rw-r--r--   0        0        0      220 2023-06-22 16:35:23.769981 pinefarm-0.3.0/src/pinefarm/confs/lhapdf.conf
+-rw-r--r--   0        0        0       56 2023-06-22 16:35:23.769981 pinefarm-0.3.0/src/pinefarm/external/__init__.py
+-rw-r--r--   0        0        0     3521 2023-06-22 16:35:23.769981 pinefarm-0.3.0/src/pinefarm/external/integrability.py
+-rw-r--r--   0        0        0     4644 2023-06-22 16:35:23.769981 pinefarm-0.3.0/src/pinefarm/external/interface.py
+-rw-r--r--   0        0        0    10614 2023-06-22 16:35:23.769981 pinefarm-0.3.0/src/pinefarm/external/mg5/__init__.py
+-rw-r--r--   0        0        0     1425 2023-06-22 16:35:23.769981 pinefarm-0.3.0/src/pinefarm/external/mg5/cuts_code/abscoscsmax.f
+-rw-r--r--   0        0        0     1425 2023-06-22 16:35:23.769981 pinefarm-0.3.0/src/pinefarm/external/mg5/cuts_code/abscoscsmin.f
+-rw-r--r--   0        0        0     1103 2023-06-22 16:35:23.769981 pinefarm-0.3.0/src/pinefarm/external/mg5/cuts_code/atlas_1jet_8tev_r06.f
+-rw-r--r--   0        0        0      504 2023-06-22 16:35:23.769981 pinefarm-0.3.0/src/pinefarm/external/mg5/cuts_code/atlas_2jet_7tev_r06_0005.f
+-rw-r--r--   0        0        0      524 2023-06-22 16:35:23.769981 pinefarm-0.3.0/src/pinefarm/external/mg5/cuts_code/atlas_2jet_7tev_r06_0510.f
+-rw-r--r--   0        0        0      524 2023-06-22 16:35:23.769981 pinefarm-0.3.0/src/pinefarm/external/mg5/cuts_code/atlas_2jet_7tev_r06_1015.f
+-rw-r--r--   0        0        0      524 2023-06-22 16:35:23.769981 pinefarm-0.3.0/src/pinefarm/external/mg5/cuts_code/atlas_2jet_7tev_r06_1520.f
+-rw-r--r--   0        0        0      525 2023-06-22 16:35:23.769981 pinefarm-0.3.0/src/pinefarm/external/mg5/cuts_code/atlas_2jet_7tev_r06_2025.f
+-rw-r--r--   0        0        0      525 2023-06-22 16:35:23.769981 pinefarm-0.3.0/src/pinefarm/external/mg5/cuts_code/atlas_2jet_7tev_r06_2530.f
+-rw-r--r--   0        0        0     3827 2023-06-22 16:35:23.769981 pinefarm-0.3.0/src/pinefarm/external/mg5/cuts_code/atlas_dy3d_8tev.f
+-rw-r--r--   0        0        0      911 2023-06-22 16:35:23.769981 pinefarm-0.3.0/src/pinefarm/external/mg5/cuts_code/atlas_wzrap11_cf.f
+-rw-r--r--   0        0        0     1854 2023-06-22 16:35:23.769981 pinefarm-0.3.0/src/pinefarm/external/mg5/cuts_code/cms_2jet_3d_8tev.f
+-rw-r--r--   0        0        0      507 2023-06-22 16:35:23.773981 pinefarm-0.3.0/src/pinefarm/external/mg5/cuts_code/cms_2jets_7tev_0005.f
+-rw-r--r--   0        0        0      526 2023-06-22 16:35:23.773981 pinefarm-0.3.0/src/pinefarm/external/mg5/cuts_code/cms_2jets_7tev_0510.f
+-rw-r--r--   0        0        0      526 2023-06-22 16:35:23.773981 pinefarm-0.3.0/src/pinefarm/external/mg5/cuts_code/cms_2jets_7tev_1015.f
+-rw-r--r--   0        0        0      526 2023-06-22 16:35:23.773981 pinefarm-0.3.0/src/pinefarm/external/mg5/cuts_code/cms_2jets_7tev_1520.f
+-rw-r--r--   0        0        0      527 2023-06-22 16:35:23.773981 pinefarm-0.3.0/src/pinefarm/external/mg5/cuts_code/cms_2jets_7tev_2025.f
+-rw-r--r--   0        0        0      230 2023-06-22 16:35:23.773981 pinefarm-0.3.0/src/pinefarm/external/mg5/cuts_code/dyjj.f
+-rw-r--r--   0        0        0      344 2023-06-22 16:35:23.773981 pinefarm-0.3.0/src/pinefarm/external/mg5/cuts_code/minetal.f
+-rw-r--r--   0        0        0      172 2023-06-22 16:35:23.773981 pinefarm-0.3.0/src/pinefarm/external/mg5/cuts_code/mjj.f
+-rw-r--r--   0        0        0      409 2023-06-22 16:35:23.773981 pinefarm-0.3.0/src/pinefarm/external/mg5/cuts_code/mmllmax.f
+-rw-r--r--   0        0        0      625 2023-06-22 16:35:23.773981 pinefarm-0.3.0/src/pinefarm/external/mg5/cuts_code/mtw.f
+-rw-r--r--   0        0        0      131 2023-06-22 16:35:23.773981 pinefarm-0.3.0/src/pinefarm/external/mg5/cuts_code/ptj1min.f
+-rw-r--r--   0        0        0      352 2023-06-22 16:35:23.773981 pinefarm-0.3.0/src/pinefarm/external/mg5/cuts_code/ptl1min.f
+-rw-r--r--   0        0        0      451 2023-06-22 16:35:23.773981 pinefarm-0.3.0/src/pinefarm/external/mg5/cuts_code/ptmiss.f
+-rw-r--r--   0        0        0      449 2023-06-22 16:35:23.773981 pinefarm-0.3.0/src/pinefarm/external/mg5/cuts_code/ptzmax.f
+-rw-r--r--   0        0        0      449 2023-06-22 16:35:23.773981 pinefarm-0.3.0/src/pinefarm/external/mg5/cuts_code/ptzmin.f
+-rw-r--r--   0        0        0      264 2023-06-22 16:35:23.773981 pinefarm-0.3.0/src/pinefarm/external/mg5/cuts_code/yh.f
+-rw-r--r--   0        0        0      977 2023-06-22 16:35:23.773981 pinefarm-0.3.0/src/pinefarm/external/mg5/cuts_code/yll.f
+-rw-r--r--   0        0        0      283 2023-06-22 16:35:23.773981 pinefarm-0.3.0/src/pinefarm/external/mg5/cuts_code/yt.f
+-rw-r--r--   0        0        0      456 2023-06-22 16:35:23.773981 pinefarm-0.3.0/src/pinefarm/external/mg5/cuts_code/yz.f
+-rw-r--r--   0        0        0      456 2023-06-22 16:35:23.773981 pinefarm-0.3.0/src/pinefarm/external/mg5/cuts_code/yzmin.f
+-rw-r--r--   0        0        0      178 2023-06-22 16:35:23.773981 pinefarm-0.3.0/src/pinefarm/external/mg5/cuts_variables/abscoscs.f
+-rw-r--r--   0        0        0       86 2023-06-22 16:35:23.773981 pinefarm-0.3.0/src/pinefarm/external/mg5/cuts_variables/atlas_1jet_8tev_r06.f
+-rw-r--r--   0        0        0      143 2023-06-22 16:35:23.773981 pinefarm-0.3.0/src/pinefarm/external/mg5/cuts_variables/atlas_dy3d_8tev.f
+-rw-r--r--   0        0        0       99 2023-06-22 16:35:23.773981 pinefarm-0.3.0/src/pinefarm/external/mg5/cuts_variables/atlas_wzrap11_cf.f
+-rw-r--r--   0        0        0       37 2023-06-22 16:35:23.773981 pinefarm-0.3.0/src/pinefarm/external/mg5/cuts_variables/cms_2jet_3d_8tev.f
+-rw-r--r--   0        0        0       45 2023-06-22 16:35:23.773981 pinefarm-0.3.0/src/pinefarm/external/mg5/cuts_variables/mtw.f
+-rw-r--r--   0        0        0       53 2023-06-22 16:35:23.773981 pinefarm-0.3.0/src/pinefarm/external/mg5/cuts_variables/ptmiss.f
+-rw-r--r--   0        0        0     2135 2023-06-22 16:35:23.773981 pinefarm-0.3.0/src/pinefarm/external/mg5/patches/change_etaj_to_rapj.patch
+-rw-r--r--   0        0        0      380 2023-06-22 16:35:23.773981 pinefarm-0.3.0/src/pinefarm/external/mg5/patches/no_pole_cancellation_checks.patch
+-rw-r--r--   0        0        0     9503 2023-06-22 16:35:23.773981 pinefarm-0.3.0/src/pinefarm/external/mg5/patches/set_tau_min.patch
+-rw-r--r--   0        0        0      209 2023-06-22 16:35:23.773981 pinefarm-0.3.0/src/pinefarm/external/mg5/paths.py
+-rw-r--r--   0        0        0     3765 2023-06-22 16:35:23.773981 pinefarm-0.3.0/src/pinefarm/external/positivity.py
+-rw-r--r--   0        0        0     7985 2023-06-22 16:35:23.773981 pinefarm-0.3.0/src/pinefarm/external/vrap.py
+-rw-r--r--   0        0        0     3565 2023-06-22 16:35:23.773981 pinefarm-0.3.0/src/pinefarm/external/yad.py
+-rw-r--r--   0        0        0     1139 2023-06-22 16:35:23.773981 pinefarm-0.3.0/src/pinefarm/info.py
+-rw-r--r--   0        0        0    10333 2023-06-22 16:35:23.773981 pinefarm-0.3.0/src/pinefarm/install.py
+-rw-r--r--   0        0        0     3585 2023-06-22 16:35:23.773981 pinefarm-0.3.0/src/pinefarm/log.py
+-rw-r--r--   0        0        0     3481 2023-06-22 16:35:23.773981 pinefarm-0.3.0/src/pinefarm/table.py
+-rw-r--r--   0        0        0     6951 2023-06-22 16:35:23.773981 pinefarm-0.3.0/src/pinefarm/tools.py
+-rw-r--r--   0        0        0      174 2023-06-22 16:35:23.773981 pinefarm-0.3.0/src/pinefarm/variables.json
+-rw-r--r--   0        0        0     2834 1970-01-01 00:00:00.000000 pinefarm-0.3.0/PKG-INFO
```

### Comparing `pinefarm-0.2.2/pyproject.toml` & `pinefarm-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pinefarm"
-version = "0.2.2"
+version = "0.3.0"
 description = "Generate PineAPPL grids from PineCards."
 authors = [
   "Alessandro Candido <candido.ale@gmail.com>",
   "Juan Cruz Martinez <juan.cruz@mi.infn.it>",
   "Felix Hekhorn <felix.hekhorn@mi.infn.it>",
   "Christopher Schwan <handgranaten-herbert@posteo.de>",
 ]
@@ -18,35 +18,29 @@
 packages = [{ include = "pinefarm", from = "src" }]
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.11"
+python = ">=3.8,<3.12"
 click = "^8.0.1"
 rich = "^12.5.1"
 PyYAML = "^6.0.0"
-yadism = { extras = ["box"], version = "^0.12.3" }
+yadism = { extras = ["box"], version = "^0.12.4" }
 pandas = "^1.3.0"
 lz4 = "^4.0.2"
 pkgconfig = "^1.5.5"
-pygit2 = "1.9.2"
+pygit2 = "^1.12.0"
 requests = "^2.26.0"
-a3b2bbc3ced97675ac3a71df45f55ba = "^6.4.0"
-lhapdf-management = "^0.2"
-pineappl = "^0.5.7"
+lhapdf-management = "^0.3"
+pineappl = "^0.6.0"
 more-itertools = "^8.10.0"
 appdirs = "^1.4.4"
 tomli = "^2.0.1"
-# docs dependencies (for readthedocs)
-Sphinx = { version = "^4.2.0", optional = true }
-sphinx-rtd-theme = { version = "^1.0.0", optional = true }
-sphinxcontrib-bibtex = { version = "^2.4.1", optional = true }
-eko = { extras = ["box"], version = "^0.12.0" }
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 Sphinx = "^4.2.0"
 sphinx-rtd-theme = "^1.0.0"
```

### Comparing `pinefarm-0.2.2/src/pinefarm/cli/_base.py` & `pinefarm-0.3.0/src/pinefarm/cli/_base.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Set up CLI."""
 import pathlib
 import warnings
 
 import click
 
 from .. import configs
 
@@ -14,14 +15,15 @@
     "--configs",
     "cfg",
     default=None,
     type=click.Path(resolve_path=True, path_type=pathlib.Path),
     help="Explicitly specify config file (it has to be a valid TOML file).",
 )
 def command(cfg):
+    """Compute theory predictions in form of interpolation grids from external generators."""
     try:
         cfgpath = configs.detect(cfg)
     except FileNotFoundError:
         warnings.warn("No configuration file detected.")
         cfgpath = None
 
     base_configs = configs.load(cfgpath)
```

### Comparing `pinefarm-0.2.2/src/pinefarm/cli/info.py` & `pinefarm-0.3.0/src/pinefarm/cli/info.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Inspect runcards."""
 import pathlib
 
 import click
 import rich
 
 from .. import configs, info, tools
 from ._base import command
@@ -49,9 +50,8 @@
 
     rich.print_json(data=infod)
 
 
 @subcommand.command("configs")
 def subconfigs():
     """Inspect loaded configs."""
-
     rich.print_json(data=configs.raw(configs.configs))
```

### Comparing `pinefarm-0.2.2/src/pinefarm/cli/install.py` & `pinefarm-0.3.0/src/pinefarm/cli/install.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Install utilities."""
 import click
 
 from .. import install
 from ._base import command
 
 
 @command.group("install")
```

### Comparing `pinefarm-0.2.2/src/pinefarm/cli/list.py` & `pinefarm-0.3.0/src/pinefarm/cli/list.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""List available resources."""
 import rich
 import rich.markdown
 
 from .. import configs, external
 from ._base import command
 
 
@@ -36,14 +37,15 @@
 @mg5.command()
 def cuts():
     """List available cuts."""
     main(external.mg5.paths.cuts_code, files=True)
 
 
 def main(path, files=False, prefix=""):
+    """List available resources."""
     report = ""
     for p in sorted(path.glob("*")):
         name = None
         if p.is_dir():
             name = p.name
         if files and p.is_file():
             name = p.stem
```

### Comparing `pinefarm-0.2.2/src/pinefarm/cli/merge.py` & `pinefarm-0.3.0/src/pinefarm/cli/merge.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Merge multiple PineAPPL grids into a single one."""
 import itertools
 import pathlib
 import re
 import shutil
 
 import click
 import pineappl
@@ -11,19 +12,19 @@
 from ._base import command
 
 
 @command.command("merge")
 @click.argument("grids", nargs=-1)
 def subcommand(grids):
     """Merge multiple PineAPPL grids into a single one."""
-
     main(grids)
 
 
 def main(grids):
+    """Merge multiple PineAPPL grids into a single one."""
     if len(grids) < 2:
         raise ValueError("At least 2 grids needed for a merge.")
 
     grid_paths = [pathlib.Path(grid) for grid in grids]
     grids = [pineappl.grid.Grid.read(str(grid)) for grid in grids]
 
     common = tools.common_substring(*(grid.name for grid in grid_paths)).strip("_")
@@ -66,15 +67,15 @@
         tmpresults.append("\n".join(results_rows))
 
     # set the results metadata in the new grid
     mgridtmp = mgrid_path.parent / (mgrid_path.name + ".tmp")
     tools.update_grid_metadata(
         mgrid_path, mgridtmp, entries={"results": "\n".join(tmpresults)}
     )
-    shutil.move(str(mgridtmp), mgrid_path)
+    shutil.move(str(mgridtmp), str(mgrid_path))
 
     mkeys = mgrid.key_values()
     for key in keys:
         if key == "results":
             continue
 
         mvalue = mkeys.get(key)
```

### Comparing `pinefarm-0.2.2/src/pinefarm/cli/run.py` & `pinefarm-0.3.0/src/pinefarm/cli/run.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Compute a dataset and compare using a given PDF."""
 import pathlib
 import time
 
 import click
 import rich
 import yaml
```

### Comparing `pinefarm-0.2.2/src/pinefarm/configs.py` & `pinefarm-0.3.0/src/pinefarm/configs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
+"""Configuration tools."""
 import copy
 import os
 import pathlib
 import shutil
 import tempfile
 import warnings
 from typing import Optional
 
 import appdirs
 import tomli
 
 NAME = "pinefarm.toml"
-"""Name of the config while (wherever it is placed)"""
+"""Name of the config while (wherever it is placed)."""
 
 PATHS_SECTIONS = ("paths", "commands")
-"""Sections containing only paths"""
+"""Sections containing only paths."""
 
 configs = {}
-"Holds loaded configurations"
+"""Holds loaded configurations."""
 
 
 def detect(path: Optional[os.PathLike] = None) -> pathlib.Path:
     """Detect configuration files.
 
     Parameters
     ----------
```

### Comparing `pinefarm-0.2.2/src/pinefarm/external/integrability.py` & `pinefarm-0.3.0/src/pinefarm/external/integrability.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,35 @@
+"""Integrability interface."""
 import dataclasses
 import json
 import typing
 
-import lhapdf
 import numpy as np
 import pandas as pd
 import pineappl
 import yaml
 from eko import basis_rotation as br
 
 from .. import configs
 from . import interface
 
 _RUNCARD = "integrability.yaml"
 
 
 def is_integrability(name):
-    """Is this an integrability dataset?
-    The decision is based on the existence of `integrability.yaml`"""
+    """Determine whether this is an integrability dataset.
+
+    The decision is based on the existence of `integrability.yaml`.
+
+    """
     return (configs.configs["paths"]["runcards"] / name / _RUNCARD).exists()
 
 
 def evolution_to_flavour(evol_fl):
-    """Uses eko to transform an evolution pid (>100) to flavour basis
-    in a pineappl-usable way (flavour, weight)
-    """
+    """Use eko to transform an evolution pid (>100) to flavour basis in a pineappl-usable way (flavour, weight)."""
     if evol_fl < 100:
         return [(evol_fl, 1.0)]
     idx = br.evol_basis_pids.index(evol_fl)
     row = br.rotate_flavor_to_evolution[idx]
     lumis = []
     for i, w in enumerate(row):
         if w != 0.0:
@@ -44,28 +45,31 @@
     xgrid: typing.List[float]
 
     def asdict(self):
         return dataclasses.asdict(self)
 
 
 class Integrability(interface.External):
+    """Interface provider."""
+
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         input_card = self.source / _RUNCARD
         yaml_dict = yaml.safe_load(input_card.open("r", encoding="utf-8"))
         self._q2 = np.power(self.theory["Q0"], 2)
         self._info = _IntegrabilityRuncard(**yaml_dict)
         self._evo2fl = evolution_to_flavour(self._info.flavour)
 
     def run(self):
+        """Empty function."""
         pass
 
     def generate_pineappl(self):
-        """Generate the pineappl grid for the integrability observable"""
+        """Generate the pineappl grid for the integrability observable."""
         ## Generate the grid
         lumi_entries = [(fl, self._info.lepton_pid, w) for fl, w in self._evo2fl]
         luminosities = [pineappl.lumi.LumiEntry(lumi_entries)]
         # Set default parameters
         orders = [pineappl.grid.Order(0, 0, 0, 0)]
         params = pineappl.subgrid.SubgridParams()
         # Initialize and parametrize grid
@@ -79,17 +83,21 @@
         x = self._info.xgrid
         w = np.array(x).reshape((1, -1, 1))
         sg = pineappl.import_only_subgrid.ImportOnlySubgridV1(w, [self._q2], x, x)
         grid.set_subgrid(0, 0, 0, sg)
         grid.write(self.grid)
 
     def collect_versions(self):
+        """Add the version defined by this file."""
         return {"integrability_version": "1.0"}
 
     def results(self):
+        """Apply PDF to grid."""
+        import lhapdf  # pylint: disable=import-error
+
         pdf = lhapdf.mkPDF(self.pdf)
         final_result = 0.0
         q2 = self._q2 * np.ones_like(self._info.xgrid)
 
         for fl, w in self._evo2fl:
             final_result += w * np.sum(pdf.xfxQ2(fl, self._info.xgrid, q2))
         final_cv = [final_result]
```

### Comparing `pinefarm-0.2.2/src/pinefarm/external/interface.py` & `pinefarm-0.3.0/src/pinefarm/external/interface.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,34 @@
+"""Abstract interface."""
 import abc
+import base64
 import os
+import pathlib
 import shutil
 import subprocess
+import tempfile
 
-import pygit2
+import pineappl
 
 from .. import __version__, configs, tools
 
 
 class External(abc.ABC):
-    """
-    Interface class for external providers.
+    """Interface class for external providers.
 
     Parameters
     ----------
-        name : str
-            dataset name
-        theory : dict
-            theory dictionary
-        pdf : str
-            PDF name
-        timestamp : str
-            timestamp of already generated output folder
+    name : str
+        dataset name
+    theory : dict
+        theory dictionary
+    pdf : str
+        PDF name
+    timestamp : str
+        timestamp of already generated output folder
 
     """
 
     def __init__(self, name, theory, pdf, timestamp=None):
         self.name = name
         self.theory = theory
         self.pdf = pdf
@@ -53,15 +56,15 @@
     @property
     def gridtmp(self):
         """Intermediate PineAPPL grid name."""
         return self.dest / f"{self.name}.pineappl.tmp"
 
     def update_with_tmp(self):
         """Move intermediate grid to final position."""
-        shutil.move(self.gridtmp, self.grid)
+        shutil.move(str(self.gridtmp), str(self.grid))
 
     @staticmethod
     def install():
         """Install all needed programs."""
 
     @abc.abstractmethod
     def run(self):
@@ -99,33 +102,33 @@
         -------
         dict
             program - version mapping related to programs specific to a single
             runner (common ones are already abstracted)
 
         """
 
+    def load_pinecard(self) -> str:
+        """Load directory as b64encoded .tar.gz file."""
+        # shutils wants to create a true file, so we go through a temp dir
+        with tempfile.TemporaryDirectory() as tmpdirname:
+            p = pathlib.Path(tmpdirname) / "pinecard"
+            shutil.make_archive(p, format="gztar", root_dir=self.source)
+            with open(p.with_suffix(".tar.gz"), "rb") as fd:
+                return base64.b64encode(fd.read()).decode("ascii")
+
     def annotate_versions(self):
         """Add version informations as meta data."""
         results_log = self.dest / "results.log"
 
         versions = self.collect_versions()
         # the pinefarm version will also pin pineappl_py version and all the
         # other python dependencies versions
         versions["pinefarm"] = __version__
-        versions["pinecard"] = pygit2.Repository(
-            configs.configs["paths"]["root"]
-        ).describe(
-            always_use_long_format=True,
-            describe_strategy=pygit2.GIT_DESCRIBE_TAGS,
-            dirty_suffix="-dirty",
-            show_commit_oid_as_fallback=True,
-        )
-        # TODO: add pineappl version
-        #  pineappl = configs.configs["commands"]["pineappl"]()
-        versions["pineappl_capi"] = "???"
+        versions["pinecard"] = self.load_pinecard()
+        versions["pineappl"] = pineappl.__version__
 
         entries = {}
         entries.update(versions)
         entries["lumi_id_types"] = "pdg_mc_ids"
         entries["results_pdf"] = self.pdf
         tools.update_grid_metadata(
             self.grid, self.gridtmp, entries, {"results": results_log}
```

### Comparing `pinefarm-0.2.2/src/pinefarm/external/mg5/__init__.py` & `pinefarm-0.3.0/src/pinefarm/external/mg5/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
+"""Madgraph interface."""
 import json
 import re
 import subprocess
 
-import lhapdf
 import numpy as np
 import pandas as pd
 import pineappl
 
 from ... import configs, install, log, tools
 from .. import interface
 from . import paths
 
 URL = "https://launchpad.net/mg5amcnlo/{major}.0/{major}.{minor}.x/+download/MG5_aMC_v{version}.tar.gz"
 "URL template for MG5aMC\\@NLO release"
-VERSION = "3.4.1"
+VERSION = "3.4.2"
 "Version in use"
 CONVERT_MODEL = """
 set auto_convert_model True
 import model loop_qcd_qed_sm_Gmu
 quit
 """
 "Instructions to set the correct model for MG5aMC\\@NLO."
@@ -26,35 +26,43 @@
 def url():
     """Compute actual download URL."""
     major, minor, _ = VERSION.split(".")
     return URL.format(version=VERSION, major=major, minor=minor)
 
 
 class Mg5(interface.External):
+    """Interface provider."""
+
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self.user_cuts = []
         self.patches = []
         self.tau_min = None
 
     @property
     def mg5_dir(self):
+        """Return output dir."""
         return self.dest / self.name
 
     @staticmethod
     def install():
+        """Execute installer."""
         install.pineappl()
         install.mg5amc()
 
     @property
     def pdf_id(self):
+        """Convert PDF to SetIndex."""
+        import lhapdf  # pylint: disable=import-error
+
         return lhapdf.mkPDF(self.pdf).info().get_entry("SetIndex")
 
     def run(self):
+        """Execute program."""
         # copy the output file to the directory and replace the variables
         output = (self.source / "output.txt").read_text().replace("@OUTPUT@", self.name)
         output_file = self.dest / "output.txt"
         output_file.write_text(output)
 
         # create output folder
         log.subprocess(
@@ -157,14 +165,15 @@
         log.subprocess(
             [str(configs.configs["commands"]["mg5"]), str(launch_file)],
             cwd=self.dest,
             out=self.dest / "launch.log",
         )
 
     def generate_pineappl(self):
+        """Generate grid."""
         # if rerunning without regenerating, let's remove the already merged
         # grid (it will be soon reobtained)
         if self.timestamp is not None:
             self.grid.unlink()
 
         # merge the final bins
         mg5_grids = sorted(
@@ -196,14 +205,15 @@
         grid.set_key_value(
             "user_cuts", "\n".join(f"{var}={value}" for var, value in self.user_cuts)
         )
 
         grid.write(str(self.grid))
 
     def results(self):
+        """Collect PDF results."""
         madatnlo = next(
             iter(self.mg5_dir.glob("Events/run_01*/MADatNLO.HwU"))
         ).read_text()
         table = filter(
             lambda line: re.match("^  [+-]", line) is not None, madatnlo.splitlines()
         )
         df = pd.DataFrame(
@@ -215,14 +225,15 @@
         df["error"] = df[4]
         df["sv_min"] = df[6]
         df["sv_max"] = df[7]
 
         return df
 
     def collect_versions(self):
+        """Add versions."""
         versions = {}
         versions["mg5amc_revno"] = (
             subprocess.run(
                 "brz revno".split(),
                 cwd=configs.configs["paths"]["mg5amc"],
                 stdout=subprocess.PIPE,
             )
@@ -243,14 +254,15 @@
         if repo is None:
             print("Invalid mg5 repository")
         versions["mg5amc_repo"] = repo[1] if repo is not None else None
         return versions
 
 
 def find_marker_position(insertion_marker, contents):
+    """Find in file."""
     marker_pos = -1
 
     for lineno, value in enumerate(contents):
         if insertion_marker in value:
             marker_pos = lineno
             break
 
@@ -259,15 +271,15 @@
             "Error: could not find insertion marker `{insertion_marker}` in cut file `{file_path}`"
         )
 
     return marker_pos
 
 
 def apply_user_cuts(cuts_file, user_cuts):
-    """Apply a user defined cut, patching a suitable cuts file"""
+    """Apply a user defined cut, patching a suitable cuts file."""
     with open(cuts_file) as fd:
         contents = fd.readlines()
 
     # insert variable declaration
     marker_pos = find_marker_position("logical function passcuts_user", contents)
     marker_pos = marker_pos + 8
```

### Comparing `pinefarm-0.2.2/src/pinefarm/external/mg5/cuts_code/abscoscsmax.f` & `pinefarm-0.3.0/src/pinefarm/external/mg5/cuts_code/abscoscsmax.f`

 * *Files identical despite different names*

### Comparing `pinefarm-0.2.2/src/pinefarm/external/mg5/cuts_code/abscoscsmin.f` & `pinefarm-0.3.0/src/pinefarm/external/mg5/cuts_code/abscoscsmin.f`

 * *Files identical despite different names*

### Comparing `pinefarm-0.2.2/src/pinefarm/external/mg5/cuts_code/atlas_1jet_8tev_r06.f` & `pinefarm-0.3.0/src/pinefarm/external/mg5/cuts_code/atlas_1jet_8tev_r06.f`

 * *Files identical despite different names*

### Comparing `pinefarm-0.2.2/src/pinefarm/external/mg5/cuts_code/atlas_2jet_7tev_r06_0510.f` & `pinefarm-0.3.0/src/pinefarm/external/mg5/cuts_code/atlas_2jet_7tev_r06_0510.f`

 * *Files identical despite different names*

### Comparing `pinefarm-0.2.2/src/pinefarm/external/mg5/cuts_code/atlas_2jet_7tev_r06_1015.f` & `pinefarm-0.3.0/src/pinefarm/external/mg5/cuts_code/atlas_2jet_7tev_r06_1015.f`

 * *Files identical despite different names*

### Comparing `pinefarm-0.2.2/src/pinefarm/external/mg5/cuts_code/atlas_2jet_7tev_r06_1520.f` & `pinefarm-0.3.0/src/pinefarm/external/mg5/cuts_code/atlas_2jet_7tev_r06_1520.f`

 * *Files identical despite different names*

### Comparing `pinefarm-0.2.2/src/pinefarm/external/mg5/cuts_code/atlas_2jet_7tev_r06_2025.f` & `pinefarm-0.3.0/src/pinefarm/external/mg5/cuts_code/atlas_2jet_7tev_r06_2025.f`

 * *Files identical despite different names*

### Comparing `pinefarm-0.2.2/src/pinefarm/external/mg5/cuts_code/atlas_2jet_7tev_r06_2530.f` & `pinefarm-0.3.0/src/pinefarm/external/mg5/cuts_code/atlas_2jet_7tev_r06_2530.f`

 * *Files identical despite different names*

### Comparing `pinefarm-0.2.2/src/pinefarm/external/mg5/cuts_code/atlas_dy3d_8tev.f` & `pinefarm-0.3.0/src/pinefarm/external/mg5/cuts_code/atlas_dy3d_8tev.f`

 * *Files identical despite different names*

### Comparing `pinefarm-0.2.2/src/pinefarm/external/mg5/cuts_code/atlas_wzrap11_cf.f` & `pinefarm-0.3.0/src/pinefarm/external/mg5/cuts_code/atlas_wzrap11_cf.f`

 * *Files identical despite different names*

### Comparing `pinefarm-0.2.2/src/pinefarm/external/mg5/cuts_code/cms_2jet_3d_8tev.f` & `pinefarm-0.3.0/src/pinefarm/external/mg5/cuts_code/cms_2jet_3d_8tev.f`

 * *Files identical despite different names*

### Comparing `pinefarm-0.2.2/src/pinefarm/external/mg5/cuts_code/cms_2jets_7tev_0510.f` & `pinefarm-0.3.0/src/pinefarm/external/mg5/cuts_code/cms_2jets_7tev_0510.f`

 * *Files identical despite different names*

### Comparing `pinefarm-0.2.2/src/pinefarm/external/mg5/cuts_code/cms_2jets_7tev_1015.f` & `pinefarm-0.3.0/src/pinefarm/external/mg5/cuts_code/cms_2jets_7tev_1015.f`

 * *Files identical despite different names*

### Comparing `pinefarm-0.2.2/src/pinefarm/external/mg5/cuts_code/cms_2jets_7tev_1520.f` & `pinefarm-0.3.0/src/pinefarm/external/mg5/cuts_code/cms_2jets_7tev_1520.f`

 * *Files identical despite different names*

### Comparing `pinefarm-0.2.2/src/pinefarm/external/mg5/cuts_code/cms_2jets_7tev_2025.f` & `pinefarm-0.3.0/src/pinefarm/external/mg5/cuts_code/cms_2jets_7tev_2025.f`

 * *Files identical despite different names*

### Comparing `pinefarm-0.2.2/src/pinefarm/external/mg5/cuts_code/mtw.f` & `pinefarm-0.3.0/src/pinefarm/external/mg5/cuts_code/mtw.f`

 * *Files identical despite different names*

### Comparing `pinefarm-0.2.2/src/pinefarm/external/mg5/cuts_code/yll.f` & `pinefarm-0.3.0/src/pinefarm/external/mg5/cuts_code/yll.f`

 * *Files identical despite different names*

### Comparing `pinefarm-0.2.2/src/pinefarm/external/mg5/patches/change_etaj_to_rapj.patch` & `pinefarm-0.3.0/src/pinefarm/external/mg5/patches/change_etaj_to_rapj.patch`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 --- NLO/SubProcesses/fastjetfortran_madfks_core.cc.orig	2020-11-27 18:11:04.027146365 +0100
 +++ NLO/SubProcesses/fastjetfortran_madfks_core.cc	2020-11-27 18:13:47.285826142 +0100
 @@ -76,7 +76,7 @@
    /// and the extraction of the jets
-   void amcatnlo_transfer_cluster_transfer(const double * p, const int & npart, 
+   void amcatnlo_transfer_cluster_transfer(const double * p, const int & npart,
                                   const JetDefinition & jet_def,
 -                                 const double & ptmin, const double & etamax,
 +                                 const double & ptmin, const double & rapmax,
  				 double * f77jets, int & njets, int * whichjet) {
- 
+
      // transfer p[4*ipart+0..3] -> input_particles[i]
 @@ -90,9 +90,9 @@
      jets = sorted_by_pt(cs->inclusive_jets(ptmin));
- 
+
      //apply the eta selector if etamax >0
 -    Selector select_eta = SelectorAbsEtaMax(etamax);
 -    if (etamax > 0.) {
 -        jets = select_eta(jets);
 +    Selector select_rap = SelectorAbsRapMax(rapmax);
 +    if (rapmax > 0.) {
 +        jets = select_rap(jets);
      }
- 
+
      // transfer jets -> f77jets[4*ijet+0..3]
 --- NLO/SubProcesses/fastjetfortran_madfks_full.cc.orig	2020-11-27 18:11:12.687075955 +0100
 +++ NLO/SubProcesses/fastjetfortran_madfks_full.cc	2020-11-27 18:13:47.289826110 +0100
 @@ -79,7 +79,7 @@
    /// and the extraction of the jets
-   void amcatnlo_transfer_cluster_transfer(const double * p, const int & npart, 
+   void amcatnlo_transfer_cluster_transfer(const double * p, const int & npart,
                                   const JetDefinition & jet_def,
 -                                 const double & ptmin, const double & etamax,
 +                                 const double & ptmin, const double & rapmax,
  				 double * f77jets, int & njets, int * whichjet,
- 				 const double & ghost_maxrap = 0.0,  
+ 				 const double & ghost_maxrap = 0.0,
  				 const int & nrepeat = 0, const double & ghost_area = 0.0) {
 @@ -101,9 +101,9 @@
      jets = sorted_by_pt(cs->inclusive_jets(ptmin));
- 
+
      //apply the eta selector if etamax >0
 -    Selector select_eta = SelectorAbsEtaMax(etamax);
 -    if (etamax > 0.) {
 -        jets = select_eta(jets);
 +    Selector select_rap = SelectorAbsRapMax(rapmax);
 +    if (rapmax > 0.) {
 +        jets = select_rap(jets);
      }
- 
+
      // transfer jets -> f77jets[4*ijet+0..3]
```

### Comparing `pinefarm-0.2.2/src/pinefarm/external/mg5/patches/set_tau_min.patch` & `pinefarm-0.3.0/src/pinefarm/external/mg5/patches/set_tau_min.patch`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
 -                     ! compare with the update from pt cut
 -                     if (smin_update.lt.nb_iden_pdg**2*(etmin(i)**2 + emass(i)**2))then
 -                        ! the pt is more restrictive
 -                        smin_update = dsqrt(etmin(i)**2 + emass(i)**2)
 -                     else
 -                        smin_update = dsqrt(smin_update)/nb_iden_pdg ! share over N particle, and change dimension
 -                     endif
--                     ! update in sqrt(s) so take the 
+-                     ! update in sqrt(s) so take the
 -                     if  (j_fks.gt.nincoming) then
 -                        taumin(iFKS,ichan)=taumin(iFKS,ichan) + smin_update
 -                     else
 -                        taumin(iFKS,ichan)=taumin(iFKS,ichan) + emass(i)
 -                     endif
 -                     taumin_s(iFKS,ichan)=taumin_s(iFKS,ichan) + smin_update
 -                     taumin_j(iFKS,ichan)=taumin_j(iFKS,ichan) + smin_update
```

### Comparing `pinefarm-0.2.2/src/pinefarm/external/positivity.py` & `pinefarm-0.3.0/src/pinefarm/external/positivity.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,39 @@
+"""Positivity interface."""
 import json
 
-import lhapdf
 import numpy as np
 import pandas as pd
 import pineappl
 import yaml
 
 from .. import configs
 from . import interface
 
 
-def is_positivity(name):
-    """
-    Is this a positivity dataset?
-
-    The decision is based on the existance of the `positivity.yaml` file.
-
-    Parameters
-    ----------
-        name : str
-            dataset name
-    """
+def is_positivity(name: str) -> bool:
+    """Determine whether this a positivity dataset."""
     return (configs.configs["paths"]["runcards"] / name / "positivity.yaml").exists()
 
 
 class Positivity(interface.External):
+    """Interface provider."""
+
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def run(self):
+        """Open configuration."""
         with open(
             configs.configs["paths"]["runcards"] / self.name / "positivity.yaml"
         ) as o:
             self.runcard = yaml.safe_load(o)
 
     def generate_pineappl(self):
+        """Generate grid."""
         self.xgrid = self.runcard["xgrid"]
         self.lepton_pid = self.runcard["lepton_pid"]
         self.pid = self.runcard["pid"]
         self.q2 = self.runcard["q2"]
         self.hadron_pid = self.runcard["hadron_pid"]
 
         # init pineappl objects
@@ -77,14 +72,17 @@
         grid.set_key_value("initial_state_2", str(self.lepton_pid))
         grid.set_key_value("runcard", json.dumps(self.runcard))
         grid.set_key_value("lumi_id_types", "pdg_mc_ids")
         grid.optimize()
         grid.write(str(self.grid))
 
     def results(self):
+        """Apply PDF to grid."""
+        import lhapdf  # pylint: disable=import-error
+
         pdf = lhapdf.mkPDF(self.pdf)
         d = {
             "result": [pdf.xfxQ2(self.pid, x, self.q2) for x in self.xgrid],
             "error": [1e-15] * len(self.xgrid),
             "sv_min": [
                 np.amin(
                     [
@@ -107,8 +105,9 @@
             ],
         }
         results = pd.DataFrame(data=d)
 
         return results
 
     def collect_versions(self):
+        """No additional programs involved."""
         return {}
```

### Comparing `pinefarm-0.2.2/src/pinefarm/external/vrap.py` & `pinefarm-0.3.0/src/pinefarm/external/vrap.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-"""
-    Runner for vrap producing pineappl grids
+"""Runner for vrap producing pineappl grids.
 
-    Uses a modified version of vrap https://github.com/NNPDF/hawaiian_vrap
-    which produces pineappl grids. It has been tested for FT DY kinematics
+Uses a modified version of vrap https://github.com/NNPDF/hawaiian_vrap
+which produces pineappl grids. It has been tested for FT DY kinematics
 
-    A ``vrap`` dataset includes a single ``vrap.yaml`` file which defines
-    how ``vrap`` will be run.
-    A dataset can include many kinematic files (min. 1), ``vrap`` will be run
-    once per kinematic file.
-    Vrap datatasets can also include ``cfactors`` which need to match the name
-    of the kinematic files and will be applied to the corresponding run
-    ex: if the kinematic file is call "906_bin0.dat" the corresponding cfactors
-        are "ACC_906_bin0.dat" and "QCD_906_bin0.dat"
+A ``vrap`` dataset includes a single ``vrap.yaml`` file which defines
+how ``vrap`` will be run.
+A dataset can include many kinematic files (min. 1), ``vrap`` will be run
+once per kinematic file.
+Vrap datatasets can also include ``cfactors`` which need to match the name
+of the kinematic files and will be applied to the corresponding run
+ex: if the kinematic file is call "906_bin0.dat" the corresponding cfactors
+    are "ACC_906_bin0.dat" and "QCD_906_bin0.dat"
 """
 import subprocess as sp
 import tempfile
 import warnings
 
 import numpy as np
 import pandas as pd
@@ -33,25 +32,21 @@
 _POSITIVITY_PDFS = {
     "pos_ddb": [1, -1, 21],
     "pos_uub": [2, -2, 21],
     "pos_ssb": [3, -3, 21],
 }
 
 
-def is_vrap(name):
-    """
-    Checks whether this is a dataset to be run with vrap
-    """
+def is_vrap(name: str) -> bool:
+    """Check whether this is a dataset to be run with vrap."""
     return (configs.configs["paths"]["runcards"] / name / "vrap.yaml").exists()
 
 
 def yaml_to_vrapcard(yaml_dict, pdf, output_file, order="NLO"):
-    """
-    Converts the dictionary from `vrap.yaml` file into a vrap runcard
-    """
+    """Convert the dictionary from `vrap.yaml` file into a vrap runcard."""
     input_yaml = dict(yaml_dict)
     # Load the run-specific options
     input_yaml["PDFfile"] = f"{pdf}.LHgrid"
     # Remove possible spurious options
     if "positivity_pdf" in input_yaml:
         input_yaml.pop("positivity_pdf")
 
@@ -59,24 +54,24 @@
     input_yaml["Order"] = order
 
     as_lines = [f"{k} {v}" for k, v in input_yaml.items()]
     output_file.write_text("\n".join(as_lines))
 
 
 def gen_pos_pdf(pdfname, base_pdf="NNPDF40_nnlo_as_01180"):
-    """
-    Generate ``pdfname`` according to the rules in _POSITIVITY_PDFS
-    """
+    """Generate ``pdfname`` according to the rules in _POSITIVITY_PDFS."""
     # If the pdfname does not exist, generate it
     if not (environment.datapath / pdfname).exists():
         pdflabels = _POSITIVITY_PDFS[pdfname]
         genpdf.generate_pdf(pdfname, pdflabels, install=True, parent_pdf_set=base_pdf)
 
 
 class Vrap(interface.External):
+    """Interface provider."""
+
     def __init__(self, pinecard, theorycard, *args, **kwargs):
         super().__init__(pinecard, theorycard, *args, **kwargs)
 
         order = theorycard.get("PTO")
         if order == 0:
             vrap_order = "LO"
         elif order == 1:
@@ -127,18 +122,20 @@
 
         yaml_to_vrapcard(yaml_dict, self.pdf, self._input_card, order=vrap_order)
 
         self._partial_grids = []
         self._partial_results = []
 
     def run(self):
-        """Run vrap for the given runcards
+        """Run vrap for the given runcards.
+
         After running vrap, the resulting grid will be optimized, cfactors
         (for instance, ACCEPTANCE factors) applied.
-        The MC results for each run (writen to results.out) will be read
+        The MC results for each run (writen to results.out) will be read.
+
         """
         for b, kin_card in enumerate(self._kin_cards):
             sp.run(
                 [configs.configs["commands"]["vrap"], self._input_card, kin_card],
                 cwd=self.dest,
                 check=True,
             )
@@ -171,15 +168,15 @@
 
             self._partial_grids.append(pinename)
 
             # Apply cfactors if needed
             self._partial_results.append((cv, stat))
 
     def generate_pineappl(self):
-        """If the run contain more than one grid, merge them all"""
+        """If the run contain more than one grid, merge them all."""
         if len(self._partial_grids) > 1:
             # Use the first subgrid as main grid
             main_grid = Grid.read(self._partial_grids[0].as_posix())
             n = len(main_grid.bin_left(0))
             rebin = BinRemapper(np.ones(n), [(i, i) for i in range(n)])
             main_grid.set_remapper(rebin)
             with tempfile.TemporaryDirectory() as tmp:
@@ -189,36 +186,35 @@
                     tmp_grid.set_remapper(rebin)
                     tmp_grid.write(tmp_output)
                     # Now merge it into the main grid!
                     main_grid.merge_from_file(tmp_output)
             main_grid.write(self.grid)
 
     def results(self):
-        """Combines the results of the partial runs of vrap
-        in order to compare with the generated grid
-        """
+        """Combinesthe results of the partial runs of vrap in order to compare with the generated grid."""
         cv, stat_errors = zip(*self._partial_results)
         final_cv = np.sum(cv, axis=0)
         final_stat = np.sqrt(np.sum(np.power(stat_errors, 2), axis=0))
 
         d = {
             "result": final_cv,
             "error": final_stat,
             "sv_min": np.zeros_like(final_cv),
             "sv_max": np.zeros_like(final_cv),
         }
 
         return pd.DataFrame(data=d)
 
     def collect_versions(self):
-        """Currently the version is defined by this file"""
+        """Add the version defined by this file."""
         vrap_run = sp.run(
             [configs.configs["commands"]["vrap"], "--version"],
             capture_output=True,
             check=True,
         )
         vrap_version = vrap_run.stdout.decode().split()[-1]
         return {"vrap_version": vrap_version}
 
     @staticmethod
     def install():
+        """Execute installer."""
         install.hawaiian_vrap()
```

### Comparing `pinefarm-0.2.2/src/pinefarm/external/yad.py` & `pinefarm-0.3.0/src/pinefarm/external/yad.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,32 @@
+"""yadism interface."""
 from functools import reduce
 
-import lhapdf
 import pandas as pd
 import yadbox.export
 import yadism
 import yadism.output
 import yaml
 
 from .. import configs, log, tools
 from . import interface
 
 
-def is_dis(name):
-    """
-    Is this a DIS dataset, i.e. is yadism needed to run?
+def is_dis(name: str) -> bool:
+    """Determine whether this is a DIS dataset, i.e. is yadism needed to run.
 
     The decision is based on the existance of the `observable.yaml` file.
 
-    Parameters
-    ----------
-        name : str
-            dataset name
     """
     return (configs.configs["paths"]["runcards"] / name / "observable.yaml").exists()
 
 
 class Yadism(interface.External):
+    """Interface provider."""
+
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         # load runcards
         with open(
             configs.configs["paths"]["runcards"] / self.name / "observable.yaml"
         ) as o:
@@ -38,37 +35,43 @@
         # deactivate TMC for positivity observables
         # (see also minutes of 2022-07-29)
         if self.obs["NCPositivityCharge"] is not None:
             self.theory["TMC"] = 0
 
     @property
     def output(self):
+        """Return yadism output path."""
         return self.grid.with_suffix(".tar")
 
     def run(self):
+        """Run program."""
         print("Running yadism...")
 
         # run yadism
         run_log = self.dest / "run.log"
         with log.Tee(run_log, stderr=True):
             try:
                 out = yadism.run_yadism(self.theory, self.obs)
             except Exception:
                 raise log.WhileRedirectedError(file=run_log)
 
         # dump output
         out.dump_tar(self.output)
 
     def generate_pineappl(self):
+        """Generate grid."""
         out = yadism.output.Output.load_tar(self.output)
         yadbox.export.dump_pineappl_to_file(
             out, str(self.grid), next(iter(self.obs["observables"].keys()))
         )
 
     def results(self):
+        """Apply PDF to output."""
+        import lhapdf  # pylint: disable=import-error
+
         pdf = lhapdf.mkPDF(self.pdf)
         out = yadism.output.Output.load_tar(self.output)
         pdf_out = out.apply_pdf_alphas_alphaqed_xir_xif(
             pdf,
             lambda muR: lhapdf.mkAlphaS(self.pdf).alphasQ(muR),
             lambda _muR: 0,
             1.0,
@@ -111,8 +114,9 @@
         ]
         pdf_out["sv_max"] = svdf.max(axis=1)
         pdf_out["sv_min"] = svdf.min(axis=1)
 
         return pdf_out
 
     def collect_versions(self):
+        """No additional programs involved."""
         return {}
```

### Comparing `pinefarm-0.2.2/src/pinefarm/info.py` & `pinefarm-0.3.0/src/pinefarm/info.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,36 @@
+"""Provide inspection tools."""
 import dataclasses
 import enum
 import typing
 
 from .external import integrability, interface, mg5, positivity, vrap, yad
 
 
 class Kind(enum.Enum):
+    """Interface types."""
+
     dis = enum.auto()
     positivity = enum.auto()
     ftdy = enum.auto()
     hadronic = enum.auto()
     integrability = enum.auto()
 
 
 @dataclasses.dataclass
 class Info:
+    """Info type."""
+
     color: str
     external: typing.Type[interface.External]
     kind: Kind
 
 
 def label(dataset: str) -> Info:
+    """Generate associated Info type."""
     if yad.is_dis(dataset):
         return Info(color="red", external=yad.Yadism, kind=Kind.dis)
     if positivity.is_positivity(dataset):
         return Info(
             color="yellow", external=positivity.Positivity, kind=Kind.positivity
         )
     if vrap.is_vrap(dataset):
```

### Comparing `pinefarm-0.2.2/src/pinefarm/install.py` & `pinefarm-0.3.0/src/pinefarm/install.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Install tools."""
 import os
 import pathlib
 import shutil
 import subprocess
 import sys
 import tarfile
 import tempfile
@@ -18,27 +19,28 @@
 "Git repo location for pineappl."
 
 LHAPDF_VERSION = "LHAPDF-6.4.0"
 "Version of LHAPDF to be used by default (if not already available)."
 
 
 def init_prefix():
+    """Set up paths."""
     configs.configs["paths"]["prefix"].mkdir(exist_ok=True)
     configs.configs["paths"]["bin"].mkdir(exist_ok=True)
     configs.configs["paths"]["lib"].mkdir(exist_ok=True)
 
 
 def is_exe(command: os.PathLike) -> bool:
     """Check if given path exists and is executable."""
     command = pathlib.Path(command)
     return command.exists() and os.access(command, os.X_OK)
 
 
 def mg5amc():
-    """Initialize `MadGraph5_aMC\\@NLO <https://code.launchpad.net/mg5amcnlo>`_.
+    r"""Initialize `MadGraph5_aMC\@NLO <https://code.launchpad.net/mg5amcnlo>`_.
 
     Returns
     -------
     bool
         whether the main executable is now existing.
 
     """
@@ -68,32 +70,32 @@
         shutil.rmtree(tmpdir)
 
     # check if the archive was wrapping a single folder
     content = list(dest.iterdir())
     if len(content) == 1:
         # in case, remove the intermediate layer
         for el in content[0].iterdir():
-            shutil.move(el, dest)
+            shutil.move(str(el), str(dest))
         content[0].rmdir()
 
     # in case we're using python3, we need to convert the model file
     subprocess.run(f"{mg5_exe}", input=mg5.CONVERT_MODEL, encoding="ascii")
 
     # retest availability
     return is_exe(mg5_exe)
 
 
 def hawaiian_vrap():
-    """Install a version of vrap flavoured with pineappl
-    from https://github.com/NNPDF/hawaiian_vrap
+    """Install a version of vrap flavoured with pineappl from https://github.com/NNPDF/hawaiian_vrap.
 
     Returns
     -------
     bool
         whether vrap is now installed
+
     """
     # Ensure that pineappl and lhapdf are installed
     _ = lhapdf()
     _ = pineappl(capi=True)
 
     vrapx = configs.configs["commands"]["vrap"]
 
@@ -125,16 +127,15 @@
         )
         subprocess.run(["make", "install"], cwd=build_dir, check=True)
 
     return is_exe(vrapx)
 
 
 def cargo():
-    """Initialize `Rust <https://www.rust-lang.org/>`_ and `Cargo
-    <https://doc.rust-lang.org/stable/cargo/>`_.
+    """Initialize `Rust <https://www.rust-lang.org/>`_ and `Cargo <https://doc.rust-lang.org/stable/cargo/>`_.
 
     Returns
     -------
     str
         path to `cargo`
 
     """
@@ -178,16 +179,17 @@
 
     Returns
     -------
     bool
         whether `pineappl` and  `pineappl_capi` are now available.
 
     """
-    # define availability condition
+
     def installed():
+        """Define availability condition."""
         return pkgconfig.exists("pineappl_capi")
 
     def cli_installed():
         return shutil.which("pineappl") is not None
 
     # check if there is something to do at all
     if (not capi or installed()) and (not cli or cli_installed()):
@@ -231,16 +233,15 @@
         configs.configs["commands"]["pineappl"] = shutil.which("pineappl")
 
     # retest availability
     return installed() and (not cli or cli_installed())
 
 
 def update_lhapdf_path(path):
-    """Update LHAPDF path, both in environment and `lhapdf_management
-    <https://pypi.org/project/lhapdf-management/>`_
+    """Update LHAPDF path, both in environment and `lhapdf_management <https://pypi.org/project/lhapdf-management/>`_.
 
     Parameters
     ----------
     path : str or pathlib.Path
         path to LHAPDF data
 
     """
@@ -290,16 +291,17 @@
 def lhapdf():
     """Install `LHAPDF <https://lhapdf.hepforge.org/>`_ C++ library.
 
     Not needed:
         - for `mg5`, since it's vendored
         - for `yadism`, since we depend on the PyPI version
     """
-    # define availability condition
+
     def installed():
+        """Define availability condition."""
         try:
             # test python package availability
             import lhapdf  # pylint: disable=unused-import
         except ModuleNotFoundError:
             return False
         return pkgconfig.exists("lhapdf")
 
@@ -316,15 +318,14 @@
     with requests.get(
         f"https://lhapdf.hepforge.org/downloads/?f={lhapdf_tar.name}"
     ) as r:
         with open(lhapdf_tar, "wb") as f:
             f.write(r.content)
 
     with tarfile.open(lhapdf_tar, "r:gz") as tar:
-
         tar.extractall(lhapdf_dest)
 
     env = os.environ.copy()
     env["PYTHON"] = sys.executable
     subprocess.run(
         f"./configure --prefix={configs.configs['paths']['prefix']}".split(),
         env=env,
```

### Comparing `pinefarm-0.2.2/src/pinefarm/log.py` & `pinefarm-0.3.0/src/pinefarm/log.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+"""Logging tools."""
 import pathlib
 import subprocess as sp
 import sys
 
 
 class WhileRedirectedError(RuntimeError):
-    """Error to signal a generic error, while stderr was redirected to file
+    """Error to signal a generic error, while stderr was redirected to file.
 
     Parameters
     ----------
     *args
         arguments passed to :class:`RuntimeError`
     file : str
         path to file to which stderr is redirected
@@ -19,28 +20,31 @@
 
     def __init__(self, *args, file, **kwargs):
         super().__init__(*args, **kwargs)
         self.file = file.absolute() if isinstance(file, pathlib.Path) else file
 
 
 class ChildStream:
+    """Inner stream."""
+
     def __init__(self, parent):
         self.parent = parent
 
     def write(self, data):
+        """Write to stream."""
         self.parent.write(data, self)
 
     def __getattribute__(self, name):
         if name[0] != "_" and name not in ["parent", "write"]:
             return super().__getattribute__("parent").__getattribute__(name)
         return super().__getattribute__(name)
 
 
 class Tee:
-    """Context manager to tee stdout to file
+    """Context manager to tee stdout to file.
 
     Parameters
     ----------
     name : str or pathlib.Path
         path to redirect stdout to
 
     """
@@ -65,21 +69,23 @@
             )
         sys.stdout = self.stdout_bk
         sys.stderr = self.stderr_bk
         self.file.flush()
         self.file.close()
 
     def write(self, data, stream):
+        """Write to stream."""
         self.file.write(data)
         if stream is self.stdout:
             self.stdout_bk.write(data)
         elif stream is self.stderr:
             self.stderr_bk.write(data)
 
     def flush(self):
+        """Flush stream."""
         self.file.flush()
 
     def __getattribute__(self, name):
         if name[0] != "_" and name not in [
             "file",
             "stdout",
             "stderr",
@@ -88,15 +94,15 @@
             "write",
         ]:
             return super().__getattribute__("file").__getattribute__(name)
         return super().__getattribute__(name)
 
 
 def subprocess(*args, cwd, out):
-    """Wrapper to :class:`subprocess.Popen` to print the output to screen and capture it.
+    """Wrap :class:`subprocess.Popen` to print the output to screen and capture it.
 
     Parameters
     ----------
     args
         positional arguments to pass to `subprocess.Popen`
     cwd : path-like or str
         directory where to execute the command
```

### Comparing `pinefarm-0.2.2/src/pinefarm/table.py` & `pinefarm-0.3.0/src/pinefarm/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
+"""Comparison tools."""
 import inspect
-import itertools
 
-import lhapdf
 import more_itertools
 import pandas as pd
 import pineappl
 
 from . import tools
 
 
@@ -23,14 +22,16 @@
 
     Returns
     -------
     list(str)
         (essential) output splitted by line
 
     """
+    import lhapdf  # pylint: disable=import-error
+
     pdf = lhapdf.mkPDF(pdf_name)
     loaded_grid = pineappl.grid.Grid.read(str(grid))
     pineappl_results = loaded_grid.convolute_with_one(
         2212, pdf.xfxQ2, pdf.alphasQ2, xi=tools.nine_points
     )
 
     df = pd.DataFrame(more_itertools.chunked(pineappl_results, len(tools.nine_points)))
```

### Comparing `pinefarm-0.2.2/src/pinefarm/tools.py` & `pinefarm-0.3.0/src/pinefarm/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Auxilariy tools."""
 import datetime
 import itertools
 import subprocess
 import time
 
 import lz4.frame
 import pineappl
@@ -178,15 +179,15 @@
     grid = pineappl.grid.Grid.read(str(input_file))
     set_grid_metadata(grid, entries, entries_from_file)
 
     grid.write(str(output_file))
 
 
 def set_grid_metadata(grid, entries=None, entries_from_file=None):
-    """Set metadata on a pineappl grid (in-place operation)
+    """Set metadata on a pineappl grid (in-place operation).
 
     Parameters
     ----------
     input_grid : pineappl.grid.Grid
         input grid on which to set metadata
     entries : dict
         mapping of key-value to store in the grid
@@ -205,15 +206,15 @@
 
     for k, v in entries_from_file.items():
         with open(v) as fd:
             grid.set_key_value(k, fd.read())
 
 
 def common_substring(s1, s2, *sn):
-    """Return the longest common part of two iterables, starting from the begininng
+    """Return the longest common part of two iterables, starting from the begininng.
 
     Parameters
     ----------
     s1 : Sequence
         first sequence to compare
     s2 : Sequence
         second sequence to compare
```

### Comparing `pinefarm-0.2.2/PKG-INFO` & `pinefarm-0.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7069 6e65  : 2.1.Name: pine
 00000020: 6661 726d 0a56 6572 7369 6f6e 3a20 302e  farm.Version: 0.
-00000030: 322e 320a 5375 6d6d 6172 793a 2047 656e  2.2.Summary: Gen
+00000030: 332e 300a 5375 6d6d 6172 793a 2047 656e  3.0.Summary: Gen
 00000040: 6572 6174 6520 5069 6e65 4150 504c 2067  erate PineAPPL g
 00000050: 7269 6473 2066 726f 6d20 5069 6e65 4361  rids from PineCa
 00000060: 7264 732e 0a48 6f6d 652d 7061 6765 3a20  rds..Home-page: 
 00000070: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
 00000080: 6f6d 2f4e 4e50 4446 2f72 756e 6361 7264  om/NNPDF/runcard
 00000090: 730a 4175 7468 6f72 3a20 416c 6573 7361  s.Author: Alessa
 000000a0: 6e64 726f 2043 616e 6469 646f 0a41 7574  ndro Candido.Aut
 000000b0: 686f 722d 656d 6169 6c3a 2063 616e 6469  hor-email: candi
 000000c0: 646f 2e61 6c65 4067 6d61 696c 2e63 6f6d  do.ale@gmail.com
 000000d0: 0a52 6571 7569 7265 732d 5079 7468 6f6e  .Requires-Python
-000000e0: 3a20 3e3d 332e 382c 3c33 2e31 310a 436c  : >=3.8,<3.11.Cl
+000000e0: 3a20 3e3d 332e 382c 3c33 2e31 320a 436c  : >=3.8,<3.12.Cl
 000000f0: 6173 7369 6669 6572 3a20 4c69 6365 6e73  assifier: Licens
 00000100: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
 00000110: 6420 3a3a 2047 4e55 2047 656e 6572 616c  d :: GNU General
 00000120: 2050 7562 6c69 6320 4c69 6365 6e73 6520   Public License 
 00000130: 7633 2028 4750 4c76 3329 0a43 6c61 7373  v3 (GPLv3).Class
 00000140: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
 00000150: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
@@ -29,120 +29,150 @@
 000001c0: 2050 7974 686f 6e20 3a3a 2033 2e39 0a43   Python :: 3.9.C
 000001d0: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
 000001e0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
 000001f0: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
 00000200: 300a 436c 6173 7369 6669 6572 3a20 5072  0.Classifier: Pr
 00000210: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
 00000220: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000230: 330a 436c 6173 7369 6669 6572 3a20 546f  3.Classifier: To
-00000240: 7069 6320 3a3a 2053 6369 656e 7469 6669  pic :: Scientifi
-00000250: 632f 456e 6769 6e65 6572 696e 6720 3a3a  c/Engineering ::
-00000260: 2050 6879 7369 6373 0a52 6571 7569 7265   Physics.Require
-00000270: 732d 4469 7374 3a20 5079 5941 4d4c 2028  s-Dist: PyYAML (
-00000280: 3e3d 362e 302e 302c 3c37 2e30 2e30 290a  >=6.0.0,<7.0.0).
-00000290: 5265 7175 6972 6573 2d44 6973 743a 2053  Requires-Dist: S
-000002a0: 7068 696e 7820 283e 3d34 2e32 2e30 2c3c  phinx (>=4.2.0,<
-000002b0: 352e 302e 3029 0a52 6571 7569 7265 732d  5.0.0).Requires-
-000002c0: 4469 7374 3a20 6133 6232 6262 6333 6365  Dist: a3b2bbc3ce
-000002d0: 6439 3736 3735 6163 3361 3731 6466 3435  d97675ac3a71df45
-000002e0: 6635 3562 6120 283e 3d36 2e34 2e30 2c3c  f55ba (>=6.4.0,<
-000002f0: 372e 302e 3029 0a52 6571 7569 7265 732d  7.0.0).Requires-
-00000300: 4469 7374 3a20 6170 7064 6972 7320 283e  Dist: appdirs (>
-00000310: 3d31 2e34 2e34 2c3c 322e 302e 3029 0a52  =1.4.4,<2.0.0).R
-00000320: 6571 7569 7265 732d 4469 7374 3a20 636c  equires-Dist: cl
-00000330: 6963 6b20 283e 3d38 2e30 2e31 2c3c 392e  ick (>=8.0.1,<9.
-00000340: 302e 3029 0a52 6571 7569 7265 732d 4469  0.0).Requires-Di
-00000350: 7374 3a20 656b 6f5b 626f 785d 2028 3e3d  st: eko[box] (>=
-00000360: 302e 3132 2e30 2c3c 302e 3133 2e30 290a  0.12.0,<0.13.0).
-00000370: 5265 7175 6972 6573 2d44 6973 743a 206c  Requires-Dist: l
-00000380: 6861 7064 662d 6d61 6e61 6765 6d65 6e74  hapdf-management
-00000390: 2028 3e3d 302e 322c 3c30 2e33 290a 5265   (>=0.2,<0.3).Re
-000003a0: 7175 6972 6573 2d44 6973 743a 206c 7a34  quires-Dist: lz4
-000003b0: 2028 3e3d 342e 302e 322c 3c35 2e30 2e30   (>=4.0.2,<5.0.0
-000003c0: 290a 5265 7175 6972 6573 2d44 6973 743a  ).Requires-Dist:
-000003d0: 206d 6f72 652d 6974 6572 746f 6f6c 7320   more-itertools 
-000003e0: 283e 3d38 2e31 302e 302c 3c39 2e30 2e30  (>=8.10.0,<9.0.0
-000003f0: 290a 5265 7175 6972 6573 2d44 6973 743a  ).Requires-Dist:
-00000400: 2070 616e 6461 7320 283e 3d31 2e33 2e30   pandas (>=1.3.0
-00000410: 2c3c 322e 302e 3029 0a52 6571 7569 7265  ,<2.0.0).Require
-00000420: 732d 4469 7374 3a20 7069 6e65 6170 706c  s-Dist: pineappl
-00000430: 2028 3e3d 302e 352e 372c 3c30 2e36 2e30   (>=0.5.7,<0.6.0
-00000440: 290a 5265 7175 6972 6573 2d44 6973 743a  ).Requires-Dist:
-00000450: 2070 6b67 636f 6e66 6967 2028 3e3d 312e   pkgconfig (>=1.
-00000460: 352e 352c 3c32 2e30 2e30 290a 5265 7175  5.5,<2.0.0).Requ
-00000470: 6972 6573 2d44 6973 743a 2070 7967 6974  ires-Dist: pygit
-00000480: 3220 283d 3d31 2e39 2e32 290a 5265 7175  2 (==1.9.2).Requ
-00000490: 6972 6573 2d44 6973 743a 2072 6571 7565  ires-Dist: reque
-000004a0: 7374 7320 283e 3d32 2e32 362e 302c 3c33  sts (>=2.26.0,<3
-000004b0: 2e30 2e30 290a 5265 7175 6972 6573 2d44  .0.0).Requires-D
-000004c0: 6973 743a 2072 6963 6820 283e 3d31 322e  ist: rich (>=12.
-000004d0: 352e 312c 3c31 332e 302e 3029 0a52 6571  5.1,<13.0.0).Req
-000004e0: 7569 7265 732d 4469 7374 3a20 7370 6869  uires-Dist: sphi
-000004f0: 6e78 2d72 7464 2d74 6865 6d65 2028 3e3d  nx-rtd-theme (>=
-00000500: 312e 302e 302c 3c32 2e30 2e30 290a 5265  1.0.0,<2.0.0).Re
-00000510: 7175 6972 6573 2d44 6973 743a 2073 7068  quires-Dist: sph
-00000520: 696e 7863 6f6e 7472 6962 2d62 6962 7465  inxcontrib-bibte
-00000530: 7820 283e 3d32 2e34 2e31 2c3c 332e 302e  x (>=2.4.1,<3.0.
-00000540: 3029 0a52 6571 7569 7265 732d 4469 7374  0).Requires-Dist
-00000550: 3a20 746f 6d6c 6920 283e 3d32 2e30 2e31  : tomli (>=2.0.1
-00000560: 2c3c 332e 302e 3029 0a52 6571 7569 7265  ,<3.0.0).Require
-00000570: 732d 4469 7374 3a20 7961 6469 736d 5b62  s-Dist: yadism[b
-00000580: 6f78 5d20 283e 3d30 2e31 322e 332c 3c30  ox] (>=0.12.3,<0
-00000590: 2e31 332e 3029 0a50 726f 6a65 6374 2d55  .13.0).Project-U
-000005a0: 524c 3a20 5265 706f 7369 746f 7279 2c20  RL: Repository, 
-000005b0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000005c0: 6f6d 2f4e 4e50 4446 2f72 756e 6361 7264  om/NNPDF/runcard
-000005d0: 730a 4465 7363 7269 7074 696f 6e2d 436f  s.Description-Co
-000005e0: 6e74 656e 742d 5479 7065 3a20 7465 7874  ntent-Type: text
-000005f0: 2f6d 6172 6b64 6f77 6e0a 0a23 2050 696e  /markdown..# Pin
-00000600: 6566 6172 6d0a 0a47 656e 6572 6174 6520  efarm..Generate 
-00000610: 7468 6520 636f 7272 6573 706f 6e64 696e  the correspondin
-00000620: 6720 5069 6e65 4150 504c 2067 7269 6473  g PineAPPL grids
-00000630: 2e0a 0a23 2320 496e 7374 616c 6c61 7469  ...## Installati
-00000640: 6f6e 0a0a 5468 6572 6520 6973 206e 6f20  on..There is no 
-00000650: 7265 6c65 6173 6564 2076 6572 7369 6f6e  released version
-00000660: 2063 7572 7265 6e74 6c79 2e0a 0a23 2323   currently...###
-00000670: 2044 6576 0a0a 466f 7220 6465 7665 6c6f   Dev..For develo
-00000680: 706d 656e 7420 796f 7520 6e65 6564 2074  pment you need t
-00000690: 6865 2066 6f6c 6c6f 7769 6e67 2074 6f6f  he following too
-000006a0: 6c73 3a0a 0a2d 2060 706f 6574 7279 602c  ls:..- `poetry`,
-000006b0: 2066 6f6c 6c6f 7720 5b69 6e73 7461 6c6c   follow [install
-000006c0: 6174 696f 6e0a 2020 696e 7374 7275 6374  ation.  instruct
-000006d0: 696f 6e73 5d28 6874 7470 733a 2f2f 7079  ions](https://py
-000006e0: 7468 6f6e 2d70 6f65 7472 792e 6f72 672f  thon-poetry.org/
-000006f0: 646f 6373 2f23 696e 7374 616c 6c61 7469  docs/#installati
-00000700: 6f6e 290a 2d20 6070 6f65 7472 792d 6479  on).- `poetry-dy
-00000710: 6e61 6d69 632d 7665 7273 696f 6e69 6e67  namic-versioning
-00000720: 602c 2075 7365 6420 746f 206d 616e 6167  `, used to manag
-00000730: 6520 7468 6520 7665 7273 696f 6e20 2873  e the version (s
-00000740: 6565 0a20 205b 7265 706f 5d28 6874 7470  ee.  [repo](http
-00000750: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6d  s://github.com/m
-00000760: 746b 656e 6e65 726c 792f 706f 6574 7279  tkennerly/poetry
-00000770: 2d64 796e 616d 6963 2d76 6572 7369 6f6e  -dynamic-version
-00000780: 696e 6729 290a 2d20 6070 7265 2d63 6f6d  ing)).- `pre-com
-00000790: 6d69 7460 2c20 746f 2072 756e 206d 6169  mit`, to run mai
-000007a0: 6e74 656e 616e 6365 2068 6f6f 6b73 2062  ntenance hooks b
-000007b0: 6566 6f72 6520 636f 6d6d 6974 7320 2873  efore commits (s
-000007c0: 6565 0a20 205b 696e 7374 7275 6374 696f  ee.  [instructio
-000007d0: 6e73 5d28 6874 7470 733a 2f2f 7072 652d  ns](https://pre-
-000007e0: 636f 6d6d 6974 2e63 6f6d 2f23 696e 7374  commit.com/#inst
-000007f0: 616c 6c29 290a 0a53 6565 205b 6265 6c6f  all))..See [belo
-00000800: 775d 282e 6769 7468 7562 2f43 4f4e 5452  w](.github/CONTR
-00000810: 4942 5554 494e 472e 6d64 236e 6f6e 2d70  IBUTING.md#non-p
-00000820: 7974 686f 6e2d 6465 7065 6e64 656e 6369  ython-dependenci
-00000830: 6573 2920 666f 7220 6120 6665 7720 6d6f  es) for a few mo
-00000840: 7265 0a64 6570 656e 6465 6e63 6965 7320  re.dependencies 
-00000850: 2861 6c72 6561 6479 2061 7661 696c 6162  (already availab
-00000860: 6c65 206f 6e20 6d6f 7374 2073 7973 7465  le on most syste
-00000870: 6d73 292e 0a0a 2323 2044 6f63 756d 656e  ms)...## Documen
-00000880: 7461 7469 6f6e 0a0a 5468 6520 646f 6375  tation..The docu
-00000890: 6d65 6e74 6174 696f 6e20 6973 206e 6f74  mentation is not
-000008a0: 2064 6570 6c6f 7965 6420 6174 2074 6865   deployed at the
-000008b0: 206d 6f6d 656e 742e 0a49 6e20 6f72 6465   moment..In orde
-000008c0: 7220 746f 2067 656e 6572 6174 6520 6974  r to generate it
-000008d0: 2069 6e73 7461 6c6c 2074 6865 2070 726f   install the pro
-000008e0: 6a65 6374 2069 6e20 6465 7665 6c6f 706d  ject in developm
-000008f0: 656e 742c 2061 6e64 2074 6865 6e20 646f  ent, and then do
-00000900: 3a0a 0a60 6060 7368 0a70 6f65 7472 7920  :..```sh.poetry 
-00000910: 7368 656c 6c0a 6364 2064 6f63 730a 6d61  shell.cd docs.ma
-00000920: 6b65 2068 746d 6c0a 6d61 6b65 2076 6965  ke html.make vie
-00000930: 770a 6060 600a 0a                        w.```..
+00000230: 332e 3131 0a43 6c61 7373 6966 6965 723a  3.11.Classifier:
+00000240: 2054 6f70 6963 203a 3a20 5363 6965 6e74   Topic :: Scient
+00000250: 6966 6963 2f45 6e67 696e 6565 7269 6e67  ific/Engineering
+00000260: 203a 3a20 5068 7973 6963 730a 5265 7175   :: Physics.Requ
+00000270: 6972 6573 2d44 6973 743a 2050 7959 414d  ires-Dist: PyYAM
+00000280: 4c20 283e 3d36 2e30 2e30 2c3c 372e 302e  L (>=6.0.0,<7.0.
+00000290: 3029 0a52 6571 7569 7265 732d 4469 7374  0).Requires-Dist
+000002a0: 3a20 6170 7064 6972 7320 283e 3d31 2e34  : appdirs (>=1.4
+000002b0: 2e34 2c3c 322e 302e 3029 0a52 6571 7569  .4,<2.0.0).Requi
+000002c0: 7265 732d 4469 7374 3a20 636c 6963 6b20  res-Dist: click 
+000002d0: 283e 3d38 2e30 2e31 2c3c 392e 302e 3029  (>=8.0.1,<9.0.0)
+000002e0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+000002f0: 6c68 6170 6466 2d6d 616e 6167 656d 656e  lhapdf-managemen
+00000300: 7420 283e 3d30 2e33 2c3c 302e 3429 0a52  t (>=0.3,<0.4).R
+00000310: 6571 7569 7265 732d 4469 7374 3a20 6c7a  equires-Dist: lz
+00000320: 3420 283e 3d34 2e30 2e32 2c3c 352e 302e  4 (>=4.0.2,<5.0.
+00000330: 3029 0a52 6571 7569 7265 732d 4469 7374  0).Requires-Dist
+00000340: 3a20 6d6f 7265 2d69 7465 7274 6f6f 6c73  : more-itertools
+00000350: 2028 3e3d 382e 3130 2e30 2c3c 392e 302e   (>=8.10.0,<9.0.
+00000360: 3029 0a52 6571 7569 7265 732d 4469 7374  0).Requires-Dist
+00000370: 3a20 7061 6e64 6173 2028 3e3d 312e 332e  : pandas (>=1.3.
+00000380: 302c 3c32 2e30 2e30 290a 5265 7175 6972  0,<2.0.0).Requir
+00000390: 6573 2d44 6973 743a 2070 696e 6561 7070  es-Dist: pineapp
+000003a0: 6c20 283e 3d30 2e36 2e30 2c3c 302e 372e  l (>=0.6.0,<0.7.
+000003b0: 3029 0a52 6571 7569 7265 732d 4469 7374  0).Requires-Dist
+000003c0: 3a20 706b 6763 6f6e 6669 6720 283e 3d31  : pkgconfig (>=1
+000003d0: 2e35 2e35 2c3c 322e 302e 3029 0a52 6571  .5.5,<2.0.0).Req
+000003e0: 7569 7265 732d 4469 7374 3a20 7079 6769  uires-Dist: pygi
+000003f0: 7432 2028 3e3d 312e 3132 2e30 2c3c 322e  t2 (>=1.12.0,<2.
+00000400: 302e 3029 0a52 6571 7569 7265 732d 4469  0.0).Requires-Di
+00000410: 7374 3a20 7265 7175 6573 7473 2028 3e3d  st: requests (>=
+00000420: 322e 3236 2e30 2c3c 332e 302e 3029 0a52  2.26.0,<3.0.0).R
+00000430: 6571 7569 7265 732d 4469 7374 3a20 7269  equires-Dist: ri
+00000440: 6368 2028 3e3d 3132 2e35 2e31 2c3c 3133  ch (>=12.5.1,<13
+00000450: 2e30 2e30 290a 5265 7175 6972 6573 2d44  .0.0).Requires-D
+00000460: 6973 743a 2074 6f6d 6c69 2028 3e3d 322e  ist: tomli (>=2.
+00000470: 302e 312c 3c33 2e30 2e30 290a 5265 7175  0.1,<3.0.0).Requ
+00000480: 6972 6573 2d44 6973 743a 2079 6164 6973  ires-Dist: yadis
+00000490: 6d5b 626f 785d 2028 3e3d 302e 3132 2e34  m[box] (>=0.12.4
+000004a0: 2c3c 302e 3133 2e30 290a 5072 6f6a 6563  ,<0.13.0).Projec
+000004b0: 742d 5552 4c3a 2052 6570 6f73 6974 6f72  t-URL: Repositor
+000004c0: 792c 2068 7474 7073 3a2f 2f67 6974 6875  y, https://githu
+000004d0: 622e 636f 6d2f 4e4e 5044 462f 7275 6e63  b.com/NNPDF/runc
+000004e0: 6172 6473 0a44 6573 6372 6970 7469 6f6e  ards.Description
+000004f0: 2d43 6f6e 7465 6e74 2d54 7970 653a 2074  -Content-Type: t
+00000500: 6578 742f 6d61 726b 646f 776e 0a0a 2320  ext/markdown..# 
+00000510: 5069 6e65 6661 726d 0a0a 3c70 2061 6c69  Pinefarm..<p ali
+00000520: 676e 3d22 6365 6e74 6572 223e 0a20 203c  gn="center">.  <
+00000530: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00000540: 6769 7468 7562 2e63 6f6d 2f4e 4e50 4446  github.com/NNPDF
+00000550: 2f70 696e 6566 6172 6d2f 6163 7469 6f6e  /pinefarm/action
+00000560: 732f 776f 726b 666c 6f77 732f 756e 6974  s/workflows/unit
+00000570: 7465 7374 732e 796d 6c22 3e3c 696d 6720  tests.yml"><img 
+00000580: 616c 743d 2254 6573 7473 2220 7372 633d  alt="Tests" src=
+00000590: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+000005a0: 636f 6d2f 4e4e 5044 462f 7069 6e65 6661  com/NNPDF/pinefa
+000005b0: 726d 2f61 6374 696f 6e73 2f77 6f72 6b66  rm/actions/workf
+000005c0: 6c6f 7773 2f75 6e69 7474 6573 7473 2e79  lows/unittests.y
+000005d0: 6d6c 2f62 6164 6765 2e73 7667 2220 2f3e  ml/badge.svg" />
+000005e0: 3c2f 613e 0a20 203c 6120 6872 6566 3d22  </a>.  <a href="
+000005f0: 6874 7470 733a 2f2f 7069 6e65 6661 726d  https://pinefarm
+00000600: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
+00000610: 656e 2f6c 6174 6573 742f 3f62 6164 6765  en/latest/?badge
+00000620: 3d6c 6174 6573 7422 3e3c 696d 6720 616c  =latest"><img al
+00000630: 743d 2244 6f63 7322 2073 7263 3d22 6874  t="Docs" src="ht
+00000640: 7470 733a 2f2f 7265 6164 7468 6564 6f63  tps://readthedoc
+00000650: 732e 6f72 672f 7072 6f6a 6563 7473 2f70  s.org/projects/p
+00000660: 696e 6566 6172 6d2f 6261 6467 652f 3f76  inefarm/badge/?v
+00000670: 6572 7369 6f6e 3d6c 6174 6573 7422 3e3c  ersion=latest"><
+00000680: 2f61 3e0a 3c2f 703e 0a0a 4765 6e65 7261  /a>.</p>..Genera
+00000690: 7465 205b 5069 6e65 4150 504c 2067 7269  te [PineAPPL gri
+000006a0: 6473 5d28 6874 7470 733a 2f2f 6769 7468  ds](https://gith
+000006b0: 7562 2e63 6f6d 2f4e 4e50 4446 2f70 696e  ub.com/NNPDF/pin
+000006c0: 6561 7070 6c29 2066 726f 6d20 5b70 696e  eappl) from [pin
+000006d0: 6563 6172 6473 5d28 6874 7470 733a 2f2f  ecards](https://
+000006e0: 6769 7468 7562 2e63 6f6d 2f4e 4e50 4446  github.com/NNPDF
+000006f0: 2f70 696e 6563 6172 6473 292e 0a0a 2323  /pinecards)...##
+00000700: 2049 6e73 7461 6c6c 6174 696f 6e0a 0a70   Installation..p
+00000710: 696e 6566 6172 6d20 6973 2061 7661 696c  inefarm is avail
+00000720: 6162 6c65 2076 6961 0a2d 2050 7950 493a  able via.- PyPI:
+00000730: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+00000740: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
+00000750: 6374 2f70 696e 6566 6172 6d2f 223e 3c69  ct/pinefarm/"><i
+00000760: 6d67 2061 6c74 3d22 5079 5049 2220 7372  mg alt="PyPI" sr
+00000770: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
+00000780: 6869 656c 6473 2e69 6f2f 7079 7069 2f76  hields.io/pypi/v
+00000790: 2f70 696e 6566 6172 6d22 2f3e 3c2f 613e  /pinefarm"/></a>
+000007a0: 0a60 6060 6261 7368 0a70 6970 2069 6e73  .```bash.pip ins
+000007b0: 7461 6c6c 2070 696e 6566 6172 6d0a 6060  tall pinefarm.``
+000007c0: 600a 0a23 2323 2044 6576 0a0a 466f 7220  `..### Dev..For 
+000007d0: 6465 7665 6c6f 706d 656e 7420 796f 7520  development you 
+000007e0: 6e65 6564 2074 6865 2066 6f6c 6c6f 7769  need the followi
+000007f0: 6e67 2074 6f6f 6c73 3a0a 0a2d 2060 706f  ng tools:..- `po
+00000800: 6574 7279 602c 2066 6f6c 6c6f 7720 5b69  etry`, follow [i
+00000810: 6e73 7461 6c6c 6174 696f 6e0a 2020 696e  nstallation.  in
+00000820: 7374 7275 6374 696f 6e73 5d28 6874 7470  structions](http
+00000830: 733a 2f2f 7079 7468 6f6e 2d70 6f65 7472  s://python-poetr
+00000840: 792e 6f72 672f 646f 6373 2f23 696e 7374  y.org/docs/#inst
+00000850: 616c 6c61 7469 6f6e 290a 2d20 6070 6f65  allation).- `poe
+00000860: 7472 792d 6479 6e61 6d69 632d 7665 7273  try-dynamic-vers
+00000870: 696f 6e69 6e67 602c 2075 7365 6420 746f  ioning`, used to
+00000880: 206d 616e 6167 6520 7468 6520 7665 7273   manage the vers
+00000890: 696f 6e20 2873 6565 0a20 205b 7265 706f  ion (see.  [repo
+000008a0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+000008b0: 2e63 6f6d 2f6d 746b 656e 6e65 726c 792f  .com/mtkennerly/
+000008c0: 706f 6574 7279 2d64 796e 616d 6963 2d76  poetry-dynamic-v
+000008d0: 6572 7369 6f6e 696e 6729 290a 2d20 6070  ersioning)).- `p
+000008e0: 7265 2d63 6f6d 6d69 7460 2c20 746f 2072  re-commit`, to r
+000008f0: 756e 206d 6169 6e74 656e 616e 6365 2068  un maintenance h
+00000900: 6f6f 6b73 2062 6566 6f72 6520 636f 6d6d  ooks before comm
+00000910: 6974 7320 2873 6565 0a20 205b 696e 7374  its (see.  [inst
+00000920: 7275 6374 696f 6e73 5d28 6874 7470 733a  ructions](https:
+00000930: 2f2f 7072 652d 636f 6d6d 6974 2e63 6f6d  //pre-commit.com
+00000940: 2f23 696e 7374 616c 6c29 290a 0a53 6565  /#install))..See
+00000950: 205b 6265 6c6f 775d 282e 6769 7468 7562   [below](.github
+00000960: 2f43 4f4e 5452 4942 5554 494e 472e 6d64  /CONTRIBUTING.md
+00000970: 236e 6f6e 2d70 7974 686f 6e2d 6465 7065  #non-python-depe
+00000980: 6e64 656e 6369 6573 2920 666f 7220 6120  ndencies) for a 
+00000990: 6665 7720 6d6f 7265 0a64 6570 656e 6465  few more.depende
+000009a0: 6e63 6965 7320 2861 6c72 6561 6479 2061  ncies (already a
+000009b0: 7661 696c 6162 6c65 206f 6e20 6d6f 7374  vailable on most
+000009c0: 2073 7973 7465 6d73 292e 0a0a 2323 2044   systems)...## D
+000009d0: 6f63 756d 656e 7461 7469 6f6e 0a2d 2054  ocumentation.- T
+000009e0: 6865 2064 6f63 756d 656e 7461 7469 6f6e  he documentation
+000009f0: 2069 7320 6176 6169 6c61 626c 6520 6865   is available he
+00000a00: 7265 3a20 3c61 2068 7265 663d 2268 7474  re: <a href="htt
+00000a10: 7073 3a2f 2f70 696e 6566 6172 6d2e 7265  ps://pinefarm.re
+00000a20: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
+00000a30: 6c61 7465 7374 2f3f 6261 6467 653d 6c61  latest/?badge=la
+00000a40: 7465 7374 223e 3c69 6d67 2061 6c74 3d22  test"><img alt="
+00000a50: 446f 6373 2220 7372 633d 2268 7474 7073  Docs" src="https
+00000a60: 3a2f 2f72 6561 6474 6865 646f 6373 2e6f  ://readthedocs.o
+00000a70: 7267 2f70 726f 6a65 6374 732f 7069 6e65  rg/projects/pine
+00000a80: 6661 726d 2f62 6164 6765 2f3f 7665 7273  farm/badge/?vers
+00000a90: 696f 6e3d 6c61 7465 7374 223e 3c2f 613e  ion=latest"></a>
+00000aa0: 0a2d 2054 6f20 6275 696c 6420 7468 6520  .- To build the 
+00000ab0: 646f 6375 6d65 6e74 6174 696f 6e20 6672  documentation fr
+00000ac0: 6f6d 2073 6f75 7263 6520 7275 6e20 7468  om source run th
+00000ad0: 6573 6520 636f 6d6d 616e 6473 0a0a 6060  ese commands..``
+00000ae0: 6073 680a 706f 6574 7279 2073 6865 6c6c  `sh.poetry shell
+00000af0: 0a63 6420 646f 6373 0a6d 616b 6520 6874  .cd docs.make ht
+00000b00: 6d6c 0a6d 616b 6520 7669 6577 0a60 6060  ml.make view.```
+00000b10: 0a0a                                     ..
```

