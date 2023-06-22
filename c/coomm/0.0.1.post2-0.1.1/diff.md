# Comparing `tmp/COOMM-0.0.1.post2.tar.gz` & `tmp/coomm-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/COOMM-0.0.1.post2.tar", last modified: Thu Sep 15 20:18:05 2022, max compression
+gzip compressed data, was "coomm-0.1.1.tar", max compression
```

## Comparing `COOMM-0.0.1.post2.tar` & `coomm-0.1.1.tar`

### file list

```diff
@@ -1,64 +1,47 @@
-drwxr-xr-x   0 skim0119   (501) staff       (20)        0 2022-09-15 20:18:05.900548 COOMM-0.0.1.post2/
-drwxr-xr-x   0 skim0119   (501) staff       (20)        0 2022-09-15 20:18:05.899632 COOMM-0.0.1.post2/COOMM.egg-info/
--rw-r--r--   0 skim0119   (501) staff       (20)     1310 2022-09-15 20:18:05.000000 COOMM-0.0.1.post2/COOMM.egg-info/PKG-INFO
--rw-r--r--   0 skim0119   (501) staff       (20)     1537 2022-09-15 20:18:05.000000 COOMM-0.0.1.post2/COOMM.egg-info/SOURCES.txt
--rw-r--r--   0 skim0119   (501) staff       (20)        1 2022-09-15 20:18:05.000000 COOMM-0.0.1.post2/COOMM.egg-info/dependency_links.txt
--rw-r--r--   0 skim0119   (501) staff       (20)       24 2022-09-15 20:18:05.000000 COOMM-0.0.1.post2/COOMM.egg-info/requires.txt
--rw-r--r--   0 skim0119   (501) staff       (20)        6 2022-09-15 20:18:05.000000 COOMM-0.0.1.post2/COOMM.egg-info/top_level.txt
--rw-r--r--   0 skim0119   (501) staff       (20)     1073 2022-03-25 04:30:36.000000 COOMM-0.0.1.post2/LICENSE
--rw-r--r--   0 skim0119   (501) staff       (20)     1310 2022-09-15 20:18:05.900267 COOMM-0.0.1.post2/PKG-INFO
--rw-r--r--   0 skim0119   (501) staff       (20)      441 2022-09-15 20:15:35.000000 COOMM-0.0.1.post2/README.md
-drwxr-xr-x   0 skim0119   (501) staff       (20)        0 2022-09-15 20:18:05.859315 COOMM-0.0.1.post2/coomm/
--rw-r--r--   0 skim0119   (501) staff       (20)      230 2022-09-15 20:10:29.000000 COOMM-0.0.1.post2/coomm/__init__.py
--rw-r--r--   0 skim0119   (501) staff       (20)     1238 2022-04-08 11:57:50.000000 COOMM-0.0.1.post2/coomm/_rendering_tool.py
--rw-r--r--   0 skim0119   (501) staff       (20)    11175 2022-04-18 01:47:01.000000 COOMM-0.0.1.post2/coomm/_rod_tool.py
-drwxr-xr-x   0 skim0119   (501) staff       (20)        0 2022-09-15 20:18:05.861047 COOMM-0.0.1.post2/coomm/actuations/
--rw-r--r--   0 skim0119   (501) staff       (20)       93 2022-04-01 18:18:22.000000 COOMM-0.0.1.post2/coomm/actuations/__init__.py
--rw-r--r--   0 skim0119   (501) staff       (20)     4264 2022-09-15 20:15:35.000000 COOMM-0.0.1.post2/coomm/actuations/actuation.py
-drwxr-xr-x   0 skim0119   (501) staff       (20)        0 2022-09-15 20:18:05.866263 COOMM-0.0.1.post2/coomm/actuations/muscles/
--rw-r--r--   0 skim0119   (501) staff       (20)      216 2022-09-15 20:15:35.000000 COOMM-0.0.1.post2/coomm/actuations/muscles/__init__.py
--rw-r--r--   0 skim0119   (501) staff       (20)     1340 2022-09-15 20:15:35.000000 COOMM-0.0.1.post2/coomm/actuations/muscles/longitudinal_muscle.py
--rw-r--r--   0 skim0119   (501) staff       (20)    17102 2022-09-15 20:15:35.000000 COOMM-0.0.1.post2/coomm/actuations/muscles/muscle.py
--rw-r--r--   0 skim0119   (501) staff       (20)     1653 2022-09-15 20:15:35.000000 COOMM-0.0.1.post2/coomm/actuations/muscles/oblique_muscle.py
--rw-r--r--   0 skim0119   (501) staff       (20)     1578 2022-09-15 20:15:35.000000 COOMM-0.0.1.post2/coomm/actuations/muscles/transverse_muscle.py
-drwxr-xr-x   0 skim0119   (501) staff       (20)        0 2022-09-15 20:18:05.870295 COOMM-0.0.1.post2/coomm/algorithms/
--rw-r--r--   0 skim0119   (501) staff       (20)      165 2022-04-01 18:18:22.000000 COOMM-0.0.1.post2/coomm/algorithms/__init__.py
--rw-r--r--   0 skim0119   (501) staff       (20)      881 2022-09-15 20:15:35.000000 COOMM-0.0.1.post2/coomm/algorithms/algorithm.py
--rw-r--r--   0 skim0119   (501) staff       (20)     1983 2022-09-15 20:15:35.000000 COOMM-0.0.1.post2/coomm/algorithms/forward_backward.py
--rw-r--r--   0 skim0119   (501) staff       (20)    10193 2022-09-15 20:15:35.000000 COOMM-0.0.1.post2/coomm/algorithms/forward_backward_muscle.py
--rw-r--r--   0 skim0119   (501) staff       (20)     5448 2022-04-08 11:57:50.000000 COOMM-0.0.1.post2/coomm/callback_func.py
-drwxr-xr-x   0 skim0119   (501) staff       (20)        0 2022-09-15 20:18:05.873801 COOMM-0.0.1.post2/coomm/forces/
--rw-r--r--   0 skim0119   (501) staff       (20)       94 2022-04-01 18:18:22.000000 COOMM-0.0.1.post2/coomm/forces/__init__.py
--rw-r--r--   0 skim0119   (501) staff       (20)     3152 2022-09-15 20:15:35.000000 COOMM-0.0.1.post2/coomm/forces/drag_force.py
-drwxr-xr-x   0 skim0119   (501) staff       (20)        0 2022-09-15 20:18:05.881911 COOMM-0.0.1.post2/coomm/frames/
--rw-r--r--   0 skim0119   (501) staff       (20)      174 2022-04-01 18:18:22.000000 COOMM-0.0.1.post2/coomm/frames/__init__.py
--rw-r--r--   0 skim0119   (501) staff       (20)     2499 2022-09-15 20:15:35.000000 COOMM-0.0.1.post2/coomm/frames/frame.py
--rw-r--r--   0 skim0119   (501) staff       (20)     6071 2022-04-08 11:57:50.000000 COOMM-0.0.1.post2/coomm/frames/frame_tools.py
--rw-r--r--   0 skim0119   (501) staff       (20)    10272 2022-09-15 20:15:35.000000 COOMM-0.0.1.post2/coomm/frames/muscle_frame.py
--rw-r--r--   0 skim0119   (501) staff       (20)     3574 2022-09-15 20:15:35.000000 COOMM-0.0.1.post2/coomm/frames/rigidbody_frame.py
--rw-r--r--   0 skim0119   (501) staff       (20)    14588 2022-09-15 20:15:35.000000 COOMM-0.0.1.post2/coomm/frames/rod_frame.py
-drwxr-xr-x   0 skim0119   (501) staff       (20)        0 2022-09-15 20:18:05.887088 COOMM-0.0.1.post2/coomm/objects/
--rw-r--r--   0 skim0119   (501) staff       (20)      193 2022-04-01 18:18:22.000000 COOMM-0.0.1.post2/coomm/objects/__init__.py
--rw-r--r--   0 skim0119   (501) staff       (20)     9076 2022-09-15 20:15:35.000000 COOMM-0.0.1.post2/coomm/objects/cylinder.py
--rw-r--r--   0 skim0119   (501) staff       (20)     5569 2022-09-15 20:15:35.000000 COOMM-0.0.1.post2/coomm/objects/director_constraint.py
--rw-r--r--   0 skim0119   (501) staff       (20)     6040 2022-04-08 11:57:50.000000 COOMM-0.0.1.post2/coomm/objects/object.py
--rw-r--r--   0 skim0119   (501) staff       (20)     4280 2022-09-15 20:15:35.000000 COOMM-0.0.1.post2/coomm/objects/point.py
--rw-r--r--   0 skim0119   (501) staff       (20)      244 2022-04-08 11:57:50.000000 COOMM-0.0.1.post2/coomm/objects/target.py
-drwxr-xr-x   0 skim0119   (501) staff       (20)        0 2022-09-15 20:18:05.894094 COOMM-0.0.1.post2/coomm/povray/
--rw-r--r--   0 skim0119   (501) staff       (20)      269 2022-04-01 18:18:22.000000 COOMM-0.0.1.post2/coomm/povray/__init__.py
--rw-r--r--   0 skim0119   (501) staff       (20)     1197 2022-09-15 20:15:35.000000 COOMM-0.0.1.post2/coomm/povray/cylinder.py
--rw-r--r--   0 skim0119   (501) staff       (20)     6870 2022-04-01 18:18:22.000000 COOMM-0.0.1.post2/coomm/povray/draw_sucker.py
-drwxr-xr-x   0 skim0119   (501) staff       (20)        0 2022-09-15 20:18:05.897510 COOMM-0.0.1.post2/coomm/povray/muscles/
--rw-r--r--   0 skim0119   (501) staff       (20)      166 2022-04-01 18:18:22.000000 COOMM-0.0.1.post2/coomm/povray/muscles/__init__.py
--rw-r--r--   0 skim0119   (501) staff       (20)     5515 2022-09-15 20:15:35.000000 COOMM-0.0.1.post2/coomm/povray/muscles/muscle.py
--rw-r--r--   0 skim0119   (501) staff       (20)      490 2022-09-15 20:15:35.000000 COOMM-0.0.1.post2/coomm/povray/muscles/muscle_longitudinal.py
--rw-r--r--   0 skim0119   (501) staff       (20)      480 2022-09-15 20:15:35.000000 COOMM-0.0.1.post2/coomm/povray/muscles/muscle_oblique.py
--rw-r--r--   0 skim0119   (501) staff       (20)      477 2022-09-15 20:15:35.000000 COOMM-0.0.1.post2/coomm/povray/muscles/muscle_transverse.py
--rw-r--r--   0 skim0119   (501) staff       (20)     1007 2022-09-15 20:15:35.000000 COOMM-0.0.1.post2/coomm/povray/povray_base.py
--rw-r--r--   0 skim0119   (501) staff       (20)     5677 2022-04-01 18:18:22.000000 COOMM-0.0.1.post2/coomm/povray/povray_camera.py
--rw-r--r--   0 skim0119   (501) staff       (20)      337 2022-04-01 18:18:22.000000 COOMM-0.0.1.post2/coomm/povray/povray_frame.py
--rw-r--r--   0 skim0119   (501) staff       (20)     1023 2022-09-15 20:15:35.000000 COOMM-0.0.1.post2/coomm/povray/rod.py
--rw-r--r--   0 skim0119   (501) staff       (20)      893 2022-09-15 20:15:35.000000 COOMM-0.0.1.post2/coomm/povray/sphere.py
--rw-r--r--   0 skim0119   (501) staff       (20)       24 2022-09-15 20:07:31.000000 COOMM-0.0.1.post2/coomm/version.py
--rw-r--r--   0 skim0119   (501) staff       (20)       38 2022-09-15 20:18:05.900651 COOMM-0.0.1.post2/setup.cfg
--rw-r--r--   0 skim0119   (501) staff       (20)     3432 2022-09-15 20:17:21.000000 COOMM-0.0.1.post2/setup.py
+-rw-r--r--   0        0        0     1073 2022-03-25 04:30:36.121838 coomm-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1865 2023-06-22 17:43:51.268902 coomm-0.1.1/README.md
+-rw-r--r--   0        0        0      230 2023-06-22 15:41:06.799540 coomm-0.1.1/coomm/__init__.py
+-rw-r--r--   0        0        0     1238 2023-06-22 15:41:06.800011 coomm-0.1.1/coomm/_rendering_tool.py
+-rw-r--r--   0        0        0    11196 2023-06-22 15:35:27.042626 coomm-0.1.1/coomm/_rod_tool.py
+-rw-r--r--   0        0        0       93 2023-06-22 15:41:06.801095 coomm-0.1.1/coomm/actuations/__init__.py
+-rw-r--r--   0        0        0     4268 2023-06-22 17:43:51.269990 coomm-0.1.1/coomm/actuations/actuation.py
+-rw-r--r--   0        0        0      216 2023-06-22 15:41:06.802215 coomm-0.1.1/coomm/actuations/muscles/__init__.py
+-rw-r--r--   0        0        0     1340 2023-06-22 15:41:06.802754 coomm-0.1.1/coomm/actuations/muscles/longitudinal_muscle.py
+-rw-r--r--   0        0        0    17102 2023-06-22 15:41:06.803357 coomm-0.1.1/coomm/actuations/muscles/muscle.py
+-rw-r--r--   0        0        0     1653 2023-06-22 15:41:06.803989 coomm-0.1.1/coomm/actuations/muscles/oblique_muscle.py
+-rw-r--r--   0        0        0     1578 2023-06-22 15:41:06.804501 coomm-0.1.1/coomm/actuations/muscles/transverse_muscle.py
+-rw-r--r--   0        0        0      165 2023-06-22 15:41:06.805031 coomm-0.1.1/coomm/algorithms/__init__.py
+-rw-r--r--   0        0        0      881 2023-06-22 15:41:06.805850 coomm-0.1.1/coomm/algorithms/algorithm.py
+-rw-r--r--   0        0        0     1983 2023-06-22 15:41:06.807117 coomm-0.1.1/coomm/algorithms/forward_backward.py
+-rw-r--r--   0        0        0    10814 2023-06-22 15:35:27.043358 coomm-0.1.1/coomm/algorithms/forward_backward_muscle.py
+-rw-r--r--   0        0        0     5447 2023-06-22 17:43:51.272131 coomm-0.1.1/coomm/callback_func.py
+-rw-r--r--   0        0        0       94 2023-06-22 15:41:06.809112 coomm-0.1.1/coomm/forces/__init__.py
+-rw-r--r--   0        0        0     3156 2023-06-22 17:43:51.274186 coomm-0.1.1/coomm/forces/drag_force.py
+-rw-r--r--   0        0        0      174 2023-06-22 15:41:06.811285 coomm-0.1.1/coomm/frames/__init__.py
+-rw-r--r--   0        0        0     2499 2023-06-22 15:41:06.811891 coomm-0.1.1/coomm/frames/frame.py
+-rw-r--r--   0        0        0     6071 2023-06-22 15:41:06.812460 coomm-0.1.1/coomm/frames/frame_tools.py
+-rw-r--r--   0        0        0    10272 2023-06-22 15:41:06.813568 coomm-0.1.1/coomm/frames/muscle_frame.py
+-rw-r--r--   0        0        0     3574 2023-06-22 15:41:06.814146 coomm-0.1.1/coomm/frames/rigidbody_frame.py
+-rw-r--r--   0        0        0    14588 2023-06-22 15:41:06.814795 coomm-0.1.1/coomm/frames/rod_frame.py
+-rw-r--r--   0        0        0      193 2023-06-22 15:41:06.815417 coomm-0.1.1/coomm/objects/__init__.py
+-rw-r--r--   0        0        0    12129 2023-06-22 17:43:51.276178 coomm-0.1.1/coomm/objects/cylinder.py
+-rw-r--r--   0        0        0     5569 2023-06-22 15:41:06.816264 coomm-0.1.1/coomm/objects/director_constraint.py
+-rw-r--r--   0        0        0     6040 2023-06-22 15:41:06.816832 coomm-0.1.1/coomm/objects/object.py
+-rw-r--r--   0        0        0     4280 2023-06-22 15:41:06.817487 coomm-0.1.1/coomm/objects/point.py
+-rw-r--r--   0        0        0      244 2023-06-22 15:41:06.818463 coomm-0.1.1/coomm/objects/target.py
+-rw-r--r--   0        0        0      269 2023-06-22 15:41:06.819688 coomm-0.1.1/coomm/povray/__init__.py
+-rw-r--r--   0        0        0     1197 2023-06-22 15:41:06.820715 coomm-0.1.1/coomm/povray/cylinder.py
+-rw-r--r--   0        0        0     6870 2023-06-22 15:41:06.821741 coomm-0.1.1/coomm/povray/draw_sucker.py
+-rw-r--r--   0        0        0      166 2023-06-22 15:41:06.822580 coomm-0.1.1/coomm/povray/muscles/__init__.py
+-rw-r--r--   0        0        0     5515 2023-06-22 16:20:03.900231 coomm-0.1.1/coomm/povray/muscles/muscle.py
+-rw-r--r--   0        0        0      490 2023-06-22 15:41:06.824080 coomm-0.1.1/coomm/povray/muscles/muscle_longitudinal.py
+-rw-r--r--   0        0        0      480 2023-06-22 15:41:06.824674 coomm-0.1.1/coomm/povray/muscles/muscle_oblique.py
+-rw-r--r--   0        0        0      477 2023-06-22 15:41:06.825230 coomm-0.1.1/coomm/povray/muscles/muscle_transverse.py
+-rw-r--r--   0        0        0     1007 2023-06-22 15:41:06.825767 coomm-0.1.1/coomm/povray/povray_base.py
+-rw-r--r--   0        0        0     5677 2023-06-22 15:41:06.826509 coomm-0.1.1/coomm/povray/povray_camera.py
+-rw-r--r--   0        0        0      337 2023-06-22 15:41:06.827104 coomm-0.1.1/coomm/povray/povray_frame.py
+-rw-r--r--   0        0        0     1023 2023-06-22 15:41:06.827825 coomm-0.1.1/coomm/povray/rod.py
+-rw-r--r--   0        0        0      893 2023-06-22 15:41:06.828447 coomm-0.1.1/coomm/povray/sphere.py
+-rw-r--r--   0        0        0       24 2023-06-22 15:41:06.828953 coomm-0.1.1/coomm/version.py
+-rw-r--r--   0        0        0      884 2023-06-22 17:43:51.279152 coomm-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2768 1970-01-01 00:00:00.000000 coomm-0.1.1/PKG-INFO
```

### Comparing `COOMM-0.0.1.post2/LICENSE` & `coomm-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `COOMM-0.0.1.post2/coomm/_rendering_tool.py` & `coomm-0.1.1/coomm/_rendering_tool.py`

 * *Files identical despite different names*

