# Comparing `tmp/cfr-0.6.4.tar.gz` & `tmp/cfr-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfr-0.6.4.tar", last modified: Wed Jun 21 18:27:14 2023, max compression
+gzip compressed data, was "cfr-0.6.5.tar", last modified: Thu Jun 22 18:48:40 2023, max compression
```

## Comparing `cfr-0.6.4.tar` & `cfr-0.6.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-21 18:27:14.261764 cfr-0.6.4/
--rw-r--r--   0 fengzhu    (502) staff       (20)     1516 2022-04-27 05:34:15.000000 cfr-0.6.4/LICENSE
--rw-r--r--   0 fengzhu    (502) staff       (20)     1770 2023-06-21 18:27:14.261573 cfr-0.6.4/PKG-INFO
--rw-r--r--   0 fengzhu    (502) staff       (20)     1207 2023-05-29 21:16:00.000000 cfr-0.6.4/README.md
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-21 18:27:14.252684 cfr-0.6.4/bin/
--rw-r--r--   0 fengzhu    (502) staff       (20)     5163 2023-06-19 02:34:42.000000 cfr-0.6.4/bin/cfr
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-21 18:27:14.257291 cfr-0.6.4/cfr/
--rw-r--r--   0 fengzhu    (502) staff       (20)      732 2023-06-21 18:25:21.000000 cfr-0.6.4/cfr/__init__.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    22467 2023-05-29 23:34:35.000000 cfr-0.6.4/cfr/climate.py
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-21 18:27:14.261235 cfr-0.6.4/cfr/da/
--rw-r--r--   0 fengzhu    (502) staff       (20)       22 2022-07-02 05:30:36.000000 cfr-0.6.4/cfr/da/__init__.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    16319 2023-03-27 02:39:30.000000 cfr-0.6.4/cfr/da/enkf.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    22484 2023-04-17 19:25:37.000000 cfr-0.6.4/cfr/gcm.py
--rw-r--r--   0 fengzhu    (502) staff       (20)     7623 2022-05-05 04:13:16.000000 cfr-0.6.4/cfr/ml.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    64854 2023-06-21 18:25:07.000000 cfr-0.6.4/cfr/proxy.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    45058 2023-06-20 03:51:38.000000 cfr-0.6.4/cfr/psm.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    54926 2023-06-19 02:39:39.000000 cfr-0.6.4/cfr/reconjob.py
--rw-r--r--   0 fengzhu    (502) staff       (20)     2311 2023-03-27 02:39:30.000000 cfr-0.6.4/cfr/reconres.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    19837 2023-05-29 21:16:00.000000 cfr-0.6.4/cfr/ts.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    26722 2023-06-20 23:08:04.000000 cfr-0.6.4/cfr/utils.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    54810 2023-04-17 19:25:37.000000 cfr-0.6.4/cfr/visual.py
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-21 18:27:14.260478 cfr-0.6.4/cfr.egg-info/
--rw-r--r--   0 fengzhu    (502) staff       (20)     1770 2023-06-21 18:27:14.000000 cfr-0.6.4/cfr.egg-info/PKG-INFO
--rw-r--r--   0 fengzhu    (502) staff       (20)      373 2023-06-21 18:27:14.000000 cfr-0.6.4/cfr.egg-info/SOURCES.txt
--rw-r--r--   0 fengzhu    (502) staff       (20)        1 2023-06-21 18:27:14.000000 cfr-0.6.4/cfr.egg-info/dependency_links.txt
--rw-r--r--   0 fengzhu    (502) staff       (20)        1 2022-04-28 04:59:29.000000 cfr-0.6.4/cfr.egg-info/not-zip-safe
--rw-r--r--   0 fengzhu    (502) staff       (20)      203 2023-06-21 18:27:14.000000 cfr-0.6.4/cfr.egg-info/requires.txt
--rw-r--r--   0 fengzhu    (502) staff       (20)        4 2023-06-21 18:27:14.000000 cfr-0.6.4/cfr.egg-info/top_level.txt
--rw-r--r--   0 fengzhu    (502) staff       (20)       38 2023-06-21 18:27:14.261824 cfr-0.6.4/setup.cfg
--rw-r--r--   0 fengzhu    (502) staff       (20)     1413 2023-06-21 18:25:41.000000 cfr-0.6.4/setup.py
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-22 18:48:40.101587 cfr-0.6.5/
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1516 2022-04-27 05:34:15.000000 cfr-0.6.5/LICENSE
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1770 2023-06-22 18:48:40.101391 cfr-0.6.5/PKG-INFO
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1207 2023-05-29 21:16:00.000000 cfr-0.6.5/README.md
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-22 18:48:40.090044 cfr-0.6.5/bin/
+-rw-r--r--   0 fengzhu    (502) staff       (20)     5163 2023-06-19 02:34:42.000000 cfr-0.6.5/bin/cfr
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-22 18:48:40.097023 cfr-0.6.5/cfr/
+-rw-r--r--   0 fengzhu    (502) staff       (20)      732 2023-06-21 18:25:21.000000 cfr-0.6.5/cfr/__init__.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    22467 2023-05-29 23:34:35.000000 cfr-0.6.5/cfr/climate.py
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-22 18:48:40.100884 cfr-0.6.5/cfr/da/
+-rw-r--r--   0 fengzhu    (502) staff       (20)       22 2022-07-02 05:30:36.000000 cfr-0.6.5/cfr/da/__init__.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    16319 2023-03-27 02:39:30.000000 cfr-0.6.5/cfr/da/enkf.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    22484 2023-04-17 19:25:37.000000 cfr-0.6.5/cfr/gcm.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)     7623 2022-05-05 04:13:16.000000 cfr-0.6.5/cfr/ml.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    67033 2023-06-22 17:29:40.000000 cfr-0.6.5/cfr/proxy.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    45058 2023-06-20 03:51:38.000000 cfr-0.6.5/cfr/psm.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    54926 2023-06-21 23:52:13.000000 cfr-0.6.5/cfr/reconjob.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)     2311 2023-03-27 02:39:30.000000 cfr-0.6.5/cfr/reconres.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    19837 2023-05-29 21:16:00.000000 cfr-0.6.5/cfr/ts.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    26722 2023-06-20 23:08:04.000000 cfr-0.6.5/cfr/utils.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    54810 2023-04-17 19:25:37.000000 cfr-0.6.5/cfr/visual.py
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-22 18:48:40.100005 cfr-0.6.5/cfr.egg-info/
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1770 2023-06-22 18:48:40.000000 cfr-0.6.5/cfr.egg-info/PKG-INFO
+-rw-r--r--   0 fengzhu    (502) staff       (20)      373 2023-06-22 18:48:40.000000 cfr-0.6.5/cfr.egg-info/SOURCES.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)        1 2023-06-22 18:48:40.000000 cfr-0.6.5/cfr.egg-info/dependency_links.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)        1 2022-04-28 04:59:29.000000 cfr-0.6.5/cfr.egg-info/not-zip-safe
+-rw-r--r--   0 fengzhu    (502) staff       (20)      203 2023-06-22 18:48:40.000000 cfr-0.6.5/cfr.egg-info/requires.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)        4 2023-06-22 18:48:40.000000 cfr-0.6.5/cfr.egg-info/top_level.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)       38 2023-06-22 18:48:40.101715 cfr-0.6.5/setup.cfg
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1413 2023-06-22 18:47:12.000000 cfr-0.6.5/setup.py
```

### Comparing `cfr-0.6.4/LICENSE` & `cfr-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cfr-0.6.4/PKG-INFO` & `cfr-0.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfr
-Version: 0.6.4
+Version: 0.6.5
 Summary: cfr: a Python package for Climate Field Reconstruction
 Home-page: https://github.com/fzhu2e/cfr
 Author: Feng Zhu, Julien Emile-Geay
 Author-email: fengzhu@ucar.edu, julieneg@usc.edu
 License: BSD 3-Clause
 Keywords: climate field reconstruction
 Classifier: Natural Language :: English
