# Comparing `tmp/ztffields-0.4.0.tar.gz` & `tmp/ztffields-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ztffields-0.4.0.tar", last modified: Wed Apr 26 14:03:14 2023, max compression
+gzip compressed data, was "ztffields-0.4.1.tar", last modified: Thu Jun 22 18:39:19 2023, max compression
```

## Comparing `ztffields-0.4.0.tar` & `ztffields-0.4.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-04-26 14:03:14.766876 ztffields-0.4.0/
--rw-r--r--   0 rigault   (2358) staff       (20)    11357 2022-12-09 18:53:25.000000 ztffields-0.4.0/LICENSE
--rw-r--r--   0 rigault   (2358) staff       (20)      731 2023-04-26 14:03:14.766953 ztffields-0.4.0/PKG-INFO
--rw-r--r--   0 rigault   (2358) staff       (20)      432 2022-12-13 14:52:32.000000 ztffields-0.4.0/README.md
--rw-r--r--   0 rigault   (2358) staff       (20)     1132 2023-04-26 14:03:14.767279 ztffields-0.4.0/setup.cfg
--rw-r--r--   0 rigault   (2358) staff       (20)       37 2022-12-11 14:43:45.000000 ztffields-0.4.0/setup.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-04-26 14:03:14.765723 ztffields-0.4.0/ztffields/
--rw-r--r--   0 rigault   (2358) staff       (20)       95 2023-04-26 14:02:47.000000 ztffields-0.4.0/ztffields/__init__.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-04-26 14:03:14.766698 ztffields-0.4.0/ztffields/data/
--rwxr-xr-x   0 rigault   (2358) staff       (20)     1419 2022-12-11 14:44:47.000000 ztffields-0.4.0/ztffields/data/ztf_ccd_layout.tbl
--rwxr-xr-x   0 rigault   (2358) staff       (20)     6230 2022-12-11 14:44:47.000000 ztffields-0.4.0/ztffields/data/ztf_ccd_quad_layout.tbl
--rwxr-xr-x   0 rigault   (2358) staff       (20)   123430 2022-12-11 14:44:47.000000 ztffields-0.4.0/ztffields/data/ztf_fields.txt
--rw-r--r--   0 rigault   (2358) staff       (20)    19743 2023-04-25 14:27:27.000000 ztffields-0.4.0/ztffields/fields.py
--rw-r--r--   0 rigault   (2358) staff       (20)      175 2022-12-11 14:47:26.000000 ztffields-0.4.0/ztffields/io.py
--rw-r--r--   0 rigault   (2358) staff       (20)    28795 2023-04-26 14:00:48.000000 ztffields-0.4.0/ztffields/plotting.py
--rw-r--r--   0 rigault   (2358) staff       (20)    12067 2023-04-19 13:38:56.000000 ztffields-0.4.0/ztffields/projection.py
--rw-r--r--   0 rigault   (2358) staff       (20)     2268 2023-02-12 07:53:02.000000 ztffields-0.4.0/ztffields/utils.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-04-26 14:03:14.766369 ztffields-0.4.0/ztffields.egg-info/
--rw-r--r--   0 rigault   (2358) staff       (20)      731 2023-04-26 14:03:14.000000 ztffields-0.4.0/ztffields.egg-info/PKG-INFO
--rw-r--r--   0 rigault   (2358) staff       (20)      458 2023-04-26 14:03:14.000000 ztffields-0.4.0/ztffields.egg-info/SOURCES.txt
--rw-r--r--   0 rigault   (2358) staff       (20)        1 2023-04-26 14:03:14.000000 ztffields-0.4.0/ztffields.egg-info/dependency_links.txt
--rw-r--r--   0 rigault   (2358) staff       (20)        1 2022-12-11 14:44:59.000000 ztffields-0.4.0/ztffields.egg-info/not-zip-safe
--rw-r--r--   0 rigault   (2358) staff       (20)      132 2023-04-26 14:03:14.000000 ztffields-0.4.0/ztffields.egg-info/requires.txt
--rw-r--r--   0 rigault   (2358) staff       (20)       10 2023-04-26 14:03:14.000000 ztffields-0.4.0/ztffields.egg-info/top_level.txt
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-22 18:39:19.475865 ztffields-0.4.1/
+-rw-r--r--   0 rigault   (2358) staff       (20)    11357 2022-12-09 18:53:25.000000 ztffields-0.4.1/LICENSE
+-rw-r--r--   0 rigault   (2358) staff       (20)      731 2023-06-22 18:39:19.475931 ztffields-0.4.1/PKG-INFO
+-rw-r--r--   0 rigault   (2358) staff       (20)      432 2022-12-13 14:52:32.000000 ztffields-0.4.1/README.md
+-rw-r--r--   0 rigault   (2358) staff       (20)     1132 2023-06-22 18:39:19.476251 ztffields-0.4.1/setup.cfg
+-rw-r--r--   0 rigault   (2358) staff       (20)       37 2022-12-11 14:43:45.000000 ztffields-0.4.1/setup.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-22 18:39:19.473870 ztffields-0.4.1/ztffields/
+-rw-r--r--   0 rigault   (2358) staff       (20)       95 2023-06-22 18:38:44.000000 ztffields-0.4.1/ztffields/__init__.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-22 18:39:19.475317 ztffields-0.4.1/ztffields/data/
+-rwxr-xr-x   0 rigault   (2358) staff       (20)     1419 2022-12-11 14:44:47.000000 ztffields-0.4.1/ztffields/data/ztf_ccd_layout.tbl
+-rwxr-xr-x   0 rigault   (2358) staff       (20)     6230 2022-12-11 14:44:47.000000 ztffields-0.4.1/ztffields/data/ztf_ccd_quad_layout.tbl
+-rwxr-xr-x   0 rigault   (2358) staff       (20)   123430 2022-12-11 14:44:47.000000 ztffields-0.4.1/ztffields/data/ztf_fields.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)    19759 2023-06-22 18:38:27.000000 ztffields-0.4.1/ztffields/fields.py
+-rw-r--r--   0 rigault   (2358) staff       (20)      175 2022-12-11 14:47:26.000000 ztffields-0.4.1/ztffields/io.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    28986 2023-06-22 13:47:08.000000 ztffields-0.4.1/ztffields/plotting.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    13379 2023-06-22 14:42:39.000000 ztffields-0.4.1/ztffields/projection.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     2268 2023-02-12 07:53:02.000000 ztffields-0.4.1/ztffields/utils.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-22 18:39:19.474713 ztffields-0.4.1/ztffields.egg-info/
+-rw-r--r--   0 rigault   (2358) staff       (20)      731 2023-06-22 18:39:19.000000 ztffields-0.4.1/ztffields.egg-info/PKG-INFO
+-rw-r--r--   0 rigault   (2358) staff       (20)      458 2023-06-22 18:39:19.000000 ztffields-0.4.1/ztffields.egg-info/SOURCES.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)        1 2023-06-22 18:39:19.000000 ztffields-0.4.1/ztffields.egg-info/dependency_links.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)        1 2022-12-11 14:44:59.000000 ztffields-0.4.1/ztffields.egg-info/not-zip-safe
+-rw-r--r--   0 rigault   (2358) staff       (20)      132 2023-06-22 18:39:19.000000 ztffields-0.4.1/ztffields.egg-info/requires.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)       10 2023-06-22 18:39:19.000000 ztffields-0.4.1/ztffields.egg-info/top_level.txt
```

### Comparing `ztffields-0.4.0/LICENSE` & `ztffields-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ztffields-0.4.0/PKG-INFO` & `ztffields-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ztffields
-Version: 0.4.0
+Version: 0.4.1
 Summary: Access and Interact with ZTF Fields
 Home-page: https://github.com/MickaelRigault/ztffields
 Author: Mickael Rigault
 Author-email: m.rigault@ipnl.in2p3.fr
 License: BSD 3-Clause "New" or "Revised" License
 Keywords: astronomy,astrophysics
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `ztffields-0.4.0/setup.cfg` & `ztffields-0.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `ztffields-0.4.0/ztffields/data/ztf_ccd_layout.tbl` & `ztffields-0.4.1/ztffields/data/ztf_ccd_layout.tbl`

 * *Files identical despite different names*

### Comparing `ztffields-0.4.0/ztffields/data/ztf_ccd_quad_layout.tbl` & `ztffields-0.4.1/ztffields/data/ztf_ccd_quad_layout.tbl`

 * *Files identical despite different names*

### Comparing `ztffields-0.4.0/ztffields/data/ztf_fields.txt` & `ztffields-0.4.1/ztffields/data/ztf_fields.txt`

 * *Files identical despite different names*

### Comparing `ztffields-0.4.0/ztffields/fields.py` & `ztffields-0.4.1/ztffields/fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -518,23 +518,23 @@
         nsmax = +np.atleast_1d(upper_left_corner["NS"])
         ewmax = -np.atleast_1d(lower_right_corner["EW"])
         nsmin = +np.atleast_1d(lower_right_corner["NS"])
 
         ra1  = (np.linspace(ewmax, ewmin, steps)/np.cos(nsmax*_DEG2RA)).T
         dec1 = (np.ones((steps,1))*nsmax).T
         #
