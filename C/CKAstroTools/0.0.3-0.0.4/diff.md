# Comparing `tmp/CKAstroTools-0.0.3.tar.gz` & `tmp/CKAstroTools-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CKAstroTools-0.0.3.tar", last modified: Mon Jun 19 09:22:16 2023, max compression
+gzip compressed data, was "CKAstroTools-0.0.4.tar", last modified: Thu Jun 22 09:01:33 2023, max compression
```

## Comparing `CKAstroTools-0.0.3.tar` & `CKAstroTools-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-19 09:22:16.043457 CKAstroTools-0.0.3/
-drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-19 09:22:16.039456 CKAstroTools-0.0.3/CKAstroTools.egg-info/
--rw-rw-r--   0 koenig    (1000) koenig    (1000)     1352 2023-06-19 09:22:16.000000 CKAstroTools-0.0.3/CKAstroTools.egg-info/PKG-INFO
--rw-rw-r--   0 koenig    (1000) koenig    (1000)      405 2023-06-19 09:22:16.000000 CKAstroTools-0.0.3/CKAstroTools.egg-info/SOURCES.txt
--rw-rw-r--   0 koenig    (1000) koenig    (1000)        1 2023-06-19 09:22:16.000000 CKAstroTools-0.0.3/CKAstroTools.egg-info/dependency_links.txt
--rw-rw-r--   0 koenig    (1000) koenig    (1000)       14 2023-06-19 09:22:16.000000 CKAstroTools-0.0.3/CKAstroTools.egg-info/requires.txt
--rw-rw-r--   0 koenig    (1000) koenig    (1000)       13 2023-06-19 09:22:16.000000 CKAstroTools-0.0.3/CKAstroTools.egg-info/top_level.txt
--rw-rw-r--   0 koenig    (1000) koenig    (1000)     1071 2022-12-19 09:28:13.000000 CKAstroTools-0.0.3/LICENSE
--rw-rw-r--   0 koenig    (1000) koenig    (1000)     1352 2023-06-19 09:22:16.043457 CKAstroTools-0.0.3/PKG-INFO
--rw-rw-r--   0 koenig    (1000) koenig    (1000)      750 2023-06-18 09:30:05.000000 CKAstroTools-0.0.3/README.md
-drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-19 09:22:16.039456 CKAstroTools-0.0.3/ckastrotools/
--rw-rw-r--   0 koenig    (1000) koenig    (1000)        1 2022-12-19 09:28:13.000000 CKAstroTools-0.0.3/ckastrotools/__init__.py
--rw-rw-r--   0 koenig    (1000) koenig    (1000)       78 2022-12-19 09:28:13.000000 CKAstroTools-0.0.3/ckastrotools/__main__.py
-drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-19 09:22:16.043457 CKAstroTools-0.0.3/ckastrotools/io/
--rw-rw-r--   0 koenig    (1000) koenig    (1000)       31 2022-12-19 10:11:43.000000 CKAstroTools-0.0.3/ckastrotools/io/__init__.py
--rw-rw-r--   0 koenig    (1000) koenig    (1000)     1270 2022-12-19 10:33:57.000000 CKAstroTools-0.0.3/ckastrotools/io/subcube.py
-drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-19 09:22:16.043457 CKAstroTools-0.0.3/ckastrotools/milkyway/
--rw-rw-r--   0 koenig    (1000) koenig    (1000)        0 2023-06-10 14:05:04.000000 CKAstroTools-0.0.3/ckastrotools/milkyway/__init__.py
--rw-rw-r--   0 koenig    (1000) koenig    (1000)    17474 2023-06-19 09:19:24.000000 CKAstroTools-0.0.3/ckastrotools/milkyway/spiralarms.py
--rw-rw-r--   0 koenig    (1000) koenig    (1000)      826 2023-06-19 09:20:37.000000 CKAstroTools-0.0.3/pyproject.toml
--rw-rw-r--   0 koenig    (1000) koenig    (1000)       38 2023-06-19 09:22:16.043457 CKAstroTools-0.0.3/setup.cfg
-drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-19 09:22:16.043457 CKAstroTools-0.0.3/tests/
--rw-rw-r--   0 koenig    (1000) koenig    (1000)      146 2022-12-19 09:28:13.000000 CKAstroTools-0.0.3/tests/test_main.py
+drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-22 09:01:33.836174 CKAstroTools-0.0.4/
+drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-22 09:01:33.832174 CKAstroTools-0.0.4/CKAstroTools.egg-info/
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)     1472 2023-06-22 09:01:33.000000 CKAstroTools-0.0.4/CKAstroTools.egg-info/PKG-INFO
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)      405 2023-06-22 09:01:33.000000 CKAstroTools-0.0.4/CKAstroTools.egg-info/SOURCES.txt
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)        1 2023-06-22 09:01:33.000000 CKAstroTools-0.0.4/CKAstroTools.egg-info/dependency_links.txt
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)       14 2023-06-22 09:01:33.000000 CKAstroTools-0.0.4/CKAstroTools.egg-info/requires.txt
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)       13 2023-06-22 09:01:33.000000 CKAstroTools-0.0.4/CKAstroTools.egg-info/top_level.txt
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)     1071 2022-12-19 09:28:13.000000 CKAstroTools-0.0.4/LICENSE
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)     1472 2023-06-22 09:01:33.832174 CKAstroTools-0.0.4/PKG-INFO
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)      870 2023-06-21 08:04:01.000000 CKAstroTools-0.0.4/README.md
+drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-22 09:01:33.832174 CKAstroTools-0.0.4/ckastrotools/
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)        1 2022-12-19 09:28:13.000000 CKAstroTools-0.0.4/ckastrotools/__init__.py
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)       78 2022-12-19 09:28:13.000000 CKAstroTools-0.0.4/ckastrotools/__main__.py
+drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-22 09:01:33.832174 CKAstroTools-0.0.4/ckastrotools/io/
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)       31 2022-12-19 10:11:43.000000 CKAstroTools-0.0.4/ckastrotools/io/__init__.py
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)     1270 2022-12-19 10:33:57.000000 CKAstroTools-0.0.4/ckastrotools/io/subcube.py
+drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-22 09:01:33.832174 CKAstroTools-0.0.4/ckastrotools/milkyway/
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)        0 2023-06-10 14:05:04.000000 CKAstroTools-0.0.4/ckastrotools/milkyway/__init__.py
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)    17016 2023-06-22 08:57:16.000000 CKAstroTools-0.0.4/ckastrotools/milkyway/spiralarms.py
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)      826 2023-06-22 08:59:18.000000 CKAstroTools-0.0.4/pyproject.toml
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)       38 2023-06-22 09:01:33.836174 CKAstroTools-0.0.4/setup.cfg
+drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-22 09:01:33.832174 CKAstroTools-0.0.4/tests/
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)      146 2022-12-19 09:28:13.000000 CKAstroTools-0.0.4/tests/test_main.py
```

### Comparing `CKAstroTools-0.0.3/CKAstroTools.egg-info/PKG-INFO` & `CKAstroTools-0.0.4/CKAstroTools.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CKAstroTools
-Version: 0.0.3
+Version: 0.0.4
 Summary: General toolks for astronomy I personally use regularly for data analysis.
 Author: Carsten König
 License: MIT License
 Project-URL: Homepage, https://gitlab.com/ck2go/ckastrotools
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -18,14 +18,16 @@
 # CK AstroTools
 
 General tools for astronomy I personally use regularly for data analysis.
 
 **Status:**  Alpha\
 **Author:** Carsten König\
 **Repository:** https://gitlab.com/ck2go/ckastrotools
