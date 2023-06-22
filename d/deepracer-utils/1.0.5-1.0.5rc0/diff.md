# Comparing `tmp/deepracer-utils-1.0.5.tar.gz` & `tmp/deepracer-utils-1.0.5rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepracer-utils-1.0.5.tar", last modified: Thu Jun 22 17:49:53 2023, max compression
+gzip compressed data, was "deepracer-utils-1.0.5rc0.tar", last modified: Sun May  7 10:31:35 2023, max compression
```

## Comparing `deepracer-utils-1.0.5.tar` & `deepracer-utils-1.0.5rc0.tar`

### file list

```diff
@@ -1,260 +1,260 @@
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.147510 deepracer-utils-1.0.5/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)       35 2021-11-14 14:06:51.000000 deepracer-utils-1.0.5/.gitattributes
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     1863 2023-05-07 10:31:02.000000 deepracer-utils-1.0.5/.gitignore
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     1002 2021-11-14 14:06:51.000000 deepracer-utils-1.0.5/LICENSE
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      101 2021-11-14 14:06:51.000000 deepracer-utils-1.0.5/MANIFEST.in
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     4347 2023-06-22 17:49:53.147510 deepracer-utils-1.0.5/PKG-INFO
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     3413 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/README.md
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.147510 deepracer-utils-1.0.5/deepracer/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      145 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/deepracer/__init__.py
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      342 2021-11-14 14:06:51.000000 deepracer-utils-1.0.5/deepracer/__main__.py
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      497 2023-06-22 17:49:53.147510 deepracer-utils-1.0.5/deepracer/_version.py
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.091509 deepracer-utils-1.0.5/deepracer/boto3_enhancer/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     2303 2021-11-14 14:06:51.000000 deepracer-utils-1.0.5/deepracer/boto3_enhancer/__init__.py
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.083509 deepracer-utils-1.0.5/deepracer/boto3_enhancer/models/
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.083509 deepracer-utils-1.0.5/deepracer/boto3_enhancer/models/deepracer/
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.091509 deepracer-utils-1.0.5/deepracer/boto3_enhancer/models/deepracer/2019-04-01/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   112300 2023-05-07 10:31:02.000000 deepracer-utils-1.0.5/deepracer/boto3_enhancer/models/deepracer/2019-04-01/service-2.json
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.091509 deepracer-utils-1.0.5/deepracer/console/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)       61 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/deepracer/console/__init__.py
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     7842 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/deepracer/console/helper.py
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.091509 deepracer-utils-1.0.5/deepracer/logs/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      322 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/deepracer/logs/__init__.py
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    16030 2023-04-01 13:03:18.000000 deepracer-utils-1.0.5/deepracer/logs/handler.py
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    16576 2023-04-01 13:03:18.000000 deepracer-utils-1.0.5/deepracer/logs/log.py
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    39268 2023-04-01 13:03:18.000000 deepracer-utils-1.0.5/deepracer/logs/log_utils.py
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    17340 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/deepracer/logs/metrics.py
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      301 2023-03-29 12:56:34.000000 deepracer-utils-1.0.5/deepracer/logs/misc.py
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.091509 deepracer-utils-1.0.5/deepracer/model/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)       82 2021-11-14 14:06:51.000000 deepracer-utils-1.0.5/deepracer/model/__init__.py
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     3934 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/deepracer/model/visualization.py
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.095509 deepracer-utils-1.0.5/deepracer/tracks/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)       69 2021-11-14 14:06:51.000000 deepracer-utils-1.0.5/deepracer/tracks/__init__.py
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    15519 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/deepracer/tracks/track_utils.py
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.095509 deepracer-utils-1.0.5/deepracer/update_action_speeds/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    11604 2021-11-14 14:06:51.000000 deepracer-utils-1.0.5/deepracer/update_action_speeds/action_space.json
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     2421 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/deepracer/update_action_speeds/updateActionSpeeds.py
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)       77 2021-11-14 14:06:51.000000 deepracer-utils-1.0.5/deepracer/utils.py
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.095509 deepracer-utils-1.0.5/deepracer_utils.egg-info/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     4347 2023-06-22 17:49:53.000000 deepracer-utils-1.0.5/deepracer_utils.egg-info/PKG-INFO
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    14162 2023-06-22 17:49:53.000000 deepracer-utils-1.0.5/deepracer_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)        1 2023-06-22 17:49:53.000000 deepracer-utils-1.0.5/deepracer_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      253 2023-06-22 17:49:53.000000 deepracer-utils-1.0.5/deepracer_utils.egg-info/requires.txt
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)       10 2023-06-22 17:49:53.000000 deepracer-utils-1.0.5/deepracer_utils.egg-info/top_level.txt
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.095509 deepracer-utils-1.0.5/docs/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     1364 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/docs/development.md
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      295 2023-04-01 13:03:18.000000 deepracer-utils-1.0.5/requirements.txt
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      336 2023-06-22 17:49:53.147510 deepracer-utils-1.0.5/setup.cfg
--rwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)     1877 2023-05-07 10:31:05.000000 deepracer-utils-1.0.5/setup.py
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.083509 deepracer-utils-1.0.5/tests/
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.087509 deepracer-utils-1.0.5/tests/deepracer/
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.095509 deepracer-utils-1.0.5/tests/deepracer/boto3_enhancer/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      143 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/boto3_enhancer/test_boto3_client.py
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.095509 deepracer-utils-1.0.5/tests/deepracer/console/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     4094 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/console/test_helper.py
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.095509 deepracer-utils-1.0.5/tests/deepracer/logs/
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.087509 deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.083509 deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/logs/
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.095509 deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/logs/evaluation/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   112947 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/logs/evaluation/evaluation-20220612082853-IBZwYd0MRMqgwKlAe7bb0A-robomaker.log
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   113488 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/logs/evaluation/evaluation-20220612083839-PMfF__s5QJSQT_-E0rEYwg-robomaker.log
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.095509 deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/logs/leaderboard/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   106112 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/logs/leaderboard/leaderboard-20220703172842-wDhqXQC-SkGOinLUdZCQZQ-robomaker.log
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   107041 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/logs/leaderboard/leaderboard-20220703174103-zi4mg1gOTvugQLn-3BfL4g-robomaker.log
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.099509 deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/logs/training/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   137849 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/logs/training/training-20220611230350-EHNgTNY2T9-77qXhqjBi6A-sagemaker.log
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)  5707542 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/logs/training/training-20220611230353-EHNgTNY2T9-77qXhqjBi6A-robomaker.log
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.087509 deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/metrics/
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.107509 deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/metrics/evaluation/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      801 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/metrics/evaluation/evaluation-20220612082523-IBZwYd0MRMqgwKlAe7bb0A.json
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      801 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/metrics/evaluation/evaluation-20220612083508-PMfF__s5QJSQT_-E0rEYwg.json
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.107509 deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/metrics/training/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   153326 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/metrics/training/training-20220611205309-EHNgTNY2T9-77qXhqjBi6A.json
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.087509 deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.087509 deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/evaluation/
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.087509 deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/evaluation/20220612082523-IBZwYd0MRMqgwKlAe7bb0A/
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.107509 deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/evaluation/20220612082523-IBZwYd0MRMqgwKlAe7bb0A/evaluation-simtrace/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   115644 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/evaluation/20220612082523-IBZwYd0MRMqgwKlAe7bb0A/evaluation-simtrace/0-iteration.csv
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.087509 deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/evaluation/20220612083508-PMfF__s5QJSQT_-E0rEYwg/
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.107509 deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/evaluation/20220612083508-PMfF__s5QJSQT_-E0rEYwg/evaluation-simtrace/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   116427 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/evaluation/20220612083508-PMfF__s5QJSQT_-E0rEYwg/evaluation-simtrace/0-iteration.csv
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.087509 deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.119509 deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    81652 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/0-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    77042 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/1-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   155513 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/10-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   233071 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/11-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   162819 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/12-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   214043 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/13-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   252793 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/14-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   261410 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/15-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   209393 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/16-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   259528 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/17-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   235348 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/18-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   279330 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/19-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    72279 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/2-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   312243 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/20-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   434094 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/21-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   480156 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/22-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   378034 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/23-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   486461 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/24-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   555753 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/25-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   585741 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/26-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   658706 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/27-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    72306 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/3-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    85863 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/4-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    87398 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/5-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    92249 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/6-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   114238 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/7-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   109345 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/8-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   131791 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/9-iteration.csv
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.119509 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.087509 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/evaluation-20220709200242/
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.119509 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/evaluation-20220709200242/evaluation-simtrace/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   100069 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/evaluation-20220709200242/evaluation-simtrace/0-iteration.csv
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.087509 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/evaluation-20220709200509/
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.119509 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/evaluation-20220709200509/evaluation-simtrace/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    97505 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/evaluation-20220709200509/evaluation-simtrace/0-iteration.csv
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.087509 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/evaluation-20220709200711/
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.119509 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/evaluation-20220709200711/evaluation-simtrace/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    96515 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/evaluation-20220709200711/evaluation-simtrace/0-iteration.csv
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.119509 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/ip/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      345 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/ip/hyperparameters.json
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.119509 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/metrics/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      799 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/metrics/EvaluationMetrics-20220709200242.json
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      799 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/metrics/EvaluationMetrics-20220709200509.json
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      799 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/metrics/EvaluationMetrics-20220709200711.json
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   129562 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/metrics/TrainingMetrics.json
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.119509 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/model/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     1347 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/model/model_metadata.json
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      814 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/reward_function.py
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.127509 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    81353 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/0-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    84136 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/1-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   168052 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/10-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   178087 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/11-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   214490 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/12-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   193144 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/13-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   194615 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/14-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   251890 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/15-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   227580 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/16-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   248032 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/17-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   320022 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/18-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   313286 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/19-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    73171 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/2-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   361801 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/20-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   344302 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/21-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   434929 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/22-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   454222 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/23-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   374326 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/24-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   421050 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/25-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   460575 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/26-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    90695 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/3-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    93003 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/4-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    98389 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/5-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   112093 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/6-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    98816 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/7-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   146572 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/8-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   137178 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/9-iteration.csv
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.087509 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.087509 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/0/
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.135510 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    47172 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/0-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    50573 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/1-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    96527 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/10-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   117657 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/11-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   101889 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/12-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    89625 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/13-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   148525 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/14-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   123770 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/15-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   106181 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/16-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   126631 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/17-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   174793 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/18-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   168419 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/19-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    39878 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/2-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   179810 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/20-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   156930 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/21-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   188297 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/22-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    48537 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/3-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    55379 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/4-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    85245 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/5-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    67049 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/6-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    77951 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/7-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    78538 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/8-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   139171 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/9-iteration.csv
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.087509 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/1/
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.139510 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    37614 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/0-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    43030 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/1-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    93980 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/10-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   113794 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/11-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   107108 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/12-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   132614 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/13-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   114432 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/14-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   149434 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/15-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   102219 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/16-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   113987 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/17-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   135489 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/18-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   155853 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/19-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    47261 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/2-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   191968 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/20-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   110352 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/21-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   144271 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/22-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    43714 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/3-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    55034 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/4-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    52608 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/5-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    51339 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/6-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    68982 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/7-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   106093 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/8-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    77558 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/9-iteration.csv
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.087509 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/2/
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.143510 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    29966 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/0-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    26515 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/1-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   117025 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/10-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    83693 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/11-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    72713 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/12-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   111947 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/13-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   113485 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/14-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   104342 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/15-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   122551 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/16-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   114585 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/17-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   146897 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/18-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   170834 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/19-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    32485 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/2-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   138286 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/20-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   162069 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/21-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   149478 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/22-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    32675 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/3-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    44562 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/4-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    49757 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/5-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    57740 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/6-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    65111 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/7-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    91385 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/8-iteration.csv
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    79828 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/9-iteration.csv
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.087509 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/evaluation-20220709201503/
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.143510 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/evaluation-20220709201503/evaluation-simtrace/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   109654 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/evaluation-20220709201503/evaluation-simtrace/0-iteration.csv
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.087509 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/evaluation-20220709201704/
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.143510 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/evaluation-20220709201704/evaluation-simtrace/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   114575 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/evaluation-20220709201704/evaluation-simtrace/0-iteration.csv
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.087509 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/evaluation-20220709201920/
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.143510 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/evaluation-20220709201920/evaluation-simtrace/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   110747 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/evaluation-20220709201920/evaluation-simtrace/0-iteration.csv
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.143510 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/ip/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      345 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/ip/hyperparameters.json
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.147510 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/metrics/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      801 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/metrics/EvaluationMetrics-20220709201503.json
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      801 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/metrics/EvaluationMetrics-20220709201704.json
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      801 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/metrics/EvaluationMetrics-20220709201920.json
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    64134 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/metrics/TrainingMetrics.json
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    51847 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/metrics/TrainingMetrics_1.json
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    51846 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/metrics/TrainingMetrics_2.json
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.147510 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/model/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     1347 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/model/model_metadata.json
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    20184 2023-04-01 13:03:18.000000 deepracer-utils-1.0.5/tests/deepracer/logs/test_logs.py
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     1793 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5/tests/deepracer/logs/test_metrics.py
-drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-06-22 17:49:53.147510 deepracer-utils-1.0.5/tests/deepracer/track_utils/
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     2373 2023-04-01 13:03:18.000000 deepracer-utils-1.0.5/tests/deepracer/track_utils/test_track_utils.py
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      397 2023-06-22 17:49:46.000000 deepracer-utils-1.0.5/tox.ini
--rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    68691 2021-11-14 14:06:51.000000 deepracer-utils-1.0.5/versioneer.py
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.924351 deepracer-utils-1.0.5rc0/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)       35 2021-11-14 14:06:51.000000 deepracer-utils-1.0.5rc0/.gitattributes
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     1863 2023-05-07 10:31:02.000000 deepracer-utils-1.0.5rc0/.gitignore
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     1002 2021-11-14 14:06:51.000000 deepracer-utils-1.0.5rc0/LICENSE
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      101 2021-11-14 14:06:51.000000 deepracer-utils-1.0.5rc0/MANIFEST.in
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     4350 2023-05-07 10:31:35.924351 deepracer-utils-1.0.5rc0/PKG-INFO
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     3413 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/README.md
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.924351 deepracer-utils-1.0.5rc0/deepracer/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      145 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/deepracer/__init__.py
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      342 2021-11-14 14:06:51.000000 deepracer-utils-1.0.5rc0/deepracer/__main__.py
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      500 2023-05-07 10:31:35.924351 deepracer-utils-1.0.5rc0/deepracer/_version.py
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.872350 deepracer-utils-1.0.5rc0/deepracer/boto3_enhancer/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     2303 2021-11-14 14:06:51.000000 deepracer-utils-1.0.5rc0/deepracer/boto3_enhancer/__init__.py
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.868350 deepracer-utils-1.0.5rc0/deepracer/boto3_enhancer/models/
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.868350 deepracer-utils-1.0.5rc0/deepracer/boto3_enhancer/models/deepracer/
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.872350 deepracer-utils-1.0.5rc0/deepracer/boto3_enhancer/models/deepracer/2019-04-01/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   112300 2023-05-07 10:31:02.000000 deepracer-utils-1.0.5rc0/deepracer/boto3_enhancer/models/deepracer/2019-04-01/service-2.json
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.876350 deepracer-utils-1.0.5rc0/deepracer/console/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)       61 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/deepracer/console/__init__.py
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     7842 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/deepracer/console/helper.py
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.876350 deepracer-utils-1.0.5rc0/deepracer/logs/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      322 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/deepracer/logs/__init__.py
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    16030 2023-04-01 13:03:18.000000 deepracer-utils-1.0.5rc0/deepracer/logs/handler.py
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    16576 2023-04-01 13:03:18.000000 deepracer-utils-1.0.5rc0/deepracer/logs/log.py
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    39268 2023-04-01 13:03:18.000000 deepracer-utils-1.0.5rc0/deepracer/logs/log_utils.py
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    17340 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/deepracer/logs/metrics.py
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      301 2023-03-29 12:56:34.000000 deepracer-utils-1.0.5rc0/deepracer/logs/misc.py
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.876350 deepracer-utils-1.0.5rc0/deepracer/model/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)       82 2021-11-14 14:06:51.000000 deepracer-utils-1.0.5rc0/deepracer/model/__init__.py
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     3934 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/deepracer/model/visualization.py
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.876350 deepracer-utils-1.0.5rc0/deepracer/tracks/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)       69 2021-11-14 14:06:51.000000 deepracer-utils-1.0.5rc0/deepracer/tracks/__init__.py
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    15519 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/deepracer/tracks/track_utils.py
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.876350 deepracer-utils-1.0.5rc0/deepracer/update_action_speeds/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    11604 2021-11-14 14:06:51.000000 deepracer-utils-1.0.5rc0/deepracer/update_action_speeds/action_space.json
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     2421 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/deepracer/update_action_speeds/updateActionSpeeds.py
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)       77 2021-11-14 14:06:51.000000 deepracer-utils-1.0.5rc0/deepracer/utils.py
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.876350 deepracer-utils-1.0.5rc0/deepracer_utils.egg-info/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     4350 2023-05-07 10:31:35.000000 deepracer-utils-1.0.5rc0/deepracer_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    14162 2023-05-07 10:31:35.000000 deepracer-utils-1.0.5rc0/deepracer_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)        1 2023-05-07 10:31:35.000000 deepracer-utils-1.0.5rc0/deepracer_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      253 2023-05-07 10:31:35.000000 deepracer-utils-1.0.5rc0/deepracer_utils.egg-info/requires.txt
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)       10 2023-05-07 10:31:35.000000 deepracer-utils-1.0.5rc0/deepracer_utils.egg-info/top_level.txt
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.876350 deepracer-utils-1.0.5rc0/docs/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     1364 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/docs/development.md
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      295 2023-04-01 13:03:18.000000 deepracer-utils-1.0.5rc0/requirements.txt
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      336 2023-05-07 10:31:35.924351 deepracer-utils-1.0.5rc0/setup.cfg
+-rwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)     1877 2023-05-07 10:31:05.000000 deepracer-utils-1.0.5rc0/setup.py
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.868350 deepracer-utils-1.0.5rc0/tests/
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.872350 deepracer-utils-1.0.5rc0/tests/deepracer/
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.876350 deepracer-utils-1.0.5rc0/tests/deepracer/boto3_enhancer/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      143 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/boto3_enhancer/test_boto3_client.py
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.876350 deepracer-utils-1.0.5rc0/tests/deepracer/console/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     4094 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/console/test_helper.py
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.876350 deepracer-utils-1.0.5rc0/tests/deepracer/logs/
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.868350 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.868350 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/logs/
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.876350 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/logs/evaluation/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   112947 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/logs/evaluation/evaluation-20220612082853-IBZwYd0MRMqgwKlAe7bb0A-robomaker.log
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   113488 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/logs/evaluation/evaluation-20220612083839-PMfF__s5QJSQT_-E0rEYwg-robomaker.log
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.876350 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/logs/leaderboard/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   106112 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/logs/leaderboard/leaderboard-20220703172842-wDhqXQC-SkGOinLUdZCQZQ-robomaker.log
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   107041 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/logs/leaderboard/leaderboard-20220703174103-zi4mg1gOTvugQLn-3BfL4g-robomaker.log
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.876350 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/logs/training/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   137849 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/logs/training/training-20220611230350-EHNgTNY2T9-77qXhqjBi6A-sagemaker.log
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)  5707542 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/logs/training/training-20220611230353-EHNgTNY2T9-77qXhqjBi6A-robomaker.log
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.868350 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/metrics/
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.884350 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/metrics/evaluation/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      801 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/metrics/evaluation/evaluation-20220612082523-IBZwYd0MRMqgwKlAe7bb0A.json
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      801 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/metrics/evaluation/evaluation-20220612083508-PMfF__s5QJSQT_-E0rEYwg.json
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.884350 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/metrics/training/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   153326 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/metrics/training/training-20220611205309-EHNgTNY2T9-77qXhqjBi6A.json
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.868350 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.868350 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/evaluation/
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.868350 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/evaluation/20220612082523-IBZwYd0MRMqgwKlAe7bb0A/
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.884350 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/evaluation/20220612082523-IBZwYd0MRMqgwKlAe7bb0A/evaluation-simtrace/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   115644 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/evaluation/20220612082523-IBZwYd0MRMqgwKlAe7bb0A/evaluation-simtrace/0-iteration.csv
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.868350 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/evaluation/20220612083508-PMfF__s5QJSQT_-E0rEYwg/
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.884350 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/evaluation/20220612083508-PMfF__s5QJSQT_-E0rEYwg/evaluation-simtrace/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   116427 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/evaluation/20220612083508-PMfF__s5QJSQT_-E0rEYwg/evaluation-simtrace/0-iteration.csv
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.868350 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.896351 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    81652 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/0-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    77042 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/1-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   155513 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/10-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   233071 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/11-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   162819 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/12-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   214043 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/13-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   252793 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/14-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   261410 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/15-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   209393 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/16-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   259528 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/17-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   235348 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/18-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   279330 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/19-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    72279 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/2-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   312243 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/20-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   434094 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/21-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   480156 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/22-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   378034 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/23-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   486461 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/24-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   555753 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/25-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   585741 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/26-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   658706 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/27-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    72306 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/3-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    85863 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/4-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    87398 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/5-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    92249 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/6-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   114238 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/7-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   109345 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/8-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   131791 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/9-iteration.csv
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.896351 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.868350 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/evaluation-20220709200242/
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.896351 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/evaluation-20220709200242/evaluation-simtrace/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   100069 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/evaluation-20220709200242/evaluation-simtrace/0-iteration.csv
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.868350 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/evaluation-20220709200509/
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.896351 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/evaluation-20220709200509/evaluation-simtrace/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    97505 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/evaluation-20220709200509/evaluation-simtrace/0-iteration.csv
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.872350 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/evaluation-20220709200711/
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.896351 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/evaluation-20220709200711/evaluation-simtrace/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    96515 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/evaluation-20220709200711/evaluation-simtrace/0-iteration.csv
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.896351 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/ip/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      345 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/ip/hyperparameters.json
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.896351 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/metrics/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      799 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/metrics/EvaluationMetrics-20220709200242.json
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      799 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/metrics/EvaluationMetrics-20220709200509.json
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      799 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/metrics/EvaluationMetrics-20220709200711.json
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   129562 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/metrics/TrainingMetrics.json
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.896351 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/model/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     1347 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/model/model_metadata.json
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      814 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/reward_function.py
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.904351 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    81353 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/0-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    84136 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/1-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   168052 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/10-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   178087 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/11-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   214490 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/12-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   193144 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/13-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   194615 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/14-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   251890 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/15-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   227580 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/16-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   248032 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/17-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   320022 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/18-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   313286 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/19-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    73171 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/2-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   361801 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/20-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   344302 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/21-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   434929 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/22-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   454222 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/23-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   374326 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/24-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   421050 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/25-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   460575 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/26-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    90695 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/3-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    93003 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/4-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    98389 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/5-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   112093 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/6-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    98816 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/7-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   146572 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/8-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   137178 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/9-iteration.csv
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.872350 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.872350 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.912351 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    47172 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/0-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    50573 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/1-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    96527 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/10-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   117657 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/11-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   101889 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/12-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    89625 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/13-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   148525 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/14-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   123770 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/15-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   106181 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/16-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   126631 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/17-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   174793 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/18-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   168419 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/19-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    39878 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/2-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   179810 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/20-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   156930 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/21-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   188297 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/22-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    48537 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/3-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    55379 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/4-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    85245 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/5-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    67049 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/6-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    77951 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/7-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    78538 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/8-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   139171 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/9-iteration.csv
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.872350 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.916351 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    37614 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/0-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    43030 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/1-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    93980 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/10-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   113794 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/11-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   107108 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/12-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   132614 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/13-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   114432 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/14-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   149434 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/15-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   102219 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/16-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   113987 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/17-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   135489 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/18-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   155853 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/19-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    47261 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/2-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   191968 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/20-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   110352 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/21-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   144271 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/22-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    43714 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/3-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    55034 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/4-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    52608 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/5-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    51339 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/6-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    68982 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/7-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   106093 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/8-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    77558 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/9-iteration.csv
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.872350 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.920351 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    29966 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/0-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    26515 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/1-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   117025 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/10-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    83693 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/11-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    72713 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/12-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   111947 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/13-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   113485 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/14-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   104342 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/15-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   122551 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/16-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   114585 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/17-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   146897 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/18-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   170834 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/19-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    32485 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/2-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   138286 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/20-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   162069 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/21-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   149478 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/22-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    32675 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/3-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    44562 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/4-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    49757 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/5-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    57740 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/6-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    65111 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/7-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    91385 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/8-iteration.csv
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    79828 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/9-iteration.csv
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.872350 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/evaluation-20220709201503/
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.920351 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/evaluation-20220709201503/evaluation-simtrace/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   109654 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/evaluation-20220709201503/evaluation-simtrace/0-iteration.csv
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.872350 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/evaluation-20220709201704/
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.920351 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/evaluation-20220709201704/evaluation-simtrace/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   114575 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/evaluation-20220709201704/evaluation-simtrace/0-iteration.csv
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.872350 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/evaluation-20220709201920/
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.920351 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/evaluation-20220709201920/evaluation-simtrace/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)   110747 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/evaluation-20220709201920/evaluation-simtrace/0-iteration.csv
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.920351 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/ip/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      345 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/ip/hyperparameters.json
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.924351 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/metrics/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      801 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/metrics/EvaluationMetrics-20220709201503.json
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      801 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/metrics/EvaluationMetrics-20220709201704.json
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      801 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/metrics/EvaluationMetrics-20220709201920.json
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    64134 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/metrics/TrainingMetrics.json
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    51847 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/metrics/TrainingMetrics_1.json
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    51846 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/metrics/TrainingMetrics_2.json
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.924351 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/model/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     1347 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/model/model_metadata.json
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    20184 2023-04-01 13:03:18.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/test_logs.py
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     1793 2022-08-11 19:53:40.000000 deepracer-utils-1.0.5rc0/tests/deepracer/logs/test_metrics.py
+drwxrwxr-x   0 ludvigse  (1000) ludvigse  (1000)        0 2023-05-07 10:31:35.924351 deepracer-utils-1.0.5rc0/tests/deepracer/track_utils/
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)     2373 2023-04-01 13:03:18.000000 deepracer-utils-1.0.5rc0/tests/deepracer/track_utils/test_track_utils.py
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)      397 2023-04-01 13:03:18.000000 deepracer-utils-1.0.5rc0/tox.ini
+-rw-rw-r--   0 ludvigse  (1000) ludvigse  (1000)    68691 2021-11-14 14:06:51.000000 deepracer-utils-1.0.5rc0/versioneer.py
```

### Comparing `deepracer-utils-1.0.5/.gitignore` & `deepracer-utils-1.0.5rc0/.gitignore`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/LICENSE` & `deepracer-utils-1.0.5rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/PKG-INFO` & `deepracer-utils-1.0.5rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepracer-utils
-Version: 1.0.5
+Version: 1.0.5rc0
 Summary: A set of tools for working with DeepRacer training
 Home-page: https://github.com/aws-deepracer-community/deepracer-utils/
 Author: AWS DeepRacer Community
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/aws-deepracer-community/deepracer-utils/issues
 Project-URL: Source, https://github.com/aws-deepracer-community/deepracer-utils/
 Keywords: aws deepracer awsdeepracer
```

