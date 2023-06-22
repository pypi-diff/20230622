# Comparing `tmp/straxen-2.0.7.tar.gz` & `tmp/straxen-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "straxen-2.0.7.tar", last modified: Tue Apr 25 03:21:47 2023, max compression
+gzip compressed data, was "straxen-2.1.0.tar", last modified: Thu Jun 22 19:23:06 2023, max compression
```

## Comparing `straxen-2.0.7.tar` & `straxen-2.1.0.tar`

### file list

```diff
@@ -1,240 +1,242 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.662989 straxen-2.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    37812 2023-04-25 03:21:42.000000 straxen-2.0.7/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-25 03:21:42.000000 straxen-2.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-25 03:21:42.000000 straxen-2.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    50278 2023-04-25 03:21:47.662989 straxen-2.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-04-25 03:21:42.000000 straxen-2.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.646988 straxen-2.0.7/bin/
--rw-r--r--   0 runner    (1001) docker     (123)    37235 2023-04-25 03:21:42.000000 straxen-2.0.7/bin/ajax
--rwxr-xr-x   0 runner    (1001) docker     (123)    67099 2023-04-25 03:21:42.000000 straxen-2.0.7/bin/bootstrax
--rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-04-25 03:21:42.000000 straxen-2.0.7/bin/fake_daq
--rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-04-25 03:21:42.000000 straxen-2.0.7/bin/microstrax
--rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-04-25 03:21:42.000000 straxen-2.0.7/bin/refresh_raw_records
--rw-r--r--   0 runner    (1001) docker     (123)    35964 2023-04-25 03:21:42.000000 straxen-2.0.7/bin/restrax
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-25 03:21:42.000000 straxen-2.0.7/bin/straxen-print_versions
--rw-r--r--   0 runner    (1001) docker     (123)    12241 2023-04-25 03:21:42.000000 straxen-2.0.7/bin/straxer
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.646988 straxen-2.0.7/extra_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-25 03:21:42.000000 straxen-2.0.7/extra_requirements/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-25 03:21:42.000000 straxen-2.0.7/extra_requirements/requirements-tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-25 03:21:43.000000 straxen-2.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-25 03:21:47.666989 straxen-2.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-04-25 03:21:43.000000 straxen-2.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.646988 straxen-2.0.7/straxen/
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.650988 straxen-2.0.7/straxen/analyses/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/analyses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38954 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/analyses/bokeh_waveform_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/analyses/daq_waveforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    18579 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/analyses/event_display.py
--rw-r--r--   0 runner    (1001) docker     (123)    17242 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/analyses/holoviews_waveform_display.py
--rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/analyses/posrec_comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/analyses/pulse_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     8723 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/analyses/quick_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/analyses/records_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    10245 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/analyses/waveform_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/bokeh_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    21032 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    21286 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/contexts.py
--rw-r--r--   0 runner    (1001) docker     (123)    18130 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/corrections_services.py
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/daq_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/entry_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     8203 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/get_corrections.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.650988 straxen-2.0.7/straxen/holoviews/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/holoviews/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11014 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/holoviews/holoviews_inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)    13244 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/holoviews/holoviews_peak_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/holoviews/holoviews_pmt_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    17711 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/holoviews/holoviews_tpc_event_display.py
--rw-r--r--   0 runner    (1001) docker     (123)    21799 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/holoviews_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10806 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/itp_map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.650988 straxen-2.0.7/straxen/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/legacy/contexts_1t.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/legacy/hitfinder_thresholds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.650988 straxen-2.0.7/straxen/legacy/plugins_1t/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/legacy/plugins_1t/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/legacy/plugins_1t/event_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/legacy/plugins_1t/pax_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/legacy/plugins_1t/peak_positions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10186 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/legacy/plugins_1t/x1t_cuts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/legacy/xenon1t_url_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/matplotlib_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/mini_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/numbafied_scipy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.650988 straxen-2.0.7/straxen/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.650988 straxen-2.0.7/straxen/plugins/afterpulses/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/afterpulses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11243 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/afterpulses/afterpulse_processing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.650988 straxen-2.0.7/straxen/plugins/aqmon_hits/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/aqmon_hits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/aqmon_hits/aqmon_hits.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.650988 straxen-2.0.7/straxen/plugins/detector_time_offsets/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/detector_time_offsets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/detector_time_offsets/detector_time_offsets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.654988 straxen-2.0.7/straxen/plugins/events/
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events/_event_s1_position_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events/_event_s2_position_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events/corrected_areas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events/distinct_channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events/energy_estimates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events/event_ambience.py
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events/event_area_per_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)    15996 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events/event_basics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events/event_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events/event_info_double.py
--rw-r--r--   0 runner    (1001) docker     (123)    25160 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events/event_pattern_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events/event_positions.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events/event_s1_position_cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events/event_s2_position_cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events/event_s2_position_gcn.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events/event_s2_position_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events/event_shadow.py
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events/event_top_bottom_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events/event_w_bayes_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     8632 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events/local_minimum_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events/multi_scatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events/s2_recon_pos_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events/veto_proximity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.654988 straxen-2.0.7/straxen/plugins/events_mv/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events_mv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events_mv/events_mv.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events_mv/events_sync_mv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.654988 straxen-2.0.7/straxen/plugins/events_nv/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events_nv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8123 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events_nv/event_positions_nv.py
--rw-r--r--   0 runner    (1001) docker     (123)     9012 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events_nv/events_nv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/events_nv/events_sync_nv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.654988 straxen-2.0.7/straxen/plugins/hitlets_mv/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/hitlets_mv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/hitlets_mv/hitlets_mv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.654988 straxen-2.0.7/straxen/plugins/hitlets_nv/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/hitlets_nv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/hitlets_nv/hitlets_nv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.654988 straxen-2.0.7/straxen/plugins/individual_peak_monitor/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/individual_peak_monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/individual_peak_monitor/individual_peak_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.654988 straxen-2.0.7/straxen/plugins/led_cal/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/led_cal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9058 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/led_cal/led_calibration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.654988 straxen-2.0.7/straxen/plugins/merged_s2s/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/merged_s2s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8530 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/merged_s2s/merged_s2s.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.654988 straxen-2.0.7/straxen/plugins/merged_s2s_he/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/merged_s2s_he/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/merged_s2s_he/merged_s2s_he.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.654988 straxen-2.0.7/straxen/plugins/online_monitor_mv/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/online_monitor_mv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/online_monitor_mv/online_monitor_mv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.654988 straxen-2.0.7/straxen/plugins/online_monitor_nv/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/online_monitor_nv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/online_monitor_nv/online_monitor_nv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.658989 straxen-2.0.7/straxen/plugins/online_peak_monitor/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/online_peak_monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6954 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/online_peak_monitor/online_peak_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.658989 straxen-2.0.7/straxen/plugins/peaklets/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/peaklets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/peaklets/peaklet_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    23844 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/peaklets/peaklets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.662989 straxen-2.0.7/straxen/plugins/peaklets_he/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/peaklets_he/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/peaklets_he/peaklet_classification_he.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/peaklets_he/peaklets_he.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.662989 straxen-2.0.7/straxen/plugins/peaks/
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/peaks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/peaks/_peak_positions_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/peaks/_peak_s1_position_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/peaks/peak_ambience.py
--rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/peaks/peak_basics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/peaks/peak_classification_bayes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/peaks/peak_positions.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/peaks/peak_positions_cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/peaks/peak_positions_gcn.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/peaks/peak_positions_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/peaks/peak_proximity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/peaks/peak_s1_position_cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     9402 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/peaks/peak_shadow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/peaks/peak_top_bottom_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/peaks/peaks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/peaks/peaks_corrections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/peaks/peaks_per_event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.662989 straxen-2.0.7/straxen/plugins/peaks_he/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/peaks_he/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/peaks_he/peak_basics_he.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/peaks_he/peaks_he.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.662989 straxen-2.0.7/straxen/plugins/raw_records/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/raw_records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16653 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/raw_records/daqreader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.662989 straxen-2.0.7/straxen/plugins/raw_records_coin_nv/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/raw_records_coin_nv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19659 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/raw_records_coin_nv/nveto_recorder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.662989 straxen-2.0.7/straxen/plugins/records/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17703 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/records/records.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.662989 straxen-2.0.7/straxen/plugins/records_he/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/records_he/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/records_he/records_he.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.662989 straxen-2.0.7/straxen/plugins/records_mv/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/records_mv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/records_mv/records_mv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.662989 straxen-2.0.7/straxen/plugins/records_nv/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/records_nv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/records_nv/records_nv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.662989 straxen-2.0.7/straxen/plugins/veto_intervals/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/veto_intervals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/plugins/veto_intervals/veto_intervals.py
--rw-r--r--   0 runner    (1001) docker     (123)    27943 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/scada.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.662989 straxen-2.0.7/straxen/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15115 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/storage/mongo_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/storage/online_monitor_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)     6954 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/storage/rucio_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/storage/rucio_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)    13251 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/storage/rundb.py
--rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/units.py
--rw-r--r--   0 runner    (1001) docker     (123)    23704 2023-04-25 03:21:43.000000 straxen-2.0.7/straxen/url_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.650988 straxen-2.0.7/straxen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    50278 2023-04-25 03:21:47.000000 straxen-2.0.7/straxen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-04-25 03:21:47.000000 straxen-2.0.7/straxen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 03:21:47.000000 straxen-2.0.7/straxen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 03:21:47.000000 straxen-2.0.7/straxen.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-25 03:21:47.000000 straxen-2.0.7/straxen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-25 03:21:47.000000 straxen-2.0.7/straxen.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.662989 straxen-2.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:47.662989 straxen-2.0.7/tests/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9751 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/storage/test_database_frontends.py
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/storage/test_mongo_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/storage/test_mongo_interactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/storage/test_rucio_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/storage/test_rucio_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/test_1T_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)    10536 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/test_aqmon.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/test_basics.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/test_channel_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/test_cmt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/test_contexts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/test_count_pulses.py
--rw-r--r--   0 runner    (1001) docker     (123)     6810 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/test_daq_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/test_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/test_holoviews_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/test_itp_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/test_led_calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)    17347 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/test_mini_analyses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9765 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/test_nveto_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/test_nveto_recorder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/test_patternfit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/test_peaklet_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/test_peaks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/test_scada.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/test_testing_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)    13701 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/test_url_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-25 03:21:43.000000 straxen-2.0.7/tests/test_veto_hitlets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.976051 straxen-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    40334 2023-06-22 19:23:01.000000 straxen-2.1.0/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-06-22 19:23:01.000000 straxen-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-22 19:23:01.000000 straxen-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    53024 2023-06-22 19:23:06.976051 straxen-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-22 19:23:01.000000 straxen-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.956050 straxen-2.1.0/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)    37235 2023-06-22 19:23:01.000000 straxen-2.1.0/bin/ajax
+-rwxr-xr-x   0 runner    (1001) docker     (123)    67099 2023-06-22 19:23:01.000000 straxen-2.1.0/bin/bootstrax
+-rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-06-22 19:23:01.000000 straxen-2.1.0/bin/fake_daq
+-rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-06-22 19:23:01.000000 straxen-2.1.0/bin/microstrax
+-rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-06-22 19:23:01.000000 straxen-2.1.0/bin/refresh_raw_records
+-rw-r--r--   0 runner    (1001) docker     (123)    35964 2023-06-22 19:23:01.000000 straxen-2.1.0/bin/restrax
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-22 19:23:01.000000 straxen-2.1.0/bin/straxen-print_versions
+-rw-r--r--   0 runner    (1001) docker     (123)    12241 2023-06-22 19:23:01.000000 straxen-2.1.0/bin/straxer
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.956050 straxen-2.1.0/extra_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-22 19:23:01.000000 straxen-2.1.0/extra_requirements/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-22 19:23:01.000000 straxen-2.1.0/extra_requirements/requirements-tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-22 19:23:01.000000 straxen-2.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-22 19:23:06.976051 straxen-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-06-22 19:23:01.000000 straxen-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.960050 straxen-2.1.0/straxen/
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.960050 straxen-2.1.0/straxen/analyses/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/analyses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38941 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/analyses/bokeh_waveform_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/analyses/daq_waveforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18579 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/analyses/event_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17242 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/analyses/holoviews_waveform_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/analyses/posrec_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/analyses/pulse_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8723 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/analyses/quick_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/analyses/records_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10245 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/analyses/waveform_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/bokeh_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21032 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22966 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/contexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18385 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/corrections_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/daq_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8203 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/get_corrections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.960050 straxen-2.1.0/straxen/holoviews/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/holoviews/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11014 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/holoviews/holoviews_inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13244 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/holoviews/holoviews_peak_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/holoviews/holoviews_pmt_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17711 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/holoviews/holoviews_tpc_event_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21799 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/holoviews_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10806 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/itp_map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.960050 straxen-2.1.0/straxen/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/legacy/contexts_1t.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/legacy/hitfinder_thresholds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.964051 straxen-2.1.0/straxen/legacy/plugins_1t/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/legacy/plugins_1t/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/legacy/plugins_1t/event_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/legacy/plugins_1t/pax_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/legacy/plugins_1t/peak_positions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10186 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/legacy/plugins_1t/x1t_cuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/legacy/xenon1t_url_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/matplotlib_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/mini_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/numbafied_scipy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.964051 straxen-2.1.0/straxen/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.964051 straxen-2.1.0/straxen/plugins/afterpulses/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/afterpulses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11243 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/afterpulses/afterpulse_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.964051 straxen-2.1.0/straxen/plugins/aqmon_hits/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/aqmon_hits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/aqmon_hits/aqmon_hits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.964051 straxen-2.1.0/straxen/plugins/detector_time_offsets/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/detector_time_offsets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/detector_time_offsets/detector_time_offsets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.964051 straxen-2.1.0/straxen/plugins/events/
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events/_event_s1_positions_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events/_event_s2_positions_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events/corrected_areas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events/distinct_channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events/energy_estimates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events/event_ambience.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events/event_area_per_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16617 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events/event_basics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events/event_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events/event_info_double.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25160 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events/event_pattern_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events/event_positions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events/event_s1_positions_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events/event_s2_positions_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events/event_s2_positions_gcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events/event_s2_positions_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events/event_shadow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events/event_top_bottom_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events/event_w_bayes_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events/event_waveform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8632 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events/local_minimum_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events/multi_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events/s2_recon_pos_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events/veto_proximity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.964051 straxen-2.1.0/straxen/plugins/events_mv/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events_mv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events_mv/events_mv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events_mv/events_sync_mv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.968051 straxen-2.1.0/straxen/plugins/events_nv/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events_nv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8123 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events_nv/event_positions_nv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9012 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events_nv/events_nv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/events_nv/events_sync_nv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.968051 straxen-2.1.0/straxen/plugins/hitlets_mv/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/hitlets_mv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/hitlets_mv/hitlets_mv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.968051 straxen-2.1.0/straxen/plugins/hitlets_nv/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/hitlets_nv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/hitlets_nv/hitlets_nv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.968051 straxen-2.1.0/straxen/plugins/individual_peak_monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/individual_peak_monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/individual_peak_monitor/individual_peak_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.968051 straxen-2.1.0/straxen/plugins/led_cal/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/led_cal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9058 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/led_cal/led_calibration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.968051 straxen-2.1.0/straxen/plugins/merged_s2s/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/merged_s2s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/merged_s2s/merged_s2s.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.968051 straxen-2.1.0/straxen/plugins/merged_s2s_he/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/merged_s2s_he/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/merged_s2s_he/merged_s2s_he.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.968051 straxen-2.1.0/straxen/plugins/online_monitor_mv/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/online_monitor_mv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/online_monitor_mv/online_monitor_mv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.968051 straxen-2.1.0/straxen/plugins/online_monitor_nv/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/online_monitor_nv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/online_monitor_nv/online_monitor_nv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.968051 straxen-2.1.0/straxen/plugins/online_peak_monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/online_peak_monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6954 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/online_peak_monitor/online_peak_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.968051 straxen-2.1.0/straxen/plugins/peaklets/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/peaklets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/peaklets/peaklet_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25757 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/peaklets/peaklets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.968051 straxen-2.1.0/straxen/plugins/peaklets_he/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/peaklets_he/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/peaklets_he/peaklet_classification_he.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/peaklets_he/peaklets_he.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.968051 straxen-2.1.0/straxen/plugins/peaks/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/peaks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/peaks/_peak_positions_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/peaks/_peak_s1_positions_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/peaks/peak_ambience.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/peaks/peak_basics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/peaks/peak_classification_bayes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/peaks/peak_corrections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/peaks/peak_per_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/peaks/peak_positions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/peaks/peak_positions_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/peaks/peak_positions_gcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/peaks/peak_positions_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/peaks/peak_proximity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/peaks/peak_s1_positions_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9402 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/peaks/peak_shadow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/peaks/peak_top_bottom_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/peaks/peaks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13029 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/peaks/peaks_subtyping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.972051 straxen-2.1.0/straxen/plugins/peaks_he/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/peaks_he/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/peaks_he/peak_basics_he.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/peaks_he/peaks_he.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.972051 straxen-2.1.0/straxen/plugins/raw_records/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/raw_records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16653 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/raw_records/daqreader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.972051 straxen-2.1.0/straxen/plugins/raw_records_coin_nv/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/raw_records_coin_nv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19659 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/raw_records_coin_nv/nveto_recorder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.972051 straxen-2.1.0/straxen/plugins/records/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17703 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/records/records.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.972051 straxen-2.1.0/straxen/plugins/records_he/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/records_he/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/records_he/records_he.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.972051 straxen-2.1.0/straxen/plugins/records_mv/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/records_mv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/records_mv/records_mv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.972051 straxen-2.1.0/straxen/plugins/records_nv/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/records_nv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/records_nv/records_nv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.972051 straxen-2.1.0/straxen/plugins/veto_intervals/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/veto_intervals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/plugins/veto_intervals/veto_intervals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27943 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/scada.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.972051 straxen-2.1.0/straxen/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15115 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/storage/mongo_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/storage/online_monitor_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6954 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/storage/rucio_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/storage/rucio_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13251 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/storage/rundb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25161 2023-06-22 19:23:01.000000 straxen-2.1.0/straxen/url_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.960050 straxen-2.1.0/straxen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    53024 2023-06-22 19:23:06.000000 straxen-2.1.0/straxen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7117 2023-06-22 19:23:06.000000 straxen-2.1.0/straxen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 19:23:06.000000 straxen-2.1.0/straxen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 19:23:06.000000 straxen-2.1.0/straxen.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-22 19:23:06.000000 straxen-2.1.0/straxen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-22 19:23:06.000000 straxen-2.1.0/straxen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.976051 straxen-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:06.976051 straxen-2.1.0/tests/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9751 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/storage/test_database_frontends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/storage/test_mongo_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/storage/test_mongo_interactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/storage/test_rucio_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/storage/test_rucio_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/test_1T_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10536 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/test_aqmon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/test_basics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/test_channel_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/test_cmt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/test_contexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/test_count_pulses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6810 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/test_daq_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/test_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/test_holoviews_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/test_itp_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/test_led_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17347 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/test_mini_analyses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9765 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/test_nveto_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/test_nveto_recorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/test_patternfit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/test_peaklet_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/test_peaks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/test_scada.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/test_testing_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15506 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/test_url_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-22 19:23:01.000000 straxen-2.1.0/tests/test_veto_hitlets.py
```

### Comparing `straxen-2.0.7/HISTORY.md` & `straxen-2.1.0/HISTORY.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,74 @@
+v2.1.70 / 2023-06-22
+-------------------
+* Added peaks subtyping by @Jianyu010 in https://github.com/XENONnT/straxen/pull/1152
+* Fix ipython version by @dachengx in https://github.com/XENONnT/straxen/pull/1169
+* Fix bug in hitlets time ordering by @dachengx in https://github.com/XENONnT/straxen/pull/1173
+* Bump actions/setup-python from 4.5.0 to 4.6.0 by @dependabot in https://github.com/XENONnT/straxen/pull/1170
+* Save hits level information(hits height and time difference) in peak and event level by @dachengx in https://github.com/XENONnT/straxen/pull/1155
+* Fix argsort inside numba.jit using kind='mergesort' by @dachengx in https://github.com/XENONnT/straxen/pull/1176
+* Bump merged_s2s version following `strax.merge_peaks` by @dachengx in https://github.com/XENONnT/straxen/pull/1179
+* Use same files names for peak and event level pos-rec by @dachengx in https://github.com/XENONnT/straxen/pull/1160
+* Update multi scatter Ignore nan in the sum of peaks. by @michaweiss89 in https://github.com/XENONnT/straxen/pull/1162
+* Add dynamic event display docs by @WenzDaniel in https://github.com/XENONnT/straxen/pull/1077
+* Lower the titles in the same notebook by @dachengx in https://github.com/XENONnT/straxen/pull/1183
+* No longer test `st.runs` in `test_extract_latest_comment_lone_hits` by @dachengx in https://github.com/XENONnT/straxen/pull/1199
+* Remove unnecessary check in `merged_s2s` by @dachengx in https://github.com/XENONnT/straxen/pull/1195
+* automatically appending local rucio path by @FaroutYLq in https://github.com/XENONnT/straxen/pull/1182
+* Performance boost veto proximity by @WenzDaniel in https://github.com/XENONnT/straxen/pull/1181
+* Update build_datastructure_doc.py by @PeterGy in https://github.com/XENONnT/straxen/pull/1202
+* Add rundoc URLConfig protocol by @jmosbacher in https://github.com/XENONnT/straxen/pull/1135
+* Split event_area_per_channel into two plugins: event_area_per_channel… by @minzhong98 in https://github.com/XENONnT/straxen/pull/1191
+* Fix event basics time ordering by @jjakob03 in https://github.com/XENONnT/straxen/pull/1194
+* Make apply_xedocs_configs more flexible by @jmosbacher in https://github.com/XENONnT/straxen/pull/1204
+* Try to make hashing more coinsistent by @LuisSanchez25 in https://github.com/XENONnT/straxen/pull/1201
+
+New Contributors
+* @PeterGy made their first contribution in https://github.com/XENONnT/straxen/pull/1202
+* @minzhong98 made their first contribution in https://github.com/XENONnT/straxen/pull/1191
+
+**Full Changelog**: https://github.com/XENONnT/straxen/compare/v2.0.7...v2.1.0
+
+
 v2.0.7 / 2023-04-25
 -------------------
