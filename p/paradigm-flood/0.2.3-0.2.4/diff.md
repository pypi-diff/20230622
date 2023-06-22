# Comparing `tmp/paradigm-flood-0.2.3.tar.gz` & `tmp/paradigm-flood-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paradigm-flood-0.2.3.tar", last modified: Thu Jun 15 17:45:35 2023, max compression
+gzip compressed data, was "paradigm-flood-0.2.4.tar", last modified: Thu Jun 22 00:50:20 2023, max compression
```

## Comparing `paradigm-flood-0.2.3.tar` & `paradigm-flood-0.2.4.tar`

### file list

```diff
@@ -1,71 +1,80 @@
--rw-r--r--   0        0        0      513 2023-06-06 19:32:53.475871 paradigm-flood-0.2.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      607 2023-06-06 19:32:53.476113 paradigm-flood-0.2.3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      193 2023-06-06 19:32:53.476353 paradigm-flood-0.2.3/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0        0        0      781 2023-06-06 19:32:53.476534 paradigm-flood-0.2.3/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      165 2023-06-06 19:32:53.476751 paradigm-flood-0.2.3/.github/workflows/lint.yml
--rw-r--r--   0        0        0      513 2023-06-06 21:16:25.551820 paradigm-flood-0.2.3/.github/workflows/tests.yml
--rw-r--r--   0        0        0      225 2023-05-06 04:56:40.389625 paradigm-flood-0.2.3/.gitignore
--rw-r--r--   0        0        0    10332 2023-06-04 20:22:19.525565 paradigm-flood-0.2.3/CONTRIBUTING.md
--rw-r--r--   0        0        0      832 2023-06-02 00:45:29.473078 paradigm-flood-0.2.3/Dockerfile
--rw-r--r--   0        0        0    10839 2023-06-04 20:13:59.817606 paradigm-flood-0.2.3/LICENSE-APACHE
--rw-r--r--   0        0        0     1085 2023-06-04 20:13:48.830823 paradigm-flood-0.2.3/LICENSE-MIT
--rw-r--r--   0        0        0     2865 2023-06-06 19:32:53.477627 paradigm-flood-0.2.3/README.md
--rw-r--r--   0        0        0  3038209 2023-06-06 19:32:53.483637 paradigm-flood-0.2.3/assets/cover.png
--rw-r--r--   0        0        0      124 2023-06-06 21:20:36.150174 paradigm-flood-0.2.3/examples/equality_test.sh
--rwxr-xr-x   0        0        0     1905 2023-06-15 16:40:12.596585 paradigm-flood-0.2.3/examples/report.sh
--rw-r--r--   0        0        0      625 2023-06-15 17:45:09.872948 paradigm-flood-0.2.3/flood/__init__.py
--rw-r--r--   0        0        0      117 2023-06-04 23:14:01.291195 paradigm-flood-0.2.3/flood/__main__.py
--rw-r--r--   0        0        0     1509 2023-06-04 23:14:01.296616 paradigm-flood-0.2.3/flood/cli/cli_run.py
--rw-r--r--   0        0        0      877 2023-06-04 23:14:01.298637 paradigm-flood-0.2.3/flood/cli/ls_command.py
--rw-r--r--   0        0        0     1221 2023-06-04 23:14:01.302153 paradigm-flood-0.2.3/flood/cli/report_command.py
--rw-r--r--   0        0        0     5729 2023-06-06 20:38:56.286320 paradigm-flood-0.2.3/flood/cli/root_command.py
--rw-r--r--   0        0        0     1315 2023-06-04 23:14:01.307482 paradigm-flood-0.2.3/flood/cli/samples_collect_command.py
--rw-r--r--   0        0        0     1687 2023-06-06 20:39:09.158213 paradigm-flood-0.2.3/flood/cli/samples_download_command.py
--rw-r--r--   0        0        0     1874 2023-06-06 20:39:23.569867 paradigm-flood-0.2.3/flood/cli/samples_ls_command.py
--rw-r--r--   0        0        0      121 2023-06-03 19:54:58.405209 paradigm-flood-0.2.3/flood/generators/__init__.py
--rw-r--r--   0        0        0      199 2023-06-03 19:54:39.491471 paradigm-flood-0.2.3/flood/generators/object_generators/__init__.py
--rw-r--r--   0        0        0      603 2023-06-04 23:14:01.311234 paradigm-flood-0.2.3/flood/generators/object_generators/address_generators.py
--rw-r--r--   0        0        0     4815 2023-06-04 23:14:01.335388 paradigm-flood-0.2.3/flood/generators/object_generators/block_generators.py
--rw-r--r--   0        0        0    17256 2023-06-06 20:39:37.317485 paradigm-flood-0.2.3/flood/generators/object_generators/call_generators.py
--rw-r--r--   0        0        0      337 2023-06-04 23:14:01.306215 paradigm-flood-0.2.3/flood/generators/object_generators/slot_generators.py
--rw-r--r--   0        0        0     4156 2023-06-06 20:41:05.406418 paradigm-flood-0.2.3/flood/generators/object_generators/timing_generators.py
--rw-r--r--   0        0        0      346 2023-06-04 23:14:01.315806 paradigm-flood-0.2.3/flood/generators/object_generators/transaction_generators.py
--rw-r--r--   0        0        0      129 2023-06-02 06:40:02.759112 paradigm-flood-0.2.3/flood/generators/raw_data_sources/__init__.py
--rw-r--r--   0        0        0      465 2023-06-04 23:14:01.312615 paradigm-flood-0.2.3/flood/generators/raw_data_sources/raw_data_spec.py
--rw-r--r--   0        0        0     1935 2023-06-04 23:14:01.327302 paradigm-flood-0.2.3/flood/generators/raw_data_sources/raw_download_utils.py
--rw-r--r--   0        0        0     5688 2023-06-04 23:14:01.364193 paradigm-flood-0.2.3/flood/generators/raw_data_sources/raw_gather_utils.py
--rw-r--r--   0        0        0     4662 2023-06-04 23:14:01.352117 paradigm-flood-0.2.3/flood/generators/raw_data_sources/raw_sample_loading.py
--rw-r--r--   0        0        0      530 2023-06-04 23:14:01.322799 paradigm-flood-0.2.3/flood/generators/rng_utils.py
--rw-r--r--   0        0        0      270 2023-06-02 21:54:22.919273 paradigm-flood-0.2.3/flood/generators/test_generators/__init__.py
--rw-r--r--   0        0        0     1507 2023-06-04 23:14:01.337667 paradigm-flood-0.2.3/flood/generators/test_generators/address_test_generators.py
--rw-r--r--   0        0        0     1559 2023-06-04 23:14:01.331116 paradigm-flood-0.2.3/flood/generators/test_generators/block_test_generators.py
--rw-r--r--   0        0        0     2150 2023-06-04 23:14:01.346034 paradigm-flood-0.2.3/flood/generators/test_generators/contract_test_generators.py
--rw-r--r--   0        0        0     3713 2023-06-04 23:14:01.359661 paradigm-flood-0.2.3/flood/generators/test_generators/generic_test_generators.py
--rw-r--r--   0        0        0     3870 2023-06-04 23:14:01.341234 paradigm-flood-0.2.3/flood/generators/test_generators/log_test_generators.py
--rw-r--r--   0        0        0     5897 2023-06-04 23:14:01.413684 paradigm-flood-0.2.3/flood/generators/test_generators/trace_test_generators.py
--rw-r--r--   0        0        0     1512 2023-06-04 23:14:01.354881 paradigm-flood-0.2.3/flood/generators/test_generators/transaction_test_generators.py
--rw-r--r--   0        0        0     5060 2023-06-04 23:14:01.380065 paradigm-flood-0.2.3/flood/spec.py
--rw-r--r--   0        0        0       78 2023-06-04 23:14:01.343121 paradigm-flood-0.2.3/flood/tests/__init__.py
--rw-r--r--   0        0        0       34 2023-06-04 23:14:01.345292 paradigm-flood-0.2.3/flood/tests/equality_tests/__init__.py
--rw-r--r--   0        0        0     6029 2023-06-15 06:20:28.831486 paradigm-flood-0.2.3/flood/tests/equality_tests/equality_test_runs.py
--rw-r--r--   0        0        0     8501 2023-06-06 20:41:24.278488 paradigm-flood-0.2.3/flood/tests/equality_tests/equality_test_sets.py
--rw-r--r--   0        0        0      154 2023-06-02 00:45:29.480806 paradigm-flood-0.2.3/flood/tests/load_tests/__init__.py
--rw-r--r--   0        0        0     2682 2023-06-04 23:14:01.379714 paradigm-flood-0.2.3/flood/tests/load_tests/load_test_construction.py
--rw-r--r--   0        0        0     5741 2023-06-04 23:14:01.398331 paradigm-flood-0.2.3/flood/tests/load_tests/load_test_plots.py
--rw-r--r--   0        0        0    10264 2023-06-06 20:42:07.952278 paradigm-flood-0.2.3/flood/tests/load_tests/load_test_reports.py
--rw-r--r--   0        0        0    10809 2023-06-06 20:43:29.736775 paradigm-flood-0.2.3/flood/tests/load_tests/load_test_runs.py
--rw-r--r--   0        0        0     4916 2023-06-04 23:14:01.417311 paradigm-flood-0.2.3/flood/tests/load_tests/vegeta.py
--rw-r--r--   0        0        0    12506 2023-06-04 23:14:01.459741 paradigm-flood-0.2.3/flood/tests/runner.py
--rw-r--r--   0        0        0       68 2023-06-02 00:45:29.482030 paradigm-flood-0.2.3/flood/user_io/__init__.py
--rw-r--r--   0        0        0     3265 2023-06-04 23:14:01.401591 paradigm-flood-0.2.3/flood/user_io/file_io.py
--rw-r--r--   0        0        0     5903 2023-06-15 06:32:18.240729 paradigm-flood-0.2.3/flood/user_io/inputs.py
--rw-r--r--   0        0        0     4285 2023-06-04 23:14:01.438468 paradigm-flood-0.2.3/flood/user_io/notebook_io.py
--rw-r--r--   0        0        0     5864 2023-06-06 20:35:25.703304 paradigm-flood-0.2.3/flood/user_io/outputs.py
--rw-r--r--   0        0        0     1890 2023-06-15 17:44:37.473182 paradigm-flood-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      381 2023-06-04 20:35:57.569281 paradigm-flood-0.2.3/tests/README.md
--rw-r--r--   0        0        0      993 2023-06-06 21:03:30.304627 paradigm-flood-0.2.3/tests/conftest.py
--rw-r--r--   0        0        0      593 2023-06-04 20:53:58.379044 paradigm-flood-0.2.3/tests/test_env_vars.py
--rw-r--r--   0        0        0      269 2023-06-06 21:04:00.022725 paradigm-flood-0.2.3/tests/test_equality_tests.py
--rw-r--r--   0        0        0     1128 2023-06-06 21:03:47.012574 paradigm-flood-0.2.3/tests/test_load_tests.py
--rw-r--r--   0        0        0     1736 2023-06-04 16:00:15.996050 paradigm-flood-0.2.3/tests/test_node_parsing.py
--rw-r--r--   0        0        0     4489 1970-01-01 00:00:00.000000 paradigm-flood-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      513 2023-06-06 19:32:53.475871 paradigm-flood-0.2.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      607 2023-06-06 19:32:53.476113 paradigm-flood-0.2.4/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      193 2023-06-06 19:32:53.476353 paradigm-flood-0.2.4/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0        0        0      781 2023-06-06 19:32:53.476534 paradigm-flood-0.2.4/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      165 2023-06-06 19:32:53.476751 paradigm-flood-0.2.4/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      513 2023-06-22 00:28:24.031464 paradigm-flood-0.2.4/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      225 2023-05-06 04:56:40.389625 paradigm-flood-0.2.4/.gitignore
+-rw-r--r--   0        0        0    10332 2023-06-04 20:22:19.525565 paradigm-flood-0.2.4/CONTRIBUTING.md
+-rw-r--r--   0        0        0      832 2023-06-02 00:45:29.473078 paradigm-flood-0.2.4/Dockerfile
+-rw-r--r--   0        0        0    10839 2023-06-04 20:13:59.817606 paradigm-flood-0.2.4/LICENSE-APACHE
+-rw-r--r--   0        0        0     1085 2023-06-04 20:13:48.830823 paradigm-flood-0.2.4/LICENSE-MIT
+-rw-r--r--   0        0        0     2865 2023-06-06 19:32:53.477627 paradigm-flood-0.2.4/README.md
+-rw-r--r--   0        0        0  3038209 2023-06-06 19:32:53.483637 paradigm-flood-0.2.4/assets/cover.png
+-rw-r--r--   0        0        0      124 2023-06-06 21:20:36.150174 paradigm-flood-0.2.4/examples/equality_test.sh
+-rwxr-xr-x   0        0        0     1905 2023-06-15 16:40:12.596585 paradigm-flood-0.2.4/examples/report.sh
+-rw-r--r--   0        0        0      648 2023-06-22 00:49:45.056970 paradigm-flood-0.2.4/flood/__init__.py
+-rw-r--r--   0        0        0      117 2023-06-04 23:14:01.291195 paradigm-flood-0.2.4/flood/__main__.py
+-rw-r--r--   0        0        0     1556 2023-06-22 00:34:03.891521 paradigm-flood-0.2.4/flood/cli/cli_run.py
+-rw-r--r--   0        0        0      877 2023-06-04 23:14:01.298637 paradigm-flood-0.2.4/flood/cli/ls_command.py
+-rw-r--r--   0        0        0     1630 2023-06-22 00:34:03.891718 paradigm-flood-0.2.4/flood/cli/print_command.py
+-rw-r--r--   0        0        0     1221 2023-06-04 23:14:01.302153 paradigm-flood-0.2.4/flood/cli/report_command.py
+-rw-r--r--   0        0        0     6215 2023-06-22 00:34:03.891970 paradigm-flood-0.2.4/flood/cli/root_command.py
+-rw-r--r--   0        0        0     1315 2023-06-04 23:14:01.307482 paradigm-flood-0.2.4/flood/cli/samples_collect_command.py
+-rw-r--r--   0        0        0     1687 2023-06-06 20:39:09.158213 paradigm-flood-0.2.4/flood/cli/samples_download_command.py
+-rw-r--r--   0        0        0     1874 2023-06-06 20:39:23.569867 paradigm-flood-0.2.4/flood/cli/samples_ls_command.py
+-rw-r--r--   0        0        0      121 2023-06-03 19:54:58.405209 paradigm-flood-0.2.4/flood/generators/__init__.py
+-rw-r--r--   0        0        0      199 2023-06-03 19:54:39.491471 paradigm-flood-0.2.4/flood/generators/object_generators/__init__.py
+-rw-r--r--   0        0        0      603 2023-06-04 23:14:01.311234 paradigm-flood-0.2.4/flood/generators/object_generators/address_generators.py
+-rw-r--r--   0        0        0     4815 2023-06-04 23:14:01.335388 paradigm-flood-0.2.4/flood/generators/object_generators/block_generators.py
+-rw-r--r--   0        0        0    17256 2023-06-06 20:39:37.317485 paradigm-flood-0.2.4/flood/generators/object_generators/call_generators.py
+-rw-r--r--   0        0        0      337 2023-06-04 23:14:01.306215 paradigm-flood-0.2.4/flood/generators/object_generators/slot_generators.py
+-rw-r--r--   0        0        0     4156 2023-06-06 20:41:05.406418 paradigm-flood-0.2.4/flood/generators/object_generators/timing_generators.py
+-rw-r--r--   0        0        0      346 2023-06-04 23:14:01.315806 paradigm-flood-0.2.4/flood/generators/object_generators/transaction_generators.py
+-rw-r--r--   0        0        0      129 2023-06-02 06:40:02.759112 paradigm-flood-0.2.4/flood/generators/raw_data_sources/__init__.py
+-rw-r--r--   0        0        0      465 2023-06-04 23:14:01.312615 paradigm-flood-0.2.4/flood/generators/raw_data_sources/raw_data_spec.py
+-rw-r--r--   0        0        0     1935 2023-06-04 23:14:01.327302 paradigm-flood-0.2.4/flood/generators/raw_data_sources/raw_download_utils.py
+-rw-r--r--   0        0        0     5688 2023-06-04 23:14:01.364193 paradigm-flood-0.2.4/flood/generators/raw_data_sources/raw_gather_utils.py
+-rw-r--r--   0        0        0     4662 2023-06-04 23:14:01.352117 paradigm-flood-0.2.4/flood/generators/raw_data_sources/raw_sample_loading.py
+-rw-r--r--   0        0        0      530 2023-06-04 23:14:01.322799 paradigm-flood-0.2.4/flood/generators/rng_utils.py
+-rw-r--r--   0        0        0      307 2023-06-16 00:43:55.812056 paradigm-flood-0.2.4/flood/generators/test_generators/__init__.py
+-rw-r--r--   0        0        0     1507 2023-06-04 23:14:01.337667 paradigm-flood-0.2.4/flood/generators/test_generators/address_test_generators.py
+-rw-r--r--   0        0        0     1559 2023-06-04 23:14:01.331116 paradigm-flood-0.2.4/flood/generators/test_generators/block_test_generators.py
+-rw-r--r--   0        0        0     2150 2023-06-04 23:14:01.346034 paradigm-flood-0.2.4/flood/generators/test_generators/contract_test_generators.py
+-rw-r--r--   0        0        0     5333 2023-06-16 00:44:54.451370 paradigm-flood-0.2.4/flood/generators/test_generators/generic_test_generators.py
+-rw-r--r--   0        0        0     3870 2023-06-04 23:14:01.341234 paradigm-flood-0.2.4/flood/generators/test_generators/log_test_generators.py
+-rw-r--r--   0        0        0      162 2023-06-16 00:43:37.064471 paradigm-flood-0.2.4/flood/generators/test_generators/multi_test_generators.py
+-rw-r--r--   0        0        0     5897 2023-06-04 23:14:01.413684 paradigm-flood-0.2.4/flood/generators/test_generators/trace_test_generators.py
+-rw-r--r--   0        0        0     1512 2023-06-04 23:14:01.354881 paradigm-flood-0.2.4/flood/generators/test_generators/transaction_test_generators.py
+-rw-r--r--   0        0        0       87 2023-06-15 23:24:24.125486 paradigm-flood-0.2.4/flood/runners/__init__.py
+-rw-r--r--   0        0        0       40 2023-06-15 23:57:58.076473 paradigm-flood-0.2.4/flood/runners/generic_runner/__init__.py
+-rw-r--r--   0        0        0     3437 2023-06-22 00:34:03.892257 paradigm-flood-0.2.4/flood/runners/generic_runner/generic_runner_execution.py
+-rw-r--r--   0        0        0       31 2023-06-15 23:25:05.871130 paradigm-flood-0.2.4/flood/runners/multi_runner/__init__.py
+-rw-r--r--   0        0        0     1081 2023-06-15 23:25:35.750693 paradigm-flood-0.2.4/flood/runners/multi_runner/multi_runner_io.py
+-rw-r--r--   0        0        0       32 2023-06-15 23:24:48.633159 paradigm-flood-0.2.4/flood/runners/single_runner/__init__.py
+-rw-r--r--   0        0        0     4845 2023-06-22 00:34:03.892502 paradigm-flood-0.2.4/flood/runners/single_runner/single_runner_execution.py
+-rw-r--r--   0        0        0     4751 2023-06-22 00:34:03.892741 paradigm-flood-0.2.4/flood/runners/single_runner/single_runner_io.py
+-rw-r--r--   0        0        0     6430 2023-06-15 23:32:29.744850 paradigm-flood-0.2.4/flood/runners/single_runner/single_runner_summary.py
+-rw-r--r--   0        0        0     5117 2023-06-20 03:52:27.584215 paradigm-flood-0.2.4/flood/spec.py
+-rw-r--r--   0        0        0       56 2023-06-15 23:55:07.358215 paradigm-flood-0.2.4/flood/tests/__init__.py
+-rw-r--r--   0        0        0       34 2023-06-04 23:14:01.345292 paradigm-flood-0.2.4/flood/tests/equality_tests/__init__.py
+-rw-r--r--   0        0        0     6200 2023-06-22 00:39:58.042086 paradigm-flood-0.2.4/flood/tests/equality_tests/equality_test_runs.py
+-rw-r--r--   0        0        0     8501 2023-06-06 20:41:24.278488 paradigm-flood-0.2.4/flood/tests/equality_tests/equality_test_sets.py
+-rw-r--r--   0        0        0      154 2023-06-02 00:45:29.480806 paradigm-flood-0.2.4/flood/tests/load_tests/__init__.py
+-rw-r--r--   0        0        0     2682 2023-06-04 23:14:01.379714 paradigm-flood-0.2.4/flood/tests/load_tests/load_test_construction.py
+-rw-r--r--   0        0        0     5740 2023-06-15 21:26:24.315199 paradigm-flood-0.2.4/flood/tests/load_tests/load_test_plots.py
+-rw-r--r--   0        0        0    10242 2023-06-15 23:17:43.297886 paradigm-flood-0.2.4/flood/tests/load_tests/load_test_reports.py
+-rw-r--r--   0        0        0    13410 2023-06-22 00:34:03.894287 paradigm-flood-0.2.4/flood/tests/load_tests/load_test_runs.py
+-rw-r--r--   0        0        0    10443 2023-06-20 06:29:09.583999 paradigm-flood-0.2.4/flood/tests/load_tests/vegeta.py
+-rw-r--r--   0        0        0       45 2023-06-15 23:20:48.386860 paradigm-flood-0.2.4/flood/user_io/__init__.py
+-rw-r--r--   0        0        0     5903 2023-06-15 06:32:18.240729 paradigm-flood-0.2.4/flood/user_io/inputs.py
+-rw-r--r--   0        0        0     4285 2023-06-04 23:14:01.438468 paradigm-flood-0.2.4/flood/user_io/notebook_io.py
+-rw-r--r--   0        0        0     5864 2023-06-06 20:35:25.703304 paradigm-flood-0.2.4/flood/user_io/outputs.py
+-rw-r--r--   0        0        0     1919 2023-06-22 00:43:46.791751 paradigm-flood-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      381 2023-06-04 20:35:57.569281 paradigm-flood-0.2.4/tests/README.md
+-rw-r--r--   0        0        0      993 2023-06-06 21:03:30.304627 paradigm-flood-0.2.4/tests/conftest.py
+-rw-r--r--   0        0        0      593 2023-06-04 20:53:58.379044 paradigm-flood-0.2.4/tests/test_env_vars.py
+-rw-r--r--   0        0        0      269 2023-06-06 21:04:00.022725 paradigm-flood-0.2.4/tests/test_equality_tests.py
+-rw-r--r--   0        0        0     1128 2023-06-06 21:03:47.012574 paradigm-flood-0.2.4/tests/test_load_tests.py
+-rw-r--r--   0        0        0     1736 2023-06-04 16:00:15.996050 paradigm-flood-0.2.4/tests/test_node_parsing.py
+-rw-r--r--   0        0        0     4526 1970-01-01 00:00:00.000000 paradigm-flood-0.2.4/PKG-INFO
```

### Comparing `paradigm-flood-0.2.3/.github/ISSUE_TEMPLATE/bug_report.md` & `paradigm-flood-0.2.4/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.3/.github/ISSUE_TEMPLATE/feature_request.md` & `paradigm-flood-0.2.4/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.3/.github/PULL_REQUEST_TEMPLATE.md` & `paradigm-flood-0.2.4/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.3/.github/workflows/tests.yml` & `paradigm-flood-0.2.4/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.3/CONTRIBUTING.md` & `paradigm-flood-0.2.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.3/Dockerfile` & `paradigm-flood-0.2.4/Dockerfile`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.3/LICENSE-APACHE` & `paradigm-flood-0.2.4/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.3/LICENSE-MIT` & `paradigm-flood-0.2.4/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.3/README.md` & `paradigm-flood-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.3/assets/cover.png` & `paradigm-flood-0.2.4/assets/cover.png`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.3/examples/report.sh` & `paradigm-flood-0.2.4/examples/report.sh`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.3/flood/__init__.py` & `paradigm-flood-0.2.4/flood/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """tool for benchmarking RPC endpoints"""
 
 from .generators import *
+from .runners import *
 from .spec import *
 from .tests import *
 from .user_io import *
 
 
-__version__ = '0.2.3'
+__version__ = '0.2.4'
 
 
 def _clean_package_imports() -> None:
     """remove deep nested modules from flood namespace"""
 
     import sys
```

