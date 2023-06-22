# Comparing `tmp/erdetect-2.2.0.tar.gz` & `tmp/erdetect-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erdetect-2.2.0.tar", last modified: Thu Jun 15 17:56:01 2023, max compression
+gzip compressed data, was "erdetect-2.3.0.tar", last modified: Thu Jun 22 08:17:58 2023, max compression
```

## Comparing `erdetect-2.2.0.tar` & `erdetect-2.3.0.tar`

### file list

```diff
@@ -1,33 +1,37 @@
-drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-06-15 17:56:01.552957 erdetect-2.2.0/
--rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    35823 2022-01-28 21:02:26.000000 erdetect-2.2.0/LICENSE
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     4846 2023-06-15 17:56:01.553121 erdetect-2.2.0/PKG-INFO
--rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     3844 2023-06-15 17:54:10.000000 erdetect-2.2.0/README.md
-drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-06-15 17:56:01.473294 erdetect-2.2.0/erdetect/
--rwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)      645 2023-04-11 21:39:35.000000 erdetect-2.2.0/erdetect/__init__.py
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     1318 2022-09-14 18:21:38.000000 erdetect-2.2.0/erdetect/__main__.py
--rwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    46689 2023-06-15 17:43:57.000000 erdetect-2.2.0/erdetect/_erdetect.py
-drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-06-15 17:56:01.521631 erdetect-2.2.0/erdetect/core/
--rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)       45 2023-04-11 17:08:10.000000 erdetect-2.2.0/erdetect/core/__init__.py
--rwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    44920 2023-06-14 22:16:11.000000 erdetect-2.2.0/erdetect/core/config.py
--rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    13275 2022-09-13 16:33:39.000000 erdetect-2.2.0/erdetect/core/detection.py
-drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-06-15 17:56:01.533029 erdetect-2.2.0/erdetect/core/metrics/
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     3088 2022-09-13 23:06:23.000000 erdetect-2.2.0/erdetect/core/metrics/metric_cross_proj.py
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     3876 2023-04-22 23:02:05.000000 erdetect-2.2.0/erdetect/core/metrics/metric_waveform.py
--rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     8720 2022-09-13 16:33:39.000000 erdetect-2.2.0/erdetect/core/peak_finder.py
--rwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    30091 2023-06-15 17:12:32.000000 erdetect-2.2.0/erdetect/main_cli.py
-drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-06-15 17:56:01.536848 erdetect-2.2.0/erdetect/utils/
--rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)       45 2023-04-11 17:08:10.000000 erdetect-2.2.0/erdetect/utils/__init__.py
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     4002 2023-04-11 17:56:08.000000 erdetect-2.2.0/erdetect/utils/misc.py
--rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)       22 2023-06-15 17:36:43.000000 erdetect-2.2.0/erdetect/version.py
-drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-06-15 17:56:01.552275 erdetect-2.2.0/erdetect/views/
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)       45 2023-04-11 17:08:17.000000 erdetect-2.2.0/erdetect/views/__init__.py
--rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    34975 2023-06-15 17:44:19.000000 erdetect-2.2.0/erdetect/views/gui.py
--rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     7934 2022-09-13 16:33:39.000000 erdetect-2.2.0/erdetect/views/output_images.py
-drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-06-15 17:56:01.486917 erdetect-2.2.0/erdetect.egg-info/
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     4846 2023-06-15 17:56:01.000000 erdetect-2.2.0/erdetect.egg-info/PKG-INFO
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)      627 2023-06-15 17:56:01.000000 erdetect-2.2.0/erdetect.egg-info/SOURCES.txt
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        1 2023-06-15 17:56:01.000000 erdetect-2.2.0/erdetect.egg-info/dependency_links.txt
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)       83 2023-06-15 17:56:01.000000 erdetect-2.2.0/erdetect.egg-info/requires.txt
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        9 2023-06-15 17:56:01.000000 erdetect-2.2.0/erdetect.egg-info/top_level.txt
--rwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     1411 2023-06-15 17:54:39.000000 erdetect-2.2.0/pyproject.toml
--rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)      192 2023-06-15 17:56:01.555985 erdetect-2.2.0/setup.cfg
+drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-06-22 08:17:58.095685 erdetect-2.3.0/
+-rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    35823 2022-01-28 21:02:26.000000 erdetect-2.3.0/LICENSE
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     4846 2023-06-22 08:17:58.095920 erdetect-2.3.0/PKG-INFO
+-rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     3844 2023-06-22 07:53:57.000000 erdetect-2.3.0/README.md
+drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-06-22 08:17:57.981462 erdetect-2.3.0/erdetect/
+-rwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)      645 2023-04-11 21:39:35.000000 erdetect-2.3.0/erdetect/__init__.py
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     1318 2022-09-14 18:21:38.000000 erdetect-2.3.0/erdetect/__main__.py
+-rwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    53286 2023-06-22 07:53:34.000000 erdetect-2.3.0/erdetect/_erdetect.py
+drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-06-22 08:17:58.022090 erdetect-2.3.0/erdetect/core/
+-rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)       45 2023-04-11 17:08:10.000000 erdetect-2.3.0/erdetect/core/__init__.py
+-rwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    44922 2023-06-22 07:50:20.000000 erdetect-2.3.0/erdetect/core/config.py
+-rwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    13277 2023-06-22 07:50:36.000000 erdetect-2.3.0/erdetect/core/detection.py
+drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-06-22 08:17:58.039183 erdetect-2.3.0/erdetect/core/metrics/
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     3088 2022-09-13 23:06:23.000000 erdetect-2.3.0/erdetect/core/metrics/metric_cross_proj.py
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     3876 2023-04-22 23:02:05.000000 erdetect-2.3.0/erdetect/core/metrics/metric_waveform.py
+-rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     8720 2022-09-13 16:33:39.000000 erdetect-2.3.0/erdetect/core/peak_finder.py
+-rwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    24010 2023-06-22 08:15:14.000000 erdetect-2.3.0/erdetect/main_cli.py
+drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-06-22 08:17:58.047133 erdetect-2.3.0/erdetect/utils/
+-rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)       45 2023-04-11 17:08:10.000000 erdetect-2.3.0/erdetect/utils/__init__.py
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     4002 2023-04-11 17:56:08.000000 erdetect-2.3.0/erdetect/utils/misc.py
+-rwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)       22 2023-06-22 08:15:23.000000 erdetect-2.3.0/erdetect/version.py
+drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-06-22 08:17:58.075827 erdetect-2.3.0/erdetect/views/
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)       45 2023-04-11 17:08:17.000000 erdetect-2.3.0/erdetect/views/__init__.py
+-rwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    94544 2023-06-22 08:15:33.000000 erdetect-2.3.0/erdetect/views/gui.py
+-rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     7934 2022-09-13 16:33:39.000000 erdetect-2.3.0/erdetect/views/output_images.py
+drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-06-22 08:17:57.994027 erdetect-2.3.0/erdetect.egg-info/
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     4846 2023-06-22 08:17:57.000000 erdetect-2.3.0/erdetect.egg-info/PKG-INFO
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)      688 2023-06-22 08:17:57.000000 erdetect-2.3.0/erdetect.egg-info/SOURCES.txt
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        1 2023-06-22 08:17:57.000000 erdetect-2.3.0/erdetect.egg-info/dependency_links.txt
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)       83 2023-06-22 08:17:57.000000 erdetect-2.3.0/erdetect.egg-info/requires.txt
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        9 2023-06-22 08:17:57.000000 erdetect-2.3.0/erdetect.egg-info/top_level.txt
+-rwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     1411 2023-06-22 07:53:54.000000 erdetect-2.3.0/pyproject.toml
+-rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)      192 2023-06-22 08:17:58.102238 erdetect-2.3.0/setup.cfg
+drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-06-22 08:17:58.094866 erdetect-2.3.0/tests/
+-rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)      968 2023-04-11 21:42:57.000000 erdetect-2.3.0/tests/test_fileio.py
+-rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)       43 2023-04-11 21:43:02.000000 erdetect-2.3.0/tests/test_gui.py
+-rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)      211 2023-04-11 21:42:59.000000 erdetect-2.3.0/tests/test_process.py
```

### Comparing `erdetect-2.2.0/LICENSE` & `erdetect-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `erdetect-2.2.0/PKG-INFO` & `erdetect-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erdetect
-Version: 2.2.0
+Version: 2.3.0
 Summary: A package for the automatic detection of evoked responses in SPES/CCEP data
 Author-email: Max van den Boom <m.a.vandenboom84@gmail.com>
 License: GPLv3
 Project-URL: homepage, https://github.com/MultimodalNeuroimagingLab/ERDetect
 Project-URL: documentation, https://github.com/MultimodalNeuroimagingLab/ERDetect
 Project-URL: repository, https://github.com/MultimodalNeuroimagingLab/ERDetect
 Keywords: evoked response,detection,ieeg,n1,SPES,CCEP
```