### Comparing `COOMM-0.0.1.post2/coomm/_rod_tool.py` & `coomm-0.1.1/coomm/_rod_tool.py`

 * *Files 0% similar despite different names*

```diff
@@ -293,18 +293,19 @@
             rest_cosserat_rod.radius,
             rest_cosserat_rod.shear_matrix,
             rest_cosserat_rod.bend_matrix
         )
 
 @njit(cache=True)
 def next_position(director, delta, positions):
+    positions[:, 1] = positions[:, 0]
     for i in range(3):
         for j in range(3):
-            positions[i, 1] = (
-                positions[i, 0] + director[j, i] * delta[j]
+            positions[i, 1] += (
+                director[j, i] * delta[j]
             )
 
 @njit(cache=True)
 def next_director(rotation, directors):
     # FIXME The following should be the right implementation once the _get_rotation_matrix is fixed
     # Rotation = _get_rotation_matrix(-1, rotation.reshape((3, 1)))[:, :, 0]
```

### Comparing `COOMM-0.0.1.post2/coomm/actuations/actuation.py` & `coomm-0.1.1/coomm/actuations/actuation.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,21 +83,21 @@
         callback_params_list : Dictionary[list]
         """
         self.current_step = 0
         self.actuations = actuations
         self.every = step_skip
         self.callback_params_list = callback_params_list
 
-    def apply_torques(self, system, time: np.float = 0.0):
+    def apply_torques(self, system, time: np.float64 = 0.0):
         """apply_torques.
 
         Parameters
         ----------
         system :
