# Comparing `tmp/radical.analytics-1.5.0.tar.gz` & `tmp/radical.analytics-1.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/radical.analytics-1.5.0.tar", last modified: Tue Aug 11 13:33:40 2020, max compression
+gzip compressed data, was "radical.analytics-1.6.7.tar", last modified: Thu Jul  8 08:08:44 2021, max compression
```

## Comparing `radical.analytics-1.5.0.tar` & `radical.analytics-1.6.7.tar`

### file list

```diff
@@ -1,100 +1,103 @@
-drwxr-xr-x   0 mturilli   (501) staff       (20)        0 2020-08-11 13:33:40.117069 radical.analytics-1.5.0/
--rw-r--r--   0 mturilli   (501) staff       (20)     5484 2020-08-11 13:23:09.000000 radical.analytics-1.5.0/CHANGES.md
--rw-r--r--   0 mturilli   (501) staff       (20)    15222 2020-05-05 15:05:35.000000 radical.analytics-1.5.0/LICENSE
--rw-r--r--   0 mturilli   (501) staff       (20)      115 2020-05-05 15:05:35.000000 radical.analytics-1.5.0/MANIFEST.in
--rw-r--r--   0 mturilli   (501) staff       (20)      958 2020-08-11 13:33:40.116748 radical.analytics-1.5.0/PKG-INFO
--rw-r--r--   0 mturilli   (501) staff       (20)      762 2020-08-11 13:23:09.000000 radical.analytics-1.5.0/README.md
--rw-r--r--   0 mturilli   (501) staff       (20)        6 2020-08-11 13:23:09.000000 radical.analytics-1.5.0/VERSION
-drwxr-xr-x   0 mturilli   (501) staff       (20)        0 2020-08-11 13:33:40.049251 radical.analytics-1.5.0/bin/
--rwxr-xr-x   0 mturilli   (501) staff       (20)     4723 2020-08-11 13:23:09.000000 radical.analytics-1.5.0/bin/radical-analytics-check
--rwxr-xr-x   0 mturilli   (501) staff       (20)     6048 2020-06-23 08:47:15.000000 radical.analytics-1.5.0/bin/radical-analytics-inspect
--rwxr-xr-x   0 mturilli   (501) staff       (20)     8933 2020-08-11 13:23:09.000000 radical.analytics-1.5.0/bin/radical-analytics-plot.py
--rwxr-xr-x   0 mturilli   (501) staff       (20)       88 2020-08-11 13:23:09.000000 radical.analytics-1.5.0/bin/radical-analytics-version
--rwxr-xr-x   0 mturilli   (501) staff       (20)    36969 2020-05-05 15:05:35.000000 radical.analytics-1.5.0/bin/radical-analytics-wrangler.py
-drwxr-xr-x   0 mturilli   (501) staff       (20)        0 2020-08-11 13:33:40.050899 radical.analytics-1.5.0/bin/rp_inspect/
--rwxr-xr-x   0 mturilli   (501) staff       (20)     2736 2020-08-11 13:23:09.000000 radical.analytics-1.5.0/bin/rp_inspect/plot_conc.py
--rwxr-xr-x   0 mturilli   (501) staff       (20)     4492 2020-05-05 15:05:35.000000 radical.analytics-1.5.0/bin/rp_inspect/plot_dur.py
--rwxr-xr-x   0 mturilli   (501) staff       (20)     2762 2020-05-05 15:05:35.000000 radical.analytics-1.5.0/bin/rp_inspect/plot_rate.py
--rwxr-xr-x   0 mturilli   (501) staff       (20)     4666 2020-05-05 15:05:35.000000 radical.analytics-1.5.0/bin/rp_inspect/plot_state.py
--rwxr-xr-x   0 mturilli   (501) staff       (20)     7037 2020-08-11 13:23:09.000000 radical.analytics-1.5.0/bin/rp_inspect/plot_util.py
-drwxr-xr-x   0 mturilli   (501) staff       (20)        0 2020-08-11 13:33:40.074938 radical.analytics-1.5.0/examples/
--rwxr-xr-x   0 mturilli   (501) staff       (20)     3017 2020-05-05 15:05:35.000000 radical.analytics-1.5.0/examples/00_session_describe_rp.py
--rwxr-xr-x   0 mturilli   (501) staff       (20)     2514 2020-05-05 15:05:35.000000 radical.analytics-1.5.0/examples/01_session_list_rp.py
--rwxr-xr-x   0 mturilli   (501) staff       (20)     4166 2020-05-05 15:05:35.000000 radical.analytics-1.5.0/examples/02_session_get_rp.py
--rwxr-xr-x   0 mturilli   (501) staff       (20)     3036 2020-05-05 15:05:35.000000 radical.analytics-1.5.0/examples/03_session_filter_rp.py
--rwxr-xr-x   0 mturilli   (501) staff       (20)     4465 2020-05-05 15:05:35.000000 radical.analytics-1.5.0/examples/04_session_duration_rp.py
--rwxr-xr-x   0 mturilli   (501) staff       (20)     1520 2020-05-05 15:05:35.000000 radical.analytics-1.5.0/examples/05_relationsships.py
--rwxr-xr-x   0 mturilli   (501) staff       (20)     4856 2020-05-05 15:05:35.000000 radical.analytics-1.5.0/examples/06_events.py
--rwxr-xr-x   0 mturilli   (501) staff       (20)     1289 2020-05-05 15:05:35.000000 radical.analytics-1.5.0/examples/06_ra_events.py
--rwxr-xr-x   0 mturilli   (501) staff       (20)     4827 2020-05-05 15:05:35.000000 radical.analytics-1.5.0/examples/07_event_timeline.py
--rwxr-xr-x   0 mturilli   (501) staff       (20)     5940 2020-05-05 15:05:35.000000 radical.analytics-1.5.0/examples/08_core_utilization_plot.py
--rwxr-xr-x   0 mturilli   (501) staff       (20)     8909 2020-05-05 15:05:35.000000 radical.analytics-1.5.0/examples/08c_core_utilization_plot.py
--rwxr-xr-x   0 mturilli   (501) staff       (20)     4990 2020-05-05 15:05:35.000000 radical.analytics-1.5.0/examples/09_session_plots.py
--rwxr-xr-x   0 mturilli   (501) staff       (20)     4717 2020-05-05 15:05:35.000000 radical.analytics-1.5.0/examples/10_durations.py
--rw-r--r--   0 mturilli   (501) staff       (20)       38 2020-08-11 13:33:40.117180 radical.analytics-1.5.0/setup.cfg
--rwxr-xr-x   0 mturilli   (501) staff       (20)     9732 2020-08-11 13:30:07.000000 radical.analytics-1.5.0/setup.py
-drwxr-xr-x   0 mturilli   (501) staff       (20)        0 2020-08-11 13:33:40.044618 radical.analytics-1.5.0/src/
-drwxr-xr-x   0 mturilli   (501) staff       (20)        0 2020-08-11 13:33:40.075216 radical.analytics-1.5.0/src/radical/
--rw-r--r--   0 mturilli   (501) staff       (20)       56 2020-05-05 15:05:35.000000 radical.analytics-1.5.0/src/radical/__init__.py
-drwxr-xr-x   0 mturilli   (501) staff       (20)        0 2020-08-11 13:33:40.082731 radical.analytics-1.5.0/src/radical/analytics/
--rw-r--r--   0 mturilli   (501) staff       (20)       56 2020-08-11 13:33:39.000000 radical.analytics-1.5.0/src/radical/analytics/SDIST
--rw-r--r--   0 mturilli   (501) staff       (20)       31 2020-08-11 13:33:39.000000 radical.analytics-1.5.0/src/radical/analytics/VERSION
--rw-r--r--   0 mturilli   (501) staff       (20)      871 2020-08-11 13:23:09.000000 radical.analytics-1.5.0/src/radical/analytics/__init__.py
--rw-r--r--   0 mturilli   (501) staff       (20)    17223 2020-08-11 13:23:09.000000 radical.analytics-1.5.0/src/radical/analytics/entity.py
--rw-r--r--   0 mturilli   (501) staff       (20)     4583 2020-08-11 13:23:09.000000 radical.analytics-1.5.0/src/radical/analytics/experiment.py
--rw-r--r--   0 mturilli   (501) staff       (20)     6514 2020-06-23 08:47:15.000000 radical.analytics-1.5.0/src/radical/analytics/plotter.py
--rw-r--r--   0 mturilli   (501) staff       (20)   959817 2020-05-10 03:21:02.000000 radical.analytics-1.5.0/src/radical/analytics/radical.analytics-0.90.7-v0.72.0-42-gcab8498-feature-unittests.tar.gz
--rw-r--r--   0 mturilli   (501) staff       (20)  1826309 2020-05-15 23:36:03.000000 radical.analytics-1.5.0/src/radical/analytics/radical.analytics-0.90.7-v0.72.0-44-ge31c6b0-fix-plot-origin.tar.gz
--rw-r--r--   0 mturilli   (501) staff       (20)    56437 2020-08-11 13:23:09.000000 radical.analytics-1.5.0/src/radical/analytics/session.py
-drwxr-xr-x   0 mturilli   (501) staff       (20)        0 2020-08-11 13:33:40.077431 radical.analytics-1.5.0/src/radical.analytics.egg-info/
--rw-r--r--   0 mturilli   (501) staff       (20)      958 2020-08-11 13:33:39.000000 radical.analytics-1.5.0/src/radical.analytics.egg-info/PKG-INFO
--rw-r--r--   0 mturilli   (501) staff       (20)     4453 2020-08-11 13:33:39.000000 radical.analytics-1.5.0/src/radical.analytics.egg-info/SOURCES.txt
--rw-r--r--   0 mturilli   (501) staff       (20)        1 2020-08-11 13:33:39.000000 radical.analytics-1.5.0/src/radical.analytics.egg-info/dependency_links.txt
--rw-r--r--   0 mturilli   (501) staff       (20)        8 2020-08-11 13:33:39.000000 radical.analytics-1.5.0/src/radical.analytics.egg-info/namespace_packages.txt
--rw-r--r--   0 mturilli   (501) staff       (20)        1 2020-08-11 13:33:39.000000 radical.analytics-1.5.0/src/radical.analytics.egg-info/not-zip-safe
--rw-r--r--   0 mturilli   (501) staff       (20)       83 2020-08-11 13:33:39.000000 radical.analytics-1.5.0/src/radical.analytics.egg-info/requires.txt
--rw-r--r--   0 mturilli   (501) staff       (20)        8 2020-08-11 13:33:39.000000 radical.analytics-1.5.0/src/radical.analytics.egg-info/top_level.txt
-drwxr-xr-x   0 mturilli   (501) staff       (20)        0 2020-08-11 13:33:40.083755 radical.analytics-1.5.0/tests/
--rw-r--r--   0 mturilli   (501) staff       (20)        0 2020-05-05 15:05:35.000000 radical.analytics-1.5.0/tests/__init__.py
-drwxr-xr-x   0 mturilli   (501) staff       (20)        0 2020-08-11 13:33:40.083989 radical.analytics-1.5.0/tests/barrier_data/
-drwxr-xr-x   0 mturilli   (501) staff       (20)        0 2020-08-11 13:33:40.088981 radical.analytics-1.5.0/tests/barrier_data/rp.session.two.jdakka.017395.0000/
--rw-r--r--   0 mturilli   (501) staff       (20)     1291 2020-05-05 15:05:35.000000 radical.analytics-1.5.0/tests/barrier_data/rp.session.two.jdakka.017395.0000/pmgr.0000.prof
--rw-r--r--   0 mturilli   (501) staff       (20)        0 2020-05-05 15:05:35.000000 radical.analytics-1.5.0/tests/barrier_data/rp.session.two.jdakka.017395.0000/pmgr.launching.0.child.prof
--rw-r--r--   0 mturilli   (501) staff       (20)      486 2020-05-05 15:05:35.000000 radical.analytics-1.5.0/tests/barrier_data/rp.session.two.jdakka.017395.0000/pmgr.launching.0.prof
--rw-r--r--   0 mturilli   (501) staff       (20)      855 2020-05-05 15:05:35.000000 radical.analytics-1.5.0/tests/barrier_data/rp.session.two.jdakka.017395.0000/rp.session.two.jdakka.017395.0000.prof
--rw-r--r--   0 mturilli   (501) staff       (20)   339968 2020-05-05 15:05:35.000000 radical.analytics-1.5.0/tests/barrier_data/rp.session.two.jdakka.017395.0000/umgr.0000.prof
--rw-r--r--   0 mturilli   (501) staff       (20)    93001 2020-05-05 15:05:35.000000 radical.analytics-1.5.0/tests/barrier_data/rp.session.two.jdakka.017395.0000/umgr.scheduling.0.child.prof
--rw-r--r--   0 mturilli   (501) staff       (20)      144 2020-05-05 15:05:35.000000 radical.analytics-1.5.0/tests/barrier_data/rp.session.two.jdakka.017395.0000/umgr.scheduling.0.prof
--rw-r--r--   0 mturilli   (501) staff       (20)    83051 2020-05-05 15:05:35.000000 radical.analytics-1.5.0/tests/barrier_data/rp.session.two.jdakka.017395.0000/umgr.staging.input.0.child.prof
--rw-r--r--   0 mturilli   (501) staff       (20)      148 2020-05-05 15:05:35.000000 radical.analytics-1.5.0/tests/barrier_data/rp.session.two.jdakka.017395.0000/umgr.staging.input.0.prof
--rw-r--r--   0 mturilli   (501) staff       (20)    79361 2020-05-05 15:05:35.000000 radical.analytics-1.5.0/tests/barrier_data/rp.session.two.jdakka.017395.0000/umgr.staging.output.0.child.prof
--rw-r--r--   0 mturilli   (501) staff       (20)      149 2020-05-05 15:05:35.000000 radical.analytics-1.5.0/tests/barrier_data/rp.session.two.jdakka.017395.0000/umgr.staging.output.0.prof
--rw-r--r--   0 mturilli   (501) staff       (20)   647168 2020-05-05 15:05:35.000000 radical.analytics-1.5.0/tests/barrier_data/rp.session.two.jdakka.017395.0000/update.0.child.prof
--rw-r--r--   0 mturilli   (501) staff       (20)      430 2020-05-05 15:05:35.000000 radical.analytics-1.5.0/tests/barrier_data/rp.session.two.jdakka.017395.0000/update.0.prof
--rw-r--r--   0 mturilli   (501) staff       (20)   426921 2020-05-05 15:05:35.000000 radical.analytics-1.5.0/tests/barrier_data/rp.session.two.jdakka.017395.0000.json
-drwxr-xr-x   0 mturilli   (501) staff       (20)        0 2020-08-11 13:33:40.090735 radical.analytics-1.5.0/tests/example-data/
--rw-r--r--   0 mturilli   (501) staff       (20)     7071 2020-05-05 15:05:35.000000 radical.analytics-1.5.0/tests/example-data/pilot-entity-example.json
--rw-r--r--   0 mturilli   (501) staff       (20)     1503 2020-05-05 15:05:35.000000 radical.analytics-1.5.0/tests/example-data/pmgr-entity-example.json
--rw-r--r--   0 mturilli   (501) staff       (20)     7057 2020-05-05 15:05:35.000000 radical.analytics-1.5.0/tests/example-data/range-testing-entity-example.json
--rw-r--r--   0 mturilli   (501) staff       (20)    22261 2020-05-05 15:05:35.000000 radical.analytics-1.5.0/tests/example-data/rp-entity-example.json
--rw-r--r--   0 mturilli   (501) staff       (20)     3543 2020-05-05 15:05:35.000000 radical.analytics-1.5.0/tests/example-data/umgr-entity-example.json
--rw-r--r--   0 mturilli   (501) staff       (20)    13872 2020-05-05 15:05:35.000000 radical.analytics-1.5.0/tests/example-data/unit-entity-example.json
-drwxr-xr-x   0 mturilli   (501) staff       (20)        0 2020-08-11 13:33:40.091070 radical.analytics-1.5.0/tests/no_barrier_data/
-drwxr-xr-x   0 mturilli   (501) staff       (20)        0 2020-08-11 13:33:40.116252 radical.analytics-1.5.0/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007/
--rw-r--r--   0 mturilli   (501) staff       (20)     1208 2020-05-05 15:05:35.000000 radical.analytics-1.5.0/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007/pmgr.0000.prof
--rw-r--r--   0 mturilli   (501) staff       (20)        0 2020-05-05 15:05:35.000000 radical.analytics-1.5.0/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007/pmgr.launching.0.child.prof
--rw-r--r--   0 mturilli   (501) staff       (20)      492 2020-05-05 15:05:35.000000 radical.analytics-1.5.0/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007/pmgr.launching.0.prof
--rw-r--r--   0 mturilli   (501) staff       (20)     1207 2020-05-05 15:05:35.000000 radical.analytics-1.5.0/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007.prof
--rw-r--r--   0 mturilli   (501) staff       (20)  3768320 2020-05-05 15:05:35.000000 radical.analytics-1.5.0/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007/umgr.0000.prof
--rw-r--r--   0 mturilli   (501) staff       (20)   847228 2020-05-05 15:05:35.000000 radical.analytics-1.5.0/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007/umgr.scheduling.0.child.prof
--rw-r--r--   0 mturilli   (501) staff       (20)      149 2020-05-05 15:05:35.000000 radical.analytics-1.5.0/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007/umgr.scheduling.0.prof
--rw-r--r--   0 mturilli   (501) staff       (20)   756110 2020-05-05 15:05:35.000000 radical.analytics-1.5.0/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007/umgr.staging.input.0.child.prof
--rw-r--r--   0 mturilli   (501) staff       (20)      150 2020-05-05 15:05:35.000000 radical.analytics-1.5.0/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007/umgr.staging.input.0.prof
--rw-r--r--   0 mturilli   (501) staff       (20)   722324 2020-05-05 15:05:35.000000 radical.analytics-1.5.0/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007/umgr.staging.output.0.child.prof
--rw-r--r--   0 mturilli   (501) staff       (20)      153 2020-05-05 15:05:35.000000 radical.analytics-1.5.0/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007/umgr.staging.output.0.prof
--rw-r--r--   0 mturilli   (501) staff       (20)  8548352 2020-05-05 15:05:35.000000 radical.analytics-1.5.0/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007/update.0.child.prof
--rw-r--r--   0 mturilli   (501) staff       (20)      436 2020-05-05 15:05:35.000000 radical.analytics-1.5.0/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007/update.0.prof
--rw-r--r--   0 mturilli   (501) staff       (20)  3762696 2020-05-05 15:05:35.000000 radical.analytics-1.5.0/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007.json
--rw-r--r--   0 mturilli   (501) staff       (20)     6185 2020-08-11 13:23:09.000000 radical.analytics-1.5.0/tests/test_duration_method.py
--rw-r--r--   0 mturilli   (501) staff       (20)    28947 2020-08-11 13:23:09.000000 radical.analytics-1.5.0/tests/test_entity.py
--rw-r--r--   0 mturilli   (501) staff       (20)      277 2020-05-05 15:05:35.000000 radical.analytics-1.5.0/tests/test_session.py
+drwxr-xr-x   0 mturilli   (501) staff       (20)        0 2021-07-08 08:08:44.969621 radical.analytics-1.6.7/
+-rw-r--r--   0 mturilli   (501) staff       (20)     5822 2021-07-08 08:06:17.000000 radical.analytics-1.6.7/CHANGES.md
+-rw-r--r--   0 mturilli   (501) staff       (20)     1093 2021-07-08 08:04:41.000000 radical.analytics-1.6.7/LICENSE
+-rw-r--r--   0 mturilli   (501) staff       (20)      115 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/MANIFEST.in
+-rw-r--r--   0 mturilli   (501) staff       (20)      958 2021-07-08 08:08:44.969018 radical.analytics-1.6.7/PKG-INFO
+-rw-r--r--   0 mturilli   (501) staff       (20)     1139 2021-07-08 08:04:41.000000 radical.analytics-1.6.7/README.md
+-rw-r--r--   0 mturilli   (501) staff       (20)        6 2021-07-08 08:06:17.000000 radical.analytics-1.6.7/VERSION
+drwxr-xr-x   0 mturilli   (501) staff       (20)        0 2021-07-08 08:08:44.750461 radical.analytics-1.6.7/bin/
+-rwxr-xr-x   0 mturilli   (501) staff       (20)     4756 2021-07-08 08:04:41.000000 radical.analytics-1.6.7/bin/radical-analytics-check
+-rwxr-xr-x   0 mturilli   (501) staff       (20)     6006 2021-07-08 08:04:41.000000 radical.analytics-1.6.7/bin/radical-analytics-inspect
+-rwxr-xr-x   0 mturilli   (501) staff       (20)    10588 2021-07-08 08:04:41.000000 radical.analytics-1.6.7/bin/radical-analytics-plot.py
+-rwxr-xr-x   0 mturilli   (501) staff       (20)       88 2020-08-11 13:23:09.000000 radical.analytics-1.6.7/bin/radical-analytics-version
+-rwxr-xr-x   0 mturilli   (501) staff       (20)    36969 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/bin/radical-analytics-wrangler.py
+drwxr-xr-x   0 mturilli   (501) staff       (20)        0 2021-07-08 08:08:44.753940 radical.analytics-1.6.7/bin/rp_inspect/
+-rwxr-xr-x   0 mturilli   (501) staff       (20)     3198 2021-07-08 08:04:41.000000 radical.analytics-1.6.7/bin/rp_inspect/plot_conc.py
+-rwxr-xr-x   0 mturilli   (501) staff       (20)     4937 2021-07-08 08:04:41.000000 radical.analytics-1.6.7/bin/rp_inspect/plot_dur.py
+-rwxr-xr-x   0 mturilli   (501) staff       (20)     2957 2021-07-08 08:04:41.000000 radical.analytics-1.6.7/bin/rp_inspect/plot_rate.py
+-rwxr-xr-x   0 mturilli   (501) staff       (20)     4824 2021-07-08 08:04:41.000000 radical.analytics-1.6.7/bin/rp_inspect/plot_state.py
+-rwxr-xr-x   0 mturilli   (501) staff       (20)     6903 2021-07-08 08:04:41.000000 radical.analytics-1.6.7/bin/rp_inspect/plot_util.py
+-rwxr-xr-x   0 mturilli   (501) staff       (20)     6785 2021-07-08 08:04:41.000000 radical.analytics-1.6.7/bin/rp_inspect/plot_util_2.py
+drwxr-xr-x   0 mturilli   (501) staff       (20)        0 2021-07-08 08:08:44.761312 radical.analytics-1.6.7/examples/
+-rwxr-xr-x   0 mturilli   (501) staff       (20)     3017 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/examples/00_session_describe_rp.py
+-rwxr-xr-x   0 mturilli   (501) staff       (20)     2514 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/examples/01_session_list_rp.py
+-rwxr-xr-x   0 mturilli   (501) staff       (20)     4166 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/examples/02_session_get_rp.py
+-rwxr-xr-x   0 mturilli   (501) staff       (20)     3036 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/examples/03_session_filter_rp.py
+-rwxr-xr-x   0 mturilli   (501) staff       (20)     4465 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/examples/04_session_duration_rp.py
+-rwxr-xr-x   0 mturilli   (501) staff       (20)     1520 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/examples/05_relationsships.py
+-rwxr-xr-x   0 mturilli   (501) staff       (20)     4856 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/examples/06_events.py
+-rwxr-xr-x   0 mturilli   (501) staff       (20)     1289 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/examples/06_ra_events.py
+-rwxr-xr-x   0 mturilli   (501) staff       (20)     4827 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/examples/07_event_timeline.py
+-rwxr-xr-x   0 mturilli   (501) staff       (20)     5940 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/examples/08_core_utilization_plot.py
+-rwxr-xr-x   0 mturilli   (501) staff       (20)     8909 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/examples/08c_core_utilization_plot.py
+-rwxr-xr-x   0 mturilli   (501) staff       (20)     4990 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/examples/09_session_plots.py
+-rwxr-xr-x   0 mturilli   (501) staff       (20)     4717 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/examples/10_durations.py
+-rw-r--r--   0 mturilli   (501) staff       (20)       38 2021-07-08 08:08:44.969798 radical.analytics-1.6.7/setup.cfg
+-rwxr-xr-x   0 mturilli   (501) staff       (20)     9903 2021-07-08 08:06:17.000000 radical.analytics-1.6.7/setup.py
+drwxr-xr-x   0 mturilli   (501) staff       (20)        0 2021-07-08 08:08:44.742047 radical.analytics-1.6.7/src/
+drwxr-xr-x   0 mturilli   (501) staff       (20)        0 2021-07-08 08:08:44.742210 radical.analytics-1.6.7/src/radical/
+drwxr-xr-x   0 mturilli   (501) staff       (20)        0 2021-07-08 08:08:44.817963 radical.analytics-1.6.7/src/radical/analytics/
+-rw-r--r--   0 mturilli   (501) staff       (20)       47 2021-07-08 08:08:44.000000 radical.analytics-1.6.7/src/radical/analytics/SDIST
+-rw-r--r--   0 mturilli   (501) staff       (20)       22 2021-07-08 08:08:44.000000 radical.analytics-1.6.7/src/radical/analytics/VERSION
+-rw-r--r--   0 mturilli   (501) staff       (20)     1361 2021-07-08 08:04:41.000000 radical.analytics-1.6.7/src/radical/analytics/__init__.py
+-rw-r--r--   0 mturilli   (501) staff       (20)    17509 2021-07-08 08:04:41.000000 radical.analytics-1.6.7/src/radical/analytics/entity.py
+-rw-r--r--   0 mturilli   (501) staff       (20)     4631 2021-07-08 08:04:41.000000 radical.analytics-1.6.7/src/radical/analytics/experiment.py
+-rw-r--r--   0 mturilli   (501) staff       (20)     6514 2020-06-23 08:47:15.000000 radical.analytics-1.6.7/src/radical/analytics/plotter.py
+-rw-r--r--   0 mturilli   (501) staff       (20)    56570 2021-07-08 08:04:41.000000 radical.analytics-1.6.7/src/radical/analytics/session.py
+drwxr-xr-x   0 mturilli   (501) staff       (20)        0 2021-07-08 08:08:44.819208 radical.analytics-1.6.7/src/radical/analytics/utils/
+-rw-r--r--   0 mturilli   (501) staff       (20)      581 2021-07-08 08:04:41.000000 radical.analytics-1.6.7/src/radical/analytics/utils/__init__.py
+-rw-r--r--   0 mturilli   (501) staff       (20)    14771 2021-07-08 08:04:41.000000 radical.analytics-1.6.7/src/radical/analytics/utils/plot.py
+drwxr-xr-x   0 mturilli   (501) staff       (20)        0 2021-07-08 08:08:44.765025 radical.analytics-1.6.7/src/radical.analytics.egg-info/
+-rw-r--r--   0 mturilli   (501) staff       (20)      958 2021-07-08 08:08:44.000000 radical.analytics-1.6.7/src/radical.analytics.egg-info/PKG-INFO
+-rw-r--r--   0 mturilli   (501) staff       (20)     4376 2021-07-08 08:08:44.000000 radical.analytics-1.6.7/src/radical.analytics.egg-info/SOURCES.txt
+-rw-r--r--   0 mturilli   (501) staff       (20)        1 2021-07-08 08:08:44.000000 radical.analytics-1.6.7/src/radical.analytics.egg-info/dependency_links.txt
+-rw-r--r--   0 mturilli   (501) staff       (20)        8 2021-07-08 08:08:44.000000 radical.analytics-1.6.7/src/radical.analytics.egg-info/namespace_packages.txt
+-rw-r--r--   0 mturilli   (501) staff       (20)        1 2021-07-08 08:08:44.000000 radical.analytics-1.6.7/src/radical.analytics.egg-info/not-zip-safe
+-rw-r--r--   0 mturilli   (501) staff       (20)       83 2021-07-08 08:08:44.000000 radical.analytics-1.6.7/src/radical.analytics.egg-info/requires.txt
+-rw-r--r--   0 mturilli   (501) staff       (20)        8 2021-07-08 08:08:44.000000 radical.analytics-1.6.7/src/radical.analytics.egg-info/top_level.txt
+drwxr-xr-x   0 mturilli   (501) staff       (20)        0 2021-07-08 08:08:44.819699 radical.analytics-1.6.7/styles/
+-rw-r--r--   0 mturilli   (501) staff       (20)     1675 2021-07-08 08:04:41.000000 radical.analytics-1.6.7/styles/radical_mpl.txt
+drwxr-xr-x   0 mturilli   (501) staff       (20)        0 2021-07-08 08:08:44.821709 radical.analytics-1.6.7/tests/
+-rw-r--r--   0 mturilli   (501) staff       (20)        0 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/__init__.py
+drwxr-xr-x   0 mturilli   (501) staff       (20)        0 2021-07-08 08:08:44.822394 radical.analytics-1.6.7/tests/barrier_data/
+drwxr-xr-x   0 mturilli   (501) staff       (20)        0 2021-07-08 08:08:44.834169 radical.analytics-1.6.7/tests/barrier_data/rp.session.two.jdakka.017395.0000/
+-rw-r--r--   0 mturilli   (501) staff       (20)     1291 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/barrier_data/rp.session.two.jdakka.017395.0000/pmgr.0000.prof
+-rw-r--r--   0 mturilli   (501) staff       (20)        0 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/barrier_data/rp.session.two.jdakka.017395.0000/pmgr.launching.0.child.prof
+-rw-r--r--   0 mturilli   (501) staff       (20)      486 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/barrier_data/rp.session.two.jdakka.017395.0000/pmgr.launching.0.prof
+-rw-r--r--   0 mturilli   (501) staff       (20)      855 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/barrier_data/rp.session.two.jdakka.017395.0000/rp.session.two.jdakka.017395.0000.prof
+-rw-r--r--   0 mturilli   (501) staff       (20)   339968 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/barrier_data/rp.session.two.jdakka.017395.0000/umgr.0000.prof
+-rw-r--r--   0 mturilli   (501) staff       (20)    93001 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/barrier_data/rp.session.two.jdakka.017395.0000/umgr.scheduling.0.child.prof
+-rw-r--r--   0 mturilli   (501) staff       (20)      144 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/barrier_data/rp.session.two.jdakka.017395.0000/umgr.scheduling.0.prof
+-rw-r--r--   0 mturilli   (501) staff       (20)    83051 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/barrier_data/rp.session.two.jdakka.017395.0000/umgr.staging.input.0.child.prof
+-rw-r--r--   0 mturilli   (501) staff       (20)      148 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/barrier_data/rp.session.two.jdakka.017395.0000/umgr.staging.input.0.prof
+-rw-r--r--   0 mturilli   (501) staff       (20)    79361 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/barrier_data/rp.session.two.jdakka.017395.0000/umgr.staging.output.0.child.prof
+-rw-r--r--   0 mturilli   (501) staff       (20)      149 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/barrier_data/rp.session.two.jdakka.017395.0000/umgr.staging.output.0.prof
+-rw-r--r--   0 mturilli   (501) staff       (20)   647168 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/barrier_data/rp.session.two.jdakka.017395.0000/update.0.child.prof
+-rw-r--r--   0 mturilli   (501) staff       (20)      430 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/barrier_data/rp.session.two.jdakka.017395.0000/update.0.prof
+-rw-r--r--   0 mturilli   (501) staff       (20)   426921 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/barrier_data/rp.session.two.jdakka.017395.0000.json
+drwxr-xr-x   0 mturilli   (501) staff       (20)        0 2021-07-08 08:08:44.839229 radical.analytics-1.6.7/tests/example-data/
+-rw-r--r--   0 mturilli   (501) staff       (20)     7071 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/example-data/pilot-entity-example.json
+-rw-r--r--   0 mturilli   (501) staff       (20)     1503 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/example-data/pmgr-entity-example.json
+-rw-r--r--   0 mturilli   (501) staff       (20)     7057 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/example-data/range-testing-entity-example.json
+-rw-r--r--   0 mturilli   (501) staff       (20)    22261 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/example-data/rp-entity-example.json
+-rw-r--r--   0 mturilli   (501) staff       (20)     3543 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/example-data/umgr-entity-example.json
+-rw-r--r--   0 mturilli   (501) staff       (20)    13630 2021-07-08 08:04:41.000000 radical.analytics-1.6.7/tests/example-data/unit-entity-example.json
+drwxr-xr-x   0 mturilli   (501) staff       (20)        0 2021-07-08 08:08:44.913094 radical.analytics-1.6.7/tests/no_barrier_data/
+drwxr-xr-x   0 mturilli   (501) staff       (20)        0 2021-07-08 08:08:44.967522 radical.analytics-1.6.7/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007/
+-rw-r--r--   0 mturilli   (501) staff       (20)     1208 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007/pmgr.0000.prof
+-rw-r--r--   0 mturilli   (501) staff       (20)        0 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007/pmgr.launching.0.child.prof
+-rw-r--r--   0 mturilli   (501) staff       (20)      492 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007/pmgr.launching.0.prof
+-rw-r--r--   0 mturilli   (501) staff       (20)     1207 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007.prof
+-rw-r--r--   0 mturilli   (501) staff       (20)  3768320 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007/umgr.0000.prof
+-rw-r--r--   0 mturilli   (501) staff       (20)   847228 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007/umgr.scheduling.0.child.prof
+-rw-r--r--   0 mturilli   (501) staff       (20)      149 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007/umgr.scheduling.0.prof
+-rw-r--r--   0 mturilli   (501) staff       (20)   756110 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007/umgr.staging.input.0.child.prof
+-rw-r--r--   0 mturilli   (501) staff       (20)      150 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007/umgr.staging.input.0.prof
+-rw-r--r--   0 mturilli   (501) staff       (20)   722324 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007/umgr.staging.output.0.child.prof
+-rw-r--r--   0 mturilli   (501) staff       (20)      153 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007/umgr.staging.output.0.prof
+-rw-r--r--   0 mturilli   (501) staff       (20)  8548352 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007/update.0.child.prof
+-rw-r--r--   0 mturilli   (501) staff       (20)      436 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007/update.0.prof
+-rw-r--r--   0 mturilli   (501) staff       (20)  3762696 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007.json
+-rw-r--r--   0 mturilli   (501) staff       (20)     6185 2020-08-11 13:34:20.000000 radical.analytics-1.6.7/tests/test_duration_method.py
+-rw-r--r--   0 mturilli   (501) staff       (20)    28947 2020-08-11 13:34:20.000000 radical.analytics-1.6.7/tests/test_entity.py
+-rw-r--r--   0 mturilli   (501) staff       (20)      277 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/test_session.py
```

### Comparing `radical.analytics-1.5.0/CHANGES.md` & `radical.analytics-1.6.7/CHANGES.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,162 +1,150 @@
 