### Comparing `erdetect-2.2.0/README.md` & `erdetect-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `erdetect-2.2.0/erdetect/__init__.py` & `erdetect-2.3.0/erdetect/__init__.py`

 * *Files identical despite different names*

### Comparing `erdetect-2.2.0/erdetect/__main__.py` & `erdetect-2.3.0/erdetect/__main__.py`

 * *Files identical despite different names*

### Comparing `erdetect-2.2.0/erdetect/_erdetect.py` & `erdetect-2.3.0/erdetect/_erdetect.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Evoked response detection - Processing functions
 =====================================================
 
 
-Copyright 2022, Max van den Boom (Multimodal Neuroimaging Lab, Mayo Clinic, Rochester MN)
+Copyright 2023, Max van den Boom (Multimodal Neuroimaging Lab, Mayo Clinic, Rochester MN)
 
 This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License
 as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied
 warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
 You should have received a copy of the GNU General Public License along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
@@ -103,15 +103,15 @@
             logging.error('Could not load the IEEG JSON sidecar (\'' + bids_subset_root + '_ieeg.json\') that is required to perform line-noise removal, exiting...')
             raise RuntimeError('Could not load the IEEG JSON sidecar')
 
     else:
         # not from JSON
 
         # check if there is a number in the config, if so, use it