### Comparing `paradigm-flood-0.2.3/flood/cli/cli_run.py` & `paradigm-flood-0.2.4/flood/cli/cli_run.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 
 def run_cli(raw_command: str | None = None) -> None:
     command_index: toolcli.CommandIndex = {
         (): 'flood.cli.root_command',
         ('help',): 'toolcli.command_utils.standard_subcommands.help_command',
         ('ls',): 'flood.cli.ls_command',
+        ('print',): 'flood.cli.print_command',
         ('report',): 'flood.cli.report_command',
         ('samples', 'collect'): 'flood.cli.samples_collect_command',
         ('samples', 'download'): 'flood.cli.samples_download_command',
         ('samples', 'ls'): 'flood.cli.samples_ls_command',
         (
             'version',
         ): 'toolcli.command_utils.standard_subcommands.version_command',
```

### Comparing `paradigm-flood-0.2.3/flood/cli/ls_command.py` & `paradigm-flood-0.2.4/flood/cli/ls_command.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.3/flood/cli/report_command.py` & `paradigm-flood-0.2.4/flood/cli/report_command.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.3/flood/cli/root_command.py` & `paradigm-flood-0.2.4/flood/cli/root_command.py`

 * *Files 6% similar despite different names*

```diff
@@ -97,14 +97,24 @@
             },
             {
                 'name': ['--no-figures'],
                 'help': 'skip generating summary figures in output_dir',
                 'dest': 'figures',
                 'action': 'store_false',
             },
