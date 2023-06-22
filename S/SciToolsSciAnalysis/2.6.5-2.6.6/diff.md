# Comparing `tmp/SciToolsSciAnalysis-2.6.5.tar.gz` & `tmp/SciToolsSciAnalysis-2.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SciToolsSciAnalysis-2.6.5.tar", last modified: Fri Jan 27 18:40:45 2023, max compression
+gzip compressed data, was "SciToolsSciAnalysis-2.6.6.tar", last modified: Thu Jun 22 16:45:37 2023, max compression
```

## Comparing `SciToolsSciAnalysis-2.6.5.tar` & `SciToolsSciAnalysis-2.6.6.tar`

### file list

```diff
@@ -1,33 +1,37 @@
-drwxrwxr-x   0 kyager   (23681) kyager   (23681)        0 2023-01-27 18:40:45.961290 SciToolsSciAnalysis-2.6.5/
--rw-rw-r--   0 kyager   (23681) kyager   (23681)     2850 2023-01-27 18:40:45.961290 SciToolsSciAnalysis-2.6.5/PKG-INFO
--rw-rw-r--   0 kyager   (23681) kyager   (23681)     2007 2023-01-27 16:05:34.000000 SciToolsSciAnalysis-2.6.5/README.md
-drwxrwxr-x   0 kyager   (23681) kyager   (23681)        0 2023-01-27 18:40:45.961290 SciToolsSciAnalysis-2.6.5/SciAnalysis/
--rw-r--r--   0 kyager   (23681) kyager   (23681)    11309 2022-09-26 17:32:36.000000 SciToolsSciAnalysis-2.6.5/SciAnalysis/Base.py
--rw-r--r--   0 kyager   (23681) kyager   (23681)    97821 2022-09-26 17:28:26.000000 SciToolsSciAnalysis-2.6.5/SciAnalysis/Data.py
--rw-r--r--   0 kyager   (23681) kyager   (23681)      783 2015-11-07 23:30:50.000000 SciToolsSciAnalysis-2.6.5/SciAnalysis/Fit.py
--rw-r--r--   0 kyager   (23681) kyager   (23681)    12055 2020-02-12 19:32:05.000000 SciToolsSciAnalysis-2.6.5/SciAnalysis/IO_HDF.py
--rw-r--r--   0 kyager   (23681) kyager   (23681)    15446 2021-07-27 02:38:38.000000 SciToolsSciAnalysis-2.6.5/SciAnalysis/Result.py
-drwxrwxr-x   0 kyager   (23681) kyager   (23681)        0 2023-01-27 18:40:45.961290 SciToolsSciAnalysis-2.6.5/SciAnalysis/XSAnalysis/
--rw-rw-r--   0 kyager   (23681) kyager   (23681)    64418 2022-09-26 18:08:17.000000 SciToolsSciAnalysis-2.6.5/SciAnalysis/XSAnalysis/Data.py
--rw-r--r--   0 kyager   (23681) kyager   (23681)     4246 2019-04-15 17:32:47.000000 SciToolsSciAnalysis-2.6.5/SciAnalysis/XSAnalysis/DataGonio.py
--rw-rw-r--   0 kyager   (23681) kyager   (23681)     3409 2019-12-17 19:57:24.000000 SciToolsSciAnalysis-2.6.5/SciAnalysis/XSAnalysis/DataQ.py
--rw-r--r--   0 kyager   (23681) kyager   (23681)    15893 2019-04-15 17:07:38.000000 SciToolsSciAnalysis-2.6.5/SciAnalysis/XSAnalysis/DataRQconv.py
--rw-r--r--   0 kyager   (23681) kyager   (23681)     5689 2016-02-23 16:33:05.000000 SciToolsSciAnalysis-2.6.5/SciAnalysis/XSAnalysis/Eiger-alternate.py
--rw-r--r--   0 kyager   (23681) kyager   (23681)     6072 2016-02-23 15:22:44.000000 SciToolsSciAnalysis-2.6.5/SciAnalysis/XSAnalysis/Eiger.py
--rw-rw-r--   0 kyager   (23681) kyager   (23681)    23104 2020-08-14 14:29:58.000000 SciToolsSciAnalysis-2.6.5/SciAnalysis/XSAnalysis/Multiple.py
--rw-rw-r--   0 kyager   (23681) kyager   (23681)   151995 2023-01-27 16:05:34.000000 SciToolsSciAnalysis-2.6.5/SciAnalysis/XSAnalysis/Protocols.py
--rw-r--r--   0 kyager   (23681) kyager   (23681)      683 2023-01-27 16:09:04.000000 SciToolsSciAnalysis-2.6.5/SciAnalysis/XSAnalysis/__init__.py
--rw-rw-r--   0 kyager   (23681) kyager   (23681)      776 2023-01-27 16:09:15.000000 SciToolsSciAnalysis-2.6.5/SciAnalysis/__init__.py
--rw-rw-r--   0 kyager   (23681) kyager   (23681)      497 2023-01-27 18:40:45.961290 SciToolsSciAnalysis-2.6.5/SciAnalysis/_version.py
--rw-rw-r--   0 kyager   (23681) kyager   (23681)    50899 2019-05-10 18:10:04.000000 SciToolsSciAnalysis-2.6.5/SciAnalysis/colormaps.py
--rw-r--r--   0 kyager   (23681) kyager   (23681)      571 2022-09-26 17:27:28.000000 SciToolsSciAnalysis-2.6.5/SciAnalysis/settings.py
--rw-rw-r--   0 kyager   (23681) kyager   (23681)    43536 2022-09-26 18:04:58.000000 SciToolsSciAnalysis-2.6.5/SciAnalysis/tools.py
-drwxrwxr-x   0 kyager   (23681) kyager   (23681)        0 2023-01-27 18:40:45.961290 SciToolsSciAnalysis-2.6.5/SciToolsSciAnalysis.egg-info/
--rw-rw-r--   0 kyager   (23681) kyager   (23681)     2850 2023-01-27 18:40:45.000000 SciToolsSciAnalysis-2.6.5/SciToolsSciAnalysis.egg-info/PKG-INFO
--rw-rw-r--   0 kyager   (23681) kyager   (23681)      825 2023-01-27 18:40:45.000000 SciToolsSciAnalysis-2.6.5/SciToolsSciAnalysis.egg-info/SOURCES.txt
--rw-rw-r--   0 kyager   (23681) kyager   (23681)        1 2023-01-27 18:40:45.000000 SciToolsSciAnalysis-2.6.5/SciToolsSciAnalysis.egg-info/dependency_links.txt
--rw-rw-r--   0 kyager   (23681) kyager   (23681)       20 2023-01-27 18:40:45.000000 SciToolsSciAnalysis-2.6.5/SciToolsSciAnalysis.egg-info/entry_points.txt
--rw-rw-r--   0 kyager   (23681) kyager   (23681)       23 2023-01-27 18:40:45.000000 SciToolsSciAnalysis-2.6.5/SciToolsSciAnalysis.egg-info/requires.txt
--rw-rw-r--   0 kyager   (23681) kyager   (23681)       12 2023-01-27 18:40:45.000000 SciToolsSciAnalysis-2.6.5/SciToolsSciAnalysis.egg-info/top_level.txt
--rw-rw-r--   0 kyager   (23681) kyager   (23681)      186 2023-01-27 18:40:45.961290 SciToolsSciAnalysis-2.6.5/setup.cfg
--rw-rw-r--   0 kyager   (23681) kyager   (23681)     2237 2023-01-27 18:39:20.000000 SciToolsSciAnalysis-2.6.5/setup.py
+drwxrwxr-x   0 kyager   (23681) kyager   (23681)        0 2023-06-22 16:45:37.180022 SciToolsSciAnalysis-2.6.6/
+-rw-rw-r--   0 kyager   (23681) kyager   (23681)     3440 2022-09-26 17:07:34.000000 SciToolsSciAnalysis-2.6.6/LICENSE
+-rw-rw-r--   0 kyager   (23681) kyager   (23681)      262 2023-06-22 16:40:42.000000 SciToolsSciAnalysis-2.6.6/MANIFEST.in
+-rw-rw-r--   0 kyager   (23681) kyager   (23681)     2886 2023-06-22 16:45:37.180022 SciToolsSciAnalysis-2.6.6/PKG-INFO
+-rw-rw-r--   0 kyager   (23681) kyager   (23681)     2021 2023-06-22 16:40:42.000000 SciToolsSciAnalysis-2.6.6/README.md
+drwxrwxr-x   0 kyager   (23681) kyager   (23681)        0 2023-06-22 16:45:37.180022 SciToolsSciAnalysis-2.6.6/SciAnalysis/
+-rw-r--r--   0 kyager   (23681) kyager   (23681)    11309 2022-09-26 17:32:36.000000 SciToolsSciAnalysis-2.6.6/SciAnalysis/Base.py
+-rw-rw-r--   0 kyager   (23681) kyager   (23681)    97826 2023-06-22 16:40:42.000000 SciToolsSciAnalysis-2.6.6/SciAnalysis/Data.py
+-rw-r--r--   0 kyager   (23681) kyager   (23681)      783 2015-11-07 23:30:50.000000 SciToolsSciAnalysis-2.6.6/SciAnalysis/Fit.py
+-rw-r--r--   0 kyager   (23681) kyager   (23681)    12055 2020-02-12 19:32:05.000000 SciToolsSciAnalysis-2.6.6/SciAnalysis/IO_HDF.py
+-rw-rw-r--   0 kyager   (23681) kyager   (23681)    15469 2023-06-22 16:40:42.000000 SciToolsSciAnalysis-2.6.6/SciAnalysis/Result.py
+drwxrwxr-x   0 kyager   (23681) kyager   (23681)        0 2023-06-22 16:45:37.180022 SciToolsSciAnalysis-2.6.6/SciAnalysis/XSAnalysis/
+-rw-rw-r--   0 kyager   (23681) kyager   (23681)    64418 2022-09-26 18:08:17.000000 SciToolsSciAnalysis-2.6.6/SciAnalysis/XSAnalysis/Data.py
+-rw-r--r--   0 kyager   (23681) kyager   (23681)     4246 2019-04-15 17:32:47.000000 SciToolsSciAnalysis-2.6.6/SciAnalysis/XSAnalysis/DataGonio.py
+-rw-rw-r--   0 kyager   (23681) kyager   (23681)     3409 2019-12-17 19:57:24.000000 SciToolsSciAnalysis-2.6.6/SciAnalysis/XSAnalysis/DataQ.py
+-rw-r--r--   0 kyager   (23681) kyager   (23681)    15893 2019-04-15 17:07:38.000000 SciToolsSciAnalysis-2.6.6/SciAnalysis/XSAnalysis/DataRQconv.py
+-rw-r--r--   0 kyager   (23681) kyager   (23681)     5689 2016-02-23 16:33:05.000000 SciToolsSciAnalysis-2.6.6/SciAnalysis/XSAnalysis/Eiger-alternate.py
+-rw-r--r--   0 kyager   (23681) kyager   (23681)     6072 2016-02-23 15:22:44.000000 SciToolsSciAnalysis-2.6.6/SciAnalysis/XSAnalysis/Eiger.py
+-rw-rw-r--   0 kyager   (23681) kyager   (23681)    23104 2020-08-14 14:29:58.000000 SciToolsSciAnalysis-2.6.6/SciAnalysis/XSAnalysis/Multiple.py
+-rw-rw-r--   0 kyager   (23681) kyager   (23681)   152957 2023-06-22 16:40:42.000000 SciToolsSciAnalysis-2.6.6/SciAnalysis/XSAnalysis/Protocols.py
+-rw-r--r--   0 kyager   (23681) kyager   (23681)      683 2023-01-27 16:09:04.000000 SciToolsSciAnalysis-2.6.6/SciAnalysis/XSAnalysis/__init__.py
+-rw-rw-r--   0 kyager   (23681) kyager   (23681)      776 2023-01-27 16:09:15.000000 SciToolsSciAnalysis-2.6.6/SciAnalysis/__init__.py
+-rw-rw-r--   0 kyager   (23681) kyager   (23681)      497 2023-06-22 16:45:37.180022 SciToolsSciAnalysis-2.6.6/SciAnalysis/_version.py
+-rw-rw-r--   0 kyager   (23681) kyager   (23681)    50899 2019-05-10 18:10:04.000000 SciToolsSciAnalysis-2.6.6/SciAnalysis/colormaps.py
+-rw-rw-r--   0 kyager   (23681) kyager   (23681)      571 2023-06-22 16:40:42.000000 SciToolsSciAnalysis-2.6.6/SciAnalysis/settings.py
+-rw-rw-r--   0 kyager   (23681) kyager   (23681)    43536 2022-09-26 18:04:58.000000 SciToolsSciAnalysis-2.6.6/SciAnalysis/tools.py
+drwxrwxr-x   0 kyager   (23681) kyager   (23681)        0 2023-06-22 16:45:37.180022 SciToolsSciAnalysis-2.6.6/SciToolsSciAnalysis.egg-info/
+-rw-rw-r--   0 kyager   (23681) kyager   (23681)     2886 2023-06-22 16:45:37.000000 SciToolsSciAnalysis-2.6.6/SciToolsSciAnalysis.egg-info/PKG-INFO
+-rw-rw-r--   0 kyager   (23681) kyager   (23681)      876 2023-06-22 16:45:37.000000 SciToolsSciAnalysis-2.6.6/SciToolsSciAnalysis.egg-info/SOURCES.txt
+-rw-rw-r--   0 kyager   (23681) kyager   (23681)        1 2023-06-22 16:45:37.000000 SciToolsSciAnalysis-2.6.6/SciToolsSciAnalysis.egg-info/dependency_links.txt
+-rw-rw-r--   0 kyager   (23681) kyager   (23681)       20 2023-06-22 16:45:37.000000 SciToolsSciAnalysis-2.6.6/SciToolsSciAnalysis.egg-info/entry_points.txt
+-rw-rw-r--   0 kyager   (23681) kyager   (23681)       23 2023-06-22 16:45:37.000000 SciToolsSciAnalysis-2.6.6/SciToolsSciAnalysis.egg-info/requires.txt
+-rw-rw-r--   0 kyager   (23681) kyager   (23681)       12 2023-06-22 16:45:37.000000 SciToolsSciAnalysis-2.6.6/SciToolsSciAnalysis.egg-info/top_level.txt
+-rw-rw-r--   0 kyager   (23681) kyager   (23681)       23 2023-01-27 16:05:34.000000 SciToolsSciAnalysis-2.6.6/requirements.txt
+-rw-rw-r--   0 kyager   (23681) kyager   (23681)      186 2023-06-22 16:45:37.180022 SciToolsSciAnalysis-2.6.6/setup.cfg
+-rw-rw-r--   0 kyager   (23681) kyager   (23681)     2235 2023-06-22 16:40:42.000000 SciToolsSciAnalysis-2.6.6/setup.py
+-rw-rw-r--   0 kyager   (23681) kyager   (23681)    68713 2023-01-27 16:05:34.000000 SciToolsSciAnalysis-2.6.6/versioneer.py
```

### Comparing `SciToolsSciAnalysis-2.6.5/PKG-INFO` & `SciToolsSciAnalysis-2.6.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: SciToolsSciAnalysis
-Version: 2.6.5
+Version: 2.6.6
 Summary: SciAnalysis scripts for processing image files.