-        time : np.float
+        time : np.float64
         """
         for actuation in self.actuations:
             actuation(system)
             inplace_addition(
                 system.external_forces, actuation.external_force
             )
             inplace_addition(
```

### Comparing `COOMM-0.0.1.post2/coomm/actuations/muscles/longitudinal_muscle.py` & `coomm-0.1.1/coomm/actuations/muscles/longitudinal_muscle.py`

 * *Files identical despite different names*

### Comparing `COOMM-0.0.1.post2/coomm/actuations/muscles/muscle.py` & `coomm-0.1.1/coomm/actuations/muscles/muscle.py`

 * *Files identical despite different names*

### Comparing `COOMM-0.0.1.post2/coomm/actuations/muscles/oblique_muscle.py` & `coomm-0.1.1/coomm/actuations/muscles/oblique_muscle.py`

 * *Files identical despite different names*

### Comparing `COOMM-0.0.1.post2/coomm/actuations/muscles/transverse_muscle.py` & `coomm-0.1.1/coomm/actuations/muscles/transverse_muscle.py`

 * *Files identical despite different names*

### Comparing `COOMM-0.0.1.post2/coomm/algorithms/algorithm.py` & `coomm-0.1.1/coomm/algorithms/algorithm.py`

 * *Files identical despite different names*

### Comparing `COOMM-0.0.1.post2/coomm/algorithms/forward_backward.py` & `coomm-0.1.1/coomm/algorithms/forward_backward.py`

 * *Files identical despite different names*

### Comparing `COOMM-0.0.1.post2/coomm/algorithms/forward_backward_muscle.py` & `coomm-0.1.1/coomm/algorithms/forward_backward_muscle.py`

 * *Files 8% similar despite different names*

```diff
@@ -186,28 +186,28 @@
         internal_force_lab_frame[:, -1] = internal_force_lab_frame_at_tip[:, -1]
         
         force_derivative = average2D(internal_force_lab_frame_derivative)
 
         # n_s = f
         for k in range(blocksize-1):
             internal_force_lab_frame[:, -1-k-1] = internal_force_lab_frame[:, -1-k] - (
-                force_derivative[:, -1-k] * rest_lengths[-1-k] * dilatation[-1-k]
+                force_derivative[:, -1-k] * 0.5 * (rest_lengths[-1-k] * dilatation[-1-k] + rest_lengths[-1-k-1] * dilatation[-1-k-1])
             )
         internal_force[:, :] = _lab_to_material(director, internal_force_lab_frame)
 
         internal_couple_lab_frame[:, -1] = internal_couple_lab_frame_at_tip[:, -1]
 
         # m_s = -r_s x n + c
         internal_couple_lab_frame_derivative[:, :] -= _batch_cross(
             _material_to_lab(director, shear), internal_force_lab_frame
         )
         couple_derivative = average2D(internal_couple_lab_frame_derivative)
         for k in range(blocksize-1):
             internal_couple_lab_frame[:, -1-k-1] = internal_couple_lab_frame[:, -1-k] - (
-                couple_derivative[:, -1-k] * rest_lengths[-1-k] * dilatation[-1-k]
+                couple_derivative[:, -1-k] * 0.5 * (rest_lengths[-1-k] * dilatation[-1-k] + rest_lengths[-1-k-1] * dilatation[-1-k-1])
             )
         internal_couple[:, :] = average2D(
             _lab_to_material(director, internal_couple_lab_frame)
         )
 
     def find_target_activations(self):
         """find_target_activations.