-        if not str(cfg('preprocess', 'line_noise_removal')).lower() == 'off':
+        if not cfg('preprocess', 'line_noise_removal').lower() == 'off':
             line_noise_removal = float(cfg('preprocess', 'line_noise_removal'))
 
 
     #
     # retrieve channel metadata
     #
 
@@ -828,7 +828,72 @@
 
     # on success, return output
     return output_dict
 
 
 def log_indented_line(caption, text):
     logging.info(caption.ljust(LOGGING_CAPTION_INDENT_LENGTH, ' ') + text)
+
+
+def print_config(preproc_prioritize_speed):
+    '''
+    Print configuration information
+    '''
+
+    log_indented_line('Preprocessing priority:', ('Speed' if preproc_prioritize_speed else 'Memory'))
+    log_indented_line('High-pass filtering:', ('Yes' if cfg('preprocess', 'high_pass') else 'No'))
+    log_indented_line('Early re-referencing:', ('Yes' if cfg('preprocess', 'early_re_referencing', 'enabled') else 'No'))
+    if cfg('preprocess', 'early_re_referencing', 'enabled'):
+        log_indented_line('    Method:', str(cfg('preprocess', 'early_re_referencing', 'method')))
+        log_indented_line('    Stim exclude epoch:', str(cfg('preprocess', 'early_re_referencing', 'stim_excl_epoch')[0]) + 's : ' + str(cfg('preprocess', 'early_re_referencing', 'stim_excl_epoch')[1]) + 's')
+        logging.info(multi_line_list(cfg('preprocess', 'early_re_referencing', 'channel_types'), LOGGING_CAPTION_INDENT_LENGTH, '    Included channels types:', 14, ' '))
+    log_indented_line('Line-noise removal:', cfg('preprocess', 'line_noise_removal') + (' Hz' if is_number(cfg('preprocess', 'line_noise_removal')) else ''))
+    log_indented_line('Late re-referencing:', ('Yes' if cfg('preprocess', 'late_re_referencing', 'enabled') else 'No'))
+    if cfg('preprocess', 'late_re_referencing', 'enabled'):
+        log_indented_line('    Method:', str(cfg('preprocess', 'late_re_referencing', 'method')))
+        if cfg('preprocess', 'late_re_referencing', 'method') in ('CAR', 'CAR_headbox'):
+            log_indented_line('    CAR by variance:', ('Off' if cfg('preprocess', 'late_re_referencing', 'CAR_by_variance') == -1 else 'Channels with lowest (' + str(cfg('preprocess', 'late_re_referencing', 'CAR_by_variance')) + ' quantile) trial variance'))
+        log_indented_line('    Stim exclude epoch:', str(cfg('preprocess', 'late_re_referencing', 'stim_excl_epoch')[0]) + 's : ' + str(cfg('preprocess', 'late_re_referencing', 'stim_excl_epoch')[1]) + 's')
+        logging.info(multi_line_list(cfg('preprocess', 'late_re_referencing', 'channel_types'), LOGGING_CAPTION_INDENT_LENGTH, '    Included channels types:', 14, ' '))
+    logging.info('')
+    log_indented_line('Trial epoch window:', str(cfg('trials', 'trial_epoch')[0]) + 's < stim onset < ' + str(cfg('trials', 'trial_epoch')[1]) + 's  (window size ' + str(abs(cfg('trials', 'trial_epoch')[1] - cfg('trials', 'trial_epoch')[0])) + 's)')
+    log_indented_line('Trial out-of-bounds handling:', str(cfg('trials', 'out_of_bounds_handling')))
+    log_indented_line('Trial baseline window:', str(cfg('trials', 'baseline_epoch')[0]) + 's : ' + str(cfg('trials', 'baseline_epoch')[1]) + 's')
+    log_indented_line('Trial baseline normalization:', str(cfg('trials', 'baseline_norm')))
+    log_indented_line('Concatenate bidirectional stimulated pairs:', ('Yes' if cfg('trials', 'concat_bidirectional_pairs') else 'No'))
+    log_indented_line('Minimum # of required stimulus-pair trials:', str(cfg('trials', 'minimum_stimpair_trials')))
+    logging.info(multi_line_list(cfg('channels', 'measured_types'), LOGGING_CAPTION_INDENT_LENGTH, 'Include channel types as measured:', 14, ' '))
+    logging.info(multi_line_list(cfg('channels', 'stim_types'), LOGGING_CAPTION_INDENT_LENGTH, 'Include channel types for stimulation:', 14, ' '))
+    logging.info('')
+    log_indented_line('Cross-projection metric:', ('Enabled' if cfg('metrics', 'cross_proj', 'enabled') else 'Disabled'))
+    if cfg('metrics', 'cross_proj', 'enabled'):
+        log_indented_line('    Cross-projection epoch:', str(cfg('metrics', 'cross_proj', 'epoch')[0]) + 's : ' + str(cfg('metrics', 'cross_proj', 'epoch')[1]) + 's')
+    log_indented_line('Waveform metric:', ('Enabled' if cfg('metrics', 'waveform', 'enabled') else 'Disabled'))
+    if cfg('metrics', 'waveform', 'enabled'):
+        log_indented_line('    Waveform epoch:', str(cfg('metrics', 'waveform', 'epoch')[0]) + 's : ' + str(cfg('metrics', 'waveform', 'epoch')[1]) + 's')
+        log_indented_line('    Waveform bandpass:', str(cfg('metrics', 'waveform', 'bandpass')[0]) + 'Hz - ' + str(cfg('metrics', 'waveform', 'bandpass')[1]) + 'Hz')
+    logging.info('')
+    logging.info('Detection')
+    log_indented_line('    Negative responses:', ('Yes' if cfg('detection', 'negative') else 'No'))
+    log_indented_line('    Positive responses:', ('Yes' if cfg('detection', 'positive') else 'No'))
+    log_indented_line('    Peak search window:', str(cfg('detection', 'peak_search_epoch')[0]) + 's : ' + str(cfg('detection', 'peak_search_epoch')[1]) + 's')
+    log_indented_line('    Evoked response search window:', str(cfg('detection', 'response_search_epoch')[0]) + 's : ' + str(cfg('detection', 'response_search_epoch')[1]) + 's')
+    log_indented_line('    Evoked response detection method:', str(cfg('detection', 'method')))
+    if cfg('detection', 'method') == 'std_base':
+        log_indented_line('        Std baseline window:', str(cfg('detection', 'std_base', 'baseline_epoch')[0]) + 's : ' + str(cfg('detection', 'std_base', 'baseline_epoch')[1]) + 's')
+        log_indented_line('        Std baseline threshold factor:', str(cfg('detection', 'std_base', 'baseline_threshold_factor')))
+    elif cfg('detection', 'method') == 'cross_proj':
+        log_indented_line('        Cross-projection detection threshold:', str(cfg('detection', 'cross_proj', 'threshold')))
+    elif cfg('detection', 'method') == 'waveform':
+        log_indented_line('        Waveform detection threshold:', str(cfg('detection', 'waveform', 'threshold')))
+    logging.info('')
+    logging.info('Visualization')
+    log_indented_line('    Negative responses:', ('Yes' if cfg('visualization', 'negative') else 'No'))
+    log_indented_line('    Positive responses:', ('Yes' if cfg('visualization', 'positive') else 'No'))
+    log_indented_line('    X-axis epoch:', str(cfg('visualization', 'x_axis_epoch')[0]) + 's : ' + str(cfg('visualization', 'x_axis_epoch')[1]) + 's')
+    log_indented_line('    Blank stimulation epoch:', str(cfg('visualization', 'blank_stim_epoch')[0]) + 's : ' + str(cfg('visualization', 'blank_stim_epoch')[1]) + 's')
+    log_indented_line('    Generate electrode images:', ('Yes' if cfg('visualization', 'generate_electrode_images') else 'No'))
+    log_indented_line('    Generate stimulation-pair images:', ('Yes' if cfg('visualization', 'generate_stimpair_images') else 'No'))
+    log_indented_line('    Generate matrix images:', ('Yes' if cfg('visualization', 'generate_matrix_images') else 'No'))
+    logging.info('')
+    logging.info('')
+    logging.info('')
```

### Comparing `erdetect-2.2.0/erdetect/core/config.py` & `erdetect-2.3.0/erdetect/core/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     config['detection']['std_base'] = dict()
     config['detection']['std_base']['baseline_epoch']               = CONFIG_DETECTION_STD_BASE_BASELINE_EPOCH_DEFAULT
     config['detection']['std_base']['baseline_threshold_factor']    = CONFIG_DETECTION_STD_BASE_BASELINE_THRESHOLD_FACTOR
 
     config['visualization'] = dict()
     config['visualization']['negative']                             = True                      # whether to output negative responses
     config['visualization']['positive']                             = False                     # whether to output positive responses