-Home-page: https://github.com//CFN-softbio//SciAnalysis
+Home-page: https://github.com/CFN-softbio/SciAnalysis
 Author: Kevin Yager
 Author-email: kyager@bnl.gov
 License: BSD (3-clause)
 Description: # SciAnalysis
         
         ## Author : Kevin G. Yager
         ## Ported to git by : Julien Lhermitte
@@ -33,16 +33,19 @@
          * Protocols.linecut_qr(qz=0.025, dq=0.02, ylog=True, show_region=True, gridlines=True); #dq is half-width
          * Protocols.linecut_qz(name='linecut_qz_new', ylog=True, qr=0, dq=0.02, show_region=True, plot_range=[0.2, 0.4, None, None])
          * Protocols.linecut_qz_fit(qr=0.0, dq=0.01, show_region=True, label_filename=True, trim_range=[0.01, 0.4], fit_range=[0.093, 0.115], plot_range=[0.01, 0.4, 0, None], q0=[0.11]) 
          * Protocols.circular_average_q2I_fit(plot_range=[0.8, 1.3, 0, None], qn_power=0.0, trim_range=[0.1, 3.5], fit_range=[0.95, 1.4], num_curves=2, q0=[1.00, 1.2], sigma=0.02, show_curves=1, label_filename=True), 
          * Protocols.sector_average(angle=70, dangle=10, plot_range=[1.2, 3.7, 0, 1200], show_region=True) #pie-shaped
          * Protocols.roi(show_region=True, qx=1, dqx=0.02, qz=1, dqz=0.02, prepend='stats_')
         
