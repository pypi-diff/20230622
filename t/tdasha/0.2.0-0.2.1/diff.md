# Comparing `tmp/tdasha-0.2.0.tar.gz` & `tmp/tdasha-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdasha-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "tdasha-0.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `tdasha-0.2.0.tar` & `tdasha-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35149 2023-06-20 13:36:15.673513 tdasha-0.2.0/LICENSE
--rw-r--r--   0        0        0        8 2023-06-20 13:36:15.673513 tdasha-0.2.0/README.md
--rw-r--r--   0        0        0      971 2023-06-20 13:36:15.673513 tdasha-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      234 2023-06-20 13:36:15.673513 tdasha-0.2.0/tdasha/__init__.py
--rw-r--r--   0        0        0    13900 2023-06-20 13:36:15.673513 tdasha-0.2.0/tdasha/compute.py
--rw-r--r--   0        0        0     2723 2023-06-20 13:36:15.673513 tdasha-0.2.0/tdasha/io.py
--rw-r--r--   0        0        0     8662 2023-06-20 13:36:15.673513 tdasha-0.2.0/tdasha/window.py
--rw-r--r--   0        0        0      858 1970-01-01 00:00:00.000000 tdasha-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-22 12:22:19.781541 tdasha-0.2.1/LICENSE
+-rw-r--r--   0        0        0        8 2023-06-22 12:22:19.781541 tdasha-0.2.1/README.md
+-rw-r--r--   0        0        0     1059 2023-06-22 12:22:19.781541 tdasha-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      234 2023-06-22 12:22:19.781541 tdasha-0.2.1/tdasha/__init__.py
+-rw-r--r--   0        0        0    13900 2023-06-22 12:22:19.781541 tdasha-0.2.1/tdasha/compute.py
+-rw-r--r--   0        0        0     3696 2023-06-22 12:22:19.781541 tdasha-0.2.1/tdasha/io.py
+-rw-r--r--   0        0        0     8662 2023-06-22 12:22:19.781541 tdasha-0.2.1/tdasha/window.py
+-rw-r--r--   0        0        0      984 1970-01-01 00:00:00.000000 tdasha-0.2.1/PKG-INFO
```

### Comparing `tdasha-0.2.0/LICENSE` & `tdasha-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tdasha-0.2.0/pyproject.toml` & `tdasha-0.2.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 authors = [
   {name = "Stanisław Lasocki"},
   {name = "Francis Tong"},
 ]
 description = "Time-dependent Anthropogenic Seismic Hazard Assessment"
 name = "tdasha"
-version = "0.2.0"
+version = "0.2.1"
 readme = "README.md"
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
 	"Programming Language :: Python :: 3",
 	"Programming Language :: Python :: 3.8",
 	"Programming Language :: Python :: 3.9",
 	"Programming Language :: Python :: 3.10",
@@ -24,14 +24,18 @@
 	"Operating System :: OS Independent",
 ]
 license = {file = "LICENSE"}
 requires-python = ">=3.8"
 dependencies = [
     "numpy >=1.21.6",
     "scipy >=1.7.3",
+    "obspy >=1.4.0",
+	"KDEpy >=1.1.3",
+    "adaptivekde >=1.1.1",
+	"resample >= 1.6.0",
 ]
 
 [project.urls]
 Source = "https://github.com/francistong/tdasha"
 
 [tool.flit.sdist]
 exclude = ["./docs"]
```

### Comparing `tdasha-0.2.0/tdasha/compute.py` & `tdasha-0.2.1/tdasha/compute.py`

 * *Files identical despite different names*

### Comparing `tdasha-0.2.0/tdasha/io.py` & `tdasha-0.2.1/tdasha/io.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,49 @@
 # -*- coding: utf-8 -*-
 """
 @author: ftong
 """
+import sys
 import pandas as pd
+import scipy.io
 from obspy import UTCDateTime
 from obspy.clients.fdsn import Client
 from obspy import read_events
 import numpy as np
 
+
+def read_mat(matlab_file, mag_label, **kwargs):
+    
+    mag = []
+    time = []
+    
+    mat = scipy.io.loadmat(matlab_file)
+
+    for i in range(0,len(mat['Catalog'][0])):
+        
+        # Extract magnitudes
+        if mat['Catalog'][0][i][0]==mag_label:
+            mag_frame = mat['Catalog'][0][i]
+            mag = mag_frame[2].flatten()
+            continue
+    
+        # Extract times
+        if mat['Catalog'][0][i][0]=='Time':
+            time_frame = mat['Catalog'][0][i]
+            t1 = time_frame[2].flatten()
+            datenums = np.array(t1)
+            t2= pd.to_datetime(datenums-719529, unit='D') #convert from Matlab's datenum format to human readable format
+            time = [UTCDateTime(str(t)) for t in t2] # convert to list of obspy UTCDateTime objects
+            
+    if len(mag)==0:
+        print("Magnitude column not found in .mat file")
+        sys.exit()
+
+    return time, mag
+
 def read_csv(csv_file,  datenum= True, **kwargs):
     
     # df = pd.read_csv(csv_file, engine="pyarrow", **kwargs) #use pyarrow for faster input
     df = pd.read_csv(csv_file, **kwargs)
     
     df.columns= df.columns.str.lower() # convert header to all lowercase letters
     header = df.columns
```

### Comparing `tdasha-0.2.0/tdasha/window.py` & `tdasha-0.2.1/tdasha/window.py`

 * *Files identical despite different names*

