# Comparing `tmp/UComp-1.0.72.tar.gz` & `tmp/UComp-1.0.73.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UComp-1.0.72.tar", last modified: Wed Jun 21 07:45:44 2023, max compression
+gzip compressed data, was "UComp-1.0.73.tar", last modified: Thu Jun 22 08:42:26 2023, max compression
```

## Comparing `UComp-1.0.72.tar` & `UComp-1.0.73.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 07:45:44.124151 UComp-1.0.72/
--rw-rw-rw-   0        0        0      403 2023-06-19 10:16:42.000000 UComp-1.0.72/MANIFEST.in
--rw-rw-rw-   0        0        0      343 2023-06-21 07:45:44.125108 UComp-1.0.72/PKG-INFO
--rw-rw-rw-   0        0        0       37 2023-05-19 10:25:10.000000 UComp-1.0.72/README.md
-drwxrwxrwx   0        0        0        0 2023-06-21 07:45:44.084790 UComp-1.0.72/UComp/
--rw-rw-rw-   0        0        0  1451960 2023-06-19 14:44:58.000000 UComp-1.0.72/UComp/ETSc.cpython-311-darwin.so
--rw-rw-rw-   0        0        0   573952 2023-05-19 09:06:21.000000 UComp-1.0.72/UComp/ETSc.pyd
--rw-rw-rw-   0        0        0    11479 2023-06-19 11:59:12.000000 UComp-1.0.72/UComp/ETSmodule.py
--rw-rw-rw-   0        0        0     3378 2023-06-19 10:14:45.000000 UComp-1.0.72/UComp/Nile.bin
--rw-rw-rw-   0        0        0    11803 2023-06-21 07:43:25.000000 UComp-1.0.72/UComp/PTSmodule.py
--rw-rw-rw-   0        0        0  1631200 2023-06-19 14:46:05.000000 UComp-1.0.72/UComp/UCc.cpython-311-darwin.so
--rw-rw-rw-   0        0        0   897024 2023-06-16 11:32:46.000000 UComp-1.0.72/UComp/UCc.pyd
--rw-rw-rw-   0        0        0    24622 2023-06-19 15:35:54.000000 UComp-1.0.72/UComp/UCmodule.py
--rw-rw-rw-   0        0        0      149 2023-06-09 15:38:31.000000 UComp-1.0.72/UComp/__init__.py
--rw-rw-rw-   0        0        0    16459 2023-06-14 08:43:27.000000 UComp-1.0.72/UComp/airpas.bin
--rw-rw-rw-   0        0        0     3645 2023-06-14 08:43:27.000000 UComp-1.0.72/UComp/gdp.bin
--rw-rw-rw-   0        0        0    14731 2023-06-14 08:43:27.000000 UComp-1.0.72/UComp/ipi.bin
--rw-rw-rw-   0        0        0 32492623 2016-06-16 16:24:20.000000 UComp-1.0.72/UComp/libopenblas.dll
--rw-rw-rw-   0        0        0    29863 2023-06-19 12:06:54.000000 UComp-1.0.72/UComp/tools.py
--rw-rw-rw-   0        0        0      641 2023-06-15 07:05:30.000000 UComp-1.0.72/UComp/tsfile.py
-drwxrwxrwx   0        0        0        0 2023-06-21 07:45:44.122103 UComp-1.0.72/UComp.egg-info/
--rw-rw-rw-   0        0        0      343 2023-06-21 07:45:43.000000 UComp-1.0.72/UComp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      465 2023-06-21 07:45:43.000000 UComp-1.0.72/UComp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 07:45:43.000000 UComp-1.0.72/UComp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-06-21 07:45:43.000000 UComp-1.0.72/UComp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-21 07:45:43.000000 UComp-1.0.72/UComp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-21 07:45:44.127909 UComp-1.0.72/setup.cfg
--rw-rw-rw-   0        0        0      667 2023-06-21 07:44:40.000000 UComp-1.0.72/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 08:42:26.878253 UComp-1.0.73/
+-rw-rw-rw-   0        0        0      403 2023-06-19 10:16:42.000000 UComp-1.0.73/MANIFEST.in
+-rw-rw-rw-   0        0        0      343 2023-06-22 08:42:26.878253 UComp-1.0.73/PKG-INFO
+-rw-rw-rw-   0        0        0       37 2023-05-19 10:25:10.000000 UComp-1.0.73/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 08:42:26.837018 UComp-1.0.73/UComp/
+-rw-rw-rw-   0        0        0  1451960 2023-06-19 14:44:58.000000 UComp-1.0.73/UComp/ETSc.cpython-311-darwin.so
+-rw-rw-rw-   0        0        0   573952 2023-05-19 09:06:21.000000 UComp-1.0.73/UComp/ETSc.pyd
+-rw-rw-rw-   0        0        0    11479 2023-06-22 08:39:51.000000 UComp-1.0.73/UComp/ETSmodule.py
+-rw-rw-rw-   0        0        0     3378 2023-06-19 10:14:45.000000 UComp-1.0.73/UComp/Nile.bin
+-rw-rw-rw-   0        0        0    11803 2023-06-22 08:39:36.000000 UComp-1.0.73/UComp/PTSmodule.py
+-rw-rw-rw-   0        0        0  1631200 2023-06-19 14:46:05.000000 UComp-1.0.73/UComp/UCc.cpython-311-darwin.so
+-rw-rw-rw-   0        0        0   897024 2023-06-16 11:32:46.000000 UComp-1.0.73/UComp/UCc.pyd
+-rw-rw-rw-   0        0        0    24622 2023-06-22 08:39:44.000000 UComp-1.0.73/UComp/UCmodule.py
+-rw-rw-rw-   0        0        0      149 2023-06-09 15:38:31.000000 UComp-1.0.73/UComp/__init__.py
+-rw-rw-rw-   0        0        0    16459 2023-06-14 08:43:27.000000 UComp-1.0.73/UComp/airpas.bin
+-rw-rw-rw-   0        0        0     3645 2023-06-14 08:43:27.000000 UComp-1.0.73/UComp/gdp.bin
+-rw-rw-rw-   0        0        0    14731 2023-06-14 08:43:27.000000 UComp-1.0.73/UComp/ipi.bin
+-rw-rw-rw-   0        0        0 32492623 2016-06-16 16:24:20.000000 UComp-1.0.73/UComp/libopenblas.dll
+-rw-rw-rw-   0        0        0    30193 2023-06-22 08:39:27.000000 UComp-1.0.73/UComp/tools.py
+-rw-rw-rw-   0        0        0      641 2023-06-15 07:05:30.000000 UComp-1.0.73/UComp/tsfile.py
+drwxrwxrwx   0        0        0        0 2023-06-22 08:42:26.878253 UComp-1.0.73/UComp.egg-info/
+-rw-rw-rw-   0        0        0      343 2023-06-22 08:42:26.000000 UComp-1.0.73/UComp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      465 2023-06-22 08:42:26.000000 UComp-1.0.73/UComp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 08:42:26.000000 UComp-1.0.73/UComp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-06-22 08:42:26.000000 UComp-1.0.73/UComp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-22 08:42:26.000000 UComp-1.0.73/UComp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-22 08:42:26.878253 UComp-1.0.73/setup.cfg
+-rw-rw-rw-   0        0        0      667 2023-06-22 08:42:23.000000 UComp-1.0.73/setup.py
```

### Comparing `UComp-1.0.72/UComp/ETSc.cpython-311-darwin.so` & `UComp-1.0.73/UComp/ETSc.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `UComp-1.0.72/UComp/ETSmodule.py` & `UComp-1.0.73/UComp/ETSmodule.py`

 * *Files identical despite different names*

