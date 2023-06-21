# Comparing `tmp/alanapy-0.4.tar.gz` & `tmp/alanapy-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alanapy-0.4.tar", last modified: Thu Jun 15 22:56:37 2023, max compression
+gzip compressed data, was "alanapy-0.5.tar", last modified: Wed Jun 21 23:26:38 2023, max compression
```

## Comparing `alanapy-0.4.tar` & `alanapy-0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 22:56:37.214319 alanapy-0.4/
--rw-rw-rw-   0        0        0     1085 2023-06-15 19:50:23.000000 alanapy-0.4/LICENSE
--rw-rw-rw-   0        0        0      634 2023-06-15 22:56:37.214319 alanapy-0.4/PKG-INFO
--rw-rw-rw-   0        0        0        9 2023-06-15 19:50:23.000000 alanapy-0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 22:56:37.184758 alanapy-0.4/alanapy/
--rw-rw-rw-   0        0        0        0 2023-06-15 22:52:11.000000 alanapy-0.4/alanapy/__init__.py
--rw-rw-rw-   0        0        0    71643 2023-06-14 20:40:01.000000 alanapy-0.4/alanapy/alanaAPI.py
-drwxrwxrwx   0        0        0        0 2023-06-15 22:56:37.204350 alanapy-0.4/alanapy.egg-info/
--rw-rw-rw-   0        0        0      634 2023-06-15 22:56:36.000000 alanapy-0.4/alanapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2023-06-15 22:56:36.000000 alanapy-0.4/alanapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 22:56:36.000000 alanapy-0.4/alanapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-06-15 22:56:36.000000 alanapy-0.4/alanapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-15 22:56:36.000000 alanapy-0.4/alanapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 22:56:37.214319 alanapy-0.4/setup.cfg
--rw-rw-rw-   0        0        0      916 2023-06-15 22:56:01.000000 alanapy-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 23:26:38.526949 alanapy-0.5/
+-rw-rw-rw-   0        0        0     1085 2023-06-15 19:50:23.000000 alanapy-0.5/LICENSE
+-rw-rw-rw-   0        0        0      634 2023-06-21 23:26:38.525973 alanapy-0.5/PKG-INFO
+-rw-rw-rw-   0        0        0        9 2023-06-15 19:50:23.000000 alanapy-0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-21 23:26:38.491901 alanapy-0.5/alanapy/
+-rw-rw-rw-   0        0        0        0 2023-06-15 22:52:11.000000 alanapy-0.5/alanapy/__init__.py
+-rw-rw-rw-   0        0        0    71651 2023-06-21 23:20:01.000000 alanapy-0.5/alanapy/alanaAPI.py
+drwxrwxrwx   0        0        0        0 2023-06-21 23:26:38.522959 alanapy-0.5/alanapy.egg-info/
+-rw-rw-rw-   0        0        0      634 2023-06-21 23:26:38.000000 alanapy-0.5/alanapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      220 2023-06-21 23:26:38.000000 alanapy-0.5/alanapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 23:26:38.000000 alanapy-0.5/alanapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-06-21 23:26:38.000000 alanapy-0.5/alanapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-21 23:26:38.000000 alanapy-0.5/alanapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-21 23:26:38.526949 alanapy-0.5/setup.cfg
+-rw-rw-rw-   0        0        0      907 2023-06-21 23:20:04.000000 alanapy-0.5/setup.py
```

### Comparing `alanapy-0.4/LICENSE` & `alanapy-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `alanapy-0.4/PKG-INFO` & `alanapy-0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alanapy
-Version: 0.4
+Version: 0.5
 Home-page: https://github.com/orkahub/alanapy
 Author: Orkahub Energy
 Author-email: orkahub@gmail.com
 License: MIT
 Keywords: RESERVOIR,ENERGY,OIL,GAS,PRODUCTION,PYTHON,ALANA
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `alanapy-0.4/alanapy/alanaAPI.py` & `alanapy-0.5/alanapy/alanaAPI.py`

 * *Files 1% similar despite different names*

```diff
@@ -1712,25 +1712,25 @@
         count_time_to_discard_well_if_zero_rates = 6
         if (dict_dca["str_date_prod"] == "daily") or (dict_dca["str_date_prod"] == "monthly"):
             count_time_to_fit = int(count_time_to_fit * 30.5)
             count_time_to_discard_well_if_zero_rates = int(count_time_to_discard_well_if_zero_rates * 30.5)
         else:
             print("No valid time")
         
