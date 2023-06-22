# Comparing `tmp/p2g-0.2.5.tar.gz` & `tmp/p2g-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p2g-0.2.5.tar", max compression
+gzip compressed data, was "p2g-0.2.6.tar", max compression
```

## Comparing `p2g-0.2.5.tar` & `p2g-0.2.6.tar`

### file list

```diff
@@ -1,85 +1,85 @@
--rwxr-xr-x   0        0        0    42500 2023-06-21 02:42:18.121336 p2g-0.2.5/README.rst
--rwxr-xr-x   0        0        0     1102 2023-06-21 10:05:40.530052 p2g-0.2.5/p2g/__init__.py
--rwxr-xr-x   0        0        0       24 2023-06-21 08:48:22.577390 p2g-0.2.5/p2g/__main__.py
--rwxr-xr-x   0        0        0      688 2023-06-19 00:17:28.273631 p2g-0.2.5/p2g/axis.py
--rwxr-xr-x   0        0        0     1215 2023-06-18 04:43:38.122521 p2g-0.2.5/p2g/builtin.py
--rwxr-xr-x   0        0        0     3357 2023-06-17 00:22:47.584219 p2g-0.2.5/p2g/coords.py
--rw-r--r--   0        0        0     4090 2023-06-19 00:15:06.786854 p2g-0.2.5/p2g/debug.py
--rwxr-xr-x   0        0        0       16 2023-06-17 00:22:47.584219 p2g-0.2.5/p2g/doc/authors.org
--rw-r--r--   0        0        0      211 2023-06-21 09:53:44.939805 p2g-0.2.5/p2g/doc/buildreadme.el
--rwxr-xr-x   0        0        0    12081 2023-06-21 10:21:12.452589 p2g-0.2.5/p2g/doc/haas.org
--rwxr-xr-x   0        0        0    16060 2023-06-21 10:21:14.096622 p2g-0.2.5/p2g/doc/haas.txt
--rw-r--r--   0        0        0     1075 2023-06-21 02:43:31.506820 p2g-0.2.5/p2g/doc/license.org
--rw-r--r--   0        0        0    33656 2023-06-21 10:21:13.628613 p2g-0.2.5/p2g/doc/readme.md
--rw-r--r--   0        0        0    33656 2023-06-21 10:21:13.648613 p2g-0.2.5/p2g/doc/readme.md.tmp
--rw-r--r--   0        0        0    33894 2023-06-21 10:16:16.954707 p2g-0.2.5/p2g/doc/readme.md~
--rwxr-xr-x   0        0        0    35449 2023-06-21 10:16:15.150672 p2g-0.2.5/p2g/doc/readme.org
--rwxr-xr-x   0        0        0     2550 2023-06-18 23:16:44.374437 p2g-0.2.5/p2g/err.py
--rwxr-xr-x   0        0        0     2732 2023-06-18 01:57:11.841792 p2g-0.2.5/p2g/examples/csearch.py
--rwxr-xr-x   0        0        0     2764 2023-06-18 03:11:37.467828 p2g-0.2.5/p2g/examples/defs.py
--rw-r--r--   0        0        0     1883 2023-06-18 04:54:07.607190 p2g-0.2.5/p2g/examples/probecalibrate.nc
--rwxr-xr-x   0        0        0     1174 2023-06-18 04:06:55.402328 p2g-0.2.5/p2g/examples/probecalibrate.py
--rw-r--r--   0        0        0    10558 2023-06-18 22:45:07.561957 p2g-0.2.5/p2g/examples/vicecenter.nc
--rwxr-xr-x   0        0        0     3942 2023-06-18 04:14:26.923355 p2g-0.2.5/p2g/examples/vicecenter.py
--rwxr-xr-x   0        0        0     1191 2023-06-18 04:16:04.897315 p2g-0.2.5/p2g/gbl.py
--rwxr-xr-x   0        0        0     5339 2023-06-18 04:17:41.923256 p2g-0.2.5/p2g/goto.py
--rw-r--r--   0        0        0     6907 2023-06-21 10:21:14.492630 p2g-0.2.5/p2g/haas.py
--rwxr-xr-x   0        0        0     3464 2023-06-21 10:05:40.530052 p2g-0.2.5/p2g/lib.py
--rwxr-xr-x   0        0        0     5598 2023-06-21 10:05:26.129765 p2g-0.2.5/p2g/main.py
--rwxr-xr-x   0        0        0    15809 2023-06-21 10:04:57.421194 p2g-0.2.5/p2g/makestdvars.py
--rwxr-xr-x   0        0        0    21488 2023-06-17 00:22:47.584219 p2g-0.2.5/p2g/mvarsorig
--rwxr-xr-x   0        0        0     1768 2023-06-18 04:50:09.654391 p2g-0.2.5/p2g/nd.py
--rwxr-xr-x   0        0        0    13462 2023-06-18 04:18:48.592590 p2g-0.2.5/p2g/op.py
--rwxr-xr-x   0        0        0      593 2023-06-21 10:05:40.562052 p2g-0.2.5/p2g/opinfo.py
--rwxr-xr-x   0        0        0     6991 2023-06-19 00:15:06.766853 p2g-0.2.5/p2g/ptest.py
--rwxr-xr-x   0        0        0     3056 2023-06-18 04:43:09.973955 p2g-0.2.5/p2g/scalar.py
--rwxr-xr-x   0        0        0     7085 2023-06-19 00:15:06.754853 p2g-0.2.5/p2g/stat.py
--rwxr-xr-x   0        0        0     2749 2023-06-18 04:14:26.855354 p2g-0.2.5/p2g/symbol.py
--rwxr-xr-x   0        0        0      194 2023-06-18 01:55:22.155594 p2g-0.2.5/p2g/tests/conftest.py
--rwxr-xr-x   0        0        0       24 2023-06-18 01:55:22.159594 p2g-0.2.5/p2g/tests/dummy.py
--rw-r--r--   0        0        0     1628 2023-06-18 04:10:24.966517 p2g-0.2.5/p2g/tests/golden/probecalibrate_probecalibrate.nc
--rw-r--r--   0        0        0      161 2023-06-21 10:03:44.567744 p2g-0.2.5/p2g/tests/golden/test_error_test_forcefail.decorator
--rw-r--r--   0        0        0        0 2023-06-21 10:03:45.071754 p2g-0.2.5/p2g/tests/golden/test_meta_test_native_gold_compare_fail.got
--rw-r--r--   0        0        0     9366 2023-06-18 04:07:32.343066 p2g-0.2.5/p2g/tests/golden/vicecenter_vicecenter.nc
--rwxr-xr-x   0        0        0      277 2023-06-18 01:55:22.159594 p2g-0.2.5/p2g/tests/not_pytest_nonlocal0.py
--rw-r--r--   0        0        0       83 2023-06-18 01:55:22.151594 p2g-0.2.5/p2g/tests/not_pytest_nonlocal1.py
--rwxr-xr-x   0        0        0      277 2023-06-18 01:55:22.131593 p2g-0.2.5/p2g/tests/not_pytest_nonlocal2.py
--rw-r--r--   0        0        0      126 2023-06-18 01:55:22.147594 p2g-0.2.5/p2g/tests/not_pytest_return.py
--rwxr-xr-x   0        0        0     2456 2023-06-18 01:55:22.147594 p2g-0.2.5/p2g/tests/test_axes.py
--rwxr-xr-x   0        0        0      535 2023-06-18 01:55:22.151594 p2g-0.2.5/p2g/tests/test_basic.py
--rwxr-xr-x   0        0        0     6290 2023-06-18 01:55:22.135593 p2g-0.2.5/p2g/tests/test_builtins.py
--rwxr-xr-x   0        0        0      331 2023-06-18 01:55:22.163594 p2g-0.2.5/p2g/tests/test_comment.py
--rwxr-xr-x   0        0        0     4071 2023-06-18 01:55:22.135593 p2g-0.2.5/p2g/tests/test_coords.py
--rw-r--r--   0        0        0       73 2023-06-18 23:49:09.560268 p2g-0.2.5/p2g/tests/test_debug.py
--rwxr-xr-x   0        0        0      419 2023-06-18 01:55:22.163594 p2g-0.2.5/p2g/tests/test_edge.py
--rwxr-xr-x   0        0        0     2866 2023-06-18 03:38:38.920293 p2g-0.2.5/p2g/tests/test_error.py
--rw-r--r--   0        0        0      550 2023-06-18 01:55:22.147594 p2g-0.2.5/p2g/tests/test_example.py
--rwxr-xr-x   0        0        0      769 2023-06-18 01:55:22.151594 p2g-0.2.5/p2g/tests/test_expr.py
--rwxr-xr-x   0        0        0     2264 2023-06-18 01:55:22.135593 p2g-0.2.5/p2g/tests/test_for.py
--rwxr-xr-x   0        0        0     4754 2023-06-18 01:55:22.131593 p2g-0.2.5/p2g/tests/test_func.py
--rwxr-xr-x   0        0        0     3402 2023-06-18 03:03:46.166348 p2g-0.2.5/p2g/tests/test_goto.py
--rwxr-xr-x   0        0        0       48 2023-06-18 01:55:22.155594 p2g-0.2.5/p2g/tests/test_gvar.py
--rwxr-xr-x   0        0        0     6728 2023-06-18 04:13:07.893775 p2g-0.2.5/p2g/tests/test_interp.py
--rwxr-xr-x   0        0        0      534 2023-06-18 01:55:22.139593 p2g-0.2.5/p2g/tests/test_linenos.py
--rwxr-xr-x   0        0        0     3690 2023-06-19 00:39:08.547261 p2g-0.2.5/p2g/tests/test_main.py
--rwxr-xr-x   0        0        0      556 2023-06-18 04:50:12.862456 p2g-0.2.5/p2g/tests/test_makestdvars.py
--rwxr-xr-x   0        0        0     2562 2023-06-18 03:40:10.694133 p2g-0.2.5/p2g/tests/test_meta.py
--rwxr-xr-x   0        0        0     1289 2023-06-18 01:55:22.151594 p2g-0.2.5/p2g/tests/test_nt1.py
--rwxr-xr-x   0        0        0     6315 2023-06-18 01:55:22.155594 p2g-0.2.5/p2g/tests/test_op.py
--rwxr-xr-x   0        0        0     8609 2023-06-18 01:55:22.159594 p2g-0.2.5/p2g/tests/test_smoke.py
--rwxr-xr-x   0        0        0     1014 2023-06-18 01:55:22.155594 p2g-0.2.5/p2g/tests/test_str.py
--rw-r--r--   0        0        0     1686 2023-06-18 01:55:22.135593 p2g-0.2.5/p2g/tests/test_symtab.py
--rwxr-xr-x   0        0        0     1206 2023-06-18 01:55:22.159594 p2g-0.2.5/p2g/tests/test_tuple.py
--rwxr-xr-x   0        0        0     4230 2023-06-18 22:48:54.014313 p2g-0.2.5/p2g/tests/test_vars.py
--rwxr-xr-x   0        0        0     9120 2023-06-18 02:46:24.501230 p2g-0.2.5/p2g/tests/test_vector.py
--rwxr-xr-x   0        0        0     1310 2023-06-17 00:22:47.584219 p2g-0.2.5/p2g/thanksto
--rwxr-xr-x   0        0        0     6466 2023-06-18 04:36:41.638150 p2g-0.2.5/p2g/vector.py
--rwxr-xr-x   0        0        0       22 2023-06-21 10:22:06.489669 p2g-0.2.5/p2g/version.py
--rwxr-xr-x   0        0        0      787 2023-06-18 04:18:25.980138 p2g-0.2.5/p2g/visible.py
--rwxr-xr-x   0        0        0    11859 2023-06-21 10:05:40.554052 p2g-0.2.5/p2g/walk.py
--rwxr-xr-x   0        0        0     3034 2023-06-18 01:57:12.521805 p2g-0.2.5/p2g/walkbase.py
--rwxr-xr-x   0        0        0     4687 2023-06-18 04:03:52.582675 p2g-0.2.5/p2g/walkexpr.py
--rwxr-xr-x   0        0        0     6373 2023-06-19 00:36:16.907866 p2g-0.2.5/p2g/walkfunc.py
--rwxr-xr-x   0        0        0     3427 2023-06-18 04:29:57.618030 p2g-0.2.5/p2g/walkns.py
--rwxr-xr-x   0        0        0     3898 2023-06-21 10:22:06.229664 p2g-0.2.5/pyproject.toml
--rw-r--r--   0        0        0    43392 1970-01-01 00:00:00.000000 p2g-0.2.5/PKG-INFO
+-rwxr-xr-x   0        0        0    42500 2023-06-21 02:42:18.121336 p2g-0.2.6/README.rst
+-rwxr-xr-x   0        0        0     1102 2023-06-21 10:05:40.530052 p2g-0.2.6/p2g/__init__.py
+-rwxr-xr-x   0        0        0       24 2023-06-21 08:48:22.577390 p2g-0.2.6/p2g/__main__.py
+-rwxr-xr-x   0        0        0      688 2023-06-19 00:17:28.273631 p2g-0.2.6/p2g/axis.py
+-rwxr-xr-x   0        0        0     1215 2023-06-18 04:43:38.122521 p2g-0.2.6/p2g/builtin.py
+-rwxr-xr-x   0        0        0     3357 2023-06-17 00:22:47.584219 p2g-0.2.6/p2g/coords.py
+-rw-r--r--   0        0        0     4090 2023-06-19 00:15:06.786854 p2g-0.2.6/p2g/debug.py
+-rwxr-xr-x   0        0        0       16 2023-06-17 00:22:47.584219 p2g-0.2.6/p2g/doc/authors.org
+-rw-r--r--   0        0        0      211 2023-06-21 09:53:44.939805 p2g-0.2.6/p2g/doc/buildreadme.el
+-rwxr-xr-x   0        0        0    12081 2023-06-21 10:21:12.452589 p2g-0.2.6/p2g/doc/haas.org
+-rwxr-xr-x   0        0        0    16060 2023-06-21 10:21:14.096622 p2g-0.2.6/p2g/doc/haas.txt
+-rw-r--r--   0        0        0     1075 2023-06-21 02:43:31.506820 p2g-0.2.6/p2g/doc/license.org
+-rw-r--r--   0        0        0    33842 2023-06-21 10:23:19.719133 p2g-0.2.6/p2g/doc/readme.md
+-rw-r--r--   0        0        0    33842 2023-06-21 10:23:19.735133 p2g-0.2.6/p2g/doc/readme.md.tmp
+-rw-r--r--   0        0        0    33894 2023-06-21 10:16:16.954707 p2g-0.2.6/p2g/doc/readme.md~
+-rwxr-xr-x   0        0        0    35277 2023-06-21 10:23:17.927097 p2g-0.2.6/p2g/doc/readme.org
+-rwxr-xr-x   0        0        0     2550 2023-06-18 23:16:44.374437 p2g-0.2.6/p2g/err.py
+-rwxr-xr-x   0        0        0     2732 2023-06-18 01:57:11.841792 p2g-0.2.6/p2g/examples/csearch.py
+-rwxr-xr-x   0        0        0     2764 2023-06-18 03:11:37.467828 p2g-0.2.6/p2g/examples/defs.py
+-rw-r--r--   0        0        0     1883 2023-06-18 04:54:07.607190 p2g-0.2.6/p2g/examples/probecalibrate.nc
+-rwxr-xr-x   0        0        0     1174 2023-06-18 04:06:55.402328 p2g-0.2.6/p2g/examples/probecalibrate.py
+-rw-r--r--   0        0        0    10558 2023-06-18 22:45:07.561957 p2g-0.2.6/p2g/examples/vicecenter.nc
+-rwxr-xr-x   0        0        0     3942 2023-06-18 04:14:26.923355 p2g-0.2.6/p2g/examples/vicecenter.py
+-rwxr-xr-x   0        0        0     1191 2023-06-18 04:16:04.897315 p2g-0.2.6/p2g/gbl.py
+-rwxr-xr-x   0        0        0     5339 2023-06-18 04:17:41.923256 p2g-0.2.6/p2g/goto.py
+-rw-r--r--   0        0        0     6907 2023-06-21 10:21:14.492630 p2g-0.2.6/p2g/haas.py
+-rwxr-xr-x   0        0        0     3464 2023-06-21 10:05:40.530052 p2g-0.2.6/p2g/lib.py
+-rwxr-xr-x   0        0        0     5598 2023-06-21 10:05:26.129765 p2g-0.2.6/p2g/main.py
+-rwxr-xr-x   0        0        0    15809 2023-06-21 10:04:57.421194 p2g-0.2.6/p2g/makestdvars.py
+-rwxr-xr-x   0        0        0    21488 2023-06-17 00:22:47.584219 p2g-0.2.6/p2g/mvarsorig
+-rwxr-xr-x   0        0        0     1768 2023-06-18 04:50:09.654391 p2g-0.2.6/p2g/nd.py
+-rwxr-xr-x   0        0        0    13462 2023-06-18 04:18:48.592590 p2g-0.2.6/p2g/op.py
+-rwxr-xr-x   0        0        0      593 2023-06-21 10:05:40.562052 p2g-0.2.6/p2g/opinfo.py
+-rwxr-xr-x   0        0        0     6991 2023-06-19 00:15:06.766853 p2g-0.2.6/p2g/ptest.py
+-rwxr-xr-x   0        0        0     3056 2023-06-18 04:43:09.973955 p2g-0.2.6/p2g/scalar.py
+-rwxr-xr-x   0        0        0     7085 2023-06-19 00:15:06.754853 p2g-0.2.6/p2g/stat.py
+-rwxr-xr-x   0        0        0     2749 2023-06-18 04:14:26.855354 p2g-0.2.6/p2g/symbol.py
+-rwxr-xr-x   0        0        0      194 2023-06-18 01:55:22.155594 p2g-0.2.6/p2g/tests/conftest.py
+-rwxr-xr-x   0        0        0       24 2023-06-18 01:55:22.159594 p2g-0.2.6/p2g/tests/dummy.py
+-rw-r--r--   0        0        0     1628 2023-06-18 04:10:24.966517 p2g-0.2.6/p2g/tests/golden/probecalibrate_probecalibrate.nc
+-rw-r--r--   0        0        0      161 2023-06-21 10:03:44.567744 p2g-0.2.6/p2g/tests/golden/test_error_test_forcefail.decorator
+-rw-r--r--   0        0        0        0 2023-06-21 10:03:45.071754 p2g-0.2.6/p2g/tests/golden/test_meta_test_native_gold_compare_fail.got
+-rw-r--r--   0        0        0     9366 2023-06-18 04:07:32.343066 p2g-0.2.6/p2g/tests/golden/vicecenter_vicecenter.nc
+-rwxr-xr-x   0        0        0      277 2023-06-18 01:55:22.159594 p2g-0.2.6/p2g/tests/not_pytest_nonlocal0.py
+-rw-r--r--   0        0        0       83 2023-06-18 01:55:22.151594 p2g-0.2.6/p2g/tests/not_pytest_nonlocal1.py
+-rwxr-xr-x   0        0        0      277 2023-06-18 01:55:22.131593 p2g-0.2.6/p2g/tests/not_pytest_nonlocal2.py
+-rw-r--r--   0        0        0      126 2023-06-18 01:55:22.147594 p2g-0.2.6/p2g/tests/not_pytest_return.py
+-rwxr-xr-x   0        0        0     2456 2023-06-18 01:55:22.147594 p2g-0.2.6/p2g/tests/test_axes.py
+-rwxr-xr-x   0        0        0      535 2023-06-18 01:55:22.151594 p2g-0.2.6/p2g/tests/test_basic.py
+-rwxr-xr-x   0        0        0     6290 2023-06-18 01:55:22.135593 p2g-0.2.6/p2g/tests/test_builtins.py
+-rwxr-xr-x   0        0        0      331 2023-06-18 01:55:22.163594 p2g-0.2.6/p2g/tests/test_comment.py
+-rwxr-xr-x   0        0        0     4071 2023-06-18 01:55:22.135593 p2g-0.2.6/p2g/tests/test_coords.py
+-rw-r--r--   0        0        0       73 2023-06-18 23:49:09.560268 p2g-0.2.6/p2g/tests/test_debug.py
+-rwxr-xr-x   0        0        0      419 2023-06-18 01:55:22.163594 p2g-0.2.6/p2g/tests/test_edge.py
+-rwxr-xr-x   0        0        0     2866 2023-06-18 03:38:38.920293 p2g-0.2.6/p2g/tests/test_error.py
+-rw-r--r--   0        0        0      550 2023-06-18 01:55:22.147594 p2g-0.2.6/p2g/tests/test_example.py
+-rwxr-xr-x   0        0        0      769 2023-06-18 01:55:22.151594 p2g-0.2.6/p2g/tests/test_expr.py
+-rwxr-xr-x   0        0        0     2264 2023-06-18 01:55:22.135593 p2g-0.2.6/p2g/tests/test_for.py
+-rwxr-xr-x   0        0        0     4754 2023-06-18 01:55:22.131593 p2g-0.2.6/p2g/tests/test_func.py
+-rwxr-xr-x   0        0        0     3402 2023-06-18 03:03:46.166348 p2g-0.2.6/p2g/tests/test_goto.py
+-rwxr-xr-x   0        0        0       48 2023-06-18 01:55:22.155594 p2g-0.2.6/p2g/tests/test_gvar.py
+-rwxr-xr-x   0        0        0     6728 2023-06-18 04:13:07.893775 p2g-0.2.6/p2g/tests/test_interp.py
+-rwxr-xr-x   0        0        0      534 2023-06-18 01:55:22.139593 p2g-0.2.6/p2g/tests/test_linenos.py
+-rwxr-xr-x   0        0        0     3690 2023-06-19 00:39:08.547261 p2g-0.2.6/p2g/tests/test_main.py
+-rwxr-xr-x   0        0        0      556 2023-06-18 04:50:12.862456 p2g-0.2.6/p2g/tests/test_makestdvars.py
+-rwxr-xr-x   0        0        0     2562 2023-06-18 03:40:10.694133 p2g-0.2.6/p2g/tests/test_meta.py
+-rwxr-xr-x   0        0        0     1289 2023-06-18 01:55:22.151594 p2g-0.2.6/p2g/tests/test_nt1.py
+-rwxr-xr-x   0        0        0     6315 2023-06-18 01:55:22.155594 p2g-0.2.6/p2g/tests/test_op.py
+-rwxr-xr-x   0        0        0     8609 2023-06-18 01:55:22.159594 p2g-0.2.6/p2g/tests/test_smoke.py
+-rwxr-xr-x   0        0        0     1014 2023-06-18 01:55:22.155594 p2g-0.2.6/p2g/tests/test_str.py
+-rw-r--r--   0        0        0     1686 2023-06-18 01:55:22.135593 p2g-0.2.6/p2g/tests/test_symtab.py
+-rwxr-xr-x   0        0        0     1206 2023-06-18 01:55:22.159594 p2g-0.2.6/p2g/tests/test_tuple.py
+-rwxr-xr-x   0        0        0     4230 2023-06-18 22:48:54.014313 p2g-0.2.6/p2g/tests/test_vars.py
+-rwxr-xr-x   0        0        0     9120 2023-06-18 02:46:24.501230 p2g-0.2.6/p2g/tests/test_vector.py
+-rwxr-xr-x   0        0        0     1310 2023-06-17 00:22:47.584219 p2g-0.2.6/p2g/thanksto
+-rwxr-xr-x   0        0        0     6466 2023-06-18 04:36:41.638150 p2g-0.2.6/p2g/vector.py
+-rwxr-xr-x   0        0        0       22 2023-06-22 01:20:27.827803 p2g-0.2.6/p2g/version.py
+-rwxr-xr-x   0        0        0      787 2023-06-18 04:18:25.980138 p2g-0.2.6/p2g/visible.py
+-rwxr-xr-x   0        0        0    11859 2023-06-21 10:05:40.554052 p2g-0.2.6/p2g/walk.py
+-rwxr-xr-x   0        0        0     3034 2023-06-18 01:57:12.521805 p2g-0.2.6/p2g/walkbase.py
+-rwxr-xr-x   0        0        0     4687 2023-06-18 04:03:52.582675 p2g-0.2.6/p2g/walkexpr.py
+-rwxr-xr-x   0        0        0     6373 2023-06-19 00:36:16.907866 p2g-0.2.6/p2g/walkfunc.py
+-rwxr-xr-x   0        0        0     3427 2023-06-18 04:29:57.618030 p2g-0.2.6/p2g/walkns.py
+-rwxr-xr-x   0        0        0     3898 2023-06-22 01:20:27.567797 p2g-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0    43392 1970-01-01 00:00:00.000000 p2g-0.2.6/PKG-INFO
```

### Comparing `p2g-0.2.5/README.rst` & `p2g-0.2.6/README.rst`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/__init__.py` & `p2g-0.2.6/p2g/__init__.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/axis.py` & `p2g-0.2.6/p2g/axis.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/builtin.py` & `p2g-0.2.6/p2g/builtin.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/coords.py` & `p2g-0.2.6/p2g/coords.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/debug.py` & `p2g-0.2.6/p2g/debug.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/doc/haas.org` & `p2g-0.2.6/p2g/doc/haas.org`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/doc/haas.txt` & `p2g-0.2.6/p2g/doc/haas.txt`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/doc/license.org` & `p2g-0.2.6/p2g/doc/license.org`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/doc/readme.md` & `p2g-0.2.6/p2g/doc/readme.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![img](https://img.shields.io/badge/License-MIT%20v3-blue.svg)][<https://img.shields.io/pypi/v/manimgl?logo=pypi>)]
+[![img](https://img.shields.io/badge/License-MIT%20v3-blue.svg)]
 
 
 # p2g - Python 2 G-code
 
 
 ## Introduction
 
@@ -65,39 +65,39 @@
 from p2g.haas import *
 
 fast_go = goto.feed(640)
 fast_probe = goto.probe.feed(30)
 
 class SearchParams:
     def __init__(self, name, search_depth, iota, delta):
-	self.name = name
-	self.its = 10
-	self.search_depth = search_depth
-	self.iota = iota
-	self.delta = delta
-	self.probe = goto.probe.feed(30)
-	self.go = goto.feed(640)
+        self.name = name
+        self.its = 10
+        self.search_depth = search_depth
+        self.iota = iota
+        self.delta = delta
+        self.probe = goto.probe.feed(30)
+        self.go = goto.feed(640)
 
 def search(cursor, sch):
     # stick from class SearchParams  iterations into macro var
     its = Var(sch.its)
     while its > 0:
-	# goto start point
-	sch.go(cursor)
-	# down until hit - or not.
-	sch.probe(z=sch.search_depth)
-	# if probe is below (+some slack) hit
-	# point, then done.
-	if SKIP_POS.z < sch.search_depth + sch.iota:
-	    break
-	# otherwise move to next point
-	cursor.xy += sch.delta
-	its -= 1
+        # goto start point
+        sch.go(cursor)
+        # down until hit - or not.
+        sch.probe(z=sch.search_depth)
+        # if probe is below (+some slack) hit
+        # point, then done.
+        if SKIP_POS.z < sch.search_depth + sch.iota:
+            break
+        # otherwise move to next point
+        cursor.xy += sch.delta
+        its -= 1
     else:
-	message(ALARM, f"too far {sch.name}.")
+        message(ALARM, f"too far {sch.name}.")
 
 def demo1():
     cursor = Var[3](2, 3, 4)
     # searching right, look down 0.4", move
     # 1.5" right if nothing hit.
     sch1 = SearchParams(name="right", search_depth=-0.4, iota=-0.1, delta=(1.5, 0))
     search(cursor, sch1)
@@ -278,15 +278,15 @@
 
 
     a,b,x = Var(),Var(),Var()
     a = tlhc[0] / tlhc[1]
     b = tlhc[0] % tlhc[1]
     x = tlhc[0] & tlhc[1]        
     tlhc.xy = ((a - b + 3) / sin(x),
-	       (a + b + 3) / cos(x))
+               (a + b + 3) / cos(x))
 
 
 
 
 ```
 
 ⇨ `p2g gen exp1.py` ⇨
@@ -334,15 +334,15 @@
 def a5():
    p2g.axis.NAMES = 'xyza*c'
    p2g.com ("rhs of vector ops get expanded as needed")
    G55.var = [0,1]
    p2g.com ("fill yz and c with some stuff")
    tmp1 = Const(y=3, z=9, c=p2g.asin(.5))
    p2g.com ("Unmentioned axes values are assumed",
-	    "to be 0, so adding them makes no code.")
+            "to be 0, so adding them makes no code.")
    G55.var += tmp1
    p2g.com ("")
    G55.ac *= 2.0
 
 
 def a3():
    # xyz is the default.
@@ -517,15 +517,15 @@
     p1.xy_then_z(v1)
 
     comment ("p2 is whatever p1 was, with changed to a probe.")
     p2 = p1.probe
     p2.xy_then_z(v1)
 
     comment ("p3 is whatever p1 was, with a probe and relative,",
-	     "using only the x and y axes")
+             "using only the x and y axes")
     p3 = p1.relative.probe
     p3.xy_then_z(v1.xy)
 
     comment ("move a and c axes ")
     axis.NAMES = 'xyza*c'
     goto.feed(20) (a=9, c= 90)
 
@@ -598,20 +598,20 @@
 
 ```python
 
 from p2g import *
 from p2g.haas import *
 
 class X():
-	 def __init__(self, a,b):
-	       self.a = a
-	       self.b = b
-	 def adjust(self, tof):
-	       self.a += tof.x
-	       self.b += tof.y
+         def __init__(self, a,b):
+               self.a = a
+               self.b = b
+         def adjust(self, tof):
+               self.a += tof.x
+               self.b += tof.y
 
 def cool():
       com ("You can do surprising things.")
       p = X(12,34)
 
       p.adjust(TOOL_OFFSET)
       tmp = Var(p.a, p.b)
@@ -627,26 +627,26 @@
 from p2g import *
 from p2g.haas import *
 
 G55 = p2g.Fixed[3](addr=5241)
 
 def beware():
     com(
-	"Names on the left hand side of an assignment need to be",
-	"treated with care.  A simple.",
+        "Names on the left hand side of an assignment need to be",
+        "treated with care.  A simple.",
     )
     G55 = [0, 0, 0]
     com(
-	"Will not do what you want - this will overwrite the definition",
-	"of G55 above - so no code will be generated.",
+        "Will not do what you want - this will overwrite the definition",
+        "of G55 above - so no code will be generated.",
     )
 
     com(
-	"You need to use .var (for everything), explicitly name the axes,"
-	"or use magic slicing."
+        "You need to use .var (for everything), explicitly name the axes,"
+        "or use magic slicing."
     )
 
     G56.var = [1, 1, 1]
     G56.xyz = [2, 2, 2]
     G56[:] = [3, 3, 3]
```

### Comparing `p2g-0.2.5/p2g/doc/readme.md.tmp` & `p2g-0.2.6/p2g/doc/readme.md.tmp`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![img](https://img.shields.io/badge/License-MIT%20v3-blue.svg)][<https://img.shields.io/pypi/v/manimgl?logo=pypi>)]
+[![img](https://img.shields.io/badge/License-MIT%20v3-blue.svg)]
 
 
 # p2g - Python 2 G-code
 
 
 ## Introduction
 
@@ -65,39 +65,39 @@
 from p2g.haas import *
 
 fast_go = goto.feed(640)
 fast_probe = goto.probe.feed(30)
 
 class SearchParams:
     def __init__(self, name, search_depth, iota, delta):
-	self.name = name
-	self.its = 10
-	self.search_depth = search_depth
-	self.iota = iota
-	self.delta = delta
-	self.probe = goto.probe.feed(30)
-	self.go = goto.feed(640)
+        self.name = name
+        self.its = 10
+        self.search_depth = search_depth
+        self.iota = iota
+        self.delta = delta
+        self.probe = goto.probe.feed(30)
+        self.go = goto.feed(640)
 
 def search(cursor, sch):
     # stick from class SearchParams  iterations into macro var
     its = Var(sch.its)
     while its > 0:
-	# goto start point
-	sch.go(cursor)
-	# down until hit - or not.
-	sch.probe(z=sch.search_depth)
-	# if probe is below (+some slack) hit
-	# point, then done.
-	if SKIP_POS.z < sch.search_depth + sch.iota:
-	    break
-	# otherwise move to next point
-	cursor.xy += sch.delta
-	its -= 1
+        # goto start point
+        sch.go(cursor)
+        # down until hit - or not.
+        sch.probe(z=sch.search_depth)
+        # if probe is below (+some slack) hit
+        # point, then done.
+        if SKIP_POS.z < sch.search_depth + sch.iota:
+            break
+        # otherwise move to next point
+        cursor.xy += sch.delta
+        its -= 1
     else:
-	message(ALARM, f"too far {sch.name}.")
+        message(ALARM, f"too far {sch.name}.")
 
 def demo1():
     cursor = Var[3](2, 3, 4)
     # searching right, look down 0.4", move
     # 1.5" right if nothing hit.
     sch1 = SearchParams(name="right", search_depth=-0.4, iota=-0.1, delta=(1.5, 0))
     search(cursor, sch1)
@@ -278,15 +278,15 @@
 
 
     a,b,x = Var(),Var(),Var()
     a = tlhc[0] / tlhc[1]
     b = tlhc[0] % tlhc[1]
     x = tlhc[0] & tlhc[1]        
     tlhc.xy = ((a - b + 3) / sin(x),
-	       (a + b + 3) / cos(x))
+               (a + b + 3) / cos(x))
 
 
 
 
 ```
 
 ⇨ `p2g gen exp1.py` ⇨
@@ -334,15 +334,15 @@
 def a5():
    p2g.axis.NAMES = 'xyza*c'
    p2g.com ("rhs of vector ops get expanded as needed")
    G55.var = [0,1]
    p2g.com ("fill yz and c with some stuff")
    tmp1 = Const(y=3, z=9, c=p2g.asin(.5))
    p2g.com ("Unmentioned axes values are assumed",
-	    "to be 0, so adding them makes no code.")
+            "to be 0, so adding them makes no code.")
    G55.var += tmp1
    p2g.com ("")
    G55.ac *= 2.0
 
 
 def a3():
    # xyz is the default.
@@ -517,15 +517,15 @@
     p1.xy_then_z(v1)
 
     comment ("p2 is whatever p1 was, with changed to a probe.")
     p2 = p1.probe
     p2.xy_then_z(v1)
 
     comment ("p3 is whatever p1 was, with a probe and relative,",
-	     "using only the x and y axes")
+             "using only the x and y axes")
     p3 = p1.relative.probe
     p3.xy_then_z(v1.xy)
 
     comment ("move a and c axes ")
     axis.NAMES = 'xyza*c'
     goto.feed(20) (a=9, c= 90)
 
