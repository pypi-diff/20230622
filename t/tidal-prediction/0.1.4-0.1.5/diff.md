# Comparing `tmp/tidal-prediction-0.1.4.tar.gz` & `tmp/tidal-prediction-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tidal-prediction-0.1.4.tar", last modified: Thu Oct  4 22:18:56 2018, max compression
+gzip compressed data, was "tidal-prediction-0.1.5.tar", last modified: Thu Jun 22 16:15:02 2023, max compression
```

## Comparing `tidal-prediction-0.1.4.tar` & `tidal-prediction-0.1.5.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxrwxr-x   0 jbl       (1000) jbl       (1000)        0 2018-10-04 22:18:56.000000 tidal-prediction-0.1.4/
--rw-rw-r--   0 jbl       (1000) jbl       (1000)      267 2018-10-04 22:18:56.000000 tidal-prediction-0.1.4/PKG-INFO
-drwxrwxr-x   0 jbl       (1000) jbl       (1000)        0 2018-10-04 22:18:56.000000 tidal-prediction-0.1.4/tidal_prediction.egg-info/
--rw-rw-r--   0 jbl       (1000) jbl       (1000)       17 2018-10-04 22:18:56.000000 tidal-prediction-0.1.4/tidal_prediction.egg-info/top_level.txt
--rw-rw-r--   0 jbl       (1000) jbl       (1000)      267 2018-10-04 22:18:56.000000 tidal-prediction-0.1.4/tidal_prediction.egg-info/PKG-INFO
--rw-rw-r--   0 jbl       (1000) jbl       (1000)        1 2018-10-04 22:18:56.000000 tidal-prediction-0.1.4/tidal_prediction.egg-info/dependency_links.txt
--rw-rw-r--   0 jbl       (1000) jbl       (1000)       38 2018-10-04 22:18:56.000000 tidal-prediction-0.1.4/tidal_prediction.egg-info/requires.txt
--rw-rw-r--   0 jbl       (1000) jbl       (1000)      541 2018-10-04 22:18:56.000000 tidal-prediction-0.1.4/tidal_prediction.egg-info/SOURCES.txt
--rw-rw-r--   0 jbl       (1000) jbl       (1000)       38 2018-10-04 22:18:56.000000 tidal-prediction-0.1.4/setup.cfg
-drwxrwxr-x   0 jbl       (1000) jbl       (1000)        0 2018-10-04 22:18:56.000000 tidal-prediction-0.1.4/tidal_prediction/
--rw-rw-r--   0 jbl       (1000) jbl       (1000)        0 2018-05-23 09:17:37.000000 tidal-prediction-0.1.4/tidal_prediction/__init__.py
-drwxrwxr-x   0 jbl       (1000) jbl       (1000)        0 2018-10-04 22:18:56.000000 tidal-prediction-0.1.4/tidal_prediction/tide/
--rw-rw-r--   0 jbl       (1000) jbl       (1000)    12311 2018-10-04 22:05:40.000000 tidal-prediction-0.1.4/tidal_prediction/tide/tidemodel.py
--rw-rw-r--   0 jbl       (1000) jbl       (1000)    26381 2018-06-18 12:13:49.000000 tidal-prediction-0.1.4/tidal_prediction/tide/tideutils.py
--rw-rw-r--   0 jbl       (1000) jbl       (1000)     3912 2018-06-18 12:13:49.000000 tidal-prediction-0.1.4/tidal_prediction/tide/tideconstit.py
--rw-rw-r--   0 jbl       (1000) jbl       (1000)        0 2018-05-23 09:17:37.000000 tidal-prediction-0.1.4/tidal_prediction/tide/__init__.py
--rw-rw-r--   0 jbl       (1000) jbl       (1000)     3951 2018-06-19 07:06:38.000000 tidal-prediction-0.1.4/tidal_prediction/tide/nc.py
-drwxrwxr-x   0 jbl       (1000) jbl       (1000)        0 2018-10-04 22:18:56.000000 tidal-prediction-0.1.4/tidal_prediction/convert/
--rw-rw-r--   0 jbl       (1000) jbl       (1000)      429 2018-06-18 12:13:49.000000 tidal-prediction-0.1.4/tidal_prediction/convert/io_nc.py
--rw-rw-r--   0 jbl       (1000) jbl       (1000)        0 2018-05-23 09:17:37.000000 tidal-prediction-0.1.4/tidal_prediction/convert/__init__.py
--rw-rw-r--   0 jbl       (1000) jbl       (1000)     5102 2018-06-27 11:49:28.000000 tidal-prediction-0.1.4/README.md
--rw-rw-r--   0 jbl       (1000) jbl       (1000)      503 2018-10-04 22:12:59.000000 tidal-prediction-0.1.4/setup.py
-drwxrwxr-x   0 jbl       (1000) jbl       (1000)        0 2018-10-04 22:18:56.000000 tidal-prediction-0.1.4/scripts/
--rwxrwxr-x   0 jbl       (1000) jbl       (1000)    28396 2018-05-23 09:17:37.000000 tidal-prediction-0.1.4/scripts/extract_local_model.py
--rwxrwxr-x   0 jbl       (1000) jbl       (1000)     1740 2018-05-23 09:24:06.000000 tidal-prediction-0.1.4/scripts/predict_tide.py
+drwxrwxr-x   0 jbl       (1000) jbl       (1000)        0 2023-06-22 16:15:02.064561 tidal-prediction-0.1.5/
+-rw-rw-r--   0 jbl       (1000) jbl       (1000)     1077 2021-02-15 11:47:25.000000 tidal-prediction-0.1.5/LICENSE
+-rw-rw-r--   0 jbl       (1000) jbl       (1000)      779 2021-02-15 11:47:25.000000 tidal-prediction-0.1.5/LICENSE.BASEMAP
+-rw-rw-r--   0 jbl       (1000) jbl       (1000)    19092 2021-02-15 11:47:25.000000 tidal-prediction-0.1.5/LICENSE.OTPS.pdf
+-rw-rw-r--   0 jbl       (1000) jbl       (1000)      339 2023-06-22 16:15:02.064561 tidal-prediction-0.1.5/PKG-INFO
+-rw-rw-r--   0 jbl       (1000) jbl       (1000)     5102 2021-02-15 11:47:25.000000 tidal-prediction-0.1.5/README.md
+drwxrwxr-x   0 jbl       (1000) jbl       (1000)        0 2023-06-22 16:15:02.064561 tidal-prediction-0.1.5/scripts/
+-rwxrwxr-x   0 jbl       (1000) jbl       (1000)    28396 2021-02-15 11:47:25.000000 tidal-prediction-0.1.5/scripts/extract_local_model.py
+-rwxrwxr-x   0 jbl       (1000) jbl       (1000)     1740 2021-02-15 11:47:25.000000 tidal-prediction-0.1.5/scripts/predict_tide.py
+-rw-rw-r--   0 jbl       (1000) jbl       (1000)       38 2023-06-22 16:15:02.064561 tidal-prediction-0.1.5/setup.cfg
+-rw-rw-r--   0 jbl       (1000) jbl       (1000)      503 2023-06-22 16:13:19.000000 tidal-prediction-0.1.5/setup.py
+drwxrwxr-x   0 jbl       (1000) jbl       (1000)        0 2023-06-22 16:15:02.064561 tidal-prediction-0.1.5/tidal_prediction/
+-rw-rw-r--   0 jbl       (1000) jbl       (1000)        0 2021-02-15 11:47:25.000000 tidal-prediction-0.1.5/tidal_prediction/__init__.py
+drwxrwxr-x   0 jbl       (1000) jbl       (1000)        0 2023-06-22 16:15:02.064561 tidal-prediction-0.1.5/tidal_prediction/convert/
+-rw-rw-r--   0 jbl       (1000) jbl       (1000)        0 2021-02-15 11:47:25.000000 tidal-prediction-0.1.5/tidal_prediction/convert/__init__.py
+-rw-rw-r--   0 jbl       (1000) jbl       (1000)      429 2021-02-15 11:47:25.000000 tidal-prediction-0.1.5/tidal_prediction/convert/io_nc.py
+drwxrwxr-x   0 jbl       (1000) jbl       (1000)        0 2023-06-22 16:15:02.064561 tidal-prediction-0.1.5/tidal_prediction/tide/
+-rw-rw-r--   0 jbl       (1000) jbl       (1000)        0 2021-02-15 11:47:25.000000 tidal-prediction-0.1.5/tidal_prediction/tide/__init__.py
+-rw-rw-r--   0 jbl       (1000) jbl       (1000)     3951 2021-02-15 11:47:25.000000 tidal-prediction-0.1.5/tidal_prediction/tide/nc.py
+-rw-rw-r--   0 jbl       (1000) jbl       (1000)     3912 2021-02-15 11:47:25.000000 tidal-prediction-0.1.5/tidal_prediction/tide/tideconstit.py
+-rw-rw-r--   0 jbl       (1000) jbl       (1000)    12311 2021-02-15 11:47:25.000000 tidal-prediction-0.1.5/tidal_prediction/tide/tidemodel.py
+-rw-rw-r--   0 jbl       (1000) jbl       (1000)    26373 2023-06-22 16:12:04.000000 tidal-prediction-0.1.5/tidal_prediction/tide/tideutils.py
+drwxrwxr-x   0 jbl       (1000) jbl       (1000)        0 2023-06-22 16:15:02.064561 tidal-prediction-0.1.5/tidal_prediction.egg-info/
+-rw-rw-r--   0 jbl       (1000) jbl       (1000)      339 2023-06-22 16:15:01.000000 tidal-prediction-0.1.5/tidal_prediction.egg-info/PKG-INFO
+-rw-rw-r--   0 jbl       (1000) jbl       (1000)      582 2023-06-22 16:15:01.000000 tidal-prediction-0.1.5/tidal_prediction.egg-info/SOURCES.txt
+-rw-rw-r--   0 jbl       (1000) jbl       (1000)        1 2023-06-22 16:15:01.000000 tidal-prediction-0.1.5/tidal_prediction.egg-info/dependency_links.txt
+-rw-rw-r--   0 jbl       (1000) jbl       (1000)       38 2023-06-22 16:15:01.000000 tidal-prediction-0.1.5/tidal_prediction.egg-info/requires.txt
+-rw-rw-r--   0 jbl       (1000) jbl       (1000)       17 2023-06-22 16:15:01.000000 tidal-prediction-0.1.5/tidal_prediction.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tidal-prediction-0.1.4/tidal_prediction/tide/tidemodel.py` & `tidal-prediction-0.1.5/tidal_prediction/tide/tidemodel.py`

 * *Files identical despite different names*

### Comparing `tidal-prediction-0.1.4/tidal_prediction/tide/tideutils.py` & `tidal-prediction-0.1.5/tidal_prediction/tide/tideutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,16 +64,16 @@
     Note N is not N', i.e. N is decreasing with time.
 
     TIME is UTC in decimal Modified Julian Day (MJD).
     All longitudes returned in degrees.
 
     R. D. Ray, NASA/GSFC   August 2003
 