@@ -245,19 +245,29 @@
         )
         temp_kappa = _batch_matvec(
             inverse(bend_matrix/voronoi_dilatation),
             muscle_internal_couple
         )
         temp_force_innerproduct = np.zeros(blocksize)
         temp_couple_innerproduct = np.zeros(blocksize+1)
-        for k in range(blocksize-1):
+        # for k in range(blocksize-1):
+        #     for i in range(3):
+        #         temp_force_innerproduct[k] += internal_force[i, k] * temp_shear[i, k]
+        #         temp_couple_innerproduct[k+1] += internal_couple[i, k+1] * temp_kappa[i, k+1]
+        # temp_force_innerproduct[-1] += internal_force[i, -1] * temp_shear[i, -1]
+
+        for k in range(blocksize):
             for i in range(3):
                 temp_force_innerproduct[k] += internal_force[i, k] * temp_shear[i, k]
-                temp_couple_innerproduct[k+1] += internal_couple[i, k+1] * temp_kappa[i, k+1]
-        temp_force_innerproduct[-1] += internal_force[i, -1] * temp_shear[i, -1]
+        for k in range(blocksize-1):
+            for i in range(3):
+                temp_couple_innerproduct[k+1] += internal_couple[i, k] * temp_kappa[i, k]
+        temp_couple_innerproduct[0] = 2*temp_couple_innerproduct[1]-temp_couple_innerproduct[2]
+        temp_couple_innerproduct[-1] = 2*temp_couple_innerproduct[-2]-temp_couple_innerproduct[-3]
+
         for k in range(blocksize):
             target_activation[k] = -temp_force_innerproduct[k] - 0.5*(
                 temp_couple_innerproduct[k] + temp_couple_innerproduct[k+1]
             )
         return target_activation
 
     def update_activations(self, target_activations):