+        
         run_args = { 'verbosity' : 3,
-                    #'save_results' : ['xml', 'plots', 'txt', 'hdf5'],
+        
+                    'save_results' : ['xml', 'plots', 'txt', 'hdf5'],
+                    
                     'rcParams': {'axes.labelsize': 25,
                                     'xtick.labelsize': 20,
                                     'ytick.labelsize': 20,
                                     'xtick.major.pad': 10,
                                     'ytick.major.pad': 10,
                                     },
                     }
```

### Comparing `SciToolsSciAnalysis-2.6.5/README.md` & `SciToolsSciAnalysis-2.6.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -25,16 +25,19 @@
  * Protocols.linecut_qr(qz=0.025, dq=0.02, ylog=True, show_region=True, gridlines=True); #dq is half-width
  * Protocols.linecut_qz(name='linecut_qz_new', ylog=True, qr=0, dq=0.02, show_region=True, plot_range=[0.2, 0.4, None, None])
  * Protocols.linecut_qz_fit(qr=0.0, dq=0.01, show_region=True, label_filename=True, trim_range=[0.01, 0.4], fit_range=[0.093, 0.115], plot_range=[0.01, 0.4, 0, None], q0=[0.11]) 
  * Protocols.circular_average_q2I_fit(plot_range=[0.8, 1.3, 0, None], qn_power=0.0, trim_range=[0.1, 3.5], fit_range=[0.95, 1.4], num_curves=2, q0=[1.00, 1.2], sigma=0.02, show_curves=1, label_filename=True), 
  * Protocols.sector_average(angle=70, dangle=10, plot_range=[1.2, 3.7, 0, 1200], show_region=True) #pie-shaped
  * Protocols.roi(show_region=True, qx=1, dqx=0.02, qz=1, dqz=0.02, prepend='stats_')
 
