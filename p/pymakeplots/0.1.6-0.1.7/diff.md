# Comparing `tmp/pymakeplots-0.1.6.tar.gz` & `tmp/pymakeplots-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymakeplots-0.1.6.tar", last modified: Fri Mar 31 14:21:08 2023, max compression
+gzip compressed data, was "pymakeplots-0.1.7.tar", last modified: Thu Jun 22 09:35:05 2023, max compression
```

## Comparing `pymakeplots-0.1.6.tar` & `pymakeplots-0.1.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 tdavis     (501) staff       (20)        0 2023-03-31 14:21:08.499700 pymakeplots-0.1.6/
--rw-r--r--   0 tdavis     (501) staff       (20)     1077 2020-09-02 10:40:49.000000 pymakeplots-0.1.6/LICENSE.md
--rw-r--r--   0 tdavis     (501) staff       (20)     1664 2023-03-31 14:21:08.499525 pymakeplots-0.1.6/PKG-INFO
--rwxr-xr-x   0 tdavis     (501) staff       (20)     1225 2020-09-04 16:00:00.000000 pymakeplots-0.1.6/README.md
-drwxr-xr-x   0 tdavis     (501) staff       (20)        0 2023-03-31 14:21:08.497909 pymakeplots-0.1.6/pymakeplots/
--rwxr-xr-x   0 tdavis     (501) staff       (20)       87 2020-09-02 10:31:25.000000 pymakeplots-0.1.6/pymakeplots/__init__.py
--rw-r--r--   0 tdavis     (501) staff       (20)    44016 2023-01-19 14:42:30.000000 pymakeplots-0.1.6/pymakeplots/pymakeplots.py
--rwxr-xr-x   0 tdavis     (501) staff       (20)     4448 2020-08-19 16:57:22.000000 pymakeplots-0.1.6/pymakeplots/sauron_colormap.py
-drwxr-xr-x   0 tdavis     (501) staff       (20)        0 2023-03-31 14:21:08.499285 pymakeplots-0.1.6/pymakeplots.egg-info/
--rw-r--r--   0 tdavis     (501) staff       (20)     1664 2023-03-31 14:21:08.000000 pymakeplots-0.1.6/pymakeplots.egg-info/PKG-INFO
--rw-r--r--   0 tdavis     (501) staff       (20)      315 2023-03-31 14:21:08.000000 pymakeplots-0.1.6/pymakeplots.egg-info/SOURCES.txt
--rw-r--r--   0 tdavis     (501) staff       (20)        1 2023-03-31 14:21:08.000000 pymakeplots-0.1.6/pymakeplots.egg-info/dependency_links.txt
--rw-r--r--   0 tdavis     (501) staff       (20)       68 2023-03-31 14:21:08.000000 pymakeplots-0.1.6/pymakeplots.egg-info/requires.txt
--rw-r--r--   0 tdavis     (501) staff       (20)       12 2023-03-31 14:21:08.000000 pymakeplots-0.1.6/pymakeplots.egg-info/top_level.txt
--rw-r--r--   0 tdavis     (501) staff       (20)        1 2020-09-02 10:52:50.000000 pymakeplots-0.1.6/pymakeplots.egg-info/zip-safe
--rw-r--r--   0 tdavis     (501) staff       (20)       38 2023-03-31 14:21:08.499752 pymakeplots-0.1.6/setup.cfg
--rw-r--r--   0 tdavis     (501) staff       (20)      914 2023-03-31 14:20:41.000000 pymakeplots-0.1.6/setup.py
+drwxr-xr-x   0 tdavis     (501) staff       (20)        0 2023-06-22 09:35:05.581225 pymakeplots-0.1.7/
+-rw-r--r--   0 tdavis     (501) staff       (20)     1077 2020-09-02 10:40:49.000000 pymakeplots-0.1.7/LICENSE.md
+-rw-r--r--   0 tdavis     (501) staff       (20)     1664 2023-06-22 09:35:05.581051 pymakeplots-0.1.7/PKG-INFO
+-rwxr-xr-x   0 tdavis     (501) staff       (20)     1225 2020-09-04 16:00:00.000000 pymakeplots-0.1.7/README.md
+drwxr-xr-x   0 tdavis     (501) staff       (20)        0 2023-06-22 09:35:05.579921 pymakeplots-0.1.7/pymakeplots/
+-rwxr-xr-x   0 tdavis     (501) staff       (20)       87 2020-09-02 10:31:25.000000 pymakeplots-0.1.7/pymakeplots/__init__.py
+-rw-r--r--   0 tdavis     (501) staff       (20)    43998 2023-06-15 14:31:16.000000 pymakeplots-0.1.7/pymakeplots/pymakeplots.py
+-rwxr-xr-x   0 tdavis     (501) staff       (20)     4448 2020-08-19 16:57:22.000000 pymakeplots-0.1.7/pymakeplots/sauron_colormap.py
+drwxr-xr-x   0 tdavis     (501) staff       (20)        0 2023-06-22 09:35:05.580833 pymakeplots-0.1.7/pymakeplots.egg-info/
+-rw-r--r--   0 tdavis     (501) staff       (20)     1664 2023-06-22 09:35:05.000000 pymakeplots-0.1.7/pymakeplots.egg-info/PKG-INFO
+-rw-r--r--   0 tdavis     (501) staff       (20)      315 2023-06-22 09:35:05.000000 pymakeplots-0.1.7/pymakeplots.egg-info/SOURCES.txt
+-rw-r--r--   0 tdavis     (501) staff       (20)        1 2023-06-22 09:35:05.000000 pymakeplots-0.1.7/pymakeplots.egg-info/dependency_links.txt
+-rw-r--r--   0 tdavis     (501) staff       (20)       68 2023-06-22 09:35:05.000000 pymakeplots-0.1.7/pymakeplots.egg-info/requires.txt
+-rw-r--r--   0 tdavis     (501) staff       (20)       12 2023-06-22 09:35:05.000000 pymakeplots-0.1.7/pymakeplots.egg-info/top_level.txt
+-rw-r--r--   0 tdavis     (501) staff       (20)        1 2020-09-02 10:52:50.000000 pymakeplots-0.1.7/pymakeplots.egg-info/zip-safe
+-rw-r--r--   0 tdavis     (501) staff       (20)       38 2023-06-22 09:35:05.581272 pymakeplots-0.1.7/setup.cfg
+-rw-r--r--   0 tdavis     (501) staff       (20)      914 2023-06-22 09:34:20.000000 pymakeplots-0.1.7/setup.py
```

### Comparing `pymakeplots-0.1.6/LICENSE.md` & `pymakeplots-0.1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pymakeplots-0.1.6/PKG-INFO` & `pymakeplots-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymakeplots
-Version: 0.1.6
+Version: 0.1.7
 Home-page: https://github.com/TimothyADavis/pymakeplots
 Author: Timothy A. Davis
 Author-email: DavisT@cardiff.ac.uk
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pymakeplots-0.1.6/README.md` & `pymakeplots-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pymakeplots-0.1.6/pymakeplots/pymakeplots.py` & `pymakeplots-0.1.7/pymakeplots/pymakeplots.py`

 * *Files 2% similar despite different names*

```diff
@@ -291,16 +291,16 @@
         matplotlib.rcParams["ytick.minor.visible"] = True
         #params = {'mathtext.default': 'regular'}
         #matplotlib.rcParams.update(params)
         matplotlib.rcParams['axes.labelsize'] = 20*mult
         
            
     def rms_estimate(self,cube,chanstart,chanend):
