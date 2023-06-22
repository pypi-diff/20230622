# Comparing `tmp/pystemmusscope-0.2.1.tar.gz` & `tmp/pystemmusscope-0.3.0.tar.gz`

## Comparing `pystemmusscope-0.2.1.tar` & `pystemmusscope-0.3.0.tar`

### file list

```diff
@@ -1,57 +1,61 @@
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/.bumpversion.cfg
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/.editorconfig
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/.mlc-config.json
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/.readthedocs.yaml
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/CITATION.cff
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/environment.yml
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/mkdocs.yml
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/run_jupyter_lab_snellius.sh
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/PyStemmusScope/__init__.py
--rw-r--r--   0        0        0     5261 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/PyStemmusScope/config_io.py
--rw-r--r--   0        0        0    11234 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/PyStemmusScope/forcing_io.py
--rw-r--r--   0        0        0    10766 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/PyStemmusScope/save.py
--rw-r--r--   0        0        0    13211 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/PyStemmusScope/soil_io.py
--rw-r--r--   0        0        0     8036 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/PyStemmusScope/stemmus_scope.py
--rw-r--r--   0        0        0     6958 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/PyStemmusScope/utils.py
--rw-r--r--   0        0        0     5745 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/PyStemmusScope/variable_conversion.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/PyStemmusScope/global_data/__init__.py
--rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/PyStemmusScope/global_data/cams_co2.py
--rw-r--r--   0        0        0     6154 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/PyStemmusScope/global_data/cci_landcover.py
--rw-r--r--   0        0        0     4513 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/PyStemmusScope/global_data/copernicus_lai.py
--rw-r--r--   0        0        0     6935 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/PyStemmusScope/global_data/era5.py
--rw-r--r--   0        0        0     3865 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/PyStemmusScope/global_data/eth_canopy_height.py
--rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/PyStemmusScope/global_data/global_data_selection.py
--rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/PyStemmusScope/global_data/prism_dem.py
--rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/PyStemmusScope/global_data/utils.py
--rw-r--r--   0        0        0    98915 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/PyStemmusScope/global_data/assets/dem_filenames_compressed.txt.gz
--rw-r--r--   0        0        0     7268 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/PyStemmusScope/global_data/assets/h_canopy_filenames_compressed.txt.gz
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/PyStemmusScope/global_data/assets/lccs_to_igbp_table.csv
--rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/docs/CHANGELOG.md
--rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/docs/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/docs/CONTRIBUTING.md
--rw-r--r--   0        0        0     6285 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/docs/README.dev.md
--rw-r--r--   0        0        0    87342 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/docs/ecoextreml_logo.png
--rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/docs/index.md
--rw-r--r--   0        0        0     4903 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/docs/installation_instructions.md
--rw-r--r--   0        0        0     6036 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/docs/project_setup.md
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/docs/reference.md
--rw-r--r--   0        0        0    12340 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/docs/notebooks/run_model_in_notebook.ipynb
--rw-r--r--   0        0        0    14535 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/docs/notebooks/verify_model_modifications.ipynb
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/docs/overrides/main.html
--rw-r--r--   0        0        0     3579 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/global_data/downloading_global_data.md
--rw-r--r--   0        0        0    63044 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/global_data/data_analysis_notebooks/compare_global_data.ipynb
--rw-r--r--   0        0        0   149768 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/global_data/data_analysis_notebooks/parse_CO2_data.ipynb
--rw-r--r--   0        0        0   235247 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/global_data/data_analysis_notebooks/parse_LAI.ipynb
--rw-r--r--   0        0        0   138298 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/global_data/data_analysis_notebooks/parse_canopy_height.ipynb
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/global_data/data_analysis_notebooks/parse_dem.ipynb
--rw-r--r--   0        0        0    60173 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/global_data/data_analysis_notebooks/parse_era5_data.ipynb
--rw-r--r--   0        0        0    31695 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/global_data/data_analysis_notebooks/parse_landcover.ipynb
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/global_data/download_scripts/download_CAMS_CO2.py
--rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/global_data/download_scripts/download_FAPAR_LAI.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/global_data/download_scripts/download_cds_landcover.py
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/global_data/download_scripts/download_era5land_monthly.py
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/LICENSE
--rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/README.md
--rw-r--r--   0        0        0     4550 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 pystemmusscope-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/.bumpversion.cfg
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/.editorconfig
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/.mlc-config.json
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/.readthedocs.yaml
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/CITATION.cff
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/environment.yml
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/mkdocs.yml
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/run_jupyter_lab_snellius.sh
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/PyStemmusScope/__init__.py
+-rw-r--r--   0        0        0     5261 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/PyStemmusScope/config_io.py
+-rw-r--r--   0        0        0    11246 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/PyStemmusScope/forcing_io.py
+-rw-r--r--   0        0        0    10766 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/PyStemmusScope/save.py
+-rw-r--r--   0        0        0    13211 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/PyStemmusScope/soil_io.py
+-rw-r--r--   0        0        0     8036 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/PyStemmusScope/stemmus_scope.py
+-rw-r--r--   0        0        0     6958 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/PyStemmusScope/utils.py
+-rw-r--r--   0        0        0     5745 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/PyStemmusScope/variable_conversion.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/PyStemmusScope/global_data/__init__.py
+-rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/PyStemmusScope/global_data/cams_co2.py
+-rw-r--r--   0        0        0     6154 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/PyStemmusScope/global_data/cci_landcover.py
+-rw-r--r--   0        0        0     4513 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/PyStemmusScope/global_data/copernicus_lai.py
+-rw-r--r--   0        0        0     6935 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/PyStemmusScope/global_data/era5.py
+-rw-r--r--   0        0        0     3865 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/PyStemmusScope/global_data/eth_canopy_height.py
+-rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/PyStemmusScope/global_data/global_data_selection.py
+-rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/PyStemmusScope/global_data/prism_dem.py
+-rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/PyStemmusScope/global_data/utils.py
+-rw-r--r--   0        0        0    98915 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/PyStemmusScope/global_data/assets/dem_filenames_compressed.txt.gz
+-rw-r--r--   0        0        0     7268 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/PyStemmusScope/global_data/assets/h_canopy_filenames_compressed.txt.gz
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/PyStemmusScope/global_data/assets/lccs_to_igbp_table.csv
+-rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/docs/CHANGELOG.md
+-rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/docs/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/docs/CONTRIBUTING.md
+-rw-r--r--   0        0        0     6285 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/docs/README.dev.md
+-rw-r--r--   0        0        0    87342 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/docs/ecoextreml_logo.png
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/docs/index.md
+-rw-r--r--   0        0        0     4903 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/docs/installation_instructions.md
+-rw-r--r--   0        0        0     6036 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/docs/project_setup.md
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/docs/reference.md
+-rw-r--r--   0        0        0  1007593 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/docs/notebooks/compare_git_branch_results_.ipynb
+-rw-r--r--   0        0        0    12340 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/docs/notebooks/run_model_in_notebook.ipynb
+-rw-r--r--   0        0        0    12491 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/docs/notebooks/run_model_in_notebook_bart.ipynb
+-rw-r--r--   0        0        0    40217 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/docs/notebooks/test.ipynb
+-rw-r--r--   0        0        0    14535 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/docs/notebooks/verify_model_modifications.ipynb
+-rw-r--r--   0        0        0    16407 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/docs/notebooks/verify_model_modifications_bart.ipynb
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/docs/overrides/main.html
+-rw-r--r--   0        0        0     3579 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/global_data/downloading_global_data.md
+-rw-r--r--   0        0        0    63044 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/global_data/data_analysis_notebooks/compare_global_data.ipynb
+-rw-r--r--   0        0        0   149768 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/global_data/data_analysis_notebooks/parse_CO2_data.ipynb
+-rw-r--r--   0        0        0   235247 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/global_data/data_analysis_notebooks/parse_LAI.ipynb
+-rw-r--r--   0        0        0   138298 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/global_data/data_analysis_notebooks/parse_canopy_height.ipynb
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/global_data/data_analysis_notebooks/parse_dem.ipynb
+-rw-r--r--   0        0        0    60173 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/global_data/data_analysis_notebooks/parse_era5_data.ipynb
+-rw-r--r--   0        0        0    31695 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/global_data/data_analysis_notebooks/parse_landcover.ipynb
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/global_data/download_scripts/download_CAMS_CO2.py
+-rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/global_data/download_scripts/download_FAPAR_LAI.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/global_data/download_scripts/download_cds_landcover.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/global_data/download_scripts/download_era5land_monthly.py
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/README.md
+-rw-r--r--   0        0        0     4550 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 pystemmusscope-0.3.0/PKG-INFO
```