-    Most of the formulae for mean longitudes are extracted from 
-    Jean Meeus, Astronomical Algorithms, 2nd ed., 1998.  
+    Most of the formulae for mean longitudes are extracted from
+    Jean Meeus, Astronomical Algorithms, 2nd ed., 1998.
     Page numbers below refer to this book.
 
     Note: This routine uses TIME in UT and does not distinguish between
     the subtle differences of UTC, UT1, etc.  This is more than adequate
     for the calculation of these arguments, especially in tidal studies.
     """
 
@@ -121,17 +121,17 @@
         pm = pm % circle
 
         return s, h, p, N, pm
 
 
 def polint(xa, ya, n, x):
     """\
-    given arrays xa and ya of length n and a value x, this routine returns a 
+    given arrays xa and ya of length n and a value x, this routine returns a
     value y and an error estimate dy. if p(x) is the polynomial of degree n-1
-    such that ya = p(xa) ya then the returned value is y = p(x) 
+    such that ya = p(xa) ya then the returned value is y = p(x)
 
     input:
     xa(0:n-1) = array of x values
     ya(0:n-1) = array of y values
     n       = order of interpolant, 2=linear, 3=quadratic ...
     x       = x value where interpolation is desired
 
@@ -181,15 +181,15 @@
             ns = ns - 1
         y = y + dy
     return y, dy
 
 
 class Deltat:
     """\
-    This routine computes the difference between 
+    This routine computes the difference between
     universal time and dynamical time.
 
     tjd  = UT julian day number
 
     Returns
     deltat = ET - UT in seconds
 
@@ -407,15 +407,15 @@
     fs = f * np.sin((arg + u) * rad)
 
     return fc, fs
 
 
 def fu_nodal(omega, p, constituent):
     """\