@@ -598,20 +598,20 @@
 
 ```python
 
 from p2g import *
 from p2g.haas import *
 
 class X():
-	 def __init__(self, a,b):
-	       self.a = a
-	       self.b = b
-	 def adjust(self, tof):
-	       self.a += tof.x
-	       self.b += tof.y
+         def __init__(self, a,b):
+               self.a = a
+               self.b = b
+         def adjust(self, tof):
+               self.a += tof.x
+               self.b += tof.y
 
 def cool():
       com ("You can do surprising things.")
       p = X(12,34)
 
       p.adjust(TOOL_OFFSET)
       tmp = Var(p.a, p.b)
@@ -627,21 +627,25 @@
 from p2g import *
 from p2g.haas import *
 
 G55 = p2g.Fixed[3](addr=5241)
 
 def beware():
     com(
-	"Names on the left hand side of an assignment need to be",
-	"treated with care.  A simple.",
+        "Names on the left hand side of an assignment need to be",
+        "treated with care.  A simple.",
     )
     G55 = [0, 0, 0]
     com(
-	"Will not do what you want - this will overwrite the definition",
-	"of G55 above - so[![img](https://img.shields.io/badge/License-MIT%20v3-blue.svg)][<https://img.shields.io/pypi/v/manimgl?logo=pypi>)"or use magic slicing."
+        "Will not do what you want - this will overwrite the definition",
+        "of G55 above - so no code will be generated.",
+    )
+
+    com(
+        "You need t[![img](https://img.shields.io/badge/License-MIT%20v3-blue.svg)]"or use magic slicing."
     )
 
     G56.var = [1, 1, 1]
     G56.xyz = [2, 2, 2]
     G56[:] = [3, 3, 3]
```

