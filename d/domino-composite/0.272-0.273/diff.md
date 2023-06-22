# Comparing `tmp/domino-composite-0.272.tar.gz` & `tmp/domino-composite-0.273.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domino-composite-0.272.tar", last modified: Mon Jun 19 15:48:06 2023, max compression
+gzip compressed data, was "domino-composite-0.273.tar", last modified: Thu Jun 22 14:50:09 2023, max compression
```

## Comparing `domino-composite-0.272.tar` & `domino-composite-0.273.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 ox5324   (243050) imk-tro  (44470)        0 2023-06-19 15:48:06.718695 domino-composite-0.272/
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     1213 2023-06-19 15:48:06.718695 domino-composite-0.272/PKG-INFO
-drwxr-xr-x   0 ox5324   (243050) imk-tro  (44470)        0 2023-06-19 15:48:06.718695 domino-composite-0.272/domino/
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)       62 2022-11-23 14:01:08.000000 domino-composite-0.272/domino/__init__.py
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     1034 2023-06-19 15:18:52.000000 domino-composite-0.272/domino/agg.py
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     2702 2022-11-23 14:10:17.000000 domino-composite-0.272/domino/categorical_analysis.py
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)    50731 2023-06-19 15:18:52.000000 domino-composite-0.272/domino/core.py
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     4248 2023-01-30 10:05:05.000000 domino-composite-0.272/domino/deseasonaliser.py
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     3851 2023-06-19 15:47:52.000000 domino-composite-0.272/domino/filtering.py
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     4784 2023-04-03 16:12:11.000000 domino-composite-0.272/domino/plsr.py
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)    14070 2023-04-12 16:04:19.000000 domino-composite-0.272/domino/prediction.py
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     5814 2023-06-19 15:18:52.000000 domino-composite-0.272/domino/util.py
-drwxr-xr-x   0 ox5324   (243050) imk-tro  (44470)        0 2023-06-19 15:48:06.718695 domino-composite-0.272/domino_composite.egg-info/
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     1213 2023-06-19 15:48:06.000000 domino-composite-0.272/domino_composite.egg-info/PKG-INFO
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)      382 2023-06-19 15:48:06.000000 domino-composite-0.272/domino_composite.egg-info/SOURCES.txt
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)        1 2023-06-19 15:48:06.000000 domino-composite-0.272/domino_composite.egg-info/dependency_links.txt
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)       62 2023-06-19 15:48:06.000000 domino-composite-0.272/domino_composite.egg-info/requires.txt
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)        7 2023-06-19 15:48:06.000000 domino-composite-0.272/domino_composite.egg-info/top_level.txt
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)       38 2023-06-19 15:48:06.718695 domino-composite-0.272/setup.cfg
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)      728 2023-06-19 15:47:59.000000 domino-composite-0.272/setup.py
+drwxr-xr-x   0 ox5324   (243050) imk-tro  (44470)        0 2023-06-22 14:50:09.374956 domino-composite-0.273/
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     1719 2023-06-22 14:50:09.374956 domino-composite-0.273/PKG-INFO
+drwxr-xr-x   0 ox5324   (243050) imk-tro  (44470)        0 2023-06-22 14:50:09.362956 domino-composite-0.273/domino/
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)       62 2022-11-23 14:01:08.000000 domino-composite-0.273/domino/__init__.py
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     1034 2023-06-19 15:18:52.000000 domino-composite-0.273/domino/agg.py
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     2702 2022-11-23 14:10:17.000000 domino-composite-0.273/domino/categorical_analysis.py
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)    50731 2023-06-19 15:18:52.000000 domino-composite-0.273/domino/core.py
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     4248 2023-01-30 10:05:05.000000 domino-composite-0.273/domino/deseasonaliser.py
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     3870 2023-06-20 12:38:32.000000 domino-composite-0.273/domino/filtering.py
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     4784 2023-04-03 16:12:11.000000 domino-composite-0.273/domino/plsr.py
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)    14070 2023-04-12 16:04:19.000000 domino-composite-0.273/domino/prediction.py
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     5814 2023-06-19 15:18:52.000000 domino-composite-0.273/domino/util.py
+drwxr-xr-x   0 ox5324   (243050) imk-tro  (44470)        0 2023-06-22 14:50:09.374956 domino-composite-0.273/domino_composite.egg-info/
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     1719 2023-06-22 14:50:09.000000 domino-composite-0.273/domino_composite.egg-info/PKG-INFO
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)      382 2023-06-22 14:50:09.000000 domino-composite-0.273/domino_composite.egg-info/SOURCES.txt
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)        1 2023-06-22 14:50:09.000000 domino-composite-0.273/domino_composite.egg-info/dependency_links.txt
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)       62 2023-06-22 14:50:09.000000 domino-composite-0.273/domino_composite.egg-info/requires.txt
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)        7 2023-06-22 14:50:09.000000 domino-composite-0.273/domino_composite.egg-info/top_level.txt
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)       38 2023-06-22 14:50:09.374956 domino-composite-0.273/setup.cfg
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)      728 2023-06-22 14:49:41.000000 domino-composite-0.273/setup.py
```

### Comparing `domino-composite-0.272/PKG-INFO` & `domino-composite-0.273/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 Metadata-Version: 2.1
 Name: domino-composite