```

### Comparing `cfr-0.6.4/README.md` & `cfr-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `cfr-0.6.4/bin/cfr` & `cfr-0.6.5/bin/cfr`

 * *Files identical despite different names*

### Comparing `cfr-0.6.4/cfr/__init__.py` & `cfr-0.6.5/cfr/__init__.py`

 * *Files identical despite different names*

### Comparing `cfr-0.6.4/cfr/climate.py` & `cfr-0.6.5/cfr/climate.py`

 * *Files identical despite different names*

### Comparing `cfr-0.6.4/cfr/da/enkf.py` & `cfr-0.6.5/cfr/da/enkf.py`

 * *Files identical despite different names*

### Comparing `cfr-0.6.4/cfr/gcm.py` & `cfr-0.6.5/cfr/gcm.py`

 * *Files identical despite different names*

### Comparing `cfr-0.6.4/cfr/ml.py` & `cfr-0.6.5/cfr/ml.py`

 * *Files identical despite different names*

### Comparing `cfr-0.6.4/cfr/proxy.py` & `cfr-0.6.5/cfr/proxy.py`

 * *Files 3% similar despite different names*

```diff
@@ -168,25 +168,14 @@
         self.time_unit = 'yr' if time_unit is None else time_unit
         self.seasonality = seasonality
 
     def copy(self):
         ''' Make a deepcopy of the object. '''
         return copy.deepcopy(self)
 
-    def center(self, ref_period):
-        ''' Centering the proxy timeseries regarding a reference period.
-
-        Args:
-            ref_period (tuple or list): the reference time period in the form or (start_yr, end_yr)
-        '''
-        new = self.copy()
-        ref = self.slice(ref_period)
-        new.value -= np.nanmean(ref.value)
-        return new
-
     def slice(self, timespan):
         ''' Slicing the timeseries with a timespan (tuple or list)
 
         Args:
             timespan (tuple or list):
                 The list of time points for slicing, whose length must be even.
                 When there are n time points, the output Series includes n/2 segments.
@@ -298,30 +287,90 @@
         try:
             new.time, new.value = utils.annualize(self.time, self.value, months=months)
             new.tags.add('annualized')
         except:
             if force:
                 new.time, new.value = utils.annualize(self.time, self.value, months=list(range(1, 13)))
                 new.tags.add('annualized')
-                print(new.tags)
                 if verbose: p_warning(f'Record {self.pid} cannot be annualized with months {months}. Use calendar year instead.')
             else:
                 if verbose: p_warning(f'Record {self.pid} cannot be annualized with months {months}. The record is untouched.')
 
         new.time, new.value = utils.clean_ts(new.time, new.value)
         new.dt = np.median(np.diff(new.time))
         return new
             
+    def center(self, ref_period=None, thresh=5, force=False, verbose=False):
+        ''' Centering the proxy timeseries regarding a reference period.
+
+        Args:
+            ref_period (tuple or list): the reference time period in the form or (start_yr, end_yr)
+        '''
+        def center_func(new, ref):
+            new.value -= np.nanmean(ref.value)
+            new.tags.add('centered')
+            return new
+            
+        if ref_period is not None:
+            ref = self.slice(ref_period)
+        else:
+            ref = self
 
-    def standardize(self):
         new = self.copy()
-        if self.value.std() == 0:
-            new.value = np.zeros(np.size(self.value))
+        if len(ref.time) < thresh:
+            if force:
+                ref = self
+                new = center_func(new, ref)
+                if verbose: p_warning(f'The overlapping with the given reference period is too short. Reference over the full record instead.')
+            else:
+                if verbose: p_warning(f'The record is untouched due to short overlapping with the reference period.')
         else:
-            new.value = (self.value - np.nanmean(self.value)) / np.nanstd(self.value)
+            new = center_func(new, ref)
+
+        return new
+
+    def standardize(self, ref_period=None, thresh=5, force=False, verbose=False):
+        '''
+        Standardizes the record. If the record is constant, a vector of 0s is returned.
+
+        Parameters
+        ----------
+        ref_period : list, optional
+            [min_time, max_time]. The default is None.
+
+        Returns
+        -------
+        new : ProxyRecord
+            contains standardized values.
+        '''
+        def std_func(new, ref):
+            z = (new.value - np.nanmean(ref.value)) / np.nanstd(ref.value)
+            if np.isfinite(z.all()) and ~np.isnan(z.all()):
+                new.value = z
+                new.tags.add('standardized')
+            else:
+                if verbose: p_warning('Standardization failed; the record is untouched.')
+
+            return new
+            
+        if ref_period is not None:
+            ref = self.slice(ref_period)
+        else:
+            ref = self
+
+        new = self.copy()
+        if len(ref.time) < thresh:
+            if force:
+                ref = self
+                new = std_func(new, ref)
+            else:
+                if verbose: p_warning(f'The record is untouched due to short overlapping with the reference period.')
+        else:
+            new = std_func(new, ref)
+
         return new
 
     def __getitem__(self, key):
         ''' This makes the object subscriptable. '''
         new = self.copy()
         if type(key) is int or type(key) is list:
             new.value = new.value[key]
@@ -863,55 +912,53 @@
 
         return new
 
     def copy(self):
         ''' Make a deepcopy of the object. '''
         return copy.deepcopy(self)
 
-    def center(self, ref_period):
+    def center(self, ref_period, force=False, thresh=5, verbose=False):
         ''' Center the proxy timeseries against a reference time period.
 
         Args:
         ----    
             ref_period (tuple or list): the reference time period in the form or (start_yr, end_yr)
             
         Returns
         -------
         new : cfr.ProxyDatabase object
         
         '''
-        new = self.copy()
+        new = ProxyDatabase()
         for pid, pobj in tqdm(self.records.items(), total=self.nrec, desc='Centering each of the ProxyRecord'):
-            ref = pobj.slice(ref_period)
-            if np.size(ref.time) == 0:
-                new -= pobj
-            else:
-                new.records[pid].value -= np.nanmean(ref.value)
+            spobj = pobj.center(ref_period=ref_period, force=force, thresh=thresh, verbose=False)
+            new += spobj
 
+        new = new.filter(by='tag', keys=['centered'])
+        if verbose and not force: p_warning(f'{self.nrec - new.nrec} records have been dropped as they cannot be properly centered with the reference period.')
         return new
     
-    def standardize(self, ref_period):
+    def standardize(self, ref_period, force=False, thresh=5, verbose=False):
         ''' Standardize elements of a proxy database against a reference time period.
             Elements that have no values over the reference period are dropped 
 
         Args:
             ref_period (tuple or list): the reference time period in the form or (start_yr, end_yr)
             
         Returns
         -------
         new : cfr.ProxyDatabase object
         '''
-        new = self.copy()
+        new = ProxyDatabase()
         for pid, pobj in tqdm(self.records.items(), total=self.nrec, desc='Standardizing each of the ProxyRecords'):
-            ref = pobj.slice(ref_period)
-            if len(ref.time) < 5:
-                new -= pobj
-            else:
-                new.records[pid].value = (pobj.value - np.nanmean(ref.value)) / np.nanstd(ref.value)
+            spobj = pobj.standardize(ref_period=ref_period, force=force, thresh=thresh, verbose=False)
+            new += spobj
 
+        new = new.filter(by='tag', keys=['standardized'])
+        if verbose and not force: p_warning(f'{self.nrec - new.nrec} records have been dropped as they cannot be properly standardized with the reference period.')
         return new
 
     def refresh(self):
         ''' Refresh a bunch of attributes. '''
         self.nrec = len(self.records)
         self.pids = [pobj.pid for pid, pobj in self.records.items()]
         self.lats = [pobj.lat for pid, pobj in self.records.items()]
@@ -1447,19 +1494,19 @@
         else:
             return ax
 
     def annualize(self, months=list(range(1, 13)), force=False, verbose=False):
         ''' Annualize the records in the proxy database.'''
         new = ProxyDatabase()
         for pid, pobj in tqdm(self.records.items(), total=self.nrec, desc='Annualizing ProxyDatabase'):
-            spobj = pobj.annualize(months=months, force=force, verbose=verbose)
+            spobj = pobj.annualize(months=months, force=force, verbose=False)
             new += spobj
 
         new = new.filter(by='tag', keys=['annualized'])
-        new.refresh()
+        if verbose and not force: p_warning(f'{self.nrec - new.nrec} records have been dropped as they cannot be properly annualized with the given months.')
         return new
 
     def slice(self, timespan):
         ''' Slice the records in the proxy database.'''
         new = ProxyDatabase()
         for pid, pobj in tqdm(self.records.items(), total=self.nrec, desc='Slicing ProxyRecord'):
             spobj = pobj.slice(timespan=timespan)
```

