# Comparing `tmp/omniplate-0.9.91.tar.gz` & `tmp/omniplate-0.9.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omniplate-0.9.91.tar", max compression
+gzip compressed data, was "omniplate-0.9.92.tar", max compression
```

## Comparing `omniplate-0.9.91.tar` & `omniplate-0.9.92.tar`

### file list

```diff
@@ -1,26 +1,25 @@
--rw-r--r--   0        0        0      244 2022-05-26 16:08:15.000000 omniplate-0.9.91/README.md
--rw-r--r--   0        0        0        0 2023-05-15 08:36:42.000000 omniplate-0.9.91/om_code/__init__.py
--rw-r--r--   0        0        0     2972 2023-05-09 11:28:17.000000 omniplate-0.9.91/om_code/admin.py
--rw-r--r--   0        0        0     1289 2023-04-24 14:56:03.907067 omniplate-0.9.91/om_code/clogger.py
--rw-r--r--   0        0        0    23910 2023-06-10 14:52:08.047214 omniplate-0.9.91/om_code/corrections.py
--rw-r--r--   0        0        0     1380 2023-01-30 16:21:38.087062 omniplate-0.9.91/om_code/dilution_data_lucia.tsv
--rw-r--r--   0        0        0     1893 2023-01-30 16:21:38.122549 omniplate-0.9.91/om_code/dilution_data_xiao.tsv
--rw-r--r--   0        0        0     7681 2023-06-10 14:52:08.058039 omniplate-0.9.91/om_code/getfitnesspenalty.py
--rw-r--r--   0        0        0     3470 2023-06-10 16:06:46.513087 omniplate-0.9.91/om_code/loaddata.py
--rw-r--r--   0        0        0     5187 2023-06-10 14:52:08.069421 omniplate-0.9.91/om_code/midlog.py
--rw-r--r--   0        0        0     2577 2023-05-26 11:17:09.866642 omniplate-0.9.91/om_code/old_analyseOldTecan.py
--rw-r--r--   0        0        0     1771 2023-05-26 11:17:09.866955 omniplate-0.9.91/om_code/old_analyseSunrise.py
--rw-r--r--   0        0        0     2609 2023-05-26 11:17:09.867263 omniplate-0.9.91/om_code/old_analyseTecan.py
--rw-r--r--   0        0        0      435 2022-05-26 16:08:15.000000 omniplate-0.9.91/om_code/omerrors.py
--rw-r--r--   0        0        0    11866 2023-06-10 14:52:08.126153 omniplate-0.9.91/om_code/omfitderiv.py
--rw-r--r--   0        0        0     3925 2023-06-10 14:52:08.317129 omniplate-0.9.91/om_code/omgenutils.py
--rw-r--r--   0        0        0    11514 2023-05-09 11:28:17.000000 omniplate-0.9.91/om_code/omplot.py
--rw-r--r--   0        0        0     6781 2023-06-10 14:52:08.375378 omniplate-0.9.91/om_code/omstats.py
--rw-r--r--   0        0        0     4211 2023-06-10 16:06:35.568372 omniplate-0.9.91/om_code/parseplate.py
--rw-r--r--   0        0        0     6068 2023-06-10 14:52:08.481613 omniplate-0.9.91/om_code/runfitderiv.py
--rw-r--r--   0        0        0     6211 2023-05-16 09:18:38.727419 omniplate-0.9.91/om_code/sunder.py
--rw-r--r--   0        0        0    93615 2023-06-10 16:11:05.939987 omniplate-0.9.91/omniplate/Omniplate.py
--rw-r--r--   0        0        0       44 2022-05-26 16:08:15.000000 omniplate-0.9.91/omniplate/__init__.py
--rw-r--r--   0        0        0     1116 2023-06-10 16:11:20.579802 omniplate-0.9.91/pyproject.toml
--rw-r--r--   0        0        0     1147 1970-01-01 00:00:00.000000 omniplate-0.9.91/setup.py
--rw-r--r--   0        0        0     1532 1970-01-01 00:00:00.000000 omniplate-0.9.91/PKG-INFO
+-rw-r--r--   0        0        0      244 2022-05-26 16:08:15.786293 omniplate-0.9.92/README.md
+-rw-r--r--   0        0        0        0 2023-05-15 08:36:42.000000 omniplate-0.9.92/om_code/__init__.py
+-rw-r--r--   0        0        0     3383 2023-06-21 10:39:14.000000 omniplate-0.9.92/om_code/admin.py
+-rw-r--r--   0        0        0     1289 2023-04-24 14:56:03.000000 omniplate-0.9.92/om_code/clogger.py
+-rw-r--r--   0        0        0    24576 2023-06-21 10:49:59.000000 omniplate-0.9.92/om_code/corrections.py
+-rw-r--r--   0        0        0     1380 2023-01-30 16:21:38.000000 omniplate-0.9.92/om_code/dilution_data_lucia.tsv
+-rw-r--r--   0        0        0     1893 2023-01-30 16:21:38.000000 omniplate-0.9.92/om_code/dilution_data_xiao.tsv
+-rw-r--r--   0        0        0     7681 2023-06-10 14:52:08.000000 omniplate-0.9.92/om_code/getfitnesspenalty.py
+-rw-r--r--   0        0        0     3470 2023-06-10 16:06:46.000000 omniplate-0.9.92/om_code/loaddata.py
+-rw-r--r--   0        0        0     5187 2023-06-10 14:52:08.000000 omniplate-0.9.92/om_code/midlog.py
+-rw-r--r--   0        0        0     2577 2023-05-26 11:17:09.000000 omniplate-0.9.92/om_code/old_analyseOldTecan.py
+-rw-r--r--   0        0        0     1771 2023-05-26 11:17:09.000000 omniplate-0.9.92/om_code/old_analyseSunrise.py
+-rw-r--r--   0        0        0     2609 2023-05-26 11:17:09.000000 omniplate-0.9.92/om_code/old_analyseTecan.py
+-rw-r--r--   0        0        0      435 2022-05-26 16:08:15.904220 omniplate-0.9.92/om_code/omerrors.py
+-rw-r--r--   0        0        0    11860 2023-06-20 18:31:25.138985 omniplate-0.9.92/om_code/omfitderiv.py
+-rw-r--r--   0        0        0     3925 2023-06-10 14:52:08.000000 omniplate-0.9.92/om_code/omgenutils.py
+-rw-r--r--   0        0        0    11471 2023-06-20 17:42:50.408709 omniplate-0.9.92/om_code/omplot.py
+-rw-r--r--   0        0        0     6794 2023-06-21 13:56:46.000000 omniplate-0.9.92/om_code/omstats.py
+-rw-r--r--   0        0        0     4211 2023-06-10 16:06:35.000000 omniplate-0.9.92/om_code/parseplate.py
+-rw-r--r--   0        0        0     6068 2023-06-10 14:52:08.000000 omniplate-0.9.92/om_code/runfitderiv.py
+-rw-r--r--   0        0        0     4597 2023-06-22 15:26:16.248601 omniplate-0.9.92/om_code/sunder.py
+-rw-r--r--   0        0        0    93755 2023-06-22 13:02:45.132194 omniplate-0.9.92/omniplate/Omniplate.py
+-rw-r--r--   0        0        0       44 2022-05-26 16:08:15.902667 omniplate-0.9.92/omniplate/__init__.py
+-rw-r--r--   0        0        0     1118 2023-06-22 14:16:05.982462 omniplate-0.9.92/pyproject.toml
+-rw-r--r--   0        0        0     1501 1970-01-01 00:00:00.000000 omniplate-0.9.92/PKG-INFO
```

### Comparing `omniplate-0.9.91/om_code/admin.py` & `omniplate-0.9.92/om_code/admin.py`

 * *Files 7% similar despite different names*

```diff
@@ -98,7 +98,17 @@
     else:
         # update sc dataframe
         self.sc = gu.absorbdf(
             self.sc,
             statsdf,
             ["experiment", "condition", "strain"],
         )