-    config['visualization']['x_axis_epoch']                         = (-0.2, 1)                 # the range for the x-axis in display, (in seconds) relative to the stimulus onset that will be used as the range
+    config['visualization']['x_axis_epoch']                         = (-0.2, 1.0)                 # the range for the x-axis in display, (in seconds) relative to the stimulus onset that will be used as the range
     config['visualization']['blank_stim_epoch']                     = (-0.015, 0.0025)          # the range
     config['visualization']['generate_electrode_images']            = True
     config['visualization']['generate_stimpair_images']             = True
     config['visualization']['generate_matrix_images']               = True
 
     # return a default configuration
     return config
```

### Comparing `erdetect-2.2.0/erdetect/core/detection.py` & `erdetect-2.3.0/erdetect/core/detection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Module that contains the function(s) to detect evoked response peaks
 
 
-Copyright 2022, Max van den Boom (Multimodal Neuroimaging Lab, Mayo Clinic, Rochester MN)
+Copyright 2023, Max van den Boom (Multimodal Neuroimaging Lab, Mayo Clinic, Rochester MN)
 
 Baseline standard deviation based detection method is adapted from:
     Original author: Dorien van Blooijs (2018)
     Adjusted by: Jaap van der Aar, Dora Hermes, Dorien van Blooijs, Giulio Castegnaro; (UMC Utrecht, 2019)
 
 This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License
 as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
