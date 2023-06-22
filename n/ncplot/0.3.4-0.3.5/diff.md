# Comparing `tmp/ncplot-0.3.4.tar.gz` & `tmp/ncplot-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncplot-0.3.4.tar", last modified: Tue Jun  6 17:18:18 2023, max compression
+gzip compressed data, was "ncplot-0.3.5.tar", last modified: Thu Jun 22 16:06:44 2023, max compression
```

## Comparing `ncplot-0.3.4.tar` & `ncplot-0.3.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:18:18.293346 ncplot-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-06 17:18:08.000000 ncplot-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-06 17:18:08.000000 ncplot-0.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-06-06 17:18:18.293346 ncplot-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-06-06 17:18:08.000000 ncplot-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:18:18.293346 ncplot-0.3.4/ncplot/
--rwxr-xr-x   0 runner    (1001) docker     (123)       29 2023-06-06 17:18:08.000000 ncplot-0.3.4/ncplot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-06 17:18:08.000000 ncplot-0.3.4/ncplot/command_line.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:18:08.000000 ncplot-0.3.4/ncplot/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)    35927 2023-06-06 17:18:08.000000 ncplot-0.3.4/ncplot/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-06-06 17:18:08.000000 ncplot-0.3.4/ncplot/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-06 17:18:08.000000 ncplot-0.3.4/ncplot/xarray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:18:18.293346 ncplot-0.3.4/ncplot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-06 17:18:18.000000 ncplot-0.3.4/ncplot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-06 17:18:08.000000 ncplot-0.3.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 17:18:18.293346 ncplot-0.3.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1952 2023-06-06 17:18:08.000000 ncplot-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:06:44.484436 ncplot-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-22 16:06:30.000000 ncplot-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-22 16:06:30.000000 ncplot-0.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-06-22 16:06:44.480435 ncplot-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-06-22 16:06:30.000000 ncplot-0.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:06:44.480435 ncplot-0.3.5/ncplot/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       29 2023-06-22 16:06:30.000000 ncplot-0.3.5/ncplot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-22 16:06:30.000000 ncplot-0.3.5/ncplot/command_line.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:06:30.000000 ncplot-0.3.5/ncplot/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35985 2023-06-22 16:06:30.000000 ncplot-0.3.5/ncplot/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-06-22 16:06:30.000000 ncplot-0.3.5/ncplot/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-22 16:06:30.000000 ncplot-0.3.5/ncplot/xarray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:06:44.480435 ncplot-0.3.5/ncplot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-22 16:06:44.000000 ncplot-0.3.5/ncplot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-22 16:06:30.000000 ncplot-0.3.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 16:06:44.484436 ncplot-0.3.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1952 2023-06-22 16:06:30.000000 ncplot-0.3.5/setup.py
```

### Comparing `ncplot-0.3.4/LICENSE` & `ncplot-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ncplot-0.3.4/MANIFEST.in` & `ncplot-0.3.5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `ncplot-0.3.4/PKG-INFO` & `ncplot-0.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncplot
-Version: 0.3.4
+Version: 0.3.5
 Summary: Interactive viewing of NetCDF data
 Home-page: https://github.com/pmlmodelling/ncplot
 Author: Robert Wilson
 Author-email: rwi@pml.ac.uk
 Maintainer: Robert Wilson
 Project-URL: Bug Tracker, https://github.com/pmlmodelling/ncplot/issues
 Project-URL: Documentation, https://ncplot.readthedocs.io/en/stable
```

### Comparing `ncplot-0.3.4/README.md` & `ncplot-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `ncplot-0.3.4/ncplot/command_line.py` & `ncplot-0.3.5/ncplot/command_line.py`

 * *Files identical despite different names*

### Comparing `ncplot-0.3.4/ncplot/plot.py` & `ncplot-0.3.5/ncplot/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,15 +211,14 @@
         xr_file = False
 
     nc_vars = None
     if xr_file is False:
         try:
             try:
                 import nctoolkit as nc