### Comparing `UComp-1.0.72/UComp/Nile.bin` & `UComp-1.0.73/UComp/Nile.bin`

 * *Files identical despite different names*

### Comparing `UComp-1.0.72/UComp/PTSmodule.py` & `UComp-1.0.73/UComp/PTSmodule.py`

 * *Files identical despite different names*

### Comparing `UComp-1.0.72/UComp/UCc.cpython-311-darwin.so` & `UComp-1.0.73/UComp/UCc.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `UComp-1.0.72/UComp/UCmodule.py` & `UComp-1.0.73/UComp/UCmodule.py`

 * *Files identical despite different names*

### Comparing `UComp-1.0.72/UComp/airpas.bin` & `UComp-1.0.73/UComp/airpas.bin`

 * *Files identical despite different names*

### Comparing `UComp-1.0.72/UComp/gdp.bin` & `UComp-1.0.73/UComp/gdp.bin`

 * *Files identical despite different names*

### Comparing `UComp-1.0.72/UComp/ipi.bin` & `UComp-1.0.73/UComp/ipi.bin`

 * *Files identical despite different names*

### Comparing `UComp-1.0.72/UComp/libopenblas.dll` & `UComp-1.0.73/UComp/libopenblas.dll`

 * *Files identical despite different names*

### Comparing `UComp-1.0.72/UComp/tools.py` & `UComp-1.0.73/UComp/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -597,19 +597,19 @@
     #     out[p, 2] = fi[p]
     #     fi[:p] = fi[:p] - fi[p] * np.flip(fi[:p])
     plotAcfPacf(out[:, 1], out[:, 2], s)
     out = pd.DataFrame(out, columns=["lag", "SACF", "SPACF"])
     return out
 
 
-def slide(y, orig, forecFun, *args, h=12, step=1, output=True, window=None, parallel=False):
+def slide(y, orig, forecFun, h=12, step=1, output=True, window=None, parallel=False, *args, **kwargs):
     """
     Rolling forecasting of a matrix of time series
     Inputs:
-        y: a vector or matrix of time series
+        y: a vector or a matrix of time series
         orig: starting forecasting origin
         forecFun: user function that implements forecasting methods
         *args: rest of inputs to forecFun function
         h: forecasting horizon
         step: observations ahead to move the forecasting origin
         output: output TRUE/FALSE
         window: fixed window width in number of observations (None for non-fixed)
@@ -617,30 +617,32 @@
     Returns:
         A vector with all the dimensions
 
     Author: Diego J. Pedregal
     """
     # Rolling for nSeries
     # out = [h, nOrigs, nModels, nSeries]
