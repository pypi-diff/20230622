# Comparing `tmp/gw-mbank-0.2.0.tar.gz` & `tmp/gw-mbank-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gw-mbank-0.2.0.tar", last modified: Mon Mar  6 11:56:26 2023, max compression
+gzip compressed data, was "gw-mbank-0.3.1.tar", last modified: Thu Jun 22 15:17:28 2023, max compression
```

## Comparing `gw-mbank-0.2.0.tar` & `gw-mbank-0.3.1.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-03-06 11:56:26.518195 gw-mbank-0.2.0/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)    35149 2021-10-27 10:33:14.000000 gw-mbank-0.2.0/LICENSE.txt
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     6210 2023-03-06 11:56:26.518195 gw-mbank-0.2.0/PKG-INFO
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     5722 2023-01-30 16:28:41.000000 gw-mbank-0.2.0/README.md
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-03-06 11:56:26.514195 gw-mbank-0.2.0/bin/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)    13718 2023-02-21 17:23:43.000000 gw-mbank-0.2.0/bin/mbank_injections
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     6179 2023-02-15 17:15:34.000000 gw-mbank-0.2.0/bin/mbank_injections_workflow
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     5795 2023-02-21 15:50:09.000000 gw-mbank-0.2.0/bin/mbank_injfile
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     9181 2022-07-18 09:57:34.000000 gw-mbank-0.2.0/bin/mbank_mcmc
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     4819 2023-02-15 17:04:13.000000 gw-mbank-0.2.0/bin/mbank_merge
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     6770 2023-02-15 17:04:50.000000 gw-mbank-0.2.0/bin/mbank_place_templates
--rw-rw-r--   0 stefano   (1000) stefano   (1000)    11646 2023-03-05 15:41:33.000000 gw-mbank-0.2.0/bin/mbank_run
--rw-rw-r--   0 stefano   (1000) stefano   (1000)    13523 2023-02-15 17:04:28.000000 gw-mbank-0.2.0/bin/mbank_validate_metric
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-03-06 11:56:26.514195 gw-mbank-0.2.0/gw_mbank.egg-info/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     6210 2023-03-06 11:56:26.000000 gw-mbank-0.2.0/gw_mbank.egg-info/PKG-INFO
--rw-rw-r--   0 stefano   (1000) stefano   (1000)      503 2023-03-06 11:56:26.000000 gw-mbank-0.2.0/gw_mbank.egg-info/SOURCES.txt
--rw-rw-r--   0 stefano   (1000) stefano   (1000)        1 2023-03-06 11:56:26.000000 gw-mbank-0.2.0/gw_mbank.egg-info/dependency_links.txt
--rw-rw-r--   0 stefano   (1000) stefano   (1000)      107 2023-03-06 11:56:26.000000 gw-mbank-0.2.0/gw_mbank.egg-info/requires.txt
--rw-rw-r--   0 stefano   (1000) stefano   (1000)        6 2023-03-06 11:56:26.000000 gw-mbank-0.2.0/gw_mbank.egg-info/top_level.txt
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-03-06 11:56:26.514195 gw-mbank-0.2.0/mbank/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     1990 2022-11-30 15:10:00.000000 gw-mbank-0.2.0/mbank/__init__.py
--rw-r--r--   0 stefano   (1000) stefano   (1000)    30172 2023-02-15 11:17:38.000000 gw-mbank-0.2.0/mbank/bank.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-03-06 11:56:26.514195 gw-mbank-0.2.0/mbank/flow/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     1804 2022-11-30 16:43:08.000000 gw-mbank-0.2.0/mbank/flow/__init__.py
--rw-rw-r--   0 stefano   (1000) stefano   (1000)    21499 2022-12-18 10:55:14.000000 gw-mbank-0.2.0/mbank/flow/flowmodel.py
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     7566 2022-12-02 12:35:01.000000 gw-mbank-0.2.0/mbank/flow/utils.py
--rw-rw-r--   0 stefano   (1000) stefano   (1000)    72234 2023-02-20 09:52:50.000000 gw-mbank-0.2.0/mbank/handlers.py
--rw-r--r--   0 stefano   (1000) stefano   (1000)    55361 2023-03-06 09:45:05.000000 gw-mbank-0.2.0/mbank/metric.py
--rw-rw-r--   0 stefano   (1000) stefano   (1000)    84069 2023-03-06 08:41:58.000000 gw-mbank-0.2.0/mbank/utils.py
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       38 2023-03-06 11:56:26.518195 gw-mbank-0.2.0/setup.cfg
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     1586 2023-03-06 11:55:33.000000 gw-mbank-0.2.0/setup.py
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-22 15:17:28.263680 gw-mbank-0.3.1/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)    35149 2021-10-27 10:33:14.000000 gw-mbank-0.3.1/LICENSE.txt
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     6210 2023-06-22 15:17:28.259680 gw-mbank-0.3.1/PKG-INFO
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     5722 2023-01-30 16:28:41.000000 gw-mbank-0.3.1/README.md
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-22 15:17:28.259680 gw-mbank-0.3.1/bin/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)    13734 2023-04-17 10:10:07.000000 gw-mbank-0.3.1/bin/mbank_injections
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     6179 2023-02-15 17:15:34.000000 gw-mbank-0.3.1/bin/mbank_injections_workflow
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     5783 2023-04-17 10:09:49.000000 gw-mbank-0.3.1/bin/mbank_injfile
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     9189 2023-04-20 12:12:33.000000 gw-mbank-0.3.1/bin/mbank_mcmc
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     5003 2023-03-14 20:40:44.000000 gw-mbank-0.3.1/bin/mbank_merge
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     7127 2023-03-29 19:06:39.000000 gw-mbank-0.3.1/bin/mbank_place_templates
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     3216 2023-04-17 16:27:56.000000 gw-mbank-0.3.1/bin/mbank_print_metric
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)    13444 2023-04-20 11:15:24.000000 gw-mbank-0.3.1/bin/mbank_run
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)    13987 2023-03-27 20:00:51.000000 gw-mbank-0.3.1/bin/mbank_validate_metric
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-22 15:17:28.259680 gw-mbank-0.3.1/gw_mbank.egg-info/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     6210 2023-06-22 15:17:27.000000 gw-mbank-0.3.1/gw_mbank.egg-info/PKG-INFO
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)      526 2023-06-22 15:17:28.000000 gw-mbank-0.3.1/gw_mbank.egg-info/SOURCES.txt
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)        1 2023-06-22 15:17:27.000000 gw-mbank-0.3.1/gw_mbank.egg-info/dependency_links.txt
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)      107 2023-06-22 15:17:28.000000 gw-mbank-0.3.1/gw_mbank.egg-info/requires.txt
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)        6 2023-06-22 15:17:28.000000 gw-mbank-0.3.1/gw_mbank.egg-info/top_level.txt
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-22 15:17:28.259680 gw-mbank-0.3.1/mbank/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     1990 2022-11-30 15:10:00.000000 gw-mbank-0.3.1/mbank/__init__.py
+-rw-r--r--   0 stefano   (1000) stefano   (1000)    30813 2023-06-14 13:55:35.000000 gw-mbank-0.3.1/mbank/bank.py
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-22 15:17:28.259680 gw-mbank-0.3.1/mbank/flow/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     1804 2022-11-30 16:43:08.000000 gw-mbank-0.3.1/mbank/flow/__init__.py
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)    27089 2023-05-08 11:51:42.000000 gw-mbank-0.3.1/mbank/flow/flowmodel.py
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     7546 2023-04-26 09:18:45.000000 gw-mbank-0.3.1/mbank/flow/utils.py
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)    71089 2023-06-22 15:16:23.000000 gw-mbank-0.3.1/mbank/handlers.py
+-rw-r--r--   0 stefano   (1000) stefano   (1000)    62880 2023-05-15 11:18:38.000000 gw-mbank-0.3.1/mbank/metric.py
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)    84022 2023-04-17 12:02:44.000000 gw-mbank-0.3.1/mbank/utils.py
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)       38 2023-06-22 15:17:28.263680 gw-mbank-0.3.1/setup.cfg
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     1615 2023-06-22 15:16:41.000000 gw-mbank-0.3.1/setup.py
```

### Comparing `gw-mbank-0.2.0/LICENSE.txt` & `gw-mbank-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gw-mbank-0.2.0/PKG-INFO` & `gw-mbank-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gw-mbank
-Version: 0.2.0
+Version: 0.3.1
 Summary: Metric bank generation for gravitational waves data analysis
 Home-page: https://github.com/stefanoschmidt1995/mbank
 Author: Stefano Schmidt
 Author-email: stefanoschmidt1995@gmail.com
 License: GNU GENERAL PUBLIC LICENSE v3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gw-mbank-0.2.0/README.md` & `gw-mbank-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `gw-mbank-0.2.0/bin/mbank_injections` & `gw-mbank-0.3.1/bin/mbank_injections`

 * *Files 2% similar despite different names*

```diff
@@ -154,15 +154,15 @@
 
 	#setting default locations for injection file, tiling file and bank file
 if isinstance(args.inj_file, str):
 	if args.inj_file.find('/') <0: args.inj_file = args.run_dir+args.inj_file
 if isinstance(args.stat_dict, str):
 	if args.stat_dict.find('/') <0: args.stat_dict = args.run_dir+args.stat_dict
 else:
-	args.stat_dict = os.path.basename(args.bank_file).split('.')[0]+'-injections_stat_dict.json'
+	args.stat_dict = args.run_dir+os.path.basename(args.bank_file).split('.')[0]+'-injections_stat_dict.json'
 if isinstance(args.flow_file, str):
 	if args.flow_file.find('/') <0: args.flow_file = args.run_dir+args.flow_file
 if metric_match:
 	if args.tiling_file.find('/') <0: args.tiling_file = args.run_dir+args.tiling_file
 if args.bank_file.find('/') <0: args.bank_file = args.run_dir+args.bank_file
 if isinstance(args.psd, str): args.psd = args.run_dir+args.psd if args.psd.find('/') <0 else args.psd
 
@@ -183,15 +183,15 @@
 
 	######
 	#	Loading the bank and instatianting a variable handler
 	######
 bank = cbc_bank(args.variable_format, args.bank_file)
 if args.verbose: print("Loaded bank {} with {} templates".format(args.bank_file, bank.templates.shape[0]))
 
-	#Loading the flow, if it's the case
+	#Loading the tiling and the flow, if it's the case
 if metric_match:
 	t_obj = tiling_handler(args.tiling_file)
 	if isinstance(args.flow_file, str): t_obj.load_flow(args.flow_file)
 
 	######
 	#	Generating injections
 	######
@@ -200,15 +200,15 @@
 
 	assert isinstance(args.n_injs, int), "Argument --n-injs must be specified if an injection file is not given"
 		#generating tiles injections
 	projected_injs = t_obj.sample_from_tiling(args.n_injs, seed = args.seed)
 	
 	#projected_injs = bank.templates; print("######### Bank injections!! ###########") #FIXME: this will become a bank-injs option!! Or something similar
 	
-	injections_full = np.array(var_handler.get_BBH_components(projected_injs, args.variable_format)).T
+	injections_full = var_handler.get_BBH_components(projected_injs, args.variable_format)
 	del projected_injs #storing projected_injs is a waste of memory that can scale super badly
 	
 		#dealing with sky location
 	
 		#Storing injections to file
 	inj_filename = args.run_dir+'injections.xml'
 	if args.fixed_sky_loc_polarization:
```

### Comparing `gw-mbank-0.2.0/bin/mbank_injections_workflow` & `gw-mbank-0.3.1/bin/mbank_injections_workflow`

 * *Files identical despite different names*

### Comparing `gw-mbank-0.2.0/bin/mbank_injfile` & `gw-mbank-0.3.1/bin/mbank_injfile`

 * *Files 1% similar despite different names*

```diff
@@ -129,15 +129,15 @@
 else:
 	raise ValueError("Either --tiling-file or --bank-file options must be non empty")
 
 	#if sky_locs is None, injections will be drawn at random from the sky inside save_injs
 sky_locs = np.array(args.fixed_sky_loc_polarization) if args.fixed_sky_loc_polarization else None
 
 var_handler = variable_handler()
-injs = np.array(var_handler.get_BBH_components(injs, args.variable_format)).T
+injs = var_handler.get_BBH_components(injs, args.variable_format)
 
 save_injs(args.inj_out_file, injs, args.gps_start, args.gps_end, args.time_step, args.approximant,
 	luminosity_distance = (min_dist, max_dist), sky_locs = sky_locs, f_min = args.f_min, f_max = args.f_max)
```

### Comparing `gw-mbank-0.2.0/bin/mbank_mcmc` & `gw-mbank-0.3.1/bin/mbank_mcmc`

 * *Files 1% similar despite different names*

```diff
@@ -105,18 +105,18 @@
 parser.add_argument(
 	"--s2-range", default = [-0.99,0.99], type=float, nargs = 2,
 	help="Range values for magnitude of spin 1 (if applicable)")
 parser.add_argument(
 	"--chi-range", default = [-0.99,0.99], type=float, nargs = 2,
 	help="Range values for effective spin parameter (if applicable)")
 parser.add_argument(
-	"--theta-range", default = [0., np.pi], type=float, nargs = 2,
+	"--theta-range", default = [-np.pi, np.pi], type=float, nargs = 2,
 	help="Range values for theta angles of spins (if applicable)")
 parser.add_argument(
-	"--phi-range", default = [-np.pi, np.pi], type=float, nargs = 2,
+	"--phi-range", default = [-np.pi/2, np.pi/2], type=float, nargs = 2,
 	help="Range values for phi angles of spins (if applicable)")
 parser.add_argument(
 	"--e-range", default = [0., 0.5], type=float, nargs = 2,
 	help="Range values for the eccentricity (if applicable)")
 parser.add_argument(
 	"--meanano-range", default = [0., 1], type=float, nargs = 2,
 	help="Range values for the mean anomaly (if applicable). TODO: find a nice default...")
```

### Comparing `gw-mbank-0.2.0/bin/mbank_merge` & `gw-mbank-0.3.1/bin/mbank_merge`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,18 @@
 if args.tiling: tiling.save(args.out_name)
 
 if args.injection_stat:
 	merged_stat_dict = {}
 	for stat_dict in stat_dict_list:
 		for k,v in stat_dict.items():
 			if k in merged_stat_dict:
-				if isinstance(v, (float, int)) or v is None:
+				if k == 'sky_loc':
+					if v.ndim == 1: assert np.allclose(v, merged_stat_dict[k]), "The sky locations of the injection statistics dictionaries are not compatible"
+					continue
+				if isinstance(v, (float, int)) or (v is None):
 					assert v == merged_stat_dict[k], "The given injection statistics dictionary are not compatible: are the metadata the same?"
 					continue
 				merged_stat_dict[k] = np.concatenate([merged_stat_dict[k], v], axis = 0)
 			else:
 				merged_stat_dict[k] = v
 	save_inj_stat_dict(args.out_name, merged_stat_dict)
