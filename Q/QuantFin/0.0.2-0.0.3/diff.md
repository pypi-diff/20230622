# Comparing `tmp/QuantFin-0.0.2.tar.gz` & `tmp/QuantFin-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QuantFin-0.0.2.tar", last modified: Mon Jun 19 15:29:38 2023, max compression
+gzip compressed data, was "QuantFin-0.0.3.tar", last modified: Thu Jun 22 12:16:56 2023, max compression
```

## Comparing `QuantFin-0.0.2.tar` & `QuantFin-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 stephencheung   (501) staff       (20)        0 2023-06-19 15:29:38.468305 QuantFin-0.0.2/
--rwx------   0 stephencheung   (501) staff       (20)     1085 2023-01-27 14:04:52.000000 QuantFin-0.0.2/LICENSE
--rw-r--r--   0 stephencheung   (501) staff       (20)     4235 2023-06-19 15:29:38.469020 QuantFin-0.0.2/PKG-INFO
-drwxr-xr-x   0 stephencheung   (501) staff       (20)        0 2023-06-19 15:29:38.402779 QuantFin-0.0.2/QuantFin/
--rwx------   0 stephencheung   (501) staff       (20)      258 2023-06-19 08:40:48.000000 QuantFin-0.0.2/QuantFin/HandleError.py
--rwx------   0 stephencheung   (501) staff       (20)      911 2022-04-18 08:21:26.000000 QuantFin-0.0.2/QuantFin/MarketRisk.py
--rw-r--r--   0 stephencheung   (501) staff       (20)    13350 2023-06-19 15:09:08.000000 QuantFin-0.0.2/QuantFin/PanelRegs.py
--rwx------   0 stephencheung   (501) staff       (20)     8087 2023-06-19 15:11:23.000000 QuantFin-0.0.2/QuantFin/Portfolio.py
--rwx------   0 stephencheung   (501) staff       (20)     2835 2023-06-19 15:11:28.000000 QuantFin-0.0.2/QuantFin/Proxy.py
--rwx------   0 stephencheung   (501) staff       (20)    12285 2023-06-19 12:36:02.000000 QuantFin-0.0.2/QuantFin/ReqData.py
--rwx------   0 stephencheung   (501) staff       (20)      256 2023-06-19 15:09:41.000000 QuantFin-0.0.2/QuantFin/__init__.py
--rwx------   0 stephencheung   (501) staff       (20)     4274 2023-06-19 10:59:09.000000 QuantFin-0.0.2/QuantFin/_deciles.py
--rwx------   0 stephencheung   (501) staff       (20)     2303 2023-06-19 15:02:45.000000 QuantFin-0.0.2/QuantFin/_regression.py
--rwx------   0 stephencheung   (501) staff       (20)     4812 2023-06-19 10:56:38.000000 QuantFin-0.0.2/QuantFin/tool.py
-drwxr-xr-x   0 stephencheung   (501) staff       (20)        0 2023-06-19 15:29:38.467443 QuantFin-0.0.2/QuantFin.egg-info/
--rw-r--r--   0 stephencheung   (501) staff       (20)     4235 2023-06-19 15:29:37.000000 QuantFin-0.0.2/QuantFin.egg-info/PKG-INFO
--rw-r--r--   0 stephencheung   (501) staff       (20)      407 2023-06-19 15:29:38.000000 QuantFin-0.0.2/QuantFin.egg-info/SOURCES.txt
--rw-r--r--   0 stephencheung   (501) staff       (20)        1 2023-06-19 15:29:37.000000 QuantFin-0.0.2/QuantFin.egg-info/dependency_links.txt
--rw-r--r--   0 stephencheung   (501) staff       (20)       47 2023-06-19 15:29:37.000000 QuantFin-0.0.2/QuantFin.egg-info/requires.txt
--rw-r--r--   0 stephencheung   (501) staff       (20)        9 2023-06-19 15:29:37.000000 QuantFin-0.0.2/QuantFin.egg-info/top_level.txt
--rwx------   0 stephencheung   (501) staff       (20)     3418 2023-06-19 15:28:49.000000 QuantFin-0.0.2/README.md
--rw-r--r--   0 stephencheung   (501) staff       (20)       79 2023-06-19 15:29:38.472461 QuantFin-0.0.2/setup.cfg
--rwx------   0 stephencheung   (501) staff       (20)     1506 2023-06-19 15:28:14.000000 QuantFin-0.0.2/setup.py
+drwxr-xr-x   0 stephencheung   (501) staff       (20)        0 2023-06-22 12:16:56.417748 QuantFin-0.0.3/
+-rwx------   0 stephencheung   (501) staff       (20)     1085 2023-01-27 14:04:52.000000 QuantFin-0.0.3/LICENSE
+-rw-r--r--   0 stephencheung   (501) staff       (20)     4211 2023-06-22 12:16:56.418003 QuantFin-0.0.3/PKG-INFO
+drwxr-xr-x   0 stephencheung   (501) staff       (20)        0 2023-06-22 12:16:56.408053 QuantFin-0.0.3/QuantFin/
+-rwx------   0 stephencheung   (501) staff       (20)      258 2023-06-19 08:40:48.000000 QuantFin-0.0.3/QuantFin/HandleError.py
+-rwx------   0 stephencheung   (501) staff       (20)      911 2022-04-18 08:21:26.000000 QuantFin-0.0.3/QuantFin/MarketRisk.py
+-rw-r--r--   0 stephencheung   (501) staff       (20)    13350 2023-06-19 15:09:08.000000 QuantFin-0.0.3/QuantFin/PanelRegs.py
+-rwx------   0 stephencheung   (501) staff       (20)     8087 2023-06-19 15:11:23.000000 QuantFin-0.0.3/QuantFin/Portfolio.py
+-rwx------   0 stephencheung   (501) staff       (20)     2835 2023-06-19 15:11:28.000000 QuantFin-0.0.3/QuantFin/Proxy.py
+-rwx------   0 stephencheung   (501) staff       (20)    12285 2023-06-19 12:36:02.000000 QuantFin-0.0.3/QuantFin/ReqData.py
+-rwx------   0 stephencheung   (501) staff       (20)      256 2023-06-19 17:28:02.000000 QuantFin-0.0.3/QuantFin/__init__.py
+-rwx------   0 stephencheung   (501) staff       (20)     4274 2023-06-19 10:59:09.000000 QuantFin-0.0.3/QuantFin/_deciles.py
+-rwx------   0 stephencheung   (501) staff       (20)     2303 2023-06-19 15:02:45.000000 QuantFin-0.0.3/QuantFin/_regression.py
+-rwx------   0 stephencheung   (501) staff       (20)     4812 2023-06-22 11:51:05.000000 QuantFin-0.0.3/QuantFin/tool.py
+drwxr-xr-x   0 stephencheung   (501) staff       (20)        0 2023-06-22 12:16:56.417241 QuantFin-0.0.3/QuantFin.egg-info/
+-rw-r--r--   0 stephencheung   (501) staff       (20)     4211 2023-06-22 12:16:56.000000 QuantFin-0.0.3/QuantFin.egg-info/PKG-INFO
+-rw-r--r--   0 stephencheung   (501) staff       (20)      416 2023-06-22 12:16:56.000000 QuantFin-0.0.3/QuantFin.egg-info/SOURCES.txt
+-rw-r--r--   0 stephencheung   (501) staff       (20)        1 2023-06-22 12:16:56.000000 QuantFin-0.0.3/QuantFin.egg-info/dependency_links.txt
+-rw-r--r--   0 stephencheung   (501) staff       (20)       47 2023-06-22 12:16:56.000000 QuantFin-0.0.3/QuantFin.egg-info/requires.txt
+-rw-r--r--   0 stephencheung   (501) staff       (20)        9 2023-06-22 12:16:56.000000 QuantFin-0.0.3/QuantFin.egg-info/top_level.txt
+-rwx------   0 stephencheung   (501) staff       (20)     3394 2023-06-19 17:34:00.000000 QuantFin-0.0.3/README.md
+-rwx------   0 stephencheung   (501) staff       (20)     1506 2023-06-22 12:16:37.000000 QuantFin-0.0.3/SETUP.py
+-rw-r--r--   0 stephencheung   (501) staff       (20)       79 2023-06-22 12:16:56.418717 QuantFin-0.0.3/setup.cfg
```

### Comparing `QuantFin-0.0.2/LICENSE` & `QuantFin-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `QuantFin-0.0.2/PKG-INFO` & `QuantFin-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuantFin
-Version: 0.0.2
+Version: 0.0.3
 Summary: Library for Academic Research on Asset Pricing
 Home-page: https://github.com/yuz0101/QuantFin
 Download-URL: https://github.com/yuz0101/QuantFin/archive/refs/tags/Test.tar.gz
 Author: Stephen Zhang
 Author-email: stephen_se@outlook.com
 License: MIT
 Keywords: ACADEMIC,EMPIRICAL,FIANCE,RESEARCH,QUANT,PORTFOLIO
@@ -99,20 +99,20 @@
 ```
 
 ![Momentum Portfolios Returns](momRetsMean2.png)
 
 Run PanelOLS/Fama-MacBeth regressions and collect results:
 
 ```python
-from QuantFin.PanelRegs import multiregressions
+from QuantFin import multiregs
 
 formulas = {
     "Customised FixedEffects": "rets ~ 1 + mom', fe(permno year)",
     "Filter data": "rets ~ 1 + mom if date >= '2000-01-01', fe(permno year)",
     "Cluster Standard Errors": "rets ~ 1 + mom if date >= '2000-01-01', fe(permno year), cluster(permno)",
     "FamaMacbeth": "rets ~ 1 + mom if date >= '2000-01-01', famamacbeth, robust",
     "logFunct": "mom ~ 1 + log(marketCap) + bm + illiq + turnover, fe(permno date), cluster(permno)",
     "Interaction": "mom ~ 1 + log(marketCap)##bm + illiq +turnover, fe(permno date), cluster(date)" 
 }
 
-multiregressions(formulas, data=sample)
+multiregs(formulas, data=sample)
 ```
