# Comparing `tmp/m23-1.1.0.tar.gz` & `tmp/m23-1.2.0.tar.gz`

## Comparing `m23-1.1.0.tar` & `m23-1.2.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 m23-1.1.0/.flake8
--rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 m23-1.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 m23-1.1.0/brown.toml
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 m23-1.1.0/mf.toml
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 m23-1.1.0/nights_csv.toml
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 m23-1.1.0/rainbow.toml
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 m23-1.1.0/renormalize.toml
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 m23-1.1.0/requirements.txt
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 m23-1.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 m23-1.1.0/.github/workflows/semantic-release.yml
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 m23-1.1.0/.vscode/settings.json
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/__init__.py
--rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/__main__.py
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/constants.py
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/align/__init__.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/calibrate/__init__.py
--rw-r--r--   0        0        0     7980 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/calibrate/calibration.py
--rw-r--r--   0        0        0     4408 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/calibrate/master_calibrate.py
--rw-r--r--   0        0        0     6966 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/charts/__init__.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/combine/__init__.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/exceptions/__init__.py
--rw-r--r--   0        0        0     8607 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/extract/__init__.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/file/__init__.py
--rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/file/aligned_combined_file.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/file/alignment_stats_file.py
--rw-r--r--   0        0        0     4232 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/file/color_normalized_file.py
--rw-r--r--   0        0        0    12074 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/file/flux_log_combined_file.py
--rw-r--r--   0        0        0     9248 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/file/log_file_combined_file.py
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/file/masterflat_file.py
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/file/normfactor_file.py
--rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/file/raw_image_file.py
--rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/file/reference_log_file.py
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/file/ri_color_file.py
--rw-r--r--   0        0        0     5527 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/file/sky_bg_file.py
--rw-r--r--   0        0        0    21812 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/internight_normalize/__init__.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/matrix/__init__.py
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/matrix/crop.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/matrix/fill.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/matrix/region.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/matrix/utils.py
--rw-r--r--   0        0        0     7926 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/norm/__init__.py
--rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/norm/get_line.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/processor/__init__.py
--rw-r--r--   0        0        0    16157 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/processor/config_loader.py
--rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/processor/generate_masterflat.py
--rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/processor/generate_masterflat_config_loader.py
--rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/processor/nights_csv.py
--rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/processor/nights_csv_config_loader.py
--rw-r--r--   0        0        0    22118 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/processor/process_nights.py
--rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/processor/renormalize.py
--rw-r--r--   0        0        0     7499 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/processor/renormalize_config_loader.py
--rw-r--r--   0        0        0   725365 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/reference/08-05-03_m23_3.5-071.txt
--rw-r--r--   0        0        0    18521 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/reference/MeanRI100.txt
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/reference/README.md
--rw-r--r--   0        0        0   191836 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/reference/ref_revised_71.txt
--rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/sky/__init__.py
--rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/sky/moon/__init__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/trans/__init__.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/trans/fits.py
--rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/utils/__init__.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/utils/date.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/utils/flux_to_magnitude.py
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 m23-1.1.0/src/m23/utils/rename.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 m23-1.1.0/tests/__init__.py
--rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 m23-1.1.0/.gitignore
--rw-r--r--   0        0        0    13309 2020-02-02 00:00:00.000000 m23-1.1.0/README.md
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 m23-1.1.0/pyproject.toml
--rw-r--r--   0        0        0    13681 2020-02-02 00:00:00.000000 m23-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 m23-1.2.0/.flake8
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 m23-1.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 m23-1.2.0/brown.toml
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 m23-1.2.0/mf.toml
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 m23-1.2.0/nights_csv.toml
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 m23-1.2.0/rainbow.toml
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 m23-1.2.0/renormalize.toml
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 m23-1.2.0/requirements.txt
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 m23-1.2.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 m23-1.2.0/.github/workflows/semantic-release.yml
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 m23-1.2.0/.vscode/settings.json
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 m23-1.2.0/src/m23/__init__.py
+-rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 m23-1.2.0/src/m23/__main__.py
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 m23-1.2.0/src/m23/constants.py
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 m23-1.2.0/src/m23/align/__init__.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 m23-1.2.0/src/m23/calibrate/__init__.py
+-rw-r--r--   0        0        0     7980 2020-02-02 00:00:00.000000 m23-1.2.0/src/m23/calibrate/calibration.py
+-rw-r--r--   0        0        0     4408 2020-02-02 00:00:00.000000 m23-1.2.0/src/m23/calibrate/master_calibrate.py
+-rw-r--r--   0        0        0     6966 2020-02-02 00:00:00.000000 m23-1.2.0/src/m23/charts/__init__.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 m23-1.2.0/src/m23/combine/__init__.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 m23-1.2.0/src/m23/exceptions/__init__.py
+-rw-r--r--   0        0        0     8607 2020-02-02 00:00:00.000000 m23-1.2.0/src/m23/extract/__init__.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 m23-1.2.0/src/m23/file/__init__.py
+-rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 m23-1.2.0/src/m23/file/aligned_combined_file.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 m23-1.2.0/src/m23/file/alignment_stats_file.py
+-rw-r--r--   0        0        0     4232 2020-02-02 00:00:00.000000 m23-1.2.0/src/m23/file/color_normalized_file.py
+-rw-r--r--   0        0        0    12074 2020-02-02 00:00:00.000000 m23-1.2.0/src/m23/file/flux_log_combined_file.py
+-rw-r--r--   0        0        0     9248 2020-02-02 00:00:00.000000 m23-1.2.0/src/m23/file/log_file_combined_file.py
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 m23-1.2.0/src/m23/file/masterflat_file.py
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 m23-1.2.0/src/m23/file/normfactor_file.py
+-rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 m23-1.2.0/src/m23/file/raw_image_file.py
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 m23-1.2.0/src/m23/file/reference_log_file.py
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 m23-1.2.0/src/m23/file/ri_color_file.py
+-rw-r--r--   0        0        0     5527 2020-02-02 00:00:00.000000 m23-1.2.0/src/m23/file/sky_bg_file.py
+-rw-r--r--   0        0        0    21812 2020-02-02 00:00:00.000000 m23-1.2.0/src/m23/internight_normalize/__init__.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 m23-1.2.0/src/m23/matrix/__init__.py
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 m23-1.2.0/src/m23/matrix/crop.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 m23-1.2.0/src/m23/matrix/fill.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 m23-1.2.0/src/m23/matrix/region.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 m23-1.2.0/src/m23/matrix/utils.py
+-rw-r--r--   0        0        0     7926 2020-02-02 00:00:00.000000 m23-1.2.0/src/m23/norm/__init__.py
+-rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 m23-1.2.0/src/m23/norm/get_line.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 m23-1.2.0/src/m23/processor/__init__.py
+-rw-r--r--   0        0        0    16157 2020-02-02 00:00:00.000000 m23-1.2.0/src/m23/processor/config_loader.py
+-rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 m23-1.2.0/src/m23/processor/generate_masterflat.py
+-rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 m23-1.2.0/src/m23/processor/generate_masterflat_config_loader.py
+-rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 m23-1.2.0/src/m23/processor/nights_csv.py
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 m23-1.2.0/src/m23/processor/nights_csv_config_loader.py
+-rw-r--r--   0        0        0    22171 2020-02-02 00:00:00.000000 m23-1.2.0/src/m23/processor/process_nights.py
+-rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 m23-1.2.0/src/m23/processor/renormalize.py
+-rw-r--r--   0        0        0     7499 2020-02-02 00:00:00.000000 m23-1.2.0/src/m23/processor/renormalize_config_loader.py
+-rw-r--r--   0        0        0   725365 2020-02-02 00:00:00.000000 m23-1.2.0/src/m23/reference/08-05-03_m23_3.5-071.txt
+-rw-r--r--   0        0        0    18521 2020-02-02 00:00:00.000000 m23-1.2.0/src/m23/reference/MeanRI100.txt
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 m23-1.2.0/src/m23/reference/README.md
+-rw-r--r--   0        0        0   191836 2020-02-02 00:00:00.000000 m23-1.2.0/src/m23/reference/ref_revised_71.txt
+-rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 m23-1.2.0/src/m23/sky/__init__.py
+-rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 m23-1.2.0/src/m23/sky/moon/__init__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 m23-1.2.0/src/m23/trans/__init__.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 m23-1.2.0/src/m23/trans/fits.py
+-rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 m23-1.2.0/src/m23/utils/__init__.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 m23-1.2.0/src/m23/utils/date.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 m23-1.2.0/src/m23/utils/flux_to_magnitude.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 m23-1.2.0/src/m23/utils/rename.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 m23-1.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 m23-1.2.0/.gitignore
+-rw-r--r--   0        0        0    13309 2020-02-02 00:00:00.000000 m23-1.2.0/README.md
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 m23-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0    13681 2020-02-02 00:00:00.000000 m23-1.2.0/PKG-INFO
```

### Comparing `m23-1.1.0/CHANGELOG.md` & `m23-1.2.0/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.2.0 (2023-06-21)
+
+### Feature
+
+* Add date to the masterflat filename ([`30a86d4`](https://github.com/LutherAstrophysics/m23/commit/30a86d4288fe94dc4dd6d44490d5991326663081))
+
+### Fix
+
+* Add missing f-string ([`0014fe4`](https://github.com/LutherAstrophysics/m23/commit/0014fe4b2dbf713487992b968589472087e1d50d))
+
 ## v1.1.0 (2023-06-21)
 
 ### Feature
 
 * Write the version number of the m23 in logfile first thing ([`25de6f1`](https://github.com/LutherAstrophysics/m23/commit/25de6f1da66ad56b4d2e5c790b1f54b547dcf4aa))
 * Add __version__ variable ([`8b29c9d`](https://github.com/LutherAstrophysics/m23/commit/8b29c9dedcee5fa7138890c9183b2f40a1073739))
```

### Comparing `m23-1.1.0/brown.toml` & `m23-1.2.0/brown.toml`

 * *Files identical despite different names*

### Comparing `m23-1.1.0/mf.toml` & `m23-1.2.0/mf.toml`

 * *Files identical despite different names*

### Comparing `m23-1.1.0/nights_csv.toml` & `m23-1.2.0/nights_csv.toml`

 * *Files identical despite different names*

### Comparing `m23-1.1.0/rainbow.toml` & `m23-1.2.0/rainbow.toml`

 * *Files identical despite different names*

### Comparing `m23-1.1.0/requirements.txt` & `m23-1.2.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `m23-1.1.0/.github/workflows/python-publish.yml` & `m23-1.2.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `m23-1.1.0/.vscode/settings.json` & `m23-1.2.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `m23-1.1.0/src/m23/__main__.py` & `m23-1.2.0/src/m23/__main__.py`

 * *Files identical despite different names*

### Comparing `m23-1.1.0/src/m23/constants.py` & `m23-1.2.0/src/m23/constants.py`

 * *Files identical despite different names*

### Comparing `m23-1.1.0/src/m23/align/__init__.py` & `m23-1.2.0/src/m23/align/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.1.0/src/m23/calibrate/calibration.py` & `m23-1.2.0/src/m23/calibrate/calibration.py`

 * *Files identical despite different names*

### Comparing `m23-1.1.0/src/m23/calibrate/master_calibrate.py` & `m23-1.2.0/src/m23/calibrate/master_calibrate.py`

 * *Files identical despite different names*

### Comparing `m23-1.1.0/src/m23/charts/__init__.py` & `m23-1.2.0/src/m23/charts/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.1.0/src/m23/combine/__init__.py` & `m23-1.2.0/src/m23/combine/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.1.0/src/m23/extract/__init__.py` & `m23-1.2.0/src/m23/extract/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.1.0/src/m23/file/__init__.py` & `m23-1.2.0/src/m23/file/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.1.0/src/m23/file/aligned_combined_file.py` & `m23-1.2.0/src/m23/file/aligned_combined_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.1.0/src/m23/file/alignment_stats_file.py` & `m23-1.2.0/src/m23/file/alignment_stats_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.1.0/src/m23/file/color_normalized_file.py` & `m23-1.2.0/src/m23/file/color_normalized_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.1.0/src/m23/file/flux_log_combined_file.py` & `m23-1.2.0/src/m23/file/flux_log_combined_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.1.0/src/m23/file/log_file_combined_file.py` & `m23-1.2.0/src/m23/file/log_file_combined_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.1.0/src/m23/file/masterflat_file.py` & `m23-1.2.0/src/m23/file/masterflat_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.1.0/src/m23/file/normfactor_file.py` & `m23-1.2.0/src/m23/file/normfactor_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.1.0/src/m23/file/raw_image_file.py` & `m23-1.2.0/src/m23/file/raw_image_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.1.0/src/m23/file/reference_log_file.py` & `m23-1.2.0/src/m23/file/reference_log_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.1.0/src/m23/file/ri_color_file.py` & `m23-1.2.0/src/m23/file/ri_color_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.1.0/src/m23/file/sky_bg_file.py` & `m23-1.2.0/src/m23/file/sky_bg_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.1.0/src/m23/internight_normalize/__init__.py` & `m23-1.2.0/src/m23/internight_normalize/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.1.0/src/m23/matrix/fill.py` & `m23-1.2.0/src/m23/matrix/fill.py`

 * *Files identical despite different names*

### Comparing `m23-1.1.0/src/m23/norm/__init__.py` & `m23-1.2.0/src/m23/norm/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.1.0/src/m23/norm/get_line.py` & `m23-1.2.0/src/m23/norm/get_line.py`

 * *Files identical despite different names*

### Comparing `m23-1.1.0/src/m23/processor/config_loader.py` & `m23-1.2.0/src/m23/processor/config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-1.1.0/src/m23/processor/generate_masterflat.py` & `m23-1.2.0/src/m23/processor/generate_masterflat.py`

 * *Files identical despite different names*

### Comparing `m23-1.1.0/src/m23/processor/generate_masterflat_config_loader.py` & `m23-1.2.0/src/m23/processor/generate_masterflat_config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-1.1.0/src/m23/processor/nights_csv.py` & `m23-1.2.0/src/m23/processor/nights_csv.py`

 * *Files identical despite different names*

### Comparing `m23-1.1.0/src/m23/processor/nights_csv_config_loader.py` & `m23-1.2.0/src/m23/processor/nights_csv_config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-1.1.0/src/m23/processor/process_nights.py` & `m23-1.2.0/src/m23/processor/process_nights.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,25 +19,25 @@
     ALIGNED_FOLDER_NAME,
     CONFIG_FILE_NAME,
     FLUX_LOGS_COMBINED_FOLDER_NAME,
     INPUT_CALIBRATION_FOLDER_NAME,
     LOG_FILES_COMBINED_FOLDER_NAME,
     M23_RAW_IMAGES_FOLDER_NAME,
     MASTER_DARK_NAME,
-    MASTER_FLAT_NAME,
     OUTPUT_CALIBRATION_FOLDER_NAME,
     RAW_CALIBRATED_FOLDER_NAME,
     SKY_BG_BOX_REGION_SIZE,
     SKY_BG_FOLDER_NAME,
 )
 from m23.exceptions import CouldNotAlignException
 from m23.extract import extract_stars, sky_bg_average_for_all_regions
 from m23.file.aligned_combined_file import AlignedCombinedFile
 from m23.file.alignment_stats_file import AlignmentStatsFile
 from m23.file.log_file_combined_file import LogFileCombinedFile
+from m23.file.masterflat_file import MasterflatFile
 from m23.file.raw_image_file import RawImageFile
 from m23.file.reference_log_file import ReferenceLogFile
 from m23.file.sky_bg_file import SkyBgFile
 from m23.internight_normalize import internight_normalize
 from m23.matrix import crop
 from m23.matrix.fill import fillMatrix
 from m23.norm import normalize_log_files
@@ -162,15 +162,15 @@
     normfactors: Dictionary of normfactors for various radii of extraction
 
     """
     logger = logging.getLogger("LOGGER_" + str(night_date))
     logger.info("Generating sky background file")
     bg_data_of_all_images = []
 
-    for index, logfile in enumerate(log_files_to_use):
+    for logfile in enumerate(log_files_to_use):
         date_time_of_image = logfile.datetime()
         # Here we find the corresponding aligned combined file first
         # so we can use that to calculate the sky bg data.
         aligned_combined_folder = logfile.path().parent.parent / ALIGNED_COMBINED_FOLDER_NAME
         aligned_combined_file_name = AlignedCombinedFile.generate_file_name(
             logfile.img_duration(), logfile.img_number()
         )
@@ -330,15 +330,15 @@
     else:
         flats = fit_data_from_fit_images(get_flats(NIGHT_INPUT_CALIBRATION_FOLDER))
         # Ensure that image dimensions are as specified by rows and cols
         # If there's extra noise cols or rows, we crop them
         flats = [crop(matrix, rows, cols) for matrix in flats]
 
         master_flat_data = makeMasterFlat(
-            saveAs=CALIBRATION_OUTPUT_FOLDER / MASTER_FLAT_NAME,
+            saveAs=CALIBRATION_OUTPUT_FOLDER / MasterflatFile.generate_file_name(night_date),
             masterDarkData=master_dark_data,
             headerToCopyFromName=next(
                 get_flats(NIGHT_INPUT_CALIBRATION_FOLDER)
             ).absolute(),  # Gets absolute path of first flat file
             listOfFlatData=flats,
         )
         logger.info("Created masterflat")
@@ -385,15 +385,15 @@
         )
 
         if save_calibrated_images:
             for index, raw_image_index in enumerate(range(from_index, to_index)):
                 raw_img = raw_images[raw_image_index]
                 calibrated_image = RawImageFile(RAW_CALIBRATED_OUTPUT_FOLDER / raw_img.path().name)
                 calibrated_image.create_file(images_data[index], raw_img)
-                logger.info("Saving calibrated image. {raw_image_index}")
+                logger.info(f"Saving calibrated image. {raw_image_index}")
 
         # Fill out the cropped regions with value of 1
         # Note, it's important to fill after the calibration step
         if len(crop_region) > 0:
             images_data = [fillMatrix(matrix, crop_region, 1) for matrix in images_data]
 
         # Alignment
```

### Comparing `m23-1.1.0/src/m23/processor/renormalize.py` & `m23-1.2.0/src/m23/processor/renormalize.py`

 * *Files identical despite different names*

### Comparing `m23-1.1.0/src/m23/processor/renormalize_config_loader.py` & `m23-1.2.0/src/m23/processor/renormalize_config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-1.1.0/src/m23/reference/08-05-03_m23_3.5-071.txt` & `m23-1.2.0/src/m23/reference/08-05-03_m23_3.5-071.txt`

 * *Files identical despite different names*

### Comparing `m23-1.1.0/src/m23/reference/MeanRI100.txt` & `m23-1.2.0/src/m23/reference/MeanRI100.txt`

 * *Files identical despite different names*

### Comparing `m23-1.1.0/src/m23/reference/README.md` & `m23-1.2.0/src/m23/reference/README.md`

 * *Files identical despite different names*

### Comparing `m23-1.1.0/src/m23/reference/ref_revised_71.txt` & `m23-1.2.0/src/m23/reference/ref_revised_71.txt`

 * *Files identical despite different names*

### Comparing `m23-1.1.0/src/m23/sky/__init__.py` & `m23-1.2.0/src/m23/sky/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.1.0/src/m23/sky/moon/__init__.py` & `m23-1.2.0/src/m23/sky/moon/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.1.0/src/m23/utils/__init__.py` & `m23-1.2.0/src/m23/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.1.0/src/m23/utils/date.py` & `m23-1.2.0/src/m23/utils/date.py`

 * *Files identical despite different names*

### Comparing `m23-1.1.0/src/m23/utils/rename.py` & `m23-1.2.0/src/m23/utils/rename.py`

 * *Files identical despite different names*

### Comparing `m23-1.1.0/.gitignore` & `m23-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `m23-1.1.0/README.md` & `m23-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `m23-1.1.0/pyproject.toml` & `m23-1.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "m23"
 readme = "README.md"
 requires-python = ">=3.10"
-version = "1.1.0"
+version = "1.2.0"
 dependencies = [
     "numpy==1.24.2",
     'toml==0.10.2',
     'astropy==5.2.1',
     'astroalign==2.4.1',
     'typing_extensions==4.4.0',
     'opencv-python==4.7.0.68',
```

### Comparing `m23-1.1.0/PKG-INFO` & `m23-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m23
-Version: 1.1.0
+Version: 1.2.0
 Requires-Python: >=3.10
 Requires-Dist: astroalign==2.4.1
 Requires-Dist: astropy==5.2.1
 Requires-Dist: ephem==4.1.4
 Requires-Dist: matplotlib==3.7.0
 Requires-Dist: numpy==1.24.2
 Requires-Dist: opencv-python==4.7.0.68
```