+            {
+                'name': ['--save-raw-output'],
+                'help': 'save raw output from Vegeta',
+                'action': 'store_true',
+            },
+            {
+                'name': ['--deep-check'],
+                'help': 'validate the contents of every RPC response',
+                'action': 'store_true',
+            },
         ],
         'examples': [
             'eth_getBlockByNumber localhost:8545',
             'eth_getLogs localhost:8545 localhost:8546 localhost:8547',
             'all client1=0.0.0.0:8545 client2=0.0.0.0:8546 --equality',
         ],
     }
@@ -119,14 +129,16 @@
     rates: typing.Sequence[int] | typing.Sequence[str] | None,
     duration: int | None,
     random_seed: int | None,
     dry: bool,
     quiet: bool,
     figures: bool,
     equality: bool,
+    save_raw_output: bool,
+    deep_check: bool,
 ) -> None:
     verbose = not quiet
     if nodes is not None and len(nodes) == 0:
         nodes = None
 
     if equality:
         if output_dir is not None:
@@ -161,8 +173,11 @@
             random_seed=random_seed,
             verbose=verbose,
             rates=rates,
             duration=duration,
             dry=dry,
             output_dir=output_dir or True,
             figures=figures,
+            include_raw_output=save_raw_output,
+            deep_check=deep_check,
         )