```

### Comparing `COOMM-0.0.1.post2/coomm/callback_func.py` & `coomm-0.1.1/coomm/callback_func.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 __doc__ = """
 Common callback function used in COMM.
 """
 
 from collections import defaultdict
 
-from elastica.wrappers import callbacks
+from elastica.modules import callbacks
 
 from elastica.callback_functions import CallBackBaseClass
 
 class BasicCallBackBaseClass(CallBackBaseClass):
     def __init__(self, step_skip: int, callback_params: dict):
         CallBackBaseClass.__init__(self)
         self.every = step_skip
```

### Comparing `COOMM-0.0.1.post2/coomm/forces/drag_force.py` & `coomm-0.1.1/coomm/forces/drag_force.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,21 +44,21 @@
         self.drag_force_material_frame = np.zeros((3, system.n_elems))
         self.drag_force = np.zeros((3, system.n_elems+1))
 
         self.step = 0
         self.every = step_skip
         self.callback_params = callback_params
     
-    def apply_torques(self, system, time: np.float = 0.0):
+    def apply_torques(self, system, time: np.float64 = 0.0):
         """apply_torques.
 
         Parameters
         ----------
         system :
-        time : np.float
+        time : np.float64
         """
         Pa = 2 * system.radius * system.lengths
         Sa = Pa * np.pi
         self.calculate_drag_force(
             self.scale_per*Pa, self.scale_tan*Sa,
             system.director_collection, system.velocity_collection,
             self.velocity_material_frame,
```

### Comparing `COOMM-0.0.1.post2/coomm/frames/frame.py` & `coomm-0.1.1/coomm/frames/frame.py`

 * *Files identical despite different names*

### Comparing `COOMM-0.0.1.post2/coomm/frames/frame_tools.py` & `coomm-0.1.1/coomm/frames/frame_tools.py`

 * *Files identical despite different names*

### Comparing `COOMM-0.0.1.post2/coomm/frames/muscle_frame.py` & `coomm-0.1.1/coomm/frames/muscle_frame.py`

 * *Files identical despite different names*

### Comparing `COOMM-0.0.1.post2/coomm/frames/rigidbody_frame.py` & `coomm-0.1.1/coomm/frames/rigidbody_frame.py`

 * *Files identical despite different names*

### Comparing `COOMM-0.0.1.post2/coomm/frames/rod_frame.py` & `coomm-0.1.1/coomm/frames/rod_frame.py`

 * *Files identical despite different names*

### Comparing `COOMM-0.0.1.post2/coomm/objects/cylinder.py` & `coomm-0.1.1/coomm/objects/cylinder.py`

 * *Files 24% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         cylinder :
             cylinder
         n_elements :
             n_elements
         cost_weight :
             cost_weight
         """
-        return Cylinder(
+        return cls(
             cylinder.position_collection[:, 0].copy(),
             cylinder.director_collection[:, :, 0].copy(),
             n_elements, cost_weight
         )
 
     def calculate_continuous_cost_gradient_wrt_position(self, **kwargs):
         """calculate_continuous_cost_gradient_wrt_position.
@@ -182,51 +182,109 @@
         adjust_distance_ratio = (position_dist-(radius+self.radius))/position_dist
         
         adjust_distance_ratio[adjust_distance_ratio<0] = 0
         self.cost_gradient.continuous.wrt_position[:, :] += (
             self.target_cost_weight['position'] * position_diff * adjust_distance_ratio
         )
     
+    """ The first method """
+    # def calculate_continuous_cost_gradient_wrt_director(self, **kwargs):
+    #     """calculate_continuous_cost_gradient_wrt_director.
+    #     """
+    #     position = 0.5*(kwargs['position'][:, :-1]+kwargs['position'][:, 1:])
+    #     director = kwargs['director'][:, :, :]
+    #     n_elems = director.shape[2]
+    #     vector = np.zeros((3, n_elems))
+    #     coefficient = np.zeros(n_elems)
+    #     # for n in range(n_elems):
+    #     #     skew_symmetric_matrix = director[:, :, n] @ self.director.T - self.director @ director[:, :, n].T
+    #     #     vector[0, n] = skew_symmetric_matrix[1, 2]
+    #     #     vector[1, n] = -skew_symmetric_matrix[0, 2]
+    #     #     vector[2, n] = skew_symmetric_matrix[0, 1]
+    #     #     self.cost_gradient.continuous.wrt_director[:, n] = (
+    #     #         self.target_cost_weight['director'][n] * director[:, :, n].T @ vector[:, n]
+    #     #     )
+        
+    #     for n in range(n_elems):
+    #         vector[1, n] = - np.dot(director[2, :, n], self.director[2, :])
+    #         vector[2, n] = np.dot(director[1, :, n], self.director[2, :])
+    #         coefficient[n] = np.dot(director[0, :, n], self.director[2, :])
+    #         self.cost_gradient.continuous.wrt_director[:, n] = (
+    #             self.target_cost_weight['director'][n] * coefficient[n] * director[:, :, n].T @ vector[:, n]
+    #         )
+
+    #     vector = np.zeros((3, n_elems))
+    #     coefficient = np.zeros(n_elems)
+    #     for n in range(n_elems):
+    #         position_diff = self.position - position[:, n]
+    #         position_diff = position_diff / np.linalg.norm(position_diff)
+    #         vector[1, n] = - np.dot(director[2, :, n], position_diff)
+    #         vector[2, n] = np.dot(director[1, :, n], position_diff)
+    #         coefficient[n] = min(np.dot(self.director[0, :], position_diff), 0)
+    #         self.cost_gradient.continuous.wrt_director[:, n] += (
+    #             self.target_cost_weight['director'][n] * coefficient[n] * director[:, :, n].T @ vector[:, n]
+    #         )
     def calculate_continuous_cost_gradient_wrt_director(self, **kwargs):
         """calculate_continuous_cost_gradient_wrt_director.
         """
         position = 0.5*(kwargs['position'][:, :-1]+kwargs['position'][:, 1:])
         director = kwargs['director'][:, :, :]
         n_elems = director.shape[2]
-        vector = np.zeros((3, n_elems))
-        coefficient = np.zeros(n_elems)
+
+        # vector = np.zeros((3, n_elems))
+        # coefficient = np.zeros(n_elems)
         # for n in range(n_elems):
         #     skew_symmetric_matrix = director[:, :, n] @ self.director.T - self.director @ director[:, :, n].T
         #     vector[0, n] = skew_symmetric_matrix[1, 2]
         #     vector[1, n] = -skew_symmetric_matrix[0, 2]
         #     vector[2, n] = skew_symmetric_matrix[0, 1]
         #     self.cost_gradient.continuous.wrt_director[:, n] = (
         #         self.target_cost_weight['director'][n] * director[:, :, n].T @ vector[:, n]
         #     )
         
-        for n in range(n_elems):
-            vector[1, n] = - np.dot(director[2, :, n], self.director[2, :])
-            vector[2, n] = np.dot(director[1, :, n], self.director[2, :])
-            coefficient[n] = np.dot(director[0, :, n], self.director[2, :])
-            self.cost_gradient.continuous.wrt_director[:, n] = (
-                self.target_cost_weight['director'][n] * coefficient[n] * director[:, :, n].T @ vector[:, n]
-            )
+        # for n in range(n_elems):
+        #     vector[1, n] = - np.dot(director[2, :, n], self.director[2, :])
+        #     vector[2, n] = np.dot(director[1, :, n], self.director[2, :])
+        #     coefficient[n] = np.dot(director[0, :, n], self.director[2, :])
+        #     self.cost_gradient.continuous.wrt_director[:, n] = (
+        #         self.target_cost_weight['director'][n] * coefficient[n] * director[:, :, n].T @ vector[:, n]
+        #     )
+
 
+
+        """ The second method """
         vector = np.zeros((3, n_elems))
         coefficient = np.zeros(n_elems)
         for n in range(n_elems):
             position_diff = self.position - position[:, n]
             position_diff = position_diff / np.linalg.norm(position_diff)
-            vector[1, n] = - np.dot(director[2, :, n], position_diff)
-            vector[2, n] = np.dot(director[1, :, n], position_diff)
-            coefficient[n] = min(np.dot(self.director[0, :], position_diff), 0)
-            self.cost_gradient.continuous.wrt_director[:, n] += (
+            vector[1, n] = - np.dot(director[2, :, n], -position_diff)
+            vector[2, n] = np.dot(director[1, :, n], -position_diff)
+            # coefficient[n] = 1-np.dot(director[0, :, n], position_diff)
+            coefficient[n] = 1
+            self.cost_gradient.continuous.wrt_director[:, n] = (
                 self.target_cost_weight['director'][n] * coefficient[n] * director[:, :, n].T @ vector[:, n]
             )
 
+        """ The third method """
+        # vector = np.zeros((3, n_elems))
+        # coefficient = np.zeros(n_elems)
+        # for n in range(n_elems):
+        #     position_diff = self.position - position[:, n]
+        #     position_diff = position_diff - np.dot(position_diff, self.director[2, :]) * self.director[2, :]
+        #     position_diff = position_diff / np.linalg.norm(position_diff)
+        #     vector[1, n] = - np.dot(director[2, :, n], -position_diff)
+        #     vector[2, n] = np.dot(director[1, :, n], -position_diff)
+        #     # coefficient[n] = 1 - np.dot(director[0, :, n], position_diff)
+        #     coefficient[n] = 1 
+        #     # print(position_diff)
+        #     self.cost_gradient.continuous.wrt_director[:, n] = (
+        #         self.target_cost_weight['director'][n] * coefficient[n] * director[:, :, n].T @ vector[:, n]
+        #     )
+
     def calculate_discrete_cost_gradient_wrt_position(self, **kwargs):
         """calculate_discrete_cost_gradient_wrt_position.
         """
         # position = 0.5*(kwargs['position'][:, -1]+kwargs['position'][:, -2])
         # self.cost_gradient.discrete.wrt_position[:, -1] = (
         #     self.target_cost_weight['position'] * (position-self.position)
         # )
```

### Comparing `COOMM-0.0.1.post2/coomm/objects/director_constraint.py` & `coomm-0.1.1/coomm/objects/director_constraint.py`

 * *Files identical despite different names*

### Comparing `COOMM-0.0.1.post2/coomm/objects/object.py` & `coomm-0.1.1/coomm/objects/object.py`

 * *Files identical despite different names*

### Comparing `COOMM-0.0.1.post2/coomm/objects/point.py` & `coomm-0.1.1/coomm/objects/point.py`

 * *Files identical despite different names*

### Comparing `COOMM-0.0.1.post2/coomm/povray/cylinder.py` & `coomm-0.1.1/coomm/povray/cylinder.py`

 * *Files identical despite different names*

### Comparing `COOMM-0.0.1.post2/coomm/povray/draw_sucker.py` & `coomm-0.1.1/coomm/povray/draw_sucker.py`

 * *Files identical despite different names*

### Comparing `COOMM-0.0.1.post2/coomm/povray/muscles/muscle.py` & `coomm-0.1.1/coomm/povray/muscles/muscle.py`

 * *Files identical despite different names*

### Comparing `COOMM-0.0.1.post2/coomm/povray/povray_base.py` & `coomm-0.1.1/coomm/povray/povray_base.py`

 * *Files identical despite different names*

### Comparing `COOMM-0.0.1.post2/coomm/povray/povray_camera.py` & `coomm-0.1.1/coomm/povray/povray_camera.py`

 * *Files identical despite different names*

### Comparing `COOMM-0.0.1.post2/coomm/povray/rod.py` & `coomm-0.1.1/coomm/povray/rod.py`

 * *Files identical despite different names*

### Comparing `COOMM-0.0.1.post2/coomm/povray/sphere.py` & `coomm-0.1.1/coomm/povray/sphere.py`

 * *Files identical despite different names*