### Comparing `cfr-0.6.4/cfr/psm.py` & `cfr-0.6.5/cfr/psm.py`

 * *Files identical despite different names*

### Comparing `cfr-0.6.4/cfr/reconjob.py` & `cfr-0.6.5/cfr/reconjob.py`

 * *Files identical despite different names*

### Comparing `cfr-0.6.4/cfr/reconres.py` & `cfr-0.6.5/cfr/reconres.py`

 * *Files identical despite different names*

### Comparing `cfr-0.6.4/cfr/ts.py` & `cfr-0.6.5/cfr/ts.py`

 * *Files identical despite different names*

### Comparing `cfr-0.6.4/cfr/utils.py` & `cfr-0.6.5/cfr/utils.py`

 * *Files identical despite different names*

### Comparing `cfr-0.6.4/cfr/visual.py` & `cfr-0.6.5/cfr/visual.py`

 * *Files identical despite different names*

### Comparing `cfr-0.6.4/cfr.egg-info/PKG-INFO` & `cfr-0.6.5/cfr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfr
-Version: 0.6.4
+Version: 0.6.5
 Summary: cfr: a Python package for Climate Field Reconstruction
 Home-page: https://github.com/fzhu2e/cfr
 Author: Feng Zhu, Julien Emile-Geay
 Author-email: fengzhu@ucar.edu, julieneg@usc.edu
 License: BSD 3-Clause
 Keywords: climate field reconstruction
 Classifier: Natural Language :: English
```

### Comparing `cfr-0.6.4/setup.py` & `cfr-0.6.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='cfr',  # required
-    version='0.6.4',
+    version='0.6.5',
     description='cfr: a Python package for Climate Field Reconstruction',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     author='Feng Zhu, Julien Emile-Geay',
     author_email='fengzhu@ucar.edu, julieneg@usc.edu',
     url='https://github.com/fzhu2e/cfr',
     packages=find_packages(),
```

