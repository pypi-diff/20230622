# Comparing `tmp/DiadFit-0.0.60.tar.gz` & `tmp/DiadFit-0.0.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DiadFit-0.0.60.tar", last modified: Wed Jun 21 02:56:01 2023, max compression
+gzip compressed data, was "DiadFit-0.0.61.tar", last modified: Thu Jun 22 21:15:53 2023, max compression
```

## Comparing `DiadFit-0.0.60.tar` & `DiadFit-0.0.61.tar`

### file list

```diff
@@ -1,27 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 02:56:01.320636 DiadFit-0.0.60/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-21 02:56:01.320636 DiadFit-0.0.60/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-21 02:55:46.000000 DiadFit-0.0.60/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 02:56:01.320636 DiadFit-0.0.60/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-21 02:55:49.000000 DiadFit-0.0.60/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 02:56:01.320636 DiadFit-0.0.60/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 02:56:01.320636 DiadFit-0.0.60/src/DiadFit/
--rw-r--r--   0 runner    (1001) docker     (123)    26927 2023-06-21 02:55:49.000000 DiadFit-0.0.60/src/DiadFit/CO2_EOS.py
--rw-r--r--   0 runner    (1001) docker     (123)    11055 2023-06-21 02:55:49.000000 DiadFit-0.0.60/src/DiadFit/CO2_in_bubble_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    43406 2023-06-21 02:55:49.000000 DiadFit-0.0.60/src/DiadFit/H2O_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-06-21 02:55:49.000000 DiadFit-0.0.60/src/DiadFit/Psensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-21 02:55:49.000000 DiadFit-0.0.60/src/DiadFit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-21 02:55:49.000000 DiadFit-0.0.60/src/DiadFit/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-06-21 02:55:49.000000 DiadFit-0.0.60/src/DiadFit/argon_lines.py
--rw-r--r--   0 runner    (1001) docker     (123)    23438 2023-06-21 02:55:49.000000 DiadFit-0.0.60/src/DiadFit/cosmicray_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-06-21 02:55:49.000000 DiadFit-0.0.60/src/DiadFit/densimeters.py
--rw-r--r--   0 runner    (1001) docker     (123)    16883 2023-06-21 02:55:49.000000 DiadFit-0.0.60/src/DiadFit/density_depth_crustal_profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)   162634 2023-06-21 02:55:49.000000 DiadFit-0.0.60/src/DiadFit/diads.py
--rw-r--r--   0 runner    (1001) docker     (123)    32657 2023-06-21 02:55:49.000000 DiadFit-0.0.60/src/DiadFit/error_propagation.py
--rw-r--r--   0 runner    (1001) docker     (123)    35199 2023-06-21 02:55:49.000000 DiadFit-0.0.60/src/DiadFit/importing_data_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    63568 2023-06-21 02:55:49.000000 DiadFit-0.0.60/src/DiadFit/ne_lines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 02:56:01.320636 DiadFit-0.0.60/src/DiadFit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-21 02:56:00.000000 DiadFit-0.0.60/src/DiadFit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-21 02:56:01.000000 DiadFit-0.0.60/src/DiadFit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 02:56:00.000000 DiadFit-0.0.60/src/DiadFit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-21 02:56:00.000000 DiadFit-0.0.60/src/DiadFit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-21 02:56:00.000000 DiadFit-0.0.60/src/DiadFit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:15:53.316125 DiadFit-0.0.61/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-22 21:15:53.316125 DiadFit-0.0.61/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-22 21:15:34.000000 DiadFit-0.0.61/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 21:15:53.316125 DiadFit-0.0.61/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-22 21:15:37.000000 DiadFit-0.0.61/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:15:53.312125 DiadFit-0.0.61/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:15:53.316125 DiadFit-0.0.61/src/DiadFit/
+-rw-r--r--   0 runner    (1001) docker     (123)    26927 2023-06-22 21:15:37.000000 DiadFit-0.0.61/src/DiadFit/CO2_EOS.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11055 2023-06-22 21:15:37.000000 DiadFit-0.0.61/src/DiadFit/CO2_in_bubble_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43406 2023-06-22 21:15:37.000000 DiadFit-0.0.61/src/DiadFit/H2O_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-22 21:15:37.000000 DiadFit-0.0.61/src/DiadFit/Highrho_polyfit_data.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-22 21:15:37.000000 DiadFit-0.0.61/src/DiadFit/Lowrho_polyfit_data.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-22 21:15:37.000000 DiadFit-0.0.61/src/DiadFit/Mediumrho_polyfit_data.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-06-22 21:15:37.000000 DiadFit-0.0.61/src/DiadFit/Psensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-22 21:15:37.000000 DiadFit-0.0.61/src/DiadFit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-22 21:15:37.000000 DiadFit-0.0.61/src/DiadFit/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-06-22 21:15:37.000000 DiadFit-0.0.61/src/DiadFit/argon_lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23438 2023-06-22 21:15:37.000000 DiadFit-0.0.61/src/DiadFit/cosmicray_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-06-22 21:15:37.000000 DiadFit-0.0.61/src/DiadFit/densimeter_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14936 2023-06-22 21:15:37.000000 DiadFit-0.0.61/src/DiadFit/densimeters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16883 2023-06-22 21:15:37.000000 DiadFit-0.0.61/src/DiadFit/density_depth_crustal_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)   162634 2023-06-22 21:15:37.000000 DiadFit-0.0.61/src/DiadFit/diads.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32657 2023-06-22 21:15:37.000000 DiadFit-0.0.61/src/DiadFit/error_propagation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35199 2023-06-22 21:15:37.000000 DiadFit-0.0.61/src/DiadFit/importing_data_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63944 2023-06-22 21:15:37.000000 DiadFit-0.0.61/src/DiadFit/ne_lines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:15:53.316125 DiadFit-0.0.61/src/DiadFit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-22 21:15:52.000000 DiadFit-0.0.61/src/DiadFit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-22 21:15:53.000000 DiadFit-0.0.61/src/DiadFit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 21:15:52.000000 DiadFit-0.0.61/src/DiadFit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-22 21:15:52.000000 DiadFit-0.0.61/src/DiadFit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-22 21:15:52.000000 DiadFit-0.0.61/src/DiadFit.egg-info/top_level.txt
```

### Comparing `DiadFit-0.0.60/PKG-INFO` & `DiadFit-0.0.61/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DiadFit
-Version: 0.0.60
+Version: 0.0.61
 Summary: DiadFit
 Home-page: https://github.com/PennyWieser/DiadFit
 Author: Penny Wieser
 Author-email: penny.wieser@gmail.com
 License: UNKNOWN
 Description: [![PyPI](https://badgen.net/pypi/v/DiadFit)](https://pypi.org/project/DiadFit/)
         [![Build Status](https://github.com/PennyWieser/DiadFit/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/PennyWieser/DiadFit/actions/workflows/main.yml)
```

### Comparing `DiadFit-0.0.60/README.md` & `DiadFit-0.0.61/README.md`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.60/setup.py` & `DiadFit-0.0.61/setup.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.60/src/DiadFit/CO2_EOS.py` & `DiadFit-0.0.61/src/DiadFit/CO2_EOS.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.60/src/DiadFit/CO2_in_bubble_error.py` & `DiadFit-0.0.61/src/DiadFit/CO2_in_bubble_error.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.60/src/DiadFit/H2O_fitting.py` & `DiadFit-0.0.61/src/DiadFit/H2O_fitting.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.60/src/DiadFit/Psensor.py` & `DiadFit-0.0.61/src/DiadFit/Psensor.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.60/src/DiadFit/__init__.py` & `DiadFit-0.0.61/src/DiadFit/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,16 @@
 # This does the work associated with fitting Diads
 from DiadFit.diads import *
 
 
 # This has densimeters from different instruments
 from DiadFit.densimeters import *
 
-
+# This has functions to fit densimeters
+from DiadFit.densimeter_fitting import *
 
 # H2O fitting
 from DiadFit.H2O_fitting import *
 
 # Monte Carlo Error propagation
 from DiadFit.error_propagation import *
```

### Comparing `DiadFit-0.0.60/src/DiadFit/argon_lines.py` & `DiadFit-0.0.61/src/DiadFit/argon_lines.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.60/src/DiadFit/cosmicray_filter.py` & `DiadFit-0.0.61/src/DiadFit/cosmicray_filter.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.60/src/DiadFit/densimeters.py` & `DiadFit-0.0.61/src/DiadFit/densimeters.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 import lmfit
 from lmfit.models import GaussianModel, VoigtModel, LinearModel, ConstantModel
 from scipy.signal import find_peaks
 import os
 import re
 from os import listdir
 from os.path import isfile, join
-
+import pickle
 encode="ISO-8859-1"
 
-
+## Cornell densimeters
 def calculate_density_cornell(*, temp='SupCrit', Split, split_err=None):
     """ This function converts Diad Splitting into CO$_2$ density using the densimeters of DeVitre et al. (2021)
     This should only be used for the Cornell Raman, not other Ramans at present
 
     Parameters
     -------------
     temp: str
@@ -98,15 +98,15 @@
     Imposs_lower_end=(df['Splitting']>103.350311768435) & (df['Splitting']<103.88)
     # Impossible densities, room T
     Imposs_upper_end=(df['Splitting']<104.407308904012) & (df['Splitting']>103.88)
     # Too low density
     Too_Low_SC=df['Splitting']<102.72
     Too_Low_RT=df['Splitting']<102.734115670188
 
-    df.loc[zero, 'Preferred_D']=0
+    df.loc[zero, 'Preferred D']=0
     df.loc[zero, 'Notes']=0
 
 
     # If room T, low density, set as low density
     df.loc[roomT&(min_lowD_RoomT_Split&max_lowD_RoomT_Split), 'Preferred D'] = LowD_RT
     df.loc[roomT&(min_lowD_RoomT_Split&max_lowD_RoomT_Split), 'Notes']='Room T, low density'
     # If room T, high density
@@ -198,11 +198,197 @@
     Diad1_err=df_sorted['Diad1_cent_err'].fillna(0)
     Diad2_err=df_sorted['Diad2_cent_err'].fillna(0)
     split_err=(Diad1_err**2 + Diad2_err**2)**0.5
     Combo_err= (((df_sorted['Splitting']* (Ne_err))**2) +  (Ne_corr['preferred_values'] *split_err  )**2 )**0.5
 
     return Combo_err
 
+## UCBerkeley densimeters
+def calculate_density_ucb(*, temp='SupCrit', Split, split_err=None):
+    """ This function converts Diad Splitting into CO$_2$ density using densimeters of UCB
+
+    Parameters
+    -------------
+    temp: str
+        'SupCrit' if measurements done at 37C
+        'RoomT' if measurements done at 24C
+
+    Split: int, float, pd.Series, np.array
+
+    Returns
+    --------------
+    pd.DataFrame
+        Prefered Density (based on different equatoins being merged), and intermediate calculations
+
+
+
+
+    """
+
+    # #if temp is "RoomT":
+    LowD_RT=-38.34631 + 0.3732578*Split
+    HighD_RT=-41.64784 + 0.4058777*Split- 0.1460339*(Split-104.653)**2
+
+    # IF temp is 37
+    pickle_str='Lowrho_polyfit_data.pkl'
+    with open(pickle_str, 'rb') as f:
+        lowrho_pickle_data = pickle.load(f)
+    pickle_str='Mediumrho_polyfit_data.pkl'
+    with open(pickle_str, 'rb') as f:
+        medrho_pickle_data = pickle.load(f)
+    pickle_str='Highrho_polyfit_data.pkl'
+    with open(pickle_str, 'rb') as f:
+        highrho_pickle_data = pickle.load(f)
+
+    lowrho_model = lowrho_pickle_data['model']
+    medrho_model = medrho_pickle_data['model']
+    highrho_model = highrho_pickle_data['model']
+
+    LowD_SC = pd.Series(lowrho_model(Split), index=Split.index)
+    MedD_SC = pd.Series(medrho_model(Split), index=Split.index)
+    HighD_SC = pd.Series(highrho_model(Split), index=Split.index)
+    if isinstance(Split, pd.Series) or isinstance(Split, np.ndarray):
+
+        df=pd.DataFrame(data={'Preferred D': 0,
+        'in range': 'Y',
+                                'Notes': 'not in range',
+                                'LowD_RT': LowD_RT,
+                                'HighD_RT': HighD_RT,
+                                'LowD_SC': LowD_SC,
+                                'MedD_SC': MedD_SC,
+                                'HighD_SC': HighD_SC,
+                                'Temperature': temp,
+                                'Splitting': Split,
+
+                                })
+
+    else:
+        df=pd.DataFrame(data={'Preferred D': 0,
+        'in range': 'Y',
+                                'Notes': 'not in range',
+                                'LowD_RT': LowD_RT,
+                                'HighD_RT': HighD_RT,
+                                'LowD_SC': LowD_SC,
+                                'MedD_SC': MedD_SC,
+                                'HighD_SC': HighD_SC,
+                                'Temperature': temp,
+                                'Splitting': Split,
+
+                                }, index=[0])
+
+
+    roomT=df['Temperature']=="RoomT"
+    SupCrit=df['Temperature']=="SupCrit"
+    # If splitting is 0
+    zero=df['Splitting']==0
+
+    # Range for SC low density
+    min_lowD_SC_Split=df['Splitting']>=102.7623598753032
+    max_lowD_SC_Split=df['Splitting']<=103.1741034592534
+    # Range for SC med density
+    min_MD_SC_Split=df['Splitting']>103.0608505403591
+    max_MD_SC_Split=df['Splitting']<=104.3836704771313
+    # Range for SC high density
+    min_HD_SC_Split=df['Splitting']>=104.2538992302499
+    max_HD_SC_Split=df['Splitting']<=105.3438707618937
+    # Range for Room T low density
+    min_lowD_RoomT_Split=df['Splitting']>=102.734115670188
+    max_lowD_RoomT_Split=df['Splitting']<=103.350311768435
+    # Range for Room T high density
+    min_HD_RoomT_Split=df['Splitting']>=104.407308904012
+    max_HD_RoomT_Split=df['Splitting']<=105.1
+    # Impossible densities, room T
+    Imposs_lower_end=(df['Splitting']>103.350311768435) & (df['Splitting']<103.88)
+    # Impossible densities, room T
+    Imposs_upper_end=(df['Splitting']<104.407308904012) & (df['Splitting']>103.88)
+    # Too low density
+    Too_Low_SC=df['Splitting']<102.7623598753032
+    Too_Low_RT=df['Splitting']<102.734115670188
+
+    df.loc[zero, 'Preferred D']=0
+    df.loc[zero, 'Notes']=0
+
+
+    # If room T, low density, set as low density
+    df.loc[roomT&(min_lowD_RoomT_Split&max_lowD_RoomT_Split), 'Preferred D'] = LowD_RT
+    df.loc[roomT&(min_lowD_RoomT_Split&max_lowD_RoomT_Split), 'Notes']='Room T, low density'
+    # If room T, high density
+    df.loc[roomT&(min_HD_RoomT_Split&max_HD_RoomT_Split), 'Preferred D'] = HighD_RT
+    df.loc[roomT&(min_HD_RoomT_Split&max_HD_RoomT_Split), 'Notes']='Room T, high density'
+
+    # If SupCrit, high density
+    df.loc[ SupCrit&(min_HD_SC_Split&max_HD_SC_Split), 'Preferred D'] = HighD_SC
+    df.loc[ SupCrit&(min_HD_SC_Split&max_HD_SC_Split), 'Notes']='SupCrit, high density'
+    # If SupCrit, Med density
+    df.loc[SupCrit&(min_MD_SC_Split&max_MD_SC_Split), 'Preferred D'] = MedD_SC
+    df.loc[SupCrit&(min_MD_SC_Split&max_MD_SC_Split), 'Notes']='SupCrit, Med density'
+
+    # If SupCrit, low density
+    df.loc[ SupCrit&(min_lowD_SC_Split&max_lowD_SC_Split), 'Preferred D'] = LowD_SC
+    df.loc[SupCrit&(min_lowD_SC_Split&max_lowD_SC_Split), 'Notes']='SupCrit, low density'
 
+    # If Supcritical, and too low
+    df.loc[SupCrit&(Too_Low_SC), 'Preferred D']=LowD_SC
+    df.loc[SupCrit&(Too_Low_SC), 'Notes']='Below lower calibration limit'
+    df.loc[SupCrit&(Too_Low_SC), 'in range']='N'
+
+
+    # If RoomT, and too low
+    df.loc[roomT&(Too_Low_RT), 'Preferred D']=LowD_RT
+    df.loc[roomT&(Too_Low_RT), 'Notes']='Below lower calibration limit'
+    df.loc[roomT&(Too_Low_RT), 'in range']='N'
+
+    #if splitting is zero
+    SplitZero=df['Splitting']==0
+    df.loc[SupCrit&(SplitZero), 'Preferred D']=np.nan
+    df.loc[SupCrit&(SplitZero), 'Notes']='Splitting=0'
+    df.loc[SupCrit&(SplitZero), 'in range']='N'
+
+    df.loc[roomT&(SplitZero), 'Preferred D']=np.nan
+    df.loc[roomT&(SplitZero), 'Notes']='Splitting=0'
+    df.loc[roomT&(SplitZero), 'in range']='N'
 
 
+    # If impossible density, lower end
+    df.loc[roomT&Imposs_lower_end, 'Preferred D'] = LowD_RT
+    df.loc[roomT&Imposs_lower_end, 'Notes']='Impossible Density, low density'
+    df.loc[roomT&Imposs_lower_end, 'in range']='N'
+
+    # If impossible density, lower end
+    df.loc[roomT&Imposs_upper_end, 'Preferred D'] = HighD_RT
+    df.loc[roomT&Imposs_upper_end, 'Notes']='Impossible Density, high density'
+    df.loc[roomT&Imposs_upper_end, 'in range']='N'
+
+
+    #df.loc[zero, 'in range']='Y'
+    # If high densiy, and beyond the upper calibration limit
+    Upper_Cal_RT=df['Splitting']>105.1
+    Upper_Cal_SC=df['Splitting']>105.3438707618937
+
+    df.loc[roomT&Upper_Cal_RT, 'Preferred D'] = HighD_RT
+    df.loc[roomT&Upper_Cal_RT, 'Notes']='Above upper Cali Limit'
+    df.loc[roomT&Upper_Cal_RT, 'in range']='N'
+
+    df.loc[SupCrit&Upper_Cal_SC, 'Preferred D'] = HighD_SC
+    df.loc[SupCrit&Upper_Cal_SC, 'Notes']='Above upper Cali Limit'
+    df.loc[SupCrit&Upper_Cal_SC, 'in range']='N'
+
+    if split_err is not None:
+        df2=calculate_dens_error_ucb(temp, Split, split_err)
+
+        df.insert(1, 'dens+1σ', df2['max_dens'])
+        df.insert(1, 'dens-1σ', df2['min_dens'])
+        df.insert(3, '1σ', (df2['max_dens']-df2['min_dens'])/2 )
+
+    return df
+
+def calculate_dens_error_ucb(temp, Split, split_err):
+
+    max_dens=calculate_density_ucb(temp=temp, Split=Split+split_err)
+    min_dens=calculate_density_ucb(temp=temp, Split=Split-split_err)
+    df=pd.DataFrame(data={
+                        'max_dens': max_dens['Preferred D'],
+                        'min_dens': min_dens['Preferred D']})
+
+    return df
+
```

### Comparing `DiadFit-0.0.60/src/DiadFit/density_depth_crustal_profiles.py` & `DiadFit-0.0.61/src/DiadFit/density_depth_crustal_profiles.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.60/src/DiadFit/diads.py` & `DiadFit-0.0.61/src/DiadFit/diads.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.60/src/DiadFit/error_propagation.py` & `DiadFit-0.0.61/src/DiadFit/error_propagation.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.60/src/DiadFit/importing_data_files.py` & `DiadFit-0.0.61/src/DiadFit/importing_data_files.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.60/src/DiadFit/ne_lines.py` & `DiadFit-0.0.61/src/DiadFit/ne_lines.py`

 * *Files 2% similar despite different names*

```diff
@@ -615,15 +615,15 @@
 
     return y_corr, Py_base, x,  Ne_short, Py_base, Baseline_y, Baseline_x
 
 
 
 
 
-def fit_pk1(x, y_corr, x_span=[-10, 8], Ne_center=1117.1, amplitude=98, pk1_sigma=0.28,
+def fit_pk1(x, y_corr, x_span=[-10, 8], Ne_center=1117.1, amplitude=98.1, pk1_sigma=0.28,
 LH_offset_mini=[1.5, 3], peaks_pk1=2, model_name='PseudoVoigtModel', block_print=True,
 const_params=True, spec_res=0.4) :
     """ This function fits the 1117 Ne line as 1 or two voigt peaks
 
     Parameters
     -----------
 
@@ -681,15 +681,19 @@
     if peaks_pk1>1:
 
         # Setting up lmfit
         if model_name == 'PseudoVoigtModel':
             model0 = PseudoVoigtModel(prefix='p0_')#+ ConstantModel(prefix='c0')
         if model_name=="VoigtModel":
             model0 = VoigtModel(prefix='p0_')#+ ConstantModel(prefix='c0')
-        pars0 = model0.make_params(p0_center=Ne_center, p0_amplitude=amplitude)
+        print(amplitude)
+        pars0 = model0.make_params()
+        pars0['p0_center'].set(Ne_center)
+        pars0['p0_amplitude'].set(amplitude)
+        
         init0 = model0.eval(pars0, x=xdat)
         result0 = model0.fit(ydat, pars0, x=xdat)
         Center_p0=result0.best_values.get('p0_center')
         if block_print is False:
             print('first iteration, peak Center='+str(np.round(Center_p0, 4)))
 
         Center_p0_error=result0.params.get('p0_center')
@@ -768,15 +772,16 @@
             model_combo = PseudoVoigtModel(prefix='p1_')#+ ConstantModel(prefix='c0')
         if model_name=="VoigtModel":
             model_combo= VoigtModel(prefix='p1_')#+ ConstantModel(prefix='c0')
 
 
 
         # create parameters with initial values
-        pars1 = model_combo.make_params(amplitude=amplitude)
+        pars1 = model_combo.make_params()
+        par1['p1_amplitude'].set(amplitude)
         pars1['p1_' + 'center'].set(Ne_center, min=Ne_center-2*spec_res,max=Ne_center+2*spec_res)
         pars1['p1_'+ 'sigma'].set(pk1_sigma, min=pk1_sigma*min_off, max=pk1_sigma*max_off)
 
 
 
 
 
@@ -908,23 +913,21 @@
         model = PseudoVoigtModel()#+ ConstantModel(prefix='c0')
     if model_name=="VoigtModel":
         model = VoigtModel()#+ ConstantModel(prefix='c0')
 
 
 
     # create parameters with initial values
-    params = model.make_params(center=Ne_center, amplitude=amplitude, sigma=pk2_sigma)
+    params = model.make_params()
+
+    params['center'].set(Ne_center, min=Ne_center+x_span[0], max=Ne_center+x_span[1])
+    params['amplitude'].set(amplitude, min=amplitude*min_off, max=amplitude*max_off)
+    params['sigma'].set(pk2_sigma, min=pk2_sigma*min_off, max=pk2_sigma*max_off)
+
 
-    # Place bounds on center allowed
-    params['center'].min = Ne_center+x_span[0]
-    params['center'].max = Ne_center+x_span[1]
-    params['sigma'].max = pk2_sigma*max_off
-    params['sigma'].min = pk2_sigma*min_off
-    params['amplitude'].max = amplitude*max_off
-    params['amplitude'].min = amplitude*min_off
     result = model.fit(Ne_pk2_reg_y.flatten(), params, x=Ne_pk2_reg_x.flatten())
 
     # Get center value
     Center_pk2=result.best_values.get('center')
     Center_pk2_error=result.params.get('center')
 
     Peak2_Prop_Lor=result.best_values.get('fraction')
@@ -1601,15 +1604,15 @@
 
 
     return ds
 
 
 ## Lets make a plotting function for this notebook 
 
-def plot_and_save_Ne_line_pickle(*, time, Ne_corr, N_poly=3, CI=0.67, bootstrap=False, std_error=True, N_bootstrap=500):
+def plot_and_save_Ne_line_pickle(*, time, Ne_corr, N_poly=3, CI=0.67, bootstrap=False, std_error=True, N_bootstrap=500,save_fig=False):
 # Define the x and y values
     x_all   = np.array([time])
     y_all = np.array([Ne_corr['Ne_Corr']])
     y_err=Ne_corr['1σ_Ne_Corr']
     non_nan_indices = ~np.isnan(x_all) & ~np.isnan(y_all)
 
     # Filter out NaN values
@@ -1645,19 +1648,33 @@
              fmt='o', ecolor='k', elinewidth=0.8, mfc='grey', ms=5, mec='k',capsize=3)
     
     ax1.plot(new_x_plot, Ne_corr2['preferred_values'], '-k', label='best fit')
     ax1.plot(new_x_plot, Ne_corr2['lower_values'], ':k', label='lower vals')
     ax1.plot(new_x_plot, Ne_corr2['upper_values'], ':k', label='upper vals')
     ax1.set_xlabel('sec after midnight')
     ax1.set_ylabel('Ne Corr factor')
-    ax1.set_title(str(100*CI) + ' % prediction interval')
     ax1.legend()
     ax1.plot(x, y, '+r', label='Ne lines')
     ax1.ticklabel_format(useOffset=False)
+    # this sets the ordinal suffix for the polynomial degree in the title
+    if N_poly == 1:
+        suffix = 'st'
+    elif N_poly == 2:
+        suffix = 'nd'
+    elif N_poly == 3:
+        suffix = 'rd'
+    else:
+        suffix='th'
+        
+    ax1.set_title(f"{N_poly}$^{{{suffix}}}$ degree polynomial: "+str(100*CI) + ' % prediction interval')
+
     
+    if save_fig is True:
+        fig.savefig('Ne_line_correction.png')
+        
 
     
 from scipy.stats import t
 import numpy as np
 
 def calculate_Ne_corr_std_err_values(*, pickle_str, new_x, CI=0.67):
     # Load the model and the data from the pickle file
```

### Comparing `DiadFit-0.0.60/src/DiadFit.egg-info/PKG-INFO` & `DiadFit-0.0.61/src/DiadFit.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DiadFit
-Version: 0.0.60
+Version: 0.0.61
 Summary: DiadFit
 Home-page: https://github.com/PennyWieser/DiadFit
 Author: Penny Wieser
 Author-email: penny.wieser@gmail.com
 License: UNKNOWN
 Description: [![PyPI](https://badgen.net/pypi/v/DiadFit)](https://pypi.org/project/DiadFit/)
         [![Build Status](https://github.com/PennyWieser/DiadFit/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/PennyWieser/DiadFit/actions/workflows/main.yml)
```

### Comparing `DiadFit-0.0.60/src/DiadFit.egg-info/SOURCES.txt` & `DiadFit-0.0.61/src/DiadFit.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 README.md
 setup.py
 src/DiadFit/CO2_EOS.py
 src/DiadFit/CO2_in_bubble_error.py
 src/DiadFit/H2O_fitting.py
+src/DiadFit/Highrho_polyfit_data.pkl
+src/DiadFit/Lowrho_polyfit_data.pkl
+src/DiadFit/Mediumrho_polyfit_data.pkl
 src/DiadFit/Psensor.py
 src/DiadFit/__init__.py
 src/DiadFit/_version.py
 src/DiadFit/argon_lines.py
 src/DiadFit/cosmicray_filter.py
+src/DiadFit/densimeter_fitting.py
 src/DiadFit/densimeters.py
 src/DiadFit/density_depth_crustal_profiles.py
 src/DiadFit/diads.py
 src/DiadFit/error_propagation.py
 src/DiadFit/importing_data_files.py
 src/DiadFit/ne_lines.py
 src/DiadFit.egg-info/PKG-INFO
```

