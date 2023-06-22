# Comparing `tmp/CKAstroTools-0.0.4.tar.gz` & `tmp/CKAstroTools-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CKAstroTools-0.0.4.tar", last modified: Thu Jun 22 09:01:33 2023, max compression
+gzip compressed data, was "CKAstroTools-0.0.5.tar", last modified: Thu Jun 22 09:26:23 2023, max compression
```

## Comparing `CKAstroTools-0.0.4.tar` & `CKAstroTools-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-22 09:01:33.836174 CKAstroTools-0.0.4/
-drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-22 09:01:33.832174 CKAstroTools-0.0.4/CKAstroTools.egg-info/
--rw-rw-r--   0 koenig    (1000) koenig    (1000)     1472 2023-06-22 09:01:33.000000 CKAstroTools-0.0.4/CKAstroTools.egg-info/PKG-INFO
--rw-rw-r--   0 koenig    (1000) koenig    (1000)      405 2023-06-22 09:01:33.000000 CKAstroTools-0.0.4/CKAstroTools.egg-info/SOURCES.txt
--rw-rw-r--   0 koenig    (1000) koenig    (1000)        1 2023-06-22 09:01:33.000000 CKAstroTools-0.0.4/CKAstroTools.egg-info/dependency_links.txt
--rw-rw-r--   0 koenig    (1000) koenig    (1000)       14 2023-06-22 09:01:33.000000 CKAstroTools-0.0.4/CKAstroTools.egg-info/requires.txt
--rw-rw-r--   0 koenig    (1000) koenig    (1000)       13 2023-06-22 09:01:33.000000 CKAstroTools-0.0.4/CKAstroTools.egg-info/top_level.txt
--rw-rw-r--   0 koenig    (1000) koenig    (1000)     1071 2022-12-19 09:28:13.000000 CKAstroTools-0.0.4/LICENSE
--rw-rw-r--   0 koenig    (1000) koenig    (1000)     1472 2023-06-22 09:01:33.832174 CKAstroTools-0.0.4/PKG-INFO
--rw-rw-r--   0 koenig    (1000) koenig    (1000)      870 2023-06-21 08:04:01.000000 CKAstroTools-0.0.4/README.md
-drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-22 09:01:33.832174 CKAstroTools-0.0.4/ckastrotools/
--rw-rw-r--   0 koenig    (1000) koenig    (1000)        1 2022-12-19 09:28:13.000000 CKAstroTools-0.0.4/ckastrotools/__init__.py
--rw-rw-r--   0 koenig    (1000) koenig    (1000)       78 2022-12-19 09:28:13.000000 CKAstroTools-0.0.4/ckastrotools/__main__.py
-drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-22 09:01:33.832174 CKAstroTools-0.0.4/ckastrotools/io/
--rw-rw-r--   0 koenig    (1000) koenig    (1000)       31 2022-12-19 10:11:43.000000 CKAstroTools-0.0.4/ckastrotools/io/__init__.py
--rw-rw-r--   0 koenig    (1000) koenig    (1000)     1270 2022-12-19 10:33:57.000000 CKAstroTools-0.0.4/ckastrotools/io/subcube.py
-drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-22 09:01:33.832174 CKAstroTools-0.0.4/ckastrotools/milkyway/
--rw-rw-r--   0 koenig    (1000) koenig    (1000)        0 2023-06-10 14:05:04.000000 CKAstroTools-0.0.4/ckastrotools/milkyway/__init__.py
--rw-rw-r--   0 koenig    (1000) koenig    (1000)    17016 2023-06-22 08:57:16.000000 CKAstroTools-0.0.4/ckastrotools/milkyway/spiralarms.py
--rw-rw-r--   0 koenig    (1000) koenig    (1000)      826 2023-06-22 08:59:18.000000 CKAstroTools-0.0.4/pyproject.toml
--rw-rw-r--   0 koenig    (1000) koenig    (1000)       38 2023-06-22 09:01:33.836174 CKAstroTools-0.0.4/setup.cfg
-drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-22 09:01:33.832174 CKAstroTools-0.0.4/tests/
--rw-rw-r--   0 koenig    (1000) koenig    (1000)      146 2022-12-19 09:28:13.000000 CKAstroTools-0.0.4/tests/test_main.py
+drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-22 09:26:23.118993 CKAstroTools-0.0.5/
+drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-22 09:26:23.118993 CKAstroTools-0.0.5/CKAstroTools.egg-info/
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)     1476 2023-06-22 09:26:23.000000 CKAstroTools-0.0.5/CKAstroTools.egg-info/PKG-INFO
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)      405 2023-06-22 09:26:23.000000 CKAstroTools-0.0.5/CKAstroTools.egg-info/SOURCES.txt
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)        1 2023-06-22 09:26:23.000000 CKAstroTools-0.0.5/CKAstroTools.egg-info/dependency_links.txt
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)       14 2023-06-22 09:26:23.000000 CKAstroTools-0.0.5/CKAstroTools.egg-info/requires.txt
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)       13 2023-06-22 09:26:23.000000 CKAstroTools-0.0.5/CKAstroTools.egg-info/top_level.txt
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)     1071 2022-12-19 09:28:13.000000 CKAstroTools-0.0.5/LICENSE
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)     1476 2023-06-22 09:26:23.118993 CKAstroTools-0.0.5/PKG-INFO
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)      874 2023-06-22 09:22:37.000000 CKAstroTools-0.0.5/README.md
+drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-22 09:26:23.118993 CKAstroTools-0.0.5/ckastrotools/
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)        1 2022-12-19 09:28:13.000000 CKAstroTools-0.0.5/ckastrotools/__init__.py
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)       78 2022-12-19 09:28:13.000000 CKAstroTools-0.0.5/ckastrotools/__main__.py
+drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-22 09:26:23.118993 CKAstroTools-0.0.5/ckastrotools/io/
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)       31 2022-12-19 10:11:43.000000 CKAstroTools-0.0.5/ckastrotools/io/__init__.py
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)     1270 2022-12-19 10:33:57.000000 CKAstroTools-0.0.5/ckastrotools/io/subcube.py
+drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-22 09:26:23.118993 CKAstroTools-0.0.5/ckastrotools/milkyway/
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)        0 2023-06-10 14:05:04.000000 CKAstroTools-0.0.5/ckastrotools/milkyway/__init__.py
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)    17687 2023-06-22 09:21:02.000000 CKAstroTools-0.0.5/ckastrotools/milkyway/spiralarms.py
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)      826 2023-06-22 09:22:53.000000 CKAstroTools-0.0.5/pyproject.toml
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)       38 2023-06-22 09:26:23.118993 CKAstroTools-0.0.5/setup.cfg
+drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-22 09:26:23.118993 CKAstroTools-0.0.5/tests/
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)      146 2022-12-19 09:28:13.000000 CKAstroTools-0.0.5/tests/test_main.py
```

### Comparing `CKAstroTools-0.0.4/CKAstroTools.egg-info/PKG-INFO` & `CKAstroTools-0.0.5/CKAstroTools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CKAstroTools
-Version: 0.0.4
+Version: 0.0.5
 Summary: General toolks for astronomy I personally use regularly for data analysis.
 Author: Carsten König
 License: MIT License
 Project-URL: Homepage, https://gitlab.com/ck2go/ckastrotools
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -17,16 +17,16 @@
 
 # CK AstroTools
 
 General tools for astronomy I personally use regularly for data analysis.
 
 **Status:**  Alpha\
 **Author:** Carsten König\