-## What's Changed
 * Bootstrax target removal after failures by @cfuselli in https://github.com/XENONnT/straxen/pull/1145
 * reforming _raw_path and _processed_path by @FaroutYLq in https://github.com/XENONnT/straxen/pull/1149
 * Adding correction of Z position due to non-uniform drift velocity by @terliuk in https://github.com/XENONnT/straxen/pull/1148
 * Bump the versions of peaklets and quality check runs-on by @dachengx in https://github.com/XENONnT/straxen/pull/1153
 * S1-Based 3D Position Reconstruction by @matteoguida in https://github.com/XENONnT/straxen/pull/1146
 * Bump xedocs from 0.2.14 to 0.2.16 in /extra_requirements by @dependabot in https://github.com/XENONnT/straxen/pull/1158
 * Use zstd as compressor of peaks by @dachengx in https://github.com/XENONnT/straxen/pull/1154
 * Bump sphinx from 5.3.0 to 6.2.0 in /extra_requirements by @dependabot in https://github.com/XENONnT/straxen/pull/1161
 
-## New Contributors
+New Contributors
 * @cfuselli made their first contribution in https://github.com/XENONnT/straxen/pull/1145
 * @matteoguida made their first contribution in https://github.com/XENONnT/straxen/pull/1146
 * @hmdyt made their first contribution in https://github.com/XENONnT/straxen/pull/1159
 
 **Full Changelog**: https://github.com/XENONnT/straxen/compare/v2.0.6...v2.0.7
 
 
 v2.0.6 / 2023-03-08
 -------------------
-## What's Changed
 * Bump supercharge/mongodb-github-action from 1.8.0 to 1.9.0 by @dependabot in https://github.com/XENONnT/straxen/pull/1140
 * Small patches to restrax module by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1143, d04a3428c52c159577b61af2a28ddd0af5652027, 602b807291211f083c8f54df6768b8198fbf6b55
 * Ms events by @michaweiss89 and @HenningSE in https://github.com/XENONnT/straxen/pull/1080
 