### Comparing `pystemmusscope-0.2.1/.mlc-config.json` & `pystemmusscope-0.3.0/.mlc-config.json`

 * *Files identical despite different names*

### Comparing `pystemmusscope-0.2.1/CITATION.cff` & `pystemmusscope-0.3.0/CITATION.cff`

 * *Files 14% similar despite different names*

```diff
@@ -16,14 +16,14 @@
   -
     affiliation: "Netherlands eScience Center"
     family-names: Liu
     given-names: Yang
     orcid: "https://orcid.org/0000-0002-1966-8460"
 date-released: 2022-11-24
 doi: <insert your DOI here>
-version: "0.2.1"
+version: "0.3.0"
 repository-code: "https://github.com/EcoExtreML/stemmus_scope_processing"
 keywords:
   - STEMMUS SCOPE Processing
   - python
 message: "If you use this software, please cite it using these metadata."
 license: Apache-2.0
```

### Comparing `pystemmusscope-0.2.1/mkdocs.yml` & `pystemmusscope-0.3.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pystemmusscope-0.2.1/run_jupyter_lab_snellius.sh` & `pystemmusscope-0.3.0/run_jupyter_lab_snellius.sh`

 * *Files identical despite different names*

### Comparing `pystemmusscope-0.2.1/PyStemmusScope/config_io.py` & `pystemmusscope-0.3.0/PyStemmusScope/config_io.py`

 * *Files identical despite different names*

