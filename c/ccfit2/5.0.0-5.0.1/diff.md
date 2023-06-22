# Comparing `tmp/ccfit2-5.0.0.tar.gz` & `tmp/ccfit2-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccfit2-5.0.0.tar", last modified: Fri Jun 16 14:31:56 2023, max compression
+gzip compressed data, was "ccfit2-5.0.1.tar", last modified: Thu Jun 22 09:00:01 2023, max compression
```

## Comparing `ccfit2-5.0.0.tar` & `ccfit2-5.0.1.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:31:56.509508 ccfit2-5.0.0/
--rw-r--r--   0 root         (0) root         (0)     1110 2023-06-16 14:31:56.508509 ccfit2-5.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      501 2023-06-16 14:31:32.000000 ccfit2-5.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:31:56.507508 ccfit2-5.0.0/ccfit2/
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-06-16 14:31:32.000000 ccfit2-5.0.0/ccfit2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-06-16 14:31:53.000000 ccfit2-5.0.0/ccfit2/__version__.py
--rw-rw-rw-   0 root         (0) root         (0)   131893 2023-06-16 14:31:32.000000 ccfit2-5.0.0/ccfit2/ac.py
--rw-rw-rw-   0 root         (0) root         (0)    67725 2023-06-16 14:31:32.000000 ccfit2-5.0.0/ccfit2/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    61106 2023-06-16 14:31:32.000000 ccfit2-5.0.0/ccfit2/dc.py
--rw-rw-rw-   0 root         (0) root         (0)    20395 2023-06-16 14:31:32.000000 ccfit2-5.0.0/ccfit2/gui.py
--rw-rw-rw-   0 root         (0) root         (0)   167544 2023-06-16 14:31:32.000000 ccfit2-5.0.0/ccfit2/relaxation.py
--rw-rw-rw-   0 root         (0) root         (0)     1756 2023-06-16 14:31:32.000000 ccfit2-5.0.0/ccfit2/stats.py
--rw-rw-rw-   0 root         (0) root         (0)    10668 2023-06-16 14:31:32.000000 ccfit2-5.0.0/ccfit2/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    21023 2023-06-16 14:31:32.000000 ccfit2-5.0.0/ccfit2/waveform.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:31:56.508509 ccfit2-5.0.0/ccfit2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1110 2023-06-16 14:31:56.000000 ccfit2-5.0.0/ccfit2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      382 2023-06-16 14:31:56.000000 ccfit2-5.0.0/ccfit2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 14:31:56.000000 ccfit2-5.0.0/ccfit2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       95 2023-06-16 14:31:56.000000 ccfit2-5.0.0/ccfit2.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      133 2023-06-16 14:31:56.000000 ccfit2-5.0.0/ccfit2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-16 14:31:56.000000 ccfit2-5.0.0/ccfit2.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      206 2023-06-16 14:31:32.000000 ccfit2-5.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-16 14:31:56.509508 ccfit2-5.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1544 2023-06-16 14:31:53.000000 ccfit2-5.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 09:00:01.312763 ccfit2-5.0.1/
+-rw-rw-rw-   0 root         (0) root         (0)    35075 2023-06-22 08:59:27.000000 ccfit2-5.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1132 2023-06-22 09:00:01.312763 ccfit2-5.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      501 2023-06-22 08:59:27.000000 ccfit2-5.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 09:00:01.310763 ccfit2-5.0.1/ccfit2/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-06-22 08:59:27.000000 ccfit2-5.0.1/ccfit2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-06-22 08:59:58.000000 ccfit2-5.0.1/ccfit2/__version__.py
+-rw-rw-rw-   0 root         (0) root         (0)   132398 2023-06-22 08:59:27.000000 ccfit2-5.0.1/ccfit2/ac.py
+-rw-rw-rw-   0 root         (0) root         (0)    67722 2023-06-22 08:59:27.000000 ccfit2-5.0.1/ccfit2/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    61106 2023-06-22 08:59:27.000000 ccfit2-5.0.1/ccfit2/dc.py
+-rw-rw-rw-   0 root         (0) root         (0)    20395 2023-06-22 08:59:27.000000 ccfit2-5.0.1/ccfit2/gui.py
+-rw-rw-rw-   0 root         (0) root         (0)   167566 2023-06-22 08:59:27.000000 ccfit2-5.0.1/ccfit2/relaxation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1756 2023-06-22 08:59:27.000000 ccfit2-5.0.1/ccfit2/stats.py
+-rw-rw-rw-   0 root         (0) root         (0)    10668 2023-06-22 08:59:27.000000 ccfit2-5.0.1/ccfit2/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    21023 2023-06-22 08:59:27.000000 ccfit2-5.0.1/ccfit2/waveform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 09:00:01.311763 ccfit2-5.0.1/ccfit2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1132 2023-06-22 09:00:01.000000 ccfit2-5.0.1/ccfit2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      390 2023-06-22 09:00:01.000000 ccfit2-5.0.1/ccfit2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 09:00:01.000000 ccfit2-5.0.1/ccfit2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       95 2023-06-22 09:00:01.000000 ccfit2-5.0.1/ccfit2.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      133 2023-06-22 09:00:01.000000 ccfit2-5.0.1/ccfit2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-22 09:00:01.000000 ccfit2-5.0.1/ccfit2.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      206 2023-06-22 08:59:27.000000 ccfit2-5.0.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 09:00:01.312763 ccfit2-5.0.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1544 2023-06-22 08:59:58.000000 ccfit2-5.0.1/setup.py
```

### Comparing `ccfit2-5.0.0/PKG-INFO` & `ccfit2-5.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: ccfit2
-Version: 5.0.0
+Version: 5.0.1
 Summary: CCFIT2 is a program for fitting AC and DC magnetisation data
 Home-page: https://gitlab.com/chilton-group/cc-fit2
 Author: Daniel Reta
 Author-email: danielreta1@gmail.com
 Project-URL: Bug Tracker, https://gitlab.com/chilton-group/cc-fit2/-/issues
 Project-URL: Documentation, https://chilton-group.gitlab.io/cc-fit2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # ccfit2
 
 ccfit2 is a package for fitting AC and DC magnetisation data to obtain magnetic
 relaxation rates, and then to model the field- and/or temperature-dependence of
 these rates with parameterised models of spin-phonon coupling mechanisms.
```

### Comparing `ccfit2-5.0.0/ccfit2/ac.py` & `ccfit2-5.0.1/ccfit2/ac.py`

 * *Files 0% similar despite different names*

```diff
@@ -3315,72 +3315,95 @@
 
     unique_temps = np.unique(
         [experiment.rep_temperature for experiment in experiments]
     )
 
     n_temps = unique_temps.size
 
+    label_on = 'x'
+
     if n_temps == 1:
         n_cols = 1
     elif n_temps < 5:
         n_cols = 2
     elif n_temps < 10:
         n_cols = 3
     elif n_temps < 17:
         n_cols = 4
+    elif n_temps < 25:
+        n_cols = 6
+        label_on = 'y'
+    elif n_temps < 43:
+        n_cols = 7
+        label_on = 'y'
+    elif n_temps < 56:
+        n_cols = 8
+        label_on = 'y'
+    elif n_temps < 64:
+        n_cols = 9
+        label_on = 'y'
     else:
-        n_cols = 5
+        n_cols = 10
+        label_on = 'y'
 
     n_rows = int(np.ceil(n_temps / n_cols))
 
-    figsize = 7. / 3. * n_rows
-    if figsize > 7:
-        figsize = 7
+    width = 7. / 3. * n_rows
+    if width > 7:
+        width = 7.
+    height = width * 1.
+
+    if n_cols > 6:
+        width = 1.5*height
 
     # Show each data set individually for identification of peaks
     fig, axs = plt.subplots(
         n_rows,
         n_cols,
         sharex='none',
         sharey='none',
-        figsize=(figsize, figsize),
+        figsize=(width, height),
         num='Select temperatures to fit',
     )
 
     suptitle = r'$\chi^{{,,}}$ vs wave frequency under {:2.1f} Oe field'.format( # noqa
         experiments[0].rep_dc_field
     )
 
     suptitle += '\n Select (click) the temperatures to fit (make green)'
     suptitle += ' then close this window.'
 
-    fig.subplots_adjust(hspace=.4, wspace=.08)
     plt.suptitle(suptitle, fontsize=11)
 
     for experiment, ax in zip(experiments, axs.flatten()):
         ax.semilogx(
             experiment.ac_freqs,
             experiment.imag_sus,
             marker='o',
             markeredgewidth=1,
             markeredgecolor='b',
             markerfacecolor='w',
             markersize=5,
             c='b',
             lw=.5
         )
-        ax.set_xlabel('{:.2f} K'.format(experiment.rep_temperature))
+
+        if label_on == 'y':
+            ax.set_ylabel('{:.2f} K'.format(experiment.rep_temperature))
+        elif label_on == 'x':
+            ax.set_xlabel('{:.2f} K'.format(experiment.rep_temperature))
 
         ax.xaxis.set_minor_formatter(NullFormatter())
         ax.yaxis.set_minor_formatter(NullFormatter())
         ax.xaxis.set_major_formatter(NullFormatter())
         ax.yaxis.set_major_formatter(NullFormatter())
         ax.yaxis.set_major_locator(NullLocator())
 
         ax.set_box_aspect(aspect=1)
+    fig.subplots_adjust(hspace=0.08, wspace=.08)
 
     # Remove empty axes
     for _ in range(axs.size - n_temps):
         fig.delaxes(axs.flatten()[-1])
         axs = np.delete(axs, -1)
 
     colors = {
```

### Comparing `ccfit2-5.0.0/ccfit2/cli.py` & `ccfit2-5.0.1/ccfit2/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1426,15 +1426,15 @@
         ccfit2 ac ...
         ccfit2 waveform ...
         ccfit2 dc ...
         ccfit2 relaxation ...
     '''
 
     epilog = '''
-    To display options for a specific module, use ccfit2.py module -h
+    To display options for a specific module, use ccfit2 module -h
     '''
 
     parser = argparse.ArgumentParser(
         description=description,
         epilog=epilog,
         formatter_class=argparse.RawDescriptionHelpFormatter
     )
```

### Comparing `ccfit2-5.0.0/ccfit2/dc.py` & `ccfit2-5.0.1/ccfit2/dc.py`

 * *Files identical despite different names*

### Comparing `ccfit2-5.0.0/ccfit2/gui.py` & `ccfit2-5.0.1/ccfit2/gui.py`

 * *Files identical despite different names*

### Comparing `ccfit2-5.0.0/ccfit2/relaxation.py` & `ccfit2-5.0.1/ccfit2/relaxation.py`

 * *Files 0% similar despite different names*

```diff
@@ -8720,1753 +8720,1754 @@
 000220f0: 2e79 6178 6973 2e73 6574 5f6d 696e 6f72  .yaxis.set_minor
 00022100: 5f6c 6f63 6174 6f72 2841 7574 6f4d 696e  _locator(AutoMin
 00022110: 6f72 4c6f 6361 746f 7228 2929 0a20 2020  orLocator()).   
 00022120: 2061 782e 7861 7869 732e 7365 745f 6d69   ax.xaxis.set_mi
 00022130: 6e6f 725f 6c6f 6361 746f 7228 4175 746f  nor_locator(Auto
 00022140: 4d69 6e6f 724c 6f63 6174 6f72 2829 290a  MinorLocator()).
 00022150: 0a20 2020 2061 782e 7365 745f 796c 6162  .    ax.set_ylab
-00022160: 656c 2872 2724 5c6c 6e7b 5c74 6175 7d24  el(r'$\ln{\tau}$
-00022170: 2024 5c6c 6566 7428 5c6c 6e5c 6c65 6674   $\left(\ln\left
-00022180: 5b5c 6d61 7468 7265 6775 6c61 727b 737d  [\mathregular{s}
-00022190: 5e5c 6d61 7468 7265 6775 6c61 727b 2d31  ^\mathregular{-1
-000221a0: 7d5c 7269 6768 745d 5c72 6967 6874 2924  }\right]\right)$
-000221b0: 2729 2023 206e 6f71 610a 0a20 2020 2066  ') # noqa..    f
-000221c0: 6967 2e74 6967 6874 5f6c 6179 6f75 7428  ig.tight_layout(
-000221d0: 290a 0a20 2020 2069 6620 7368 6f77 3a0a  )..    if show:.
-000221e0: 2020 2020 2020 2020 706c 742e 7368 6f77          plt.show
-000221f0: 2829 0a0a 2020 2020 6966 2073 6176 653a  ()..    if save:
-00022200: 0a20 2020 2020 2020 2066 6967 2e73 6176  .        fig.sav
-00022210: 6566 6967 2873 6176 655f 6e61 6d65 2c20  efig(save_name, 
-00022220: 6470 693d 3530 3029 0a20 2020 2020 2020  dpi=500).       
-00022230: 2069 6620 7665 7262 6f73 653a 0a20 2020   if verbose:.   
-00022240: 2020 2020 2020 2020 2069 6620 6973 696e           if isin
-00022250: 7374 616e 6365 2864 6174 6173 6574 2c20  stance(dataset, 
-00022260: 2854 6175 5444 6174 6173 6574 2929 3a0a  (TauTDataset)):.
-00022270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022280: 5f78 7661 7220 3d20 2754 270a 2020 2020  _xvar = 'T'.    
-00022290: 2020 2020 2020 2020 656c 6966 2069 7369          elif isi
-000222a0: 6e73 7461 6e63 6528 6461 7461 7365 742c  nstance(dataset,
-000222b0: 2028 5461 7548 4461 7461 7365 7429 293a   (TauHDataset)):
-000222c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000222d0: 205f 7876 6172 203d 2027 4827 0a20 2020   _xvar = 'H'.   
-000222e0: 2020 2020 2020 2020 2075 742e 6370 7269           ut.cpri
-000222f0: 6e74 280a 2020 2020 2020 2020 2020 2020  nt(.            
-00022300: 2020 2020 6627 5c6e 2046 6974 7465 6420      f'\n Fitted 
-00022310: 6c6e 2874 6175 2920 7673 2031 2f7b 5f78  ln(tau) vs 1/{_x
-00022320: 7661 727d 2070 6c6f 7420 7361 7665 6420  var} plot saved 
-00022330: 746f 205c 6e20 7b73 6176 655f 6e61 6d65  to \n {save_name
-00022340: 7d5c 6e27 2c20 2320 6e6f 7161 0a20 2020  }\n', # noqa.   
-00022350: 2020 2020 2020 2020 2020 2020 2027 6379               'cy
-00022360: 616e 270a 2020 2020 2020 2020 2020 2020  an'.            
-00022370: 290a 0a20 2020 2072 6574 7572 6e20 6669  )..    return fi
-00022380: 672c 2061 780a 0a0a 6465 6620 5f70 6c6f  g, ax...def _plo
-00022390: 745f 6669 7474 6564 5f74 696d 6573 2864  t_fitted_times(d
-000223a0: 6174 6173 6574 3a20 5461 7554 4461 7461  ataset: TauTData
-000223b0: 7365 7420 7c20 5461 7548 4461 7461 7365  set | TauHDatase
-000223c0: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
-000223d0: 2020 2020 2020 2020 2020 6d6f 6465 6c3a            model:
-000223e0: 204c 6f67 5461 7554 4d6f 6465 6c20 7c20   LogTauTModel | 
-000223f0: 4d75 6c74 694c 6f67 5461 7554 4d6f 6465  MultiLogTauTMode
-00022400: 6c20 7c20 4c6f 6754 6175 484d 6f64 656c  l | LogTauHModel
-00022410: 207c 204d 756c 7469 4c6f 6754 6175 484d   | MultiLogTauHM
-00022420: 6f64 656c 2c20 2320 6e6f 7161 0a20 2020  odel, # noqa.   
-00022430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022440: 2020 2020 6669 673a 2070 6c74 2e46 6967      fig: plt.Fig
-00022450: 7572 652c 2061 783a 2070 6c74 2e41 7865  ure, ax: plt.Axe
-00022460: 7329 3a0a 2020 2020 2727 270a 2020 2020  s):.    '''.    
-00022470: 506c 6f74 7320 6578 7065 7269 6d65 6e74  Plots experiment
-00022480: 616c 2061 6e64 2066 6974 7465 6420 286d  al and fitted (m
-00022490: 6f64 656c 2920 7265 6c61 7861 7469 6f6e  odel) relaxation
-000224a0: 2072 6174 6520 6173 5c6e 0a20 2020 206c   rate as\n.    l
-000224b0: 6e28 7461 7529 2076 7320 312f 7876 6172  n(tau) vs 1/xvar
-000224c0: 2077 6865 7265 2078 7661 7220 6973 2054   where xvar is T
-000224d0: 206f 7220 482e 0a0a 2020 2020 5061 7261   or H...    Para
-000224e0: 6d65 7465 7273 0a20 2020 202d 2d2d 2d2d  meters.    -----
-000224f0: 2d2d 2d2d 2d0a 2020 2020 6461 7461 7365  -----.    datase
-00022500: 743a 2054 6175 5444 6174 6173 6574 207c  t: TauTDataset |
-00022510: 2054 6175 4844 6174 6173 6574 0a20 2020   TauHDataset.   
-00022520: 2020 2020 2044 6174 6173 6574 2074 6f20       Dataset to 
-00022530: 706c 6f74 0a20 2020 206d 6f64 656c 3a20  plot.    model: 
-00022540: 4c6f 6754 6175 544d 6f64 656c 207c 204d  LogTauTModel | M
-00022550: 756c 7469 4c6f 6754 6175 544d 6f64 656c  ultiLogTauTModel
-00022560: 207c 204c 6f67 5461 7548 4d6f 6465 6c20   | LogTauHModel 
-00022570: 7c20 4d75 6c74 694c 6f67 5461 7548 4d6f  | MultiLogTauHMo
-00022580: 6465 6c0a 2020 2020 2020 2020 4d6f 6465  del.        Mode
-00022590: 6c20 2866 6974 7465 6429 2074 6f20 706c  l (fitted) to pl
-000225a0: 6f74 0a20 2020 2066 6967 3a20 706c 742e  ot.    fig: plt.
-000225b0: 4669 6775 7265 0a20 2020 2020 2020 204d  Figure.        M
-000225c0: 6174 706c 6f74 6c69 6220 4669 6775 7265  atplotlib Figure
-000225d0: 206f 626a 6563 7420 7573 6564 2066 6f72   object used for
-000225e0: 2070 6c6f 740a 2020 2020 6178 3a20 706c   plot.    ax: pl
-000225f0: 742e 4178 6573 0a20 2020 2020 2020 204d  t.Axes.        M
-00022600: 6174 706c 6f74 6c69 6220 4178 6973 206f  atplotlib Axis o
-00022610: 626a 6563 7420 7573 6564 2066 6f72 2070  bject used for p
-00022620: 6c6f 740a 0a20 2020 2052 6574 7572 6e73  lot..    Returns
-00022630: 0a20 2020 202d 2d2d 2d2d 2d2d 0a20 2020  .    -------.   
-00022640: 204e 6f6e 650a 2020 2020 2727 270a 0a20   None.    '''.. 
-00022650: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-00022660: 2864 6174 6173 6574 2c20 5461 7548 4461  (dataset, TauHDa
-00022670: 7461 7365 7429 3a0a 2020 2020 2020 2020  taset):.        
-00022680: 785f 7661 7273 203d 2064 6174 6173 6574  x_vars = dataset
-00022690: 2e66 6965 6c64 730a 2020 2020 2020 2020  .fields.        
-000226a0: 6178 2e73 6574 5f78 6c61 6265 6c28 7227  ax.set_xlabel(r'
-000226b0: 312f 4820 245c 6c65 6674 285c 6d61 7468  1/H $\left(\math
-000226c0: 7265 6775 6c61 727b 4f65 7d5e 5c6d 6174  regular{Oe}^\mat
-000226d0: 6872 6567 756c 6172 7b2d 317d 5c72 6967  hregular{-1}\rig
-000226e0: 6874 2924 2729 0a20 2020 2065 6c69 6620  ht)$').    elif 
-000226f0: 6973 696e 7374 616e 6365 2864 6174 6173  isinstance(datas
-00022700: 6574 2c20 5461 7554 4461 7461 7365 7429  et, TauTDataset)
-00022710: 3a0a 2020 2020 2020 2020 785f 7661 7273  :.        x_vars
-00022720: 203d 2064 6174 6173 6574 2e74 656d 7065   = dataset.tempe
-00022730: 7261 7475 7265 730a 2020 2020 2020 2020  ratures.        
-00022740: 6178 2e73 6574 5f78 6c61 6265 6c28 7227  ax.set_xlabel(r'
-00022750: 312f 5420 245c 6c65 6674 285c 6d61 7468  1/T $\left(\math
-00022760: 7265 6775 6c61 727b 4b7d 5e5c 6d61 7468  regular{K}^\math
-00022770: 7265 6775 6c61 727b 2d31 7d5c 7269 6768  regular{-1}\righ
-00022780: 7429 2427 290a 0a20 2020 2023 2041 6464  t)$')..    # Add
-00022790: 2075 6e63 6572 7461 696e 7469 6573 2061   uncertainties a
-000227a0: 7320 6572 726f 7262 6172 730a 2020 2020  s errorbars.    
-000227b0: 6966 206c 656e 2864 6174 6173 6574 2e72  if len(dataset.r
-000227c0: 6174 655f 706d 293a 0a0a 2020 2020 2020  ate_pm):..      
-000227d0: 2020 2320 4361 6c63 756c 6174 6520 7469    # Calculate ti
-000227e0: 6d65 2065 7272 6f72 6261 7273 0a20 2020  me errorbars.   
-000227f0: 2020 2020 2074 696d 6573 203d 2031 2e20       times = 1. 
-00022800: 2f20 6461 7461 7365 742e 7261 7465 730a  / dataset.rates.
-00022810: 2020 2020 2020 2020 6d69 6e5f 7469 6d65          min_time
-00022820: 203d 2031 2e20 2f20 2864 6174 6173 6574   = 1. / (dataset
-00022830: 2e72 6174 6573 202b 2064 6174 6173 6574  .rates + dataset
-00022840: 2e72 6174 655f 706d 5b31 2c20 3a5d 290a  .rate_pm[1, :]).
-00022850: 2020 2020 2020 2020 6d61 785f 7469 6d65          max_time
-00022860: 203d 2031 2e20 2f20 2864 6174 6173 6574   = 1. / (dataset
-00022870: 2e72 6174 6573 202d 2064 6174 6173 6574  .rates - dataset
-00022880: 2e72 6174 655f 706d 5b30 2c20 3a5d 290a  .rate_pm[0, :]).
-00022890: 0a20 2020 2020 2020 206c 6e5f 6d69 6e5f  .        ln_min_
-000228a0: 7469 6d65 203d 206e 702e 6c6f 6728 6d69  time = np.log(mi
-000228b0: 6e5f 7469 6d65 290a 2020 2020 2020 2020  n_time).        
-000228c0: 6c6e 5f6d 6178 5f74 696d 6520 3d20 6e70  ln_max_time = np
-000228d0: 2e6c 6f67 286d 6178 5f74 696d 6529 0a0a  .log(max_time)..
-000228e0: 2020 2020 2020 2020 6c6e 5f74 696d 655f          ln_time_
-000228f0: 706c 7573 203d 206c 6e5f 6d61 785f 7469  plus = ln_max_ti
-00022900: 6d65 202d 206e 702e 6c6f 6728 7469 6d65  me - np.log(time
-00022910: 7329 0a20 2020 2020 2020 206c 6e5f 7469  s).        ln_ti
-00022920: 6d65 5f6d 696e 7573 203d 206e 702e 6c6f  me_minus = np.lo
-00022930: 6728 7469 6d65 7329 202d 206c 6e5f 6d69  g(times) - ln_mi
-00022940: 6e5f 7469 6d65 0a0a 2020 2020 2020 2020  n_time..        
-00022950: 6c6e 7469 6d65 5f6d 7020 3d20 6e70 2e61  lntime_mp = np.a
-00022960: 7272 6179 285b 6c6e 5f74 696d 655f 6d69  rray([ln_time_mi
-00022970: 6e75 732c 206c 6e5f 7469 6d65 5f70 6c75  nus, ln_time_plu
-00022980: 735d 290a 0a20 2020 2020 2020 2061 782e  s])..        ax.
-00022990: 6572 726f 7262 6172 280a 2020 2020 2020  errorbar(.      
-000229a0: 2020 2020 2020 312e 202f 2078 5f76 6172        1. / x_var
-000229b0: 732c 0a20 2020 2020 2020 2020 2020 206e  s,.            n
-000229c0: 702e 6c6f 6728 7469 6d65 7329 2c0a 2020  p.log(times),.  
-000229d0: 2020 2020 2020 2020 2020 7965 7272 3d6c            yerr=l
-000229e0: 6e74 696d 655f 6d70 2c0a 2020 2020 2020  ntime_mp,.      
-000229f0: 2020 2020 2020 6d61 726b 6572 3d27 6f27        marker='o'
-00022a00: 2c0a 2020 2020 2020 2020 2020 2020 6c77  ,.            lw
-00022a10: 3d30 2c0a 2020 2020 2020 2020 2020 2020  =0,.            
-00022a20: 656c 696e 6577 6964 7468 3d31 2e35 2c0a  elinewidth=1.5,.
-00022a30: 2020 2020 2020 2020 2020 2020 6669 6c6c              fill
-00022a40: 7374 796c 653d 276e 6f6e 6527 2c0a 2020  style='none',.  
-00022a50: 2020 2020 2020 2020 2020 6c61 6265 6c3d            label=
-00022a60: 2745 7870 6572 696d 656e 7427 2c0a 2020  'Experiment',.  
-00022a70: 2020 2020 2020 2020 2020 636f 6c6f 723d            color=
-00022a80: 2762 6c61 636b 270a 2020 2020 2020 2020  'black'.        
-00022a90: 290a 2020 2020 656c 7365 3a0a 2020 2020  ).    else:.    
-00022aa0: 2020 2020 6178 2e70 6c6f 7428 0a20 2020      ax.plot(.   
-00022ab0: 2020 2020 2020 2020 2031 2e20 2f20 785f           1. / x_
-00022ac0: 7661 7273 2c0a 2020 2020 2020 2020 2020  vars,.          
-00022ad0: 2020 6e70 2e6c 6f67 2831 2e20 2f20 6461    np.log(1. / da
-00022ae0: 7461 7365 742e 7261 7465 7329 2c0a 2020  taset.rates),.  
-00022af0: 2020 2020 2020 2020 2020 6d61 726b 6572            marker
-00022b00: 3d27 6f27 2c0a 2020 2020 2020 2020 2020  ='o',.          
-00022b10: 2020 6c77 3d30 2c0a 2020 2020 2020 2020    lw=0,.        
-00022b20: 2020 2020 6669 6c6c 7374 796c 653d 276e      fillstyle='n
-00022b30: 6f6e 6527 2c0a 2020 2020 2020 2020 2020  one',.          
-00022b40: 2020 6c61 6265 6c3d 2745 7870 6572 696d    label='Experim
-00022b50: 656e 7427 2c0a 2020 2020 2020 2020 2020  ent',.          
-00022b60: 2020 636f 6c6f 723d 2762 6c61 636b 270a    color='black'.
-00022b70: 2020 2020 2020 2020 290a 0a20 2020 2078          )..    x
-00022b80: 5f76 6172 735f 6772 6964 203d 206e 702e  _vars_grid = np.
-00022b90: 6c6f 6773 7061 6365 280a 2020 2020 2020  logspace(.      
-00022ba0: 2020 6e70 2e6c 6f67 3130 286e 702e 6d69    np.log10(np.mi
-00022bb0: 6e28 785f 7661 7273 2929 2c0a 2020 2020  n(x_vars)),.    
-00022bc0: 2020 2020 6e70 2e6c 6f67 3130 286e 702e      np.log10(np.
-00022bd0: 6d61 7828 785f 7661 7273 2929 2c0a 2020  max(x_vars)),.  
-00022be0: 2020 2020 2020 3530 300a 2020 2020 290a        500.    ).
-00022bf0: 0a20 2020 2069 6620 7479 7065 286d 6f64  .    if type(mod
-00022c00: 656c 2920 696e 205b 4d75 6c74 694c 6f67  el) in [MultiLog
-00022c10: 5461 7554 4d6f 6465 6c2c 204d 756c 7469  TauTModel, Multi
-00022c20: 4c6f 6754 6175 484d 6f64 656c 5d3a 0a20  LogTauHModel]:. 
-00022c30: 2020 2020 2020 206c 6f67 6d6f 6465 6c73         logmodels
-00022c40: 203d 206d 6f64 656c 2e6c 6f67 6d6f 6465   = model.logmode
-00022c50: 6c73 0a20 2020 2065 6c73 653a 0a20 2020  ls.    else:.   
-00022c60: 2020 2020 206c 6f67 6d6f 6465 6c73 203d       logmodels =
-00022c70: 205b 6d6f 6465 6c5d 0a0a 2020 2020 666f   [model]..    fo
-00022c80: 7220 6c6f 676d 6f64 656c 2069 6e20 6c6f  r logmodel in lo
-00022c90: 676d 6f64 656c 733a 0a0a 2020 2020 2020  gmodels:..      
-00022ca0: 2020 6966 2074 7970 6528 6c6f 676d 6f64    if type(logmod
-00022cb0: 656c 2920 6973 204c 6f67 4f72 6261 6368  el) is LogOrbach
-00022cc0: 4d6f 6465 6c3a 0a20 2020 2020 2020 2020  Model:.         
-00022cd0: 2020 206c 6162 656c 5f66 6974 203d 2027     label_fit = '
-00022ce0: 5c6e 4669 7420 7769 7468 270a 2020 2020  \nFit with'.    
-00022cf0: 2020 2020 2020 2020 6c61 6265 6c5f 6669          label_fi
-00022d00: 7420 2b3d 2027 5c6e 2720 2b20 7227 7b7d  t += '\n' + r'{}
-00022d10: 207b 3a36 2e32 667d 2073 272e 666f 726d   {:6.2f} s'.form
-00022d20: 6174 280a 2020 2020 2020 2020 2020 2020  at(.            
-00022d30: 2020 2020 6c6f 676d 6f64 656c 2e56 4152      logmodel.VAR
-00022d40: 4e41 4d45 535f 4d4d 5b27 755f 6566 6627  NAMES_MM['u_eff'
-00022d50: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-00022d60: 2020 206c 6f67 6d6f 6465 6c2e 6669 6e61     logmodel.fina
-00022d70: 6c5f 7661 725f 7661 6c75 6573 5b27 755f  l_var_values['u_
-00022d80: 6566 6627 5d0a 2020 2020 2020 2020 2020  eff'].          
-00022d90: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-00022da0: 6c61 6265 6c5f 6669 7420 2b3d 2027 5c6e  label_fit += '\n
-00022db0: 2720 2b20 7227 7b7d 207b 3a30 342e 3365  ' + r'{} {:04.3e
-00022dc0: 7d27 2e66 6f72 6d61 7428 0a20 2020 2020  }'.format(.     
-00022dd0: 2020 2020 2020 2020 2020 206c 6f67 6d6f             logmo
-00022de0: 6465 6c2e 5641 524e 414d 4553 5f4d 4d5b  del.VARNAMES_MM[
-00022df0: 2741 275d 2c20 6c6f 676d 6f64 656c 2e66  'A'], logmodel.f
-00022e00: 696e 616c 5f76 6172 5f76 616c 7565 735b  inal_var_values[
-00022e10: 2741 275d 0a20 2020 2020 2020 2020 2020  'A'].           
-00022e20: 2029 0a20 2020 2020 2020 2065 6c69 6620   ).        elif 
-00022e30: 7479 7065 286c 6f67 6d6f 6465 6c29 2069  type(logmodel) i
-00022e40: 7320 4c6f 6752 616d 616e 4d6f 6465 6c3a  s LogRamanModel:
-00022e50: 0a20 2020 2020 2020 2020 2020 206c 6162  .            lab
-00022e60: 656c 5f66 6974 203d 2027 5c6e 4669 7420  el_fit = '\nFit 
-00022e70: 7769 7468 270a 2020 2020 2020 2020 2020  with'.          
-00022e80: 2020 6c61 6265 6c5f 6669 7420 2b3d 2027    label_fit += '
-00022e90: 5c6e 2720 2b20 7227 7b7d 207b 3a36 2e32  \n' + r'{} {:6.2
-00022ea0: 667d 2073 272e 666f 726d 6174 280a 2020  f} s'.format(.  
-00022eb0: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-00022ec0: 676d 6f64 656c 2e56 4152 4e41 4d45 535f  gmodel.VARNAMES_
-00022ed0: 4d4d 5b27 5227 5d2c 206c 6f67 6d6f 6465  MM['R'], logmode
-00022ee0: 6c2e 6669 6e61 6c5f 7661 725f 7661 6c75  l.final_var_valu
-00022ef0: 6573 5b27 5227 5d0a 2020 2020 2020 2020  es['R'].        
-00022f00: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00022f10: 2020 6c61 6265 6c5f 6669 7420 2b3d 2027    label_fit += '
-00022f20: 5c6e 2720 2b20 7227 7b7d 207b 3a30 342e  \n' + r'{} {:04.
-00022f30: 3365 7d27 2e66 6f72 6d61 7428 0a20 2020  3e}'.format(.   
-00022f40: 2020 2020 2020 2020 2020 2020 206c 6f67               log
-00022f50: 6d6f 6465 6c2e 5641 524e 414d 4553 5f4d  model.VARNAMES_M
-00022f60: 4d5b 276e 275d 2c20 6c6f 676d 6f64 656c  M['n'], logmodel
-00022f70: 2e66 696e 616c 5f76 6172 5f76 616c 7565  .final_var_value
-00022f80: 735b 276e 275d 0a20 2020 2020 2020 2020  s['n'].         
-00022f90: 2020 2029 0a20 2020 2020 2020 2065 6c69     ).        eli
-00022fa0: 6620 7479 7065 286c 6f67 6d6f 6465 6c29  f type(logmodel)
-00022fb0: 2069 7320 4c6f 6751 544d 4d6f 6465 6c3a   is LogQTMModel:
-00022fc0: 0a20 2020 2020 2020 2020 2020 206c 6162  .            lab
-00022fd0: 656c 5f66 6974 203d 2027 5c6e 4669 7420  el_fit = '\nFit 
-00022fe0: 7769 7468 270a 2020 2020 2020 2020 2020  with'.          
-00022ff0: 2020 6c61 6265 6c5f 6669 7420 2b3d 2027    label_fit += '
-00023000: 5c6e 2720 2b20 7227 7b7d 207b 3a36 2e32  \n' + r'{} {:6.2
-00023010: 667d 2073 272e 666f 726d 6174 280a 2020  f} s'.format(.  
-00023020: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-00023030: 676d 6f64 656c 2e56 4152 4e41 4d45 535f  gmodel.VARNAMES_
-00023040: 4d4d 5b27 5127 5d2c 206c 6f67 6d6f 6465  MM['Q'], logmode
-00023050: 6c2e 6669 6e61 6c5f 7661 725f 7661 6c75  l.final_var_valu
-00023060: 6573 5b27 5127 5d0a 2020 2020 2020 2020  es['Q'].        
-00023070: 2020 2020 290a 2020 2020 2020 2020 656c      ).        el
-00023080: 6966 2074 7970 6528 6c6f 676d 6f64 656c  if type(logmodel
-00023090: 2920 6973 204c 6f67 4469 7265 6374 4d6f  ) is LogDirectMo
-000230a0: 6465 6c3a 0a20 2020 2020 2020 2020 2020  del:.           
-000230b0: 206c 6162 656c 5f66 6974 203d 2027 5c6e   label_fit = '\n
-000230c0: 4669 7420 7769 7468 270a 2020 2020 2020  Fit with'.      
-000230d0: 2020 2020 2020 6c61 6265 6c5f 6669 7420        label_fit 
-000230e0: 2b3d 2027 5c6e 2720 2b20 7227 7b7d 207b  += '\n' + r'{} {
-000230f0: 3a36 2e32 667d 2073 272e 666f 726d 6174  :6.2f} s'.format
-00023100: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00023110: 2020 6c6f 676d 6f64 656c 2e56 4152 4e41    logmodel.VARNA
-00023120: 4d45 535f 4d4d 5b27 4427 5d2c 206c 6f67  MES_MM['D'], log
-00023130: 6d6f 6465 6c2e 6669 6e61 6c5f 7661 725f  model.final_var_
-00023140: 7661 6c75 6573 5b27 4427 5d0a 2020 2020  values['D'].    
-00023150: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00023160: 2020 6d6f 6465 6c5f 7261 7465 7320 3d20    model_rates = 
-00023170: 3130 2a2a 6c6f 676d 6f64 656c 2e6d 6f64  10**logmodel.mod
-00023180: 656c 280a 2020 2020 2020 2020 2020 2020  el(.            
-00023190: 6c6f 676d 6f64 656c 2e66 696e 616c 5f76  logmodel.final_v
-000231a0: 6172 5f76 616c 7565 732c 0a20 2020 2020  ar_values,.     
-000231b0: 2020 2020 2020 2078 5f76 6172 735f 6772         x_vars_gr
-000231c0: 6964 2c0a 2020 2020 2020 2020 290a 0a20  id,.        ).. 
-000231d0: 2020 2020 2020 2023 2054 7269 6d20 6d6f         # Trim mo
-000231e0: 6465 6c20 7261 7465 7320 746f 2073 656e  del rates to sen
-000231f0: 7369 626c 6520 7661 6c75 6573 0a20 2020  sible values.   
-00023200: 2020 2020 2076 616c 6964 5f69 6e74 203d       valid_int =
-00023210: 206e 702e 7768 6572 6528 6d6f 6465 6c5f   np.where(model_
-00023220: 7261 7465 7320 3e20 3145 2d36 295b 305d  rates > 1E-6)[0]
-00023230: 0a0a 2020 2020 2020 2020 6178 2e70 6c6f  ..        ax.plo
-00023240: 7428 0a20 2020 2020 2020 2020 2020 2031  t(.            1
-00023250: 2e20 2f20 6e70 2e61 7272 6179 2878 5f76  . / np.array(x_v
-00023260: 6172 735f 6772 6964 295b 7661 6c69 645f  ars_grid)[valid_
-00023270: 696e 745d 2c0a 2020 2020 2020 2020 2020  int],.          
-00023280: 2020 6e70 2e6c 6f67 2831 2e20 2f20 6e70    np.log(1. / np
-00023290: 2e61 7272 6179 286d 6f64 656c 5f72 6174  .array(model_rat
-000232a0: 6573 295b 7661 6c69 645f 696e 745d 292c  es)[valid_int]),
-000232b0: 0a20 2020 2020 2020 2020 2020 206c 773d  .            lw=
-000232c0: 312e 352c 0a20 2020 2020 2020 2020 2020  1.5,.           
-000232d0: 206c 6162 656c 3d6c 6f67 6d6f 6465 6c2e   label=logmodel.
-000232e0: 4e41 4d45 2c0a 2020 2020 2020 2020 2020  NAME,.          
-000232f0: 2020 6c73 3d27 2d2d 270a 2020 2020 2020    ls='--'.      
-00023300: 2020 290a 0a20 2020 2069 6620 7479 7065    )..    if type
-00023310: 286d 6f64 656c 2920 696e 205b 4d75 6c74  (model) in [Mult
-00023320: 694c 6f67 5461 7554 4d6f 6465 6c2c 204d  iLogTauTModel, M
-00023330: 756c 7469 4c6f 6754 6175 484d 6f64 656c  ultiLogTauHModel
-00023340: 5d20 616e 6420 6c65 6e28 6c6f 676d 6f64  ] and len(logmod
-00023350: 656c 7329 203e 2031 3a20 2320 6e6f 7161  els) > 1: # noqa
-00023360: 0a20 2020 2020 2020 2074 6f74 616c 203d  .        total =
-00023370: 206e 702e 7a65 726f 7328 6c65 6e28 785f   np.zeros(len(x_
-00023380: 7661 7273 5f67 7269 6429 290a 0a20 2020  vars_grid))..   
-00023390: 2020 2020 2066 6f72 206c 6f67 6d6f 6465       for logmode
-000233a0: 6c20 696e 206c 6f67 6d6f 6465 6c73 3a0a  l in logmodels:.
-000233b0: 2020 2020 2020 2020 2020 2020 746f 7461              tota
-000233c0: 6c20 2b3d 2031 302a 2a6c 6f67 6d6f 6465  l += 10**logmode
-000233d0: 6c2e 6d6f 6465 6c28 0a20 2020 2020 2020  l.model(.       
-000233e0: 2020 2020 2020 2020 206c 6f67 6d6f 6465           logmode
-000233f0: 6c2e 6669 6e61 6c5f 7661 725f 7661 6c75  l.final_var_valu
-00023400: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
-00023410: 2020 2020 785f 7661 7273 5f67 7269 642c      x_vars_grid,
-00023420: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
-00023430: 2020 2020 2020 2020 6178 2e70 6c6f 7428          ax.plot(
-00023440: 0a20 2020 2020 2020 2020 2020 2031 2e20  .            1. 
-00023450: 2f20 785f 7661 7273 5f67 7269 642c 0a20  / x_vars_grid,. 
-00023460: 2020 2020 2020 2020 2020 206e 702e 6c6f             np.lo
-00023470: 6728 312e 202f 2074 6f74 616c 292c 0a20  g(1. / total),. 
-00023480: 2020 2020 2020 2020 2020 206c 773d 312e             lw=1.
-00023490: 352c 0a20 2020 2020 2020 2020 2020 206c  5,.            l
-000234a0: 6162 656c 3d27 546f 7461 6c27 2c0a 2020  abel='Total',.  
-000234b0: 2020 2020 2020 2020 2020 636f 6c6f 723d            color=
-000234c0: 2772 6564 270a 2020 2020 2020 2020 290a  'red'.        ).
-000234d0: 0a20 2020 2023 2045 6e61 626c 6520 6d69  .    # Enable mi
-000234e0: 6e6f 7220 7469 636b 730a 2020 2020 6178  nor ticks.    ax
-000234f0: 2e79 6178 6973 2e73 6574 5f6d 696e 6f72  .yaxis.set_minor
-00023500: 5f6c 6f63 6174 6f72 2841 7574 6f4d 696e  _locator(AutoMin
-00023510: 6f72 4c6f 6361 746f 7228 2929 0a20 2020  orLocator()).   
-00023520: 2061 782e 7861 7869 732e 7365 745f 6d69   ax.xaxis.set_mi
-00023530: 6e6f 725f 6c6f 6361 746f 7228 4175 746f  nor_locator(Auto
-00023540: 4d69 6e6f 724c 6f63 6174 6f72 2829 290a  MinorLocator()).
-00023550: 0a20 2020 2065 7870 7265 7373 696f 6e20  .    expression 
-00023560: 3d20 2727 0a0a 2020 2020 666f 7220 6c6f  = ''..    for lo
-00023570: 676d 6f64 656c 2069 6e20 6c6f 676d 6f64  gmodel in logmod
-00023580: 656c 733a 0a20 2020 2020 2020 2066 6f72  els:.        for
-00023590: 2069 742c 206e 616d 6520 696e 2065 6e75   it, name in enu
-000235a0: 6d65 7261 7465 286c 6f67 6d6f 6465 6c2e  merate(logmodel.
-000235b0: 5041 524e 414d 4553 293a 0a20 2020 2020  PARNAMES):.     
-000235c0: 2020 2020 2020 2065 7870 7265 7373 696f         expressio
-000235d0: 6e20 2b3d 2027 7b7d 203d 207b 3a2e 3366  n += '{} = {:.3f
-000235e0: 7d20 272e 666f 726d 6174 280a 2020 2020  } '.format(.    
-000235f0: 2020 2020 2020 2020 2020 2020 6c6f 676d              logm
-00023600: 6f64 656c 2e56 4152 4e41 4d45 535f 4d4d  odel.VARNAMES_MM
-00023610: 5b6e 616d 655d 2c0a 2020 2020 2020 2020  [name],.        
-00023620: 2020 2020 2020 2020 6c6f 676d 6f64 656c          logmodel
-00023630: 2e66 696e 616c 5f76 6172 5f76 616c 7565  .final_var_value
-00023640: 735b 6e61 6d65 5d2c 0a20 2020 2020 2020  s[name],.       
-00023650: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00023660: 2020 2069 6620 6e61 6d65 2069 6e20 6c6f     if name in lo
-00023670: 676d 6f64 656c 2e66 6974 5f76 6172 732e  gmodel.fit_vars.
-00023680: 6b65 7973 2829 3a0a 2020 2020 2020 2020  keys():.        
-00023690: 2020 2020 2020 2020 6578 7072 6573 7369          expressi
-000236a0: 6f6e 202b 3d20 7227 245c 706d 2420 270a  on += r'$\pm$ '.
-000236b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000236c0: 6578 7072 6573 7369 6f6e 202b 3d20 277b  expression += '{
-000236d0: 3a2e 3366 7d20 272e 666f 726d 6174 286c  :.3f} '.format(l
-000236e0: 6f67 6d6f 6465 6c2e 6669 745f 7374 6465  ogmodel.fit_stde
-000236f0: 765b 6e61 6d65 5d29 0a20 2020 2020 2020  v[name]).       
-00023700: 2020 2020 2065 7870 7265 7373 696f 6e20       expression 
-00023710: 2b3d 2027 7b7d 2020 2020 272e 666f 726d  += '{}    '.form
-00023720: 6174 286c 6f67 6d6f 6465 6c2e 554e 4954  at(logmodel.UNIT
-00023730: 535f 4d4d 5b6e 616d 655d 290a 2020 2020  S_MM[name]).    
-00023740: 2020 2020 2020 2020 6966 2069 7420 3d3d          if it ==
-00023750: 2031 2061 6e64 206c 656e 286c 6f67 6d6f   1 and len(logmo
-00023760: 6465 6c2e 6669 745f 7661 7273 2e6b 6579  del.fit_vars.key
-00023770: 7328 2929 203e 2032 3a0a 2020 2020 2020  s()) > 2:.      
-00023780: 2020 2020 2020 2020 2020 6578 7072 6573            expres
-00023790: 7369 6f6e 202b 3d20 275c 6e27 0a20 2020  sion += '\n'.   
-000237a0: 2020 2020 2065 7870 7265 7373 696f 6e20       expression 
-000237b0: 2b3d 2027 5c6e 270a 0a20 2020 2061 782e  += '\n'..    ax.
-000237c0: 7465 7874 280a 2020 2020 2020 2020 302e  text(.        0.
-000237d0: 302c 2031 2e30 322c 2073 3d65 7870 7265  0, 1.02, s=expre
-000237e0: 7373 696f 6e2c 2066 6f6e 7473 697a 653d  ssion, fontsize=
-000237f0: 3130 2c20 7472 616e 7366 6f72 6d3d 6178  10, transform=ax
-00023800: 2e74 7261 6e73 4178 6573 0a20 2020 2029  .transAxes.    )
-00023810: 0a0a 2020 2020 6178 2e6c 6567 656e 6428  ..    ax.legend(
-00023820: 0a20 2020 2020 2020 206c 6f63 3d27 6c6f  .        loc='lo
-00023830: 7765 7220 7269 6768 7427 2c20 666f 6e74  wer right', font
-00023840: 7369 7a65 3d27 3130 272c 206e 756d 706f  size='10', numpo
-00023850: 696e 7473 3d31 2c20 6e63 6f6c 3d31 2c20  ints=1, ncol=1, 
-00023860: 6672 616d 656f 6e3d 4661 6c73 650a 2020  frameon=False.  
-00023870: 2020 290a 2020 2020 6178 2e73 6574 5f79    ).    ax.set_y
-00023880: 6c61 6265 6c28 7227 245c 6c6e 7b5c 7461  label(r'$\ln{\ta
-00023890: 757d 2420 245c 6c65 6674 285c 6c6e 5c6c  u}$ $\left(\ln\l
-000238a0: 6566 745b 5c6d 6174 6872 6567 756c 6172  eft[\mathregular
-000238b0: 7b73 7d5e 5c6d 6174 6872 6567 756c 6172  {s}^\mathregular
-000238c0: 7b2d 317d 5c72 6967 6874 5d5c 7269 6768  {-1}\right]\righ
-000238d0: 7429 2427 2920 2320 6e6f 7161 0a0a 2020  t)$') # noqa..  
-000238e0: 2020 7265 7475 726e 0a0a 0a64 6566 2070    return...def p
-000238f0: 6c6f 745f 6669 7474 6564 5f72 6174 6573  lot_fitted_rates
-00023900: 2864 6174 6173 6574 3a20 5461 7554 4461  (dataset: TauTDa
-00023910: 7461 7365 7420 7c20 5461 7548 4461 7461  taset | TauHData
-00023920: 7365 742c 0a20 2020 2020 2020 2020 2020  set,.           
-00023930: 2020 2020 2020 2020 2020 206d 6f64 656c             model
-00023940: 3a20 4c6f 6754 6175 544d 6f64 656c 207c  : LogTauTModel |
-00023950: 204d 756c 7469 4c6f 6754 6175 544d 6f64   MultiLogTauTMod
-00023960: 656c 207c 204c 6f67 5461 7548 4d6f 6465  el | LogTauHMode
-00023970: 6c20 7c20 4d75 6c74 694c 6f67 5461 7548  l | MultiLogTauH
-00023980: 4d6f 6465 6c2c 2023 206e 6f71 610a 2020  Model, # noqa.  
-00023990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000239a0: 2020 2020 7368 6f77 3a20 626f 6f6c 203d      show: bool =
-000239b0: 2054 7275 652c 2073 6176 653a 2062 6f6f   True, save: boo
-000239c0: 6c20 3d20 4661 6c73 652c 0a20 2020 2020  l = False,.     
-000239d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000239e0: 2073 6176 655f 6e61 6d65 3a20 7374 7220   save_name: str 
-000239f0: 3d20 2766 6974 7465 645f 7261 7465 732e  = 'fitted_rates.
-00023a00: 706e 6727 2c0a 2020 2020 2020 2020 2020  png',.          
-00023a10: 2020 2020 2020 2020 2020 2020 7665 7262              verb
-00023a20: 6f73 653a 2062 6f6f 6c20 3d20 5472 7565  ose: bool = True
-00023a30: 2920 2d3e 2074 7570 6c65 5b70 6c74 2e46  ) -> tuple[plt.F
-00023a40: 6967 7572 652c 2070 6c74 2e41 7865 735d  igure, plt.Axes]
-00023a50: 3a0a 2020 2020 2727 270a 2020 2020 506c  :.    '''.    Pl
-00023a60: 6f74 7320 6578 7065 7269 6d65 6e74 616c  ots experimental
-00023a70: 2061 6e64 2066 6974 7465 6420 286d 6f64   and fitted (mod
-00023a80: 656c 2920 7265 6c61 7861 7469 6f6e 2072  el) relaxation r
-00023a90: 6174 6520 6173 5c6e 0a20 2020 2072 6174  ate as\n.    rat
-00023aa0: 6520 7673 2078 7661 7220 7768 6572 6520  e vs xvar where 
-00023ab0: 7876 6172 2069 7320 5420 6f72 2048 2e20  xvar is T or H. 
-00023ac0: 5769 7468 206c 6f67 206c 6f67 2073 6361  With log log sca
-00023ad0: 6c65 2e0a 0a20 2020 2050 6172 616d 6574  le...    Paramet
-00023ae0: 6572 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ers.    --------
-00023af0: 2d2d 0a20 2020 2064 6174 6173 6574 3a20  --.    dataset: 
-00023b00: 5461 7554 4461 7461 7365 7420 7c20 5461  TauTDataset | Ta
-00023b10: 7548 4461 7461 7365 740a 2020 2020 2020  uHDataset.      
-00023b20: 2020 4461 7461 7365 7420 746f 2070 6c6f    Dataset to plo
-00023b30: 740a 2020 2020 6d6f 6465 6c3a 204c 6f67  t.    model: Log
-00023b40: 5461 7554 4d6f 6465 6c20 7c20 4d75 6c74  TauTModel | Mult
-00023b50: 694c 6f67 5461 7554 4d6f 6465 6c20 7c20  iLogTauTModel | 
-00023b60: 4c6f 6754 6175 484d 6f64 656c 207c 204d  LogTauHModel | M
-00023b70: 756c 7469 4c6f 6754 6175 484d 6f64 656c  ultiLogTauHModel
-00023b80: 0a20 2020 2020 2020 204d 6f64 656c 2028  .        Model (
-00023b90: 6669 7474 6564 2920 746f 2070 6c6f 740a  fitted) to plot.
-00023ba0: 2020 2020 7368 6f77 3a20 626f 6f6c 2c20      show: bool, 
-00023bb0: 6465 6661 756c 7420 5472 7565 0a20 2020  default True.   
-00023bc0: 2020 2020 2049 6620 5472 7565 2c20 7368       If True, sh
-00023bd0: 6f77 2070 6c6f 7420 6f6e 2073 6372 6565  ow plot on scree
-00023be0: 6e0a 2020 2020 7361 7665 3a20 626f 6f6c  n.    save: bool
-00023bf0: 2c20 6465 6661 756c 7420 4661 6c73 650a  , default False.
-00023c00: 2020 2020 2020 2020 4966 2054 7275 652c          If True,
-00023c10: 2073 6176 6520 706c 6f74 2074 6f20 6669   save plot to fi
-00023c20: 6c65 2060 7361 7665 5f6e 616d 6560 0a20  le `save_name`. 
-00023c30: 2020 2073 6176 655f 6e61 6d65 3a20 7374     save_name: st
-00023c40: 722c 2064 6566 6175 6c74 203d 2027 6669  r, default = 'fi
-00023c50: 7474 6564 5f72 6174 6573 2e70 6e67 270a  tted_rates.png'.
-00023c60: 2020 2020 2020 2020 4966 2073 6176 6520          If save 
-00023c70: 6973 2054 7275 652c 2077 696c 6c20 7361  is True, will sa
-00023c80: 7665 2070 6c6f 7420 746f 2074 6869 7320  ve plot to this 
-00023c90: 6669 6c65 6e61 6d65 0a20 2020 2076 6572  filename.    ver
-00023ca0: 626f 7365 3a20 626f 6f6c 2c20 6465 6661  bose: bool, defa
-00023cb0: 756c 7420 5472 7565 0a20 2020 2020 2020  ult True.       
-00023cc0: 2049 6620 5472 7565 2c20 706c 6f74 2066   If True, plot f
-00023cd0: 696c 6520 6c6f 6361 7469 6f6e 2069 7320  ile location is 
-00023ce0: 7772 6974 7465 6e20 746f 2074 6572 6d69  written to termi
-00023cf0: 6e61 6c0a 2020 2020 5265 7475 726e 730a  nal.    Returns.
-00023d00: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-00023d10: 706c 742e 4669 6775 7265 0a20 2020 2020  plt.Figure.     
-00023d20: 2020 204d 6174 706c 6f74 6c69 6220 6669     Matplotlib fi
-00023d30: 6775 7265 206f 626a 6563 740a 2020 2020  gure object.    
-00023d40: 706c 742e 4178 6573 0a20 2020 2020 2020  plt.Axes.       
-00023d50: 204d 6174 706c 6f74 6c69 6220 6178 6973   Matplotlib axis
-00023d60: 206f 626a 6563 740a 2020 2020 2727 270a   object.    '''.
-00023d70: 0a20 2020 2023 2043 7265 6174 6520 6669  .    # Create fi
-00023d80: 6775 7265 2061 6e64 2061 7865 730a 2020  gure and axes.  
-00023d90: 2020 6669 672c 2061 7820 3d20 706c 742e    fig, ax = plt.
-00023da0: 7375 6270 6c6f 7473 280a 2020 2020 2020  subplots(.      
-00023db0: 2020 312c 0a20 2020 2020 2020 2031 2c0a    1,.        1,.
-00023dc0: 2020 2020 2020 2020 7368 6172 6578 3d54          sharex=T
-00023dd0: 7275 652c 0a20 2020 2020 2020 2073 6861  rue,.        sha
-00023de0: 7265 793d 5472 7565 2c0a 2020 2020 2020  rey=True,.      
-00023df0: 2020 6669 6773 697a 653d 2836 2c20 3629    figsize=(6, 6)
-00023e00: 2c0a 2020 2020 2020 2020 6e75 6d3d 2746  ,.        num='F
-00023e10: 6974 7465 6420 7265 6c61 7861 7469 6f6e  itted relaxation
-00023e20: 2070 726f 6669 6c65 270a 2020 2020 290a   profile'.    ).
-00023e30: 0a20 2020 205f 706c 6f74 5f66 6974 7465  .    _plot_fitte
-00023e40: 645f 7261 7465 7328 6461 7461 7365 742c  d_rates(dataset,
-00023e50: 206d 6f64 656c 2c20 6669 672c 2061 7829   model, fig, ax)
-00023e60: 0a0a 2020 2020 6669 672e 7469 6768 745f  ..    fig.tight_
-00023e70: 6c61 796f 7574 2829 0a0a 2020 2020 6966  layout()..    if
-00023e80: 2073 686f 773a 0a20 2020 2020 2020 2070   show:.        p
-00023e90: 6c74 2e73 686f 7728 290a 0a20 2020 2069  lt.show()..    i
-00023ea0: 6620 7361 7665 3a0a 2020 2020 2020 2020  f save:.        
-00023eb0: 6669 672e 7361 7665 6669 6728 7361 7665  fig.savefig(save
-00023ec0: 5f6e 616d 652c 2064 7069 3d35 3030 290a  _name, dpi=500).
-00023ed0: 2020 2020 2020 2020 6966 2076 6572 626f          if verbo
-00023ee0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00023ef0: 6966 2069 7369 6e73 7461 6e63 6528 6461  if isinstance(da
-00023f00: 7461 7365 742c 2028 5461 7554 4461 7461  taset, (TauTData
-00023f10: 7365 7429 293a 0a20 2020 2020 2020 2020  set)):.         
-00023f20: 2020 2020 2020 205f 7876 6172 203d 2027         _xvar = '
-00023f30: 5427 0a20 2020 2020 2020 2020 2020 2065  T'.            e
-00023f40: 6c69 6620 6973 696e 7374 616e 6365 2864  lif isinstance(d
-00023f50: 6174 6173 6574 2c20 2854 6175 4844 6174  ataset, (TauHDat
-00023f60: 6173 6574 2929 3a0a 2020 2020 2020 2020  aset)):.        
-00023f70: 2020 2020 2020 2020 5f78 7661 7220 3d20          _xvar = 
-00023f80: 2748 270a 2020 2020 2020 2020 2020 2020  'H'.            
-00023f90: 7574 2e63 7072 696e 7428 0a20 2020 2020  ut.cprint(.     
-00023fa0: 2020 2020 2020 2020 2020 2066 275c 6e20             f'\n 
-00023fb0: 4669 7474 6564 20cf 84e2 81bb c2b9 2076  Fitted ....... v
-00023fc0: 7320 7b5f 7876 6172 7d20 706c 6f74 2073  s {_xvar} plot s
-00023fd0: 6176 6564 2074 6f20 5c6e 207b 7361 7665  aved to \n {save
-00023fe0: 5f6e 616d 657d 5c6e 272c 0a20 2020 2020  _name}\n',.     
-00023ff0: 2020 2020 2020 2020 2020 2027 6379 616e             'cyan
-00024000: 270a 2020 2020 2020 2020 2020 2020 290a  '.            ).
-00024010: 0a20 2020 2072 6574 7572 6e20 6669 672c  .    return fig,
-00024020: 2061 780a 0a0a 6465 6620 7174 5f70 6c6f   ax...def qt_plo
-00024030: 745f 6669 7474 6564 5f72 6174 6573 2861  t_fitted_rates(a
-00024040: 7070 3a20 5174 5769 6467 6574 732e 5141  pp: QtWidgets.QA
-00024050: 7070 6c69 6361 7469 6f6e 2c0a 2020 2020  pplication,.    
-00024060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024070: 2020 2020 2064 6174 6173 6574 3a20 5461       dataset: Ta
-00024080: 7554 4461 7461 7365 7420 7c20 5461 7548  uTDataset | TauH
-00024090: 4461 7461 7365 742c 0a20 2020 2020 2020  Dataset,.       
-000240a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000240b0: 2020 6d6f 6465 6c3a 204c 6f67 5461 7554    model: LogTauT
-000240c0: 4d6f 6465 6c20 7c20 4d75 6c74 694c 6f67  Model | MultiLog
-000240d0: 5461 7554 4d6f 6465 6c20 7c20 4c6f 6754  TauTModel | LogT
-000240e0: 6175 484d 6f64 656c 207c 204d 756c 7469  auHModel | Multi
-000240f0: 4c6f 6754 6175 484d 6f64 656c 2c20 2320  LogTauHModel, # 
-00024100: 6e6f 7161 0a20 2020 2020 2020 2020 2020  noqa.           
-00024110: 2020 2020 2020 2020 2020 2020 2020 7361                sa
-00024120: 7665 3a20 626f 6f6c 203d 2046 616c 7365  ve: bool = False
-00024130: 2c20 7368 6f77 3a20 626f 6f6c 203d 2054  , show: bool = T
-00024140: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
-00024150: 2020 2020 2020 2020 2020 2020 2020 7361                sa
-00024160: 7665 5f6e 616d 653a 2073 7472 203d 2027  ve_name: str = '
-00024170: 6669 7474 6564 5f72 6174 6573 2e70 6e67  fitted_rates.png
-00024180: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
-00024190: 2020 2020 2020 2020 2020 2020 7665 7262              verb
-000241a0: 6f73 653a 2062 6f6f 6c20 3d20 5472 7565  ose: bool = True
-000241b0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2027  ) -> None:.    '
-000241c0: 2727 0a20 2020 2050 6c6f 7473 2065 7870  ''.    Plots exp
-000241d0: 6572 696d 656e 7461 6c20 616e 6420 6669  erimental and fi
-000241e0: 7474 6564 2028 6d6f 6465 6c29 2072 656c  tted (model) rel
-000241f0: 6178 6174 696f 6e20 7261 7465 2061 735c  axation rate as\
-00024200: 6e0a 2020 2020 7261 7465 2076 7320 7876  n.    rate vs xv
-00024210: 6172 2077 6865 7265 2078 7661 7220 6973  ar where xvar is
-00024220: 2054 206f 7220 482e 2057 6974 6820 6c6f   T or H. With lo
-00024230: 6720 6c6f 6720 7363 616c 652e 0a0a 2020  g log scale...  
-00024240: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
-00024250: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-00024260: 6461 7461 7365 743a 2054 6175 5444 6174  dataset: TauTDat
-00024270: 6173 6574 207c 2054 6175 4844 6174 6173  aset | TauHDatas
-00024280: 6574 0a20 2020 2020 2020 2044 6174 6173  et.        Datas
-00024290: 6574 2074 6f20 706c 6f74 0a20 2020 206d  et to plot.    m
-000242a0: 6f64 656c 3a20 4c6f 6754 6175 544d 6f64  odel: LogTauTMod
-000242b0: 656c 207c 204d 756c 7469 4c6f 6754 6175  el | MultiLogTau
-000242c0: 544d 6f64 656c 207c 204c 6f67 5461 7548  TModel | LogTauH
-000242d0: 4d6f 6465 6c20 7c20 4d75 6c74 694c 6f67  Model | MultiLog
-000242e0: 5461 7548 4d6f 6465 6c0a 2020 2020 2020  TauHModel.      
-000242f0: 2020 4d6f 6465 6c20 2866 6974 7465 6429    Model (fitted)
-00024300: 2074 6f20 706c 6f74 0a20 2020 2073 686f   to plot.    sho
-00024310: 773a 2062 6f6f 6c2c 2064 6566 6175 6c74  w: bool, default
-00024320: 2054 7275 650a 2020 2020 2020 2020 4966   True.        If
-00024330: 2054 7275 652c 2073 686f 7720 706c 6f74   True, show plot
-00024340: 206f 6e20 7363 7265 656e 0a20 2020 2073   on screen.    s
-00024350: 6176 653a 2062 6f6f 6c2c 2064 6566 6175  ave: bool, defau
-00024360: 6c74 2046 616c 7365 0a20 2020 2020 2020  lt False.       
-00024370: 2049 6620 5472 7565 2c20 7361 7665 2070   If True, save p
-00024380: 6c6f 7420 746f 2066 696c 6520 6073 6176  lot to file `sav
-00024390: 655f 6e61 6d65 600a 2020 2020 7361 7665  e_name`.    save
-000243a0: 5f6e 616d 653a 2073 7472 2c20 6465 6661  _name: str, defa
-000243b0: 756c 7420 2766 6974 7465 645f 7261 7465  ult 'fitted_rate
-000243c0: 732e 706e 6727 0a20 2020 2020 2020 2049  s.png'.        I
-000243d0: 6620 7361 7665 2069 7320 5472 7565 2c20  f save is True, 
-000243e0: 7769 6c6c 2073 6176 6520 706c 6f74 2074  will save plot t
-000243f0: 6f20 7468 6973 2066 696c 656e 616d 650a  o this filename.
-00024400: 2020 2020 7665 7262 6f73 653a 2062 6f6f      verbose: boo
-00024410: 6c2c 2064 6566 6175 6c74 2054 7275 650a  l, default True.
-00024420: 2020 2020 2020 2020 4966 2054 7275 652c          If True,
-00024430: 2070 6c6f 7420 6669 6c65 206c 6f63 6174   plot file locat
-00024440: 696f 6e20 6973 2077 7269 7474 656e 2074  ion is written t
-00024450: 6f20 7465 726d 696e 616c 0a0a 2020 2020  o terminal..    
-00024460: 5265 7475 726e 730a 2020 2020 2d2d 2d2d  Returns.    ----
-00024470: 2d2d 2d0a 2020 2020 4e6f 6e65 0a20 2020  ---.    None.   
-00024480: 2027 2727 0a0a 2020 2020 7769 6e64 6f77   '''..    window
-00024490: 203d 2067 7569 2e4d 6174 706c 6f74 6c69   = gui.Matplotli
-000244a0: 6257 696e 646f 7728 290a 0a20 2020 2077  bWindow()..    w
-000244b0: 696e 646f 772e 7365 7457 696e 646f 7754  indow.setWindowT
-000244c0: 6974 6c65 2827 4669 7474 6564 2072 656c  itle('Fitted rel
-000244d0: 6178 6174 696f 6e20 7072 6f66 696c 6527  axation profile'
-000244e0: 290a 0a20 2020 2023 2041 6464 2070 6c6f  )..    # Add plo
-000244f0: 740a 2020 2020 5f70 6c6f 745f 6669 7474  t.    _plot_fitt
-00024500: 6564 5f72 6174 6573 2864 6174 6173 6574  ed_rates(dataset
-00024510: 2c20 6d6f 6465 6c2c 2077 696e 646f 772e  , model, window.
-00024520: 7363 2e66 6967 2c20 7769 6e64 6f77 2e73  sc.fig, window.s
-00024530: 632e 6178 290a 0a20 2020 2023 2053 6176  c.ax)..    # Sav
-00024540: 6520 706c 6f74 0a20 2020 2069 6620 7361  e plot.    if sa
-00024550: 7665 3a0a 2020 2020 2020 2020 7769 6e64  ve:.        wind
-00024560: 6f77 2e73 632e 6669 672e 7361 7665 6669  ow.sc.fig.savefi
-00024570: 6728 7361 7665 5f6e 616d 652c 2064 7069  g(save_name, dpi
-00024580: 3d33 3030 290a 2020 2020 2020 2020 6966  =300).        if
-00024590: 2076 6572 626f 7365 3a0a 2020 2020 2020   verbose:.      
-000245a0: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
-000245b0: 6e63 6528 6461 7461 7365 742c 2028 5461  nce(dataset, (Ta
-000245c0: 7554 4461 7461 7365 7429 293a 0a20 2020  uTDataset)):.   
-000245d0: 2020 2020 2020 2020 2020 2020 205f 7876               _xv
-000245e0: 6172 203d 2027 5427 0a20 2020 2020 2020  ar = 'T'.       
-000245f0: 2020 2020 2065 6c69 6620 6973 696e 7374       elif isinst
-00024600: 616e 6365 2864 6174 6173 6574 2c20 2854  ance(dataset, (T
-00024610: 6175 4844 6174 6173 6574 2929 3a0a 2020  auHDataset)):.  
-00024620: 2020 2020 2020 2020 2020 2020 2020 5f78                _x
-00024630: 7661 7220 3d20 2748 270a 2020 2020 2020  var = 'H'.      
-00024640: 2020 2020 2020 7574 2e63 7072 696e 7428        ut.cprint(
-00024650: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00024660: 2066 275c 6e20 4669 7474 6564 20cf 84e2   f'\n Fitted ...
-00024670: 81bb c2b9 2076 7320 7b5f 7876 6172 7d20  .... vs {_xvar} 
-00024680: 706c 6f74 2073 6176 6564 2074 6f20 5c6e  plot saved to \n
-00024690: 207b 7361 7665 5f6e 616d 657d 5c6e 272c   {save_name}\n',
-000246a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000246b0: 2027 6379 616e 270a 2020 2020 2020 2020   'cyan'.        
-000246c0: 2020 2020 290a 0a20 2020 2069 6620 7368      )..    if sh
-000246d0: 6f77 3a0a 2020 2020 2020 2020 7769 6e64  ow:.        wind
-000246e0: 6f77 2e73 686f 7728 290a 2020 2020 2020  ow.show().      
-000246f0: 2020 2320 4361 6c6c 2074 7769 6365 2065    # Call twice e
-00024700: 6c73 6520 6974 2077 6f6e 7420 776f 726b  lse it wont work
-00024710: 210a 2020 2020 2020 2020 7769 6e64 6f77  !.        window
-00024720: 2e73 632e 6669 672e 7469 6768 745f 6c61  .sc.fig.tight_la
-00024730: 796f 7574 2829 0a20 2020 2020 2020 2077  yout().        w
-00024740: 696e 646f 772e 7363 2e66 6967 2e74 6967  indow.sc.fig.tig
-00024750: 6874 5f6c 6179 6f75 7428 290a 2020 2020  ht_layout().    
-00024760: 2020 2020 6170 702e 6578 6563 5f28 290a      app.exec_().
-00024770: 0a20 2020 2072 6574 7572 6e0a 0a0a 6465  .    return...de
-00024780: 6620 5f70 6c6f 745f 6669 7474 6564 5f72  f _plot_fitted_r
-00024790: 6174 6573 2864 6174 6173 6574 3a20 5461  ates(dataset: Ta
-000247a0: 7554 4461 7461 7365 7420 7c20 5461 7548  uTDataset | TauH
-000247b0: 4461 7461 7365 742c 0a20 2020 2020 2020  Dataset,.       
-000247c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000247d0: 6d6f 6465 6c3a 204c 6f67 5461 7554 4d6f  model: LogTauTMo
-000247e0: 6465 6c20 7c20 4d75 6c74 694c 6f67 5461  del | MultiLogTa
-000247f0: 7554 4d6f 6465 6c20 7c20 4c6f 6754 6175  uTModel | LogTau
-00024800: 484d 6f64 656c 207c 204d 756c 7469 4c6f  HModel | MultiLo
-00024810: 6754 6175 484d 6f64 656c 2c20 2320 6e6f  gTauHModel, # no
-00024820: 7161 0a20 2020 2020 2020 2020 2020 2020  qa.             
-00024830: 2020 2020 2020 2020 2020 6669 673a 2070            fig: p
-00024840: 6c74 2e46 6967 7572 652c 2061 783a 2070  lt.Figure, ax: p
-00024850: 6c74 2e41 7865 7329 3a0a 2020 2020 2727  lt.Axes):.    ''
-00024860: 270a 2020 2020 506c 6f74 7320 6578 7065  '.    Plots expe
-00024870: 7269 6d65 6e74 616c 2061 6e64 2066 6974  rimental and fit
-00024880: 7465 6420 286d 6f64 656c 2920 7265 6c61  ted (model) rela
-00024890: 7861 7469 6f6e 2072 6174 6520 6173 5c6e  xation rate as\n
-000248a0: 0a20 2020 2072 6174 6520 7673 2078 7661  .    rate vs xva
-000248b0: 7220 7768 6572 6520 7876 6172 2069 7320  r where xvar is 
-000248c0: 5420 6f72 2048 2e20 5769 7468 206c 6f67  T or H. With log
-000248d0: 206c 6f67 2073 6361 6c65 2e0a 0a20 2020   log scale...   
-000248e0: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-000248f0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2064  ----------.    d
-00024900: 6174 6173 6574 3a20 5461 7554 4461 7461  ataset: TauTData
-00024910: 7365 7420 7c20 5461 7548 4461 7461 7365  set | TauHDatase
-00024920: 740a 2020 2020 2020 2020 4461 7461 7365  t.        Datase
-00024930: 7420 746f 2070 6c6f 740a 2020 2020 6d6f  t to plot.    mo
-00024940: 6465 6c3a 204c 6f67 5461 7554 4d6f 6465  del: LogTauTMode
-00024950: 6c20 7c20 4d75 6c74 694c 6f67 5461 7554  l | MultiLogTauT
-00024960: 4d6f 6465 6c20 7c20 4c6f 6754 6175 484d  Model | LogTauHM
-00024970: 6f64 656c 207c 204d 756c 7469 4c6f 6754  odel | MultiLogT
-00024980: 6175 484d 6f64 656c 0a20 2020 2020 2020  auHModel.       
-00024990: 204d 6f64 656c 2028 6669 7474 6564 2920   Model (fitted) 
-000249a0: 746f 2070 6c6f 740a 2020 2020 6669 673a  to plot.    fig:
-000249b0: 2070 6c74 2e46 6967 7572 650a 2020 2020   plt.Figure.    
-000249c0: 2020 2020 4d61 7470 6c6f 746c 6962 2046      Matplotlib F
-000249d0: 6967 7572 6520 6f62 6a65 6374 2075 7365  igure object use
-000249e0: 6420 666f 7220 706c 6f74 0a20 2020 2061  d for plot.    a
-000249f0: 783a 2070 6c74 2e41 7865 730a 2020 2020  x: plt.Axes.    
-00024a00: 2020 2020 4d61 7470 6c6f 746c 6962 2041      Matplotlib A
-00024a10: 7869 7320 6f62 6a65 6374 2075 7365 6420  xis object used 
-00024a20: 666f 7220 706c 6f74 0a0a 2020 2020 5265  for plot..    Re
-00024a30: 7475 726e 730a 2020 2020 2d2d 2d2d 2d2d  turns.    ------
-00024a40: 2d0a 2020 2020 4e6f 6e65 0a20 2020 2027  -.    None.    '
-00024a50: 2727 0a0a 2020 2020 6966 2069 7369 6e73  ''..    if isins
-00024a60: 7461 6e63 6528 6461 7461 7365 742c 2054  tance(dataset, T
-00024a70: 6175 4844 6174 6173 6574 293a 0a20 2020  auHDataset):.   
-00024a80: 2020 2020 2078 5f76 6172 7320 3d20 6461       x_vars = da
-00024a90: 7461 7365 742e 6669 656c 6473 0a20 2020  taset.fields.   
-00024aa0: 2020 2020 2061 782e 7365 745f 786c 6162       ax.set_xlab
-00024ab0: 656c 2872 2746 6965 6c64 2028 4f65 2927  el(r'Field (Oe)'
-00024ac0: 290a 2020 2020 656c 6966 2069 7369 6e73  ).    elif isins
-00024ad0: 7461 6e63 6528 6461 7461 7365 742c 2054  tance(dataset, T
-00024ae0: 6175 5444 6174 6173 6574 293a 0a20 2020  auTDataset):.   
-00024af0: 2020 2020 2078 5f76 6172 7320 3d20 6461       x_vars = da
-00024b00: 7461 7365 742e 7465 6d70 6572 6174 7572  taset.temperatur
-00024b10: 6573 0a20 2020 2020 2020 2061 782e 7365  es.        ax.se
-00024b20: 745f 786c 6162 656c 2872 2754 656d 7065  t_xlabel(r'Tempe
-00024b30: 7261 7475 7265 2028 4b29 2729 0a0a 2020  rature (K)')..  
-00024b40: 2020 2320 4164 6420 756e 6365 7274 6169    # Add uncertai
-00024b50: 6e74 6965 7320 6173 2065 7272 6f72 6261  nties as errorba
-00024b60: 7273 0a20 2020 2069 6620 6c65 6e28 6461  rs.    if len(da
-00024b70: 7461 7365 742e 7261 7465 5f70 6d29 3a0a  taset.rate_pm):.
-00024b80: 2020 2020 2020 2020 6178 2e65 7272 6f72          ax.error
-00024b90: 6261 7228 0a20 2020 2020 2020 2020 2020  bar(.           
-00024ba0: 2078 5f76 6172 732c 0a20 2020 2020 2020   x_vars,.       
-00024bb0: 2020 2020 2064 6174 6173 6574 2e72 6174       dataset.rat
-00024bc0: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
-00024bd0: 7965 7272 3d64 6174 6173 6574 2e72 6174  yerr=dataset.rat
-00024be0: 655f 706d 2c0a 2020 2020 2020 2020 2020  e_pm,.          
-00024bf0: 2020 6d61 726b 6572 3d27 6f27 2c0a 2020    marker='o',.  
-00024c00: 2020 2020 2020 2020 2020 6c77 3d30 2c0a            lw=0,.
-00024c10: 2020 2020 2020 2020 2020 2020 656c 696e              elin
-00024c20: 6577 6964 7468 3d31 2e35 2c0a 2020 2020  ewidth=1.5,.    
-00024c30: 2020 2020 2020 2020 6669 6c6c 7374 796c          fillstyl
-00024c40: 653d 276e 6f6e 6527 2c0a 2020 2020 2020  e='none',.      
-00024c50: 2020 2020 2020 6c61 6265 6c3d 2745 7870        label='Exp
-00024c60: 6572 696d 656e 7427 2c0a 2020 2020 2020  eriment',.      
-00024c70: 2020 2020 2020 636f 6c6f 723d 2762 6c61        color='bla
-00024c80: 636b 270a 2020 2020 2020 2020 290a 2020  ck'.        ).  
-00024c90: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00024ca0: 6178 2e70 6c6f 7428 0a20 2020 2020 2020  ax.plot(.       
-00024cb0: 2020 2020 2078 5f76 6172 732c 0a20 2020       x_vars,.   
-00024cc0: 2020 2020 2020 2020 2064 6174 6173 6574           dataset
-00024cd0: 2e72 6174 6573 2c0a 2020 2020 2020 2020  .rates,.        
-00024ce0: 2020 2020 6d61 726b 6572 3d27 6f27 2c0a      marker='o',.
-00024cf0: 2020 2020 2020 2020 2020 2020 6c77 3d30              lw=0
-00024d00: 2c0a 2020 2020 2020 2020 2020 2020 6669  ,.            fi
-00024d10: 6c6c 7374 796c 653d 276e 6f6e 6527 2c0a  llstyle='none',.
-00024d20: 2020 2020 2020 2020 2020 2020 6c61 6265              labe
-00024d30: 6c3d 2745 7870 6572 696d 656e 7427 2c0a  l='Experiment',.
-00024d40: 2020 2020 2020 2020 2020 2020 636f 6c6f              colo
-00024d50: 723d 2762 6c61 636b 270a 2020 2020 2020  r='black'.      
-00024d60: 2020 290a 0a20 2020 2078 5f76 6172 735f    )..    x_vars_
-00024d70: 6772 6964 203d 206e 702e 6c6f 6773 7061  grid = np.logspa
-00024d80: 6365 280a 2020 2020 2020 2020 6e70 2e6c  ce(.        np.l
-00024d90: 6f67 3130 286e 702e 6d69 6e28 785f 7661  og10(np.min(x_va
-00024da0: 7273 2929 2c0a 2020 2020 2020 2020 6e70  rs)),.        np
-00024db0: 2e6c 6f67 3130 286e 702e 6d61 7828 785f  .log10(np.max(x_
-00024dc0: 7661 7273 2929 2c0a 2020 2020 2020 2020  vars)),.        
-00024dd0: 3530 300a 2020 2020 290a 0a20 2020 2069  500.    )..    i
-00024de0: 6620 7479 7065 286d 6f64 656c 2920 696e  f type(model) in
-00024df0: 205b 4d75 6c74 694c 6f67 5461 7554 4d6f   [MultiLogTauTMo
-00024e00: 6465 6c2c 204d 756c 7469 4c6f 6754 6175  del, MultiLogTau
-00024e10: 484d 6f64 656c 5d3a 0a20 2020 2020 2020  HModel]:.       
-00024e20: 206c 6f67 6d6f 6465 6c73 203d 206d 6f64   logmodels = mod
-00024e30: 656c 2e6c 6f67 6d6f 6465 6c73 0a20 2020  el.logmodels.   
-00024e40: 2065 6c73 653a 0a20 2020 2020 2020 206c   else:.        l
-00024e50: 6f67 6d6f 6465 6c73 203d 205b 6d6f 6465  ogmodels = [mode
-00024e60: 6c5d 0a0a 2020 2020 666f 7220 6c6f 676d  l]..    for logm
-00024e70: 6f64 656c 2069 6e20 6c6f 676d 6f64 656c  odel in logmodel
-00024e80: 733a 0a0a 2020 2020 2020 2020 6966 2074  s:..        if t
-00024e90: 7970 6528 6c6f 676d 6f64 656c 2920 6973  ype(logmodel) is
-00024ea0: 204c 6f67 4f72 6261 6368 4d6f 6465 6c3a   LogOrbachModel:
-00024eb0: 0a20 2020 2020 2020 2020 2020 206c 6162  .            lab
-00024ec0: 656c 5f66 6974 203d 2027 5c6e 4669 7420  el_fit = '\nFit 
-00024ed0: 7769 7468 270a 2020 2020 2020 2020 2020  with'.          
-00024ee0: 2020 6c61 6265 6c5f 6669 7420 2b3d 2027    label_fit += '
-00024ef0: 5c6e 2720 2b20 7227 7b7d 207b 3a36 2e32  \n' + r'{} {:6.2
-00024f00: 667d 2073 272e 666f 726d 6174 280a 2020  f} s'.format(.  
-00024f10: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-00024f20: 676d 6f64 656c 2e56 4152 4e41 4d45 535f  gmodel.VARNAMES_
-00024f30: 4d4d 5b27 755f 6566 6627 5d2c 0a20 2020  MM['u_eff'],.   
-00024f40: 2020 2020 2020 2020 2020 2020 206c 6f67               log
-00024f50: 6d6f 6465 6c2e 6669 6e61 6c5f 7661 725f  model.final_var_
-00024f60: 7661 6c75 6573 5b27 755f 6566 6627 5d0a  values['u_eff'].
-00024f70: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00024f80: 2020 2020 2020 2020 2020 6c61 6265 6c5f            label_
-00024f90: 6669 7420 2b3d 2027 5c6e 2720 2b20 7227  fit += '\n' + r'
-00024fa0: 7b7d 207b 3a30 342e 3365 7d27 2e66 6f72  {} {:04.3e}'.for
-00024fb0: 6d61 7428 0a20 2020 2020 2020 2020 2020  mat(.           
-00024fc0: 2020 2020 206c 6f67 6d6f 6465 6c2e 5641       logmodel.VA
-00024fd0: 524e 414d 4553 5f4d 4d5b 2741 275d 2c20  RNAMES_MM['A'], 
-00024fe0: 6c6f 676d 6f64 656c 2e66 696e 616c 5f76  logmodel.final_v
-00024ff0: 6172 5f76 616c 7565 735b 2741 275d 0a20  ar_values['A']. 
-00025000: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00025010: 2020 2020 2065 6c69 6620 7479 7065 286c       elif type(l
-00025020: 6f67 6d6f 6465 6c29 2069 7320 4c6f 6752  ogmodel) is LogR
-00025030: 616d 616e 4d6f 6465 6c3a 0a20 2020 2020  amanModel:.     
-00025040: 2020 2020 2020 206c 6162 656c 5f66 6974         label_fit
-00025050: 203d 2027 5c6e 4669 7420 7769 7468 270a   = '\nFit with'.
-00025060: 2020 2020 2020 2020 2020 2020 6c61 6265              labe
-00025070: 6c5f 6669 7420 2b3d 2027 5c6e 2720 2b20  l_fit += '\n' + 
-00025080: 7227 7b7d 207b 3a36 2e32 667d 2073 272e  r'{} {:6.2f} s'.
-00025090: 666f 726d 6174 280a 2020 2020 2020 2020  format(.        
-000250a0: 2020 2020 2020 2020 6c6f 676d 6f64 656c          logmodel
-000250b0: 2e56 4152 4e41 4d45 535f 4d4d 5b27 5227  .VARNAMES_MM['R'
-000250c0: 5d2c 206c 6f67 6d6f 6465 6c2e 6669 6e61  ], logmodel.fina
-000250d0: 6c5f 7661 725f 7661 6c75 6573 5b27 5227  l_var_values['R'
-000250e0: 5d0a 2020 2020 2020 2020 2020 2020 290a  ].            ).
-000250f0: 2020 2020 2020 2020 2020 2020 6c61 6265              labe
-00025100: 6c5f 6669 7420 2b3d 2027 5c6e 2720 2b20  l_fit += '\n' + 
-00025110: 7227 7b7d 207b 3a30 342e 3365 7d27 2e66  r'{} {:04.3e}'.f
-00025120: 6f72 6d61 7428 0a20 2020 2020 2020 2020  ormat(.         
-00025130: 2020 2020 2020 206c 6f67 6d6f 6465 6c2e         logmodel.
-00025140: 5641 524e 414d 4553 5f4d 4d5b 276e 275d  VARNAMES_MM['n']
-00025150: 2c20 6c6f 676d 6f64 656c 2e66 696e 616c  , logmodel.final
-00025160: 5f76 6172 5f76 616c 7565 735b 276e 275d  _var_values['n']
-00025170: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-00025180: 2020 2020 2020 2065 6c69 6620 7479 7065         elif type
-00025190: 286c 6f67 6d6f 6465 6c29 2069 7320 4c6f  (logmodel) is Lo
-000251a0: 6751 544d 4d6f 6465 6c3a 0a20 2020 2020  gQTMModel:.     
-000251b0: 2020 2020 2020 206c 6162 656c 5f66 6974         label_fit
-000251c0: 203d 2027 5c6e 4669 7420 7769 7468 270a   = '\nFit with'.
-000251d0: 2020 2020 2020 2020 2020 2020 6c61 6265              labe
-000251e0: 6c5f 6669 7420 2b3d 2027 5c6e 2720 2b20  l_fit += '\n' + 
-000251f0: 7227 7b7d 207b 3a36 2e32 667d 2073 272e  r'{} {:6.2f} s'.
-00025200: 666f 726d 6174 280a 2020 2020 2020 2020  format(.        
-00025210: 2020 2020 2020 2020 6c6f 676d 6f64 656c          logmodel
-00025220: 2e56 4152 4e41 4d45 535f 4d4d 5b27 5127  .VARNAMES_MM['Q'
-00025230: 5d2c 206c 6f67 6d6f 6465 6c2e 6669 6e61  ], logmodel.fina
-00025240: 6c5f 7661 725f 7661 6c75 6573 5b27 5127  l_var_values['Q'
-00025250: 5d0a 2020 2020 2020 2020 2020 2020 290a  ].            ).
-00025260: 2020 2020 2020 2020 656c 6966 2074 7970          elif typ
-00025270: 6528 6c6f 676d 6f64 656c 2920 6973 204c  e(logmodel) is L
-00025280: 6f67 4469 7265 6374 4d6f 6465 6c3a 0a20  ogDirectModel:. 
-00025290: 2020 2020 2020 2020 2020 206c 6162 656c             label
-000252a0: 5f66 6974 203d 2027 5c6e 4669 7420 7769  _fit = '\nFit wi
-000252b0: 7468 270a 2020 2020 2020 2020 2020 2020  th'.            
-000252c0: 6c61 6265 6c5f 6669 7420 2b3d 2027 5c6e  label_fit += '\n
-000252d0: 2720 2b20 7227 7b7d 207b 3a36 2e32 667d  ' + r'{} {:6.2f}
-000252e0: 2073 272e 666f 726d 6174 280a 2020 2020   s'.format(.    
-000252f0: 2020 2020 2020 2020 2020 2020 6c6f 676d              logm
-00025300: 6f64 656c 2e56 4152 4e41 4d45 535f 4d4d  odel.VARNAMES_MM
-00025310: 5b27 4427 5d2c 206c 6f67 6d6f 6465 6c2e  ['D'], logmodel.
-00025320: 6669 6e61 6c5f 7661 725f 7661 6c75 6573  final_var_values
-00025330: 5b27 4427 5d0a 2020 2020 2020 2020 2020  ['D'].          
-00025340: 2020 290a 2020 2020 2020 2020 6d6f 6465    ).        mode
-00025350: 6c5f 7261 7465 7320 3d20 3130 2a2a 6c6f  l_rates = 10**lo
-00025360: 676d 6f64 656c 2e6d 6f64 656c 280a 2020  gmodel.model(.  
-00025370: 2020 2020 2020 2020 2020 6c6f 676d 6f64            logmod
-00025380: 656c 2e66 696e 616c 5f76 6172 5f76 616c  el.final_var_val
-00025390: 7565 732c 0a20 2020 2020 2020 2020 2020  ues,.           
-000253a0: 2078 5f76 6172 735f 6772 6964 2c0a 2020   x_vars_grid,.  
-000253b0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-000253c0: 2023 2054 7269 6d20 6d6f 6465 6c20 7261   # Trim model ra
-000253d0: 7465 7320 746f 2073 656e 7369 626c 6520  tes to sensible 
-000253e0: 7661 6c75 6573 0a20 2020 2020 2020 2076  values.        v
-000253f0: 616c 6964 5f69 6e74 203d 206e 702e 7768  alid_int = np.wh
-00025400: 6572 6528 6d6f 6465 6c5f 7261 7465 7320  ere(model_rates 
-00025410: 3e20 3145 2d36 295b 305d 0a0a 2020 2020  > 1E-6)[0]..    
-00025420: 2020 2020 6178 2e70 6c6f 7428 0a20 2020      ax.plot(.   
-00025430: 2020 2020 2020 2020 206e 702e 6172 7261           np.arra
-00025440: 7928 785f 7661 7273 5f67 7269 6429 5b76  y(x_vars_grid)[v
-00025450: 616c 6964 5f69 6e74 5d2c 0a20 2020 2020  alid_int],.     
-00025460: 2020 2020 2020 206e 702e 6172 7261 7928         np.array(
-00025470: 6d6f 6465 6c5f 7261 7465 7329 5b76 616c  model_rates)[val
-00025480: 6964 5f69 6e74 5d2c 0a20 2020 2020 2020  id_int],.       
-00025490: 2020 2020 206c 773d 312e 352c 0a20 2020       lw=1.5,.   
-000254a0: 2020 2020 2020 2020 206c 6162 656c 3d6c           label=l
-000254b0: 6f67 6d6f 6465 6c2e 4e41 4d45 2c0a 2020  ogmodel.NAME,.  
-000254c0: 2020 2020 2020 2020 2020 6c73 3d27 2d2d            ls='--
-000254d0: 270a 2020 2020 2020 2020 290a 0a20 2020  '.        )..   
-000254e0: 2069 6620 7479 7065 286d 6f64 656c 2920   if type(model) 
-000254f0: 696e 205b 4d75 6c74 694c 6f67 5461 7554  in [MultiLogTauT
-00025500: 4d6f 6465 6c2c 204d 756c 7469 4c6f 6754  Model, MultiLogT
-00025510: 6175 484d 6f64 656c 5d20 616e 6420 6c65  auHModel] and le
-00025520: 6e28 6c6f 676d 6f64 656c 7329 203e 2031  n(logmodels) > 1
-00025530: 3a20 2320 6e6f 7161 0a20 2020 2020 2020  : # noqa.       
-00025540: 2074 6f74 616c 203d 206e 702e 7a65 726f   total = np.zero
-00025550: 7328 6c65 6e28 785f 7661 7273 5f67 7269  s(len(x_vars_gri
-00025560: 6429 290a 0a20 2020 2020 2020 2066 6f72  d))..        for
-00025570: 206c 6f67 6d6f 6465 6c20 696e 206c 6f67   logmodel in log
-00025580: 6d6f 6465 6c73 3a0a 2020 2020 2020 2020  models:.        
-00025590: 2020 2020 746f 7461 6c20 2b3d 2031 302a      total += 10*
-000255a0: 2a6c 6f67 6d6f 6465 6c2e 6d6f 6465 6c28  *logmodel.model(
-000255b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000255c0: 206c 6f67 6d6f 6465 6c2e 6669 6e61 6c5f   logmodel.final_
-000255d0: 7661 725f 7661 6c75 6573 2c0a 2020 2020  var_values,.    
-000255e0: 2020 2020 2020 2020 2020 2020 785f 7661              x_va
-000255f0: 7273 5f67 7269 642c 0a20 2020 2020 2020  rs_grid,.       
-00025600: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-00025610: 6178 2e70 6c6f 7428 0a20 2020 2020 2020  ax.plot(.       
-00025620: 2020 2020 2078 5f76 6172 735f 6772 6964       x_vars_grid
-00025630: 2c0a 2020 2020 2020 2020 2020 2020 746f  ,.            to
-00025640: 7461 6c2c 0a20 2020 2020 2020 2020 2020  tal,.           
-00025650: 206c 773d 312e 352c 0a20 2020 2020 2020   lw=1.5,.       
-00025660: 2020 2020 206c 6162 656c 3d27 546f 7461       label='Tota
-00025670: 6c27 2c0a 2020 2020 2020 2020 2020 2020  l',.            
-00025680: 636f 6c6f 723d 2772 6564 270a 2020 2020  color='red'.    
-00025690: 2020 2020 290a 0a20 2020 2061 782e 7365      )..    ax.se
-000256a0: 745f 7873 6361 6c65 2827 6c6f 6727 290a  t_xscale('log').
-000256b0: 2020 2020 6178 2e73 6574 5f79 7363 616c      ax.set_yscal
-000256c0: 6528 276c 6f67 2729 0a0a 2020 2020 6775  e('log')..    gu
-000256d0: 692e 666f 726d 6174 5f72 6174 655f 785f  i.format_rate_x_
-000256e0: 795f 6178 6573 280a 2020 2020 2020 2020  y_axes(.        
-000256f0: 6178 2c0a 2020 2020 2020 2020 6461 7461  ax,.        data
-00025700: 7365 742e 7261 7465 732c 0a20 2020 2020  set.rates,.     
-00025710: 2020 2078 5f76 6172 735f 6772 6964 2c0a     x_vars_grid,.
-00025720: 2020 2020 2020 2020 6e70 2e61 6273 2864          np.abs(d
-00025730: 6174 6173 6574 2e72 6174 655f 706d 290a  ataset.rate_pm).
-00025740: 2020 2020 290a 0a20 2020 2065 7870 7265      )..    expre
-00025750: 7373 696f 6e20 3d20 2727 0a0a 2020 2020  ssion = ''..    
-00025760: 666f 7220 6c6f 676d 6f64 656c 2069 6e20  for logmodel in 
-00025770: 6c6f 676d 6f64 656c 733a 0a20 2020 2020  logmodels:.     
-00025780: 2020 2066 6f72 2069 742c 206e 616d 6520     for it, name 
-00025790: 696e 2065 6e75 6d65 7261 7465 286c 6f67  in enumerate(log
-000257a0: 6d6f 6465 6c2e 5041 524e 414d 4553 293a  model.PARNAMES):
-000257b0: 0a20 2020 2020 2020 2020 2020 2065 7870  .            exp
-000257c0: 7265 7373 696f 6e20 2b3d 2027 7b7d 203d  ression += '{} =
-000257d0: 207b 3a2e 3366 7d20 272e 666f 726d 6174   {:.3f} '.format
-000257e0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-000257f0: 2020 6c6f 676d 6f64 656c 2e56 4152 4e41    logmodel.VARNA
-00025800: 4d45 535f 4d4d 5b6e 616d 655d 2c0a 2020  MES_MM[name],.  
-00025810: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-00025820: 676d 6f64 656c 2e66 696e 616c 5f76 6172  gmodel.final_var
-00025830: 5f76 616c 7565 735b 6e61 6d65 5d2c 0a20  _values[name],. 
-00025840: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00025850: 2020 2020 2020 2020 2069 6620 6e61 6d65           if name
-00025860: 2069 6e20 6c6f 676d 6f64 656c 2e66 6974   in logmodel.fit
-00025870: 5f76 6172 732e 6b65 7973 2829 3a0a 2020  _vars.keys():.  
-00025880: 2020 2020 2020 2020 2020 2020 2020 6578                ex
-00025890: 7072 6573 7369 6f6e 202b 3d20 7227 245c  pression += r'$\
-000258a0: 706d 2420 270a 2020 2020 2020 2020 2020  pm$ '.          
-000258b0: 2020 2020 2020 6578 7072 6573 7369 6f6e        expression
-000258c0: 202b 3d20 277b 3a2e 3366 7d20 272e 666f   += '{:.3f} '.fo
-000258d0: 726d 6174 286c 6f67 6d6f 6465 6c2e 6669  rmat(logmodel.fi
-000258e0: 745f 7374 6465 765b 6e61 6d65 5d29 0a20  t_stdev[name]). 
-000258f0: 2020 2020 2020 2020 2020 2065 7870 7265             expre
-00025900: 7373 696f 6e20 2b3d 2027 7b7d 2020 2020  ssion += '{}    
-00025910: 272e 666f 726d 6174 286c 6f67 6d6f 6465  '.format(logmode
-00025920: 6c2e 554e 4954 535f 4d4d 5b6e 616d 655d  l.UNITS_MM[name]
-00025930: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-00025940: 2069 7420 3d3d 2031 2061 6e64 206c 656e   it == 1 and len
-00025950: 286c 6f67 6d6f 6465 6c2e 6669 745f 7661  (logmodel.fit_va
-00025960: 7273 2e6b 6579 7328 2929 203e 2032 3a0a  rs.keys()) > 2:.
-00025970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025980: 6578 7072 6573 7369 6f6e 202b 3d20 275c  expression += '\
-00025990: 6e27 0a20 2020 2020 2020 2065 7870 7265  n'.        expre
-000259a0: 7373 696f 6e20 2b3d 2027 5c6e 270a 0a20  ssion += '\n'.. 
-000259b0: 2020 2061 782e 7465 7874 280a 2020 2020     ax.text(.    
-000259c0: 2020 2020 302e 302c 2031 2e30 322c 2073      0.0, 1.02, s
-000259d0: 3d65 7870 7265 7373 696f 6e2c 2066 6f6e  =expression, fon
-000259e0: 7473 697a 653d 3130 2c20 7472 616e 7366  tsize=10, transf
-000259f0: 6f72 6d3d 6178 2e74 7261 6e73 4178 6573  orm=ax.transAxes
-00025a00: 0a20 2020 2029 0a0a 2020 2020 6178 2e6c  .    )..    ax.l
-00025a10: 6567 656e 6428 0a20 2020 2020 2020 206c  egend(.        l
-00025a20: 6f63 3d27 7570 7065 7220 6c65 6674 272c  oc='upper left',
-00025a30: 2066 6f6e 7473 697a 653d 2731 3027 2c20   fontsize='10', 
-00025a40: 6e75 6d70 6f69 6e74 733d 312c 206e 636f  numpoints=1, nco
-00025a50: 6c3d 312c 2066 7261 6d65 6f6e 3d46 616c  l=1, frameon=Fal
-00025a60: 7365 0a20 2020 2029 0a20 2020 2061 782e  se.    ).    ax.
-00025a70: 7365 745f 796c 6162 656c 2872 2752 6174  set_ylabel(r'Rat
-00025a80: 6520 2873 245e 5c6d 6174 6872 6567 756c  e (s$^\mathregul
-00025a90: 6172 7b2d 317d 2429 2729 0a0a 2020 2020  ar{-1}$)')..    
-00025aa0: 7265 7475 726e 0a0a 0a64 6566 2070 6c6f  return...def plo
-00025ab0: 745f 7261 7465 7328 6461 7461 7365 743a  t_rates(dataset:
-00025ac0: 2054 6175 5444 6174 6173 6574 207c 2054   TauTDataset | T
-00025ad0: 6175 4844 6174 6173 6574 2c20 7368 6f77  auHDataset, show
-00025ae0: 3a20 626f 6f6c 203d 2054 7275 652c 0a20  : bool = True,. 
-00025af0: 2020 2020 2020 2020 2020 2020 2020 7361                sa
-00025b00: 7665 3a20 626f 6f6c 203d 2046 616c 7365  ve: bool = False
-00025b10: 2c20 7361 7665 5f6e 616d 653a 2073 7472  , save_name: str
-00025b20: 203d 2027 7265 6c61 7861 7469 6f6e 5f72   = 'relaxation_r
-00025b30: 6174 6573 2e70 6e67 272c 0a20 2020 2020  ates.png',.     
-00025b40: 2020 2020 2020 2020 2020 7665 7262 6f73            verbos
-00025b50: 653a 2062 6f6f 6c20 3d20 5472 7565 2920  e: bool = True) 
-00025b60: 2d3e 2074 7570 6c65 5b70 6c74 2e46 6967  -> tuple[plt.Fig
-00025b70: 7572 652c 2070 6c74 2e41 7865 735d 3a0a  ure, plt.Axes]:.
-00025b80: 2020 2020 2727 270a 2020 2020 506c 6f74      '''.    Plot
-00025b90: 7320 6578 7065 7269 6d65 6e74 616c 2072  s experimental r
-00025ba0: 656c 6178 6174 696f 6e20 7261 7465 2076  elaxation rate v
-00025bb0: 7320 6669 656c 642f 7465 6d70 6572 6174  s field/temperat
-00025bc0: 7572 6520 616e 640a 2020 2020 6469 7370  ure and.    disp
-00025bd0: 6c61 7973 206f 6e20 7363 7265 656e 2e0a  lays on screen..
-00025be0: 0a20 2020 2050 6172 616d 6574 6572 730a  .    Parameters.
-00025bf0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-00025c00: 2020 2064 6174 6173 6574 3a20 5461 7554     dataset: TauT
-00025c10: 4461 7461 7365 7420 7c20 5461 7548 4461  Dataset | TauHDa
-00025c20: 7461 7365 740a 2020 2020 2020 2020 4461  taset.        Da
-00025c30: 7461 7365 7420 746f 2070 6c6f 740a 2020  taset to plot.  
-00025c40: 2020 7368 6f77 3a20 626f 6f6c 2c20 6465    show: bool, de
-00025c50: 6661 756c 7420 5472 7565 0a20 2020 2020  fault True.     
-00025c60: 2020 2049 6620 5472 7565 2c20 7368 6f77     If True, show
-00025c70: 2070 6c6f 7420 6f6e 2073 6372 6565 6e0a   plot on screen.
-00025c80: 2020 2020 7361 7665 3a20 626f 6f6c 2c20      save: bool, 
-00025c90: 6465 6661 756c 7420 4661 6c73 650a 2020  default False.  
-00025ca0: 2020 2020 2020 4966 2054 7275 652c 2073        If True, s
-00025cb0: 6176 6520 706c 6f74 2074 6f20 6669 6c65  ave plot to file
-00025cc0: 2060 7361 7665 5f6e 616d 6560 0a20 2020   `save_name`.   
-00025cd0: 2073 6176 655f 6e61 6d65 3a20 7374 722c   save_name: str,
-00025ce0: 2064 6566 6175 6c74 2027 7265 6c61 7861   default 'relaxa
-00025cf0: 7469 6f6e 5f72 6174 6573 2e70 6e67 270a  tion_rates.png'.
-00025d00: 2020 2020 2020 2020 4966 2073 6176 6520          If save 
-00025d10: 6973 2054 7275 652c 2077 696c 6c20 7361  is True, will sa
-00025d20: 7665 2070 6c6f 7420 746f 2074 6869 7320  ve plot to this 
-00025d30: 6669 6c65 6e61 6d65 0a20 2020 2076 6572  filename.    ver
-00025d40: 626f 7365 3a20 626f 6f6c 2c20 6465 6661  bose: bool, defa
-00025d50: 756c 7420 5472 7565 0a20 2020 2020 2020  ult True.       
-00025d60: 2049 6620 5472 7565 2c20 706c 6f74 2066   If True, plot f
-00025d70: 696c 6520 6c6f 6361 7469 6f6e 2069 7320  ile location is 
-00025d80: 7772 6974 7465 6e20 746f 2074 6572 6d69  written to termi
-00025d90: 6e61 6c0a 0a20 2020 2052 6574 7572 6e73  nal..    Returns
-00025da0: 0a20 2020 202d 2d2d 2d2d 2d2d 0a20 2020  .    -------.   
-00025db0: 2070 6c74 2e46 6967 7572 650a 2020 2020   plt.Figure.    
-00025dc0: 2020 2020 4d61 7470 6c6f 746c 6962 2066      Matplotlib f
-00025dd0: 6967 7572 6520 6f62 6a65 6374 0a20 2020  igure object.   
-00025de0: 2070 6c74 2e41 7865 730a 2020 2020 2020   plt.Axes.      
-00025df0: 2020 4d61 7470 6c6f 746c 6962 2061 7869    Matplotlib axi
-00025e00: 7320 6f62 6a65 6374 0a20 2020 2027 2727  s object.    '''
-00025e10: 0a0a 2020 2020 2320 4372 6561 7465 2066  ..    # Create f
-00025e20: 6967 7572 6520 616e 6420 6178 6573 0a20  igure and axes. 
-00025e30: 2020 2066 6967 2c20 6178 203d 2070 6c74     fig, ax = plt
-00025e40: 2e73 7562 706c 6f74 7328 0a20 2020 2020  .subplots(.     
-00025e50: 2020 2031 2c0a 2020 2020 2020 2020 312c     1,.        1,
-00025e60: 0a20 2020 2020 2020 2073 6861 7265 783d  .        sharex=
-00025e70: 5472 7565 2c0a 2020 2020 2020 2020 7368  True,.        sh
-00025e80: 6172 6579 3d54 7275 652c 0a20 2020 2020  arey=True,.     
-00025e90: 2020 2066 6967 7369 7a65 3d28 362c 2036     figsize=(6, 6
-00025ea0: 292c 0a20 2020 2020 2020 206e 756d 3d27  ),.        num='
-00025eb0: 4669 7474 6564 2072 656c 6178 6174 696f  Fitted relaxatio
-00025ec0: 6e20 7072 6f66 696c 6527 0a20 2020 2029  n profile'.    )
-00025ed0: 0a0a 2020 2020 6966 2069 7369 6e73 7461  ..    if isinsta
-00025ee0: 6e63 6528 6461 7461 7365 742c 2054 6175  nce(dataset, Tau
-00025ef0: 4844 6174 6173 6574 293a 0a20 2020 2020  HDataset):.     
-00025f00: 2020 2078 5f76 6172 7320 3d20 6461 7461     x_vars = data
-00025f10: 7365 742e 6669 656c 6473 0a20 2020 2020  set.fields.     
-00025f20: 2020 2061 782e 7365 745f 786c 6162 656c     ax.set_xlabel
-00025f30: 2872 2746 6965 6c64 2028 4f65 2927 290a  (r'Field (Oe)').
-00025f40: 2020 2020 656c 6966 2069 7369 6e73 7461      elif isinsta
-00025f50: 6e63 6528 6461 7461 7365 742c 2054 6175  nce(dataset, Tau
-00025f60: 5444 6174 6173 6574 293a 0a20 2020 2020  TDataset):.     
-00025f70: 2020 2078 5f76 6172 7320 3d20 6461 7461     x_vars = data
-00025f80: 7365 742e 7465 6d70 6572 6174 7572 6573  set.temperatures
-00025f90: 0a20 2020 2020 2020 2061 782e 7365 745f  .        ax.set_
-00025fa0: 786c 6162 656c 2872 2754 656d 7065 7261  xlabel(r'Tempera
-00025fb0: 7475 7265 2028 4b29 2729 0a0a 2020 2020  ture (K)')..    
-00025fc0: 2320 4164 6420 756e 6365 7274 6169 6e74  # Add uncertaint
-00025fd0: 6965 7320 6173 2065 7272 6f72 6261 7273  ies as errorbars
-00025fe0: 0a20 2020 2069 6620 6c65 6e28 6461 7461  .    if len(data
-00025ff0: 7365 742e 7261 7465 5f70 6d29 3a0a 2020  set.rate_pm):.  
-00026000: 2020 2020 2020 6178 2e65 7272 6f72 6261        ax.errorba
-00026010: 7228 0a20 2020 2020 2020 2020 2020 2078  r(.            x
-00026020: 5f76 6172 732c 0a20 2020 2020 2020 2020  _vars,.         
-00026030: 2020 2064 6174 6173 6574 2e72 6174 6573     dataset.rates
-00026040: 2c0a 2020 2020 2020 2020 2020 2020 7965  ,.            ye
-00026050: 7272 3d64 6174 6173 6574 2e72 6174 655f  rr=dataset.rate_
-00026060: 706d 2c0a 2020 2020 2020 2020 2020 2020  pm,.            
-00026070: 6d61 726b 6572 3d27 6f27 2c0a 2020 2020  marker='o',.    
-00026080: 2020 2020 2020 2020 6c77 3d30 2c0a 2020          lw=0,.  
-00026090: 2020 2020 2020 2020 2020 656c 696e 6577            elinew
-000260a0: 6964 7468 3d31 2e35 2c0a 2020 2020 2020  idth=1.5,.      
-000260b0: 2020 2020 2020 6669 6c6c 7374 796c 653d        fillstyle=
-000260c0: 276e 6f6e 6527 2c0a 2020 2020 2020 2020  'none',.        
-000260d0: 2020 2020 636f 6c6f 723d 2762 6c61 636b      color='black
-000260e0: 270a 2020 2020 2020 2020 290a 2020 2020  '.        ).    
-000260f0: 656c 7365 3a0a 2020 2020 2020 2020 6178  else:.        ax
-00026100: 2e70 6c6f 7428 0a20 2020 2020 2020 2020  .plot(.         
-00026110: 2020 2078 5f76 6172 732c 0a20 2020 2020     x_vars,.     
-00026120: 2020 2020 2020 2064 6174 6173 6574 2e72         dataset.r
-00026130: 6174 6573 2c0a 2020 2020 2020 2020 2020  ates,.          
-00026140: 2020 6d61 726b 6572 3d27 6f27 2c0a 2020    marker='o',.  
-00026150: 2020 2020 2020 2020 2020 6c77 3d30 2c0a            lw=0,.
-00026160: 2020 2020 2020 2020 2020 2020 6669 6c6c              fill
-00026170: 7374 796c 653d 276e 6f6e 6527 2c0a 2020  style='none',.  
-00026180: 2020 2020 2020 2020 2020 636f 6c6f 723d            color=
-00026190: 2762 6c61 636b 270a 2020 2020 2020 2020  'black'.        
-000261a0: 290a 0a20 2020 2061 782e 7365 745f 7873  )..    ax.set_xs
-000261b0: 6361 6c65 2827 6c6f 6727 290a 2020 2020  cale('log').    
-000261c0: 6178 2e73 6574 5f79 7363 616c 6528 276c  ax.set_yscale('l
-000261d0: 6f67 2729 0a0a 2020 2020 6178 2e73 6574  og')..    ax.set
-000261e0: 5f79 6c61 6265 6c28 7227 5261 7465 2028  _ylabel(r'Rate (
-000261f0: 7324 5e5c 6d61 7468 7265 6775 6c61 727b  s$^\mathregular{
-00026200: 2d31 7d24 2927 290a 0a20 2020 2069 6620  -1}$)')..    if 
-00026210: 6c65 6e28 6461 7461 7365 742e 6c6f 6772  len(dataset.logr
-00026220: 6174 655f 706d 293a 0a20 2020 2020 2020  ate_pm):.       
-00026230: 2061 6c6c 5f64 6174 6120 3d20 5b0a 2020   all_data = [.  
-00026240: 2020 2020 2020 2020 2020 6e70 2e6c 6f67            np.log
-00026250: 3130 2864 6174 6173 6574 2e72 6174 6573  10(dataset.rates
-00026260: 2920 2b20 6461 7461 7365 742e 6c6f 6772  ) + dataset.logr
-00026270: 6174 655f 706d 0a20 2020 2020 2020 205d  ate_pm.        ]
-00026280: 0a20 2020 2020 2020 2061 6c6c 5f64 6174  .        all_dat
-00026290: 6120 2b3d 205b 0a20 2020 2020 2020 2020  a += [.         
-000262a0: 2020 206e 702e 6c6f 6731 3028 6461 7461     np.log10(data
-000262b0: 7365 742e 7261 7465 7329 202d 2064 6174  set.rates) - dat
-000262c0: 6173 6574 2e6c 6f67 7261 7465 5f70 6d0a  aset.lograte_pm.
-000262d0: 2020 2020 2020 2020 5d0a 2020 2020 656c          ].    el
-000262e0: 7365 3a0a 2020 2020 2020 2020 616c 6c5f  se:.        all_
-000262f0: 6461 7461 203d 205b 0a20 2020 2020 2020  data = [.       
-00026300: 2020 2020 206e 702e 6c6f 6731 3028 6461       np.log10(da
-00026310: 7461 7365 742e 7261 7465 7329 0a20 2020  taset.rates).   
-00026320: 2020 2020 205d 0a20 2020 2020 2020 2061       ].        a
-00026330: 6c6c 5f64 6174 6120 2b3d 205b 0a20 2020  ll_data += [.   
-00026340: 2020 2020 2020 2020 206e 702e 6c6f 6731           np.log1
-00026350: 3028 6461 7461 7365 742e 7261 7465 7329  0(dataset.rates)
-00026360: 0a20 2020 2020 2020 205d 0a0a 2020 2020  .        ]..    
-00026370: 6775 692e 666f 726d 6174 5f72 6174 655f  gui.format_rate_
-00026380: 785f 795f 6178 6573 280a 2020 2020 2020  x_y_axes(.      
-00026390: 2020 6178 2c0a 2020 2020 2020 2020 6461    ax,.        da
-000263a0: 7461 7365 742e 7261 7465 732c 0a20 2020  taset.rates,.   
-000263b0: 2020 2020 2078 5f76 6172 732c 0a20 2020       x_vars,.   
-000263c0: 2020 2020 206e 702e 6162 7328 6461 7461       np.abs(data
-000263d0: 7365 742e 7261 7465 5f70 6d29 0a20 2020  set.rate_pm).   
-000263e0: 2029 0a0a 2020 2020 2320 5365 7420 7820   )..    # Set x 
-000263f0: 7469 636b 2066 6f72 6d61 7474 696e 670a  tick formatting.
-00026400: 2020 2020 6775 692e 7365 745f 7261 7465      gui.set_rate
-00026410: 5f78 7469 636b 5f66 6f72 6d61 7474 696e  _xtick_formattin
-00026420: 6728 6178 2c20 785f 7661 7273 290a 0a20  g(ax, x_vars).. 
-00026430: 2020 2066 6967 2e74 6967 6874 5f6c 6179     fig.tight_lay
-00026440: 6f75 7428 290a 0a20 2020 2069 6620 7361  out()..    if sa
-00026450: 7665 3a0a 2020 2020 2020 2020 706c 742e  ve:.        plt.
-00026460: 7361 7665 6669 6728 7361 7665 5f6e 616d  savefig(save_nam
-00026470: 6529 0a20 2020 2020 2020 2069 6620 7665  e).        if ve
-00026480: 7262 6f73 653a 0a20 2020 2020 2020 2020  rbose:.         
-00026490: 2020 2075 742e 6370 7269 6e74 280a 2020     ut.cprint(.  
-000264a0: 2020 2020 2020 2020 2020 2020 2020 6627                f'
-000264b0: 5c6e 2052 656c 6178 6174 696f 6e20 706c  \n Relaxation pl
-000264c0: 6f74 2073 6176 6564 2074 6f20 5c6e 207b  ot saved to \n {
-000264d0: 7361 7665 5f6e 616d 657d 5c6e 272c 0a20  save_name}\n',. 
-000264e0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-000264f0: 6379 616e 270a 2020 2020 2020 2020 2020  cyan'.          
-00026500: 2020 290a 2020 2020 6966 2073 686f 773a    ).    if show:
-00026510: 0a20 2020 2020 2020 2070 6c74 2e73 686f  .        plt.sho
-00026520: 7728 290a 0a20 2020 2072 6574 7572 6e20  w()..    return 
-00026530: 6669 672c 2061 780a 0a0a 6465 6620 706c  fig, ax...def pl
-00026540: 6f74 5f72 6174 655f 7265 7369 6475 616c  ot_rate_residual
-00026550: 7328 6461 7461 7365 743a 2054 6175 5444  s(dataset: TauTD
-00026560: 6174 6173 6574 2c0a 2020 2020 2020 2020  ataset,.        
-00026570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026580: 6d6f 6465 6c3a 204c 6f67 5461 7554 4d6f  model: LogTauTMo
-00026590: 6465 6c20 7c20 4d75 6c74 694c 6f67 5461  del | MultiLogTa
-000265a0: 7554 4d6f 6465 6c20 7c20 4c6f 6754 6175  uTModel | LogTau
-000265b0: 484d 6f64 656c 207c 204d 756c 7469 4c6f  HModel | MultiLo
-000265c0: 6754 6175 484d 6f64 656c 2c20 2320 6e6f  gTauHModel, # no
-000265d0: 7161 0a20 2020 2020 2020 2020 2020 2020  qa.             
-000265e0: 2020 2020 2020 2020 2020 2073 6176 653a             save:
-000265f0: 2062 6f6f 6c20 3d20 4661 6c73 652c 2073   bool = False, s
-00026600: 686f 773a 2062 6f6f 6c20 3d20 5472 7565  how: bool = True
-00026610: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00026620: 2020 2020 2020 2020 2020 7361 7665 5f6e            save_n
-00026630: 616d 653a 2073 7472 203d 2027 6d6f 6465  ame: str = 'mode
-00026640: 6c5f 7265 7369 6475 616c 5f74 6175 2e70  l_residual_tau.p
-00026650: 6e67 272c 0a20 2020 2020 2020 2020 2020  ng',.           
-00026660: 2020 2020 2020 2020 2020 2020 2076 6572               ver
-00026670: 626f 7365 3a20 626f 6f6c 203d 2054 7275  bose: bool = Tru
-00026680: 6529 202d 3e20 7475 706c 655b 706c 742e  e) -> tuple[plt.
-00026690: 4669 6775 7265 2c20 706c 742e 4178 6573  Figure, plt.Axes
-000266a0: 5d3a 0a20 2020 2027 2727 0a20 2020 2050  ]:.    '''.    P
-000266b0: 6c6f 7473 2064 6966 6665 7265 6e63 6520  lots difference 
-000266c0: 6f66 206c 6f67 3130 2865 7870 6572 696d  of log10(experim
-000266d0: 656e 7429 2061 6e64 206c 6f67 3130 286d  ent) and log10(m
-000266e0: 6f64 656c 2920 7265 6c61 7861 7469 6f6e  odel) relaxation
-000266f0: 2072 6174 6573 0a20 2020 2028 6c6f 6731   rates.    (log1
-00026700: 3028 6578 7065 7269 6d65 6e74 5f72 6174  0(experiment_rat
-00026710: 6529 202d 206c 6f67 3130 286d 6f64 656c  e) - log10(model
-00026720: 5f72 6174 6529 2076 7320 5465 6d70 6572  _rate) vs Temper
-00026730: 6174 7572 6520 6f72 2046 6965 6c64 290a  ature or Field).
-00026740: 0a20 2020 2050 6172 616d 6574 6572 730a  .    Parameters.
-00026750: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-00026760: 2020 2064 6174 6173 6574 3a20 5461 7554     dataset: TauT
-00026770: 4461 7461 7365 7420 7c20 5461 7548 4461  Dataset | TauHDa
-00026780: 7461 7365 740a 2020 2020 2020 2020 4461  taset.        Da
-00026790: 7461 7365 7420 746f 2070 6c6f 740a 2020  taset to plot.  
-000267a0: 2020 6d6f 6465 6c3a 204c 6f67 5461 7554    model: LogTauT
-000267b0: 4d6f 6465 6c20 7c20 4d75 6c74 694c 6f67  Model | MultiLog
-000267c0: 5461 7554 4d6f 6465 6c20 7c20 4c6f 6754  TauTModel | LogT
-000267d0: 6175 484d 6f64 656c 207c 204d 756c 7469  auHModel | Multi
-000267e0: 4c6f 6754 6175 484d 6f64 656c 0a20 2020  LogTauHModel.   
-000267f0: 2020 2020 204d 6f64 656c 2028 6669 7474       Model (fitt
-00026800: 6564 2920 746f 2070 6c6f 740a 2020 2020  ed) to plot.    
-00026810: 7368 6f77 3a20 626f 6f6c 2c20 6465 6661  show: bool, defa
-00026820: 756c 7420 5472 7565 0a20 2020 2020 2020  ult True.       
-00026830: 2049 6620 5472 7565 2c20 7368 6f77 2070   If True, show p
-00026840: 6c6f 7420 6f6e 2073 6372 6565 6e0a 2020  lot on screen.  
-00026850: 2020 7361 7665 3a20 626f 6f6c 2c20 6465    save: bool, de
-00026860: 6661 756c 7420 4661 6c73 650a 2020 2020  fault False.    
-00026870: 2020 2020 4966 2054 7275 652c 2073 6176      If True, sav
-00026880: 6520 706c 6f74 2074 6f20 6669 6c65 2060  e plot to file `
-00026890: 7361 7665 5f6e 616d 6560 0a20 2020 2073  save_name`.    s
-000268a0: 6176 655f 6e61 6d65 3a20 7374 722c 2064  ave_name: str, d
-000268b0: 6566 6175 6c74 2027 6d6f 6465 6c5f 7265  efault 'model_re
-000268c0: 7369 6475 616c 5f74 6175 2e70 6e67 270a  sidual_tau.png'.
-000268d0: 2020 2020 2020 2020 4966 2073 6176 6520          If save 
-000268e0: 6973 2054 7275 652c 2077 696c 6c20 7361  is True, will sa
-000268f0: 7665 2070 6c6f 7420 746f 2074 6869 7320  ve plot to this 
-00026900: 6669 6c65 6e61 6d65 0a20 2020 2076 6572  filename.    ver
-00026910: 626f 7365 3a20 626f 6f6c 2c20 6465 6661  bose: bool, defa
-00026920: 756c 7420 5472 7565 0a20 2020 2020 2020  ult True.       
-00026930: 2049 6620 5472 7565 2c20 706c 6f74 2066   If True, plot f
-00026940: 696c 6520 6c6f 6361 7469 6f6e 2069 7320  ile location is 
-00026950: 7772 6974 7465 6e20 746f 2074 6572 6d69  written to termi
-00026960: 6e61 6c0a 0a20 2020 2052 6574 7572 6e73  nal..    Returns
-00026970: 0a20 2020 202d 2d2d 2d2d 2d2d 0a20 2020  .    -------.   
-00026980: 2070 6c74 2e46 6967 7572 650a 2020 2020   plt.Figure.    
-00026990: 2020 2020 4d61 7470 6c6f 746c 6962 2066      Matplotlib f
-000269a0: 6967 7572 6520 6f62 6a65 6374 0a20 2020  igure object.   
-000269b0: 2070 6c74 2e41 7865 730a 2020 2020 2020   plt.Axes.      
-000269c0: 2020 4d61 7470 6c6f 746c 6962 2061 7869    Matplotlib axi
-000269d0: 7320 6f62 6a65 6374 0a20 2020 2027 2727  s object.    '''
-000269e0: 0a20 2020 2023 2043 7265 6174 6520 6669  .    # Create fi
-000269f0: 6775 7265 2061 6e64 2061 7865 730a 2020  gure and axes.  
-00026a00: 2020 6669 672c 2061 7820 3d20 706c 742e    fig, ax = plt.
-00026a10: 7375 6270 6c6f 7473 280a 2020 2020 2020  subplots(.      
-00026a20: 2020 312c 0a20 2020 2020 2020 2031 2c0a    1,.        1,.
-00026a30: 2020 2020 2020 2020 6669 6773 697a 653d          figsize=
-00026a40: 5b36 2c20 365d 2c0a 2020 2020 2020 2020  [6, 6],.        
-00026a50: 6e75 6d3d 2752 6573 6964 7561 6c73 270a  num='Residuals'.
-00026a60: 2020 2020 290a 0a20 2020 205f 706c 6f74      )..    _plot
-00026a70: 5f72 6174 655f 7265 7369 6475 616c 7328  _rate_residuals(
-00026a80: 6461 7461 7365 742c 206d 6f64 656c 2c20  dataset, model, 
-00026a90: 6178 290a 0a20 2020 2066 6967 2e74 6967  ax)..    fig.tig
-00026aa0: 6874 5f6c 6179 6f75 7428 290a 0a20 2020  ht_layout()..   
-00026ab0: 2023 2053 6176 6520 706c 6f74 0a20 2020   # Save plot.   
-00026ac0: 2069 6620 7361 7665 3a0a 2020 2020 2020   if save:.      
-00026ad0: 2020 706c 742e 7361 7665 6669 6728 7361    plt.savefig(sa
-00026ae0: 7665 5f6e 616d 652c 2064 7069 3d33 3030  ve_name, dpi=300
-00026af0: 290a 2020 2020 2020 2020 6966 2076 6572  ).        if ver
-00026b00: 626f 7365 3a0a 2020 2020 2020 2020 2020  bose:.          
-00026b10: 2020 7574 2e63 7072 696e 7428 0a20 2020    ut.cprint(.   
-00026b20: 2020 2020 2020 2020 2020 2020 2066 275c               f'\
-00026b30: 6e20 5261 7465 2072 6573 6964 7561 6c73  n Rate residuals
-00026b40: 2070 6c6f 7420 7361 7665 6420 746f 205c   plot saved to \
-00026b50: 6e20 7b73 6176 655f 6e61 6d65 7d5c 6e27  n {save_name}\n'
-00026b60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00026b70: 2020 2763 7961 6e27 0a20 2020 2020 2020    'cyan'.       
-00026b80: 2020 2020 2029 0a20 2020 2069 6620 7368       ).    if sh
-00026b90: 6f77 3a0a 2020 2020 2020 2020 706c 742e  ow:.        plt.
-00026ba0: 7368 6f77 2829 0a0a 2020 2020 7265 7475  show()..    retu
-00026bb0: 726e 2066 6967 2c20 6178 0a0a 0a64 6566  rn fig, ax...def
-00026bc0: 2071 745f 706c 6f74 5f72 6174 655f 7265   qt_plot_rate_re
-00026bd0: 7369 6475 616c 7328 6170 703a 2051 7457  siduals(app: QtW
-00026be0: 6964 6765 7473 2e51 4170 706c 6963 6174  idgets.QApplicat
-00026bf0: 696f 6e2c 2064 6174 6173 6574 3a20 5461  ion, dataset: Ta
-00026c00: 7554 4461 7461 7365 742c 0a20 2020 2020  uTDataset,.     
-00026c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026c20: 2020 2020 2020 6d6f 6465 6c3a 204c 6f67        model: Log
-00026c30: 5461 7554 4d6f 6465 6c20 7c20 4d75 6c74  TauTModel | Mult
-00026c40: 694c 6f67 5461 7554 4d6f 6465 6c20 7c20  iLogTauTModel | 
-00026c50: 4c6f 6754 6175 484d 6f64 656c 207c 204d  LogTauHModel | M
-00026c60: 756c 7469 4c6f 6754 6175 484d 6f64 656c  ultiLogTauHModel
-00026c70: 2c20 2320 6e6f 7161 0a20 2020 2020 2020  , # noqa.       
-00026c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026c90: 2020 2020 7361 7665 3a20 626f 6f6c 203d      save: bool =
-00026ca0: 2046 616c 7365 2c20 7368 6f77 3a20 626f   False, show: bo
-00026cb0: 6f6c 203d 2054 7275 652c 0a20 2020 2020  ol = True,.     
-00026cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026cd0: 2020 2020 2020 7361 7665 5f6e 616d 653a        save_name:
-00026ce0: 2073 7472 203d 2027 6d6f 6465 6c5f 7265   str = 'model_re
-00026cf0: 7369 6475 616c 5f74 6175 2e70 6e67 272c  sidual_tau.png',
-00026d00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00026d10: 2020 2020 2020 2020 2020 2020 7665 7262              verb
-00026d20: 6f73 653a 2062 6f6f 6c20 3d20 5472 7565  ose: bool = True
-00026d30: 2920 2d3e 204e 6f6e 653a 0a20 2020 2027  ) -> None:.    '
-00026d40: 2727 0a20 2020 2050 6c6f 7473 2064 6966  ''.    Plots dif
-00026d50: 6665 7265 6e63 6520 6f66 206c 6f67 3130  ference of log10
-00026d60: 2865 7870 6572 696d 656e 7429 2061 6e64  (experiment) and
-00026d70: 206c 6f67 3130 286d 6f64 656c 2920 7265   log10(model) re
-00026d80: 6c61 7861 7469 6f6e 2072 6174 6573 0a20  laxation rates. 
-00026d90: 2020 2069 6e20 6120 7174 2077 696e 646f     in a qt windo
-00026da0: 7720 7573 696e 6720 6d61 7470 6c6f 746c  w using matplotl
-00026db0: 6962 0a0a 2020 2020 5061 7261 6d65 7465  ib..    Paramete
-00026dc0: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
-00026dd0: 2d0a 2020 2020 6170 703a 2051 7457 6964  -.    app: QtWid
-00026de0: 6765 7473 2e51 4170 706c 6963 6174 696f  gets.QApplicatio
-00026df0: 6e0a 2020 2020 2020 2020 4170 706c 6963  n.        Applic
-00026e00: 6174 696f 6e20 7573 6564 2062 7920 6375  ation used by cu
-00026e10: 7272 656e 7420 7072 6f67 7261 6d0a 2020  rrent program.  
-00026e20: 2020 2020 2020 4372 6561 7465 2077 6974        Create wit
-00026e30: 6820 6061 7070 3d51 7457 6964 6765 7473  h `app=QtWidgets
-00026e40: 2e51 4170 706c 6963 6174 696f 6e28 5b5d  .QApplication([]
-00026e50: 2960 0a20 2020 2064 6174 6173 6574 3a20  )`.    dataset: 
-00026e60: 5461 7554 4461 7461 7365 7420 7c20 5461  TauTDataset | Ta
-00026e70: 7548 4461 7461 7365 740a 2020 2020 2020  uHDataset.      
-00026e80: 2020 4461 7461 7365 7420 746f 2070 6c6f    Dataset to plo
-00026e90: 740a 2020 2020 6d6f 6465 6c3a 204c 6f67  t.    model: Log
-00026ea0: 5461 7554 4d6f 6465 6c20 7c20 4d75 6c74  TauTModel | Mult
-00026eb0: 694c 6f67 5461 7554 4d6f 6465 6c20 7c20  iLogTauTModel | 
-00026ec0: 4c6f 6754 6175 484d 6f64 656c 207c 204d  LogTauHModel | M
-00026ed0: 756c 7469 4c6f 6754 6175 484d 6f64 656c  ultiLogTauHModel
-00026ee0: 0a20 2020 2020 2020 204d 6f64 656c 2028  .        Model (
-00026ef0: 6669 7474 6564 2920 746f 2070 6c6f 740a  fitted) to plot.
-00026f00: 2020 2020 7368 6f77 3a20 626f 6f6c 2c20      show: bool, 
-00026f10: 6465 6661 756c 7420 5472 7565 0a20 2020  default True.   
-00026f20: 2020 2020 2049 6620 5472 7565 2c20 7368       If True, sh
-00026f30: 6f77 2070 6c6f 7420 6f6e 2073 6372 6565  ow plot on scree
-00026f40: 6e0a 2020 2020 7361 7665 3a20 626f 6f6c  n.    save: bool
-00026f50: 2c20 6465 6661 756c 7420 4661 6c73 650a  , default False.
-00026f60: 2020 2020 2020 2020 4966 2054 7275 652c          If True,
-00026f70: 2073 6176 6520 706c 6f74 2074 6f20 6669   save plot to fi
-00026f80: 6c65 2060 7361 7665 5f6e 616d 6560 0a20  le `save_name`. 
-00026f90: 2020 2073 6176 655f 6e61 6d65 3a20 7374     save_name: st
-00026fa0: 722c 2064 6566 6175 6c74 2027 6d6f 6465  r, default 'mode
-00026fb0: 6c5f 7265 7369 6475 616c 5f74 6175 2e70  l_residual_tau.p
-00026fc0: 6e67 270a 2020 2020 2020 2020 4966 2073  ng'.        If s
-00026fd0: 6176 6520 6973 2054 7275 652c 2077 696c  ave is True, wil
-00026fe0: 6c20 7361 7665 2070 6c6f 7420 746f 2074  l save plot to t
-00026ff0: 6869 7320 6669 6c65 6e61 6d65 0a20 2020  his filename.   
-00027000: 2076 6572 626f 7365 3a20 626f 6f6c 2c20   verbose: bool, 
-00027010: 6465 6661 756c 7420 5472 7565 0a20 2020  default True.   
-00027020: 2020 2020 2049 6620 5472 7565 2c20 706c       If True, pl
-00027030: 6f74 2066 696c 6520 6c6f 6361 7469 6f6e  ot file location
-00027040: 2069 7320 7772 6974 7465 6e20 746f 2074   is written to t
-00027050: 6572 6d69 6e61 6c0a 0a20 2020 2052 6574  erminal..    Ret
-00027060: 7572 6e73 0a20 2020 202d 2d2d 2d2d 2d2d  urns.    -------
-00027070: 0a20 2020 204e 6f6e 650a 2020 2020 2727  .    None.    ''
-00027080: 270a 0a20 2020 2077 696e 646f 7720 3d20  '..    window = 
-00027090: 6775 692e 4d61 7470 6c6f 746c 6962 5769  gui.MatplotlibWi
-000270a0: 6e64 6f77 2829 0a20 2020 2077 696e 646f  ndow().    windo
-000270b0: 772e 7365 7457 696e 646f 7754 6974 6c65  w.setWindowTitle
-000270c0: 2827 5265 7369 6475 616c 7327 290a 0a20  ('Residuals').. 
-000270d0: 2020 205f 706c 6f74 5f72 6174 655f 7265     _plot_rate_re
-000270e0: 7369 6475 616c 7328 6461 7461 7365 742c  siduals(dataset,
-000270f0: 206d 6f64 656c 2c20 7769 6e64 6f77 2e73   model, window.s
-00027100: 632e 6178 290a 0a20 2020 2023 2053 6176  c.ax)..    # Sav
-00027110: 6520 706c 6f74 0a20 2020 2069 6620 7361  e plot.    if sa
-00027120: 7665 3a0a 2020 2020 2020 2020 7769 6e64  ve:.        wind
-00027130: 6f77 2e73 632e 6669 672e 7361 7665 6669  ow.sc.fig.savefi
-00027140: 6728 7361 7665 5f6e 616d 652c 2064 7069  g(save_name, dpi
-00027150: 3d33 3030 290a 2020 2020 2020 2020 6966  =300).        if
-00027160: 2076 6572 626f 7365 3a0a 2020 2020 2020   verbose:.      
-00027170: 2020 2020 2020 7574 2e63 7072 696e 7428        ut.cprint(
-00027180: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00027190: 2066 275c 6e20 5261 7465 2072 6573 6964   f'\n Rate resid
-000271a0: 7561 6c73 2070 6c6f 7420 7361 7665 6420  uals plot saved 
-000271b0: 746f 205c 6e20 7b73 6176 655f 6e61 6d65  to \n {save_name
-000271c0: 7d5c 6e27 2c0a 2020 2020 2020 2020 2020  }\n',.          
-000271d0: 2020 2020 2020 2763 7961 6e27 0a20 2020        'cyan'.   
-000271e0: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-000271f0: 6966 2073 686f 773a 0a20 2020 2020 2020  if show:.       
-00027200: 2077 696e 646f 772e 7368 6f77 2829 0a20   window.show(). 
-00027210: 2020 2020 2020 2023 2043 616c 6c20 7477         # Call tw
-00027220: 6963 6520 656c 7365 2069 7420 776f 6e74  ice else it wont
-00027230: 2077 6f72 6b21 0a20 2020 2020 2020 2077   work!.        w
-00027240: 696e 646f 772e 7363 2e66 6967 2e74 6967  indow.sc.fig.tig
-00027250: 6874 5f6c 6179 6f75 7428 290a 2020 2020  ht_layout().    
-00027260: 2020 2020 7769 6e64 6f77 2e73 632e 6669      window.sc.fi
-00027270: 672e 7469 6768 745f 6c61 796f 7574 2829  g.tight_layout()
-00027280: 0a20 2020 2020 2020 2061 7070 2e65 7865  .        app.exe
-00027290: 635f 2829 0a0a 2020 2020 7265 7475 726e  c_()..    return
-000272a0: 0a0a 0a64 6566 205f 706c 6f74 5f72 6174  ...def _plot_rat
-000272b0: 655f 7265 7369 6475 616c 7328 6461 7461  e_residuals(data
-000272c0: 7365 743a 2054 6175 5444 6174 6173 6574  set: TauTDataset
-000272d0: 207c 2054 6175 4844 6174 6173 6574 2c0a   | TauHDataset,.
-000272e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000272f0: 2020 2020 2020 2020 206d 6f64 656c 3a20           model: 
-00027300: 4c6f 6754 6175 544d 6f64 656c 207c 204d  LogTauTModel | M
-00027310: 756c 7469 4c6f 6754 6175 544d 6f64 656c  ultiLogTauTModel
-00027320: 207c 204c 6f67 5461 7548 4d6f 6465 6c20   | LogTauHModel 
-00027330: 7c20 4d75 6c74 694c 6f67 5461 7548 4d6f  | MultiLogTauHMo
-00027340: 6465 6c2c 2023 206e 6f71 610a 2020 2020  del, # noqa.    
-00027350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027360: 2020 2020 2061 783a 2070 6c74 2e41 7865       ax: plt.Axe
-00027370: 7329 202d 3e20 4e6f 6e65 3a0a 2020 2020  s) -> None:.    
-00027380: 2727 270a 2020 2020 506c 6f74 7320 6469  '''.    Plots di
-00027390: 6666 6572 656e 6365 206f 6620 6c6f 6731  fference of log1
-000273a0: 3028 6578 7065 7269 6d65 6e74 2920 616e  0(experiment) an
-000273b0: 6420 6c6f 6731 3028 6d6f 6465 6c29 2072  d log10(model) r
-000273c0: 656c 6178 6174 696f 6e20 7261 7465 730a  elaxation rates.
-000273d0: 2020 2020 6f6e 746f 2061 2067 6976 656e      onto a given
-000273e0: 2066 6967 7572 6520 616e 6420 6178 6973   figure and axis
-000273f0: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
-00027400: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
-00027410: 2020 2020 6d6f 6465 6c73 3a20 6c69 7374      models: list
-00027420: 5b4c 6f67 5461 7554 4d6f 6465 6c20 7c20  [LogTauTModel | 
-00027430: 4d75 6c74 694c 6f67 5461 7554 4d6f 6465  MultiLogTauTMode
-00027440: 6c20 7c20 4c6f 6754 6175 484d 6f64 656c  l | LogTauHModel
-00027450: 207c 204d 756c 7469 4c6f 6754 6175 484d   | MultiLogTauHM
-00027460: 6f64 656c 5d0a 2020 2020 2020 2020 4d6f  odel].        Mo
-00027470: 6465 6c73 2c20 6f6e 6520 7065 7220 7465  dels, one per te
-00027480: 6d70 6572 6174 7572 650a 2020 2020 6669  mperature.    fi
-00027490: 6c65 5f6e 616d 653a 2073 7472 0a20 2020  le_name: str.   
-000274a0: 2020 2020 204e 616d 6520 6f66 206f 7574       Name of out
-000274b0: 7075 7420 6669 6c65 0a20 2020 2061 783a  put file.    ax:
-000274c0: 2070 6c74 2e41 7865 730a 2020 2020 2020   plt.Axes.      
-000274d0: 2020 4d61 7470 6c6f 746c 6962 2041 7869    Matplotlib Axi
-000274e0: 7320 6f62 6a65 6374 2075 7365 6420 666f  s object used fo
-000274f0: 7220 706c 6f74 0a0a 2020 2020 5265 7475  r plot..    Retu
-00027500: 726e 730a 2020 2020 2d2d 2d2d 2d2d 2d0a  rns.    -------.
-00027510: 2020 2020 4e6f 6e65 0a20 2020 2027 2727      None.    '''
-00027520: 2023 206e 6f71 610a 0a20 2020 2069 6620   # noqa..    if 
-00027530: 6973 696e 7374 616e 6365 2864 6174 6173  isinstance(datas
-00027540: 6574 2c20 5461 7548 4461 7461 7365 7429  et, TauHDataset)
-00027550: 3a0a 2020 2020 2020 2020 785f 7661 7273  :.        x_vars
-00027560: 203d 2064 6174 6173 6574 2e66 6965 6c64   = dataset.field
-00027570: 730a 2020 2020 2020 2020 6178 2e73 6574  s.        ax.set
-00027580: 5f78 6c61 6265 6c28 7227 4669 656c 6420  _xlabel(r'Field 
-00027590: 284f 6529 2729 0a20 2020 2065 6c69 6620  (Oe)').    elif 
-000275a0: 6973 696e 7374 616e 6365 2864 6174 6173  isinstance(datas
-000275b0: 6574 2c20 5461 7554 4461 7461 7365 7429  et, TauTDataset)
-000275c0: 3a0a 2020 2020 2020 2020 785f 7661 7273  :.        x_vars
-000275d0: 203d 2064 6174 6173 6574 2e74 656d 7065   = dataset.tempe
-000275e0: 7261 7475 7265 730a 2020 2020 2020 2020  ratures.        
-000275f0: 6178 2e73 6574 5f78 6c61 6265 6c28 7227  ax.set_xlabel(r'
-00027600: 5465 6d70 6572 6174 7572 6520 284b 2927  Temperature (K)'
-00027610: 290a 0a20 2020 2023 2041 6464 2061 6464  )..    # Add add
-00027620: 6974 696f 6e61 6c20 7365 7420 6f66 2061  itional set of a
-00027630: 7865 7320 746f 2063 7265 6174 6520 277a  xes to create 'z
-00027640: 6572 6f27 206c 696e 650a 2020 2020 6178  ero' line.    ax
-00027650: 3220 3d20 6178 2e74 7769 6e79 2829 0a20  2 = ax.twiny(). 
-00027660: 2020 2061 7832 2e67 6574 5f79 6178 6973     ax2.get_yaxis
-00027670: 2829 2e73 6574 5f76 6973 6962 6c65 2846  ().set_visible(F
-00027680: 616c 7365 290a 2020 2020 6178 322e 7365  alse).    ax2.se
-00027690: 745f 7974 6963 6b73 285b 5d29 0a20 2020  t_yticks([]).   
-000276a0: 2061 7832 2e73 6574 5f78 7469 636b 7328   ax2.set_xticks(
-000276b0: 5b5d 290a 2020 2020 6178 322e 7370 696e  []).    ax2.spin
-000276c0: 6573 5b27 626f 7474 6f6d 275d 2e73 6574  es['bottom'].set
-000276d0: 5f70 6f73 6974 696f 6e28 2827 7a65 726f  _position(('zero
-000276e0: 2729 290a 0a20 2020 2069 6620 7479 7065  '))..    if type
-000276f0: 286d 6f64 656c 2920 696e 205b 4d75 6c74  (model) in [Mult
-00027700: 694c 6f67 5461 7554 4d6f 6465 6c2c 204d  iLogTauTModel, M
-00027710: 756c 7469 4c6f 6754 6175 484d 6f64 656c  ultiLogTauHModel
-00027720: 5d3a 0a20 2020 2020 2020 206c 6f67 6d6f  ]:.        logmo
-00027730: 6465 6c73 203d 206d 6f64 656c 2e6c 6f67  dels = model.log
-00027740: 6d6f 6465 6c73 0a20 2020 2065 6c73 653a  models.    else:
-00027750: 0a20 2020 2020 2020 206c 6f67 6d6f 6465  .        logmode
-00027760: 6c73 203d 205b 6d6f 6465 6c5d 0a0a 2020  ls = [model]..  
-00027770: 2020 6d6f 6465 6c5f 7261 7465 203d 206e    model_rate = n
-00027780: 702e 7a65 726f 7328 6c65 6e28 785f 7661  p.zeros(len(x_va
-00027790: 7273 2929 0a0a 2020 2020 666f 7220 6c6f  rs))..    for lo
-000277a0: 676d 6f64 656c 2069 6e20 6c6f 676d 6f64  gmodel in logmod
-000277b0: 656c 733a 0a20 2020 2020 2020 206d 6f64  els:.        mod
-000277c0: 656c 5f72 6174 6520 2b3d 2031 302a 2a6c  el_rate += 10**l
-000277d0: 6f67 6d6f 6465 6c2e 6d6f 6465 6c28 0a20  ogmodel.model(. 
-000277e0: 2020 2020 2020 2020 2020 206c 6f67 6d6f             logmo
-000277f0: 6465 6c2e 6669 6e61 6c5f 7661 725f 7661  del.final_var_va
-00027800: 6c75 6573 2c0a 2020 2020 2020 2020 2020  lues,.          
-00027810: 2020 785f 7661 7273 2c0a 2020 2020 2020    x_vars,.      
-00027820: 2020 290a 0a20 2020 206d 6f64 656c 5f6c    )..    model_l
-00027830: 6f67 7261 7465 203d 206e 702e 6c6f 6731  ograte = np.log1
-00027840: 3028 6d6f 6465 6c5f 7261 7465 290a 0a20  0(model_rate).. 
-00027850: 2020 2023 2050 6c6f 7420 7265 7369 6475     # Plot residu
-00027860: 616c 730a 2020 2020 6966 206c 656e 2864  als.    if len(d
-00027870: 6174 6173 6574 2e6c 6f67 7261 7465 5f70  ataset.lograte_p
-00027880: 6d29 3a0a 2020 2020 2020 2020 6178 2e65  m):.        ax.e
-00027890: 7272 6f72 6261 7228 0a20 2020 2020 2020  rrorbar(.       
-000278a0: 2020 2020 2078 5f76 6172 732c 0a20 2020       x_vars,.   
-000278b0: 2020 2020 2020 2020 206e 702e 6c6f 6731           np.log1
-000278c0: 3028 6461 7461 7365 742e 7261 7465 7329  0(dataset.rates)
-000278d0: 202d 206d 6f64 656c 5f6c 6f67 7261 7465   - model_lograte
-000278e0: 2c0a 2020 2020 2020 2020 2020 2020 7965  ,.            ye
-000278f0: 7272 3d64 6174 6173 6574 2e6c 6f67 7261  rr=dataset.logra
-00027900: 7465 5f70 6d2c 0a20 2020 2020 2020 2020  te_pm,.         
-00027910: 2020 2066 6d74 3d27 622e 270a 2020 2020     fmt='b.'.    
-00027920: 2020 2020 290a 2020 2020 656c 7365 3a0a      ).    else:.
-00027930: 2020 2020 2020 2020 6178 2e70 6c6f 7428          ax.plot(
-00027940: 0a20 2020 2020 2020 2020 2020 2078 5f76  .            x_v
-00027950: 6172 732c 0a20 2020 2020 2020 2020 2020  ars,.           
-00027960: 206e 702e 6c6f 6731 3028 6461 7461 7365   np.log10(datase
-00027970: 742e 7261 7465 7329 202d 206d 6f64 656c  t.rates) - model
-00027980: 5f6c 6f67 7261 7465 2c0a 2020 2020 2020  _lograte,.      
-00027990: 2020 2020 2020 636f 6c6f 723d 2762 272c        color='b',
-000279a0: 0a20 2020 2020 2020 2020 2020 206d 6172  .            mar
-000279b0: 6b65 723d 276f 272c 0a20 2020 2020 2020  ker='o',.       
-000279c0: 2020 2020 206c 773d 302c 0a20 2020 2020       lw=0,.     
-000279d0: 2020 2020 2020 2066 696c 6c73 7479 6c65         fillstyle
-000279e0: 3d27 6e6f 6e65 272c 0a20 2020 2020 2020  ='none',.       
-000279f0: 2020 2020 206c 6162 656c 3d27 4578 7065       label='Expe
-00027a00: 7269 6d65 6e74 270a 2020 2020 2020 2020  riment'.        
-00027a10: 290a 2020 2020 2320 5365 7420 6c6f 6720  ).    # Set log 
-00027a20: 7363 616c 6520 6f6e 2078 2061 7869 730a  scale on x axis.
-00027a30: 2020 2020 6178 2e73 6574 5f78 7363 616c      ax.set_xscal
-00027a40: 6528 276c 6f67 2729 0a0a 2020 2020 2320  e('log')..    # 
-00027a50: 5365 7420 666f 726d 6174 7469 6e67 2066  Set formatting f
-00027a60: 6f72 2079 2061 7869 7320 6d61 6a6f 7220  or y axis major 
-00027a70: 7469 636b 730a 2020 2020 6178 2e79 6178  ticks.    ax.yax
-00027a80: 6973 2e73 6574 5f6d 616a 6f72 5f66 6f72  is.set_major_for
-00027a90: 6d61 7474 6572 2853 6361 6c61 7246 6f72  matter(ScalarFor
-00027aa0: 6d61 7474 6572 2829 290a 0a20 2020 2023  matter())..    #
-00027ab0: 2041 6464 206d 696e 6f72 2074 6963 6b73   Add minor ticks
-00027ac0: 2074 6f20 7920 6178 6973 2077 6974 6820   to y axis with 
-00027ad0: 6e6f 206c 6162 656c 730a 2020 2020 6178  no labels.    ax
-00027ae0: 2e79 6178 6973 2e73 6574 5f6d 696e 6f72  .yaxis.set_minor
-00027af0: 5f6c 6f63 6174 6f72 2841 7574 6f4d 696e  _locator(AutoMin
-00027b00: 6f72 4c6f 6361 746f 7228 2929 0a0a 2020  orLocator())..  
-00027b10: 2020 2320 5379 6d6d 6574 7269 7365 2079    # Symmetrise y
-00027b20: 2061 7869 7320 6c69 6d69 7473 2062 6173   axis limits bas
-00027b30: 6564 206f 6e20 6d61 7820 6162 7320 6572  ed on max abs er
-00027b40: 726f 720a 2020 2020 6966 206c 656e 2864  ror.    if len(d
-00027b50: 6174 6173 6574 2e6c 6f67 7261 7465 5f70  ataset.lograte_p
-00027b60: 6d29 3a0a 2020 2020 2020 2020 616c 6c5f  m):.        all_
-00027b70: 6461 7461 203d 205b 0a20 2020 2020 2020  data = [.       
-00027b80: 2020 2020 206e 702e 6c6f 6731 3028 6461       np.log10(da
-00027b90: 7461 7365 742e 7261 7465 7329 202d 206d  taset.rates) - m
-00027ba0: 6f64 656c 5f6c 6f67 7261 7465 202b 2064  odel_lograte + d
-00027bb0: 6174 6173 6574 2e6c 6f67 7261 7465 5f70  ataset.lograte_p
-00027bc0: 6d0a 2020 2020 2020 2020 5d0a 2020 2020  m.        ].    
-00027bd0: 2020 2020 616c 6c5f 6461 7461 202b 3d20      all_data += 
-00027be0: 5b0a 2020 2020 2020 2020 2020 2020 6e70  [.            np
-00027bf0: 2e6c 6f67 3130 2864 6174 6173 6574 2e72  .log10(dataset.r
-00027c00: 6174 6573 2920 2d20 6d6f 6465 6c5f 6c6f  ates) - model_lo
-00027c10: 6772 6174 6520 2d20 6461 7461 7365 742e  grate - dataset.
-00027c20: 6c6f 6772 6174 655f 706d 0a20 2020 2020  lograte_pm.     
-00027c30: 2020 205d 0a20 2020 2065 6c73 653a 0a20     ].    else:. 
-00027c40: 2020 2020 2020 2061 6c6c 5f64 6174 6120         all_data 
-00027c50: 3d20 5b0a 2020 2020 2020 2020 2020 2020  = [.            
-00027c60: 6e70 2e6c 6f67 3130 2864 6174 6173 6574  np.log10(dataset
-00027c70: 2e72 6174 6573 2920 2d20 6d6f 6465 6c5f  .rates) - model_
-00027c80: 6c6f 6772 6174 650a 2020 2020 2020 2020  lograte.        
-00027c90: 5d0a 2020 2020 2020 2020 616c 6c5f 6461  ].        all_da
-00027ca0: 7461 202b 3d20 5b0a 2020 2020 2020 2020  ta += [.        
-00027cb0: 2020 2020 6e70 2e6c 6f67 3130 2864 6174      np.log10(dat
-00027cc0: 6173 6574 2e72 6174 6573 2920 2d20 6d6f  aset.rates) - mo
-00027cd0: 6465 6c5f 6c6f 6772 6174 650a 2020 2020  del_lograte.    
-00027ce0: 2020 2020 5d0a 0a20 2020 2074 6963 6b73      ]..    ticks
-00027cf0: 2c20 6d61 7876 616c 203d 2067 7569 2e6d  , maxval = gui.m
-00027d00: 696e 5f6d 6178 5f74 6963 6b73 5f77 6974  in_max_ticks_wit
-00027d10: 685f 7a65 726f 2861 6c6c 5f64 6174 612c  h_zero(all_data,
-00027d20: 2035 290a 2020 2020 6178 2e73 6574 5f79   5).    ax.set_y
-00027d30: 7469 636b 7328 7469 636b 7329 0a0a 2020  ticks(ticks)..  
-00027d40: 2020 6178 2e73 6574 5f79 6c69 6d28 5b2d    ax.set_ylim([-
-00027d50: 206d 6178 7661 6c20 2a20 312e 312c 202b   maxval * 1.1, +
-00027d60: 206d 6178 7661 6c20 2a20 312e 315d 290a   maxval * 1.1]).
-00027d70: 0a20 2020 2023 2041 7869 7320 6c61 6265  .    # Axis labe
-00027d80: 6c73 0a20 2020 2061 782e 7365 745f 796c  ls.    ax.set_yl
-00027d90: 6162 656c 280a 2020 2020 2020 2020 7227  abel(.        r'
-00027da0: 245c 6c6f 675f 5c6d 6174 6872 6567 756c  $\log_\mathregul
-00027db0: 6172 7b31 307d 5b5c 7461 755e 5c6d 6174  ar{10}[\tau^\mat
-00027dc0: 6872 6567 756c 6172 7b2d 317d 5f7b 5c6d  hregular{-1}_{\m
-00027dd0: 6174 6872 6567 756c 6172 7b65 7870 7d7d  athregular{exp}}
-00027de0: 5d24 202d 2024 5c6c 6f67 5f5c 6d61 7468  ]$ - $\log_\math
-00027df0: 7265 6775 6c61 727b 3130 7d5b 5c74 6175  regular{10}[\tau
-00027e00: 5e5c 6d61 7468 7265 6775 6c61 727b 2d31  ^\mathregular{-1
-00027e10: 7d5f 7b5c 6d61 7468 7265 6775 6c61 727b  }_{\mathregular{
-00027e20: 6669 747d 7d5d 2427 2023 206e 6f71 610a  fit}}]$' # noqa.
-00027e30: 2020 2020 290a 0a20 2020 2023 2053 6574      )..    # Set
-00027e40: 2078 2074 6963 6b20 666f 726d 6174 7469   x tick formatti
-00027e50: 6e67 0a20 2020 2067 7569 2e73 6574 5f72  ng.    gui.set_r
-00027e60: 6174 655f 7874 6963 6b5f 666f 726d 6174  ate_xtick_format
-00027e70: 7469 6e67 2861 782c 2078 5f76 6172 7329  ting(ax, x_vars)
-00027e80: 0a0a 2020 2020 7265 7475 726e 0a0a 0a64  ..    return...d
-00027e90: 6566 2077 7269 7465 5f6d 6f64 656c 5f70  ef write_model_p
-00027ea0: 6172 616d 7328 6d6f 6465 6c3a 204c 6f67  arams(model: Log
-00027eb0: 5461 7554 4d6f 6465 6c20 7c20 4d75 6c74  TauTModel | Mult
-00027ec0: 694c 6f67 5461 7554 4d6f 6465 6c20 7c20  iLogTauTModel | 
-00027ed0: 4c6f 6754 6175 484d 6f64 656c 207c 204d  LogTauHModel | M
-00027ee0: 756c 7469 4c6f 6754 6175 484d 6f64 656c  ultiLogTauHModel
-00027ef0: 2c20 2320 6e6f 7161 0a20 2020 2020 2020  , # noqa.       
-00027f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027f10: 6669 6c65 5f6e 616d 653a 2073 7472 2c20  file_name: str, 
-00027f20: 7665 7262 6f73 653a 2062 6f6f 6c20 3d20  verbose: bool = 
-00027f30: 5472 7565 2920 2d3e 204e 6f6e 653a 0a20  True) -> None:. 
-00027f40: 2020 2027 2727 0a20 2020 2057 7269 7465     '''.    Write
-00027f50: 7320 6669 7474 6564 2061 6e64 2066 6978  s fitted and fix
-00027f60: 6564 2070 6172 616d 6574 6572 7320 6f66  ed parameters of
-00027f70: 206d 6f64 656c 2873 2920 746f 2066 696c   model(s) to fil
-00027f80: 650a 0a20 2020 2050 6172 616d 6574 6572  e..    Parameter
-00027f90: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  s.    ----------
-00027fa0: 0a20 2020 206d 6f64 656c 733a 206c 6973  .    models: lis
-00027fb0: 745b 4c6f 6754 6175 544d 6f64 656c 207c  t[LogTauTModel |
-00027fc0: 204d 756c 7469 4c6f 6754 6175 544d 6f64   MultiLogTauTMod
-00027fd0: 656c 207c 204c 6f67 5461 7548 4d6f 6465  el | LogTauHMode
-00027fe0: 6c20 7c20 4d75 6c74 694c 6f67 5461 7548  l | MultiLogTauH
-00027ff0: 4d6f 6465 6c5d 0a20 2020 2020 2020 204d  Model].        M
-00028000: 6f64 656c 732c 206f 6e65 2070 6572 2074  odels, one per t
-00028010: 656d 7065 7261 7475 7265 0a20 2020 2066  emperature.    f
-00028020: 696c 655f 6e61 6d65 3a20 7374 720a 2020  ile_name: str.  
-00028030: 2020 2020 2020 4e61 6d65 206f 6620 6f75        Name of ou
-00028040: 7470 7574 2066 696c 650a 2020 2020 7665  tput file.    ve
-00028050: 7262 6f73 653a 2062 6f6f 6c2c 2064 6566  rbose: bool, def
-00028060: 6175 6c74 2054 7275 650a 2020 2020 2020  ault True.      
-00028070: 2020 4966 2054 7275 652c 206f 7574 7075    If True, outpu
-00028080: 7420 6669 6c65 206c 6f63 6174 696f 6e20  t file location 
-00028090: 6973 2077 7269 7474 656e 2074 6f20 7465  is written to te
-000280a0: 726d 696e 616c 0a0a 2020 2020 5265 7475  rminal..    Retu
-000280b0: 726e 730a 2020 2020 2d2d 2d2d 2d2d 2d0a  rns.    -------.
-000280c0: 2020 2020 4e6f 6e65 0a20 2020 2027 2727      None.    '''
-000280d0: 2023 206e 6f71 610a 0a20 2020 2069 6620   # noqa..    if 
-000280e0: 7479 7065 286d 6f64 656c 2920 696e 205b  type(model) in [
-000280f0: 4d75 6c74 694c 6f67 5461 7554 4d6f 6465  MultiLogTauTMode
-00028100: 6c2c 204d 756c 7469 4c6f 6754 6175 484d  l, MultiLogTauHM
-00028110: 6f64 656c 5d3a 0a20 2020 2020 2020 206c  odel]:.        l
-00028120: 6f67 6d6f 6465 6c73 203d 206d 6f64 656c  ogmodels = model
-00028130: 2e6c 6f67 6d6f 6465 6c73 0a20 2020 2065  .logmodels.    e
-00028140: 6c73 653a 0a20 2020 2020 2020 206c 6f67  lse:.        log
-00028150: 6d6f 6465 6c73 203d 205b 6d6f 6465 6c5d  models = [model]
-00028160: 0a0a 2020 2020 6620 3d20 6f70 656e 2866  ..    f = open(f
-00028170: 696c 655f 6e61 6d65 2c20 2777 272c 2065  ile_name, 'w', e
-00028180: 6e63 6f64 696e 673d 2775 7466 2d38 2729  ncoding='utf-8')
-00028190: 0a0a 2020 2020 2320 5772 6974 6520 6561  ..    # Write ea
-000281a0: 6368 2074 6572 6d27 7320 6e61 6d65 2c20  ch term's name, 
-000281b0: 6669 7420 7661 7273 2c20 7374 6465 762c  fit vars, stdev,
-000281c0: 2061 6e64 2066 6978 2076 6172 730a 2020   and fix vars.  
-000281d0: 2020 666f 7220 6c6f 676d 6f64 656c 2069    for logmodel i
-000281e0: 6e20 6c6f 676d 6f64 656c 733a 0a20 2020  n logmodels:.   
-000281f0: 2020 2020 2066 2e77 7269 7465 2827 7b7d       f.write('{}
-00028200: 5c6e 272e 666f 726d 6174 286c 6f67 6d6f  \n'.format(logmo
-00028210: 6465 6c2e 4e41 4d45 2929 0a20 2020 2020  del.NAME)).     
-00028220: 2020 2069 6620 6c65 6e28 6c6f 676d 6f64     if len(logmod
-00028230: 656c 2e66 6974 5f76 6172 732e 6b65 7973  el.fit_vars.keys
-00028240: 2829 293a 0a20 2020 2020 2020 2020 2020  ()):.           
-00028250: 2066 2e77 7269 7465 2827 4669 7474 6564   f.write('Fitted
-00028260: 2054 6572 6d73 3a20 5661 6c75 6520 616e   Terms: Value an
-00028270: 6420 5374 616e 6461 7264 2044 6576 6961  d Standard Devia
-00028280: 7469 6f6e 3a5c 6e27 290a 2020 2020 2020  tion:\n').      
-00028290: 2020 2020 2020 666f 7220 6e61 6d65 2069        for name i
-000282a0: 6e20 6c6f 676d 6f64 656c 2e66 6974 5f76  n logmodel.fit_v
-000282b0: 6172 732e 6b65 7973 2829 3a0a 2020 2020  ars.keys():.    
-000282c0: 2020 2020 2020 2020 2020 2020 662e 7772              f.wr
-000282d0: 6974 6528 277b 3a3e 367d 207b 3a20 312e  ite('{:>6} {: 1.
-000282e0: 3845 7d20 7b3a 2031 2e38 457d 207b 7d5c  8E} {: 1.8E} {}\
-000282f0: 6e27 2e66 6f72 6d61 7428 0a20 2020 2020  n'.format(.     
-00028300: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00028310: 616d 652c 0a20 2020 2020 2020 2020 2020  ame,.           
-00028320: 2020 2020 2020 2020 206c 6f67 6d6f 6465           logmode
-00028330: 6c2e 6669 6e61 6c5f 7661 725f 7661 6c75  l.final_var_valu
-00028340: 6573 5b6e 616d 655d 2c0a 2020 2020 2020  es[name],.      
-00028350: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-00028360: 676d 6f64 656c 2e66 6974 5f73 7464 6576  gmodel.fit_stdev
-00028370: 5b6e 616d 655d 2c0a 2020 2020 2020 2020  [name],.        
-00028380: 2020 2020 2020 2020 2020 2020 6c6f 676d              logm
-00028390: 6f64 656c 2e55 4e49 5453 5b6e 616d 655d  odel.UNITS[name]
-000283a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000283b0: 2029 290a 2020 2020 2020 2020 6966 206c   )).        if l
-000283c0: 656e 286c 6f67 6d6f 6465 6c2e 6669 785f  en(logmodel.fix_
-000283d0: 7661 7273 2e6b 6579 7328 2929 3a0a 2020  vars.keys()):.  
-000283e0: 2020 2020 2020 2020 2020 662e 7772 6974            f.writ
-000283f0: 6528 2746 6978 6564 2054 6572 6d73 3a20  e('Fixed Terms: 
-00028400: 5661 6c75 6573 5c6e 2729 0a20 2020 2020  Values\n').     
-00028410: 2020 2020 2020 2066 6f72 206e 616d 6520         for name 
-00028420: 696e 206c 6f67 6d6f 6465 6c2e 6669 785f  in logmodel.fix_
-00028430: 7661 7273 2e6b 6579 7328 293a 0a20 2020  vars.keys():.   
-00028440: 2020 2020 2020 2020 2020 2020 2066 2e77               f.w
-00028450: 7269 7465 2827 7b3a 3e36 7d20 7b3a 2031  rite('{:>6} {: 1
-00028460: 2e38 457d 207b 7d5c 6e27 2e66 6f72 6d61  .8E} {}\n'.forma
-00028470: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
-00028480: 2020 2020 2020 206e 616d 652c 0a20 2020         name,.   
-00028490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000284a0: 206c 6f67 6d6f 6465 6c2e 6669 6e61 6c5f   logmodel.final_
-000284b0: 7661 725f 7661 6c75 6573 5b6e 616d 655d  var_values[name]
-000284c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000284d0: 2020 2020 2020 6c6f 676d 6f64 656c 2e55        logmodel.U
-000284e0: 4e49 5453 5b6e 616d 655d 0a20 2020 2020  NITS[name].     
-000284f0: 2020 2020 2020 2020 2020 2029 290a 2020             )).  
-00028500: 2020 2020 2020 662e 7772 6974 6528 275c        f.write('\
-00028510: 6e27 290a 0a20 2020 2069 6620 7665 7262  n')..    if verb
-00028520: 6f73 653a 0a20 2020 2020 2020 2075 742e  ose:.        ut.
-00028530: 6370 7269 6e74 280a 2020 2020 2020 2020  cprint(.        
-00028540: 2020 2020 275c 6e20 5265 6c61 7861 7469      '\n Relaxati
-00028550: 6f6e 204d 6f64 656c 2070 6172 616d 6574  on Model paramet
-00028560: 6572 7320 7772 6974 7465 6e20 746f 205c  ers written to \
-00028570: 6e20 7b7d 5c6e 272e 666f 726d 6174 280a  n {}\n'.format(.
-00028580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028590: 6669 6c65 5f6e 616d 650a 2020 2020 2020  file_name.      
-000285a0: 2020 2020 2020 292c 0a20 2020 2020 2020        ),.       
-000285b0: 2020 2020 2027 6379 616e 270a 2020 2020       'cyan'.    
-000285c0: 2020 2020 290a 0a20 2020 2072 6574 7572      )..    retur
-000285d0: 6e0a 0a0a 6465 6620 7772 6974 655f 6d6f  n...def write_mo
-000285e0: 6465 6c5f 6461 7461 2864 6174 6173 6574  del_data(dataset
-000285f0: 3a20 5461 7554 4461 7461 7365 7420 7c20  : TauTDataset | 
-00028600: 5461 7548 4461 7461 7365 742c 0a20 2020  TauHDataset,.   
-00028610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028620: 2020 6d6f 6465 6c3a 204c 6f67 5461 7554    model: LogTauT
-00028630: 4d6f 6465 6c20 7c20 4d75 6c74 694c 6f67  Model | MultiLog
-00028640: 5461 7554 4d6f 6465 6c20 7c20 4c6f 6754  TauTModel | LogT
-00028650: 6175 484d 6f64 656c 207c 204d 756c 7469  auHModel | Multi
-00028660: 4c6f 6754 6175 484d 6f64 656c 2c20 2320  LogTauHModel, # 
-00028670: 6e6f 7161 0a20 2020 2020 2020 2020 2020  noqa.           
-00028680: 2020 2020 2020 2020 2020 6669 6c65 5f6e            file_n
-00028690: 616d 653a 2073 7472 2c20 7665 7262 6f73  ame: str, verbos
-000286a0: 653a 2062 6f6f 6c20 3d20 5472 7565 2920  e: bool = True) 
-000286b0: 2d3e 204e 6f6e 653a 0a20 2020 2027 2727  -> None:.    '''
-000286c0: 0a20 2020 2043 7265 6174 6573 2066 696c  .    Creates fil
-000286d0: 6520 636f 6e74 6169 6e69 6e67 2072 6174  e containing rat
-000286e0: 6520 7673 2074 656d 7065 7261 7475 7265  e vs temperature
-000286f0: 2f66 6965 6c64 2063 616c 6375 6c61 7465  /field calculate
-00028700: 6420 7573 696e 6720 6d6f 6465 6c0a 2020  d using model.  
-00028710: 2020 7061 7261 6d65 7465 7273 0a0a 2020    parameters..  
-00028720: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
-00028730: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-00028740: 6461 7461 7365 743a 2054 6175 5444 6174  dataset: TauTDat
-00028750: 6173 6574 207c 2054 6175 4844 6174 6173  aset | TauHDatas
-00028760: 6574 0a20 2020 2020 2020 2044 6174 6173  et.        Datas
-00028770: 6574 2074 6f20 7768 6963 6820 6120 6d6f  et to which a mo
-00028780: 6465 6c20 7761 7320 7375 6363 6573 7366  del was successf
-00028790: 756c 6c79 2066 6974 7465 6420 2869 2e65  ully fitted (i.e
-000287a0: 2e20 6669 745f 7374 6174 7573 3d54 7275  . fit_status=Tru
-000287b0: 6529 0a20 2020 206d 6f64 656c 3a20 4c6f  e).    model: Lo
-000287c0: 6754 6175 544d 6f64 656c 207c 204d 756c  gTauTModel | Mul
-000287d0: 7469 4c6f 6754 6175 544d 6f64 656c 207c  tiLogTauTModel |
-000287e0: 204c 6f67 5461 7548 4d6f 6465 6c20 7c20   LogTauHModel | 
-000287f0: 4d75 6c74 694c 6f67 5461 7548 4d6f 6465  MultiLogTauHMode
-00028800: 6c0a 2020 2020 2020 2020 4d6f 6465 6c20  l.        Model 
-00028810: 7768 6963 6820 6861 7320 6265 656e 2066  which has been f
-00028820: 6974 7465 6420 746f 2064 6174 6173 6574  itted to dataset
-00028830: 0a20 2020 2066 696c 655f 6e61 6d65 3a20  .    file_name: 
-00028840: 7374 720a 2020 2020 2020 2020 4e61 6d65  str.        Name
-00028850: 206f 6620 6f75 7470 7574 2066 696c 650a   of output file.
-00028860: 2020 2020 7665 7262 6f73 653a 2062 6f6f      verbose: boo
-00028870: 6c2c 2064 6566 6175 6c74 2054 7275 650a  l, default True.
-00028880: 2020 2020 2020 2020 4966 2054 7275 652c          If True,
-00028890: 206f 7574 7075 7420 6669 6c65 206c 6f63   output file loc
-000288a0: 6174 696f 6e20 6973 2077 7269 7474 656e  ation is written
-000288b0: 2074 6f20 7465 726d 696e 616c 0a0a 2020   to terminal..  
-000288c0: 2020 5265 7475 726e 730a 2020 2020 2d2d    Returns.    --
-000288d0: 2d2d 2d2d 2d0a 2020 2020 4e6f 6e65 0a20  -----.    None. 
-000288e0: 2020 2027 2727 0a0a 2020 2020 6966 206e     '''..    if n
-000288f0: 6f74 206d 6f64 656c 2e66 6974 5f73 7461  ot model.fit_sta
-00028900: 7475 733a 0a20 2020 2020 2020 2072 6574  tus:.        ret
-00028910: 7572 6e0a 0a20 2020 2069 6620 6973 696e  urn..    if isin
-00028920: 7374 616e 6365 2864 6174 6173 6574 2c20  stance(dataset, 
-00028930: 5461 7548 4461 7461 7365 7429 3a0a 2020  TauHDataset):.  
-00028940: 2020 2020 2020 785f 7661 7273 203d 2064        x_vars = d
-00028950: 6174 6173 6574 2e66 6965 6c64 730a 2020  ataset.fields.  
-00028960: 2020 2020 2020 785f 7661 725f 6c61 6265        x_var_labe
-00028970: 6c20 3d20 2748 2028 4f65 2927 0a0a 2020  l = 'H (Oe)'..  
-00028980: 2020 656c 6966 2069 7369 6e73 7461 6e63    elif isinstanc
-00028990: 6528 6461 7461 7365 742c 2054 6175 5444  e(dataset, TauTD
-000289a0: 6174 6173 6574 293a 0a20 2020 2020 2020  ataset):.       
-000289b0: 2078 5f76 6172 7320 3d20 6461 7461 7365   x_vars = datase
-000289c0: 742e 7465 6d70 6572 6174 7572 6573 0a20  t.temperatures. 
-000289d0: 2020 2020 2020 2078 5f76 6172 5f6c 6162         x_var_lab
-000289e0: 656c 203d 2027 5420 284b 2927 0a0a 2020  el = 'T (K)'..  
-000289f0: 2020 6966 2074 7970 6528 6d6f 6465 6c29    if type(model)
-00028a00: 2069 6e20 5b4d 756c 7469 4c6f 6754 6175   in [MultiLogTau
-00028a10: 544d 6f64 656c 2c20 4d75 6c74 694c 6f67  TModel, MultiLog
-00028a20: 5461 7548 4d6f 6465 6c5d 3a0a 2020 2020  TauHModel]:.    
-00028a30: 2020 2020 6c6f 676d 6f64 656c 7320 3d20      logmodels = 
-00028a40: 6d6f 6465 6c2e 6c6f 676d 6f64 656c 730a  model.logmodels.
-00028a50: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00028a60: 2020 6c6f 676d 6f64 656c 7320 3d20 5b6d    logmodels = [m
-00028a70: 6f64 656c 5d0a 0a20 2020 2066 203d 206f  odel]..    f = o
-00028a80: 7065 6e28 6669 6c65 5f6e 616d 652c 2027  pen(file_name, '
-00028a90: 7727 2c20 656e 636f 6469 6e67 3d27 7574  w', encoding='ut
-00028aa0: 662d 3827 290a 0a20 2020 2078 5f76 6172  f-8')..    x_var
-00028ab0: 735f 6772 6964 203d 206e 702e 6c6f 6773  s_grid = np.logs
-00028ac0: 7061 6365 280a 2020 2020 2020 2020 6e70  pace(.        np
-00028ad0: 2e6c 6f67 3130 286e 702e 6d69 6e28 785f  .log10(np.min(x_
-00028ae0: 7661 7273 2929 2c0a 2020 2020 2020 2020  vars)),.        
-00028af0: 6e70 2e6c 6f67 3130 286e 702e 6d61 7828  np.log10(np.max(
-00028b00: 785f 7661 7273 2929 2c0a 2020 2020 2020  x_vars)),.      
-00028b10: 2020 3130 300a 2020 2020 290a 0a20 2020    100.    )..   
-00028b20: 2066 2e77 7269 7465 2827 7b3a 3e39 7d20   f.write('{:>9} 
-00028b30: 272e 666f 726d 6174 2878 5f76 6172 5f6c  '.format(x_var_l
-00028b40: 6162 656c 2929 0a20 2020 2066 6f72 206c  abel)).    for l
-00028b50: 6f67 6d6f 6465 6c20 696e 206c 6f67 6d6f  ogmodel in logmo
-00028b60: 6465 6c73 3a0a 2020 2020 2020 2020 662e  dels:.        f.
-00028b70: 7772 6974 6528 277b 3a3e 377d 2072 6174  write('{:>7} rat
-00028b80: 6520 272e 666f 726d 6174 286c 6f67 6d6f  e '.format(logmo
-00028b90: 6465 6c2e 4e41 4d45 2929 0a20 2020 2069  del.NAME)).    i
-00028ba0: 6620 6c65 6e28 6c6f 676d 6f64 656c 7329  f len(logmodels)
-00028bb0: 203e 2031 3a0a 2020 2020 2020 2020 662e   > 1:.        f.
-00028bc0: 7772 6974 6528 2720 2054 6f74 616c 2072  write('  Total r
-00028bd0: 6174 6520 2873 5e2d 3129 2729 0a20 2020  ate (s^-1)').   
-00028be0: 2066 2e77 7269 7465 2827 5c6e 2729 0a0a   f.write('\n')..
-00028bf0: 2020 2020 666f 7220 6772 6964 5f70 7420      for grid_pt 
-00028c00: 696e 2078 5f76 6172 735f 6772 6964 3a0a  in x_vars_grid:.
-00028c10: 2020 2020 2020 2020 662e 7772 6974 6528          f.write(
-00028c20: 277b 3a20 392e 3566 7d20 272e 666f 726d  '{: 9.5f} '.form
-00028c30: 6174 2867 7269 645f 7074 2929 0a20 2020  at(grid_pt)).   
-00028c40: 2020 2020 2074 6f74 616c 203d 2030 2e0a       total = 0..
-00028c50: 2020 2020 2020 2020 666f 7220 6c6f 676d          for logm
-00028c60: 6f64 656c 2069 6e20 6c6f 676d 6f64 656c  odel in logmodel
-00028c70: 733a 0a20 2020 2020 2020 2020 2020 2072  s:.            r
-00028c80: 6174 6520 3d20 3130 2a2a 6c6f 676d 6f64  ate = 10**logmod
-00028c90: 656c 2e6d 6f64 656c 280a 2020 2020 2020  el.model(.      
-00028ca0: 2020 2020 2020 2020 2020 6c6f 676d 6f64            logmod
-00028cb0: 656c 2e66 696e 616c 5f76 6172 5f76 616c  el.final_var_val
-00028cc0: 7565 732c 0a20 2020 2020 2020 2020 2020  ues,.           
-00028cd0: 2020 2020 205b 6772 6964 5f70 745d 0a20       [grid_pt]. 
-00028ce0: 2020 2020 2020 2020 2020 2029 5b30 5d0a             )[0].
-00028cf0: 2020 2020 2020 2020 2020 2020 662e 7772              f.wr
-00028d00: 6974 6528 277b 3a2e 3645 7d20 272e 666f  ite('{:.6E} '.fo
-00028d10: 726d 6174 2872 6174 6529 290a 2020 2020  rmat(rate)).    
-00028d20: 2020 2020 2020 2020 746f 7461 6c20 2b3d          total +=
-00028d30: 2072 6174 650a 2020 2020 2020 2020 6966   rate.        if
-00028d40: 206c 656e 286c 6f67 6d6f 6465 6c73 2920   len(logmodels) 
-00028d50: 3e20 313a 0a20 2020 2020 2020 2020 2020  > 1:.           
-00028d60: 2066 2e77 7269 7465 2827 7b3a 2e36 457d   f.write('{:.6E}
-00028d70: 272e 666f 726d 6174 2874 6f74 616c 2929  '.format(total))
-00028d80: 0a20 2020 2020 2020 2066 2e77 7269 7465  .        f.write
-00028d90: 2827 5c6e 2729 0a0a 2020 2020 6966 2076  ('\n')..    if v
-00028da0: 6572 626f 7365 3a0a 2020 2020 2020 2020  erbose:.        
-00028db0: 7574 2e63 7072 696e 7428 0a20 2020 2020  ut.cprint(.     
-00028dc0: 2020 2020 2020 2027 5c6e 2052 656c 6178         '\n Relax
-00028dd0: 6174 696f 6e20 6d6f 6465 6c20 cf84 e281  ation model ....
-00028de0: bbc2 b920 7673 207b 7d20 7772 6974 7465  ... vs {} writte
-00028df0: 6e20 746f 205c 6e20 7b7d 5c6e 272e 666f  n to \n {}\n'.fo
-00028e00: 726d 6174 280a 2020 2020 2020 2020 2020  rmat(.          
-00028e10: 2020 2020 2020 785f 7661 725f 6c61 6265        x_var_labe
-00028e20: 6c5b 305d 2c0a 2020 2020 2020 2020 2020  l[0],.          
-00028e30: 2020 2020 2020 6669 6c65 5f6e 616d 650a        file_name.
-00028e40: 2020 2020 2020 2020 2020 2020 292c 0a20              ),. 
-00028e50: 2020 2020 2020 2020 2020 2027 6379 616e             'cyan
-00028e60: 270a 2020 2020 2020 2020 290a 0a20 2020  '.        )..   
-00028e70: 2072 6574 7572 6e0a                       return.
+00022160: 656c 2872 2724 5c6c 6e5c 6c65 6674 5b5c  el(r'$\ln\left[\
+00022170: 7461 755c 7269 6768 745d 2420 245c 6c65  tau\right]$ $\le
+00022180: 6674 285c 6c6e 5c6c 6566 745b 5c6d 6174  ft(\ln\left[\mat
+00022190: 6872 6567 756c 6172 7b73 7d5e 5c6d 6174  hregular{s}^\mat
+000221a0: 6872 6567 756c 6172 7b2d 317d 5c72 6967  hregular{-1}\rig
+000221b0: 6874 5d5c 7269 6768 7429 2427 2920 2320  ht]\right)$') # 
+000221c0: 6e6f 7161 0a0a 2020 2020 6669 672e 7469  noqa..    fig.ti
+000221d0: 6768 745f 6c61 796f 7574 2829 0a0a 2020  ght_layout()..  
+000221e0: 2020 6966 2073 686f 773a 0a20 2020 2020    if show:.     
+000221f0: 2020 2070 6c74 2e73 686f 7728 290a 0a20     plt.show().. 
+00022200: 2020 2069 6620 7361 7665 3a0a 2020 2020     if save:.    
+00022210: 2020 2020 6669 672e 7361 7665 6669 6728      fig.savefig(
+00022220: 7361 7665 5f6e 616d 652c 2064 7069 3d35  save_name, dpi=5
+00022230: 3030 290a 2020 2020 2020 2020 6966 2076  00).        if v
+00022240: 6572 626f 7365 3a0a 2020 2020 2020 2020  erbose:.        
+00022250: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+00022260: 6528 6461 7461 7365 742c 2028 5461 7554  e(dataset, (TauT
+00022270: 4461 7461 7365 7429 293a 0a20 2020 2020  Dataset)):.     
+00022280: 2020 2020 2020 2020 2020 205f 7876 6172             _xvar
+00022290: 203d 2027 5427 0a20 2020 2020 2020 2020   = 'T'.         
+000222a0: 2020 2065 6c69 6620 6973 696e 7374 616e     elif isinstan
+000222b0: 6365 2864 6174 6173 6574 2c20 2854 6175  ce(dataset, (Tau
+000222c0: 4844 6174 6173 6574 2929 3a0a 2020 2020  HDataset)):.    
+000222d0: 2020 2020 2020 2020 2020 2020 5f78 7661              _xva
+000222e0: 7220 3d20 2748 270a 2020 2020 2020 2020  r = 'H'.        
+000222f0: 2020 2020 7574 2e63 7072 696e 7428 0a20      ut.cprint(. 
+00022300: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00022310: 275c 6e20 4669 7474 6564 206c 6e28 7461  '\n Fitted ln(ta
+00022320: 7529 2076 7320 312f 7b5f 7876 6172 7d20  u) vs 1/{_xvar} 
+00022330: 706c 6f74 2073 6176 6564 2074 6f20 5c6e  plot saved to \n
+00022340: 207b 7361 7665 5f6e 616d 657d 5c6e 272c   {save_name}\n',
+00022350: 2023 206e 6f71 610a 2020 2020 2020 2020   # noqa.        
+00022360: 2020 2020 2020 2020 2763 7961 6e27 0a20          'cyan'. 
+00022370: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+00022380: 2020 7265 7475 726e 2066 6967 2c20 6178    return fig, ax
+00022390: 0a0a 0a64 6566 205f 706c 6f74 5f66 6974  ...def _plot_fit
+000223a0: 7465 645f 7469 6d65 7328 6461 7461 7365  ted_times(datase
+000223b0: 743a 2054 6175 5444 6174 6173 6574 207c  t: TauTDataset |
+000223c0: 2054 6175 4844 6174 6173 6574 2c0a 2020   TauHDataset,.  
+000223d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000223e0: 2020 2020 206d 6f64 656c 3a20 4c6f 6754       model: LogT
+000223f0: 6175 544d 6f64 656c 207c 204d 756c 7469  auTModel | Multi
+00022400: 4c6f 6754 6175 544d 6f64 656c 207c 204c  LogTauTModel | L
+00022410: 6f67 5461 7548 4d6f 6465 6c20 7c20 4d75  ogTauHModel | Mu
+00022420: 6c74 694c 6f67 5461 7548 4d6f 6465 6c2c  ltiLogTauHModel,
+00022430: 2023 206e 6f71 610a 2020 2020 2020 2020   # noqa.        
+00022440: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00022450: 6967 3a20 706c 742e 4669 6775 7265 2c20  ig: plt.Figure, 
+00022460: 6178 3a20 706c 742e 4178 6573 293a 0a20  ax: plt.Axes):. 
+00022470: 2020 2027 2727 0a20 2020 2050 6c6f 7473     '''.    Plots
+00022480: 2065 7870 6572 696d 656e 7461 6c20 616e   experimental an
+00022490: 6420 6669 7474 6564 2028 6d6f 6465 6c29  d fitted (model)
+000224a0: 2072 656c 6178 6174 696f 6e20 7261 7465   relaxation rate
+000224b0: 2061 735c 6e0a 2020 2020 6c6e 2874 6175   as\n.    ln(tau
+000224c0: 2920 7673 2031 2f78 7661 7220 7768 6572  ) vs 1/xvar wher
+000224d0: 6520 7876 6172 2069 7320 5420 6f72 2048  e xvar is T or H
+000224e0: 2e0a 0a20 2020 2050 6172 616d 6574 6572  ...    Parameter
+000224f0: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  s.    ----------
+00022500: 0a20 2020 2064 6174 6173 6574 3a20 5461  .    dataset: Ta
+00022510: 7554 4461 7461 7365 7420 7c20 5461 7548  uTDataset | TauH
+00022520: 4461 7461 7365 740a 2020 2020 2020 2020  Dataset.        
+00022530: 4461 7461 7365 7420 746f 2070 6c6f 740a  Dataset to plot.
+00022540: 2020 2020 6d6f 6465 6c3a 204c 6f67 5461      model: LogTa
+00022550: 7554 4d6f 6465 6c20 7c20 4d75 6c74 694c  uTModel | MultiL
+00022560: 6f67 5461 7554 4d6f 6465 6c20 7c20 4c6f  ogTauTModel | Lo
+00022570: 6754 6175 484d 6f64 656c 207c 204d 756c  gTauHModel | Mul
+00022580: 7469 4c6f 6754 6175 484d 6f64 656c 0a20  tiLogTauHModel. 
+00022590: 2020 2020 2020 204d 6f64 656c 2028 6669         Model (fi
+000225a0: 7474 6564 2920 746f 2070 6c6f 740a 2020  tted) to plot.  
+000225b0: 2020 6669 673a 2070 6c74 2e46 6967 7572    fig: plt.Figur
+000225c0: 650a 2020 2020 2020 2020 4d61 7470 6c6f  e.        Matplo
+000225d0: 746c 6962 2046 6967 7572 6520 6f62 6a65  tlib Figure obje
+000225e0: 6374 2075 7365 6420 666f 7220 706c 6f74  ct used for plot
+000225f0: 0a20 2020 2061 783a 2070 6c74 2e41 7865  .    ax: plt.Axe
+00022600: 730a 2020 2020 2020 2020 4d61 7470 6c6f  s.        Matplo
+00022610: 746c 6962 2041 7869 7320 6f62 6a65 6374  tlib Axis object
+00022620: 2075 7365 6420 666f 7220 706c 6f74 0a0a   used for plot..
+00022630: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
+00022640: 2d2d 2d2d 2d2d 2d0a 2020 2020 4e6f 6e65  -------.    None
+00022650: 0a20 2020 2027 2727 0a0a 2020 2020 6966  .    '''..    if
+00022660: 2069 7369 6e73 7461 6e63 6528 6461 7461   isinstance(data
+00022670: 7365 742c 2054 6175 4844 6174 6173 6574  set, TauHDataset
+00022680: 293a 0a20 2020 2020 2020 2078 5f76 6172  ):.        x_var
+00022690: 7320 3d20 6461 7461 7365 742e 6669 656c  s = dataset.fiel
+000226a0: 6473 0a20 2020 2020 2020 2061 782e 7365  ds.        ax.se
+000226b0: 745f 786c 6162 656c 2872 2731 2f48 2024  t_xlabel(r'1/H $
+000226c0: 5c6c 6566 7428 5c6d 6174 6872 6567 756c  \left(\mathregul
+000226d0: 6172 7b4f 657d 5e5c 6d61 7468 7265 6775  ar{Oe}^\mathregu
+000226e0: 6c61 727b 2d31 7d5c 7269 6768 7429 2427  lar{-1}\right)$'
+000226f0: 290a 2020 2020 656c 6966 2069 7369 6e73  ).    elif isins
+00022700: 7461 6e63 6528 6461 7461 7365 742c 2054  tance(dataset, T
+00022710: 6175 5444 6174 6173 6574 293a 0a20 2020  auTDataset):.   
+00022720: 2020 2020 2078 5f76 6172 7320 3d20 6461       x_vars = da
+00022730: 7461 7365 742e 7465 6d70 6572 6174 7572  taset.temperatur
+00022740: 6573 0a20 2020 2020 2020 2061 782e 7365  es.        ax.se
+00022750: 745f 786c 6162 656c 2872 2731 2f54 2024  t_xlabel(r'1/T $
+00022760: 5c6c 6566 7428 5c6d 6174 6872 6567 756c  \left(\mathregul
+00022770: 6172 7b4b 7d5e 5c6d 6174 6872 6567 756c  ar{K}^\mathregul
+00022780: 6172 7b2d 317d 5c72 6967 6874 2924 2729  ar{-1}\right)$')
+00022790: 0a0a 2020 2020 2320 4164 6420 756e 6365  ..    # Add unce
+000227a0: 7274 6169 6e74 6965 7320 6173 2065 7272  rtainties as err
+000227b0: 6f72 6261 7273 0a20 2020 2069 6620 6c65  orbars.    if le
+000227c0: 6e28 6461 7461 7365 742e 7261 7465 5f70  n(dataset.rate_p
+000227d0: 6d29 3a0a 0a20 2020 2020 2020 2023 2043  m):..        # C
+000227e0: 616c 6375 6c61 7465 2074 696d 6520 6572  alculate time er
+000227f0: 726f 7262 6172 730a 2020 2020 2020 2020  rorbars.        
+00022800: 7469 6d65 7320 3d20 312e 202f 2064 6174  times = 1. / dat
+00022810: 6173 6574 2e72 6174 6573 0a20 2020 2020  aset.rates.     
+00022820: 2020 206d 696e 5f74 696d 6520 3d20 312e     min_time = 1.
+00022830: 202f 2028 6461 7461 7365 742e 7261 7465   / (dataset.rate
+00022840: 7320 2b20 6461 7461 7365 742e 7261 7465  s + dataset.rate
+00022850: 5f70 6d5b 312c 203a 5d29 0a20 2020 2020  _pm[1, :]).     
+00022860: 2020 206d 6178 5f74 696d 6520 3d20 312e     max_time = 1.
+00022870: 202f 2028 6461 7461 7365 742e 7261 7465   / (dataset.rate
+00022880: 7320 2d20 6461 7461 7365 742e 7261 7465  s - dataset.rate
+00022890: 5f70 6d5b 302c 203a 5d29 0a0a 2020 2020  _pm[0, :])..    
+000228a0: 2020 2020 6c6e 5f6d 696e 5f74 696d 6520      ln_min_time 
+000228b0: 3d20 6e70 2e6c 6f67 286d 696e 5f74 696d  = np.log(min_tim
+000228c0: 6529 0a20 2020 2020 2020 206c 6e5f 6d61  e).        ln_ma
+000228d0: 785f 7469 6d65 203d 206e 702e 6c6f 6728  x_time = np.log(
+000228e0: 6d61 785f 7469 6d65 290a 0a20 2020 2020  max_time)..     
+000228f0: 2020 206c 6e5f 7469 6d65 5f70 6c75 7320     ln_time_plus 
+00022900: 3d20 6c6e 5f6d 6178 5f74 696d 6520 2d20  = ln_max_time - 
+00022910: 6e70 2e6c 6f67 2874 696d 6573 290a 2020  np.log(times).  
+00022920: 2020 2020 2020 6c6e 5f74 696d 655f 6d69        ln_time_mi
+00022930: 6e75 7320 3d20 6e70 2e6c 6f67 2874 696d  nus = np.log(tim
+00022940: 6573 2920 2d20 6c6e 5f6d 696e 5f74 696d  es) - ln_min_tim
+00022950: 650a 0a20 2020 2020 2020 206c 6e74 696d  e..        lntim
+00022960: 655f 6d70 203d 206e 702e 6172 7261 7928  e_mp = np.array(
+00022970: 5b6c 6e5f 7469 6d65 5f6d 696e 7573 2c20  [ln_time_minus, 
+00022980: 6c6e 5f74 696d 655f 706c 7573 5d29 0a0a  ln_time_plus])..
+00022990: 2020 2020 2020 2020 6178 2e65 7272 6f72          ax.error
+000229a0: 6261 7228 0a20 2020 2020 2020 2020 2020  bar(.           
+000229b0: 2031 2e20 2f20 785f 7661 7273 2c0a 2020   1. / x_vars,.  
+000229c0: 2020 2020 2020 2020 2020 6e70 2e6c 6f67            np.log
+000229d0: 2874 696d 6573 292c 0a20 2020 2020 2020  (times),.       
+000229e0: 2020 2020 2079 6572 723d 6c6e 7469 6d65       yerr=lntime
+000229f0: 5f6d 702c 0a20 2020 2020 2020 2020 2020  _mp,.           
+00022a00: 206d 6172 6b65 723d 276f 272c 0a20 2020   marker='o',.   
+00022a10: 2020 2020 2020 2020 206c 773d 302c 0a20           lw=0,. 
+00022a20: 2020 2020 2020 2020 2020 2065 6c69 6e65             eline
+00022a30: 7769 6474 683d 312e 352c 0a20 2020 2020  width=1.5,.     
+00022a40: 2020 2020 2020 2066 696c 6c73 7479 6c65         fillstyle
+00022a50: 3d27 6e6f 6e65 272c 0a20 2020 2020 2020  ='none',.       
+00022a60: 2020 2020 206c 6162 656c 3d27 4578 7065       label='Expe
+00022a70: 7269 6d65 6e74 272c 0a20 2020 2020 2020  riment',.       
+00022a80: 2020 2020 2063 6f6c 6f72 3d27 626c 6163       color='blac
+00022a90: 6b27 0a20 2020 2020 2020 2029 0a20 2020  k'.        ).   
+00022aa0: 2065 6c73 653a 0a20 2020 2020 2020 2061   else:.        a
+00022ab0: 782e 706c 6f74 280a 2020 2020 2020 2020  x.plot(.        
+00022ac0: 2020 2020 312e 202f 2078 5f76 6172 732c      1. / x_vars,
+00022ad0: 0a20 2020 2020 2020 2020 2020 206e 702e  .            np.
+00022ae0: 6c6f 6728 312e 202f 2064 6174 6173 6574  log(1. / dataset
+00022af0: 2e72 6174 6573 292c 0a20 2020 2020 2020  .rates),.       
+00022b00: 2020 2020 206d 6172 6b65 723d 276f 272c       marker='o',
+00022b10: 0a20 2020 2020 2020 2020 2020 206c 773d  .            lw=
+00022b20: 302c 0a20 2020 2020 2020 2020 2020 2066  0,.            f
+00022b30: 696c 6c73 7479 6c65 3d27 6e6f 6e65 272c  illstyle='none',
+00022b40: 0a20 2020 2020 2020 2020 2020 206c 6162  .            lab
+00022b50: 656c 3d27 4578 7065 7269 6d65 6e74 272c  el='Experiment',
+00022b60: 0a20 2020 2020 2020 2020 2020 2063 6f6c  .            col
+00022b70: 6f72 3d27 626c 6163 6b27 0a20 2020 2020  or='black'.     
+00022b80: 2020 2029 0a0a 2020 2020 785f 7661 7273     )..    x_vars
+00022b90: 5f67 7269 6420 3d20 6e70 2e6c 6f67 7370  _grid = np.logsp
+00022ba0: 6163 6528 0a20 2020 2020 2020 206e 702e  ace(.        np.
+00022bb0: 6c6f 6731 3028 6e70 2e6d 696e 2878 5f76  log10(np.min(x_v
+00022bc0: 6172 7329 292c 0a20 2020 2020 2020 206e  ars)),.        n
+00022bd0: 702e 6c6f 6731 3028 6e70 2e6d 6178 2878  p.log10(np.max(x
+00022be0: 5f76 6172 7329 292c 0a20 2020 2020 2020  _vars)),.       
+00022bf0: 2035 3030 0a20 2020 2029 0a0a 2020 2020   500.    )..    
+00022c00: 6966 2074 7970 6528 6d6f 6465 6c29 2069  if type(model) i
+00022c10: 6e20 5b4d 756c 7469 4c6f 6754 6175 544d  n [MultiLogTauTM
+00022c20: 6f64 656c 2c20 4d75 6c74 694c 6f67 5461  odel, MultiLogTa
+00022c30: 7548 4d6f 6465 6c5d 3a0a 2020 2020 2020  uHModel]:.      
+00022c40: 2020 6c6f 676d 6f64 656c 7320 3d20 6d6f    logmodels = mo
+00022c50: 6465 6c2e 6c6f 676d 6f64 656c 730a 2020  del.logmodels.  
+00022c60: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00022c70: 6c6f 676d 6f64 656c 7320 3d20 5b6d 6f64  logmodels = [mod
+00022c80: 656c 5d0a 0a20 2020 2066 6f72 206c 6f67  el]..    for log
+00022c90: 6d6f 6465 6c20 696e 206c 6f67 6d6f 6465  model in logmode
+00022ca0: 6c73 3a0a 0a20 2020 2020 2020 2069 6620  ls:..        if 
+00022cb0: 7479 7065 286c 6f67 6d6f 6465 6c29 2069  type(logmodel) i
+00022cc0: 7320 4c6f 674f 7262 6163 684d 6f64 656c  s LogOrbachModel
+00022cd0: 3a0a 2020 2020 2020 2020 2020 2020 6c61  :.            la
+00022ce0: 6265 6c5f 6669 7420 3d20 275c 6e46 6974  bel_fit = '\nFit
+00022cf0: 2077 6974 6827 0a20 2020 2020 2020 2020   with'.         
+00022d00: 2020 206c 6162 656c 5f66 6974 202b 3d20     label_fit += 
+00022d10: 275c 6e27 202b 2072 277b 7d20 7b3a 362e  '\n' + r'{} {:6.
+00022d20: 3266 7d20 7327 2e66 6f72 6d61 7428 0a20  2f} s'.format(. 
+00022d30: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00022d40: 6f67 6d6f 6465 6c2e 5641 524e 414d 4553  ogmodel.VARNAMES
+00022d50: 5f4d 4d5b 2775 5f65 6666 275d 2c0a 2020  _MM['u_eff'],.  
+00022d60: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+00022d70: 676d 6f64 656c 2e66 696e 616c 5f76 6172  gmodel.final_var
+00022d80: 5f76 616c 7565 735b 2775 5f65 6666 275d  _values['u_eff']
+00022d90: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+00022da0: 2020 2020 2020 2020 2020 206c 6162 656c             label
+00022db0: 5f66 6974 202b 3d20 275c 6e27 202b 2072  _fit += '\n' + r
+00022dc0: 277b 7d20 7b3a 3034 2e33 657d 272e 666f  '{} {:04.3e}'.fo
+00022dd0: 726d 6174 280a 2020 2020 2020 2020 2020  rmat(.          
+00022de0: 2020 2020 2020 6c6f 676d 6f64 656c 2e56        logmodel.V
+00022df0: 4152 4e41 4d45 535f 4d4d 5b27 4127 5d2c  ARNAMES_MM['A'],
+00022e00: 206c 6f67 6d6f 6465 6c2e 6669 6e61 6c5f   logmodel.final_
+00022e10: 7661 725f 7661 6c75 6573 5b27 4127 5d0a  var_values['A'].
+00022e20: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00022e30: 2020 2020 2020 656c 6966 2074 7970 6528        elif type(
+00022e40: 6c6f 676d 6f64 656c 2920 6973 204c 6f67  logmodel) is Log
+00022e50: 5261 6d61 6e4d 6f64 656c 3a0a 2020 2020  RamanModel:.    
+00022e60: 2020 2020 2020 2020 6c61 6265 6c5f 6669          label_fi
+00022e70: 7420 3d20 275c 6e46 6974 2077 6974 6827  t = '\nFit with'
+00022e80: 0a20 2020 2020 2020 2020 2020 206c 6162  .            lab
+00022e90: 656c 5f66 6974 202b 3d20 275c 6e27 202b  el_fit += '\n' +
+00022ea0: 2072 277b 7d20 7b3a 362e 3266 7d20 7327   r'{} {:6.2f} s'
+00022eb0: 2e66 6f72 6d61 7428 0a20 2020 2020 2020  .format(.       
+00022ec0: 2020 2020 2020 2020 206c 6f67 6d6f 6465           logmode
+00022ed0: 6c2e 5641 524e 414d 4553 5f4d 4d5b 2752  l.VARNAMES_MM['R
+00022ee0: 275d 2c20 6c6f 676d 6f64 656c 2e66 696e  '], logmodel.fin
+00022ef0: 616c 5f76 6172 5f76 616c 7565 735b 2752  al_var_values['R
+00022f00: 275d 0a20 2020 2020 2020 2020 2020 2029  '].            )
+00022f10: 0a20 2020 2020 2020 2020 2020 206c 6162  .            lab
+00022f20: 656c 5f66 6974 202b 3d20 275c 6e27 202b  el_fit += '\n' +
+00022f30: 2072 277b 7d20 7b3a 3034 2e33 657d 272e   r'{} {:04.3e}'.
+00022f40: 666f 726d 6174 280a 2020 2020 2020 2020  format(.        
+00022f50: 2020 2020 2020 2020 6c6f 676d 6f64 656c          logmodel
+00022f60: 2e56 4152 4e41 4d45 535f 4d4d 5b27 6e27  .VARNAMES_MM['n'
+00022f70: 5d2c 206c 6f67 6d6f 6465 6c2e 6669 6e61  ], logmodel.fina
+00022f80: 6c5f 7661 725f 7661 6c75 6573 5b27 6e27  l_var_values['n'
+00022f90: 5d0a 2020 2020 2020 2020 2020 2020 290a  ].            ).
+00022fa0: 2020 2020 2020 2020 656c 6966 2074 7970          elif typ
+00022fb0: 6528 6c6f 676d 6f64 656c 2920 6973 204c  e(logmodel) is L
+00022fc0: 6f67 5154 4d4d 6f64 656c 3a0a 2020 2020  ogQTMModel:.    
+00022fd0: 2020 2020 2020 2020 6c61 6265 6c5f 6669          label_fi
+00022fe0: 7420 3d20 275c 6e46 6974 2077 6974 6827  t = '\nFit with'
+00022ff0: 0a20 2020 2020 2020 2020 2020 206c 6162  .            lab
+00023000: 656c 5f66 6974 202b 3d20 275c 6e27 202b  el_fit += '\n' +
+00023010: 2072 277b 7d20 7b3a 362e 3266 7d20 7327   r'{} {:6.2f} s'
+00023020: 2e66 6f72 6d61 7428 0a20 2020 2020 2020  .format(.       
+00023030: 2020 2020 2020 2020 206c 6f67 6d6f 6465           logmode
+00023040: 6c2e 5641 524e 414d 4553 5f4d 4d5b 2751  l.VARNAMES_MM['Q
+00023050: 275d 2c20 6c6f 676d 6f64 656c 2e66 696e  '], logmodel.fin
+00023060: 616c 5f76 6172 5f76 616c 7565 735b 2751  al_var_values['Q
+00023070: 275d 0a20 2020 2020 2020 2020 2020 2029  '].            )
+00023080: 0a20 2020 2020 2020 2065 6c69 6620 7479  .        elif ty
+00023090: 7065 286c 6f67 6d6f 6465 6c29 2069 7320  pe(logmodel) is 
+000230a0: 4c6f 6744 6972 6563 744d 6f64 656c 3a0a  LogDirectModel:.
+000230b0: 2020 2020 2020 2020 2020 2020 6c61 6265              labe
+000230c0: 6c5f 6669 7420 3d20 275c 6e46 6974 2077  l_fit = '\nFit w
+000230d0: 6974 6827 0a20 2020 2020 2020 2020 2020  ith'.           
+000230e0: 206c 6162 656c 5f66 6974 202b 3d20 275c   label_fit += '\
+000230f0: 6e27 202b 2072 277b 7d20 7b3a 362e 3266  n' + r'{} {:6.2f
+00023100: 7d20 7327 2e66 6f72 6d61 7428 0a20 2020  } s'.format(.   
+00023110: 2020 2020 2020 2020 2020 2020 206c 6f67               log
+00023120: 6d6f 6465 6c2e 5641 524e 414d 4553 5f4d  model.VARNAMES_M
+00023130: 4d5b 2744 275d 2c20 6c6f 676d 6f64 656c  M['D'], logmodel
+00023140: 2e66 696e 616c 5f76 6172 5f76 616c 7565  .final_var_value
+00023150: 735b 2744 275d 0a20 2020 2020 2020 2020  s['D'].         
+00023160: 2020 2029 0a20 2020 2020 2020 206d 6f64     ).        mod
+00023170: 656c 5f72 6174 6573 203d 2031 302a 2a6c  el_rates = 10**l
+00023180: 6f67 6d6f 6465 6c2e 6d6f 6465 6c28 0a20  ogmodel.model(. 
+00023190: 2020 2020 2020 2020 2020 206c 6f67 6d6f             logmo
+000231a0: 6465 6c2e 6669 6e61 6c5f 7661 725f 7661  del.final_var_va
+000231b0: 6c75 6573 2c0a 2020 2020 2020 2020 2020  lues,.          
+000231c0: 2020 785f 7661 7273 5f67 7269 642c 0a20    x_vars_grid,. 
+000231d0: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+000231e0: 2020 2320 5472 696d 206d 6f64 656c 2072    # Trim model r
+000231f0: 6174 6573 2074 6f20 7365 6e73 6962 6c65  ates to sensible
+00023200: 2076 616c 7565 730a 2020 2020 2020 2020   values.        
+00023210: 7661 6c69 645f 696e 7420 3d20 6e70 2e77  valid_int = np.w
+00023220: 6865 7265 286d 6f64 656c 5f72 6174 6573  here(model_rates
+00023230: 203e 2031 452d 3629 5b30 5d0a 0a20 2020   > 1E-6)[0]..   
+00023240: 2020 2020 2061 782e 706c 6f74 280a 2020       ax.plot(.  
+00023250: 2020 2020 2020 2020 2020 312e 202f 206e            1. / n
+00023260: 702e 6172 7261 7928 785f 7661 7273 5f67  p.array(x_vars_g
+00023270: 7269 6429 5b76 616c 6964 5f69 6e74 5d2c  rid)[valid_int],
+00023280: 0a20 2020 2020 2020 2020 2020 206e 702e  .            np.
+00023290: 6c6f 6728 312e 202f 206e 702e 6172 7261  log(1. / np.arra
+000232a0: 7928 6d6f 6465 6c5f 7261 7465 7329 5b76  y(model_rates)[v
+000232b0: 616c 6964 5f69 6e74 5d29 2c0a 2020 2020  alid_int]),.    
+000232c0: 2020 2020 2020 2020 6c77 3d31 2e35 2c0a          lw=1.5,.
+000232d0: 2020 2020 2020 2020 2020 2020 6c61 6265              labe
+000232e0: 6c3d 6c6f 676d 6f64 656c 2e4e 414d 452c  l=logmodel.NAME,
+000232f0: 0a20 2020 2020 2020 2020 2020 206c 733d  .            ls=
+00023300: 272d 2d27 0a20 2020 2020 2020 2029 0a0a  '--'.        )..
+00023310: 2020 2020 6966 2074 7970 6528 6d6f 6465      if type(mode
+00023320: 6c29 2069 6e20 5b4d 756c 7469 4c6f 6754  l) in [MultiLogT
+00023330: 6175 544d 6f64 656c 2c20 4d75 6c74 694c  auTModel, MultiL
+00023340: 6f67 5461 7548 4d6f 6465 6c5d 2061 6e64  ogTauHModel] and
+00023350: 206c 656e 286c 6f67 6d6f 6465 6c73 2920   len(logmodels) 
+00023360: 3e20 313a 2023 206e 6f71 610a 2020 2020  > 1: # noqa.    
+00023370: 2020 2020 746f 7461 6c20 3d20 6e70 2e7a      total = np.z
+00023380: 6572 6f73 286c 656e 2878 5f76 6172 735f  eros(len(x_vars_
+00023390: 6772 6964 2929 0a0a 2020 2020 2020 2020  grid))..        
+000233a0: 666f 7220 6c6f 676d 6f64 656c 2069 6e20  for logmodel in 
+000233b0: 6c6f 676d 6f64 656c 733a 0a20 2020 2020  logmodels:.     
+000233c0: 2020 2020 2020 2074 6f74 616c 202b 3d20         total += 
+000233d0: 3130 2a2a 6c6f 676d 6f64 656c 2e6d 6f64  10**logmodel.mod
+000233e0: 656c 280a 2020 2020 2020 2020 2020 2020  el(.            
+000233f0: 2020 2020 6c6f 676d 6f64 656c 2e66 696e      logmodel.fin
+00023400: 616c 5f76 6172 5f76 616c 7565 732c 0a20  al_var_values,. 
+00023410: 2020 2020 2020 2020 2020 2020 2020 2078                 x
+00023420: 5f76 6172 735f 6772 6964 2c0a 2020 2020  _vars_grid,.    
+00023430: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+00023440: 2020 2061 782e 706c 6f74 280a 2020 2020     ax.plot(.    
+00023450: 2020 2020 2020 2020 312e 202f 2078 5f76          1. / x_v
+00023460: 6172 735f 6772 6964 2c0a 2020 2020 2020  ars_grid,.      
+00023470: 2020 2020 2020 6e70 2e6c 6f67 2831 2e20        np.log(1. 
+00023480: 2f20 746f 7461 6c29 2c0a 2020 2020 2020  / total),.      
+00023490: 2020 2020 2020 6c77 3d31 2e35 2c0a 2020        lw=1.5,.  
+000234a0: 2020 2020 2020 2020 2020 6c61 6265 6c3d            label=
+000234b0: 2754 6f74 616c 272c 0a20 2020 2020 2020  'Total',.       
+000234c0: 2020 2020 2063 6f6c 6f72 3d27 7265 6427       color='red'
+000234d0: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+000234e0: 2320 456e 6162 6c65 206d 696e 6f72 2074  # Enable minor t
+000234f0: 6963 6b73 0a20 2020 2061 782e 7961 7869  icks.    ax.yaxi
+00023500: 732e 7365 745f 6d69 6e6f 725f 6c6f 6361  s.set_minor_loca
+00023510: 746f 7228 4175 746f 4d69 6e6f 724c 6f63  tor(AutoMinorLoc
+00023520: 6174 6f72 2829 290a 2020 2020 6178 2e78  ator()).    ax.x
+00023530: 6178 6973 2e73 6574 5f6d 696e 6f72 5f6c  axis.set_minor_l
+00023540: 6f63 6174 6f72 2841 7574 6f4d 696e 6f72  ocator(AutoMinor
+00023550: 4c6f 6361 746f 7228 2929 0a0a 2020 2020  Locator())..    
+00023560: 6578 7072 6573 7369 6f6e 203d 2027 270a  expression = ''.
+00023570: 0a20 2020 2066 6f72 206c 6f67 6d6f 6465  .    for logmode
+00023580: 6c20 696e 206c 6f67 6d6f 6465 6c73 3a0a  l in logmodels:.
+00023590: 2020 2020 2020 2020 666f 7220 6974 2c20          for it, 
+000235a0: 6e61 6d65 2069 6e20 656e 756d 6572 6174  name in enumerat
+000235b0: 6528 6c6f 676d 6f64 656c 2e50 4152 4e41  e(logmodel.PARNA
+000235c0: 4d45 5329 3a0a 2020 2020 2020 2020 2020  MES):.          
+000235d0: 2020 6578 7072 6573 7369 6f6e 202b 3d20    expression += 
+000235e0: 277b 7d20 3d20 7b3a 2e33 667d 2027 2e66  '{} = {:.3f} '.f
+000235f0: 6f72 6d61 7428 0a20 2020 2020 2020 2020  ormat(.         
+00023600: 2020 2020 2020 206c 6f67 6d6f 6465 6c2e         logmodel.
+00023610: 5641 524e 414d 4553 5f4d 4d5b 6e61 6d65  VARNAMES_MM[name
+00023620: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+00023630: 2020 206c 6f67 6d6f 6465 6c2e 6669 6e61     logmodel.fina
+00023640: 6c5f 7661 725f 7661 6c75 6573 5b6e 616d  l_var_values[nam
+00023650: 655d 2c0a 2020 2020 2020 2020 2020 2020  e],.            
+00023660: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+00023670: 206e 616d 6520 696e 206c 6f67 6d6f 6465   name in logmode
+00023680: 6c2e 6669 745f 7661 7273 2e6b 6579 7328  l.fit_vars.keys(
+00023690: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+000236a0: 2020 2065 7870 7265 7373 696f 6e20 2b3d     expression +=
+000236b0: 2072 2724 5c70 6d24 2027 0a20 2020 2020   r'$\pm$ '.     
+000236c0: 2020 2020 2020 2020 2020 2065 7870 7265             expre
+000236d0: 7373 696f 6e20 2b3d 2027 7b3a 2e33 667d  ssion += '{:.3f}
+000236e0: 2027 2e66 6f72 6d61 7428 6c6f 676d 6f64   '.format(logmod
+000236f0: 656c 2e66 6974 5f73 7464 6576 5b6e 616d  el.fit_stdev[nam
+00023700: 655d 290a 2020 2020 2020 2020 2020 2020  e]).            
+00023710: 6578 7072 6573 7369 6f6e 202b 3d20 277b  expression += '{
+00023720: 7d20 2020 2027 2e66 6f72 6d61 7428 6c6f  }    '.format(lo
+00023730: 676d 6f64 656c 2e55 4e49 5453 5f4d 4d5b  gmodel.UNITS_MM[
+00023740: 6e61 6d65 5d29 0a20 2020 2020 2020 2020  name]).         
+00023750: 2020 2069 6620 6974 203d 3d20 3120 616e     if it == 1 an
+00023760: 6420 6c65 6e28 6c6f 676d 6f64 656c 2e66  d len(logmodel.f
+00023770: 6974 5f76 6172 732e 6b65 7973 2829 2920  it_vars.keys()) 
+00023780: 3e20 323a 0a20 2020 2020 2020 2020 2020  > 2:.           
+00023790: 2020 2020 2065 7870 7265 7373 696f 6e20       expression 
+000237a0: 2b3d 2027 5c6e 270a 2020 2020 2020 2020  += '\n'.        
+000237b0: 6578 7072 6573 7369 6f6e 202b 3d20 275c  expression += '\
+000237c0: 6e27 0a0a 2020 2020 6178 2e74 6578 7428  n'..    ax.text(
+000237d0: 0a20 2020 2020 2020 2030 2e30 2c20 312e  .        0.0, 1.
+000237e0: 3032 2c20 733d 6578 7072 6573 7369 6f6e  02, s=expression
+000237f0: 2c20 666f 6e74 7369 7a65 3d31 302c 2074  , fontsize=10, t
+00023800: 7261 6e73 666f 726d 3d61 782e 7472 616e  ransform=ax.tran
+00023810: 7341 7865 730a 2020 2020 290a 0a20 2020  sAxes.    )..   
+00023820: 2061 782e 6c65 6765 6e64 280a 2020 2020   ax.legend(.    
+00023830: 2020 2020 6c6f 633d 276c 6f77 6572 2072      loc='lower r
+00023840: 6967 6874 272c 2066 6f6e 7473 697a 653d  ight', fontsize=
+00023850: 2731 3027 2c20 6e75 6d70 6f69 6e74 733d  '10', numpoints=
+00023860: 312c 206e 636f 6c3d 312c 2066 7261 6d65  1, ncol=1, frame
+00023870: 6f6e 3d46 616c 7365 0a20 2020 2029 0a20  on=False.    ). 
+00023880: 2020 2061 782e 7365 745f 796c 6162 656c     ax.set_ylabel
+00023890: 2872 2724 5c6c 6e5c 6c65 6674 5b5c 7461  (r'$\ln\left[\ta
+000238a0: 755c 7269 6768 745d 2420 245c 6c65 6674  u\right]$ $\left
+000238b0: 285c 6c6e 5c6c 6566 745b 5c6d 6174 6872  (\ln\left[\mathr
+000238c0: 6567 756c 6172 7b73 7d5e 5c6d 6174 6872  egular{s}^\mathr
+000238d0: 6567 756c 6172 7b2d 317d 5c72 6967 6874  egular{-1}\right
+000238e0: 5d5c 7269 6768 7429 2427 2920 2320 6e6f  ]\right)$') # no
+000238f0: 7161 0a0a 2020 2020 7265 7475 726e 0a0a  qa..    return..
+00023900: 0a64 6566 2070 6c6f 745f 6669 7474 6564  .def plot_fitted
+00023910: 5f72 6174 6573 2864 6174 6173 6574 3a20  _rates(dataset: 
+00023920: 5461 7554 4461 7461 7365 7420 7c20 5461  TauTDataset | Ta
+00023930: 7548 4461 7461 7365 742c 0a20 2020 2020  uHDataset,.     
+00023940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023950: 206d 6f64 656c 3a20 4c6f 6754 6175 544d   model: LogTauTM
+00023960: 6f64 656c 207c 204d 756c 7469 4c6f 6754  odel | MultiLogT
+00023970: 6175 544d 6f64 656c 207c 204c 6f67 5461  auTModel | LogTa
+00023980: 7548 4d6f 6465 6c20 7c20 4d75 6c74 694c  uHModel | MultiL
+00023990: 6f67 5461 7548 4d6f 6465 6c2c 2023 206e  ogTauHModel, # n
+000239a0: 6f71 610a 2020 2020 2020 2020 2020 2020  oqa.            
+000239b0: 2020 2020 2020 2020 2020 7368 6f77 3a20            show: 
+000239c0: 626f 6f6c 203d 2054 7275 652c 2073 6176  bool = True, sav
+000239d0: 653a 2062 6f6f 6c20 3d20 4661 6c73 652c  e: bool = False,
+000239e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000239f0: 2020 2020 2020 2073 6176 655f 6e61 6d65         save_name
+00023a00: 3a20 7374 7220 3d20 2766 6974 7465 645f  : str = 'fitted_
+00023a10: 7261 7465 732e 706e 6727 2c0a 2020 2020  rates.png',.    
+00023a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023a30: 2020 7665 7262 6f73 653a 2062 6f6f 6c20    verbose: bool 
+00023a40: 3d20 5472 7565 2920 2d3e 2074 7570 6c65  = True) -> tuple
+00023a50: 5b70 6c74 2e46 6967 7572 652c 2070 6c74  [plt.Figure, plt
+00023a60: 2e41 7865 735d 3a0a 2020 2020 2727 270a  .Axes]:.    '''.
+00023a70: 2020 2020 506c 6f74 7320 6578 7065 7269      Plots experi
+00023a80: 6d65 6e74 616c 2061 6e64 2066 6974 7465  mental and fitte
+00023a90: 6420 286d 6f64 656c 2920 7265 6c61 7861  d (model) relaxa
+00023aa0: 7469 6f6e 2072 6174 6520 6173 5c6e 0a20  tion rate as\n. 
+00023ab0: 2020 2072 6174 6520 7673 2078 7661 7220     rate vs xvar 
+00023ac0: 7768 6572 6520 7876 6172 2069 7320 5420  where xvar is T 
+00023ad0: 6f72 2048 2e20 5769 7468 206c 6f67 206c  or H. With log l
+00023ae0: 6f67 2073 6361 6c65 2e0a 0a20 2020 2050  og scale...    P
+00023af0: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
+00023b00: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2064 6174  --------.    dat
+00023b10: 6173 6574 3a20 5461 7554 4461 7461 7365  aset: TauTDatase
+00023b20: 7420 7c20 5461 7548 4461 7461 7365 740a  t | TauHDataset.
+00023b30: 2020 2020 2020 2020 4461 7461 7365 7420          Dataset 
+00023b40: 746f 2070 6c6f 740a 2020 2020 6d6f 6465  to plot.    mode
+00023b50: 6c3a 204c 6f67 5461 7554 4d6f 6465 6c20  l: LogTauTModel 
+00023b60: 7c20 4d75 6c74 694c 6f67 5461 7554 4d6f  | MultiLogTauTMo
+00023b70: 6465 6c20 7c20 4c6f 6754 6175 484d 6f64  del | LogTauHMod
+00023b80: 656c 207c 204d 756c 7469 4c6f 6754 6175  el | MultiLogTau
+00023b90: 484d 6f64 656c 0a20 2020 2020 2020 204d  HModel.        M
+00023ba0: 6f64 656c 2028 6669 7474 6564 2920 746f  odel (fitted) to
+00023bb0: 2070 6c6f 740a 2020 2020 7368 6f77 3a20   plot.    show: 
+00023bc0: 626f 6f6c 2c20 6465 6661 756c 7420 5472  bool, default Tr
+00023bd0: 7565 0a20 2020 2020 2020 2049 6620 5472  ue.        If Tr
+00023be0: 7565 2c20 7368 6f77 2070 6c6f 7420 6f6e  ue, show plot on
+00023bf0: 2073 6372 6565 6e0a 2020 2020 7361 7665   screen.    save
+00023c00: 3a20 626f 6f6c 2c20 6465 6661 756c 7420  : bool, default 
+00023c10: 4661 6c73 650a 2020 2020 2020 2020 4966  False.        If
+00023c20: 2054 7275 652c 2073 6176 6520 706c 6f74   True, save plot
+00023c30: 2074 6f20 6669 6c65 2060 7361 7665 5f6e   to file `save_n
+00023c40: 616d 6560 0a20 2020 2073 6176 655f 6e61  ame`.    save_na
+00023c50: 6d65 3a20 7374 722c 2064 6566 6175 6c74  me: str, default
+00023c60: 203d 2027 6669 7474 6564 5f72 6174 6573   = 'fitted_rates
+00023c70: 2e70 6e67 270a 2020 2020 2020 2020 4966  .png'.        If
+00023c80: 2073 6176 6520 6973 2054 7275 652c 2077   save is True, w
+00023c90: 696c 6c20 7361 7665 2070 6c6f 7420 746f  ill save plot to
+00023ca0: 2074 6869 7320 6669 6c65 6e61 6d65 0a20   this filename. 
+00023cb0: 2020 2076 6572 626f 7365 3a20 626f 6f6c     verbose: bool
+00023cc0: 2c20 6465 6661 756c 7420 5472 7565 0a20  , default True. 
+00023cd0: 2020 2020 2020 2049 6620 5472 7565 2c20         If True, 
+00023ce0: 706c 6f74 2066 696c 6520 6c6f 6361 7469  plot file locati
+00023cf0: 6f6e 2069 7320 7772 6974 7465 6e20 746f  on is written to
+00023d00: 2074 6572 6d69 6e61 6c0a 2020 2020 5265   terminal.    Re
+00023d10: 7475 726e 730a 2020 2020 2d2d 2d2d 2d2d  turns.    ------
+00023d20: 2d0a 2020 2020 706c 742e 4669 6775 7265  -.    plt.Figure
+00023d30: 0a20 2020 2020 2020 204d 6174 706c 6f74  .        Matplot
+00023d40: 6c69 6220 6669 6775 7265 206f 626a 6563  lib figure objec
+00023d50: 740a 2020 2020 706c 742e 4178 6573 0a20  t.    plt.Axes. 
+00023d60: 2020 2020 2020 204d 6174 706c 6f74 6c69         Matplotli
+00023d70: 6220 6178 6973 206f 626a 6563 740a 2020  b axis object.  
+00023d80: 2020 2727 270a 0a20 2020 2023 2043 7265    '''..    # Cre
+00023d90: 6174 6520 6669 6775 7265 2061 6e64 2061  ate figure and a
+00023da0: 7865 730a 2020 2020 6669 672c 2061 7820  xes.    fig, ax 
+00023db0: 3d20 706c 742e 7375 6270 6c6f 7473 280a  = plt.subplots(.
+00023dc0: 2020 2020 2020 2020 312c 0a20 2020 2020          1,.     
+00023dd0: 2020 2031 2c0a 2020 2020 2020 2020 7368     1,.        sh
+00023de0: 6172 6578 3d54 7275 652c 0a20 2020 2020  arex=True,.     
+00023df0: 2020 2073 6861 7265 793d 5472 7565 2c0a     sharey=True,.
+00023e00: 2020 2020 2020 2020 6669 6773 697a 653d          figsize=
+00023e10: 2836 2c20 3629 2c0a 2020 2020 2020 2020  (6, 6),.        
+00023e20: 6e75 6d3d 2746 6974 7465 6420 7265 6c61  num='Fitted rela
+00023e30: 7861 7469 6f6e 2070 726f 6669 6c65 270a  xation profile'.
+00023e40: 2020 2020 290a 0a20 2020 205f 706c 6f74      )..    _plot
+00023e50: 5f66 6974 7465 645f 7261 7465 7328 6461  _fitted_rates(da
+00023e60: 7461 7365 742c 206d 6f64 656c 2c20 6669  taset, model, fi
+00023e70: 672c 2061 7829 0a0a 2020 2020 6669 672e  g, ax)..    fig.
+00023e80: 7469 6768 745f 6c61 796f 7574 2829 0a0a  tight_layout()..
+00023e90: 2020 2020 6966 2073 686f 773a 0a20 2020      if show:.   
+00023ea0: 2020 2020 2070 6c74 2e73 686f 7728 290a       plt.show().
+00023eb0: 0a20 2020 2069 6620 7361 7665 3a0a 2020  .    if save:.  
+00023ec0: 2020 2020 2020 6669 672e 7361 7665 6669        fig.savefi
+00023ed0: 6728 7361 7665 5f6e 616d 652c 2064 7069  g(save_name, dpi
+00023ee0: 3d35 3030 290a 2020 2020 2020 2020 6966  =500).        if
+00023ef0: 2076 6572 626f 7365 3a0a 2020 2020 2020   verbose:.      
+00023f00: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
+00023f10: 6e63 6528 6461 7461 7365 742c 2028 5461  nce(dataset, (Ta
+00023f20: 7554 4461 7461 7365 7429 293a 0a20 2020  uTDataset)):.   
+00023f30: 2020 2020 2020 2020 2020 2020 205f 7876               _xv
+00023f40: 6172 203d 2027 5427 0a20 2020 2020 2020  ar = 'T'.       
+00023f50: 2020 2020 2065 6c69 6620 6973 696e 7374       elif isinst
+00023f60: 616e 6365 2864 6174 6173 6574 2c20 2854  ance(dataset, (T
+00023f70: 6175 4844 6174 6173 6574 2929 3a0a 2020  auHDataset)):.  
+00023f80: 2020 2020 2020 2020 2020 2020 2020 5f78                _x
+00023f90: 7661 7220 3d20 2748 270a 2020 2020 2020  var = 'H'.      
+00023fa0: 2020 2020 2020 7574 2e63 7072 696e 7428        ut.cprint(
+00023fb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00023fc0: 2066 275c 6e20 4669 7474 6564 20cf 84e2   f'\n Fitted ...
+00023fd0: 81bb c2b9 2076 7320 7b5f 7876 6172 7d20  .... vs {_xvar} 
+00023fe0: 706c 6f74 2073 6176 6564 2074 6f20 5c6e  plot saved to \n
+00023ff0: 207b 7361 7665 5f6e 616d 657d 5c6e 272c   {save_name}\n',
+00024000: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00024010: 2027 6379 616e 270a 2020 2020 2020 2020   'cyan'.        
+00024020: 2020 2020 290a 0a20 2020 2072 6574 7572      )..    retur
+00024030: 6e20 6669 672c 2061 780a 0a0a 6465 6620  n fig, ax...def 
+00024040: 7174 5f70 6c6f 745f 6669 7474 6564 5f72  qt_plot_fitted_r
+00024050: 6174 6573 2861 7070 3a20 5174 5769 6467  ates(app: QtWidg
+00024060: 6574 732e 5141 7070 6c69 6361 7469 6f6e  ets.QApplication
+00024070: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00024080: 2020 2020 2020 2020 2020 2064 6174 6173             datas
+00024090: 6574 3a20 5461 7554 4461 7461 7365 7420  et: TauTDataset 
+000240a0: 7c20 5461 7548 4461 7461 7365 742c 0a20  | TauHDataset,. 
+000240b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000240c0: 2020 2020 2020 2020 6d6f 6465 6c3a 204c          model: L
+000240d0: 6f67 5461 7554 4d6f 6465 6c20 7c20 4d75  ogTauTModel | Mu
+000240e0: 6c74 694c 6f67 5461 7554 4d6f 6465 6c20  ltiLogTauTModel 
+000240f0: 7c20 4c6f 6754 6175 484d 6f64 656c 207c  | LogTauHModel |
+00024100: 204d 756c 7469 4c6f 6754 6175 484d 6f64   MultiLogTauHMod
+00024110: 656c 2c20 2320 6e6f 7161 0a20 2020 2020  el, # noqa.     
+00024120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024130: 2020 2020 7361 7665 3a20 626f 6f6c 203d      save: bool =
+00024140: 2046 616c 7365 2c20 7368 6f77 3a20 626f   False, show: bo
+00024150: 6f6c 203d 2054 7275 652c 0a20 2020 2020  ol = True,.     
+00024160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024170: 2020 2020 7361 7665 5f6e 616d 653a 2073      save_name: s
+00024180: 7472 203d 2027 6669 7474 6564 5f72 6174  tr = 'fitted_rat
+00024190: 6573 2e70 6e67 272c 0a20 2020 2020 2020  es.png',.       
+000241a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000241b0: 2020 7665 7262 6f73 653a 2062 6f6f 6c20    verbose: bool 
+000241c0: 3d20 5472 7565 2920 2d3e 204e 6f6e 653a  = True) -> None:
+000241d0: 0a20 2020 2027 2727 0a20 2020 2050 6c6f  .    '''.    Plo
+000241e0: 7473 2065 7870 6572 696d 656e 7461 6c20  ts experimental 
+000241f0: 616e 6420 6669 7474 6564 2028 6d6f 6465  and fitted (mode
+00024200: 6c29 2072 656c 6178 6174 696f 6e20 7261  l) relaxation ra
+00024210: 7465 2061 735c 6e0a 2020 2020 7261 7465  te as\n.    rate
+00024220: 2076 7320 7876 6172 2077 6865 7265 2078   vs xvar where x
+00024230: 7661 7220 6973 2054 206f 7220 482e 2057  var is T or H. W
+00024240: 6974 6820 6c6f 6720 6c6f 6720 7363 616c  ith log log scal
+00024250: 652e 0a0a 2020 2020 5061 7261 6d65 7465  e...    Paramete
+00024260: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
+00024270: 2d0a 2020 2020 6461 7461 7365 743a 2054  -.    dataset: T
+00024280: 6175 5444 6174 6173 6574 207c 2054 6175  auTDataset | Tau
+00024290: 4844 6174 6173 6574 0a20 2020 2020 2020  HDataset.       
+000242a0: 2044 6174 6173 6574 2074 6f20 706c 6f74   Dataset to plot
+000242b0: 0a20 2020 206d 6f64 656c 3a20 4c6f 6754  .    model: LogT
+000242c0: 6175 544d 6f64 656c 207c 204d 756c 7469  auTModel | Multi
+000242d0: 4c6f 6754 6175 544d 6f64 656c 207c 204c  LogTauTModel | L
+000242e0: 6f67 5461 7548 4d6f 6465 6c20 7c20 4d75  ogTauHModel | Mu
+000242f0: 6c74 694c 6f67 5461 7548 4d6f 6465 6c0a  ltiLogTauHModel.
+00024300: 2020 2020 2020 2020 4d6f 6465 6c20 2866          Model (f
+00024310: 6974 7465 6429 2074 6f20 706c 6f74 0a20  itted) to plot. 
+00024320: 2020 2073 686f 773a 2062 6f6f 6c2c 2064     show: bool, d
+00024330: 6566 6175 6c74 2054 7275 650a 2020 2020  efault True.    
+00024340: 2020 2020 4966 2054 7275 652c 2073 686f      If True, sho
+00024350: 7720 706c 6f74 206f 6e20 7363 7265 656e  w plot on screen
+00024360: 0a20 2020 2073 6176 653a 2062 6f6f 6c2c  .    save: bool,
+00024370: 2064 6566 6175 6c74 2046 616c 7365 0a20   default False. 
+00024380: 2020 2020 2020 2049 6620 5472 7565 2c20         If True, 
+00024390: 7361 7665 2070 6c6f 7420 746f 2066 696c  save plot to fil
+000243a0: 6520 6073 6176 655f 6e61 6d65 600a 2020  e `save_name`.  
+000243b0: 2020 7361 7665 5f6e 616d 653a 2073 7472    save_name: str
+000243c0: 2c20 6465 6661 756c 7420 2766 6974 7465  , default 'fitte
+000243d0: 645f 7261 7465 732e 706e 6727 0a20 2020  d_rates.png'.   
+000243e0: 2020 2020 2049 6620 7361 7665 2069 7320       If save is 
+000243f0: 5472 7565 2c20 7769 6c6c 2073 6176 6520  True, will save 
+00024400: 706c 6f74 2074 6f20 7468 6973 2066 696c  plot to this fil
+00024410: 656e 616d 650a 2020 2020 7665 7262 6f73  ename.    verbos
+00024420: 653a 2062 6f6f 6c2c 2064 6566 6175 6c74  e: bool, default
+00024430: 2054 7275 650a 2020 2020 2020 2020 4966   True.        If
+00024440: 2054 7275 652c 2070 6c6f 7420 6669 6c65   True, plot file
+00024450: 206c 6f63 6174 696f 6e20 6973 2077 7269   location is wri
+00024460: 7474 656e 2074 6f20 7465 726d 696e 616c  tten to terminal
+00024470: 0a0a 2020 2020 5265 7475 726e 730a 2020  ..    Returns.  
+00024480: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 4e6f    -------.    No
+00024490: 6e65 0a20 2020 2027 2727 0a0a 2020 2020  ne.    '''..    
+000244a0: 7769 6e64 6f77 203d 2067 7569 2e4d 6174  window = gui.Mat
+000244b0: 706c 6f74 6c69 6257 696e 646f 7728 290a  plotlibWindow().
+000244c0: 0a20 2020 2077 696e 646f 772e 7365 7457  .    window.setW
+000244d0: 696e 646f 7754 6974 6c65 2827 4669 7474  indowTitle('Fitt
+000244e0: 6564 2072 656c 6178 6174 696f 6e20 7072  ed relaxation pr
+000244f0: 6f66 696c 6527 290a 0a20 2020 2023 2041  ofile')..    # A
+00024500: 6464 2070 6c6f 740a 2020 2020 5f70 6c6f  dd plot.    _plo
+00024510: 745f 6669 7474 6564 5f72 6174 6573 2864  t_fitted_rates(d
+00024520: 6174 6173 6574 2c20 6d6f 6465 6c2c 2077  ataset, model, w
+00024530: 696e 646f 772e 7363 2e66 6967 2c20 7769  indow.sc.fig, wi
+00024540: 6e64 6f77 2e73 632e 6178 290a 0a20 2020  ndow.sc.ax)..   
+00024550: 2023 2053 6176 6520 706c 6f74 0a20 2020   # Save plot.   
+00024560: 2069 6620 7361 7665 3a0a 2020 2020 2020   if save:.      
+00024570: 2020 7769 6e64 6f77 2e73 632e 6669 672e    window.sc.fig.
+00024580: 7361 7665 6669 6728 7361 7665 5f6e 616d  savefig(save_nam
+00024590: 652c 2064 7069 3d33 3030 290a 2020 2020  e, dpi=300).    
+000245a0: 2020 2020 6966 2076 6572 626f 7365 3a0a      if verbose:.
+000245b0: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+000245c0: 7369 6e73 7461 6e63 6528 6461 7461 7365  sinstance(datase
+000245d0: 742c 2028 5461 7554 4461 7461 7365 7429  t, (TauTDataset)
+000245e0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+000245f0: 2020 205f 7876 6172 203d 2027 5427 0a20     _xvar = 'T'. 
+00024600: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+00024610: 6973 696e 7374 616e 6365 2864 6174 6173  isinstance(datas
+00024620: 6574 2c20 2854 6175 4844 6174 6173 6574  et, (TauHDataset
+00024630: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
+00024640: 2020 2020 5f78 7661 7220 3d20 2748 270a      _xvar = 'H'.
+00024650: 2020 2020 2020 2020 2020 2020 7574 2e63              ut.c
+00024660: 7072 696e 7428 0a20 2020 2020 2020 2020  print(.         
+00024670: 2020 2020 2020 2066 275c 6e20 4669 7474         f'\n Fitt
+00024680: 6564 20cf 84e2 81bb c2b9 2076 7320 7b5f  ed ....... vs {_
+00024690: 7876 6172 7d20 706c 6f74 2073 6176 6564  xvar} plot saved
+000246a0: 2074 6f20 5c6e 207b 7361 7665 5f6e 616d   to \n {save_nam
+000246b0: 657d 5c6e 272c 0a20 2020 2020 2020 2020  e}\n',.         
+000246c0: 2020 2020 2020 2027 6379 616e 270a 2020         'cyan'.  
+000246d0: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+000246e0: 2069 6620 7368 6f77 3a0a 2020 2020 2020   if show:.      
+000246f0: 2020 7769 6e64 6f77 2e73 686f 7728 290a    window.show().
+00024700: 2020 2020 2020 2020 2320 4361 6c6c 2074          # Call t
+00024710: 7769 6365 2065 6c73 6520 6974 2077 6f6e  wice else it won
+00024720: 7420 776f 726b 210a 2020 2020 2020 2020  t work!.        
+00024730: 7769 6e64 6f77 2e73 632e 6669 672e 7469  window.sc.fig.ti
+00024740: 6768 745f 6c61 796f 7574 2829 0a20 2020  ght_layout().   
+00024750: 2020 2020 2077 696e 646f 772e 7363 2e66       window.sc.f
+00024760: 6967 2e74 6967 6874 5f6c 6179 6f75 7428  ig.tight_layout(
+00024770: 290a 2020 2020 2020 2020 6170 702e 6578  ).        app.ex
+00024780: 6563 5f28 290a 0a20 2020 2072 6574 7572  ec_()..    retur
+00024790: 6e0a 0a0a 6465 6620 5f70 6c6f 745f 6669  n...def _plot_fi
+000247a0: 7474 6564 5f72 6174 6573 2864 6174 6173  tted_rates(datas
+000247b0: 6574 3a20 5461 7554 4461 7461 7365 7420  et: TauTDataset 
+000247c0: 7c20 5461 7548 4461 7461 7365 742c 0a20  | TauHDataset,. 
+000247d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000247e0: 2020 2020 2020 6d6f 6465 6c3a 204c 6f67        model: Log
+000247f0: 5461 7554 4d6f 6465 6c20 7c20 4d75 6c74  TauTModel | Mult
+00024800: 694c 6f67 5461 7554 4d6f 6465 6c20 7c20  iLogTauTModel | 
+00024810: 4c6f 6754 6175 484d 6f64 656c 207c 204d  LogTauHModel | M
+00024820: 756c 7469 4c6f 6754 6175 484d 6f64 656c  ultiLogTauHModel
+00024830: 2c20 2320 6e6f 7161 0a20 2020 2020 2020  , # noqa.       
+00024840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024850: 6669 673a 2070 6c74 2e46 6967 7572 652c  fig: plt.Figure,
+00024860: 2061 783a 2070 6c74 2e41 7865 7329 3a0a   ax: plt.Axes):.
+00024870: 2020 2020 2727 270a 2020 2020 506c 6f74      '''.    Plot
+00024880: 7320 6578 7065 7269 6d65 6e74 616c 2061  s experimental a
+00024890: 6e64 2066 6974 7465 6420 286d 6f64 656c  nd fitted (model
+000248a0: 2920 7265 6c61 7861 7469 6f6e 2072 6174  ) relaxation rat
+000248b0: 6520 6173 5c6e 0a20 2020 2072 6174 6520  e as\n.    rate 
+000248c0: 7673 2078 7661 7220 7768 6572 6520 7876  vs xvar where xv
+000248d0: 6172 2069 7320 5420 6f72 2048 2e20 5769  ar is T or H. Wi
+000248e0: 7468 206c 6f67 206c 6f67 2073 6361 6c65  th log log scale
+000248f0: 2e0a 0a20 2020 2050 6172 616d 6574 6572  ...    Parameter
+00024900: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  s.    ----------
+00024910: 0a20 2020 2064 6174 6173 6574 3a20 5461  .    dataset: Ta
+00024920: 7554 4461 7461 7365 7420 7c20 5461 7548  uTDataset | TauH
+00024930: 4461 7461 7365 740a 2020 2020 2020 2020  Dataset.        
+00024940: 4461 7461 7365 7420 746f 2070 6c6f 740a  Dataset to plot.
+00024950: 2020 2020 6d6f 6465 6c3a 204c 6f67 5461      model: LogTa
+00024960: 7554 4d6f 6465 6c20 7c20 4d75 6c74 694c  uTModel | MultiL
+00024970: 6f67 5461 7554 4d6f 6465 6c20 7c20 4c6f  ogTauTModel | Lo
+00024980: 6754 6175 484d 6f64 656c 207c 204d 756c  gTauHModel | Mul
+00024990: 7469 4c6f 6754 6175 484d 6f64 656c 0a20  tiLogTauHModel. 
+000249a0: 2020 2020 2020 204d 6f64 656c 2028 6669         Model (fi
+000249b0: 7474 6564 2920 746f 2070 6c6f 740a 2020  tted) to plot.  
+000249c0: 2020 6669 673a 2070 6c74 2e46 6967 7572    fig: plt.Figur
+000249d0: 650a 2020 2020 2020 2020 4d61 7470 6c6f  e.        Matplo
+000249e0: 746c 6962 2046 6967 7572 6520 6f62 6a65  tlib Figure obje
+000249f0: 6374 2075 7365 6420 666f 7220 706c 6f74  ct used for plot
+00024a00: 0a20 2020 2061 783a 2070 6c74 2e41 7865  .    ax: plt.Axe
+00024a10: 730a 2020 2020 2020 2020 4d61 7470 6c6f  s.        Matplo
+00024a20: 746c 6962 2041 7869 7320 6f62 6a65 6374  tlib Axis object
+00024a30: 2075 7365 6420 666f 7220 706c 6f74 0a0a   used for plot..
+00024a40: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
+00024a50: 2d2d 2d2d 2d2d 2d0a 2020 2020 4e6f 6e65  -------.    None
+00024a60: 0a20 2020 2027 2727 0a0a 2020 2020 6966  .    '''..    if
+00024a70: 2069 7369 6e73 7461 6e63 6528 6461 7461   isinstance(data
+00024a80: 7365 742c 2054 6175 4844 6174 6173 6574  set, TauHDataset
+00024a90: 293a 0a20 2020 2020 2020 2078 5f76 6172  ):.        x_var
+00024aa0: 7320 3d20 6461 7461 7365 742e 6669 656c  s = dataset.fiel
+00024ab0: 6473 0a20 2020 2020 2020 2061 782e 7365  ds.        ax.se
+00024ac0: 745f 786c 6162 656c 2872 2746 6965 6c64  t_xlabel(r'Field
+00024ad0: 2028 4f65 2927 290a 2020 2020 656c 6966   (Oe)').    elif
+00024ae0: 2069 7369 6e73 7461 6e63 6528 6461 7461   isinstance(data
+00024af0: 7365 742c 2054 6175 5444 6174 6173 6574  set, TauTDataset
+00024b00: 293a 0a20 2020 2020 2020 2078 5f76 6172  ):.        x_var
+00024b10: 7320 3d20 6461 7461 7365 742e 7465 6d70  s = dataset.temp
+00024b20: 6572 6174 7572 6573 0a20 2020 2020 2020  eratures.       
+00024b30: 2061 782e 7365 745f 786c 6162 656c 2872   ax.set_xlabel(r
+00024b40: 2754 656d 7065 7261 7475 7265 2028 4b29  'Temperature (K)
+00024b50: 2729 0a0a 2020 2020 2320 4164 6420 756e  ')..    # Add un
+00024b60: 6365 7274 6169 6e74 6965 7320 6173 2065  certainties as e
+00024b70: 7272 6f72 6261 7273 0a20 2020 2069 6620  rrorbars.    if 
+00024b80: 6c65 6e28 6461 7461 7365 742e 7261 7465  len(dataset.rate
+00024b90: 5f70 6d29 3a0a 2020 2020 2020 2020 6178  _pm):.        ax
+00024ba0: 2e65 7272 6f72 6261 7228 0a20 2020 2020  .errorbar(.     
+00024bb0: 2020 2020 2020 2078 5f76 6172 732c 0a20         x_vars,. 
+00024bc0: 2020 2020 2020 2020 2020 2064 6174 6173             datas
+00024bd0: 6574 2e72 6174 6573 2c0a 2020 2020 2020  et.rates,.      
+00024be0: 2020 2020 2020 7965 7272 3d64 6174 6173        yerr=datas
+00024bf0: 6574 2e72 6174 655f 706d 2c0a 2020 2020  et.rate_pm,.    
+00024c00: 2020 2020 2020 2020 6d61 726b 6572 3d27          marker='
+00024c10: 6f27 2c0a 2020 2020 2020 2020 2020 2020  o',.            
+00024c20: 6c77 3d30 2c0a 2020 2020 2020 2020 2020  lw=0,.          
+00024c30: 2020 656c 696e 6577 6964 7468 3d31 2e35    elinewidth=1.5
+00024c40: 2c0a 2020 2020 2020 2020 2020 2020 6669  ,.            fi
+00024c50: 6c6c 7374 796c 653d 276e 6f6e 6527 2c0a  llstyle='none',.
+00024c60: 2020 2020 2020 2020 2020 2020 6c61 6265              labe
+00024c70: 6c3d 2745 7870 6572 696d 656e 7427 2c0a  l='Experiment',.
+00024c80: 2020 2020 2020 2020 2020 2020 636f 6c6f              colo
+00024c90: 723d 2762 6c61 636b 270a 2020 2020 2020  r='black'.      
+00024ca0: 2020 290a 2020 2020 656c 7365 3a0a 2020    ).    else:.  
+00024cb0: 2020 2020 2020 6178 2e70 6c6f 7428 0a20        ax.plot(. 
+00024cc0: 2020 2020 2020 2020 2020 2078 5f76 6172             x_var
+00024cd0: 732c 0a20 2020 2020 2020 2020 2020 2064  s,.            d
+00024ce0: 6174 6173 6574 2e72 6174 6573 2c0a 2020  ataset.rates,.  
+00024cf0: 2020 2020 2020 2020 2020 6d61 726b 6572            marker
+00024d00: 3d27 6f27 2c0a 2020 2020 2020 2020 2020  ='o',.          
+00024d10: 2020 6c77 3d30 2c0a 2020 2020 2020 2020    lw=0,.        
+00024d20: 2020 2020 6669 6c6c 7374 796c 653d 276e      fillstyle='n
+00024d30: 6f6e 6527 2c0a 2020 2020 2020 2020 2020  one',.          
+00024d40: 2020 6c61 6265 6c3d 2745 7870 6572 696d    label='Experim
+00024d50: 656e 7427 2c0a 2020 2020 2020 2020 2020  ent',.          
+00024d60: 2020 636f 6c6f 723d 2762 6c61 636b 270a    color='black'.
+00024d70: 2020 2020 2020 2020 290a 0a20 2020 2078          )..    x
+00024d80: 5f76 6172 735f 6772 6964 203d 206e 702e  _vars_grid = np.
+00024d90: 6c6f 6773 7061 6365 280a 2020 2020 2020  logspace(.      
+00024da0: 2020 6e70 2e6c 6f67 3130 286e 702e 6d69    np.log10(np.mi
+00024db0: 6e28 785f 7661 7273 2929 2c0a 2020 2020  n(x_vars)),.    
+00024dc0: 2020 2020 6e70 2e6c 6f67 3130 286e 702e      np.log10(np.
+00024dd0: 6d61 7828 785f 7661 7273 2929 2c0a 2020  max(x_vars)),.  
+00024de0: 2020 2020 2020 3530 300a 2020 2020 290a        500.    ).
+00024df0: 0a20 2020 2069 6620 7479 7065 286d 6f64  .    if type(mod
+00024e00: 656c 2920 696e 205b 4d75 6c74 694c 6f67  el) in [MultiLog
+00024e10: 5461 7554 4d6f 6465 6c2c 204d 756c 7469  TauTModel, Multi
+00024e20: 4c6f 6754 6175 484d 6f64 656c 5d3a 0a20  LogTauHModel]:. 
+00024e30: 2020 2020 2020 206c 6f67 6d6f 6465 6c73         logmodels
+00024e40: 203d 206d 6f64 656c 2e6c 6f67 6d6f 6465   = model.logmode
+00024e50: 6c73 0a20 2020 2065 6c73 653a 0a20 2020  ls.    else:.   
+00024e60: 2020 2020 206c 6f67 6d6f 6465 6c73 203d       logmodels =
+00024e70: 205b 6d6f 6465 6c5d 0a0a 2020 2020 666f   [model]..    fo
+00024e80: 7220 6c6f 676d 6f64 656c 2069 6e20 6c6f  r logmodel in lo
+00024e90: 676d 6f64 656c 733a 0a0a 2020 2020 2020  gmodels:..      
+00024ea0: 2020 6966 2074 7970 6528 6c6f 676d 6f64    if type(logmod
+00024eb0: 656c 2920 6973 204c 6f67 4f72 6261 6368  el) is LogOrbach
+00024ec0: 4d6f 6465 6c3a 0a20 2020 2020 2020 2020  Model:.         
+00024ed0: 2020 206c 6162 656c 5f66 6974 203d 2027     label_fit = '
+00024ee0: 5c6e 4669 7420 7769 7468 270a 2020 2020  \nFit with'.    
+00024ef0: 2020 2020 2020 2020 6c61 6265 6c5f 6669          label_fi
+00024f00: 7420 2b3d 2027 5c6e 2720 2b20 7227 7b7d  t += '\n' + r'{}
+00024f10: 207b 3a36 2e32 667d 2073 272e 666f 726d   {:6.2f} s'.form
+00024f20: 6174 280a 2020 2020 2020 2020 2020 2020  at(.            
+00024f30: 2020 2020 6c6f 676d 6f64 656c 2e56 4152      logmodel.VAR
+00024f40: 4e41 4d45 535f 4d4d 5b27 755f 6566 6627  NAMES_MM['u_eff'
+00024f50: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+00024f60: 2020 206c 6f67 6d6f 6465 6c2e 6669 6e61     logmodel.fina
+00024f70: 6c5f 7661 725f 7661 6c75 6573 5b27 755f  l_var_values['u_
+00024f80: 6566 6627 5d0a 2020 2020 2020 2020 2020  eff'].          
+00024f90: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00024fa0: 6c61 6265 6c5f 6669 7420 2b3d 2027 5c6e  label_fit += '\n
+00024fb0: 2720 2b20 7227 7b7d 207b 3a30 342e 3365  ' + r'{} {:04.3e
+00024fc0: 7d27 2e66 6f72 6d61 7428 0a20 2020 2020  }'.format(.     
+00024fd0: 2020 2020 2020 2020 2020 206c 6f67 6d6f             logmo
+00024fe0: 6465 6c2e 5641 524e 414d 4553 5f4d 4d5b  del.VARNAMES_MM[
+00024ff0: 2741 275d 2c20 6c6f 676d 6f64 656c 2e66  'A'], logmodel.f
+00025000: 696e 616c 5f76 6172 5f76 616c 7565 735b  inal_var_values[
+00025010: 2741 275d 0a20 2020 2020 2020 2020 2020  'A'].           
+00025020: 2029 0a20 2020 2020 2020 2065 6c69 6620   ).        elif 
+00025030: 7479 7065 286c 6f67 6d6f 6465 6c29 2069  type(logmodel) i
+00025040: 7320 4c6f 6752 616d 616e 4d6f 6465 6c3a  s LogRamanModel:
+00025050: 0a20 2020 2020 2020 2020 2020 206c 6162  .            lab
+00025060: 656c 5f66 6974 203d 2027 5c6e 4669 7420  el_fit = '\nFit 
+00025070: 7769 7468 270a 2020 2020 2020 2020 2020  with'.          
+00025080: 2020 6c61 6265 6c5f 6669 7420 2b3d 2027    label_fit += '
+00025090: 5c6e 2720 2b20 7227 7b7d 207b 3a36 2e32  \n' + r'{} {:6.2
+000250a0: 667d 2073 272e 666f 726d 6174 280a 2020  f} s'.format(.  
+000250b0: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+000250c0: 676d 6f64 656c 2e56 4152 4e41 4d45 535f  gmodel.VARNAMES_
+000250d0: 4d4d 5b27 5227 5d2c 206c 6f67 6d6f 6465  MM['R'], logmode
+000250e0: 6c2e 6669 6e61 6c5f 7661 725f 7661 6c75  l.final_var_valu
+000250f0: 6573 5b27 5227 5d0a 2020 2020 2020 2020  es['R'].        
+00025100: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00025110: 2020 6c61 6265 6c5f 6669 7420 2b3d 2027    label_fit += '
+00025120: 5c6e 2720 2b20 7227 7b7d 207b 3a30 342e  \n' + r'{} {:04.
+00025130: 3365 7d27 2e66 6f72 6d61 7428 0a20 2020  3e}'.format(.   
+00025140: 2020 2020 2020 2020 2020 2020 206c 6f67               log
+00025150: 6d6f 6465 6c2e 5641 524e 414d 4553 5f4d  model.VARNAMES_M
+00025160: 4d5b 276e 275d 2c20 6c6f 676d 6f64 656c  M['n'], logmodel
+00025170: 2e66 696e 616c 5f76 6172 5f76 616c 7565  .final_var_value
+00025180: 735b 276e 275d 0a20 2020 2020 2020 2020  s['n'].         
+00025190: 2020 2029 0a20 2020 2020 2020 2065 6c69     ).        eli
+000251a0: 6620 7479 7065 286c 6f67 6d6f 6465 6c29  f type(logmodel)
+000251b0: 2069 7320 4c6f 6751 544d 4d6f 6465 6c3a   is LogQTMModel:
+000251c0: 0a20 2020 2020 2020 2020 2020 206c 6162  .            lab
+000251d0: 656c 5f66 6974 203d 2027 5c6e 4669 7420  el_fit = '\nFit 
+000251e0: 7769 7468 270a 2020 2020 2020 2020 2020  with'.          
+000251f0: 2020 6c61 6265 6c5f 6669 7420 2b3d 2027    label_fit += '
+00025200: 5c6e 2720 2b20 7227 7b7d 207b 3a36 2e32  \n' + r'{} {:6.2
+00025210: 667d 2073 272e 666f 726d 6174 280a 2020  f} s'.format(.  
+00025220: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+00025230: 676d 6f64 656c 2e56 4152 4e41 4d45 535f  gmodel.VARNAMES_
+00025240: 4d4d 5b27 5127 5d2c 206c 6f67 6d6f 6465  MM['Q'], logmode
+00025250: 6c2e 6669 6e61 6c5f 7661 725f 7661 6c75  l.final_var_valu
+00025260: 6573 5b27 5127 5d0a 2020 2020 2020 2020  es['Q'].        
+00025270: 2020 2020 290a 2020 2020 2020 2020 656c      ).        el
+00025280: 6966 2074 7970 6528 6c6f 676d 6f64 656c  if type(logmodel
+00025290: 2920 6973 204c 6f67 4469 7265 6374 4d6f  ) is LogDirectMo
+000252a0: 6465 6c3a 0a20 2020 2020 2020 2020 2020  del:.           
+000252b0: 206c 6162 656c 5f66 6974 203d 2027 5c6e   label_fit = '\n
+000252c0: 4669 7420 7769 7468 270a 2020 2020 2020  Fit with'.      
+000252d0: 2020 2020 2020 6c61 6265 6c5f 6669 7420        label_fit 
+000252e0: 2b3d 2027 5c6e 2720 2b20 7227 7b7d 207b  += '\n' + r'{} {
+000252f0: 3a36 2e32 667d 2073 272e 666f 726d 6174  :6.2f} s'.format
+00025300: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00025310: 2020 6c6f 676d 6f64 656c 2e56 4152 4e41    logmodel.VARNA
+00025320: 4d45 535f 4d4d 5b27 4427 5d2c 206c 6f67  MES_MM['D'], log
+00025330: 6d6f 6465 6c2e 6669 6e61 6c5f 7661 725f  model.final_var_
+00025340: 7661 6c75 6573 5b27 4427 5d0a 2020 2020  values['D'].    
+00025350: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00025360: 2020 6d6f 6465 6c5f 7261 7465 7320 3d20    model_rates = 
+00025370: 3130 2a2a 6c6f 676d 6f64 656c 2e6d 6f64  10**logmodel.mod
+00025380: 656c 280a 2020 2020 2020 2020 2020 2020  el(.            
+00025390: 6c6f 676d 6f64 656c 2e66 696e 616c 5f76  logmodel.final_v
+000253a0: 6172 5f76 616c 7565 732c 0a20 2020 2020  ar_values,.     
+000253b0: 2020 2020 2020 2078 5f76 6172 735f 6772         x_vars_gr
+000253c0: 6964 2c0a 2020 2020 2020 2020 290a 0a20  id,.        ).. 
+000253d0: 2020 2020 2020 2023 2054 7269 6d20 6d6f         # Trim mo
+000253e0: 6465 6c20 7261 7465 7320 746f 2073 656e  del rates to sen
+000253f0: 7369 626c 6520 7661 6c75 6573 0a20 2020  sible values.   
+00025400: 2020 2020 2076 616c 6964 5f69 6e74 203d       valid_int =
+00025410: 206e 702e 7768 6572 6528 6d6f 6465 6c5f   np.where(model_
+00025420: 7261 7465 7320 3e20 3145 2d36 295b 305d  rates > 1E-6)[0]
+00025430: 0a0a 2020 2020 2020 2020 6178 2e70 6c6f  ..        ax.plo
+00025440: 7428 0a20 2020 2020 2020 2020 2020 206e  t(.            n
+00025450: 702e 6172 7261 7928 785f 7661 7273 5f67  p.array(x_vars_g
+00025460: 7269 6429 5b76 616c 6964 5f69 6e74 5d2c  rid)[valid_int],
+00025470: 0a20 2020 2020 2020 2020 2020 206e 702e  .            np.
+00025480: 6172 7261 7928 6d6f 6465 6c5f 7261 7465  array(model_rate
+00025490: 7329 5b76 616c 6964 5f69 6e74 5d2c 0a20  s)[valid_int],. 
+000254a0: 2020 2020 2020 2020 2020 206c 773d 312e             lw=1.
+000254b0: 352c 0a20 2020 2020 2020 2020 2020 206c  5,.            l
+000254c0: 6162 656c 3d6c 6f67 6d6f 6465 6c2e 4e41  abel=logmodel.NA
+000254d0: 4d45 2c0a 2020 2020 2020 2020 2020 2020  ME,.            
+000254e0: 6c73 3d27 2d2d 270a 2020 2020 2020 2020  ls='--'.        
+000254f0: 290a 0a20 2020 2069 6620 7479 7065 286d  )..    if type(m
+00025500: 6f64 656c 2920 696e 205b 4d75 6c74 694c  odel) in [MultiL
+00025510: 6f67 5461 7554 4d6f 6465 6c2c 204d 756c  ogTauTModel, Mul
+00025520: 7469 4c6f 6754 6175 484d 6f64 656c 5d20  tiLogTauHModel] 
+00025530: 616e 6420 6c65 6e28 6c6f 676d 6f64 656c  and len(logmodel
+00025540: 7329 203e 2031 3a20 2320 6e6f 7161 0a20  s) > 1: # noqa. 
+00025550: 2020 2020 2020 2074 6f74 616c 203d 206e         total = n
+00025560: 702e 7a65 726f 7328 6c65 6e28 785f 7661  p.zeros(len(x_va
+00025570: 7273 5f67 7269 6429 290a 0a20 2020 2020  rs_grid))..     
+00025580: 2020 2066 6f72 206c 6f67 6d6f 6465 6c20     for logmodel 
+00025590: 696e 206c 6f67 6d6f 6465 6c73 3a0a 2020  in logmodels:.  
+000255a0: 2020 2020 2020 2020 2020 746f 7461 6c20            total 
+000255b0: 2b3d 2031 302a 2a6c 6f67 6d6f 6465 6c2e  += 10**logmodel.
+000255c0: 6d6f 6465 6c28 0a20 2020 2020 2020 2020  model(.         
+000255d0: 2020 2020 2020 206c 6f67 6d6f 6465 6c2e         logmodel.
+000255e0: 6669 6e61 6c5f 7661 725f 7661 6c75 6573  final_var_values
+000255f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00025600: 2020 785f 7661 7273 5f67 7269 642c 0a20    x_vars_grid,. 
+00025610: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+00025620: 2020 2020 2020 6178 2e70 6c6f 7428 0a20        ax.plot(. 
+00025630: 2020 2020 2020 2020 2020 2078 5f76 6172             x_var
+00025640: 735f 6772 6964 2c0a 2020 2020 2020 2020  s_grid,.        
+00025650: 2020 2020 746f 7461 6c2c 0a20 2020 2020      total,.     
+00025660: 2020 2020 2020 206c 773d 312e 352c 0a20         lw=1.5,. 
+00025670: 2020 2020 2020 2020 2020 206c 6162 656c             label
+00025680: 3d27 546f 7461 6c27 2c0a 2020 2020 2020  ='Total',.      
+00025690: 2020 2020 2020 636f 6c6f 723d 2772 6564        color='red
+000256a0: 270a 2020 2020 2020 2020 290a 0a20 2020  '.        )..   
+000256b0: 2061 782e 7365 745f 7873 6361 6c65 2827   ax.set_xscale('
+000256c0: 6c6f 6727 290a 2020 2020 6178 2e73 6574  log').    ax.set
+000256d0: 5f79 7363 616c 6528 276c 6f67 2729 0a0a  _yscale('log')..
+000256e0: 2020 2020 6775 692e 666f 726d 6174 5f72      gui.format_r
+000256f0: 6174 655f 785f 795f 6178 6573 280a 2020  ate_x_y_axes(.  
+00025700: 2020 2020 2020 6178 2c0a 2020 2020 2020        ax,.      
+00025710: 2020 6461 7461 7365 742e 7261 7465 732c    dataset.rates,
+00025720: 0a20 2020 2020 2020 2078 5f76 6172 735f  .        x_vars_
+00025730: 6772 6964 2c0a 2020 2020 2020 2020 6e70  grid,.        np
+00025740: 2e61 6273 2864 6174 6173 6574 2e72 6174  .abs(dataset.rat
+00025750: 655f 706d 290a 2020 2020 290a 0a20 2020  e_pm).    )..   
+00025760: 2065 7870 7265 7373 696f 6e20 3d20 2727   expression = ''
+00025770: 0a0a 2020 2020 666f 7220 6c6f 676d 6f64  ..    for logmod
+00025780: 656c 2069 6e20 6c6f 676d 6f64 656c 733a  el in logmodels:
+00025790: 0a20 2020 2020 2020 2066 6f72 2069 742c  .        for it,
+000257a0: 206e 616d 6520 696e 2065 6e75 6d65 7261   name in enumera
+000257b0: 7465 286c 6f67 6d6f 6465 6c2e 5041 524e  te(logmodel.PARN
+000257c0: 414d 4553 293a 0a20 2020 2020 2020 2020  AMES):.         
+000257d0: 2020 2065 7870 7265 7373 696f 6e20 2b3d     expression +=
+000257e0: 2027 7b7d 203d 207b 3a2e 3366 7d20 272e   '{} = {:.3f} '.
+000257f0: 666f 726d 6174 280a 2020 2020 2020 2020  format(.        
+00025800: 2020 2020 2020 2020 6c6f 676d 6f64 656c          logmodel
+00025810: 2e56 4152 4e41 4d45 535f 4d4d 5b6e 616d  .VARNAMES_MM[nam
+00025820: 655d 2c0a 2020 2020 2020 2020 2020 2020  e],.            
+00025830: 2020 2020 6c6f 676d 6f64 656c 2e66 696e      logmodel.fin
+00025840: 616c 5f76 6172 5f76 616c 7565 735b 6e61  al_var_values[na
+00025850: 6d65 5d2c 0a20 2020 2020 2020 2020 2020  me],.           
+00025860: 2029 0a20 2020 2020 2020 2020 2020 2069   ).            i
+00025870: 6620 6e61 6d65 2069 6e20 6c6f 676d 6f64  f name in logmod
+00025880: 656c 2e66 6974 5f76 6172 732e 6b65 7973  el.fit_vars.keys
+00025890: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+000258a0: 2020 2020 6578 7072 6573 7369 6f6e 202b      expression +
+000258b0: 3d20 7227 245c 706d 2420 270a 2020 2020  = r'$\pm$ '.    
+000258c0: 2020 2020 2020 2020 2020 2020 6578 7072              expr
+000258d0: 6573 7369 6f6e 202b 3d20 277b 3a2e 3366  ession += '{:.3f
+000258e0: 7d20 272e 666f 726d 6174 286c 6f67 6d6f  } '.format(logmo
+000258f0: 6465 6c2e 6669 745f 7374 6465 765b 6e61  del.fit_stdev[na
+00025900: 6d65 5d29 0a20 2020 2020 2020 2020 2020  me]).           
+00025910: 2065 7870 7265 7373 696f 6e20 2b3d 2027   expression += '
+00025920: 7b7d 2020 2020 272e 666f 726d 6174 286c  {}    '.format(l
+00025930: 6f67 6d6f 6465 6c2e 554e 4954 535f 4d4d  ogmodel.UNITS_MM
+00025940: 5b6e 616d 655d 290a 2020 2020 2020 2020  [name]).        
+00025950: 2020 2020 6966 2069 7420 3d3d 2031 2061      if it == 1 a
+00025960: 6e64 206c 656e 286c 6f67 6d6f 6465 6c2e  nd len(logmodel.
+00025970: 6669 745f 7661 7273 2e6b 6579 7328 2929  fit_vars.keys())
+00025980: 203e 2032 3a0a 2020 2020 2020 2020 2020   > 2:.          
+00025990: 2020 2020 2020 6578 7072 6573 7369 6f6e        expression
+000259a0: 202b 3d20 275c 6e27 0a20 2020 2020 2020   += '\n'.       
+000259b0: 2065 7870 7265 7373 696f 6e20 2b3d 2027   expression += '
+000259c0: 5c6e 270a 0a20 2020 2061 782e 7465 7874  \n'..    ax.text
+000259d0: 280a 2020 2020 2020 2020 302e 302c 2031  (.        0.0, 1
+000259e0: 2e30 322c 2073 3d65 7870 7265 7373 696f  .02, s=expressio
+000259f0: 6e2c 2066 6f6e 7473 697a 653d 3130 2c20  n, fontsize=10, 
+00025a00: 7472 616e 7366 6f72 6d3d 6178 2e74 7261  transform=ax.tra
+00025a10: 6e73 4178 6573 0a20 2020 2029 0a0a 2020  nsAxes.    )..  
+00025a20: 2020 6178 2e6c 6567 656e 6428 0a20 2020    ax.legend(.   
+00025a30: 2020 2020 206c 6f63 3d27 7570 7065 7220       loc='upper 
+00025a40: 6c65 6674 272c 2066 6f6e 7473 697a 653d  left', fontsize=
+00025a50: 2731 3027 2c20 6e75 6d70 6f69 6e74 733d  '10', numpoints=
+00025a60: 312c 206e 636f 6c3d 312c 2066 7261 6d65  1, ncol=1, frame
+00025a70: 6f6e 3d46 616c 7365 0a20 2020 2029 0a20  on=False.    ). 
+00025a80: 2020 2061 782e 7365 745f 796c 6162 656c     ax.set_ylabel
+00025a90: 2872 2752 6174 6520 2873 245e 5c6d 6174  (r'Rate (s$^\mat
+00025aa0: 6872 6567 756c 6172 7b2d 317d 2429 2729  hregular{-1}$)')
+00025ab0: 0a0a 2020 2020 7265 7475 726e 0a0a 0a64  ..    return...d
+00025ac0: 6566 2070 6c6f 745f 7261 7465 7328 6461  ef plot_rates(da
+00025ad0: 7461 7365 743a 2054 6175 5444 6174 6173  taset: TauTDatas
+00025ae0: 6574 207c 2054 6175 4844 6174 6173 6574  et | TauHDataset
+00025af0: 2c20 7368 6f77 3a20 626f 6f6c 203d 2054  , show: bool = T
+00025b00: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
+00025b10: 2020 2020 7361 7665 3a20 626f 6f6c 203d      save: bool =
+00025b20: 2046 616c 7365 2c20 7361 7665 5f6e 616d   False, save_nam
+00025b30: 653a 2073 7472 203d 2027 7265 6c61 7861  e: str = 'relaxa
+00025b40: 7469 6f6e 5f72 6174 6573 2e70 6e67 272c  tion_rates.png',
+00025b50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00025b60: 7665 7262 6f73 653a 2062 6f6f 6c20 3d20  verbose: bool = 
+00025b70: 5472 7565 2920 2d3e 2074 7570 6c65 5b70  True) -> tuple[p
+00025b80: 6c74 2e46 6967 7572 652c 2070 6c74 2e41  lt.Figure, plt.A
+00025b90: 7865 735d 3a0a 2020 2020 2727 270a 2020  xes]:.    '''.  
+00025ba0: 2020 506c 6f74 7320 6578 7065 7269 6d65    Plots experime
+00025bb0: 6e74 616c 2072 656c 6178 6174 696f 6e20  ntal relaxation 
+00025bc0: 7261 7465 2076 7320 6669 656c 642f 7465  rate vs field/te
+00025bd0: 6d70 6572 6174 7572 6520 616e 640a 2020  mperature and.  
+00025be0: 2020 6469 7370 6c61 7973 206f 6e20 7363    displays on sc
+00025bf0: 7265 656e 2e0a 0a20 2020 2050 6172 616d  reen...    Param
+00025c00: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
+00025c10: 2d2d 2d2d 0a20 2020 2064 6174 6173 6574  ----.    dataset
+00025c20: 3a20 5461 7554 4461 7461 7365 7420 7c20  : TauTDataset | 
+00025c30: 5461 7548 4461 7461 7365 740a 2020 2020  TauHDataset.    
+00025c40: 2020 2020 4461 7461 7365 7420 746f 2070      Dataset to p
+00025c50: 6c6f 740a 2020 2020 7368 6f77 3a20 626f  lot.    show: bo
+00025c60: 6f6c 2c20 6465 6661 756c 7420 5472 7565  ol, default True
+00025c70: 0a20 2020 2020 2020 2049 6620 5472 7565  .        If True
+00025c80: 2c20 7368 6f77 2070 6c6f 7420 6f6e 2073  , show plot on s
+00025c90: 6372 6565 6e0a 2020 2020 7361 7665 3a20  creen.    save: 
+00025ca0: 626f 6f6c 2c20 6465 6661 756c 7420 4661  bool, default Fa
+00025cb0: 6c73 650a 2020 2020 2020 2020 4966 2054  lse.        If T
+00025cc0: 7275 652c 2073 6176 6520 706c 6f74 2074  rue, save plot t
+00025cd0: 6f20 6669 6c65 2060 7361 7665 5f6e 616d  o file `save_nam
+00025ce0: 6560 0a20 2020 2073 6176 655f 6e61 6d65  e`.    save_name
+00025cf0: 3a20 7374 722c 2064 6566 6175 6c74 2027  : str, default '
+00025d00: 7265 6c61 7861 7469 6f6e 5f72 6174 6573  relaxation_rates
+00025d10: 2e70 6e67 270a 2020 2020 2020 2020 4966  .png'.        If
+00025d20: 2073 6176 6520 6973 2054 7275 652c 2077   save is True, w
+00025d30: 696c 6c20 7361 7665 2070 6c6f 7420 746f  ill save plot to
+00025d40: 2074 6869 7320 6669 6c65 6e61 6d65 0a20   this filename. 
+00025d50: 2020 2076 6572 626f 7365 3a20 626f 6f6c     verbose: bool
+00025d60: 2c20 6465 6661 756c 7420 5472 7565 0a20  , default True. 
+00025d70: 2020 2020 2020 2049 6620 5472 7565 2c20         If True, 
+00025d80: 706c 6f74 2066 696c 6520 6c6f 6361 7469  plot file locati
+00025d90: 6f6e 2069 7320 7772 6974 7465 6e20 746f  on is written to
+00025da0: 2074 6572 6d69 6e61 6c0a 0a20 2020 2052   terminal..    R
+00025db0: 6574 7572 6e73 0a20 2020 202d 2d2d 2d2d  eturns.    -----
+00025dc0: 2d2d 0a20 2020 2070 6c74 2e46 6967 7572  --.    plt.Figur
+00025dd0: 650a 2020 2020 2020 2020 4d61 7470 6c6f  e.        Matplo
+00025de0: 746c 6962 2066 6967 7572 6520 6f62 6a65  tlib figure obje
+00025df0: 6374 0a20 2020 2070 6c74 2e41 7865 730a  ct.    plt.Axes.
+00025e00: 2020 2020 2020 2020 4d61 7470 6c6f 746c          Matplotl
+00025e10: 6962 2061 7869 7320 6f62 6a65 6374 0a20  ib axis object. 
+00025e20: 2020 2027 2727 0a0a 2020 2020 2320 4372     '''..    # Cr
+00025e30: 6561 7465 2066 6967 7572 6520 616e 6420  eate figure and 
+00025e40: 6178 6573 0a20 2020 2066 6967 2c20 6178  axes.    fig, ax
+00025e50: 203d 2070 6c74 2e73 7562 706c 6f74 7328   = plt.subplots(
+00025e60: 0a20 2020 2020 2020 2031 2c0a 2020 2020  .        1,.    
+00025e70: 2020 2020 312c 0a20 2020 2020 2020 2073      1,.        s
+00025e80: 6861 7265 783d 5472 7565 2c0a 2020 2020  harex=True,.    
+00025e90: 2020 2020 7368 6172 6579 3d54 7275 652c      sharey=True,
+00025ea0: 0a20 2020 2020 2020 2066 6967 7369 7a65  .        figsize
+00025eb0: 3d28 362c 2036 292c 0a20 2020 2020 2020  =(6, 6),.       
+00025ec0: 206e 756d 3d27 4669 7474 6564 2072 656c   num='Fitted rel
+00025ed0: 6178 6174 696f 6e20 7072 6f66 696c 6527  axation profile'
+00025ee0: 0a20 2020 2029 0a0a 2020 2020 6966 2069  .    )..    if i
+00025ef0: 7369 6e73 7461 6e63 6528 6461 7461 7365  sinstance(datase
+00025f00: 742c 2054 6175 4844 6174 6173 6574 293a  t, TauHDataset):
+00025f10: 0a20 2020 2020 2020 2078 5f76 6172 7320  .        x_vars 
+00025f20: 3d20 6461 7461 7365 742e 6669 656c 6473  = dataset.fields
+00025f30: 0a20 2020 2020 2020 2061 782e 7365 745f  .        ax.set_
+00025f40: 786c 6162 656c 2872 2746 6965 6c64 2028  xlabel(r'Field (
+00025f50: 4f65 2927 290a 2020 2020 656c 6966 2069  Oe)').    elif i
+00025f60: 7369 6e73 7461 6e63 6528 6461 7461 7365  sinstance(datase
+00025f70: 742c 2054 6175 5444 6174 6173 6574 293a  t, TauTDataset):
+00025f80: 0a20 2020 2020 2020 2078 5f76 6172 7320  .        x_vars 
+00025f90: 3d20 6461 7461 7365 742e 7465 6d70 6572  = dataset.temper
+00025fa0: 6174 7572 6573 0a20 2020 2020 2020 2061  atures.        a
+00025fb0: 782e 7365 745f 786c 6162 656c 2872 2754  x.set_xlabel(r'T
+00025fc0: 656d 7065 7261 7475 7265 2028 4b29 2729  emperature (K)')
+00025fd0: 0a0a 2020 2020 2320 4164 6420 756e 6365  ..    # Add unce
+00025fe0: 7274 6169 6e74 6965 7320 6173 2065 7272  rtainties as err
+00025ff0: 6f72 6261 7273 0a20 2020 2069 6620 6c65  orbars.    if le
+00026000: 6e28 6461 7461 7365 742e 7261 7465 5f70  n(dataset.rate_p
+00026010: 6d29 3a0a 2020 2020 2020 2020 6178 2e65  m):.        ax.e
+00026020: 7272 6f72 6261 7228 0a20 2020 2020 2020  rrorbar(.       
+00026030: 2020 2020 2078 5f76 6172 732c 0a20 2020       x_vars,.   
+00026040: 2020 2020 2020 2020 2064 6174 6173 6574           dataset
+00026050: 2e72 6174 6573 2c0a 2020 2020 2020 2020  .rates,.        
+00026060: 2020 2020 7965 7272 3d64 6174 6173 6574      yerr=dataset
+00026070: 2e72 6174 655f 706d 2c0a 2020 2020 2020  .rate_pm,.      
+00026080: 2020 2020 2020 6d61 726b 6572 3d27 6f27        marker='o'
+00026090: 2c0a 2020 2020 2020 2020 2020 2020 6c77  ,.            lw
+000260a0: 3d30 2c0a 2020 2020 2020 2020 2020 2020  =0,.            
+000260b0: 656c 696e 6577 6964 7468 3d31 2e35 2c0a  elinewidth=1.5,.
+000260c0: 2020 2020 2020 2020 2020 2020 6669 6c6c              fill
+000260d0: 7374 796c 653d 276e 6f6e 6527 2c0a 2020  style='none',.  
+000260e0: 2020 2020 2020 2020 2020 636f 6c6f 723d            color=
+000260f0: 2762 6c61 636b 270a 2020 2020 2020 2020  'black'.        
+00026100: 290a 2020 2020 656c 7365 3a0a 2020 2020  ).    else:.    
+00026110: 2020 2020 6178 2e70 6c6f 7428 0a20 2020      ax.plot(.   
+00026120: 2020 2020 2020 2020 2078 5f76 6172 732c           x_vars,
+00026130: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+00026140: 6173 6574 2e72 6174 6573 2c0a 2020 2020  aset.rates,.    
+00026150: 2020 2020 2020 2020 6d61 726b 6572 3d27          marker='
+00026160: 6f27 2c0a 2020 2020 2020 2020 2020 2020  o',.            
+00026170: 6c77 3d30 2c0a 2020 2020 2020 2020 2020  lw=0,.          
+00026180: 2020 6669 6c6c 7374 796c 653d 276e 6f6e    fillstyle='non
+00026190: 6527 2c0a 2020 2020 2020 2020 2020 2020  e',.            
+000261a0: 636f 6c6f 723d 2762 6c61 636b 270a 2020  color='black'.  
+000261b0: 2020 2020 2020 290a 0a20 2020 2061 782e        )..    ax.
+000261c0: 7365 745f 7873 6361 6c65 2827 6c6f 6727  set_xscale('log'
+000261d0: 290a 2020 2020 6178 2e73 6574 5f79 7363  ).    ax.set_ysc
+000261e0: 616c 6528 276c 6f67 2729 0a0a 2020 2020  ale('log')..    
+000261f0: 6178 2e73 6574 5f79 6c61 6265 6c28 7227  ax.set_ylabel(r'
+00026200: 5261 7465 2028 7324 5e5c 6d61 7468 7265  Rate (s$^\mathre
+00026210: 6775 6c61 727b 2d31 7d24 2927 290a 0a20  gular{-1}$)').. 
+00026220: 2020 2069 6620 6c65 6e28 6461 7461 7365     if len(datase
+00026230: 742e 6c6f 6772 6174 655f 706d 293a 0a20  t.lograte_pm):. 
+00026240: 2020 2020 2020 2061 6c6c 5f64 6174 6120         all_data 
+00026250: 3d20 5b0a 2020 2020 2020 2020 2020 2020  = [.            
+00026260: 6e70 2e6c 6f67 3130 2864 6174 6173 6574  np.log10(dataset
+00026270: 2e72 6174 6573 2920 2b20 6461 7461 7365  .rates) + datase
+00026280: 742e 6c6f 6772 6174 655f 706d 0a20 2020  t.lograte_pm.   
+00026290: 2020 2020 205d 0a20 2020 2020 2020 2061       ].        a
+000262a0: 6c6c 5f64 6174 6120 2b3d 205b 0a20 2020  ll_data += [.   
+000262b0: 2020 2020 2020 2020 206e 702e 6c6f 6731           np.log1
+000262c0: 3028 6461 7461 7365 742e 7261 7465 7329  0(dataset.rates)
+000262d0: 202d 2064 6174 6173 6574 2e6c 6f67 7261   - dataset.logra
+000262e0: 7465 5f70 6d0a 2020 2020 2020 2020 5d0a  te_pm.        ].
+000262f0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00026300: 2020 616c 6c5f 6461 7461 203d 205b 0a20    all_data = [. 
+00026310: 2020 2020 2020 2020 2020 206e 702e 6c6f             np.lo
+00026320: 6731 3028 6461 7461 7365 742e 7261 7465  g10(dataset.rate
+00026330: 7329 0a20 2020 2020 2020 205d 0a20 2020  s).        ].   
+00026340: 2020 2020 2061 6c6c 5f64 6174 6120 2b3d       all_data +=
+00026350: 205b 0a20 2020 2020 2020 2020 2020 206e   [.            n
+00026360: 702e 6c6f 6731 3028 6461 7461 7365 742e  p.log10(dataset.
+00026370: 7261 7465 7329 0a20 2020 2020 2020 205d  rates).        ]
+00026380: 0a0a 2020 2020 6775 692e 666f 726d 6174  ..    gui.format
+00026390: 5f72 6174 655f 785f 795f 6178 6573 280a  _rate_x_y_axes(.
+000263a0: 2020 2020 2020 2020 6178 2c0a 2020 2020          ax,.    
+000263b0: 2020 2020 6461 7461 7365 742e 7261 7465      dataset.rate
+000263c0: 732c 0a20 2020 2020 2020 2078 5f76 6172  s,.        x_var
+000263d0: 732c 0a20 2020 2020 2020 206e 702e 6162  s,.        np.ab
+000263e0: 7328 6461 7461 7365 742e 7261 7465 5f70  s(dataset.rate_p
+000263f0: 6d29 0a20 2020 2029 0a0a 2020 2020 2320  m).    )..    # 
+00026400: 5365 7420 7820 7469 636b 2066 6f72 6d61  Set x tick forma
+00026410: 7474 696e 670a 2020 2020 6775 692e 7365  tting.    gui.se
+00026420: 745f 7261 7465 5f78 7469 636b 5f66 6f72  t_rate_xtick_for
+00026430: 6d61 7474 696e 6728 6178 2c20 785f 7661  matting(ax, x_va
+00026440: 7273 290a 0a20 2020 2066 6967 2e74 6967  rs)..    fig.tig
+00026450: 6874 5f6c 6179 6f75 7428 290a 0a20 2020  ht_layout()..   
+00026460: 2069 6620 7361 7665 3a0a 2020 2020 2020   if save:.      
+00026470: 2020 706c 742e 7361 7665 6669 6728 7361    plt.savefig(sa
+00026480: 7665 5f6e 616d 6529 0a20 2020 2020 2020  ve_name).       
+00026490: 2069 6620 7665 7262 6f73 653a 0a20 2020   if verbose:.   
+000264a0: 2020 2020 2020 2020 2075 742e 6370 7269           ut.cpri
+000264b0: 6e74 280a 2020 2020 2020 2020 2020 2020  nt(.            
+000264c0: 2020 2020 6627 5c6e 2052 656c 6178 6174      f'\n Relaxat
+000264d0: 696f 6e20 706c 6f74 2073 6176 6564 2074  ion plot saved t
+000264e0: 6f20 5c6e 207b 7361 7665 5f6e 616d 657d  o \n {save_name}
+000264f0: 5c6e 272c 0a20 2020 2020 2020 2020 2020  \n',.           
+00026500: 2020 2020 2027 6379 616e 270a 2020 2020       'cyan'.    
+00026510: 2020 2020 2020 2020 290a 2020 2020 6966          ).    if
+00026520: 2073 686f 773a 0a20 2020 2020 2020 2070   show:.        p
+00026530: 6c74 2e73 686f 7728 290a 0a20 2020 2072  lt.show()..    r
+00026540: 6574 7572 6e20 6669 672c 2061 780a 0a0a  eturn fig, ax...
+00026550: 6465 6620 706c 6f74 5f72 6174 655f 7265  def plot_rate_re
+00026560: 7369 6475 616c 7328 6461 7461 7365 743a  siduals(dataset:
+00026570: 2054 6175 5444 6174 6173 6574 2c0a 2020   TauTDataset,.  
+00026580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026590: 2020 2020 2020 6d6f 6465 6c3a 204c 6f67        model: Log
+000265a0: 5461 7554 4d6f 6465 6c20 7c20 4d75 6c74  TauTModel | Mult
+000265b0: 694c 6f67 5461 7554 4d6f 6465 6c20 7c20  iLogTauTModel | 
+000265c0: 4c6f 6754 6175 484d 6f64 656c 207c 204d  LogTauHModel | M
+000265d0: 756c 7469 4c6f 6754 6175 484d 6f64 656c  ultiLogTauHModel
+000265e0: 2c20 2320 6e6f 7161 0a20 2020 2020 2020  , # noqa.       
+000265f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026600: 2073 6176 653a 2062 6f6f 6c20 3d20 4661   save: bool = Fa
+00026610: 6c73 652c 2073 686f 773a 2062 6f6f 6c20  lse, show: bool 
+00026620: 3d20 5472 7565 2c0a 2020 2020 2020 2020  = True,.        
+00026630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026640: 7361 7665 5f6e 616d 653a 2073 7472 203d  save_name: str =
+00026650: 2027 6d6f 6465 6c5f 7265 7369 6475 616c   'model_residual
+00026660: 5f74 6175 2e70 6e67 272c 0a20 2020 2020  _tau.png',.     
+00026670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026680: 2020 2076 6572 626f 7365 3a20 626f 6f6c     verbose: bool
+00026690: 203d 2054 7275 6529 202d 3e20 7475 706c   = True) -> tupl
+000266a0: 655b 706c 742e 4669 6775 7265 2c20 706c  e[plt.Figure, pl
+000266b0: 742e 4178 6573 5d3a 0a20 2020 2027 2727  t.Axes]:.    '''
+000266c0: 0a20 2020 2050 6c6f 7473 2064 6966 6665  .    Plots diffe
+000266d0: 7265 6e63 6520 6f66 206c 6f67 3130 2865  rence of log10(e
+000266e0: 7870 6572 696d 656e 7429 2061 6e64 206c  xperiment) and l
+000266f0: 6f67 3130 286d 6f64 656c 2920 7265 6c61  og10(model) rela
+00026700: 7861 7469 6f6e 2072 6174 6573 0a20 2020  xation rates.   
+00026710: 2028 6c6f 6731 3028 6578 7065 7269 6d65   (log10(experime
+00026720: 6e74 5f72 6174 6529 202d 206c 6f67 3130  nt_rate) - log10
+00026730: 286d 6f64 656c 5f72 6174 6529 2076 7320  (model_rate) vs 
+00026740: 5465 6d70 6572 6174 7572 6520 6f72 2046  Temperature or F
+00026750: 6965 6c64 290a 0a20 2020 2050 6172 616d  ield)..    Param
+00026760: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
+00026770: 2d2d 2d2d 0a20 2020 2064 6174 6173 6574  ----.    dataset
+00026780: 3a20 5461 7554 4461 7461 7365 7420 7c20  : TauTDataset | 
+00026790: 5461 7548 4461 7461 7365 740a 2020 2020  TauHDataset.    
+000267a0: 2020 2020 4461 7461 7365 7420 746f 2070      Dataset to p
+000267b0: 6c6f 740a 2020 2020 6d6f 6465 6c3a 204c  lot.    model: L
+000267c0: 6f67 5461 7554 4d6f 6465 6c20 7c20 4d75  ogTauTModel | Mu
+000267d0: 6c74 694c 6f67 5461 7554 4d6f 6465 6c20  ltiLogTauTModel 
+000267e0: 7c20 4c6f 6754 6175 484d 6f64 656c 207c  | LogTauHModel |
+000267f0: 204d 756c 7469 4c6f 6754 6175 484d 6f64   MultiLogTauHMod
+00026800: 656c 0a20 2020 2020 2020 204d 6f64 656c  el.        Model
+00026810: 2028 6669 7474 6564 2920 746f 2070 6c6f   (fitted) to plo
+00026820: 740a 2020 2020 7368 6f77 3a20 626f 6f6c  t.    show: bool
+00026830: 2c20 6465 6661 756c 7420 5472 7565 0a20  , default True. 
+00026840: 2020 2020 2020 2049 6620 5472 7565 2c20         If True, 
+00026850: 7368 6f77 2070 6c6f 7420 6f6e 2073 6372  show plot on scr
+00026860: 6565 6e0a 2020 2020 7361 7665 3a20 626f  een.    save: bo
+00026870: 6f6c 2c20 6465 6661 756c 7420 4661 6c73  ol, default Fals
+00026880: 650a 2020 2020 2020 2020 4966 2054 7275  e.        If Tru
+00026890: 652c 2073 6176 6520 706c 6f74 2074 6f20  e, save plot to 
+000268a0: 6669 6c65 2060 7361 7665 5f6e 616d 6560  file `save_name`
+000268b0: 0a20 2020 2073 6176 655f 6e61 6d65 3a20  .    save_name: 
+000268c0: 7374 722c 2064 6566 6175 6c74 2027 6d6f  str, default 'mo
+000268d0: 6465 6c5f 7265 7369 6475 616c 5f74 6175  del_residual_tau
+000268e0: 2e70 6e67 270a 2020 2020 2020 2020 4966  .png'.        If
+000268f0: 2073 6176 6520 6973 2054 7275 652c 2077   save is True, w
+00026900: 696c 6c20 7361 7665 2070 6c6f 7420 746f  ill save plot to
+00026910: 2074 6869 7320 6669 6c65 6e61 6d65 0a20   this filename. 
+00026920: 2020 2076 6572 626f 7365 3a20 626f 6f6c     verbose: bool
+00026930: 2c20 6465 6661 756c 7420 5472 7565 0a20  , default True. 
+00026940: 2020 2020 2020 2049 6620 5472 7565 2c20         If True, 
+00026950: 706c 6f74 2066 696c 6520 6c6f 6361 7469  plot file locati
+00026960: 6f6e 2069 7320 7772 6974 7465 6e20 746f  on is written to
+00026970: 2074 6572 6d69 6e61 6c0a 0a20 2020 2052   terminal..    R
+00026980: 6574 7572 6e73 0a20 2020 202d 2d2d 2d2d  eturns.    -----
+00026990: 2d2d 0a20 2020 2070 6c74 2e46 6967 7572  --.    plt.Figur
+000269a0: 650a 2020 2020 2020 2020 4d61 7470 6c6f  e.        Matplo
+000269b0: 746c 6962 2066 6967 7572 6520 6f62 6a65  tlib figure obje
+000269c0: 6374 0a20 2020 2070 6c74 2e41 7865 730a  ct.    plt.Axes.
+000269d0: 2020 2020 2020 2020 4d61 7470 6c6f 746c          Matplotl
+000269e0: 6962 2061 7869 7320 6f62 6a65 6374 0a20  ib axis object. 
+000269f0: 2020 2027 2727 0a20 2020 2023 2043 7265     '''.    # Cre
+00026a00: 6174 6520 6669 6775 7265 2061 6e64 2061  ate figure and a
+00026a10: 7865 730a 2020 2020 6669 672c 2061 7820  xes.    fig, ax 
+00026a20: 3d20 706c 742e 7375 6270 6c6f 7473 280a  = plt.subplots(.
+00026a30: 2020 2020 2020 2020 312c 0a20 2020 2020          1,.     
+00026a40: 2020 2031 2c0a 2020 2020 2020 2020 6669     1,.        fi
+00026a50: 6773 697a 653d 5b36 2c20 365d 2c0a 2020  gsize=[6, 6],.  
+00026a60: 2020 2020 2020 6e75 6d3d 2752 6573 6964        num='Resid
+00026a70: 7561 6c73 270a 2020 2020 290a 0a20 2020  uals'.    )..   
+00026a80: 205f 706c 6f74 5f72 6174 655f 7265 7369   _plot_rate_resi
+00026a90: 6475 616c 7328 6461 7461 7365 742c 206d  duals(dataset, m
+00026aa0: 6f64 656c 2c20 6178 290a 0a20 2020 2066  odel, ax)..    f
+00026ab0: 6967 2e74 6967 6874 5f6c 6179 6f75 7428  ig.tight_layout(
+00026ac0: 290a 0a20 2020 2023 2053 6176 6520 706c  )..    # Save pl
+00026ad0: 6f74 0a20 2020 2069 6620 7361 7665 3a0a  ot.    if save:.
+00026ae0: 2020 2020 2020 2020 706c 742e 7361 7665          plt.save
+00026af0: 6669 6728 7361 7665 5f6e 616d 652c 2064  fig(save_name, d
+00026b00: 7069 3d33 3030 290a 2020 2020 2020 2020  pi=300).        
+00026b10: 6966 2076 6572 626f 7365 3a0a 2020 2020  if verbose:.    
+00026b20: 2020 2020 2020 2020 7574 2e63 7072 696e          ut.cprin
+00026b30: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
+00026b40: 2020 2066 275c 6e20 5261 7465 2072 6573     f'\n Rate res
+00026b50: 6964 7561 6c73 2070 6c6f 7420 7361 7665  iduals plot save
+00026b60: 6420 746f 205c 6e20 7b73 6176 655f 6e61  d to \n {save_na
+00026b70: 6d65 7d5c 6e27 2c0a 2020 2020 2020 2020  me}\n',.        
+00026b80: 2020 2020 2020 2020 2763 7961 6e27 0a20          'cyan'. 
+00026b90: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00026ba0: 2069 6620 7368 6f77 3a0a 2020 2020 2020   if show:.      
+00026bb0: 2020 706c 742e 7368 6f77 2829 0a0a 2020    plt.show()..  
+00026bc0: 2020 7265 7475 726e 2066 6967 2c20 6178    return fig, ax
+00026bd0: 0a0a 0a64 6566 2071 745f 706c 6f74 5f72  ...def qt_plot_r
+00026be0: 6174 655f 7265 7369 6475 616c 7328 6170  ate_residuals(ap
+00026bf0: 703a 2051 7457 6964 6765 7473 2e51 4170  p: QtWidgets.QAp
+00026c00: 706c 6963 6174 696f 6e2c 2064 6174 6173  plication, datas
+00026c10: 6574 3a20 5461 7554 4461 7461 7365 742c  et: TauTDataset,
+00026c20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00026c30: 2020 2020 2020 2020 2020 2020 6d6f 6465              mode
+00026c40: 6c3a 204c 6f67 5461 7554 4d6f 6465 6c20  l: LogTauTModel 
+00026c50: 7c20 4d75 6c74 694c 6f67 5461 7554 4d6f  | MultiLogTauTMo
+00026c60: 6465 6c20 7c20 4c6f 6754 6175 484d 6f64  del | LogTauHMod
+00026c70: 656c 207c 204d 756c 7469 4c6f 6754 6175  el | MultiLogTau
+00026c80: 484d 6f64 656c 2c20 2320 6e6f 7161 0a20  HModel, # noqa. 
+00026c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026ca0: 2020 2020 2020 2020 2020 7361 7665 3a20            save: 
+00026cb0: 626f 6f6c 203d 2046 616c 7365 2c20 7368  bool = False, sh
+00026cc0: 6f77 3a20 626f 6f6c 203d 2054 7275 652c  ow: bool = True,
+00026cd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00026ce0: 2020 2020 2020 2020 2020 2020 7361 7665              save
+00026cf0: 5f6e 616d 653a 2073 7472 203d 2027 6d6f  _name: str = 'mo
+00026d00: 6465 6c5f 7265 7369 6475 616c 5f74 6175  del_residual_tau
+00026d10: 2e70 6e67 272c 0a20 2020 2020 2020 2020  .png',.         
+00026d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026d30: 2020 7665 7262 6f73 653a 2062 6f6f 6c20    verbose: bool 
+00026d40: 3d20 5472 7565 2920 2d3e 204e 6f6e 653a  = True) -> None:
+00026d50: 0a20 2020 2027 2727 0a20 2020 2050 6c6f  .    '''.    Plo
+00026d60: 7473 2064 6966 6665 7265 6e63 6520 6f66  ts difference of
+00026d70: 206c 6f67 3130 2865 7870 6572 696d 656e   log10(experimen
+00026d80: 7429 2061 6e64 206c 6f67 3130 286d 6f64  t) and log10(mod
+00026d90: 656c 2920 7265 6c61 7861 7469 6f6e 2072  el) relaxation r
+00026da0: 6174 6573 0a20 2020 2069 6e20 6120 7174  ates.    in a qt
+00026db0: 2077 696e 646f 7720 7573 696e 6720 6d61   window using ma
+00026dc0: 7470 6c6f 746c 6962 0a0a 2020 2020 5061  tplotlib..    Pa
+00026dd0: 7261 6d65 7465 7273 0a20 2020 202d 2d2d  rameters.    ---
+00026de0: 2d2d 2d2d 2d2d 2d0a 2020 2020 6170 703a  -------.    app:
+00026df0: 2051 7457 6964 6765 7473 2e51 4170 706c   QtWidgets.QAppl
+00026e00: 6963 6174 696f 6e0a 2020 2020 2020 2020  ication.        
+00026e10: 4170 706c 6963 6174 696f 6e20 7573 6564  Application used
+00026e20: 2062 7920 6375 7272 656e 7420 7072 6f67   by current prog
+00026e30: 7261 6d0a 2020 2020 2020 2020 4372 6561  ram.        Crea
+00026e40: 7465 2077 6974 6820 6061 7070 3d51 7457  te with `app=QtW
+00026e50: 6964 6765 7473 2e51 4170 706c 6963 6174  idgets.QApplicat
+00026e60: 696f 6e28 5b5d 2960 0a20 2020 2064 6174  ion([])`.    dat
+00026e70: 6173 6574 3a20 5461 7554 4461 7461 7365  aset: TauTDatase
+00026e80: 7420 7c20 5461 7548 4461 7461 7365 740a  t | TauHDataset.
+00026e90: 2020 2020 2020 2020 4461 7461 7365 7420          Dataset 
+00026ea0: 746f 2070 6c6f 740a 2020 2020 6d6f 6465  to plot.    mode
+00026eb0: 6c3a 204c 6f67 5461 7554 4d6f 6465 6c20  l: LogTauTModel 
+00026ec0: 7c20 4d75 6c74 694c 6f67 5461 7554 4d6f  | MultiLogTauTMo
+00026ed0: 6465 6c20 7c20 4c6f 6754 6175 484d 6f64  del | LogTauHMod
+00026ee0: 656c 207c 204d 756c 7469 4c6f 6754 6175  el | MultiLogTau
+00026ef0: 484d 6f64 656c 0a20 2020 2020 2020 204d  HModel.        M
+00026f00: 6f64 656c 2028 6669 7474 6564 2920 746f  odel (fitted) to
+00026f10: 2070 6c6f 740a 2020 2020 7368 6f77 3a20   plot.    show: 
+00026f20: 626f 6f6c 2c20 6465 6661 756c 7420 5472  bool, default Tr
+00026f30: 7565 0a20 2020 2020 2020 2049 6620 5472  ue.        If Tr
+00026f40: 7565 2c20 7368 6f77 2070 6c6f 7420 6f6e  ue, show plot on
+00026f50: 2073 6372 6565 6e0a 2020 2020 7361 7665   screen.    save
+00026f60: 3a20 626f 6f6c 2c20 6465 6661 756c 7420  : bool, default 
+00026f70: 4661 6c73 650a 2020 2020 2020 2020 4966  False.        If
+00026f80: 2054 7275 652c 2073 6176 6520 706c 6f74   True, save plot
+00026f90: 2074 6f20 6669 6c65 2060 7361 7665 5f6e   to file `save_n
+00026fa0: 616d 6560 0a20 2020 2073 6176 655f 6e61  ame`.    save_na
+00026fb0: 6d65 3a20 7374 722c 2064 6566 6175 6c74  me: str, default
+00026fc0: 2027 6d6f 6465 6c5f 7265 7369 6475 616c   'model_residual
+00026fd0: 5f74 6175 2e70 6e67 270a 2020 2020 2020  _tau.png'.      
+00026fe0: 2020 4966 2073 6176 6520 6973 2054 7275    If save is Tru
+00026ff0: 652c 2077 696c 6c20 7361 7665 2070 6c6f  e, will save plo
+00027000: 7420 746f 2074 6869 7320 6669 6c65 6e61  t to this filena
+00027010: 6d65 0a20 2020 2076 6572 626f 7365 3a20  me.    verbose: 
+00027020: 626f 6f6c 2c20 6465 6661 756c 7420 5472  bool, default Tr
+00027030: 7565 0a20 2020 2020 2020 2049 6620 5472  ue.        If Tr
+00027040: 7565 2c20 706c 6f74 2066 696c 6520 6c6f  ue, plot file lo
+00027050: 6361 7469 6f6e 2069 7320 7772 6974 7465  cation is writte
+00027060: 6e20 746f 2074 6572 6d69 6e61 6c0a 0a20  n to terminal.. 
+00027070: 2020 2052 6574 7572 6e73 0a20 2020 202d     Returns.    -
+00027080: 2d2d 2d2d 2d2d 0a20 2020 204e 6f6e 650a  ------.    None.
+00027090: 2020 2020 2727 270a 0a20 2020 2077 696e      '''..    win
+000270a0: 646f 7720 3d20 6775 692e 4d61 7470 6c6f  dow = gui.Matplo
+000270b0: 746c 6962 5769 6e64 6f77 2829 0a20 2020  tlibWindow().   
+000270c0: 2077 696e 646f 772e 7365 7457 696e 646f   window.setWindo
+000270d0: 7754 6974 6c65 2827 5265 7369 6475 616c  wTitle('Residual
+000270e0: 7327 290a 0a20 2020 205f 706c 6f74 5f72  s')..    _plot_r
+000270f0: 6174 655f 7265 7369 6475 616c 7328 6461  ate_residuals(da
+00027100: 7461 7365 742c 206d 6f64 656c 2c20 7769  taset, model, wi
+00027110: 6e64 6f77 2e73 632e 6178 290a 0a20 2020  ndow.sc.ax)..   
+00027120: 2023 2053 6176 6520 706c 6f74 0a20 2020   # Save plot.   
+00027130: 2069 6620 7361 7665 3a0a 2020 2020 2020   if save:.      
+00027140: 2020 7769 6e64 6f77 2e73 632e 6669 672e    window.sc.fig.
+00027150: 7361 7665 6669 6728 7361 7665 5f6e 616d  savefig(save_nam
+00027160: 652c 2064 7069 3d33 3030 290a 2020 2020  e, dpi=300).    
+00027170: 2020 2020 6966 2076 6572 626f 7365 3a0a      if verbose:.
+00027180: 2020 2020 2020 2020 2020 2020 7574 2e63              ut.c
+00027190: 7072 696e 7428 0a20 2020 2020 2020 2020  print(.         
+000271a0: 2020 2020 2020 2066 275c 6e20 5261 7465         f'\n Rate
+000271b0: 2072 6573 6964 7561 6c73 2070 6c6f 7420   residuals plot 
+000271c0: 7361 7665 6420 746f 205c 6e20 7b73 6176  saved to \n {sav
+000271d0: 655f 6e61 6d65 7d5c 6e27 2c0a 2020 2020  e_name}\n',.    
+000271e0: 2020 2020 2020 2020 2020 2020 2763 7961              'cya
+000271f0: 6e27 0a20 2020 2020 2020 2020 2020 2029  n'.            )
+00027200: 0a0a 2020 2020 6966 2073 686f 773a 0a20  ..    if show:. 
+00027210: 2020 2020 2020 2077 696e 646f 772e 7368         window.sh
+00027220: 6f77 2829 0a20 2020 2020 2020 2023 2043  ow().        # C
+00027230: 616c 6c20 7477 6963 6520 656c 7365 2069  all twice else i
+00027240: 7420 776f 6e74 2077 6f72 6b21 0a20 2020  t wont work!.   
+00027250: 2020 2020 2077 696e 646f 772e 7363 2e66       window.sc.f
+00027260: 6967 2e74 6967 6874 5f6c 6179 6f75 7428  ig.tight_layout(
+00027270: 290a 2020 2020 2020 2020 7769 6e64 6f77  ).        window
+00027280: 2e73 632e 6669 672e 7469 6768 745f 6c61  .sc.fig.tight_la
+00027290: 796f 7574 2829 0a20 2020 2020 2020 2061  yout().        a
+000272a0: 7070 2e65 7865 635f 2829 0a0a 2020 2020  pp.exec_()..    
+000272b0: 7265 7475 726e 0a0a 0a64 6566 205f 706c  return...def _pl
+000272c0: 6f74 5f72 6174 655f 7265 7369 6475 616c  ot_rate_residual
+000272d0: 7328 6461 7461 7365 743a 2054 6175 5444  s(dataset: TauTD
+000272e0: 6174 6173 6574 207c 2054 6175 4844 6174  ataset | TauHDat
+000272f0: 6173 6574 2c0a 2020 2020 2020 2020 2020  aset,.          
+00027300: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00027310: 6f64 656c 3a20 4c6f 6754 6175 544d 6f64  odel: LogTauTMod
+00027320: 656c 207c 204d 756c 7469 4c6f 6754 6175  el | MultiLogTau
+00027330: 544d 6f64 656c 207c 204c 6f67 5461 7548  TModel | LogTauH
+00027340: 4d6f 6465 6c20 7c20 4d75 6c74 694c 6f67  Model | MultiLog
+00027350: 5461 7548 4d6f 6465 6c2c 2023 206e 6f71  TauHModel, # noq
+00027360: 610a 2020 2020 2020 2020 2020 2020 2020  a.              
+00027370: 2020 2020 2020 2020 2020 2061 783a 2070             ax: p
+00027380: 6c74 2e41 7865 7329 202d 3e20 4e6f 6e65  lt.Axes) -> None
+00027390: 3a0a 2020 2020 2727 270a 2020 2020 506c  :.    '''.    Pl
+000273a0: 6f74 7320 6469 6666 6572 656e 6365 206f  ots difference o
+000273b0: 6620 6c6f 6731 3028 6578 7065 7269 6d65  f log10(experime
+000273c0: 6e74 2920 616e 6420 6c6f 6731 3028 6d6f  nt) and log10(mo
+000273d0: 6465 6c29 2072 656c 6178 6174 696f 6e20  del) relaxation 
+000273e0: 7261 7465 730a 2020 2020 6f6e 746f 2061  rates.    onto a
+000273f0: 2067 6976 656e 2066 6967 7572 6520 616e   given figure an
+00027400: 6420 6178 6973 0a0a 2020 2020 5061 7261  d axis..    Para
+00027410: 6d65 7465 7273 0a20 2020 202d 2d2d 2d2d  meters.    -----
+00027420: 2d2d 2d2d 2d0a 2020 2020 6d6f 6465 6c73  -----.    models
+00027430: 3a20 6c69 7374 5b4c 6f67 5461 7554 4d6f  : list[LogTauTMo
+00027440: 6465 6c20 7c20 4d75 6c74 694c 6f67 5461  del | MultiLogTa
+00027450: 7554 4d6f 6465 6c20 7c20 4c6f 6754 6175  uTModel | LogTau
+00027460: 484d 6f64 656c 207c 204d 756c 7469 4c6f  HModel | MultiLo
+00027470: 6754 6175 484d 6f64 656c 5d0a 2020 2020  gTauHModel].    
+00027480: 2020 2020 4d6f 6465 6c73 2c20 6f6e 6520      Models, one 
+00027490: 7065 7220 7465 6d70 6572 6174 7572 650a  per temperature.
+000274a0: 2020 2020 6669 6c65 5f6e 616d 653a 2073      file_name: s
+000274b0: 7472 0a20 2020 2020 2020 204e 616d 6520  tr.        Name 
+000274c0: 6f66 206f 7574 7075 7420 6669 6c65 0a20  of output file. 
+000274d0: 2020 2061 783a 2070 6c74 2e41 7865 730a     ax: plt.Axes.
+000274e0: 2020 2020 2020 2020 4d61 7470 6c6f 746c          Matplotl
+000274f0: 6962 2041 7869 7320 6f62 6a65 6374 2075  ib Axis object u
+00027500: 7365 6420 666f 7220 706c 6f74 0a0a 2020  sed for plot..  
+00027510: 2020 5265 7475 726e 730a 2020 2020 2d2d    Returns.    --
+00027520: 2d2d 2d2d 2d0a 2020 2020 4e6f 6e65 0a20  -----.    None. 
+00027530: 2020 2027 2727 2023 206e 6f71 610a 0a20     ''' # noqa.. 
+00027540: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+00027550: 2864 6174 6173 6574 2c20 5461 7548 4461  (dataset, TauHDa
+00027560: 7461 7365 7429 3a0a 2020 2020 2020 2020  taset):.        
+00027570: 785f 7661 7273 203d 2064 6174 6173 6574  x_vars = dataset
+00027580: 2e66 6965 6c64 730a 2020 2020 2020 2020  .fields.        
+00027590: 6178 2e73 6574 5f78 6c61 6265 6c28 7227  ax.set_xlabel(r'
+000275a0: 4669 656c 6420 284f 6529 2729 0a20 2020  Field (Oe)').   
+000275b0: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
+000275c0: 2864 6174 6173 6574 2c20 5461 7554 4461  (dataset, TauTDa
+000275d0: 7461 7365 7429 3a0a 2020 2020 2020 2020  taset):.        
+000275e0: 785f 7661 7273 203d 2064 6174 6173 6574  x_vars = dataset
+000275f0: 2e74 656d 7065 7261 7475 7265 730a 2020  .temperatures.  
+00027600: 2020 2020 2020 6178 2e73 6574 5f78 6c61        ax.set_xla
+00027610: 6265 6c28 7227 5465 6d70 6572 6174 7572  bel(r'Temperatur
+00027620: 6520 284b 2927 290a 0a20 2020 2023 2041  e (K)')..    # A
+00027630: 6464 2061 6464 6974 696f 6e61 6c20 7365  dd additional se
+00027640: 7420 6f66 2061 7865 7320 746f 2063 7265  t of axes to cre
+00027650: 6174 6520 277a 6572 6f27 206c 696e 650a  ate 'zero' line.
+00027660: 2020 2020 6178 3220 3d20 6178 2e74 7769      ax2 = ax.twi
+00027670: 6e79 2829 0a20 2020 2061 7832 2e67 6574  ny().    ax2.get
+00027680: 5f79 6178 6973 2829 2e73 6574 5f76 6973  _yaxis().set_vis
+00027690: 6962 6c65 2846 616c 7365 290a 2020 2020  ible(False).    
+000276a0: 6178 322e 7365 745f 7974 6963 6b73 285b  ax2.set_yticks([
+000276b0: 5d29 0a20 2020 2061 7832 2e73 6574 5f78  ]).    ax2.set_x
+000276c0: 7469 636b 7328 5b5d 290a 2020 2020 6178  ticks([]).    ax
+000276d0: 322e 7370 696e 6573 5b27 626f 7474 6f6d  2.spines['bottom
+000276e0: 275d 2e73 6574 5f70 6f73 6974 696f 6e28  '].set_position(
+000276f0: 2827 7a65 726f 2729 290a 0a20 2020 2069  ('zero'))..    i
+00027700: 6620 7479 7065 286d 6f64 656c 2920 696e  f type(model) in
+00027710: 205b 4d75 6c74 694c 6f67 5461 7554 4d6f   [MultiLogTauTMo
+00027720: 6465 6c2c 204d 756c 7469 4c6f 6754 6175  del, MultiLogTau
+00027730: 484d 6f64 656c 5d3a 0a20 2020 2020 2020  HModel]:.       
+00027740: 206c 6f67 6d6f 6465 6c73 203d 206d 6f64   logmodels = mod
+00027750: 656c 2e6c 6f67 6d6f 6465 6c73 0a20 2020  el.logmodels.   
+00027760: 2065 6c73 653a 0a20 2020 2020 2020 206c   else:.        l
+00027770: 6f67 6d6f 6465 6c73 203d 205b 6d6f 6465  ogmodels = [mode
+00027780: 6c5d 0a0a 2020 2020 6d6f 6465 6c5f 7261  l]..    model_ra
+00027790: 7465 203d 206e 702e 7a65 726f 7328 6c65  te = np.zeros(le
+000277a0: 6e28 785f 7661 7273 2929 0a0a 2020 2020  n(x_vars))..    
+000277b0: 666f 7220 6c6f 676d 6f64 656c 2069 6e20  for logmodel in 
+000277c0: 6c6f 676d 6f64 656c 733a 0a20 2020 2020  logmodels:.     
+000277d0: 2020 206d 6f64 656c 5f72 6174 6520 2b3d     model_rate +=
+000277e0: 2031 302a 2a6c 6f67 6d6f 6465 6c2e 6d6f   10**logmodel.mo
+000277f0: 6465 6c28 0a20 2020 2020 2020 2020 2020  del(.           
+00027800: 206c 6f67 6d6f 6465 6c2e 6669 6e61 6c5f   logmodel.final_
+00027810: 7661 725f 7661 6c75 6573 2c0a 2020 2020  var_values,.    
+00027820: 2020 2020 2020 2020 785f 7661 7273 2c0a          x_vars,.
+00027830: 2020 2020 2020 2020 290a 0a20 2020 206d          )..    m
+00027840: 6f64 656c 5f6c 6f67 7261 7465 203d 206e  odel_lograte = n
+00027850: 702e 6c6f 6731 3028 6d6f 6465 6c5f 7261  p.log10(model_ra
+00027860: 7465 290a 0a20 2020 2023 2050 6c6f 7420  te)..    # Plot 
+00027870: 7265 7369 6475 616c 730a 2020 2020 6966  residuals.    if
+00027880: 206c 656e 2864 6174 6173 6574 2e6c 6f67   len(dataset.log
+00027890: 7261 7465 5f70 6d29 3a0a 2020 2020 2020  rate_pm):.      
+000278a0: 2020 6178 2e65 7272 6f72 6261 7228 0a20    ax.errorbar(. 
+000278b0: 2020 2020 2020 2020 2020 2078 5f76 6172             x_var
+000278c0: 732c 0a20 2020 2020 2020 2020 2020 206e  s,.            n
+000278d0: 702e 6c6f 6731 3028 6461 7461 7365 742e  p.log10(dataset.
+000278e0: 7261 7465 7329 202d 206d 6f64 656c 5f6c  rates) - model_l
+000278f0: 6f67 7261 7465 2c0a 2020 2020 2020 2020  ograte,.        
+00027900: 2020 2020 7965 7272 3d64 6174 6173 6574      yerr=dataset
+00027910: 2e6c 6f67 7261 7465 5f70 6d2c 0a20 2020  .lograte_pm,.   
+00027920: 2020 2020 2020 2020 2066 6d74 3d27 622e           fmt='b.
+00027930: 270a 2020 2020 2020 2020 290a 2020 2020  '.        ).    
+00027940: 656c 7365 3a0a 2020 2020 2020 2020 6178  else:.        ax
+00027950: 2e70 6c6f 7428 0a20 2020 2020 2020 2020  .plot(.         
+00027960: 2020 2078 5f76 6172 732c 0a20 2020 2020     x_vars,.     
+00027970: 2020 2020 2020 206e 702e 6c6f 6731 3028         np.log10(
+00027980: 6461 7461 7365 742e 7261 7465 7329 202d  dataset.rates) -
+00027990: 206d 6f64 656c 5f6c 6f67 7261 7465 2c0a   model_lograte,.
+000279a0: 2020 2020 2020 2020 2020 2020 636f 6c6f              colo
+000279b0: 723d 2762 272c 0a20 2020 2020 2020 2020  r='b',.         
+000279c0: 2020 206d 6172 6b65 723d 276f 272c 0a20     marker='o',. 
+000279d0: 2020 2020 2020 2020 2020 206c 773d 302c             lw=0,
+000279e0: 0a20 2020 2020 2020 2020 2020 2066 696c  .            fil
+000279f0: 6c73 7479 6c65 3d27 6e6f 6e65 272c 0a20  lstyle='none',. 
+00027a00: 2020 2020 2020 2020 2020 206c 6162 656c             label
+00027a10: 3d27 4578 7065 7269 6d65 6e74 270a 2020  ='Experiment'.  
+00027a20: 2020 2020 2020 290a 2020 2020 2320 5365        ).    # Se
+00027a30: 7420 6c6f 6720 7363 616c 6520 6f6e 2078  t log scale on x
+00027a40: 2061 7869 730a 2020 2020 6178 2e73 6574   axis.    ax.set
+00027a50: 5f78 7363 616c 6528 276c 6f67 2729 0a0a  _xscale('log')..
+00027a60: 2020 2020 2320 5365 7420 666f 726d 6174      # Set format
+00027a70: 7469 6e67 2066 6f72 2079 2061 7869 7320  ting for y axis 
+00027a80: 6d61 6a6f 7220 7469 636b 730a 2020 2020  major ticks.    
+00027a90: 6178 2e79 6178 6973 2e73 6574 5f6d 616a  ax.yaxis.set_maj
+00027aa0: 6f72 5f66 6f72 6d61 7474 6572 2853 6361  or_formatter(Sca
+00027ab0: 6c61 7246 6f72 6d61 7474 6572 2829 290a  larFormatter()).
+00027ac0: 0a20 2020 2023 2041 6464 206d 696e 6f72  .    # Add minor
+00027ad0: 2074 6963 6b73 2074 6f20 7920 6178 6973   ticks to y axis
+00027ae0: 2077 6974 6820 6e6f 206c 6162 656c 730a   with no labels.
+00027af0: 2020 2020 6178 2e79 6178 6973 2e73 6574      ax.yaxis.set
+00027b00: 5f6d 696e 6f72 5f6c 6f63 6174 6f72 2841  _minor_locator(A
+00027b10: 7574 6f4d 696e 6f72 4c6f 6361 746f 7228  utoMinorLocator(
+00027b20: 2929 0a0a 2020 2020 2320 5379 6d6d 6574  ))..    # Symmet
+00027b30: 7269 7365 2079 2061 7869 7320 6c69 6d69  rise y axis limi
+00027b40: 7473 2062 6173 6564 206f 6e20 6d61 7820  ts based on max 
+00027b50: 6162 7320 6572 726f 720a 2020 2020 6966  abs error.    if
+00027b60: 206c 656e 2864 6174 6173 6574 2e6c 6f67   len(dataset.log
+00027b70: 7261 7465 5f70 6d29 3a0a 2020 2020 2020  rate_pm):.      
+00027b80: 2020 616c 6c5f 6461 7461 203d 205b 0a20    all_data = [. 
+00027b90: 2020 2020 2020 2020 2020 206e 702e 6c6f             np.lo
+00027ba0: 6731 3028 6461 7461 7365 742e 7261 7465  g10(dataset.rate
+00027bb0: 7329 202d 206d 6f64 656c 5f6c 6f67 7261  s) - model_logra
+00027bc0: 7465 202b 2064 6174 6173 6574 2e6c 6f67  te + dataset.log
+00027bd0: 7261 7465 5f70 6d0a 2020 2020 2020 2020  rate_pm.        
+00027be0: 5d0a 2020 2020 2020 2020 616c 6c5f 6461  ].        all_da
+00027bf0: 7461 202b 3d20 5b0a 2020 2020 2020 2020  ta += [.        
+00027c00: 2020 2020 6e70 2e6c 6f67 3130 2864 6174      np.log10(dat
+00027c10: 6173 6574 2e72 6174 6573 2920 2d20 6d6f  aset.rates) - mo
+00027c20: 6465 6c5f 6c6f 6772 6174 6520 2d20 6461  del_lograte - da
+00027c30: 7461 7365 742e 6c6f 6772 6174 655f 706d  taset.lograte_pm
+00027c40: 0a20 2020 2020 2020 205d 0a20 2020 2065  .        ].    e
+00027c50: 6c73 653a 0a20 2020 2020 2020 2061 6c6c  lse:.        all
+00027c60: 5f64 6174 6120 3d20 5b0a 2020 2020 2020  _data = [.      
+00027c70: 2020 2020 2020 6e70 2e6c 6f67 3130 2864        np.log10(d
+00027c80: 6174 6173 6574 2e72 6174 6573 2920 2d20  ataset.rates) - 
+00027c90: 6d6f 6465 6c5f 6c6f 6772 6174 650a 2020  model_lograte.  
+00027ca0: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
+00027cb0: 616c 6c5f 6461 7461 202b 3d20 5b0a 2020  all_data += [.  
+00027cc0: 2020 2020 2020 2020 2020 6e70 2e6c 6f67            np.log
+00027cd0: 3130 2864 6174 6173 6574 2e72 6174 6573  10(dataset.rates
+00027ce0: 2920 2d20 6d6f 6465 6c5f 6c6f 6772 6174  ) - model_lograt
+00027cf0: 650a 2020 2020 2020 2020 5d0a 0a20 2020  e.        ]..   
+00027d00: 2074 6963 6b73 2c20 6d61 7876 616c 203d   ticks, maxval =
+00027d10: 2067 7569 2e6d 696e 5f6d 6178 5f74 6963   gui.min_max_tic
+00027d20: 6b73 5f77 6974 685f 7a65 726f 2861 6c6c  ks_with_zero(all
+00027d30: 5f64 6174 612c 2035 290a 2020 2020 6178  _data, 5).    ax
+00027d40: 2e73 6574 5f79 7469 636b 7328 7469 636b  .set_yticks(tick
+00027d50: 7329 0a0a 2020 2020 6178 2e73 6574 5f79  s)..    ax.set_y
+00027d60: 6c69 6d28 5b2d 206d 6178 7661 6c20 2a20  lim([- maxval * 
+00027d70: 312e 312c 202b 206d 6178 7661 6c20 2a20  1.1, + maxval * 
+00027d80: 312e 315d 290a 0a20 2020 2023 2041 7869  1.1])..    # Axi
+00027d90: 7320 6c61 6265 6c73 0a20 2020 2061 782e  s labels.    ax.
+00027da0: 7365 745f 796c 6162 656c 280a 2020 2020  set_ylabel(.    
+00027db0: 2020 2020 7227 245c 6c6f 675f 5c6d 6174      r'$\log_\mat
+00027dc0: 6872 6567 756c 6172 7b31 307d 5b5c 7461  hregular{10}[\ta
+00027dd0: 755e 5c6d 6174 6872 6567 756c 6172 7b2d  u^\mathregular{-
+00027de0: 317d 5f7b 5c6d 6174 6872 6567 756c 6172  1}_{\mathregular
+00027df0: 7b65 7870 7d7d 5d24 202d 2024 5c6c 6f67  {exp}}]$ - $\log
+00027e00: 5f5c 6d61 7468 7265 6775 6c61 727b 3130  _\mathregular{10
+00027e10: 7d5b 5c74 6175 5e5c 6d61 7468 7265 6775  }[\tau^\mathregu
+00027e20: 6c61 727b 2d31 7d5f 7b5c 6d61 7468 7265  lar{-1}_{\mathre
+00027e30: 6775 6c61 727b 6669 747d 7d5d 2427 2023  gular{fit}}]$' #
+00027e40: 206e 6f71 610a 2020 2020 290a 0a20 2020   noqa.    )..   
+00027e50: 2023 2053 6574 2078 2074 6963 6b20 666f   # Set x tick fo
+00027e60: 726d 6174 7469 6e67 0a20 2020 2067 7569  rmatting.    gui
+00027e70: 2e73 6574 5f72 6174 655f 7874 6963 6b5f  .set_rate_xtick_
+00027e80: 666f 726d 6174 7469 6e67 2861 782c 2078  formatting(ax, x
+00027e90: 5f76 6172 7329 0a0a 2020 2020 7265 7475  _vars)..    retu
+00027ea0: 726e 0a0a 0a64 6566 2077 7269 7465 5f6d  rn...def write_m
+00027eb0: 6f64 656c 5f70 6172 616d 7328 6d6f 6465  odel_params(mode
+00027ec0: 6c3a 204c 6f67 5461 7554 4d6f 6465 6c20  l: LogTauTModel 
+00027ed0: 7c20 4d75 6c74 694c 6f67 5461 7554 4d6f  | MultiLogTauTMo
+00027ee0: 6465 6c20 7c20 4c6f 6754 6175 484d 6f64  del | LogTauHMod
+00027ef0: 656c 207c 204d 756c 7469 4c6f 6754 6175  el | MultiLogTau
+00027f00: 484d 6f64 656c 2c20 2320 6e6f 7161 0a20  HModel, # noqa. 
+00027f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027f20: 2020 2020 2020 6669 6c65 5f6e 616d 653a        file_name:
+00027f30: 2073 7472 2c20 7665 7262 6f73 653a 2062   str, verbose: b
+00027f40: 6f6f 6c20 3d20 5472 7565 2920 2d3e 204e  ool = True) -> N
+00027f50: 6f6e 653a 0a20 2020 2027 2727 0a20 2020  one:.    '''.   
+00027f60: 2057 7269 7465 7320 6669 7474 6564 2061   Writes fitted a
+00027f70: 6e64 2066 6978 6564 2070 6172 616d 6574  nd fixed paramet
+00027f80: 6572 7320 6f66 206d 6f64 656c 2873 2920  ers of model(s) 
+00027f90: 746f 2066 696c 650a 0a20 2020 2050 6172  to file..    Par
+00027fa0: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
+00027fb0: 2d2d 2d2d 2d2d 0a20 2020 206d 6f64 656c  ------.    model
+00027fc0: 733a 206c 6973 745b 4c6f 6754 6175 544d  s: list[LogTauTM
+00027fd0: 6f64 656c 207c 204d 756c 7469 4c6f 6754  odel | MultiLogT
+00027fe0: 6175 544d 6f64 656c 207c 204c 6f67 5461  auTModel | LogTa
+00027ff0: 7548 4d6f 6465 6c20 7c20 4d75 6c74 694c  uHModel | MultiL
+00028000: 6f67 5461 7548 4d6f 6465 6c5d 0a20 2020  ogTauHModel].   
+00028010: 2020 2020 204d 6f64 656c 732c 206f 6e65       Models, one
+00028020: 2070 6572 2074 656d 7065 7261 7475 7265   per temperature
+00028030: 0a20 2020 2066 696c 655f 6e61 6d65 3a20  .    file_name: 
+00028040: 7374 720a 2020 2020 2020 2020 4e61 6d65  str.        Name
+00028050: 206f 6620 6f75 7470 7574 2066 696c 650a   of output file.
+00028060: 2020 2020 7665 7262 6f73 653a 2062 6f6f      verbose: boo
+00028070: 6c2c 2064 6566 6175 6c74 2054 7275 650a  l, default True.
+00028080: 2020 2020 2020 2020 4966 2054 7275 652c          If True,
+00028090: 206f 7574 7075 7420 6669 6c65 206c 6f63   output file loc
+000280a0: 6174 696f 6e20 6973 2077 7269 7474 656e  ation is written
+000280b0: 2074 6f20 7465 726d 696e 616c 0a0a 2020   to terminal..  
+000280c0: 2020 5265 7475 726e 730a 2020 2020 2d2d    Returns.    --
+000280d0: 2d2d 2d2d 2d0a 2020 2020 4e6f 6e65 0a20  -----.    None. 
+000280e0: 2020 2027 2727 2023 206e 6f71 610a 0a20     ''' # noqa.. 
+000280f0: 2020 2069 6620 7479 7065 286d 6f64 656c     if type(model
+00028100: 2920 696e 205b 4d75 6c74 694c 6f67 5461  ) in [MultiLogTa
+00028110: 7554 4d6f 6465 6c2c 204d 756c 7469 4c6f  uTModel, MultiLo
+00028120: 6754 6175 484d 6f64 656c 5d3a 0a20 2020  gTauHModel]:.   
+00028130: 2020 2020 206c 6f67 6d6f 6465 6c73 203d       logmodels =
+00028140: 206d 6f64 656c 2e6c 6f67 6d6f 6465 6c73   model.logmodels
+00028150: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+00028160: 2020 206c 6f67 6d6f 6465 6c73 203d 205b     logmodels = [
+00028170: 6d6f 6465 6c5d 0a0a 2020 2020 6620 3d20  model]..    f = 
+00028180: 6f70 656e 2866 696c 655f 6e61 6d65 2c20  open(file_name, 
+00028190: 2777 272c 2065 6e63 6f64 696e 673d 2775  'w', encoding='u
+000281a0: 7466 2d38 2729 0a0a 2020 2020 2320 5772  tf-8')..    # Wr
+000281b0: 6974 6520 6561 6368 2074 6572 6d27 7320  ite each term's 
+000281c0: 6e61 6d65 2c20 6669 7420 7661 7273 2c20  name, fit vars, 
+000281d0: 7374 6465 762c 2061 6e64 2066 6978 2076  stdev, and fix v
+000281e0: 6172 730a 2020 2020 666f 7220 6c6f 676d  ars.    for logm
+000281f0: 6f64 656c 2069 6e20 6c6f 676d 6f64 656c  odel in logmodel
+00028200: 733a 0a20 2020 2020 2020 2066 2e77 7269  s:.        f.wri
+00028210: 7465 2827 7b7d 5c6e 272e 666f 726d 6174  te('{}\n'.format
+00028220: 286c 6f67 6d6f 6465 6c2e 4e41 4d45 2929  (logmodel.NAME))
+00028230: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
+00028240: 6c6f 676d 6f64 656c 2e66 6974 5f76 6172  logmodel.fit_var
+00028250: 732e 6b65 7973 2829 293a 0a20 2020 2020  s.keys()):.     
+00028260: 2020 2020 2020 2066 2e77 7269 7465 2827         f.write('
+00028270: 4669 7474 6564 2054 6572 6d73 3a20 5661  Fitted Terms: Va
+00028280: 6c75 6520 616e 6420 5374 616e 6461 7264  lue and Standard
+00028290: 2044 6576 6961 7469 6f6e 3a5c 6e27 290a   Deviation:\n').
+000282a0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+000282b0: 6e61 6d65 2069 6e20 6c6f 676d 6f64 656c  name in logmodel
+000282c0: 2e66 6974 5f76 6172 732e 6b65 7973 2829  .fit_vars.keys()
+000282d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000282e0: 2020 662e 7772 6974 6528 277b 3a3e 367d    f.write('{:>6}
+000282f0: 207b 3a20 312e 3845 7d20 7b3a 2031 2e38   {: 1.8E} {: 1.8
+00028300: 457d 207b 7d5c 6e27 2e66 6f72 6d61 7428  E} {}\n'.format(
+00028310: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00028320: 2020 2020 206e 616d 652c 0a20 2020 2020       name,.     
+00028330: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00028340: 6f67 6d6f 6465 6c2e 6669 6e61 6c5f 7661  ogmodel.final_va
+00028350: 725f 7661 6c75 6573 5b6e 616d 655d 2c0a  r_values[name],.
+00028360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028370: 2020 2020 6c6f 676d 6f64 656c 2e66 6974      logmodel.fit
+00028380: 5f73 7464 6576 5b6e 616d 655d 2c0a 2020  _stdev[name],.  
+00028390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000283a0: 2020 6c6f 676d 6f64 656c 2e55 4e49 5453    logmodel.UNITS
+000283b0: 5b6e 616d 655d 0a20 2020 2020 2020 2020  [name].         
+000283c0: 2020 2020 2020 2029 290a 2020 2020 2020         )).      
+000283d0: 2020 6966 206c 656e 286c 6f67 6d6f 6465    if len(logmode
+000283e0: 6c2e 6669 785f 7661 7273 2e6b 6579 7328  l.fix_vars.keys(
+000283f0: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
+00028400: 662e 7772 6974 6528 2746 6978 6564 2054  f.write('Fixed T
+00028410: 6572 6d73 3a20 5661 6c75 6573 5c6e 2729  erms: Values\n')
+00028420: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00028430: 206e 616d 6520 696e 206c 6f67 6d6f 6465   name in logmode
+00028440: 6c2e 6669 785f 7661 7273 2e6b 6579 7328  l.fix_vars.keys(
+00028450: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00028460: 2020 2066 2e77 7269 7465 2827 7b3a 3e36     f.write('{:>6
+00028470: 7d20 7b3a 2031 2e38 457d 207b 7d5c 6e27  } {: 1.8E} {}\n'
+00028480: 2e66 6f72 6d61 7428 0a20 2020 2020 2020  .format(.       
+00028490: 2020 2020 2020 2020 2020 2020 206e 616d               nam
+000284a0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+000284b0: 2020 2020 2020 206c 6f67 6d6f 6465 6c2e         logmodel.
+000284c0: 6669 6e61 6c5f 7661 725f 7661 6c75 6573  final_var_values
+000284d0: 5b6e 616d 655d 2c0a 2020 2020 2020 2020  [name],.        
+000284e0: 2020 2020 2020 2020 2020 2020 6c6f 676d              logm
+000284f0: 6f64 656c 2e55 4e49 5453 5b6e 616d 655d  odel.UNITS[name]
+00028500: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00028510: 2029 290a 2020 2020 2020 2020 662e 7772   )).        f.wr
+00028520: 6974 6528 275c 6e27 290a 0a20 2020 2069  ite('\n')..    i
+00028530: 6620 7665 7262 6f73 653a 0a20 2020 2020  f verbose:.     
+00028540: 2020 2075 742e 6370 7269 6e74 280a 2020     ut.cprint(.  
+00028550: 2020 2020 2020 2020 2020 275c 6e20 5265            '\n Re
+00028560: 6c61 7861 7469 6f6e 204d 6f64 656c 2070  laxation Model p
+00028570: 6172 616d 6574 6572 7320 7772 6974 7465  arameters writte
+00028580: 6e20 746f 205c 6e20 7b7d 5c6e 272e 666f  n to \n {}\n'.fo
+00028590: 726d 6174 280a 2020 2020 2020 2020 2020  rmat(.          
+000285a0: 2020 2020 2020 6669 6c65 5f6e 616d 650a        file_name.
+000285b0: 2020 2020 2020 2020 2020 2020 292c 0a20              ),. 
+000285c0: 2020 2020 2020 2020 2020 2027 6379 616e             'cyan
+000285d0: 270a 2020 2020 2020 2020 290a 0a20 2020  '.        )..   
+000285e0: 2072 6574 7572 6e0a 0a0a 6465 6620 7772   return...def wr
+000285f0: 6974 655f 6d6f 6465 6c5f 6461 7461 2864  ite_model_data(d
+00028600: 6174 6173 6574 3a20 5461 7554 4461 7461  ataset: TauTData
+00028610: 7365 7420 7c20 5461 7548 4461 7461 7365  set | TauHDatase
+00028620: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
+00028630: 2020 2020 2020 2020 6d6f 6465 6c3a 204c          model: L
+00028640: 6f67 5461 7554 4d6f 6465 6c20 7c20 4d75  ogTauTModel | Mu
+00028650: 6c74 694c 6f67 5461 7554 4d6f 6465 6c20  ltiLogTauTModel 
+00028660: 7c20 4c6f 6754 6175 484d 6f64 656c 207c  | LogTauHModel |
+00028670: 204d 756c 7469 4c6f 6754 6175 484d 6f64   MultiLogTauHMod
+00028680: 656c 2c20 2320 6e6f 7161 0a20 2020 2020  el, # noqa.     
+00028690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000286a0: 6669 6c65 5f6e 616d 653a 2073 7472 2c20  file_name: str, 
+000286b0: 7665 7262 6f73 653a 2062 6f6f 6c20 3d20  verbose: bool = 
+000286c0: 5472 7565 2920 2d3e 204e 6f6e 653a 0a20  True) -> None:. 
+000286d0: 2020 2027 2727 0a20 2020 2043 7265 6174     '''.    Creat
+000286e0: 6573 2066 696c 6520 636f 6e74 6169 6e69  es file containi
+000286f0: 6e67 2072 6174 6520 7673 2074 656d 7065  ng rate vs tempe
+00028700: 7261 7475 7265 2f66 6965 6c64 2063 616c  rature/field cal
+00028710: 6375 6c61 7465 6420 7573 696e 6720 6d6f  culated using mo
+00028720: 6465 6c0a 2020 2020 7061 7261 6d65 7465  del.    paramete
+00028730: 7273 0a0a 2020 2020 5061 7261 6d65 7465  rs..    Paramete
+00028740: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
+00028750: 2d0a 2020 2020 6461 7461 7365 743a 2054  -.    dataset: T
+00028760: 6175 5444 6174 6173 6574 207c 2054 6175  auTDataset | Tau
+00028770: 4844 6174 6173 6574 0a20 2020 2020 2020  HDataset.       
+00028780: 2044 6174 6173 6574 2074 6f20 7768 6963   Dataset to whic
+00028790: 6820 6120 6d6f 6465 6c20 7761 7320 7375  h a model was su
+000287a0: 6363 6573 7366 756c 6c79 2066 6974 7465  ccessfully fitte
+000287b0: 6420 2869 2e65 2e20 6669 745f 7374 6174  d (i.e. fit_stat
+000287c0: 7573 3d54 7275 6529 0a20 2020 206d 6f64  us=True).    mod
+000287d0: 656c 3a20 4c6f 6754 6175 544d 6f64 656c  el: LogTauTModel
+000287e0: 207c 204d 756c 7469 4c6f 6754 6175 544d   | MultiLogTauTM
+000287f0: 6f64 656c 207c 204c 6f67 5461 7548 4d6f  odel | LogTauHMo
+00028800: 6465 6c20 7c20 4d75 6c74 694c 6f67 5461  del | MultiLogTa
+00028810: 7548 4d6f 6465 6c0a 2020 2020 2020 2020  uHModel.        
+00028820: 4d6f 6465 6c20 7768 6963 6820 6861 7320  Model which has 
+00028830: 6265 656e 2066 6974 7465 6420 746f 2064  been fitted to d
+00028840: 6174 6173 6574 0a20 2020 2066 696c 655f  ataset.    file_
+00028850: 6e61 6d65 3a20 7374 720a 2020 2020 2020  name: str.      
+00028860: 2020 4e61 6d65 206f 6620 6f75 7470 7574    Name of output
+00028870: 2066 696c 650a 2020 2020 7665 7262 6f73   file.    verbos
+00028880: 653a 2062 6f6f 6c2c 2064 6566 6175 6c74  e: bool, default
+00028890: 2054 7275 650a 2020 2020 2020 2020 4966   True.        If
+000288a0: 2054 7275 652c 206f 7574 7075 7420 6669   True, output fi
+000288b0: 6c65 206c 6f63 6174 696f 6e20 6973 2077  le location is w
+000288c0: 7269 7474 656e 2074 6f20 7465 726d 696e  ritten to termin
+000288d0: 616c 0a0a 2020 2020 5265 7475 726e 730a  al..    Returns.
+000288e0: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
+000288f0: 4e6f 6e65 0a20 2020 2027 2727 0a0a 2020  None.    '''..  
+00028900: 2020 6966 206e 6f74 206d 6f64 656c 2e66    if not model.f
+00028910: 6974 5f73 7461 7475 733a 0a20 2020 2020  it_status:.     
+00028920: 2020 2072 6574 7572 6e0a 0a20 2020 2069     return..    i
+00028930: 6620 6973 696e 7374 616e 6365 2864 6174  f isinstance(dat
+00028940: 6173 6574 2c20 5461 7548 4461 7461 7365  aset, TauHDatase
+00028950: 7429 3a0a 2020 2020 2020 2020 785f 7661  t):.        x_va
+00028960: 7273 203d 2064 6174 6173 6574 2e66 6965  rs = dataset.fie
+00028970: 6c64 730a 2020 2020 2020 2020 785f 7661  lds.        x_va
+00028980: 725f 6c61 6265 6c20 3d20 2748 2028 4f65  r_label = 'H (Oe
+00028990: 2927 0a0a 2020 2020 656c 6966 2069 7369  )'..    elif isi
+000289a0: 6e73 7461 6e63 6528 6461 7461 7365 742c  nstance(dataset,
+000289b0: 2054 6175 5444 6174 6173 6574 293a 0a20   TauTDataset):. 
+000289c0: 2020 2020 2020 2078 5f76 6172 7320 3d20         x_vars = 
+000289d0: 6461 7461 7365 742e 7465 6d70 6572 6174  dataset.temperat
+000289e0: 7572 6573 0a20 2020 2020 2020 2078 5f76  ures.        x_v
+000289f0: 6172 5f6c 6162 656c 203d 2027 5420 284b  ar_label = 'T (K
+00028a00: 2927 0a0a 2020 2020 6966 2074 7970 6528  )'..    if type(
+00028a10: 6d6f 6465 6c29 2069 6e20 5b4d 756c 7469  model) in [Multi
+00028a20: 4c6f 6754 6175 544d 6f64 656c 2c20 4d75  LogTauTModel, Mu
+00028a30: 6c74 694c 6f67 5461 7548 4d6f 6465 6c5d  ltiLogTauHModel]
+00028a40: 3a0a 2020 2020 2020 2020 6c6f 676d 6f64  :.        logmod
+00028a50: 656c 7320 3d20 6d6f 6465 6c2e 6c6f 676d  els = model.logm
+00028a60: 6f64 656c 730a 2020 2020 656c 7365 3a0a  odels.    else:.
+00028a70: 2020 2020 2020 2020 6c6f 676d 6f64 656c          logmodel
+00028a80: 7320 3d20 5b6d 6f64 656c 5d0a 0a20 2020  s = [model]..   
+00028a90: 2066 203d 206f 7065 6e28 6669 6c65 5f6e   f = open(file_n
+00028aa0: 616d 652c 2027 7727 2c20 656e 636f 6469  ame, 'w', encodi
+00028ab0: 6e67 3d27 7574 662d 3827 290a 0a20 2020  ng='utf-8')..   
+00028ac0: 2078 5f76 6172 735f 6772 6964 203d 206e   x_vars_grid = n
+00028ad0: 702e 6c6f 6773 7061 6365 280a 2020 2020  p.logspace(.    
+00028ae0: 2020 2020 6e70 2e6c 6f67 3130 286e 702e      np.log10(np.
+00028af0: 6d69 6e28 785f 7661 7273 2929 2c0a 2020  min(x_vars)),.  
+00028b00: 2020 2020 2020 6e70 2e6c 6f67 3130 286e        np.log10(n
+00028b10: 702e 6d61 7828 785f 7661 7273 2929 2c0a  p.max(x_vars)),.
+00028b20: 2020 2020 2020 2020 3130 300a 2020 2020          100.    
+00028b30: 290a 0a20 2020 2066 2e77 7269 7465 2827  )..    f.write('
+00028b40: 7b3a 3e39 7d20 272e 666f 726d 6174 2878  {:>9} '.format(x
+00028b50: 5f76 6172 5f6c 6162 656c 2929 0a20 2020  _var_label)).   
+00028b60: 2066 6f72 206c 6f67 6d6f 6465 6c20 696e   for logmodel in
+00028b70: 206c 6f67 6d6f 6465 6c73 3a0a 2020 2020   logmodels:.    
+00028b80: 2020 2020 662e 7772 6974 6528 277b 3a3e      f.write('{:>
+00028b90: 377d 2072 6174 6520 272e 666f 726d 6174  7} rate '.format
+00028ba0: 286c 6f67 6d6f 6465 6c2e 4e41 4d45 2929  (logmodel.NAME))
+00028bb0: 0a20 2020 2069 6620 6c65 6e28 6c6f 676d  .    if len(logm
+00028bc0: 6f64 656c 7329 203e 2031 3a0a 2020 2020  odels) > 1:.    
+00028bd0: 2020 2020 662e 7772 6974 6528 2720 2054      f.write('  T
+00028be0: 6f74 616c 2072 6174 6520 2873 5e2d 3129  otal rate (s^-1)
+00028bf0: 2729 0a20 2020 2066 2e77 7269 7465 2827  ').    f.write('
+00028c00: 5c6e 2729 0a0a 2020 2020 666f 7220 6772  \n')..    for gr
+00028c10: 6964 5f70 7420 696e 2078 5f76 6172 735f  id_pt in x_vars_
+00028c20: 6772 6964 3a0a 2020 2020 2020 2020 662e  grid:.        f.
+00028c30: 7772 6974 6528 277b 3a20 392e 3566 7d20  write('{: 9.5f} 
+00028c40: 272e 666f 726d 6174 2867 7269 645f 7074  '.format(grid_pt
+00028c50: 2929 0a20 2020 2020 2020 2074 6f74 616c  )).        total
+00028c60: 203d 2030 2e0a 2020 2020 2020 2020 666f   = 0..        fo
+00028c70: 7220 6c6f 676d 6f64 656c 2069 6e20 6c6f  r logmodel in lo
+00028c80: 676d 6f64 656c 733a 0a20 2020 2020 2020  gmodels:.       
+00028c90: 2020 2020 2072 6174 6520 3d20 3130 2a2a       rate = 10**
+00028ca0: 6c6f 676d 6f64 656c 2e6d 6f64 656c 280a  logmodel.model(.
+00028cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028cc0: 6c6f 676d 6f64 656c 2e66 696e 616c 5f76  logmodel.final_v
+00028cd0: 6172 5f76 616c 7565 732c 0a20 2020 2020  ar_values,.     
+00028ce0: 2020 2020 2020 2020 2020 205b 6772 6964             [grid
+00028cf0: 5f70 745d 0a20 2020 2020 2020 2020 2020  _pt].           
+00028d00: 2029 5b30 5d0a 2020 2020 2020 2020 2020   )[0].          
+00028d10: 2020 662e 7772 6974 6528 277b 3a2e 3645    f.write('{:.6E
+00028d20: 7d20 272e 666f 726d 6174 2872 6174 6529  } '.format(rate)
+00028d30: 290a 2020 2020 2020 2020 2020 2020 746f  ).            to
+00028d40: 7461 6c20 2b3d 2072 6174 650a 2020 2020  tal += rate.    
+00028d50: 2020 2020 6966 206c 656e 286c 6f67 6d6f      if len(logmo
+00028d60: 6465 6c73 2920 3e20 313a 0a20 2020 2020  dels) > 1:.     
+00028d70: 2020 2020 2020 2066 2e77 7269 7465 2827         f.write('
+00028d80: 7b3a 2e36 457d 272e 666f 726d 6174 2874  {:.6E}'.format(t
+00028d90: 6f74 616c 2929 0a20 2020 2020 2020 2066  otal)).        f
+00028da0: 2e77 7269 7465 2827 5c6e 2729 0a0a 2020  .write('\n')..  
+00028db0: 2020 6966 2076 6572 626f 7365 3a0a 2020    if verbose:.  
+00028dc0: 2020 2020 2020 7574 2e63 7072 696e 7428        ut.cprint(
+00028dd0: 0a20 2020 2020 2020 2020 2020 2027 5c6e  .            '\n
+00028de0: 2052 656c 6178 6174 696f 6e20 6d6f 6465   Relaxation mode
+00028df0: 6c20 cf84 e281 bbc2 b920 7673 207b 7d20  l ....... vs {} 
+00028e00: 7772 6974 7465 6e20 746f 205c 6e20 7b7d  written to \n {}
+00028e10: 5c6e 272e 666f 726d 6174 280a 2020 2020  \n'.format(.    
+00028e20: 2020 2020 2020 2020 2020 2020 785f 7661              x_va
+00028e30: 725f 6c61 6265 6c5b 305d 2c0a 2020 2020  r_label[0],.    
+00028e40: 2020 2020 2020 2020 2020 2020 6669 6c65              file
+00028e50: 5f6e 616d 650a 2020 2020 2020 2020 2020  _name.          
+00028e60: 2020 292c 0a20 2020 2020 2020 2020 2020    ),.           
+00028e70: 2027 6379 616e 270a 2020 2020 2020 2020   'cyan'.        
+00028e80: 290a 0a20 2020 2072 6574 7572 6e0a       )..    return.
```

### Comparing `ccfit2-5.0.0/ccfit2/stats.py` & `ccfit2-5.0.1/ccfit2/stats.py`

 * *Files identical despite different names*

### Comparing `ccfit2-5.0.0/ccfit2/utils.py` & `ccfit2-5.0.1/ccfit2/utils.py`

 * *Files identical despite different names*

### Comparing `ccfit2-5.0.0/ccfit2/waveform.py` & `ccfit2-5.0.1/ccfit2/waveform.py`

 * *Files identical despite different names*

### Comparing `ccfit2-5.0.0/ccfit2.egg-info/PKG-INFO` & `ccfit2-5.0.1/ccfit2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: ccfit2
-Version: 5.0.0
+Version: 5.0.1
 Summary: CCFIT2 is a program for fitting AC and DC magnetisation data
 Home-page: https://gitlab.com/chilton-group/cc-fit2
 Author: Daniel Reta
 Author-email: danielreta1@gmail.com
 Project-URL: Bug Tracker, https://gitlab.com/chilton-group/cc-fit2/-/issues
 Project-URL: Documentation, https://chilton-group.gitlab.io/cc-fit2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # ccfit2
 
 ccfit2 is a package for fitting AC and DC magnetisation data to obtain magnetic
 relaxation rates, and then to model the field- and/or temperature-dependence of
 these rates with parameterised models of spin-phonon coupling mechanisms.
```

### Comparing `ccfit2-5.0.0/setup.py` & `ccfit2-5.0.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import setuptools
 
 with open('README.md', 'r') as file:
     long_description = file.read()
 
 # DO NOT EDIT THIS NUMBER!
 # IT IS AUTOMATICALLY CHANGED BY python-semantic-release
-__version__ = "5.0.0"
+__version__ = "5.0.1"
 
 setuptools.setup(
     name='ccfit2',
     version=__version__,
     author='Daniel Reta',
     author_email='danielreta1@gmail.com',
     description='CCFIT2 is a program for fitting AC and DC magnetisation data', # noqa
```