-        for n, well_fk in enumerate(list_well_ids):
+        for n, well_fk in enumerate(dict_dca["list_well_names"]):
             if dict_dca["str_date_prod"] == "monthly":
                 well_monthly_dict = {}
-                well_monthly_dict['data'] = mydatasource.getMonthlyProduction(int(well_fk))["data"]
+                well_monthly_dict['data'] = mydatasource.getMonthlyProduction(well_fk)["data"]
                 dates = [x['date'] for x in well_monthly_dict['data']]
                 dates = [datetime.strptime(x, "%Y-%m-%d") for x in dates]
                 rates = [x["oil_rate"] for x in well_monthly_dict['data']]
                 dates_or, rates_or = dates, rates
             elif dict_dca["str_date_prod"] == "daily":
                 well_daily_dict = {}
-                well_daily_dict['data'] = mydatasource.getDailyProduction(int(well_fk))["data"]
+                well_daily_dict['data'] = mydatasource.getDailyProduction(well_fk)["data"]
                 dates = [x['date'] for x in well_daily_dict['data']]
                 dates = [datetime.strptime(x, "%Y-%m-%d") for x in dates]
                 rates = [x["oil_rate"] for x in well_daily_dict['data']]
                 dates_or, rates_or = dates, rates
             else:
                 print("Wrong date frequency")
                 break
@@ -1758,15 +1758,15 @@
                 dca_template_fit_forecast['fc_date_choice'] = "DEFAULT"
                 dca_template_fit_forecast['fc_rate_choice'] = "LASTVALFIT"
                 #print("dca_template_fit_forecast: ",dca_template_fit_forecast)
                 dca_forecast = self.master._fitForecastDCA(dates, rates, dca_template_fit_forecast)
                 # print("dca_forecast: ",dca_forecast)
                 # dca_forecast['primary_phase_forecast_rate'] = rates_or[-1]
                 # dca_forecast['arps_type'] = dca_arps
-                self.master._saveDCA(dcamaster_fk, int(well_fk), dca_forecast, x_selected, rates, dca_template_fit_forecast)
+                self.master._saveDCA(dcamaster_fk, list_well_ids[n], dca_forecast, x_selected, rates, dca_template_fit_forecast)
         #print("Total analyzed wells: ", len(dict_dca["list_well_names"]))#, "\nWells with issues: ",
               #[self.master._getKeyFromDict(well, self.master.wellmasterdict) for well in wells_nofit], "\n Total with issues: ",
               #len(wells_nofit), [self.master._getKeyFromDict(well, self.master.wellmasterdict) for well in wells_noprod],
               #"\n Total with no Production in the last 6 months: ", len(wells_noprod))
         print(f"Total analyzed wells: {len(dict_dca['list_well_names'])} \nWells with issues: {[self.master._getKeyFromDict(well, self.master.wellmasterdict) for well in wells_nofit]}")
 
     def editDCAMaster(self, master_fk: int, dict_edit_master: dict):
```

### Comparing `alanapy-0.4/alanapy.egg-info/PKG-INFO` & `alanapy-0.5/alanapy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alanapy
-Version: 0.4
+Version: 0.5
 Home-page: https://github.com/orkahub/alanapy
 Author: Orkahub Energy
 Author-email: orkahub@gmail.com
 License: MIT
 Keywords: RESERVOIR,ENERGY,OIL,GAS,PRODUCTION,PYTHON,ALANA
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `alanapy-0.4/setup.py` & `alanapy-0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name="alanapy",
     packages=["alanapy"],
-    version="0.4",
+    version="0.5",
     license="MIT",
     author = "Orkahub Energy",
 	author_email = "orkahub@gmail.com",
 	url = "https://github.com/orkahub/alanapy",
     long_description="Script for Alana API connection and functions https://alana.tech/open/accounts/login",
     long_description_content_type = "text/x-rst",
     classifiers=[
@@ -20,11 +20,10 @@
     keywords= ["RESERVOIR", "ENERGY", "OIL", "GAS", "PRODUCTION", "PYTHON","ALANA"],
     install_requires=[
         "requests",
         "matplotlib",
         "numpy",
         "pandas",
 		"datetime",
-		"os",
 		"re"
     ],
 )
```