+
 run_args = { 'verbosity' : 3,
-            #'save_results' : ['xml', 'plots', 'txt', 'hdf5'],
+
+            'save_results' : ['xml', 'plots', 'txt', 'hdf5'],
+            
             'rcParams': {'axes.labelsize': 25,
                             'xtick.labelsize': 20,
                             'ytick.labelsize': 20,
                             'xtick.major.pad': 10,
                             'ytick.major.pad': 10,
                             },
             }
```

### Comparing `SciToolsSciAnalysis-2.6.5/SciAnalysis/Base.py` & `SciToolsSciAnalysis-2.6.6/SciAnalysis/Base.py`

 * *Files identical despite different names*

### Comparing `SciToolsSciAnalysis-2.6.5/SciAnalysis/Data.py` & `SciToolsSciAnalysis-2.6.6/SciAnalysis/Data.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,24 +155,24 @@
     def save_data(self, outfile):
         
         if self.x_err is None and self.y_err is None:
             data = np.dstack([self.x, self.y])[0]
             header = '%s %s' % (self.x_label, self.y_label)
         
         elif self.y_err is None:
-            data = np.dstack([self.x, self.x_err, self.y])[0]
-            header = '%s %serr %s' % (self.x_label, self.x_label, self.y_label)
+            data = np.dstack([self.x, self.y, self.x_err])[0]
+            header = '%s %serr %s' % (self.x_label, self.y_label, self.x_label )
             
         elif self.x_err is None:
             data = np.dstack([self.x, self.y, self.y_err])[0]
             header = '%s %s %serr' % (self.x_label, self.y_label, self.y_label)
             
         else:
-            data = np.dstack([self.x, self.x_err, self.y, self.y_err])[0]
-            header = '%s %serr %s %serr' % (self.x_label, self.x_label, self.y_label, self.y_label)
+            data = np.dstack([self.x, self.y, self.x_err, self.y_err])[0]
+            header = '%s %serr %s %serr' % (self.x_label, self.y_label, self.x_label, self.y_label)
         
         np.savetxt( outfile, data, header=header )
     
     
     # Data access
     ########################################
     def get_x_spacing(self, mode='avg'):
@@ -515,17 +515,17 @@
     
                    
     # Plot interaction
     ########################################
     
     def _plot_interact(self):
         
-        self.fig.canvas.set_window_title('SciAnalysis')
+        #self.fig.canvas.set_window_title('SciAnalysis')
         #plt.get_current_fig_manager().toolbar.pan()
-        self.fig.canvas.toolbar.pan()
+        #self.fig.canvas.toolbar.pan()
         self.fig.canvas.mpl_connect('scroll_event', self._scroll_event )
         #self.fig.canvas.mpl_connect('motion_notify_event', self._move_event )
         #self.fig.canvas.mpl_connect('key_press_event', self._key_press_event)
         
         #self.ax.format_coord = self._format_coord       
         
         
@@ -2169,17 +2169,17 @@
         
         
     # Plot interaction
     ########################################
     
     def _plot_interact(self):
         