-        dec2  = np.linspace(nsmax,nsmin, steps).T
+        dec2  = np.linspace(nsmax,nsmin, steps).T        
         ra2   = ewmin[:,None]/np.cos(dec2*_DEG2RA)
         #
         ra3 = (np.linspace(ewmin,ewmax, steps)/np.cos(nsmin*_DEG2RA)).T
         dec3 = (np.ones((steps,1))*nsmin).T
         #
         dec4  = np.linspace(nsmin,nsmax, steps).T
         ra4 = ewmax[:,None]/np.cos(dec4*_DEG2RA)
-
+        
         ra_bd = np.concatenate((ra1, ra2, ra3, ra4  ), axis=1)  
         dec_bd = np.concatenate((dec1, dec2, dec3,dec4 ), axis=1)
 
         ra_,dec_ = rot_xz_sph(np.moveaxis(ra_bd,0,1), np.moveaxis(dec_bd,0,1), np.moveaxis(np.atleast_3d(dec),0,1))
         ra_ += np.moveaxis(np.atleast_3d(ra),0,1)
 
         if inrad:
```

### Comparing `ztffields-0.4.0/ztffields/plotting.py` & `ztffields-0.4.1/ztffields/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,15 +193,15 @@
     
     """
     return FieldFigure.skyplot_fields(fieldid, figsize=figsize, level=level,
                                           system=system, projection=projection, **kwargs)
 
 class FieldFigure( object ):
 
-    def __init__(self, figsize=(7,4), level="focalplane", system="icrs", origin=180, **kwargs):
+    def __init__(self, geodf, figsize=(7,4), system="icrs", origin=180, **kwargs):
         """ 
         
         Parameters
         ----------
 
         figsize : (float, float)
             Width, height in inches.