+**PyPi:** https://test.pypi.org/project/CKAstroTools/
+**Documentation:** https://ckastrotools.readthedocs.io/en/latest/
 
 ## Purpose
 
 Providing common tools, functions, workflows that I use for my everyday scientific work.
 
 ## Installation
```

### Comparing `CKAstroTools-0.0.3/LICENSE` & `CKAstroTools-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `CKAstroTools-0.0.3/PKG-INFO` & `CKAstroTools-0.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CKAstroTools
-Version: 0.0.3
+Version: 0.0.4
 Summary: General toolks for astronomy I personally use regularly for data analysis.
 Author: Carsten König
 License: MIT License
 Project-URL: Homepage, https://gitlab.com/ck2go/ckastrotools
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -18,14 +18,16 @@
 # CK AstroTools
 
 General tools for astronomy I personally use regularly for data analysis.
 
 **Status:**  Alpha\
 **Author:** Carsten König\
 **Repository:** https://gitlab.com/ck2go/ckastrotools
+**PyPi:** https://test.pypi.org/project/CKAstroTools/
+**Documentation:** https://ckastrotools.readthedocs.io/en/latest/
 
 ## Purpose
 
 Providing common tools, functions, workflows that I use for my everyday scientific work.
 
 ## Installation
```

### Comparing `CKAstroTools-0.0.3/README.md` & `CKAstroTools-0.0.4/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # CK AstroTools
 
 General tools for astronomy I personally use regularly for data analysis.
 
 **Status:**  Alpha\
 **Author:** Carsten König\
 **Repository:** https://gitlab.com/ck2go/ckastrotools