### Comparing `pystemmusscope-0.2.1/PyStemmusScope/forcing_io.py` & `pystemmusscope-0.3.0/PyStemmusScope/forcing_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,17 @@
     ) / np.timedelta64(1, "s")
     data["DELT"] = time_delta.astype(float)
     data["total_timesteps"] = ds_forcing.time.size
 
     data["latitude"] = ds_forcing["latitude"].values
     data["longitude"] = ds_forcing["longitude"].values
     data["elevation"] = ds_forcing["elevation"].values
-    data["IGBP_veg_long"] = ds_forcing["IGBP_veg_long"].values
+    data["IGBP_veg_long"] = np.repeat(
+        ds_forcing["IGBP_veg_long"].values, ds_forcing.time.size
+    ).T
     data["reference_height"] = ds_forcing["reference_height"].values
     data["canopy_height"] = ds_forcing["canopy_height"].values
 
     # these are needed by save.py
     data["time"] = ds_forcing["time"]
     data["Qair"] = ds_forcing["Qair"]
 
@@ -205,29 +207,27 @@
     'forcing_globals.mat' in the specified input directory.
 
     Args:
         data: Dictionary containing the required variables. Generated by the
             function `read_forcing_data`.
         input_path: Path to which the file should be written to.
     """
-    total_duration = data["total_timesteps"]
-
     matfile_vars = [
         "latitude",
         "longitude",
         "elevation",
         "IGBP_veg_long",
         "reference_height",
         "canopy_height",
         "DELT",
         "sitename",
     ]
     matfiledata = {key: data[key] for key in matfile_vars}
 
-    matfiledata["Dur_tot"] = float(total_duration)  # Matlab expects a 'double'
+    matfiledata["Dur_tot"] = float(data["total_timesteps"])  # Matlab expects a 'double'
 
     hdf5storage.savemat(
         input_path / "forcing_globals.mat", matfiledata, appendmat=False
     )
     utils.remove_dates_from_header(input_path / "forcing_globals.mat")
```

### Comparing `pystemmusscope-0.2.1/PyStemmusScope/save.py` & `pystemmusscope-0.3.0/PyStemmusScope/save.py`

 * *Files identical despite different names*

### Comparing `pystemmusscope-0.2.1/PyStemmusScope/soil_io.py` & `pystemmusscope-0.3.0/PyStemmusScope/soil_io.py`

 * *Files identical despite different names*

### Comparing `pystemmusscope-0.2.1/PyStemmusScope/stemmus_scope.py` & `pystemmusscope-0.3.0/PyStemmusScope/stemmus_scope.py`

 * *Files identical despite different names*

### Comparing `pystemmusscope-0.2.1/PyStemmusScope/utils.py` & `pystemmusscope-0.3.0/PyStemmusScope/utils.py`

 * *Files identical despite different names*

### Comparing `pystemmusscope-0.2.1/PyStemmusScope/variable_conversion.py` & `pystemmusscope-0.3.0/PyStemmusScope/variable_conversion.py`

 * *Files identical despite different names*

### Comparing `pystemmusscope-0.2.1/PyStemmusScope/global_data/__init__.py` & `pystemmusscope-0.3.0/PyStemmusScope/global_data/__init__.py`

 * *Files identical despite different names*

### Comparing `pystemmusscope-0.2.1/PyStemmusScope/global_data/cams_co2.py` & `pystemmusscope-0.3.0/PyStemmusScope/global_data/cams_co2.py`

 * *Files identical despite different names*

### Comparing `pystemmusscope-0.2.1/PyStemmusScope/global_data/cci_landcover.py` & `pystemmusscope-0.3.0/PyStemmusScope/global_data/cci_landcover.py`

 * *Files identical despite different names*

### Comparing `pystemmusscope-0.2.1/PyStemmusScope/global_data/copernicus_lai.py` & `pystemmusscope-0.3.0/PyStemmusScope/global_data/copernicus_lai.py`

 * *Files identical despite different names*

### Comparing `pystemmusscope-0.2.1/PyStemmusScope/global_data/era5.py` & `pystemmusscope-0.3.0/PyStemmusScope/global_data/era5.py`

 * *Files identical despite different names*

### Comparing `pystemmusscope-0.2.1/PyStemmusScope/global_data/eth_canopy_height.py` & `pystemmusscope-0.3.0/PyStemmusScope/global_data/eth_canopy_height.py`

 * *Files identical despite different names*

### Comparing `pystemmusscope-0.2.1/PyStemmusScope/global_data/global_data_selection.py` & `pystemmusscope-0.3.0/PyStemmusScope/global_data/global_data_selection.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,13 +102,11 @@
 
     landcover_data = gd.cci_landcover.retrieve_landcover_data(
         global_data_dir,
         latlon,
         time_range,
         timestep,
     )
-    # TODO see issue github.com/EcoExtreML/STEMMUS_SCOPE/issues/137
-    # for now, we only use the first value of the time series
-    data["IGBP_veg_long"] = landcover_data["IGBP_veg_long"][0]
-    data["LCCS_landcover"] = landcover_data["LCCS_landcover"][0]
+    data["IGBP_veg_long"] = landcover_data["IGBP_veg_long"]
+    data["LCCS_landcover"] = landcover_data["LCCS_landcover"]
 
     return data
```

### Comparing `pystemmusscope-0.2.1/PyStemmusScope/global_data/prism_dem.py` & `pystemmusscope-0.3.0/PyStemmusScope/global_data/prism_dem.py`

 * *Files identical despite different names*

### Comparing `pystemmusscope-0.2.1/PyStemmusScope/global_data/utils.py` & `pystemmusscope-0.3.0/PyStemmusScope/global_data/utils.py`

 * *Files identical despite different names*

### Comparing `pystemmusscope-0.2.1/PyStemmusScope/global_data/assets/dem_filenames_compressed.txt.gz` & `pystemmusscope-0.3.0/PyStemmusScope/global_data/assets/dem_filenames_compressed.txt.gz`

 * *Files identical despite different names*

### Comparing `pystemmusscope-0.2.1/PyStemmusScope/global_data/assets/h_canopy_filenames_compressed.txt.gz` & `pystemmusscope-0.3.0/PyStemmusScope/global_data/assets/h_canopy_filenames_compressed.txt.gz`

 * *Files identical despite different names*

### Comparing `pystemmusscope-0.2.1/PyStemmusScope/global_data/assets/lccs_to_igbp_table.csv` & `pystemmusscope-0.3.0/PyStemmusScope/global_data/assets/lccs_to_igbp_table.csv`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,39 @@
 "lccs_class","IGBP_STEMMUS_SCOPE"
 0,"No vegetation"
 10,"Croplands"
+11,"Croplands"
+12,"Croplands"
 20,"Croplands"
 30,"Cropland mosaics"
 40,"Cropland mosaics"
 50,"Evergreen Broadleaf Forest"
 60,"Deciduous Broadleaf Forests"
+61,"Deciduous Broadleaf Forests"
+62,"Deciduous Broadleaf Forests"
 70,"Evergreen Needleleaf Forests"
+71,"Evergreen Needleleaf Forests"
+72,"Evergreen Needleleaf Forests"
 80,"Deciduous needleleaf forests"
+81,"Deciduous needleleaf forests"
+82,"Deciduous needleleaf forests"
 90,"Mixed Forests"
 100,"Woody savannas"
 110,"Savannas"
 120,"Closed shrublands"
+121,"Closed shrublands"
+122,"Closed shrublands"
 130,"Grasslands"
 140,"Not available in IGBP"
 150,"Open shrublands"
+151,"Open shrublands"
+152,"Open shrublands"
+153,"Open shrublands"
 160,"Permanent Wetlands"
 170,"Permanent Wetlands"
 180,"Permanent Wetlands"
 190,"Urban and built-up lands"
 200,"Barren"
+201,"Barren"
+202,"Barren"
 210,"Water bodies"
 220,"Snow and ice"
```

### Comparing `pystemmusscope-0.2.1/docs/CHANGELOG.md` & `pystemmusscope-0.3.0/docs/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -2,31 +2,46 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
-## [0.2.1] - 2023-04-03
+### Added:
+
+### Removed:
+
+### Changed:
+
+
+## [0.3.0] - 2023-06-21
 <!-- markdown-link-check-disable-next-line -->
+This version is only compatible with [STEMMUS_SCOPE 1.3.0](https://github.com/EcoExtreML/STEMMUS_SCOPE/releases/tag/1.2.0).
+
+### Changed:
+- The landcover type outputs in `forcing_globals.mat` (e.g. `IGBP_veg_long`) are now time dependent, instead of a single constant value ([#84](https://github.com/EcoExtreML/STEMMUS_SCOPE_Processing/pull/84)).
+
+### Fixed:
+- The regional landcover classes from the IGBP classification system are now supported as well ([#80](https://github.com/EcoExtreML/STEMMUS_SCOPE_Processing/pull/80)).
+
+## [0.2.1] - 2023-04-03
 This version is only compatible with [STEMMUS_SCOPE 1.2.0](https://github.com/EcoExtreML/STEMMUS_SCOPE/releases/tag/1.2.0).
 
 ### Added:
 - LAI data can now be read by the global data routines ([#69](https://github.com/EcoExtreML/STEMMUS_SCOPE_Processing/pull/69)).
 - Land cover data can now be read by global data routines ([#73](https://github.com/EcoExtreML/STEMMUS_SCOPE_Processing/pull/73))
 - Data validation checks (file existance, spatial & temporal bounds, ...) to global data read routines ([#71](https://github.com/EcoExtreML/STEMMUS_SCOPE_Processing/pull/71)).
 
 ### Changed:
 - The project has been moved to a `pyproject.toml` + `hatch` setup, with ruff as the linter and mypy as type checker ([#68](https://github.com/EcoExtreML/STEMMUS_SCOPE_Processing/pull/68)).
 
 ### Fixed:
 - The output netcdf file is again compatible to the model evaluation website ([#76](https://github.com/EcoExtreML/STEMMUS_SCOPE_Processing/pull/76)).
 
 ## [0.2.0] - 2023-02-21
-<!-- markdown-link-check-disable-next-line -->
 This version is only compatible with [STEMMUS_SCOPE 1.2.0](https://github.com/EcoExtreML/STEMMUS_SCOPE/releases/tag/1.2.0).
 
 ### Added:
  - A time range can now be specified for which the model should be run.
  - The model can now be run on any site globally, by providing a latitude and longitude, assuming that the required data is available for those sites.
      - Note: land cover and LAI are not dynamically retrieved yet, but use a dummy value.
 
@@ -36,15 +51,13 @@
 ## [0.1.1] - 2022-11-24
 ### Changed:
 - Supported Python versions are now 3.8, 3.9 and 3.10.
 
 ## [0.1.0] - 2022-11-24
 The first release of PyStemmusScope. Compatible with STEMMUS_SCOPE 1.1.11.
 
-### Added
-
-### Removed
-
-### Changed
-
-<!-- [Unreleased]: https://github.com/EcoExtreML/STEMMUS_SCOPE_Processing/compare/v1.0.0...HEAD
-[0.0.1]: https://github.com/EcoExtreML/STEMMUS_SCOPE_Processing/releases/tag/v0.0.1 -->
+[Unreleased]: https://github.com/EcoExtreML/STEMMUS_SCOPE_Processing/compare/v0.3.0...HEAD
+[0.1.0]: https://github.com/EcoExtreML/STEMMUS_SCOPE_Processing/releases/tag/v0.1.0
+[0.1.1]: https://github.com/EcoExtreML/STEMMUS_SCOPE_Processing/releases/tag/v0.1.1
+[0.2.0]: https://github.com/EcoExtreML/STEMMUS_SCOPE_Processing/releases/tag/v0.2.0
+[0.2.1]: https://github.com/EcoExtreML/STEMMUS_SCOPE_Processing/releases/tag/v0.2.1
+[0.3.0]: https://github.com/EcoExtreML/STEMMUS_SCOPE_Processing/releases/tag/v0.3.0
```

### Comparing `pystemmusscope-0.2.1/docs/CODE_OF_CONDUCT.md` & `pystemmusscope-0.3.0/docs/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pystemmusscope-0.2.1/docs/CONTRIBUTING.md` & `pystemmusscope-0.3.0/docs/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pystemmusscope-0.2.1/docs/README.dev.md` & `pystemmusscope-0.3.0/docs/README.dev.md`

 * *Files identical despite different names*

### Comparing `pystemmusscope-0.2.1/docs/ecoextreml_logo.png` & `pystemmusscope-0.3.0/docs/ecoextreml_logo.png`

 * *Files identical despite different names*

### Comparing `pystemmusscope-0.2.1/docs/index.md` & `pystemmusscope-0.3.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `pystemmusscope-0.2.1/docs/installation_instructions.md` & `pystemmusscope-0.3.0/docs/installation_instructions.md`

 * *Files identical despite different names*

### Comparing `pystemmusscope-0.2.1/docs/project_setup.md` & `pystemmusscope-0.3.0/docs/project_setup.md`

 * *Files identical despite different names*

### Comparing `pystemmusscope-0.2.1/docs/reference.md` & `pystemmusscope-0.3.0/docs/reference.md`

 * *Files identical despite different names*

### Comparing `pystemmusscope-0.2.1/docs/notebooks/run_model_in_notebook.ipynb` & `pystemmusscope-0.3.0/docs/notebooks/run_model_in_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `pystemmusscope-0.2.1/docs/notebooks/verify_model_modifications.ipynb` & `pystemmusscope-0.3.0/docs/notebooks/verify_model_modifications.ipynb`

 * *Files identical despite different names*

### Comparing `pystemmusscope-0.2.1/global_data/downloading_global_data.md` & `pystemmusscope-0.3.0/global_data/downloading_global_data.md`

 * *Files identical despite different names*

### Comparing `pystemmusscope-0.2.1/global_data/data_analysis_notebooks/compare_global_data.ipynb` & `pystemmusscope-0.3.0/global_data/data_analysis_notebooks/compare_global_data.ipynb`

 * *Files identical despite different names*

### Comparing `pystemmusscope-0.2.1/global_data/data_analysis_notebooks/parse_CO2_data.ipynb` & `pystemmusscope-0.3.0/global_data/data_analysis_notebooks/parse_CO2_data.ipynb`

 * *Files identical despite different names*

### Comparing `pystemmusscope-0.2.1/global_data/data_analysis_notebooks/parse_LAI.ipynb` & `pystemmusscope-0.3.0/global_data/data_analysis_notebooks/parse_LAI.ipynb`

 * *Files identical despite different names*

### Comparing `pystemmusscope-0.2.1/global_data/data_analysis_notebooks/parse_canopy_height.ipynb` & `pystemmusscope-0.3.0/global_data/data_analysis_notebooks/parse_canopy_height.ipynb`

 * *Files identical despite different names*

### Comparing `pystemmusscope-0.2.1/global_data/data_analysis_notebooks/parse_dem.ipynb` & `pystemmusscope-0.3.0/global_data/data_analysis_notebooks/parse_dem.ipynb`

 * *Files identical despite different names*

### Comparing `pystemmusscope-0.2.1/global_data/data_analysis_notebooks/parse_era5_data.ipynb` & `pystemmusscope-0.3.0/global_data/data_analysis_notebooks/parse_era5_data.ipynb`

 * *Files identical despite different names*

### Comparing `pystemmusscope-0.2.1/global_data/data_analysis_notebooks/parse_landcover.ipynb` & `pystemmusscope-0.3.0/global_data/data_analysis_notebooks/parse_landcover.ipynb`

 * *Files identical despite different names*

### Comparing `pystemmusscope-0.2.1/global_data/download_scripts/download_CAMS_CO2.py` & `pystemmusscope-0.3.0/global_data/download_scripts/download_CAMS_CO2.py`

 * *Files identical despite different names*

### Comparing `pystemmusscope-0.2.1/global_data/download_scripts/download_FAPAR_LAI.py` & `pystemmusscope-0.3.0/global_data/download_scripts/download_FAPAR_LAI.py`

 * *Files identical despite different names*

### Comparing `pystemmusscope-0.2.1/global_data/download_scripts/download_cds_landcover.py` & `pystemmusscope-0.3.0/global_data/download_scripts/download_cds_landcover.py`

 * *Files identical despite different names*

### Comparing `pystemmusscope-0.2.1/global_data/download_scripts/download_era5land_monthly.py` & `pystemmusscope-0.3.0/global_data/download_scripts/download_era5land_monthly.py`

 * *Files identical despite different names*

### Comparing `pystemmusscope-0.2.1/.gitignore` & `pystemmusscope-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pystemmusscope-0.2.1/LICENSE` & `pystemmusscope-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pystemmusscope-0.2.1/README.md` & `pystemmusscope-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pystemmusscope-0.2.1/pyproject.toml` & `pystemmusscope-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pystemmusscope-0.2.1/PKG-INFO` & `pystemmusscope-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyStemmusScope
-Version: 0.2.1
+Version: 0.3.0
 Summary: Python modules for running the STEMMUS-SCOPE model.
 Author: Sarah Alidoost, Bart Schilperoort, Yang Liu
 Author-email: f.alidoost@esciencecenter.nl
 Maintainer-email: Sarah Alidoost <f.alidoost@esciencecenter.nl>, Yang Liu <y.liu@esciencecenter.nl>, Bart Schilperoort <b.schilperoort@esciencecenter.nl>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Keywords: STEMMUS-SCOPE,py
```