### Comparing `deepracer-utils-1.0.5/README.md` & `deepracer-utils-1.0.5rc0/README.md`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/deepracer/boto3_enhancer/__init__.py` & `deepracer-utils-1.0.5rc0/deepracer/boto3_enhancer/__init__.py`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/deepracer/boto3_enhancer/models/deepracer/2019-04-01/service-2.json` & `deepracer-utils-1.0.5rc0/deepracer/boto3_enhancer/models/deepracer/2019-04-01/service-2.json`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/deepracer/console/helper.py` & `deepracer-utils-1.0.5rc0/deepracer/console/helper.py`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/deepracer/logs/handler.py` & `deepracer-utils-1.0.5rc0/deepracer/logs/handler.py`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/deepracer/logs/log.py` & `deepracer-utils-1.0.5rc0/deepracer/logs/log.py`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/deepracer/logs/log_utils.py` & `deepracer-utils-1.0.5rc0/deepracer/logs/log_utils.py`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/deepracer/logs/metrics.py` & `deepracer-utils-1.0.5rc0/deepracer/logs/metrics.py`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/deepracer/model/visualization.py` & `deepracer-utils-1.0.5rc0/deepracer/model/visualization.py`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/deepracer/tracks/track_utils.py` & `deepracer-utils-1.0.5rc0/deepracer/tracks/track_utils.py`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/deepracer/update_action_speeds/action_space.json` & `deepracer-utils-1.0.5rc0/deepracer/update_action_speeds/action_space.json`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/deepracer/update_action_speeds/updateActionSpeeds.py` & `deepracer-utils-1.0.5rc0/deepracer/update_action_speeds/updateActionSpeeds.py`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/deepracer_utils.egg-info/PKG-INFO` & `deepracer-utils-1.0.5rc0/deepracer_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepracer-utils
-Version: 1.0.5
+Version: 1.0.5rc0
 Summary: A set of tools for working with DeepRacer training
 Home-page: https://github.com/aws-deepracer-community/deepracer-utils/
 Author: AWS DeepRacer Community
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/aws-deepracer-community/deepracer-utils/issues
 Project-URL: Source, https://github.com/aws-deepracer-community/deepracer-utils/
 Keywords: aws deepracer awsdeepracer
