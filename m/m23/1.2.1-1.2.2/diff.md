# Comparing `tmp/m23-1.2.1.tar.gz` & `tmp/m23-1.2.2.tar.gz`

## Comparing `m23-1.2.1.tar` & `m23-1.2.2.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 m23-1.2.1/.flake8
--rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 m23-1.2.1/CHANGELOG.md
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 m23-1.2.1/brown.toml
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 m23-1.2.1/mf.toml
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 m23-1.2.1/nights_csv.toml
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 m23-1.2.1/rainbow.toml
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 m23-1.2.1/renormalize.toml
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 m23-1.2.1/requirements.txt
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 m23-1.2.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 m23-1.2.1/.github/workflows/semantic-release.yml
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 m23-1.2.1/.vscode/settings.json
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 m23-1.2.1/src/m23/__init__.py
--rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 m23-1.2.1/src/m23/__main__.py
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 m23-1.2.1/src/m23/constants.py
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 m23-1.2.1/src/m23/align/__init__.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 m23-1.2.1/src/m23/calibrate/__init__.py
--rw-r--r--   0        0        0     7980 2020-02-02 00:00:00.000000 m23-1.2.1/src/m23/calibrate/calibration.py
--rw-r--r--   0        0        0     4486 2020-02-02 00:00:00.000000 m23-1.2.1/src/m23/calibrate/master_calibrate.py
--rw-r--r--   0        0        0     6966 2020-02-02 00:00:00.000000 m23-1.2.1/src/m23/charts/__init__.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 m23-1.2.1/src/m23/combine/__init__.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 m23-1.2.1/src/m23/exceptions/__init__.py
--rw-r--r--   0        0        0     8607 2020-02-02 00:00:00.000000 m23-1.2.1/src/m23/extract/__init__.py
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 m23-1.2.1/src/m23/file/__init__.py
--rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 m23-1.2.1/src/m23/file/aligned_combined_file.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 m23-1.2.1/src/m23/file/alignment_stats_file.py
--rw-r--r--   0        0        0     4232 2020-02-02 00:00:00.000000 m23-1.2.1/src/m23/file/color_normalized_file.py
--rw-r--r--   0        0        0    12074 2020-02-02 00:00:00.000000 m23-1.2.1/src/m23/file/flux_log_combined_file.py
--rw-r--r--   0        0        0     9248 2020-02-02 00:00:00.000000 m23-1.2.1/src/m23/file/log_file_combined_file.py
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 m23-1.2.1/src/m23/file/masterflat_file.py
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 m23-1.2.1/src/m23/file/normfactor_file.py
--rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 m23-1.2.1/src/m23/file/raw_image_file.py
--rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 m23-1.2.1/src/m23/file/reference_log_file.py
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 m23-1.2.1/src/m23/file/ri_color_file.py
--rw-r--r--   0        0        0     5527 2020-02-02 00:00:00.000000 m23-1.2.1/src/m23/file/sky_bg_file.py
--rw-r--r--   0        0        0    21812 2020-02-02 00:00:00.000000 m23-1.2.1/src/m23/internight_normalize/__init__.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 m23-1.2.1/src/m23/matrix/__init__.py
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 m23-1.2.1/src/m23/matrix/crop.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 m23-1.2.1/src/m23/matrix/fill.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 m23-1.2.1/src/m23/matrix/region.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 m23-1.2.1/src/m23/matrix/utils.py
--rw-r--r--   0        0        0     7926 2020-02-02 00:00:00.000000 m23-1.2.1/src/m23/norm/__init__.py
--rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 m23-1.2.1/src/m23/norm/get_line.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 m23-1.2.1/src/m23/processor/__init__.py
--rw-r--r--   0        0        0    16157 2020-02-02 00:00:00.000000 m23-1.2.1/src/m23/processor/config_loader.py
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 m23-1.2.1/src/m23/processor/generate_masterflat.py
--rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 m23-1.2.1/src/m23/processor/generate_masterflat_config_loader.py
--rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 m23-1.2.1/src/m23/processor/nights_csv.py
--rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 m23-1.2.1/src/m23/processor/nights_csv_config_loader.py
--rw-r--r--   0        0        0    22276 2020-02-02 00:00:00.000000 m23-1.2.1/src/m23/processor/process_nights.py
--rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 m23-1.2.1/src/m23/processor/renormalize.py
--rw-r--r--   0        0        0     7499 2020-02-02 00:00:00.000000 m23-1.2.1/src/m23/processor/renormalize_config_loader.py
--rw-r--r--   0        0        0   725365 2020-02-02 00:00:00.000000 m23-1.2.1/src/m23/reference/08-05-03_m23_3.5-071.txt
--rw-r--r--   0        0        0    18521 2020-02-02 00:00:00.000000 m23-1.2.1/src/m23/reference/MeanRI100.txt
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 m23-1.2.1/src/m23/reference/README.md
--rw-r--r--   0        0        0   191836 2020-02-02 00:00:00.000000 m23-1.2.1/src/m23/reference/ref_revised_71.txt
--rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 m23-1.2.1/src/m23/sky/__init__.py
--rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 m23-1.2.1/src/m23/sky/moon/__init__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 m23-1.2.1/src/m23/trans/__init__.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 m23-1.2.1/src/m23/trans/fits.py
--rw-r--r--   0        0        0     6839 2020-02-02 00:00:00.000000 m23-1.2.1/src/m23/utils/__init__.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 m23-1.2.1/src/m23/utils/date.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 m23-1.2.1/src/m23/utils/flux_to_magnitude.py
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 m23-1.2.1/src/m23/utils/rename.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 m23-1.2.1/tests/__init__.py
--rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 m23-1.2.1/.gitignore
--rw-r--r--   0        0        0    13309 2020-02-02 00:00:00.000000 m23-1.2.1/README.md
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 m23-1.2.1/pyproject.toml
--rw-r--r--   0        0        0    13681 2020-02-02 00:00:00.000000 m23-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 m23-1.2.2/.flake8
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 m23-1.2.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 m23-1.2.2/brown.toml
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 m23-1.2.2/mf.toml
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 m23-1.2.2/nights_csv.toml
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 m23-1.2.2/rainbow.toml
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 m23-1.2.2/renormalize.toml
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 m23-1.2.2/requirements.txt
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 m23-1.2.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 m23-1.2.2/.github/workflows/semantic-release.yml
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 m23-1.2.2/.vscode/settings.json
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 m23-1.2.2/src/m23/__init__.py
+-rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 m23-1.2.2/src/m23/__main__.py
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 m23-1.2.2/src/m23/constants.py
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 m23-1.2.2/src/m23/align/__init__.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 m23-1.2.2/src/m23/calibrate/__init__.py
+-rw-r--r--   0        0        0     7980 2020-02-02 00:00:00.000000 m23-1.2.2/src/m23/calibrate/calibration.py
+-rw-r--r--   0        0        0     4486 2020-02-02 00:00:00.000000 m23-1.2.2/src/m23/calibrate/master_calibrate.py
+-rw-r--r--   0        0        0     6966 2020-02-02 00:00:00.000000 m23-1.2.2/src/m23/charts/__init__.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 m23-1.2.2/src/m23/combine/__init__.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 m23-1.2.2/src/m23/exceptions/__init__.py
+-rw-r--r--   0        0        0     8607 2020-02-02 00:00:00.000000 m23-1.2.2/src/m23/extract/__init__.py
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 m23-1.2.2/src/m23/file/__init__.py
+-rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 m23-1.2.2/src/m23/file/aligned_combined_file.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 m23-1.2.2/src/m23/file/alignment_stats_file.py
+-rw-r--r--   0        0        0     4232 2020-02-02 00:00:00.000000 m23-1.2.2/src/m23/file/color_normalized_file.py
+-rw-r--r--   0        0        0    12074 2020-02-02 00:00:00.000000 m23-1.2.2/src/m23/file/flux_log_combined_file.py
+-rw-r--r--   0        0        0     9248 2020-02-02 00:00:00.000000 m23-1.2.2/src/m23/file/log_file_combined_file.py
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 m23-1.2.2/src/m23/file/masterflat_file.py
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 m23-1.2.2/src/m23/file/normfactor_file.py
+-rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 m23-1.2.2/src/m23/file/raw_image_file.py
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 m23-1.2.2/src/m23/file/reference_log_file.py
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 m23-1.2.2/src/m23/file/ri_color_file.py
+-rw-r--r--   0        0        0     5527 2020-02-02 00:00:00.000000 m23-1.2.2/src/m23/file/sky_bg_file.py
+-rw-r--r--   0        0        0    21812 2020-02-02 00:00:00.000000 m23-1.2.2/src/m23/internight_normalize/__init__.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 m23-1.2.2/src/m23/matrix/__init__.py
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 m23-1.2.2/src/m23/matrix/crop.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 m23-1.2.2/src/m23/matrix/fill.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 m23-1.2.2/src/m23/matrix/region.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 m23-1.2.2/src/m23/matrix/utils.py
+-rw-r--r--   0        0        0     7926 2020-02-02 00:00:00.000000 m23-1.2.2/src/m23/norm/__init__.py
+-rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 m23-1.2.2/src/m23/norm/get_line.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 m23-1.2.2/src/m23/processor/__init__.py
+-rw-r--r--   0        0        0    16157 2020-02-02 00:00:00.000000 m23-1.2.2/src/m23/processor/config_loader.py
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 m23-1.2.2/src/m23/processor/generate_masterflat.py
+-rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 m23-1.2.2/src/m23/processor/generate_masterflat_config_loader.py
+-rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 m23-1.2.2/src/m23/processor/nights_csv.py
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 m23-1.2.2/src/m23/processor/nights_csv_config_loader.py
+-rw-r--r--   0        0        0    22296 2020-02-02 00:00:00.000000 m23-1.2.2/src/m23/processor/process_nights.py
+-rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 m23-1.2.2/src/m23/processor/renormalize.py
+-rw-r--r--   0        0        0     7499 2020-02-02 00:00:00.000000 m23-1.2.2/src/m23/processor/renormalize_config_loader.py
+-rw-r--r--   0        0        0   725365 2020-02-02 00:00:00.000000 m23-1.2.2/src/m23/reference/08-05-03_m23_3.5-071.txt
+-rw-r--r--   0        0        0    18521 2020-02-02 00:00:00.000000 m23-1.2.2/src/m23/reference/MeanRI100.txt
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 m23-1.2.2/src/m23/reference/README.md
+-rw-r--r--   0        0        0   191836 2020-02-02 00:00:00.000000 m23-1.2.2/src/m23/reference/ref_revised_71.txt
+-rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 m23-1.2.2/src/m23/sky/__init__.py
+-rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 m23-1.2.2/src/m23/sky/moon/__init__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 m23-1.2.2/src/m23/trans/__init__.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 m23-1.2.2/src/m23/trans/fits.py
+-rw-r--r--   0        0        0     6839 2020-02-02 00:00:00.000000 m23-1.2.2/src/m23/utils/__init__.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 m23-1.2.2/src/m23/utils/date.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 m23-1.2.2/src/m23/utils/flux_to_magnitude.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 m23-1.2.2/src/m23/utils/rename.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 m23-1.2.2/tests/__init__.py
+-rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 m23-1.2.2/.gitignore
+-rw-r--r--   0        0        0    13474 2020-02-02 00:00:00.000000 m23-1.2.2/README.md
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 m23-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0    13846 2020-02-02 00:00:00.000000 m23-1.2.2/PKG-INFO
```

### Comparing `m23-1.2.1/CHANGELOG.md` & `m23-1.2.2/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.2.2 (2023-06-22)
+
+### Fix
+
+* Error during sky bg generation ([`2cd4b47`](https://github.com/LutherAstrophysics/m23/commit/2cd4b47f7b4bd4b3f0bc03a6b995920c57be61fa))
+
+### Documentation
+
+* Add photo illustrating commit subjects ([`c2819c6`](https://github.com/LutherAstrophysics/m23/commit/c2819c67846b4e218575b1d8e8c46a5528c7fa56))
+
 ## v1.2.1 (2023-06-21)
 
 ### Fix
 
 * Masterflat generation bug ([`4c47ca2`](https://github.com/LutherAstrophysics/m23/commit/4c47ca27ae812a95dc164896fd3e67fda0498acd))
 
 ## v1.2.0 (2023-06-21)
```

### Comparing `m23-1.2.1/brown.toml` & `m23-1.2.2/brown.toml`

 * *Files identical despite different names*

### Comparing `m23-1.2.1/mf.toml` & `m23-1.2.2/mf.toml`

 * *Files identical despite different names*

### Comparing `m23-1.2.1/nights_csv.toml` & `m23-1.2.2/nights_csv.toml`

 * *Files identical despite different names*

### Comparing `m23-1.2.1/rainbow.toml` & `m23-1.2.2/rainbow.toml`

 * *Files identical despite different names*

### Comparing `m23-1.2.1/requirements.txt` & `m23-1.2.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `m23-1.2.1/.github/workflows/python-publish.yml` & `m23-1.2.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `m23-1.2.1/.vscode/settings.json` & `m23-1.2.2/.vscode/settings.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992063492063492%*

 * *Differences: {"'cSpell.words'": "{insert: [(52, 'starttime')]}"}*

```diff
@@ -54,14 +54,15 @@
         "Renormalize",
         "reslife",
         "rown",
         "savefig",
         "savetxt",
         "scipy",
         "setuptools",
+        "starttime",
         "tuti",
         "venv",
         "writeto",
         "XFWHM",
         "xlabel",
         "xlim",
         "yaspin",
```

### Comparing `m23-1.2.1/src/m23/__main__.py` & `m23-1.2.2/src/m23/__main__.py`

 * *Files identical despite different names*

### Comparing `m23-1.2.1/src/m23/constants.py` & `m23-1.2.2/src/m23/constants.py`

 * *Files identical despite different names*

### Comparing `m23-1.2.1/src/m23/align/__init__.py` & `m23-1.2.2/src/m23/align/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.2.1/src/m23/calibrate/calibration.py` & `m23-1.2.2/src/m23/calibrate/calibration.py`

 * *Files identical despite different names*

### Comparing `m23-1.2.1/src/m23/calibrate/master_calibrate.py` & `m23-1.2.2/src/m23/calibrate/master_calibrate.py`

 * *Files identical despite different names*

### Comparing `m23-1.2.1/src/m23/charts/__init__.py` & `m23-1.2.2/src/m23/charts/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.2.1/src/m23/combine/__init__.py` & `m23-1.2.2/src/m23/combine/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.2.1/src/m23/extract/__init__.py` & `m23-1.2.2/src/m23/extract/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.2.1/src/m23/file/__init__.py` & `m23-1.2.2/src/m23/file/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.2.1/src/m23/file/aligned_combined_file.py` & `m23-1.2.2/src/m23/file/aligned_combined_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.2.1/src/m23/file/alignment_stats_file.py` & `m23-1.2.2/src/m23/file/alignment_stats_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.2.1/src/m23/file/color_normalized_file.py` & `m23-1.2.2/src/m23/file/color_normalized_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.2.1/src/m23/file/flux_log_combined_file.py` & `m23-1.2.2/src/m23/file/flux_log_combined_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.2.1/src/m23/file/log_file_combined_file.py` & `m23-1.2.2/src/m23/file/log_file_combined_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.2.1/src/m23/file/masterflat_file.py` & `m23-1.2.2/src/m23/file/masterflat_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.2.1/src/m23/file/normfactor_file.py` & `m23-1.2.2/src/m23/file/normfactor_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.2.1/src/m23/file/raw_image_file.py` & `m23-1.2.2/src/m23/file/raw_image_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.2.1/src/m23/file/reference_log_file.py` & `m23-1.2.2/src/m23/file/reference_log_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.2.1/src/m23/file/ri_color_file.py` & `m23-1.2.2/src/m23/file/ri_color_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.2.1/src/m23/file/sky_bg_file.py` & `m23-1.2.2/src/m23/file/sky_bg_file.py`

 * *Files identical despite different names*

### Comparing `m23-1.2.1/src/m23/internight_normalize/__init__.py` & `m23-1.2.2/src/m23/internight_normalize/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.2.1/src/m23/matrix/fill.py` & `m23-1.2.2/src/m23/matrix/fill.py`

 * *Files identical despite different names*

### Comparing `m23-1.2.1/src/m23/norm/__init__.py` & `m23-1.2.2/src/m23/norm/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.2.1/src/m23/norm/get_line.py` & `m23-1.2.2/src/m23/norm/get_line.py`

 * *Files identical despite different names*

### Comparing `m23-1.2.1/src/m23/processor/config_loader.py` & `m23-1.2.2/src/m23/processor/config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-1.2.1/src/m23/processor/generate_masterflat.py` & `m23-1.2.2/src/m23/processor/generate_masterflat.py`

 * *Files identical despite different names*

### Comparing `m23-1.2.1/src/m23/processor/generate_masterflat_config_loader.py` & `m23-1.2.2/src/m23/processor/generate_masterflat_config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-1.2.1/src/m23/processor/nights_csv.py` & `m23-1.2.2/src/m23/processor/nights_csv.py`

 * *Files identical despite different names*

### Comparing `m23-1.2.1/src/m23/processor/nights_csv_config_loader.py` & `m23-1.2.2/src/m23/processor/nights_csv_config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-1.2.1/src/m23/processor/process_nights.py` & `m23-1.2.2/src/m23/processor/process_nights.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,15 +163,15 @@
     normfactors: Dictionary of normfactors for various radii of extraction
 
     """
     logger = logging.getLogger("LOGGER_" + str(night_date))
     logger.info("Generating sky background file")
     bg_data_of_all_images = []
 
-    for logfile in enumerate(log_files_to_use):
+    for logfile in log_files_to_use:
         date_time_of_image = logfile.datetime()
         # Here we find the corresponding aligned combined file first
         # so we can use that to calculate the sky bg data.
         aligned_combined_folder = logfile.path().parent.parent / ALIGNED_COMBINED_FOLDER_NAME
         aligned_combined_file_name = AlignedCombinedFile.generate_file_name(
             logfile.img_duration(), logfile.img_number()
         )
@@ -320,21 +320,23 @@
     )
     logger.info("Created master dark")
     del darks  # Deleting to free memory as we don't use darks anymore
 
     # Flats
     if night.get("masterflat"):
         master_flat_data = getdata(night["masterflat"])
-        # Copy the masteflat provided to the calibration frames
+        # Copy the masterflat provided to the calibration frames
         masterflat_path = Path(night["masterflat"])
         shutil.copy(masterflat_path, CALIBRATION_OUTPUT_FOLDER)
         logger.info("Using pre-provided masterflat")
     else:
         # Note the order is important when generating masterflat
-        flats = fit_data_from_fit_images(sorted_by_number(get_flats(NIGHT_INPUT_CALIBRATION_FOLDER)))
+        flats = fit_data_from_fit_images(
+            sorted_by_number(get_flats(NIGHT_INPUT_CALIBRATION_FOLDER))
+        )  # noqa
         # Ensure that image dimensions are as specified by rows and cols
         # If there's extra noise cols or rows, we crop them
         flats = [crop(matrix, rows, cols) for matrix in flats]
 
         master_flat_data = makeMasterFlat(
             saveAs=CALIBRATION_OUTPUT_FOLDER / MasterflatFile.generate_file_name(night_date),
             masterDarkData=master_dark_data,
```

### Comparing `m23-1.2.1/src/m23/processor/renormalize.py` & `m23-1.2.2/src/m23/processor/renormalize.py`

 * *Files identical despite different names*

### Comparing `m23-1.2.1/src/m23/processor/renormalize_config_loader.py` & `m23-1.2.2/src/m23/processor/renormalize_config_loader.py`

 * *Files identical despite different names*

### Comparing `m23-1.2.1/src/m23/reference/08-05-03_m23_3.5-071.txt` & `m23-1.2.2/src/m23/reference/08-05-03_m23_3.5-071.txt`

 * *Files identical despite different names*

### Comparing `m23-1.2.1/src/m23/reference/MeanRI100.txt` & `m23-1.2.2/src/m23/reference/MeanRI100.txt`

 * *Files identical despite different names*

### Comparing `m23-1.2.1/src/m23/reference/README.md` & `m23-1.2.2/src/m23/reference/README.md`

 * *Files identical despite different names*

### Comparing `m23-1.2.1/src/m23/reference/ref_revised_71.txt` & `m23-1.2.2/src/m23/reference/ref_revised_71.txt`

 * *Files identical despite different names*

### Comparing `m23-1.2.1/src/m23/sky/__init__.py` & `m23-1.2.2/src/m23/sky/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.2.1/src/m23/sky/moon/__init__.py` & `m23-1.2.2/src/m23/sky/moon/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.2.1/src/m23/utils/__init__.py` & `m23-1.2.2/src/m23/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `m23-1.2.1/src/m23/utils/date.py` & `m23-1.2.2/src/m23/utils/date.py`

 * *Files identical despite different names*

### Comparing `m23-1.2.1/src/m23/utils/rename.py` & `m23-1.2.2/src/m23/utils/rename.py`

 * *Files identical despite different names*

### Comparing `m23-1.2.1/.gitignore` & `m23-1.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `m23-1.2.1/README.md` & `m23-1.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -280,11 +280,14 @@
 commit message must be followed by one of the few special keywords:
 
 1. "chore" for chore tasks
 1. "docs" for documentation related commits
 1. "feat" for new feature
 1. "fix" for bugfix
 
+and couple others:
+![screenshot of summary of valid commitizen commits](https://raw.githubusercontent.com/commitizen/cz-cli/master/meta/screenshots/add-commit.png)
+
 Note that if any of your commits make breaking changes, your commit message must
 also contain the phrase "BREAKING CHANGE". This will trigger a major version
 update. See some of the previous commit messages for more information and feel
 free too ask if you have confusion.
```

### Comparing `m23-1.2.1/pyproject.toml` & `m23-1.2.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "m23"
 readme = "README.md"
 requires-python = ">=3.10"
-version = "1.2.1"
+version = "1.2.2"
 dependencies = [
     "numpy==1.24.2",
     'toml==0.10.2',
     'astropy==5.2.1',
     'astroalign==2.4.1',
     'typing_extensions==4.4.0',
     'opencv-python==4.7.0.68',
```

### Comparing `m23-1.2.1/PKG-INFO` & `m23-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m23
-Version: 1.2.1
+Version: 1.2.2
 Requires-Python: >=3.10
 Requires-Dist: astroalign==2.4.1
 Requires-Dist: astropy==5.2.1
 Requires-Dist: ephem==4.1.4
 Requires-Dist: matplotlib==3.7.0
 Requires-Dist: numpy==1.24.2
 Requires-Dist: opencv-python==4.7.0.68
@@ -294,11 +294,14 @@
 commit message must be followed by one of the few special keywords:
 
 1. "chore" for chore tasks
 1. "docs" for documentation related commits
 1. "feat" for new feature
 1. "fix" for bugfix
 
+and couple others:
+![screenshot of summary of valid commitizen commits](https://raw.githubusercontent.com/commitizen/cz-cli/master/meta/screenshots/add-commit.png)
+
 Note that if any of your commits make breaking changes, your commit message must
 also contain the phrase "BREAKING CHANGE". This will trigger a major version
 update. See some of the previous commit messages for more information and feel
 free too ask if you have confusion.
```