-        quarterx=np.array(cube.shape[0]/4.).astype(np.int)
-        quartery=np.array(cube.shape[1]/4.).astype(np.int)
+        quarterx=np.array(cube.shape[0]/4.).astype(int)
+        quartery=np.array(cube.shape[1]/4.).astype(int)
         return np.nanstd(cube[quarterx*1:3*quarterx,1*quartery:3*quartery,chanstart:chanend])
         
     def get_header_coord_arrays(self,hdr):
 
         y,x=self.spectralcube.spatial_coordinate_map
 
         x1=np.median(x[0:hdr['NAXIS2'],0:hdr['NAXIS1']],0).value
@@ -551,15 +551,15 @@
             barlength_arc=  barlength_pc/(4.84*self.gal_distance)
             
             
         
         if np.log10(barlength_pc) > 3:
             label=(barlength_pc/1e3).astype(np.str)+ " kpc"
         else:
-            label=barlength_pc.astype(np.int).astype(np.str)+ " pc"
+            label=barlength_pc.astype(int).astype(np.str)+ " pc"
             
         asb = AnchoredSizeBar(ax.transData,  barlength_arc,   label,  loc=loc,  pad=0.25, borderpad=0.5, sep=5, frameon=False)
         ax.add_artist(asb)
         
         
         
         