@@ -56,15 +56,14 @@
     # (tuple) The time-span in which an evoked response will be searched, expressed as a tuple with the start- and end-point in seconds
     # relative to stimulation onset (e.g. the standard tuple of '0.02, 0.09' will have the algorithm start the search
     # for an app at 20ms after stimulation onset up to 90ms after stimulation onset)
     er_search_epoch = config('detection', 'response_search_epoch')
 
     #
     method = config('detection', 'method')
-
     if method == 'std_base':
 
         # (tuple) The time-span on which the baseline is calculated, expressed as a tuple with the start- and end-point in
         # seconds relative to stimulation onset (e.g. the standard tuple of '-1, -.1' will use the period from 1s before
         # stimulation onset to 100ms before stimulation onset to calculate the baseline on)
         baseline_epoch = config('detection', 'std_base', 'baseline_epoch')
 
@@ -128,18 +127,18 @@
             raise ValueError('No waveform-metrics were passed')
         elif not waveform_metrics.shape == er_peak_indices.shape:
             logging.error('Size of the waveform-metrics matrix does not match the size of the output buffer (the number of electrodes and stim-pairs do not match)')
             raise ValueError('Waveform-metrics and output buffer size mismatch')
 
     elif method == 'cross_proj':
 
-        if waveform_metrics is None:
+        if cross_proj_metrics is None:
             logging.error('Method is set to \'cross_proj\' but no cross-projection metrics were passed to the detection function')
             raise ValueError('No cross-projection were passed')
-        elif not waveform_metrics.shape == er_peak_indices.shape:
+        elif not cross_proj_metrics.shape == er_peak_indices.shape:
             logging.error('Size of the cross-projection metrics matrix does not match the size of the output buffer (the number of electrodes and stim-pairs do not match)')
             raise ValueError('Cross-projection and output buffer size mismatch')
 
     # for every electrode
     for iElec in range(data.shape[0]):
 
         # for every stimulation-pair