```

### Comparing `QuantFin-0.0.2/QuantFin/MarketRisk.py` & `QuantFin-0.0.3/QuantFin/MarketRisk.py`

 * *Files identical despite different names*

### Comparing `QuantFin-0.0.2/QuantFin/PanelRegs.py` & `QuantFin-0.0.3/QuantFin/PanelRegs.py`

 * *Files identical despite different names*

### Comparing `QuantFin-0.0.2/QuantFin/Portfolio.py` & `QuantFin-0.0.3/QuantFin/Portfolio.py`

 * *Files identical despite different names*

### Comparing `QuantFin-0.0.2/QuantFin/Proxy.py` & `QuantFin-0.0.3/QuantFin/Proxy.py`

 * *Files identical despite different names*

### Comparing `QuantFin-0.0.2/QuantFin/ReqData.py` & `QuantFin-0.0.3/QuantFin/ReqData.py`

 * *Files identical despite different names*

### Comparing `QuantFin-0.0.2/QuantFin/_deciles.py` & `QuantFin-0.0.3/QuantFin/_deciles.py`

 * *Files identical despite different names*

### Comparing `QuantFin-0.0.2/QuantFin/_regression.py` & `QuantFin-0.0.3/QuantFin/_regression.py`

 * *Files identical despite different names*

### Comparing `QuantFin-0.0.2/QuantFin/tool.py` & `QuantFin-0.0.3/QuantFin/tool.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,20 +58,20 @@
     -------
         a pandas Series object with the winsorized values of the specified variable. If a new label is
     provided, the Series is also renamed with the new label.
     
     '''
     if by:
         df = data[by+[var]].set_index(by)
-        df['u'] = data.groupby(by)[var].quantile(interval[0])
-        df['d'] = data.groupby(by)[var].quantile(interval[1])
+        df['u'] = data.groupby(by)[var].quantile(interval[1])
+        df['d'] = data.groupby(by)[var].quantile(interval[0])
     else:
         df = data[[var]]
-        df['u'] = data[var].quantile(interval[0])
-        df['d'] = data[var].quantile(interval[1])        
+        df['u'] = data[var].quantile(interval[1])
+        df['d'] = data[var].quantile(interval[0])        
     df.loc[df[var]>df['u'], var] = df.loc[df[var]>df['u'], 'u']
     df.loc[df[var]<df['d'], var] = df.loc[df[var]<df['d'], 'd']
     df.index = data.index
     df = df[var]
     if new_label:
         df = df.rename(new_label)
     return df
```

### Comparing `QuantFin-0.0.2/QuantFin.egg-info/PKG-INFO` & `QuantFin-0.0.3/QuantFin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuantFin
-Version: 0.0.2
+Version: 0.0.3
 Summary: Library for Academic Research on Asset Pricing
 Home-page: https://github.com/yuz0101/QuantFin
 Download-URL: https://github.com/yuz0101/QuantFin/archive/refs/tags/Test.tar.gz
 Author: Stephen Zhang
 Author-email: stephen_se@outlook.com
 License: MIT
 Keywords: ACADEMIC,EMPIRICAL,FIANCE,RESEARCH,QUANT,PORTFOLIO
@@ -99,20 +99,20 @@
 ```
 
 ![Momentum Portfolios Returns](momRetsMean2.png)
 
 Run PanelOLS/Fama-MacBeth regressions and collect results:
 
 ```python
-from QuantFin.PanelRegs import multiregressions
+from QuantFin import multiregs
 
 formulas = {
     "Customised FixedEffects": "rets ~ 1 + mom', fe(permno year)",
     "Filter data": "rets ~ 1 + mom if date >= '2000-01-01', fe(permno year)",
     "Cluster Standard Errors": "rets ~ 1 + mom if date >= '2000-01-01', fe(permno year), cluster(permno)",
     "FamaMacbeth": "rets ~ 1 + mom if date >= '2000-01-01', famamacbeth, robust",
     "logFunct": "mom ~ 1 + log(marketCap) + bm + illiq + turnover, fe(permno date), cluster(permno)",
     "Interaction": "mom ~ 1 + log(marketCap)##bm + illiq +turnover, fe(permno date), cluster(date)" 
 }
 
-multiregressions(formulas, data=sample)
+multiregs(formulas, data=sample)
 ```
```

### Comparing `QuantFin-0.0.2/README.md` & `QuantFin-0.0.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -78,20 +78,20 @@
 ```
 
 ![Momentum Portfolios Returns](momRetsMean2.png)
 
 Run PanelOLS/Fama-MacBeth regressions and collect results:
 
 ```python
-from QuantFin.PanelRegs import multiregressions
+from QuantFin import multiregs
 
 formulas = {
     "Customised FixedEffects": "rets ~ 1 + mom', fe(permno year)",
     "Filter data": "rets ~ 1 + mom if date >= '2000-01-01', fe(permno year)",
     "Cluster Standard Errors": "rets ~ 1 + mom if date >= '2000-01-01', fe(permno year), cluster(permno)",
     "FamaMacbeth": "rets ~ 1 + mom if date >= '2000-01-01', famamacbeth, robust",
     "logFunct": "mom ~ 1 + log(marketCap) + bm + illiq + turnover, fe(permno date), cluster(permno)",
     "Interaction": "mom ~ 1 + log(marketCap)##bm + illiq +turnover, fe(permno date), cluster(date)" 
 }
 
-multiregressions(formulas, data=sample)
+multiregs(formulas, data=sample)
 ```
```

### Comparing `QuantFin-0.0.2/setup.py` & `QuantFin-0.0.3/SETUP.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="QuantFin",
     packages=["QuantFin"],
-    version="0.0.2",
+    version="0.0.3",
     license="MIT",
     description="Library for Academic Research on Asset Pricing",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Stephen Zhang",
     author_email="stephen_se@outlook.com",
     url="https://github.com/yuz0101/QuantFin",
```