-        self.fig.canvas.set_window_title('SciAnalysis')
+        #self.fig.canvas.set_window_title('SciAnalysis')
         #plt.get_current_fig_manager().toolbar.pan()
-        self.fig.canvas.toolbar.pan()
+        #self.fig.canvas.toolbar.pan()
         self.fig.canvas.mpl_connect('scroll_event', self._scroll_event )
         #self.fig.canvas.mpl_connect('motion_notify_event', self._move_event )
         self.fig.canvas.mpl_connect('key_press_event', self._key_press_event)
         
         #self.ax.format_coord = self._format_coord_simple
         self.ax.format_coord = self._format_coord
```

### Comparing `SciToolsSciAnalysis-2.6.5/SciAnalysis/Fit.py` & `SciToolsSciAnalysis-2.6.6/SciAnalysis/Fit.py`

 * *Files identical despite different names*

### Comparing `SciToolsSciAnalysis-2.6.5/SciAnalysis/IO_HDF.py` & `SciToolsSciAnalysis-2.6.6/SciAnalysis/IO_HDF.py`

 * *Files identical despite different names*

### Comparing `SciToolsSciAnalysis-2.6.5/SciAnalysis/Result.py` & `SciToolsSciAnalysis-2.6.6/SciAnalysis/Result.py`

 * *Files 0% similar despite different names*

```diff
@@ -387,14 +387,15 @@
         
         sql = '''-- Retrieve list of files
         SELECT DISTINCT filename 
         FROM analyses
         WHERE filename like ? ESCAPE ? 
         ORDER BY filename
         '''
+        print(pattern)
         self.db_cursor.execute(sql, ( pattern, "\\", ))
         result_rows = self.db_cursor.fetchall()
         
         #for result_row in result_rows:
             #result_row = dict(result_row)
             #print(result_row)
```

### Comparing `SciToolsSciAnalysis-2.6.5/SciAnalysis/XSAnalysis/Data.py` & `SciToolsSciAnalysis-2.6.6/SciAnalysis/XSAnalysis/Data.py`

 * *Files identical despite different names*

### Comparing `SciToolsSciAnalysis-2.6.5/SciAnalysis/XSAnalysis/DataGonio.py` & `SciToolsSciAnalysis-2.6.6/SciAnalysis/XSAnalysis/DataGonio.py`

 * *Files identical despite different names*

### Comparing `SciToolsSciAnalysis-2.6.5/SciAnalysis/XSAnalysis/DataQ.py` & `SciToolsSciAnalysis-2.6.6/SciAnalysis/XSAnalysis/DataQ.py`

 * *Files identical despite different names*

### Comparing `SciToolsSciAnalysis-2.6.5/SciAnalysis/XSAnalysis/DataRQconv.py` & `SciToolsSciAnalysis-2.6.6/SciAnalysis/XSAnalysis/DataRQconv.py`

 * *Files identical despite different names*

### Comparing `SciToolsSciAnalysis-2.6.5/SciAnalysis/XSAnalysis/Eiger-alternate.py` & `SciToolsSciAnalysis-2.6.6/SciAnalysis/XSAnalysis/Eiger-alternate.py`

 * *Files identical despite different names*

### Comparing `SciToolsSciAnalysis-2.6.5/SciAnalysis/XSAnalysis/Eiger.py` & `SciToolsSciAnalysis-2.6.6/SciAnalysis/XSAnalysis/Eiger.py`

 * *Files identical despite different names*

### Comparing `SciToolsSciAnalysis-2.6.5/SciAnalysis/XSAnalysis/Multiple.py` & `SciToolsSciAnalysis-2.6.6/SciAnalysis/XSAnalysis/Multiple.py`

 * *Files identical despite different names*

### Comparing `SciToolsSciAnalysis-2.6.5/SciAnalysis/XSAnalysis/Protocols.py` & `SciToolsSciAnalysis-2.6.6/SciAnalysis/XSAnalysis/Protocols.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 from SciAnalysis.XSAnalysis.Data import * #from .Data import *
 from SciAnalysis.tools import * #from ..tools import *
 #from SciAnalysis.IO_HDF import *
 
 import copy, glob
 
 class ProcessorXS(Processor):
