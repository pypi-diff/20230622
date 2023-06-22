# Comparing `tmp/ccfit2-5.0.1.tar.gz` & `tmp/ccfit2-5.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccfit2-5.0.1.tar", last modified: Thu Jun 22 09:00:01 2023, max compression
+gzip compressed data, was "ccfit2-5.0.2.tar", last modified: Thu Jun 22 11:15:50 2023, max compression
```

## Comparing `ccfit2-5.0.1.tar` & `ccfit2-5.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 09:00:01.312763 ccfit2-5.0.1/
--rw-rw-rw-   0 root         (0) root         (0)    35075 2023-06-22 08:59:27.000000 ccfit2-5.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1132 2023-06-22 09:00:01.312763 ccfit2-5.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      501 2023-06-22 08:59:27.000000 ccfit2-5.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 09:00:01.310763 ccfit2-5.0.1/ccfit2/
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-06-22 08:59:27.000000 ccfit2-5.0.1/ccfit2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-06-22 08:59:58.000000 ccfit2-5.0.1/ccfit2/__version__.py
--rw-rw-rw-   0 root         (0) root         (0)   132398 2023-06-22 08:59:27.000000 ccfit2-5.0.1/ccfit2/ac.py
--rw-rw-rw-   0 root         (0) root         (0)    67722 2023-06-22 08:59:27.000000 ccfit2-5.0.1/ccfit2/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    61106 2023-06-22 08:59:27.000000 ccfit2-5.0.1/ccfit2/dc.py
--rw-rw-rw-   0 root         (0) root         (0)    20395 2023-06-22 08:59:27.000000 ccfit2-5.0.1/ccfit2/gui.py
--rw-rw-rw-   0 root         (0) root         (0)   167566 2023-06-22 08:59:27.000000 ccfit2-5.0.1/ccfit2/relaxation.py
--rw-rw-rw-   0 root         (0) root         (0)     1756 2023-06-22 08:59:27.000000 ccfit2-5.0.1/ccfit2/stats.py
--rw-rw-rw-   0 root         (0) root         (0)    10668 2023-06-22 08:59:27.000000 ccfit2-5.0.1/ccfit2/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    21023 2023-06-22 08:59:27.000000 ccfit2-5.0.1/ccfit2/waveform.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 09:00:01.311763 ccfit2-5.0.1/ccfit2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1132 2023-06-22 09:00:01.000000 ccfit2-5.0.1/ccfit2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      390 2023-06-22 09:00:01.000000 ccfit2-5.0.1/ccfit2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 09:00:01.000000 ccfit2-5.0.1/ccfit2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       95 2023-06-22 09:00:01.000000 ccfit2-5.0.1/ccfit2.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      133 2023-06-22 09:00:01.000000 ccfit2-5.0.1/ccfit2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-22 09:00:01.000000 ccfit2-5.0.1/ccfit2.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      206 2023-06-22 08:59:27.000000 ccfit2-5.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 09:00:01.312763 ccfit2-5.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1544 2023-06-22 08:59:58.000000 ccfit2-5.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 11:15:50.792697 ccfit2-5.0.2/
+-rw-rw-rw-   0 root         (0) root         (0)    35075 2023-06-22 11:15:19.000000 ccfit2-5.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1132 2023-06-22 11:15:50.792697 ccfit2-5.0.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      501 2023-06-22 11:15:19.000000 ccfit2-5.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 11:15:50.791697 ccfit2-5.0.2/ccfit2/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-06-22 11:15:19.000000 ccfit2-5.0.2/ccfit2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-06-22 11:15:48.000000 ccfit2-5.0.2/ccfit2/__version__.py
+-rw-rw-rw-   0 root         (0) root         (0)   132398 2023-06-22 11:15:19.000000 ccfit2-5.0.2/ccfit2/ac.py
+-rw-rw-rw-   0 root         (0) root         (0)    69084 2023-06-22 11:15:19.000000 ccfit2-5.0.2/ccfit2/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    61106 2023-06-22 11:15:19.000000 ccfit2-5.0.2/ccfit2/dc.py
+-rw-rw-rw-   0 root         (0) root         (0)    22471 2023-06-22 11:15:19.000000 ccfit2-5.0.2/ccfit2/gui.py
+-rw-rw-rw-   0 root         (0) root         (0)   168387 2023-06-22 11:15:19.000000 ccfit2-5.0.2/ccfit2/relaxation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1756 2023-06-22 11:15:19.000000 ccfit2-5.0.2/ccfit2/stats.py
+-rw-rw-rw-   0 root         (0) root         (0)    10668 2023-06-22 11:15:19.000000 ccfit2-5.0.2/ccfit2/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    21023 2023-06-22 11:15:19.000000 ccfit2-5.0.2/ccfit2/waveform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 11:15:50.792697 ccfit2-5.0.2/ccfit2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1132 2023-06-22 11:15:50.000000 ccfit2-5.0.2/ccfit2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      390 2023-06-22 11:15:50.000000 ccfit2-5.0.2/ccfit2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 11:15:50.000000 ccfit2-5.0.2/ccfit2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       95 2023-06-22 11:15:50.000000 ccfit2-5.0.2/ccfit2.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      133 2023-06-22 11:15:50.000000 ccfit2-5.0.2/ccfit2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-22 11:15:50.000000 ccfit2-5.0.2/ccfit2.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      206 2023-06-22 11:15:19.000000 ccfit2-5.0.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 11:15:50.792697 ccfit2-5.0.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1544 2023-06-22 11:15:48.000000 ccfit2-5.0.2/setup.py
```

### Comparing `ccfit2-5.0.1/LICENSE` & `ccfit2-5.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ccfit2-5.0.1/PKG-INFO` & `ccfit2-5.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccfit2
-Version: 5.0.1
+Version: 5.0.2
 Summary: CCFIT2 is a program for fitting AC and DC magnetisation data
 Home-page: https://gitlab.com/chilton-group/cc-fit2
 Author: Daniel Reta
 Author-email: danielreta1@gmail.com
 Project-URL: Bug Tracker, https://gitlab.com/chilton-group/cc-fit2/-/issues
 Project-URL: Documentation, https://chilton-group.gitlab.io/cc-fit2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ccfit2-5.0.1/ccfit2/ac.py` & `ccfit2-5.0.2/ccfit2/ac.py`

 * *Files identical despite different names*

### Comparing `ccfit2-5.0.1/ccfit2/cli.py` & `ccfit2-5.0.2/ccfit2/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
                         experiment.rep_temperature,
                         np.min(experiment.raw_temperatures),
                         np.max(experiment.raw_temperatures),
                         experiment.raw_temperatures
                     )
                 )
                 print('{} Frequencies: {}\n'.format(
-                    len(experiment.ac_freq), experiment.ac_freq)
+                    len(experiment.ac_freqs), experiment.ac_freqs)
                 )
 
     # Manual selection of temperatures to fit
     if uargs.select_T:
         all_experiments_sep = [
             ac.interactive_t_select(experiments)
             for experiments in all_experiments_sep
@@ -1087,28 +1087,44 @@
     # plots are made
     app = QtWidgets.QApplication([])
 
     # Use glob to expand wildcards if on windows
     if 'nt' in os.name and '*' in uargs.input_files[0]:
         uargs.input_files = glob(uargs.input_files[0])
 
-    if uargs.process == 'tau_vs_T':
+    if uargs.x_var.lower() == 't':
         ut.cprint(
             '\n Fitting relaxation rate vs temperature\n',
             'black_bluebg'
         )
 
         if uargs.filetype == 'rate':
             dataset = relax.TauTDataset.from_rate_files(uargs.input_files)
         else:
             # Create dataset to store relaxation rate and temperature data
             dataset = relax.TauTDataset.from_ccfit2_files(
                 uargs.input_files
             )
 
+        # Plot rates and exit
+        if uargs.process == 'plot':
+            if uargs.plot_type in ['rate', 'both']:
+                relax.plot_rates(
+                    dataset,
+                    save=True,
+                    save_name=f'relaxation_rates{PFF}'
+                )
+            if uargs.plot_type in ['time', 'both']:
+                relax.plot_times(
+                    dataset,
+                    save=True,
+                    save_name=f'relaxation_times{PFF}'
+                )
+            sys.exit()
+
         # Disable weighting of residuals by setting uncertainties
         # as empty arrays
         if uargs.no_weights:
             dataset.lograte_pm = []
 
         # Ask user to select relaxation processes to fit, select
         # initial values, and fix parameters if desired
@@ -1164,25 +1180,41 @@
 
         fit_filename = f'relaxation_{model_names}params.out'
         model_filename = f'relaxation_{model_names}model.out'
 
         relax.write_model_params(multilogmodel, fit_filename)
         relax.write_model_data(dataset, multilogmodel, model_filename)
 
-    elif uargs.process == 'tau_vs_H':
+    elif uargs.x_var.lower() == 'h':
         ut.cprint('\n Fitting relaxation rate vs field\n', 'black_bluebg')
 
         if uargs.filetype == 'rate':
             dataset = relax.TauHDataset.from_rate_files(uargs.input_files)
         else:
             # Create dataset to store relaxation rate and temperature data
             dataset = relax.TauHDataset.from_ccfit2_files(
                 uargs.input_files
             )
 
+        # Plot rates and exit
+        if uargs.process == 'plot':
+            if uargs.plot_type in ['rate', 'both']:
+                relax.plot_rates(
+                    dataset,
+                    save=True,
+                    save_name=f'relaxation_rates{PFF}'
+                )
+            if uargs.plot_type in ['time', 'both']:
+                relax.plot_times(
+                    dataset,
+                    save=True,
+                    save_name=f'relaxation_times{PFF}'
+                )
+            sys.exit()
+
         if uargs.no_weights:
             dataset.lograte_pm = []
             dataset.rate_pm = []
 
         model_opt = [
             relax.LogFDQTMModel,
             relax.LogRamanIIModel,
@@ -2008,35 +2040,47 @@
         nargs='+',
         help=(
             'Either AC or DC <>_params.out files.'
             'See documentation for format'
         )
     )
     relaxation_parser.add_argument(
+        '--x_var',
+        metavar='<Option>',
+        choices=['T', 'H'],
+        default='T',
+        help=(
+            'Fit either the temperature (T) or field (H) dependence of '
+            'rates (isofield or isothermal).\n'
+            'Options: T, H\n'
+            'Default: T'
+        )
+    )
+    relaxation_parser.add_argument(
         '--process',
         metavar='<Option>',
-        choices=['tau_vs_T', 'tau_vs_H'],
-        default='tau_vs_T',
+        choices=['plot', 'all'],
+        default='all',
         help=(
-            'Fit either the temperature- or field-dependence of '
-            'rate (isofield or isothermal).\n'
-            'Options: tau_vs_T, tau_vs_H.\n'
-            'Default: tau_vs_T'
+            'What to do:\n'
+            ' - \'plot\' Show only raw relaxation profile\n'
+            ' - \'all\' - Fit relaxation profile\n'
+            'Default: all\n'
         )
     )
 
     relaxation_parser.add_argument(
         '--filetype',
         metavar='<Option>',
         choices=['ccfit2', 'rate'],
         default='ccfit2',
         help=(
-            'Type of file to read, either'
-            'ccfit2 *_params.out file\n'
-            'or rates file (see docs)\n'
+            'Type of file to read. Options:\n'
+            ' - ccfit2 *_params.out file\n'
+            ' - rates file (see docs)\n'
             'Default: ccfit2'
         )
     )
 
     relaxation_parser.add_argument(
         '--no_weights',
         action='store_true',
@@ -2052,26 +2096,26 @@
     relaxation_parser.add_argument(
         '--plot_type',
         metavar='<Option>',
         choices=['rate', 'time', 'both'],
         default='rate',
         help=(
             'Type of final relaxation plot to produce\n'
-            ' - \'rate\' rate vs T or H on a log-log plot\n'
+            ' - \'rate\' rate vs T or H on a log-log or log-symlog plot\n'
             ' - \'time\' ln(time) vs 1/T or 1/H on a lin-lin plot\n'
             ' - \'both\' produce both of the above\n'
             'Default: rate'
         )
     )
 
     # If argument list is none, then call function func
     # which is assigned to help function
     # read sub-parser
     parser.set_defaults(func=lambda args: parser.print_help())
-    known_args, unknown_args = parser.parse_known_args(arg_list)
+    known_args = parser.parse_args(arg_list)
 
     known_args.func(known_args)
 
     return known_args
 
 
 def main():
```

### Comparing `ccfit2-5.0.1/ccfit2/dc.py` & `ccfit2-5.0.2/ccfit2/dc.py`

 * *Files identical despite different names*

### Comparing `ccfit2-5.0.1/ccfit2/gui.py` & `ccfit2-5.0.2/ccfit2/gui.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 from matplotlib.widgets import RadioButtons
 import matplotlib.cm as cm
 from matplotlib.colorbar import Colorbar
 import matplotlib.colors as mpl_col
 from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg
 from matplotlib.figure import Figure
 import matplotlib.gridspec as gridspec
-from matplotlib.ticker import NullFormatter, FormatStrFormatter, LogLocator
+from matplotlib.ticker import NullFormatter, FormatStrFormatter, LogLocator, \
+                              SymmetricalLogLocator, FuncFormatter
 
 import numpy as np
 import sys
 
 from qtpy import QtWidgets, QtCore
 import pyqtgraph as pg
 
@@ -70,108 +71,108 @@
             'valinit': 0.1,
             'step': 0.01,
             'decimals': 4
         }
     },
     'FD-QTM': {
         'Q': {
-            'min': -6.,
-            'max': 6.,
+            'min': -30.,
+            'max': 30.,
             'valinit': 0.1,
             'step': 0.01,
             'decimals': 4
         },
         'Q_H': {
-            'min': -6.,
-            'max': 6.,
+            'min': -30.,
+            'max': 30.,
             'valinit': 0.1,
             'step': 0.01,
             'decimals': 4
         },
         'p': {
-            'min': -6.,
-            'max': 6.,
+            'min': -30.,
+            'max': 30.,
             'valinit': 0.1,
             'step': 0.01,
             'decimals': 4
         }
     },
     'Raman-II': {
         'C': {
-            'min': -6.,
-            'max': 6.,
+            'min': -30.,
+            'max': 30.,
             'valinit': 0.1,
             'step': 0.01,
             'decimals': 4
         },
         'm': {
-            'min': -6.,
-            'max': 6.,
+            'min': -30.,
+            'max': 30.,
             'valinit': 0.1,
             'step': 0.01,
             'decimals': 4
         }
     },
     'Constant': {
         'Ct': {
-            'min': -6.,
-            'max': 6.,
+            'min': -30.,
+            'max': 10.,
             'valinit': 0.1,
             'step': 0.01,
             'decimals': 4
         }
     },
     'Brons-Van-Vleck * Raman-II': {
         'e': {
-            'min': -6.,
-            'max': 6.,
+            'min': -30.,
+            'max': 30.,
             'valinit': 0.1,
             'step': 0.01,
             'decimals': 4
         },
         'f': {
-            'min': -6.,
-            'max': 6.,
+            'min': -30.,
+            'max': 30.,
             'valinit': 0.1,
             'step': 0.01,
             'decimals': 4
         },
         'C': {
-            'min': -6.,
-            'max': 6.,
+            'min': -30.,
+            'max': 30.,
             'valinit': 0.1,
             'step': 0.01,
             'decimals': 4
         },
         'm': {
-            'min': -6.,
-            'max': 6.,
+            'min': -30.,
+            'max': 30.,
             'valinit': 0.1,
             'step': 0.01,
             'decimals': 4
         },
     },
     'Brons-Van-Vleck * Constant': {
         'e': {
-            'min': -6.,
-            'max': 6.,
+            'min': -30.,
+            'max': 30.,
             'valinit': 0.1,
             'step': 0.01,
             'decimals': 4
         },
         'f': {
-            'min': -6.,
-            'max': 6.,
+            'min': -30.,
+            'max': 30.,
             'valinit': 0.1,
             'step': 0.01,
             'decimals': 4
         },
         'Ct': {
-            'min': -6.,
-            'max': 6.,
+            'min': -30.,
+            'max': 30.,
             'valinit': 0.1,
             'step': 0.01,
             'decimals': 4
         }
     }
 }
 
@@ -256,17 +257,49 @@
         y_lower = y_upper / 10
     if np.isnan(y_upper):
         y_upper = y_lower / 10
 
     return y_lower, y_upper
 
 
+def calc_linthresh(x_vals: list[float]):
+    '''
+    Calculates linthresh for symlog scale using field values.
+    Valid only for rate/time versus field plots
+
+    Parameters
+    ----------
+    x_vals: list[float]
+        Field values in Oe
+
+    Returns
+    -------
+    float
+        linthresh for symlog scale
+    '''
+
+    # All values < 1, calculate new threshold
+    if all(val <= 1 for val in x_vals):
+        linthresh = 10**np.floor(np.log10(np.max(x_vals)-0.00001))
+    # Some values < 1, find smallest value >= 1 and use this as threshold
+    elif any(val < 1 for val in x_vals):
+        it = np.argmin(x_vals[np.where(x_vals > 1)])
+        linthresh = 10**np.floor(
+            np.log10(x_vals[np.where(x_vals > 1)][it]-0.00001)
+        )
+    else:
+        linthresh = 1.
+
+    return linthresh
+
+
 def format_rate_x_y_axes(ax: plt.Axes, rates: list[float],
                          x_vals: list[float],
-                         rate_err: list[float] = []) -> None:
+                         rate_err: list[float] = [],
+                         x_type: str = 'temperature') -> None:
     '''
     Wrapper for calc_y_rate_lims and set_rate_xtick_formatting
     Formats both axes of a rate vs T or H plot
 
     Parameters
     ----------
     ax: plt.Axes
@@ -274,57 +307,85 @@
     rates: list[float]
         Relaxation rates in s^-1
     x_vals: list[float]
         x values of plot (T or H)
     rate_err: list[float], default []
         Error on rates, upper then lower one per rate.\n
         Shape (n_rates, 2)
+    x_type: str, {'field', 'temperature'}
+        Type of data, temperature (T) or field (H)
 
     Returns
     -------
     None
     '''
 
     y_lower, y_upper = calc_y_rate_lims(rates, rate_err)
 
     ax.set_ylim([y_lower, y_upper])
 
-    set_rate_xtick_formatting(ax, x_vals)
+    set_rate_xtick_formatting(ax, x_vals, x_type=x_type)
 
     # Enable minor log ticks
-    ax.yaxis.set_minor_locator(LogLocator(base=10, subs='auto'))
+    if x_type == 'field':
+        ax.xaxis.set_minor_locator(
+            SymmetricalLogLocator(
+                base=10,
+                subs=[1, 2, 3, 4, 5, 6, 7, 8, 9, 10],
+                linthresh=calc_linthresh(x_vals)
+            )
+        )
+    else:
+        ax.yaxis.set_minor_locator(LogLocator(base=10, subs='auto'))
 
     return
 
 
-def set_rate_xtick_formatting(ax: plt.Axes, x_vals: list[float]) -> None:
+def set_rate_xtick_formatting(ax: plt.Axes, x_vals: list[float],
+                              x_type: str = 'temperature') -> None:
     '''
     Sets x-tick formatting for rate plot. Enables minor tick labels if <1.1
     order of magnitude spanned by ticks
 
     Parameters
     ----------
     ax: plt.Axes
         Axis to modify
     x_vals: list[float]
         x values of plot (T or H)
+    x_type: str, {'field', 'temperature'}
+        Type of data, temperature (T) or field (H)
 
     Returns
     -------
     None
     '''
     x_vals = np.log10(x_vals)
-    ax.xaxis.set_major_formatter(FormatStrFormatter('%.0f'))
 
-    if np.max(x_vals) - np.min(x_vals) > 1.05:
+    if x_type == 'field':
+        # Major ticks
+        # Let matplotlib decide decimal values, but stop it
+        # converting them to 10^val notation
+        ax.xaxis.set_major_formatter(
+            FuncFormatter(lambda y, _: '{:g}'.format(y))
+        )
+        # No minor tick labels
         ax.xaxis.set_minor_formatter(NullFormatter())
-    else:
-        ax.xaxis.set_minor_formatter(FormatStrFormatter('%.0f'))
-        ax.tick_params('x', length=3.5, width=1, which='major')
-        ax.tick_params('x', length=3.5, width=1, which='minor')
+    elif x_type == 'temperature':
+        # Minor ticks
+        if np.max(x_vals) - np.min(x_vals) > 1.05:
+            # No minor ticks if > 1 and a bit decades spanned by temperature
+            ax.xaxis.set_minor_formatter(NullFormatter())
+        else:
+            # Add minor tick labels when range is small
+            # i.e. only just crosses a decade
+            # and make tick lengths equal to major ticks
+            ax.xaxis.set_minor_formatter(FormatStrFormatter('%.0f'))
+            ax.tick_params('x', length=3.5, width=1, which='major')
+            ax.tick_params('x', length=3.5, width=1, which='minor')
 
     return
 
 
 def convert_log_ticks_to_lin(ax: pg.graphicsItems.AxisItem.AxisItem,
                              logx_vals: list[float]) -> None:
     '''
```

### Comparing `ccfit2-5.0.1/ccfit2/relaxation.py` & `ccfit2-5.0.2/ccfit2/relaxation.py`

 * *Files 0% similar despite different names*

```diff
@@ -3560,6914 +3560,6966 @@
 0000de70: 2c0a 2020 2020 2020 2020 2751 5f48 272c  ,.        'Q_H',
 0000de80: 0a20 2020 2020 2020 2027 7027 0a20 2020  .        'p'.   
 0000de90: 205d 0a0a 2020 2020 233a 204d 6f64 656c   ]..    #: Model
 0000dea0: 2050 6172 616d 6574 6572 206e 616d 6520   Parameter name 
 0000deb0: 6d61 7468 6d6f 6465 2073 7472 696e 6773  mathmode strings
 0000dec0: 0a20 2020 2056 4152 4e41 4d45 535f 4d4d  .    VARNAMES_MM
 0000ded0: 203d 207b 0a20 2020 2020 2020 2027 5127   = {.        'Q'
-0000dee0: 3a20 7227 2451 5f48 2427 2c0a 2020 2020  : r'$Q_H$',.    
-0000def0: 2020 2020 2751 5f48 273a 2072 2724 5124      'Q_H': r'$Q$
+0000dee0: 3a20 7227 2451 2427 2c0a 2020 2020 2020  : r'$Q$',.      
+0000def0: 2020 2751 5f48 273a 2072 2724 515f 4824    'Q_H': r'$Q_H$
 0000df00: 272c 0a20 2020 2020 2020 2027 7027 3a20  ',.        'p': 
 0000df10: 7227 2470 2427 0a20 2020 207d 0a0a 2020  r'$p$'.    }..  
 0000df20: 2020 233a 204d 6f64 656c 2050 6172 616d    #: Model Param
 0000df30: 6574 6572 206e 616d 6520 4854 4d4c 2073  eter name HTML s
 0000df40: 7472 696e 6773 0a20 2020 2056 4152 4e41  trings.    VARNA
 0000df50: 4d45 535f 4854 4d4c 203d 207b 0a20 2020  MES_HTML = {.   
-0000df60: 2020 2020 2027 5127 3a20 2751 3c73 7562       'Q': 'Q<sub
-0000df70: 3e48 3c2f 7375 623e 272c 0a20 2020 2020  >H</sub>',.     
-0000df80: 2020 2027 515f 4827 3a20 2751 272c 0a20     'Q_H': 'Q',. 
+0000df60: 2020 2020 2027 515f 4827 3a20 2751 3c73       'Q_H': 'Q<s
+0000df70: 7562 3e48 3c2f 7375 623e 272c 0a20 2020  ub>H</sub>',.   
+0000df80: 2020 2020 2027 5127 3a20 2751 272c 0a20       'Q': 'Q',. 
 0000df90: 2020 2020 2020 2027 7027 3a20 2770 270a         'p': 'p'.
 0000dfa0: 2020 2020 7d0a 0a20 2020 2023 3a20 4d6f      }..    #: Mo
 0000dfb0: 6465 6c20 5061 7261 6d65 7465 7220 756e  del Parameter un
 0000dfc0: 6974 2073 7472 696e 6773 0a20 2020 2055  it strings.    U
 0000dfd0: 4e49 5453 203d 207b 0a20 2020 2020 2020  NITS = {.       
 0000dfe0: 2027 5127 3a20 276c 6f67 3130 5b73 5d27   'Q': 'log10[s]'
 0000dff0: 2c0a 2020 2020 2020 2020 2751 5f48 273a  ,.        'Q_H':
-0000e000: 2027 6c6f 6731 305b 7320 4f65 5e70 5d27   'log10[s Oe^p]'
-0000e010: 2c0a 2020 2020 2020 2020 2770 273a 2027  ,.        'p': '
-0000e020: 270a 2020 2020 7d0a 0a20 2020 2023 3a20  '.    }..    #: 
-0000e030: 4d6f 6465 6c20 5061 7261 6d65 7465 7220  Model Parameter 
-0000e040: 756e 6974 206d 6174 686d 6f64 6520 7374  unit mathmode st
-0000e050: 7269 6e67 730a 2020 2020 554e 4954 535f  rings.    UNITS_
-0000e060: 4d4d 203d 207b 0a20 2020 2020 2020 2027  MM = {.        '
-0000e070: 5127 3a20 7227 245c 6c6f 675f 5c6d 6174  Q': r'$\log_\mat
-0000e080: 6872 6567 756c 6172 7b31 307d 5c6c 6566  hregular{10}\lef
-0000e090: 745b 5c6d 6174 6872 6567 756c 6172 7b73  t[\mathregular{s
-0000e0a0: 7d5c 7269 6768 745d 2427 2c0a 2020 2020  }\right]$',.    
-0000e0b0: 2020 2020 2751 5f48 273a 2072 2724 5c6c      'Q_H': r'$\l
-0000e0c0: 6f67 5f5c 6d61 7468 7265 6775 6c61 727b  og_\mathregular{
-0000e0d0: 3130 7d5c 6c65 6674 5b5c 6d61 7468 7265  10}\left[\mathre
-0000e0e0: 6775 6c61 727b 737d 205c 205c 6d61 7468  gular{s} \ \math
-0000e0f0: 7265 6775 6c61 727b 4f65 7d5e 7b70 7d5c  regular{Oe}^{p}\
-0000e100: 7269 6768 745d 2427 2c20 2320 6e6f 7161  right]$', # noqa
-0000e110: 0a20 2020 2020 2020 2027 7027 3a20 2727  .        'p': ''
-0000e120: 0a20 2020 207d 0a0a 2020 2020 233a 204d  .    }..    #: M
-0000e130: 6f64 656c 2050 6172 616d 6574 6572 2075  odel Parameter u
-0000e140: 6e69 7420 4854 4d4c 2073 7472 696e 6773  nit HTML strings
-0000e150: 0a20 2020 2055 4e49 5453 5f48 544d 4c20  .    UNITS_HTML 
-0000e160: 3d20 7b0a 2020 2020 2020 2020 2751 273a  = {.        'Q':
-0000e170: 2072 276c 6f67 3c73 7562 3e31 303c 2f73   r'log<sub>10</s
-0000e180: 7562 3e5b 735d 272c 0a20 2020 2020 2020  ub>[s]',.       
-0000e190: 2027 515f 4827 3a20 7227 6c6f 673c 7375   'Q_H': r'log<su
-0000e1a0: 623e 3130 3c2f 7375 623e 5b73 204f 653c  b>10</sub>[s Oe<
-0000e1b0: 7375 703e 703c 2f73 7570 3e5d 272c 0a20  sup>p</sup>]',. 
-0000e1c0: 2020 2020 2020 2027 7027 3a20 2727 0a20         'p': ''. 
-0000e1d0: 2020 207d 0a0a 2020 2020 233a 204d 6f64     }..    #: Mod
-0000e1e0: 656c 2050 6172 616d 6574 6572 2062 6f75  el Parameter bou
-0000e1f0: 6e64 730a 2020 2020 424f 554e 4453 203d  nds.    BOUNDS =
-0000e200: 207b 0a20 2020 2020 2020 2027 5127 3a20   {.        'Q': 
-0000e210: 5b2d 3330 2e2c 206e 702e 696e 665d 2c0a  [-30., np.inf],.
-0000e220: 2020 2020 2020 2020 2751 5f48 273a 205b          'Q_H': [
-0000e230: 2d33 302e 2c20 6e70 2e69 6e66 5d2c 0a20  -30., np.inf],. 
-0000e240: 2020 2020 2020 2027 7027 3a20 5b30 2c20         'p': [0, 
-0000e250: 3130 5d0a 2020 2020 7d0a 0a20 2020 2040  10].    }..    @
-0000e260: 7374 6174 6963 6d65 7468 6f64 0a20 2020  staticmethod.   
-0000e270: 2064 6566 2073 6574 5f69 6e69 7469 616c   def set_initial
-0000e280: 5f76 616c 7328 7061 7261 6d5f 6469 6374  _vals(param_dict
-0000e290: 3a20 6469 6374 5b73 7472 2c20 7374 7220  : dict[str, str 
-0000e2a0: 7c20 666c 6f61 745d 2920 2d3e 2064 6963  | float]) -> dic
-0000e2b0: 745b 7374 722c 2066 6c6f 6174 5d3a 2023  t[str, float]: #
-0000e2c0: 206e 6f71 610a 2020 2020 2020 2020 2727   noqa.        ''
-0000e2d0: 270a 2020 2020 2020 2020 5365 7473 2067  '.        Sets g
-0000e2e0: 7565 7373 2076 616c 7565 7320 666f 7220  uess values for 
-0000e2f0: 7061 7261 6d65 7465 7273 2069 6620 7265  parameters if re
-0000e300: 7175 6573 7465 6420 6279 2075 7365 720a  quested by user.
-0000e310: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
-0000e320: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
-0000e330: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2070  ------.        p
-0000e340: 6172 616d 5f64 6963 743a 2064 6963 745b  aram_dict: dict[
-0000e350: 7374 722c 2073 7472 207c 2066 6c6f 6174  str, str | float
-0000e360: 5d0a 2020 2020 2020 2020 2020 2020 4b65  ].            Ke
-0000e370: 7973 2061 7265 2066 6974 2f66 6978 2070  ys are fit/fix p
-0000e380: 6172 616d 6574 6572 206e 616d 6573 2028  arameter names (
-0000e390: 7365 6520 636c 6173 732e 5041 524e 414d  see class.PARNAM
-0000e3a0: 4553 295c 6e0a 2020 2020 2020 2020 2020  ES)\n.          
-0000e3b0: 2020 5661 6c75 6573 2061 7265 2065 6974    Values are eit
-0000e3c0: 6865 7220 666c 6f61 7420 2861 6374 7561  her float (actua
-0000e3d0: 6c20 7661 6c75 6529 206f 7220 7468 6520  l value) or the 
-0000e3e0: 7374 7269 6e67 2027 6775 6573 7327 0a0a  string 'guess'..
-0000e3f0: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
-0000e400: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
-0000e410: 2020 2020 2020 2020 6469 6374 5b73 7472          dict[str
-0000e420: 2c20 666c 6f61 745d 0a20 2020 2020 2020  , float].       
-0000e430: 2020 2020 204b 6579 7320 6172 6520 6669       Keys are fi
-0000e440: 742f 6669 7820 7061 7261 6d65 7465 7220  t/fix parameter 
-0000e450: 6e61 6d65 7320 2873 6565 2063 6c61 7373  names (see class
-0000e460: 2e50 4152 4e41 4d45 5329 5c6e 0a20 2020  .PARNAMES)\n.   
-0000e470: 2020 2020 2020 2020 2056 616c 7565 7320           Values 
-0000e480: 6172 6520 666c 6f61 7420 2861 6374 7561  are float (actua
-0000e490: 6c20 7661 6c75 6529 2077 6869 6368 2061  l value) which a
-0000e4a0: 7265 2069 6e69 7469 616c 2076 616c 7565  re initial value
-0000e4b0: 7320 6f66 0a20 2020 2020 2020 2020 2020  s of.           
-0000e4c0: 2070 6172 616d 6574 6572 0a20 2020 2020   parameter.     
-0000e4d0: 2020 2027 2727 0a0a 2020 2020 2020 2020     '''..        
-0000e4e0: 2320 4d61 6b65 2063 6f70 792c 2061 6e79  # Make copy, any
-0000e4f0: 2073 7472 2076 616c 7565 7320 7769 6c6c   str values will
-0000e500: 2062 6520 7265 706c 6163 6564 0a20 2020   be replaced.   
-0000e510: 2020 2020 206e 6577 5f70 6172 616d 5f64       new_param_d
-0000e520: 6963 7420 3d20 636f 7079 2e63 6f70 7928  ict = copy.copy(
-0000e530: 7061 7261 6d5f 6469 6374 290a 0a20 2020  param_dict)..   
-0000e540: 2020 2020 2023 2047 7565 7373 6573 0a20       # Guesses. 
-0000e550: 2020 2020 2020 2067 7565 7373 6469 6374         guessdict
-0000e560: 203d 207b 0a20 2020 2020 2020 2020 2020   = {.           
-0000e570: 2027 5127 3a20 2d32 2c0a 2020 2020 2020   'Q': -2,.      
-0000e580: 2020 2020 2020 2751 5f48 273a 202d 322c        'Q_H': -2,
-0000e590: 0a20 2020 2020 2020 2020 2020 2027 7027  .            'p'
-0000e5a0: 3a20 320a 2020 2020 2020 2020 7d0a 0a20  : 2.        }.. 
-0000e5b0: 2020 2020 2020 2023 2052 6570 6c61 6365         # Replace
-0000e5c0: 2027 6775 6573 7327 2077 6974 6820 7265   'guess' with re
-0000e5d0: 6c65 7661 6e74 2067 7565 7373 0a20 2020  levant guess.   
-0000e5e0: 2020 2020 2066 6f72 2076 6172 2c20 7661       for var, va
-0000e5f0: 6c20 696e 2070 6172 616d 5f64 6963 742e  l in param_dict.
-0000e600: 6974 656d 7328 293a 0a20 2020 2020 2020  items():.       
-0000e610: 2020 2020 2069 6620 7661 6c20 3d3d 2027       if val == '
-0000e620: 6775 6573 7327 3a0a 2020 2020 2020 2020  guess':.        
-0000e630: 2020 2020 2020 2020 6e65 775f 7061 7261          new_para
-0000e640: 6d5f 6469 6374 5b76 6172 5d20 3d20 6775  m_dict[var] = gu
-0000e650: 6573 7364 6963 745b 7661 725d 0a0a 2020  essdict[var]..  
-0000e660: 2020 2020 2020 7265 7475 726e 206e 6577        return new
-0000e670: 5f70 6172 616d 5f64 6963 740a 0a20 2020  _param_dict..   
-0000e680: 2040 7374 6174 6963 6d65 7468 6f64 0a20   @staticmethod. 
-0000e690: 2020 2064 6566 206d 6f64 656c 2870 6172     def model(par
-0000e6a0: 616d 6574 6572 733a 2064 6963 745b 7374  ameters: dict[st
-0000e6b0: 722c 2066 6c6f 6174 5d2c 0a20 2020 2020  r, float],.     
-0000e6c0: 2020 2020 2020 2020 2066 6965 6c64 733a           fields:
-0000e6d0: 206e 7074 2e41 7272 6179 4c69 6b65 2920   npt.ArrayLike) 
-0000e6e0: 2d3e 206e 7074 2e4e 4441 7272 6179 3a0a  -> npt.NDArray:.
-0000e6f0: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
-0000e700: 2020 2020 4576 616c 7561 7465 7320 6c6f      Evaluates lo
-0000e710: 6731 3028 4644 2d51 544d 2920 6d6f 6465  g10(FD-QTM) mode
-0000e720: 6c20 6f66 206c 6f67 3130 2872 656c 6178  l of log10(relax
-0000e730: 6174 696f 6e20 7261 7465 290a 2020 2020  ation rate).    
-0000e740: 2020 2020 7573 696e 6720 7072 6f76 6964      using provid
-0000e750: 6564 2070 6172 616d 6574 6572 2061 6e64  ed parameter and
-0000e760: 2066 6965 6c64 2076 616c 7565 732e 0a0a   field values...
-0000e770: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-0000e780: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
-0000e790: 2d2d 2d2d 2d0a 2020 2020 2020 2020 7061  -----.        pa
-0000e7a0: 7261 6d65 7465 7273 3a20 6469 6374 5b73  rameters: dict[s
-0000e7b0: 7472 2c20 666c 6f61 745d 0a20 2020 2020  tr, float].     
-0000e7c0: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
-0000e7d0: 7320 746f 2075 7365 2069 6e20 6d6f 6465  s to use in mode
-0000e7e0: 6c20 6675 6e63 7469 6f6e 2c20 6b65 7973  l function, keys
-0000e7f0: 2061 7265 2067 6976 656e 2069 6e0a 2020   are given in.  
-0000e800: 2020 2020 2020 2020 2020 636c 6173 732e            class.
-0000e810: 5041 524e 414d 4553 0a20 2020 2020 2020  PARNAMES.       
-0000e820: 2066 6965 6c64 733a 2061 7272 6179 5f6c   fields: array_l
-0000e830: 696b 650a 2020 2020 2020 2020 2020 2020  ike.            
-0000e840: 6669 656c 6420 7661 6c75 6573 2028 4f65  field values (Oe
-0000e850: 2920 6174 2077 6869 6368 206d 6f64 656c  ) at which model
-0000e860: 2066 756e 6374 696f 6e20 6973 2065 7661   function is eva
-0000e870: 6c75 6174 6564 0a0a 2020 2020 2020 2020  luated..        
-0000e880: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
-0000e890: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-0000e8a0: 6e64 6172 7261 7920 6f66 2066 6c6f 6174  ndarray of float
-0000e8b0: 730a 2020 2020 2020 2020 2020 2020 6c6f  s.            lo
-0000e8c0: 6731 3028 5265 6c61 7861 7469 6f6e 2072  g10(Relaxation r
-0000e8d0: 6174 6529 2061 7320 6120 6675 6e63 7469  ate) as a functi
-0000e8e0: 6f6e 206f 6620 6669 656c 640a 0a20 2020  on of field..   
-0000e8f0: 2020 2020 2027 2727 0a0a 2020 2020 2020       '''..      
-0000e900: 2020 7120 3d20 7061 7261 6d65 7465 7273    q = parameters
-0000e910: 5b27 5127 5d0a 2020 2020 2020 2020 7168  ['Q'].        qh
-0000e920: 203d 2070 6172 616d 6574 6572 735b 2751   = parameters['Q
-0000e930: 5f48 275d 0a20 2020 2020 2020 2070 203d  _H'].        p =
-0000e940: 2070 6172 616d 6574 6572 735b 2770 275d   parameters['p']
-0000e950: 0a0a 2020 2020 2020 2020 6c6f 6772 6174  ..        lograt
-0000e960: 6520 3d20 6e70 2e6c 6f67 3130 2831 302a  e = np.log10(10*
-0000e970: 2a2d 7120 2f20 2831 202b 2031 302a 2a2d  *-q / (1 + 10**-
-0000e980: 7168 202a 206e 702e 6173 6172 7261 7928  qh * np.asarray(
-0000e990: 6669 656c 6473 292a 2a70 2929 0a0a 2020  fields)**p))..  
-0000e9a0: 2020 2020 2020 7265 7475 726e 206c 6f67        return log
-0000e9b0: 7261 7465 0a0a 0a63 6c61 7373 204c 6f67  rate...class Log
-0000e9c0: 5261 6d61 6e49 494d 6f64 656c 284c 6f67  RamanIIModel(Log
-0000e9d0: 5461 7548 4d6f 6465 6c29 3a0a 2020 2020  TauHModel):.    
-0000e9e0: 2727 270a 2020 2020 4c6f 6728 5261 6d61  '''.    Log(Rama
-0000e9f0: 6e2d 4949 2920 4d6f 6465 6c20 6f66 206c  n-II) Model of l
-0000ea00: 6f67 3130 2852 656c 6178 6174 696f 6e20  og10(Relaxation 
-0000ea10: 7261 7465 2920 7673 2066 6965 6c64 0a20  rate) vs field. 
-0000ea20: 2020 2027 2727 0a0a 2020 2020 233a 204d     '''..    #: M
-0000ea30: 6f64 656c 206e 616d 650a 2020 2020 4e41  odel name.    NA
-0000ea40: 4d45 203d 2027 5261 6d61 6e2d 4949 270a  ME = 'Raman-II'.
-0000ea50: 0a20 2020 2023 3a20 4d6f 6465 6c20 6e61  .    #: Model na
-0000ea60: 6d65 2077 6974 6820 6c6f 6720 6272 6163  me with log brac
-0000ea70: 6b65 7473 0a20 2020 204c 4e41 4d45 203d  kets.    LNAME =
-0000ea80: 2027 4c6f 6728 5261 6d61 6e2d 4949 2927   'Log(Raman-II)'
-0000ea90: 0a0a 2020 2020 233a 204d 6f64 656c 2050  ..    #: Model P
-0000eaa0: 6172 616d 6574 6572 206e 616d 6520 7374  arameter name st
-0000eab0: 7269 6e67 730a 2020 2020 5041 524e 414d  rings.    PARNAM
-0000eac0: 4553 203d 205b 0a20 2020 2020 2020 2027  ES = [.        '
-0000ead0: 4327 2c0a 2020 2020 2020 2020 276d 272c  C',.        'm',
-0000eae0: 0a20 2020 205d 0a0a 2020 2020 233a 204d  .    ]..    #: M
-0000eaf0: 6f64 656c 2050 6172 616d 6574 6572 206e  odel Parameter n
-0000eb00: 616d 6520 6d61 7468 6d6f 6465 2073 7472  ame mathmode str
-0000eb10: 696e 6773 0a20 2020 2056 4152 4e41 4d45  ings.    VARNAME
-0000eb20: 535f 4d4d 203d 207b 0a20 2020 2020 2020  S_MM = {.       
-0000eb30: 2027 4327 3a20 2724 4324 272c 0a20 2020   'C': '$C$',.   
-0000eb40: 2020 2020 2027 6d27 3a20 2724 6d24 270a       'm': '$m$'.
-0000eb50: 2020 2020 7d0a 0a20 2020 2023 3a20 4d6f      }..    #: Mo
-0000eb60: 6465 6c20 5061 7261 6d65 7465 7220 6e61  del Parameter na
-0000eb70: 6d65 2048 544d 4c20 7374 7269 6e67 730a  me HTML strings.
-0000eb80: 2020 2020 5641 524e 414d 4553 5f48 544d      VARNAMES_HTM
-0000eb90: 4c20 3d20 7b0a 2020 2020 2020 2020 2743  L = {.        'C
-0000eba0: 273a 2027 4327 2c0a 2020 2020 2020 2020  ': 'C',.        
-0000ebb0: 276d 273a 2027 6d27 0a20 2020 207d 0a0a  'm': 'm'.    }..
-0000ebc0: 2020 2020 233a 204d 6f64 656c 2050 6172      #: Model Par
-0000ebd0: 616d 6574 6572 2075 6e69 7420 7374 7269  ameter unit stri
-0000ebe0: 6e67 730a 2020 2020 554e 4954 5320 3d20  ngs.    UNITS = 
-0000ebf0: 7b0a 2020 2020 2020 2020 2743 273a 2027  {.        'C': '
-0000ec00: 6c6f 6731 305b 4f65 5e2d 7020 735e 2d31  log10[Oe^-p s^-1
-0000ec10: 5d27 2c0a 2020 2020 2020 2020 276d 273a  ]',.        'm':
-0000ec20: 2027 270a 2020 2020 7d0a 0a20 2020 2023   ''.    }..    #
-0000ec30: 3a20 4d6f 6465 6c20 5061 7261 6d65 7465  : Model Paramete
-0000ec40: 7220 756e 6974 206d 6174 686d 6f64 6520  r unit mathmode 
-0000ec50: 7374 7269 6e67 730a 2020 2020 554e 4954  strings.    UNIT
-0000ec60: 535f 4d4d 203d 207b 0a20 2020 2020 2020  S_MM = {.       
-0000ec70: 2027 4327 3a20 7227 245c 6c6f 675f 5c6d   'C': r'$\log_\m
-0000ec80: 6174 6872 6567 756c 6172 7b31 307d 5c6c  athregular{10}\l
-0000ec90: 6566 745b 5c6d 6174 6872 6567 756c 6172  eft[\mathregular
-0000eca0: 7b4f 657d 5e7b 2d6d 7d20 5c20 5c6d 6174  {Oe}^{-m} \ \mat
-0000ecb0: 6872 6567 756c 6172 7b73 7d5e 5c6d 6174  hregular{s}^\mat
-0000ecc0: 6872 6567 756c 6172 7b2d 317d 5c72 6967  hregular{-1}\rig
-0000ecd0: 6874 5d24 272c 2023 206e 6f71 610a 2020  ht]$', # noqa.  
-0000ece0: 2020 2020 2020 276d 273a 2027 270a 2020        'm': ''.  
-0000ecf0: 2020 7d0a 0a20 2020 2023 3a20 4d6f 6465    }..    #: Mode
-0000ed00: 6c20 5061 7261 6d65 7465 7220 6e61 6d65  l Parameter name
-0000ed10: 2048 544d 4c20 7374 7269 6e67 730a 2020   HTML strings.  
-0000ed20: 2020 554e 4954 535f 4854 4d4c 203d 207b    UNITS_HTML = {
-0000ed30: 0a20 2020 2020 2020 2027 4327 3a20 7227  .        'C': r'
-0000ed40: 6c6f 673c 7375 623e 3130 3c2f 7375 623e  log<sub>10</sub>
-0000ed50: 5b4f 653c 7375 703e 2d6d 3c2f 7375 703e  [Oe<sup>-m</sup>
-0000ed60: 2073 3c73 7570 3e2d 313c 2f73 7570 3e5d   s<sup>-1</sup>]
-0000ed70: 272c 0a20 2020 2020 2020 2027 6d27 3a20  ',.        'm': 
-0000ed80: 2727 0a20 2020 207d 0a0a 2020 2020 233a  ''.    }..    #:
-0000ed90: 204d 6f64 656c 2050 6172 616d 6574 6572   Model Parameter
-0000eda0: 2062 6f75 6e64 730a 2020 2020 424f 554e   bounds.    BOUN
-0000edb0: 4453 203d 207b 0a20 2020 2020 2020 2027  DS = {.        '
-0000edc0: 4327 3a20 5b2d 3330 2c20 6e70 2e69 6e66  C': [-30, np.inf
-0000edd0: 5d2c 0a20 2020 2020 2020 2027 6d27 3a20  ],.        'm': 
-0000ede0: 5b2d 3330 2c20 6e70 2e69 6e66 5d2c 0a20  [-30, np.inf],. 
-0000edf0: 2020 207d 0a0a 2020 2020 4073 7461 7469     }..    @stati
-0000ee00: 636d 6574 686f 640a 2020 2020 6465 6620  cmethod.    def 
-0000ee10: 7365 745f 696e 6974 6961 6c5f 7661 6c73  set_initial_vals
-0000ee20: 2870 6172 616d 5f64 6963 743a 2064 6963  (param_dict: dic
-0000ee30: 745b 7374 722c 2073 7472 207c 2066 6c6f  t[str, str | flo
-0000ee40: 6174 5d29 202d 3e20 6469 6374 5b73 7472  at]) -> dict[str
-0000ee50: 2c20 666c 6f61 745d 3a20 2320 6e6f 7161  , float]: # noqa
-0000ee60: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
-0000ee70: 2020 2020 2053 6574 7320 6775 6573 7320       Sets guess 
-0000ee80: 7661 6c75 6573 2066 6f72 2070 6172 616d  values for param
-0000ee90: 6574 6572 7320 6966 2072 6571 7565 7374  eters if request
-0000eea0: 6564 2062 7920 7573 6572 0a0a 2020 2020  ed by user..    
-0000eeb0: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-0000eec0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
-0000eed0: 2d0a 2020 2020 2020 2020 7061 7261 6d5f  -.        param_
-0000eee0: 6469 6374 3a20 6469 6374 5b73 7472 2c20  dict: dict[str, 
-0000eef0: 7374 7220 7c20 666c 6f61 745d 0a20 2020  str | float].   
-0000ef00: 2020 2020 2020 2020 204b 6579 7320 6172           Keys ar
-0000ef10: 6520 6669 742f 6669 7820 7061 7261 6d65  e fit/fix parame
-0000ef20: 7465 7220 6e61 6d65 7320 2873 6565 2063  ter names (see c
-0000ef30: 6c61 7373 2e50 4152 4e41 4d45 5329 5c6e  lass.PARNAMES)\n
-0000ef40: 0a20 2020 2020 2020 2020 2020 2056 616c  .            Val
-0000ef50: 7565 7320 6172 6520 6569 7468 6572 2066  ues are either f
-0000ef60: 6c6f 6174 2028 6163 7475 616c 2076 616c  loat (actual val
-0000ef70: 7565 2920 6f72 2074 6865 2073 7472 696e  ue) or the strin
-0000ef80: 6720 2767 7565 7373 270a 0a20 2020 2020  g 'guess'..     
-0000ef90: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
-0000efa0: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
-0000efb0: 2020 2064 6963 745b 7374 722c 2066 6c6f     dict[str, flo
-0000efc0: 6174 5d0a 2020 2020 2020 2020 2020 2020  at].            
-0000efd0: 4b65 7973 2061 7265 2066 6974 2f66 6978  Keys are fit/fix
-0000efe0: 2070 6172 616d 6574 6572 206e 616d 6573   parameter names
-0000eff0: 2028 7365 6520 636c 6173 732e 5041 524e   (see class.PARN
-0000f000: 414d 4553 295c 6e0a 2020 2020 2020 2020  AMES)\n.        
-0000f010: 2020 2020 5661 6c75 6573 2061 7265 2066      Values are f
-0000f020: 6c6f 6174 2028 6163 7475 616c 2076 616c  loat (actual val
-0000f030: 7565 2920 7768 6963 6820 6172 6520 696e  ue) which are in
-0000f040: 6974 6961 6c20 7661 6c75 6573 206f 660a  itial values of.
-0000f050: 2020 2020 2020 2020 2020 2020 7061 7261              para
-0000f060: 6d65 7465 720a 2020 2020 2020 2020 2727  meter.        ''
-0000f070: 270a 0a20 2020 2020 2020 2023 204d 616b  '..        # Mak
-0000f080: 6520 636f 7079 2c20 616e 7920 7374 7220  e copy, any str 
-0000f090: 7661 6c75 6573 2077 696c 6c20 6265 2072  values will be r
-0000f0a0: 6570 6c61 6365 640a 2020 2020 2020 2020  eplaced.        
-0000f0b0: 6e65 775f 7061 7261 6d5f 6469 6374 203d  new_param_dict =
-0000f0c0: 2063 6f70 792e 636f 7079 2870 6172 616d   copy.copy(param
-0000f0d0: 5f64 6963 7429 0a0a 2020 2020 2020 2020  _dict)..        
-0000f0e0: 2320 4775 6573 7365 730a 2020 2020 2020  # Guesses.      
-0000f0f0: 2020 6775 6573 7364 6963 7420 3d20 7b0a    guessdict = {.
-0000f100: 2020 2020 2020 2020 2020 2020 2743 273a              'C':
-0000f110: 202d 342c 0a20 2020 2020 2020 2020 2020   -4,.           
-0000f120: 2027 6d27 3a20 340a 2020 2020 2020 2020   'm': 4.        
-0000f130: 7d0a 0a20 2020 2020 2020 2023 2052 6570  }..        # Rep
-0000f140: 6c61 6365 2027 6775 6573 7327 2077 6974  lace 'guess' wit
-0000f150: 6820 7265 6c65 7661 6e74 2067 7565 7373  h relevant guess
-0000f160: 0a20 2020 2020 2020 2066 6f72 2076 6172  .        for var
-0000f170: 2c20 7661 6c20 696e 2070 6172 616d 5f64  , val in param_d
-0000f180: 6963 742e 6974 656d 7328 293a 0a20 2020  ict.items():.   
-0000f190: 2020 2020 2020 2020 2069 6620 7661 6c20           if val 
-0000f1a0: 3d3d 2027 6775 6573 7327 3a0a 2020 2020  == 'guess':.    
-0000f1b0: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
-0000f1c0: 7061 7261 6d5f 6469 6374 5b76 6172 5d20  param_dict[var] 
-0000f1d0: 3d20 6775 6573 7364 6963 745b 7661 725d  = guessdict[var]
-0000f1e0: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-0000f1f0: 206e 6577 5f70 6172 616d 5f64 6963 740a   new_param_dict.
-0000f200: 0a20 2020 2040 7374 6174 6963 6d65 7468  .    @staticmeth
-0000f210: 6f64 0a20 2020 2064 6566 206d 6f64 656c  od.    def model
-0000f220: 2870 6172 616d 6574 6572 733a 2064 6963  (parameters: dic
-0000f230: 745b 7374 722c 2066 6c6f 6174 5d2c 0a20  t[str, float],. 
-0000f240: 2020 2020 2020 2020 2020 2020 2066 6965               fie
-0000f250: 6c64 733a 206e 7074 2e41 7272 6179 4c69  lds: npt.ArrayLi
-0000f260: 6b65 2920 2d3e 206e 7074 2e4e 4441 7272  ke) -> npt.NDArr
-0000f270: 6179 3a0a 2020 2020 2020 2020 2727 270a  ay:.        '''.
-0000f280: 2020 2020 2020 2020 4576 616c 7561 7465          Evaluate
-0000f290: 7320 6c6f 6731 3028 5261 6d61 6e2d 4949  s log10(Raman-II
-0000f2a0: 2920 6d6f 6465 6c20 6f66 206c 6f67 3130  ) model of log10
-0000f2b0: 2872 656c 6178 6174 696f 6e20 7261 7465  (relaxation rate
-0000f2c0: 290a 2020 2020 2020 2020 7573 696e 6720  ).        using 
-0000f2d0: 7072 6f76 6964 6564 2070 6172 616d 6574  provided paramet
-0000f2e0: 6572 2061 6e64 2066 6965 6c64 2076 616c  er and field val
-0000f2f0: 7565 732e 0a0a 2020 2020 2020 2020 5061  ues...        Pa
-0000f300: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
-0000f310: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-0000f320: 2020 2020 7061 7261 6d65 7465 7273 3a20      parameters: 
-0000f330: 6469 6374 5b73 7472 2c20 666c 6f61 745d  dict[str, float]
-0000f340: 0a20 2020 2020 2020 2020 2020 2050 6172  .            Par
-0000f350: 616d 6574 6572 7320 746f 2075 7365 2069  ameters to use i
-0000f360: 6e20 6d6f 6465 6c20 6675 6e63 7469 6f6e  n model function
-0000f370: 2c20 6b65 7973 2061 7265 2067 6976 656e  , keys are given
-0000f380: 2069 6e0a 2020 2020 2020 2020 2020 2020   in.            
-0000f390: 636c 6173 732e 5041 524e 414d 4553 0a20  class.PARNAMES. 
-0000f3a0: 2020 2020 2020 2066 6965 6c64 733a 2061         fields: a
-0000f3b0: 7272 6179 5f6c 696b 650a 2020 2020 2020  rray_like.      
-0000f3c0: 2020 2020 2020 6669 656c 6420 7661 6c75        field valu
-0000f3d0: 6573 2028 4f65 2920 6174 2077 6869 6368  es (Oe) at which
-0000f3e0: 206d 6f64 656c 2066 756e 6374 696f 6e20   model function 
-0000f3f0: 6973 2065 7661 6c75 6174 6564 0a0a 2020  is evaluated..  
-0000f400: 2020 2020 2020 5265 7475 726e 730a 2020        Returns.  
-0000f410: 2020 2020 2020 2d2d 2d2d 2d2d 2d0a 2020        -------.  
-0000f420: 2020 2020 2020 6e64 6172 7261 7920 6f66        ndarray of
-0000f430: 2066 6c6f 6174 730a 2020 2020 2020 2020   floats.        
-0000f440: 2020 2020 6c6f 6731 3028 5265 6c61 7861      log10(Relaxa
-0000f450: 7469 6f6e 2072 6174 6529 2061 7320 6120  tion rate) as a 
-0000f460: 6675 6e63 7469 6f6e 206f 6620 6669 656c  function of fiel
-0000f470: 640a 0a20 2020 2020 2020 2027 2727 0a0a  d..        '''..
-0000f480: 2020 2020 2020 2020 6320 3d20 7061 7261          c = para
-0000f490: 6d65 7465 7273 5b27 4327 5d0a 2020 2020  meters['C'].    
-0000f4a0: 2020 2020 6d20 3d20 7061 7261 6d65 7465      m = paramete
-0000f4b0: 7273 5b27 6d27 5d0a 0a20 2020 2020 2020  rs['m']..       
-0000f4c0: 206c 6f67 7261 7465 203d 206e 702e 6c6f   lograte = np.lo
-0000f4d0: 6731 3028 3130 2a2a 6320 2a20 6e70 2e61  g10(10**c * np.a
-0000f4e0: 7361 7272 6179 2866 6965 6c64 7329 2a2a  sarray(fields)**
-0000f4f0: 6d29 0a0a 2020 2020 2020 2020 7265 7475  m)..        retu
-0000f500: 726e 206c 6f67 7261 7465 0a0a 0a63 6c61  rn lograte...cla
-0000f510: 7373 204c 6f67 436f 6e73 7461 6e74 4d6f  ss LogConstantMo
-0000f520: 6465 6c28 4c6f 6754 6175 484d 6f64 656c  del(LogTauHModel
-0000f530: 293a 0a20 2020 2027 2727 0a20 2020 204c  ):.    '''.    L
-0000f540: 6f67 2843 6f6e 7374 616e 7429 204d 6f64  og(Constant) Mod
-0000f550: 656c 206f 6620 6c6f 6731 3028 5265 6c61  el of log10(Rela
-0000f560: 7861 7469 6f6e 2072 6174 6529 2076 7320  xation rate) vs 
-0000f570: 6669 656c 640a 2020 2020 2727 270a 0a20  field.    '''.. 
-0000f580: 2020 2023 3a20 4d6f 6465 6c20 6e61 6d65     #: Model name
-0000f590: 0a20 2020 204e 414d 4520 3d20 2743 6f6e  .    NAME = 'Con
-0000f5a0: 7374 616e 7427 0a0a 2020 2020 233a 204d  stant'..    #: M
-0000f5b0: 6f64 656c 206e 616d 6520 7769 7468 206c  odel name with l
-0000f5c0: 6f67 2062 7261 636b 6574 730a 2020 2020  og brackets.    
-0000f5d0: 4c4e 414d 4520 3d20 274c 6f67 2843 6f6e  LNAME = 'Log(Con
-0000f5e0: 7374 616e 7429 270a 0a20 2020 2023 3a20  stant)'..    #: 
-0000f5f0: 4d6f 6465 6c20 5061 7261 6d65 7465 7220  Model Parameter 
-0000f600: 6e61 6d65 2073 7472 696e 6773 0a20 2020  name strings.   
-0000f610: 2050 4152 4e41 4d45 5320 3d20 5b0a 2020   PARNAMES = [.  
-0000f620: 2020 2020 2020 2743 7427 2c0a 2020 2020        'Ct',.    
-0000f630: 5d0a 0a20 2020 2023 3a20 4d6f 6465 6c20  ]..    #: Model 
-0000f640: 5061 7261 6d65 7465 7220 6e61 6d65 206d  Parameter name m
-0000f650: 6174 686d 6f64 6520 7374 7269 6e67 730a  athmode strings.
-0000f660: 2020 2020 5641 524e 414d 4553 5f4d 4d20      VARNAMES_MM 
-0000f670: 3d20 7b0a 2020 2020 2020 2020 2743 7427  = {.        'Ct'
-0000f680: 3a20 7227 2443 7424 272c 0a20 2020 207d  : r'$Ct$',.    }
-0000f690: 0a0a 2020 2020 233a 204d 6f64 656c 2050  ..    #: Model P
-0000f6a0: 6172 616d 6574 6572 206e 616d 6520 4854  arameter name HT
-0000f6b0: 4d4c 2073 7472 696e 6773 0a20 2020 2056  ML strings.    V
-0000f6c0: 4152 4e41 4d45 535f 4854 4d4c 203d 207b  ARNAMES_HTML = {
-0000f6d0: 0a20 2020 2020 2020 2027 4374 273a 2027  .        'Ct': '
-0000f6e0: 4374 270a 2020 2020 7d0a 0a20 2020 2023  Ct'.    }..    #
-0000f6f0: 3a20 4d6f 6465 6c20 5061 7261 6d65 7465  : Model Paramete
-0000f700: 7220 756e 6974 2073 7472 696e 6773 0a20  r unit strings. 
-0000f710: 2020 2055 4e49 5453 203d 207b 0a20 2020     UNITS = {.   
-0000f720: 2020 2020 2027 4374 273a 2027 6c6f 6731       'Ct': 'log1
-0000f730: 305b 735e 2d31 5d27 0a20 2020 207d 0a0a  0[s^-1]'.    }..
-0000f740: 2020 2020 233a 204d 6f64 656c 2050 6172      #: Model Par
-0000f750: 616d 6574 6572 2075 6e69 7420 6d61 7468  ameter unit math
-0000f760: 6d6f 6465 2073 7472 696e 6773 0a20 2020  mode strings.   
-0000f770: 2055 4e49 5453 5f4d 4d20 3d20 7b0a 2020   UNITS_MM = {.  
-0000f780: 2020 2020 2020 2743 7427 3a20 7227 245c        'Ct': r'$\
-0000f790: 6c6f 675f 5c6d 6174 6872 6567 756c 6172  log_\mathregular
-0000f7a0: 7b31 307d 5c6c 6566 745b 5c6d 6174 6872  {10}\left[\mathr
-0000f7b0: 6567 756c 6172 7b73 7d5e 5c6d 6174 6872  egular{s}^\mathr
-0000f7c0: 6567 756c 6172 7b2d 317d 5c72 6967 6874  egular{-1}\right
-0000f7d0: 5d24 272c 2023 206e 6f71 610a 2020 2020  ]$', # noqa.    
-0000f7e0: 7d0a 0a20 2020 2023 3a20 4d6f 6465 6c20  }..    #: Model 
-0000f7f0: 5061 7261 6d65 7465 7220 756e 6974 2048  Parameter unit H
-0000f800: 544d 4c20 7374 7269 6e67 730a 2020 2020  TML strings.    
-0000f810: 554e 4954 535f 4854 4d4c 203d 207b 0a20  UNITS_HTML = {. 
-0000f820: 2020 2020 2020 2027 4374 273a 2072 276c         'Ct': r'l
-0000f830: 6f67 3c73 7562 3e31 303c 2f73 7562 3e5b  og<sub>10</sub>[
-0000f840: 733c 7375 703e 2d31 3c2f 7375 703e 5d27  s<sup>-1</sup>]'
-0000f850: 0a20 2020 207d 0a0a 2020 2020 233a 204d  .    }..    #: M
-0000f860: 6f64 656c 2070 6172 616d 6574 6572 2062  odel parameter b
-0000f870: 6f75 6e64 730a 2020 2020 424f 554e 4453  ounds.    BOUNDS
-0000f880: 203d 207b 0a20 2020 2020 2020 2027 4374   = {.        'Ct
-0000f890: 273a 205b 2d33 302c 2031 305d 2c0a 2020  ': [-30, 10],.  
-0000f8a0: 2020 7d0a 0a20 2020 2040 7374 6174 6963    }..    @static
-0000f8b0: 6d65 7468 6f64 0a20 2020 2064 6566 2073  method.    def s
-0000f8c0: 6574 5f69 6e69 7469 616c 5f76 616c 7328  et_initial_vals(
-0000f8d0: 7061 7261 6d5f 6469 6374 3a20 6469 6374  param_dict: dict
-0000f8e0: 5b73 7472 2c20 7374 7220 7c20 666c 6f61  [str, str | floa
-0000f8f0: 745d 2920 2d3e 2064 6963 745b 7374 722c  t]) -> dict[str,
-0000f900: 2066 6c6f 6174 5d3a 2023 206e 6f71 610a   float]: # noqa.
-0000f910: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
-0000f920: 2020 2020 5365 7473 2067 7565 7373 2076      Sets guess v
-0000f930: 616c 7565 7320 666f 7220 7061 7261 6d65  alues for parame
-0000f940: 7465 7273 2069 6620 7265 7175 6573 7465  ters if requeste
-0000f950: 6420 6279 2075 7365 720a 0a20 2020 2020  d by user..     
-0000f960: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
-0000f970: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
-0000f980: 0a20 2020 2020 2020 2070 6172 616d 5f64  .        param_d
-0000f990: 6963 743a 2064 6963 745b 7374 722c 2073  ict: dict[str, s
-0000f9a0: 7472 207c 2066 6c6f 6174 5d0a 2020 2020  tr | float].    
-0000f9b0: 2020 2020 2020 2020 4b65 7973 2061 7265          Keys are
-0000f9c0: 2066 6974 2f66 6978 2070 6172 616d 6574   fit/fix paramet
-0000f9d0: 6572 206e 616d 6573 2028 7365 6520 636c  er names (see cl
-0000f9e0: 6173 732e 5041 524e 414d 4553 295c 6e0a  ass.PARNAMES)\n.
-0000f9f0: 2020 2020 2020 2020 2020 2020 5661 6c75              Valu
-0000fa00: 6573 2061 7265 2065 6974 6865 7220 666c  es are either fl
-0000fa10: 6f61 7420 2861 6374 7561 6c20 7661 6c75  oat (actual valu
-0000fa20: 6529 206f 7220 7468 6520 7374 7269 6e67  e) or the string
-0000fa30: 2027 6775 6573 7327 0a0a 2020 2020 2020   'guess'..      
-0000fa40: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
-0000fa50: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
-0000fa60: 2020 6469 6374 5b73 7472 2c20 666c 6f61    dict[str, floa
-0000fa70: 745d 0a20 2020 2020 2020 2020 2020 204b  t].            K
-0000fa80: 6579 7320 6172 6520 6669 742f 6669 7820  eys are fit/fix 
-0000fa90: 7061 7261 6d65 7465 7220 6e61 6d65 7320  parameter names 
-0000faa0: 2873 6565 2063 6c61 7373 2e50 4152 4e41  (see class.PARNA
-0000fab0: 4d45 5329 5c6e 0a20 2020 2020 2020 2020  MES)\n.         
-0000fac0: 2020 2056 616c 7565 7320 6172 6520 666c     Values are fl
-0000fad0: 6f61 7420 2861 6374 7561 6c20 7661 6c75  oat (actual valu
-0000fae0: 6529 2077 6869 6368 2061 7265 2069 6e69  e) which are ini
-0000faf0: 7469 616c 2076 616c 7565 7320 6f66 0a20  tial values of. 
-0000fb00: 2020 2020 2020 2020 2020 2070 6172 616d             param
-0000fb10: 6574 6572 0a20 2020 2020 2020 2027 2727  eter.        '''
-0000fb20: 0a0a 2020 2020 2020 2020 2320 4d61 6b65  ..        # Make
-0000fb30: 2063 6f70 792c 2061 6e79 2073 7472 2076   copy, any str v
-0000fb40: 616c 7565 7320 7769 6c6c 2062 6520 7265  alues will be re
-0000fb50: 706c 6163 6564 0a20 2020 2020 2020 206e  placed.        n
-0000fb60: 6577 5f70 6172 616d 5f64 6963 7420 3d20  ew_param_dict = 
-0000fb70: 636f 7079 2e63 6f70 7928 7061 7261 6d5f  copy.copy(param_
-0000fb80: 6469 6374 290a 0a20 2020 2020 2020 2023  dict)..        #
-0000fb90: 2047 7565 7373 6573 0a20 2020 2020 2020   Guesses.       
-0000fba0: 2067 7565 7373 6469 6374 203d 207b 0a20   guessdict = {. 
-0000fbb0: 2020 2020 2020 2020 2020 2027 4374 273a             'Ct':
-0000fbc0: 202d 340a 2020 2020 2020 2020 7d0a 0a20   -4.        }.. 
-0000fbd0: 2020 2020 2020 2023 2052 6570 6c61 6365         # Replace
-0000fbe0: 2027 6775 6573 7327 2077 6974 6820 7265   'guess' with re
-0000fbf0: 6c65 7661 6e74 2067 7565 7373 0a20 2020  levant guess.   
-0000fc00: 2020 2020 2066 6f72 2076 6172 2c20 7661       for var, va
-0000fc10: 6c20 696e 2070 6172 616d 5f64 6963 742e  l in param_dict.
-0000fc20: 6974 656d 7328 293a 0a20 2020 2020 2020  items():.       
-0000fc30: 2020 2020 2069 6620 7661 6c20 3d3d 2027       if val == '
-0000fc40: 6775 6573 7327 3a0a 2020 2020 2020 2020  guess':.        
-0000fc50: 2020 2020 2020 2020 6e65 775f 7061 7261          new_para
-0000fc60: 6d5f 6469 6374 5b76 6172 5d20 3d20 6775  m_dict[var] = gu
-0000fc70: 6573 7364 6963 745b 7661 725d 0a0a 2020  essdict[var]..  
-0000fc80: 2020 2020 2020 7265 7475 726e 206e 6577        return new
-0000fc90: 5f70 6172 616d 5f64 6963 740a 0a20 2020  _param_dict..   
-0000fca0: 2040 7374 6174 6963 6d65 7468 6f64 0a20   @staticmethod. 
-0000fcb0: 2020 2064 6566 206d 6f64 656c 2870 6172     def model(par
-0000fcc0: 616d 6574 6572 733a 2064 6963 745b 7374  ameters: dict[st
-0000fcd0: 722c 2066 6c6f 6174 5d2c 0a20 2020 2020  r, float],.     
-0000fce0: 2020 2020 2020 2020 2066 6965 6c64 733a           fields:
-0000fcf0: 206e 7074 2e41 7272 6179 4c69 6b65 2920   npt.ArrayLike) 
-0000fd00: 2d3e 206e 7074 2e4e 4441 7272 6179 3a0a  -> npt.NDArray:.
-0000fd10: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
-0000fd20: 2020 2020 4576 616c 7561 7465 7320 6c6f      Evaluates lo
-0000fd30: 6731 3028 436f 6e73 7461 6e74 2920 6d6f  g10(Constant) mo
-0000fd40: 6465 6c20 6f66 206c 6f67 3130 2872 656c  del of log10(rel
-0000fd50: 6178 6174 696f 6e20 7261 7465 290a 2020  axation rate).  
-0000fd60: 2020 2020 2020 7573 696e 6720 7072 6f76        using prov
-0000fd70: 6964 6564 2070 6172 616d 6574 6572 2061  ided parameter a
-0000fd80: 6e64 2066 6965 6c64 2076 616c 7565 732e  nd field values.
-0000fd90: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
-0000fda0: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
-0000fdb0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-0000fdc0: 7061 7261 6d65 7465 7273 3a20 6469 6374  parameters: dict
-0000fdd0: 5b73 7472 2c20 666c 6f61 745d 0a20 2020  [str, float].   
-0000fde0: 2020 2020 2020 2020 2050 6172 616d 6574           Paramet
-0000fdf0: 6572 7320 746f 2075 7365 2069 6e20 6d6f  ers to use in mo
-0000fe00: 6465 6c20 6675 6e63 7469 6f6e 2c20 6b65  del function, ke
-0000fe10: 7973 2061 7265 2067 6976 656e 2069 6e0a  ys are given in.
-0000fe20: 2020 2020 2020 2020 2020 2020 636c 6173              clas
-0000fe30: 732e 5041 524e 414d 4553 0a20 2020 2020  s.PARNAMES.     
-0000fe40: 2020 2066 6965 6c64 733a 2061 7272 6179     fields: array
-0000fe50: 5f6c 696b 650a 2020 2020 2020 2020 2020  _like.          
-0000fe60: 2020 6669 656c 6420 7661 6c75 6573 2028    field values (
-0000fe70: 4f65 2920 6174 2077 6869 6368 206d 6f64  Oe) at which mod
-0000fe80: 656c 2066 756e 6374 696f 6e20 6973 2065  el function is e
-0000fe90: 7661 6c75 6174 6564 0a0a 2020 2020 2020  valuated..      
-0000fea0: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
-0000feb0: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
-0000fec0: 2020 6e64 6172 7261 7920 6f66 2066 6c6f    ndarray of flo
-0000fed0: 6174 730a 2020 2020 2020 2020 2020 2020  ats.            
-0000fee0: 6c6f 6731 3028 5265 6c61 7861 7469 6f6e  log10(Relaxation
-0000fef0: 2072 6174 6529 2061 7320 6120 6675 6e63   rate) as a func
-0000ff00: 7469 6f6e 206f 6620 6669 656c 640a 0a20  tion of field.. 
-0000ff10: 2020 2020 2020 2027 2727 0a0a 2020 2020         '''..    
-0000ff20: 2020 2020 6374 203d 2070 6172 616d 6574      ct = paramet
-0000ff30: 6572 735b 2743 7427 5d0a 0a20 2020 2020  ers['Ct']..     
-0000ff40: 2020 206c 6f67 7261 7465 203d 206e 702e     lograte = np.
-0000ff50: 7a65 726f 7328 6c65 6e28 6669 656c 6473  zeros(len(fields
-0000ff60: 2929 202b 206e 702e 6c6f 6731 3028 3130  )) + np.log10(10
-0000ff70: 2a2a 6374 290a 0a20 2020 2020 2020 2072  **ct)..        r
-0000ff80: 6574 7572 6e20 6c6f 6772 6174 650a 0a0a  eturn lograte...
-0000ff90: 636c 6173 7320 4c6f 6742 5656 5261 6d61  class LogBVVRama
-0000ffa0: 6e49 494d 6f64 656c 284c 6f67 5461 7548  nIIModel(LogTauH
-0000ffb0: 4d6f 6465 6c29 3a0a 2020 2020 2727 270a  Model):.    '''.
-0000ffc0: 2020 2020 4c6f 6728 4272 6f6e 732d 5661      Log(Brons-Va
-0000ffd0: 6e2d 566c 6563 6b20 2a20 5261 6d61 6e2d  n-Vleck * Raman-
-0000ffe0: 4949 2920 4d6f 6465 6c20 6f66 206c 6f67  II) Model of log
-0000fff0: 3130 2852 656c 6178 6174 696f 6e20 7261  10(Relaxation ra
-00010000: 7465 2920 7673 2066 6965 6c64 0a20 2020  te) vs field.   
-00010010: 2027 2727 0a0a 2020 2020 233a 204d 6f64   '''..    #: Mod
-00010020: 656c 206e 616d 650a 2020 2020 4e41 4d45  el name.    NAME
-00010030: 203d 2027 4272 6f6e 732d 5661 6e2d 566c   = 'Brons-Van-Vl
-00010040: 6563 6b20 2a20 5261 6d61 6e2d 4949 270a  eck * Raman-II'.
-00010050: 0a20 2020 2023 3a20 4d6f 6465 6c20 6e61  .    #: Model na
-00010060: 6d65 2077 6974 6820 6c6f 6720 6272 6163  me with log brac
-00010070: 6b65 7473 0a20 2020 204c 4e41 4d45 203d  kets.    LNAME =
-00010080: 2027 4c6f 6728 4272 6f6e 732d 5661 6e2d   'Log(Brons-Van-
-00010090: 566c 6563 6b20 2a20 5261 6d61 6e2d 4949  Vleck * Raman-II
-000100a0: 2927 0a0a 2020 2020 233a 204d 6f64 656c  )'..    #: Model
-000100b0: 2050 6172 616d 6574 6572 206e 616d 6520   Parameter name 
-000100c0: 7374 7269 6e67 730a 2020 2020 5041 524e  strings.    PARN
-000100d0: 414d 4553 203d 205b 0a20 2020 2020 2020  AMES = [.       
-000100e0: 2027 6527 2c0a 2020 2020 2020 2020 2766   'e',.        'f
-000100f0: 272c 0a20 2020 2020 2020 2027 4327 2c0a  ',.        'C',.
-00010100: 2020 2020 2020 2020 276d 270a 2020 2020          'm'.    
-00010110: 5d0a 0a20 2020 2023 3a20 4d6f 6465 6c20  ]..    #: Model 
-00010120: 5061 7261 6d65 7465 7220 6e61 6d65 206d  Parameter name m
-00010130: 6174 686d 6f64 6520 7374 7269 6e67 730a  athmode strings.
-00010140: 2020 2020 5641 524e 414d 4553 5f4d 4d20      VARNAMES_MM 
-00010150: 3d20 7b0a 2020 2020 2020 2020 2765 273a  = {.        'e':
-00010160: 2072 2724 6524 272c 0a20 2020 2020 2020   r'$e$',.       
-00010170: 2027 6627 3a20 7227 2466 2427 2c0a 2020   'f': r'$f$',.  
-00010180: 2020 2020 2020 2743 273a 2072 2724 4324        'C': r'$C$
-00010190: 272c 0a20 2020 2020 2020 2027 6d27 3a20  ',.        'm': 
-000101a0: 7227 246d 2427 2c0a 2020 2020 7d0a 0a20  r'$m$',.    }.. 
-000101b0: 2020 2023 3a20 4d6f 6465 6c20 5061 7261     #: Model Para
-000101c0: 6d65 7465 7220 6e61 6d65 2048 544d 4c20  meter name HTML 
-000101d0: 7374 7269 6e67 730a 2020 2020 5641 524e  strings.    VARN
-000101e0: 414d 4553 5f48 544d 4c20 3d20 7b0a 2020  AMES_HTML = {.  
-000101f0: 2020 2020 2020 2765 273a 2027 6527 2c0a        'e': 'e',.
-00010200: 2020 2020 2020 2020 2766 273a 2027 6627          'f': 'f'
-00010210: 2c0a 2020 2020 2020 2020 2743 273a 2027  ,.        'C': '
-00010220: 4327 2c0a 2020 2020 2020 2020 276d 273a  C',.        'm':
-00010230: 2027 6d27 0a20 2020 207d 0a0a 2020 2020   'm'.    }..    
-00010240: 233a 204d 6f64 656c 2050 6172 616d 6574  #: Model Paramet
-00010250: 6572 2075 6e69 7420 7374 7269 6e67 730a  er unit strings.
-00010260: 2020 2020 554e 4954 5320 3d20 7b0a 2020      UNITS = {.  
-00010270: 2020 2020 2020 2765 273a 2027 6c6f 6731        'e': 'log1
-00010280: 305b 4f65 5e2d 325d 272c 0a20 2020 2020  0[Oe^-2]',.     
-00010290: 2020 2027 6627 3a20 276c 6f67 3130 5b4f     'f': 'log10[O
-000102a0: 655e 2d32 5d27 2c0a 2020 2020 2020 2020  e^-2]',.        
-000102b0: 2743 273a 2027 6c6f 6731 305b 735e 2d31  'C': 'log10[s^-1
-000102c0: 204f 655e 2d6d 5d27 2c0a 2020 2020 2020   Oe^-m]',.      
-000102d0: 2020 276d 273a 2027 270a 2020 2020 7d0a    'm': ''.    }.
-000102e0: 0a20 2020 2023 3a20 4d6f 6465 6c20 5061  .    #: Model Pa
-000102f0: 7261 6d65 7465 7220 756e 6974 206d 6174  rameter unit mat
-00010300: 686d 6f64 6520 7374 7269 6e67 730a 2020  hmode strings.  
-00010310: 2020 554e 4954 535f 4d4d 203d 207b 0a20    UNITS_MM = {. 
-00010320: 2020 2020 2020 2027 6527 3a20 7227 245c         'e': r'$\
-00010330: 6c6f 675f 5c6d 6174 6872 6567 756c 6172  log_\mathregular
-00010340: 7b31 307d 5c6c 6566 745b 5c6d 6174 6872  {10}\left[\mathr
-00010350: 6567 756c 6172 7b4f 657d 5e5c 6d61 7468  egular{Oe}^\math
-00010360: 7265 6775 6c61 727b 2d32 7d5c 7269 6768  regular{-2}\righ
-00010370: 745d 2427 2c20 2320 6e6f 7161 0a20 2020  t]$', # noqa.   
-00010380: 2020 2020 2027 6627 3a20 7227 245c 6c6f       'f': r'$\lo
-00010390: 675f 5c6d 6174 6872 6567 756c 6172 7b31  g_\mathregular{1
-000103a0: 307d 5c6c 6566 745b 5c6d 6174 6872 6567  0}\left[\mathreg
-000103b0: 756c 6172 7b4f 657d 5e5c 6d61 7468 7265  ular{Oe}^\mathre
-000103c0: 6775 6c61 727b 2d32 7d5c 7269 6768 745d  gular{-2}\right]
-000103d0: 2427 2c20 2320 6e6f 7161 0a20 2020 2020  $', # noqa.     
-000103e0: 2020 2027 4327 3a20 7227 245c 6c6f 675f     'C': r'$\log_
-000103f0: 5c6d 6174 6872 6567 756c 6172 7b31 307d  \mathregular{10}
-00010400: 5c6c 6566 745b 5c6d 6174 6872 6567 756c  \left[\mathregul
-00010410: 6172 7b73 7d5e 5c6d 6174 6872 6567 756c  ar{s}^\mathregul
-00010420: 6172 7b2d 317d 205c 6d61 7468 7265 6775  ar{-1} \mathregu
-00010430: 6c61 727b 4f65 7d5e 5c6d 6174 6872 6567  lar{Oe}^\mathreg
-00010440: 756c 6172 7b2d 327d 5c72 6967 6874 5d24  ular{-2}\right]$
-00010450: 272c 2023 206e 6f71 610a 2020 2020 2020  ', # noqa.      
-00010460: 2020 276d 273a 2027 270a 2020 2020 7d0a    'm': ''.    }.
-00010470: 0a20 2020 2023 3a20 4d6f 6465 6c20 5061  .    #: Model Pa
-00010480: 7261 6d65 7465 7220 756e 6974 2048 544d  rameter unit HTM
-00010490: 4c20 7374 7269 6e67 730a 2020 2020 554e  L strings.    UN
-000104a0: 4954 535f 4854 4d4c 203d 207b 0a20 2020  ITS_HTML = {.   
-000104b0: 2020 2020 2027 6527 3a20 7227 6c6f 673c       'e': r'log<
-000104c0: 7375 623e 3130 3c2f 7375 623e 5b4f 653c  sub>10</sub>[Oe<
-000104d0: 7375 703e 2d32 3c2f 7375 703e 5d27 2c0a  sup>-2</sup>]',.
-000104e0: 2020 2020 2020 2020 2766 273a 2072 276c          'f': r'l
-000104f0: 6f67 3c73 7562 3e31 303c 2f73 7562 3e5b  og<sub>10</sub>[
-00010500: 4f65 3c73 7570 3e2d 323c 2f73 7570 3e5d  Oe<sup>-2</sup>]
-00010510: 272c 0a20 2020 2020 2020 2027 4327 3a20  ',.        'C': 
-00010520: 7227 6c6f 673c 7375 623e 3130 3c2f 7375  r'log<sub>10</su
-00010530: 623e 5b73 3c73 7570 3e2d 313c 2f73 7570  b>[s<sup>-1</sup
-00010540: 3e20 4f65 3c73 7570 3e2d 6d3c 2f73 7570  > Oe<sup>-m</sup
-00010550: 3e5d 272c 0a20 2020 2020 2020 2027 6d27  >]',.        'm'
-00010560: 3a20 2727 0a20 2020 207d 0a0a 2020 2020  : ''.    }..    
-00010570: 233a 204d 6f64 656c 2070 6172 616d 6574  #: Model paramet
-00010580: 6572 2062 6f75 6e64 730a 2020 2020 424f  er bounds.    BO
-00010590: 554e 4453 203d 207b 0a20 2020 2020 2020  UNDS = {.       
-000105a0: 2027 6527 3a20 5b2d 3330 2c20 6e70 2e69   'e': [-30, np.i
-000105b0: 6e66 5d2c 0a20 2020 2020 2020 2027 6627  nf],.        'f'
-000105c0: 3a20 5b2d 3330 2c20 6e70 2e69 6e66 5d2c  : [-30, np.inf],
-000105d0: 0a20 2020 2020 2020 2027 4327 3a20 5b2d  .        'C': [-
-000105e0: 3330 2c20 6e70 2e69 6e66 5d2c 0a20 2020  30, np.inf],.   
-000105f0: 2020 2020 2027 6d27 3a20 5b30 2c20 3130       'm': [0, 10
-00010600: 5d2c 0a20 2020 207d 0a0a 2020 2020 4073  ],.    }..    @s
-00010610: 7461 7469 636d 6574 686f 640a 2020 2020  taticmethod.    
-00010620: 6465 6620 7365 745f 696e 6974 6961 6c5f  def set_initial_
-00010630: 7661 6c73 2870 6172 616d 5f64 6963 743a  vals(param_dict:
-00010640: 2064 6963 745b 7374 722c 2073 7472 207c   dict[str, str |
-00010650: 2066 6c6f 6174 5d29 202d 3e20 6469 6374   float]) -> dict
-00010660: 5b73 7472 2c20 666c 6f61 745d 3a20 2320  [str, float]: # 
-00010670: 6e6f 7161 0a20 2020 2020 2020 2027 2727  noqa.        '''
-00010680: 0a20 2020 2020 2020 2053 6574 7320 6775  .        Sets gu
-00010690: 6573 7320 7661 6c75 6573 2066 6f72 2070  ess values for p
-000106a0: 6172 616d 6574 6572 7320 6966 2072 6571  arameters if req
-000106b0: 7565 7374 6564 2062 7920 7573 6572 0a0a  uested by user..
-000106c0: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-000106d0: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
-000106e0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 7061  -----.        pa
-000106f0: 7261 6d5f 6469 6374 3a20 6469 6374 5b73  ram_dict: dict[s
-00010700: 7472 2c20 7374 7220 7c20 666c 6f61 745d  tr, str | float]
-00010710: 0a20 2020 2020 2020 2020 2020 204b 6579  .            Key
-00010720: 7320 6172 6520 6669 742f 6669 7820 7061  s are fit/fix pa
-00010730: 7261 6d65 7465 7220 6e61 6d65 7320 2873  rameter names (s
-00010740: 6565 2063 6c61 7373 2e50 4152 4e41 4d45  ee class.PARNAME
-00010750: 5329 5c6e 0a20 2020 2020 2020 2020 2020  S)\n.           
-00010760: 2056 616c 7565 7320 6172 6520 6569 7468   Values are eith
-00010770: 6572 2066 6c6f 6174 2028 6163 7475 616c  er float (actual
-00010780: 2076 616c 7565 2920 6f72 2074 6865 2073   value) or the s
-00010790: 7472 696e 6720 2767 7565 7373 270a 0a20  tring 'guess'.. 
-000107a0: 2020 2020 2020 2052 6574 7572 6e73 0a20         Returns. 
-000107b0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0a20         -------. 
-000107c0: 2020 2020 2020 2064 6963 745b 7374 722c         dict[str,
-000107d0: 2066 6c6f 6174 5d0a 2020 2020 2020 2020   float].        
-000107e0: 2020 2020 4b65 7973 2061 7265 2066 6974      Keys are fit
-000107f0: 2f66 6978 2070 6172 616d 6574 6572 206e  /fix parameter n
-00010800: 616d 6573 2028 7365 6520 636c 6173 732e  ames (see class.
-00010810: 5041 524e 414d 4553 295c 6e0a 2020 2020  PARNAMES)\n.    
-00010820: 2020 2020 2020 2020 5661 6c75 6573 2061          Values a
-00010830: 7265 2066 6c6f 6174 2028 6163 7475 616c  re float (actual
-00010840: 2076 616c 7565 2920 7768 6963 6820 6172   value) which ar
-00010850: 6520 696e 6974 6961 6c20 7661 6c75 6573  e initial values
-00010860: 206f 660a 2020 2020 2020 2020 2020 2020   of.            
-00010870: 7061 7261 6d65 7465 720a 2020 2020 2020  parameter.      
-00010880: 2020 2727 270a 0a20 2020 2020 2020 2023    '''..        #
-00010890: 204d 616b 6520 636f 7079 2c20 616e 7920   Make copy, any 
-000108a0: 7374 7220 7661 6c75 6573 2077 696c 6c20  str values will 
-000108b0: 6265 2072 6570 6c61 6365 640a 2020 2020  be replaced.    
-000108c0: 2020 2020 6e65 775f 7061 7261 6d5f 6469      new_param_di
-000108d0: 6374 203d 2063 6f70 792e 636f 7079 2870  ct = copy.copy(p
-000108e0: 6172 616d 5f64 6963 7429 0a0a 2020 2020  aram_dict)..    
-000108f0: 2020 2020 2320 4775 6573 7365 730a 2020      # Guesses.  
-00010900: 2020 2020 2020 6775 6573 7364 6963 7420        guessdict 
-00010910: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
-00010920: 2765 273a 202d 352e 2c0a 2020 2020 2020  'e': -5.,.      
-00010930: 2020 2020 2020 2766 273a 202d 352e 2c0a        'f': -5.,.
-00010940: 2020 2020 2020 2020 2020 2020 2743 273a              'C':
-00010950: 202d 342c 0a20 2020 2020 2020 2020 2020   -4,.           
-00010960: 2027 6d27 3a20 342e 0a20 2020 2020 2020   'm': 4..       
-00010970: 207d 0a0a 2020 2020 2020 2020 2320 5265   }..        # Re
-00010980: 706c 6163 6520 2767 7565 7373 2720 7769  place 'guess' wi
-00010990: 7468 2072 656c 6576 616e 7420 6775 6573  th relevant gues
-000109a0: 730a 2020 2020 2020 2020 666f 7220 7661  s.        for va
-000109b0: 722c 2076 616c 2069 6e20 7061 7261 6d5f  r, val in param_
-000109c0: 6469 6374 2e69 7465 6d73 2829 3a0a 2020  dict.items():.  
-000109d0: 2020 2020 2020 2020 2020 6966 2076 616c            if val
-000109e0: 203d 3d20 2767 7565 7373 273a 0a20 2020   == 'guess':.   
-000109f0: 2020 2020 2020 2020 2020 2020 206e 6577               new
-00010a00: 5f70 6172 616d 5f64 6963 745b 7661 725d  _param_dict[var]
-00010a10: 203d 2067 7565 7373 6469 6374 5b76 6172   = guessdict[var
-00010a20: 5d0a 0a20 2020 2020 2020 2072 6574 7572  ]..        retur
-00010a30: 6e20 6e65 775f 7061 7261 6d5f 6469 6374  n new_param_dict
-00010a40: 0a0a 2020 2020 4073 7461 7469 636d 6574  ..    @staticmet
-00010a50: 686f 640a 2020 2020 6465 6620 6d6f 6465  hod.    def mode
-00010a60: 6c28 7061 7261 6d65 7465 7273 3a20 6469  l(parameters: di
-00010a70: 6374 5b73 7472 2c20 666c 6f61 745d 2c0a  ct[str, float],.
-00010a80: 2020 2020 2020 2020 2020 2020 2020 6669                fi
-00010a90: 656c 6473 3a20 6e70 742e 4172 7261 794c  elds: npt.ArrayL
-00010aa0: 696b 6529 202d 3e20 6e70 742e 4e44 4172  ike) -> npt.NDAr
-00010ab0: 7261 793a 0a20 2020 2020 2020 2027 2727  ray:.        '''
-00010ac0: 0a20 2020 2020 2020 2045 7661 6c75 6174  .        Evaluat
-00010ad0: 6573 206c 6f67 3130 2852 616d 616e 2d49  es log10(Raman-I
-00010ae0: 4929 206d 6f64 656c 206f 6620 6c6f 6731  I) model of log1
-00010af0: 3028 7265 6c61 7861 7469 6f6e 2072 6174  0(relaxation rat
-00010b00: 6529 0a20 2020 2020 2020 2075 7369 6e67  e).        using
-00010b10: 2070 726f 7669 6465 6420 7061 7261 6d65   provided parame
-00010b20: 7465 7220 616e 6420 6669 656c 6420 7661  ter and field va
-00010b30: 6c75 6573 2e0a 0a20 2020 2020 2020 2050  lues...        P
-00010b40: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
-00010b50: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-00010b60: 2020 2020 2070 6172 616d 6574 6572 733a       parameters:
-00010b70: 2064 6963 745b 7374 722c 2066 6c6f 6174   dict[str, float
-00010b80: 5d0a 2020 2020 2020 2020 2020 2020 5061  ].            Pa
-00010b90: 7261 6d65 7465 7273 2074 6f20 7573 6520  rameters to use 
-00010ba0: 696e 206d 6f64 656c 2066 756e 6374 696f  in model functio
-00010bb0: 6e2c 206b 6579 7320 6172 6520 6769 7665  n, keys are give
-00010bc0: 6e20 696e 0a20 2020 2020 2020 2020 2020  n in.           
-00010bd0: 2063 6c61 7373 2e50 4152 4e41 4d45 530a   class.PARNAMES.
-00010be0: 2020 2020 2020 2020 6669 656c 6473 3a20          fields: 
-00010bf0: 6172 7261 795f 6c69 6b65 0a20 2020 2020  array_like.     
-00010c00: 2020 2020 2020 2066 6965 6c64 2076 616c         field val
-00010c10: 7565 7320 284f 6529 2061 7420 7768 6963  ues (Oe) at whic
-00010c20: 6820 6d6f 6465 6c20 6675 6e63 7469 6f6e  h model function
-00010c30: 2069 7320 6576 616c 7561 7465 640a 0a20   is evaluated.. 
-00010c40: 2020 2020 2020 2052 6574 7572 6e73 0a20         Returns. 
-00010c50: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0a20         -------. 
-00010c60: 2020 2020 2020 206e 6461 7272 6179 206f         ndarray o
-00010c70: 6620 666c 6f61 7473 0a20 2020 2020 2020  f floats.       
-00010c80: 2020 2020 206c 6f67 3130 2852 656c 6178       log10(Relax
-00010c90: 6174 696f 6e20 7261 7465 2920 6173 2061  ation rate) as a
-00010ca0: 2066 756e 6374 696f 6e20 6f66 2066 6965   function of fie
-00010cb0: 6c64 0a0a 2020 2020 2020 2020 2727 270a  ld..        '''.
-00010cc0: 0a20 2020 2020 2020 2065 203d 2070 6172  .        e = par
-00010cd0: 616d 6574 6572 735b 2765 275d 0a20 2020  ameters['e'].   
-00010ce0: 2020 2020 2066 203d 2070 6172 616d 6574       f = paramet
-00010cf0: 6572 735b 2766 275d 0a20 2020 2020 2020  ers['f'].       
-00010d00: 2043 203d 2070 6172 616d 6574 6572 735b   C = parameters[
-00010d10: 2743 275d 0a20 2020 2020 2020 206d 203d  'C'].        m =
-00010d20: 2070 6172 616d 6574 6572 735b 276d 275d   parameters['m']
-00010d30: 0a0a 2020 2020 2020 2020 6c6f 6772 6174  ..        lograt
-00010d40: 6520 3d20 6e70 2e6c 6f67 3130 280a 2020  e = np.log10(.  
-00010d50: 2020 2020 2020 2020 2020 2831 302a 2a43            (10**C
-00010d60: 202a 206e 702e 6173 6172 7261 7928 6669   * np.asarray(fi
-00010d70: 656c 6473 292a 2a6d 2920 2a20 2831 202b  elds)**m) * (1 +
-00010d80: 2031 302a 2a65 202a 206e 702e 6173 6172   10**e * np.asar
-00010d90: 7261 7928 6669 656c 6473 292a 2a32 292f  ray(fields)**2)/
-00010da0: 2831 202b 2031 302a 2a66 202a 206e 702e  (1 + 10**f * np.
-00010db0: 6173 6172 7261 7928 6669 656c 6473 292a  asarray(fields)*
-00010dc0: 2a32 2920 2320 6e6f 7161 0a20 2020 2020  *2) # noqa.     
-00010dd0: 2020 2029 0a0a 2020 2020 2020 2020 7265     )..        re
-00010de0: 7475 726e 206c 6f67 7261 7465 0a0a 0a63  turn lograte...c
-00010df0: 6c61 7373 204c 6f67 4256 5643 6f6e 7374  lass LogBVVConst
-00010e00: 616e 744d 6f64 656c 284c 6f67 5461 7548  antModel(LogTauH
-00010e10: 4d6f 6465 6c29 3a0a 2020 2020 2727 270a  Model):.    '''.
-00010e20: 2020 2020 4c6f 6728 4272 6f6e 732d 5661      Log(Brons-Va
-00010e30: 6e2d 566c 6563 6b20 2a20 436f 6e73 7461  n-Vleck * Consta
-00010e40: 6e74 2920 4d6f 6465 6c20 6f66 206c 6f67  nt) Model of log
-00010e50: 3130 2852 656c 6178 6174 696f 6e20 7261  10(Relaxation ra
-00010e60: 7465 2920 7673 2066 6965 6c64 0a20 2020  te) vs field.   
-00010e70: 2027 2727 0a0a 2020 2020 233a 204d 6f64   '''..    #: Mod
-00010e80: 656c 206e 616d 650a 2020 2020 4e41 4d45  el name.    NAME
-00010e90: 203d 2027 4272 6f6e 732d 5661 6e2d 566c   = 'Brons-Van-Vl
-00010ea0: 6563 6b20 2a20 436f 6e73 7461 6e74 270a  eck * Constant'.
-00010eb0: 0a20 2020 2023 3a20 4d6f 6465 6c20 6e61  .    #: Model na
-00010ec0: 6d65 2077 6974 6820 6c6f 6720 6272 6163  me with log brac
-00010ed0: 6b65 7473 0a20 2020 204c 4e41 4d45 203d  kets.    LNAME =
-00010ee0: 2027 4c6f 6728 4272 6f6e 732d 5661 6e2d   'Log(Brons-Van-
-00010ef0: 566c 6563 6b20 2a20 436f 6e73 7461 6e74  Vleck * Constant
-00010f00: 2927 0a0a 2020 2020 233a 204d 6f64 656c  )'..    #: Model
-00010f10: 2050 6172 616d 6574 6572 206e 616d 6520   Parameter name 
-00010f20: 7374 7269 6e67 730a 2020 2020 5041 524e  strings.    PARN
-00010f30: 414d 4553 203d 205b 0a20 2020 2020 2020  AMES = [.       
-00010f40: 2027 6527 2c0a 2020 2020 2020 2020 2766   'e',.        'f
-00010f50: 272c 0a20 2020 2020 2020 2027 4374 270a  ',.        'Ct'.
-00010f60: 2020 2020 5d0a 0a20 2020 2023 3a20 4d6f      ]..    #: Mo
-00010f70: 6465 6c20 5061 7261 6d65 7465 7220 6e61  del Parameter na
-00010f80: 6d65 206d 6174 686d 6f64 6520 7374 7269  me mathmode stri
-00010f90: 6e67 730a 2020 2020 5641 524e 414d 4553  ngs.    VARNAMES
-00010fa0: 5f4d 4d20 3d20 7b0a 2020 2020 2020 2020  _MM = {.        
-00010fb0: 2765 273a 2072 2724 6524 272c 0a20 2020  'e': r'$e$',.   
-00010fc0: 2020 2020 2027 6627 3a20 7227 2466 2427       'f': r'$f$'
-00010fd0: 2c0a 2020 2020 2020 2020 2743 7427 3a20  ,.        'Ct': 
-00010fe0: 7227 2443 7424 270a 2020 2020 7d0a 0a20  r'$Ct$'.    }.. 
-00010ff0: 2020 2023 3a20 4d6f 6465 6c20 5061 7261     #: Model Para
-00011000: 6d65 7465 7220 6e61 6d65 2048 544d 4c20  meter name HTML 
-00011010: 7374 7269 6e67 730a 2020 2020 5641 524e  strings.    VARN
-00011020: 414d 4553 5f48 544d 4c20 3d20 7b0a 2020  AMES_HTML = {.  
-00011030: 2020 2020 2020 2765 273a 2027 6527 2c0a        'e': 'e',.
-00011040: 2020 2020 2020 2020 2766 273a 2027 6627          'f': 'f'
-00011050: 2c0a 2020 2020 2020 2020 2743 7427 3a20  ,.        'Ct': 
-00011060: 2743 7427 0a20 2020 207d 0a0a 2020 2020  'Ct'.    }..    
-00011070: 233a 204d 6f64 656c 2050 6172 616d 6574  #: Model Paramet
-00011080: 6572 2075 6e69 7420 7374 7269 6e67 730a  er unit strings.
-00011090: 2020 2020 554e 4954 5320 3d20 7b0a 2020      UNITS = {.  
-000110a0: 2020 2020 2020 2765 273a 2027 6c6f 6731        'e': 'log1
-000110b0: 305b 4f65 5e2d 325d 272c 0a20 2020 2020  0[Oe^-2]',.     
-000110c0: 2020 2027 6627 3a20 276c 6f67 3130 5b4f     'f': 'log10[O
-000110d0: 655e 2d32 5d27 2c0a 2020 2020 2020 2020  e^-2]',.        
-000110e0: 2743 7427 3a20 276c 6f67 3130 5b73 5e2d  'Ct': 'log10[s^-
-000110f0: 315d 270a 2020 2020 7d0a 0a20 2020 2023  1]'.    }..    #
-00011100: 3a20 4d6f 6465 6c20 5061 7261 6d65 7465  : Model Paramete
-00011110: 7220 756e 6974 206d 6174 686d 6f64 6520  r unit mathmode 
-00011120: 7374 7269 6e67 730a 2020 2020 554e 4954  strings.    UNIT
-00011130: 535f 4d4d 203d 207b 0a20 2020 2020 2020  S_MM = {.       
-00011140: 2027 6527 3a20 7227 245c 6c6f 675f 5c6d   'e': r'$\log_\m
-00011150: 6174 6872 6567 756c 6172 7b31 307d 5c6c  athregular{10}\l
-00011160: 6566 745b 5c6d 6174 6872 6567 756c 6172  eft[\mathregular
-00011170: 7b4f 657d 5e5c 6d61 7468 7265 6775 6c61  {Oe}^\mathregula
-00011180: 727b 2d32 7d5c 7269 6768 745d 2427 2c20  r{-2}\right]$', 
-00011190: 2320 6e6f 7161 0a20 2020 2020 2020 2027  # noqa.        '
-000111a0: 6627 3a20 7227 245c 6c6f 675f 5c6d 6174  f': r'$\log_\mat
-000111b0: 6872 6567 756c 6172 7b31 307d 5c6c 6566  hregular{10}\lef
-000111c0: 745b 5c6d 6174 6872 6567 756c 6172 7b4f  t[\mathregular{O
-000111d0: 657d 5e5c 6d61 7468 7265 6775 6c61 727b  e}^\mathregular{
-000111e0: 2d32 7d5c 7269 6768 745d 2427 2c20 2320  -2}\right]$', # 
-000111f0: 6e6f 7161 0a20 2020 2020 2020 2027 4374  noqa.        'Ct
-00011200: 273a 2072 2724 5c6c 6f67 5f5c 6d61 7468  ': r'$\log_\math
-00011210: 7265 6775 6c61 727b 3130 7d5c 6c65 6674  regular{10}\left
-00011220: 5b5c 6d61 7468 7265 6775 6c61 727b 737d  [\mathregular{s}
-00011230: 5e5c 6d61 7468 7265 6775 6c61 727b 2d31  ^\mathregular{-1
-00011240: 7d5c 7269 6768 745d 2427 2c20 2320 6e6f  }\right]$', # no
-00011250: 7161 0a20 2020 207d 0a0a 2020 2020 233a  qa.    }..    #:
-00011260: 204d 6f64 656c 2050 6172 616d 6574 6572   Model Parameter
-00011270: 2075 6e69 7420 4854 4d4c 2073 7472 696e   unit HTML strin
-00011280: 6773 0a20 2020 2055 4e49 5453 5f48 544d  gs.    UNITS_HTM
-00011290: 4c20 3d20 7b0a 2020 2020 2020 2020 2765  L = {.        'e
-000112a0: 273a 2072 276c 6f67 3c73 7562 3e31 303c  ': r'log<sub>10<
-000112b0: 2f73 7562 3e5b 4f65 3c73 7570 3e2d 323c  /sub>[Oe<sup>-2<
-000112c0: 2f73 7570 3e5d 272c 0a20 2020 2020 2020  /sup>]',.       
-000112d0: 2027 6627 3a20 7227 6c6f 673c 7375 623e   'f': r'log<sub>
-000112e0: 3130 3c2f 7375 623e 5b4f 653c 7375 703e  10</sub>[Oe<sup>
-000112f0: 2d32 3c2f 7375 703e 5d27 2c0a 2020 2020  -2</sup>]',.    
-00011300: 2020 2020 2743 7427 3a20 7227 6c6f 673c      'Ct': r'log<
-00011310: 7375 623e 3130 3c2f 7375 623e 5b73 3c73  sub>10</sub>[s<s
-00011320: 7570 3e2d 313c 2f73 7570 3e5d 270a 2020  up>-1</sup>]'.  
-00011330: 2020 7d0a 0a20 2020 2023 3a20 4d6f 6465    }..    #: Mode
-00011340: 6c20 7061 7261 6d65 7465 7220 626f 756e  l parameter boun
-00011350: 6473 0a20 2020 2042 4f55 4e44 5320 3d20  ds.    BOUNDS = 
-00011360: 7b0a 2020 2020 2020 2020 2765 273a 205b  {.        'e': [
-00011370: 2d33 302c 206e 702e 696e 665d 2c0a 2020  -30, np.inf],.  
-00011380: 2020 2020 2020 2766 273a 205b 2d33 302c        'f': [-30,
-00011390: 206e 702e 696e 665d 2c0a 2020 2020 2020   np.inf],.      
-000113a0: 2020 2743 7427 3a20 5b2d 3330 2c20 3130    'Ct': [-30, 10
-000113b0: 5d0a 2020 2020 7d0a 0a20 2020 2040 7374  ].    }..    @st
-000113c0: 6174 6963 6d65 7468 6f64 0a20 2020 2064  aticmethod.    d
-000113d0: 6566 2073 6574 5f69 6e69 7469 616c 5f76  ef set_initial_v
-000113e0: 616c 7328 7061 7261 6d5f 6469 6374 3a20  als(param_dict: 
-000113f0: 6469 6374 5b73 7472 2c20 7374 7220 7c20  dict[str, str | 
-00011400: 666c 6f61 745d 2920 2d3e 2064 6963 745b  float]) -> dict[
-00011410: 7374 722c 2066 6c6f 6174 5d3a 2023 206e  str, float]: # n
-00011420: 6f71 610a 2020 2020 2020 2020 2727 270a  oqa.        '''.
-00011430: 2020 2020 2020 2020 5365 7473 2067 7565          Sets gue
-00011440: 7373 2076 616c 7565 7320 666f 7220 7061  ss values for pa
-00011450: 7261 6d65 7465 7273 2069 6620 7265 7175  rameters if requ
-00011460: 6573 7465 6420 6279 2075 7365 720a 0a20  ested by user.. 
-00011470: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
-00011480: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
-00011490: 2d2d 2d2d 0a20 2020 2020 2020 2070 6172  ----.        par
-000114a0: 616d 5f64 6963 743a 2064 6963 745b 7374  am_dict: dict[st
-000114b0: 722c 2073 7472 207c 2066 6c6f 6174 5d0a  r, str | float].
-000114c0: 2020 2020 2020 2020 2020 2020 4b65 7973              Keys
-000114d0: 2061 7265 2066 6974 2f66 6978 2070 6172   are fit/fix par
-000114e0: 616d 6574 6572 206e 616d 6573 2028 7365  ameter names (se
-000114f0: 6520 636c 6173 732e 5041 524e 414d 4553  e class.PARNAMES
-00011500: 295c 6e0a 2020 2020 2020 2020 2020 2020  )\n.            
-00011510: 5661 6c75 6573 2061 7265 2065 6974 6865  Values are eithe
-00011520: 7220 666c 6f61 7420 2861 6374 7561 6c20  r float (actual 
-00011530: 7661 6c75 6529 206f 7220 7468 6520 7374  value) or the st
-00011540: 7269 6e67 2027 6775 6573 7327 0a0a 2020  ring 'guess'..  
-00011550: 2020 2020 2020 5265 7475 726e 730a 2020        Returns.  
-00011560: 2020 2020 2020 2d2d 2d2d 2d2d 2d0a 2020        -------.  
-00011570: 2020 2020 2020 6469 6374 5b73 7472 2c20        dict[str, 
-00011580: 666c 6f61 745d 0a20 2020 2020 2020 2020  float].         
-00011590: 2020 204b 6579 7320 6172 6520 6669 742f     Keys are fit/
-000115a0: 6669 7820 7061 7261 6d65 7465 7220 6e61  fix parameter na
-000115b0: 6d65 7320 2873 6565 2063 6c61 7373 2e50  mes (see class.P
-000115c0: 4152 4e41 4d45 5329 5c6e 0a20 2020 2020  ARNAMES)\n.     
-000115d0: 2020 2020 2020 2056 616c 7565 7320 6172         Values ar
-000115e0: 6520 666c 6f61 7420 2861 6374 7561 6c20  e float (actual 
-000115f0: 7661 6c75 6529 2077 6869 6368 2061 7265  value) which are
-00011600: 2069 6e69 7469 616c 2076 616c 7565 7320   initial values 
-00011610: 6f66 0a20 2020 2020 2020 2020 2020 2070  of.            p
-00011620: 6172 616d 6574 6572 0a20 2020 2020 2020  arameter.       
-00011630: 2027 2727 0a0a 2020 2020 2020 2020 2320   '''..        # 
-00011640: 4d61 6b65 2063 6f70 792c 2061 6e79 2073  Make copy, any s
-00011650: 7472 2076 616c 7565 7320 7769 6c6c 2062  tr values will b
-00011660: 6520 7265 706c 6163 6564 0a20 2020 2020  e replaced.     
-00011670: 2020 206e 6577 5f70 6172 616d 5f64 6963     new_param_dic
-00011680: 7420 3d20 636f 7079 2e63 6f70 7928 7061  t = copy.copy(pa
-00011690: 7261 6d5f 6469 6374 290a 0a20 2020 2020  ram_dict)..     
-000116a0: 2020 2023 2047 7565 7373 6573 0a20 2020     # Guesses.   
-000116b0: 2020 2020 2067 7565 7373 6469 6374 203d       guessdict =
-000116c0: 207b 0a20 2020 2020 2020 2020 2020 2027   {.            '
-000116d0: 6527 3a20 2d35 2e2c 0a20 2020 2020 2020  e': -5.,.       
-000116e0: 2020 2020 2027 6627 3a20 2d35 2e2c 0a20       'f': -5.,. 
-000116f0: 2020 2020 2020 2020 2020 2027 4374 273a             'Ct':
-00011700: 202d 340a 2020 2020 2020 2020 7d0a 0a20   -4.        }.. 
-00011710: 2020 2020 2020 2023 2052 6570 6c61 6365         # Replace
-00011720: 2027 6775 6573 7327 2077 6974 6820 7265   'guess' with re
-00011730: 6c65 7661 6e74 2067 7565 7373 0a20 2020  levant guess.   
-00011740: 2020 2020 2066 6f72 2076 6172 2c20 7661       for var, va
-00011750: 6c20 696e 2070 6172 616d 5f64 6963 742e  l in param_dict.
-00011760: 6974 656d 7328 293a 0a20 2020 2020 2020  items():.       
-00011770: 2020 2020 2069 6620 7661 6c20 3d3d 2027       if val == '
-00011780: 6775 6573 7327 3a0a 2020 2020 2020 2020  guess':.        
-00011790: 2020 2020 2020 2020 6e65 775f 7061 7261          new_para
-000117a0: 6d5f 6469 6374 5b76 6172 5d20 3d20 6775  m_dict[var] = gu
-000117b0: 6573 7364 6963 745b 7661 725d 0a0a 2020  essdict[var]..  
-000117c0: 2020 2020 2020 7265 7475 726e 206e 6577        return new
-000117d0: 5f70 6172 616d 5f64 6963 740a 0a20 2020  _param_dict..   
-000117e0: 2040 7374 6174 6963 6d65 7468 6f64 0a20   @staticmethod. 
-000117f0: 2020 2064 6566 206d 6f64 656c 2870 6172     def model(par
-00011800: 616d 6574 6572 733a 2064 6963 745b 7374  ameters: dict[st
-00011810: 722c 2066 6c6f 6174 5d2c 0a20 2020 2020  r, float],.     
-00011820: 2020 2020 2020 2020 2066 6965 6c64 733a           fields:
-00011830: 206e 7074 2e41 7272 6179 4c69 6b65 2920   npt.ArrayLike) 
-00011840: 2d3e 206e 7074 2e4e 4441 7272 6179 3a0a  -> npt.NDArray:.
-00011850: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
-00011860: 2020 2020 4576 616c 7561 7465 7320 6c6f      Evaluates lo
-00011870: 6731 3028 4c6f 6742 5656 436f 6e73 7461  g10(LogBVVConsta
-00011880: 6e74 4d6f 6465 6c29 206d 6f64 656c 206f  ntModel) model o
-00011890: 6620 6c6f 6731 3028 7265 6c61 7861 7469  f log10(relaxati
-000118a0: 6f6e 2072 6174 6529 0a20 2020 2020 2020  on rate).       
-000118b0: 2075 7369 6e67 2070 726f 7669 6465 6420   using provided 
-000118c0: 7061 7261 6d65 7465 7220 616e 6420 6669  parameter and fi
-000118d0: 656c 6420 7661 6c75 6573 2e0a 0a20 2020  eld values...   
-000118e0: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
-000118f0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-00011900: 2d2d 0a20 2020 2020 2020 2070 6172 616d  --.        param
-00011910: 6574 6572 733a 2064 6963 745b 7374 722c  eters: dict[str,
-00011920: 2066 6c6f 6174 5d0a 2020 2020 2020 2020   float].        
-00011930: 2020 2020 5061 7261 6d65 7465 7273 2074      Parameters t
-00011940: 6f20 7573 6520 696e 206d 6f64 656c 2066  o use in model f
-00011950: 756e 6374 696f 6e2c 206b 6579 7320 6172  unction, keys ar
-00011960: 6520 6769 7665 6e20 696e 0a20 2020 2020  e given in.     
-00011970: 2020 2020 2020 2063 6c61 7373 2e50 4152         class.PAR
-00011980: 4e41 4d45 530a 2020 2020 2020 2020 6669  NAMES.        fi
-00011990: 656c 6473 3a20 6172 7261 795f 6c69 6b65  elds: array_like
-000119a0: 0a20 2020 2020 2020 2020 2020 2066 6965  .            fie
-000119b0: 6c64 2076 616c 7565 7320 284f 6529 2061  ld values (Oe) a
-000119c0: 7420 7768 6963 6820 6d6f 6465 6c20 6675  t which model fu
-000119d0: 6e63 7469 6f6e 2069 7320 6576 616c 7561  nction is evalua
-000119e0: 7465 640a 0a20 2020 2020 2020 2052 6574  ted..        Ret
-000119f0: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
-00011a00: 2d2d 2d2d 0a20 2020 2020 2020 206e 6461  ----.        nda
-00011a10: 7272 6179 206f 6620 666c 6f61 7473 0a20  rray of floats. 
-00011a20: 2020 2020 2020 2020 2020 206c 6f67 3130             log10
-00011a30: 2852 656c 6178 6174 696f 6e20 7261 7465  (Relaxation rate
-00011a40: 2920 6173 2061 2066 756e 6374 696f 6e20  ) as a function 
-00011a50: 6f66 2066 6965 6c64 0a0a 2020 2020 2020  of field..      
-00011a60: 2020 2727 270a 0a20 2020 2020 2020 2065    '''..        e
-00011a70: 203d 2070 6172 616d 6574 6572 735b 2765   = parameters['e
-00011a80: 275d 0a20 2020 2020 2020 2066 203d 2070  '].        f = p
-00011a90: 6172 616d 6574 6572 735b 2766 275d 0a20  arameters['f']. 
-00011aa0: 2020 2020 2020 2043 7420 3d20 7061 7261         Ct = para
-00011ab0: 6d65 7465 7273 5b27 4374 275d 0a0a 2020  meters['Ct']..  
-00011ac0: 2020 2020 2020 6c6f 6772 6174 6520 3d20        lograte = 
-00011ad0: 6e70 2e6c 6f67 3130 280a 2020 2020 2020  np.log10(.      
-00011ae0: 2020 2020 2020 3130 2a2a 4374 202a 2028        10**Ct * (
-00011af0: 3120 2b20 3130 2a2a 6520 2a20 6e70 2e61  1 + 10**e * np.a
-00011b00: 7361 7272 6179 2866 6965 6c64 7329 2a2a  sarray(fields)**
-00011b10: 3229 202f 2028 3120 2b20 3130 2a2a 6620  2) / (1 + 10**f 
-00011b20: 2a20 6e70 2e61 7361 7272 6179 2866 6965  * np.asarray(fie
-00011b30: 6c64 7329 2a2a 3229 2023 206e 6f71 610a  lds)**2) # noqa.
-00011b40: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-00011b50: 2020 2072 6574 7572 6e20 6c6f 6772 6174     return lograt
-00011b60: 650a 0a0a 636c 6173 7320 4c6f 6754 6175  e...class LogTau
-00011b70: 544d 6f64 656c 2841 4243 293a 0a20 2020  TModel(ABC):.   
-00011b80: 2027 2727 0a20 2020 2041 6273 7472 6163   '''.    Abstrac
-00011b90: 7420 636c 6173 7320 6f6e 2077 6869 6368  t class on which
-00011ba0: 2061 6c6c 2070 6865 6e6f 6d65 6e6f 6c6f   all phenomenolo
-00011bb0: 6769 6361 6c20 6d6f 6465 6c73 206f 660a  gical models of.
-00011bc0: 2020 2020 7465 6d70 6572 6174 7572 652d      temperature-
-00011bd0: 6465 7065 6e64 656e 7420 6d61 676e 6574  dependent magnet
-00011be0: 6963 2072 656c 6178 6174 696f 6e20 4c6f  ic relaxation Lo
-00011bf0: 6731 3028 7261 7465 2920 6172 6520 6261  g10(rate) are ba
-00011c00: 7365 640a 2020 2020 2727 270a 0a20 2020  sed.    '''..   
-00011c10: 2040 7072 6f70 6572 7479 0a20 2020 2040   @property.    @
-00011c20: 6162 7374 7261 6374 6d65 7468 6f64 0a20  abstractmethod. 
-00011c30: 2020 2064 6566 204e 414d 4528 2920 2d3e     def NAME() ->
-00011c40: 2073 7472 3a0a 2020 2020 2020 2020 2773   str:.        's
-00011c50: 7472 696e 6720 6e61 6d65 206f 6620 6d6f  tring name of mo
-00011c60: 6465 6c27 0a20 2020 2020 2020 2072 6169  del'.        rai
-00011c70: 7365 204e 6f74 496d 706c 656d 656e 7465  se NotImplemente
-00011c80: 6445 7272 6f72 0a0a 2020 2020 4070 726f  dError..    @pro
-00011c90: 7065 7274 790a 2020 2020 4061 6273 7472  perty.    @abstr
-00011ca0: 6163 746d 6574 686f 640a 2020 2020 6465  actmethod.    de
-00011cb0: 6620 4c4e 414d 4528 2920 2d3e 2073 7472  f LNAME() -> str
-00011cc0: 3a0a 2020 2020 2020 2020 2773 7472 696e  :.        'strin
-00011cd0: 6720 6e61 6d65 206f 6620 6d6f 6465 6c20  g name of model 
-00011ce0: 7769 7468 204c 6f67 2829 2061 726f 756e  with Log() aroun
-00011cf0: 6420 6974 2c20 652e 672e 204c 6f67 284f  d it, e.g. Log(O
-00011d00: 7262 6163 6829 270a 2020 2020 2020 2020  rbach)'.        
-00011d10: 7261 6973 6520 4e6f 7449 6d70 6c65 6d65  raise NotImpleme
-00011d20: 6e74 6564 4572 726f 720a 0a20 2020 2040  ntedError..    @
-00011d30: 7072 6f70 6572 7479 0a20 2020 2040 6162  property.    @ab
-00011d40: 7374 7261 6374 6d65 7468 6f64 0a20 2020  stractmethod.   
-00011d50: 2064 6566 2050 4152 4e41 4d45 5328 2920   def PARNAMES() 
-00011d60: 2d3e 206c 6973 745b 7374 725d 3a0a 2020  -> list[str]:.  
-00011d70: 2020 2020 2020 2773 7472 696e 6720 6e61        'string na
-00011d80: 6d65 7320 6f66 2070 6172 616d 6574 6572  mes of parameter
-00011d90: 7320 7768 6963 6820 6361 6e20 6265 2066  s which can be f
-00011da0: 6974 7465 6420 6f72 2066 6978 6564 270a  itted or fixed'.
-00011db0: 2020 2020 2020 2020 7261 6973 6520 4e6f          raise No
-00011dc0: 7449 6d70 6c65 6d65 6e74 6564 4572 726f  tImplementedErro
-00011dd0: 720a 0a20 2020 2040 7072 6f70 6572 7479  r..    @property
-00011de0: 0a20 2020 2040 6162 7374 7261 6374 6d65  .    @abstractme
-00011df0: 7468 6f64 0a20 2020 2064 6566 2056 4152  thod.    def VAR
-00011e00: 4e41 4d45 535f 4d4d 2829 202d 3e20 6469  NAMES_MM() -> di
-00011e10: 6374 5b73 7472 2c20 7374 725d 3a0a 2020  ct[str, str]:.  
-00011e20: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
-00011e30: 2020 4d61 7468 6d6f 6465 2028 692e 652e    Mathmode (i.e.
-00011e40: 2024 242c 206c 6174 6578 2029 2076 6572   $$, latex ) ver
-00011e50: 7369 6f6e 7320 6f66 2050 4152 4e41 4d45  sions of PARNAME
-00011e60: 535c 6e0a 2020 2020 2020 2020 4b65 7973  S\n.        Keys
-00011e70: 2061 7265 2073 7472 696e 6773 2066 726f   are strings fro
-00011e80: 6d20 5041 524e 414d 4553 2070 6c75 7320  m PARNAMES plus 
-00011e90: 616e 7920 6f74 6865 7220 7661 7269 6162  any other variab
-00011ea0: 6c65 7320 7768 6963 680a 2020 2020 2020  les which.      
-00011eb0: 2020 6d69 6768 7420 6265 206e 6565 6465    might be neede
-00011ec0: 645c 6e0a 2020 2020 2020 2020 5661 6c75  d\n.        Valu
-00011ed0: 6573 2061 7265 206d 6174 686d 6f64 6520  es are mathmode 
-00011ee0: 7374 7269 6e67 730a 2020 2020 2020 2020  strings.        
-00011ef0: 2727 270a 2020 2020 2020 2020 7261 6973  '''.        rais
-00011f00: 6520 4e6f 7449 6d70 6c65 6d65 6e74 6564  e NotImplemented
-00011f10: 4572 726f 720a 0a20 2020 2040 7072 6f70  Error..    @prop
-00011f20: 6572 7479 0a20 2020 2040 6162 7374 7261  erty.    @abstra
-00011f30: 6374 6d65 7468 6f64 0a20 2020 2064 6566  ctmethod.    def
-00011f40: 2056 4152 4e41 4d45 535f 4854 4d4c 2829   VARNAMES_HTML()
-00011f50: 202d 3e20 6469 6374 5b73 7472 2c20 7374   -> dict[str, st
-00011f60: 725d 3a0a 2020 2020 2020 2020 2727 270a  r]:.        '''.
-00011f70: 2020 2020 2020 2020 4854 4d4c 2076 6572          HTML ver
-00011f80: 7369 6f6e 7320 6f66 2050 4152 4e41 4d45  sions of PARNAME
-00011f90: 535c 6e0a 2020 2020 2020 2020 4b65 7973  S\n.        Keys
-00011fa0: 2061 7265 2073 7472 696e 6773 2066 726f   are strings fro
-00011fb0: 6d20 5041 524e 414d 4553 2070 6c75 7320  m PARNAMES plus 
-00011fc0: 616e 7920 6f74 6865 7220 7661 7269 6162  any other variab
-00011fd0: 6c65 7320 7768 6963 680a 2020 2020 2020  les which.      
-00011fe0: 2020 6d69 6768 7420 6265 206e 6565 6465    might be neede
-00011ff0: 645c 6e0a 2020 2020 2020 2020 5661 6c75  d\n.        Valu
-00012000: 6573 2061 7265 206d 6174 686d 6f64 6520  es are mathmode 
-00012010: 7374 7269 6e67 730a 2020 2020 2020 2020  strings.        
-00012020: 2727 270a 2020 2020 2020 2020 7261 6973  '''.        rais
-00012030: 6520 4e6f 7449 6d70 6c65 6d65 6e74 6564  e NotImplemented
-00012040: 4572 726f 720a 0a20 2020 2040 7072 6f70  Error..    @prop
-00012050: 6572 7479 0a20 2020 2040 6162 7374 7261  erty.    @abstra
-00012060: 6374 6d65 7468 6f64 0a20 2020 2064 6566  ctmethod.    def
-00012070: 2055 4e49 5453 2829 202d 3e20 6469 6374   UNITS() -> dict
-00012080: 5b73 7472 2c20 7374 725d 3a0a 2020 2020  [str, str]:.    
-00012090: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
-000120a0: 7374 7269 6e67 206e 616d 6573 206f 6620  string names of 
-000120b0: 756e 6974 7320 6f66 2050 4152 4e41 4d45  units of PARNAME
-000120c0: 535c 6e0a 2020 2020 2020 2020 4b65 7973  S\n.        Keys
-000120d0: 2061 7265 2073 7472 696e 6773 2066 726f   are strings fro
-000120e0: 6d20 5041 524e 414d 4553 2070 6c75 7320  m PARNAMES plus 
-000120f0: 616e 7920 6f74 6865 7220 7661 7269 6162  any other variab
-00012100: 6c65 7320 7768 6963 680a 2020 2020 2020  les which.      
-00012110: 2020 6d69 6768 7420 6265 206e 6565 6465    might be neede
-00012120: 645c 6e0a 2020 2020 2020 2020 5661 6c75  d\n.        Valu
-00012130: 6573 2061 7265 2075 6e69 7420 6e61 6d65  es are unit name
-00012140: 2073 7472 696e 6773 0a20 2020 2020 2020   strings.       
-00012150: 2027 2727 0a20 2020 2020 2020 2072 6169   '''.        rai
-00012160: 7365 204e 6f74 496d 706c 656d 656e 7465  se NotImplemente
-00012170: 6445 7272 6f72 0a0a 2020 2020 4070 726f  dError..    @pro
-00012180: 7065 7274 790a 2020 2020 4061 6273 7472  perty.    @abstr
-00012190: 6163 746d 6574 686f 640a 2020 2020 6465  actmethod.    de
-000121a0: 6620 554e 4954 535f 4d4d 2829 202d 3e20  f UNITS_MM() -> 
-000121b0: 6469 6374 5b73 7472 2c20 7374 725d 3a0a  dict[str, str]:.
-000121c0: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
-000121d0: 2020 2020 4d61 7468 6d6f 6465 2028 692e      Mathmode (i.
-000121e0: 652e 2024 242c 206c 6174 6578 2029 2076  e. $$, latex ) v
-000121f0: 6572 7369 6f6e 7320 6f66 2055 4e49 5453  ersions of UNITS
-00012200: 5c6e 0a20 2020 2020 2020 204b 6579 7320  \n.        Keys 
-00012210: 6172 6520 7374 7269 6e67 7320 6672 6f6d  are strings from
-00012220: 2050 4152 4e41 4d45 5320 706c 7573 2061   PARNAMES plus a
-00012230: 6e79 206f 7468 6572 2076 6172 6961 626c  ny other variabl
-00012240: 6573 2077 6869 6368 0a20 2020 2020 2020  es which.       
-00012250: 206d 6967 6874 2062 6520 6e65 6564 6564   might be needed
-00012260: 5c6e 0a20 2020 2020 2020 2056 616c 7565  \n.        Value
-00012270: 7320 6172 6520 756e 6974 206e 616d 6520  s are unit name 
-00012280: 7374 7269 6e67 730a 2020 2020 2020 2020  strings.        
-00012290: 2727 270a 2020 2020 2020 2020 7261 6973  '''.        rais
-000122a0: 6520 4e6f 7449 6d70 6c65 6d65 6e74 6564  e NotImplemented
-000122b0: 4572 726f 720a 0a20 2020 2040 7072 6f70  Error..    @prop
-000122c0: 6572 7479 0a20 2020 2040 6162 7374 7261  erty.    @abstra
-000122d0: 6374 6d65 7468 6f64 0a20 2020 2064 6566  ctmethod.    def
-000122e0: 2055 4e49 5453 5f48 544d 4c28 2920 2d3e   UNITS_HTML() ->
-000122f0: 2064 6963 745b 7374 722c 2073 7472 5d3a   dict[str, str]:
-00012300: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
-00012310: 2020 2020 2048 544d 4c20 7665 7273 696f       HTML versio
-00012320: 6e73 206f 6620 554e 4954 535c 6e0a 2020  ns of UNITS\n.  
-00012330: 2020 2020 2020 4b65 7973 2061 7265 2073        Keys are s
-00012340: 7472 696e 6773 2066 726f 6d20 5041 524e  trings from PARN
-00012350: 414d 4553 2070 6c75 7320 616e 7920 6f74  AMES plus any ot
-00012360: 6865 7220 7661 7269 6162 6c65 7320 7768  her variables wh
-00012370: 6963 680a 2020 2020 2020 2020 6d69 6768  ich.        migh
-00012380: 7420 6265 206e 6565 6465 645c 6e0a 2020  t be needed\n.  
-00012390: 2020 2020 2020 5661 6c75 6573 2061 7265        Values are
-000123a0: 2075 6e69 7420 6e61 6d65 2073 7472 696e   unit name strin
-000123b0: 6773 0a20 2020 2020 2020 2027 2727 0a20  gs.        '''. 
-000123c0: 2020 2020 2020 2072 6169 7365 204e 6f74         raise Not
-000123d0: 496d 706c 656d 656e 7465 6445 7272 6f72  ImplementedError
-000123e0: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
-000123f0: 2020 2020 4061 6273 7472 6163 746d 6574      @abstractmet
-00012400: 686f 640a 2020 2020 6465 6620 424f 554e  hod.    def BOUN
-00012410: 4453 2829 202d 3e20 6469 6374 5b73 7472  DS() -> dict[str
-00012420: 2c20 6c69 7374 5b66 6c6f 6174 2c20 666c  , list[float, fl
-00012430: 6f61 745d 5d3a 0a20 2020 2020 2020 2027  oat]]:.        '
-00012440: 2727 0a20 2020 2020 2020 2042 6f75 6e64  ''.        Bound
-00012450: 7320 666f 7220 6561 6368 2070 6172 616d  s for each param
-00012460: 6574 6572 206f 6620 6d6f 6465 6c5c 6e0a  eter of model\n.
-00012470: 2020 2020 2020 2020 4b65 7973 3a20 7061          Keys: pa
-00012480: 7261 6d65 7465 7220 6e61 6d65 5c6e 0a20  rameter name\n. 
-00012490: 2020 2020 2020 2056 616c 7565 733a 205b         Values: [
-000124a0: 7570 7065 722c 206c 6f77 6572 5d5c 6e0a  upper, lower]\n.
-000124b0: 2020 2020 2020 2020 7573 6564 2062 7920          used by 
-000124c0: 7363 6970 7920 6c65 6173 745f 7371 7561  scipy least_squa
-000124d0: 7265 730a 2020 2020 2020 2020 2727 270a  res.        '''.
-000124e0: 2020 2020 2020 2020 7261 6973 6520 4e6f          raise No
-000124f0: 7449 6d70 6c65 6d65 6e74 6564 4572 726f  tImplementedErro
-00012500: 720a 0a20 2020 2040 7374 6174 6963 6d65  r..    @staticme
-00012510: 7468 6f64 0a20 2020 2040 6162 7374 7261  thod.    @abstra
-00012520: 6374 6d65 7468 6f64 0a20 2020 2064 6566  ctmethod.    def
-00012530: 206d 6f64 656c 2870 6172 616d 6574 6572   model(parameter
-00012540: 733a 2064 6963 745b 7374 722c 2066 6c6f  s: dict[str, flo
-00012550: 6174 5d2c 0a20 2020 2020 2020 2020 2020  at],.           
-00012560: 2020 2074 656d 7065 7261 7475 7265 733a     temperatures:
-00012570: 206e 7074 2e41 7272 6179 4c69 6b65 2920   npt.ArrayLike) 
-00012580: 2d3e 206e 7074 2e4e 4441 7272 6179 3a0a  -> npt.NDArray:.
-00012590: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
-000125a0: 2020 2020 4576 616c 7561 7465 7320 6d6f      Evaluates mo
-000125b0: 6465 6c20 6675 6e63 7469 6f6e 206f 6620  del function of 
-000125c0: 6c6f 6728 7265 6c61 7861 7469 6f6e 2072  log(relaxation r
-000125d0: 6174 6529 2075 7369 6e67 2070 726f 7669  ate) using provi
-000125e0: 6465 640a 2020 2020 2020 2020 7061 7261  ded.        para
-000125f0: 6d65 7465 7220 616e 6420 7465 6d70 6572  meter and temper
-00012600: 6174 7572 6520 7661 6c75 6573 2e0a 0a20  ature values... 
-00012610: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
-00012620: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
-00012630: 2d2d 2d2d 0a20 2020 2020 2020 2070 6172  ----.        par
-00012640: 616d 6574 6572 733a 2061 7272 6179 5f6c  ameters: array_l
-00012650: 696b 650a 2020 2020 2020 2020 2020 2020  ike.            
-00012660: 5061 7261 6d65 7465 7273 2074 6f20 7573  Parameters to us
-00012670: 6520 696e 206d 6f64 656c 2066 756e 6374  e in model funct
-00012680: 696f 6e0a 2020 2020 2020 2020 7465 6d70  ion.        temp
-00012690: 6572 6174 7572 6573 3a20 6172 7261 795f  eratures: array_
-000126a0: 6c69 6b65 0a20 2020 2020 2020 2020 2020  like.           
-000126b0: 2054 656d 7065 7261 7475 7265 2076 616c   Temperature val
-000126c0: 7565 7320 284b 2920 6174 2077 6869 6368  ues (K) at which
-000126d0: 206d 6f64 656c 2066 756e 6374 696f 6e20   model function 
-000126e0: 6973 2065 7661 6c75 6174 6564 0a0a 2020  is evaluated..  
-000126f0: 2020 2020 2020 5265 7475 726e 730a 2020        Returns.  
-00012700: 2020 2020 2020 2d2d 2d2d 2d2d 2d0a 2020        -------.  
-00012710: 2020 2020 2020 6e64 6172 7261 7920 6f66        ndarray of
-00012720: 2066 6c6f 6174 730a 2020 2020 2020 2020   floats.        
-00012730: 2020 2020 6c6f 6731 3028 5265 6c61 7861      log10(Relaxa
-00012740: 7469 6f6e 2072 6174 6529 2061 7320 6120  tion rate) as a 
-00012750: 6675 6e63 7469 6f6e 206f 6620 7465 6d70  function of temp
-00012760: 6572 6174 7572 650a 0a20 2020 2020 2020  erature..       
-00012770: 2027 2727 0a20 2020 2020 2020 2072 6169   '''.        rai
-00012780: 7365 204e 6f74 496d 706c 656d 656e 7465  se NotImplemente
-00012790: 6445 7272 6f72 0a0a 2020 2020 4073 7461  dError..    @sta
-000127a0: 7469 636d 6574 686f 640a 2020 2020 4061  ticmethod.    @a
-000127b0: 6273 7472 6163 746d 6574 686f 640a 2020  bstractmethod.  
-000127c0: 2020 6465 6620 7365 745f 696e 6974 6961    def set_initia
-000127d0: 6c5f 7661 6c73 2870 6172 616d 6574 6572  l_vals(parameter
-000127e0: 733a 2064 6963 745b 7374 722c 2066 6c6f  s: dict[str, flo
-000127f0: 6174 5d29 202d 3e20 6469 6374 5b73 7472  at]) -> dict[str
-00012800: 2c20 666c 6f61 745d 3a0a 2020 2020 2020  , float]:.      
-00012810: 2020 2727 270a 2020 2020 2020 2020 5365    '''.        Se
-00012820: 7473 2067 7565 7373 2076 616c 7565 7320  ts guess values 
-00012830: 666f 7220 7061 7261 6d65 7465 7273 2069  for parameters i
-00012840: 6620 7265 7175 6573 7465 6420 6279 2075  f requested by u
-00012850: 7365 720a 0a20 2020 2020 2020 2050 6172  ser..        Par
-00012860: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
-00012870: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
-00012880: 2020 2070 6172 616d 5f64 6963 743a 2064     param_dict: d
-00012890: 6963 745b 7374 722c 2073 7472 207c 2066  ict[str, str | f
-000128a0: 6c6f 6174 5d0a 2020 2020 2020 2020 2020  loat].          
-000128b0: 2020 4b65 7973 2061 7265 2066 6974 2f66    Keys are fit/f
-000128c0: 6978 2070 6172 616d 6574 6572 206e 616d  ix parameter nam
-000128d0: 6573 2028 7365 6520 636c 6173 732e 5041  es (see class.PA
-000128e0: 524e 414d 4553 295c 6e0a 2020 2020 2020  RNAMES)\n.      
-000128f0: 2020 2020 2020 5661 6c75 6573 2061 7265        Values are
-00012900: 2065 6974 6865 7220 666c 6f61 7420 2861   either float (a
-00012910: 6374 7561 6c20 7661 6c75 6529 206f 7220  ctual value) or 
-00012920: 7468 6520 7374 7269 6e67 2027 6775 6573  the string 'gues
-00012930: 7327 0a0a 2020 2020 2020 2020 5265 7475  s'..        Retu
-00012940: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
-00012950: 2d2d 2d0a 2020 2020 2020 2020 6469 6374  ---.        dict
-00012960: 5b73 7472 2c20 666c 6f61 745d 0a20 2020  [str, float].   
-00012970: 2020 2020 2020 2020 204b 6579 7320 6172           Keys ar
-00012980: 6520 6669 742f 6669 7820 7061 7261 6d65  e fit/fix parame
-00012990: 7465 7220 6e61 6d65 7320 2873 6565 2063  ter names (see c
-000129a0: 6c61 7373 2e50 4152 4e41 4d45 5329 5c6e  lass.PARNAMES)\n
-000129b0: 0a20 2020 2020 2020 2020 2020 2056 616c  .            Val
-000129c0: 7565 7320 6172 6520 666c 6f61 7420 2861  ues are float (a
-000129d0: 6374 7561 6c20 7661 6c75 6529 2077 6869  ctual value) whi
-000129e0: 6368 2061 7265 2069 6e69 7469 616c 2076  ch are initial v
-000129f0: 616c 7565 7320 6f66 0a20 2020 2020 2020  alues of.       
-00012a00: 2020 2020 2070 6172 616d 6574 6572 0a20       parameter. 
-00012a10: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
-00012a20: 2020 2072 6169 7365 204e 6f74 496d 706c     raise NotImpl
-00012a30: 656d 656e 7465 6445 7272 6f72 0a0a 2020  ementedError..  
-00012a40: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
-00012a50: 656c 662c 2066 6974 5f76 6172 733a 2064  elf, fit_vars: d
-00012a60: 6963 745b 7374 722c 2066 6c6f 6174 207c  ict[str, float |
-00012a70: 2073 7472 5d2c 0a20 2020 2020 2020 2020   str],.         
-00012a80: 2020 2020 2020 2020 6669 785f 7661 7273          fix_vars
-00012a90: 3a20 6469 6374 5b73 7472 2c20 666c 6f61  : dict[str, floa
-00012aa0: 7420 7c20 7374 725d 293a 0a20 2020 2020  t | str]):.     
-00012ab0: 2020 2027 2727 0a20 2020 2020 2020 2053     '''.        S
-00012ac0: 6574 2064 6566 6175 6c74 2076 616c 7565  et default value
-00012ad0: 7320 666f 7220 6d61 6e64 6174 6f72 7920  s for mandatory 
-00012ae0: 6174 7472 6962 7574 6573 0a20 2020 2020  attributes.     
-00012af0: 2020 2027 2727 0a0a 2020 2020 2020 2020     '''..        
-00012b00: 2320 5265 706c 6163 6520 616e 7920 2767  # Replace any 'g
-00012b10: 7565 7373 2720 7374 7269 6e67 7320 7769  uess' strings wi
-00012b20: 7468 2070 726f 7065 7220 6775 6573 7365  th proper guesse
-00012b30: 730a 2020 2020 2020 2020 7365 6c66 2e66  s.        self.f
-00012b40: 6974 5f76 6172 7320 3d20 7365 6c66 2e73  it_vars = self.s
-00012b50: 6574 5f69 6e69 7469 616c 5f76 616c 7328  et_initial_vals(
-00012b60: 6669 745f 7661 7273 290a 2020 2020 2020  fit_vars).      
-00012b70: 2020 7365 6c66 2e66 6978 5f76 6172 7320    self.fix_vars 
-00012b80: 3d20 7365 6c66 2e73 6574 5f69 6e69 7469  = self.set_initi
-00012b90: 616c 5f76 616c 7328 6669 785f 7661 7273  al_vals(fix_vars
-00012ba0: 290a 0a20 2020 2020 2020 2023 2043 6865  )..        # Che
-00012bb0: 636b 2061 6c6c 2050 4152 4e41 4d45 5320  ck all PARNAMES 
-00012bc0: 6172 6520 7072 6f76 6964 6564 2069 6e20  are provided in 
-00012bd0: 6669 742b 6669 780a 2020 2020 2020 2020  fit+fix.        
-00012be0: 696e 7075 745f 6e61 6d65 7320 3d20 5b0a  input_names = [.
-00012bf0: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
-00012c00: 2066 6f72 206e 616d 6520 696e 207b 2a2a   for name in {**
-00012c10: 7365 6c66 2e66 6974 5f76 6172 732c 202a  self.fit_vars, *
-00012c20: 2a73 656c 662e 6669 785f 7661 7273 7d2e  *self.fix_vars}.
-00012c30: 6b65 7973 2829 0a20 2020 2020 2020 205d  keys().        ]
-00012c40: 0a0a 2020 2020 2020 2020 6966 2061 6e79  ..        if any
-00012c50: 285b 7265 715f 6e61 6d65 206e 6f74 2069  ([req_name not i
-00012c60: 6e20 696e 7075 745f 6e61 6d65 7320 666f  n input_names fo
-00012c70: 7220 7265 715f 6e61 6d65 2069 6e20 7365  r req_name in se
-00012c80: 6c66 2e50 4152 4e41 4d45 535d 293a 0a20  lf.PARNAMES]):. 
-00012c90: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00012ca0: 2056 616c 7565 4572 726f 7228 0a20 2020   ValueError(.   
-00012cb0: 2020 2020 2020 2020 2020 2020 2027 4d69               'Mi
-00012cc0: 7373 696e 6720 6669 742f 6669 7820 7061  ssing fit/fix pa
-00012cd0: 7261 6d65 7465 7273 2069 6e20 7b7d 204d  rameters in {} M
-00012ce0: 6f64 656c 272e 666f 726d 6174 280a 2020  odel'.format(.  
-00012cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012d00: 2020 7365 6c66 2e4e 414d 450a 2020 2020    self.NAME.    
-00012d10: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00012d20: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
-00012d30: 2020 2020 2023 2046 696e 616c 206d 6f64       # Final mod
-00012d40: 656c 2070 6172 616d 6574 6572 2076 616c  el parameter val
-00012d50: 7565 730a 2020 2020 2020 2020 2320 6669  ues.        # fi
-00012d60: 7474 6564 2061 6e64 2066 6978 6564 0a20  tted and fixed. 
-00012d70: 2020 2020 2020 2073 656c 662e 5f66 696e         self._fin
-00012d80: 616c 5f76 6172 5f76 616c 7565 7320 3d20  al_var_values = 
-00012d90: 7b0a 2020 2020 2020 2020 2020 2020 7661  {.            va
-00012da0: 723a 204e 6f6e 650a 2020 2020 2020 2020  r: None.        
-00012db0: 2020 2020 666f 7220 7661 7220 696e 2073      for var in s
-00012dc0: 656c 662e 5041 524e 414d 4553 0a20 2020  elf.PARNAMES.   
-00012dd0: 2020 2020 207d 0a0a 2020 2020 2020 2020       }..        
-00012de0: 2320 4669 7420 7374 6174 7573 2061 6e64  # Fit status and
-00012df0: 2074 656d 7065 7261 7475 7265 0a20 2020   temperature.   
-00012e00: 2020 2020 2073 656c 662e 5f66 6974 5f73       self._fit_s
-00012e10: 7461 7475 7320 3d20 4661 6c73 650a 0a20  tatus = False.. 
-00012e20: 2020 2020 2020 2023 2046 6974 2073 7461         # Fit sta
-00012e30: 6e64 6172 6420 6465 7669 6174 696f 6e0a  ndard deviation.
-00012e40: 2020 2020 2020 2020 7365 6c66 2e5f 6669          self._fi
-00012e50: 745f 7374 6465 7620 3d20 7b0a 2020 2020  t_stdev = {.    
-00012e60: 2020 2020 2020 2020 7661 723a 204e 6f6e          var: Non
-00012e70: 650a 2020 2020 2020 2020 2020 2020 666f  e.            fo
-00012e80: 7220 7661 7220 696e 2073 656c 662e 6669  r var in self.fi
-00012e90: 745f 7661 7273 2e6b 6579 7328 290a 2020  t_vars.keys().  
-00012ea0: 2020 2020 2020 7d0a 0a20 2020 2020 2020        }..       
-00012eb0: 2072 6574 7572 6e0a 0a20 2020 2040 7072   return..    @pr
-00012ec0: 6f70 6572 7479 0a20 2020 2064 6566 2066  operty.    def f
-00012ed0: 6974 5f73 7461 7475 7328 7365 6c66 2920  it_status(self) 
-00012ee0: 2d3e 2062 6f6f 6c3a 0a20 2020 2020 2020  -> bool:.       
-00012ef0: 2027 5472 7565 2069 6620 6669 7420 7375   'True if fit su
-00012f00: 6363 6573 7366 756c 2c20 656c 7365 2046  ccessful, else F
-00012f10: 616c 7365 270a 2020 2020 2020 2020 7265  alse'.        re
-00012f20: 7475 726e 2073 656c 662e 5f66 6974 5f73  turn self._fit_s
-00012f30: 7461 7475 730a 0a20 2020 2040 6669 745f  tatus..    @fit_
-00012f40: 7374 6174 7573 2e73 6574 7465 720a 2020  status.setter.  
-00012f50: 2020 6465 6620 6669 745f 7374 6174 7573    def fit_status
-00012f60: 2873 656c 662c 2076 616c 7565 293a 0a20  (self, value):. 
-00012f70: 2020 2020 2020 2069 6620 7479 7065 2876         if type(v
-00012f80: 616c 7565 2920 3d3d 2062 6f6f 6c3a 0a20  alue) == bool:. 
-00012f90: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00012fa0: 5f66 6974 5f73 7461 7475 7320 3d20 7661  _fit_status = va
-00012fb0: 6c75 650a 2020 2020 2020 2020 656c 7365  lue.        else
-00012fc0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-00012fd0: 6973 6520 5479 7065 4572 726f 720a 2020  ise TypeError.  
-00012fe0: 2020 2020 2020 7265 7475 726e 0a0a 2020        return..  
-00012ff0: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
-00013000: 6465 6620 6669 6e61 6c5f 7661 725f 7661  def final_var_va
-00013010: 6c75 6573 2873 656c 6629 202d 3e20 666c  lues(self) -> fl
-00013020: 6f61 743a 0a20 2020 2020 2020 2027 4669  oat:.        'Fi
-00013030: 6e61 6c20 7661 6c75 6573 206f 6620 7061  nal values of pa
-00013040: 7261 6d65 7465 7273 2c20 626f 7468 2066  rameters, both f
-00013050: 6974 7465 6420 616e 6420 6669 7865 6427  itted and fixed'
-00013060: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00013070: 7365 6c66 2e5f 6669 6e61 6c5f 7661 725f  self._final_var_
-00013080: 7661 6c75 6573 0a0a 2020 2020 4066 696e  values..    @fin
-00013090: 616c 5f76 6172 5f76 616c 7565 732e 7365  al_var_values.se
-000130a0: 7474 6572 0a20 2020 2064 6566 2066 696e  tter.    def fin
-000130b0: 616c 5f76 6172 5f76 616c 7565 7328 7365  al_var_values(se
-000130c0: 6c66 2c20 7661 6c75 6529 3a0a 2020 2020  lf, value):.    
-000130d0: 2020 2020 6966 2074 7970 6528 7661 6c75      if type(valu
-000130e0: 6529 203d 3d20 6469 6374 3a0a 2020 2020  e) == dict:.    
-000130f0: 2020 2020 2020 2020 7365 6c66 2e5f 6669          self._fi
-00013100: 6e61 6c5f 7661 725f 7661 6c75 6573 203d  nal_var_values =
-00013110: 2076 616c 7565 0a20 2020 2020 2020 2065   value.        e
-00013120: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00013130: 2072 6169 7365 2054 7970 6545 7272 6f72   raise TypeError
-00013140: 0a20 2020 2020 2020 2072 6574 7572 6e0a  .        return.
-00013150: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-00013160: 2020 2064 6566 2066 6974 5f73 7464 6576     def fit_stdev
-00013170: 2873 656c 6629 202d 3e20 666c 6f61 743a  (self) -> float:
-00013180: 0a20 2020 2020 2020 2027 5374 616e 6461  .        'Standa
-00013190: 7264 2064 6576 6961 7469 6f6e 206f 6e20  rd deviation on 
-000131a0: 6669 7474 6564 2070 6172 616d 6574 6572  fitted parameter
-000131b0: 732c 2066 726f 6d20 6669 7474 696e 6720  s, from fitting 
-000131c0: 726f 7574 696e 6527 0a20 2020 2020 2020  routine'.       
-000131d0: 2072 6574 7572 6e20 7365 6c66 2e5f 6669   return self._fi
-000131e0: 745f 7374 6465 760a 0a20 2020 2040 6669  t_stdev..    @fi
-000131f0: 745f 7374 6465 762e 7365 7474 6572 0a20  t_stdev.setter. 
-00013200: 2020 2064 6566 2066 6974 5f73 7464 6576     def fit_stdev
-00013210: 2873 656c 662c 2076 616c 7565 293a 0a20  (self, value):. 
-00013220: 2020 2020 2020 2069 6620 7479 7065 2876         if type(v
-00013230: 616c 7565 2920 3d3d 2064 6963 743a 0a20  alue) == dict:. 
-00013240: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00013250: 5f66 6974 5f73 7464 6576 203d 2076 616c  _fit_stdev = val
-00013260: 7565 0a20 2020 2020 2020 2065 6c73 653a  ue.        else:
-00013270: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-00013280: 7365 2054 7970 6545 7272 6f72 0a20 2020  se TypeError.   
-00013290: 2020 2020 2072 6574 7572 6e0a 0a20 2020       return..   
-000132a0: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-000132b0: 6566 2066 6978 5f76 6172 7328 7365 6c66  ef fix_vars(self
-000132c0: 2920 2d3e 2066 6c6f 6174 3a0a 2020 2020  ) -> float:.    
-000132d0: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
-000132e0: 5061 7261 6d65 7465 7273 2074 6f20 6669  Parameters to fi
-000132f0: 7820 2869 2e65 2e20 6e6f 7420 6669 7429  x (i.e. not fit)
-00013300: 0a20 2020 2020 2020 206b 6579 7320 6172  .        keys ar
-00013310: 6520 6e61 6d65 7320 696e 2050 4152 4e41  e names in PARNA
-00013320: 4d45 532c 2076 616c 7565 7320 6172 6520  MES, values are 
-00013330: 7661 6c75 6573 0a20 2020 2020 2020 2027  values.        '
-00013340: 2727 0a20 2020 2020 2020 2023 2043 6865  ''.        # Che
-00013350: 636b 2066 6f72 2069 6d70 6c65 6d65 6e74  ck for implement
-00013360: 6174 696f 6e20 696e 204d 6f64 656c 2063  ation in Model c
-00013370: 6c61 7373 2069 6e69 740a 2020 2020 2020  lass init.      
-00013380: 2020 7265 7475 726e 2073 656c 662e 5f66    return self._f
-00013390: 6978 5f76 6172 730a 0a20 2020 2040 6669  ix_vars..    @fi
-000133a0: 785f 7661 7273 2e73 6574 7465 720a 2020  x_vars.setter.  
-000133b0: 2020 6465 6620 6669 785f 7661 7273 2873    def fix_vars(s
-000133c0: 656c 662c 2076 616c 7565 293a 0a20 2020  elf, value):.   
-000133d0: 2020 2020 2069 6620 7479 7065 2876 616c       if type(val
-000133e0: 7565 2920 3d3d 2064 6963 743a 0a20 2020  ue) == dict:.   
-000133f0: 2020 2020 2020 2020 2069 6620 616e 7928           if any(
-00013400: 5b6b 6579 206e 6f74 2069 6e20 7365 6c66  [key not in self
-00013410: 2e50 4152 4e41 4d45 5320 666f 7220 6b65  .PARNAMES for ke
-00013420: 7920 696e 2076 616c 7565 2e6b 6579 7328  y in value.keys(
-00013430: 295d 293a 0a20 2020 2020 2020 2020 2020  )]):.           
-00013440: 2020 2020 2072 6169 7365 204b 6579 4572       raise KeyEr
-00013450: 726f 7228 2755 6e6b 6e6f 776e 2076 6172  ror('Unknown var
-00013460: 6961 626c 6520 6e61 6d65 7320 7072 6f76  iable names prov
-00013470: 6964 6564 2074 6f20 6669 7827 290a 2020  ided to fix').  
-00013480: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00013490: 6669 785f 7661 7273 203d 2076 616c 7565  fix_vars = value
-000134a0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-000134b0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-000134c0: 2054 7970 6545 7272 6f72 2827 6669 7820   TypeError('fix 
-000134d0: 6d75 7374 2062 6520 6469 6374 696f 6e61  must be dictiona
-000134e0: 7279 2729 0a20 2020 2020 2020 2072 6574  ry').        ret
-000134f0: 7572 6e0a 0a20 2020 2040 7072 6f70 6572  urn..    @proper
-00013500: 7479 0a20 2020 2064 6566 2066 6974 5f76  ty.    def fit_v
-00013510: 6172 7328 7365 6c66 2920 2d3e 2066 6c6f  ars(self) -> flo
-00013520: 6174 3a0a 2020 2020 2020 2020 2727 270a  at:.        '''.
-00013530: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-00013540: 7273 2074 6f20 6669 740a 2020 2020 2020  rs to fit.      
-00013550: 2020 6b65 7973 2061 7265 206e 616d 6573    keys are names
-00013560: 2069 6e20 5041 524e 414d 4553 2c20 7661   in PARNAMES, va
-00013570: 6c75 6573 2061 7265 2076 616c 7565 730a  lues are values.
-00013580: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
-00013590: 2020 2020 2320 4368 6563 6b20 666f 7220      # Check for 
-000135a0: 696d 706c 656d 656e 7461 7469 6f6e 2069  implementation i
-000135b0: 6e20 4d6f 6465 6c20 636c 6173 7320 696e  n Model class in
-000135c0: 6974 0a20 2020 2020 2020 2072 6574 7572  it.        retur
-000135d0: 6e20 7365 6c66 2e5f 6669 745f 7661 7273  n self._fit_vars
-000135e0: 0a0a 2020 2020 4066 6974 5f76 6172 732e  ..    @fit_vars.
-000135f0: 7365 7474 6572 0a20 2020 2064 6566 2066  setter.    def f
-00013600: 6974 5f76 6172 7328 7365 6c66 2c20 7661  it_vars(self, va
-00013610: 6c75 6529 3a0a 2020 2020 2020 2020 6966  lue):.        if
-00013620: 2074 7970 6528 7661 6c75 6529 203d 3d20   type(value) == 
-00013630: 6469 6374 3a0a 2020 2020 2020 2020 2020  dict:.          
-00013640: 2020 6966 2061 6e79 285b 6b65 7920 6e6f    if any([key no
-00013650: 7420 696e 2073 656c 662e 5041 524e 414d  t in self.PARNAM
-00013660: 4553 2066 6f72 206b 6579 2069 6e20 7661  ES for key in va
-00013670: 6c75 652e 6b65 7973 2829 5d29 3a0a 2020  lue.keys()]):.  
-00013680: 2020 2020 2020 2020 2020 2020 2020 7261                ra
-00013690: 6973 6520 4b65 7945 7272 6f72 2827 556e  ise KeyError('Un
-000136a0: 6b6e 6f77 6e20 7661 7269 6162 6c65 206e  known variable n
-000136b0: 616d 6573 2070 726f 7669 6465 6420 746f  ames provided to
-000136c0: 2066 6974 2729 0a20 2020 2020 2020 2020   fit').         
-000136d0: 2020 2073 656c 662e 5f66 6974 5f76 6172     self._fit_var
-000136e0: 7320 3d20 7661 6c75 650a 2020 2020 2020  s = value.      
-000136f0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00013700: 2020 2020 7261 6973 6520 5479 7065 4572      raise TypeEr
-00013710: 726f 7228 2746 6974 206d 7573 7420 6265  ror('Fit must be
-00013720: 2064 6963 7469 6f6e 6172 7927 290a 2020   dictionary').  
-00013730: 2020 2020 2020 7265 7475 726e 0a0a 2020        return..  
-00013740: 2020 4063 6c61 7373 6d65 7468 6f64 0a20    @classmethod. 
-00013750: 2020 2064 6566 2072 6573 6964 7561 6c73     def residuals
-00013760: 2863 6c73 2c20 7061 7261 6d73 3a20 6469  (cls, params: di
-00013770: 6374 5b73 7472 2c20 666c 6f61 745d 2c20  ct[str, float], 
-00013780: 7465 6d70 6572 6174 7572 6573 3a20 6e70  temperatures: np
-00013790: 742e 4172 7261 794c 696b 652c 0a20 2020  t.ArrayLike,.   
-000137a0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-000137b0: 7275 655f 6c6f 6772 6174 653a 206e 7074  rue_lograte: npt
-000137c0: 2e41 7272 6179 4c69 6b65 2920 2d3e 206e  .ArrayLike) -> n
-000137d0: 7074 2e4e 4441 7272 6179 3a0a 2020 2020  pt.NDArray:.    
-000137e0: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
-000137f0: 4361 6c63 756c 6174 6573 2064 6966 6665  Calculates diffe
-00013800: 7265 6e63 6520 6265 7477 6565 6e20 6d65  rence between me
-00013810: 6173 7572 6564 206c 6f67 3130 2872 656c  asured log10(rel
-00013820: 6178 6174 696f 6e20 7261 7465 2920 616e  axation rate) an
-00013830: 6420 7472 6961 6c0a 2020 2020 2020 2020  d trial.        
-00013840: 6672 6f6d 206d 6f64 656c 0a0a 2020 2020  from model..    
-00013850: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-00013860: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
-00013870: 2d0a 2020 2020 2020 2020 7061 7261 6d73  -.        params
-00013880: 3a20 6172 7261 795f 6c69 6b65 0a20 2020  : array_like.   
-00013890: 2020 2020 2020 2020 206d 6f64 656c 2070           model p
-000138a0: 6172 616d 6574 6572 2076 616c 7565 730a  arameter values.
-000138b0: 2020 2020 2020 2020 7465 6d70 6572 6174          temperat
-000138c0: 7572 6573 3a20 6172 7261 795f 6c69 6b65  ures: array_like
-000138d0: 0a20 2020 2020 2020 2020 2020 2054 656d  .            Tem
-000138e0: 7065 7261 7475 7265 2076 616c 7565 7320  perature values 
-000138f0: 284b 2920 6174 2077 6869 6368 206d 6f64  (K) at which mod
-00013900: 656c 2066 756e 6374 696f 6e20 6973 2065  el function is e
-00013910: 7661 6c75 6174 6564 0a20 2020 2020 2020  valuated.       
-00013920: 2074 7275 655f 6c6f 6772 6174 653a 2061   true_lograte: a
-00013930: 7272 6179 5f6c 696b 650a 2020 2020 2020  rray_like.      
-00013940: 2020 2020 2020 7472 7565 2028 6578 7065        true (expe
-00013950: 7269 6d65 6e74 616c 2920 7661 6c75 6573  rimental) values
-00013960: 206f 6620 6c6f 6731 3028 7265 6c61 7861   of log10(relaxa
-00013970: 7469 6f6e 2072 6174 6529 0a0a 2020 2020  tion rate)..    
-00013980: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-00013990: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-000139a0: 2020 2020 6e64 6172 7261 7920 6f66 2066      ndarray of f
-000139b0: 6c6f 6174 730a 2020 2020 2020 2020 2020  loats.          
-000139c0: 2020 5265 7369 6475 616c 730a 2020 2020    Residuals.    
-000139d0: 2020 2020 2727 270a 0a20 2020 2020 2020      '''..       
-000139e0: 2023 2043 616c 6375 6c61 7465 206d 6f64   # Calculate mod
-000139f0: 656c 206c 6f67 3130 2872 656c 6178 6174  el log10(relaxat
-00013a00: 696f 6e20 7261 7465 2920 7573 696e 6720  ion rate) using 
-00013a10: 7061 7261 6d65 7465 7273 0a20 2020 2020  parameters.     
-00013a20: 2020 2074 7269 616c 5f6c 6f67 7261 7465     trial_lograte
-00013a30: 203d 2063 6c73 2e6d 6f64 656c 2870 6172   = cls.model(par
-00013a40: 616d 732c 2074 656d 7065 7261 7475 7265  ams, temperature
-00013a50: 7329 0a0a 2020 2020 2020 2020 7265 7369  s)..        resi
-00013a60: 6475 616c 7320 3d20 7472 6961 6c5f 6c6f  duals = trial_lo
-00013a70: 6772 6174 6520 2d20 7472 7565 5f6c 6f67  grate - true_log
-00013a80: 7261 7465 0a0a 2020 2020 2020 2020 7265  rate..        re
-00013a90: 7475 726e 2072 6573 6964 7561 6c73 0a0a  turn residuals..
-00013aa0: 2020 2020 4063 6c61 7373 6d65 7468 6f64      @classmethod
-00013ab0: 0a20 2020 2064 6566 2072 6573 6964 7561  .    def residua
-00013ac0: 6c5f 6672 6f6d 5f66 6c6f 6174 5f6c 6973  l_from_float_lis
-00013ad0: 7428 636c 732c 206e 6577 5f76 616c 733a  t(cls, new_vals:
-00013ae0: 206e 7074 2e41 7272 6179 4c69 6b65 2c0a   npt.ArrayLike,.
-00013af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013b10: 2066 6974 5f76 6172 733a 2064 6963 745b   fit_vars: dict[
-00013b20: 7374 722c 2066 6c6f 6174 5d2c 0a20 2020  str, float],.   
-00013b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013b40: 2020 2020 2020 2020 2020 2020 2020 6669                fi
-00013b50: 785f 7661 7273 3a20 6469 6374 5b73 7472  x_vars: dict[str
-00013b60: 2c20 666c 6f61 745d 2c0a 2020 2020 2020  , float],.      
-00013b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013b80: 2020 2020 2020 2020 2020 2074 656d 7065             tempe
-00013b90: 7261 7475 7265 733a 206e 7074 2e41 7272  ratures: npt.Arr
-00013ba0: 6179 4c69 6b65 2c0a 2020 2020 2020 2020  ayLike,.        
-00013bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013bc0: 2020 2020 2020 2020 206c 6f67 7261 7465           lograte
-00013bd0: 3a20 6e70 742e 4172 7261 794c 696b 652c  : npt.ArrayLike,
-00013be0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013c00: 2020 7369 676d 613a 206e 7074 2e41 7272    sigma: npt.Arr
-00013c10: 6179 4c69 6b65 203d 205b 5d29 202d 3e20  ayLike = []) -> 
-00013c20: 6e70 742e 4e44 4172 7261 793a 0a20 2020  npt.NDArray:.   
-00013c30: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
-00013c40: 2057 7261 7070 6572 2066 6f72 2060 7265   Wrapper for `re
-00013c50: 7369 6475 616c 7360 206d 6574 686f 642c  siduals` method,
-00013c60: 2074 616b 6573 206e 6577 2076 616c 7565   takes new value
-00013c70: 7320 6672 6f6d 2073 6369 7079 0a20 2020  s from scipy.   
-00013c80: 2020 2020 206c 6561 7374 5f73 7175 6172       least_squar
-00013c90: 6573 2077 6869 6368 2070 726f 7669 6465  es which provide
-00013ca0: 7320 6c69 7374 5b66 6c6f 6174 5d2c 2074  s list[float], t
-00013cb0: 6f20 636f 6e73 7472 7563 7420 6e65 770a  o construct new.
-00013cc0: 2020 2020 2020 2020 6669 745f 7661 7273          fit_vars
-00013cd0: 2064 6963 742c 2074 6865 6e20 7275 6e73   dict, then runs
-00013ce0: 2060 7265 7369 6475 616c 7360 206d 6574   `residuals` met
-00013cf0: 686f 642e 0a0a 2020 2020 2020 2020 5061  hod...        Pa
-00013d00: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
-00013d10: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-00013d20: 2020 2020 6e65 775f 7661 6c73 3a20 6172      new_vals: ar
-00013d30: 7261 795f 6c69 6b65 0a20 2020 2020 2020  ray_like.       
-00013d40: 2020 2020 2054 6869 7320 6974 6572 6174       This iterat
-00013d50: 696f 6e27 7320 6669 7420 7061 7261 6d65  ion's fit parame
-00013d60: 7465 7220 7661 6c75 6573 2070 726f 7669  ter values provi
-00013d70: 6465 6420 6279 206c 6561 7374 5f73 7175  ded by least_squ
-00013d80: 6172 6573 0a20 2020 2020 2020 2020 2020  ares.           
-00013d90: 2074 6869 7320 6861 7320 7468 6520 7361   this has the sa
-00013da0: 6d65 206f 7264 6572 2061 7420 6669 745f  me order at fit_
-00013db0: 7661 7273 2e6b 6579 730a 2020 2020 2020  vars.keys.      
-00013dc0: 2020 6669 745f 7661 7273 3a20 6469 6374    fit_vars: dict
-00013dd0: 5b73 7472 2c20 666c 6f61 745d 0a20 2020  [str, float].   
-00013de0: 2020 2020 2020 2020 2050 6172 616d 6574           Paramet
-00013df0: 6572 2074 6f20 6669 7420 696e 206d 6f64  er to fit in mod
-00013e00: 656c 2066 756e 6374 696f 6e5c 6e0a 2020  el function\n.  
-00013e10: 2020 2020 2020 2020 2020 6b65 7973 2061            keys a
-00013e20: 7265 2050 4152 4e41 4d45 532c 2076 616c  re PARNAMES, val
-00013e30: 7565 7320 6172 6520 666c 6f61 7420 7661  ues are float va
-00013e40: 6c75 6573 0a20 2020 2020 2020 2066 6978  lues.        fix
-00013e50: 5f76 6172 733a 2064 6963 745b 7374 722c  _vars: dict[str,
-00013e60: 2066 6c6f 6174 5d0a 2020 2020 2020 2020   float].        
-00013e70: 2020 2020 5061 7261 6d65 7465 7220 7768      Parameter wh
-00013e80: 6963 6820 7265 6d61 696e 2066 6978 6564  ich remain fixed
-00013e90: 2069 6e20 6d6f 6465 6c20 6675 6e63 7469   in model functi
-00013ea0: 6f6e 5c6e 0a20 2020 2020 2020 2020 2020  on\n.           
-00013eb0: 206b 6579 7320 6172 6520 5041 524e 414d   keys are PARNAM
-00013ec0: 4553 2c20 7661 6c75 6573 2061 7265 2066  ES, values are f
-00013ed0: 6c6f 6174 2076 616c 7565 730a 2020 2020  loat values.    
-00013ee0: 2020 2020 7465 6d70 6572 6174 7572 6573      temperatures
-00013ef0: 3a20 6172 7261 795f 6c69 6b65 0a20 2020  : array_like.   
-00013f00: 2020 2020 2020 2020 2054 656d 7065 7261           Tempera
-00013f10: 7475 7265 2076 616c 7565 7320 284b 2920  ture values (K) 
-00013f20: 6174 2077 6869 6368 206d 6f64 656c 2066  at which model f
-00013f30: 756e 6374 696f 6e20 6973 2065 7661 6c75  unction is evalu
-00013f40: 6174 6564 0a20 2020 2020 2020 206c 6f67  ated.        log
-00013f50: 7261 7465 3a20 6172 7261 795f 6c69 6b65  rate: array_like
-00013f60: 0a20 2020 2020 2020 2020 2020 2054 7275  .            Tru
-00013f70: 6520 2865 7870 6572 696d 656e 7461 6c29  e (experimental)
-00013f80: 2076 616c 7565 7320 6f66 206c 6f67 3130   values of log10
-00013f90: 2872 656c 6178 6174 696f 6e20 7261 7465  (relaxation rate
-00013fa0: 290a 2020 2020 2020 2020 7369 676d 613a  ).        sigma:
-00013fb0: 2061 7272 6179 5f6c 696b 650a 2020 2020   array_like.    
-00013fc0: 2020 2020 2020 2020 5374 616e 6461 7264          Standard
-00013fd0: 2064 6576 6961 7469 6f6e 206f 6620 7461   deviation of ta
-00013fe0: 7520 696e 206c 6f67 7370 6163 650a 0a20  u in logspace.. 
-00013ff0: 2020 2020 2020 2052 6574 7572 6e73 0a20         Returns. 
-00014000: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0a20         -------. 
-00014010: 2020 2020 2020 206e 6461 7272 6179 206f         ndarray o
-00014020: 6620 666c 6f61 7473 0a20 2020 2020 2020  f floats.       
-00014030: 2020 2020 2052 6573 6964 7561 6c73 0a20       Residuals. 
-00014040: 2020 2020 2020 2027 2727 0a0a 2020 2020         '''..    
-00014050: 2020 2020 2320 5377 6170 2066 6974 2076      # Swap fit v
-00014060: 616c 7565 7320 666f 7220 6e65 7720 7661  alues for new va
-00014070: 6c75 6573 2066 726f 6d20 6669 7420 726f  lues from fit ro
-00014080: 7574 696e 650a 2020 2020 2020 2020 6e65  utine.        ne
-00014090: 775f 6669 745f 7661 7273 203d 207b 0a20  w_fit_vars = {. 
-000140a0: 2020 2020 2020 2020 2020 206e 616d 653a             name:
-000140b0: 2067 7565 7373 0a20 2020 2020 2020 2020   guess.         
-000140c0: 2020 2066 6f72 2067 7565 7373 2c20 6e61     for guess, na
-000140d0: 6d65 2069 6e20 7a69 7028 6e65 775f 7661  me in zip(new_va
-000140e0: 6c73 2c20 6669 745f 7661 7273 2e6b 6579  ls, fit_vars.key
-000140f0: 7328 2929 0a20 2020 2020 2020 207d 0a0a  s()).        }..
-00014100: 2020 2020 2020 2020 2320 416e 6420 6d61          # And ma
-00014110: 6b65 2063 6f6d 6269 6e65 6420 6469 6374  ke combined dict
-00014120: 206f 6620 6669 7420 616e 6420 6669 7865   of fit and fixe
-00014130: 640a 2020 2020 2020 2020 2320 7661 7269  d.        # vari
-00014140: 6162 6c65 206e 616d 6573 2028 6b65 7973  able names (keys
-00014150: 2920 616e 6420 7661 6c75 6573 0a20 2020  ) and values.   
-00014160: 2020 2020 2061 6c6c 5f76 6172 7320 3d20       all_vars = 
-00014170: 7b2a 2a66 6978 5f76 6172 732c 202a 2a6e  {**fix_vars, **n
-00014180: 6577 5f66 6974 5f76 6172 737d 0a0a 2020  ew_fit_vars}..  
-00014190: 2020 2020 2020 7265 7369 6475 616c 7320        residuals 
-000141a0: 3d20 636c 732e 7265 7369 6475 616c 7328  = cls.residuals(
-000141b0: 616c 6c5f 7661 7273 2c20 7465 6d70 6572  all_vars, temper
-000141c0: 6174 7572 6573 2c20 6c6f 6772 6174 6529  atures, lograte)
-000141d0: 0a0a 2020 2020 2020 2020 6966 206c 656e  ..        if len
-000141e0: 2873 6967 6d61 293a 0a20 2020 2020 2020  (sigma):.       
-000141f0: 2020 2020 2072 6573 6964 7561 6c73 202f       residuals /
-00014200: 3d20 7369 676d 610a 0a20 2020 2020 2020  = sigma..       
-00014210: 2072 6574 7572 6e20 7265 7369 6475 616c   return residual
-00014220: 730a 0a20 2020 2064 6566 2066 6974 5f74  s..    def fit_t
-00014230: 6f28 7365 6c66 2c20 6461 7461 7365 743a  o(self, dataset:
-00014240: 2054 6175 5444 6174 6173 6574 2c0a 2020   TauTDataset,.  
-00014250: 2020 2020 2020 2020 2020 2020 2067 7565               gue
-00014260: 7373 3a20 7374 7220 7c20 6469 6374 5b73  ss: str | dict[s
-00014270: 7472 2c20 666c 6f61 745d 203d 2027 7072  tr, float] = 'pr
-00014280: 6564 6566 696e 6564 272c 0a20 2020 2020  edefined',.     
-00014290: 2020 2020 2020 2020 2020 7665 7262 6f73            verbos
-000142a0: 653a 2062 6f6f 6c20 3d20 5472 7565 2920  e: bool = True) 
-000142b0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-000142c0: 2027 2727 0a20 2020 2020 2020 2046 6974   '''.        Fit
-000142d0: 7320 6d6f 6465 6c20 746f 2044 6174 6173  s model to Datas
-000142e0: 6574 0a0a 2020 2020 2020 2020 5061 7261  et..        Para
-000142f0: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
-00014300: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
-00014310: 2020 6461 7461 7365 743a 2054 6175 5444    dataset: TauTD
-00014320: 6174 6173 6574 0a20 2020 2020 2020 2020  ataset.         
-00014330: 2020 2044 6174 6173 6574 2074 6f20 7768     Dataset to wh
-00014340: 6963 6820 6120 6d6f 6465 6c20 6f66 2072  ich a model of r
-00014350: 6174 6520 7673 2074 656d 7065 7261 7475  ate vs temperatu
-00014360: 7265 2077 696c 6c20 6265 2066 6974 7465  re will be fitte
-00014370: 640a 2020 2020 2020 2020 6775 6573 733a  d.        guess:
-00014380: 2073 7472 207c 2064 6963 745b 7374 722c   str | dict[str,
-00014390: 2066 6c6f 6174 5d2c 2064 6566 6175 6c74   float], default
-000143a0: 2027 7072 6564 6566 696e 6564 270a 2020   'predefined'.  
-000143b0: 2020 2020 2020 2020 2020 4569 7468 6572            Either
-000143c0: 2073 7472 696e 6720 2770 7265 6465 6669   string 'predefi
-000143d0: 6e65 6427 2c20 6f72 2064 6963 7420 6f66  ned', or dict of
-000143e0: 2069 6e69 7469 616c 2070 6172 616d 6574   initial paramet
-000143f0: 6572 730a 2020 2020 2020 2020 2020 2020  ers.            
-00014400: 7573 6564 2061 7320 7374 6172 7469 6e67  used as starting
-00014410: 2067 7565 7373 2077 6974 6820 6b65 7973   guess with keys
-00014420: 2061 7320 7061 7261 6d65 7465 7220 6e61   as parameter na
-00014430: 6d65 7320 616e 6420 7661 6c75 6573 2061  mes and values a
-00014440: 730a 2020 2020 2020 2020 2020 2020 6e75  s.            nu
-00014450: 6d65 7269 6361 6c20 7661 6c75 6573 0a20  merical values. 
-00014460: 2020 2020 2020 2076 6572 626f 7365 3a20         verbose: 
-00014470: 626f 6f6c 2c20 6465 6661 756c 7420 5472  bool, default Tr
-00014480: 7565 0a20 2020 2020 2020 2020 2020 2049  ue.            I
-00014490: 6620 5472 7565 2c20 7072 696e 7473 2069  f True, prints i
-000144a0: 6e66 6f72 6d61 7469 6f6e 2074 6f20 7465  nformation to te
-000144b0: 726d 696e 616c 0a0a 2020 2020 2020 2020  rminal..        
-000144c0: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
-000144d0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-000144e0: 4e6f 6e65 0a20 2020 2020 2020 2027 2727  None.        '''
-000144f0: 0a0a 2020 2020 2020 2020 2320 4765 7420  ..        # Get 
-00014500: 7374 6172 7469 6e67 2067 7565 7373 6573  starting guesses
-00014510: 2c20 6569 7468 6572 2070 7265 6465 6669  , either predefi
-00014520: 6e65 6420 696e 2073 656c 6620 6f72 2067  ned in self or g
-00014530: 6976 656e 0a20 2020 2020 2020 2023 2062  iven.        # b
-00014540: 7920 7573 6572 0a20 2020 2020 2020 2069  y user.        i
-00014550: 6620 6775 6573 7320 213d 2027 7072 6564  f guess != 'pred
-00014560: 6566 696e 6564 273a 0a20 2020 2020 2020  efined':.       
-00014570: 2020 2020 2067 7565 7373 203d 205b 0a20       guess = [. 
-00014580: 2020 2020 2020 2020 2020 2020 2020 2067                 g
-00014590: 7565 7373 5b6b 6579 5d20 666f 7220 6b65  uess[key] for ke
-000145a0: 7920 696e 2073 656c 662e 6669 745f 7661  y in self.fit_va
-000145b0: 7273 2e6b 6579 7328 290a 2020 2020 2020  rs.keys().      
-000145c0: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
-000145d0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-000145e0: 2020 6775 6573 7320 3d20 5b76 616c 2066    guess = [val f
-000145f0: 6f72 2076 616c 2069 6e20 7365 6c66 2e66  or val in self.f
-00014600: 6974 5f76 6172 732e 7661 6c75 6573 2829  it_vars.values()
-00014610: 5d0a 0a20 2020 2020 2020 2023 2047 6574  ]..        # Get
-00014620: 2062 6f75 6e64 7320 666f 7220 7661 7269   bounds for vari
-00014630: 6162 6c65 7320 746f 2062 6520 6669 7474  ables to be fitt
-00014640: 6564 0a20 2020 2020 2020 2062 6f75 6e64  ed.        bound
-00014650: 7320 3d20 6e70 2e61 7272 6179 285b 0a20  s = np.array([. 
-00014660: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00014670: 424f 554e 4453 5b6e 616d 655d 0a20 2020  BOUNDS[name].   
-00014680: 2020 2020 2020 2020 2066 6f72 206e 616d           for nam
-00014690: 6520 696e 2073 656c 662e 6669 745f 7661  e in self.fit_va
-000146a0: 7273 2e6b 6579 7328 290a 2020 2020 2020  rs.keys().      
-000146b0: 2020 5d29 2e54 0a0a 2020 2020 2020 2020    ]).T..        
-000146c0: 6375 7272 5f66 6974 203d 206c 6561 7374  curr_fit = least
-000146d0: 5f73 7175 6172 6573 280a 2020 2020 2020  _squares(.      
-000146e0: 2020 2020 2020 7365 6c66 2e72 6573 6964        self.resid
-000146f0: 7561 6c5f 6672 6f6d 5f66 6c6f 6174 5f6c  ual_from_float_l
-00014700: 6973 742c 0a20 2020 2020 2020 2020 2020  ist,.           
-00014710: 2061 7267 733d 5b0a 2020 2020 2020 2020   args=[.        
-00014720: 2020 2020 2020 2020 7365 6c66 2e66 6974          self.fit
-00014730: 5f76 6172 732c 0a20 2020 2020 2020 2020  _vars,.         
-00014740: 2020 2020 2020 2073 656c 662e 6669 785f         self.fix_
-00014750: 7661 7273 2c0a 2020 2020 2020 2020 2020  vars,.          
-00014760: 2020 2020 2020 6461 7461 7365 742e 7465        dataset.te
-00014770: 6d70 6572 6174 7572 6573 2c0a 2020 2020  mperatures,.    
-00014780: 2020 2020 2020 2020 2020 2020 6e70 2e6c              np.l
-00014790: 6f67 3130 2864 6174 6173 6574 2e72 6174  og10(dataset.rat
-000147a0: 6573 292c 0a20 2020 2020 2020 2020 2020  es),.           
-000147b0: 2020 2020 2064 6174 6173 6574 2e6c 6f67       dataset.log
-000147c0: 7261 7465 5f70 6d0a 2020 2020 2020 2020  rate_pm.        
-000147d0: 2020 2020 5d2c 0a20 2020 2020 2020 2020      ],.         
-000147e0: 2020 2078 303d 6775 6573 732c 0a20 2020     x0=guess,.   
-000147f0: 2020 2020 2020 2020 2062 6f75 6e64 733d           bounds=
-00014800: 626f 756e 6473 0a20 2020 2020 2020 2029  bounds.        )
-00014810: 0a0a 2020 2020 2020 2020 6966 2063 7572  ..        if cur
-00014820: 725f 6669 742e 7374 6174 7573 203d 3d20  r_fit.status == 
-00014830: 303a 0a20 2020 2020 2020 2020 2020 2069  0:.            i
-00014840: 6620 7665 7262 6f73 653a 0a20 2020 2020  f verbose:.     
-00014850: 2020 2020 2020 2020 2020 2075 742e 6370             ut.cp
-00014860: 7269 6e74 280a 2020 2020 2020 2020 2020  rint(.          
-00014870: 2020 2020 2020 2020 2020 275c 6e20 4669            '\n Fi
-00014880: 7420 6661 696c 6564 202d 2054 6f6f 206d  t failed - Too m
-00014890: 616e 7920 6974 6572 6174 696f 6e73 272c  any iterations',
-000148a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000148b0: 2020 2020 2027 626c 6163 6b5f 7965 6c6c       'black_yell
-000148c0: 6f77 6267 270a 2020 2020 2020 2020 2020  owbg'.          
-000148d0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-000148e0: 2020 2020 2073 656c 662e 6669 6e61 6c5f       self.final_
-000148f0: 7661 725f 7661 6c75 6573 203d 207b 0a20  var_values = {. 
-00014900: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00014910: 616d 653a 2076 616c 7565 0a20 2020 2020  ame: value.     
-00014920: 2020 2020 2020 2020 2020 2066 6f72 206e             for n
-00014930: 616d 652c 2076 616c 7565 2069 6e20 7a69  ame, value in zi
-00014940: 7028 7365 6c66 2e66 6974 5f76 6172 732c  p(self.fit_vars,
-00014950: 2063 7572 725f 6669 742e 7829 0a20 2020   curr_fit.x).   
-00014960: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-00014970: 2020 2020 2020 2073 656c 662e 6669 745f         self.fit_
-00014980: 7374 6465 7620 3d20 7b0a 2020 2020 2020  stdev = {.      
-00014990: 2020 2020 2020 2020 2020 6c61 6265 6c3a            label:
-000149a0: 206e 702e 6e61 6e0a 2020 2020 2020 2020   np.nan.        
-000149b0: 2020 2020 2020 2020 666f 7220 6c61 6265          for labe
-000149c0: 6c20 696e 2073 656c 662e 6669 745f 7661  l in self.fit_va
-000149d0: 7273 2e6b 6579 7328 290a 2020 2020 2020  rs.keys().      
-000149e0: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-000149f0: 2020 2020 7365 6c66 2e66 6974 5f73 7461      self.fit_sta
-00014a00: 7475 7320 3d20 4661 6c73 650a 2020 2020  tus = False.    
-00014a10: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00014a20: 2020 2020 2020 7374 6465 762c 206e 6f5f        stdev, no_
-00014a30: 7374 6465 7620 3d20 7374 6174 732e 7376  stdev = stats.sv
-00014a40: 645f 7374 6465 7628 6375 7272 5f66 6974  d_stdev(curr_fit
-00014a50: 290a 0a20 2020 2020 2020 2020 2020 2023  )..            #
-00014a60: 2053 7461 6e64 6172 6420 6465 7669 6174   Standard deviat
-00014a70: 696f 6e20 6572 726f 7220 6f6e 2074 6865  ion error on the
-00014a80: 2070 6172 616d 6574 6572 730a 2020 2020   parameters.    
-00014a90: 2020 2020 2020 2020 7365 6c66 2e66 6974          self.fit
-00014aa0: 5f73 7464 6576 203d 207b 0a20 2020 2020  _stdev = {.     
-00014ab0: 2020 2020 2020 2020 2020 206c 6162 656c             label
-00014ac0: 3a20 7661 6c0a 2020 2020 2020 2020 2020  : val.          
-00014ad0: 2020 2020 2020 666f 7220 6c61 6265 6c2c        for label,
-00014ae0: 2076 616c 2069 6e20 7a69 7028 7365 6c66   val in zip(self
-00014af0: 2e66 6974 5f76 6172 732e 6b65 7973 2829  .fit_vars.keys()
-00014b00: 2c20 7374 6465 7629 0a20 2020 2020 2020  , stdev).       
-00014b10: 2020 2020 207d 0a0a 2020 2020 2020 2020       }..        
-00014b20: 2020 2020 7365 6c66 2e66 6974 5f73 7461      self.fit_sta
-00014b30: 7475 7320 3d20 5472 7565 0a0a 2020 2020  tus = True..    
-00014b40: 2020 2020 2020 2020 2320 5265 706f 7274          # Report
-00014b50: 2073 696e 6775 6c61 7220 7661 6c75 6573   singular values
-00014b60: 3d30 206f 6620 4a61 636f 6269 616e 0a20  =0 of Jacobian. 
-00014b70: 2020 2020 2020 2020 2020 2023 2061 6e64             # and
-00014b80: 2069 6e64 6963 6174 6520 7468 6174 2073   indicate that s
-00014b90: 7464 5f64 6576 2063 616e 6e6f 7420 6265  td_dev cannot be
-00014ba0: 2063 616c 6375 6c61 7465 640a 2020 2020   calculated.    
-00014bb0: 2020 2020 2020 2020 666f 7220 7061 722c          for par,
-00014bc0: 2073 6920 696e 207a 6970 2873 656c 662e   si in zip(self.
-00014bd0: 6669 745f 7661 7273 2e6b 6579 7328 292c  fit_vars.keys(),
-00014be0: 206e 6f5f 7374 6465 7629 3a0a 2020 2020   no_stdev):.    
-00014bf0: 2020 2020 2020 2020 2020 2020 6966 2076              if v
-00014c00: 6572 626f 7365 2061 6e64 206e 6f74 2073  erbose and not s
-00014c10: 693a 0a20 2020 2020 2020 2020 2020 2020  i:.             
-00014c20: 2020 2020 2020 2075 742e 6370 7269 6e74         ut.cprint
-00014c30: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00014c40: 2020 2020 2020 2020 2020 6627 5761 726e            f'Warn
-00014c50: 696e 673a 204a 6163 6f62 6961 6e20 6973  ing: Jacobian is
-00014c60: 2064 6567 656e 6572 6174 6520 666f 7220   degenerate for 
-00014c70: 7b70 6172 7d2c 2073 7461 6e64 6172 6420  {par}, standard 
-00014c80: 6465 7669 6174 696f 6e20 6361 6e6e 6f74  deviation cannot
-00014c90: 2062 6520 666f 756e 642c 2061 6e64 2069   be found, and i
-00014ca0: 7320 7365 7420 746f 207a 6572 6f5c 6e27  s set to zero\n'
-00014cb0: 2c20 2320 6e6f 7161 0a20 2020 2020 2020  , # noqa.       
-00014cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014cd0: 2027 626c 6163 6b5f 7965 6c6c 6f77 6267   'black_yellowbg
-00014ce0: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
-00014cf0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-00014d00: 2020 2020 2023 2053 6574 2066 6974 7465       # Set fitte
-00014d10: 6420 7661 6c75 6573 0a20 2020 2020 2020  d values.       
-00014d20: 2020 2020 2073 656c 662e 6669 6e61 6c5f       self.final_
-00014d30: 7661 725f 7661 6c75 6573 203d 207b 0a20  var_values = {. 
-00014d40: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00014d50: 616d 653a 2076 616c 7565 0a20 2020 2020  ame: value.     
-00014d60: 2020 2020 2020 2020 2020 2066 6f72 206e             for n
-00014d70: 616d 652c 2076 616c 7565 2069 6e20 7a69  ame, value in zi
-00014d80: 7028 7365 6c66 2e66 6974 5f76 6172 732e  p(self.fit_vars.
-00014d90: 6b65 7973 2829 2c20 6375 7272 5f66 6974  keys(), curr_fit
-00014da0: 2e78 290a 2020 2020 2020 2020 2020 2020  .x).            
-00014db0: 7d0a 2020 2020 2020 2020 2020 2020 2320  }.            # 
-00014dc0: 616e 6420 6669 7865 6420 7661 6c75 6573  and fixed values
-00014dd0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00014de0: 206b 6579 2c20 7661 6c20 696e 2073 656c   key, val in sel
-00014df0: 662e 6669 785f 7661 7273 2e69 7465 6d73  f.fix_vars.items
-00014e00: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00014e10: 2020 2020 7365 6c66 2e66 696e 616c 5f76      self.final_v
-00014e20: 6172 5f76 616c 7565 735b 6b65 795d 203d  ar_values[key] =
-00014e30: 2076 616c 0a0a 2020 2020 2020 2020 7265   val..        re
-00014e40: 7475 726e 0a0a 0a63 6c61 7373 204c 6f67  turn...class Log
-00014e50: 4f72 6261 6368 4d6f 6465 6c28 4c6f 6754  OrbachModel(LogT
-00014e60: 6175 544d 6f64 656c 293a 0a20 2020 2027  auTModel):.    '
-00014e70: 2727 0a20 2020 204c 6f67 284f 7262 6163  ''.    Log(Orbac
-00014e80: 6829 204d 6f64 656c 206f 6620 6c6f 6731  h) Model of log1
-00014e90: 3028 5265 6c61 7861 7469 6f6e 2072 6174  0(Relaxation rat
-00014ea0: 6529 2076 7320 7465 6d70 6572 6174 7572  e) vs temperatur
-00014eb0: 650a 2020 2020 2727 270a 0a20 2020 2023  e.    '''..    #
-00014ec0: 3a20 4d6f 6465 6c20 6e61 6d65 0a20 2020  : Model name.   
-00014ed0: 204e 414d 4520 3d20 274f 7262 6163 6827   NAME = 'Orbach'
-00014ee0: 0a20 2020 2023 3a20 4d6f 6465 6c20 6e61  .    #: Model na
-00014ef0: 6d65 2077 6974 6820 6c6f 6720 6272 6163  me with log brac
-00014f00: 6b65 7473 0a20 2020 204c 4e41 4d45 203d  kets.    LNAME =
-00014f10: 2027 4c6f 6728 4f72 6261 6368 2927 0a0a   'Log(Orbach)'..
-00014f20: 2020 2020 233a 204d 6f64 656c 2050 6172      #: Model Par
-00014f30: 616d 6574 6572 206e 616d 6520 7374 7269  ameter name stri
-00014f40: 6e67 730a 2020 2020 5041 524e 414d 4553  ngs.    PARNAMES
-00014f50: 203d 205b 0a20 2020 2020 2020 2027 755f   = [.        'u_
-00014f60: 6566 6627 2c20 2741 272c 0a20 2020 205d  eff', 'A',.    ]
-00014f70: 0a0a 2020 2020 233a 204d 6f64 656c 2050  ..    #: Model P
-00014f80: 6172 616d 6574 6572 206e 616d 6520 6d61  arameter name ma
-00014f90: 7468 6d6f 6465 2073 7472 696e 6773 0a20  thmode strings. 
-00014fa0: 2020 2056 4152 4e41 4d45 535f 4d4d 203d     VARNAMES_MM =
-00014fb0: 207b 0a20 2020 2020 2020 2027 755f 6566   {.        'u_ef
-00014fc0: 6627 3a20 7227 2455 5f5c 6d61 7468 7265  f': r'$U_\mathre
-00014fd0: 6775 6c61 727b 6566 667d 2427 2c0a 2020  gular{eff}$',.  
-00014fe0: 2020 2020 2020 2741 273a 2072 2724 4124        'A': r'$A$
-00014ff0: 270a 2020 2020 7d0a 0a20 2020 2023 3a20  '.    }..    #: 
-00015000: 4d6f 6465 6c20 5061 7261 6d65 7465 7220  Model Parameter 
-00015010: 6e61 6d65 2048 544d 4c20 7374 7269 6e67  name HTML string
-00015020: 730a 2020 2020 5641 524e 414d 4553 5f48  s.    VARNAMES_H
-00015030: 544d 4c20 3d20 7b0a 2020 2020 2020 2020  TML = {.        
-00015040: 2775 5f65 6666 273a 2027 553c 7375 623e  'u_eff': 'U<sub>
-00015050: 6566 663c 2f73 7562 3e27 2c0a 2020 2020  eff</sub>',.    
-00015060: 2020 2020 2741 273a 2027 4127 0a20 2020      'A': 'A'.   
-00015070: 207d 0a0a 2020 2020 233a 204d 6f64 656c   }..    #: Model
-00015080: 2050 6172 616d 6574 6572 2075 6e69 7420   Parameter unit 
-00015090: 7374 7269 6e67 730a 2020 2020 554e 4954  strings.    UNIT
-000150a0: 5320 3d20 7b0a 2020 2020 2020 2020 2775  S = {.        'u
-000150b0: 5f65 6666 273a 2072 274b 272c 0a20 2020  _eff': r'K',.   
-000150c0: 2020 2020 2027 4127 3a20 7227 6c6f 6731       'A': r'log1
-000150d0: 305b 735d 270a 2020 2020 7d0a 0a20 2020  0[s]'.    }..   
-000150e0: 2023 3a20 4d6f 6465 6c20 5061 7261 6d65   #: Model Parame
-000150f0: 7465 7220 756e 6974 206d 6174 686d 6f64  ter unit mathmod
-00015100: 6520 7374 7269 6e67 730a 2020 2020 554e  e strings.    UN
-00015110: 4954 535f 4d4d 203d 207b 0a20 2020 2020  ITS_MM = {.     
-00015120: 2020 2027 755f 6566 6627 3a20 7227 245c     'u_eff': r'$\
-00015130: 6d61 7468 7265 6775 6c61 727b 4b7d 2427  mathregular{K}$'
-00015140: 2c0a 2020 2020 2020 2020 2741 273a 2072  ,.        'A': r
-00015150: 2724 5c6c 6f67 5f5c 6d61 7468 7265 6775  '$\log_\mathregu
-00015160: 6c61 727b 3130 7d5c 6c65 6674 5b5c 6d61  lar{10}\left[\ma
-00015170: 7468 7265 6775 6c61 727b 737d 5c72 6967  thregular{s}\rig
-00015180: 6874 5d24 2720 2320 6e6f 7161 0a20 2020  ht]$' # noqa.   
-00015190: 207d 0a0a 2020 2020 233a 204d 6f64 656c   }..    #: Model
-000151a0: 2050 6172 616d 6574 6572 2075 6e69 7420   Parameter unit 
-000151b0: 4854 4d4c 2073 7472 696e 6773 0a20 2020  HTML strings.   
-000151c0: 2055 4e49 5453 5f48 544d 4c20 3d20 7b0a   UNITS_HTML = {.
-000151d0: 2020 2020 2020 2020 2775 5f65 6666 273a          'u_eff':
-000151e0: 2027 4b27 2c0a 2020 2020 2020 2020 2741   'K',.        'A
-000151f0: 273a 2027 6c6f 673c 7375 623e 3130 3c2f  ': 'log<sub>10</
-00015200: 7375 623e 5b73 5d27 0a20 2020 207d 0a0a  sub>[s]'.    }..
-00015210: 2020 2020 233a 204d 6f64 656c 2070 6172      #: Model par
-00015220: 616d 6574 6572 2062 6f75 6e64 730a 2020  ameter bounds.  
-00015230: 2020 424f 554e 4453 203d 207b 0a20 2020    BOUNDS = {.   
-00015240: 2020 2020 2027 755f 6566 6627 3a20 5b30       'u_eff': [0
-00015250: 2e2c 206e 702e 696e 665d 2c0a 2020 2020  ., np.inf],.    
-00015260: 2020 2020 2741 273a 205b 2d33 302c 2030      'A': [-30, 0
-00015270: 5d0a 2020 2020 7d0a 0a20 2020 2040 7374  ].    }..    @st
-00015280: 6174 6963 6d65 7468 6f64 0a20 2020 2064  aticmethod.    d
-00015290: 6566 2073 6574 5f69 6e69 7469 616c 5f76  ef set_initial_v
-000152a0: 616c 7328 7061 7261 6d5f 6469 6374 3a20  als(param_dict: 
-000152b0: 6469 6374 5b73 7472 2c20 7374 7220 7c20  dict[str, str | 
-000152c0: 666c 6f61 745d 2920 2d3e 2064 6963 745b  float]) -> dict[
-000152d0: 7374 722c 2066 6c6f 6174 5d3a 2023 206e  str, float]: # n
-000152e0: 6f71 610a 2020 2020 2020 2020 2727 270a  oqa.        '''.
-000152f0: 2020 2020 2020 2020 5365 7473 2067 7565          Sets gue
-00015300: 7373 2076 616c 7565 7320 666f 7220 7061  ss values for pa
-00015310: 7261 6d65 7465 7273 2069 6620 7265 7175  rameters if requ
-00015320: 6573 7465 6420 6279 2075 7365 720a 0a20  ested by user.. 
-00015330: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
-00015340: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
-00015350: 2d2d 2d2d 0a20 2020 2020 2020 2070 6172  ----.        par
-00015360: 616d 5f64 6963 743a 2064 6963 745b 7374  am_dict: dict[st
-00015370: 722c 2073 7472 207c 2066 6c6f 6174 5d0a  r, str | float].
-00015380: 2020 2020 2020 2020 2020 2020 4b65 7973              Keys
-00015390: 2061 7265 2066 6974 2f66 6978 2070 6172   are fit/fix par
-000153a0: 616d 6574 6572 206e 616d 6573 2028 7365  ameter names (se
-000153b0: 6520 636c 6173 732e 5041 524e 414d 4553  e class.PARNAMES
-000153c0: 295c 6e0a 2020 2020 2020 2020 2020 2020  )\n.            
-000153d0: 5661 6c75 6573 2061 7265 2065 6974 6865  Values are eithe
-000153e0: 7220 666c 6f61 7420 2861 6374 7561 6c20  r float (actual 
-000153f0: 7661 6c75 6529 206f 7220 7468 6520 7374  value) or the st
-00015400: 7269 6e67 2027 6775 6573 7327 0a0a 2020  ring 'guess'..  
-00015410: 2020 2020 2020 5265 7475 726e 730a 2020        Returns.  
-00015420: 2020 2020 2020 2d2d 2d2d 2d2d 2d0a 2020        -------.  
-00015430: 2020 2020 2020 6469 6374 5b73 7472 2c20        dict[str, 
-00015440: 666c 6f61 745d 0a20 2020 2020 2020 2020  float].         
-00015450: 2020 204b 6579 7320 6172 6520 6669 742f     Keys are fit/
-00015460: 6669 7820 7061 7261 6d65 7465 7220 6e61  fix parameter na
-00015470: 6d65 7320 2873 6565 2063 6c61 7373 2e50  mes (see class.P
-00015480: 4152 4e41 4d45 5329 5c6e 0a20 2020 2020  ARNAMES)\n.     
-00015490: 2020 2020 2020 2056 616c 7565 7320 6172         Values ar
-000154a0: 6520 666c 6f61 7420 2861 6374 7561 6c20  e float (actual 
-000154b0: 7661 6c75 6529 2077 6869 6368 2061 7265  value) which are
-000154c0: 2069 6e69 7469 616c 2076 616c 7565 7320   initial values 
-000154d0: 6f66 0a20 2020 2020 2020 2020 2020 2070  of.            p
-000154e0: 6172 616d 6574 6572 0a20 2020 2020 2020  arameter.       
-000154f0: 2027 2727 0a0a 2020 2020 2020 2020 2320   '''..        # 
-00015500: 4d61 6b65 2063 6f70 792c 2061 6e79 2073  Make copy, any s
-00015510: 7472 2076 616c 7565 7320 7769 6c6c 2062  tr values will b
-00015520: 6520 7265 706c 6163 6564 0a20 2020 2020  e replaced.     
-00015530: 2020 206e 6577 5f70 6172 616d 5f64 6963     new_param_dic
-00015540: 7420 3d20 636f 7079 2e63 6f70 7928 7061  t = copy.copy(pa
-00015550: 7261 6d5f 6469 6374 290a 0a20 2020 2020  ram_dict)..     
-00015560: 2020 2023 2047 7565 7373 6573 0a20 2020     # Guesses.   
-00015570: 2020 2020 2067 7565 7373 6469 6374 203d       guessdict =
-00015580: 207b 0a20 2020 2020 2020 2020 2020 2027   {.            '
-00015590: 755f 6566 6627 3a20 3135 3030 2e2c 0a20  u_eff': 1500.,. 
-000155a0: 2020 2020 2020 2020 2020 2027 4127 3a20             'A': 
-000155b0: 2d31 310a 2020 2020 2020 2020 7d0a 0a20  -11.        }.. 
-000155c0: 2020 2020 2020 2023 2052 6570 6c61 6365         # Replace
-000155d0: 2027 6775 6573 7327 2077 6974 6820 7265   'guess' with re
-000155e0: 6c65 7661 6e74 2067 7565 7373 0a20 2020  levant guess.   
-000155f0: 2020 2020 2066 6f72 2076 6172 2c20 7661       for var, va
-00015600: 6c20 696e 2070 6172 616d 5f64 6963 742e  l in param_dict.
-00015610: 6974 656d 7328 293a 0a20 2020 2020 2020  items():.       
-00015620: 2020 2020 2069 6620 7661 6c20 3d3d 2027       if val == '
-00015630: 6775 6573 7327 3a0a 2020 2020 2020 2020  guess':.        
-00015640: 2020 2020 2020 2020 6e65 775f 7061 7261          new_para
-00015650: 6d5f 6469 6374 5b76 6172 5d20 3d20 6775  m_dict[var] = gu
-00015660: 6573 7364 6963 745b 7661 725d 0a0a 2020  essdict[var]..  
-00015670: 2020 2020 2020 7265 7475 726e 206e 6577        return new
-00015680: 5f70 6172 616d 5f64 6963 740a 0a20 2020  _param_dict..   
-00015690: 2040 7374 6174 6963 6d65 7468 6f64 0a20   @staticmethod. 
-000156a0: 2020 2064 6566 206d 6f64 656c 2870 6172     def model(par
-000156b0: 616d 6574 6572 733a 2064 6963 745b 7374  ameters: dict[st
-000156c0: 722c 2066 6c6f 6174 5d2c 0a20 2020 2020  r, float],.     
-000156d0: 2020 2020 2020 2020 2074 656d 7065 7261           tempera
-000156e0: 7475 7265 733a 206e 7074 2e41 7272 6179  tures: npt.Array
-000156f0: 4c69 6b65 2920 2d3e 206e 7074 2e4e 4441  Like) -> npt.NDA
-00015700: 7272 6179 3a0a 2020 2020 2020 2020 2727  rray:.        ''
-00015710: 270a 2020 2020 2020 2020 4576 616c 7561  '.        Evalua
-00015720: 7465 7320 6c6f 6731 3028 4f72 6261 6368  tes log10(Orbach
-00015730: 2920 6d6f 6465 6c20 6f66 206c 6f67 3130  ) model of log10
-00015740: 2872 656c 6178 6174 696f 6e20 7261 7465  (relaxation rate
-00015750: 290a 2020 2020 2020 2020 7573 696e 6720  ).        using 
-00015760: 7072 6f76 6964 6564 2070 6172 616d 6574  provided paramet
-00015770: 6572 2061 6e64 2074 656d 7065 7261 7475  er and temperatu
-00015780: 7265 2076 616c 7565 732e 0a0a 2020 2020  re values...    
-00015790: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-000157a0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
-000157b0: 2d0a 2020 2020 2020 2020 7061 7261 6d65  -.        parame
-000157c0: 7465 7273 3a20 6469 6374 5b73 7472 2c20  ters: dict[str, 
-000157d0: 666c 6f61 745d 0a20 2020 2020 2020 2020  float].         
-000157e0: 2020 2050 6172 616d 6574 6572 7320 746f     Parameters to
-000157f0: 2075 7365 2069 6e20 6d6f 6465 6c20 6675   use in model fu
-00015800: 6e63 7469 6f6e 2c20 6b65 7973 2061 7265  nction, keys are
-00015810: 2067 6976 656e 2069 6e0a 2020 2020 2020   given in.      
-00015820: 2020 2020 2020 636c 6173 732e 5041 524e        class.PARN
-00015830: 414d 4553 0a20 2020 2020 2020 2074 656d  AMES.        tem
-00015840: 7065 7261 7475 7265 733a 2061 7272 6179  peratures: array
-00015850: 5f6c 696b 650a 2020 2020 2020 2020 2020  _like.          
-00015860: 2020 7465 6d70 6572 6174 7572 6520 7661    temperature va
-00015870: 6c75 6573 2028 4b29 2061 7420 7768 6963  lues (K) at whic
-00015880: 6820 6d6f 6465 6c20 6675 6e63 7469 6f6e  h model function
-00015890: 2069 7320 6576 616c 7561 7465 640a 0a20   is evaluated.. 
-000158a0: 2020 2020 2020 2052 6574 7572 6e73 0a20         Returns. 
-000158b0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0a20         -------. 
-000158c0: 2020 2020 2020 206e 6461 7272 6179 206f         ndarray o
-000158d0: 6620 666c 6f61 7473 0a20 2020 2020 2020  f floats.       
-000158e0: 2020 2020 206c 6f67 3130 2852 656c 6178       log10(Relax
-000158f0: 6174 696f 6e20 7261 7465 2920 6173 2061  ation rate) as a
-00015900: 2066 756e 6374 696f 6e20 6f66 2074 656d   function of tem
-00015910: 7065 7261 7475 7265 0a0a 2020 2020 2020  perature..      
-00015920: 2020 2727 270a 0a20 2020 2020 2020 2075    '''..        u
-00015930: 5f65 6666 203d 2070 6172 616d 6574 6572  _eff = parameter
-00015940: 735b 2775 5f65 6666 275d 0a20 2020 2020  s['u_eff'].     
-00015950: 2020 2061 203d 2070 6172 616d 6574 6572     a = parameter
-00015960: 735b 2741 275d 0a0a 2020 2020 2020 2020  s['A']..        
-00015970: 6c6f 6772 6174 6520 3d20 6e70 2e6c 6f67  lograte = np.log
-00015980: 3130 2831 302a 2a2d 6120 2a20 6e70 2e65  10(10**-a * np.e
-00015990: 7870 282d 755f 6566 6620 2f20 6e70 2e61  xp(-u_eff / np.a
-000159a0: 7361 7272 6179 2874 656d 7065 7261 7475  sarray(temperatu
-000159b0: 7265 7329 2929 0a0a 2020 2020 2020 2020  res)))..        
-000159c0: 7265 7475 726e 206c 6f67 7261 7465 0a0a  return lograte..
-000159d0: 0a63 6c61 7373 204c 6f67 5261 6d61 6e4d  .class LogRamanM
-000159e0: 6f64 656c 284c 6f67 5461 7554 4d6f 6465  odel(LogTauTMode
-000159f0: 6c29 3a0a 2020 2020 2727 270a 2020 2020  l):.    '''.    
-00015a00: 4c6f 6728 5261 6d61 6e29 204d 6f64 656c  Log(Raman) Model
-00015a10: 206f 6620 6c6f 6731 3028 5265 6c61 7861   of log10(Relaxa
-00015a20: 7469 6f6e 2072 6174 6529 2076 7320 7465  tion rate) vs te
-00015a30: 6d70 6572 6174 7572 650a 2020 2020 2727  mperature.    ''
-00015a40: 270a 0a20 2020 2023 3a20 4d6f 6465 6c20  '..    #: Model 
-00015a50: 6e61 6d65 0a20 2020 204e 414d 4520 3d20  name.    NAME = 
-00015a60: 2752 616d 616e 270a 2020 2020 233a 204d  'Raman'.    #: M
-00015a70: 6f64 656c 206e 616d 6520 7769 7468 206c  odel name with l
-00015a80: 6f67 2062 7261 636b 6574 730a 2020 2020  og brackets.    
-00015a90: 4c4e 414d 4520 3d20 274c 6f67 2852 616d  LNAME = 'Log(Ram
-00015aa0: 616e 2927 0a0a 2020 2020 233a 204d 6f64  an)'..    #: Mod
-00015ab0: 656c 2050 6172 616d 6574 6572 206e 616d  el Parameter nam
-00015ac0: 6520 7374 7269 6e67 730a 2020 2020 5041  e strings.    PA
-00015ad0: 524e 414d 4553 203d 205b 0a20 2020 2020  RNAMES = [.     
-00015ae0: 2020 2027 5227 2c20 276e 272c 0a20 2020     'R', 'n',.   
-00015af0: 205d 0a0a 2020 2020 233a 204d 6f64 656c   ]..    #: Model
-00015b00: 2050 6172 616d 6574 6572 206e 616d 6520   Parameter name 
-00015b10: 6d61 7468 6d6f 6465 2073 7472 696e 6773  mathmode strings
-00015b20: 0a20 2020 2056 4152 4e41 4d45 535f 4d4d  .    VARNAMES_MM
-00015b30: 203d 207b 0a20 2020 2020 2020 2027 5227   = {.        'R'
-00015b40: 3a20 7227 2452 2427 2c0a 2020 2020 2020  : r'$R$',.      
-00015b50: 2020 276e 273a 2072 2724 6e24 270a 2020    'n': r'$n$'.  
-00015b60: 2020 7d0a 0a20 2020 2023 3a20 4d6f 6465    }..    #: Mode
-00015b70: 6c20 5061 7261 6d65 7465 7220 6e61 6d65  l Parameter name
-00015b80: 2048 544d 4c20 7374 7269 6e67 730a 2020   HTML strings.  
-00015b90: 2020 5641 524e 414d 4553 5f48 544d 4c20    VARNAMES_HTML 
-00015ba0: 3d20 7b0a 2020 2020 2020 2020 2752 273a  = {.        'R':
-00015bb0: 2027 5227 2c0a 2020 2020 2020 2020 276e   'R',.        'n
-00015bc0: 273a 2027 6e27 0a20 2020 207d 0a0a 2020  ': 'n'.    }..  
-00015bd0: 2020 233a 204d 6f64 656c 2050 6172 616d    #: Model Param
-00015be0: 6574 6572 2075 6e69 7420 7374 7269 6e67  eter unit string
-00015bf0: 730a 2020 2020 554e 4954 5320 3d20 7b0a  s.    UNITS = {.
-00015c00: 2020 2020 2020 2020 2752 273a 2027 6c6f          'R': 'lo
-00015c10: 6731 305b 735e 2d31 204b 5e2d 6e5d 272c  g10[s^-1 K^-n]',
-00015c20: 0a20 2020 2020 2020 2027 6e27 3a20 2727  .        'n': ''
-00015c30: 0a20 2020 207d 0a0a 2020 2020 233a 204d  .    }..    #: M
-00015c40: 6f64 656c 2050 6172 616d 6574 6572 2075  odel Parameter u
-00015c50: 6e69 7420 6d61 7468 6d6f 6465 2073 7472  nit mathmode str
-00015c60: 696e 6773 0a20 2020 2055 4e49 5453 5f4d  ings.    UNITS_M
-00015c70: 4d20 3d20 7b0a 2020 2020 2020 2020 2752  M = {.        'R
-00015c80: 273a 2072 2724 5c6c 6f67 5f5c 6d61 7468  ': r'$\log_\math
-00015c90: 7265 6775 6c61 727b 3130 7d5c 6c65 6674  regular{10}\left
-00015ca0: 5b5c 6d61 7468 7265 6775 6c61 727b 737d  [\mathregular{s}
-00015cb0: 5e5c 6d61 7468 7265 6775 6c61 727b 2d31  ^\mathregular{-1
-00015cc0: 7d20 5c6d 6174 6872 6567 756c 6172 7b4b  } \mathregular{K
-00015cd0: 7d5e 5c6d 6174 6872 6567 756c 6172 7b2d  }^\mathregular{-
-00015ce0: 6e7d 5c72 6967 6874 5d24 272c 2023 206e  n}\right]$', # n
-00015cf0: 6f71 610a 2020 2020 2020 2020 276e 273a  oqa.        'n':
-00015d00: 2027 270a 2020 2020 7d0a 0a20 2020 2023   ''.    }..    #
-00015d10: 3a20 4d6f 6465 6c20 5061 7261 6d65 7465  : Model Paramete
-00015d20: 7220 756e 6974 2048 544d 4c20 7374 7269  r unit HTML stri
-00015d30: 6e67 730a 2020 2020 554e 4954 535f 4854  ngs.    UNITS_HT
-00015d40: 4d4c 203d 207b 0a20 2020 2020 2020 2027  ML = {.        '
-00015d50: 5227 3a20 276c 6f67 3c73 7562 3e31 303c  R': 'log<sub>10<
-00015d60: 2f73 7562 3e5b 733c 7375 703e 2d31 3c2f  /sub>[s<sup>-1</
-00015d70: 7375 703e 204b 3c73 7570 3e2d 6e3c 2f73  sup> K<sup>-n</s
-00015d80: 7570 3e5d 272c 0a20 2020 2020 2020 2027  up>]',.        '
-00015d90: 6e27 3a20 2727 0a20 2020 207d 0a0a 2020  n': ''.    }..  
-00015da0: 2020 233a 204d 6f64 656c 2070 6172 616d    #: Model param
-00015db0: 6574 6572 2062 6f75 6e64 730a 2020 2020  eter bounds.    
-00015dc0: 424f 554e 4453 203d 207b 0a20 2020 2020  BOUNDS = {.     
-00015dd0: 2020 2027 5227 3a20 5b2d 3330 2c20 6e70     'R': [-30, np
-00015de0: 2e69 6e66 5d2c 0a20 2020 2020 2020 2027  .inf],.        '
-00015df0: 6e27 3a20 5b30 2c20 6e70 2e69 6e66 5d0a  n': [0, np.inf].
-00015e00: 2020 2020 7d0a 0a20 2020 2040 7374 6174      }..    @stat
-00015e10: 6963 6d65 7468 6f64 0a20 2020 2064 6566  icmethod.    def
-00015e20: 2073 6574 5f69 6e69 7469 616c 5f76 616c   set_initial_val
-00015e30: 7328 7061 7261 6d5f 6469 6374 3a20 6469  s(param_dict: di
-00015e40: 6374 5b73 7472 2c20 7374 7220 7c20 666c  ct[str, str | fl
-00015e50: 6f61 745d 2920 2d3e 2064 6963 745b 7374  oat]) -> dict[st
-00015e60: 722c 2066 6c6f 6174 5d3a 2023 206e 6f71  r, float]: # noq
-00015e70: 610a 2020 2020 2020 2020 2727 270a 2020  a.        '''.  
-00015e80: 2020 2020 2020 5365 7473 2067 7565 7373        Sets guess
-00015e90: 2076 616c 7565 7320 666f 7220 7061 7261   values for para
-00015ea0: 6d65 7465 7273 2069 6620 7265 7175 6573  meters if reques
-00015eb0: 7465 6420 6279 2075 7365 720a 0a20 2020  ted by user..   
-00015ec0: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
-00015ed0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-00015ee0: 2d2d 0a20 2020 2020 2020 2070 6172 616d  --.        param
-00015ef0: 5f64 6963 743a 2064 6963 745b 7374 722c  _dict: dict[str,
-00015f00: 2073 7472 207c 2066 6c6f 6174 5d0a 2020   str | float].  
-00015f10: 2020 2020 2020 2020 2020 4b65 7973 2061            Keys a
-00015f20: 7265 2066 6974 2f66 6978 2070 6172 616d  re fit/fix param
-00015f30: 6574 6572 206e 616d 6573 2028 7365 6520  eter names (see 
-00015f40: 636c 6173 732e 5041 524e 414d 4553 295c  class.PARNAMES)\
-00015f50: 6e0a 2020 2020 2020 2020 2020 2020 5661  n.            Va
-00015f60: 6c75 6573 2061 7265 2065 6974 6865 7220  lues are either 
-00015f70: 666c 6f61 7420 2861 6374 7561 6c20 7661  float (actual va
-00015f80: 6c75 6529 206f 7220 7468 6520 7374 7269  lue) or the stri
-00015f90: 6e67 2027 6775 6573 7327 0a0a 2020 2020  ng 'guess'..    
-00015fa0: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-00015fb0: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-00015fc0: 2020 2020 6469 6374 5b73 7472 2c20 666c      dict[str, fl
-00015fd0: 6f61 745d 0a20 2020 2020 2020 2020 2020  oat].           
-00015fe0: 204b 6579 7320 6172 6520 6669 742f 6669   Keys are fit/fi
-00015ff0: 7820 7061 7261 6d65 7465 7220 6e61 6d65  x parameter name
-00016000: 7320 2873 6565 2063 6c61 7373 2e50 4152  s (see class.PAR
-00016010: 4e41 4d45 5329 5c6e 0a20 2020 2020 2020  NAMES)\n.       
-00016020: 2020 2020 2056 616c 7565 7320 6172 6520       Values are 
-00016030: 666c 6f61 7420 2861 6374 7561 6c20 7661  float (actual va
-00016040: 6c75 6529 2077 6869 6368 2061 7265 2069  lue) which are i
-00016050: 6e69 7469 616c 2076 616c 7565 7320 6f66  nitial values of
-00016060: 0a20 2020 2020 2020 2020 2020 2070 6172  .            par
-00016070: 616d 6574 6572 0a20 2020 2020 2020 2027  ameter.        '
-00016080: 2727 0a0a 2020 2020 2020 2020 2320 4d61  ''..        # Ma
-00016090: 6b65 2063 6f70 792c 2061 6e79 2073 7472  ke copy, any str
-000160a0: 2076 616c 7565 7320 7769 6c6c 2062 6520   values will be 
-000160b0: 7265 706c 6163 6564 0a20 2020 2020 2020  replaced.       
-000160c0: 206e 6577 5f70 6172 616d 5f64 6963 7420   new_param_dict 
-000160d0: 3d20 636f 7079 2e63 6f70 7928 7061 7261  = copy.copy(para
-000160e0: 6d5f 6469 6374 290a 0a20 2020 2020 2020  m_dict)..       
-000160f0: 2023 2047 7565 7373 6573 0a20 2020 2020   # Guesses.     
-00016100: 2020 2067 7565 7373 6469 6374 203d 207b     guessdict = {
-00016110: 0a20 2020 2020 2020 2020 2020 2027 5227  .            'R'
-00016120: 3a20 2d36 2c0a 2020 2020 2020 2020 2020  : -6,.          
-00016130: 2020 276e 273a 2033 0a20 2020 2020 2020    'n': 3.       
-00016140: 207d 0a0a 2020 2020 2020 2020 2320 5265   }..        # Re
-00016150: 706c 6163 6520 2767 7565 7373 2720 7769  place 'guess' wi
-00016160: 7468 2072 656c 6576 616e 7420 6775 6573  th relevant gues
-00016170: 730a 2020 2020 2020 2020 666f 7220 7661  s.        for va
-00016180: 722c 2076 616c 2069 6e20 7061 7261 6d5f  r, val in param_
-00016190: 6469 6374 2e69 7465 6d73 2829 3a0a 2020  dict.items():.  
-000161a0: 2020 2020 2020 2020 2020 6966 2076 616c            if val
-000161b0: 203d 3d20 2767 7565 7373 273a 0a20 2020   == 'guess':.   
-000161c0: 2020 2020 2020 2020 2020 2020 206e 6577               new
-000161d0: 5f70 6172 616d 5f64 6963 745b 7661 725d  _param_dict[var]
-000161e0: 203d 2067 7565 7373 6469 6374 5b76 6172   = guessdict[var
-000161f0: 5d0a 0a20 2020 2020 2020 2072 6574 7572  ]..        retur
-00016200: 6e20 6e65 775f 7061 7261 6d5f 6469 6374  n new_param_dict
-00016210: 0a0a 2020 2020 4073 7461 7469 636d 6574  ..    @staticmet
-00016220: 686f 640a 2020 2020 6465 6620 6d6f 6465  hod.    def mode
-00016230: 6c28 7061 7261 6d65 7465 7273 3a20 6469  l(parameters: di
-00016240: 6374 5b73 7472 2c20 666c 6f61 745d 2c0a  ct[str, float],.
-00016250: 2020 2020 2020 2020 2020 2020 2020 7465                te
-00016260: 6d70 6572 6174 7572 6573 3a20 6e70 742e  mperatures: npt.
-00016270: 4172 7261 794c 696b 6529 202d 3e20 6e70  ArrayLike) -> np
-00016280: 742e 4e44 4172 7261 793a 0a20 2020 2020  t.NDArray:.     
-00016290: 2020 2027 2727 0a20 2020 2020 2020 2045     '''.        E
-000162a0: 7661 6c75 6174 6573 206c 6f67 3130 2852  valuates log10(R
-000162b0: 616d 616e 2920 6d6f 6465 6c20 6f66 206c  aman) model of l
-000162c0: 6f67 3130 2872 656c 6178 6174 696f 6e20  og10(relaxation 
-000162d0: 7261 7465 290a 2020 2020 2020 2020 7573  rate).        us
-000162e0: 696e 6720 7072 6f76 6964 6564 2070 6172  ing provided par
-000162f0: 616d 6574 6572 2061 6e64 2074 656d 7065  ameter and tempe
-00016300: 7261 7475 7265 2076 616c 7565 732e 0a0a  rature values...
-00016310: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-00016320: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
-00016330: 2d2d 2d2d 2d0a 2020 2020 2020 2020 7061  -----.        pa
-00016340: 7261 6d65 7465 7273 3a20 6469 6374 5b73  rameters: dict[s
-00016350: 7472 2c20 666c 6f61 745d 0a20 2020 2020  tr, float].     
-00016360: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
-00016370: 7320 746f 2075 7365 2069 6e20 6d6f 6465  s to use in mode
-00016380: 6c20 6675 6e63 7469 6f6e 2c20 6b65 7973  l function, keys
-00016390: 2061 7265 2067 6976 656e 2069 6e0a 2020   are given in.  
-000163a0: 2020 2020 2020 2020 2020 636c 6173 732e            class.
-000163b0: 5041 524e 414d 4553 0a20 2020 2020 2020  PARNAMES.       
-000163c0: 2074 656d 7065 7261 7475 7265 733a 2061   temperatures: a
-000163d0: 7272 6179 5f6c 696b 650a 2020 2020 2020  rray_like.      
-000163e0: 2020 2020 2020 7465 6d70 6572 6174 7572        temperatur
-000163f0: 6520 7661 6c75 6573 2028 4b29 2061 7420  e values (K) at 
-00016400: 7768 6963 6820 6d6f 6465 6c20 6675 6e63  which model func
-00016410: 7469 6f6e 2069 7320 6576 616c 7561 7465  tion is evaluate
-00016420: 640a 0a20 2020 2020 2020 2052 6574 7572  d..        Retur
-00016430: 6e73 0a20 2020 2020 2020 202d 2d2d 2d2d  ns.        -----
-00016440: 2d2d 0a20 2020 2020 2020 206e 6461 7272  --.        ndarr
-00016450: 6179 206f 6620 666c 6f61 7473 0a20 2020  ay of floats.   
-00016460: 2020 2020 2020 2020 206c 6f67 3130 2852           log10(R
-00016470: 656c 6178 6174 696f 6e20 7261 7465 2920  elaxation rate) 
-00016480: 6173 2061 2066 756e 6374 696f 6e20 6f66  as a function of
-00016490: 2074 656d 7065 7261 7475 7265 0a0a 2020   temperature..  
-000164a0: 2020 2020 2020 2727 270a 0a20 2020 2020        '''..     
-000164b0: 2020 2072 203d 2070 6172 616d 6574 6572     r = parameter
-000164c0: 735b 2752 275d 0a20 2020 2020 2020 206e  s['R'].        n
-000164d0: 203d 2070 6172 616d 6574 6572 735b 276e   = parameters['n
-000164e0: 275d 0a0a 2020 2020 2020 2020 6c6f 6772  ']..        logr
-000164f0: 6174 6520 3d20 6e70 2e6c 6f67 3130 2831  ate = np.log10(1
-00016500: 302a 2a72 202a 206e 702e 6173 6172 7261  0**r * np.asarra
-00016510: 7928 7465 6d70 6572 6174 7572 6573 292a  y(temperatures)*
-00016520: 2a6e 290a 0a20 2020 2020 2020 2072 6574  *n)..        ret
-00016530: 7572 6e20 6c6f 6772 6174 650a 0a0a 636c  urn lograte...cl
-00016540: 6173 7320 4c6f 6751 544d 4d6f 6465 6c28  ass LogQTMModel(
-00016550: 4c6f 6754 6175 544d 6f64 656c 293a 0a20  LogTauTModel):. 
-00016560: 2020 2027 2727 0a20 2020 204c 6f67 2851     '''.    Log(Q
-00016570: 544d 2920 4d6f 6465 6c20 6f66 206c 6f67  TM) Model of log
-00016580: 3130 2852 656c 6178 6174 696f 6e20 7261  10(Relaxation ra
-00016590: 7465 2920 7673 2074 656d 7065 7261 7475  te) vs temperatu
-000165a0: 7265 0a20 2020 2027 2727 0a20 2020 2023  re.    '''.    #
-000165b0: 3a20 4d6f 6465 6c20 6e61 6d65 0a20 2020  : Model name.   
-000165c0: 204e 414d 4520 3d20 2751 544d 270a 2020   NAME = 'QTM'.  
-000165d0: 2020 233a 204d 6f64 656c 206e 616d 6520    #: Model name 
-000165e0: 7769 7468 206c 6f67 2062 7261 636b 6574  with log bracket
-000165f0: 730a 2020 2020 4c4e 414d 4520 3d20 274c  s.    LNAME = 'L
-00016600: 6f67 2851 544d 2927 0a0a 2020 2020 233a  og(QTM)'..    #:
-00016610: 204d 6f64 656c 2050 6172 616d 6574 6572   Model Parameter
-00016620: 206e 616d 6520 7374 7269 6e67 730a 2020   name strings.  
-00016630: 2020 5041 524e 414d 4553 203d 205b 0a20    PARNAMES = [. 
-00016640: 2020 2020 2020 2027 5127 0a20 2020 205d         'Q'.    ]
-00016650: 0a0a 2020 2020 233a 204d 6f64 656c 2050  ..    #: Model P
-00016660: 6172 616d 6574 6572 206e 616d 6520 6d61  arameter name ma
-00016670: 7468 6d6f 6465 2073 7472 696e 6773 0a20  thmode strings. 
-00016680: 2020 2056 4152 4e41 4d45 535f 4d4d 203d     VARNAMES_MM =
-00016690: 207b 0a20 2020 2020 2020 2027 5127 3a20   {.        'Q': 
-000166a0: 7227 2451 2427 2c0a 2020 2020 7d0a 0a20  r'$Q$',.    }.. 
-000166b0: 2020 2023 3a20 4d6f 6465 6c20 5061 7261     #: Model Para
-000166c0: 6d65 7465 7220 6e61 6d65 2048 544d 4c20  meter name HTML 
-000166d0: 7374 7269 6e67 730a 2020 2020 5641 524e  strings.    VARN
-000166e0: 414d 4553 5f48 544d 4c20 3d20 7b0a 2020  AMES_HTML = {.  
-000166f0: 2020 2020 2020 2751 273a 2027 5127 2c0a        'Q': 'Q',.
-00016700: 2020 2020 7d0a 0a20 2020 2023 3a20 4d6f      }..    #: Mo
-00016710: 6465 6c20 5061 7261 6d65 7465 7220 756e  del Parameter un
-00016720: 6974 2073 7472 696e 6773 0a20 2020 2055  it strings.    U
-00016730: 4e49 5453 203d 207b 0a20 2020 2020 2020  NITS = {.       
-00016740: 2027 5127 3a20 276c 6f67 3130 5b73 5d27   'Q': 'log10[s]'
-00016750: 2c0a 2020 2020 7d0a 0a20 2020 2023 3a20  ,.    }..    #: 
-00016760: 4d6f 6465 6c20 5061 7261 6d65 7465 7220  Model Parameter 
-00016770: 756e 6974 206d 6174 686d 6f64 6520 7374  unit mathmode st
-00016780: 7269 6e67 730a 2020 2020 554e 4954 535f  rings.    UNITS_
-00016790: 4d4d 203d 207b 0a20 2020 2020 2020 2027  MM = {.        '
-000167a0: 5127 3a20 7227 245c 6c6f 675f 5c6d 6174  Q': r'$\log_\mat
-000167b0: 6872 6567 756c 6172 7b31 307d 5c6c 6566  hregular{10}\lef
-000167c0: 745b 5c6d 6174 6872 6567 756c 6172 7b73  t[\mathregular{s
-000167d0: 7d5c 7269 6768 745d 2427 2c0a 2020 2020  }\right]$',.    
-000167e0: 7d0a 0a20 2020 2023 3a20 4d6f 6465 6c20  }..    #: Model 
-000167f0: 5061 7261 6d65 7465 7220 756e 6974 2048  Parameter unit H
-00016800: 544d 4c20 7374 7269 6e67 730a 2020 2020  TML strings.    
-00016810: 554e 4954 535f 4854 4d4c 203d 207b 0a20  UNITS_HTML = {. 
-00016820: 2020 2020 2020 2027 5127 3a20 7227 6c6f         'Q': r'lo
-00016830: 673c 7375 623e 3130 3c2f 7375 623e 5b73  g<sub>10</sub>[s
-00016840: 5d27 0a20 2020 207d 0a0a 2020 2020 233a  ]'.    }..    #:
-00016850: 204d 6f64 656c 2070 6172 616d 6574 6572   Model parameter
-00016860: 2062 6f75 6e64 730a 2020 2020 424f 554e   bounds.    BOUN
-00016870: 4453 203d 207b 0a20 2020 2020 2020 2027  DS = {.        '
-00016880: 5127 3a20 5b2d 3330 2c20 3330 2e5d 0a20  Q': [-30, 30.]. 
-00016890: 2020 207d 0a0a 2020 2020 4073 7461 7469     }..    @stati
-000168a0: 636d 6574 686f 640a 2020 2020 6465 6620  cmethod.    def 
-000168b0: 7365 745f 696e 6974 6961 6c5f 7661 6c73  set_initial_vals
-000168c0: 2870 6172 616d 5f64 6963 743a 2064 6963  (param_dict: dic
-000168d0: 745b 7374 722c 2073 7472 207c 2066 6c6f  t[str, str | flo
-000168e0: 6174 5d29 202d 3e20 6469 6374 5b73 7472  at]) -> dict[str
-000168f0: 2c20 666c 6f61 745d 3a20 2320 6e6f 7161  , float]: # noqa
-00016900: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
-00016910: 2020 2020 2053 6574 7320 6775 6573 7320       Sets guess 
-00016920: 7661 6c75 6573 2066 6f72 2070 6172 616d  values for param
-00016930: 6574 6572 7320 6966 2072 6571 7565 7374  eters if request
-00016940: 6564 2062 7920 7573 6572 0a0a 2020 2020  ed by user..    
-00016950: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-00016960: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
-00016970: 2d0a 2020 2020 2020 2020 7061 7261 6d5f  -.        param_
-00016980: 6469 6374 3a20 6469 6374 5b73 7472 2c20  dict: dict[str, 
-00016990: 7374 7220 7c20 666c 6f61 745d 0a20 2020  str | float].   
-000169a0: 2020 2020 2020 2020 204b 6579 7320 6172           Keys ar
-000169b0: 6520 6669 742f 6669 7820 7061 7261 6d65  e fit/fix parame
-000169c0: 7465 7220 6e61 6d65 7320 2873 6565 2063  ter names (see c
-000169d0: 6c61 7373 2e50 4152 4e41 4d45 5329 5c6e  lass.PARNAMES)\n
-000169e0: 0a20 2020 2020 2020 2020 2020 2056 616c  .            Val
-000169f0: 7565 7320 6172 6520 6569 7468 6572 2066  ues are either f
-00016a00: 6c6f 6174 2028 6163 7475 616c 2076 616c  loat (actual val
-00016a10: 7565 2920 6f72 2074 6865 2073 7472 696e  ue) or the strin
-00016a20: 6720 2767 7565 7373 270a 0a20 2020 2020  g 'guess'..     
-00016a30: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
-00016a40: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
-00016a50: 2020 2064 6963 745b 7374 722c 2066 6c6f     dict[str, flo
-00016a60: 6174 5d0a 2020 2020 2020 2020 2020 2020  at].            
-00016a70: 4b65 7973 2061 7265 2066 6974 2f66 6978  Keys are fit/fix
-00016a80: 2070 6172 616d 6574 6572 206e 616d 6573   parameter names
-00016a90: 2028 7365 6520 636c 6173 732e 5041 524e   (see class.PARN
-00016aa0: 414d 4553 295c 6e0a 2020 2020 2020 2020  AMES)\n.        
-00016ab0: 2020 2020 5661 6c75 6573 2061 7265 2066      Values are f
-00016ac0: 6c6f 6174 2028 6163 7475 616c 2076 616c  loat (actual val
-00016ad0: 7565 2920 7768 6963 6820 6172 6520 696e  ue) which are in
-00016ae0: 6974 6961 6c20 7661 6c75 6573 206f 660a  itial values of.
-00016af0: 2020 2020 2020 2020 2020 2020 7061 7261              para
-00016b00: 6d65 7465 720a 2020 2020 2020 2020 2727  meter.        ''
-00016b10: 270a 0a20 2020 2020 2020 2023 204d 616b  '..        # Mak
-00016b20: 6520 636f 7079 2c20 616e 7920 7374 7220  e copy, any str 
-00016b30: 7661 6c75 6573 2077 696c 6c20 6265 2072  values will be r
-00016b40: 6570 6c61 6365 640a 2020 2020 2020 2020  eplaced.        
-00016b50: 6e65 775f 7061 7261 6d5f 6469 6374 203d  new_param_dict =
-00016b60: 2063 6f70 792e 636f 7079 2870 6172 616d   copy.copy(param
-00016b70: 5f64 6963 7429 0a0a 2020 2020 2020 2020  _dict)..        
-00016b80: 2320 4775 6573 7365 730a 2020 2020 2020  # Guesses.      
-00016b90: 2020 6775 6573 7364 6963 7420 3d20 7b0a    guessdict = {.
-00016ba0: 2020 2020 2020 2020 2020 2020 2751 273a              'Q':
-00016bb0: 2031 0a20 2020 2020 2020 207d 0a0a 2020   1.        }..  
-00016bc0: 2020 2020 2020 2320 5265 706c 6163 6520        # Replace 
-00016bd0: 2767 7565 7373 2720 7769 7468 2072 656c  'guess' with rel
-00016be0: 6576 616e 7420 6775 6573 730a 2020 2020  evant guess.    
-00016bf0: 2020 2020 666f 7220 7661 722c 2076 616c      for var, val
-00016c00: 2069 6e20 7061 7261 6d5f 6469 6374 2e69   in param_dict.i
-00016c10: 7465 6d73 2829 3a0a 2020 2020 2020 2020  tems():.        
-00016c20: 2020 2020 6966 2076 616c 203d 3d20 2767      if val == 'g
-00016c30: 7565 7373 273a 0a20 2020 2020 2020 2020  uess':.         
-00016c40: 2020 2020 2020 206e 6577 5f70 6172 616d         new_param
-00016c50: 5f64 6963 745b 7661 725d 203d 2067 7565  _dict[var] = gue
-00016c60: 7373 6469 6374 5b76 6172 5d0a 0a20 2020  ssdict[var]..   
-00016c70: 2020 2020 2072 6574 7572 6e20 6e65 775f       return new_
-00016c80: 7061 7261 6d5f 6469 6374 0a0a 2020 2020  param_dict..    
-00016c90: 4073 7461 7469 636d 6574 686f 640a 2020  @staticmethod.  
-00016ca0: 2020 6465 6620 6d6f 6465 6c28 7061 7261    def model(para
-00016cb0: 6d65 7465 7273 3a20 6469 6374 5b73 7472  meters: dict[str
-00016cc0: 2c20 666c 6f61 745d 2c0a 2020 2020 2020  , float],.      
-00016cd0: 2020 2020 2020 2020 7465 6d70 6572 6174          temperat
-00016ce0: 7572 6573 3a20 6e70 742e 4172 7261 794c  ures: npt.ArrayL
-00016cf0: 696b 6529 202d 3e20 6e70 742e 4e44 4172  ike) -> npt.NDAr
-00016d00: 7261 793a 0a20 2020 2020 2020 2027 2727  ray:.        '''
-00016d10: 0a20 2020 2020 2020 2045 7661 6c75 6174  .        Evaluat
-00016d20: 6573 206c 6f67 3130 2851 544d 2920 6d6f  es log10(QTM) mo
-00016d30: 6465 6c20 6f66 206c 6f67 3130 2872 656c  del of log10(rel
-00016d40: 6178 6174 696f 6e20 7261 7465 290a 2020  axation rate).  
-00016d50: 2020 2020 2020 7573 696e 6720 7072 6f76        using prov
-00016d60: 6964 6564 2070 6172 616d 6574 6572 2061  ided parameter a
-00016d70: 6e64 2074 656d 7065 7261 7475 7265 2076  nd temperature v
-00016d80: 616c 7565 732e 0a0a 2020 2020 2020 2020  alues...        
-00016d90: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
-00016da0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-00016db0: 2020 2020 2020 7061 7261 6d65 7465 7273        parameters
-00016dc0: 3a20 6469 6374 5b73 7472 2c20 666c 6f61  : dict[str, floa
-00016dd0: 745d 0a20 2020 2020 2020 2020 2020 2050  t].            P
-00016de0: 6172 616d 6574 6572 7320 746f 2075 7365  arameters to use
-00016df0: 2069 6e20 6d6f 6465 6c20 6675 6e63 7469   in model functi
-00016e00: 6f6e 2c20 6b65 7973 2061 7265 2067 6976  on, keys are giv
-00016e10: 656e 2069 6e0a 2020 2020 2020 2020 2020  en in.          
-00016e20: 2020 636c 6173 732e 5041 524e 414d 4553    class.PARNAMES
-00016e30: 0a20 2020 2020 2020 2074 656d 7065 7261  .        tempera
-00016e40: 7475 7265 733a 2061 7272 6179 5f6c 696b  tures: array_lik
-00016e50: 650a 2020 2020 2020 2020 2020 2020 7465  e.            te
-00016e60: 6d70 6572 6174 7572 6520 7661 6c75 6573  mperature values
-00016e70: 2028 4b29 2061 7420 7768 6963 6820 6d6f   (K) at which mo
-00016e80: 6465 6c20 6675 6e63 7469 6f6e 2069 7320  del function is 
-00016e90: 6576 616c 7561 7465 640a 0a20 2020 2020  evaluated..     
-00016ea0: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
-00016eb0: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
-00016ec0: 2020 206e 6461 7272 6179 206f 6620 666c     ndarray of fl
-00016ed0: 6f61 7473 0a20 2020 2020 2020 2020 2020  oats.           
-00016ee0: 206c 6f67 3130 2852 656c 6178 6174 696f   log10(Relaxatio
-00016ef0: 6e20 7261 7465 2920 6173 2061 2066 756e  n rate) as a fun
-00016f00: 6374 696f 6e20 6f66 2074 656d 7065 7261  ction of tempera
-00016f10: 7475 7265 0a0a 2020 2020 2020 2020 2727  ture..        ''
-00016f20: 270a 0a20 2020 2020 2020 2071 203d 2070  '..        q = p
-00016f30: 6172 616d 6574 6572 735b 2751 275d 0a0a  arameters['Q']..
-00016f40: 2020 2020 2020 2020 6c6f 6772 6174 6520          lograte 
-00016f50: 3d20 6e70 2e7a 6572 6f73 286c 656e 2874  = np.zeros(len(t
-00016f60: 656d 7065 7261 7475 7265 7329 2920 2b20  emperatures)) + 
-00016f70: 6e70 2e6c 6f67 3130 2831 302a 2a2d 7129  np.log10(10**-q)
-00016f80: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00016f90: 206c 6f67 7261 7465 0a0a 0a63 6c61 7373   lograte...class
-00016fa0: 204c 6f67 4469 7265 6374 4d6f 6465 6c28   LogDirectModel(
-00016fb0: 4c6f 6754 6175 544d 6f64 656c 293a 0a20  LogTauTModel):. 
-00016fc0: 2020 2027 2727 0a20 2020 204c 6f67 2844     '''.    Log(D
-00016fd0: 6972 6563 7429 204d 6f64 656c 206f 6620  irect) Model of 
-00016fe0: 6c6f 6731 3028 5265 6c61 7861 7469 6f6e  log10(Relaxation
-00016ff0: 2072 6174 6529 2076 7320 7465 6d70 6572   rate) vs temper
-00017000: 6174 7572 650a 2020 2020 2727 270a 2020  ature.    '''.  
-00017010: 2020 233a 204d 6f64 656c 206e 616d 650a    #: Model name.
-00017020: 2020 2020 4e41 4d45 203d 2027 4469 7265      NAME = 'Dire
-00017030: 6374 270a 0a20 2020 2023 3a20 4d6f 6465  ct'..    #: Mode
-00017040: 6c20 6e61 6d65 2077 6974 6820 6c6f 6720  l name with log 
-00017050: 6272 6163 6b65 7473 0a20 2020 204c 4e41  brackets.    LNA
-00017060: 4d45 203d 2027 4c6f 6728 4469 7265 6374  ME = 'Log(Direct
-00017070: 2927 0a0a 2020 2020 233a 204d 6f64 656c  )'..    #: Model
-00017080: 2050 6172 616d 6574 6572 206e 616d 6520   Parameter name 
-00017090: 7374 7269 6e67 730a 2020 2020 5041 524e  strings.    PARN
-000170a0: 414d 4553 203d 205b 0a20 2020 2020 2020  AMES = [.       
-000170b0: 2027 4427 0a20 2020 205d 0a0a 2020 2020   'D'.    ]..    
-000170c0: 233a 204d 6f64 656c 2050 6172 616d 6574  #: Model Paramet
-000170d0: 6572 206e 616d 6520 6d61 7468 6d6f 6465  er name mathmode
-000170e0: 2073 7472 696e 6773 0a20 2020 2056 4152   strings.    VAR
-000170f0: 4e41 4d45 535f 4d4d 203d 207b 0a20 2020  NAMES_MM = {.   
-00017100: 2020 2020 2027 4427 3a20 7227 2444 2427       'D': r'$D$'
-00017110: 2c0a 2020 2020 7d0a 0a20 2020 2023 3a20  ,.    }..    #: 
-00017120: 4d6f 6465 6c20 5061 7261 6d65 7465 7220  Model Parameter 
-00017130: 6e61 6d65 2048 544d 4c20 7374 7269 6e67  name HTML string
-00017140: 730a 2020 2020 5641 524e 414d 4553 5f48  s.    VARNAMES_H
-00017150: 544d 4c20 3d20 7b0a 2020 2020 2020 2020  TML = {.        
-00017160: 2744 273a 2027 4427 0a20 2020 207d 0a0a  'D': 'D'.    }..
-00017170: 2020 2020 233a 204d 6f64 656c 2050 6172      #: Model Par
-00017180: 616d 6574 6572 2075 6e69 7420 7374 7269  ameter unit stri
-00017190: 6e67 730a 2020 2020 554e 4954 5320 3d20  ngs.    UNITS = 
-000171a0: 7b0a 2020 2020 2020 2020 2744 273a 2027  {.        'D': '
-000171b0: 6c6f 6731 305b 732d 3120 4b2d 315d 272c  log10[s-1 K-1]',
-000171c0: 0a20 2020 207d 0a0a 2020 2020 233a 204d  .    }..    #: M
-000171d0: 6f64 656c 2050 6172 616d 6574 6572 2075  odel Parameter u
-000171e0: 6e69 7420 6d61 7468 6d6f 6465 2073 7472  nit mathmode str
-000171f0: 696e 6773 0a20 2020 2055 4e49 5453 5f4d  ings.    UNITS_M
-00017200: 4d20 3d20 7b0a 2020 2020 2020 2020 2744  M = {.        'D
-00017210: 273a 2072 2724 5c6c 6f67 5f5c 6d61 7468  ': r'$\log_\math
-00017220: 7265 6775 6c61 727b 3130 7d5c 6c65 6674  regular{10}\left
-00017230: 5b5c 6d61 7468 7265 6775 6c61 727b 737d  [\mathregular{s}
-00017240: 5e5c 6d61 7468 7265 6775 6c61 727b 2d31  ^\mathregular{-1
-00017250: 7d20 5c6d 6174 6872 6567 756c 6172 7b4b  } \mathregular{K
-00017260: 7d5e 5c6d 6174 6872 6567 756c 6172 7b2d  }^\mathregular{-
-00017270: 317d 5c72 6967 6874 5d24 272c 2023 206e  1}\right]$', # n
-00017280: 6f71 610a 2020 2020 7d0a 0a20 2020 2023  oqa.    }..    #
-00017290: 3a20 4d6f 6465 6c20 5061 7261 6d65 7465  : Model Paramete
-000172a0: 7220 756e 6974 2048 544d 4c20 7374 7269  r unit HTML stri
-000172b0: 6e67 730a 2020 2020 554e 4954 535f 4854  ngs.    UNITS_HT
-000172c0: 4d4c 203d 207b 0a20 2020 2020 2020 2027  ML = {.        '
-000172d0: 4427 3a20 7227 733c 7375 703e 2d31 3c2f  D': r's<sup>-1</
-000172e0: 7375 703e 204b 3c73 7570 3e2d 313c 2f73  sup> K<sup>-1</s
-000172f0: 7570 3e27 0a20 2020 207d 0a0a 2020 2020  up>'.    }..    
-00017300: 233a 204d 6f64 656c 2070 6172 616d 6574  #: Model paramet
-00017310: 6572 2062 6f75 6e64 730a 2020 2020 424f  er bounds.    BO
-00017320: 554e 4453 203d 207b 0a20 2020 2020 2020  UNDS = {.       
-00017330: 2027 4427 3a20 5b2d 3330 2c20 302e 5d0a   'D': [-30, 0.].
-00017340: 2020 2020 7d0a 0a20 2020 2040 7374 6174      }..    @stat
-00017350: 6963 6d65 7468 6f64 0a20 2020 2064 6566  icmethod.    def
-00017360: 2073 6574 5f69 6e69 7469 616c 5f76 616c   set_initial_val
-00017370: 7328 7061 7261 6d5f 6469 6374 3a20 6469  s(param_dict: di
-00017380: 6374 5b73 7472 2c20 7374 7220 7c20 666c  ct[str, str | fl
-00017390: 6f61 745d 2920 2d3e 2064 6963 745b 7374  oat]) -> dict[st
-000173a0: 722c 2066 6c6f 6174 5d3a 2023 206e 6f71  r, float]: # noq
-000173b0: 610a 2020 2020 2020 2020 2727 270a 2020  a.        '''.  
-000173c0: 2020 2020 2020 5365 7473 2067 7565 7373        Sets guess
-000173d0: 2076 616c 7565 7320 666f 7220 7061 7261   values for para
-000173e0: 6d65 7465 7273 2069 6620 7265 7175 6573  meters if reques
-000173f0: 7465 6420 6279 2075 7365 720a 0a20 2020  ted by user..   
-00017400: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
-00017410: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-00017420: 2d2d 0a20 2020 2020 2020 2070 6172 616d  --.        param
-00017430: 5f64 6963 743a 2064 6963 745b 7374 722c  _dict: dict[str,
-00017440: 2073 7472 207c 2066 6c6f 6174 5d0a 2020   str | float].  
-00017450: 2020 2020 2020 2020 2020 4b65 7973 2061            Keys a
-00017460: 7265 2066 6974 2f66 6978 2070 6172 616d  re fit/fix param
-00017470: 6574 6572 206e 616d 6573 2028 7365 6520  eter names (see 
-00017480: 636c 6173 732e 5041 524e 414d 4553 295c  class.PARNAMES)\
-00017490: 6e0a 2020 2020 2020 2020 2020 2020 5661  n.            Va
-000174a0: 6c75 6573 2061 7265 2065 6974 6865 7220  lues are either 
-000174b0: 666c 6f61 7420 2861 6374 7561 6c20 7661  float (actual va
-000174c0: 6c75 6529 206f 7220 7468 6520 7374 7269  lue) or the stri
-000174d0: 6e67 2027 6775 6573 7327 0a0a 2020 2020  ng 'guess'..    
-000174e0: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-000174f0: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-00017500: 2020 2020 6469 6374 5b73 7472 2c20 666c      dict[str, fl
-00017510: 6f61 745d 0a20 2020 2020 2020 2020 2020  oat].           
-00017520: 204b 6579 7320 6172 6520 6669 742f 6669   Keys are fit/fi
-00017530: 7820 7061 7261 6d65 7465 7220 6e61 6d65  x parameter name
-00017540: 7320 2873 6565 2063 6c61 7373 2e50 4152  s (see class.PAR
-00017550: 4e41 4d45 5329 5c6e 0a20 2020 2020 2020  NAMES)\n.       
-00017560: 2020 2020 2056 616c 7565 7320 6172 6520       Values are 
-00017570: 666c 6f61 7420 2861 6374 7561 6c20 7661  float (actual va
-00017580: 6c75 6529 2077 6869 6368 2061 7265 2069  lue) which are i
-00017590: 6e69 7469 616c 2076 616c 7565 7320 6f66  nitial values of
-000175a0: 0a20 2020 2020 2020 2020 2020 2070 6172  .            par
-000175b0: 616d 6574 6572 0a20 2020 2020 2020 2027  ameter.        '
-000175c0: 2727 0a0a 2020 2020 2020 2020 2320 4d61  ''..        # Ma
-000175d0: 6b65 2063 6f70 792c 2061 6e79 2073 7472  ke copy, any str
-000175e0: 2076 616c 7565 7320 7769 6c6c 2062 6520   values will be 
-000175f0: 7265 706c 6163 6564 0a20 2020 2020 2020  replaced.       
-00017600: 206e 6577 5f70 6172 616d 5f64 6963 7420   new_param_dict 
-00017610: 3d20 636f 7079 2e63 6f70 7928 7061 7261  = copy.copy(para
-00017620: 6d5f 6469 6374 290a 0a20 2020 2020 2020  m_dict)..       
-00017630: 2023 2047 7565 7373 6573 0a20 2020 2020   # Guesses.     
-00017640: 2020 2067 7565 7373 6469 6374 203d 207b     guessdict = {
-00017650: 0a20 2020 2020 2020 2020 2020 2027 4427  .            'D'
-00017660: 3a20 2d32 0a20 2020 2020 2020 207d 0a0a  : -2.        }..
-00017670: 2020 2020 2020 2020 2320 5265 706c 6163          # Replac
-00017680: 6520 2767 7565 7373 2720 7769 7468 2072  e 'guess' with r
-00017690: 656c 6576 616e 7420 6775 6573 730a 2020  elevant guess.  
-000176a0: 2020 2020 2020 666f 7220 7661 722c 2076        for var, v
-000176b0: 616c 2069 6e20 7061 7261 6d5f 6469 6374  al in param_dict
-000176c0: 2e69 7465 6d73 2829 3a0a 2020 2020 2020  .items():.      
-000176d0: 2020 2020 2020 6966 2076 616c 203d 3d20        if val == 
-000176e0: 2767 7565 7373 273a 0a20 2020 2020 2020  'guess':.       
-000176f0: 2020 2020 2020 2020 206e 6577 5f70 6172           new_par
-00017700: 616d 5f64 6963 745b 7661 725d 203d 2067  am_dict[var] = g
-00017710: 7565 7373 6469 6374 5b76 6172 5d0a 0a20  uessdict[var].. 
-00017720: 2020 2020 2020 2072 6574 7572 6e20 6e65         return ne
-00017730: 775f 7061 7261 6d5f 6469 6374 0a0a 2020  w_param_dict..  
-00017740: 2020 4073 7461 7469 636d 6574 686f 640a    @staticmethod.
-00017750: 2020 2020 6465 6620 6d6f 6465 6c28 7061      def model(pa
-00017760: 7261 6d65 7465 7273 3a20 6469 6374 5b73  rameters: dict[s
-00017770: 7472 2c20 666c 6f61 745d 2c0a 2020 2020  tr, float],.    
-00017780: 2020 2020 2020 2020 2020 7465 6d70 6572            temper
-00017790: 6174 7572 6573 3a20 6e70 742e 4172 7261  atures: npt.Arra
-000177a0: 794c 696b 6529 202d 3e20 6e70 742e 4e44  yLike) -> npt.ND
-000177b0: 4172 7261 793a 0a20 2020 2020 2020 2027  Array:.        '
-000177c0: 2727 0a20 2020 2020 2020 2045 7661 6c75  ''.        Evalu
-000177d0: 6174 6573 206c 6f67 3130 2844 6972 6563  ates log10(Direc
-000177e0: 7429 206d 6f64 656c 206f 6620 6c6f 6731  t) model of log1
-000177f0: 3028 7265 6c61 7861 7469 6f6e 2072 6174  0(relaxation rat
-00017800: 6529 0a20 2020 2020 2020 2075 7369 6e67  e).        using
-00017810: 2070 726f 7669 6465 6420 7061 7261 6d65   provided parame
-00017820: 7465 7220 616e 6420 7465 6d70 6572 6174  ter and temperat
-00017830: 7572 6520 7661 6c75 6573 2e0a 0a20 2020  ure values...   
-00017840: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
-00017850: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-00017860: 2d2d 0a20 2020 2020 2020 2070 6172 616d  --.        param
-00017870: 6574 6572 733a 2064 6963 745b 7374 722c  eters: dict[str,
-00017880: 2066 6c6f 6174 5d0a 2020 2020 2020 2020   float].        
-00017890: 2020 2020 5061 7261 6d65 7465 7273 2074      Parameters t
-000178a0: 6f20 7573 6520 696e 206d 6f64 656c 2066  o use in model f
-000178b0: 756e 6374 696f 6e2c 206b 6579 7320 6172  unction, keys ar
-000178c0: 6520 6769 7665 6e20 696e 0a20 2020 2020  e given in.     
-000178d0: 2020 2020 2020 2063 6c61 7373 2e50 4152         class.PAR
-000178e0: 4e41 4d45 530a 2020 2020 2020 2020 7465  NAMES.        te
-000178f0: 6d70 6572 6174 7572 6573 3a20 6172 7261  mperatures: arra
-00017900: 795f 6c69 6b65 0a20 2020 2020 2020 2020  y_like.         
-00017910: 2020 2074 656d 7065 7261 7475 7265 2076     temperature v
-00017920: 616c 7565 7320 284b 2920 6174 2077 6869  alues (K) at whi
-00017930: 6368 206d 6f64 656c 2066 756e 6374 696f  ch model functio
-00017940: 6e20 6973 2065 7661 6c75 6174 6564 0a0a  n is evaluated..
-00017950: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
-00017960: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
-00017970: 2020 2020 2020 2020 6e64 6172 7261 7920          ndarray 
-00017980: 6f66 2066 6c6f 6174 730a 2020 2020 2020  of floats.      
-00017990: 2020 2020 2020 6c6f 6731 3028 5265 6c61        log10(Rela
-000179a0: 7861 7469 6f6e 2072 6174 6529 2061 7320  xation rate) as 
-000179b0: 6120 6675 6e63 7469 6f6e 206f 6620 7465  a function of te
-000179c0: 6d70 6572 6174 7572 650a 0a20 2020 2020  mperature..     
-000179d0: 2020 2027 2727 0a0a 2020 2020 2020 2020     '''..        
-000179e0: 6420 3d20 7061 7261 6d65 7465 7273 5b27  d = parameters['
-000179f0: 4427 5d0a 0a20 2020 2020 2020 206c 6f67  D']..        log
-00017a00: 7261 7465 203d 206e 702e 6c6f 6731 3028  rate = np.log10(
-00017a10: 3130 2a2a 6420 2a20 6e70 2e61 7361 7272  10**d * np.asarr
-00017a20: 6179 2874 656d 7065 7261 7475 7265 7329  ay(temperatures)
-00017a30: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-00017a40: 6e20 6c6f 6772 6174 650a 0a0a 636c 6173  n lograte...clas
-00017a50: 7320 4d75 6c74 694c 6f67 5461 7554 4d6f  s MultiLogTauTMo
-00017a60: 6465 6c28 293a 0a20 2020 2027 2727 0a20  del():.    '''. 
-00017a70: 2020 2054 616b 6573 206d 756c 7469 706c     Takes multipl
-00017a80: 6520 4c6f 6754 6175 544d 6f64 656c 206f  e LogTauTModel o
-00017a90: 626a 6563 7473 2061 6e64 2063 6f6d 6269  bjects and combi
-00017aa0: 6e65 7320 696e 746f 2061 2073 696e 676c  nes into a singl
-00017ab0: 6520 6f62 6a65 6374 0a0a 2020 2020 5061  e object..    Pa
-00017ac0: 7261 6d65 7465 7273 0a20 2020 202d 2d2d  rameters.    ---
-00017ad0: 2d2d 2d2d 2d2d 2d0a 2020 2020 6669 745f  -------.    fit_
-00017ae0: 7661 7273 3a20 6c69 7374 5b64 6963 745b  vars: list[dict[
-00017af0: 7374 722c 2066 6c6f 6174 207c 2073 7472  str, float | str
-00017b00: 5d5d 0a20 2020 2020 2020 204c 6973 7420  ]].        List 
-00017b10: 6f66 2066 6974 2064 6963 7473 2c20 7769  of fit dicts, wi
-00017b20: 7468 206b 6579 7320 6173 2050 4152 4e41  th keys as PARNA
-00017b30: 4d45 5320 6f66 2065 6163 6820 4c6f 6754  MES of each LogT
-00017b40: 6175 544d 6f64 656c 0a20 2020 2020 2020  auTModel.       
-00017b50: 2061 6e64 2076 616c 7565 7320 6173 2065   and values as e
-00017b60: 6974 6865 7220 7468 6520 7374 7269 6e67  ither the string
-00017b70: 2027 6775 6573 7327 206f 7220 6120 666c   'guess' or a fl
-00017b80: 6f61 7420 7661 6c75 650a 2020 2020 6669  oat value.    fi
-00017b90: 785f 7661 7273 3a20 6c69 7374 5b64 6963  x_vars: list[dic
-00017ba0: 745b 7374 722c 2066 6c6f 6174 207c 2073  t[str, float | s
-00017bb0: 7472 5d5d 0a20 2020 2020 2020 204c 6973  tr]].        Lis
-00017bc0: 7420 6f66 2066 6978 2064 6963 7473 2c20  t of fix dicts, 
-00017bd0: 7769 7468 206b 6579 7320 6173 2050 4152  with keys as PAR
-00017be0: 4e41 4d45 5320 6f66 2065 6163 6820 4c6f  NAMES of each Lo
-00017bf0: 6754 6175 544d 6f64 656c 0a20 2020 2020  gTauTModel.     
-00017c00: 2020 2061 6e64 2076 616c 7565 7320 6173     and values as
-00017c10: 2065 6974 6865 7220 7468 6520 7374 7269   either the stri
-00017c20: 6e67 2027 6775 6573 7327 206f 7220 6120  ng 'guess' or a 
-00017c30: 666c 6f61 7420 7661 6c75 650a 2020 2020  float value.    
-00017c40: 6c6f 676d 6f64 656c 733a 206c 6973 745b  logmodels: list[
-00017c50: 4c6f 6754 6175 544d 6f64 656c 5d0a 2020  LogTauTModel].  
-00017c60: 2020 2020 2020 4c69 7374 206f 6620 756e        List of un
-00017c70: 696e 7374 616e 7469 6174 6564 204c 6f67  instantiated Log
-00017c80: 5461 7554 4d6f 6465 6c20 6f62 6a65 6374  TauTModel object
-00017c90: 730a 0a20 2020 2041 7474 7269 6275 7465  s..    Attribute
-00017ca0: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  s.    ----------
-00017cb0: 0a20 2020 206c 6f67 6d6f 6465 6c73 3a20  .    logmodels: 
-00017cc0: 6c69 7374 5b4c 6f67 5461 7554 4d6f 6465  list[LogTauTMode
-00017cd0: 6c5d 0a20 2020 2020 2020 204c 6973 7420  l].        List 
-00017ce0: 6f66 204c 6f67 5461 7554 4d6f 6465 6c20  of LogTauTModel 
-00017cf0: 6f62 6a65 6374 730a 2020 2020 4e41 4d45  objects.    NAME
-00017d00: 3a20 7374 720a 2020 2020 2020 2020 4e61  : str.        Na
-00017d10: 6d65 7320 6f66 2065 6163 6820 4c6f 6754  mes of each LogT
-00017d20: 6175 544d 6f64 656c 2063 6f6e 6361 7465  auTModel concate
-00017d30: 6e61 7465 640a 2020 2020 2727 270a 0a20  nated.    '''.. 
-00017d40: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-00017d50: 7365 6c66 2c20 6c6f 676d 6f64 656c 733a  self, logmodels:
-00017d60: 206c 6973 745b 4c6f 6754 6175 544d 6f64   list[LogTauTMod
-00017d70: 656c 5d2c 0a20 2020 2020 2020 2020 2020  el],.           
-00017d80: 2020 2020 2020 6669 745f 7661 7273 3a20        fit_vars: 
-00017d90: 6c69 7374 5b64 6963 745b 7374 722c 2066  list[dict[str, f
-00017da0: 6c6f 6174 207c 2073 7472 5d5d 2c0a 2020  loat | str]],.  
-00017db0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00017dc0: 6978 5f76 6172 733a 206c 6973 745b 6469  ix_vars: list[di
-00017dd0: 6374 5b73 7472 2c20 666c 6f61 7420 7c20  ct[str, float | 
-00017de0: 7374 725d 5d29 202d 3e20 4e6f 6e65 3a0a  str]]) -> None:.
-00017df0: 0a20 2020 2020 2020 2023 2049 6e73 7461  .        # Insta
-00017e00: 6e74 6961 7465 2065 6163 6820 6c6f 676d  ntiate each logm
-00017e10: 6f64 656c 2061 6e64 2063 7265 6174 6520  odel and create 
-00017e20: 6c69 7374 206f 6620 696e 7374 616e 7469  list of instanti
-00017e30: 6174 6564 206c 6f67 6d6f 6465 6c73 0a20  ated logmodels. 
-00017e40: 2020 2020 2020 2073 656c 662e 6c6f 676d         self.logm
-00017e50: 6f64 656c 7320 3d20 7365 6c66 2e70 726f  odels = self.pro
-00017e60: 6365 7373 5f66 6974 6669 7828 6669 745f  cess_fitfix(fit_
-00017e70: 7661 7273 2c20 6669 785f 7661 7273 2c20  vars, fix_vars, 
-00017e80: 6c6f 676d 6f64 656c 7329 0a0a 2020 2020  logmodels)..    
-00017e90: 2020 2020 7365 6c66 2e4e 414d 4520 3d20      self.NAME = 
-00017ea0: 5b6c 6f67 6d6f 6465 6c2e 4e41 4d45 2066  [logmodel.NAME f
-00017eb0: 6f72 206c 6f67 6d6f 6465 6c20 696e 206c  or logmodel in l
-00017ec0: 6f67 6d6f 6465 6c73 5d0a 2020 2020 2020  ogmodels].      
-00017ed0: 2020 7365 6c66 2e4e 414d 4520 3d20 2727    self.NAME = ''
-00017ee0: 2e6a 6f69 6e28 5b27 7b7d 2b27 2e66 6f72  .join(['{}+'.for
-00017ef0: 6d61 7428 6e61 6d65 2920 666f 7220 6e61  mat(name) for na
-00017f00: 6d65 2069 6e20 7365 6c66 2e4e 414d 455d  me in self.NAME]
-00017f10: 295b 3a2d 315d 0a0a 2020 2020 2020 2020  )[:-1]..        
-00017f20: 7365 6c66 2e5f 6669 745f 7374 6174 7573  self._fit_status
-00017f30: 203d 2046 616c 7365 0a0a 2020 2020 2020   = False..      
-00017f40: 2020 7265 7475 726e 0a0a 2020 2020 4070    return..    @p
-00017f50: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-00017f60: 6669 745f 7374 6174 7573 2873 656c 6629  fit_status(self)
-00017f70: 202d 3e20 626f 6f6c 3a0a 2020 2020 2020   -> bool:.      
-00017f80: 2020 2754 7275 6520 6966 2066 6974 2073    'True if fit s
-00017f90: 7563 6365 7373 6675 6c2c 2065 6c73 6520  uccessful, else 
-00017fa0: 4661 6c73 6527 0a20 2020 2020 2020 2072  False'.        r
-00017fb0: 6574 7572 6e20 7365 6c66 2e5f 6669 745f  eturn self._fit_
-00017fc0: 7374 6174 7573 0a0a 2020 2020 4066 6974  status..    @fit
-00017fd0: 5f73 7461 7475 732e 7365 7474 6572 0a20  _status.setter. 
-00017fe0: 2020 2064 6566 2066 6974 5f73 7461 7475     def fit_statu
-00017ff0: 7328 7365 6c66 2c20 7661 6c75 6529 3a0a  s(self, value):.
-00018000: 2020 2020 2020 2020 6966 2074 7970 6528          if type(
-00018010: 7661 6c75 6529 203d 3d20 626f 6f6c 3a0a  value) == bool:.
-00018020: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00018030: 2e5f 6669 745f 7374 6174 7573 203d 2076  ._fit_status = v
-00018040: 616c 7565 0a20 2020 2020 2020 2065 6c73  alue.        els
-00018050: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00018060: 6169 7365 2054 7970 6545 7272 6f72 0a20  aise TypeError. 
-00018070: 2020 2020 2020 2072 6574 7572 6e0a 0a20         return.. 
-00018080: 2020 2040 7374 6174 6963 6d65 7468 6f64     @staticmethod
-00018090: 0a20 2020 2064 6566 2070 726f 6365 7373  .    def process
-000180a0: 5f66 6974 6669 7828 6669 745f 7661 7273  _fitfix(fit_vars
-000180b0: 3a20 6c69 7374 5b64 6963 745b 7374 722c  : list[dict[str,
-000180c0: 2066 6c6f 6174 207c 2073 7472 5d5d 2c0a   float | str]],.
-000180d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000180e0: 2020 2020 2020 2066 6978 5f76 6172 733a         fix_vars:
-000180f0: 206c 6973 745b 6469 6374 5b73 7472 2c20   list[dict[str, 
-00018100: 666c 6f61 7420 7c20 7374 725d 5d2c 0a20  float | str]],. 
-00018110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018120: 2020 2020 2020 6c6f 676d 6f64 656c 733a        logmodels:
-00018130: 206c 6973 745b 4c6f 6754 6175 544d 6f64   list[LogTauTMod
-00018140: 656c 5d29 202d 3e20 6c69 7374 5b4c 6f67  el]) -> list[Log
-00018150: 5461 7554 4d6f 6465 6c5d 3a0a 2020 2020  TauTModel]:.    
-00018160: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
-00018170: 4173 736f 6369 6174 6573 2066 6974 2061  Associates fit a
-00018180: 6e64 2066 6978 2064 6963 7473 2077 6974  nd fix dicts wit
-00018190: 6820 6120 6c69 7374 206f 6620 6c6f 676d  h a list of logm
-000181a0: 6f64 656c 7320 6279 2069 6e73 7461 6e74  odels by instant
-000181b0: 6961 7469 6e67 0a20 2020 2020 2020 2065  iating.        e
-000181c0: 6163 6820 6c6f 676d 6f64 656c 2077 6974  ach logmodel wit
-000181d0: 6820 7468 6520 7370 6563 6966 6965 6420  h the specified 
-000181e0: 7061 7261 6d65 7465 7273 0a0a 2020 2020  parameters..    
-000181f0: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-00018200: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
-00018210: 2d0a 0a20 2020 2020 2020 2066 6974 5f76  -..        fit_v
-00018220: 6172 733a 206c 6973 745b 6469 6374 5b73  ars: list[dict[s
-00018230: 7472 2c20 666c 6f61 7420 7c20 7374 725d  tr, float | str]
-00018240: 5d0a 2020 2020 2020 2020 2020 2020 4c69  ].            Li
-00018250: 7374 206f 6620 6669 7420 6469 6374 732c  st of fit dicts,
-00018260: 2077 6974 6820 6b65 7973 2061 7320 5041   with keys as PA
-00018270: 524e 414d 4553 206f 6620 6561 6368 204c  RNAMES of each L
-00018280: 6f67 5461 7554 4d6f 6465 6c0a 2020 2020  ogTauTModel.    
-00018290: 2020 2020 2020 2020 616e 6420 7661 6c75          and valu
-000182a0: 6573 2061 7320 6569 7468 6572 2074 6865  es as either the
-000182b0: 2073 7472 696e 6720 2767 7565 7373 2720   string 'guess' 
-000182c0: 6f72 2061 2066 6c6f 6174 2076 616c 7565  or a float value
-000182d0: 0a20 2020 2020 2020 2066 6978 5f76 6172  .        fix_var
-000182e0: 733a 206c 6973 745b 6469 6374 5b73 7472  s: list[dict[str
-000182f0: 2c20 666c 6f61 7420 7c20 7374 725d 5d0a  , float | str]].
-00018300: 2020 2020 2020 2020 2020 2020 4c69 7374              List
-00018310: 206f 6620 6669 7820 6469 6374 732c 2077   of fix dicts, w
-00018320: 6974 6820 6b65 7973 2061 7320 5041 524e  ith keys as PARN
-00018330: 414d 4553 206f 6620 6561 6368 204c 6f67  AMES of each Log
-00018340: 5461 7554 4d6f 6465 6c0a 2020 2020 2020  TauTModel.      
-00018350: 2020 2020 2020 616e 6420 7661 6c75 6573        and values
-00018360: 2061 7320 6569 7468 6572 2074 6865 2073   as either the s
-00018370: 7472 696e 6720 2767 7565 7373 2720 6f72  tring 'guess' or
-00018380: 2061 2066 6c6f 6174 2076 616c 7565 0a20   a float value. 
-00018390: 2020 2020 2020 206c 6f67 6d6f 6465 6c73         logmodels
-000183a0: 3a20 6c69 7374 5b4c 6f67 5461 7554 4d6f  : list[LogTauTMo
-000183b0: 6465 6c5d 0a20 2020 2020 2020 2020 2020  del].           
-000183c0: 204c 6973 7420 6f66 2075 6e69 6e73 7461   List of uninsta
-000183d0: 6e74 6961 7465 6420 4c6f 6754 6175 544d  ntiated LogTauTM
-000183e0: 6f64 656c 206f 626a 6563 7473 0a0a 2020  odel objects..  
-000183f0: 2020 2020 2020 5265 7475 726e 730a 2020        Returns.  
-00018400: 2020 2020 2020 2d2d 2d2d 2d2d 2d0a 2020        -------.  
-00018410: 2020 2020 2020 6c69 7374 5b4c 6f67 5461        list[LogTa
-00018420: 7554 4d6f 6465 6c5d 0a20 2020 2020 2020  uTModel].       
-00018430: 2020 2020 2049 6e73 7461 6e74 6961 7465       Instantiate
-00018440: 6420 4c6f 6754 6175 544d 6f64 656c 7320  d LogTauTModels 
-00018450: 7769 7468 2066 6974 2061 6e64 2066 6978  with fit and fix
-00018460: 2064 6963 7473 2061 7070 6c69 6564 0a20   dicts applied. 
-00018470: 2020 2020 2020 2027 2727 0a0a 2020 2020         '''..    
-00018480: 2020 2020 6d61 726b 6564 203d 205b 4661      marked = [Fa
-00018490: 6c73 655d 202a 206c 656e 2866 6974 5f76  lse] * len(fit_v
-000184a0: 6172 7329 0a0a 2020 2020 2020 2020 696e  ars)..        in
-000184b0: 7374 616e 7469 6174 6564 5f6d 6f64 656c  stantiated_model
-000184c0: 7320 3d20 5b5d 0a0a 2020 2020 2020 2020  s = []..        
-000184d0: 666f 7220 6c6f 676d 6f64 656c 2069 6e20  for logmodel in 
-000184e0: 6c6f 676d 6f64 656c 733a 0a20 2020 2020  logmodels:.     
-000184f0: 2020 2020 2020 2066 6f72 2069 742c 2028         for it, (
-00018500: 6669 7476 6172 5f73 6574 2c20 6669 785f  fitvar_set, fix_
-00018510: 7661 725f 7365 7429 2069 6e20 656e 756d  var_set) in enum
-00018520: 6572 6174 6528 7a69 7028 6669 745f 7661  erate(zip(fit_va
-00018530: 7273 2c20 6669 785f 7661 7273 2929 3a20  rs, fix_vars)): 
-00018540: 2320 6e6f 7161 0a20 2020 2020 2020 2020  # noqa.         
-00018550: 2020 2020 2020 2069 6620 6d61 726b 6564         if marked
-00018560: 5b69 745d 3a0a 2020 2020 2020 2020 2020  [it]:.          
-00018570: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
-00018580: 7565 0a20 2020 2020 2020 2020 2020 2020  ue.             
-00018590: 2020 2065 6c69 6620 616c 6c28 5b6b 2069     elif all([k i
-000185a0: 6e20 6c6f 676d 6f64 656c 2e50 4152 4e41  n logmodel.PARNA
-000185b0: 4d45 5320 666f 7220 6b20 696e 2066 6974  MES for k in fit
-000185c0: 7661 725f 7365 742e 6b65 7973 2829 5d29  var_set.keys()])
-000185d0: 3a20 2320 6e6f 7161 0a20 2020 2020 2020  : # noqa.       
-000185e0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000185f0: 616c 6c28 5b6b 2069 6e20 6c6f 676d 6f64  all([k in logmod
-00018600: 656c 2e50 4152 4e41 4d45 5320 666f 7220  el.PARNAMES for 
-00018610: 6b20 696e 2066 6978 5f76 6172 5f73 6574  k in fix_var_set
-00018620: 2e6b 6579 7328 295d 2920 6f72 206e 6f74  .keys()]) or not
-00018630: 206c 656e 2866 6978 5f76 6172 5f73 6574   len(fix_var_set
-00018640: 293a 2023 206e 6f71 610a 2020 2020 2020  ): # noqa.      
-00018650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018660: 2020 696e 7374 616e 7469 6174 6564 5f6d    instantiated_m
-00018670: 6f64 656c 732e 6170 7065 6e64 280a 2020  odels.append(.  
-00018680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018690: 2020 2020 2020 2020 2020 6c6f 676d 6f64            logmod
-000186a0: 656c 2866 6974 7661 725f 7365 742c 2066  el(fitvar_set, f
-000186b0: 6978 5f76 6172 5f73 6574 290a 2020 2020  ix_var_set).    
+0000e000: 2027 6c6f 6731 305b 4f65 5e70 5d27 2c0a   'log10[Oe^p]',.
+0000e010: 2020 2020 2020 2020 2770 273a 2027 270a          'p': ''.
+0000e020: 2020 2020 7d0a 0a20 2020 2023 3a20 4d6f      }..    #: Mo
+0000e030: 6465 6c20 5061 7261 6d65 7465 7220 756e  del Parameter un
+0000e040: 6974 206d 6174 686d 6f64 6520 7374 7269  it mathmode stri
+0000e050: 6e67 730a 2020 2020 554e 4954 535f 4d4d  ngs.    UNITS_MM
+0000e060: 203d 207b 0a20 2020 2020 2020 2027 5127   = {.        'Q'
+0000e070: 3a20 7227 245c 6c6f 675f 5c6d 6174 6872  : r'$\log_\mathr
+0000e080: 6567 756c 6172 7b31 307d 5c6c 6566 745b  egular{10}\left[
+0000e090: 5c6d 6174 6872 6567 756c 6172 7b73 7d5c  \mathregular{s}\
+0000e0a0: 7269 6768 745d 2427 2c0a 2020 2020 2020  right]$',.      
+0000e0b0: 2020 2751 5f48 273a 2072 2724 5c6c 6f67    'Q_H': r'$\log
+0000e0c0: 5f5c 6d61 7468 7265 6775 6c61 727b 3130  _\mathregular{10
+0000e0d0: 7d5c 6c65 6674 5b5c 6d61 7468 7265 6775  }\left[\mathregu
+0000e0e0: 6c61 727b 4f65 7d5e 7b70 7d5c 7269 6768  lar{Oe}^{p}\righ
+0000e0f0: 745d 2427 2c20 2320 6e6f 7161 0a20 2020  t]$', # noqa.   
+0000e100: 2020 2020 2027 7027 3a20 2727 0a20 2020       'p': ''.   
+0000e110: 207d 0a0a 2020 2020 233a 204d 6f64 656c   }..    #: Model
+0000e120: 2050 6172 616d 6574 6572 2075 6e69 7420   Parameter unit 
+0000e130: 4854 4d4c 2073 7472 696e 6773 0a20 2020  HTML strings.   
+0000e140: 2055 4e49 5453 5f48 544d 4c20 3d20 7b0a   UNITS_HTML = {.
+0000e150: 2020 2020 2020 2020 2751 273a 2072 276c          'Q': r'l
+0000e160: 6f67 3c73 7562 3e31 303c 2f73 7562 3e5b  og<sub>10</sub>[
+0000e170: 735d 272c 0a20 2020 2020 2020 2027 515f  s]',.        'Q_
+0000e180: 4827 3a20 7227 6c6f 673c 7375 623e 3130  H': r'log<sub>10
+0000e190: 3c2f 7375 623e 5b4f 653c 7375 703e 703c  </sub>[Oe<sup>p<
+0000e1a0: 2f73 7570 3e5d 272c 0a20 2020 2020 2020  /sup>]',.       
+0000e1b0: 2027 7027 3a20 2727 0a20 2020 207d 0a0a   'p': ''.    }..
+0000e1c0: 2020 2020 233a 204d 6f64 656c 2050 6172      #: Model Par
+0000e1d0: 616d 6574 6572 2062 6f75 6e64 730a 2020  ameter bounds.  
+0000e1e0: 2020 424f 554e 4453 203d 207b 0a20 2020    BOUNDS = {.   
+0000e1f0: 2020 2020 2027 5127 3a20 5b2d 3330 2e2c       'Q': [-30.,
+0000e200: 206e 702e 696e 665d 2c0a 2020 2020 2020   np.inf],.      
+0000e210: 2020 2751 5f48 273a 205b 2d33 302e 2c20    'Q_H': [-30., 
+0000e220: 6e70 2e69 6e66 5d2c 0a20 2020 2020 2020  np.inf],.       
+0000e230: 2027 7027 3a20 5b30 2c20 3130 5d0a 2020   'p': [0, 10].  
+0000e240: 2020 7d0a 0a20 2020 2040 7374 6174 6963    }..    @static
+0000e250: 6d65 7468 6f64 0a20 2020 2064 6566 2073  method.    def s
+0000e260: 6574 5f69 6e69 7469 616c 5f76 616c 7328  et_initial_vals(
+0000e270: 7061 7261 6d5f 6469 6374 3a20 6469 6374  param_dict: dict
+0000e280: 5b73 7472 2c20 7374 7220 7c20 666c 6f61  [str, str | floa
+0000e290: 745d 2920 2d3e 2064 6963 745b 7374 722c  t]) -> dict[str,
+0000e2a0: 2066 6c6f 6174 5d3a 2023 206e 6f71 610a   float]: # noqa.
+0000e2b0: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
+0000e2c0: 2020 2020 5365 7473 2067 7565 7373 2076      Sets guess v
+0000e2d0: 616c 7565 7320 666f 7220 7061 7261 6d65  alues for parame
+0000e2e0: 7465 7273 2069 6620 7265 7175 6573 7465  ters if requeste
+0000e2f0: 6420 6279 2075 7365 720a 0a20 2020 2020  d by user..     
+0000e300: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+0000e310: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
+0000e320: 0a20 2020 2020 2020 2070 6172 616d 5f64  .        param_d
+0000e330: 6963 743a 2064 6963 745b 7374 722c 2073  ict: dict[str, s
+0000e340: 7472 207c 2066 6c6f 6174 5d0a 2020 2020  tr | float].    
+0000e350: 2020 2020 2020 2020 4b65 7973 2061 7265          Keys are
+0000e360: 2066 6974 2f66 6978 2070 6172 616d 6574   fit/fix paramet
+0000e370: 6572 206e 616d 6573 2028 7365 6520 636c  er names (see cl
+0000e380: 6173 732e 5041 524e 414d 4553 295c 6e0a  ass.PARNAMES)\n.
+0000e390: 2020 2020 2020 2020 2020 2020 5661 6c75              Valu
+0000e3a0: 6573 2061 7265 2065 6974 6865 7220 666c  es are either fl
+0000e3b0: 6f61 7420 2861 6374 7561 6c20 7661 6c75  oat (actual valu
+0000e3c0: 6529 206f 7220 7468 6520 7374 7269 6e67  e) or the string
+0000e3d0: 2027 6775 6573 7327 0a0a 2020 2020 2020   'guess'..      
+0000e3e0: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
+0000e3f0: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
+0000e400: 2020 6469 6374 5b73 7472 2c20 666c 6f61    dict[str, floa
+0000e410: 745d 0a20 2020 2020 2020 2020 2020 204b  t].            K
+0000e420: 6579 7320 6172 6520 6669 742f 6669 7820  eys are fit/fix 
+0000e430: 7061 7261 6d65 7465 7220 6e61 6d65 7320  parameter names 
+0000e440: 2873 6565 2063 6c61 7373 2e50 4152 4e41  (see class.PARNA
+0000e450: 4d45 5329 5c6e 0a20 2020 2020 2020 2020  MES)\n.         
+0000e460: 2020 2056 616c 7565 7320 6172 6520 666c     Values are fl
+0000e470: 6f61 7420 2861 6374 7561 6c20 7661 6c75  oat (actual valu
+0000e480: 6529 2077 6869 6368 2061 7265 2069 6e69  e) which are ini
+0000e490: 7469 616c 2076 616c 7565 7320 6f66 0a20  tial values of. 
+0000e4a0: 2020 2020 2020 2020 2020 2070 6172 616d             param
+0000e4b0: 6574 6572 0a20 2020 2020 2020 2027 2727  eter.        '''
+0000e4c0: 0a0a 2020 2020 2020 2020 2320 4d61 6b65  ..        # Make
+0000e4d0: 2063 6f70 792c 2061 6e79 2073 7472 2076   copy, any str v
+0000e4e0: 616c 7565 7320 7769 6c6c 2062 6520 7265  alues will be re
+0000e4f0: 706c 6163 6564 0a20 2020 2020 2020 206e  placed.        n
+0000e500: 6577 5f70 6172 616d 5f64 6963 7420 3d20  ew_param_dict = 
+0000e510: 636f 7079 2e63 6f70 7928 7061 7261 6d5f  copy.copy(param_
+0000e520: 6469 6374 290a 0a20 2020 2020 2020 2023  dict)..        #
+0000e530: 2047 7565 7373 6573 0a20 2020 2020 2020   Guesses.       
+0000e540: 2067 7565 7373 6469 6374 203d 207b 0a20   guessdict = {. 
+0000e550: 2020 2020 2020 2020 2020 2027 5127 3a20             'Q': 
+0000e560: 2d32 2c0a 2020 2020 2020 2020 2020 2020  -2,.            
+0000e570: 2751 5f48 273a 202d 322c 0a20 2020 2020  'Q_H': -2,.     
+0000e580: 2020 2020 2020 2027 7027 3a20 320a 2020         'p': 2.  
+0000e590: 2020 2020 2020 7d0a 0a20 2020 2020 2020        }..       
+0000e5a0: 2023 2052 6570 6c61 6365 2027 6775 6573   # Replace 'gues
+0000e5b0: 7327 2077 6974 6820 7265 6c65 7661 6e74  s' with relevant
+0000e5c0: 2067 7565 7373 0a20 2020 2020 2020 2066   guess.        f
+0000e5d0: 6f72 2076 6172 2c20 7661 6c20 696e 2070  or var, val in p
+0000e5e0: 6172 616d 5f64 6963 742e 6974 656d 7328  aram_dict.items(
+0000e5f0: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
+0000e600: 6620 7661 6c20 3d3d 2027 6775 6573 7327  f val == 'guess'
+0000e610: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000e620: 2020 6e65 775f 7061 7261 6d5f 6469 6374    new_param_dict
+0000e630: 5b76 6172 5d20 3d20 6775 6573 7364 6963  [var] = guessdic
+0000e640: 745b 7661 725d 0a0a 2020 2020 2020 2020  t[var]..        
+0000e650: 7265 7475 726e 206e 6577 5f70 6172 616d  return new_param
+0000e660: 5f64 6963 740a 0a20 2020 2040 7374 6174  _dict..    @stat
+0000e670: 6963 6d65 7468 6f64 0a20 2020 2064 6566  icmethod.    def
+0000e680: 206d 6f64 656c 2870 6172 616d 6574 6572   model(parameter
+0000e690: 733a 2064 6963 745b 7374 722c 2066 6c6f  s: dict[str, flo
+0000e6a0: 6174 5d2c 0a20 2020 2020 2020 2020 2020  at],.           
+0000e6b0: 2020 2066 6965 6c64 733a 206e 7074 2e41     fields: npt.A
+0000e6c0: 7272 6179 4c69 6b65 2920 2d3e 206e 7074  rrayLike) -> npt
+0000e6d0: 2e4e 4441 7272 6179 3a0a 2020 2020 2020  .NDArray:.      
+0000e6e0: 2020 2727 270a 2020 2020 2020 2020 4576    '''.        Ev
+0000e6f0: 616c 7561 7465 7320 6c6f 6731 3028 4644  aluates log10(FD
+0000e700: 2d51 544d 2920 6d6f 6465 6c20 6f66 206c  -QTM) model of l
+0000e710: 6f67 3130 2872 656c 6178 6174 696f 6e20  og10(relaxation 
+0000e720: 7261 7465 290a 2020 2020 2020 2020 7573  rate).        us
+0000e730: 696e 6720 7072 6f76 6964 6564 2070 6172  ing provided par
+0000e740: 616d 6574 6572 2061 6e64 2066 6965 6c64  ameter and field
+0000e750: 2076 616c 7565 732e 0a0a 2020 2020 2020   values...      
+0000e760: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+0000e770: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a       ----------.
+0000e780: 2020 2020 2020 2020 7061 7261 6d65 7465          paramete
+0000e790: 7273 3a20 6469 6374 5b73 7472 2c20 666c  rs: dict[str, fl
+0000e7a0: 6f61 745d 0a20 2020 2020 2020 2020 2020  oat].           
+0000e7b0: 2050 6172 616d 6574 6572 7320 746f 2075   Parameters to u
+0000e7c0: 7365 2069 6e20 6d6f 6465 6c20 6675 6e63  se in model func
+0000e7d0: 7469 6f6e 2c20 6b65 7973 2061 7265 2067  tion, keys are g
+0000e7e0: 6976 656e 2069 6e0a 2020 2020 2020 2020  iven in.        
+0000e7f0: 2020 2020 636c 6173 732e 5041 524e 414d      class.PARNAM
+0000e800: 4553 0a20 2020 2020 2020 2066 6965 6c64  ES.        field
+0000e810: 733a 2061 7272 6179 5f6c 696b 650a 2020  s: array_like.  
+0000e820: 2020 2020 2020 2020 2020 6669 656c 6420            field 
+0000e830: 7661 6c75 6573 2028 4f65 2920 6174 2077  values (Oe) at w
+0000e840: 6869 6368 206d 6f64 656c 2066 756e 6374  hich model funct
+0000e850: 696f 6e20 6973 2065 7661 6c75 6174 6564  ion is evaluated
+0000e860: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+0000e870: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+0000e880: 2d0a 2020 2020 2020 2020 6e64 6172 7261  -.        ndarra
+0000e890: 7920 6f66 2066 6c6f 6174 730a 2020 2020  y of floats.    
+0000e8a0: 2020 2020 2020 2020 6c6f 6731 3028 5265          log10(Re
+0000e8b0: 6c61 7861 7469 6f6e 2072 6174 6529 2061  laxation rate) a
+0000e8c0: 7320 6120 6675 6e63 7469 6f6e 206f 6620  s a function of 
+0000e8d0: 6669 656c 640a 0a20 2020 2020 2020 2027  field..        '
+0000e8e0: 2727 0a0a 2020 2020 2020 2020 7120 3d20  ''..        q = 
+0000e8f0: 7061 7261 6d65 7465 7273 5b27 5127 5d0a  parameters['Q'].
+0000e900: 2020 2020 2020 2020 7168 203d 2070 6172          qh = par
+0000e910: 616d 6574 6572 735b 2751 5f48 275d 0a20  ameters['Q_H']. 
+0000e920: 2020 2020 2020 2070 203d 2070 6172 616d         p = param
+0000e930: 6574 6572 735b 2770 275d 0a0a 2020 2020  eters['p']..    
+0000e940: 2020 2020 6c6f 6772 6174 6520 3d20 6e70      lograte = np
+0000e950: 2e6c 6f67 3130 2831 302a 2a2d 7120 2f20  .log10(10**-q / 
+0000e960: 2831 202b 2031 302a 2a2d 7168 202a 206e  (1 + 10**-qh * n
+0000e970: 702e 6173 6172 7261 7928 6669 656c 6473  p.asarray(fields
+0000e980: 292a 2a70 2929 0a0a 2020 2020 2020 2020  )**p))..        
+0000e990: 7265 7475 726e 206c 6f67 7261 7465 0a0a  return lograte..
+0000e9a0: 0a63 6c61 7373 204c 6f67 5261 6d61 6e49  .class LogRamanI
+0000e9b0: 494d 6f64 656c 284c 6f67 5461 7548 4d6f  IModel(LogTauHMo
+0000e9c0: 6465 6c29 3a0a 2020 2020 2727 270a 2020  del):.    '''.  
+0000e9d0: 2020 4c6f 6728 5261 6d61 6e2d 4949 2920    Log(Raman-II) 
+0000e9e0: 4d6f 6465 6c20 6f66 206c 6f67 3130 2852  Model of log10(R
+0000e9f0: 656c 6178 6174 696f 6e20 7261 7465 2920  elaxation rate) 
+0000ea00: 7673 2066 6965 6c64 0a20 2020 2027 2727  vs field.    '''
+0000ea10: 0a0a 2020 2020 233a 204d 6f64 656c 206e  ..    #: Model n
+0000ea20: 616d 650a 2020 2020 4e41 4d45 203d 2027  ame.    NAME = '
+0000ea30: 5261 6d61 6e2d 4949 270a 0a20 2020 2023  Raman-II'..    #
+0000ea40: 3a20 4d6f 6465 6c20 6e61 6d65 2077 6974  : Model name wit
+0000ea50: 6820 6c6f 6720 6272 6163 6b65 7473 0a20  h log brackets. 
+0000ea60: 2020 204c 4e41 4d45 203d 2027 4c6f 6728     LNAME = 'Log(
+0000ea70: 5261 6d61 6e2d 4949 2927 0a0a 2020 2020  Raman-II)'..    
+0000ea80: 233a 204d 6f64 656c 2050 6172 616d 6574  #: Model Paramet
+0000ea90: 6572 206e 616d 6520 7374 7269 6e67 730a  er name strings.
+0000eaa0: 2020 2020 5041 524e 414d 4553 203d 205b      PARNAMES = [
+0000eab0: 0a20 2020 2020 2020 2027 4327 2c0a 2020  .        'C',.  
+0000eac0: 2020 2020 2020 276d 272c 0a20 2020 205d        'm',.    ]
+0000ead0: 0a0a 2020 2020 233a 204d 6f64 656c 2050  ..    #: Model P
+0000eae0: 6172 616d 6574 6572 206e 616d 6520 6d61  arameter name ma
+0000eaf0: 7468 6d6f 6465 2073 7472 696e 6773 0a20  thmode strings. 
+0000eb00: 2020 2056 4152 4e41 4d45 535f 4d4d 203d     VARNAMES_MM =
+0000eb10: 207b 0a20 2020 2020 2020 2027 4327 3a20   {.        'C': 
+0000eb20: 2724 4324 272c 0a20 2020 2020 2020 2027  '$C$',.        '
+0000eb30: 6d27 3a20 2724 6d24 270a 2020 2020 7d0a  m': '$m$'.    }.
+0000eb40: 0a20 2020 2023 3a20 4d6f 6465 6c20 5061  .    #: Model Pa
+0000eb50: 7261 6d65 7465 7220 6e61 6d65 2048 544d  rameter name HTM
+0000eb60: 4c20 7374 7269 6e67 730a 2020 2020 5641  L strings.    VA
+0000eb70: 524e 414d 4553 5f48 544d 4c20 3d20 7b0a  RNAMES_HTML = {.
+0000eb80: 2020 2020 2020 2020 2743 273a 2027 4327          'C': 'C'
+0000eb90: 2c0a 2020 2020 2020 2020 276d 273a 2027  ,.        'm': '
+0000eba0: 6d27 0a20 2020 207d 0a0a 2020 2020 233a  m'.    }..    #:
+0000ebb0: 204d 6f64 656c 2050 6172 616d 6574 6572   Model Parameter
+0000ebc0: 2075 6e69 7420 7374 7269 6e67 730a 2020   unit strings.  
+0000ebd0: 2020 554e 4954 5320 3d20 7b0a 2020 2020    UNITS = {.    
+0000ebe0: 2020 2020 2743 273a 2027 6c6f 6731 305b      'C': 'log10[
+0000ebf0: 4f65 5e2d 7020 735e 2d31 5d27 2c0a 2020  Oe^-p s^-1]',.  
+0000ec00: 2020 2020 2020 276d 273a 2027 270a 2020        'm': ''.  
+0000ec10: 2020 7d0a 0a20 2020 2023 3a20 4d6f 6465    }..    #: Mode
+0000ec20: 6c20 5061 7261 6d65 7465 7220 756e 6974  l Parameter unit
+0000ec30: 206d 6174 686d 6f64 6520 7374 7269 6e67   mathmode string
+0000ec40: 730a 2020 2020 554e 4954 535f 4d4d 203d  s.    UNITS_MM =
+0000ec50: 207b 0a20 2020 2020 2020 2027 4327 3a20   {.        'C': 
+0000ec60: 7227 245c 6c6f 675f 5c6d 6174 6872 6567  r'$\log_\mathreg
+0000ec70: 756c 6172 7b31 307d 5c6c 6566 745b 5c6d  ular{10}\left[\m
+0000ec80: 6174 6872 6567 756c 6172 7b4f 657d 5e7b  athregular{Oe}^{
+0000ec90: 2d6d 7d20 5c20 5c6d 6174 6872 6567 756c  -m} \ \mathregul
+0000eca0: 6172 7b73 7d5e 5c6d 6174 6872 6567 756c  ar{s}^\mathregul
+0000ecb0: 6172 7b2d 317d 5c72 6967 6874 5d24 272c  ar{-1}\right]$',
+0000ecc0: 2023 206e 6f71 610a 2020 2020 2020 2020   # noqa.        
+0000ecd0: 276d 273a 2027 270a 2020 2020 7d0a 0a20  'm': ''.    }.. 
+0000ece0: 2020 2023 3a20 4d6f 6465 6c20 5061 7261     #: Model Para
+0000ecf0: 6d65 7465 7220 6e61 6d65 2048 544d 4c20  meter name HTML 
+0000ed00: 7374 7269 6e67 730a 2020 2020 554e 4954  strings.    UNIT
+0000ed10: 535f 4854 4d4c 203d 207b 0a20 2020 2020  S_HTML = {.     
+0000ed20: 2020 2027 4327 3a20 7227 6c6f 673c 7375     'C': r'log<su
+0000ed30: 623e 3130 3c2f 7375 623e 5b4f 653c 7375  b>10</sub>[Oe<su
+0000ed40: 703e 2d6d 3c2f 7375 703e 2073 3c73 7570  p>-m</sup> s<sup
+0000ed50: 3e2d 313c 2f73 7570 3e5d 272c 0a20 2020  >-1</sup>]',.   
+0000ed60: 2020 2020 2027 6d27 3a20 2727 0a20 2020       'm': ''.   
+0000ed70: 207d 0a0a 2020 2020 233a 204d 6f64 656c   }..    #: Model
+0000ed80: 2050 6172 616d 6574 6572 2062 6f75 6e64   Parameter bound
+0000ed90: 730a 2020 2020 424f 554e 4453 203d 207b  s.    BOUNDS = {
+0000eda0: 0a20 2020 2020 2020 2027 4327 3a20 5b2d  .        'C': [-
+0000edb0: 3330 2c20 6e70 2e69 6e66 5d2c 0a20 2020  30, np.inf],.   
+0000edc0: 2020 2020 2027 6d27 3a20 5b2d 3330 2c20       'm': [-30, 
+0000edd0: 6e70 2e69 6e66 5d2c 0a20 2020 207d 0a0a  np.inf],.    }..
+0000ede0: 2020 2020 4073 7461 7469 636d 6574 686f      @staticmetho
+0000edf0: 640a 2020 2020 6465 6620 7365 745f 696e  d.    def set_in
+0000ee00: 6974 6961 6c5f 7661 6c73 2870 6172 616d  itial_vals(param
+0000ee10: 5f64 6963 743a 2064 6963 745b 7374 722c  _dict: dict[str,
+0000ee20: 2073 7472 207c 2066 6c6f 6174 5d29 202d   str | float]) -
+0000ee30: 3e20 6469 6374 5b73 7472 2c20 666c 6f61  > dict[str, floa
+0000ee40: 745d 3a20 2320 6e6f 7161 0a20 2020 2020  t]: # noqa.     
+0000ee50: 2020 2027 2727 0a20 2020 2020 2020 2053     '''.        S
+0000ee60: 6574 7320 6775 6573 7320 7661 6c75 6573  ets guess values
+0000ee70: 2066 6f72 2070 6172 616d 6574 6572 7320   for parameters 
+0000ee80: 6966 2072 6571 7565 7374 6564 2062 7920  if requested by 
+0000ee90: 7573 6572 0a0a 2020 2020 2020 2020 5061  user..        Pa
+0000eea0: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
+0000eeb0: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+0000eec0: 2020 2020 7061 7261 6d5f 6469 6374 3a20      param_dict: 
+0000eed0: 6469 6374 5b73 7472 2c20 7374 7220 7c20  dict[str, str | 
+0000eee0: 666c 6f61 745d 0a20 2020 2020 2020 2020  float].         
+0000eef0: 2020 204b 6579 7320 6172 6520 6669 742f     Keys are fit/
+0000ef00: 6669 7820 7061 7261 6d65 7465 7220 6e61  fix parameter na
+0000ef10: 6d65 7320 2873 6565 2063 6c61 7373 2e50  mes (see class.P
+0000ef20: 4152 4e41 4d45 5329 5c6e 0a20 2020 2020  ARNAMES)\n.     
+0000ef30: 2020 2020 2020 2056 616c 7565 7320 6172         Values ar
+0000ef40: 6520 6569 7468 6572 2066 6c6f 6174 2028  e either float (
+0000ef50: 6163 7475 616c 2076 616c 7565 2920 6f72  actual value) or
+0000ef60: 2074 6865 2073 7472 696e 6720 2767 7565   the string 'gue
+0000ef70: 7373 270a 0a20 2020 2020 2020 2052 6574  ss'..        Ret
+0000ef80: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
+0000ef90: 2d2d 2d2d 0a20 2020 2020 2020 2064 6963  ----.        dic
+0000efa0: 745b 7374 722c 2066 6c6f 6174 5d0a 2020  t[str, float].  
+0000efb0: 2020 2020 2020 2020 2020 4b65 7973 2061            Keys a
+0000efc0: 7265 2066 6974 2f66 6978 2070 6172 616d  re fit/fix param
+0000efd0: 6574 6572 206e 616d 6573 2028 7365 6520  eter names (see 
+0000efe0: 636c 6173 732e 5041 524e 414d 4553 295c  class.PARNAMES)\
+0000eff0: 6e0a 2020 2020 2020 2020 2020 2020 5661  n.            Va
+0000f000: 6c75 6573 2061 7265 2066 6c6f 6174 2028  lues are float (
+0000f010: 6163 7475 616c 2076 616c 7565 2920 7768  actual value) wh
+0000f020: 6963 6820 6172 6520 696e 6974 6961 6c20  ich are initial 
+0000f030: 7661 6c75 6573 206f 660a 2020 2020 2020  values of.      
+0000f040: 2020 2020 2020 7061 7261 6d65 7465 720a        parameter.
+0000f050: 2020 2020 2020 2020 2727 270a 0a20 2020          '''..   
+0000f060: 2020 2020 2023 204d 616b 6520 636f 7079       # Make copy
+0000f070: 2c20 616e 7920 7374 7220 7661 6c75 6573  , any str values
+0000f080: 2077 696c 6c20 6265 2072 6570 6c61 6365   will be replace
+0000f090: 640a 2020 2020 2020 2020 6e65 775f 7061  d.        new_pa
+0000f0a0: 7261 6d5f 6469 6374 203d 2063 6f70 792e  ram_dict = copy.
+0000f0b0: 636f 7079 2870 6172 616d 5f64 6963 7429  copy(param_dict)
+0000f0c0: 0a0a 2020 2020 2020 2020 2320 4775 6573  ..        # Gues
+0000f0d0: 7365 730a 2020 2020 2020 2020 6775 6573  ses.        gues
+0000f0e0: 7364 6963 7420 3d20 7b0a 2020 2020 2020  sdict = {.      
+0000f0f0: 2020 2020 2020 2743 273a 202d 342c 0a20        'C': -4,. 
+0000f100: 2020 2020 2020 2020 2020 2027 6d27 3a20             'm': 
+0000f110: 340a 2020 2020 2020 2020 7d0a 0a20 2020  4.        }..   
+0000f120: 2020 2020 2023 2052 6570 6c61 6365 2027       # Replace '
+0000f130: 6775 6573 7327 2077 6974 6820 7265 6c65  guess' with rele
+0000f140: 7661 6e74 2067 7565 7373 0a20 2020 2020  vant guess.     
+0000f150: 2020 2066 6f72 2076 6172 2c20 7661 6c20     for var, val 
+0000f160: 696e 2070 6172 616d 5f64 6963 742e 6974  in param_dict.it
+0000f170: 656d 7328 293a 0a20 2020 2020 2020 2020  ems():.         
+0000f180: 2020 2069 6620 7661 6c20 3d3d 2027 6775     if val == 'gu
+0000f190: 6573 7327 3a0a 2020 2020 2020 2020 2020  ess':.          
+0000f1a0: 2020 2020 2020 6e65 775f 7061 7261 6d5f        new_param_
+0000f1b0: 6469 6374 5b76 6172 5d20 3d20 6775 6573  dict[var] = gues
+0000f1c0: 7364 6963 745b 7661 725d 0a0a 2020 2020  sdict[var]..    
+0000f1d0: 2020 2020 7265 7475 726e 206e 6577 5f70      return new_p
+0000f1e0: 6172 616d 5f64 6963 740a 0a20 2020 2040  aram_dict..    @
+0000f1f0: 7374 6174 6963 6d65 7468 6f64 0a20 2020  staticmethod.   
+0000f200: 2064 6566 206d 6f64 656c 2870 6172 616d   def model(param
+0000f210: 6574 6572 733a 2064 6963 745b 7374 722c  eters: dict[str,
+0000f220: 2066 6c6f 6174 5d2c 0a20 2020 2020 2020   float],.       
+0000f230: 2020 2020 2020 2066 6965 6c64 733a 206e         fields: n
+0000f240: 7074 2e41 7272 6179 4c69 6b65 2920 2d3e  pt.ArrayLike) ->
+0000f250: 206e 7074 2e4e 4441 7272 6179 3a0a 2020   npt.NDArray:.  
+0000f260: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
+0000f270: 2020 4576 616c 7561 7465 7320 6c6f 6731    Evaluates log1
+0000f280: 3028 5261 6d61 6e2d 4949 2920 6d6f 6465  0(Raman-II) mode
+0000f290: 6c20 6f66 206c 6f67 3130 2872 656c 6178  l of log10(relax
+0000f2a0: 6174 696f 6e20 7261 7465 290a 2020 2020  ation rate).    
+0000f2b0: 2020 2020 7573 696e 6720 7072 6f76 6964      using provid
+0000f2c0: 6564 2070 6172 616d 6574 6572 2061 6e64  ed parameter and
+0000f2d0: 2066 6965 6c64 2076 616c 7565 732e 0a0a   field values...
+0000f2e0: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+0000f2f0: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
+0000f300: 2d2d 2d2d 2d0a 2020 2020 2020 2020 7061  -----.        pa
+0000f310: 7261 6d65 7465 7273 3a20 6469 6374 5b73  rameters: dict[s
+0000f320: 7472 2c20 666c 6f61 745d 0a20 2020 2020  tr, float].     
+0000f330: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+0000f340: 7320 746f 2075 7365 2069 6e20 6d6f 6465  s to use in mode
+0000f350: 6c20 6675 6e63 7469 6f6e 2c20 6b65 7973  l function, keys
+0000f360: 2061 7265 2067 6976 656e 2069 6e0a 2020   are given in.  
+0000f370: 2020 2020 2020 2020 2020 636c 6173 732e            class.
+0000f380: 5041 524e 414d 4553 0a20 2020 2020 2020  PARNAMES.       
+0000f390: 2066 6965 6c64 733a 2061 7272 6179 5f6c   fields: array_l
+0000f3a0: 696b 650a 2020 2020 2020 2020 2020 2020  ike.            
+0000f3b0: 6669 656c 6420 7661 6c75 6573 2028 4f65  field values (Oe
+0000f3c0: 2920 6174 2077 6869 6368 206d 6f64 656c  ) at which model
+0000f3d0: 2066 756e 6374 696f 6e20 6973 2065 7661   function is eva
+0000f3e0: 6c75 6174 6564 0a0a 2020 2020 2020 2020  luated..        
+0000f3f0: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
+0000f400: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+0000f410: 6e64 6172 7261 7920 6f66 2066 6c6f 6174  ndarray of float
+0000f420: 730a 2020 2020 2020 2020 2020 2020 6c6f  s.            lo
+0000f430: 6731 3028 5265 6c61 7861 7469 6f6e 2072  g10(Relaxation r
+0000f440: 6174 6529 2061 7320 6120 6675 6e63 7469  ate) as a functi
+0000f450: 6f6e 206f 6620 6669 656c 640a 0a20 2020  on of field..   
+0000f460: 2020 2020 2027 2727 0a0a 2020 2020 2020       '''..      
+0000f470: 2020 6320 3d20 7061 7261 6d65 7465 7273    c = parameters
+0000f480: 5b27 4327 5d0a 2020 2020 2020 2020 6d20  ['C'].        m 
+0000f490: 3d20 7061 7261 6d65 7465 7273 5b27 6d27  = parameters['m'
+0000f4a0: 5d0a 0a20 2020 2020 2020 206c 6f67 7261  ]..        logra
+0000f4b0: 7465 203d 206e 702e 6c6f 6731 3028 3130  te = np.log10(10
+0000f4c0: 2a2a 6320 2a20 6e70 2e61 7361 7272 6179  **c * np.asarray
+0000f4d0: 2866 6965 6c64 7329 2a2a 6d29 0a0a 2020  (fields)**m)..  
+0000f4e0: 2020 2020 2020 7265 7475 726e 206c 6f67        return log
+0000f4f0: 7261 7465 0a0a 0a63 6c61 7373 204c 6f67  rate...class Log
+0000f500: 436f 6e73 7461 6e74 4d6f 6465 6c28 4c6f  ConstantModel(Lo
+0000f510: 6754 6175 484d 6f64 656c 293a 0a20 2020  gTauHModel):.   
+0000f520: 2027 2727 0a20 2020 204c 6f67 2843 6f6e   '''.    Log(Con
+0000f530: 7374 616e 7429 204d 6f64 656c 206f 6620  stant) Model of 
+0000f540: 6c6f 6731 3028 5265 6c61 7861 7469 6f6e  log10(Relaxation
+0000f550: 2072 6174 6529 2076 7320 6669 656c 640a   rate) vs field.
+0000f560: 2020 2020 2727 270a 0a20 2020 2023 3a20      '''..    #: 
+0000f570: 4d6f 6465 6c20 6e61 6d65 0a20 2020 204e  Model name.    N
+0000f580: 414d 4520 3d20 2743 6f6e 7374 616e 7427  AME = 'Constant'
+0000f590: 0a0a 2020 2020 233a 204d 6f64 656c 206e  ..    #: Model n
+0000f5a0: 616d 6520 7769 7468 206c 6f67 2062 7261  ame with log bra
+0000f5b0: 636b 6574 730a 2020 2020 4c4e 414d 4520  ckets.    LNAME 
+0000f5c0: 3d20 274c 6f67 2843 6f6e 7374 616e 7429  = 'Log(Constant)
+0000f5d0: 270a 0a20 2020 2023 3a20 4d6f 6465 6c20  '..    #: Model 
+0000f5e0: 5061 7261 6d65 7465 7220 6e61 6d65 2073  Parameter name s
+0000f5f0: 7472 696e 6773 0a20 2020 2050 4152 4e41  trings.    PARNA
+0000f600: 4d45 5320 3d20 5b0a 2020 2020 2020 2020  MES = [.        
+0000f610: 2743 7427 2c0a 2020 2020 5d0a 0a20 2020  'Ct',.    ]..   
+0000f620: 2023 3a20 4d6f 6465 6c20 5061 7261 6d65   #: Model Parame
+0000f630: 7465 7220 6e61 6d65 206d 6174 686d 6f64  ter name mathmod
+0000f640: 6520 7374 7269 6e67 730a 2020 2020 5641  e strings.    VA
+0000f650: 524e 414d 4553 5f4d 4d20 3d20 7b0a 2020  RNAMES_MM = {.  
+0000f660: 2020 2020 2020 2743 7427 3a20 7227 2443        'Ct': r'$C
+0000f670: 7424 272c 0a20 2020 207d 0a0a 2020 2020  t$',.    }..    
+0000f680: 233a 204d 6f64 656c 2050 6172 616d 6574  #: Model Paramet
+0000f690: 6572 206e 616d 6520 4854 4d4c 2073 7472  er name HTML str
+0000f6a0: 696e 6773 0a20 2020 2056 4152 4e41 4d45  ings.    VARNAME
+0000f6b0: 535f 4854 4d4c 203d 207b 0a20 2020 2020  S_HTML = {.     
+0000f6c0: 2020 2027 4374 273a 2027 4374 270a 2020     'Ct': 'Ct'.  
+0000f6d0: 2020 7d0a 0a20 2020 2023 3a20 4d6f 6465    }..    #: Mode
+0000f6e0: 6c20 5061 7261 6d65 7465 7220 756e 6974  l Parameter unit
+0000f6f0: 2073 7472 696e 6773 0a20 2020 2055 4e49   strings.    UNI
+0000f700: 5453 203d 207b 0a20 2020 2020 2020 2027  TS = {.        '
+0000f710: 4374 273a 2027 6c6f 6731 305b 735e 2d31  Ct': 'log10[s^-1
+0000f720: 5d27 0a20 2020 207d 0a0a 2020 2020 233a  ]'.    }..    #:
+0000f730: 204d 6f64 656c 2050 6172 616d 6574 6572   Model Parameter
+0000f740: 2075 6e69 7420 6d61 7468 6d6f 6465 2073   unit mathmode s
+0000f750: 7472 696e 6773 0a20 2020 2055 4e49 5453  trings.    UNITS
+0000f760: 5f4d 4d20 3d20 7b0a 2020 2020 2020 2020  _MM = {.        
+0000f770: 2743 7427 3a20 7227 245c 6c6f 675f 5c6d  'Ct': r'$\log_\m
+0000f780: 6174 6872 6567 756c 6172 7b31 307d 5c6c  athregular{10}\l
+0000f790: 6566 745b 5c6d 6174 6872 6567 756c 6172  eft[\mathregular
+0000f7a0: 7b73 7d5e 5c6d 6174 6872 6567 756c 6172  {s}^\mathregular
+0000f7b0: 7b2d 317d 5c72 6967 6874 5d24 272c 2023  {-1}\right]$', #
+0000f7c0: 206e 6f71 610a 2020 2020 7d0a 0a20 2020   noqa.    }..   
+0000f7d0: 2023 3a20 4d6f 6465 6c20 5061 7261 6d65   #: Model Parame
+0000f7e0: 7465 7220 756e 6974 2048 544d 4c20 7374  ter unit HTML st
+0000f7f0: 7269 6e67 730a 2020 2020 554e 4954 535f  rings.    UNITS_
+0000f800: 4854 4d4c 203d 207b 0a20 2020 2020 2020  HTML = {.       
+0000f810: 2027 4374 273a 2072 276c 6f67 3c73 7562   'Ct': r'log<sub
+0000f820: 3e31 303c 2f73 7562 3e5b 733c 7375 703e  >10</sub>[s<sup>
+0000f830: 2d31 3c2f 7375 703e 5d27 0a20 2020 207d  -1</sup>]'.    }
+0000f840: 0a0a 2020 2020 233a 204d 6f64 656c 2070  ..    #: Model p
+0000f850: 6172 616d 6574 6572 2062 6f75 6e64 730a  arameter bounds.
+0000f860: 2020 2020 424f 554e 4453 203d 207b 0a20      BOUNDS = {. 
+0000f870: 2020 2020 2020 2027 4374 273a 205b 2d33         'Ct': [-3
+0000f880: 302c 2031 305d 2c0a 2020 2020 7d0a 0a20  0, 10],.    }.. 
+0000f890: 2020 2040 7374 6174 6963 6d65 7468 6f64     @staticmethod
+0000f8a0: 0a20 2020 2064 6566 2073 6574 5f69 6e69  .    def set_ini
+0000f8b0: 7469 616c 5f76 616c 7328 7061 7261 6d5f  tial_vals(param_
+0000f8c0: 6469 6374 3a20 6469 6374 5b73 7472 2c20  dict: dict[str, 
+0000f8d0: 7374 7220 7c20 666c 6f61 745d 2920 2d3e  str | float]) ->
+0000f8e0: 2064 6963 745b 7374 722c 2066 6c6f 6174   dict[str, float
+0000f8f0: 5d3a 2023 206e 6f71 610a 2020 2020 2020  ]: # noqa.      
+0000f900: 2020 2727 270a 2020 2020 2020 2020 5365    '''.        Se
+0000f910: 7473 2067 7565 7373 2076 616c 7565 7320  ts guess values 
+0000f920: 666f 7220 7061 7261 6d65 7465 7273 2069  for parameters i
+0000f930: 6620 7265 7175 6573 7465 6420 6279 2075  f requested by u
+0000f940: 7365 720a 0a20 2020 2020 2020 2050 6172  ser..        Par
+0000f950: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
+0000f960: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
+0000f970: 2020 2070 6172 616d 5f64 6963 743a 2064     param_dict: d
+0000f980: 6963 745b 7374 722c 2073 7472 207c 2066  ict[str, str | f
+0000f990: 6c6f 6174 5d0a 2020 2020 2020 2020 2020  loat].          
+0000f9a0: 2020 4b65 7973 2061 7265 2066 6974 2f66    Keys are fit/f
+0000f9b0: 6978 2070 6172 616d 6574 6572 206e 616d  ix parameter nam
+0000f9c0: 6573 2028 7365 6520 636c 6173 732e 5041  es (see class.PA
+0000f9d0: 524e 414d 4553 295c 6e0a 2020 2020 2020  RNAMES)\n.      
+0000f9e0: 2020 2020 2020 5661 6c75 6573 2061 7265        Values are
+0000f9f0: 2065 6974 6865 7220 666c 6f61 7420 2861   either float (a
+0000fa00: 6374 7561 6c20 7661 6c75 6529 206f 7220  ctual value) or 
+0000fa10: 7468 6520 7374 7269 6e67 2027 6775 6573  the string 'gues
+0000fa20: 7327 0a0a 2020 2020 2020 2020 5265 7475  s'..        Retu
+0000fa30: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
+0000fa40: 2d2d 2d0a 2020 2020 2020 2020 6469 6374  ---.        dict
+0000fa50: 5b73 7472 2c20 666c 6f61 745d 0a20 2020  [str, float].   
+0000fa60: 2020 2020 2020 2020 204b 6579 7320 6172           Keys ar
+0000fa70: 6520 6669 742f 6669 7820 7061 7261 6d65  e fit/fix parame
+0000fa80: 7465 7220 6e61 6d65 7320 2873 6565 2063  ter names (see c
+0000fa90: 6c61 7373 2e50 4152 4e41 4d45 5329 5c6e  lass.PARNAMES)\n
+0000faa0: 0a20 2020 2020 2020 2020 2020 2056 616c  .            Val
+0000fab0: 7565 7320 6172 6520 666c 6f61 7420 2861  ues are float (a
+0000fac0: 6374 7561 6c20 7661 6c75 6529 2077 6869  ctual value) whi
+0000fad0: 6368 2061 7265 2069 6e69 7469 616c 2076  ch are initial v
+0000fae0: 616c 7565 7320 6f66 0a20 2020 2020 2020  alues of.       
+0000faf0: 2020 2020 2070 6172 616d 6574 6572 0a20       parameter. 
+0000fb00: 2020 2020 2020 2027 2727 0a0a 2020 2020         '''..    
+0000fb10: 2020 2020 2320 4d61 6b65 2063 6f70 792c      # Make copy,
+0000fb20: 2061 6e79 2073 7472 2076 616c 7565 7320   any str values 
+0000fb30: 7769 6c6c 2062 6520 7265 706c 6163 6564  will be replaced
+0000fb40: 0a20 2020 2020 2020 206e 6577 5f70 6172  .        new_par
+0000fb50: 616d 5f64 6963 7420 3d20 636f 7079 2e63  am_dict = copy.c
+0000fb60: 6f70 7928 7061 7261 6d5f 6469 6374 290a  opy(param_dict).
+0000fb70: 0a20 2020 2020 2020 2023 2047 7565 7373  .        # Guess
+0000fb80: 6573 0a20 2020 2020 2020 2067 7565 7373  es.        guess
+0000fb90: 6469 6374 203d 207b 0a20 2020 2020 2020  dict = {.       
+0000fba0: 2020 2020 2027 4374 273a 202d 340a 2020       'Ct': -4.  
+0000fbb0: 2020 2020 2020 7d0a 0a20 2020 2020 2020        }..       
+0000fbc0: 2023 2052 6570 6c61 6365 2027 6775 6573   # Replace 'gues
+0000fbd0: 7327 2077 6974 6820 7265 6c65 7661 6e74  s' with relevant
+0000fbe0: 2067 7565 7373 0a20 2020 2020 2020 2066   guess.        f
+0000fbf0: 6f72 2076 6172 2c20 7661 6c20 696e 2070  or var, val in p
+0000fc00: 6172 616d 5f64 6963 742e 6974 656d 7328  aram_dict.items(
+0000fc10: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
+0000fc20: 6620 7661 6c20 3d3d 2027 6775 6573 7327  f val == 'guess'
+0000fc30: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000fc40: 2020 6e65 775f 7061 7261 6d5f 6469 6374    new_param_dict
+0000fc50: 5b76 6172 5d20 3d20 6775 6573 7364 6963  [var] = guessdic
+0000fc60: 745b 7661 725d 0a0a 2020 2020 2020 2020  t[var]..        
+0000fc70: 7265 7475 726e 206e 6577 5f70 6172 616d  return new_param
+0000fc80: 5f64 6963 740a 0a20 2020 2040 7374 6174  _dict..    @stat
+0000fc90: 6963 6d65 7468 6f64 0a20 2020 2064 6566  icmethod.    def
+0000fca0: 206d 6f64 656c 2870 6172 616d 6574 6572   model(parameter
+0000fcb0: 733a 2064 6963 745b 7374 722c 2066 6c6f  s: dict[str, flo
+0000fcc0: 6174 5d2c 0a20 2020 2020 2020 2020 2020  at],.           
+0000fcd0: 2020 2066 6965 6c64 733a 206e 7074 2e41     fields: npt.A
+0000fce0: 7272 6179 4c69 6b65 2920 2d3e 206e 7074  rrayLike) -> npt
+0000fcf0: 2e4e 4441 7272 6179 3a0a 2020 2020 2020  .NDArray:.      
+0000fd00: 2020 2727 270a 2020 2020 2020 2020 4576    '''.        Ev
+0000fd10: 616c 7561 7465 7320 6c6f 6731 3028 436f  aluates log10(Co
+0000fd20: 6e73 7461 6e74 2920 6d6f 6465 6c20 6f66  nstant) model of
+0000fd30: 206c 6f67 3130 2872 656c 6178 6174 696f   log10(relaxatio
+0000fd40: 6e20 7261 7465 290a 2020 2020 2020 2020  n rate).        
+0000fd50: 7573 696e 6720 7072 6f76 6964 6564 2070  using provided p
+0000fd60: 6172 616d 6574 6572 2061 6e64 2066 6965  arameter and fie
+0000fd70: 6c64 2076 616c 7565 732e 0a0a 2020 2020  ld values...    
+0000fd80: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+0000fd90: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+0000fda0: 2d0a 2020 2020 2020 2020 7061 7261 6d65  -.        parame
+0000fdb0: 7465 7273 3a20 6469 6374 5b73 7472 2c20  ters: dict[str, 
+0000fdc0: 666c 6f61 745d 0a20 2020 2020 2020 2020  float].         
+0000fdd0: 2020 2050 6172 616d 6574 6572 7320 746f     Parameters to
+0000fde0: 2075 7365 2069 6e20 6d6f 6465 6c20 6675   use in model fu
+0000fdf0: 6e63 7469 6f6e 2c20 6b65 7973 2061 7265  nction, keys are
+0000fe00: 2067 6976 656e 2069 6e0a 2020 2020 2020   given in.      
+0000fe10: 2020 2020 2020 636c 6173 732e 5041 524e        class.PARN
+0000fe20: 414d 4553 0a20 2020 2020 2020 2066 6965  AMES.        fie
+0000fe30: 6c64 733a 2061 7272 6179 5f6c 696b 650a  lds: array_like.
+0000fe40: 2020 2020 2020 2020 2020 2020 6669 656c              fiel
+0000fe50: 6420 7661 6c75 6573 2028 4f65 2920 6174  d values (Oe) at
+0000fe60: 2077 6869 6368 206d 6f64 656c 2066 756e   which model fun
+0000fe70: 6374 696f 6e20 6973 2065 7661 6c75 6174  ction is evaluat
+0000fe80: 6564 0a0a 2020 2020 2020 2020 5265 7475  ed..        Retu
+0000fe90: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
+0000fea0: 2d2d 2d0a 2020 2020 2020 2020 6e64 6172  ---.        ndar
+0000feb0: 7261 7920 6f66 2066 6c6f 6174 730a 2020  ray of floats.  
+0000fec0: 2020 2020 2020 2020 2020 6c6f 6731 3028            log10(
+0000fed0: 5265 6c61 7861 7469 6f6e 2072 6174 6529  Relaxation rate)
+0000fee0: 2061 7320 6120 6675 6e63 7469 6f6e 206f   as a function o
+0000fef0: 6620 6669 656c 640a 0a20 2020 2020 2020  f field..       
+0000ff00: 2027 2727 0a0a 2020 2020 2020 2020 6374   '''..        ct
+0000ff10: 203d 2070 6172 616d 6574 6572 735b 2743   = parameters['C
+0000ff20: 7427 5d0a 0a20 2020 2020 2020 206c 6f67  t']..        log
+0000ff30: 7261 7465 203d 206e 702e 7a65 726f 7328  rate = np.zeros(
+0000ff40: 6c65 6e28 6669 656c 6473 2929 202b 206e  len(fields)) + n
+0000ff50: 702e 6c6f 6731 3028 3130 2a2a 6374 290a  p.log10(10**ct).
+0000ff60: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000ff70: 6c6f 6772 6174 650a 0a0a 636c 6173 7320  lograte...class 
+0000ff80: 4c6f 6742 5656 5261 6d61 6e49 494d 6f64  LogBVVRamanIIMod
+0000ff90: 656c 284c 6f67 5461 7548 4d6f 6465 6c29  el(LogTauHModel)
+0000ffa0: 3a0a 2020 2020 2727 270a 2020 2020 4c6f  :.    '''.    Lo
+0000ffb0: 6728 4272 6f6e 732d 5661 6e2d 566c 6563  g(Brons-Van-Vlec
+0000ffc0: 6b20 2a20 5261 6d61 6e2d 4949 2920 4d6f  k * Raman-II) Mo
+0000ffd0: 6465 6c20 6f66 206c 6f67 3130 2852 656c  del of log10(Rel
+0000ffe0: 6178 6174 696f 6e20 7261 7465 2920 7673  axation rate) vs
+0000fff0: 2066 6965 6c64 0a20 2020 2027 2727 0a0a   field.    '''..
+00010000: 2020 2020 233a 204d 6f64 656c 206e 616d      #: Model nam
+00010010: 650a 2020 2020 4e41 4d45 203d 2027 4272  e.    NAME = 'Br
+00010020: 6f6e 732d 5661 6e2d 566c 6563 6b20 2a20  ons-Van-Vleck * 
+00010030: 5261 6d61 6e2d 4949 270a 0a20 2020 2023  Raman-II'..    #
+00010040: 3a20 4d6f 6465 6c20 6e61 6d65 2077 6974  : Model name wit
+00010050: 6820 6c6f 6720 6272 6163 6b65 7473 0a20  h log brackets. 
+00010060: 2020 204c 4e41 4d45 203d 2027 4c6f 6728     LNAME = 'Log(
+00010070: 4272 6f6e 732d 5661 6e2d 566c 6563 6b20  Brons-Van-Vleck 
+00010080: 2a20 5261 6d61 6e2d 4949 2927 0a0a 2020  * Raman-II)'..  
+00010090: 2020 233a 204d 6f64 656c 2050 6172 616d    #: Model Param
+000100a0: 6574 6572 206e 616d 6520 7374 7269 6e67  eter name string
+000100b0: 730a 2020 2020 5041 524e 414d 4553 203d  s.    PARNAMES =
+000100c0: 205b 0a20 2020 2020 2020 2027 6527 2c0a   [.        'e',.
+000100d0: 2020 2020 2020 2020 2766 272c 0a20 2020          'f',.   
+000100e0: 2020 2020 2027 4327 2c0a 2020 2020 2020       'C',.      
+000100f0: 2020 276d 270a 2020 2020 5d0a 0a20 2020    'm'.    ]..   
+00010100: 2023 3a20 4d6f 6465 6c20 5061 7261 6d65   #: Model Parame
+00010110: 7465 7220 6e61 6d65 206d 6174 686d 6f64  ter name mathmod
+00010120: 6520 7374 7269 6e67 730a 2020 2020 5641  e strings.    VA
+00010130: 524e 414d 4553 5f4d 4d20 3d20 7b0a 2020  RNAMES_MM = {.  
+00010140: 2020 2020 2020 2765 273a 2072 2724 6524        'e': r'$e$
+00010150: 272c 0a20 2020 2020 2020 2027 6627 3a20  ',.        'f': 
+00010160: 7227 2466 2427 2c0a 2020 2020 2020 2020  r'$f$',.        
+00010170: 2743 273a 2072 2724 4324 272c 0a20 2020  'C': r'$C$',.   
+00010180: 2020 2020 2027 6d27 3a20 7227 246d 2427       'm': r'$m$'
+00010190: 2c0a 2020 2020 7d0a 0a20 2020 2023 3a20  ,.    }..    #: 
+000101a0: 4d6f 6465 6c20 5061 7261 6d65 7465 7220  Model Parameter 
+000101b0: 6e61 6d65 2048 544d 4c20 7374 7269 6e67  name HTML string
+000101c0: 730a 2020 2020 5641 524e 414d 4553 5f48  s.    VARNAMES_H
+000101d0: 544d 4c20 3d20 7b0a 2020 2020 2020 2020  TML = {.        
+000101e0: 2765 273a 2027 6527 2c0a 2020 2020 2020  'e': 'e',.      
+000101f0: 2020 2766 273a 2027 6627 2c0a 2020 2020    'f': 'f',.    
+00010200: 2020 2020 2743 273a 2027 4327 2c0a 2020      'C': 'C',.  
+00010210: 2020 2020 2020 276d 273a 2027 6d27 0a20        'm': 'm'. 
+00010220: 2020 207d 0a0a 2020 2020 233a 204d 6f64     }..    #: Mod
+00010230: 656c 2050 6172 616d 6574 6572 2075 6e69  el Parameter uni
+00010240: 7420 7374 7269 6e67 730a 2020 2020 554e  t strings.    UN
+00010250: 4954 5320 3d20 7b0a 2020 2020 2020 2020  ITS = {.        
+00010260: 2765 273a 2027 6c6f 6731 305b 4f65 5e2d  'e': 'log10[Oe^-
+00010270: 325d 272c 0a20 2020 2020 2020 2027 6627  2]',.        'f'
+00010280: 3a20 276c 6f67 3130 5b4f 655e 2d32 5d27  : 'log10[Oe^-2]'
+00010290: 2c0a 2020 2020 2020 2020 2743 273a 2027  ,.        'C': '
+000102a0: 6c6f 6731 305b 735e 2d31 204f 655e 2d6d  log10[s^-1 Oe^-m
+000102b0: 5d27 2c0a 2020 2020 2020 2020 276d 273a  ]',.        'm':
+000102c0: 2027 270a 2020 2020 7d0a 0a20 2020 2023   ''.    }..    #
+000102d0: 3a20 4d6f 6465 6c20 5061 7261 6d65 7465  : Model Paramete
+000102e0: 7220 756e 6974 206d 6174 686d 6f64 6520  r unit mathmode 
+000102f0: 7374 7269 6e67 730a 2020 2020 554e 4954  strings.    UNIT
+00010300: 535f 4d4d 203d 207b 0a20 2020 2020 2020  S_MM = {.       
+00010310: 2027 6527 3a20 7227 245c 6c6f 675f 5c6d   'e': r'$\log_\m
+00010320: 6174 6872 6567 756c 6172 7b31 307d 5c6c  athregular{10}\l
+00010330: 6566 745b 5c6d 6174 6872 6567 756c 6172  eft[\mathregular
+00010340: 7b4f 657d 5e5c 6d61 7468 7265 6775 6c61  {Oe}^\mathregula
+00010350: 727b 2d32 7d5c 7269 6768 745d 2427 2c20  r{-2}\right]$', 
+00010360: 2320 6e6f 7161 0a20 2020 2020 2020 2027  # noqa.        '
+00010370: 6627 3a20 7227 245c 6c6f 675f 5c6d 6174  f': r'$\log_\mat
+00010380: 6872 6567 756c 6172 7b31 307d 5c6c 6566  hregular{10}\lef
+00010390: 745b 5c6d 6174 6872 6567 756c 6172 7b4f  t[\mathregular{O
+000103a0: 657d 5e5c 6d61 7468 7265 6775 6c61 727b  e}^\mathregular{
+000103b0: 2d32 7d5c 7269 6768 745d 2427 2c20 2320  -2}\right]$', # 
+000103c0: 6e6f 7161 0a20 2020 2020 2020 2027 4327  noqa.        'C'
+000103d0: 3a20 7227 245c 6c6f 675f 5c6d 6174 6872  : r'$\log_\mathr
+000103e0: 6567 756c 6172 7b31 307d 5c6c 6566 745b  egular{10}\left[
+000103f0: 5c6d 6174 6872 6567 756c 6172 7b73 7d5e  \mathregular{s}^
+00010400: 5c6d 6174 6872 6567 756c 6172 7b2d 317d  \mathregular{-1}
+00010410: 205c 6d61 7468 7265 6775 6c61 727b 4f65   \mathregular{Oe
+00010420: 7d5e 5c6d 6174 6872 6567 756c 6172 7b2d  }^\mathregular{-
+00010430: 327d 5c72 6967 6874 5d24 272c 2023 206e  2}\right]$', # n
+00010440: 6f71 610a 2020 2020 2020 2020 276d 273a  oqa.        'm':
+00010450: 2027 270a 2020 2020 7d0a 0a20 2020 2023   ''.    }..    #
+00010460: 3a20 4d6f 6465 6c20 5061 7261 6d65 7465  : Model Paramete
+00010470: 7220 756e 6974 2048 544d 4c20 7374 7269  r unit HTML stri
+00010480: 6e67 730a 2020 2020 554e 4954 535f 4854  ngs.    UNITS_HT
+00010490: 4d4c 203d 207b 0a20 2020 2020 2020 2027  ML = {.        '
+000104a0: 6527 3a20 7227 6c6f 673c 7375 623e 3130  e': r'log<sub>10
+000104b0: 3c2f 7375 623e 5b4f 653c 7375 703e 2d32  </sub>[Oe<sup>-2
+000104c0: 3c2f 7375 703e 5d27 2c0a 2020 2020 2020  </sup>]',.      
+000104d0: 2020 2766 273a 2072 276c 6f67 3c73 7562    'f': r'log<sub
+000104e0: 3e31 303c 2f73 7562 3e5b 4f65 3c73 7570  >10</sub>[Oe<sup
+000104f0: 3e2d 323c 2f73 7570 3e5d 272c 0a20 2020  >-2</sup>]',.   
+00010500: 2020 2020 2027 4327 3a20 7227 6c6f 673c       'C': r'log<
+00010510: 7375 623e 3130 3c2f 7375 623e 5b73 3c73  sub>10</sub>[s<s
+00010520: 7570 3e2d 313c 2f73 7570 3e20 4f65 3c73  up>-1</sup> Oe<s
+00010530: 7570 3e2d 6d3c 2f73 7570 3e5d 272c 0a20  up>-m</sup>]',. 
+00010540: 2020 2020 2020 2027 6d27 3a20 2727 0a20         'm': ''. 
+00010550: 2020 207d 0a0a 2020 2020 233a 204d 6f64     }..    #: Mod
+00010560: 656c 2070 6172 616d 6574 6572 2062 6f75  el parameter bou
+00010570: 6e64 730a 2020 2020 424f 554e 4453 203d  nds.    BOUNDS =
+00010580: 207b 0a20 2020 2020 2020 2027 6527 3a20   {.        'e': 
+00010590: 5b2d 3330 2c20 6e70 2e69 6e66 5d2c 0a20  [-30, np.inf],. 
+000105a0: 2020 2020 2020 2027 6627 3a20 5b2d 3330         'f': [-30
+000105b0: 2c20 6e70 2e69 6e66 5d2c 0a20 2020 2020  , np.inf],.     
+000105c0: 2020 2027 4327 3a20 5b2d 3330 2c20 6e70     'C': [-30, np
+000105d0: 2e69 6e66 5d2c 0a20 2020 2020 2020 2027  .inf],.        '
+000105e0: 6d27 3a20 5b30 2c20 3130 5d2c 0a20 2020  m': [0, 10],.   
+000105f0: 207d 0a0a 2020 2020 4073 7461 7469 636d   }..    @staticm
+00010600: 6574 686f 640a 2020 2020 6465 6620 7365  ethod.    def se
+00010610: 745f 696e 6974 6961 6c5f 7661 6c73 2870  t_initial_vals(p
+00010620: 6172 616d 5f64 6963 743a 2064 6963 745b  aram_dict: dict[
+00010630: 7374 722c 2073 7472 207c 2066 6c6f 6174  str, str | float
+00010640: 5d29 202d 3e20 6469 6374 5b73 7472 2c20  ]) -> dict[str, 
+00010650: 666c 6f61 745d 3a20 2320 6e6f 7161 0a20  float]: # noqa. 
+00010660: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
+00010670: 2020 2053 6574 7320 6775 6573 7320 7661     Sets guess va
+00010680: 6c75 6573 2066 6f72 2070 6172 616d 6574  lues for paramet
+00010690: 6572 7320 6966 2072 6571 7565 7374 6564  ers if requested
+000106a0: 2062 7920 7573 6572 0a0a 2020 2020 2020   by user..      
+000106b0: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+000106c0: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a       ----------.
+000106d0: 2020 2020 2020 2020 7061 7261 6d5f 6469          param_di
+000106e0: 6374 3a20 6469 6374 5b73 7472 2c20 7374  ct: dict[str, st
+000106f0: 7220 7c20 666c 6f61 745d 0a20 2020 2020  r | float].     
+00010700: 2020 2020 2020 204b 6579 7320 6172 6520         Keys are 
+00010710: 6669 742f 6669 7820 7061 7261 6d65 7465  fit/fix paramete
+00010720: 7220 6e61 6d65 7320 2873 6565 2063 6c61  r names (see cla
+00010730: 7373 2e50 4152 4e41 4d45 5329 5c6e 0a20  ss.PARNAMES)\n. 
+00010740: 2020 2020 2020 2020 2020 2056 616c 7565             Value
+00010750: 7320 6172 6520 6569 7468 6572 2066 6c6f  s are either flo
+00010760: 6174 2028 6163 7475 616c 2076 616c 7565  at (actual value
+00010770: 2920 6f72 2074 6865 2073 7472 696e 6720  ) or the string 
+00010780: 2767 7565 7373 270a 0a20 2020 2020 2020  'guess'..       
+00010790: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
+000107a0: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
+000107b0: 2064 6963 745b 7374 722c 2066 6c6f 6174   dict[str, float
+000107c0: 5d0a 2020 2020 2020 2020 2020 2020 4b65  ].            Ke
+000107d0: 7973 2061 7265 2066 6974 2f66 6978 2070  ys are fit/fix p
+000107e0: 6172 616d 6574 6572 206e 616d 6573 2028  arameter names (
+000107f0: 7365 6520 636c 6173 732e 5041 524e 414d  see class.PARNAM
+00010800: 4553 295c 6e0a 2020 2020 2020 2020 2020  ES)\n.          
+00010810: 2020 5661 6c75 6573 2061 7265 2066 6c6f    Values are flo
+00010820: 6174 2028 6163 7475 616c 2076 616c 7565  at (actual value
+00010830: 2920 7768 6963 6820 6172 6520 696e 6974  ) which are init
+00010840: 6961 6c20 7661 6c75 6573 206f 660a 2020  ial values of.  
+00010850: 2020 2020 2020 2020 2020 7061 7261 6d65            parame
+00010860: 7465 720a 2020 2020 2020 2020 2727 270a  ter.        '''.
+00010870: 0a20 2020 2020 2020 2023 204d 616b 6520  .        # Make 
+00010880: 636f 7079 2c20 616e 7920 7374 7220 7661  copy, any str va
+00010890: 6c75 6573 2077 696c 6c20 6265 2072 6570  lues will be rep
+000108a0: 6c61 6365 640a 2020 2020 2020 2020 6e65  laced.        ne
+000108b0: 775f 7061 7261 6d5f 6469 6374 203d 2063  w_param_dict = c
+000108c0: 6f70 792e 636f 7079 2870 6172 616d 5f64  opy.copy(param_d
+000108d0: 6963 7429 0a0a 2020 2020 2020 2020 2320  ict)..        # 
+000108e0: 4775 6573 7365 730a 2020 2020 2020 2020  Guesses.        
+000108f0: 6775 6573 7364 6963 7420 3d20 7b0a 2020  guessdict = {.  
+00010900: 2020 2020 2020 2020 2020 2765 273a 202d            'e': -
+00010910: 352e 2c0a 2020 2020 2020 2020 2020 2020  5.,.            
+00010920: 2766 273a 202d 352e 2c0a 2020 2020 2020  'f': -5.,.      
+00010930: 2020 2020 2020 2743 273a 202d 342c 0a20        'C': -4,. 
+00010940: 2020 2020 2020 2020 2020 2027 6d27 3a20             'm': 
+00010950: 342e 0a20 2020 2020 2020 207d 0a0a 2020  4..        }..  
+00010960: 2020 2020 2020 2320 5265 706c 6163 6520        # Replace 
+00010970: 2767 7565 7373 2720 7769 7468 2072 656c  'guess' with rel
+00010980: 6576 616e 7420 6775 6573 730a 2020 2020  evant guess.    
+00010990: 2020 2020 666f 7220 7661 722c 2076 616c      for var, val
+000109a0: 2069 6e20 7061 7261 6d5f 6469 6374 2e69   in param_dict.i
+000109b0: 7465 6d73 2829 3a0a 2020 2020 2020 2020  tems():.        
+000109c0: 2020 2020 6966 2076 616c 203d 3d20 2767      if val == 'g
+000109d0: 7565 7373 273a 0a20 2020 2020 2020 2020  uess':.         
+000109e0: 2020 2020 2020 206e 6577 5f70 6172 616d         new_param
+000109f0: 5f64 6963 745b 7661 725d 203d 2067 7565  _dict[var] = gue
+00010a00: 7373 6469 6374 5b76 6172 5d0a 0a20 2020  ssdict[var]..   
+00010a10: 2020 2020 2072 6574 7572 6e20 6e65 775f       return new_
+00010a20: 7061 7261 6d5f 6469 6374 0a0a 2020 2020  param_dict..    
+00010a30: 4073 7461 7469 636d 6574 686f 640a 2020  @staticmethod.  
+00010a40: 2020 6465 6620 6d6f 6465 6c28 7061 7261    def model(para
+00010a50: 6d65 7465 7273 3a20 6469 6374 5b73 7472  meters: dict[str
+00010a60: 2c20 666c 6f61 745d 2c0a 2020 2020 2020  , float],.      
+00010a70: 2020 2020 2020 2020 6669 656c 6473 3a20          fields: 
+00010a80: 6e70 742e 4172 7261 794c 696b 6529 202d  npt.ArrayLike) -
+00010a90: 3e20 6e70 742e 4e44 4172 7261 793a 0a20  > npt.NDArray:. 
+00010aa0: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
+00010ab0: 2020 2045 7661 6c75 6174 6573 206c 6f67     Evaluates log
+00010ac0: 3130 2852 616d 616e 2d49 4929 206d 6f64  10(Raman-II) mod
+00010ad0: 656c 206f 6620 6c6f 6731 3028 7265 6c61  el of log10(rela
+00010ae0: 7861 7469 6f6e 2072 6174 6529 0a20 2020  xation rate).   
+00010af0: 2020 2020 2075 7369 6e67 2070 726f 7669       using provi
+00010b00: 6465 6420 7061 7261 6d65 7465 7220 616e  ded parameter an
+00010b10: 6420 6669 656c 6420 7661 6c75 6573 2e0a  d field values..
+00010b20: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+00010b30: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
+00010b40: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2070  ------.        p
+00010b50: 6172 616d 6574 6572 733a 2064 6963 745b  arameters: dict[
+00010b60: 7374 722c 2066 6c6f 6174 5d0a 2020 2020  str, float].    
+00010b70: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+00010b80: 7273 2074 6f20 7573 6520 696e 206d 6f64  rs to use in mod
+00010b90: 656c 2066 756e 6374 696f 6e2c 206b 6579  el function, key
+00010ba0: 7320 6172 6520 6769 7665 6e20 696e 0a20  s are given in. 
+00010bb0: 2020 2020 2020 2020 2020 2063 6c61 7373             class
+00010bc0: 2e50 4152 4e41 4d45 530a 2020 2020 2020  .PARNAMES.      
+00010bd0: 2020 6669 656c 6473 3a20 6172 7261 795f    fields: array_
+00010be0: 6c69 6b65 0a20 2020 2020 2020 2020 2020  like.           
+00010bf0: 2066 6965 6c64 2076 616c 7565 7320 284f   field values (O
+00010c00: 6529 2061 7420 7768 6963 6820 6d6f 6465  e) at which mode
+00010c10: 6c20 6675 6e63 7469 6f6e 2069 7320 6576  l function is ev
+00010c20: 616c 7561 7465 640a 0a20 2020 2020 2020  aluated..       
+00010c30: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
+00010c40: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
+00010c50: 206e 6461 7272 6179 206f 6620 666c 6f61   ndarray of floa
+00010c60: 7473 0a20 2020 2020 2020 2020 2020 206c  ts.            l
+00010c70: 6f67 3130 2852 656c 6178 6174 696f 6e20  og10(Relaxation 
+00010c80: 7261 7465 2920 6173 2061 2066 756e 6374  rate) as a funct
+00010c90: 696f 6e20 6f66 2066 6965 6c64 0a0a 2020  ion of field..  
+00010ca0: 2020 2020 2020 2727 270a 0a20 2020 2020        '''..     
+00010cb0: 2020 2065 203d 2070 6172 616d 6574 6572     e = parameter
+00010cc0: 735b 2765 275d 0a20 2020 2020 2020 2066  s['e'].        f
+00010cd0: 203d 2070 6172 616d 6574 6572 735b 2766   = parameters['f
+00010ce0: 275d 0a20 2020 2020 2020 2043 203d 2070  '].        C = p
+00010cf0: 6172 616d 6574 6572 735b 2743 275d 0a20  arameters['C']. 
+00010d00: 2020 2020 2020 206d 203d 2070 6172 616d         m = param
+00010d10: 6574 6572 735b 276d 275d 0a0a 2020 2020  eters['m']..    
+00010d20: 2020 2020 6c6f 6772 6174 6520 3d20 6e70      lograte = np
+00010d30: 2e6c 6f67 3130 280a 2020 2020 2020 2020  .log10(.        
+00010d40: 2020 2020 2831 302a 2a43 202a 206e 702e      (10**C * np.
+00010d50: 6173 6172 7261 7928 6669 656c 6473 292a  asarray(fields)*
+00010d60: 2a6d 2920 2a20 2831 202b 2031 302a 2a65  *m) * (1 + 10**e
+00010d70: 202a 206e 702e 6173 6172 7261 7928 6669   * np.asarray(fi
+00010d80: 656c 6473 292a 2a32 292f 2831 202b 2031  elds)**2)/(1 + 1
+00010d90: 302a 2a66 202a 206e 702e 6173 6172 7261  0**f * np.asarra
+00010da0: 7928 6669 656c 6473 292a 2a32 2920 2320  y(fields)**2) # 
+00010db0: 6e6f 7161 0a20 2020 2020 2020 2029 0a0a  noqa.        )..
+00010dc0: 2020 2020 2020 2020 7265 7475 726e 206c          return l
+00010dd0: 6f67 7261 7465 0a0a 0a63 6c61 7373 204c  ograte...class L
+00010de0: 6f67 4256 5643 6f6e 7374 616e 744d 6f64  ogBVVConstantMod
+00010df0: 656c 284c 6f67 5461 7548 4d6f 6465 6c29  el(LogTauHModel)
+00010e00: 3a0a 2020 2020 2727 270a 2020 2020 4c6f  :.    '''.    Lo
+00010e10: 6728 4272 6f6e 732d 5661 6e2d 566c 6563  g(Brons-Van-Vlec
+00010e20: 6b20 2a20 436f 6e73 7461 6e74 2920 4d6f  k * Constant) Mo
+00010e30: 6465 6c20 6f66 206c 6f67 3130 2852 656c  del of log10(Rel
+00010e40: 6178 6174 696f 6e20 7261 7465 2920 7673  axation rate) vs
+00010e50: 2066 6965 6c64 0a20 2020 2027 2727 0a0a   field.    '''..
+00010e60: 2020 2020 233a 204d 6f64 656c 206e 616d      #: Model nam
+00010e70: 650a 2020 2020 4e41 4d45 203d 2027 4272  e.    NAME = 'Br
+00010e80: 6f6e 732d 5661 6e2d 566c 6563 6b20 2a20  ons-Van-Vleck * 
+00010e90: 436f 6e73 7461 6e74 270a 0a20 2020 2023  Constant'..    #
+00010ea0: 3a20 4d6f 6465 6c20 6e61 6d65 2077 6974  : Model name wit
+00010eb0: 6820 6c6f 6720 6272 6163 6b65 7473 0a20  h log brackets. 
+00010ec0: 2020 204c 4e41 4d45 203d 2027 4c6f 6728     LNAME = 'Log(
+00010ed0: 4272 6f6e 732d 5661 6e2d 566c 6563 6b20  Brons-Van-Vleck 
+00010ee0: 2a20 436f 6e73 7461 6e74 2927 0a0a 2020  * Constant)'..  
+00010ef0: 2020 233a 204d 6f64 656c 2050 6172 616d    #: Model Param
+00010f00: 6574 6572 206e 616d 6520 7374 7269 6e67  eter name string
+00010f10: 730a 2020 2020 5041 524e 414d 4553 203d  s.    PARNAMES =
+00010f20: 205b 0a20 2020 2020 2020 2027 6527 2c0a   [.        'e',.
+00010f30: 2020 2020 2020 2020 2766 272c 0a20 2020          'f',.   
+00010f40: 2020 2020 2027 4374 270a 2020 2020 5d0a       'Ct'.    ].
+00010f50: 0a20 2020 2023 3a20 4d6f 6465 6c20 5061  .    #: Model Pa
+00010f60: 7261 6d65 7465 7220 6e61 6d65 206d 6174  rameter name mat
+00010f70: 686d 6f64 6520 7374 7269 6e67 730a 2020  hmode strings.  
+00010f80: 2020 5641 524e 414d 4553 5f4d 4d20 3d20    VARNAMES_MM = 
+00010f90: 7b0a 2020 2020 2020 2020 2765 273a 2072  {.        'e': r
+00010fa0: 2724 6524 272c 0a20 2020 2020 2020 2027  '$e$',.        '
+00010fb0: 6627 3a20 7227 2466 2427 2c0a 2020 2020  f': r'$f$',.    
+00010fc0: 2020 2020 2743 7427 3a20 7227 2443 7424      'Ct': r'$Ct$
+00010fd0: 270a 2020 2020 7d0a 0a20 2020 2023 3a20  '.    }..    #: 
+00010fe0: 4d6f 6465 6c20 5061 7261 6d65 7465 7220  Model Parameter 
+00010ff0: 6e61 6d65 2048 544d 4c20 7374 7269 6e67  name HTML string
+00011000: 730a 2020 2020 5641 524e 414d 4553 5f48  s.    VARNAMES_H
+00011010: 544d 4c20 3d20 7b0a 2020 2020 2020 2020  TML = {.        
+00011020: 2765 273a 2027 6527 2c0a 2020 2020 2020  'e': 'e',.      
+00011030: 2020 2766 273a 2027 6627 2c0a 2020 2020    'f': 'f',.    
+00011040: 2020 2020 2743 7427 3a20 2743 7427 0a20      'Ct': 'Ct'. 
+00011050: 2020 207d 0a0a 2020 2020 233a 204d 6f64     }..    #: Mod
+00011060: 656c 2050 6172 616d 6574 6572 2075 6e69  el Parameter uni
+00011070: 7420 7374 7269 6e67 730a 2020 2020 554e  t strings.    UN
+00011080: 4954 5320 3d20 7b0a 2020 2020 2020 2020  ITS = {.        
+00011090: 2765 273a 2027 6c6f 6731 305b 4f65 5e2d  'e': 'log10[Oe^-
+000110a0: 325d 272c 0a20 2020 2020 2020 2027 6627  2]',.        'f'
+000110b0: 3a20 276c 6f67 3130 5b4f 655e 2d32 5d27  : 'log10[Oe^-2]'
+000110c0: 2c0a 2020 2020 2020 2020 2743 7427 3a20  ,.        'Ct': 
+000110d0: 276c 6f67 3130 5b73 5e2d 315d 270a 2020  'log10[s^-1]'.  
+000110e0: 2020 7d0a 0a20 2020 2023 3a20 4d6f 6465    }..    #: Mode
+000110f0: 6c20 5061 7261 6d65 7465 7220 756e 6974  l Parameter unit
+00011100: 206d 6174 686d 6f64 6520 7374 7269 6e67   mathmode string
+00011110: 730a 2020 2020 554e 4954 535f 4d4d 203d  s.    UNITS_MM =
+00011120: 207b 0a20 2020 2020 2020 2027 6527 3a20   {.        'e': 
+00011130: 7227 245c 6c6f 675f 5c6d 6174 6872 6567  r'$\log_\mathreg
+00011140: 756c 6172 7b31 307d 5c6c 6566 745b 5c6d  ular{10}\left[\m
+00011150: 6174 6872 6567 756c 6172 7b4f 657d 5e5c  athregular{Oe}^\
+00011160: 6d61 7468 7265 6775 6c61 727b 2d32 7d5c  mathregular{-2}\
+00011170: 7269 6768 745d 2427 2c20 2320 6e6f 7161  right]$', # noqa
+00011180: 0a20 2020 2020 2020 2027 6627 3a20 7227  .        'f': r'
+00011190: 245c 6c6f 675f 5c6d 6174 6872 6567 756c  $\log_\mathregul
+000111a0: 6172 7b31 307d 5c6c 6566 745b 5c6d 6174  ar{10}\left[\mat
+000111b0: 6872 6567 756c 6172 7b4f 657d 5e5c 6d61  hregular{Oe}^\ma
+000111c0: 7468 7265 6775 6c61 727b 2d32 7d5c 7269  thregular{-2}\ri
+000111d0: 6768 745d 2427 2c20 2320 6e6f 7161 0a20  ght]$', # noqa. 
+000111e0: 2020 2020 2020 2027 4374 273a 2072 2724         'Ct': r'$
+000111f0: 5c6c 6f67 5f5c 6d61 7468 7265 6775 6c61  \log_\mathregula
+00011200: 727b 3130 7d5c 6c65 6674 5b5c 6d61 7468  r{10}\left[\math
+00011210: 7265 6775 6c61 727b 737d 5e5c 6d61 7468  regular{s}^\math
+00011220: 7265 6775 6c61 727b 2d31 7d5c 7269 6768  regular{-1}\righ
+00011230: 745d 2427 2c20 2320 6e6f 7161 0a20 2020  t]$', # noqa.   
+00011240: 207d 0a0a 2020 2020 233a 204d 6f64 656c   }..    #: Model
+00011250: 2050 6172 616d 6574 6572 2075 6e69 7420   Parameter unit 
+00011260: 4854 4d4c 2073 7472 696e 6773 0a20 2020  HTML strings.   
+00011270: 2055 4e49 5453 5f48 544d 4c20 3d20 7b0a   UNITS_HTML = {.
+00011280: 2020 2020 2020 2020 2765 273a 2072 276c          'e': r'l
+00011290: 6f67 3c73 7562 3e31 303c 2f73 7562 3e5b  og<sub>10</sub>[
+000112a0: 4f65 3c73 7570 3e2d 323c 2f73 7570 3e5d  Oe<sup>-2</sup>]
+000112b0: 272c 0a20 2020 2020 2020 2027 6627 3a20  ',.        'f': 
+000112c0: 7227 6c6f 673c 7375 623e 3130 3c2f 7375  r'log<sub>10</su
+000112d0: 623e 5b4f 653c 7375 703e 2d32 3c2f 7375  b>[Oe<sup>-2</su
+000112e0: 703e 5d27 2c0a 2020 2020 2020 2020 2743  p>]',.        'C
+000112f0: 7427 3a20 7227 6c6f 673c 7375 623e 3130  t': r'log<sub>10
+00011300: 3c2f 7375 623e 5b73 3c73 7570 3e2d 313c  </sub>[s<sup>-1<
+00011310: 2f73 7570 3e5d 270a 2020 2020 7d0a 0a20  /sup>]'.    }.. 
+00011320: 2020 2023 3a20 4d6f 6465 6c20 7061 7261     #: Model para
+00011330: 6d65 7465 7220 626f 756e 6473 0a20 2020  meter bounds.   
+00011340: 2042 4f55 4e44 5320 3d20 7b0a 2020 2020   BOUNDS = {.    
+00011350: 2020 2020 2765 273a 205b 2d33 302c 206e      'e': [-30, n
+00011360: 702e 696e 665d 2c0a 2020 2020 2020 2020  p.inf],.        
+00011370: 2766 273a 205b 2d33 302c 206e 702e 696e  'f': [-30, np.in
+00011380: 665d 2c0a 2020 2020 2020 2020 2743 7427  f],.        'Ct'
+00011390: 3a20 5b2d 3330 2c20 3130 5d0a 2020 2020  : [-30, 10].    
+000113a0: 7d0a 0a20 2020 2040 7374 6174 6963 6d65  }..    @staticme
+000113b0: 7468 6f64 0a20 2020 2064 6566 2073 6574  thod.    def set
+000113c0: 5f69 6e69 7469 616c 5f76 616c 7328 7061  _initial_vals(pa
+000113d0: 7261 6d5f 6469 6374 3a20 6469 6374 5b73  ram_dict: dict[s
+000113e0: 7472 2c20 7374 7220 7c20 666c 6f61 745d  tr, str | float]
+000113f0: 2920 2d3e 2064 6963 745b 7374 722c 2066  ) -> dict[str, f
+00011400: 6c6f 6174 5d3a 2023 206e 6f71 610a 2020  loat]: # noqa.  
+00011410: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
+00011420: 2020 5365 7473 2067 7565 7373 2076 616c    Sets guess val
+00011430: 7565 7320 666f 7220 7061 7261 6d65 7465  ues for paramete
+00011440: 7273 2069 6620 7265 7175 6573 7465 6420  rs if requested 
+00011450: 6279 2075 7365 720a 0a20 2020 2020 2020  by user..       
+00011460: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
+00011470: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+00011480: 2020 2020 2020 2070 6172 616d 5f64 6963         param_dic
+00011490: 743a 2064 6963 745b 7374 722c 2073 7472  t: dict[str, str
+000114a0: 207c 2066 6c6f 6174 5d0a 2020 2020 2020   | float].      
+000114b0: 2020 2020 2020 4b65 7973 2061 7265 2066        Keys are f
+000114c0: 6974 2f66 6978 2070 6172 616d 6574 6572  it/fix parameter
+000114d0: 206e 616d 6573 2028 7365 6520 636c 6173   names (see clas
+000114e0: 732e 5041 524e 414d 4553 295c 6e0a 2020  s.PARNAMES)\n.  
+000114f0: 2020 2020 2020 2020 2020 5661 6c75 6573            Values
+00011500: 2061 7265 2065 6974 6865 7220 666c 6f61   are either floa
+00011510: 7420 2861 6374 7561 6c20 7661 6c75 6529  t (actual value)
+00011520: 206f 7220 7468 6520 7374 7269 6e67 2027   or the string '
+00011530: 6775 6573 7327 0a0a 2020 2020 2020 2020  guess'..        
+00011540: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
+00011550: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+00011560: 6469 6374 5b73 7472 2c20 666c 6f61 745d  dict[str, float]
+00011570: 0a20 2020 2020 2020 2020 2020 204b 6579  .            Key
+00011580: 7320 6172 6520 6669 742f 6669 7820 7061  s are fit/fix pa
+00011590: 7261 6d65 7465 7220 6e61 6d65 7320 2873  rameter names (s
+000115a0: 6565 2063 6c61 7373 2e50 4152 4e41 4d45  ee class.PARNAME
+000115b0: 5329 5c6e 0a20 2020 2020 2020 2020 2020  S)\n.           
+000115c0: 2056 616c 7565 7320 6172 6520 666c 6f61   Values are floa
+000115d0: 7420 2861 6374 7561 6c20 7661 6c75 6529  t (actual value)
+000115e0: 2077 6869 6368 2061 7265 2069 6e69 7469   which are initi
+000115f0: 616c 2076 616c 7565 7320 6f66 0a20 2020  al values of.   
+00011600: 2020 2020 2020 2020 2070 6172 616d 6574           paramet
+00011610: 6572 0a20 2020 2020 2020 2027 2727 0a0a  er.        '''..
+00011620: 2020 2020 2020 2020 2320 4d61 6b65 2063          # Make c
+00011630: 6f70 792c 2061 6e79 2073 7472 2076 616c  opy, any str val
+00011640: 7565 7320 7769 6c6c 2062 6520 7265 706c  ues will be repl
+00011650: 6163 6564 0a20 2020 2020 2020 206e 6577  aced.        new
+00011660: 5f70 6172 616d 5f64 6963 7420 3d20 636f  _param_dict = co
+00011670: 7079 2e63 6f70 7928 7061 7261 6d5f 6469  py.copy(param_di
+00011680: 6374 290a 0a20 2020 2020 2020 2023 2047  ct)..        # G
+00011690: 7565 7373 6573 0a20 2020 2020 2020 2067  uesses.        g
+000116a0: 7565 7373 6469 6374 203d 207b 0a20 2020  uessdict = {.   
+000116b0: 2020 2020 2020 2020 2027 6527 3a20 2d35           'e': -5
+000116c0: 2e2c 0a20 2020 2020 2020 2020 2020 2027  .,.            '
+000116d0: 6627 3a20 2d35 2e2c 0a20 2020 2020 2020  f': -5.,.       
+000116e0: 2020 2020 2027 4374 273a 202d 340a 2020       'Ct': -4.  
+000116f0: 2020 2020 2020 7d0a 0a20 2020 2020 2020        }..       
+00011700: 2023 2052 6570 6c61 6365 2027 6775 6573   # Replace 'gues
+00011710: 7327 2077 6974 6820 7265 6c65 7661 6e74  s' with relevant
+00011720: 2067 7565 7373 0a20 2020 2020 2020 2066   guess.        f
+00011730: 6f72 2076 6172 2c20 7661 6c20 696e 2070  or var, val in p
+00011740: 6172 616d 5f64 6963 742e 6974 656d 7328  aram_dict.items(
+00011750: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
+00011760: 6620 7661 6c20 3d3d 2027 6775 6573 7327  f val == 'guess'
+00011770: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00011780: 2020 6e65 775f 7061 7261 6d5f 6469 6374    new_param_dict
+00011790: 5b76 6172 5d20 3d20 6775 6573 7364 6963  [var] = guessdic
+000117a0: 745b 7661 725d 0a0a 2020 2020 2020 2020  t[var]..        
+000117b0: 7265 7475 726e 206e 6577 5f70 6172 616d  return new_param
+000117c0: 5f64 6963 740a 0a20 2020 2040 7374 6174  _dict..    @stat
+000117d0: 6963 6d65 7468 6f64 0a20 2020 2064 6566  icmethod.    def
+000117e0: 206d 6f64 656c 2870 6172 616d 6574 6572   model(parameter
+000117f0: 733a 2064 6963 745b 7374 722c 2066 6c6f  s: dict[str, flo
+00011800: 6174 5d2c 0a20 2020 2020 2020 2020 2020  at],.           
+00011810: 2020 2066 6965 6c64 733a 206e 7074 2e41     fields: npt.A
+00011820: 7272 6179 4c69 6b65 2920 2d3e 206e 7074  rrayLike) -> npt
+00011830: 2e4e 4441 7272 6179 3a0a 2020 2020 2020  .NDArray:.      
+00011840: 2020 2727 270a 2020 2020 2020 2020 4576    '''.        Ev
+00011850: 616c 7561 7465 7320 6c6f 6731 3028 4c6f  aluates log10(Lo
+00011860: 6742 5656 436f 6e73 7461 6e74 4d6f 6465  gBVVConstantMode
+00011870: 6c29 206d 6f64 656c 206f 6620 6c6f 6731  l) model of log1
+00011880: 3028 7265 6c61 7861 7469 6f6e 2072 6174  0(relaxation rat
+00011890: 6529 0a20 2020 2020 2020 2075 7369 6e67  e).        using
+000118a0: 2070 726f 7669 6465 6420 7061 7261 6d65   provided parame
+000118b0: 7465 7220 616e 6420 6669 656c 6420 7661  ter and field va
+000118c0: 6c75 6573 2e0a 0a20 2020 2020 2020 2050  lues...        P
+000118d0: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
+000118e0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+000118f0: 2020 2020 2070 6172 616d 6574 6572 733a       parameters:
+00011900: 2064 6963 745b 7374 722c 2066 6c6f 6174   dict[str, float
+00011910: 5d0a 2020 2020 2020 2020 2020 2020 5061  ].            Pa
+00011920: 7261 6d65 7465 7273 2074 6f20 7573 6520  rameters to use 
+00011930: 696e 206d 6f64 656c 2066 756e 6374 696f  in model functio
+00011940: 6e2c 206b 6579 7320 6172 6520 6769 7665  n, keys are give
+00011950: 6e20 696e 0a20 2020 2020 2020 2020 2020  n in.           
+00011960: 2063 6c61 7373 2e50 4152 4e41 4d45 530a   class.PARNAMES.
+00011970: 2020 2020 2020 2020 6669 656c 6473 3a20          fields: 
+00011980: 6172 7261 795f 6c69 6b65 0a20 2020 2020  array_like.     
+00011990: 2020 2020 2020 2066 6965 6c64 2076 616c         field val
+000119a0: 7565 7320 284f 6529 2061 7420 7768 6963  ues (Oe) at whic
+000119b0: 6820 6d6f 6465 6c20 6675 6e63 7469 6f6e  h model function
+000119c0: 2069 7320 6576 616c 7561 7465 640a 0a20   is evaluated.. 
+000119d0: 2020 2020 2020 2052 6574 7572 6e73 0a20         Returns. 
+000119e0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0a20         -------. 
+000119f0: 2020 2020 2020 206e 6461 7272 6179 206f         ndarray o
+00011a00: 6620 666c 6f61 7473 0a20 2020 2020 2020  f floats.       
+00011a10: 2020 2020 206c 6f67 3130 2852 656c 6178       log10(Relax
+00011a20: 6174 696f 6e20 7261 7465 2920 6173 2061  ation rate) as a
+00011a30: 2066 756e 6374 696f 6e20 6f66 2066 6965   function of fie
+00011a40: 6c64 0a0a 2020 2020 2020 2020 2727 270a  ld..        '''.
+00011a50: 0a20 2020 2020 2020 2065 203d 2070 6172  .        e = par
+00011a60: 616d 6574 6572 735b 2765 275d 0a20 2020  ameters['e'].   
+00011a70: 2020 2020 2066 203d 2070 6172 616d 6574       f = paramet
+00011a80: 6572 735b 2766 275d 0a20 2020 2020 2020  ers['f'].       
+00011a90: 2043 7420 3d20 7061 7261 6d65 7465 7273   Ct = parameters
+00011aa0: 5b27 4374 275d 0a0a 2020 2020 2020 2020  ['Ct']..        
+00011ab0: 6c6f 6772 6174 6520 3d20 6e70 2e6c 6f67  lograte = np.log
+00011ac0: 3130 280a 2020 2020 2020 2020 2020 2020  10(.            
+00011ad0: 3130 2a2a 4374 202a 2028 3120 2b20 3130  10**Ct * (1 + 10
+00011ae0: 2a2a 6520 2a20 6e70 2e61 7361 7272 6179  **e * np.asarray
+00011af0: 2866 6965 6c64 7329 2a2a 3229 202f 2028  (fields)**2) / (
+00011b00: 3120 2b20 3130 2a2a 6620 2a20 6e70 2e61  1 + 10**f * np.a
+00011b10: 7361 7272 6179 2866 6965 6c64 7329 2a2a  sarray(fields)**
+00011b20: 3229 2023 206e 6f71 610a 2020 2020 2020  2) # noqa.      
+00011b30: 2020 290a 0a20 2020 2020 2020 2072 6574    )..        ret
+00011b40: 7572 6e20 6c6f 6772 6174 650a 0a0a 636c  urn lograte...cl
+00011b50: 6173 7320 4c6f 6754 6175 544d 6f64 656c  ass LogTauTModel
+00011b60: 2841 4243 293a 0a20 2020 2027 2727 0a20  (ABC):.    '''. 
+00011b70: 2020 2041 6273 7472 6163 7420 636c 6173     Abstract clas
+00011b80: 7320 6f6e 2077 6869 6368 2061 6c6c 2070  s on which all p
+00011b90: 6865 6e6f 6d65 6e6f 6c6f 6769 6361 6c20  henomenological 
+00011ba0: 6d6f 6465 6c73 206f 660a 2020 2020 7465  models of.    te
+00011bb0: 6d70 6572 6174 7572 652d 6465 7065 6e64  mperature-depend
+00011bc0: 656e 7420 6d61 676e 6574 6963 2072 656c  ent magnetic rel
+00011bd0: 6178 6174 696f 6e20 4c6f 6731 3028 7261  axation Log10(ra
+00011be0: 7465 2920 6172 6520 6261 7365 640a 2020  te) are based.  
+00011bf0: 2020 2727 270a 0a20 2020 2040 7072 6f70    '''..    @prop
+00011c00: 6572 7479 0a20 2020 2040 6162 7374 7261  erty.    @abstra
+00011c10: 6374 6d65 7468 6f64 0a20 2020 2064 6566  ctmethod.    def
+00011c20: 204e 414d 4528 2920 2d3e 2073 7472 3a0a   NAME() -> str:.
+00011c30: 2020 2020 2020 2020 2773 7472 696e 6720          'string 
+00011c40: 6e61 6d65 206f 6620 6d6f 6465 6c27 0a20  name of model'. 
+00011c50: 2020 2020 2020 2072 6169 7365 204e 6f74         raise Not
+00011c60: 496d 706c 656d 656e 7465 6445 7272 6f72  ImplementedError
+00011c70: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+00011c80: 2020 2020 4061 6273 7472 6163 746d 6574      @abstractmet
+00011c90: 686f 640a 2020 2020 6465 6620 4c4e 414d  hod.    def LNAM
+00011ca0: 4528 2920 2d3e 2073 7472 3a0a 2020 2020  E() -> str:.    
+00011cb0: 2020 2020 2773 7472 696e 6720 6e61 6d65      'string name
+00011cc0: 206f 6620 6d6f 6465 6c20 7769 7468 204c   of model with L
+00011cd0: 6f67 2829 2061 726f 756e 6420 6974 2c20  og() around it, 
+00011ce0: 652e 672e 204c 6f67 284f 7262 6163 6829  e.g. Log(Orbach)
+00011cf0: 270a 2020 2020 2020 2020 7261 6973 6520  '.        raise 
+00011d00: 4e6f 7449 6d70 6c65 6d65 6e74 6564 4572  NotImplementedEr
+00011d10: 726f 720a 0a20 2020 2040 7072 6f70 6572  ror..    @proper
+00011d20: 7479 0a20 2020 2040 6162 7374 7261 6374  ty.    @abstract
+00011d30: 6d65 7468 6f64 0a20 2020 2064 6566 2050  method.    def P
+00011d40: 4152 4e41 4d45 5328 2920 2d3e 206c 6973  ARNAMES() -> lis
+00011d50: 745b 7374 725d 3a0a 2020 2020 2020 2020  t[str]:.        
+00011d60: 2773 7472 696e 6720 6e61 6d65 7320 6f66  'string names of
+00011d70: 2070 6172 616d 6574 6572 7320 7768 6963   parameters whic
+00011d80: 6820 6361 6e20 6265 2066 6974 7465 6420  h can be fitted 
+00011d90: 6f72 2066 6978 6564 270a 2020 2020 2020  or fixed'.      
+00011da0: 2020 7261 6973 6520 4e6f 7449 6d70 6c65    raise NotImple
+00011db0: 6d65 6e74 6564 4572 726f 720a 0a20 2020  mentedError..   
+00011dc0: 2040 7072 6f70 6572 7479 0a20 2020 2040   @property.    @
+00011dd0: 6162 7374 7261 6374 6d65 7468 6f64 0a20  abstractmethod. 
+00011de0: 2020 2064 6566 2056 4152 4e41 4d45 535f     def VARNAMES_
+00011df0: 4d4d 2829 202d 3e20 6469 6374 5b73 7472  MM() -> dict[str
+00011e00: 2c20 7374 725d 3a0a 2020 2020 2020 2020  , str]:.        
+00011e10: 2727 270a 2020 2020 2020 2020 4d61 7468  '''.        Math
+00011e20: 6d6f 6465 2028 692e 652e 2024 242c 206c  mode (i.e. $$, l
+00011e30: 6174 6578 2029 2076 6572 7369 6f6e 7320  atex ) versions 
+00011e40: 6f66 2050 4152 4e41 4d45 535c 6e0a 2020  of PARNAMES\n.  
+00011e50: 2020 2020 2020 4b65 7973 2061 7265 2073        Keys are s
+00011e60: 7472 696e 6773 2066 726f 6d20 5041 524e  trings from PARN
+00011e70: 414d 4553 2070 6c75 7320 616e 7920 6f74  AMES plus any ot
+00011e80: 6865 7220 7661 7269 6162 6c65 7320 7768  her variables wh
+00011e90: 6963 680a 2020 2020 2020 2020 6d69 6768  ich.        migh
+00011ea0: 7420 6265 206e 6565 6465 645c 6e0a 2020  t be needed\n.  
+00011eb0: 2020 2020 2020 5661 6c75 6573 2061 7265        Values are
+00011ec0: 206d 6174 686d 6f64 6520 7374 7269 6e67   mathmode string
+00011ed0: 730a 2020 2020 2020 2020 2727 270a 2020  s.        '''.  
+00011ee0: 2020 2020 2020 7261 6973 6520 4e6f 7449        raise NotI
+00011ef0: 6d70 6c65 6d65 6e74 6564 4572 726f 720a  mplementedError.
+00011f00: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
+00011f10: 2020 2040 6162 7374 7261 6374 6d65 7468     @abstractmeth
+00011f20: 6f64 0a20 2020 2064 6566 2056 4152 4e41  od.    def VARNA
+00011f30: 4d45 535f 4854 4d4c 2829 202d 3e20 6469  MES_HTML() -> di
+00011f40: 6374 5b73 7472 2c20 7374 725d 3a0a 2020  ct[str, str]:.  
+00011f50: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
+00011f60: 2020 4854 4d4c 2076 6572 7369 6f6e 7320    HTML versions 
+00011f70: 6f66 2050 4152 4e41 4d45 535c 6e0a 2020  of PARNAMES\n.  
+00011f80: 2020 2020 2020 4b65 7973 2061 7265 2073        Keys are s
+00011f90: 7472 696e 6773 2066 726f 6d20 5041 524e  trings from PARN
+00011fa0: 414d 4553 2070 6c75 7320 616e 7920 6f74  AMES plus any ot
+00011fb0: 6865 7220 7661 7269 6162 6c65 7320 7768  her variables wh
+00011fc0: 6963 680a 2020 2020 2020 2020 6d69 6768  ich.        migh
+00011fd0: 7420 6265 206e 6565 6465 645c 6e0a 2020  t be needed\n.  
+00011fe0: 2020 2020 2020 5661 6c75 6573 2061 7265        Values are
+00011ff0: 206d 6174 686d 6f64 6520 7374 7269 6e67   mathmode string
+00012000: 730a 2020 2020 2020 2020 2727 270a 2020  s.        '''.  
+00012010: 2020 2020 2020 7261 6973 6520 4e6f 7449        raise NotI
+00012020: 6d70 6c65 6d65 6e74 6564 4572 726f 720a  mplementedError.
+00012030: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
+00012040: 2020 2040 6162 7374 7261 6374 6d65 7468     @abstractmeth
+00012050: 6f64 0a20 2020 2064 6566 2055 4e49 5453  od.    def UNITS
+00012060: 2829 202d 3e20 6469 6374 5b73 7472 2c20  () -> dict[str, 
+00012070: 7374 725d 3a0a 2020 2020 2020 2020 2727  str]:.        ''
+00012080: 270a 2020 2020 2020 2020 7374 7269 6e67  '.        string
+00012090: 206e 616d 6573 206f 6620 756e 6974 7320   names of units 
+000120a0: 6f66 2050 4152 4e41 4d45 535c 6e0a 2020  of PARNAMES\n.  
+000120b0: 2020 2020 2020 4b65 7973 2061 7265 2073        Keys are s
+000120c0: 7472 696e 6773 2066 726f 6d20 5041 524e  trings from PARN
+000120d0: 414d 4553 2070 6c75 7320 616e 7920 6f74  AMES plus any ot
+000120e0: 6865 7220 7661 7269 6162 6c65 7320 7768  her variables wh
+000120f0: 6963 680a 2020 2020 2020 2020 6d69 6768  ich.        migh
+00012100: 7420 6265 206e 6565 6465 645c 6e0a 2020  t be needed\n.  
+00012110: 2020 2020 2020 5661 6c75 6573 2061 7265        Values are
+00012120: 2075 6e69 7420 6e61 6d65 2073 7472 696e   unit name strin
+00012130: 6773 0a20 2020 2020 2020 2027 2727 0a20  gs.        '''. 
+00012140: 2020 2020 2020 2072 6169 7365 204e 6f74         raise Not
+00012150: 496d 706c 656d 656e 7465 6445 7272 6f72  ImplementedError
+00012160: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+00012170: 2020 2020 4061 6273 7472 6163 746d 6574      @abstractmet
+00012180: 686f 640a 2020 2020 6465 6620 554e 4954  hod.    def UNIT
+00012190: 535f 4d4d 2829 202d 3e20 6469 6374 5b73  S_MM() -> dict[s
+000121a0: 7472 2c20 7374 725d 3a0a 2020 2020 2020  tr, str]:.      
+000121b0: 2020 2727 270a 2020 2020 2020 2020 4d61    '''.        Ma
+000121c0: 7468 6d6f 6465 2028 692e 652e 2024 242c  thmode (i.e. $$,
+000121d0: 206c 6174 6578 2029 2076 6572 7369 6f6e   latex ) version
+000121e0: 7320 6f66 2055 4e49 5453 5c6e 0a20 2020  s of UNITS\n.   
+000121f0: 2020 2020 204b 6579 7320 6172 6520 7374       Keys are st
+00012200: 7269 6e67 7320 6672 6f6d 2050 4152 4e41  rings from PARNA
+00012210: 4d45 5320 706c 7573 2061 6e79 206f 7468  MES plus any oth
+00012220: 6572 2076 6172 6961 626c 6573 2077 6869  er variables whi
+00012230: 6368 0a20 2020 2020 2020 206d 6967 6874  ch.        might
+00012240: 2062 6520 6e65 6564 6564 5c6e 0a20 2020   be needed\n.   
+00012250: 2020 2020 2056 616c 7565 7320 6172 6520       Values are 
+00012260: 756e 6974 206e 616d 6520 7374 7269 6e67  unit name string
+00012270: 730a 2020 2020 2020 2020 2727 270a 2020  s.        '''.  
+00012280: 2020 2020 2020 7261 6973 6520 4e6f 7449        raise NotI
+00012290: 6d70 6c65 6d65 6e74 6564 4572 726f 720a  mplementedError.
+000122a0: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
+000122b0: 2020 2040 6162 7374 7261 6374 6d65 7468     @abstractmeth
+000122c0: 6f64 0a20 2020 2064 6566 2055 4e49 5453  od.    def UNITS
+000122d0: 5f48 544d 4c28 2920 2d3e 2064 6963 745b  _HTML() -> dict[
+000122e0: 7374 722c 2073 7472 5d3a 0a20 2020 2020  str, str]:.     
+000122f0: 2020 2027 2727 0a20 2020 2020 2020 2048     '''.        H
+00012300: 544d 4c20 7665 7273 696f 6e73 206f 6620  TML versions of 
+00012310: 554e 4954 535c 6e0a 2020 2020 2020 2020  UNITS\n.        
+00012320: 4b65 7973 2061 7265 2073 7472 696e 6773  Keys are strings
+00012330: 2066 726f 6d20 5041 524e 414d 4553 2070   from PARNAMES p
+00012340: 6c75 7320 616e 7920 6f74 6865 7220 7661  lus any other va
+00012350: 7269 6162 6c65 7320 7768 6963 680a 2020  riables which.  
+00012360: 2020 2020 2020 6d69 6768 7420 6265 206e        might be n
+00012370: 6565 6465 645c 6e0a 2020 2020 2020 2020  eeded\n.        
+00012380: 5661 6c75 6573 2061 7265 2075 6e69 7420  Values are unit 
+00012390: 6e61 6d65 2073 7472 696e 6773 0a20 2020  name strings.   
+000123a0: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
+000123b0: 2072 6169 7365 204e 6f74 496d 706c 656d   raise NotImplem
+000123c0: 656e 7465 6445 7272 6f72 0a0a 2020 2020  entedError..    
+000123d0: 4070 726f 7065 7274 790a 2020 2020 4061  @property.    @a
+000123e0: 6273 7472 6163 746d 6574 686f 640a 2020  bstractmethod.  
+000123f0: 2020 6465 6620 424f 554e 4453 2829 202d    def BOUNDS() -
+00012400: 3e20 6469 6374 5b73 7472 2c20 6c69 7374  > dict[str, list
+00012410: 5b66 6c6f 6174 2c20 666c 6f61 745d 5d3a  [float, float]]:
+00012420: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
+00012430: 2020 2020 2042 6f75 6e64 7320 666f 7220       Bounds for 
+00012440: 6561 6368 2070 6172 616d 6574 6572 206f  each parameter o
+00012450: 6620 6d6f 6465 6c5c 6e0a 2020 2020 2020  f model\n.      
+00012460: 2020 4b65 7973 3a20 7061 7261 6d65 7465    Keys: paramete
+00012470: 7220 6e61 6d65 5c6e 0a20 2020 2020 2020  r name\n.       
+00012480: 2056 616c 7565 733a 205b 7570 7065 722c   Values: [upper,
+00012490: 206c 6f77 6572 5d5c 6e0a 2020 2020 2020   lower]\n.      
+000124a0: 2020 7573 6564 2062 7920 7363 6970 7920    used by scipy 
+000124b0: 6c65 6173 745f 7371 7561 7265 730a 2020  least_squares.  
+000124c0: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
+000124d0: 2020 7261 6973 6520 4e6f 7449 6d70 6c65    raise NotImple
+000124e0: 6d65 6e74 6564 4572 726f 720a 0a20 2020  mentedError..   
+000124f0: 2040 7374 6174 6963 6d65 7468 6f64 0a20   @staticmethod. 
+00012500: 2020 2040 6162 7374 7261 6374 6d65 7468     @abstractmeth
+00012510: 6f64 0a20 2020 2064 6566 206d 6f64 656c  od.    def model
+00012520: 2870 6172 616d 6574 6572 733a 2064 6963  (parameters: dic
+00012530: 745b 7374 722c 2066 6c6f 6174 5d2c 0a20  t[str, float],. 
+00012540: 2020 2020 2020 2020 2020 2020 2074 656d               tem
+00012550: 7065 7261 7475 7265 733a 206e 7074 2e41  peratures: npt.A
+00012560: 7272 6179 4c69 6b65 2920 2d3e 206e 7074  rrayLike) -> npt
+00012570: 2e4e 4441 7272 6179 3a0a 2020 2020 2020  .NDArray:.      
+00012580: 2020 2727 270a 2020 2020 2020 2020 4576    '''.        Ev
+00012590: 616c 7561 7465 7320 6d6f 6465 6c20 6675  aluates model fu
+000125a0: 6e63 7469 6f6e 206f 6620 6c6f 6728 7265  nction of log(re
+000125b0: 6c61 7861 7469 6f6e 2072 6174 6529 2075  laxation rate) u
+000125c0: 7369 6e67 2070 726f 7669 6465 640a 2020  sing provided.  
+000125d0: 2020 2020 2020 7061 7261 6d65 7465 7220        parameter 
+000125e0: 616e 6420 7465 6d70 6572 6174 7572 6520  and temperature 
+000125f0: 7661 6c75 6573 2e0a 0a20 2020 2020 2020  values...       
+00012600: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
+00012610: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+00012620: 2020 2020 2020 2070 6172 616d 6574 6572         parameter
+00012630: 733a 2061 7272 6179 5f6c 696b 650a 2020  s: array_like.  
+00012640: 2020 2020 2020 2020 2020 5061 7261 6d65            Parame
+00012650: 7465 7273 2074 6f20 7573 6520 696e 206d  ters to use in m
+00012660: 6f64 656c 2066 756e 6374 696f 6e0a 2020  odel function.  
+00012670: 2020 2020 2020 7465 6d70 6572 6174 7572        temperatur
+00012680: 6573 3a20 6172 7261 795f 6c69 6b65 0a20  es: array_like. 
+00012690: 2020 2020 2020 2020 2020 2054 656d 7065             Tempe
+000126a0: 7261 7475 7265 2076 616c 7565 7320 284b  rature values (K
+000126b0: 2920 6174 2077 6869 6368 206d 6f64 656c  ) at which model
+000126c0: 2066 756e 6374 696f 6e20 6973 2065 7661   function is eva
+000126d0: 6c75 6174 6564 0a0a 2020 2020 2020 2020  luated..        
+000126e0: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
+000126f0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+00012700: 6e64 6172 7261 7920 6f66 2066 6c6f 6174  ndarray of float
+00012710: 730a 2020 2020 2020 2020 2020 2020 6c6f  s.            lo
+00012720: 6731 3028 5265 6c61 7861 7469 6f6e 2072  g10(Relaxation r
+00012730: 6174 6529 2061 7320 6120 6675 6e63 7469  ate) as a functi
+00012740: 6f6e 206f 6620 7465 6d70 6572 6174 7572  on of temperatur
+00012750: 650a 0a20 2020 2020 2020 2027 2727 0a20  e..        '''. 
+00012760: 2020 2020 2020 2072 6169 7365 204e 6f74         raise Not
+00012770: 496d 706c 656d 656e 7465 6445 7272 6f72  ImplementedError
+00012780: 0a0a 2020 2020 4073 7461 7469 636d 6574  ..    @staticmet
+00012790: 686f 640a 2020 2020 4061 6273 7472 6163  hod.    @abstrac
+000127a0: 746d 6574 686f 640a 2020 2020 6465 6620  tmethod.    def 
+000127b0: 7365 745f 696e 6974 6961 6c5f 7661 6c73  set_initial_vals
+000127c0: 2870 6172 616d 6574 6572 733a 2064 6963  (parameters: dic
+000127d0: 745b 7374 722c 2066 6c6f 6174 5d29 202d  t[str, float]) -
+000127e0: 3e20 6469 6374 5b73 7472 2c20 666c 6f61  > dict[str, floa
+000127f0: 745d 3a0a 2020 2020 2020 2020 2727 270a  t]:.        '''.
+00012800: 2020 2020 2020 2020 5365 7473 2067 7565          Sets gue
+00012810: 7373 2076 616c 7565 7320 666f 7220 7061  ss values for pa
+00012820: 7261 6d65 7465 7273 2069 6620 7265 7175  rameters if requ
+00012830: 6573 7465 6420 6279 2075 7365 720a 0a20  ested by user.. 
+00012840: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+00012850: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+00012860: 2d2d 2d2d 0a20 2020 2020 2020 2070 6172  ----.        par
+00012870: 616d 5f64 6963 743a 2064 6963 745b 7374  am_dict: dict[st
+00012880: 722c 2073 7472 207c 2066 6c6f 6174 5d0a  r, str | float].
+00012890: 2020 2020 2020 2020 2020 2020 4b65 7973              Keys
+000128a0: 2061 7265 2066 6974 2f66 6978 2070 6172   are fit/fix par
+000128b0: 616d 6574 6572 206e 616d 6573 2028 7365  ameter names (se
+000128c0: 6520 636c 6173 732e 5041 524e 414d 4553  e class.PARNAMES
+000128d0: 295c 6e0a 2020 2020 2020 2020 2020 2020  )\n.            
+000128e0: 5661 6c75 6573 2061 7265 2065 6974 6865  Values are eithe
+000128f0: 7220 666c 6f61 7420 2861 6374 7561 6c20  r float (actual 
+00012900: 7661 6c75 6529 206f 7220 7468 6520 7374  value) or the st
+00012910: 7269 6e67 2027 6775 6573 7327 0a0a 2020  ring 'guess'..  
+00012920: 2020 2020 2020 5265 7475 726e 730a 2020        Returns.  
+00012930: 2020 2020 2020 2d2d 2d2d 2d2d 2d0a 2020        -------.  
+00012940: 2020 2020 2020 6469 6374 5b73 7472 2c20        dict[str, 
+00012950: 666c 6f61 745d 0a20 2020 2020 2020 2020  float].         
+00012960: 2020 204b 6579 7320 6172 6520 6669 742f     Keys are fit/
+00012970: 6669 7820 7061 7261 6d65 7465 7220 6e61  fix parameter na
+00012980: 6d65 7320 2873 6565 2063 6c61 7373 2e50  mes (see class.P
+00012990: 4152 4e41 4d45 5329 5c6e 0a20 2020 2020  ARNAMES)\n.     
+000129a0: 2020 2020 2020 2056 616c 7565 7320 6172         Values ar
+000129b0: 6520 666c 6f61 7420 2861 6374 7561 6c20  e float (actual 
+000129c0: 7661 6c75 6529 2077 6869 6368 2061 7265  value) which are
+000129d0: 2069 6e69 7469 616c 2076 616c 7565 7320   initial values 
+000129e0: 6f66 0a20 2020 2020 2020 2020 2020 2070  of.            p
+000129f0: 6172 616d 6574 6572 0a20 2020 2020 2020  arameter.       
+00012a00: 2027 2727 0a20 2020 2020 2020 2072 6169   '''.        rai
+00012a10: 7365 204e 6f74 496d 706c 656d 656e 7465  se NotImplemente
+00012a20: 6445 7272 6f72 0a0a 2020 2020 6465 6620  dError..    def 
+00012a30: 5f5f 696e 6974 5f5f 2873 656c 662c 2066  __init__(self, f
+00012a40: 6974 5f76 6172 733a 2064 6963 745b 7374  it_vars: dict[st
+00012a50: 722c 2066 6c6f 6174 207c 2073 7472 5d2c  r, float | str],
+00012a60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012a70: 2020 6669 785f 7661 7273 3a20 6469 6374    fix_vars: dict
+00012a80: 5b73 7472 2c20 666c 6f61 7420 7c20 7374  [str, float | st
+00012a90: 725d 293a 0a20 2020 2020 2020 2027 2727  r]):.        '''
+00012aa0: 0a20 2020 2020 2020 2053 6574 2064 6566  .        Set def
+00012ab0: 6175 6c74 2076 616c 7565 7320 666f 7220  ault values for 
+00012ac0: 6d61 6e64 6174 6f72 7920 6174 7472 6962  mandatory attrib
+00012ad0: 7574 6573 0a20 2020 2020 2020 2027 2727  utes.        '''
+00012ae0: 0a0a 2020 2020 2020 2020 2320 5265 706c  ..        # Repl
+00012af0: 6163 6520 616e 7920 2767 7565 7373 2720  ace any 'guess' 
+00012b00: 7374 7269 6e67 7320 7769 7468 2070 726f  strings with pro
+00012b10: 7065 7220 6775 6573 7365 730a 2020 2020  per guesses.    
+00012b20: 2020 2020 7365 6c66 2e66 6974 5f76 6172      self.fit_var
+00012b30: 7320 3d20 7365 6c66 2e73 6574 5f69 6e69  s = self.set_ini
+00012b40: 7469 616c 5f76 616c 7328 6669 745f 7661  tial_vals(fit_va
+00012b50: 7273 290a 2020 2020 2020 2020 7365 6c66  rs).        self
+00012b60: 2e66 6978 5f76 6172 7320 3d20 7365 6c66  .fix_vars = self
+00012b70: 2e73 6574 5f69 6e69 7469 616c 5f76 616c  .set_initial_val
+00012b80: 7328 6669 785f 7661 7273 290a 0a20 2020  s(fix_vars)..   
+00012b90: 2020 2020 2023 2043 6865 636b 2061 6c6c       # Check all
+00012ba0: 2050 4152 4e41 4d45 5320 6172 6520 7072   PARNAMES are pr
+00012bb0: 6f76 6964 6564 2069 6e20 6669 742b 6669  ovided in fit+fi
+00012bc0: 780a 2020 2020 2020 2020 696e 7075 745f  x.        input_
+00012bd0: 6e61 6d65 7320 3d20 5b0a 2020 2020 2020  names = [.      
+00012be0: 2020 2020 2020 6e61 6d65 2066 6f72 206e        name for n
+00012bf0: 616d 6520 696e 207b 2a2a 7365 6c66 2e66  ame in {**self.f
+00012c00: 6974 5f76 6172 732c 202a 2a73 656c 662e  it_vars, **self.
+00012c10: 6669 785f 7661 7273 7d2e 6b65 7973 2829  fix_vars}.keys()
+00012c20: 0a20 2020 2020 2020 205d 0a0a 2020 2020  .        ]..    
+00012c30: 2020 2020 6966 2061 6e79 285b 7265 715f      if any([req_
+00012c40: 6e61 6d65 206e 6f74 2069 6e20 696e 7075  name not in inpu
+00012c50: 745f 6e61 6d65 7320 666f 7220 7265 715f  t_names for req_
+00012c60: 6e61 6d65 2069 6e20 7365 6c66 2e50 4152  name in self.PAR
+00012c70: 4e41 4d45 535d 293a 0a20 2020 2020 2020  NAMES]):.       
+00012c80: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+00012c90: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
+00012ca0: 2020 2020 2020 2027 4d69 7373 696e 6720         'Missing 
+00012cb0: 6669 742f 6669 7820 7061 7261 6d65 7465  fit/fix paramete
+00012cc0: 7273 2069 6e20 7b7d 204d 6f64 656c 272e  rs in {} Model'.
+00012cd0: 666f 726d 6174 280a 2020 2020 2020 2020  format(.        
+00012ce0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00012cf0: 2e4e 414d 450a 2020 2020 2020 2020 2020  .NAME.          
+00012d00: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00012d10: 2020 2020 290a 0a20 2020 2020 2020 2023      )..        #
+00012d20: 2046 696e 616c 206d 6f64 656c 2070 6172   Final model par
+00012d30: 616d 6574 6572 2076 616c 7565 730a 2020  ameter values.  
+00012d40: 2020 2020 2020 2320 6669 7474 6564 2061        # fitted a
+00012d50: 6e64 2066 6978 6564 0a20 2020 2020 2020  nd fixed.       
+00012d60: 2073 656c 662e 5f66 696e 616c 5f76 6172   self._final_var
+00012d70: 5f76 616c 7565 7320 3d20 7b0a 2020 2020  _values = {.    
+00012d80: 2020 2020 2020 2020 7661 723a 204e 6f6e          var: Non
+00012d90: 650a 2020 2020 2020 2020 2020 2020 666f  e.            fo
+00012da0: 7220 7661 7220 696e 2073 656c 662e 5041  r var in self.PA
+00012db0: 524e 414d 4553 0a20 2020 2020 2020 207d  RNAMES.        }
+00012dc0: 0a0a 2020 2020 2020 2020 2320 4669 7420  ..        # Fit 
+00012dd0: 7374 6174 7573 2061 6e64 2074 656d 7065  status and tempe
+00012de0: 7261 7475 7265 0a20 2020 2020 2020 2073  rature.        s
+00012df0: 656c 662e 5f66 6974 5f73 7461 7475 7320  elf._fit_status 
+00012e00: 3d20 4661 6c73 650a 0a20 2020 2020 2020  = False..       
+00012e10: 2023 2046 6974 2073 7461 6e64 6172 6420   # Fit standard 
+00012e20: 6465 7669 6174 696f 6e0a 2020 2020 2020  deviation.      
+00012e30: 2020 7365 6c66 2e5f 6669 745f 7374 6465    self._fit_stde
+00012e40: 7620 3d20 7b0a 2020 2020 2020 2020 2020  v = {.          
+00012e50: 2020 7661 723a 204e 6f6e 650a 2020 2020    var: None.    
+00012e60: 2020 2020 2020 2020 666f 7220 7661 7220          for var 
+00012e70: 696e 2073 656c 662e 6669 745f 7661 7273  in self.fit_vars
+00012e80: 2e6b 6579 7328 290a 2020 2020 2020 2020  .keys().        
+00012e90: 7d0a 0a20 2020 2020 2020 2072 6574 7572  }..        retur
+00012ea0: 6e0a 0a20 2020 2040 7072 6f70 6572 7479  n..    @property
+00012eb0: 0a20 2020 2064 6566 2066 6974 5f73 7461  .    def fit_sta
+00012ec0: 7475 7328 7365 6c66 2920 2d3e 2062 6f6f  tus(self) -> boo
+00012ed0: 6c3a 0a20 2020 2020 2020 2027 5472 7565  l:.        'True
+00012ee0: 2069 6620 6669 7420 7375 6363 6573 7366   if fit successf
+00012ef0: 756c 2c20 656c 7365 2046 616c 7365 270a  ul, else False'.
+00012f00: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00012f10: 656c 662e 5f66 6974 5f73 7461 7475 730a  elf._fit_status.
+00012f20: 0a20 2020 2040 6669 745f 7374 6174 7573  .    @fit_status
+00012f30: 2e73 6574 7465 720a 2020 2020 6465 6620  .setter.    def 
+00012f40: 6669 745f 7374 6174 7573 2873 656c 662c  fit_status(self,
+00012f50: 2076 616c 7565 293a 0a20 2020 2020 2020   value):.       
+00012f60: 2069 6620 7479 7065 2876 616c 7565 2920   if type(value) 
+00012f70: 3d3d 2062 6f6f 6c3a 0a20 2020 2020 2020  == bool:.       
+00012f80: 2020 2020 2073 656c 662e 5f66 6974 5f73       self._fit_s
+00012f90: 7461 7475 7320 3d20 7661 6c75 650a 2020  tatus = value.  
+00012fa0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00012fb0: 2020 2020 2020 2020 7261 6973 6520 5479          raise Ty
+00012fc0: 7065 4572 726f 720a 2020 2020 2020 2020  peError.        
+00012fd0: 7265 7475 726e 0a0a 2020 2020 4070 726f  return..    @pro
+00012fe0: 7065 7274 790a 2020 2020 6465 6620 6669  perty.    def fi
+00012ff0: 6e61 6c5f 7661 725f 7661 6c75 6573 2873  nal_var_values(s
+00013000: 656c 6629 202d 3e20 666c 6f61 743a 0a20  elf) -> float:. 
+00013010: 2020 2020 2020 2027 4669 6e61 6c20 7661         'Final va
+00013020: 6c75 6573 206f 6620 7061 7261 6d65 7465  lues of paramete
+00013030: 7273 2c20 626f 7468 2066 6974 7465 6420  rs, both fitted 
+00013040: 616e 6420 6669 7865 6427 0a20 2020 2020  and fixed'.     
+00013050: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+00013060: 6669 6e61 6c5f 7661 725f 7661 6c75 6573  final_var_values
+00013070: 0a0a 2020 2020 4066 696e 616c 5f76 6172  ..    @final_var
+00013080: 5f76 616c 7565 732e 7365 7474 6572 0a20  _values.setter. 
+00013090: 2020 2064 6566 2066 696e 616c 5f76 6172     def final_var
+000130a0: 5f76 616c 7565 7328 7365 6c66 2c20 7661  _values(self, va
+000130b0: 6c75 6529 3a0a 2020 2020 2020 2020 6966  lue):.        if
+000130c0: 2074 7970 6528 7661 6c75 6529 203d 3d20   type(value) == 
+000130d0: 6469 6374 3a0a 2020 2020 2020 2020 2020  dict:.          
+000130e0: 2020 7365 6c66 2e5f 6669 6e61 6c5f 7661    self._final_va
+000130f0: 725f 7661 6c75 6573 203d 2076 616c 7565  r_values = value
+00013100: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00013110: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00013120: 2054 7970 6545 7272 6f72 0a20 2020 2020   TypeError.     
+00013130: 2020 2072 6574 7572 6e0a 0a20 2020 2040     return..    @
+00013140: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
+00013150: 2066 6974 5f73 7464 6576 2873 656c 6629   fit_stdev(self)
+00013160: 202d 3e20 666c 6f61 743a 0a20 2020 2020   -> float:.     
+00013170: 2020 2027 5374 616e 6461 7264 2064 6576     'Standard dev
+00013180: 6961 7469 6f6e 206f 6e20 6669 7474 6564  iation on fitted
+00013190: 2070 6172 616d 6574 6572 732c 2066 726f   parameters, fro
+000131a0: 6d20 6669 7474 696e 6720 726f 7574 696e  m fitting routin
+000131b0: 6527 0a20 2020 2020 2020 2072 6574 7572  e'.        retur
+000131c0: 6e20 7365 6c66 2e5f 6669 745f 7374 6465  n self._fit_stde
+000131d0: 760a 0a20 2020 2040 6669 745f 7374 6465  v..    @fit_stde
+000131e0: 762e 7365 7474 6572 0a20 2020 2064 6566  v.setter.    def
+000131f0: 2066 6974 5f73 7464 6576 2873 656c 662c   fit_stdev(self,
+00013200: 2076 616c 7565 293a 0a20 2020 2020 2020   value):.       
+00013210: 2069 6620 7479 7065 2876 616c 7565 2920   if type(value) 
+00013220: 3d3d 2064 6963 743a 0a20 2020 2020 2020  == dict:.       
+00013230: 2020 2020 2073 656c 662e 5f66 6974 5f73       self._fit_s
+00013240: 7464 6576 203d 2076 616c 7565 0a20 2020  tdev = value.   
+00013250: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00013260: 2020 2020 2020 2072 6169 7365 2054 7970         raise Typ
+00013270: 6545 7272 6f72 0a20 2020 2020 2020 2072  eError.        r
+00013280: 6574 7572 6e0a 0a20 2020 2040 7072 6f70  eturn..    @prop
+00013290: 6572 7479 0a20 2020 2064 6566 2066 6978  erty.    def fix
+000132a0: 5f76 6172 7328 7365 6c66 2920 2d3e 2066  _vars(self) -> f
+000132b0: 6c6f 6174 3a0a 2020 2020 2020 2020 2727  loat:.        ''
+000132c0: 270a 2020 2020 2020 2020 5061 7261 6d65  '.        Parame
+000132d0: 7465 7273 2074 6f20 6669 7820 2869 2e65  ters to fix (i.e
+000132e0: 2e20 6e6f 7420 6669 7429 0a20 2020 2020  . not fit).     
+000132f0: 2020 206b 6579 7320 6172 6520 6e61 6d65     keys are name
+00013300: 7320 696e 2050 4152 4e41 4d45 532c 2076  s in PARNAMES, v
+00013310: 616c 7565 7320 6172 6520 7661 6c75 6573  alues are values
+00013320: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
+00013330: 2020 2020 2023 2043 6865 636b 2066 6f72       # Check for
+00013340: 2069 6d70 6c65 6d65 6e74 6174 696f 6e20   implementation 
+00013350: 696e 204d 6f64 656c 2063 6c61 7373 2069  in Model class i
+00013360: 6e69 740a 2020 2020 2020 2020 7265 7475  nit.        retu
+00013370: 726e 2073 656c 662e 5f66 6978 5f76 6172  rn self._fix_var
+00013380: 730a 0a20 2020 2040 6669 785f 7661 7273  s..    @fix_vars
+00013390: 2e73 6574 7465 720a 2020 2020 6465 6620  .setter.    def 
+000133a0: 6669 785f 7661 7273 2873 656c 662c 2076  fix_vars(self, v
+000133b0: 616c 7565 293a 0a20 2020 2020 2020 2069  alue):.        i
+000133c0: 6620 7479 7065 2876 616c 7565 2920 3d3d  f type(value) ==
+000133d0: 2064 6963 743a 0a20 2020 2020 2020 2020   dict:.         
+000133e0: 2020 2069 6620 616e 7928 5b6b 6579 206e     if any([key n
+000133f0: 6f74 2069 6e20 7365 6c66 2e50 4152 4e41  ot in self.PARNA
+00013400: 4d45 5320 666f 7220 6b65 7920 696e 2076  MES for key in v
+00013410: 616c 7565 2e6b 6579 7328 295d 293a 0a20  alue.keys()]):. 
+00013420: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00013430: 6169 7365 204b 6579 4572 726f 7228 2755  aise KeyError('U
+00013440: 6e6b 6e6f 776e 2076 6172 6961 626c 6520  nknown variable 
+00013450: 6e61 6d65 7320 7072 6f76 6964 6564 2074  names provided t
+00013460: 6f20 6669 7827 290a 2020 2020 2020 2020  o fix').        
+00013470: 2020 2020 7365 6c66 2e5f 6669 785f 7661      self._fix_va
+00013480: 7273 203d 2076 616c 7565 0a20 2020 2020  rs = value.     
+00013490: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+000134a0: 2020 2020 2072 6169 7365 2054 7970 6545       raise TypeE
+000134b0: 7272 6f72 2827 6669 7820 6d75 7374 2062  rror('fix must b
+000134c0: 6520 6469 6374 696f 6e61 7279 2729 0a20  e dictionary'). 
+000134d0: 2020 2020 2020 2072 6574 7572 6e0a 0a20         return.. 
+000134e0: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+000134f0: 2064 6566 2066 6974 5f76 6172 7328 7365   def fit_vars(se
+00013500: 6c66 2920 2d3e 2066 6c6f 6174 3a0a 2020  lf) -> float:.  
+00013510: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
+00013520: 2020 5061 7261 6d65 7465 7273 2074 6f20    Parameters to 
+00013530: 6669 740a 2020 2020 2020 2020 6b65 7973  fit.        keys
+00013540: 2061 7265 206e 616d 6573 2069 6e20 5041   are names in PA
+00013550: 524e 414d 4553 2c20 7661 6c75 6573 2061  RNAMES, values a
+00013560: 7265 2076 616c 7565 730a 2020 2020 2020  re values.      
+00013570: 2020 2727 270a 2020 2020 2020 2020 2320    '''.        # 
+00013580: 4368 6563 6b20 666f 7220 696d 706c 656d  Check for implem
+00013590: 656e 7461 7469 6f6e 2069 6e20 4d6f 6465  entation in Mode
+000135a0: 6c20 636c 6173 7320 696e 6974 0a20 2020  l class init.   
+000135b0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+000135c0: 2e5f 6669 745f 7661 7273 0a0a 2020 2020  ._fit_vars..    
+000135d0: 4066 6974 5f76 6172 732e 7365 7474 6572  @fit_vars.setter
+000135e0: 0a20 2020 2064 6566 2066 6974 5f76 6172  .    def fit_var
+000135f0: 7328 7365 6c66 2c20 7661 6c75 6529 3a0a  s(self, value):.
+00013600: 2020 2020 2020 2020 6966 2074 7970 6528          if type(
+00013610: 7661 6c75 6529 203d 3d20 6469 6374 3a0a  value) == dict:.
+00013620: 2020 2020 2020 2020 2020 2020 6966 2061              if a
+00013630: 6e79 285b 6b65 7920 6e6f 7420 696e 2073  ny([key not in s
+00013640: 656c 662e 5041 524e 414d 4553 2066 6f72  elf.PARNAMES for
+00013650: 206b 6579 2069 6e20 7661 6c75 652e 6b65   key in value.ke
+00013660: 7973 2829 5d29 3a0a 2020 2020 2020 2020  ys()]):.        
+00013670: 2020 2020 2020 2020 7261 6973 6520 4b65          raise Ke
+00013680: 7945 7272 6f72 2827 556e 6b6e 6f77 6e20  yError('Unknown 
+00013690: 7661 7269 6162 6c65 206e 616d 6573 2070  variable names p
+000136a0: 726f 7669 6465 6420 746f 2066 6974 2729  rovided to fit')
+000136b0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000136c0: 662e 5f66 6974 5f76 6172 7320 3d20 7661  f._fit_vars = va
+000136d0: 6c75 650a 2020 2020 2020 2020 656c 7365  lue.        else
+000136e0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+000136f0: 6973 6520 5479 7065 4572 726f 7228 2746  ise TypeError('F
+00013700: 6974 206d 7573 7420 6265 2064 6963 7469  it must be dicti
+00013710: 6f6e 6172 7927 290a 2020 2020 2020 2020  onary').        
+00013720: 7265 7475 726e 0a0a 2020 2020 4063 6c61  return..    @cla
+00013730: 7373 6d65 7468 6f64 0a20 2020 2064 6566  ssmethod.    def
+00013740: 2072 6573 6964 7561 6c73 2863 6c73 2c20   residuals(cls, 
+00013750: 7061 7261 6d73 3a20 6469 6374 5b73 7472  params: dict[str
+00013760: 2c20 666c 6f61 745d 2c20 7465 6d70 6572  , float], temper
+00013770: 6174 7572 6573 3a20 6e70 742e 4172 7261  atures: npt.Arra
+00013780: 794c 696b 652c 0a20 2020 2020 2020 2020  yLike,.         
+00013790: 2020 2020 2020 2020 2074 7275 655f 6c6f           true_lo
+000137a0: 6772 6174 653a 206e 7074 2e41 7272 6179  grate: npt.Array
+000137b0: 4c69 6b65 2920 2d3e 206e 7074 2e4e 4441  Like) -> npt.NDA
+000137c0: 7272 6179 3a0a 2020 2020 2020 2020 2727  rray:.        ''
+000137d0: 270a 2020 2020 2020 2020 4361 6c63 756c  '.        Calcul
+000137e0: 6174 6573 2064 6966 6665 7265 6e63 6520  ates difference 
+000137f0: 6265 7477 6565 6e20 6d65 6173 7572 6564  between measured
+00013800: 206c 6f67 3130 2872 656c 6178 6174 696f   log10(relaxatio
+00013810: 6e20 7261 7465 2920 616e 6420 7472 6961  n rate) and tria
+00013820: 6c0a 2020 2020 2020 2020 6672 6f6d 206d  l.        from m
+00013830: 6f64 656c 0a0a 2020 2020 2020 2020 5061  odel..        Pa
+00013840: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
+00013850: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+00013860: 2020 2020 7061 7261 6d73 3a20 6172 7261      params: arra
+00013870: 795f 6c69 6b65 0a20 2020 2020 2020 2020  y_like.         
+00013880: 2020 206d 6f64 656c 2070 6172 616d 6574     model paramet
+00013890: 6572 2076 616c 7565 730a 2020 2020 2020  er values.      
+000138a0: 2020 7465 6d70 6572 6174 7572 6573 3a20    temperatures: 
+000138b0: 6172 7261 795f 6c69 6b65 0a20 2020 2020  array_like.     
+000138c0: 2020 2020 2020 2054 656d 7065 7261 7475         Temperatu
+000138d0: 7265 2076 616c 7565 7320 284b 2920 6174  re values (K) at
+000138e0: 2077 6869 6368 206d 6f64 656c 2066 756e   which model fun
+000138f0: 6374 696f 6e20 6973 2065 7661 6c75 6174  ction is evaluat
+00013900: 6564 0a20 2020 2020 2020 2074 7275 655f  ed.        true_
+00013910: 6c6f 6772 6174 653a 2061 7272 6179 5f6c  lograte: array_l
+00013920: 696b 650a 2020 2020 2020 2020 2020 2020  ike.            
+00013930: 7472 7565 2028 6578 7065 7269 6d65 6e74  true (experiment
+00013940: 616c 2920 7661 6c75 6573 206f 6620 6c6f  al) values of lo
+00013950: 6731 3028 7265 6c61 7861 7469 6f6e 2072  g10(relaxation r
+00013960: 6174 6529 0a0a 2020 2020 2020 2020 5265  ate)..        Re
+00013970: 7475 726e 730a 2020 2020 2020 2020 2d2d  turns.        --
+00013980: 2d2d 2d2d 2d0a 2020 2020 2020 2020 6e64  -----.        nd
+00013990: 6172 7261 7920 6f66 2066 6c6f 6174 730a  array of floats.
+000139a0: 2020 2020 2020 2020 2020 2020 5265 7369              Resi
+000139b0: 6475 616c 730a 2020 2020 2020 2020 2727  duals.        ''
+000139c0: 270a 0a20 2020 2020 2020 2023 2043 616c  '..        # Cal
+000139d0: 6375 6c61 7465 206d 6f64 656c 206c 6f67  culate model log
+000139e0: 3130 2872 656c 6178 6174 696f 6e20 7261  10(relaxation ra
+000139f0: 7465 2920 7573 696e 6720 7061 7261 6d65  te) using parame
+00013a00: 7465 7273 0a20 2020 2020 2020 2074 7269  ters.        tri
+00013a10: 616c 5f6c 6f67 7261 7465 203d 2063 6c73  al_lograte = cls
+00013a20: 2e6d 6f64 656c 2870 6172 616d 732c 2074  .model(params, t
+00013a30: 656d 7065 7261 7475 7265 7329 0a0a 2020  emperatures)..  
+00013a40: 2020 2020 2020 7265 7369 6475 616c 7320        residuals 
+00013a50: 3d20 7472 6961 6c5f 6c6f 6772 6174 6520  = trial_lograte 
+00013a60: 2d20 7472 7565 5f6c 6f67 7261 7465 0a0a  - true_lograte..
+00013a70: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+00013a80: 6573 6964 7561 6c73 0a0a 2020 2020 4063  esiduals..    @c
+00013a90: 6c61 7373 6d65 7468 6f64 0a20 2020 2064  lassmethod.    d
+00013aa0: 6566 2072 6573 6964 7561 6c5f 6672 6f6d  ef residual_from
+00013ab0: 5f66 6c6f 6174 5f6c 6973 7428 636c 732c  _float_list(cls,
+00013ac0: 206e 6577 5f76 616c 733a 206e 7074 2e41   new_vals: npt.A
+00013ad0: 7272 6179 4c69 6b65 2c0a 2020 2020 2020  rrayLike,.      
+00013ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013af0: 2020 2020 2020 2020 2020 2066 6974 5f76             fit_v
+00013b00: 6172 733a 2064 6963 745b 7374 722c 2066  ars: dict[str, f
+00013b10: 6c6f 6174 5d2c 0a20 2020 2020 2020 2020  loat],.         
+00013b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013b30: 2020 2020 2020 2020 6669 785f 7661 7273          fix_vars
+00013b40: 3a20 6469 6374 5b73 7472 2c20 666c 6f61  : dict[str, floa
+00013b50: 745d 2c0a 2020 2020 2020 2020 2020 2020  t],.            
+00013b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013b70: 2020 2020 2074 656d 7065 7261 7475 7265       temperature
+00013b80: 733a 206e 7074 2e41 7272 6179 4c69 6b65  s: npt.ArrayLike
+00013b90: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00013ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013bb0: 2020 206c 6f67 7261 7465 3a20 6e70 742e     lograte: npt.
+00013bc0: 4172 7261 794c 696b 652c 0a20 2020 2020  ArrayLike,.     
+00013bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013be0: 2020 2020 2020 2020 2020 2020 7369 676d              sigm
+00013bf0: 613a 206e 7074 2e41 7272 6179 4c69 6b65  a: npt.ArrayLike
+00013c00: 203d 205b 5d29 202d 3e20 6e70 742e 4e44   = []) -> npt.ND
+00013c10: 4172 7261 793a 0a20 2020 2020 2020 2027  Array:.        '
+00013c20: 2727 0a20 2020 2020 2020 2057 7261 7070  ''.        Wrapp
+00013c30: 6572 2066 6f72 2060 7265 7369 6475 616c  er for `residual
+00013c40: 7360 206d 6574 686f 642c 2074 616b 6573  s` method, takes
+00013c50: 206e 6577 2076 616c 7565 7320 6672 6f6d   new values from
+00013c60: 2073 6369 7079 0a20 2020 2020 2020 206c   scipy.        l
+00013c70: 6561 7374 5f73 7175 6172 6573 2077 6869  east_squares whi
+00013c80: 6368 2070 726f 7669 6465 7320 6c69 7374  ch provides list
+00013c90: 5b66 6c6f 6174 5d2c 2074 6f20 636f 6e73  [float], to cons
+00013ca0: 7472 7563 7420 6e65 770a 2020 2020 2020  truct new.      
+00013cb0: 2020 6669 745f 7661 7273 2064 6963 742c    fit_vars dict,
+00013cc0: 2074 6865 6e20 7275 6e73 2060 7265 7369   then runs `resi
+00013cd0: 6475 616c 7360 206d 6574 686f 642e 0a0a  duals` method...
+00013ce0: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+00013cf0: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
+00013d00: 2d2d 2d2d 2d0a 2020 2020 2020 2020 6e65  -----.        ne
+00013d10: 775f 7661 6c73 3a20 6172 7261 795f 6c69  w_vals: array_li
+00013d20: 6b65 0a20 2020 2020 2020 2020 2020 2054  ke.            T
+00013d30: 6869 7320 6974 6572 6174 696f 6e27 7320  his iteration's 
+00013d40: 6669 7420 7061 7261 6d65 7465 7220 7661  fit parameter va
+00013d50: 6c75 6573 2070 726f 7669 6465 6420 6279  lues provided by
+00013d60: 206c 6561 7374 5f73 7175 6172 6573 0a20   least_squares. 
+00013d70: 2020 2020 2020 2020 2020 2074 6869 7320             this 
+00013d80: 6861 7320 7468 6520 7361 6d65 206f 7264  has the same ord
+00013d90: 6572 2061 7420 6669 745f 7661 7273 2e6b  er at fit_vars.k
+00013da0: 6579 730a 2020 2020 2020 2020 6669 745f  eys.        fit_
+00013db0: 7661 7273 3a20 6469 6374 5b73 7472 2c20  vars: dict[str, 
+00013dc0: 666c 6f61 745d 0a20 2020 2020 2020 2020  float].         
+00013dd0: 2020 2050 6172 616d 6574 6572 2074 6f20     Parameter to 
+00013de0: 6669 7420 696e 206d 6f64 656c 2066 756e  fit in model fun
+00013df0: 6374 696f 6e5c 6e0a 2020 2020 2020 2020  ction\n.        
+00013e00: 2020 2020 6b65 7973 2061 7265 2050 4152      keys are PAR
+00013e10: 4e41 4d45 532c 2076 616c 7565 7320 6172  NAMES, values ar
+00013e20: 6520 666c 6f61 7420 7661 6c75 6573 0a20  e float values. 
+00013e30: 2020 2020 2020 2066 6978 5f76 6172 733a         fix_vars:
+00013e40: 2064 6963 745b 7374 722c 2066 6c6f 6174   dict[str, float
+00013e50: 5d0a 2020 2020 2020 2020 2020 2020 5061  ].            Pa
+00013e60: 7261 6d65 7465 7220 7768 6963 6820 7265  rameter which re
+00013e70: 6d61 696e 2066 6978 6564 2069 6e20 6d6f  main fixed in mo
+00013e80: 6465 6c20 6675 6e63 7469 6f6e 5c6e 0a20  del function\n. 
+00013e90: 2020 2020 2020 2020 2020 206b 6579 7320             keys 
+00013ea0: 6172 6520 5041 524e 414d 4553 2c20 7661  are PARNAMES, va
+00013eb0: 6c75 6573 2061 7265 2066 6c6f 6174 2076  lues are float v
+00013ec0: 616c 7565 730a 2020 2020 2020 2020 7465  alues.        te
+00013ed0: 6d70 6572 6174 7572 6573 3a20 6172 7261  mperatures: arra
+00013ee0: 795f 6c69 6b65 0a20 2020 2020 2020 2020  y_like.         
+00013ef0: 2020 2054 656d 7065 7261 7475 7265 2076     Temperature v
+00013f00: 616c 7565 7320 284b 2920 6174 2077 6869  alues (K) at whi
+00013f10: 6368 206d 6f64 656c 2066 756e 6374 696f  ch model functio
+00013f20: 6e20 6973 2065 7661 6c75 6174 6564 0a20  n is evaluated. 
+00013f30: 2020 2020 2020 206c 6f67 7261 7465 3a20         lograte: 
+00013f40: 6172 7261 795f 6c69 6b65 0a20 2020 2020  array_like.     
+00013f50: 2020 2020 2020 2054 7275 6520 2865 7870         True (exp
+00013f60: 6572 696d 656e 7461 6c29 2076 616c 7565  erimental) value
+00013f70: 7320 6f66 206c 6f67 3130 2872 656c 6178  s of log10(relax
+00013f80: 6174 696f 6e20 7261 7465 290a 2020 2020  ation rate).    
+00013f90: 2020 2020 7369 676d 613a 2061 7272 6179      sigma: array
+00013fa0: 5f6c 696b 650a 2020 2020 2020 2020 2020  _like.          
+00013fb0: 2020 5374 616e 6461 7264 2064 6576 6961    Standard devia
+00013fc0: 7469 6f6e 206f 6620 7461 7520 696e 206c  tion of tau in l
+00013fd0: 6f67 7370 6163 650a 0a20 2020 2020 2020  ogspace..       
+00013fe0: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
+00013ff0: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
+00014000: 206e 6461 7272 6179 206f 6620 666c 6f61   ndarray of floa
+00014010: 7473 0a20 2020 2020 2020 2020 2020 2052  ts.            R
+00014020: 6573 6964 7561 6c73 0a20 2020 2020 2020  esiduals.       
+00014030: 2027 2727 0a0a 2020 2020 2020 2020 2320   '''..        # 
+00014040: 5377 6170 2066 6974 2076 616c 7565 7320  Swap fit values 
+00014050: 666f 7220 6e65 7720 7661 6c75 6573 2066  for new values f
+00014060: 726f 6d20 6669 7420 726f 7574 696e 650a  rom fit routine.
+00014070: 2020 2020 2020 2020 6e65 775f 6669 745f          new_fit_
+00014080: 7661 7273 203d 207b 0a20 2020 2020 2020  vars = {.       
+00014090: 2020 2020 206e 616d 653a 2067 7565 7373       name: guess
+000140a0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+000140b0: 2067 7565 7373 2c20 6e61 6d65 2069 6e20   guess, name in 
+000140c0: 7a69 7028 6e65 775f 7661 6c73 2c20 6669  zip(new_vals, fi
+000140d0: 745f 7661 7273 2e6b 6579 7328 2929 0a20  t_vars.keys()). 
+000140e0: 2020 2020 2020 207d 0a0a 2020 2020 2020         }..      
+000140f0: 2020 2320 416e 6420 6d61 6b65 2063 6f6d    # And make com
+00014100: 6269 6e65 6420 6469 6374 206f 6620 6669  bined dict of fi
+00014110: 7420 616e 6420 6669 7865 640a 2020 2020  t and fixed.    
+00014120: 2020 2020 2320 7661 7269 6162 6c65 206e      # variable n
+00014130: 616d 6573 2028 6b65 7973 2920 616e 6420  ames (keys) and 
+00014140: 7661 6c75 6573 0a20 2020 2020 2020 2061  values.        a
+00014150: 6c6c 5f76 6172 7320 3d20 7b2a 2a66 6978  ll_vars = {**fix
+00014160: 5f76 6172 732c 202a 2a6e 6577 5f66 6974  _vars, **new_fit
+00014170: 5f76 6172 737d 0a0a 2020 2020 2020 2020  _vars}..        
+00014180: 7265 7369 6475 616c 7320 3d20 636c 732e  residuals = cls.
+00014190: 7265 7369 6475 616c 7328 616c 6c5f 7661  residuals(all_va
+000141a0: 7273 2c20 7465 6d70 6572 6174 7572 6573  rs, temperatures
+000141b0: 2c20 6c6f 6772 6174 6529 0a0a 2020 2020  , lograte)..    
+000141c0: 2020 2020 6966 206c 656e 2873 6967 6d61      if len(sigma
+000141d0: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
+000141e0: 6573 6964 7561 6c73 202f 3d20 7369 676d  esiduals /= sigm
+000141f0: 610a 0a20 2020 2020 2020 2072 6574 7572  a..        retur
+00014200: 6e20 7265 7369 6475 616c 730a 0a20 2020  n residuals..   
+00014210: 2064 6566 2066 6974 5f74 6f28 7365 6c66   def fit_to(self
+00014220: 2c20 6461 7461 7365 743a 2054 6175 5444  , dataset: TauTD
+00014230: 6174 6173 6574 2c0a 2020 2020 2020 2020  ataset,.        
+00014240: 2020 2020 2020 2067 7565 7373 3a20 7374         guess: st
+00014250: 7220 7c20 6469 6374 5b73 7472 2c20 666c  r | dict[str, fl
+00014260: 6f61 745d 203d 2027 7072 6564 6566 696e  oat] = 'predefin
+00014270: 6564 272c 0a20 2020 2020 2020 2020 2020  ed',.           
+00014280: 2020 2020 7665 7262 6f73 653a 2062 6f6f      verbose: boo
+00014290: 6c20 3d20 5472 7565 2920 2d3e 204e 6f6e  l = True) -> Non
+000142a0: 653a 0a20 2020 2020 2020 2027 2727 0a20  e:.        '''. 
+000142b0: 2020 2020 2020 2046 6974 7320 6d6f 6465         Fits mode
+000142c0: 6c20 746f 2044 6174 6173 6574 0a0a 2020  l to Dataset..  
+000142d0: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
+000142e0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+000142f0: 2d2d 2d0a 2020 2020 2020 2020 6461 7461  ---.        data
+00014300: 7365 743a 2054 6175 5444 6174 6173 6574  set: TauTDataset
+00014310: 0a20 2020 2020 2020 2020 2020 2044 6174  .            Dat
+00014320: 6173 6574 2074 6f20 7768 6963 6820 6120  aset to which a 
+00014330: 6d6f 6465 6c20 6f66 2072 6174 6520 7673  model of rate vs
+00014340: 2074 656d 7065 7261 7475 7265 2077 696c   temperature wil
+00014350: 6c20 6265 2066 6974 7465 640a 2020 2020  l be fitted.    
+00014360: 2020 2020 6775 6573 733a 2073 7472 207c      guess: str |
+00014370: 2064 6963 745b 7374 722c 2066 6c6f 6174   dict[str, float
+00014380: 5d2c 2064 6566 6175 6c74 2027 7072 6564  ], default 'pred
+00014390: 6566 696e 6564 270a 2020 2020 2020 2020  efined'.        
+000143a0: 2020 2020 4569 7468 6572 2073 7472 696e      Either strin
+000143b0: 6720 2770 7265 6465 6669 6e65 6427 2c20  g 'predefined', 
+000143c0: 6f72 2064 6963 7420 6f66 2069 6e69 7469  or dict of initi
+000143d0: 616c 2070 6172 616d 6574 6572 730a 2020  al parameters.  
+000143e0: 2020 2020 2020 2020 2020 7573 6564 2061            used a
+000143f0: 7320 7374 6172 7469 6e67 2067 7565 7373  s starting guess
+00014400: 2077 6974 6820 6b65 7973 2061 7320 7061   with keys as pa
+00014410: 7261 6d65 7465 7220 6e61 6d65 7320 616e  rameter names an
+00014420: 6420 7661 6c75 6573 2061 730a 2020 2020  d values as.    
+00014430: 2020 2020 2020 2020 6e75 6d65 7269 6361          numerica
+00014440: 6c20 7661 6c75 6573 0a20 2020 2020 2020  l values.       
+00014450: 2076 6572 626f 7365 3a20 626f 6f6c 2c20   verbose: bool, 
+00014460: 6465 6661 756c 7420 5472 7565 0a20 2020  default True.   
+00014470: 2020 2020 2020 2020 2049 6620 5472 7565           If True
+00014480: 2c20 7072 696e 7473 2069 6e66 6f72 6d61  , prints informa
+00014490: 7469 6f6e 2074 6f20 7465 726d 696e 616c  tion to terminal
+000144a0: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+000144b0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+000144c0: 2d0a 2020 2020 2020 2020 4e6f 6e65 0a20  -.        None. 
+000144d0: 2020 2020 2020 2027 2727 0a0a 2020 2020         '''..    
+000144e0: 2020 2020 2320 4765 7420 7374 6172 7469      # Get starti
+000144f0: 6e67 2067 7565 7373 6573 2c20 6569 7468  ng guesses, eith
+00014500: 6572 2070 7265 6465 6669 6e65 6420 696e  er predefined in
+00014510: 2073 656c 6620 6f72 2067 6976 656e 0a20   self or given. 
+00014520: 2020 2020 2020 2023 2062 7920 7573 6572         # by user
+00014530: 0a20 2020 2020 2020 2069 6620 6775 6573  .        if gues
+00014540: 7320 213d 2027 7072 6564 6566 696e 6564  s != 'predefined
+00014550: 273a 0a20 2020 2020 2020 2020 2020 2067  ':.            g
+00014560: 7565 7373 203d 205b 0a20 2020 2020 2020  uess = [.       
+00014570: 2020 2020 2020 2020 2067 7565 7373 5b6b           guess[k
+00014580: 6579 5d20 666f 7220 6b65 7920 696e 2073  ey] for key in s
+00014590: 656c 662e 6669 745f 7661 7273 2e6b 6579  elf.fit_vars.key
+000145a0: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
+000145b0: 5d0a 2020 2020 2020 2020 656c 7365 3a0a  ].        else:.
+000145c0: 2020 2020 2020 2020 2020 2020 6775 6573              gues
+000145d0: 7320 3d20 5b76 616c 2066 6f72 2076 616c  s = [val for val
+000145e0: 2069 6e20 7365 6c66 2e66 6974 5f76 6172   in self.fit_var
+000145f0: 732e 7661 6c75 6573 2829 5d0a 0a20 2020  s.values()]..   
+00014600: 2020 2020 2023 2047 6574 2062 6f75 6e64       # Get bound
+00014610: 7320 666f 7220 7661 7269 6162 6c65 7320  s for variables 
+00014620: 746f 2062 6520 6669 7474 6564 0a20 2020  to be fitted.   
+00014630: 2020 2020 2062 6f75 6e64 7320 3d20 6e70       bounds = np
+00014640: 2e61 7272 6179 285b 0a20 2020 2020 2020  .array([.       
+00014650: 2020 2020 2073 656c 662e 424f 554e 4453       self.BOUNDS
+00014660: 5b6e 616d 655d 0a20 2020 2020 2020 2020  [name].         
+00014670: 2020 2066 6f72 206e 616d 6520 696e 2073     for name in s
+00014680: 656c 662e 6669 745f 7661 7273 2e6b 6579  elf.fit_vars.key
+00014690: 7328 290a 2020 2020 2020 2020 5d29 2e54  s().        ]).T
+000146a0: 0a0a 2020 2020 2020 2020 6375 7272 5f66  ..        curr_f
+000146b0: 6974 203d 206c 6561 7374 5f73 7175 6172  it = least_squar
+000146c0: 6573 280a 2020 2020 2020 2020 2020 2020  es(.            
+000146d0: 7365 6c66 2e72 6573 6964 7561 6c5f 6672  self.residual_fr
+000146e0: 6f6d 5f66 6c6f 6174 5f6c 6973 742c 0a20  om_float_list,. 
+000146f0: 2020 2020 2020 2020 2020 2061 7267 733d             args=
+00014700: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
+00014710: 2020 7365 6c66 2e66 6974 5f76 6172 732c    self.fit_vars,
+00014720: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014730: 2073 656c 662e 6669 785f 7661 7273 2c0a   self.fix_vars,.
+00014740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014750: 6461 7461 7365 742e 7465 6d70 6572 6174  dataset.temperat
+00014760: 7572 6573 2c0a 2020 2020 2020 2020 2020  ures,.          
+00014770: 2020 2020 2020 6e70 2e6c 6f67 3130 2864        np.log10(d
+00014780: 6174 6173 6574 2e72 6174 6573 292c 0a20  ataset.rates),. 
+00014790: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+000147a0: 6174 6173 6574 2e6c 6f67 7261 7465 5f70  ataset.lograte_p
+000147b0: 6d0a 2020 2020 2020 2020 2020 2020 5d2c  m.            ],
+000147c0: 0a20 2020 2020 2020 2020 2020 2078 303d  .            x0=
+000147d0: 6775 6573 732c 0a20 2020 2020 2020 2020  guess,.         
+000147e0: 2020 2062 6f75 6e64 733d 626f 756e 6473     bounds=bounds
+000147f0: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+00014800: 2020 2020 6966 2063 7572 725f 6669 742e      if curr_fit.
+00014810: 7374 6174 7573 203d 3d20 303a 0a20 2020  status == 0:.   
+00014820: 2020 2020 2020 2020 2069 6620 7665 7262           if verb
+00014830: 6f73 653a 0a20 2020 2020 2020 2020 2020  ose:.           
+00014840: 2020 2020 2075 742e 6370 7269 6e74 280a       ut.cprint(.
+00014850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014860: 2020 2020 275c 6e20 4669 7420 6661 696c      '\n Fit fail
+00014870: 6564 202d 2054 6f6f 206d 616e 7920 6974  ed - Too many it
+00014880: 6572 6174 696f 6e73 272c 0a20 2020 2020  erations',.     
+00014890: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+000148a0: 626c 6163 6b5f 7965 6c6c 6f77 6267 270a  black_yellowbg'.
+000148b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000148c0: 290a 0a20 2020 2020 2020 2020 2020 2073  )..            s
+000148d0: 656c 662e 6669 6e61 6c5f 7661 725f 7661  elf.final_var_va
+000148e0: 6c75 6573 203d 207b 0a20 2020 2020 2020  lues = {.       
+000148f0: 2020 2020 2020 2020 206e 616d 653a 2076           name: v
+00014900: 616c 7565 0a20 2020 2020 2020 2020 2020  alue.           
+00014910: 2020 2020 2066 6f72 206e 616d 652c 2076       for name, v
+00014920: 616c 7565 2069 6e20 7a69 7028 7365 6c66  alue in zip(self
+00014930: 2e66 6974 5f76 6172 732c 2063 7572 725f  .fit_vars, curr_
+00014940: 6669 742e 7829 0a20 2020 2020 2020 2020  fit.x).         
+00014950: 2020 207d 0a20 2020 2020 2020 2020 2020     }.           
+00014960: 2073 656c 662e 6669 745f 7374 6465 7620   self.fit_stdev 
+00014970: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
+00014980: 2020 2020 6c61 6265 6c3a 206e 702e 6e61      label: np.na
+00014990: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
+000149a0: 2020 666f 7220 6c61 6265 6c20 696e 2073    for label in s
+000149b0: 656c 662e 6669 745f 7661 7273 2e6b 6579  elf.fit_vars.key
+000149c0: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
+000149d0: 7d0a 2020 2020 2020 2020 2020 2020 7365  }.            se
+000149e0: 6c66 2e66 6974 5f73 7461 7475 7320 3d20  lf.fit_status = 
+000149f0: 4661 6c73 650a 2020 2020 2020 2020 656c  False.        el
+00014a00: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00014a10: 7374 6465 762c 206e 6f5f 7374 6465 7620  stdev, no_stdev 
+00014a20: 3d20 7374 6174 732e 7376 645f 7374 6465  = stats.svd_stde
+00014a30: 7628 6375 7272 5f66 6974 290a 0a20 2020  v(curr_fit)..   
+00014a40: 2020 2020 2020 2020 2023 2053 7461 6e64           # Stand
+00014a50: 6172 6420 6465 7669 6174 696f 6e20 6572  ard deviation er
+00014a60: 726f 7220 6f6e 2074 6865 2070 6172 616d  ror on the param
+00014a70: 6574 6572 730a 2020 2020 2020 2020 2020  eters.          
+00014a80: 2020 7365 6c66 2e66 6974 5f73 7464 6576    self.fit_stdev
+00014a90: 203d 207b 0a20 2020 2020 2020 2020 2020   = {.           
+00014aa0: 2020 2020 206c 6162 656c 3a20 7661 6c0a       label: val.
+00014ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014ac0: 666f 7220 6c61 6265 6c2c 2076 616c 2069  for label, val i
+00014ad0: 6e20 7a69 7028 7365 6c66 2e66 6974 5f76  n zip(self.fit_v
+00014ae0: 6172 732e 6b65 7973 2829 2c20 7374 6465  ars.keys(), stde
+00014af0: 7629 0a20 2020 2020 2020 2020 2020 207d  v).            }
+00014b00: 0a0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00014b10: 6c66 2e66 6974 5f73 7461 7475 7320 3d20  lf.fit_status = 
+00014b20: 5472 7565 0a0a 2020 2020 2020 2020 2020  True..          
+00014b30: 2020 2320 5265 706f 7274 2073 696e 6775    # Report singu
+00014b40: 6c61 7220 7661 6c75 6573 3d30 206f 6620  lar values=0 of 
+00014b50: 4a61 636f 6269 616e 0a20 2020 2020 2020  Jacobian.       
+00014b60: 2020 2020 2023 2061 6e64 2069 6e64 6963       # and indic
+00014b70: 6174 6520 7468 6174 2073 7464 5f64 6576  ate that std_dev
+00014b80: 2063 616e 6e6f 7420 6265 2063 616c 6375   cannot be calcu
+00014b90: 6c61 7465 640a 2020 2020 2020 2020 2020  lated.          
+00014ba0: 2020 666f 7220 7061 722c 2073 6920 696e    for par, si in
+00014bb0: 207a 6970 2873 656c 662e 6669 745f 7661   zip(self.fit_va
+00014bc0: 7273 2e6b 6579 7328 292c 206e 6f5f 7374  rs.keys(), no_st
+00014bd0: 6465 7629 3a0a 2020 2020 2020 2020 2020  dev):.          
+00014be0: 2020 2020 2020 6966 2076 6572 626f 7365        if verbose
+00014bf0: 2061 6e64 206e 6f74 2073 693a 0a20 2020   and not si:.   
+00014c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014c10: 2075 742e 6370 7269 6e74 280a 2020 2020   ut.cprint(.    
+00014c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014c30: 2020 2020 6627 5761 726e 696e 673a 204a      f'Warning: J
+00014c40: 6163 6f62 6961 6e20 6973 2064 6567 656e  acobian is degen
+00014c50: 6572 6174 6520 666f 7220 7b70 6172 7d2c  erate for {par},
+00014c60: 2073 7461 6e64 6172 6420 6465 7669 6174   standard deviat
+00014c70: 696f 6e20 6361 6e6e 6f74 2062 6520 666f  ion cannot be fo
+00014c80: 756e 642c 2061 6e64 2069 7320 7365 7420  und, and is set 
+00014c90: 746f 207a 6572 6f5c 6e27 2c20 2320 6e6f  to zero\n', # no
+00014ca0: 7161 0a20 2020 2020 2020 2020 2020 2020  qa.             
+00014cb0: 2020 2020 2020 2020 2020 2027 626c 6163             'blac
+00014cc0: 6b5f 7965 6c6c 6f77 6267 270a 2020 2020  k_yellowbg'.    
+00014cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014ce0: 290a 0a20 2020 2020 2020 2020 2020 2023  )..            #
+00014cf0: 2053 6574 2066 6974 7465 6420 7661 6c75   Set fitted valu
+00014d00: 6573 0a20 2020 2020 2020 2020 2020 2073  es.            s
+00014d10: 656c 662e 6669 6e61 6c5f 7661 725f 7661  elf.final_var_va
+00014d20: 6c75 6573 203d 207b 0a20 2020 2020 2020  lues = {.       
+00014d30: 2020 2020 2020 2020 206e 616d 653a 2076           name: v
+00014d40: 616c 7565 0a20 2020 2020 2020 2020 2020  alue.           
+00014d50: 2020 2020 2066 6f72 206e 616d 652c 2076       for name, v
+00014d60: 616c 7565 2069 6e20 7a69 7028 7365 6c66  alue in zip(self
+00014d70: 2e66 6974 5f76 6172 732e 6b65 7973 2829  .fit_vars.keys()
+00014d80: 2c20 6375 7272 5f66 6974 2e78 290a 2020  , curr_fit.x).  
+00014d90: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+00014da0: 2020 2020 2020 2020 2320 616e 6420 6669          # and fi
+00014db0: 7865 6420 7661 6c75 6573 0a20 2020 2020  xed values.     
+00014dc0: 2020 2020 2020 2066 6f72 206b 6579 2c20         for key, 
+00014dd0: 7661 6c20 696e 2073 656c 662e 6669 785f  val in self.fix_
+00014de0: 7661 7273 2e69 7465 6d73 2829 3a0a 2020  vars.items():.  
+00014df0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00014e00: 6c66 2e66 696e 616c 5f76 6172 5f76 616c  lf.final_var_val
+00014e10: 7565 735b 6b65 795d 203d 2076 616c 0a0a  ues[key] = val..
+00014e20: 2020 2020 2020 2020 7265 7475 726e 0a0a          return..
+00014e30: 0a63 6c61 7373 204c 6f67 4f72 6261 6368  .class LogOrbach
+00014e40: 4d6f 6465 6c28 4c6f 6754 6175 544d 6f64  Model(LogTauTMod
+00014e50: 656c 293a 0a20 2020 2027 2727 0a20 2020  el):.    '''.   
+00014e60: 204c 6f67 284f 7262 6163 6829 204d 6f64   Log(Orbach) Mod
+00014e70: 656c 206f 6620 6c6f 6731 3028 5265 6c61  el of log10(Rela
+00014e80: 7861 7469 6f6e 2072 6174 6529 2076 7320  xation rate) vs 
+00014e90: 7465 6d70 6572 6174 7572 650a 2020 2020  temperature.    
+00014ea0: 2727 270a 0a20 2020 2023 3a20 4d6f 6465  '''..    #: Mode
+00014eb0: 6c20 6e61 6d65 0a20 2020 204e 414d 4520  l name.    NAME 
+00014ec0: 3d20 274f 7262 6163 6827 0a20 2020 2023  = 'Orbach'.    #
+00014ed0: 3a20 4d6f 6465 6c20 6e61 6d65 2077 6974  : Model name wit
+00014ee0: 6820 6c6f 6720 6272 6163 6b65 7473 0a20  h log brackets. 
+00014ef0: 2020 204c 4e41 4d45 203d 2027 4c6f 6728     LNAME = 'Log(
+00014f00: 4f72 6261 6368 2927 0a0a 2020 2020 233a  Orbach)'..    #:
+00014f10: 204d 6f64 656c 2050 6172 616d 6574 6572   Model Parameter
+00014f20: 206e 616d 6520 7374 7269 6e67 730a 2020   name strings.  
+00014f30: 2020 5041 524e 414d 4553 203d 205b 0a20    PARNAMES = [. 
+00014f40: 2020 2020 2020 2027 755f 6566 6627 2c20         'u_eff', 
+00014f50: 2741 272c 0a20 2020 205d 0a0a 2020 2020  'A',.    ]..    
+00014f60: 233a 204d 6f64 656c 2050 6172 616d 6574  #: Model Paramet
+00014f70: 6572 206e 616d 6520 6d61 7468 6d6f 6465  er name mathmode
+00014f80: 2073 7472 696e 6773 0a20 2020 2056 4152   strings.    VAR
+00014f90: 4e41 4d45 535f 4d4d 203d 207b 0a20 2020  NAMES_MM = {.   
+00014fa0: 2020 2020 2027 755f 6566 6627 3a20 7227       'u_eff': r'
+00014fb0: 2455 5f5c 6d61 7468 7265 6775 6c61 727b  $U_\mathregular{
+00014fc0: 6566 667d 2427 2c0a 2020 2020 2020 2020  eff}$',.        
+00014fd0: 2741 273a 2072 2724 4124 270a 2020 2020  'A': r'$A$'.    
+00014fe0: 7d0a 0a20 2020 2023 3a20 4d6f 6465 6c20  }..    #: Model 
+00014ff0: 5061 7261 6d65 7465 7220 6e61 6d65 2048  Parameter name H
+00015000: 544d 4c20 7374 7269 6e67 730a 2020 2020  TML strings.    
+00015010: 5641 524e 414d 4553 5f48 544d 4c20 3d20  VARNAMES_HTML = 
+00015020: 7b0a 2020 2020 2020 2020 2775 5f65 6666  {.        'u_eff
+00015030: 273a 2027 553c 7375 623e 6566 663c 2f73  ': 'U<sub>eff</s
+00015040: 7562 3e27 2c0a 2020 2020 2020 2020 2741  ub>',.        'A
+00015050: 273a 2027 4127 0a20 2020 207d 0a0a 2020  ': 'A'.    }..  
+00015060: 2020 233a 204d 6f64 656c 2050 6172 616d    #: Model Param
+00015070: 6574 6572 2075 6e69 7420 7374 7269 6e67  eter unit string
+00015080: 730a 2020 2020 554e 4954 5320 3d20 7b0a  s.    UNITS = {.
+00015090: 2020 2020 2020 2020 2775 5f65 6666 273a          'u_eff':
+000150a0: 2072 274b 272c 0a20 2020 2020 2020 2027   r'K',.        '
+000150b0: 4127 3a20 7227 6c6f 6731 305b 735d 270a  A': r'log10[s]'.
+000150c0: 2020 2020 7d0a 0a20 2020 2023 3a20 4d6f      }..    #: Mo
+000150d0: 6465 6c20 5061 7261 6d65 7465 7220 756e  del Parameter un
+000150e0: 6974 206d 6174 686d 6f64 6520 7374 7269  it mathmode stri
+000150f0: 6e67 730a 2020 2020 554e 4954 535f 4d4d  ngs.    UNITS_MM
+00015100: 203d 207b 0a20 2020 2020 2020 2027 755f   = {.        'u_
+00015110: 6566 6627 3a20 7227 245c 6d61 7468 7265  eff': r'$\mathre
+00015120: 6775 6c61 727b 4b7d 2427 2c0a 2020 2020  gular{K}$',.    
+00015130: 2020 2020 2741 273a 2072 2724 5c6c 6f67      'A': r'$\log
+00015140: 5f5c 6d61 7468 7265 6775 6c61 727b 3130  _\mathregular{10
+00015150: 7d5c 6c65 6674 5b5c 6d61 7468 7265 6775  }\left[\mathregu
+00015160: 6c61 727b 737d 5c72 6967 6874 5d24 2720  lar{s}\right]$' 
+00015170: 2320 6e6f 7161 0a20 2020 207d 0a0a 2020  # noqa.    }..  
+00015180: 2020 233a 204d 6f64 656c 2050 6172 616d    #: Model Param
+00015190: 6574 6572 2075 6e69 7420 4854 4d4c 2073  eter unit HTML s
+000151a0: 7472 696e 6773 0a20 2020 2055 4e49 5453  trings.    UNITS
+000151b0: 5f48 544d 4c20 3d20 7b0a 2020 2020 2020  _HTML = {.      
+000151c0: 2020 2775 5f65 6666 273a 2027 4b27 2c0a    'u_eff': 'K',.
+000151d0: 2020 2020 2020 2020 2741 273a 2027 6c6f          'A': 'lo
+000151e0: 673c 7375 623e 3130 3c2f 7375 623e 5b73  g<sub>10</sub>[s
+000151f0: 5d27 0a20 2020 207d 0a0a 2020 2020 233a  ]'.    }..    #:
+00015200: 204d 6f64 656c 2070 6172 616d 6574 6572   Model parameter
+00015210: 2062 6f75 6e64 730a 2020 2020 424f 554e   bounds.    BOUN
+00015220: 4453 203d 207b 0a20 2020 2020 2020 2027  DS = {.        '
+00015230: 755f 6566 6627 3a20 5b30 2e2c 206e 702e  u_eff': [0., np.
+00015240: 696e 665d 2c0a 2020 2020 2020 2020 2741  inf],.        'A
+00015250: 273a 205b 2d33 302c 2030 5d0a 2020 2020  ': [-30, 0].    
+00015260: 7d0a 0a20 2020 2040 7374 6174 6963 6d65  }..    @staticme
+00015270: 7468 6f64 0a20 2020 2064 6566 2073 6574  thod.    def set
+00015280: 5f69 6e69 7469 616c 5f76 616c 7328 7061  _initial_vals(pa
+00015290: 7261 6d5f 6469 6374 3a20 6469 6374 5b73  ram_dict: dict[s
+000152a0: 7472 2c20 7374 7220 7c20 666c 6f61 745d  tr, str | float]
+000152b0: 2920 2d3e 2064 6963 745b 7374 722c 2066  ) -> dict[str, f
+000152c0: 6c6f 6174 5d3a 2023 206e 6f71 610a 2020  loat]: # noqa.  
+000152d0: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
+000152e0: 2020 5365 7473 2067 7565 7373 2076 616c    Sets guess val
+000152f0: 7565 7320 666f 7220 7061 7261 6d65 7465  ues for paramete
+00015300: 7273 2069 6620 7265 7175 6573 7465 6420  rs if requested 
+00015310: 6279 2075 7365 720a 0a20 2020 2020 2020  by user..       
+00015320: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
+00015330: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+00015340: 2020 2020 2020 2070 6172 616d 5f64 6963         param_dic
+00015350: 743a 2064 6963 745b 7374 722c 2073 7472  t: dict[str, str
+00015360: 207c 2066 6c6f 6174 5d0a 2020 2020 2020   | float].      
+00015370: 2020 2020 2020 4b65 7973 2061 7265 2066        Keys are f
+00015380: 6974 2f66 6978 2070 6172 616d 6574 6572  it/fix parameter
+00015390: 206e 616d 6573 2028 7365 6520 636c 6173   names (see clas
+000153a0: 732e 5041 524e 414d 4553 295c 6e0a 2020  s.PARNAMES)\n.  
+000153b0: 2020 2020 2020 2020 2020 5661 6c75 6573            Values
+000153c0: 2061 7265 2065 6974 6865 7220 666c 6f61   are either floa
+000153d0: 7420 2861 6374 7561 6c20 7661 6c75 6529  t (actual value)
+000153e0: 206f 7220 7468 6520 7374 7269 6e67 2027   or the string '
+000153f0: 6775 6573 7327 0a0a 2020 2020 2020 2020  guess'..        
+00015400: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
+00015410: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+00015420: 6469 6374 5b73 7472 2c20 666c 6f61 745d  dict[str, float]
+00015430: 0a20 2020 2020 2020 2020 2020 204b 6579  .            Key
+00015440: 7320 6172 6520 6669 742f 6669 7820 7061  s are fit/fix pa
+00015450: 7261 6d65 7465 7220 6e61 6d65 7320 2873  rameter names (s
+00015460: 6565 2063 6c61 7373 2e50 4152 4e41 4d45  ee class.PARNAME
+00015470: 5329 5c6e 0a20 2020 2020 2020 2020 2020  S)\n.           
+00015480: 2056 616c 7565 7320 6172 6520 666c 6f61   Values are floa
+00015490: 7420 2861 6374 7561 6c20 7661 6c75 6529  t (actual value)
+000154a0: 2077 6869 6368 2061 7265 2069 6e69 7469   which are initi
+000154b0: 616c 2076 616c 7565 7320 6f66 0a20 2020  al values of.   
+000154c0: 2020 2020 2020 2020 2070 6172 616d 6574           paramet
+000154d0: 6572 0a20 2020 2020 2020 2027 2727 0a0a  er.        '''..
+000154e0: 2020 2020 2020 2020 2320 4d61 6b65 2063          # Make c
+000154f0: 6f70 792c 2061 6e79 2073 7472 2076 616c  opy, any str val
+00015500: 7565 7320 7769 6c6c 2062 6520 7265 706c  ues will be repl
+00015510: 6163 6564 0a20 2020 2020 2020 206e 6577  aced.        new
+00015520: 5f70 6172 616d 5f64 6963 7420 3d20 636f  _param_dict = co
+00015530: 7079 2e63 6f70 7928 7061 7261 6d5f 6469  py.copy(param_di
+00015540: 6374 290a 0a20 2020 2020 2020 2023 2047  ct)..        # G
+00015550: 7565 7373 6573 0a20 2020 2020 2020 2067  uesses.        g
+00015560: 7565 7373 6469 6374 203d 207b 0a20 2020  uessdict = {.   
+00015570: 2020 2020 2020 2020 2027 755f 6566 6627           'u_eff'
+00015580: 3a20 3135 3030 2e2c 0a20 2020 2020 2020  : 1500.,.       
+00015590: 2020 2020 2027 4127 3a20 2d31 310a 2020       'A': -11.  
+000155a0: 2020 2020 2020 7d0a 0a20 2020 2020 2020        }..       
+000155b0: 2023 2052 6570 6c61 6365 2027 6775 6573   # Replace 'gues
+000155c0: 7327 2077 6974 6820 7265 6c65 7661 6e74  s' with relevant
+000155d0: 2067 7565 7373 0a20 2020 2020 2020 2066   guess.        f
+000155e0: 6f72 2076 6172 2c20 7661 6c20 696e 2070  or var, val in p
+000155f0: 6172 616d 5f64 6963 742e 6974 656d 7328  aram_dict.items(
+00015600: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
+00015610: 6620 7661 6c20 3d3d 2027 6775 6573 7327  f val == 'guess'
+00015620: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00015630: 2020 6e65 775f 7061 7261 6d5f 6469 6374    new_param_dict
+00015640: 5b76 6172 5d20 3d20 6775 6573 7364 6963  [var] = guessdic
+00015650: 745b 7661 725d 0a0a 2020 2020 2020 2020  t[var]..        
+00015660: 7265 7475 726e 206e 6577 5f70 6172 616d  return new_param
+00015670: 5f64 6963 740a 0a20 2020 2040 7374 6174  _dict..    @stat
+00015680: 6963 6d65 7468 6f64 0a20 2020 2064 6566  icmethod.    def
+00015690: 206d 6f64 656c 2870 6172 616d 6574 6572   model(parameter
+000156a0: 733a 2064 6963 745b 7374 722c 2066 6c6f  s: dict[str, flo
+000156b0: 6174 5d2c 0a20 2020 2020 2020 2020 2020  at],.           
+000156c0: 2020 2074 656d 7065 7261 7475 7265 733a     temperatures:
+000156d0: 206e 7074 2e41 7272 6179 4c69 6b65 2920   npt.ArrayLike) 
+000156e0: 2d3e 206e 7074 2e4e 4441 7272 6179 3a0a  -> npt.NDArray:.
+000156f0: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
+00015700: 2020 2020 4576 616c 7561 7465 7320 6c6f      Evaluates lo
+00015710: 6731 3028 4f72 6261 6368 2920 6d6f 6465  g10(Orbach) mode
+00015720: 6c20 6f66 206c 6f67 3130 2872 656c 6178  l of log10(relax
+00015730: 6174 696f 6e20 7261 7465 290a 2020 2020  ation rate).    
+00015740: 2020 2020 7573 696e 6720 7072 6f76 6964      using provid
+00015750: 6564 2070 6172 616d 6574 6572 2061 6e64  ed parameter and
+00015760: 2074 656d 7065 7261 7475 7265 2076 616c   temperature val
+00015770: 7565 732e 0a0a 2020 2020 2020 2020 5061  ues...        Pa
+00015780: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
+00015790: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+000157a0: 2020 2020 7061 7261 6d65 7465 7273 3a20      parameters: 
+000157b0: 6469 6374 5b73 7472 2c20 666c 6f61 745d  dict[str, float]
+000157c0: 0a20 2020 2020 2020 2020 2020 2050 6172  .            Par
+000157d0: 616d 6574 6572 7320 746f 2075 7365 2069  ameters to use i
+000157e0: 6e20 6d6f 6465 6c20 6675 6e63 7469 6f6e  n model function
+000157f0: 2c20 6b65 7973 2061 7265 2067 6976 656e  , keys are given
+00015800: 2069 6e0a 2020 2020 2020 2020 2020 2020   in.            
+00015810: 636c 6173 732e 5041 524e 414d 4553 0a20  class.PARNAMES. 
+00015820: 2020 2020 2020 2074 656d 7065 7261 7475         temperatu
+00015830: 7265 733a 2061 7272 6179 5f6c 696b 650a  res: array_like.
+00015840: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
+00015850: 6572 6174 7572 6520 7661 6c75 6573 2028  erature values (
+00015860: 4b29 2061 7420 7768 6963 6820 6d6f 6465  K) at which mode
+00015870: 6c20 6675 6e63 7469 6f6e 2069 7320 6576  l function is ev
+00015880: 616c 7561 7465 640a 0a20 2020 2020 2020  aluated..       
+00015890: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
+000158a0: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
+000158b0: 206e 6461 7272 6179 206f 6620 666c 6f61   ndarray of floa
+000158c0: 7473 0a20 2020 2020 2020 2020 2020 206c  ts.            l
+000158d0: 6f67 3130 2852 656c 6178 6174 696f 6e20  og10(Relaxation 
+000158e0: 7261 7465 2920 6173 2061 2066 756e 6374  rate) as a funct
+000158f0: 696f 6e20 6f66 2074 656d 7065 7261 7475  ion of temperatu
+00015900: 7265 0a0a 2020 2020 2020 2020 2727 270a  re..        '''.
+00015910: 0a20 2020 2020 2020 2075 5f65 6666 203d  .        u_eff =
+00015920: 2070 6172 616d 6574 6572 735b 2775 5f65   parameters['u_e
+00015930: 6666 275d 0a20 2020 2020 2020 2061 203d  ff'].        a =
+00015940: 2070 6172 616d 6574 6572 735b 2741 275d   parameters['A']
+00015950: 0a0a 2020 2020 2020 2020 6c6f 6772 6174  ..        lograt
+00015960: 6520 3d20 6e70 2e6c 6f67 3130 2831 302a  e = np.log10(10*
+00015970: 2a2d 6120 2a20 6e70 2e65 7870 282d 755f  *-a * np.exp(-u_
+00015980: 6566 6620 2f20 6e70 2e61 7361 7272 6179  eff / np.asarray
+00015990: 2874 656d 7065 7261 7475 7265 7329 2929  (temperatures)))
+000159a0: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+000159b0: 206c 6f67 7261 7465 0a0a 0a63 6c61 7373   lograte...class
+000159c0: 204c 6f67 5261 6d61 6e4d 6f64 656c 284c   LogRamanModel(L
+000159d0: 6f67 5461 7554 4d6f 6465 6c29 3a0a 2020  ogTauTModel):.  
+000159e0: 2020 2727 270a 2020 2020 4c6f 6728 5261    '''.    Log(Ra
+000159f0: 6d61 6e29 204d 6f64 656c 206f 6620 6c6f  man) Model of lo
+00015a00: 6731 3028 5265 6c61 7861 7469 6f6e 2072  g10(Relaxation r
+00015a10: 6174 6529 2076 7320 7465 6d70 6572 6174  ate) vs temperat
+00015a20: 7572 650a 2020 2020 2727 270a 0a20 2020  ure.    '''..   
+00015a30: 2023 3a20 4d6f 6465 6c20 6e61 6d65 0a20   #: Model name. 
+00015a40: 2020 204e 414d 4520 3d20 2752 616d 616e     NAME = 'Raman
+00015a50: 270a 2020 2020 233a 204d 6f64 656c 206e  '.    #: Model n
+00015a60: 616d 6520 7769 7468 206c 6f67 2062 7261  ame with log bra
+00015a70: 636b 6574 730a 2020 2020 4c4e 414d 4520  ckets.    LNAME 
+00015a80: 3d20 274c 6f67 2852 616d 616e 2927 0a0a  = 'Log(Raman)'..
+00015a90: 2020 2020 233a 204d 6f64 656c 2050 6172      #: Model Par
+00015aa0: 616d 6574 6572 206e 616d 6520 7374 7269  ameter name stri
+00015ab0: 6e67 730a 2020 2020 5041 524e 414d 4553  ngs.    PARNAMES
+00015ac0: 203d 205b 0a20 2020 2020 2020 2027 5227   = [.        'R'
+00015ad0: 2c20 276e 272c 0a20 2020 205d 0a0a 2020  , 'n',.    ]..  
+00015ae0: 2020 233a 204d 6f64 656c 2050 6172 616d    #: Model Param
+00015af0: 6574 6572 206e 616d 6520 6d61 7468 6d6f  eter name mathmo
+00015b00: 6465 2073 7472 696e 6773 0a20 2020 2056  de strings.    V
+00015b10: 4152 4e41 4d45 535f 4d4d 203d 207b 0a20  ARNAMES_MM = {. 
+00015b20: 2020 2020 2020 2027 5227 3a20 7227 2452         'R': r'$R
+00015b30: 2427 2c0a 2020 2020 2020 2020 276e 273a  $',.        'n':
+00015b40: 2072 2724 6e24 270a 2020 2020 7d0a 0a20   r'$n$'.    }.. 
+00015b50: 2020 2023 3a20 4d6f 6465 6c20 5061 7261     #: Model Para
+00015b60: 6d65 7465 7220 6e61 6d65 2048 544d 4c20  meter name HTML 
+00015b70: 7374 7269 6e67 730a 2020 2020 5641 524e  strings.    VARN
+00015b80: 414d 4553 5f48 544d 4c20 3d20 7b0a 2020  AMES_HTML = {.  
+00015b90: 2020 2020 2020 2752 273a 2027 5227 2c0a        'R': 'R',.
+00015ba0: 2020 2020 2020 2020 276e 273a 2027 6e27          'n': 'n'
+00015bb0: 0a20 2020 207d 0a0a 2020 2020 233a 204d  .    }..    #: M
+00015bc0: 6f64 656c 2050 6172 616d 6574 6572 2075  odel Parameter u
+00015bd0: 6e69 7420 7374 7269 6e67 730a 2020 2020  nit strings.    
+00015be0: 554e 4954 5320 3d20 7b0a 2020 2020 2020  UNITS = {.      
+00015bf0: 2020 2752 273a 2027 6c6f 6731 305b 735e    'R': 'log10[s^
+00015c00: 2d31 204b 5e2d 6e5d 272c 0a20 2020 2020  -1 K^-n]',.     
+00015c10: 2020 2027 6e27 3a20 2727 0a20 2020 207d     'n': ''.    }
+00015c20: 0a0a 2020 2020 233a 204d 6f64 656c 2050  ..    #: Model P
+00015c30: 6172 616d 6574 6572 2075 6e69 7420 6d61  arameter unit ma
+00015c40: 7468 6d6f 6465 2073 7472 696e 6773 0a20  thmode strings. 
+00015c50: 2020 2055 4e49 5453 5f4d 4d20 3d20 7b0a     UNITS_MM = {.
+00015c60: 2020 2020 2020 2020 2752 273a 2072 2724          'R': r'$
+00015c70: 5c6c 6f67 5f5c 6d61 7468 7265 6775 6c61  \log_\mathregula
+00015c80: 727b 3130 7d5c 6c65 6674 5b5c 6d61 7468  r{10}\left[\math
+00015c90: 7265 6775 6c61 727b 737d 5e5c 6d61 7468  regular{s}^\math
+00015ca0: 7265 6775 6c61 727b 2d31 7d20 5c6d 6174  regular{-1} \mat
+00015cb0: 6872 6567 756c 6172 7b4b 7d5e 5c6d 6174  hregular{K}^\mat
+00015cc0: 6872 6567 756c 6172 7b2d 6e7d 5c72 6967  hregular{-n}\rig
+00015cd0: 6874 5d24 272c 2023 206e 6f71 610a 2020  ht]$', # noqa.  
+00015ce0: 2020 2020 2020 276e 273a 2027 270a 2020        'n': ''.  
+00015cf0: 2020 7d0a 0a20 2020 2023 3a20 4d6f 6465    }..    #: Mode
+00015d00: 6c20 5061 7261 6d65 7465 7220 756e 6974  l Parameter unit
+00015d10: 2048 544d 4c20 7374 7269 6e67 730a 2020   HTML strings.  
+00015d20: 2020 554e 4954 535f 4854 4d4c 203d 207b    UNITS_HTML = {
+00015d30: 0a20 2020 2020 2020 2027 5227 3a20 276c  .        'R': 'l
+00015d40: 6f67 3c73 7562 3e31 303c 2f73 7562 3e5b  og<sub>10</sub>[
+00015d50: 733c 7375 703e 2d31 3c2f 7375 703e 204b  s<sup>-1</sup> K
+00015d60: 3c73 7570 3e2d 6e3c 2f73 7570 3e5d 272c  <sup>-n</sup>]',
+00015d70: 0a20 2020 2020 2020 2027 6e27 3a20 2727  .        'n': ''
+00015d80: 0a20 2020 207d 0a0a 2020 2020 233a 204d  .    }..    #: M
+00015d90: 6f64 656c 2070 6172 616d 6574 6572 2062  odel parameter b
+00015da0: 6f75 6e64 730a 2020 2020 424f 554e 4453  ounds.    BOUNDS
+00015db0: 203d 207b 0a20 2020 2020 2020 2027 5227   = {.        'R'
+00015dc0: 3a20 5b2d 3330 2c20 6e70 2e69 6e66 5d2c  : [-30, np.inf],
+00015dd0: 0a20 2020 2020 2020 2027 6e27 3a20 5b30  .        'n': [0
+00015de0: 2c20 6e70 2e69 6e66 5d0a 2020 2020 7d0a  , np.inf].    }.
+00015df0: 0a20 2020 2040 7374 6174 6963 6d65 7468  .    @staticmeth
+00015e00: 6f64 0a20 2020 2064 6566 2073 6574 5f69  od.    def set_i
+00015e10: 6e69 7469 616c 5f76 616c 7328 7061 7261  nitial_vals(para
+00015e20: 6d5f 6469 6374 3a20 6469 6374 5b73 7472  m_dict: dict[str
+00015e30: 2c20 7374 7220 7c20 666c 6f61 745d 2920  , str | float]) 
+00015e40: 2d3e 2064 6963 745b 7374 722c 2066 6c6f  -> dict[str, flo
+00015e50: 6174 5d3a 2023 206e 6f71 610a 2020 2020  at]: # noqa.    
+00015e60: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
+00015e70: 5365 7473 2067 7565 7373 2076 616c 7565  Sets guess value
+00015e80: 7320 666f 7220 7061 7261 6d65 7465 7273  s for parameters
+00015e90: 2069 6620 7265 7175 6573 7465 6420 6279   if requested by
+00015ea0: 2075 7365 720a 0a20 2020 2020 2020 2050   user..        P
+00015eb0: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
+00015ec0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+00015ed0: 2020 2020 2070 6172 616d 5f64 6963 743a       param_dict:
+00015ee0: 2064 6963 745b 7374 722c 2073 7472 207c   dict[str, str |
+00015ef0: 2066 6c6f 6174 5d0a 2020 2020 2020 2020   float].        
+00015f00: 2020 2020 4b65 7973 2061 7265 2066 6974      Keys are fit
+00015f10: 2f66 6978 2070 6172 616d 6574 6572 206e  /fix parameter n
+00015f20: 616d 6573 2028 7365 6520 636c 6173 732e  ames (see class.
+00015f30: 5041 524e 414d 4553 295c 6e0a 2020 2020  PARNAMES)\n.    
+00015f40: 2020 2020 2020 2020 5661 6c75 6573 2061          Values a
+00015f50: 7265 2065 6974 6865 7220 666c 6f61 7420  re either float 
+00015f60: 2861 6374 7561 6c20 7661 6c75 6529 206f  (actual value) o
+00015f70: 7220 7468 6520 7374 7269 6e67 2027 6775  r the string 'gu
+00015f80: 6573 7327 0a0a 2020 2020 2020 2020 5265  ess'..        Re
+00015f90: 7475 726e 730a 2020 2020 2020 2020 2d2d  turns.        --
+00015fa0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 6469  -----.        di
+00015fb0: 6374 5b73 7472 2c20 666c 6f61 745d 0a20  ct[str, float]. 
+00015fc0: 2020 2020 2020 2020 2020 204b 6579 7320             Keys 
+00015fd0: 6172 6520 6669 742f 6669 7820 7061 7261  are fit/fix para
+00015fe0: 6d65 7465 7220 6e61 6d65 7320 2873 6565  meter names (see
+00015ff0: 2063 6c61 7373 2e50 4152 4e41 4d45 5329   class.PARNAMES)
+00016000: 5c6e 0a20 2020 2020 2020 2020 2020 2056  \n.            V
+00016010: 616c 7565 7320 6172 6520 666c 6f61 7420  alues are float 
+00016020: 2861 6374 7561 6c20 7661 6c75 6529 2077  (actual value) w
+00016030: 6869 6368 2061 7265 2069 6e69 7469 616c  hich are initial
+00016040: 2076 616c 7565 7320 6f66 0a20 2020 2020   values of.     
+00016050: 2020 2020 2020 2070 6172 616d 6574 6572         parameter
+00016060: 0a20 2020 2020 2020 2027 2727 0a0a 2020  .        '''..  
+00016070: 2020 2020 2020 2320 4d61 6b65 2063 6f70        # Make cop
+00016080: 792c 2061 6e79 2073 7472 2076 616c 7565  y, any str value
+00016090: 7320 7769 6c6c 2062 6520 7265 706c 6163  s will be replac
+000160a0: 6564 0a20 2020 2020 2020 206e 6577 5f70  ed.        new_p
+000160b0: 6172 616d 5f64 6963 7420 3d20 636f 7079  aram_dict = copy
+000160c0: 2e63 6f70 7928 7061 7261 6d5f 6469 6374  .copy(param_dict
+000160d0: 290a 0a20 2020 2020 2020 2023 2047 7565  )..        # Gue
+000160e0: 7373 6573 0a20 2020 2020 2020 2067 7565  sses.        gue
+000160f0: 7373 6469 6374 203d 207b 0a20 2020 2020  ssdict = {.     
+00016100: 2020 2020 2020 2027 5227 3a20 2d36 2c0a         'R': -6,.
+00016110: 2020 2020 2020 2020 2020 2020 276e 273a              'n':
+00016120: 2033 0a20 2020 2020 2020 207d 0a0a 2020   3.        }..  
+00016130: 2020 2020 2020 2320 5265 706c 6163 6520        # Replace 
+00016140: 2767 7565 7373 2720 7769 7468 2072 656c  'guess' with rel
+00016150: 6576 616e 7420 6775 6573 730a 2020 2020  evant guess.    
+00016160: 2020 2020 666f 7220 7661 722c 2076 616c      for var, val
+00016170: 2069 6e20 7061 7261 6d5f 6469 6374 2e69   in param_dict.i
+00016180: 7465 6d73 2829 3a0a 2020 2020 2020 2020  tems():.        
+00016190: 2020 2020 6966 2076 616c 203d 3d20 2767      if val == 'g
+000161a0: 7565 7373 273a 0a20 2020 2020 2020 2020  uess':.         
+000161b0: 2020 2020 2020 206e 6577 5f70 6172 616d         new_param
+000161c0: 5f64 6963 745b 7661 725d 203d 2067 7565  _dict[var] = gue
+000161d0: 7373 6469 6374 5b76 6172 5d0a 0a20 2020  ssdict[var]..   
+000161e0: 2020 2020 2072 6574 7572 6e20 6e65 775f       return new_
+000161f0: 7061 7261 6d5f 6469 6374 0a0a 2020 2020  param_dict..    
+00016200: 4073 7461 7469 636d 6574 686f 640a 2020  @staticmethod.  
+00016210: 2020 6465 6620 6d6f 6465 6c28 7061 7261    def model(para
+00016220: 6d65 7465 7273 3a20 6469 6374 5b73 7472  meters: dict[str
+00016230: 2c20 666c 6f61 745d 2c0a 2020 2020 2020  , float],.      
+00016240: 2020 2020 2020 2020 7465 6d70 6572 6174          temperat
+00016250: 7572 6573 3a20 6e70 742e 4172 7261 794c  ures: npt.ArrayL
+00016260: 696b 6529 202d 3e20 6e70 742e 4e44 4172  ike) -> npt.NDAr
+00016270: 7261 793a 0a20 2020 2020 2020 2027 2727  ray:.        '''
+00016280: 0a20 2020 2020 2020 2045 7661 6c75 6174  .        Evaluat
+00016290: 6573 206c 6f67 3130 2852 616d 616e 2920  es log10(Raman) 
+000162a0: 6d6f 6465 6c20 6f66 206c 6f67 3130 2872  model of log10(r
+000162b0: 656c 6178 6174 696f 6e20 7261 7465 290a  elaxation rate).
+000162c0: 2020 2020 2020 2020 7573 696e 6720 7072          using pr
+000162d0: 6f76 6964 6564 2070 6172 616d 6574 6572  ovided parameter
+000162e0: 2061 6e64 2074 656d 7065 7261 7475 7265   and temperature
+000162f0: 2076 616c 7565 732e 0a0a 2020 2020 2020   values...      
+00016300: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+00016310: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a       ----------.
+00016320: 2020 2020 2020 2020 7061 7261 6d65 7465          paramete
+00016330: 7273 3a20 6469 6374 5b73 7472 2c20 666c  rs: dict[str, fl
+00016340: 6f61 745d 0a20 2020 2020 2020 2020 2020  oat].           
+00016350: 2050 6172 616d 6574 6572 7320 746f 2075   Parameters to u
+00016360: 7365 2069 6e20 6d6f 6465 6c20 6675 6e63  se in model func
+00016370: 7469 6f6e 2c20 6b65 7973 2061 7265 2067  tion, keys are g
+00016380: 6976 656e 2069 6e0a 2020 2020 2020 2020  iven in.        
+00016390: 2020 2020 636c 6173 732e 5041 524e 414d      class.PARNAM
+000163a0: 4553 0a20 2020 2020 2020 2074 656d 7065  ES.        tempe
+000163b0: 7261 7475 7265 733a 2061 7272 6179 5f6c  ratures: array_l
+000163c0: 696b 650a 2020 2020 2020 2020 2020 2020  ike.            
+000163d0: 7465 6d70 6572 6174 7572 6520 7661 6c75  temperature valu
+000163e0: 6573 2028 4b29 2061 7420 7768 6963 6820  es (K) at which 
+000163f0: 6d6f 6465 6c20 6675 6e63 7469 6f6e 2069  model function i
+00016400: 7320 6576 616c 7561 7465 640a 0a20 2020  s evaluated..   
+00016410: 2020 2020 2052 6574 7572 6e73 0a20 2020       Returns.   
+00016420: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
+00016430: 2020 2020 206e 6461 7272 6179 206f 6620       ndarray of 
+00016440: 666c 6f61 7473 0a20 2020 2020 2020 2020  floats.         
+00016450: 2020 206c 6f67 3130 2852 656c 6178 6174     log10(Relaxat
+00016460: 696f 6e20 7261 7465 2920 6173 2061 2066  ion rate) as a f
+00016470: 756e 6374 696f 6e20 6f66 2074 656d 7065  unction of tempe
+00016480: 7261 7475 7265 0a0a 2020 2020 2020 2020  rature..        
+00016490: 2727 270a 0a20 2020 2020 2020 2072 203d  '''..        r =
+000164a0: 2070 6172 616d 6574 6572 735b 2752 275d   parameters['R']
+000164b0: 0a20 2020 2020 2020 206e 203d 2070 6172  .        n = par
+000164c0: 616d 6574 6572 735b 276e 275d 0a0a 2020  ameters['n']..  
+000164d0: 2020 2020 2020 6c6f 6772 6174 6520 3d20        lograte = 
+000164e0: 6e70 2e6c 6f67 3130 2831 302a 2a72 202a  np.log10(10**r *
+000164f0: 206e 702e 6173 6172 7261 7928 7465 6d70   np.asarray(temp
+00016500: 6572 6174 7572 6573 292a 2a6e 290a 0a20  eratures)**n).. 
+00016510: 2020 2020 2020 2072 6574 7572 6e20 6c6f         return lo
+00016520: 6772 6174 650a 0a0a 636c 6173 7320 4c6f  grate...class Lo
+00016530: 6751 544d 4d6f 6465 6c28 4c6f 6754 6175  gQTMModel(LogTau
+00016540: 544d 6f64 656c 293a 0a20 2020 2027 2727  TModel):.    '''
+00016550: 0a20 2020 204c 6f67 2851 544d 2920 4d6f  .    Log(QTM) Mo
+00016560: 6465 6c20 6f66 206c 6f67 3130 2852 656c  del of log10(Rel
+00016570: 6178 6174 696f 6e20 7261 7465 2920 7673  axation rate) vs
+00016580: 2074 656d 7065 7261 7475 7265 0a20 2020   temperature.   
+00016590: 2027 2727 0a20 2020 2023 3a20 4d6f 6465   '''.    #: Mode
+000165a0: 6c20 6e61 6d65 0a20 2020 204e 414d 4520  l name.    NAME 
+000165b0: 3d20 2751 544d 270a 2020 2020 233a 204d  = 'QTM'.    #: M
+000165c0: 6f64 656c 206e 616d 6520 7769 7468 206c  odel name with l
+000165d0: 6f67 2062 7261 636b 6574 730a 2020 2020  og brackets.    
+000165e0: 4c4e 414d 4520 3d20 274c 6f67 2851 544d  LNAME = 'Log(QTM
+000165f0: 2927 0a0a 2020 2020 233a 204d 6f64 656c  )'..    #: Model
+00016600: 2050 6172 616d 6574 6572 206e 616d 6520   Parameter name 
+00016610: 7374 7269 6e67 730a 2020 2020 5041 524e  strings.    PARN
+00016620: 414d 4553 203d 205b 0a20 2020 2020 2020  AMES = [.       
+00016630: 2027 5127 0a20 2020 205d 0a0a 2020 2020   'Q'.    ]..    
+00016640: 233a 204d 6f64 656c 2050 6172 616d 6574  #: Model Paramet
+00016650: 6572 206e 616d 6520 6d61 7468 6d6f 6465  er name mathmode
+00016660: 2073 7472 696e 6773 0a20 2020 2056 4152   strings.    VAR
+00016670: 4e41 4d45 535f 4d4d 203d 207b 0a20 2020  NAMES_MM = {.   
+00016680: 2020 2020 2027 5127 3a20 7227 2451 2427       'Q': r'$Q$'
+00016690: 2c0a 2020 2020 7d0a 0a20 2020 2023 3a20  ,.    }..    #: 
+000166a0: 4d6f 6465 6c20 5061 7261 6d65 7465 7220  Model Parameter 
+000166b0: 6e61 6d65 2048 544d 4c20 7374 7269 6e67  name HTML string
+000166c0: 730a 2020 2020 5641 524e 414d 4553 5f48  s.    VARNAMES_H
+000166d0: 544d 4c20 3d20 7b0a 2020 2020 2020 2020  TML = {.        
+000166e0: 2751 273a 2027 5127 2c0a 2020 2020 7d0a  'Q': 'Q',.    }.
+000166f0: 0a20 2020 2023 3a20 4d6f 6465 6c20 5061  .    #: Model Pa
+00016700: 7261 6d65 7465 7220 756e 6974 2073 7472  rameter unit str
+00016710: 696e 6773 0a20 2020 2055 4e49 5453 203d  ings.    UNITS =
+00016720: 207b 0a20 2020 2020 2020 2027 5127 3a20   {.        'Q': 
+00016730: 276c 6f67 3130 5b73 5d27 2c0a 2020 2020  'log10[s]',.    
+00016740: 7d0a 0a20 2020 2023 3a20 4d6f 6465 6c20  }..    #: Model 
+00016750: 5061 7261 6d65 7465 7220 756e 6974 206d  Parameter unit m
+00016760: 6174 686d 6f64 6520 7374 7269 6e67 730a  athmode strings.
+00016770: 2020 2020 554e 4954 535f 4d4d 203d 207b      UNITS_MM = {
+00016780: 0a20 2020 2020 2020 2027 5127 3a20 7227  .        'Q': r'
+00016790: 245c 6c6f 675f 5c6d 6174 6872 6567 756c  $\log_\mathregul
+000167a0: 6172 7b31 307d 5c6c 6566 745b 5c6d 6174  ar{10}\left[\mat
+000167b0: 6872 6567 756c 6172 7b73 7d5c 7269 6768  hregular{s}\righ
+000167c0: 745d 2427 2c0a 2020 2020 7d0a 0a20 2020  t]$',.    }..   
+000167d0: 2023 3a20 4d6f 6465 6c20 5061 7261 6d65   #: Model Parame
+000167e0: 7465 7220 756e 6974 2048 544d 4c20 7374  ter unit HTML st
+000167f0: 7269 6e67 730a 2020 2020 554e 4954 535f  rings.    UNITS_
+00016800: 4854 4d4c 203d 207b 0a20 2020 2020 2020  HTML = {.       
+00016810: 2027 5127 3a20 7227 6c6f 673c 7375 623e   'Q': r'log<sub>
+00016820: 3130 3c2f 7375 623e 5b73 5d27 0a20 2020  10</sub>[s]'.   
+00016830: 207d 0a0a 2020 2020 233a 204d 6f64 656c   }..    #: Model
+00016840: 2070 6172 616d 6574 6572 2062 6f75 6e64   parameter bound
+00016850: 730a 2020 2020 424f 554e 4453 203d 207b  s.    BOUNDS = {
+00016860: 0a20 2020 2020 2020 2027 5127 3a20 5b2d  .        'Q': [-
+00016870: 3330 2c20 3330 2e5d 0a20 2020 207d 0a0a  30, 30.].    }..
+00016880: 2020 2020 4073 7461 7469 636d 6574 686f      @staticmetho
+00016890: 640a 2020 2020 6465 6620 7365 745f 696e  d.    def set_in
+000168a0: 6974 6961 6c5f 7661 6c73 2870 6172 616d  itial_vals(param
+000168b0: 5f64 6963 743a 2064 6963 745b 7374 722c  _dict: dict[str,
+000168c0: 2073 7472 207c 2066 6c6f 6174 5d29 202d   str | float]) -
+000168d0: 3e20 6469 6374 5b73 7472 2c20 666c 6f61  > dict[str, floa
+000168e0: 745d 3a20 2320 6e6f 7161 0a20 2020 2020  t]: # noqa.     
+000168f0: 2020 2027 2727 0a20 2020 2020 2020 2053     '''.        S
+00016900: 6574 7320 6775 6573 7320 7661 6c75 6573  ets guess values
+00016910: 2066 6f72 2070 6172 616d 6574 6572 7320   for parameters 
+00016920: 6966 2072 6571 7565 7374 6564 2062 7920  if requested by 
+00016930: 7573 6572 0a0a 2020 2020 2020 2020 5061  user..        Pa
+00016940: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
+00016950: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+00016960: 2020 2020 7061 7261 6d5f 6469 6374 3a20      param_dict: 
+00016970: 6469 6374 5b73 7472 2c20 7374 7220 7c20  dict[str, str | 
+00016980: 666c 6f61 745d 0a20 2020 2020 2020 2020  float].         
+00016990: 2020 204b 6579 7320 6172 6520 6669 742f     Keys are fit/
+000169a0: 6669 7820 7061 7261 6d65 7465 7220 6e61  fix parameter na
+000169b0: 6d65 7320 2873 6565 2063 6c61 7373 2e50  mes (see class.P
+000169c0: 4152 4e41 4d45 5329 5c6e 0a20 2020 2020  ARNAMES)\n.     
+000169d0: 2020 2020 2020 2056 616c 7565 7320 6172         Values ar
+000169e0: 6520 6569 7468 6572 2066 6c6f 6174 2028  e either float (
+000169f0: 6163 7475 616c 2076 616c 7565 2920 6f72  actual value) or
+00016a00: 2074 6865 2073 7472 696e 6720 2767 7565   the string 'gue
+00016a10: 7373 270a 0a20 2020 2020 2020 2052 6574  ss'..        Ret
+00016a20: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
+00016a30: 2d2d 2d2d 0a20 2020 2020 2020 2064 6963  ----.        dic
+00016a40: 745b 7374 722c 2066 6c6f 6174 5d0a 2020  t[str, float].  
+00016a50: 2020 2020 2020 2020 2020 4b65 7973 2061            Keys a
+00016a60: 7265 2066 6974 2f66 6978 2070 6172 616d  re fit/fix param
+00016a70: 6574 6572 206e 616d 6573 2028 7365 6520  eter names (see 
+00016a80: 636c 6173 732e 5041 524e 414d 4553 295c  class.PARNAMES)\
+00016a90: 6e0a 2020 2020 2020 2020 2020 2020 5661  n.            Va
+00016aa0: 6c75 6573 2061 7265 2066 6c6f 6174 2028  lues are float (
+00016ab0: 6163 7475 616c 2076 616c 7565 2920 7768  actual value) wh
+00016ac0: 6963 6820 6172 6520 696e 6974 6961 6c20  ich are initial 
+00016ad0: 7661 6c75 6573 206f 660a 2020 2020 2020  values of.      
+00016ae0: 2020 2020 2020 7061 7261 6d65 7465 720a        parameter.
+00016af0: 2020 2020 2020 2020 2727 270a 0a20 2020          '''..   
+00016b00: 2020 2020 2023 204d 616b 6520 636f 7079       # Make copy
+00016b10: 2c20 616e 7920 7374 7220 7661 6c75 6573  , any str values
+00016b20: 2077 696c 6c20 6265 2072 6570 6c61 6365   will be replace
+00016b30: 640a 2020 2020 2020 2020 6e65 775f 7061  d.        new_pa
+00016b40: 7261 6d5f 6469 6374 203d 2063 6f70 792e  ram_dict = copy.
+00016b50: 636f 7079 2870 6172 616d 5f64 6963 7429  copy(param_dict)
+00016b60: 0a0a 2020 2020 2020 2020 2320 4775 6573  ..        # Gues
+00016b70: 7365 730a 2020 2020 2020 2020 6775 6573  ses.        gues
+00016b80: 7364 6963 7420 3d20 7b0a 2020 2020 2020  sdict = {.      
+00016b90: 2020 2020 2020 2751 273a 2031 0a20 2020        'Q': 1.   
+00016ba0: 2020 2020 207d 0a0a 2020 2020 2020 2020       }..        
+00016bb0: 2320 5265 706c 6163 6520 2767 7565 7373  # Replace 'guess
+00016bc0: 2720 7769 7468 2072 656c 6576 616e 7420  ' with relevant 
+00016bd0: 6775 6573 730a 2020 2020 2020 2020 666f  guess.        fo
+00016be0: 7220 7661 722c 2076 616c 2069 6e20 7061  r var, val in pa
+00016bf0: 7261 6d5f 6469 6374 2e69 7465 6d73 2829  ram_dict.items()
+00016c00: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+00016c10: 2076 616c 203d 3d20 2767 7565 7373 273a   val == 'guess':
+00016c20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016c30: 206e 6577 5f70 6172 616d 5f64 6963 745b   new_param_dict[
+00016c40: 7661 725d 203d 2067 7565 7373 6469 6374  var] = guessdict
+00016c50: 5b76 6172 5d0a 0a20 2020 2020 2020 2072  [var]..        r
+00016c60: 6574 7572 6e20 6e65 775f 7061 7261 6d5f  eturn new_param_
+00016c70: 6469 6374 0a0a 2020 2020 4073 7461 7469  dict..    @stati
+00016c80: 636d 6574 686f 640a 2020 2020 6465 6620  cmethod.    def 
+00016c90: 6d6f 6465 6c28 7061 7261 6d65 7465 7273  model(parameters
+00016ca0: 3a20 6469 6374 5b73 7472 2c20 666c 6f61  : dict[str, floa
+00016cb0: 745d 2c0a 2020 2020 2020 2020 2020 2020  t],.            
+00016cc0: 2020 7465 6d70 6572 6174 7572 6573 3a20    temperatures: 
+00016cd0: 6e70 742e 4172 7261 794c 696b 6529 202d  npt.ArrayLike) -
+00016ce0: 3e20 6e70 742e 4e44 4172 7261 793a 0a20  > npt.NDArray:. 
+00016cf0: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
+00016d00: 2020 2045 7661 6c75 6174 6573 206c 6f67     Evaluates log
+00016d10: 3130 2851 544d 2920 6d6f 6465 6c20 6f66  10(QTM) model of
+00016d20: 206c 6f67 3130 2872 656c 6178 6174 696f   log10(relaxatio
+00016d30: 6e20 7261 7465 290a 2020 2020 2020 2020  n rate).        
+00016d40: 7573 696e 6720 7072 6f76 6964 6564 2070  using provided p
+00016d50: 6172 616d 6574 6572 2061 6e64 2074 656d  arameter and tem
+00016d60: 7065 7261 7475 7265 2076 616c 7565 732e  perature values.
+00016d70: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
+00016d80: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
+00016d90: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+00016da0: 7061 7261 6d65 7465 7273 3a20 6469 6374  parameters: dict
+00016db0: 5b73 7472 2c20 666c 6f61 745d 0a20 2020  [str, float].   
+00016dc0: 2020 2020 2020 2020 2050 6172 616d 6574           Paramet
+00016dd0: 6572 7320 746f 2075 7365 2069 6e20 6d6f  ers to use in mo
+00016de0: 6465 6c20 6675 6e63 7469 6f6e 2c20 6b65  del function, ke
+00016df0: 7973 2061 7265 2067 6976 656e 2069 6e0a  ys are given in.
+00016e00: 2020 2020 2020 2020 2020 2020 636c 6173              clas
+00016e10: 732e 5041 524e 414d 4553 0a20 2020 2020  s.PARNAMES.     
+00016e20: 2020 2074 656d 7065 7261 7475 7265 733a     temperatures:
+00016e30: 2061 7272 6179 5f6c 696b 650a 2020 2020   array_like.    
+00016e40: 2020 2020 2020 2020 7465 6d70 6572 6174          temperat
+00016e50: 7572 6520 7661 6c75 6573 2028 4b29 2061  ure values (K) a
+00016e60: 7420 7768 6963 6820 6d6f 6465 6c20 6675  t which model fu
+00016e70: 6e63 7469 6f6e 2069 7320 6576 616c 7561  nction is evalua
+00016e80: 7465 640a 0a20 2020 2020 2020 2052 6574  ted..        Ret
+00016e90: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
+00016ea0: 2d2d 2d2d 0a20 2020 2020 2020 206e 6461  ----.        nda
+00016eb0: 7272 6179 206f 6620 666c 6f61 7473 0a20  rray of floats. 
+00016ec0: 2020 2020 2020 2020 2020 206c 6f67 3130             log10
+00016ed0: 2852 656c 6178 6174 696f 6e20 7261 7465  (Relaxation rate
+00016ee0: 2920 6173 2061 2066 756e 6374 696f 6e20  ) as a function 
+00016ef0: 6f66 2074 656d 7065 7261 7475 7265 0a0a  of temperature..
+00016f00: 2020 2020 2020 2020 2727 270a 0a20 2020          '''..   
+00016f10: 2020 2020 2071 203d 2070 6172 616d 6574       q = paramet
+00016f20: 6572 735b 2751 275d 0a0a 2020 2020 2020  ers['Q']..      
+00016f30: 2020 6c6f 6772 6174 6520 3d20 6e70 2e7a    lograte = np.z
+00016f40: 6572 6f73 286c 656e 2874 656d 7065 7261  eros(len(tempera
+00016f50: 7475 7265 7329 2920 2b20 6e70 2e6c 6f67  tures)) + np.log
+00016f60: 3130 2831 302a 2a2d 7129 0a0a 2020 2020  10(10**-q)..    
+00016f70: 2020 2020 7265 7475 726e 206c 6f67 7261      return logra
+00016f80: 7465 0a0a 0a63 6c61 7373 204c 6f67 4469  te...class LogDi
+00016f90: 7265 6374 4d6f 6465 6c28 4c6f 6754 6175  rectModel(LogTau
+00016fa0: 544d 6f64 656c 293a 0a20 2020 2027 2727  TModel):.    '''
+00016fb0: 0a20 2020 204c 6f67 2844 6972 6563 7429  .    Log(Direct)
+00016fc0: 204d 6f64 656c 206f 6620 6c6f 6731 3028   Model of log10(
+00016fd0: 5265 6c61 7861 7469 6f6e 2072 6174 6529  Relaxation rate)
+00016fe0: 2076 7320 7465 6d70 6572 6174 7572 650a   vs temperature.
+00016ff0: 2020 2020 2727 270a 2020 2020 233a 204d      '''.    #: M
+00017000: 6f64 656c 206e 616d 650a 2020 2020 4e41  odel name.    NA
+00017010: 4d45 203d 2027 4469 7265 6374 270a 0a20  ME = 'Direct'.. 
+00017020: 2020 2023 3a20 4d6f 6465 6c20 6e61 6d65     #: Model name
+00017030: 2077 6974 6820 6c6f 6720 6272 6163 6b65   with log bracke
+00017040: 7473 0a20 2020 204c 4e41 4d45 203d 2027  ts.    LNAME = '
+00017050: 4c6f 6728 4469 7265 6374 2927 0a0a 2020  Log(Direct)'..  
+00017060: 2020 233a 204d 6f64 656c 2050 6172 616d    #: Model Param
+00017070: 6574 6572 206e 616d 6520 7374 7269 6e67  eter name string
+00017080: 730a 2020 2020 5041 524e 414d 4553 203d  s.    PARNAMES =
+00017090: 205b 0a20 2020 2020 2020 2027 4427 0a20   [.        'D'. 
+000170a0: 2020 205d 0a0a 2020 2020 233a 204d 6f64     ]..    #: Mod
+000170b0: 656c 2050 6172 616d 6574 6572 206e 616d  el Parameter nam
+000170c0: 6520 6d61 7468 6d6f 6465 2073 7472 696e  e mathmode strin
+000170d0: 6773 0a20 2020 2056 4152 4e41 4d45 535f  gs.    VARNAMES_
+000170e0: 4d4d 203d 207b 0a20 2020 2020 2020 2027  MM = {.        '
+000170f0: 4427 3a20 7227 2444 2427 2c0a 2020 2020  D': r'$D$',.    
+00017100: 7d0a 0a20 2020 2023 3a20 4d6f 6465 6c20  }..    #: Model 
+00017110: 5061 7261 6d65 7465 7220 6e61 6d65 2048  Parameter name H
+00017120: 544d 4c20 7374 7269 6e67 730a 2020 2020  TML strings.    
+00017130: 5641 524e 414d 4553 5f48 544d 4c20 3d20  VARNAMES_HTML = 
+00017140: 7b0a 2020 2020 2020 2020 2744 273a 2027  {.        'D': '
+00017150: 4427 0a20 2020 207d 0a0a 2020 2020 233a  D'.    }..    #:
+00017160: 204d 6f64 656c 2050 6172 616d 6574 6572   Model Parameter
+00017170: 2075 6e69 7420 7374 7269 6e67 730a 2020   unit strings.  
+00017180: 2020 554e 4954 5320 3d20 7b0a 2020 2020    UNITS = {.    
+00017190: 2020 2020 2744 273a 2027 6c6f 6731 305b      'D': 'log10[
+000171a0: 732d 3120 4b2d 315d 272c 0a20 2020 207d  s-1 K-1]',.    }
+000171b0: 0a0a 2020 2020 233a 204d 6f64 656c 2050  ..    #: Model P
+000171c0: 6172 616d 6574 6572 2075 6e69 7420 6d61  arameter unit ma
+000171d0: 7468 6d6f 6465 2073 7472 696e 6773 0a20  thmode strings. 
+000171e0: 2020 2055 4e49 5453 5f4d 4d20 3d20 7b0a     UNITS_MM = {.
+000171f0: 2020 2020 2020 2020 2744 273a 2072 2724          'D': r'$
+00017200: 5c6c 6f67 5f5c 6d61 7468 7265 6775 6c61  \log_\mathregula
+00017210: 727b 3130 7d5c 6c65 6674 5b5c 6d61 7468  r{10}\left[\math
+00017220: 7265 6775 6c61 727b 737d 5e5c 6d61 7468  regular{s}^\math
+00017230: 7265 6775 6c61 727b 2d31 7d20 5c6d 6174  regular{-1} \mat
+00017240: 6872 6567 756c 6172 7b4b 7d5e 5c6d 6174  hregular{K}^\mat
+00017250: 6872 6567 756c 6172 7b2d 317d 5c72 6967  hregular{-1}\rig
+00017260: 6874 5d24 272c 2023 206e 6f71 610a 2020  ht]$', # noqa.  
+00017270: 2020 7d0a 0a20 2020 2023 3a20 4d6f 6465    }..    #: Mode
+00017280: 6c20 5061 7261 6d65 7465 7220 756e 6974  l Parameter unit
+00017290: 2048 544d 4c20 7374 7269 6e67 730a 2020   HTML strings.  
+000172a0: 2020 554e 4954 535f 4854 4d4c 203d 207b    UNITS_HTML = {
+000172b0: 0a20 2020 2020 2020 2027 4427 3a20 7227  .        'D': r'
+000172c0: 733c 7375 703e 2d31 3c2f 7375 703e 204b  s<sup>-1</sup> K
+000172d0: 3c73 7570 3e2d 313c 2f73 7570 3e27 0a20  <sup>-1</sup>'. 
+000172e0: 2020 207d 0a0a 2020 2020 233a 204d 6f64     }..    #: Mod
+000172f0: 656c 2070 6172 616d 6574 6572 2062 6f75  el parameter bou
+00017300: 6e64 730a 2020 2020 424f 554e 4453 203d  nds.    BOUNDS =
+00017310: 207b 0a20 2020 2020 2020 2027 4427 3a20   {.        'D': 
+00017320: 5b2d 3330 2c20 302e 5d0a 2020 2020 7d0a  [-30, 0.].    }.
+00017330: 0a20 2020 2040 7374 6174 6963 6d65 7468  .    @staticmeth
+00017340: 6f64 0a20 2020 2064 6566 2073 6574 5f69  od.    def set_i
+00017350: 6e69 7469 616c 5f76 616c 7328 7061 7261  nitial_vals(para
+00017360: 6d5f 6469 6374 3a20 6469 6374 5b73 7472  m_dict: dict[str
+00017370: 2c20 7374 7220 7c20 666c 6f61 745d 2920  , str | float]) 
+00017380: 2d3e 2064 6963 745b 7374 722c 2066 6c6f  -> dict[str, flo
+00017390: 6174 5d3a 2023 206e 6f71 610a 2020 2020  at]: # noqa.    
+000173a0: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
+000173b0: 5365 7473 2067 7565 7373 2076 616c 7565  Sets guess value
+000173c0: 7320 666f 7220 7061 7261 6d65 7465 7273  s for parameters
+000173d0: 2069 6620 7265 7175 6573 7465 6420 6279   if requested by
+000173e0: 2075 7365 720a 0a20 2020 2020 2020 2050   user..        P
+000173f0: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
+00017400: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+00017410: 2020 2020 2070 6172 616d 5f64 6963 743a       param_dict:
+00017420: 2064 6963 745b 7374 722c 2073 7472 207c   dict[str, str |
+00017430: 2066 6c6f 6174 5d0a 2020 2020 2020 2020   float].        
+00017440: 2020 2020 4b65 7973 2061 7265 2066 6974      Keys are fit
+00017450: 2f66 6978 2070 6172 616d 6574 6572 206e  /fix parameter n
+00017460: 616d 6573 2028 7365 6520 636c 6173 732e  ames (see class.
+00017470: 5041 524e 414d 4553 295c 6e0a 2020 2020  PARNAMES)\n.    
+00017480: 2020 2020 2020 2020 5661 6c75 6573 2061          Values a
+00017490: 7265 2065 6974 6865 7220 666c 6f61 7420  re either float 
+000174a0: 2861 6374 7561 6c20 7661 6c75 6529 206f  (actual value) o
+000174b0: 7220 7468 6520 7374 7269 6e67 2027 6775  r the string 'gu
+000174c0: 6573 7327 0a0a 2020 2020 2020 2020 5265  ess'..        Re
+000174d0: 7475 726e 730a 2020 2020 2020 2020 2d2d  turns.        --
+000174e0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 6469  -----.        di
+000174f0: 6374 5b73 7472 2c20 666c 6f61 745d 0a20  ct[str, float]. 
+00017500: 2020 2020 2020 2020 2020 204b 6579 7320             Keys 
+00017510: 6172 6520 6669 742f 6669 7820 7061 7261  are fit/fix para
+00017520: 6d65 7465 7220 6e61 6d65 7320 2873 6565  meter names (see
+00017530: 2063 6c61 7373 2e50 4152 4e41 4d45 5329   class.PARNAMES)
+00017540: 5c6e 0a20 2020 2020 2020 2020 2020 2056  \n.            V
+00017550: 616c 7565 7320 6172 6520 666c 6f61 7420  alues are float 
+00017560: 2861 6374 7561 6c20 7661 6c75 6529 2077  (actual value) w
+00017570: 6869 6368 2061 7265 2069 6e69 7469 616c  hich are initial
+00017580: 2076 616c 7565 7320 6f66 0a20 2020 2020   values of.     
+00017590: 2020 2020 2020 2070 6172 616d 6574 6572         parameter
+000175a0: 0a20 2020 2020 2020 2027 2727 0a0a 2020  .        '''..  
+000175b0: 2020 2020 2020 2320 4d61 6b65 2063 6f70        # Make cop
+000175c0: 792c 2061 6e79 2073 7472 2076 616c 7565  y, any str value
+000175d0: 7320 7769 6c6c 2062 6520 7265 706c 6163  s will be replac
+000175e0: 6564 0a20 2020 2020 2020 206e 6577 5f70  ed.        new_p
+000175f0: 6172 616d 5f64 6963 7420 3d20 636f 7079  aram_dict = copy
+00017600: 2e63 6f70 7928 7061 7261 6d5f 6469 6374  .copy(param_dict
+00017610: 290a 0a20 2020 2020 2020 2023 2047 7565  )..        # Gue
+00017620: 7373 6573 0a20 2020 2020 2020 2067 7565  sses.        gue
+00017630: 7373 6469 6374 203d 207b 0a20 2020 2020  ssdict = {.     
+00017640: 2020 2020 2020 2027 4427 3a20 2d32 0a20         'D': -2. 
+00017650: 2020 2020 2020 207d 0a0a 2020 2020 2020         }..      
+00017660: 2020 2320 5265 706c 6163 6520 2767 7565    # Replace 'gue
+00017670: 7373 2720 7769 7468 2072 656c 6576 616e  ss' with relevan
+00017680: 7420 6775 6573 730a 2020 2020 2020 2020  t guess.        
+00017690: 666f 7220 7661 722c 2076 616c 2069 6e20  for var, val in 
+000176a0: 7061 7261 6d5f 6469 6374 2e69 7465 6d73  param_dict.items
+000176b0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+000176c0: 6966 2076 616c 203d 3d20 2767 7565 7373  if val == 'guess
+000176d0: 273a 0a20 2020 2020 2020 2020 2020 2020  ':.             
+000176e0: 2020 206e 6577 5f70 6172 616d 5f64 6963     new_param_dic
+000176f0: 745b 7661 725d 203d 2067 7565 7373 6469  t[var] = guessdi
+00017700: 6374 5b76 6172 5d0a 0a20 2020 2020 2020  ct[var]..       
+00017710: 2072 6574 7572 6e20 6e65 775f 7061 7261   return new_para
+00017720: 6d5f 6469 6374 0a0a 2020 2020 4073 7461  m_dict..    @sta
+00017730: 7469 636d 6574 686f 640a 2020 2020 6465  ticmethod.    de
+00017740: 6620 6d6f 6465 6c28 7061 7261 6d65 7465  f model(paramete
+00017750: 7273 3a20 6469 6374 5b73 7472 2c20 666c  rs: dict[str, fl
+00017760: 6f61 745d 2c0a 2020 2020 2020 2020 2020  oat],.          
+00017770: 2020 2020 7465 6d70 6572 6174 7572 6573      temperatures
+00017780: 3a20 6e70 742e 4172 7261 794c 696b 6529  : npt.ArrayLike)
+00017790: 202d 3e20 6e70 742e 4e44 4172 7261 793a   -> npt.NDArray:
+000177a0: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
+000177b0: 2020 2020 2045 7661 6c75 6174 6573 206c       Evaluates l
+000177c0: 6f67 3130 2844 6972 6563 7429 206d 6f64  og10(Direct) mod
+000177d0: 656c 206f 6620 6c6f 6731 3028 7265 6c61  el of log10(rela
+000177e0: 7861 7469 6f6e 2072 6174 6529 0a20 2020  xation rate).   
+000177f0: 2020 2020 2075 7369 6e67 2070 726f 7669       using provi
+00017800: 6465 6420 7061 7261 6d65 7465 7220 616e  ded parameter an
+00017810: 6420 7465 6d70 6572 6174 7572 6520 7661  d temperature va
+00017820: 6c75 6573 2e0a 0a20 2020 2020 2020 2050  lues...        P
+00017830: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
+00017840: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+00017850: 2020 2020 2070 6172 616d 6574 6572 733a       parameters:
+00017860: 2064 6963 745b 7374 722c 2066 6c6f 6174   dict[str, float
+00017870: 5d0a 2020 2020 2020 2020 2020 2020 5061  ].            Pa
+00017880: 7261 6d65 7465 7273 2074 6f20 7573 6520  rameters to use 
+00017890: 696e 206d 6f64 656c 2066 756e 6374 696f  in model functio
+000178a0: 6e2c 206b 6579 7320 6172 6520 6769 7665  n, keys are give
+000178b0: 6e20 696e 0a20 2020 2020 2020 2020 2020  n in.           
+000178c0: 2063 6c61 7373 2e50 4152 4e41 4d45 530a   class.PARNAMES.
+000178d0: 2020 2020 2020 2020 7465 6d70 6572 6174          temperat
+000178e0: 7572 6573 3a20 6172 7261 795f 6c69 6b65  ures: array_like
+000178f0: 0a20 2020 2020 2020 2020 2020 2074 656d  .            tem
+00017900: 7065 7261 7475 7265 2076 616c 7565 7320  perature values 
+00017910: 284b 2920 6174 2077 6869 6368 206d 6f64  (K) at which mod
+00017920: 656c 2066 756e 6374 696f 6e20 6973 2065  el function is e
+00017930: 7661 6c75 6174 6564 0a0a 2020 2020 2020  valuated..      
+00017940: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
+00017950: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
+00017960: 2020 6e64 6172 7261 7920 6f66 2066 6c6f    ndarray of flo
+00017970: 6174 730a 2020 2020 2020 2020 2020 2020  ats.            
+00017980: 6c6f 6731 3028 5265 6c61 7861 7469 6f6e  log10(Relaxation
+00017990: 2072 6174 6529 2061 7320 6120 6675 6e63   rate) as a func
+000179a0: 7469 6f6e 206f 6620 7465 6d70 6572 6174  tion of temperat
+000179b0: 7572 650a 0a20 2020 2020 2020 2027 2727  ure..        '''
+000179c0: 0a0a 2020 2020 2020 2020 6420 3d20 7061  ..        d = pa
+000179d0: 7261 6d65 7465 7273 5b27 4427 5d0a 0a20  rameters['D'].. 
+000179e0: 2020 2020 2020 206c 6f67 7261 7465 203d         lograte =
+000179f0: 206e 702e 6c6f 6731 3028 3130 2a2a 6420   np.log10(10**d 
+00017a00: 2a20 6e70 2e61 7361 7272 6179 2874 656d  * np.asarray(tem
+00017a10: 7065 7261 7475 7265 7329 290a 0a20 2020  peratures))..   
+00017a20: 2020 2020 2072 6574 7572 6e20 6c6f 6772       return logr
+00017a30: 6174 650a 0a0a 636c 6173 7320 4d75 6c74  ate...class Mult
+00017a40: 694c 6f67 5461 7554 4d6f 6465 6c28 293a  iLogTauTModel():
+00017a50: 0a20 2020 2027 2727 0a20 2020 2054 616b  .    '''.    Tak
+00017a60: 6573 206d 756c 7469 706c 6520 4c6f 6754  es multiple LogT
+00017a70: 6175 544d 6f64 656c 206f 626a 6563 7473  auTModel objects
+00017a80: 2061 6e64 2063 6f6d 6269 6e65 7320 696e   and combines in
+00017a90: 746f 2061 2073 696e 676c 6520 6f62 6a65  to a single obje
+00017aa0: 6374 0a0a 2020 2020 5061 7261 6d65 7465  ct..    Paramete
+00017ab0: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
+00017ac0: 2d0a 2020 2020 6669 745f 7661 7273 3a20  -.    fit_vars: 
+00017ad0: 6c69 7374 5b64 6963 745b 7374 722c 2066  list[dict[str, f
+00017ae0: 6c6f 6174 207c 2073 7472 5d5d 0a20 2020  loat | str]].   
+00017af0: 2020 2020 204c 6973 7420 6f66 2066 6974       List of fit
+00017b00: 2064 6963 7473 2c20 7769 7468 206b 6579   dicts, with key
+00017b10: 7320 6173 2050 4152 4e41 4d45 5320 6f66  s as PARNAMES of
+00017b20: 2065 6163 6820 4c6f 6754 6175 544d 6f64   each LogTauTMod
+00017b30: 656c 0a20 2020 2020 2020 2061 6e64 2076  el.        and v
+00017b40: 616c 7565 7320 6173 2065 6974 6865 7220  alues as either 
+00017b50: 7468 6520 7374 7269 6e67 2027 6775 6573  the string 'gues
+00017b60: 7327 206f 7220 6120 666c 6f61 7420 7661  s' or a float va
+00017b70: 6c75 650a 2020 2020 6669 785f 7661 7273  lue.    fix_vars
+00017b80: 3a20 6c69 7374 5b64 6963 745b 7374 722c  : list[dict[str,
+00017b90: 2066 6c6f 6174 207c 2073 7472 5d5d 0a20   float | str]]. 
+00017ba0: 2020 2020 2020 204c 6973 7420 6f66 2066         List of f
+00017bb0: 6978 2064 6963 7473 2c20 7769 7468 206b  ix dicts, with k
+00017bc0: 6579 7320 6173 2050 4152 4e41 4d45 5320  eys as PARNAMES 
+00017bd0: 6f66 2065 6163 6820 4c6f 6754 6175 544d  of each LogTauTM
+00017be0: 6f64 656c 0a20 2020 2020 2020 2061 6e64  odel.        and
+00017bf0: 2076 616c 7565 7320 6173 2065 6974 6865   values as eithe
+00017c00: 7220 7468 6520 7374 7269 6e67 2027 6775  r the string 'gu
+00017c10: 6573 7327 206f 7220 6120 666c 6f61 7420  ess' or a float 
+00017c20: 7661 6c75 650a 2020 2020 6c6f 676d 6f64  value.    logmod
+00017c30: 656c 733a 206c 6973 745b 4c6f 6754 6175  els: list[LogTau
+00017c40: 544d 6f64 656c 5d0a 2020 2020 2020 2020  TModel].        
+00017c50: 4c69 7374 206f 6620 756e 696e 7374 616e  List of uninstan
+00017c60: 7469 6174 6564 204c 6f67 5461 7554 4d6f  tiated LogTauTMo
+00017c70: 6465 6c20 6f62 6a65 6374 730a 0a20 2020  del objects..   
+00017c80: 2041 7474 7269 6275 7465 730a 2020 2020   Attributes.    
+00017c90: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 206c  ----------.    l
+00017ca0: 6f67 6d6f 6465 6c73 3a20 6c69 7374 5b4c  ogmodels: list[L
+00017cb0: 6f67 5461 7554 4d6f 6465 6c5d 0a20 2020  ogTauTModel].   
+00017cc0: 2020 2020 204c 6973 7420 6f66 204c 6f67       List of Log
+00017cd0: 5461 7554 4d6f 6465 6c20 6f62 6a65 6374  TauTModel object
+00017ce0: 730a 2020 2020 4e41 4d45 3a20 7374 720a  s.    NAME: str.
+00017cf0: 2020 2020 2020 2020 4e61 6d65 7320 6f66          Names of
+00017d00: 2065 6163 6820 4c6f 6754 6175 544d 6f64   each LogTauTMod
+00017d10: 656c 2063 6f6e 6361 7465 6e61 7465 640a  el concatenated.
+00017d20: 2020 2020 2727 270a 0a20 2020 2064 6566      '''..    def
+00017d30: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
+00017d40: 6c6f 676d 6f64 656c 733a 206c 6973 745b  logmodels: list[
+00017d50: 4c6f 6754 6175 544d 6f64 656c 5d2c 0a20  LogTauTModel],. 
+00017d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017d70: 6669 745f 7661 7273 3a20 6c69 7374 5b64  fit_vars: list[d
+00017d80: 6963 745b 7374 722c 2066 6c6f 6174 207c  ict[str, float |
+00017d90: 2073 7472 5d5d 2c0a 2020 2020 2020 2020   str]],.        
+00017da0: 2020 2020 2020 2020 2066 6978 5f76 6172           fix_var
+00017db0: 733a 206c 6973 745b 6469 6374 5b73 7472  s: list[dict[str
+00017dc0: 2c20 666c 6f61 7420 7c20 7374 725d 5d29  , float | str]])
+00017dd0: 202d 3e20 4e6f 6e65 3a0a 0a20 2020 2020   -> None:..     
+00017de0: 2020 2023 2049 6e73 7461 6e74 6961 7465     # Instantiate
+00017df0: 2065 6163 6820 6c6f 676d 6f64 656c 2061   each logmodel a
+00017e00: 6e64 2063 7265 6174 6520 6c69 7374 206f  nd create list o
+00017e10: 6620 696e 7374 616e 7469 6174 6564 206c  f instantiated l
+00017e20: 6f67 6d6f 6465 6c73 0a20 2020 2020 2020  ogmodels.       
+00017e30: 2073 656c 662e 6c6f 676d 6f64 656c 7320   self.logmodels 
+00017e40: 3d20 7365 6c66 2e70 726f 6365 7373 5f66  = self.process_f
+00017e50: 6974 6669 7828 6669 745f 7661 7273 2c20  itfix(fit_vars, 
+00017e60: 6669 785f 7661 7273 2c20 6c6f 676d 6f64  fix_vars, logmod
+00017e70: 656c 7329 0a0a 2020 2020 2020 2020 7365  els)..        se
+00017e80: 6c66 2e4e 414d 4520 3d20 5b6c 6f67 6d6f  lf.NAME = [logmo
+00017e90: 6465 6c2e 4e41 4d45 2066 6f72 206c 6f67  del.NAME for log
+00017ea0: 6d6f 6465 6c20 696e 206c 6f67 6d6f 6465  model in logmode
+00017eb0: 6c73 5d0a 2020 2020 2020 2020 7365 6c66  ls].        self
+00017ec0: 2e4e 414d 4520 3d20 2727 2e6a 6f69 6e28  .NAME = ''.join(
+00017ed0: 5b27 7b7d 2b27 2e66 6f72 6d61 7428 6e61  ['{}+'.format(na
+00017ee0: 6d65 2920 666f 7220 6e61 6d65 2069 6e20  me) for name in 
+00017ef0: 7365 6c66 2e4e 414d 455d 295b 3a2d 315d  self.NAME])[:-1]
+00017f00: 0a0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
+00017f10: 6669 745f 7374 6174 7573 203d 2046 616c  fit_status = Fal
+00017f20: 7365 0a0a 2020 2020 2020 2020 7265 7475  se..        retu
+00017f30: 726e 0a0a 2020 2020 4070 726f 7065 7274  rn..    @propert
+00017f40: 790a 2020 2020 6465 6620 6669 745f 7374  y.    def fit_st
+00017f50: 6174 7573 2873 656c 6629 202d 3e20 626f  atus(self) -> bo
+00017f60: 6f6c 3a0a 2020 2020 2020 2020 2754 7275  ol:.        'Tru
+00017f70: 6520 6966 2066 6974 2073 7563 6365 7373  e if fit success
+00017f80: 6675 6c2c 2065 6c73 6520 4661 6c73 6527  ful, else False'
+00017f90: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00017fa0: 7365 6c66 2e5f 6669 745f 7374 6174 7573  self._fit_status
+00017fb0: 0a0a 2020 2020 4066 6974 5f73 7461 7475  ..    @fit_statu
+00017fc0: 732e 7365 7474 6572 0a20 2020 2064 6566  s.setter.    def
+00017fd0: 2066 6974 5f73 7461 7475 7328 7365 6c66   fit_status(self
+00017fe0: 2c20 7661 6c75 6529 3a0a 2020 2020 2020  , value):.      
+00017ff0: 2020 6966 2074 7970 6528 7661 6c75 6529    if type(value)
+00018000: 203d 3d20 626f 6f6c 3a0a 2020 2020 2020   == bool:.      
+00018010: 2020 2020 2020 7365 6c66 2e5f 6669 745f        self._fit_
+00018020: 7374 6174 7573 203d 2076 616c 7565 0a20  status = value. 
+00018030: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00018040: 2020 2020 2020 2020 2072 6169 7365 2054           raise T
+00018050: 7970 6545 7272 6f72 0a20 2020 2020 2020  ypeError.       
+00018060: 2072 6574 7572 6e0a 0a20 2020 2040 7374   return..    @st
+00018070: 6174 6963 6d65 7468 6f64 0a20 2020 2064  aticmethod.    d
+00018080: 6566 2070 726f 6365 7373 5f66 6974 6669  ef process_fitfi
+00018090: 7828 6669 745f 7661 7273 3a20 6c69 7374  x(fit_vars: list
+000180a0: 5b64 6963 745b 7374 722c 2066 6c6f 6174  [dict[str, float
+000180b0: 207c 2073 7472 5d5d 2c0a 2020 2020 2020   | str]],.      
+000180c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000180d0: 2066 6978 5f76 6172 733a 206c 6973 745b   fix_vars: list[
+000180e0: 6469 6374 5b73 7472 2c20 666c 6f61 7420  dict[str, float 
+000180f0: 7c20 7374 725d 5d2c 0a20 2020 2020 2020  | str]],.       
+00018100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018110: 6c6f 676d 6f64 656c 733a 206c 6973 745b  logmodels: list[
+00018120: 4c6f 6754 6175 544d 6f64 656c 5d29 202d  LogTauTModel]) -
+00018130: 3e20 6c69 7374 5b4c 6f67 5461 7554 4d6f  > list[LogTauTMo
+00018140: 6465 6c5d 3a0a 2020 2020 2020 2020 2727  del]:.        ''
+00018150: 270a 2020 2020 2020 2020 4173 736f 6369  '.        Associ
+00018160: 6174 6573 2066 6974 2061 6e64 2066 6978  ates fit and fix
+00018170: 2064 6963 7473 2077 6974 6820 6120 6c69   dicts with a li
+00018180: 7374 206f 6620 6c6f 676d 6f64 656c 7320  st of logmodels 
+00018190: 6279 2069 6e73 7461 6e74 6961 7469 6e67  by instantiating
+000181a0: 0a20 2020 2020 2020 2065 6163 6820 6c6f  .        each lo
+000181b0: 676d 6f64 656c 2077 6974 6820 7468 6520  gmodel with the 
+000181c0: 7370 6563 6966 6965 6420 7061 7261 6d65  specified parame
+000181d0: 7465 7273 0a0a 2020 2020 2020 2020 5061  ters..        Pa
+000181e0: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
+000181f0: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 0a20 2020   ----------..   
+00018200: 2020 2020 2066 6974 5f76 6172 733a 206c       fit_vars: l
+00018210: 6973 745b 6469 6374 5b73 7472 2c20 666c  ist[dict[str, fl
+00018220: 6f61 7420 7c20 7374 725d 5d0a 2020 2020  oat | str]].    
+00018230: 2020 2020 2020 2020 4c69 7374 206f 6620          List of 
+00018240: 6669 7420 6469 6374 732c 2077 6974 6820  fit dicts, with 
+00018250: 6b65 7973 2061 7320 5041 524e 414d 4553  keys as PARNAMES
+00018260: 206f 6620 6561 6368 204c 6f67 5461 7554   of each LogTauT
+00018270: 4d6f 6465 6c0a 2020 2020 2020 2020 2020  Model.          
+00018280: 2020 616e 6420 7661 6c75 6573 2061 7320    and values as 
+00018290: 6569 7468 6572 2074 6865 2073 7472 696e  either the strin
+000182a0: 6720 2767 7565 7373 2720 6f72 2061 2066  g 'guess' or a f
+000182b0: 6c6f 6174 2076 616c 7565 0a20 2020 2020  loat value.     
+000182c0: 2020 2066 6978 5f76 6172 733a 206c 6973     fix_vars: lis
+000182d0: 745b 6469 6374 5b73 7472 2c20 666c 6f61  t[dict[str, floa
+000182e0: 7420 7c20 7374 725d 5d0a 2020 2020 2020  t | str]].      
+000182f0: 2020 2020 2020 4c69 7374 206f 6620 6669        List of fi
+00018300: 7820 6469 6374 732c 2077 6974 6820 6b65  x dicts, with ke
+00018310: 7973 2061 7320 5041 524e 414d 4553 206f  ys as PARNAMES o
+00018320: 6620 6561 6368 204c 6f67 5461 7554 4d6f  f each LogTauTMo
+00018330: 6465 6c0a 2020 2020 2020 2020 2020 2020  del.            
+00018340: 616e 6420 7661 6c75 6573 2061 7320 6569  and values as ei
+00018350: 7468 6572 2074 6865 2073 7472 696e 6720  ther the string 
+00018360: 2767 7565 7373 2720 6f72 2061 2066 6c6f  'guess' or a flo
+00018370: 6174 2076 616c 7565 0a20 2020 2020 2020  at value.       
+00018380: 206c 6f67 6d6f 6465 6c73 3a20 6c69 7374   logmodels: list
+00018390: 5b4c 6f67 5461 7554 4d6f 6465 6c5d 0a20  [LogTauTModel]. 
+000183a0: 2020 2020 2020 2020 2020 204c 6973 7420             List 
+000183b0: 6f66 2075 6e69 6e73 7461 6e74 6961 7465  of uninstantiate
+000183c0: 6420 4c6f 6754 6175 544d 6f64 656c 206f  d LogTauTModel o
+000183d0: 626a 6563 7473 0a0a 2020 2020 2020 2020  bjects..        
+000183e0: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
+000183f0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+00018400: 6c69 7374 5b4c 6f67 5461 7554 4d6f 6465  list[LogTauTMode
+00018410: 6c5d 0a20 2020 2020 2020 2020 2020 2049  l].            I
+00018420: 6e73 7461 6e74 6961 7465 6420 4c6f 6754  nstantiated LogT
+00018430: 6175 544d 6f64 656c 7320 7769 7468 2066  auTModels with f
+00018440: 6974 2061 6e64 2066 6978 2064 6963 7473  it and fix dicts
+00018450: 2061 7070 6c69 6564 0a20 2020 2020 2020   applied.       
+00018460: 2027 2727 0a0a 2020 2020 2020 2020 6d61   '''..        ma
+00018470: 726b 6564 203d 205b 4661 6c73 655d 202a  rked = [False] *
+00018480: 206c 656e 2866 6974 5f76 6172 7329 0a0a   len(fit_vars)..
+00018490: 2020 2020 2020 2020 696e 7374 616e 7469          instanti
+000184a0: 6174 6564 5f6d 6f64 656c 7320 3d20 5b5d  ated_models = []
+000184b0: 0a0a 2020 2020 2020 2020 666f 7220 6c6f  ..        for lo
+000184c0: 676d 6f64 656c 2069 6e20 6c6f 676d 6f64  gmodel in logmod
+000184d0: 656c 733a 0a20 2020 2020 2020 2020 2020  els:.           
+000184e0: 2066 6f72 2069 742c 2028 6669 7476 6172   for it, (fitvar
+000184f0: 5f73 6574 2c20 6669 785f 7661 725f 7365  _set, fix_var_se
+00018500: 7429 2069 6e20 656e 756d 6572 6174 6528  t) in enumerate(
+00018510: 7a69 7028 6669 745f 7661 7273 2c20 6669  zip(fit_vars, fi
+00018520: 785f 7661 7273 2929 3a20 2320 6e6f 7161  x_vars)): # noqa
+00018530: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018540: 2069 6620 6d61 726b 6564 5b69 745d 3a0a   if marked[it]:.
+00018550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018560: 2020 2020 636f 6e74 696e 7565 0a20 2020      continue.   
+00018570: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
+00018580: 6620 616c 6c28 5b6b 2069 6e20 6c6f 676d  f all([k in logm
+00018590: 6f64 656c 2e50 4152 4e41 4d45 5320 666f  odel.PARNAMES fo
+000185a0: 7220 6b20 696e 2066 6974 7661 725f 7365  r k in fitvar_se
+000185b0: 742e 6b65 7973 2829 5d29 3a20 2320 6e6f  t.keys()]): # no
+000185c0: 7161 0a20 2020 2020 2020 2020 2020 2020  qa.             
+000185d0: 2020 2020 2020 2069 6620 616c 6c28 5b6b         if all([k
+000185e0: 2069 6e20 6c6f 676d 6f64 656c 2e50 4152   in logmodel.PAR
+000185f0: 4e41 4d45 5320 666f 7220 6b20 696e 2066  NAMES for k in f
+00018600: 6978 5f76 6172 5f73 6574 2e6b 6579 7328  ix_var_set.keys(
+00018610: 295d 2920 6f72 206e 6f74 206c 656e 2866  )]) or not len(f
+00018620: 6978 5f76 6172 5f73 6574 293a 2023 206e  ix_var_set): # n
+00018630: 6f71 610a 2020 2020 2020 2020 2020 2020  oqa.            
+00018640: 2020 2020 2020 2020 2020 2020 696e 7374              inst
+00018650: 616e 7469 6174 6564 5f6d 6f64 656c 732e  antiated_models.
+00018660: 6170 7065 6e64 280a 2020 2020 2020 2020  append(.        
+00018670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018680: 2020 2020 6c6f 676d 6f64 656c 2866 6974      logmodel(fit
+00018690: 7661 725f 7365 742c 2066 6978 5f76 6172  var_set, fix_var
+000186a0: 5f73 6574 290a 2020 2020 2020 2020 2020  _set).          
+000186b0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
 000186c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000186d0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-000186e0: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
-000186f0: 726b 6564 5b69 745d 203d 2054 7275 650a  rked[it] = True.
-00018700: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00018710: 696e 7374 616e 7469 6174 6564 5f6d 6f64  instantiated_mod
-00018720: 656c 730a 0a20 2020 2040 636c 6173 736d  els..    @classm
-00018730: 6574 686f 640a 2020 2020 6465 6620 7265  ethod.    def re
-00018740: 7369 6475 616c 5f66 726f 6d5f 666c 6f61  sidual_from_floa
-00018750: 745f 6c69 7374 2863 6c73 2c20 6e65 775f  t_list(cls, new_
-00018760: 7661 6c73 3a20 6e70 742e 4172 7261 794c  vals: npt.ArrayL
-00018770: 696b 652c 0a20 2020 2020 2020 2020 2020  ike,.           
-00018780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018790: 2020 2020 2020 6c6f 676d 6f64 656c 733a        logmodels:
-000187a0: 206c 6973 745b 4c6f 6754 6175 544d 6f64   list[LogTauTMod
-000187b0: 656c 5d2c 0a20 2020 2020 2020 2020 2020  el],.           
-000187c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000187d0: 2020 2020 2020 7465 6d70 6572 6174 7572        temperatur
-000187e0: 6573 3a20 6e70 742e 4172 7261 794c 696b  es: npt.ArrayLik
-000187f0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00018800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018810: 2020 2020 6c6f 6772 6174 653a 206e 7074      lograte: npt
-00018820: 2e41 7272 6179 4c69 6b65 2c0a 2020 2020  .ArrayLike,.    
-00018830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018840: 2020 2020 2020 2020 2020 2020 2073 6967               sig
-00018850: 6d61 3a20 6e70 742e 4172 7261 794c 696b  ma: npt.ArrayLik
-00018860: 6520 3d20 5b5d 2920 2d3e 206e 7074 2e4e  e = []) -> npt.N
-00018870: 4441 7272 6179 3a0a 2020 2020 2020 2020  DArray:.        
-00018880: 2727 270a 2020 2020 2020 2020 5772 6170  '''.        Wrap
-00018890: 7065 7220 666f 7220 6072 6573 6964 7561  per for `residua
-000188a0: 6c73 6020 6d65 7468 6f64 2c20 7461 6b65  ls` method, take
-000188b0: 7320 6e65 7720 7661 6c75 6573 2066 726f  s new values fro
-000188c0: 6d20 6669 7474 696e 6720 726f 7574 696e  m fitting routin
-000188d0: 650a 2020 2020 2020 2020 7768 6963 6820  e.        which 
-000188e0: 7072 6f76 6964 6573 206c 6973 745b 666c  provides list[fl
-000188f0: 6f61 745d 2c20 746f 2063 6f6e 7374 7275  oat], to constru
-00018900: 6374 206e 6577 2066 6974 5f76 6172 7320  ct new fit_vars 
-00018910: 6469 6374 2c20 7468 656e 0a20 2020 2020  dict, then.     
-00018920: 2020 2072 756e 7320 6072 6573 6964 7561     runs `residua
-00018930: 6c73 6020 6d65 7468 6f64 2e0a 0a20 2020  ls` method...   
-00018940: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
-00018950: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-00018960: 2d2d 0a20 2020 2020 2020 206e 6577 5f76  --.        new_v
-00018970: 616c 733a 2061 7272 6179 5f6c 696b 650a  als: array_like.
-00018980: 2020 2020 2020 2020 2020 2020 5468 6973              This
-00018990: 2069 7465 7261 7469 6f6e 2773 2066 6974   iteration's fit
-000189a0: 2070 6172 616d 6574 6572 2076 616c 7565   parameter value
-000189b0: 7320 7072 6f76 6964 6564 2062 7920 6c65  s provided by le
-000189c0: 6173 745f 7371 7561 7265 730a 2020 2020  ast_squares.    
-000189d0: 2020 2020 2020 2020 7468 6973 2068 6173          this has
-000189e0: 2074 6865 2073 616d 6520 6f72 6465 7220   the same order 
-000189f0: 6174 2066 6974 5f76 6172 732e 6b65 7973  at fit_vars.keys
-00018a00: 0a20 2020 2020 2020 206c 6f67 6d6f 6465  .        logmode
-00018a10: 6c73 3a20 6c69 7374 5b4c 6f67 5461 7554  ls: list[LogTauT
-00018a20: 4d6f 6465 6c5d 0a20 2020 2020 2020 2020  Model].         
-00018a30: 2020 204d 6f64 656c 7320 746f 2075 7365     Models to use
-00018a40: 0a20 2020 2020 2020 2074 656d 7065 7261  .        tempera
-00018a50: 7475 7265 733a 2061 7272 6179 5f6c 696b  tures: array_lik
-00018a60: 650a 2020 2020 2020 2020 2020 2020 5465  e.            Te
-00018a70: 6d70 6572 6174 7572 6520 7661 6c75 6573  mperature values
-00018a80: 2028 4b29 2061 7420 7768 6963 6820 6d6f   (K) at which mo
-00018a90: 6465 6c20 6675 6e63 7469 6f6e 2069 7320  del function is 
-00018aa0: 6576 616c 7561 7465 640a 2020 2020 2020  evaluated.      
-00018ab0: 2020 6c6f 6772 6174 653a 2061 7272 6179    lograte: array
-00018ac0: 5f6c 696b 650a 2020 2020 2020 2020 2020  _like.          
-00018ad0: 2020 5472 7565 2028 6578 7065 7269 6d65    True (experime
-00018ae0: 6e74 616c 2920 7661 6c75 6573 206f 6620  ntal) values of 
-00018af0: 6c6f 6731 3028 7265 6c61 7861 7469 6f6e  log10(relaxation
-00018b00: 2072 6174 6529 0a20 2020 2020 2020 2073   rate).        s
-00018b10: 6967 6d61 3a20 6172 7261 795f 6c69 6b65  igma: array_like
-00018b20: 0a20 2020 2020 2020 2020 2020 2053 7461  .            Sta
-00018b30: 6e64 6172 6420 6465 7669 6174 696f 6e20  ndard deviation 
-00018b40: 6f66 2074 6175 2069 6e20 6c6f 6773 7061  of tau in logspa
-00018b50: 6365 0a0a 2020 2020 2020 2020 5265 7475  ce..        Retu
-00018b60: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
-00018b70: 2d2d 2d0a 2020 2020 2020 2020 6e64 6172  ---.        ndar
-00018b80: 7261 7920 6f66 2066 6c6f 6174 730a 2020  ray of floats.  
-00018b90: 2020 2020 2020 2020 2020 5265 7369 6475            Residu
-00018ba0: 616c 730a 2020 2020 2020 2020 2727 270a  als.        '''.
-00018bb0: 0a20 2020 2020 2020 2023 2053 7761 7020  .        # Swap 
-00018bc0: 6669 7420 7661 6c75 6573 2066 6f72 206e  fit values for n
-00018bd0: 6577 2076 616c 7565 7320 6672 6f6d 2066  ew values from f
-00018be0: 6974 2072 6f75 7469 6e65 0a20 2020 2020  it routine.     
-00018bf0: 2020 206e 6577 5f66 6974 5f76 6172 7320     new_fit_vars 
-00018c00: 3d20 5b5d 0a0a 2020 2020 2020 2020 6974  = []..        it
-00018c10: 203d 2030 0a20 2020 2020 2020 2066 6f72   = 0.        for
-00018c20: 206c 6f67 6d6f 6465 6c20 696e 206c 6f67   logmodel in log
-00018c30: 6d6f 6465 6c73 3a0a 2020 2020 2020 2020  models:.        
-00018c40: 2020 2020 6e65 775f 6469 6374 203d 207b      new_dict = {
-00018c50: 7d0a 2020 2020 2020 2020 2020 2020 666f  }.            fo
-00018c60: 7220 6e61 6d65 2069 6e20 6c6f 676d 6f64  r name in logmod
-00018c70: 656c 2e66 6974 5f76 6172 732e 6b65 7973  el.fit_vars.keys
-00018c80: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00018c90: 2020 2020 6e65 775f 6469 6374 5b6e 616d      new_dict[nam
-00018ca0: 655d 203d 206e 6577 5f76 616c 735b 6974  e] = new_vals[it
-00018cb0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-00018cc0: 2020 6974 202b 3d20 310a 2020 2020 2020    it += 1.      
-00018cd0: 2020 2020 2020 6e65 775f 6669 745f 7661        new_fit_va
-00018ce0: 7273 2e61 7070 656e 6428 6e65 775f 6469  rs.append(new_di
-00018cf0: 6374 290a 0a20 2020 2020 2020 2072 6573  ct)..        res
-00018d00: 6964 7561 6c73 203d 2063 6c73 2e72 6573  iduals = cls.res
-00018d10: 6964 7561 6c73 280a 2020 2020 2020 2020  iduals(.        
-00018d20: 2020 2020 6c6f 676d 6f64 656c 732c 206e      logmodels, n
-00018d30: 6577 5f66 6974 5f76 6172 732c 2074 656d  ew_fit_vars, tem
-00018d40: 7065 7261 7475 7265 732c 206c 6f67 7261  peratures, logra
-00018d50: 7465 0a20 2020 2020 2020 2029 0a0a 2020  te.        )..  
-00018d60: 2020 2020 2020 6966 206c 656e 2873 6967        if len(sig
-00018d70: 6d61 293a 0a20 2020 2020 2020 2020 2020  ma):.           
-00018d80: 2072 6573 6964 7561 6c73 202f 3d20 7369   residuals /= si
-00018d90: 676d 610a 0a20 2020 2020 2020 2072 6574  gma..        ret
-00018da0: 7572 6e20 7265 7369 6475 616c 730a 0a20  urn residuals.. 
-00018db0: 2020 2040 7374 6174 6963 6d65 7468 6f64     @staticmethod
-00018dc0: 0a20 2020 2064 6566 2072 6573 6964 7561  .    def residua
-00018dd0: 6c73 286c 6f67 6d6f 6465 6c73 3a20 6c69  ls(logmodels: li
-00018de0: 7374 5b4c 6f67 5461 7554 4d6f 6465 6c5d  st[LogTauTModel]
-00018df0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00018e00: 2020 2020 6e65 775f 6669 745f 7661 7273      new_fit_vars
-00018e10: 3a20 6c69 7374 5b64 6963 745b 7374 722c  : list[dict[str,
-00018e20: 2066 6c6f 6174 5d5d 2c0a 2020 2020 2020   float]],.      
-00018e30: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
-00018e40: 6572 6174 7572 6573 3a20 6e70 742e 4172  eratures: npt.Ar
-00018e50: 7261 794c 696b 652c 0a20 2020 2020 2020  rayLike,.       
-00018e60: 2020 2020 2020 2020 2020 2074 7275 655f             true_
-00018e70: 6c6f 6772 6174 653a 206e 7074 2e41 7272  lograte: npt.Arr
-00018e80: 6179 4c69 6b65 2920 2d3e 206e 7074 2e4e  ayLike) -> npt.N
-00018e90: 4441 7272 6179 3a0a 2020 2020 2020 2020  DArray:.        
-00018ea0: 2727 270a 2020 2020 2020 2020 4361 6c63  '''.        Calc
-00018eb0: 756c 6174 6573 2064 6966 6665 7265 6e63  ulates differenc
-00018ec0: 6520 6265 7477 6565 6e20 6578 7065 7269  e between experi
-00018ed0: 6d65 6e74 616c 206c 6f67 3130 2874 6175  mental log10(tau
-00018ee0: 5e2d 3129 0a20 2020 2020 2020 2061 6e64  ^-1).        and
-00018ef0: 206c 6f67 3130 2874 6175 5e2d 3129 206f   log10(tau^-1) o
-00018f00: 6274 6169 6e65 6420 6672 6f6d 2074 6865  btained from the
-00018f10: 2073 756d 206f 6620 7468 6520 7072 6f76   sum of the prov
-00018f20: 6964 6564 206c 6f67 6d6f 6465 6c73 0a20  ided logmodels. 
-00018f30: 2020 2020 2020 2075 7369 6e67 2074 6865         using the
-00018f40: 2070 726f 7669 6465 6420 6669 7420 7661   provided fit va
-00018f50: 7269 6162 6c65 2076 616c 7565 7320 6174  riable values at
-00018f60: 2070 726f 7669 6465 6420 7465 6d70 6572   provided temper
-00018f70: 6174 7572 6573 0a0a 2020 2020 2020 2020  atures..        
-00018f80: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
-00018f90: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-00018fa0: 2020 2020 2020 6c6f 676d 6f64 656c 733a        logmodels:
-00018fb0: 206c 6973 745b 4c6f 6754 6175 544d 6f64   list[LogTauTMod
-00018fc0: 656c 5d0a 2020 2020 2020 2020 2020 2020  el].            
-00018fd0: 4c6f 6754 6175 544d 6f64 656c 7320 7768  LogTauTModels wh
-00018fe0: 6963 6820 7769 6c6c 2062 6520 6576 616c  ich will be eval
-00018ff0: 7561 7465 640a 2020 2020 2020 2020 6e65  uated.        ne
-00019000: 775f 6669 745f 7661 7273 3a20 6c69 7374  w_fit_vars: list
-00019010: 5b64 6963 745b 7374 722c 2066 6c6f 6174  [dict[str, float
-00019020: 5d5d 0a20 2020 2020 2020 2020 2020 2066  ]].            f
-00019030: 6974 2064 6963 7473 2066 6f72 2065 6163  it dicts for eac
-00019040: 6820 4c6f 6754 6175 544d 6f64 656c 2c20  h LogTauTModel, 
-00019050: 6d75 7374 2068 6176 6520 7361 6d65 206f  must have same o
-00019060: 7264 6572 2061 7320 6c6f 676d 6f64 656c  rder as logmodel
-00019070: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00019080: 6e6f 2076 6172 7320 746f 2066 6974 2066  no vars to fit f
-00019090: 6f72 2074 6861 7420 6d6f 6465 6c2c 2074  or that model, t
-000190a0: 6865 6e20 656d 7074 7920 6469 6374 2069  hen empty dict i
-000190b0: 7320 6769 7665 6e0a 2020 2020 2020 2020  s given.        
-000190c0: 7465 6d70 6572 6174 7572 6573 3a20 6172  temperatures: ar
-000190d0: 7261 795f 6c69 6b65 0a20 2020 2020 2020  ray_like.       
-000190e0: 2020 2020 2045 7870 6572 696d 656e 7461       Experimenta
-000190f0: 6c20 7465 6d70 6572 6174 7572 6573 2028  l temperatures (
-00019100: 4b29 0a20 2020 2020 2020 2074 7275 655f  K).        true_
-00019110: 6c6f 6772 6174 653a 2061 7272 6179 5f6c  lograte: array_l
-00019120: 696b 650a 2020 2020 2020 2020 2020 2020  ike.            
-00019130: 4578 7065 7269 6d65 6e74 616c 204c 6f67  Experimental Log
-00019140: 3130 2872 6174 6529 730a 0a20 2020 2020  10(rate)s..     
-00019150: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
-00019160: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
-00019170: 2020 206e 6461 7272 6179 206f 6620 666c     ndarray of fl
-00019180: 6f61 7473 0a20 2020 2020 2020 2020 2020  oats.           
-00019190: 204c 6f67 3130 2872 6174 6529 5f74 7269   Log10(rate)_tri
-000191a0: 616c 202d 204c 6f67 3130 2872 6174 6529  al - Log10(rate)
-000191b0: 5f65 7870 2066 6f72 2065 6163 6820 7465  _exp for each te
-000191c0: 6d70 6572 6174 7572 650a 2020 2020 2020  mperature.      
-000191d0: 2020 2727 270a 0a20 2020 2020 2020 2023    '''..        #
-000191e0: 2043 616c 6375 6c61 7465 206d 6f64 656c   Calculate model
-000191f0: 206c 6f67 3130 2872 656c 6178 6174 696f   log10(relaxatio
-00019200: 6e20 7261 7465 2920 7573 696e 6720 7061  n rate) using pa
-00019210: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
-00019220: 2023 2061 7320 7375 6d20 6f66 2063 6f6e   # as sum of con
-00019230: 7472 6962 7574 696f 6e73 2066 726f 6d20  tributions from 
-00019240: 6561 6368 2070 726f 6365 7373 0a20 2020  each process.   
-00019250: 2020 2020 2074 7269 616c 5f6c 6f67 7261       trial_logra
-00019260: 7465 203d 206e 702e 7a65 726f 7328 6c65  te = np.zeros(le
-00019270: 6e28 7465 6d70 6572 6174 7572 6573 2929  n(temperatures))
-00019280: 0a0a 2020 2020 2020 2020 666f 7220 6c6f  ..        for lo
-00019290: 676d 6f64 656c 2c20 6669 745f 7661 7273  gmodel, fit_vars
-000192a0: 2069 6e20 7a69 7028 6c6f 676d 6f64 656c   in zip(logmodel
-000192b0: 732c 206e 6577 5f66 6974 5f76 6172 7329  s, new_fit_vars)
-000192c0: 3a0a 2020 2020 2020 2020 2020 2020 616c  :.            al
-000192d0: 6c5f 7661 7273 203d 207b 2a2a 6c6f 676d  l_vars = {**logm
-000192e0: 6f64 656c 2e66 6978 5f76 6172 732c 202a  odel.fix_vars, *
-000192f0: 2a66 6974 5f76 6172 737d 0a20 2020 2020  *fit_vars}.     
-00019300: 2020 2020 2020 2074 7269 616c 5f6c 6f67         trial_log
-00019310: 7261 7465 202b 3d20 3130 2a2a 6c6f 676d  rate += 10**logm
-00019320: 6f64 656c 2e6d 6f64 656c 2861 6c6c 5f76  odel.model(all_v
-00019330: 6172 732c 2074 656d 7065 7261 7475 7265  ars, temperature
-00019340: 7329 0a0a 2020 2020 2020 2020 2320 7375  s)..        # su
-00019350: 6d20 696e 206c 696e 6561 7220 7370 6163  m in linear spac
-00019360: 652c 2074 6865 6e20 7461 6b65 206c 6f67  e, then take log
-00019370: 0a20 2020 2020 2020 2074 7269 616c 5f6c  .        trial_l
-00019380: 6f67 7261 7465 203d 206e 702e 6c6f 6731  ograte = np.log1
-00019390: 3028 7472 6961 6c5f 6c6f 6772 6174 6529  0(trial_lograte)
-000193a0: 0a0a 2020 2020 2020 2020 7265 7369 6475  ..        residu
-000193b0: 616c 7320 3d20 7472 6961 6c5f 6c6f 6772  als = trial_logr
-000193c0: 6174 6520 2d20 7472 7565 5f6c 6f67 7261  ate - true_logra
-000193d0: 7465 0a0a 2020 2020 2020 2020 7265 7475  te..        retu
-000193e0: 726e 2072 6573 6964 7561 6c73 0a0a 2020  rn residuals..  
-000193f0: 2020 6465 6620 6669 745f 746f 2873 656c    def fit_to(sel
-00019400: 662c 2064 6174 6173 6574 3a20 5461 7554  f, dataset: TauT
-00019410: 4461 7461 7365 742c 2076 6572 626f 7365  Dataset, verbose
-00019420: 3a20 626f 6f6c 203d 2054 7275 6529 202d  : bool = True) -
-00019430: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-00019440: 2727 270a 2020 2020 2020 2020 4669 7473  '''.        Fits
-00019450: 206d 6f64 656c 2074 6f20 4461 7461 7365   model to Datase
-00019460: 740a 0a20 2020 2020 2020 2050 6172 616d  t..        Param
-00019470: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
-00019480: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
-00019490: 2064 6174 6173 6574 3a20 5461 7554 4461   dataset: TauTDa
-000194a0: 7461 7365 740a 2020 2020 2020 2020 2020  taset.          
-000194b0: 2020 4461 7461 7365 7420 746f 2077 6869    Dataset to whi
-000194c0: 6368 2061 206d 6f64 656c 206f 6620 7261  ch a model of ra
-000194d0: 7465 2076 7320 7465 6d70 6572 6174 7572  te vs temperatur
-000194e0: 6520 7769 6c6c 2062 6520 6669 7474 6564  e will be fitted
-000194f0: 0a20 2020 2020 2020 2076 6572 626f 7365  .        verbose
-00019500: 3a20 626f 6f6c 2c20 6465 6661 756c 7420  : bool, default 
-00019510: 5472 7565 0a20 2020 2020 2020 2020 2020  True.           
-00019520: 2049 6620 5472 7565 2c20 7072 696e 7473   If True, prints
-00019530: 2069 6e66 6f72 6d61 7469 6f6e 2074 6f20   information to 
-00019540: 7465 726d 696e 616c 0a0a 2020 2020 2020  terminal..      
-00019550: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
-00019560: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
-00019570: 2020 4e6f 6e65 0a20 2020 2020 2020 2027    None.        '
-00019580: 2727 0a0a 2020 2020 2020 2020 2320 496e  ''..        # In
-00019590: 6974 6961 6c20 6775 6573 7320 6973 2061  itial guess is a
-000195a0: 206c 6973 7420 6f66 2066 6974 7661 7273   list of fitvars
-000195b0: 2076 616c 7565 730a 2020 2020 2020 2020   values.        
-000195c0: 6775 6573 7320 3d20 5b0a 2020 2020 2020  guess = [.      
-000195d0: 2020 2020 2020 7661 6c75 6520 666f 7220        value for 
-000195e0: 6c6f 676d 6f64 656c 2069 6e20 7365 6c66  logmodel in self
-000195f0: 2e6c 6f67 6d6f 6465 6c73 0a20 2020 2020  .logmodels.     
-00019600: 2020 2020 2020 2066 6f72 2076 616c 7565         for value
-00019610: 2069 6e20 6c6f 676d 6f64 656c 2e66 6974   in logmodel.fit
-00019620: 5f76 6172 732e 7661 6c75 6573 2829 0a20  _vars.values(). 
-00019630: 2020 2020 2020 205d 0a0a 2020 2020 2020         ]..      
-00019640: 2020 626f 756e 6473 203d 206e 702e 6172    bounds = np.ar
-00019650: 7261 7928 5b0a 2020 2020 2020 2020 2020  ray([.          
-00019660: 2020 6c6f 676d 6f64 656c 2e42 4f55 4e44    logmodel.BOUND
-00019670: 535b 6e61 6d65 5d20 666f 7220 6c6f 676d  S[name] for logm
-00019680: 6f64 656c 2069 6e20 7365 6c66 2e6c 6f67  odel in self.log
-00019690: 6d6f 6465 6c73 0a20 2020 2020 2020 2020  models.         
-000196a0: 2020 2066 6f72 206e 616d 6520 696e 206c     for name in l
-000196b0: 6f67 6d6f 6465 6c2e 6669 745f 7661 7273  ogmodel.fit_vars
-000196c0: 2e6b 6579 7328 290a 2020 2020 2020 2020  .keys().        
-000196d0: 5d29 2e54 0a0a 2020 2020 2020 2020 6375  ]).T..        cu
-000196e0: 7272 5f66 6974 203d 206c 6561 7374 5f73  rr_fit = least_s
-000196f0: 7175 6172 6573 280a 2020 2020 2020 2020  quares(.        
-00019700: 2020 2020 7365 6c66 2e72 6573 6964 7561      self.residua
-00019710: 6c5f 6672 6f6d 5f66 6c6f 6174 5f6c 6973  l_from_float_lis
-00019720: 742c 0a20 2020 2020 2020 2020 2020 2061  t,.            a
-00019730: 7267 733d 5b0a 2020 2020 2020 2020 2020  rgs=[.          
-00019740: 2020 2020 2020 7365 6c66 2e6c 6f67 6d6f        self.logmo
-00019750: 6465 6c73 2c0a 2020 2020 2020 2020 2020  dels,.          
-00019760: 2020 2020 2020 6461 7461 7365 742e 7465        dataset.te
-00019770: 6d70 6572 6174 7572 6573 2c0a 2020 2020  mperatures,.    
-00019780: 2020 2020 2020 2020 2020 2020 6e70 2e6c              np.l
-00019790: 6f67 3130 2864 6174 6173 6574 2e72 6174  og10(dataset.rat
-000197a0: 6573 292c 0a20 2020 2020 2020 2020 2020  es),.           
-000197b0: 2020 2020 2064 6174 6173 6574 2e6c 6f67       dataset.log
-000197c0: 7261 7465 5f70 6d0a 2020 2020 2020 2020  rate_pm.        
-000197d0: 2020 2020 5d2c 0a20 2020 2020 2020 2020      ],.         
-000197e0: 2020 2078 303d 6775 6573 732c 0a20 2020     x0=guess,.   
-000197f0: 2020 2020 2020 2020 2062 6f75 6e64 733d           bounds=
-00019800: 626f 756e 6473 2c0a 2020 2020 2020 2020  bounds,.        
-00019810: 2020 2020 6a61 633d 2733 2d70 6f69 6e74      jac='3-point
-00019820: 270a 2020 2020 2020 2020 290a 0a20 2020  '.        )..   
-00019830: 2020 2020 2069 6620 6375 7272 5f66 6974       if curr_fit
-00019840: 2e73 7461 7475 7320 3d3d 2030 3a0a 2020  .status == 0:.  
-00019850: 2020 2020 2020 2020 2020 6966 2076 6572            if ver
-00019860: 626f 7365 3a0a 2020 2020 2020 2020 2020  bose:.          
-00019870: 2020 2020 2020 7574 2e63 7072 696e 7428        ut.cprint(
-00019880: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019890: 2020 2020 2027 5c6e 2046 6974 2066 6169       '\n Fit fai
-000198a0: 6c65 6420 2d20 546f 6f20 6d61 6e79 2069  led - Too many i
-000198b0: 7465 7261 7469 6f6e 7327 2c0a 2020 2020  terations',.    
-000198c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000198d0: 2762 6c61 636b 5f79 656c 6c6f 7762 6727  'black_yellowbg'
-000198e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000198f0: 2029 0a0a 2020 2020 2020 2020 2020 2020   )..            
-00019900: 6e5f 6669 7474 6564 5f70 6172 7320 3d20  n_fitted_pars = 
-00019910: 6e70 2e73 756d 280a 2020 2020 2020 2020  np.sum(.        
-00019920: 2020 2020 2020 2020 5b6c 656e 286c 6f67          [len(log
-00019930: 6d6f 6465 6c2e 6669 745f 7661 7273 2e6b  model.fit_vars.k
-00019940: 6579 7328 2929 2066 6f72 206c 6f67 6d6f  eys()) for logmo
-00019950: 6465 6c20 696e 2073 656c 662e 6c6f 676d  del in self.logm
-00019960: 6f64 656c 735d 0a20 2020 2020 2020 2020  odels].         
-00019970: 2020 2029 0a0a 2020 2020 2020 2020 2020     )..          
-00019980: 2020 7374 6465 7620 3d20 5b6e 702e 6e61    stdev = [np.na
-00019990: 6e5d 202a 206e 5f66 6974 7465 645f 7061  n] * n_fitted_pa
-000199a0: 7273 0a20 2020 2020 2020 2020 2020 2073  rs.            s
-000199b0: 656c 662e 6669 745f 7374 6174 7573 203d  elf.fit_status =
-000199c0: 2046 616c 7365 0a20 2020 2020 2020 2065   False.        e
-000199d0: 6c73 653a 0a0a 2020 2020 2020 2020 2020  lse:..          
-000199e0: 2020 7374 6465 762c 206e 6f5f 7374 6465    stdev, no_stde
-000199f0: 7620 3d20 7374 6174 732e 7376 645f 7374  v = stats.svd_st
-00019a00: 6465 7628 6375 7272 5f66 6974 290a 0a20  dev(curr_fit).. 
-00019a10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00019a20: 6669 745f 7374 6174 7573 203d 2054 7275  fit_status = Tru
-00019a30: 650a 0a20 2020 2020 2020 2023 2041 6464  e..        # Add
-00019a40: 2070 6172 616d 6574 6572 732c 2073 7461   parameters, sta
-00019a50: 7475 7320 616e 6420 7374 6465 7620 746f  tus and stdev to
-00019a60: 2065 6163 6820 4c6f 6754 6175 544d 6f64   each LogTauTMod
-00019a70: 656c 0a20 2020 2020 2020 2069 7420 3d20  el.        it = 
-00019a80: 300a 2020 2020 2020 2020 666f 7220 6c6f  0.        for lo
-00019a90: 676d 6f64 656c 2069 6e20 7365 6c66 2e6c  gmodel in self.l
-00019aa0: 6f67 6d6f 6465 6c73 3a0a 0a20 2020 2020  ogmodels:..     
-00019ab0: 2020 2020 2020 2023 204e 616d 6520 6f66         # Name of
-00019ac0: 2066 6974 7465 6420 7661 7269 6162 6c65   fitted variable
-00019ad0: 7320 696e 2074 6869 7320 6c6f 676d 6f64  s in this logmod
-00019ae0: 656c 0a20 2020 2020 2020 2020 2020 2066  el.            f
-00019af0: 6974 5f76 6172 5f6e 616d 6573 203d 206c  it_var_names = l
-00019b00: 6f67 6d6f 6465 6c2e 6669 745f 7661 7273  ogmodel.fit_vars
-00019b10: 2e6b 6579 7328 290a 2020 2020 2020 2020  .keys().        
-00019b20: 2020 2020 2320 4e75 6d62 6572 206f 6620      # Number of 
-00019b30: 7061 7261 6d65 7465 7273 2066 6f72 2074  parameters for t
-00019b40: 6869 7320 6c6f 676d 6f64 656c 0a20 2020  his logmodel.   
-00019b50: 2020 2020 2020 2020 206e 5f70 6172 7320           n_pars 
-00019b60: 3d20 6c65 6e28 6669 745f 7661 725f 6e61  = len(fit_var_na
-00019b70: 6d65 7329 0a0a 2020 2020 2020 2020 2020  mes)..          
-00019b80: 2020 2320 5365 7420 6561 6368 2073 7461    # Set each sta
-00019b90: 6e64 6172 6420 6465 7669 6174 696f 6e0a  ndard deviation.
-00019ba0: 2020 2020 2020 2020 2020 2020 5f73 7464              _std
-00019bb0: 6576 203d 2073 7464 6576 5b69 743a 2069  ev = stdev[it: i
-00019bc0: 7420 2b20 6e5f 7061 7273 5d0a 2020 2020  t + n_pars].    
-00019bd0: 2020 2020 2020 2020 6c6f 676d 6f64 656c          logmodel
-00019be0: 2e66 6974 5f73 7464 6576 203d 207b 0a20  .fit_stdev = {. 
-00019bf0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00019c00: 6162 656c 3a20 7661 6c0a 2020 2020 2020  abel: val.      
-00019c10: 2020 2020 2020 2020 2020 666f 7220 6c61            for la
-00019c20: 6265 6c2c 2076 616c 2069 6e20 7a69 7028  bel, val in zip(
-00019c30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019c40: 2020 2020 2066 6974 5f76 6172 5f6e 616d       fit_var_nam
-00019c50: 6573 2c20 5f73 7464 6576 0a20 2020 2020  es, _stdev.     
-00019c60: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00019c70: 2020 2020 2020 2020 207d 0a0a 2020 2020           }..    
-00019c80: 2020 2020 2020 2020 2320 5265 706f 7274          # Report
-00019c90: 2073 696e 6775 6c61 7220 7661 6c75 6573   singular values
-00019ca0: 3d30 206f 6620 4a61 636f 6269 616e 0a20  =0 of Jacobian. 
-00019cb0: 2020 2020 2020 2020 2020 2023 2061 6e64             # and
-00019cc0: 2069 6e64 6963 6174 6520 7468 6174 2073   indicate that s
-00019cd0: 7464 5f64 6576 2063 616e 6e6f 7420 6265  td_dev cannot be
-00019ce0: 2063 616c 6375 6c61 7465 640a 2020 2020   calculated.    
-00019cf0: 2020 2020 2020 2020 7369 6e67 7320 3d20          sings = 
-00019d00: 6e6f 5f73 7464 6576 5b69 743a 2069 7420  no_stdev[it: it 
-00019d10: 2b20 6e5f 7061 7273 5d0a 2020 2020 2020  + n_pars].      
-00019d20: 2020 2020 2020 666f 7220 7061 722c 2073        for par, s
-00019d30: 6920 696e 207a 6970 2866 6974 5f76 6172  i in zip(fit_var
-00019d40: 5f6e 616d 6573 2c20 7369 6e67 7329 3a0a  _names, sings):.
-00019d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019d60: 6966 2076 6572 626f 7365 2061 6e64 206e  if verbose and n
-00019d70: 6f74 2073 693a 0a20 2020 2020 2020 2020  ot si:.         
-00019d80: 2020 2020 2020 2020 2020 2075 742e 6370             ut.cp
-00019d90: 7269 6e74 280a 2020 2020 2020 2020 2020  rint(.          
-00019da0: 2020 2020 2020 2020 2020 2020 2020 6627                f'
-00019db0: 5761 726e 696e 673a 204a 6163 6f62 6961  Warning: Jacobia
-00019dc0: 6e20 6973 2064 6567 656e 6572 6174 6520  n is degenerate 
-00019dd0: 666f 7220 7b70 6172 7d2c 2073 7461 6e64  for {par}, stand
-00019de0: 6172 6420 6465 7669 6174 696f 6e20 6361  ard deviation ca
-00019df0: 6e6e 6f74 2062 6520 666f 756e 642c 2061  nnot be found, a
-00019e00: 6e64 2069 7320 7365 7420 746f 207a 6572  nd is set to zer
-00019e10: 6f5c 6e27 2c20 2320 6e6f 7161 0a20 2020  o\n', # noqa.   
-00019e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019e30: 2020 2020 2027 626c 6163 6b5f 7965 6c6c       'black_yell
-00019e40: 6f77 6267 270a 2020 2020 2020 2020 2020  owbg'.          
-00019e50: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
-00019e60: 2020 2020 2020 2020 2023 2053 6574 2066           # Set f
-00019e70: 696e 616c 2066 6974 7465 6420 7661 6c75  inal fitted valu
-00019e80: 6573 0a20 2020 2020 2020 2020 2020 205f  es.            _
-00019e90: 7661 6c73 203d 2063 7572 725f 6669 742e  vals = curr_fit.
-00019ea0: 785b 6974 3a20 6974 202b 206e 5f70 6172  x[it: it + n_par
-00019eb0: 735d 0a20 2020 2020 2020 2020 2020 206c  s].            l
-00019ec0: 6f67 6d6f 6465 6c2e 6669 6e61 6c5f 7661  ogmodel.final_va
-00019ed0: 725f 7661 6c75 6573 203d 207b 0a20 2020  r_values = {.   
-00019ee0: 2020 2020 2020 2020 2020 2020 206e 616d               nam
-00019ef0: 653a 2076 616c 7565 0a20 2020 2020 2020  e: value.       
-00019f00: 2020 2020 2020 2020 2066 6f72 206e 616d           for nam
-00019f10: 652c 2076 616c 7565 2069 6e20 7a69 7028  e, value in zip(
-00019f20: 6669 745f 7661 725f 6e61 6d65 732c 205f  fit_var_names, _
-00019f30: 7661 6c73 290a 2020 2020 2020 2020 2020  vals).          
-00019f40: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
-00019f50: 2320 616e 6420 6669 7865 6420 7661 6c75  # and fixed valu
-00019f60: 6573 0a20 2020 2020 2020 2020 2020 2066  es.            f
-00019f70: 6f72 206b 6579 2c20 7661 6c20 696e 206c  or key, val in l
-00019f80: 6f67 6d6f 6465 6c2e 6669 785f 7661 7273  ogmodel.fix_vars
-00019f90: 2e69 7465 6d73 2829 3a0a 2020 2020 2020  .items():.      
-00019fa0: 2020 2020 2020 2020 2020 6c6f 676d 6f64            logmod
-00019fb0: 656c 2e66 696e 616c 5f76 6172 5f76 616c  el.final_var_val
-00019fc0: 7565 735b 6b65 795d 203d 2076 616c 0a0a  ues[key] = val..
-00019fd0: 2020 2020 2020 2020 2020 2020 6974 202b              it +
-00019fe0: 3d20 6e5f 7061 7273 0a0a 2020 2020 2020  = n_pars..      
-00019ff0: 2020 7265 7475 726e 0a0a 0a63 6c61 7373    return...class
-0001a000: 2046 6974 5769 6e64 6f77 2851 7457 6964   FitWindow(QtWid
-0001a010: 6765 7473 2e51 4d61 696e 5769 6e64 6f77  gets.QMainWindow
-0001a020: 293a 0a20 2020 2027 2727 0a20 2020 2049  ):.    '''.    I
-0001a030: 6e74 6572 6163 7469 7665 2046 6974 2057  nteractive Fit W
-0001a040: 696e 646f 7720 666f 7220 7261 7465 2076  indow for rate v
-0001a050: 7320 7465 6d70 6572 6174 7572 652f 6669  s temperature/fi
-0001a060: 656c 6420 6461 7461 2066 6974 7469 6e67  eld data fitting
-0001a070: 0a20 2020 2027 2727 0a0a 2020 2020 6465  .    '''..    de
-0001a080: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
-0001a090: 2064 6174 6173 6574 3a20 5461 7554 4461   dataset: TauTDa
-0001a0a0: 7461 7365 7420 7c20 5461 7548 4461 7461  taset | TauHData
-0001a0b0: 7365 742c 2075 7365 6c3a 206f 626a 6563  set, usel: objec
-0001a0c0: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
-0001a0d0: 2020 2020 7375 7070 6f72 7465 645f 6d6f      supported_mo
-0001a0e0: 6465 6c73 3a20 6c69 7374 2c0a 2020 2020  dels: list,.    
-0001a0f0: 2020 2020 2020 2020 2020 2020 2077 6964               wid
-0001a100: 6765 745f 6465 6661 756c 7473 3a20 6469  get_defaults: di
-0001a110: 6374 5b73 7472 2c20 6469 6374 5b73 7472  ct[str, dict[str
-0001a120: 2c20 666c 6f61 745d 5d20 3d20 6775 692e  , float]] = gui.
-0001a130: 7769 6467 6574 5f64 6566 6175 6c74 732c  widget_defaults,
-0001a140: 2023 206e 6f71 610a 2020 2020 2020 2020   # noqa.        
-0001a150: 2020 2020 2020 2020 202a 6172 6773 2c20           *args, 
-0001a160: 2a2a 6b77 6172 6773 293a 0a0a 2020 2020  **kwargs):..    
-0001a170: 2020 2020 7375 7065 7228 4669 7457 696e      super(FitWin
-0001a180: 646f 772c 2073 656c 6629 2e5f 5f69 6e69  dow, self).__ini
-0001a190: 745f 5f28 2a61 7267 732c 202a 2a6b 7761  t__(*args, **kwa
-0001a1a0: 7267 7329 0a0a 2020 2020 2020 2020 2320  rgs)..        # 
-0001a1b0: 4164 6420 7368 6f72 7463 7574 2074 6f20  Add shortcut to 
-0001a1c0: 7072 6573 7320 7120 746f 2071 7569 740a  press q to quit.
-0001a1d0: 2020 2020 2020 2020 7365 6c66 2e65 7869          self.exi
-0001a1e0: 745f 7368 6f72 7463 7574 203d 2051 7457  t_shortcut = QtW
-0001a1f0: 6964 6765 7473 2e51 5368 6f72 7463 7574  idgets.QShortcut
-0001a200: 2851 7447 7569 2e51 4b65 7953 6571 7565  (QtGui.QKeySeque
-0001a210: 6e63 6528 2771 2729 2c20 7365 6c66 290a  nce('q'), self).
-0001a220: 2020 2020 2020 2020 7365 6c66 2e65 7869          self.exi
-0001a230: 745f 7368 6f72 7463 7574 2e61 6374 6976  t_shortcut.activ
-0001a240: 6174 6564 2e63 6f6e 6e65 6374 280a 2020  ated.connect(.  
-0001a250: 2020 2020 2020 2020 2020 6c61 6d62 6461            lambda
-0001a260: 3a20 7365 6c66 2e63 6c6f 7365 2829 0a20  : self.close(). 
-0001a270: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-0001a280: 2020 7365 6c66 2e73 6574 5769 6e64 6f77    self.setWindow
-0001a290: 5469 746c 6528 2749 6e74 6572 6163 7469  Title('Interacti
-0001a2a0: 7665 2052 656c 6178 6174 696f 6e20 5072  ve Relaxation Pr
-0001a2b0: 6f66 696c 6527 290a 0a20 2020 2020 2020  ofile')..       
-0001a2c0: 2073 656c 662e 7365 7441 7474 7269 6275   self.setAttribu
-0001a2d0: 7465 2851 7443 6f72 652e 5174 2e57 415f  te(QtCore.Qt.WA_
-0001a2e0: 4465 6c65 7465 4f6e 436c 6f73 6529 0a20  DeleteOnClose). 
-0001a2f0: 2020 2020 2020 2073 656c 662e 7365 7453         self.setS
-0001a300: 7479 6c65 5368 6565 7428 0a20 2020 2020  tyleSheet(.     
-0001a310: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
-0001a320: 2020 2020 2020 2051 4d61 696e 5769 6e64         QMainWind
-0001a330: 6f77 207b 0a20 2020 2020 2020 2020 2020  ow {.           
-0001a340: 2020 2020 2062 6163 6b67 726f 756e 642d       background-
-0001a350: 636f 6c6f 723a 2077 6869 7465 0a20 2020  color: white.   
-0001a360: 2020 2020 2020 2020 207d 0a0a 2020 2020           }..    
-0001a370: 2020 2020 2020 2020 5143 6865 636b 426f          QCheckBo
-0001a380: 7820 7b0a 2020 2020 2020 2020 2020 2020  x {.            
-0001a390: 2020 2020 7370 6163 696e 673a 2035 7078      spacing: 5px
-0001a3a0: 3b0a 2020 2020 2020 2020 2020 2020 2020  ;.              
-0001a3b0: 2020 666f 6e74 2d73 697a 653a 3135 7078    font-size:15px
-0001a3c0: 3b0a 2020 2020 2020 2020 2020 2020 7d0a  ;.            }.
-0001a3d0: 2020 2020 2020 2020 2020 2020 5153 6c69              QSli
-0001a3e0: 6465 723a 3a67 726f 6f76 653a 686f 7269  der::groove:hori
-0001a3f0: 7a6f 6e74 616c 207b 0a20 2020 2020 2020  zontal {.       
-0001a400: 2020 2020 2062 6f72 6465 723a 2031 7078       border: 1px
-0001a410: 2073 6f6c 6964 2023 6262 623b 0a20 2020   solid #bbb;.   
-0001a420: 2020 2020 2020 2020 2062 6163 6b67 726f           backgro
-0001a430: 756e 643a 2077 6869 7465 3b0a 2020 2020  und: white;.    
-0001a440: 2020 2020 2020 2020 6865 6967 6874 3a20          height: 
-0001a450: 3130 7078 3b0a 2020 2020 2020 2020 2020  10px;.          
-0001a460: 2020 626f 7264 6572 2d72 6164 6975 733a    border-radius:
-0001a470: 2034 7078 3b0a 2020 2020 2020 2020 2020   4px;.          
-0001a480: 2020 7d0a 0a20 2020 2020 2020 2020 2020    }..           
-0001a490: 2051 536c 6964 6572 3a3a 7375 622d 7061   QSlider::sub-pa
-0001a4a0: 6765 3a68 6f72 697a 6f6e 7461 6c20 7b0a  ge:horizontal {.
-0001a4b0: 2020 2020 2020 2020 2020 2020 6261 636b              back
-0001a4c0: 6772 6f75 6e64 3a20 716c 696e 6561 7267  ground: qlinearg
-0001a4d0: 7261 6469 656e 7428 7831 3a20 302c 2079  radient(x1: 0, y
-0001a4e0: 313a 2030 2c20 2020 2078 323a 2030 2c20  1: 0,    x2: 0, 
-0001a4f0: 7932 3a20 312c 0a20 2020 2020 2020 2020  y2: 1,.         
-0001a500: 2020 2020 2020 2073 746f 703a 2030 2023         stop: 0 #
-0001a510: 3636 652c 2073 746f 703a 2031 2023 6262  66e, stop: 1 #bb
-0001a520: 6629 3b0a 2020 2020 2020 2020 2020 2020  f);.            
-0001a530: 6261 636b 6772 6f75 6e64 3a20 716c 696e  background: qlin
-0001a540: 6561 7267 7261 6469 656e 7428 7831 3a20  eargradient(x1: 
-0001a550: 302c 2079 313a 2030 2e32 2c20 7832 3a20  0, y1: 0.2, x2: 
-0001a560: 312c 2079 323a 2031 2c0a 2020 2020 2020  1, y2: 1,.      
-0001a570: 2020 2020 2020 2020 2020 7374 6f70 3a20            stop: 
-0001a580: 3020 2362 6266 2c20 7374 6f70 3a20 3120  0 #bbf, stop: 1 
-0001a590: 2335 3566 293b 0a20 2020 2020 2020 2020  #55f);.         
-0001a5a0: 2020 2062 6f72 6465 723a 2031 7078 2073     border: 1px s
-0001a5b0: 6f6c 6964 2023 3737 373b 0a20 2020 2020  olid #777;.     
-0001a5c0: 2020 2020 2020 2068 6569 6768 743a 2031         height: 1
-0001a5d0: 3070 783b 0a20 2020 2020 2020 2020 2020  0px;.           
-0001a5e0: 2062 6f72 6465 722d 7261 6469 7573 3a20   border-radius: 
-0001a5f0: 3470 783b 0a20 2020 2020 2020 2020 2020  4px;.           
-0001a600: 207d 0a0a 2020 2020 2020 2020 2020 2020   }..            
-0001a610: 5153 6c69 6465 723a 3a61 6464 2d70 6167  QSlider::add-pag
-0001a620: 653a 686f 7269 7a6f 6e74 616c 207b 0a20  e:horizontal {. 
-0001a630: 2020 2020 2020 2020 2020 2062 6163 6b67             backg
-0001a640: 726f 756e 643a 2023 6666 663b 0a20 2020  round: #fff;.   
-0001a650: 2020 2020 2020 2020 2062 6f72 6465 723a           border:
-0001a660: 2031 7078 2073 6f6c 6964 2023 3737 373b   1px solid #777;
-0001a670: 0a20 2020 2020 2020 2020 2020 2068 6569  .            hei
-0001a680: 6768 743a 2031 3070 783b 0a20 2020 2020  ght: 10px;.     
-0001a690: 2020 2020 2020 2062 6f72 6465 722d 7261         border-ra
-0001a6a0: 6469 7573 3a20 3470 783b 0a20 2020 2020  dius: 4px;.     
-0001a6b0: 2020 2020 2020 207d 0a0a 2020 2020 2020         }..      
-0001a6c0: 2020 2020 2020 5153 6c69 6465 723a 3a68        QSlider::h
-0001a6d0: 616e 646c 653a 686f 7269 7a6f 6e74 616c  andle:horizontal
-0001a6e0: 207b 0a20 2020 2020 2020 2020 2020 2062   {.            b
-0001a6f0: 6163 6b67 726f 756e 643a 2071 6c69 6e65  ackground: qline
-0001a700: 6172 6772 6164 6965 6e74 2878 313a 302c  argradient(x1:0,
-0001a710: 2079 313a 302c 2078 323a 312c 2079 323a   y1:0, x2:1, y2:
-0001a720: 312c 0a20 2020 2020 2020 2020 2020 2020  1,.             
-0001a730: 2020 2073 746f 703a 3020 2365 6565 2c20     stop:0 #eee, 
-0001a740: 7374 6f70 3a31 2023 6363 6329 3b0a 2020  stop:1 #ccc);.  
-0001a750: 2020 2020 2020 2020 2020 626f 7264 6572            border
-0001a760: 3a20 3170 7820 736f 6c69 6420 2337 3737  : 1px solid #777
-0001a770: 3b0a 2020 2020 2020 2020 2020 2020 7769  ;.            wi
-0001a780: 6474 683a 2031 3370 783b 0a20 2020 2020  dth: 13px;.     
-0001a790: 2020 2020 2020 206d 6172 6769 6e2d 746f         margin-to
-0001a7a0: 703a 202d 3270 783b 0a20 2020 2020 2020  p: -2px;.       
-0001a7b0: 2020 2020 206d 6172 6769 6e2d 626f 7474       margin-bott
-0001a7c0: 6f6d 3a20 2d32 7078 3b0a 2020 2020 2020  om: -2px;.      
-0001a7d0: 2020 2020 2020 626f 7264 6572 2d72 6164        border-rad
-0001a7e0: 6975 733a 2034 7078 3b0a 2020 2020 2020  ius: 4px;.      
-0001a7f0: 2020 2020 2020 7d0a 0a20 2020 2020 2020        }..       
-0001a800: 2020 2020 2051 536c 6964 6572 3a3a 6861       QSlider::ha
-0001a810: 6e64 6c65 3a68 6f72 697a 6f6e 7461 6c3a  ndle:horizontal:
-0001a820: 686f 7665 7220 7b0a 2020 2020 2020 2020  hover {.        
-0001a830: 2020 2020 6261 636b 6772 6f75 6e64 3a20      background: 
-0001a840: 716c 696e 6561 7267 7261 6469 656e 7428  qlineargradient(
-0001a850: 7831 3a30 2c20 7931 3a30 2c20 7832 3a31  x1:0, y1:0, x2:1
-0001a860: 2c20 7932 3a31 2c0a 2020 2020 2020 2020  , y2:1,.        
-0001a870: 2020 2020 2020 2020 7374 6f70 3a30 2023          stop:0 #
-0001a880: 6666 662c 2073 746f 703a 3120 2364 6464  fff, stop:1 #ddd
-0001a890: 293b 0a20 2020 2020 2020 2020 2020 2062  );.            b
-0001a8a0: 6f72 6465 723a 2031 7078 2073 6f6c 6964  order: 1px solid
-0001a8b0: 2023 3434 343b 0a20 2020 2020 2020 2020   #444;.         
-0001a8c0: 2020 2062 6f72 6465 722d 7261 6469 7573     border-radius
-0001a8d0: 3a20 3470 783b 0a20 2020 2020 2020 2020  : 4px;.         
-0001a8e0: 2020 207d 0a0a 2020 2020 2020 2020 2020     }..          
-0001a8f0: 2020 5153 6c69 6465 723a 3a73 7562 2d70    QSlider::sub-p
-0001a900: 6167 653a 686f 7269 7a6f 6e74 616c 3a64  age:horizontal:d
-0001a910: 6973 6162 6c65 6420 7b0a 2020 2020 2020  isabled {.      
-0001a920: 2020 2020 2020 6261 636b 6772 6f75 6e64        background
-0001a930: 3a20 2362 6262 3b0a 2020 2020 2020 2020  : #bbb;.        
-0001a940: 2020 2020 626f 7264 6572 2d63 6f6c 6f72      border-color
-0001a950: 3a20 2339 3939 3b0a 2020 2020 2020 2020  : #999;.        
-0001a960: 2020 2020 7d0a 0a20 2020 2020 2020 2020      }..         
-0001a970: 2020 2051 536c 6964 6572 3a3a 6164 642d     QSlider::add-
-0001a980: 7061 6765 3a68 6f72 697a 6f6e 7461 6c3a  page:horizontal:
-0001a990: 6469 7361 626c 6564 207b 0a20 2020 2020  disabled {.     
-0001a9a0: 2020 2020 2020 2062 6163 6b67 726f 756e         backgroun
-0001a9b0: 643a 2023 6565 653b 0a20 2020 2020 2020  d: #eee;.       
-0001a9c0: 2020 2020 2062 6f72 6465 722d 636f 6c6f       border-colo
-0001a9d0: 723a 2023 3939 393b 0a20 2020 2020 2020  r: #999;.       
-0001a9e0: 2020 2020 207d 0a0a 2020 2020 2020 2020       }..        
-0001a9f0: 2020 2020 5153 6c69 6465 723a 3a68 616e      QSlider::han
-0001aa00: 646c 653a 686f 7269 7a6f 6e74 616c 3a64  dle:horizontal:d
-0001aa10: 6973 6162 6c65 6420 7b0a 2020 2020 2020  isabled {.      
-0001aa20: 2020 2020 2020 6261 636b 6772 6f75 6e64        background
-0001aa30: 3a20 2365 6565 3b0a 2020 2020 2020 2020  : #eee;.        
-0001aa40: 2020 2020 626f 7264 6572 3a20 3170 7820      border: 1px 
-0001aa50: 736f 6c69 6420 2361 6161 3b0a 2020 2020  solid #aaa;.    
-0001aa60: 2020 2020 2020 2020 626f 7264 6572 2d72          border-r
-0001aa70: 6164 6975 733a 2034 7078 3b0a 2020 2020  adius: 4px;.    
-0001aa80: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-0001aa90: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
-0001aaa0: 2020 290a 0a20 2020 2020 2020 2023 2053    )..        # S
-0001aab0: 6574 2064 6566 6175 6c74 206d 696e 2c20  et default min, 
-0001aac0: 6d61 782c 2069 6e69 742c 2061 6e64 2073  max, init, and s
-0001aad0: 7465 7020 7661 6c75 6573 206f 6620 736c  tep values of sl
-0001aae0: 6964 6572 7320 616e 6420 7465 7874 2062  iders and text b
-0001aaf0: 6f78 6573 0a20 2020 2020 2020 2073 656c  oxes.        sel
-0001ab00: 662e 6465 6661 756c 7473 203d 2077 6964  f.defaults = wid
-0001ab10: 6765 745f 6465 6661 756c 7473 0a0a 2020  get_defaults..  
-0001ab20: 2020 2020 2020 2320 4469 6374 696f 6e61        # Dictiona
-0001ab30: 7279 2066 6f72 2074 6963 6b62 6f78 2077  ry for tickbox w
-0001ab40: 6964 6765 7473 0a20 2020 2020 2020 2073  idgets.        s
-0001ab50: 656c 662e 7469 636b 6469 6374 203d 207b  elf.tickdict = {
-0001ab60: 0a20 2020 2020 2020 2020 2020 206d 6f64  .            mod
-0001ab70: 656c 2e4e 414d 452e 6c6f 7765 7228 293a  el.NAME.lower():
-0001ab80: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
-0001ab90: 2020 666f 7220 6d6f 6465 6c20 696e 2073    for model in s
-0001aba0: 7570 706f 7274 6564 5f6d 6f64 656c 730a  upported_models.
-0001abb0: 2020 2020 2020 2020 7d0a 0a20 2020 2020          }..     
-0001abc0: 2020 2023 2044 6963 7469 6f6e 6172 7920     # Dictionary 
-0001abd0: 666f 7220 7061 7261 6d65 7465 7220 736c  for parameter sl
-0001abe0: 6964 6572 2c20 656e 7472 792c 2061 6e64  ider, entry, and
-0001abf0: 2066 6974 6669 7820 7769 6467 6574 730a   fitfix widgets.
-0001ac00: 2020 2020 2020 2020 7365 6c66 2e77 6964          self.wid
-0001ac10: 6765 7464 6963 7420 3d20 7b0a 2020 2020  getdict = {.    
-0001ac20: 2020 2020 2020 2020 6d6f 6465 6c2e 4e41          model.NA
-0001ac30: 4d45 2e6c 6f77 6572 2829 3a20 7b0a 2020  ME.lower(): {.  
-0001ac40: 2020 2020 2020 2020 2020 2020 2020 7061                pa
-0001ac50: 726e 616d 653a 207b 0a20 2020 2020 2020  rname: {.       
-0001ac60: 2020 2020 2020 2020 2020 2020 2027 736c               'sl
-0001ac70: 6964 6572 273a 204e 6f6e 652c 0a20 2020  ider': None,.   
-0001ac80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ac90: 2027 6666 5f74 6f67 676c 6527 3a20 4e6f   'ff_toggle': No
-0001aca0: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
-0001acb0: 2020 2020 2020 2020 2765 6e74 7279 273a          'entry':
-0001acc0: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
-0001acd0: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-0001ace0: 2020 2020 2020 2020 666f 7220 7061 726e          for parn
-0001acf0: 616d 6520 696e 206d 6f64 656c 2e50 4152  ame in model.PAR
-0001ad00: 4e41 4d45 530a 2020 2020 2020 2020 2020  NAMES.          
-0001ad10: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
-0001ad20: 666f 7220 6d6f 6465 6c20 696e 2073 7570  for model in sup
-0001ad30: 706f 7274 6564 5f6d 6f64 656c 730a 2020  ported_models.  
-0001ad40: 2020 2020 2020 7d0a 0a20 2020 2020 2020        }..       
-0001ad50: 2023 204d 696e 696d 756d 2057 696e 646f   # Minimum Windo
-0001ad60: 7720 7369 7a65 0a20 2020 2020 2020 2073  w size.        s
-0001ad70: 656c 662e 7365 744d 696e 696d 756d 5369  elf.setMinimumSi
-0001ad80: 7a65 2851 7443 6f72 652e 5153 697a 6528  ze(QtCore.QSize(
-0001ad90: 3132 3030 2c20 3730 3029 290a 0a20 2020  1200, 700))..   
-0001ada0: 2020 2020 2023 204d 616b 6520 7769 6467       # Make widg
-0001adb0: 6574 7320 666f 7220 656e 7469 7265 2077  ets for entire w
-0001adc0: 696e 646f 770a 2020 2020 2020 2020 7365  indow.        se
-0001add0: 6c66 2e77 6964 6765 7420 3d20 5174 5769  lf.widget = QtWi
-0001ade0: 6467 6574 732e 5157 6964 6765 7428 7061  dgets.QWidget(pa
-0001adf0: 7265 6e74 3d73 656c 6629 0a20 2020 2020  rent=self).     
-0001ae00: 2020 2073 656c 662e 7365 7443 656e 7472     self.setCentr
-0001ae10: 616c 5769 6467 6574 2873 656c 662e 7769  alWidget(self.wi
-0001ae20: 6467 6574 290a 2020 2020 2020 2020 626f  dget).        bo
-0001ae30: 745f 726f 775f 7769 6467 6574 203d 2051  t_row_widget = Q
-0001ae40: 7457 6964 6765 7473 2e51 5769 6467 6574  tWidgets.QWidget
-0001ae50: 2873 656c 662e 7769 6467 6574 290a 2020  (self.widget).  
-0001ae60: 2020 2020 2020 746f 705f 726f 775f 7769        top_row_wi
-0001ae70: 6467 6574 203d 2051 7457 6964 6765 7473  dget = QtWidgets
-0001ae80: 2e51 5769 6467 6574 2873 656c 662e 7769  .QWidget(self.wi
-0001ae90: 6467 6574 290a 2020 2020 2020 2020 7268  dget).        rh
-0001aea0: 735f 636f 6c5f 7769 6467 6574 203d 2051  s_col_widget = Q
-0001aeb0: 7457 6964 6765 7473 2e51 5769 6467 6574  tWidgets.QWidget
-0001aec0: 2874 6f70 5f72 6f77 5f77 6964 6765 7429  (top_row_widget)
-0001aed0: 0a0a 2020 2020 2020 2020 7268 735f 636f  ..        rhs_co
-0001aee0: 6c5f 7363 726f 6c6c 203d 2051 7457 6964  l_scroll = QtWid
-0001aef0: 6765 7473 2e51 5363 726f 6c6c 4172 6561  gets.QScrollArea
-0001af00: 2872 6873 5f63 6f6c 5f77 6964 6765 7429  (rhs_col_widget)
-0001af10: 0a20 2020 2020 2020 2072 6873 5f63 6f6c  .        rhs_col
-0001af20: 5f73 6372 6f6c 6c2e 7365 7456 6572 7469  _scroll.setVerti
-0001af30: 6361 6c53 6372 6f6c 6c42 6172 506f 6c69  calScrollBarPoli
-0001af40: 6379 280a 2020 2020 2020 2020 2020 2020  cy(.            
-0001af50: 5174 436f 7265 2e51 742e 5363 726f 6c6c  QtCore.Qt.Scroll
-0001af60: 4261 7241 6c77 6179 734f 6e0a 2020 2020  BarAlwaysOn.    
-0001af70: 2020 2020 290a 2020 2020 2020 2020 7268      ).        rh
-0001af80: 735f 636f 6c5f 7363 726f 6c6c 2e73 6574  s_col_scroll.set
-0001af90: 486f 7269 7a6f 6e74 616c 5363 726f 6c6c  HorizontalScroll
-0001afa0: 4261 7250 6f6c 6963 7928 0a20 2020 2020  BarPolicy(.     
-0001afb0: 2020 2020 2020 2051 7443 6f72 652e 5174         QtCore.Qt
-0001afc0: 2e53 6372 6f6c 6c42 6172 416c 7761 7973  .ScrollBarAlways
-0001afd0: 4f66 660a 2020 2020 2020 2020 290a 2020  Off.        ).  
-0001afe0: 2020 2020 2020 7268 735f 636f 6c5f 7363        rhs_col_sc
-0001aff0: 726f 6c6c 2e73 6574 5769 6467 6574 5265  roll.setWidgetRe
-0001b000: 7369 7a61 626c 6528 5472 7565 290a 0a20  sizable(True).. 
-0001b010: 2020 2020 2020 2073 6372 6f6c 6c5f 636f         scroll_co
-0001b020: 6e74 6169 6e65 7220 3d20 5174 5769 6467  ntainer = QtWidg
-0001b030: 6574 732e 5157 6964 6765 7428 7268 735f  ets.QWidget(rhs_
-0001b040: 636f 6c5f 7363 726f 6c6c 290a 2020 2020  col_scroll).    
-0001b050: 2020 2020 7268 735f 636f 6c5f 7363 726f      rhs_col_scro
-0001b060: 6c6c 2e73 6574 5769 6467 6574 2873 6372  ll.setWidget(scr
-0001b070: 6f6c 6c5f 636f 6e74 6169 6e65 7229 0a0a  oll_container)..
-0001b080: 2020 2020 2020 2020 6c68 735f 636f 6c5f          lhs_col_
-0001b090: 7769 6467 6574 203d 2051 7457 6964 6765  widget = QtWidge
-0001b0a0: 7473 2e51 5769 6467 6574 2874 6f70 5f72  ts.QWidget(top_r
-0001b0b0: 6f77 5f77 6964 6765 7429 0a0a 2020 2020  ow_widget)..    
-0001b0c0: 2020 2020 2320 4c48 5320 636f 6c75 6d6e      # LHS column
-0001b0d0: 202d 2070 6c6f 7420 6f6e 6c79 0a20 2020   - plot only.   
-0001b0e0: 2020 2020 206c 6873 5f63 6f6c 5f6c 6179       lhs_col_lay
-0001b0f0: 6f75 7420 3d20 5174 5769 6467 6574 732e  out = QtWidgets.
-0001b100: 5156 426f 784c 6179 6f75 7428 6c68 735f  QVBoxLayout(lhs_
-0001b110: 636f 6c5f 7769 6467 6574 290a 0a20 2020  col_widget)..   
-0001b120: 2020 2020 2023 206d 616b 6520 7067 6670       # make pgfp
-0001b130: 6c6f 7473 2070 6c6f 7420 7769 6467 6574  lots plot widget
-0001b140: 0a20 2020 2020 2020 2073 656c 662e 706c  .        self.pl
-0001b150: 6f74 5f77 6964 6765 7420 3d20 7067 2e50  ot_widget = pg.P
-0001b160: 6c6f 7457 6964 6765 7428 0a20 2020 2020  lotWidget(.     
-0001b170: 2020 2020 2020 2070 6172 656e 743d 6c68         parent=lh
-0001b180: 735f 636f 6c5f 7769 6467 6574 0a20 2020  s_col_widget.   
-0001b190: 2020 2020 2029 0a20 2020 2020 2020 2023       ).        #
-0001b1a0: 2041 6464 2070 6c6f 7420 746f 206c 6566   Add plot to lef
-0001b1b0: 7420 636f 6c75 6d6e 0a20 2020 2020 2020  t column.       
-0001b1c0: 206c 6873 5f63 6f6c 5f6c 6179 6f75 742e   lhs_col_layout.
-0001b1d0: 6164 6457 6964 6765 7428 7365 6c66 2e70  addWidget(self.p
-0001b1e0: 6c6f 745f 7769 6467 6574 290a 0a20 2020  lot_widget)..   
-0001b1f0: 2020 2020 2023 2053 6574 206c 6f67 6c6f       # Set loglo
-0001b200: 6720 6178 6573 0a20 2020 2020 2020 2073  g axes.        s
-0001b210: 656c 662e 706c 6f74 5f77 6964 6765 742e  elf.plot_widget.
-0001b220: 7365 744c 6f67 4d6f 6465 2854 7275 652c  setLogMode(True,
-0001b230: 2054 7275 6529 0a0a 2020 2020 2020 2020   True)..        
-0001b240: 2320 5365 7420 7768 6974 6520 706c 6f74  # Set white plot
-0001b250: 2062 6163 6b67 726f 756e 640a 2020 2020   background.    
-0001b260: 2020 2020 7365 6c66 2e70 6c6f 745f 7769      self.plot_wi
-0001b270: 6467 6574 2e73 6574 4261 636b 6772 6f75  dget.setBackgrou
-0001b280: 6e64 2827 7727 290a 0a20 2020 2020 2020  nd('w')..       
-0001b290: 2023 2053 656c 6563 7420 6569 7468 6572   # Select either
-0001b2a0: 2066 6965 6c64 206f 7220 7465 6d70 6572   field or temper
-0001b2b0: 6174 7572 6520 6173 2078 2064 6174 6120  ature as x data 
-0001b2c0: 6261 7365 6420 6f6e 2064 6174 6173 6574  based on dataset
-0001b2d0: 2074 7970 650a 2020 2020 2020 2020 2320   type.        # 
-0001b2e0: 616e 6420 7365 7420 7820 6c61 6265 6c20  and set x label 
-0001b2f0: 6f66 2070 6c6f 740a 2020 2020 2020 2020  of plot.        
-0001b300: 6966 2069 7369 6e73 7461 6e63 6528 6461  if isinstance(da
-0001b310: 7461 7365 742c 2054 6175 4844 6174 6173  taset, TauHDatas
-0001b320: 6574 293a 0a20 2020 2020 2020 2020 2020  et):.           
-0001b330: 2078 5f76 6172 7320 3d20 6461 7461 7365   x_vars = datase
-0001b340: 742e 6669 656c 6473 0a20 2020 2020 2020  t.fields.       
-0001b350: 2020 2020 2073 656c 662e 706c 6f74 5f77       self.plot_w
-0001b360: 6964 6765 742e 7365 744c 6162 656c 2827  idget.setLabel('
-0001b370: 626f 7474 6f6d 272c 2027 4669 656c 6420  bottom', 'Field 
-0001b380: 284f 6529 2729 0a0a 2020 2020 2020 2020  (Oe)')..        
-0001b390: 656c 6966 2069 7369 6e73 7461 6e63 6528  elif isinstance(
-0001b3a0: 6461 7461 7365 742c 2054 6175 5444 6174  dataset, TauTDat
-0001b3b0: 6173 6574 293a 0a20 2020 2020 2020 2020  aset):.         
-0001b3c0: 2020 2078 5f76 6172 7320 3d20 6461 7461     x_vars = data
-0001b3d0: 7365 742e 7465 6d70 6572 6174 7572 6573  set.temperatures
-0001b3e0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0001b3f0: 662e 706c 6f74 5f77 6964 6765 742e 7365  f.plot_widget.se
-0001b400: 744c 6162 656c 2827 626f 7474 6f6d 272c  tLabel('bottom',
-0001b410: 2027 5465 6d70 6572 6174 7572 6520 284b   'Temperature (K
-0001b420: 2927 290a 0a20 2020 2020 2020 2023 2045  )')..        # E
-0001b430: 7870 6572 696d 656e 7461 6c20 6461 7461  xperimental data
-0001b440: 0a20 2020 2020 2020 2073 656c 662e 6578  .        self.ex
-0001b450: 7020 3d20 7365 6c66 2e70 6c6f 745f 7769  p = self.plot_wi
-0001b460: 6467 6574 2e70 6c6f 7428 0a20 2020 2020  dget.plot(.     
-0001b470: 2020 2020 2020 206e 702e 6172 7261 7928         np.array(
-0001b480: 785f 7661 7273 292c 0a20 2020 2020 2020  x_vars),.       
-0001b490: 2020 2020 206e 702e 6172 7261 7928 6461       np.array(da
-0001b4a0: 7461 7365 742e 7261 7465 7329 2c0a 2020  taset.rates),.  
-0001b4b0: 2020 2020 2020 2020 2020 7065 6e3d 4e6f            pen=No
-0001b4c0: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
-0001b4d0: 7379 6d62 6f6c 3d27 7827 2c0a 2020 2020  symbol='x',.    
-0001b4e0: 2020 2020 2020 2020 7379 6d62 6f6c 4272          symbolBr
-0001b4f0: 7573 683d 2830 2c20 302c 2030 290a 2020  ush=(0, 0, 0).  
-0001b500: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-0001b510: 2023 2046 696e 6420 6e69 6365 2079 2d61   # Find nice y-a
-0001b520: 7869 7320 6c69 6d69 7473 0a20 2020 2020  xis limits.     
-0001b530: 2020 2079 5f6c 6f77 6572 2c20 795f 7570     y_lower, y_up
-0001b540: 7065 7220 3d20 6775 692e 6361 6c63 5f79  per = gui.calc_y
-0001b550: 5f72 6174 655f 6c69 6d73 280a 2020 2020  _rate_lims(.    
-0001b560: 2020 2020 2020 2020 6461 7461 7365 742e          dataset.
-0001b570: 7261 7465 732c 0a20 2020 2020 2020 2020  rates,.         
-0001b580: 2020 206e 702e 6172 7261 7928 6461 7461     np.array(data
-0001b590: 7365 742e 7261 7465 5f70 6d29 0a20 2020  set.rate_pm).   
-0001b5a0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-0001b5b0: 2320 436c 6970 2074 6865 6d20 6174 2073  # Clip them at s
-0001b5c0: 656e 7369 626c 6520 7661 6c75 6573 0a20  ensible values. 
-0001b5d0: 2020 2020 2020 205b 795f 6c6f 7765 722c         [y_lower,
-0001b5e0: 2079 5f75 7070 6572 5d20 3d20 6e70 2e63   y_upper] = np.c
-0001b5f0: 6c69 7028 5b79 5f6c 6f77 6572 2c20 795f  lip([y_lower, y_
-0001b600: 7570 7065 725d 2c20 3145 2d31 302c 2031  upper], 1E-10, 1
-0001b610: 4531 3029 0a0a 2020 2020 2020 2020 2320  E10)..        # 
-0001b620: 616e 6420 7365 7420 7661 6c75 6573 0a20  and set values. 
-0001b630: 2020 2020 2020 2073 656c 662e 706c 6f74         self.plot
-0001b640: 5f77 6964 6765 742e 7365 7459 5261 6e67  _widget.setYRang
-0001b650: 6528 0a20 2020 2020 2020 2020 2020 206e  e(.            n
-0001b660: 702e 6c6f 6731 3028 795f 6c6f 7765 7229  p.log10(y_lower)
-0001b670: 2c0a 2020 2020 2020 2020 2020 2020 6e70  ,.            np
-0001b680: 2e6c 6f67 3130 2879 5f75 7070 6572 292c  .log10(y_upper),
-0001b690: 0a20 2020 2020 2020 2020 2020 2070 6164  .            pad
-0001b6a0: 6469 6e67 3d30 0a20 2020 2020 2020 2029  ding=0.        )
-0001b6b0: 0a0a 2020 2020 2020 2020 2320 4164 6420  ..        # Add 
-0001b6c0: 6578 7065 7269 6d65 6e74 616c 2065 7272  experimental err
-0001b6d0: 6f72 6261 7273 0a20 2020 2020 2020 2069  orbars.        i
-0001b6e0: 6620 6c65 6e28 6461 7461 7365 742e 6c6f  f len(dataset.lo
-0001b6f0: 6772 6174 655f 706d 293a 0a20 2020 2020  grate_pm):.     
-0001b700: 2020 2020 2020 2065 7272 203d 2070 672e         err = pg.
-0001b710: 4572 726f 7242 6172 4974 656d 280a 2020  ErrorBarItem(.  
-0001b720: 2020 2020 2020 2020 2020 2020 2020 783d                x=
-0001b730: 6e70 2e6c 6f67 3130 2878 5f76 6172 7329  np.log10(x_vars)
-0001b740: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0001b750: 2020 793d 6e70 2e6c 6f67 3130 2864 6174    y=np.log10(dat
-0001b760: 6173 6574 2e72 6174 6573 292c 0a20 2020  aset.rates),.   
-0001b770: 2020 2020 2020 2020 2020 2020 2074 6f70               top
-0001b780: 3d64 6174 6173 6574 2e6c 6f67 7261 7465  =dataset.lograte
-0001b790: 5f70 6d2c 0a20 2020 2020 2020 2020 2020  _pm,.           
-0001b7a0: 2020 2020 2062 6f74 746f 6d3d 6461 7461       bottom=data
-0001b7b0: 7365 742e 6c6f 6772 6174 655f 706d 2c0a  set.lograte_pm,.
-0001b7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b7d0: 6265 616d 3d30 2e30 3035 0a20 2020 2020  beam=0.005.     
-0001b7e0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0001b7f0: 2020 2020 2073 656c 662e 706c 6f74 5f77       self.plot_w
-0001b800: 6964 6765 742e 6164 6449 7465 6d28 6572  idget.addItem(er
-0001b810: 7229 0a0a 2020 2020 2020 2020 2320 4178  r)..        # Ax
-0001b820: 6973 206c 6162 656c 730a 2020 2020 2020  is labels.      
-0001b830: 2020 7365 6c66 2e70 6c6f 745f 7769 6467    self.plot_widg
-0001b840: 6574 2e73 6574 4c61 6265 6c28 276c 6566  et.setLabel('lef
-0001b850: 7427 2c20 2752 6174 6520 2873 3c73 7570  t', 'Rate (s<sup
-0001b860: 3e2d 313c 2f73 7570 3e29 2729 0a0a 2020  >-1</sup>)')..  
-0001b870: 2020 2020 2020 2320 5365 7420 6469 6374        # Set dict
-0001b880: 696f 6e61 7279 206f 6620 5472 7565 2028  ionary of True (
-0001b890: 6669 7429 2061 6e64 2046 616c 7365 2028  fit) and False (
-0001b8a0: 6669 7829 2066 6f72 2065 6163 680a 2020  fix) for each.  
-0001b8b0: 2020 2020 2020 2320 7061 7261 6d65 7465        # paramete
-0001b8c0: 7220 6f66 2061 6c6c 2061 7661 696c 6162  r of all availab
-0001b8d0: 6c65 206d 6f64 656c 730a 2020 2020 2020  le models.      
-0001b8e0: 2020 7573 656c 2e66 6974 203d 207b 0a20    usel.fit = {. 
-0001b8f0: 2020 2020 2020 2020 2020 2070 6172 6e61             parna
-0001b900: 6d65 3a20 5472 7565 0a20 2020 2020 2020  me: True.       
-0001b910: 2020 2020 2066 6f72 206d 6f64 656c 2069       for model i
-0001b920: 6e20 7375 7070 6f72 7465 645f 6d6f 6465  n supported_mode
-0001b930: 6c73 0a20 2020 2020 2020 2020 2020 2066  ls.            f
-0001b940: 6f72 2070 6172 6e61 6d65 2069 6e20 6d6f  or parname in mo
-0001b950: 6465 6c2e 5041 524e 414d 4553 0a20 2020  del.PARNAMES.   
-0001b960: 2020 2020 207d 0a0a 2020 2020 2020 2020       }..        
-0001b970: 2320 5365 7420 7573 6572 2073 656c 6563  # Set user selec
-0001b980: 7469 6f6e 206f 626a 6563 7420 616e 6420  tion object and 
-0001b990: 7375 7070 6f72 7465 6420 6d6f 6465 6c73  supported models
-0001b9a0: 0a20 2020 2020 2020 2073 656c 662e 7573  .        self.us
-0001b9b0: 656c 203d 2075 7365 6c0a 2020 2020 2020  el = usel.      
-0001b9c0: 2020 7365 6c66 2e73 7570 706f 7274 6564    self.supported
-0001b9d0: 5f6d 6f64 656c 7320 3d20 7375 7070 6f72  _models = suppor
-0001b9e0: 7465 645f 6d6f 6465 6c73 0a0a 2020 2020  ted_models..    
-0001b9f0: 2020 2020 2320 4361 6c63 756c 6174 6520      # Calculate 
-0001ba00: 6561 6368 206d 6f64 656c 2066 756e 6374  each model funct
-0001ba10: 696f 6e20 616e 6420 706c 6f74 0a20 2020  ion and plot.   
-0001ba20: 2020 2020 2073 656c 662e 7465 6d70 5f67       self.temp_g
-0001ba30: 7269 6420 3d20 6e70 2e6c 696e 7370 6163  rid = np.linspac
-0001ba40: 6528 0a20 2020 2020 2020 2020 2020 206e  e(.            n
-0001ba50: 702e 6d69 6e28 785f 7661 7273 292c 206e  p.min(x_vars), n
-0001ba60: 702e 6d61 7828 785f 7661 7273 292c 2031  p.max(x_vars), 1
-0001ba70: 3030 300a 2020 2020 2020 2020 290a 0a20  000.        ).. 
-0001ba80: 2020 2020 2020 2023 2053 756d 206f 6620         # Sum of 
-0001ba90: 616c 6c20 6d6f 6465 6c73 2c20 7365 7420  all models, set 
-0001baa0: 746f 207a 6572 6f20 696e 6974 6961 6c6c  to zero initiall
-0001bab0: 790a 2020 2020 2020 2020 746f 7461 6c5f  y.        total_
-0001bac0: 7261 7465 7320 3d20 6e70 2e7a 6572 6f73  rates = np.zeros
-0001bad0: 286e 702e 7368 6170 6528 7365 6c66 2e74  (np.shape(self.t
-0001bae0: 656d 705f 6772 6964 2929 0a0a 2020 2020  emp_grid))..    
-0001baf0: 2020 2020 2320 4469 6374 696f 6e61 7279      # Dictionary
-0001bb00: 206f 6620 706c 6f74 730a 2020 2020 2020   of plots.      
-0001bb10: 2020 2320 6b65 7973 2061 7265 206d 6f64    # keys are mod
-0001bb20: 656c 2e4e 414d 452e 6c6f 7765 7228 292c  el.NAME.lower(),
-0001bb30: 2076 616c 7565 7320 6172 6520 706c 6f74   values are plot
-0001bb40: 5f77 6964 6765 742e 706c 6f74 0a20 2020  _widget.plot.   
-0001bb50: 2020 2020 2073 656c 662e 6d6f 6465 6c5f       self.model_
-0001bb60: 706c 6f74 7320 3d20 7b7d 0a0a 2020 2020  plots = {}..    
-0001bb70: 2020 2020 2320 4c69 7374 206f 6620 6e69      # List of ni
-0001bb80: 6365 2063 6f6c 6f72 730a 2020 2020 2020  ce colors.      
-0001bb90: 2020 636f 6c6f 7273 203d 206d 636f 6c6f    colors = mcolo
-0001bba0: 7273 2e54 4142 4c45 4155 5f43 4f4c 4f52  rs.TABLEAU_COLOR
-0001bbb0: 532e 7661 6c75 6573 2829 0a0a 2020 2020  S.values()..    
-0001bbc0: 2020 2020 2320 4c6f 6f70 206f 7665 7220      # Loop over 
-0001bbd0: 616c 6c20 706f 7373 6962 6c65 206d 6f64  all possible mod
-0001bbe0: 656c 732c 2063 616c 6375 6c61 7465 206d  els, calculate m
-0001bbf0: 6f64 656c 2076 616c 7565 730a 2020 2020  odel values.    
-0001bc00: 2020 2020 2320 6174 2072 616e 6765 206f      # at range o
-0001bc10: 6620 7465 6d70 6572 6174 7572 6573 2061  f temperatures a
-0001bc20: 6e64 2070 6c6f 740a 2020 2020 2020 2020  nd plot.        
-0001bc30: 2320 7468 656e 2061 6464 2074 6f20 6172  # then add to ar
-0001bc40: 7261 7920 6f66 2074 6f74 616c 2072 6174  ray of total rat
-0001bc50: 6573 0a20 2020 2020 2020 2066 6f72 2063  es.        for c
-0001bc60: 6f6c 6f72 2c20 6d6f 6465 6c20 696e 207a  olor, model in z
-0001bc70: 6970 2863 6f6c 6f72 732c 2073 7570 706f  ip(colors, suppo
-0001bc80: 7274 6564 5f6d 6f64 656c 7329 3a0a 0a20  rted_models):.. 
-0001bc90: 2020 2020 2020 2020 2020 2023 2047 6574             # Get
-0001bca0: 2069 6e69 7469 616c 2076 616c 7565 730a   initial values.
-0001bcb0: 2020 2020 2020 2020 2020 2020 696e 6974              init
-0001bcc0: 6961 6c73 203d 206d 6f64 656c 2e73 6574  ials = model.set
-0001bcd0: 5f69 6e69 7469 616c 5f76 616c 7328 0a20  _initial_vals(. 
-0001bce0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-0001bcf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001bd00: 2020 2020 2070 6172 3a20 7365 6c66 2e64       par: self.d
-0001bd10: 6566 6175 6c74 735b 6d6f 6465 6c2e 4e41  efaults[model.NA
-0001bd20: 4d45 5d5b 7061 725d 5b27 7661 6c69 6e69  ME][par]['valini
-0001bd30: 7427 5d0a 2020 2020 2020 2020 2020 2020  t'].            
-0001bd40: 2020 2020 2020 2020 666f 7220 7061 7220          for par 
-0001bd50: 696e 206d 6f64 656c 2e50 4152 4e41 4d45  in model.PARNAME
-0001bd60: 530a 2020 2020 2020 2020 2020 2020 2020  S.              
-0001bd70: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
-0001bd80: 290a 2020 2020 2020 2020 2020 2020 2320  ).            # 
-0001bd90: 4361 6c63 756c 6174 6520 7261 7465 730a  Calculate rates.
-0001bda0: 2020 2020 2020 2020 2020 2020 7261 7465              rate
-0001bdb0: 7320 3d20 3130 2a2a 286d 6f64 656c 2e6d  s = 10**(model.m
-0001bdc0: 6f64 656c 2869 6e69 7469 616c 732c 2073  odel(initials, s
-0001bdd0: 656c 662e 7465 6d70 5f67 7269 6429 290a  elf.temp_grid)).
-0001bde0: 2020 2020 2020 2020 2020 2020 2320 616e              # an
-0001bdf0: 6420 6164 6420 746f 2074 6f74 616c 206f  d add to total o
-0001be00: 6620 616c 6c20 6d6f 6465 6c73 0a20 2020  f all models.   
-0001be10: 2020 2020 2020 2020 2074 6f74 616c 5f72           total_r
-0001be20: 6174 6573 202b 3d20 7261 7465 730a 2020  ates += rates.  
-0001be30: 2020 2020 2020 2020 2020 2320 506c 6f74            # Plot
-0001be40: 2074 6869 7320 6d6f 6465 6c0a 2020 2020   this model.    
-0001be50: 2020 2020 2020 2020 5f70 6c6f 7420 3d20          _plot = 
-0001be60: 7365 6c66 2e70 6c6f 745f 7769 6467 6574  self.plot_widget
-0001be70: 2e70 6c6f 7428 0a20 2020 2020 2020 2020  .plot(.         
-0001be80: 2020 2020 2020 2073 656c 662e 7465 6d70         self.temp
-0001be90: 5f67 7269 642c 0a20 2020 2020 2020 2020  _grid,.         
-0001bea0: 2020 2020 2020 2072 6174 6573 2c0a 2020         rates,.  
-0001beb0: 2020 2020 2020 2020 2020 2020 2020 7065                pe
-0001bec0: 6e3d 7b27 7769 6474 6827 3a20 322e 352c  n={'width': 2.5,
-0001bed0: 2027 636f 6c6f 7227 3a20 636f 6c6f 722c   'color': color,
-0001bee0: 2027 7374 796c 6527 3a20 5174 436f 7265   'style': QtCore
-0001bef0: 2e51 742e 4461 7368 4c69 6e65 7d0a 2020  .Qt.DashLine}.  
-0001bf00: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0001bf10: 2020 2020 2020 2020 2320 616e 6420 7374          # and st
-0001bf20: 6f72 6520 696e 2064 6963 7420 6f66 2061  ore in dict of a
-0001bf30: 6c6c 2070 6c6f 7473 0a20 2020 2020 2020  ll plots.       
-0001bf40: 2020 2020 2073 656c 662e 6d6f 6465 6c5f       self.model_
-0001bf50: 706c 6f74 735b 6d6f 6465 6c2e 4e41 4d45  plots[model.NAME
-0001bf60: 2e6c 6f77 6572 2829 5d20 3d20 5f70 6c6f  .lower()] = _plo
-0001bf70: 740a 2020 2020 2020 2020 2020 2020 2320  t.            # 
-0001bf80: 5265 6d6f 7665 2066 726f 6d20 6163 7475  Remove from actu
-0001bf90: 616c 2070 6c6f 7420 7769 6467 6574 0a20  al plot widget. 
-0001bfa0: 2020 2020 2020 2020 2020 2023 2073 696e             # sin
-0001bfb0: 6365 206e 6f20 6d6f 6465 6c73 2061 7265  ce no models are
-0001bfc0: 2076 6973 6962 6c65 2069 6e69 7469 616c   visible initial
-0001bfd0: 6c79 0a20 2020 2020 2020 2020 2020 2023  ly.            #
-0001bfe0: 2050 6c6f 7473 2061 7265 2072 652d 6164   Plots are re-ad
-0001bff0: 6465 6420 7769 7468 206d 6f64 656c 2063  ded with model c
-0001c000: 6865 636b 626f 7865 730a 2020 2020 2020  heckboxes.      
-0001c010: 2020 2020 2020 7365 6c66 2e70 6c6f 745f        self.plot_
-0001c020: 7769 6467 6574 2e72 656d 6f76 6549 7465  widget.removeIte
-0001c030: 6d28 5f70 6c6f 7429 0a0a 2020 2020 2020  m(_plot)..      
-0001c040: 2020 2320 506c 6f74 2073 756d 206f 6620    # Plot sum of 
-0001c050: 616c 6c20 6d6f 6465 6c73 0a20 2020 2020  all models.     
-0001c060: 2020 2073 656c 662e 746f 7420 3d20 7365     self.tot = se
-0001c070: 6c66 2e70 6c6f 745f 7769 6467 6574 2e70  lf.plot_widget.p
-0001c080: 6c6f 7428 0a20 2020 2020 2020 2020 2020  lot(.           
-0001c090: 2073 656c 662e 7465 6d70 5f67 7269 642c   self.temp_grid,
-0001c0a0: 0a20 2020 2020 2020 2020 2020 2074 6f74  .            tot
-0001c0b0: 616c 5f72 6174 6573 2c0a 2020 2020 2020  al_rates,.      
-0001c0c0: 2020 2020 2020 7065 6e3d 7b27 7769 6474        pen={'widt
-0001c0d0: 6827 3a20 322e 352c 2027 636f 6c6f 7227  h': 2.5, 'color'
-0001c0e0: 3a20 2772 6564 277d 0a20 2020 2020 2020  : 'red'}.       
-0001c0f0: 2029 0a20 2020 2020 2020 2073 656c 662e   ).        self.
-0001c100: 706c 6f74 5f77 6964 6765 742e 7265 6d6f  plot_widget.remo
-0001c110: 7665 4974 656d 2873 656c 662e 746f 7429  veItem(self.tot)
-0001c120: 0a0a 2020 2020 2020 2020 2320 5374 6f72  ..        # Stor
-0001c130: 6167 6520 6f62 6a65 6374 2066 6f72 2066  age object for f
-0001c140: 696e 616c 2070 6172 616d 6574 6572 2076  inal parameter v
-0001c150: 616c 7565 730a 2020 2020 2020 2020 2320  alues.        # 
-0001c160: 5365 7420 616c 6c20 696e 6974 6961 6c20  Set all initial 
-0001c170: 7661 6c75 6573 2064 6566 6175 6c74 730a  values defaults.
-0001c180: 2020 2020 2020 2020 7365 6c66 2e70 6172          self.par
-0001c190: 7374 6f72 6520 3d20 7479 7065 280a 2020  store = type(.  
-0001c1a0: 2020 2020 2020 2020 2020 276f 626a 272c            'obj',
-0001c1b0: 0a20 2020 2020 2020 2020 2020 2028 6f62  .            (ob
-0001c1c0: 6a65 6374 2c29 2c0a 2020 2020 2020 2020  ject,),.        
-0001c1d0: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
-0001c1e0: 2020 2020 2020 7061 723a 2073 656c 662e        par: self.
-0001c1f0: 6465 6661 756c 7473 5b6d 6f64 656c 2e4e  defaults[model.N
-0001c200: 414d 455d 5b70 6172 5d5b 2776 616c 696e  AME][par]['valin
-0001c210: 6974 275d 0a20 2020 2020 2020 2020 2020  it'].           
-0001c220: 2020 2020 2066 6f72 206d 6f64 656c 2069       for model i
-0001c230: 6e20 7375 7070 6f72 7465 645f 6d6f 6465  n supported_mode
-0001c240: 6c73 0a20 2020 2020 2020 2020 2020 2020  ls.             
-0001c250: 2020 2066 6f72 2070 6172 2069 6e20 6d6f     for par in mo
-0001c260: 6465 6c2e 5041 524e 414d 4553 0a20 2020  del.PARNAMES.   
-0001c270: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-0001c280: 2020 2029 0a0a 2020 2020 2020 2020 2320     )..        # 
-0001c290: 436f 6e76 6572 7420 6c6f 6720 7465 6d70  Convert log temp
-0001c2a0: 6572 6174 7572 6520 7469 636b 7320 746f  erature ticks to
-0001c2b0: 206c 696e 6561 720a 2020 2020 2020 2020   linear.        
-0001c2c0: 6178 203d 2073 656c 662e 706c 6f74 5f77  ax = self.plot_w
-0001c2d0: 6964 6765 742e 6765 7441 7869 7328 2762  idget.getAxis('b
-0001c2e0: 6f74 746f 6d27 290a 2020 2020 2020 2020  ottom').        
-0001c2f0: 6775 692e 636f 6e76 6572 745f 6c6f 675f  gui.convert_log_
-0001c300: 7469 636b 735f 746f 5f6c 696e 2861 782c  ticks_to_lin(ax,
-0001c310: 206e 702e 6c6f 6731 3028 785f 7661 7273   np.log10(x_vars
-0001c320: 2929 0a0a 2020 2020 2020 2020 2320 5248  ))..        # RH
-0001c330: 5320 636f 6c75 6d6e 206f 6620 7769 6e64  S column of wind
-0001c340: 6f77 0a20 2020 2020 2020 2023 2054 6869  ow.        # Thi
-0001c350: 7320 636f 6e74 6169 6e73 2065 6163 6820  s contains each 
-0001c360: 6d6f 6465 6c20 616e 6420 6974 7320 6173  model and its as
-0001c370: 736f 6369 6174 6564 2070 6172 616d 6574  sociated paramet
-0001c380: 6572 730a 2020 2020 2020 2020 2320 4561  ers.        # Ea
-0001c390: 6368 2070 6172 616d 6574 6572 2069 7320  ch parameter is 
-0001c3a0: 636f 6e74 726f 6c6c 6564 2062 7920 610a  controlled by a.
-0001c3b0: 2020 2020 2020 2020 2320 736c 6964 6572          # slider
-0001c3c0: 732c 2054 6578 7420 656e 7472 792c 2061  s, Text entry, a
-0001c3d0: 6e64 2061 2066 6974 2f66 6978 2074 6f67  nd a fit/fix tog
-0001c3e0: 676c 650a 2020 2020 2020 2020 636f 6e74  gle.        cont
-0001c3f0: 6169 6e65 725f 6c61 796f 7574 203d 2051  ainer_layout = Q
-0001c400: 7457 6964 6765 7473 2e51 5642 6f78 4c61  tWidgets.QVBoxLa
-0001c410: 796f 7574 2873 6372 6f6c 6c5f 636f 6e74  yout(scroll_cont
-0001c420: 6169 6e65 7229 0a0a 2020 2020 2020 2020  ainer)..        
-0001c430: 2320 4c69 7374 206f 6620 6e75 6d62 6572  # List of number
-0001c440: 206b 6579 2073 686f 7274 6375 7473 2074   key shortcuts t
-0001c450: 6f20 746f 6767 6c65 206d 6f64 656c 730a  o toggle models.
-0001c460: 2020 2020 2020 2020 7365 6c66 2e6f 6e5f          self.on_
-0001c470: 6f66 665f 7368 6f72 7463 7574 203d 205b  off_shortcut = [
-0001c480: 5d0a 0a20 2020 2020 2020 2023 2046 6f72  ]..        # For
-0001c490: 2065 6163 6820 6d6f 6465 6c2c 206d 616b   each model, mak
-0001c4a0: 6520 6120 626f 7820 746f 2063 6f6e 7461  e a box to conta
-0001c4b0: 696e 2061 6c6c 2070 6172 616d 6574 6572  in all parameter
-0001c4c0: 730a 2020 2020 2020 2020 2320 616e 6420  s.        # and 
-0001c4d0: 706f 7075 6c61 7465 2077 6974 6820 7061  populate with pa
-0001c4e0: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
-0001c4f0: 2066 6f72 206d 6974 2c20 6d6f 6465 6c20   for mit, model 
-0001c500: 696e 2065 6e75 6d65 7261 7465 2873 7570  in enumerate(sup
-0001c510: 706f 7274 6564 5f6d 6f64 656c 7329 3a0a  ported_models):.
-0001c520: 2020 2020 2020 2020 2020 2020 6d6f 6465              mode
-0001c530: 6c5f 7769 6467 6574 203d 2073 656c 662e  l_widget = self.
-0001c540: 6d61 6b65 5f6d 6f64 656c 626f 7828 6d6f  make_modelbox(mo
-0001c550: 6465 6c2c 2073 6372 6f6c 6c5f 636f 6e74  del, scroll_cont
-0001c560: 6169 6e65 722c 206d 6974 202b 2031 290a  ainer, mit + 1).
-0001c570: 0a20 2020 2020 2020 2020 2020 2023 2041  .            # A
-0001c580: 6464 2074 6869 7320 6d6f 6465 6c20 746f  dd this model to
-0001c590: 2074 6865 2072 6967 6874 2068 616e 6420   the right hand 
-0001c5a0: 7369 6465 206f 6620 7468 6520 7769 6e64  side of the wind
-0001c5b0: 6f77 0a20 2020 2020 2020 2020 2020 2063  ow.            c
-0001c5c0: 6f6e 7461 696e 6572 5f6c 6179 6f75 742e  ontainer_layout.
-0001c5d0: 6164 6457 6964 6765 7428 6d6f 6465 6c5f  addWidget(model_
-0001c5e0: 7769 6467 6574 2c20 6c65 6e28 6d6f 6465  widget, len(mode
-0001c5f0: 6c2e 5041 524e 414d 4553 2929 0a0a 2020  l.PARNAMES))..  
-0001c600: 2020 2020 2020 2320 4469 7361 626c 6520        # Disable 
-0001c610: 6576 6572 7920 736c 6964 6572 2c20 656e  every slider, en
-0001c620: 7472 792c 2061 6e64 2066 6974 2f66 6978  try, and fit/fix
-0001c630: 2062 7920 6465 6661 756c 740a 2020 2020   by default.    
-0001c640: 2020 2020 2320 5468 6973 2069 7320 746f      # This is to
-0001c650: 6767 6c65 6420 6279 2074 6865 206d 6f64  ggled by the mod
-0001c660: 656c 2063 6865 636b 626f 7865 730a 2020  el checkboxes.  
-0001c670: 2020 2020 2020 666f 7220 6d6f 6465 6c20        for model 
-0001c680: 696e 2073 7570 706f 7274 6564 5f6d 6f64  in supported_mod
-0001c690: 656c 733a 0a20 2020 2020 2020 2020 2020  els:.           
-0001c6a0: 206d 6f64 656c 6e61 6d65 203d 206d 6f64   modelname = mod
-0001c6b0: 656c 2e4e 414d 452e 6c6f 7765 7228 290a  el.NAME.lower().
-0001c6c0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0001c6d0: 7061 726e 616d 6520 696e 206d 6f64 656c  parname in model
-0001c6e0: 2e50 4152 4e41 4d45 533a 0a20 2020 2020  .PARNAMES:.     
-0001c6f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0001c700: 7769 6467 6574 6469 6374 5b6d 6f64 656c  widgetdict[model
-0001c710: 6e61 6d65 5d5b 7061 726e 616d 655d 5b27  name][parname]['
-0001c720: 736c 6964 6572 275d 2e73 6574 456e 6162  slider'].setEnab
-0001c730: 6c65 6428 4661 6c73 6529 0a20 2020 2020  led(False).     
-0001c740: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0001c750: 7769 6467 6574 6469 6374 5b6d 6f64 656c  widgetdict[model
-0001c760: 6e61 6d65 5d5b 7061 726e 616d 655d 5b27  name][parname]['
-0001c770: 656e 7472 7927 5d2e 7365 7445 6e61 626c  entry'].setEnabl
-0001c780: 6564 2846 616c 7365 290a 2020 2020 2020  ed(False).      
-0001c790: 2020 2020 2020 2020 2020 7365 6c66 2e77            self.w
-0001c7a0: 6964 6765 7464 6963 745b 6d6f 6465 6c6e  idgetdict[modeln
-0001c7b0: 616d 655d 5b70 6172 6e61 6d65 5d5b 2766  ame][parname]['f
-0001c7c0: 665f 746f 6767 6c65 275d 2e73 6574 456e  f_toggle'].setEn
-0001c7d0: 6162 6c65 6428 0a20 2020 2020 2020 2020  abled(.         
-0001c7e0: 2020 2020 2020 2020 2020 2046 616c 7365             False
-0001c7f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001c800: 2029 0a0a 2020 2020 2020 2020 636f 6e74   )..        cont
-0001c810: 6169 6e65 725f 6c61 796f 7574 2e73 6574  ainer_layout.set
-0001c820: 416c 6967 6e6d 656e 7428 5174 436f 7265  Alignment(QtCore
-0001c830: 2e51 742e 416c 6967 6e56 4365 6e74 6572  .Qt.AlignVCenter
-0001c840: 290a 2020 2020 2020 2020 7363 726f 6c6c  ).        scroll
-0001c850: 5f63 6f6e 7461 696e 6572 2e73 6574 5369  _container.setSi
-0001c860: 7a65 506f 6c69 6379 280a 2020 2020 2020  zePolicy(.      
-0001c870: 2020 2020 2020 5174 5769 6467 6574 732e        QtWidgets.
-0001c880: 5153 697a 6550 6f6c 6963 792e 4d61 7869  QSizePolicy.Maxi
-0001c890: 6d75 6d2c 0a20 2020 2020 2020 2020 2020  mum,.           
-0001c8a0: 2051 7457 6964 6765 7473 2e51 5369 7a65   QtWidgets.QSize
-0001c8b0: 506f 6c69 6379 2e4d 6178 696d 756d 0a20  Policy.Maximum. 
-0001c8c0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0001c8d0: 2072 6873 5f63 6f6c 5f73 6372 6f6c 6c2e   rhs_col_scroll.
-0001c8e0: 7365 744d 696e 696d 756d 4865 6967 6874  setMinimumHeight
-0001c8f0: 2835 3735 290a 0a20 2020 2020 2020 2023  (575)..        #
-0001c900: 2054 6f70 2072 6f77 0a20 2020 2020 2020   Top row.       
-0001c910: 2023 204c 4853 2070 6c6f 742c 2052 4853   # LHS plot, RHS
-0001c920: 2053 6c69 6465 7273 2c20 7465 7874 2c20   Sliders, text, 
-0001c930: 6c61 6265 6c73 0a20 2020 2020 2020 2074  labels.        t
-0001c940: 6f70 5f72 6f77 5f6c 6179 6f75 7420 3d20  op_row_layout = 
-0001c950: 5174 5769 6467 6574 732e 5148 426f 784c  QtWidgets.QHBoxL
-0001c960: 6179 6f75 7428 746f 705f 726f 775f 7769  ayout(top_row_wi
-0001c970: 6467 6574 290a 2020 2020 2020 2020 746f  dget).        to
-0001c980: 705f 726f 775f 6c61 796f 7574 2e61 6464  p_row_layout.add
-0001c990: 5769 6467 6574 286c 6873 5f63 6f6c 5f77  Widget(lhs_col_w
-0001c9a0: 6964 6765 742c 2033 290a 2020 2020 2020  idget, 3).      
-0001c9b0: 2020 746f 705f 726f 775f 6c61 796f 7574    top_row_layout
-0001c9c0: 2e61 6464 5769 6467 6574 2872 6873 5f63  .addWidget(rhs_c
-0001c9d0: 6f6c 5f77 6964 6765 742c 2032 290a 0a20  ol_widget, 2).. 
-0001c9e0: 2020 2020 2020 2023 2042 6f74 746f 6d20         # Bottom 
-0001c9f0: 726f 770a 2020 2020 2020 2020 2320 4275  row.        # Bu
-0001ca00: 7474 6f6e 7320 666f 7220 7265 7365 7420  ttons for reset 
-0001ca10: 616e 6420 6669 740a 2020 2020 2020 2020  and fit.        
-0001ca20: 7365 6c66 2e66 6974 5f62 746e 5f77 6964  self.fit_btn_wid
-0001ca30: 6765 7420 3d20 5174 5769 6467 6574 732e  get = QtWidgets.
-0001ca40: 5150 7573 6842 7574 746f 6e28 0a20 2020  QPushButton(.   
-0001ca50: 2020 2020 2020 2020 2070 6172 656e 743d           parent=
-0001ca60: 626f 745f 726f 775f 7769 6467 6574 2c0a  bot_row_widget,.
-0001ca70: 2020 2020 2020 2020 2020 2020 7465 7874              text
-0001ca80: 3d27 4669 7427 0a20 2020 2020 2020 2029  ='Fit'.        )
-0001ca90: 0a20 2020 2020 2020 2073 656c 662e 6669  .        self.fi
-0001caa0: 745f 6274 6e5f 7769 6467 6574 2e73 6574  t_btn_widget.set
-0001cab0: 5374 796c 6553 6865 6574 2827 666f 6e74  StyleSheet('font
-0001cac0: 2d77 6569 6768 743a 2062 6f6c 643b 2729  -weight: bold;')
-0001cad0: 0a0a 2020 2020 2020 2020 7365 6c66 2e66  ..        self.f
-0001cae0: 6974 5f62 746e 5f77 6964 6765 742e 7365  it_btn_widget.se
-0001caf0: 7445 6e61 626c 6564 2846 616c 7365 290a  tEnabled(False).
-0001cb00: 2020 2020 2020 2020 7365 6c66 2e66 6974          self.fit
-0001cb10: 5f62 746e 5f77 6964 6765 742e 636c 6963  _btn_widget.clic
-0001cb20: 6b65 642e 636f 6e6e 6563 7428 7365 6c66  ked.connect(self
-0001cb30: 2e66 6974 290a 2020 2020 2020 2020 7365  .fit).        se
-0001cb40: 6c66 2e66 6974 5f62 746e 5f77 6964 6765  lf.fit_btn_widge
-0001cb50: 742e 7365 7453 697a 6550 6f6c 6963 7928  t.setSizePolicy(
-0001cb60: 0a20 2020 2020 2020 2020 2020 2051 7457  .            QtW
-0001cb70: 6964 6765 7473 2e51 5369 7a65 506f 6c69  idgets.QSizePoli
-0001cb80: 6379 2e46 6978 6564 2c0a 2020 2020 2020  cy.Fixed,.      
-0001cb90: 2020 2020 2020 5174 5769 6467 6574 732e        QtWidgets.
-0001cba0: 5153 697a 6550 6f6c 6963 792e 4669 7865  QSizePolicy.Fixe
-0001cbb0: 640a 2020 2020 2020 2020 290a 2020 2020  d.        ).    
-0001cbc0: 2020 2020 7265 7365 745f 6274 6e5f 7769      reset_btn_wi
-0001cbd0: 6467 6574 203d 2051 7457 6964 6765 7473  dget = QtWidgets
-0001cbe0: 2e51 5075 7368 4275 7474 6f6e 280a 2020  .QPushButton(.  
-0001cbf0: 2020 2020 2020 2020 2020 7061 7265 6e74            parent
-0001cc00: 3d62 6f74 5f72 6f77 5f77 6964 6765 742c  =bot_row_widget,
-0001cc10: 0a20 2020 2020 2020 2020 2020 2074 6578  .            tex
-0001cc20: 743d 2752 6573 6574 272c 0a20 2020 2020  t='Reset',.     
-0001cc30: 2020 2029 0a20 2020 2020 2020 2072 6573     ).        res
-0001cc40: 6574 5f62 746e 5f77 6964 6765 742e 7365  et_btn_widget.se
-0001cc50: 7453 7479 6c65 5368 6565 7428 2766 6f6e  tStyleSheet('fon
-0001cc60: 742d 7765 6967 6874 3a20 626f 6c64 3b27  t-weight: bold;'
-0001cc70: 290a 2020 2020 2020 2020 7265 7365 745f  ).        reset_
-0001cc80: 6274 6e5f 7769 6467 6574 2e63 6c69 636b  btn_widget.click
-0001cc90: 6564 2e63 6f6e 6e65 6374 2873 656c 662e  ed.connect(self.
-0001cca0: 7265 7365 7429 0a20 2020 2020 2020 2072  reset).        r
-0001ccb0: 6573 6574 5f62 746e 5f77 6964 6765 742e  eset_btn_widget.
-0001ccc0: 7365 7453 697a 6550 6f6c 6963 7928 0a20  setSizePolicy(. 
-0001ccd0: 2020 2020 2020 2020 2020 2051 7457 6964             QtWid
-0001cce0: 6765 7473 2e51 5369 7a65 506f 6c69 6379  gets.QSizePolicy
-0001ccf0: 2e46 6978 6564 2c0a 2020 2020 2020 2020  .Fixed,.        
-0001cd00: 2020 2020 5174 5769 6467 6574 732e 5153      QtWidgets.QS
-0001cd10: 697a 6550 6f6c 6963 792e 4669 7865 640a  izePolicy.Fixed.
-0001cd20: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-0001cd30: 2020 2023 204d 6f64 6966 7920 6669 7420     # Modify fit 
-0001cd40: 616e 6420 7265 7365 7420 6275 7474 6f6e  and reset button
-0001cd50: 2074 6578 7420 636f 6c6f 7273 2074 6f20   text colors to 
-0001cd60: 6c6f 6f6b 2067 6f6f 6420 6576 656e 0a20  look good even. 
-0001cd70: 2020 2020 2020 2023 2069 6e20 4d61 634f         # in MacO
-0001cd80: 5320 6461 726b 6d6f 6465 2e0a 2020 2020  S darkmode..    
-0001cd90: 2020 2020 7061 6c65 7474 6520 3d20 5174      palette = Qt
-0001cda0: 4775 692e 5150 616c 6574 7465 2873 656c  Gui.QPalette(sel
-0001cdb0: 662e 6669 745f 6274 6e5f 7769 6467 6574  f.fit_btn_widget
-0001cdc0: 2e70 616c 6574 7465 2829 290a 2020 2020  .palette()).    
-0001cdd0: 2020 2020 7061 6c65 7474 652e 7365 7443      palette.setC
-0001cde0: 6f6c 6f72 2851 7447 7569 2e51 5061 6c65  olor(QtGui.QPale
-0001cdf0: 7474 652e 4275 7474 6f6e 5465 7874 2c20  tte.ButtonText, 
-0001ce00: 5174 4775 692e 5143 6f6c 6f72 2827 2330  QtGui.QColor('#0
-0001ce10: 6462 3237 3327 2929 0a20 2020 2020 2020  db273')).       
-0001ce20: 2073 656c 662e 6669 745f 6274 6e5f 7769   self.fit_btn_wi
-0001ce30: 6467 6574 2e73 6574 5061 6c65 7474 6528  dget.setPalette(
-0001ce40: 7061 6c65 7474 6529 0a20 2020 2020 2020  palette).       
-0001ce50: 2070 616c 6574 7465 2e73 6574 436f 6c6f   palette.setColo
-0001ce60: 7228 5174 4775 692e 5150 616c 6574 7465  r(QtGui.QPalette
-0001ce70: 2e42 7574 746f 6e54 6578 742c 2051 7447  .ButtonText, QtG
-0001ce80: 7569 2e51 436f 6c6f 7228 2723 3462 3661  ui.QColor('#4b6a
-0001ce90: 6164 2729 290a 2020 2020 2020 2020 7265  ad')).        re
-0001cea0: 7365 745f 6274 6e5f 7769 6467 6574 2e73  set_btn_widget.s
-0001ceb0: 6574 5061 6c65 7474 6528 7061 6c65 7474  etPalette(palett
-0001cec0: 6529 0a0a 2020 2020 2020 2020 2320 4b65  e)..        # Ke
-0001ced0: 7962 6f61 7264 2073 686f 7274 6375 742c  yboard shortcut,
-0001cee0: 2070 7265 7373 2066 2074 6f20 6669 7420   press f to fit 
-0001cef0: 6966 2066 6974 2062 7574 746f 6e20 6e6f  if fit button no
-0001cf00: 7420 6772 6579 6564 206f 7574 0a20 2020  t greyed out.   
-0001cf10: 2020 2020 2073 656c 662e 6669 745f 7368       self.fit_sh
-0001cf20: 6f72 7463 7574 203d 2051 7457 6964 6765  ortcut = QtWidge
-0001cf30: 7473 2e51 5368 6f72 7463 7574 2851 7447  ts.QShortcut(QtG
-0001cf40: 7569 2e51 4b65 7953 6571 7565 6e63 6528  ui.QKeySequence(
-0001cf50: 2766 2729 2c20 7365 6c66 290a 2020 2020  'f'), self).    
-0001cf60: 2020 2020 7365 6c66 2e66 6974 5f73 686f      self.fit_sho
-0001cf70: 7274 6375 742e 6163 7469 7661 7465 642e  rtcut.activated.
-0001cf80: 636f 6e6e 6563 7428 0a20 2020 2020 2020  connect(.       
-0001cf90: 2020 2020 206c 616d 6264 613a 2073 656c       lambda: sel
-0001cfa0: 662e 6b65 7962 6f61 7264 5f66 6974 5f63  f.keyboard_fit_c
-0001cfb0: 616c 6c62 6163 6b28 290a 2020 2020 2020  allback().      
-0001cfc0: 2020 290a 0a20 2020 2020 2020 2062 6f74    )..        bot
-0001cfd0: 5f72 6f77 5f6c 6179 6f75 7420 3d20 5174  _row_layout = Qt
-0001cfe0: 5769 6467 6574 732e 5148 426f 784c 6179  Widgets.QHBoxLay
-0001cff0: 6f75 7428 626f 745f 726f 775f 7769 6467  out(bot_row_widg
-0001d000: 6574 290a 2020 2020 2020 2020 626f 745f  et).        bot_
-0001d010: 726f 775f 6c61 796f 7574 2e61 6464 5769  row_layout.addWi
-0001d020: 6467 6574 2873 656c 662e 6669 745f 6274  dget(self.fit_bt
-0001d030: 6e5f 7769 6467 6574 290a 2020 2020 2020  n_widget).      
-0001d040: 2020 626f 745f 726f 775f 6c61 796f 7574    bot_row_layout
-0001d050: 2e61 6464 5769 6467 6574 2872 6573 6574  .addWidget(reset
-0001d060: 5f62 746e 5f77 6964 6765 7429 0a0a 2020  _btn_widget)..  
-0001d070: 2020 2020 2020 2320 4f76 6572 616c 6c20        # Overall 
-0001d080: 6170 700a 2020 2020 2020 2020 2320 546f  app.        # To
-0001d090: 7020 616e 6420 426f 7474 6f6d 2072 6f77  p and Bottom row
-0001d0a0: 730a 2020 2020 2020 2020 6675 6c6c 5f6c  s.        full_l
-0001d0b0: 6179 6f75 7420 3d20 5174 5769 6467 6574  ayout = QtWidget
-0001d0c0: 732e 5156 426f 784c 6179 6f75 7428 7365  s.QVBoxLayout(se
-0001d0d0: 6c66 2e77 6964 6765 7429 0a20 2020 2020  lf.widget).     
-0001d0e0: 2020 2066 756c 6c5f 6c61 796f 7574 2e61     full_layout.a
-0001d0f0: 6464 5769 6467 6574 2874 6f70 5f72 6f77  ddWidget(top_row
-0001d100: 5f77 6964 6765 7429 0a20 2020 2020 2020  _widget).       
-0001d110: 2066 756c 6c5f 6c61 796f 7574 2e61 6464   full_layout.add
-0001d120: 5769 6467 6574 2862 6f74 5f72 6f77 5f77  Widget(bot_row_w
-0001d130: 6964 6765 7429 0a0a 2020 2020 2020 2020  idget)..        
-0001d140: 2320 5365 7420 6c61 796f 7574 0a20 2020  # Set layout.   
-0001d150: 2020 2020 2073 656c 662e 7769 6467 6574       self.widget
-0001d160: 2e73 6574 4c61 796f 7574 2866 756c 6c5f  .setLayout(full_
-0001d170: 6c61 796f 7574 290a 2020 2020 2020 2020  layout).        
-0001d180: 7365 6c66 2e77 6964 6765 742e 7365 7453  self.widget.setS
-0001d190: 697a 6550 6f6c 6963 7928 0a20 2020 2020  izePolicy(.     
-0001d1a0: 2020 2020 2020 2051 7457 6964 6765 7473         QtWidgets
-0001d1b0: 2e51 5369 7a65 506f 6c69 6379 2e45 7870  .QSizePolicy.Exp
-0001d1c0: 616e 6469 6e67 2c0a 2020 2020 2020 2020  anding,.        
-0001d1d0: 2020 2020 5174 5769 6467 6574 732e 5153      QtWidgets.QS
-0001d1e0: 697a 6550 6f6c 6963 792e 4578 7061 6e64  izePolicy.Expand
-0001d1f0: 696e 670a 2020 2020 2020 2020 290a 0a20  ing.        ).. 
-0001d200: 2020 2020 2020 2072 6574 7572 6e0a 0a20         return.. 
-0001d210: 2020 2064 6566 206b 6579 626f 6172 645f     def keyboard_
-0001d220: 6669 745f 6361 6c6c 6261 636b 2873 656c  fit_callback(sel
-0001d230: 6629 3a0a 2020 2020 2020 2020 2727 270a  f):.        '''.
-0001d240: 2020 2020 2020 2020 4361 6c6c 6261 636b          Callback
-0001d250: 2066 6f72 2070 7265 7373 696e 6720 2766   for pressing 'f
-0001d260: 2720 6b65 792e 2052 756e 7320 6669 7420  ' key. Runs fit 
-0001d270: 6275 7474 6f6e 2069 6620 6e6f 7420 6772  button if not gr
-0001d280: 6579 6564 206f 7574 0a20 2020 2020 2020  eyed out.       
-0001d290: 2027 2727 0a0a 2020 2020 2020 2020 2320   '''..        # 
-0001d2a0: 4368 6563 6b20 6669 7420 6275 7474 6f6e  Check fit button
-0001d2b0: 2069 7320 6e6f 7420 6772 6579 6564 206f   is not greyed o
-0001d2c0: 7574 0a20 2020 2020 2020 2069 6620 7365  ut.        if se
-0001d2d0: 6c66 2e66 6974 5f62 746e 5f77 6964 6765  lf.fit_btn_widge
-0001d2e0: 742e 6973 456e 6162 6c65 6428 293a 0a20  t.isEnabled():. 
-0001d2f0: 2020 2020 2020 2020 2020 2023 2052 756e             # Run
-0001d300: 2066 6974 2063 6f64 652c 2074 6869 7320   fit code, this 
-0001d310: 636c 6f73 6573 2061 7070 0a20 2020 2020  closes app.     
-0001d320: 2020 2020 2020 2073 656c 662e 6669 7428         self.fit(
-0001d330: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-0001d340: 6e0a 0a20 2020 2064 6566 2072 6573 6574  n..    def reset
-0001d350: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0001d360: 2727 270a 2020 2020 2020 2020 4361 6c6c  '''.        Call
-0001d370: 6261 636b 2066 6f72 2052 6573 6574 2062  back for Reset b
-0001d380: 7574 746f 6e2e 0a20 2020 2020 2020 2052  utton..        R
-0001d390: 6574 7572 6e73 2077 696e 646f 7720 6261  eturns window ba
-0001d3a0: 636b 2074 6f20 6f72 6967 696e 616c 206c  ck to original l
-0001d3b0: 6179 6f75 742f 7365 6c65 6374 696f 6e73  ayout/selections
-0001d3c0: 0a20 2020 2020 2020 2027 2727 0a0a 2020  .        '''..  
-0001d3d0: 2020 2020 2020 2320 466f 7220 6561 6368        # For each
-0001d3e0: 206d 6f64 656c 2c20 7265 6d6f 7665 2070   model, remove p
-0001d3f0: 6c6f 742c 2061 6e64 2072 6573 6574 2070  lot, and reset p
-0001d400: 6172 616d 6574 6572 2076 616c 7565 730a  arameter values.
-0001d410: 2020 2020 2020 2020 666f 7220 6d6f 6465          for mode
-0001d420: 6c20 696e 2073 656c 662e 7375 7070 6f72  l in self.suppor
-0001d430: 7465 645f 6d6f 6465 6c73 3a0a 2020 2020  ted_models:.    
-0001d440: 2020 2020 2020 2020 6d6f 6465 6c6e 616d          modelnam
-0001d450: 6520 3d20 6d6f 6465 6c2e 4e41 4d45 2e6c  e = model.NAME.l
-0001d460: 6f77 6572 2829 0a0a 2020 2020 2020 2020  ower()..        
-0001d470: 2020 2020 2320 4469 7361 626c 6520 616c      # Disable al
-0001d480: 6c20 6d6f 6465 6c73 0a20 2020 2020 2020  l models.       
-0001d490: 2020 2020 2073 656c 662e 7573 656c 2e6d       self.usel.m
-0001d4a0: 6f64 656c 735b 6d6f 6465 6c6e 616d 655d  odels[modelname]
-0001d4b0: 203d 2046 616c 7365 0a20 2020 2020 2020   = False.       
-0001d4c0: 2020 2020 2023 2061 6e64 2075 6e74 6963       # and untic
-0001d4d0: 6b20 6368 6563 6b62 6f78 6573 0a20 2020  k checkboxes.   
-0001d4e0: 2020 2020 2020 2020 2073 656c 662e 7469           self.ti
-0001d4f0: 636b 6469 6374 5b6d 6f64 656c 6e61 6d65  ckdict[modelname
-0001d500: 5d2e 7365 7443 6865 636b 5374 6174 6528  ].setCheckState(
-0001d510: 4661 6c73 6529 0a0a 2020 2020 2020 2020  False)..        
-0001d520: 2020 2020 2320 5265 6d6f 7665 2063 6f72      # Remove cor
-0001d530: 7265 7370 6f6e 6469 6e67 2070 6c6f 740a  responding plot.
-0001d540: 2020 2020 2020 2020 2020 2020 5f70 6c6f              _plo
-0001d550: 7420 3d20 7365 6c66 2e6d 6f64 656c 5f70  t = self.model_p
-0001d560: 6c6f 7473 5b6d 6f64 656c 6e61 6d65 5d0a  lots[modelname].
-0001d570: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0001d580: 2e70 6c6f 745f 7769 6467 6574 2e72 656d  .plot_widget.rem
-0001d590: 6f76 6549 7465 6d28 5f70 6c6f 7429 0a0a  oveItem(_plot)..
-0001d5a0: 2020 2020 2020 2020 2020 2020 2320 5265              # Re
-0001d5b0: 7365 7420 6561 6368 2070 6172 616d 6574  set each paramet
-0001d5c0: 6572 2073 6c69 6465 722c 2065 6e74 7279  er slider, entry
-0001d5d0: 2c20 616e 6420 6669 7466 6978 0a20 2020  , and fitfix.   
-0001d5e0: 2020 2020 2020 2020 2023 2062 6163 6b20           # back 
-0001d5f0: 746f 206f 7269 6769 6e61 6c20 7661 6c75  to original valu
-0001d600: 650a 2020 2020 2020 2020 2020 2020 666f  e.            fo
-0001d610: 7220 7061 726e 616d 6520 696e 206d 6f64  r parname in mod
-0001d620: 656c 2e50 4152 4e41 4d45 533a 0a20 2020  el.PARNAMES:.   
-0001d630: 2020 2020 2020 2020 2020 2020 2073 6574               set
-0001d640: 6174 7472 280a 2020 2020 2020 2020 2020  attr(.          
-0001d650: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
-0001d660: 6172 7374 6f72 652c 0a20 2020 2020 2020  arstore,.       
-0001d670: 2020 2020 2020 2020 2020 2020 2070 6172               par
-0001d680: 6e61 6d65 2c0a 2020 2020 2020 2020 2020  name,.          
-0001d690: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
-0001d6a0: 6566 6175 6c74 735b 6d6f 6465 6c2e 4e41  efaults[model.NA
-0001d6b0: 4d45 5d5b 7061 726e 616d 655d 5b27 7661  ME][parname]['va
-0001d6c0: 6c69 6e69 7427 5d0a 2020 2020 2020 2020  linit'].        
-0001d6d0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0001d6e0: 2020 2020 2020 2020 2020 7365 6c66 2e77            self.w
-0001d6f0: 6964 6765 7464 6963 745b 6d6f 6465 6c6e  idgetdict[modeln
-0001d700: 616d 655d 5b70 6172 6e61 6d65 5d5b 2773  ame][parname]['s
-0001d710: 6c69 6465 7227 5d2e 7365 7456 616c 7565  lider'].setValue
-0001d720: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0001d730: 2020 2020 2020 696e 7428 7365 6c66 2e64        int(self.d
-0001d740: 6566 6175 6c74 735b 6d6f 6465 6c2e 4e41  efaults[model.NA
-0001d750: 4d45 5d5b 7061 726e 616d 655d 5b27 7661  ME][parname]['va
-0001d760: 6c69 6e69 7427 5d29 0a20 2020 2020 2020  linit']).       
-0001d770: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-0001d780: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0001d790: 7769 6467 6574 6469 6374 5b6d 6f64 656c  widgetdict[model
-0001d7a0: 6e61 6d65 5d5b 7061 726e 616d 655d 5b27  name][parname]['
-0001d7b0: 656e 7472 7927 5d2e 7365 7456 616c 7565  entry'].setValue
-0001d7c0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0001d7d0: 2020 2020 2020 7365 6c66 2e64 6566 6175        self.defau
-0001d7e0: 6c74 735b 6d6f 6465 6c2e 4e41 4d45 5d5b  lts[model.NAME][
-0001d7f0: 7061 726e 616d 655d 5b27 7661 6c69 6e69  parname]['valini
-0001d800: 7427 5d0a 2020 2020 2020 2020 2020 2020  t'].            
-0001d810: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-0001d820: 2020 2020 2020 7365 6c66 2e77 6964 6765        self.widge
-0001d830: 7464 6963 745b 6d6f 6465 6c6e 616d 655d  tdict[modelname]
-0001d840: 5b70 6172 6e61 6d65 5d5b 2766 665f 746f  [parname]['ff_to
-0001d850: 6767 6c65 275d 2e73 6574 5465 7874 280a  ggle'].setText(.
-0001d860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d870: 2020 2020 2746 7265 6527 0a20 2020 2020      'Free'.     
-0001d880: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
-0001d890: 2020 2020 2020 2320 5265 6d6f 7665 2074        # Remove t
-0001d8a0: 6f74 616c 206d 6f64 656c 2070 6c6f 740a  otal model plot.
-0001d8b0: 2020 2020 2020 2020 7365 6c66 2e70 6c6f          self.plo
-0001d8c0: 745f 7769 6467 6574 2e72 656d 6f76 6549  t_widget.removeI
-0001d8d0: 7465 6d28 7365 6c66 2e74 6f74 290a 0a20  tem(self.tot).. 
-0001d8e0: 2020 2020 2020 2072 6574 7572 6e0a 0a20         return.. 
-0001d8f0: 2020 2064 6566 2066 6974 2873 656c 6629     def fit(self)
-0001d900: 3a0a 2020 2020 2020 2020 2727 270a 2020  :.        '''.  
-0001d910: 2020 2020 2020 4361 6c6c 6261 636b 2066        Callback f
-0001d920: 6f72 2046 6974 2062 7574 746f 6e2e 0a20  or Fit button.. 
-0001d930: 2020 2020 2020 2043 6f6c 6c65 6374 7320         Collects 
-0001d940: 7661 7269 6162 6c65 2076 616c 7565 7320  variable values 
-0001d950: 6f66 2065 6163 6820 6d6f 6465 6c20 616e  of each model an
-0001d960: 6420 6173 7365 6d62 6c65 7320 696e 746f  d assembles into
-0001d970: 2066 6974 2f66 6978 0a20 2020 2020 2020   fit/fix.       
-0001d980: 2064 6963 7469 6f6e 6172 6965 732c 2074   dictionaries, t
-0001d990: 6865 6e20 636c 6f73 6573 2074 6865 2077  hen closes the w
-0001d9a0: 696e 646f 772e 0a20 2020 2020 2020 2027  indow..        '
-0001d9b0: 2727 0a0a 2020 2020 2020 2020 6c6e 616d  ''..        lnam
-0001d9c0: 655f 746f 5f6d 6f64 656c 203d 207b 0a20  e_to_model = {. 
-0001d9d0: 2020 2020 2020 2020 2020 206d 6f64 656c             model
-0001d9e0: 2e4e 414d 452e 6c6f 7765 7228 293a 206d  .NAME.lower(): m
-0001d9f0: 6f64 656c 0a20 2020 2020 2020 2020 2020  odel.           
-0001da00: 2066 6f72 206d 6f64 656c 2069 6e20 7365   for model in se
-0001da10: 6c66 2e73 7570 706f 7274 6564 5f6d 6f64  lf.supported_mod
-0001da20: 656c 730a 2020 2020 2020 2020 7d0a 0a20  els.        }.. 
-0001da30: 2020 2020 2020 2023 2043 6f6c 6c65 6374         # Collect
-0001da40: 2076 6172 6961 626c 6573 206f 6620 6561   variables of ea
-0001da50: 6368 206d 6f64 656c 2c20 6966 2074 6861  ch model, if tha
-0001da60: 7420 6d6f 6465 6c20 6973 2065 6e61 626c  t model is enabl
-0001da70: 6564 0a20 2020 2020 2020 2023 2061 6e64  ed.        # and
-0001da80: 2061 7373 6967 6e20 746f 2066 6974 206f   assign to fit o
-0001da90: 7220 6669 780a 2020 2020 2020 2020 666f  r fix.        fo
-0001daa0: 7220 6d6f 6465 6c6e 616d 652c 2065 6e61  r modelname, ena
-0001dab0: 626c 6564 2069 6e20 7365 6c66 2e75 7365  bled in self.use
-0001dac0: 6c2e 6d6f 6465 6c73 2e69 7465 6d73 2829  l.models.items()
-0001dad0: 3a0a 2020 2020 2020 2020 2020 2020 5f66  :.            _f
-0001dae0: 6974 5f76 6172 7320 3d20 6469 6374 2829  it_vars = dict()
-0001daf0: 0a20 2020 2020 2020 2020 2020 205f 6669  .            _fi
-0001db00: 785f 7661 7273 203d 2064 6963 7428 290a  x_vars = dict().
-0001db10: 2020 2020 2020 2020 2020 2020 6966 2065              if e
-0001db20: 6e61 626c 6564 3a0a 2020 2020 2020 2020  nabled:.        
-0001db30: 2020 2020 2020 2020 6d6f 6465 6c20 3d20          model = 
-0001db40: 6c6e 616d 655f 746f 5f6d 6f64 656c 5b6d  lname_to_model[m
-0001db50: 6f64 656c 6e61 6d65 5d0a 2020 2020 2020  odelname].      
-0001db60: 2020 2020 2020 2020 2020 666f 7220 6e61            for na
-0001db70: 6d65 2069 6e20 6d6f 6465 6c2e 5041 524e  me in model.PARN
-0001db80: 414d 4553 3a0a 2020 2020 2020 2020 2020  AMES:.          
-0001db90: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-0001dba0: 662e 7573 656c 2e66 6974 5b6e 616d 655d  f.usel.fit[name]
-0001dbb0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001dbc0: 2020 2020 2020 2020 2020 5f66 6974 5f76            _fit_v
-0001dbd0: 6172 735b 6e61 6d65 5d20 3d20 6765 7461  ars[name] = geta
-0001dbe0: 7474 7228 7365 6c66 2e70 6172 7374 6f72  ttr(self.parstor
-0001dbf0: 652c 206e 616d 6529 0a20 2020 2020 2020  e, name).       
-0001dc00: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-0001dc10: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0001dc20: 2020 2020 2020 2020 2020 205f 6669 785f             _fix_
-0001dc30: 7661 7273 5b6e 616d 655d 203d 2067 6574  vars[name] = get
-0001dc40: 6174 7472 2873 656c 662e 7061 7273 746f  attr(self.parsto
-0001dc50: 7265 2c20 6e61 6d65 290a 0a20 2020 2020  re, name)..     
-0001dc60: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0001dc70: 7573 656c 2e66 6974 5f76 6172 732e 6170  usel.fit_vars.ap
-0001dc80: 7065 6e64 285f 6669 745f 7661 7273 290a  pend(_fit_vars).
-0001dc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dca0: 7365 6c66 2e75 7365 6c2e 6669 785f 7661  self.usel.fix_va
-0001dcb0: 7273 2e61 7070 656e 6428 5f66 6978 5f76  rs.append(_fix_v
-0001dcc0: 6172 7329 0a0a 2020 2020 2020 2020 2320  ars)..        # 
-0001dcd0: 5365 7420 2768 6173 2070 726f 6772 616d  Set 'has program
-0001dce0: 2062 6565 6e20 6578 6974 6564 2720 666c   been exited' fl
-0001dcf0: 6167 2074 6f20 6661 6c73 650a 2020 2020  ag to false.    
-0001dd00: 2020 2020 7365 6c66 2e75 7365 6c2e 6578      self.usel.ex
-0001dd10: 6974 6564 203d 2046 616c 7365 0a0a 2020  ited = False..  
-0001dd20: 2020 2020 2020 2320 436c 6f73 6520 7468        # Close th
-0001dd30: 6520 7769 6e64 6f77 0a20 2020 2020 2020  e window.       
-0001dd40: 2073 656c 662e 636c 6f73 6528 290a 2020   self.close().  
-0001dd50: 2020 2020 2020 7265 7475 726e 0a0a 2020        return..  
-0001dd60: 2020 6465 6620 7570 6461 7465 5f6d 6f64    def update_mod
-0001dd70: 656c 706c 6f74 2873 656c 662c 2076 616c  elplot(self, val
-0001dd80: 7565 2c20 7061 726e 616d 652c 206d 6f64  ue, parname, mod
-0001dd90: 656c 3a20 4c6f 6754 6175 544d 6f64 656c  el: LogTauTModel
-0001dda0: 293a 0a0a 2020 2020 2020 2020 2320 5365  ):..        # Se
-0001ddb0: 7420 6e65 7720 7061 7261 6d65 7465 7220  t new parameter 
-0001ddc0: 7661 6c75 650a 2020 2020 2020 2020 7365  value.        se
-0001ddd0: 7461 7474 7228 7365 6c66 2e70 6172 7374  tattr(self.parst
-0001dde0: 6f72 652c 2070 6172 6e61 6d65 2c20 666c  ore, parname, fl
-0001ddf0: 6f61 7428 7661 6c75 6529 290a 0a20 2020  oat(value))..   
-0001de00: 2020 2020 2070 6172 616d 6574 6572 7320       parameters 
-0001de10: 3d20 6d6f 6465 6c2e 7365 745f 696e 6974  = model.set_init
-0001de20: 6961 6c5f 7661 6c73 280a 2020 2020 2020  ial_vals(.      
-0001de30: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
-0001de40: 2020 2020 2020 2020 7061 726e 616d 653a          parname:
-0001de50: 2067 6574 6174 7472 2873 656c 662e 7061   getattr(self.pa
-0001de60: 7273 746f 7265 2c20 7061 726e 616d 6529  rstore, parname)
-0001de70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001de80: 2066 6f72 2070 6172 6e61 6d65 2069 6e20   for parname in 
-0001de90: 6d6f 6465 6c2e 5041 524e 414d 4553 0a20  model.PARNAMES. 
-0001dea0: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
-0001deb0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-0001dec0: 6e65 775f 7261 7465 7320 3d20 3130 2a2a  new_rates = 10**
-0001ded0: 6d6f 6465 6c2e 6d6f 6465 6c28 7061 7261  model.model(para
-0001dee0: 6d65 7465 7273 2c20 7365 6c66 2e74 656d  meters, self.tem
-0001def0: 705f 6772 6964 290a 0a20 2020 2020 2020  p_grid)..       
-0001df00: 205f 706c 6f74 203d 2073 656c 662e 6d6f   _plot = self.mo
-0001df10: 6465 6c5f 706c 6f74 735b 6d6f 6465 6c2e  del_plots[model.
-0001df20: 4e41 4d45 2e6c 6f77 6572 2829 5d0a 2020  NAME.lower()].  
-0001df30: 2020 2020 2020 5f70 6c6f 742e 7365 7444        _plot.setD
-0001df40: 6174 6128 7365 6c66 2e74 656d 705f 6772  ata(self.temp_gr
-0001df50: 6964 2c20 6e65 775f 7261 7465 7329 0a0a  id, new_rates)..
-0001df60: 2020 2020 2020 2020 2320 5570 6461 7465          # Update
-0001df70: 2074 6f74 616c 2070 6c6f 7420 6173 2073   total plot as s
-0001df80: 756d 206f 6620 616c 6c20 6d6f 6465 6c73  um of all models
-0001df90: 0a20 2020 2020 2020 2023 2075 7365 2079  .        # use y
-0001dfa0: 6461 7461 206f 6620 6561 6368 206d 6f64  data of each mod
-0001dfb0: 656c 0a20 2020 2020 2020 2074 6f74 616c  el.        total
-0001dfc0: 5f72 6174 6573 203d 206e 702e 7a65 726f  _rates = np.zero
-0001dfd0: 7328 7365 6c66 2e74 656d 705f 6772 6964  s(self.temp_grid
-0001dfe0: 2e73 6861 7065 290a 2020 2020 2020 2020  .shape).        
-0001dff0: 746f 7461 6c5f 7261 7465 7320 2b3d 206e  total_rates += n
-0001e000: 702e 7375 6d28 0a20 2020 2020 2020 2020  p.sum(.         
-0001e010: 2020 205b 0a20 2020 2020 2020 2020 2020     [.           
-0001e020: 2020 2020 205f 706c 6f74 2e79 4461 7461       _plot.yData
-0001e030: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001e040: 2066 6f72 206e 616d 652c 205f 706c 6f74   for name, _plot
-0001e050: 2069 6e20 7365 6c66 2e6d 6f64 656c 5f70   in self.model_p
-0001e060: 6c6f 7473 2e69 7465 6d73 2829 0a20 2020  lots.items().   
-0001e070: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0001e080: 7365 6c66 2e75 7365 6c2e 6d6f 6465 6c73  self.usel.models
-0001e090: 5b6e 616d 655d 0a20 2020 2020 2020 2020  [name].         
-0001e0a0: 2020 205d 2c0a 2020 2020 2020 2020 2020     ],.          
-0001e0b0: 2020 6178 6973 3d30 0a20 2020 2020 2020    axis=0.       
-0001e0c0: 2029 0a20 2020 2020 2020 2073 656c 662e   ).        self.
-0001e0d0: 746f 742e 7365 7444 6174 6128 7365 6c66  tot.setData(self
-0001e0e0: 2e74 656d 705f 6772 6964 2c20 746f 7461  .temp_grid, tota
-0001e0f0: 6c5f 7261 7465 7329 0a0a 2020 2020 2020  l_rates)..      
-0001e100: 2020 7265 7475 726e 0a0a 2020 2020 6465    return..    de
-0001e110: 6620 746f 6767 6c65 5f70 6c6f 7428 7365  f toggle_plot(se
-0001e120: 6c66 2c20 7661 6c3a 2069 6e74 2c0a 2020  lf, val: int,.  
-0001e130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e140: 2020 6d6f 6465 6c3a 204c 6f67 5461 7554    model: LogTauT
-0001e150: 4d6f 6465 6c20 7c20 4c6f 6754 6175 484d  Model | LogTauHM
-0001e160: 6f64 656c 2920 2d3e 204e 6f6e 653a 0a20  odel) -> None:. 
-0001e170: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
-0001e180: 2020 2043 616c 6c62 6163 6b20 666f 7220     Callback for 
-0001e190: 746f 6767 6c69 6e67 206d 6f64 656c 2063  toggling model c
-0001e1a0: 6865 636b 626f 7865 730a 0a20 2020 2020  heckboxes..     
-0001e1b0: 2020 2043 616c 6375 6c61 7465 7320 6d6f     Calculates mo
-0001e1c0: 6465 6c20 6461 7461 2c20 6164 6473 2f64  del data, adds/d
-0001e1d0: 656c 6574 6573 206c 696e 6520 6672 6f6d  eletes line from
-0001e1e0: 2070 6c6f 740a 2020 2020 2020 2020 616e   plot.        an
-0001e1f0: 6420 7570 6461 7465 7320 746f 7461 6c20  d updates total 
-0001e200: 6d6f 6465 6c20 706c 6f74 0a20 2020 2020  model plot.     
-0001e210: 2020 2027 2727 0a0a 2020 2020 2020 2020     '''..        
-0001e220: 6d6f 6465 6c6e 616d 6520 3d20 6d6f 6465  modelname = mode
-0001e230: 6c2e 4e41 4d45 2e6c 6f77 6572 2829 0a0a  l.NAME.lower()..
-0001e240: 2020 2020 2020 2020 2320 436f 6e76 6572          # Conver
-0001e250: 7420 7661 6c20 746f 2062 6f6f 6c0a 2020  t val to bool.  
-0001e260: 2020 2020 2020 7661 6c20 3d20 626f 6f6c        val = bool
-0001e270: 2876 616c 202f 2032 290a 0a20 2020 2020  (val / 2)..     
-0001e280: 2020 2023 2055 7064 6174 6520 6c69 7374     # Update list
-0001e290: 206f 6620 6d6f 6465 6c73 0a20 2020 2020   of models.     
-0001e2a0: 2020 2073 656c 662e 7573 656c 2e6d 6f64     self.usel.mod
-0001e2b0: 656c 735b 6d6f 6465 6c6e 616d 655d 203d  els[modelname] =
-0001e2c0: 2076 616c 0a0a 2020 2020 2020 2020 2320   val..        # 
-0001e2d0: 5570 6461 7465 206d 6f64 656c 2076 616c  Update model val
-0001e2e0: 7565 7320 616e 6420 706c 6f74 2064 6174  ues and plot dat
-0001e2f0: 6120 666f 7220 6561 6368 206d 6f64 656c  a for each model
-0001e300: 2c20 616e 6420 666f 7220 746f 7461 6c0a  , and for total.
-0001e310: 2020 2020 2020 2020 666f 7220 7061 726e          for parn
-0001e320: 616d 6520 696e 206d 6f64 656c 2e50 4152  ame in model.PAR
-0001e330: 4e41 4d45 533a 0a20 2020 2020 2020 2020  NAMES:.         
-0001e340: 2020 2073 656c 662e 7570 6461 7465 5f6d     self.update_m
-0001e350: 6f64 656c 706c 6f74 280a 2020 2020 2020  odelplot(.      
-0001e360: 2020 2020 2020 2020 2020 6765 7461 7474            getatt
-0001e370: 7228 7365 6c66 2e70 6172 7374 6f72 652c  r(self.parstore,
-0001e380: 2070 6172 6e61 6d65 292c 0a20 2020 2020   parname),.     
-0001e390: 2020 2020 2020 2020 2020 2070 6172 6e61             parna
-0001e3a0: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
-0001e3b0: 2020 2020 6d6f 6465 6c0a 2020 2020 2020      model.      
-0001e3c0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-0001e3d0: 2023 2053 656c 6563 7420 6d6f 6465 6c20   # Select model 
-0001e3e0: 706c 6f74 2074 6f20 746f 6767 6c65 0a20  plot to toggle. 
-0001e3f0: 2020 2020 2020 205f 706c 6f74 203d 2073         _plot = s
-0001e400: 656c 662e 6d6f 6465 6c5f 706c 6f74 735b  elf.model_plots[
-0001e410: 6d6f 6465 6c6e 616d 655d 0a0a 2020 2020  modelname]..    
-0001e420: 2020 2020 2320 4164 6420 6261 636b 2069      # Add back i
-0001e430: 6e20 706c 6f74 0a20 2020 2020 2020 2069  n plot.        i
-0001e440: 6620 7661 6c3a 0a20 2020 2020 2020 2020  f val:.         
-0001e450: 2020 2073 656c 662e 706c 6f74 5f77 6964     self.plot_wid
-0001e460: 6765 742e 7265 6d6f 7665 4974 656d 285f  get.removeItem(_
-0001e470: 706c 6f74 290a 2020 2020 2020 2020 2020  plot).          
-0001e480: 2020 7365 6c66 2e70 6c6f 745f 7769 6467    self.plot_widg
-0001e490: 6574 2e61 6464 4974 656d 285f 706c 6f74  et.addItem(_plot
-0001e4a0: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-0001e4b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0001e4c0: 2e70 6c6f 745f 7769 6467 6574 2e72 656d  .plot_widget.rem
-0001e4d0: 6f76 6549 7465 6d28 5f70 6c6f 7429 0a0a  oveItem(_plot)..
-0001e4e0: 2020 2020 2020 2020 2320 456e 6162 6c65          # Enable
-0001e4f0: 2074 6f74 616c 2070 6c6f 7420 6966 203e   total plot if >
-0001e500: 2031 206d 6f64 656c 0a20 2020 2020 2020   1 model.       
-0001e510: 2023 2061 6e64 2065 6e61 626c 6520 6669   # and enable fi
-0001e520: 7420 6275 7474 6f6e 2069 6620 3e20 3020  t button if > 0 
-0001e530: 6d6f 6465 6c73 0a20 2020 2020 2020 206e  models.        n
-0001e540: 5f6d 6f64 656c 7320 3d20 6e70 2e73 756d  _models = np.sum
-0001e550: 285b 7661 6c20 666f 7220 7661 6c20 696e  ([val for val in
-0001e560: 2073 656c 662e 7573 656c 2e6d 6f64 656c   self.usel.model
-0001e570: 732e 7661 6c75 6573 2829 5d29 0a20 2020  s.values()]).   
-0001e580: 2020 2020 2069 6620 6e5f 6d6f 6465 6c73       if n_models
-0001e590: 203d 3d20 303a 0a20 2020 2020 2020 2020   == 0:.         
-0001e5a0: 2020 2073 656c 662e 6669 745f 6274 6e5f     self.fit_btn_
-0001e5b0: 7769 6467 6574 2e73 6574 456e 6162 6c65  widget.setEnable
-0001e5c0: 6428 4661 6c73 6529 0a20 2020 2020 2020  d(False).       
-0001e5d0: 2065 6c69 6620 6e5f 6d6f 6465 6c73 203d   elif n_models =
-0001e5e0: 3d20 313a 0a20 2020 2020 2020 2020 2020  = 1:.           
-0001e5f0: 2073 656c 662e 6669 745f 6274 6e5f 7769   self.fit_btn_wi
-0001e600: 6467 6574 2e73 6574 456e 6162 6c65 6428  dget.setEnabled(
-0001e610: 5472 7565 290a 2020 2020 2020 2020 2020  True).          
-0001e620: 2020 7365 6c66 2e70 6c6f 745f 7769 6467    self.plot_widg
-0001e630: 6574 2e72 656d 6f76 6549 7465 6d28 7365  et.removeItem(se
-0001e640: 6c66 2e74 6f74 290a 2020 2020 2020 2020  lf.tot).        
-0001e650: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0001e660: 2020 7365 6c66 2e66 6974 5f62 746e 5f77    self.fit_btn_w
-0001e670: 6964 6765 742e 7365 7445 6e61 626c 6564  idget.setEnabled
-0001e680: 2854 7275 6529 0a20 2020 2020 2020 2020  (True).         
-0001e690: 2020 2073 656c 662e 706c 6f74 5f77 6964     self.plot_wid
-0001e6a0: 6765 742e 7265 6d6f 7665 4974 656d 2873  get.removeItem(s
-0001e6b0: 656c 662e 746f 7429 0a20 2020 2020 2020  elf.tot).       
-0001e6c0: 2020 2020 2073 656c 662e 706c 6f74 5f77       self.plot_w
-0001e6d0: 6964 6765 742e 6164 6449 7465 6d28 7365  idget.addItem(se
-0001e6e0: 6c66 2e74 6f74 290a 0a20 2020 2020 2020  lf.tot)..       
-0001e6f0: 2023 2045 6e61 626c 652f 4469 7361 626c   # Enable/Disabl
-0001e700: 6520 736c 6964 6572 2c20 6368 6563 6b62  e slider, checkb
-0001e710: 6f78 2c20 616e 6420 6669 7466 6978 0a20  ox, and fitfix. 
-0001e720: 2020 2020 2020 2066 6f72 2070 6172 6e61         for parna
-0001e730: 6d65 2069 6e20 6d6f 6465 6c2e 5041 524e  me in model.PARN
-0001e740: 414d 4553 3a0a 2020 2020 2020 2020 2020  AMES:.          
-0001e750: 2020 7365 6c66 2e77 6964 6765 7464 6963    self.widgetdic
-0001e760: 745b 6d6f 6465 6c6e 616d 655d 5b70 6172  t[modelname][par
-0001e770: 6e61 6d65 5d5b 2773 6c69 6465 7227 5d2e  name]['slider'].
-0001e780: 7365 7445 6e61 626c 6564 2876 616c 290a  setEnabled(val).
-0001e790: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0001e7a0: 2e77 6964 6765 7464 6963 745b 6d6f 6465  .widgetdict[mode
-0001e7b0: 6c6e 616d 655d 5b70 6172 6e61 6d65 5d5b  lname][parname][
-0001e7c0: 2765 6e74 7279 275d 2e73 6574 456e 6162  'entry'].setEnab
-0001e7d0: 6c65 6428 7661 6c29 0a20 2020 2020 2020  led(val).       
-0001e7e0: 2020 2020 2073 656c 662e 7769 6467 6574       self.widget
-0001e7f0: 6469 6374 5b6d 6f64 656c 6e61 6d65 5d5b  dict[modelname][
-0001e800: 7061 726e 616d 655d 5b27 6666 5f74 6f67  parname]['ff_tog
-0001e810: 676c 6527 5d2e 7365 7445 6e61 626c 6564  gle'].setEnabled
-0001e820: 2876 616c 290a 0a20 2020 2020 2020 2072  (val)..        r
-0001e830: 6574 7572 6e0a 0a20 2020 2064 6566 206d  eturn..    def m
-0001e840: 616b 655f 6d6f 6465 6c62 6f78 2873 656c  ake_modelbox(sel
-0001e850: 662c 206d 6f64 656c 3a20 4c6f 6754 6175  f, model: LogTau
-0001e860: 544d 6f64 656c 2c20 7061 7265 6e74 2c20  TModel, parent, 
-0001e870: 696e 6465 783a 2069 6e74 293a 0a20 2020  index: int):.   
-0001e880: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
-0001e890: 2043 7265 6174 6573 2077 6964 6765 7420   Creates widget 
-0001e8a0: 666f 7220 6120 6769 7665 6e20 6d6f 6465  for a given mode
-0001e8b0: 6c2c 2063 6f6e 7461 696e 696e 6720 6120  l, containing a 
-0001e8c0: 6368 6563 6b62 6f78 2074 6f20 746f 6767  checkbox to togg
-0001e8d0: 6c65 0a20 2020 2020 2020 2074 6865 206d  le.        the m
-0001e8e0: 6f64 656c 2c20 616e 6420 6120 726f 7720  odel, and a row 
-0001e8f0: 6f66 2069 6e74 6572 6163 7469 7665 2077  of interactive w
-0001e900: 6964 6765 7473 2066 6f72 2065 6163 6820  idgets for each 
-0001e910: 7061 7261 6d65 7465 7220 6f66 2074 6865  parameter of the
-0001e920: 0a20 2020 2020 2020 206d 6f64 656c 0a20  .        model. 
-0001e930: 2020 2020 2020 2027 2727 0a0a 2020 2020         '''..    
-0001e940: 2020 2020 2320 5769 6467 6574 2066 6f72      # Widget for
-0001e950: 2074 6869 7320 6d6f 6465 6c0a 2020 2020   this model.    
-0001e960: 2020 2020 6d6f 6465 6c5f 7769 6467 6574      model_widget
-0001e970: 203d 2051 7457 6964 6765 7473 2e51 5769   = QtWidgets.QWi
-0001e980: 6467 6574 2870 6172 656e 743d 7061 7265  dget(parent=pare
-0001e990: 6e74 290a 2020 2020 2020 2020 6d6f 6465  nt).        mode
-0001e9a0: 6c5f 6c61 796f 7574 203d 2051 7457 6964  l_layout = QtWid
-0001e9b0: 6765 7473 2e51 4842 6f78 4c61 796f 7574  gets.QHBoxLayout
-0001e9c0: 286d 6f64 656c 5f77 6964 6765 7429 0a0a  (model_widget)..
-0001e9d0: 2020 2020 2020 2020 2320 4372 6561 7465          # Create
-0001e9e0: 2074 6963 6b62 6f78 2074 6f20 746f 6767   tickbox to togg
-0001e9f0: 6c65 2074 6869 7320 7769 6467 6574 0a20  le this widget. 
-0001ea00: 2020 2020 2020 2074 6963 6b62 6f78 5f77         tickbox_w
-0001ea10: 6964 6765 7420 3d20 5174 5769 6467 6574  idget = QtWidget
-0001ea20: 732e 5143 6865 636b 426f 7828 0a20 2020  s.QCheckBox(.   
-0001ea30: 2020 2020 2020 2020 2070 6172 656e 743d           parent=
-0001ea40: 6d6f 6465 6c5f 7769 6467 6574 2c0a 2020  model_widget,.  
-0001ea50: 2020 2020 2020 2020 2020 7465 7874 3d6d            text=m
-0001ea60: 6f64 656c 2e4e 414d 452e 7265 706c 6163  odel.NAME.replac
-0001ea70: 6528 2742 726f 6e73 2d56 616e 2d56 6c65  e('Brons-Van-Vle
-0001ea80: 636b 272c 2027 4256 5627 292c 0a0a 2020  ck', 'BVV'),..  
-0001ea90: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-0001eaa0: 2023 2041 6464 2074 6963 6b62 6f78 2074   # Add tickbox t
-0001eab0: 6f20 7468 6973 206d 6f64 656c 0a20 2020  o this model.   
-0001eac0: 2020 2020 206d 6f64 656c 5f6c 6179 6f75       model_layou
-0001ead0: 742e 6164 6457 6964 6765 7428 7469 636b  t.addWidget(tick
-0001eae0: 626f 785f 7769 6467 6574 290a 0a20 2020  box_widget)..   
-0001eaf0: 2020 2020 2023 2041 6464 2074 6f20 6469       # Add to di
-0001eb00: 6374 696f 6e61 7279 206f 6620 616c 6c20  ctionary of all 
-0001eb10: 7469 636b 626f 7865 732c 2069 6e64 6578  tickboxes, index
-0001eb20: 6564 2062 7920 6d6f 6465 6c2e 4e41 4d45  ed by model.NAME
-0001eb30: 2e6c 6f77 6572 2829 0a20 2020 2020 2020  .lower().       
-0001eb40: 2073 656c 662e 7469 636b 6469 6374 5b6d   self.tickdict[m
-0001eb50: 6f64 656c 2e4e 414d 452e 6c6f 7765 7228  odel.NAME.lower(
-0001eb60: 295d 203d 2074 6963 6b62 6f78 5f77 6964  )] = tickbox_wid
-0001eb70: 6765 740a 0a20 2020 2020 2020 2023 2057  get..        # W
-0001eb80: 6865 6e20 746f 6767 6c65 642c 2070 6c6f  hen toggled, plo
-0001eb90: 7420 7468 6973 206d 6f64 656c 0a20 2020  t this model.   
-0001eba0: 2020 2020 2074 6963 6b62 6f78 5f77 6964       tickbox_wid
-0001ebb0: 6765 742e 7374 6174 6543 6861 6e67 6564  get.stateChanged
-0001ebc0: 2e63 6f6e 6e65 6374 280a 2020 2020 2020  .connect(.      
-0001ebd0: 2020 2020 2020 6c61 6d62 6461 2076 616c        lambda val
-0001ebe0: 3a20 7365 6c66 2e74 6f67 676c 655f 706c  : self.toggle_pl
-0001ebf0: 6f74 2876 616c 2c20 6d6f 6465 6c29 0a20  ot(val, model). 
-0001ec00: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-0001ec10: 2020 2320 4164 6420 6162 696c 6974 7920    # Add ability 
-0001ec20: 746f 2074 6f67 676c 6520 6d6f 6465 6c20  to toggle model 
-0001ec30: 7573 696e 6720 6e75 6d62 6572 206b 6579  using number key
-0001ec40: 0a20 2020 2020 2020 206f 6e5f 6f66 665f  .        on_off_
-0001ec50: 7368 6f72 7463 7574 203d 2051 7457 6964  shortcut = QtWid
-0001ec60: 6765 7473 2e51 5368 6f72 7463 7574 280a  gets.QShortcut(.
-0001ec70: 2020 2020 2020 2020 2020 2020 5174 4775              QtGu
-0001ec80: 692e 514b 6579 5365 7175 656e 6365 2827  i.QKeySequence('
-0001ec90: 7b3a 647d 272e 666f 726d 6174 2869 6e64  {:d}'.format(ind
-0001eca0: 6578 2929 2c0a 2020 2020 2020 2020 2020  ex)),.          
-0001ecb0: 2020 7365 6c66 0a20 2020 2020 2020 2029    self.        )
-0001ecc0: 0a20 2020 2020 2020 206f 6e5f 6f66 665f  .        on_off_
-0001ecd0: 7368 6f72 7463 7574 2e61 6374 6976 6174  shortcut.activat
-0001ece0: 6564 2e63 6f6e 6e65 6374 280a 2020 2020  ed.connect(.    
-0001ecf0: 2020 2020 2020 2020 6c61 6d62 6461 3a20          lambda: 
-0001ed00: 7469 636b 626f 785f 7769 6467 6574 2e74  tickbox_widget.t
-0001ed10: 6f67 676c 6528 290a 2020 2020 2020 2020  oggle().        
-0001ed20: 290a 2020 2020 2020 2020 7365 6c66 2e6f  ).        self.o
-0001ed30: 6e5f 6f66 665f 7368 6f72 7463 7574 2e61  n_off_shortcut.a
-0001ed40: 7070 656e 6428 6f6e 5f6f 6666 5f73 686f  ppend(on_off_sho
-0001ed50: 7274 6375 7429 0a0a 2020 2020 2020 2020  rtcut)..        
-0001ed60: 2320 4372 6561 7465 2063 6f6e 7461 696e  # Create contain
-0001ed70: 6572 2077 6964 6765 7420 666f 7220 616c  er widget for al
-0001ed80: 6c20 7061 7261 6d65 7465 7220 726f 7773  l parameter rows
-0001ed90: 0a20 2020 2020 2020 2072 6873 5f77 6964  .        rhs_wid
-0001eda0: 6765 7420 3d20 5174 5769 6467 6574 732e  get = QtWidgets.
-0001edb0: 5157 6964 6765 7428 7061 7265 6e74 3d6d  QWidget(parent=m
-0001edc0: 6f64 656c 5f77 6964 6765 7429 0a20 2020  odel_widget).   
-0001edd0: 2020 2020 2072 6873 5f6c 6179 6f75 7420       rhs_layout 
-0001ede0: 3d20 5174 5769 6467 6574 732e 5156 426f  = QtWidgets.QVBo
-0001edf0: 784c 6179 6f75 7428 7268 735f 7769 6467  xLayout(rhs_widg
-0001ee00: 6574 290a 0a20 2020 2020 2020 2023 204d  et)..        # M
-0001ee10: 616b 6520 736c 6964 6572 2c20 7465 7874  ake slider, text
-0001ee20: 626f 782c 2061 6e64 2066 6974 2f66 6978  box, and fit/fix
-0001ee30: 2074 6f67 676c 6520 666f 7220 6561 6368   toggle for each
-0001ee40: 0a20 2020 2020 2020 2023 2070 6172 616d  .        # param
-0001ee50: 6574 6572 206f 6620 7468 6520 6375 7272  eter of the curr
-0001ee60: 656e 7420 6d6f 6465 6c0a 2020 2020 2020  ent model.      
-0001ee70: 2020 666f 7220 7061 726e 616d 6520 696e    for parname in
-0001ee80: 206d 6f64 656c 2e50 4152 4e41 4d45 533a   model.PARNAMES:
-0001ee90: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-0001eea0: 4465 6661 756c 7420 7061 7261 6d65 7465  Default paramete
-0001eeb0: 7220 7661 6c75 6573 0a20 2020 2020 2020  r values.       
-0001eec0: 2020 2020 205f 6465 6661 756c 7473 203d       _defaults =
-0001eed0: 2073 656c 662e 6465 6661 756c 7473 5b6d   self.defaults[m
-0001eee0: 6f64 656c 2e4e 414d 455d 5b70 6172 6e61  odel.NAME][parna
-0001eef0: 6d65 5d0a 0a20 2020 2020 2020 2020 2020  me]..           
-0001ef00: 2023 204e 616d 6520 616e 6420 556e 6974   # Name and Unit
-0001ef10: 7320 6173 2073 7472 696e 670a 2020 2020  s as string.    
-0001ef20: 2020 2020 2020 2020 5f6e 755f 7374 7269          _nu_stri
-0001ef30: 6e67 203d 2027 7b7d 2028 7b7d 2927 2e66  ng = '{} ({})'.f
-0001ef40: 6f72 6d61 7428 0a20 2020 2020 2020 2020  ormat(.         
-0001ef50: 2020 2020 2020 206d 6f64 656c 2e56 4152         model.VAR
-0001ef60: 4e41 4d45 535f 4854 4d4c 5b70 6172 6e61  NAMES_HTML[parna
-0001ef70: 6d65 5d2c 0a20 2020 2020 2020 2020 2020  me],.           
-0001ef80: 2020 2020 206d 6f64 656c 2e55 4e49 5453       model.UNITS
-0001ef90: 5f48 544d 4c5b 7061 726e 616d 655d 0a20  _HTML[parname]. 
-0001efa0: 2020 2020 2020 2020 2020 2029 2e72 6570             ).rep
-0001efb0: 6c61 6365 2827 2829 272c 2027 2729 0a0a  lace('()', '')..
-0001efc0: 2020 2020 2020 2020 2020 2020 2320 4361              # Ca
-0001efd0: 6c6c 6261 636b 2066 6f72 2069 6e74 6572  llback for inter
-0001efe0: 6163 7469 6f6e 2077 6974 6820 736c 6964  action with slid
-0001eff0: 6572 2c20 7465 7874 626f 782e 2e2e 0a20  er, textbox.... 
-0001f000: 2020 2020 2020 2020 2020 2063 6220 3d20             cb = 
-0001f010: 7061 7274 6961 6c28 7365 6c66 2e75 7064  partial(self.upd
-0001f020: 6174 655f 6d6f 6465 6c70 6c6f 742c 206d  ate_modelplot, m
-0001f030: 6f64 656c 3d6d 6f64 656c 2c20 7061 726e  odel=model, parn
-0001f040: 616d 653d 7061 726e 616d 6529 0a0a 2020  ame=parname)..  
-0001f050: 2020 2020 2020 2020 2020 2320 4d61 6b65            # Make
-0001f060: 2072 6f77 206f 6620 7769 6467 6574 7320   row of widgets 
-0001f070: 666f 7220 7468 6973 2070 6172 616d 6574  for this paramet
-0001f080: 6572 0a20 2020 2020 2020 2020 2020 2070  er.            p
-0001f090: 6172 626f 785f 7769 6467 6574 2c20 7061  arbox_widget, pa
-0001f0a0: 7262 6f78 5f6c 6179 6f75 7420 3d20 7365  rbox_layout = se
-0001f0b0: 6c66 2e6d 616b 655f 7061 7262 6f78 280a  lf.make_parbox(.
-0001f0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f0d0: 6362 2c20 7061 726e 616d 652c 205f 6e75  cb, parname, _nu
-0001f0e0: 5f73 7472 696e 672c 205f 6465 6661 756c  _string, _defaul
-0001f0f0: 7473 2c20 6d6f 6465 6c5f 7769 6467 6574  ts, model_widget
-0001f100: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0001f110: 2020 6d6f 6465 6c2e 4e41 4d45 2e6c 6f77    model.NAME.low
-0001f120: 6572 2829 0a20 2020 2020 2020 2020 2020  er().           
-0001f130: 2029 0a0a 2020 2020 2020 2020 2020 2020   )..            
-0001f140: 2320 616e 6420 6164 6420 746f 2074 6865  # and add to the
-0001f150: 206d 6f64 656c 2773 2062 6f78 206f 6620   model's box of 
-0001f160: 7061 7261 6d65 7465 720a 2020 2020 2020  parameter.      
-0001f170: 2020 2020 2020 7268 735f 6c61 796f 7574        rhs_layout
-0001f180: 2e61 6464 5769 6467 6574 2870 6172 626f  .addWidget(parbo
-0001f190: 785f 7769 6467 6574 290a 0a20 2020 2020  x_widget)..     
-0001f1a0: 2020 2023 2053 6574 2065 7870 616e 7369     # Set expansi
-0001f1b0: 6f6e 2062 6568 6176 696f 7572 2061 6e64  on behaviour and
-0001f1c0: 2063 656e 7465 7269 6e67 206f 6620 7769   centering of wi
-0001f1d0: 6467 6574 730a 2020 2020 2020 2020 7268  dgets.        rh
-0001f1e0: 735f 6c61 796f 7574 2e73 6574 416c 6967  s_layout.setAlig
-0001f1f0: 6e6d 656e 7428 5174 436f 7265 2e51 742e  nment(QtCore.Qt.
-0001f200: 416c 6967 6e56 4365 6e74 6572 290a 2020  AlignVCenter).  
-0001f210: 2020 2020 2020 7268 735f 7769 6467 6574        rhs_widget
-0001f220: 2e73 6574 5369 7a65 506f 6c69 6379 280a  .setSizePolicy(.
-0001f230: 2020 2020 2020 2020 2020 2020 5174 5769              QtWi
-0001f240: 6467 6574 732e 5153 697a 6550 6f6c 6963  dgets.QSizePolic
-0001f250: 792e 4669 7865 642c 0a20 2020 2020 2020  y.Fixed,.       
-0001f260: 2020 2020 2051 7457 6964 6765 7473 2e51       QtWidgets.Q
-0001f270: 5369 7a65 506f 6c69 6379 2e46 6978 6564  SizePolicy.Fixed
-0001f280: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-0001f290: 2020 2074 6963 6b62 6f78 5f77 6964 6765     tickbox_widge
-0001f2a0: 742e 7365 7453 697a 6550 6f6c 6963 7928  t.setSizePolicy(
-0001f2b0: 0a20 2020 2020 2020 2020 2020 2051 7457  .            QtW
-0001f2c0: 6964 6765 7473 2e51 5369 7a65 506f 6c69  idgets.QSizePoli
-0001f2d0: 6379 2e46 6978 6564 2c0a 2020 2020 2020  cy.Fixed,.      
-0001f2e0: 2020 2020 2020 5174 5769 6467 6574 732e        QtWidgets.
-0001f2f0: 5153 697a 6550 6f6c 6963 792e 4669 7865  QSizePolicy.Fixe
-0001f300: 640a 2020 2020 2020 2020 290a 0a20 2020  d.        )..   
-0001f310: 2020 2020 2072 6873 5f6c 6179 6f75 742e       rhs_layout.
-0001f320: 7365 7453 7061 6369 6e67 2830 290a 2020  setSpacing(0).  
-0001f330: 2020 2020 2020 7268 735f 6c61 796f 7574        rhs_layout
-0001f340: 2e61 6464 5374 7265 7463 6828 3429 0a0a  .addStretch(4)..
-0001f350: 2020 2020 2020 2020 2320 4164 6420 7061          # Add pa
-0001f360: 7261 6d65 7465 7220 726f 7773 2074 6f20  rameter rows to 
-0001f370: 7468 6973 206d 6f64 656c 0a20 2020 2020  this model.     
-0001f380: 2020 206d 6f64 656c 5f6c 6179 6f75 742e     model_layout.
-0001f390: 6164 6457 6964 6765 7428 7268 735f 7769  addWidget(rhs_wi
-0001f3a0: 6467 6574 290a 0a20 2020 2020 2020 2023  dget)..        #
-0001f3b0: 2061 6e64 2073 6574 2061 6c69 676e 6d65   and set alignme
-0001f3c0: 6e74 206f 6620 7468 6520 6d6f 6465 6c0a  nt of the model.
-0001f3d0: 2020 2020 2020 2020 6d6f 6465 6c5f 6c61          model_la
-0001f3e0: 796f 7574 2e73 6574 416c 6967 6e6d 656e  yout.setAlignmen
-0001f3f0: 7428 5174 436f 7265 2e51 742e 416c 6967  t(QtCore.Qt.Alig
-0001f400: 6e54 6f70 290a 0a20 2020 2020 2020 2072  nTop)..        r
-0001f410: 6574 7572 6e20 6d6f 6465 6c5f 7769 6467  eturn model_widg
-0001f420: 6574 0a0a 2020 2020 6465 6620 6e6f 745f  et..    def not_
-0001f430: 6966 7928 7365 6c66 2c20 7061 726e 616d  ify(self, parnam
-0001f440: 653a 2073 7472 293a 0a20 2020 2020 2020  e: str):.       
-0001f450: 2027 2727 0a20 2020 2020 2020 2053 7769   '''.        Swi
-0001f460: 7463 6865 7320 6669 7420 6469 6374 696f  tches fit dictio
-0001f470: 6e61 7279 2065 6e74 7279 2054 7275 6520  nary entry True 
-0001f480: 3c2d 2d3e 2046 616c 7365 0a20 2020 2020  <--> False.     
-0001f490: 2020 2066 6f72 2074 6865 2070 726f 7669     for the provi
-0001f4a0: 6465 6420 7061 726e 616d 650a 2020 2020  ded parname.    
-0001f4b0: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
-0001f4c0: 7365 6c66 2e75 7365 6c2e 6669 745b 7061  self.usel.fit[pa
-0001f4d0: 726e 616d 655d 203d 206e 6f74 2073 656c  rname] = not sel
-0001f4e0: 662e 7573 656c 2e66 6974 5b70 6172 6e61  f.usel.fit[parna
-0001f4f0: 6d65 5d0a 0a20 2020 2064 6566 206d 616b  me]..    def mak
-0001f500: 655f 7061 7262 6f78 2873 656c 662c 2063  e_parbox(self, c
-0001f510: 623a 2070 6172 7469 616c 2c20 7061 726e  b: partial, parn
-0001f520: 616d 653a 2073 7472 2c20 5f6e 755f 7374  ame: str, _nu_st
-0001f530: 7269 6e67 3a20 7374 722c 0a20 2020 2020  ring: str,.     
-0001f540: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-0001f550: 6566 6175 6c74 733a 2064 6963 745b 7374  efaults: dict[st
-0001f560: 722c 2066 6c6f 6174 5d2c 206f 705f 7061  r, float], op_pa
-0001f570: 723a 2051 7457 6964 6765 7473 2e51 5769  r: QtWidgets.QWi
-0001f580: 6467 6574 2c0a 2020 2020 2020 2020 2020  dget,.          
-0001f590: 2020 2020 2020 2020 2020 6d6f 6465 6c6e            modeln
-0001f5a0: 616d 653a 2073 7472 293a 0a20 2020 2020  ame: str):.     
-0001f5b0: 2020 2027 2727 0a20 2020 2020 2020 2043     '''.        C
-0001f5c0: 7265 6174 6573 2073 6574 206f 6620 7769  reates set of wi
-0001f5d0: 6467 6574 7320 666f 7220 6120 7369 6e67  dgets for a sing
-0001f5e0: 6c65 2070 6172 616d 6574 6572 206f 6620  le parameter of 
-0001f5f0: 6120 6d6f 6465 6c2e 5c6e 0a20 2020 2020  a model.\n.     
-0001f600: 2020 2043 6f6e 7461 696e 7320 3220 726f     Contains 2 ro
-0001f610: 7773 2c20 7570 7065 7220 6973 206c 6162  ws, upper is lab
-0001f620: 656c 2061 6e64 2075 6e69 7473 2061 7320  el and units as 
-0001f630: 7374 7269 6e67 2c20 616e 6420 6c6f 7765  string, and lowe
-0001f640: 720a 2020 2020 2020 2020 6973 2073 6c69  r.        is sli
-0001f650: 6465 722c 2074 6578 7465 6e74 7279 2028  der, textentry (
-0001f660: 646f 7562 6c65 7370 696e 626f 7829 2c20  doublespinbox), 
-0001f670: 616e 6420 6669 742f 6669 7820 746f 6767  and fit/fix togg
-0001f680: 6c65 2062 7574 746f 6e2e 0a0a 2020 2020  le button...    
-0001f690: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-0001f6a0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
-0001f6b0: 2d0a 2020 2020 2020 2020 6362 3a20 6675  -.        cb: fu
-0001f6c0: 6e63 746f 6f6c 732e 7061 7274 6961 6c0a  nctools.partial.
-0001f6d0: 2020 2020 2020 2020 2020 2020 5061 7274              Part
-0001f6e0: 6961 6c2d 6c79 2069 6e73 7461 6e74 6961  ial-ly instantia
-0001f6f0: 7465 6420 6361 6c6c 6261 636b 2077 6869  ted callback whi
-0001f700: 6368 2077 696c 6c20 6265 2066 6972 6564  ch will be fired
-0001f710: 2077 6865 6e0a 2020 2020 2020 2020 2020   when.          
-0001f720: 2020 7769 6467 6574 7320 6f66 2074 6869    widgets of thi
-0001f730: 7320 7061 7261 6d65 7465 7220 6172 6520  s parameter are 
-0001f740: 696e 7465 7261 6374 6564 2077 6974 682e  interacted with.
-0001f750: 0a20 2020 2020 2020 2070 6172 6e61 6d65  .        parname
-0001f760: 3a20 7374 720a 2020 2020 2020 2020 2020  : str.          
-0001f770: 2020 5374 7269 6e67 206e 616d 6520 6f66    String name of
-0001f780: 2070 6172 616d 6574 6572 2075 7365 6420   parameter used 
-0001f790: 6173 206b 6579 2069 6e0a 2020 2020 2020  as key in.      
-0001f7a0: 2020 2020 2020 7365 6c66 2e77 6964 6765        self.widge
-0001f7b0: 7464 6963 745b 7769 6467 6574 6469 6374  tdict[widgetdict
-0001f7c0: 5d0a 2020 2020 2020 2020 5f6e 755f 7374  ].        _nu_st
-0001f7d0: 7269 6e67 3a20 7374 720a 2020 2020 2020  ring: str.      
-0001f7e0: 2020 2020 2020 5374 7269 6e67 206e 616d        String nam
-0001f7f0: 6520 6f66 2070 6172 616d 6574 6572 2061  e of parameter a
-0001f800: 6e64 2075 6e69 7473 2075 7365 6420 6173  nd units used as
-0001f810: 2074 6974 6c65 206f 6620 7468 6973 2070   title of this p
-0001f820: 6172 616d 6574 6572 0a20 2020 2020 2020  arameter.       
-0001f830: 2064 6566 6175 6c74 733a 2064 6963 745b   defaults: dict[
-0001f840: 7374 722c 2066 6c6f 6174 5d0a 2020 2020  str, float].    
-0001f850: 2020 2020 2020 2020 4465 6661 756c 7420          Default 
-0001f860: 7661 6c75 6573 206f 6620 7468 6973 2070  values of this p
-0001f870: 6172 616d 6574 6572 2c20 6b65 7973 2061  arameter, keys a
-0001f880: 7265 206d 696e 2c20 6d61 782c 2076 616c  re min, max, val
-0001f890: 696e 6974 2c20 7374 6570 0a20 2020 2020  init, step.     
-0001f8a0: 2020 206f 705f 7061 723a 2051 7457 6964     op_par: QtWid
-0001f8b0: 6765 7473 2e51 5769 6467 6574 0a20 2020  gets.QWidget.   
-0001f8c0: 2020 2020 2020 2020 2050 6172 656e 7420           Parent 
-0001f8d0: 7769 6467 6574 0a20 2020 2020 2020 206d  widget.        m
-0001f8e0: 6f64 656c 6e61 6d65 3a20 7374 720a 2020  odelname: str.  
-0001f8f0: 2020 2020 2020 2020 2020 5374 7269 6e67            String
-0001f900: 206e 616d 6520 6f66 206d 6f64 656c 2075   name of model u
-0001f910: 7365 6420 6173 206b 6579 2069 6e20 7365  sed as key in se
-0001f920: 6c66 2e77 6964 6765 7464 6963 740a 2020  lf.widgetdict.  
-0001f930: 2020 2020 2020 2727 270a 0a20 2020 2020        '''..     
-0001f940: 2020 2023 2057 6964 6765 7420 666f 7220     # Widget for 
-0001f950: 7468 6973 2070 6172 616d 6574 6572 2773  this parameter's
-0001f960: 2072 6f77 206f 6620 7769 6467 6574 730a   row of widgets.
-0001f970: 2020 2020 2020 2020 6f6e 655f 7061 7261          one_para
-0001f980: 6d5f 7769 6467 6574 203d 2051 7457 6964  m_widget = QtWid
-0001f990: 6765 7473 2e51 5769 6467 6574 2870 6172  gets.QWidget(par
-0001f9a0: 656e 743d 6f70 5f70 6172 290a 2020 2020  ent=op_par).    
-0001f9b0: 2020 2020 6f6e 655f 7061 7261 6d5f 6c61      one_param_la
-0001f9c0: 796f 7574 203d 2051 7457 6964 6765 7473  yout = QtWidgets
-0001f9d0: 2e51 5642 6f78 4c61 796f 7574 286f 6e65  .QVBoxLayout(one
-0001f9e0: 5f70 6172 616d 5f77 6964 6765 7429 0a0a  _param_widget)..
-0001f9f0: 2020 2020 2020 2020 2320 466f 7220 6c61          # For la
-0001fa00: 6265 6c20 616e 6420 756e 6974 730a 2020  bel and units.  
-0001fa10: 2020 2020 2020 746f 705f 626f 7877 6964        top_boxwid
-0001fa20: 6765 7420 3d20 5174 5769 6467 6574 732e  get = QtWidgets.
-0001fa30: 5157 6964 6765 7428 7061 7265 6e74 3d6f  QWidget(parent=o
-0001fa40: 6e65 5f70 6172 616d 5f77 6964 6765 7429  ne_param_widget)
-0001fa50: 0a20 2020 2020 2020 2074 6f70 5f62 6f78  .        top_box
-0001fa60: 6c61 796f 7574 203d 2051 7457 6964 6765  layout = QtWidge
-0001fa70: 7473 2e51 4842 6f78 4c61 796f 7574 2874  ts.QHBoxLayout(t
-0001fa80: 6f70 5f62 6f78 7769 6467 6574 290a 0a20  op_boxwidget).. 
-0001fa90: 2020 2020 2020 2023 2046 6f72 2069 6e74         # For int
-0001faa0: 6572 6163 7469 7665 2077 6964 6765 7473  eractive widgets
-0001fab0: 0a20 2020 2020 2020 2062 6f74 5f62 6f78  .        bot_box
-0001fac0: 7769 6467 6574 203d 2051 7457 6964 6765  widget = QtWidge
-0001fad0: 7473 2e51 5769 6467 6574 2870 6172 656e  ts.QWidget(paren
-0001fae0: 743d 6f6e 655f 7061 7261 6d5f 7769 6467  t=one_param_widg
-0001faf0: 6574 290a 2020 2020 2020 2020 626f 745f  et).        bot_
-0001fb00: 626f 786c 6179 6f75 7420 3d20 5174 5769  boxlayout = QtWi
-0001fb10: 6467 6574 732e 5148 426f 784c 6179 6f75  dgets.QHBoxLayou
-0001fb20: 7428 626f 745f 626f 7877 6964 6765 7429  t(bot_boxwidget)
-0001fb30: 0a0a 2020 2020 2020 2020 2320 4164 6420  ..        # Add 
-0001fb40: 6c61 6265 6c20 616e 6420 756e 6974 730a  label and units.
-0001fb50: 2020 2020 2020 2020 6e61 6d65 5f75 6e69          name_uni
-0001fb60: 7473 203d 2051 7457 6964 6765 7473 2e51  ts = QtWidgets.Q
-0001fb70: 4c61 6265 6c28 5f6e 755f 7374 7269 6e67  Label(_nu_string
-0001fb80: 290a 2020 2020 2020 2020 6e61 6d65 5f75  ).        name_u
-0001fb90: 6e69 7473 2e73 6574 466f 6e74 2851 7447  nits.setFont(QtG
-0001fba0: 7569 2e51 466f 6e74 2827 4172 6961 6c27  ui.QFont('Arial'
-0001fbb0: 2c20 3131 2929 0a0a 2020 2020 2020 2020  , 11))..        
-0001fbc0: 6e61 6d65 5f75 6e69 7473 2e73 6574 5369  name_units.setSi
-0001fbd0: 7a65 506f 6c69 6379 280a 2020 2020 2020  zePolicy(.      
-0001fbe0: 2020 2020 2020 5174 5769 6467 6574 732e        QtWidgets.
-0001fbf0: 5153 697a 6550 6f6c 6963 792e 4669 7865  QSizePolicy.Fixe
-0001fc00: 642c 0a20 2020 2020 2020 2020 2020 2051  d,.            Q
-0001fc10: 7457 6964 6765 7473 2e51 5369 7a65 506f  tWidgets.QSizePo
-0001fc20: 6c69 6379 2e46 6978 6564 0a20 2020 2020  licy.Fixed.     
-0001fc30: 2020 2029 0a0a 2020 2020 2020 2020 746f     )..        to
-0001fc40: 705f 626f 786c 6179 6f75 742e 6164 6457  p_boxlayout.addW
-0001fc50: 6964 6765 7428 6e61 6d65 5f75 6e69 7473  idget(name_units
-0001fc60: 290a 0a20 2020 2020 2020 2023 2043 7265  )..        # Cre
-0001fc70: 6174 6520 736c 6964 6572 0a20 2020 2020  ate slider.     
-0001fc80: 2020 2073 6c69 6465 7220 3d20 5174 5769     slider = QtWi
-0001fc90: 6467 6574 732e 5153 6c69 6465 7228 0a20  dgets.QSlider(. 
-0001fca0: 2020 2020 2020 2020 2020 206f 7269 656e             orien
-0001fcb0: 7461 7469 6f6e 3d51 7443 6f72 652e 5174  tation=QtCore.Qt
-0001fcc0: 2e48 6f72 697a 6f6e 7461 6c2c 0a20 2020  .Horizontal,.   
-0001fcd0: 2020 2020 2020 2020 2070 6172 656e 743d           parent=
-0001fce0: 626f 745f 626f 7877 6964 6765 740a 2020  bot_boxwidget.  
-0001fcf0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-0001fd00: 2023 2053 6361 6c65 2061 6c6c 2073 6c69   # Scale all sli
-0001fd10: 6465 7220 6e75 6d62 6572 7320 6279 2074  der numbers by t
-0001fd20: 6869 7320 746f 206d 616b 6520 696e 746f  his to make into
-0001fd30: 2066 6c6f 6174 730a 2020 2020 2020 2020   floats.        
-0001fd40: 736c 6964 6572 5f73 6361 6c65 203d 2031  slider_scale = 1
-0001fd50: 4535 0a0a 2020 2020 2020 2020 736c 6964  E5..        slid
-0001fd60: 6572 2e73 6574 4d69 6e69 6d75 6d28 696e  er.setMinimum(in
-0001fd70: 7428 6465 6661 756c 7473 5b27 6d69 6e27  t(defaults['min'
-0001fd80: 5d20 2a20 736c 6964 6572 5f73 6361 6c65  ] * slider_scale
-0001fd90: 2929 0a20 2020 2020 2020 2073 6c69 6465  )).        slide
-0001fda0: 722e 7365 744d 6178 696d 756d 2869 6e74  r.setMaximum(int
-0001fdb0: 2864 6566 6175 6c74 735b 276d 6178 275d  (defaults['max']
-0001fdc0: 202a 2073 6c69 6465 725f 7363 616c 6529   * slider_scale)
-0001fdd0: 290a 2020 2020 2020 2020 736c 6964 6572  ).        slider
-0001fde0: 2e73 6574 5661 6c75 6528 696e 7428 6465  .setValue(int(de
-0001fdf0: 6661 756c 7473 5b27 7661 6c69 6e69 7427  faults['valinit'
-0001fe00: 5d20 2a20 736c 6964 6572 5f73 6361 6c65  ] * slider_scale
-0001fe10: 2929 0a20 2020 2020 2020 2073 6c69 6465  )).        slide
-0001fe20: 722e 7365 7453 696e 676c 6553 7465 7028  r.setSingleStep(
-0001fe30: 696e 7428 6465 6661 756c 7473 5b27 7374  int(defaults['st
-0001fe40: 6570 275d 202a 2073 6c69 6465 725f 7363  ep'] * slider_sc
-0001fe50: 616c 6529 290a 0a20 2020 2020 2020 2073  ale))..        s
-0001fe60: 656c 662e 7769 6467 6574 6469 6374 5b6d  elf.widgetdict[m
-0001fe70: 6f64 656c 6e61 6d65 2e6c 6f77 6572 2829  odelname.lower()
-0001fe80: 5d5b 7061 726e 616d 655d 5b27 736c 6964  ][parname]['slid
-0001fe90: 6572 275d 203d 2073 6c69 6465 720a 0a20  er'] = slider.. 
-0001fea0: 2020 2020 2020 2023 2041 6464 2073 6c69         # Add sli
-0001feb0: 6465 7220 746f 206c 6179 6f75 740a 2020  der to layout.  
-0001fec0: 2020 2020 2020 626f 745f 626f 786c 6179        bot_boxlay
-0001fed0: 6f75 742e 6164 6457 6964 6765 7428 736c  out.addWidget(sl
-0001fee0: 6964 6572 290a 0a20 2020 2020 2020 2023  ider)..        #
-0001fef0: 2043 7265 6174 6520 7465 7874 2065 6e74   Create text ent
-0001ff00: 7279 2028 446f 7562 6c65 5370 696e 426f  ry (DoubleSpinBo
-0001ff10: 7829 0a20 2020 2020 2020 2065 6e74 7279  x).        entry
-0001ff20: 203d 2051 7457 6964 6765 7473 2e51 446f   = QtWidgets.QDo
-0001ff30: 7562 6c65 5370 696e 426f 7828 7061 7265  ubleSpinBox(pare
-0001ff40: 6e74 3d62 6f74 5f62 6f78 7769 6467 6574  nt=bot_boxwidget
-0001ff50: 290a 2020 2020 2020 2020 656e 7472 792e  ).        entry.
-0001ff60: 7365 7444 6563 696d 616c 7328 696e 7428  setDecimals(int(
-0001ff70: 6465 6661 756c 7473 5b27 6465 6369 6d61  defaults['decima
-0001ff80: 6c73 275d 2929 0a20 2020 2020 2020 2065  ls'])).        e
-0001ff90: 6e74 7279 2e73 6574 4275 7474 6f6e 5379  ntry.setButtonSy
-0001ffa0: 6d62 6f6c 7328 5174 5769 6467 6574 732e  mbols(QtWidgets.
-0001ffb0: 5144 6f75 626c 6553 7069 6e42 6f78 2e4e  QDoubleSpinBox.N
-0001ffc0: 6f42 7574 746f 6e73 290a 2020 2020 2020  oButtons).      
-0001ffd0: 2020 656e 7472 792e 7365 744b 6579 626f    entry.setKeybo
-0001ffe0: 6172 6454 7261 636b 696e 6728 4661 6c73  ardTracking(Fals
-0001fff0: 6529 0a20 2020 2020 2020 2065 6e74 7279  e).        entry
-00020000: 2e73 6574 4d69 6e69 6d75 6d28 6465 6661  .setMinimum(defa
-00020010: 756c 7473 5b27 6d69 6e27 5d29 0a20 2020  ults['min']).   
-00020020: 2020 2020 2065 6e74 7279 2e73 6574 4d61       entry.setMa
-00020030: 7869 6d75 6d28 6465 6661 756c 7473 5b27  ximum(defaults['
-00020040: 6d61 7827 5d29 0a20 2020 2020 2020 2065  max']).        e
-00020050: 6e74 7279 2e73 6574 5661 6c75 6528 6465  ntry.setValue(de
-00020060: 6661 756c 7473 5b27 7661 6c69 6e69 7427  faults['valinit'
-00020070: 5d29 0a20 2020 2020 2020 2065 6e74 7279  ]).        entry
-00020080: 2e73 6574 5369 6e67 6c65 5374 6570 2864  .setSingleStep(d
-00020090: 6566 6175 6c74 735b 2773 7465 7027 5d29  efaults['step'])
-000200a0: 0a0a 2020 2020 2020 2020 7365 6c66 2e77  ..        self.w
-000200b0: 6964 6765 7464 6963 745b 6d6f 6465 6c6e  idgetdict[modeln
-000200c0: 616d 652e 6c6f 7765 7228 295d 5b70 6172  ame.lower()][par
-000200d0: 6e61 6d65 5d5b 2765 6e74 7279 275d 203d  name]['entry'] =
-000200e0: 2065 6e74 7279 0a0a 2020 2020 2020 2020   entry..        
-000200f0: 2320 4164 6420 646f 7562 6c65 7370 696e  # Add doublespin
-00020100: 626f 7820 746f 206c 6179 6f75 740a 2020  box to layout.  
-00020110: 2020 2020 2020 626f 745f 626f 786c 6179        bot_boxlay
-00020120: 6f75 742e 6164 6457 6964 6765 7428 656e  out.addWidget(en
-00020130: 7472 7929 0a0a 2020 2020 2020 2020 2320  try)..        # 
-00020140: 4372 6561 7465 2066 6974 2f66 6978 2074  Create fit/fix t
-00020150: 6f67 676c 6520 6275 7474 6f6e 0a20 2020  oggle button.   
-00020160: 2020 2020 2066 665f 746f 6767 6c65 203d       ff_toggle =
-00020170: 2051 7457 6964 6765 7473 2e51 5075 7368   QtWidgets.QPush
-00020180: 4275 7474 6f6e 2827 4672 6565 272c 2070  Button('Free', p
-00020190: 6172 656e 743d 626f 745f 626f 7877 6964  arent=bot_boxwid
-000201a0: 6765 7429 0a0a 2020 2020 2020 2020 7365  get)..        se
-000201b0: 6c66 2e77 6964 6765 7464 6963 745b 6d6f  lf.widgetdict[mo
-000201c0: 6465 6c6e 616d 652e 6c6f 7765 7228 295d  delname.lower()]
-000201d0: 5b70 6172 6e61 6d65 5d5b 2766 665f 746f  [parname]['ff_to
-000201e0: 6767 6c65 275d 203d 2066 665f 746f 6767  ggle'] = ff_togg
-000201f0: 6c65 0a0a 2020 2020 2020 2020 6666 7377  le..        ffsw
-00020200: 203d 207b 0a20 2020 2020 2020 2020 2020   = {.           
-00020210: 2027 4672 6565 273a 2027 4669 7865 6427   'Free': 'Fixed'
-00020220: 2c0a 2020 2020 2020 2020 2020 2020 2746  ,.            'F
-00020230: 6978 6564 273a 2027 4672 6565 272c 0a20  ixed': 'Free',. 
-00020240: 2020 2020 2020 207d 0a0a 2020 2020 2020         }..      
-00020250: 2020 2320 4361 6c6c 6261 636b 2066 6f72    # Callback for
-00020260: 2074 6578 740a 2020 2020 2020 2020 6666   text.        ff
-00020270: 5f74 6f67 676c 652e 636c 6963 6b65 642e  _toggle.clicked.
-00020280: 636f 6e6e 6563 7428 0a20 2020 2020 2020  connect(.       
-00020290: 2020 2020 206c 616d 6264 6120 5f3a 2066       lambda _: f
-000202a0: 665f 746f 6767 6c65 2e73 6574 5465 7874  f_toggle.setText
-000202b0: 2866 6673 775b 6666 5f74 6f67 676c 652e  (ffsw[ff_toggle.
-000202c0: 7465 7874 2829 5d29 0a20 2020 2020 2020  text()]).       
-000202d0: 2029 0a0a 2020 2020 2020 2020 2320 4361   )..        # Ca
-000202e0: 6c6c 6261 636b 2066 6f72 2066 6974 2f66  llback for fit/f
-000202f0: 6978 206f 6620 7468 6973 2070 6172 616d  ix of this param
-00020300: 6574 6572 0a20 2020 2020 2020 2066 665f  eter.        ff_
-00020310: 746f 6767 6c65 2e63 6c69 636b 6564 2e63  toggle.clicked.c
-00020320: 6f6e 6e65 6374 280a 2020 2020 2020 2020  onnect(.        
-00020330: 2020 2020 6c61 6d62 6461 205f 3a20 7365      lambda _: se
-00020340: 6c66 2e6e 6f74 5f69 6679 2870 6172 6e61  lf.not_ify(parna
-00020350: 6d65 290a 2020 2020 2020 2020 290a 0a20  me).        ).. 
-00020360: 2020 2020 2020 2023 2043 6f6e 6e65 6374         # Connect
-00020370: 2066 6974 2f66 6978 2074 6f20 736c 6964   fit/fix to slid
-00020380: 6572 2061 6e64 2074 6578 7465 6e74 7279  er and textentry
-00020390: 0a20 2020 2020 2020 2073 6c69 6465 722e  .        slider.
-000203a0: 7661 6c75 6543 6861 6e67 6564 2e63 6f6e  valueChanged.con
-000203b0: 6e65 6374 286c 616d 6264 6120 7661 6c3a  nect(lambda val:
-000203c0: 2063 6228 7661 6c20 2a20 736c 6964 6572   cb(val * slider
-000203d0: 5f73 6361 6c65 2a2a 2d31 2929 0a20 2020  _scale**-1)).   
-000203e0: 2020 2020 2073 6c69 6465 722e 7661 6c75       slider.valu
-000203f0: 6543 6861 6e67 6564 2e63 6f6e 6e65 6374  eChanged.connect
-00020400: 280a 2020 2020 2020 2020 2020 2020 6c61  (.            la
-00020410: 6d62 6461 2076 616c 3a20 656e 7472 792e  mbda val: entry.
-00020420: 7365 7456 616c 7565 2876 616c 202a 2073  setValue(val * s
-00020430: 6c69 6465 725f 7363 616c 652a 2a2d 3129  lider_scale**-1)
-00020440: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-00020450: 2020 2065 6e74 7279 2e76 616c 7565 4368     entry.valueCh
-00020460: 616e 6765 642e 636f 6e6e 6563 7428 6362  anged.connect(cb
-00020470: 290a 2020 2020 2020 2020 656e 7472 792e  ).        entry.
-00020480: 7661 6c75 6543 6861 6e67 6564 2e63 6f6e  valueChanged.con
-00020490: 6e65 6374 280a 2020 2020 2020 2020 2020  nect(.          
-000204a0: 2020 6c61 6d62 6461 2076 616c 3a20 736c    lambda val: sl
-000204b0: 6964 6572 2e73 6574 5661 6c75 6528 696e  ider.setValue(in
-000204c0: 7428 7661 6c20 2a20 736c 6964 6572 5f73  t(val * slider_s
-000204d0: 6361 6c65 2929 0a20 2020 2020 2020 2029  cale)).        )
-000204e0: 0a0a 2020 2020 2020 2020 2320 4164 6420  ..        # Add 
-000204f0: 6669 742f 6669 7820 746f 206c 6179 6f75  fit/fix to layou
-00020500: 740a 2020 2020 2020 2020 626f 745f 626f  t.        bot_bo
-00020510: 786c 6179 6f75 742e 6164 6457 6964 6765  xlayout.addWidge
-00020520: 7428 6666 5f74 6f67 676c 6529 0a0a 2020  t(ff_toggle)..  
-00020530: 2020 2020 2020 746f 705f 626f 7877 6964        top_boxwid
-00020540: 6765 742e 7365 7453 697a 6550 6f6c 6963  get.setSizePolic
-00020550: 7928 0a20 2020 2020 2020 2020 2020 2051  y(.            Q
-00020560: 7457 6964 6765 7473 2e51 5369 7a65 506f  tWidgets.QSizePo
-00020570: 6c69 6379 2e46 6978 6564 2c0a 2020 2020  licy.Fixed,.    
-00020580: 2020 2020 2020 2020 5174 5769 6467 6574          QtWidget
-00020590: 732e 5153 697a 6550 6f6c 6963 792e 4669  s.QSizePolicy.Fi
-000205a0: 7865 640a 2020 2020 2020 2020 290a 2020  xed.        ).  
-000205b0: 2020 2020 2020 626f 745f 626f 7877 6964        bot_boxwid
-000205c0: 6765 742e 7365 7453 697a 6550 6f6c 6963  get.setSizePolic
-000205d0: 7928 0a20 2020 2020 2020 2020 2020 2051  y(.            Q
-000205e0: 7457 6964 6765 7473 2e51 5369 7a65 506f  tWidgets.QSizePo
-000205f0: 6c69 6379 2e46 6978 6564 2c0a 2020 2020  licy.Fixed,.    
-00020600: 2020 2020 2020 2020 5174 5769 6467 6574          QtWidget
-00020610: 732e 5153 697a 6550 6f6c 6963 792e 4669  s.QSizePolicy.Fi
-00020620: 7865 640a 2020 2020 2020 2020 290a 2020  xed.        ).  
-00020630: 2020 2020 2020 746f 705f 626f 786c 6179        top_boxlay
-00020640: 6f75 742e 7365 7441 6c69 676e 6d65 6e74  out.setAlignment
-00020650: 2851 7443 6f72 652e 5174 2e41 6c69 676e  (QtCore.Qt.Align
-00020660: 4843 656e 7465 7229 0a0a 2020 2020 2020  HCenter)..      
-00020670: 2020 6f6e 655f 7061 7261 6d5f 6c61 796f    one_param_layo
-00020680: 7574 2e61 6464 5769 6467 6574 2874 6f70  ut.addWidget(top
-00020690: 5f62 6f78 7769 6467 6574 290a 2020 2020  _boxwidget).    
-000206a0: 2020 2020 6f6e 655f 7061 7261 6d5f 6c61      one_param_la
-000206b0: 796f 7574 2e61 6464 5769 6467 6574 2862  yout.addWidget(b
-000206c0: 6f74 5f62 6f78 7769 6467 6574 290a 0a20  ot_boxwidget).. 
-000206d0: 2020 2020 2020 206f 6e65 5f70 6172 616d         one_param
-000206e0: 5f6c 6179 6f75 742e 7365 7443 6f6e 7465  _layout.setConte
-000206f0: 6e74 734d 6172 6769 6e73 2830 2c20 302c  ntsMargins(0, 0,
-00020700: 2030 2c20 3029 0a20 2020 2020 2020 206f   0, 0).        o
-00020710: 6e65 5f70 6172 616d 5f6c 6179 6f75 742e  ne_param_layout.
-00020720: 7365 7453 7061 6369 6e67 2832 290a 2020  setSpacing(2).  
-00020730: 2020 2020 2020 6f6e 655f 7061 7261 6d5f        one_param_
-00020740: 6c61 796f 7574 2e61 6464 5374 7265 7463  layout.addStretc
-00020750: 6828 3129 0a20 2020 2020 2020 206f 6e65  h(1).        one
-00020760: 5f70 6172 616d 5f6c 6179 6f75 742e 7365  _param_layout.se
-00020770: 7441 6c69 676e 6d65 6e74 2851 7443 6f72  tAlignment(QtCor
-00020780: 652e 5174 2e41 6c69 676e 5643 656e 7465  e.Qt.AlignVCente
-00020790: 7229 0a0a 2020 2020 2020 2020 7265 7475  r)..        retu
-000207a0: 726e 206f 6e65 5f70 6172 616d 5f77 6964  rn one_param_wid
-000207b0: 6765 742c 206f 6e65 5f70 6172 616d 5f6c  get, one_param_l
-000207c0: 6179 6f75 740a 0a0a 6465 6620 696e 7465  ayout...def inte
-000207d0: 7261 6374 6976 655f 6669 7474 696e 6728  ractive_fitting(
-000207e0: 6461 7461 7365 743a 2054 6175 5444 6174  dataset: TauTDat
-000207f0: 6173 6574 207c 2054 6175 4844 6174 6173  aset | TauHDatas
-00020800: 6574 2c20 6170 702c 0a20 2020 2020 2020  et, app,.       
-00020810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020820: 206d 6f64 656c 5f6f 7074 3a20 7374 7220   model_opt: str 
-00020830: 7c20 6c69 7374 5b4c 6f67 5461 7554 4d6f  | list[LogTauTMo
-00020840: 6465 6c20 7c20 4c6f 6754 6175 484d 6f64  del | LogTauHMod
-00020850: 656c 5d20 3d20 2766 726f 6d5f 6461 7461  el] = 'from_data
-00020860: 7365 7427 2920 2d3e 2074 7570 6c65 5b6c  set') -> tuple[l
-00020870: 6973 745b 4c6f 6754 6175 544d 6f64 656c  ist[LogTauTModel
-00020880: 207c 204c 6f67 5461 7548 4d6f 6465 6c5d   | LogTauHModel]
-00020890: 2c20 6c69 7374 5b64 6963 745b 7374 722c  , list[dict[str,
-000208a0: 2066 6c6f 6174 5d5d 2c20 6c69 7374 5b64   float]], list[d
-000208b0: 6963 745b 7374 722c 2066 6c6f 6174 5d5d  ict[str, float]]
-000208c0: 2c20 626f 6f6c 5d3a 2023 206e 6f71 610a  , bool]: # noqa.
-000208d0: 2020 2020 2727 270a 2020 2020 4372 6561      '''.    Crea
-000208e0: 7465 7320 7174 2077 696e 646f 7720 666f  tes qt window fo
-000208f0: 7220 7573 6572 2074 6f20 696e 7465 7261  r user to intera
-00020900: 6374 6976 656c 7920 6669 7420 6d6f 6465  ctively fit mode
-00020910: 6c73 2074 6f20 7265 6c61 7861 7469 6f6e  ls to relaxation
-00020920: 0a20 2020 2064 6174 610a 0a20 2020 2050  .    data..    P
-00020930: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
-00020940: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2064 6174  --------.    dat
-00020950: 6173 6574 3a20 5461 7554 4461 7461 7365  aset: TauTDatase
-00020960: 7420 7c20 5461 7548 4461 7461 7365 740a  t | TauHDataset.
-00020970: 2020 2020 2020 2020 4461 7461 7365 7420          Dataset 
-00020980: 746f 2070 6c6f 740a 2020 2020 6170 703a  to plot.    app:
-00020990: 2051 7457 6964 6765 7473 2e51 4170 706c   QtWidgets.QAppl
-000209a0: 6963 6174 696f 6e0a 2020 2020 2020 2020  ication.        
-000209b0: 4170 706c 6963 6174 696f 6e20 7573 6564  Application used
-000209c0: 2062 7920 6375 7272 656e 7420 7072 6f67   by current prog
-000209d0: 7261 6d0a 2020 2020 2020 2020 4372 6561  ram.        Crea
-000209e0: 7465 2077 6974 6820 6061 7070 3d51 7457  te with `app=QtW
-000209f0: 6964 6765 7473 2e51 4170 706c 6963 6174  idgets.QApplicat
-00020a00: 696f 6e28 5b5d 2960 0a20 2020 206d 6f64  ion([])`.    mod
-00020a10: 656c 5f6f 7074 3a20 7374 7220 7c20 6c69  el_opt: str | li
-00020a20: 7374 5b4c 6f67 5461 7554 4d6f 6465 6c20  st[LogTauTModel 
-00020a30: 7c20 4c6f 6754 6175 484d 6f64 656c 5d20  | LogTauHModel] 
-00020a40: 6465 6661 756c 7420 2766 726f 6d5f 6461  default 'from_da
-00020a50: 7461 7365 7427 200a 2020 2020 2020 2020  taset' .        
-00020a60: 4c69 7374 206f 6620 6d6f 6465 6c73 2074  List of models t
-00020a70: 6f20 6f66 6665 7220 746f 2075 7365 722c  o offer to user,
-00020a80: 2069 6620 2766 726f 6d5f 6461 7461 7365   if 'from_datase
-00020a90: 7427 2077 696c 6c20 6765 6e65 7261 7465  t' will generate
-00020aa0: 0a20 2020 2020 2020 2061 206c 6973 7420  .        a list 
-00020ab0: 6261 7365 6420 6f6e 2074 6865 2064 6174  based on the dat
-00020ac0: 6173 6574 2070 726f 7669 6465 640a 0a20  aset provided.. 
-00020ad0: 2020 2052 6574 7572 6e73 0a20 2020 202d     Returns.    -
-00020ae0: 2d2d 2d2d 2d2d 0a20 2020 206c 6973 745b  ------.    list[
-00020af0: 4c6f 6754 6175 544d 6f64 656c 207c 204c  LogTauTModel | L
-00020b00: 6f67 5461 7548 4d6f 6465 6c5d 0a20 2020  ogTauHModel].   
-00020b10: 2020 2020 204d 6f64 656c 7320 7365 6c65       Models sele
-00020b20: 6374 6564 2062 7920 7573 6572 0a20 2020  cted by user.   
-00020b30: 206c 6973 745b 6469 6374 5b73 7472 2c20   list[dict[str, 
-00020b40: 666c 6f61 745d 5d0a 2020 2020 2020 2020  float]].        
-00020b50: 6669 745f 7661 7273 2064 6963 7473 2c20  fit_vars dicts, 
-00020b60: 6f6e 6520 7065 7220 6d6f 6465 6c0a 2020  one per model.  
-00020b70: 2020 6c69 7374 5b64 6963 745b 7374 722c    list[dict[str,
-00020b80: 2066 6c6f 6174 5d5d 0a20 2020 2020 2020   float]].       
-00020b90: 2066 6978 5f76 6172 7320 6469 6374 732c   fix_vars dicts,
-00020ba0: 206f 6e65 2070 6572 206d 6f64 656c 0a20   one per model. 
-00020bb0: 2020 2062 6f6f 6c0a 2020 2020 2020 2020     bool.        
-00020bc0: 5472 7565 2069 6620 7573 6572 2068 6173  True if user has
-00020bd0: 2065 7869 7465 6420 7769 6e64 6f77 2069   exited window i
-00020be0: 6e73 7465 6164 206f 6620 6669 7474 696e  nstead of fittin
-00020bf0: 670a 2020 2020 2020 2020 656c 7365 2046  g.        else F
-00020c00: 616c 7365 0a20 2020 2027 2727 2023 206e  alse.    ''' # n
-00020c10: 6f71 610a 0a20 2020 2069 6620 6d6f 6465  oqa..    if mode
-00020c20: 6c5f 6f70 7420 3d3d 2027 6672 6f6d 5f64  l_opt == 'from_d
-00020c30: 6174 6173 6574 273a 0a20 2020 2020 2020  ataset':.       
-00020c40: 2069 6620 6973 696e 7374 616e 6365 2864   if isinstance(d
-00020c50: 6174 6173 6574 2c20 5461 7554 4461 7461  ataset, TauTData
-00020c60: 7365 7429 3a0a 2020 2020 2020 2020 2020  set):.          
-00020c70: 2020 6d6f 6465 6c5f 6f70 7420 3d20 5b0a    model_opt = [.
-00020c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020c90: 4c6f 674f 7262 6163 684d 6f64 656c 2c0a  LogOrbachModel,.
-00020ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020cb0: 4c6f 6752 616d 616e 4d6f 6465 6c2c 0a20  LogRamanModel,. 
-00020cc0: 2020 2020 2020 2020 2020 2020 2020 204c                 L
-00020cd0: 6f67 5154 4d4d 6f64 656c 2c0a 2020 2020  ogQTMModel,.    
-00020ce0: 2020 2020 2020 2020 2020 2020 4c6f 6744              LogD
-00020cf0: 6972 6563 744d 6f64 656c 0a20 2020 2020  irectModel.     
-00020d00: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
-00020d10: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
-00020d20: 2864 6174 6173 6574 2c20 5461 7548 4461  (dataset, TauHDa
-00020d30: 7461 7365 7429 3a0a 2020 2020 2020 2020  taset):.        
-00020d40: 2020 2020 6d6f 6465 6c5f 6f70 7420 3d20      model_opt = 
-00020d50: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
-00020d60: 2020 4c6f 6746 4451 544d 4d6f 6465 6c2c    LogFDQTMModel,
-00020d70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00020d80: 204c 6f67 5261 6d61 6e49 494d 6f64 656c   LogRamanIIModel
-00020d90: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00020da0: 2020 4c6f 6742 5656 5261 6d61 6e49 494d    LogBVVRamanIIM
-00020db0: 6f64 656c 2c0a 2020 2020 2020 2020 2020  odel,.          
-00020dc0: 2020 2020 2020 4c6f 6743 6f6e 7374 616e        LogConstan
-00020dd0: 744d 6f64 656c 2c0a 2020 2020 2020 2020  tModel,.        
-00020de0: 2020 2020 2020 2020 4c6f 6742 5656 436f          LogBVVCo
-00020df0: 6e73 7461 6e74 4d6f 6465 6c2c 0a20 2020  nstantModel,.   
-00020e00: 2020 2020 2020 2020 205d 0a0a 2020 2020           ]..    
-00020e10: 7573 656c 203d 2074 7970 6528 276f 626a  usel = type('obj
-00020e20: 272c 2028 6f62 6a65 6374 2c29 2c20 7b0a  ', (object,), {.
-00020e30: 2020 2020 2020 2020 276d 6f64 656c 7327          'models'
-00020e40: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
-00020e50: 6d6f 6465 6c2e 4e41 4d45 2e6c 6f77 6572  model.NAME.lower
-00020e60: 2829 3a20 4661 6c73 650a 2020 2020 2020  (): False.      
-00020e70: 2020 2020 2020 666f 7220 6d6f 6465 6c20        for model 
-00020e80: 696e 206d 6f64 656c 5f6f 7074 0a20 2020  in model_opt.   
-00020e90: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
-00020ea0: 2766 6974 5f76 6172 7327 3a20 5b5d 2c0a  'fit_vars': [],.
-00020eb0: 2020 2020 2020 2020 2766 6978 5f76 6172          'fix_var
-00020ec0: 7327 3a20 5b5d 2c0a 2020 2020 2020 2020  s': [],.        
-00020ed0: 2766 6978 273a 205b 5d2c 0a20 2020 2020  'fix': [],.     
-00020ee0: 2020 2027 6578 6974 6564 273a 2054 7275     'exited': Tru
-00020ef0: 650a 2020 2020 7d29 0a0a 2020 2020 7061  e.    })..    pa
-00020f00: 7261 6d5f 7769 6e64 6f77 203d 2046 6974  ram_window = Fit
-00020f10: 5769 6e64 6f77 280a 2020 2020 2020 2020  Window(.        
-00020f20: 6461 7461 7365 742c 0a20 2020 2020 2020  dataset,.       
-00020f30: 2075 7365 6c2c 0a20 2020 2020 2020 206d   usel,.        m
-00020f40: 6f64 656c 5f6f 7074 2c0a 2020 2020 2020  odel_opt,.      
-00020f50: 2020 6775 692e 7769 6467 6574 5f64 6566    gui.widget_def
-00020f60: 6175 6c74 730a 2020 2020 290a 2020 2020  aults.    ).    
-00020f70: 7061 7261 6d5f 7769 6e64 6f77 2e73 686f  param_window.sho
-00020f80: 7728 290a 0a20 2020 2061 7070 2e65 7865  w()..    app.exe
-00020f90: 6328 290a 0a20 2020 206e 616d 655f 746f  c()..    name_to
-00020fa0: 5f6d 6f64 656c 203d 207b 0a20 2020 2020  _model = {.     
-00020fb0: 2020 206d 6f64 656c 2e4e 414d 452e 6c6f     model.NAME.lo
-00020fc0: 7765 7228 293a 206d 6f64 656c 0a20 2020  wer(): model.   
-00020fd0: 2020 2020 2066 6f72 206d 6f64 656c 2069       for model i
-00020fe0: 6e20 6d6f 6465 6c5f 6f70 740a 2020 2020  n model_opt.    
-00020ff0: 7d0a 0a20 2020 2072 5f6d 6f64 656c 7320  }..    r_models 
-00021000: 3d20 5b0a 2020 2020 2020 2020 6e61 6d65  = [.        name
-00021010: 5f74 6f5f 6d6f 6465 6c5b 6e61 6d65 5d0a  _to_model[name].
-00021020: 2020 2020 2020 2020 666f 7220 6e61 6d65          for name
-00021030: 2069 6e20 7573 656c 2e6d 6f64 656c 730a   in usel.models.
-00021040: 2020 2020 5d0a 0a20 2020 2072 6574 7572      ]..    retur
-00021050: 6e20 725f 6d6f 6465 6c73 2c20 7573 656c  n r_models, usel
-00021060: 2e66 6974 5f76 6172 732c 2075 7365 6c2e  .fit_vars, usel.
-00021070: 6669 785f 7661 7273 2c20 7573 656c 2e65  fix_vars, usel.e
-00021080: 7869 7465 640a 0a0a 6465 6620 706c 6f74  xited...def plot
-00021090: 5f66 6974 7465 645f 7469 6d65 7328 6461  _fitted_times(da
-000210a0: 7461 7365 743a 2054 6175 5444 6174 6173  taset: TauTDatas
-000210b0: 6574 207c 2054 6175 4844 6174 6173 6574  et | TauHDataset
-000210c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000210d0: 2020 2020 2020 2020 6d6f 6465 6c3a 204c          model: L
-000210e0: 6f67 5461 7554 4d6f 6465 6c20 7c20 4d75  ogTauTModel | Mu
-000210f0: 6c74 694c 6f67 5461 7554 4d6f 6465 6c20  ltiLogTauTModel 
-00021100: 7c20 4c6f 6754 6175 484d 6f64 656c 207c  | LogTauHModel |
-00021110: 204d 756c 7469 4c6f 6754 6175 484d 6f64   MultiLogTauHMod
-00021120: 656c 2c20 2320 6e6f 7161 0a20 2020 2020  el, # noqa.     
-00021130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021140: 2073 686f 773a 2062 6f6f 6c20 3d20 5472   show: bool = Tr
-00021150: 7565 2c20 7361 7665 3a20 626f 6f6c 203d  ue, save: bool =
-00021160: 2046 616c 7365 2c0a 2020 2020 2020 2020   False,.        
-00021170: 2020 2020 2020 2020 2020 2020 2020 7361                sa
-00021180: 7665 5f6e 616d 653a 2073 7472 203d 2027  ve_name: str = '
-00021190: 6669 7474 6564 5f72 6174 6573 2e70 6e67  fitted_rates.png
-000211a0: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
-000211b0: 2020 2020 2020 2020 2076 6572 626f 7365           verbose
-000211c0: 3a20 626f 6f6c 203d 2054 7275 6529 202d  : bool = True) -
-000211d0: 3e20 7475 706c 655b 706c 742e 4669 6775  > tuple[plt.Figu
-000211e0: 7265 2c20 706c 742e 4178 6573 5d3a 0a20  re, plt.Axes]:. 
-000211f0: 2020 2027 2727 0a20 2020 2050 6c6f 7473     '''.    Plots
-00021200: 2065 7870 6572 696d 656e 7461 6c20 616e   experimental an
-00021210: 6420 6669 7474 6564 2028 6d6f 6465 6c29  d fitted (model)
-00021220: 2072 656c 6178 6174 696f 6e20 7261 7465   relaxation rate
-00021230: 2061 735c 6e0a 2020 2020 6c6e 2874 6175   as\n.    ln(tau
-00021240: 2920 7673 2031 2f78 7661 7220 7768 6572  ) vs 1/xvar wher
-00021250: 6520 7876 6172 2069 7320 5420 6f72 2048  e xvar is T or H
-00021260: 2e0a 0a20 2020 2050 6172 616d 6574 6572  ...    Parameter
-00021270: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  s.    ----------
-00021280: 0a20 2020 2064 6174 6173 6574 3a20 5461  .    dataset: Ta
-00021290: 7554 4461 7461 7365 7420 7c20 5461 7548  uTDataset | TauH
-000212a0: 4461 7461 7365 740a 2020 2020 2020 2020  Dataset.        
-000212b0: 4461 7461 7365 7420 746f 2070 6c6f 740a  Dataset to plot.
-000212c0: 2020 2020 6d6f 6465 6c3a 204c 6f67 5461      model: LogTa
-000212d0: 7554 4d6f 6465 6c20 7c20 4d75 6c74 694c  uTModel | MultiL
-000212e0: 6f67 5461 7554 4d6f 6465 6c20 7c20 4c6f  ogTauTModel | Lo
-000212f0: 6754 6175 484d 6f64 656c 207c 204d 756c  gTauHModel | Mul
-00021300: 7469 4c6f 6754 6175 484d 6f64 656c 0a20  tiLogTauHModel. 
-00021310: 2020 2020 2020 204d 6f64 656c 2028 6669         Model (fi
-00021320: 7474 6564 2920 746f 2070 6c6f 740a 2020  tted) to plot.  
-00021330: 2020 7368 6f77 3a20 626f 6f6c 2c20 6465    show: bool, de
-00021340: 6661 756c 7420 5472 7565 0a20 2020 2020  fault True.     
-00021350: 2020 2049 6620 5472 7565 2c20 7368 6f77     If True, show
-00021360: 2070 6c6f 7420 6f6e 2073 6372 6565 6e0a   plot on screen.
-00021370: 2020 2020 7361 7665 3a20 626f 6f6c 2c20      save: bool, 
-00021380: 6465 6661 756c 7420 4661 6c73 650a 2020  default False.  
-00021390: 2020 2020 2020 4966 2054 7275 652c 2073        If True, s
-000213a0: 6176 6520 706c 6f74 2074 6f20 6669 6c65  ave plot to file
-000213b0: 2060 7361 7665 5f6e 616d 6560 0a20 2020   `save_name`.   
-000213c0: 2073 6176 655f 6e61 6d65 3a20 7374 722c   save_name: str,
-000213d0: 2064 6566 6175 6c74 203d 2027 6669 7474   default = 'fitt
-000213e0: 6564 5f72 6174 6573 2e70 6e67 270a 2020  ed_rates.png'.  
-000213f0: 2020 2020 2020 4966 2073 6176 6520 6973        If save is
-00021400: 2054 7275 652c 2077 696c 6c20 7361 7665   True, will save
-00021410: 2070 6c6f 7420 746f 2074 6869 7320 6669   plot to this fi
-00021420: 6c65 6e61 6d65 0a20 2020 2076 6572 626f  lename.    verbo
-00021430: 7365 3a20 626f 6f6c 2c20 6465 6661 756c  se: bool, defaul
-00021440: 7420 5472 7565 0a20 2020 2020 2020 2049  t True.        I
-00021450: 6620 5472 7565 2c20 706c 6f74 2066 696c  f True, plot fil
-00021460: 6520 6c6f 6361 7469 6f6e 2069 7320 7772  e location is wr
-00021470: 6974 7465 6e20 746f 2074 6572 6d69 6e61  itten to termina
-00021480: 6c0a 2020 2020 5265 7475 726e 730a 2020  l.    Returns.  
-00021490: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 706c    -------.    pl
-000214a0: 742e 4669 6775 7265 0a20 2020 2020 2020  t.Figure.       
-000214b0: 204d 6174 706c 6f74 6c69 6220 6669 6775   Matplotlib figu
-000214c0: 7265 206f 626a 6563 740a 2020 2020 706c  re object.    pl
-000214d0: 742e 4178 6573 0a20 2020 2020 2020 204d  t.Axes.        M
-000214e0: 6174 706c 6f74 6c69 6220 6178 6973 206f  atplotlib axis o
-000214f0: 626a 6563 740a 2020 2020 2727 270a 0a20  bject.    '''.. 
-00021500: 2020 2023 2043 7265 6174 6520 6669 6775     # Create figu
-00021510: 7265 2061 6e64 2061 7865 730a 2020 2020  re and axes.    
-00021520: 6669 672c 2061 7820 3d20 706c 742e 7375  fig, ax = plt.su
-00021530: 6270 6c6f 7473 280a 2020 2020 2020 2020  bplots(.        
-00021540: 312c 0a20 2020 2020 2020 2031 2c0a 2020  1,.        1,.  
-00021550: 2020 2020 2020 7368 6172 6578 3d54 7275        sharex=Tru
-00021560: 652c 0a20 2020 2020 2020 2073 6861 7265  e,.        share
-00021570: 793d 5472 7565 2c0a 2020 2020 2020 2020  y=True,.        
-00021580: 6669 6773 697a 653d 2836 2c20 3629 2c0a  figsize=(6, 6),.
-00021590: 2020 2020 2020 2020 6e75 6d3d 2746 6974          num='Fit
-000215a0: 7465 6420 7265 6c61 7861 7469 6f6e 2070  ted relaxation p
-000215b0: 726f 6669 6c65 270a 2020 2020 290a 0a20  rofile'.    ).. 
-000215c0: 2020 205f 706c 6f74 5f66 6974 7465 645f     _plot_fitted_
-000215d0: 7469 6d65 7328 6461 7461 7365 742c 206d  times(dataset, m
-000215e0: 6f64 656c 2c20 6669 672c 2061 7829 0a0a  odel, fig, ax)..
-000215f0: 2020 2020 6669 672e 7469 6768 745f 6c61      fig.tight_la
-00021600: 796f 7574 2829 0a0a 2020 2020 6966 2073  yout()..    if s
-00021610: 686f 773a 0a20 2020 2020 2020 2070 6c74  how:.        plt
-00021620: 2e73 686f 7728 290a 0a20 2020 2069 6620  .show()..    if 
-00021630: 7361 7665 3a0a 2020 2020 2020 2020 6669  save:.        fi
-00021640: 672e 7361 7665 6669 6728 7361 7665 5f6e  g.savefig(save_n
-00021650: 616d 652c 2064 7069 3d35 3030 290a 2020  ame, dpi=500).  
-00021660: 2020 2020 2020 6966 2076 6572 626f 7365        if verbose
-00021670: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00021680: 2069 7369 6e73 7461 6e63 6528 6461 7461   isinstance(data
-00021690: 7365 742c 2028 5461 7554 4461 7461 7365  set, (TauTDatase
-000216a0: 7429 293a 0a20 2020 2020 2020 2020 2020  t)):.           
-000216b0: 2020 2020 205f 7876 6172 203d 2027 5427       _xvar = 'T'
-000216c0: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
-000216d0: 6620 6973 696e 7374 616e 6365 2864 6174  f isinstance(dat
-000216e0: 6173 6574 2c20 2854 6175 4844 6174 6173  aset, (TauHDatas
-000216f0: 6574 2929 3a0a 2020 2020 2020 2020 2020  et)):.          
-00021700: 2020 2020 2020 5f78 7661 7220 3d20 2748        _xvar = 'H
-00021710: 270a 2020 2020 2020 2020 2020 2020 7574  '.            ut
-00021720: 2e63 7072 696e 7428 0a20 2020 2020 2020  .cprint(.       
-00021730: 2020 2020 2020 2020 2066 275c 6e20 4669           f'\n Fi
-00021740: 7474 6564 206c 6e28 cf84 2920 7673 2031  tted ln(..) vs 1
-00021750: 2f7b 5f78 7661 727d 2070 6c6f 7420 7361  /{_xvar} plot sa
-00021760: 7665 6420 746f 205c 6e20 7b73 6176 655f  ved to \n {save_
-00021770: 6e61 6d65 7d5c 6e27 2c20 2320 6e6f 7161  name}\n', # noqa
-00021780: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00021790: 2027 6379 616e 270a 2020 2020 2020 2020   'cyan'.        
-000217a0: 2020 2020 290a 0a20 2020 2072 6574 7572      )..    retur
-000217b0: 6e20 6669 672c 2061 780a 0a0a 6465 6620  n fig, ax...def 
-000217c0: 706c 6f74 5f74 696d 6573 2864 6174 6173  plot_times(datas
-000217d0: 6574 3a20 5461 7554 4461 7461 7365 7420  et: TauTDataset 
-000217e0: 7c20 5461 7548 4461 7461 7365 742c 2073  | TauHDataset, s
-000217f0: 686f 773a 2062 6f6f 6c20 3d20 5472 7565  how: bool = True
-00021800: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00021810: 2073 6176 653a 2062 6f6f 6c20 3d20 4661   save: bool = Fa
-00021820: 6c73 652c 2073 6176 655f 6e61 6d65 3a20  lse, save_name: 
-00021830: 7374 7220 3d20 2772 656c 6178 6174 696f  str = 'relaxatio
-00021840: 6e5f 7469 6d65 732e 706e 6727 2c0a 2020  n_times.png',.  
-00021850: 2020 2020 2020 2020 2020 2020 2076 6572               ver
-00021860: 626f 7365 3a20 626f 6f6c 203d 2054 7275  bose: bool = Tru
-00021870: 6529 202d 3e20 7475 706c 655b 706c 742e  e) -> tuple[plt.
-00021880: 4669 6775 7265 2c20 706c 742e 4178 6573  Figure, plt.Axes
-00021890: 5d3a 0a20 2020 2027 2727 0a20 2020 2050  ]:.    '''.    P
-000218a0: 6c6f 7473 2065 7870 6572 696d 656e 7461  lots experimenta
-000218b0: 6c20 7265 6c61 7861 7469 6f6e 2074 696d  l relaxation tim
-000218c0: 6520 6173 5c6e 0a20 2020 206c 6e28 7461  e as\n.    ln(ta
-000218d0: 7529 2076 7320 312f 7876 6172 2077 6865  u) vs 1/xvar whe
-000218e0: 7265 2078 7661 7220 6973 2054 206f 7220  re xvar is T or 
-000218f0: 482e 0a0a 2020 2020 5061 7261 6d65 7465  H...    Paramete
-00021900: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
-00021910: 2d0a 2020 2020 6461 7461 7365 743a 2054  -.    dataset: T
-00021920: 6175 5444 6174 6173 6574 207c 2054 6175  auTDataset | Tau
-00021930: 4844 6174 6173 6574 0a20 2020 2020 2020  HDataset.       
-00021940: 2044 6174 6173 6574 2074 6f20 706c 6f74   Dataset to plot
-00021950: 0a20 2020 2073 686f 773a 2062 6f6f 6c2c  .    show: bool,
-00021960: 2064 6566 6175 6c74 2054 7275 650a 2020   default True.  
-00021970: 2020 2020 2020 4966 2054 7275 652c 2073        If True, s
-00021980: 686f 7720 706c 6f74 206f 6e20 7363 7265  how plot on scre
-00021990: 656e 0a20 2020 2073 6176 653a 2062 6f6f  en.    save: boo
-000219a0: 6c2c 2064 6566 6175 6c74 2046 616c 7365  l, default False
-000219b0: 0a20 2020 2020 2020 2049 6620 5472 7565  .        If True
-000219c0: 2c20 7361 7665 2070 6c6f 7420 746f 2066  , save plot to f
-000219d0: 696c 6520 6073 6176 655f 6e61 6d65 600a  ile `save_name`.
-000219e0: 2020 2020 7361 7665 5f6e 616d 653a 2073      save_name: s
-000219f0: 7472 2c20 6465 6661 756c 7420 2772 656c  tr, default 'rel
-00021a00: 6178 6174 696f 6e5f 7469 6d65 732e 706e  axation_times.pn
-00021a10: 6727 0a20 2020 2020 2020 2049 6620 7361  g'.        If sa
-00021a20: 7665 2069 7320 5472 7565 2c20 7769 6c6c  ve is True, will
-00021a30: 2073 6176 6520 706c 6f74 2074 6f20 7468   save plot to th
-00021a40: 6973 2066 696c 656e 616d 650a 2020 2020  is filename.    
-00021a50: 7665 7262 6f73 653a 2062 6f6f 6c2c 2064  verbose: bool, d
-00021a60: 6566 6175 6c74 2054 7275 650a 2020 2020  efault True.    
-00021a70: 2020 2020 4966 2054 7275 652c 2070 6c6f      If True, plo
-00021a80: 7420 6669 6c65 206c 6f63 6174 696f 6e20  t file location 
-00021a90: 6973 2077 7269 7474 656e 2074 6f20 7465  is written to te
-00021aa0: 726d 696e 616c 0a0a 2020 2020 5265 7475  rminal..    Retu
-00021ab0: 726e 730a 2020 2020 2d2d 2d2d 2d2d 2d0a  rns.    -------.
-00021ac0: 2020 2020 706c 742e 4669 6775 7265 0a20      plt.Figure. 
-00021ad0: 2020 2020 2020 204d 6174 706c 6f74 6c69         Matplotli
-00021ae0: 6220 6669 6775 7265 206f 626a 6563 740a  b figure object.
-00021af0: 2020 2020 706c 742e 4178 6573 0a20 2020      plt.Axes.   
-00021b00: 2020 2020 204d 6174 706c 6f74 6c69 6220       Matplotlib 
-00021b10: 6178 6973 206f 626a 6563 740a 2020 2020  axis object.    
-00021b20: 2727 270a 0a20 2020 2023 2043 7265 6174  '''..    # Creat
-00021b30: 6520 6669 6775 7265 2061 6e64 2061 7865  e figure and axe
-00021b40: 730a 2020 2020 6669 672c 2061 7820 3d20  s.    fig, ax = 
-00021b50: 706c 742e 7375 6270 6c6f 7473 280a 2020  plt.subplots(.  
-00021b60: 2020 2020 2020 312c 0a20 2020 2020 2020        1,.       
-00021b70: 2031 2c0a 2020 2020 2020 2020 7368 6172   1,.        shar
-00021b80: 6578 3d54 7275 652c 0a20 2020 2020 2020  ex=True,.       
-00021b90: 2073 6861 7265 793d 5472 7565 2c0a 2020   sharey=True,.  
-00021ba0: 2020 2020 2020 6669 6773 697a 653d 2836        figsize=(6
-00021bb0: 2c20 3629 2c0a 2020 2020 2020 2020 6e75  , 6),.        nu
-00021bc0: 6d3d 2746 6974 7465 6420 7265 6c61 7861  m='Fitted relaxa
-00021bd0: 7469 6f6e 2070 726f 6669 6c65 270a 2020  tion profile'.  
-00021be0: 2020 290a 0a20 2020 2069 6620 6973 696e    )..    if isin
-00021bf0: 7374 616e 6365 2864 6174 6173 6574 2c20  stance(dataset, 
-00021c00: 5461 7548 4461 7461 7365 7429 3a0a 2020  TauHDataset):.  
-00021c10: 2020 2020 2020 785f 7661 7273 203d 2064        x_vars = d
-00021c20: 6174 6173 6574 2e66 6965 6c64 730a 2020  ataset.fields.  
-00021c30: 2020 2020 2020 6178 2e73 6574 5f78 6c61        ax.set_xla
-00021c40: 6265 6c28 7227 312f 4820 245c 6c65 6674  bel(r'1/H $\left
-00021c50: 285c 6d61 7468 7265 6775 6c61 727b 4f65  (\mathregular{Oe
-00021c60: 7d5e 5c6d 6174 6872 6567 756c 6172 7b2d  }^\mathregular{-
-00021c70: 317d 5c72 6967 6874 2924 2729 0a20 2020  1}\right)$').   
-00021c80: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
-00021c90: 2864 6174 6173 6574 2c20 5461 7554 4461  (dataset, TauTDa
-00021ca0: 7461 7365 7429 3a0a 2020 2020 2020 2020  taset):.        
-00021cb0: 785f 7661 7273 203d 2064 6174 6173 6574  x_vars = dataset
-00021cc0: 2e74 656d 7065 7261 7475 7265 730a 2020  .temperatures.  
-00021cd0: 2020 2020 2020 6178 2e73 6574 5f78 6c61        ax.set_xla
-00021ce0: 6265 6c28 7227 312f 5420 245c 6c65 6674  bel(r'1/T $\left
-00021cf0: 285c 6d61 7468 7265 6775 6c61 727b 4b7d  (\mathregular{K}
-00021d00: 5e5c 6d61 7468 7265 6775 6c61 727b 2d31  ^\mathregular{-1
-00021d10: 7d5c 7269 6768 7429 2427 290a 0a20 2020  }\right)$')..   
-00021d20: 2023 2041 6464 2075 6e63 6572 7461 696e   # Add uncertain
-00021d30: 7469 6573 2061 7320 6572 726f 7262 6172  ties as errorbar
-00021d40: 730a 2020 2020 6966 206c 656e 2864 6174  s.    if len(dat
-00021d50: 6173 6574 2e72 6174 655f 706d 293a 0a0a  aset.rate_pm):..
-00021d60: 2020 2020 2020 2020 2320 4361 6c63 756c          # Calcul
-00021d70: 6174 6520 7469 6d65 2065 7272 6f72 6261  ate time errorba
-00021d80: 7273 0a20 2020 2020 2020 2074 696d 6573  rs.        times
-00021d90: 203d 2031 2e20 2f20 6461 7461 7365 742e   = 1. / dataset.
-00021da0: 7261 7465 730a 2020 2020 2020 2020 6d69  rates.        mi
-00021db0: 6e5f 7469 6d65 203d 2031 2e20 2f20 2864  n_time = 1. / (d
-00021dc0: 6174 6173 6574 2e72 6174 6573 202b 2064  ataset.rates + d
-00021dd0: 6174 6173 6574 2e72 6174 655f 706d 5b31  ataset.rate_pm[1
-00021de0: 2c20 3a5d 290a 2020 2020 2020 2020 6d61  , :]).        ma
-00021df0: 785f 7469 6d65 203d 2031 2e20 2f20 2864  x_time = 1. / (d
-00021e00: 6174 6173 6574 2e72 6174 6573 202d 2064  ataset.rates - d
-00021e10: 6174 6173 6574 2e72 6174 655f 706d 5b30  ataset.rate_pm[0
-00021e20: 2c20 3a5d 290a 0a20 2020 2020 2020 206c  , :])..        l
-00021e30: 6e5f 6d69 6e5f 7469 6d65 203d 206e 702e  n_min_time = np.
-00021e40: 6c6f 6728 6d69 6e5f 7469 6d65 290a 2020  log(min_time).  
-00021e50: 2020 2020 2020 6c6e 5f6d 6178 5f74 696d        ln_max_tim
-00021e60: 6520 3d20 6e70 2e6c 6f67 286d 6178 5f74  e = np.log(max_t
-00021e70: 696d 6529 0a0a 2020 2020 2020 2020 6c6e  ime)..        ln
-00021e80: 5f74 696d 655f 706c 7573 203d 206c 6e5f  _time_plus = ln_
-00021e90: 6d61 785f 7469 6d65 202d 206e 702e 6c6f  max_time - np.lo
-00021ea0: 6728 7469 6d65 7329 0a20 2020 2020 2020  g(times).       
-00021eb0: 206c 6e5f 7469 6d65 5f6d 696e 7573 203d   ln_time_minus =
-00021ec0: 206e 702e 6c6f 6728 7469 6d65 7329 202d   np.log(times) -
-00021ed0: 206c 6e5f 6d69 6e5f 7469 6d65 0a0a 2020   ln_min_time..  
-00021ee0: 2020 2020 2020 6c6e 7469 6d65 5f6d 7020        lntime_mp 
-00021ef0: 3d20 6e70 2e61 7272 6179 285b 6c6e 5f74  = np.array([ln_t
-00021f00: 696d 655f 6d69 6e75 732c 206c 6e5f 7469  ime_minus, ln_ti
-00021f10: 6d65 5f70 6c75 735d 290a 0a20 2020 2020  me_plus])..     
-00021f20: 2020 2061 782e 6572 726f 7262 6172 280a     ax.errorbar(.
-00021f30: 2020 2020 2020 2020 2020 2020 312e 202f              1. /
-00021f40: 2078 5f76 6172 732c 0a20 2020 2020 2020   x_vars,.       
-00021f50: 2020 2020 206e 702e 6c6f 6728 7469 6d65       np.log(time
-00021f60: 7329 2c0a 2020 2020 2020 2020 2020 2020  s),.            
-00021f70: 7965 7272 3d6c 6e74 696d 655f 6d70 2c0a  yerr=lntime_mp,.
-00021f80: 2020 2020 2020 2020 2020 2020 6d61 726b              mark
-00021f90: 6572 3d27 6f27 2c0a 2020 2020 2020 2020  er='o',.        
-00021fa0: 2020 2020 6c77 3d30 2c0a 2020 2020 2020      lw=0,.      
-00021fb0: 2020 2020 2020 656c 696e 6577 6964 7468        elinewidth
-00021fc0: 3d31 2e35 2c0a 2020 2020 2020 2020 2020  =1.5,.          
-00021fd0: 2020 6669 6c6c 7374 796c 653d 276e 6f6e    fillstyle='non
-00021fe0: 6527 2c0a 2020 2020 2020 2020 2020 2020  e',.            
-00021ff0: 636f 6c6f 723d 2762 6c61 636b 270a 2020  color='black'.  
-00022000: 2020 2020 2020 290a 2020 2020 656c 7365        ).    else
-00022010: 3a0a 2020 2020 2020 2020 6178 2e70 6c6f  :.        ax.plo
-00022020: 7428 0a20 2020 2020 2020 2020 2020 2031  t(.            1
-00022030: 2e20 2f20 785f 7661 7273 2c0a 2020 2020  . / x_vars,.    
-00022040: 2020 2020 2020 2020 6e70 2e6c 6f67 2831          np.log(1
-00022050: 2e20 2f20 6461 7461 7365 742e 7261 7465  . / dataset.rate
-00022060: 7329 2c0a 2020 2020 2020 2020 2020 2020  s),.            
-00022070: 6d61 726b 6572 3d27 6f27 2c0a 2020 2020  marker='o',.    
-00022080: 2020 2020 2020 2020 6c77 3d30 2c0a 2020          lw=0,.  
-00022090: 2020 2020 2020 2020 2020 6669 6c6c 7374            fillst
-000220a0: 796c 653d 276e 6f6e 6527 2c0a 2020 2020  yle='none',.    
-000220b0: 2020 2020 2020 2020 636f 6c6f 723d 2762          color='b
-000220c0: 6c61 636b 270a 2020 2020 2020 2020 290a  lack'.        ).
-000220d0: 0a20 2020 2023 2045 6e61 626c 6520 6d69  .    # Enable mi
-000220e0: 6e6f 7220 7469 636b 730a 2020 2020 6178  nor ticks.    ax
-000220f0: 2e79 6178 6973 2e73 6574 5f6d 696e 6f72  .yaxis.set_minor
-00022100: 5f6c 6f63 6174 6f72 2841 7574 6f4d 696e  _locator(AutoMin
-00022110: 6f72 4c6f 6361 746f 7228 2929 0a20 2020  orLocator()).   
-00022120: 2061 782e 7861 7869 732e 7365 745f 6d69   ax.xaxis.set_mi
-00022130: 6e6f 725f 6c6f 6361 746f 7228 4175 746f  nor_locator(Auto
-00022140: 4d69 6e6f 724c 6f63 6174 6f72 2829 290a  MinorLocator()).
-00022150: 0a20 2020 2061 782e 7365 745f 796c 6162  .    ax.set_ylab
-00022160: 656c 2872 2724 5c6c 6e5c 6c65 6674 5b5c  el(r'$\ln\left[\
-00022170: 7461 755c 7269 6768 745d 2420 245c 6c65  tau\right]$ $\le
-00022180: 6674 285c 6c6e 5c6c 6566 745b 5c6d 6174  ft(\ln\left[\mat
-00022190: 6872 6567 756c 6172 7b73 7d5e 5c6d 6174  hregular{s}^\mat
-000221a0: 6872 6567 756c 6172 7b2d 317d 5c72 6967  hregular{-1}\rig
-000221b0: 6874 5d5c 7269 6768 7429 2427 2920 2320  ht]\right)$') # 
-000221c0: 6e6f 7161 0a0a 2020 2020 6669 672e 7469  noqa..    fig.ti
-000221d0: 6768 745f 6c61 796f 7574 2829 0a0a 2020  ght_layout()..  
-000221e0: 2020 6966 2073 686f 773a 0a20 2020 2020    if show:.     
-000221f0: 2020 2070 6c74 2e73 686f 7728 290a 0a20     plt.show().. 
-00022200: 2020 2069 6620 7361 7665 3a0a 2020 2020     if save:.    
-00022210: 2020 2020 6669 672e 7361 7665 6669 6728      fig.savefig(
-00022220: 7361 7665 5f6e 616d 652c 2064 7069 3d35  save_name, dpi=5
-00022230: 3030 290a 2020 2020 2020 2020 6966 2076  00).        if v
-00022240: 6572 626f 7365 3a0a 2020 2020 2020 2020  erbose:.        
-00022250: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-00022260: 6528 6461 7461 7365 742c 2028 5461 7554  e(dataset, (TauT
-00022270: 4461 7461 7365 7429 293a 0a20 2020 2020  Dataset)):.     
-00022280: 2020 2020 2020 2020 2020 205f 7876 6172             _xvar
-00022290: 203d 2027 5427 0a20 2020 2020 2020 2020   = 'T'.         
-000222a0: 2020 2065 6c69 6620 6973 696e 7374 616e     elif isinstan
-000222b0: 6365 2864 6174 6173 6574 2c20 2854 6175  ce(dataset, (Tau
-000222c0: 4844 6174 6173 6574 2929 3a0a 2020 2020  HDataset)):.    
-000222d0: 2020 2020 2020 2020 2020 2020 5f78 7661              _xva
-000222e0: 7220 3d20 2748 270a 2020 2020 2020 2020  r = 'H'.        
-000222f0: 2020 2020 7574 2e63 7072 696e 7428 0a20      ut.cprint(. 
-00022300: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00022310: 275c 6e20 4669 7474 6564 206c 6e28 7461  '\n Fitted ln(ta
-00022320: 7529 2076 7320 312f 7b5f 7876 6172 7d20  u) vs 1/{_xvar} 
-00022330: 706c 6f74 2073 6176 6564 2074 6f20 5c6e  plot saved to \n
-00022340: 207b 7361 7665 5f6e 616d 657d 5c6e 272c   {save_name}\n',
-00022350: 2023 206e 6f71 610a 2020 2020 2020 2020   # noqa.        
-00022360: 2020 2020 2020 2020 2763 7961 6e27 0a20          'cyan'. 
-00022370: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
-00022380: 2020 7265 7475 726e 2066 6967 2c20 6178    return fig, ax
-00022390: 0a0a 0a64 6566 205f 706c 6f74 5f66 6974  ...def _plot_fit
-000223a0: 7465 645f 7469 6d65 7328 6461 7461 7365  ted_times(datase
-000223b0: 743a 2054 6175 5444 6174 6173 6574 207c  t: TauTDataset |
-000223c0: 2054 6175 4844 6174 6173 6574 2c0a 2020   TauHDataset,.  
-000223d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000223e0: 2020 2020 206d 6f64 656c 3a20 4c6f 6754       model: LogT
-000223f0: 6175 544d 6f64 656c 207c 204d 756c 7469  auTModel | Multi
-00022400: 4c6f 6754 6175 544d 6f64 656c 207c 204c  LogTauTModel | L
-00022410: 6f67 5461 7548 4d6f 6465 6c20 7c20 4d75  ogTauHModel | Mu
-00022420: 6c74 694c 6f67 5461 7548 4d6f 6465 6c2c  ltiLogTauHModel,
-00022430: 2023 206e 6f71 610a 2020 2020 2020 2020   # noqa.        
-00022440: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00022450: 6967 3a20 706c 742e 4669 6775 7265 2c20  ig: plt.Figure, 
-00022460: 6178 3a20 706c 742e 4178 6573 293a 0a20  ax: plt.Axes):. 
-00022470: 2020 2027 2727 0a20 2020 2050 6c6f 7473     '''.    Plots
-00022480: 2065 7870 6572 696d 656e 7461 6c20 616e   experimental an
-00022490: 6420 6669 7474 6564 2028 6d6f 6465 6c29  d fitted (model)
-000224a0: 2072 656c 6178 6174 696f 6e20 7261 7465   relaxation rate
-000224b0: 2061 735c 6e0a 2020 2020 6c6e 2874 6175   as\n.    ln(tau
-000224c0: 2920 7673 2031 2f78 7661 7220 7768 6572  ) vs 1/xvar wher
-000224d0: 6520 7876 6172 2069 7320 5420 6f72 2048  e xvar is T or H
-000224e0: 2e0a 0a20 2020 2050 6172 616d 6574 6572  ...    Parameter
-000224f0: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  s.    ----------
-00022500: 0a20 2020 2064 6174 6173 6574 3a20 5461  .    dataset: Ta
-00022510: 7554 4461 7461 7365 7420 7c20 5461 7548  uTDataset | TauH
-00022520: 4461 7461 7365 740a 2020 2020 2020 2020  Dataset.        
-00022530: 4461 7461 7365 7420 746f 2070 6c6f 740a  Dataset to plot.
-00022540: 2020 2020 6d6f 6465 6c3a 204c 6f67 5461      model: LogTa
-00022550: 7554 4d6f 6465 6c20 7c20 4d75 6c74 694c  uTModel | MultiL
-00022560: 6f67 5461 7554 4d6f 6465 6c20 7c20 4c6f  ogTauTModel | Lo
-00022570: 6754 6175 484d 6f64 656c 207c 204d 756c  gTauHModel | Mul
-00022580: 7469 4c6f 6754 6175 484d 6f64 656c 0a20  tiLogTauHModel. 
-00022590: 2020 2020 2020 204d 6f64 656c 2028 6669         Model (fi
-000225a0: 7474 6564 2920 746f 2070 6c6f 740a 2020  tted) to plot.  
-000225b0: 2020 6669 673a 2070 6c74 2e46 6967 7572    fig: plt.Figur
-000225c0: 650a 2020 2020 2020 2020 4d61 7470 6c6f  e.        Matplo
-000225d0: 746c 6962 2046 6967 7572 6520 6f62 6a65  tlib Figure obje
-000225e0: 6374 2075 7365 6420 666f 7220 706c 6f74  ct used for plot
-000225f0: 0a20 2020 2061 783a 2070 6c74 2e41 7865  .    ax: plt.Axe
-00022600: 730a 2020 2020 2020 2020 4d61 7470 6c6f  s.        Matplo
-00022610: 746c 6962 2041 7869 7320 6f62 6a65 6374  tlib Axis object
-00022620: 2075 7365 6420 666f 7220 706c 6f74 0a0a   used for plot..
-00022630: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-00022640: 2d2d 2d2d 2d2d 2d0a 2020 2020 4e6f 6e65  -------.    None
-00022650: 0a20 2020 2027 2727 0a0a 2020 2020 6966  .    '''..    if
-00022660: 2069 7369 6e73 7461 6e63 6528 6461 7461   isinstance(data
-00022670: 7365 742c 2054 6175 4844 6174 6173 6574  set, TauHDataset
-00022680: 293a 0a20 2020 2020 2020 2078 5f76 6172  ):.        x_var
-00022690: 7320 3d20 6461 7461 7365 742e 6669 656c  s = dataset.fiel
-000226a0: 6473 0a20 2020 2020 2020 2061 782e 7365  ds.        ax.se
-000226b0: 745f 786c 6162 656c 2872 2731 2f48 2024  t_xlabel(r'1/H $
-000226c0: 5c6c 6566 7428 5c6d 6174 6872 6567 756c  \left(\mathregul
-000226d0: 6172 7b4f 657d 5e5c 6d61 7468 7265 6775  ar{Oe}^\mathregu
-000226e0: 6c61 727b 2d31 7d5c 7269 6768 7429 2427  lar{-1}\right)$'
-000226f0: 290a 2020 2020 656c 6966 2069 7369 6e73  ).    elif isins
-00022700: 7461 6e63 6528 6461 7461 7365 742c 2054  tance(dataset, T
-00022710: 6175 5444 6174 6173 6574 293a 0a20 2020  auTDataset):.   
-00022720: 2020 2020 2078 5f76 6172 7320 3d20 6461       x_vars = da
-00022730: 7461 7365 742e 7465 6d70 6572 6174 7572  taset.temperatur
-00022740: 6573 0a20 2020 2020 2020 2061 782e 7365  es.        ax.se
-00022750: 745f 786c 6162 656c 2872 2731 2f54 2024  t_xlabel(r'1/T $
-00022760: 5c6c 6566 7428 5c6d 6174 6872 6567 756c  \left(\mathregul
-00022770: 6172 7b4b 7d5e 5c6d 6174 6872 6567 756c  ar{K}^\mathregul
-00022780: 6172 7b2d 317d 5c72 6967 6874 2924 2729  ar{-1}\right)$')
-00022790: 0a0a 2020 2020 2320 4164 6420 756e 6365  ..    # Add unce
-000227a0: 7274 6169 6e74 6965 7320 6173 2065 7272  rtainties as err
-000227b0: 6f72 6261 7273 0a20 2020 2069 6620 6c65  orbars.    if le
-000227c0: 6e28 6461 7461 7365 742e 7261 7465 5f70  n(dataset.rate_p
-000227d0: 6d29 3a0a 0a20 2020 2020 2020 2023 2043  m):..        # C
-000227e0: 616c 6375 6c61 7465 2074 696d 6520 6572  alculate time er
-000227f0: 726f 7262 6172 730a 2020 2020 2020 2020  rorbars.        
-00022800: 7469 6d65 7320 3d20 312e 202f 2064 6174  times = 1. / dat
-00022810: 6173 6574 2e72 6174 6573 0a20 2020 2020  aset.rates.     
-00022820: 2020 206d 696e 5f74 696d 6520 3d20 312e     min_time = 1.
-00022830: 202f 2028 6461 7461 7365 742e 7261 7465   / (dataset.rate
-00022840: 7320 2b20 6461 7461 7365 742e 7261 7465  s + dataset.rate
-00022850: 5f70 6d5b 312c 203a 5d29 0a20 2020 2020  _pm[1, :]).     
-00022860: 2020 206d 6178 5f74 696d 6520 3d20 312e     max_time = 1.
-00022870: 202f 2028 6461 7461 7365 742e 7261 7465   / (dataset.rate
-00022880: 7320 2d20 6461 7461 7365 742e 7261 7465  s - dataset.rate
-00022890: 5f70 6d5b 302c 203a 5d29 0a0a 2020 2020  _pm[0, :])..    
-000228a0: 2020 2020 6c6e 5f6d 696e 5f74 696d 6520      ln_min_time 
-000228b0: 3d20 6e70 2e6c 6f67 286d 696e 5f74 696d  = np.log(min_tim
-000228c0: 6529 0a20 2020 2020 2020 206c 6e5f 6d61  e).        ln_ma
-000228d0: 785f 7469 6d65 203d 206e 702e 6c6f 6728  x_time = np.log(
-000228e0: 6d61 785f 7469 6d65 290a 0a20 2020 2020  max_time)..     
-000228f0: 2020 206c 6e5f 7469 6d65 5f70 6c75 7320     ln_time_plus 
-00022900: 3d20 6c6e 5f6d 6178 5f74 696d 6520 2d20  = ln_max_time - 
-00022910: 6e70 2e6c 6f67 2874 696d 6573 290a 2020  np.log(times).  
-00022920: 2020 2020 2020 6c6e 5f74 696d 655f 6d69        ln_time_mi
-00022930: 6e75 7320 3d20 6e70 2e6c 6f67 2874 696d  nus = np.log(tim
-00022940: 6573 2920 2d20 6c6e 5f6d 696e 5f74 696d  es) - ln_min_tim
-00022950: 650a 0a20 2020 2020 2020 206c 6e74 696d  e..        lntim
-00022960: 655f 6d70 203d 206e 702e 6172 7261 7928  e_mp = np.array(
-00022970: 5b6c 6e5f 7469 6d65 5f6d 696e 7573 2c20  [ln_time_minus, 
-00022980: 6c6e 5f74 696d 655f 706c 7573 5d29 0a0a  ln_time_plus])..
-00022990: 2020 2020 2020 2020 6178 2e65 7272 6f72          ax.error
-000229a0: 6261 7228 0a20 2020 2020 2020 2020 2020  bar(.           
-000229b0: 2031 2e20 2f20 785f 7661 7273 2c0a 2020   1. / x_vars,.  
-000229c0: 2020 2020 2020 2020 2020 6e70 2e6c 6f67            np.log
-000229d0: 2874 696d 6573 292c 0a20 2020 2020 2020  (times),.       
-000229e0: 2020 2020 2079 6572 723d 6c6e 7469 6d65       yerr=lntime
-000229f0: 5f6d 702c 0a20 2020 2020 2020 2020 2020  _mp,.           
-00022a00: 206d 6172 6b65 723d 276f 272c 0a20 2020   marker='o',.   
-00022a10: 2020 2020 2020 2020 206c 773d 302c 0a20           lw=0,. 
-00022a20: 2020 2020 2020 2020 2020 2065 6c69 6e65             eline
-00022a30: 7769 6474 683d 312e 352c 0a20 2020 2020  width=1.5,.     
-00022a40: 2020 2020 2020 2066 696c 6c73 7479 6c65         fillstyle
-00022a50: 3d27 6e6f 6e65 272c 0a20 2020 2020 2020  ='none',.       
-00022a60: 2020 2020 206c 6162 656c 3d27 4578 7065       label='Expe
-00022a70: 7269 6d65 6e74 272c 0a20 2020 2020 2020  riment',.       
-00022a80: 2020 2020 2063 6f6c 6f72 3d27 626c 6163       color='blac
-00022a90: 6b27 0a20 2020 2020 2020 2029 0a20 2020  k'.        ).   
-00022aa0: 2065 6c73 653a 0a20 2020 2020 2020 2061   else:.        a
-00022ab0: 782e 706c 6f74 280a 2020 2020 2020 2020  x.plot(.        
-00022ac0: 2020 2020 312e 202f 2078 5f76 6172 732c      1. / x_vars,
-00022ad0: 0a20 2020 2020 2020 2020 2020 206e 702e  .            np.
-00022ae0: 6c6f 6728 312e 202f 2064 6174 6173 6574  log(1. / dataset
-00022af0: 2e72 6174 6573 292c 0a20 2020 2020 2020  .rates),.       
-00022b00: 2020 2020 206d 6172 6b65 723d 276f 272c       marker='o',
-00022b10: 0a20 2020 2020 2020 2020 2020 206c 773d  .            lw=
-00022b20: 302c 0a20 2020 2020 2020 2020 2020 2066  0,.            f
-00022b30: 696c 6c73 7479 6c65 3d27 6e6f 6e65 272c  illstyle='none',
-00022b40: 0a20 2020 2020 2020 2020 2020 206c 6162  .            lab
-00022b50: 656c 3d27 4578 7065 7269 6d65 6e74 272c  el='Experiment',
-00022b60: 0a20 2020 2020 2020 2020 2020 2063 6f6c  .            col
-00022b70: 6f72 3d27 626c 6163 6b27 0a20 2020 2020  or='black'.     
-00022b80: 2020 2029 0a0a 2020 2020 785f 7661 7273     )..    x_vars
-00022b90: 5f67 7269 6420 3d20 6e70 2e6c 6f67 7370  _grid = np.logsp
-00022ba0: 6163 6528 0a20 2020 2020 2020 206e 702e  ace(.        np.
-00022bb0: 6c6f 6731 3028 6e70 2e6d 696e 2878 5f76  log10(np.min(x_v
-00022bc0: 6172 7329 292c 0a20 2020 2020 2020 206e  ars)),.        n
-00022bd0: 702e 6c6f 6731 3028 6e70 2e6d 6178 2878  p.log10(np.max(x
-00022be0: 5f76 6172 7329 292c 0a20 2020 2020 2020  _vars)),.       
-00022bf0: 2035 3030 0a20 2020 2029 0a0a 2020 2020   500.    )..    
-00022c00: 6966 2074 7970 6528 6d6f 6465 6c29 2069  if type(model) i
-00022c10: 6e20 5b4d 756c 7469 4c6f 6754 6175 544d  n [MultiLogTauTM
-00022c20: 6f64 656c 2c20 4d75 6c74 694c 6f67 5461  odel, MultiLogTa
-00022c30: 7548 4d6f 6465 6c5d 3a0a 2020 2020 2020  uHModel]:.      
-00022c40: 2020 6c6f 676d 6f64 656c 7320 3d20 6d6f    logmodels = mo
-00022c50: 6465 6c2e 6c6f 676d 6f64 656c 730a 2020  del.logmodels.  
-00022c60: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00022c70: 6c6f 676d 6f64 656c 7320 3d20 5b6d 6f64  logmodels = [mod
-00022c80: 656c 5d0a 0a20 2020 2066 6f72 206c 6f67  el]..    for log
-00022c90: 6d6f 6465 6c20 696e 206c 6f67 6d6f 6465  model in logmode
-00022ca0: 6c73 3a0a 0a20 2020 2020 2020 2069 6620  ls:..        if 
-00022cb0: 7479 7065 286c 6f67 6d6f 6465 6c29 2069  type(logmodel) i
-00022cc0: 7320 4c6f 674f 7262 6163 684d 6f64 656c  s LogOrbachModel
-00022cd0: 3a0a 2020 2020 2020 2020 2020 2020 6c61  :.            la
-00022ce0: 6265 6c5f 6669 7420 3d20 275c 6e46 6974  bel_fit = '\nFit
-00022cf0: 2077 6974 6827 0a20 2020 2020 2020 2020   with'.         
-00022d00: 2020 206c 6162 656c 5f66 6974 202b 3d20     label_fit += 
-00022d10: 275c 6e27 202b 2072 277b 7d20 7b3a 362e  '\n' + r'{} {:6.
-00022d20: 3266 7d20 7327 2e66 6f72 6d61 7428 0a20  2f} s'.format(. 
-00022d30: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00022d40: 6f67 6d6f 6465 6c2e 5641 524e 414d 4553  ogmodel.VARNAMES
-00022d50: 5f4d 4d5b 2775 5f65 6666 275d 2c0a 2020  _MM['u_eff'],.  
-00022d60: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-00022d70: 676d 6f64 656c 2e66 696e 616c 5f76 6172  gmodel.final_var
-00022d80: 5f76 616c 7565 735b 2775 5f65 6666 275d  _values['u_eff']
-00022d90: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-00022da0: 2020 2020 2020 2020 2020 206c 6162 656c             label
-00022db0: 5f66 6974 202b 3d20 275c 6e27 202b 2072  _fit += '\n' + r
-00022dc0: 277b 7d20 7b3a 3034 2e33 657d 272e 666f  '{} {:04.3e}'.fo
-00022dd0: 726d 6174 280a 2020 2020 2020 2020 2020  rmat(.          
-00022de0: 2020 2020 2020 6c6f 676d 6f64 656c 2e56        logmodel.V
-00022df0: 4152 4e41 4d45 535f 4d4d 5b27 4127 5d2c  ARNAMES_MM['A'],
-00022e00: 206c 6f67 6d6f 6465 6c2e 6669 6e61 6c5f   logmodel.final_
-00022e10: 7661 725f 7661 6c75 6573 5b27 4127 5d0a  var_values['A'].
-00022e20: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00022e30: 2020 2020 2020 656c 6966 2074 7970 6528        elif type(
-00022e40: 6c6f 676d 6f64 656c 2920 6973 204c 6f67  logmodel) is Log
-00022e50: 5261 6d61 6e4d 6f64 656c 3a0a 2020 2020  RamanModel:.    
-00022e60: 2020 2020 2020 2020 6c61 6265 6c5f 6669          label_fi
-00022e70: 7420 3d20 275c 6e46 6974 2077 6974 6827  t = '\nFit with'
-00022e80: 0a20 2020 2020 2020 2020 2020 206c 6162  .            lab
-00022e90: 656c 5f66 6974 202b 3d20 275c 6e27 202b  el_fit += '\n' +
-00022ea0: 2072 277b 7d20 7b3a 362e 3266 7d20 7327   r'{} {:6.2f} s'
-00022eb0: 2e66 6f72 6d61 7428 0a20 2020 2020 2020  .format(.       
-00022ec0: 2020 2020 2020 2020 206c 6f67 6d6f 6465           logmode
-00022ed0: 6c2e 5641 524e 414d 4553 5f4d 4d5b 2752  l.VARNAMES_MM['R
-00022ee0: 275d 2c20 6c6f 676d 6f64 656c 2e66 696e  '], logmodel.fin
-00022ef0: 616c 5f76 6172 5f76 616c 7565 735b 2752  al_var_values['R
-00022f00: 275d 0a20 2020 2020 2020 2020 2020 2029  '].            )
-00022f10: 0a20 2020 2020 2020 2020 2020 206c 6162  .            lab
-00022f20: 656c 5f66 6974 202b 3d20 275c 6e27 202b  el_fit += '\n' +
-00022f30: 2072 277b 7d20 7b3a 3034 2e33 657d 272e   r'{} {:04.3e}'.
-00022f40: 666f 726d 6174 280a 2020 2020 2020 2020  format(.        
-00022f50: 2020 2020 2020 2020 6c6f 676d 6f64 656c          logmodel
-00022f60: 2e56 4152 4e41 4d45 535f 4d4d 5b27 6e27  .VARNAMES_MM['n'
-00022f70: 5d2c 206c 6f67 6d6f 6465 6c2e 6669 6e61  ], logmodel.fina
-00022f80: 6c5f 7661 725f 7661 6c75 6573 5b27 6e27  l_var_values['n'
-00022f90: 5d0a 2020 2020 2020 2020 2020 2020 290a  ].            ).
-00022fa0: 2020 2020 2020 2020 656c 6966 2074 7970          elif typ
-00022fb0: 6528 6c6f 676d 6f64 656c 2920 6973 204c  e(logmodel) is L
-00022fc0: 6f67 5154 4d4d 6f64 656c 3a0a 2020 2020  ogQTMModel:.    
-00022fd0: 2020 2020 2020 2020 6c61 6265 6c5f 6669          label_fi
-00022fe0: 7420 3d20 275c 6e46 6974 2077 6974 6827  t = '\nFit with'
-00022ff0: 0a20 2020 2020 2020 2020 2020 206c 6162  .            lab
-00023000: 656c 5f66 6974 202b 3d20 275c 6e27 202b  el_fit += '\n' +
-00023010: 2072 277b 7d20 7b3a 362e 3266 7d20 7327   r'{} {:6.2f} s'
-00023020: 2e66 6f72 6d61 7428 0a20 2020 2020 2020  .format(.       
-00023030: 2020 2020 2020 2020 206c 6f67 6d6f 6465           logmode
-00023040: 6c2e 5641 524e 414d 4553 5f4d 4d5b 2751  l.VARNAMES_MM['Q
-00023050: 275d 2c20 6c6f 676d 6f64 656c 2e66 696e  '], logmodel.fin
-00023060: 616c 5f76 6172 5f76 616c 7565 735b 2751  al_var_values['Q
-00023070: 275d 0a20 2020 2020 2020 2020 2020 2029  '].            )
-00023080: 0a20 2020 2020 2020 2065 6c69 6620 7479  .        elif ty
-00023090: 7065 286c 6f67 6d6f 6465 6c29 2069 7320  pe(logmodel) is 
-000230a0: 4c6f 6744 6972 6563 744d 6f64 656c 3a0a  LogDirectModel:.
-000230b0: 2020 2020 2020 2020 2020 2020 6c61 6265              labe
-000230c0: 6c5f 6669 7420 3d20 275c 6e46 6974 2077  l_fit = '\nFit w
-000230d0: 6974 6827 0a20 2020 2020 2020 2020 2020  ith'.           
-000230e0: 206c 6162 656c 5f66 6974 202b 3d20 275c   label_fit += '\
-000230f0: 6e27 202b 2072 277b 7d20 7b3a 362e 3266  n' + r'{} {:6.2f
-00023100: 7d20 7327 2e66 6f72 6d61 7428 0a20 2020  } s'.format(.   
-00023110: 2020 2020 2020 2020 2020 2020 206c 6f67               log
-00023120: 6d6f 6465 6c2e 5641 524e 414d 4553 5f4d  model.VARNAMES_M
-00023130: 4d5b 2744 275d 2c20 6c6f 676d 6f64 656c  M['D'], logmodel
-00023140: 2e66 696e 616c 5f76 6172 5f76 616c 7565  .final_var_value
-00023150: 735b 2744 275d 0a20 2020 2020 2020 2020  s['D'].         
-00023160: 2020 2029 0a20 2020 2020 2020 206d 6f64     ).        mod
-00023170: 656c 5f72 6174 6573 203d 2031 302a 2a6c  el_rates = 10**l
-00023180: 6f67 6d6f 6465 6c2e 6d6f 6465 6c28 0a20  ogmodel.model(. 
-00023190: 2020 2020 2020 2020 2020 206c 6f67 6d6f             logmo
-000231a0: 6465 6c2e 6669 6e61 6c5f 7661 725f 7661  del.final_var_va
-000231b0: 6c75 6573 2c0a 2020 2020 2020 2020 2020  lues,.          
-000231c0: 2020 785f 7661 7273 5f67 7269 642c 0a20    x_vars_grid,. 
-000231d0: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-000231e0: 2020 2320 5472 696d 206d 6f64 656c 2072    # Trim model r
-000231f0: 6174 6573 2074 6f20 7365 6e73 6962 6c65  ates to sensible
-00023200: 2076 616c 7565 730a 2020 2020 2020 2020   values.        
-00023210: 7661 6c69 645f 696e 7420 3d20 6e70 2e77  valid_int = np.w
-00023220: 6865 7265 286d 6f64 656c 5f72 6174 6573  here(model_rates
-00023230: 203e 2031 452d 3629 5b30 5d0a 0a20 2020   > 1E-6)[0]..   
-00023240: 2020 2020 2061 782e 706c 6f74 280a 2020       ax.plot(.  
-00023250: 2020 2020 2020 2020 2020 312e 202f 206e            1. / n
-00023260: 702e 6172 7261 7928 785f 7661 7273 5f67  p.array(x_vars_g
-00023270: 7269 6429 5b76 616c 6964 5f69 6e74 5d2c  rid)[valid_int],
-00023280: 0a20 2020 2020 2020 2020 2020 206e 702e  .            np.
-00023290: 6c6f 6728 312e 202f 206e 702e 6172 7261  log(1. / np.arra
-000232a0: 7928 6d6f 6465 6c5f 7261 7465 7329 5b76  y(model_rates)[v
-000232b0: 616c 6964 5f69 6e74 5d29 2c0a 2020 2020  alid_int]),.    
-000232c0: 2020 2020 2020 2020 6c77 3d31 2e35 2c0a          lw=1.5,.
-000232d0: 2020 2020 2020 2020 2020 2020 6c61 6265              labe
-000232e0: 6c3d 6c6f 676d 6f64 656c 2e4e 414d 452c  l=logmodel.NAME,
-000232f0: 0a20 2020 2020 2020 2020 2020 206c 733d  .            ls=
-00023300: 272d 2d27 0a20 2020 2020 2020 2029 0a0a  '--'.        )..
-00023310: 2020 2020 6966 2074 7970 6528 6d6f 6465      if type(mode
-00023320: 6c29 2069 6e20 5b4d 756c 7469 4c6f 6754  l) in [MultiLogT
-00023330: 6175 544d 6f64 656c 2c20 4d75 6c74 694c  auTModel, MultiL
-00023340: 6f67 5461 7548 4d6f 6465 6c5d 2061 6e64  ogTauHModel] and
-00023350: 206c 656e 286c 6f67 6d6f 6465 6c73 2920   len(logmodels) 
-00023360: 3e20 313a 2023 206e 6f71 610a 2020 2020  > 1: # noqa.    
-00023370: 2020 2020 746f 7461 6c20 3d20 6e70 2e7a      total = np.z
-00023380: 6572 6f73 286c 656e 2878 5f76 6172 735f  eros(len(x_vars_
-00023390: 6772 6964 2929 0a0a 2020 2020 2020 2020  grid))..        
-000233a0: 666f 7220 6c6f 676d 6f64 656c 2069 6e20  for logmodel in 
-000233b0: 6c6f 676d 6f64 656c 733a 0a20 2020 2020  logmodels:.     
-000233c0: 2020 2020 2020 2074 6f74 616c 202b 3d20         total += 
-000233d0: 3130 2a2a 6c6f 676d 6f64 656c 2e6d 6f64  10**logmodel.mod
-000233e0: 656c 280a 2020 2020 2020 2020 2020 2020  el(.            
-000233f0: 2020 2020 6c6f 676d 6f64 656c 2e66 696e      logmodel.fin
-00023400: 616c 5f76 6172 5f76 616c 7565 732c 0a20  al_var_values,. 
-00023410: 2020 2020 2020 2020 2020 2020 2020 2078                 x
-00023420: 5f76 6172 735f 6772 6964 2c0a 2020 2020  _vars_grid,.    
-00023430: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-00023440: 2020 2061 782e 706c 6f74 280a 2020 2020     ax.plot(.    
-00023450: 2020 2020 2020 2020 312e 202f 2078 5f76          1. / x_v
-00023460: 6172 735f 6772 6964 2c0a 2020 2020 2020  ars_grid,.      
-00023470: 2020 2020 2020 6e70 2e6c 6f67 2831 2e20        np.log(1. 
-00023480: 2f20 746f 7461 6c29 2c0a 2020 2020 2020  / total),.      
-00023490: 2020 2020 2020 6c77 3d31 2e35 2c0a 2020        lw=1.5,.  
-000234a0: 2020 2020 2020 2020 2020 6c61 6265 6c3d            label=
-000234b0: 2754 6f74 616c 272c 0a20 2020 2020 2020  'Total',.       
-000234c0: 2020 2020 2063 6f6c 6f72 3d27 7265 6427       color='red'
-000234d0: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-000234e0: 2320 456e 6162 6c65 206d 696e 6f72 2074  # Enable minor t
-000234f0: 6963 6b73 0a20 2020 2061 782e 7961 7869  icks.    ax.yaxi
-00023500: 732e 7365 745f 6d69 6e6f 725f 6c6f 6361  s.set_minor_loca
-00023510: 746f 7228 4175 746f 4d69 6e6f 724c 6f63  tor(AutoMinorLoc
-00023520: 6174 6f72 2829 290a 2020 2020 6178 2e78  ator()).    ax.x
-00023530: 6178 6973 2e73 6574 5f6d 696e 6f72 5f6c  axis.set_minor_l
-00023540: 6f63 6174 6f72 2841 7574 6f4d 696e 6f72  ocator(AutoMinor
-00023550: 4c6f 6361 746f 7228 2929 0a0a 2020 2020  Locator())..    
-00023560: 6578 7072 6573 7369 6f6e 203d 2027 270a  expression = ''.
-00023570: 0a20 2020 2066 6f72 206c 6f67 6d6f 6465  .    for logmode
-00023580: 6c20 696e 206c 6f67 6d6f 6465 6c73 3a0a  l in logmodels:.
-00023590: 2020 2020 2020 2020 666f 7220 6974 2c20          for it, 
-000235a0: 6e61 6d65 2069 6e20 656e 756d 6572 6174  name in enumerat
-000235b0: 6528 6c6f 676d 6f64 656c 2e50 4152 4e41  e(logmodel.PARNA
-000235c0: 4d45 5329 3a0a 2020 2020 2020 2020 2020  MES):.          
-000235d0: 2020 6578 7072 6573 7369 6f6e 202b 3d20    expression += 
-000235e0: 277b 7d20 3d20 7b3a 2e33 667d 2027 2e66  '{} = {:.3f} '.f
-000235f0: 6f72 6d61 7428 0a20 2020 2020 2020 2020  ormat(.         
-00023600: 2020 2020 2020 206c 6f67 6d6f 6465 6c2e         logmodel.
-00023610: 5641 524e 414d 4553 5f4d 4d5b 6e61 6d65  VARNAMES_MM[name
-00023620: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-00023630: 2020 206c 6f67 6d6f 6465 6c2e 6669 6e61     logmodel.fina
-00023640: 6c5f 7661 725f 7661 6c75 6573 5b6e 616d  l_var_values[nam
-00023650: 655d 2c0a 2020 2020 2020 2020 2020 2020  e],.            
-00023660: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-00023670: 206e 616d 6520 696e 206c 6f67 6d6f 6465   name in logmode
-00023680: 6c2e 6669 745f 7661 7273 2e6b 6579 7328  l.fit_vars.keys(
-00023690: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-000236a0: 2020 2065 7870 7265 7373 696f 6e20 2b3d     expression +=
-000236b0: 2072 2724 5c70 6d24 2027 0a20 2020 2020   r'$\pm$ '.     
-000236c0: 2020 2020 2020 2020 2020 2065 7870 7265             expre
-000236d0: 7373 696f 6e20 2b3d 2027 7b3a 2e33 667d  ssion += '{:.3f}
-000236e0: 2027 2e66 6f72 6d61 7428 6c6f 676d 6f64   '.format(logmod
-000236f0: 656c 2e66 6974 5f73 7464 6576 5b6e 616d  el.fit_stdev[nam
-00023700: 655d 290a 2020 2020 2020 2020 2020 2020  e]).            
-00023710: 6578 7072 6573 7369 6f6e 202b 3d20 277b  expression += '{
-00023720: 7d20 2020 2027 2e66 6f72 6d61 7428 6c6f  }    '.format(lo
-00023730: 676d 6f64 656c 2e55 4e49 5453 5f4d 4d5b  gmodel.UNITS_MM[
-00023740: 6e61 6d65 5d29 0a20 2020 2020 2020 2020  name]).         
-00023750: 2020 2069 6620 6974 203d 3d20 3120 616e     if it == 1 an
-00023760: 6420 6c65 6e28 6c6f 676d 6f64 656c 2e66  d len(logmodel.f
-00023770: 6974 5f76 6172 732e 6b65 7973 2829 2920  it_vars.keys()) 
-00023780: 3e20 323a 0a20 2020 2020 2020 2020 2020  > 2:.           
-00023790: 2020 2020 2065 7870 7265 7373 696f 6e20       expression 
-000237a0: 2b3d 2027 5c6e 270a 2020 2020 2020 2020  += '\n'.        
-000237b0: 6578 7072 6573 7369 6f6e 202b 3d20 275c  expression += '\
-000237c0: 6e27 0a0a 2020 2020 6178 2e74 6578 7428  n'..    ax.text(
-000237d0: 0a20 2020 2020 2020 2030 2e30 2c20 312e  .        0.0, 1.
-000237e0: 3032 2c20 733d 6578 7072 6573 7369 6f6e  02, s=expression
-000237f0: 2c20 666f 6e74 7369 7a65 3d31 302c 2074  , fontsize=10, t
-00023800: 7261 6e73 666f 726d 3d61 782e 7472 616e  ransform=ax.tran
-00023810: 7341 7865 730a 2020 2020 290a 0a20 2020  sAxes.    )..   
-00023820: 2061 782e 6c65 6765 6e64 280a 2020 2020   ax.legend(.    
-00023830: 2020 2020 6c6f 633d 276c 6f77 6572 2072      loc='lower r
-00023840: 6967 6874 272c 2066 6f6e 7473 697a 653d  ight', fontsize=
-00023850: 2731 3027 2c20 6e75 6d70 6f69 6e74 733d  '10', numpoints=
-00023860: 312c 206e 636f 6c3d 312c 2066 7261 6d65  1, ncol=1, frame
-00023870: 6f6e 3d46 616c 7365 0a20 2020 2029 0a20  on=False.    ). 
-00023880: 2020 2061 782e 7365 745f 796c 6162 656c     ax.set_ylabel
-00023890: 2872 2724 5c6c 6e5c 6c65 6674 5b5c 7461  (r'$\ln\left[\ta
-000238a0: 755c 7269 6768 745d 2420 245c 6c65 6674  u\right]$ $\left
-000238b0: 285c 6c6e 5c6c 6566 745b 5c6d 6174 6872  (\ln\left[\mathr
-000238c0: 6567 756c 6172 7b73 7d5e 5c6d 6174 6872  egular{s}^\mathr
-000238d0: 6567 756c 6172 7b2d 317d 5c72 6967 6874  egular{-1}\right
-000238e0: 5d5c 7269 6768 7429 2427 2920 2320 6e6f  ]\right)$') # no
-000238f0: 7161 0a0a 2020 2020 7265 7475 726e 0a0a  qa..    return..
-00023900: 0a64 6566 2070 6c6f 745f 6669 7474 6564  .def plot_fitted
-00023910: 5f72 6174 6573 2864 6174 6173 6574 3a20  _rates(dataset: 
-00023920: 5461 7554 4461 7461 7365 7420 7c20 5461  TauTDataset | Ta
-00023930: 7548 4461 7461 7365 742c 0a20 2020 2020  uHDataset,.     
-00023940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023950: 206d 6f64 656c 3a20 4c6f 6754 6175 544d   model: LogTauTM
-00023960: 6f64 656c 207c 204d 756c 7469 4c6f 6754  odel | MultiLogT
-00023970: 6175 544d 6f64 656c 207c 204c 6f67 5461  auTModel | LogTa
-00023980: 7548 4d6f 6465 6c20 7c20 4d75 6c74 694c  uHModel | MultiL
-00023990: 6f67 5461 7548 4d6f 6465 6c2c 2023 206e  ogTauHModel, # n
-000239a0: 6f71 610a 2020 2020 2020 2020 2020 2020  oqa.            
-000239b0: 2020 2020 2020 2020 2020 7368 6f77 3a20            show: 
-000239c0: 626f 6f6c 203d 2054 7275 652c 2073 6176  bool = True, sav
-000239d0: 653a 2062 6f6f 6c20 3d20 4661 6c73 652c  e: bool = False,
-000239e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000239f0: 2020 2020 2020 2073 6176 655f 6e61 6d65         save_name
-00023a00: 3a20 7374 7220 3d20 2766 6974 7465 645f  : str = 'fitted_
-00023a10: 7261 7465 732e 706e 6727 2c0a 2020 2020  rates.png',.    
-00023a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023a30: 2020 7665 7262 6f73 653a 2062 6f6f 6c20    verbose: bool 
-00023a40: 3d20 5472 7565 2920 2d3e 2074 7570 6c65  = True) -> tuple
-00023a50: 5b70 6c74 2e46 6967 7572 652c 2070 6c74  [plt.Figure, plt
-00023a60: 2e41 7865 735d 3a0a 2020 2020 2727 270a  .Axes]:.    '''.
-00023a70: 2020 2020 506c 6f74 7320 6578 7065 7269      Plots experi
-00023a80: 6d65 6e74 616c 2061 6e64 2066 6974 7465  mental and fitte
-00023a90: 6420 286d 6f64 656c 2920 7265 6c61 7861  d (model) relaxa
-00023aa0: 7469 6f6e 2072 6174 6520 6173 5c6e 0a20  tion rate as\n. 
-00023ab0: 2020 2072 6174 6520 7673 2078 7661 7220     rate vs xvar 
-00023ac0: 7768 6572 6520 7876 6172 2069 7320 5420  where xvar is T 
-00023ad0: 6f72 2048 2e20 5769 7468 206c 6f67 206c  or H. With log l
-00023ae0: 6f67 2073 6361 6c65 2e0a 0a20 2020 2050  og scale...    P
-00023af0: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
-00023b00: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2064 6174  --------.    dat
-00023b10: 6173 6574 3a20 5461 7554 4461 7461 7365  aset: TauTDatase
-00023b20: 7420 7c20 5461 7548 4461 7461 7365 740a  t | TauHDataset.
-00023b30: 2020 2020 2020 2020 4461 7461 7365 7420          Dataset 
-00023b40: 746f 2070 6c6f 740a 2020 2020 6d6f 6465  to plot.    mode
-00023b50: 6c3a 204c 6f67 5461 7554 4d6f 6465 6c20  l: LogTauTModel 
-00023b60: 7c20 4d75 6c74 694c 6f67 5461 7554 4d6f  | MultiLogTauTMo
-00023b70: 6465 6c20 7c20 4c6f 6754 6175 484d 6f64  del | LogTauHMod
-00023b80: 656c 207c 204d 756c 7469 4c6f 6754 6175  el | MultiLogTau
-00023b90: 484d 6f64 656c 0a20 2020 2020 2020 204d  HModel.        M
-00023ba0: 6f64 656c 2028 6669 7474 6564 2920 746f  odel (fitted) to
-00023bb0: 2070 6c6f 740a 2020 2020 7368 6f77 3a20   plot.    show: 
-00023bc0: 626f 6f6c 2c20 6465 6661 756c 7420 5472  bool, default Tr
-00023bd0: 7565 0a20 2020 2020 2020 2049 6620 5472  ue.        If Tr
-00023be0: 7565 2c20 7368 6f77 2070 6c6f 7420 6f6e  ue, show plot on
-00023bf0: 2073 6372 6565 6e0a 2020 2020 7361 7665   screen.    save
-00023c00: 3a20 626f 6f6c 2c20 6465 6661 756c 7420  : bool, default 
-00023c10: 4661 6c73 650a 2020 2020 2020 2020 4966  False.        If
-00023c20: 2054 7275 652c 2073 6176 6520 706c 6f74   True, save plot
-00023c30: 2074 6f20 6669 6c65 2060 7361 7665 5f6e   to file `save_n
-00023c40: 616d 6560 0a20 2020 2073 6176 655f 6e61  ame`.    save_na
-00023c50: 6d65 3a20 7374 722c 2064 6566 6175 6c74  me: str, default
-00023c60: 203d 2027 6669 7474 6564 5f72 6174 6573   = 'fitted_rates
-00023c70: 2e70 6e67 270a 2020 2020 2020 2020 4966  .png'.        If
-00023c80: 2073 6176 6520 6973 2054 7275 652c 2077   save is True, w
-00023c90: 696c 6c20 7361 7665 2070 6c6f 7420 746f  ill save plot to
-00023ca0: 2074 6869 7320 6669 6c65 6e61 6d65 0a20   this filename. 
-00023cb0: 2020 2076 6572 626f 7365 3a20 626f 6f6c     verbose: bool
-00023cc0: 2c20 6465 6661 756c 7420 5472 7565 0a20  , default True. 
-00023cd0: 2020 2020 2020 2049 6620 5472 7565 2c20         If True, 
-00023ce0: 706c 6f74 2066 696c 6520 6c6f 6361 7469  plot file locati
-00023cf0: 6f6e 2069 7320 7772 6974 7465 6e20 746f  on is written to
-00023d00: 2074 6572 6d69 6e61 6c0a 2020 2020 5265   terminal.    Re
-00023d10: 7475 726e 730a 2020 2020 2d2d 2d2d 2d2d  turns.    ------
-00023d20: 2d0a 2020 2020 706c 742e 4669 6775 7265  -.    plt.Figure
-00023d30: 0a20 2020 2020 2020 204d 6174 706c 6f74  .        Matplot
-00023d40: 6c69 6220 6669 6775 7265 206f 626a 6563  lib figure objec
-00023d50: 740a 2020 2020 706c 742e 4178 6573 0a20  t.    plt.Axes. 
-00023d60: 2020 2020 2020 204d 6174 706c 6f74 6c69         Matplotli
-00023d70: 6220 6178 6973 206f 626a 6563 740a 2020  b axis object.  
-00023d80: 2020 2727 270a 0a20 2020 2023 2043 7265    '''..    # Cre
-00023d90: 6174 6520 6669 6775 7265 2061 6e64 2061  ate figure and a
-00023da0: 7865 730a 2020 2020 6669 672c 2061 7820  xes.    fig, ax 
-00023db0: 3d20 706c 742e 7375 6270 6c6f 7473 280a  = plt.subplots(.
-00023dc0: 2020 2020 2020 2020 312c 0a20 2020 2020          1,.     
-00023dd0: 2020 2031 2c0a 2020 2020 2020 2020 7368     1,.        sh
-00023de0: 6172 6578 3d54 7275 652c 0a20 2020 2020  arex=True,.     
-00023df0: 2020 2073 6861 7265 793d 5472 7565 2c0a     sharey=True,.
-00023e00: 2020 2020 2020 2020 6669 6773 697a 653d          figsize=
-00023e10: 2836 2c20 3629 2c0a 2020 2020 2020 2020  (6, 6),.        
-00023e20: 6e75 6d3d 2746 6974 7465 6420 7265 6c61  num='Fitted rela
-00023e30: 7861 7469 6f6e 2070 726f 6669 6c65 270a  xation profile'.
-00023e40: 2020 2020 290a 0a20 2020 205f 706c 6f74      )..    _plot
-00023e50: 5f66 6974 7465 645f 7261 7465 7328 6461  _fitted_rates(da
-00023e60: 7461 7365 742c 206d 6f64 656c 2c20 6669  taset, model, fi
-00023e70: 672c 2061 7829 0a0a 2020 2020 6669 672e  g, ax)..    fig.
-00023e80: 7469 6768 745f 6c61 796f 7574 2829 0a0a  tight_layout()..
-00023e90: 2020 2020 6966 2073 686f 773a 0a20 2020      if show:.   
-00023ea0: 2020 2020 2070 6c74 2e73 686f 7728 290a       plt.show().
-00023eb0: 0a20 2020 2069 6620 7361 7665 3a0a 2020  .    if save:.  
-00023ec0: 2020 2020 2020 6669 672e 7361 7665 6669        fig.savefi
-00023ed0: 6728 7361 7665 5f6e 616d 652c 2064 7069  g(save_name, dpi
-00023ee0: 3d35 3030 290a 2020 2020 2020 2020 6966  =500).        if
-00023ef0: 2076 6572 626f 7365 3a0a 2020 2020 2020   verbose:.      
-00023f00: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
-00023f10: 6e63 6528 6461 7461 7365 742c 2028 5461  nce(dataset, (Ta
-00023f20: 7554 4461 7461 7365 7429 293a 0a20 2020  uTDataset)):.   
-00023f30: 2020 2020 2020 2020 2020 2020 205f 7876               _xv
-00023f40: 6172 203d 2027 5427 0a20 2020 2020 2020  ar = 'T'.       
-00023f50: 2020 2020 2065 6c69 6620 6973 696e 7374       elif isinst
-00023f60: 616e 6365 2864 6174 6173 6574 2c20 2854  ance(dataset, (T
-00023f70: 6175 4844 6174 6173 6574 2929 3a0a 2020  auHDataset)):.  
-00023f80: 2020 2020 2020 2020 2020 2020 2020 5f78                _x
-00023f90: 7661 7220 3d20 2748 270a 2020 2020 2020  var = 'H'.      
-00023fa0: 2020 2020 2020 7574 2e63 7072 696e 7428        ut.cprint(
-00023fb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00023fc0: 2066 275c 6e20 4669 7474 6564 20cf 84e2   f'\n Fitted ...
-00023fd0: 81bb c2b9 2076 7320 7b5f 7876 6172 7d20  .... vs {_xvar} 
-00023fe0: 706c 6f74 2073 6176 6564 2074 6f20 5c6e  plot saved to \n
-00023ff0: 207b 7361 7665 5f6e 616d 657d 5c6e 272c   {save_name}\n',
-00024000: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00024010: 2027 6379 616e 270a 2020 2020 2020 2020   'cyan'.        
-00024020: 2020 2020 290a 0a20 2020 2072 6574 7572      )..    retur
-00024030: 6e20 6669 672c 2061 780a 0a0a 6465 6620  n fig, ax...def 
-00024040: 7174 5f70 6c6f 745f 6669 7474 6564 5f72  qt_plot_fitted_r
-00024050: 6174 6573 2861 7070 3a20 5174 5769 6467  ates(app: QtWidg
-00024060: 6574 732e 5141 7070 6c69 6361 7469 6f6e  ets.QApplication
-00024070: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00024080: 2020 2020 2020 2020 2020 2064 6174 6173             datas
-00024090: 6574 3a20 5461 7554 4461 7461 7365 7420  et: TauTDataset 
-000240a0: 7c20 5461 7548 4461 7461 7365 742c 0a20  | TauHDataset,. 
-000240b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000240c0: 2020 2020 2020 2020 6d6f 6465 6c3a 204c          model: L
-000240d0: 6f67 5461 7554 4d6f 6465 6c20 7c20 4d75  ogTauTModel | Mu
-000240e0: 6c74 694c 6f67 5461 7554 4d6f 6465 6c20  ltiLogTauTModel 
-000240f0: 7c20 4c6f 6754 6175 484d 6f64 656c 207c  | LogTauHModel |
-00024100: 204d 756c 7469 4c6f 6754 6175 484d 6f64   MultiLogTauHMod
-00024110: 656c 2c20 2320 6e6f 7161 0a20 2020 2020  el, # noqa.     
-00024120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024130: 2020 2020 7361 7665 3a20 626f 6f6c 203d      save: bool =
-00024140: 2046 616c 7365 2c20 7368 6f77 3a20 626f   False, show: bo
-00024150: 6f6c 203d 2054 7275 652c 0a20 2020 2020  ol = True,.     
-00024160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024170: 2020 2020 7361 7665 5f6e 616d 653a 2073      save_name: s
-00024180: 7472 203d 2027 6669 7474 6564 5f72 6174  tr = 'fitted_rat
-00024190: 6573 2e70 6e67 272c 0a20 2020 2020 2020  es.png',.       
-000241a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000241b0: 2020 7665 7262 6f73 653a 2062 6f6f 6c20    verbose: bool 
-000241c0: 3d20 5472 7565 2920 2d3e 204e 6f6e 653a  = True) -> None:
-000241d0: 0a20 2020 2027 2727 0a20 2020 2050 6c6f  .    '''.    Plo
-000241e0: 7473 2065 7870 6572 696d 656e 7461 6c20  ts experimental 
-000241f0: 616e 6420 6669 7474 6564 2028 6d6f 6465  and fitted (mode
-00024200: 6c29 2072 656c 6178 6174 696f 6e20 7261  l) relaxation ra
-00024210: 7465 2061 735c 6e0a 2020 2020 7261 7465  te as\n.    rate
-00024220: 2076 7320 7876 6172 2077 6865 7265 2078   vs xvar where x
-00024230: 7661 7220 6973 2054 206f 7220 482e 2057  var is T or H. W
-00024240: 6974 6820 6c6f 6720 6c6f 6720 7363 616c  ith log log scal
-00024250: 652e 0a0a 2020 2020 5061 7261 6d65 7465  e...    Paramete
-00024260: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
-00024270: 2d0a 2020 2020 6461 7461 7365 743a 2054  -.    dataset: T
-00024280: 6175 5444 6174 6173 6574 207c 2054 6175  auTDataset | Tau
-00024290: 4844 6174 6173 6574 0a20 2020 2020 2020  HDataset.       
-000242a0: 2044 6174 6173 6574 2074 6f20 706c 6f74   Dataset to plot
-000242b0: 0a20 2020 206d 6f64 656c 3a20 4c6f 6754  .    model: LogT
-000242c0: 6175 544d 6f64 656c 207c 204d 756c 7469  auTModel | Multi
-000242d0: 4c6f 6754 6175 544d 6f64 656c 207c 204c  LogTauTModel | L
-000242e0: 6f67 5461 7548 4d6f 6465 6c20 7c20 4d75  ogTauHModel | Mu
-000242f0: 6c74 694c 6f67 5461 7548 4d6f 6465 6c0a  ltiLogTauHModel.
-00024300: 2020 2020 2020 2020 4d6f 6465 6c20 2866          Model (f
-00024310: 6974 7465 6429 2074 6f20 706c 6f74 0a20  itted) to plot. 
-00024320: 2020 2073 686f 773a 2062 6f6f 6c2c 2064     show: bool, d
-00024330: 6566 6175 6c74 2054 7275 650a 2020 2020  efault True.    
-00024340: 2020 2020 4966 2054 7275 652c 2073 686f      If True, sho
-00024350: 7720 706c 6f74 206f 6e20 7363 7265 656e  w plot on screen
-00024360: 0a20 2020 2073 6176 653a 2062 6f6f 6c2c  .    save: bool,
-00024370: 2064 6566 6175 6c74 2046 616c 7365 0a20   default False. 
-00024380: 2020 2020 2020 2049 6620 5472 7565 2c20         If True, 
-00024390: 7361 7665 2070 6c6f 7420 746f 2066 696c  save plot to fil
-000243a0: 6520 6073 6176 655f 6e61 6d65 600a 2020  e `save_name`.  
-000243b0: 2020 7361 7665 5f6e 616d 653a 2073 7472    save_name: str
-000243c0: 2c20 6465 6661 756c 7420 2766 6974 7465  , default 'fitte
-000243d0: 645f 7261 7465 732e 706e 6727 0a20 2020  d_rates.png'.   
-000243e0: 2020 2020 2049 6620 7361 7665 2069 7320       If save is 
-000243f0: 5472 7565 2c20 7769 6c6c 2073 6176 6520  True, will save 
-00024400: 706c 6f74 2074 6f20 7468 6973 2066 696c  plot to this fil
-00024410: 656e 616d 650a 2020 2020 7665 7262 6f73  ename.    verbos
-00024420: 653a 2062 6f6f 6c2c 2064 6566 6175 6c74  e: bool, default
-00024430: 2054 7275 650a 2020 2020 2020 2020 4966   True.        If
-00024440: 2054 7275 652c 2070 6c6f 7420 6669 6c65   True, plot file
-00024450: 206c 6f63 6174 696f 6e20 6973 2077 7269   location is wri
-00024460: 7474 656e 2074 6f20 7465 726d 696e 616c  tten to terminal
-00024470: 0a0a 2020 2020 5265 7475 726e 730a 2020  ..    Returns.  
-00024480: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 4e6f    -------.    No
-00024490: 6e65 0a20 2020 2027 2727 0a0a 2020 2020  ne.    '''..    
-000244a0: 7769 6e64 6f77 203d 2067 7569 2e4d 6174  window = gui.Mat
-000244b0: 706c 6f74 6c69 6257 696e 646f 7728 290a  plotlibWindow().
-000244c0: 0a20 2020 2077 696e 646f 772e 7365 7457  .    window.setW
-000244d0: 696e 646f 7754 6974 6c65 2827 4669 7474  indowTitle('Fitt
-000244e0: 6564 2072 656c 6178 6174 696f 6e20 7072  ed relaxation pr
-000244f0: 6f66 696c 6527 290a 0a20 2020 2023 2041  ofile')..    # A
-00024500: 6464 2070 6c6f 740a 2020 2020 5f70 6c6f  dd plot.    _plo
-00024510: 745f 6669 7474 6564 5f72 6174 6573 2864  t_fitted_rates(d
-00024520: 6174 6173 6574 2c20 6d6f 6465 6c2c 2077  ataset, model, w
-00024530: 696e 646f 772e 7363 2e66 6967 2c20 7769  indow.sc.fig, wi
-00024540: 6e64 6f77 2e73 632e 6178 290a 0a20 2020  ndow.sc.ax)..   
-00024550: 2023 2053 6176 6520 706c 6f74 0a20 2020   # Save plot.   
-00024560: 2069 6620 7361 7665 3a0a 2020 2020 2020   if save:.      
-00024570: 2020 7769 6e64 6f77 2e73 632e 6669 672e    window.sc.fig.
-00024580: 7361 7665 6669 6728 7361 7665 5f6e 616d  savefig(save_nam
-00024590: 652c 2064 7069 3d33 3030 290a 2020 2020  e, dpi=300).    
-000245a0: 2020 2020 6966 2076 6572 626f 7365 3a0a      if verbose:.
-000245b0: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-000245c0: 7369 6e73 7461 6e63 6528 6461 7461 7365  sinstance(datase
-000245d0: 742c 2028 5461 7554 4461 7461 7365 7429  t, (TauTDataset)
-000245e0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-000245f0: 2020 205f 7876 6172 203d 2027 5427 0a20     _xvar = 'T'. 
-00024600: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-00024610: 6973 696e 7374 616e 6365 2864 6174 6173  isinstance(datas
-00024620: 6574 2c20 2854 6175 4844 6174 6173 6574  et, (TauHDataset
-00024630: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
-00024640: 2020 2020 5f78 7661 7220 3d20 2748 270a      _xvar = 'H'.
-00024650: 2020 2020 2020 2020 2020 2020 7574 2e63              ut.c
-00024660: 7072 696e 7428 0a20 2020 2020 2020 2020  print(.         
-00024670: 2020 2020 2020 2066 275c 6e20 4669 7474         f'\n Fitt
-00024680: 6564 20cf 84e2 81bb c2b9 2076 7320 7b5f  ed ....... vs {_
-00024690: 7876 6172 7d20 706c 6f74 2073 6176 6564  xvar} plot saved
-000246a0: 2074 6f20 5c6e 207b 7361 7665 5f6e 616d   to \n {save_nam
-000246b0: 657d 5c6e 272c 0a20 2020 2020 2020 2020  e}\n',.         
-000246c0: 2020 2020 2020 2027 6379 616e 270a 2020         'cyan'.  
-000246d0: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
-000246e0: 2069 6620 7368 6f77 3a0a 2020 2020 2020   if show:.      
-000246f0: 2020 7769 6e64 6f77 2e73 686f 7728 290a    window.show().
-00024700: 2020 2020 2020 2020 2320 4361 6c6c 2074          # Call t
-00024710: 7769 6365 2065 6c73 6520 6974 2077 6f6e  wice else it won
-00024720: 7420 776f 726b 210a 2020 2020 2020 2020  t work!.        
-00024730: 7769 6e64 6f77 2e73 632e 6669 672e 7469  window.sc.fig.ti
-00024740: 6768 745f 6c61 796f 7574 2829 0a20 2020  ght_layout().   
-00024750: 2020 2020 2077 696e 646f 772e 7363 2e66       window.sc.f
-00024760: 6967 2e74 6967 6874 5f6c 6179 6f75 7428  ig.tight_layout(
-00024770: 290a 2020 2020 2020 2020 6170 702e 6578  ).        app.ex
-00024780: 6563 5f28 290a 0a20 2020 2072 6574 7572  ec_()..    retur
-00024790: 6e0a 0a0a 6465 6620 5f70 6c6f 745f 6669  n...def _plot_fi
-000247a0: 7474 6564 5f72 6174 6573 2864 6174 6173  tted_rates(datas
-000247b0: 6574 3a20 5461 7554 4461 7461 7365 7420  et: TauTDataset 
-000247c0: 7c20 5461 7548 4461 7461 7365 742c 0a20  | TauHDataset,. 
-000247d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000247e0: 2020 2020 2020 6d6f 6465 6c3a 204c 6f67        model: Log
-000247f0: 5461 7554 4d6f 6465 6c20 7c20 4d75 6c74  TauTModel | Mult
-00024800: 694c 6f67 5461 7554 4d6f 6465 6c20 7c20  iLogTauTModel | 
-00024810: 4c6f 6754 6175 484d 6f64 656c 207c 204d  LogTauHModel | M
-00024820: 756c 7469 4c6f 6754 6175 484d 6f64 656c  ultiLogTauHModel
-00024830: 2c20 2320 6e6f 7161 0a20 2020 2020 2020  , # noqa.       
-00024840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024850: 6669 673a 2070 6c74 2e46 6967 7572 652c  fig: plt.Figure,
-00024860: 2061 783a 2070 6c74 2e41 7865 7329 3a0a   ax: plt.Axes):.
-00024870: 2020 2020 2727 270a 2020 2020 506c 6f74      '''.    Plot
-00024880: 7320 6578 7065 7269 6d65 6e74 616c 2061  s experimental a
-00024890: 6e64 2066 6974 7465 6420 286d 6f64 656c  nd fitted (model
-000248a0: 2920 7265 6c61 7861 7469 6f6e 2072 6174  ) relaxation rat
-000248b0: 6520 6173 5c6e 0a20 2020 2072 6174 6520  e as\n.    rate 
-000248c0: 7673 2078 7661 7220 7768 6572 6520 7876  vs xvar where xv
-000248d0: 6172 2069 7320 5420 6f72 2048 2e20 5769  ar is T or H. Wi
-000248e0: 7468 206c 6f67 206c 6f67 2073 6361 6c65  th log log scale
-000248f0: 2e0a 0a20 2020 2050 6172 616d 6574 6572  ...    Parameter
-00024900: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  s.    ----------
-00024910: 0a20 2020 2064 6174 6173 6574 3a20 5461  .    dataset: Ta
-00024920: 7554 4461 7461 7365 7420 7c20 5461 7548  uTDataset | TauH
-00024930: 4461 7461 7365 740a 2020 2020 2020 2020  Dataset.        
-00024940: 4461 7461 7365 7420 746f 2070 6c6f 740a  Dataset to plot.
-00024950: 2020 2020 6d6f 6465 6c3a 204c 6f67 5461      model: LogTa
-00024960: 7554 4d6f 6465 6c20 7c20 4d75 6c74 694c  uTModel | MultiL
-00024970: 6f67 5461 7554 4d6f 6465 6c20 7c20 4c6f  ogTauTModel | Lo
-00024980: 6754 6175 484d 6f64 656c 207c 204d 756c  gTauHModel | Mul
-00024990: 7469 4c6f 6754 6175 484d 6f64 656c 0a20  tiLogTauHModel. 
-000249a0: 2020 2020 2020 204d 6f64 656c 2028 6669         Model (fi
-000249b0: 7474 6564 2920 746f 2070 6c6f 740a 2020  tted) to plot.  
-000249c0: 2020 6669 673a 2070 6c74 2e46 6967 7572    fig: plt.Figur
-000249d0: 650a 2020 2020 2020 2020 4d61 7470 6c6f  e.        Matplo
-000249e0: 746c 6962 2046 6967 7572 6520 6f62 6a65  tlib Figure obje
-000249f0: 6374 2075 7365 6420 666f 7220 706c 6f74  ct used for plot
-00024a00: 0a20 2020 2061 783a 2070 6c74 2e41 7865  .    ax: plt.Axe
-00024a10: 730a 2020 2020 2020 2020 4d61 7470 6c6f  s.        Matplo
-00024a20: 746c 6962 2041 7869 7320 6f62 6a65 6374  tlib Axis object
-00024a30: 2075 7365 6420 666f 7220 706c 6f74 0a0a   used for plot..
-00024a40: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-00024a50: 2d2d 2d2d 2d2d 2d0a 2020 2020 4e6f 6e65  -------.    None
-00024a60: 0a20 2020 2027 2727 0a0a 2020 2020 6966  .    '''..    if
-00024a70: 2069 7369 6e73 7461 6e63 6528 6461 7461   isinstance(data
-00024a80: 7365 742c 2054 6175 4844 6174 6173 6574  set, TauHDataset
-00024a90: 293a 0a20 2020 2020 2020 2078 5f76 6172  ):.        x_var
-00024aa0: 7320 3d20 6461 7461 7365 742e 6669 656c  s = dataset.fiel
-00024ab0: 6473 0a20 2020 2020 2020 2061 782e 7365  ds.        ax.se
-00024ac0: 745f 786c 6162 656c 2872 2746 6965 6c64  t_xlabel(r'Field
-00024ad0: 2028 4f65 2927 290a 2020 2020 656c 6966   (Oe)').    elif
-00024ae0: 2069 7369 6e73 7461 6e63 6528 6461 7461   isinstance(data
-00024af0: 7365 742c 2054 6175 5444 6174 6173 6574  set, TauTDataset
-00024b00: 293a 0a20 2020 2020 2020 2078 5f76 6172  ):.        x_var
-00024b10: 7320 3d20 6461 7461 7365 742e 7465 6d70  s = dataset.temp
-00024b20: 6572 6174 7572 6573 0a20 2020 2020 2020  eratures.       
-00024b30: 2061 782e 7365 745f 786c 6162 656c 2872   ax.set_xlabel(r
-00024b40: 2754 656d 7065 7261 7475 7265 2028 4b29  'Temperature (K)
-00024b50: 2729 0a0a 2020 2020 2320 4164 6420 756e  ')..    # Add un
-00024b60: 6365 7274 6169 6e74 6965 7320 6173 2065  certainties as e
-00024b70: 7272 6f72 6261 7273 0a20 2020 2069 6620  rrorbars.    if 
-00024b80: 6c65 6e28 6461 7461 7365 742e 7261 7465  len(dataset.rate
-00024b90: 5f70 6d29 3a0a 2020 2020 2020 2020 6178  _pm):.        ax
-00024ba0: 2e65 7272 6f72 6261 7228 0a20 2020 2020  .errorbar(.     
-00024bb0: 2020 2020 2020 2078 5f76 6172 732c 0a20         x_vars,. 
-00024bc0: 2020 2020 2020 2020 2020 2064 6174 6173             datas
-00024bd0: 6574 2e72 6174 6573 2c0a 2020 2020 2020  et.rates,.      
-00024be0: 2020 2020 2020 7965 7272 3d64 6174 6173        yerr=datas
-00024bf0: 6574 2e72 6174 655f 706d 2c0a 2020 2020  et.rate_pm,.    
-00024c00: 2020 2020 2020 2020 6d61 726b 6572 3d27          marker='
-00024c10: 6f27 2c0a 2020 2020 2020 2020 2020 2020  o',.            
-00024c20: 6c77 3d30 2c0a 2020 2020 2020 2020 2020  lw=0,.          
-00024c30: 2020 656c 696e 6577 6964 7468 3d31 2e35    elinewidth=1.5
-00024c40: 2c0a 2020 2020 2020 2020 2020 2020 6669  ,.            fi
-00024c50: 6c6c 7374 796c 653d 276e 6f6e 6527 2c0a  llstyle='none',.
-00024c60: 2020 2020 2020 2020 2020 2020 6c61 6265              labe
-00024c70: 6c3d 2745 7870 6572 696d 656e 7427 2c0a  l='Experiment',.
-00024c80: 2020 2020 2020 2020 2020 2020 636f 6c6f              colo
-00024c90: 723d 2762 6c61 636b 270a 2020 2020 2020  r='black'.      
-00024ca0: 2020 290a 2020 2020 656c 7365 3a0a 2020    ).    else:.  
-00024cb0: 2020 2020 2020 6178 2e70 6c6f 7428 0a20        ax.plot(. 
-00024cc0: 2020 2020 2020 2020 2020 2078 5f76 6172             x_var
-00024cd0: 732c 0a20 2020 2020 2020 2020 2020 2064  s,.            d
-00024ce0: 6174 6173 6574 2e72 6174 6573 2c0a 2020  ataset.rates,.  
-00024cf0: 2020 2020 2020 2020 2020 6d61 726b 6572            marker
-00024d00: 3d27 6f27 2c0a 2020 2020 2020 2020 2020  ='o',.          
-00024d10: 2020 6c77 3d30 2c0a 2020 2020 2020 2020    lw=0,.        
-00024d20: 2020 2020 6669 6c6c 7374 796c 653d 276e      fillstyle='n
-00024d30: 6f6e 6527 2c0a 2020 2020 2020 2020 2020  one',.          
-00024d40: 2020 6c61 6265 6c3d 2745 7870 6572 696d    label='Experim
-00024d50: 656e 7427 2c0a 2020 2020 2020 2020 2020  ent',.          
-00024d60: 2020 636f 6c6f 723d 2762 6c61 636b 270a    color='black'.
-00024d70: 2020 2020 2020 2020 290a 0a20 2020 2078          )..    x
-00024d80: 5f76 6172 735f 6772 6964 203d 206e 702e  _vars_grid = np.
-00024d90: 6c6f 6773 7061 6365 280a 2020 2020 2020  logspace(.      
-00024da0: 2020 6e70 2e6c 6f67 3130 286e 702e 6d69    np.log10(np.mi
-00024db0: 6e28 785f 7661 7273 2929 2c0a 2020 2020  n(x_vars)),.    
-00024dc0: 2020 2020 6e70 2e6c 6f67 3130 286e 702e      np.log10(np.
-00024dd0: 6d61 7828 785f 7661 7273 2929 2c0a 2020  max(x_vars)),.  
-00024de0: 2020 2020 2020 3530 300a 2020 2020 290a        500.    ).
-00024df0: 0a20 2020 2069 6620 7479 7065 286d 6f64  .    if type(mod
-00024e00: 656c 2920 696e 205b 4d75 6c74 694c 6f67  el) in [MultiLog
-00024e10: 5461 7554 4d6f 6465 6c2c 204d 756c 7469  TauTModel, Multi
-00024e20: 4c6f 6754 6175 484d 6f64 656c 5d3a 0a20  LogTauHModel]:. 
-00024e30: 2020 2020 2020 206c 6f67 6d6f 6465 6c73         logmodels
-00024e40: 203d 206d 6f64 656c 2e6c 6f67 6d6f 6465   = model.logmode
-00024e50: 6c73 0a20 2020 2065 6c73 653a 0a20 2020  ls.    else:.   
-00024e60: 2020 2020 206c 6f67 6d6f 6465 6c73 203d       logmodels =
-00024e70: 205b 6d6f 6465 6c5d 0a0a 2020 2020 666f   [model]..    fo
-00024e80: 7220 6c6f 676d 6f64 656c 2069 6e20 6c6f  r logmodel in lo
-00024e90: 676d 6f64 656c 733a 0a0a 2020 2020 2020  gmodels:..      
-00024ea0: 2020 6966 2074 7970 6528 6c6f 676d 6f64    if type(logmod
-00024eb0: 656c 2920 6973 204c 6f67 4f72 6261 6368  el) is LogOrbach
-00024ec0: 4d6f 6465 6c3a 0a20 2020 2020 2020 2020  Model:.         
-00024ed0: 2020 206c 6162 656c 5f66 6974 203d 2027     label_fit = '
-00024ee0: 5c6e 4669 7420 7769 7468 270a 2020 2020  \nFit with'.    
-00024ef0: 2020 2020 2020 2020 6c61 6265 6c5f 6669          label_fi
-00024f00: 7420 2b3d 2027 5c6e 2720 2b20 7227 7b7d  t += '\n' + r'{}
-00024f10: 207b 3a36 2e32 667d 2073 272e 666f 726d   {:6.2f} s'.form
-00024f20: 6174 280a 2020 2020 2020 2020 2020 2020  at(.            
-00024f30: 2020 2020 6c6f 676d 6f64 656c 2e56 4152      logmodel.VAR
-00024f40: 4e41 4d45 535f 4d4d 5b27 755f 6566 6627  NAMES_MM['u_eff'
-00024f50: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-00024f60: 2020 206c 6f67 6d6f 6465 6c2e 6669 6e61     logmodel.fina
-00024f70: 6c5f 7661 725f 7661 6c75 6573 5b27 755f  l_var_values['u_
-00024f80: 6566 6627 5d0a 2020 2020 2020 2020 2020  eff'].          
-00024f90: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-00024fa0: 6c61 6265 6c5f 6669 7420 2b3d 2027 5c6e  label_fit += '\n
-00024fb0: 2720 2b20 7227 7b7d 207b 3a30 342e 3365  ' + r'{} {:04.3e
-00024fc0: 7d27 2e66 6f72 6d61 7428 0a20 2020 2020  }'.format(.     
-00024fd0: 2020 2020 2020 2020 2020 206c 6f67 6d6f             logmo
-00024fe0: 6465 6c2e 5641 524e 414d 4553 5f4d 4d5b  del.VARNAMES_MM[
-00024ff0: 2741 275d 2c20 6c6f 676d 6f64 656c 2e66  'A'], logmodel.f
-00025000: 696e 616c 5f76 6172 5f76 616c 7565 735b  inal_var_values[
-00025010: 2741 275d 0a20 2020 2020 2020 2020 2020  'A'].           
-00025020: 2029 0a20 2020 2020 2020 2065 6c69 6620   ).        elif 
-00025030: 7479 7065 286c 6f67 6d6f 6465 6c29 2069  type(logmodel) i
-00025040: 7320 4c6f 6752 616d 616e 4d6f 6465 6c3a  s LogRamanModel:
-00025050: 0a20 2020 2020 2020 2020 2020 206c 6162  .            lab
-00025060: 656c 5f66 6974 203d 2027 5c6e 4669 7420  el_fit = '\nFit 
-00025070: 7769 7468 270a 2020 2020 2020 2020 2020  with'.          
-00025080: 2020 6c61 6265 6c5f 6669 7420 2b3d 2027    label_fit += '
-00025090: 5c6e 2720 2b20 7227 7b7d 207b 3a36 2e32  \n' + r'{} {:6.2
-000250a0: 667d 2073 272e 666f 726d 6174 280a 2020  f} s'.format(.  
-000250b0: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-000250c0: 676d 6f64 656c 2e56 4152 4e41 4d45 535f  gmodel.VARNAMES_
-000250d0: 4d4d 5b27 5227 5d2c 206c 6f67 6d6f 6465  MM['R'], logmode
-000250e0: 6c2e 6669 6e61 6c5f 7661 725f 7661 6c75  l.final_var_valu
-000250f0: 6573 5b27 5227 5d0a 2020 2020 2020 2020  es['R'].        
-00025100: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00025110: 2020 6c61 6265 6c5f 6669 7420 2b3d 2027    label_fit += '
-00025120: 5c6e 2720 2b20 7227 7b7d 207b 3a30 342e  \n' + r'{} {:04.
-00025130: 3365 7d27 2e66 6f72 6d61 7428 0a20 2020  3e}'.format(.   
-00025140: 2020 2020 2020 2020 2020 2020 206c 6f67               log
-00025150: 6d6f 6465 6c2e 5641 524e 414d 4553 5f4d  model.VARNAMES_M
-00025160: 4d5b 276e 275d 2c20 6c6f 676d 6f64 656c  M['n'], logmodel
-00025170: 2e66 696e 616c 5f76 6172 5f76 616c 7565  .final_var_value
-00025180: 735b 276e 275d 0a20 2020 2020 2020 2020  s['n'].         
-00025190: 2020 2029 0a20 2020 2020 2020 2065 6c69     ).        eli
-000251a0: 6620 7479 7065 286c 6f67 6d6f 6465 6c29  f type(logmodel)
-000251b0: 2069 7320 4c6f 6751 544d 4d6f 6465 6c3a   is LogQTMModel:
-000251c0: 0a20 2020 2020 2020 2020 2020 206c 6162  .            lab
-000251d0: 656c 5f66 6974 203d 2027 5c6e 4669 7420  el_fit = '\nFit 
-000251e0: 7769 7468 270a 2020 2020 2020 2020 2020  with'.          
-000251f0: 2020 6c61 6265 6c5f 6669 7420 2b3d 2027    label_fit += '
-00025200: 5c6e 2720 2b20 7227 7b7d 207b 3a36 2e32  \n' + r'{} {:6.2
-00025210: 667d 2073 272e 666f 726d 6174 280a 2020  f} s'.format(.  
-00025220: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-00025230: 676d 6f64 656c 2e56 4152 4e41 4d45 535f  gmodel.VARNAMES_
-00025240: 4d4d 5b27 5127 5d2c 206c 6f67 6d6f 6465  MM['Q'], logmode
-00025250: 6c2e 6669 6e61 6c5f 7661 725f 7661 6c75  l.final_var_valu
-00025260: 6573 5b27 5127 5d0a 2020 2020 2020 2020  es['Q'].        
-00025270: 2020 2020 290a 2020 2020 2020 2020 656c      ).        el
-00025280: 6966 2074 7970 6528 6c6f 676d 6f64 656c  if type(logmodel
-00025290: 2920 6973 204c 6f67 4469 7265 6374 4d6f  ) is LogDirectMo
-000252a0: 6465 6c3a 0a20 2020 2020 2020 2020 2020  del:.           
-000252b0: 206c 6162 656c 5f66 6974 203d 2027 5c6e   label_fit = '\n
-000252c0: 4669 7420 7769 7468 270a 2020 2020 2020  Fit with'.      
-000252d0: 2020 2020 2020 6c61 6265 6c5f 6669 7420        label_fit 
-000252e0: 2b3d 2027 5c6e 2720 2b20 7227 7b7d 207b  += '\n' + r'{} {
-000252f0: 3a36 2e32 667d 2073 272e 666f 726d 6174  :6.2f} s'.format
-00025300: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00025310: 2020 6c6f 676d 6f64 656c 2e56 4152 4e41    logmodel.VARNA
-00025320: 4d45 535f 4d4d 5b27 4427 5d2c 206c 6f67  MES_MM['D'], log
-00025330: 6d6f 6465 6c2e 6669 6e61 6c5f 7661 725f  model.final_var_
-00025340: 7661 6c75 6573 5b27 4427 5d0a 2020 2020  values['D'].    
-00025350: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00025360: 2020 6d6f 6465 6c5f 7261 7465 7320 3d20    model_rates = 
-00025370: 3130 2a2a 6c6f 676d 6f64 656c 2e6d 6f64  10**logmodel.mod
-00025380: 656c 280a 2020 2020 2020 2020 2020 2020  el(.            
-00025390: 6c6f 676d 6f64 656c 2e66 696e 616c 5f76  logmodel.final_v
-000253a0: 6172 5f76 616c 7565 732c 0a20 2020 2020  ar_values,.     
-000253b0: 2020 2020 2020 2078 5f76 6172 735f 6772         x_vars_gr
-000253c0: 6964 2c0a 2020 2020 2020 2020 290a 0a20  id,.        ).. 
-000253d0: 2020 2020 2020 2023 2054 7269 6d20 6d6f         # Trim mo
-000253e0: 6465 6c20 7261 7465 7320 746f 2073 656e  del rates to sen
-000253f0: 7369 626c 6520 7661 6c75 6573 0a20 2020  sible values.   
-00025400: 2020 2020 2076 616c 6964 5f69 6e74 203d       valid_int =
-00025410: 206e 702e 7768 6572 6528 6d6f 6465 6c5f   np.where(model_
-00025420: 7261 7465 7320 3e20 3145 2d36 295b 305d  rates > 1E-6)[0]
-00025430: 0a0a 2020 2020 2020 2020 6178 2e70 6c6f  ..        ax.plo
-00025440: 7428 0a20 2020 2020 2020 2020 2020 206e  t(.            n
-00025450: 702e 6172 7261 7928 785f 7661 7273 5f67  p.array(x_vars_g
-00025460: 7269 6429 5b76 616c 6964 5f69 6e74 5d2c  rid)[valid_int],
-00025470: 0a20 2020 2020 2020 2020 2020 206e 702e  .            np.
-00025480: 6172 7261 7928 6d6f 6465 6c5f 7261 7465  array(model_rate
-00025490: 7329 5b76 616c 6964 5f69 6e74 5d2c 0a20  s)[valid_int],. 
-000254a0: 2020 2020 2020 2020 2020 206c 773d 312e             lw=1.
-000254b0: 352c 0a20 2020 2020 2020 2020 2020 206c  5,.            l
-000254c0: 6162 656c 3d6c 6f67 6d6f 6465 6c2e 4e41  abel=logmodel.NA
-000254d0: 4d45 2c0a 2020 2020 2020 2020 2020 2020  ME,.            
-000254e0: 6c73 3d27 2d2d 270a 2020 2020 2020 2020  ls='--'.        
-000254f0: 290a 0a20 2020 2069 6620 7479 7065 286d  )..    if type(m
-00025500: 6f64 656c 2920 696e 205b 4d75 6c74 694c  odel) in [MultiL
-00025510: 6f67 5461 7554 4d6f 6465 6c2c 204d 756c  ogTauTModel, Mul
-00025520: 7469 4c6f 6754 6175 484d 6f64 656c 5d20  tiLogTauHModel] 
-00025530: 616e 6420 6c65 6e28 6c6f 676d 6f64 656c  and len(logmodel
-00025540: 7329 203e 2031 3a20 2320 6e6f 7161 0a20  s) > 1: # noqa. 
-00025550: 2020 2020 2020 2074 6f74 616c 203d 206e         total = n
-00025560: 702e 7a65 726f 7328 6c65 6e28 785f 7661  p.zeros(len(x_va
-00025570: 7273 5f67 7269 6429 290a 0a20 2020 2020  rs_grid))..     
-00025580: 2020 2066 6f72 206c 6f67 6d6f 6465 6c20     for logmodel 
-00025590: 696e 206c 6f67 6d6f 6465 6c73 3a0a 2020  in logmodels:.  
-000255a0: 2020 2020 2020 2020 2020 746f 7461 6c20            total 
-000255b0: 2b3d 2031 302a 2a6c 6f67 6d6f 6465 6c2e  += 10**logmodel.
-000255c0: 6d6f 6465 6c28 0a20 2020 2020 2020 2020  model(.         
-000255d0: 2020 2020 2020 206c 6f67 6d6f 6465 6c2e         logmodel.
-000255e0: 6669 6e61 6c5f 7661 725f 7661 6c75 6573  final_var_values
-000255f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00025600: 2020 785f 7661 7273 5f67 7269 642c 0a20    x_vars_grid,. 
-00025610: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
-00025620: 2020 2020 2020 6178 2e70 6c6f 7428 0a20        ax.plot(. 
-00025630: 2020 2020 2020 2020 2020 2078 5f76 6172             x_var
-00025640: 735f 6772 6964 2c0a 2020 2020 2020 2020  s_grid,.        
-00025650: 2020 2020 746f 7461 6c2c 0a20 2020 2020      total,.     
-00025660: 2020 2020 2020 206c 773d 312e 352c 0a20         lw=1.5,. 
-00025670: 2020 2020 2020 2020 2020 206c 6162 656c             label
-00025680: 3d27 546f 7461 6c27 2c0a 2020 2020 2020  ='Total',.      
-00025690: 2020 2020 2020 636f 6c6f 723d 2772 6564        color='red
-000256a0: 270a 2020 2020 2020 2020 290a 0a20 2020  '.        )..   
-000256b0: 2061 782e 7365 745f 7873 6361 6c65 2827   ax.set_xscale('
-000256c0: 6c6f 6727 290a 2020 2020 6178 2e73 6574  log').    ax.set
-000256d0: 5f79 7363 616c 6528 276c 6f67 2729 0a0a  _yscale('log')..
-000256e0: 2020 2020 6775 692e 666f 726d 6174 5f72      gui.format_r
-000256f0: 6174 655f 785f 795f 6178 6573 280a 2020  ate_x_y_axes(.  
-00025700: 2020 2020 2020 6178 2c0a 2020 2020 2020        ax,.      
-00025710: 2020 6461 7461 7365 742e 7261 7465 732c    dataset.rates,
-00025720: 0a20 2020 2020 2020 2078 5f76 6172 735f  .        x_vars_
-00025730: 6772 6964 2c0a 2020 2020 2020 2020 6e70  grid,.        np
-00025740: 2e61 6273 2864 6174 6173 6574 2e72 6174  .abs(dataset.rat
-00025750: 655f 706d 290a 2020 2020 290a 0a20 2020  e_pm).    )..   
-00025760: 2065 7870 7265 7373 696f 6e20 3d20 2727   expression = ''
-00025770: 0a0a 2020 2020 666f 7220 6c6f 676d 6f64  ..    for logmod
-00025780: 656c 2069 6e20 6c6f 676d 6f64 656c 733a  el in logmodels:
-00025790: 0a20 2020 2020 2020 2066 6f72 2069 742c  .        for it,
-000257a0: 206e 616d 6520 696e 2065 6e75 6d65 7261   name in enumera
-000257b0: 7465 286c 6f67 6d6f 6465 6c2e 5041 524e  te(logmodel.PARN
-000257c0: 414d 4553 293a 0a20 2020 2020 2020 2020  AMES):.         
-000257d0: 2020 2065 7870 7265 7373 696f 6e20 2b3d     expression +=
-000257e0: 2027 7b7d 203d 207b 3a2e 3366 7d20 272e   '{} = {:.3f} '.
-000257f0: 666f 726d 6174 280a 2020 2020 2020 2020  format(.        
-00025800: 2020 2020 2020 2020 6c6f 676d 6f64 656c          logmodel
-00025810: 2e56 4152 4e41 4d45 535f 4d4d 5b6e 616d  .VARNAMES_MM[nam
-00025820: 655d 2c0a 2020 2020 2020 2020 2020 2020  e],.            
-00025830: 2020 2020 6c6f 676d 6f64 656c 2e66 696e      logmodel.fin
-00025840: 616c 5f76 6172 5f76 616c 7565 735b 6e61  al_var_values[na
-00025850: 6d65 5d2c 0a20 2020 2020 2020 2020 2020  me],.           
-00025860: 2029 0a20 2020 2020 2020 2020 2020 2069   ).            i
-00025870: 6620 6e61 6d65 2069 6e20 6c6f 676d 6f64  f name in logmod
-00025880: 656c 2e66 6974 5f76 6172 732e 6b65 7973  el.fit_vars.keys
-00025890: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-000258a0: 2020 2020 6578 7072 6573 7369 6f6e 202b      expression +
-000258b0: 3d20 7227 245c 706d 2420 270a 2020 2020  = r'$\pm$ '.    
-000258c0: 2020 2020 2020 2020 2020 2020 6578 7072              expr
-000258d0: 6573 7369 6f6e 202b 3d20 277b 3a2e 3366  ession += '{:.3f
-000258e0: 7d20 272e 666f 726d 6174 286c 6f67 6d6f  } '.format(logmo
-000258f0: 6465 6c2e 6669 745f 7374 6465 765b 6e61  del.fit_stdev[na
-00025900: 6d65 5d29 0a20 2020 2020 2020 2020 2020  me]).           
-00025910: 2065 7870 7265 7373 696f 6e20 2b3d 2027   expression += '
-00025920: 7b7d 2020 2020 272e 666f 726d 6174 286c  {}    '.format(l
-00025930: 6f67 6d6f 6465 6c2e 554e 4954 535f 4d4d  ogmodel.UNITS_MM
-00025940: 5b6e 616d 655d 290a 2020 2020 2020 2020  [name]).        
-00025950: 2020 2020 6966 2069 7420 3d3d 2031 2061      if it == 1 a
-00025960: 6e64 206c 656e 286c 6f67 6d6f 6465 6c2e  nd len(logmodel.
-00025970: 6669 745f 7661 7273 2e6b 6579 7328 2929  fit_vars.keys())
-00025980: 203e 2032 3a0a 2020 2020 2020 2020 2020   > 2:.          
-00025990: 2020 2020 2020 6578 7072 6573 7369 6f6e        expression
-000259a0: 202b 3d20 275c 6e27 0a20 2020 2020 2020   += '\n'.       
-000259b0: 2065 7870 7265 7373 696f 6e20 2b3d 2027   expression += '
-000259c0: 5c6e 270a 0a20 2020 2061 782e 7465 7874  \n'..    ax.text
-000259d0: 280a 2020 2020 2020 2020 302e 302c 2031  (.        0.0, 1
-000259e0: 2e30 322c 2073 3d65 7870 7265 7373 696f  .02, s=expressio
-000259f0: 6e2c 2066 6f6e 7473 697a 653d 3130 2c20  n, fontsize=10, 
-00025a00: 7472 616e 7366 6f72 6d3d 6178 2e74 7261  transform=ax.tra
-00025a10: 6e73 4178 6573 0a20 2020 2029 0a0a 2020  nsAxes.    )..  
-00025a20: 2020 6178 2e6c 6567 656e 6428 0a20 2020    ax.legend(.   
-00025a30: 2020 2020 206c 6f63 3d27 7570 7065 7220       loc='upper 
-00025a40: 6c65 6674 272c 2066 6f6e 7473 697a 653d  left', fontsize=
-00025a50: 2731 3027 2c20 6e75 6d70 6f69 6e74 733d  '10', numpoints=
-00025a60: 312c 206e 636f 6c3d 312c 2066 7261 6d65  1, ncol=1, frame
-00025a70: 6f6e 3d46 616c 7365 0a20 2020 2029 0a20  on=False.    ). 
-00025a80: 2020 2061 782e 7365 745f 796c 6162 656c     ax.set_ylabel
-00025a90: 2872 2752 6174 6520 2873 245e 5c6d 6174  (r'Rate (s$^\mat
-00025aa0: 6872 6567 756c 6172 7b2d 317d 2429 2729  hregular{-1}$)')
-00025ab0: 0a0a 2020 2020 7265 7475 726e 0a0a 0a64  ..    return...d
-00025ac0: 6566 2070 6c6f 745f 7261 7465 7328 6461  ef plot_rates(da
-00025ad0: 7461 7365 743a 2054 6175 5444 6174 6173  taset: TauTDatas
-00025ae0: 6574 207c 2054 6175 4844 6174 6173 6574  et | TauHDataset
-00025af0: 2c20 7368 6f77 3a20 626f 6f6c 203d 2054  , show: bool = T
-00025b00: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
-00025b10: 2020 2020 7361 7665 3a20 626f 6f6c 203d      save: bool =
-00025b20: 2046 616c 7365 2c20 7361 7665 5f6e 616d   False, save_nam
-00025b30: 653a 2073 7472 203d 2027 7265 6c61 7861  e: str = 'relaxa
-00025b40: 7469 6f6e 5f72 6174 6573 2e70 6e67 272c  tion_rates.png',
-00025b50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00025b60: 7665 7262 6f73 653a 2062 6f6f 6c20 3d20  verbose: bool = 
-00025b70: 5472 7565 2920 2d3e 2074 7570 6c65 5b70  True) -> tuple[p
-00025b80: 6c74 2e46 6967 7572 652c 2070 6c74 2e41  lt.Figure, plt.A
-00025b90: 7865 735d 3a0a 2020 2020 2727 270a 2020  xes]:.    '''.  
-00025ba0: 2020 506c 6f74 7320 6578 7065 7269 6d65    Plots experime
-00025bb0: 6e74 616c 2072 656c 6178 6174 696f 6e20  ntal relaxation 
-00025bc0: 7261 7465 2076 7320 6669 656c 642f 7465  rate vs field/te
-00025bd0: 6d70 6572 6174 7572 6520 616e 640a 2020  mperature and.  
-00025be0: 2020 6469 7370 6c61 7973 206f 6e20 7363    displays on sc
-00025bf0: 7265 656e 2e0a 0a20 2020 2050 6172 616d  reen...    Param
-00025c00: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
-00025c10: 2d2d 2d2d 0a20 2020 2064 6174 6173 6574  ----.    dataset
-00025c20: 3a20 5461 7554 4461 7461 7365 7420 7c20  : TauTDataset | 
-00025c30: 5461 7548 4461 7461 7365 740a 2020 2020  TauHDataset.    
-00025c40: 2020 2020 4461 7461 7365 7420 746f 2070      Dataset to p
-00025c50: 6c6f 740a 2020 2020 7368 6f77 3a20 626f  lot.    show: bo
-00025c60: 6f6c 2c20 6465 6661 756c 7420 5472 7565  ol, default True
-00025c70: 0a20 2020 2020 2020 2049 6620 5472 7565  .        If True
-00025c80: 2c20 7368 6f77 2070 6c6f 7420 6f6e 2073  , show plot on s
-00025c90: 6372 6565 6e0a 2020 2020 7361 7665 3a20  creen.    save: 
-00025ca0: 626f 6f6c 2c20 6465 6661 756c 7420 4661  bool, default Fa
-00025cb0: 6c73 650a 2020 2020 2020 2020 4966 2054  lse.        If T
-00025cc0: 7275 652c 2073 6176 6520 706c 6f74 2074  rue, save plot t
-00025cd0: 6f20 6669 6c65 2060 7361 7665 5f6e 616d  o file `save_nam
-00025ce0: 6560 0a20 2020 2073 6176 655f 6e61 6d65  e`.    save_name
-00025cf0: 3a20 7374 722c 2064 6566 6175 6c74 2027  : str, default '
-00025d00: 7265 6c61 7861 7469 6f6e 5f72 6174 6573  relaxation_rates
-00025d10: 2e70 6e67 270a 2020 2020 2020 2020 4966  .png'.        If
-00025d20: 2073 6176 6520 6973 2054 7275 652c 2077   save is True, w
-00025d30: 696c 6c20 7361 7665 2070 6c6f 7420 746f  ill save plot to
-00025d40: 2074 6869 7320 6669 6c65 6e61 6d65 0a20   this filename. 
-00025d50: 2020 2076 6572 626f 7365 3a20 626f 6f6c     verbose: bool
-00025d60: 2c20 6465 6661 756c 7420 5472 7565 0a20  , default True. 
-00025d70: 2020 2020 2020 2049 6620 5472 7565 2c20         If True, 
-00025d80: 706c 6f74 2066 696c 6520 6c6f 6361 7469  plot file locati
-00025d90: 6f6e 2069 7320 7772 6974 7465 6e20 746f  on is written to
-00025da0: 2074 6572 6d69 6e61 6c0a 0a20 2020 2052   terminal..    R
-00025db0: 6574 7572 6e73 0a20 2020 202d 2d2d 2d2d  eturns.    -----
-00025dc0: 2d2d 0a20 2020 2070 6c74 2e46 6967 7572  --.    plt.Figur
-00025dd0: 650a 2020 2020 2020 2020 4d61 7470 6c6f  e.        Matplo
-00025de0: 746c 6962 2066 6967 7572 6520 6f62 6a65  tlib figure obje
-00025df0: 6374 0a20 2020 2070 6c74 2e41 7865 730a  ct.    plt.Axes.
-00025e00: 2020 2020 2020 2020 4d61 7470 6c6f 746c          Matplotl
-00025e10: 6962 2061 7869 7320 6f62 6a65 6374 0a20  ib axis object. 
-00025e20: 2020 2027 2727 0a0a 2020 2020 2320 4372     '''..    # Cr
-00025e30: 6561 7465 2066 6967 7572 6520 616e 6420  eate figure and 
-00025e40: 6178 6573 0a20 2020 2066 6967 2c20 6178  axes.    fig, ax
-00025e50: 203d 2070 6c74 2e73 7562 706c 6f74 7328   = plt.subplots(
-00025e60: 0a20 2020 2020 2020 2031 2c0a 2020 2020  .        1,.    
-00025e70: 2020 2020 312c 0a20 2020 2020 2020 2073      1,.        s
-00025e80: 6861 7265 783d 5472 7565 2c0a 2020 2020  harex=True,.    
-00025e90: 2020 2020 7368 6172 6579 3d54 7275 652c      sharey=True,
-00025ea0: 0a20 2020 2020 2020 2066 6967 7369 7a65  .        figsize
-00025eb0: 3d28 362c 2036 292c 0a20 2020 2020 2020  =(6, 6),.       
-00025ec0: 206e 756d 3d27 4669 7474 6564 2072 656c   num='Fitted rel
-00025ed0: 6178 6174 696f 6e20 7072 6f66 696c 6527  axation profile'
-00025ee0: 0a20 2020 2029 0a0a 2020 2020 6966 2069  .    )..    if i
-00025ef0: 7369 6e73 7461 6e63 6528 6461 7461 7365  sinstance(datase
-00025f00: 742c 2054 6175 4844 6174 6173 6574 293a  t, TauHDataset):
-00025f10: 0a20 2020 2020 2020 2078 5f76 6172 7320  .        x_vars 
-00025f20: 3d20 6461 7461 7365 742e 6669 656c 6473  = dataset.fields
-00025f30: 0a20 2020 2020 2020 2061 782e 7365 745f  .        ax.set_
-00025f40: 786c 6162 656c 2872 2746 6965 6c64 2028  xlabel(r'Field (
-00025f50: 4f65 2927 290a 2020 2020 656c 6966 2069  Oe)').    elif i
-00025f60: 7369 6e73 7461 6e63 6528 6461 7461 7365  sinstance(datase
-00025f70: 742c 2054 6175 5444 6174 6173 6574 293a  t, TauTDataset):
-00025f80: 0a20 2020 2020 2020 2078 5f76 6172 7320  .        x_vars 
-00025f90: 3d20 6461 7461 7365 742e 7465 6d70 6572  = dataset.temper
-00025fa0: 6174 7572 6573 0a20 2020 2020 2020 2061  atures.        a
-00025fb0: 782e 7365 745f 786c 6162 656c 2872 2754  x.set_xlabel(r'T
-00025fc0: 656d 7065 7261 7475 7265 2028 4b29 2729  emperature (K)')
-00025fd0: 0a0a 2020 2020 2320 4164 6420 756e 6365  ..    # Add unce
-00025fe0: 7274 6169 6e74 6965 7320 6173 2065 7272  rtainties as err
-00025ff0: 6f72 6261 7273 0a20 2020 2069 6620 6c65  orbars.    if le
-00026000: 6e28 6461 7461 7365 742e 7261 7465 5f70  n(dataset.rate_p
-00026010: 6d29 3a0a 2020 2020 2020 2020 6178 2e65  m):.        ax.e
-00026020: 7272 6f72 6261 7228 0a20 2020 2020 2020  rrorbar(.       
-00026030: 2020 2020 2078 5f76 6172 732c 0a20 2020       x_vars,.   
-00026040: 2020 2020 2020 2020 2064 6174 6173 6574           dataset
-00026050: 2e72 6174 6573 2c0a 2020 2020 2020 2020  .rates,.        
-00026060: 2020 2020 7965 7272 3d64 6174 6173 6574      yerr=dataset
-00026070: 2e72 6174 655f 706d 2c0a 2020 2020 2020  .rate_pm,.      
-00026080: 2020 2020 2020 6d61 726b 6572 3d27 6f27        marker='o'
-00026090: 2c0a 2020 2020 2020 2020 2020 2020 6c77  ,.            lw
-000260a0: 3d30 2c0a 2020 2020 2020 2020 2020 2020  =0,.            
-000260b0: 656c 696e 6577 6964 7468 3d31 2e35 2c0a  elinewidth=1.5,.
-000260c0: 2020 2020 2020 2020 2020 2020 6669 6c6c              fill
-000260d0: 7374 796c 653d 276e 6f6e 6527 2c0a 2020  style='none',.  
-000260e0: 2020 2020 2020 2020 2020 636f 6c6f 723d            color=
-000260f0: 2762 6c61 636b 270a 2020 2020 2020 2020  'black'.        
-00026100: 290a 2020 2020 656c 7365 3a0a 2020 2020  ).    else:.    
-00026110: 2020 2020 6178 2e70 6c6f 7428 0a20 2020      ax.plot(.   
-00026120: 2020 2020 2020 2020 2078 5f76 6172 732c           x_vars,
-00026130: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
-00026140: 6173 6574 2e72 6174 6573 2c0a 2020 2020  aset.rates,.    
-00026150: 2020 2020 2020 2020 6d61 726b 6572 3d27          marker='
-00026160: 6f27 2c0a 2020 2020 2020 2020 2020 2020  o',.            
-00026170: 6c77 3d30 2c0a 2020 2020 2020 2020 2020  lw=0,.          
-00026180: 2020 6669 6c6c 7374 796c 653d 276e 6f6e    fillstyle='non
-00026190: 6527 2c0a 2020 2020 2020 2020 2020 2020  e',.            
-000261a0: 636f 6c6f 723d 2762 6c61 636b 270a 2020  color='black'.  
-000261b0: 2020 2020 2020 290a 0a20 2020 2061 782e        )..    ax.
-000261c0: 7365 745f 7873 6361 6c65 2827 6c6f 6727  set_xscale('log'
-000261d0: 290a 2020 2020 6178 2e73 6574 5f79 7363  ).    ax.set_ysc
-000261e0: 616c 6528 276c 6f67 2729 0a0a 2020 2020  ale('log')..    
-000261f0: 6178 2e73 6574 5f79 6c61 6265 6c28 7227  ax.set_ylabel(r'
-00026200: 5261 7465 2028 7324 5e5c 6d61 7468 7265  Rate (s$^\mathre
-00026210: 6775 6c61 727b 2d31 7d24 2927 290a 0a20  gular{-1}$)').. 
-00026220: 2020 2069 6620 6c65 6e28 6461 7461 7365     if len(datase
-00026230: 742e 6c6f 6772 6174 655f 706d 293a 0a20  t.lograte_pm):. 
-00026240: 2020 2020 2020 2061 6c6c 5f64 6174 6120         all_data 
-00026250: 3d20 5b0a 2020 2020 2020 2020 2020 2020  = [.            
-00026260: 6e70 2e6c 6f67 3130 2864 6174 6173 6574  np.log10(dataset
-00026270: 2e72 6174 6573 2920 2b20 6461 7461 7365  .rates) + datase
-00026280: 742e 6c6f 6772 6174 655f 706d 0a20 2020  t.lograte_pm.   
-00026290: 2020 2020 205d 0a20 2020 2020 2020 2061       ].        a
-000262a0: 6c6c 5f64 6174 6120 2b3d 205b 0a20 2020  ll_data += [.   
-000262b0: 2020 2020 2020 2020 206e 702e 6c6f 6731           np.log1
-000262c0: 3028 6461 7461 7365 742e 7261 7465 7329  0(dataset.rates)
-000262d0: 202d 2064 6174 6173 6574 2e6c 6f67 7261   - dataset.logra
-000262e0: 7465 5f70 6d0a 2020 2020 2020 2020 5d0a  te_pm.        ].
-000262f0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00026300: 2020 616c 6c5f 6461 7461 203d 205b 0a20    all_data = [. 
-00026310: 2020 2020 2020 2020 2020 206e 702e 6c6f             np.lo
-00026320: 6731 3028 6461 7461 7365 742e 7261 7465  g10(dataset.rate
-00026330: 7329 0a20 2020 2020 2020 205d 0a20 2020  s).        ].   
-00026340: 2020 2020 2061 6c6c 5f64 6174 6120 2b3d       all_data +=
-00026350: 205b 0a20 2020 2020 2020 2020 2020 206e   [.            n
-00026360: 702e 6c6f 6731 3028 6461 7461 7365 742e  p.log10(dataset.
-00026370: 7261 7465 7329 0a20 2020 2020 2020 205d  rates).        ]
-00026380: 0a0a 2020 2020 6775 692e 666f 726d 6174  ..    gui.format
-00026390: 5f72 6174 655f 785f 795f 6178 6573 280a  _rate_x_y_axes(.
-000263a0: 2020 2020 2020 2020 6178 2c0a 2020 2020          ax,.    
-000263b0: 2020 2020 6461 7461 7365 742e 7261 7465      dataset.rate
-000263c0: 732c 0a20 2020 2020 2020 2078 5f76 6172  s,.        x_var
-000263d0: 732c 0a20 2020 2020 2020 206e 702e 6162  s,.        np.ab
-000263e0: 7328 6461 7461 7365 742e 7261 7465 5f70  s(dataset.rate_p
-000263f0: 6d29 0a20 2020 2029 0a0a 2020 2020 2320  m).    )..    # 
-00026400: 5365 7420 7820 7469 636b 2066 6f72 6d61  Set x tick forma
-00026410: 7474 696e 670a 2020 2020 6775 692e 7365  tting.    gui.se
-00026420: 745f 7261 7465 5f78 7469 636b 5f66 6f72  t_rate_xtick_for
-00026430: 6d61 7474 696e 6728 6178 2c20 785f 7661  matting(ax, x_va
-00026440: 7273 290a 0a20 2020 2066 6967 2e74 6967  rs)..    fig.tig
-00026450: 6874 5f6c 6179 6f75 7428 290a 0a20 2020  ht_layout()..   
-00026460: 2069 6620 7361 7665 3a0a 2020 2020 2020   if save:.      
-00026470: 2020 706c 742e 7361 7665 6669 6728 7361    plt.savefig(sa
-00026480: 7665 5f6e 616d 6529 0a20 2020 2020 2020  ve_name).       
-00026490: 2069 6620 7665 7262 6f73 653a 0a20 2020   if verbose:.   
-000264a0: 2020 2020 2020 2020 2075 742e 6370 7269           ut.cpri
-000264b0: 6e74 280a 2020 2020 2020 2020 2020 2020  nt(.            
-000264c0: 2020 2020 6627 5c6e 2052 656c 6178 6174      f'\n Relaxat
-000264d0: 696f 6e20 706c 6f74 2073 6176 6564 2074  ion plot saved t
-000264e0: 6f20 5c6e 207b 7361 7665 5f6e 616d 657d  o \n {save_name}
-000264f0: 5c6e 272c 0a20 2020 2020 2020 2020 2020  \n',.           
-00026500: 2020 2020 2027 6379 616e 270a 2020 2020       'cyan'.    
-00026510: 2020 2020 2020 2020 290a 2020 2020 6966          ).    if
-00026520: 2073 686f 773a 0a20 2020 2020 2020 2070   show:.        p
-00026530: 6c74 2e73 686f 7728 290a 0a20 2020 2072  lt.show()..    r
-00026540: 6574 7572 6e20 6669 672c 2061 780a 0a0a  eturn fig, ax...
-00026550: 6465 6620 706c 6f74 5f72 6174 655f 7265  def plot_rate_re
-00026560: 7369 6475 616c 7328 6461 7461 7365 743a  siduals(dataset:
-00026570: 2054 6175 5444 6174 6173 6574 2c0a 2020   TauTDataset,.  
-00026580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026590: 2020 2020 2020 6d6f 6465 6c3a 204c 6f67        model: Log
-000265a0: 5461 7554 4d6f 6465 6c20 7c20 4d75 6c74  TauTModel | Mult
-000265b0: 694c 6f67 5461 7554 4d6f 6465 6c20 7c20  iLogTauTModel | 
-000265c0: 4c6f 6754 6175 484d 6f64 656c 207c 204d  LogTauHModel | M
-000265d0: 756c 7469 4c6f 6754 6175 484d 6f64 656c  ultiLogTauHModel
-000265e0: 2c20 2320 6e6f 7161 0a20 2020 2020 2020  , # noqa.       
-000265f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026600: 2073 6176 653a 2062 6f6f 6c20 3d20 4661   save: bool = Fa
-00026610: 6c73 652c 2073 686f 773a 2062 6f6f 6c20  lse, show: bool 
-00026620: 3d20 5472 7565 2c0a 2020 2020 2020 2020  = True,.        
-00026630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026640: 7361 7665 5f6e 616d 653a 2073 7472 203d  save_name: str =
-00026650: 2027 6d6f 6465 6c5f 7265 7369 6475 616c   'model_residual
-00026660: 5f74 6175 2e70 6e67 272c 0a20 2020 2020  _tau.png',.     
-00026670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026680: 2020 2076 6572 626f 7365 3a20 626f 6f6c     verbose: bool
-00026690: 203d 2054 7275 6529 202d 3e20 7475 706c   = True) -> tupl
-000266a0: 655b 706c 742e 4669 6775 7265 2c20 706c  e[plt.Figure, pl
-000266b0: 742e 4178 6573 5d3a 0a20 2020 2027 2727  t.Axes]:.    '''
-000266c0: 0a20 2020 2050 6c6f 7473 2064 6966 6665  .    Plots diffe
-000266d0: 7265 6e63 6520 6f66 206c 6f67 3130 2865  rence of log10(e
-000266e0: 7870 6572 696d 656e 7429 2061 6e64 206c  xperiment) and l
-000266f0: 6f67 3130 286d 6f64 656c 2920 7265 6c61  og10(model) rela
-00026700: 7861 7469 6f6e 2072 6174 6573 0a20 2020  xation rates.   
-00026710: 2028 6c6f 6731 3028 6578 7065 7269 6d65   (log10(experime
-00026720: 6e74 5f72 6174 6529 202d 206c 6f67 3130  nt_rate) - log10
-00026730: 286d 6f64 656c 5f72 6174 6529 2076 7320  (model_rate) vs 
-00026740: 5465 6d70 6572 6174 7572 6520 6f72 2046  Temperature or F
-00026750: 6965 6c64 290a 0a20 2020 2050 6172 616d  ield)..    Param
-00026760: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
-00026770: 2d2d 2d2d 0a20 2020 2064 6174 6173 6574  ----.    dataset
-00026780: 3a20 5461 7554 4461 7461 7365 7420 7c20  : TauTDataset | 
-00026790: 5461 7548 4461 7461 7365 740a 2020 2020  TauHDataset.    
-000267a0: 2020 2020 4461 7461 7365 7420 746f 2070      Dataset to p
-000267b0: 6c6f 740a 2020 2020 6d6f 6465 6c3a 204c  lot.    model: L
-000267c0: 6f67 5461 7554 4d6f 6465 6c20 7c20 4d75  ogTauTModel | Mu
-000267d0: 6c74 694c 6f67 5461 7554 4d6f 6465 6c20  ltiLogTauTModel 
-000267e0: 7c20 4c6f 6754 6175 484d 6f64 656c 207c  | LogTauHModel |
-000267f0: 204d 756c 7469 4c6f 6754 6175 484d 6f64   MultiLogTauHMod
-00026800: 656c 0a20 2020 2020 2020 204d 6f64 656c  el.        Model
-00026810: 2028 6669 7474 6564 2920 746f 2070 6c6f   (fitted) to plo
-00026820: 740a 2020 2020 7368 6f77 3a20 626f 6f6c  t.    show: bool
-00026830: 2c20 6465 6661 756c 7420 5472 7565 0a20  , default True. 
-00026840: 2020 2020 2020 2049 6620 5472 7565 2c20         If True, 
-00026850: 7368 6f77 2070 6c6f 7420 6f6e 2073 6372  show plot on scr
-00026860: 6565 6e0a 2020 2020 7361 7665 3a20 626f  een.    save: bo
-00026870: 6f6c 2c20 6465 6661 756c 7420 4661 6c73  ol, default Fals
-00026880: 650a 2020 2020 2020 2020 4966 2054 7275  e.        If Tru
-00026890: 652c 2073 6176 6520 706c 6f74 2074 6f20  e, save plot to 
-000268a0: 6669 6c65 2060 7361 7665 5f6e 616d 6560  file `save_name`
-000268b0: 0a20 2020 2073 6176 655f 6e61 6d65 3a20  .    save_name: 
-000268c0: 7374 722c 2064 6566 6175 6c74 2027 6d6f  str, default 'mo
-000268d0: 6465 6c5f 7265 7369 6475 616c 5f74 6175  del_residual_tau
-000268e0: 2e70 6e67 270a 2020 2020 2020 2020 4966  .png'.        If
-000268f0: 2073 6176 6520 6973 2054 7275 652c 2077   save is True, w
-00026900: 696c 6c20 7361 7665 2070 6c6f 7420 746f  ill save plot to
-00026910: 2074 6869 7320 6669 6c65 6e61 6d65 0a20   this filename. 
-00026920: 2020 2076 6572 626f 7365 3a20 626f 6f6c     verbose: bool
-00026930: 2c20 6465 6661 756c 7420 5472 7565 0a20  , default True. 
-00026940: 2020 2020 2020 2049 6620 5472 7565 2c20         If True, 
-00026950: 706c 6f74 2066 696c 6520 6c6f 6361 7469  plot file locati
-00026960: 6f6e 2069 7320 7772 6974 7465 6e20 746f  on is written to
-00026970: 2074 6572 6d69 6e61 6c0a 0a20 2020 2052   terminal..    R
-00026980: 6574 7572 6e73 0a20 2020 202d 2d2d 2d2d  eturns.    -----
-00026990: 2d2d 0a20 2020 2070 6c74 2e46 6967 7572  --.    plt.Figur
-000269a0: 650a 2020 2020 2020 2020 4d61 7470 6c6f  e.        Matplo
-000269b0: 746c 6962 2066 6967 7572 6520 6f62 6a65  tlib figure obje
-000269c0: 6374 0a20 2020 2070 6c74 2e41 7865 730a  ct.    plt.Axes.
-000269d0: 2020 2020 2020 2020 4d61 7470 6c6f 746c          Matplotl
-000269e0: 6962 2061 7869 7320 6f62 6a65 6374 0a20  ib axis object. 
-000269f0: 2020 2027 2727 0a20 2020 2023 2043 7265     '''.    # Cre
-00026a00: 6174 6520 6669 6775 7265 2061 6e64 2061  ate figure and a
-00026a10: 7865 730a 2020 2020 6669 672c 2061 7820  xes.    fig, ax 
-00026a20: 3d20 706c 742e 7375 6270 6c6f 7473 280a  = plt.subplots(.
-00026a30: 2020 2020 2020 2020 312c 0a20 2020 2020          1,.     
-00026a40: 2020 2031 2c0a 2020 2020 2020 2020 6669     1,.        fi
-00026a50: 6773 697a 653d 5b36 2c20 365d 2c0a 2020  gsize=[6, 6],.  
-00026a60: 2020 2020 2020 6e75 6d3d 2752 6573 6964        num='Resid
-00026a70: 7561 6c73 270a 2020 2020 290a 0a20 2020  uals'.    )..   
-00026a80: 205f 706c 6f74 5f72 6174 655f 7265 7369   _plot_rate_resi
-00026a90: 6475 616c 7328 6461 7461 7365 742c 206d  duals(dataset, m
-00026aa0: 6f64 656c 2c20 6178 290a 0a20 2020 2066  odel, ax)..    f
-00026ab0: 6967 2e74 6967 6874 5f6c 6179 6f75 7428  ig.tight_layout(
-00026ac0: 290a 0a20 2020 2023 2053 6176 6520 706c  )..    # Save pl
-00026ad0: 6f74 0a20 2020 2069 6620 7361 7665 3a0a  ot.    if save:.
-00026ae0: 2020 2020 2020 2020 706c 742e 7361 7665          plt.save
-00026af0: 6669 6728 7361 7665 5f6e 616d 652c 2064  fig(save_name, d
-00026b00: 7069 3d33 3030 290a 2020 2020 2020 2020  pi=300).        
-00026b10: 6966 2076 6572 626f 7365 3a0a 2020 2020  if verbose:.    
-00026b20: 2020 2020 2020 2020 7574 2e63 7072 696e          ut.cprin
-00026b30: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
-00026b40: 2020 2066 275c 6e20 5261 7465 2072 6573     f'\n Rate res
-00026b50: 6964 7561 6c73 2070 6c6f 7420 7361 7665  iduals plot save
-00026b60: 6420 746f 205c 6e20 7b73 6176 655f 6e61  d to \n {save_na
-00026b70: 6d65 7d5c 6e27 2c0a 2020 2020 2020 2020  me}\n',.        
-00026b80: 2020 2020 2020 2020 2763 7961 6e27 0a20          'cyan'. 
-00026b90: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00026ba0: 2069 6620 7368 6f77 3a0a 2020 2020 2020   if show:.      
-00026bb0: 2020 706c 742e 7368 6f77 2829 0a0a 2020    plt.show()..  
-00026bc0: 2020 7265 7475 726e 2066 6967 2c20 6178    return fig, ax
-00026bd0: 0a0a 0a64 6566 2071 745f 706c 6f74 5f72  ...def qt_plot_r
-00026be0: 6174 655f 7265 7369 6475 616c 7328 6170  ate_residuals(ap
-00026bf0: 703a 2051 7457 6964 6765 7473 2e51 4170  p: QtWidgets.QAp
-00026c00: 706c 6963 6174 696f 6e2c 2064 6174 6173  plication, datas
-00026c10: 6574 3a20 5461 7554 4461 7461 7365 742c  et: TauTDataset,
-00026c20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00026c30: 2020 2020 2020 2020 2020 2020 6d6f 6465              mode
-00026c40: 6c3a 204c 6f67 5461 7554 4d6f 6465 6c20  l: LogTauTModel 
-00026c50: 7c20 4d75 6c74 694c 6f67 5461 7554 4d6f  | MultiLogTauTMo
-00026c60: 6465 6c20 7c20 4c6f 6754 6175 484d 6f64  del | LogTauHMod
-00026c70: 656c 207c 204d 756c 7469 4c6f 6754 6175  el | MultiLogTau
-00026c80: 484d 6f64 656c 2c20 2320 6e6f 7161 0a20  HModel, # noqa. 
-00026c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026ca0: 2020 2020 2020 2020 2020 7361 7665 3a20            save: 
-00026cb0: 626f 6f6c 203d 2046 616c 7365 2c20 7368  bool = False, sh
-00026cc0: 6f77 3a20 626f 6f6c 203d 2054 7275 652c  ow: bool = True,
-00026cd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00026ce0: 2020 2020 2020 2020 2020 2020 7361 7665              save
-00026cf0: 5f6e 616d 653a 2073 7472 203d 2027 6d6f  _name: str = 'mo
-00026d00: 6465 6c5f 7265 7369 6475 616c 5f74 6175  del_residual_tau
-00026d10: 2e70 6e67 272c 0a20 2020 2020 2020 2020  .png',.         
-00026d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026d30: 2020 7665 7262 6f73 653a 2062 6f6f 6c20    verbose: bool 
-00026d40: 3d20 5472 7565 2920 2d3e 204e 6f6e 653a  = True) -> None:
-00026d50: 0a20 2020 2027 2727 0a20 2020 2050 6c6f  .    '''.    Plo
-00026d60: 7473 2064 6966 6665 7265 6e63 6520 6f66  ts difference of
-00026d70: 206c 6f67 3130 2865 7870 6572 696d 656e   log10(experimen
-00026d80: 7429 2061 6e64 206c 6f67 3130 286d 6f64  t) and log10(mod
-00026d90: 656c 2920 7265 6c61 7861 7469 6f6e 2072  el) relaxation r
-00026da0: 6174 6573 0a20 2020 2069 6e20 6120 7174  ates.    in a qt
-00026db0: 2077 696e 646f 7720 7573 696e 6720 6d61   window using ma
-00026dc0: 7470 6c6f 746c 6962 0a0a 2020 2020 5061  tplotlib..    Pa
-00026dd0: 7261 6d65 7465 7273 0a20 2020 202d 2d2d  rameters.    ---
-00026de0: 2d2d 2d2d 2d2d 2d0a 2020 2020 6170 703a  -------.    app:
-00026df0: 2051 7457 6964 6765 7473 2e51 4170 706c   QtWidgets.QAppl
-00026e00: 6963 6174 696f 6e0a 2020 2020 2020 2020  ication.        
-00026e10: 4170 706c 6963 6174 696f 6e20 7573 6564  Application used
-00026e20: 2062 7920 6375 7272 656e 7420 7072 6f67   by current prog
-00026e30: 7261 6d0a 2020 2020 2020 2020 4372 6561  ram.        Crea
-00026e40: 7465 2077 6974 6820 6061 7070 3d51 7457  te with `app=QtW
-00026e50: 6964 6765 7473 2e51 4170 706c 6963 6174  idgets.QApplicat
-00026e60: 696f 6e28 5b5d 2960 0a20 2020 2064 6174  ion([])`.    dat
-00026e70: 6173 6574 3a20 5461 7554 4461 7461 7365  aset: TauTDatase
-00026e80: 7420 7c20 5461 7548 4461 7461 7365 740a  t | TauHDataset.
-00026e90: 2020 2020 2020 2020 4461 7461 7365 7420          Dataset 
-00026ea0: 746f 2070 6c6f 740a 2020 2020 6d6f 6465  to plot.    mode
-00026eb0: 6c3a 204c 6f67 5461 7554 4d6f 6465 6c20  l: LogTauTModel 
-00026ec0: 7c20 4d75 6c74 694c 6f67 5461 7554 4d6f  | MultiLogTauTMo
-00026ed0: 6465 6c20 7c20 4c6f 6754 6175 484d 6f64  del | LogTauHMod
-00026ee0: 656c 207c 204d 756c 7469 4c6f 6754 6175  el | MultiLogTau
-00026ef0: 484d 6f64 656c 0a20 2020 2020 2020 204d  HModel.        M
-00026f00: 6f64 656c 2028 6669 7474 6564 2920 746f  odel (fitted) to
-00026f10: 2070 6c6f 740a 2020 2020 7368 6f77 3a20   plot.    show: 
-00026f20: 626f 6f6c 2c20 6465 6661 756c 7420 5472  bool, default Tr
-00026f30: 7565 0a20 2020 2020 2020 2049 6620 5472  ue.        If Tr
-00026f40: 7565 2c20 7368 6f77 2070 6c6f 7420 6f6e  ue, show plot on
-00026f50: 2073 6372 6565 6e0a 2020 2020 7361 7665   screen.    save
-00026f60: 3a20 626f 6f6c 2c20 6465 6661 756c 7420  : bool, default 
-00026f70: 4661 6c73 650a 2020 2020 2020 2020 4966  False.        If
-00026f80: 2054 7275 652c 2073 6176 6520 706c 6f74   True, save plot
-00026f90: 2074 6f20 6669 6c65 2060 7361 7665 5f6e   to file `save_n
-00026fa0: 616d 6560 0a20 2020 2073 6176 655f 6e61  ame`.    save_na
-00026fb0: 6d65 3a20 7374 722c 2064 6566 6175 6c74  me: str, default
-00026fc0: 2027 6d6f 6465 6c5f 7265 7369 6475 616c   'model_residual
-00026fd0: 5f74 6175 2e70 6e67 270a 2020 2020 2020  _tau.png'.      
-00026fe0: 2020 4966 2073 6176 6520 6973 2054 7275    If save is Tru
-00026ff0: 652c 2077 696c 6c20 7361 7665 2070 6c6f  e, will save plo
-00027000: 7420 746f 2074 6869 7320 6669 6c65 6e61  t to this filena
-00027010: 6d65 0a20 2020 2076 6572 626f 7365 3a20  me.    verbose: 
-00027020: 626f 6f6c 2c20 6465 6661 756c 7420 5472  bool, default Tr
-00027030: 7565 0a20 2020 2020 2020 2049 6620 5472  ue.        If Tr
-00027040: 7565 2c20 706c 6f74 2066 696c 6520 6c6f  ue, plot file lo
-00027050: 6361 7469 6f6e 2069 7320 7772 6974 7465  cation is writte
-00027060: 6e20 746f 2074 6572 6d69 6e61 6c0a 0a20  n to terminal.. 
-00027070: 2020 2052 6574 7572 6e73 0a20 2020 202d     Returns.    -
-00027080: 2d2d 2d2d 2d2d 0a20 2020 204e 6f6e 650a  ------.    None.
-00027090: 2020 2020 2727 270a 0a20 2020 2077 696e      '''..    win
-000270a0: 646f 7720 3d20 6775 692e 4d61 7470 6c6f  dow = gui.Matplo
-000270b0: 746c 6962 5769 6e64 6f77 2829 0a20 2020  tlibWindow().   
-000270c0: 2077 696e 646f 772e 7365 7457 696e 646f   window.setWindo
-000270d0: 7754 6974 6c65 2827 5265 7369 6475 616c  wTitle('Residual
-000270e0: 7327 290a 0a20 2020 205f 706c 6f74 5f72  s')..    _plot_r
-000270f0: 6174 655f 7265 7369 6475 616c 7328 6461  ate_residuals(da
-00027100: 7461 7365 742c 206d 6f64 656c 2c20 7769  taset, model, wi
-00027110: 6e64 6f77 2e73 632e 6178 290a 0a20 2020  ndow.sc.ax)..   
-00027120: 2023 2053 6176 6520 706c 6f74 0a20 2020   # Save plot.   
-00027130: 2069 6620 7361 7665 3a0a 2020 2020 2020   if save:.      
-00027140: 2020 7769 6e64 6f77 2e73 632e 6669 672e    window.sc.fig.
-00027150: 7361 7665 6669 6728 7361 7665 5f6e 616d  savefig(save_nam
-00027160: 652c 2064 7069 3d33 3030 290a 2020 2020  e, dpi=300).    
-00027170: 2020 2020 6966 2076 6572 626f 7365 3a0a      if verbose:.
-00027180: 2020 2020 2020 2020 2020 2020 7574 2e63              ut.c
-00027190: 7072 696e 7428 0a20 2020 2020 2020 2020  print(.         
-000271a0: 2020 2020 2020 2066 275c 6e20 5261 7465         f'\n Rate
-000271b0: 2072 6573 6964 7561 6c73 2070 6c6f 7420   residuals plot 
-000271c0: 7361 7665 6420 746f 205c 6e20 7b73 6176  saved to \n {sav
-000271d0: 655f 6e61 6d65 7d5c 6e27 2c0a 2020 2020  e_name}\n',.    
-000271e0: 2020 2020 2020 2020 2020 2020 2763 7961              'cya
-000271f0: 6e27 0a20 2020 2020 2020 2020 2020 2029  n'.            )
-00027200: 0a0a 2020 2020 6966 2073 686f 773a 0a20  ..    if show:. 
-00027210: 2020 2020 2020 2077 696e 646f 772e 7368         window.sh
-00027220: 6f77 2829 0a20 2020 2020 2020 2023 2043  ow().        # C
-00027230: 616c 6c20 7477 6963 6520 656c 7365 2069  all twice else i
-00027240: 7420 776f 6e74 2077 6f72 6b21 0a20 2020  t wont work!.   
-00027250: 2020 2020 2077 696e 646f 772e 7363 2e66       window.sc.f
-00027260: 6967 2e74 6967 6874 5f6c 6179 6f75 7428  ig.tight_layout(
-00027270: 290a 2020 2020 2020 2020 7769 6e64 6f77  ).        window
-00027280: 2e73 632e 6669 672e 7469 6768 745f 6c61  .sc.fig.tight_la
-00027290: 796f 7574 2829 0a20 2020 2020 2020 2061  yout().        a
-000272a0: 7070 2e65 7865 635f 2829 0a0a 2020 2020  pp.exec_()..    
-000272b0: 7265 7475 726e 0a0a 0a64 6566 205f 706c  return...def _pl
-000272c0: 6f74 5f72 6174 655f 7265 7369 6475 616c  ot_rate_residual
-000272d0: 7328 6461 7461 7365 743a 2054 6175 5444  s(dataset: TauTD
-000272e0: 6174 6173 6574 207c 2054 6175 4844 6174  ataset | TauHDat
-000272f0: 6173 6574 2c0a 2020 2020 2020 2020 2020  aset,.          
-00027300: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00027310: 6f64 656c 3a20 4c6f 6754 6175 544d 6f64  odel: LogTauTMod
-00027320: 656c 207c 204d 756c 7469 4c6f 6754 6175  el | MultiLogTau
-00027330: 544d 6f64 656c 207c 204c 6f67 5461 7548  TModel | LogTauH
-00027340: 4d6f 6465 6c20 7c20 4d75 6c74 694c 6f67  Model | MultiLog
-00027350: 5461 7548 4d6f 6465 6c2c 2023 206e 6f71  TauHModel, # noq
-00027360: 610a 2020 2020 2020 2020 2020 2020 2020  a.              
-00027370: 2020 2020 2020 2020 2020 2061 783a 2070             ax: p
-00027380: 6c74 2e41 7865 7329 202d 3e20 4e6f 6e65  lt.Axes) -> None
-00027390: 3a0a 2020 2020 2727 270a 2020 2020 506c  :.    '''.    Pl
-000273a0: 6f74 7320 6469 6666 6572 656e 6365 206f  ots difference o
-000273b0: 6620 6c6f 6731 3028 6578 7065 7269 6d65  f log10(experime
-000273c0: 6e74 2920 616e 6420 6c6f 6731 3028 6d6f  nt) and log10(mo
-000273d0: 6465 6c29 2072 656c 6178 6174 696f 6e20  del) relaxation 
-000273e0: 7261 7465 730a 2020 2020 6f6e 746f 2061  rates.    onto a
-000273f0: 2067 6976 656e 2066 6967 7572 6520 616e   given figure an
-00027400: 6420 6178 6973 0a0a 2020 2020 5061 7261  d axis..    Para
-00027410: 6d65 7465 7273 0a20 2020 202d 2d2d 2d2d  meters.    -----
-00027420: 2d2d 2d2d 2d0a 2020 2020 6d6f 6465 6c73  -----.    models
-00027430: 3a20 6c69 7374 5b4c 6f67 5461 7554 4d6f  : list[LogTauTMo
-00027440: 6465 6c20 7c20 4d75 6c74 694c 6f67 5461  del | MultiLogTa
-00027450: 7554 4d6f 6465 6c20 7c20 4c6f 6754 6175  uTModel | LogTau
-00027460: 484d 6f64 656c 207c 204d 756c 7469 4c6f  HModel | MultiLo
-00027470: 6754 6175 484d 6f64 656c 5d0a 2020 2020  gTauHModel].    
-00027480: 2020 2020 4d6f 6465 6c73 2c20 6f6e 6520      Models, one 
-00027490: 7065 7220 7465 6d70 6572 6174 7572 650a  per temperature.
-000274a0: 2020 2020 6669 6c65 5f6e 616d 653a 2073      file_name: s
-000274b0: 7472 0a20 2020 2020 2020 204e 616d 6520  tr.        Name 
-000274c0: 6f66 206f 7574 7075 7420 6669 6c65 0a20  of output file. 
-000274d0: 2020 2061 783a 2070 6c74 2e41 7865 730a     ax: plt.Axes.
-000274e0: 2020 2020 2020 2020 4d61 7470 6c6f 746c          Matplotl
-000274f0: 6962 2041 7869 7320 6f62 6a65 6374 2075  ib Axis object u
-00027500: 7365 6420 666f 7220 706c 6f74 0a0a 2020  sed for plot..  
-00027510: 2020 5265 7475 726e 730a 2020 2020 2d2d    Returns.    --
-00027520: 2d2d 2d2d 2d0a 2020 2020 4e6f 6e65 0a20  -----.    None. 
-00027530: 2020 2027 2727 2023 206e 6f71 610a 0a20     ''' # noqa.. 
-00027540: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-00027550: 2864 6174 6173 6574 2c20 5461 7548 4461  (dataset, TauHDa
-00027560: 7461 7365 7429 3a0a 2020 2020 2020 2020  taset):.        
-00027570: 785f 7661 7273 203d 2064 6174 6173 6574  x_vars = dataset
-00027580: 2e66 6965 6c64 730a 2020 2020 2020 2020  .fields.        
-00027590: 6178 2e73 6574 5f78 6c61 6265 6c28 7227  ax.set_xlabel(r'
-000275a0: 4669 656c 6420 284f 6529 2729 0a20 2020  Field (Oe)').   
-000275b0: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
-000275c0: 2864 6174 6173 6574 2c20 5461 7554 4461  (dataset, TauTDa
-000275d0: 7461 7365 7429 3a0a 2020 2020 2020 2020  taset):.        
-000275e0: 785f 7661 7273 203d 2064 6174 6173 6574  x_vars = dataset
-000275f0: 2e74 656d 7065 7261 7475 7265 730a 2020  .temperatures.  
-00027600: 2020 2020 2020 6178 2e73 6574 5f78 6c61        ax.set_xla
-00027610: 6265 6c28 7227 5465 6d70 6572 6174 7572  bel(r'Temperatur
-00027620: 6520 284b 2927 290a 0a20 2020 2023 2041  e (K)')..    # A
-00027630: 6464 2061 6464 6974 696f 6e61 6c20 7365  dd additional se
-00027640: 7420 6f66 2061 7865 7320 746f 2063 7265  t of axes to cre
-00027650: 6174 6520 277a 6572 6f27 206c 696e 650a  ate 'zero' line.
-00027660: 2020 2020 6178 3220 3d20 6178 2e74 7769      ax2 = ax.twi
-00027670: 6e79 2829 0a20 2020 2061 7832 2e67 6574  ny().    ax2.get
-00027680: 5f79 6178 6973 2829 2e73 6574 5f76 6973  _yaxis().set_vis
-00027690: 6962 6c65 2846 616c 7365 290a 2020 2020  ible(False).    
-000276a0: 6178 322e 7365 745f 7974 6963 6b73 285b  ax2.set_yticks([
-000276b0: 5d29 0a20 2020 2061 7832 2e73 6574 5f78  ]).    ax2.set_x
-000276c0: 7469 636b 7328 5b5d 290a 2020 2020 6178  ticks([]).    ax
-000276d0: 322e 7370 696e 6573 5b27 626f 7474 6f6d  2.spines['bottom
-000276e0: 275d 2e73 6574 5f70 6f73 6974 696f 6e28  '].set_position(
-000276f0: 2827 7a65 726f 2729 290a 0a20 2020 2069  ('zero'))..    i
-00027700: 6620 7479 7065 286d 6f64 656c 2920 696e  f type(model) in
-00027710: 205b 4d75 6c74 694c 6f67 5461 7554 4d6f   [MultiLogTauTMo
-00027720: 6465 6c2c 204d 756c 7469 4c6f 6754 6175  del, MultiLogTau
-00027730: 484d 6f64 656c 5d3a 0a20 2020 2020 2020  HModel]:.       
-00027740: 206c 6f67 6d6f 6465 6c73 203d 206d 6f64   logmodels = mod
-00027750: 656c 2e6c 6f67 6d6f 6465 6c73 0a20 2020  el.logmodels.   
-00027760: 2065 6c73 653a 0a20 2020 2020 2020 206c   else:.        l
-00027770: 6f67 6d6f 6465 6c73 203d 205b 6d6f 6465  ogmodels = [mode
-00027780: 6c5d 0a0a 2020 2020 6d6f 6465 6c5f 7261  l]..    model_ra
-00027790: 7465 203d 206e 702e 7a65 726f 7328 6c65  te = np.zeros(le
-000277a0: 6e28 785f 7661 7273 2929 0a0a 2020 2020  n(x_vars))..    
-000277b0: 666f 7220 6c6f 676d 6f64 656c 2069 6e20  for logmodel in 
-000277c0: 6c6f 676d 6f64 656c 733a 0a20 2020 2020  logmodels:.     
-000277d0: 2020 206d 6f64 656c 5f72 6174 6520 2b3d     model_rate +=
-000277e0: 2031 302a 2a6c 6f67 6d6f 6465 6c2e 6d6f   10**logmodel.mo
-000277f0: 6465 6c28 0a20 2020 2020 2020 2020 2020  del(.           
-00027800: 206c 6f67 6d6f 6465 6c2e 6669 6e61 6c5f   logmodel.final_
-00027810: 7661 725f 7661 6c75 6573 2c0a 2020 2020  var_values,.    
-00027820: 2020 2020 2020 2020 785f 7661 7273 2c0a          x_vars,.
-00027830: 2020 2020 2020 2020 290a 0a20 2020 206d          )..    m
-00027840: 6f64 656c 5f6c 6f67 7261 7465 203d 206e  odel_lograte = n
-00027850: 702e 6c6f 6731 3028 6d6f 6465 6c5f 7261  p.log10(model_ra
-00027860: 7465 290a 0a20 2020 2023 2050 6c6f 7420  te)..    # Plot 
-00027870: 7265 7369 6475 616c 730a 2020 2020 6966  residuals.    if
-00027880: 206c 656e 2864 6174 6173 6574 2e6c 6f67   len(dataset.log
-00027890: 7261 7465 5f70 6d29 3a0a 2020 2020 2020  rate_pm):.      
-000278a0: 2020 6178 2e65 7272 6f72 6261 7228 0a20    ax.errorbar(. 
-000278b0: 2020 2020 2020 2020 2020 2078 5f76 6172             x_var
-000278c0: 732c 0a20 2020 2020 2020 2020 2020 206e  s,.            n
-000278d0: 702e 6c6f 6731 3028 6461 7461 7365 742e  p.log10(dataset.
-000278e0: 7261 7465 7329 202d 206d 6f64 656c 5f6c  rates) - model_l
-000278f0: 6f67 7261 7465 2c0a 2020 2020 2020 2020  ograte,.        
-00027900: 2020 2020 7965 7272 3d64 6174 6173 6574      yerr=dataset
-00027910: 2e6c 6f67 7261 7465 5f70 6d2c 0a20 2020  .lograte_pm,.   
-00027920: 2020 2020 2020 2020 2066 6d74 3d27 622e           fmt='b.
-00027930: 270a 2020 2020 2020 2020 290a 2020 2020  '.        ).    
-00027940: 656c 7365 3a0a 2020 2020 2020 2020 6178  else:.        ax
-00027950: 2e70 6c6f 7428 0a20 2020 2020 2020 2020  .plot(.         
-00027960: 2020 2078 5f76 6172 732c 0a20 2020 2020     x_vars,.     
-00027970: 2020 2020 2020 206e 702e 6c6f 6731 3028         np.log10(
-00027980: 6461 7461 7365 742e 7261 7465 7329 202d  dataset.rates) -
-00027990: 206d 6f64 656c 5f6c 6f67 7261 7465 2c0a   model_lograte,.
-000279a0: 2020 2020 2020 2020 2020 2020 636f 6c6f              colo
-000279b0: 723d 2762 272c 0a20 2020 2020 2020 2020  r='b',.         
-000279c0: 2020 206d 6172 6b65 723d 276f 272c 0a20     marker='o',. 
-000279d0: 2020 2020 2020 2020 2020 206c 773d 302c             lw=0,
-000279e0: 0a20 2020 2020 2020 2020 2020 2066 696c  .            fil
-000279f0: 6c73 7479 6c65 3d27 6e6f 6e65 272c 0a20  lstyle='none',. 
-00027a00: 2020 2020 2020 2020 2020 206c 6162 656c             label
-00027a10: 3d27 4578 7065 7269 6d65 6e74 270a 2020  ='Experiment'.  
-00027a20: 2020 2020 2020 290a 2020 2020 2320 5365        ).    # Se
-00027a30: 7420 6c6f 6720 7363 616c 6520 6f6e 2078  t log scale on x
-00027a40: 2061 7869 730a 2020 2020 6178 2e73 6574   axis.    ax.set
-00027a50: 5f78 7363 616c 6528 276c 6f67 2729 0a0a  _xscale('log')..
-00027a60: 2020 2020 2320 5365 7420 666f 726d 6174      # Set format
-00027a70: 7469 6e67 2066 6f72 2079 2061 7869 7320  ting for y axis 
-00027a80: 6d61 6a6f 7220 7469 636b 730a 2020 2020  major ticks.    
-00027a90: 6178 2e79 6178 6973 2e73 6574 5f6d 616a  ax.yaxis.set_maj
-00027aa0: 6f72 5f66 6f72 6d61 7474 6572 2853 6361  or_formatter(Sca
-00027ab0: 6c61 7246 6f72 6d61 7474 6572 2829 290a  larFormatter()).
-00027ac0: 0a20 2020 2023 2041 6464 206d 696e 6f72  .    # Add minor
-00027ad0: 2074 6963 6b73 2074 6f20 7920 6178 6973   ticks to y axis
-00027ae0: 2077 6974 6820 6e6f 206c 6162 656c 730a   with no labels.
-00027af0: 2020 2020 6178 2e79 6178 6973 2e73 6574      ax.yaxis.set
-00027b00: 5f6d 696e 6f72 5f6c 6f63 6174 6f72 2841  _minor_locator(A
-00027b10: 7574 6f4d 696e 6f72 4c6f 6361 746f 7228  utoMinorLocator(
-00027b20: 2929 0a0a 2020 2020 2320 5379 6d6d 6574  ))..    # Symmet
-00027b30: 7269 7365 2079 2061 7869 7320 6c69 6d69  rise y axis limi
-00027b40: 7473 2062 6173 6564 206f 6e20 6d61 7820  ts based on max 
-00027b50: 6162 7320 6572 726f 720a 2020 2020 6966  abs error.    if
-00027b60: 206c 656e 2864 6174 6173 6574 2e6c 6f67   len(dataset.log
-00027b70: 7261 7465 5f70 6d29 3a0a 2020 2020 2020  rate_pm):.      
-00027b80: 2020 616c 6c5f 6461 7461 203d 205b 0a20    all_data = [. 
-00027b90: 2020 2020 2020 2020 2020 206e 702e 6c6f             np.lo
-00027ba0: 6731 3028 6461 7461 7365 742e 7261 7465  g10(dataset.rate
-00027bb0: 7329 202d 206d 6f64 656c 5f6c 6f67 7261  s) - model_logra
-00027bc0: 7465 202b 2064 6174 6173 6574 2e6c 6f67  te + dataset.log
-00027bd0: 7261 7465 5f70 6d0a 2020 2020 2020 2020  rate_pm.        
-00027be0: 5d0a 2020 2020 2020 2020 616c 6c5f 6461  ].        all_da
-00027bf0: 7461 202b 3d20 5b0a 2020 2020 2020 2020  ta += [.        
-00027c00: 2020 2020 6e70 2e6c 6f67 3130 2864 6174      np.log10(dat
-00027c10: 6173 6574 2e72 6174 6573 2920 2d20 6d6f  aset.rates) - mo
-00027c20: 6465 6c5f 6c6f 6772 6174 6520 2d20 6461  del_lograte - da
-00027c30: 7461 7365 742e 6c6f 6772 6174 655f 706d  taset.lograte_pm
-00027c40: 0a20 2020 2020 2020 205d 0a20 2020 2065  .        ].    e
-00027c50: 6c73 653a 0a20 2020 2020 2020 2061 6c6c  lse:.        all
-00027c60: 5f64 6174 6120 3d20 5b0a 2020 2020 2020  _data = [.      
-00027c70: 2020 2020 2020 6e70 2e6c 6f67 3130 2864        np.log10(d
-00027c80: 6174 6173 6574 2e72 6174 6573 2920 2d20  ataset.rates) - 
-00027c90: 6d6f 6465 6c5f 6c6f 6772 6174 650a 2020  model_lograte.  
-00027ca0: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
-00027cb0: 616c 6c5f 6461 7461 202b 3d20 5b0a 2020  all_data += [.  
-00027cc0: 2020 2020 2020 2020 2020 6e70 2e6c 6f67            np.log
-00027cd0: 3130 2864 6174 6173 6574 2e72 6174 6573  10(dataset.rates
-00027ce0: 2920 2d20 6d6f 6465 6c5f 6c6f 6772 6174  ) - model_lograt
-00027cf0: 650a 2020 2020 2020 2020 5d0a 0a20 2020  e.        ]..   
-00027d00: 2074 6963 6b73 2c20 6d61 7876 616c 203d   ticks, maxval =
-00027d10: 2067 7569 2e6d 696e 5f6d 6178 5f74 6963   gui.min_max_tic
-00027d20: 6b73 5f77 6974 685f 7a65 726f 2861 6c6c  ks_with_zero(all
-00027d30: 5f64 6174 612c 2035 290a 2020 2020 6178  _data, 5).    ax
-00027d40: 2e73 6574 5f79 7469 636b 7328 7469 636b  .set_yticks(tick
-00027d50: 7329 0a0a 2020 2020 6178 2e73 6574 5f79  s)..    ax.set_y
-00027d60: 6c69 6d28 5b2d 206d 6178 7661 6c20 2a20  lim([- maxval * 
-00027d70: 312e 312c 202b 206d 6178 7661 6c20 2a20  1.1, + maxval * 
-00027d80: 312e 315d 290a 0a20 2020 2023 2041 7869  1.1])..    # Axi
-00027d90: 7320 6c61 6265 6c73 0a20 2020 2061 782e  s labels.    ax.
-00027da0: 7365 745f 796c 6162 656c 280a 2020 2020  set_ylabel(.    
-00027db0: 2020 2020 7227 245c 6c6f 675f 5c6d 6174      r'$\log_\mat
-00027dc0: 6872 6567 756c 6172 7b31 307d 5b5c 7461  hregular{10}[\ta
-00027dd0: 755e 5c6d 6174 6872 6567 756c 6172 7b2d  u^\mathregular{-
-00027de0: 317d 5f7b 5c6d 6174 6872 6567 756c 6172  1}_{\mathregular
-00027df0: 7b65 7870 7d7d 5d24 202d 2024 5c6c 6f67  {exp}}]$ - $\log
-00027e00: 5f5c 6d61 7468 7265 6775 6c61 727b 3130  _\mathregular{10
-00027e10: 7d5b 5c74 6175 5e5c 6d61 7468 7265 6775  }[\tau^\mathregu
-00027e20: 6c61 727b 2d31 7d5f 7b5c 6d61 7468 7265  lar{-1}_{\mathre
-00027e30: 6775 6c61 727b 6669 747d 7d5d 2427 2023  gular{fit}}]$' #
-00027e40: 206e 6f71 610a 2020 2020 290a 0a20 2020   noqa.    )..   
-00027e50: 2023 2053 6574 2078 2074 6963 6b20 666f   # Set x tick fo
-00027e60: 726d 6174 7469 6e67 0a20 2020 2067 7569  rmatting.    gui
-00027e70: 2e73 6574 5f72 6174 655f 7874 6963 6b5f  .set_rate_xtick_
-00027e80: 666f 726d 6174 7469 6e67 2861 782c 2078  formatting(ax, x
-00027e90: 5f76 6172 7329 0a0a 2020 2020 7265 7475  _vars)..    retu
-00027ea0: 726e 0a0a 0a64 6566 2077 7269 7465 5f6d  rn...def write_m
-00027eb0: 6f64 656c 5f70 6172 616d 7328 6d6f 6465  odel_params(mode
-00027ec0: 6c3a 204c 6f67 5461 7554 4d6f 6465 6c20  l: LogTauTModel 
-00027ed0: 7c20 4d75 6c74 694c 6f67 5461 7554 4d6f  | MultiLogTauTMo
-00027ee0: 6465 6c20 7c20 4c6f 6754 6175 484d 6f64  del | LogTauHMod
-00027ef0: 656c 207c 204d 756c 7469 4c6f 6754 6175  el | MultiLogTau
-00027f00: 484d 6f64 656c 2c20 2320 6e6f 7161 0a20  HModel, # noqa. 
-00027f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027f20: 2020 2020 2020 6669 6c65 5f6e 616d 653a        file_name:
-00027f30: 2073 7472 2c20 7665 7262 6f73 653a 2062   str, verbose: b
-00027f40: 6f6f 6c20 3d20 5472 7565 2920 2d3e 204e  ool = True) -> N
-00027f50: 6f6e 653a 0a20 2020 2027 2727 0a20 2020  one:.    '''.   
-00027f60: 2057 7269 7465 7320 6669 7474 6564 2061   Writes fitted a
-00027f70: 6e64 2066 6978 6564 2070 6172 616d 6574  nd fixed paramet
-00027f80: 6572 7320 6f66 206d 6f64 656c 2873 2920  ers of model(s) 
-00027f90: 746f 2066 696c 650a 0a20 2020 2050 6172  to file..    Par
-00027fa0: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
-00027fb0: 2d2d 2d2d 2d2d 0a20 2020 206d 6f64 656c  ------.    model
-00027fc0: 733a 206c 6973 745b 4c6f 6754 6175 544d  s: list[LogTauTM
-00027fd0: 6f64 656c 207c 204d 756c 7469 4c6f 6754  odel | MultiLogT
-00027fe0: 6175 544d 6f64 656c 207c 204c 6f67 5461  auTModel | LogTa
-00027ff0: 7548 4d6f 6465 6c20 7c20 4d75 6c74 694c  uHModel | MultiL
-00028000: 6f67 5461 7548 4d6f 6465 6c5d 0a20 2020  ogTauHModel].   
-00028010: 2020 2020 204d 6f64 656c 732c 206f 6e65       Models, one
-00028020: 2070 6572 2074 656d 7065 7261 7475 7265   per temperature
-00028030: 0a20 2020 2066 696c 655f 6e61 6d65 3a20  .    file_name: 
-00028040: 7374 720a 2020 2020 2020 2020 4e61 6d65  str.        Name
-00028050: 206f 6620 6f75 7470 7574 2066 696c 650a   of output file.
-00028060: 2020 2020 7665 7262 6f73 653a 2062 6f6f      verbose: boo
-00028070: 6c2c 2064 6566 6175 6c74 2054 7275 650a  l, default True.
-00028080: 2020 2020 2020 2020 4966 2054 7275 652c          If True,
-00028090: 206f 7574 7075 7420 6669 6c65 206c 6f63   output file loc
-000280a0: 6174 696f 6e20 6973 2077 7269 7474 656e  ation is written
-000280b0: 2074 6f20 7465 726d 696e 616c 0a0a 2020   to terminal..  
-000280c0: 2020 5265 7475 726e 730a 2020 2020 2d2d    Returns.    --
-000280d0: 2d2d 2d2d 2d0a 2020 2020 4e6f 6e65 0a20  -----.    None. 
-000280e0: 2020 2027 2727 2023 206e 6f71 610a 0a20     ''' # noqa.. 
-000280f0: 2020 2069 6620 7479 7065 286d 6f64 656c     if type(model
-00028100: 2920 696e 205b 4d75 6c74 694c 6f67 5461  ) in [MultiLogTa
-00028110: 7554 4d6f 6465 6c2c 204d 756c 7469 4c6f  uTModel, MultiLo
-00028120: 6754 6175 484d 6f64 656c 5d3a 0a20 2020  gTauHModel]:.   
-00028130: 2020 2020 206c 6f67 6d6f 6465 6c73 203d       logmodels =
-00028140: 206d 6f64 656c 2e6c 6f67 6d6f 6465 6c73   model.logmodels
-00028150: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
-00028160: 2020 206c 6f67 6d6f 6465 6c73 203d 205b     logmodels = [
-00028170: 6d6f 6465 6c5d 0a0a 2020 2020 6620 3d20  model]..    f = 
-00028180: 6f70 656e 2866 696c 655f 6e61 6d65 2c20  open(file_name, 
-00028190: 2777 272c 2065 6e63 6f64 696e 673d 2775  'w', encoding='u
-000281a0: 7466 2d38 2729 0a0a 2020 2020 2320 5772  tf-8')..    # Wr
-000281b0: 6974 6520 6561 6368 2074 6572 6d27 7320  ite each term's 
-000281c0: 6e61 6d65 2c20 6669 7420 7661 7273 2c20  name, fit vars, 
-000281d0: 7374 6465 762c 2061 6e64 2066 6978 2076  stdev, and fix v
-000281e0: 6172 730a 2020 2020 666f 7220 6c6f 676d  ars.    for logm
-000281f0: 6f64 656c 2069 6e20 6c6f 676d 6f64 656c  odel in logmodel
-00028200: 733a 0a20 2020 2020 2020 2066 2e77 7269  s:.        f.wri
-00028210: 7465 2827 7b7d 5c6e 272e 666f 726d 6174  te('{}\n'.format
-00028220: 286c 6f67 6d6f 6465 6c2e 4e41 4d45 2929  (logmodel.NAME))
-00028230: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
-00028240: 6c6f 676d 6f64 656c 2e66 6974 5f76 6172  logmodel.fit_var
-00028250: 732e 6b65 7973 2829 293a 0a20 2020 2020  s.keys()):.     
-00028260: 2020 2020 2020 2066 2e77 7269 7465 2827         f.write('
-00028270: 4669 7474 6564 2054 6572 6d73 3a20 5661  Fitted Terms: Va
-00028280: 6c75 6520 616e 6420 5374 616e 6461 7264  lue and Standard
-00028290: 2044 6576 6961 7469 6f6e 3a5c 6e27 290a   Deviation:\n').
-000282a0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-000282b0: 6e61 6d65 2069 6e20 6c6f 676d 6f64 656c  name in logmodel
-000282c0: 2e66 6974 5f76 6172 732e 6b65 7973 2829  .fit_vars.keys()
-000282d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000282e0: 2020 662e 7772 6974 6528 277b 3a3e 367d    f.write('{:>6}
-000282f0: 207b 3a20 312e 3845 7d20 7b3a 2031 2e38   {: 1.8E} {: 1.8
-00028300: 457d 207b 7d5c 6e27 2e66 6f72 6d61 7428  E} {}\n'.format(
-00028310: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00028320: 2020 2020 206e 616d 652c 0a20 2020 2020       name,.     
-00028330: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00028340: 6f67 6d6f 6465 6c2e 6669 6e61 6c5f 7661  ogmodel.final_va
-00028350: 725f 7661 6c75 6573 5b6e 616d 655d 2c0a  r_values[name],.
-00028360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028370: 2020 2020 6c6f 676d 6f64 656c 2e66 6974      logmodel.fit
-00028380: 5f73 7464 6576 5b6e 616d 655d 2c0a 2020  _stdev[name],.  
-00028390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000283a0: 2020 6c6f 676d 6f64 656c 2e55 4e49 5453    logmodel.UNITS
-000283b0: 5b6e 616d 655d 0a20 2020 2020 2020 2020  [name].         
-000283c0: 2020 2020 2020 2029 290a 2020 2020 2020         )).      
-000283d0: 2020 6966 206c 656e 286c 6f67 6d6f 6465    if len(logmode
-000283e0: 6c2e 6669 785f 7661 7273 2e6b 6579 7328  l.fix_vars.keys(
-000283f0: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
-00028400: 662e 7772 6974 6528 2746 6978 6564 2054  f.write('Fixed T
-00028410: 6572 6d73 3a20 5661 6c75 6573 5c6e 2729  erms: Values\n')
-00028420: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00028430: 206e 616d 6520 696e 206c 6f67 6d6f 6465   name in logmode
-00028440: 6c2e 6669 785f 7661 7273 2e6b 6579 7328  l.fix_vars.keys(
-00028450: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00028460: 2020 2066 2e77 7269 7465 2827 7b3a 3e36     f.write('{:>6
-00028470: 7d20 7b3a 2031 2e38 457d 207b 7d5c 6e27  } {: 1.8E} {}\n'
-00028480: 2e66 6f72 6d61 7428 0a20 2020 2020 2020  .format(.       
-00028490: 2020 2020 2020 2020 2020 2020 206e 616d               nam
-000284a0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-000284b0: 2020 2020 2020 206c 6f67 6d6f 6465 6c2e         logmodel.
-000284c0: 6669 6e61 6c5f 7661 725f 7661 6c75 6573  final_var_values
-000284d0: 5b6e 616d 655d 2c0a 2020 2020 2020 2020  [name],.        
-000284e0: 2020 2020 2020 2020 2020 2020 6c6f 676d              logm
-000284f0: 6f64 656c 2e55 4e49 5453 5b6e 616d 655d  odel.UNITS[name]
-00028500: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00028510: 2029 290a 2020 2020 2020 2020 662e 7772   )).        f.wr
-00028520: 6974 6528 275c 6e27 290a 0a20 2020 2069  ite('\n')..    i
-00028530: 6620 7665 7262 6f73 653a 0a20 2020 2020  f verbose:.     
-00028540: 2020 2075 742e 6370 7269 6e74 280a 2020     ut.cprint(.  
-00028550: 2020 2020 2020 2020 2020 275c 6e20 5265            '\n Re
-00028560: 6c61 7861 7469 6f6e 204d 6f64 656c 2070  laxation Model p
-00028570: 6172 616d 6574 6572 7320 7772 6974 7465  arameters writte
-00028580: 6e20 746f 205c 6e20 7b7d 5c6e 272e 666f  n to \n {}\n'.fo
-00028590: 726d 6174 280a 2020 2020 2020 2020 2020  rmat(.          
-000285a0: 2020 2020 2020 6669 6c65 5f6e 616d 650a        file_name.
-000285b0: 2020 2020 2020 2020 2020 2020 292c 0a20              ),. 
-000285c0: 2020 2020 2020 2020 2020 2027 6379 616e             'cyan
-000285d0: 270a 2020 2020 2020 2020 290a 0a20 2020  '.        )..   
-000285e0: 2072 6574 7572 6e0a 0a0a 6465 6620 7772   return...def wr
-000285f0: 6974 655f 6d6f 6465 6c5f 6461 7461 2864  ite_model_data(d
-00028600: 6174 6173 6574 3a20 5461 7554 4461 7461  ataset: TauTData
-00028610: 7365 7420 7c20 5461 7548 4461 7461 7365  set | TauHDatase
-00028620: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
-00028630: 2020 2020 2020 2020 6d6f 6465 6c3a 204c          model: L
-00028640: 6f67 5461 7554 4d6f 6465 6c20 7c20 4d75  ogTauTModel | Mu
-00028650: 6c74 694c 6f67 5461 7554 4d6f 6465 6c20  ltiLogTauTModel 
-00028660: 7c20 4c6f 6754 6175 484d 6f64 656c 207c  | LogTauHModel |
-00028670: 204d 756c 7469 4c6f 6754 6175 484d 6f64   MultiLogTauHMod
-00028680: 656c 2c20 2320 6e6f 7161 0a20 2020 2020  el, # noqa.     
-00028690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000286a0: 6669 6c65 5f6e 616d 653a 2073 7472 2c20  file_name: str, 
-000286b0: 7665 7262 6f73 653a 2062 6f6f 6c20 3d20  verbose: bool = 
-000286c0: 5472 7565 2920 2d3e 204e 6f6e 653a 0a20  True) -> None:. 
-000286d0: 2020 2027 2727 0a20 2020 2043 7265 6174     '''.    Creat
-000286e0: 6573 2066 696c 6520 636f 6e74 6169 6e69  es file containi
-000286f0: 6e67 2072 6174 6520 7673 2074 656d 7065  ng rate vs tempe
-00028700: 7261 7475 7265 2f66 6965 6c64 2063 616c  rature/field cal
-00028710: 6375 6c61 7465 6420 7573 696e 6720 6d6f  culated using mo
-00028720: 6465 6c0a 2020 2020 7061 7261 6d65 7465  del.    paramete
-00028730: 7273 0a0a 2020 2020 5061 7261 6d65 7465  rs..    Paramete
-00028740: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
-00028750: 2d0a 2020 2020 6461 7461 7365 743a 2054  -.    dataset: T
-00028760: 6175 5444 6174 6173 6574 207c 2054 6175  auTDataset | Tau
-00028770: 4844 6174 6173 6574 0a20 2020 2020 2020  HDataset.       
-00028780: 2044 6174 6173 6574 2074 6f20 7768 6963   Dataset to whic
-00028790: 6820 6120 6d6f 6465 6c20 7761 7320 7375  h a model was su
-000287a0: 6363 6573 7366 756c 6c79 2066 6974 7465  ccessfully fitte
-000287b0: 6420 2869 2e65 2e20 6669 745f 7374 6174  d (i.e. fit_stat
-000287c0: 7573 3d54 7275 6529 0a20 2020 206d 6f64  us=True).    mod
-000287d0: 656c 3a20 4c6f 6754 6175 544d 6f64 656c  el: LogTauTModel
-000287e0: 207c 204d 756c 7469 4c6f 6754 6175 544d   | MultiLogTauTM
-000287f0: 6f64 656c 207c 204c 6f67 5461 7548 4d6f  odel | LogTauHMo
-00028800: 6465 6c20 7c20 4d75 6c74 694c 6f67 5461  del | MultiLogTa
-00028810: 7548 4d6f 6465 6c0a 2020 2020 2020 2020  uHModel.        
-00028820: 4d6f 6465 6c20 7768 6963 6820 6861 7320  Model which has 
-00028830: 6265 656e 2066 6974 7465 6420 746f 2064  been fitted to d
-00028840: 6174 6173 6574 0a20 2020 2066 696c 655f  ataset.    file_
-00028850: 6e61 6d65 3a20 7374 720a 2020 2020 2020  name: str.      
-00028860: 2020 4e61 6d65 206f 6620 6f75 7470 7574    Name of output
-00028870: 2066 696c 650a 2020 2020 7665 7262 6f73   file.    verbos
-00028880: 653a 2062 6f6f 6c2c 2064 6566 6175 6c74  e: bool, default
-00028890: 2054 7275 650a 2020 2020 2020 2020 4966   True.        If
-000288a0: 2054 7275 652c 206f 7574 7075 7420 6669   True, output fi
-000288b0: 6c65 206c 6f63 6174 696f 6e20 6973 2077  le location is w
-000288c0: 7269 7474 656e 2074 6f20 7465 726d 696e  ritten to termin
-000288d0: 616c 0a0a 2020 2020 5265 7475 726e 730a  al..    Returns.
-000288e0: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-000288f0: 4e6f 6e65 0a20 2020 2027 2727 0a0a 2020  None.    '''..  
-00028900: 2020 6966 206e 6f74 206d 6f64 656c 2e66    if not model.f
-00028910: 6974 5f73 7461 7475 733a 0a20 2020 2020  it_status:.     
-00028920: 2020 2072 6574 7572 6e0a 0a20 2020 2069     return..    i
-00028930: 6620 6973 696e 7374 616e 6365 2864 6174  f isinstance(dat
-00028940: 6173 6574 2c20 5461 7548 4461 7461 7365  aset, TauHDatase
-00028950: 7429 3a0a 2020 2020 2020 2020 785f 7661  t):.        x_va
-00028960: 7273 203d 2064 6174 6173 6574 2e66 6965  rs = dataset.fie
-00028970: 6c64 730a 2020 2020 2020 2020 785f 7661  lds.        x_va
-00028980: 725f 6c61 6265 6c20 3d20 2748 2028 4f65  r_label = 'H (Oe
-00028990: 2927 0a0a 2020 2020 656c 6966 2069 7369  )'..    elif isi
-000289a0: 6e73 7461 6e63 6528 6461 7461 7365 742c  nstance(dataset,
-000289b0: 2054 6175 5444 6174 6173 6574 293a 0a20   TauTDataset):. 
-000289c0: 2020 2020 2020 2078 5f76 6172 7320 3d20         x_vars = 
-000289d0: 6461 7461 7365 742e 7465 6d70 6572 6174  dataset.temperat
-000289e0: 7572 6573 0a20 2020 2020 2020 2078 5f76  ures.        x_v
-000289f0: 6172 5f6c 6162 656c 203d 2027 5420 284b  ar_label = 'T (K
-00028a00: 2927 0a0a 2020 2020 6966 2074 7970 6528  )'..    if type(
-00028a10: 6d6f 6465 6c29 2069 6e20 5b4d 756c 7469  model) in [Multi
-00028a20: 4c6f 6754 6175 544d 6f64 656c 2c20 4d75  LogTauTModel, Mu
-00028a30: 6c74 694c 6f67 5461 7548 4d6f 6465 6c5d  ltiLogTauHModel]
-00028a40: 3a0a 2020 2020 2020 2020 6c6f 676d 6f64  :.        logmod
-00028a50: 656c 7320 3d20 6d6f 6465 6c2e 6c6f 676d  els = model.logm
-00028a60: 6f64 656c 730a 2020 2020 656c 7365 3a0a  odels.    else:.
-00028a70: 2020 2020 2020 2020 6c6f 676d 6f64 656c          logmodel
-00028a80: 7320 3d20 5b6d 6f64 656c 5d0a 0a20 2020  s = [model]..   
-00028a90: 2066 203d 206f 7065 6e28 6669 6c65 5f6e   f = open(file_n
-00028aa0: 616d 652c 2027 7727 2c20 656e 636f 6469  ame, 'w', encodi
-00028ab0: 6e67 3d27 7574 662d 3827 290a 0a20 2020  ng='utf-8')..   
-00028ac0: 2078 5f76 6172 735f 6772 6964 203d 206e   x_vars_grid = n
-00028ad0: 702e 6c6f 6773 7061 6365 280a 2020 2020  p.logspace(.    
-00028ae0: 2020 2020 6e70 2e6c 6f67 3130 286e 702e      np.log10(np.
-00028af0: 6d69 6e28 785f 7661 7273 2929 2c0a 2020  min(x_vars)),.  
-00028b00: 2020 2020 2020 6e70 2e6c 6f67 3130 286e        np.log10(n
-00028b10: 702e 6d61 7828 785f 7661 7273 2929 2c0a  p.max(x_vars)),.
-00028b20: 2020 2020 2020 2020 3130 300a 2020 2020          100.    
-00028b30: 290a 0a20 2020 2066 2e77 7269 7465 2827  )..    f.write('
-00028b40: 7b3a 3e39 7d20 272e 666f 726d 6174 2878  {:>9} '.format(x
-00028b50: 5f76 6172 5f6c 6162 656c 2929 0a20 2020  _var_label)).   
-00028b60: 2066 6f72 206c 6f67 6d6f 6465 6c20 696e   for logmodel in
-00028b70: 206c 6f67 6d6f 6465 6c73 3a0a 2020 2020   logmodels:.    
-00028b80: 2020 2020 662e 7772 6974 6528 277b 3a3e      f.write('{:>
-00028b90: 377d 2072 6174 6520 272e 666f 726d 6174  7} rate '.format
-00028ba0: 286c 6f67 6d6f 6465 6c2e 4e41 4d45 2929  (logmodel.NAME))
-00028bb0: 0a20 2020 2069 6620 6c65 6e28 6c6f 676d  .    if len(logm
-00028bc0: 6f64 656c 7329 203e 2031 3a0a 2020 2020  odels) > 1:.    
-00028bd0: 2020 2020 662e 7772 6974 6528 2720 2054      f.write('  T
-00028be0: 6f74 616c 2072 6174 6520 2873 5e2d 3129  otal rate (s^-1)
-00028bf0: 2729 0a20 2020 2066 2e77 7269 7465 2827  ').    f.write('
-00028c00: 5c6e 2729 0a0a 2020 2020 666f 7220 6772  \n')..    for gr
-00028c10: 6964 5f70 7420 696e 2078 5f76 6172 735f  id_pt in x_vars_
-00028c20: 6772 6964 3a0a 2020 2020 2020 2020 662e  grid:.        f.
-00028c30: 7772 6974 6528 277b 3a20 392e 3566 7d20  write('{: 9.5f} 
-00028c40: 272e 666f 726d 6174 2867 7269 645f 7074  '.format(grid_pt
-00028c50: 2929 0a20 2020 2020 2020 2074 6f74 616c  )).        total
-00028c60: 203d 2030 2e0a 2020 2020 2020 2020 666f   = 0..        fo
-00028c70: 7220 6c6f 676d 6f64 656c 2069 6e20 6c6f  r logmodel in lo
-00028c80: 676d 6f64 656c 733a 0a20 2020 2020 2020  gmodels:.       
-00028c90: 2020 2020 2072 6174 6520 3d20 3130 2a2a       rate = 10**
-00028ca0: 6c6f 676d 6f64 656c 2e6d 6f64 656c 280a  logmodel.model(.
-00028cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028cc0: 6c6f 676d 6f64 656c 2e66 696e 616c 5f76  logmodel.final_v
-00028cd0: 6172 5f76 616c 7565 732c 0a20 2020 2020  ar_values,.     
-00028ce0: 2020 2020 2020 2020 2020 205b 6772 6964             [grid
-00028cf0: 5f70 745d 0a20 2020 2020 2020 2020 2020  _pt].           
-00028d00: 2029 5b30 5d0a 2020 2020 2020 2020 2020   )[0].          
-00028d10: 2020 662e 7772 6974 6528 277b 3a2e 3645    f.write('{:.6E
-00028d20: 7d20 272e 666f 726d 6174 2872 6174 6529  } '.format(rate)
-00028d30: 290a 2020 2020 2020 2020 2020 2020 746f  ).            to
-00028d40: 7461 6c20 2b3d 2072 6174 650a 2020 2020  tal += rate.    
-00028d50: 2020 2020 6966 206c 656e 286c 6f67 6d6f      if len(logmo
-00028d60: 6465 6c73 2920 3e20 313a 0a20 2020 2020  dels) > 1:.     
-00028d70: 2020 2020 2020 2066 2e77 7269 7465 2827         f.write('
-00028d80: 7b3a 2e36 457d 272e 666f 726d 6174 2874  {:.6E}'.format(t
-00028d90: 6f74 616c 2929 0a20 2020 2020 2020 2066  otal)).        f
-00028da0: 2e77 7269 7465 2827 5c6e 2729 0a0a 2020  .write('\n')..  
-00028db0: 2020 6966 2076 6572 626f 7365 3a0a 2020    if verbose:.  
-00028dc0: 2020 2020 2020 7574 2e63 7072 696e 7428        ut.cprint(
-00028dd0: 0a20 2020 2020 2020 2020 2020 2027 5c6e  .            '\n
-00028de0: 2052 656c 6178 6174 696f 6e20 6d6f 6465   Relaxation mode
-00028df0: 6c20 cf84 e281 bbc2 b920 7673 207b 7d20  l ....... vs {} 
-00028e00: 7772 6974 7465 6e20 746f 205c 6e20 7b7d  written to \n {}
-00028e10: 5c6e 272e 666f 726d 6174 280a 2020 2020  \n'.format(.    
-00028e20: 2020 2020 2020 2020 2020 2020 785f 7661              x_va
-00028e30: 725f 6c61 6265 6c5b 305d 2c0a 2020 2020  r_label[0],.    
-00028e40: 2020 2020 2020 2020 2020 2020 6669 6c65              file
-00028e50: 5f6e 616d 650a 2020 2020 2020 2020 2020  _name.          
-00028e60: 2020 292c 0a20 2020 2020 2020 2020 2020    ),.           
-00028e70: 2027 6379 616e 270a 2020 2020 2020 2020   'cyan'.        
-00028e80: 290a 0a20 2020 2072 6574 7572 6e0a       )..    return.
+000186d0: 2020 2020 2020 2020 6d61 726b 6564 5b69          marked[i
+000186e0: 745d 203d 2054 7275 650a 0a20 2020 2020  t] = True..     
+000186f0: 2020 2072 6574 7572 6e20 696e 7374 616e     return instan
+00018700: 7469 6174 6564 5f6d 6f64 656c 730a 0a20  tiated_models.. 
+00018710: 2020 2040 636c 6173 736d 6574 686f 640a     @classmethod.
+00018720: 2020 2020 6465 6620 7265 7369 6475 616c      def residual
+00018730: 5f66 726f 6d5f 666c 6f61 745f 6c69 7374  _from_float_list
+00018740: 2863 6c73 2c20 6e65 775f 7661 6c73 3a20  (cls, new_vals: 
+00018750: 6e70 742e 4172 7261 794c 696b 652c 0a20  npt.ArrayLike,. 
+00018760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018780: 6c6f 676d 6f64 656c 733a 206c 6973 745b  logmodels: list[
+00018790: 4c6f 6754 6175 544d 6f64 656c 5d2c 0a20  LogTauTModel],. 
+000187a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000187b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000187c0: 7465 6d70 6572 6174 7572 6573 3a20 6e70  temperatures: np
+000187d0: 742e 4172 7261 794c 696b 652c 0a20 2020  t.ArrayLike,.   
+000187e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000187f0: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+00018800: 6772 6174 653a 206e 7074 2e41 7272 6179  grate: npt.Array
+00018810: 4c69 6b65 2c0a 2020 2020 2020 2020 2020  Like,.          
+00018820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018830: 2020 2020 2020 2073 6967 6d61 3a20 6e70         sigma: np
+00018840: 742e 4172 7261 794c 696b 6520 3d20 5b5d  t.ArrayLike = []
+00018850: 2920 2d3e 206e 7074 2e4e 4441 7272 6179  ) -> npt.NDArray
+00018860: 3a0a 2020 2020 2020 2020 2727 270a 2020  :.        '''.  
+00018870: 2020 2020 2020 5772 6170 7065 7220 666f        Wrapper fo
+00018880: 7220 6072 6573 6964 7561 6c73 6020 6d65  r `residuals` me
+00018890: 7468 6f64 2c20 7461 6b65 7320 6e65 7720  thod, takes new 
+000188a0: 7661 6c75 6573 2066 726f 6d20 6669 7474  values from fitt
+000188b0: 696e 6720 726f 7574 696e 650a 2020 2020  ing routine.    
+000188c0: 2020 2020 7768 6963 6820 7072 6f76 6964      which provid
+000188d0: 6573 206c 6973 745b 666c 6f61 745d 2c20  es list[float], 
+000188e0: 746f 2063 6f6e 7374 7275 6374 206e 6577  to construct new
+000188f0: 2066 6974 5f76 6172 7320 6469 6374 2c20   fit_vars dict, 
+00018900: 7468 656e 0a20 2020 2020 2020 2072 756e  then.        run
+00018910: 7320 6072 6573 6964 7561 6c73 6020 6d65  s `residuals` me
+00018920: 7468 6f64 2e0a 0a20 2020 2020 2020 2050  thod...        P
+00018930: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
+00018940: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+00018950: 2020 2020 206e 6577 5f76 616c 733a 2061       new_vals: a
+00018960: 7272 6179 5f6c 696b 650a 2020 2020 2020  rray_like.      
+00018970: 2020 2020 2020 5468 6973 2069 7465 7261        This itera
+00018980: 7469 6f6e 2773 2066 6974 2070 6172 616d  tion's fit param
+00018990: 6574 6572 2076 616c 7565 7320 7072 6f76  eter values prov
+000189a0: 6964 6564 2062 7920 6c65 6173 745f 7371  ided by least_sq
+000189b0: 7561 7265 730a 2020 2020 2020 2020 2020  uares.          
+000189c0: 2020 7468 6973 2068 6173 2074 6865 2073    this has the s
+000189d0: 616d 6520 6f72 6465 7220 6174 2066 6974  ame order at fit
+000189e0: 5f76 6172 732e 6b65 7973 0a20 2020 2020  _vars.keys.     
+000189f0: 2020 206c 6f67 6d6f 6465 6c73 3a20 6c69     logmodels: li
+00018a00: 7374 5b4c 6f67 5461 7554 4d6f 6465 6c5d  st[LogTauTModel]
+00018a10: 0a20 2020 2020 2020 2020 2020 204d 6f64  .            Mod
+00018a20: 656c 7320 746f 2075 7365 0a20 2020 2020  els to use.     
+00018a30: 2020 2074 656d 7065 7261 7475 7265 733a     temperatures:
+00018a40: 2061 7272 6179 5f6c 696b 650a 2020 2020   array_like.    
+00018a50: 2020 2020 2020 2020 5465 6d70 6572 6174          Temperat
+00018a60: 7572 6520 7661 6c75 6573 2028 4b29 2061  ure values (K) a
+00018a70: 7420 7768 6963 6820 6d6f 6465 6c20 6675  t which model fu
+00018a80: 6e63 7469 6f6e 2069 7320 6576 616c 7561  nction is evalua
+00018a90: 7465 640a 2020 2020 2020 2020 6c6f 6772  ted.        logr
+00018aa0: 6174 653a 2061 7272 6179 5f6c 696b 650a  ate: array_like.
+00018ab0: 2020 2020 2020 2020 2020 2020 5472 7565              True
+00018ac0: 2028 6578 7065 7269 6d65 6e74 616c 2920   (experimental) 
+00018ad0: 7661 6c75 6573 206f 6620 6c6f 6731 3028  values of log10(
+00018ae0: 7265 6c61 7861 7469 6f6e 2072 6174 6529  relaxation rate)
+00018af0: 0a20 2020 2020 2020 2073 6967 6d61 3a20  .        sigma: 
+00018b00: 6172 7261 795f 6c69 6b65 0a20 2020 2020  array_like.     
+00018b10: 2020 2020 2020 2053 7461 6e64 6172 6420         Standard 
+00018b20: 6465 7669 6174 696f 6e20 6f66 2074 6175  deviation of tau
+00018b30: 2069 6e20 6c6f 6773 7061 6365 0a0a 2020   in logspace..  
+00018b40: 2020 2020 2020 5265 7475 726e 730a 2020        Returns.  
+00018b50: 2020 2020 2020 2d2d 2d2d 2d2d 2d0a 2020        -------.  
+00018b60: 2020 2020 2020 6e64 6172 7261 7920 6f66        ndarray of
+00018b70: 2066 6c6f 6174 730a 2020 2020 2020 2020   floats.        
+00018b80: 2020 2020 5265 7369 6475 616c 730a 2020      Residuals.  
+00018b90: 2020 2020 2020 2727 270a 0a20 2020 2020        '''..     
+00018ba0: 2020 2023 2053 7761 7020 6669 7420 7661     # Swap fit va
+00018bb0: 6c75 6573 2066 6f72 206e 6577 2076 616c  lues for new val
+00018bc0: 7565 7320 6672 6f6d 2066 6974 2072 6f75  ues from fit rou
+00018bd0: 7469 6e65 0a20 2020 2020 2020 206e 6577  tine.        new
+00018be0: 5f66 6974 5f76 6172 7320 3d20 5b5d 0a0a  _fit_vars = []..
+00018bf0: 2020 2020 2020 2020 6974 203d 2030 0a20          it = 0. 
+00018c00: 2020 2020 2020 2066 6f72 206c 6f67 6d6f         for logmo
+00018c10: 6465 6c20 696e 206c 6f67 6d6f 6465 6c73  del in logmodels
+00018c20: 3a0a 2020 2020 2020 2020 2020 2020 6e65  :.            ne
+00018c30: 775f 6469 6374 203d 207b 7d0a 2020 2020  w_dict = {}.    
+00018c40: 2020 2020 2020 2020 666f 7220 6e61 6d65          for name
+00018c50: 2069 6e20 6c6f 676d 6f64 656c 2e66 6974   in logmodel.fit
+00018c60: 5f76 6172 732e 6b65 7973 2829 3a0a 2020  _vars.keys():.  
+00018c70: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
+00018c80: 775f 6469 6374 5b6e 616d 655d 203d 206e  w_dict[name] = n
+00018c90: 6577 5f76 616c 735b 6974 5d0a 2020 2020  ew_vals[it].    
+00018ca0: 2020 2020 2020 2020 2020 2020 6974 202b              it +
+00018cb0: 3d20 310a 2020 2020 2020 2020 2020 2020  = 1.            
+00018cc0: 6e65 775f 6669 745f 7661 7273 2e61 7070  new_fit_vars.app
+00018cd0: 656e 6428 6e65 775f 6469 6374 290a 0a20  end(new_dict).. 
+00018ce0: 2020 2020 2020 2072 6573 6964 7561 6c73         residuals
+00018cf0: 203d 2063 6c73 2e72 6573 6964 7561 6c73   = cls.residuals
+00018d00: 280a 2020 2020 2020 2020 2020 2020 6c6f  (.            lo
+00018d10: 676d 6f64 656c 732c 206e 6577 5f66 6974  gmodels, new_fit
+00018d20: 5f76 6172 732c 2074 656d 7065 7261 7475  _vars, temperatu
+00018d30: 7265 732c 206c 6f67 7261 7465 0a20 2020  res, lograte.   
+00018d40: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+00018d50: 6966 206c 656e 2873 6967 6d61 293a 0a20  if len(sigma):. 
+00018d60: 2020 2020 2020 2020 2020 2072 6573 6964             resid
+00018d70: 7561 6c73 202f 3d20 7369 676d 610a 0a20  uals /= sigma.. 
+00018d80: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+00018d90: 7369 6475 616c 730a 0a20 2020 2040 7374  siduals..    @st
+00018da0: 6174 6963 6d65 7468 6f64 0a20 2020 2064  aticmethod.    d
+00018db0: 6566 2072 6573 6964 7561 6c73 286c 6f67  ef residuals(log
+00018dc0: 6d6f 6465 6c73 3a20 6c69 7374 5b4c 6f67  models: list[Log
+00018dd0: 5461 7554 4d6f 6465 6c5d 2c0a 2020 2020  TauTModel],.    
+00018de0: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
+00018df0: 775f 6669 745f 7661 7273 3a20 6c69 7374  w_fit_vars: list
+00018e00: 5b64 6963 745b 7374 722c 2066 6c6f 6174  [dict[str, float
+00018e10: 5d5d 2c0a 2020 2020 2020 2020 2020 2020  ]],.            
+00018e20: 2020 2020 2020 7465 6d70 6572 6174 7572        temperatur
+00018e30: 6573 3a20 6e70 742e 4172 7261 794c 696b  es: npt.ArrayLik
+00018e40: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00018e50: 2020 2020 2074 7275 655f 6c6f 6772 6174       true_lograt
+00018e60: 653a 206e 7074 2e41 7272 6179 4c69 6b65  e: npt.ArrayLike
+00018e70: 2920 2d3e 206e 7074 2e4e 4441 7272 6179  ) -> npt.NDArray
+00018e80: 3a0a 2020 2020 2020 2020 2727 270a 2020  :.        '''.  
+00018e90: 2020 2020 2020 4361 6c63 756c 6174 6573        Calculates
+00018ea0: 2064 6966 6665 7265 6e63 6520 6265 7477   difference betw
+00018eb0: 6565 6e20 6578 7065 7269 6d65 6e74 616c  een experimental
+00018ec0: 206c 6f67 3130 2874 6175 5e2d 3129 0a20   log10(tau^-1). 
+00018ed0: 2020 2020 2020 2061 6e64 206c 6f67 3130         and log10
+00018ee0: 2874 6175 5e2d 3129 206f 6274 6169 6e65  (tau^-1) obtaine
+00018ef0: 6420 6672 6f6d 2074 6865 2073 756d 206f  d from the sum o
+00018f00: 6620 7468 6520 7072 6f76 6964 6564 206c  f the provided l
+00018f10: 6f67 6d6f 6465 6c73 0a20 2020 2020 2020  ogmodels.       
+00018f20: 2075 7369 6e67 2074 6865 2070 726f 7669   using the provi
+00018f30: 6465 6420 6669 7420 7661 7269 6162 6c65  ded fit variable
+00018f40: 2076 616c 7565 7320 6174 2070 726f 7669   values at provi
+00018f50: 6465 6420 7465 6d70 6572 6174 7572 6573  ded temperatures
+00018f60: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
+00018f70: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
+00018f80: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+00018f90: 6c6f 676d 6f64 656c 733a 206c 6973 745b  logmodels: list[
+00018fa0: 4c6f 6754 6175 544d 6f64 656c 5d0a 2020  LogTauTModel].  
+00018fb0: 2020 2020 2020 2020 2020 4c6f 6754 6175            LogTau
+00018fc0: 544d 6f64 656c 7320 7768 6963 6820 7769  TModels which wi
+00018fd0: 6c6c 2062 6520 6576 616c 7561 7465 640a  ll be evaluated.
+00018fe0: 2020 2020 2020 2020 6e65 775f 6669 745f          new_fit_
+00018ff0: 7661 7273 3a20 6c69 7374 5b64 6963 745b  vars: list[dict[
+00019000: 7374 722c 2066 6c6f 6174 5d5d 0a20 2020  str, float]].   
+00019010: 2020 2020 2020 2020 2066 6974 2064 6963           fit dic
+00019020: 7473 2066 6f72 2065 6163 6820 4c6f 6754  ts for each LogT
+00019030: 6175 544d 6f64 656c 2c20 6d75 7374 2068  auTModel, must h
+00019040: 6176 6520 7361 6d65 206f 7264 6572 2061  ave same order a
+00019050: 7320 6c6f 676d 6f64 656c 0a20 2020 2020  s logmodel.     
+00019060: 2020 2020 2020 2069 6620 6e6f 2076 6172         if no var
+00019070: 7320 746f 2066 6974 2066 6f72 2074 6861  s to fit for tha
+00019080: 7420 6d6f 6465 6c2c 2074 6865 6e20 656d  t model, then em
+00019090: 7074 7920 6469 6374 2069 7320 6769 7665  pty dict is give
+000190a0: 6e0a 2020 2020 2020 2020 7465 6d70 6572  n.        temper
+000190b0: 6174 7572 6573 3a20 6172 7261 795f 6c69  atures: array_li
+000190c0: 6b65 0a20 2020 2020 2020 2020 2020 2045  ke.            E
+000190d0: 7870 6572 696d 656e 7461 6c20 7465 6d70  xperimental temp
+000190e0: 6572 6174 7572 6573 2028 4b29 0a20 2020  eratures (K).   
+000190f0: 2020 2020 2074 7275 655f 6c6f 6772 6174       true_lograt
+00019100: 653a 2061 7272 6179 5f6c 696b 650a 2020  e: array_like.  
+00019110: 2020 2020 2020 2020 2020 4578 7065 7269            Experi
+00019120: 6d65 6e74 616c 204c 6f67 3130 2872 6174  mental Log10(rat
+00019130: 6529 730a 0a20 2020 2020 2020 2052 6574  e)s..        Ret
+00019140: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
+00019150: 2d2d 2d2d 0a20 2020 2020 2020 206e 6461  ----.        nda
+00019160: 7272 6179 206f 6620 666c 6f61 7473 0a20  rray of floats. 
+00019170: 2020 2020 2020 2020 2020 204c 6f67 3130             Log10
+00019180: 2872 6174 6529 5f74 7269 616c 202d 204c  (rate)_trial - L
+00019190: 6f67 3130 2872 6174 6529 5f65 7870 2066  og10(rate)_exp f
+000191a0: 6f72 2065 6163 6820 7465 6d70 6572 6174  or each temperat
+000191b0: 7572 650a 2020 2020 2020 2020 2727 270a  ure.        '''.
+000191c0: 0a20 2020 2020 2020 2023 2043 616c 6375  .        # Calcu
+000191d0: 6c61 7465 206d 6f64 656c 206c 6f67 3130  late model log10
+000191e0: 2872 656c 6178 6174 696f 6e20 7261 7465  (relaxation rate
+000191f0: 2920 7573 696e 6720 7061 7261 6d65 7465  ) using paramete
+00019200: 7273 0a20 2020 2020 2020 2023 2061 7320  rs.        # as 
+00019210: 7375 6d20 6f66 2063 6f6e 7472 6962 7574  sum of contribut
+00019220: 696f 6e73 2066 726f 6d20 6561 6368 2070  ions from each p
+00019230: 726f 6365 7373 0a20 2020 2020 2020 2074  rocess.        t
+00019240: 7269 616c 5f6c 6f67 7261 7465 203d 206e  rial_lograte = n
+00019250: 702e 7a65 726f 7328 6c65 6e28 7465 6d70  p.zeros(len(temp
+00019260: 6572 6174 7572 6573 2929 0a0a 2020 2020  eratures))..    
+00019270: 2020 2020 666f 7220 6c6f 676d 6f64 656c      for logmodel
+00019280: 2c20 6669 745f 7661 7273 2069 6e20 7a69  , fit_vars in zi
+00019290: 7028 6c6f 676d 6f64 656c 732c 206e 6577  p(logmodels, new
+000192a0: 5f66 6974 5f76 6172 7329 3a0a 2020 2020  _fit_vars):.    
+000192b0: 2020 2020 2020 2020 616c 6c5f 7661 7273          all_vars
+000192c0: 203d 207b 2a2a 6c6f 676d 6f64 656c 2e66   = {**logmodel.f
+000192d0: 6978 5f76 6172 732c 202a 2a66 6974 5f76  ix_vars, **fit_v
+000192e0: 6172 737d 0a20 2020 2020 2020 2020 2020  ars}.           
+000192f0: 2074 7269 616c 5f6c 6f67 7261 7465 202b   trial_lograte +
+00019300: 3d20 3130 2a2a 6c6f 676d 6f64 656c 2e6d  = 10**logmodel.m
+00019310: 6f64 656c 2861 6c6c 5f76 6172 732c 2074  odel(all_vars, t
+00019320: 656d 7065 7261 7475 7265 7329 0a0a 2020  emperatures)..  
+00019330: 2020 2020 2020 2320 7375 6d20 696e 206c        # sum in l
+00019340: 696e 6561 7220 7370 6163 652c 2074 6865  inear space, the
+00019350: 6e20 7461 6b65 206c 6f67 0a20 2020 2020  n take log.     
+00019360: 2020 2074 7269 616c 5f6c 6f67 7261 7465     trial_lograte
+00019370: 203d 206e 702e 6c6f 6731 3028 7472 6961   = np.log10(tria
+00019380: 6c5f 6c6f 6772 6174 6529 0a0a 2020 2020  l_lograte)..    
+00019390: 2020 2020 7265 7369 6475 616c 7320 3d20      residuals = 
+000193a0: 7472 6961 6c5f 6c6f 6772 6174 6520 2d20  trial_lograte - 
+000193b0: 7472 7565 5f6c 6f67 7261 7465 0a0a 2020  true_lograte..  
+000193c0: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+000193d0: 6964 7561 6c73 0a0a 2020 2020 6465 6620  iduals..    def 
+000193e0: 6669 745f 746f 2873 656c 662c 2064 6174  fit_to(self, dat
+000193f0: 6173 6574 3a20 5461 7554 4461 7461 7365  aset: TauTDatase
+00019400: 742c 2076 6572 626f 7365 3a20 626f 6f6c  t, verbose: bool
+00019410: 203d 2054 7275 6529 202d 3e20 4e6f 6e65   = True) -> None
+00019420: 3a0a 2020 2020 2020 2020 2727 270a 2020  :.        '''.  
+00019430: 2020 2020 2020 4669 7473 206d 6f64 656c        Fits model
+00019440: 2074 6f20 4461 7461 7365 740a 0a20 2020   to Dataset..   
+00019450: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
+00019460: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+00019470: 2d2d 0a20 2020 2020 2020 2064 6174 6173  --.        datas
+00019480: 6574 3a20 5461 7554 4461 7461 7365 740a  et: TauTDataset.
+00019490: 2020 2020 2020 2020 2020 2020 4461 7461              Data
+000194a0: 7365 7420 746f 2077 6869 6368 2061 206d  set to which a m
+000194b0: 6f64 656c 206f 6620 7261 7465 2076 7320  odel of rate vs 
+000194c0: 7465 6d70 6572 6174 7572 6520 7769 6c6c  temperature will
+000194d0: 2062 6520 6669 7474 6564 0a20 2020 2020   be fitted.     
+000194e0: 2020 2076 6572 626f 7365 3a20 626f 6f6c     verbose: bool
+000194f0: 2c20 6465 6661 756c 7420 5472 7565 0a20  , default True. 
+00019500: 2020 2020 2020 2020 2020 2049 6620 5472             If Tr
+00019510: 7565 2c20 7072 696e 7473 2069 6e66 6f72  ue, prints infor
+00019520: 6d61 7469 6f6e 2074 6f20 7465 726d 696e  mation to termin
+00019530: 616c 0a0a 2020 2020 2020 2020 5265 7475  al..        Retu
+00019540: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
+00019550: 2d2d 2d0a 2020 2020 2020 2020 4e6f 6e65  ---.        None
+00019560: 0a20 2020 2020 2020 2027 2727 0a0a 2020  .        '''..  
+00019570: 2020 2020 2020 2320 496e 6974 6961 6c20        # Initial 
+00019580: 6775 6573 7320 6973 2061 206c 6973 7420  guess is a list 
+00019590: 6f66 2066 6974 7661 7273 2076 616c 7565  of fitvars value
+000195a0: 730a 2020 2020 2020 2020 6775 6573 7320  s.        guess 
+000195b0: 3d20 5b0a 2020 2020 2020 2020 2020 2020  = [.            
+000195c0: 7661 6c75 6520 666f 7220 6c6f 676d 6f64  value for logmod
+000195d0: 656c 2069 6e20 7365 6c66 2e6c 6f67 6d6f  el in self.logmo
+000195e0: 6465 6c73 0a20 2020 2020 2020 2020 2020  dels.           
+000195f0: 2066 6f72 2076 616c 7565 2069 6e20 6c6f   for value in lo
+00019600: 676d 6f64 656c 2e66 6974 5f76 6172 732e  gmodel.fit_vars.
+00019610: 7661 6c75 6573 2829 0a20 2020 2020 2020  values().       
+00019620: 205d 0a0a 2020 2020 2020 2020 626f 756e   ]..        boun
+00019630: 6473 203d 206e 702e 6172 7261 7928 5b0a  ds = np.array([.
+00019640: 2020 2020 2020 2020 2020 2020 6c6f 676d              logm
+00019650: 6f64 656c 2e42 4f55 4e44 535b 6e61 6d65  odel.BOUNDS[name
+00019660: 5d20 666f 7220 6c6f 676d 6f64 656c 2069  ] for logmodel i
+00019670: 6e20 7365 6c66 2e6c 6f67 6d6f 6465 6c73  n self.logmodels
+00019680: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00019690: 206e 616d 6520 696e 206c 6f67 6d6f 6465   name in logmode
+000196a0: 6c2e 6669 745f 7661 7273 2e6b 6579 7328  l.fit_vars.keys(
+000196b0: 290a 2020 2020 2020 2020 5d29 2e54 0a0a  ).        ]).T..
+000196c0: 2020 2020 2020 2020 6375 7272 5f66 6974          curr_fit
+000196d0: 203d 206c 6561 7374 5f73 7175 6172 6573   = least_squares
+000196e0: 280a 2020 2020 2020 2020 2020 2020 7365  (.            se
+000196f0: 6c66 2e72 6573 6964 7561 6c5f 6672 6f6d  lf.residual_from
+00019700: 5f66 6c6f 6174 5f6c 6973 742c 0a20 2020  _float_list,.   
+00019710: 2020 2020 2020 2020 2061 7267 733d 5b0a           args=[.
+00019720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019730: 7365 6c66 2e6c 6f67 6d6f 6465 6c73 2c0a  self.logmodels,.
+00019740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019750: 6461 7461 7365 742e 7465 6d70 6572 6174  dataset.temperat
+00019760: 7572 6573 2c0a 2020 2020 2020 2020 2020  ures,.          
+00019770: 2020 2020 2020 6e70 2e6c 6f67 3130 2864        np.log10(d
+00019780: 6174 6173 6574 2e72 6174 6573 292c 0a20  ataset.rates),. 
+00019790: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+000197a0: 6174 6173 6574 2e6c 6f67 7261 7465 5f70  ataset.lograte_p
+000197b0: 6d0a 2020 2020 2020 2020 2020 2020 5d2c  m.            ],
+000197c0: 0a20 2020 2020 2020 2020 2020 2078 303d  .            x0=
+000197d0: 6775 6573 732c 0a20 2020 2020 2020 2020  guess,.         
+000197e0: 2020 2062 6f75 6e64 733d 626f 756e 6473     bounds=bounds
+000197f0: 2c0a 2020 2020 2020 2020 2020 2020 6a61  ,.            ja
+00019800: 633d 2733 2d70 6f69 6e74 270a 2020 2020  c='3-point'.    
+00019810: 2020 2020 290a 0a20 2020 2020 2020 2069      )..        i
+00019820: 6620 6375 7272 5f66 6974 2e73 7461 7475  f curr_fit.statu
+00019830: 7320 3d3d 2030 3a0a 2020 2020 2020 2020  s == 0:.        
+00019840: 2020 2020 6966 2076 6572 626f 7365 3a0a      if verbose:.
+00019850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019860: 7574 2e63 7072 696e 7428 0a20 2020 2020  ut.cprint(.     
+00019870: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00019880: 5c6e 2046 6974 2066 6169 6c65 6420 2d20  \n Fit failed - 
+00019890: 546f 6f20 6d61 6e79 2069 7465 7261 7469  Too many iterati
+000198a0: 6f6e 7327 2c0a 2020 2020 2020 2020 2020  ons',.          
+000198b0: 2020 2020 2020 2020 2020 2762 6c61 636b            'black
+000198c0: 5f79 656c 6c6f 7762 6727 0a20 2020 2020  _yellowbg'.     
+000198d0: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+000198e0: 2020 2020 2020 2020 2020 6e5f 6669 7474            n_fitt
+000198f0: 6564 5f70 6172 7320 3d20 6e70 2e73 756d  ed_pars = np.sum
+00019900: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00019910: 2020 5b6c 656e 286c 6f67 6d6f 6465 6c2e    [len(logmodel.
+00019920: 6669 745f 7661 7273 2e6b 6579 7328 2929  fit_vars.keys())
+00019930: 2066 6f72 206c 6f67 6d6f 6465 6c20 696e   for logmodel in
+00019940: 2073 656c 662e 6c6f 676d 6f64 656c 735d   self.logmodels]
+00019950: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
+00019960: 2020 2020 2020 2020 2020 2020 7374 6465              stde
+00019970: 7620 3d20 5b6e 702e 6e61 6e5d 202a 206e  v = [np.nan] * n
+00019980: 5f66 6974 7465 645f 7061 7273 0a20 2020  _fitted_pars.   
+00019990: 2020 2020 2020 2020 2073 656c 662e 6669           self.fi
+000199a0: 745f 7374 6174 7573 203d 2046 616c 7365  t_status = False
+000199b0: 0a20 2020 2020 2020 2065 6c73 653a 0a0a  .        else:..
+000199c0: 2020 2020 2020 2020 2020 2020 7374 6465              stde
+000199d0: 762c 206e 6f5f 7374 6465 7620 3d20 7374  v, no_stdev = st
+000199e0: 6174 732e 7376 645f 7374 6465 7628 6375  ats.svd_stdev(cu
+000199f0: 7272 5f66 6974 290a 0a20 2020 2020 2020  rr_fit)..       
+00019a00: 2020 2020 2073 656c 662e 6669 745f 7374       self.fit_st
+00019a10: 6174 7573 203d 2054 7275 650a 0a20 2020  atus = True..   
+00019a20: 2020 2020 2023 2041 6464 2070 6172 616d       # Add param
+00019a30: 6574 6572 732c 2073 7461 7475 7320 616e  eters, status an
+00019a40: 6420 7374 6465 7620 746f 2065 6163 6820  d stdev to each 
+00019a50: 4c6f 6754 6175 544d 6f64 656c 0a20 2020  LogTauTModel.   
+00019a60: 2020 2020 2069 7420 3d20 300a 2020 2020       it = 0.    
+00019a70: 2020 2020 666f 7220 6c6f 676d 6f64 656c      for logmodel
+00019a80: 2069 6e20 7365 6c66 2e6c 6f67 6d6f 6465   in self.logmode
+00019a90: 6c73 3a0a 0a20 2020 2020 2020 2020 2020  ls:..           
+00019aa0: 2023 204e 616d 6520 6f66 2066 6974 7465   # Name of fitte
+00019ab0: 6420 7661 7269 6162 6c65 7320 696e 2074  d variables in t
+00019ac0: 6869 7320 6c6f 676d 6f64 656c 0a20 2020  his logmodel.   
+00019ad0: 2020 2020 2020 2020 2066 6974 5f76 6172           fit_var
+00019ae0: 5f6e 616d 6573 203d 206c 6f67 6d6f 6465  _names = logmode
+00019af0: 6c2e 6669 745f 7661 7273 2e6b 6579 7328  l.fit_vars.keys(
+00019b00: 290a 2020 2020 2020 2020 2020 2020 2320  ).            # 
+00019b10: 4e75 6d62 6572 206f 6620 7061 7261 6d65  Number of parame
+00019b20: 7465 7273 2066 6f72 2074 6869 7320 6c6f  ters for this lo
+00019b30: 676d 6f64 656c 0a20 2020 2020 2020 2020  gmodel.         
+00019b40: 2020 206e 5f70 6172 7320 3d20 6c65 6e28     n_pars = len(
+00019b50: 6669 745f 7661 725f 6e61 6d65 7329 0a0a  fit_var_names)..
+00019b60: 2020 2020 2020 2020 2020 2020 2320 5365              # Se
+00019b70: 7420 6561 6368 2073 7461 6e64 6172 6420  t each standard 
+00019b80: 6465 7669 6174 696f 6e0a 2020 2020 2020  deviation.      
+00019b90: 2020 2020 2020 5f73 7464 6576 203d 2073        _stdev = s
+00019ba0: 7464 6576 5b69 743a 2069 7420 2b20 6e5f  tdev[it: it + n_
+00019bb0: 7061 7273 5d0a 2020 2020 2020 2020 2020  pars].          
+00019bc0: 2020 6c6f 676d 6f64 656c 2e66 6974 5f73    logmodel.fit_s
+00019bd0: 7464 6576 203d 207b 0a20 2020 2020 2020  tdev = {.       
+00019be0: 2020 2020 2020 2020 206c 6162 656c 3a20           label: 
+00019bf0: 7661 6c0a 2020 2020 2020 2020 2020 2020  val.            
+00019c00: 2020 2020 666f 7220 6c61 6265 6c2c 2076      for label, v
+00019c10: 616c 2069 6e20 7a69 7028 0a20 2020 2020  al in zip(.     
+00019c20: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00019c30: 6974 5f76 6172 5f6e 616d 6573 2c20 5f73  it_var_names, _s
+00019c40: 7464 6576 0a20 2020 2020 2020 2020 2020  tdev.           
+00019c50: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00019c60: 2020 207d 0a0a 2020 2020 2020 2020 2020     }..          
+00019c70: 2020 2320 5265 706f 7274 2073 696e 6775    # Report singu
+00019c80: 6c61 7220 7661 6c75 6573 3d30 206f 6620  lar values=0 of 
+00019c90: 4a61 636f 6269 616e 0a20 2020 2020 2020  Jacobian.       
+00019ca0: 2020 2020 2023 2061 6e64 2069 6e64 6963       # and indic
+00019cb0: 6174 6520 7468 6174 2073 7464 5f64 6576  ate that std_dev
+00019cc0: 2063 616e 6e6f 7420 6265 2063 616c 6375   cannot be calcu
+00019cd0: 6c61 7465 640a 2020 2020 2020 2020 2020  lated.          
+00019ce0: 2020 7369 6e67 7320 3d20 6e6f 5f73 7464    sings = no_std
+00019cf0: 6576 5b69 743a 2069 7420 2b20 6e5f 7061  ev[it: it + n_pa
+00019d00: 7273 5d0a 2020 2020 2020 2020 2020 2020  rs].            
+00019d10: 666f 7220 7061 722c 2073 6920 696e 207a  for par, si in z
+00019d20: 6970 2866 6974 5f76 6172 5f6e 616d 6573  ip(fit_var_names
+00019d30: 2c20 7369 6e67 7329 3a0a 2020 2020 2020  , sings):.      
+00019d40: 2020 2020 2020 2020 2020 6966 2076 6572            if ver
+00019d50: 626f 7365 2061 6e64 206e 6f74 2073 693a  bose and not si:
+00019d60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019d70: 2020 2020 2075 742e 6370 7269 6e74 280a       ut.cprint(.
+00019d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019d90: 2020 2020 2020 2020 6627 5761 726e 696e          f'Warnin
+00019da0: 673a 204a 6163 6f62 6961 6e20 6973 2064  g: Jacobian is d
+00019db0: 6567 656e 6572 6174 6520 666f 7220 7b70  egenerate for {p
+00019dc0: 6172 7d2c 2073 7461 6e64 6172 6420 6465  ar}, standard de
+00019dd0: 7669 6174 696f 6e20 6361 6e6e 6f74 2062  viation cannot b
+00019de0: 6520 666f 756e 642c 2061 6e64 2069 7320  e found, and is 
+00019df0: 7365 7420 746f 207a 6572 6f5c 6e27 2c20  set to zero\n', 
+00019e00: 2320 6e6f 7161 0a20 2020 2020 2020 2020  # noqa.         
+00019e10: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00019e20: 626c 6163 6b5f 7965 6c6c 6f77 6267 270a  black_yellowbg'.
+00019e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019e40: 2020 2020 290a 0a20 2020 2020 2020 2020      )..         
+00019e50: 2020 2023 2053 6574 2066 696e 616c 2066     # Set final f
+00019e60: 6974 7465 6420 7661 6c75 6573 0a20 2020  itted values.   
+00019e70: 2020 2020 2020 2020 205f 7661 6c73 203d           _vals =
+00019e80: 2063 7572 725f 6669 742e 785b 6974 3a20   curr_fit.x[it: 
+00019e90: 6974 202b 206e 5f70 6172 735d 0a20 2020  it + n_pars].   
+00019ea0: 2020 2020 2020 2020 206c 6f67 6d6f 6465           logmode
+00019eb0: 6c2e 6669 6e61 6c5f 7661 725f 7661 6c75  l.final_var_valu
+00019ec0: 6573 203d 207b 0a20 2020 2020 2020 2020  es = {.         
+00019ed0: 2020 2020 2020 206e 616d 653a 2076 616c         name: val
+00019ee0: 7565 0a20 2020 2020 2020 2020 2020 2020  ue.             
+00019ef0: 2020 2066 6f72 206e 616d 652c 2076 616c     for name, val
+00019f00: 7565 2069 6e20 7a69 7028 6669 745f 7661  ue in zip(fit_va
+00019f10: 725f 6e61 6d65 732c 205f 7661 6c73 290a  r_names, _vals).
+00019f20: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+00019f30: 2020 2020 2020 2020 2020 2320 616e 6420            # and 
+00019f40: 6669 7865 6420 7661 6c75 6573 0a20 2020  fixed values.   
+00019f50: 2020 2020 2020 2020 2066 6f72 206b 6579           for key
+00019f60: 2c20 7661 6c20 696e 206c 6f67 6d6f 6465  , val in logmode
+00019f70: 6c2e 6669 785f 7661 7273 2e69 7465 6d73  l.fix_vars.items
+00019f80: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00019f90: 2020 2020 6c6f 676d 6f64 656c 2e66 696e      logmodel.fin
+00019fa0: 616c 5f76 6172 5f76 616c 7565 735b 6b65  al_var_values[ke
+00019fb0: 795d 203d 2076 616c 0a0a 2020 2020 2020  y] = val..      
+00019fc0: 2020 2020 2020 6974 202b 3d20 6e5f 7061        it += n_pa
+00019fd0: 7273 0a0a 2020 2020 2020 2020 7265 7475  rs..        retu
+00019fe0: 726e 0a0a 0a63 6c61 7373 2046 6974 5769  rn...class FitWi
+00019ff0: 6e64 6f77 2851 7457 6964 6765 7473 2e51  ndow(QtWidgets.Q
+0001a000: 4d61 696e 5769 6e64 6f77 293a 0a20 2020  MainWindow):.   
+0001a010: 2027 2727 0a20 2020 2049 6e74 6572 6163   '''.    Interac
+0001a020: 7469 7665 2046 6974 2057 696e 646f 7720  tive Fit Window 
+0001a030: 666f 7220 7261 7465 2076 7320 7465 6d70  for rate vs temp
+0001a040: 6572 6174 7572 652f 6669 656c 6420 6461  erature/field da
+0001a050: 7461 2066 6974 7469 6e67 0a20 2020 2027  ta fitting.    '
+0001a060: 2727 0a0a 2020 2020 6465 6620 5f5f 696e  ''..    def __in
+0001a070: 6974 5f5f 2873 656c 662c 2064 6174 6173  it__(self, datas
+0001a080: 6574 3a20 5461 7554 4461 7461 7365 7420  et: TauTDataset 
+0001a090: 7c20 5461 7548 4461 7461 7365 742c 2075  | TauHDataset, u
+0001a0a0: 7365 6c3a 206f 626a 6563 742c 0a20 2020  sel: object,.   
+0001a0b0: 2020 2020 2020 2020 2020 2020 2020 7375                su
+0001a0c0: 7070 6f72 7465 645f 6d6f 6465 6c73 3a20  pported_models: 
+0001a0d0: 6c69 7374 2c0a 2020 2020 2020 2020 2020  list,.          
+0001a0e0: 2020 2020 2020 2077 6964 6765 745f 6465         widget_de
+0001a0f0: 6661 756c 7473 3a20 6469 6374 5b73 7472  faults: dict[str
+0001a100: 2c20 6469 6374 5b73 7472 2c20 666c 6f61  , dict[str, floa
+0001a110: 745d 5d20 3d20 6775 692e 7769 6467 6574  t]] = gui.widget
+0001a120: 5f64 6566 6175 6c74 732c 2023 206e 6f71  _defaults, # noq
+0001a130: 610a 2020 2020 2020 2020 2020 2020 2020  a.              
+0001a140: 2020 202a 6172 6773 2c20 2a2a 6b77 6172     *args, **kwar
+0001a150: 6773 293a 0a0a 2020 2020 2020 2020 7375  gs):..        su
+0001a160: 7065 7228 4669 7457 696e 646f 772c 2073  per(FitWindow, s
+0001a170: 656c 6629 2e5f 5f69 6e69 745f 5f28 2a61  elf).__init__(*a
+0001a180: 7267 732c 202a 2a6b 7761 7267 7329 0a0a  rgs, **kwargs)..
+0001a190: 2020 2020 2020 2020 2320 4164 6420 7368          # Add sh
+0001a1a0: 6f72 7463 7574 2074 6f20 7072 6573 7320  ortcut to press 
+0001a1b0: 7120 746f 2071 7569 740a 2020 2020 2020  q to quit.      
+0001a1c0: 2020 7365 6c66 2e65 7869 745f 7368 6f72    self.exit_shor
+0001a1d0: 7463 7574 203d 2051 7457 6964 6765 7473  tcut = QtWidgets
+0001a1e0: 2e51 5368 6f72 7463 7574 2851 7447 7569  .QShortcut(QtGui
+0001a1f0: 2e51 4b65 7953 6571 7565 6e63 6528 2771  .QKeySequence('q
+0001a200: 2729 2c20 7365 6c66 290a 2020 2020 2020  '), self).      
+0001a210: 2020 7365 6c66 2e65 7869 745f 7368 6f72    self.exit_shor
+0001a220: 7463 7574 2e61 6374 6976 6174 6564 2e63  tcut.activated.c
+0001a230: 6f6e 6e65 6374 280a 2020 2020 2020 2020  onnect(.        
+0001a240: 2020 2020 6c61 6d62 6461 3a20 7365 6c66      lambda: self
+0001a250: 2e63 6c6f 7365 2829 0a20 2020 2020 2020  .close().       
+0001a260: 2029 0a0a 2020 2020 2020 2020 7365 6c66   )..        self
+0001a270: 2e73 6574 5769 6e64 6f77 5469 746c 6528  .setWindowTitle(
+0001a280: 2749 6e74 6572 6163 7469 7665 2052 656c  'Interactive Rel
+0001a290: 6178 6174 696f 6e20 5072 6f66 696c 6527  axation Profile'
+0001a2a0: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+0001a2b0: 7365 7441 7474 7269 6275 7465 2851 7443  setAttribute(QtC
+0001a2c0: 6f72 652e 5174 2e57 415f 4465 6c65 7465  ore.Qt.WA_Delete
+0001a2d0: 4f6e 436c 6f73 6529 0a20 2020 2020 2020  OnClose).       
+0001a2e0: 2073 656c 662e 7365 7453 7479 6c65 5368   self.setStyleSh
+0001a2f0: 6565 7428 0a20 2020 2020 2020 2020 2020  eet(.           
+0001a300: 2027 2727 0a20 2020 2020 2020 2020 2020   '''.           
+0001a310: 2051 4d61 696e 5769 6e64 6f77 207b 0a20   QMainWindow {. 
+0001a320: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+0001a330: 6163 6b67 726f 756e 642d 636f 6c6f 723a  ackground-color:
+0001a340: 2077 6869 7465 0a20 2020 2020 2020 2020   white.         
+0001a350: 2020 207d 0a0a 2020 2020 2020 2020 2020     }..          
+0001a360: 2020 5143 6865 636b 426f 7820 7b0a 2020    QCheckBox {.  
+0001a370: 2020 2020 2020 2020 2020 2020 2020 7370                sp
+0001a380: 6163 696e 673a 2035 7078 3b0a 2020 2020  acing: 5px;.    
+0001a390: 2020 2020 2020 2020 2020 2020 666f 6e74              font
+0001a3a0: 2d73 697a 653a 3135 7078 3b0a 2020 2020  -size:15px;.    
+0001a3b0: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+0001a3c0: 2020 2020 2020 5153 6c69 6465 723a 3a67        QSlider::g
+0001a3d0: 726f 6f76 653a 686f 7269 7a6f 6e74 616c  roove:horizontal
+0001a3e0: 207b 0a20 2020 2020 2020 2020 2020 2062   {.            b
+0001a3f0: 6f72 6465 723a 2031 7078 2073 6f6c 6964  order: 1px solid
+0001a400: 2023 6262 623b 0a20 2020 2020 2020 2020   #bbb;.         
+0001a410: 2020 2062 6163 6b67 726f 756e 643a 2077     background: w
+0001a420: 6869 7465 3b0a 2020 2020 2020 2020 2020  hite;.          
+0001a430: 2020 6865 6967 6874 3a20 3130 7078 3b0a    height: 10px;.
+0001a440: 2020 2020 2020 2020 2020 2020 626f 7264              bord
+0001a450: 6572 2d72 6164 6975 733a 2034 7078 3b0a  er-radius: 4px;.
+0001a460: 2020 2020 2020 2020 2020 2020 7d0a 0a20              }.. 
+0001a470: 2020 2020 2020 2020 2020 2051 536c 6964             QSlid
+0001a480: 6572 3a3a 7375 622d 7061 6765 3a68 6f72  er::sub-page:hor
+0001a490: 697a 6f6e 7461 6c20 7b0a 2020 2020 2020  izontal {.      
+0001a4a0: 2020 2020 2020 6261 636b 6772 6f75 6e64        background
+0001a4b0: 3a20 716c 696e 6561 7267 7261 6469 656e  : qlineargradien
+0001a4c0: 7428 7831 3a20 302c 2079 313a 2030 2c20  t(x1: 0, y1: 0, 
+0001a4d0: 2020 2078 323a 2030 2c20 7932 3a20 312c     x2: 0, y2: 1,
+0001a4e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a4f0: 2073 746f 703a 2030 2023 3636 652c 2073   stop: 0 #66e, s
+0001a500: 746f 703a 2031 2023 6262 6629 3b0a 2020  top: 1 #bbf);.  
+0001a510: 2020 2020 2020 2020 2020 6261 636b 6772            backgr
+0001a520: 6f75 6e64 3a20 716c 696e 6561 7267 7261  ound: qlineargra
+0001a530: 6469 656e 7428 7831 3a20 302c 2079 313a  dient(x1: 0, y1:
+0001a540: 2030 2e32 2c20 7832 3a20 312c 2079 323a   0.2, x2: 1, y2:
+0001a550: 2031 2c0a 2020 2020 2020 2020 2020 2020   1,.            
+0001a560: 2020 2020 7374 6f70 3a20 3020 2362 6266      stop: 0 #bbf
+0001a570: 2c20 7374 6f70 3a20 3120 2335 3566 293b  , stop: 1 #55f);
+0001a580: 0a20 2020 2020 2020 2020 2020 2062 6f72  .            bor
+0001a590: 6465 723a 2031 7078 2073 6f6c 6964 2023  der: 1px solid #
+0001a5a0: 3737 373b 0a20 2020 2020 2020 2020 2020  777;.           
+0001a5b0: 2068 6569 6768 743a 2031 3070 783b 0a20   height: 10px;. 
+0001a5c0: 2020 2020 2020 2020 2020 2062 6f72 6465             borde
+0001a5d0: 722d 7261 6469 7573 3a20 3470 783b 0a20  r-radius: 4px;. 
+0001a5e0: 2020 2020 2020 2020 2020 207d 0a0a 2020             }..  
+0001a5f0: 2020 2020 2020 2020 2020 5153 6c69 6465            QSlide
+0001a600: 723a 3a61 6464 2d70 6167 653a 686f 7269  r::add-page:hori
+0001a610: 7a6f 6e74 616c 207b 0a20 2020 2020 2020  zontal {.       
+0001a620: 2020 2020 2062 6163 6b67 726f 756e 643a       background:
+0001a630: 2023 6666 663b 0a20 2020 2020 2020 2020   #fff;.         
+0001a640: 2020 2062 6f72 6465 723a 2031 7078 2073     border: 1px s
+0001a650: 6f6c 6964 2023 3737 373b 0a20 2020 2020  olid #777;.     
+0001a660: 2020 2020 2020 2068 6569 6768 743a 2031         height: 1
+0001a670: 3070 783b 0a20 2020 2020 2020 2020 2020  0px;.           
+0001a680: 2062 6f72 6465 722d 7261 6469 7573 3a20   border-radius: 
+0001a690: 3470 783b 0a20 2020 2020 2020 2020 2020  4px;.           
+0001a6a0: 207d 0a0a 2020 2020 2020 2020 2020 2020   }..            
+0001a6b0: 5153 6c69 6465 723a 3a68 616e 646c 653a  QSlider::handle:
+0001a6c0: 686f 7269 7a6f 6e74 616c 207b 0a20 2020  horizontal {.   
+0001a6d0: 2020 2020 2020 2020 2062 6163 6b67 726f           backgro
+0001a6e0: 756e 643a 2071 6c69 6e65 6172 6772 6164  und: qlineargrad
+0001a6f0: 6965 6e74 2878 313a 302c 2079 313a 302c  ient(x1:0, y1:0,
+0001a700: 2078 323a 312c 2079 323a 312c 0a20 2020   x2:1, y2:1,.   
+0001a710: 2020 2020 2020 2020 2020 2020 2073 746f               sto
+0001a720: 703a 3020 2365 6565 2c20 7374 6f70 3a31  p:0 #eee, stop:1
+0001a730: 2023 6363 6329 3b0a 2020 2020 2020 2020   #ccc);.        
+0001a740: 2020 2020 626f 7264 6572 3a20 3170 7820      border: 1px 
+0001a750: 736f 6c69 6420 2337 3737 3b0a 2020 2020  solid #777;.    
+0001a760: 2020 2020 2020 2020 7769 6474 683a 2031          width: 1
+0001a770: 3370 783b 0a20 2020 2020 2020 2020 2020  3px;.           
+0001a780: 206d 6172 6769 6e2d 746f 703a 202d 3270   margin-top: -2p
+0001a790: 783b 0a20 2020 2020 2020 2020 2020 206d  x;.            m
+0001a7a0: 6172 6769 6e2d 626f 7474 6f6d 3a20 2d32  argin-bottom: -2
+0001a7b0: 7078 3b0a 2020 2020 2020 2020 2020 2020  px;.            
+0001a7c0: 626f 7264 6572 2d72 6164 6975 733a 2034  border-radius: 4
+0001a7d0: 7078 3b0a 2020 2020 2020 2020 2020 2020  px;.            
+0001a7e0: 7d0a 0a20 2020 2020 2020 2020 2020 2051  }..            Q
+0001a7f0: 536c 6964 6572 3a3a 6861 6e64 6c65 3a68  Slider::handle:h
+0001a800: 6f72 697a 6f6e 7461 6c3a 686f 7665 7220  orizontal:hover 
+0001a810: 7b0a 2020 2020 2020 2020 2020 2020 6261  {.            ba
+0001a820: 636b 6772 6f75 6e64 3a20 716c 696e 6561  ckground: qlinea
+0001a830: 7267 7261 6469 656e 7428 7831 3a30 2c20  rgradient(x1:0, 
+0001a840: 7931 3a30 2c20 7832 3a31 2c20 7932 3a31  y1:0, x2:1, y2:1
+0001a850: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001a860: 2020 7374 6f70 3a30 2023 6666 662c 2073    stop:0 #fff, s
+0001a870: 746f 703a 3120 2364 6464 293b 0a20 2020  top:1 #ddd);.   
+0001a880: 2020 2020 2020 2020 2062 6f72 6465 723a           border:
+0001a890: 2031 7078 2073 6f6c 6964 2023 3434 343b   1px solid #444;
+0001a8a0: 0a20 2020 2020 2020 2020 2020 2062 6f72  .            bor
+0001a8b0: 6465 722d 7261 6469 7573 3a20 3470 783b  der-radius: 4px;
+0001a8c0: 0a20 2020 2020 2020 2020 2020 207d 0a0a  .            }..
+0001a8d0: 2020 2020 2020 2020 2020 2020 5153 6c69              QSli
+0001a8e0: 6465 723a 3a73 7562 2d70 6167 653a 686f  der::sub-page:ho
+0001a8f0: 7269 7a6f 6e74 616c 3a64 6973 6162 6c65  rizontal:disable
+0001a900: 6420 7b0a 2020 2020 2020 2020 2020 2020  d {.            
+0001a910: 6261 636b 6772 6f75 6e64 3a20 2362 6262  background: #bbb
+0001a920: 3b0a 2020 2020 2020 2020 2020 2020 626f  ;.            bo
+0001a930: 7264 6572 2d63 6f6c 6f72 3a20 2339 3939  rder-color: #999
+0001a940: 3b0a 2020 2020 2020 2020 2020 2020 7d0a  ;.            }.
+0001a950: 0a20 2020 2020 2020 2020 2020 2051 536c  .            QSl
+0001a960: 6964 6572 3a3a 6164 642d 7061 6765 3a68  ider::add-page:h
+0001a970: 6f72 697a 6f6e 7461 6c3a 6469 7361 626c  orizontal:disabl
+0001a980: 6564 207b 0a20 2020 2020 2020 2020 2020  ed {.           
+0001a990: 2062 6163 6b67 726f 756e 643a 2023 6565   background: #ee
+0001a9a0: 653b 0a20 2020 2020 2020 2020 2020 2062  e;.            b
+0001a9b0: 6f72 6465 722d 636f 6c6f 723a 2023 3939  order-color: #99
+0001a9c0: 393b 0a20 2020 2020 2020 2020 2020 207d  9;.            }
+0001a9d0: 0a0a 2020 2020 2020 2020 2020 2020 5153  ..            QS
+0001a9e0: 6c69 6465 723a 3a68 616e 646c 653a 686f  lider::handle:ho
+0001a9f0: 7269 7a6f 6e74 616c 3a64 6973 6162 6c65  rizontal:disable
+0001aa00: 6420 7b0a 2020 2020 2020 2020 2020 2020  d {.            
+0001aa10: 6261 636b 6772 6f75 6e64 3a20 2365 6565  background: #eee
+0001aa20: 3b0a 2020 2020 2020 2020 2020 2020 626f  ;.            bo
+0001aa30: 7264 6572 3a20 3170 7820 736f 6c69 6420  rder: 1px solid 
+0001aa40: 2361 6161 3b0a 2020 2020 2020 2020 2020  #aaa;.          
+0001aa50: 2020 626f 7264 6572 2d72 6164 6975 733a    border-radius:
+0001aa60: 2034 7078 3b0a 2020 2020 2020 2020 2020   4px;.          
+0001aa70: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
+0001aa80: 2727 270a 2020 2020 2020 2020 290a 0a20  '''.        ).. 
+0001aa90: 2020 2020 2020 2023 2053 6574 2064 6566         # Set def
+0001aaa0: 6175 6c74 206d 696e 2c20 6d61 782c 2069  ault min, max, i
+0001aab0: 6e69 742c 2061 6e64 2073 7465 7020 7661  nit, and step va
+0001aac0: 6c75 6573 206f 6620 736c 6964 6572 7320  lues of sliders 
+0001aad0: 616e 6420 7465 7874 2062 6f78 6573 0a20  and text boxes. 
+0001aae0: 2020 2020 2020 2073 656c 662e 6465 6661         self.defa
+0001aaf0: 756c 7473 203d 2077 6964 6765 745f 6465  ults = widget_de
+0001ab00: 6661 756c 7473 0a0a 2020 2020 2020 2020  faults..        
+0001ab10: 2320 4469 6374 696f 6e61 7279 2066 6f72  # Dictionary for
+0001ab20: 2074 6963 6b62 6f78 2077 6964 6765 7473   tickbox widgets
+0001ab30: 0a20 2020 2020 2020 2073 656c 662e 7469  .        self.ti
+0001ab40: 636b 6469 6374 203d 207b 0a20 2020 2020  ckdict = {.     
+0001ab50: 2020 2020 2020 206d 6f64 656c 2e4e 414d         model.NAM
+0001ab60: 452e 6c6f 7765 7228 293a 204e 6f6e 650a  E.lower(): None.
+0001ab70: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0001ab80: 6d6f 6465 6c20 696e 2073 7570 706f 7274  model in support
+0001ab90: 6564 5f6d 6f64 656c 730a 2020 2020 2020  ed_models.      
+0001aba0: 2020 7d0a 0a20 2020 2020 2020 2023 2044    }..        # D
+0001abb0: 6963 7469 6f6e 6172 7920 666f 7220 7061  ictionary for pa
+0001abc0: 7261 6d65 7465 7220 736c 6964 6572 2c20  rameter slider, 
+0001abd0: 656e 7472 792c 2061 6e64 2066 6974 6669  entry, and fitfi
+0001abe0: 7820 7769 6467 6574 730a 2020 2020 2020  x widgets.      
+0001abf0: 2020 7365 6c66 2e77 6964 6765 7464 6963    self.widgetdic
+0001ac00: 7420 3d20 7b0a 2020 2020 2020 2020 2020  t = {.          
+0001ac10: 2020 6d6f 6465 6c2e 4e41 4d45 2e6c 6f77    model.NAME.low
+0001ac20: 6572 2829 3a20 7b0a 2020 2020 2020 2020  er(): {.        
+0001ac30: 2020 2020 2020 2020 7061 726e 616d 653a          parname:
+0001ac40: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+0001ac50: 2020 2020 2020 2027 736c 6964 6572 273a         'slider':
+0001ac60: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
+0001ac70: 2020 2020 2020 2020 2020 2027 6666 5f74             'ff_t
+0001ac80: 6f67 676c 6527 3a20 4e6f 6e65 2c0a 2020  oggle': None,.  
+0001ac90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001aca0: 2020 2765 6e74 7279 273a 204e 6f6e 650a    'entry': None.
+0001acb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001acc0: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+0001acd0: 2020 666f 7220 7061 726e 616d 6520 696e    for parname in
+0001ace0: 206d 6f64 656c 2e50 4152 4e41 4d45 530a   model.PARNAMES.
+0001acf0: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+0001ad00: 2020 2020 2020 2020 2020 666f 7220 6d6f            for mo
+0001ad10: 6465 6c20 696e 2073 7570 706f 7274 6564  del in supported
+0001ad20: 5f6d 6f64 656c 730a 2020 2020 2020 2020  _models.        
+0001ad30: 7d0a 0a20 2020 2020 2020 2023 204d 696e  }..        # Min
+0001ad40: 696d 756d 2057 696e 646f 7720 7369 7a65  imum Window size
+0001ad50: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
+0001ad60: 744d 696e 696d 756d 5369 7a65 2851 7443  tMinimumSize(QtC
+0001ad70: 6f72 652e 5153 697a 6528 3132 3030 2c20  ore.QSize(1200, 
+0001ad80: 3730 3029 290a 0a20 2020 2020 2020 2023  700))..        #
+0001ad90: 204d 616b 6520 7769 6467 6574 7320 666f   Make widgets fo
+0001ada0: 7220 656e 7469 7265 2077 696e 646f 770a  r entire window.
+0001adb0: 2020 2020 2020 2020 7365 6c66 2e77 6964          self.wid
+0001adc0: 6765 7420 3d20 5174 5769 6467 6574 732e  get = QtWidgets.
+0001add0: 5157 6964 6765 7428 7061 7265 6e74 3d73  QWidget(parent=s
+0001ade0: 656c 6629 0a20 2020 2020 2020 2073 656c  elf).        sel
+0001adf0: 662e 7365 7443 656e 7472 616c 5769 6467  f.setCentralWidg
+0001ae00: 6574 2873 656c 662e 7769 6467 6574 290a  et(self.widget).
+0001ae10: 2020 2020 2020 2020 626f 745f 726f 775f          bot_row_
+0001ae20: 7769 6467 6574 203d 2051 7457 6964 6765  widget = QtWidge
+0001ae30: 7473 2e51 5769 6467 6574 2873 656c 662e  ts.QWidget(self.
+0001ae40: 7769 6467 6574 290a 2020 2020 2020 2020  widget).        
+0001ae50: 746f 705f 726f 775f 7769 6467 6574 203d  top_row_widget =
+0001ae60: 2051 7457 6964 6765 7473 2e51 5769 6467   QtWidgets.QWidg
+0001ae70: 6574 2873 656c 662e 7769 6467 6574 290a  et(self.widget).
+0001ae80: 2020 2020 2020 2020 7268 735f 636f 6c5f          rhs_col_
+0001ae90: 7769 6467 6574 203d 2051 7457 6964 6765  widget = QtWidge
+0001aea0: 7473 2e51 5769 6467 6574 2874 6f70 5f72  ts.QWidget(top_r
+0001aeb0: 6f77 5f77 6964 6765 7429 0a0a 2020 2020  ow_widget)..    
+0001aec0: 2020 2020 7268 735f 636f 6c5f 7363 726f      rhs_col_scro
+0001aed0: 6c6c 203d 2051 7457 6964 6765 7473 2e51  ll = QtWidgets.Q
+0001aee0: 5363 726f 6c6c 4172 6561 2872 6873 5f63  ScrollArea(rhs_c
+0001aef0: 6f6c 5f77 6964 6765 7429 0a20 2020 2020  ol_widget).     
+0001af00: 2020 2072 6873 5f63 6f6c 5f73 6372 6f6c     rhs_col_scrol
+0001af10: 6c2e 7365 7456 6572 7469 6361 6c53 6372  l.setVerticalScr
+0001af20: 6f6c 6c42 6172 506f 6c69 6379 280a 2020  ollBarPolicy(.  
+0001af30: 2020 2020 2020 2020 2020 5174 436f 7265            QtCore
+0001af40: 2e51 742e 5363 726f 6c6c 4261 7241 6c77  .Qt.ScrollBarAlw
+0001af50: 6179 734f 6e0a 2020 2020 2020 2020 290a  aysOn.        ).
+0001af60: 2020 2020 2020 2020 7268 735f 636f 6c5f          rhs_col_
+0001af70: 7363 726f 6c6c 2e73 6574 486f 7269 7a6f  scroll.setHorizo
+0001af80: 6e74 616c 5363 726f 6c6c 4261 7250 6f6c  ntalScrollBarPol
+0001af90: 6963 7928 0a20 2020 2020 2020 2020 2020  icy(.           
+0001afa0: 2051 7443 6f72 652e 5174 2e53 6372 6f6c   QtCore.Qt.Scrol
+0001afb0: 6c42 6172 416c 7761 7973 4f66 660a 2020  lBarAlwaysOff.  
+0001afc0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0001afd0: 7268 735f 636f 6c5f 7363 726f 6c6c 2e73  rhs_col_scroll.s
+0001afe0: 6574 5769 6467 6574 5265 7369 7a61 626c  etWidgetResizabl
+0001aff0: 6528 5472 7565 290a 0a20 2020 2020 2020  e(True)..       
+0001b000: 2073 6372 6f6c 6c5f 636f 6e74 6169 6e65   scroll_containe
+0001b010: 7220 3d20 5174 5769 6467 6574 732e 5157  r = QtWidgets.QW
+0001b020: 6964 6765 7428 7268 735f 636f 6c5f 7363  idget(rhs_col_sc
+0001b030: 726f 6c6c 290a 2020 2020 2020 2020 7268  roll).        rh
+0001b040: 735f 636f 6c5f 7363 726f 6c6c 2e73 6574  s_col_scroll.set
+0001b050: 5769 6467 6574 2873 6372 6f6c 6c5f 636f  Widget(scroll_co
+0001b060: 6e74 6169 6e65 7229 0a0a 2020 2020 2020  ntainer)..      
+0001b070: 2020 6c68 735f 636f 6c5f 7769 6467 6574    lhs_col_widget
+0001b080: 203d 2051 7457 6964 6765 7473 2e51 5769   = QtWidgets.QWi
+0001b090: 6467 6574 2874 6f70 5f72 6f77 5f77 6964  dget(top_row_wid
+0001b0a0: 6765 7429 0a0a 2020 2020 2020 2020 2320  get)..        # 
+0001b0b0: 4c48 5320 636f 6c75 6d6e 202d 2070 6c6f  LHS column - plo
+0001b0c0: 7420 6f6e 6c79 0a20 2020 2020 2020 206c  t only.        l
+0001b0d0: 6873 5f63 6f6c 5f6c 6179 6f75 7420 3d20  hs_col_layout = 
+0001b0e0: 5174 5769 6467 6574 732e 5156 426f 784c  QtWidgets.QVBoxL
+0001b0f0: 6179 6f75 7428 6c68 735f 636f 6c5f 7769  ayout(lhs_col_wi
+0001b100: 6467 6574 290a 0a20 2020 2020 2020 2023  dget)..        #
+0001b110: 206d 616b 6520 7067 6670 6c6f 7473 2070   make pgfplots p
+0001b120: 6c6f 7420 7769 6467 6574 0a20 2020 2020  lot widget.     
+0001b130: 2020 2073 656c 662e 706c 6f74 5f77 6964     self.plot_wid
+0001b140: 6765 7420 3d20 7067 2e50 6c6f 7457 6964  get = pg.PlotWid
+0001b150: 6765 7428 0a20 2020 2020 2020 2020 2020  get(.           
+0001b160: 2070 6172 656e 743d 6c68 735f 636f 6c5f   parent=lhs_col_
+0001b170: 7769 6467 6574 0a20 2020 2020 2020 2029  widget.        )
+0001b180: 0a20 2020 2020 2020 2023 2041 6464 2070  .        # Add p
+0001b190: 6c6f 7420 746f 206c 6566 7420 636f 6c75  lot to left colu
+0001b1a0: 6d6e 0a20 2020 2020 2020 206c 6873 5f63  mn.        lhs_c
+0001b1b0: 6f6c 5f6c 6179 6f75 742e 6164 6457 6964  ol_layout.addWid
+0001b1c0: 6765 7428 7365 6c66 2e70 6c6f 745f 7769  get(self.plot_wi
+0001b1d0: 6467 6574 290a 0a20 2020 2020 2020 2023  dget)..        #
+0001b1e0: 2053 6574 206c 6f67 6c6f 6720 6178 6573   Set loglog axes
+0001b1f0: 0a20 2020 2020 2020 2073 656c 662e 706c  .        self.pl
+0001b200: 6f74 5f77 6964 6765 742e 7365 744c 6f67  ot_widget.setLog
+0001b210: 4d6f 6465 2854 7275 652c 2054 7275 6529  Mode(True, True)
+0001b220: 0a0a 2020 2020 2020 2020 2320 5365 7420  ..        # Set 
+0001b230: 7768 6974 6520 706c 6f74 2062 6163 6b67  white plot backg
+0001b240: 726f 756e 640a 2020 2020 2020 2020 7365  round.        se
+0001b250: 6c66 2e70 6c6f 745f 7769 6467 6574 2e73  lf.plot_widget.s
+0001b260: 6574 4261 636b 6772 6f75 6e64 2827 7727  etBackground('w'
+0001b270: 290a 0a20 2020 2020 2020 2023 2053 656c  )..        # Sel
+0001b280: 6563 7420 6569 7468 6572 2066 6965 6c64  ect either field
+0001b290: 206f 7220 7465 6d70 6572 6174 7572 6520   or temperature 
+0001b2a0: 6173 2078 2064 6174 6120 6261 7365 6420  as x data based 
+0001b2b0: 6f6e 2064 6174 6173 6574 2074 7970 650a  on dataset type.
+0001b2c0: 2020 2020 2020 2020 2320 616e 6420 7365          # and se
+0001b2d0: 7420 7820 6c61 6265 6c20 6f66 2070 6c6f  t x label of plo
+0001b2e0: 740a 2020 2020 2020 2020 6966 2069 7369  t.        if isi
+0001b2f0: 6e73 7461 6e63 6528 6461 7461 7365 742c  nstance(dataset,
+0001b300: 2054 6175 4844 6174 6173 6574 293a 0a20   TauHDataset):. 
+0001b310: 2020 2020 2020 2020 2020 2078 5f76 616c             x_val
+0001b320: 7320 3d20 6461 7461 7365 742e 6669 656c  s = dataset.fiel
+0001b330: 6473 0a20 2020 2020 2020 2020 2020 2073  ds.            s
+0001b340: 656c 662e 706c 6f74 5f77 6964 6765 742e  elf.plot_widget.
+0001b350: 7365 744c 6162 656c 2827 626f 7474 6f6d  setLabel('bottom
+0001b360: 272c 2027 4669 656c 6420 284f 6529 2729  ', 'Field (Oe)')
+0001b370: 0a0a 2020 2020 2020 2020 656c 6966 2069  ..        elif i
+0001b380: 7369 6e73 7461 6e63 6528 6461 7461 7365  sinstance(datase
+0001b390: 742c 2054 6175 5444 6174 6173 6574 293a  t, TauTDataset):
+0001b3a0: 0a20 2020 2020 2020 2020 2020 2078 5f76  .            x_v
+0001b3b0: 616c 7320 3d20 6461 7461 7365 742e 7465  als = dataset.te
+0001b3c0: 6d70 6572 6174 7572 6573 0a20 2020 2020  mperatures.     
+0001b3d0: 2020 2020 2020 2073 656c 662e 706c 6f74         self.plot
+0001b3e0: 5f77 6964 6765 742e 7365 744c 6162 656c  _widget.setLabel
+0001b3f0: 2827 626f 7474 6f6d 272c 2027 5465 6d70  ('bottom', 'Temp
+0001b400: 6572 6174 7572 6520 284b 2927 290a 0a20  erature (K)').. 
+0001b410: 2020 2020 2020 2023 2045 7870 6572 696d         # Experim
+0001b420: 656e 7461 6c20 6461 7461 0a20 2020 2020  ental data.     
+0001b430: 2020 2073 656c 662e 6578 7020 3d20 7365     self.exp = se
+0001b440: 6c66 2e70 6c6f 745f 7769 6467 6574 2e70  lf.plot_widget.p
+0001b450: 6c6f 7428 0a20 2020 2020 2020 2020 2020  lot(.           
+0001b460: 206e 702e 6172 7261 7928 785f 7661 6c73   np.array(x_vals
+0001b470: 292c 0a20 2020 2020 2020 2020 2020 206e  ),.            n
+0001b480: 702e 6172 7261 7928 6461 7461 7365 742e  p.array(dataset.
+0001b490: 7261 7465 7329 2c0a 2020 2020 2020 2020  rates),.        
+0001b4a0: 2020 2020 7065 6e3d 4e6f 6e65 2c0a 2020      pen=None,.  
+0001b4b0: 2020 2020 2020 2020 2020 7379 6d62 6f6c            symbol
+0001b4c0: 3d27 7827 2c0a 2020 2020 2020 2020 2020  ='x',.          
+0001b4d0: 2020 7379 6d62 6f6c 4272 7573 683d 2830    symbolBrush=(0
+0001b4e0: 2c20 302c 2030 290a 2020 2020 2020 2020  , 0, 0).        
+0001b4f0: 290a 0a20 2020 2020 2020 2023 2046 696e  )..        # Fin
+0001b500: 6420 6e69 6365 2079 2d61 7869 7320 6c69  d nice y-axis li
+0001b510: 6d69 7473 0a20 2020 2020 2020 2079 5f6c  mits.        y_l
+0001b520: 6f77 6572 2c20 795f 7570 7065 7220 3d20  ower, y_upper = 
+0001b530: 6775 692e 6361 6c63 5f79 5f72 6174 655f  gui.calc_y_rate_
+0001b540: 6c69 6d73 280a 2020 2020 2020 2020 2020  lims(.          
+0001b550: 2020 6461 7461 7365 742e 7261 7465 732c    dataset.rates,
+0001b560: 0a20 2020 2020 2020 2020 2020 206e 702e  .            np.
+0001b570: 6172 7261 7928 6461 7461 7365 742e 7261  array(dataset.ra
+0001b580: 7465 5f70 6d29 0a20 2020 2020 2020 2029  te_pm).        )
+0001b590: 0a0a 2020 2020 2020 2020 2320 436c 6970  ..        # Clip
+0001b5a0: 2074 6865 6d20 6174 2073 656e 7369 626c   them at sensibl
+0001b5b0: 6520 7661 6c75 6573 0a20 2020 2020 2020  e values.       
+0001b5c0: 205b 795f 6c6f 7765 722c 2079 5f75 7070   [y_lower, y_upp
+0001b5d0: 6572 5d20 3d20 6e70 2e63 6c69 7028 5b79  er] = np.clip([y
+0001b5e0: 5f6c 6f77 6572 2c20 795f 7570 7065 725d  _lower, y_upper]
+0001b5f0: 2c20 3145 2d31 302c 2031 4531 3029 0a0a  , 1E-10, 1E10)..
+0001b600: 2020 2020 2020 2020 2320 616e 6420 7365          # and se
+0001b610: 7420 7661 6c75 6573 0a20 2020 2020 2020  t values.       
+0001b620: 2073 656c 662e 706c 6f74 5f77 6964 6765   self.plot_widge
+0001b630: 742e 7365 7459 5261 6e67 6528 0a20 2020  t.setYRange(.   
+0001b640: 2020 2020 2020 2020 206e 702e 6c6f 6731           np.log1
+0001b650: 3028 795f 6c6f 7765 7229 2c0a 2020 2020  0(y_lower),.    
+0001b660: 2020 2020 2020 2020 6e70 2e6c 6f67 3130          np.log10
+0001b670: 2879 5f75 7070 6572 292c 0a20 2020 2020  (y_upper),.     
+0001b680: 2020 2020 2020 2070 6164 6469 6e67 3d30         padding=0
+0001b690: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+0001b6a0: 2020 2020 2320 4164 6420 6578 7065 7269      # Add experi
+0001b6b0: 6d65 6e74 616c 2065 7272 6f72 6261 7273  mental errorbars
+0001b6c0: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
+0001b6d0: 6461 7461 7365 742e 6c6f 6772 6174 655f  dataset.lograte_
+0001b6e0: 706d 293a 0a20 2020 2020 2020 2020 2020  pm):.           
+0001b6f0: 2065 7272 203d 2070 672e 4572 726f 7242   err = pg.ErrorB
+0001b700: 6172 4974 656d 280a 2020 2020 2020 2020  arItem(.        
+0001b710: 2020 2020 2020 2020 783d 6e70 2e6c 6f67          x=np.log
+0001b720: 3130 2878 5f76 616c 7329 2c0a 2020 2020  10(x_vals),.    
+0001b730: 2020 2020 2020 2020 2020 2020 793d 6e70              y=np
+0001b740: 2e6c 6f67 3130 2864 6174 6173 6574 2e72  .log10(dataset.r
+0001b750: 6174 6573 292c 0a20 2020 2020 2020 2020  ates),.         
+0001b760: 2020 2020 2020 2074 6f70 3d64 6174 6173         top=datas
+0001b770: 6574 2e6c 6f67 7261 7465 5f70 6d2c 0a20  et.lograte_pm,. 
+0001b780: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+0001b790: 6f74 746f 6d3d 6461 7461 7365 742e 6c6f  ottom=dataset.lo
+0001b7a0: 6772 6174 655f 706d 2c0a 2020 2020 2020  grate_pm,.      
+0001b7b0: 2020 2020 2020 2020 2020 6265 616d 3d30            beam=0
+0001b7c0: 2e30 3035 0a20 2020 2020 2020 2020 2020  .005.           
+0001b7d0: 2029 0a20 2020 2020 2020 2020 2020 2073   ).            s
+0001b7e0: 656c 662e 706c 6f74 5f77 6964 6765 742e  elf.plot_widget.
+0001b7f0: 6164 6449 7465 6d28 6572 7229 0a0a 2020  addItem(err)..  
+0001b800: 2020 2020 2020 2320 4178 6973 206c 6162        # Axis lab
+0001b810: 656c 730a 2020 2020 2020 2020 7365 6c66  els.        self
+0001b820: 2e70 6c6f 745f 7769 6467 6574 2e73 6574  .plot_widget.set
+0001b830: 4c61 6265 6c28 276c 6566 7427 2c20 2752  Label('left', 'R
+0001b840: 6174 6520 2873 3c73 7570 3e2d 313c 2f73  ate (s<sup>-1</s
+0001b850: 7570 3e29 2729 0a0a 2020 2020 2020 2020  up>)')..        
+0001b860: 2320 5365 7420 6469 6374 696f 6e61 7279  # Set dictionary
+0001b870: 206f 6620 5472 7565 2028 6669 7429 2061   of True (fit) a
+0001b880: 6e64 2046 616c 7365 2028 6669 7829 2066  nd False (fix) f
+0001b890: 6f72 2065 6163 680a 2020 2020 2020 2020  or each.        
+0001b8a0: 2320 7061 7261 6d65 7465 7220 6f66 2061  # parameter of a
+0001b8b0: 6c6c 2061 7661 696c 6162 6c65 206d 6f64  ll available mod
+0001b8c0: 656c 730a 2020 2020 2020 2020 7573 656c  els.        usel
+0001b8d0: 2e66 6974 203d 207b 0a20 2020 2020 2020  .fit = {.       
+0001b8e0: 2020 2020 2070 6172 6e61 6d65 3a20 5472       parname: Tr
+0001b8f0: 7565 0a20 2020 2020 2020 2020 2020 2066  ue.            f
+0001b900: 6f72 206d 6f64 656c 2069 6e20 7375 7070  or model in supp
+0001b910: 6f72 7465 645f 6d6f 6465 6c73 0a20 2020  orted_models.   
+0001b920: 2020 2020 2020 2020 2066 6f72 2070 6172           for par
+0001b930: 6e61 6d65 2069 6e20 6d6f 6465 6c2e 5041  name in model.PA
+0001b940: 524e 414d 4553 0a20 2020 2020 2020 207d  RNAMES.        }
+0001b950: 0a0a 2020 2020 2020 2020 2320 5365 7420  ..        # Set 
+0001b960: 7573 6572 2073 656c 6563 7469 6f6e 206f  user selection o
+0001b970: 626a 6563 7420 616e 6420 7375 7070 6f72  bject and suppor
+0001b980: 7465 6420 6d6f 6465 6c73 0a20 2020 2020  ted models.     
+0001b990: 2020 2073 656c 662e 7573 656c 203d 2075     self.usel = u
+0001b9a0: 7365 6c0a 2020 2020 2020 2020 7365 6c66  sel.        self
+0001b9b0: 2e73 7570 706f 7274 6564 5f6d 6f64 656c  .supported_model
+0001b9c0: 7320 3d20 7375 7070 6f72 7465 645f 6d6f  s = supported_mo
+0001b9d0: 6465 6c73 0a0a 2020 2020 2020 2020 2320  dels..        # 
+0001b9e0: 4361 6c63 756c 6174 6520 6561 6368 206d  Calculate each m
+0001b9f0: 6f64 656c 2066 756e 6374 696f 6e20 616e  odel function an
+0001ba00: 6420 706c 6f74 0a20 2020 2020 2020 2073  d plot.        s
+0001ba10: 656c 662e 7465 6d70 5f67 7269 6420 3d20  elf.temp_grid = 
+0001ba20: 6e70 2e6c 696e 7370 6163 6528 0a20 2020  np.linspace(.   
+0001ba30: 2020 2020 2020 2020 206e 702e 6d69 6e28           np.min(
+0001ba40: 785f 7661 6c73 292c 206e 702e 6d61 7828  x_vals), np.max(
+0001ba50: 785f 7661 6c73 292c 2031 3030 300a 2020  x_vals), 1000.  
+0001ba60: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+0001ba70: 2023 2053 756d 206f 6620 616c 6c20 6d6f   # Sum of all mo
+0001ba80: 6465 6c73 2c20 7365 7420 746f 207a 6572  dels, set to zer
+0001ba90: 6f20 696e 6974 6961 6c6c 790a 2020 2020  o initially.    
+0001baa0: 2020 2020 746f 7461 6c5f 7261 7465 7320      total_rates 
+0001bab0: 3d20 6e70 2e7a 6572 6f73 286e 702e 7368  = np.zeros(np.sh
+0001bac0: 6170 6528 7365 6c66 2e74 656d 705f 6772  ape(self.temp_gr
+0001bad0: 6964 2929 0a0a 2020 2020 2020 2020 2320  id))..        # 
+0001bae0: 4469 6374 696f 6e61 7279 206f 6620 706c  Dictionary of pl
+0001baf0: 6f74 730a 2020 2020 2020 2020 2320 6b65  ots.        # ke
+0001bb00: 7973 2061 7265 206d 6f64 656c 2e4e 414d  ys are model.NAM
+0001bb10: 452e 6c6f 7765 7228 292c 2076 616c 7565  E.lower(), value
+0001bb20: 7320 6172 6520 706c 6f74 5f77 6964 6765  s are plot_widge
+0001bb30: 742e 706c 6f74 0a20 2020 2020 2020 2073  t.plot.        s
+0001bb40: 656c 662e 6d6f 6465 6c5f 706c 6f74 7320  elf.model_plots 
+0001bb50: 3d20 7b7d 0a0a 2020 2020 2020 2020 2320  = {}..        # 
+0001bb60: 4c69 7374 206f 6620 6e69 6365 2063 6f6c  List of nice col
+0001bb70: 6f72 730a 2020 2020 2020 2020 636f 6c6f  ors.        colo
+0001bb80: 7273 203d 206d 636f 6c6f 7273 2e54 4142  rs = mcolors.TAB
+0001bb90: 4c45 4155 5f43 4f4c 4f52 532e 7661 6c75  LEAU_COLORS.valu
+0001bba0: 6573 2829 0a0a 2020 2020 2020 2020 2320  es()..        # 
+0001bbb0: 4c6f 6f70 206f 7665 7220 616c 6c20 706f  Loop over all po
+0001bbc0: 7373 6962 6c65 206d 6f64 656c 732c 2063  ssible models, c
+0001bbd0: 616c 6375 6c61 7465 206d 6f64 656c 2076  alculate model v
+0001bbe0: 616c 7565 730a 2020 2020 2020 2020 2320  alues.        # 
+0001bbf0: 6174 2072 616e 6765 206f 6620 7465 6d70  at range of temp
+0001bc00: 6572 6174 7572 6573 2061 6e64 2070 6c6f  eratures and plo
+0001bc10: 740a 2020 2020 2020 2020 2320 7468 656e  t.        # then
+0001bc20: 2061 6464 2074 6f20 6172 7261 7920 6f66   add to array of
+0001bc30: 2074 6f74 616c 2072 6174 6573 0a20 2020   total rates.   
+0001bc40: 2020 2020 2066 6f72 2063 6f6c 6f72 2c20       for color, 
+0001bc50: 6d6f 6465 6c20 696e 207a 6970 2863 6f6c  model in zip(col
+0001bc60: 6f72 732c 2073 7570 706f 7274 6564 5f6d  ors, supported_m
+0001bc70: 6f64 656c 7329 3a0a 0a20 2020 2020 2020  odels):..       
+0001bc80: 2020 2020 2023 2047 6574 2069 6e69 7469       # Get initi
+0001bc90: 616c 2076 616c 7565 730a 2020 2020 2020  al values.      
+0001bca0: 2020 2020 2020 696e 6974 6961 6c73 203d        initials =
+0001bcb0: 206d 6f64 656c 2e73 6574 5f69 6e69 7469   model.set_initi
+0001bcc0: 616c 5f76 616c 7328 0a20 2020 2020 2020  al_vals(.       
+0001bcd0: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
+0001bce0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0001bcf0: 6172 3a20 7365 6c66 2e64 6566 6175 6c74  ar: self.default
+0001bd00: 735b 6d6f 6465 6c2e 4e41 4d45 5d5b 7061  s[model.NAME][pa
+0001bd10: 725d 5b27 7661 6c69 6e69 7427 5d0a 2020  r]['valinit'].  
+0001bd20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bd30: 2020 666f 7220 7061 7220 696e 206d 6f64    for par in mod
+0001bd40: 656c 2e50 4152 4e41 4d45 530a 2020 2020  el.PARNAMES.    
+0001bd50: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+0001bd60: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+0001bd70: 2020 2020 2020 2020 2320 4361 6c63 756c          # Calcul
+0001bd80: 6174 6520 7261 7465 730a 2020 2020 2020  ate rates.      
+0001bd90: 2020 2020 2020 7261 7465 7320 3d20 3130        rates = 10
+0001bda0: 2a2a 286d 6f64 656c 2e6d 6f64 656c 2869  **(model.model(i
+0001bdb0: 6e69 7469 616c 732c 2073 656c 662e 7465  nitials, self.te
+0001bdc0: 6d70 5f67 7269 6429 290a 2020 2020 2020  mp_grid)).      
+0001bdd0: 2020 2020 2020 2320 616e 6420 6164 6420        # and add 
+0001bde0: 746f 2074 6f74 616c 206f 6620 616c 6c20  to total of all 
+0001bdf0: 6d6f 6465 6c73 0a20 2020 2020 2020 2020  models.         
+0001be00: 2020 2074 6f74 616c 5f72 6174 6573 202b     total_rates +
+0001be10: 3d20 7261 7465 730a 2020 2020 2020 2020  = rates.        
+0001be20: 2020 2020 2320 506c 6f74 2074 6869 7320      # Plot this 
+0001be30: 6d6f 6465 6c0a 2020 2020 2020 2020 2020  model.          
+0001be40: 2020 5f70 6c6f 7420 3d20 7365 6c66 2e70    _plot = self.p
+0001be50: 6c6f 745f 7769 6467 6574 2e70 6c6f 7428  lot_widget.plot(
+0001be60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001be70: 2073 656c 662e 7465 6d70 5f67 7269 642c   self.temp_grid,
+0001be80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001be90: 2072 6174 6573 2c0a 2020 2020 2020 2020   rates,.        
+0001bea0: 2020 2020 2020 2020 7065 6e3d 7b27 7769          pen={'wi
+0001beb0: 6474 6827 3a20 322e 352c 2027 636f 6c6f  dth': 2.5, 'colo
+0001bec0: 7227 3a20 636f 6c6f 722c 2027 7374 796c  r': color, 'styl
+0001bed0: 6527 3a20 5174 436f 7265 2e51 742e 4461  e': QtCore.Qt.Da
+0001bee0: 7368 4c69 6e65 7d0a 2020 2020 2020 2020  shLine}.        
+0001bef0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+0001bf00: 2020 2320 616e 6420 7374 6f72 6520 696e    # and store in
+0001bf10: 2064 6963 7420 6f66 2061 6c6c 2070 6c6f   dict of all plo
+0001bf20: 7473 0a20 2020 2020 2020 2020 2020 2073  ts.            s
+0001bf30: 656c 662e 6d6f 6465 6c5f 706c 6f74 735b  elf.model_plots[
+0001bf40: 6d6f 6465 6c2e 4e41 4d45 2e6c 6f77 6572  model.NAME.lower
+0001bf50: 2829 5d20 3d20 5f70 6c6f 740a 2020 2020  ()] = _plot.    
+0001bf60: 2020 2020 2020 2020 2320 5265 6d6f 7665          # Remove
+0001bf70: 2066 726f 6d20 6163 7475 616c 2070 6c6f   from actual plo
+0001bf80: 7420 7769 6467 6574 0a20 2020 2020 2020  t widget.       
+0001bf90: 2020 2020 2023 2073 696e 6365 206e 6f20       # since no 
+0001bfa0: 6d6f 6465 6c73 2061 7265 2076 6973 6962  models are visib
+0001bfb0: 6c65 2069 6e69 7469 616c 6c79 0a20 2020  le initially.   
+0001bfc0: 2020 2020 2020 2020 2023 2050 6c6f 7473           # Plots
+0001bfd0: 2061 7265 2072 652d 6164 6465 6420 7769   are re-added wi
+0001bfe0: 7468 206d 6f64 656c 2063 6865 636b 626f  th model checkbo
+0001bff0: 7865 730a 2020 2020 2020 2020 2020 2020  xes.            
+0001c000: 7365 6c66 2e70 6c6f 745f 7769 6467 6574  self.plot_widget
+0001c010: 2e72 656d 6f76 6549 7465 6d28 5f70 6c6f  .removeItem(_plo
+0001c020: 7429 0a0a 2020 2020 2020 2020 2320 506c  t)..        # Pl
+0001c030: 6f74 2073 756d 206f 6620 616c 6c20 6d6f  ot sum of all mo
+0001c040: 6465 6c73 0a20 2020 2020 2020 2073 656c  dels.        sel
+0001c050: 662e 746f 7420 3d20 7365 6c66 2e70 6c6f  f.tot = self.plo
+0001c060: 745f 7769 6467 6574 2e70 6c6f 7428 0a20  t_widget.plot(. 
+0001c070: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0001c080: 7465 6d70 5f67 7269 642c 0a20 2020 2020  temp_grid,.     
+0001c090: 2020 2020 2020 2074 6f74 616c 5f72 6174         total_rat
+0001c0a0: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
+0001c0b0: 7065 6e3d 7b27 7769 6474 6827 3a20 322e  pen={'width': 2.
+0001c0c0: 352c 2027 636f 6c6f 7227 3a20 2772 6564  5, 'color': 'red
+0001c0d0: 277d 0a20 2020 2020 2020 2029 0a20 2020  '}.        ).   
+0001c0e0: 2020 2020 2073 656c 662e 706c 6f74 5f77       self.plot_w
+0001c0f0: 6964 6765 742e 7265 6d6f 7665 4974 656d  idget.removeItem
+0001c100: 2873 656c 662e 746f 7429 0a0a 2020 2020  (self.tot)..    
+0001c110: 2020 2020 2320 5374 6f72 6167 6520 6f62      # Storage ob
+0001c120: 6a65 6374 2066 6f72 2066 696e 616c 2070  ject for final p
+0001c130: 6172 616d 6574 6572 2076 616c 7565 730a  arameter values.
+0001c140: 2020 2020 2020 2020 2320 5365 7420 616c          # Set al
+0001c150: 6c20 696e 6974 6961 6c20 7661 6c75 6573  l initial values
+0001c160: 2064 6566 6175 6c74 730a 2020 2020 2020   defaults.      
+0001c170: 2020 7365 6c66 2e70 6172 7374 6f72 6520    self.parstore 
+0001c180: 3d20 7479 7065 280a 2020 2020 2020 2020  = type(.        
+0001c190: 2020 2020 276f 626a 272c 0a20 2020 2020      'obj',.     
+0001c1a0: 2020 2020 2020 2028 6f62 6a65 6374 2c29         (object,)
+0001c1b0: 2c0a 2020 2020 2020 2020 2020 2020 7b0a  ,.            {.
+0001c1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c1d0: 7061 723a 2073 656c 662e 6465 6661 756c  par: self.defaul
+0001c1e0: 7473 5b6d 6f64 656c 2e4e 414d 455d 5b70  ts[model.NAME][p
+0001c1f0: 6172 5d5b 2776 616c 696e 6974 275d 0a20  ar]['valinit']. 
+0001c200: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0001c210: 6f72 206d 6f64 656c 2069 6e20 7375 7070  or model in supp
+0001c220: 6f72 7465 645f 6d6f 6465 6c73 0a20 2020  orted_models.   
+0001c230: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+0001c240: 2070 6172 2069 6e20 6d6f 6465 6c2e 5041   par in model.PA
+0001c250: 524e 414d 4553 0a20 2020 2020 2020 2020  RNAMES.         
+0001c260: 2020 207d 0a20 2020 2020 2020 2029 0a0a     }.        )..
+0001c270: 2020 2020 2020 2020 2320 436f 6e76 6572          # Conver
+0001c280: 7420 6c6f 6720 7465 6d70 6572 6174 7572  t log temperatur
+0001c290: 6520 7469 636b 7320 746f 206c 696e 6561  e ticks to linea
+0001c2a0: 720a 2020 2020 2020 2020 6178 203d 2073  r.        ax = s
+0001c2b0: 656c 662e 706c 6f74 5f77 6964 6765 742e  elf.plot_widget.
+0001c2c0: 6765 7441 7869 7328 2762 6f74 746f 6d27  getAxis('bottom'
+0001c2d0: 290a 2020 2020 2020 2020 6775 692e 636f  ).        gui.co
+0001c2e0: 6e76 6572 745f 6c6f 675f 7469 636b 735f  nvert_log_ticks_
+0001c2f0: 746f 5f6c 696e 2861 782c 206e 702e 6c6f  to_lin(ax, np.lo
+0001c300: 6731 3028 785f 7661 6c73 2929 0a0a 2020  g10(x_vals))..  
+0001c310: 2020 2020 2020 2320 5248 5320 636f 6c75        # RHS colu
+0001c320: 6d6e 206f 6620 7769 6e64 6f77 0a20 2020  mn of window.   
+0001c330: 2020 2020 2023 2054 6869 7320 636f 6e74       # This cont
+0001c340: 6169 6e73 2065 6163 6820 6d6f 6465 6c20  ains each model 
+0001c350: 616e 6420 6974 7320 6173 736f 6369 6174  and its associat
+0001c360: 6564 2070 6172 616d 6574 6572 730a 2020  ed parameters.  
+0001c370: 2020 2020 2020 2320 4561 6368 2070 6172        # Each par
+0001c380: 616d 6574 6572 2069 7320 636f 6e74 726f  ameter is contro
+0001c390: 6c6c 6564 2062 7920 610a 2020 2020 2020  lled by a.      
+0001c3a0: 2020 2320 736c 6964 6572 732c 2054 6578    # sliders, Tex
+0001c3b0: 7420 656e 7472 792c 2061 6e64 2061 2066  t entry, and a f
+0001c3c0: 6974 2f66 6978 2074 6f67 676c 650a 2020  it/fix toggle.  
+0001c3d0: 2020 2020 2020 636f 6e74 6169 6e65 725f        container_
+0001c3e0: 6c61 796f 7574 203d 2051 7457 6964 6765  layout = QtWidge
+0001c3f0: 7473 2e51 5642 6f78 4c61 796f 7574 2873  ts.QVBoxLayout(s
+0001c400: 6372 6f6c 6c5f 636f 6e74 6169 6e65 7229  croll_container)
+0001c410: 0a0a 2020 2020 2020 2020 2320 4c69 7374  ..        # List
+0001c420: 206f 6620 6e75 6d62 6572 206b 6579 2073   of number key s
+0001c430: 686f 7274 6375 7473 2074 6f20 746f 6767  hortcuts to togg
+0001c440: 6c65 206d 6f64 656c 730a 2020 2020 2020  le models.      
+0001c450: 2020 7365 6c66 2e6f 6e5f 6f66 665f 7368    self.on_off_sh
+0001c460: 6f72 7463 7574 203d 205b 5d0a 0a20 2020  ortcut = []..   
+0001c470: 2020 2020 2023 2046 6f72 2065 6163 6820       # For each 
+0001c480: 6d6f 6465 6c2c 206d 616b 6520 6120 626f  model, make a bo
+0001c490: 7820 746f 2063 6f6e 7461 696e 2061 6c6c  x to contain all
+0001c4a0: 2070 6172 616d 6574 6572 730a 2020 2020   parameters.    
+0001c4b0: 2020 2020 2320 616e 6420 706f 7075 6c61      # and popula
+0001c4c0: 7465 2077 6974 6820 7061 7261 6d65 7465  te with paramete
+0001c4d0: 7273 0a20 2020 2020 2020 2066 6f72 206d  rs.        for m
+0001c4e0: 6974 2c20 6d6f 6465 6c20 696e 2065 6e75  it, model in enu
+0001c4f0: 6d65 7261 7465 2873 7570 706f 7274 6564  merate(supported
+0001c500: 5f6d 6f64 656c 7329 3a0a 2020 2020 2020  _models):.      
+0001c510: 2020 2020 2020 6d6f 6465 6c5f 7769 6467        model_widg
+0001c520: 6574 203d 2073 656c 662e 6d61 6b65 5f6d  et = self.make_m
+0001c530: 6f64 656c 626f 7828 6d6f 6465 6c2c 2073  odelbox(model, s
+0001c540: 6372 6f6c 6c5f 636f 6e74 6169 6e65 722c  croll_container,
+0001c550: 206d 6974 202b 2031 290a 0a20 2020 2020   mit + 1)..     
+0001c560: 2020 2020 2020 2023 2041 6464 2074 6869         # Add thi
+0001c570: 7320 6d6f 6465 6c20 746f 2074 6865 2072  s model to the r
+0001c580: 6967 6874 2068 616e 6420 7369 6465 206f  ight hand side o
+0001c590: 6620 7468 6520 7769 6e64 6f77 0a20 2020  f the window.   
+0001c5a0: 2020 2020 2020 2020 2063 6f6e 7461 696e           contain
+0001c5b0: 6572 5f6c 6179 6f75 742e 6164 6457 6964  er_layout.addWid
+0001c5c0: 6765 7428 6d6f 6465 6c5f 7769 6467 6574  get(model_widget
+0001c5d0: 2c20 6c65 6e28 6d6f 6465 6c2e 5041 524e  , len(model.PARN
+0001c5e0: 414d 4553 2929 0a0a 2020 2020 2020 2020  AMES))..        
+0001c5f0: 2320 4469 7361 626c 6520 6576 6572 7920  # Disable every 
+0001c600: 736c 6964 6572 2c20 656e 7472 792c 2061  slider, entry, a
+0001c610: 6e64 2066 6974 2f66 6978 2062 7920 6465  nd fit/fix by de
+0001c620: 6661 756c 740a 2020 2020 2020 2020 2320  fault.        # 
+0001c630: 5468 6973 2069 7320 746f 6767 6c65 6420  This is toggled 
+0001c640: 6279 2074 6865 206d 6f64 656c 2063 6865  by the model che
+0001c650: 636b 626f 7865 730a 2020 2020 2020 2020  ckboxes.        
+0001c660: 666f 7220 6d6f 6465 6c20 696e 2073 7570  for model in sup
+0001c670: 706f 7274 6564 5f6d 6f64 656c 733a 0a20  ported_models:. 
+0001c680: 2020 2020 2020 2020 2020 206d 6f64 656c             model
+0001c690: 6e61 6d65 203d 206d 6f64 656c 2e4e 414d  name = model.NAM
+0001c6a0: 452e 6c6f 7765 7228 290a 2020 2020 2020  E.lower().      
+0001c6b0: 2020 2020 2020 666f 7220 7061 726e 616d        for parnam
+0001c6c0: 6520 696e 206d 6f64 656c 2e50 4152 4e41  e in model.PARNA
+0001c6d0: 4d45 533a 0a20 2020 2020 2020 2020 2020  MES:.           
+0001c6e0: 2020 2020 2073 656c 662e 7769 6467 6574       self.widget
+0001c6f0: 6469 6374 5b6d 6f64 656c 6e61 6d65 5d5b  dict[modelname][
+0001c700: 7061 726e 616d 655d 5b27 736c 6964 6572  parname]['slider
+0001c710: 275d 2e73 6574 456e 6162 6c65 6428 4661  '].setEnabled(Fa
+0001c720: 6c73 6529 0a20 2020 2020 2020 2020 2020  lse).           
+0001c730: 2020 2020 2073 656c 662e 7769 6467 6574       self.widget
+0001c740: 6469 6374 5b6d 6f64 656c 6e61 6d65 5d5b  dict[modelname][
+0001c750: 7061 726e 616d 655d 5b27 656e 7472 7927  parname]['entry'
+0001c760: 5d2e 7365 7445 6e61 626c 6564 2846 616c  ].setEnabled(Fal
+0001c770: 7365 290a 2020 2020 2020 2020 2020 2020  se).            
+0001c780: 2020 2020 7365 6c66 2e77 6964 6765 7464      self.widgetd
+0001c790: 6963 745b 6d6f 6465 6c6e 616d 655d 5b70  ict[modelname][p
+0001c7a0: 6172 6e61 6d65 5d5b 2766 665f 746f 6767  arname]['ff_togg
+0001c7b0: 6c65 275d 2e73 6574 456e 6162 6c65 6428  le'].setEnabled(
+0001c7c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001c7d0: 2020 2020 2046 616c 7365 0a20 2020 2020       False.     
+0001c7e0: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+0001c7f0: 2020 2020 2020 636f 6e74 6169 6e65 725f        container_
+0001c800: 6c61 796f 7574 2e73 6574 416c 6967 6e6d  layout.setAlignm
+0001c810: 656e 7428 5174 436f 7265 2e51 742e 416c  ent(QtCore.Qt.Al
+0001c820: 6967 6e56 4365 6e74 6572 290a 2020 2020  ignVCenter).    
+0001c830: 2020 2020 7363 726f 6c6c 5f63 6f6e 7461      scroll_conta
+0001c840: 696e 6572 2e73 6574 5369 7a65 506f 6c69  iner.setSizePoli
+0001c850: 6379 280a 2020 2020 2020 2020 2020 2020  cy(.            
+0001c860: 5174 5769 6467 6574 732e 5153 697a 6550  QtWidgets.QSizeP
+0001c870: 6f6c 6963 792e 4d61 7869 6d75 6d2c 0a20  olicy.Maximum,. 
+0001c880: 2020 2020 2020 2020 2020 2051 7457 6964             QtWid
+0001c890: 6765 7473 2e51 5369 7a65 506f 6c69 6379  gets.QSizePolicy
+0001c8a0: 2e4d 6178 696d 756d 0a20 2020 2020 2020  .Maximum.       
+0001c8b0: 2029 0a20 2020 2020 2020 2072 6873 5f63   ).        rhs_c
+0001c8c0: 6f6c 5f73 6372 6f6c 6c2e 7365 744d 696e  ol_scroll.setMin
+0001c8d0: 696d 756d 4865 6967 6874 2835 3735 290a  imumHeight(575).
+0001c8e0: 0a20 2020 2020 2020 2023 2054 6f70 2072  .        # Top r
+0001c8f0: 6f77 0a20 2020 2020 2020 2023 204c 4853  ow.        # LHS
+0001c900: 2070 6c6f 742c 2052 4853 2053 6c69 6465   plot, RHS Slide
+0001c910: 7273 2c20 7465 7874 2c20 6c61 6265 6c73  rs, text, labels
+0001c920: 0a20 2020 2020 2020 2074 6f70 5f72 6f77  .        top_row
+0001c930: 5f6c 6179 6f75 7420 3d20 5174 5769 6467  _layout = QtWidg
+0001c940: 6574 732e 5148 426f 784c 6179 6f75 7428  ets.QHBoxLayout(
+0001c950: 746f 705f 726f 775f 7769 6467 6574 290a  top_row_widget).
+0001c960: 2020 2020 2020 2020 746f 705f 726f 775f          top_row_
+0001c970: 6c61 796f 7574 2e61 6464 5769 6467 6574  layout.addWidget
+0001c980: 286c 6873 5f63 6f6c 5f77 6964 6765 742c  (lhs_col_widget,
+0001c990: 2033 290a 2020 2020 2020 2020 746f 705f   3).        top_
+0001c9a0: 726f 775f 6c61 796f 7574 2e61 6464 5769  row_layout.addWi
+0001c9b0: 6467 6574 2872 6873 5f63 6f6c 5f77 6964  dget(rhs_col_wid
+0001c9c0: 6765 742c 2032 290a 0a20 2020 2020 2020  get, 2)..       
+0001c9d0: 2023 2042 6f74 746f 6d20 726f 770a 2020   # Bottom row.  
+0001c9e0: 2020 2020 2020 2320 4275 7474 6f6e 7320        # Buttons 
+0001c9f0: 666f 7220 7265 7365 7420 616e 6420 6669  for reset and fi
+0001ca00: 740a 2020 2020 2020 2020 7365 6c66 2e66  t.        self.f
+0001ca10: 6974 5f62 746e 5f77 6964 6765 7420 3d20  it_btn_widget = 
+0001ca20: 5174 5769 6467 6574 732e 5150 7573 6842  QtWidgets.QPushB
+0001ca30: 7574 746f 6e28 0a20 2020 2020 2020 2020  utton(.         
+0001ca40: 2020 2070 6172 656e 743d 626f 745f 726f     parent=bot_ro
+0001ca50: 775f 7769 6467 6574 2c0a 2020 2020 2020  w_widget,.      
+0001ca60: 2020 2020 2020 7465 7874 3d27 4669 7427        text='Fit'
+0001ca70: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+0001ca80: 2020 2073 656c 662e 6669 745f 6274 6e5f     self.fit_btn_
+0001ca90: 7769 6467 6574 2e73 6574 5374 796c 6553  widget.setStyleS
+0001caa0: 6865 6574 2827 666f 6e74 2d77 6569 6768  heet('font-weigh
+0001cab0: 743a 2062 6f6c 643b 2729 0a0a 2020 2020  t: bold;')..    
+0001cac0: 2020 2020 7365 6c66 2e66 6974 5f62 746e      self.fit_btn
+0001cad0: 5f77 6964 6765 742e 7365 7445 6e61 626c  _widget.setEnabl
+0001cae0: 6564 2846 616c 7365 290a 2020 2020 2020  ed(False).      
+0001caf0: 2020 7365 6c66 2e66 6974 5f62 746e 5f77    self.fit_btn_w
+0001cb00: 6964 6765 742e 636c 6963 6b65 642e 636f  idget.clicked.co
+0001cb10: 6e6e 6563 7428 7365 6c66 2e66 6974 290a  nnect(self.fit).
+0001cb20: 2020 2020 2020 2020 7365 6c66 2e66 6974          self.fit
+0001cb30: 5f62 746e 5f77 6964 6765 742e 7365 7453  _btn_widget.setS
+0001cb40: 697a 6550 6f6c 6963 7928 0a20 2020 2020  izePolicy(.     
+0001cb50: 2020 2020 2020 2051 7457 6964 6765 7473         QtWidgets
+0001cb60: 2e51 5369 7a65 506f 6c69 6379 2e46 6978  .QSizePolicy.Fix
+0001cb70: 6564 2c0a 2020 2020 2020 2020 2020 2020  ed,.            
+0001cb80: 5174 5769 6467 6574 732e 5153 697a 6550  QtWidgets.QSizeP
+0001cb90: 6f6c 6963 792e 4669 7865 640a 2020 2020  olicy.Fixed.    
+0001cba0: 2020 2020 290a 2020 2020 2020 2020 7265      ).        re
+0001cbb0: 7365 745f 6274 6e5f 7769 6467 6574 203d  set_btn_widget =
+0001cbc0: 2051 7457 6964 6765 7473 2e51 5075 7368   QtWidgets.QPush
+0001cbd0: 4275 7474 6f6e 280a 2020 2020 2020 2020  Button(.        
+0001cbe0: 2020 2020 7061 7265 6e74 3d62 6f74 5f72      parent=bot_r
+0001cbf0: 6f77 5f77 6964 6765 742c 0a20 2020 2020  ow_widget,.     
+0001cc00: 2020 2020 2020 2074 6578 743d 2752 6573         text='Res
+0001cc10: 6574 272c 0a20 2020 2020 2020 2029 0a20  et',.        ). 
+0001cc20: 2020 2020 2020 2072 6573 6574 5f62 746e         reset_btn
+0001cc30: 5f77 6964 6765 742e 7365 7453 7479 6c65  _widget.setStyle
+0001cc40: 5368 6565 7428 2766 6f6e 742d 7765 6967  Sheet('font-weig
+0001cc50: 6874 3a20 626f 6c64 3b27 290a 2020 2020  ht: bold;').    
+0001cc60: 2020 2020 7265 7365 745f 6274 6e5f 7769      reset_btn_wi
+0001cc70: 6467 6574 2e63 6c69 636b 6564 2e63 6f6e  dget.clicked.con
+0001cc80: 6e65 6374 2873 656c 662e 7265 7365 7429  nect(self.reset)
+0001cc90: 0a20 2020 2020 2020 2072 6573 6574 5f62  .        reset_b
+0001cca0: 746e 5f77 6964 6765 742e 7365 7453 697a  tn_widget.setSiz
+0001ccb0: 6550 6f6c 6963 7928 0a20 2020 2020 2020  ePolicy(.       
+0001ccc0: 2020 2020 2051 7457 6964 6765 7473 2e51       QtWidgets.Q
+0001ccd0: 5369 7a65 506f 6c69 6379 2e46 6978 6564  SizePolicy.Fixed
+0001cce0: 2c0a 2020 2020 2020 2020 2020 2020 5174  ,.            Qt
+0001ccf0: 5769 6467 6574 732e 5153 697a 6550 6f6c  Widgets.QSizePol
+0001cd00: 6963 792e 4669 7865 640a 2020 2020 2020  icy.Fixed.      
+0001cd10: 2020 290a 0a20 2020 2020 2020 2023 204d    )..        # M
+0001cd20: 6f64 6966 7920 6669 7420 616e 6420 7265  odify fit and re
+0001cd30: 7365 7420 6275 7474 6f6e 2074 6578 7420  set button text 
+0001cd40: 636f 6c6f 7273 2074 6f20 6c6f 6f6b 2067  colors to look g
+0001cd50: 6f6f 6420 6576 656e 0a20 2020 2020 2020  ood even.       
+0001cd60: 2023 2069 6e20 4d61 634f 5320 6461 726b   # in MacOS dark
+0001cd70: 6d6f 6465 2e0a 2020 2020 2020 2020 7061  mode..        pa
+0001cd80: 6c65 7474 6520 3d20 5174 4775 692e 5150  lette = QtGui.QP
+0001cd90: 616c 6574 7465 2873 656c 662e 6669 745f  alette(self.fit_
+0001cda0: 6274 6e5f 7769 6467 6574 2e70 616c 6574  btn_widget.palet
+0001cdb0: 7465 2829 290a 2020 2020 2020 2020 7061  te()).        pa
+0001cdc0: 6c65 7474 652e 7365 7443 6f6c 6f72 2851  lette.setColor(Q
+0001cdd0: 7447 7569 2e51 5061 6c65 7474 652e 4275  tGui.QPalette.Bu
+0001cde0: 7474 6f6e 5465 7874 2c20 5174 4775 692e  ttonText, QtGui.
+0001cdf0: 5143 6f6c 6f72 2827 2330 6462 3237 3327  QColor('#0db273'
+0001ce00: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+0001ce10: 6669 745f 6274 6e5f 7769 6467 6574 2e73  fit_btn_widget.s
+0001ce20: 6574 5061 6c65 7474 6528 7061 6c65 7474  etPalette(palett
+0001ce30: 6529 0a20 2020 2020 2020 2070 616c 6574  e).        palet
+0001ce40: 7465 2e73 6574 436f 6c6f 7228 5174 4775  te.setColor(QtGu
+0001ce50: 692e 5150 616c 6574 7465 2e42 7574 746f  i.QPalette.Butto
+0001ce60: 6e54 6578 742c 2051 7447 7569 2e51 436f  nText, QtGui.QCo
+0001ce70: 6c6f 7228 2723 3462 3661 6164 2729 290a  lor('#4b6aad')).
+0001ce80: 2020 2020 2020 2020 7265 7365 745f 6274          reset_bt
+0001ce90: 6e5f 7769 6467 6574 2e73 6574 5061 6c65  n_widget.setPale
+0001cea0: 7474 6528 7061 6c65 7474 6529 0a0a 2020  tte(palette)..  
+0001ceb0: 2020 2020 2020 2320 4b65 7962 6f61 7264        # Keyboard
+0001cec0: 2073 686f 7274 6375 742c 2070 7265 7373   shortcut, press
+0001ced0: 2066 2074 6f20 6669 7420 6966 2066 6974   f to fit if fit
+0001cee0: 2062 7574 746f 6e20 6e6f 7420 6772 6579   button not grey
+0001cef0: 6564 206f 7574 0a20 2020 2020 2020 2073  ed out.        s
+0001cf00: 656c 662e 6669 745f 7368 6f72 7463 7574  elf.fit_shortcut
+0001cf10: 203d 2051 7457 6964 6765 7473 2e51 5368   = QtWidgets.QSh
+0001cf20: 6f72 7463 7574 2851 7447 7569 2e51 4b65  ortcut(QtGui.QKe
+0001cf30: 7953 6571 7565 6e63 6528 2766 2729 2c20  ySequence('f'), 
+0001cf40: 7365 6c66 290a 2020 2020 2020 2020 7365  self).        se
+0001cf50: 6c66 2e66 6974 5f73 686f 7274 6375 742e  lf.fit_shortcut.
+0001cf60: 6163 7469 7661 7465 642e 636f 6e6e 6563  activated.connec
+0001cf70: 7428 0a20 2020 2020 2020 2020 2020 206c  t(.            l
+0001cf80: 616d 6264 613a 2073 656c 662e 6b65 7962  ambda: self.keyb
+0001cf90: 6f61 7264 5f66 6974 5f63 616c 6c62 6163  oard_fit_callbac
+0001cfa0: 6b28 290a 2020 2020 2020 2020 290a 0a20  k().        ).. 
+0001cfb0: 2020 2020 2020 2062 6f74 5f72 6f77 5f6c         bot_row_l
+0001cfc0: 6179 6f75 7420 3d20 5174 5769 6467 6574  ayout = QtWidget
+0001cfd0: 732e 5148 426f 784c 6179 6f75 7428 626f  s.QHBoxLayout(bo
+0001cfe0: 745f 726f 775f 7769 6467 6574 290a 2020  t_row_widget).  
+0001cff0: 2020 2020 2020 626f 745f 726f 775f 6c61        bot_row_la
+0001d000: 796f 7574 2e61 6464 5769 6467 6574 2873  yout.addWidget(s
+0001d010: 656c 662e 6669 745f 6274 6e5f 7769 6467  elf.fit_btn_widg
+0001d020: 6574 290a 2020 2020 2020 2020 626f 745f  et).        bot_
+0001d030: 726f 775f 6c61 796f 7574 2e61 6464 5769  row_layout.addWi
+0001d040: 6467 6574 2872 6573 6574 5f62 746e 5f77  dget(reset_btn_w
+0001d050: 6964 6765 7429 0a0a 2020 2020 2020 2020  idget)..        
+0001d060: 2320 4f76 6572 616c 6c20 6170 700a 2020  # Overall app.  
+0001d070: 2020 2020 2020 2320 546f 7020 616e 6420        # Top and 
+0001d080: 426f 7474 6f6d 2072 6f77 730a 2020 2020  Bottom rows.    
+0001d090: 2020 2020 6675 6c6c 5f6c 6179 6f75 7420      full_layout 
+0001d0a0: 3d20 5174 5769 6467 6574 732e 5156 426f  = QtWidgets.QVBo
+0001d0b0: 784c 6179 6f75 7428 7365 6c66 2e77 6964  xLayout(self.wid
+0001d0c0: 6765 7429 0a20 2020 2020 2020 2066 756c  get).        ful
+0001d0d0: 6c5f 6c61 796f 7574 2e61 6464 5769 6467  l_layout.addWidg
+0001d0e0: 6574 2874 6f70 5f72 6f77 5f77 6964 6765  et(top_row_widge
+0001d0f0: 7429 0a20 2020 2020 2020 2066 756c 6c5f  t).        full_
+0001d100: 6c61 796f 7574 2e61 6464 5769 6467 6574  layout.addWidget
+0001d110: 2862 6f74 5f72 6f77 5f77 6964 6765 7429  (bot_row_widget)
+0001d120: 0a0a 2020 2020 2020 2020 2320 5365 7420  ..        # Set 
+0001d130: 6c61 796f 7574 0a20 2020 2020 2020 2073  layout.        s
+0001d140: 656c 662e 7769 6467 6574 2e73 6574 4c61  elf.widget.setLa
+0001d150: 796f 7574 2866 756c 6c5f 6c61 796f 7574  yout(full_layout
+0001d160: 290a 2020 2020 2020 2020 7365 6c66 2e77  ).        self.w
+0001d170: 6964 6765 742e 7365 7453 697a 6550 6f6c  idget.setSizePol
+0001d180: 6963 7928 0a20 2020 2020 2020 2020 2020  icy(.           
+0001d190: 2051 7457 6964 6765 7473 2e51 5369 7a65   QtWidgets.QSize
+0001d1a0: 506f 6c69 6379 2e45 7870 616e 6469 6e67  Policy.Expanding
+0001d1b0: 2c0a 2020 2020 2020 2020 2020 2020 5174  ,.            Qt
+0001d1c0: 5769 6467 6574 732e 5153 697a 6550 6f6c  Widgets.QSizePol
+0001d1d0: 6963 792e 4578 7061 6e64 696e 670a 2020  icy.Expanding.  
+0001d1e0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+0001d1f0: 2072 6574 7572 6e0a 0a20 2020 2064 6566   return..    def
+0001d200: 206b 6579 626f 6172 645f 6669 745f 6361   keyboard_fit_ca
+0001d210: 6c6c 6261 636b 2873 656c 6629 3a0a 2020  llback(self):.  
+0001d220: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
+0001d230: 2020 4361 6c6c 6261 636b 2066 6f72 2070    Callback for p
+0001d240: 7265 7373 696e 6720 2766 2720 6b65 792e  ressing 'f' key.
+0001d250: 2052 756e 7320 6669 7420 6275 7474 6f6e   Runs fit button
+0001d260: 2069 6620 6e6f 7420 6772 6579 6564 206f   if not greyed o
+0001d270: 7574 0a20 2020 2020 2020 2027 2727 0a0a  ut.        '''..
+0001d280: 2020 2020 2020 2020 2320 4368 6563 6b20          # Check 
+0001d290: 6669 7420 6275 7474 6f6e 2069 7320 6e6f  fit button is no
+0001d2a0: 7420 6772 6579 6564 206f 7574 0a20 2020  t greyed out.   
+0001d2b0: 2020 2020 2069 6620 7365 6c66 2e66 6974       if self.fit
+0001d2c0: 5f62 746e 5f77 6964 6765 742e 6973 456e  _btn_widget.isEn
+0001d2d0: 6162 6c65 6428 293a 0a20 2020 2020 2020  abled():.       
+0001d2e0: 2020 2020 2023 2052 756e 2066 6974 2063       # Run fit c
+0001d2f0: 6f64 652c 2074 6869 7320 636c 6f73 6573  ode, this closes
+0001d300: 2061 7070 0a20 2020 2020 2020 2020 2020   app.           
+0001d310: 2073 656c 662e 6669 7428 290a 0a20 2020   self.fit()..   
+0001d320: 2020 2020 2072 6574 7572 6e0a 0a20 2020       return..   
+0001d330: 2064 6566 2072 6573 6574 2873 656c 6629   def reset(self)
+0001d340: 3a0a 2020 2020 2020 2020 2727 270a 2020  :.        '''.  
+0001d350: 2020 2020 2020 4361 6c6c 6261 636b 2066        Callback f
+0001d360: 6f72 2052 6573 6574 2062 7574 746f 6e2e  or Reset button.
+0001d370: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+0001d380: 2077 696e 646f 7720 6261 636b 2074 6f20   window back to 
+0001d390: 6f72 6967 696e 616c 206c 6179 6f75 742f  original layout/
+0001d3a0: 7365 6c65 6374 696f 6e73 0a20 2020 2020  selections.     
+0001d3b0: 2020 2027 2727 0a0a 2020 2020 2020 2020     '''..        
+0001d3c0: 2320 466f 7220 6561 6368 206d 6f64 656c  # For each model
+0001d3d0: 2c20 7265 6d6f 7665 2070 6c6f 742c 2061  , remove plot, a
+0001d3e0: 6e64 2072 6573 6574 2070 6172 616d 6574  nd reset paramet
+0001d3f0: 6572 2076 616c 7565 730a 2020 2020 2020  er values.      
+0001d400: 2020 666f 7220 6d6f 6465 6c20 696e 2073    for model in s
+0001d410: 656c 662e 7375 7070 6f72 7465 645f 6d6f  elf.supported_mo
+0001d420: 6465 6c73 3a0a 2020 2020 2020 2020 2020  dels:.          
+0001d430: 2020 6d6f 6465 6c6e 616d 6520 3d20 6d6f    modelname = mo
+0001d440: 6465 6c2e 4e41 4d45 2e6c 6f77 6572 2829  del.NAME.lower()
+0001d450: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+0001d460: 4469 7361 626c 6520 616c 6c20 6d6f 6465  Disable all mode
+0001d470: 6c73 0a20 2020 2020 2020 2020 2020 2073  ls.            s
+0001d480: 656c 662e 7573 656c 2e6d 6f64 656c 735b  elf.usel.models[
+0001d490: 6d6f 6465 6c6e 616d 655d 203d 2046 616c  modelname] = Fal
+0001d4a0: 7365 0a20 2020 2020 2020 2020 2020 2023  se.            #
+0001d4b0: 2061 6e64 2075 6e74 6963 6b20 6368 6563   and untick chec
+0001d4c0: 6b62 6f78 6573 0a20 2020 2020 2020 2020  kboxes.         
+0001d4d0: 2020 2073 656c 662e 7469 636b 6469 6374     self.tickdict
+0001d4e0: 5b6d 6f64 656c 6e61 6d65 5d2e 7365 7443  [modelname].setC
+0001d4f0: 6865 636b 5374 6174 6528 4661 6c73 6529  heckState(False)
+0001d500: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+0001d510: 5265 6d6f 7665 2063 6f72 7265 7370 6f6e  Remove correspon
+0001d520: 6469 6e67 2070 6c6f 740a 2020 2020 2020  ding plot.      
+0001d530: 2020 2020 2020 5f70 6c6f 7420 3d20 7365        _plot = se
+0001d540: 6c66 2e6d 6f64 656c 5f70 6c6f 7473 5b6d  lf.model_plots[m
+0001d550: 6f64 656c 6e61 6d65 5d0a 2020 2020 2020  odelname].      
+0001d560: 2020 2020 2020 7365 6c66 2e70 6c6f 745f        self.plot_
+0001d570: 7769 6467 6574 2e72 656d 6f76 6549 7465  widget.removeIte
+0001d580: 6d28 5f70 6c6f 7429 0a0a 2020 2020 2020  m(_plot)..      
+0001d590: 2020 2020 2020 2320 5265 7365 7420 6561        # Reset ea
+0001d5a0: 6368 2070 6172 616d 6574 6572 2073 6c69  ch parameter sli
+0001d5b0: 6465 722c 2065 6e74 7279 2c20 616e 6420  der, entry, and 
+0001d5c0: 6669 7466 6978 0a20 2020 2020 2020 2020  fitfix.         
+0001d5d0: 2020 2023 2062 6163 6b20 746f 206f 7269     # back to ori
+0001d5e0: 6769 6e61 6c20 7661 6c75 650a 2020 2020  ginal value.    
+0001d5f0: 2020 2020 2020 2020 666f 7220 7061 726e          for parn
+0001d600: 616d 6520 696e 206d 6f64 656c 2e50 4152  ame in model.PAR
+0001d610: 4e41 4d45 533a 0a20 2020 2020 2020 2020  NAMES:.         
+0001d620: 2020 2020 2020 2073 6574 6174 7472 280a         setattr(.
+0001d630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d640: 2020 2020 7365 6c66 2e70 6172 7374 6f72      self.parstor
+0001d650: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+0001d660: 2020 2020 2020 2070 6172 6e61 6d65 2c0a         parname,.
+0001d670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d680: 2020 2020 7365 6c66 2e64 6566 6175 6c74      self.default
+0001d690: 735b 6d6f 6465 6c2e 4e41 4d45 5d5b 7061  s[model.NAME][pa
+0001d6a0: 726e 616d 655d 5b27 7661 6c69 6e69 7427  rname]['valinit'
+0001d6b0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+0001d6c0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+0001d6d0: 2020 2020 7365 6c66 2e77 6964 6765 7464      self.widgetd
+0001d6e0: 6963 745b 6d6f 6465 6c6e 616d 655d 5b70  ict[modelname][p
+0001d6f0: 6172 6e61 6d65 5d5b 2773 6c69 6465 7227  arname]['slider'
+0001d700: 5d2e 7365 7456 616c 7565 280a 2020 2020  ].setValue(.    
+0001d710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d720: 696e 7428 7365 6c66 2e64 6566 6175 6c74  int(self.default
+0001d730: 735b 6d6f 6465 6c2e 4e41 4d45 5d5b 7061  s[model.NAME][pa
+0001d740: 726e 616d 655d 5b27 7661 6c69 6e69 7427  rname]['valinit'
+0001d750: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
+0001d760: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+0001d770: 2020 2020 2073 656c 662e 7769 6467 6574       self.widget
+0001d780: 6469 6374 5b6d 6f64 656c 6e61 6d65 5d5b  dict[modelname][
+0001d790: 7061 726e 616d 655d 5b27 656e 7472 7927  parname]['entry'
+0001d7a0: 5d2e 7365 7456 616c 7565 280a 2020 2020  ].setValue(.    
+0001d7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d7c0: 7365 6c66 2e64 6566 6175 6c74 735b 6d6f  self.defaults[mo
+0001d7d0: 6465 6c2e 4e41 4d45 5d5b 7061 726e 616d  del.NAME][parnam
+0001d7e0: 655d 5b27 7661 6c69 6e69 7427 5d0a 2020  e]['valinit'].  
+0001d7f0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+0001d800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d810: 7365 6c66 2e77 6964 6765 7464 6963 745b  self.widgetdict[
+0001d820: 6d6f 6465 6c6e 616d 655d 5b70 6172 6e61  modelname][parna
+0001d830: 6d65 5d5b 2766 665f 746f 6767 6c65 275d  me]['ff_toggle']
+0001d840: 2e73 6574 5465 7874 280a 2020 2020 2020  .setText(.      
+0001d850: 2020 2020 2020 2020 2020 2020 2020 2746                'F
+0001d860: 7265 6527 0a20 2020 2020 2020 2020 2020  ree'.           
+0001d870: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+0001d880: 2320 5265 6d6f 7665 2074 6f74 616c 206d  # Remove total m
+0001d890: 6f64 656c 2070 6c6f 740a 2020 2020 2020  odel plot.      
+0001d8a0: 2020 7365 6c66 2e70 6c6f 745f 7769 6467    self.plot_widg
+0001d8b0: 6574 2e72 656d 6f76 6549 7465 6d28 7365  et.removeItem(se
+0001d8c0: 6c66 2e74 6f74 290a 0a20 2020 2020 2020  lf.tot)..       
+0001d8d0: 2072 6574 7572 6e0a 0a20 2020 2064 6566   return..    def
+0001d8e0: 2066 6974 2873 656c 6629 3a0a 2020 2020   fit(self):.    
+0001d8f0: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
+0001d900: 4361 6c6c 6261 636b 2066 6f72 2046 6974  Callback for Fit
+0001d910: 2062 7574 746f 6e2e 0a20 2020 2020 2020   button..       
+0001d920: 2043 6f6c 6c65 6374 7320 7661 7269 6162   Collects variab
+0001d930: 6c65 2076 616c 7565 7320 6f66 2065 6163  le values of eac
+0001d940: 6820 6d6f 6465 6c20 616e 6420 6173 7365  h model and asse
+0001d950: 6d62 6c65 7320 696e 746f 2066 6974 2f66  mbles into fit/f
+0001d960: 6978 0a20 2020 2020 2020 2064 6963 7469  ix.        dicti
+0001d970: 6f6e 6172 6965 732c 2074 6865 6e20 636c  onaries, then cl
+0001d980: 6f73 6573 2074 6865 2077 696e 646f 772e  oses the window.
+0001d990: 0a20 2020 2020 2020 2027 2727 0a0a 2020  .        '''..  
+0001d9a0: 2020 2020 2020 6c6e 616d 655f 746f 5f6d        lname_to_m
+0001d9b0: 6f64 656c 203d 207b 0a20 2020 2020 2020  odel = {.       
+0001d9c0: 2020 2020 206d 6f64 656c 2e4e 414d 452e       model.NAME.
+0001d9d0: 6c6f 7765 7228 293a 206d 6f64 656c 0a20  lower(): model. 
+0001d9e0: 2020 2020 2020 2020 2020 2066 6f72 206d             for m
+0001d9f0: 6f64 656c 2069 6e20 7365 6c66 2e73 7570  odel in self.sup
+0001da00: 706f 7274 6564 5f6d 6f64 656c 730a 2020  ported_models.  
+0001da10: 2020 2020 2020 7d0a 0a20 2020 2020 2020        }..       
+0001da20: 2023 2043 6f6c 6c65 6374 2076 6172 6961   # Collect varia
+0001da30: 626c 6573 206f 6620 6561 6368 206d 6f64  bles of each mod
+0001da40: 656c 2c20 6966 2074 6861 7420 6d6f 6465  el, if that mode
+0001da50: 6c20 6973 2065 6e61 626c 6564 0a20 2020  l is enabled.   
+0001da60: 2020 2020 2023 2061 6e64 2061 7373 6967       # and assig
+0001da70: 6e20 746f 2066 6974 206f 7220 6669 780a  n to fit or fix.
+0001da80: 2020 2020 2020 2020 666f 7220 6d6f 6465          for mode
+0001da90: 6c6e 616d 652c 2065 6e61 626c 6564 2069  lname, enabled i
+0001daa0: 6e20 7365 6c66 2e75 7365 6c2e 6d6f 6465  n self.usel.mode
+0001dab0: 6c73 2e69 7465 6d73 2829 3a0a 2020 2020  ls.items():.    
+0001dac0: 2020 2020 2020 2020 5f66 6974 5f76 6172          _fit_var
+0001dad0: 7320 3d20 6469 6374 2829 0a20 2020 2020  s = dict().     
+0001dae0: 2020 2020 2020 205f 6669 785f 7661 7273         _fix_vars
+0001daf0: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
+0001db00: 2020 2020 2020 6966 2065 6e61 626c 6564        if enabled
+0001db10: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001db20: 2020 6d6f 6465 6c20 3d20 6c6e 616d 655f    model = lname_
+0001db30: 746f 5f6d 6f64 656c 5b6d 6f64 656c 6e61  to_model[modelna
+0001db40: 6d65 5d0a 2020 2020 2020 2020 2020 2020  me].            
+0001db50: 2020 2020 666f 7220 6e61 6d65 2069 6e20      for name in 
+0001db60: 6d6f 6465 6c2e 5041 524e 414d 4553 3a0a  model.PARNAMES:.
+0001db70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001db80: 2020 2020 6966 2073 656c 662e 7573 656c      if self.usel
+0001db90: 2e66 6974 5b6e 616d 655d 3a0a 2020 2020  .fit[name]:.    
+0001dba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dbb0: 2020 2020 5f66 6974 5f76 6172 735b 6e61      _fit_vars[na
+0001dbc0: 6d65 5d20 3d20 6765 7461 7474 7228 7365  me] = getattr(se
+0001dbd0: 6c66 2e70 6172 7374 6f72 652c 206e 616d  lf.parstore, nam
+0001dbe0: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
+0001dbf0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0001dc00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dc10: 2020 2020 205f 6669 785f 7661 7273 5b6e       _fix_vars[n
+0001dc20: 616d 655d 203d 2067 6574 6174 7472 2873  ame] = getattr(s
+0001dc30: 656c 662e 7061 7273 746f 7265 2c20 6e61  elf.parstore, na
+0001dc40: 6d65 290a 0a20 2020 2020 2020 2020 2020  me)..           
+0001dc50: 2020 2020 2073 656c 662e 7573 656c 2e66       self.usel.f
+0001dc60: 6974 5f76 6172 732e 6170 7065 6e64 285f  it_vars.append(_
+0001dc70: 6669 745f 7661 7273 290a 2020 2020 2020  fit_vars).      
+0001dc80: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
+0001dc90: 7365 6c2e 6669 785f 7661 7273 2e61 7070  sel.fix_vars.app
+0001dca0: 656e 6428 5f66 6978 5f76 6172 7329 0a0a  end(_fix_vars)..
+0001dcb0: 2020 2020 2020 2020 2320 5365 7420 2768          # Set 'h
+0001dcc0: 6173 2070 726f 6772 616d 2062 6565 6e20  as program been 
+0001dcd0: 6578 6974 6564 2720 666c 6167 2074 6f20  exited' flag to 
+0001dce0: 6661 6c73 650a 2020 2020 2020 2020 7365  false.        se
+0001dcf0: 6c66 2e75 7365 6c2e 6578 6974 6564 203d  lf.usel.exited =
+0001dd00: 2046 616c 7365 0a0a 2020 2020 2020 2020   False..        
+0001dd10: 2320 436c 6f73 6520 7468 6520 7769 6e64  # Close the wind
+0001dd20: 6f77 0a20 2020 2020 2020 2073 656c 662e  ow.        self.
+0001dd30: 636c 6f73 6528 290a 2020 2020 2020 2020  close().        
+0001dd40: 7265 7475 726e 0a0a 2020 2020 6465 6620  return..    def 
+0001dd50: 7570 6461 7465 5f6d 6f64 656c 706c 6f74  update_modelplot
+0001dd60: 2873 656c 662c 2076 616c 7565 2c20 7061  (self, value, pa
+0001dd70: 726e 616d 652c 206d 6f64 656c 3a20 4c6f  rname, model: Lo
+0001dd80: 6754 6175 544d 6f64 656c 293a 0a0a 2020  gTauTModel):..  
+0001dd90: 2020 2020 2020 2320 5365 7420 6e65 7720        # Set new 
+0001dda0: 7061 7261 6d65 7465 7220 7661 6c75 650a  parameter value.
+0001ddb0: 2020 2020 2020 2020 7365 7461 7474 7228          setattr(
+0001ddc0: 7365 6c66 2e70 6172 7374 6f72 652c 2070  self.parstore, p
+0001ddd0: 6172 6e61 6d65 2c20 666c 6f61 7428 7661  arname, float(va
+0001dde0: 6c75 6529 290a 0a20 2020 2020 2020 2070  lue))..        p
+0001ddf0: 6172 616d 6574 6572 7320 3d20 6d6f 6465  arameters = mode
+0001de00: 6c2e 7365 745f 696e 6974 6961 6c5f 7661  l.set_initial_va
+0001de10: 6c73 280a 2020 2020 2020 2020 2020 2020  ls(.            
+0001de20: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+0001de30: 2020 7061 726e 616d 653a 2067 6574 6174    parname: getat
+0001de40: 7472 2873 656c 662e 7061 7273 746f 7265  tr(self.parstore
+0001de50: 2c20 7061 726e 616d 6529 0a20 2020 2020  , parname).     
+0001de60: 2020 2020 2020 2020 2020 2066 6f72 2070             for p
+0001de70: 6172 6e61 6d65 2069 6e20 6d6f 6465 6c2e  arname in model.
+0001de80: 5041 524e 414d 4553 0a20 2020 2020 2020  PARNAMES.       
+0001de90: 2020 2020 207d 0a20 2020 2020 2020 2029       }.        )
+0001dea0: 0a0a 2020 2020 2020 2020 6e65 775f 7261  ..        new_ra
+0001deb0: 7465 7320 3d20 3130 2a2a 6d6f 6465 6c2e  tes = 10**model.
+0001dec0: 6d6f 6465 6c28 7061 7261 6d65 7465 7273  model(parameters
+0001ded0: 2c20 7365 6c66 2e74 656d 705f 6772 6964  , self.temp_grid
+0001dee0: 290a 0a20 2020 2020 2020 205f 706c 6f74  )..        _plot
+0001def0: 203d 2073 656c 662e 6d6f 6465 6c5f 706c   = self.model_pl
+0001df00: 6f74 735b 6d6f 6465 6c2e 4e41 4d45 2e6c  ots[model.NAME.l
+0001df10: 6f77 6572 2829 5d0a 2020 2020 2020 2020  ower()].        
+0001df20: 5f70 6c6f 742e 7365 7444 6174 6128 7365  _plot.setData(se
+0001df30: 6c66 2e74 656d 705f 6772 6964 2c20 6e65  lf.temp_grid, ne
+0001df40: 775f 7261 7465 7329 0a0a 2020 2020 2020  w_rates)..      
+0001df50: 2020 2320 5570 6461 7465 2074 6f74 616c    # Update total
+0001df60: 2070 6c6f 7420 6173 2073 756d 206f 6620   plot as sum of 
+0001df70: 616c 6c20 6d6f 6465 6c73 0a20 2020 2020  all models.     
+0001df80: 2020 2023 2075 7365 2079 6461 7461 206f     # use ydata o
+0001df90: 6620 6561 6368 206d 6f64 656c 0a20 2020  f each model.   
+0001dfa0: 2020 2020 2074 6f74 616c 5f72 6174 6573       total_rates
+0001dfb0: 203d 206e 702e 7a65 726f 7328 7365 6c66   = np.zeros(self
+0001dfc0: 2e74 656d 705f 6772 6964 2e73 6861 7065  .temp_grid.shape
+0001dfd0: 290a 2020 2020 2020 2020 746f 7461 6c5f  ).        total_
+0001dfe0: 7261 7465 7320 2b3d 206e 702e 7375 6d28  rates += np.sum(
+0001dff0: 0a20 2020 2020 2020 2020 2020 205b 0a20  .            [. 
+0001e000: 2020 2020 2020 2020 2020 2020 2020 205f                 _
+0001e010: 706c 6f74 2e79 4461 7461 0a20 2020 2020  plot.yData.     
+0001e020: 2020 2020 2020 2020 2020 2066 6f72 206e             for n
+0001e030: 616d 652c 205f 706c 6f74 2069 6e20 7365  ame, _plot in se
+0001e040: 6c66 2e6d 6f64 656c 5f70 6c6f 7473 2e69  lf.model_plots.i
+0001e050: 7465 6d73 2829 0a20 2020 2020 2020 2020  tems().         
+0001e060: 2020 2020 2020 2069 6620 7365 6c66 2e75         if self.u
+0001e070: 7365 6c2e 6d6f 6465 6c73 5b6e 616d 655d  sel.models[name]
+0001e080: 0a20 2020 2020 2020 2020 2020 205d 2c0a  .            ],.
+0001e090: 2020 2020 2020 2020 2020 2020 6178 6973              axis
+0001e0a0: 3d30 0a20 2020 2020 2020 2029 0a20 2020  =0.        ).   
+0001e0b0: 2020 2020 2073 656c 662e 746f 742e 7365       self.tot.se
+0001e0c0: 7444 6174 6128 7365 6c66 2e74 656d 705f  tData(self.temp_
+0001e0d0: 6772 6964 2c20 746f 7461 6c5f 7261 7465  grid, total_rate
+0001e0e0: 7329 0a0a 2020 2020 2020 2020 7265 7475  s)..        retu
+0001e0f0: 726e 0a0a 2020 2020 6465 6620 746f 6767  rn..    def togg
+0001e100: 6c65 5f70 6c6f 7428 7365 6c66 2c20 7661  le_plot(self, va
+0001e110: 6c3a 2069 6e74 2c0a 2020 2020 2020 2020  l: int,.        
+0001e120: 2020 2020 2020 2020 2020 2020 6d6f 6465              mode
+0001e130: 6c3a 204c 6f67 5461 7554 4d6f 6465 6c20  l: LogTauTModel 
+0001e140: 7c20 4c6f 6754 6175 484d 6f64 656c 2920  | LogTauHModel) 
+0001e150: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+0001e160: 2027 2727 0a20 2020 2020 2020 2043 616c   '''.        Cal
+0001e170: 6c62 6163 6b20 666f 7220 746f 6767 6c69  lback for toggli
+0001e180: 6e67 206d 6f64 656c 2063 6865 636b 626f  ng model checkbo
+0001e190: 7865 730a 0a20 2020 2020 2020 2043 616c  xes..        Cal
+0001e1a0: 6375 6c61 7465 7320 6d6f 6465 6c20 6461  culates model da
+0001e1b0: 7461 2c20 6164 6473 2f64 656c 6574 6573  ta, adds/deletes
+0001e1c0: 206c 696e 6520 6672 6f6d 2070 6c6f 740a   line from plot.
+0001e1d0: 2020 2020 2020 2020 616e 6420 7570 6461          and upda
+0001e1e0: 7465 7320 746f 7461 6c20 6d6f 6465 6c20  tes total model 
+0001e1f0: 706c 6f74 0a20 2020 2020 2020 2027 2727  plot.        '''
+0001e200: 0a0a 2020 2020 2020 2020 6d6f 6465 6c6e  ..        modeln
+0001e210: 616d 6520 3d20 6d6f 6465 6c2e 4e41 4d45  ame = model.NAME
+0001e220: 2e6c 6f77 6572 2829 0a0a 2020 2020 2020  .lower()..      
+0001e230: 2020 2320 436f 6e76 6572 7420 7661 6c20    # Convert val 
+0001e240: 746f 2062 6f6f 6c0a 2020 2020 2020 2020  to bool.        
+0001e250: 7661 6c20 3d20 626f 6f6c 2876 616c 202f  val = bool(val /
+0001e260: 2032 290a 0a20 2020 2020 2020 2023 2055   2)..        # U
+0001e270: 7064 6174 6520 6c69 7374 206f 6620 6d6f  pdate list of mo
+0001e280: 6465 6c73 0a20 2020 2020 2020 2073 656c  dels.        sel
+0001e290: 662e 7573 656c 2e6d 6f64 656c 735b 6d6f  f.usel.models[mo
+0001e2a0: 6465 6c6e 616d 655d 203d 2076 616c 0a0a  delname] = val..
+0001e2b0: 2020 2020 2020 2020 2320 5570 6461 7465          # Update
+0001e2c0: 206d 6f64 656c 2076 616c 7565 7320 616e   model values an
+0001e2d0: 6420 706c 6f74 2064 6174 6120 666f 7220  d plot data for 
+0001e2e0: 6561 6368 206d 6f64 656c 2c20 616e 6420  each model, and 
+0001e2f0: 666f 7220 746f 7461 6c0a 2020 2020 2020  for total.      
+0001e300: 2020 666f 7220 7061 726e 616d 6520 696e    for parname in
+0001e310: 206d 6f64 656c 2e50 4152 4e41 4d45 533a   model.PARNAMES:
+0001e320: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0001e330: 662e 7570 6461 7465 5f6d 6f64 656c 706c  f.update_modelpl
+0001e340: 6f74 280a 2020 2020 2020 2020 2020 2020  ot(.            
+0001e350: 2020 2020 6765 7461 7474 7228 7365 6c66      getattr(self
+0001e360: 2e70 6172 7374 6f72 652c 2070 6172 6e61  .parstore, parna
+0001e370: 6d65 292c 0a20 2020 2020 2020 2020 2020  me),.           
+0001e380: 2020 2020 2070 6172 6e61 6d65 2c0a 2020       parname,.  
+0001e390: 2020 2020 2020 2020 2020 2020 2020 6d6f                mo
+0001e3a0: 6465 6c0a 2020 2020 2020 2020 2020 2020  del.            
+0001e3b0: 290a 0a20 2020 2020 2020 2023 2053 656c  )..        # Sel
+0001e3c0: 6563 7420 6d6f 6465 6c20 706c 6f74 2074  ect model plot t
+0001e3d0: 6f20 746f 6767 6c65 0a20 2020 2020 2020  o toggle.       
+0001e3e0: 205f 706c 6f74 203d 2073 656c 662e 6d6f   _plot = self.mo
+0001e3f0: 6465 6c5f 706c 6f74 735b 6d6f 6465 6c6e  del_plots[modeln
+0001e400: 616d 655d 0a0a 2020 2020 2020 2020 2320  ame]..        # 
+0001e410: 4164 6420 6261 636b 2069 6e20 706c 6f74  Add back in plot
+0001e420: 0a20 2020 2020 2020 2069 6620 7661 6c3a  .        if val:
+0001e430: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0001e440: 662e 706c 6f74 5f77 6964 6765 742e 7265  f.plot_widget.re
+0001e450: 6d6f 7665 4974 656d 285f 706c 6f74 290a  moveItem(_plot).
+0001e460: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001e470: 2e70 6c6f 745f 7769 6467 6574 2e61 6464  .plot_widget.add
+0001e480: 4974 656d 285f 706c 6f74 290a 2020 2020  Item(_plot).    
+0001e490: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0001e4a0: 2020 2020 2020 7365 6c66 2e70 6c6f 745f        self.plot_
+0001e4b0: 7769 6467 6574 2e72 656d 6f76 6549 7465  widget.removeIte
+0001e4c0: 6d28 5f70 6c6f 7429 0a0a 2020 2020 2020  m(_plot)..      
+0001e4d0: 2020 2320 456e 6162 6c65 2074 6f74 616c    # Enable total
+0001e4e0: 2070 6c6f 7420 6966 203e 2031 206d 6f64   plot if > 1 mod
+0001e4f0: 656c 0a20 2020 2020 2020 2023 2061 6e64  el.        # and
+0001e500: 2065 6e61 626c 6520 6669 7420 6275 7474   enable fit butt
+0001e510: 6f6e 2069 6620 3e20 3020 6d6f 6465 6c73  on if > 0 models
+0001e520: 0a20 2020 2020 2020 206e 5f6d 6f64 656c  .        n_model
+0001e530: 7320 3d20 6e70 2e73 756d 285b 7661 6c20  s = np.sum([val 
+0001e540: 666f 7220 7661 6c20 696e 2073 656c 662e  for val in self.
+0001e550: 7573 656c 2e6d 6f64 656c 732e 7661 6c75  usel.models.valu
+0001e560: 6573 2829 5d29 0a20 2020 2020 2020 2069  es()]).        i
+0001e570: 6620 6e5f 6d6f 6465 6c73 203d 3d20 303a  f n_models == 0:
+0001e580: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0001e590: 662e 6669 745f 6274 6e5f 7769 6467 6574  f.fit_btn_widget
+0001e5a0: 2e73 6574 456e 6162 6c65 6428 4661 6c73  .setEnabled(Fals
+0001e5b0: 6529 0a20 2020 2020 2020 2065 6c69 6620  e).        elif 
+0001e5c0: 6e5f 6d6f 6465 6c73 203d 3d20 313a 0a20  n_models == 1:. 
+0001e5d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0001e5e0: 6669 745f 6274 6e5f 7769 6467 6574 2e73  fit_btn_widget.s
+0001e5f0: 6574 456e 6162 6c65 6428 5472 7565 290a  etEnabled(True).
+0001e600: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001e610: 2e70 6c6f 745f 7769 6467 6574 2e72 656d  .plot_widget.rem
+0001e620: 6f76 6549 7465 6d28 7365 6c66 2e74 6f74  oveItem(self.tot
+0001e630: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+0001e640: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001e650: 2e66 6974 5f62 746e 5f77 6964 6765 742e  .fit_btn_widget.
+0001e660: 7365 7445 6e61 626c 6564 2854 7275 6529  setEnabled(True)
+0001e670: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0001e680: 662e 706c 6f74 5f77 6964 6765 742e 7265  f.plot_widget.re
+0001e690: 6d6f 7665 4974 656d 2873 656c 662e 746f  moveItem(self.to
+0001e6a0: 7429 0a20 2020 2020 2020 2020 2020 2073  t).            s
+0001e6b0: 656c 662e 706c 6f74 5f77 6964 6765 742e  elf.plot_widget.
+0001e6c0: 6164 6449 7465 6d28 7365 6c66 2e74 6f74  addItem(self.tot
+0001e6d0: 290a 0a20 2020 2020 2020 2023 2045 6e61  )..        # Ena
+0001e6e0: 626c 652f 4469 7361 626c 6520 736c 6964  ble/Disable slid
+0001e6f0: 6572 2c20 6368 6563 6b62 6f78 2c20 616e  er, checkbox, an
+0001e700: 6420 6669 7466 6978 0a20 2020 2020 2020  d fitfix.       
+0001e710: 2066 6f72 2070 6172 6e61 6d65 2069 6e20   for parname in 
+0001e720: 6d6f 6465 6c2e 5041 524e 414d 4553 3a0a  model.PARNAMES:.
+0001e730: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001e740: 2e77 6964 6765 7464 6963 745b 6d6f 6465  .widgetdict[mode
+0001e750: 6c6e 616d 655d 5b70 6172 6e61 6d65 5d5b  lname][parname][
+0001e760: 2773 6c69 6465 7227 5d2e 7365 7445 6e61  'slider'].setEna
+0001e770: 626c 6564 2876 616c 290a 2020 2020 2020  bled(val).      
+0001e780: 2020 2020 2020 7365 6c66 2e77 6964 6765        self.widge
+0001e790: 7464 6963 745b 6d6f 6465 6c6e 616d 655d  tdict[modelname]
+0001e7a0: 5b70 6172 6e61 6d65 5d5b 2765 6e74 7279  [parname]['entry
+0001e7b0: 275d 2e73 6574 456e 6162 6c65 6428 7661  '].setEnabled(va
+0001e7c0: 6c29 0a20 2020 2020 2020 2020 2020 2073  l).            s
+0001e7d0: 656c 662e 7769 6467 6574 6469 6374 5b6d  elf.widgetdict[m
+0001e7e0: 6f64 656c 6e61 6d65 5d5b 7061 726e 616d  odelname][parnam
+0001e7f0: 655d 5b27 6666 5f74 6f67 676c 6527 5d2e  e]['ff_toggle'].
+0001e800: 7365 7445 6e61 626c 6564 2876 616c 290a  setEnabled(val).
+0001e810: 0a20 2020 2020 2020 2072 6574 7572 6e0a  .        return.
+0001e820: 0a20 2020 2064 6566 206d 616b 655f 6d6f  .    def make_mo
+0001e830: 6465 6c62 6f78 2873 656c 662c 206d 6f64  delbox(self, mod
+0001e840: 656c 3a20 4c6f 6754 6175 544d 6f64 656c  el: LogTauTModel
+0001e850: 2c20 7061 7265 6e74 2c20 696e 6465 783a  , parent, index:
+0001e860: 2069 6e74 293a 0a20 2020 2020 2020 2027   int):.        '
+0001e870: 2727 0a20 2020 2020 2020 2043 7265 6174  ''.        Creat
+0001e880: 6573 2077 6964 6765 7420 666f 7220 6120  es widget for a 
+0001e890: 6769 7665 6e20 6d6f 6465 6c2c 2063 6f6e  given model, con
+0001e8a0: 7461 696e 696e 6720 6120 6368 6563 6b62  taining a checkb
+0001e8b0: 6f78 2074 6f20 746f 6767 6c65 0a20 2020  ox to toggle.   
+0001e8c0: 2020 2020 2074 6865 206d 6f64 656c 2c20       the model, 
+0001e8d0: 616e 6420 6120 726f 7720 6f66 2069 6e74  and a row of int
+0001e8e0: 6572 6163 7469 7665 2077 6964 6765 7473  eractive widgets
+0001e8f0: 2066 6f72 2065 6163 6820 7061 7261 6d65   for each parame
+0001e900: 7465 7220 6f66 2074 6865 0a20 2020 2020  ter of the.     
+0001e910: 2020 206d 6f64 656c 0a20 2020 2020 2020     model.       
+0001e920: 2027 2727 0a0a 2020 2020 2020 2020 2320   '''..        # 
+0001e930: 5769 6467 6574 2066 6f72 2074 6869 7320  Widget for this 
+0001e940: 6d6f 6465 6c0a 2020 2020 2020 2020 6d6f  model.        mo
+0001e950: 6465 6c5f 7769 6467 6574 203d 2051 7457  del_widget = QtW
+0001e960: 6964 6765 7473 2e51 5769 6467 6574 2870  idgets.QWidget(p
+0001e970: 6172 656e 743d 7061 7265 6e74 290a 2020  arent=parent).  
+0001e980: 2020 2020 2020 6d6f 6465 6c5f 6c61 796f        model_layo
+0001e990: 7574 203d 2051 7457 6964 6765 7473 2e51  ut = QtWidgets.Q
+0001e9a0: 4842 6f78 4c61 796f 7574 286d 6f64 656c  HBoxLayout(model
+0001e9b0: 5f77 6964 6765 7429 0a0a 2020 2020 2020  _widget)..      
+0001e9c0: 2020 2320 4372 6561 7465 2074 6963 6b62    # Create tickb
+0001e9d0: 6f78 2074 6f20 746f 6767 6c65 2074 6869  ox to toggle thi
+0001e9e0: 7320 7769 6467 6574 0a20 2020 2020 2020  s widget.       
+0001e9f0: 2074 6963 6b62 6f78 5f77 6964 6765 7420   tickbox_widget 
+0001ea00: 3d20 5174 5769 6467 6574 732e 5143 6865  = QtWidgets.QChe
+0001ea10: 636b 426f 7828 0a20 2020 2020 2020 2020  ckBox(.         
+0001ea20: 2020 2070 6172 656e 743d 6d6f 6465 6c5f     parent=model_
+0001ea30: 7769 6467 6574 2c0a 2020 2020 2020 2020  widget,.        
+0001ea40: 2020 2020 7465 7874 3d6d 6f64 656c 2e4e      text=model.N
+0001ea50: 414d 452e 7265 706c 6163 6528 2742 726f  AME.replace('Bro
+0001ea60: 6e73 2d56 616e 2d56 6c65 636b 272c 2027  ns-Van-Vleck', '
+0001ea70: 4256 5627 292c 0a0a 2020 2020 2020 2020  BVV'),..        
+0001ea80: 290a 0a20 2020 2020 2020 2023 2041 6464  )..        # Add
+0001ea90: 2074 6963 6b62 6f78 2074 6f20 7468 6973   tickbox to this
+0001eaa0: 206d 6f64 656c 0a20 2020 2020 2020 206d   model.        m
+0001eab0: 6f64 656c 5f6c 6179 6f75 742e 6164 6457  odel_layout.addW
+0001eac0: 6964 6765 7428 7469 636b 626f 785f 7769  idget(tickbox_wi
+0001ead0: 6467 6574 290a 0a20 2020 2020 2020 2023  dget)..        #
+0001eae0: 2041 6464 2074 6f20 6469 6374 696f 6e61   Add to dictiona
+0001eaf0: 7279 206f 6620 616c 6c20 7469 636b 626f  ry of all tickbo
+0001eb00: 7865 732c 2069 6e64 6578 6564 2062 7920  xes, indexed by 
+0001eb10: 6d6f 6465 6c2e 4e41 4d45 2e6c 6f77 6572  model.NAME.lower
+0001eb20: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+0001eb30: 7469 636b 6469 6374 5b6d 6f64 656c 2e4e  tickdict[model.N
+0001eb40: 414d 452e 6c6f 7765 7228 295d 203d 2074  AME.lower()] = t
+0001eb50: 6963 6b62 6f78 5f77 6964 6765 740a 0a20  ickbox_widget.. 
+0001eb60: 2020 2020 2020 2023 2057 6865 6e20 746f         # When to
+0001eb70: 6767 6c65 642c 2070 6c6f 7420 7468 6973  ggled, plot this
+0001eb80: 206d 6f64 656c 0a20 2020 2020 2020 2074   model.        t
+0001eb90: 6963 6b62 6f78 5f77 6964 6765 742e 7374  ickbox_widget.st
+0001eba0: 6174 6543 6861 6e67 6564 2e63 6f6e 6e65  ateChanged.conne
+0001ebb0: 6374 280a 2020 2020 2020 2020 2020 2020  ct(.            
+0001ebc0: 6c61 6d62 6461 2076 616c 3a20 7365 6c66  lambda val: self
+0001ebd0: 2e74 6f67 676c 655f 706c 6f74 2876 616c  .toggle_plot(val
+0001ebe0: 2c20 6d6f 6465 6c29 0a20 2020 2020 2020  , model).       
+0001ebf0: 2029 0a0a 2020 2020 2020 2020 2320 4164   )..        # Ad
+0001ec00: 6420 6162 696c 6974 7920 746f 2074 6f67  d ability to tog
+0001ec10: 676c 6520 6d6f 6465 6c20 7573 696e 6720  gle model using 
+0001ec20: 6e75 6d62 6572 206b 6579 0a20 2020 2020  number key.     
+0001ec30: 2020 206f 6e5f 6f66 665f 7368 6f72 7463     on_off_shortc
+0001ec40: 7574 203d 2051 7457 6964 6765 7473 2e51  ut = QtWidgets.Q
+0001ec50: 5368 6f72 7463 7574 280a 2020 2020 2020  Shortcut(.      
+0001ec60: 2020 2020 2020 5174 4775 692e 514b 6579        QtGui.QKey
+0001ec70: 5365 7175 656e 6365 2827 7b3a 647d 272e  Sequence('{:d}'.
+0001ec80: 666f 726d 6174 2869 6e64 6578 2929 2c0a  format(index)),.
+0001ec90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001eca0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+0001ecb0: 2020 206f 6e5f 6f66 665f 7368 6f72 7463     on_off_shortc
+0001ecc0: 7574 2e61 6374 6976 6174 6564 2e63 6f6e  ut.activated.con
+0001ecd0: 6e65 6374 280a 2020 2020 2020 2020 2020  nect(.          
+0001ece0: 2020 6c61 6d62 6461 3a20 7469 636b 626f    lambda: tickbo
+0001ecf0: 785f 7769 6467 6574 2e74 6f67 676c 6528  x_widget.toggle(
+0001ed00: 290a 2020 2020 2020 2020 290a 2020 2020  ).        ).    
+0001ed10: 2020 2020 7365 6c66 2e6f 6e5f 6f66 665f      self.on_off_
+0001ed20: 7368 6f72 7463 7574 2e61 7070 656e 6428  shortcut.append(
+0001ed30: 6f6e 5f6f 6666 5f73 686f 7274 6375 7429  on_off_shortcut)
+0001ed40: 0a0a 2020 2020 2020 2020 2320 4372 6561  ..        # Crea
+0001ed50: 7465 2063 6f6e 7461 696e 6572 2077 6964  te container wid
+0001ed60: 6765 7420 666f 7220 616c 6c20 7061 7261  get for all para
+0001ed70: 6d65 7465 7220 726f 7773 0a20 2020 2020  meter rows.     
+0001ed80: 2020 2072 6873 5f77 6964 6765 7420 3d20     rhs_widget = 
+0001ed90: 5174 5769 6467 6574 732e 5157 6964 6765  QtWidgets.QWidge
+0001eda0: 7428 7061 7265 6e74 3d6d 6f64 656c 5f77  t(parent=model_w
+0001edb0: 6964 6765 7429 0a20 2020 2020 2020 2072  idget).        r
+0001edc0: 6873 5f6c 6179 6f75 7420 3d20 5174 5769  hs_layout = QtWi
+0001edd0: 6467 6574 732e 5156 426f 784c 6179 6f75  dgets.QVBoxLayou
+0001ede0: 7428 7268 735f 7769 6467 6574 290a 0a20  t(rhs_widget).. 
+0001edf0: 2020 2020 2020 2023 204d 616b 6520 736c         # Make sl
+0001ee00: 6964 6572 2c20 7465 7874 626f 782c 2061  ider, textbox, a
+0001ee10: 6e64 2066 6974 2f66 6978 2074 6f67 676c  nd fit/fix toggl
+0001ee20: 6520 666f 7220 6561 6368 0a20 2020 2020  e for each.     
+0001ee30: 2020 2023 2070 6172 616d 6574 6572 206f     # parameter o
+0001ee40: 6620 7468 6520 6375 7272 656e 7420 6d6f  f the current mo
+0001ee50: 6465 6c0a 2020 2020 2020 2020 666f 7220  del.        for 
+0001ee60: 7061 726e 616d 6520 696e 206d 6f64 656c  parname in model
+0001ee70: 2e50 4152 4e41 4d45 533a 0a0a 2020 2020  .PARNAMES:..    
+0001ee80: 2020 2020 2020 2020 2320 4465 6661 756c          # Defaul
+0001ee90: 7420 7061 7261 6d65 7465 7220 7661 6c75  t parameter valu
+0001eea0: 6573 0a20 2020 2020 2020 2020 2020 205f  es.            _
+0001eeb0: 6465 6661 756c 7473 203d 2073 656c 662e  defaults = self.
+0001eec0: 6465 6661 756c 7473 5b6d 6f64 656c 2e4e  defaults[model.N
+0001eed0: 414d 455d 5b70 6172 6e61 6d65 5d0a 0a20  AME][parname].. 
+0001eee0: 2020 2020 2020 2020 2020 2023 204e 616d             # Nam
+0001eef0: 6520 616e 6420 556e 6974 7320 6173 2073  e and Units as s
+0001ef00: 7472 696e 670a 2020 2020 2020 2020 2020  tring.          
+0001ef10: 2020 5f6e 755f 7374 7269 6e67 203d 2027    _nu_string = '
+0001ef20: 7b7d 2028 7b7d 2927 2e66 6f72 6d61 7428  {} ({})'.format(
+0001ef30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001ef40: 206d 6f64 656c 2e56 4152 4e41 4d45 535f   model.VARNAMES_
+0001ef50: 4854 4d4c 5b70 6172 6e61 6d65 5d2c 0a20  HTML[parname],. 
+0001ef60: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+0001ef70: 6f64 656c 2e55 4e49 5453 5f48 544d 4c5b  odel.UNITS_HTML[
+0001ef80: 7061 726e 616d 655d 0a20 2020 2020 2020  parname].       
+0001ef90: 2020 2020 2029 2e72 6570 6c61 6365 2827       ).replace('
+0001efa0: 2829 272c 2027 2729 0a0a 2020 2020 2020  ()', '')..      
+0001efb0: 2020 2020 2020 2320 4361 6c6c 6261 636b        # Callback
+0001efc0: 2066 6f72 2069 6e74 6572 6163 7469 6f6e   for interaction
+0001efd0: 2077 6974 6820 736c 6964 6572 2c20 7465   with slider, te
+0001efe0: 7874 626f 782e 2e2e 0a20 2020 2020 2020  xtbox....       
+0001eff0: 2020 2020 2063 6220 3d20 7061 7274 6961       cb = partia
+0001f000: 6c28 7365 6c66 2e75 7064 6174 655f 6d6f  l(self.update_mo
+0001f010: 6465 6c70 6c6f 742c 206d 6f64 656c 3d6d  delplot, model=m
+0001f020: 6f64 656c 2c20 7061 726e 616d 653d 7061  odel, parname=pa
+0001f030: 726e 616d 6529 0a0a 2020 2020 2020 2020  rname)..        
+0001f040: 2020 2020 2320 4d61 6b65 2072 6f77 206f      # Make row o
+0001f050: 6620 7769 6467 6574 7320 666f 7220 7468  f widgets for th
+0001f060: 6973 2070 6172 616d 6574 6572 0a20 2020  is parameter.   
+0001f070: 2020 2020 2020 2020 2070 6172 626f 785f           parbox_
+0001f080: 7769 6467 6574 2c20 7061 7262 6f78 5f6c  widget, parbox_l
+0001f090: 6179 6f75 7420 3d20 7365 6c66 2e6d 616b  ayout = self.mak
+0001f0a0: 655f 7061 7262 6f78 280a 2020 2020 2020  e_parbox(.      
+0001f0b0: 2020 2020 2020 2020 2020 6362 2c20 7061            cb, pa
+0001f0c0: 726e 616d 652c 205f 6e75 5f73 7472 696e  rname, _nu_strin
+0001f0d0: 672c 205f 6465 6661 756c 7473 2c20 6d6f  g, _defaults, mo
+0001f0e0: 6465 6c5f 7769 6467 6574 2c0a 2020 2020  del_widget,.    
+0001f0f0: 2020 2020 2020 2020 2020 2020 6d6f 6465              mode
+0001f100: 6c2e 4e41 4d45 2e6c 6f77 6572 2829 0a20  l.NAME.lower(). 
+0001f110: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+0001f120: 2020 2020 2020 2020 2020 2320 616e 6420            # and 
+0001f130: 6164 6420 746f 2074 6865 206d 6f64 656c  add to the model
+0001f140: 2773 2062 6f78 206f 6620 7061 7261 6d65  's box of parame
+0001f150: 7465 720a 2020 2020 2020 2020 2020 2020  ter.            
+0001f160: 7268 735f 6c61 796f 7574 2e61 6464 5769  rhs_layout.addWi
+0001f170: 6467 6574 2870 6172 626f 785f 7769 6467  dget(parbox_widg
+0001f180: 6574 290a 0a20 2020 2020 2020 2023 2053  et)..        # S
+0001f190: 6574 2065 7870 616e 7369 6f6e 2062 6568  et expansion beh
+0001f1a0: 6176 696f 7572 2061 6e64 2063 656e 7465  aviour and cente
+0001f1b0: 7269 6e67 206f 6620 7769 6467 6574 730a  ring of widgets.
+0001f1c0: 2020 2020 2020 2020 7268 735f 6c61 796f          rhs_layo
+0001f1d0: 7574 2e73 6574 416c 6967 6e6d 656e 7428  ut.setAlignment(
+0001f1e0: 5174 436f 7265 2e51 742e 416c 6967 6e56  QtCore.Qt.AlignV
+0001f1f0: 4365 6e74 6572 290a 2020 2020 2020 2020  Center).        
+0001f200: 7268 735f 7769 6467 6574 2e73 6574 5369  rhs_widget.setSi
+0001f210: 7a65 506f 6c69 6379 280a 2020 2020 2020  zePolicy(.      
+0001f220: 2020 2020 2020 5174 5769 6467 6574 732e        QtWidgets.
+0001f230: 5153 697a 6550 6f6c 6963 792e 4669 7865  QSizePolicy.Fixe
+0001f240: 642c 0a20 2020 2020 2020 2020 2020 2051  d,.            Q
+0001f250: 7457 6964 6765 7473 2e51 5369 7a65 506f  tWidgets.QSizePo
+0001f260: 6c69 6379 2e46 6978 6564 0a20 2020 2020  licy.Fixed.     
+0001f270: 2020 2029 0a20 2020 2020 2020 2074 6963     ).        tic
+0001f280: 6b62 6f78 5f77 6964 6765 742e 7365 7453  kbox_widget.setS
+0001f290: 697a 6550 6f6c 6963 7928 0a20 2020 2020  izePolicy(.     
+0001f2a0: 2020 2020 2020 2051 7457 6964 6765 7473         QtWidgets
+0001f2b0: 2e51 5369 7a65 506f 6c69 6379 2e46 6978  .QSizePolicy.Fix
+0001f2c0: 6564 2c0a 2020 2020 2020 2020 2020 2020  ed,.            
+0001f2d0: 5174 5769 6467 6574 732e 5153 697a 6550  QtWidgets.QSizeP
+0001f2e0: 6f6c 6963 792e 4669 7865 640a 2020 2020  olicy.Fixed.    
+0001f2f0: 2020 2020 290a 0a20 2020 2020 2020 2072      )..        r
+0001f300: 6873 5f6c 6179 6f75 742e 7365 7453 7061  hs_layout.setSpa
+0001f310: 6369 6e67 2830 290a 2020 2020 2020 2020  cing(0).        
+0001f320: 7268 735f 6c61 796f 7574 2e61 6464 5374  rhs_layout.addSt
+0001f330: 7265 7463 6828 3429 0a0a 2020 2020 2020  retch(4)..      
+0001f340: 2020 2320 4164 6420 7061 7261 6d65 7465    # Add paramete
+0001f350: 7220 726f 7773 2074 6f20 7468 6973 206d  r rows to this m
+0001f360: 6f64 656c 0a20 2020 2020 2020 206d 6f64  odel.        mod
+0001f370: 656c 5f6c 6179 6f75 742e 6164 6457 6964  el_layout.addWid
+0001f380: 6765 7428 7268 735f 7769 6467 6574 290a  get(rhs_widget).
+0001f390: 0a20 2020 2020 2020 2023 2061 6e64 2073  .        # and s
+0001f3a0: 6574 2061 6c69 676e 6d65 6e74 206f 6620  et alignment of 
+0001f3b0: 7468 6520 6d6f 6465 6c0a 2020 2020 2020  the model.      
+0001f3c0: 2020 6d6f 6465 6c5f 6c61 796f 7574 2e73    model_layout.s
+0001f3d0: 6574 416c 6967 6e6d 656e 7428 5174 436f  etAlignment(QtCo
+0001f3e0: 7265 2e51 742e 416c 6967 6e54 6f70 290a  re.Qt.AlignTop).
+0001f3f0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0001f400: 6d6f 6465 6c5f 7769 6467 6574 0a0a 2020  model_widget..  
+0001f410: 2020 6465 6620 6e6f 745f 6966 7928 7365    def not_ify(se
+0001f420: 6c66 2c20 7061 726e 616d 653a 2073 7472  lf, parname: str
+0001f430: 293a 0a20 2020 2020 2020 2027 2727 0a20  ):.        '''. 
+0001f440: 2020 2020 2020 2053 7769 7463 6865 7320         Switches 
+0001f450: 6669 7420 6469 6374 696f 6e61 7279 2065  fit dictionary e
+0001f460: 6e74 7279 2054 7275 6520 3c2d 2d3e 2046  ntry True <--> F
+0001f470: 616c 7365 0a20 2020 2020 2020 2066 6f72  alse.        for
+0001f480: 2074 6865 2070 726f 7669 6465 6420 7061   the provided pa
+0001f490: 726e 616d 650a 2020 2020 2020 2020 2727  rname.        ''
+0001f4a0: 270a 2020 2020 2020 2020 7365 6c66 2e75  '.        self.u
+0001f4b0: 7365 6c2e 6669 745b 7061 726e 616d 655d  sel.fit[parname]
+0001f4c0: 203d 206e 6f74 2073 656c 662e 7573 656c   = not self.usel
+0001f4d0: 2e66 6974 5b70 6172 6e61 6d65 5d0a 0a20  .fit[parname].. 
+0001f4e0: 2020 2064 6566 206d 616b 655f 7061 7262     def make_parb
+0001f4f0: 6f78 2873 656c 662c 2063 623a 2070 6172  ox(self, cb: par
+0001f500: 7469 616c 2c20 7061 726e 616d 653a 2073  tial, parname: s
+0001f510: 7472 2c20 5f6e 755f 7374 7269 6e67 3a20  tr, _nu_string: 
+0001f520: 7374 722c 0a20 2020 2020 2020 2020 2020  str,.           
+0001f530: 2020 2020 2020 2020 2064 6566 6175 6c74           default
+0001f540: 733a 2064 6963 745b 7374 722c 2066 6c6f  s: dict[str, flo
+0001f550: 6174 5d2c 206f 705f 7061 723a 2051 7457  at], op_par: QtW
+0001f560: 6964 6765 7473 2e51 5769 6467 6574 2c0a  idgets.QWidget,.
+0001f570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f580: 2020 2020 6d6f 6465 6c6e 616d 653a 2073      modelname: s
+0001f590: 7472 293a 0a20 2020 2020 2020 2027 2727  tr):.        '''
+0001f5a0: 0a20 2020 2020 2020 2043 7265 6174 6573  .        Creates
+0001f5b0: 2073 6574 206f 6620 7769 6467 6574 7320   set of widgets 
+0001f5c0: 666f 7220 6120 7369 6e67 6c65 2070 6172  for a single par
+0001f5d0: 616d 6574 6572 206f 6620 6120 6d6f 6465  ameter of a mode
+0001f5e0: 6c2e 5c6e 0a20 2020 2020 2020 2043 6f6e  l.\n.        Con
+0001f5f0: 7461 696e 7320 3220 726f 7773 2c20 7570  tains 2 rows, up
+0001f600: 7065 7220 6973 206c 6162 656c 2061 6e64  per is label and
+0001f610: 2075 6e69 7473 2061 7320 7374 7269 6e67   units as string
+0001f620: 2c20 616e 6420 6c6f 7765 720a 2020 2020  , and lower.    
+0001f630: 2020 2020 6973 2073 6c69 6465 722c 2074      is slider, t
+0001f640: 6578 7465 6e74 7279 2028 646f 7562 6c65  extentry (double
+0001f650: 7370 696e 626f 7829 2c20 616e 6420 6669  spinbox), and fi
+0001f660: 742f 6669 7820 746f 6767 6c65 2062 7574  t/fix toggle but
+0001f670: 746f 6e2e 0a0a 2020 2020 2020 2020 5061  ton...        Pa
+0001f680: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
+0001f690: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+0001f6a0: 2020 2020 6362 3a20 6675 6e63 746f 6f6c      cb: functool
+0001f6b0: 732e 7061 7274 6961 6c0a 2020 2020 2020  s.partial.      
+0001f6c0: 2020 2020 2020 5061 7274 6961 6c2d 6c79        Partial-ly
+0001f6d0: 2069 6e73 7461 6e74 6961 7465 6420 6361   instantiated ca
+0001f6e0: 6c6c 6261 636b 2077 6869 6368 2077 696c  llback which wil
+0001f6f0: 6c20 6265 2066 6972 6564 2077 6865 6e0a  l be fired when.
+0001f700: 2020 2020 2020 2020 2020 2020 7769 6467              widg
+0001f710: 6574 7320 6f66 2074 6869 7320 7061 7261  ets of this para
+0001f720: 6d65 7465 7220 6172 6520 696e 7465 7261  meter are intera
+0001f730: 6374 6564 2077 6974 682e 0a20 2020 2020  cted with..     
+0001f740: 2020 2070 6172 6e61 6d65 3a20 7374 720a     parname: str.
+0001f750: 2020 2020 2020 2020 2020 2020 5374 7269              Stri
+0001f760: 6e67 206e 616d 6520 6f66 2070 6172 616d  ng name of param
+0001f770: 6574 6572 2075 7365 6420 6173 206b 6579  eter used as key
+0001f780: 2069 6e0a 2020 2020 2020 2020 2020 2020   in.            
+0001f790: 7365 6c66 2e77 6964 6765 7464 6963 745b  self.widgetdict[
+0001f7a0: 7769 6467 6574 6469 6374 5d0a 2020 2020  widgetdict].    
+0001f7b0: 2020 2020 5f6e 755f 7374 7269 6e67 3a20      _nu_string: 
+0001f7c0: 7374 720a 2020 2020 2020 2020 2020 2020  str.            
+0001f7d0: 5374 7269 6e67 206e 616d 6520 6f66 2070  String name of p
+0001f7e0: 6172 616d 6574 6572 2061 6e64 2075 6e69  arameter and uni
+0001f7f0: 7473 2075 7365 6420 6173 2074 6974 6c65  ts used as title
+0001f800: 206f 6620 7468 6973 2070 6172 616d 6574   of this paramet
+0001f810: 6572 0a20 2020 2020 2020 2064 6566 6175  er.        defau
+0001f820: 6c74 733a 2064 6963 745b 7374 722c 2066  lts: dict[str, f
+0001f830: 6c6f 6174 5d0a 2020 2020 2020 2020 2020  loat].          
+0001f840: 2020 4465 6661 756c 7420 7661 6c75 6573    Default values
+0001f850: 206f 6620 7468 6973 2070 6172 616d 6574   of this paramet
+0001f860: 6572 2c20 6b65 7973 2061 7265 206d 696e  er, keys are min
+0001f870: 2c20 6d61 782c 2076 616c 696e 6974 2c20  , max, valinit, 
+0001f880: 7374 6570 0a20 2020 2020 2020 206f 705f  step.        op_
+0001f890: 7061 723a 2051 7457 6964 6765 7473 2e51  par: QtWidgets.Q
+0001f8a0: 5769 6467 6574 0a20 2020 2020 2020 2020  Widget.         
+0001f8b0: 2020 2050 6172 656e 7420 7769 6467 6574     Parent widget
+0001f8c0: 0a20 2020 2020 2020 206d 6f64 656c 6e61  .        modelna
+0001f8d0: 6d65 3a20 7374 720a 2020 2020 2020 2020  me: str.        
+0001f8e0: 2020 2020 5374 7269 6e67 206e 616d 6520      String name 
+0001f8f0: 6f66 206d 6f64 656c 2075 7365 6420 6173  of model used as
+0001f900: 206b 6579 2069 6e20 7365 6c66 2e77 6964   key in self.wid
+0001f910: 6765 7464 6963 740a 2020 2020 2020 2020  getdict.        
+0001f920: 2727 270a 0a20 2020 2020 2020 2023 2057  '''..        # W
+0001f930: 6964 6765 7420 666f 7220 7468 6973 2070  idget for this p
+0001f940: 6172 616d 6574 6572 2773 2072 6f77 206f  arameter's row o
+0001f950: 6620 7769 6467 6574 730a 2020 2020 2020  f widgets.      
+0001f960: 2020 6f6e 655f 7061 7261 6d5f 7769 6467    one_param_widg
+0001f970: 6574 203d 2051 7457 6964 6765 7473 2e51  et = QtWidgets.Q
+0001f980: 5769 6467 6574 2870 6172 656e 743d 6f70  Widget(parent=op
+0001f990: 5f70 6172 290a 2020 2020 2020 2020 6f6e  _par).        on
+0001f9a0: 655f 7061 7261 6d5f 6c61 796f 7574 203d  e_param_layout =
+0001f9b0: 2051 7457 6964 6765 7473 2e51 5642 6f78   QtWidgets.QVBox
+0001f9c0: 4c61 796f 7574 286f 6e65 5f70 6172 616d  Layout(one_param
+0001f9d0: 5f77 6964 6765 7429 0a0a 2020 2020 2020  _widget)..      
+0001f9e0: 2020 2320 466f 7220 6c61 6265 6c20 616e    # For label an
+0001f9f0: 6420 756e 6974 730a 2020 2020 2020 2020  d units.        
+0001fa00: 746f 705f 626f 7877 6964 6765 7420 3d20  top_boxwidget = 
+0001fa10: 5174 5769 6467 6574 732e 5157 6964 6765  QtWidgets.QWidge
+0001fa20: 7428 7061 7265 6e74 3d6f 6e65 5f70 6172  t(parent=one_par
+0001fa30: 616d 5f77 6964 6765 7429 0a20 2020 2020  am_widget).     
+0001fa40: 2020 2074 6f70 5f62 6f78 6c61 796f 7574     top_boxlayout
+0001fa50: 203d 2051 7457 6964 6765 7473 2e51 4842   = QtWidgets.QHB
+0001fa60: 6f78 4c61 796f 7574 2874 6f70 5f62 6f78  oxLayout(top_box
+0001fa70: 7769 6467 6574 290a 0a20 2020 2020 2020  widget)..       
+0001fa80: 2023 2046 6f72 2069 6e74 6572 6163 7469   # For interacti
+0001fa90: 7665 2077 6964 6765 7473 0a20 2020 2020  ve widgets.     
+0001faa0: 2020 2062 6f74 5f62 6f78 7769 6467 6574     bot_boxwidget
+0001fab0: 203d 2051 7457 6964 6765 7473 2e51 5769   = QtWidgets.QWi
+0001fac0: 6467 6574 2870 6172 656e 743d 6f6e 655f  dget(parent=one_
+0001fad0: 7061 7261 6d5f 7769 6467 6574 290a 2020  param_widget).  
+0001fae0: 2020 2020 2020 626f 745f 626f 786c 6179        bot_boxlay
+0001faf0: 6f75 7420 3d20 5174 5769 6467 6574 732e  out = QtWidgets.
+0001fb00: 5148 426f 784c 6179 6f75 7428 626f 745f  QHBoxLayout(bot_
+0001fb10: 626f 7877 6964 6765 7429 0a0a 2020 2020  boxwidget)..    
+0001fb20: 2020 2020 2320 4164 6420 6c61 6265 6c20      # Add label 
+0001fb30: 616e 6420 756e 6974 730a 2020 2020 2020  and units.      
+0001fb40: 2020 6e61 6d65 5f75 6e69 7473 203d 2051    name_units = Q
+0001fb50: 7457 6964 6765 7473 2e51 4c61 6265 6c28  tWidgets.QLabel(
+0001fb60: 5f6e 755f 7374 7269 6e67 290a 2020 2020  _nu_string).    
+0001fb70: 2020 2020 6e61 6d65 5f75 6e69 7473 2e73      name_units.s
+0001fb80: 6574 466f 6e74 2851 7447 7569 2e51 466f  etFont(QtGui.QFo
+0001fb90: 6e74 2827 4172 6961 6c27 2c20 3131 2929  nt('Arial', 11))
+0001fba0: 0a0a 2020 2020 2020 2020 6e61 6d65 5f75  ..        name_u
+0001fbb0: 6e69 7473 2e73 6574 5369 7a65 506f 6c69  nits.setSizePoli
+0001fbc0: 6379 280a 2020 2020 2020 2020 2020 2020  cy(.            
+0001fbd0: 5174 5769 6467 6574 732e 5153 697a 6550  QtWidgets.QSizeP
+0001fbe0: 6f6c 6963 792e 4669 7865 642c 0a20 2020  olicy.Fixed,.   
+0001fbf0: 2020 2020 2020 2020 2051 7457 6964 6765           QtWidge
+0001fc00: 7473 2e51 5369 7a65 506f 6c69 6379 2e46  ts.QSizePolicy.F
+0001fc10: 6978 6564 0a20 2020 2020 2020 2029 0a0a  ixed.        )..
+0001fc20: 2020 2020 2020 2020 746f 705f 626f 786c          top_boxl
+0001fc30: 6179 6f75 742e 6164 6457 6964 6765 7428  ayout.addWidget(
+0001fc40: 6e61 6d65 5f75 6e69 7473 290a 0a20 2020  name_units)..   
+0001fc50: 2020 2020 2023 2043 7265 6174 6520 736c       # Create sl
+0001fc60: 6964 6572 0a20 2020 2020 2020 2073 6c69  ider.        sli
+0001fc70: 6465 7220 3d20 5174 5769 6467 6574 732e  der = QtWidgets.
+0001fc80: 5153 6c69 6465 7228 0a20 2020 2020 2020  QSlider(.       
+0001fc90: 2020 2020 206f 7269 656e 7461 7469 6f6e       orientation
+0001fca0: 3d51 7443 6f72 652e 5174 2e48 6f72 697a  =QtCore.Qt.Horiz
+0001fcb0: 6f6e 7461 6c2c 0a20 2020 2020 2020 2020  ontal,.         
+0001fcc0: 2020 2070 6172 656e 743d 626f 745f 626f     parent=bot_bo
+0001fcd0: 7877 6964 6765 740a 2020 2020 2020 2020  xwidget.        
+0001fce0: 290a 0a20 2020 2020 2020 2023 2053 6361  )..        # Sca
+0001fcf0: 6c65 2061 6c6c 2073 6c69 6465 7220 6e75  le all slider nu
+0001fd00: 6d62 6572 7320 6279 2074 6869 7320 746f  mbers by this to
+0001fd10: 206d 616b 6520 696e 746f 2066 6c6f 6174   make into float
+0001fd20: 730a 2020 2020 2020 2020 736c 6964 6572  s.        slider
+0001fd30: 5f73 6361 6c65 203d 2031 4535 0a0a 2020  _scale = 1E5..  
+0001fd40: 2020 2020 2020 736c 6964 6572 2e73 6574        slider.set
+0001fd50: 4d69 6e69 6d75 6d28 696e 7428 6465 6661  Minimum(int(defa
+0001fd60: 756c 7473 5b27 6d69 6e27 5d20 2a20 736c  ults['min'] * sl
+0001fd70: 6964 6572 5f73 6361 6c65 2929 0a20 2020  ider_scale)).   
+0001fd80: 2020 2020 2073 6c69 6465 722e 7365 744d       slider.setM
+0001fd90: 6178 696d 756d 2869 6e74 2864 6566 6175  aximum(int(defau
+0001fda0: 6c74 735b 276d 6178 275d 202a 2073 6c69  lts['max'] * sli
+0001fdb0: 6465 725f 7363 616c 6529 290a 2020 2020  der_scale)).    
+0001fdc0: 2020 2020 736c 6964 6572 2e73 6574 5661      slider.setVa
+0001fdd0: 6c75 6528 696e 7428 6465 6661 756c 7473  lue(int(defaults
+0001fde0: 5b27 7661 6c69 6e69 7427 5d20 2a20 736c  ['valinit'] * sl
+0001fdf0: 6964 6572 5f73 6361 6c65 2929 0a20 2020  ider_scale)).   
+0001fe00: 2020 2020 2073 6c69 6465 722e 7365 7453       slider.setS
+0001fe10: 696e 676c 6553 7465 7028 696e 7428 6465  ingleStep(int(de
+0001fe20: 6661 756c 7473 5b27 7374 6570 275d 202a  faults['step'] *
+0001fe30: 2073 6c69 6465 725f 7363 616c 6529 290a   slider_scale)).
+0001fe40: 0a20 2020 2020 2020 2073 656c 662e 7769  .        self.wi
+0001fe50: 6467 6574 6469 6374 5b6d 6f64 656c 6e61  dgetdict[modelna
+0001fe60: 6d65 2e6c 6f77 6572 2829 5d5b 7061 726e  me.lower()][parn
+0001fe70: 616d 655d 5b27 736c 6964 6572 275d 203d  ame]['slider'] =
+0001fe80: 2073 6c69 6465 720a 0a20 2020 2020 2020   slider..       
+0001fe90: 2023 2041 6464 2073 6c69 6465 7220 746f   # Add slider to
+0001fea0: 206c 6179 6f75 740a 2020 2020 2020 2020   layout.        
+0001feb0: 626f 745f 626f 786c 6179 6f75 742e 6164  bot_boxlayout.ad
+0001fec0: 6457 6964 6765 7428 736c 6964 6572 290a  dWidget(slider).
+0001fed0: 0a20 2020 2020 2020 2023 2043 7265 6174  .        # Creat
+0001fee0: 6520 7465 7874 2065 6e74 7279 2028 446f  e text entry (Do
+0001fef0: 7562 6c65 5370 696e 426f 7829 0a20 2020  ubleSpinBox).   
+0001ff00: 2020 2020 2065 6e74 7279 203d 2051 7457       entry = QtW
+0001ff10: 6964 6765 7473 2e51 446f 7562 6c65 5370  idgets.QDoubleSp
+0001ff20: 696e 426f 7828 7061 7265 6e74 3d62 6f74  inBox(parent=bot
+0001ff30: 5f62 6f78 7769 6467 6574 290a 2020 2020  _boxwidget).    
+0001ff40: 2020 2020 656e 7472 792e 7365 7444 6563      entry.setDec
+0001ff50: 696d 616c 7328 696e 7428 6465 6661 756c  imals(int(defaul
+0001ff60: 7473 5b27 6465 6369 6d61 6c73 275d 2929  ts['decimals']))
+0001ff70: 0a20 2020 2020 2020 2065 6e74 7279 2e73  .        entry.s
+0001ff80: 6574 4275 7474 6f6e 5379 6d62 6f6c 7328  etButtonSymbols(
+0001ff90: 5174 5769 6467 6574 732e 5144 6f75 626c  QtWidgets.QDoubl
+0001ffa0: 6553 7069 6e42 6f78 2e4e 6f42 7574 746f  eSpinBox.NoButto
+0001ffb0: 6e73 290a 2020 2020 2020 2020 656e 7472  ns).        entr
+0001ffc0: 792e 7365 744b 6579 626f 6172 6454 7261  y.setKeyboardTra
+0001ffd0: 636b 696e 6728 4661 6c73 6529 0a20 2020  cking(False).   
+0001ffe0: 2020 2020 2065 6e74 7279 2e73 6574 4d69       entry.setMi
+0001fff0: 6e69 6d75 6d28 6465 6661 756c 7473 5b27  nimum(defaults['
+00020000: 6d69 6e27 5d29 0a20 2020 2020 2020 2065  min']).        e
+00020010: 6e74 7279 2e73 6574 4d61 7869 6d75 6d28  ntry.setMaximum(
+00020020: 6465 6661 756c 7473 5b27 6d61 7827 5d29  defaults['max'])
+00020030: 0a20 2020 2020 2020 2065 6e74 7279 2e73  .        entry.s
+00020040: 6574 5661 6c75 6528 6465 6661 756c 7473  etValue(defaults
+00020050: 5b27 7661 6c69 6e69 7427 5d29 0a20 2020  ['valinit']).   
+00020060: 2020 2020 2065 6e74 7279 2e73 6574 5369       entry.setSi
+00020070: 6e67 6c65 5374 6570 2864 6566 6175 6c74  ngleStep(default
+00020080: 735b 2773 7465 7027 5d29 0a0a 2020 2020  s['step'])..    
+00020090: 2020 2020 7365 6c66 2e77 6964 6765 7464      self.widgetd
+000200a0: 6963 745b 6d6f 6465 6c6e 616d 652e 6c6f  ict[modelname.lo
+000200b0: 7765 7228 295d 5b70 6172 6e61 6d65 5d5b  wer()][parname][
+000200c0: 2765 6e74 7279 275d 203d 2065 6e74 7279  'entry'] = entry
+000200d0: 0a0a 2020 2020 2020 2020 2320 4164 6420  ..        # Add 
+000200e0: 646f 7562 6c65 7370 696e 626f 7820 746f  doublespinbox to
+000200f0: 206c 6179 6f75 740a 2020 2020 2020 2020   layout.        
+00020100: 626f 745f 626f 786c 6179 6f75 742e 6164  bot_boxlayout.ad
+00020110: 6457 6964 6765 7428 656e 7472 7929 0a0a  dWidget(entry)..
+00020120: 2020 2020 2020 2020 2320 4372 6561 7465          # Create
+00020130: 2066 6974 2f66 6978 2074 6f67 676c 6520   fit/fix toggle 
+00020140: 6275 7474 6f6e 0a20 2020 2020 2020 2066  button.        f
+00020150: 665f 746f 6767 6c65 203d 2051 7457 6964  f_toggle = QtWid
+00020160: 6765 7473 2e51 5075 7368 4275 7474 6f6e  gets.QPushButton
+00020170: 2827 4672 6565 272c 2070 6172 656e 743d  ('Free', parent=
+00020180: 626f 745f 626f 7877 6964 6765 7429 0a0a  bot_boxwidget)..
+00020190: 2020 2020 2020 2020 7365 6c66 2e77 6964          self.wid
+000201a0: 6765 7464 6963 745b 6d6f 6465 6c6e 616d  getdict[modelnam
+000201b0: 652e 6c6f 7765 7228 295d 5b70 6172 6e61  e.lower()][parna
+000201c0: 6d65 5d5b 2766 665f 746f 6767 6c65 275d  me]['ff_toggle']
+000201d0: 203d 2066 665f 746f 6767 6c65 0a0a 2020   = ff_toggle..  
+000201e0: 2020 2020 2020 6666 7377 203d 207b 0a20        ffsw = {. 
+000201f0: 2020 2020 2020 2020 2020 2027 4672 6565             'Free
+00020200: 273a 2027 4669 7865 6427 2c0a 2020 2020  ': 'Fixed',.    
+00020210: 2020 2020 2020 2020 2746 6978 6564 273a          'Fixed':
+00020220: 2027 4672 6565 272c 0a20 2020 2020 2020   'Free',.       
+00020230: 207d 0a0a 2020 2020 2020 2020 2320 4361   }..        # Ca
+00020240: 6c6c 6261 636b 2066 6f72 2074 6578 740a  llback for text.
+00020250: 2020 2020 2020 2020 6666 5f74 6f67 676c          ff_toggl
+00020260: 652e 636c 6963 6b65 642e 636f 6e6e 6563  e.clicked.connec
+00020270: 7428 0a20 2020 2020 2020 2020 2020 206c  t(.            l
+00020280: 616d 6264 6120 5f3a 2066 665f 746f 6767  ambda _: ff_togg
+00020290: 6c65 2e73 6574 5465 7874 2866 6673 775b  le.setText(ffsw[
+000202a0: 6666 5f74 6f67 676c 652e 7465 7874 2829  ff_toggle.text()
+000202b0: 5d29 0a20 2020 2020 2020 2029 0a0a 2020  ]).        )..  
+000202c0: 2020 2020 2020 2320 4361 6c6c 6261 636b        # Callback
+000202d0: 2066 6f72 2066 6974 2f66 6978 206f 6620   for fit/fix of 
+000202e0: 7468 6973 2070 6172 616d 6574 6572 0a20  this parameter. 
+000202f0: 2020 2020 2020 2066 665f 746f 6767 6c65         ff_toggle
+00020300: 2e63 6c69 636b 6564 2e63 6f6e 6e65 6374  .clicked.connect
+00020310: 280a 2020 2020 2020 2020 2020 2020 6c61  (.            la
+00020320: 6d62 6461 205f 3a20 7365 6c66 2e6e 6f74  mbda _: self.not
+00020330: 5f69 6679 2870 6172 6e61 6d65 290a 2020  _ify(parname).  
+00020340: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+00020350: 2023 2043 6f6e 6e65 6374 2066 6974 2f66   # Connect fit/f
+00020360: 6978 2074 6f20 736c 6964 6572 2061 6e64  ix to slider and
+00020370: 2074 6578 7465 6e74 7279 0a20 2020 2020   textentry.     
+00020380: 2020 2073 6c69 6465 722e 7661 6c75 6543     slider.valueC
+00020390: 6861 6e67 6564 2e63 6f6e 6e65 6374 286c  hanged.connect(l
+000203a0: 616d 6264 6120 7661 6c3a 2063 6228 7661  ambda val: cb(va
+000203b0: 6c20 2a20 736c 6964 6572 5f73 6361 6c65  l * slider_scale
+000203c0: 2a2a 2d31 2929 0a20 2020 2020 2020 2073  **-1)).        s
+000203d0: 6c69 6465 722e 7661 6c75 6543 6861 6e67  lider.valueChang
+000203e0: 6564 2e63 6f6e 6e65 6374 280a 2020 2020  ed.connect(.    
+000203f0: 2020 2020 2020 2020 6c61 6d62 6461 2076          lambda v
+00020400: 616c 3a20 656e 7472 792e 7365 7456 616c  al: entry.setVal
+00020410: 7565 2876 616c 202a 2073 6c69 6465 725f  ue(val * slider_
+00020420: 7363 616c 652a 2a2d 3129 0a20 2020 2020  scale**-1).     
+00020430: 2020 2029 0a20 2020 2020 2020 2065 6e74     ).        ent
+00020440: 7279 2e76 616c 7565 4368 616e 6765 642e  ry.valueChanged.
+00020450: 636f 6e6e 6563 7428 6362 290a 2020 2020  connect(cb).    
+00020460: 2020 2020 656e 7472 792e 7661 6c75 6543      entry.valueC
+00020470: 6861 6e67 6564 2e63 6f6e 6e65 6374 280a  hanged.connect(.
+00020480: 2020 2020 2020 2020 2020 2020 6c61 6d62              lamb
+00020490: 6461 2076 616c 3a20 736c 6964 6572 2e73  da val: slider.s
+000204a0: 6574 5661 6c75 6528 696e 7428 7661 6c20  etValue(int(val 
+000204b0: 2a20 736c 6964 6572 5f73 6361 6c65 2929  * slider_scale))
+000204c0: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+000204d0: 2020 2020 2320 4164 6420 6669 742f 6669      # Add fit/fi
+000204e0: 7820 746f 206c 6179 6f75 740a 2020 2020  x to layout.    
+000204f0: 2020 2020 626f 745f 626f 786c 6179 6f75      bot_boxlayou
+00020500: 742e 6164 6457 6964 6765 7428 6666 5f74  t.addWidget(ff_t
+00020510: 6f67 676c 6529 0a0a 2020 2020 2020 2020  oggle)..        
+00020520: 746f 705f 626f 7877 6964 6765 742e 7365  top_boxwidget.se
+00020530: 7453 697a 6550 6f6c 6963 7928 0a20 2020  tSizePolicy(.   
+00020540: 2020 2020 2020 2020 2051 7457 6964 6765           QtWidge
+00020550: 7473 2e51 5369 7a65 506f 6c69 6379 2e46  ts.QSizePolicy.F
+00020560: 6978 6564 2c0a 2020 2020 2020 2020 2020  ixed,.          
+00020570: 2020 5174 5769 6467 6574 732e 5153 697a    QtWidgets.QSiz
+00020580: 6550 6f6c 6963 792e 4669 7865 640a 2020  ePolicy.Fixed.  
+00020590: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+000205a0: 626f 745f 626f 7877 6964 6765 742e 7365  bot_boxwidget.se
+000205b0: 7453 697a 6550 6f6c 6963 7928 0a20 2020  tSizePolicy(.   
+000205c0: 2020 2020 2020 2020 2051 7457 6964 6765           QtWidge
+000205d0: 7473 2e51 5369 7a65 506f 6c69 6379 2e46  ts.QSizePolicy.F
+000205e0: 6978 6564 2c0a 2020 2020 2020 2020 2020  ixed,.          
+000205f0: 2020 5174 5769 6467 6574 732e 5153 697a    QtWidgets.QSiz
+00020600: 6550 6f6c 6963 792e 4669 7865 640a 2020  ePolicy.Fixed.  
+00020610: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00020620: 746f 705f 626f 786c 6179 6f75 742e 7365  top_boxlayout.se
+00020630: 7441 6c69 676e 6d65 6e74 2851 7443 6f72  tAlignment(QtCor
+00020640: 652e 5174 2e41 6c69 676e 4843 656e 7465  e.Qt.AlignHCente
+00020650: 7229 0a0a 2020 2020 2020 2020 6f6e 655f  r)..        one_
+00020660: 7061 7261 6d5f 6c61 796f 7574 2e61 6464  param_layout.add
+00020670: 5769 6467 6574 2874 6f70 5f62 6f78 7769  Widget(top_boxwi
+00020680: 6467 6574 290a 2020 2020 2020 2020 6f6e  dget).        on
+00020690: 655f 7061 7261 6d5f 6c61 796f 7574 2e61  e_param_layout.a
+000206a0: 6464 5769 6467 6574 2862 6f74 5f62 6f78  ddWidget(bot_box
+000206b0: 7769 6467 6574 290a 0a20 2020 2020 2020  widget)..       
+000206c0: 206f 6e65 5f70 6172 616d 5f6c 6179 6f75   one_param_layou
+000206d0: 742e 7365 7443 6f6e 7465 6e74 734d 6172  t.setContentsMar
+000206e0: 6769 6e73 2830 2c20 302c 2030 2c20 3029  gins(0, 0, 0, 0)
+000206f0: 0a20 2020 2020 2020 206f 6e65 5f70 6172  .        one_par
+00020700: 616d 5f6c 6179 6f75 742e 7365 7453 7061  am_layout.setSpa
+00020710: 6369 6e67 2832 290a 2020 2020 2020 2020  cing(2).        
+00020720: 6f6e 655f 7061 7261 6d5f 6c61 796f 7574  one_param_layout
+00020730: 2e61 6464 5374 7265 7463 6828 3129 0a20  .addStretch(1). 
+00020740: 2020 2020 2020 206f 6e65 5f70 6172 616d         one_param
+00020750: 5f6c 6179 6f75 742e 7365 7441 6c69 676e  _layout.setAlign
+00020760: 6d65 6e74 2851 7443 6f72 652e 5174 2e41  ment(QtCore.Qt.A
+00020770: 6c69 676e 5643 656e 7465 7229 0a0a 2020  lignVCenter)..  
+00020780: 2020 2020 2020 7265 7475 726e 206f 6e65        return one
+00020790: 5f70 6172 616d 5f77 6964 6765 742c 206f  _param_widget, o
+000207a0: 6e65 5f70 6172 616d 5f6c 6179 6f75 740a  ne_param_layout.
+000207b0: 0a0a 6465 6620 696e 7465 7261 6374 6976  ..def interactiv
+000207c0: 655f 6669 7474 696e 6728 6461 7461 7365  e_fitting(datase
+000207d0: 743a 2054 6175 5444 6174 6173 6574 207c  t: TauTDataset |
+000207e0: 2054 6175 4844 6174 6173 6574 2c20 6170   TauHDataset, ap
+000207f0: 702c 0a20 2020 2020 2020 2020 2020 2020  p,.             
+00020800: 2020 2020 2020 2020 2020 206d 6f64 656c             model
+00020810: 5f6f 7074 3a20 7374 7220 7c20 6c69 7374  _opt: str | list
+00020820: 5b4c 6f67 5461 7554 4d6f 6465 6c20 7c20  [LogTauTModel | 
+00020830: 4c6f 6754 6175 484d 6f64 656c 5d20 3d20  LogTauHModel] = 
+00020840: 2766 726f 6d5f 6461 7461 7365 7427 2920  'from_dataset') 
+00020850: 2d3e 2074 7570 6c65 5b6c 6973 745b 4c6f  -> tuple[list[Lo
+00020860: 6754 6175 544d 6f64 656c 207c 204c 6f67  gTauTModel | Log
+00020870: 5461 7548 4d6f 6465 6c5d 2c20 6c69 7374  TauHModel], list
+00020880: 5b64 6963 745b 7374 722c 2066 6c6f 6174  [dict[str, float
+00020890: 5d5d 2c20 6c69 7374 5b64 6963 745b 7374  ]], list[dict[st
+000208a0: 722c 2066 6c6f 6174 5d5d 2c20 626f 6f6c  r, float]], bool
+000208b0: 5d3a 2023 206e 6f71 610a 2020 2020 2727  ]: # noqa.    ''
+000208c0: 270a 2020 2020 4372 6561 7465 7320 7174  '.    Creates qt
+000208d0: 2077 696e 646f 7720 666f 7220 7573 6572   window for user
+000208e0: 2074 6f20 696e 7465 7261 6374 6976 656c   to interactivel
+000208f0: 7920 6669 7420 6d6f 6465 6c73 2074 6f20  y fit models to 
+00020900: 7265 6c61 7861 7469 6f6e 0a20 2020 2064  relaxation.    d
+00020910: 6174 610a 0a20 2020 2050 6172 616d 6574  ata..    Paramet
+00020920: 6572 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ers.    --------
+00020930: 2d2d 0a20 2020 2064 6174 6173 6574 3a20  --.    dataset: 
+00020940: 5461 7554 4461 7461 7365 7420 7c20 5461  TauTDataset | Ta
+00020950: 7548 4461 7461 7365 740a 2020 2020 2020  uHDataset.      
+00020960: 2020 4461 7461 7365 7420 746f 2070 6c6f    Dataset to plo
+00020970: 740a 2020 2020 6170 703a 2051 7457 6964  t.    app: QtWid
+00020980: 6765 7473 2e51 4170 706c 6963 6174 696f  gets.QApplicatio
+00020990: 6e0a 2020 2020 2020 2020 4170 706c 6963  n.        Applic
+000209a0: 6174 696f 6e20 7573 6564 2062 7920 6375  ation used by cu
+000209b0: 7272 656e 7420 7072 6f67 7261 6d0a 2020  rrent program.  
+000209c0: 2020 2020 2020 4372 6561 7465 2077 6974        Create wit
+000209d0: 6820 6061 7070 3d51 7457 6964 6765 7473  h `app=QtWidgets
+000209e0: 2e51 4170 706c 6963 6174 696f 6e28 5b5d  .QApplication([]
+000209f0: 2960 0a20 2020 206d 6f64 656c 5f6f 7074  )`.    model_opt
+00020a00: 3a20 7374 7220 7c20 6c69 7374 5b4c 6f67  : str | list[Log
+00020a10: 5461 7554 4d6f 6465 6c20 7c20 4c6f 6754  TauTModel | LogT
+00020a20: 6175 484d 6f64 656c 5d20 6465 6661 756c  auHModel] defaul
+00020a30: 7420 2766 726f 6d5f 6461 7461 7365 7427  t 'from_dataset'
+00020a40: 200a 2020 2020 2020 2020 4c69 7374 206f   .        List o
+00020a50: 6620 6d6f 6465 6c73 2074 6f20 6f66 6665  f models to offe
+00020a60: 7220 746f 2075 7365 722c 2069 6620 2766  r to user, if 'f
+00020a70: 726f 6d5f 6461 7461 7365 7427 2077 696c  rom_dataset' wil
+00020a80: 6c20 6765 6e65 7261 7465 0a20 2020 2020  l generate.     
+00020a90: 2020 2061 206c 6973 7420 6261 7365 6420     a list based 
+00020aa0: 6f6e 2074 6865 2064 6174 6173 6574 2070  on the dataset p
+00020ab0: 726f 7669 6465 640a 0a20 2020 2052 6574  rovided..    Ret
+00020ac0: 7572 6e73 0a20 2020 202d 2d2d 2d2d 2d2d  urns.    -------
+00020ad0: 0a20 2020 206c 6973 745b 4c6f 6754 6175  .    list[LogTau
+00020ae0: 544d 6f64 656c 207c 204c 6f67 5461 7548  TModel | LogTauH
+00020af0: 4d6f 6465 6c5d 0a20 2020 2020 2020 204d  Model].        M
+00020b00: 6f64 656c 7320 7365 6c65 6374 6564 2062  odels selected b
+00020b10: 7920 7573 6572 0a20 2020 206c 6973 745b  y user.    list[
+00020b20: 6469 6374 5b73 7472 2c20 666c 6f61 745d  dict[str, float]
+00020b30: 5d0a 2020 2020 2020 2020 6669 745f 7661  ].        fit_va
+00020b40: 7273 2064 6963 7473 2c20 6f6e 6520 7065  rs dicts, one pe
+00020b50: 7220 6d6f 6465 6c0a 2020 2020 6c69 7374  r model.    list
+00020b60: 5b64 6963 745b 7374 722c 2066 6c6f 6174  [dict[str, float
+00020b70: 5d5d 0a20 2020 2020 2020 2066 6978 5f76  ]].        fix_v
+00020b80: 6172 7320 6469 6374 732c 206f 6e65 2070  ars dicts, one p
+00020b90: 6572 206d 6f64 656c 0a20 2020 2062 6f6f  er model.    boo
+00020ba0: 6c0a 2020 2020 2020 2020 5472 7565 2069  l.        True i
+00020bb0: 6620 7573 6572 2068 6173 2065 7869 7465  f user has exite
+00020bc0: 6420 7769 6e64 6f77 2069 6e73 7465 6164  d window instead
+00020bd0: 206f 6620 6669 7474 696e 670a 2020 2020   of fitting.    
+00020be0: 2020 2020 656c 7365 2046 616c 7365 0a20      else False. 
+00020bf0: 2020 2027 2727 2023 206e 6f71 610a 0a20     ''' # noqa.. 
+00020c00: 2020 2069 6620 6d6f 6465 6c5f 6f70 7420     if model_opt 
+00020c10: 3d3d 2027 6672 6f6d 5f64 6174 6173 6574  == 'from_dataset
+00020c20: 273a 0a20 2020 2020 2020 2069 6620 6973  ':.        if is
+00020c30: 696e 7374 616e 6365 2864 6174 6173 6574  instance(dataset
+00020c40: 2c20 5461 7554 4461 7461 7365 7429 3a0a  , TauTDataset):.
+00020c50: 2020 2020 2020 2020 2020 2020 6d6f 6465              mode
+00020c60: 6c5f 6f70 7420 3d20 5b0a 2020 2020 2020  l_opt = [.      
+00020c70: 2020 2020 2020 2020 2020 4c6f 674f 7262            LogOrb
+00020c80: 6163 684d 6f64 656c 2c0a 2020 2020 2020  achModel,.      
+00020c90: 2020 2020 2020 2020 2020 4c6f 6752 616d            LogRam
+00020ca0: 616e 4d6f 6465 6c2c 0a20 2020 2020 2020  anModel,.       
+00020cb0: 2020 2020 2020 2020 204c 6f67 5154 4d4d           LogQTMM
+00020cc0: 6f64 656c 2c0a 2020 2020 2020 2020 2020  odel,.          
+00020cd0: 2020 2020 2020 4c6f 6744 6972 6563 744d        LogDirectM
+00020ce0: 6f64 656c 0a20 2020 2020 2020 2020 2020  odel.           
+00020cf0: 205d 0a20 2020 2020 2020 2065 6c69 6620   ].        elif 
+00020d00: 6973 696e 7374 616e 6365 2864 6174 6173  isinstance(datas
+00020d10: 6574 2c20 5461 7548 4461 7461 7365 7429  et, TauHDataset)
+00020d20: 3a0a 2020 2020 2020 2020 2020 2020 6d6f  :.            mo
+00020d30: 6465 6c5f 6f70 7420 3d20 5b0a 2020 2020  del_opt = [.    
+00020d40: 2020 2020 2020 2020 2020 2020 4c6f 6746              LogF
+00020d50: 4451 544d 4d6f 6465 6c2c 0a20 2020 2020  DQTMModel,.     
+00020d60: 2020 2020 2020 2020 2020 204c 6f67 5261             LogRa
+00020d70: 6d61 6e49 494d 6f64 656c 2c0a 2020 2020  manIIModel,.    
+00020d80: 2020 2020 2020 2020 2020 2020 4c6f 6742              LogB
+00020d90: 5656 5261 6d61 6e49 494d 6f64 656c 2c0a  VVRamanIIModel,.
+00020da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020db0: 4c6f 6743 6f6e 7374 616e 744d 6f64 656c  LogConstantModel
+00020dc0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00020dd0: 2020 4c6f 6742 5656 436f 6e73 7461 6e74    LogBVVConstant
+00020de0: 4d6f 6465 6c2c 0a20 2020 2020 2020 2020  Model,.         
+00020df0: 2020 205d 0a0a 2020 2020 7573 656c 203d     ]..    usel =
+00020e00: 2074 7970 6528 276f 626a 272c 2028 6f62   type('obj', (ob
+00020e10: 6a65 6374 2c29 2c20 7b0a 2020 2020 2020  ject,), {.      
+00020e20: 2020 276d 6f64 656c 7327 3a20 7b0a 2020    'models': {.  
+00020e30: 2020 2020 2020 2020 2020 6d6f 6465 6c2e            model.
+00020e40: 4e41 4d45 2e6c 6f77 6572 2829 3a20 4661  NAME.lower(): Fa
+00020e50: 6c73 650a 2020 2020 2020 2020 2020 2020  lse.            
+00020e60: 666f 7220 6d6f 6465 6c20 696e 206d 6f64  for model in mod
+00020e70: 656c 5f6f 7074 0a20 2020 2020 2020 207d  el_opt.        }
+00020e80: 2c0a 2020 2020 2020 2020 2766 6974 5f76  ,.        'fit_v
+00020e90: 6172 7327 3a20 5b5d 2c0a 2020 2020 2020  ars': [],.      
+00020ea0: 2020 2766 6978 5f76 6172 7327 3a20 5b5d    'fix_vars': []
+00020eb0: 2c0a 2020 2020 2020 2020 2766 6978 273a  ,.        'fix':
+00020ec0: 205b 5d2c 0a20 2020 2020 2020 2027 6578   [],.        'ex
+00020ed0: 6974 6564 273a 2054 7275 650a 2020 2020  ited': True.    
+00020ee0: 7d29 0a0a 2020 2020 7061 7261 6d5f 7769  })..    param_wi
+00020ef0: 6e64 6f77 203d 2046 6974 5769 6e64 6f77  ndow = FitWindow
+00020f00: 280a 2020 2020 2020 2020 6461 7461 7365  (.        datase
+00020f10: 742c 0a20 2020 2020 2020 2075 7365 6c2c  t,.        usel,
+00020f20: 0a20 2020 2020 2020 206d 6f64 656c 5f6f  .        model_o
+00020f30: 7074 2c0a 2020 2020 2020 2020 6775 692e  pt,.        gui.
+00020f40: 7769 6467 6574 5f64 6566 6175 6c74 730a  widget_defaults.
+00020f50: 2020 2020 290a 2020 2020 7061 7261 6d5f      ).    param_
+00020f60: 7769 6e64 6f77 2e73 686f 7728 290a 0a20  window.show().. 
+00020f70: 2020 2061 7070 2e65 7865 6328 290a 0a20     app.exec().. 
+00020f80: 2020 206e 616d 655f 746f 5f6d 6f64 656c     name_to_model
+00020f90: 203d 207b 0a20 2020 2020 2020 206d 6f64   = {.        mod
+00020fa0: 656c 2e4e 414d 452e 6c6f 7765 7228 293a  el.NAME.lower():
+00020fb0: 206d 6f64 656c 0a20 2020 2020 2020 2066   model.        f
+00020fc0: 6f72 206d 6f64 656c 2069 6e20 6d6f 6465  or model in mode
+00020fd0: 6c5f 6f70 740a 2020 2020 7d0a 0a20 2020  l_opt.    }..   
+00020fe0: 2072 5f6d 6f64 656c 7320 3d20 5b0a 2020   r_models = [.  
+00020ff0: 2020 2020 2020 6e61 6d65 5f74 6f5f 6d6f        name_to_mo
+00021000: 6465 6c5b 6e61 6d65 5d0a 2020 2020 2020  del[name].      
+00021010: 2020 666f 7220 6e61 6d65 2069 6e20 7573    for name in us
+00021020: 656c 2e6d 6f64 656c 730a 2020 2020 5d0a  el.models.    ].
+00021030: 0a20 2020 2072 6574 7572 6e20 725f 6d6f  .    return r_mo
+00021040: 6465 6c73 2c20 7573 656c 2e66 6974 5f76  dels, usel.fit_v
+00021050: 6172 732c 2075 7365 6c2e 6669 785f 7661  ars, usel.fix_va
+00021060: 7273 2c20 7573 656c 2e65 7869 7465 640a  rs, usel.exited.
+00021070: 0a0a 6465 6620 706c 6f74 5f66 6974 7465  ..def plot_fitte
+00021080: 645f 7469 6d65 7328 6461 7461 7365 743a  d_times(dataset:
+00021090: 2054 6175 5444 6174 6173 6574 207c 2054   TauTDataset | T
+000210a0: 6175 4844 6174 6173 6574 2c0a 2020 2020  auHDataset,.    
+000210b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000210c0: 2020 6d6f 6465 6c3a 204c 6f67 5461 7554    model: LogTauT
+000210d0: 4d6f 6465 6c20 7c20 4d75 6c74 694c 6f67  Model | MultiLog
+000210e0: 5461 7554 4d6f 6465 6c20 7c20 4c6f 6754  TauTModel | LogT
+000210f0: 6175 484d 6f64 656c 207c 204d 756c 7469  auHModel | Multi
+00021100: 4c6f 6754 6175 484d 6f64 656c 2c20 2320  LogTauHModel, # 
+00021110: 6e6f 7161 0a20 2020 2020 2020 2020 2020  noqa.           
+00021120: 2020 2020 2020 2020 2020 2073 686f 773a             show:
+00021130: 2062 6f6f 6c20 3d20 5472 7565 2c20 7361   bool = True, sa
+00021140: 7665 3a20 626f 6f6c 203d 2046 616c 7365  ve: bool = False
+00021150: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00021160: 2020 2020 2020 2020 7361 7665 5f6e 616d          save_nam
+00021170: 653a 2073 7472 203d 2027 6669 7474 6564  e: str = 'fitted
+00021180: 5f72 6174 6573 2e70 6e67 272c 0a20 2020  _rates.png',.   
+00021190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000211a0: 2020 2076 6572 626f 7365 3a20 626f 6f6c     verbose: bool
+000211b0: 203d 2054 7275 6529 202d 3e20 7475 706c   = True) -> tupl
+000211c0: 655b 706c 742e 4669 6775 7265 2c20 706c  e[plt.Figure, pl
+000211d0: 742e 4178 6573 5d3a 0a20 2020 2027 2727  t.Axes]:.    '''
+000211e0: 0a20 2020 2050 6c6f 7473 2065 7870 6572  .    Plots exper
+000211f0: 696d 656e 7461 6c20 616e 6420 6669 7474  imental and fitt
+00021200: 6564 2028 6d6f 6465 6c29 2072 656c 6178  ed (model) relax
+00021210: 6174 696f 6e20 7261 7465 2061 735c 6e0a  ation rate as\n.
+00021220: 2020 2020 6c6e 2874 6175 2920 7673 2031      ln(tau) vs 1
+00021230: 2f78 7661 7220 7768 6572 6520 7876 6172  /xvar where xvar
+00021240: 2069 7320 5420 6f72 2048 2e0a 0a20 2020   is T or H...   
+00021250: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
+00021260: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2064  ----------.    d
+00021270: 6174 6173 6574 3a20 5461 7554 4461 7461  ataset: TauTData
+00021280: 7365 7420 7c20 5461 7548 4461 7461 7365  set | TauHDatase
+00021290: 740a 2020 2020 2020 2020 4461 7461 7365  t.        Datase
+000212a0: 7420 746f 2070 6c6f 740a 2020 2020 6d6f  t to plot.    mo
+000212b0: 6465 6c3a 204c 6f67 5461 7554 4d6f 6465  del: LogTauTMode
+000212c0: 6c20 7c20 4d75 6c74 694c 6f67 5461 7554  l | MultiLogTauT
+000212d0: 4d6f 6465 6c20 7c20 4c6f 6754 6175 484d  Model | LogTauHM
+000212e0: 6f64 656c 207c 204d 756c 7469 4c6f 6754  odel | MultiLogT
+000212f0: 6175 484d 6f64 656c 0a20 2020 2020 2020  auHModel.       
+00021300: 204d 6f64 656c 2028 6669 7474 6564 2920   Model (fitted) 
+00021310: 746f 2070 6c6f 740a 2020 2020 7368 6f77  to plot.    show
+00021320: 3a20 626f 6f6c 2c20 6465 6661 756c 7420  : bool, default 
+00021330: 5472 7565 0a20 2020 2020 2020 2049 6620  True.        If 
+00021340: 5472 7565 2c20 7368 6f77 2070 6c6f 7420  True, show plot 
+00021350: 6f6e 2073 6372 6565 6e0a 2020 2020 7361  on screen.    sa
+00021360: 7665 3a20 626f 6f6c 2c20 6465 6661 756c  ve: bool, defaul
+00021370: 7420 4661 6c73 650a 2020 2020 2020 2020  t False.        
+00021380: 4966 2054 7275 652c 2073 6176 6520 706c  If True, save pl
+00021390: 6f74 2074 6f20 6669 6c65 2060 7361 7665  ot to file `save
+000213a0: 5f6e 616d 6560 0a20 2020 2073 6176 655f  _name`.    save_
+000213b0: 6e61 6d65 3a20 7374 722c 2064 6566 6175  name: str, defau
+000213c0: 6c74 203d 2027 6669 7474 6564 5f72 6174  lt = 'fitted_rat
+000213d0: 6573 2e70 6e67 270a 2020 2020 2020 2020  es.png'.        
+000213e0: 4966 2073 6176 6520 6973 2054 7275 652c  If save is True,
+000213f0: 2077 696c 6c20 7361 7665 2070 6c6f 7420   will save plot 
+00021400: 746f 2074 6869 7320 6669 6c65 6e61 6d65  to this filename
+00021410: 0a20 2020 2076 6572 626f 7365 3a20 626f  .    verbose: bo
+00021420: 6f6c 2c20 6465 6661 756c 7420 5472 7565  ol, default True
+00021430: 0a20 2020 2020 2020 2049 6620 5472 7565  .        If True
+00021440: 2c20 706c 6f74 2066 696c 6520 6c6f 6361  , plot file loca
+00021450: 7469 6f6e 2069 7320 7772 6974 7465 6e20  tion is written 
+00021460: 746f 2074 6572 6d69 6e61 6c0a 2020 2020  to terminal.    
+00021470: 5265 7475 726e 730a 2020 2020 2d2d 2d2d  Returns.    ----
+00021480: 2d2d 2d0a 2020 2020 706c 742e 4669 6775  ---.    plt.Figu
+00021490: 7265 0a20 2020 2020 2020 204d 6174 706c  re.        Matpl
+000214a0: 6f74 6c69 6220 6669 6775 7265 206f 626a  otlib figure obj
+000214b0: 6563 740a 2020 2020 706c 742e 4178 6573  ect.    plt.Axes
+000214c0: 0a20 2020 2020 2020 204d 6174 706c 6f74  .        Matplot
+000214d0: 6c69 6220 6178 6973 206f 626a 6563 740a  lib axis object.
+000214e0: 2020 2020 2727 270a 0a20 2020 2023 2043      '''..    # C
+000214f0: 7265 6174 6520 6669 6775 7265 2061 6e64  reate figure and
+00021500: 2061 7865 730a 2020 2020 6669 672c 2061   axes.    fig, a
+00021510: 7820 3d20 706c 742e 7375 6270 6c6f 7473  x = plt.subplots
+00021520: 280a 2020 2020 2020 2020 312c 0a20 2020  (.        1,.   
+00021530: 2020 2020 2031 2c0a 2020 2020 2020 2020       1,.        
+00021540: 7368 6172 6578 3d54 7275 652c 0a20 2020  sharex=True,.   
+00021550: 2020 2020 2073 6861 7265 793d 5472 7565       sharey=True
+00021560: 2c0a 2020 2020 2020 2020 6669 6773 697a  ,.        figsiz
+00021570: 653d 2836 2c20 3629 2c0a 2020 2020 2020  e=(6, 6),.      
+00021580: 2020 6e75 6d3d 2746 6974 7465 6420 7265    num='Fitted re
+00021590: 6c61 7861 7469 6f6e 2070 726f 6669 6c65  laxation profile
+000215a0: 270a 2020 2020 290a 0a20 2020 205f 706c  '.    )..    _pl
+000215b0: 6f74 5f66 6974 7465 645f 7469 6d65 7328  ot_fitted_times(
+000215c0: 6461 7461 7365 742c 206d 6f64 656c 2c20  dataset, model, 
+000215d0: 6669 672c 2061 7829 0a0a 2020 2020 6669  fig, ax)..    fi
+000215e0: 672e 7469 6768 745f 6c61 796f 7574 2829  g.tight_layout()
+000215f0: 0a0a 2020 2020 6966 2073 686f 773a 0a20  ..    if show:. 
+00021600: 2020 2020 2020 2070 6c74 2e73 686f 7728         plt.show(
+00021610: 290a 0a20 2020 2069 6620 7361 7665 3a0a  )..    if save:.
+00021620: 2020 2020 2020 2020 6669 672e 7361 7665          fig.save
+00021630: 6669 6728 7361 7665 5f6e 616d 652c 2064  fig(save_name, d
+00021640: 7069 3d35 3030 290a 2020 2020 2020 2020  pi=500).        
+00021650: 6966 2076 6572 626f 7365 3a0a 2020 2020  if verbose:.    
+00021660: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
+00021670: 7461 6e63 6528 6461 7461 7365 742c 2028  tance(dataset, (
+00021680: 5461 7554 4461 7461 7365 7429 293a 0a20  TauTDataset)):. 
+00021690: 2020 2020 2020 2020 2020 2020 2020 205f                 _
+000216a0: 7876 6172 203d 2027 5427 0a20 2020 2020  xvar = 'T'.     
+000216b0: 2020 2020 2020 2065 6c69 6620 6973 696e         elif isin
+000216c0: 7374 616e 6365 2864 6174 6173 6574 2c20  stance(dataset, 
+000216d0: 2854 6175 4844 6174 6173 6574 2929 3a0a  (TauHDataset)):.
+000216e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000216f0: 5f78 7661 7220 3d20 2748 270a 2020 2020  _xvar = 'H'.    
+00021700: 2020 2020 2020 2020 7574 2e63 7072 696e          ut.cprin
+00021710: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
+00021720: 2020 2066 275c 6e20 4669 7474 6564 206c     f'\n Fitted l
+00021730: 6e28 cf84 2920 7673 2031 2f7b 5f78 7661  n(..) vs 1/{_xva
+00021740: 727d 2070 6c6f 7420 7361 7665 6420 746f  r} plot saved to
+00021750: 205c 6e20 7b73 6176 655f 6e61 6d65 7d5c   \n {save_name}\
+00021760: 6e27 2c20 2320 6e6f 7161 0a20 2020 2020  n', # noqa.     
+00021770: 2020 2020 2020 2020 2020 2027 6379 616e             'cyan
+00021780: 270a 2020 2020 2020 2020 2020 2020 290a  '.            ).
+00021790: 0a20 2020 2072 6574 7572 6e20 6669 672c  .    return fig,
+000217a0: 2061 780a 0a0a 6465 6620 706c 6f74 5f74   ax...def plot_t
+000217b0: 696d 6573 2864 6174 6173 6574 3a20 5461  imes(dataset: Ta
+000217c0: 7554 4461 7461 7365 7420 7c20 5461 7548  uTDataset | TauH
+000217d0: 4461 7461 7365 742c 2073 686f 773a 2062  Dataset, show: b
+000217e0: 6f6f 6c20 3d20 5472 7565 2c0a 2020 2020  ool = True,.    
+000217f0: 2020 2020 2020 2020 2020 2073 6176 653a             save:
+00021800: 2062 6f6f 6c20 3d20 4661 6c73 652c 2073   bool = False, s
+00021810: 6176 655f 6e61 6d65 3a20 7374 7220 3d20  ave_name: str = 
+00021820: 2772 656c 6178 6174 696f 6e5f 7469 6d65  'relaxation_time
+00021830: 732e 706e 6727 2c0a 2020 2020 2020 2020  s.png',.        
+00021840: 2020 2020 2020 2076 6572 626f 7365 3a20         verbose: 
+00021850: 626f 6f6c 203d 2054 7275 6529 202d 3e20  bool = True) -> 
+00021860: 7475 706c 655b 706c 742e 4669 6775 7265  tuple[plt.Figure
+00021870: 2c20 706c 742e 4178 6573 5d3a 0a20 2020  , plt.Axes]:.   
+00021880: 2027 2727 0a20 2020 2050 6c6f 7473 2065   '''.    Plots e
+00021890: 7870 6572 696d 656e 7461 6c20 7265 6c61  xperimental rela
+000218a0: 7861 7469 6f6e 2074 696d 6520 6173 5c6e  xation time as\n
+000218b0: 0a20 2020 206c 6e28 7461 7529 2076 7320  .    ln(tau) vs 
+000218c0: 312f 7876 6172 2077 6865 7265 2078 7661  1/xvar where xva
+000218d0: 7220 6973 2054 206f 7220 482e 0a0a 2020  r is T or H...  
+000218e0: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+000218f0: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+00021900: 6461 7461 7365 743a 2054 6175 5444 6174  dataset: TauTDat
+00021910: 6173 6574 207c 2054 6175 4844 6174 6173  aset | TauHDatas
+00021920: 6574 0a20 2020 2020 2020 2044 6174 6173  et.        Datas
+00021930: 6574 2074 6f20 706c 6f74 0a20 2020 2073  et to plot.    s
+00021940: 686f 773a 2062 6f6f 6c2c 2064 6566 6175  how: bool, defau
+00021950: 6c74 2054 7275 650a 2020 2020 2020 2020  lt True.        
+00021960: 4966 2054 7275 652c 2073 686f 7720 706c  If True, show pl
+00021970: 6f74 206f 6e20 7363 7265 656e 0a20 2020  ot on screen.   
+00021980: 2073 6176 653a 2062 6f6f 6c2c 2064 6566   save: bool, def
+00021990: 6175 6c74 2046 616c 7365 0a20 2020 2020  ault False.     
+000219a0: 2020 2049 6620 5472 7565 2c20 7361 7665     If True, save
+000219b0: 2070 6c6f 7420 746f 2066 696c 6520 6073   plot to file `s
+000219c0: 6176 655f 6e61 6d65 600a 2020 2020 7361  ave_name`.    sa
+000219d0: 7665 5f6e 616d 653a 2073 7472 2c20 6465  ve_name: str, de
+000219e0: 6661 756c 7420 2772 656c 6178 6174 696f  fault 'relaxatio
+000219f0: 6e5f 7469 6d65 732e 706e 6727 0a20 2020  n_times.png'.   
+00021a00: 2020 2020 2049 6620 7361 7665 2069 7320       If save is 
+00021a10: 5472 7565 2c20 7769 6c6c 2073 6176 6520  True, will save 
+00021a20: 706c 6f74 2074 6f20 7468 6973 2066 696c  plot to this fil
+00021a30: 656e 616d 650a 2020 2020 7665 7262 6f73  ename.    verbos
+00021a40: 653a 2062 6f6f 6c2c 2064 6566 6175 6c74  e: bool, default
+00021a50: 2054 7275 650a 2020 2020 2020 2020 4966   True.        If
+00021a60: 2054 7275 652c 2070 6c6f 7420 6669 6c65   True, plot file
+00021a70: 206c 6f63 6174 696f 6e20 6973 2077 7269   location is wri
+00021a80: 7474 656e 2074 6f20 7465 726d 696e 616c  tten to terminal
+00021a90: 0a0a 2020 2020 5265 7475 726e 730a 2020  ..    Returns.  
+00021aa0: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 706c    -------.    pl
+00021ab0: 742e 4669 6775 7265 0a20 2020 2020 2020  t.Figure.       
+00021ac0: 204d 6174 706c 6f74 6c69 6220 6669 6775   Matplotlib figu
+00021ad0: 7265 206f 626a 6563 740a 2020 2020 706c  re object.    pl
+00021ae0: 742e 4178 6573 0a20 2020 2020 2020 204d  t.Axes.        M
+00021af0: 6174 706c 6f74 6c69 6220 6178 6973 206f  atplotlib axis o
+00021b00: 626a 6563 740a 2020 2020 2727 270a 0a20  bject.    '''.. 
+00021b10: 2020 2023 2043 7265 6174 6520 6669 6775     # Create figu
+00021b20: 7265 2061 6e64 2061 7865 730a 2020 2020  re and axes.    
+00021b30: 6669 672c 2061 7820 3d20 706c 742e 7375  fig, ax = plt.su
+00021b40: 6270 6c6f 7473 280a 2020 2020 2020 2020  bplots(.        
+00021b50: 312c 0a20 2020 2020 2020 2031 2c0a 2020  1,.        1,.  
+00021b60: 2020 2020 2020 7368 6172 6578 3d54 7275        sharex=Tru
+00021b70: 652c 0a20 2020 2020 2020 2073 6861 7265  e,.        share
+00021b80: 793d 5472 7565 2c0a 2020 2020 2020 2020  y=True,.        
+00021b90: 6669 6773 697a 653d 2836 2c20 3629 2c0a  figsize=(6, 6),.
+00021ba0: 2020 2020 2020 2020 6e75 6d3d 2746 6974          num='Fit
+00021bb0: 7465 6420 7265 6c61 7861 7469 6f6e 2070  ted relaxation p
+00021bc0: 726f 6669 6c65 270a 2020 2020 290a 0a20  rofile'.    ).. 
+00021bd0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+00021be0: 2864 6174 6173 6574 2c20 5461 7548 4461  (dataset, TauHDa
+00021bf0: 7461 7365 7429 3a0a 2020 2020 2020 2020  taset):.        
+00021c00: 785f 7661 6c73 203d 2064 6174 6173 6574  x_vals = dataset
+00021c10: 2e66 6965 6c64 730a 2020 2020 2020 2020  .fields.        
+00021c20: 6178 2e73 6574 5f78 6c61 6265 6c28 7227  ax.set_xlabel(r'
+00021c30: 312f 4820 245c 6c65 6674 285c 6d61 7468  1/H $\left(\math
+00021c40: 7265 6775 6c61 727b 4f65 7d5e 5c6d 6174  regular{Oe}^\mat
+00021c50: 6872 6567 756c 6172 7b2d 317d 5c72 6967  hregular{-1}\rig
+00021c60: 6874 2924 2729 0a20 2020 2065 6c69 6620  ht)$').    elif 
+00021c70: 6973 696e 7374 616e 6365 2864 6174 6173  isinstance(datas
+00021c80: 6574 2c20 5461 7554 4461 7461 7365 7429  et, TauTDataset)
+00021c90: 3a0a 2020 2020 2020 2020 785f 7661 6c73  :.        x_vals
+00021ca0: 203d 2064 6174 6173 6574 2e74 656d 7065   = dataset.tempe
+00021cb0: 7261 7475 7265 730a 2020 2020 2020 2020  ratures.        
+00021cc0: 6178 2e73 6574 5f78 6c61 6265 6c28 7227  ax.set_xlabel(r'
+00021cd0: 312f 5420 245c 6c65 6674 285c 6d61 7468  1/T $\left(\math
+00021ce0: 7265 6775 6c61 727b 4b7d 5e5c 6d61 7468  regular{K}^\math
+00021cf0: 7265 6775 6c61 727b 2d31 7d5c 7269 6768  regular{-1}\righ
+00021d00: 7429 2427 290a 0a20 2020 2023 2041 6464  t)$')..    # Add
+00021d10: 2075 6e63 6572 7461 696e 7469 6573 2061   uncertainties a
+00021d20: 7320 6572 726f 7262 6172 730a 2020 2020  s errorbars.    
+00021d30: 6966 206c 656e 2864 6174 6173 6574 2e72  if len(dataset.r
+00021d40: 6174 655f 706d 293a 0a0a 2020 2020 2020  ate_pm):..      
+00021d50: 2020 2320 4361 6c63 756c 6174 6520 7469    # Calculate ti
+00021d60: 6d65 2065 7272 6f72 6261 7273 0a20 2020  me errorbars.   
+00021d70: 2020 2020 2074 696d 6573 203d 2031 2e20       times = 1. 
+00021d80: 2f20 6461 7461 7365 742e 7261 7465 730a  / dataset.rates.
+00021d90: 2020 2020 2020 2020 6d69 6e5f 7469 6d65          min_time
+00021da0: 203d 2031 2e20 2f20 2864 6174 6173 6574   = 1. / (dataset
+00021db0: 2e72 6174 6573 202b 2064 6174 6173 6574  .rates + dataset
+00021dc0: 2e72 6174 655f 706d 5b31 2c20 3a5d 290a  .rate_pm[1, :]).
+00021dd0: 2020 2020 2020 2020 6d61 785f 7469 6d65          max_time
+00021de0: 203d 2031 2e20 2f20 2864 6174 6173 6574   = 1. / (dataset
+00021df0: 2e72 6174 6573 202d 2064 6174 6173 6574  .rates - dataset
+00021e00: 2e72 6174 655f 706d 5b30 2c20 3a5d 290a  .rate_pm[0, :]).
+00021e10: 0a20 2020 2020 2020 206c 6e5f 6d69 6e5f  .        ln_min_
+00021e20: 7469 6d65 203d 206e 702e 6c6f 6728 6d69  time = np.log(mi
+00021e30: 6e5f 7469 6d65 290a 2020 2020 2020 2020  n_time).        
+00021e40: 6c6e 5f6d 6178 5f74 696d 6520 3d20 6e70  ln_max_time = np
+00021e50: 2e6c 6f67 286d 6178 5f74 696d 6529 0a0a  .log(max_time)..
+00021e60: 2020 2020 2020 2020 6c6e 5f74 696d 655f          ln_time_
+00021e70: 706c 7573 203d 206c 6e5f 6d61 785f 7469  plus = ln_max_ti
+00021e80: 6d65 202d 206e 702e 6c6f 6728 7469 6d65  me - np.log(time
+00021e90: 7329 0a20 2020 2020 2020 206c 6e5f 7469  s).        ln_ti
+00021ea0: 6d65 5f6d 696e 7573 203d 206e 702e 6c6f  me_minus = np.lo
+00021eb0: 6728 7469 6d65 7329 202d 206c 6e5f 6d69  g(times) - ln_mi
+00021ec0: 6e5f 7469 6d65 0a0a 2020 2020 2020 2020  n_time..        
+00021ed0: 6c6e 7469 6d65 5f6d 7020 3d20 6e70 2e61  lntime_mp = np.a
+00021ee0: 7272 6179 285b 6c6e 5f74 696d 655f 6d69  rray([ln_time_mi
+00021ef0: 6e75 732c 206c 6e5f 7469 6d65 5f70 6c75  nus, ln_time_plu
+00021f00: 735d 290a 0a20 2020 2020 2020 2061 782e  s])..        ax.
+00021f10: 6572 726f 7262 6172 280a 2020 2020 2020  errorbar(.      
+00021f20: 2020 2020 2020 312e 202f 2078 5f76 616c        1. / x_val
+00021f30: 732c 0a20 2020 2020 2020 2020 2020 206e  s,.            n
+00021f40: 702e 6c6f 6728 7469 6d65 7329 2c0a 2020  p.log(times),.  
+00021f50: 2020 2020 2020 2020 2020 7965 7272 3d6c            yerr=l
+00021f60: 6e74 696d 655f 6d70 2c0a 2020 2020 2020  ntime_mp,.      
+00021f70: 2020 2020 2020 6d61 726b 6572 3d27 6f27        marker='o'
+00021f80: 2c0a 2020 2020 2020 2020 2020 2020 6c77  ,.            lw
+00021f90: 3d30 2c0a 2020 2020 2020 2020 2020 2020  =0,.            
+00021fa0: 656c 696e 6577 6964 7468 3d31 2e35 2c0a  elinewidth=1.5,.
+00021fb0: 2020 2020 2020 2020 2020 2020 6669 6c6c              fill
+00021fc0: 7374 796c 653d 276e 6f6e 6527 2c0a 2020  style='none',.  
+00021fd0: 2020 2020 2020 2020 2020 636f 6c6f 723d            color=
+00021fe0: 2762 6c61 636b 270a 2020 2020 2020 2020  'black'.        
+00021ff0: 290a 2020 2020 656c 7365 3a0a 2020 2020  ).    else:.    
+00022000: 2020 2020 6178 2e70 6c6f 7428 0a20 2020      ax.plot(.   
+00022010: 2020 2020 2020 2020 2031 2e20 2f20 785f           1. / x_
+00022020: 7661 6c73 2c0a 2020 2020 2020 2020 2020  vals,.          
+00022030: 2020 6e70 2e6c 6f67 2831 2e20 2f20 6461    np.log(1. / da
+00022040: 7461 7365 742e 7261 7465 7329 2c0a 2020  taset.rates),.  
+00022050: 2020 2020 2020 2020 2020 6d61 726b 6572            marker
+00022060: 3d27 6f27 2c0a 2020 2020 2020 2020 2020  ='o',.          
+00022070: 2020 6c77 3d30 2c0a 2020 2020 2020 2020    lw=0,.        
+00022080: 2020 2020 6669 6c6c 7374 796c 653d 276e      fillstyle='n
+00022090: 6f6e 6527 2c0a 2020 2020 2020 2020 2020  one',.          
+000220a0: 2020 636f 6c6f 723d 2762 6c61 636b 270a    color='black'.
+000220b0: 2020 2020 2020 2020 290a 0a20 2020 2023          )..    #
+000220c0: 2045 6e61 626c 6520 6d69 6e6f 7220 7469   Enable minor ti
+000220d0: 636b 730a 2020 2020 6178 2e79 6178 6973  cks.    ax.yaxis
+000220e0: 2e73 6574 5f6d 696e 6f72 5f6c 6f63 6174  .set_minor_locat
+000220f0: 6f72 2841 7574 6f4d 696e 6f72 4c6f 6361  or(AutoMinorLoca
+00022100: 746f 7228 2929 0a20 2020 2061 782e 7861  tor()).    ax.xa
+00022110: 7869 732e 7365 745f 6d69 6e6f 725f 6c6f  xis.set_minor_lo
+00022120: 6361 746f 7228 4175 746f 4d69 6e6f 724c  cator(AutoMinorL
+00022130: 6f63 6174 6f72 2829 290a 0a20 2020 2061  ocator())..    a
+00022140: 782e 7365 745f 796c 6162 656c 2872 2724  x.set_ylabel(r'$
+00022150: 5c6c 6e5c 6c65 6674 5b5c 7461 755c 7269  \ln\left[\tau\ri
+00022160: 6768 745d 2420 245c 6c65 6674 285c 6c6e  ght]$ $\left(\ln
+00022170: 5c6c 6566 745b 5c6d 6174 6872 6567 756c  \left[\mathregul
+00022180: 6172 7b73 7d5e 5c6d 6174 6872 6567 756c  ar{s}^\mathregul
+00022190: 6172 7b2d 317d 5c72 6967 6874 5d5c 7269  ar{-1}\right]\ri
+000221a0: 6768 7429 2427 2920 2320 6e6f 7161 0a0a  ght)$') # noqa..
+000221b0: 2020 2020 6669 672e 7469 6768 745f 6c61      fig.tight_la
+000221c0: 796f 7574 2829 0a0a 2020 2020 6966 2073  yout()..    if s
+000221d0: 686f 773a 0a20 2020 2020 2020 2070 6c74  how:.        plt
+000221e0: 2e73 686f 7728 290a 0a20 2020 2069 6620  .show()..    if 
+000221f0: 7361 7665 3a0a 2020 2020 2020 2020 6669  save:.        fi
+00022200: 672e 7361 7665 6669 6728 7361 7665 5f6e  g.savefig(save_n
+00022210: 616d 652c 2064 7069 3d35 3030 290a 2020  ame, dpi=500).  
+00022220: 2020 2020 2020 6966 2076 6572 626f 7365        if verbose
+00022230: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+00022240: 2069 7369 6e73 7461 6e63 6528 6461 7461   isinstance(data
+00022250: 7365 742c 2028 5461 7554 4461 7461 7365  set, (TauTDatase
+00022260: 7429 293a 0a20 2020 2020 2020 2020 2020  t)):.           
+00022270: 2020 2020 205f 7876 6172 203d 2027 5427       _xvar = 'T'
+00022280: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
+00022290: 6620 6973 696e 7374 616e 6365 2864 6174  f isinstance(dat
+000222a0: 6173 6574 2c20 2854 6175 4844 6174 6173  aset, (TauHDatas
+000222b0: 6574 2929 3a0a 2020 2020 2020 2020 2020  et)):.          
+000222c0: 2020 2020 2020 5f78 7661 7220 3d20 2748        _xvar = 'H
+000222d0: 270a 2020 2020 2020 2020 2020 2020 7574  '.            ut
+000222e0: 2e63 7072 696e 7428 0a20 2020 2020 2020  .cprint(.       
+000222f0: 2020 2020 2020 2020 2066 275c 6e20 4669           f'\n Fi
+00022300: 7474 6564 206c 6e28 7461 7529 2076 7320  tted ln(tau) vs 
+00022310: 312f 7b5f 7876 6172 7d20 706c 6f74 2073  1/{_xvar} plot s
+00022320: 6176 6564 2074 6f20 5c6e 207b 7361 7665  aved to \n {save
+00022330: 5f6e 616d 657d 5c6e 272c 2023 206e 6f71  _name}\n', # noq
+00022340: 610a 2020 2020 2020 2020 2020 2020 2020  a.              
+00022350: 2020 2763 7961 6e27 0a20 2020 2020 2020    'cyan'.       
+00022360: 2020 2020 2029 0a0a 2020 2020 7265 7475       )..    retu
+00022370: 726e 2066 6967 2c20 6178 0a0a 0a64 6566  rn fig, ax...def
+00022380: 205f 706c 6f74 5f66 6974 7465 645f 7469   _plot_fitted_ti
+00022390: 6d65 7328 6461 7461 7365 743a 2054 6175  mes(dataset: Tau
+000223a0: 5444 6174 6173 6574 207c 2054 6175 4844  TDataset | TauHD
+000223b0: 6174 6173 6574 2c0a 2020 2020 2020 2020  ataset,.        
+000223c0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+000223d0: 6f64 656c 3a20 4c6f 6754 6175 544d 6f64  odel: LogTauTMod
+000223e0: 656c 207c 204d 756c 7469 4c6f 6754 6175  el | MultiLogTau
+000223f0: 544d 6f64 656c 207c 204c 6f67 5461 7548  TModel | LogTauH
+00022400: 4d6f 6465 6c20 7c20 4d75 6c74 694c 6f67  Model | MultiLog
+00022410: 5461 7548 4d6f 6465 6c2c 2023 206e 6f71  TauHModel, # noq
+00022420: 610a 2020 2020 2020 2020 2020 2020 2020  a.              
+00022430: 2020 2020 2020 2020 2066 6967 3a20 706c           fig: pl
+00022440: 742e 4669 6775 7265 2c20 6178 3a20 706c  t.Figure, ax: pl
+00022450: 742e 4178 6573 293a 0a20 2020 2027 2727  t.Axes):.    '''
+00022460: 0a20 2020 2050 6c6f 7473 2065 7870 6572  .    Plots exper
+00022470: 696d 656e 7461 6c20 616e 6420 6669 7474  imental and fitt
+00022480: 6564 2028 6d6f 6465 6c29 2072 656c 6178  ed (model) relax
+00022490: 6174 696f 6e20 7261 7465 2061 735c 6e0a  ation rate as\n.
+000224a0: 2020 2020 6c6e 2874 6175 2920 7673 2031      ln(tau) vs 1
+000224b0: 2f78 7661 7220 7768 6572 6520 7876 6172  /xvar where xvar
+000224c0: 2069 7320 5420 6f72 2048 2e0a 0a20 2020   is T or H...   
+000224d0: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
+000224e0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2064  ----------.    d
+000224f0: 6174 6173 6574 3a20 5461 7554 4461 7461  ataset: TauTData
+00022500: 7365 7420 7c20 5461 7548 4461 7461 7365  set | TauHDatase
+00022510: 740a 2020 2020 2020 2020 4461 7461 7365  t.        Datase
+00022520: 7420 746f 2070 6c6f 740a 2020 2020 6d6f  t to plot.    mo
+00022530: 6465 6c3a 204c 6f67 5461 7554 4d6f 6465  del: LogTauTMode
+00022540: 6c20 7c20 4d75 6c74 694c 6f67 5461 7554  l | MultiLogTauT
+00022550: 4d6f 6465 6c20 7c20 4c6f 6754 6175 484d  Model | LogTauHM
+00022560: 6f64 656c 207c 204d 756c 7469 4c6f 6754  odel | MultiLogT
+00022570: 6175 484d 6f64 656c 0a20 2020 2020 2020  auHModel.       
+00022580: 204d 6f64 656c 2028 6669 7474 6564 2920   Model (fitted) 
+00022590: 746f 2070 6c6f 740a 2020 2020 6669 673a  to plot.    fig:
+000225a0: 2070 6c74 2e46 6967 7572 650a 2020 2020   plt.Figure.    
+000225b0: 2020 2020 4d61 7470 6c6f 746c 6962 2046      Matplotlib F
+000225c0: 6967 7572 6520 6f62 6a65 6374 2075 7365  igure object use
+000225d0: 6420 666f 7220 706c 6f74 0a20 2020 2061  d for plot.    a
+000225e0: 783a 2070 6c74 2e41 7865 730a 2020 2020  x: plt.Axes.    
+000225f0: 2020 2020 4d61 7470 6c6f 746c 6962 2041      Matplotlib A
+00022600: 7869 7320 6f62 6a65 6374 2075 7365 6420  xis object used 
+00022610: 666f 7220 706c 6f74 0a0a 2020 2020 5265  for plot..    Re
+00022620: 7475 726e 730a 2020 2020 2d2d 2d2d 2d2d  turns.    ------
+00022630: 2d0a 2020 2020 4e6f 6e65 0a20 2020 2027  -.    None.    '
+00022640: 2727 0a0a 2020 2020 6966 2069 7369 6e73  ''..    if isins
+00022650: 7461 6e63 6528 6461 7461 7365 742c 2054  tance(dataset, T
+00022660: 6175 4844 6174 6173 6574 293a 0a20 2020  auHDataset):.   
+00022670: 2020 2020 2078 5f76 616c 7320 3d20 6461       x_vals = da
+00022680: 7461 7365 742e 6669 656c 6473 0a20 2020  taset.fields.   
+00022690: 2020 2020 2061 782e 7365 745f 786c 6162       ax.set_xlab
+000226a0: 656c 2872 2731 2f48 2024 5c6c 6566 7428  el(r'1/H $\left(
+000226b0: 5c6d 6174 6872 6567 756c 6172 7b4f 657d  \mathregular{Oe}
+000226c0: 5e5c 6d61 7468 7265 6775 6c61 727b 2d31  ^\mathregular{-1
+000226d0: 7d5c 7269 6768 7429 2427 290a 2020 2020  }\right)$').    
+000226e0: 2020 2020 785f 7479 7065 203d 2027 6669      x_type = 'fi
+000226f0: 656c 6427 0a20 2020 2065 6c69 6620 6973  eld'.    elif is
+00022700: 696e 7374 616e 6365 2864 6174 6173 6574  instance(dataset
+00022710: 2c20 5461 7554 4461 7461 7365 7429 3a0a  , TauTDataset):.
+00022720: 2020 2020 2020 2020 785f 7661 6c73 203d          x_vals =
+00022730: 2064 6174 6173 6574 2e74 656d 7065 7261   dataset.tempera
+00022740: 7475 7265 730a 2020 2020 2020 2020 6178  tures.        ax
+00022750: 2e73 6574 5f78 6c61 6265 6c28 7227 312f  .set_xlabel(r'1/
+00022760: 5420 245c 6c65 6674 285c 6d61 7468 7265  T $\left(\mathre
+00022770: 6775 6c61 727b 4b7d 5e5c 6d61 7468 7265  gular{K}^\mathre
+00022780: 6775 6c61 727b 2d31 7d5c 7269 6768 7429  gular{-1}\right)
+00022790: 2427 290a 2020 2020 2020 2020 785f 7479  $').        x_ty
+000227a0: 7065 203d 2027 7465 6d70 6572 6174 7572  pe = 'temperatur
+000227b0: 6527 0a0a 2020 2020 2320 4164 6420 756e  e'..    # Add un
+000227c0: 6365 7274 6169 6e74 6965 7320 6173 2065  certainties as e
+000227d0: 7272 6f72 6261 7273 0a20 2020 2069 6620  rrorbars.    if 
+000227e0: 6c65 6e28 6461 7461 7365 742e 7261 7465  len(dataset.rate
+000227f0: 5f70 6d29 3a0a 0a20 2020 2020 2020 2023  _pm):..        #
+00022800: 2043 616c 6375 6c61 7465 2074 696d 6520   Calculate time 
+00022810: 6572 726f 7262 6172 730a 2020 2020 2020  errorbars.      
+00022820: 2020 7469 6d65 7320 3d20 312e 202f 2064    times = 1. / d
+00022830: 6174 6173 6574 2e72 6174 6573 0a20 2020  ataset.rates.   
+00022840: 2020 2020 206d 696e 5f74 696d 6520 3d20       min_time = 
+00022850: 312e 202f 2028 6461 7461 7365 742e 7261  1. / (dataset.ra
+00022860: 7465 7320 2b20 6461 7461 7365 742e 7261  tes + dataset.ra
+00022870: 7465 5f70 6d5b 312c 203a 5d29 0a20 2020  te_pm[1, :]).   
+00022880: 2020 2020 206d 6178 5f74 696d 6520 3d20       max_time = 
+00022890: 312e 202f 2028 6461 7461 7365 742e 7261  1. / (dataset.ra
+000228a0: 7465 7320 2d20 6461 7461 7365 742e 7261  tes - dataset.ra
+000228b0: 7465 5f70 6d5b 302c 203a 5d29 0a0a 2020  te_pm[0, :])..  
+000228c0: 2020 2020 2020 6c6e 5f6d 696e 5f74 696d        ln_min_tim
+000228d0: 6520 3d20 6e70 2e6c 6f67 286d 696e 5f74  e = np.log(min_t
+000228e0: 696d 6529 0a20 2020 2020 2020 206c 6e5f  ime).        ln_
+000228f0: 6d61 785f 7469 6d65 203d 206e 702e 6c6f  max_time = np.lo
+00022900: 6728 6d61 785f 7469 6d65 290a 0a20 2020  g(max_time)..   
+00022910: 2020 2020 206c 6e5f 7469 6d65 5f70 6c75       ln_time_plu
+00022920: 7320 3d20 6c6e 5f6d 6178 5f74 696d 6520  s = ln_max_time 
+00022930: 2d20 6e70 2e6c 6f67 2874 696d 6573 290a  - np.log(times).
+00022940: 2020 2020 2020 2020 6c6e 5f74 696d 655f          ln_time_
+00022950: 6d69 6e75 7320 3d20 6e70 2e6c 6f67 2874  minus = np.log(t
+00022960: 696d 6573 2920 2d20 6c6e 5f6d 696e 5f74  imes) - ln_min_t
+00022970: 696d 650a 0a20 2020 2020 2020 206c 6e74  ime..        lnt
+00022980: 696d 655f 6d70 203d 206e 702e 6172 7261  ime_mp = np.arra
+00022990: 7928 5b6c 6e5f 7469 6d65 5f6d 696e 7573  y([ln_time_minus
+000229a0: 2c20 6c6e 5f74 696d 655f 706c 7573 5d29  , ln_time_plus])
+000229b0: 0a0a 2020 2020 2020 2020 6178 2e65 7272  ..        ax.err
+000229c0: 6f72 6261 7228 0a20 2020 2020 2020 2020  orbar(.         
+000229d0: 2020 2031 2e20 2f20 785f 7661 6c73 2c0a     1. / x_vals,.
+000229e0: 2020 2020 2020 2020 2020 2020 6e70 2e6c              np.l
+000229f0: 6f67 2874 696d 6573 292c 0a20 2020 2020  og(times),.     
+00022a00: 2020 2020 2020 2079 6572 723d 6c6e 7469         yerr=lnti
+00022a10: 6d65 5f6d 702c 0a20 2020 2020 2020 2020  me_mp,.         
+00022a20: 2020 206d 6172 6b65 723d 276f 272c 0a20     marker='o',. 
+00022a30: 2020 2020 2020 2020 2020 206c 773d 302c             lw=0,
+00022a40: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
+00022a50: 6e65 7769 6474 683d 312e 352c 0a20 2020  newidth=1.5,.   
+00022a60: 2020 2020 2020 2020 2066 696c 6c73 7479           fillsty
+00022a70: 6c65 3d27 6e6f 6e65 272c 0a20 2020 2020  le='none',.     
+00022a80: 2020 2020 2020 206c 6162 656c 3d27 4578         label='Ex
+00022a90: 7065 7269 6d65 6e74 272c 0a20 2020 2020  periment',.     
+00022aa0: 2020 2020 2020 2063 6f6c 6f72 3d27 626c         color='bl
+00022ab0: 6163 6b27 0a20 2020 2020 2020 2029 0a20  ack'.        ). 
+00022ac0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00022ad0: 2061 782e 706c 6f74 280a 2020 2020 2020   ax.plot(.      
+00022ae0: 2020 2020 2020 312e 202f 2078 5f76 616c        1. / x_val
+00022af0: 732c 0a20 2020 2020 2020 2020 2020 206e  s,.            n
+00022b00: 702e 6c6f 6728 312e 202f 2064 6174 6173  p.log(1. / datas
+00022b10: 6574 2e72 6174 6573 292c 0a20 2020 2020  et.rates),.     
+00022b20: 2020 2020 2020 206d 6172 6b65 723d 276f         marker='o
+00022b30: 272c 0a20 2020 2020 2020 2020 2020 206c  ',.            l
+00022b40: 773d 302c 0a20 2020 2020 2020 2020 2020  w=0,.           
+00022b50: 2066 696c 6c73 7479 6c65 3d27 6e6f 6e65   fillstyle='none
+00022b60: 272c 0a20 2020 2020 2020 2020 2020 206c  ',.            l
+00022b70: 6162 656c 3d27 4578 7065 7269 6d65 6e74  abel='Experiment
+00022b80: 272c 0a20 2020 2020 2020 2020 2020 2063  ',.            c
+00022b90: 6f6c 6f72 3d27 626c 6163 6b27 0a20 2020  olor='black'.   
+00022ba0: 2020 2020 2029 0a0a 2020 2020 785f 7661       )..    x_va
+00022bb0: 7273 5f67 7269 6420 3d20 6e70 2e6c 696e  rs_grid = np.lin
+00022bc0: 7370 6163 6528 0a20 2020 2020 2020 206e  space(.        n
+00022bd0: 702e 6d69 6e28 785f 7661 6c73 292c 0a20  p.min(x_vals),. 
+00022be0: 2020 2020 2020 206e 702e 6d61 7828 785f         np.max(x_
+00022bf0: 7661 6c73 292c 0a20 2020 2020 2020 2031  vals),.        1
+00022c00: 3030 300a 2020 2020 290a 0a20 2020 2069  000.    )..    i
+00022c10: 6620 7479 7065 286d 6f64 656c 2920 696e  f type(model) in
+00022c20: 205b 4d75 6c74 694c 6f67 5461 7554 4d6f   [MultiLogTauTMo
+00022c30: 6465 6c2c 204d 756c 7469 4c6f 6754 6175  del, MultiLogTau
+00022c40: 484d 6f64 656c 5d3a 0a20 2020 2020 2020  HModel]:.       
+00022c50: 206c 6f67 6d6f 6465 6c73 203d 206d 6f64   logmodels = mod
+00022c60: 656c 2e6c 6f67 6d6f 6465 6c73 0a20 2020  el.logmodels.   
+00022c70: 2065 6c73 653a 0a20 2020 2020 2020 206c   else:.        l
+00022c80: 6f67 6d6f 6465 6c73 203d 205b 6d6f 6465  ogmodels = [mode
+00022c90: 6c5d 0a0a 2020 2020 666f 7220 6c6f 676d  l]..    for logm
+00022ca0: 6f64 656c 2069 6e20 6c6f 676d 6f64 656c  odel in logmodel
+00022cb0: 733a 0a0a 2020 2020 2020 2020 6966 2074  s:..        if t
+00022cc0: 7970 6528 6c6f 676d 6f64 656c 2920 6973  ype(logmodel) is
+00022cd0: 204c 6f67 4f72 6261 6368 4d6f 6465 6c3a   LogOrbachModel:
+00022ce0: 0a20 2020 2020 2020 2020 2020 206c 6162  .            lab
+00022cf0: 656c 5f66 6974 203d 2027 5c6e 4669 7420  el_fit = '\nFit 
+00022d00: 7769 7468 270a 2020 2020 2020 2020 2020  with'.          
+00022d10: 2020 6c61 6265 6c5f 6669 7420 2b3d 2027    label_fit += '
+00022d20: 5c6e 2720 2b20 7227 7b7d 207b 3a36 2e32  \n' + r'{} {:6.2
+00022d30: 667d 2073 272e 666f 726d 6174 280a 2020  f} s'.format(.  
+00022d40: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+00022d50: 676d 6f64 656c 2e56 4152 4e41 4d45 535f  gmodel.VARNAMES_
+00022d60: 4d4d 5b27 755f 6566 6627 5d2c 0a20 2020  MM['u_eff'],.   
+00022d70: 2020 2020 2020 2020 2020 2020 206c 6f67               log
+00022d80: 6d6f 6465 6c2e 6669 6e61 6c5f 7661 725f  model.final_var_
+00022d90: 7661 6c75 6573 5b27 755f 6566 6627 5d0a  values['u_eff'].
+00022da0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00022db0: 2020 2020 2020 2020 2020 6c61 6265 6c5f            label_
+00022dc0: 6669 7420 2b3d 2027 5c6e 2720 2b20 7227  fit += '\n' + r'
+00022dd0: 7b7d 207b 3a30 342e 3365 7d27 2e66 6f72  {} {:04.3e}'.for
+00022de0: 6d61 7428 0a20 2020 2020 2020 2020 2020  mat(.           
+00022df0: 2020 2020 206c 6f67 6d6f 6465 6c2e 5641       logmodel.VA
+00022e00: 524e 414d 4553 5f4d 4d5b 2741 275d 2c20  RNAMES_MM['A'], 
+00022e10: 6c6f 676d 6f64 656c 2e66 696e 616c 5f76  logmodel.final_v
+00022e20: 6172 5f76 616c 7565 735b 2741 275d 0a20  ar_values['A']. 
+00022e30: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00022e40: 2020 2020 2065 6c69 6620 7479 7065 286c       elif type(l
+00022e50: 6f67 6d6f 6465 6c29 2069 7320 4c6f 6752  ogmodel) is LogR
+00022e60: 616d 616e 4d6f 6465 6c3a 0a20 2020 2020  amanModel:.     
+00022e70: 2020 2020 2020 206c 6162 656c 5f66 6974         label_fit
+00022e80: 203d 2027 5c6e 4669 7420 7769 7468 270a   = '\nFit with'.
+00022e90: 2020 2020 2020 2020 2020 2020 6c61 6265              labe
+00022ea0: 6c5f 6669 7420 2b3d 2027 5c6e 2720 2b20  l_fit += '\n' + 
+00022eb0: 7227 7b7d 207b 3a36 2e32 667d 2073 272e  r'{} {:6.2f} s'.
+00022ec0: 666f 726d 6174 280a 2020 2020 2020 2020  format(.        
+00022ed0: 2020 2020 2020 2020 6c6f 676d 6f64 656c          logmodel
+00022ee0: 2e56 4152 4e41 4d45 535f 4d4d 5b27 5227  .VARNAMES_MM['R'
+00022ef0: 5d2c 206c 6f67 6d6f 6465 6c2e 6669 6e61  ], logmodel.fina
+00022f00: 6c5f 7661 725f 7661 6c75 6573 5b27 5227  l_var_values['R'
+00022f10: 5d0a 2020 2020 2020 2020 2020 2020 290a  ].            ).
+00022f20: 2020 2020 2020 2020 2020 2020 6c61 6265              labe
+00022f30: 6c5f 6669 7420 2b3d 2027 5c6e 2720 2b20  l_fit += '\n' + 
+00022f40: 7227 7b7d 207b 3a30 342e 3365 7d27 2e66  r'{} {:04.3e}'.f
+00022f50: 6f72 6d61 7428 0a20 2020 2020 2020 2020  ormat(.         
+00022f60: 2020 2020 2020 206c 6f67 6d6f 6465 6c2e         logmodel.
+00022f70: 5641 524e 414d 4553 5f4d 4d5b 276e 275d  VARNAMES_MM['n']
+00022f80: 2c20 6c6f 676d 6f64 656c 2e66 696e 616c  , logmodel.final
+00022f90: 5f76 6172 5f76 616c 7565 735b 276e 275d  _var_values['n']
+00022fa0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+00022fb0: 2020 2020 2020 2065 6c69 6620 7479 7065         elif type
+00022fc0: 286c 6f67 6d6f 6465 6c29 2069 7320 4c6f  (logmodel) is Lo
+00022fd0: 6751 544d 4d6f 6465 6c3a 0a20 2020 2020  gQTMModel:.     
+00022fe0: 2020 2020 2020 206c 6162 656c 5f66 6974         label_fit
+00022ff0: 203d 2027 5c6e 4669 7420 7769 7468 270a   = '\nFit with'.
+00023000: 2020 2020 2020 2020 2020 2020 6c61 6265              labe
+00023010: 6c5f 6669 7420 2b3d 2027 5c6e 2720 2b20  l_fit += '\n' + 
+00023020: 7227 7b7d 207b 3a36 2e32 667d 2073 272e  r'{} {:6.2f} s'.
+00023030: 666f 726d 6174 280a 2020 2020 2020 2020  format(.        
+00023040: 2020 2020 2020 2020 6c6f 676d 6f64 656c          logmodel
+00023050: 2e56 4152 4e41 4d45 535f 4d4d 5b27 5127  .VARNAMES_MM['Q'
+00023060: 5d2c 206c 6f67 6d6f 6465 6c2e 6669 6e61  ], logmodel.fina
+00023070: 6c5f 7661 725f 7661 6c75 6573 5b27 5127  l_var_values['Q'
+00023080: 5d0a 2020 2020 2020 2020 2020 2020 290a  ].            ).
+00023090: 2020 2020 2020 2020 656c 6966 2074 7970          elif typ
+000230a0: 6528 6c6f 676d 6f64 656c 2920 6973 204c  e(logmodel) is L
+000230b0: 6f67 4469 7265 6374 4d6f 6465 6c3a 0a20  ogDirectModel:. 
+000230c0: 2020 2020 2020 2020 2020 206c 6162 656c             label
+000230d0: 5f66 6974 203d 2027 5c6e 4669 7420 7769  _fit = '\nFit wi
+000230e0: 7468 270a 2020 2020 2020 2020 2020 2020  th'.            
+000230f0: 6c61 6265 6c5f 6669 7420 2b3d 2027 5c6e  label_fit += '\n
+00023100: 2720 2b20 7227 7b7d 207b 3a36 2e32 667d  ' + r'{} {:6.2f}
+00023110: 2073 272e 666f 726d 6174 280a 2020 2020   s'.format(.    
+00023120: 2020 2020 2020 2020 2020 2020 6c6f 676d              logm
+00023130: 6f64 656c 2e56 4152 4e41 4d45 535f 4d4d  odel.VARNAMES_MM
+00023140: 5b27 4427 5d2c 206c 6f67 6d6f 6465 6c2e  ['D'], logmodel.
+00023150: 6669 6e61 6c5f 7661 725f 7661 6c75 6573  final_var_values
+00023160: 5b27 4427 5d0a 2020 2020 2020 2020 2020  ['D'].          
+00023170: 2020 290a 2020 2020 2020 2020 6d6f 6465    ).        mode
+00023180: 6c5f 7261 7465 7320 3d20 3130 2a2a 6c6f  l_rates = 10**lo
+00023190: 676d 6f64 656c 2e6d 6f64 656c 280a 2020  gmodel.model(.  
+000231a0: 2020 2020 2020 2020 2020 6c6f 676d 6f64            logmod
+000231b0: 656c 2e66 696e 616c 5f76 6172 5f76 616c  el.final_var_val
+000231c0: 7565 732c 0a20 2020 2020 2020 2020 2020  ues,.           
+000231d0: 2078 5f76 6172 735f 6772 6964 2c0a 2020   x_vars_grid,.  
+000231e0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+000231f0: 2023 2054 7269 6d20 6d6f 6465 6c20 7261   # Trim model ra
+00023200: 7465 7320 746f 2073 656e 7369 626c 6520  tes to sensible 
+00023210: 7661 6c75 6573 0a20 2020 2020 2020 2076  values.        v
+00023220: 616c 6964 5f69 6e74 203d 206e 702e 7768  alid_int = np.wh
+00023230: 6572 6528 6d6f 6465 6c5f 7261 7465 7320  ere(model_rates 
+00023240: 3e20 3145 2d36 295b 305d 0a0a 2020 2020  > 1E-6)[0]..    
+00023250: 2020 2020 6178 2e70 6c6f 7428 0a20 2020      ax.plot(.   
+00023260: 2020 2020 2020 2020 2031 2e20 2f20 6e70           1. / np
+00023270: 2e61 7272 6179 2878 5f76 6172 735f 6772  .array(x_vars_gr
+00023280: 6964 295b 7661 6c69 645f 696e 745d 2c0a  id)[valid_int],.
+00023290: 2020 2020 2020 2020 2020 2020 6e70 2e6c              np.l
+000232a0: 6f67 2831 2e20 2f20 6e70 2e61 7272 6179  og(1. / np.array
+000232b0: 286d 6f64 656c 5f72 6174 6573 295b 7661  (model_rates)[va
+000232c0: 6c69 645f 696e 745d 292c 0a20 2020 2020  lid_int]),.     
+000232d0: 2020 2020 2020 206c 773d 312e 352c 0a20         lw=1.5,. 
+000232e0: 2020 2020 2020 2020 2020 206c 6162 656c             label
+000232f0: 3d6c 6f67 6d6f 6465 6c2e 4e41 4d45 2c0a  =logmodel.NAME,.
+00023300: 2020 2020 2020 2020 2020 2020 6c73 3d27              ls='
+00023310: 2d2d 270a 2020 2020 2020 2020 290a 0a20  --'.        ).. 
+00023320: 2020 2069 6620 7479 7065 286d 6f64 656c     if type(model
+00023330: 2920 696e 205b 4d75 6c74 694c 6f67 5461  ) in [MultiLogTa
+00023340: 7554 4d6f 6465 6c2c 204d 756c 7469 4c6f  uTModel, MultiLo
+00023350: 6754 6175 484d 6f64 656c 5d20 616e 6420  gTauHModel] and 
+00023360: 6c65 6e28 6c6f 676d 6f64 656c 7329 203e  len(logmodels) >
+00023370: 2031 3a20 2320 6e6f 7161 0a20 2020 2020   1: # noqa.     
+00023380: 2020 2074 6f74 616c 203d 206e 702e 7a65     total = np.ze
+00023390: 726f 7328 6c65 6e28 785f 7661 7273 5f67  ros(len(x_vars_g
+000233a0: 7269 6429 290a 0a20 2020 2020 2020 2066  rid))..        f
+000233b0: 6f72 206c 6f67 6d6f 6465 6c20 696e 206c  or logmodel in l
+000233c0: 6f67 6d6f 6465 6c73 3a0a 2020 2020 2020  ogmodels:.      
+000233d0: 2020 2020 2020 746f 7461 6c20 2b3d 2031        total += 1
+000233e0: 302a 2a6c 6f67 6d6f 6465 6c2e 6d6f 6465  0**logmodel.mode
+000233f0: 6c28 0a20 2020 2020 2020 2020 2020 2020  l(.             
+00023400: 2020 206c 6f67 6d6f 6465 6c2e 6669 6e61     logmodel.fina
+00023410: 6c5f 7661 725f 7661 6c75 6573 2c0a 2020  l_var_values,.  
+00023420: 2020 2020 2020 2020 2020 2020 2020 785f                x_
+00023430: 7661 7273 5f67 7269 642c 0a20 2020 2020  vars_grid,.     
+00023440: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+00023450: 2020 6178 2e70 6c6f 7428 0a20 2020 2020    ax.plot(.     
+00023460: 2020 2020 2020 2031 2e20 2f20 785f 7661         1. / x_va
+00023470: 7273 5f67 7269 642c 0a20 2020 2020 2020  rs_grid,.       
+00023480: 2020 2020 206e 702e 6c6f 6728 312e 202f       np.log(1. /
+00023490: 2074 6f74 616c 292c 0a20 2020 2020 2020   total),.       
+000234a0: 2020 2020 206c 773d 312e 352c 0a20 2020       lw=1.5,.   
+000234b0: 2020 2020 2020 2020 206c 6162 656c 3d27           label='
+000234c0: 546f 7461 6c27 2c0a 2020 2020 2020 2020  Total',.        
+000234d0: 2020 2020 636f 6c6f 723d 2772 6564 270a      color='red'.
+000234e0: 2020 2020 2020 2020 290a 0a20 2020 2023          )..    #
+000234f0: 2045 6e61 626c 6520 6d69 6e6f 7220 7469   Enable minor ti
+00023500: 636b 730a 2020 2020 6178 2e79 6178 6973  cks.    ax.yaxis
+00023510: 2e73 6574 5f6d 696e 6f72 5f6c 6f63 6174  .set_minor_locat
+00023520: 6f72 2841 7574 6f4d 696e 6f72 4c6f 6361  or(AutoMinorLoca
+00023530: 746f 7228 2929 0a20 2020 2061 782e 7861  tor()).    ax.xa
+00023540: 7869 732e 7365 745f 6d69 6e6f 725f 6c6f  xis.set_minor_lo
+00023550: 6361 746f 7228 4175 746f 4d69 6e6f 724c  cator(AutoMinorL
+00023560: 6f63 6174 6f72 2829 290a 0a20 2020 2065  ocator())..    e
+00023570: 7870 7265 7373 696f 6e20 3d20 2727 0a0a  xpression = ''..
+00023580: 2020 2020 666f 7220 6c6f 676d 6f64 656c      for logmodel
+00023590: 2069 6e20 6c6f 676d 6f64 656c 733a 0a20   in logmodels:. 
+000235a0: 2020 2020 2020 2066 6f72 2069 742c 206e         for it, n
+000235b0: 616d 6520 696e 2065 6e75 6d65 7261 7465  ame in enumerate
+000235c0: 286c 6f67 6d6f 6465 6c2e 5041 524e 414d  (logmodel.PARNAM
+000235d0: 4553 293a 0a20 2020 2020 2020 2020 2020  ES):.           
+000235e0: 2065 7870 7265 7373 696f 6e20 2b3d 2027   expression += '
+000235f0: 7b7d 203d 207b 3a2e 3366 7d20 272e 666f  {} = {:.3f} '.fo
+00023600: 726d 6174 280a 2020 2020 2020 2020 2020  rmat(.          
+00023610: 2020 2020 2020 6c6f 676d 6f64 656c 2e56        logmodel.V
+00023620: 4152 4e41 4d45 535f 4d4d 5b6e 616d 655d  ARNAMES_MM[name]
+00023630: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00023640: 2020 6c6f 676d 6f64 656c 2e66 696e 616c    logmodel.final
+00023650: 5f76 6172 5f76 616c 7565 735b 6e61 6d65  _var_values[name
+00023660: 5d2c 0a20 2020 2020 2020 2020 2020 2029  ],.            )
+00023670: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00023680: 6e61 6d65 2069 6e20 6c6f 676d 6f64 656c  name in logmodel
+00023690: 2e66 6974 5f76 6172 732e 6b65 7973 2829  .fit_vars.keys()
+000236a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000236b0: 2020 6578 7072 6573 7369 6f6e 202b 3d20    expression += 
+000236c0: 7227 245c 706d 2420 270a 2020 2020 2020  r'$\pm$ '.      
+000236d0: 2020 2020 2020 2020 2020 6578 7072 6573            expres
+000236e0: 7369 6f6e 202b 3d20 277b 3a2e 3366 7d20  sion += '{:.3f} 
+000236f0: 272e 666f 726d 6174 286c 6f67 6d6f 6465  '.format(logmode
+00023700: 6c2e 6669 745f 7374 6465 765b 6e61 6d65  l.fit_stdev[name
+00023710: 5d29 0a20 2020 2020 2020 2020 2020 2065  ]).            e
+00023720: 7870 7265 7373 696f 6e20 2b3d 2027 7b7d  xpression += '{}
+00023730: 2020 2020 272e 666f 726d 6174 286c 6f67      '.format(log
+00023740: 6d6f 6465 6c2e 554e 4954 535f 4d4d 5b6e  model.UNITS_MM[n
+00023750: 616d 655d 290a 2020 2020 2020 2020 2020  ame]).          
+00023760: 2020 6966 2069 7420 3d3d 2031 2061 6e64    if it == 1 and
+00023770: 206c 656e 286c 6f67 6d6f 6465 6c2e 6669   len(logmodel.fi
+00023780: 745f 7661 7273 2e6b 6579 7328 2929 203e  t_vars.keys()) >
+00023790: 2032 3a0a 2020 2020 2020 2020 2020 2020   2:.            
+000237a0: 2020 2020 6578 7072 6573 7369 6f6e 202b      expression +
+000237b0: 3d20 275c 6e27 0a20 2020 2020 2020 2065  = '\n'.        e
+000237c0: 7870 7265 7373 696f 6e20 2b3d 2027 5c6e  xpression += '\n
+000237d0: 270a 0a20 2020 2061 782e 7465 7874 280a  '..    ax.text(.
+000237e0: 2020 2020 2020 2020 302e 302c 2031 2e30          0.0, 1.0
+000237f0: 322c 2073 3d65 7870 7265 7373 696f 6e2c  2, s=expression,
+00023800: 2066 6f6e 7473 697a 653d 3130 2c20 7472   fontsize=10, tr
+00023810: 616e 7366 6f72 6d3d 6178 2e74 7261 6e73  ansform=ax.trans
+00023820: 4178 6573 0a20 2020 2029 0a0a 2020 2020  Axes.    )..    
+00023830: 6966 2078 5f74 7970 6520 3d3d 2027 6669  if x_type == 'fi
+00023840: 656c 6427 3a0a 2020 2020 2020 2020 6178  eld':.        ax
+00023850: 2e6c 6567 656e 6428 0a20 2020 2020 2020  .legend(.       
+00023860: 2020 2020 2066 6f6e 7473 697a 653d 2731       fontsize='1
+00023870: 3027 2c20 6e75 6d70 6f69 6e74 733d 312c  0', numpoints=1,
+00023880: 206e 636f 6c3d 312c 2066 7261 6d65 6f6e   ncol=1, frameon
+00023890: 3d46 616c 7365 0a20 2020 2020 2020 2029  =False.        )
+000238a0: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+000238b0: 2020 2061 782e 6c65 6765 6e64 280a 2020     ax.legend(.  
+000238c0: 2020 2020 2020 2020 2020 6c6f 633d 276c            loc='l
+000238d0: 6f77 6572 2072 6967 6874 272c 2066 6f6e  ower right', fon
+000238e0: 7473 697a 653d 2731 3027 2c20 6e75 6d70  tsize='10', nump
+000238f0: 6f69 6e74 733d 312c 206e 636f 6c3d 312c  oints=1, ncol=1,
+00023900: 0a20 2020 2020 2020 2020 2020 2066 7261  .            fra
+00023910: 6d65 6f6e 3d46 616c 7365 0a20 2020 2020  meon=False.     
+00023920: 2020 2029 0a0a 2020 2020 6178 2e73 6574     )..    ax.set
+00023930: 5f79 6c61 6265 6c28 7227 245c 6c6e 5c6c  _ylabel(r'$\ln\l
+00023940: 6566 745b 5c74 6175 5c72 6967 6874 5d24  eft[\tau\right]$
+00023950: 2028 245c 6c6e 5c6c 6566 745b 5c6d 6174   ($\ln\left[\mat
+00023960: 6872 6567 756c 6172 7b73 7d5e 5c6d 6174  hregular{s}^\mat
+00023970: 6872 6567 756c 6172 7b2d 317d 5c72 6967  hregular{-1}\rig
+00023980: 6874 5d24 2927 2920 2320 6e6f 7161 0a0a  ht]$)') # noqa..
+00023990: 2020 2020 7265 7475 726e 0a0a 0a64 6566      return...def
+000239a0: 2070 6c6f 745f 6669 7474 6564 5f72 6174   plot_fitted_rat
+000239b0: 6573 2864 6174 6173 6574 3a20 5461 7554  es(dataset: TauT
+000239c0: 4461 7461 7365 7420 7c20 5461 7548 4461  Dataset | TauHDa
+000239d0: 7461 7365 742c 0a20 2020 2020 2020 2020  taset,.         
+000239e0: 2020 2020 2020 2020 2020 2020 206d 6f64               mod
+000239f0: 656c 3a20 4c6f 6754 6175 544d 6f64 656c  el: LogTauTModel
+00023a00: 207c 204d 756c 7469 4c6f 6754 6175 544d   | MultiLogTauTM
+00023a10: 6f64 656c 207c 204c 6f67 5461 7548 4d6f  odel | LogTauHMo
+00023a20: 6465 6c20 7c20 4d75 6c74 694c 6f67 5461  del | MultiLogTa
+00023a30: 7548 4d6f 6465 6c2c 2023 206e 6f71 610a  uHModel, # noqa.
+00023a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023a50: 2020 2020 2020 7368 6f77 3a20 626f 6f6c        show: bool
+00023a60: 203d 2054 7275 652c 2073 6176 653a 2062   = True, save: b
+00023a70: 6f6f 6c20 3d20 4661 6c73 652c 0a20 2020  ool = False,.   
+00023a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023a90: 2020 2073 6176 655f 6e61 6d65 3a20 7374     save_name: st
+00023aa0: 7220 3d20 2766 6974 7465 645f 7261 7465  r = 'fitted_rate
+00023ab0: 732e 706e 6727 2c0a 2020 2020 2020 2020  s.png',.        
+00023ac0: 2020 2020 2020 2020 2020 2020 2020 7665                ve
+00023ad0: 7262 6f73 653a 2062 6f6f 6c20 3d20 5472  rbose: bool = Tr
+00023ae0: 7565 2920 2d3e 2074 7570 6c65 5b70 6c74  ue) -> tuple[plt
+00023af0: 2e46 6967 7572 652c 2070 6c74 2e41 7865  .Figure, plt.Axe
+00023b00: 735d 3a0a 2020 2020 2727 270a 2020 2020  s]:.    '''.    
+00023b10: 506c 6f74 7320 6578 7065 7269 6d65 6e74  Plots experiment
+00023b20: 616c 2061 6e64 2066 6974 7465 6420 286d  al and fitted (m
+00023b30: 6f64 656c 2920 7265 6c61 7861 7469 6f6e  odel) relaxation
+00023b40: 2072 6174 6520 6173 5c6e 0a20 2020 2072   rate as\n.    r
+00023b50: 6174 6520 7673 2078 7661 7220 7768 6572  ate vs xvar wher
+00023b60: 6520 7876 6172 2069 7320 5420 6f72 2048  e xvar is T or H
+00023b70: 2e20 5769 7468 206c 6f67 206c 6f67 2073  . With log log s
+00023b80: 6361 6c65 2e0a 0a20 2020 2050 6172 616d  cale...    Param
+00023b90: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
+00023ba0: 2d2d 2d2d 0a20 2020 2064 6174 6173 6574  ----.    dataset
+00023bb0: 3a20 5461 7554 4461 7461 7365 7420 7c20  : TauTDataset | 
+00023bc0: 5461 7548 4461 7461 7365 740a 2020 2020  TauHDataset.    
+00023bd0: 2020 2020 4461 7461 7365 7420 746f 2070      Dataset to p
+00023be0: 6c6f 740a 2020 2020 6d6f 6465 6c3a 204c  lot.    model: L
+00023bf0: 6f67 5461 7554 4d6f 6465 6c20 7c20 4d75  ogTauTModel | Mu
+00023c00: 6c74 694c 6f67 5461 7554 4d6f 6465 6c20  ltiLogTauTModel 
+00023c10: 7c20 4c6f 6754 6175 484d 6f64 656c 207c  | LogTauHModel |
+00023c20: 204d 756c 7469 4c6f 6754 6175 484d 6f64   MultiLogTauHMod
+00023c30: 656c 0a20 2020 2020 2020 204d 6f64 656c  el.        Model
+00023c40: 2028 6669 7474 6564 2920 746f 2070 6c6f   (fitted) to plo
+00023c50: 740a 2020 2020 7368 6f77 3a20 626f 6f6c  t.    show: bool
+00023c60: 2c20 6465 6661 756c 7420 5472 7565 0a20  , default True. 
+00023c70: 2020 2020 2020 2049 6620 5472 7565 2c20         If True, 
+00023c80: 7368 6f77 2070 6c6f 7420 6f6e 2073 6372  show plot on scr
+00023c90: 6565 6e0a 2020 2020 7361 7665 3a20 626f  een.    save: bo
+00023ca0: 6f6c 2c20 6465 6661 756c 7420 4661 6c73  ol, default Fals
+00023cb0: 650a 2020 2020 2020 2020 4966 2054 7275  e.        If Tru
+00023cc0: 652c 2073 6176 6520 706c 6f74 2074 6f20  e, save plot to 
+00023cd0: 6669 6c65 2060 7361 7665 5f6e 616d 6560  file `save_name`
+00023ce0: 0a20 2020 2073 6176 655f 6e61 6d65 3a20  .    save_name: 
+00023cf0: 7374 722c 2064 6566 6175 6c74 203d 2027  str, default = '
+00023d00: 6669 7474 6564 5f72 6174 6573 2e70 6e67  fitted_rates.png
+00023d10: 270a 2020 2020 2020 2020 4966 2073 6176  '.        If sav
+00023d20: 6520 6973 2054 7275 652c 2077 696c 6c20  e is True, will 
+00023d30: 7361 7665 2070 6c6f 7420 746f 2074 6869  save plot to thi
+00023d40: 7320 6669 6c65 6e61 6d65 0a20 2020 2076  s filename.    v
+00023d50: 6572 626f 7365 3a20 626f 6f6c 2c20 6465  erbose: bool, de
+00023d60: 6661 756c 7420 5472 7565 0a20 2020 2020  fault True.     
+00023d70: 2020 2049 6620 5472 7565 2c20 706c 6f74     If True, plot
+00023d80: 2066 696c 6520 6c6f 6361 7469 6f6e 2069   file location i
+00023d90: 7320 7772 6974 7465 6e20 746f 2074 6572  s written to ter
+00023da0: 6d69 6e61 6c0a 2020 2020 5265 7475 726e  minal.    Return
+00023db0: 730a 2020 2020 2d2d 2d2d 2d2d 2d0a 2020  s.    -------.  
+00023dc0: 2020 706c 742e 4669 6775 7265 0a20 2020    plt.Figure.   
+00023dd0: 2020 2020 204d 6174 706c 6f74 6c69 6220       Matplotlib 
+00023de0: 6669 6775 7265 206f 626a 6563 740a 2020  figure object.  
+00023df0: 2020 706c 742e 4178 6573 0a20 2020 2020    plt.Axes.     
+00023e00: 2020 204d 6174 706c 6f74 6c69 6220 6178     Matplotlib ax
+00023e10: 6973 206f 626a 6563 740a 2020 2020 2727  is object.    ''
+00023e20: 270a 0a20 2020 2023 2043 7265 6174 6520  '..    # Create 
+00023e30: 6669 6775 7265 2061 6e64 2061 7865 730a  figure and axes.
+00023e40: 2020 2020 6669 672c 2061 7820 3d20 706c      fig, ax = pl
+00023e50: 742e 7375 6270 6c6f 7473 280a 2020 2020  t.subplots(.    
+00023e60: 2020 2020 312c 0a20 2020 2020 2020 2031      1,.        1
+00023e70: 2c0a 2020 2020 2020 2020 7368 6172 6578  ,.        sharex
+00023e80: 3d54 7275 652c 0a20 2020 2020 2020 2073  =True,.        s
+00023e90: 6861 7265 793d 5472 7565 2c0a 2020 2020  harey=True,.    
+00023ea0: 2020 2020 6669 6773 697a 653d 2836 2c20      figsize=(6, 
+00023eb0: 3629 2c0a 2020 2020 2020 2020 6e75 6d3d  6),.        num=
+00023ec0: 2746 6974 7465 6420 7265 6c61 7861 7469  'Fitted relaxati
+00023ed0: 6f6e 2070 726f 6669 6c65 270a 2020 2020  on profile'.    
+00023ee0: 290a 0a20 2020 205f 706c 6f74 5f66 6974  )..    _plot_fit
+00023ef0: 7465 645f 7261 7465 7328 6461 7461 7365  ted_rates(datase
+00023f00: 742c 206d 6f64 656c 2c20 6669 672c 2061  t, model, fig, a
+00023f10: 7829 0a0a 2020 2020 6669 672e 7469 6768  x)..    fig.tigh
+00023f20: 745f 6c61 796f 7574 2829 0a0a 2020 2020  t_layout()..    
+00023f30: 6966 2073 686f 773a 0a20 2020 2020 2020  if show:.       
+00023f40: 2070 6c74 2e73 686f 7728 290a 0a20 2020   plt.show()..   
+00023f50: 2069 6620 7361 7665 3a0a 2020 2020 2020   if save:.      
+00023f60: 2020 6669 672e 7361 7665 6669 6728 7361    fig.savefig(sa
+00023f70: 7665 5f6e 616d 652c 2064 7069 3d35 3030  ve_name, dpi=500
+00023f80: 290a 2020 2020 2020 2020 6966 2076 6572  ).        if ver
+00023f90: 626f 7365 3a0a 2020 2020 2020 2020 2020  bose:.          
+00023fa0: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+00023fb0: 6461 7461 7365 742c 2028 5461 7554 4461  dataset, (TauTDa
+00023fc0: 7461 7365 7429 293a 0a20 2020 2020 2020  taset)):.       
+00023fd0: 2020 2020 2020 2020 205f 7876 6172 203d           _xvar =
+00023fe0: 2027 5427 0a20 2020 2020 2020 2020 2020   'T'.           
+00023ff0: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
+00024000: 2864 6174 6173 6574 2c20 2854 6175 4844  (dataset, (TauHD
+00024010: 6174 6173 6574 2929 3a0a 2020 2020 2020  ataset)):.      
+00024020: 2020 2020 2020 2020 2020 5f78 7661 7220            _xvar 
+00024030: 3d20 2748 270a 2020 2020 2020 2020 2020  = 'H'.          
+00024040: 2020 7574 2e63 7072 696e 7428 0a20 2020    ut.cprint(.   
+00024050: 2020 2020 2020 2020 2020 2020 2066 275c               f'\
+00024060: 6e20 4669 7474 6564 20cf 84e2 81bb c2b9  n Fitted .......
+00024070: 2076 7320 7b5f 7876 6172 7d20 706c 6f74   vs {_xvar} plot
+00024080: 2073 6176 6564 2074 6f20 5c6e 207b 7361   saved to \n {sa
+00024090: 7665 5f6e 616d 657d 5c6e 272c 0a20 2020  ve_name}\n',.   
+000240a0: 2020 2020 2020 2020 2020 2020 2027 6379               'cy
+000240b0: 616e 270a 2020 2020 2020 2020 2020 2020  an'.            
+000240c0: 290a 0a20 2020 2072 6574 7572 6e20 6669  )..    return fi
+000240d0: 672c 2061 780a 0a0a 6465 6620 7174 5f70  g, ax...def qt_p
+000240e0: 6c6f 745f 6669 7474 6564 5f72 6174 6573  lot_fitted_rates
+000240f0: 2861 7070 3a20 5174 5769 6467 6574 732e  (app: QtWidgets.
+00024100: 5141 7070 6c69 6361 7469 6f6e 2c0a 2020  QApplication,.  
+00024110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024120: 2020 2020 2020 2064 6174 6173 6574 3a20         dataset: 
+00024130: 5461 7554 4461 7461 7365 7420 7c20 5461  TauTDataset | Ta
+00024140: 7548 4461 7461 7365 742c 0a20 2020 2020  uHDataset,.     
+00024150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024160: 2020 2020 6d6f 6465 6c3a 204c 6f67 5461      model: LogTa
+00024170: 7554 4d6f 6465 6c20 7c20 4d75 6c74 694c  uTModel | MultiL
+00024180: 6f67 5461 7554 4d6f 6465 6c20 7c20 4c6f  ogTauTModel | Lo
+00024190: 6754 6175 484d 6f64 656c 207c 204d 756c  gTauHModel | Mul
+000241a0: 7469 4c6f 6754 6175 484d 6f64 656c 2c20  tiLogTauHModel, 
+000241b0: 2320 6e6f 7161 0a20 2020 2020 2020 2020  # noqa.         
+000241c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000241d0: 7361 7665 3a20 626f 6f6c 203d 2046 616c  save: bool = Fal
+000241e0: 7365 2c20 7368 6f77 3a20 626f 6f6c 203d  se, show: bool =
+000241f0: 2054 7275 652c 0a20 2020 2020 2020 2020   True,.         
+00024200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024210: 7361 7665 5f6e 616d 653a 2073 7472 203d  save_name: str =
+00024220: 2027 6669 7474 6564 5f72 6174 6573 2e70   'fitted_rates.p
+00024230: 6e67 272c 0a20 2020 2020 2020 2020 2020  ng',.           
+00024240: 2020 2020 2020 2020 2020 2020 2020 7665                ve
+00024250: 7262 6f73 653a 2062 6f6f 6c20 3d20 5472  rbose: bool = Tr
+00024260: 7565 2920 2d3e 204e 6f6e 653a 0a20 2020  ue) -> None:.   
+00024270: 2027 2727 0a20 2020 2050 6c6f 7473 2065   '''.    Plots e
+00024280: 7870 6572 696d 656e 7461 6c20 616e 6420  xperimental and 
+00024290: 6669 7474 6564 2028 6d6f 6465 6c29 2072  fitted (model) r
+000242a0: 656c 6178 6174 696f 6e20 7261 7465 2061  elaxation rate a
+000242b0: 735c 6e0a 2020 2020 7261 7465 2076 7320  s\n.    rate vs 
+000242c0: 7876 6172 2077 6865 7265 2078 7661 7220  xvar where xvar 
+000242d0: 6973 2054 206f 7220 482e 2057 6974 6820  is T or H. With 
+000242e0: 6c6f 6720 6c6f 6720 7363 616c 652e 0a0a  log log scale...
+000242f0: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+00024300: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+00024310: 2020 6461 7461 7365 743a 2054 6175 5444    dataset: TauTD
+00024320: 6174 6173 6574 207c 2054 6175 4844 6174  ataset | TauHDat
+00024330: 6173 6574 0a20 2020 2020 2020 2044 6174  aset.        Dat
+00024340: 6173 6574 2074 6f20 706c 6f74 0a20 2020  aset to plot.   
+00024350: 206d 6f64 656c 3a20 4c6f 6754 6175 544d   model: LogTauTM
+00024360: 6f64 656c 207c 204d 756c 7469 4c6f 6754  odel | MultiLogT
+00024370: 6175 544d 6f64 656c 207c 204c 6f67 5461  auTModel | LogTa
+00024380: 7548 4d6f 6465 6c20 7c20 4d75 6c74 694c  uHModel | MultiL
+00024390: 6f67 5461 7548 4d6f 6465 6c0a 2020 2020  ogTauHModel.    
+000243a0: 2020 2020 4d6f 6465 6c20 2866 6974 7465      Model (fitte
+000243b0: 6429 2074 6f20 706c 6f74 0a20 2020 2073  d) to plot.    s
+000243c0: 686f 773a 2062 6f6f 6c2c 2064 6566 6175  how: bool, defau
+000243d0: 6c74 2054 7275 650a 2020 2020 2020 2020  lt True.        
+000243e0: 4966 2054 7275 652c 2073 686f 7720 706c  If True, show pl
+000243f0: 6f74 206f 6e20 7363 7265 656e 0a20 2020  ot on screen.   
+00024400: 2073 6176 653a 2062 6f6f 6c2c 2064 6566   save: bool, def
+00024410: 6175 6c74 2046 616c 7365 0a20 2020 2020  ault False.     
+00024420: 2020 2049 6620 5472 7565 2c20 7361 7665     If True, save
+00024430: 2070 6c6f 7420 746f 2066 696c 6520 6073   plot to file `s
+00024440: 6176 655f 6e61 6d65 600a 2020 2020 7361  ave_name`.    sa
+00024450: 7665 5f6e 616d 653a 2073 7472 2c20 6465  ve_name: str, de
+00024460: 6661 756c 7420 2766 6974 7465 645f 7261  fault 'fitted_ra
+00024470: 7465 732e 706e 6727 0a20 2020 2020 2020  tes.png'.       
+00024480: 2049 6620 7361 7665 2069 7320 5472 7565   If save is True
+00024490: 2c20 7769 6c6c 2073 6176 6520 706c 6f74  , will save plot
+000244a0: 2074 6f20 7468 6973 2066 696c 656e 616d   to this filenam
+000244b0: 650a 2020 2020 7665 7262 6f73 653a 2062  e.    verbose: b
+000244c0: 6f6f 6c2c 2064 6566 6175 6c74 2054 7275  ool, default Tru
+000244d0: 650a 2020 2020 2020 2020 4966 2054 7275  e.        If Tru
+000244e0: 652c 2070 6c6f 7420 6669 6c65 206c 6f63  e, plot file loc
+000244f0: 6174 696f 6e20 6973 2077 7269 7474 656e  ation is written
+00024500: 2074 6f20 7465 726d 696e 616c 0a0a 2020   to terminal..  
+00024510: 2020 5265 7475 726e 730a 2020 2020 2d2d    Returns.    --
+00024520: 2d2d 2d2d 2d0a 2020 2020 4e6f 6e65 0a20  -----.    None. 
+00024530: 2020 2027 2727 0a0a 2020 2020 7769 6e64     '''..    wind
+00024540: 6f77 203d 2067 7569 2e4d 6174 706c 6f74  ow = gui.Matplot
+00024550: 6c69 6257 696e 646f 7728 290a 0a20 2020  libWindow()..   
+00024560: 2077 696e 646f 772e 7365 7457 696e 646f   window.setWindo
+00024570: 7754 6974 6c65 2827 4669 7474 6564 2072  wTitle('Fitted r
+00024580: 656c 6178 6174 696f 6e20 7072 6f66 696c  elaxation profil
+00024590: 6527 290a 0a20 2020 2023 2041 6464 2070  e')..    # Add p
+000245a0: 6c6f 740a 2020 2020 5f70 6c6f 745f 6669  lot.    _plot_fi
+000245b0: 7474 6564 5f72 6174 6573 2864 6174 6173  tted_rates(datas
+000245c0: 6574 2c20 6d6f 6465 6c2c 2077 696e 646f  et, model, windo
+000245d0: 772e 7363 2e66 6967 2c20 7769 6e64 6f77  w.sc.fig, window
+000245e0: 2e73 632e 6178 290a 0a20 2020 2023 2053  .sc.ax)..    # S
+000245f0: 6176 6520 706c 6f74 0a20 2020 2069 6620  ave plot.    if 
+00024600: 7361 7665 3a0a 2020 2020 2020 2020 7769  save:.        wi
+00024610: 6e64 6f77 2e73 632e 6669 672e 7361 7665  ndow.sc.fig.save
+00024620: 6669 6728 7361 7665 5f6e 616d 652c 2064  fig(save_name, d
+00024630: 7069 3d33 3030 290a 2020 2020 2020 2020  pi=300).        
+00024640: 6966 2076 6572 626f 7365 3a0a 2020 2020  if verbose:.    
+00024650: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
+00024660: 7461 6e63 6528 6461 7461 7365 742c 2028  tance(dataset, (
+00024670: 5461 7554 4461 7461 7365 7429 293a 0a20  TauTDataset)):. 
+00024680: 2020 2020 2020 2020 2020 2020 2020 205f                 _
+00024690: 7876 6172 203d 2027 5427 0a20 2020 2020  xvar = 'T'.     
+000246a0: 2020 2020 2020 2065 6c69 6620 6973 696e         elif isin
+000246b0: 7374 616e 6365 2864 6174 6173 6574 2c20  stance(dataset, 
+000246c0: 2854 6175 4844 6174 6173 6574 2929 3a0a  (TauHDataset)):.
+000246d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000246e0: 5f78 7661 7220 3d20 2748 270a 2020 2020  _xvar = 'H'.    
+000246f0: 2020 2020 2020 2020 7574 2e63 7072 696e          ut.cprin
+00024700: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
+00024710: 2020 2066 275c 6e20 4669 7474 6564 20cf     f'\n Fitted .
+00024720: 84e2 81bb c2b9 2076 7320 7b5f 7876 6172  ...... vs {_xvar
+00024730: 7d20 706c 6f74 2073 6176 6564 2074 6f20  } plot saved to 
+00024740: 5c6e 207b 7361 7665 5f6e 616d 657d 5c6e  \n {save_name}\n
+00024750: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+00024760: 2020 2027 6379 616e 270a 2020 2020 2020     'cyan'.      
+00024770: 2020 2020 2020 290a 0a20 2020 2069 6620        )..    if 
+00024780: 7368 6f77 3a0a 2020 2020 2020 2020 7769  show:.        wi
+00024790: 6e64 6f77 2e73 686f 7728 290a 2020 2020  ndow.show().    
+000247a0: 2020 2020 2320 4361 6c6c 2074 7769 6365      # Call twice
+000247b0: 2065 6c73 6520 6974 2077 6f6e 7420 776f   else it wont wo
+000247c0: 726b 210a 2020 2020 2020 2020 7769 6e64  rk!.        wind
+000247d0: 6f77 2e73 632e 6669 672e 7469 6768 745f  ow.sc.fig.tight_
+000247e0: 6c61 796f 7574 2829 0a20 2020 2020 2020  layout().       
+000247f0: 2077 696e 646f 772e 7363 2e66 6967 2e74   window.sc.fig.t
+00024800: 6967 6874 5f6c 6179 6f75 7428 290a 2020  ight_layout().  
+00024810: 2020 2020 2020 6170 702e 6578 6563 5f28        app.exec_(
+00024820: 290a 0a20 2020 2072 6574 7572 6e0a 0a0a  )..    return...
+00024830: 6465 6620 5f70 6c6f 745f 6669 7474 6564  def _plot_fitted
+00024840: 5f72 6174 6573 2864 6174 6173 6574 3a20  _rates(dataset: 
+00024850: 5461 7554 4461 7461 7365 7420 7c20 5461  TauTDataset | Ta
+00024860: 7548 4461 7461 7365 742c 0a20 2020 2020  uHDataset,.     
+00024870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024880: 2020 6d6f 6465 6c3a 204c 6f67 5461 7554    model: LogTauT
+00024890: 4d6f 6465 6c20 7c20 4d75 6c74 694c 6f67  Model | MultiLog
+000248a0: 5461 7554 4d6f 6465 6c20 7c20 4c6f 6754  TauTModel | LogT
+000248b0: 6175 484d 6f64 656c 207c 204d 756c 7469  auHModel | Multi
+000248c0: 4c6f 6754 6175 484d 6f64 656c 2c20 2320  LogTauHModel, # 
+000248d0: 6e6f 7161 0a20 2020 2020 2020 2020 2020  noqa.           
+000248e0: 2020 2020 2020 2020 2020 2020 6669 673a              fig:
+000248f0: 2070 6c74 2e46 6967 7572 652c 2061 783a   plt.Figure, ax:
+00024900: 2070 6c74 2e41 7865 7329 3a0a 2020 2020   plt.Axes):.    
+00024910: 2727 270a 2020 2020 506c 6f74 7320 6578  '''.    Plots ex
+00024920: 7065 7269 6d65 6e74 616c 2061 6e64 2066  perimental and f
+00024930: 6974 7465 6420 286d 6f64 656c 2920 7265  itted (model) re
+00024940: 6c61 7861 7469 6f6e 2072 6174 6520 6173  laxation rate as
+00024950: 5c6e 0a20 2020 2072 6174 6520 7673 2078  \n.    rate vs x
+00024960: 7661 7220 7768 6572 6520 7876 6172 2069  var where xvar i
+00024970: 7320 5420 6f72 2048 2e20 5769 7468 206c  s T or H. With l
+00024980: 6f67 206c 6f67 2073 6361 6c65 2e0a 0a20  og log scale... 
+00024990: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+000249a0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+000249b0: 2064 6174 6173 6574 3a20 5461 7554 4461   dataset: TauTDa
+000249c0: 7461 7365 7420 7c20 5461 7548 4461 7461  taset | TauHData
+000249d0: 7365 740a 2020 2020 2020 2020 4461 7461  set.        Data
+000249e0: 7365 7420 746f 2070 6c6f 740a 2020 2020  set to plot.    
+000249f0: 6d6f 6465 6c3a 204c 6f67 5461 7554 4d6f  model: LogTauTMo
+00024a00: 6465 6c20 7c20 4d75 6c74 694c 6f67 5461  del | MultiLogTa
+00024a10: 7554 4d6f 6465 6c20 7c20 4c6f 6754 6175  uTModel | LogTau
+00024a20: 484d 6f64 656c 207c 204d 756c 7469 4c6f  HModel | MultiLo
+00024a30: 6754 6175 484d 6f64 656c 0a20 2020 2020  gTauHModel.     
+00024a40: 2020 204d 6f64 656c 2028 6669 7474 6564     Model (fitted
+00024a50: 2920 746f 2070 6c6f 740a 2020 2020 6669  ) to plot.    fi
+00024a60: 673a 2070 6c74 2e46 6967 7572 650a 2020  g: plt.Figure.  
+00024a70: 2020 2020 2020 4d61 7470 6c6f 746c 6962        Matplotlib
+00024a80: 2046 6967 7572 6520 6f62 6a65 6374 2075   Figure object u
+00024a90: 7365 6420 666f 7220 706c 6f74 0a20 2020  sed for plot.   
+00024aa0: 2061 783a 2070 6c74 2e41 7865 730a 2020   ax: plt.Axes.  
+00024ab0: 2020 2020 2020 4d61 7470 6c6f 746c 6962        Matplotlib
+00024ac0: 2041 7869 7320 6f62 6a65 6374 2075 7365   Axis object use
+00024ad0: 6420 666f 7220 706c 6f74 0a0a 2020 2020  d for plot..    
+00024ae0: 5265 7475 726e 730a 2020 2020 2d2d 2d2d  Returns.    ----
+00024af0: 2d2d 2d0a 2020 2020 4e6f 6e65 0a20 2020  ---.    None.   
+00024b00: 2027 2727 0a0a 2020 2020 6966 2069 7369   '''..    if isi
+00024b10: 6e73 7461 6e63 6528 6461 7461 7365 742c  nstance(dataset,
+00024b20: 2054 6175 4844 6174 6173 6574 293a 0a20   TauHDataset):. 
+00024b30: 2020 2020 2020 2078 5f76 616c 7320 3d20         x_vals = 
+00024b40: 6461 7461 7365 742e 6669 656c 6473 0a20  dataset.fields. 
+00024b50: 2020 2020 2020 2078 5f74 7970 6520 3d20         x_type = 
+00024b60: 2766 6965 6c64 270a 2020 2020 2020 2020  'field'.        
+00024b70: 6178 2e73 6574 5f78 6c61 6265 6c28 7227  ax.set_xlabel(r'
+00024b80: 4669 656c 6420 284f 6529 2729 0a20 2020  Field (Oe)').   
+00024b90: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
+00024ba0: 2864 6174 6173 6574 2c20 5461 7554 4461  (dataset, TauTDa
+00024bb0: 7461 7365 7429 3a0a 2020 2020 2020 2020  taset):.        
+00024bc0: 785f 7661 6c73 203d 2064 6174 6173 6574  x_vals = dataset
+00024bd0: 2e74 656d 7065 7261 7475 7265 730a 2020  .temperatures.  
+00024be0: 2020 2020 2020 785f 7479 7065 203d 2027        x_type = '
+00024bf0: 7465 6d70 6572 6174 7572 6527 0a20 2020  temperature'.   
+00024c00: 2020 2020 2061 782e 7365 745f 786c 6162       ax.set_xlab
+00024c10: 656c 2872 2754 656d 7065 7261 7475 7265  el(r'Temperature
+00024c20: 2028 4b29 2729 0a0a 2020 2020 2320 4164   (K)')..    # Ad
+00024c30: 6420 756e 6365 7274 6169 6e74 6965 7320  d uncertainties 
+00024c40: 6173 2065 7272 6f72 6261 7273 0a20 2020  as errorbars.   
+00024c50: 2069 6620 6c65 6e28 6461 7461 7365 742e   if len(dataset.
+00024c60: 7261 7465 5f70 6d29 3a0a 2020 2020 2020  rate_pm):.      
+00024c70: 2020 6178 2e65 7272 6f72 6261 7228 0a20    ax.errorbar(. 
+00024c80: 2020 2020 2020 2020 2020 2078 5f76 616c             x_val
+00024c90: 732c 0a20 2020 2020 2020 2020 2020 2064  s,.            d
+00024ca0: 6174 6173 6574 2e72 6174 6573 2c0a 2020  ataset.rates,.  
+00024cb0: 2020 2020 2020 2020 2020 7965 7272 3d64            yerr=d
+00024cc0: 6174 6173 6574 2e72 6174 655f 706d 2c0a  ataset.rate_pm,.
+00024cd0: 2020 2020 2020 2020 2020 2020 6d61 726b              mark
+00024ce0: 6572 3d27 6f27 2c0a 2020 2020 2020 2020  er='o',.        
+00024cf0: 2020 2020 6c77 3d30 2c0a 2020 2020 2020      lw=0,.      
+00024d00: 2020 2020 2020 656c 696e 6577 6964 7468        elinewidth
+00024d10: 3d31 2e35 2c0a 2020 2020 2020 2020 2020  =1.5,.          
+00024d20: 2020 6669 6c6c 7374 796c 653d 276e 6f6e    fillstyle='non
+00024d30: 6527 2c0a 2020 2020 2020 2020 2020 2020  e',.            
+00024d40: 6c61 6265 6c3d 2745 7870 6572 696d 656e  label='Experimen
+00024d50: 7427 2c0a 2020 2020 2020 2020 2020 2020  t',.            
+00024d60: 636f 6c6f 723d 2762 6c61 636b 270a 2020  color='black'.  
+00024d70: 2020 2020 2020 290a 2020 2020 656c 7365        ).    else
+00024d80: 3a0a 2020 2020 2020 2020 6178 2e70 6c6f  :.        ax.plo
+00024d90: 7428 0a20 2020 2020 2020 2020 2020 2078  t(.            x
+00024da0: 5f76 616c 732c 0a20 2020 2020 2020 2020  _vals,.         
+00024db0: 2020 2064 6174 6173 6574 2e72 6174 6573     dataset.rates
+00024dc0: 2c0a 2020 2020 2020 2020 2020 2020 6d61  ,.            ma
+00024dd0: 726b 6572 3d27 6f27 2c0a 2020 2020 2020  rker='o',.      
+00024de0: 2020 2020 2020 6c77 3d30 2c0a 2020 2020        lw=0,.    
+00024df0: 2020 2020 2020 2020 6669 6c6c 7374 796c          fillstyl
+00024e00: 653d 276e 6f6e 6527 2c0a 2020 2020 2020  e='none',.      
+00024e10: 2020 2020 2020 6c61 6265 6c3d 2745 7870        label='Exp
+00024e20: 6572 696d 656e 7427 2c0a 2020 2020 2020  eriment',.      
+00024e30: 2020 2020 2020 636f 6c6f 723d 2762 6c61        color='bla
+00024e40: 636b 270a 2020 2020 2020 2020 290a 0a20  ck'.        ).. 
+00024e50: 2020 2078 5f76 6172 735f 6772 6964 203d     x_vars_grid =
+00024e60: 206e 702e 6c69 6e73 7061 6365 280a 2020   np.linspace(.  
+00024e70: 2020 2020 2020 6e70 2e6d 696e 2878 5f76        np.min(x_v
+00024e80: 616c 7329 2c0a 2020 2020 2020 2020 6e70  als),.        np
+00024e90: 2e6d 6178 2878 5f76 616c 7329 2c0a 2020  .max(x_vals),.  
+00024ea0: 2020 2020 2020 3530 3030 0a20 2020 2029        5000.    )
+00024eb0: 0a0a 2020 2020 6966 2074 7970 6528 6d6f  ..    if type(mo
+00024ec0: 6465 6c29 2069 6e20 5b4d 756c 7469 4c6f  del) in [MultiLo
+00024ed0: 6754 6175 544d 6f64 656c 2c20 4d75 6c74  gTauTModel, Mult
+00024ee0: 694c 6f67 5461 7548 4d6f 6465 6c5d 3a0a  iLogTauHModel]:.
+00024ef0: 2020 2020 2020 2020 6c6f 676d 6f64 656c          logmodel
+00024f00: 7320 3d20 6d6f 6465 6c2e 6c6f 676d 6f64  s = model.logmod
+00024f10: 656c 730a 2020 2020 656c 7365 3a0a 2020  els.    else:.  
+00024f20: 2020 2020 2020 6c6f 676d 6f64 656c 7320        logmodels 
+00024f30: 3d20 5b6d 6f64 656c 5d0a 0a20 2020 2066  = [model]..    f
+00024f40: 6f72 206c 6f67 6d6f 6465 6c20 696e 206c  or logmodel in l
+00024f50: 6f67 6d6f 6465 6c73 3a0a 0a20 2020 2020  ogmodels:..     
+00024f60: 2020 2069 6620 7479 7065 286c 6f67 6d6f     if type(logmo
+00024f70: 6465 6c29 2069 7320 4c6f 674f 7262 6163  del) is LogOrbac
+00024f80: 684d 6f64 656c 3a0a 2020 2020 2020 2020  hModel:.        
+00024f90: 2020 2020 6c61 6265 6c5f 6669 7420 3d20      label_fit = 
+00024fa0: 275c 6e46 6974 2077 6974 6827 0a20 2020  '\nFit with'.   
+00024fb0: 2020 2020 2020 2020 206c 6162 656c 5f66           label_f
+00024fc0: 6974 202b 3d20 275c 6e27 202b 2072 277b  it += '\n' + r'{
+00024fd0: 7d20 7b3a 362e 3266 7d20 7327 2e66 6f72  } {:6.2f} s'.for
+00024fe0: 6d61 7428 0a20 2020 2020 2020 2020 2020  mat(.           
+00024ff0: 2020 2020 206c 6f67 6d6f 6465 6c2e 5641       logmodel.VA
+00025000: 524e 414d 4553 5f4d 4d5b 2775 5f65 6666  RNAMES_MM['u_eff
+00025010: 275d 2c0a 2020 2020 2020 2020 2020 2020  '],.            
+00025020: 2020 2020 6c6f 676d 6f64 656c 2e66 696e      logmodel.fin
+00025030: 616c 5f76 6172 5f76 616c 7565 735b 2775  al_var_values['u
+00025040: 5f65 6666 275d 0a20 2020 2020 2020 2020  _eff'].         
+00025050: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00025060: 206c 6162 656c 5f66 6974 202b 3d20 275c   label_fit += '\
+00025070: 6e27 202b 2072 277b 7d20 7b3a 3034 2e33  n' + r'{} {:04.3
+00025080: 657d 272e 666f 726d 6174 280a 2020 2020  e}'.format(.    
+00025090: 2020 2020 2020 2020 2020 2020 6c6f 676d              logm
+000250a0: 6f64 656c 2e56 4152 4e41 4d45 535f 4d4d  odel.VARNAMES_MM
+000250b0: 5b27 4127 5d2c 206c 6f67 6d6f 6465 6c2e  ['A'], logmodel.
+000250c0: 6669 6e61 6c5f 7661 725f 7661 6c75 6573  final_var_values
+000250d0: 5b27 4127 5d0a 2020 2020 2020 2020 2020  ['A'].          
+000250e0: 2020 290a 2020 2020 2020 2020 656c 6966    ).        elif
+000250f0: 2074 7970 6528 6c6f 676d 6f64 656c 2920   type(logmodel) 
+00025100: 6973 204c 6f67 5261 6d61 6e4d 6f64 656c  is LogRamanModel
+00025110: 3a0a 2020 2020 2020 2020 2020 2020 6c61  :.            la
+00025120: 6265 6c5f 6669 7420 3d20 275c 6e46 6974  bel_fit = '\nFit
+00025130: 2077 6974 6827 0a20 2020 2020 2020 2020   with'.         
+00025140: 2020 206c 6162 656c 5f66 6974 202b 3d20     label_fit += 
+00025150: 275c 6e27 202b 2072 277b 7d20 7b3a 362e  '\n' + r'{} {:6.
+00025160: 3266 7d20 7327 2e66 6f72 6d61 7428 0a20  2f} s'.format(. 
+00025170: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00025180: 6f67 6d6f 6465 6c2e 5641 524e 414d 4553  ogmodel.VARNAMES
+00025190: 5f4d 4d5b 2752 275d 2c20 6c6f 676d 6f64  _MM['R'], logmod
+000251a0: 656c 2e66 696e 616c 5f76 6172 5f76 616c  el.final_var_val
+000251b0: 7565 735b 2752 275d 0a20 2020 2020 2020  ues['R'].       
+000251c0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+000251d0: 2020 206c 6162 656c 5f66 6974 202b 3d20     label_fit += 
+000251e0: 275c 6e27 202b 2072 277b 7d20 7b3a 3034  '\n' + r'{} {:04
+000251f0: 2e33 657d 272e 666f 726d 6174 280a 2020  .3e}'.format(.  
+00025200: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+00025210: 676d 6f64 656c 2e56 4152 4e41 4d45 535f  gmodel.VARNAMES_
+00025220: 4d4d 5b27 6e27 5d2c 206c 6f67 6d6f 6465  MM['n'], logmode
+00025230: 6c2e 6669 6e61 6c5f 7661 725f 7661 6c75  l.final_var_valu
+00025240: 6573 5b27 6e27 5d0a 2020 2020 2020 2020  es['n'].        
+00025250: 2020 2020 290a 2020 2020 2020 2020 656c      ).        el
+00025260: 6966 2074 7970 6528 6c6f 676d 6f64 656c  if type(logmodel
+00025270: 2920 6973 204c 6f67 5154 4d4d 6f64 656c  ) is LogQTMModel
+00025280: 3a0a 2020 2020 2020 2020 2020 2020 6c61  :.            la
+00025290: 6265 6c5f 6669 7420 3d20 275c 6e46 6974  bel_fit = '\nFit
+000252a0: 2077 6974 6827 0a20 2020 2020 2020 2020   with'.         
+000252b0: 2020 206c 6162 656c 5f66 6974 202b 3d20     label_fit += 
+000252c0: 275c 6e27 202b 2072 277b 7d20 7b3a 362e  '\n' + r'{} {:6.
+000252d0: 3266 7d20 7327 2e66 6f72 6d61 7428 0a20  2f} s'.format(. 
+000252e0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+000252f0: 6f67 6d6f 6465 6c2e 5641 524e 414d 4553  ogmodel.VARNAMES
+00025300: 5f4d 4d5b 2751 275d 2c20 6c6f 676d 6f64  _MM['Q'], logmod
+00025310: 656c 2e66 696e 616c 5f76 6172 5f76 616c  el.final_var_val
+00025320: 7565 735b 2751 275d 0a20 2020 2020 2020  ues['Q'].       
+00025330: 2020 2020 2029 0a20 2020 2020 2020 2065       ).        e
+00025340: 6c69 6620 7479 7065 286c 6f67 6d6f 6465  lif type(logmode
+00025350: 6c29 2069 7320 4c6f 6744 6972 6563 744d  l) is LogDirectM
+00025360: 6f64 656c 3a0a 2020 2020 2020 2020 2020  odel:.          
+00025370: 2020 6c61 6265 6c5f 6669 7420 3d20 275c    label_fit = '\
+00025380: 6e46 6974 2077 6974 6827 0a20 2020 2020  nFit with'.     
+00025390: 2020 2020 2020 206c 6162 656c 5f66 6974         label_fit
+000253a0: 202b 3d20 275c 6e27 202b 2072 277b 7d20   += '\n' + r'{} 
+000253b0: 7b3a 362e 3266 7d20 7327 2e66 6f72 6d61  {:6.2f} s'.forma
+000253c0: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
+000253d0: 2020 206c 6f67 6d6f 6465 6c2e 5641 524e     logmodel.VARN
+000253e0: 414d 4553 5f4d 4d5b 2744 275d 2c20 6c6f  AMES_MM['D'], lo
+000253f0: 676d 6f64 656c 2e66 696e 616c 5f76 6172  gmodel.final_var
+00025400: 5f76 616c 7565 735b 2744 275d 0a20 2020  _values['D'].   
+00025410: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00025420: 2020 206d 6f64 656c 5f72 6174 6573 203d     model_rates =
+00025430: 2031 302a 2a6c 6f67 6d6f 6465 6c2e 6d6f   10**logmodel.mo
+00025440: 6465 6c28 0a20 2020 2020 2020 2020 2020  del(.           
+00025450: 206c 6f67 6d6f 6465 6c2e 6669 6e61 6c5f   logmodel.final_
+00025460: 7661 725f 7661 6c75 6573 2c0a 2020 2020  var_values,.    
+00025470: 2020 2020 2020 2020 785f 7661 7273 5f67          x_vars_g
+00025480: 7269 642c 0a20 2020 2020 2020 2029 0a0a  rid,.        )..
+00025490: 2020 2020 2020 2020 2320 5472 696d 206d          # Trim m
+000254a0: 6f64 656c 2072 6174 6573 2074 6f20 7365  odel rates to se
+000254b0: 6e73 6962 6c65 2076 616c 7565 730a 2020  nsible values.  
+000254c0: 2020 2020 2020 7661 6c69 645f 696e 7420        valid_int 
+000254d0: 3d20 6e70 2e77 6865 7265 286d 6f64 656c  = np.where(model
+000254e0: 5f72 6174 6573 203e 2031 452d 3629 5b30  _rates > 1E-6)[0
+000254f0: 5d0a 0a20 2020 2020 2020 2061 782e 706c  ]..        ax.pl
+00025500: 6f74 280a 2020 2020 2020 2020 2020 2020  ot(.            
+00025510: 6e70 2e61 7272 6179 2878 5f76 6172 735f  np.array(x_vars_
+00025520: 6772 6964 295b 7661 6c69 645f 696e 745d  grid)[valid_int]
+00025530: 2c0a 2020 2020 2020 2020 2020 2020 6e70  ,.            np
+00025540: 2e61 7272 6179 286d 6f64 656c 5f72 6174  .array(model_rat
+00025550: 6573 295b 7661 6c69 645f 696e 745d 2c0a  es)[valid_int],.
+00025560: 2020 2020 2020 2020 2020 2020 6c77 3d31              lw=1
+00025570: 2e35 2c0a 2020 2020 2020 2020 2020 2020  .5,.            
+00025580: 6c61 6265 6c3d 6c6f 676d 6f64 656c 2e4e  label=logmodel.N
+00025590: 414d 452c 0a20 2020 2020 2020 2020 2020  AME,.           
+000255a0: 206c 733d 272d 2d27 0a20 2020 2020 2020   ls='--'.       
+000255b0: 2029 0a0a 2020 2020 6966 2074 7970 6528   )..    if type(
+000255c0: 6d6f 6465 6c29 2069 6e20 5b4d 756c 7469  model) in [Multi
+000255d0: 4c6f 6754 6175 544d 6f64 656c 2c20 4d75  LogTauTModel, Mu
+000255e0: 6c74 694c 6f67 5461 7548 4d6f 6465 6c5d  ltiLogTauHModel]
+000255f0: 2061 6e64 206c 656e 286c 6f67 6d6f 6465   and len(logmode
+00025600: 6c73 2920 3e20 313a 2023 206e 6f71 610a  ls) > 1: # noqa.
+00025610: 2020 2020 2020 2020 746f 7461 6c20 3d20          total = 
+00025620: 6e70 2e7a 6572 6f73 286c 656e 2878 5f76  np.zeros(len(x_v
+00025630: 6172 735f 6772 6964 2929 0a0a 2020 2020  ars_grid))..    
+00025640: 2020 2020 666f 7220 6c6f 676d 6f64 656c      for logmodel
+00025650: 2069 6e20 6c6f 676d 6f64 656c 733a 0a20   in logmodels:. 
+00025660: 2020 2020 2020 2020 2020 2074 6f74 616c             total
+00025670: 202b 3d20 3130 2a2a 6c6f 676d 6f64 656c   += 10**logmodel
+00025680: 2e6d 6f64 656c 280a 2020 2020 2020 2020  .model(.        
+00025690: 2020 2020 2020 2020 6c6f 676d 6f64 656c          logmodel
+000256a0: 2e66 696e 616c 5f76 6172 5f76 616c 7565  .final_var_value
+000256b0: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
+000256c0: 2020 2078 5f76 6172 735f 6772 6964 2c0a     x_vars_grid,.
+000256d0: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+000256e0: 2020 2020 2020 2061 782e 706c 6f74 280a         ax.plot(.
+000256f0: 2020 2020 2020 2020 2020 2020 785f 7661              x_va
+00025700: 7273 5f67 7269 642c 0a20 2020 2020 2020  rs_grid,.       
+00025710: 2020 2020 2074 6f74 616c 2c0a 2020 2020       total,.    
+00025720: 2020 2020 2020 2020 6c77 3d31 2e35 2c0a          lw=1.5,.
+00025730: 2020 2020 2020 2020 2020 2020 6c61 6265              labe
+00025740: 6c3d 2754 6f74 616c 272c 0a20 2020 2020  l='Total',.     
+00025750: 2020 2020 2020 2063 6f6c 6f72 3d27 7265         color='re
+00025760: 6427 0a20 2020 2020 2020 2029 0a0a 2020  d'.        )..  
+00025770: 2020 6966 2078 5f74 7970 6520 3d3d 2027    if x_type == '
+00025780: 6669 656c 6427 3a0a 2020 2020 2020 2020  field':.        
+00025790: 6178 2e73 6574 5f78 7363 616c 6528 2773  ax.set_xscale('s
+000257a0: 796d 6c6f 6727 2c20 6c69 6e74 6872 6573  ymlog', linthres
+000257b0: 683d 6775 692e 6361 6c63 5f6c 696e 7468  h=gui.calc_linth
+000257c0: 7265 7368 2878 5f76 616c 7329 290a 2020  resh(x_vals)).  
+000257d0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+000257e0: 6178 2e73 6574 5f78 7363 616c 6528 276c  ax.set_xscale('l
+000257f0: 6f67 2729 0a20 2020 2061 782e 7365 745f  og').    ax.set_
+00025800: 7973 6361 6c65 2827 6c6f 6727 290a 0a20  yscale('log').. 
+00025810: 2020 2067 7569 2e66 6f72 6d61 745f 7261     gui.format_ra
+00025820: 7465 5f78 5f79 5f61 7865 7328 0a20 2020  te_x_y_axes(.   
+00025830: 2020 2020 2061 782c 0a20 2020 2020 2020       ax,.       
+00025840: 2064 6174 6173 6574 2e72 6174 6573 2c0a   dataset.rates,.
+00025850: 2020 2020 2020 2020 785f 7661 7273 5f67          x_vars_g
+00025860: 7269 642c 0a20 2020 2020 2020 206e 702e  rid,.        np.
+00025870: 6162 7328 6461 7461 7365 742e 7261 7465  abs(dataset.rate
+00025880: 5f70 6d29 2c0a 2020 2020 2020 2020 785f  _pm),.        x_
+00025890: 7479 7065 3d78 5f74 7970 650a 2020 2020  type=x_type.    
+000258a0: 290a 0a20 2020 2065 7870 7265 7373 696f  )..    expressio
+000258b0: 6e20 3d20 2727 0a0a 2020 2020 666f 7220  n = ''..    for 
+000258c0: 6c6f 676d 6f64 656c 2069 6e20 6c6f 676d  logmodel in logm
+000258d0: 6f64 656c 733a 0a20 2020 2020 2020 2066  odels:.        f
+000258e0: 6f72 2069 742c 206e 616d 6520 696e 2065  or it, name in e
+000258f0: 6e75 6d65 7261 7465 286c 6f67 6d6f 6465  numerate(logmode
+00025900: 6c2e 5041 524e 414d 4553 293a 0a20 2020  l.PARNAMES):.   
+00025910: 2020 2020 2020 2020 2065 7870 7265 7373           express
+00025920: 696f 6e20 2b3d 2027 7b7d 203d 207b 3a2e  ion += '{} = {:.
+00025930: 3366 7d20 272e 666f 726d 6174 280a 2020  3f} '.format(.  
+00025940: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+00025950: 676d 6f64 656c 2e56 4152 4e41 4d45 535f  gmodel.VARNAMES_
+00025960: 4d4d 5b6e 616d 655d 2c0a 2020 2020 2020  MM[name],.      
+00025970: 2020 2020 2020 2020 2020 6c6f 676d 6f64            logmod
+00025980: 656c 2e66 696e 616c 5f76 6172 5f76 616c  el.final_var_val
+00025990: 7565 735b 6e61 6d65 5d2c 0a20 2020 2020  ues[name],.     
+000259a0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+000259b0: 2020 2020 2069 6620 6e61 6d65 2069 6e20       if name in 
+000259c0: 6c6f 676d 6f64 656c 2e66 6974 5f76 6172  logmodel.fit_var
+000259d0: 732e 6b65 7973 2829 3a0a 2020 2020 2020  s.keys():.      
+000259e0: 2020 2020 2020 2020 2020 6578 7072 6573            expres
+000259f0: 7369 6f6e 202b 3d20 7227 245c 706d 2420  sion += r'$\pm$ 
+00025a00: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
+00025a10: 2020 6578 7072 6573 7369 6f6e 202b 3d20    expression += 
+00025a20: 277b 3a2e 3366 7d20 272e 666f 726d 6174  '{:.3f} '.format
+00025a30: 286c 6f67 6d6f 6465 6c2e 6669 745f 7374  (logmodel.fit_st
+00025a40: 6465 765b 6e61 6d65 5d29 0a20 2020 2020  dev[name]).     
+00025a50: 2020 2020 2020 2065 7870 7265 7373 696f         expressio
+00025a60: 6e20 2b3d 2027 7b7d 2020 2020 272e 666f  n += '{}    '.fo
+00025a70: 726d 6174 286c 6f67 6d6f 6465 6c2e 554e  rmat(logmodel.UN
+00025a80: 4954 535f 4d4d 5b6e 616d 655d 290a 2020  ITS_MM[name]).  
+00025a90: 2020 2020 2020 2020 2020 6966 2069 7420            if it 
+00025aa0: 3d3d 2031 2061 6e64 206c 656e 286c 6f67  == 1 and len(log
+00025ab0: 6d6f 6465 6c2e 6669 745f 7661 7273 2e6b  model.fit_vars.k
+00025ac0: 6579 7328 2929 203e 2032 3a0a 2020 2020  eys()) > 2:.    
+00025ad0: 2020 2020 2020 2020 2020 2020 6578 7072              expr
+00025ae0: 6573 7369 6f6e 202b 3d20 275c 6e27 0a20  ession += '\n'. 
+00025af0: 2020 2020 2020 2065 7870 7265 7373 696f         expressio
+00025b00: 6e20 2b3d 2027 5c6e 270a 0a20 2020 2061  n += '\n'..    a
+00025b10: 782e 7465 7874 280a 2020 2020 2020 2020  x.text(.        
+00025b20: 302e 302c 2031 2e30 322c 2073 3d65 7870  0.0, 1.02, s=exp
+00025b30: 7265 7373 696f 6e2c 2066 6f6e 7473 697a  ression, fontsiz
+00025b40: 653d 3130 2c20 7472 616e 7366 6f72 6d3d  e=10, transform=
+00025b50: 6178 2e74 7261 6e73 4178 6573 0a20 2020  ax.transAxes.   
+00025b60: 2029 0a0a 2020 2020 6966 2078 5f74 7970   )..    if x_typ
+00025b70: 6520 3d3d 2027 6669 656c 6427 3a0a 2020  e == 'field':.  
+00025b80: 2020 2020 2020 6178 2e6c 6567 656e 6428        ax.legend(
+00025b90: 0a20 2020 2020 2020 2020 2020 2066 6f6e  .            fon
+00025ba0: 7473 697a 653d 2731 3027 2c20 6e75 6d70  tsize='10', nump
+00025bb0: 6f69 6e74 733d 312c 206e 636f 6c3d 312c  oints=1, ncol=1,
+00025bc0: 2066 7261 6d65 6f6e 3d46 616c 7365 0a20   frameon=False. 
+00025bd0: 2020 2020 2020 2029 0a20 2020 2065 6c73         ).    els
+00025be0: 653a 0a20 2020 2020 2020 2061 782e 6c65  e:.        ax.le
+00025bf0: 6765 6e64 280a 2020 2020 2020 2020 2020  gend(.          
+00025c00: 2020 6c6f 633d 2775 7070 6572 206c 6566    loc='upper lef
+00025c10: 7427 2c20 666f 6e74 7369 7a65 3d27 3130  t', fontsize='10
+00025c20: 272c 206e 756d 706f 696e 7473 3d31 2c20  ', numpoints=1, 
+00025c30: 6e63 6f6c 3d31 2c20 6672 616d 656f 6e3d  ncol=1, frameon=
+00025c40: 4661 6c73 650a 2020 2020 2020 2020 290a  False.        ).
+00025c50: 0a20 2020 2061 782e 7365 745f 796c 6162  .    ax.set_ylab
+00025c60: 656c 2872 2752 6174 6520 2873 245e 5c6d  el(r'Rate (s$^\m
+00025c70: 6174 6872 6567 756c 6172 7b2d 317d 2429  athregular{-1}$)
+00025c80: 2729 0a0a 2020 2020 7265 7475 726e 0a0a  ')..    return..
+00025c90: 0a64 6566 2070 6c6f 745f 7261 7465 7328  .def plot_rates(
+00025ca0: 6461 7461 7365 743a 2054 6175 5444 6174  dataset: TauTDat
+00025cb0: 6173 6574 207c 2054 6175 4844 6174 6173  aset | TauHDatas
+00025cc0: 6574 2c20 7368 6f77 3a20 626f 6f6c 203d  et, show: bool =
+00025cd0: 2054 7275 652c 0a20 2020 2020 2020 2020   True,.         
+00025ce0: 2020 2020 2020 7361 7665 3a20 626f 6f6c        save: bool
+00025cf0: 203d 2046 616c 7365 2c20 7361 7665 5f6e   = False, save_n
+00025d00: 616d 653a 2073 7472 203d 2027 7265 6c61  ame: str = 'rela
+00025d10: 7861 7469 6f6e 5f72 6174 6573 2e70 6e67  xation_rates.png
+00025d20: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+00025d30: 2020 7665 7262 6f73 653a 2062 6f6f 6c20    verbose: bool 
+00025d40: 3d20 5472 7565 2920 2d3e 2074 7570 6c65  = True) -> tuple
+00025d50: 5b70 6c74 2e46 6967 7572 652c 2070 6c74  [plt.Figure, plt
+00025d60: 2e41 7865 735d 3a0a 2020 2020 2727 270a  .Axes]:.    '''.
+00025d70: 2020 2020 506c 6f74 7320 6578 7065 7269      Plots experi
+00025d80: 6d65 6e74 616c 2072 656c 6178 6174 696f  mental relaxatio
+00025d90: 6e20 7261 7465 2076 7320 6669 656c 642f  n rate vs field/
+00025da0: 7465 6d70 6572 6174 7572 6520 616e 640a  temperature and.
+00025db0: 2020 2020 6469 7370 6c61 7973 206f 6e20      displays on 
+00025dc0: 7363 7265 656e 2e0a 0a20 2020 2050 6172  screen...    Par
+00025dd0: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
+00025de0: 2d2d 2d2d 2d2d 0a20 2020 2064 6174 6173  ------.    datas
+00025df0: 6574 3a20 5461 7554 4461 7461 7365 7420  et: TauTDataset 
+00025e00: 7c20 5461 7548 4461 7461 7365 740a 2020  | TauHDataset.  
+00025e10: 2020 2020 2020 4461 7461 7365 7420 746f        Dataset to
+00025e20: 2070 6c6f 740a 2020 2020 7368 6f77 3a20   plot.    show: 
+00025e30: 626f 6f6c 2c20 6465 6661 756c 7420 5472  bool, default Tr
+00025e40: 7565 0a20 2020 2020 2020 2049 6620 5472  ue.        If Tr
+00025e50: 7565 2c20 7368 6f77 2070 6c6f 7420 6f6e  ue, show plot on
+00025e60: 2073 6372 6565 6e0a 2020 2020 7361 7665   screen.    save
+00025e70: 3a20 626f 6f6c 2c20 6465 6661 756c 7420  : bool, default 
+00025e80: 4661 6c73 650a 2020 2020 2020 2020 4966  False.        If
+00025e90: 2054 7275 652c 2073 6176 6520 706c 6f74   True, save plot
+00025ea0: 2074 6f20 6669 6c65 2060 7361 7665 5f6e   to file `save_n
+00025eb0: 616d 6560 0a20 2020 2073 6176 655f 6e61  ame`.    save_na
+00025ec0: 6d65 3a20 7374 722c 2064 6566 6175 6c74  me: str, default
+00025ed0: 2027 7265 6c61 7861 7469 6f6e 5f72 6174   'relaxation_rat
+00025ee0: 6573 2e70 6e67 270a 2020 2020 2020 2020  es.png'.        
+00025ef0: 4966 2073 6176 6520 6973 2054 7275 652c  If save is True,
+00025f00: 2077 696c 6c20 7361 7665 2070 6c6f 7420   will save plot 
+00025f10: 746f 2074 6869 7320 6669 6c65 6e61 6d65  to this filename
+00025f20: 0a20 2020 2076 6572 626f 7365 3a20 626f  .    verbose: bo
+00025f30: 6f6c 2c20 6465 6661 756c 7420 5472 7565  ol, default True
+00025f40: 0a20 2020 2020 2020 2049 6620 5472 7565  .        If True
+00025f50: 2c20 706c 6f74 2066 696c 6520 6c6f 6361  , plot file loca
+00025f60: 7469 6f6e 2069 7320 7772 6974 7465 6e20  tion is written 
+00025f70: 746f 2074 6572 6d69 6e61 6c0a 0a20 2020  to terminal..   
+00025f80: 2052 6574 7572 6e73 0a20 2020 202d 2d2d   Returns.    ---
+00025f90: 2d2d 2d2d 0a20 2020 2070 6c74 2e46 6967  ----.    plt.Fig
+00025fa0: 7572 650a 2020 2020 2020 2020 4d61 7470  ure.        Matp
+00025fb0: 6c6f 746c 6962 2066 6967 7572 6520 6f62  lotlib figure ob
+00025fc0: 6a65 6374 0a20 2020 2070 6c74 2e41 7865  ject.    plt.Axe
+00025fd0: 730a 2020 2020 2020 2020 4d61 7470 6c6f  s.        Matplo
+00025fe0: 746c 6962 2061 7869 7320 6f62 6a65 6374  tlib axis object
+00025ff0: 0a20 2020 2027 2727 0a0a 2020 2020 2320  .    '''..    # 
+00026000: 4372 6561 7465 2066 6967 7572 6520 616e  Create figure an
+00026010: 6420 6178 6573 0a20 2020 2066 6967 2c20  d axes.    fig, 
+00026020: 6178 203d 2070 6c74 2e73 7562 706c 6f74  ax = plt.subplot
+00026030: 7328 0a20 2020 2020 2020 2031 2c0a 2020  s(.        1,.  
+00026040: 2020 2020 2020 312c 0a20 2020 2020 2020        1,.       
+00026050: 2073 6861 7265 783d 5472 7565 2c0a 2020   sharex=True,.  
+00026060: 2020 2020 2020 7368 6172 6579 3d54 7275        sharey=Tru
+00026070: 652c 0a20 2020 2020 2020 2066 6967 7369  e,.        figsi
+00026080: 7a65 3d28 362c 2036 292c 0a20 2020 2020  ze=(6, 6),.     
+00026090: 2020 206e 756d 3d27 4669 7474 6564 2072     num='Fitted r
+000260a0: 656c 6178 6174 696f 6e20 7072 6f66 696c  elaxation profil
+000260b0: 6527 0a20 2020 2029 0a0a 2020 2020 6966  e'.    )..    if
+000260c0: 2069 7369 6e73 7461 6e63 6528 6461 7461   isinstance(data
+000260d0: 7365 742c 2054 6175 4844 6174 6173 6574  set, TauHDataset
+000260e0: 293a 0a20 2020 2020 2020 2078 5f76 616c  ):.        x_val
+000260f0: 7320 3d20 6461 7461 7365 742e 6669 656c  s = dataset.fiel
+00026100: 6473 0a20 2020 2020 2020 2078 5f74 7970  ds.        x_typ
+00026110: 6520 3d20 2766 6965 6c64 270a 2020 2020  e = 'field'.    
+00026120: 2020 2020 6178 2e73 6574 5f78 6c61 6265      ax.set_xlabe
+00026130: 6c28 7227 4669 656c 6420 284f 6529 2729  l(r'Field (Oe)')
+00026140: 0a20 2020 2065 6c69 6620 6973 696e 7374  .    elif isinst
+00026150: 616e 6365 2864 6174 6173 6574 2c20 5461  ance(dataset, Ta
+00026160: 7554 4461 7461 7365 7429 3a0a 2020 2020  uTDataset):.    
+00026170: 2020 2020 785f 7661 6c73 203d 2064 6174      x_vals = dat
+00026180: 6173 6574 2e74 656d 7065 7261 7475 7265  aset.temperature
+00026190: 730a 2020 2020 2020 2020 785f 7479 7065  s.        x_type
+000261a0: 203d 2027 7465 6d70 6572 6174 7572 6527   = 'temperature'
+000261b0: 0a20 2020 2020 2020 2061 782e 7365 745f  .        ax.set_
+000261c0: 786c 6162 656c 2872 2754 656d 7065 7261  xlabel(r'Tempera
+000261d0: 7475 7265 2028 4b29 2729 0a0a 2020 2020  ture (K)')..    
+000261e0: 2320 4164 6420 756e 6365 7274 6169 6e74  # Add uncertaint
+000261f0: 6965 7320 6173 2065 7272 6f72 6261 7273  ies as errorbars
+00026200: 0a20 2020 2069 6620 6c65 6e28 6461 7461  .    if len(data
+00026210: 7365 742e 7261 7465 5f70 6d29 3a0a 2020  set.rate_pm):.  
+00026220: 2020 2020 2020 6178 2e65 7272 6f72 6261        ax.errorba
+00026230: 7228 0a20 2020 2020 2020 2020 2020 2078  r(.            x
+00026240: 5f76 616c 732c 0a20 2020 2020 2020 2020  _vals,.         
+00026250: 2020 2064 6174 6173 6574 2e72 6174 6573     dataset.rates
+00026260: 2c0a 2020 2020 2020 2020 2020 2020 7965  ,.            ye
+00026270: 7272 3d64 6174 6173 6574 2e72 6174 655f  rr=dataset.rate_
+00026280: 706d 2c0a 2020 2020 2020 2020 2020 2020  pm,.            
+00026290: 6d61 726b 6572 3d27 6f27 2c0a 2020 2020  marker='o',.    
+000262a0: 2020 2020 2020 2020 6c77 3d30 2c0a 2020          lw=0,.  
+000262b0: 2020 2020 2020 2020 2020 656c 696e 6577            elinew
+000262c0: 6964 7468 3d31 2e35 2c0a 2020 2020 2020  idth=1.5,.      
+000262d0: 2020 2020 2020 6669 6c6c 7374 796c 653d        fillstyle=
+000262e0: 276e 6f6e 6527 2c0a 2020 2020 2020 2020  'none',.        
+000262f0: 2020 2020 636f 6c6f 723d 2762 6c61 636b      color='black
+00026300: 270a 2020 2020 2020 2020 290a 2020 2020  '.        ).    
+00026310: 656c 7365 3a0a 2020 2020 2020 2020 6178  else:.        ax
+00026320: 2e70 6c6f 7428 0a20 2020 2020 2020 2020  .plot(.         
+00026330: 2020 2078 5f76 616c 732c 0a20 2020 2020     x_vals,.     
+00026340: 2020 2020 2020 2064 6174 6173 6574 2e72         dataset.r
+00026350: 6174 6573 2c0a 2020 2020 2020 2020 2020  ates,.          
+00026360: 2020 6d61 726b 6572 3d27 6f27 2c0a 2020    marker='o',.  
+00026370: 2020 2020 2020 2020 2020 6c77 3d30 2c0a            lw=0,.
+00026380: 2020 2020 2020 2020 2020 2020 6669 6c6c              fill
+00026390: 7374 796c 653d 276e 6f6e 6527 2c0a 2020  style='none',.  
+000263a0: 2020 2020 2020 2020 2020 636f 6c6f 723d            color=
+000263b0: 2762 6c61 636b 270a 2020 2020 2020 2020  'black'.        
+000263c0: 290a 0a20 2020 2069 6620 785f 7479 7065  )..    if x_type
+000263d0: 203d 3d20 2766 6965 6c64 273a 0a20 2020   == 'field':.   
+000263e0: 2020 2020 2061 782e 7365 745f 7873 6361       ax.set_xsca
+000263f0: 6c65 2827 7379 6d6c 6f67 272c 206c 696e  le('symlog', lin
+00026400: 7468 7265 7368 3d67 7569 2e63 616c 635f  thresh=gui.calc_
+00026410: 6c69 6e74 6872 6573 6828 785f 7661 6c73  linthresh(x_vals
+00026420: 2929 0a20 2020 2065 6c73 653a 0a20 2020  )).    else:.   
+00026430: 2020 2020 2061 782e 7365 745f 7873 6361       ax.set_xsca
+00026440: 6c65 2827 6c6f 6727 290a 2020 2020 6178  le('log').    ax
+00026450: 2e73 6574 5f79 7363 616c 6528 276c 6f67  .set_yscale('log
+00026460: 2729 0a0a 2020 2020 6178 2e73 6574 5f79  ')..    ax.set_y
+00026470: 6c61 6265 6c28 7227 5261 7465 2028 7324  label(r'Rate (s$
+00026480: 5e5c 6d61 7468 7265 6775 6c61 727b 2d31  ^\mathregular{-1
+00026490: 7d24 2927 290a 0a20 2020 2069 6620 6c65  }$)')..    if le
+000264a0: 6e28 6461 7461 7365 742e 6c6f 6772 6174  n(dataset.lograt
+000264b0: 655f 706d 293a 0a20 2020 2020 2020 2061  e_pm):.        a
+000264c0: 6c6c 5f64 6174 6120 3d20 5b0a 2020 2020  ll_data = [.    
+000264d0: 2020 2020 2020 2020 6e70 2e6c 6f67 3130          np.log10
+000264e0: 2864 6174 6173 6574 2e72 6174 6573 2920  (dataset.rates) 
+000264f0: 2b20 6461 7461 7365 742e 6c6f 6772 6174  + dataset.lograt
+00026500: 655f 706d 0a20 2020 2020 2020 205d 0a20  e_pm.        ]. 
+00026510: 2020 2020 2020 2061 6c6c 5f64 6174 6120         all_data 
+00026520: 2b3d 205b 0a20 2020 2020 2020 2020 2020  += [.           
+00026530: 206e 702e 6c6f 6731 3028 6461 7461 7365   np.log10(datase
+00026540: 742e 7261 7465 7329 202d 2064 6174 6173  t.rates) - datas
+00026550: 6574 2e6c 6f67 7261 7465 5f70 6d0a 2020  et.lograte_pm.  
+00026560: 2020 2020 2020 5d0a 2020 2020 656c 7365        ].    else
+00026570: 3a0a 2020 2020 2020 2020 616c 6c5f 6461  :.        all_da
+00026580: 7461 203d 205b 0a20 2020 2020 2020 2020  ta = [.         
+00026590: 2020 206e 702e 6c6f 6731 3028 6461 7461     np.log10(data
+000265a0: 7365 742e 7261 7465 7329 0a20 2020 2020  set.rates).     
+000265b0: 2020 205d 0a20 2020 2020 2020 2061 6c6c     ].        all
+000265c0: 5f64 6174 6120 2b3d 205b 0a20 2020 2020  _data += [.     
+000265d0: 2020 2020 2020 206e 702e 6c6f 6731 3028         np.log10(
+000265e0: 6461 7461 7365 742e 7261 7465 7329 0a20  dataset.rates). 
+000265f0: 2020 2020 2020 205d 0a0a 2020 2020 6775         ]..    gu
+00026600: 692e 666f 726d 6174 5f72 6174 655f 785f  i.format_rate_x_
+00026610: 795f 6178 6573 280a 2020 2020 2020 2020  y_axes(.        
+00026620: 6178 2c0a 2020 2020 2020 2020 6461 7461  ax,.        data
+00026630: 7365 742e 7261 7465 732c 0a20 2020 2020  set.rates,.     
+00026640: 2020 2078 5f76 616c 732c 0a20 2020 2020     x_vals,.     
+00026650: 2020 206e 702e 6162 7328 6461 7461 7365     np.abs(datase
+00026660: 742e 7261 7465 5f70 6d29 2c0a 2020 2020  t.rate_pm),.    
+00026670: 2020 2020 785f 7479 7065 3d78 5f74 7970      x_type=x_typ
+00026680: 650a 2020 2020 290a 0a20 2020 2023 2053  e.    )..    # S
+00026690: 6574 2078 2074 6963 6b20 666f 726d 6174  et x tick format
+000266a0: 7469 6e67 0a20 2020 2067 7569 2e73 6574  ting.    gui.set
+000266b0: 5f72 6174 655f 7874 6963 6b5f 666f 726d  _rate_xtick_form
+000266c0: 6174 7469 6e67 2861 782c 2078 5f76 616c  atting(ax, x_val
+000266d0: 732c 2078 5f74 7970 653d 2766 6965 6c64  s, x_type='field
+000266e0: 2729 0a0a 2020 2020 6669 672e 7469 6768  ')..    fig.tigh
+000266f0: 745f 6c61 796f 7574 2829 0a0a 2020 2020  t_layout()..    
+00026700: 2320 5375 7070 7265 7373 2073 796d 6c6f  # Suppress symlo
+00026710: 6720 7761 726e 696e 670a 2020 2020 7761  g warning.    wa
+00026720: 726e 696e 6773 2e66 696c 7465 7277 6172  rnings.filterwar
+00026730: 6e69 6e67 7328 2769 676e 6f72 6527 2c20  nings('ignore', 
+00026740: 2755 7365 7257 6172 6e69 6e67 2729 0a0a  'UserWarning')..
+00026750: 2020 2020 6966 2073 6176 653a 0a20 2020      if save:.   
+00026760: 2020 2020 2070 6c74 2e73 6176 6566 6967       plt.savefig
+00026770: 2873 6176 655f 6e61 6d65 290a 2020 2020  (save_name).    
+00026780: 2020 2020 6966 2076 6572 626f 7365 3a0a      if verbose:.
+00026790: 2020 2020 2020 2020 2020 2020 7574 2e63              ut.c
+000267a0: 7072 696e 7428 0a20 2020 2020 2020 2020  print(.         
+000267b0: 2020 2020 2020 2066 275c 6e20 5265 6c61         f'\n Rela
+000267c0: 7861 7469 6f6e 2070 6c6f 7420 7361 7665  xation plot save
+000267d0: 6420 746f 205c 6e20 7b73 6176 655f 6e61  d to \n {save_na
+000267e0: 6d65 7d5c 6e27 2c0a 2020 2020 2020 2020  me}\n',.        
+000267f0: 2020 2020 2020 2020 2763 7961 6e27 0a20          'cyan'. 
+00026800: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00026810: 2069 6620 7368 6f77 3a0a 2020 2020 2020   if show:.      
+00026820: 2020 706c 742e 7368 6f77 2829 0a0a 2020    plt.show()..  
+00026830: 2020 2320 5265 656e 6162 6c65 2073 796d    # Reenable sym
+00026840: 6c6f 6720 7761 726e 696e 670a 2020 2020  log warning.    
+00026850: 7761 726e 696e 6773 2e66 696c 7465 7277  warnings.filterw
+00026860: 6172 6e69 6e67 7328 2764 6566 6175 6c74  arnings('default
+00026870: 272c 2027 5573 6572 5761 726e 696e 6727  ', 'UserWarning'
+00026880: 290a 0a20 2020 2072 6574 7572 6e20 6669  )..    return fi
+00026890: 672c 2061 780a 0a0a 6465 6620 706c 6f74  g, ax...def plot
+000268a0: 5f72 6174 655f 7265 7369 6475 616c 7328  _rate_residuals(
+000268b0: 6461 7461 7365 743a 2054 6175 5444 6174  dataset: TauTDat
+000268c0: 6173 6574 2c0a 2020 2020 2020 2020 2020  aset,.          
+000268d0: 2020 2020 2020 2020 2020 2020 2020 6d6f                mo
+000268e0: 6465 6c3a 204c 6f67 5461 7554 4d6f 6465  del: LogTauTMode
+000268f0: 6c20 7c20 4d75 6c74 694c 6f67 5461 7554  l | MultiLogTauT
+00026900: 4d6f 6465 6c20 7c20 4c6f 6754 6175 484d  Model | LogTauHM
+00026910: 6f64 656c 207c 204d 756c 7469 4c6f 6754  odel | MultiLogT
+00026920: 6175 484d 6f64 656c 2c20 2320 6e6f 7161  auHModel, # noqa
+00026930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00026940: 2020 2020 2020 2020 2073 6176 653a 2062           save: b
+00026950: 6f6f 6c20 3d20 4661 6c73 652c 2073 686f  ool = False, sho
+00026960: 773a 2062 6f6f 6c20 3d20 5472 7565 2c0a  w: bool = True,.
+00026970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026980: 2020 2020 2020 2020 7361 7665 5f6e 616d          save_nam
+00026990: 653a 2073 7472 203d 2027 6d6f 6465 6c5f  e: str = 'model_
+000269a0: 7265 7369 6475 616c 5f74 6175 2e70 6e67  residual_tau.png
+000269b0: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+000269c0: 2020 2020 2020 2020 2020 2076 6572 626f             verbo
+000269d0: 7365 3a20 626f 6f6c 203d 2054 7275 6529  se: bool = True)
+000269e0: 202d 3e20 7475 706c 655b 706c 742e 4669   -> tuple[plt.Fi
+000269f0: 6775 7265 2c20 706c 742e 4178 6573 5d3a  gure, plt.Axes]:
+00026a00: 0a20 2020 2027 2727 0a20 2020 2050 6c6f  .    '''.    Plo
+00026a10: 7473 2064 6966 6665 7265 6e63 6520 6f66  ts difference of
+00026a20: 206c 6f67 3130 2865 7870 6572 696d 656e   log10(experimen
+00026a30: 7429 2061 6e64 206c 6f67 3130 286d 6f64  t) and log10(mod
+00026a40: 656c 2920 7265 6c61 7861 7469 6f6e 2072  el) relaxation r
+00026a50: 6174 6573 0a20 2020 2028 6c6f 6731 3028  ates.    (log10(
+00026a60: 6578 7065 7269 6d65 6e74 5f72 6174 6529  experiment_rate)
+00026a70: 202d 206c 6f67 3130 286d 6f64 656c 5f72   - log10(model_r
+00026a80: 6174 6529 2076 7320 5465 6d70 6572 6174  ate) vs Temperat
+00026a90: 7572 6520 6f72 2046 6965 6c64 290a 0a20  ure or Field).. 
+00026aa0: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+00026ab0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+00026ac0: 2064 6174 6173 6574 3a20 5461 7554 4461   dataset: TauTDa
+00026ad0: 7461 7365 7420 7c20 5461 7548 4461 7461  taset | TauHData
+00026ae0: 7365 740a 2020 2020 2020 2020 4461 7461  set.        Data
+00026af0: 7365 7420 746f 2070 6c6f 740a 2020 2020  set to plot.    
+00026b00: 6d6f 6465 6c3a 204c 6f67 5461 7554 4d6f  model: LogTauTMo
+00026b10: 6465 6c20 7c20 4d75 6c74 694c 6f67 5461  del | MultiLogTa
+00026b20: 7554 4d6f 6465 6c20 7c20 4c6f 6754 6175  uTModel | LogTau
+00026b30: 484d 6f64 656c 207c 204d 756c 7469 4c6f  HModel | MultiLo
+00026b40: 6754 6175 484d 6f64 656c 0a20 2020 2020  gTauHModel.     
+00026b50: 2020 204d 6f64 656c 2028 6669 7474 6564     Model (fitted
+00026b60: 2920 746f 2070 6c6f 740a 2020 2020 7368  ) to plot.    sh
+00026b70: 6f77 3a20 626f 6f6c 2c20 6465 6661 756c  ow: bool, defaul
+00026b80: 7420 5472 7565 0a20 2020 2020 2020 2049  t True.        I
+00026b90: 6620 5472 7565 2c20 7368 6f77 2070 6c6f  f True, show plo
+00026ba0: 7420 6f6e 2073 6372 6565 6e0a 2020 2020  t on screen.    
+00026bb0: 7361 7665 3a20 626f 6f6c 2c20 6465 6661  save: bool, defa
+00026bc0: 756c 7420 4661 6c73 650a 2020 2020 2020  ult False.      
+00026bd0: 2020 4966 2054 7275 652c 2073 6176 6520    If True, save 
+00026be0: 706c 6f74 2074 6f20 6669 6c65 2060 7361  plot to file `sa
+00026bf0: 7665 5f6e 616d 6560 0a20 2020 2073 6176  ve_name`.    sav
+00026c00: 655f 6e61 6d65 3a20 7374 722c 2064 6566  e_name: str, def
+00026c10: 6175 6c74 2027 6d6f 6465 6c5f 7265 7369  ault 'model_resi
+00026c20: 6475 616c 5f74 6175 2e70 6e67 270a 2020  dual_tau.png'.  
+00026c30: 2020 2020 2020 4966 2073 6176 6520 6973        If save is
+00026c40: 2054 7275 652c 2077 696c 6c20 7361 7665   True, will save
+00026c50: 2070 6c6f 7420 746f 2074 6869 7320 6669   plot to this fi
+00026c60: 6c65 6e61 6d65 0a20 2020 2076 6572 626f  lename.    verbo
+00026c70: 7365 3a20 626f 6f6c 2c20 6465 6661 756c  se: bool, defaul
+00026c80: 7420 5472 7565 0a20 2020 2020 2020 2049  t True.        I
+00026c90: 6620 5472 7565 2c20 706c 6f74 2066 696c  f True, plot fil
+00026ca0: 6520 6c6f 6361 7469 6f6e 2069 7320 7772  e location is wr
+00026cb0: 6974 7465 6e20 746f 2074 6572 6d69 6e61  itten to termina
+00026cc0: 6c0a 0a20 2020 2052 6574 7572 6e73 0a20  l..    Returns. 
+00026cd0: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2070     -------.    p
+00026ce0: 6c74 2e46 6967 7572 650a 2020 2020 2020  lt.Figure.      
+00026cf0: 2020 4d61 7470 6c6f 746c 6962 2066 6967    Matplotlib fig
+00026d00: 7572 6520 6f62 6a65 6374 0a20 2020 2070  ure object.    p
+00026d10: 6c74 2e41 7865 730a 2020 2020 2020 2020  lt.Axes.        
+00026d20: 4d61 7470 6c6f 746c 6962 2061 7869 7320  Matplotlib axis 
+00026d30: 6f62 6a65 6374 0a20 2020 2027 2727 0a20  object.    '''. 
+00026d40: 2020 2023 2043 7265 6174 6520 6669 6775     # Create figu
+00026d50: 7265 2061 6e64 2061 7865 730a 2020 2020  re and axes.    
+00026d60: 6669 672c 2061 7820 3d20 706c 742e 7375  fig, ax = plt.su
+00026d70: 6270 6c6f 7473 280a 2020 2020 2020 2020  bplots(.        
+00026d80: 312c 0a20 2020 2020 2020 2031 2c0a 2020  1,.        1,.  
+00026d90: 2020 2020 2020 6669 6773 697a 653d 5b36        figsize=[6
+00026da0: 2c20 365d 2c0a 2020 2020 2020 2020 6e75  , 6],.        nu
+00026db0: 6d3d 2752 6573 6964 7561 6c73 270a 2020  m='Residuals'.  
+00026dc0: 2020 290a 0a20 2020 205f 706c 6f74 5f72    )..    _plot_r
+00026dd0: 6174 655f 7265 7369 6475 616c 7328 6461  ate_residuals(da
+00026de0: 7461 7365 742c 206d 6f64 656c 2c20 6178  taset, model, ax
+00026df0: 290a 0a20 2020 2066 6967 2e74 6967 6874  )..    fig.tight
+00026e00: 5f6c 6179 6f75 7428 290a 0a20 2020 2023  _layout()..    #
+00026e10: 2053 6176 6520 706c 6f74 0a20 2020 2069   Save plot.    i
+00026e20: 6620 7361 7665 3a0a 2020 2020 2020 2020  f save:.        
+00026e30: 706c 742e 7361 7665 6669 6728 7361 7665  plt.savefig(save
+00026e40: 5f6e 616d 652c 2064 7069 3d33 3030 290a  _name, dpi=300).
+00026e50: 2020 2020 2020 2020 6966 2076 6572 626f          if verbo
+00026e60: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00026e70: 7574 2e63 7072 696e 7428 0a20 2020 2020  ut.cprint(.     
+00026e80: 2020 2020 2020 2020 2020 2066 275c 6e20             f'\n 
+00026e90: 5261 7465 2072 6573 6964 7561 6c73 2070  Rate residuals p
+00026ea0: 6c6f 7420 7361 7665 6420 746f 205c 6e20  lot saved to \n 
+00026eb0: 7b73 6176 655f 6e61 6d65 7d5c 6e27 2c0a  {save_name}\n',.
+00026ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026ed0: 2763 7961 6e27 0a20 2020 2020 2020 2020  'cyan'.         
+00026ee0: 2020 2029 0a20 2020 2069 6620 7368 6f77     ).    if show
+00026ef0: 3a0a 2020 2020 2020 2020 706c 742e 7368  :.        plt.sh
+00026f00: 6f77 2829 0a0a 2020 2020 7265 7475 726e  ow()..    return
+00026f10: 2066 6967 2c20 6178 0a0a 0a64 6566 2071   fig, ax...def q
+00026f20: 745f 706c 6f74 5f72 6174 655f 7265 7369  t_plot_rate_resi
+00026f30: 6475 616c 7328 6170 703a 2051 7457 6964  duals(app: QtWid
+00026f40: 6765 7473 2e51 4170 706c 6963 6174 696f  gets.QApplicatio
+00026f50: 6e2c 2064 6174 6173 6574 3a20 5461 7554  n, dataset: TauT
+00026f60: 4461 7461 7365 742c 0a20 2020 2020 2020  Dataset,.       
+00026f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026f80: 2020 2020 6d6f 6465 6c3a 204c 6f67 5461      model: LogTa
+00026f90: 7554 4d6f 6465 6c20 7c20 4d75 6c74 694c  uTModel | MultiL
+00026fa0: 6f67 5461 7554 4d6f 6465 6c20 7c20 4c6f  ogTauTModel | Lo
+00026fb0: 6754 6175 484d 6f64 656c 207c 204d 756c  gTauHModel | Mul
+00026fc0: 7469 4c6f 6754 6175 484d 6f64 656c 2c20  tiLogTauHModel, 
+00026fd0: 2320 6e6f 7161 0a20 2020 2020 2020 2020  # noqa.         
+00026fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026ff0: 2020 7361 7665 3a20 626f 6f6c 203d 2046    save: bool = F
+00027000: 616c 7365 2c20 7368 6f77 3a20 626f 6f6c  alse, show: bool
+00027010: 203d 2054 7275 652c 0a20 2020 2020 2020   = True,.       
+00027020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027030: 2020 2020 7361 7665 5f6e 616d 653a 2073      save_name: s
+00027040: 7472 203d 2027 6d6f 6465 6c5f 7265 7369  tr = 'model_resi
+00027050: 6475 616c 5f74 6175 2e70 6e67 272c 0a20  dual_tau.png',. 
+00027060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027070: 2020 2020 2020 2020 2020 7665 7262 6f73            verbos
+00027080: 653a 2062 6f6f 6c20 3d20 5472 7565 2920  e: bool = True) 
+00027090: 2d3e 204e 6f6e 653a 0a20 2020 2027 2727  -> None:.    '''
+000270a0: 0a20 2020 2050 6c6f 7473 2064 6966 6665  .    Plots diffe
+000270b0: 7265 6e63 6520 6f66 206c 6f67 3130 2865  rence of log10(e
+000270c0: 7870 6572 696d 656e 7429 2061 6e64 206c  xperiment) and l
+000270d0: 6f67 3130 286d 6f64 656c 2920 7265 6c61  og10(model) rela
+000270e0: 7861 7469 6f6e 2072 6174 6573 0a20 2020  xation rates.   
+000270f0: 2069 6e20 6120 7174 2077 696e 646f 7720   in a qt window 
+00027100: 7573 696e 6720 6d61 7470 6c6f 746c 6962  using matplotlib
+00027110: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
+00027120: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
+00027130: 2020 2020 6170 703a 2051 7457 6964 6765      app: QtWidge
+00027140: 7473 2e51 4170 706c 6963 6174 696f 6e0a  ts.QApplication.
+00027150: 2020 2020 2020 2020 4170 706c 6963 6174          Applicat
+00027160: 696f 6e20 7573 6564 2062 7920 6375 7272  ion used by curr
+00027170: 656e 7420 7072 6f67 7261 6d0a 2020 2020  ent program.    
+00027180: 2020 2020 4372 6561 7465 2077 6974 6820      Create with 
+00027190: 6061 7070 3d51 7457 6964 6765 7473 2e51  `app=QtWidgets.Q
+000271a0: 4170 706c 6963 6174 696f 6e28 5b5d 2960  Application([])`
+000271b0: 0a20 2020 2064 6174 6173 6574 3a20 5461  .    dataset: Ta
+000271c0: 7554 4461 7461 7365 7420 7c20 5461 7548  uTDataset | TauH
+000271d0: 4461 7461 7365 740a 2020 2020 2020 2020  Dataset.        
+000271e0: 4461 7461 7365 7420 746f 2070 6c6f 740a  Dataset to plot.
+000271f0: 2020 2020 6d6f 6465 6c3a 204c 6f67 5461      model: LogTa
+00027200: 7554 4d6f 6465 6c20 7c20 4d75 6c74 694c  uTModel | MultiL
+00027210: 6f67 5461 7554 4d6f 6465 6c20 7c20 4c6f  ogTauTModel | Lo
+00027220: 6754 6175 484d 6f64 656c 207c 204d 756c  gTauHModel | Mul
+00027230: 7469 4c6f 6754 6175 484d 6f64 656c 0a20  tiLogTauHModel. 
+00027240: 2020 2020 2020 204d 6f64 656c 2028 6669         Model (fi
+00027250: 7474 6564 2920 746f 2070 6c6f 740a 2020  tted) to plot.  
+00027260: 2020 7368 6f77 3a20 626f 6f6c 2c20 6465    show: bool, de
+00027270: 6661 756c 7420 5472 7565 0a20 2020 2020  fault True.     
+00027280: 2020 2049 6620 5472 7565 2c20 7368 6f77     If True, show
+00027290: 2070 6c6f 7420 6f6e 2073 6372 6565 6e0a   plot on screen.
+000272a0: 2020 2020 7361 7665 3a20 626f 6f6c 2c20      save: bool, 
+000272b0: 6465 6661 756c 7420 4661 6c73 650a 2020  default False.  
+000272c0: 2020 2020 2020 4966 2054 7275 652c 2073        If True, s
+000272d0: 6176 6520 706c 6f74 2074 6f20 6669 6c65  ave plot to file
+000272e0: 2060 7361 7665 5f6e 616d 6560 0a20 2020   `save_name`.   
+000272f0: 2073 6176 655f 6e61 6d65 3a20 7374 722c   save_name: str,
+00027300: 2064 6566 6175 6c74 2027 6d6f 6465 6c5f   default 'model_
+00027310: 7265 7369 6475 616c 5f74 6175 2e70 6e67  residual_tau.png
+00027320: 270a 2020 2020 2020 2020 4966 2073 6176  '.        If sav
+00027330: 6520 6973 2054 7275 652c 2077 696c 6c20  e is True, will 
+00027340: 7361 7665 2070 6c6f 7420 746f 2074 6869  save plot to thi
+00027350: 7320 6669 6c65 6e61 6d65 0a20 2020 2076  s filename.    v
+00027360: 6572 626f 7365 3a20 626f 6f6c 2c20 6465  erbose: bool, de
+00027370: 6661 756c 7420 5472 7565 0a20 2020 2020  fault True.     
+00027380: 2020 2049 6620 5472 7565 2c20 706c 6f74     If True, plot
+00027390: 2066 696c 6520 6c6f 6361 7469 6f6e 2069   file location i
+000273a0: 7320 7772 6974 7465 6e20 746f 2074 6572  s written to ter
+000273b0: 6d69 6e61 6c0a 0a20 2020 2052 6574 7572  minal..    Retur
+000273c0: 6e73 0a20 2020 202d 2d2d 2d2d 2d2d 0a20  ns.    -------. 
+000273d0: 2020 204e 6f6e 650a 2020 2020 2727 270a     None.    '''.
+000273e0: 0a20 2020 2077 696e 646f 7720 3d20 6775  .    window = gu
+000273f0: 692e 4d61 7470 6c6f 746c 6962 5769 6e64  i.MatplotlibWind
+00027400: 6f77 2829 0a20 2020 2077 696e 646f 772e  ow().    window.
+00027410: 7365 7457 696e 646f 7754 6974 6c65 2827  setWindowTitle('
+00027420: 5265 7369 6475 616c 7327 290a 0a20 2020  Residuals')..   
+00027430: 205f 706c 6f74 5f72 6174 655f 7265 7369   _plot_rate_resi
+00027440: 6475 616c 7328 6461 7461 7365 742c 206d  duals(dataset, m
+00027450: 6f64 656c 2c20 7769 6e64 6f77 2e73 632e  odel, window.sc.
+00027460: 6178 290a 0a20 2020 2023 2053 6176 6520  ax)..    # Save 
+00027470: 706c 6f74 0a20 2020 2069 6620 7361 7665  plot.    if save
+00027480: 3a0a 2020 2020 2020 2020 7769 6e64 6f77  :.        window
+00027490: 2e73 632e 6669 672e 7361 7665 6669 6728  .sc.fig.savefig(
+000274a0: 7361 7665 5f6e 616d 652c 2064 7069 3d33  save_name, dpi=3
+000274b0: 3030 290a 2020 2020 2020 2020 6966 2076  00).        if v
+000274c0: 6572 626f 7365 3a0a 2020 2020 2020 2020  erbose:.        
+000274d0: 2020 2020 7574 2e63 7072 696e 7428 0a20      ut.cprint(. 
+000274e0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+000274f0: 275c 6e20 5261 7465 2072 6573 6964 7561  '\n Rate residua
+00027500: 6c73 2070 6c6f 7420 7361 7665 6420 746f  ls plot saved to
+00027510: 205c 6e20 7b73 6176 655f 6e61 6d65 7d5c   \n {save_name}\
+00027520: 6e27 2c0a 2020 2020 2020 2020 2020 2020  n',.            
+00027530: 2020 2020 2763 7961 6e27 0a20 2020 2020      'cyan'.     
+00027540: 2020 2020 2020 2029 0a0a 2020 2020 6966         )..    if
+00027550: 2073 686f 773a 0a20 2020 2020 2020 2077   show:.        w
+00027560: 696e 646f 772e 7368 6f77 2829 0a20 2020  indow.show().   
+00027570: 2020 2020 2023 2043 616c 6c20 7477 6963       # Call twic
+00027580: 6520 656c 7365 2069 7420 776f 6e74 2077  e else it wont w
+00027590: 6f72 6b21 0a20 2020 2020 2020 2077 696e  ork!.        win
+000275a0: 646f 772e 7363 2e66 6967 2e74 6967 6874  dow.sc.fig.tight
+000275b0: 5f6c 6179 6f75 7428 290a 2020 2020 2020  _layout().      
+000275c0: 2020 7769 6e64 6f77 2e73 632e 6669 672e    window.sc.fig.
+000275d0: 7469 6768 745f 6c61 796f 7574 2829 0a20  tight_layout(). 
+000275e0: 2020 2020 2020 2061 7070 2e65 7865 635f         app.exec_
+000275f0: 2829 0a0a 2020 2020 7265 7475 726e 0a0a  ()..    return..
+00027600: 0a64 6566 205f 706c 6f74 5f72 6174 655f  .def _plot_rate_
+00027610: 7265 7369 6475 616c 7328 6461 7461 7365  residuals(datase
+00027620: 743a 2054 6175 5444 6174 6173 6574 207c  t: TauTDataset |
+00027630: 2054 6175 4844 6174 6173 6574 2c0a 2020   TauHDataset,.  
+00027640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027650: 2020 2020 2020 206d 6f64 656c 3a20 4c6f         model: Lo
+00027660: 6754 6175 544d 6f64 656c 207c 204d 756c  gTauTModel | Mul
+00027670: 7469 4c6f 6754 6175 544d 6f64 656c 207c  tiLogTauTModel |
+00027680: 204c 6f67 5461 7548 4d6f 6465 6c20 7c20   LogTauHModel | 
+00027690: 4d75 6c74 694c 6f67 5461 7548 4d6f 6465  MultiLogTauHMode
+000276a0: 6c2c 2023 206e 6f71 610a 2020 2020 2020  l, # noqa.      
+000276b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000276c0: 2020 2061 783a 2070 6c74 2e41 7865 7329     ax: plt.Axes)
+000276d0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2727   -> None:.    ''
+000276e0: 270a 2020 2020 506c 6f74 7320 6469 6666  '.    Plots diff
+000276f0: 6572 656e 6365 206f 6620 6c6f 6731 3028  erence of log10(
+00027700: 6578 7065 7269 6d65 6e74 2920 616e 6420  experiment) and 
+00027710: 6c6f 6731 3028 6d6f 6465 6c29 2072 656c  log10(model) rel
+00027720: 6178 6174 696f 6e20 7261 7465 730a 2020  axation rates.  
+00027730: 2020 6f6e 746f 2061 2067 6976 656e 2066    onto a given f
+00027740: 6967 7572 6520 616e 6420 6178 6973 0a0a  igure and axis..
+00027750: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+00027760: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+00027770: 2020 6d6f 6465 6c73 3a20 6c69 7374 5b4c    models: list[L
+00027780: 6f67 5461 7554 4d6f 6465 6c20 7c20 4d75  ogTauTModel | Mu
+00027790: 6c74 694c 6f67 5461 7554 4d6f 6465 6c20  ltiLogTauTModel 
+000277a0: 7c20 4c6f 6754 6175 484d 6f64 656c 207c  | LogTauHModel |
+000277b0: 204d 756c 7469 4c6f 6754 6175 484d 6f64   MultiLogTauHMod
+000277c0: 656c 5d0a 2020 2020 2020 2020 4d6f 6465  el].        Mode
+000277d0: 6c73 2c20 6f6e 6520 7065 7220 7465 6d70  ls, one per temp
+000277e0: 6572 6174 7572 650a 2020 2020 6669 6c65  erature.    file
+000277f0: 5f6e 616d 653a 2073 7472 0a20 2020 2020  _name: str.     
+00027800: 2020 204e 616d 6520 6f66 206f 7574 7075     Name of outpu
+00027810: 7420 6669 6c65 0a20 2020 2061 783a 2070  t file.    ax: p
+00027820: 6c74 2e41 7865 730a 2020 2020 2020 2020  lt.Axes.        
+00027830: 4d61 7470 6c6f 746c 6962 2041 7869 7320  Matplotlib Axis 
+00027840: 6f62 6a65 6374 2075 7365 6420 666f 7220  object used for 
+00027850: 706c 6f74 0a0a 2020 2020 5265 7475 726e  plot..    Return
+00027860: 730a 2020 2020 2d2d 2d2d 2d2d 2d0a 2020  s.    -------.  
+00027870: 2020 4e6f 6e65 0a20 2020 2027 2727 2023    None.    ''' #
+00027880: 206e 6f71 610a 0a20 2020 2069 6620 6973   noqa..    if is
+00027890: 696e 7374 616e 6365 2864 6174 6173 6574  instance(dataset
+000278a0: 2c20 5461 7548 4461 7461 7365 7429 3a0a  , TauHDataset):.
+000278b0: 2020 2020 2020 2020 785f 7661 6c73 203d          x_vals =
+000278c0: 2064 6174 6173 6574 2e66 6965 6c64 730a   dataset.fields.
+000278d0: 2020 2020 2020 2020 6178 2e73 6574 5f78          ax.set_x
+000278e0: 6c61 6265 6c28 7227 4669 656c 6420 284f  label(r'Field (O
+000278f0: 6529 2729 0a20 2020 2065 6c69 6620 6973  e)').    elif is
+00027900: 696e 7374 616e 6365 2864 6174 6173 6574  instance(dataset
+00027910: 2c20 5461 7554 4461 7461 7365 7429 3a0a  , TauTDataset):.
+00027920: 2020 2020 2020 2020 785f 7661 6c73 203d          x_vals =
+00027930: 2064 6174 6173 6574 2e74 656d 7065 7261   dataset.tempera
+00027940: 7475 7265 730a 2020 2020 2020 2020 6178  tures.        ax
+00027950: 2e73 6574 5f78 6c61 6265 6c28 7227 5465  .set_xlabel(r'Te
+00027960: 6d70 6572 6174 7572 6520 284b 2927 290a  mperature (K)').
+00027970: 0a20 2020 2023 2041 6464 2061 6464 6974  .    # Add addit
+00027980: 696f 6e61 6c20 7365 7420 6f66 2061 7865  ional set of axe
+00027990: 7320 746f 2063 7265 6174 6520 277a 6572  s to create 'zer
+000279a0: 6f27 206c 696e 650a 2020 2020 6178 3220  o' line.    ax2 
+000279b0: 3d20 6178 2e74 7769 6e79 2829 0a20 2020  = ax.twiny().   
+000279c0: 2061 7832 2e67 6574 5f79 6178 6973 2829   ax2.get_yaxis()
+000279d0: 2e73 6574 5f76 6973 6962 6c65 2846 616c  .set_visible(Fal
+000279e0: 7365 290a 2020 2020 6178 322e 7365 745f  se).    ax2.set_
+000279f0: 7974 6963 6b73 285b 5d29 0a20 2020 2061  yticks([]).    a
+00027a00: 7832 2e73 6574 5f78 7469 636b 7328 5b5d  x2.set_xticks([]
+00027a10: 290a 2020 2020 6178 322e 7370 696e 6573  ).    ax2.spines
+00027a20: 5b27 626f 7474 6f6d 275d 2e73 6574 5f70  ['bottom'].set_p
+00027a30: 6f73 6974 696f 6e28 2827 7a65 726f 2729  osition(('zero')
+00027a40: 290a 0a20 2020 2069 6620 7479 7065 286d  )..    if type(m
+00027a50: 6f64 656c 2920 696e 205b 4d75 6c74 694c  odel) in [MultiL
+00027a60: 6f67 5461 7554 4d6f 6465 6c2c 204d 756c  ogTauTModel, Mul
+00027a70: 7469 4c6f 6754 6175 484d 6f64 656c 5d3a  tiLogTauHModel]:
+00027a80: 0a20 2020 2020 2020 206c 6f67 6d6f 6465  .        logmode
+00027a90: 6c73 203d 206d 6f64 656c 2e6c 6f67 6d6f  ls = model.logmo
+00027aa0: 6465 6c73 0a20 2020 2065 6c73 653a 0a20  dels.    else:. 
+00027ab0: 2020 2020 2020 206c 6f67 6d6f 6465 6c73         logmodels
+00027ac0: 203d 205b 6d6f 6465 6c5d 0a0a 2020 2020   = [model]..    
+00027ad0: 6d6f 6465 6c5f 7261 7465 203d 206e 702e  model_rate = np.
+00027ae0: 7a65 726f 7328 6c65 6e28 785f 7661 6c73  zeros(len(x_vals
+00027af0: 2929 0a0a 2020 2020 666f 7220 6c6f 676d  ))..    for logm
+00027b00: 6f64 656c 2069 6e20 6c6f 676d 6f64 656c  odel in logmodel
+00027b10: 733a 0a20 2020 2020 2020 206d 6f64 656c  s:.        model
+00027b20: 5f72 6174 6520 2b3d 2031 302a 2a6c 6f67  _rate += 10**log
+00027b30: 6d6f 6465 6c2e 6d6f 6465 6c28 0a20 2020  model.model(.   
+00027b40: 2020 2020 2020 2020 206c 6f67 6d6f 6465           logmode
+00027b50: 6c2e 6669 6e61 6c5f 7661 725f 7661 6c75  l.final_var_valu
+00027b60: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
+00027b70: 785f 7661 6c73 2c0a 2020 2020 2020 2020  x_vals,.        
+00027b80: 290a 0a20 2020 206d 6f64 656c 5f6c 6f67  )..    model_log
+00027b90: 7261 7465 203d 206e 702e 6c6f 6731 3028  rate = np.log10(
+00027ba0: 6d6f 6465 6c5f 7261 7465 290a 0a20 2020  model_rate)..   
+00027bb0: 2023 2050 6c6f 7420 7265 7369 6475 616c   # Plot residual
+00027bc0: 730a 2020 2020 6966 206c 656e 2864 6174  s.    if len(dat
+00027bd0: 6173 6574 2e6c 6f67 7261 7465 5f70 6d29  aset.lograte_pm)
+00027be0: 3a0a 2020 2020 2020 2020 6178 2e65 7272  :.        ax.err
+00027bf0: 6f72 6261 7228 0a20 2020 2020 2020 2020  orbar(.         
+00027c00: 2020 2078 5f76 616c 732c 0a20 2020 2020     x_vals,.     
+00027c10: 2020 2020 2020 206e 702e 6c6f 6731 3028         np.log10(
+00027c20: 6461 7461 7365 742e 7261 7465 7329 202d  dataset.rates) -
+00027c30: 206d 6f64 656c 5f6c 6f67 7261 7465 2c0a   model_lograte,.
+00027c40: 2020 2020 2020 2020 2020 2020 7965 7272              yerr
+00027c50: 3d64 6174 6173 6574 2e6c 6f67 7261 7465  =dataset.lograte
+00027c60: 5f70 6d2c 0a20 2020 2020 2020 2020 2020  _pm,.           
+00027c70: 2066 6d74 3d27 622e 270a 2020 2020 2020   fmt='b.'.      
+00027c80: 2020 290a 2020 2020 656c 7365 3a0a 2020    ).    else:.  
+00027c90: 2020 2020 2020 6178 2e70 6c6f 7428 0a20        ax.plot(. 
+00027ca0: 2020 2020 2020 2020 2020 2078 5f76 616c             x_val
+00027cb0: 732c 0a20 2020 2020 2020 2020 2020 206e  s,.            n
+00027cc0: 702e 6c6f 6731 3028 6461 7461 7365 742e  p.log10(dataset.
+00027cd0: 7261 7465 7329 202d 206d 6f64 656c 5f6c  rates) - model_l
+00027ce0: 6f67 7261 7465 2c0a 2020 2020 2020 2020  ograte,.        
+00027cf0: 2020 2020 636f 6c6f 723d 2762 272c 0a20      color='b',. 
+00027d00: 2020 2020 2020 2020 2020 206d 6172 6b65             marke
+00027d10: 723d 276f 272c 0a20 2020 2020 2020 2020  r='o',.         
+00027d20: 2020 206c 773d 302c 0a20 2020 2020 2020     lw=0,.       
+00027d30: 2020 2020 2066 696c 6c73 7479 6c65 3d27       fillstyle='
+00027d40: 6e6f 6e65 272c 0a20 2020 2020 2020 2020  none',.         
+00027d50: 2020 206c 6162 656c 3d27 4578 7065 7269     label='Experi
+00027d60: 6d65 6e74 270a 2020 2020 2020 2020 290a  ment'.        ).
+00027d70: 2020 2020 2320 5365 7420 6c6f 6720 7363      # Set log sc
+00027d80: 616c 6520 6f6e 2078 2061 7869 730a 2020  ale on x axis.  
+00027d90: 2020 6178 2e73 6574 5f78 7363 616c 6528    ax.set_xscale(
+00027da0: 276c 6f67 2729 0a0a 2020 2020 2320 5365  'log')..    # Se
+00027db0: 7420 666f 726d 6174 7469 6e67 2066 6f72  t formatting for
+00027dc0: 2079 2061 7869 7320 6d61 6a6f 7220 7469   y axis major ti
+00027dd0: 636b 730a 2020 2020 6178 2e79 6178 6973  cks.    ax.yaxis
+00027de0: 2e73 6574 5f6d 616a 6f72 5f66 6f72 6d61  .set_major_forma
+00027df0: 7474 6572 2853 6361 6c61 7246 6f72 6d61  tter(ScalarForma
+00027e00: 7474 6572 2829 290a 0a20 2020 2023 2041  tter())..    # A
+00027e10: 6464 206d 696e 6f72 2074 6963 6b73 2074  dd minor ticks t
+00027e20: 6f20 7920 6178 6973 2077 6974 6820 6e6f  o y axis with no
+00027e30: 206c 6162 656c 730a 2020 2020 6178 2e79   labels.    ax.y
+00027e40: 6178 6973 2e73 6574 5f6d 696e 6f72 5f6c  axis.set_minor_l
+00027e50: 6f63 6174 6f72 2841 7574 6f4d 696e 6f72  ocator(AutoMinor
+00027e60: 4c6f 6361 746f 7228 2929 0a0a 2020 2020  Locator())..    
+00027e70: 2320 5379 6d6d 6574 7269 7365 2079 2061  # Symmetrise y a
+00027e80: 7869 7320 6c69 6d69 7473 2062 6173 6564  xis limits based
+00027e90: 206f 6e20 6d61 7820 6162 7320 6572 726f   on max abs erro
+00027ea0: 720a 2020 2020 6966 206c 656e 2864 6174  r.    if len(dat
+00027eb0: 6173 6574 2e6c 6f67 7261 7465 5f70 6d29  aset.lograte_pm)
+00027ec0: 3a0a 2020 2020 2020 2020 616c 6c5f 6461  :.        all_da
+00027ed0: 7461 203d 205b 0a20 2020 2020 2020 2020  ta = [.         
+00027ee0: 2020 206e 702e 6c6f 6731 3028 6461 7461     np.log10(data
+00027ef0: 7365 742e 7261 7465 7329 202d 206d 6f64  set.rates) - mod
+00027f00: 656c 5f6c 6f67 7261 7465 202b 2064 6174  el_lograte + dat
+00027f10: 6173 6574 2e6c 6f67 7261 7465 5f70 6d0a  aset.lograte_pm.
+00027f20: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
+00027f30: 2020 616c 6c5f 6461 7461 202b 3d20 5b0a    all_data += [.
+00027f40: 2020 2020 2020 2020 2020 2020 6e70 2e6c              np.l
+00027f50: 6f67 3130 2864 6174 6173 6574 2e72 6174  og10(dataset.rat
+00027f60: 6573 2920 2d20 6d6f 6465 6c5f 6c6f 6772  es) - model_logr
+00027f70: 6174 6520 2d20 6461 7461 7365 742e 6c6f  ate - dataset.lo
+00027f80: 6772 6174 655f 706d 0a20 2020 2020 2020  grate_pm.       
+00027f90: 205d 0a20 2020 2065 6c73 653a 0a20 2020   ].    else:.   
+00027fa0: 2020 2020 2061 6c6c 5f64 6174 6120 3d20       all_data = 
+00027fb0: 5b0a 2020 2020 2020 2020 2020 2020 6e70  [.            np
+00027fc0: 2e6c 6f67 3130 2864 6174 6173 6574 2e72  .log10(dataset.r
+00027fd0: 6174 6573 2920 2d20 6d6f 6465 6c5f 6c6f  ates) - model_lo
+00027fe0: 6772 6174 650a 2020 2020 2020 2020 5d0a  grate.        ].
+00027ff0: 2020 2020 2020 2020 616c 6c5f 6461 7461          all_data
+00028000: 202b 3d20 5b0a 2020 2020 2020 2020 2020   += [.          
+00028010: 2020 6e70 2e6c 6f67 3130 2864 6174 6173    np.log10(datas
+00028020: 6574 2e72 6174 6573 2920 2d20 6d6f 6465  et.rates) - mode
+00028030: 6c5f 6c6f 6772 6174 650a 2020 2020 2020  l_lograte.      
+00028040: 2020 5d0a 0a20 2020 2074 6963 6b73 2c20    ]..    ticks, 
+00028050: 6d61 7876 616c 203d 2067 7569 2e6d 696e  maxval = gui.min
+00028060: 5f6d 6178 5f74 6963 6b73 5f77 6974 685f  _max_ticks_with_
+00028070: 7a65 726f 2861 6c6c 5f64 6174 612c 2035  zero(all_data, 5
+00028080: 290a 2020 2020 6178 2e73 6574 5f79 7469  ).    ax.set_yti
+00028090: 636b 7328 7469 636b 7329 0a0a 2020 2020  cks(ticks)..    
+000280a0: 6178 2e73 6574 5f79 6c69 6d28 5b2d 206d  ax.set_ylim([- m
+000280b0: 6178 7661 6c20 2a20 312e 312c 202b 206d  axval * 1.1, + m
+000280c0: 6178 7661 6c20 2a20 312e 315d 290a 0a20  axval * 1.1]).. 
+000280d0: 2020 2023 2041 7869 7320 6c61 6265 6c73     # Axis labels
+000280e0: 0a20 2020 2061 782e 7365 745f 796c 6162  .    ax.set_ylab
+000280f0: 656c 280a 2020 2020 2020 2020 7227 245c  el(.        r'$\
+00028100: 6c6f 675f 5c6d 6174 6872 6567 756c 6172  log_\mathregular
+00028110: 7b31 307d 5b5c 7461 755e 5c6d 6174 6872  {10}[\tau^\mathr
+00028120: 6567 756c 6172 7b2d 317d 5f7b 5c6d 6174  egular{-1}_{\mat
+00028130: 6872 6567 756c 6172 7b65 7870 7d7d 5d24  hregular{exp}}]$
+00028140: 202d 2024 5c6c 6f67 5f5c 6d61 7468 7265   - $\log_\mathre
+00028150: 6775 6c61 727b 3130 7d5b 5c74 6175 5e5c  gular{10}[\tau^\
+00028160: 6d61 7468 7265 6775 6c61 727b 2d31 7d5f  mathregular{-1}_
+00028170: 7b5c 6d61 7468 7265 6775 6c61 727b 6669  {\mathregular{fi
+00028180: 747d 7d5d 2427 2023 206e 6f71 610a 2020  t}}]$' # noqa.  
+00028190: 2020 290a 0a20 2020 2023 2053 6574 2078    )..    # Set x
+000281a0: 2074 6963 6b20 666f 726d 6174 7469 6e67   tick formatting
+000281b0: 0a20 2020 2067 7569 2e73 6574 5f72 6174  .    gui.set_rat
+000281c0: 655f 7874 6963 6b5f 666f 726d 6174 7469  e_xtick_formatti
+000281d0: 6e67 2861 782c 2078 5f76 616c 7329 0a0a  ng(ax, x_vals)..
+000281e0: 2020 2020 7265 7475 726e 0a0a 0a64 6566      return...def
+000281f0: 2077 7269 7465 5f6d 6f64 656c 5f70 6172   write_model_par
+00028200: 616d 7328 6d6f 6465 6c3a 204c 6f67 5461  ams(model: LogTa
+00028210: 7554 4d6f 6465 6c20 7c20 4d75 6c74 694c  uTModel | MultiL
+00028220: 6f67 5461 7554 4d6f 6465 6c20 7c20 4c6f  ogTauTModel | Lo
+00028230: 6754 6175 484d 6f64 656c 207c 204d 756c  gTauHModel | Mul
+00028240: 7469 4c6f 6754 6175 484d 6f64 656c 2c20  tiLogTauHModel, 
+00028250: 2320 6e6f 7161 0a20 2020 2020 2020 2020  # noqa.         
+00028260: 2020 2020 2020 2020 2020 2020 2020 6669                fi
+00028270: 6c65 5f6e 616d 653a 2073 7472 2c20 7665  le_name: str, ve
+00028280: 7262 6f73 653a 2062 6f6f 6c20 3d20 5472  rbose: bool = Tr
+00028290: 7565 2920 2d3e 204e 6f6e 653a 0a20 2020  ue) -> None:.   
+000282a0: 2027 2727 0a20 2020 2057 7269 7465 7320   '''.    Writes 
+000282b0: 6669 7474 6564 2061 6e64 2066 6978 6564  fitted and fixed
+000282c0: 2070 6172 616d 6574 6572 7320 6f66 206d   parameters of m
+000282d0: 6f64 656c 2873 2920 746f 2066 696c 650a  odel(s) to file.
+000282e0: 0a20 2020 2050 6172 616d 6574 6572 730a  .    Parameters.
+000282f0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+00028300: 2020 206d 6f64 656c 733a 206c 6973 745b     models: list[
+00028310: 4c6f 6754 6175 544d 6f64 656c 207c 204d  LogTauTModel | M
+00028320: 756c 7469 4c6f 6754 6175 544d 6f64 656c  ultiLogTauTModel
+00028330: 207c 204c 6f67 5461 7548 4d6f 6465 6c20   | LogTauHModel 
+00028340: 7c20 4d75 6c74 694c 6f67 5461 7548 4d6f  | MultiLogTauHMo
+00028350: 6465 6c5d 0a20 2020 2020 2020 204d 6f64  del].        Mod
+00028360: 656c 732c 206f 6e65 2070 6572 2074 656d  els, one per tem
+00028370: 7065 7261 7475 7265 0a20 2020 2066 696c  perature.    fil
+00028380: 655f 6e61 6d65 3a20 7374 720a 2020 2020  e_name: str.    
+00028390: 2020 2020 4e61 6d65 206f 6620 6f75 7470      Name of outp
+000283a0: 7574 2066 696c 650a 2020 2020 7665 7262  ut file.    verb
+000283b0: 6f73 653a 2062 6f6f 6c2c 2064 6566 6175  ose: bool, defau
+000283c0: 6c74 2054 7275 650a 2020 2020 2020 2020  lt True.        
+000283d0: 4966 2054 7275 652c 206f 7574 7075 7420  If True, output 
+000283e0: 6669 6c65 206c 6f63 6174 696f 6e20 6973  file location is
+000283f0: 2077 7269 7474 656e 2074 6f20 7465 726d   written to term
+00028400: 696e 616c 0a0a 2020 2020 5265 7475 726e  inal..    Return
+00028410: 730a 2020 2020 2d2d 2d2d 2d2d 2d0a 2020  s.    -------.  
+00028420: 2020 4e6f 6e65 0a20 2020 2027 2727 2023    None.    ''' #
+00028430: 206e 6f71 610a 0a20 2020 2069 6620 7479   noqa..    if ty
+00028440: 7065 286d 6f64 656c 2920 696e 205b 4d75  pe(model) in [Mu
+00028450: 6c74 694c 6f67 5461 7554 4d6f 6465 6c2c  ltiLogTauTModel,
+00028460: 204d 756c 7469 4c6f 6754 6175 484d 6f64   MultiLogTauHMod
+00028470: 656c 5d3a 0a20 2020 2020 2020 206c 6f67  el]:.        log
+00028480: 6d6f 6465 6c73 203d 206d 6f64 656c 2e6c  models = model.l
+00028490: 6f67 6d6f 6465 6c73 0a20 2020 2065 6c73  ogmodels.    els
+000284a0: 653a 0a20 2020 2020 2020 206c 6f67 6d6f  e:.        logmo
+000284b0: 6465 6c73 203d 205b 6d6f 6465 6c5d 0a0a  dels = [model]..
+000284c0: 2020 2020 6620 3d20 6f70 656e 2866 696c      f = open(fil
+000284d0: 655f 6e61 6d65 2c20 2777 272c 2065 6e63  e_name, 'w', enc
+000284e0: 6f64 696e 673d 2775 7466 2d38 2729 0a0a  oding='utf-8')..
+000284f0: 2020 2020 2320 5772 6974 6520 6561 6368      # Write each
+00028500: 2074 6572 6d27 7320 6e61 6d65 2c20 6669   term's name, fi
+00028510: 7420 7661 7273 2c20 7374 6465 762c 2061  t vars, stdev, a
+00028520: 6e64 2066 6978 2076 6172 730a 2020 2020  nd fix vars.    
+00028530: 666f 7220 6c6f 676d 6f64 656c 2069 6e20  for logmodel in 
+00028540: 6c6f 676d 6f64 656c 733a 0a20 2020 2020  logmodels:.     
+00028550: 2020 2066 2e77 7269 7465 2827 7b7d 5c6e     f.write('{}\n
+00028560: 272e 666f 726d 6174 286c 6f67 6d6f 6465  '.format(logmode
+00028570: 6c2e 4e41 4d45 2929 0a20 2020 2020 2020  l.NAME)).       
+00028580: 2069 6620 6c65 6e28 6c6f 676d 6f64 656c   if len(logmodel
+00028590: 2e66 6974 5f76 6172 732e 6b65 7973 2829  .fit_vars.keys()
+000285a0: 293a 0a20 2020 2020 2020 2020 2020 2066  ):.            f
+000285b0: 2e77 7269 7465 2827 4669 7474 6564 2054  .write('Fitted T
+000285c0: 6572 6d73 3a20 5661 6c75 6520 616e 6420  erms: Value and 
+000285d0: 5374 616e 6461 7264 2044 6576 6961 7469  Standard Deviati
+000285e0: 6f6e 3a5c 6e27 290a 2020 2020 2020 2020  on:\n').        
+000285f0: 2020 2020 666f 7220 6e61 6d65 2069 6e20      for name in 
+00028600: 6c6f 676d 6f64 656c 2e66 6974 5f76 6172  logmodel.fit_var
+00028610: 732e 6b65 7973 2829 3a0a 2020 2020 2020  s.keys():.      
+00028620: 2020 2020 2020 2020 2020 662e 7772 6974            f.writ
+00028630: 6528 277b 3a3e 367d 207b 3a20 312e 3845  e('{:>6} {: 1.8E
+00028640: 7d20 7b3a 2031 2e38 457d 207b 7d5c 6e27  } {: 1.8E} {}\n'
+00028650: 2e66 6f72 6d61 7428 0a20 2020 2020 2020  .format(.       
+00028660: 2020 2020 2020 2020 2020 2020 206e 616d               nam
+00028670: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00028680: 2020 2020 2020 206c 6f67 6d6f 6465 6c2e         logmodel.
+00028690: 6669 6e61 6c5f 7661 725f 7661 6c75 6573  final_var_values
+000286a0: 5b6e 616d 655d 2c0a 2020 2020 2020 2020  [name],.        
+000286b0: 2020 2020 2020 2020 2020 2020 6c6f 676d              logm
+000286c0: 6f64 656c 2e66 6974 5f73 7464 6576 5b6e  odel.fit_stdev[n
+000286d0: 616d 655d 2c0a 2020 2020 2020 2020 2020  ame],.          
+000286e0: 2020 2020 2020 2020 2020 6c6f 676d 6f64            logmod
+000286f0: 656c 2e55 4e49 5453 5b6e 616d 655d 0a20  el.UNITS[name]. 
+00028700: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00028710: 290a 2020 2020 2020 2020 6966 206c 656e  ).        if len
+00028720: 286c 6f67 6d6f 6465 6c2e 6669 785f 7661  (logmodel.fix_va
+00028730: 7273 2e6b 6579 7328 2929 3a0a 2020 2020  rs.keys()):.    
+00028740: 2020 2020 2020 2020 662e 7772 6974 6528          f.write(
+00028750: 2746 6978 6564 2054 6572 6d73 3a20 5661  'Fixed Terms: Va
+00028760: 6c75 6573 5c6e 2729 0a20 2020 2020 2020  lues\n').       
+00028770: 2020 2020 2066 6f72 206e 616d 6520 696e       for name in
+00028780: 206c 6f67 6d6f 6465 6c2e 6669 785f 7661   logmodel.fix_va
+00028790: 7273 2e6b 6579 7328 293a 0a20 2020 2020  rs.keys():.     
+000287a0: 2020 2020 2020 2020 2020 2066 2e77 7269             f.wri
+000287b0: 7465 2827 7b3a 3e36 7d20 7b3a 2031 2e38  te('{:>6} {: 1.8
+000287c0: 457d 207b 7d5c 6e27 2e66 6f72 6d61 7428  E} {}\n'.format(
+000287d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000287e0: 2020 2020 206e 616d 652c 0a20 2020 2020       name,.     
+000287f0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00028800: 6f67 6d6f 6465 6c2e 6669 6e61 6c5f 7661  ogmodel.final_va
+00028810: 725f 7661 6c75 6573 5b6e 616d 655d 2c0a  r_values[name],.
+00028820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028830: 2020 2020 6c6f 676d 6f64 656c 2e55 4e49      logmodel.UNI
+00028840: 5453 5b6e 616d 655d 0a20 2020 2020 2020  TS[name].       
+00028850: 2020 2020 2020 2020 2029 290a 2020 2020           )).    
+00028860: 2020 2020 662e 7772 6974 6528 275c 6e27      f.write('\n'
+00028870: 290a 0a20 2020 2069 6620 7665 7262 6f73  )..    if verbos
+00028880: 653a 0a20 2020 2020 2020 2075 742e 6370  e:.        ut.cp
+00028890: 7269 6e74 280a 2020 2020 2020 2020 2020  rint(.          
+000288a0: 2020 275c 6e20 5265 6c61 7861 7469 6f6e    '\n Relaxation
+000288b0: 204d 6f64 656c 2070 6172 616d 6574 6572   Model parameter
+000288c0: 7320 7772 6974 7465 6e20 746f 205c 6e20  s written to \n 
+000288d0: 7b7d 5c6e 272e 666f 726d 6174 280a 2020  {}\n'.format(.  
+000288e0: 2020 2020 2020 2020 2020 2020 2020 6669                fi
+000288f0: 6c65 5f6e 616d 650a 2020 2020 2020 2020  le_name.        
+00028900: 2020 2020 292c 0a20 2020 2020 2020 2020      ),.         
+00028910: 2020 2027 6379 616e 270a 2020 2020 2020     'cyan'.      
+00028920: 2020 290a 0a20 2020 2072 6574 7572 6e0a    )..    return.
+00028930: 0a0a 6465 6620 7772 6974 655f 6d6f 6465  ..def write_mode
+00028940: 6c5f 6461 7461 2864 6174 6173 6574 3a20  l_data(dataset: 
+00028950: 5461 7554 4461 7461 7365 7420 7c20 5461  TauTDataset | Ta
+00028960: 7548 4461 7461 7365 742c 0a20 2020 2020  uHDataset,.     
+00028970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028980: 6d6f 6465 6c3a 204c 6f67 5461 7554 4d6f  model: LogTauTMo
+00028990: 6465 6c20 7c20 4d75 6c74 694c 6f67 5461  del | MultiLogTa
+000289a0: 7554 4d6f 6465 6c20 7c20 4c6f 6754 6175  uTModel | LogTau
+000289b0: 484d 6f64 656c 207c 204d 756c 7469 4c6f  HModel | MultiLo
+000289c0: 6754 6175 484d 6f64 656c 2c20 2320 6e6f  gTauHModel, # no
+000289d0: 7161 0a20 2020 2020 2020 2020 2020 2020  qa.             
+000289e0: 2020 2020 2020 2020 6669 6c65 5f6e 616d          file_nam
+000289f0: 653a 2073 7472 2c20 7665 7262 6f73 653a  e: str, verbose:
+00028a00: 2062 6f6f 6c20 3d20 5472 7565 2920 2d3e   bool = True) ->
+00028a10: 204e 6f6e 653a 0a20 2020 2027 2727 0a20   None:.    '''. 
+00028a20: 2020 2043 7265 6174 6573 2066 696c 6520     Creates file 
+00028a30: 636f 6e74 6169 6e69 6e67 2072 6174 6520  containing rate 
+00028a40: 7673 2074 656d 7065 7261 7475 7265 2f66  vs temperature/f
+00028a50: 6965 6c64 2063 616c 6375 6c61 7465 6420  ield calculated 
+00028a60: 7573 696e 6720 6d6f 6465 6c0a 2020 2020  using model.    
+00028a70: 7061 7261 6d65 7465 7273 0a0a 2020 2020  parameters..    
+00028a80: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
+00028a90: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6461  ---------.    da
+00028aa0: 7461 7365 743a 2054 6175 5444 6174 6173  taset: TauTDatas
+00028ab0: 6574 207c 2054 6175 4844 6174 6173 6574  et | TauHDataset
+00028ac0: 0a20 2020 2020 2020 2044 6174 6173 6574  .        Dataset
+00028ad0: 2074 6f20 7768 6963 6820 6120 6d6f 6465   to which a mode
+00028ae0: 6c20 7761 7320 7375 6363 6573 7366 756c  l was successful
+00028af0: 6c79 2066 6974 7465 6420 2869 2e65 2e20  ly fitted (i.e. 
+00028b00: 6669 745f 7374 6174 7573 3d54 7275 6529  fit_status=True)
+00028b10: 0a20 2020 206d 6f64 656c 3a20 4c6f 6754  .    model: LogT
+00028b20: 6175 544d 6f64 656c 207c 204d 756c 7469  auTModel | Multi
+00028b30: 4c6f 6754 6175 544d 6f64 656c 207c 204c  LogTauTModel | L
+00028b40: 6f67 5461 7548 4d6f 6465 6c20 7c20 4d75  ogTauHModel | Mu
+00028b50: 6c74 694c 6f67 5461 7548 4d6f 6465 6c0a  ltiLogTauHModel.
+00028b60: 2020 2020 2020 2020 4d6f 6465 6c20 7768          Model wh
+00028b70: 6963 6820 6861 7320 6265 656e 2066 6974  ich has been fit
+00028b80: 7465 6420 746f 2064 6174 6173 6574 0a20  ted to dataset. 
+00028b90: 2020 2066 696c 655f 6e61 6d65 3a20 7374     file_name: st
+00028ba0: 720a 2020 2020 2020 2020 4e61 6d65 206f  r.        Name o
+00028bb0: 6620 6f75 7470 7574 2066 696c 650a 2020  f output file.  
+00028bc0: 2020 7665 7262 6f73 653a 2062 6f6f 6c2c    verbose: bool,
+00028bd0: 2064 6566 6175 6c74 2054 7275 650a 2020   default True.  
+00028be0: 2020 2020 2020 4966 2054 7275 652c 206f        If True, o
+00028bf0: 7574 7075 7420 6669 6c65 206c 6f63 6174  utput file locat
+00028c00: 696f 6e20 6973 2077 7269 7474 656e 2074  ion is written t
+00028c10: 6f20 7465 726d 696e 616c 0a0a 2020 2020  o terminal..    
+00028c20: 5265 7475 726e 730a 2020 2020 2d2d 2d2d  Returns.    ----
+00028c30: 2d2d 2d0a 2020 2020 4e6f 6e65 0a20 2020  ---.    None.   
+00028c40: 2027 2727 0a0a 2020 2020 6966 206e 6f74   '''..    if not
+00028c50: 206d 6f64 656c 2e66 6974 5f73 7461 7475   model.fit_statu
+00028c60: 733a 0a20 2020 2020 2020 2072 6574 7572  s:.        retur
+00028c70: 6e0a 0a20 2020 2069 6620 6973 696e 7374  n..    if isinst
+00028c80: 616e 6365 2864 6174 6173 6574 2c20 5461  ance(dataset, Ta
+00028c90: 7548 4461 7461 7365 7429 3a0a 2020 2020  uHDataset):.    
+00028ca0: 2020 2020 785f 7661 6c73 203d 2064 6174      x_vals = dat
+00028cb0: 6173 6574 2e66 6965 6c64 730a 2020 2020  aset.fields.    
+00028cc0: 2020 2020 785f 7661 725f 6c61 6265 6c20      x_var_label 
+00028cd0: 3d20 2748 2028 4f65 2927 0a0a 2020 2020  = 'H (Oe)'..    
+00028ce0: 656c 6966 2069 7369 6e73 7461 6e63 6528  elif isinstance(
+00028cf0: 6461 7461 7365 742c 2054 6175 5444 6174  dataset, TauTDat
+00028d00: 6173 6574 293a 0a20 2020 2020 2020 2078  aset):.        x
+00028d10: 5f76 616c 7320 3d20 6461 7461 7365 742e  _vals = dataset.
+00028d20: 7465 6d70 6572 6174 7572 6573 0a20 2020  temperatures.   
+00028d30: 2020 2020 2078 5f76 6172 5f6c 6162 656c       x_var_label
+00028d40: 203d 2027 5420 284b 2927 0a0a 2020 2020   = 'T (K)'..    
+00028d50: 6966 2074 7970 6528 6d6f 6465 6c29 2069  if type(model) i
+00028d60: 6e20 5b4d 756c 7469 4c6f 6754 6175 544d  n [MultiLogTauTM
+00028d70: 6f64 656c 2c20 4d75 6c74 694c 6f67 5461  odel, MultiLogTa
+00028d80: 7548 4d6f 6465 6c5d 3a0a 2020 2020 2020  uHModel]:.      
+00028d90: 2020 6c6f 676d 6f64 656c 7320 3d20 6d6f    logmodels = mo
+00028da0: 6465 6c2e 6c6f 676d 6f64 656c 730a 2020  del.logmodels.  
+00028db0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00028dc0: 6c6f 676d 6f64 656c 7320 3d20 5b6d 6f64  logmodels = [mod
+00028dd0: 656c 5d0a 0a20 2020 2066 203d 206f 7065  el]..    f = ope
+00028de0: 6e28 6669 6c65 5f6e 616d 652c 2027 7727  n(file_name, 'w'
+00028df0: 2c20 656e 636f 6469 6e67 3d27 7574 662d  , encoding='utf-
+00028e00: 3827 290a 0a20 2020 2078 5f76 6172 735f  8')..    x_vars_
+00028e10: 6772 6964 203d 206e 702e 6c69 6e73 7061  grid = np.linspa
+00028e20: 6365 280a 2020 2020 2020 2020 6e70 2e6d  ce(.        np.m
+00028e30: 696e 2878 5f76 616c 7329 2c0a 2020 2020  in(x_vals),.    
+00028e40: 2020 2020 6e70 2e6d 6178 2878 5f76 616c      np.max(x_val
+00028e50: 7329 2c0a 2020 2020 2020 2020 3130 3030  s),.        1000
+00028e60: 0a20 2020 2029 0a0a 2020 2020 662e 7772  .    )..    f.wr
+00028e70: 6974 6528 277b 3a3e 397d 2027 2e66 6f72  ite('{:>9} '.for
+00028e80: 6d61 7428 785f 7661 725f 6c61 6265 6c29  mat(x_var_label)
+00028e90: 290a 2020 2020 666f 7220 6c6f 676d 6f64  ).    for logmod
+00028ea0: 656c 2069 6e20 6c6f 676d 6f64 656c 733a  el in logmodels:
+00028eb0: 0a20 2020 2020 2020 2066 2e77 7269 7465  .        f.write
+00028ec0: 2827 7b3a 3e37 7d20 7261 7465 2027 2e66  ('{:>7} rate '.f
+00028ed0: 6f72 6d61 7428 6c6f 676d 6f64 656c 2e4e  ormat(logmodel.N
+00028ee0: 414d 4529 290a 2020 2020 6966 206c 656e  AME)).    if len
+00028ef0: 286c 6f67 6d6f 6465 6c73 2920 3e20 313a  (logmodels) > 1:
+00028f00: 0a20 2020 2020 2020 2066 2e77 7269 7465  .        f.write
+00028f10: 2827 2020 546f 7461 6c20 7261 7465 2028  ('  Total rate (
+00028f20: 735e 2d31 2927 290a 2020 2020 662e 7772  s^-1)').    f.wr
+00028f30: 6974 6528 275c 6e27 290a 0a20 2020 2066  ite('\n')..    f
+00028f40: 6f72 2067 7269 645f 7074 2069 6e20 785f  or grid_pt in x_
+00028f50: 7661 7273 5f67 7269 643a 0a20 2020 2020  vars_grid:.     
+00028f60: 2020 2066 2e77 7269 7465 2827 7b3a 2039     f.write('{: 9
+00028f70: 2e35 667d 2027 2e66 6f72 6d61 7428 6772  .5f} '.format(gr
+00028f80: 6964 5f70 7429 290a 2020 2020 2020 2020  id_pt)).        
+00028f90: 746f 7461 6c20 3d20 302e 0a20 2020 2020  total = 0..     
+00028fa0: 2020 2066 6f72 206c 6f67 6d6f 6465 6c20     for logmodel 
+00028fb0: 696e 206c 6f67 6d6f 6465 6c73 3a0a 2020  in logmodels:.  
+00028fc0: 2020 2020 2020 2020 2020 7261 7465 203d            rate =
+00028fd0: 2031 302a 2a6c 6f67 6d6f 6465 6c2e 6d6f   10**logmodel.mo
+00028fe0: 6465 6c28 0a20 2020 2020 2020 2020 2020  del(.           
+00028ff0: 2020 2020 206c 6f67 6d6f 6465 6c2e 6669       logmodel.fi
+00029000: 6e61 6c5f 7661 725f 7661 6c75 6573 2c0a  nal_var_values,.
+00029010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029020: 5b67 7269 645f 7074 5d0a 2020 2020 2020  [grid_pt].      
+00029030: 2020 2020 2020 295b 305d 0a20 2020 2020        )[0].     
+00029040: 2020 2020 2020 2066 2e77 7269 7465 2827         f.write('
+00029050: 7b3a 2e36 457d 2027 2e66 6f72 6d61 7428  {:.6E} '.format(
+00029060: 7261 7465 2929 0a20 2020 2020 2020 2020  rate)).         
+00029070: 2020 2074 6f74 616c 202b 3d20 7261 7465     total += rate
+00029080: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
+00029090: 6c6f 676d 6f64 656c 7329 203e 2031 3a0a  logmodels) > 1:.
+000290a0: 2020 2020 2020 2020 2020 2020 662e 7772              f.wr
+000290b0: 6974 6528 277b 3a2e 3645 7d27 2e66 6f72  ite('{:.6E}'.for
+000290c0: 6d61 7428 746f 7461 6c29 290a 2020 2020  mat(total)).    
+000290d0: 2020 2020 662e 7772 6974 6528 275c 6e27      f.write('\n'
+000290e0: 290a 0a20 2020 2069 6620 7665 7262 6f73  )..    if verbos
+000290f0: 653a 0a20 2020 2020 2020 2075 742e 6370  e:.        ut.cp
+00029100: 7269 6e74 280a 2020 2020 2020 2020 2020  rint(.          
+00029110: 2020 275c 6e20 5265 6c61 7861 7469 6f6e    '\n Relaxation
+00029120: 206d 6f64 656c 20cf 84e2 81bb c2b9 2076   model ....... v
+00029130: 7320 7b7d 2077 7269 7474 656e 2074 6f20  s {} written to 
+00029140: 5c6e 207b 7d5c 6e27 2e66 6f72 6d61 7428  \n {}\n'.format(
+00029150: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00029160: 2078 5f76 6172 5f6c 6162 656c 5b30 5d2c   x_var_label[0],
+00029170: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00029180: 2066 696c 655f 6e61 6d65 0a20 2020 2020   file_name.     
+00029190: 2020 2020 2020 2029 2c0a 2020 2020 2020         ),.      
+000291a0: 2020 2020 2020 2763 7961 6e27 0a20 2020        'cyan'.   
+000291b0: 2020 2020 2029 0a0a 2020 2020 7265 7475       )..    retu
+000291c0: 726e 0a                                  rn.
```

### Comparing `ccfit2-5.0.1/ccfit2/stats.py` & `ccfit2-5.0.2/ccfit2/stats.py`

 * *Files identical despite different names*

### Comparing `ccfit2-5.0.1/ccfit2/utils.py` & `ccfit2-5.0.2/ccfit2/utils.py`

 * *Files identical despite different names*

### Comparing `ccfit2-5.0.1/ccfit2/waveform.py` & `ccfit2-5.0.2/ccfit2/waveform.py`

 * *Files identical despite different names*

### Comparing `ccfit2-5.0.1/ccfit2.egg-info/PKG-INFO` & `ccfit2-5.0.2/ccfit2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccfit2
-Version: 5.0.1
+Version: 5.0.2
 Summary: CCFIT2 is a program for fitting AC and DC magnetisation data
 Home-page: https://gitlab.com/chilton-group/cc-fit2
 Author: Daniel Reta
 Author-email: danielreta1@gmail.com
 Project-URL: Bug Tracker, https://gitlab.com/chilton-group/cc-fit2/-/issues
 Project-URL: Documentation, https://chilton-group.gitlab.io/cc-fit2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ccfit2-5.0.1/setup.py` & `ccfit2-5.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import setuptools
 
 with open('README.md', 'r') as file:
     long_description = file.read()
 
 # DO NOT EDIT THIS NUMBER!
 # IT IS AUTOMATICALLY CHANGED BY python-semantic-release
-__version__ = "5.0.1"
+__version__ = "5.0.2"
 
 setuptools.setup(
     name='ccfit2',
     version=__version__,
     author='Daniel Reta',
     author_email='danielreta1@gmail.com',
     description='CCFIT2 is a program for fitting AC and DC magnetisation data', # noqa
```

