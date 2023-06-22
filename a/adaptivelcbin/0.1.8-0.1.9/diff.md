# Comparing `tmp/adaptivelcbin-0.1.8.tar.gz` & `tmp/adaptivelcbin-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adaptivelcbin-0.1.8.tar", last modified: Tue May 10 10:55:03 2022, max compression
+gzip compressed data, was "adaptivelcbin-0.1.9.tar", last modified: Thu Aug 25 12:49:56 2022, max compression
```

## Comparing `adaptivelcbin-0.1.8.tar` & `adaptivelcbin-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 ferrigno  (1000) ferrigno  (1000)        0 2022-05-10 10:55:03.164472 adaptivelcbin-0.1.8/
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)     1071 2021-03-11 14:33:46.000000 adaptivelcbin-0.1.8/LICENSE
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)     1438 2022-05-10 10:55:03.164472 adaptivelcbin-0.1.8/PKG-INFO
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)      633 2021-03-11 14:33:46.000000 adaptivelcbin-0.1.8/README.md
-drwxrwxr-x   0 ferrigno  (1000) ferrigno  (1000)        0 2022-05-10 10:55:03.164472 adaptivelcbin-0.1.8/adaptivelcbin.egg-info/
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)     1438 2022-05-10 10:55:03.000000 adaptivelcbin-0.1.8/adaptivelcbin.egg-info/PKG-INFO
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)      279 2022-05-10 10:55:03.000000 adaptivelcbin-0.1.8/adaptivelcbin.egg-info/SOURCES.txt
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)        1 2022-05-10 10:55:03.000000 adaptivelcbin-0.1.8/adaptivelcbin.egg-info/dependency_links.txt
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)       42 2022-05-10 10:55:03.000000 adaptivelcbin-0.1.8/adaptivelcbin.egg-info/entry_points.txt
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)       20 2022-05-10 10:55:03.000000 adaptivelcbin-0.1.8/adaptivelcbin.egg-info/requires.txt
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)        7 2022-05-10 10:55:03.000000 adaptivelcbin-0.1.8/adaptivelcbin.egg-info/top_level.txt
-drwxrwxr-x   0 ferrigno  (1000) ferrigno  (1000)        0 2022-05-10 10:55:03.164472 adaptivelcbin-0.1.8/hratio/
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)    28459 2022-05-10 10:53:12.000000 adaptivelcbin-0.1.8/hratio/__init__.py
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)     1298 2022-05-10 10:55:03.164472 adaptivelcbin-0.1.8/setup.cfg
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)      359 2022-05-10 10:39:04.000000 adaptivelcbin-0.1.8/setup.py
+drwxrwxr-x   0 ferrigno  (1000) ferrigno  (1000)        0 2022-08-25 12:49:56.981594 adaptivelcbin-0.1.9/
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)     1071 2021-03-11 14:33:46.000000 adaptivelcbin-0.1.9/LICENSE
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)     1438 2022-08-25 12:49:56.981594 adaptivelcbin-0.1.9/PKG-INFO
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)      633 2021-03-11 14:33:46.000000 adaptivelcbin-0.1.9/README.md
+drwxrwxr-x   0 ferrigno  (1000) ferrigno  (1000)        0 2022-08-25 12:49:56.981594 adaptivelcbin-0.1.9/adaptivelcbin.egg-info/
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)     1438 2022-08-25 12:49:56.000000 adaptivelcbin-0.1.9/adaptivelcbin.egg-info/PKG-INFO
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)      279 2022-08-25 12:49:56.000000 adaptivelcbin-0.1.9/adaptivelcbin.egg-info/SOURCES.txt
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)        1 2022-08-25 12:49:56.000000 adaptivelcbin-0.1.9/adaptivelcbin.egg-info/dependency_links.txt
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)       42 2022-08-25 12:49:56.000000 adaptivelcbin-0.1.9/adaptivelcbin.egg-info/entry_points.txt
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)       20 2022-08-25 12:49:56.000000 adaptivelcbin-0.1.9/adaptivelcbin.egg-info/requires.txt
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)        7 2022-08-25 12:49:56.000000 adaptivelcbin-0.1.9/adaptivelcbin.egg-info/top_level.txt
+drwxrwxr-x   0 ferrigno  (1000) ferrigno  (1000)        0 2022-08-25 12:49:56.981594 adaptivelcbin-0.1.9/hratio/
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)    28452 2022-08-25 12:09:06.000000 adaptivelcbin-0.1.9/hratio/__init__.py
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)     1298 2022-08-25 12:49:56.981594 adaptivelcbin-0.1.9/setup.cfg
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)      359 2022-08-25 12:09:31.000000 adaptivelcbin-0.1.9/setup.py
```

### Comparing `adaptivelcbin-0.1.8/LICENSE` & `adaptivelcbin-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adaptivelcbin-0.1.8/PKG-INFO` & `adaptivelcbin-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adaptivelcbin
-Version: 0.1.8
+Version: 0.1.9
 Summary: adaptivelcbin
 Home-page: https://gitlab.astro.unige.ch/ferrigno/adaptivelcbin
 Author: C.F.
 Author-email: carlo.ferrigno@unige.ch
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `adaptivelcbin-0.1.8/README.md` & `adaptivelcbin-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `adaptivelcbin-0.1.8/adaptivelcbin.egg-info/PKG-INFO` & `adaptivelcbin-0.1.9/adaptivelcbin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adaptivelcbin
-Version: 0.1.8
+Version: 0.1.9
 Summary: adaptivelcbin
 Home-page: https://gitlab.astro.unige.ch/ferrigno/adaptivelcbin
 Author: C.F.
 Author-email: carlo.ferrigno@unige.ch
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `adaptivelcbin-0.1.8/hratio/__init__.py` & `adaptivelcbin-0.1.9/hratio/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,16 +114,16 @@
         try:
             self._dtimes_ = ff[data_ind].data['XAX_E']
         except:
             logger.info("Initializing delta_times from TIMEDEL")
             self._dtimes_ = np.ones(len(self._times_)) * self._timedel_
 
         if self._gti_header_ is not None:
-            self._gti_start_ = self._gti_header_.data['START']
-            self._gti_stop_ = self._gti_header_.data['STOP']
+            self._gti_start_ = ff[gti_ind].data['START']
+            self._gti_stop_ = ff[gti_ind].data['STOP']
         else:
             logger.warning('No GTI, using data start and stop')
             self._gti_start_ = np.array([self._tstart_])
             self._gti_stop_ = np.array([self._tstop_])
 
         ff.close()
         self.dump_info()
@@ -625,16 +625,16 @@
         self._times_ = np.array(new_x)
         self._dtimes_ = np.array(new_dx)
         self._rates_ = np.array(new_y) / self._dtimes_
         self._drates_ = np.array(new_dy) / self._dtimes_
         self._frac_exp_ = new_frac_exp
 
 
-def hratio_func(soft_lcname, hard_lcname, hratio_fname, min_sn: float, max_time=1e4, gti_threshold=100, flag_rebin=1, min_bin_size=0,
-           ext_t0=-1, max_point_sn=100, single_point_check=False):
+def hratio_func(soft_lcname, hard_lcname, hratio_fname, min_sn: float, max_time=1e4, gti_threshold=100, flag_rebin=1,
+                min_bin_size=0, ext_t0=-1, max_point_sn=100, single_point_check=False):
 
     logger.info("Soft LC " + soft_lcname)
     logger.info("Hard LC " + hard_lcname)
 
     if hratio_fname is not None:
         logger.info("Hardness ratio output file " + hratio_fname)
     else:
```

### Comparing `adaptivelcbin-0.1.8/setup.cfg` & `adaptivelcbin-0.1.9/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.6
+current_version = 0.1.9
 commit = True
 tag = False
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\-(?P<release>[a-z]+)(?P<build>\d+))?
 serialize = 
 	{major}.{minor}.{patch}-{release}{build}
 	{major}.{minor}.{patch}
```