### Comparing `p2g-0.2.5/p2g/doc/readme.md~` & `p2g-0.2.6/p2g/doc/readme.md~`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/doc/readme.org` & `p2g-0.2.6/p2g/doc/readme.org`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 #+OPTIONS: toc:nil
 #+OPTIONS: ^:{}
 #+TITLE: p2g - Python 2 G-code
 #+AUTHOR: sac@0x5ac.com
 
 
 
-#+macro: melpa [[https://melpa.org/#/ox-hugo][file:https://melpa.org/packages/ox-hugo-badge.svg]]
 #+macro: MIT  [https://img.shields.io/badge/License-MIT%20v3-blue.svg]
-#+macro: FISH [https://img.shields.io/pypi/v/manimgl?logo=pypi)]
-{{{MIT}}}{{{FISH}}}
+
+{{{MIT}}}
 * p2g - Python 2 G-code
 ** Introduction
 Many styli died to bring us this information.
 
 This project makes it simpl(er) to ensure that
 parts are in fixtures correctly, coordinate systems are
 adjusted to deal with stock placement and cope with
```

### Comparing `p2g-0.2.5/p2g/err.py` & `p2g-0.2.6/p2g/err.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/examples/csearch.py` & `p2g-0.2.6/p2g/examples/csearch.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/examples/defs.py` & `p2g-0.2.6/p2g/examples/defs.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/examples/probecalibrate.nc` & `p2g-0.2.6/p2g/examples/probecalibrate.nc`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/examples/probecalibrate.py` & `p2g-0.2.6/p2g/examples/probecalibrate.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/examples/vicecenter.nc` & `p2g-0.2.6/p2g/examples/vicecenter.nc`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/examples/vicecenter.py` & `p2g-0.2.6/p2g/examples/vicecenter.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/gbl.py` & `p2g-0.2.6/p2g/gbl.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/goto.py` & `p2g-0.2.6/p2g/goto.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/haas.py` & `p2g-0.2.6/p2g/haas.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/lib.py` & `p2g-0.2.6/p2g/lib.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/main.py` & `p2g-0.2.6/p2g/main.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/makestdvars.py` & `p2g-0.2.6/p2g/makestdvars.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/mvarsorig` & `p2g-0.2.6/p2g/mvarsorig`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/nd.py` & `p2g-0.2.6/p2g/nd.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/op.py` & `p2g-0.2.6/p2g/op.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/opinfo.py` & `p2g-0.2.6/p2g/opinfo.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/ptest.py` & `p2g-0.2.6/p2g/ptest.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/scalar.py` & `p2g-0.2.6/p2g/scalar.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/stat.py` & `p2g-0.2.6/p2g/stat.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/symbol.py` & `p2g-0.2.6/p2g/symbol.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/tests/golden/probecalibrate_probecalibrate.nc` & `p2g-0.2.6/p2g/tests/golden/probecalibrate_probecalibrate.nc`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/tests/golden/vicecenter_vicecenter.nc` & `p2g-0.2.6/p2g/tests/golden/vicecenter_vicecenter.nc`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/tests/test_axes.py` & `p2g-0.2.6/p2g/tests/test_axes.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/tests/test_basic.py` & `p2g-0.2.6/p2g/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/tests/test_builtins.py` & `p2g-0.2.6/p2g/tests/test_builtins.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/tests/test_coords.py` & `p2g-0.2.6/p2g/tests/test_coords.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/tests/test_error.py` & `p2g-0.2.6/p2g/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/tests/test_example.py` & `p2g-0.2.6/p2g/tests/test_example.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/tests/test_expr.py` & `p2g-0.2.6/p2g/tests/test_expr.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/tests/test_for.py` & `p2g-0.2.6/p2g/tests/test_for.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/tests/test_func.py` & `p2g-0.2.6/p2g/tests/test_func.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/tests/test_goto.py` & `p2g-0.2.6/p2g/tests/test_goto.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/tests/test_interp.py` & `p2g-0.2.6/p2g/tests/test_interp.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/tests/test_linenos.py` & `p2g-0.2.6/p2g/tests/test_linenos.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/tests/test_main.py` & `p2g-0.2.6/p2g/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/tests/test_makestdvars.py` & `p2g-0.2.6/p2g/tests/test_makestdvars.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/tests/test_meta.py` & `p2g-0.2.6/p2g/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/tests/test_nt1.py` & `p2g-0.2.6/p2g/tests/test_nt1.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/tests/test_op.py` & `p2g-0.2.6/p2g/tests/test_op.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/tests/test_smoke.py` & `p2g-0.2.6/p2g/tests/test_smoke.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/tests/test_str.py` & `p2g-0.2.6/p2g/tests/test_str.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/tests/test_symtab.py` & `p2g-0.2.6/p2g/tests/test_symtab.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/tests/test_tuple.py` & `p2g-0.2.6/p2g/tests/test_tuple.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/tests/test_vars.py` & `p2g-0.2.6/p2g/tests/test_vars.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/tests/test_vector.py` & `p2g-0.2.6/p2g/tests/test_vector.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/thanksto` & `p2g-0.2.6/p2g/thanksto`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/vector.py` & `p2g-0.2.6/p2g/vector.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/visible.py` & `p2g-0.2.6/p2g/visible.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/walk.py` & `p2g-0.2.6/p2g/walk.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/walkbase.py` & `p2g-0.2.6/p2g/walkbase.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/walkexpr.py` & `p2g-0.2.6/p2g/walkexpr.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/walkfunc.py` & `p2g-0.2.6/p2g/walkfunc.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/p2g/walkns.py` & `p2g-0.2.6/p2g/walkns.py`

 * *Files identical despite different names*

### Comparing `p2g-0.2.5/pyproject.toml` & `p2g-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 
 
 
 name = "p2g"
-version = "0.2.5"
+version = "0.2.6"
 description = "Transpile python into cnc gcode."
 authors = ["sac <sac@0x5ac.com>"]
 readme = "README.rst"
 license = "MIT"
 keywords = ["cnc", "gcode", "mill", "haas"]
 classifiers = [
 "Development Status :: 3 - Alpha",
```

### Comparing `p2g-0.2.5/PKG-INFO` & `p2g-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p2g
-Version: 0.2.5
+Version: 0.2.6
 Summary: Transpile python into cnc gcode.
 Home-page: https://github.com/0x5ac/p2g
 License: MIT
 Keywords: cnc,gcode,mill,haas
 Author: sac
 Author-email: sac@0x5ac.com
 Requires-Python: >=3.10,<4.0
```