```

### Comparing `gw-mbank-0.2.0/bin/mbank_place_templates` & `gw-mbank-0.3.1/bin/mbank_place_templates`

 * *Files 3% similar despite different names*

```diff
@@ -55,14 +55,17 @@
 parser.add_argument(
 	"--placing-method", default = 'geometric', type = str, choices = cbc_bank('Mq_nonspinning').placing_methods,
 	help="Which placing method to use for each tile")
 parser.add_argument(
 	"--n-livepoints", default = 10000, type = float,
 	help="Parameter to control the number of livepoints to use in the `random` and `pruning` placing method. For `random` (or related), it represents the number of livepoints to use for the estimation of the coverage fraction. For `pruning`, it amounts to the the ratio between the number of livepoints and the number of templates placed by ``uniform`` placing method.")
 parser.add_argument(
+	"--covering-fraction", default = 0.01, type = float,
+	help="Parameter to control the maximum fraction of livepoints alive before terminating the bank generation with the `random` and `pruning` placing method. The smaller the threshold, the higher the nuber of templates in the final bank.")
+parser.add_argument(
 	"--empty-iterations", default = 100, type = float,
 	help="Number of consecutive rejected proposal after which the `stochastic` placing method stops.")
 parser.add_argument(
 	"--use-ray", action='store_true', default = False,
 	help="Whether to use ray package to parallelize the metric computation")
 parser.add_argument(
 	"--show", action='store_true', default = False,
@@ -131,15 +134,15 @@
 t_obj = tiling_handler(args.tiling_file)
 
 if args.train_flow:
 	t_obj.train_flow(N_epochs = args.n_epochs, n_layers = args.n_layers, hidden_features = args.hidden_features, verbose = True)
 	t_obj.flow.save_weigths(args.flow_file)
 elif isinstance(args.flow_file, str): t_obj.load_flow(args.flow_file)
 
-bank.place_templates(t_obj, args.mm, placing_method = args.placing_method, N_livepoints = args.n_livepoints, empty_iterations = args.empty_iterations, verbose = True)
+bank.place_templates(t_obj, args.mm, placing_method = args.placing_method, N_livepoints = args.n_livepoints, covering_fraction = args.covering_fraction, empty_iterations = args.empty_iterations, verbose = True)
 
 	######
 	#	Plotting & saving
 	######
 
 print("Generated bank with {} templates".format(len(bank.templates)))
 print("Saving bank to {}".format(args.run_dir))
```

### Comparing `gw-mbank-0.2.0/bin/mbank_run` & `gw-mbank-0.3.1/bin/mbank_run`

 * *Files 11% similar despite different names*

```diff
@@ -10,21 +10,27 @@
 	mbank_run --options-you-like
 
 You can also load (some) options from an ini-file:
 
 	mbank_run --some-options other_options.ini
 
 Make sure that the mbank is properly installed.
+
+To create a sub file and run in condor:
+
+	mbank_run --make-sub options.ini
+
 To know which options are available:
 
 	mbank_run --help
 """
 import numpy as np
 import matplotlib.pyplot as plt
 import sys
+import warnings
 from ligo.lw.utils import load_filename
 
 from mbank import variable_handler, cbc_metric, cbc_bank
 from mbank.utils import updates_args_from_ini, int_tuple_type, load_PSD, avg_dist, plot_tiles_templates, get_boundaries_from_ranges
 from mbank.flow.utils import compare_probability_distribution
 
 import argparse
@@ -79,24 +85,27 @@
 parser.add_argument(
 	"--placing-method", default = 'geometric', type = str, choices = cbc_bank('Mq_nonspinning').placing_methods,
 	help="Which placing method to use for each tile")
 parser.add_argument(
 	"--n-livepoints", default = 10000, type = float,
 	help="Parameter to control the number of livepoints to use in the `random` and `pruning` placing method. For `random` (or related), it represents the number of livepoints to use for the estimation of the coverage fraction. For `pruning`, it amounts to the the ratio between the number of livepoints and the number of templates placed by ``uniform`` placing method.")
 parser.add_argument(
+	"--covering-fraction", default = 0.01, type = float,
+	help="Parameter to control the maximum fraction of livepoints alive before terminating the bank generation with the `random` and `pruning` placing method. The smaller the threshold, the higher the nuber of templates in the final bank.")
+parser.add_argument(
 	"--empty-iterations", default = 100, type = float,
 	help="Number of consecutive rejected proposal after which the `stochastic` placing method stops.")
 parser.add_argument(
 	"--tile-tolerance", default = 0.1, type = float,
 	help="Maximum tolerated variation of the relative difference of the metric determinant between parent and child in the iterative splitting procedure")
 parser.add_argument(
 	"--max-depth", default = 6, type = int,
 	help="Maximum number of iterative splitting before terminating.")
 parser.add_argument(
-	"--metric-type", default = 'hessian', type = str, choices = ['hessian', 'parabolic_fit_hessian', 'symmetrized'],
+	"--metric-type", default = 'hessian', type = str, choices = ['hessian', 'parabolic_fit_hessian', 'symphony'],
 	help="Method to use to compute the metric.")
 parser.add_argument(
 	"--use-ray", action='store_true', default = False,
 	help="Whether to use ray package to parallelize the metric computation")
 
 parser.add_argument(
 	"--train-flow", action='store_true', default = False,
@@ -133,34 +142,52 @@
 parser.add_argument(
 	"--s2-range", default = [-0.99,0.99], type=float, nargs = 2,
 	help="Range values for magnitude of spin 1 (if applicable)")
 parser.add_argument(
 	"--chi-range", default = [-0.99,0.99], type=float, nargs = 2,
 	help="Range values for effective spin parameter (if applicable)")
 parser.add_argument(
-	"--theta-range", default = [0., np.pi], type=float, nargs = 2,
+	"--theta-range", default = [-np.pi, np.pi], type=float, nargs = 2,
 	help="Range values for theta angles of spins (if applicable)")
 parser.add_argument(
-	"--phi-range", default = [-np.pi, np.pi], type=float, nargs = 2,
+	"--phi-range", default = [-np.pi/2, np.pi/2], type=float, nargs = 2,
 	help="Range values for phi angles of spins (if applicable)")
 parser.add_argument(
 	"--e-range", default = [0., 0.5], type=float, nargs = 2,
 	help="Range values for the eccentricity (if applicable)")
 parser.add_argument(
 	"--meanano-range", default = [0., 1], type=float, nargs = 2,
 	help="Range values for the mean anomaly (if applicable). TODO: find a nice default...")
 parser.add_argument(
 	"--iota-range", default = [0., np.pi], type=float, nargs = 2,
 	help="Range values for iota (if applicable)")
 parser.add_argument(
 	"--ref-phase-range", default = [-np.pi, np.pi], type=float, nargs = 2,
 	help="Range values for reference phase (if applicable)")
 
+parser.add_argument(
+	"--make-sub",  default = False, action='store_true',
+	help="If set, it will make a condor submit file that the user can use to launch the job through condor.")
+
 args, filenames = parser.parse_known_args()
 
+sub_file_str = """Universe   = vanilla
+Executable = {}
+arguments = "{}"
+getenv = true
+Log = {}_mbank_run_{}.log
+Error = {}_mbank_run_{}.err
+Output = {}_mbank_run_{}.out
+request_memory = 4GB
+request_cpus = {}
+request_disk = 4GB
+
+queue
+"""
+
 	#updating from the ini file(s), if it's the case
 for f in filenames:
 	args = updates_args_from_ini(f, args, parser)
 
 ####################################################################################################
 	######
 	#	Interpreting the parser and initializing variables
@@ -175,14 +202,37 @@
 if args.run_dir == './out_$(run_name)':	args.run_dir = './out_{}/'.format(args.run_name)
 if not args.run_dir.endswith('/'): args.run_dir = args.run_dir+'/'
 if not os.path.exists(args.run_dir): os.makedirs(args.run_dir)
 if args.psd.find('/') <0: args.psd = args.run_dir+args.psd
 
 if args.grid_size is None: args.grid_size = tuple([1 for i in range(var_handler.D(args.variable_format))])
 
+if args.make_sub:
+	if '--make-sub' in sys.argv:
+		sys.argv.remove('--make-sub')
+	else:
+		warnings.warn('The option --make-sub was given in the inifile. Make sure you remove it from your ini before launching the condor job!')
+	n_cpu = None if args.grid_size is None else int(np.prod(args.grid_size))
+	sub_file_str = sub_file_str.format(sys.argv[0], ' '.join(sys.argv[1:]),
+		args.run_dir, args.run_name,
+		args.run_dir, args.run_name,
+		args.run_dir, args.run_name,
+		n_cpu)
+	
+	sub_file = args.run_dir+'mbank_run_{}.sub'.format(args.run_name)
+	with open(sub_file, 'w') as f:
+		f.write(sub_file_str)
+	print('#####')
+	sub_file = args.run_dir+'mbank_run_{}.sub'.format(args.run_name)
+	print("Submit file generated @ {}\nSubmit a job it with condor_submit {}\n".format(sub_file, sub_file))
+	print("Monitor it with: tail -f {}mbank_run_{}.err".format(args.run_dir, args.run_name))
+	print('#####')
+	print(sub_file_str)
+	quit()
+
 m_min, m_max = args.m_range
 mtot_min, mtot_max = args.mtot_range
 q_min, q_max = args.q_range
 mc_min, mc_max = args.mc_range
 eta_min, eta_max = args.eta_range
 s1_min, s1_max = args.s1_range
 s2_min, s2_max = args.s2_range
@@ -236,18 +286,18 @@
 bank = cbc_bank(args.variable_format)
 
 if format_info['mass_format'] == 'm1m2':
 	raise NotImplementedError("Currently no template placement is implemented for the mass format m1m2.")
 
 else:
 	t_obj = bank.generate_bank(m, minimum_match = args.mm, boundaries = boundaries,
-		tolerance = args.tile_tolerance,
+		max_depth = args.max_depth, tolerance = args.tile_tolerance,
 		placing_method = args.placing_method, metric_type = args.metric_type,
 		grid_list = args.grid_size, train_flow = args.train_flow,
-		N_livepoints = args.n_livepoints, empty_iterations = args.empty_iterations, max_depth = args.max_depth,
+		N_livepoints = args.n_livepoints, covering_fraction = args.covering_fraction, empty_iterations = args.empty_iterations,
 		use_ray = args.use_ray, n_layers = args.n_layers, hidden_features = args.hidden_features, N_epochs = args.n_epochs)
 	
 	tiling_file = args.run_dir+'tiling_{}.npy'.format(args.run_name)
 	flow_file = args.run_dir+'flow_{}.zip'.format(args.run_name) if args.train_flow else None
 	t_obj.save(tiling_file, flow_file) #saving also the flow
 
 if bank.templates is None:
```

### Comparing `gw-mbank-0.2.0/bin/mbank_validate_metric` & `gw-mbank-0.3.1/bin/mbank_validate_metric`

 * *Files 2% similar despite different names*

```diff
@@ -135,14 +135,17 @@
 parser.add_argument(
 	"--overlap",  default = False, action='store_true',
 	help="Whether to compute the metric based on the overlap rather than the match")
 parser.add_argument(
 	"--metric-type", default = 'hessian',
 	help="The metric computation method to use")
 parser.add_argument(
+	"--symphony-match", default = False, action='store_true',
+	help="Whether to compute the match with the symphony match")
+parser.add_argument(
 	"--on-boundaries",  default = False, action='store_true',
 	help="Whether the sampled points for validation should be drawn on the boundaries of the constant match ellipse. If False (default) points will be drawn inside.")
 parser.add_argument(
 	"--show", type = bool, default = True,
 	help="Whether to show the plots")
 parser.add_argument(
 	"--N-points",  default = 500, type=int,
@@ -183,27 +186,29 @@
 
 	######
 	# Computing the metric in all its forms
 	######
 
 target_match = 0.9
 metric_hessian = m_obj.get_hessian(center, overlap = args.overlap, order = None, epsilon = args.epsilon)
+metric_symphony = m_obj.get_hessian_symphony(center, overlap = args.overlap, order = None, epsilon = args.epsilon)
 metric_fisher = m_obj.get_fisher_matrix(center, overlap = args.overlap, order = None, epsilon = args.epsilon)
 metric_block_diagonal = m_obj.get_block_diagonal_hessian(center,  overlap = args.overlap, epsilon = 1e-6, order = None)
 metric_numerical = np.eye(center.shape[0])  #m_obj.get_numerical_hessian(center,  overlap = overlap, target_match = 0.999, epsilon = 1e-6)
 metric_parabolae, parabolae, original_parabola_metric = m_obj.get_parabolic_fit_hessian(center, overlap = args.overlap, target_match = target_match,
 			N_epsilon_points = 10, log_epsilon_range = (-5, 1), full_output = True)
 
 metric = m_obj.get_metric(center, overlap = args.overlap, metric_type = args.metric_type, epsilon = args.epsilon)
 
 print("Variable format: ", args.variable_format)
 print("Approximant: ", args.approximant)
 print("Frequency range: ", args.f_min, args.f_max)
 print("center: ", center)
 print("  Eig hessian: ", np.linalg.eig(metric_hessian)[0], np.linalg.det(metric_hessian))
+print("  Eig symphony: ", np.linalg.eig(metric_symphony)[0], np.linalg.det(metric_symphony))
 print("  Eig Fisher: ", np.linalg.eig(metric_fisher)[0], np.linalg.det(metric_fisher))
 print("  Eig block diagonal: ", np.linalg.eig(metric_block_diagonal)[0], np.linalg.det(metric_block_diagonal))
 print("  Eig numerical hessian: ", np.linalg.eig(metric_numerical)[0], np.linalg.det(metric_numerical))
 print("  Eig parabola metric: ", np.linalg.eig(metric_parabolae)[0], np.linalg.det(metric_parabolae))
 
 if args.save_dir is None and not args.show: quit()
 
@@ -215,15 +220,16 @@
 ids_inside = m_obj.var_handler.is_theta_ok(points, args.variable_format, raise_error = False) #DEBUG
 
 #p1, p2 = m_obj.get_points_at_match(args.N_points, center, match = args.match, metric = metric, overlap = args.overlap)
 #ids_inside = np.logical_and(m_obj.var_handler.is_theta_ok(p1, args.variable_format, raise_error = False),
 #		m_obj.var_handler.is_theta_ok(p2, args.variable_format, raise_error = False))#DEBUG
 
 if sum(ids_inside)>0:
-	matches[ids_inside] = m_obj.match(points[ids_inside, :], center, overlap = args.overlap)
+	matches[ids_inside] = m_obj.match(points[ids_inside, :], center,
+		overlap = args.overlap, symphony = args.symphony_match, antenna_patterns = (1,0))
 	#matches[ids_inside] = m_obj.match(p1[ids_inside, :], p2[ids_inside, :], overlap = args.overlap) #DEBUG
 #points = np.concatenate([p1, p2], axis = 0)
 #matches = np.concatenate([matches, matches], axis = 0)
 
 	######
 	# Plotting the parabolae
 	######
@@ -250,17 +256,18 @@
 plt.close(plt.get_fignums()[-1])
 plt.suptitle("{} - {}\ncenter = {}".format(args.variable_format, args.approximant, center), fontsize = 25)
 if args.save_dir is not None: plt.savefig(args.save_dir+"ellipses.png")
 
 	#histogram
 plt.figure()
 plt.title("Center: {} - Overlap {}".format(center, args.overlap))
-hist_kwargs = {'bins': 20, 'histtype':'step', 'color':'orange'}
+hist_kwargs = {'bins': 20, 'histtype':'step', 'density':True, 'cumulative': True, 'color':'orange'}
 plt.hist(matches, label = 'mbank', **hist_kwargs)
 plt.axvline(args.match, c = 'r')
+plt.yscale('log')
 plt.legend()
 if args.save_dir is not None: plt.savefig(args.save_dir+"validation_hist.png")
 
 	
 	######
 	# Epsilon validation (plots and computation)
 	######
```

### Comparing `gw-mbank-0.2.0/gw_mbank.egg-info/PKG-INFO` & `gw-mbank-0.3.1/gw_mbank.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gw-mbank
-Version: 0.2.0
+Version: 0.3.1
 Summary: Metric bank generation for gravitational waves data analysis
 Home-page: https://github.com/stefanoschmidt1995/mbank
 Author: Stefano Schmidt
 Author-email: stefanoschmidt1995@gmail.com
 License: GNU GENERAL PUBLIC LICENSE v3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gw-mbank-0.2.0/mbank/__init__.py` & `gw-mbank-0.3.1/mbank/__init__.py`

 * *Files identical despite different names*

### Comparing `gw-mbank-0.2.0/mbank/bank.py` & `gw-mbank-0.3.1/mbank/bank.py`

 * *Files 3% similar despite different names*

```diff
@@ -163,15 +163,15 @@
 			End frequency (in Hz) for the templates
 		
 		ifo: str
 			Name of the interferometer the bank refers to 
 		
 		"""
 			#getting the masses and spins of the rows
-		m1, m2, s1x, s1y, s1z, s2x, s2y, s2z, e, meanano, iota, phi = self.var_handler.get_BBH_components(self.templates, self.variable_format)
+		m1, m2, s1x, s1y, s1z, s2x, s2y, s2z, e, meanano, iota, phi = self.var_handler.get_BBH_components(self.templates, self.variable_format).T
 		
 		if np.any(e != 0.):
 			msg = "Currently xml format does not support eccentricity... The saved bank '{}' will have zero eccentricity".format(filename)
 			warnings.warn(msg)
 		
 			#preparing the doc
 			#See: https://git.ligo.org/RatesAndPopulations/lvc-rates-and-pop/-/blob/master/bin/lvc_rates_injections#L168
@@ -270,15 +270,15 @@
 		Returns
 		-------
 			BBH_components: :class:`~numpy:numpy.ndarray`
 				shape: (N,12)
 				Array of BBH components of the templates in the bank. They have the same layout as :func:`mbank.handlers.variable_handler.get_BBH_components`
 		"""
 		if self.templates is not None:
-			return np.array(self.var_handler.get_BBH_components(self.templates, self.variable_format)).T
+			return self.var_handler.get_BBH_components(self.templates, self.variable_format)
 		return
 		
 	def add_templates(self, new_templates):
 		"""
 		Adds a bunch of templates to the bank. They must be of a shape suitable for the variable format
 		
 		Parameters
@@ -303,15 +303,15 @@
 		if self.templates is None:
 			self.templates = new_templates
 		else:
 			self.templates = np.concatenate([self.templates, new_templates], axis = 0) #(N,4)
 		
 		return
 		
-	def place_templates(self, tiling, minimum_match, placing_method, N_livepoints = 10000, empty_iterations = 100, verbose = True):
+	def place_templates(self, tiling, minimum_match, placing_method, N_livepoints = 10000, covering_fraction = 0.01, empty_iterations = 100, verbose = True):
 		"""
 		Given a tiling, it places the templates according to the given method and **adds** them to the bank
 		
 		Parameters
 		----------
 
 		tiling: tiling_handler
@@ -339,14 +339,17 @@
 			Those methods are listed in `cbc_bank.placing_methods`
 		
 		N_livepoints: float
 			Only applies for `random` method or `pruning` method.
 			For `random` (or related), it represents the number of livepoints to use for the estimation of the coverage fraction.
 			For `pruning`, it amounts to the the ratio between the number of livepoints and the number of templates placed by ``uniform`` placing method.
 		
+		covering_fraction: float
+			Only applies for `random` method or `pruning` method. Fraction of livepoints to be covered before terminating the loop
+		
 		empty_iterations: int
 			Number of consecutive proposal inside a tile to be rejected before the tile is considered full. It only applies to the ``stochastic`` placing method (or related).
 		
 		verbose: bool
 			Whether to print the output
 		
 		Returns
@@ -365,15 +368,15 @@
 		if self.variable_format.startswith('m1m2_'):
 			raise RuntimeError("Currently mbank does not support template placing with m1m2 format for the masses")
 		
 		for R, M in tiling:
 			eigs, _ = np.linalg.eig(M)
 					#sanity checks on the metric eigenvalues
 			if np.any(eigs < 0):
-				warnings.warn("The metric has a negative eigenvalue: the template placing in this tile may be unreliable. This is pathological as the metric computation may have failed.")
+				warnings.warn("The metric has a negative eigenvalue @ {}: the template placing in this tile may be unreliable. This is pathological as the metric computation may have failed.\nEigvs are: {}".format((R.maxes+R.mins)/2, eigs))
 			
 			abs_det = np.abs(np.prod(eigs))
 			if abs_det < 1e-50: #checking if the determinant is close to zero...
 				msg = "The determinant of the metric is zero! It is impossible to place templates into this tile: maybe the approximant you are using is degenerate with some of the sampled quantities?\nRectangle: {}\nMetric: {}".format(R, M)
 				raise ValueError(msg)
 		
 		
@@ -424,15 +427,15 @@
 		if placing_method in ['uniform', 'qmc']:
 			vol_tot, _ = tiling.compute_volume()
 			N_templates = int( vol_tot/(dist**self.D) )+1
 			if tiling.flow and placing_method == 'uniform': new_templates = tiling.sample_from_flow(N_templates)
 			else: new_templates = tiling.sample_from_tiling(N_templates, qmc = (placing_method=='qmc'))
 		
 		if placing_method in ['random', 'random_stochastic']:
-			new_templates = place_random(minimum_match, tiling, N_livepoints = N_livepoints, tolerance = 0.01, verbose = verbose)
+			new_templates = place_random(minimum_match, tiling, N_livepoints = N_livepoints, covering_fraction = covering_fraction, verbose = verbose)
 		
 		if placing_method in ['geo_stochastic', 'random_stochastic', 'iterative_stochastic', 'stochastic']:
 			new_templates = place_stochastically(minimum_match, tiling,
 					empty_iterations = empty_iterations,
 					seed_bank =  None if placing_method == 'stochastic' else new_templates, verbose = verbose)	
 		
 		
@@ -454,26 +457,28 @@
 			new_templates = []
 			if verbose: it = tqdm(partition, desc = 'Loops on the partitions for random placement')
 			else: it = partition
 			for p in it:
 				#TODO: make this a ray function? Too much memory expensive, probably...
 					#The template volume for random is sqrt(1-MM) (not dist)
 				
-				new_templates_ = place_pruning(minimum_match, p, N_points = int(N_points(p)), tolerance = 0.0001, verbose = verbose)
+				new_templates_ = place_pruning(minimum_match, p, N_points = int(N_points(p)),
+					covering_fraction = covering_fraction, verbose = verbose)
 				
 				new_templates.extend(new_templates_)
 			
 		new_templates = np.stack(new_templates, axis =0)
 		self.add_templates(new_templates)
 		
 		return new_templates
 
 	def generate_bank(self, metric_obj, minimum_match, boundaries, tolerance,
 			placing_method = 'random', metric_type = 'hessian', grid_list = None, train_flow = False,
-			use_ray = False, N_livepoints = 50, empty_iterations = 100, max_depth = 6, n_layers = 2, hidden_features = 4, N_epochs = 1000):
+			use_ray = False, N_livepoints = 50, covering_fraction = 0.01, empty_iterations = 100,
+			max_depth = 6, n_layers = 2, hidden_features = 4, N_epochs = 1000, verbose = True):
 		#FIXME: here you should use kwargs, directing the user to the docs of other functions?
 		"""
 		Generates a bank using a hierarchical hypercube tesselation. 
 		The bank generation consists in two steps:
 		
 		1. Tiling generation by iterative splitting of the parameter space
 		2. Template placing in each tile, according to the method given in ``placing_method``
@@ -512,14 +517,17 @@
 		use_ray: bool
 			Whether to use ray to parallelize
 		
 		N_livepoints: float
 			Only applies for `random` method or `pruning` method.
 			For `random` (or related), it represents the number of livepoints to use for the estimation of the coverage fraction.
 			For `pruning`, it amounts to the the ratio between the number of livepoints and the number of templates placed by ``uniform`` placing method.
+			
+		covering_fraction: float
+			Only applies for `random` method or `pruning` method. Fraction of livepoints to be covered before terminating the template placing
 		
 		empty_iterations: int
 			Number of consecutive proposal inside a tile to be rejected before the tile is considered full. It only applies to the ``stochastic`` placing method.
 		
 		max_depth: int
 			Maximum number of splitting before quitting the iteration. If None, the iteration will go on until the volume condition is not met
 		
@@ -530,14 +538,17 @@
 		hidden_features: int
 			Number of hidden features for the masked autoregressive flow in use.
 			See `mbank.flow.STD_GW_flow` for more information
 		
 		N_epochs: int
 			Number of epochs for the training of the flow
 		
+		verbose: bool
+			Whether to print some output
+		
 		Returns
 		-------
 		
 		tiling: tiling_handler 
 			A list of tiles used for the bank generation
 		"""
 			##
@@ -564,45 +575,48 @@
 		metric_fun = lambda center: metric_obj.get_metric(center, overlap = False, metric_type = metric_type)
 									#metric_type = 'hessian')
 									#metric_type = 'block_diagonal_hessian')
 									#metric_type = 'parabolic_fit_hessian', target_match = 0.9, N_epsilon_points = 10, log_epsilon_range = (-4, 1))
 		t_obj = tiling_handler() #empty tiling handler
 		t_obj.create_tiling_from_list(boundaries_list, tolerance, metric_fun, max_depth = max_depth, use_ray = use_ray )	
 		
-		if train_flow: t_obj.train_flow(N_epochs = N_epochs, n_layers = n_layers, hidden_features =  hidden_features, verbose = True)
+		if train_flow: t_obj.train_flow(N_epochs = N_epochs, n_layers = n_layers, hidden_features =  hidden_features, verbose = verbose)
 		
 			##
 			#placing the templates
 			#(if there is KeyboardInterrupt, the tiling is returned anyway)
 
 		try:
-			self.place_templates(t_obj, minimum_match, placing_method = placing_method, N_livepoints = N_livepoints, empty_iterations = empty_iterations, verbose = True)
+			self.place_templates(t_obj, minimum_match, placing_method = placing_method, N_livepoints = N_livepoints,
+				covering_fraction =covering_fraction, empty_iterations = empty_iterations, verbose = verbose)
 		except KeyboardInterrupt:
 			self.templates = None
 		
 		return t_obj
 				
 	def enforce_boundaries(self, boundaries):
 		"""
 		Remove from the bank the templates that do not lie within the given boundaries
 		
 		Parameters
 		----------
 
 		boundaries: :class:`~numpy:numpy.ndarray`
-			shape: (2,4)/(2,2) -
+			shape: (2,D) -
 			An array with the boundaries for the model. Lower limit is boundaries[0,:] while upper limits is boundaries[1,:]
 		"""	
+		boundaries = np.asarray(boundaries)
 		if self.templates is None: return
 
 		ids_ok = np.logical_and(np.all(self.templates > boundaries[0,:], axis =1), np.all(self.templates < boundaries[1,:], axis = 1)) #(N,)
-		if len(ids_ok) == 0:
+		new_bank_size = sum(ids_ok)
+		if new_bank_size == 0:
 			self.templates = None
 			warnings.warn("No template fits into the boundaries")
-		elif len(ids_ok) < self.templates.shape[0]:
+		elif new_bank_size < self.templates.shape[0]:
 			self.templates = self.templates[ids_ok,:]
 		else:
 			pass
 			#print("The bank already fits into the boundaries")
 
 		return
```

### Comparing `gw-mbank-0.2.0/mbank/flow/__init__.py` & `gw-mbank-0.3.1/mbank/flow/__init__.py`

 * *Files identical despite different names*

### Comparing `gw-mbank-0.2.0/mbank/flow/flowmodel.py` & `gw-mbank-0.3.1/mbank/flow/flowmodel.py`

 * *Files 9% similar despite different names*

```diff
@@ -201,15 +201,15 @@
 		
 				#Dealing with the first transformation
 				#Setting low and high
 		if isinstance(self._transform._transforms[0], TanhTransform):
 			low, _ = torch.min(train_data, axis = 0)
 			high, _ = torch.max(train_data, axis = 0)
 				#the interval between low and high is made larger by a factor epsilon
-			epsilon_ = 0.01 #TODO: tune this number: previously it was 0.2
+			epsilon_ = 0.1 #TODO: tune this number: previously it was 0.2
 			diff = high-low
 			assert torch.all(torch.abs(diff)>1e-20), "The training set has at least one degenerate dimension! Unable to continue with the training"
 			low = low - diff*epsilon_
 			high = high + diff*epsilon_
 
 			for param, val in zip(self._transform._transforms[0].parameters(), [low, high]):
 				param.data = val
@@ -268,14 +268,151 @@
 			'valmetric_value': np.array(metric),
 			'valmetric_mean': metric_computer.metric_mean,
 			'valmetric_std': metric_computer.metric_std,
 			'validation_metric': validation_metric
 		}
 
 		return history
+
+	def train_flow_importance_sampling(self, N_epochs, train_data, train_weights, validation_data, validation_weights, optimizer, batch_size = None, validation_step = 10, callback = None, verbose = False):
+		"""
+		Trains the flow with forward KL plus importance sampling
+		We use importance sampling to have a MC estimation of Eq. (13) of `1912.02762 <https://arxiv.org/abs/1912.02762>`_.
+		
+		Parameters
+		----------
+			N_epochs: int
+				Number of training epochs
+			
+			train_data: :class:`~numpy:numpy.ndarray`
+				Training data. They need to fit the dimensionality of the flow and be convertible into a torch tensor
+			
+			train_weights: :class:`~numpy:numpy.ndarray`
+				Weights for each of the training data
+			
+			validation_data: :class:`~numpy:numpy.ndarray`
+				Validation data. They need to fit the dimensionality of the flow and be convertible into a torch tensor
+			
+			validation_weights: :class:`~numpy:numpy.ndarray`
+				Weights for each of the validation data
+			
+			optimizer: torch.optim
+				An torch optimizer object. Typical usage is:
+				
+				.. code-block:: python
+				
+					from torch import optim
+					flow = GW_Flow(**args)
+					optimizer = optim.Adam(flow.parameters(), lr=0.001)
+
+			batch_size: int
+				Batch size: number of points of the training set to be used at each iteration
+			
+			validation_step: int
+				Number of training steps after which the validation metric is computed
+			
+			callback: callable
+				A callable, called at each validation step of the training.
+				It has to have call signature ``callback(GW_Flow, epoch)``: see :func:`mbank.flow.utils.plotting_callback` for an example.
+
+			verbose: bool
+				Whether to print a progress bar during the training
+
+		Returns
+		-------
+			history: dict
+				A dictionary keeping the historical values of training & validation loss function + KS metric.
+				It has the following entries:
+				
+				- `validation_step`: number of epochs between two consecutive evaluation of the validation metrics
+				- `train_loss`: values of the loss function at each iteration
+				- `validation_loss`: values of the validation loss function at each validation iteration
+				- `valmetric_value`: values of the validation metric at each validation iteration
+				- `valmetric_mean`: expected value of the validation metric for a perfectly trained flow
+				- `valmetric_std`: standard deviation of the validation metric for a perfectly trained flow
+				- `validation_metric`: name of the validation metric being used
+		"""
+		#TODO: implement early stopping!!
+		#FIXME: there's something weird with cross entropy: why do you exceed the threshold even though the loss function still goes down?
+
+		if isinstance(callback, tuple): callback, callback_step = callback
+		else: callback_step = 10
+		
+			#Are you sure you want float32?
+		train_data = torch.tensor(train_data, dtype=torch.float32)
+		validation_data = torch.tensor(validation_data, dtype=torch.float32)
+		train_weights = torch.tensor(train_weights, dtype=torch.float32)
+		validation_weights = torch.tensor(validation_weights, dtype=torch.float32)
+		
+		N_train = train_data.shape[0]
+		
+				#Dealing with the first transformation
+				#Setting low and high
+		if isinstance(self._transform._transforms[0], TanhTransform):
+			low, _ = torch.min(train_data, axis = 0)
+			high, _ = torch.max(train_data, axis = 0)
+				#the interval between low and high is made larger by a factor epsilon
+			epsilon_ = 0.1 #TODO: tune this number: previously it was 0.2
+			diff = high-low
+			assert torch.all(torch.abs(diff)>1e-20), "The training set has at least one degenerate dimension! Unable to continue with the training"
+			low = low - diff*epsilon_
+			high = high + diff*epsilon_
+
+			for param, val in zip(self._transform._transforms[0].parameters(), [low, high]):
+				param.data = val
+			#print("params: ",[p.data for p in self._transform._transforms[0].parameters()])
+			#print("train low high ", [torch.min(train_data, axis = 0)[0],  torch.max(train_data, axis = 0)[0]])
+			#print("val low high ",[torch.min(validation_data, axis = 0)[0],
+			#			torch.max(validation_data, axis = 0)[0]])
+
+		else:
+			msg = "The first layer is not of the kind 'TanhTransform': although this will not break anything, it is *really* recommended to have it as a first layer. It is much needed to transform bounded data into unbounded ones."
+			warnings.warn(msg)
+
+		val_loss=[]
+		train_loss=[]
+		metric = [] #Kolmogorov–Smirnov metric (kind of)
+				
+		desc_str = 'Training loop - loss: {:5f}|{:5f}'
+		if verbose: it = tqdm(range(N_epochs), desc = desc_str.format(np.inf, np.inf))
+		else: it = range(N_epochs)
+		
+		try:
+			for i in it:
+
+				if isinstance(batch_size, int):
+					ids_ = torch.randperm(N_train)[:batch_size]
+				else:
+					ids_ = range(N_train)
+
+				optimizer.zero_grad()
+				loss = -(self.log_prob(inputs=train_data[ids_,:])*train_weights[ids_]).mean()
+				loss.backward()
+				optimizer.step()
+				
+				train_loss.append(loss.item())
+
+				if not (i%validation_step):
+					with torch.no_grad():			
+						loss = -(self.log_prob(inputs=validation_data)*validation_weights).mean()
+					val_loss.append(loss)
+					
+				if callable(callback) and not (i%callback_step): callback(self, i)
+				if not (i%int(N_epochs//1000+1)) and verbose: it.set_description(desc_str.format(train_loss[i], val_loss[-1]))
+		except KeyboardInterrupt:
+			if verbose: print("KeyboardInterrupt: quitting the training loop")
+
+		history = {'validation_step': validation_step,
+			'train_loss': np.array(train_loss),
+			'validation_loss': np.array(val_loss),
+			'valmetric_value': np.array(metric),
+		}
+
+		return history
+
 	
 	def train_flow_metric(self, N_epochs, train_data, validation_data, optimizer, batch_size = None, validation_step = 10, alpha = 100, callback = None, validation_metric = 'cross_entropy', verbose = False):
 		#"Train the flow with PDF and metric"
 		#raise NotImplementedError("Implement a nice and viable loss function :D")
 		if isinstance(callback, tuple): callback, callback_step = callback
 		else: callback_step = 10
```

### Comparing `gw-mbank-0.2.0/mbank/flow/utils.py` & `gw-mbank-0.3.1/mbank/flow/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,16 +221,14 @@
 	g.map_diag(sns.histplot, element = 'step')
 	g.add_legend()
 
 	if isinstance(title, str): plt.suptitle(title)
 	if isinstance(savefile, str):plt.savefig(savefile)
 	if show: plt.show()
 
-	plt.close('all')
-	
 	return
```

### Comparing `gw-mbank-0.2.0/mbank/handlers.py` & `gw-mbank-0.3.1/mbank/handlers.py`

 * *Files 5% similar despite different names*

```diff
@@ -166,15 +166,24 @@
 				#adding the format to the different dicts
 			self.valid_formats.append(format_to_add)
 			self.format_D[format_to_add] = 2+ D_spins[s_] + D_ecc[e_] + D_angles[a_] #dimension of the variable format
 			self.format_info[format_to_add] = {'D':self.format_D[format_to_add],
 				'mass_format': m_, 'spin_format': s_, 'eccentricity_format': e_, 'angle_format':a_,
 				'e': (e_.find('e')>-1), 'meanano': (e_.find('meanano')>-1),
 				'iota': (a_.find('iota')>-1) ,'phi': (a_.find('phi')>-1)}
-			
+		
+			#Adding format BBH_components
+		self.valid_formats.append('BBH_components')
+		self.format_D['BBH_components'] = 12
+		self.format_info['BBH_components'] = {'D':12,
+				'mass_format': 'BBH_components', 'spin_format': 'BBH_components',
+				'eccentricity_format': 'BBH_components', 'angle_format': 'BBH_components',
+				'e': True, 'meanano':True,
+				'iota': True,'phi': True}
+		
 		self.MAX_SPIN = 0.999 #defining the constant maximum value for the spin (used for any check that's being done)
 		self.MAX_Q = 100.
 		
 		self.constraints = {'M':(0.,np.inf), 'logM':(-np.inf,np.inf), 'q': (1./self.MAX_Q, self.MAX_Q),
 				'Mc':(0., np.inf), 'eta':(1./self.MAX_Q, 0.25),
 				'mass1':(0, np.inf), 'mass2':(0, np.inf),
 				'chi': (-self.MAX_SPIN, self.MAX_SPIN), 
@@ -183,14 +192,44 @@
 				#At the moment, mbank cannot cover the negative s1x region in for spin format s1xz
 				's1': (0., self.MAX_SPIN), 's2': (0., self.MAX_SPIN),
 				'theta1':(-np.pi, np.pi), 'phi1':(-np.pi, np.pi),
 				'theta2':(-np.pi, np.pi), 'phi1':(-np.pi, np.pi),
 				'iota': (0.,np.pi), 'phi': (-np.inf, np.inf),
 				'e': (0., 1.), 'meanano': (0, 1.)
 				} #allowed ranges for each label
+		
+			#Adding a set of functions to extract some values from the BBH components
+		self.theta_getter = {
+			'mass1': lambda x: x[:,0],
+			'mass2': lambda x: x[:,1],
+			'M': lambda x: x[:,0] + x[:,1],
+			'logM': lambda x: np.log10(x[:,0] + x[:,1]),
+			'q': lambda x: np.maximum(x[:,1] / x[:,0], x[:,0] / x[:,1]),
+			'Mc': lambda x: (x[:,0] + x[:,1])*np.power(np.divide(x[:,1] * x[:,0], np.square(x[:,0] + x[:,1])), 3./5.),
+			'eta': lambda x: np.divide(x[:,1] * x[:,0], np.square(x[:,0] + x[:,1]) ),
+			'chi': lambda x: (x[:,0]*x[:,4] + x[:,7]*x[:,1])/(x[:,0]+x[:,1]),
+			's1z': lambda x: x[:,4],
+			's2z': lambda x: x[:,7],
+			's1': lambda x: np.linalg.norm(x[:,2:5], axis =1),
+			'theta1': lambda x: np.arctan2(np.linalg.norm(x[:,[2,3]], axis =1)*np.sign(x[:,2]), x[:,4]),
+			'phi1': lambda x: np.arctan(x[:,3]/(x[:,2]+1e-20)),
+			's2': lambda x: np.linalg.norm(x[:, 5:8], axis =1),
+			'theta2': lambda x: np.arctan2(np.linalg.norm(x[:,[5,6]], axis = -1)*np.sign(x[:,5]), x[:,7]),
+			'phi2': lambda x: np.arctan(x[:,6]/(x[:,5]+1e-20)),
+			'e': lambda x: x[:,8],
+			'meanano': lambda x: x[:,9],
+			'iota': lambda x: x[:,10],
+			'phi': lambda x: x[:,11]
+		}
+		for v, tg in self.theta_getter.items():
+			setattr(self, 'get_'+v, tg)
+		
+		self.comp_getter = [
+		'm1', 'm2', 's1x', 's1y', 's1z', 's2x', 's2y', 's2z', 'e', 'meanano', 'iota', 'phi'
+		] #does this obj make sense?
 				
 		
 		return
 
 	def is_theta_ok(self, theta, variable_format, raise_error = False):
 		"""
 		Given a value of theta, it checks whether it is an acceptable value for the given spin format.
@@ -268,15 +307,15 @@
 		elif self.format_info[variable_format]['spin_format'] == 's1xyz':
 			pass #chiP is always intended to be on the largest BH (pay attention to this)
 		elif self.format_info[variable_format]['spin_format'] == 's1xz_s2z':
 			theta[ids,3], theta[ids,4] = theta[ids,4], theta[ids,3] #switching spins
 		elif self.format_info[variable_format]['spin_format'] == 's1xyz_s2z':
 			theta[ids,4], theta[ids,5] = theta[ids,5], theta[ids,4] #switching spins
 		elif self.format_info[variable_format]['spin_format'] == 'fullspins':
-			theta[ids,[2,3,4]], theta[ids,[5,6,7]] =  theta[ids,[5,6,7]], theta[ids,[2,3,4]] #switching spins
+			theta[ids,2:5], theta[ids,5:8] =  theta[ids,5:8], theta[ids,2:5] #switching spins
 
 
 		if squeeze: theta = np.squeeze(theta)
 		return theta
 	
 	def labels(self, variable_format, latex = False):
 		"""
@@ -295,14 +334,19 @@
 			List of labels for the parmams in the BBH (each a str)
 		
 		latex: bool
 			Whether the labels should be in latex
 		"""
 		assert variable_format in self.valid_formats, "Wrong variable format given"
 		
+		if variable_format == 'BBH_components':
+			if latex: labels = [r'$m_1$', r'$m_2$', r'$s_{1x}$', r'$s_{1y}$', r'$s_{1z}$', r'$s_{2x}$', r'$s_{2y}$', r'$s_{2z}$', r'$e$', r'$meanano$', r'$\iota$', r'$\phi$']
+			else:  labels = ['m1', 'm2', 's1x', 's1y', 's1z', 's2x', 's2y', 's2z', 'e', 'meanano', 'iota', 'phi']
+			return labels
+		
 		if self.format_info[variable_format]['mass_format'] == 'm1m2':
 			if latex: labels = [r'$m_1$', r'$m_2$']
 			else: labels = ['mass1', 'mass2']
 		elif self.format_info[variable_format]['mass_format'] == 'Mq':
 			if latex: labels = [r'$M$', r'$q$']
 			else: labels = ['M', 'q']
 		elif self.format_info[variable_format]['mass_format'] == 'logMq':
@@ -333,15 +377,15 @@
 			if latex: labels.extend([r'$s_{1}$', r'$\theta_1$', r'$s_{2z}$'])
 			else: labels.extend(['s1', 'theta1', 's2z'])
 		elif self.format_info[variable_format]['spin_format'] == 's1xyz_s2z':
 			if latex: labels.extend([r'$s_{1}$', r'$\theta_1$', r'$\phi_1$', r'$s_{2z}$'])
 			else: labels.extend(['s1','theta1', 'phi1', 's2z'])
 		elif self.format_info[variable_format]['spin_format'] == 'fullspins':
 			if latex: labels.extend([r'$s_{1}$', r'$\theta_1$', r'$\phi_1$', r'$s_{2}$', r'$\theta_2$', r'$\phi_2$'])
-			else: labels.extend(['s1','theta1', 'phi1', 's2z', 'theta2', 'phi2'])
+			else: labels.extend(['s1','theta1', 'phi1', 's2', 'theta2', 'phi2'])
 		
 		if self.format_info[variable_format]['e'] and latex: labels.append(r'$e$')
 		if self.format_info[variable_format]['e'] and not latex: labels.append('e')
 
 		if self.format_info[variable_format]['meanano'] and latex: labels.append(r'$meanano$')
 		if self.format_info[variable_format]['meanano'] and not latex: labels.append('meanano')
 		
@@ -408,15 +452,15 @@
 		
 		Parameters
 		----------
 		
 		BBH_components: :class:`~numpy:numpy.ndarray`
 			shape: (N,12)/(12,) -
 			Parameters of the BBHs.
-			Each row should be: m1, m2, s1x, s1y, s1z, s2x, s2y, s2z, e, meanano, iota, phi
+			The columns of the array should be: `m1, m2, s1x, s1y, s1z, s2x, s2y, s2z, e, meanano, iota, phi`
 
 		variable_format: str
 			How to handle the BBH variables.
 		
 		Returns
 		-------
 			theta: :class:`~numpy:numpy.ndarray`
@@ -424,112 +468,56 @@
 				Components of the BBH in the format suitable for the bank.
 				The dimensionality depends on variable_format
 		"""
 		BBH_components, squeeze = self._check_theta_and_format(BBH_components, variable_format)
 		
 		assert BBH_components.shape[1] == 12, "The number of BBH parameter is not enough. Expected 12 [m1, m2, s1x, s1y, s1z, s2x, s2y, s2z, e, meanano, iota, phi], given {}".format(BBH_components.shape[1])
 		
-		if self.format_info[variable_format]['mass_format'] == 'm1m2':
-			theta = [BBH_components[:,0], BBH_components[:,1]]
-		elif self.format_info[variable_format]['mass_format'] == 'Mq':
-			q = np.maximum(BBH_components[:,1] / BBH_components[:,0], BBH_components[:,0] / BBH_components[:,1])
-			theta = [BBH_components[:,0] + BBH_components[:,1], q]
-		elif self.format_info[variable_format]['mass_format'] == 'logMq':
-			q = np.maximum(BBH_components[:,1] / BBH_components[:,0], BBH_components[:,0] / BBH_components[:,1])
-			theta = [np.log10(BBH_components[:,0] + BBH_components[:,1]), q]
-		elif self.format_info[variable_format]['mass_format'] == 'mceta':
-			eta = np.divide(BBH_components[:,1] * BBH_components[:,0], np.square(BBH_components[:,0] + BBH_components[:,1]) )
-			theta = [(BBH_components[:,0] + BBH_components[:,1])*np.power(eta, 3./5.), eta]
-
-			#starting a case swich
-		if self.format_info[variable_format]['spin_format'] =='nonspinning':
-			pass
-		elif self.format_info[variable_format]['spin_format'] == 'chi':
-			chi = (BBH_components[:,0]*BBH_components[:,4] + BBH_components[:,7]*BBH_components[:,1])/ \
-					(BBH_components[:,0]+BBH_components[:,1])
-			theta.append(chi)
-		elif self.format_info[variable_format]['spin_format'] == 's1z':
-			theta.append(BBH_components[:,4])
-		elif self.format_info[variable_format]['spin_format'] == 's1z_s2z':
-			theta.append(BBH_components[:,4])
-			theta.append(BBH_components[:,7])
-		elif self.format_info[variable_format]['spin_format'] == 's1xz':
-			s1 = np.linalg.norm(BBH_components[:,2:5], axis =1) #(N,)
-			theta1 = np.arctan2(BBH_components[:,2], BBH_components[:,4])
-			theta.extend([s1, theta1])
-		elif self.format_info[variable_format]['spin_format'] == 's1xyz':
-			s1 = np.linalg.norm(BBH_components[:,2:5], axis =1) #(N,)
-			theta1 = np.arccos(BBH_components[:,4]/s1)
-			phi1 = np.arctan2(BBH_components[:,3], BBH_components[:,2])
-			theta.extend([s1, theta1, phi1])
-		elif self.format_info[variable_format]['spin_format'] == 's1xz_s2z':
-			s1 = np.linalg.norm(BBH_components[:,2:5], axis =1)+1e-10 #(N,)
-			theta1 = np.arccos(BBH_components[:,4]/s1)
-			theta.append(s1)
-			theta.append(theta1)
-			theta.append(BBH_components[:,7])
-		elif self.format_info[variable_format]['spin_format'] == 's1xyz_s2z':
-			s1 = np.linalg.norm(BBH_components[:,2:5], axis =1)+1e-10 #(N,)
-			theta1 = np.arccos(BBH_components[:,4]/s1)
-			phi1 = np.arctan2(BBH_components[:,3], BBH_components[:,2])
-			theta.extend([s1, theta1, phi1, BBH_components[:,7]])
-		elif self.format_info[variable_format]['spin_format'] == 'fullspins':
-			s1 = np.maximum(np.linalg.norm(BBH_components[:,2:5], axis =1), 1e-20) #(N,)
-			theta1 = np.arccos(BBH_components[:,4]/s1)
-			phi1 = np.arctan2(BBH_components[:,3], BBH_components[:,2])
-			s2 = np.maximum(np.linalg.norm(BBH_components[:, 5:8], axis =1), 1e-20) #(N,)
-			theta2 = np.arccos(BBH_components[:,7]/s2)
-			phi2 = np.arctan2(BBH_components[:,6], BBH_components[:,5])
-			theta.extend([s1, theta1, phi1, s2, theta2, phi2])
+		if variable_format == 'BBH_components':
+			theta = [*BBH_components.T]
 		else:
-			raise RuntimeError("Wrong setting for variable_format")
-			
-			#dealing with eccentricity
-		if self.format_info[variable_format]['e']:
-			theta.append(BBH_components[:,8])
-		if self.format_info[variable_format]['meanano']:
-			theta.append(BBH_components[:,9])
-		
-			#dealing with angles
-		if self.format_info[variable_format]['iota']:
-			theta.append(BBH_components[:,10])
-		if self.format_info[variable_format]['phi']:
-			theta.append(BBH_components[:,11])
-		
+			theta = [self.theta_getter[l](BBH_components) for l in self.labels(variable_format)]
+
 		theta = np.column_stack(theta)
 		
 		if squeeze: theta = np.squeeze(theta)
 		
 		return theta
 
 
 	def get_BBH_components(self, theta, variable_format):
 		"""
 		Given ``theta``, it returns the components of the BBH suitable for lal
 		
 		Parameters
 		----------
 		
-		theta: :class:`~numpy:numpy.ndarray` (N,D)
+		theta: :class:`~numpy:numpy.ndarray`
+			shape: (N,12) -
 			Parameters of the BBHs. The dimensionality depends on variable_format
 
 		variable_format: str
 			How to handle the BBH variables.
 		
 		Returns
 		-------
 		
-		m1, m2, s1x, s1y, s1z, s2x, s2y, s2z, e, meanano iota, phi: :class:`~numpy:numpy.ndarray`
-			Components of the BBH in the std parametrization.
-			Each has shape (N,)
+		BBH_components: :class:`~numpy:numpy.ndarray`
+			shape: (N,12) -
+			Components of the BBH.
+			Columns of the array are `m1, m2, s1x, s1y, s1z, s2x, s2y, s2z, e, meanano iota, phi`.
 		"""
 		theta, squeeze = self._check_theta_and_format(theta, variable_format)
 		
 		assert theta.shape[1]==self.D(variable_format), "The number of BBH parameter doesn't fit into the given variable format. Expected {}, given {}".format(self.D(variable_format), theta.shape[1])
 		
+		if variable_format == 'BBH_components':
+			if squeeze: return np.squeeze(theta)
+			return theta
+		
 			#setting the masses
 		if self.format_info[variable_format]['mass_format'] == 'm1m2':
 			m1, m2 = theta[:,0], theta[:,1]
 		elif self.format_info[variable_format]['mass_format'] == 'Mq':
 			m1, m2 = theta[:,0]*theta[:,1]/(1+theta[:,1]), theta[:,0]/(1+theta[:,1])
 			m1, m2 = np.maximum(m1, m2), np.minimum(m1, m2) #this is to make sure that m1>m2, also if q is less than 1
 		elif self.format_info[variable_format]['mass_format'] == 'logMq':
@@ -563,16 +551,18 @@
 		elif self.format_info[variable_format]['spin_format'] == 's1xyz':
 			s1x, s1y, s1z = theta[:,2]*np.sin(theta[:,3])*np.cos(theta[:,4]), theta[:,2]*np.sin(theta[:,3])*np.sin(theta[:,4]), theta[:,2]*np.cos(theta[:,3])
 		elif self.format_info[variable_format]['spin_format'] == 's1xz_s2z':
 			s1x, s1z, s2z = theta[:,2]*np.sin(theta[:,3]), theta[:,2]*np.cos(theta[:,3]), theta[:,4]
 		elif self.format_info[variable_format]['spin_format'] == 's1xyz_s2z':
 			s1x, s1y, s1z, s2z = theta[:,2]*np.sin(theta[:,3])*np.cos(theta[:,4]), theta[:,2]*np.sin(theta[:,3])*np.sin(theta[:,4]), theta[:,2]*np.cos(theta[:,3]), theta[:,5]
 		elif self.format_info[variable_format]['spin_format'] == 'fullspins':
-			s1x, s1y, s1z = theta[:,2]*np.sin(theta[:,3])*np.cos(theta[:,4]), theta[:,2]*np.sin(theta[:,3])*np.sin(theta[:,4]), theta[:,2]*np.cos(theta[:,3])
-			s2x, s2y, s2z = theta[:,5]*np.sin(theta[:,6])*np.cos(theta[:,7]), theta[:,5]*np.sin(theta[:,6])*np.sin(theta[:,7]), theta[:,5]*np.cos(theta[:,6])
+			s1x, s1y = theta[:,2]*np.sin(theta[:,3])*np.cos(theta[:,4]), theta[:,2]*np.sin(theta[:,3])*np.sin(theta[:,4])
+			s1z = theta[:,2]*np.cos(theta[:,3])
+			s2x, s2y = theta[:,5]*np.sin(theta[:,6])*np.cos(theta[:,7]), theta[:,5]*np.sin(theta[:,6])*np.sin(theta[:,7])
+			s2z = theta[:,5]*np.cos(theta[:,6])
 
 			#dealing with angles and eccentricity (tricky!!)
 		assign_var =  [self.format_info[variable_format]['e'], self.format_info[variable_format]['meanano'],
 				self.format_info[variable_format]['iota'], self.format_info[variable_format]['phi']]
 		N_to_assign = sum(assign_var)
 		
 		vars_to_assign = []
@@ -590,19 +580,19 @@
 		def set_zero_spin(s):
 			ids_ = np.where(np.abs(s)<1e-10)[0]
 			if len(ids_)>0: s[ids_] = 0.
 			return s
 		s1x, s1y, s1z = set_zero_spin(s1x), set_zero_spin(s1y), set_zero_spin(s1z)
 		s2x, s2y, s2z = set_zero_spin(s2x), set_zero_spin(s2y), set_zero_spin(s2z)
 		
+		BBH_comps = np.stack([m1, m2, s1x, s1y, s1z, s2x, s2y, s2z, e, meanano, iota, phi], axis = 1)
 		
-		if squeeze:
-			m1, m2, s1x, s1y, s1z, s2x, s2y, s2z,  e, meanano, iota, phi = m1[0], m2[0], s1x[0], s1y[0], s1z[0], s2x[0], s2y[0], s2z[0], e[0], meanano[0], iota[0], phi[0]
+		if squeeze:	BBH_comps = np.squeeze(BBH_comps)
 		
-		return m1, m2, s1x, s1y, s1z, s2x, s2y, s2z, e, meanano, iota, phi
+		return BBH_comps
 	
 	def get_mchirp(self, theta, variable_format):
 		"""
 		Given theta, it returns the chirp mass
 
 		Parameters
 		----------
@@ -1562,14 +1552,15 @@
 			samples = [	gen.uniform(self[t_id][0].mins, self[t_id][0].maxes, (c, D) )
 						for t_id, c in zip(tiles_rand_id, counts)]
 		samples = np.concatenate(samples, axis = 0, dtype = dtype)
 
 		if tile_id:
 			tile_id_vector = np.concatenate([np.full(c, t_id) for t_id, c in zip(tiles_rand_id, counts)])
 			return samples, tile_id_vector
+		np.random.shuffle(samples)
 		return samples
 
 
 	def split_tiling(self, d, split):
 		"""
 		Produce two tilings by splitting the parameter space along dimension `d`. The splitting is done by the threshold `split`.
 		It is roughly the equivalent for a tiling to the ``split`` method of :class:`~scipy.spatial.Rectangle`.
```

### Comparing `gw-mbank-0.2.0/mbank/metric.py` & `gw-mbank-0.3.1/mbank/metric.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 import lal 
 import lalsimulation as lalsim
 
 import warnings
 
 from .handlers import variable_handler
-from .utils import project_metric
+from .utils import project_metric, get_projected_metric
 
 	#TODO: understand whether it's a good idea to use anycache
 #from anycache import anycache
 
 #############DEBUG LINE PROFILING
 try:
 	from line_profiler import LineProfiler
@@ -97,14 +97,15 @@
 		"""
 		self.var_handler = variable_handler() #this obj is to keep in a single place all the possible spin manipulations that may be required
 
 		self.set_approximant(approx)
 		self.set_variable_format(variable_format)
 		
 		self.f_min = float(f_min)
+		if isinstance(f_max, str): f_max = float(f_max)
 		
 		if not isinstance(PSD, tuple):
 			raise ValueError("Wrong format for the PSD. Expected a tuple of np.ndarray, got {}".format(type(PSD)))
 
 		#####Tackling the PSD
 		#FIXME: do you really need to store the PSD and the frequency grid all the way to zero? It seems like an useless waste of memory/computational time
 		#TODO: allow for the PSD to be None!
@@ -210,41 +211,74 @@
 		
 		vol_element : :class:`~numpy:numpy.ndarray`
 			shape: (N,) -
 			Volume element of the metric for the given input
 			
 		"""
 		return np.sqrt(np.abs(np.linalg.det(self.get_metric(theta, overlap = overlap)))) #(N,)
+
+	def get_hpc(self, theta):
+		"""
+		Returns the real part of the overlap between plus and cross polarization:
+		
+		.. math::
+		
+			h_{+\\times} = \Re \int df \\frac{\\tilde{h}_+(f) \\tilde{h}_\\times^*(f)}{S_n(f)}
+		
+		It is a good measurement of the amount of precession/HM present in a signal; for a non-precessing signal: :math:`h_{+\\times} = 0` 
+		
+		Parameters
+		----------
+		
+		theta: :class:`~numpy:numpy.ndarray`
+			shape: (N,D) -
+			Parameters of the BBHs. The dimensionality depends on the variable format set for the metric
+
+		Returns
+		-------
+		
+		h_pc : :class:`~numpy:numpy.ndarray`
+			shape: (N,) -
+			Overlap between plus and cross components
+			
+		"""
+		hp, hc = self.get_WF(theta, approx = None, plus_cross = True)
+		
+		hp_W = (hp/np.sqrt(self.PSD)) #whithened WF
+		hc_W = (hc/np.sqrt(self.PSD)) #whithened WF
+		
+		hpc = np.vdot(hp_W, hc_W)/np.sqrt(np.vdot(hp_W,hp_W)*np.vdot(hc_W,hc_W))
+		
+		return hpc.real
 	
-	def get_metric_determinant(self, theta, overlap = False):
+	def get_metric_determinant(self, theta, **kwargs):
 		"""
 		Returns the metric determinant
 		
 		Parameters
 		----------
 		
 		theta: :class:`~numpy:numpy.ndarray`
 			shape: (N,D) -
 			Parameters of the BBHs. The dimensionality depends on the variable format set for the metric
 		
-		overlap: bool
-			Whether to compute the metric based on the local expansion of the overlap rather than of the match
-			In this context the match is the overlap maximized over time
+		**kwargs:
+			Any argument to pass to :func:`get_metric`
 
 		Returns
 		-------
 		
 		det : :class:`~numpy:numpy.ndarray`
 			shape: (N,) -
 			Determinant of the metric for the given input
 			
 		"""
-		return np.linalg.det(self.get_metric(theta, overlap = overlap)) #(N,)
+		return np.linalg.det(self.get_metric(theta, **kwargs)) #(N,)
 
-	def log_pdf(self, theta, boundaries = None):
+	def log_pdf(self, theta, boundaries = None, **kwargs):
 		"""
 		Returns the logarithm log(pdf) of the probability distribution function we want to sample from:
 		.. math::
 		
 			pdf = p(theta) ~ sqrt(|M(theta)|)
 
 		imposing the boundaries
@@ -257,14 +291,17 @@
 			parameters of the BBHs. The dimensionality depends on the variable format set for the metric
 		
 		boundaries: :class:`~numpy:numpy.ndarray`
 			shape: (2,D)
 			An optional array with the boundaries for the model. If a point is asked below the limit, -10000000 is returned
 			Lower limit is boundaries[0,:] while upper limits is boundaries[1,:]
 			If None, no boundaries are implemented
+				
+		**kwargs:
+			Any argument to pass to :func:`get_metric`
 		
 		Returns
 		-------
 		
 		log_pdf : :class:`~numpy:numpy.ndarray`
 			shape: (N,) -
 			Logarithm of the pdf, ready to use for sampling
@@ -279,21 +316,21 @@
 		
 		if isinstance(boundaries,np.ndarray):
 			if boundaries.shape != (2,self.D):
 				raise ValueError("Wrong shape of boundaries given: expected (2,{}), given {}".format(self.D, boundaries.shape))
 			
 			ids_ok = np.logical_and(np.all(theta > boundaries[0,:], axis =1), np.all(theta < boundaries[1,:], axis = 1)) #(N,)
 		else:
-			ids_ok = np.full((theta.shape[0],), True)
+			ids_ok = range(theta.shape[0])
 			
 		
 		res = np.zeros((theta.shape[0],)) -10000000
 		
 		if np.any(ids_ok):
-			det = self.get_metric_determinant(theta[ids_ok,:])
+			det = self.get_metric_determinant(theta[ids_ok,:], **kwargs)
 			det = np.log(np.abs(det))*0.5 #log(sqrt(|det|))
 			res[ids_ok] = det
 		
 		return res
 	
 	def log_pdf_gauss(self, theta, boundaries = None):
 		return -0.5*np.sum(np.square(theta-10.), axis =-1) #DEBUG!!!!!
@@ -473,15 +510,15 @@
 			lal_approx = lalsim.SimInspiralGetApproximantFromString(approx) #getting the approximant
 		except RuntimeError:
 			raise RuntimeError("Given approximant not supported by lal")
 
 			#generating the WF
 		if not lalsim.SimInspiralImplementedFDApproximants(lal_approx):
 			raise RuntimeError("Approximant {} is TD: only FD approximants are supported".format(approx)) #must be FD approximant
-		m1, m2, s1x, s1y, s1z, s2x, s2y, s2z, e, meanano, iota, phi = self.var_handler.get_BBH_components(theta, self.variable_format)
+		m1, m2, s1x, s1y, s1z, s2x, s2y, s2z, e, meanano, iota, phi = self.var_handler.get_BBH_components(theta, self.variable_format).T
 		#print("mbank pars - {}: ".format(self.variable_format),m1, m2, s1x, s1y, s1z, s2x, s2y, s2z, iota, phi, e, meanano) #DEBUG
 		#warnings.warn("Set non-zero spins!"); s1z = s1z + 0.4; s2z = s2z -0.7
 
 		try:
 			hptilde, hctilde = lalsim.SimInspiralChooseFDWaveform(m1*lalsim.lal.MSUN_SI,
                         m2*lalsim.lal.MSUN_SI,
                         float(s1x), float(s1y), float(s1z),
@@ -582,42 +619,61 @@
 		
 		overlap: bool
 			Whether to compute the metric based on the local expansion of the overlap rather than of the match
 			In this context the match is the overlap maximized over time
 
 		metric_type: str
 			How to compute the metric. Available options are:
-				- 'hessian': Computes the hessian (calls ``cbc_metric.get_hessian``)
-				- 'numerical_hessian': computes the numerical hessian with finite difference methods (uses package ``numdifftools`` and calls ``cbc_metric.get_numerical_hessian``)
-				- 'WRITEME!'
+				- `hessian`: Computes the hessian of the standard match (calls :func:`get_hessian`)
+				- `numerical_hessian`: computes the numerical hessian with finite difference methods using the standard match (uses package ``numdifftools`` and calls :func:`get_numerical_hessian`)
+				- `symphony`: Computes the hessian of the symphony match (calls :func:`get_hessian_symphony`)
+				- `numerical_symphony`: computes the numerical hessian with finite difference methods using the symphony match (uses package ``numdifftools`` and calls :func:`get_numerical_hessian`)
+				- `parabolic_fit_hessian`: it updates the eigenvalues of the metric by doing a "parabolic fit" along each eigen-direction (calls :func:`get_parabolic_fit_hessian`) - *This method experimental and not validated!*
+			
+			There are a number of other methods but we don't guarantee on their performance: you shouldn't use, unless you really know what you're doing.
 
 		Returns
 		-------
 		
 		metric : :class:`~numpy:numpy.ndarray`
 			shape: (N,D,D)/(D,D) -
 			Array containing the metric in the given parameters
 			
 		"""
 		#TODO: allow to implement a custom metric function...
 		metric_dict ={
 			'hessian': self.get_hessian,
-			'symmetrized': self.get_hessian_symmetrized_plus_cross,
-			'projected_hessian': self.get_projected_hessian,
+			'symphony': self.get_hessian_symphony,
 			'numerical_hessian': self.get_numerical_hessian,
+			'numerical_symphony': self.get_numerical_hessian,
+			'projected_hessian': self.get_projected_hessian,
 			'parabolic_fit_hessian': self.get_parabolic_fit_hessian,
 			'block_diagonal_hessian': self.get_block_diagonal_hessian,
 			'fisher':self.get_fisher_matrix
 			}
 		
 		if metric_type not in metric_dict.keys():
 			msg = "Unknown metric_type '{}' given. It must be one of {}".format(metric_type, list(metric_dict.keys()))
 			raise ValueError(msg)
 		
-		return metric_dict[metric_type](theta, overlap = overlap, **kwargs)
+		if metric_type == 'numerical_symphony':
+			kwargs['symphony'] = True
+			kwargs['antenna_patterns'] = None
+		
+			###
+			#Being sustainable and doing things in batch
+		N, N_batch = theta.shape[0], 100
+		metric_list = []
+		
+		for i in range(0, N, N_batch):
+			metric_list.append(
+				metric_dict[metric_type](theta[i:i+N_batch], overlap = overlap, **kwargs)
+			)
+
+		return np.concatenate(metric_list, axis = 0)
 
 	def get_projected_hessian(self, theta, overlap = False,  min_eig = 1e-3, order = None, epsilon = 1e-5):
 		"""
 		Returns the projected Hessian matrix. The projections happens on the subspace spanned the eigenvectors with eigenvalues larger than ``min_eig``.
 		
 		See ``mbank.utils.get_projected_metric`` for more information.
 		
@@ -695,15 +751,15 @@
 				metric[i, j,2:] = 0.
 				metric[i, 2:,j] = 0.
 
 		if squeeze: return metric[0,...]
 		else: return metric
 
 
-	def get_parabolic_fit_hessian(self, theta, overlap = False, target_match = 0.9, N_epsilon_points = 7, log_epsilon_range = (-4, 1), full_output = False, **kwargs):
+	def get_parabolic_fit_hessian(self, theta, overlap = False, symphony = False, target_match = 0.9, N_epsilon_points = 7, log_epsilon_range = (-4, 1), antenna_patterns = None, full_output = False, **kwargs):
 		"""
 		Returns the hessian with the adjusted eigenvalues.
 		The eigenvalues are adjusted by fitting a parabola on the match along each direction.
 		
 		Parameters
 		----------
 		
@@ -711,26 +767,32 @@
 			shape: (N,D)/(D,) -
 			Parameters of the BBHs. The dimensionality depends on self.variable_format
 		
 		overlap: bool
 			Whether to compute the metric based on the local expansion of the overlap rather than of the match
 			In this context the match is the overlap maximized over time
 
+		symphony: bool
+			Whether to compute the metric approximation for the symphony match
+
 		target_match: float
 			Target match for the eigenvalues fixing. Maximum range for the optimization problem
 		
 		N_epsilon_points: int
 			Number of points to evaluate the match along each dimension
 		
 		log_epsilon_range: tuple
 			Tuple of floats. They represent the range in the log10(epsilon) to explore
+
+		antenna_patterns: tuple
+			Tuple of float/:class:`~numpy:numpy.ndarray` (:math:`F_+`, :math:`F_\\times`) for the two antenna patterns.
+			If given, it is used to build the signal :math:`s`, starting from :math:`h(\\theta_1)`; if ``None``, :math:`s = h_+(\\theta_\\mathrm{template})`. See :func:`get_antenna_patterns`.
 		
 		full_output: bool
 			Whether to return (together with the metric) a list of array, one for each dimension. The arrays have rows ``(step, match)``
-		
 
 		Returns
 		-------
 		
 		metric : :class:`~numpy:numpy.ndarray`
 			shape: (N,D,D)/(D,D) -
 			Array containing the metric in the given parameters
@@ -745,21 +807,28 @@
 		"""
 		theta = np.asarray(theta)
 		squeeze = False
 		if theta.ndim ==1:
 			theta = theta[None,:]
 			squeeze = True
 		
-		metric_hessian = self.get_hessian(theta, overlap = overlap, order = None) #(N,D,D)
+		if antenna_patterns is None:
+			antenna_patterns = (1,0)
+		assert isinstance(antenna_patterns, (tuple, list, np.ndarray)), "Antenna pattern must be a tuple"
+		F_p, F_c = antenna_patterns
+		
+		metric_hessian = self.get_hessian_symphony(theta, overlap = overlap, order = None) #(N,D,D)
 		#metric_hessian = self.get_block_diagonal_hessian(theta, overlap = overlap, order = None); warnings.warn("Using block diagonal hessian")#(N,D,D)
 		parabolae = []
 		metric = []
 
 		for center, metric_ in zip(theta, metric_hessian):
-			WF1 = self.get_WF(center, self.approx)
+			WF1_p, WF1_c = self.get_WF(center, self.approx, plus_cross = True)
+				#Building the signal
+			WF1 = WF1_p *F_p + WF1_c*F_c
 			eigvals, eigvecs = np.linalg.eig(metric_)
 			
 			parabolae_ = []
 			new_eigvals = []
 			
 				#recomputing the eigenvalues by parabolic fitting
 			for d, eigvec in enumerate(eigvecs.T):
@@ -770,80 +839,100 @@
 				
 				for epsilon, s in itertools.product(epsilon_list,[+1,-1]):
 					id_s = (s+1)//2
 					if max_epsilon[id_s] < epsilon: continue #this is to make sure not to explore weird regions
 					
 					theta_ = np.array(center)+s*epsilon*eigvec
 					if self.var_handler.is_theta_ok(theta_, self.variable_format):
-						WF2 = self.get_WF(theta_, self.approx)
-						temp_match = self.WF_match(WF1, WF2, overlap = overlap) #Why was it set to True??
+						WF2_p, WF2_c = self.get_WF(theta_, self.approx, plus_cross = True)
+						if symphony:
+							temp_match = self.WF_symphony_match(WF1, WF2_p, WF2_c, overlap = overlap)
+						else:
+							temp_match = self.WF_match(WF1, WF2_p, overlap = overlap)
 						if temp_match >= target_match:
 							parabola_list_d.append((s*epsilon, temp_match))
 						else:
 							max_epsilon[id_s] = epsilon
 					else:
 						max_epsilon[id_s] = epsilon
 
 				parabolae_.append(np.array(parabola_list_d))
 				p = np.polyfit(parabolae_[-1][:,0]**2, parabolae_[-1][:,1], 1)[0] #parabolic fit
 				#p = np.polyfit(parabolae_[-1][:,0]**2, parabolae_[-1][:,1], 2)[1] #quartic fit
-				new_eigvals.append(np.abs(p)) #abs is dangerous, as if you have a negative eigenvalues, you wouldn't note
+				new_eigvals.append(np.abs(p)) #abs is dangerous, since if you have a negative eigenvalues you wouldn't note
 		
 			parabolae.append(parabolae_)
 			metric.append(np.linalg.multi_dot([eigvecs, np.diag(new_eigvals), eigvecs.T]))
 		
 		metric = np.stack(metric, axis = 0)
 		if squeeze:
 			metric = np.squeeze(metric)
 			parabolae = parabolae[0]
 			metric_hessian = metric_hessian[0]
 		
 		if full_output: return metric, parabolae, metric_hessian
 		else: return metric
 		
 	
-	def get_numerical_hessian(self, theta, overlap = False, epsilon = 1e-6, target_match = 0.97):
+	def get_numerical_hessian(self, theta, overlap = False, symphony = False, epsilon = 1e-6, target_match = 0.97, antenna_patterns = None):
 		"""
-		Returns the Hessian matrix, obtained by finite difference differentiation. Within numerical erorrs, it should reproduce `cbc_metric.get_hessian_metric`.
-		This function is slower and most prone to numerical errors than its counterparts, based on waveform gradients. For this reason it is mostly intended as a check of the recommended function `cbc_metric.get_hessian_metric`.
+		Returns the Hessian matrix, obtained by finite difference differentiation.
+		Within numerical erorrs, it should reproduce :func:`get_hessian` or :func:`get_hessian_symphony`, depending on the ``symphony`` option.
+		This function is slower and most prone to numerical errors than its counterparts, based on waveform gradients. For this reason it is mostly intended as a check of the recommended function :func:`get_hessian` and :func:`get_hessian_symphony`.
 		In particular the step size epsilon must be tuned carefully and the results are really sensible on this choice.
-		Uses package ``numdifftools``, not among the dependencies.
+		Uses package ``numdifftools``: it not among the dependencies, so it must be installed separately!
 		
 		Parameters
 		----------
 		
 		theta: :class:`~numpy:numpy.ndarray`
 			shape: (N,D)/(D,) -
 			Parameters of the BBHs. The dimensionality depends on self.variable_format
 		
 		overlap: bool
 			Whether to compute the metric based on the local expansion of the overlap rather than of the match
 			In this context the match is the overlap maximized over time
 
+		symphony: bool
+			Whether to compute the metric approximation for the symphony match
+
 		epsilon: float
 			Size of the jump for the finite difference scheme.
 			If `None`, it will be authomatically computed.
 		
 		target_match: float
 			Target match for the authomatic epsilon computation. Only applies is epsilon is None.
 		
+		antenna_patterns: tuple
+			Tuple of float/:class:`~numpy:numpy.ndarray` (:math:`F_+`, :math:`F_\\times`) for the two antenna patterns.
+			If given, it is used to build the signal :math:`s`, starting from :math:`h(\\theta_1)`; if ``None``, :math:`s = h_+(\\theta_\\mathrm{template})`. See :func:`get_antenna_patterns`.
+		
 		Returns
 		-------
 		
 		metric : :class:`~numpy:numpy.ndarray`
 			shape: (N,D,D)/(D,D) -
 			Array containing the metric Hessian in the given parameters
 		"""
 		##
 		# Defining a match functions
 		
 		def match_t(x):
+			#WF2 is the "template" and it is in global scope
 			t, theta_ = x[0], x[1:]
-			WF2 = self.get_WF(theta_, self.approx)*np.exp(-1j*2*np.pi*self.f_grid*t)
-			return self.WF_match(WF1, WF2, False) #WF1 is in global scope
+			WF1_p, WF1_c = self.get_WF(theta_, self.approx, plus_cross = True)
+			WF1 = WF1_p *F_p + WF1_c*F_c
+			WF1 *= np.exp(-1j*2*np.pi*self.f_grid*t)
+			if symphony:
+				return self.WF_symphony_match(WF1, WF2_p, WF2_c, overlap = False)
+				#return self.WF_symphony_match(WF2_p *F_p + WF2_c*F_c,
+				#		WF1_p*np.exp(-1j*2*np.pi*self.f_grid*t),
+				#		WF1_c*np.exp(-1j*2*np.pi*self.f_grid*t), overlap = False)
+			else:
+				return self.WF_match(WF1, WF2_p, overlap = False) 
 		
 		###
 		# Loss function
 		def loss_epsilon(log10_epsilon, axis, center):
 			"Loss function to compute the proper value of epsilon"
 			theta_p, theta_m = np.array(center), np.array(center)
 			theta_p[axis] = center[axis]+10**log10_epsilon
@@ -870,24 +959,30 @@
 		theta = np.asarray(theta)
 		squeeze = False
 		if theta.ndim ==1:
 			theta = theta[None,:]
 			squeeze = True
 
 		##		
-		# Dealing with epsilon
+		# Dealing with epsilon & antenna patterns
 		if not (isinstance(epsilon, (float, list, np.ndarray)) or epsilon is None):
 			raise ValueError("epsilon should be a float, list or None")
 	
+		if antenna_patterns is None:
+			antenna_patterns = (1,0)
+		assert isinstance(antenna_patterns, (tuple, list, np.ndarray)), "Antenna pattern must be a tuple"
+		F_p, F_c = antenna_patterns
+	
 		##
 		# Computing the metric
 		
 		metric = []
 		for theta_i in theta:
-			WF1 = self.get_WF(theta_i, self.approx) #used by
+			WF2_p, WF2_c = self.get_WF(theta_i, self.approx, plus_cross = True) #used by
+				#Building the signal
 			center = np.array([0, *theta_i])
 
 			#setting epsilon (if it's the case)
 			#FIXME: this does not work!!
 			if epsilon is None:			
 				epsilon_list = np.full(center.shape, 1e-5)
 			
@@ -993,17 +1088,17 @@
 			metric[i,...] = project_metric(M_, [j for j in range(theta.shape[-1])])
 		metric = 0.5*metric
 				
 		if squeeze: metric = metric[0]
 		
 		return metric
 
-	def get_hessian_symmetrized_plus_cross(self, theta, overlap = False, order = None, epsilon = 1e-5):
+	def get_hessian_symphony(self, theta, overlap = False, order = None, epsilon = 1e-5, time_comps = False):
 		"""
-		Returns the Hessian matrix where :math:`h_+` and :math:`h_\\times` are treated on the same footing.
+		Returns the Hessian matrix of the symphony match.
 		
 		Parameters
 		----------
 		
 		theta: :class:`~numpy:numpy.ndarray`
 			shape: (N,D)/(D,) -
 			Parameters of the BBHs. The dimensionality depends on self.variable_format
@@ -1014,29 +1109,109 @@
 
 		order: int
 			Order of the finite difference scheme for the gradient computation.
 			If None, some defaults values will be set, depending on the total mass.
 
 		epsilon: list
 			Size of the jump for the finite difference scheme for each dimension. If a float, the same jump will be used for all dimensions
+		
+		time_comps: bool
+			Whether to return the time components :math:`H_{it}, H_{tt}` of the hessian of the overlap.
 
 		Returns
 		-------
 		
 		metric : :class:`~numpy:numpy.ndarray`
 			shape: (N,D,D)/(D,D) -
 			Array containing the metric Hessian in the given parameters
 			
 		"""
-		H_pp = self.get_hessian(theta, overlap = overlap, order = order, epsilon = epsilon, use_cross = False)
-		H_cc = self.get_hessian(theta, overlap = overlap, order = order, epsilon = epsilon, use_cross = True)
-		#print(np.linalg.det(H_pp), np.linalg.det(H_cc))
-		return (H_pp + H_cc)/2.
+		#TODO: this function is weird: it should return either the (D,D) hessian or the (D+1, D+1) hessian. The merginalization should be performed by get_metric. On the other hands, this will be computationally inefficient, so we can probably keep it as it is for the sake of speed.
+		theta = np.asarray(theta)
+		squeeze = False
+		if theta.ndim ==1:
+			theta = theta[None,:]
+			squeeze = True
+
+		####
+		#computing the metric
+		####
+
+		###
+		# Scalar products in FD
+		hp, hc = self.get_WF(theta, approx = self.approx, plus_cross = True) #(N,D)
+		grad_h = self.get_WF_grads(theta, approx = self.approx, order = order, epsilon = epsilon) #(N,D, K)
+		
+		hp_W = hp / np.sqrt(self.PSD) #whithened plus
+		hc_W = hc / np.sqrt(self.PSD) #whithened cross
+		#hc_W = 1j*hp_W #Add this to recover the NP limit...
+		
+		grad_h_W = grad_h/np.sqrt(self.PSD[:,None]) #whithened grads
+		
+		hpp = np.sum(np.multiply(np.conj(hp_W), hp_W), axis =1).real #(N,)
+		hcc = np.sum(np.multiply(np.conj(hc_W), hc_W), axis =1).real #(N,)
+		hpc = np.sum(np.multiply(np.conj(hp_W), hc_W), axis =1).real #(N,)
+		hpc_norm = hpc/np.sqrt(hpp*hcc)
+		
+		hp_grad_h = np.einsum('ij,ijk->ik', np.conj(hp_W), grad_h_W) #(N,K)
+		hc_grad_h = np.einsum('ij,ijk->ik', np.conj(hc_W), grad_h_W) #(N,K)
+		grad_h_grad_h_real = np.einsum('ijk,ijl->ikl', np.conj(grad_h_W), grad_h_W).real #(N,K,K)
+		
+		###
+		#computing the metric
+		
+		metric = np.einsum('ij,ik->ijk', (hp_grad_h.real.T/hpp).T, (hc_grad_h.real.T/np.sqrt(hcc*hpp)).T) #(N,K,K) 
+		metric =  - hpc_norm[:,None,None] * (metric + np.swapaxes(metric,1,2)) #(N,K,K) 
+		metric = metric + np.einsum('ij,ik,i->ijk', hp_grad_h.real, hp_grad_h.real, 1./np.square(hpp)) #(N,K,K) 
+		metric = metric + np.einsum('ij,ik,i->ijk', hc_grad_h.real, hc_grad_h.real, 1./(hpp*hcc)) #(N,K,K)
+		metric = np.divide(metric, (1-hpc_norm**2)[:,None,None])
+		metric = metric - np.divide(grad_h_grad_h_real, hpp[:,None,None]) #(N,K,K)
 
-	def get_hessian(self, theta, overlap = False, order = None, epsilon = 1e-5, use_cross = False):
+			#including time dependence
+		if (not overlap) or time_comps:
+			hp_hp_f = np.sum(np.multiply(np.conj(hp_W), hp_W*self.f_grid), axis =1) #(N,)
+			hc_hp_f = np.sum(np.multiply(np.conj(hc_W), hp_W*self.f_grid), axis =1) #(N,)
+			hp_hp_f2 = np.sum(np.multiply(np.conj(hp_W), hp_W*np.square(self.f_grid)), axis =1) #(N,)
+			hp_grad_h_f = np.einsum('ij,ijk->ik', np.conj(hp_W)*self.f_grid, grad_h_W) #(N,K)
+			hc_grad_h_f = np.einsum('ij,ijk->ik', np.conj(hc_W)*self.f_grid, grad_h_W) #(N,K)
+			
+			g_tt = np.square(hc_hp_f.imag/np.sqrt(hpp*hcc))/(1-hpc_norm**2)
+			g_tt = g_tt- hp_hp_f2.real/hpp #(N,)
+			
+			g_ti = - (hc_grad_h.real.T/hpp)*(hc_hp_f.imag/hcc) #(K,N)
+			g_ti = g_ti + hpc_norm*(hc_hp_f.imag/np.sqrt(hpp*hcc))*(hp_grad_h.real.T/hpp) #(K,N)
+			g_ti = g_ti / (1-hpc_norm**2) #(K,N)
+			g_ti = g_ti - hp_grad_h_f.imag.T/hpp #(K,N)
+			g_ti = g_ti.T #(N,K)
+		
+		if not overlap:
+			time_factor = np.einsum('ij,ik,i->ijk', g_ti, g_ti, 1./g_tt)
+			metric = metric - time_factor
+		
+			#adding the -0.5 factor
+		metric = -0.5*metric
+
+		eigval, eigvec = np.linalg.eig(metric)
+		if np.any(eigval<=0):
+			#FIXME: this shouldn't be happening!
+			msg = "One of the metric eigenvalue is negative! Beware: metric computation is not stable...\nCenter: {}\n\thpc: {}\n\teigs: {}".format(theta, hpc_norm, eigval)
+			warnings.warn(msg)
+			#metric = np.einsum('ijk,ik,ilk->ijl', eigvec, np.abs(eigval), eigvec)
+			
+		#print('hpc norm: ',hpc_norm)
+
+		if squeeze: metric = np.squeeze(metric)
+		if squeeze and time_comps: g_ti, g_tt = np.squeeze(g_ti), np.squeeze(g_tt)
+
+		if time_comps:
+			return metric, g_ti, g_tt
+		return metric
+			
+
+	def get_hessian(self, theta, overlap = False, order = None, epsilon = 1e-5, time_comps = False):
 		"""
 		Returns the Hessian matrix.
 		
 		Parameters
 		----------
 		
 		theta: :class:`~numpy:numpy.ndarray`
@@ -1050,44 +1225,42 @@
 		order: int
 			Order of the finite difference scheme for the gradient computation.
 			If None, some defaults values will be set, depending on the total mass.
 
 		epsilon: list
 			Size of the jump for the finite difference scheme for each dimension. If a float, the same jump will be used for all dimensions
 
-		use_cross: bool
-			Whether to use the cross polarization to compute the hessian.
+		time_comps: bool
+			Whether to return the time components :math:`H_{it}, H_{tt}` of the hessian of the overlap.
 
 		Returns
 		-------
 		
 		metric : :class:`~numpy:numpy.ndarray`
 			shape: (N,D,D)/(D,D) -
 			Array containing the metric Hessian in the given parameters
 			
 		"""
-			#TODO: understand whether the time shift is an issue here!!
-			#		Usually match is max_t0 <h1(t)|h2(t-t0)>. How to cope with that? It this may make the space larger than expected
+		#TODO: this function is weird: it should return either the (D,D) hessian or the (D+1, D+1) hessian. The merginalization should be performed by get_metric. On the other hands, this will be computationally inefficient, so we can probably keep it as it is for the sake of speed.
 		theta = np.asarray(theta)
 		squeeze = False
 		if theta.ndim ==1:
 			theta = theta[None,:]
 			squeeze = True
 
 		####
 		#computing the metric
 		####
 			#M(theta) = - 0.5 * { (h|d_i h)(h|d_j h) / <h|h>^2 + [h|d_i h][h|d_j h] / <h|h>^2 - (d_i h|d_j h) / <h|h> }
 
 		#The following outputs grad_h_grad_h_real (N,D,4,4), h_grad_h.real/h_grad_h.imag (N,D,4) and h_h (N,D), evaluated on self.f_grid (or in a std grid if PSD is None)
 
 		### scalar product in FD
-		hp, hc = self.get_WF(theta, approx = self.approx, plus_cross = True) #(N,D)
-		h = hc if use_cross else hp
-		grad_h = self.get_WF_grads(theta, approx = self.approx, order = order, epsilon = epsilon, use_cross = use_cross) #(N,D, K)
+		h = self.get_WF(theta, approx = self.approx, plus_cross = False) #(N,D)
+		grad_h = self.get_WF_grads(theta, approx = self.approx, order = order, epsilon = epsilon) #(N,D, K)
 		
 		h_W = h / np.sqrt(self.PSD) #whithened WF
 		grad_h_W = grad_h/np.sqrt(self.PSD[:,None]) #whithened grads
 		
 		h_h = np.sum(np.multiply(np.conj(h_W), h_W), axis =1).real #(N,)
 		h_grad_h = np.einsum('ij,ijk->ik', np.conj(h_W), grad_h_W) #(N,K)
 		grad_h_grad_h_real = np.einsum('ijk,ijl->ikl', np.conj(grad_h_W), grad_h_W).real #(N,K,K)
@@ -1095,34 +1268,38 @@
 		###
 		#computing the metric, given h_grad_h.real (N,D,4), h_grad_h.imag (N,D,4) and h_h (N,D)
 		metric = np.einsum('ij,ik->ijk', h_grad_h.real, h_grad_h.real) 
 		metric = metric + np.einsum('ij,ik->ijk', h_grad_h.imag, h_grad_h.imag)
 		metric = np.einsum('ijk,i->ijk', metric , 1./np.square(h_h))
 		metric = metric - np.divide(grad_h_grad_h_real, h_h[:,None,None])
 
-		if not overlap:
+		if (not overlap) or time_comps:
 			#including time dependence
 			h_h_f = np.sum(np.multiply(np.conj(h_W), h_W*self.f_grid), axis =1) #(N,)
 			h_h_f2 = np.sum(np.multiply(np.conj(h_W), h_W*np.square(self.f_grid)), axis =1) #(N,)
 			h_grad_h_f = np.einsum('ij,ijk->ik', np.conj(h_W)*self.f_grid, grad_h_W) #(N,4)
 			
 			g_tt = np.square(h_h_f.real/h_h) - h_h_f2.real/h_h #(N,)
 			
-			g_ti = (h_grad_h.imag.T * h_h_f.real + h_grad_h.real.T * h_h_f.imag).T #(N,K)
+			g_ti = (h_grad_h.imag.T * h_h_f.real).T #(N,K)
 			g_ti = (g_ti.T/np.square(h_h)).T
 			g_ti = g_ti - (h_grad_h_f.imag.T/h_h).T
-			
+		
+		if not overlap:
 			time_factor = np.einsum('ij,ik,i->ijk', g_ti, g_ti, 1./g_tt)
 			metric = metric - time_factor
 		
 			#adding the -0.5 factor
 		metric = -0.5*metric
 		
-		if squeeze:	metric = np.squeeze(metric)
+		if squeeze: metric = np.squeeze(metric)
+		if squeeze and time_comps: g_ti, g_tt = np.squeeze(g_ti), np.squeeze(g_tt)
 
+		if time_comps:
+			return metric, g_ti, g_tt
 		return metric
 	
 	def WF_symphony_match(self, signal, template_plus, template_cross, overlap = False):
 		"""
 		Computes the match element by element between two set of frequency domain WFs, using the `symphony` match.
 		The symphony match is defined in eq (13) of `1709.09181 <https://arxiv.org/abs/1709.09181>`_
 		No checks will be perfomed on the inputs
@@ -1178,15 +1355,14 @@
 			#TODO: pad with zeros the frequency series here!!
 		SNR_fs_p = np.multiply(np.conj(s_WN), h1p_WN) #(N,D) #frequency series
 		SNR_fs_c = np.multiply(np.conj(s_WN), h1c_WN) #(N,D) #frequency series
 		
 		SNR_ts_p = np.fft.ifft(SNR_fs_p, axis =-1).real*SNR_fs_p.shape[-1]
 		SNR_ts_c = np.fft.ifft(SNR_fs_c, axis =-1).real*SNR_fs_c.shape[-1]
 
-			#This correlation does not agree with sbank!!
 		h1pc = np.sum(np.multiply(np.conj(h1p_WN), h1c_WN), axis = -1).real
 		den = 1- np.square(h1pc)
 		
 		SNR_ts = np.square(SNR_ts_p).T + np.square(SNR_ts_c).T - 2*SNR_ts_p.T*SNR_ts_c.T*h1pc #(N,D)
 		SNR_ts = SNR_ts/den #(N,D)
 		SNR_ts = SNR_ts.T
 		SNR_ts = np.sqrt(SNR_ts) #remember this!! It is important :)
```

### Comparing `gw-mbank-0.2.0/mbank/utils.py` & `gw-mbank-0.3.1/mbank/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -205,15 +205,15 @@
 	return 2*np.sqrt((1-avg_match)/D) #Owen
 	#return 2*np.sqrt(1-avg_match)
 
 
 ####################################################################################################################
 
 def get_boundaries_from_ranges(variable_format, M_range, q_range,
-	s1_range = (-0.99,0.99), s2_range = (-0.99,0.99), chi_range = (-0.99,0.99), theta_range = (0, np.pi), phi_range = (-np.pi, np.pi),
+	s1_range = (-0.99,0.99), s2_range = (-0.99,0.99), chi_range = (-0.99,0.99), theta_range = (-np.pi, np.pi), phi_range = (-np.pi/2., np.pi/2.),
 	iota_range = (0, np.pi), ref_phase_range = (-np.pi, np.pi), e_range = (0., 0.5), meanano_range = (0.1, 1.)):
 	"""
 	Given the ranges of each quantity, it combines them in a bondary array, suitable for other uses in the package (for instance in the bank generation).
 	No checks are performed whether the given ranges make sense.
 	
 	Parameters
 	----------
@@ -449,27 +449,27 @@
 		inj_dict: dict
 			The output dictionary with the updated matches
 	"""
 	inj_dict = dict(inj_dict)
 	sky_locs = inj_dict['sky_loc']
 	
 	old_format = metric_obj.variable_format
-	if metric_obj.variable_format != 'm1m2_fullspins_emeanano_iotaphi':
-		metric_obj.set_variable_format('m1m2_fullspins_emeanano_iotaphi')
+	if metric_obj.variable_format != 'BBH_components':
+		metric_obj.set_variable_format('BBH_components')
 
 		#allocating memory for the match
 	inj_dict['id_match'] = np.zeros((inj_dict['theta_inj'].shape[0],), int)
 	inj_dict['match'] = np.zeros((inj_dict['theta_inj'].shape[0],))
 	inj_dict['symphony_SNR'] = symphony_match
 	inj_dict['mchirp_window'] = mchirp_window
 
 		#putting injections and templates with the format 'm1m2_fullspins_emeanano_iotaphi'
 		# The format is basically the full 12 dimensional space, with spins in spherical coordinates
-	injs = metric_obj.var_handler.get_theta(inj_dict['theta_inj'], 'm1m2_fullspins_emeanano_iotaphi')
-	templates = metric_obj.var_handler.get_theta(bank.BBH_components, 'm1m2_fullspins_emeanano_iotaphi')
+	injs = inj_dict['theta_inj']
+	templates = bank.BBH_components
 	
 	chirp_injs = metric_obj.var_handler.get_mchirp(injs[:,[0,1]], 'm1m2_nonspinning')
 	chirp_templates = metric_obj.var_handler.get_mchirp(templates[:,[0,1]], 'm1m2_nonspinning')
 
 		#Dealing with antenna patterns
 	if sky_locs is not None:
 		sky_locs = np.asarray(sky_locs)
@@ -816,15 +816,15 @@
 	
 		###
 		#Plotting templates & tiles
 		###
 	if templates.shape[0] >500000: ids_ = np.random.choice(templates.shape[0], 500000, replace = False)
 	else: ids_ = range(templates.shape[0])
 	
-	size_template = [20 if templates.shape[0] < 5000 else 2][0]
+	size_template = 20 if templates.shape[0] < 500 else 2
 	fsize = 4* templates.shape[1]-1
 	fig, axes = plt.subplots(templates.shape[1]-1, templates.shape[1]-1, figsize = (fsize, fsize))
 	plt.suptitle('Templates of the bank: {} points'.format(templates.shape[0]), fontsize = fs+10)
 	if templates.shape[1]-1 == 1:
 		axes = np.array([[axes]])
 	for i,j in permutations(range(templates.shape[1]-1), 2):
 		if i<j:	axes[i,j].remove()
@@ -1343,45 +1343,45 @@
 			template_list.remove(t_)
 			template_list.extend(extended_list)
 	new_templates = np.array([t_.center for t_, _ in template_list])
 	
 	return new_templates
 
 #@do_profile(follow = [])
-def place_random(minimum_match, tiling, N_livepoints, tolerance = 0.01, verbose = True):	
+def place_random(minimum_match, tiling, N_livepoints, covering_fraction = 0.01, verbose = True):	
 	"""
-	Draw templates from the uniform distribution on the manifold. For each proposal, all the livepoints in the ellipse of constant ``minimum_match`` are killed. The iteration goes on until a fraction of ``tolerance`` of livepoints are alive.
+	Draw templates from the uniform distribution on the manifold. For each proposal, all the livepoints in the ellipse of constant ``minimum_match`` are killed. The iteration goes on until a fraction of ``covering_fraction`` of livepoints are alive.
 	It follows `2202.09380 <https://arxiv.org/abs/2202.09380>`_
 	
 	Parameters
 	----------
 	
 		minimum_match: float
 			Minimum match between templates.
 		
 		tiling: tiling_handler
 			Tiling handler that tiles the parameter space
 		
 		N_livepoints: int
 			Number of livepoints to cover the space with
 		
-		tolerance: float
+		covering_fraction: float
 			Fraction of livepoints to be covered before terminating the loop
 		
 		verbose: bool
 			Whether to display the progress bar
 	
 	Returns
 	-------
 		new_templates: :class:`~numpy:numpy.ndarray`
 			shape: (N,D) -
 			A set of templates generated by the placing algorithm
 	
 	"""
-	assert 0<tolerance <=1., "The tolerance should be a fraction in (0,1]"
+	assert 0<covering_fraction <=1., "The covering_fraction should be a fraction in (0,1]"
 	MM = minimum_match
 	dtype = np.float32
 	N_livepoints = 10000
 	
 	livepoints = tiling.sample_from_tiling(N_livepoints,
 				dtype = dtype, tile_id = False, p_equal = False)
 	new_templates = []
@@ -1392,15 +1392,15 @@
 	proposal_list, proposal_ids_, log_pdf_theta_list = [], [], []
 	
 	bar_str = '{} templates placed ({} % livepoints alive)'
 	if verbose: it = tqdm(dummy_iterator(), desc = bar_str.format(len(new_templates), 100), leave = True)
 	else: it = dummy_iterator()
 	
 	for _ in it: 
-		if len(livepoints)<N_livepoints*tolerance: break
+		if len(livepoints)<N_livepoints*covering_fraction: break
 		
 			#Generating proposals
 		if tiling.flow:
 			with torch.no_grad():
 				if len(proposal_list)==0:
 					proposal_list, log_pdf_theta_list = tiling.flow.sample_and_log_prob(1000)
 					proposal_list, log_pdf_theta_list = list(proposal_list.numpy()), list(log_pdf_theta_list.numpy())
@@ -1441,15 +1441,15 @@
 
 
 	new_templates = np.array(new_templates)
 	
 	return new_templates
 
 #@do_profile(follow=[])
-def place_pruning(minimum_match, tiling, N_points, tolerance = 0.01, verbose = True):
+def place_pruning(minimum_match, tiling, N_points, covering_fraction = 0.01, verbose = True):
 	"""
 	Given a tiling object, it covers the volume with points and covers them with templates.
 	It uses a pruning method, where proposal are chosen from a large set of random points, called livepoints. The bank is created by selecting a proposal from the set of livepoints and removing (killing) the livepoints too close from the proposal. This methods effectively prunes the original set of livepoints, to remove the random points that are too close from each other.
 	
 	Parameters
 	----------
 	
@@ -1458,30 +1458,30 @@
 		
 		tiling: tiling_handler
 			Tiling handler that tiles the parameter space
 		
 		N_points: int
 			Number of livepoints to cover the space with
 		
-		tolerance: float
+		covering_fraction: float
 			Fraction of livepoints to be covered before terminating the loop
 		
 		verbose: bool
 			Whether to display the progress bar
 	
 	Returns
 	-------
 		new_templates: :class:`~numpy:numpy.ndarray`
 			shape: (N,D) -
 			A set of templates generated by the placing algorithm
 	"""
 	#TODO: maybe here you can use the tiling KDTree for saving some useless computations?
 	#i.e. you should add a tiling label to all the generated livepoints and use it somehow...
 	
-	assert 0<tolerance <=1., "The tolerance should be a fraction in (0,1]"
+	assert 0<covering_fraction <=1., "The covering_fraction should be a fraction in (0,1]"
 	assert isinstance(N_points, int) and N_points>0, "N_points should be a positive integer"
 	
 	MM = minimum_match
 	dtype = np.float32 #better to downcast to single precision! There is a mild speedup there
 	
 		#FIXME: add here the sampling from flow option!
 	livepoints, id_tile_livepoints = tiling.sample_from_tiling(N_points,
@@ -1545,15 +1545,15 @@
 		det_livepoints = np.delete(det_livepoints, ids_kill, axis = 0)
 		
 				#this is very very subtle: if you don't allocate new memory with np.array, you won't decrease the reference to livepoints, which won't be deallocated. This is real real bad!!
 		new_templates.append(np.array(point, dtype = np.float64))
 		del point
 			
 			#communication and exit condition
-		if len(livepoints)<=tolerance*N_points: break
+		if len(livepoints)<=covering_fraction*N_points: break
 		if len(new_templates) %100 ==0 and verbose: it.set_description(bar_str.format(N_points -len(livepoints), N_points, len(new_templates)) )
 	
 	new_templates = np.column_stack([new_templates])
 	#if len(livepoints)>0: new_templates = np.concatenate([new_templates, livepoints], axis =0) #adding the remaining livepoints
 	
 	return new_templates
 
@@ -1682,15 +1682,15 @@
 ###########################################################################################
 
 #All the garbage here should be removed!!
 
 def points_in_hull(points, hull, tolerance=1e-12):
 	#"Check if points (N,D) are in the hull"
 	if points.ndim == 1:
-		points = point[None,:]
+		points = points[None,:]
 	
 	value_list = [np.einsum('ij,j->i', points, eq[:-1])+eq[-1] for eq in hull.equations]
 	value_list = np.array(value_list).T #(N, N_eqs)
 	
 	return np.prod(value_list<= tolerance, axis = 1).astype(bool) #(N,)
 
 def all_line_hull_intersection(v, c, hull):
@@ -2181,15 +2181,15 @@
 			sim_inspiral_table.append(row)
 
 		#ligolw_process.set_process_end_time(process)
 		xmldoc.childNodes[-1].appendChild(sim_inspiral_table)
 		lw_utils.write_filename(xmldoc, filename, verbose=False)
 		xmldoc.unlink()
 
-		print("Saved {} injections to {}".format(i+1, filename))
+		print("Saved {} injections to {}".format(i+1, filename)) #FIXME: remove this from here!
 
 		return 
 
 def load_inj_stat_dict(filename):
 	"""
 	Loads an injection statistics dictionary (see :func`compute_injections_match`) from a json or pickle file.
```

### Comparing `gw-mbank-0.2.0/setup.py` & `gw-mbank-0.3.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,29 +14,30 @@
 #required_packages =[]
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name="gw-mbank",
-	version="0.2.0",
+	version="0.3.1",
 	author="Stefano Schmidt",
 	author_email="stefanoschmidt1995@gmail.com",
 	description="Metric bank generation for gravitational waves data analysis",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	url="https://github.com/stefanoschmidt1995/mbank",
 	packages=setuptools.find_packages(),
 	license = 'GNU GENERAL PUBLIC LICENSE v3',
 	classifiers=[
 		"Programming Language :: Python :: 3",
 		"Operating System :: OS Independent",
 	],
 	scripts = ["bin/mbank_run", "bin/mbank_injfile", "bin/mbank_mcmc", 
-		"bin/mbank_place_templates", "bin/mbank_merge","bin/mbank_validate_metric",
+		"bin/mbank_place_templates", "bin/mbank_merge",
+		"bin/mbank_validate_metric", "bin/mbank_print_metric",
 		"bin/mbank_injections", "bin/mbank_injections_workflow"],
 	python_requires='>=3.7',
 	install_requires=required_packages,
 	command_options={
         'build_sphinx': {
             'source_dir': ('setup.py', 'docs'),
             'build_dir': ('setup.py', 'docs/__build'),
```