+**PyPi:** https://test.pypi.org/project/CKAstroTools/
+**Documentation:** https://ckastrotools.readthedocs.io/en/latest/
 
 ## Purpose
 
 Providing common tools, functions, workflows that I use for my everyday scientific work.
 
 ## Installation
```

### Comparing `CKAstroTools-0.0.3/ckastrotools/io/subcube.py` & `CKAstroTools-0.0.4/ckastrotools/io/subcube.py`

 * *Files identical despite different names*

### Comparing `CKAstroTools-0.0.3/ckastrotools/milkyway/spiralarms.py` & `CKAstroTools-0.0.4/ckastrotools/milkyway/spiralarms.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,40 +5,40 @@
 from astropy import units as u
 
 
 def _getSpiralParameters(model):
     # Spiral arm params from Reid et al. (2014)
     reid2014 = {'perseus': {'R_ref': 9.9,  # kpc
                             'beta_ref': 14.2,  # deg (from Galactic center to sun =0)
-                            'beta_min': -110.0,  # deg
-                            'beta_max': 270.0,  # deg
+                            'beta_min': -160.0,  # deg
+                            'beta_max': 390.0,  # deg
                             'pitch': 9.9,  # deg
                             'width': 0.38},  # kpc
                 'sagittarius': {'R_ref': 6.6,  # kpc
                                 'beta_ref': 25.6,  # deg (from Galactic center to sun =0)
-                                'beta_min': -110.0,  # deg
-                                'beta_max': 270.0,  # deg
+                                'beta_min': -245.0,  # deg
+                                'beta_max': 225.0,  # deg
                                 'pitch': 6.9,  # deg
                                 'width': 0.26},  # kpc
                 'scutum': {'R_ref': 5.0,  # kpc
                            'beta_ref': 27.6,  # deg (from Galactic center to sun =0)
-                           'beta_min': -110.0,  # deg
-                           'beta_max': 270.0,  # deg
+                           'beta_min': 3.0,  # deg
+                           'beta_max': 560.0,  # deg
                            'pitch': 19.8,  # deg
                            'width': 0.17},  # kpc
                 'local': {'R_ref': 8.4,  # kpc
                           'beta_ref': 8.9,  # deg (from Galactic center to sun =0)
                           'beta_min': -110.0,  # deg
                           'beta_max': 270.0,  # deg
                           'pitch': 12.8,  # deg
                           'width': 0.33},  # kpc
                 'outer': {'R_ref': 13.0,  # kpc
                           'beta_ref': 18.6,  # deg (from Galactic center to sun =0)
-                          'beta_min': -110.0,  # deg
-                          'beta_max': 270.0,  # deg
+                          'beta_min': -70.0,  # deg
+                          'beta_max': 410.0,  # deg
                           'pitch': 13.8,  # deg
                           'width': 0.63}}  # kpc
 
 
     # Spiral arm params combined from Reid et al. (2019), CK
     custom2019 = {
         'norma1': {'R_ref': 4.46,  # kpc
@@ -154,15 +154,15 @@
                    'pitch': 3.0,  # deg
                    'width': 0.65},  # kpc
         'outer0': {'R_ref': 12.24,  # kpc
                    'beta_ref': 18.,  # deg (from Galactic center to sun =0)
                    'pitch': 9.4,  # deg
                    'width': 0.65}}  # kpc
 