+
```

### Comparing `paradigm-flood-0.2.3/flood/cli/samples_collect_command.py` & `paradigm-flood-0.2.4/flood/cli/samples_collect_command.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.3/flood/cli/samples_download_command.py` & `paradigm-flood-0.2.4/flood/cli/samples_download_command.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.3/flood/cli/samples_ls_command.py` & `paradigm-flood-0.2.4/flood/cli/samples_ls_command.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.3/flood/generators/object_generators/address_generators.py` & `paradigm-flood-0.2.4/flood/generators/object_generators/address_generators.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.3/flood/generators/object_generators/block_generators.py` & `paradigm-flood-0.2.4/flood/generators/object_generators/block_generators.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.3/flood/generators/object_generators/call_generators.py` & `paradigm-flood-0.2.4/flood/generators/object_generators/call_generators.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.3/flood/generators/object_generators/timing_generators.py` & `paradigm-flood-0.2.4/flood/generators/object_generators/timing_generators.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.3/flood/generators/raw_data_sources/raw_download_utils.py` & `paradigm-flood-0.2.4/flood/generators/raw_data_sources/raw_download_utils.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.3/flood/generators/raw_data_sources/raw_gather_utils.py` & `paradigm-flood-0.2.4/flood/generators/raw_data_sources/raw_gather_utils.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.3/flood/generators/raw_data_sources/raw_sample_loading.py` & `paradigm-flood-0.2.4/flood/generators/raw_data_sources/raw_sample_loading.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.3/flood/generators/rng_utils.py` & `paradigm-flood-0.2.4/flood/generators/rng_utils.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.3/flood/generators/test_generators/address_test_generators.py` & `paradigm-flood-0.2.4/flood/generators/test_generators/address_test_generators.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.3/flood/generators/test_generators/block_test_generators.py` & `paradigm-flood-0.2.4/flood/generators/test_generators/block_test_generators.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.3/flood/generators/test_generators/contract_test_generators.py` & `paradigm-flood-0.2.4/flood/generators/test_generators/contract_test_generators.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.3/flood/generators/test_generators/generic_test_generators.py` & `paradigm-flood-0.2.4/flood/generators/test_generators/generic_test_generators.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
 
 import typing
 
 import flood