-**Repository:** https://gitlab.com/ck2go/ckastrotools
-**PyPi:** https://test.pypi.org/project/CKAstroTools/
+**Repository:** https://gitlab.com/ck2go/ckastrotools \
+**PyPi:** https://test.pypi.org/project/CKAstroTools/ \
 **Documentation:** https://ckastrotools.readthedocs.io/en/latest/
 
 ## Purpose
 
 Providing common tools, functions, workflows that I use for my everyday scientific work.
 
 ## Installation
```

### Comparing `CKAstroTools-0.0.4/LICENSE` & `CKAstroTools-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `CKAstroTools-0.0.4/PKG-INFO` & `CKAstroTools-0.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CKAstroTools
-Version: 0.0.4
+Version: 0.0.5
 Summary: General toolks for astronomy I personally use regularly for data analysis.
 Author: Carsten König
 License: MIT License
 Project-URL: Homepage, https://gitlab.com/ck2go/ckastrotools
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -17,16 +17,16 @@
 
 # CK AstroTools
 
 General tools for astronomy I personally use regularly for data analysis.
 
 **Status:**  Alpha\
 **Author:** Carsten König\
-**Repository:** https://gitlab.com/ck2go/ckastrotools
-**PyPi:** https://test.pypi.org/project/CKAstroTools/
+**Repository:** https://gitlab.com/ck2go/ckastrotools \
+**PyPi:** https://test.pypi.org/project/CKAstroTools/ \
 **Documentation:** https://ckastrotools.readthedocs.io/en/latest/
 
 ## Purpose
 
 Providing common tools, functions, workflows that I use for my everyday scientific work.
 
 ## Installation
```