-## New Contributors
+New Contributors
 * @michaweiss89 made their first contribution in https://github.com/XENONnT/straxen/pull/1080
 
 **Full Changelog**: https://github.com/XENONnT/straxen/compare/v2.0.5...v2.0.6
 
 Notes:
  - new data types: `peaks_per_event`, `event_top_bottom_params`, `peaks_corrections` (see #1080)
 
 
 v2.0.5 / 2023-02-24
 -------------------
-## What's Changed
 * fix xedocs for testing by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1139
 * Restart python style guide by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1138
 * Decrease number of chunks by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1123
 * Restrax by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1074
 
 
 **Full Changelog**: https://github.com/XENONnT/straxen/compare/v2.0.4...v2.0.5
@@ -979,15 +1007,15 @@
 - Updated bin scripts like straxer (#204) 
 - Updated PMT gains (#208)
 - Renamed high energy plugins (#200)
 - Bugifx in nveto-plugins (#183, #209)
 - Bugfix in clean_up_empty_records (#210)
 
 
-0.10.0 / 2020-08-187
+0.10.0 / 2020-08-18
 --------------------
 - Neutron-veto integration (#86)
 - Processing for high energy channels (#161, #176)
 - Integrate rucio as storage backend (#164)
 - Remapping of old runs (#166)
 - Bootstrax/microstrax/ajax updates (#165)
 - Pull request template (#168)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `straxen-2.0.7/LICENSE` & `straxen-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/PKG-INFO` & `straxen-2.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: straxen
-Version: 2.0.7
+Version: 2.1.0
 Summary: Streaming analysis for XENON
 Home-page: https://github.com/XENONnT/straxen
 Author: Straxen contributors, the XENON collaboration
 License: UNKNOWN
 Description: # straxen
         Streaming analysis for XENON(nT)
         
@@ -25,53 +25,81 @@
         [![Python Versions](https://img.shields.io/pypi/pyversions/straxen.svg)](https://pypi.python.org/pypi/straxen)
         [![PyPI downloads](https://img.shields.io/pypi/dm/straxen.svg)](https://pypistats.org/packages/straxen)
         
         [![Update context collection](https://github.com/XENONnT/straxen/workflows/Update%20context%20collection/badge.svg)](https://github.com/XENONnT/straxen/actions/workflows/contexts.yml)
         [![Python style](https://github.com/XENONnT/straxen/actions/workflows/code_style.yml/badge.svg)](https://github.com/XENONnT/straxen/actions/workflows/code_style.yml)
         
         
+        v2.1.70 / 2023-06-22
+        -------------------
+        * Added peaks subtyping by @Jianyu010 in https://github.com/XENONnT/straxen/pull/1152
+        * Fix ipython version by @dachengx in https://github.com/XENONnT/straxen/pull/1169
+        * Fix bug in hitlets time ordering by @dachengx in https://github.com/XENONnT/straxen/pull/1173
+        * Bump actions/setup-python from 4.5.0 to 4.6.0 by @dependabot in https://github.com/XENONnT/straxen/pull/1170
+        * Save hits level information(hits height and time difference) in peak and event level by @dachengx in https://github.com/XENONnT/straxen/pull/1155
+        * Fix argsort inside numba.jit using kind='mergesort' by @dachengx in https://github.com/XENONnT/straxen/pull/1176
+        * Bump merged_s2s version following `strax.merge_peaks` by @dachengx in https://github.com/XENONnT/straxen/pull/1179
+        * Use same files names for peak and event level pos-rec by @dachengx in https://github.com/XENONnT/straxen/pull/1160
+        * Update multi scatter Ignore nan in the sum of peaks. by @michaweiss89 in https://github.com/XENONnT/straxen/pull/1162
+        * Add dynamic event display docs by @WenzDaniel in https://github.com/XENONnT/straxen/pull/1077
+        * Lower the titles in the same notebook by @dachengx in https://github.com/XENONnT/straxen/pull/1183
+        * No longer test `st.runs` in `test_extract_latest_comment_lone_hits` by @dachengx in https://github.com/XENONnT/straxen/pull/1199
+        * Remove unnecessary check in `merged_s2s` by @dachengx in https://github.com/XENONnT/straxen/pull/1195
+        * automatically appending local rucio path by @FaroutYLq in https://github.com/XENONnT/straxen/pull/1182
+        * Performance boost veto proximity by @WenzDaniel in https://github.com/XENONnT/straxen/pull/1181
+        * Update build_datastructure_doc.py by @PeterGy in https://github.com/XENONnT/straxen/pull/1202
+        * Add rundoc URLConfig protocol by @jmosbacher in https://github.com/XENONnT/straxen/pull/1135
+        * Split event_area_per_channel into two plugins: event_area_per_channel… by @minzhong98 in https://github.com/XENONnT/straxen/pull/1191
+        * Fix event basics time ordering by @jjakob03 in https://github.com/XENONnT/straxen/pull/1194
+        * Make apply_xedocs_configs more flexible by @jmosbacher in https://github.com/XENONnT/straxen/pull/1204
+        * Try to make hashing more coinsistent by @LuisSanchez25 in https://github.com/XENONnT/straxen/pull/1201
+        
+        New Contributors
+        * @PeterGy made their first contribution in https://github.com/XENONnT/straxen/pull/1202
+        * @minzhong98 made their first contribution in https://github.com/XENONnT/straxen/pull/1191
+        
+        **Full Changelog**: https://github.com/XENONnT/straxen/compare/v2.0.7...v2.1.0
+        
+        
         v2.0.7 / 2023-04-25
         -------------------
-        ## What's Changed
         * Bootstrax target removal after failures by @cfuselli in https://github.com/XENONnT/straxen/pull/1145
         * reforming _raw_path and _processed_path by @FaroutYLq in https://github.com/XENONnT/straxen/pull/1149
         * Adding correction of Z position due to non-uniform drift velocity by @terliuk in https://github.com/XENONnT/straxen/pull/1148
         * Bump the versions of peaklets and quality check runs-on by @dachengx in https://github.com/XENONnT/straxen/pull/1153
         * S1-Based 3D Position Reconstruction by @matteoguida in https://github.com/XENONnT/straxen/pull/1146
         * Bump xedocs from 0.2.14 to 0.2.16 in /extra_requirements by @dependabot in https://github.com/XENONnT/straxen/pull/1158
         * Use zstd as compressor of peaks by @dachengx in https://github.com/XENONnT/straxen/pull/1154
         * Bump sphinx from 5.3.0 to 6.2.0 in /extra_requirements by @dependabot in https://github.com/XENONnT/straxen/pull/1161
         
-        ## New Contributors
+        New Contributors
         * @cfuselli made their first contribution in https://github.com/XENONnT/straxen/pull/1145
         * @matteoguida made their first contribution in https://github.com/XENONnT/straxen/pull/1146
         * @hmdyt made their first contribution in https://github.com/XENONnT/straxen/pull/1159
         
         **Full Changelog**: https://github.com/XENONnT/straxen/compare/v2.0.6...v2.0.7
         
         
         v2.0.6 / 2023-03-08
         -------------------
-        ## What's Changed
         * Bump supercharge/mongodb-github-action from 1.8.0 to 1.9.0 by @dependabot in https://github.com/XENONnT/straxen/pull/1140
         * Small patches to restrax module by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1143, d04a3428c52c159577b61af2a28ddd0af5652027, 602b807291211f083c8f54df6768b8198fbf6b55
         * Ms events by @michaweiss89 and @HenningSE in https://github.com/XENONnT/straxen/pull/1080
         
-        ## New Contributors
+        New Contributors
         * @michaweiss89 made their first contribution in https://github.com/XENONnT/straxen/pull/1080
         
         **Full Changelog**: https://github.com/XENONnT/straxen/compare/v2.0.5...v2.0.6
         
         Notes:
          - new data types: `peaks_per_event`, `event_top_bottom_params`, `peaks_corrections` (see #1080)
         
         
         v2.0.5 / 2023-02-24
         -------------------
-        ## What's Changed
         * fix xedocs for testing by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1139
         * Restart python style guide by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1138
         * Decrease number of chunks by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1123
         * Restrax by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1074
         
         
         **Full Changelog**: https://github.com/XENONnT/straxen/compare/v2.0.4...v2.0.5
@@ -1010,15 +1038,15 @@
         - Updated bin scripts like straxer (#204) 
         - Updated PMT gains (#208)
         - Renamed high energy plugins (#200)
         - Bugifx in nveto-plugins (#183, #209)
         - Bugfix in clean_up_empty_records (#210)
         
         
-        0.10.0 / 2020-08-187
+        0.10.0 / 2020-08-18
         --------------------
         - Neutron-veto integration (#86)
         - Processing for high energy channels (#161, #176)
         - Integrate rucio as storage backend (#164)
         - Remapping of old runs (#166)
         - Bootstrax/microstrax/ajax updates (#165)
         - Pull request template (#168)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `straxen-2.0.7/README.md` & `straxen-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/bin/ajax` & `straxen-2.1.0/bin/ajax`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/bin/bootstrax` & `straxen-2.1.0/bin/bootstrax`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/bin/fake_daq` & `straxen-2.1.0/bin/fake_daq`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/bin/microstrax` & `straxen-2.1.0/bin/microstrax`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/bin/refresh_raw_records` & `straxen-2.1.0/bin/refresh_raw_records`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/bin/restrax` & `straxen-2.1.0/bin/restrax`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/bin/straxen-print_versions` & `straxen-2.1.0/bin/straxen-print_versions`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/bin/straxer` & `straxen-2.1.0/bin/straxer`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/setup.cfg` & `straxen-2.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/setup.py` & `straxen-2.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 with open('README.md') as file:
     readme = file.read()
 
 with open('HISTORY.md') as file:
     history = file.read()
 
 setuptools.setup(name='straxen',
-                 version='2.0.7',
+                 version='2.1.0',
                  description='Streaming analysis for XENON',
                  author='Straxen contributors, the XENON collaboration',
                  url='https://github.com/XENONnT/straxen',
                  long_description=readme + '\n\n' + history,
                  long_description_content_type="text/markdown",
                  setup_requires=['pytest-runner'],
                  install_requires=requires,
```

### Comparing `straxen-2.0.7/straxen/__init__.py` & `straxen-2.1.0/straxen/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '2.0.7'
+__version__ = '2.1.0'
 
 from utilix import uconfig
 from .common import *
 # contexts.py below
 from .corrections_services import *
 from .get_corrections import *
```

### Comparing `straxen-2.0.7/straxen/analyses/bokeh_waveform_plot.py` & `straxen-2.1.0/straxen/analyses/bokeh_waveform_plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -876,16 +876,16 @@
         f.yaxis.axis_label = y_label
 
         self.selection_index = None
         s1.selected.js_on_change('indices',
                                  bokeh.models.CustomJS(args=dict(s1=s1), code=f"""
                 var inds = cb_obj.indices;
                 var kernel = IPython.notebook.kernel;
-                IPython.notebook.kernel.execute("{self.name}.selection_index = " + inds);
-            """)
+                kernel.execute("{self.name}.selection_index = " + inds);
+                """)
                                  )
         return f
 
     def get_back_selected_items(self):
         if not self.selection_index:
             raise ValueError('No data selection found. Have you selected any data? '
                              'If yes you most likely have not intialized the DataSelctor correctly. '
```

### Comparing `straxen-2.0.7/straxen/analyses/daq_waveforms.py` & `straxen-2.1.0/straxen/analyses/daq_waveforms.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/analyses/event_display.py` & `straxen-2.1.0/straxen/analyses/event_display.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/analyses/holoviews_waveform_display.py` & `straxen-2.1.0/straxen/analyses/holoviews_waveform_display.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/analyses/posrec_comparison.py` & `straxen-2.1.0/straxen/analyses/posrec_comparison.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/analyses/pulse_plots.py` & `straxen-2.1.0/straxen/analyses/pulse_plots.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/analyses/quick_checks.py` & `straxen-2.1.0/straxen/analyses/quick_checks.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/analyses/records_matrix.py` & `straxen-2.1.0/straxen/analyses/records_matrix.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/analyses/waveform_plot.py` & `straxen-2.1.0/straxen/analyses/waveform_plot.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/bokeh_utils.py` & `straxen-2.1.0/straxen/bokeh_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     :param fig: Figure to be conerted
     :param outputfile: String of absolute file path. If specified output
         is writen to the file. Else output is print to the notebook and
         can be simply copied into the wiki.
     """
     # convert plot to wiki format:
     html = file_html(fig, CDN)
-    html = '\n'.join((['<html>'] + html.split('\n')[6:]))
+    html = '\n'.join((['<html>'] + html.split('\n')[2:]))
 
     if outputfile:
         with open(outputfile, mode='w') as file:
             file.write(html)
     else:
         print(html)
```

### Comparing `straxen-2.0.7/straxen/common.py` & `straxen-2.1.0/straxen/common.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/contexts.py` & `straxen-2.1.0/straxen/contexts.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import straxen
 from copy import deepcopy
 from straxen import HAVE_ADMIX
 import os
 import warnings
 import typing as ty
 from pandas.util._decorators import deprecate_kwarg
+import socket
+
 
 common_opts = dict(
     register_all=[],
     # Register all peak/pulse processing by hand as 1T does not need to have
     # the high-energy plugins.
     register=[
         straxen.PulseProcessing,
@@ -91,28 +93,56 @@
 
 ##
 # XENONnT
 ##
 
 
 def xenonnt(cmt_version='global_ONLINE', xedocs_version=None,
-            _from_cutax=False,  **kwargs):
+            _from_cutax=False, **kwargs):
     """XENONnT context"""
     if not _from_cutax and cmt_version != 'global_ONLINE':
         warnings.warn('Don\'t load a context directly from straxen, '
                       'use cutax instead!')
     st = straxen.contexts.xenonnt_online(**kwargs)
     st.apply_cmt_version(cmt_version)
     
     if xedocs_version is not None:
-        st.apply_xedocs_configs(xedocs_version)
+        st.apply_xedocs_configs(version=xedocs_version, **kwargs)
 
     return st
 
 
+def find_rucio_local_path(include_rucio_local, _rucio_local_path):
+    """
+    Check the hostname to determine which rucio local path to use. Note that access to
+    /dali/lgrandi/rucio/ is possible only if you are on dali compute node or login node.
+
+    :param include_rucio_local: add the rucio local storage frontend.
+        This is only needed if one wants to do a fuzzy search in the
+        data the runs database is out of sync with rucio
+    :param _rucio_local_path: str, path of local RSE of rucio. Only use
+        for testing!
+    """
+    hostname = socket.gethostname()
+    # if you are on dali compute node, do nothing
+    if ('dali' in hostname) and ('login' not in hostname):
+        _include_rucio_local = include_rucio_local
+        __rucio_local_path = _rucio_local_path
+    # Assumed the only other option is 'midway' or login nodes, 
+    # where we have full access to dali and project space. 
+    # This doesn't make sense outside XENON but we don't care.
+    else:
+        _include_rucio_local = True
+        __rucio_local_path = '/project/lgrandi/rucio/'
+        print('You specified _auto_append_rucio_local=True and you are not on dali compute nodes,'
+              'so we will add the following rucio local path: ', __rucio_local_path)
+
+    return _include_rucio_local, __rucio_local_path
+
+
 @deprecate_kwarg('_minimum_run_number', 'minimum_run_number')
 @deprecate_kwarg('_maximum_run_number', 'maximum_run_number')
 @deprecate_kwarg('_include_rucio_remote', 'include_rucio_remote')
 @deprecate_kwarg('_add_online_monitor_frontend', 'include_online_monitor')
 def xenonnt_online(output_folder: str = './strax_data',
                    we_are_the_daq: bool = False,
                    minimum_run_number: int = 7157,
@@ -121,14 +151,15 @@
                    # Frontends
                    include_rucio_remote: bool = False,
                    include_online_monitor: bool = False,
                    include_rucio_local: bool = False,
 
                    # Frontend options
                    download_heavy: bool = False,
+                   _auto_append_rucio_local: bool = True,
                    _rucio_path: str = '/dali/lgrandi/rucio/',
                    _rucio_local_path: ty.Optional[str] = None,
                    _raw_paths: ty.Optional[str] = ['/dali/lgrandi/xenonnt/raw'],
                    _processed_paths: ty.Optional[ty.List[str]] = ['/dali/lgrandi/xenonnt/processed',
                                                                   '/project2/lgrandi/xenonnt/processed',
                                                                   '/project/lgrandi/xenonnt/processed'],
 
@@ -152,14 +183,16 @@
     :param include_online_monitor: add the online monitor storage frontend.
     :param include_rucio_local: add the rucio local storage frontend.
         This is only needed if one wants to do a fuzzy search in the
         data the runs database is out of sync with rucio
     :param download_heavy: bool, whether or not to allow downloads of
         heavy data (raw_records*, less the aqmon)
 
+    :param _auto_append_rucio_local: bool, whether or not to automatically append the 
+        rucio local path
     :param _rucio_path: str, path of rucio
     :param _rucio_local_path: str, path of local RSE of rucio. Only use
         for testing!
     :param _raw_paths: list[str], common path of the raw-data
     :param _processed_paths: list[str]. common paths of output data
     :param _context_config_overwrite: dict, overwrite config
     :param _database_init: bool, start the database (for testing)
@@ -175,14 +208,18 @@
     st = strax.Context(
         config=straxen.contexts.xnt_common_config,
         **context_options)
     st.register([straxen.DAQReader,
                  straxen.LEDCalibration,
                  straxen.LEDAfterpulseProcessing])
 
+    if _auto_append_rucio_local:
+        include_rucio_local, _rucio_local_path = find_rucio_local_path(
+            include_rucio_local, _rucio_local_path)
+
     st.storage = [
         straxen.RunDB(
             readonly=not we_are_the_daq,
             minimum_run_number=minimum_run_number,
             maximum_run_number=maximum_run_number,
             runid_field='number',
             new_data_path=output_folder,
```

### Comparing `straxen-2.0.7/straxen/corrections_services.py` & `straxen-2.1.0/straxen/corrections_services.py`

 * *Files 1% similar despite different names*

```diff
@@ -399,27 +399,34 @@
             raise CMTVersionError(msg)
 
     context.set_config(cmt_config)
 
 
 @strax.Context.add_method
 def apply_xedocs_configs(context: strax.Context, 
-                         version: str, db='straxen_db') -> None:
+                         db='straxen_db', **kwargs) -> None:
     import xedocs
 
-    docs = xedocs.find_docs('context_configs', 
-                            datasource=db, 
-                            version=version)
+    if isinstance(db, str):
+        func = getattr(xedocs.databases, db)
+        db_kwargs = straxen.filter_kwargs(func, kwargs)
+        db = func(**db_kwargs)
+
+    filter_kwargs = {k: v for k, v in kwargs.items()
+                        if k in db.context_configs.schema.__fields__}
+
+    docs = db.context_configs.find_docs(**filter_kwargs)
 
     global_config = {doc.config_name: doc.value for doc in docs}
     
     if len(global_config):
         context.set_config(global_config)
     else:
-        warnings.warn(f"Could not find any context configs for version {version}")
+        warnings.warn(f"Could not find any context configs matchin {filter_kwargs}",
+                      RuntimeWarning, stacklevel=2)
 
 
 def replace_url_version(url, version):
     """Replace the local version of a correction in a CMT config"""
     kwargs = {k: v[0] for k, v in parse_qs(urlparse(url).query).items()}
     kwargs['version'] = version
     args = [f"{k}={v}" for k, v in kwargs.items()]
```

### Comparing `straxen-2.0.7/straxen/daq_core.py` & `straxen-2.1.0/straxen/daq_core.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/entry_points.py` & `straxen-2.1.0/straxen/entry_points.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/get_corrections.py` & `straxen-2.1.0/straxen/get_corrections.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/holoviews/holoviews_inspector.py` & `straxen-2.1.0/straxen/holoviews/holoviews_inspector.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/holoviews/holoviews_peak_data.py` & `straxen-2.1.0/straxen/holoviews/holoviews_peak_data.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/holoviews/holoviews_pmt_array.py` & `straxen-2.1.0/straxen/holoviews/holoviews_pmt_array.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/holoviews/holoviews_tpc_event_display.py` & `straxen-2.1.0/straxen/holoviews/holoviews_tpc_event_display.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/holoviews_utils.py` & `straxen-2.1.0/straxen/holoviews_utils.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/itp_map.py` & `straxen-2.1.0/straxen/itp_map.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/legacy/contexts_1t.py` & `straxen-2.1.0/straxen/legacy/contexts_1t.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/legacy/hitfinder_thresholds.py` & `straxen-2.1.0/straxen/legacy/hitfinder_thresholds.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/legacy/plugins_1t/event_info.py` & `straxen-2.1.0/straxen/legacy/plugins_1t/event_info.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/legacy/plugins_1t/pax_interface.py` & `straxen-2.1.0/straxen/legacy/plugins_1t/pax_interface.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/legacy/plugins_1t/peak_positions.py` & `straxen-2.1.0/straxen/legacy/plugins_1t/peak_positions.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/legacy/plugins_1t/x1t_cuts.py` & `straxen-2.1.0/straxen/legacy/plugins_1t/x1t_cuts.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/legacy/xenon1t_url_configs.py` & `straxen-2.1.0/straxen/legacy/xenon1t_url_configs.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/matplotlib_utils.py` & `straxen-2.1.0/straxen/matplotlib_utils.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/mini_analysis.py` & `straxen-2.1.0/straxen/mini_analysis.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/misc.py` & `straxen-2.1.0/straxen/misc.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/numbafied_scipy.py` & `straxen-2.1.0/straxen/numbafied_scipy.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/plugins/__init__.py` & `straxen-2.1.0/straxen/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/plugins/afterpulses/afterpulse_processing.py` & `straxen-2.1.0/straxen/plugins/afterpulses/afterpulse_processing.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/plugins/aqmon_hits/aqmon_hits.py` & `straxen-2.1.0/straxen/plugins/aqmon_hits/aqmon_hits.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/plugins/defaults.py` & `straxen-2.1.0/straxen/plugins/defaults.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/plugins/detector_time_offsets/detector_time_offsets.py` & `straxen-2.1.0/straxen/plugins/detector_time_offsets/detector_time_offsets.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/plugins/events/__init__.py` & `straxen-2.1.0/straxen/plugins/events/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 
 from . import event_ambience
 from .event_ambience import *
 
 from . import event_area_per_channel
 from .event_area_per_channel import *
 
+from . import event_waveform
+from .event_waveform import *
+
 from . import event_top_bottom_params
 from .event_top_bottom_params import *
 
 from . import event_basics
 from .event_basics import *
 
 from . import event_info
@@ -42,24 +45,24 @@
 
 from . import s2_recon_pos_diff
 from .s2_recon_pos_diff import *
 
 from . import veto_proximity
 from .veto_proximity import *
 
-from . import event_s2_position_mlp
-from .event_s2_position_mlp import *
+from . import event_s2_positions_mlp
+from .event_s2_positions_mlp import *
 
-from . import event_s2_position_cnn
-from .event_s2_position_cnn import *
+from . import event_s2_positions_cnn
+from .event_s2_positions_cnn import *
 
-from . import event_s2_position_gcn
-from .event_s2_position_gcn import *
+from . import event_s2_positions_gcn
+from .event_s2_positions_gcn import *
 
-from . import event_s1_position_cnn
-from .event_s1_position_cnn import *
+from . import event_s1_positions_cnn
+from .event_s1_positions_cnn import *
 
 from . import local_minimum_info
 from .local_minimum_info import *
 
 from . import multi_scatter
 from .multi_scatter import *
```

### Comparing `straxen-2.0.7/straxen/plugins/events/_event_s1_position_base.py` & `straxen-2.1.0/straxen/plugins/events/_event_s1_positions_base.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/plugins/events/_event_s2_position_base.py` & `straxen-2.1.0/straxen/plugins/events/_event_s2_positions_base.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/plugins/events/corrected_areas.py` & `straxen-2.1.0/straxen/plugins/events/corrected_areas.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/plugins/events/distinct_channels.py` & `straxen-2.1.0/straxen/plugins/events/distinct_channels.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/plugins/events/energy_estimates.py` & `straxen-2.1.0/straxen/plugins/events/energy_estimates.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/plugins/events/event_ambience.py` & `straxen-2.1.0/straxen/plugins/events/event_ambience.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/plugins/events/event_area_per_channel.py` & `straxen-2.1.0/straxen/plugins/events/event_area_per_channel.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,76 +2,73 @@
 import strax
 import straxen
 
 export, __all__ = strax.exporter()
 
 
 @export
-class EventAreaPerChannel(strax.LoopPlugin):
+class EventAreaPerChannel(strax.Plugin):
     """
-    Simple plugin that provides area per channel, total (data) and top (data_top) 
-    waveforms for main and alternative S1/S2 in the event. 
+    Simple plugin that provides area per channel for main and alternative S1/S2 in the event.
     """
+    
     depends_on = ('event_basics', 'peaks')
     provides = "event_area_per_channel"
-    __version__ = '0.0.2'
+    __version__ = '0.1.0'
 
     compressor = 'zstd'
     save_when = strax.SaveWhen.EXPLICIT
 
     n_top_pmts = straxen.URLConfig(default=straxen.n_top_pmts, type=int, help="Number of top PMTs")
 
     def infer_dtype(self):
         # setting data type from peak dtype
-        pfields_=self.deps['peaks'].dtype_for('peaks').fields
-        ## Populating data type
-        infoline = {'s1': 'main S1', 
-                    's2': 'main S2', 
+        pfields_ = self.deps['peaks'].dtype_for('peaks').fields
+        # populating data type
+        infoline = {'s1': 'main S1',
+                    's2': 'main S2',
                     'alt_s1': 'alternative S1',
                     'alt_s2': 'alternative S2',
                    }
         dtype = []
-        # populating APC and waveform samples
+        # populating APC
         ptypes = ['s1', 's2', 'alt_s1', 'alt_s2']
         for type_ in ptypes:
-            dtype +=[((f'Area per channel for {infoline[type_]}', f'{type_}_area_per_channel'),
+            dtype += [((f'Area per channel for {infoline[type_]}', f'{type_}_area_per_channel'),
                      pfields_['area_per_channel'][0])]
-            dtype +=[((f'Waveform for {infoline[type_]} [ PE / sample ]', f'{type_}_data'),
-                     pfields_['data'][0])]
-            dtype +=[((f'Top waveform for {infoline[type_]} [ PE / sample ]', f'{type_}_data_top'),
-                     pfields_['data_top'][0])]
-            dtype +=[((f'Length of the interval in samples for {infoline[type_]}', f'{type_}_length'),
+            dtype += [((f'Length of the interval in samples for {infoline[type_]}', f'{type_}_length'),
                      pfields_['length'][0])]
-            dtype +=[((f'Width of one sample for {infoline[type_]} [ns]', f'{type_}_dt'),
+            dtype += [((f'Width of one sample for {infoline[type_]} [ns]', f'{type_}_dt'),
                      pfields_['dt'][0])]
         # populating S1 n channel properties
         dtype += [(("Main S1 count of contributing PMTs", "s1_n_channels"),
                   np.int16),
                  (("Main S1 top count of contributing PMTs", "s1_top_n_channels"),
                   np.int16),
                  (("Main S1 bottom count of contributing PMTs", "s1_bottom_n_channels"),
                   np.int16),
                  ]
         dtype += strax.time_fields
         return dtype
 
-    def compute_loop(self, event, peaks):
-        result = dict()
-        result['time'] = event['time']
-        result['endtime'] = strax.endtime(event)
-
-        for type_ in ['s1', 's2', 'alt_s1', 'alt_s2']:
-            type_index = event[f'{type_}_index']
-            if type_index != -1:
-                type_area_per_channel = peaks['area_per_channel'][type_index]
-                result[f'{type_}_area_per_channel'] = type_area_per_channel
-                result[f'{type_}_length'] = peaks['length'][type_index]
-                result[f'{type_}_data'] = peaks['data'][type_index]
-                result[f'{type_}_data_top'] = peaks['data_top'][type_index]
-                result[f'{type_}_dt'] = peaks['dt'][type_index]
-                if type_ == 's1':
-                    result['s1_n_channels'] = len(type_area_per_channel[type_area_per_channel > 0])
-                    result['s1_top_n_channels'] = len(type_area_per_channel[:self.config['n_top_pmts']][
-                                                          type_area_per_channel[:self.config['n_top_pmts']] > 0])
-                    result['s1_bottom_n_channels'] = len(type_area_per_channel[self.config['n_top_pmts']:][
-                                                             type_area_per_channel[self.config['n_top_pmts']:] > 0])
+    def compute(self, events, peaks):
+        result = np.zeros(len(events), self.dtype)
+        result['time'] = events['time']
+        result['endtime'] = strax.endtime(events)
+
+        split_peaks = strax.split_by_containment(peaks, events)
+        for event_i, (event, sp) in enumerate(zip(events, split_peaks)):
+            for type_ in ['s1', 's2', 'alt_s1', 'alt_s2']:
+                type_index = event[f'{type_}_index']
+                if type_index != -1:
+                    type_area_per_channel = sp['area_per_channel'][type_index]
+                    result[f'{type_}_area_per_channel'][event_i] = type_area_per_channel
+                    result[f'{type_}_length'][event_i] = sp['length'][type_index]
+                    result[f'{type_}_dt'][event_i] = sp['dt'][type_index]
+                    if type_ == 's1':
+                        result['s1_n_channels'][event_i] = (
+                            type_area_per_channel > 0).sum()
+                        result['s1_top_n_channels'][event_i] = (
+                            type_area_per_channel[:self.config['n_top_pmts']] > 0).sum()
+                        result['s1_bottom_n_channels'][event_i] = (
+                            type_area_per_channel[self.config['n_top_pmts']:] > 0).sum()
         return result
```

### Comparing `straxen-2.0.7/straxen/plugins/events/event_basics.py` & `straxen-2.1.0/straxen/plugins/events/event_basics.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
     The main S1 and alternative S1 are given by the largest two S1-Peaks
     within the event.
     The main S2 is given by the largest S2-Peak within the event, while
     alternative S2 is selected as the largest S2 other than main S2
     in the time window [main S1 time, main S1 time + max drift time].
     """
-    __version__ = '1.3.1'
+    __version__ = '1.3.3'
 
     depends_on = ('events',
                   'peak_basics',
                   'peak_positions',
                   'peak_proximity')
     provides = 'event_basics'
     data_kind = 'events'
@@ -73,14 +73,25 @@
                   ('event_number', np.int64,
                    'Event number in this dataset'),
                   ]
 
         dtype += self._get_si_dtypes(self.peak_properties)
 
         dtype += [
+            (f's1_max_diff', np.int32,
+             f'Main S1 largest time difference between apexes of hits [ns]'),
+            (f'alt_s1_max_diff', np.int32,
+             f'Alternate S1 largest time difference between apexes of hits [ns]'),
+            (f's1_min_diff', np.int32,
+             f'Main S1 smallest time difference between apexes of hits [ns]'),
+            (f'alt_s1_min_diff', np.int32,
+             f'Alternate S1 smallest time difference between apexes of hits [ns]'),
+        ]
+
+        dtype += [
             (f's2_x', np.float32,
              f'Main S2 reconstructed X position, uncorrected [cm]'),
             (f's2_y', np.float32,
              f'Main S2 reconstructed Y position, uncorrected [cm]'),
             (f'alt_s2_x', np.float32,
              f'Alternate S2 reconstructed X position, uncorrected [cm]'),
             (f'alt_s2_y', np.float32,
@@ -249,15 +260,17 @@
         self.set_event_properties(event, largest_s1s, largest_s2s, peaks)
 
         # Loop over S1s and S2s and over main / alt.
         for s_i, largest_s_i in enumerate([largest_s1s, largest_s2s], 1):
             # Largest index 0 -> main sx, 1 -> alt sx
             for largest_index, main_or_alt in enumerate(['s', 'alt_s']):
                 peak_properties_to_save = [name for name, _, _ in self.peak_properties]
-                if s_i == 2:
+                if s_i == 1:
+                    peak_properties_to_save += ['max_diff', 'min_diff']
+                elif s_i == 2:
                     peak_properties_to_save += ['x', 'y']
                     peak_properties_to_save += self.posrec_save
                 field_names = [f'{main_or_alt}{s_i}_{name}' for name in peak_properties_to_save]
                 self.copy_largest_peaks_into_event(event,
                                                    largest_s_i,
                                                    largest_index,
                                                    field_names,
@@ -272,16 +285,16 @@
             s2_after_s1 = largest_s2s['center_time'] > largest_s1s[0]['center_time']
             s2_before_max_drift_time = (largest_s2s['center_time']
                                         - largest_s1s[0]['center_time']) < 1.01 * drift_time_max
             mask = s2_after_s1 & s2_before_max_drift_time
             # The selection avoids main_S2
             mask[0] = True
             # Take main and the largest valid alt_S2
-            s2_idx, largest_s2s = s2_idx[mask][:2], largest_s2s[mask][:2]
-        return s2_idx, largest_s2s
+            s2_idx, largest_s2s = s2_idx[mask], largest_s2s[mask]
+        return s2_idx[:2], largest_s2s[:2]
 
     @staticmethod
     @numba.njit
     def set_event_properties(result, largest_s1s, largest_s2s, peaks):
         """Get properties like drift time and area before main S2"""
         # Compute drift times only if we have a valid S1-S2 pair
         if len(largest_s1s) > 0 and len(largest_s2s) > 0:
```

### Comparing `straxen-2.0.7/straxen/plugins/events/event_info.py` & `straxen-2.1.0/straxen/plugins/events/event_info.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/plugins/events/event_info_double.py` & `straxen-2.1.0/straxen/plugins/events/event_info_double.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/plugins/events/event_pattern_fit.py` & `straxen-2.1.0/straxen/plugins/events/event_pattern_fit.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/plugins/events/event_positions.py` & `straxen-2.1.0/straxen/plugins/events/event_positions.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
                 comment = f'Alternative S{s_i} interaction (rel. main S{int(2 * (1.5 - s_i) + s_i)}) {j}-position, field-distortion corrected (cm)'
                 field = f'alt_s{s_i}_{j}_fdc'
                 dtype += [(field, np.float32, comment)]
 
         for j in ['z']:
             comment = 'Interaction z-position, using mean drift velocity only (cm)'
             dtype += [(j, np.float32, comment)]
-            comment = 'Interaction z-position corrected to non-uniform drift velocity [ cm ]'
+            comment = 'Interaction z-position corrected to non-uniform drift velocity (cm)'
             dtype += [(j + "_dv_corr", np.float32, comment)]
             for s_i in [1, 2]:
                 comment = f'Alternative S{s_i} z-position (rel. main S{int(2 * (1.5 - s_i) + s_i)}), using mean drift velocity only (cm)'
                 field = f'alt_s{s_i}_z'
                 dtype += [(field, np.float32, comment)]
                 # values for corrected Z position
                 comment = f'Alternative S{s_i} z-position (rel. main S{[1 if s_i==2 else 2]}), corrected for non-uniform field (cm)'
```

### Comparing `straxen-2.0.7/straxen/plugins/events/event_s1_position_cnn.py` & `straxen-2.1.0/straxen/plugins/events/event_s2_positions_cnn.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 import strax
 import straxen
-from straxen.plugins.events._event_s1_position_base import EventS1PositionBase
+from straxen.plugins.events._event_s2_positions_base import EventS2PositionBase
 
 
 export, __all__ = strax.exporter()
 
 
 @export
-class EventS1PositionCNN(EventS1PositionBase):
+class EventS2PositionCNN(EventS2PositionBase):
     """
-    CNN for (x,y,z) position S1 reconstruction at event level
+    CNN for position S2 reconstruction at event level
     """
-    algorithm = "s1_cnn"
-    provides = "event_s1_position_cnn"
-    # tf_event_model_s1_cnn = straxen.URLConfig.evaluate_dry(f'tf:///project2/lgrandi/guidam/CNN_S1_XYZ_SAVED_MODELS/xnt_s1_posrec_cnn_datadriven_00_080921.tar.gz')
-    tf_event_model_s1_cnn = straxen.URLConfig(
+    algorithm = "cnn"
+    provides = "event_s2_positions_cnn"
+
+    tf_event_model_cnn = straxen.URLConfig(
         default=f'tf://'
                 f'resource://'
-                f'xedocs://posrec_models'
+                f'cmt://{algorithm}_model'
                 f'?version=ONLINE'
                 f'&run_id=plugin.run_id'
-                f'&kind=s1_cnn'
-                f'&fmt=abs_path'
-                f'&attr=value',
-        help='s1 position 3d reconstruction cnn model. Should be opened using the "tf" descriptor. '
+                f'&fmt=abs_path',
+        help='CNN model. Should be opened using the "tf" descriptor. '
              'Set to "None" to skip computation',
         cache=3,
-)
+    )
```

### Comparing `straxen-2.0.7/straxen/plugins/events/event_s2_position_cnn.py` & `straxen-2.1.0/straxen/plugins/peaks/peak_positions_mlp.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 import strax
 import straxen
-from straxen.plugins.events._event_s2_position_base import EventS2PositionBase
+from straxen.plugins.peaks._peak_positions_base import PeakPositionsBaseNT
 
 
 export, __all__ = strax.exporter()
 
 
 @export
-class EventS2PositionCNN(EventS2PositionBase):
-    """
-    CNN for position S2 reconstruction at event level
-    """
-    algorithm = "cnn"
-    provides = "event_s2_position_cnn"
+class PeakPositionsMLP(PeakPositionsBaseNT):
+    """Multilayer Perceptron (MLP) neural net for position reconstruction"""
+    provides = "peak_positions_mlp"
+    algorithm = "mlp"
 
-    tf_event_model_cnn = straxen.URLConfig(
+    tf_model_mlp = straxen.URLConfig(
         default=f'tf://'
                 f'resource://'
                 f'cmt://{algorithm}_model'
                 f'?version=ONLINE'
                 f'&run_id=plugin.run_id'
                 f'&fmt=abs_path',
-        help='CNN model. Should be opened using the "tf" descriptor. '
+        help='MLP model. Should be opened using the "tf" descriptor. '
              'Set to "None" to skip computation',
         cache=3,
     )
```

### Comparing `straxen-2.0.7/straxen/plugins/events/event_s2_position_gcn.py` & `straxen-2.1.0/straxen/plugins/events/event_s2_positions_gcn.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import strax
 import straxen
-from straxen.plugins.events._event_s2_position_base import EventS2PositionBase
+from straxen.plugins.events._event_s2_positions_base import EventS2PositionBase
 
 
 export, __all__ = strax.exporter()
 
 
 @export
 class EventS2PositionGCN(EventS2PositionBase):
     """
     GCN net for position S2 reconstruction at event level
     """
     algorithm = "gcn"
-    provides = "event_s2_position_gcn"
+    provides = "event_s2_positions_gcn"
 
     tf_event_model_gcn = straxen.URLConfig(
         default=f'tf://'
                 f'resource://'
                 f'cmt://{algorithm}_model'
                 f'?version=ONLINE'
                 f'&run_id=plugin.run_id'
```

### Comparing `straxen-2.0.7/straxen/plugins/events/event_s2_position_mlp.py` & `straxen-2.1.0/straxen/plugins/events/event_s2_positions_mlp.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import strax
 import straxen
-from straxen.plugins.events._event_s2_position_base import EventS2PositionBase
+from straxen.plugins.events._event_s2_positions_base import EventS2PositionBase
 
 
 export, __all__ = strax.exporter()
 
 
 @export
 class EventS2PositionMLP(EventS2PositionBase):
     """
     MLP neural net for S2 position reconstruction at event level
     """
     algorithm = "mlp"
-    provides = "event_s2_position_mlp"
+    provides = "event_s2_positions_mlp"
 
     tf_event_model_mlp = straxen.URLConfig(
         default=f'tf://'
                 f'resource://'
                 f'cmt://{algorithm}_model'
                 f'?version=ONLINE'
                 f'&run_id=plugin.run_id'
```

### Comparing `straxen-2.0.7/straxen/plugins/events/event_shadow.py` & `straxen-2.1.0/straxen/plugins/events/event_shadow.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/plugins/events/event_top_bottom_params.py` & `straxen-2.1.0/straxen/plugins/events/event_top_bottom_params.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 @export
 class EventTopBottomParams(strax.Plugin):
     """
     Pluging that computes timing characteristics of top and bottom waveforms 
     based on waveforms stored at event level for main/alt S1/S2
     """
-    depends_on = ('event_info', 'event_area_per_channel')
+    depends_on = ('event_info', 'event_waveform')
     provides = 'event_top_bottom_params'
     __version__ = '0.0.0'
     def infer_dtype(self):
         ## Populating data type information
         infoline = {'s1': 'main S1',
                     's2': 'main S2',
                     'alt_s1': 'alternative S1',
@@ -51,44 +51,44 @@
         peak_dtype = strax.peak_dtype(n_channels=straxen.n_tpc_pmts, digitize_top=False)
         for type_ in self.ptypes:
             for arr_ in self.arrs:
                 # in order to reuse the same definitions as in other parts, we create "fake peaks"
                 # based only on data from corresponding array
                 fpeaks_ = np.zeros(events.shape[0], dtype=peak_dtype)
                 if arr_ == 'top':
-                    fpeaks_['data']=events[f'{type_}_data_top']
-                    fpeaks_['area']=events[f'{type_}_area']*events[f'{type_}_area_fraction_top']
+                    fpeaks_['data'] = events[f'{type_}_data_top']
+                    fpeaks_['area'] = events[f'{type_}_area'] * events[f'{type_}_area_fraction_top']
                 elif arr_ == 'bot':
-                    fpeaks_['data']=(events[f'{type_}_data']-events[f'{type_}_data_top'])
-                    fpeaks_['area']=events[f'{type_}_area']*(1.-events[f'{type_}_area_fraction_top'])
+                    fpeaks_['data'] = (events[f'{type_}_data'] - events[f'{type_}_data_top'])
+                    fpeaks_['area'] = events[f'{type_}_area'] * (1.-events[f'{type_}_area_fraction_top'])
                 elif arr_ == 'tot':
                     # This one is ony
-                    fpeaks_['data']=events[f'{type_}_data']
-                    fpeaks_['area']=events[f'{type_}_area']
+                    fpeaks_['data'] = events[f'{type_}_data']
+                    fpeaks_['area'] = events[f'{type_}_area']
                 else:
-                    raise RuntimeError(f'Received unknown array type : '+ arr_)
-                fpeaks_['length']=events[f'{type_}_length']
-                fpeaks_['dt']=events[f'{type_}_dt']
+                    raise RuntimeError(f'Received unknown array type : ' + arr_)
+                fpeaks_['length'] = events[f'{type_}_length']
+                fpeaks_['dt'] = events[f'{type_}_dt']
                 # computing central times
                 # note that here we ignore 1/2 sample length to be consistent with other definitions
                 with np.errstate(divide='ignore', invalid='ignore'):
-                    recalc_ctime = np.sum(fpeaks_['data']*(np.arange(0, fpeaks_['data'].shape[1])), axis=1 )
-                    recalc_ctime/=fpeaks_['area']
-                    recalc_ctime*=fpeaks_['dt']
-                    recalc_ctime[~(fpeaks_['area']>0)]=0.0
+                    recalc_ctime = np.sum(fpeaks_['data'] * (np.arange(0, fpeaks_['data'].shape[1])), axis=1)
+                    recalc_ctime /= fpeaks_['area']
+                    recalc_ctime *= fpeaks_['dt']
+                    recalc_ctime[~(fpeaks_['area'] > 0)] = 0.0
                 # setting central times in the same way as inside peak processing
-                mask=(fpeaks_['area']>0)
-                result[f'{type_}_center_time_{arr_}']=events[f'{type_}_time']
-                result[f'{type_}_center_time_{arr_}'][mask]+=recalc_ctime[mask].astype(int)
+                mask = (fpeaks_['area'] > 0)
+                result[f'{type_}_center_time_{arr_}'] = events[f'{type_}_time']
+                result[f'{type_}_center_time_{arr_}'][mask] += recalc_ctime[mask].astype(int)
                 # computing widths ##
                 # zero or undefined area peaks should have nans
                 strax.compute_widths(fpeaks_)
-                result[f'{type_}_rise_time_{arr_}'][:]=np.nan
-                result[f'{type_}_rise_time_{arr_}'][mask]= -fpeaks_['area_decile_from_midpoint'][mask][:, 1]
-                result[f'{type_}_range_50p_area_{arr_}'][:]=np.nan
+                result[f'{type_}_rise_time_{arr_}'][:] = np.nan
+                result[f'{type_}_rise_time_{arr_}'][mask] = -fpeaks_['area_decile_from_midpoint'][mask][:, 1]
+                result[f'{type_}_range_50p_area_{arr_}'][:] = np.nan
                 result[f'{type_}_range_50p_area_{arr_}'][mask] = fpeaks_['width'][mask][:, 5]
-                result[f'{type_}_range_90p_area_{arr_}'][:]=np.nan
+                result[f'{type_}_range_90p_area_{arr_}'][:] = np.nan
                 result[f'{type_}_range_90p_area_{arr_}'][mask] = fpeaks_['width'][mask][:, 9]
             # Difference between center times of top and bottom arrays
             result[f'{type_}_center_time_diff_top_bot'] = (result[f'{type_}_center_time_top'] -
                                                             result[f'{type_}_center_time_bot'])
         return result
```

### Comparing `straxen-2.0.7/straxen/plugins/events/event_w_bayes_class.py` & `straxen-2.1.0/straxen/plugins/events/event_w_bayes_class.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/plugins/events/events.py` & `straxen-2.1.0/straxen/plugins/events/events.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/plugins/events/local_minimum_info.py` & `straxen-2.1.0/straxen/plugins/events/local_minimum_info.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/plugins/events/multi_scatter.py` & `straxen-2.1.0/straxen/plugins/events/multi_scatter.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,91 +1,123 @@
 import strax
 import straxen
 import numpy as np
 export, __all__ = strax.exporter()
 
+
 @export
 class EventInfoMS(strax.Plugin):
     """
-    Get the sum of s2 and s1,
-    Get the sum of cs2 inside the drift length. 
+    Plugin to collect multiple-scatter event observables
     """
-    __version__ = '0.0.1'
-    depends_on = ('event_info', 'peak_basics','peaks_per_event','peaks_corrections')
-    provides = 'event_MS_naive'
-
-    def infer_dtype(self):
-        dtype = []
-        dtype += [
-            ((f's1_sum'), np.float32),
-            ((f'cs1_multi'), np.float32),
-            ((f'cs1_multi_wo_timecorr'), np.float32),
-            ((f's2_sum'), np.float32),
-            ((f'cs2_sum'), np.float32),
-            ((f'cs2_wo_timecorr_sum'), np.float32),
-            ((f'cs2_wo_elifecorr_sum'), np.float32),
-            ((f'cs2_area_fraction_sum'), np.float32),
-            ((f'ces_sum'), np.float32),
-            ((f'e_charge_sum'), np.float32),
-             ]
-        dtype += strax.time_fields
-        return dtype
-
+    __version__ = '0.0.2'
+    depends_on = (
+        'event_info',
+        'peak_basics', 'peak_per_event', 'peak_corrections', 'peak_positions')
+    provides = 'event_ms_naive'
     save_when = strax.SaveWhen.TARGET
 
     # config options don't double cache things from the resource cache!
     g1 = straxen.URLConfig(
         default='bodega://g1?bodega_version=v2',
-        help="S1 gain in PE / photons produced",
+        help='S1 gain in PE / photons produced',
     )
     g2 = straxen.URLConfig(
         default='bodega://g2?bodega_version=v2',
-        help="S2 gain in PE / electrons produced",
+        help='S2 gain in PE / electrons produced',
     )
     lxe_w = straxen.URLConfig(
         default=13.7e-3,
-        help="LXe work function in quanta/keV"
+        help='LXe work function in quanta/keV'
     )
     electron_drift_velocity = straxen.URLConfig(
         default='cmt://'
                 'electron_drift_velocity'
                 '?version=ONLINE&run_id=plugin.run_id',
         cache=True,
         help='Vertical electron drift velocity in cm/ns (1e4 m/ms)'
     )
     max_drift_length = straxen.URLConfig(
         default=straxen.tpc_z, infer_type=False,
         help='Total length of the TPC from the bottom of gate to the '
-             'top of cathode wires [cm]', )
+             'top of cathode wires [cm]')
+
+    ms_window_fac = straxen.URLConfig(
+        default=1.01, type=(int, float),
+        help='Max drift time window to look for peaks in multiple scatter events'
+    )
+
+    def infer_dtype(self):
+        dtype = strax.time_fields + [
+            (('Sum of S1 areas in event',
+              's1_sum'), np.float32),
+            (('Corrected S1 area based on average position of S2s in event',
+              'cs1_multi'), np.float32),
+            (('Corrected S1 area based on average position of S2s in event before time-dep LY correction',
+              'cs1_multi_wo_timecorr'), np.float32),
+            (('Sum of S2 areas in event',
+              's2_sum'), np.float32),
+            (('Sum of corrected S2 areas in event',
+              'cs2_sum'), np.float32),
+            (('Sum of corrected S2 areas in event S2 before elife correction',
+              'cs2_wo_timecorr_sum'), np.float32),
+            (('Sum of corrected S2 areas in event before SEG/EE and elife corrections',
+              'cs2_wo_elifecorr_sum'), np.float32),
+            (('Average of S2 area fraction top in event',
+              'cs2_area_fraction_top_avg'), np.float32),
+            (('Sum of the energy estimates in event',
+              'ces_sum'), np.float32),
+            (('Sum of the charge estimates in event',
+              'e_charge_sum'), np.float32),
+            (('Average x position of S2s in event',
+              'x_avg'), np.float32),
+            (('Average y position of S2s in event',
+              'y_avg'), np.float32),
+            (('Average observed z position of energy deposits in event',
+              'z_obs_avg'), np.float32),
+            (('Number of S2s in event',
+              'multiplicity'), np.int32),
+        ]
+        return dtype
+
     def setup(self):
         self.drift_time_max = int(self.max_drift_length / self.electron_drift_velocity)
+
     def cs1_to_e(self, x):
         return self.lxe_w * x / self.g1
 
     def cs2_to_e(self, x):
         return self.lxe_w * x / self.g2
 
-    
     def compute(self, events, peaks):
         split_peaks = strax.split_by_containment(peaks, events)
         result = np.zeros(len(events), self.infer_dtype())
-        #result['s2_sum'] = np.zeros(len(events))
-   
-         #1. Assign peaks features to main S1 and main S2 in the event
+
+        # Assign peaks features to main S1 and main S2 in the event
         for event_i, (event, sp) in enumerate(zip(events, split_peaks)):
-            cond = (sp["type"]==2)&(sp["drift_time"]>0)&(sp["drift_time"]< 1.01 * self.drift_time_max)&(sp["cs2"]>0)
-            result[f's2_sum'][event_i] = np.sum(sp[cond]['area'])
-            result[f'cs2_sum'][event_i] = np.sum(sp[cond]['cs2'])
-            result[f'cs2_wo_timecorr_sum'][event_i] = np.sum(sp[cond]['cs2_wo_timecorr'])
-            result[f'cs2_wo_elifecorr_sum'][event_i] = np.sum(sp[cond]['cs2_wo_elifecorr'])
-            result[f'cs2_area_fraction_sum'][event_i] = np.sum(sp[cond]['cs2_area_fraction_top'])            
-            result[f's1_sum'][event_i] = np.sum(sp[sp["type"]==1]['area'])
+            cond = (sp['type'] == 2) & (sp['drift_time'] > 0)
+            cond &= (sp['drift_time'] < self.ms_window_fac * self.drift_time_max) & (sp['cs2'] > 0)
+            result['s2_sum'][event_i] = np.nansum(sp[cond]['area'])
+            result['cs2_sum'][event_i] = np.nansum(sp[cond]['cs2'])
+            result['cs2_wo_timecorr_sum'][event_i] = np.nansum(sp[cond]['cs2_wo_timecorr'])
+            result['cs2_wo_elifecorr_sum'][event_i] = np.nansum(sp[cond]['cs2_wo_elifecorr'])         
+            result['s1_sum'][event_i] = np.nansum(sp[sp['type'] == 1]['area'])
+
             if np.sum(sp[cond]['cs2']) > 0: 
-                result[f'cs1_multi_wo_timecorr'][event_i] = event["s1_area"] * np.average(sp[cond]['s1_xyz_correction_factor'], weights = sp[cond]['cs2'])
-                result[f'cs1_multi'][event_i] = result[f'cs1_multi_wo_timecorr'][event_i] * np.average(sp[cond]['s1_rel_light_yield_correction_factor'], weights = sp[cond]['cs2'])
-        el = self.cs1_to_e(result[f'cs1_multi'])
-        ec = self.cs2_to_e(result[f'cs2_sum'])
-        result[f'ces_sum'] = el+ec
-        result[f'e_charge_sum'] = ec
+                result['cs1_multi_wo_timecorr'][event_i] = event['s1_area'] * np.average(
+                    sp[cond]['s1_xyz_correction_factor'], weights=sp[cond]['cs2'])
+                result['cs1_multi'][event_i] = result['cs1_multi_wo_timecorr'][event_i] * np.average(
+                    sp[cond]['s1_rel_light_yield_correction_factor'], weights=sp[cond]['cs2'])
+                result['x_avg'][event_i] = np.average(sp[cond]['x'], weights=sp[cond]['cs2'])
+                result['y_avg'][event_i] = np.average(sp[cond]['y'], weights=sp[cond]['cs2'])
+                result['z_obs_avg'][event_i] = np.average(sp[cond]['z_obs_ms'], weights=sp[cond]['cs2'])
+                result['cs2_area_fraction_top_avg'][event_i] = np.average(
+                    sp[cond]['cs2_area_fraction_top'], weights=sp[cond]['cs2'])   
+                result['multiplicity'][event_i] = len(sp[cond]['area'])
+
+        el = self.cs1_to_e(result['cs1_multi'])
+        ec = self.cs2_to_e(result['cs2_sum'])
+        result['ces_sum'] = el + ec
+        result['e_charge_sum'] = ec
         result['time'] = events['time']
         result['endtime'] = strax.endtime(events)
         return result
```

### Comparing `straxen-2.0.7/straxen/plugins/events/s2_recon_pos_diff.py` & `straxen-2.1.0/straxen/plugins/events/s2_recon_pos_diff.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/plugins/events/veto_proximity.py` & `straxen-2.1.0/straxen/plugins/events/veto_proximity.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 @export
 class VetoProximity(strax.OverlapWindowPlugin):
     """
     Find the closest next/previous veto start w.r.t. the event time or
     when a busy happens during an event.
     """
 
-    __version__ = '2.1.0'
+    __version__ = '2.2.0'
     # Strictly speaking, we could depend on 'events', but then you couldn't
     # change the event_window_fields to e.g. s1_time and s2_endtime.
     depends_on = ('event_basics', 'veto_intervals')
     provides = 'veto_proximity'
     data_kind = 'events'
 
     event_window_fields = straxen.URLConfig(
@@ -87,65 +87,50 @@
         # Set defaults to be some very long time
         result_buffer[f'time_to_previous_{veto_name}'] = self.time_no_aqmon_veto_found
         result_buffer[f'time_to_next_{veto_name}'] = self.time_no_aqmon_veto_found
 
         selected_intervals = veto_intervals[veto_intervals['veto_type'] == f'{veto_name}_veto']
         if not len(selected_intervals):
             return
-
+        
         vetos_during_event = strax.touching_windows(selected_intervals,
                                                     event_window)
-
+        
         # Figure out the vetos *during* an event
+        res = self.get_overlapping_window_time(vetos_during_event, selected_intervals, event_window, result_buffer)
+        result_buffer[f'veto_{veto_name}_overlap'] = res
+        
+        # Find the next and previous veto's
+        times_to_prev, times_to_next = strax.abs_time_to_prev_next_interval(event_window, selected_intervals)
+        mask_prev = times_to_prev > 0
+        result_buffer[f'time_to_previous_{veto_name}'][mask_prev] = times_to_prev[mask_prev]
+
+        max_next = times_to_next > 0
+        result_buffer[f'time_to_next_{veto_name}'][max_next] = times_to_next[max_next]
+      
+    @staticmethod
+    @numba.njit
+    def get_overlapping_window_time(vetos_during_event, selected_intervals, event_window, result_buffer):
+        """Computes total time each event overlaps with the corresponding veto.
+        """
+        res = np.zeros(len(vetos_during_event), np.int64)
+        
         for event_i, veto_window in enumerate(vetos_during_event):
             if veto_window[1] - veto_window[0]:
                 vetos_in_window = selected_intervals[veto_window[0]:
                                                      veto_window[1]].copy()
                 starts = np.clip(vetos_in_window['time'],
                                  event_window[event_i]['time'],
                                  event_window[event_i]['endtime'])
                 stops = np.clip(vetos_in_window['endtime'],
                                 event_window[event_i]['time'],
                                 event_window[event_i]['endtime'])
-                # Now sum over all the stops-starts that are clipped
-                # within the duration of the event
-                result_buffer[event_i][f'veto_{veto_name}_overlap'] = np.sum(stops -
-                                                                             starts)
-
-        # Find the next and previous veto's
-        times_to_prev, times_to_next = self.abs_time_to_prev_next(event_window, selected_intervals)
-        mask_prev = times_to_prev > 0
-        result_buffer[f'time_to_previous_{veto_name}'][mask_prev] = times_to_prev[mask_prev]
-
-        max_next = times_to_next > 0
-        result_buffer[f'time_to_next_{veto_name}'][max_next] = times_to_next[max_next]
-
-    @staticmethod
-    @numba.njit
-    def abs_time_to_prev_next(event_window, selected_intervals):
-        """Get the absolute time to the previous and the next interval"""
-        times_to_prev = np.ones(len(event_window)) * -1
-        times_to_next = np.ones(len(event_window)) * -1
-        for event_i, ev_wind in enumerate(event_window):
-            # Two cases left, either veto's are before or after the event window
-            interval_before = selected_intervals['endtime'] < ev_wind['time']
-            interval_after = selected_intervals['time'] > ev_wind['endtime']
-
-            if np.sum(interval_before):
-                prev_intervals = selected_intervals[interval_before]
-                time_to_prev = np.abs(ev_wind['time'] - prev_intervals['endtime'])
-                prev_idx = np.argmin(time_to_prev)
-                times_to_prev[event_i] = time_to_prev[prev_idx]
-
-            if np.sum(interval_after):
-                next_intervals = selected_intervals[interval_after]
-                time_to_next = np.abs(next_intervals['endtime'] - ev_wind['endtime'])
-                next_idx = np.argmin(time_to_next)
-                times_to_next[event_i] = time_to_next[next_idx]
-        return times_to_prev, times_to_next
+                
+                res[event_i] = np.sum(stops - starts)
+        return res
 
     def compute(self, events, veto_intervals):
         result = np.zeros(len(events), self.dtype)
         result['time'] = events['time']
         result['endtime'] = events['endtime']
 
         # Get containers for touching windows based on self.event_window_fields
```

### Comparing `straxen-2.0.7/straxen/plugins/events_mv/events_mv.py` & `straxen-2.1.0/straxen/plugins/events_mv/events_mv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/plugins/events_mv/events_sync_mv.py` & `straxen-2.1.0/straxen/plugins/events_mv/events_sync_mv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/plugins/events_nv/event_positions_nv.py` & `straxen-2.1.0/straxen/plugins/events_nv/event_positions_nv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/plugins/events_nv/events_nv.py` & `straxen-2.1.0/straxen/plugins/events_nv/events_nv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/plugins/events_nv/events_sync_nv.py` & `straxen-2.1.0/straxen/plugins/events_nv/events_sync_nv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/plugins/hitlets_mv/hitlets_mv.py` & `straxen-2.1.0/straxen/plugins/hitlets_mv/hitlets_mv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/plugins/hitlets_nv/hitlets_nv.py` & `straxen-2.1.0/straxen/plugins/hitlets_nv/hitlets_nv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/plugins/individual_peak_monitor/individual_peak_monitor.py` & `straxen-2.1.0/straxen/plugins/individual_peak_monitor/individual_peak_monitor.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/plugins/led_cal/led_calibration.py` & `straxen-2.1.0/straxen/plugins/led_cal/led_calibration.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/plugins/merged_s2s/merged_s2s.py` & `straxen-2.1.0/straxen/plugins/merged_s2s/merged_s2s.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 @export
 class MergedS2s(strax.OverlapWindowPlugin):
     """
     Merge together peaklets if peak finding favours that they would
     form a single peak instead.
     """
-    __version__ = '1.0.0'
+    __version__ = '1.0.2'
 
     depends_on = ('peaklets', 'peaklet_classification', 'lone_hits')
     data_kind = 'merged_s2s'
     provides = 'merged_s2s'
 
     s2_merge_max_duration = straxen.URLConfig(
         default=50_000, infer_type=False,
@@ -98,15 +98,16 @@
             areas=peaklets['area'],
             types=peaklets['type'],
             gap_thresholds=gap_thresholds,
             max_duration=self.s2_merge_max_duration,
             max_gap=max_gap,
             max_area=max_area,
         )
-        assert 'data_top'  in peaklets.dtype.names
+
+        assert 'data_top' in peaklets.dtype.names
 
         merged_s2s = strax.merge_peaks(
             peaklets,
             start_merge_at, end_merge_at,
             max_buffer=int(self.s2_merge_max_duration // np.gcd.reduce(peaklets['dt'])),
         )
         merged_s2s['type'] = 2
@@ -129,15 +130,16 @@
             merged_s2s = drop_data_top_field(merged_s2s, self.dtype, '_drop_top_merged_s2s')
         return merged_s2s
 
     @staticmethod
     @numba.njit(cache=True, nogil=True)
     def get_merge_instructions(
             peaklet_starts, peaklet_ends, areas, types,
-            gap_thresholds, max_duration, max_gap, max_area):
+            gap_thresholds, max_duration, max_gap, max_area,
+            sort_kind='mergesort'):
         """
         Finding the group of peaklets to merge. To do this start with the
         smallest gaps and keep merging until the new, merged S2 has such a
         large area or gap to adjacent peaks that merging is not required
         anymore.
         see https://github.com/XENONnT/straxen/pull/548 and https://github.com/XENONnT/straxen/pull/568
 
@@ -145,15 +147,15 @@
         list of the exclusive last index of peaklet to be merged
         """
 
         peaklet_gaps = peaklet_starts[1:] - peaklet_ends[:-1]
         peaklet_start_index = np.arange(len(peaklet_starts))
         peaklet_end_index = np.arange(len(peaklet_starts))
 
-        for gap_i in np.argsort(peaklet_gaps):
+        for gap_i in np.argsort(peaklet_gaps, kind=sort_kind):
             start_idx = peaklet_start_index[gap_i]
             inclusive_end_idx = peaklet_end_index[gap_i + 1]
             sum_area = np.sum(areas[start_idx:inclusive_end_idx + 1])
             this_gap = peaklet_gaps[gap_i]
 
             if inclusive_end_idx < start_idx:
                 raise ValueError('Something went wrong, left is bigger then right?!')
```

### Comparing `straxen-2.0.7/straxen/plugins/merged_s2s_he/merged_s2s_he.py` & `straxen-2.1.0/straxen/plugins/merged_s2s_he/merged_s2s_he.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/plugins/online_monitor_mv/online_monitor_mv.py` & `straxen-2.1.0/straxen/plugins/online_monitor_mv/online_monitor_mv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/plugins/online_monitor_nv/online_monitor_nv.py` & `straxen-2.1.0/straxen/plugins/online_monitor_nv/online_monitor_nv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/plugins/online_peak_monitor/online_peak_monitor.py` & `straxen-2.1.0/straxen/plugins/online_peak_monitor/online_peak_monitor.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/plugins/peaklets/peaklet_classification.py` & `straxen-2.1.0/straxen/plugins/peaklets/peaklet_classification.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/plugins/peaklets/peaklets.py` & `straxen-2.1.0/straxen/plugins/peaklets/peaklets.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numba
 import numpy as np
 import strax
 from immutabledict import immutabledict
 from strax.processing.general import _touching_windows
+from strax.dtypes import DIGITAL_SUM_WAVEFORM_CHANNEL
 import straxen
 
 
 export, __all__ = strax.exporter()
 
 
 @export
@@ -33,15 +34,15 @@
     depends_on = ('records',)
     provides = ('peaklets', 'lone_hits')
     data_kind = dict(peaklets='peaklets',
                      lone_hits='lone_hits')
     parallel = 'process'
     compressor = 'zstd'
 
-    __version__ = '1.0.1'
+    __version__ = '1.1.0'
 
     peaklet_gap_threshold = straxen.URLConfig(
         default=700, infer_type=False,
         help="No hits for this many ns triggers a new peak")
 
     peak_left_extension = straxen.URLConfig(
         default=30, infer_type=False,
@@ -225,17 +226,16 @@
         # Transform hits to hitlets for naming conventions. A hit refers
         # to the central part above threshold a hitlet to the entire signal
         # including the left and right extension.
         # (We are not going to use the actual hitlet data_type here.)
         hitlets = hits
         del hits
 
-        hitlet_time_shift = (hitlets['left'] - hitlets['left_integration']) * hitlets['dt']
-        hitlets['time'] = hitlets['time'] - hitlet_time_shift
-        hitlets['length'] = (hitlets['right_integration'] - hitlets['left_integration'])
+        hitlets['time'] -= (hitlets['left'] - hitlets['left_integration']) * hitlets['dt']
+        hitlets['length'] = hitlets['right_integration'] - hitlets['left_integration']
         hitlets = strax.sort_by_time(hitlets)
         rlinks = strax.record_links(records)
 
         # If sum_waveform_top_array is false, don't digitize the top array
         n_top_pmts_if_digitize_top = self.n_top_pmts if self.sum_waveform_top_array else -1
         strax.sum_waveform(peaklets, hitlets, r, rlinks, self.to_pe, n_top_channels=n_top_pmts_if_digitize_top)
 
@@ -271,36 +271,39 @@
                 min_reference_length=self.saturation_min_reference_length,
                 n_top_channels=n_top_pmts_if_digitize_top,
             )
 
             # Compute the width again for corrected peaks
             strax.compute_widths(peaklets, select_peaks_indices=peak_list)
 
+        hitlet_time_shift = (hitlets['left'] - hitlets['left_integration']) * hitlets['dt']
+        hit_max_times = hitlets['time'] + hitlet_time_shift  # add time shift again to get correct maximum
+        hit_max_times += hitlets['dt'] * hit_max_sample(records, hitlets)
+
         # Compute tight coincidence level.
         # Making this a separate plugin would
         # (a) doing hitfinding yet again (or storing hits)
         # (b) increase strax memory usage / max_messages,
         #     possibly due to its currently primitive scheduling.
-        hit_max_times = np.sort(
-            hitlets['time']
-            + hitlets['dt'] * hit_max_sample(records, hitlets)
-            + hitlet_time_shift  # add time shift again to get correct maximum
-        )
+        hit_max_times_argsort = np.argsort(hit_max_times)
+        sorted_hit_max_times = hit_max_times[hit_max_times_argsort]
+        sorted_hit_channels = hitlets['channel'][hit_max_times_argsort]
         peaklet_max_times = (
-                peaklets['time']
-                + np.argmax(peaklets['data'], axis=1) * peaklets['dt'])
-        tight_coincidence_channel = get_tight_coin(
-            hit_max_times,
-            hitlets['channel'],
+            peaklets['time']
+            + np.argmax(peaklets['data'], axis=1) * peaklets['dt'])
+        peaklets['tight_coincidence'] = get_tight_coin(
+            sorted_hit_max_times,
+            sorted_hit_channels,
             peaklet_max_times,
             self.tight_coincidence_window_left,
             self.tight_coincidence_window_right,
             self.channel_range)
 
-        peaklets['tight_coincidence'] = tight_coincidence_channel
+        # Add max and min time difference between apexes of hits
+        self.add_hit_features(hitlets, hit_max_times, peaklets)
 
         if self.diagnose_sorting and len(r):
             assert np.diff(r['time']).min(initial=1) >= 0, "Records not sorted"
             assert np.diff(hitlets['time']).min(initial=1) >= 0, "Hits/Hitlets not sorted"
             assert np.all(peaklets['time'][1:]
                           >= strax.endtime(peaklets)[:-1]), "Peaks not disjoint"
 
@@ -309,14 +312,24 @@
         counts = np.diff(counts, axis=1).flatten()
         peaklets['n_hits'] = counts
 
         # Drop the data_top field
         if n_top_pmts_if_digitize_top <= 0:
             peaklets = drop_data_top_field(peaklets, self.dtype_for('peaklets'))
 
+        # Check channel of peaklets
+        peaklets_unique_channel = np.unique(peaklets['channel'])
+        if (peaklets_unique_channel == DIGITAL_SUM_WAVEFORM_CHANNEL).sum() > 1:
+            raise ValueError(
+                f'Found channel number of peaklets other than {DIGITAL_SUM_WAVEFORM_CHANNEL}')
+        # Check tight_coincidence
+        if not np.all(peaklets['n_hits'] >= peaklets['tight_coincidence']):
+            raise ValueError(
+                f'Found n_hits less than tight_coincidence')
+
         return dict(peaklets=peaklets,
                     lone_hits=lone_hits)
 
     def natural_breaks_threshold(self, peaks):
         rise_time = -peaks['area_decile_from_midpoint'][:, 1]
 
         # This is ~1 for an clean S2, ~0 for a clean S1,
@@ -363,14 +376,39 @@
         outside_peaks[0]['endtime'] = peaklets[0]['time']
         outside_peaks[1:-1]['time'] = strax.endtime(peaklets[:-1])
         outside_peaks[1:-1]['endtime'] = peaklets['time'][1:]
         outside_peaks[-1]['time'] = strax.endtime(peaklets[-1])
         outside_peaks[-1]['endtime'] = end
         return outside_peaks
 
+    @staticmethod
+    def add_hit_features(hitlets, hit_max_times, peaklets):
+        """
+        Create hits timing features
+        :param hitlets_max: hitlets with only max height time.
+        :param peaklets: Peaklets for which intervals should be computed.
+        :return: array of peaklet_timing dtype.
+        """
+        hits_w_max = np.zeros(
+            len(hitlets),
+            strax.merged_dtype(
+                [np.dtype([('max_time', np.int64)]), np.dtype(strax.time_fields)]))
+        hits_w_max['time'] = hitlets['time']
+        hits_w_max['endtime'] = strax.endtime(hitlets)
+        hits_w_max['max_time'] = hit_max_times
+        split_hits = strax.split_by_containment(hits_w_max, peaklets)
+        for peaklet, h_max in zip(peaklets, split_hits):
+            max_time_diff = np.diff(np.sort(h_max['max_time']))
+            if len(max_time_diff) > 0:
+                peaklet['max_diff'] = max_time_diff.max()
+                peaklet['min_diff'] = max_time_diff.min()
+            else:
+                peaklet['max_diff'] = -1
+                peaklet['min_diff'] = -1
+
 def drop_data_top_field(peaklets, goal_dtype, _name_function= '_drop_data_top_field'):
     """Return peaklets without the data_top field"""
     peaklets_without_top_field = np.zeros(len(peaklets), dtype=goal_dtype)
     strax.copy_to_buffer(peaklets, peaklets_without_top_field, _name_function)
     del peaklets
     return peaklets_without_top_field
```

### Comparing `straxen-2.0.7/straxen/plugins/peaklets_he/peaklet_classification_he.py` & `straxen-2.1.0/straxen/plugins/peaklets_he/peaklet_classification_he.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/plugins/peaklets_he/peaklets_he.py` & `straxen-2.1.0/straxen/plugins/peaklets_he/peaklets_he.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/plugins/peaks/__init__.py` & `straxen-2.1.0/straxen/plugins/peaks/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 from . import peak_basics
 from .peak_basics import *
 
 from . import peak_classification_bayes
 from .peak_classification_bayes import *
 
-from . import peak_s1_position_cnn
-from .peak_s1_position_cnn import *
+from . import peak_s1_positions_cnn
+from .peak_s1_positions_cnn import *
 
 from . import peak_positions
 from .peak_positions import *
 
 from . import peak_positions_cnn
 from .peak_positions_cnn import *
 
@@ -30,12 +30,15 @@
 
 from . import peak_shadow
 from .peak_shadow import *
 
 from . import peaks
 from .peaks import *
 
-from . import peaks_per_event
-from .peaks_per_event import *
+from . import peak_per_event
+from .peak_per_event import *
 
-from . import peaks_corrections
-from .peaks_corrections import *
+from . import peak_corrections
+from .peak_corrections import *
+
+from . import peaks_subtyping
+from .peaks_subtyping import *
```

### Comparing `straxen-2.0.7/straxen/plugins/peaks/_peak_positions_base.py` & `straxen-2.1.0/straxen/plugins/peaks/_peak_positions_base.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/plugins/peaks/_peak_s1_position_base.py` & `straxen-2.1.0/straxen/plugins/peaks/_peak_s1_positions_base.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/plugins/peaks/peak_ambience.py` & `straxen-2.1.0/straxen/plugins/peaks/peak_ambience.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/plugins/peaks/peak_basics.py` & `straxen-2.1.0/straxen/plugins/peaks/peak_basics.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 @export
 class PeakBasics(strax.Plugin):
     """
     Compute the basic peak-properties, thereby dropping structured
     arrays.
     NB: This plugin can therefore be loaded as a pandas DataFrame.
     """
-    __version__ = "0.1.3"
+    __version__ = '0.1.4'
     parallel = True
     depends_on = ('peaks',)
     provides = 'peak_basics'
     dtype = [
         (('Start time of the peak (ns since unix epoch)',
           'time'), np.int64),
         (('End time of the peak (ns since unix epoch)',
@@ -49,30 +49,35 @@
         (('Time resolution of the peak waveform in ns',
           'dt'), np.int16),
         (('Time between 10% and 50% area quantiles [ns]',
           'rise_time'), np.float32),
         (('Number of PMTs with hits within tight range of mean',
           'tight_coincidence'), np.int16),
         (('Classification of the peak(let)',
-          'type'), np.int8)
+          'type'), np.int8),
+        (('Largest time difference between apexes of hits inside peak [ns]',
+          'max_diff'), np.int32),
+        (('Smallest time difference between apexes of hits inside peak [ns]',
+          'min_diff'), np.int32),
     ]
 
     n_top_pmts = straxen.URLConfig(default=straxen.n_top_pmts, infer_type=False,
                                    help="Number of top PMTs")
 
     check_peak_sum_area_rtol = straxen.URLConfig(default=None, track=False, infer_type=False,
                                                  help="Check if the sum area and the sum of area per "
                                                       "channel are the same. If None, don't do the "
                                                       "check. To perform the check, set to the desired "
                                                       " rtol value used e.g. '1e-4' (see np.isclose).")
 
     def compute(self, peaks):
         p = peaks
         r = np.zeros(len(p), self.dtype)
-        for q in 'time length dt area type'.split():
+        needed_fields = 'time length dt area type max_diff min_diff'
+        for q in needed_fields.split():
             r[q] = p[q]
         r['endtime'] = p['time'] + p['dt'] * p['length']
         r['n_channels'] = (p['area_per_channel'] > 0).sum(axis=1)
         r['n_hits'] = p['n_hits']
         r['range_50p_area'] = p['width'][:, 5]
         r['range_90p_area'] = p['width'][:, 9]
         r['max_pmt'] = np.argmax(p['area_per_channel'], axis=1)
```

### Comparing `straxen-2.0.7/straxen/plugins/peaks/peak_classification_bayes.py` & `straxen-2.1.0/straxen/plugins/peaks/peak_classification_bayes.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/plugins/peaks/peak_positions.py` & `straxen-2.1.0/straxen/plugins/peaks/peak_positions.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/plugins/peaks/peak_positions_gcn.py` & `straxen-2.1.0/straxen/plugins/peaks/peak_positions_gcn.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/plugins/peaks/peak_positions_mlp.py` & `straxen-2.1.0/straxen/plugins/peaks/peak_positions_cnn.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,23 +3,24 @@
 from straxen.plugins.peaks._peak_positions_base import PeakPositionsBaseNT
 
 
 export, __all__ = strax.exporter()
 
 
 @export
-class PeakPositionsMLP(PeakPositionsBaseNT):
-    """Multilayer Perceptron (MLP) neural net for position reconstruction"""
-    provides = "peak_positions_mlp"
-    algorithm = "mlp"
+class PeakPositionsCNN(PeakPositionsBaseNT):
+    """Convolutional Neural Network (CNN) neural net for position reconstruction"""
+    provides = "peak_positions_cnn"
+    algorithm = "cnn"
+    __version__ = '0.0.1'
 
-    tf_model_mlp = straxen.URLConfig(
+    tf_model_cnn = straxen.URLConfig(
         default=f'tf://'
                 f'resource://'
                 f'cmt://{algorithm}_model'
                 f'?version=ONLINE'
                 f'&run_id=plugin.run_id'
                 f'&fmt=abs_path',
-        help='MLP model. Should be opened using the "tf" descriptor. '
+        help='CNN model. Should be opened using the "tf" descriptor. '
              'Set to "None" to skip computation',
         cache=3,
     )
```

### Comparing `straxen-2.0.7/straxen/plugins/peaks/peak_proximity.py` & `straxen-2.1.0/straxen/plugins/peaks/peak_proximity.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/plugins/peaks/peak_s1_position_cnn.py` & `straxen-2.1.0/straxen/plugins/peaks/peak_s1_positions_cnn.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 import strax
 import straxen
-from straxen.plugins.peaks._peak_s1_position_base import PeakS1PositionBase
+from straxen.plugins.peaks._peak_s1_positions_base import PeakS1PositionBase
 
 
 export, __all__ = strax.exporter()
 
 
 @export
 class PeakS1PositionCNN(PeakS1PositionBase):
     """
     S1 CNN for (x,y,z) position S1 reconstruction at peak level
     """
-    provides = "peak_s1_position_cnn"
+    provides = "peak_s1_positions_cnn"
     algorithm = "s1_cnn"
     __version__ = '0.0.1'
 
-    # tf_peak_model_s1_cnn = straxen.URLConfig.evaluate_dry(f'tf:///project2/lgrandi/guidam/CNN_S1_XYZ_SAVED_MODELS/xnt_s1_posrec_cnn_datadriven_00_080921.tar.gz')
     tf_peak_model_s1_cnn = straxen.URLConfig(
         default=f'tf://'
                 f'resource://'
                 f'xedocs://posrec_models'
                 f'?version=ONLINE'
                 f'&run_id=plugin.run_id'
                 f'&kind=s1_cnn'
                 f'&fmt=abs_path'
                 f'&attr=value',
         help='s1 position 3d reconstruction cnn model. Should be opened using the "tf" descriptor. '
              'Set to "None" to skip computation',
         cache=3,
-)
+    )
```

### Comparing `straxen-2.0.7/straxen/plugins/peaks/peak_shadow.py` & `straxen-2.1.0/straxen/plugins/peaks/peak_shadow.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/plugins/peaks/peak_top_bottom_params.py` & `straxen-2.1.0/straxen/plugins/peaks/peak_top_bottom_params.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/plugins/peaks/peaks.py` & `straxen-2.1.0/straxen/plugins/peaks/peaks.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/plugins/peaks/peaks_corrections.py` & `straxen-2.1.0/straxen/plugins/peaks/peak_corrections.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,19 +4,23 @@
 import straxen
 
 export, __all__ = strax.exporter()
 
 
 @export
 class PeakCorrectedAreas(CorrectedAreas):
-    __version__ = '0.0.0'
+    """
+    Pluging to apply corrections on peak level assuming that the main 
+    S1 is the only physical S1. 
+    """
+    __version__ = '0.0.1'
 
-    depends_on = ['peak_basics', 'peak_positions', 'peaks_per_event']
+    depends_on = ('peak_basics', 'peak_positions', 'peak_per_event')
     data_kind = 'peaks'
-    provides = 'peaks_corrections'
+    provides = 'peak_corrections'
 
     electron_drift_velocity = straxen.URLConfig(
         default='cmt://'
                 'electron_drift_velocity'
                 '?version=ONLINE&run_id=plugin.run_id',
         cache=True,
         help='Vertical electron drift velocity in cm/ns (1e4 m/ms)'
@@ -26,93 +30,100 @@
         default='cmt://'
                 'electron_drift_time_gate'
                 '?version=ONLINE&run_id=plugin.run_id',
         help='Electron drift time from the gate in ns',
         cache=True)
 
     def infer_dtype(self):
-        dtype = []
-        dtype += strax.time_fields
-        dtype += [(f'cs2_wo_elifecorr', np.float32,
-                   f'Corrected area of S2 before elife correction '
-                   f'(s2 xy correction + SEG/EE correction applied) [PE]'),
-                  (f'cs2_wo_timecorr', np.float32,
-                   f'Corrected area of S2 before SEG/EE and elife corrections'
-                   f'(s2 xy correction applied) [PE]'),
-                  (f'cs2_area_fraction_top', np.float32,
-                   f'Fraction of area seen by the top PMT array for corrected  S2'),
-                  (f'cs2_bottom', np.float32,
-                   f'Corrected area of S2 in the bottom PMT array [PE]'),
-                  (f'cs2', np.float32, f'Corrected area of  S2 [PE]'),
-                  (f's1_xyz_correction_factor', np.float32,
-                   f'Correction factor for the S1 area based on S2 position'),
-                  (f's1_rel_light_yield_correction_factor', np.float32,
-                   f'Relative light yield correction factor for the S1 area'),
-                  ]
+        dtype = strax.time_fields + [
+            (('Corrected area of S2 before elife correction '
+              '(s2 xy correction + SEG/EE correction applied) [PE]',
+              'cs2_wo_elifecorr'), np.float32),
+            (('Corrected area of S2 before SEG/EE and elife corrections '
+              '(s2 xy correction applied) [PE]',
+              'cs2_wo_timecorr'), np.float32),
+            (('Fraction of area seen by the top PMT array for corrected S2',
+              'cs2_area_fraction_top'), np.float32),
+            (('Corrected area of S2 in the bottom PMT array [PE]',
+              'cs2_bottom'), np.float32),
+            (('Corrected area of S2 [PE]', 'cs2'), np.float32),
+            (('Correction factor for the S1 area based on S2 position',
+              's1_xyz_correction_factor'), np.float32),
+            (('Relative light yield correction factor for the S1 area',
+              's1_rel_light_yield_correction_factor'), np.float32),
+            (('z position of the multiscatter peak',
+              'z_obs_ms'), np.float32),
+        ]
         return dtype
 
     def compute(self, peaks):
         result = np.zeros(len(peaks), self.dtype)
         result['time'] = peaks['time']
         result['endtime'] = peaks['endtime']
 
-        # Get S1 correction factors
-        z_obs = - self.electron_drift_velocity * peaks[f'drift_time']
+        # Get z position of the peak
+        z_obs = -self.electron_drift_velocity * peaks['drift_time']
         z_obs = z_obs + self.electron_drift_velocity * self.electron_drift_time_gate
+        result['z_obs_ms'] = z_obs
+
+        # Get S1 correction factors
         peak_positions = np.vstack([peaks['x'], peaks['y'], z_obs]).T
-        result["s1_xyz_correction_factor"] = 1 / self.s1_xyz_map(peak_positions)
-        result["s1_rel_light_yield_correction_factor"] = 1 / self.rel_light_yield
+        result['s1_xyz_correction_factor'] = 1 / self.s1_xyz_map(peak_positions)
+        result['s1_rel_light_yield_correction_factor'] = 1 / self.rel_light_yield
 
         # s2 corrections
         s2_top_map_name, s2_bottom_map_name = self.s2_map_names()
 
         seg, avg_seg, ee = self.seg_ee_correction_preparation()
 
         # now can start doing corrections
 
         # S2(x,y) corrections use the observed S2 positions
-        s2_positions = np.vstack([peaks[f'x'], peaks[f'y']]).T
+        s2_positions = np.vstack([peaks['x'], peaks['y']]).T
 
         # corrected s2 with s2 xy map only, i.e. no elife correction
         # this is for s2-only events which don't have drift time info
 
-        cs2_top_xycorr = (peaks[f'area']
-                          * peaks[f'area_fraction_top']
+        cs2_top_xycorr = (peaks['area']
+                          * peaks['area_fraction_top']
                           / self.s2_xy_map(s2_positions, map_name=s2_top_map_name))
-        cs2_bottom_xycorr = (peaks[f'area']
-                             * (1 - peaks[f'area_fraction_top'])
+        cs2_bottom_xycorr = (peaks['area']
+                             * (1 - peaks['area_fraction_top'])
                              / self.s2_xy_map(s2_positions, map_name=s2_bottom_map_name))
 
         # For electron lifetime corrections to the S2s,
         # use drift time computed using the main S1.
 
-        elife_correction = np.exp(peaks[f'drift_time'] / self.elife)
-        result[f"cs2_wo_timecorr"] = ((cs2_top_xycorr + cs2_bottom_xycorr) * elife_correction)
+        elife_correction = np.exp(peaks['drift_time'] / self.elife)
+        result['cs2_wo_timecorr'] = ((cs2_top_xycorr + cs2_bottom_xycorr) * elife_correction)
 
         for partition, func in self.regions.items():
             # partitioned SE and EE
-            partition_mask = func(peaks[f'x'], peaks[f'y'])
+            partition_mask = func(peaks['x'], peaks['y'])
 
             # Correct for SEgain and extraction efficiency
             seg_ee_corr = seg[partition] / avg_seg[partition] * ee[partition]
 
             # note that these are already masked!
             cs2_top_wo_elifecorr = cs2_top_xycorr[partition_mask] / seg_ee_corr
             cs2_bottom_wo_elifecorr = cs2_bottom_xycorr[partition_mask] / seg_ee_corr
 
-            result[f"cs2_wo_elifecorr"][partition_mask] = cs2_top_wo_elifecorr + cs2_bottom_wo_elifecorr
+            result['cs2_wo_elifecorr'][partition_mask] = cs2_top_wo_elifecorr + cs2_bottom_wo_elifecorr
 
             # cs2aft doesn't need elife/time corrections as they cancel
-            result[f"cs2_area_fraction_top"][partition_mask] = cs2_top_wo_elifecorr / (
+            result['cs2_area_fraction_top'][partition_mask] = cs2_top_wo_elifecorr / (
                         cs2_top_wo_elifecorr + cs2_bottom_wo_elifecorr)
 
-            result[f"cs2"][partition_mask] = result[f"cs2_wo_elifecorr"][partition_mask] * elife_correction[
-                partition_mask]
-            result[f"cs2_bottom"][partition_mask] = cs2_bottom_wo_elifecorr * elife_correction[partition_mask]
-        result[f"cs2_wo_timecorr"][peaks["type"] != 2] = np.nan
-        result[f"cs2_wo_elifecorr"][peaks["type"] != 2] = np.nan
-        result[f"cs2_area_fraction_top"][peaks["type"] != 2] = np.nan
-        result[f"cs2"][peaks["type"] != 2] = np.nan
-        result[f"cs2_bottom"][peaks["type"] != 2] = np.nan
-        result["s1_xyz_correction_factor"][peaks["type"] != 2] = np.nan
-        result["s1_rel_light_yield_correction_factor"][peaks["type"] != 2] = np.nan
+            result['cs2'][partition_mask] = result['cs2_wo_elifecorr'][
+                partition_mask] * elife_correction[partition_mask]
+            result['cs2_bottom'][partition_mask] = cs2_bottom_wo_elifecorr * elife_correction[partition_mask]
+
+        not_s2_mask = peaks['type'] != 2
+        result['cs2_wo_timecorr'][not_s2_mask] = np.nan
+        result['cs2_wo_elifecorr'][not_s2_mask] = np.nan
+        result['cs2_area_fraction_top'][not_s2_mask] = np.nan
+        result['cs2'][not_s2_mask] = np.nan
+        result['z_obs_ms'][not_s2_mask] = np.nan
+        result['cs2_bottom'][not_s2_mask] = np.nan
+        result['s1_xyz_correction_factor'][not_s2_mask] = np.nan
+        result['s1_rel_light_yield_correction_factor'][not_s2_mask] = np.nan
         return result
```

### Comparing `straxen-2.0.7/straxen/plugins/peaks_he/peaks_he.py` & `straxen-2.1.0/straxen/plugins/peaks_he/peaks_he.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/plugins/raw_records/daqreader.py` & `straxen-2.1.0/straxen/plugins/raw_records/daqreader.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/plugins/raw_records_coin_nv/nveto_recorder.py` & `straxen-2.1.0/straxen/plugins/raw_records_coin_nv/nveto_recorder.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/plugins/records/records.py` & `straxen-2.1.0/straxen/plugins/records/records.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/plugins/records_he/records_he.py` & `straxen-2.1.0/straxen/plugins/records_he/records_he.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/plugins/records_mv/records_mv.py` & `straxen-2.1.0/straxen/plugins/records_mv/records_mv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/plugins/records_nv/records_nv.py` & `straxen-2.1.0/straxen/plugins/records_nv/records_nv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/plugins/veto_intervals/veto_intervals.py` & `straxen-2.1.0/straxen/plugins/veto_intervals/veto_intervals.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/scada.py` & `straxen-2.1.0/straxen/scada.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/storage/mongo_storage.py` & `straxen-2.1.0/straxen/storage/mongo_storage.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/storage/online_monitor_frontend.py` & `straxen-2.1.0/straxen/storage/online_monitor_frontend.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/storage/rucio_local.py` & `straxen-2.1.0/straxen/storage/rucio_local.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/storage/rucio_remote.py` & `straxen-2.1.0/straxen/storage/rucio_remote.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/storage/rundb.py` & `straxen-2.1.0/straxen/storage/rundb.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/test_utils.py` & `straxen-2.1.0/straxen/test_utils.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/units.py` & `straxen-2.1.0/straxen/units.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/straxen/url_config.py` & `straxen-2.1.0/straxen/url_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import strax
 import fsspec
 import numbers
 import straxen
 import inspect
 import tarfile
 import tempfile
+import warnings
 
 import numpy as np
 import pandas as pd
 
 from urllib.parse import urlparse, parse_qs
 from immutabledict import immutabledict
 
@@ -689,7 +690,43 @@
     :param objects: Any list of objects'''
         
     if not isinstance(objects, Iterable):
         raise TypeError(f'The list-to-array protocol expects an '
                         f'iterable but recieved a {type(objects)} instead')
         
     return np.array(objects)
+
+
+@URLConfig.preprocessor
+def alphabetize_url_kwargs(url: str):
+    """
+    Reorders queries for urlconfigs to avoid hashing issues
+    """
+
+    if isinstance(url, str) and URLConfig.SCHEME_SEP in url:
+        if url != URLConfig.format_url_kwargs(url):
+            warnings.warn("From straxen version 2.1.0 onward, URLConfig parameters will be sorted alphabetically before being passed to the plugins, this will change the lineage hash for non-sorted URLs. To load data processed with non-sorted URLs, you will need to use an older version.", FutureWarning)
+        return URLConfig.format_url_kwargs(url)
+    return url
+
+
+@URLConfig.register('run_doc')
+def read_rundoc(path, run_id=None, default=None):
+    """Read a path from the rundoc.
+    """
+    if run_id is None:
+        raise ValueError('rundoc protocol: missing run_id.')
+    runs = xent_collection()
+    rundoc = runs.find_one({'number': int(run_id)}, {'_id': 0, path: 1})
+    if rundoc is None:
+        raise ValueError(f'No rundoc found for run {run_id}')
+
+    for part in path.split('.'):
+        if isinstance(rundoc, list) and part.isdigit() and len(rundoc)>int(part):
+            rundoc = rundoc[int(part)]
+        elif isinstance(rundoc, dict) and part in rundoc:
+            rundoc = rundoc[part]
+        elif default is not None:
+            return default
+        else:
+            raise ValueError(f'No path {path} found in rundoc for run {run_id}')
+    return rundoc
```

### Comparing `straxen-2.0.7/straxen.egg-info/PKG-INFO` & `straxen-2.1.0/straxen.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: straxen
-Version: 2.0.7
+Version: 2.1.0
 Summary: Streaming analysis for XENON
 Home-page: https://github.com/XENONnT/straxen
 Author: Straxen contributors, the XENON collaboration
 License: UNKNOWN
 Description: # straxen
         Streaming analysis for XENON(nT)
         
@@ -25,53 +25,81 @@
         [![Python Versions](https://img.shields.io/pypi/pyversions/straxen.svg)](https://pypi.python.org/pypi/straxen)
         [![PyPI downloads](https://img.shields.io/pypi/dm/straxen.svg)](https://pypistats.org/packages/straxen)
         
         [![Update context collection](https://github.com/XENONnT/straxen/workflows/Update%20context%20collection/badge.svg)](https://github.com/XENONnT/straxen/actions/workflows/contexts.yml)
         [![Python style](https://github.com/XENONnT/straxen/actions/workflows/code_style.yml/badge.svg)](https://github.com/XENONnT/straxen/actions/workflows/code_style.yml)
         
         
+        v2.1.70 / 2023-06-22
+        -------------------
+        * Added peaks subtyping by @Jianyu010 in https://github.com/XENONnT/straxen/pull/1152
+        * Fix ipython version by @dachengx in https://github.com/XENONnT/straxen/pull/1169
+        * Fix bug in hitlets time ordering by @dachengx in https://github.com/XENONnT/straxen/pull/1173
+        * Bump actions/setup-python from 4.5.0 to 4.6.0 by @dependabot in https://github.com/XENONnT/straxen/pull/1170
+        * Save hits level information(hits height and time difference) in peak and event level by @dachengx in https://github.com/XENONnT/straxen/pull/1155
+        * Fix argsort inside numba.jit using kind='mergesort' by @dachengx in https://github.com/XENONnT/straxen/pull/1176
+        * Bump merged_s2s version following `strax.merge_peaks` by @dachengx in https://github.com/XENONnT/straxen/pull/1179
+        * Use same files names for peak and event level pos-rec by @dachengx in https://github.com/XENONnT/straxen/pull/1160
+        * Update multi scatter Ignore nan in the sum of peaks. by @michaweiss89 in https://github.com/XENONnT/straxen/pull/1162
+        * Add dynamic event display docs by @WenzDaniel in https://github.com/XENONnT/straxen/pull/1077
+        * Lower the titles in the same notebook by @dachengx in https://github.com/XENONnT/straxen/pull/1183
+        * No longer test `st.runs` in `test_extract_latest_comment_lone_hits` by @dachengx in https://github.com/XENONnT/straxen/pull/1199
+        * Remove unnecessary check in `merged_s2s` by @dachengx in https://github.com/XENONnT/straxen/pull/1195
+        * automatically appending local rucio path by @FaroutYLq in https://github.com/XENONnT/straxen/pull/1182
+        * Performance boost veto proximity by @WenzDaniel in https://github.com/XENONnT/straxen/pull/1181
+        * Update build_datastructure_doc.py by @PeterGy in https://github.com/XENONnT/straxen/pull/1202
+        * Add rundoc URLConfig protocol by @jmosbacher in https://github.com/XENONnT/straxen/pull/1135
+        * Split event_area_per_channel into two plugins: event_area_per_channel… by @minzhong98 in https://github.com/XENONnT/straxen/pull/1191
+        * Fix event basics time ordering by @jjakob03 in https://github.com/XENONnT/straxen/pull/1194
+        * Make apply_xedocs_configs more flexible by @jmosbacher in https://github.com/XENONnT/straxen/pull/1204
+        * Try to make hashing more coinsistent by @LuisSanchez25 in https://github.com/XENONnT/straxen/pull/1201
+        
+        New Contributors
+        * @PeterGy made their first contribution in https://github.com/XENONnT/straxen/pull/1202
+        * @minzhong98 made their first contribution in https://github.com/XENONnT/straxen/pull/1191
+        
+        **Full Changelog**: https://github.com/XENONnT/straxen/compare/v2.0.7...v2.1.0
+        
+        
         v2.0.7 / 2023-04-25
         -------------------
-        ## What's Changed
         * Bootstrax target removal after failures by @cfuselli in https://github.com/XENONnT/straxen/pull/1145
         * reforming _raw_path and _processed_path by @FaroutYLq in https://github.com/XENONnT/straxen/pull/1149
         * Adding correction of Z position due to non-uniform drift velocity by @terliuk in https://github.com/XENONnT/straxen/pull/1148
         * Bump the versions of peaklets and quality check runs-on by @dachengx in https://github.com/XENONnT/straxen/pull/1153
         * S1-Based 3D Position Reconstruction by @matteoguida in https://github.com/XENONnT/straxen/pull/1146
         * Bump xedocs from 0.2.14 to 0.2.16 in /extra_requirements by @dependabot in https://github.com/XENONnT/straxen/pull/1158
         * Use zstd as compressor of peaks by @dachengx in https://github.com/XENONnT/straxen/pull/1154
         * Bump sphinx from 5.3.0 to 6.2.0 in /extra_requirements by @dependabot in https://github.com/XENONnT/straxen/pull/1161
         
-        ## New Contributors
+        New Contributors
         * @cfuselli made their first contribution in https://github.com/XENONnT/straxen/pull/1145
         * @matteoguida made their first contribution in https://github.com/XENONnT/straxen/pull/1146
         * @hmdyt made their first contribution in https://github.com/XENONnT/straxen/pull/1159
         
         **Full Changelog**: https://github.com/XENONnT/straxen/compare/v2.0.6...v2.0.7
         
         
         v2.0.6 / 2023-03-08
         -------------------
-        ## What's Changed
         * Bump supercharge/mongodb-github-action from 1.8.0 to 1.9.0 by @dependabot in https://github.com/XENONnT/straxen/pull/1140
         * Small patches to restrax module by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1143, d04a3428c52c159577b61af2a28ddd0af5652027, 602b807291211f083c8f54df6768b8198fbf6b55
         * Ms events by @michaweiss89 and @HenningSE in https://github.com/XENONnT/straxen/pull/1080
         
-        ## New Contributors
+        New Contributors
         * @michaweiss89 made their first contribution in https://github.com/XENONnT/straxen/pull/1080
         
         **Full Changelog**: https://github.com/XENONnT/straxen/compare/v2.0.5...v2.0.6
         
         Notes:
          - new data types: `peaks_per_event`, `event_top_bottom_params`, `peaks_corrections` (see #1080)
         
         
         v2.0.5 / 2023-02-24
         -------------------
-        ## What's Changed
         * fix xedocs for testing by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1139
         * Restart python style guide by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1138
         * Decrease number of chunks by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1123
         * Restrax by @JoranAngevaare in https://github.com/XENONnT/straxen/pull/1074
         
         
         **Full Changelog**: https://github.com/XENONnT/straxen/compare/v2.0.4...v2.0.5
@@ -1010,15 +1038,15 @@
         - Updated bin scripts like straxer (#204) 
         - Updated PMT gains (#208)
         - Renamed high energy plugins (#200)
         - Bugifx in nveto-plugins (#183, #209)
         - Bugfix in clean_up_empty_records (#210)
         
         
-        0.10.0 / 2020-08-187
+        0.10.0 / 2020-08-18
         --------------------
         - Neutron-veto integration (#86)
         - Processing for high energy channels (#161, #176)
         - Integrate rucio as storage backend (#164)
         - Remapping of old runs (#166)
         - Bootstrax/microstrax/ajax updates (#165)
         - Pull request template (#168)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `straxen-2.0.7/straxen.egg-info/SOURCES.txt` & `straxen-2.1.0/straxen.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -68,33 +68,34 @@
 straxen/plugins/afterpulses/__init__.py
 straxen/plugins/afterpulses/afterpulse_processing.py
 straxen/plugins/aqmon_hits/__init__.py
 straxen/plugins/aqmon_hits/aqmon_hits.py
 straxen/plugins/detector_time_offsets/__init__.py
 straxen/plugins/detector_time_offsets/detector_time_offsets.py
 straxen/plugins/events/__init__.py
-straxen/plugins/events/_event_s1_position_base.py
-straxen/plugins/events/_event_s2_position_base.py
+straxen/plugins/events/_event_s1_positions_base.py
+straxen/plugins/events/_event_s2_positions_base.py
 straxen/plugins/events/corrected_areas.py
 straxen/plugins/events/distinct_channels.py
 straxen/plugins/events/energy_estimates.py
 straxen/plugins/events/event_ambience.py
 straxen/plugins/events/event_area_per_channel.py
 straxen/plugins/events/event_basics.py
 straxen/plugins/events/event_info.py
 straxen/plugins/events/event_info_double.py
 straxen/plugins/events/event_pattern_fit.py
 straxen/plugins/events/event_positions.py
-straxen/plugins/events/event_s1_position_cnn.py
-straxen/plugins/events/event_s2_position_cnn.py
-straxen/plugins/events/event_s2_position_gcn.py
-straxen/plugins/events/event_s2_position_mlp.py
+straxen/plugins/events/event_s1_positions_cnn.py
+straxen/plugins/events/event_s2_positions_cnn.py
+straxen/plugins/events/event_s2_positions_gcn.py
+straxen/plugins/events/event_s2_positions_mlp.py
 straxen/plugins/events/event_shadow.py
 straxen/plugins/events/event_top_bottom_params.py
 straxen/plugins/events/event_w_bayes_class.py
+straxen/plugins/events/event_waveform.py
 straxen/plugins/events/events.py
 straxen/plugins/events/local_minimum_info.py
 straxen/plugins/events/multi_scatter.py
 straxen/plugins/events/s2_recon_pos_diff.py
 straxen/plugins/events/veto_proximity.py
 straxen/plugins/events_mv/__init__.py
 straxen/plugins/events_mv/events_mv.py
@@ -125,29 +126,30 @@
 straxen/plugins/peaklets/peaklet_classification.py
 straxen/plugins/peaklets/peaklets.py
 straxen/plugins/peaklets_he/__init__.py
 straxen/plugins/peaklets_he/peaklet_classification_he.py
 straxen/plugins/peaklets_he/peaklets_he.py
 straxen/plugins/peaks/__init__.py
 straxen/plugins/peaks/_peak_positions_base.py
-straxen/plugins/peaks/_peak_s1_position_base.py
+straxen/plugins/peaks/_peak_s1_positions_base.py
 straxen/plugins/peaks/peak_ambience.py
 straxen/plugins/peaks/peak_basics.py
 straxen/plugins/peaks/peak_classification_bayes.py
+straxen/plugins/peaks/peak_corrections.py
+straxen/plugins/peaks/peak_per_event.py
 straxen/plugins/peaks/peak_positions.py
 straxen/plugins/peaks/peak_positions_cnn.py
 straxen/plugins/peaks/peak_positions_gcn.py
 straxen/plugins/peaks/peak_positions_mlp.py
 straxen/plugins/peaks/peak_proximity.py
-straxen/plugins/peaks/peak_s1_position_cnn.py
+straxen/plugins/peaks/peak_s1_positions_cnn.py
 straxen/plugins/peaks/peak_shadow.py
 straxen/plugins/peaks/peak_top_bottom_params.py
 straxen/plugins/peaks/peaks.py
-straxen/plugins/peaks/peaks_corrections.py
-straxen/plugins/peaks/peaks_per_event.py
+straxen/plugins/peaks/peaks_subtyping.py
 straxen/plugins/peaks_he/__init__.py
 straxen/plugins/peaks_he/peak_basics_he.py
 straxen/plugins/peaks_he/peaks_he.py
 straxen/plugins/raw_records/__init__.py
 straxen/plugins/raw_records/daqreader.py
 straxen/plugins/raw_records_coin_nv/__init__.py
 straxen/plugins/raw_records_coin_nv/nveto_recorder.py
```

### Comparing `straxen-2.0.7/tests/storage/test_database_frontends.py` & `straxen-2.1.0/tests/storage/test_database_frontends.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/tests/storage/test_mongo_downloader.py` & `straxen-2.1.0/tests/storage/test_mongo_downloader.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/tests/storage/test_mongo_interactions.py` & `straxen-2.1.0/tests/storage/test_mongo_interactions.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/tests/storage/test_rucio_local.py` & `straxen-2.1.0/tests/storage/test_rucio_local.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/tests/storage/test_rucio_remote.py` & `straxen-2.1.0/tests/storage/test_rucio_remote.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/tests/test_1T_plugins.py` & `straxen-2.1.0/tests/test_1T_plugins.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/tests/test_aqmon.py` & `straxen-2.1.0/tests/test_aqmon.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/tests/test_basics.py` & `straxen-2.1.0/tests/test_basics.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,18 +53,18 @@
         if context == 'xenonnt_online' and not straxen.utilix_is_configured():
             return
         st = getattr(straxen.contexts, context)(**context_kwargs)
         assert hasattr(st, 'extract_latest_comment'), "extract_latest_comment not added to context?"
         st.extract_latest_comment()
         assert st.runs is not None, "No registry build?"
         assert 'comments' in st.runs.keys()
-        st.select_runs(available=test_for_target)
+        runs = st.select_runs(available=test_for_target)
         if context == 'demo':
             assert len(st.runs)
-        assert f'{test_for_target}_available' in st.runs.keys()
+        assert f'{test_for_target}_available' in runs.keys()
 
     def test_extract_latest_comment_nt(self, **opt):
         """Run the test for nt (but only 2000 runs"""
         self._extract_latest_comment(context='xenonnt_online',
                                      minimum_run_number=10_000,
                                      maximum_run_number=12_000,
                                      **opt)
```

### Comparing `straxen-2.0.7/tests/test_channel_split.py` & `straxen-2.1.0/tests/test_channel_split.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/tests/test_cmt.py` & `straxen-2.1.0/tests/test_cmt.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/tests/test_common.py` & `straxen-2.1.0/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/tests/test_contexts.py` & `straxen-2.1.0/tests/test_contexts.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/tests/test_count_pulses.py` & `straxen-2.1.0/tests/test_count_pulses.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/tests/test_daq_reader.py` & `straxen-2.1.0/tests/test_daq_reader.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/tests/test_holoviews_utils.py` & `straxen-2.1.0/tests/test_holoviews_utils.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/tests/test_itp_map.py` & `straxen-2.1.0/tests/test_itp_map.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/tests/test_led_calibration.py` & `straxen-2.1.0/tests/test_led_calibration.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/tests/test_mini_analyses.py` & `straxen-2.1.0/tests/test_mini_analyses.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/tests/test_misc.py` & `straxen-2.1.0/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/tests/test_nveto_events.py` & `straxen-2.1.0/tests/test_nveto_events.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/tests/test_nveto_recorder.py` & `straxen-2.1.0/tests/test_nveto_recorder.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/tests/test_patternfit.py` & `straxen-2.1.0/tests/test_patternfit.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/tests/test_peaklet_processing.py` & `straxen-2.1.0/tests/test_peaklet_processing.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     peaklets = res['peaklets']
     assert peaklets['n_hits'] == 3, f"Peaklet has the wrong number of hits!"
 
 
 @given(fake_hits,
        strat.lists(elements=strat.integers(0, 9), min_size=20))
 @settings(deadline=None)
-def test_tight_coincidence(hits, channel):
+def test_get_tight_coin(hits, channel):
     hits['area'] = 1
     hits['channel'] = channel[:len(hits)]  # In case there are less channel then hits (unlikely)
     gap_threshold = 10
     peaks = strax.find_peaks(hits,
                              adc_to_pe=np.ones(10),
                              right_extension=0, left_extension=0,
                              gap_threshold=gap_threshold,
@@ -64,17 +64,16 @@
 
     peaks_max_time = peaks['time'] + peaks['length']//2
     hits_max_time = hits['time'] + hits['length']//2
 
     left = 5
     right = 5
     tight_coin_channel = get_tight_coin(hits_max_time,
-                                                    hits['channel'],
-                                                    peaks_max_time,
-                                                    left,
-                                                    right,
-                                                    )
+                                        hits['channel'],
+                                        peaks_max_time,
+                                        left,
+                                        right)
     for ind, p_max_t in enumerate(peaks_max_time):
         m_hits_in_peak = (hits_max_time >= (p_max_t - left))
         m_hits_in_peak &= (hits_max_time <= (p_max_t + right))
         n_channel = len(np.unique(hits[m_hits_in_peak]['channel']))
         assert n_channel == tight_coin_channel[ind], f'Wrong number of tight channel got {tight_coin_channel[ind]}, but expectd {n_channel}'  # noqa
```

### Comparing `straxen-2.0.7/tests/test_peaks.py` & `straxen-2.1.0/tests/test_peaks.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/tests/test_scada.py` & `straxen-2.1.0/tests/test_scada.py`

 * *Files identical despite different names*

### Comparing `straxen-2.0.7/tests/test_url_config.py` & `straxen-2.1.0/tests/test_url_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -340,14 +340,28 @@
         self.assertEqual(p.test_config, f'test_config:{nt_test_run_id}')
         self.assertEqual(p.test_config, p.config['test_config'])
 
     def test_global_version_preprocessor(self):
         self.st.set_config({'test_config': 'fake://url?version=global_v1'})
         p = self.st.get_single_plugin(nt_test_run_id, 'test_data')
         self.assertEqual(p.test_config, 'fake://url?version=v0')
+
+    def test_alphabetize_url_kwargs(self):
+        """URLConfig preprocessor to rearange the order of arguments given buy a 
+        url to ensure the same url with a different hash order gives the same hash"""
+        url = "xedocs://electron_lifetimes?run_id=034678&version=v5&attr=value"
+        intended_url = "xedocs://electron_lifetimes?attr=value&run_id=034678&version=v5"
+        preprocessed_url = straxen.url_config.alphabetize_url_kwargs(url)
+        self.assertEqual(intended_url, preprocessed_url)
+
+    def test_xedocs_global_version_hash_coinsistency(self):
+        # Same URLs but the queries are in a different order
+        st1 = self.st.new_context(config={"test_config":"fake://electron_lifetimes?run_id=25000&version=v5&attr=value"})
+        st2 = self.st.new_context(config={"test_config":"fake://electron_lifetimes?attr=value&run_id=25000&version=v5"})
+        self.assertEqual(st1.key_for(25000, 'corrected_areas').lineage_hash, st2.key_for(25000, 'corrected_areas').lineage_hash)
     
     def test_global_version_not_changed(self):
         """
           - if no global version is matched, the url version should not be changed
           - if config is not matched, the url version should not be changed
         """
         assert 'global_v2' not in GLOBAL_VERSIONS
@@ -358,7 +372,22 @@
         class ExamplePluginNew(ExamplePlugin):
             test_config_new = straxen.URLConfig(default='rootisthesourceofallevil',)
 
         self.st.register(ExamplePluginNew)
         self.st.set_config({'test_config_new': 'fake://url?version=global_v1'})
         p = self.st.get_single_plugin(nt_test_run_id, 'test_data')
         self.assertEqual(p.test_config_new, 'fake://url?version=global_v1')
+
+    @unittest.skipIf(not straxen.utilix_is_configured(), "No db access, cannot test run_doc protocol.")
+    def test_run_doc_protocol(self):
+        self.st.set_config({ 'test_config': "run_doc://mode?run_id=plugin.run_id" })
+        p = self.st.get_single_plugin(nt_test_run_id, 'test_data')
+        self.assertEqual(p.test_config, 'tpc_commissioning')
+
+        self.st.set_config({ 'test_config': "run_doc://fake_key?run_id=plugin.run_id&default=42" })
+        p = self.st.get_single_plugin(nt_test_run_id, 'test_data')
+        self.assertEqual(p.test_config, 42)
+
+        with self.assertRaises(ValueError):
+            self.st.set_config({ 'test_config': "run_doc://mode?run_id=plugin.run_id" })
+            p = self.st.get_single_plugin(999999999, 'test_data')
+            return p.test_config
```

### Comparing `straxen-2.0.7/tests/test_veto_hitlets.py` & `straxen-2.1.0/tests/test_veto_hitlets.py`

 * *Files identical despite different names*