-Version: 0.272
+Version: 0.273
 Summary: A package for compositing atmospheric datasets
 Home-page: https://github.com/joshdorrington/domino
 Author: Josh Dorrington
 Author-email: joshua.dorrington@kit.edu
 License: bsd-3-clause
 Description-Content-Type: text/markdown
 
 # Domino is a package for analysing composites of atmospheric data.
 ## Based on xarray, Domino makes it easy to calculate lagged composites of fields and scalar indices around categorical event time series, and to compute bootstrapped confidence bounds. This is still an alpha release! While core functionality is stable, there could be some bugs!
 
 ## Documentation
 
-See https://github.com/joshdorrington/domino/blob/master/docbuild/domino-composite.pdf
+See our API reference here: https://github.com/joshdorrington/domino/blob/master/docbuild/domino-composite.pdf
 
 ## Examples
 
-A basic introduction to using the package out of the box, with three example applications:
+See our Jupyter notebook examples for more detailed discussion of how to apply Domino to different use cases.
 
-https://github.com/joshdorrington/domino/blob/master/examples/basic_usage.ipynb
+Our [basic](https://github.com/joshdorrington/domino/blob/master/examples/basic_compositing.ipynb) and [advanced](https://github.com/joshdorrington/domino/blob/master/examples/advanced_compositing.ipynb) compositing guides cover the use of Domino's flexible LaggedAnalyser class to easily compute time-lagged composites and apply bootstrap significance tests to them.
 
-A more in-depth discussion of how to customise the behaviour of the LaggedAnalyser class:
+Producing filtered precursor patterns from composites, and computing precursor activity indices from those is covered in our [IndexGenerator](https://github.com/joshdorrington/domino/blob/master/examples/precursor_index_computation.ipynb) guide.
 
-https://github.com/joshdorrington/domino/blob/master/examples/advanced_usage.ipynb
 
 ## Install
 
 domino can be installed using pip:
 ```
-python -m pip install "domino-composite==0.14"
+python -m pip install "domino-composite==0.272"
+```
+If you want to run the worked examples in the Jupyter notebooks you will need:
+```
+TO BE DECIDED
 ```
```

### Comparing `domino-composite-0.272/domino/agg.py` & `domino-composite-0.273/domino/agg.py`

 * *Files identical despite different names*

### Comparing `domino-composite-0.272/domino/categorical_analysis.py` & `domino-composite-0.273/domino/categorical_analysis.py`

 * *Files identical despite different names*

### Comparing `domino-composite-0.272/domino/core.py` & `domino-composite-0.273/domino/core.py`

 * *Files identical despite different names*

### Comparing `domino-composite-0.272/domino/deseasonaliser.py` & `domino-composite-0.273/domino/deseasonaliser.py`

 * *Files identical despite different names*

### Comparing `domino-composite-0.272/domino/filtering.py` & `domino-composite-0.273/domino/filtering.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     connected,ncon=label(grid)
     connected=connected.astype(float)
     ix,n=np.unique(connected,return_counts=True)
     
     connected_da=xr.DataArray(connected,coords=area.coords)
     ix_areas=np.array([area.where(connected_da==i).sum().values\
               for i in ix])
-
+    print(ix_areas)
     for m in ix[ix_areas<area_thresh]:
         connected[connected==m]=0
     return connected>0
 
 
 def da_large_regions(da,n,dims,area_based=False):
```

### Comparing `domino-composite-0.272/domino/plsr.py` & `domino-composite-0.273/domino/plsr.py`

 * *Files identical despite different names*

### Comparing `domino-composite-0.272/domino/prediction.py` & `domino-composite-0.273/domino/prediction.py`

 * *Files identical despite different names*

### Comparing `domino-composite-0.272/domino/util.py` & `domino-composite-0.273/domino/util.py`

 * *Files identical despite different names*

### Comparing `domino-composite-0.272/domino_composite.egg-info/PKG-INFO` & `domino-composite-0.273/domino_composite.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 Metadata-Version: 2.1
 Name: domino-composite
-Version: 0.272
+Version: 0.273
 Summary: A package for compositing atmospheric datasets
 Home-page: https://github.com/joshdorrington/domino
 Author: Josh Dorrington
 Author-email: joshua.dorrington@kit.edu
 License: bsd-3-clause
 Description-Content-Type: text/markdown
 
 # Domino is a package for analysing composites of atmospheric data.
 ## Based on xarray, Domino makes it easy to calculate lagged composites of fields and scalar indices around categorical event time series, and to compute bootstrapped confidence bounds. This is still an alpha release! While core functionality is stable, there could be some bugs!
 
 ## Documentation
 
-See https://github.com/joshdorrington/domino/blob/master/docbuild/domino-composite.pdf
+See our API reference here: https://github.com/joshdorrington/domino/blob/master/docbuild/domino-composite.pdf
 
 ## Examples
 
-A basic introduction to using the package out of the box, with three example applications:
+See our Jupyter notebook examples for more detailed discussion of how to apply Domino to different use cases.
 
-https://github.com/joshdorrington/domino/blob/master/examples/basic_usage.ipynb
+Our [basic](https://github.com/joshdorrington/domino/blob/master/examples/basic_compositing.ipynb) and [advanced](https://github.com/joshdorrington/domino/blob/master/examples/advanced_compositing.ipynb) compositing guides cover the use of Domino's flexible LaggedAnalyser class to easily compute time-lagged composites and apply bootstrap significance tests to them.
 
-A more in-depth discussion of how to customise the behaviour of the LaggedAnalyser class:
+Producing filtered precursor patterns from composites, and computing precursor activity indices from those is covered in our [IndexGenerator](https://github.com/joshdorrington/domino/blob/master/examples/precursor_index_computation.ipynb) guide.
 
-https://github.com/joshdorrington/domino/blob/master/examples/advanced_usage.ipynb
 
 ## Install
 
 domino can be installed using pip:
 ```
-python -m pip install "domino-composite==0.14"
+python -m pip install "domino-composite==0.272"
+```
+If you want to run the worked examples in the Jupyter notebooks you will need:
+```
+TO BE DECIDED
 ```
```

### Comparing `domino-composite-0.272/setup.py` & `domino-composite-0.273/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("/data/ox5324/Domino/readme.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='domino-composite',
-    version='0.272',
+    version='0.273',
     author='Josh Dorrington',
     author_email='joshua.dorrington@kit.edu',
     description='A package for compositing atmospheric datasets',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/joshdorrington/domino',
     license='bsd-3-clause',
```