### Comparing `CKAstroTools-0.0.4/README.md` & `CKAstroTools-0.0.5/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # CK AstroTools
 
 General tools for astronomy I personally use regularly for data analysis.
 
 **Status:**  Alpha\
 **Author:** Carsten König\
-**Repository:** https://gitlab.com/ck2go/ckastrotools
-**PyPi:** https://test.pypi.org/project/CKAstroTools/
+**Repository:** https://gitlab.com/ck2go/ckastrotools \
+**PyPi:** https://test.pypi.org/project/CKAstroTools/ \
 **Documentation:** https://ckastrotools.readthedocs.io/en/latest/
 
 ## Purpose
 
 Providing common tools, functions, workflows that I use for my everyday scientific work.
 
 ## Installation
```

### Comparing `CKAstroTools-0.0.4/ckastrotools/io/subcube.py` & `CKAstroTools-0.0.5/ckastrotools/io/subcube.py`

 * *Files identical despite different names*

### Comparing `CKAstroTools-0.0.4/ckastrotools/milkyway/spiralarms.py` & `CKAstroTools-0.0.5/ckastrotools/milkyway/spiralarms.py`

 * *Files 8% similar despite different names*

```diff
@@ -220,25 +220,35 @@
     elif model == 'ck2021':
         spiral_arm_params = ck2021
 
     return spiral_arm_params
 
 
 def getSpiralArm(name, model='reid2014',
+                 glon_min=-np.inf, glon_max=np.inf,
+                 r_gal_min=0., r_gal_max=np.inf,
                  resolution=0.0001, R_0=8.34):
     """
     Get the spiral arm model for a given arm name.
 
     Parameters
     ----------
     name: str
         Name of the spiral arm.
     model: str
         Name of the spiral arm model to be used.
         Available models: reid2014 (default), ck, vallee2015.
+    glon_min: float
+        Minimum galactic longitude [deg] of the spiral arm in degrees.
+    glon_max: float
+        Maximum galactic longitude [deg] of the spiral arm in degrees.
+    r_gal_min: float
+        Minimum galactocentric distance [kpc] of the spiral arm in kpc.
+    r_gal_max: float
+        Maximum galactocentric distance [kpc] of the spiral arm in kpc.
     resolution: float
         Resolution of the spiral arm model in degrees.
     R_0: float
         Galactocentric distance of the sun in kpc.
 
     Returns
     -------
@@ -261,14 +271,18 @@
     y = R_gal * np.cos((90 - beta) * np.pi / 180.)
 
     arm = SkyCoord(frame='galactocentric', x=x*u.kpc, y=y*u.kpc, z=0.0*u.kpc,
                    galcen_distance=R_0*u.kpc,
                    galcen_coord=SkyCoord(frame='galactic', l=0*u.deg, b=0*u.deg).icrs,
                    z_sun=0.*u.kpc,
                    roll=0.).galactocentric
+    arm = arm[arm.galactic.l.degree > glon_min]
+    arm = arm[arm.galactic.l.degree < glon_max]
+    arm = arm[arm.galactic.distance.kpc > r_gal_min]
+    arm = arm[arm.galactic.distance.kpc < r_gal_max]
     return arm
 
 
 def getSpiralArmsDetail(model='reid2019'):
 
     # if model=='optimized':
     #     # SAGITTARIUS arm
```

### Comparing `CKAstroTools-0.0.4/pyproject.toml` & `CKAstroTools-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
             "pytest",
             "pytest-mock"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "CKAstroTools"
 description = "General toolks for astronomy I personally use regularly for data analysis."
-version = "0.0.4"
+version = "0.0.5"
 requires-python = ">=3.7"
 dependencies = ["spectral-cube"]
 keywords = []
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
```