```

### Comparing `erdetect-2.2.0/erdetect/core/metrics/metric_cross_proj.py` & `erdetect-2.3.0/erdetect/core/metrics/metric_cross_proj.py`

 * *Files identical despite different names*

### Comparing `erdetect-2.2.0/erdetect/core/metrics/metric_waveform.py` & `erdetect-2.3.0/erdetect/core/metrics/metric_waveform.py`

 * *Files identical despite different names*

### Comparing `erdetect-2.2.0/erdetect/core/peak_finder.py` & `erdetect-2.3.0/erdetect/core/peak_finder.py`

 * *Files identical despite different names*

### Comparing `erdetect-2.2.0/erdetect/main_cli.py` & `erdetect-2.3.0/erdetect/main_cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     LOGGING_CAPTION_INDENT_LENGTH, CONFIG_DETECTION_STD_BASE_BASELINE_EPOCH_DEFAULT, \
     CONFIG_DETECTION_STD_BASE_BASELINE_THRESHOLD_FACTOR, CONFIG_DETECTION_CROSS_PROJ_THRESHOLD, CONFIG_DETECTION_WAVEFORM_PROJ_THRESHOLD
 from erdetect._erdetect import process_subset
 from ieegprep import VALID_FORMAT_EXTENSIONS
 from ieegprep.bids.data_structure import list_bids_datasets
 from ieegprep.utils.console import multi_line_list
 from ieegprep.utils.misc import is_number
-from erdetect._erdetect import log_indented_line
+from erdetect._erdetect import log_indented_line, print_config
 from erdetect.views.gui import open_gui
 
 
 def execute():
 
     #
     # define and parse the input arguments