-  - For a list of bug fixes, see:
-    https://github.com/radical-cybertools/radical.analytics/issues?q=is%3Aissue+is%3Aclosed+sort%3Aupdated-desc
-  - For a list of open issues and known problems, see:
-    https://github.com/radical-cybertools/radical.analytics/issues?q=is%3Aissue+is%3Aopen+
+- For a list of bug fixes, see:
+    <https://github.com/radical-cybertools/radical.analytics/issues?q=is%3Aissue+is%3Aclosed+sort%3Aupdated-desc>
+- For a list of open issues and known problems, see:
+    <https://github.com/radical-cybertools/radical.analytics/issues?q=is%3Aissue+is%3Aopen>
+
+1.6.7 Release                                                         2021-07-08
+--------------------------------------------------------------------------------
 
+- utils/plot.py: help functions for plotting with Matplotlib
+- style/radical_mpl.txt: default Matplotlib style for publication-grade plots.
+- Separate type of resources (e.g., 'cpu', 'gpu) in resource utilization plot
+- New utilization plot. aggregated utilization to improve performance and scale
+- Documentation: Resource utilization, renaming compute unit -> task
+- Tools: bin/rp_inspect/*.py plot 4 metrics for RP sessions
+- Various bug fixes
 
 1.5.0 Release                                                         2020-08-04
 --------------------------------------------------------------------------------
 
-  - Move to Python 3
-  - Fix multiple bugs
-  - Align with release number of RCT stack
-  - Linting and RCT best code practices
-  - New documentation
-
+- Move to Python 3
+- Fix multiple bugs
+- Align with release number of RCT stack
+- Linting and RCT best code practices
+- New documentation
 
 0.72.1 Hotfix Release                                                 2019-09-28
 --------------------------------------------------------------------------------
 
-  - fix #102
-
+- fix #102
 
 0.72.0 Release                                                        2019-09-11
 --------------------------------------------------------------------------------
 
-  - introduce analytics.Experiment class and move utilization method to it
-  - sessions are now cached
-  - Expand upon modeling TTX
-  - TTC diagrams
-  - add jsrun version of metrics
-  - add quick plotter script
-  - documentation
-  - entity.ranges() *always* returns a list
-  - experiment level utilization plots
-  - fix off-by-one error
-  - increase timer precision
-  - re-align utilization plot with pilot runtime
-  - recursive profiles for RA sessions
-  - support bz2
-  - support global session time shift (session.tzero)
-
+- introduce analytics.Experiment class and move utilization method to it
+- sessions are now cached
+- Expand upon modeling TTX
+- TTC diagrams
+- add jsrun version of metrics
+- add quick plotter script
+- documentation
+- entity.ranges() *always* returns a list
+- experiment level utilization plots
+- fix off-by-one error
+- increase timer precision
+- re-align utilization plot with pilot runtime
+- recursive profiles for RA sessions
+- support bz2
+- support global session time shift (session.tzero)
 
 0.70.0 Release                                                        2019-07-07
 --------------------------------------------------------------------------------
 
-  - plot improvements
-  - fix tarball handling
-
+- plot improvements
+- fix tarball handling
 
 0.60.1 Hotfix                                                         2019-05-28
 --------------------------------------------------------------------------------
 
-  - fix deployement dependency (thanks Matteo!)
-
+- fix deployment dependency (thanks Matteo!)
 
 0.60.0 Release                                                        2019-04-10
 --------------------------------------------------------------------------------
 
-  - fail on and mark missing mandatory events
-  - add a native radical.analytics session (#63)
-  - add events to capture pre-exec durations (#67)
-  - add consistency check
-  - add allocation plot script
-  - add figure size option
-  - add plotting class
-  - add concurrency plot
-  - add statistics
-  - add utilization plot
-  - example fixes
-  - fix issue (#74)
-  - fix logger creation
-  - fix prints in wrangler
-  - apply coding guidelines
-
+- fail on and mark missing mandatory events
+- add a native radical.analytics session (#63)
+- add events to capture pre-exec durations (#67)
+- add consistency check
+- add allocation plot script
+- add figure size option
+- add plotting class
+- add concurrency plot
+- add statistics
+- add utilization plot
+- example fixes
+- fix issue (#74)
+- fix logger creation
+- fix prints in wrangler
+- apply coding guidelines
 
 0.50.4 Release                                                        2018-12-20
 --------------------------------------------------------------------------------
 
-  - make pypi happy
-
+- make pypi happy
 
 0.50.3 Release                                                        2018-12-19
 --------------------------------------------------------------------------------
 
-  - fix license inconsistency
-
+- fix license inconsistency
 
 0.50.2 Release                                                        2018-12-19
 --------------------------------------------------------------------------------
 
-  - add license file
-
+- add license file
 
 0.50.1 Release                                                        2018-11-20
 --------------------------------------------------------------------------------
 
-  - fixes to EnTK integration
-
+- fixes to EnTK integration
 
 0.50.0 Release                                                        2018-08-20
 --------------------------------------------------------------------------------
 
-  - support sessions which only have profiles, but a limited or no event or
-    state model
-
-
+- support sessions which only have profiles, but a limited or no event or state model
 
 0.47 Release                                                          2017-11-19
 --------------------------------------------------------------------------------
 
-  - Adding plotting class
-  - add concurrency plot
-  - PR #41
-  - If ranges is empty do nothing, else update dict.
-    Value of dict is a list of lists in case there are more than one ranges
-  - Single session, multiple pilots utilization
-  - TTC diagrams
-  - Utilization method. For the moment single RP session, single pilot
-  - add several examples
-  - add time filter tests
-  - add valid range testing
-  - adding test case for the magic function -- currently test fails for dataset
-    with execution barrier
-  - behave on empty event queries
-  - better testing for time filters
-  - entk integration
-  - entity.ranges() *always* returns a list
-  - event profiling cleanup
-  - expose session id
-  - expose stats, new event type
-  - ignore gitignore
-  - import matplotlib only if needed, to avoid hard dependency
-  - keep up with RU changes
-  - make sure we get session ID from an experiment dir
-  - mocking tests file structure, better .gitignore
-  - owner and consumer are mandatory inputs in the API call
-  - remove unwanted files
-  - support tarballs tarballs: those named "sid.tbz" etc. are now transparently
-    unpacked and used.
-  - testing ranges
-  - tests require pytest
-  - use empty range set and "None" to indicate condition mismatch
-  - work on RA memory consumption
-
+- Adding plotting class
+- add concurrency plot
+- PR #41
+- If ranges is empty do nothing, else update dict. Value of dict is a list of lists in case there are more than one ranges
+- Single session, multiple pilots utilization
+- TTC diagrams
+- Utilization method. For the moment single RP session, single pilot
+- add several examples
+- add time filter tests
+- add valid range testing
+- adding test case for the magic function -- currently test fails for dataset with execution barrier
+- behave on empty event queries
+- better testing for time filters
+- entk integration
+- entity.ranges() *always* returns a list
+- event profiling cleanup
+- expose session id
+- expose stats, new event type
+- ignore gitignore
+- import matplotlib only if needed, to avoid hard dependency
+- keep up with RU changes
+- make sure we get session ID from an experiment dir
+- mocking tests file structure, better .gitignore
+- owner and consumer are mandatory inputs in the API call
+- remove unwanted files
+- support tarballs tarballs: those named "sid.tbz" etc. are now transparently unpacked and used.
+- testing ranges
+- tests require pytest
+- use empty range set and "None" to indicate condition mismatch
+- work on RA memory consumption
 
 0.45 Release                                                          2017-02-28
 --------------------------------------------------------------------------------
 
-  - clean out repository
-  - sync branches
-  - sync version across radical stack
-
+- clean out repository
+- sync branches
+- sync version across radical stack
 
 0.1  Release                                                          2016-02-20
 --------------------------------------------------------------------------------
 
-  - initial release
-
-
---------------------------------------------------------------------------------
-
+- initial release
```

### Comparing `radical.analytics-1.5.0/PKG-INFO` & `radical.analytics-1.6.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: radical.analytics
-Version: 1.5.0
+Version: 1.6.7
 Summary: The RADICAL analytics framework
 Home-page: https://www.github.com/radical-cybertools/radical.analytics/
 Author: RADICAL Group at Rutgers University
 Author-email: radical@rutgers.edu
 Maintainer: The RADICAL Devel Team
 Maintainer-email: radical@rutgers.edu
 License: MIT
```

### Comparing `radical.analytics-1.5.0/README.md` & `radical.analytics-1.6.7/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,10 @@
-# radical.analytics
+# RADICAL-Analytics (RA)
 
-[RADICAL-Anlytics](https://github.com/radical-cybertools/radical.analytics) is a library supporting the analysis of data produced by the [RADICAL-Cybertools](https://radical-cybertools.github.io/). Currently, RADICAL-Analytics supports [RADICAL-Pilot (RP)](https://github.com/radical-cybertools/radical.pilot) and [RADICAl-EnsembleToolkit (EnTK)](https://github.com/radical-cybertools/radical.entk). RADICAL-Analytics supports the experimental analyses [published](http://radical.rutgers.edu/publications/) by the [RADICAL Group](http://radical.rutgers.edu/) at Rutgers University.
+[![Build Status](https://github.com/radical-cybertools/radical.analytics/actions/workflows/python-app.yml/badge.svg)](https://github.com/radical-cybertools/radical.analytics/actions/workflows/python-app.yml)
+[![codecov](https://codecov.io/gh/radical-cybertools/radical.analytics/branch/devel/graph/badge.svg)](https://codecov.io/gh/radical-cybertools/radical.analytics)
+
+[RADICAL-Analytics](https://github.com/radical-cybertools/radical.analytics) is a library supporting the analysis of data produced by the [RADICAL-Cybertools](https://radical-cybertools.github.io/). Currently, RADICAL-Analytics supports [RADICAL-Pilot (RP)](https://github.com/radical-cybertools/radical.pilot) and [RADICAl-EnsembleToolkit (EnTK)](https://github.com/radical-cybertools/radical.entk). RADICAL-Analytics supports the experimental analyses [published](http://radical.rutgers.edu/publications/) by the [RADICAL Group](http://radical.rutgers.edu/) at Rutgers University.
 
 ## Documentation
 * General: https://radicalanalytics.readthedocs.io/en/latest/index.html
 * API: https://radicalanalytics.readthedocs.io/en/latest/apidoc.html
```

### Comparing `radical.analytics-1.5.0/bin/radical-analytics-check` & `radical.analytics-1.6.7/bin/radical-analytics-check`

 * *Files 3% similar despite different names*

```diff
@@ -105,33 +105,33 @@
     smodel = session._description['entities']['pilot']['state_model']
     for s in {k: v for k, v in sorted(smodel.items(), key=lambda item: item[1])}:
         print('            %9d : %s' % (states.get(s, 0), s))
 
 
 
     print()
-    print('  units   : %9d' % len(session.get(etype='unit')))
+    print('  tasks   : %9d' % len(session.get(etype='task')))
     uetypes = dict()
     states  = dict()
-    for u in session.get(etype='unit'):
+    for u in session.get(etype=['task', 'master', 'worker', 'request']):
         for e in u.events:
             t = e[ru.EVENT]
             if t not in uetypes: uetypes[t]  = 1
             else               : uetypes[t] += 1
             if t == 'state':
                 s = e[ru.STATE]
                 if s not in states: states[s]  = 1
                 else              : states[s] += 1
     for t in sorted(uetypes.keys()):
         print('            %9d : %s' % (uetypes[t], t))
         n_events += uetypes[t]
     n_types += len(uetypes.keys())
 
     print()
-    smodel = session._description['entities']['unit']['state_model']
+    smodel = session._description['entities']['task']['state_model']
     for s in {k: v for k, v in sorted(smodel.items(), key=lambda item: item[1])}:
         print('            %9d : %s' % (states.get(s, 0), s))
 
 
     print()
     print('  total   : %9d  (%d types)' % (n_events, n_types))
```

### Comparing `radical.analytics-1.5.0/bin/radical-analytics-inspect` & `radical.analytics-1.6.7/bin/radical-analytics-inspect`

 * *Files 8% similar despite different names*

```diff
@@ -103,33 +103,30 @@
                       The x-axis is time, the y-axis is an integer index over
                       resource elements (cpus and gpus).  The coloring of the
                       entries shows how the specific resource element has been
                       used at that point in time, and also shows in many cases
                       why a specific resource element has *not* been used for
                       task execution at that point in time (overhead).
 
-                      An additional utilization plot (util.png) is provided to
-                      compare utilization across all given sessions (sorted by
-                      pilot size and number of units).  This plot is only
-                      produced when this script is called with multiple
-                      sessions.
-                      (TODO)
-
+         utilization: (\$sid.\$pid.util.png)
+                      Plot the resource utilization for each pilot is plotted
+                      as percentage over time.
 EOT
 }
 
 test -z "$ARGS"          && usage "missing session ID(s)"
 test    "$ARGS" = "-h"   && usage
 test    "$ARGS" = "help" && usage
 
 for session in $ARGS
 do
     sid=$(basename $session)
     echo -n "$sid "
-    $bin/rp_inspect/plot_state.py "$session" && echo -n .
-    $bin/rp_inspect/plot_dur.py   "$session" && echo -n .
-    $bin/rp_inspect/plot_conc.py  "$session" && echo -n .
-    $bin/rp_inspect/plot_rate.py  "$session" && echo -n .
-    $bin/rp_inspect/plot_util.py  "$session" && echo -n .
+    echo 'STATE:'; $bin/rp_inspect/plot_state.py  "$session" && echo -n .
+    echo 'DUR  :'; $bin/rp_inspect/plot_dur.py    "$session" && echo -n .
+    echo 'CONC :'; $bin/rp_inspect/plot_conc.py   "$session" && echo -n .
+    echo 'RATE :'; $bin/rp_inspect/plot_rate.py   "$session" && echo -n .
+    echo 'UTIL :'; $bin/rp_inspect/plot_util.py   "$session" && echo -n .
+    echo 'UTIL2:'; $bin/rp_inspect/plot_util_2.py "$session" && echo -n .
     echo " done"
 done
```

### Comparing `radical.analytics-1.5.0/bin/radical-analytics-wrangler.py` & `radical.analytics-1.6.7/bin/radical-analytics-wrangler.py`

 * *Files identical despite different names*

### Comparing `radical.analytics-1.5.0/bin/rp_inspect/plot_conc.py` & `radical.analytics-1.6.7/bin/rp_inspect/plot_rate.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,77 +8,82 @@
 
 import matplotlib.pyplot as plt
 
 import radical.utils     as ru
 import radical.pilot     as rp
 import radical.analytics as ra
 
+from radical.analytics.utils import to_latex
+
+
+# ----------------------------------------------------------------------------
+#
+plt.style.use(ra.get_mplstyle("radical_mpl"))
+
+
+# ----------------------------------------------------------------------------
+#
 states  = [
            [rp.NEW                          , '#660000'],
-         # [rp.UMGR_SCHEDULING_PENDING      , '#000000'],
-           [rp.UMGR_SCHEDULING              , '#666600'],
-         # [rp.UMGR_STAGING_INPUT_PENDING   , '#000000'],
-           [rp.UMGR_STAGING_INPUT           , '#006600'],
+         # [rp.TMGR_SCHEDULING_PENDING      , '#000000'],
+           [rp.TMGR_SCHEDULING              , '#666600'],
+         # [rp.TMGR_STAGING_INPUT_PENDING   , '#000000'],
+           [rp.TMGR_STAGING_INPUT           , '#006600'],
          # [rp.AGENT_STAGING_INPUT_PENDING  , '#000000'],
            [rp.AGENT_STAGING_INPUT          , '#006666'],
          # [rp.AGENT_SCHEDULING_PENDING     , '#000000'],
            [rp.AGENT_SCHEDULING             , '#000066'],
            [rp.AGENT_EXECUTING_PENDING      , '#000000'],
            [rp.AGENT_EXECUTING              , '#660066'],
          # [rp.AGENT_STAGING_OUTPUT_PENDING , '#000000'],
            [rp.AGENT_STAGING_OUTPUT         , '#990000'],
-         # [rp.UMGR_STAGING_OUTPUT_PENDING  , '#000000'],
-           [rp.UMGR_STAGING_OUTPUT          , '#009900'],
+         # [rp.TMGR_STAGING_OUTPUT_PENDING  , '#000000'],
+           [rp.TMGR_STAGING_OUTPUT          , '#009900'],
            [rp.DONE                         , '#00CC00'],
            [rp.FAILED                       , '#FF0000'],
            [rp.CANCELED                     , '#AA00AA'],
           ]
-# state to sort units by
-state_key = rp.AGENT_EXECUTING
-state_key = rp.NEW
-
 
-metrics = {'Unit Scheduling': [{ru.STATE: 'AGENT_SCHEDULING'},
-                               {ru.EVENT: 'schedule_ok'     }],
-           'Unit Execution' : [{ru.EVENT: 'exec_start'      },
-                               {ru.EVENT: 'exec_stop'       }],
-}
 
-colors  = {'Unit Scheduling': '#CC5555',
-           'Unit Execution' : '#55CC55'}
+metrics = {'Task Scheduling': {ru.EVENT: 'schedule_ok'},
+           'Task Execution' : {ru.EVENT: 'exec_start' },
+          }
+colors  = {'Task Scheduling': '#CC5555',
+           'Task Execution' : '#55CC55'}
 
 
 # ------------------------------------------------------------------------------
 #
 if __name__ == '__main__':
 
-    if len(sys.argv) != 2:
+    if len(sys.argv) < 2:
         print("\n\tusage: %s <dir|tarball>\n" % sys.argv[0])
         sys.exit(1)
 
-    src = sys.argv[1]
-    session = ra.Session.create(src, 'radical.pilot')
+    src     = sys.argv[1]
+    stype   = 'radical.pilot'
+    session = ra.Session.create(src, stype)
 
-    data = {metric: session.concurrency(event=metrics[metric])
+    # FIXME: adaptive sampling (100 bins over range?)
+    data = {metric: session.rate(event=metrics[metric], sampling=1.0)
             for metric in metrics}
 
-    # prep figure
-    fig  = plt.figure(figsize=(10,7))
-    ax   = fig.add_subplot(111)
+    fig, ax = plt.subplots(figsize=ra.get_plotsize(500))
 
     for metric in data:
         x = [e[0] for e in data[metric]]
         y = [e[1] for e in data[metric]]
-        plt.step(x, y, color=colors[metric], label=metric, where='post')
+        # FIXME: use cmap
+        ax.plot(x, y, color=colors[metric], label=to_latex(metric))
+      # ax.step(x, y, color=colors[metric], label=to_latex(metric),
+      #               where='post', linewidth=2, alpha=0.8)
+
+    ax.legend(to_latex(list(data.keys())))
+    # FIXME: why is the x-axis label gone?
+    plt.xlabel(to_latex('time [s]'))
+    plt.ylabel(to_latex('rate (#tasks / sec)'))
 
-    ax.legend(list(data.keys()), ncol=3, loc='upper center',
-                                 bbox_to_anchor=(0.5,1.11))
-    plt.xlabel('time [s]')
-    plt.ylabel('concurrency (#tasks)')
-
-    fig.savefig('%s_conc.png' % session.uid)
-  # plt.show()
+    fig.savefig('%s_rate.png' % session.uid)
 
 
 # ------------------------------------------------------------------------------
 
-
```

### Comparing `radical.analytics-1.5.0/bin/rp_inspect/plot_dur.py` & `radical.analytics-1.6.7/bin/rp_inspect/plot_dur.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,55 +1,60 @@
 #!/usr/bin/env python
 
 __copyright__ = 'Copyright 2013-2016, http://radical.rutgers.edu'
 __license__   = 'MIT'
 
 
 import sys
-import pprint
+
+import matplotlib.pyplot as plt
+import numpy             as np
 
 import radical.utils     as ru
 import radical.analytics as ra
 
-import matplotlib.pyplot as plt
-import numpy             as np
+from radical.analytics.utils import to_latex
+
+
+# ----------------------------------------------------------------------------
+#
+plt.style.use(ra.get_mplstyle("radical_mpl"))
 
 
 # We look into individual contributions of sub-durations to a larger duration.
 # The event list below will describe the whole duration (first to last event),
 # and the durations between subsequential events are considered contributing
 # sub-durations.  For each entity, we plot the times derived that way.
 #
-event_entity = 'unit'
-event_list   = \
-    [
+event_entity = 'task'
+event_list   = [
     # {ru.STATE: 'NEW'                          , ru.EVENT: 'state'           },
-    # {ru.STATE: 'UMGR_SCHEDULING_PENDING'      , ru.EVENT: 'state'           },
-    # {ru.STATE: 'UMGR_SCHEDULING'              , ru.EVENT: 'state'           },
-    # {ru.STATE: 'UMGR_STAGING_INPUT_PENDING'   , ru.EVENT: 'state'           },
-    # {ru.STATE: 'UMGR_STAGING_INPUT'           , ru.EVENT: 'state'           },
+    # {ru.STATE: 'TMGR_SCHEDULING_PENDING'      , ru.EVENT: 'state'           },
+    # {ru.STATE: 'TMGR_SCHEDULING'              , ru.EVENT: 'state'           },
+    # {ru.STATE: 'TMGR_STAGING_INPUT_PENDING'   , ru.EVENT: 'state'           },
+    # {ru.STATE: 'TMGR_STAGING_INPUT'           , ru.EVENT: 'state'           },
     # {ru.STATE: 'AGENT_STAGING_INPUT_PENDING'  , ru.EVENT: 'state'           },
     # {ru.STATE: None                           , ru.EVENT: 'get'             },
     # {ru.STATE: 'AGENT_STAGING_INPUT'          , ru.EVENT: 'state'           },
     # {ru.STATE: 'AGENT_SCHEDULING_PENDING'     , ru.EVENT: 'state'           },
       {ru.STATE: 'AGENT_SCHEDULING'             , ru.EVENT: 'state'           },
     # {ru.STATE: None                           , ru.EVENT: 'schedule_ok'     },
       {ru.STATE: 'AGENT_EXECUTING_PENDING'      , ru.EVENT: 'state'           },
       {ru.STATE: 'AGENT_EXECUTING'              , ru.EVENT: 'state'           },
       {ru.STATE: None                           , ru.EVENT: 'exec_start'      },
     # {ru.STATE: None                           , ru.EVENT: 'exec_ok'         },
       {ru.STATE: None                           , ru.EVENT: 'exec_stop'       },
     # {ru.STATE: None                           , ru.EVENT: 'unschedule_start'},
       {ru.STATE: None                           , ru.EVENT: 'unschedule_stop' },
     # {ru.STATE: 'AGENT_STAGING_OUTPUT_PENDING' , ru.EVENT: 'state'           },
-    # {ru.STATE: 'UMGR_STAGING_OUTPUT_PENDING'  , ru.EVENT: 'state'           },
-    # {ru.STATE: 'UMGR_STAGING_OUTPUT'          , ru.EVENT: 'state'           },
+    # {ru.STATE: 'TMGR_STAGING_OUTPUT_PENDING'  , ru.EVENT: 'state'           },
+    # {ru.STATE: 'TMGR_STAGING_OUTPUT'          , ru.EVENT: 'state'           },
     # {ru.STATE: 'AGENT_STAGING_OUTPUT'         , ru.EVENT: 'state'           },
     # {ru.STATE: 'DONE'                         , ru.EVENT: 'state'           },
-    ]
+]
 
 # ------------------------------------------------------------------------------
 #
 if __name__ == '__main__':
 
     if len(sys.argv) < 2:
         print("\n\tusage: %s <dir|tarball>\n" % sys.argv[0])
@@ -67,47 +72,54 @@
         for event in event_list:
             times = thing.timestamps(event=event)
             if times: tstamps.append(times[0])
             else    : tstamps.append(np.nan)
 
         data[thing.uid] = tstamps
 
-    # We sort the entities by the timestamp of the first event
-    # We also derive the durations, first the individual contributions, then the
-    # overall duration.
-    # timestamp in the list
-    sorted_things = sorted(list(data.items()), key=lambda e: e[1][0])
+    # We sort the entities by the timestamp of the last event (completion)
+    # We also derive the durations, first the overall duration, then the
+    # individual contributions.
+    sorted_things = sorted(list(data.items()), key=lambda e: e[1][-1])
     sorted_data   = list()
     index         = 0
     for uid,tstamps in sorted_things:
 
         durations = list()
-        durations.append(tstamps[-1] - tstamps[0])  # global duration
+        durations.append(tstamps[-1] - tstamps[0])  # overall duration
         for i in range(len(tstamps) - 1):
             durations.append(tstamps[i + 1] - tstamps[i])
 
         # create plottable data
         sorted_data.append([index] + durations)
         index += 1
 
     # create a numpyarray for plotting
     np_data = np.array(sorted_data)
-  # print(np_data)
 
-    plt.figure(figsize=(10,7))
+    fig, ax = plt.subplots(figsize=ra.get_plotsize(500))
+
     for e_idx in range(len(event_list)):
         if e_idx == 0:
             label = 'total'
         else:
-            label = '%s - %s' % (ru.event_to_label(event_list[e_idx - 1]),
-                                 ru.event_to_label(event_list[e_idx]))
-        plt.plot(np_data[:,0], np_data[:,(1 + e_idx)], label=label)
+            label = to_latex('%s - %s' % (ru.event_to_label(event_list[e_idx - 1]),
+                                          ru.event_to_label(event_list[e_idx])))
+        ax.plot(np_data[:,0], np_data[:,(1 + e_idx)], label=label)
 
     plt.yscale('log')
+
+    # FIXME: how to do the legend now?  With the large font size, I don't see
+    # a way to fit it anymore... :-/
+  # plt.legend(fancybox=True, shadow=True)
     plt.legend(loc='upper center', bbox_to_anchor=(0.5, 1.15),
           ncol=2, fancybox=True, shadow=True)
+
+    # FIXME: why is the x-axis label gone?
+    plt.xlabel(to_latex('task ID'))
+    plt.ylabel(to_latex('duration [sec]'))
     plt.savefig('%s_dur.png' % session.uid)
   # plt.show()
 
 
 # ------------------------------------------------------------------------------
```

### Comparing `radical.analytics-1.5.0/bin/rp_inspect/plot_state.py` & `radical.analytics-1.6.7/bin/rp_inspect/plot_state.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,26 +9,33 @@
 import radical.utils     as ru
 import radical.pilot     as rp
 import radical.analytics as ra
 
 import matplotlib.pyplot as plt
 import numpy             as np
 
+from radical.analytics.utils import to_latex
+
+
+# ----------------------------------------------------------------------------
+#
+plt.style.use(ra.get_mplstyle("radical_mpl"))
+
 
 # We plot timelines for all events listed in `event_list` for all entities of
 # type `event_entity`..  Before plotting, we sort those entities by the
 # timestamp of the first event in the event list
 
-event_entity = 'unit'
+event_entity = 'task'
 event_list   = [
     # {ru.STATE: rp.NEW                         , ru.EVENT: 'state'          },
-    # {ru.STATE: rp.UMGR_SCHEDULING_PENDING     , ru.EVENT: 'state'          },
-    # {ru.STATE: rp.UMGR_SCHEDULING             , ru.EVENT: 'state'          },
-    # {ru.STATE: rp.UMGR_STAGING_INPUT_PENDING  , ru.EVENT: 'state'          },
-    # {ru.STATE: rp.UMGR_STAGING_INPUT          , ru.EVENT: 'state'          },
+    # {ru.STATE: rp.TMGR_SCHEDULING_PENDING     , ru.EVENT: 'state'          },
+    # {ru.STATE: rp.TMGR_SCHEDULING             , ru.EVENT: 'state'          },
+    # {ru.STATE: rp.TMGR_STAGING_INPUT_PENDING  , ru.EVENT: 'state'          },
+    # {ru.STATE: rp.TMGR_STAGING_INPUT          , ru.EVENT: 'state'          },
     # {ru.STATE: rp.AGENT_STAGING_INPUT_PENDING , ru.EVENT: 'state'          },
     # {ru.COMP : 'agent_0'                      , ru.EVENT: 'get'            },
       {ru.STATE: rp.AGENT_STAGING_INPUT         , ru.EVENT: 'state'          },
       {ru.STATE: rp.AGENT_SCHEDULING_PENDING    , ru.EVENT: 'state'          },
       {ru.STATE: rp.AGENT_SCHEDULING            , ru.EVENT: 'state'          },
     # {ru.STATE: None                           , ru.EVENT: 'schedule_ok'    },
       {ru.STATE: rp.AGENT_EXECUTING_PENDING     , ru.EVENT: 'state'          },
@@ -38,16 +45,16 @@
     # {ru.STATE: None                           , ru.EVENT: 'exec_start'     },
     # {ru.STATE: None                           , ru.EVENT: 'app_start'      },
     # {ru.STATE: None                           , ru.EVENT: 'app_stop'       },
     # {ru.STATE: None                           , ru.EVENT: 'exec_ok'        },
     # {ru.STATE: None                           , ru.EVENT: 'exec_stop'      },
       {ru.STATE: rp.AGENT_STAGING_OUTPUT_PENDING, ru.EVENT: 'state'          },
       {ru.STATE: rp.AGENT_STAGING_OUTPUT        , ru.EVENT: 'state'          },
-    # {ru.STATE: rp.UMGR_STAGING_OUTPUT_PENDING , ru.EVENT: 'state'          },
-    # {ru.STATE: rp.UMGR_STAGING_OUTPUT         , ru.EVENT: 'state'          },
+    # {ru.STATE: rp.TMGR_STAGING_OUTPUT_PENDING , ru.EVENT: 'state'          },
+    # {ru.STATE: rp.TMGR_STAGING_OUTPUT         , ru.EVENT: 'state'          },
     # {ru.STATE: rp.DONE                        , ru.EVENT: 'state'          },
 ]
 
 
 # ------------------------------------------------------------------------------
 #
 if __name__ == '__main__':
@@ -81,15 +88,15 @@
 
   # diffs = list()
   # for uid in data:
   #     diffs.append(data[uid][-1] - data[uid][0])
   # print(sorted(diffs))
 
 
-  # sort x-axis (unit IDs) by
+  # sort x-axis (task IDs) by
   #     'uid'  : task ID
   #     'get'  : time of ingest
   #     'sched': time of sccheduling
   #     'pipe' : pipeline ID (RE sessions only)
     order = 'AGENT_EXECUTING state'
     index = 4
 
@@ -102,24 +109,24 @@
     index         = 0
     for uid in sorted_uids:
         sorted_data.append([index] + data[uid])
         index += 1
 
     np_data = np.array(sorted_data)
 
-    plt.figure(figsize=(10,7))
+    fig, ax = plt.subplots(figsize=ra.get_plotsize(500))
+
     for e_idx in range(len(event_list)):
-        plt.plot(np_data[:,0], np_data[:,(1 + e_idx)],
-                 label=ru.event_to_label(event_list[e_idx]))
-    plt.xlabel('task ID')
-    plt.ylabel('time [sec]')
-
-    plt.xlabel('task (sorted by %s)' % order)
-    plt.ylabel('time / sec')
-    plt.legend(loc='upper center', bbox_to_anchor=(0.5, 1.15),
-               ncol=2, fancybox=True, shadow=True)
+        ax.plot(np_data[:,0], np_data[:,(1 + e_idx)],
+                 label=to_latex(ru.event_to_label(event_list[e_idx])))
+
+    plt.xlabel(to_latex('task (sorted by %s)' % order))
+    plt.ylabel(to_latex('time [sec]'))
+
+    # FIXME: how to do the legend now?  With the large font size, I don't see
+    plt.legend()
     plt.savefig('%s.state.png' % session.uid)
   # plt.show()
 
 
 # ------------------------------------------------------------------------------
```

### Comparing `radical.analytics-1.5.0/bin/rp_inspect/plot_util.py` & `radical.analytics-1.6.7/examples/08c_core_utilization_plot.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 #!/usr/bin/env python
 
 __copyright__ = 'Copyright 2013-2016, http://radical.rutgers.edu'
 __license__   = 'MIT'
 
 
 import sys
+import pprint
 
+import numpy             as np
 import matplotlib        as mpl
 import matplotlib.pyplot as plt
 
-import radical.utils     as ru
 import radical.analytics as ra
 
 
 # This script plots the core utilization of a set of RP sessions in a stacked
 # barplot, where the stacked elements represent how the cores were (or were not)
 # utilized.  The elements will always add up to 100%, thus the whole bar
 # represents the amount of core-hours available to the session.  We only look at
@@ -92,108 +93,158 @@
 metrics = metrics_default
 
 
 # ------------------------------------------------------------------------------
 #
 if __name__ == '__main__':
 
-    if len(sys.argv) < 2:
-        print("\n\tusage: %s <dir|tarball>\n" % sys.argv[0])
-        sys.exit(1)
-
-    src = sys.argv[1]
-
-    if len(sys.argv) == 2: stype = 'radical.pilot'
-    else                 : stype = sys.argv[2]
-
-    session = ra.Session.create(src, stype)
-    sid     = session.uid
-    n_units = len(session.get(etype='unit'))
-    p_size  = 0
-    p_zero  = None
-    for pilot in session.get(etype='pilot'):
-        p_size += pilot.description['cores']
-        p_zero  = pilot.timestamps(event={ru.EVENT: 'bootstrap_0_start'})[0]
+    sources = sys.argv[1:]
+    xkeys   = dict()  # x-axis labels
+    sids    = list()  # need to sort SIDs
+
+    exp = ra.Experiment(sources, stype='radical.pilot')
+
+    # get the numbers we actually want to plot
+    for session in exp.sessions:
+
+        sid = session.uid
+        n_units = len(session.get(etype='unit'))
+        p_size  = 0
+        for pilot in session.get(etype='pilot'):
+            p_size += pilot.description['cores']
+
+        xkeys[sid] = [n_units, p_size]
+        sids.append(sid)
+
+    # sort sessions by pilot size
+    sids = sorted(sids, key=lambda sid: xkeys[sid][1])
+
 
     # get utilization information
-    prov, cons, stats_abs, stats_rel, info = session.utilization(metrics)
+    provided, consumed, stats_abs, stats_rel, info = exp.utilization(metrics=metrics)
+  # provided, consumed, stats_abs, stats_rel = exp.utilization(metrics='/path/metrics.json')
 
     with open('%s.stats' % sid, 'w') as fout:
         fout.write('\n%s\n\n' % info)
 
-  # import pprint
-  # pprint.pprint(prov)
-  # pprint.pprint(cons)
+  # pprint.pprint(provided)
+  # pprint.pprint(consumed)
   # pprint.pprint(stats_abs)
   # pprint.pprint(stats_rel)
 
     cmap = mpl.cm.get_cmap('tab20c')
 
     # --------------------------------------------------------------------------
     # core utilization over time (box plot)
-    fig  = plt.figure(figsize=(10,7))
-    ax   = fig.add_subplot(111)
+    for sid in sids:
+        fig  = plt.figure(figsize=(20,14))
+        ax   = fig.add_subplot(111)
+
+        step   = 1.0  / (len(metrics) + 1)
+        this   = step / 1.0
+        legend = list()
+
+        x_min = None
+        x_max = None
+        y_min = None
+        y_max = None
+
+        for metric in metrics:
+
+            color = cmap(this)
+            this += step
+
+            legend.append(mpl.lines.Line2D([0], [0], color=color, lw=6))
+
+            if isinstance(metric, list):
+                name  = metric[0]
+                parts = metric[1]
+            else:
+                name  = metric
+                parts = [metric]
+
+            for part in parts:
+                for uid in sorted(consumed[sid][part]):
+                    for block in consumed[sid][part][uid]:
+                        orig_x = block[0]
+                        orig_y = block[2] - 0.5
+                        width  = block[1] - block[0]
+                        height = block[3] - block[2] + 1.0
+
+                        if x_min is None: x_min = orig_x
+                        if x_max is None: x_max = orig_x + width
+                        if y_min is None: y_min = orig_x
+                        if y_max is None: y_max = orig_x + height
+
+                        x_min = min(x_min, orig_x)
+                        y_min = min(y_min, orig_y)
+                        x_max = max(x_max, orig_x + width)
+                        y_max = max(y_max, orig_y + height)
+
+                        patch = mpl.patches.Rectangle((orig_x, orig_y),
+                                                      width, height,
+                                                      facecolor=color,
+                                                      edgecolor='black',
+                                                      fill=True, lw=0.0)
+                        ax.add_patch(patch)
+
+        ax.legend(legend, [m[0] for m in metrics], ncol=6,
+                   loc='upper center', bbox_to_anchor=(0.5,1.11))
+        plt.xlabel('runtime [s]')
+        plt.ylabel('resource slot (index)')
+
+        plt.xlim([x_min, x_max])
+        plt.ylim([y_min, y_max])
+      # plt.xticks(list(range(int(x_min)-1, int(x_max)+1)))
+        fig.savefig('%s_core_allocation.png' % sid)
+        plt.show()
 
-    step   = 1.0  / (len(metrics) + 1)
-    this   = step / 1.0
-    legend = list()
-
-    x_min = None
-    x_max = None
-    y_min = None
-    y_max = None
 
-    for metric in metrics:
+    # --------------------------------------------------------------------------
+    # utilization: contributions as stacked barplot
+    #
+    # yes, stacked barplot is this cumbersome:
+    # http://matplotlib.org/examples/pylab_examples/bar_stacked.html
+    #
+    plt.figure(figsize=(20,14))
+    bottom = np.zeros(len(exp.sessions))
+    ind    = np.arange(len(exp.sessions))  # locations of bars on x-axis
+    width  = 0.35                          # width of bars
+
+    labels = list()
+    plots  = list()
+
+    for metric in metrics + ['Other']:
 
         color = cmap(this)
         this += step
 
         legend.append(mpl.lines.Line2D([0], [0], color=color, lw=6))
 
         if isinstance(metric, list):
             name  = metric[0]
             parts = metric[1]
         else:
             name  = metric
             parts = [metric]
 
-        for part in parts:
-            for uid in sorted(cons[part]):
-                for block in cons[part][uid]:
-                    orig_x = block[0] - p_zero
-                    orig_y = block[2] - 0.5
-                    width  = block[1] - block[0]
-                    height = block[3] - block[2] + 1.0
-
-                    if x_min is None: x_min = orig_x
-                    if x_max is None: x_max = orig_x + width
-                    if y_min is None: y_min = orig_y
-                    if y_max is None: y_max = orig_y + height
-
-                    x_min = min(x_min, orig_x)
-                    y_min = min(y_min, orig_y)
-                    x_max = max(x_max, orig_x + width)
-                    y_max = max(y_max, orig_y + height)
-
-                    patch = mpl.patches.Rectangle((orig_x, orig_y),
-                                                  width, height,
-                                                  facecolor=color,
-                                                  edgecolor='black',
-                                                  fill=True, lw=0.0)
-                    ax.add_patch(patch)
-
-    ax.legend(legend, [m[0] for m in metrics], ncol=5, loc='upper center',
-                                               bbox_to_anchor=(0.5,1.11))
-    plt.xlabel('runtime [s]')
-    plt.ylabel('resource slot (index)')
-
-    print([x_min, x_max])
-    plt.xlim([x_min, x_max])
-    plt.ylim([y_min, y_max])
-  # plt.xticks(list(range(int(x_min)-1, int(x_max)+1)))
-    fig.savefig('%s_util.png' % sid)
-  # plt.show()
+        values = [stats_rel[sid][name] for sid in sids]
+        plots.append(plt.bar(ind, values, width, bottom=bottom))
+        bottom += values
+        labels.append(name)
+
+    if False: plt.ylabel('utilization (% of total resources)')
+    else    : plt.ylabel('utilization (in core-seconds)')
+
+    plt.xlabel('#CU / #cores')
+    plt.ylabel('utilization (% of total resources)')
+    plt.title ('pilot utilization over workload size (#units)')
+    plt.xticks(ind, ['%s / %s' % (xkeys[sid][0], xkeys[sid][1]) for sid in sids])
+
+    plt.legend([p[0] for p in plots], labels, ncol=5, loc='upper left',
+               bbox_to_anchor=(0,1.13))
+    plt.savefig('08c_core_utilization.png')
+    plt.show()
 
 
 # ------------------------------------------------------------------------------
 
-
```

### Comparing `radical.analytics-1.5.0/examples/00_session_describe_rp.py` & `radical.analytics-1.6.7/examples/00_session_describe_rp.py`

 * *Files identical despite different names*

### Comparing `radical.analytics-1.5.0/examples/01_session_list_rp.py` & `radical.analytics-1.6.7/examples/01_session_list_rp.py`

 * *Files identical despite different names*

### Comparing `radical.analytics-1.5.0/examples/02_session_get_rp.py` & `radical.analytics-1.6.7/examples/02_session_get_rp.py`

 * *Files identical despite different names*

### Comparing `radical.analytics-1.5.0/examples/03_session_filter_rp.py` & `radical.analytics-1.6.7/examples/03_session_filter_rp.py`

 * *Files identical despite different names*

### Comparing `radical.analytics-1.5.0/examples/04_session_duration_rp.py` & `radical.analytics-1.6.7/examples/04_session_duration_rp.py`

 * *Files identical despite different names*

### Comparing `radical.analytics-1.5.0/examples/05_relationsships.py` & `radical.analytics-1.6.7/examples/05_relationsships.py`

 * *Files identical despite different names*

### Comparing `radical.analytics-1.5.0/examples/06_events.py` & `radical.analytics-1.6.7/examples/06_events.py`

 * *Files identical despite different names*

### Comparing `radical.analytics-1.5.0/examples/06_ra_events.py` & `radical.analytics-1.6.7/examples/06_ra_events.py`

 * *Files identical despite different names*

### Comparing `radical.analytics-1.5.0/examples/07_event_timeline.py` & `radical.analytics-1.6.7/examples/07_event_timeline.py`

 * *Files identical despite different names*

### Comparing `radical.analytics-1.5.0/examples/08_core_utilization_plot.py` & `radical.analytics-1.6.7/examples/08_core_utilization_plot.py`

 * *Files identical despite different names*

### Comparing `radical.analytics-1.5.0/examples/08c_core_utilization_plot.py` & `radical.analytics-1.6.7/bin/rp_inspect/plot_util.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 #!/usr/bin/env python
 
 __copyright__ = 'Copyright 2013-2016, http://radical.rutgers.edu'
 __license__   = 'MIT'
 
 
 import sys
-import pprint
 
-import numpy             as np
-import matplotlib        as mpl
 import matplotlib.pyplot as plt
 
+import radical.utils     as ru
 import radical.analytics as ra
 
+from radical.analytics.utils import to_latex
+
+
+# ----------------------------------------------------------------------------
+#
+plt.style.use(ra.get_mplstyle("radical_mpl"))
+
+
 
 # This script plots the core utilization of a set of RP sessions in a stacked
 # barplot, where the stacked elements represent how the cores were (or were not)
 # utilized.  The elements will always add up to 100%, thus the whole bar
 # represents the amount of core-hours available to the session.  We only look at
 # events on the agent side.
 #
@@ -24,38 +30,38 @@
 #
 #  - During bootstrap, configuration, setup, and termination, cores are
 #    essentially unused.  We separate out the times needed for those steps, and
 #    multiply by pilot size, to derive the number of core hours essentially
 #    spent on those activities (see `PILOT_DURATIONS` below).
 #
 #    NOTE: we assume that the pilot activities thus measured stop at the point
-#          when the first unit gets scheduled on a (set of) core(s), and
-#          restarts when the last unit gets unscheduled, as that is the time
+#          when the first task gets scheduled on a (set of) core(s), and
+#          restarts when the last task gets unscheduled, as that is the time
 #          frame where we in principle consider cores to be available to the
 #          workload.
 #
-#  - For each unit, we look at the amount of time that unit has been scheduled
+#  - For each task, we look at the amount of time that task has been scheduled
 #    on a set of cores, as those cores are then essentially blocked.  Multiplied
-#    by the size of the unit, that gives a number of core-hours those cores are
-#    'used' for that unit.
+#    by the size of the task, that gives a number of core-hours those cores are
+#    'used' for that task.
 #
 #    not all of that time is utilized for application use though: some is spent
 #    on preparation for execution, on spawning, unscheduling etc.  We separate
-#    out those utilizations for each unit.
+#    out those utilizations for each task.
 #
 #  - we consider core hours to be additive, in the following sense:
 #
 #    - all core-hours used by the pilot in various global activities listed in
-#      the first point, plus the sumof core hours spend by all units in various
+#      the first point, plus the sumof core hours spend by all tasks in various
 #      individual activities as in the second point, equals the overall core
 #      hours available to the pilot.
 #
-#      This only holds with one caveat: after the agent started to work on unit
+#      This only holds with one caveat: after the agent started to work on task
 #      execution, some cores may not *yet* be allocated (scheduler is too slow),
-#      or may not be allocated *anymore* (some units finished, we wait for the
+#      or may not be allocated *anymore* (some tasks finished, we wait for the
 #      remaining ones).  We consider those core-hours as 'idle'.
 #
 #      Also, the agent itself utilizes one node, and we consider that time as
 #      agent utilization overhead.
 #
 # NOTE: we actually use core-seconds instead of core-hours.  So what?!
 #
@@ -88,163 +94,97 @@
         ['Unschedule',        ['unschedule']],
         ['Draining',          ['drain']],
         ['Idle',              ['idle' ]],
 ]
 
 metrics = metrics_default
 
+metrics = [
+    ['Bootstrap', ['boot', 'setup_1']                         , '#c6dbef'],
+    ['Warmup'   , ['warm' ]                                   , '#f0f0f0'],
+    ['Schedule' , ['exec_queue','exec_prep', 'unschedule']    , '#c994c7'],
+    ['Exec RP'  , ['exec_rp', 'exec_sh', 'term_sh', 'term_rp'], '#fdbb84'],
+    ['Exec Cmd' , ['exec_cmd']                                , '#e31a1c'],
+    ['Cooldown' , ['drain']                                   , '#addd8e']
+]
 
 # ------------------------------------------------------------------------------
 #
 if __name__ == '__main__':
 
-    sources = sys.argv[1:]
-    xkeys   = dict()  # x-axis labels
-    sids    = list()  # need to sort SIDs
-
-    exp = ra.Experiment(sources, stype='radical.pilot')
-
-    # get the numbers we actually want to plot
-    for session in exp.sessions:
-
-        sid = session.uid
-        n_units = len(session.get(etype='unit'))
-        p_size  = 0
-        for pilot in session.get(etype='pilot'):
-            p_size += pilot.description['cores']
-
-        xkeys[sid] = [n_units, p_size]
-        sids.append(sid)
-
-    # sort sessions by pilot size
-    sids = sorted(sids, key=lambda sid: xkeys[sid][1])
-
-
-    # get utilization information
-    provided, consumed, stats_abs, stats_rel, info = exp.utilization(metrics=metrics)
-  # provided, consumed, stats_abs, stats_rel = exp.utilization(metrics='/path/metrics.json')
-
-    with open('%s.stats' % sid, 'w') as fout:
-        fout.write('\n%s\n\n' % info)
-
-  # pprint.pprint(provided)
-  # pprint.pprint(consumed)
-  # pprint.pprint(stats_abs)
-  # pprint.pprint(stats_rel)
-
-    cmap = mpl.cm.get_cmap('tab20c')
-
-    # --------------------------------------------------------------------------
-    # core utilization over time (box plot)
-    for sid in sids:
-        fig  = plt.figure(figsize=(20,14))
-        ax   = fig.add_subplot(111)
-
-        step   = 1.0  / (len(metrics) + 1)
-        this   = step / 1.0
-        legend = list()
-
-        x_min = None
-        x_max = None
-        y_min = None
-        y_max = None
-
-        for metric in metrics:
-
-            color = cmap(this)
-            this += step
-
-            legend.append(mpl.lines.Line2D([0], [0], color=color, lw=6))
-
-            if isinstance(metric, list):
-                name  = metric[0]
-                parts = metric[1]
-            else:
-                name  = metric
-                parts = [metric]
-
-            for part in parts:
-                for uid in sorted(consumed[sid][part]):
-                    for block in consumed[sid][part][uid]:
-                        orig_x = block[0]
-                        orig_y = block[2] - 0.5
-                        width  = block[1] - block[0]
-                        height = block[3] - block[2] + 1.0
-
-                        if x_min is None: x_min = orig_x
-                        if x_max is None: x_max = orig_x + width
-                        if y_min is None: y_min = orig_x
-                        if y_max is None: y_max = orig_x + height
-
-                        x_min = min(x_min, orig_x)
-                        y_min = min(y_min, orig_y)
-                        x_max = max(x_max, orig_x + width)
-                        y_max = max(y_max, orig_y + height)
-
-                        patch = mpl.patches.Rectangle((orig_x, orig_y),
-                                                      width, height,
-                                                      facecolor=color,
-                                                      edgecolor='black',
-                                                      fill=True, lw=0.0)
-                        ax.add_patch(patch)
-
-        ax.legend(legend, [m[0] for m in metrics], ncol=6,
-                   loc='upper center', bbox_to_anchor=(0.5,1.11))
-        plt.xlabel('runtime [s]')
-        plt.ylabel('resource slot (index)')
-
-        plt.xlim([x_min, x_max])
-        plt.ylim([y_min, y_max])
-      # plt.xticks(list(range(int(x_min)-1, int(x_max)+1)))
-        fig.savefig('%s_core_allocation.png' % sid)
-        plt.show()
-
-
-    # --------------------------------------------------------------------------
-    # utilization: contributions as stacked barplot
-    #
-    # yes, stacked barplot is this cumbersome:
-    # http://matplotlib.org/examples/pylab_examples/bar_stacked.html
-    #
-    plt.figure(figsize=(20,14))
-    bottom = np.zeros(len(exp.sessions))
-    ind    = np.arange(len(exp.sessions))  # locations of bars on x-axis
-    width  = 0.35                          # width of bars
-
-    labels = list()
-    plots  = list()
-
-    for metric in metrics + ['Other']:
-
-        color = cmap(this)
-        this += step
-
-        legend.append(mpl.lines.Line2D([0], [0], color=color, lw=6))
-
-        if isinstance(metric, list):
-            name  = metric[0]
-            parts = metric[1]
-        else:
-            name  = metric
-            parts = [metric]
-
-        values = [stats_rel[sid][name] for sid in sids]
-        plots.append(plt.bar(ind, values, width, bottom=bottom))
-        bottom += values
-        labels.append(name)
-
-    if False: plt.ylabel('utilization (% of total resources)')
-    else    : plt.ylabel('utilization (in core-seconds)')
-
-    plt.xlabel('#CU / #cores')
-    plt.ylabel('utilization (% of total resources)')
-    plt.title ('pilot utilization over workload size (#units)')
-    plt.xticks(ind, ['%s / %s' % (xkeys[sid][0], xkeys[sid][1]) for sid in sids])
-
-    plt.legend([p[0] for p in plots], labels, ncol=5, loc='upper left',
-               bbox_to_anchor=(0,1.13))
-    plt.savefig('08c_core_utilization.png')
-    plt.show()
+    if len(sys.argv) < 2:
+        print("\n\tusage: %s <dir|tarball>\n" % sys.argv[0])
+        sys.exit(1)
+
+    src = sys.argv[1]
+
+    if len(sys.argv) == 3: stype = sys.argv[2]
+    else                 : stype = 'radical.pilot'
+
+    fig, axes = plt.subplots(2, figsize=ra.get_plotsize(500))
+    session   = ra.Session(src, stype=stype)
+
+    # this script only works for one pilot
+    pilots = session.get(etype='pilot')
+    assert(len(pilots) == 1), len(pilots)
+
+    sid     = session.uid
+    p_zero  = pilots[0].timestamps(event={ru.EVENT: 'bootstrap_0_start'})[0]
+    p_size  = pilots[0].description['cores']
+    n_nodes = int(p_size / pilots[0].cfg['cores_per_node'])
+    n_tasks = len(session.get(etype='task'))
+
+    legend = None
+    rtypes = ['cpu', 'gpu']
+    for i, rtype in enumerate(rtypes):
+
+        # get utilization information
+        prov, consumed, stats_abs, stats_rel, info = session.utilization(metrics, rtype)
+
+        with open('%s.stats' % sid, 'w') as fout:
+            fout.write('\n%s\n\n' % info)
+
+      # import pprint
+      # pprint.pprint(prov)
+      # pprint.pprint(consumed)
+      # pprint.pprint(stats_abs)
+      # pprint.pprint(stats_rel)
+
+        legend, patches, x, y = ra.get_plot_utilization(metrics,
+                {sid: consumed}, p_zero, sid, 'pilot.0000')
+
+        for patch in patches:
+            axes[i].add_patch(patch)
+
+        # Format axes
+        axes[i].set_xlim([x['min'], x['max']])
+        axes[i].set_ylim([y['min'], y['max']])
+
+        axes[i].yaxis.set_major_locator(plt.MaxNLocator(5))
+        axes[i].xaxis.set_major_locator(plt.MaxNLocator(5))
+
+        # Resource-type dependend labels
+        axes[i].set_ylabel(to_latex('%ss' % rtype.upper()))
+        axes[i].set_xlabel(to_latex('time (s)'))
+
+    # Do not repeat the X-axes label in the topmost plot
+    for ax in fig.get_axes():
+        ax.label_outer()
+
+    # Title of the plot. Facultative, requires info about session
+    # (see RA Info Chapter)
+    axes[0].set_title(to_latex('%s Tasks - %s Nodes' % (n_tasks, n_nodes)))
+
+    # Add legend for both plots
+    fig.legend([to_latex(l) for l in legend],
+               [m[0] for m in metrics], ncol=3,
+               loc='upper center', bbox_to_anchor=(0.5, 1.10))
+
+
+  # plt.xticks(list(range(int(x_min)-1, int(x_max)+1)))
+    fig.savefig('%s_util.png' % sid, bbox_inches="tight")
+  # plt.show()
 
 
 # ------------------------------------------------------------------------------
 
+
```

### Comparing `radical.analytics-1.5.0/examples/09_session_plots.py` & `radical.analytics-1.6.7/examples/09_session_plots.py`

 * *Files identical despite different names*

### Comparing `radical.analytics-1.5.0/examples/10_durations.py` & `radical.analytics-1.6.7/examples/10_durations.py`

 * *Files identical despite different names*

### Comparing `radical.analytics-1.5.0/setup.py` & `radical.analytics-1.6.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-#!/usr/bin/env python
+#!/usr/bin/env python3
 
-__author__    = 'RADICAL Team'
+__author__    = 'RADICAL Devel Team'
 __email__     = 'radical@rutgers.edu'
 __copyright__ = 'Copyright 2013-20, RADICAL Devel Team'
 __license__   = 'MIT'
 
 
 ''' Setup script, only usable via pip. '''
 
@@ -12,15 +12,16 @@
 import os
 import sys
 import glob
 import shutil
 
 import subprocess as sp
 
-from setuptools import setup, Command, find_packages
+
+from setuptools import setup, Command, find_namespace_packages
 
 
 # ------------------------------------------------------------------------------
 name     = 'radical.analytics'
 mod_root = 'src/radical/analytics/'
 
 
@@ -119,26 +120,26 @@
             # pip install stage 2 or easy_install stage 1
             #
             # pip install will untar the sdist in a tmp tree.  In that tmp
             # tree, we won't be able to derive git version tags -- so we pack
             # the formerly derived version as ./VERSION
             shutil.move("VERSION", "VERSION.bak")            # backup version
             shutil.copy("%s/VERSION" % path, "VERSION")      # use full version
-            os.system  ("python setup.py sdist")             # build sdist
+            os.system  ("python3 setup.py sdist")             # build sdist
             shutil.copy('dist/%s' % sdist_name,
                         '%s/%s'   % (mod_root, sdist_name))  # copy into tree
             shutil.move('VERSION.bak', 'VERSION')            # restore version
 
         with open(path + '/SDIST', 'w') as f:
             f.write(sdist_name + '\n')
 
         return version_base, version_detail, sdist_name
 
     except Exception as e:
-        raise RuntimeError('Could not extract/set version: %s' % e)
+        raise RuntimeError('Could not extract/set version: %s' % e) from e
 
 
 # ------------------------------------------------------------------------------
 # check python version. we need >= 3.6
 if sys.hexversion < 0x03060000:
     raise RuntimeError('%s requires Python 3.6 or higher' % name)
 
@@ -161,26 +162,27 @@
 # ------------------------------------------------------------------------------
 #
 class RunTwine(Command):
     user_options = []
     def initialize_options (self) : pass
     def finalize_options   (self) : pass
     def run (self) :
-        _,  _, ret = sh_callout('python setup.py sdist upload -r pypi')
+        _, _, ret = sh_callout('python3 setup.py sdist upload -r pypi')
         raise SystemExit(ret)
 
 
 # ------------------------------------------------------------------------------
 #
 # This copies the contents like examples/ dir under sys.prefix/share/$name
 # It needs the MANIFEST.in entries to work.
 share = 'share/%s' % name
 df    = [
-    ('%s/examples' % share, glob.glob('examples/[01]*.py')),
-    ('bin/rp_inspect/',     glob.glob('bin/rp_inspect/*')),
+    ('%s/styles/'   % share, glob.glob('styles/*.txt')),
+    ('%s/examples/' % share, glob.glob('examples/[01]*.py')),
+    ('bin/rp_inspect/',      glob.glob('bin/rp_inspect/*')),
 ]
 
 
 # ------------------------------------------------------------------------------
 #
 setup_args = {
     'name'               : name,
@@ -206,39 +208,40 @@
         'Programming Language :: Python :: 3.6',
         'Topic :: Utilities',
         'Topic :: System :: Distributed Computing',
         'Topic :: Scientific/Engineering',
         'Operating System :: POSIX',
         'Operating System :: Unix'
     ],
-    'packages'           : find_packages('src'),
+    'packages'           : find_namespace_packages('src', include=['radical.*']),
     'package_dir'        : {'': 'src'},
     'scripts'            : [
                             'bin/radical-analytics-check',
                             'bin/radical-analytics-inspect',
                             'bin/radical-analytics-plot.py',
                             'bin/radical-analytics-version',
                             'bin/radical-analytics-wrangler.py',
                            ],
     'package_data'       : {'': ['*.txt', '*.sh', '*.json', '*.gz', '*.c',
                                  '*.md', 'VERSION', 'SDIST', sdist_name]},
   # 'setup_requires'     : ['pytest-runner'],
-    'install_requires'   : ['radical.utils>=1.4',
+    'install_requires'   : ['radical.utils>=1.6',
                             'matplotlib>=3.1.2',
                             'psutil',
                             'pandas',
                             'numpy',
                             'sqlalchemy',
                             'more_itertools',
                             ],
     'tests_require'      : ['pytest',
                             'pylint',
                             'flake8',
                             'coverage',
                             'mock==2.0.0.',
+                            'radical.pilo >= 1.6.7',
                            ],
     'test_suite'         : '%s.tests' % name,
     'zip_safe'           : False,
   # 'build_sphinx'       : {
   #     'source-dir'     : 'docs/',
   #     'build-dir'      : 'docs/build',
   #     'all_files'      : 1,
```

### Comparing `radical.analytics-1.5.0/src/radical/analytics/__init__.py` & `radical.analytics-1.6.7/src/radical/analytics/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,22 +8,36 @@
 from .experiment import Experiment
 from .session    import Session
 from .entity     import Entity
 from .plotter    import Plotter
 
 # ------------------------------------------------------------------------------
 #
+from .utils import get_plotsize, get_mplstyle, stack_transitions
+from .utils import get_pilot_series, get_plot_utilization, get_pilots_zeros
+from .utils import to_latex
+
+
+# ------------------------------------------------------------------------------
+#
 import os
 import radical.utils as ru
 
 pwd  = os.path.dirname (__file__)
 root = "%s" % pwd
 version_short, version_detail, version_base, \
         version_branch, sdist_name, sdist_path = ru.get_version(paths=[root])
 version = version_short
 
 logger = ru.Logger('radical.analytics')
 logger.info('radical.analytics    version: %s' % version_detail)
 
+
+# ------------------------------------------------------------------------------
+#
+__all__ = ('Experiment','Session','Entity','Plotter', 'get_plotsize',
+           'get_mplstyle', 'stack_transitions', 'get_pilot_series',
+           'get_plot_utilization', 'get_pilots_zeros', 'to_latex')
+
+
 # ------------------------------------------------------------------------------
 
-__all__ = ('Experiment','Session','Entity','Plotter',)
```

### Comparing `radical.analytics-1.5.0/src/radical/analytics/entity.py` & `radical.analytics-1.6.7/src/radical/analytics/entity.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
         assert(_profile)
 
         self._uid         = _uid
         self._etype       = _etype
         self._details     = _details
         self._description = self._details.get('description', dict())
         self._cfg         = self._details.get('cfg',         dict())
+        self._resources   = self._details.get('resources',   dict())
 
         # FIXME: this should be sorted out on RP level
         self._cfg['hostid'] = self._details['hostid']
 
         self._states      = dict()
         self._events      = list()
         self._consistency = {'log'         : list(),
@@ -52,14 +53,15 @@
     def __getstate__(self):
 
         state = {
                  'uid'         : self._uid,
                  'etype'       : self._etype,
                  'details'     : self._details,
                  'description' : self._description,
+                 'resources'   : self._resources,
                  'cfg'         : self._cfg,
 
                  'states'      : self._states,
                  'events'      : self._events,
                  'consistency' : self._consistency,
 
                  't_start'     : self._t_start,
@@ -74,14 +76,15 @@
     #
     def __setstate__(self, state):
 
         self._uid          = state['uid']
         self._etype        = state['etype']
         self._details      = state['details']
         self._description  = state['description']
+        self._resources    = state['resources']
         self._cfg          = state['cfg']
 
         self._states       = state['states']
         self._events       = state['events']
         self._consistency  = state['consistency']
 
         self._t_start      = state['t_start']
@@ -120,14 +123,18 @@
         return self._states
 
     @property
     def description(self):
         return self._description
 
     @property
+    def resources(self):
+        return self._resources
+
+    @property
     def cfg(self):
         return self._cfg
 
     @property
     def events(self):
         return self._events
 
@@ -219,14 +226,15 @@
 
         return {
                 'uid'        : self._uid,
                 'etype'      : self._etype,
                 'states'     : self._states,
                 'events'     : self._events,
                 'cfg'        : self._cfg,
+                'resources'  : self._resources,
                 'description': self._description,
                }
 
 
     # --------------------------------------------------------------------------
     #
     def dump(self):
@@ -322,15 +330,15 @@
         return sorted(ret)
 
 
     # --------------------------------------------------------------------------
     #
     def _match_event(self, needle, hay):
 
-        for key in range(ru.PROF_KEY_MAX - 2):
+        for key in range(ru.PROF_KEY_MAX - 1):
             if needle[key] is not None:
                 if key == ru.MSG:
                     if needle[key] not in hay[key]:
                         return False
                 else:
                     if needle[key] != hay[key]:
                         return False
```

### Comparing `radical.analytics-1.5.0/src/radical/analytics/experiment.py` & `radical.analytics-1.6.7/src/radical/analytics/experiment.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,17 +41,17 @@
     @property
     def sids(self):
         return [s.sid for s in self._sessions]
 
 
     # --------------------------------------------------------------------------
     #
-    def utilization(self, metrics):
+    def utilization(self, metrics, rtype='cpu', udurations=None):
         '''
-        return five dictionaries: 
+        return five dictionaries:
           - provided resources
           - consumed resources
           - absolute stats
           - relative stats
           - information about resource utilization
 
         The resource dictionaries have the following structures::
@@ -106,15 +106,15 @@
         stats_rel = dict()
         info      = dict()
 
         # obtain resources provisions and consumptions for all sessions
         for session in self._sessions:
 
             sid = session.uid
-            p, c, sa, sr, i = session.utilization(metrics)
+            p, c, sa, sr, i = session.utilization(metrics, rtype, udurations)
 
             provided [sid] = p
             consumed [sid] = c
             stats_abs[sid] = sa
             stats_rel[sid] = sr
             info     [sid] = i
```

### Comparing `radical.analytics-1.5.0/src/radical/analytics/plotter.py` & `radical.analytics-1.6.7/src/radical/analytics/plotter.py`

 * *Files identical despite different names*

### Comparing `radical.analytics-1.5.0/src/radical/analytics/session.py` & `radical.analytics-1.6.7/src/radical/analytics/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,16 @@
                 elif ext in ['tgz, tar.gz']:
                     tf = tarfile.open(name=src, mode='r:gz')
                     tf.extractall(path=os.path.dirname(tgt))
                 else:
                     raise ValueError('cannot handle extension %s' % ext)
 
             except Exception as e:
-                raise RuntimeError('Cannot extract tarball: %s' % repr(e))
+                raise RuntimeError(
+                    'Cannot extract tarball: %s' % repr(e)) from e
 
         self._sid   = sid
         self._src   = src
         self._stype = stype
 
       # print 'sid: %s [%s]' % (sid, stype)
       # print 'src: %s'      % src
@@ -94,35 +95,35 @@
                                        'hostmap'  : dict(),
                                        'accuracy' : 0.0}
 
         elif stype == 'radical.pilot':
 
             try:
                 import radical.pilot.utils as rpu
-            except:
+            except Exception as e:
                 raise RuntimeError('radical.analytics requires the '
                                    'radical.pilot module to analyze this '
-                                   'session - please install it.')
+                                   'session - please install it.') from e
 
             self._profile, accuracy, hostmap \
                               = rpu.get_session_profile    (sid=sid, src=self._src)
             self._description = rpu.get_session_description(sid=sid, src=self._src)
 
             self._description['accuracy'] = accuracy
             self._description['hostmap']  = hostmap
 
 
         elif stype == 'radical.entk':
 
             try:
                 import radical.entk.utils as reu
-            except:
+            except Exception as e:
                 raise RuntimeError('radical.analytics requires the '
                                    'radical.entk module to analyze this '
-                                   'session - please install it.')
+                                   'session - please install it.') from e
 
             self._profile, accuracy, hostmap \
                               = reu.get_session_profile    (sid=sid, src=self._src)
             self._description = reu.get_session_description(sid=sid, src=self._src)
 
             self._description['accuracy'] = accuracy
             self._description['hostmap']  = hostmap
@@ -407,15 +408,15 @@
               }
             }
 
         We count how often any property value appears in the current set of
         entities.
 
         RA knows exactly 4 properties:
-          - uid   (entity idetifiers)
+          - uid   (entity identifiers)
           - etype (type of entities)
           - event (names of events)
           - state (state identifiers)
         '''
 
         # FIXME: initializing properties can be expensive, and we might not
         #        always need them anyway.  So we can lazily defer this
@@ -851,15 +852,15 @@
         else:
             # select data points according to sampling
             # get min time, and create timestamps at regular intervals
             t     = times[0][0]
             ret   = list()
             for time, val in collapsed:
                 while time >= t:
-                    ret.append(t, val)
+                    ret.append([t, val])
                     t += sampling
 
             # append last time stamp if it is not appended, yet
             if ret[-1] != [t, val]:
                 ret.append([t, val])
 
         return ret
@@ -869,21 +870,21 @@
     #
     def rate(self, state=None, event=None, time=None, sampling=None,
             first=False):
         '''
         This method accepts the same parameters as the `timestamps()` method: it
         will count all matching events and state transitions as given, and will
         return a time series of the rate of how many of those events and/or
-        transitions occured per second.
+        transitions occurred per second.
 
         The additional parameter `sampling` determines the exact points in time
         for which the rate is computed, and thus determines the sampling rate
         for the returned time series.  If not specified, the time series will
-        contain all points at which and event occured, and the rate value will
-        only be determined by the time passed between two consequtuve events.
+        contain all points at which and event occurred, and the rate value will
+        only be determined by the time passed between two consecutive events.
         If specified, it is interpreted as second (float) interval at which,
         after the starting point (begin of first event matching the filters) the
         rate is computed.
 
         Returned is an ordered list of tuples::
 
           [ [time_0, rate_0] ,
@@ -975,24 +976,24 @@
             ret.append([t_stop, cnt / (t_stop - t_start)])
 
         return ret
 
 
     # --------------------------------------------------------------------------
     #
-    def utilization(self, metrics):
+    def utilization(self, metrics, rtype='cpu', udurations=None):
 
         if self._stype != 'radical.pilot':
             raise ValueError('session utilization is only available on '
                              'radical.pilot sessions')
 
         import radical.pilot as rp
 
-        provided  = rp.utils.get_provided_resources(self)
-        consumed  = rp.utils.get_consumed_resources(self)
+        provided  = rp.utils.get_provided_resources(self, rtype)
+        consumed  = rp.utils.get_consumed_resources(self, rtype, udurations)
         stats_abs = {'total':   0.0}
         stats_rel = {'total': 100.0}
         total     = 0.0
 
         for pid in provided['total']:
             for box in provided['total'][pid]:
                 stats_abs['total'] += (box[1] - box[0]) * \
```

### Comparing `radical.analytics-1.5.0/src/radical.analytics.egg-info/PKG-INFO` & `radical.analytics-1.6.7/src/radical.analytics.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: radical.analytics
-Version: 1.5.0
+Version: 1.6.7
 Summary: The RADICAL analytics framework
 Home-page: https://www.github.com/radical-cybertools/radical.analytics/
 Author: RADICAL Group at Rutgers University
 Author-email: radical@rutgers.edu
 Maintainer: The RADICAL Devel Team
 Maintainer-email: radical@rutgers.edu
 License: MIT
```

### Comparing `radical.analytics-1.5.0/src/radical.analytics.egg-info/SOURCES.txt` & `radical.analytics-1.6.7/src/radical.analytics.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -10,44 +10,45 @@
 bin/radical-analytics-version
 bin/radical-analytics-wrangler.py
 bin/rp_inspect/plot_conc.py
 bin/rp_inspect/plot_dur.py
 bin/rp_inspect/plot_rate.py
 bin/rp_inspect/plot_state.py
 bin/rp_inspect/plot_util.py
+bin/rp_inspect/plot_util_2.py
 examples/00_session_describe_rp.py
 examples/01_session_list_rp.py
 examples/02_session_get_rp.py
 examples/03_session_filter_rp.py
 examples/04_session_duration_rp.py
 examples/05_relationsships.py
 examples/06_events.py
 examples/06_ra_events.py
 examples/07_event_timeline.py
 examples/08_core_utilization_plot.py
 examples/08c_core_utilization_plot.py
 examples/09_session_plots.py
 examples/10_durations.py
-src/radical/__init__.py
 src/radical.analytics.egg-info/PKG-INFO
 src/radical.analytics.egg-info/SOURCES.txt
 src/radical.analytics.egg-info/dependency_links.txt
 src/radical.analytics.egg-info/namespace_packages.txt
 src/radical.analytics.egg-info/not-zip-safe
 src/radical.analytics.egg-info/requires.txt
 src/radical.analytics.egg-info/top_level.txt
 src/radical/analytics/SDIST
 src/radical/analytics/VERSION
 src/radical/analytics/__init__.py
 src/radical/analytics/entity.py
 src/radical/analytics/experiment.py
 src/radical/analytics/plotter.py
-src/radical/analytics/radical.analytics-0.90.7-v0.72.0-42-gcab8498-feature-unittests.tar.gz
-src/radical/analytics/radical.analytics-0.90.7-v0.72.0-44-ge31c6b0-fix-plot-origin.tar.gz
 src/radical/analytics/session.py
+src/radical/analytics/utils/__init__.py
+src/radical/analytics/utils/plot.py
+styles/radical_mpl.txt
 tests/__init__.py
 tests/test_duration_method.py
 tests/test_entity.py
 tests/test_session.py
 tests/barrier_data/rp.session.two.jdakka.017395.0000.json
 tests/barrier_data/rp.session.two.jdakka.017395.0000/pmgr.0000.prof
 tests/barrier_data/rp.session.two.jdakka.017395.0000/pmgr.launching.0.child.prof
```

### Comparing `radical.analytics-1.5.0/tests/barrier_data/rp.session.two.jdakka.017395.0000/pmgr.0000.prof` & `radical.analytics-1.6.7/tests/barrier_data/rp.session.two.jdakka.017395.0000/pmgr.0000.prof`

 * *Files identical despite different names*

### Comparing `radical.analytics-1.5.0/tests/barrier_data/rp.session.two.jdakka.017395.0000/rp.session.two.jdakka.017395.0000.prof` & `radical.analytics-1.6.7/tests/barrier_data/rp.session.two.jdakka.017395.0000/rp.session.two.jdakka.017395.0000.prof`

 * *Files identical despite different names*

### Comparing `radical.analytics-1.5.0/tests/barrier_data/rp.session.two.jdakka.017395.0000/umgr.0000.prof` & `radical.analytics-1.6.7/tests/barrier_data/rp.session.two.jdakka.017395.0000/umgr.0000.prof`

 * *Files identical despite different names*

### Comparing `radical.analytics-1.5.0/tests/barrier_data/rp.session.two.jdakka.017395.0000/umgr.scheduling.0.child.prof` & `radical.analytics-1.6.7/tests/barrier_data/rp.session.two.jdakka.017395.0000/umgr.scheduling.0.child.prof`

 * *Files identical despite different names*

### Comparing `radical.analytics-1.5.0/tests/barrier_data/rp.session.two.jdakka.017395.0000/umgr.staging.input.0.child.prof` & `radical.analytics-1.6.7/tests/barrier_data/rp.session.two.jdakka.017395.0000/umgr.staging.input.0.child.prof`

 * *Files identical despite different names*

### Comparing `radical.analytics-1.5.0/tests/barrier_data/rp.session.two.jdakka.017395.0000/umgr.staging.output.0.child.prof` & `radical.analytics-1.6.7/tests/barrier_data/rp.session.two.jdakka.017395.0000/umgr.staging.output.0.child.prof`

 * *Files identical despite different names*

### Comparing `radical.analytics-1.5.0/tests/barrier_data/rp.session.two.jdakka.017395.0000/update.0.child.prof` & `radical.analytics-1.6.7/tests/barrier_data/rp.session.two.jdakka.017395.0000/update.0.child.prof`

 * *Files identical despite different names*

### Comparing `radical.analytics-1.5.0/tests/barrier_data/rp.session.two.jdakka.017395.0000.json` & `radical.analytics-1.6.7/tests/barrier_data/rp.session.two.jdakka.017395.0000.json`

 * *Files identical despite different names*

### Comparing `radical.analytics-1.5.0/tests/example-data/pilot-entity-example.json` & `radical.analytics-1.6.7/tests/example-data/pilot-entity-example.json`

 * *Files identical despite different names*

### Comparing `radical.analytics-1.5.0/tests/example-data/pmgr-entity-example.json` & `radical.analytics-1.6.7/tests/example-data/pmgr-entity-example.json`

 * *Files identical despite different names*

### Comparing `radical.analytics-1.5.0/tests/example-data/range-testing-entity-example.json` & `radical.analytics-1.6.7/tests/example-data/range-testing-entity-example.json`

 * *Files identical despite different names*

### Comparing `radical.analytics-1.5.0/tests/example-data/rp-entity-example.json` & `radical.analytics-1.6.7/tests/example-data/rp-entity-example.json`

 * *Files identical despite different names*

### Comparing `radical.analytics-1.5.0/tests/example-data/umgr-entity-example.json` & `radical.analytics-1.6.7/tests/example-data/umgr-entity-example.json`

 * *Files identical despite different names*

### Comparing `radical.analytics-1.5.0/tests/example-data/unit-entity-example.json` & `radical.analytics-1.6.7/tests/example-data/unit-entity-example.json`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,138 @@
 {
-  "uid": "unit.000001",
-  "etype": "unit",
-  "events": [[5.005199909210205,"state","umgr.0000","MainThread","unit.000001","NEW","","unit"],[5.005199909210205,"state","umgr.0000","MainThread","unit.000001","NEW","","unit"],[5.157599925994873,"state","umgr.0000","MainThread","unit.000001","UMGR_SCHEDULING_PENDING","","unit"],[5.157599925994873,"state","umgr.0000","MainThread","unit.000001","UMGR_SCHEDULING_PENDING","","unit"],[5.159499883651733,"update_request","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","UMGR_SCHEDULING_PENDING","unit"],[5.162600040435791,"put","umgr.0000","MainThread","unit.000001","UMGR_SCHEDULING_PENDING","umgr.scheduling.queue.input.0000","unit"],[5.1677000522613525,"get","umgr.scheduling.0.child","MainThread","unit.000001","UMGR_SCHEDULING_PENDING","","unit"],[5.184700012207031,"state","umgr.scheduling.0.child","MainThread","unit.000001","UMGR_SCHEDULING","","unit"],[5.184700012207031,"state","umgr.scheduling.0.child","MainThread","unit.000001","UMGR_SCHEDULING","","unit"],[5.199300050735474,"state","umgr.scheduling.0.child","MainThread","unit.000001","UMGR_STAGING_INPUT_PENDING","","unit"],[5.199300050735474,"state","umgr.scheduling.0.child","MainThread","unit.000001","UMGR_STAGING_INPUT_PENDING","","unit"],[5.2037999629974365,"put","umgr.scheduling.0.child","MainThread","unit.000001","UMGR_STAGING_INPUT_PENDING","umgr.staging.input.queue.input.0000","unit"],[5.211299896240234,"get","umgr.staging.input.0.child","MainThread","unit.000001","UMGR_STAGING_INPUT_PENDING","","unit"],[5.227599859237671,"state","umgr.staging.input.0.child","MainThread","unit.000001","UMGR_STAGING_INPUT","","unit"],[5.227599859237671,"state","umgr.staging.input.0.child","MainThread","unit.000001","UMGR_STAGING_INPUT","","unit"],[5.230299949645996,"state","umgr.staging.input.0.child","MainThread","unit.000001","AGENT_STAGING_INPUT_PENDING","","unit"],[5.230299949645996,"state","umgr.staging.input.0.child","MainThread","unit.000001","AGENT_STAGING_INPUT_PENDING","","unit"],[5.236299991607666,"update_pushed","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","UMGR_SCHEDULING_PENDING","unit"],[5.237499952316284,"update_request","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","UMGR_SCHEDULING","unit"],[5.286499977111816,"update_pushed","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","UMGR_SCHEDULING","unit"],[5.287699937820435,"update_request","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","UMGR_STAGING_INPUT_PENDING","unit"],[5.327600002288818,"update_pushed","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","UMGR_STAGING_INPUT_PENDING","unit"],[5.3282999992370605,"update_request","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","UMGR_STAGING_INPUT","unit"],[5.365200042724609,"update_pushed","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","UMGR_STAGING_INPUT","unit"],[5.366699934005737,"update_request","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","AGENT_STAGING_INPUT_PENDING","unit"],[5.44539999961853,"update_pushed","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","AGENT_STAGING_INPUT_PENDING","unit"],[29.84999990463257,"get","agent_0","agent_0.idler._check_units_cb","unit.000001","","","unit"],[29.856899976730347,"put","agent_0","agent_0.idler._check_units_cb","unit.000001","AGENT_STAGING_INPUT_PENDING","agent.staging.input.queue.input.0000","unit"],[29.860699892044067,"get","agent.staging.input.0.child","MainThread","unit.000001","AGENT_STAGING_INPUT_PENDING","","unit"],[29.87150001525879,"state","agent.staging.input.0.child","MainThread","unit.000001","AGENT_STAGING_INPUT","","unit"],[29.87150001525879,"state","agent.staging.input.0.child","MainThread","unit.000001","AGENT_STAGING_INPUT","","unit"],[29.873199939727783,"update_request","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","AGENT_STAGING_INPUT","unit"],[29.873199939727783,"state","agent.staging.input.0.child","MainThread","unit.000001","AGENT_SCHEDULING_PENDING","","unit"],[29.873199939727783,"state","agent.staging.input.0.child","MainThread","unit.000001","AGENT_SCHEDULING_PENDING","","unit"],[29.875399827957153,"put","agent.staging.input.0.child","MainThread","unit.000001","AGENT_SCHEDULING_PENDING","agent.scheduling.queue.input.0000","unit"],[29.879299879074097,"get","agent.scheduling.0.child","MainThread","unit.000001","AGENT_SCHEDULING_PENDING","","unit"],[29.891299962997437,"state","agent.scheduling.0.child","MainThread","unit.000001","AGENT_SCHEDULING","","unit"],[29.891299962997437,"state","agent.scheduling.0.child","MainThread","unit.000001","AGENT_SCHEDULING","","unit"],[29.894700050354004,"schedule_try","agent.scheduling.0.child","MainThread","unit.000001","","","unit"],[29.894799947738647,"schedule_ok","agent.scheduling.0.child","MainThread","unit.000001","","","unit"],[29.895999908447266,"state","agent.scheduling.0.child","MainThread","unit.000001","AGENT_EXECUTING_PENDING","","unit"],[29.895999908447266,"state","agent.scheduling.0.child","MainThread","unit.000001","AGENT_EXECUTING_PENDING","","unit"],[29.896600008010864,"put","agent.scheduling.0.child","MainThread","unit.000001","AGENT_EXECUTING_PENDING","agent.executing.queue.input.0000","unit"],[29.906100034713745,"get","agent.executing.0.child","MainThread","unit.000001","AGENT_EXECUTING_PENDING","","unit"],[29.9064998626709,"state","agent.executing.0.child","MainThread","unit.000001","AGENT_EXECUTING","","unit"],[29.9064998626709,"state","agent.executing.0.child","MainThread","unit.000001","AGENT_EXECUTING","","unit"],[29.906999826431274,"exec","agent.executing.0.child","MainThread","unit.000001","","unit launch","unit"],[29.90779995918274,"exec_start","agent.executing.0.child","MainThread","unit.000001","","","unit"],[29.916599988937378,"exec_ok","agent.executing.0.child","MainThread","unit.000001","","","unit"],[29.93969988822937,"update_pushed","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","AGENT_STAGING_INPUT","unit"],[29.94089984893799,"update_request","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","AGENT_SCHEDULING_PENDING","unit"],[29.991999864578247,"update_pushed","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","AGENT_SCHEDULING_PENDING","unit"],[29.993199825286865,"update_request","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","AGENT_SCHEDULING","unit"],[30.035599946975708,"update_pushed","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","AGENT_SCHEDULING","unit"],[30.037699937820435,"update_request","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","AGENT_EXECUTING_PENDING","unit"],[30.038899898529053,"update_request","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","AGENT_EXECUTING","unit"],[30.602999925613403,"update_request","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","AGENT_STAGING_INPUT","unit"],[30.603099822998047,"update_request","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","AGENT_SCHEDULING_PENDING","unit"],[30.603099822998047,"update_request","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","AGENT_SCHEDULING","unit"],[31.685499906539917,"update_pushed","update.0.child","update.0.child.idler._idle_cb","unit.000001","","AGENT_EXECUTING_PENDING","unit"],[31.685499906539917,"update_pushed","update.0.child","update.0.child.idler._idle_cb","unit.000001","","AGENT_EXECUTING","unit"],[32.28670001029968,"update_pushed","update.0.child","update.0.child.idler._idle_cb","unit.000001","","AGENT_STAGING_INPUT","unit"],[32.28670001029968,"update_pushed","update.0.child","update.0.child.idler._idle_cb","unit.000001","","AGENT_SCHEDULING_PENDING","unit"],[32.28670001029968,"update_pushed","update.0.child","update.0.child.idler._idle_cb","unit.000001","","AGENT_SCHEDULING","unit"],[32.74600005149841,"exec_stop","agent.executing.0.child","Watcher","unit.000001","","","unit"],[32.746399879455566,"state","agent.executing.0.child","Watcher","unit.000001","AGENT_STAGING_OUTPUT_PENDING","","unit"],[32.746399879455566,"state","agent.executing.0.child","Watcher","unit.000001","AGENT_STAGING_OUTPUT_PENDING","","unit"],[32.74689984321594,"put","agent.executing.0.child","Watcher","unit.000001","AGENT_STAGING_OUTPUT_PENDING","agent.staging.output.queue.input.0000","unit"],[32.752699851989746,"update_request","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","AGENT_STAGING_OUTPUT_PENDING","unit"],[32.7574999332428,"unschedule_start","agent.scheduling.0.child","agent.scheduling.0.child.subscriber.unschedule_cb","unit.000001","","","unit"],[32.75789999961853,"unschedule_stop","agent.scheduling.0.child","agent.scheduling.0.child.subscriber.unschedule_cb","unit.000001","","","unit"],[32.77279996871948,"get","agent.staging.output.0.child","MainThread","unit.000001","AGENT_STAGING_OUTPUT_PENDING","","unit"],[32.77309989929199,"state","agent.staging.output.0.child","MainThread","unit.000001","AGENT_STAGING_OUTPUT","","unit"],[32.77309989929199,"state","agent.staging.output.0.child","MainThread","unit.000001","AGENT_STAGING_OUTPUT","","unit"],[32.7733998298645,"staging_stdout_start","agent.staging.output.0.child","MainThread","unit.000001","","","unit"],[32.7733998298645,"staging_stdout_stop","agent.staging.output.0.child","MainThread","unit.000001","","","unit"],[32.7733998298645,"staging_stderr_start","agent.staging.output.0.child","MainThread","unit.000001","","","unit"],[32.773499965667725,"staging_stderr_stop","agent.staging.output.0.child","MainThread","unit.000001","","","unit"],[32.773499965667725,"staging_uprof_start","agent.staging.output.0.child","MainThread","unit.000001","","","unit"],[32.773499965667725,"staging_uprof_stop","agent.staging.output.0.child","MainThread","unit.000001","","","unit"],[32.773499965667725,"state","agent.staging.output.0.child","MainThread","unit.000001","UMGR_STAGING_OUTPUT_PENDING","","unit"],[32.773499965667725,"state","agent.staging.output.0.child","MainThread","unit.000001","UMGR_STAGING_OUTPUT_PENDING","","unit"],[32.77439999580383,"update_request","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","AGENT_STAGING_OUTPUT","unit"],[32.77449989318848,"update_request","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","UMGR_STAGING_OUTPUT_PENDING","unit"],[32.84150004386902,"update_pushed","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","AGENT_STAGING_OUTPUT_PENDING","unit"],[32.841699838638306,"update_pushed","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","AGENT_STAGING_OUTPUT","unit"],[32.841699838638306,"update_pushed","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","UMGR_STAGING_OUTPUT_PENDING","unit"],[32.85109996795654,"update_request","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","AGENT_EXECUTING_PENDING","unit"],[32.85119986534119,"update_request","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","AGENT_EXECUTING","unit"],[32.89369988441467,"get","umgr.0000","umgr.0000.idler._unit_pull_cb","unit.000001","","","unit"],[32.8957998752594,"update_request","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","UMGR_STAGING_OUTPUT_PENDING","unit"],[32.89750003814697,"put","umgr.0000","umgr.0000.idler._unit_pull_cb","unit.000001","UMGR_STAGING_OUTPUT_PENDING","umgr.staging.output.queue.input.0000","unit"],[32.901700019836426,"get","umgr.staging.output.0.child","MainThread","unit.000001","UMGR_STAGING_OUTPUT_PENDING","","unit"],[32.90590000152588,"state","umgr.staging.output.0.child","MainThread","unit.000001","UMGR_STAGING_OUTPUT","","unit"],[32.90590000152588,"state","umgr.staging.output.0.child","MainThread","unit.000001","UMGR_STAGING_OUTPUT","","unit"],[32.906699895858765,"state","umgr.staging.output.0.child","MainThread","unit.000001","DONE","","unit"],[32.906699895858765,"state","umgr.staging.output.0.child","MainThread","unit.000001","DONE","","unit"],[32.90779995918274,"update_request","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","UMGR_STAGING_OUTPUT","unit"],[32.94509983062744,"update_pushed","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","AGENT_EXECUTING_PENDING","unit"],[32.94509983062744,"update_pushed","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","AGENT_EXECUTING","unit"],[32.94509983062744,"update_pushed","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","UMGR_STAGING_OUTPUT_PENDING","unit"],[32.94529986381531,"update_pushed","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","UMGR_STAGING_OUTPUT","unit"],[32.94609999656677,"update_request","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","DONE","unit"],[33.98679995536804,"update_pushed","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","DONE","unit"]],
+  "uid"    : "unit.000001",
+  "etype"  : "unit",
+  "events" : [
+      [ 5.005199909210205,"state","umgr.0000","MainThread","unit.000001","NEW","","unit"],
+      [ 5.157599925994873,"state","umgr.0000","MainThread","unit.000001","UMGR_SCHEDULING_PENDING","","unit"],
+      [ 5.159499883651733,"update_request","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","UMGR_SCHEDULING_PENDING","unit"],
+      [ 5.162600040435791,"put","umgr.0000","MainThread","unit.000001","UMGR_SCHEDULING_PENDING","umgr.scheduling.queue.input.0000","unit"],
+      [ 5.167700052261352,"get","umgr.scheduling.0.child","MainThread","unit.000001","UMGR_SCHEDULING_PENDING","","unit"],
+      [ 5.184700012207031,"state","umgr.scheduling.0.child","MainThread","unit.000001","UMGR_SCHEDULING","","unit"],
+      [ 5.199300050735474,"state","umgr.scheduling.0.child","MainThread","unit.000001","UMGR_STAGING_INPUT_PENDING","","unit"],
+      [ 5.203799962997436,"put","umgr.scheduling.0.child","MainThread","unit.000001","UMGR_STAGING_INPUT_PENDING","umgr.staging.input.queue.input.0000","unit"],
+      [ 5.211299896240234,"get","umgr.staging.input.0.child","MainThread","unit.000001","UMGR_STAGING_INPUT_PENDING","","unit"],
+      [ 5.227599859237671,"state","umgr.staging.input.0.child","MainThread","unit.000001","UMGR_STAGING_INPUT","","unit"],
+      [ 5.230299949645996,"state","umgr.staging.input.0.child","MainThread","unit.000001","AGENT_STAGING_INPUT_PENDING","","unit"],
+      [ 5.236299991607666,"update_pushed","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","UMGR_SCHEDULING_PENDING","unit"],
+      [ 5.237499952316284,"update_request","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","UMGR_SCHEDULING","unit"],
+      [ 5.286499977111816,"update_pushed","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","UMGR_SCHEDULING","unit"],
+      [ 5.287699937820435,"update_request","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","UMGR_STAGING_INPUT_PENDING","unit"],
+      [ 5.327600002288818,"update_pushed","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","UMGR_STAGING_INPUT_PENDING","unit"],
+      [ 5.328299999237060,"update_request","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","UMGR_STAGING_INPUT","unit"],
+      [ 5.365200042724609,"update_pushed","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","UMGR_STAGING_INPUT","unit"],
+      [ 5.366699934005737,"update_request","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","AGENT_STAGING_INPUT_PENDING","unit"],
+      [ 5.445399999618530,"update_pushed","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","AGENT_STAGING_INPUT_PENDING","unit"],
+      [29.849999904632570,"get","agent_0","agent_0.idler._check_units_cb","unit.000001","","","unit"],
+      [29.856899976730347,"put","agent_0","agent_0.idler._check_units_cb","unit.000001","AGENT_STAGING_INPUT_PENDING","agent.staging.input.queue.input.0000","unit"],
+      [29.860699892044067,"get","agent.staging.input.0.child","MainThread","unit.000001","AGENT_STAGING_INPUT_PENDING","","unit"],
+      [29.871500015258790,"state","agent.staging.input.0.child","MainThread","unit.000001","AGENT_STAGING_INPUT","","unit"],
+      [29.873199939727783,"update_request","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","AGENT_STAGING_INPUT","unit"],
+      [29.873199939727783,"state","agent.staging.input.0.child","MainThread","unit.000001","AGENT_SCHEDULING_PENDING","","unit"],
+      [29.875399827957153,"put","agent.staging.input.0.child","MainThread","unit.000001","AGENT_SCHEDULING_PENDING","agent.scheduling.queue.input.0000","unit"],
+      [29.879299879074097,"get","agent.scheduling.0.child","MainThread","unit.000001","AGENT_SCHEDULING_PENDING","","unit"],
+      [29.891299962997437,"state","agent.scheduling.0.child","MainThread","unit.000001","AGENT_SCHEDULING","","unit"],
+      [29.894700050354004,"schedule_try","agent.scheduling.0.child","MainThread","unit.000001","","","unit"],
+      [29.894799947738647,"schedule_ok","agent.scheduling.0.child","MainThread","unit.000001","","","unit"],
+      [29.895999908447266,"state","agent.scheduling.0.child","MainThread","unit.000001","AGENT_EXECUTING_PENDING","","unit"],
+      [29.896600008010864,"put","agent.scheduling.0.child","MainThread","unit.000001","AGENT_EXECUTING_PENDING","agent.executing.queue.input.0000","unit"],
+      [29.906100034713745,"get","agent.executing.0.child","MainThread","unit.000001","AGENT_EXECUTING_PENDING","","unit"],
+      [29.906499862670900,"state","agent.executing.0.child","MainThread","unit.000001","AGENT_EXECUTING","","unit"],
+      [29.906999826431274,"exec","agent.executing.0.child","MainThread","unit.000001","","unit launch","unit"],
+      [29.907799959182740,"exec_start","agent.executing.0.child","MainThread","unit.000001","","","unit"],
+      [29.916599988937378,"exec_ok","agent.executing.0.child","MainThread","unit.000001","","","unit"],
+      [29.939699888229370,"update_pushed","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","AGENT_STAGING_INPUT","unit"],
+      [29.940899848937990,"update_request","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","AGENT_SCHEDULING_PENDING","unit"],
+      [29.991999864578247,"update_pushed","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","AGENT_SCHEDULING_PENDING","unit"],
+      [29.993199825286865,"update_request","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","AGENT_SCHEDULING","unit"],
+      [30.035599946975708,"update_pushed","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","AGENT_SCHEDULING","unit"],
+      [30.037699937820435,"update_request","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","AGENT_EXECUTING_PENDING","unit"],
+      [30.038899898529053,"update_request","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","AGENT_EXECUTING","unit"],
+      [30.602999925613403,"update_request","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","AGENT_STAGING_INPUT","unit"],
+      [30.603099822998047,"update_request","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","AGENT_SCHEDULING_PENDING","unit"],
+      [30.603099822998047,"update_request","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","AGENT_SCHEDULING","unit"],
+      [31.685499906539917,"update_pushed","update.0.child","update.0.child.idler._idle_cb","unit.000001","","AGENT_EXECUTING_PENDING","unit"],
+      [31.685499906539917,"update_pushed","update.0.child","update.0.child.idler._idle_cb","unit.000001","","AGENT_EXECUTING","unit"],
+      [32.286700010299680,"update_pushed","update.0.child","update.0.child.idler._idle_cb","unit.000001","","AGENT_STAGING_INPUT","unit"],
+      [32.286700010299680,"update_pushed","update.0.child","update.0.child.idler._idle_cb","unit.000001","","AGENT_SCHEDULING_PENDING","unit"],
+      [32.286700010299680,"update_pushed","update.0.child","update.0.child.idler._idle_cb","unit.000001","","AGENT_SCHEDULING","unit"],
+      [32.746000051498410,"exec_stop","agent.executing.0.child","Watcher","unit.000001","","","unit"],
+      [32.746399879455566,"state","agent.executing.0.child","Watcher","unit.000001","AGENT_STAGING_OUTPUT_PENDING","","unit"],
+      [32.746899843215940,"put","agent.executing.0.child","Watcher","unit.000001","AGENT_STAGING_OUTPUT_PENDING","agent.staging.output.queue.input.0000","unit"],
+      [32.752699851989746,"update_request","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","AGENT_STAGING_OUTPUT_PENDING","unit"],
+      [32.757499933242800,"unschedule_start","agent.scheduling.0.child","agent.scheduling.0.child.subscriber.unschedule_cb","unit.000001","","","unit"],
+      [32.757899999618530,"unschedule_stop","agent.scheduling.0.child","agent.scheduling.0.child.subscriber.unschedule_cb","unit.000001","","","unit"],
+      [32.772799968719480,"get","agent.staging.output.0.child","MainThread","unit.000001","AGENT_STAGING_OUTPUT_PENDING","","unit"],
+      [32.773099899291990,"state","agent.staging.output.0.child","MainThread","unit.000001","AGENT_STAGING_OUTPUT","","unit"],
+      [32.773399829864500,"staging_stdout_start","agent.staging.output.0.child","MainThread","unit.000001","","","unit"],
+      [32.773399829864500,"staging_stdout_stop","agent.staging.output.0.child","MainThread","unit.000001","","","unit"],
+      [32.773399829864500,"staging_stderr_start","agent.staging.output.0.child","MainThread","unit.000001","","","unit"],
+      [32.773499965667725,"staging_stderr_stop","agent.staging.output.0.child","MainThread","unit.000001","","","unit"],
+      [32.773499965667725,"staging_uprof_start","agent.staging.output.0.child","MainThread","unit.000001","","","unit"],
+      [32.773499965667725,"staging_uprof_stop","agent.staging.output.0.child","MainThread","unit.000001","","","unit"],
+      [32.773499965667725,"state","agent.staging.output.0.child","MainThread","unit.000001","UMGR_STAGING_OUTPUT_PENDING","","unit"],
+      [32.774399995803830,"update_request","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","AGENT_STAGING_OUTPUT","unit"],
+      [32.774499893188480,"update_request","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","UMGR_STAGING_OUTPUT_PENDING","unit"],
+      [32.841500043869020,"update_pushed","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","AGENT_STAGING_OUTPUT_PENDING","unit"],
+      [32.841699838638306,"update_pushed","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","AGENT_STAGING_OUTPUT","unit"],
+      [32.841699838638306,"update_pushed","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","UMGR_STAGING_OUTPUT_PENDING","unit"],
+      [32.851099967956540,"update_request","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","AGENT_EXECUTING_PENDING","unit"],
+      [32.851199865341190,"update_request","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","AGENT_EXECUTING","unit"],
+      [32.893699884414670,"get","umgr.0000","umgr.0000.idler._unit_pull_cb","unit.000001","","","unit"],
+      [32.895799875259400,"update_request","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","UMGR_STAGING_OUTPUT_PENDING","unit"],
+      [32.897500038146970,"put","umgr.0000","umgr.0000.idler._unit_pull_cb","unit.000001","UMGR_STAGING_OUTPUT_PENDING","umgr.staging.output.queue.input.0000","unit"],
+      [32.901700019836426,"get","umgr.staging.output.0.child","MainThread","unit.000001","UMGR_STAGING_OUTPUT_PENDING","","unit"],
+      [32.905900001525880,"state","umgr.staging.output.0.child","MainThread","unit.000001","UMGR_STAGING_OUTPUT","","unit"],
+      [32.906699895858765,"state","umgr.staging.output.0.child","MainThread","unit.000001","DONE","","unit"],
+      [32.907799959182740,"update_request","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","UMGR_STAGING_OUTPUT","unit"],
+      [32.945099830627440,"update_pushed","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","AGENT_EXECUTING_PENDING","unit"],
+      [32.945099830627440,"update_pushed","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","AGENT_EXECUTING","unit"],
+      [32.945099830627440,"update_pushed","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","UMGR_STAGING_OUTPUT_PENDING","unit"],
+      [32.945299863815310,"update_pushed","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","UMGR_STAGING_OUTPUT","unit"],
+      [32.946099996566770,"update_request","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","DONE","unit"],
+      [33.986799955368040,"update_pushed","update.0.child","update.0.child.subscriber._state_cb","unit.000001","","DONE","unit"]],
   "details": {
-    "hostid": null,
-    "uid": "unit.000071",
-    "cfg": {"hostid":null,"uid":"unit.000001","cfg":{"kernel":null,"executable":"/bin/sleep","name":null,"restartable":false,"output_staging":[],"stdout":null,"pre_exec":null,"mpi":false,"environment":null,"cleanup":false,"arguments":["2"],"stderr":null,"cores":1,"post_exec":null,"input_staging":[],"pilot":null},"etype":"unit","has":[],"children":[],"description":{"kernel":null,"executable":"/bin/sleep","name":null,"restartable":false,"output_staging":[],"stdout":null,"pre_exec":null,"mpi":false,"environment":null,"cleanup":false,"arguments":["2"],"stderr":null,"cores":1,"post_exec":null,"input_staging":[],"pilot":null}}
-}
+     "hostid": null,
+     "uid"   : "unit.000071",
+     "cfg"   : {
+         "hostid": null,
+         "uid"   : "unit.000001",
+         "cfg"   : {
+             "kernel"        : null,
+             "executable"    : "/bin/sleep",
+             "name"          : null,
+             "restartable"   : false,
+             "output_staging": [],
+             "stdout"        : null,
+             "pre_exec"      : null,
+             "mpi"           : false,
+             "environment"   : null,
+             "cleanup"       : false,
+             "arguments"     : ["2"],
+             "stderr"        : null,
+             "cores"         : 1,
+             "post_exec"     : null,
+             "input_staging" : [],
+             "pilot"         : null},
+             "etype"         : "unit",
+             "has"           : [],
+             "children"      : [],
+             "description"   : {
+                 "kernel"        : null,
+                 "executable"    : "/bin/sleep",
+                 "name"          : null,
+                 "restartable"   : false,
+                 "output_staging": [],
+                 "stdout"        : null,
+                 "pre_exec"      : null,
+                 "mpi"           : false,
+                 "environment"   : null,
+                 "cleanup"       : false,
+                 "arguments"     : ["2"],
+                 "stderr"        : null,
+                 "cores"         : 1,
+                 "post_exec"     : null,
+                 "input_staging" : [],
+                 "pilot"         : null
+             }
+     }
+}
```

### Comparing `radical.analytics-1.5.0/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007/pmgr.0000.prof` & `radical.analytics-1.6.7/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007/pmgr.0000.prof`

 * *Files identical despite different names*

### Comparing `radical.analytics-1.5.0/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007.prof` & `radical.analytics-1.6.7/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007.prof`

 * *Files identical despite different names*

### Comparing `radical.analytics-1.5.0/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007/umgr.0000.prof` & `radical.analytics-1.6.7/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007/umgr.0000.prof`

 * *Files identical despite different names*

### Comparing `radical.analytics-1.5.0/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007/umgr.scheduling.0.child.prof` & `radical.analytics-1.6.7/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007/umgr.scheduling.0.child.prof`

 * *Files identical despite different names*

### Comparing `radical.analytics-1.5.0/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007/umgr.staging.input.0.child.prof` & `radical.analytics-1.6.7/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007/umgr.staging.input.0.child.prof`

 * *Files identical despite different names*

### Comparing `radical.analytics-1.5.0/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007/umgr.staging.output.0.child.prof` & `radical.analytics-1.6.7/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007/umgr.staging.output.0.child.prof`

 * *Files identical despite different names*

### Comparing `radical.analytics-1.5.0/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007/update.0.child.prof` & `radical.analytics-1.6.7/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007/update.0.child.prof`

 * *Files identical despite different names*

### Comparing `radical.analytics-1.5.0/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007.json` & `radical.analytics-1.6.7/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007.json`

 * *Files identical despite different names*

### Comparing `radical.analytics-1.5.0/tests/test_duration_method.py` & `radical.analytics-1.6.7/tests/test_duration_method.py`

 * *Files identical despite different names*

### Comparing `radical.analytics-1.5.0/tests/test_entity.py` & `radical.analytics-1.6.7/tests/test_entity.py`

 * *Files identical despite different names*