+
+
+def check_kwargs(kwargs):
+    """Stop if final s missing from experiments, conditions, or strains."""
+    if "condition" in kwargs:
+        raise SystemExit("Use conditions not condition as an argument.")
+    elif "strain" in kwargs:
+        raise SystemExit("Use strains not strain as an argument.")
+    elif "experiment" in kwargs:
+        raise SystemExit("Use experiments not experiment as an argument.")
```

### Comparing `omniplate-0.9.91/om_code/clogger.py` & `omniplate-0.9.92/om_code/clogger.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.91/om_code/corrections.py` & `omniplate-0.9.92/om_code/corrections.py`

 * *Files 1% similar despite different names*

```diff
@@ -407,26 +407,26 @@
         self, experiments, experimentincludes, experimentexcludes, "experiment"
     ):
         for c in sunder.getset(
             self,
             conditions,
             conditionincludes,
             conditionexcludes,
-            "condition",
+            labeltype="condition",
             nomedia=True,
         ):
             # process reference strain
             refqrfn = processref2(self, f, refstrain, figs, e, c)
             # process other strains
             for s in sunder.getset(
                 self,
                 strains,
                 strainincludes,
                 strainexcludes,
-                "strain",
+                labeltype="strain",
                 nonull=True,
             ):
                 if s != refstrain:
                     fl_0, fl_1, od = sunder.extractwells(
                         self.r, self.s, e, c, s, f.copy() + ["OD"]
                     )
                     if fl_0.size == 0 or fl_1.size == 0:
@@ -684,30 +684,43 @@
             f"\nYou first must run getstats for {s} in {c} for {e}."
         )
     # initialise GP for log ODs
     go = instantiateGP(hypers, cvfn, t, np.log(od))
     # run GP for log fluorescence
     fitvar = f"log_{flname}"
     derivname = f"d/dt_{fitvar}"
-    ff, _ = runfitderiv(
-        self,
-        t,
-        fl,
-        fitvar,
-        derivname,
-        e,
-        c,
-        s,
-        bd=bd,
-        cvfn=flcvfn,
-        logs=True,
-        figs=figs,
-        **kwargs,
-    )
-    if not ff.success:
-        print(f"\n-> Fitting fluorescence failed for {e}: {s} in {c}.\n")
-        return np.nan * np.ones(fl.shape)
-    # sample
-    lod_samples = go.sample(nosamples)
-    lfl_samples = ff.fitderivsample(nosamples)[0]
-    flperod = np.exp(lfl_samples - lod_samples)
+    # find rows with data not all NaNs
+    i_data = np.where(~np.isnan(fl))[0]
+    if np.any(i_data):
+        # all rows are not NaN
+        min_tpt = np.min(i_data)
+        max_tpt = np.max(i_data)
+        # only run GP between time points with data
+        ff, _ = runfitderiv(
+            self,
+            t[min_tpt:max_tpt],
+            fl[min_tpt:max_tpt, :],
+            fitvar,
+            derivname,
+            e,
+            c,
+            s,
+            bd=bd,
+            cvfn=flcvfn,
+            logs=True,
+            figs=figs,
+            **kwargs,
+        )
+        if not ff.success:
+            print(f"\n-> Fitting fluorescence failed for {e}: {s} in {c}.\n")
+            return np.nan * np.ones(fl.shape)
+        # sample
+        lod_samples = go.sample(nosamples)
+        lfl_samples = ff.fitderivsample(nosamples)[0]
+        flperod_samples = np.exp(lfl_samples - lod_samples[min_tpt:max_tpt, :])
+        # insert into or replace matrix of NaNs
+        flperod = np.nan * np.ones((t.size, nosamples))
+        flperod[min_tpt:max_tpt, :] = flperod_samples
+    else:
+        # all NaN
+        flperod = np.nan * np.ones((t.size, nosamples))
     return flperod
```

### Comparing `omniplate-0.9.91/om_code/dilution_data_lucia.tsv` & `omniplate-0.9.92/om_code/dilution_data_lucia.tsv`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.91/om_code/dilution_data_xiao.tsv` & `omniplate-0.9.92/om_code/dilution_data_xiao.tsv`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.91/om_code/getfitnesspenalty.py` & `omniplate-0.9.92/om_code/getfitnesspenalty.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.91/om_code/loaddata.py` & `omniplate-0.9.92/om_code/loaddata.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.91/om_code/midlog.py` & `omniplate-0.9.92/om_code/midlog.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.91/om_code/old_analyseOldTecan.py` & `omniplate-0.9.92/om_code/old_analyseOldTecan.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.91/om_code/old_analyseSunrise.py` & `omniplate-0.9.92/om_code/old_analyseSunrise.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.91/om_code/old_analyseTecan.py` & `omniplate-0.9.92/om_code/old_analyseTecan.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.91/om_code/omfitderiv.py` & `omniplate-0.9.92/om_code/omfitderiv.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,20 +198,20 @@
             )
         else:
             keep = np.nonzero(~np.isnan(db))[0]
         # remove any NaNs
         da = db[keep]
         ta = tb[keep]
         # check data remains after removing NaNs