-                warnings.warn("Checking if nctoolkit is available")
 
                 if os.path.exists(x):
                     ds = nc.open_data(x)
                     nc_vars = ds.variables
                     ds = ds.to_xarray()
                 else:
                     ds = nc.open_thredds(x)
@@ -234,14 +233,15 @@
         ds = x
 
     if type(vars) is list:
         ds = ds[vars]
 
     coord_list = list(ds.coords)
 
+
     for cc in coord_list:
         if len(ds[cc].values.ravel()) <= 1:
             if cc in list(ds.dims):
                 ds = ds.squeeze(cc, drop=True)
 
     coord_list = list(ds.dims)
 
@@ -294,24 +294,26 @@
                 if "long_name" in ds[lon_name].attrs:
                     if "rotate" in ds[lon_name].long_name:
                         coastline = False
 
                     if "pole" in ds[lon_name].long_name:
                         coastline = False
 
-    if lon_name is not None:
-        for vv in ds.variables:
-            if lon_name not in list(ds[vv].dims):
-                if lat_name not in list(ds[vv].dims):
-                    if "time" not in list(ds[vv].dims):
-                        bad += [vv]
-    
-        if len(bad) > 0:
-            ds = ds.drop(bad)
-
+    #print(ds.data_vars)
+    #if lon_name is not None:
+    #    for vv in ds.data_vars:
+    #        if lon_name not in list(ds[vv].dims):
+    #            if lat_name not in list(ds[vv].dims):
+    #                [x for x in list(ds[vv].dims] if "time" in x'
+    #                if "time" not in list(ds[vv].dims):
+    #                    bad += [vv]
+    #
+    #    if len(bad) > 0:
+    #        ds = ds.drop(bad)
+    #print(ds.data_vars)
 
     if len([x for x in ds.coords if "lon" in x]) > len(
         [x for x in ds.dims if "lon" in x]
     ):
         coastline = False
 
     if quadmesh is False and lat_name is not None:
@@ -415,15 +417,15 @@
     else:
         if ds[possible_others[0]].values.ndim == 0:
             n_levels = 0
         else:
             n_levels = len(ds[possible_others[0]].values)
 
     if vars is None:
-        vars = [x for x in list(ds.variables) if x not in ff_dims]
+        vars = [x for x in list(ds.data_vars) if x not in ff_dims]
 
         # also must have all of the coordinates...
 
     # code below figures out what is a variable, not a coordinate. Could be improved...
 
     coord_list = list(ds.coords)
 
@@ -444,18 +446,18 @@
 
     if type(vars) is list:
         if len(vars) == 1:
             vars = vars[0]
 
     if type(vars) is list:
         for vv in vars:
-            if vv not in list(ds.variables):
+            if vv not in list(ds.data_vars):
                 raise ValueError(f"{vv} is not a valid variable")
     else:
-        if vars not in list(ds.variables):
+        if vars not in list(ds.data_vars):
             raise ValueError(f"{vars} is not a valid variable")
 
     if (lon_name is not None) and (lat_name is not None) and type(vars) is list:
         new_vars = []
         for x in vars:
 
             dims_required = []
```

### Comparing `ncplot-0.3.4/ncplot/utils.py` & `ncplot-0.3.5/ncplot/utils.py`

 * *Files identical despite different names*

### Comparing `ncplot-0.3.4/ncplot/xarray.py` & `ncplot-0.3.5/ncplot/xarray.py`

 * *Files identical despite different names*

### Comparing `ncplot-0.3.4/setup.py` & `ncplot-0.3.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         ],
 }
 
 
 extras_require["complete"] = ["geoviews"]
 
 setup(name='ncplot',
-      version='0.3.4',
+      version='0.3.5',
       description=DESCRIPTION,
       long_description=long_description,
       long_description_content_type='text/markdown',
 
       python_requires='>=3.6.1',
 
       entry_points={
```