+    '''Processor (and data loader) intended for loading x-ray scattering data
+    from files stored on disk.'''
 
     
     def load(self, infile, **kwargs):
 
         #calibration = kwargs['calibration'] if 'calibration' in kwargs else None
         #mask = kwargs['mask'] if 'mask' in kwargs else None
         #data = Data2DScattering(infile, calibration=calibration, mask=mask)
@@ -172,27 +174,48 @@
         #print( list_configs() ) # List of available beamlines
 
         from databroker import Broker
         self.db = Broker.named(beamline)
 
 
     def get_db(self, recent_days=None, verbosity=3, **constraints):
-        
+        '''Retrieve a databroker "header", based on a set of constraints.
+        For instance, the constraints could specify the exact uid of the scan.'''
         if recent_days is not None:
             constraints['since'] = time.time() - recent_days*24*60*60
         
         headers = self.db(**constraints)
         headers = [h for h in headers]
         
         if verbosity>=1 and len(headers)!=1:
             print('  WARNING: get_db got {} matches for constraints: {}'.format(len(headers), constraints))
         
         
         return headers[0]
-            
+    
+    
+
+
+class ProcessorBS(ProcessorXS):
+    '''Processor (and data loader) intended for loading x-ray scattering data
+    from Bluesky databroker.'''
+
+
+    def get_detector_image(self, recent_days=None, verbosity=3, **constraints):
+        '''Retrieve a detector image (2D array from databroker,
+        based on a set of constraints. For instance, the constraints 
+        could specify the exact uid of the scan.'''
+        
+        h = self.get_db(recent_days=recent_days, verbosity=verbosity, **constraints)
+        detector_image = h.table(fill=True)["pilatus2M_image"].to_numpy()
+        
+        return detector_image
+    
+    
+    
         
 class HDF5(Protocol):
 
     def __init__(self, name='HDF5', **kwargs):
         
         self.name = self.__class__.__name__ if name is None else name
         
@@ -1043,15 +1066,15 @@
         self.name = self.__class__.__name__ if name is None else name
         
         self.default_ext = '.png'
         self.run_args = {
             'bins_relative' : 1.0,
             'markersize' : 0,
             'linewidth' : 1.5,
-            'error' : True, 
+            # 'error' : True, 
             'show_region' : False,
             }
         self.run_args.update(kwargs)
     
         
     @run_default
     def run(self, data, output_dir, **run_args):
@@ -1072,15 +1095,16 @@
             elif run_args['show_region']:
                 data.plot(show=True)
         
         
         if 'plots' in run_args['save_results']:
             self.label_filename(data, line, **run_args)
             outfile = self.get_outfile(data.name, output_dir)
-            line.plot(save=outfile, error_band=False, ecolor='0.75', capsize=2, elinewidth=1, **run_args)
+            # line.plot(save=outfile, error_band=False, ecolor='0.75', capsize=2, elinewidth=1, **run_args)
+            line.plot(save=outfile, error_band=False,   **run_args)
 
         if 'txt' in run_args['save_results']:
             outfile = self.get_outfile(data.name, output_dir, ext='.dat')
             line.save_data(outfile)
 
         if 'hdf5' in run_args['save_results']:          
             self.save_DataLine_HDF5(line, data.name, output_dir, results=results)
```

### Comparing `SciToolsSciAnalysis-2.6.5/SciAnalysis/XSAnalysis/__init__.py` & `SciToolsSciAnalysis-2.6.6/SciAnalysis/XSAnalysis/__init__.py`

 * *Files identical despite different names*

### Comparing `SciToolsSciAnalysis-2.6.5/SciAnalysis/__init__.py` & `SciToolsSciAnalysis-2.6.6/SciAnalysis/__init__.py`

 * *Files identical despite different names*

### Comparing `SciToolsSciAnalysis-2.6.5/SciAnalysis/colormaps.py` & `SciToolsSciAnalysis-2.6.6/SciAnalysis/colormaps.py`

 * *Files identical despite different names*

### Comparing `SciToolsSciAnalysis-2.6.5/SciAnalysis/settings.py` & `SciToolsSciAnalysis-2.6.6/SciAnalysis/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Global settings which influence how SciAnalysis operates.
 
 
-SUPPRESS_EXCEPTIONS = False
-#SUPPRESS_EXCEPTIONS = True # Suppress Python exceptions (errors). This allows the script to keep running even if there is an error processing one particular file.
+#SUPPRESS_EXCEPTIONS = False
+SUPPRESS_EXCEPTIONS = True # Suppress Python exceptions (errors). This allows the script to keep running even if there is an error processing one particular file.
 
 
 #MATPLOTLIB_BACKEND = None # Leave as default
 MATPLOTLIB_BACKEND = 'Agg' # For 'headless' plotting (e.g. over an SSH connection, or to avoid bugs with joblib parallelization)
 
 
 DEFAULT_SAVE_RESULTS = ['xml', 'sql', 'plots', 'txt']