-    ck = {'perseus': {'R_ref': 10.9,  # kpc
+    ck2021 = {'perseus': {'R_ref': 10.9,  # kpc
                       'beta_ref': -16.6,  # deg (from Galactic center to sun =0)
                       'beta_min': -91.415,  # deg (i.e. ~l=280)
                       'beta_max': 0.0,  # deg (i.e. ~l=180)
                       'pitch': 5.7,  # deg
                       'width': 0.38},  # kpc
           'local': {'R_ref': 9.8,  # kpc
                     'beta_ref': -0.5,  # deg (from Galactic center to sun =0)
@@ -182,89 +182,79 @@
                            'beta_min': -110.0,  # deg
                            'beta_max': 270.0,  # deg
                            'pitch': 13.1,  # deg
                            'width': np.nan}}  # kpc
 
     vallee2015 = {'perseus': {'R_ref': 7.0,  # kpc
                               'beta_ref': 90.,  # deg (from Galactic center to sun =0)
-                              'beta_min': -110.0,  # deg
-                              'beta_max': 270.0,  # deg
+                              'beta_min': -160.0,  # deg
+                              'beta_max': 390.0,  # deg
                               'pitch': 13.,  # deg
                               'width': 0.38},  # kpc
                   'sagittarius': {'R_ref': 7.0,  # kpc
                                   'beta_ref': 0.,  # deg (from Galactic center to sun =0)
-                                  'beta_min': -110.0,  # deg
-                                  'beta_max': 270.0,  # deg
+                                  'beta_min': -245.0,  # deg
+                                  'beta_max': 225.0,  # deg
                                   'pitch': 13.,  # deg
                                   'width': 0.33},  # kpc
                   'scutum': {'R_ref': 7.0,  # kpc
                              'beta_ref': 270.,  # deg (from Galactic center to sun =0)
-                             'beta_min': -110.0,  # deg
-                             'beta_max': 270.0,  # deg
+                             'beta_min': 3.0,  # deg
+                             'beta_max': 560.,  # deg
                              'pitch': 13.,  # deg
                              'width': 0.33},  # kpc
                   'outer': {'R_ref': 7.0,  # kpc
                             'beta_ref': 180.,  # deg (from Galactic center to sun =0)
-                            'beta_min': -110.0,  # deg
-                            'beta_max': 270.0,  # deg
+                            'beta_min': -70.0,  # deg
+                            'beta_max': 410.0,  # deg
                             'pitch': 12.5,  # deg
                             'width': 0.63}}  # kpc
 
     if model == 'reid2014':
         spiral_arm_params = reid2014
     elif model == 'reid2019':
         spiral_arm_params = reid2019
     elif model == 'xinyu2016':
         spiral_arm_params = xinyu2016
     elif model == 'vallee2015':
         spiral_arm_params = vallee2015
-    elif model == 'ck':
-        spiral_arm_params = ck
+    elif model == 'ck2021':
+        spiral_arm_params = ck2021
 
     return spiral_arm_params
 
 
-def getSpiralArm(name, model='reid2014', beta_min=None, beta_max=None,
+def getSpiralArm(name, model='reid2014',
                  resolution=0.0001, R_0=8.34):
     """
     Get the spiral arm model for a given arm name.
 
     Parameters
     ----------
     name: str
         Name of the spiral arm.
     model: str
         Name of the spiral arm model to be used.
-    beta_min: float
-        Minimum galactocentric angle in degrees (0=GC to sun, clockwise).
-        If None, the default value.
-    beta_max: float
-        Maximum galactocentric angle in degrees (0=GC to sun, clockwise).
-        If None, the default value.
+        Available models: reid2014 (default), ck, vallee2015.
     resolution: float
         Resolution of the spiral arm model in degrees.
     R_0: float
         Galactocentric distance of the sun in kpc.
 
     Returns
     -------
     Coordinates of the spiral arm in the galactocentric frame.
     """
     spiral_arm_params = _getSpiralParameters(model)
 
     R_ref = spiral_arm_params[name]['R_ref']
     beta_ref = spiral_arm_params[name]['beta_ref']
     pitch = spiral_arm_params[name]['pitch']
-    if beta_min is None:
-        beta_min = spiral_arm_params[name]['beta_min']
-    if beta_max is None:
-        beta_max = spiral_arm_params[name]['beta_max']
-    print(beta_min)
-    print(beta_max)
-    print(resolution)
+    beta_min = spiral_arm_params[name]['beta_min']
+    beta_max = spiral_arm_params[name]['beta_max']
     beta = np.arange(beta_max, beta_min, -1. * resolution)  # [deg]
 
     R_gal = R_ref * np.exp(-1 * (beta - beta_ref) * np.pi / 180. * np.tan(np.pi / 180. * pitch))  # kpc
 
     #     x = R_gal * -1. * np.cos(beta * np.pi/180.)
     #     y = R_gal * np.sin(beta * np.pi/180.)
     x = -1 * R_gal * np.sin((90 - beta) * np.pi / 180.)
@@ -307,40 +297,40 @@
 
     # SAGITTARIUS arm
     # svx1, svy1 = getSpiralArm('sagittarius', beta_min=-245., beta_max=-2, model=model)
     # sx, sy = getSpiralArm('sagittarius', beta_min=-2, beta_max=68, model=model)
     # svx2, svy2 = getSpiralArm('sagittarius', beta_min=68, beta_max=225, model=model)
     # sag_x = list(svx1)+list(sx)+list(svx2)
     # sag_y = list(svy1)+list(sy)+list(svy2)
-    sagittarius = getSpiralArm('sagittarius', model=model, beta_min=-245., beta_max=225)
+    sagittarius = getSpiralArm('sagittarius', model=model)
 
     # SCUTUM arm
     # scx, scy = getSpiralArm('scutum', beta_min=3, beta_max=101, model=model)
     # scvx, scvy = getSpiralArm('scutum', beta_min=101, beta_max=363, model=model)
     # scvx2, scvy2 = getSpiralArm('scutum', beta_min=363, beta_max=560, model=model)
     # scutum_x = list(scx)+list(scvx)+list(scvx2)
     # scutum_y = list(scy)+list(scvy)+list(scvy2)
-    scutum = getSpiralArm('scutum', beta_max=560, model=model, beta_min=3)
+    scutum = getSpiralArm('scutum', model=model)
 
     # OUTER arm
     # ockx, ocky = getSpiralArm('outer', beta_min=-70, beta_max=-6, model=model)
     # ox, oy = getSpiralArm('outer', beta_min=-6, beta_max=56, model=model)
     # ovx, ovy = getSpiralArm('outer', beta_min=56, beta_max=410, model=model)
     # outer_x = list(ockx) + list(ox) + list(ovx)
     # outer_y = list(ocky) + list(oy) + list(ovy)
-    outer = getSpiralArm('outer', model=model, beta_min=-70, beta_max=410)
+    outer = getSpiralArm('outer', model=model)
 
     # PERSEUS spiral arm
     # pvx2, pvy2 = getSpiralArm('perseus', beta_min=-160, beta_max=-40, model=model)
     # pckx, pcky = getSpiralArm('perseus', beta_min=-40, beta_max=-10, model=model)
     # px, py = getSpiralArm('perseus', beta_min=-10, beta_max=90, model=model)
     # pvx, pvy = getSpiralArm('perseus', beta_min=90, beta_max=390, model=model)
     # per_x = list(pckx) + list(pvx2) + list(px) + list(pvx)
     # per_y = list(pcky) + list(pvy2) + list(py) + list(pvy)
-    perseus = getSpiralArm('perseus', model=model, beta_min=-160, beta_max=390)
+    perseus = getSpiralArm('perseus', model=model)
 
     return sagittarius, scutum, outer, perseus
 
 
 def getSpiralArms(model='vallee2015'):
     """
     Returns the spiral arms in a dictionary.
```

### Comparing `CKAstroTools-0.0.3/pyproject.toml` & `CKAstroTools-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
             "pytest",
             "pytest-mock"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "CKAstroTools"
 description = "General toolks for astronomy I personally use regularly for data analysis."
-version = "0.0.3"
+version = "0.0.4"
 requires-python = ">=3.7"
 dependencies = ["spectral-cube"]
 keywords = []
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
```