-    Computes tidal nodal (& perigee) corrections "f" and "u" 
+    Computes tidal nodal (& perigee) corrections "f" and "u"
     for n tidal constituents,
     given the mean longitudes p and omega.
 
     Input:
        omega - mean longitude of lunar node, in degrees.
        p     - mean longitude of lunar perigee.
        consituent - array of constituent names
@@ -580,15 +580,15 @@
     return pf, pu
 
 
 def nodal_A(mjd, constids):
     """\
     At a specific time, calculate nodal factors for constituents at
     all points
- 
+
     Based on subroutine ptide() by Lana Erofeeva, June 2004
     """
     const_idx = []
     for constid in constids:
         const_idx.append(tideconstit.constid.index(constid))
 
     pf, pu = nodal(mjd)
@@ -607,15 +607,15 @@
     # To use phase shifts from constit.h time should be in seconds
     # relatively Jan 1 1992 (48622mjd)
     rebase = 48622.0
     seconds_per_day = 86400.0
     tm = (mjd - rebase) * seconds_per_day
 
     ncon = len(const_idx)
-    A = np.empty((ncon), dtype=np.complex)
+    A = np.empty((ncon), dtype=np.cdouble)
     for j in range(ncon):
         i = const_idx[j]
         if i == -1:
             continue
         A[j] = pf[i]*math.cos(omega_d[i]*tm + phase_mkB[i]+pu[i]) + \
                (pf[i]*math.sin(omega_d[i]*tm + phase_mkB[i]+pu[i]))*1.0j
     return A
