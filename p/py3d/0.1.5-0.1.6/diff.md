# Comparing `tmp/py3d-0.1.5.tar.gz` & `tmp/py3d-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3d-0.1.5.tar", last modified: Sun Jun 18 15:25:21 2023, max compression
+gzip compressed data, was "py3d-0.1.6.tar", last modified: Thu Jun 22 04:01:25 2023, max compression
```

## Comparing `py3d-0.1.5.tar` & `py3d-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 15:25:21.450456 py3d-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (122)     1968 2023-06-18 15:25:21.450456 py3d-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1578 2023-06-18 15:24:55.000000 py3d-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 15:25:21.450456 py3d-0.1.5/py3d/
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-06-18 15:23:59.000000 py3d-0.1.5/py3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    28904 2023-06-18 15:23:59.000000 py3d-0.1.5/py3d/core.py
--rw-r--r--   0 runner    (1001) docker     (122)    22694 2023-06-18 15:23:59.000000 py3d-0.1.5/py3d/viewer.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 15:25:21.450456 py3d-0.1.5/py3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1968 2023-06-18 15:25:21.000000 py3d-0.1.5/py3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      204 2023-06-18 15:25:21.000000 py3d-0.1.5/py3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-18 15:25:21.000000 py3d-0.1.5/py3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-06-18 15:25:21.000000 py3d-0.1.5/py3d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-18 15:25:21.000000 py3d-0.1.5/py3d.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-18 15:25:21.450456 py3d-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-06-18 15:23:59.000000 py3d-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 04:01:25.459198 py3d-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (122)     1968 2023-06-22 04:01:25.459198 py3d-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1578 2023-06-22 04:01:05.000000 py3d-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 04:01:25.459198 py3d-0.1.6/py3d/
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-06-22 04:00:23.000000 py3d-0.1.6/py3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29619 2023-06-22 04:00:23.000000 py3d-0.1.6/py3d/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22693 2023-06-22 04:00:23.000000 py3d-0.1.6/py3d/viewer.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 04:01:25.459198 py3d-0.1.6/py3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1968 2023-06-22 04:01:25.000000 py3d-0.1.6/py3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-06-22 04:01:25.000000 py3d-0.1.6/py3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-22 04:01:25.000000 py3d-0.1.6/py3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-06-22 04:01:25.000000 py3d-0.1.6/py3d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-22 04:01:25.000000 py3d-0.1.6/py3d.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-22 04:01:25.459198 py3d-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-06-22 04:00:23.000000 py3d-0.1.6/setup.py
```

### Comparing `py3d-0.1.5/PKG-INFO` & `py3d-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3d
-Version: 0.1.5
+Version: 0.1.6
 Summary: py3d is a 3d computational geometry library that deals with 3d data in batches. And it embedded an interactive viewer that can work in jupyter notebook.
 Home-page: https://tumiz.github.io/scenario/
 Author: Tumiz
 Author-email: hh11698@163.com
 License: GPL-3.0 License
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `py3d-0.1.5/README.md` & `py3d-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `py3d-0.1.5/py3d/core.py` & `py3d-0.1.6/py3d/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -249,25 +249,25 @@
     def M(self) -> Vector | Vector2 | Vector3 | Vector4:
         # mean vector
         return super().mean(axis=self.ndim-2)
 
     @property
     def L(self) -> Vector:
         # length
-        return numpy.linalg.norm(self, axis=self.ndim - 1)
+        return numpy.linalg.norm(self, axis=self.ndim - 1).view(Vector)
 
     def min(self) -> Vector:
         return super().min(axis=self.ndim-2)
 
     def max(self) -> Vector:
         return super().max(axis=self.ndim-2)
 
     def diff(self, n=1) -> Vector:
         return numpy.diff(self, n, axis=self.ndim-2)
-    
+
     def lerp(self, x, xp) -> Vector:
         '''
         linear interpolation
         x: 1-D array, the data to be interpolated.
         xp: 1-D array, the data to interpolate into. For example, time series.
         '''
         x = numpy.array(x)
@@ -403,14 +403,30 @@
         return p0 + (self - p0).vector_projection(p1 - p0)
 
     def projection_on_plane(self, plane) -> numpy.ndarray:
         return self + (plane.position[:, numpy.newaxis] - self).vector_projection(
             plane.normal[:, numpy.newaxis]
         )
 
+    def closest_point_to_points(self, points: Vector3 | numpy.ndarray | list) -> Vector3:
+        '''
+        return closest point indexes of one point cloud to another point cloud, and also return indexes of the pair points in the another point cloud
+        both self and points should be flattened
+        '''
+        pts = Vector3(points)
+        assert self.ndim < 3, "self should be flattened"
+        assert pts.ndim < 3, "parameter `points` should be flattened"
+        d: Vector = (self[..., numpy.newaxis, :] - pts).L
+        d = d.reshape(*d.shape[:-2], -1)
+        idx = d.argmin(d.ndim-1)
+        spts = sum(pts.n)
+        idx0 = idx//spts
+        idx1 = idx % spts
+        return idx0, idx1
+
     def as_scaling(self) -> Transform:
         ret = Transform
         ret[..., 0, 0] = self[..., 0]
         ret[..., 1, 1] = self[..., 1]
         ret[..., 2, 2] = self[..., 2]
         return ret.view(Transform)
```

### Comparing `py3d-0.1.5/py3d/viewer.html` & `py3d-0.1.6/py3d/viewer.html`

 * *Files 0% similar despite different names*

```diff
@@ -305,15 +305,15 @@
             }
             this.canvas.onmousemove = (ev) => {
                 let dx = ev.clientX - this.canvas_x
                 let dy = ev.clientY - this.canvas_y
                 let d = Math.hypot(dx, dy)
                 if (d) {
                     if (ev.ctrlKey | ev.buttons == 4) {
-                        this.camera.rotation = mat.mm(mat.angle_axis(d / 100, -dy / d, dx / d, 0), this.camera.rotation)
+                        this.camera.rotation = mat.mm(mat.angle_axis(d / 100, dy / d, dx / d, 0), this.camera.rotation)
                         this.render()
                     } else if (ev.shiftKey | ev.buttons == 1) {
                         const ratio = this.camera.height / 200
                         this.camera.center = mat.add(this.camera.center, mat.vm([-dx * ratio, dy * ratio, 0], this.camera.rotation))
                         this.toolbar.tooltip.innerHTML = this.camera.position()
                         this.render()
                     }
```

### Comparing `py3d-0.1.5/py3d.egg-info/PKG-INFO` & `py3d-0.1.6/py3d.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3d
-Version: 0.1.5
+Version: 0.1.6
 Summary: py3d is a 3d computational geometry library that deals with 3d data in batches. And it embedded an interactive viewer that can work in jupyter notebook.
 Home-page: https://tumiz.github.io/scenario/
 Author: Tumiz
 Author-email: hh11698@163.com
 License: GPL-3.0 License
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `py3d-0.1.5/setup.py` & `py3d-0.1.6/setup.py`

 * *Files identical despite different names*