@@ -606,15 +606,15 @@
             wy_low,=np.where(cumulative_y < 0.02)
             if wy_low.size ==0: wy_low=np.array([0])
             wy_high,=np.where(cumulative_y > 0.98)
             if wy_high.size ==0: wy_high=np.array([cumulative_y.size])
             
 
             
-            beam_in_pix = np.int(np.ceil(self.bmaj/self.cellsize))
+            beam_in_pix = int(np.ceil(self.bmaj/self.cellsize))
             
 
             self.spatial_trim = [np.clip(np.max(wx_low) - 2*beam_in_pix,0,self.xcoord.size),np.clip(np.min(wx_high) + 2*beam_in_pix,0,self.xcoord.size)\
                                 , np.clip(np.max(wy_low) - 2*beam_in_pix,0,self.ycoord.size), np.clip(np.min(wy_high) + 2*beam_in_pix,0,self.ycoord.size)]
             
         #breakpoint()
         #print(np.where(np.isclose(self.xcoord-self.obj_ra,0,atol=self.cellsize/3600)))   
@@ -970,15 +970,15 @@
         centpix_y=np.where(np.isclose(self.yc,0.0,atol=self.cellsize/1.9))[0]
         
 
 
         rotcube= rotateImage(self.pbcorr_cube_trim*self.mask_trim,90-self.posang,[centpix_x[0],centpix_y[0]])
 
 
-        pvd=rotcube[:,np.array(rotcube.shape[1]//2-self.pvdthick).astype(np.int):np.array(rotcube.shape[1]//2+self.pvdthick).astype(np.int),:].sum(axis=1)
+        pvd=rotcube[:,np.array(rotcube.shape[1]//2-self.pvdthick).astype(int):np.array(rotcube.shape[1]//2+self.pvdthick).astype(int),:].sum(axis=1)
         
 
         
         if self.posang < 180:
             loc1="upper left"
             loc2="lower right"
         else:
```

### Comparing `pymakeplots-0.1.6/pymakeplots/sauron_colormap.py` & `pymakeplots-0.1.7/pymakeplots/sauron_colormap.py`

 * *Files identical despite different names*

### Comparing `pymakeplots-0.1.6/pymakeplots.egg-info/PKG-INFO` & `pymakeplots-0.1.7/pymakeplots.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymakeplots
-Version: 0.1.6
+Version: 0.1.7
 Home-page: https://github.com/TimothyADavis/pymakeplots
 Author: Timothy A. Davis
 Author-email: DavisT@cardiff.ac.uk
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pymakeplots-0.1.6/setup.py` & `pymakeplots-0.1.7/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
  
 setup(name='pymakeplots',
-       version='0.1.6',
+       version='0.1.7',
        description='',
        url='https://github.com/TimothyADavis/pymakeplots',
        author='Timothy A. Davis',
        author_email='DavisT@cardiff.ac.uk',
        long_description=long_description,
        long_description_content_type="text/markdown",
        license='MIT',
```

