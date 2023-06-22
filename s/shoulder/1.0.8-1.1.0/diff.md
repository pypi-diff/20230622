# Comparing `tmp/shoulder-1.0.8.tar.gz` & `tmp/shoulder-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shoulder-1.0.8.tar", max compression
+gzip compressed data, was "shoulder-1.1.0.tar", max compression
```

## Comparing `shoulder-1.0.8.tar` & `shoulder-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,20 @@
--rw-r--r--   0        0        0     1097 2023-05-12 01:39:37.059210 shoulder-1.0.8/LICENSE.md
--rw-r--r--   0        0        0     1867 2023-05-12 20:38:29.614149 shoulder-1.0.8/README.md
--rw-r--r--   0        0        0      910 2023-05-24 14:53:16.753428 shoulder-1.0.8/pyproject.toml
--rw-r--r--   0        0        0      109 2023-05-12 01:39:37.059210 shoulder-1.0.8/src/shoulder/__init__.py
--rw-r--r--   0        0        0     1293 2023-05-12 01:39:37.059210 shoulder-1.0.8/src/shoulder/base.py
--rw-r--r--   0        0        0     2838 2023-05-15 14:44:39.754454 shoulder-1.0.8/src/shoulder/bone.py
--rw-r--r--   0        0        0        0 2023-05-12 01:39:37.059210 shoulder-1.0.8/src/shoulder/glenoid/__init__.py
--rw-r--r--   0        0        0        1 2023-05-12 01:39:37.059210 shoulder-1.0.8/src/shoulder/humerus/__init__.py
--rw-r--r--   0        0        0    18164 2023-05-24 14:14:18.056882 shoulder-1.0.8/src/shoulder/humerus/anatomic_neck.py
--rw-r--r--   0        0        0     3300 2023-05-24 14:14:18.056882 shoulder-1.0.8/src/shoulder/humerus/angles.py
--rw-r--r--   0        0        0    14089 2023-05-24 14:14:18.056882 shoulder-1.0.8/src/shoulder/humerus/bicipital_groove.py
--rw-r--r--   0        0        0     6628 2023-05-14 03:39:04.887022 shoulder-1.0.8/src/shoulder/humerus/canal.py
--rw-r--r--   0        0        0     5276 2023-05-24 14:14:18.056882 shoulder-1.0.8/src/shoulder/humerus/epicondyle.py
--rw-r--r--   0        0        0     7262 2023-05-24 14:10:21.631802 shoulder-1.0.8/src/shoulder/humerus/mesh.py
--rw-r--r--   0        0        0     2803 2023-05-12 01:39:37.059210 shoulder-1.0.8/src/shoulder/plotting.py
--rw-r--r--   0        0        0     6681 2023-05-12 01:39:37.059210 shoulder-1.0.8/src/shoulder/utils.py
--rw-r--r--   0        0        0     2886 1970-01-01 00:00:00.000000 shoulder-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1097 2023-06-22 14:31:55.982409 shoulder-1.1.0/LICENSE.md
+-rw-r--r--   0        0        0     1867 2023-06-22 14:31:55.982589 shoulder-1.1.0/README.md
+-rw-r--r--   0        0        0      960 2023-06-22 14:33:22.153220 shoulder-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      109 2023-06-22 14:31:55.984432 shoulder-1.1.0/src/shoulder/__init__.py
+-rw-r--r--   0        0        0     1293 2023-06-22 14:31:55.984598 shoulder-1.1.0/src/shoulder/base.py
+-rw-r--r--   0        0        0     2862 2023-06-22 14:31:55.984738 shoulder-1.1.0/src/shoulder/bone.py
+-rw-r--r--   0        0        0        0 2023-06-22 14:31:55.984909 shoulder-1.1.0/src/shoulder/glenoid/__init__.py
+-rw-r--r--   0        0        0        1 2023-06-22 14:31:55.985091 shoulder-1.1.0/src/shoulder/humerus/__init__.py
+-rw-r--r--   0        0        0    18164 2023-06-22 14:31:55.985293 shoulder-1.1.0/src/shoulder/humerus/anatomic_neck.py
+-rw-r--r--   0        0        0     3300 2023-06-22 14:31:55.985451 shoulder-1.1.0/src/shoulder/humerus/angles.py
+-rw-r--r--   0        0        0    18396 2023-06-22 14:31:55.985679 shoulder-1.1.0/src/shoulder/humerus/bicipital_groove.py
+-rw-r--r--   0        0        0     6628 2023-06-22 14:31:55.985869 shoulder-1.1.0/src/shoulder/humerus/canal.py
+-rw-r--r--   0        0        0     5276 2023-06-22 14:31:55.986035 shoulder-1.1.0/src/shoulder/humerus/epicondyle.py
+-rw-r--r--   0        0        0     7262 2023-06-22 14:31:55.986214 shoulder-1.1.0/src/shoulder/humerus/mesh.py
+-rw-r--r--   0        0        0 19631658 2023-06-22 14:31:56.060294 shoulder-1.1.0/src/shoulder/humerus/models/RFC_bg.pkl
+-rw-r--r--   0        0        0 13850118 2023-06-22 14:31:56.183273 shoulder-1.1.0/src/shoulder/humerus/models/RFC_bg2.pkl
+-rw-r--r--   0        0        0 12444896 2023-06-22 14:31:56.197936 shoulder-1.1.0/src/shoulder/humerus/models/RFC_bg_a.pkl
+-rw-r--r--   0        0        0     2803 2023-06-22 14:31:56.199047 shoulder-1.1.0/src/shoulder/plotting.py
+-rw-r--r--   0        0        0     6681 2023-06-22 14:31:56.199221 shoulder-1.1.0/src/shoulder/utils.py
+-rw-r--r--   0        0        0     2886 1970-01-01 00:00:00.000000 shoulder-1.1.0/PKG-INFO
```

### Comparing `shoulder-1.0.8/LICENSE.md` & `shoulder-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `shoulder-1.0.8/README.md` & `shoulder-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `shoulder-1.0.8/pyproject.toml` & `shoulder-1.1.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shoulder"
-version = "1.0.8"
+version = "1.1.0"
 description = "patient specific anatomic coordinate system generation for shoulder bones"
 authors = ["Gregory W Spangenberg <gspangen@westerneng.ca>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/gregspangenberg/shoulder"
 
 [tool.poetry.dependencies]
@@ -28,11 +28,13 @@
 nbformat = "^5.7.0"
 pwlf = "^2.2.1"
 pyglet = "~1.5"
 ipywidgets = "^7"
 pandas = "^2.0.1"
 statsmodels = "^0.14.0"
 snakeviz = "^2.2.0"
+imbalanced-learn = "^0.10.1"
+xgboost = "^1.7.5"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `shoulder-1.0.8/src/shoulder/base.py` & `shoulder-1.1.0/src/shoulder/base.py`

 * *Files identical despite different names*

### Comparing `shoulder-1.0.8/src/shoulder/bone.py` & `shoulder-1.1.0/src/shoulder/bone.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         self.transform = np.identity(4)
         msh = mesh.FullObb(stl_file)
         self._mesh = msh
 
         self.canal = canal.Canal(msh)
         self.trans_epiconylar = epicondyle.TransEpicondylar(msh)
         self.anatomic_neck = anatomic_neck.AnatomicNeck(msh, self.trans_epiconylar)
-        self.bicipital_groove = bicipital_groove.DeepGroove(msh)
+        self.bicipital_groove = bicipital_groove.DeepGroove(msh, self.canal)
 
     def apply_csys_canal_transepiconylar(self) -> np.ndarray:
         self.transform = construct_csys(self.canal._axis, self.trans_epiconylar._axis)
         self._update_landmark_data(self.transform)
         return self.transform
 
 
@@ -41,15 +41,15 @@
         self.stl_file = stl_file
         self.transform = np.identity(4)
 
         msh = mesh.ProxObb(stl_file)
         self._mesh = msh
 
         self.canal = canal.Canal(msh)
-        self.bicipital_groove = bicipital_groove.DeepGroove(msh)
+        self.bicipital_groove = bicipital_groove.DeepGroove(msh, self.canal)
 
     def apply_csys_canal_articular(self, articular) -> np.ndarray:
         self.transform = construct_csys(self.canal._axis, articular)
         self._update_landmark_data(self.transform)
         return self.transform
```

### Comparing `shoulder-1.0.8/src/shoulder/humerus/anatomic_neck.py` & `shoulder-1.1.0/src/shoulder/humerus/anatomic_neck.py`

 * *Files identical despite different names*

### Comparing `shoulder-1.0.8/src/shoulder/humerus/angles.py` & `shoulder-1.1.0/src/shoulder/humerus/angles.py`

 * *Files identical despite different names*

### Comparing `shoulder-1.0.8/src/shoulder/humerus/bicipital_groove.py` & `shoulder-1.1.0/src/shoulder/humerus/bicipital_groove.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,162 +1,344 @@
 from shoulder import utils
 from shoulder.base import Landmark
 
-import ruptures
 import numpy as np
+import math
 import scipy.signal
 import skspatial.objects
 import plotly.graph_objects as go
-from functools import cached_property
-import matplotlib.pyplot as plt
+import pandas as pd
+
+import ruptures
+from sklearn.preprocessing import MinMaxScaler, StandardScaler
+import sklearn.neighbors
+import pickle
+
+import pathlib
+import importlib.resources
 
 
 class DeepGroove(Landmark):
-    def __init__(self, obb):
+    def __init__(self, obb, canal):
         self._mesh_oriented_uobb = obb.mesh
         self._transform_uobb = obb.transform
         self._obb_cutoff_pcts = obb.cutoff_pcts
+        self._canal_axis = canal.axis()
         self._points_ct = None
         self._points = None
         self._axis_ct = None
         self._axis = None
+        self._X = None
+        self._y = None
 
-    def axis(self, cutoff_pcts=[0.35, 0.85], slice_num=35, interp_num=250):
-        def _multislice(mesh, zs, interp_num, slice_num):
+    def axis(
+        self, cutoff_pcts=[0.35, 0.85], zslice_num=300, interp_num=1000, deg_window=6
+    ):
+        def _multislice(mesh, zs, interp_num, zslice_num):
             # preallocate variables
-            xy = np.zeros((interp_num, 2, slice_num))
-            polar = np.zeros((interp_num, 2, slice_num))
-            weights = np.zeros((interp_num, 2, slice_num))
-            to_3Ds = np.zeros((4, 4, slice_num))
+            polar = np.zeros(
+                (
+                    zslice_num,
+                    2,
+                    interp_num,
+                )
+            )
+            weights = np.zeros((zslice_num, 2, interp_num))
+            to_3Ds = np.zeros((zslice_num, 4, 4))
 
             for i, z in enumerate(zs):
                 # grab the polygon of the slice
                 origin = [0, 0, z]
                 normal = [0, 0, 1]
                 path = mesh.section(plane_origin=origin, plane_normal=normal)
                 slice, to_3D = path.to_planar(normal=normal)
                 # keep only largest polygon
                 big_poly = slice.polygons_closed[
                     np.argmax([p.area for p in slice.polygons_closed])
                 ]
                 # resample cartesion coordinates to create evenly spaced points
-                _pts = np.asarray(big_poly.exterior.xy).T
+                _pts = np.asarray(big_poly.exterior.xy)
                 _pts = _resample_polygon(_pts, interp_num)
-
+                # _pts = _pts.T
                 # convert to polar and ensure even degree spacing
-                _pol = _cart2pol(_pts)
+                _pol = _cart2pol(_pts[0, :], _pts[1, :])
 
                 # if a cavity is present do not count that as a weight
-                # prepend -10 so first difference is positive
-                theta_diff = np.diff(_pol[:, 0], prepend=-10) < 0
-                cav_weight = _remove_cavitites(theta_diff)
-
-                # log data
-                xy[:, :, i] = _pts
-                polar[:, :, i] = _pol
-                weights[:, :, i] = cav_weight
-                to_3Ds[:, :, i] = to_3D
+                # theta_diff = np.diff(_pol[:, 0], prepend=-10) < 0
+                # print(_pol.shape)
+                # _pol = _remove_cavitites(_pol)
+                # if _pol.shape[0] != interp_num:
+                #     print(z)
+                #     print(_pol.shape)
+
+                # _pts = _pol2cart(_pol)
+                # _pts = _resample_polygon(_pts, interp_num)
+                # _pol = _cart2pol(_pts)
+                # _pol = _pol[np.argsort(_pol[:, 0]), :]
+
+                polar[i, :, :] = _pol
+                # weights[i, :, :] = cav_weight.T
+                to_3Ds[i, :, :] = to_3D
+
+            return polar, to_3Ds
+
+        def _X_process(polar, polar_0, zs):
+            def closest_angles(array, v):
+                angs = []
+                for a in array:
+                    angs.append(math.atan2(math.sin(v - a), math.cos(v - a)))
+                return np.abs(angs)
+
+            def peak_nearest(all_peaks_theta):
+                angles = []
+                if len(all_peaks_theta) == 1:
+                    return np.array([0])
+                for p in all_peaks_theta:
+                    angs = closest_angles(all_peaks_theta, p)
+                    angs = angs[np.round(angs, 2) != 0]
+                    angs.sort()
+                    angles.append(angs[0])
+
+                return np.array(angles)
+
+            def peak_next_nearest(all_peaks_theta):
+                angles = []
+                if len(all_peaks_theta) == 1:
+                    return np.array([0])
+                if len(all_peaks_theta) == 2:
+                    return np.array([0, 0])
+                for p in all_peaks_theta:
+                    angs = closest_angles(all_peaks_theta, p)
+                    angs = angs[np.round(angs, 2) != 0]
+                    angs.sort()
+                    angles.append(angs[1])
+
+                return np.array(angles)
+
+            def canal_dist(self, theta_peaks, radius_peaks, z_peaks):
+                # repeat z_peaks for the length of the peaks
+                z_peaks = np.repeat(z_peaks, len(theta_peaks))
+
+                canal_u = utils.unit_vector(self._canal_axis[0], self._canal_axis[1])
+                # get canal points at the z heights
+                canal_pts = canal_u.reshape(-1, 1) @ z_peaks.reshape(1, -1)
+                canal_pts = canal_pts[:2, :]  # remove z
+                peak_pts = _pol2cart(np.c_[theta_peaks, radius_peaks]).T
+
+                dist = peak_pts - canal_pts
+                dist = np.sqrt(np.sum(dist**2, axis=0))  # get distance
+
+                return dist
+
+            def theta_zstd(polar, peak):
+                allradi_atpeak = polar[:, 1, peak]
+
+                return allradi_atpeak.flatten().std()
+
+            # def theta_near_zstd(polar0, peak):
+            #     allradi_atpeak = polar0[:, 1, peak].flatten()
+
+            #     n = len(allradi_atpeak)
+            #     stds = []
+            #     window = 3
+            #     padding = int((window - 1) / 2)
+            #     pad_rp = np.pad(allradi_atpeak, ((0, 0), (padding, padding)), "edge")
+            #     np.lib.stride_tricks.sliding_window_view(pad_rp, window, axis=1)
+
+            #     return n
+            # def radial_change_above(polar0, peak, z):
+            #     allradi_atpeak = polar0[:, 1, peak].flatten()
+
+            #     n = len(allradi_atpeak)
+            #     window = 3
+            #     padding = int((window - 1) / 2)
+            #     pad_rp = np.pad(allradi_atpeak, ((0, 0), (padding, padding)), "edge")
+            #     np.lib.stride_tricks.sliding_window_view(pad_rp, window, axis=1)
+
+            #     return n
+
+            z_scale = MinMaxScaler().fit_transform(zs.reshape(-1, 1)).flatten()
+            peak_zs = []
+            peak_theta = []
+            peak_radius = []
+            peak_near = []
+            peak_next_near = []
+            peak_prom = []
+            peak_width = []
+            peak_widthheight = []
+            peak_canal_dist = []
+            peak_num = []
+            peak_zstd = []
+
+            for i, (rpol, rpol0) in enumerate(zip(polar, polar_0)):
+                theta = rpol0[0]
+                radius = rpol0[1]
+                radius_og = rpol[1]
+                radius = -1 * radius
+                radius = scipy.signal.savgol_filter(radius, 10, 1)
+
+                # sometimes the start or end contains a peak we need to shift
+                rmin = -1 * np.argmin(radius)
+                radius_roll = np.roll(radius, rmin)
+                # now find peaks
+                peaks, _prop = scipy.signal.find_peaks(
+                    radius_roll,
+                    height=-10,
+                    prominence=0.6,
+                    width=0.1,
+                )
+                peaks = (peaks - rmin) % interp_num
+
+                # if there are more than 10 peaks discard the lowest prominence one
+                n = 5
+                if len(peaks) > n:
+                    part = np.argpartition(_prop["prominences"], -n)[-n:]
+                    peaks = peaks[part]  # top n largest
+
+                    for k, v in _prop.items():
+                        _prop[k] = [v[i] for i in part]
+
+                peak_theta.extend(theta[peaks])
+                peak_radius.extend(radius_og[peaks])
+                peak_near.extend(peak_nearest(theta[peaks]))
+                peak_next_near.extend(peak_next_nearest(theta[peaks]))
+                peak_zs.extend([z_scale[i]] * len(peaks))
+                peak_prom.extend(_prop["prominences"])
+                peak_width.extend(_prop["widths"])
+                peak_widthheight.extend(_prop["width_heights"])
+                peak_canal_dist.extend(
+                    canal_dist(self, theta[peaks], radius_og[peaks], zs[i])
+                )
+                peak_num.extend(np.repeat((len(peaks) / n), len(peaks)))
+                peak_zstd.extend([theta_zstd(polar, p) for p in peaks])
+
+            X = pd.DataFrame(
+                {
+                    "peak_theta": peak_theta,
+                    "peak_radius": peak_radius,
+                    "peak_near": peak_near,
+                    "peak_next_near": peak_next_near,
+                    "peak_z": peak_zs,
+                    "peak_prom": peak_prom,
+                    "peak_width": peak_width,
+                    "peak_widthheight": peak_widthheight,
+                    "peak_canal_dist": peak_canal_dist,
+                    "peak_num": peak_num,
+                    "peak_zstd": peak_zstd,
+                }
+            )
+
+            self._X = X.copy()
 
-            return xy, polar, weights, to_3Ds
+            scaler = StandardScaler()
+            col_modify = [
+                "peak_theta",
+                "peak_radius",
+                "peak_near",
+                "peak_next_near",
+                "peak_prom",
+                "peak_width",
+                "peak_widthheight",
+                "peak_canal_dist",
+                "peak_zstd",
+                "peak_num",
+                "peak_z",
+            ]
+            for col in col_modify:
+                X[col] = scaler.fit_transform(X[col].values.reshape(-1, 1)).flatten()
+
+            # X = X.drop(["peak_theta", "peak_canal_dist", "peak_zstd"], axis=1)
+            X = X.drop(["peak_theta"], axis=1)
+            return X, np.array(peak_theta), np.array(peak_zs), np.array(peak_num)
 
         if self._axis is None:
             proximal_cutoff, distal_cutoff = self._surgical_neck_cutoff_zs(*cutoff_pcts)
-            # slice_num  must use odd soo add 1 if even
-            if (slice_num % 2) == 0:
-                slice_num += 1
+            # slice_num  must use odd soo 1 if even
+            if (zslice_num % 2) == 0:
+                zslice_num += 1
 
-            zs = np.linspace(distal_cutoff, proximal_cutoff, num=slice_num).flatten()
+            zs = np.linspace(distal_cutoff, proximal_cutoff, num=zslice_num).flatten()
 
-            xy, polar, weights, to_3Ds = _multislice(
-                self._mesh_oriented_uobb, zs, interp_num, slice_num
+            polar, to_3Ds = _multislice(
+                self._mesh_oriented_uobb, zs, interp_num, zslice_num
             )
-            # make each radial slice stationary
+            # make each radial slice stationary by subtracting the mean
             polar_0 = polar.copy()
             polar_0[:, 1, :] = np.apply_along_axis(
-                lambda x: x - np.mean(x), axis=0, arr=polar[:, 1, :]
+                lambda x: x - np.mean(x), axis=1, arr=polar[:, 1, :]
             )
 
-            # calculate weighted mean across slices where cavities have a weight of 0
-            polar_avg_0 = np.average(polar_0, axis=2, weights=weights)
-            deg = np.rad2deg(polar_avg_0[:, 0])
-            radius = polar_avg_0[:, 1]
-            # weights create jagged edges
-            radius = scipy.signal.savgol_filter(radius, 10, 1)
+            # preprocess the data to get in the correct format
+            X, peak_theta, peak_zs, peak_num = _X_process(polar, polar_0, zs)
 
-            # calulate derivatives
-            dd_radius = _derivative_smooth_ends(radius, 2, 10, 2)
-
-            peaks, _prop = scipy.signal.find_peaks(
-                dd_radius, height=0, distance=interp_num / 360 * 25
-            )
-            peaks = peaks[
-                np.argpartition(_prop["peak_heights"], -3)[-3:]
-            ]  # top 3 largest
-
-            # find the peaks that are not near the furthest point
-            # the furthest point is on the articular surface so any peaks neighbouring there
-            # would not be the biciptal groove
-            peaks.sort()
-            deg_rmax = deg[np.argmax(radius)]
-            deg_peaks = deg[peaks]
-            filt_vals = np.r_[deg_peaks, deg_rmax]
-            deg_shft = np.r_[deg[peaks[0] :], deg[: peaks[0]], deg[peaks[0]]]
-            filt = [x for x in deg_shft if x in filt_vals]
-            non_bg_peaks = (
-                filt[filt.index(deg_rmax) - 1],
-                filt[filt.index(deg_rmax) + 1],
-            )
-            bg_peak = list(set(deg_peaks) - set(non_bg_peaks))[0]
+            # open model
+            with open(
+                importlib.resources.files("shoulder") / "humerus/models/RFC_bg_a.pkl",
+                "rb",
+            ) as file:
+                clf = pickle.load(file)
+            # apply activation kernel
+            kde = sklearn.neighbors.KernelDensity(kernel="linear")
+            print(peak_theta[clf.predict_proba(X)[:, 1] > 0.6].reshape(-1, 1).shape)
+            kde.fit(peak_theta[clf.predict_proba(X)[:, 1] > 0.6].reshape(-1, 1))
+            tlin = np.linspace(-1 * np.pi, np.pi, 1000).reshape(-1, 1)
+            bg_prob = np.exp(kde.score_samples(tlin))
+            bg_theta = tlin[np.argmax(bg_prob)][0]
 
             # get local minima by specifying serach window for
             # search up to 15 degrees away on each side
-            deg_variance = int(round(360 / interp_num) * 15)
-            bg_xyz = np.zeros((1, 3, len(zs)))
+            ivar = int(round(deg_window / (360 / interp_num)))
+
+            if ivar < 1:
+                ivar = 1
+            bg_xyz = np.zeros((len(zs), 3))
+            bg_local_theta = np.zeros((len(zs), 1))
             for i, z in enumerate(zs):
-                # print(polar_0)
-                bg_idx_near = _find_nearest_idx(
-                    polar_0[:, 0, i].flatten(), np.deg2rad(bg_peak)
-                )
+                bg_i_esti = _find_nearest_idx(polar_0[i, 0, :].flatten(), bg_theta)
+
                 # sometimes the degree variance will be higher than than the index bg is found at
                 # when this occurs the indexing will start with a negative numebr causing it to fail
                 # basically a wrap around problem
-
-                if deg_variance > bg_idx_near:
+                if ivar > bg_i_esti:
                     bg_range = np.concatenate(
                         (
-                            polar_0[(bg_idx_near - deg_variance) :, :, i],
-                            polar_0[: (bg_idx_near + deg_variance), :, i],
+                            polar_0[i, :, (bg_i_esti - ivar) :],
+                            polar_0[i, :, : (bg_i_esti + ivar)],
                         ),
-                        axis=0,
+                        axis=1,
                     )
                 else:
                     bg_range = polar_0[
-                        (bg_idx_near - deg_variance) : (bg_idx_near + deg_variance),
-                        :,
                         i,
+                        :,
+                        (bg_i_esti - ivar) : (bg_i_esti + ivar),
                     ]
-                bg_local_i = np.argmin(bg_range[:, 1])
-
+                bg_i_local = np.argmin(bg_range[1, :])
                 # transform back to radial coordinates
-                bg_i = bg_local_i + (bg_idx_near - deg_variance)  # put back in context
-                _bg_xy = _pol2cart(polar[bg_i, :, i].reshape(1, 2))
-
-                # i think to_3D is perhaps fully broken, doesn't seem to work
-                bg_xyz[:, :, i] = utils.transform_pts(np.c_[_bg_xy, 0], to_3Ds[:, :, i])
-
-            bg_xyz = bg_xyz.transpose(2, 1, 0).reshape(-1, 3)
+                bg_i_local = bg_i_local + (bg_i_esti - ivar)  # put back in context
+                bg_i_theta = polar[i, 0, bg_i_local]
+                bg_local_theta[i, :] = bg_i_theta
+                _bg_xy = _pol2cart(
+                    polar[
+                        i,
+                        :,
+                        bg_i_local,
+                    ].reshape(1, 2)
+                )
+                bg_xyz[i, :] = utils.transform_pts(np.c_[_bg_xy, 0], to_3Ds[i, :, :])
 
             # transform back
             bg_xyz = utils.transform_pts(
                 bg_xyz, utils.inv_transform(self._transform_uobb)
             )
 
             # construct an estimate of the bicipital groove axis from the bg_xyz pts
             line_ends = _fit_line(bg_xyz)
 
+            self._y = bg_local_theta
             self._axis_ct = line_ends
             self._axis = line_ends
             self._points_ct = bg_xyz
             self._points = bg_xyz
 
         return self._axis
 
@@ -187,15 +369,14 @@
         z_min = np.min(self._mesh_oriented_uobb.bounds[:, -1])
         z_length = abs(z_max) + abs(z_min)
 
         z_low_pct = self._obb_cutoff_pcts[0]
         z_high_pct = self._obb_cutoff_pcts[1]
         distal_cutoff = z_low_pct * z_length + z_min
         proximal_cutoff = z_high_pct * z_length + z_min
-        # print(distal_cutoff)
 
         z_intervals = np.linspace(distal_cutoff, 0.99 * z_max, 100)
 
         z_area = np.zeros(len(z_intervals))
         for i, z in enumerate(z_intervals):
             slice = self._mesh_oriented_uobb.section(
                 plane_origin=[0, 0, z], plane_normal=[0, 0, 1]
@@ -217,51 +398,28 @@
 
         # interval on which to calcaulte bicipital groove
         return [bottom, top]
 
 
 def _find_nearest_idx(array, value):
     idx = np.searchsorted(array, value, side="left")
-    if idx > 0 and (
-        idx == len(array) or np.abs(value - array[idx - 1]) < np.abs(value - array[idx])
-    ):
+
+    if idx == len(array):
         return idx - 1
     else:
         return idx
 
 
-def _reorder_by_theta(arr):
-    """reorder the array to start at the most negative theta.
-    only works when it is an ordered array from a path object"""
-
-    re_arr = np.r_[arr[np.argmin(arr[:, 0]) :], arr[: np.argmin(arr[:, 0])]]
-    # there is an error that can occur when the most positive number which should be at
-    # the end has a negative theta
-    if re_arr[-1, 0] < 0:
-        re_arr[-1, 0] = np.deg2rad(179.99)
-
-    return re_arr
-
-
-def _cart2pol(arr: np.ndarray) -> np.ndarray:
-    """convert from cartesian coordinates to radial
-
-    Args:
-        arr (np.ndarray): cartesian coordiantes
-
-    Returns:
-        np.ndarray: radial coordinates
-    """
-    x = arr[:, 0]
-    y = arr[:, 1]
+def _cart2pol(x: np.ndarray, y: np.ndarray) -> np.ndarray:
+    """convert from cartesian coordinates to radial"""
     r = np.sqrt(x**2 + y**2)
     theta = np.arctan2(y, x)
-    r_arr = np.c_[theta, r]
-    # r_arr = r_arr[r_arr[:,1].argsort()] # sort by theta angle
-    r_arr = _reorder_by_theta(r_arr)
+    sorter = np.argsort(theta)
+    r_arr = np.vstack((theta[sorter], r[sorter]))
+
     return r_arr
 
 
 def _pol2cart(arr):
     r = arr[:, 1]
     theta = arr[:, 0]
     x = r * np.cos(theta)
@@ -278,68 +436,30 @@
         n_points (int, optional): number of evenly spaced points to return. Defaults to 100.
 
     Returns:
         np.ndarray: evenly spaced points
     """
     # Cumulative Euclidean distance between successive polygon points.
     # This will be the "x" for interpolation
-    d = np.cumsum(np.r_[0, np.sqrt((np.diff(xy, axis=0) ** 2).sum(axis=1))])
+    d = np.cumsum(np.r_[0, np.sqrt((np.diff(xy, axis=1) ** 2).sum(axis=0))])
 
     # get linearly spaced points along the cumulative Euclidean distance
     d_sampled = np.linspace(0, d.max(), n_points)
 
     # interpolate x and y coordinates
-    xy_interp = np.c_[
-        np.interp(d_sampled, d, xy[:, 0]),
-        np.interp(d_sampled, d, xy[:, 1]),
-    ]
+    xy_interp = np.vstack(
+        (
+            np.interp(d_sampled, d, xy[0, :]),
+            np.interp(d_sampled, d, xy[1, :]),
+        )
+    )
 
     return xy_interp
 
 
-def _derivative_smooth(arr, dd_order, window, smooth_order, _depth=0):
-    """calculates nth order derivatives while smoothing in-between each step
-
-    Args:
-        arr (np.array): 1D array to calculate the derivative of
-        dd_order (int): order of derivate to calculate
-        window (int): interval upon which the smoothing occurs
-        smooth_order (int): order of function which smoothing uses
-        _depth (int, optional): . Defaults to 0.
-
-    Returns:
-        np.array: derivative of array of order n
-    """
-    if _depth == dd_order:
-        return scipy.signal.savgol_filter(arr, window, smooth_order)
-    arr = scipy.signal.savgol_filter(np.gradient(arr), window, smooth_order)
-    return _derivative_smooth(arr, dd_order, window, smooth_order, _depth + 1)
-
-
-def _derivative_smooth_ends(arr, dd_order, window, smooth_order, _depth=0):
-    """calculates nth order derivatives while smoothing at the end
-
-    Args:
-        arr (np.array): 1D array to calculate the derivative of
-        dd_order (int): order of derivate to calculate
-        window (int): interval upon which the smoothing occurs
-        smooth_order (int): order of function which smoothing uses
-        _depth (int, optional): . Defaults to 0.
-
-    Returns:
-        np.array: derivative of array of order n
-    """
-    if _depth == dd_order:  # initial pass
-        return scipy.signal.savgol_filter(arr, window, smooth_order)
-    elif _depth == 0:  # final pass
-        arr = scipy.signal.savgol_filter(arr, window, smooth_order)
-    arr = np.gradient(arr)
-    return _derivative_smooth(arr, dd_order, window, smooth_order, _depth + 1)
-
-
 def _true_propogate(arr):
     """for each true interval double the size starting at same position"""
 
     def true_interval(x):
         """find interval where true bools  occur"""
         z = np.concatenate(([False], x, [False]))
 
@@ -362,25 +482,23 @@
         else:
             a[end : end + length] = np.repeat(True, length)
 
     return a
 
 
 def _remove_cavitites(arr):
-    arr = _true_propogate(arr)
-    cav = np.array(arr, dtype=np.int32)  # make all true 1
+    # prepend -10 so first difference is positive
+    theta_diff = np.diff(arr[:, 0], prepend=-10) < 0
+    theta_diff = _true_propogate(theta_diff)
+    cav = np.array(theta_diff, dtype=np.int32)  # make all true 1
     # flip all 0s to 1s, since we want to preserve everythin but cavities
     cav = cav ^ (cav & 1 == cav)
-    # print(cav)
-    # print(cav.shape)
-    # weighting for each x,y point
-    cav_weight = np.c_[cav, cav]
-    # print(cav_weight)
-    # print(cav_weight.shape)
-    return cav_weight
+    cav = cav.astype(bool)
+
+    return arr[cav]
 
 
 def _fit_line(bg_xyz):
     x, y, z = bg_xyz.T
     z_dist = np.max(z) - np.min(z)
     line_fit = skspatial.objects.Line.best_fit(bg_xyz)
     ends = np.array(
```

### Comparing `shoulder-1.0.8/src/shoulder/humerus/canal.py` & `shoulder-1.1.0/src/shoulder/humerus/canal.py`

 * *Files identical despite different names*

### Comparing `shoulder-1.0.8/src/shoulder/humerus/epicondyle.py` & `shoulder-1.1.0/src/shoulder/humerus/epicondyle.py`

 * *Files identical despite different names*

### Comparing `shoulder-1.0.8/src/shoulder/humerus/mesh.py` & `shoulder-1.1.0/src/shoulder/humerus/mesh.py`

 * *Files identical despite different names*

### Comparing `shoulder-1.0.8/src/shoulder/plotting.py` & `shoulder-1.1.0/src/shoulder/plotting.py`

 * *Files identical despite different names*

### Comparing `shoulder-1.0.8/src/shoulder/utils.py` & `shoulder-1.1.0/src/shoulder/utils.py`

 * *Files identical despite different names*

### Comparing `shoulder-1.0.8/PKG-INFO` & `shoulder-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shoulder
-Version: 1.0.8
+Version: 1.1.0
 Summary: patient specific anatomic coordinate system generation for shoulder bones
 Home-page: https://github.com/gregspangenberg/shoulder
 License: MIT
 Author: Gregory W Spangenberg
 Author-email: gspangen@westerneng.ca
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