```

### Comparing `SciToolsSciAnalysis-2.6.5/SciAnalysis/tools.py` & `SciToolsSciAnalysis-2.6.6/SciAnalysis/tools.py`

 * *Files identical despite different names*

### Comparing `SciToolsSciAnalysis-2.6.5/SciToolsSciAnalysis.egg-info/PKG-INFO` & `SciToolsSciAnalysis-2.6.6/SciToolsSciAnalysis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: SciToolsSciAnalysis
-Version: 2.6.5
+Version: 2.6.6
 Summary: SciAnalysis scripts for processing image files.
-Home-page: https://github.com//CFN-softbio//SciAnalysis
+Home-page: https://github.com/CFN-softbio/SciAnalysis
 Author: Kevin Yager
 Author-email: kyager@bnl.gov
 License: BSD (3-clause)
 Description: # SciAnalysis
         
         ## Author : Kevin G. Yager
         ## Ported to git by : Julien Lhermitte
@@ -33,16 +33,19 @@
          * Protocols.linecut_qr(qz=0.025, dq=0.02, ylog=True, show_region=True, gridlines=True); #dq is half-width
          * Protocols.linecut_qz(name='linecut_qz_new', ylog=True, qr=0, dq=0.02, show_region=True, plot_range=[0.2, 0.4, None, None])
          * Protocols.linecut_qz_fit(qr=0.0, dq=0.01, show_region=True, label_filename=True, trim_range=[0.01, 0.4], fit_range=[0.093, 0.115], plot_range=[0.01, 0.4, 0, None], q0=[0.11]) 
          * Protocols.circular_average_q2I_fit(plot_range=[0.8, 1.3, 0, None], qn_power=0.0, trim_range=[0.1, 3.5], fit_range=[0.95, 1.4], num_curves=2, q0=[1.00, 1.2], sigma=0.02, show_curves=1, label_filename=True), 
          * Protocols.sector_average(angle=70, dangle=10, plot_range=[1.2, 3.7, 0, 1200], show_region=True) #pie-shaped
          * Protocols.roi(show_region=True, qx=1, dqx=0.02, qz=1, dqz=0.02, prepend='stats_')
         
+        
         run_args = { 'verbosity' : 3,
-                    #'save_results' : ['xml', 'plots', 'txt', 'hdf5'],
+        
+                    'save_results' : ['xml', 'plots', 'txt', 'hdf5'],
+                    
                     'rcParams': {'axes.labelsize': 25,
                                     'xtick.labelsize': 20,
                                     'ytick.labelsize': 20,
                                     'xtick.major.pad': 10,
                                     'ytick.major.pad': 10,
                                     },
                     }
```

### Comparing `SciToolsSciAnalysis-2.6.5/SciToolsSciAnalysis.egg-info/SOURCES.txt` & `SciToolsSciAnalysis-2.6.6/SciToolsSciAnalysis.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,14 @@
+LICENSE
+MANIFEST.in
 README.md
+requirements.txt
 setup.cfg
 setup.py
+versioneer.py
 SciAnalysis/Base.py
 SciAnalysis/Data.py
 SciAnalysis/Fit.py
 SciAnalysis/IO_HDF.py
 SciAnalysis/Result.py
 SciAnalysis/__init__.py
 SciAnalysis/_version.py
```

### Comparing `SciToolsSciAnalysis-2.6.5/setup.py` & `SciToolsSciAnalysis-2.6.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     cmdclass=versioneer.get_cmdclass(),
     description="SciAnalysis scripts for processing image files.",
     long_description=readme,
     long_description_content_type='text/markdown',
     author="Kevin Yager",
     author_email="kyager@bnl.gov",
     keywords="Analysis",
-    url="https://github.com//CFN-softbio//SciAnalysis",
+    url="https://github.com/CFN-softbio/SciAnalysis",
     python_requires=">={}".format(".".join(str(n) for n in min_version)),
     packages=find_packages(exclude=["docs", "tests"]),
     entry_points={
         "console_scripts": [
             # 'command = some.module:some_function',
         ],
     },
```