@@ -689,27 +689,27 @@
     """
 
     def __init__(self, z, constids):
         nc, ny, nx = z.shape
         ncon = len(constids)
         constids8 = ['q1', 'o1', 'p1', 'k1', 'n2', 'm2', 's2', 'k2']
         # Re-order to correspond to constids8
-        z8 = np.zeros((8, ny, nx), dtype=np.complex)
+        z8 = np.zeros((8, ny, nx), dtype=np.cdouble)
         ni = 0
         for i in range(8):
             for j in range(ncon):
                 if constids[j] == constids8[i]:
                     z8[i] = z[j]
                     if i not in [2, 8]:
                         ni += 1
 
         if ni <= 6:
             raise ValueError('Not enough constituents for inference')
 
-        self.zmin = np.empty((18, ny, nx), dtype=np.complex)
+        self.zmin = np.empty((18, ny, nx), dtype=np.cdouble)
         self.zmin[0] = 0.263 * z8[0] - 0.0252 * z8[1]  # 2Q1
         self.zmin[1] = 0.297 * z8[0] - 0.0264 * z8[1]  # sigma1
         self.zmin[2] = 0.164 * z8[0] + 0.0048 * z8[1]  # rho1 +
         self.zmin[3] = 0.0140 * z8[1] + 0.0101 * z8[3]  # M1
         self.zmin[4] = 0.0389 * z8[1] + 0.0282 * z8[3]  # M1
         self.zmin[5] = 0.0064 * z8[1] + 0.0060 * z8[3]  # chi1
         self.zmin[6] = 0.0030 * z8[1] + 0.0171 * z8[3]  # pi1
```

### Comparing `tidal-prediction-0.1.4/tidal_prediction/tide/tideconstit.py` & `tidal-prediction-0.1.5/tidal_prediction/tide/tideconstit.py`

 * *Files identical despite different names*

### Comparing `tidal-prediction-0.1.4/tidal_prediction/tide/nc.py` & `tidal-prediction-0.1.5/tidal_prediction/tide/nc.py`

 * *Files identical despite different names*

### Comparing `tidal-prediction-0.1.4/README.md` & `tidal-prediction-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `tidal-prediction-0.1.4/scripts/extract_local_model.py` & `tidal-prediction-0.1.5/scripts/extract_local_model.py`

 * *Files identical despite different names*

### Comparing `tidal-prediction-0.1.4/scripts/predict_tide.py` & `tidal-prediction-0.1.5/scripts/predict_tide.py`

 * *Files identical despite different names*