```

### Comparing `deepracer-utils-1.0.5/deepracer_utils.egg-info/SOURCES.txt` & `deepracer-utils-1.0.5rc0/deepracer_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/docs/development.md` & `deepracer-utils-1.0.5rc0/docs/development.md`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/setup.py` & `deepracer-utils-1.0.5rc0/setup.py`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/console/test_helper.py` & `deepracer-utils-1.0.5rc0/tests/deepracer/console/test_helper.py`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/logs/evaluation/evaluation-20220612082853-IBZwYd0MRMqgwKlAe7bb0A-robomaker.log` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/logs/evaluation/evaluation-20220612082853-IBZwYd0MRMqgwKlAe7bb0A-robomaker.log`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/logs/evaluation/evaluation-20220612083839-PMfF__s5QJSQT_-E0rEYwg-robomaker.log` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/logs/evaluation/evaluation-20220612083839-PMfF__s5QJSQT_-E0rEYwg-robomaker.log`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/logs/leaderboard/leaderboard-20220703172842-wDhqXQC-SkGOinLUdZCQZQ-robomaker.log` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/logs/leaderboard/leaderboard-20220703172842-wDhqXQC-SkGOinLUdZCQZQ-robomaker.log`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/logs/leaderboard/leaderboard-20220703174103-zi4mg1gOTvugQLn-3BfL4g-robomaker.log` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/logs/leaderboard/leaderboard-20220703174103-zi4mg1gOTvugQLn-3BfL4g-robomaker.log`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/logs/training/training-20220611230350-EHNgTNY2T9-77qXhqjBi6A-sagemaker.log` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/logs/training/training-20220611230350-EHNgTNY2T9-77qXhqjBi6A-sagemaker.log`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/logs/training/training-20220611230353-EHNgTNY2T9-77qXhqjBi6A-robomaker.log` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/logs/training/training-20220611230353-EHNgTNY2T9-77qXhqjBi6A-robomaker.log`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/metrics/evaluation/evaluation-20220612082523-IBZwYd0MRMqgwKlAe7bb0A.json` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/metrics/evaluation/evaluation-20220612082523-IBZwYd0MRMqgwKlAe7bb0A.json`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/metrics/evaluation/evaluation-20220612083508-PMfF__s5QJSQT_-E0rEYwg.json` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/metrics/evaluation/evaluation-20220612083508-PMfF__s5QJSQT_-E0rEYwg.json`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/metrics/training/training-20220611205309-EHNgTNY2T9-77qXhqjBi6A.json` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/metrics/training/training-20220611205309-EHNgTNY2T9-77qXhqjBi6A.json`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/evaluation/20220612082523-IBZwYd0MRMqgwKlAe7bb0A/evaluation-simtrace/0-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/evaluation/20220612082523-IBZwYd0MRMqgwKlAe7bb0A/evaluation-simtrace/0-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/evaluation/20220612083508-PMfF__s5QJSQT_-E0rEYwg/evaluation-simtrace/0-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/evaluation/20220612083508-PMfF__s5QJSQT_-E0rEYwg/evaluation-simtrace/0-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/0-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/0-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/1-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/1-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/10-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/10-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/11-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/11-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/12-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/12-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/13-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/13-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/14-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/14-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/15-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/15-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/16-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/16-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/17-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/17-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/18-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/18-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/19-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/19-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/2-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/2-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/20-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/20-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/21-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/21-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/22-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/22-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/23-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/23-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/24-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/24-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/25-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/25-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/26-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/26-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/27-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/27-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/3-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/3-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/4-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/4-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/5-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/5-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/6-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/6-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/7-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/7-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/8-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/8-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/9-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-console-logs/sim-trace/training/training-simtrace/9-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/evaluation-20220709200242/evaluation-simtrace/0-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/evaluation-20220709200242/evaluation-simtrace/0-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/evaluation-20220709200509/evaluation-simtrace/0-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/evaluation-20220709200509/evaluation-simtrace/0-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/evaluation-20220709200711/evaluation-simtrace/0-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/evaluation-20220709200711/evaluation-simtrace/0-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/metrics/EvaluationMetrics-20220709200242.json` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/metrics/EvaluationMetrics-20220709200242.json`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/metrics/EvaluationMetrics-20220709200509.json` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/metrics/EvaluationMetrics-20220709200509.json`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/metrics/EvaluationMetrics-20220709200711.json` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/metrics/EvaluationMetrics-20220709200711.json`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/metrics/TrainingMetrics.json` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/metrics/TrainingMetrics.json`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/model/model_metadata.json` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/model/model_metadata.json`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/reward_function.py` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/reward_function.py`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/0-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/0-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/1-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/1-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/10-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/10-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/11-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/11-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/12-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/12-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/13-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/13-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/14-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/14-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/15-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/15-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/16-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/16-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/17-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/17-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/18-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/18-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/19-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/19-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/2-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/2-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/20-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/20-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/21-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/21-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/22-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/22-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/23-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/23-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/24-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/24-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/25-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/25-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/26-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/26-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/3-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/3-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/4-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/4-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/5-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/5-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/6-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/6-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/7-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/7-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/8-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/8-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/9-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-1-logs/training-simtrace/9-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/0-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/0-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/1-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/1-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/10-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/10-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/11-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/11-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/12-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/12-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/13-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/13-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/14-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/14-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/15-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/15-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/16-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/16-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/17-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/17-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/18-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/18-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/19-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/19-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/2-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/2-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/20-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/20-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/21-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/21-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/22-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/22-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/3-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/3-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/4-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/4-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/5-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/5-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/6-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/6-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/7-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/7-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/8-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/8-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/9-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/0/training-simtrace/9-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/0-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/0-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/1-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/1-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/10-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/10-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/11-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/11-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/12-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/12-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/13-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/13-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/14-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/14-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/15-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/15-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/16-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/16-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/17-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/17-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/18-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/18-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/19-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/19-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/2-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/2-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/20-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/20-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/21-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/21-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/22-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/22-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/3-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/3-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/4-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/4-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/5-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/5-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/6-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/6-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/7-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/7-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/8-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/8-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/9-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/1/training-simtrace/9-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/0-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/0-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/1-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/1-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/10-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/10-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/11-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/11-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/12-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/12-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/13-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/13-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/14-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/14-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/15-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/15-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/16-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/16-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/17-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/17-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/18-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/18-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/19-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/19-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/2-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/2-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/20-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/20-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/21-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/21-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/22-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/22-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/3-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/3-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/4-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/4-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/5-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/5-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/6-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/6-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/7-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/7-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/8-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/8-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/9-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/2/training-simtrace/9-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/evaluation-20220709201503/evaluation-simtrace/0-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/evaluation-20220709201503/evaluation-simtrace/0-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/evaluation-20220709201704/evaluation-simtrace/0-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/evaluation-20220709201704/evaluation-simtrace/0-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/evaluation-20220709201920/evaluation-simtrace/0-iteration.csv` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/evaluation-20220709201920/evaluation-simtrace/0-iteration.csv`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/metrics/EvaluationMetrics-20220709201503.json` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/metrics/EvaluationMetrics-20220709201503.json`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/metrics/EvaluationMetrics-20220709201704.json` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/metrics/EvaluationMetrics-20220709201704.json`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/metrics/EvaluationMetrics-20220709201920.json` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/metrics/EvaluationMetrics-20220709201920.json`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/metrics/TrainingMetrics.json` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/metrics/TrainingMetrics.json`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/metrics/TrainingMetrics_1.json` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/metrics/TrainingMetrics_1.json`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/metrics/TrainingMetrics_2.json` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/metrics/TrainingMetrics_2.json`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/sample-drfc-3-logs/model/model_metadata.json` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/sample-drfc-3-logs/model/model_metadata.json`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/test_logs.py` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/test_logs.py`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/logs/test_metrics.py` & `deepracer-utils-1.0.5rc0/tests/deepracer/logs/test_metrics.py`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/tests/deepracer/track_utils/test_track_utils.py` & `deepracer-utils-1.0.5rc0/tests/deepracer/track_utils/test_track_utils.py`

 * *Files identical despite different names*

### Comparing `deepracer-utils-1.0.5/versioneer.py` & `deepracer-utils-1.0.5rc0/versioneer.py`

 * *Files identical despite different names*