@@ -125,15 +125,17 @@
                              '                       The headbox number should be indicated for each channel in '
                              '                       the _channels.tsv file in a column with the heading \'headbox\'.\n'
                              'Note: If a configuration file is provided, then this command-line argument will overrule the\n'
                              '      late re-referencing setting in the configuration file\n\n',
                         nargs=1)
     parser.add_argument('--late_reref_CAR_by_variance',
                         help='Perform late re-referencing by calculating a common average for each stim-pair condition\n'
-                             '(per group) over only the channels with the lowest trial signal variance.\n\n',
+                             '(per group) over only the channels with the lowest trial signal variance.\n'
+                             'Note: If a configuration file is provided, then this command-line argument will overrule the\n'
+                             '      late re-referencing by variance setting in the configuration file\n\n',
                         nargs='?', const='0.2')
     parser.add_argument('--include_positive_responses',
                         help='Detect and visualize positive evoked responses in addition to the negative responses\n\n',
                         action='store_true')
     parser.add_argument('--method',
                         help='The method that should be used to detect evoked responses. the options are:\n'
                              '      - std_base   = The standard deviation of a baseline-epoch is used as a threshold\n'
@@ -193,15 +195,15 @@
         preproc_prioritize_speed = True
 
     if args.high_pass:
         cfg_set(True, 'preprocess', 'high_pass')
 
     if args.line_noise_removal:
         if str(args.line_noise_removal).lower() == 'json' or str(args.line_noise_removal).lower() == 'sidecar':
-            cfg_set('json', 'preprocess', 'line_noise_removal')
+            cfg_set('JSON', 'preprocess', 'line_noise_removal')
         elif is_number(args.line_noise_removal):
             # TODO: valid number
             cfg_set(str(args.line_noise_removal), 'preprocess', 'line_noise_removal')
         else:
             logging.error('Invalid \'line_noise_removal\' argument \'' + args.line_noise_removal + '\', either set to \'json\' or \'sidecar\' to retrieve the line-noise frequency from the *_ieeg.json file, or provide the line-noise frequency as a number.')
             return 1
 
@@ -277,82 +279,30 @@
     if cfg('detection', 'method') == 'cross_proj' and not cfg('metrics', 'cross_proj', 'enabled'):
         logging.warning('Evoked response detection is set to use cross-projections but the cross-projection metric is disabled, the cross-projection metric will be enabled')
         cfg_set(True, 'metrics', 'cross_proj', 'enabled')
     if cfg('detection', 'method') == 'waveform' and not cfg('metrics', 'waveform', 'enabled'):
         logging.warning('Evoked response detection is set to use waveforms but the waveform metric is disabled, the waveform metric will be enabled')
         cfg_set(True, 'metrics', 'waveform', 'enabled')
 
-    # print configuration information
-    log_indented_line('Preprocessing priority:', ('Speed' if preproc_prioritize_speed else 'Memory'))
-    log_indented_line('High-pass filtering:', ('Yes' if cfg('preprocess', 'high_pass') else 'No'))
-    log_indented_line('Early re-referencing:', ('Yes' if cfg('preprocess', 'early_re_referencing', 'enabled') else 'No'))
-    if cfg('preprocess', 'early_re_referencing', 'enabled'):
-        log_indented_line('    Method:', str(cfg('preprocess', 'early_re_referencing', 'method')))
-        log_indented_line('    Stim exclude epoch:', str(cfg('preprocess', 'early_re_referencing', 'stim_excl_epoch')[0]) + 's : ' + str(cfg('preprocess', 'early_re_referencing', 'stim_excl_epoch')[1]) + 's')
-        logging.info(multi_line_list(cfg('preprocess', 'early_re_referencing', 'channel_types'), LOGGING_CAPTION_INDENT_LENGTH, '    Included channels types:', 14, ' '))
-    log_indented_line('Line-noise removal:', cfg('preprocess', 'line_noise_removal') + (' Hz' if is_number(cfg('preprocess', 'line_noise_removal')) else ''))
-    log_indented_line('Late re-referencing:', ('Yes' if cfg('preprocess', 'late_re_referencing', 'enabled') else 'No'))
-    if cfg('preprocess', 'late_re_referencing', 'enabled'):
-        log_indented_line('    Method:', str(cfg('preprocess', 'late_re_referencing', 'method')))
-        if cfg('preprocess', 'late_re_referencing', 'method') in ('CAR', 'CAR_headbox'):
-            log_indented_line('    CAR by variance:', ('Off' if cfg('preprocess', 'late_re_referencing', 'CAR_by_variance') == -1 else 'Channels with lowest (' + str(cfg('preprocess', 'late_re_referencing', 'CAR_by_variance')) + ' quantile) trial variance'))
-        log_indented_line('    Stim exclude epoch:', str(cfg('preprocess', 'late_re_referencing', 'stim_excl_epoch')[0]) + 's : ' + str(cfg('preprocess', 'late_re_referencing', 'stim_excl_epoch')[1]) + 's')
-        logging.info(multi_line_list(cfg('preprocess', 'late_re_referencing', 'channel_types'), LOGGING_CAPTION_INDENT_LENGTH, '    Included channels types:', 14, ' '))
-    logging.info('')
-    log_indented_line('Trial epoch window:', str(cfg('trials', 'trial_epoch')[0]) + 's < stim onset < ' + str(cfg('trials', 'trial_epoch')[1]) + 's  (window size ' + str(abs(cfg('trials', 'trial_epoch')[1] - cfg('trials', 'trial_epoch')[0])) + 's)')
-    log_indented_line('Trial out-of-bounds handling:', str(cfg('trials', 'out_of_bounds_handling')))
-    log_indented_line('Trial baseline window:', str(cfg('trials', 'baseline_epoch')[0]) + 's : ' + str(cfg('trials', 'baseline_epoch')[1]) + 's')
-    log_indented_line('Trial baseline normalization:', str(cfg('trials', 'baseline_norm')))
-    log_indented_line('Concatenate bidirectional stimulated pairs:', ('Yes' if cfg('trials', 'concat_bidirectional_pairs') else 'No'))
-    log_indented_line('Minimum # of required stimulus-pair trials:', str(cfg('trials', 'minimum_stimpair_trials')))
-    logging.info(multi_line_list(cfg('channels', 'measured_types'), LOGGING_CAPTION_INDENT_LENGTH, 'Include channel types as measured:', 14, ' '))
-    logging.info(multi_line_list(cfg('channels', 'stim_types'), LOGGING_CAPTION_INDENT_LENGTH, 'Include channel types for stimulation:', 14, ' '))
-    logging.info('')
-    log_indented_line('Cross-projection metric:', ('Enabled' if cfg('metrics', 'cross_proj', 'enabled') else 'Disabled'))
-    if cfg('metrics', 'cross_proj', 'enabled'):
-        log_indented_line('    Cross-projection epoch:', str(cfg('metrics', 'cross_proj', 'epoch')[0]) + 's : ' + str(cfg('metrics', 'cross_proj', 'epoch')[1]) + 's')
-    log_indented_line('Waveform metric:', ('Enabled' if cfg('metrics', 'waveform', 'enabled') else 'Disabled'))
-    if cfg('metrics', 'waveform', 'enabled'):
-        log_indented_line('    Waveform epoch:', str(cfg('metrics', 'waveform', 'epoch')[0]) + 's : ' + str(cfg('metrics', 'waveform', 'epoch')[1]) + 's')
-        log_indented_line('    Waveform bandpass:', str(cfg('metrics', 'waveform', 'bandpass')[0]) + 'Hz - ' + str(cfg('metrics', 'waveform', 'bandpass')[1]) + 'Hz')
-    logging.info('')
-    logging.info('Detection')
-    log_indented_line('    Negative responses:', ('Yes' if cfg('detection', 'negative') else 'No'))
-    log_indented_line('    Positive responses:', ('Yes' if cfg('detection', 'positive') else 'No'))
-    log_indented_line('    Peak search window:', str(cfg('detection', 'peak_search_epoch')[0]) + 's : ' + str(cfg('detection', 'peak_search_epoch')[1]) + 's')
-    log_indented_line('    Evoked response search window:', str(cfg('detection', 'response_search_epoch')[0]) + 's : ' + str(cfg('detection', 'response_search_epoch')[1]) + 's')
-    log_indented_line('    Evoked response detection method:', str(cfg('detection', 'method')))
-    if cfg('detection', 'method') == 'std_base':
-        log_indented_line('        Std baseline window:', str(cfg('detection', 'std_base', 'baseline_epoch')[0]) + 's : ' + str(cfg('detection', 'std_base', 'baseline_epoch')[1]) + 's')
-        log_indented_line('        Std baseline threshold factor:', str(cfg('detection', 'std_base', 'baseline_threshold_factor')))
-    elif cfg('detection', 'method') == 'cross_proj':
-        log_indented_line('        Cross-projection detection threshold:', str(cfg('detection', 'cross_proj', 'threshold')))
-    elif cfg('detection', 'method') == 'waveform':
-        log_indented_line('        Waveform detection threshold:', str(cfg('detection', 'waveform', 'threshold')))
-    logging.info('')
-    logging.info('Visualization')
-    log_indented_line('    Negative responses:', ('Yes' if cfg('visualization', 'negative') else 'No'))
-    log_indented_line('    Positive responses:', ('Yes' if cfg('visualization', 'positive') else 'No'))
-    log_indented_line('    X-axis epoch:', str(cfg('visualization', 'x_axis_epoch')[0]) + 's : ' + str(cfg('visualization', 'x_axis_epoch')[1]) + 's')
-    log_indented_line('    Blank stimulation epoch:', str(cfg('visualization', 'blank_stim_epoch')[0]) + 's : ' + str(cfg('visualization', 'blank_stim_epoch')[1]) + 's')
-    log_indented_line('    Generate electrode images:', ('Yes' if cfg('visualization', 'generate_electrode_images') else 'No'))
-    log_indented_line('    Generate stimulation-pair images:', ('Yes' if cfg('visualization', 'generate_stimpair_images') else 'No'))
-    log_indented_line('    Generate matrix images:', ('Yes' if cfg('visualization', 'generate_matrix_images') else 'No'))
-    logging.info('')
-    logging.info('')
-    logging.info('')
+
+    #
+    # open GUI or CLI processing
+    #
 
     if args.gui:
 
         # open and run on theGUI
-        open_gui()
-        # TODO: transfer CLI arguments to GUI
+        open_gui(init_input_directory=args.bids_dir, init_output_directory=args.output_dir)
 
     else:
 
+        # print configuration
+        print_config(preproc_prioritize_speed)
+
+
         #
         # Find and process participants and their datasets
         #
 
         args.bids_dir = os.path.abspath(os.path.expanduser(os.path.expandvars(args.bids_dir)))
         args.output_dir = os.path.abspath(os.path.expanduser(os.path.expandvars(args.output_dir)))
```

### Comparing `erdetect-2.2.0/erdetect/utils/misc.py` & `erdetect-2.3.0/erdetect/utils/misc.py`

 * *Files identical despite different names*

### Comparing `erdetect-2.2.0/erdetect/views/output_images.py` & `erdetect-2.3.0/erdetect/views/output_images.py`

 * *Files identical despite different names*

### Comparing `erdetect-2.2.0/erdetect.egg-info/PKG-INFO` & `erdetect-2.3.0/erdetect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erdetect
-Version: 2.2.0
+Version: 2.3.0
 Summary: A package for the automatic detection of evoked responses in SPES/CCEP data
 Author-email: Max van den Boom <m.a.vandenboom84@gmail.com>
 License: GPLv3
 Project-URL: homepage, https://github.com/MultimodalNeuroimagingLab/ERDetect
 Project-URL: documentation, https://github.com/MultimodalNeuroimagingLab/ERDetect
 Project-URL: repository, https://github.com/MultimodalNeuroimagingLab/ERDetect
 Keywords: evoked response,detection,ieeg,n1,SPES,CCEP
```

### Comparing `erdetect-2.2.0/erdetect.egg-info/SOURCES.txt` & `erdetect-2.3.0/erdetect.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -18,8 +18,11 @@
 erdetect/core/peak_finder.py
 erdetect/core/metrics/metric_cross_proj.py
 erdetect/core/metrics/metric_waveform.py
 erdetect/utils/__init__.py
 erdetect/utils/misc.py
 erdetect/views/__init__.py
 erdetect/views/gui.py
-erdetect/views/output_images.py
+erdetect/views/output_images.py
+tests/test_fileio.py
+tests/test_gui.py
+tests/test_process.py
```

### Comparing `erdetect-2.2.0/pyproject.toml` & `erdetect-2.3.0/pyproject.toml`

 * *Files identical despite different names*