@@ -213,22 +213,29 @@
             - quadrant: 1 polygon per quadrant (64 per per footprint then)
             ccd and quadrant level will account for gaps between the CCDs.
 
         Returns
         -------
         None
         """
-        self._geodf = Fields.get_field_geometry(level=level, **kwargs)
+        self._geodf = geodf
         self.set_system(system, origin=origin)
         
         import matplotlib.pyplot as plt
         self._figure = plt.figure(figsize=(7,4))
         self._plotting = {}
 
 
+    @classmethod
+    def from_level(cls, level, figsize=(7,4), system="icrs", origin=180, **kwargs):
+        """ """
+        geodf = Fields.get_field_geometry(level=level, **kwargs)
+        return cls(geodf=geodf, figsize=figsize, system=system, origin=origin)
+
+
     def set_system(self, system="icrs", origin=180):
         """ set the plotting coordinate system.
 
         Parameters
         ----------
         system: str
             coordinates system: 
@@ -266,15 +273,14 @@
                 raise NotImplementedError(f"'{system}' has not been implemented")
 
         # identify and correct edge effects
         flag_egde = np.any(np.diff(xy, axis=1)>300, axis=1)[:,0]
         xy[flag_egde] = ((xy[flag_egde] + origin)%360 - origin)
 
         if not is_cartopy:
-            
             xy -= [origin,0] # set the origin
             xy *= np.pi/180 # in radian
             
         self._geodf["xy"] = list(xy)
         self._system = system
         self._origin = origin
         
@@ -352,15 +358,15 @@
         **kwargs goes to plot_sky | e.g. cmap, vmin, vmax ...
 
         Returns
         -------
         figure
         """
         # Create figure and the plotting system        
-        figfield = cls(figsize=figsize, level=level, system=system)
+        figfield = cls.from_level(level=level,figsize=figsize,system=system)
         
         # Create the axes
         ax = figfield.add_axes(projection=projection)
         
         # Draw the fields as matplolib's polygon
         _ = figfield.plot_sky(ax=ax, fieldid=fieldid,
                               facealpha=facealpha, edgecolor=edgecolor,
@@ -513,15 +519,15 @@
             fieldid = fieldid.index
 
         if system is not None:
             self.set_system(system)
             
         import matplotlib.pyplot as plt
 
-        fieldverts = self.geodf[["xy"]].copy()            
+        fieldverts = self.geodf[["xy"]].copy()
         if fieldid is not None:
             fieldverts = fieldverts.loc[fieldid]
             
         if ax is None:
             ax = self.add_axes(reset=True)
 
         self._plotting["ax"] = ax
```

### Comparing `ztffields-0.4.0/ztffields/projection.py` & `ztffields-0.4.1/ztffields/projection.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,20 +35,67 @@
     """ """
     return FieldProjection.radec_to_fieldid(radecs, level=level, **kwargs)
 
 def fieldid_to_radec(fieldid, level="focalplane", **kwargs):
     """ """
     return FieldProjection.fieldid_to_radec(fieldid, level=level, **kwargs)
 
-
 # ============== #
 #                #
 # Generic Tools  #
 #                #
 # ============== #
+def project_to_radec(verts_or_polygon, ra, dec):
+    """ project a geometry (or its vertices) to given ra, dec coordinates
+    
+    Parameters
+    ----------
+    verts_or_polygon: shapely.Polygon or 2d-array
+        geometry or vertices representing the camera footprint in the sky
+        if vertices, the format is: x, y = vertices
+
+    ra: float or array
+        poiting(s) R.A.
+
+    dec: float or array
+        poiting(s) declination
+
+    Returns
+    -------
+    list
+        if input are vertices
+        - list of new verticies
+        if input are geometry
+        - list of new geometries
+
+    """
+    from .utils import rot_xz_sph
+    
+    if type(verts_or_polygon) == geometry.Polygon: # polygon
+        as_polygon = True
+        fra, fdec = np.asarray(verts_or_polygon.exterior.xy)
+    else:
+        as_polygon = False
+        fra, fdec = np.asarray(verts_or_polygon)
+    
+    ra = np.atleast_1d(ra)
+    dec = np.atleast_1d(dec)
+    ra_, dec_ = np.squeeze(rot_xz_sph((fra/np.cos(fdec*np.pi/180))[:,None], 
+                                            fdec[:,None], 
+                                            dec)
+                          )
+    ra_ += ra
+    pointings = np.asarray([ra_, dec_]).T
+    if as_polygon:
+        return [geometry.Polygon(p) for p in pointings]
+    
+    return pointings
+
+
+
 def spatialjoin_radec_to_fields(radec, fields,
                                 how="inner", predicate="intersects",
                                 index_radec="index_radec", **kwargs):
     """ join the radecs with the fields
 
     Parameters
     ----------
```

### Comparing `ztffields-0.4.0/ztffields/utils.py` & `ztffields-0.4.1/ztffields/utils.py`

 * *Files identical despite different names*

### Comparing `ztffields-0.4.0/ztffields.egg-info/PKG-INFO` & `ztffields-0.4.1/ztffields.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ztffields
-Version: 0.4.0
+Version: 0.4.1
 Summary: Access and Interact with ZTF Fields
 Home-page: https://github.com/MickaelRigault/ztffields
 Author: Mickael Rigault
 Author-email: m.rigault@ipnl.in2p3.fr
 License: BSD 3-Clause "New" or "Revised" License
 Keywords: astronomy,astrophysics
 Classifier: Development Status :: 2 - Pre-Alpha
```