+    if isinstance(y, pd.Series) or isinstance(y, pd.DataFrame):
+        y = y.values
     if y.ndim == 1:
         y = y.reshape(-1, 1)
     nSeries = y.shape[1]
     n = y.shape[0]
     dataList = [y[:, j] for j in range(nSeries)]
     nOr = len(range(orig, n - h + 1, step))
     if not parallel or (nSeries == 1 and nOr == 1):
-        listOut = [slideAux(data, orig, forecFun, h, step, output, False, window, False, *args) for data in dataList]
+        listOut = [slideAux(data, orig, forecFun, h, step, output, False, window, False, *args, **kwargs) for data in dataList]
     else:
-        if nSeries > 1:
-            with mp.Pool() as pool:
-                listOut = pool.starmap(slideAux,
-                                       [(data, orig, forecFun, h, step, output, False, window, False, *args) for data in
-                                        dataList])
-        elif nOr > 1:
-            listOut = [slideAux(data, orig, forecFun, h, step, output, False, window, True, *args) for data in dataList]
+        # if nSeries > 1:
+        #     with mp.Pool() as pool:
+        #         listOut = pool.starmap(slideAux,
+        #                                [(data, orig, forecFun, h, step, output, False, window, False, *args, **kwargs) for data in
+        #                                 dataList])
+        # elif nOr > 1:
+        listOut = [slideAux(data, orig, forecFun, h, step, output, False, window, True, *args, **kwargs) for data in dataList]
     out = np.empty(listOut[0].shape + (nSeries,))
     for i in range(nSeries):
         out[:, :, :, i] = listOut[i]
     return out
 
 def slideAux(y, orig, forecFun, h=12, step=1, output=True, graph=True, window=None, parallel=False, *args, **kwargs):
     """
@@ -697,15 +699,15 @@
                 out[:, i, :] = np.reshape(np.array(listOut[i - 1]), (-1, 1))
             else:
                 out[:, i, :] = np.array(listOut[i - 1])
     if output:
         return out
 
 
-def plotSlide(py1, y, orig, step=1, errorFun=None, collectFun=np.mean):
+def plotSlide(py1, y, orig, step=1, errorFun=None, collectFun=np.mean, *args, **kwargs):
     """
     Plot summarised results from slide
     Inputs:
         py1 output from slide function
         y a vector or matrix of time series (the same used in slide call)
         orig starting forecasting origin (the same used in slide call)
         step observations ahead to move the forecasting origin (the same used in slide call)
@@ -723,28 +725,32 @@
     nSeries = py1.shape[3]
     if pd.isna(nSeries):
         nSeries = 1
         py = np.empty((h, nOrigs, nMethods, 1))
         py[:, :, :, 0] = py1
     else:
         py = py1
+    if isinstance(y, pd.Series) or isinstance(y, pd.DataFrame):
+        y = y.values
+    if y.ndim == 1:
+        y = y.reshape(-1, 1)
     # y = np.array(y)
     metrics = np.empty((h, nMethods))
     outj = np.empty((h, nOrigs, nMethods, nSeries))
     for i in range(nOrigs):
-        actuali = y[:orig + (i - 1) * step + h, :]
+        actuali = y[:orig + (i - 1) * step + h + 1, :]
         aux = py[:, i, :, :].copy()
         # aux = pd.DataFrame(aux, columns=np.arange(1, nMethods + 1))
         if nSeries == 1:
             for j in range(nMethods):
-                outj[:, i, j, 0] = errorFun(aux[:, j], actuali)
+                outj[:, i, j, 0] = errorFun(aux[:, j], actuali, *args, **kwargs)
         else:
             for k in range(nSeries):
                 for j in range(nMethods):
-                    outj[:, i, j, k] = errorFun(aux[:, j, k], actuali[:, k])
+                    outj[:, i, j, k] = errorFun(aux[:, j, k], actuali[:, k], *args, **kwargs)
     for m in range(nMethods):
         for j in range(h):
             metrics[j, m] = collectFun(outj[j, :, m])
     plotH = pd.DataFrame(metrics, index=np.arange(1, h + 1))
     plt.plot(plotH)
     plt.ylabel("Error metric")
     plt.show(block=False)
```

### Comparing `UComp-1.0.72/UComp/tsfile.py` & `UComp-1.0.73/UComp/tsfile.py`

 * *Files identical despite different names*

### Comparing `UComp-1.0.72/setup.py` & `UComp-1.0.73/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='UComp',
-    version='1.0.72',
+    version='1.0.73',
     author='Diego J. Pedregal',
     author_email='diego.pedregal@uclm.es',
     description='Modelling and forecasting univariate time series',
     long_description='Modelling and forecasting univariate time series',
     url='https://github.com/djpedregal/UComp',
     packages=find_packages(),
     include_package_data=True,
```