-        if not np.any(da):
+        if not da.size:
             print("Warning: omfitderiv failed - too many NaNs.")
             self.success = False
         elif np.any(merrors):
             ma = mb[keep]
-            if not np.any(ma):
+            if not ma.size:
                 print("Warning: omfitderiv failed - too many NaNs.")
                 self.success = False
         else:
             ma = None
         if self.success:
             self.run(
                 cvfn,
```

### Comparing `omniplate-0.9.91/om_code/omgenutils.py` & `omniplate-0.9.92/om_code/omgenutils.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.91/om_code/omplot.py` & `omniplate-0.9.92/om_code/omplot.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,14 @@
                             sfig.fig.suptitle(title)
                         else:
                             sfig.fig.suptitle(e + ": " + s + " in " + c)
                         if xlim is not None:
                             plt.xlim(xlim)
                         if ylim is not None:
                             plt.ylim(ylim)
-                        plt.tight_layout()
                         plt.show(block=False)
 
 
 def plot_rs(
     x,
     y,
     basedf,
```

### Comparing `omniplate-0.9.91/om_code/omstats.py` & `omniplate-0.9.92/om_code/omstats.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,19 +45,18 @@
     statistic calculated from time series sampled from the optimal Gaussian
     process.
 
     Its error is estimated as the interquartile range of this
     distribution.
     """
     # check derivative has been sensibly defined
-    if (
-        np.max(np.abs(f.df)) < 1.0e-20
-        and np.max(np.abs(np.diff(f.dfvar))) < 1.0e-20
+    if np.max(np.abs(f.df)) < 1.0e-20 and (
+        f.dfvar.size > 1 and np.max(np.abs(np.diff(f.dfvar))) < 1.0e-20
     ):
-        warning = f"\nWarning: getstats may have failed for {e}: {s} in {c}."
+        warning = f"\nWarning: fitderiv may have failed for {e}: {s} in {c}."
     else:
         warning = None
     # time-series for s dataframe
     df_for_s = pd.DataFrame(
         {
             "experiment": e,
             "condition": c,
```

### Comparing `omniplate-0.9.91/om_code/parseplate.py` & `omniplate-0.9.92/om_code/parseplate.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.91/om_code/runfitderiv.py` & `omniplate-0.9.92/om_code/runfitderiv.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.91/omniplate/Omniplate.py` & `omniplate-0.9.92/omniplate/Omniplate.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import om_code.omgenutils as gu
 import om_code.omplot as omplot
 import om_code.sunder as sunder
 import pandas as pd
 import seaborn as sns
 from om_code.runfitderiv import runfitderiv
 
-version = "0.9.91"
+version = "0.9.92"
 
 plt.rcParams["figure.max_open_warning"] = 0
 sns.set()
 
 
 class platereader:
     """
@@ -1359,14 +1359,15 @@
         ...        hue= 'strain')
         >>> p.plot(y= 'c-mCherryperOD', conditions= ['0.5% Mal',
         ...        '1% Mal'], hue= 'strain', style= 'condition',
         ...         nonull= True, strainincludes= 'mCherry')
         >>> p.plot(y= 'c-GFPperOD', col= 'experiment')
         >>> p.plot(y= 'max gr')
         """
+        admin.check_kwargs(kwargs)
         # choose the correct dataframe
         basedf, dfname = omplot.plotfinddf(self, x, y)
         # get experiments, conditions and strains
         exps, cons, strs = sunder.getall(
             self,
             experiments,
             experimentincludes,
@@ -1962,14 +1963,15 @@
 
         References
         ----------
         PS Swain, K Stevenson, A Leary, LF Montano-Gutierrez, IB Clark,
         J Vogel, T Pilizota. (2016). Inferring time derivatives including cell
         growth rates using Gaussian processes. Nat Commun, 7, 1-8.
         """
+        admin.check_kwargs(kwargs)
         linalgmax = 5
         warnings = ""
         # variable to be fit
         if logs:
             fitvar = f"log_{dtype}"
         else:
             fitvar = dtype
@@ -2025,15 +2027,15 @@
                     else:
                         print(f"\n-> {dtype} not recognised for {esc_name}.\n")
                         return
                     # checks
                     if d.size == 0:
                         # no data
                         print(
-                            f"\n-> No data found for {dtype} for {esc_name}.\m"
+                            f"\n-> No data found for {dtype} for {esc_name}.\n"
                         )
                         continue
                     # run fit
                     _, warning = runfitderiv(
                         self,
                         t,
                         d,
@@ -2286,14 +2288,15 @@
 
         I Mihalcescu, MVM Gateau, B Chelli, C Pinel, JL Ravanat (2015).
         Green autofluorescence, a double edged monitoring tool for bacterial
         growth and activity in micro-plates.
         Phys Biol, 12, 066016.
 
         """
+        admin.check_kwargs(kwargs)
         f = gu.makelist(f)
         exps, cons, _ = sunder.getall(
             self,
             experiments,
             experimentincludes,
             experimentexcludes,
             conditions,
@@ -2612,14 +2615,15 @@
         strainincludes: string, optional
             Selects only strains that include the specified string in their
             name.
         strainexcludes: string, optional
             Ignores strains that include the specified string in their name.
         kwargs: passed to Nunchaku
         """
+        admin.check_kwargs(kwargs)
         exps, cons, strs = sunder.getall(
             self,
             experiments,
             experimentincludes,
             experimentexcludes,
             conditions,
             conditionincludes,
```

### Comparing `omniplate-0.9.91/pyproject.toml` & `omniplate-0.9.92/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "omniplate"
-version = "0.9.91"
+version = "0.9.92"
 description = "For analysing and meta-analysing plate-reader data"
 authors = ["Peter Swain <peter.swain@ed.ac.uk>"]
 
 license = "MIT"
 readme = "README.md"
 homepage = "https://swainlab.bio.ed.ac.uk/software/omniplate"
 repository = "https://git.ecdf.ed.ac.uk/pswain/omniplate"
@@ -19,22 +19,22 @@
     { include = "omniplate" },
     { include = "om_code" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
 pandas = ">=1.5.1"
-numpy = "^1.24.3"
-scipy = "^1.10.1"
-matplotlib = "^3.7.1"
-seaborn = ">=0.11.2"
+numpy = ">=1.24.3"
+scipy = ">=1.10.1"
+matplotlib = ">=3.7.1"
+seaborn = ">=0.12"
 statsmodels = ">=0.13.1"
 openpyxl = ">=3.0.9"
 gaussianprocessderivatives = ">=0.1.64"
-nunchaku = "^0.11.0"
+nunchaku = ">=0.12.0"
 
 [tool.black]
 line-length = 79
 
 [tool.poetry.dev-dependencies]
```

### Comparing `omniplate-0.9.91/PKG-INFO` & `omniplate-0.9.92/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omniplate
-Version: 0.9.91
+Version: 0.9.92
 Summary: For analysing and meta-analysing plate-reader data
 Home-page: https://swainlab.bio.ed.ac.uk/software/omniplate
 License: MIT
 Keywords: omniplate,systems biology,bioinformatics,plate readers
 Author: Peter Swain
 Author-email: peter.swain@ed.ac.uk
 Requires-Python: >=3.8,<3.11
@@ -13,21 +13,21 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Dist: gaussianprocessderivatives (>=0.1.64)
-Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
-Requires-Dist: numpy (>=1.24.3,<2.0.0)
-Requires-Dist: nunchaku (>=0.11.0,<0.12.0)
+Requires-Dist: matplotlib (>=3.7.1)
+Requires-Dist: numpy (>=1.24.3)
+Requires-Dist: nunchaku (>=0.12.0)
 Requires-Dist: openpyxl (>=3.0.9)
 Requires-Dist: pandas (>=1.5.1)
-Requires-Dist: scipy (>=1.10.1,<2.0.0)
-Requires-Dist: seaborn (>=0.11.2)
+Requires-Dist: scipy (>=1.10.1)
+Requires-Dist: seaborn (>=0.12)
 Requires-Dist: statsmodels (>=0.13.1)
 Project-URL: Documentation, https://swainlab.bio.ed.ac.uk/software/omniplate
 Project-URL: Repository, https://git.ecdf.ed.ac.uk/pswain/omniplate
 Description-Content-Type: text/markdown
 
 A Python package for analysing data from plate-reader studies of growing biological cells. Users can correct for autofluorescence, determine growth rates and the amount of fluorescence per cell, and simultaneously analyse multiple experiments.
```