-from flood.user_io import file_io
 
 
 #
 # # bookkeeping
 #
 
 
@@ -21,46 +20,69 @@
     }
 
 
 def get_multi_test_generators() -> (
     typing.Mapping[str, flood.MultiLoadTestGenerator]
 ):
     return {
-        get_test_generator_display_name(item): item  # type: ignore
+        get_test_generator_display_name(item, multi=True): item  # type: ignore
         for item in dir(flood)
         if item.startswith('generate_tests_')
     }
 
 
 def get_test_generator(test_name: str) -> flood.LoadTestGenerator:
     function_name = get_test_generator_function_name(test_name)
     if hasattr(flood, function_name):
         return getattr(flood, function_name)  # type: ignore
     else:
         raise Exception()
 
 
-def get_test_generator_display_name(test: str | flood.LoadTestGenerator) -> str:
+def get_tests_generator(test_name: str) -> flood.MultiLoadTestGenerator:
+    function_name = get_test_generator_function_name(test_name)
+    if hasattr(flood, function_name):
+        return getattr(flood, function_name)  # type: ignore
+    else:
+        raise Exception()
+
+
+def get_test_generator_display_name(
+    test: str | flood.LoadTestGenerator,
+    multi: bool = False,
+) -> str:
+    if multi:
+        prefix = 'generate_tests_'
+    else:
+        prefix = 'generate_test_'
+
     if not isinstance(test, str):
         import types
 
         if not isinstance(test, types.FunctionType):
             raise Exception('should be str or function')
         test = test.__name__
 
-    if not test.startswith('generate_test_'):
+    if not test.startswith(prefix):
         raise Exception()
-    test = test[len('generate_test_') :]
+    test = test[len(prefix) :]
     head, tail = test.split('_', 1)
     test = head + '_' + _snake_case_to_camel_case(tail)
     return test
 
 
-def get_test_generator_function_name(display_name: str) -> str:
-    function_name = 'generate_test_' + _camel_case_to_snake_case(display_name)
+def get_test_generator_function_name(
+    display_name: str, multi: bool = False
+) -> str:
+    if multi:
+        prefix = 'generate_tests_'
+    else:
+        prefix = 'generate_test_'
+
+    function_name = prefix + _camel_case_to_snake_case(display_name)
     return function_name
 
 
 def _camel_case_to_snake_case(string: str) -> str:
     # adapted from https://stackoverflow.com/a/1176023
     import re
 
@@ -94,20 +116,53 @@
         rates=rates,
         durations=durations,
         vegeta_kwargs=vegeta_kwargs,
         network=network,
         random_seed=random_seed,
     )
     if output_dir is not None:
-        file_io._save_single_run_test(
+        flood.runners.single_runner.single_runner_io._save_single_run_test(
             test_name=test_name, output_dir=output_dir, test=test
         )
     return test
 
 
+def generate_tests(
+    *,
+    test_name: str,
+    random_seed: flood.RandomSeed | None = None,
+    rates: typing.Sequence[int] | None = None,
+    durations: typing.Sequence[int] | None = None,
+    vegeta_kwargs: flood.VegetaKwargsShorthand | None = None,
+    network: str,
+    output_dir: str | None = None,
+    common_parameters: typing.Mapping[str, typing.Any] | None = None,
+    specific_parameters: typing.Mapping[str, typing.Mapping[str, typing.Any]]
+    | None = None,
+) -> typing.Mapping[str, flood.LoadTest]:
+    if test_name is None:
+        raise Exception('must specify test_name')
+    test_generator = get_tests_generator(test_name)
+    tests = test_generator(
+        rates=rates,
+        durations=durations,
+        vegeta_kwargs=vegeta_kwargs,
+        network=network,
+        random_seed=random_seed,
+        common_parameters=common_parameters,
+        specific_parameters=specific_parameters,
+    )
+    if output_dir is not None:
+        flood.runners.multi_runner.multi_runner_io._save_multi_run_tests(
+            output_dir=output_dir,
+            tests=tests,
+        )
+    return tests
+
+
 # def generate_tests(
 #     test_name: str,
 #     constants: typing.Mapping[str, typing.Any] | None = None,
 #     variables: typing.Mapping[
 #         str, typing.Mapping[str, typing.Sequence[typing.Any]]
 #     ]
 #     | None = None,
@@ -131,7 +186,8 @@
 #     test_generator = get_test_generator(test_name)
 #     tests = []
 #     for test_kwargs in tests_kwargs:
 #         test = test_generator(**test_kwargs)
 #         tests.append(test)
 
 #     return tests
+
```

### Comparing `paradigm-flood-0.2.3/flood/generators/test_generators/log_test_generators.py` & `paradigm-flood-0.2.4/flood/generators/test_generators/log_test_generators.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.3/flood/generators/test_generators/trace_test_generators.py` & `paradigm-flood-0.2.4/flood/generators/test_generators/trace_test_generators.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.3/flood/generators/test_generators/transaction_test_generators.py` & `paradigm-flood-0.2.4/flood/generators/test_generators/transaction_test_generators.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.3/flood/spec.py` & `paradigm-flood-0.2.4/flood/spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,14 +139,15 @@
         max: float
         status_codes: typing.Mapping[str, int]
         errors: typing.Sequence[str]
         first_request_timestamp: str
         last_request_timestamp: str
         last_response_timestamp: str
         final_wait_time: float
+        raw_output: str | None
 
     class LoadTestOutput(typing.TypedDict):
         target_rate: typing.Sequence[int]
         actual_rate: typing.Sequence[float]
         target_duration: typing.Sequence[int]
         actual_duration: typing.Sequence[float]
         requests: typing.Sequence[int]
@@ -161,22 +162,22 @@
         max: typing.Sequence[float]
         status_codes: typing.Sequence[typing.Mapping[str, int]]
         errors: typing.Sequence[typing.Sequence[str]]
         first_request_timestamp: typing.Sequence[str]
         last_request_timestamp: typing.Sequence[str]
         last_response_timestamp: typing.Sequence[str]
         final_wait_time: typing.Sequence[float]
+        raw_output: typing.Sequence[str | None]
 
-    RunType = typing.Literal['single_run']
+    RunType = typing.Literal['single_test']
 
     class SingleRunTestPayload(typing.TypedDict):
         version: str
         type: RunType
         name: str
         test: LoadTest
 
     class SingleRunResultsPayload(typing.TypedDict):
         version: str
         type: RunType
-        test: LoadTest
         nodes: Nodes
         results: typing.Mapping[str, LoadTestOutput]
```

### Comparing `paradigm-flood-0.2.3/flood/tests/equality_tests/equality_test_runs.py` & `paradigm-flood-0.2.4/flood/tests/equality_tests/equality_test_runs.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,18 +22,23 @@
     nodes = flood.parse_nodes(nodes, request_metadata=True)
     for node in nodes.values():
         if node['remote'] is not None:
             raise Exception('remote not supported for equality test')
     if len(nodes) != 2:
         raise Exception('should use two nodes in equality test')
 
+    equality_tests = equality_test_sets.get_all_equality_tests()
+
     # get tests
     if test_name != 'all':
-        raise NotImplementedError('must use test_name="all" for equality test')
-    equality_tests = equality_test_sets.get_all_equality_tests()
+        equality_tests = [t for t in equality_tests if t[0] == test_name]
+        if not equality_tests:
+            raise NotImplementedError(
+                'no matching test found for name "' + test_name + '"'
+            )
 
     if output_dir is None:
         import tempfile
 
         output_dir = tempfile.mkdtemp()
 
     # print preamble
@@ -139,15 +144,15 @@
     test: flood.EqualityTest,
     call: typing.Mapping[str, typing.Any],
 ) -> bool:
     import toolstr
 
     test_name, constructor, args, kwargs = test
 
-    if not toolstr.nested_equal(results[0], results[1]):
+    if results[0] is None or not toolstr.nested_equal(results[0], results[1]):
         print()
         flood.print_text_box('Discrepancies in ' + test_name)
         print()
         flood.print_header('args')
         if len(args) > 0:
             for arg in args:
                 flood.print_bullet(key=arg, value='', colon_str='')
```

### Comparing `paradigm-flood-0.2.3/flood/tests/equality_tests/equality_test_sets.py` & `paradigm-flood-0.2.4/flood/tests/equality_tests/equality_test_sets.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.3/flood/tests/load_tests/load_test_construction.py` & `paradigm-flood-0.2.4/flood/tests/load_tests/load_test_construction.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.3/flood/tests/load_tests/load_test_plots.py` & `paradigm-flood-0.2.4/flood/tests/load_tests/load_test_plots.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import flood
 
 
 def plot_load_test_results(
     outputs: typing.Mapping[str, flood.LoadTestOutput],
     test_name: str,
     output_dir: str | None = None,
-    latency_yscale_log: bool = False,
+    latency_yscale_log: bool = True,
     colors: typing.Mapping[str, str] | None = None,
 ) -> None:
     import os
     import matplotlib.pyplot as plt  # type: ignore
     import toolplot
 
     toolplot.setup_plot_formatting()
```

### Comparing `paradigm-flood-0.2.3/flood/tests/load_tests/load_test_reports.py` & `paradigm-flood-0.2.4/flood/tests/load_tests/load_test_reports.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     from flood.user_io import notebook_io
 
     if metrics is None:
         metrics = ['success', 'throughput', 'p50', 'p90', 'p99']
 
     test_paths_map = {}
     for test_path in test_paths:
-        payload = flood.load_single_run_test_payload(output_dir=test_path)
+        payload = flood.load_single_run_test_payload(test_path)
         name = payload['name']
         test_paths_map[name] = test_path
 
     inputs = {
         'test_paths': test_paths_map,
         'metrics': metrics,
         'test_names': list(test_paths_map.keys()),
@@ -189,15 +189,15 @@
     {
         # load data
         'type': 'code',
         'content': """
             # load data
 
             test_payloads = {{
-                test_name: flood.load_single_run_test_payload(output_dir=test_path)
+                test_name: flood.load_single_run_test_payload(test_path)
                 for test_name, test_path in test_paths.items()
             }}
 
             results_payloads = {{
                 test_name: flood.load_single_run_results_payload(output_dir=test_path)
                 for test_name, test_path in test_paths.items()
             }}
```

### Comparing `paradigm-flood-0.2.3/flood/tests/load_tests/load_test_runs.py` & `paradigm-flood-0.2.4/flood/tests/load_tests/load_test_runs.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 def run_load_tests(
     *,
     node: spec.NodeShorthand | None = None,
     nodes: spec.NodesShorthand | None = None,
     test: spec.LoadTest | None = None,
     tests: typing.Mapping[str, spec.LoadTest] | None = None,
     verbose: bool | int = False,
+    include_raw_output: bool = False,
 ) -> typing.Mapping[str, spec.LoadTestOutput]:
     """run multiple load tests"""
     # parse user_io
     if (node is None) == (nodes is None):
         raise Exception('must specify either node or nodes')
     if (test is None) == (tests is None):
         raise Exception('must specify either test or tests')
@@ -32,99 +33,119 @@
         nodes = user_io.parse_nodes(nodes, request_metadata=False)
     tqdm = user_io.outputs._get_tqdm()
     pbar = {
         'leave': False,
         'desc': 'nodes',
         'position': 0,
         'colour': flood.styles['content'],
-        'disable': not verbose,
+        # 'disable': not verbose,
+        'disable': True,
     }
 
     results = {}
 
     # case: single node and single test
     if node is not None and test is not None:
-        results[node['name']] = schedule_load_test(node=node, test=test)
+        results[node['name']] = schedule_load_test(
+            node=node,
+            test=test,
+            include_raw_output=include_raw_output,
+        )
 
     # case: single node and multiple tests
     elif node is not None and tests is not None:
         for name, test in tqdm.tqdm(tests.items(), **pbar):
             results[name] = schedule_load_test(
-                node=node, verbose=verbose, test=test
+                node=node,
+                verbose=verbose,
+                test=test,
+                include_raw_output=include_raw_output,
             )
 
     # case: multiple nodes and single tests
     elif nodes is not None and test is not None:
         for name, nd in tqdm.tqdm(nodes.items(), **pbar):
             results[name] = schedule_load_test(
-                node=nd, verbose=verbose, test=test
+                node=nd,
+                verbose=verbose,
+                test=test,
+                include_raw_output=include_raw_output,
             )
 
     # case: multiple nodes and multiple tests
     elif nodes is not None and tests is not None:
         for node_name, node in nodes.items():
             for test_name, test in tests.items():
                 results[node_name + '__' + test_name] = schedule_load_test(
                     node=node,
                     verbose=verbose,
                     test=test,
+                    include_raw_output=include_raw_output,
                 )
 
     # case: invalid input
     else:
         raise Exception('invalid user_io')
 
     # join any multiprocessing results
     joined = {}
     for name, result in results.items():
         if isinstance(result, dict):
             joined[name] = result
-        else:
+        elif isinstance(result, tuple):
             process, queue = result
             process.join()
-            joined[name] = queue.get()
+            results_path = queue.get()
+            with open(results_path, 'r') as f:
+                import json
+
+                test_results: spec.SingleRunResultsPayload = json.load(f)
+                joined[name] = test_results['results'][name]
+        else:
+            raise Exception('invalid result type')
 
     return joined
 
 
 def schedule_load_test(
     *,
     node: spec.NodeShorthand,
     test: spec.LoadTest | None = None,
     rates: typing.Sequence[int] | None = None,
     calls: typing.Sequence[typing.Any] | None = None,
     duration: int | None = None,
     durations: typing.Sequence[int] | None = None,
     vegeta_kwargs: typing.Mapping[str, str | None] | None = None,
     verbose: bool | int = False,
+    include_raw_output: bool = False,
     _pbar_kwargs: typing.Mapping[str, typing.Any] | None = None,
 ) -> (
     spec.LoadTestOutput
-    | tuple[multiprocessing.Process, multiprocessing.Queue[spec.LoadTestOutput]]
+    | str
+    | tuple[multiprocessing.Process, multiprocessing.Queue[str]]
 ):
     """runs local tests synchronously, remote tests asynchronously"""
 
     node = user_io.parse_node(node)
     if node['remote'] is not None:
         import multiprocessing
 
-        queue: multiprocessing.Queue[
-            spec.LoadTestOutput
-        ] = multiprocessing.Queue()
+        queue: multiprocessing.Queue[str] = multiprocessing.Queue()
         process = multiprocessing.Process(
             target=run_load_test,
             kwargs=dict(
                 node=node,
                 test=test,
                 rates=rates,
                 calls=calls,
                 duration=duration,
                 durations=durations,
                 vegeta_kwargs=vegeta_kwargs,
                 verbose=verbose,
+                include_raw_output=include_raw_output,
                 _pbar_kwargs=_pbar_kwargs,
                 _container=queue,
             ),
         )
         process.start()
         return (process, queue)
     else:
@@ -133,14 +154,15 @@
             test=test,
             rates=rates,
             calls=calls,
             duration=duration,
             durations=durations,
             vegeta_kwargs=vegeta_kwargs,
             verbose=verbose,
+            include_raw_output=include_raw_output,
             _pbar_kwargs=_pbar_kwargs,
         )
 
 
 def run_load_test(
     *,
     node: spec.NodeShorthand,
@@ -148,16 +170,17 @@
     rates: typing.Sequence[int] | None = None,
     calls: typing.Sequence[typing.Any] | None = None,
     duration: int | None = None,
     durations: typing.Sequence[int] | None = None,
     vegeta_kwargs: typing.Mapping[str, str | None] | None = None,
     verbose: bool | int = False,
     _pbar_kwargs: typing.Mapping[str, typing.Any] | None = None,
-    _container: multiprocessing.Queue[spec.LoadTestOutput] | None = None,
-) -> spec.LoadTestOutput:
+    _container: multiprocessing.Queue[str] | None = None,
+    include_raw_output: bool = False,
+) -> spec.LoadTestOutput | str:
     """run a load test against a single node"""
 
     # parse user_io
     node = user_io.parse_node(node)
     if test is None:
         if rates is None or calls is None:
             raise Exception('specify rates and calls')
@@ -167,66 +190,110 @@
             duration=duration,
             durations=durations,
             vegeta_kwargs=vegeta_kwargs,
         )
 
     # run tests
     if node.get('remote') is None:
-        result = _run_load_test_locally(
+        result: spec.LoadTestOutput | str = _run_load_test_locally(
             node=node,
             test=test,
             verbose=verbose,
             _pbar_kwargs=_pbar_kwargs,
+            include_raw_output=include_raw_output,
         )
     else:
         result = _run_load_test_remotely(
             node=node,
             test=test,
             verbose=verbose,
             _pbar_kwargs=_pbar_kwargs,
+            include_raw_output=include_raw_output,
         )
 
     if _container is not None:
+        if not isinstance(result, str):
+            raise Exception('_container only supportted for remote testing')
         _container.put(result)
 
     return result
 
 
 def _run_load_test_locally(
     *,
     node: spec.Node,
     test: spec.LoadTest | None,
     verbose: bool | int = False,
     _pbar_kwargs: typing.Mapping[str, typing.Any] | None = None,
+    include_raw_output: bool = False,
 ) -> spec.LoadTestOutput:
     """run a load test from local node"""
+    import datetime
+    import toolstr
+
+    if verbose:
+        dt = datetime.datetime.now()
+        if dt.microsecond >= 500_000:
+            dt = dt + datetime.timedelta(
+                microseconds=1_000_000 - dt.microsecond
+            )
+        else:
+            dt = dt - datetime.timedelta(microseconds=dt.microsecond)
+        timestamp = (
+            toolstr.add_style('\[', flood.styles['content'])
+            + toolstr.add_style(str(dt), flood.styles['metavar'])
+            + toolstr.add_style(']', flood.styles['content'])
+        )
+        toolstr.print(timestamp + ' Running load test for ' + node['name'])
 
     # construct progress bar
     if _pbar_kwargs is None:
         _pbar_kwargs = {}
     tqdm = user_io.outputs._get_tqdm()
     tqdm_kwargs = dict(
         leave=False,
         desc='samples',
         position=1,
         colour=flood.styles['content'],
-        disable=not verbose,
+        # disable=not verbose,
+        disable=True,
         **_pbar_kwargs,
     )
 
     # perform tests
     results = []
     for attack in tqdm.tqdm(test, **tqdm_kwargs):
+        if verbose:
+            dt = datetime.datetime.now()
+            if dt.microsecond >= 500_000:
+                dt = dt + datetime.timedelta(
+                    microseconds=1_000_000 - dt.microsecond
+                )
+            else:
+                dt = dt - datetime.timedelta(microseconds=dt.microsecond)
+            timestamp = (
+                toolstr.add_style('\[', flood.styles['content'])
+                + toolstr.add_style(str(dt), flood.styles['metavar'])
+                + toolstr.add_style(']', flood.styles['content'])
+            )
+            toolstr.print(
+                timestamp
+                + ' Running attack at rate = '
+                + str(attack['rate'])
+                + ' rps'
+            )
+
         result = vegeta.run_vegeta_attack(
             url=node['url'],
             calls=attack['calls'],
             duration=attack['duration'],
             rate=attack['rate'],
             vegeta_kwargs=attack['vegeta_kwargs'],
             verbose=verbose >= 2,
+            include_raw_output=include_raw_output,
         )
         results.append(result)
         if verbose >= 2:
             print()
 
     # format output
     keys = results[0].keys()
@@ -235,33 +302,33 @@
 
 def _run_load_test_remotely(
     *,
     node: spec.Node,
     test: spec.LoadTest,
     verbose: bool | int = False,
     _pbar_kwargs: typing.Mapping[str, typing.Any] | None = None,
-) -> spec.LoadTestOutput:
+    include_raw_output: bool = False,
+) -> str:
     """run a load test from local node"""
 
-    import json
     import os
     import subprocess
     import uuid
     import toolstr
 
     # parse node specification
     remote = node['remote']
     if remote is None:
         raise Exception('not a remote node')
 
     # save call data, saving methods to preserve ordering in json
     job_id = str(uuid.uuid4())
     tempdir = '/tmp/flood__' + job_id
     os.makedirs(tempdir)
-    flood.user_io.file_io._save_single_run_test(
+    flood.runners.single_runner.single_runner_io._save_single_run_test(
         test_name='',
         test=test,
         output_dir=tempdir,
     )
 
     # send call data to remote server
     if verbose:
@@ -305,22 +372,28 @@
             toolstr.add_style('\[', flood.styles['content'])
             + toolstr.add_style(str(dt), flood.styles['metavar'])
             + toolstr.add_style(']', flood.styles['content'])
         )
         toolstr.print(
             timestamp + ' ' + node_name + ' Executing test on remote node'
         )
-    cmd_template = "ssh {host} bash -c 'source ~/.profile; python3 -m flood {test} {name}={url} --output {output} --no-figures'" # noqa: E501
+    cmd_template = "ssh {host} bash -c 'source ~/.profile; python3 -m flood {test} {name}={url} --output {output} --no-figures {extra_kwargs}'"  # noqa: E501
+    if include_raw_output:
+        extra_kwargs = '--save-raw-output'
+    else:
+        extra_kwargs = ''
     cmd = cmd_template.format(
         host=remote,
         name=node['name'],
         url=node['url'],
         test=tempdir,
         output=tempdir,
+        extra_kwargs=extra_kwargs,
     )
+    cmd = cmd.strip()
     subprocess.check_output(cmd.split(' '), stderr=subprocess.DEVNULL)
 
     # retrieve benchmark results
     if verbose:
         dt = datetime.datetime.now()
         if dt.microsecond >= 500_000:
             dt = dt + datetime.timedelta(
@@ -334,11 +407,9 @@
             + toolstr.add_style(']', flood.styles['content'])
         )
         toolstr.print(timestamp + ' ' + node_name + ' Retrieving results')
     results_path = os.path.join(tempdir, 'results.json')
     cmd = 'rsync ' + remote + ':' + results_path + ' ' + results_path
     subprocess.call(cmd.split(' '), stderr=subprocess.DEVNULL)
 
-    # return results
-    with open(results_path, 'r') as f:
-        results: spec.SingleRunResultsPayload = json.load(f)
-        return results['results'][node['name']]
+    return results_path
+
```

### Comparing `paradigm-flood-0.2.3/flood/user_io/inputs.py` & `paradigm-flood-0.2.4/flood/user_io/inputs.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.3/flood/user_io/notebook_io.py` & `paradigm-flood-0.2.4/flood/user_io/notebook_io.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.3/flood/user_io/outputs.py` & `paradigm-flood-0.2.4/flood/user_io/outputs.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.3/pyproject.toml` & `paradigm-flood-0.2.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -26,23 +26,24 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Typing :: Typed",
 ]
 dependencies = [
     'typing-extensions >=4.2.0, <5',
     'toolcli >=0.6.14, <0.7',
-    'toolstr >=0.9.6, <0.10',
+    'toolstr >=0.9.7, <0.10',
     'requests >=2.20.0, <3',
     'tqdm >=4.65.0, <5',
     'numpy >=1.19.0, <1.25',
     'nbformat >= 5.8.0, <6',
     'toolplot >= 0.3.4, <0.4',
     'matplotlib >= 3.7.1, <4',
     'paradigm-data-portal >= 0.2.2, <0.3',
     'checkthechain >= 0.3.6, <0.4.0',
+    'nbconvert > 5.6.0, <6',
 ]
 
 [project.optional-dependencies]
 test = [
     'mypy ==1.2.0',
     'mypy_extensions >= 1.0.0, <1.1.0',
     'pytest >=6, <7',
```

### Comparing `paradigm-flood-0.2.3/tests/conftest.py` & `paradigm-flood-0.2.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.3/tests/test_env_vars.py` & `paradigm-flood-0.2.4/tests/test_env_vars.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.3/tests/test_load_tests.py` & `paradigm-flood-0.2.4/tests/test_load_tests.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.3/tests/test_node_parsing.py` & `paradigm-flood-0.2.4/tests/test_node_parsing.py`

 * *Files identical despite different names*

### Comparing `paradigm-flood-0.2.3/PKG-INFO` & `paradigm-flood-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paradigm-flood
-Version: 0.2.3
+Version: 0.2.4
 Summary: tool for benchmarking RPC endpoints
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Science/Research
@@ -18,23 +18,24 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Dist: typing-extensions >=4.2.0, <5
 Requires-Dist: toolcli >=0.6.14, <0.7
-Requires-Dist: toolstr >=0.9.6, <0.10
+Requires-Dist: toolstr >=0.9.7, <0.10
 Requires-Dist: requests >=2.20.0, <3
 Requires-Dist: tqdm >=4.65.0, <5
 Requires-Dist: numpy >=1.19.0, <1.25
 Requires-Dist: nbformat >= 5.8.0, <6
 Requires-Dist: toolplot >= 0.3.4, <0.4
 Requires-Dist: matplotlib >= 3.7.1, <4
 Requires-Dist: paradigm-data-portal >= 0.2.2, <0.3
 Requires-Dist: checkthechain >= 0.3.6, <0.4.0
+Requires-Dist: nbconvert > 5.6.0, <6
 Requires-Dist: mypy ==1.2.0 ; extra == "test"
 Requires-Dist: mypy_extensions >= 1.0.0, <1.1.0 ; extra == "test"
 Requires-Dist: pytest >=6, <7 ; extra == "test"
 Requires-Dist: types-tqdm >= 4.65.0.1, <5 ; extra == "test"
 Provides-Extra: test
```

