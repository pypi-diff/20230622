# Comparing `tmp/glow-0.11.3.tar.gz` & `tmp/glow-0.12.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glow-0.11.3.tar", last modified: Sat Dec 18 18:42:24 2021, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `glow-0.11.3.tar` & `glow-0.12.7.tar`

### file list

```diff
@@ -1,104 +1,86 @@
-drwxrwxrwx   0        0        0        0 2021-12-18 18:42:24.483320 glow-0.11.3/
--rw-rw-rw-   0        0        0       25 2021-10-01 18:46:08.000000 glow-0.11.3/.coveragerc
--rw-rw-rw-   0        0        0      136 2020-02-22 10:35:07.000000 glow-0.11.3/.editorconfig
--rw-rw-rw-   0        0        0      162 2021-10-01 18:46:08.000000 glow-0.11.3/.gitignore
--rw-rw-rw-   0        0        0     1071 2020-02-22 10:35:07.000000 glow-0.11.3/LICENSE
--rw-rw-rw-   0        0        0     2746 2021-12-18 18:42:24.483320 glow-0.11.3/PKG-INFO
--rw-rw-rw-   0        0        0     1873 2021-12-18 18:38:01.000000 glow-0.11.3/README.md
--rw-rw-rw-   0        0        0     2307 2021-10-01 18:46:08.000000 glow-0.11.3/TODO.md
-drwxrwxrwx   0        0        0        0 2021-12-18 18:42:24.409320 glow-0.11.3/glow/
--rw-rw-rw-   0        0        0      158 2021-10-01 18:46:08.000000 glow-0.11.3/glow/__init__.py
-drwxrwxrwx   0        0        0        0 2021-12-18 18:42:24.416319 glow-0.11.3/glow/api/
--rw-rw-rw-   0        0        0      149 2021-10-01 18:46:08.000000 glow-0.11.3/glow/api/__init__.py
--rw-rw-rw-   0        0        0     1009 2021-10-06 12:12:06.000000 glow-0.11.3/glow/api/config.py
--rw-rw-rw-   0        0        0     1908 2021-10-14 10:55:54.000000 glow-0.11.3/glow/api/exporting.py
--rw-rw-rw-   0        0        0     6349 2021-12-18 18:38:01.000000 glow-0.11.3/glow/cli.py
--rw-rw-rw-   0        0        0     1277 2021-12-18 18:38:01.000000 glow-0.11.3/glow/cli.pyi
-drwxrwxrwx   0        0        0        0 2021-12-18 18:42:24.428319 glow-0.11.3/glow/core/
--rw-rw-rw-   0        0        0     1077 2021-11-30 12:29:53.000000 glow-0.11.3/glow/core/__init__.py
--rw-rw-rw-   0        0        0     2280 2021-12-18 18:38:01.000000 glow-0.11.3/glow/core/_import_hook.py
--rw-rw-rw-   0        0        0     4776 2021-12-18 18:38:01.000000 glow-0.11.3/glow/core/_len_helpers.py
--rw-rw-rw-   0        0        0     3846 2021-12-18 18:38:01.000000 glow-0.11.3/glow/core/_more.py
--rw-rw-rw-   0        0        0    11080 2021-12-18 18:38:01.000000 glow-0.11.3/glow/core/_parallel.py
--rw-rw-rw-   0        0        0     2944 2021-10-06 12:11:55.000000 glow-0.11.3/glow/core/_patch_len.py
--rw-rw-rw-   0        0        0     1008 2021-08-01 20:27:56.000000 glow-0.11.3/glow/core/_patch_print.py
--rw-rw-rw-   0        0        0     2192 2021-12-18 18:38:01.000000 glow-0.11.3/glow/core/_patch_scipy.py
--rw-rw-rw-   0        0        0     4425 2021-12-18 18:38:01.000000 glow-0.11.3/glow/core/_profile.py
--rw-rw-rw-   0        0        0      537 2021-12-18 18:38:01.000000 glow-0.11.3/glow/core/_profile.pyi
--rw-rw-rw-   0        0        0     4735 2021-12-18 18:38:01.000000 glow-0.11.3/glow/core/_reduction.py
--rw-rw-rw-   0        0        0     3541 2021-12-18 18:38:01.000000 glow-0.11.3/glow/core/_repr.py
--rw-rw-rw-   0        0        0     3616 2021-10-06 12:09:57.000000 glow-0.11.3/glow/core/_sizeof.py
--rw-rw-rw-   0        0        0     2942 2021-10-14 17:40:02.000000 glow-0.11.3/glow/core/_uuid.py
--rw-rw-rw-   0        0        0     4949 2021-12-18 18:38:01.000000 glow-0.11.3/glow/core/debug.py
-drwxrwxrwx   0        0        0        0 2021-12-18 18:42:24.432321 glow-0.11.3/glow/core/wrap/
--rw-rw-rw-   0        0        0      241 2021-10-06 12:10:15.000000 glow-0.11.3/glow/core/wrap/__init__.py
--rw-rw-rw-   0        0        0     9330 2021-12-18 18:38:01.000000 glow-0.11.3/glow/core/wrap/cache.py
--rw-rw-rw-   0        0        0      601 2021-10-06 12:10:12.000000 glow-0.11.3/glow/core/wrap/cache.pyi
--rw-rw-rw-   0        0        0     4314 2021-12-18 18:38:01.000000 glow-0.11.3/glow/core/wrap/concurrency.py
--rw-rw-rw-   0        0        0      867 2021-10-06 12:10:12.000000 glow-0.11.3/glow/core/wrap/concurrency.pyi
--rw-rw-rw-   0        0        0     2198 2021-12-18 18:38:01.000000 glow-0.11.3/glow/core/wrap/reusable.py
-drwxrwxrwx   0        0        0        0 2021-12-18 18:42:24.434319 glow-0.11.3/glow/cv/
--rw-rw-rw-   0        0        0       50 2021-08-01 20:26:26.000000 glow-0.11.3/glow/cv/__init__.py
--rw-rw-rw-   0        0        0    11316 2021-12-18 18:38:01.000000 glow-0.11.3/glow/cv/_mosaic.py
--rw-rw-rw-   0        0        0     4516 2021-12-18 18:38:01.000000 glow-0.11.3/glow/distributed.py
-drwxrwxrwx   0        0        0        0 2021-12-18 18:42:24.436321 glow-0.11.3/glow/examples/
--rw-rw-rw-   0        0        0        0 2020-02-22 10:35:07.000000 glow-0.11.3/glow/examples/__init__.py
--rw-rw-rw-   0        0        0     4873 2021-12-18 18:38:01.000000 glow-0.11.3/glow/examples/cifar10.py
--rw-rw-rw-   0        0        0      463 2020-02-22 10:35:07.000000 glow-0.11.3/glow/examples/gan.py
-drwxrwxrwx   0        0        0        0 2021-12-18 18:42:24.439320 glow-0.11.3/glow/io/
--rw-rw-rw-   0        0        0      111 2021-12-18 18:38:01.000000 glow-0.11.3/glow/io/__init__.py
--rw-rw-rw-   0        0        0     3074 2021-12-18 18:38:01.000000 glow-0.11.3/glow/io/_sound.py
--rw-rw-rw-   0        0        0     3308 2021-10-14 11:03:56.000000 glow-0.11.3/glow/io/_svg.py
--rw-rw-rw-   0        0        0    18605 2021-12-18 18:38:01.000000 glow-0.11.3/glow/io/_tiled.py
-drwxrwxrwx   0        0        0        0 2021-12-18 18:42:24.442319 glow-0.11.3/glow/metrics/
--rw-rw-rw-   0        0        0      539 2021-10-06 12:13:52.000000 glow-0.11.3/glow/metrics/__init__.py
--rw-rw-rw-   0        0        0     3524 2021-10-07 10:48:26.000000 glow-0.11.3/glow/metrics/base.py
--rw-rw-rw-   0        0        0     1801 2021-10-06 12:20:46.000000 glow-0.11.3/glow/metrics/confusion.py
--rw-rw-rw-   0        0        0     2139 2021-12-18 18:38:01.000000 glow-0.11.3/glow/metrics/raw.py
-drwxrwxrwx   0        0        0        0 2021-12-18 18:42:24.453319 glow-0.11.3/glow/nn/
--rw-rw-rw-   0        0        0      761 2021-12-18 18:38:01.000000 glow-0.11.3/glow/nn/__init__.py
--rw-rw-rw-   0        0        0     8889 2021-12-18 18:35:24.000000 glow-0.11.3/glow/nn/_loader.py
--rw-rw-rw-   0        0        0     1691 2021-12-18 18:38:01.000000 glow-0.11.3/glow/nn/_stepper.py
--rw-rw-rw-   0        0        0     7246 2021-12-18 18:38:01.000000 glow-0.11.3/glow/nn/amp.py
--rw-rw-rw-   0        0        0      837 2021-10-06 12:19:53.000000 glow-0.11.3/glow/nn/amp.pyi
--rw-rw-rw-   0        0        0     3102 2021-10-06 12:16:19.000000 glow-0.11.3/glow/nn/auto.py
--rw-rw-rw-   0        0        0     1116 2021-10-06 12:17:39.000000 glow-0.11.3/glow/nn/driver.py
--rw-rw-rw-   0        0        0     9371 2021-10-06 12:20:10.000000 glow-0.11.3/glow/nn/modules.py
--rw-rw-rw-   0        0        0     1673 2021-10-06 12:16:19.000000 glow-0.11.3/glow/nn/modules_extra.py
--rw-rw-rw-   0        0        0     5570 2021-10-06 12:17:15.000000 glow-0.11.3/glow/nn/modules_factory.py
--rw-rw-rw-   0        0        0     6975 2021-12-18 18:38:01.000000 glow-0.11.3/glow/nn/optimizers.py
--rw-rw-rw-   0        0        0     6715 2021-12-18 18:38:01.000000 glow-0.11.3/glow/nn/plot.py
--rw-rw-rw-   0        0        0     1412 2021-10-06 12:21:06.000000 glow-0.11.3/glow/nn/proto.py
--rw-rw-rw-   0        0        0     4547 2021-12-18 18:38:01.000000 glow-0.11.3/glow/nn/util.py
--rw-rw-rw-   0        0        0     1356 2021-12-18 18:38:01.000000 glow-0.11.3/glow/nn/vision.py
-drwxrwxrwx   0        0        0        0 2021-12-18 18:42:24.473484 glow-0.11.3/glow/test/
--rw-rw-rw-   0        0        0        0 2020-02-22 10:35:07.000000 glow-0.11.3/glow/test/__init__.py
--rw-rw-rw-   0        0        0     1688 2021-10-06 12:16:20.000000 glow-0.11.3/glow/test/run_metrics.py
--rw-rw-rw-   0        0        0      820 2021-10-02 18:18:43.000000 glow-0.11.3/glow/test/test_api.py
--rw-rw-rw-   0        0        0      893 2021-11-30 12:29:53.000000 glow-0.11.3/glow/test/test_batch.py
--rw-rw-rw-   0        0        0      617 2021-11-30 12:29:53.000000 glow-0.11.3/glow/test/test_buffered.py
--rw-rw-rw-   0        0        0     3522 2021-12-18 18:38:01.000000 glow-0.11.3/glow/test/test_cli.py
--rw-rw-rw-   0        0        0     1172 2021-12-18 18:38:01.000000 glow-0.11.3/glow/test/test_len.py
--rw-rw-rw-   0        0        0      815 2021-10-06 12:24:38.000000 glow-0.11.3/glow/test/test_loader.py
--rw-rw-rw-   0        0        0     1046 2021-11-30 12:29:53.000000 glow-0.11.3/glow/test/test_shm.py
--rw-rw-rw-   0        0        0     4191 2021-11-30 12:29:53.000000 glow-0.11.3/glow/test/test_thread_pool.py
--rw-rw-rw-   0        0        0      873 2021-12-18 18:38:01.000000 glow-0.11.3/glow/test/test_timed.py
--rw-rw-rw-   0        0        0      362 2021-07-09 17:43:25.000000 glow-0.11.3/glow/test/test_timer.py
--rw-rw-rw-   0        0        0     1469 2021-10-06 12:25:37.000000 glow-0.11.3/glow/test/test_uuid.py
-drwxrwxrwx   0        0        0        0 2021-12-18 18:42:24.477319 glow-0.11.3/glow/transforms/
--rw-rw-rw-   0        0        0      546 2021-12-18 18:38:01.000000 glow-0.11.3/glow/transforms/__init__.py
--rw-rw-rw-   0        0        0    10854 2021-12-18 18:38:01.000000 glow-0.11.3/glow/transforms/classes.py
--rw-rw-rw-   0        0        0     4476 2021-12-18 18:38:01.000000 glow-0.11.3/glow/transforms/core.py
-drwxrwxrwx   0        0        0        0 2021-12-18 18:42:24.482320 glow-0.11.3/glow/transforms/functional/
--rw-rw-rw-   0        0        0      121 2021-12-18 18:38:01.000000 glow-0.11.3/glow/transforms/functional/__init__.py
--rw-rw-rw-   0        0        0     3866 2021-12-18 18:38:01.000000 glow-0.11.3/glow/transforms/functional/core.py
--rw-rw-rw-   0        0        0     1772 2021-12-18 18:38:01.000000 glow-0.11.3/glow/transforms/functional/numba.py
-drwxrwxrwx   0        0        0        0 2021-12-18 18:42:24.414321 glow-0.11.3/glow.egg-info/
--rw-rw-rw-   0        0        0     2746 2021-12-18 18:42:24.000000 glow-0.11.3/glow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1934 2021-12-18 18:42:24.000000 glow-0.11.3/glow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       51 2021-12-18 18:42:24.000000 glow-0.11.3/glow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2020-11-03 12:28:57.000000 glow-0.11.3/glow.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     1113 2021-12-18 18:42:24.000000 glow-0.11.3/glow.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2021-12-18 18:42:24.000000 glow-0.11.3/glow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3291 2021-12-18 18:42:24.485319 glow-0.11.3/setup.cfg
--rw-rw-rw-   0        0        0     1702 2021-12-18 18:38:01.000000 glow-0.11.3/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glow-0.12.7/examples/__init__.py
+-rw-r--r--   0        0        0     4860 2020-02-02 00:00:00.000000 glow-0.12.7/examples/cifar10.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 glow-0.12.7/examples/gan.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/__init__.py
+-rw-r--r--   0        0        0     8055 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/cli.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/cli.pyi
+-rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/distributed.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/py.typed
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/api/__init__.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/api/config.py
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/api/exporting.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/core/__init__.py
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/core/_coro.py
+-rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/core/_import_hook.py
+-rw-r--r--   0        0        0     6110 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/core/_more.py
+-rw-r--r--   0        0        0    16055 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/core/_parallel.py
+-rw-r--r--   0        0        0     3377 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/core/_parallel.pyi
+-rw-r--r--   0        0        0     4872 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/core/_patch_len.py
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/core/_patch_print.py
+-rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/core/_patch_scipy.py
+-rw-r--r--   0        0        0     5797 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/core/_profile.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/core/_profile.pyi
+-rw-r--r--   0        0        0     4780 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/core/_reduction.py
+-rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/core/_repr.py
+-rw-r--r--   0        0        0     3774 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/core/_sizeof.py
+-rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/core/_thread_quota.py
+-rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/core/_uuid.py
+-rw-r--r--   0        0        0     3846 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/core/debug.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/core/wrap/__init__.py
+-rw-r--r--   0        0        0     9469 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/core/wrap/cache.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/core/wrap/cache.pyi
+-rw-r--r--   0        0        0     7634 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/core/wrap/concurrency.py
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/core/wrap/concurrency.pyi
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/core/wrap/reusable.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/core/wrap/util.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/io/__init__.py
+-rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/io/_sound.py
+-rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/io/_svg.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/metrics/__init__.py
+-rw-r--r--   0        0        0     4683 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/metrics/base.py
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/metrics/confusion.py
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/metrics/raw.py
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/nn/__init__.py
+-rw-r--r--   0        0        0    11705 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/nn/_loader.py
+-rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/nn/_sampler.py
+-rw-r--r--   0        0        0     4492 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/nn/_trainer.py
+-rw-r--r--   0        0        0    13040 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/nn/amp.py
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/nn/driver.py
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/nn/functional.py
+-rw-r--r--   0        0        0     6886 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/nn/optimizers.py
+-rw-r--r--   0        0        0     7640 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/nn/plot.py
+-rw-r--r--   0        0        0     5720 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/nn/proto.py
+-rw-r--r--   0        0        0     6368 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/nn/util.py
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/nn/modules/__init__.py
+-rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/nn/modules/aggregates.py
+-rw-r--r--   0        0        0     7009 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/nn/modules/context.py
+-rw-r--r--   0        0        0    11277 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/nn/modules/convnets.py
+-rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/nn/modules/lazy.py
+-rw-r--r--   0        0        0     4666 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/nn/modules/simple.py
+-rw-r--r--   0        0        0     9355 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/nn/modules/transformers.py
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/nn/modules/util.py
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/nn/modules/vision.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/transforms/__init__.py
+-rw-r--r--   0        0        0    10958 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/transforms/classes.py
+-rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/transforms/core.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/transforms/functional/__init__.py
+-rw-r--r--   0        0        0     3891 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/transforms/functional/core.py
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/transforms/functional/numba.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glow-0.12.7/test/__init__.py
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 glow-0.12.7/test/run_metrics.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 glow-0.12.7/test/test_api.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 glow-0.12.7/test/test_batch.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 glow-0.12.7/test/test_buffered.py
+-rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 glow-0.12.7/test/test_cli.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 glow-0.12.7/test/test_iter.py
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 glow-0.12.7/test/test_loader.py
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 glow-0.12.7/test/test_shm.py
+-rw-r--r--   0        0        0     4418 2020-02-02 00:00:00.000000 glow-0.12.7/test/test_thread_pool.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 glow-0.12.7/test/test_timed.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 glow-0.12.7/test/test_timer.py
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 glow-0.12.7/test/test_uuid.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 glow-0.12.7/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 glow-0.12.7/LICENSE
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 glow-0.12.7/README.md
+-rw-r--r--   0        0        0     4589 2020-02-02 00:00:00.000000 glow-0.12.7/pyproject.toml
+-rw-r--r--   0        0        0     5146 2020-02-02 00:00:00.000000 glow-0.12.7/PKG-INFO
```

### Comparing `glow-0.11.3/LICENSE` & `glow-0.12.7/LICENSE`

 * *Files identical despite different names*

### Comparing `glow-0.11.3/README.md` & `glow-0.12.7/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 
 ```bash
 pip install glow[nn]  # For cv/neural network extras
 pip install glow[io]  # For I/O extras
 pip install glow[all]  # For all
 ```
 </details>
-Glow is compatible with: Python 3.9+, PyTorch 1.9+.
-Tested on ArchLinux, Ubuntu 18.04/20.04, Windows 10.
+Glow is compatible with: Python 3.9+, PyTorch 1.11+.
+Tested on ArchLinux, Ubuntu 18.04/20.04, Windows 10/11.
 
 ## Structure
 - `glow.*` - Core parts, available out the box
 - `glow.cv.*` - Tools for computer vision tasks
 - `glow.io.*` - I/O wrappers to access data in convenient formats
 - `glow.transforms` - Some custom-made augmentations for data
 - `glow.nn` - Neural nets and building blocks for them
@@ -33,27 +33,14 @@
 
 ## Core features
 - `glow.mapped` - convenient tool to parallelize computations
 - `glow.memoize` - use if you want to reduce number of calls for any function
 
 ## IO features
 
-### `glow.io.Slide` - ndarray-like reader for multiscale images (svs, tiff, etc...)
-<details>
-
-```python
-from glow.io import Slide
-
-slide = Slide.open('test.svs')
-shape: tuple[int, ...] = slide.shape
-scales: tuple[int, ...] = slide.scales
-image: np.ndarray = slide[:2048, :2048]  # Get numpy.ndarray
-```
-</details>
-
 ### `glow.io.Sound` - playable sound wrapper
 <details>
 
 ```python
 from datetime import timedelta
 
 import numpy as np
```

### Comparing `glow-0.11.3/glow/api/config.py` & `glow-0.12.7/src/glow/api/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 __all__ = ['env']
 
 from collections import ChainMap
 from collections.abc import Iterator
 from contextlib import contextmanager
-from typing import Any
 
 from ..core import repr_as_obj
 
 
 class _Env(ChainMap):
     """Environment with scopes.
     The outermost scope takes highest priority.
@@ -25,15 +24,15 @@
         _Env(a=1, b=3)
         _Env(a=1)
         >>> print(env)  # Reset to initial state
         _Env()
 
     """
     @contextmanager
-    def __call__(self, **items: Any) -> Iterator[None]:
+    def __call__(self, **items) -> Iterator[None]:
         self.maps.append(items)
         try:
             yield
         finally:
             self.maps.pop()
 
     def __repr__(self) -> str:
```

### Comparing `glow-0.11.3/glow/api/exporting.py` & `glow-0.12.7/src/glow/api/exporting.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,16 +47,17 @@
         return obj
 
     name = obj.__name__
     namespace = sys.modules[parent].__dict__
 
     __all__ = namespace.setdefault('__all__', [])
     if name in __all__ or name in namespace:
-        raise ExportError(f'Name "{name}" is reserved in <{parent}>'
-                          f' by <{namespace[name].__module__}:{name}>')
+        err = (f'Name "{name}" is reserved in <{parent}>'
+               f' by <{namespace[name].__module__}:{name}>')
+        raise ExportError(err)
 
     namespace[name] = obj
     __all__.append(name)
     return obj
 
 
 def import_tree(pkg: str):
@@ -74,8 +75,8 @@
 
 
 def get_wild_imports(module: ModuleType) -> tuple[str, ...]:
     """Get contents of module.__all__ if possible"""
     __all__ = getattr(module, '__all__', None)
     if __all__ is not None:
         return __all__
-    return tuple(name for name in dir(module) if not name.startswith('_'))
+    return *(name for name in dir(module) if not name.startswith('_')),
```

### Comparing `glow-0.11.3/glow/cli.py` & `glow-0.12.7/src/glow/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,91 @@
+"""argparse and dataclasses, married.
+
+Example:
+```
+@dataclass
+class Args:
+    a: int
+    b: str = 'hello'
+
+args, parser = parse_args(Args)
+```
+Or with plain function:
+```
+@parse_args
+def main(name: str = 'user'):
+    print(f'Hello {name}')
+```
+
+Reasons not to use alternatives:
+- [simple-parsing](https://github.com/lebrice/SimpleParsing):
+  - Has underscores (`--like_this`) instead of dashes (`--like-this`)
+  - Erases type on parser result, thus making typed prototype useless
+    (what is the point of using dataclasses if it is passed
+     through function returning typing.Any/argparse.Namespace?)
+
+- [datargs](https://github.com/roee30/datargs):
+  - No nesting support
+  - No function's support
+
+- [pydantic](https://github.com/samuelcolvin/pydantic):
+  - supports CLI via BaseSettings and environment variables parsing
+  - no nesting, as requires mixing only via multiple inheritance
+
+- [typer](https://github.com/tiangolo/typer):
+  - No support on dataclasses
+    (https://github.com/tiangolo/typer/issues/154).
+  - No fine way to extract parsed options without invoking because of
+    decorator/callback based implementation. Thus enforces wrapping of the
+    whole app into `typer.run`.
+    (https://github.com/tiangolo/typer/issues/197).
+"""
+
 from __future__ import annotations
 
 __all__ = ['arg', 'parse_args']
 
 import argparse
 import sys
 import types
 from argparse import ArgumentParser, BooleanOptionalAction, _ArgumentGroup
 from collections.abc import Callable, Collection, Iterator, Sequence
 from dataclasses import MISSING, Field, field, fields, is_dataclass
-from inspect import signature
+from inspect import getmodule, signature, stack
 from typing import (Any, Literal, TypeVar, Union, get_args, get_origin,
                     get_type_hints)
 
 _T = TypeVar('_T')
-_Node = Union[str, tuple[str, type[Any], list['_Node']]]  # type: ignore
+_Node = Union[str, tuple[str, type, list['_Node']]]
 _NoneType = type(None)
-_UNION_TYPES = [Union]
+_UNION_TYPES: list = [Union]
 
 if sys.version_info >= (3, 10):
     _UNION_TYPES += [types.UnionType]
 
 
 def arg(
-        default=MISSING,
-        /,
-        *,
-        flag=None,
-        factory=MISSING,
-        init=True,
-        repr=True,  # noqa: A002
-        hash=None,  # noqa: A002
-        help=None,  # noqa: A002
-        compare=True,
-        metadata=None):
+    default=MISSING,
+    /,
+    *,
+    flag=None,
+    factory=MISSING,
+    init=True,
+    repr=True,  # noqa: A002
+    hash=None,  # noqa: A002
+    help=None,  # noqa: A002
+    compare=True,
+    metadata=None,
+):
     """Convinient alias for dataclass.field with extra metadata (like help)"""
     metadata = metadata or {}
     for k, v in {'flag': flag, 'help': help}.items():
         if v:
             metadata = metadata | {k: v}
-    return field(  # type: ignore
+    return field(  # type: ignore[call-overload]
         default=default,
         default_factory=factory,
         init=init,
         repr=repr,
         hash=hash,
         compare=compare,
         metadata=metadata)
@@ -50,29 +93,30 @@
 
 def _unwrap_type(tp: type) -> tuple[type, dict[str, Any]]:
     if tp is list:
         raise ValueError('Type list should be parametrized')
 
     origin = get_origin(tp)
     *args, = get_args(tp)
-    if not origin or not args:
+    if not origin or not args:  # Not a generic type
         return tp, {'type': tp}
 
-    if origin is list:
+    if origin is list:  # `List[T]`
         cls, opts = _unwrap_type(args[0])
         return cls, opts | {'nargs': argparse.ZERO_OR_MORE}
 
+    # `Optional[T]` or `T | None`
     if origin in _UNION_TYPES and len(args) == 2 and _NoneType in args:
         args.remove(_NoneType)
         cls, opts = _unwrap_type(args[0])
         if opts.get('nargs') == argparse.ZERO_OR_MORE:
             return cls, opts
         return cls, opts | {'nargs': argparse.OPTIONAL}
 
-    if origin is Literal:
+    if origin is Literal:  # `Literal[x, y]`
         choices = get_args(tp)
         if len(tps := {type(c) for c in choices}) != 1:
             raise ValueError('Literal parameters should have '
                              f'the same type. Got: {tps}')
         cls, = tps
         return cls, {'type': cls, 'choices': choices}
 
@@ -95,63 +139,75 @@
             fd = p.default
         else:
             fd = arg(MISSING if p.default is p.empty else p.default)
         fd.name = p.name
         yield fd
 
 
-def _prepare_nested(parser: ArgumentParser | _ArgumentGroup, fn: Callable,
-                    seen: dict[str, list]) -> list[_Node]:
-    hints = get_type_hints(fn)
+def _visit_nested(parser: ArgumentParser | _ArgumentGroup, fn: Callable,
+                  seen: dict[str, list]) -> list[_Node]:
+    try:
+        hints = get_type_hints(fn)
+    except NameError:
+        if fn.__module__ != '__main__':
+            raise
+        for finfo in stack():
+            if not getmodule(finfo.frame):
+                hints = get_type_hints(fn, finfo.frame.f_globals)
+                break
+        else:
+            raise
 
     nodes: list[_Node] = []
     for fd in _get_fields(fn):
         if fd.init:
             seen.setdefault(fd.name, []).append(fn)
-            nodes.append(_prepare_field(parser, hints[fd.name], fd, seen))
+            nodes.append(_visit_field(parser, hints[fd.name], fd, seen))
 
     for name, usages in seen.items():
         if len(usages) > 1:
-            raise ValueError(f'Field name "{name}" occured multiple times: ' +
-                             ', '.join(f'{c.__module__}.{c.__qualname__}'
-                                       for c in usages) +
-                             '. All field names should be unique')
+            raise ValueError(f'Field name "{name}" occured multiple times: '
+                             + ', '.join(f'{c.__module__}.{c.__qualname__}'
+                                         for c in usages)
+                             + '. All field names should be unique')
     return nodes
 
 
-def _prepare_field(parser: ArgumentParser | _ArgumentGroup, tp: type,
-                   fd: Field, seen: dict[str, list]) -> _Node:
+def _visit_field(parser: ArgumentParser | _ArgumentGroup, tp: type, fd: Field,
+                 seen: dict[str, list]) -> _Node:
     cls, opts = _unwrap_type(tp)
 
     help_ = fd.metadata.get('help') or ''
     if cls is not bool and fd.default is not MISSING:
         help_ += f' (default: {fd.default})'
 
     if is_dataclass(cls):  # Nested dataclass
         arg_group = parser.add_argument_group(fd.name)
-        return fd.name, cls, _prepare_nested(arg_group, cls, seen)
+        return fd.name, cls, _visit_nested(arg_group, cls, seen)
 
     snake = fd.name.replace('_', '-')
     flags = [f] if (f := fd.metadata.get('flag')) else []
 
     if cls is bool:  # Optional
         if fd.default is MISSING:
             raise ValueError(f'Boolean field "{fd.name}" should have default')
         parser.add_argument(
             f'--{snake}',
             *flags,
             action=BooleanOptionalAction,
             default=fd.default,
             help=help_)
 
-    elif fd.default is not MISSING:  # Generic optional
+    # Generic optional
+    elif fd.default is not MISSING or fd.default_factory is not MISSING:
         if opts.get('nargs') == argparse.OPTIONAL:
             del opts['nargs']
+        default = fd.default_factory() if fd.default is MISSING else fd.default
         parser.add_argument(
-            f'--{snake}', *flags, **opts, default=fd.default, help=help_)
+            f'--{snake}', *flags, **opts, default=default, help=help_)
 
     elif isinstance(parser, ArgumentParser):  # Allow only for root parser
         if flags:
             raise ValueError(f'Positional-only field "{fd.name}" '
                              'should not have flag')
         parser.add_argument(snake, **opts, help=help_)
 
@@ -174,17 +230,17 @@
     return fn(**kwargs)
 
 
 def parse_args(fn: Callable[..., _T],
                args: Sequence[str] | None = None,
                prog: str | None = None) -> tuple[_T, ArgumentParser]:
     """Create parser from type hints of callable, parse args and do call"""
-    # TODO: Rename to `exec_cli`
+    # TODO: Rename to `run`
     parser = ArgumentParser(prog)
-    nodes = _prepare_nested(parser, fn, {})
+    nodes = _visit_nested(parser, fn, {})
 
     if args is not None:  # fool's protection
         args = line.split(' ') if (line := ' '.join(args).strip()) else []
 
     namespace = parser.parse_args(args)
     obj = _construct(vars(namespace), fn, nodes)
     return obj, parser
```

### Comparing `glow-0.11.3/glow/cli.pyi` & `glow-0.12.7/src/glow/cli.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import annotations
-
 from argparse import ArgumentParser
 from collections.abc import Callable, Mapping, Sequence
 from typing import Any, TypeVar, overload
 
 _T = TypeVar('_T')
 
 
@@ -14,42 +12,42 @@
         *,
         flag: str = ...,
         init: bool = ...,
         repr: bool = ...,  # noqa: A002
         hash: bool = ...,  # noqa: A002
         help: str = ...,  # noqa: A002
         compare: bool = ...,
-        metadata: Mapping[str, Any] = ...) -> _T:
+        metadata: Mapping[str, object] = ...) -> _T:
     ...
 
 
 @overload
 def arg(
         *,
         factory: Callable[[], _T],
         flag: str = ...,
         init: bool = ...,
         repr: bool = ...,  # noqa: A002
         hash: bool = ...,  # noqa: A002
         help: str = ...,  # noqa: A002
         compare: bool = ...,
-        metadata: Mapping[str, Any] = ...) -> _T:
+        metadata: Mapping[str, object] = ...) -> _T:
     ...
 
 
 @overload
 def arg(
         *,
         flag: str = ...,
         init: bool = ...,
         repr: bool = ...,  # noqa: A002
         hash: bool = ...,  # noqa: A002
         help: str = ...,  # noqa: A002
         compare: bool = ...,
-        metadata: Mapping[str, Any] = ...) -> Any:
+        metadata: Mapping[str, object] = ...) -> Any:
     ...
 
 
 def parse_args(fn: Callable[..., _T],
                args: Sequence[str] = ...,
                prog: str = ...) -> tuple[_T, ArgumentParser]:
     ...
```

### Comparing `glow-0.11.3/glow/core/__init__.py` & `glow-0.12.7/src/glow/core/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from . import _patch_len, _patch_print, _patch_scipy
-from ._len_helpers import as_sized
-from ._more import (as_iter, chunked, eat, ichunked, roundrobin, sliced,
-                    windowed)
-from ._parallel import buffered, map_n, starmap_n
+from ._coro import as_actor, coroutine, summary
+from ._more import as_iter, chunked, eat, ichunked, ilen, roundrobin, windowed
+from ._parallel import buffered, map_n, map_n_dict, starmap_n
 from ._profile import memprof, time_this, timer
 from ._repr import countable, mangle, repr_as_obj, si, si_bin
 from ._sizeof import sizeof
 from ._uuid import Uid
-from .debug import coroutine, lock_seed, summary, trace, trace_module, whereami
-from .wrap import (Reusable, call_once, memoize, shared_call, stream_batched,
-                   threadlocal)
+from .debug import lock_seed, trace, trace_module, whereami
+from .wrap import (Reusable, call_once, memoize, shared_call, streaming,
+                   threadlocal, weak_memoize)
 
 __all__ = [
-    'as_iter', 'as_sized', 'buffered', 'call_once', 'chunked', 'coroutine',
-    'countable', 'eat', 'ichunked', 'lock_seed', 'mangle', 'map_n', 'memoize',
-    'memprof', 'repr_as_obj', 'Reusable', 'roundrobin', 'shared_call', 'si',
-    'si_bin', 'sizeof', 'sliced', 'starmap_n', 'stream_batched', 'summary',
-    'threadlocal', 'time_this', 'timer', 'trace_module', 'trace', 'Uid',
-    'whereami', 'windowed'
+    'Reusable', 'Uid', 'as_actor', 'as_iter', 'buffered', 'call_once',
+    'chunked', 'coroutine', 'countable', 'eat', 'ichunked', 'ilen',
+    'lock_seed', 'mangle', 'map_n', 'map_n_dict', 'memoize', 'memprof',
+    'repr_as_obj', 'roundrobin', 'shared_call', 'si', 'si_bin', 'sizeof',
+    'starmap_n', 'streaming', 'summary', 'threadlocal', 'time_this', 'timer',
+    'trace', 'trace_module', 'weak_memoize', 'whereami', 'windowed'
 ]
 
 _patch_print.apply()
 _patch_len.apply()
 _patch_scipy.apply()
```

### Comparing `glow-0.11.3/glow/core/_import_hook.py` & `glow-0.12.7/src/glow/core/_import_hook.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 __all__ = ['register_post_import_hook', 'when_imported']
 
 import sys
 from collections.abc import Callable
 from importlib import abc, util
 from threading import RLock
 from typing import Any, TypeVar
@@ -19,15 +21,15 @@
         self.loader = loader
 
     def load_module(self, fullname):
         module = self.loader.load_module(fullname)
 
         with _LOCK:
             name = getattr(module, '__name__', None)
-            if hooks := _HOOKS.get(name):
+            if hooks := _HOOKS.get(name):  # type: ignore[arg-type]
                 while hooks:
                     hooks.pop()(module)
 
         return module
 
 
 class _ImportHookFinder(abc.MetaPathFinder, set):
@@ -36,30 +38,30 @@
             if fullname not in _HOOKS or fullname in self:
                 return None
 
             self.add(fullname)
             try:
                 if (spec := util.find_spec(fullname)) and spec.loader:
                     return _ImportHookChainedLoader(spec.loader)
-                return None
             finally:
                 self.remove(fullname)
+            return None
 
 
 def register_post_import_hook(hook: _Hook, name: str) -> None:
     """Register a new post import hook for the target module name.
 
     This will result in a proxy callback being registered which will defer
     loading of the specified module containing the callback function until
     required.
 
     Simplified version of wrapt.register_post_import_hook.
     """
     with _LOCK:
-        global _INITIALIZED
+        global _INITIALIZED  # noqa: PLW0603
         if not _INITIALIZED:
             _INITIALIZED = True
             sys.meta_path.insert(0, _ImportHookFinder())
 
         if (module := sys.modules.get(name)) is not None:
             hook(module)
         else:
```

### Comparing `glow-0.11.3/glow/core/_more.py` & `glow-0.12.7/src/glow/core/_more.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,129 +1,220 @@
 from __future__ import annotations
 
 __all__ = [
-    'as_iter', 'chunked', 'eat', 'ichunked', 'roundrobin', 'sliced', 'windowed'
+    'as_iter', 'chunked', 'eat', 'ichunked', 'ilen', 'roundrobin', 'windowed'
 ]
 
-import enum
 import threading
 from collections import deque
-from collections.abc import Iterable, Iterator, Sequence
-from itertools import chain, cycle, islice, repeat, tee
-from typing import Any, TypeVar, overload
+from collections.abc import Iterable, Iterator, Mapping, Sequence, Sized
+from functools import partial
+from itertools import chain, count, cycle, islice, repeat
+from typing import Protocol, TypeVar, overload
 
-import numpy as np
-
-from ._len_helpers import _SizedIterator, as_sized
+_T = TypeVar('_T')
+_T_co = TypeVar('_T_co', covariant=True)
 
 
-class _Empty(enum.Enum):
-    token = 0
+class SupportsSlice(Sized, Protocol[_T_co]):
+    def __getitem__(self, __s: slice) -> _T_co:
+        ...
 
 
-_T = TypeVar('_T')
-_Seq = TypeVar('_Seq', bound=Sequence)
-_Dtype = TypeVar('_Dtype', bound=np.dtype)
-_empty = _Empty.token
+# ----------------------------------------------------------------------------
 
 
-def as_iter(obj: Iterable[_T] | _T, limit: int = None) -> Iterator[_T]:
+def as_iter(obj: Iterable[_T] | _T, limit: int | None = None) -> Iterator[_T]:
     """Make iterator with at most `limit` items"""
     if isinstance(obj, Iterable):
         return islice(obj, limit)
     return repeat(obj) if limit is None else repeat(obj, limit)
 
 
-def windowed(it: Iterable[_T], size: int) -> Iterator[tuple[_T, ...]]:
-    """Retrieve overlapped windows from iterable.
+# ----------------------------------------------------------------------------
 
-    >>> [*windowed(range(5), 3)]
-    [(0, 1, 2), (1, 2, 3), (2, 3, 4)]
-    """
-    return zip(*(islice(it_, start, None)
-                 for start, it_ in enumerate(tee(it, size))))
+
+def _dispatch(fallback_fn, fn, it, *args):
+    if (not isinstance(it, Sized) or not hasattr(it, '__getitem__')
+            or isinstance(it, Mapping)):
+        return fallback_fn(it, *args)
+
+    r = fn(it, *args)
+    if isinstance(it, Sequence):
+        return r
+
+    try:
+        # Ensure that slice is supported by prefetching 1st item
+        first_or_none = *islice(r, 1),
+    except TypeError:
+        return fallback_fn(it, *args)
+    else:
+        return chain(first_or_none, r)
+
+
+# ----------------------------------------------------------------------------
+
+
+def window_hint(it, size):
+    return len(it) + 1 - size
+
+
+def chunk_hint(it, size):
+    return len(range(0, len(it), size))
+
+
+def _sliced_windowed(s: SupportsSlice[_T], size: int) -> Iterator[_T]:
+    indices = range(len(s) + 1)
+    slices = map(slice, indices[:-size], indices[size:])
+    return map(s.__getitem__, slices)
+
+
+def _windowed(it: Iterable[_T], size: int) -> Iterator[tuple[_T, ...]]:
+    if size == 1:  # Trivial case
+        return zip(it)
+
+    it = iter(it)
+    w = deque(islice(it, size), maxlen=size)
+
+    if len(w) != size:
+        return iter(())
+    return map(tuple, chain([w], map(w.__iadd__, zip(it))))
+
+
+def _sliced(s: SupportsSlice[_T], size: int) -> Iterator[_T]:
+    indices = range(len(s) + size)
+    slices = map(slice, indices[::size], indices[size::size])
+    return map(s.__getitem__, slices)
+
+
+def _chunked(it: Iterable[_T], size: int) -> Iterator[tuple[_T, ...]]:
+    if size == 1:  # Trivial case
+        return zip(it)
+
+    # TODO: python 3.12 - `itertools.batched(it, size)`
+    fetch_chunk = partial(islice, iter(it), size)
+    chunks = iter(fetch_chunk, None)
+    return iter(map(tuple, chunks).__next__, ())  # type: ignore[arg-type]
 
 
 # ---------------------------------------------------------------------------
+
+
 @overload
-def sliced(seq: _Seq, size: int) -> Iterator[_Seq]:
+def windowed(it: SupportsSlice[_T], size: int) -> Iterator[_T]:
     ...
 
 
 @overload
-def sliced(seq: np.ndarray[Any, _Dtype],
-           size: int) -> Iterator[np.ndarray[Any, _Dtype]]:
+def windowed(it: Iterable[_T], size: int) -> Iterator[tuple[_T, ...]]:
     ...
 
 
-def sliced(seq, size):
-    """Split sequence to slices of at most size items each.
+def windowed(it, size):
+    """Retrieve overlapped windows from iterable.
+    Tries to use slicing if possible.
 
-    >>> s = sliced(range(10), 3)
-    >>> len(s)
-    4
-    >>> [*s]
-    [range(0, 3), range(3, 6), range(6, 9), range(9, 10)]
+    >>> [*windowed(range(6), 3)]
+    [range(0, 3), range(1, 4), range(2, 5), range(3, 6)]
+
+    >>> [*windowed(iter(range(6)), 3)]
+    [(0, 1, 2), (1, 2, 3), (2, 3, 4), (3, 4, 5)]
     """
-    offsets = range(len(seq) + size)
-    slices = map(slice, offsets[0::size], offsets[size::size])
-    return map(seq.__getitem__, slices)
+    return _dispatch(_windowed, _sliced_windowed, it, size)
 
 
-# ---------------------------------------------------------------------------
-def chunk_hint(it, size):
-    return len(range(0, len(it), size))
+@overload
+def chunked(__it: SupportsSlice[_T], size: int) -> Iterator[_T]:
+    ...
 
 
-@as_sized(hint=chunk_hint)
-def chunked(it: Iterable[_T], size: int) -> Iterator[tuple[_T, ...]]:
-    """Split iterable to chunks of at most size items each.
+@overload
+def chunked(__it: Iterable[_T], size: int) -> Iterator[tuple[_T, ...]]:
+    ...
+
+
+def chunked(it, size):
+    """
+    Splits iterable to chunks of at most size items each.
+    Uses slicing if possible.
     Each next() on result will advance passed iterable to size items.
 
-    >>> s = chunked(range(10), 3)
-    >>> len(s)
-    4
-    >>> [*s]
+    >>> [*chunked(range(10), 3)]
+    [range(0, 3), range(3, 6), range(6, 9), range(9, 10)]
+
+    >>> [*chunked(iter(range(10)), 3)]
     [(0, 1, 2), (3, 4, 5), (6, 7, 8), (9,)]
     """
-    chunks = map(islice, repeat(iter(it)), repeat(size))  # type: ignore
-    return iter(map(tuple, chunks).__next__, ())  # type: ignore
+    return _dispatch(_chunked, _sliced, it, size)
+
+
+# ----------------------------------------------------------------------------
+
+
+def _deiter(q: deque[_T]) -> Iterator[_T]:
+    # Same as iter_except(q.popleft, IndexError) from docs of itertools
+    try:
+        while True:
+            yield q.popleft()
+    except IndexError:
+        return
 
 
-@as_sized(hint=chunk_hint)
 def ichunked(it: Iterable[_T], size: int) -> Iterator[Iterator[_T]]:
     """Split iterable to chunks of at most size items each.
 
     Does't consume items from passed iterable to return complete chunk
     unlike chunked, as yields iterators, not sequences.
 
     >>> s = ichunked(range(10), 3)
     >>> len(s)
     4
     >>> [[*chunk] for chunk in s]
     [[0, 1, 2], [3, 4, 5], [6, 7, 8], [9]]
     """
-    head = iter(it)
-    while (item := next(head, _empty)) is not _empty:
-        chunk = islice(chain([item], head), size)  # Restore iterable
-        chunk1, chunk2 = tee(chunk)  # Fork to keep not-yet-consumed
-        yield _SizedIterator(chunk1, size)
-        eat(chunk2)  # Advance to head[size:]
+    if size == 1:  # Trivial case
+        yield from map(iter, zip(it))  # type: ignore[arg-type]
+        return
+
+    it = iter(it)
+    while head := deque(islice(it, 1)):
+        # Remaining chunk items
+        body = islice(it, size - 1)
+
+        # Cache for not-yet-consumed
+        tail = deque[_T]()
+
+        # Include early fetched item into chunk
+        yield chain(_deiter(head), body, _deiter(tail))
+
+        # Advance and fill internal cache, expand tail with items from body
+        tail += body
+
+
+# ----------------------------------------------------------------------------
+
+
+def ilen(iterable: Iterable) -> int:
+    """Return number of items in *iterable*.
+
+    This consumes iterable, so handle with care.
+    See `more_itertools.ilen`.
+    """
+    counter = count()
+    deque(zip(iterable, counter), maxlen=0)
+    return next(counter)
 
 
 def eat(iterable: Iterable, daemon: bool = False) -> None:
     """Consume iterable, daemonize if needed (move to background thread)"""
     if daemon:
         threading.Thread(target=deque, args=(iterable, 0), daemon=True).start()
     else:
-        deque(iterable, 0)
+        deque(iterable, 0)  # Same as `more_itertools.consume(..., n=None)`
 
 
-@as_sized(hint=lambda *it: sum(map(len, it)))
 def roundrobin(*iterables: Iterable[_T]) -> Iterator[_T]:
     """roundrobin('ABC', 'D', 'EF') --> A D E B F C"""
-    # FIXME: remove size hint
-    # size hint fails when iterables are repeated, it gives only top bound
-    iters = cycle(map(iter, iterables))
-    for pending in range(len(iterables))[::-1]:
+    iters = cycle(iter(it) for it in iterables)
+    for pending in range(len(iterables) - 1, -1, -1):
         yield from map(next, iters)
         iters = cycle(islice(iters, pending))
```

### Comparing `glow-0.11.3/glow/core/_parallel.py` & `glow-0.12.7/src/glow/core/_parallel.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,67 +1,153 @@
 from __future__ import annotations
 
-__all__ = ['buffered', 'map_n', 'starmap_n']
+__all__ = ['buffered', 'map_n', 'map_n_dict', 'starmap_n']
 
 import atexit
 import enum
 import os
 import signal
 import sys
-from collections.abc import Callable, Iterable, Iterator
-from concurrent.futures import Executor, Future, ThreadPoolExecutor
+import warnings
+import weakref
+from collections.abc import Callable, Iterable, Iterator, Mapping, Sized
+from concurrent.futures import Executor, Future
+from concurrent.futures import TimeoutError as _TimeoutError
 from contextlib import ExitStack, contextmanager
 from cProfile import Profile
-from dataclasses import dataclass
 from functools import partial
-from itertools import chain, islice, starmap, tee
+from itertools import chain, islice, starmap
+from multiprocessing.managers import BaseManager
 from operator import methodcaller
 from pstats import Stats
-from queue import Queue, SimpleQueue
-from threading import Event, RLock
-from time import perf_counter
-from typing import ContextManager, Protocol, TypeVar, cast
+from queue import Empty, SimpleQueue
+from threading import Lock
+from time import perf_counter, sleep
+from typing import Protocol, TypeVar, cast
 
 import loky
-from loky.process_executor import ProcessPoolExecutor
 
-from ._more import chunked, sliced
+try:
+    import psutil
+except ImportError:
+    psutil = None
+
+from ._more import chunked, ilen
 from ._reduction import move_to_shmem, reducers
+from ._thread_quota import ThreadQuota
 
 _T = TypeVar('_T')
+_T_ctr = TypeVar('_T_ctr', contravariant=True)
+_K = TypeVar('_K')
 _F = TypeVar('_F', bound=Future)
+
 _NUM_CPUS = os.cpu_count() or 0
+_NUM_CPUS = min(_NUM_CPUS, int(os.getenv('GLOW_CPUS', _NUM_CPUS)))
 _IDLE_WORKER_TIMEOUT = 10
+_GRANULAR_SCHEDULING = False  # TODO: investigate whether this improves load
 
 
 class _Empty(enum.Enum):
     token = 0
 
 
 _empty = _Empty.token
 
-# -------------------------- some useful interfaces --------------------------
+# ------------------- some useful interfaces and functions -------------------
 
 
-class _IQueue(Protocol[_T]):
-    def get(self) -> _T:
+class _Queue(Protocol[_T]):
+    def get(self, block: bool = ..., timeout: float | None = ...) -> _T:
         ...
 
-    def put(self, value: _T) -> None:
+    def put(self, item: _T) -> None:
         ...
 
 
-class _IEvent(Protocol):
+class _Event(Protocol):
     def is_set(self) -> bool:
         ...
 
-    def set(self) -> None:  # noqa: A003
+    def set(self) -> None:
         ...
 
 
+def _get_cpu_count_limits(upper_bound: int = sys.maxsize,
+                          mp: bool = False) -> Iterator[int]:
+    yield upper_bound
+    yield os.cpu_count() or 1
+
+    # Windows platform lacks memory overcommit, so it's sensitive to VMS growth
+    if not mp or sys.platform != 'win32' or 'torch' not in sys.modules:
+        return
+
+    import torch
+    if torch.version.cuda and torch.version.cuda >= '11.7.0':
+        # It's expected that torch will fix .nv_fatb readonly flag in its DLLs
+        # See https://stackoverflow.com/a/69489193/9868257
+        return
+
+    if psutil is None:
+        warnings.warn(
+            'Max process count may be calculated incorrectly, '
+            'leading to application crash or even BSOD. '
+            'Install psutil to avoid that',
+            stacklevel=3)
+        return
+
+    # Overcommit on Windows is forbidden, thus VMS planning is necessary
+    vms: int = psutil.Process().memory_info().vms
+    free_vms: int = psutil.virtual_memory().free + psutil.swap_memory().free
+    yield free_vms // vms
+
+
+def max_cpu_count(upper_bound: int = sys.maxsize, mp: bool = False) -> int:
+    return min(_get_cpu_count_limits(upper_bound, mp))
+
+
+_PATIENCE = 0.01
+
+
+def _retry_call(fn: Callable[..., _T], *exc: type[BaseException]) -> _T:
+    # See issues
+    # https://bugs.python.org/issue29971
+    # https://github.com/python/cpython/issues/74157
+    # https://github.com/dask/dask/pull/2144#issuecomment-290556996
+    # https://github.com/dask/dask/pull/2144/files
+    while True:
+        try:
+            return fn(timeout=_PATIENCE)
+        except exc:
+            sleep(0)  # Force switch to another thread to proceed
+
+
+if sys.platform == 'win32':
+
+    def _result(f: Future[_T], /) -> _T:
+        return _retry_call(f.result, _TimeoutError)
+else:
+    _result = Future.result
+
+
+def _result_or_cancel(f: Future[_T]) -> _T:
+    try:
+        try:
+            return _result(f)
+        finally:
+            f.cancel()
+    finally:
+        del f
+
+
+def _q_get_fn(q: _Queue[_T]) -> Callable[[], _T]:
+    if sys.platform != 'win32':
+        return q.get
+    return partial(_retry_call, q.get, Empty)
+
+
 # ---------------------------- pool initialization ----------------------------
 
 
 def _mp_profile():
     """Multiprocessed profiler"""
     prof = Profile()
     prof.enable()
@@ -80,106 +166,123 @@
     if os.environ.get('_GLOW_MP_PROFILE'):
         _mp_profile()
 
 
 @contextmanager
 def _get_executor(max_workers: int, mp: bool) -> Iterator[Executor]:
     if mp:
-        processes: ProcessPoolExecutor = loky.get_reusable_executor(
+        processes: loky.ProcessPoolExecutor = loky.get_reusable_executor(
             max_workers,
             'loky_init_main',
             _IDLE_WORKER_TIMEOUT,
             job_reducers=reducers,
             result_reducers=reducers,
             initializer=_initializer,
         )
         # In generator 'finally' is not reliable enough, use atexit
         hook = atexit.register(processes.shutdown, kill_workers=True)
         yield processes
         atexit.unregister(hook)
     else:
-        threads = ThreadPoolExecutor(max_workers)
+        threads = ThreadQuota(max_workers)
         try:
             yield threads
         finally:
-            # TODO: On pool death, set flag in proxy.
-            # TODO: In each worker, check this flag before call,
-            # TODO:  if it's set, then kill all worker-owned pools.
-            # TODO: To use this, somethere should be dict[ident, list[pool]]
-            is_success = sys.exc_info() is None
+            is_success = sys.exc_info()[0] is None
             threads.shutdown(wait=is_success, cancel_futures=True)
 
 
-def _setup_queues(
-        stack: ExitStack, latency: int,
-        executor: bool | Executor) -> tuple[Executor, _IQueue, _IEvent]:
-    if not isinstance(executor, Executor):
-        executor = stack.enter_context(_get_executor(1, executor))
-
-    if isinstance(executor, ThreadPoolExecutor):
-        return executor, Queue(latency), Event()
-
-    assert isinstance(executor, loky.ProcessPoolExecutor)
-    mgr = stack.enter_context(executor._context.Manager())
-    return executor, mgr.Queue(latency), mgr.Event()
+def _get_manager(executor: Executor):
+    if isinstance(executor, loky.ProcessPoolExecutor):
+        return executor._context.Manager()
+
+    else:  # noqa: RET505
+        from multiprocessing.dummy import Manager
+        return Manager()
 
 
 # -------- bufferize iterable by offloading to another thread/process --------
 
 
-@dataclass
-class buffered(Iterable[_T]):  # noqa: N801
+def _consume(iterable: Iterable[_T], q: _Queue[_T | _Empty], ev: _Event):
+    try:
+        for item in iterable:
+            if ev.is_set():
+                break
+            q.put(item)
+    finally:
+        q.put(_empty)  # Signal to stop iteration
+        q.put(_empty)  # Match last q.get
+
+
+class buffered(Iterator[_T]):  # noqa: N801
     """
     Iterates over `iterable` in background thread with at most `latency`
     items ahead from caller
     """
-    iterable: Iterable[_T]
-    latency: int = 2
-    mp: bool | Executor = False
-
-    def _consume(self, q: _IQueue[_T | _Empty], stop: _IEvent):
-        with ExitStack() as s:
-            s.callback(q.put, _empty)  # Match last q.get
-            s.callback(q.put, _empty)  # Signal to stop iteration
-
-            for item, _ in zip(self.iterable, iter(stop.is_set, True)):
-                q.put(item)
-
-            # if stop.is_set():
-            #     s.pop_all()
-            # q.put(_empty)  # Will happen if all ok to notify main to stop
+    __slots__ = ('_get', '_task', 'close', '__weakref__')
+
+    def __init__(self,
+                 iterable: Iterable[_T],
+                 /,
+                 *,
+                 latency: int = 2,
+                 mp: bool | Executor = False):
+        s = ExitStack()
+        if isinstance(mp, Executor):
+            executor = mp
+        else:
+            executor = s.enter_context(_get_executor(1, mp))
+
+        mgr = _get_manager(executor)
+        if isinstance(mgr, BaseManager):
+            s.enter_context(mgr)
+
+        ev: _Event = mgr.Event()
+        q: _Queue[_T | _Empty] = mgr.Queue(latency)
+        self._task = executor.submit(_consume, iterable, q, ev)  # type: ignore
+        self._get = q_get = _q_get_fn(q)
+
+        # If main killed, wakes up consume to check ev
+        # Otherwise collects 2nd _empty from q.
+        # Called 2nd
+        s.callback(q_get)
+
+        # If main killed, signals consume to stop.
+        # If consume is already stopped (on error or not), does nothing.
+        # Called 1st
+        s.callback(ev.set)
+
+        self.close = weakref.finalize(self, s.close)
 
     def __iter__(self) -> Iterator[_T]:
-        with ExitStack() as s:
-            q: _IQueue[_T | _Empty]
-            executor, q, stop = _setup_queues(s, self.latency, self.mp)
-
-            s.callback(q.get)  # Wakes q.put when main fails
-            s.callback(stop.set)
-
-            task = executor.submit(self._consume, q, stop)
-            while (item := q.get()) is not _empty:
-                yield item
-            task.result()  # Throws if `consume` is dead
+        return self
 
-    def __len__(self) -> int:
-        return len(self.iterable)  # type: ignore
+    def __next__(self) -> _T:
+        if self.close.alive:
+            if (item := self._get()) is not _empty:
+                return item
+
+            self.close()
+            _result(self._task)  # Throws exception if worker killed itself
+
+        raise StopIteration
 
 
 # ---------------------------- automatic batching ----------------------------
 
 
 class _AutoSize:
     MIN_DURATION = 0.2
     MAX_DURATION = 2.0
     size: int = 1
     duration: float = 0.0
 
     def __init__(self) -> None:
-        self.lock = RLock()
+        self.lock = Lock()
 
     def suggest(self) -> int:
         with self.lock:
             if 0 < self.duration < self.MIN_DURATION:
                 self.size *= 2
                 self.duration = 0.0
 
@@ -188,68 +291,113 @@
                 size = max(size, 1)
                 if self.size != size:
                     self.duration = 0.0
                     self.size = size
 
             return self.size
 
-    def update(self, start_time: float, fut: Future[list]):
-        if fut.cancelled() or fut.exception():
+    def update(self, start_time: float, fut: Future[Sized]):
+        # Compute as soon as future became done, discard later if not needed
+        duration = perf_counter() - start_time
+
+        try:
+            # Cannot time out, as future is always completed at this point.
+            # Though it's unknown whether it succeeded or not, so use EAFP
+            r = fut.result()
+        except BaseException:  # noqa: BLE001
             return
 
-        size = len(fut.result())
         with self.lock:
-            if size != self.size:
+            if len(r) != self.size:
                 return
-            duration = perf_counter() - start_time
             self.duration = ((0.8 * self.duration + 0.2 * duration)
                              if self.duration > 0 else duration)
 
 
 # ---------------------- map iterable through function ----------------------
 
 
-def _schedule(make_future: Callable[..., _F], args_zip: Iterable[tuple],
+def _schedule(make_future: Callable[..., _F], args_zip: Iterable[Iterable],
               chunksize: int) -> Iterator[_F]:
     return starmap(make_future, chunked(args_zip, chunksize))
 
 
-def _schedule_auto(make_future: Callable[..., _F], args_zip: Iterable[tuple],
-                   max_workers: int) -> Iterator[_F]:
-    it = iter(args_zip)
+def _schedule_auto(
+    make_future: Callable[..., _F],
+    args_zip: Iterator[Iterable],
+    max_workers: int,
+) -> Iterator[_F]:
+    # For the whole wave make futures with the same job size
     size = _AutoSize()
-    while items := [*islice(it, size.suggest() * max_workers)]:
-        chunksize = len(items) // max_workers or 1
-        for f in starmap(make_future, sliced(items, chunksize)):
+    while tuples := [*islice(args_zip, size.suggest() * max_workers)]:
+        chunksize = len(tuples) // max_workers or 1
+        for f in starmap(make_future, chunked(tuples, chunksize)):
             f.add_done_callback(partial(size.update, perf_counter()))
             yield f
 
 
-def _unwrap(cm: ContextManager, fs: Iterable[Future[_T]], qsize: int | None,
+def _schedule_auto_v2(make_future: Callable[..., _F],
+                      args_zip: Iterator[Iterable]) -> Iterator[_F]:
+    # Vary job size from future to future
+    size = _AutoSize()
+    while args := [*islice(args_zip, size.suggest())]:
+        f = make_future(*args)
+        f.add_done_callback(partial(size.update, perf_counter()))
+        yield f
+
+
+def _get_unwrap_iter(s: ExitStack, qsize: int,
+                     get_done_f: Callable[[], Future[_T]],
+                     fs_scheduler: Iterator) -> Iterator[_T]:
+    with s:
+        if not qsize:  # No tasks to do
+            return
+
+        # Unwrap 1st / schedule `N-qsize` / unwrap `qsize-1`
+        for _ in chain([None], fs_scheduler, range(qsize - 1)):
+
+            # Retrieve done task, exactly `N` calls
+            yield _result_or_cancel(get_done_f())
+
+
+def _unwrap(s: ExitStack, fs: Iterable[Future[_T]], qsize: int | None,
             order: bool) -> Iterator[_T]:
-    q: SimpleQueue[Future] = SimpleQueue()
-    q_put = q.put if order else methodcaller('add_done_callback', q.put)
+    q = SimpleQueue[Future[_T]]()
 
-    it1, it2 = tee(fs)
-    f_to_none = zip(it1, map(q_put, it2))  # type: ignore
-    with cm:
-        todo = dict(islice(f_to_none, qsize))
-        while todo:
-            f = q.get()
-            yield f.result()
-            todo.pop(f)
-            todo.update(islice(f_to_none, 1))
+    # If `order`, then `q` has "PENDING"/"RUNNING"/"DONE" tasks,
+    # otherwise it only has "DONE" tasks.
+    # FIXME: order=False -> random freezes (in q.get -> Empty)
+    q_put = cast(Callable[[Future[_T]], None],
+                 q.put if order else methodcaller('add_done_callback', q.put))
+
+    # On each `next()` schedules new task
+    fs_scheduler = map(q_put, fs)
+    try:
+        # Fetch up to `qsize` tasks to pre-fill `q`
+        qsize = ilen(islice(fs_scheduler, qsize))
+
+    except BaseException:
+        # Unwind stack here on an error
+        s.close()
+        raise
+
+    else:
+        return _get_unwrap_iter(s, qsize, _q_get_fn(q), fs_scheduler)
+
+
+def _batch_invoke(func: Callable[..., _T], *items: tuple) -> list[_T]:
+    return [*starmap(func, items)]
 
 
 def starmap_n(func: Callable[..., _T],
-              iterable: Iterable[tuple],
+              iterable: Iterable[Iterable],
               /,
               *,
               max_workers: int | None = None,
-              prefetch: int | None = None,
+              prefetch: int | None = 2,
               mp: bool = False,
               chunksize: int | None = None,
               order: bool = True) -> Iterator[_T]:
     """
     Equivalent to itertools.starmap(fn, iterable).
 
     Return an iterator whose values are returned from the function evaluated
@@ -266,65 +414,73 @@
     - order - Whether keep results order, or ignore it to increase performance.
 
     Unlike multiprocessing.Pool or concurrent.futures.Executor this one:
 
     - never deadlocks on any exception or Ctrl-C interruption.
     - accepts infinite iterables due to lazy task creation (option prefetch).
     - has single interface for both threads and processes.
-    - TODO: serializes array-like data using out-of-band Pickle 5 buffers
+    - TODO: serializes array-like data using out-of-band Pickle 5 buffers.
+    - before first `__next__` call it submits at most `prefetch` jobs
+      to warmup pool of workers.
 
     Notes:
 
     - To reduce latency set order to False, order of results will be arbitrary.
     - To increase CPU usage increase prefetch or set it to None.
     - In terms of CPU usage there's no difference between
       prefetch=None and order=False, so choose wisely.
     - Setting order to False makes no use of prefetch more than 0.
 
+    TODO: replace `order=True` with `heap=False`
     """
     if max_workers is None:
-        max_workers = _NUM_CPUS
-        if mp and sys.platform == 'win32' and 'torch' in sys.modules:
-            # On Windows torch initializes CUDA in each process
-            # with RSS leak up to 2GB/process,
-            # so we limit count of subprocesses
-            max_workers = min(_NUM_CPUS, 12)
+        max_workers = max_cpu_count(_NUM_CPUS, mp)
 
-    if not max_workers:
+    if not max_workers or not _NUM_CPUS:
         return starmap(func, iterable)  # Fallback to single thread
 
     if mp and chunksize is None and prefetch is None:
         raise ValueError('With multiprocessing either chunksize or prefetch '
                          'must be not None')
 
     if prefetch is not None:
-        prefetch += max_workers
+        prefetch = max(prefetch + max_workers, 1)
 
     it = iter(iterable)
-    cm = ExitStack()
-    submit = cm.enter_context(_get_executor(max_workers, mp)).submit
+    s = ExitStack()
+    submit = s.enter_context(_get_executor(max_workers, mp)).submit
 
     if mp:
-        submit_many = cast(
-            Callable[..., Future[list[_T]]],
-            partial(submit, move_to_shmem(func)),
-        )
-        if chunksize is None:
-            fs = _schedule_auto(submit_many, it, max_workers)
-        else:
-            fs = _schedule(submit_many, it, chunksize or 1)
-
-        chunks = _unwrap(cm, fs, prefetch, order)
-        return chain.from_iterable(chunks)
+        func = move_to_shmem(func)
     else:
+        chunksize = chunksize or 1
+
+    if chunksize == 1:
         submit_one = cast(
             Callable[..., Future[_T]],
             partial(submit, func),
         )
-        return _unwrap(cm, starmap(submit_one, it), prefetch, order)
+        return _unwrap(s, starmap(submit_one, it), prefetch, order)
+
+    submit_many = cast(
+        Callable[..., Future[list[_T]]],
+        partial(submit, _batch_invoke, func),
+    )
+    if chunksize is not None:
+        # Fixed chunksize
+        fs = _schedule(submit_many, it, chunksize)
+    elif not _GRANULAR_SCHEDULING:
+        # Dynamic chunksize scaling, submit tasks in waves
+        fs = _schedule_auto(submit_many, it, max_workers)
+    else:
+        # Dynamic chunksize scaling
+        fs = _schedule_auto_v2(submit_many, it)
+
+    chunks = _unwrap(s, fs, prefetch, order)
+    return chain.from_iterable(chunks)
 
 
 def map_n(func: Callable[..., _T],
           /,
           *iterables: Iterable,
           max_workers: int | None = None,
           prefetch: int | None = 2,
@@ -343,7 +499,29 @@
         func,
         zip(*iterables),
         max_workers=max_workers,
         prefetch=prefetch,
         mp=mp,
         chunksize=chunksize,
         order=order)
+
+
+def map_n_dict(func: Callable[[_T_ctr], _T],
+               obj: Mapping[_K, _T_ctr],
+               /,
+               *,
+               max_workers: int | None = None,
+               prefetch: int | None = 2,
+               mp: bool = False,
+               chunksize: int | None = None) -> dict[_K, _T]:
+    """
+    Apply `func` to each value in a mapping in parallel way.
+    For extra options, see starmap_n, which is used under hood.
+    """
+    iter_values = map_n(
+        func,
+        obj.values(),
+        max_workers=max_workers,
+        prefetch=prefetch,
+        mp=mp,
+        chunksize=chunksize)
+    return dict(zip(obj.keys(), iter_values))
```

### Comparing `glow-0.11.3/glow/core/_patch_print.py` & `glow-0.12.7/src/glow/core/_patch_print.py`

 * *Files identical despite different names*

### Comparing `glow-0.11.3/glow/core/_patch_scipy.py` & `glow-0.12.7/src/glow/core/_patch_scipy.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,35 +32,39 @@
     # Source - (stackoverflow)[https://stackoverflow.com/a/39021051/9868257]
     ptr = ctypes.c_void_p()
     ok = ctypes.windll.kernel32.VirtualProtect(
         ptr, ctypes.c_size_t(1), 0x40, ctypes.byref(ctypes.c_uint32(0)))
     if not ok or (addr := ptr.value) is None:
         return
 
-    code: bytearray = (ctypes.c_char * 3).from_address(addr)  # type: ignore
+    code: bytearray = (ctypes.c_char * 3).from_address(
+        addr)  # type: ignore[assignment]
     if not code:
         return
 
     new = b'\xC2\x08\x00' if ctypes.sizeof(ctypes.c_void_p) == 4 else b'\xC3'
     patch_size = len(new)
     old, code[:patch_size] = code[:patch_size], new
     try:
         import scipy.stats  # noqa: F401
     finally:
         code[:patch_size] = old
 
 
 def apply() -> None:
-    if (sys.platform != 'win32' or
-            _FORTRAN_FLAG in os.environ or  # Patch is already applied
-            not [*_get_conda_libs()]):  # Onle Anaconda's SciPy is affected
+    if (sys.platform != 'win32'
+            or _FORTRAN_FLAG in os.environ  # Patch is already applied
+            or not [*_get_conda_libs()]):  # Only Anaconda's SciPy is affected
         return
 
     os.environ[_FORTRAN_FLAG] = '1'  # Child will inherit this, and work fine
 
-    warnings.warn('Ctrl-C on Windows is broken when scipy is from conda. '
-                  'Please use scipy from PyPI')
+    msg = ('Ctrl-C on Windows is broken when scipy is from conda. '
+           'Please use scipy from PyPI')
+    warnings.warn(msg, stacklevel=2)
+
     if 'scipy.stats' in sys.modules:
-        warnings.warn('Cannot fix handling of Ctrl-C in current process. '
-                      'Import glow before scipy.stats to fix this.')
+        msg2 = ('Cannot fix handling of Ctrl-C in current process. '
+                'Import glow before scipy.stats to fix this.')
+        warnings.warn(msg2, stacklevel=2)
     else:
         _patch_handler_and_load_scipy()
```

### Comparing `glow-0.11.3/glow/core/_profile.pyi` & `glow-0.12.7/src/glow/core/_profile.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from collections.abc import Callable
-from typing import ContextManager, TypeVar, overload
+from contextlib import AbstractContextManager
+from typing import TypeVar, overload
 
 _F = TypeVar('_F', bound=Callable)
 
 
 def memprof(name_or_callback: str | Callable[[float], object] | None = ...,
-            /) -> ContextManager[None]:
+            /) -> AbstractContextManager[None]:
     ...
 
 
-def timer(name_or_callback: str | Callable[[float], object] | None = ...,
-          /) -> ContextManager[None]:
+def timer(name_or_callback: str | Callable[[int], object] | None = ...,
+          time: Callable[[], int] = ...,
+          /) -> AbstractContextManager[None]:
     ...
 
 
 @overload
 def time_this(fn: _F, /, *, name: str | None = ...) -> _F:
     ...
```

### Comparing `glow-0.11.3/glow/core/_reduction.py` & `glow-0.12.7/src/glow/core/_reduction.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 import mmap
 import os
 import pickle
 import sys
 import tempfile
 import weakref
 from collections.abc import Callable
-from itertools import starmap
 from multiprocessing.shared_memory import SharedMemory
 from pathlib import Path
 from typing import Generic, TypeVar
 
 import loky
 
 from ._import_hook import when_imported
@@ -44,40 +43,33 @@
                 return _SYSTEM_SHM
         except OSError:
             pass
     return _SYSTEM_TEMP
 
 
 class _Proxy(Generic[_F]):
-    uid: int
+    call: _F
 
-    def get(self) -> _F:
-        raise NotImplementedError
-
-    def __call__(self, *chunk) -> list:
-        return list(starmap(self.get(), chunk))
+    def __call__(self, *args):
+        return self.call(*args)
 
 
 class _NullProxy(_Proxy[_F]):
-    __slots__ = ('obj', 'uid')
-
-    def __init__(self, obj: _F):
-        self.obj = obj
-        self.uid = id(obj)
+    __slots__ = ('call', )
 
-    def get(self) -> _F:
-        return self.obj
+    def __init__(self, call: _F):
+        self.call = call
 
 
 class _Mmap:
     __slots__ = ('size', 'tag', 'buf', '__weakref__')
     _shm_root = _get_shm_dir()
 
     @classmethod
-    def from_bytes(cls, data: memoryview, tag: str) -> '_Mmap':
+    def from_bytes(cls, data: memoryview, tag: str) -> _Mmap:
         mv = cls(data.nbytes, f'shm-{os.getpid()}-{tag}', create=True)
         mv.buf[:] = data
         return mv
 
     def __init__(self, size, tag, create=False):
         self.size = size
         self.tag = tag
@@ -117,55 +109,66 @@
         **{
             t: torch.multiprocessing.reductions.reduce_storage
             for t in torch.storage._StorageBase.__subclasses__()
         },
     })
 
 
-def _dumps(obj: object,
-           callback: Callable[[pickle.PickleBuffer], object] = None) -> bytes:
+def _dumps(
+    obj: object,
+    callback: Callable[[pickle.PickleBuffer], object] | None = None,
+) -> bytes:
     fp = io.BytesIO()
     p = pickle.Pickler(fp, -1, buffer_callback=callback)
-    p.dispatch_table = copyreg.dispatch_table | reducers  # type: ignore
+    p.dispatch_table = copyreg.dispatch_table | reducers
     p.dump(obj)
     return fp.getvalue()
 
 
+def _mmap_reconstruct(data: bytes, memos: list[_Mmap]):
+    buffers = [m.buf for m in memos]
+    return pickle.loads(data, buffers=buffers)
+
+
 class _MmapProxy(_Proxy[_F]):
-    __slots__ = ('uid', 'root', 'memos')
+    __slots__ = ('uid', 'call', 'data', 'memos')
 
-    def __init__(self, obj: _Proxy[_F]) -> None:
+    def __init__(self, call: _F) -> None:
         buffers: list[pickle.PickleBuffer] = []
-        self.uid = obj.uid
-        self.root = _dumps(obj, callback=buffers.append)
+        self.uid = id(call)
+        self.call = call
+        self.data = _dumps(call, callback=buffers.append)
         self.memos = []
         for i, buf in enumerate(buffers):
             with buf.raw() as m:
-                self.memos += [_Mmap.from_bytes(m, f'{obj.uid:x}-{i}')]
+                self.memos += [_Mmap.from_bytes(m, f'{self.uid:x}-{i}')]
+
+    def __reduce__(self) -> tuple:
+        return _mmap_reconstruct, (self.data, self.memos)
+
 
-    def get(self) -> _F:
-        buffers = [m.buf for m in self.memos]
-        return pickle.loads(self.root, buffers=buffers)
+def _shn_reconstruct(data: bytes, memos: list[tuple[SharedMemory, int]]):
+    buffers = [sm.buf[:size] for sm, size in memos]
+    return pickle.loads(data, buffers=buffers)
 
 
 class _ShmemProxy(_Proxy[_F]):
-    __slots__ = ('uid', 'root', 'memos')
+    __slots__ = ('call', 'data', 'memos')
 
-    def __init__(self, obj: _Proxy[_F]) -> None:
+    def __init__(self, call: _F) -> None:
         buffers: list[pickle.PickleBuffer] = []
-        self.uid = obj.uid
-        self.root = _dumps(obj, callback=buffers.append)
+        self.call = call
+        self.data = _dumps(call, callback=buffers.append)
         self.memos = []
         for buf in buffers:
             with buf.raw() as m:
                 sm = SharedMemory(create=True, size=m.nbytes)
                 sm.buf[:] = m
                 self.memos.append((sm, sm.size))
 
-    def get(self) -> _F:
-        buffers = [sm.buf[:size] for sm, size in self.memos]
-        return pickle.loads(self.root, buffers=buffers)
+    def __reduce__(self) -> tuple:
+        return _shn_reconstruct, (self.data, self.memos)
 
 
-def move_to_shmem(fn: Callable[..., _T]) -> Callable[..., list[_T]]:
+def move_to_shmem(fn: Callable[..., _T]) -> Callable[..., _T]:
     return _NullProxy(fn)
     return _ShmemProxy(fn)
```

### Comparing `glow-0.11.3/glow/core/_repr.py` & `glow-0.12.7/src/glow/core/_repr.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     >>> mangled('a')
     'a'
     >>> mangled('b')
     'b'
     >>> mangled('a')
     'a:1'
     """
-    store: Counter[str] = Counter()
+    store = Counter[str]()
 
     def call(name: str) -> str | None:
         if name is None:
             return None
 
         seen = store[name]
         store[name] += 1
@@ -68,15 +68,15 @@
 
 def _find_prefix(value: float | int, base: int,
                  prefixes: str) -> tuple[float, str]:
     threshold = base - 0.5
     origin = prefixes.find(' ') + 1
     value *= base ** origin
 
-    for prefix in prefixes:  # noqa: B007
+    for prefix in prefixes:
         value /= base
         if -threshold < value < threshold:
             return value, prefix
 
     return value, prefixes[-1]
```

### Comparing `glow-0.11.3/glow/core/_sizeof.py` & `glow-0.12.7/src/glow/core/_sizeof.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,14 +35,18 @@
     return functools.update_wrapper(wrapper, fn)
 
 
 def true_vars(obj) -> dict[str, object] | None:
     """Get instance's vars(), even it's hidden.
 
     Inspired by [magic_get_dict](https://stackoverflow.com/a/45315745/9868257)
+
+    For more details see:
+    - https://utcc.utoronto.ca/~cks/space/blog/python/HowSlotsWorkI
+    - https://utcc.utoronto.ca/~cks/space/blog/python/DictoffsetNotes
     """
     tp = type(obj)
 
     if sys.implementation.name == 'cpython':
         if (ptr := pythonapi._PyObject_GetDictPtr(obj)) and ptr.contents:
             return ptr.contents.value
         return None
@@ -54,16 +58,16 @@
         #     ptr = ctypes.cast(addr, ctypes.POINTER(ctypes.py_object))
         #     return ptr.contents.value
         # return None
 
     if hasattr(obj, '__dict__'):
         for cls in tp.__mro__:
             if (attr := vars(cls).get('__dict__')) is not None:
-                return (vars(obj) if (isgetsetdescriptor(attr) or
-                                      ismemberdescriptor(attr)) else None)
+                return (vars(obj) if (isgetsetdescriptor(attr)
+                                      or ismemberdescriptor(attr)) else None)
     return None
 
 
 @functools.singledispatch
 @unique_only
 def _sizeof(obj, seen: set[int]) -> int:
     if obj is None:
@@ -80,15 +84,15 @@
     size += _sizeof(true_vars(obj), seen)
 
     if hasattr(obj, '__wrapped__'):  # Unwrap
         size += _sizeof(obj.__wrapped__, seen)
         return size
 
     if issubclass(tp, dict):
-        size += sum(_sizeof(k, seen) for k in obj.keys())
+        size += sum(_sizeof(k, seen) for k in obj)
         size += sum(_sizeof(v, seen) for v in obj.values())
     elif issubclass(tp, abc.Collection):
         size += sum(_sizeof(item, seen) for item in obj)
 
     if hasattr(obj, '__slots__'):
         size += sum(
             _sizeof(getattr(obj, slot, None), seen)
```

### Comparing `glow-0.11.3/glow/core/_uuid.py` & `glow-0.12.7/src/glow/core/_uuid.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 def base57_encode(number: int) -> str:
     out = bytearray(_LEN)
     for i in range(_LEN - 1, -1, -1):
         number, out[i] = divmod(number, _BASE)
     return out.translate(_TABLE).decode('ascii')
 
 
+@lru_cache  # Small performance optimization
 def base57_decode(shortuuid: str) -> int:
     if not _REGEX.fullmatch(shortuuid):
         raise ValueError('invalid shortuuid format')
     out = 0
     for char in shortuuid:
         out = out * _BASE + _NUMBERS[char]
     return out
@@ -67,33 +68,33 @@
     """
     def __init__(self, obj: str | SupportsInt):
         """
         Creates Uid either from str (parsing it as short-uuid) or
         from int()-compatible type
         """
         if not isinstance(obj, (str, SupportsInt)):
-            raise ValueError('Either int, string or UUID required. '
-                             f'Got {type(obj)}')
+            raise TypeError('Either int, string or UUID required. '
+                            f'Got {type(obj)}')
 
         value = base57_decode(obj) if isinstance(obj, str) else int(obj)
         super().__init__(int=value)
 
     def __str__(self) -> str:
         return base57_encode(int(self))
 
     @classmethod
     def __get_validators__(cls):  # Required for Pydantic
         yield cls
 
     @classmethod
-    def __modify_schema__(cls, field_schema):  # Required for OpenAPI
-        field_schema |= {
-            'examples': [str(cls.v4()) for _ in range(2)],
-            'type': 'string',
-            'format': None,
-            'pattern': _REGEX.pattern,
-        }
+    def __modify_schema__(cls, field_schema: dict):  # Required for OpenAPI
+        field_schema.update(
+            examples=[str(cls.v4()) for _ in range(2)],
+            type='string',
+            format=None,
+            pattern=_REGEX.pattern,
+        )
 
     @classmethod
     def v4(cls) -> Uid:
         """Alias for Uid(uuid.uuid4())"""
         return cls(uuid4())
```

### Comparing `glow-0.11.3/glow/core/wrap/cache.py` & `glow-0.12.7/src/glow/core/wrap/cache.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,45 +1,48 @@
 from __future__ import annotations
 
 __all__ = ['memoize']
 
-# TODO: add case capacity=None for unbound cache
-
 import argparse
 import asyncio
 import concurrent.futures as cf
 import enum
 import functools
 from collections import Counter
-from collections.abc import (Callable, Hashable, KeysView, MutableMapping,
-                             Sequence)
+from collections.abc import (Callable, Hashable, Iterable, KeysView,
+                             MutableMapping)
 from contextlib import ExitStack
 from dataclasses import dataclass, field
 from threading import RLock
 from typing import (Any, ClassVar, Generic, Literal, NamedTuple, SupportsInt,
                     TypeVar, cast)
 from weakref import WeakValueDictionary
 
 from .._repr import si_bin
 from .._sizeof import sizeof
 from .reusable import make_loop
+from .util import make_key
 
 
 class _Empty(enum.Enum):
     token = 0
 
 
 _T = TypeVar('_T')
 _F = TypeVar('_F', bound=Callable)
-_Fbatch = TypeVar('_Fbatch', bound=Callable[[Sequence], list])
+_BatchedFn = TypeVar('_BatchedFn', bound=Callable[[list], Iterable])
 _Policy = Literal['raw', 'lru', 'mru']
 _KeyFn = Callable[..., Hashable]
 _empty = _Empty.token
 
 
+def _unit_size(x):
+    return 1
+
+
 @dataclass(repr=False)
 class _Node(Generic[_T]):
     __slots__ = ('value', 'size')
     value: _T
     size: int
 
     def __repr__(self) -> str:
@@ -64,28 +67,29 @@
 
     def store_get(self, key: Hashable) -> _Node[_T] | None:
         raise NotImplementedError
 
     def store_set(self, key: Hashable, node: _Node[_T]) -> None:
         raise NotImplementedError
 
-    def can_swap(self, size: int) -> bool:
+    def can_shrink_for(self, size: int) -> bool:
         raise NotImplementedError
 
 
 @dataclass(repr=False)
 class _InitializedStore:
     capacity: int
-    size: int = 0
-    stats: Stats = field(default_factory=Stats)
+    size_fn: Callable[[object], int]
+    size: int = field(default=0, init=False)
+    stats: Stats = field(default_factory=Stats, init=False)
 
 
 @dataclass(repr=False)
 class _DictMixin(_InitializedStore, _IStore[_T]):
-    lock: RLock = field(default_factory=RLock)
+    lock: RLock = field(default_factory=RLock, init=False)
 
     def clear(self):
         with self.lock:
             self.store_clear()
             self.size = 0
 
     def keys(self) -> KeysView:
@@ -97,16 +101,18 @@
                 self.stats.hits += 1
                 return node.value
         return _empty
 
     def __setitem__(self, key: Hashable, value: _T) -> None:
         with self.lock:
             self.stats.misses += 1
-            size = int(sizeof(value))
-            if (self.size + size <= self.capacity) or self.can_swap(size):
+            size = int(self.size_fn(value))
+            if (self.capacity < 0  # is unbound
+                    or self.size + size <= self.capacity  # has free place
+                    or (size < self.capacity and self.can_shrink_for(size))):
                 self.store_set(key, _Node(value, size))
                 self.size += size
 
 
 @dataclass(repr=False)
 class _ReprMixin(_InitializedStore, _IStore[_T]):
     refs: ClassVar[MutableMapping[int, _ReprMixin]] = WeakValueDictionary()
@@ -147,32 +153,30 @@
         return self.store.get(key)
 
     def store_set(self, key: Hashable, node: _Node[_T]) -> None:
         self.store[key] = node
 
 
 class _HeapCache(_Store[_T]):
-    def can_swap(self, size: int) -> bool:
+    def can_shrink_for(self, size: int) -> bool:
         return False
 
 
 class _LruCache(_Store[_T]):
     drop_recent = False
 
     def store_get(self, key: Hashable) -> _Node[_T] | None:
         if node := self.store.pop(key, None):
             self.store[key] = node
             return node
         return None
 
-    def can_swap(self, size: int) -> bool:
-        if size > self.capacity:
-            return False
-
-        while self.size + size > self.capacity:
+    def can_shrink_for(self, size: int) -> bool:
+        size = 0
+        while self.store and self.size + size > self.capacity:
             if self.drop_recent:
                 self.size -= self.store.popitem()[1].size
             else:
                 self.size -= self.store.pop(next(iter(self.store))).size
             self.stats.dropped += 1
         return True
 
@@ -187,48 +191,52 @@
 def _memoize(cache: _DictMixin, key_fn: _KeyFn, fn: _F) -> _F:
     def wrapper(*args, **kwargs):
         key = key_fn(*args, **kwargs)
 
         if (value := cache[key]) is not _empty:
             return value
 
+        # NOTE: fn() is not within lock
         cache[key] = value = fn(*args, **kwargs)
         return value
 
-    wrapper.cache = cache  # type: ignore
+    wrapper.cache = cache  # type: ignore[attr-defined]
     return cast(_F, functools.update_wrapper(wrapper, fn))
 
 
 # ----------------------- wrapper with batching support ----------------------
 
 
 class _Job(NamedTuple):
     token: Any
     future: asyncio.Future | cf.Future
 
 
-def _dispatch(fn: Callable[[Sequence], list], cache: dict[Hashable, object],
-              queue: dict[Hashable, _Job]) -> None:
+def _dispatch(
+    fn: Callable[[list], Iterable],
+    evict: Callable[[Hashable], object],
+    queue: dict[Hashable, _Job],
+):
     jobs = {**queue}
     queue.clear()
 
     try:
-        values = fn([job.token for job in jobs.values()])
+        *values, = fn([job.token for job in jobs.values()])
         assert len(values) == len(jobs)
 
         for job, value in zip(jobs.values(), values):
             job.future.set_result(value)
 
-    except BaseException as exc:  # noqa: PIE786
+    except BaseException as exc:  # noqa: BLE001
         for key, job in jobs.items():
-            cache.pop(key)
+            evict(key)
             job.future.set_exception(exc)
 
 
-def _memoize_batched_aio(key_fn: _KeyFn, fn: _Fbatch) -> _Fbatch:
+def _memoize_batched_aio(key_fn: _KeyFn, fn: _BatchedFn) -> _BatchedFn:
     assert callable(fn)
     cache: dict[Hashable, asyncio.Future] = {}
     queue: dict[Hashable, _Job] = {}
     loop = make_loop()
 
     def _load(token) -> asyncio.Future:
         key = key_fn(token)
@@ -239,100 +247,87 @@
         cache[key] = future = loop.create_future()
         queue[key] = _Job(token, future)
         if len(queue) == 1:
             loop.call_soon(_dispatch, fn, cache, queue)
 
         return future
 
-    async def _load_many(tokens: Sequence) -> list:
-        return list(await asyncio.gather(*map(_load, tokens)))
+    async def _load_many(tokens: Iterable) -> tuple:
+        return await asyncio.gather(*map(_load, tokens))
 
-    def wrapper(tokens: Sequence) -> list:
+    def wrapper(tokens: Iterable) -> tuple:
         coro = _load_many(tokens)
         return asyncio.run_coroutine_threadsafe(coro, loop).result()
 
-    wrapper.cache = cache  # type: ignore
-    return cast(_Fbatch, functools.update_wrapper(wrapper, fn))
+    wrapper.cache = cache  # type: ignore[attr-defined]
+    return cast(_BatchedFn, functools.update_wrapper(wrapper, fn))
 
 
-def _memoize_batched(key_fn: _KeyFn, fn: _Fbatch) -> _Fbatch:
+def _memoize_batched(key_fn: _KeyFn, fn: _BatchedFn) -> _BatchedFn:
     assert callable(fn)
     lock = RLock()
     cache: dict[Hashable, cf.Future] = {}
     queue: dict[Hashable, _Job] = {}
 
-    def _load(stack: ExitStack, token: Any) -> cf.Future:
+    def _load(stack: ExitStack, token: object) -> cf.Future:
         key = key_fn(token)
         with lock:
             if result := cache.get(key):
                 return result
 
-            cache[key] = future = cf.Future()  # type: ignore
+            cache[key] = future = cf.Future()  # type: ignore[var-annotated]
             queue[key] = _Job(token, future)
             if len(queue) == 1:
-                stack.callback(_dispatch, fn, cache, queue)
+                stack.callback(_dispatch, fn, cache.pop, queue)
 
         return future
 
-    def wrapper(tokens: Sequence) -> list:
+    def wrapper(tokens: Iterable) -> list:
+        futs = []
         with ExitStack() as stack:
-            futs = [_load(stack, token) for token in tokens]
+            futs += [_load(stack, token) for token in tokens]
         return [fut.result() for fut in futs]
 
-    wrapper.cache = cache  # type: ignore
-    return cast(_Fbatch, functools.update_wrapper(wrapper, fn))
+    wrapper.cache = cache  # type: ignore[attr-defined]
+    return cast(_BatchedFn, functools.update_wrapper(wrapper, fn))
 
 
 # ----------------------------- factory wrappers -----------------------------
 
-_KWD_MARK = object()
-
-
-class _HashedSeq(list):  # List is mutable, that's why not NamedTuple
-    __slots__ = 'hashvalue',
-
-    def __init__(self, tup: tuple):
-        self[:] = tup
-        self.hashvalue = hash(tup)  # Memorize hash
-
-    def __hash__(self):
-        return self.hashvalue
-
-
-def _make_key(*args, **kwargs) -> Hashable:
-    """Copied from functools._make_key, as private function"""
-    if len(args) == 1 and isinstance(args[0], (int, str)):
-        return args[0]
-    if kwargs:
-        args = sum(kwargs.items(), (*args, _KWD_MARK))
-    return _HashedSeq(args)
-
 
 def memoize(
-    capacity: SupportsInt,
+    capacity: SupportsInt | None,
     *,
     batched: bool = False,
     policy: _Policy = 'raw',
-    key_fn: _KeyFn = _make_key,
-) -> Callable[[_F], _F] | Callable[[_Fbatch], _Fbatch]:
+    key_fn: _KeyFn = make_key,
+    bytesize: bool = True,
+) -> Callable[[_F], _F] | Callable[[_BatchedFn], _BatchedFn]:
     """Returns dict-cache decorator.
 
     Parameters:
-    - capacity - size in bytes.
+    - capacity - max size in bytes if `bytesize` is set, otherwise objects.
+      Cache is unbound if None set.
     - policy - eviction policy, either "raw" (no eviction), or "lru"
       (evict oldest), or "mru" (evict most recent).
+    - bytesize - if set limits bytes, not objects.
     """
-    capacity = int(capacity)
-    if not capacity:
+    capacity = int(capacity) if capacity is not None else -1
+    if capacity == 0:
         return lambda fn: fn
 
     caches: dict[str, type[_Store]] = {
         'raw': _HeapCache,
         'lru': _LruCache,
         'mru': _MruCache,
     }
+    size_fn = sizeof if bytesize else _unit_size
+
     if (cache_cls := caches.get(policy)) is not None:
         if batched:
             return functools.partial(_memoize_batched, key_fn)
-        return functools.partial(_memoize, cache_cls(capacity), key_fn)
+        if capacity < 0:
+            cache_cls = _HeapCache
+        return functools.partial(_memoize, cache_cls(capacity, size_fn),
+                                 key_fn)
     raise ValueError(f'Unknown policy: "{policy}". '
                      f'Only "{set(caches)}" are available')
```

### Comparing `glow-0.11.3/glow/core/wrap/concurrency.py` & `glow-0.12.7/src/glow/nn/modules/simple.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,142 +1,160 @@
-__all__ = ['stream_batched', 'call_once', 'threadlocal', 'shared_call']
+__all__ = [
+    'Bias2d', 'BlurPool2d', 'Conv2dWs', 'Decimate2d', 'Noise', 'Upscale2d'
+]
 
-import functools
-import threading
-import time
-from collections.abc import Callable, Sequence
-from concurrent.futures import Future
-from contextlib import ExitStack
-from queue import Empty, SimpleQueue
-from threading import Thread
-from typing import Any, TypeVar, cast
-from weakref import WeakValueDictionary
-
-_T = TypeVar('_T')
-_F = TypeVar('_F', bound=Callable)
-_ZeroArgsF = TypeVar('_ZeroArgsF', bound=Callable[[], Any])
-
-
-def threadlocal(fn: Callable[..., _T], *args: object,
-                **kwargs: object) -> Callable[[], _T]:
-    """Thread-local singleton factory, mimics `functools.partial`"""
-    local_ = threading.local()
-
-    def wrapper() -> _T:
-        try:
-            return local_.obj
-        except AttributeError:
-            local_.obj = fn(*args, **kwargs)
-            return local_.obj
+from string import ascii_lowercase
+from typing import Optional
 
-    return wrapper
+import torch
+import torch.nn.functional as TF
+from torch import nn
 
+from .. import functional as F
+
+
+class Noise(nn.Module):
+    __constants__ = ['std']
+
+    def __init__(self, std: float):
+        super().__init__()
+        self.std = std
+
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
+        if not self.training:
+            return x
+        return torch.empty_like(x).normal_(std=self.std).add_(x)
+
+    def extra_repr(self) -> str:
+        return f'std={self.std}'
 
-class _DeferredStack(ExitStack):
-    """
-    ExitStack that allows deferring.
-    When return value of callback function should be accessible, use this.
-    """
-    def defer(self, fn: Callable[..., _T], *args, **kwargs) -> Future[_T]:
-        future: Future[_T] = Future()
 
-        def apply(future: Future[_T]) -> None:
-            try:
-                result = fn(*args, **kwargs)
-            except BaseException as exc:  # noqa: PIE786
-                future.set_exception(exc)
-            else:
-                future.set_result(result)
+class Bias2d(nn.Module):
+    def __init__(self,
+                 dim: int,
+                 *size: int,
+                 device: Optional[torch.device] = None):
+        super().__init__()
+        assert len(size) == 2
+        self.bias = nn.Parameter(torch.empty(1, dim, *size, device=device))
+        self.reset_parameters()
 
-        self.callback(apply, future)
-        return future
+    def reset_parameters(self):
+        nn.init.normal_(self.bias)
 
+    def extra_repr(self) -> str:
+        _, dim, *space = self.bias.shape
+        return f'features={dim}, size={tuple(space)}'
 
-def call_once(fn: _ZeroArgsF) -> _ZeroArgsF:
-    """Makes `fn()` callable a singleton"""
-    lock = threading.RLock()
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
+        bias = self.bias
+        size = [x.shape[2], x.shape[3]]
 
-    def wrapper():
-        with _DeferredStack() as stack, lock:
-            if fn._future is None:
-                # This way setting future is protected, but fn() is not
-                fn._future = stack.defer(fn)
+        if torch.jit.is_tracing() or bias.shape[2:] != size:
+            # Stretch to input size
+            bias = TF.interpolate(
+                bias, size, mode='bicubic', align_corners=False)
 
-        return fn._future.result()
+        return x + bias
 
-    fn._future = None  # type: ignore
-    return cast(_ZeroArgsF, functools.update_wrapper(wrapper, fn))
 
+class Decimate2d(nn.Module):
+    __constants__ = ['stride']
 
-def shared_call(fn: _F) -> _F:
-    """Merges concurrent calls to `fn` with the same `args` to single one"""
-    lock = threading.RLock()
-    futures: WeakValueDictionary[str, Future] = WeakValueDictionary()
+    def __init__(self, stride: int = 2):
+        super().__init__()
+        self.stride = stride
 
-    def wrapper(*args, **kwargs):
-        key = f'{fn}{args}{kwargs}'
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
+        return x[:, :, ::self.stride, ::self.stride]
 
-        with _DeferredStack() as stack, lock:
-            try:
-                future = futures[key]
-            except KeyError:
-                futures[key] = future = stack.defer(fn, *args, **kwargs)
+    def extra_repr(self) -> str:
+        return f'stride={self.stride}'
 
-        return future.result()
 
-    return cast(_F, functools.update_wrapper(wrapper, fn))
+class Upscale2d(nn.Module):
+    """Upsamples input tensor in `scale` times.
+    Use as inverse for `nn.Conv2d(kernel=3, stride=2)`.
 
+    There're 2 different methods:
 
-def _batch_apply(func: Callable, args: Sequence, futures: Sequence[Future]):
-    try:
-        results = func(args)
-        assert len(args) == len(results)
-    except BaseException as exc:  # noqa: PIE786
-        for fut in futures:
-            fut.set_exception(exc)
-    else:
-        for fut, res in zip(futures, results):
-            fut.set_result(res)
+    - Pixels are thought as squares. Aligns the outer edges of the outermost
+      pixels.
+      Used in `torch.nn.Upsample(align_corners=True)`.
 
+    - Pixels are thought as points. Aligns centers of the outermost pixels.
+      Avoids the need to extrapolate sample values that are outside of any of
+      the existing samples.
+      In this mode doubling number of pixels doesn't exactly double size of the
+      objects in the image.
 
-def stream_batched(func=None, *, batch_size, latency=0.1, timeout=20.):
+    This module implements the second way (match centers).
+    New image size will be computed as follows:
+        `destination size = (source size - 1) * scale + 1`
+
+    For comparison see [here](http://entropymine.com/imageworsener/matching).
     """
-    Delays start of computation up to `latency` seconds
-    in order to fill batch to batch_size items and
-    send it at once to target function.
-    `timeout` specifies timeout to wait results from worker.
+    __constants__ = ['stride']
+
+    def __init__(self, stride: int = 2):
+        super().__init__()
+        self.stride = stride
+
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
+        return F.upscale2d(x, self.stride)
 
-    Simplified version of https://github.com/ShannonAI/service-streamer
+    def extra_repr(self):
+        return f'stride={self.stride}'
+
+
+class Conv2dWs(nn.Conv2d):
+    """
+    [Weight standartization](https://arxiv.org/pdf/1903.10520.pdf).
+    Better use with GroupNorm(32, features).
     """
-    if func is None:
-        return functools.partial(
-            stream_batched,
-            batch_size=batch_size,
-            latency=latency,
-            timeout=timeout)
-
-    assert callable(func)
-    buf = SimpleQueue()
-
-    def _fetch_batch():
-        end_time = time.monotonic() + latency
-        for _ in range(batch_size):
-            try:
-                yield buf.get(timeout=end_time - time.monotonic())
-            except (Empty, ValueError):  # ValueError on negative timeout
-                return
-
-    def _serve_forever():
-        while True:
-            if batch := [*_fetch_batch()]:
-                _batch_apply(func, *zip(*batch))
-            else:
-                time.sleep(0.001)
-
-    def wrapper(batch):
-        futures = [Future() for _ in batch]
-        for item, fut in zip(batch, futures):
-            buf.put((item, fut))
-        return [f.result(timeout=timeout) for f in futures]
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
+        return F.conv2d_ws(x, self.weight, self.bias, self.stride,
+                           self.padding, self.dilation, self.groups)
+
+
+# --------------------------------- blurpool ---------------------------------
+
+
+def _pascal_triangle(n: int) -> list[int]:
+    values = [1]
+    for _ in range(n - 1):
+        values = [a + b for a, b in zip([*values, 0], [0, *values])]
+    return values[:n]
+
+
+def _outer_mul(*ts: torch.Tensor) -> torch.Tensor:
+    assert all(t.ndim == 1 for t in ts)
+    letters = ascii_lowercase[:len(ts)]
+    return torch.einsum(','.join(letters) + ' -> ' + letters, *ts)
+
+
+class BlurPool2d(nn.Conv2d):
+    def __init__(self,
+                 dim: int,
+                 kernel: int = 4,
+                 stride: int = 2,
+                 padding: int = 1,
+                 padding_mode: str = 'reflect'):
+        super().__init__(dim, dim, kernel, stride, padding, 1, dim, False,
+                         padding_mode)
+        del self.weight
+        self.register_buffer(
+            'weight', torch.empty(dim, 1, kernel, kernel), persistent=False)
+        self.reset_parameters()
+
+    def reset_parameters(self) -> None:
+        if not self.in_channels:
+            return
+
+        weights = [
+            torch.as_tensor(_pascal_triangle(k)).float()
+            for k in self.kernel_size
+        ]
+        weight = _outer_mul(*weights)
+        weight /= weight.sum()
 
-    Thread(target=_serve_forever, daemon=True).start()
-    return functools.update_wrapper(wrapper, func)
+        self.weight.copy_(weight, non_blocking=True)
```

### Comparing `glow-0.11.3/glow/core/wrap/concurrency.pyi` & `glow-0.12.7/src/glow/core/wrap/concurrency.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,50 @@
-from typing import Callable, ContextManager, Sequence, TypeVar, overload
+from collections.abc import Callable, Iterable
+from contextlib import AbstractContextManager
+from typing import TypeVar, overload
+
+from typing_extensions import ParamSpec
 
 _T = TypeVar('_T')
 _F = TypeVar('_F', bound=Callable)
-_BatchF = TypeVar('_BatchF', bound=Callable[[Sequence], list])
+_P = ParamSpec('_P')
+_BatchedFn = TypeVar('_BatchedFn', bound=Callable[[list], Iterable])
+
+
+def threadlocal(fn: Callable[_P, _T], *args: _P.args,
+                **kwargs: _P.kwargs) -> Callable[[], _T]:
+    ...
 
 
-def threadlocal(fn: Callable[..., _T], *args: object,
-                **kwargs: object) -> Callable[[], _T]:
+def interpreter_lock(timeout: float = ...) -> AbstractContextManager[None]:
     ...
 
 
-def interpreter_lock(timeout: float = ...) -> ContextManager[None]:
+def call_once(fn: _F, /) -> _F:
     ...
 
 
-def call_once(fn: _F) -> _F:
+def shared_call(fn: _F, /) -> _F:
     ...
 
 
-def shared_call(fn: _F) -> _F:
+def weak_memoize(fn: _F, /) -> _F:
     ...
 
 
 @overload
-def stream_batched(*,
-                   batch_size: int,
-                   latency: float = ...,
-                   timeout: float = ...) -> Callable[[_BatchF], _BatchF]:
+def streaming(*,
+              batch_size: int,
+              timeout: float = ...,
+              workers: int = ...,
+              pool_timeout: float = ...) -> Callable[[_BatchedFn], _BatchedFn]:
     ...
 
 
 @overload
-def stream_batched(func: _BatchF,
-                   *,
-                   batch_size: int,
-                   latency: float = ...,
-                   timeout: float = ...) -> _BatchF:
+def streaming(func: _BatchedFn,
+              *,
+              batch_size: int,
+              timeout: float = ...,
+              workers: int = ...,
+              pool_timeout: float = ...) -> _BatchedFn:
     ...
```

### Comparing `glow-0.11.3/glow/core/wrap/reusable.py` & `glow-0.12.7/src/glow/core/wrap/reusable.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 import asyncio
 import sys
 import weakref
 from collections.abc import Callable
 from dataclasses import dataclass, field
 from functools import partial
 from threading import Thread
-from typing import Any, Generic, TypeVar
+from typing import Generic, TypeVar
 
 from .concurrency import call_once
 
 _T = TypeVar('_T')
 _Make = Callable[[], _T]
-_Callback = Callable[[_T], Any]
+_Callback = Callable[[_T], object]
 
 
 @call_once
 def make_loop() -> asyncio.AbstractEventLoop:
     loop = asyncio.new_event_loop()
     Thread(target=loop.run_forever, daemon=True).start()
     return loop
```

### Comparing `glow-0.11.3/glow/distributed.py` & `glow-0.12.7/src/glow/distributed.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,74 +1,67 @@
 from __future__ import annotations
 
 __all__ = [
-    'auto_ddp', 'auto_model', 'barrier', 'get_rank', 'get_world_size',
-    'reduce_if_needed'
+    'auto_ddp', 'auto_model', 'barrier', 'get_ddp_info', 'reduce_if_needed'
 ]
 
 import pickle
 from collections.abc import Callable
 from functools import partial, update_wrapper
 from pathlib import Path
-from typing import Any, Protocol, TypeVar, cast
+from typing import Any, NamedTuple, Protocol, TypeVar, cast
 
 import torch
 import torch.cuda
 import torch.distributed as dist
 import torch.multiprocessing as tmp
 from torch import nn
 
 # -------------------------------- primitives --------------------------------
 
 
-def get_rank() -> int:
-    """
-    In distributed context returns the rank of current process group. otherwise
-    returns -1.
-    """
-    return dist.get_rank() if dist.is_initialized() else -1
+class _DdpInfo(NamedTuple):
+    world: int
+    rank: int
 
 
-def get_world_size() -> int:
-    """
-    In distributed context returns number of processes in the current process
-    group, otherwise returns 0.
-    """
-    return dist.get_world_size() if dist.is_initialized() else 0
+def get_ddp_info() -> _DdpInfo | None:
+    if not dist.is_initialized():
+        return None
+    return _DdpInfo(dist.get_rank(), dist.get_world_size())
 
 
 def barrier(rank: int | None = None) -> None:
     """Synchronize all processes"""
-    if get_world_size() > 1 and (rank is None or rank == get_rank()):
+    if (info := get_ddp_info()) and (rank is None or rank == info.rank):
         dist.barrier()
 
 
 def reduce_if_needed(*tensors: torch.Tensor,
                      mean: bool = False) -> tuple[torch.Tensor, ...]:
     """Reduce tensors across all machines"""
-    if (world := get_world_size()) > 1:
+    if (ddp := get_ddp_info()) and ddp.world > 1:
         tensors = *(t.clone() for t in tensors),
-        for op in [dist.all_reduce(t, async_op=True) for t in tensors]:
-            op.wait()
+        dist.all_reduce_multigpu(tensors)
         if mean:
-            tensors = *(t / world for t in tensors),
+            tensors = *(t / ddp.world for t in tensors),
     return tensors
 
 
 # --------------------------------- wrappers ---------------------------------
 
 
 def auto_model(net: nn.Module, sync_bn: bool = True) -> nn.Module:
-    if (rank := get_rank()) >= 0:
-        torch.cuda.set_device(rank)
+    if (ddp := get_ddp_info()) and ddp.world > 1:
+        torch.cuda.set_device(ddp.rank)
 
-        net.to(rank)
+        net.to(ddp.rank)
         if sync_bn:
             net = nn.SyncBatchNorm.convert_sync_batchnorm(net)
-        return nn.parallel.DistributedDataParallel(net, device_ids=[rank])
+        return nn.parallel.DistributedDataParallel(net, device_ids=[ddp.rank])
 
     net.cuda()
     return (nn.parallel.DataParallel(net)
             if torch.cuda.device_count() > 1 else net)
 
 
 class _TrainFn(Protocol):
@@ -117,38 +110,39 @@
     return cast(_TrainFnType,
                 update_wrapper(partial(_AutoDdp, train_fn), train_fn))
 
 
 def once_per_world(fn: _F) -> _F:
     """Call function only in rank=0 process, and share result for others"""
     def wrapper(*args, **kwargs):
-        rank = get_rank()
-        world = get_world_size()
+        ddp = get_ddp_info()
+        if not ddp or ddp.world == 1:
+            # Master process, so no neighbors to share results with
+            return fn(*args, **kwargs)
 
         # Generate random fname and share it among whole world
         idx = torch.empty((), dtype=torch.int64).random_()
-        if rank == 0:
+        if ddp.rank == 0:
             dist.broadcast(idx, 0)
+
         tmp = Path(f'/tmp/_ddp_share_{idx.item():x}.pkl')
         result = None
 
-        if rank <= 0:  # master
+        if ddp.rank == 0:  # 0th child
             result = fn(*args, **kwargs)
-            if world <= 1:
-                return result  # only master exists
             with tmp.open('wb') as fp:
                 pickle.dump(result, fp)
 
         barrier()
 
-        if rank > 0:  # slave, here must be IPC with PickleBuffers, i.e. reduce
+        if ddp.rank > 0:  # Gather results from 0th child
             with tmp.open('rb') as fp:
                 result = pickle.load(fp)
 
         barrier()
 
-        if rank == 0 and world > 1:  # parent
+        if ddp.rank == 0:  # 0th child
             tmp.unlink()
 
         return result
 
     return cast(_F, update_wrapper(wrapper, fn))
```

### Comparing `glow-0.11.3/glow/examples/cifar10.py` & `glow-0.12.7/examples/cifar10.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,15 +120,15 @@
 metrics = [
     m.Lambda(criterion, name='loss'),
     m.Confusion(acc=m.accuracy, kappa=m.kappa),
 ]
 stepper = gnn.Stepper(
     net, opt, criterion, metrics, device=DEVICE, fp16=args.fp16)
 
-history: defaultdict[str, list] = defaultdict(list)
+history = defaultdict[str, list](list)
 with tqdm(total=epoch_len * args.epochs, desc='train') as pbar:
     for i, split in enumerate(glow.ichunked(loader, epoch_len), 1):
         tscalars = stepper.run(split, pbar).scalars
         with tqdm(total=len(val_loader), desc='val', leave=False) as pbar_val:
             vscalars = stepper.run(val_loader, pbar_val, False).scalars
 
         _tags = sorted({*tscalars, *vscalars})
```

### Comparing `glow-0.11.3/glow/io/_sound.py` & `glow-0.12.7/src/glow/io/_sound.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 from __future__ import annotations
 
 __all__ = ['Sound']
 
 from contextlib import ExitStack
-from dataclasses import dataclass, field
+from dataclasses import dataclass
 from datetime import timedelta
 from pathlib import Path
 from queue import Queue
 from threading import Event
+from typing import Generic, TypeVar
 
 import numpy as np
+import numpy.typing as npt
 from tqdm.auto import tqdm
 
-from .. import sliced
+from .. import chunked
+
+_Scalar = TypeVar('_Scalar', bound=np.generic, covariant=True)
 
 
 def _play(arr: np.ndarray,
           rate: int,
           blocksize: int = 1024,
           bufsize: int = 20):
     """Plays audio from array. Supports interruption via Crtl-C."""
@@ -35,28 +39,28 @@
             out[size:] = 0
             raise sd.CallbackStop
 
     stream = sd.OutputStream(
         rate, blocksize, callback=callback, finished_callback=ev.set)
 
     fmt = '{percentage:3.0f}% |{bar}| [{elapsed}<{remaining}]'
-    blocks = sliced(arr, blocksize)
+    blocks = chunked(arr, blocksize)
 
-    with ExitStack() as stack:
-        stack.enter_context(stream)  # Close stream
-        stack.callback(ev.wait)  # Wait for completion
-        stack.callback(q.put, None)  # Close queue
+    with ExitStack() as s:
+        s.enter_context(stream)  # Close stream
+        s.callback(ev.wait)  # Wait for completion
+        s.callback(q.put, None)  # Close queue
 
-        for data in stack.enter_context(
+        for data in s.enter_context(
                 tqdm(blocks, leave=False, smoothing=0, bar_format=fmt)):
             q.put(data)
 
 
-@dataclass(repr=False)
-class Sound:
+@dataclass(repr=False, frozen=True)
+class Sound(Generic[_Scalar]):
     """Wraps numpy.array to be playable as sound
 
     Parameters:
     - rate - sample rate to use for playback
 
     Usage:
     ```
@@ -78,40 +82,44 @@
     # Extract underlying array
     raw = sound.raw
 
     # Same result
     raw = np.array(sound)
     ```
     """
-    raw: np.ndarray
+    data: npt.NDArray[_Scalar]
     rate: int = 44_100
-    duration: timedelta = field(init=False)
-    channels: int = field(init=False)
 
     def __post_init__(self):
-        assert self.raw.ndim == 2
-        assert 0 < self.raw.shape[-1] <= 2
-        assert self.raw.dtype in {'int8', 'int16', 'int32', 'float32'}
-        num_samples, self.channels = self.raw.shape
-        self.duration = timedelta(seconds=num_samples / self.rate)
+        assert self.data.ndim == 2
+        assert self.data.shape[-1] in (1, 2)
+        assert self.data.dtype in ('i1', 'i2', 'i4', 'f4')
+
+    @property
+    def channels(self) -> int:
+        return self.data.shape[1]
+
+    @property
+    def duration(self) -> timedelta:
+        return timedelta(seconds=self.data.shape[0] / self.rate)
 
     def __repr__(self) -> str:
         duration = self.duration
         channels = self.channels
-        dtype = self.raw.dtype
+        dtype = self.data.dtype
         return f'{type(self).__name__}({duration=!s}, {channels=}, {dtype=!s})'
 
-    def __array__(self) -> np.ndarray:
-        return self.raw
+    def __array__(self) -> npt.NDArray[_Scalar]:
+        return self.data
 
     def play(self, blocksize=1024) -> None:
         """Plays audio from array. Supports interruption via Crtl-C."""
-        _play(self.raw, self.rate, blocksize=blocksize)
+        _play(self.data, self.rate, blocksize=blocksize)
 
     @classmethod
-    def load(cls, path: Path | str) -> 'Sound':
+    def load(cls, path: Path | str) -> Sound:
         spath = str(path)
         assert spath.endswith('.flac')
         import soundfile
 
         data, rate = soundfile.read(spath)
-        return cls(data.astype('float32'), rate)
+        return cls(data.astype('f4'), rate)
```

### Comparing `glow-0.11.3/glow/io/_svg.py` & `glow-0.12.7/src/glow/io/_svg.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 __all__ = ['Svg']
 
-from collections.abc import Iterable, Sequence
+from collections.abc import Iterator, Sequence
 from pathlib import Path
 
 import cv2
 import numpy as np
 from lxml.builder import ElementMaker
 from lxml.etree import ElementTree, indent, tostring
 
@@ -25,15 +25,15 @@
 
 for (let group of svg.getElementsByTagName("g")) {
     group.setAttribute("fill", "none");
 };
 """
 
 
-def hsv_colors(count):
+def hsv_colors(count: int) -> Iterator[str]:
     for hue in np.linspace(0, 360, num=count, endpoint=False, dtype='int32'):
         yield f'hsl({hue},100%,50%)'
 
 
 class Svg:
     """Converts raster mask (2d numpy.ndarray of integers) to SVG-file.
 
@@ -74,34 +74,32 @@
 
         maxlen = max(len(c) for c in labels)
         self.labels = [f'{c:{maxlen}s}' for c in labels]
 
     def save(self, path: Path) -> None:
         path = Path(path)
 
-        script = path.parent / 'main.js'
-        if not script.exists():
+        if not (script := path.parent / 'main.js').exists():
             script.write_text(_SCRIPT)
 
-        style = path.parent / 'main.css'
-        if not style.exists():
+        if not (style := path.parent / 'main.css').exists():
             labels = zip(hsv_colors(len(self.labels)), self.labels)
             style.write_text('\n'.join(
                 f'.{name} {{ stroke: {color} }}' for color, name in labels))
 
         path.with_suffix('.svg').write_text(self.body)
 
     @staticmethod
-    def load(path: Path) -> Iterable[tuple[str, list[np.ndarray]]]:
+    def load(path: Path) -> dict[str, list[np.ndarray]]:
         """
         Yields contours, contour is 2d numpy array of shape [count, (x, y)]
         """
         tree = ElementTree()
         tree.parse(path.with_suffix('.svg').as_posix())
 
-        for group in tree.getiterator(f'{{{_SVG_NS}}}g'):
-            points = (polygon.attrib['points'].split(' ') for polygon in group)
-            contours = [
-                np.array([int(p) for p in pset], dtype='i4').reshape(-1, 2)
-                for pset in points
-            ]
-            yield group.attrib['label'], contours
+        fields = ((node.attrib['label'], (p.attrib['points'] for p in node))
+                  for node in tree.getiterator(f'{{{_SVG_NS}}}g'))
+        return {
+            name:
+            [np.fromstring(ll, 'i4', sep=' ').reshape(-1, 2) for ll in lines]
+            for name, lines in fields
+        }
```

### Comparing `glow-0.11.3/glow/metrics/__init__.py` & `glow-0.12.7/src/glow/metrics/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .base import Lambda, Metric, Scores, Staged, compose, to_index, to_prob
 from .confusion import (Confusion, ConfusionGrad, accuracy, accuracy_balanced,
                         iou, kappa, kappa_quadratic_weighted)
 from .raw import accuracy_, auroc, average_precision, dice
 
 __all__ = [
-    'Confusion', 'ConfusionGrad', 'Metric', 'Lambda', 'Scores', 'Staged',
+    'Confusion', 'ConfusionGrad', 'Lambda', 'Metric', 'Scores', 'Staged',
     'accuracy', 'accuracy_', 'accuracy_balanced', 'auroc', 'average_precision',
     'compose', 'dice', 'iou', 'kappa', 'kappa_quadratic_weighted', 'to_index',
     'to_prob'
 ]
```

### Comparing `glow-0.11.3/glow/metrics/base.py` & `glow-0.12.7/src/glow/metrics/base.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,134 +1,171 @@
 from __future__ import annotations
 
 __all__ = [
-    'Metric', 'Lambda', 'Scores', 'Staged', 'compose', 'to_index', 'to_prob'
+    'Lambda', 'Metric', 'Scores', 'Staged', 'compose', 'to_index',
+    'to_index_sparse', 'to_prob', 'to_prob_sparse'
 ]
 
-import itertools
 from abc import ABC, abstractmethod
 from collections.abc import Callable, Generator, Sequence
 from dataclasses import dataclass, field
+from itertools import count
 from typing import Protocol, overload
 
 import torch
 
 from .. import coroutine
 
 
-@dataclass
+@dataclass(frozen=True)
 class Scores:
     scalars: dict[str, float | int] = field(default_factory=dict)
     tensors: dict[str, torch.Tensor] = field(default_factory=dict)
 
     @classmethod
-    def from_dict(cls, mapping: dict[str, torch.Tensor]) -> 'Scores':
+    def from_dict(cls, mapping: dict[str, torch.Tensor]) -> Scores:
         obj = cls()
         for k, v in mapping.items():
             if v.numel() == 1:
                 obj.scalars[k] = v.item()
             else:
                 obj.tensors[k] = v
         return obj
 
 
-class _MetricFn(Protocol):
+class MetricFn(Protocol):
     def __call__(self, pred, true) -> torch.Tensor:
         ...
 
 
 class Metric(ABC):
     """Base class for metric"""
     @abstractmethod
     def __call__(self, pred, true) -> torch.Tensor:
         raise NotImplementedError
 
-    def collect(self, state) -> dict[str, torch.Tensor]:
-        raise state
+    @abstractmethod
+    def collect(self, state: torch.Tensor) -> dict[str, torch.Tensor]:
+        raise NotImplementedError
 
 
 class Lambda(Metric):
     """Wraps arbitary loss function to metric"""
-    fn: _MetricFn
+    fn: MetricFn
 
     @overload
     def __init__(self, fn: Callable, name: str):
         ...
 
     @overload
-    def __init__(self, fn: _MetricFn, name: None = ...):
+    def __init__(self, fn: MetricFn, name: None = ...):
         ...
 
     def __init__(self, fn, name=None):
         self.fn = fn
-        self.name = fn.__name__ if name is None else name  # type: ignore
+        self.name = fn.__name__ if name is None else name
 
     def __call__(self, pred, true) -> torch.Tensor:
         return self.fn(pred, true)
 
-    def collect(self, state):
+    def collect(self, state: torch.Tensor) -> dict[str, torch.Tensor]:
         return {self.name: state}
 
 
 class Staged(Metric):
     """Makes metric a "producer": applies multiple functions to its "state" """
     def __init__(self, **funcs: Callable[[torch.Tensor], torch.Tensor]):
         self.funcs = funcs
 
-    def collect(self, state):
+    def collect(self, state: torch.Tensor) -> dict[str, torch.Tensor]:
         return {key: fn(state) for key, fn in self.funcs.items()}
 
 
-def to_index(pred, true) -> tuple[int, torch.LongTensor, torch.LongTensor]:
+def to_index(pred: torch.Tensor,
+             true: torch.Tensor) -> tuple[int, torch.Tensor, torch.Tensor]:
     """
-    Convert `pred` of logits with shape [B, C, ...] to [B, ...] of indices.
-    Drop bad indices.
+    Convert `pred` of logits with shape [B, C, ...] to [B, ...] of indices,
+    i.e. tensors of long.
     """
+    assert pred.shape[0] == true.shape[0]
+    assert pred.shape[2:] == true.shape[1:]
+
     c = pred.shape[1]
     pred = pred.argmax(dim=1)
 
-    if true.min() < 0 or true.max() >= c:
-        mask = (true >= 0) & (true < c)
-        true = true[mask][None]
-        pred = pred[mask][None]
-
     return c, pred, true
 
 
-def to_prob(pred, true) -> tuple[int, torch.Tensor, torch.LongTensor]:
+def to_index_sparse(
+        pred: torch.Tensor,
+        true: torch.Tensor) -> tuple[int, torch.Tensor, torch.Tensor]:
     """
-    Convert `pred` of logits with shape [B, C, ...] to probs.
-    Drop bad indices.
+    Convert `pred` of logits with shape [B, C, ...] to [B, ...] of indices,
+    i.e. tensors of long. Drops bad indices.
+    Result is flattened.
     """
-    b, c = pred.shape[:2]
-    pred = pred.softmax(dim=1)
+    c, pred, true = to_index(pred, true)
 
-    if true.min() < 0 or true.max() >= c:
-        true = true.view(-1)
-        pred = pred.view(b, c, -1).permute(0, 2, 1).view(-1, c)
+    pred = pred.view(-1)
+    true = true.view(-1)
+
+    mask = (true >= 0) & (true < c)
+    return c, pred[mask], true[mask]
+
+
+def to_prob(pred: torch.Tensor,
+            true: torch.Tensor) -> tuple[int, torch.Tensor, torch.Tensor]:
+    """
+    Convert `pred` of logits with shape [B, C, ...] to probs,
+    i.e. tensors of float32.
+    """
+    assert pred.shape[0] == true.shape[0]
+    assert pred.shape[2:] == true.shape[1:]
+    c = pred.shape[1]
 
-        mask = (true >= 0) & (true < c)
-        true = true[mask]
-        pred = pred[mask]
+    with torch.autocast('cuda'):  # Softmax is always fp32
+        pred = pred.softmax(dim=1)
 
+    assert pred.dtype == torch.float32
     return c, pred, true
 
 
+def to_prob_sparse(
+        pred: torch.Tensor,
+        true: torch.Tensor) -> tuple[int, torch.Tensor, torch.Tensor]:
+    """
+    Convert `pred` of logits with shape [B, C, ...] to probs,
+    i.e. tensors of float.
+    Drops bad indices, i.e. those that are out of range(C).
+    Results have shape of [N, C] and [N].
+    """
+    c, pred, true = to_prob(pred, true)
+
+    b = true.shape[0]
+    true = true.view(-1)  # (b n)
+    pred = pred.view(b, c, -1).permute(0, 2, 1).view(-1, c)  # (b n) c
+
+    mask = (true >= 0) & (true < c)
+    return c, pred[mask], true[mask]
+
+
 @coroutine
 def _batch_averaged(
     fn: Metric
 ) -> Generator[dict[str, torch.Tensor], Sequence[torch.Tensor], None]:
     assert isinstance(fn, Metric)
     args = yield {}
-    state = torch.as_tensor(fn(*args))
-    for step in itertools.count(2):
+    state = fn(*args)
+    for n in count(2):
         args = yield fn.collect(state)
-        state += (torch.as_tensor(fn(*args)) - state) / step
+        state.lerp_(fn(*args), 1 / n)
 
 
 @coroutine
 def compose(*fns: Metric) -> Generator[Scores, Sequence[torch.Tensor], None]:
-    updates = *map(_batch_averaged, fns),
+    updates = *(_batch_averaged(fn) for fn in fns),
     args = yield Scores()
     while True:
-        scores = {k: v for u in updates for k, v in u.send(args).items()}
+        scores: dict[str, torch.Tensor] = {}
+        for u in updates:
+            scores |= u.send(args)
         args = yield Scores.from_dict(scores)
```

### Comparing `glow-0.11.3/glow/metrics/raw.py` & `glow-0.12.7/src/glow/metrics/raw.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 __all__ = ['accuracy_', 'auroc', 'average_precision', 'dice']
 
 import torch
 
 from .base import to_index, to_prob
 
 
-def accuracy_(pred, true) -> torch.Tensor:
+def accuracy_(pred: torch.Tensor, true: torch.Tensor) -> torch.Tensor:
     # TODO: Add docs
     _, pred, true = to_index(pred, true)
     return (true == pred).double().mean()
 
 
-def dice(pred, true, macro=True) -> torch.Tensor:
+def dice(pred: torch.Tensor,
+         true: torch.Tensor,
+         macro: bool = True) -> torch.Tensor:
     # TODO: Add docs
     c, pred, true = to_index(pred, true)
 
-    def _dice(pred, true) -> torch.Tensor:
+    def _dice(pred: torch.Tensor, true: torch.Tensor) -> torch.Tensor:
         true = true.view(-1)
         pred = pred.view(-1)
         tp, t, p = (
             x.bincount(minlength=c).clamp_(1).double()
             for x in (true[true == pred], true, pred))
         return 2 * tp / (t + p)
 
@@ -44,34 +46,37 @@
     count = torch.cat([diff, torch.tensor([diff.numel()])])
     # count = np.r_[diff.nonzero(diff).view(-1), diff.numel()]
 
     return 0.5 * (count[dense] + count[dense - 1] + 1)
 
 
 def _binary_metric(fn):
-    def call(pred, true, index: int = 0) -> torch.Tensor:
-        c, pred, true = to_prob(pred, true)
+    """Applies specified function only on probabilities of indexed class"""
+    def call(pred: torch.Tensor,
+             true: torch.Tensor,
+             index: int = 0) -> torch.Tensor:
+        c, probs, targets = to_prob(pred, true)
         assert 0 <= index < c
-        return fn(pred[:, index].view(-1), (true == index).view(-1))
+        return fn(probs[:, index].view(-1), (targets == index).view(-1))
 
     return call
 
 
 @_binary_metric
-def auroc(pred, true) -> torch.Tensor:
+def auroc(pred: torch.Tensor, true: torch.Tensor) -> torch.Tensor:
     n = true.numel()
     n_pos = true.sum()
 
     r = _rankdata(pred)
     total = n_pos * (n - n_pos)
     return (r[true == 1].sum() - n_pos * (n_pos + 1) // 2) / float(total)
 
 
 @_binary_metric
-def average_precision(pred, true) -> torch.Tensor:
+def average_precision(pred: torch.Tensor, true: torch.Tensor) -> torch.Tensor:
     n = true.numel()
     n_pos = true.sum()
 
     true = true[torch.argsort(pred)].flipud()
     weights = torch.arange(1, n + 1).float().reciprocal()
     precision = true.cumsum(0).float()
     return torch.einsum('i,i,i', true.float(), precision, weights) / n_pos
```

### Comparing `glow-0.11.3/glow/nn/_loader.py` & `glow-0.12.7/src/glow/nn/_loader.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,282 +1,393 @@
 from __future__ import annotations
 
-__all__ = ['make_loader']
+__all__ = ['get_loader']
 
 import os
+import re
 import warnings
-from collections.abc import Iterator, Mapping, Sequence, Sized
-from dataclasses import dataclass
+from collections.abc import Callable, Iterator, Mapping, Sequence, Sized
+from dataclasses import dataclass, replace
+from functools import partial
+from itertools import islice
 from typing import Any, Protocol
 
+import numpy as np
 import torch
-from torch.utils.data import Dataset, IterableDataset, Sampler
+from torch.utils.data import (Dataset, IterableDataset, RandomSampler, Sampler,
+                              SequentialSampler)
 from torch.utils.data._utils import worker as torch_worker
 
 from .. import buffered, chunked, map_n, roundrobin
-from ..core._parallel import _get_executor
-from ..distributed import get_rank, get_world_size
+from ..core._parallel import _get_executor, max_cpu_count
+from ..distributed import get_ddp_info
+from ._sampler import DdpSampler, SamplerLike, generate_seed
+from .util import _apply
 
 _NUM_CPUS: int = os.cpu_count() or 1
 
+# ------------------------------- common bases -------------------------------
 
-class _CollateFn(Protocol):
-    def __call__(self, __items: Sequence) -> Any:
-        ...
+
+class _Loader(Protocol):
+    def __iter__(self) -> Iterator:
+        raise NotImplementedError
+
+    def __len__(self) -> int:
+        raise NotImplementedError
 
 
-def default_collate(batch: Sequence[tuple]) -> Any:
-    return tuple(
-        torch.stack([torch.as_tensor(item) for item in row])
-        for row in zip(*batch))
+# ------------------------------ memory pinning ------------------------------
 
 
 def pin_memory(data):
-    if isinstance(data, torch.Tensor):
-        return data.pin_memory()
-    if hasattr(data, 'pin_memory'):
-        return data._pin_memory()
+    def _pin_memory(x):
+        return x.pin_memory()
+
+    return _apply(data, _pin_memory)
+
+
+@dataclass(frozen=True)
+class _PinningLoader(_Loader):
+    base: _Loader
+
+    def __iter__(self) -> Iterator:
+        return map_n(pin_memory, self.base, max_workers=1)
+
+    def __len__(self) -> int:
+        return len(self.base)
 
-    if isinstance(data, (str, bytes)):
-        return data
-    if isinstance(data, tuple) and hasattr(data, '_fields'):  # namedtuple
-        return type(data)(*(pin_memory(sample) for sample in data))
-    if isinstance(data, Sequence):
-        return [pin_memory(sample) for sample in data]
 
-    if isinstance(data, Mapping):
-        return {k: pin_memory(sample) for k, sample in data.items()}
+class _PinnableLoader(_Loader):
+    def pin(self) -> _Loader:
+        """
+        Copies Tensors into device/CUDA pinned memory before returning them.
+        Works in extra thread.
+        """
+        return _PinningLoader(self) if torch.cuda.is_available() else self
 
-    return data
 
+# --------------------------------- batching ---------------------------------
 
-# ------------------------------- base loader -------------------------------
+
+class _CollateFn(Protocol):
+    def __call__(self, __items: tuple) -> Any:
+        ...
 
 
 @dataclass(frozen=True)
-class _BaseLoader:
+class _BatchedLoader(_PinnableLoader):
+    base: _Loader
     batch_size: int
-    max_workers: int
     collate_fn: _CollateFn
-    pin_memory: bool
-    dataset: Dataset
-
-    def _iter_samples(self) -> Iterator:
-        raise NotImplementedError
+    drop_last: bool
+    workers: int
 
     def __iter__(self) -> Iterator:
-        batches = chunked(self._iter_samples(), self.batch_size)
-        batches = map(self.collate_fn, batches)
-        if not self.pin_memory:
-            return batches
-        return map_n(pin_memory, batches, max_workers=1)
+        it = iter(self.base)
+
+        if self.drop_last:
+            total = len(self) * self.batch_size
+            it = islice(it, total)
+
+        batches = chunked(it, self.batch_size)
+        return map_n(self.collate_fn, batches, max_workers=self.workers)
 
     def __len__(self) -> int:
+        len_ = len(self.base)
+
+        if self.drop_last:
+            return len_ // self.batch_size
+
+        return len(range(0, len_, self.batch_size))
+
+
+class _BatchableLoader(_PinnableLoader):
+    def batch(self,
+              batch_size: int,
+              collate_fn: _CollateFn | None = None,
+              drop_last: bool = False,
+              daemon: bool = False) -> _BatchedLoader:
+        """
+        Groups data into batches.
+
+        Parameters:
+        - batch_size - How many samples per batch to load
+        - collate_fn - Merges a list of samples to form a mini-batch of
+          Tensor(s).
+        - drop_last - Set to `True` to drop the last incomplete batch,
+          if size of underlying loader is not divisible by the batch size.
+          Otherwise the last batch can be smaller than others.
+        - daemon - Set to do batching in background thread.
+        """
+        if collate_fn is None:
+            collate_fn = collate
+        # TODO: return _BatchedLoader(
+        #   replace(self, finalize=None),
+        #   batch_size, collate_fn, drop_last,
+        # )
+        return _BatchedLoader(self, batch_size, collate_fn, drop_last,
+                              int(daemon))
+
+    def shuffle(self,
+                sampler: Sampler | SamplerLike | None) -> _BatchableLoader:
+        """
+        Reshuffle data at every epoch.
+
+        Parameters:
+        - sampler - Defines the strategy to draw samples from the dataset.
+          Can be any `Iterable` with `__len__` implemented.
+        """
         raise NotImplementedError
 
 
 # ---------------------- loader for map-style datasets ----------------------
 
 
 @dataclass(frozen=True)
-class _MapLoader(_BaseLoader):
+class _MapLoader(_BatchableLoader):
+    dataset: Dataset
     sampler: Sampler
+
+    def __iter__(self) -> Iterator:
+        return map(self.dataset.__getitem__, self.sampler)
+
+    def __len__(self) -> int:
+        assert isinstance(self.sampler, Sized)
+        return len(self.sampler)
+
+    def shuffle(self,
+                sampler: Sampler | SamplerLike | bool | None) -> _MapLoader:
+        if not sampler:
+            return self
+
+        if sampler is True:
+            assert isinstance(self.dataset, Sized)
+            sampler = RandomSampler(self.dataset)
+
+        return replace(self, sampler=DdpSampler(sampler))
+
+
+@dataclass(frozen=True)
+class _MapMultiLoader(_MapLoader):
+    max_workers: int
     mp: bool
-    chunksize: int | None
+    chunksize: int | None = None
 
-    def _iter_samples(self) -> Iterator:
+    def __iter__(self) -> Iterator:
         max_workers = self.max_workers
-        if (world := get_world_size()) > 1:
-            max_workers //= world
-
-        if not max_workers:
-            return map(self.dataset.__getitem__, self.sampler)
+        if ddp := get_ddp_info():
+            max_workers //= ddp.world
 
         return map_n(
             self.dataset.__getitem__,
             self.sampler,
             max_workers=max_workers,
             chunksize=self.chunksize,
             mp=self.mp)
 
-    def __len__(self) -> int:
-        indices = range(0, len(self.sampler), self.batch_size)  # type: ignore
-        return len(indices)
-
-    def set_epoch(self, epoch: int):
-        if isinstance(self.sampler, _AutoSampler):
-            self.sampler.set_epoch(epoch)
-
 
 # -------------------- loader for iterable-style datasets --------------------
 
 
 @dataclass(frozen=True)
 class _Worker:
     dataset: IterableDataset
     id: int
     num_workers: int
     seed: int | None = None
 
     def __iter__(self) -> Iterator:
-        torch_worker._worker_info = self
+        torch_worker._worker_info = self  # type: ignore[assignment]
         try:
             yield from self.dataset
         finally:
             torch_worker._worker_info = None
 
 
 @dataclass(frozen=True)
-class _IterableLoader(_BaseLoader):
+class _IterableLoader(_BatchableLoader):
     dataset: IterableDataset
 
-    def _iter_samples(self) -> Iterator:
-        if not self.max_workers:
-            yield from buffered(self.dataset)
-            return
+    def __iter__(self) -> Iterator:
+        return buffered(self.dataset)
+
+    def __len__(self) -> int:
+        assert isinstance(self.dataset, Sized)
+        return len(self.dataset)
 
-        seed = torch.empty((), dtype=torch.int64).random_().item()
+
+@dataclass(frozen=True)
+class _IterableMultiLoader(_IterableLoader):
+    max_workers: int
+
+    def __iter__(self) -> Iterator:
+        seed = generate_seed()
         workers = [
-            _Worker(self.dataset, idx, self.max_workers, int(seed))
+            _Worker(self.dataset, idx, self.max_workers, seed)
             for idx in range(self.max_workers)
         ]
-        with _get_executor(self.max_workers, True) as executor:
-            yield from roundrobin(*(buffered(w, mp=executor) for w in workers))
+        with _get_executor(self.max_workers, True) as ex:
+            yield from roundrobin(*(buffered(w, mp=ex) for w in workers))
 
-    def __len__(self) -> int:
-        indices = range(0, len(self.dataset), self.batch_size)  # type: ignore
-        return len(indices)
 
+# ----------------------------- factory function -----------------------------
 
-# --------------------------------- samplers ---------------------------------
 
+def get_loader(dataset: Dataset,
+               max_workers: int | None = 0,
+               mp: bool = False) -> _BatchableLoader:
+    """
+    Data loader. Combines a dataset and a sampler (via shuffle method), and
+    provides an iterable over the given dataset.
 
-class _IAutoSampler(Sampler):
-    def __init__(self, source: Dataset | Sampler) -> None:
-        if not isinstance(source, Sized):
-            raise TypeError('Argument should have length')
+    The data loader supports both map-style and iterable-style datasets with
+    single- or multi-process loading, customizing loading order and
+    automatic batching (collation) and memory pinning.
 
-        self.source = source
-        self.epoch = 0
-        self.seed = int(torch.empty((), dtype=torch.int64).random_().item())
+    Differences from torch.utils.data.DataLoader:
+    - Support of threadpool backend for map-style datasets.
+    - Automatically adjusts chunksize of data for passing to the workers to
+      reduce IPC overhead when multiple processes are used.
+    - Automatically adjusts number of workers in distributed context for
+      map-style datasets.
 
-    def _indices(self) -> list:
-        raise NotImplementedError
+    Parameters:
+    - dataset - Dataset from which to load the data.
+    - max_workers - How many threads or subprocesses to use for data loading.
+      `0` means that the data will be loaded in the main process/thread.
+      `None` means all logical processors.
+    - mp - Whether to use multiprocessing or not.
+    """
+    if max_workers is None:
+        max_workers = max_cpu_count(_NUM_CPUS, mp)
 
-    def __iter__(self) -> Iterator:
-        indices = self._indices()
+    if isinstance(dataset, IterableDataset):
+        if not mp and max_workers != 0:
+            warnings.warn(
+                'For iterable-style datasets multithreading is not supported. '
+                'Setting max_workers to 0',
+                stacklevel=2)
+            max_workers = 0
 
-        if (world := get_world_size()) > 1:
-            if remainder := (len(indices) % world):
-                indices += indices[:world - remainder]
-            indices = indices[get_rank()::world]
+        if (ddp := get_ddp_info()) and ddp.world > 1:
+            raise ValueError(
+                'For iterable-style datasets distributed use is not '
+                'supported')
 
-        if len(indices) != len(self):
-            raise RuntimeError(f'{len(indices)} vs {len(self)}')
+        if not max_workers:
+            return _IterableLoader(dataset)
+        return _IterableMultiLoader(dataset, max_workers)
 
-        return iter(indices)
+    else:  # noqa; RET505
+        if not isinstance(dataset, Sized):
+            raise TypeError("dataset should be sized when it's not iterable")
 
-    def __len__(self) -> int:
-        world = get_world_size() or 1
-        return (len(self.source) + world - 1) // world
+        sampler = SequentialSampler(dataset)
 
-    def set_epoch(self, epoch: int) -> None:
-        self.epoch = epoch
+        if not max_workers:
+            return _MapLoader(dataset, DdpSampler(sampler))
+        return _MapMultiLoader(dataset, DdpSampler(sampler), max_workers, mp)
 
 
-class _AutoSampler(_IAutoSampler):
-    def __init__(self, dataset: Dataset, shuffle: bool = False):
-        if not isinstance(dataset, Sized):
-            raise TypeError('Argument sampler should have length')
+# ---------------- convert & collate. forked from pytorch 2.0 ----------------
 
-        super().__init__(dataset)
-        self.shuffle = shuffle
+# TODO: split `collate` to `convert` (within worker) + `collate` (in main)
+# TODO: i.e. "Loader".tensors [alters workers] .batch() [adds collation]
 
-    def _indices(self) -> list:
-        if not self.shuffle:
-            return list(range(len(self.source)))
 
-        rng = torch.Generator()
-        rng.manual_seed(self.seed + self.epoch)
-        return torch.randperm(len(self.source), generator=rng).tolist()
+def convert(x):  # noqa: PLR0911
+    tp = type(x)
+    if isinstance(x, torch.Tensor):
+        return x
 
+    if tp.__module__ == 'numpy' and not isinstance(x, np.str_ | np.bytes_):
+        if (isinstance(x, np.ndarray)
+                and _NP_STR_DTYPE_PATTERN.search(x.dtype.str)):
+            return x
+        return torch.as_tensor(x)
 
-class _AutoSamplerProxy(_IAutoSampler):
-    def _indices(self) -> list:
-        torch.manual_seed(self.seed + self.epoch)
-        return [*self.source]  # type: ignore
+    if isinstance(x, Mapping):
+        return _apply_type(tp, {k: convert(v) for k, v in x.items()})
 
+    if isinstance(x, Sequence) and not isinstance(x, str | bytes):
+        list_ = [convert(xx) for xx in x]
 
-# ----------------------------- factory function -----------------------------
+        if isinstance(x, tuple) and hasattr(x, '_fields'):  # namedtuple
+            return tp(*list_)
+        return _apply_type(tp, list_)
 
+    return x
 
-def make_loader(dataset: Dataset,
-                batch_size: int,
-                shuffle: bool = False,
-                sampler: Sampler = None,
-                max_workers: int = _NUM_CPUS,
-                collate_fn: _CollateFn = default_collate,
-                pin_memory: bool = False,
-                multiprocessing: bool = True,
-                chunk_from_batch: bool = False) -> _BaseLoader:
-    """
-    Data loader. Combines a dataset and a sampler, and provides an iterable
-    over the given dataset.
 
-    The data loader supports both map-style and iterable-style datasets with
-    single- or multi-process loading, customizing loading order and
-    automatic batching (collation) and memory pinning.
+def collate(batch):
+    x0 = batch[0]
+    tp = type(x0)
 
-    Yields batches of batch_size from dataset in order from sampler.
+    if _HINT is not None:  # Fast alternative to functools.singledispatch
+        fn = _HINT.get(tp) or next(
+            (fn for tp_, fn in _HINT.items() if isinstance(x0, tp_)), None)
+        if fn is not None:
+            return fn(batch)
 
-    Differences from torch.utils.data.DataLoader:
-    - Support of threadpool backend for map-style datasets.
-    - Automatically adjusts chunksize of data for passing to the workers to
-      reduce IPC overhead when multiple processes are used.
-    - Automatically adjusts number of workers in distributed context for
-      map-style datasets.
-    - Use set_epoch() method before __iter__() for reprocucibility.
+    if isinstance(x0, Mapping):
+        return _apply_type(tp, {k: collate([x[k] for x in batch]) for k in x0})
 
-    Parameters:
-    - batch_size - size of batch, each workers computes batch independently.
-    - workers - Count of workers, by default all hardware threads are occupied.
-    - multiprocessing - whether to use processes or threads.
-    - chunk_from_batch - Set count of samples to pass each worker. If set
-      then chunksize will be equal to batch_size, otherwise it will be
-      estimated automatically.
-    """
-    if isinstance(dataset, IterableDataset):
-        if shuffle or sampler is not None:
-            raise ValueError(
-                'Loader with IterableDataset: sampler/shuffle options are '
-                'not supported')
+    if isinstance(x0, Sequence):
+        assert len({len(x) for x in batch}) <= 1  # py3.10+: zip(strict=True)
+        list_ = [collate(samples) for samples in zip(*batch)]
 
-        if not multiprocessing and max_workers != 0:
-            warnings.warn(
-                'Loader with IterableDataset: ThreadPool is not supported. '
-                'Setting max_workers to 0')
-            max_workers = 0
+        if isinstance(x0, tuple) and hasattr(x0, '_fields'):  # namedtuple
+            return tp(*list_)
+        return _apply_type(tp, list_)
 
-        if get_world_size() > 1:
-            raise ValueError(
-                'Loader with IterableDataset: distributed context is not '
-                'supported')
+    raise TypeError(_COLLATE_ERROR_MSG.format(tp))
 
-        return _IterableLoader(batch_size, max_workers, collate_fn, pin_memory,
-                               dataset)
 
-    else:
-        if shuffle and sampler is not None:
-            raise ValueError(
-                'Loader with MapDataset: sampler option is mutually exclusive '
-                'with shuffle')
+def _apply_type(tp, x):
+    try:
+        return tp(x)
+    except TypeError:
+        return x
+
+
+def _collate_tensor(batch: Sequence[torch.Tensor]):
+    x = batch[0]
+    out = None
+    if torch_worker.get_worker_info() is not None:
+        # If we're in a background process, concatenate directly into a
+        # shared memory tensor to avoid an extra copy
+        numel = sum(x.numel() for x in batch)
+        storage = x._typed_storage()._new_shared(numel, device=x.device)
+        out = x.new(storage).resize_(len(batch), *x.shape)
+
+    return torch.stack([*batch], out=out)
+
+
+def _collate_ndarray(batch: Sequence[np.ndarray]):
+    x = batch[0]
+    if _NP_STR_DTYPE_PATTERN.search(x.dtype.str):
+        raise TypeError(_COLLATE_ERROR_MSG.format(x.dtype))
+
+    return collate([torch.as_tensor(x) for x in batch])
+
+
+def _nop(batch):
+    return batch
+
+
+_HINT: dict[type | tuple[type, ...], Callable] = {
+    torch.Tensor: _collate_tensor,
+    np.ndarray: _collate_ndarray,  # For both ndarray and memmap
+    # Skip strings
+    bytes: _nop,
+    str: _nop,
+    # Tensorify scalars
+    (np.bool_, np.number, np.object_): torch.as_tensor,  # py3.10: UnionType
+    float: partial(torch.tensor, dtype=torch.float64),
+    int: torch.tensor,
+}
 
-        if sampler is None:
-            sampler = _AutoSampler(dataset, shuffle=shuffle)
-        else:
-            sampler = _AutoSamplerProxy(sampler)
-
-        chunksize = None
-        if multiprocessing and chunk_from_batch:
-            chunksize = batch_size
-        return _MapLoader(batch_size, max_workers, collate_fn, pin_memory,
-                          dataset, sampler, multiprocessing, chunksize)
+_NP_STR_DTYPE_PATTERN = re.compile('[SOUa]')
+_COLLATE_ERROR_MSG = (
+    'default_collate: batch must contain tensors, numpy arrays, numbers, '
+    'dicts or lists; found {}')
```

### Comparing `glow-0.11.3/glow/nn/modules.py` & `glow-0.12.7/src/glow/nn/modules/transformers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,336 +1,273 @@
 from __future__ import annotations
 
 __all__ = [
-    'Activation', 'Cat', 'Mish', 'Noise', 'Sum', 'Swish', 'UpsampleArea',
-    'UpsamplePoint', 'View', 'resblock'
+    'Attention',
+    'FeedForward',
+    'MaxVitBlock',
+    'MultiAxisAttention',
+    'VitBlock',
 ]
 
-import functools
-from collections.abc import Sequence
-from typing import Literal
-
 import torch
-import torch.autograd
-import torch.jit
 import torch.nn.functional as F
+from einops import rearrange
+from einops.layers.torch import Rearrange
+from packaging.version import Version
 from torch import nn
 
-from .. import repr_as_obj
-
-
-class Activation(nn.Module):  # TODO: deprecate and/or refactor
-    closure = staticmethod(F.relu)
-
-    @classmethod
-    def new(cls, inplace=True):
-        module = cls()
-        module.closure = functools.partial(cls.closure, inplace=inplace)
-        return module
-
-    def forward(self, x):
-        return self.closure(x)
+from .aggregates import pre_norm
+from .context import ConvCtx
+from .convnets import mbconv
+from .util import NameMixin, round8
+
+_IS_TORCH_1_12 = Version('1.12') <= Version(torch.__version__) < Version('2.0')
+_IS_TORCH_2X = Version(torch.__version__) >= Version('2.0')
+_TORCH_MHA_AUTOCAST = True
 
-    def extra_repr(self):
-        fn = self.closure.func
-        return (f'fn={fn.__module__}.{fn.__qualname__},'
-                f' {repr_as_obj(self.closure.keywords)}')
 
+class ReAttention(nn.Sequential):
+    """Re-Attention from [DeepViT](https://arxiv.org/abs/2103.11886)"""
+    def __init__(self, heads: int) -> None:
+        super().__init__(
+            Rearrange('b h i j -> b i j h'),
+            nn.Linear(heads, heads, bias=False),
+            nn.LayerNorm(heads),
+            Rearrange('b i j h -> b h i j'),
+        )
+        nn.init.normal_(self[1].weight)
 
-class View(nn.Module):
-    def __init__(self, *shape):
-        super().__init__()
-        self.shape = shape
-
-    def forward(self, x):
-        return x.view(x.shape[0], *self.shape)
 
-    def extra_repr(self):
-        return f'shape={(None, *self.shape)}'
+class Attention(NameMixin, nn.Module):
+    """
+    Multihead self-attention module (M-SA)
+    from [ViT](https://openreview.net/pdf?id=YicbFdNTTy).
 
+    Supports Re-attention mechanism
+    from [DeepViT](https://arxiv.org/abs/2103.11886).
+    """
+    __constants__ = ['reattention']
 
-class Noise(nn.Module):
-    def __init__(self, std):
+    def __init__(self,
+                 dim: int,
+                 dim_head: int = 64,
+                 dropout: float = 0.,
+                 qkv_bias: bool = False,
+                 reattention: bool = False):
         super().__init__()
-        self.std = std
-
-    def forward(self, x):
-        if not self.training:
-            return x
-        return torch.empty_like(x).normal_(std=self.std).add_(x)
-
-    def extra_repr(self):
-        return f'std={self.std}'
-
-
-# ------------------------- EfficientNet activations -------------------------
-
-
-class _ModuleBase(nn.Module):
-    class _AutoFn(torch.autograd.Function):
-        @classmethod
-        def forward(cls, ctx, x):
-            ctx.save_for_backward(x)
-            return cls._forward(x)
-
-        @classmethod
-        def backward(cls, ctx, grad):
-            return cls._backward(ctx.saved_tensors[0], grad)
-
-    def forward(self, x):
-        return self._AutoFn.apply(x)
-
-
-class Swish(_ModuleBase):
-    class _AutoFn(_ModuleBase._AutoFn):
-        @staticmethod
-        @torch.jit.script
-        def _forward(x):
-            return x.sigmoid().mul(x)
-
-        @staticmethod
-        @torch.jit.script
-        def _backward(x, grad):
-            sig = x.sigmoid()
-            return (sig * (1 + x * (1 - sig))).mul(grad)
-
-
-class Mish(_ModuleBase):
-    class _AutoFn(_ModuleBase._AutoFn):
-        @staticmethod
-        @torch.jit.script
-        def _forward(x):
-            return F.softplus(x).tanh().mul(x)
-
-        @staticmethod
-        @torch.jit.script
-        def _backward(x, grad):
-            sig = x.sigmoid()
-            tanh = F.softplus(x).tanh()
-            return (tanh + x * sig * (1 - tanh * tanh)).mul(grad)
-
-
-# ---------------------------- proper upsampling ----------------------------
+        assert dim % dim_head == 0
+        self.dim = dim
+        self.heads = heads = dim // dim_head
+        self.scale = dim_head ** -0.5
+        self.dropout = dropout
+
+        self.to_qkv = nn.Sequential(
+            fc := nn.Linear(dim, 3 * dim, bias=qkv_bias),
+            Rearrange('b n (split h d) -> split b h n d', h=heads, split=3),
+        )
+        nn.init.normal_(fc.weight, 0, (2 / (dim + dim_head)) ** .5)
 
+        self.attend = nn.Sequential(
+            nn.Softmax(-1),
+            nn.Dropout(dropout, inplace=True),
+        )
+        self.reattention = reattention
+        if reattention:
+            self.attend.append(ReAttention(heads))
+
+        self.to_out = nn.Sequential(
+            Rearrange('b h n d -> b n (h d)'),
+            fc := nn.Linear(dim, dim),
+            nn.Dropout(dropout, inplace=True),
+        )
+        nn.init.xavier_normal_(fc.weight)
 
-class UpsampleArea(nn.Module):
-    """Upsamples input image, treating samples as squares.
+        self.name = f'{dim}, {heads=}'
+        if qkv_bias:
+            self.name += ', qkv_bias=True'
+        if dropout:
+            self.name += f', {dropout=}'
+        if reattention:
+            self.name += ', reattention=True'
+
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
+        # Optimized eval-only impl since Torch 1.12
+        if _IS_TORCH_1_12 and not self.training and not self.reattention:
+            in_w, in_b, out_w, out_b = (self.to_qkv[0].weight,
+                                        self.to_qkv[0].bias,
+                                        self.to_out[1].weight,
+                                        self.to_out[1].bias)
+            tensor_args = (x, in_w, in_b, out_w, out_b)
+            if ((_TORCH_MHA_AUTOCAST or not torch.is_autocast_enabled())
+                    and not (torch.is_grad_enabled() and any([  # noqa: C419
+                        t.requires_grad for t in tensor_args
+                    ]))):
+                if torch.is_autocast_enabled():
+                    # torch uses slowpath, but this allows it go fast
+                    dtype = torch.get_autocast_gpu_dtype()
+                    if in_b.dtype != dtype:
+                        in_b = in_b.to(dtype)
+                out, _ = torch._native_multi_head_attention(
+                    x, x, x, self.dim, self.heads, in_w, in_b, out_w, out_b,
+                    None, False)
+                return out
+
+        # b n dim -> b h n d
+        qkv = self.to_qkv(x)
+        q, k, v = qkv[0], qkv[1], qkv[2]  # make torchscript happy
+
+        # Use FLASH-attention (https://arxiv.org/abs/2205.14135)
+        # and Memory-Efficient attention from XFormers
+        # for PyTorch 2.x
+        if _IS_TORCH_2X and not self.reattention:
+            dropout = self.droupout if self.is_train else 0
+            out = F.scaled_dot_product_attention(q, k, v, dropout_p=dropout)
+
+        else:
+            # Compute weights for each token
+            dots = torch.einsum('bhid,bhjd -> bhij', q, k)
+            attn = self.attend(dots * self.scale)
+
+            # Remix tokens using weights
+            out = torch.einsum('bhij,bhjd -> bhid', attn, v)
 
-    Splits original samples to S interpolated ones, where S == `scale`.
-    Result size is always multiple of `scale`.
-    """
+        # Restore shape, b h n d -> b n (h d)
+        return self.to_out(out)
 
-    _modes = {3: 'linear', 4: 'bilinear', 5: 'trilinear'}
-    _offset = 0
-    _alignment = False
 
-    def __init__(self, scale=2):
+class _RelativePositionalBias(nn.Module):
+    def __init__(self, heads: int, window_size: int) -> None:
         super().__init__()
-        self.scale = scale
 
-    def forward(self, x):
-        size = tuple((s - self._offset) * self.scale + self._offset
-                     for s in x.shape[2:])
-        return F.interpolate(
-            x, size, mode=self._modes[x.ndim], align_corners=self._alignment)
+        wdiff = 2 * window_size - 1
+        self.bias = nn.Sequential(
+            nn.Embedding(wdiff ** 2, heads),
+            Rearrange('i j h -> h i j'),
+        )
 
-    def extra_repr(self):
-        return f'scale={self.scale}'
+        axis = torch.arange(window_size)
+        grid = torch.stack(torch.meshgrid(axis, axis, indexing='ij'), -1)
+        pos = (
+            rearrange(grid, 'i j c -> (i j) 1 c')
+            - rearrange(grid, 'i j c -> 1 (i j) c'))
+        pos -= pos.min()
+        indices = pos @ torch.tensor([wdiff, 1])
+        self.register_buffer('indices', indices, persistent=False)
 
+    def forward(self) -> torch.Tensor:
+        return self.bias(self.indices)
 
-class UpsamplePoint(UpsampleArea):
-    """Upsamples input image, treating samples as points.
 
-    Inserts S-1 interpolated samples between pair of original ones,
-    where S is `scale`.
-    Thus for scale `S`, and input size `N`, result size is `(N - 1) * S + 1`.
+class MultiAxisAttention(NameMixin, nn.Module):
     """
-    _offset = 1
-    _alignment = True
-
-
-# --------------------------------- joiners ---------------------------------
-
-
-class Cat(nn.Sequential):
-    def forward(self, x):
-        return torch.cat([m(x) for m in self], dim=1)
-
-
-class Sum(nn.Sequential):
-    def forward(self, x):
-        first, *rest = self
-        return sum((m(x) for m in rest), first(x))
-
-
-def cat_seq(*blocks):
-    """Creates block returning `cat([seq(*blocks)(x), x])`, useful for U-Net"""
-    return Cat(nn.Sequential(*blocks), nn.Identity())
-
-
-# ---------------------------------- basics ----------------------------------
-
-
-def _norm_fn(channels: int) -> nn.Module:
-    return nn.BatchNorm2d(channels)
-
-
-def _act_fn(inplace: bool = False) -> nn.Module:
-    return nn.ReLU(inplace=inplace)
-
-
-def conv(cin, cout=None, kernel=3, stride=1, padding=1):
-    cout = cout or cin
-    return nn.Sequential(
-        nn.Conv2d(cin, cout, kernel, stride, padding=padding, bias=False),
-        _norm_fn(cout),
-        _act_fn(inplace=True),
-    )
-
-
-def upconv(cin: int, cout: int | None = None) -> nn.Sequential:
-    cout = cout or cin
-    return nn.Sequential(
-        nn.ConvTranspose2d(cin, cout, 3, stride=2, padding=1),
-        _norm_fn(cout),
-        _act_fn(inplace=True),
-    )
-
-
-# ---------------------------------- combos ----------------------------------
-
-
-class _Named:
-    name: str
-
-    def __repr__(self):
-        return self.name or super().__repr__()
+    Multi-axis self-attention (Max-SA)
+    from [MaxViT](https://arxiv.org/abs/2204.01697)
+    """
+    def __init__(self,
+                 dim: int,
+                 dim_head: int = 32,
+                 dropout: float = 0.,
+                 qkv_bias: bool = False,
+                 window_size: int = 7):
+        super().__init__()
+        assert dim % dim_head == 0
+        heads = dim // dim_head
 
+        self.scale = dim_head ** -0.5
+        self.to_qkv = nn.Sequential(
+            nn.Linear(dim, dim * 3, bias=qkv_bias),
+            Rearrange('... i (s h d) -> s ... h i d', s=3, h=heads),
+        )
+        self.bias = _RelativePositionalBias(heads, window_size)
 
-class SEBlock(_Named, nn.Sequential):
-    def __init__(self, cin: int, reduction: int = 16):
-        mid = cin // reduction
+        self.attend = nn.Sequential(
+            nn.Softmax(-1),
+            nn.Dropout(dropout, inplace=True),
+        )
+        self.to_out = nn.Sequential(
+            Rearrange('... h i d -> ... i (h d)'),
+            nn.Linear(dim, dim, bias=False),
+            nn.Dropout(dropout, inplace=True),
+        )
+        self.name = f'{dim}, {heads=}, {window_size=}'
+        if qkv_bias:
+            self.name += ', qkv_bias=True'
+        if dropout:
+            self.name += f', {dropout=}'
+
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
+        # ... i d -> ... i d, self-attention over i
+        q, k, v = self.to_qkv(x).unbind(0)  # ... h i d
+
+        sim = torch.einsum('... i d, ... j d -> ... i j', q, k) * self.scale
+        sim += self.bias()
+        attn = self.attend(sim)
+
+        # aggregate
+        out = torch.einsum('... i j, ... j d -> ... i d', attn, v)
+
+        # combine heads out
+        return self.to_out(out)
+
+
+class FeedForward(NameMixin, nn.Sequential):
+    def __init__(self, dim: int, ratio: float, dropout: float = 0.):
+        dim_inner = round8(dim * ratio)
         super().__init__(
-            nn.AdaptiveAvgPool2d(1),
-            nn.Conv2d(cin, mid, 1, bias=False),
-            nn.ReLU(inplace=True),
-            nn.Conv2d(mid, cin, 1, bias=False),
-            nn.Sigmoid(),
+            nn.Linear(dim, dim_inner),
+            nn.GELU(),
+            nn.Dropout(dropout, inplace=True),
+            nn.Linear(dim_inner, dim),
+            nn.Dropout(dropout, inplace=True),
+        )
+        self.name = f'{dim}, {dim_inner=}'
+        if dropout:
+            self.name += f', {dropout=}'
+
+
+# ----------------------------- complete blocks ------------------------------
+
+
+class VitBlock(nn.Sequential):
+    def __init__(self,
+                 dim: int,
+                 dim_head: int,
+                 mlp_ratio: float = 4.,
+                 dropout: float = 0.,
+                 qkv_bias: bool = False,
+                 reattn: bool = False):
+        super().__init__(
+            pre_norm(Attention(dim, dim_head, dropout, qkv_bias, reattn)),
+            pre_norm(FeedForward(dim, mlp_ratio, dropout)),
         )
-        self.name = f'{type(self).__name__}({cin} -> {mid} -> {cin})'
-
-    def forward(self, x):
-        return x * super().forward(x)
-
 
-class SplitAttention(_Named, nn.Sequential):
-    def __init__(self, cin: int, groups: int = 1, radix: int = 2):
-        mid = cin * radix // 4
 
+class MaxVitBlock(nn.Sequential):
+    def __init__(self,
+                 dim: int,
+                 dim_head: int,
+                 window: int,
+                 stride: int = 1,
+                 bn_ratio: float = 4.,
+                 se_ratio: float = 0.25,
+                 mlp_ratio: float = 4,
+                 dropout: float = 0.,
+                 qkv_bias: bool = False,
+                 ctx: ConvCtx | None = None):
         super().__init__(
-            # Mean by radix and spatial dims
-            View(groups, radix, cin // groups, -1),
-            nn.AdaptiveAvgPool3d((1, None, 1)),  # type: ignore
-            View(-1, 1, 1),
-            # Core
-            nn.Conv2d(cin, mid, 1, groups=groups, bias=False),
-            _norm_fn(mid),
-            _act_fn(inplace=True),
-            nn.Conv2d(mid, cin * radix, 1, groups=groups, bias=False),
-            # Normalize
-            View(groups, radix, cin // groups),
-            nn.Sigmoid() if radix == 1 else nn.Softmax(dim=2),
-        )
-        self.groups = groups
-        self.radix = radix
-        self.name = (f'{type(self).__name__}'
-                     f'({cin} -> {mid} -> {cin}x{radix}, groups={groups}')
-
-    def forward(self, x):
-        b, _, h, w = x.shape
-        return torch.einsum(
-            'bgrc,bgrchw->bgchw',
-            super().forward(x * self.radix),
-            x.view(b, self.groups, self.radix, -1, h, w),
-        ).view(b, -1, h, w)
-
-
-def _resblock(
-        core: Sequence[nn.Module],
-        tail: Sequence[nn.Module] = (),
-) -> nn.Sequential:
-    return nn.Sequential(
-        Sum(nn.Identity(), nn.Sequential(*core)),
-        *tail,
-    )
-
-
-def _resblock_core(cin: int, bottleneck: bool, groups: int, radix: int,
-                   expansion: int) -> list[nn.Module]:
-    if not bottleneck:  # resnet-18/34
-        return [
-            nn.Conv2d(cin, cin, 3, padding=1, bias=False),
-            _norm_fn(cin),
-            _act_fn(inplace=True),
-            nn.Conv2d(cin, cin, 3, padding=1, bias=False),
-        ]
-
-    if radix:  # resnest-50/...
-        mid = round(cin * groups / expansion)
-        sa = [SplitAttention(mid, groups=groups, radix=radix)]
-        mid2 = mid * radix
-        groups *= radix
-    else:  # (wide)resnet/resnext-50/101/152
-        mid = mid2 = round(cin / expansion)
-        sa = []
-
-    return [
-        nn.Conv2d(cin, mid, 1, bias=False),
-        _norm_fn(mid),
-        _act_fn(inplace=True),
-        nn.Conv2d(mid, mid2, 3, padding=1, groups=groups, bias=False),
-        _norm_fn(mid2),
-        _act_fn(inplace=True),
-        *sa,
-        nn.Conv2d(mid, cin, 1, bias=False),
-    ]
-
-
-def resblock(cin: int,
-             se: bool = False,
-             bottleneck: bool = False,
-             groups: int = 1,
-             radix: int = 1,
-             expansion: int = 4,
-             preact: Literal['no', 'base', 'full'] = 'no') -> nn.Sequential:
-    """
-    Modes:
-    - basic: 3x3(cin, cin) -> 3x3(cin, cin)
-    - bottleneck: 1x1(cin, mid) -> 3x3(mid, mid, groups) -> sa -> 1x1(mid, cin)
-        where: mid = cout // expansion.
-
-    For ResNet-18/34 use basic mode. Groups, expansion & radix are not used.
-    For deeper nets:
-    - groups=1:
-        - ResNet-X: expansion=4
-        - WideResNet: expansion=2
-        - ResNeSt: expansion=4, radix=2 (with se = False)
-    - groups=32:
-        - ResNeXt-32x4d: expansion=2
-        - ResNeXt-32x8d: expansion=1
-
-    If preactivation is used, first resblock should use only 'base' mode,
-    subsequent blocks should use 'full'.
-    """
-    assert not (se and radix)
+            # mbconv
+            mbconv(dim, stride, bn_ratio, se_ratio, dropout, ctx),
 
-    core = _resblock_core(cin, bottleneck, groups, radix, expansion)
-    norm = _norm_fn(cin)
-    act = _act_fn(inplace=True)
-    se_block = [SEBlock(cin)] if se else ()
-
-    if preact == 'full':  # fully pre-activated block
-        return _resblock([norm, act, *core, *se_block])
-    elif preact == 'base':
-        return _resblock([*core, *se_block])  # first pre-activated block
-    else:
-        return _resblock([*core, norm, *se_block], [act])
+            # block attention
+            Rearrange('b d (x u) (y v) -> b x y (u v) d', u=window, v=window),
+            pre_norm(
+                MultiAxisAttention(dim, dim_head, dropout, qkv_bias, window)),
+            pre_norm(FeedForward(dim, mlp_ratio, dropout)),
+            Rearrange('b x y (u v) d -> b d (x u) (y v)', u=window, v=window),
+
+            # grid attention
+            Rearrange('b d (u x) (v y) -> b x y (u v) d', u=window, v=window),
+            pre_norm(
+                MultiAxisAttention(dim, dim_head, dropout, qkv_bias, window)),
+            pre_norm(FeedForward(dim, mlp_ratio, dropout)),
+            Rearrange('b x y (u v) d -> b d (u x) (v y)', u=window, v=window),
+        )
```

### Comparing `glow-0.11.3/glow/nn/modules_factory.py` & `glow-0.12.7/src/glow/core/_profile.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,197 +1,212 @@
 from __future__ import annotations
 
-__all__ = ['linear', 'conv', 'Cat', 'Sum', 'DenseBlock', 'SEBlock']
+__all__ = ['memprof', 'time_this', 'timer']
 
-import random
+import atexit
+from collections import defaultdict, deque
+from collections.abc import Callable, Iterator
+from contextlib import contextmanager
+from dataclasses import dataclass, field
+from functools import partial
+from itertools import accumulate, count
+from threading import get_ident
+from time import perf_counter_ns, process_time_ns, thread_time_ns
+from typing import TYPE_CHECKING
+
+from wrapt import ObjectProxy
+
+from ._repr import si, si_bin
+from .debug import whereami
+
+if TYPE_CHECKING:
+    import psutil
+    _THIS: psutil.Process | None
+
+_THIS = None
+
+
+@contextmanager
+def memprof(name_or_callback: str | Callable[[float], object] | None = None,
+            /) -> Iterator[None]:
+    global _THIS  # noqa: PLW0603
+    if _THIS is None:
+        import psutil
+        _THIS = psutil.Process()
+
+    init = _THIS.memory_info().rss
+    try:
+        yield
+    finally:
+        size = _THIS.memory_info().rss - init
+        if callable(name_or_callback):
+            name_or_callback(size)
+        else:
+            name = name_or_callback
+            if name is None:
+                name = f'{whereami(2, 1)} line'
+            sign = '+' if size >= 0 else ''
+            print(f'{name} done: {sign}{si_bin(size)}')
+
+
+@contextmanager
+def timer(name_or_callback: str | Callable[[int], object] | None = None,
+          time: Callable[[], int] = perf_counter_ns,
+          /) -> Iterator[None]:
+    begin = time()
+    try:
+        yield
+    finally:
+        end = time()
+        if callable(name_or_callback):
+            name_or_callback(end - begin)
+        else:
+            name = name_or_callback or f'{whereami(2, 1)} line'
+            print(f'{name} done in {si((end - begin) / 1e9)}s')
+
+
+def _to_fname(obj) -> str:
+    if not hasattr(obj, '__module__') or not hasattr(obj, '__qualname__'):
+        obj = type(obj)
+    if obj.__module__ == 'builtins':
+        return obj.__qualname__
+    return f'{obj.__module__}.{obj.__qualname__}'
+
+
+class _Times(dict[int, int]):
+    def add(self, value: int):
+        idx = get_ident()
+        self[idx] = self.get(idx, 0) + value
+
+    def total(self) -> int:
+        return sum(self.values())
+
+
+class _Nlwp:
+    __slots__ = ('_add_event', '_get_max')
+
+    def __init__(self) -> None:
+        events = deque[int]()
+        self._add_event = events.append
+
+        deltas = iter(events.popleft, None)
+        totals = accumulate(deltas)
+        maximums = accumulate(totals, max, initial=0)
+        self._get_max = maximums.__next__
+
+    def __enter__(self):
+        self._add_event(+1)
+        self._get_max()
+
+    def __exit__(self, *args):
+        self._add_event(-1)
+        self._get_max()
+
+    def max(self) -> int:
+        self._add_event(0)
+        return self._get_max()
+
+
+@dataclass(frozen=True)
+class _Stat:
+    calls: count = field(default_factory=count)
+    nlwp: _Nlwp = field(default_factory=_Nlwp)
+    cpu_ns: _Times = field(default_factory=_Times)
+    all_ns: _Times = field(default_factory=_Times)
+
+    def __call__(self, op, *args, **kwargs):
+        with self.nlwp, \
+                timer(self.all_ns.add), \
+                timer(self.cpu_ns.add, thread_time_ns):
+            return op(*args, **kwargs)
+
+    def stat(self) -> tuple[float, float, str] | None:
+        if not (n := next(self.calls)):
+            return None
+        w = self.nlwp.max()
+        t_ns = self.cpu_ns.total()  # CPU
+        i_ns = self.all_ns.total() - t_ns  # idle = total - CPU
+        t, i = t_ns / 1e9, i_ns / 1e9
+
+        tail = (f'{n} x {si(t / n)}s' +
+                (f' @ {w}T' if w > 1 else '')) if n > 1 else ''
+        return t, i, tail
+
+
+class _Proxy(ObjectProxy):
+    def __init__(self, wrapped, wrapper):
+        super().__init__(wrapped)
+        self._self_wrapper = wrapper
+
+
+class _TimedCall(_Proxy):
+    def __get__(self, instance, owner):
+        fn = self.__wrapped__.__get__(instance, owner)
+        return _BoundTimedCall(fn, self._self_wrapper)
+
+    def __call__(self, *args, **kwargs):
+        next(self._self_wrapper.calls)
+        r = self._self_wrapper(self.__wrapped__, *args, **kwargs)
+        if isinstance(r, Iterator):
+            return _TimedIter(r, self._self_wrapper)
+        return r
+
+
+class _BoundTimedCall(_TimedCall):
+    def __get__(self, instance, owner):
+        return self
+
+
+class _TimedIter(_Proxy):
+    def __iter__(self):
+        return self
+
+    def __next__(self):
+        return self._self_wrapper(self.__wrapped__.__next__)
+
+    def send(self, value):
+        return self._self_wrapper(self.__wrapped__.send, value)
+
+    def throw(self, typ, val=None, tb=None):
+        return self._self_wrapper(self.__wrapped__.throw, typ, val, tb)
+
+    def close(self):
+        return self._self_wrapper(self.__wrapped__.close)
+
+
+# Wall time, i.e. sum of per-thread times, excluding sleep
+_start = process_time_ns()
+_stats = defaultdict[str, _Stat](_Stat)
+
+
+@atexit.register
+def _print_stats(*names: str):
+    all_busy = (process_time_ns() - _start + 1) / 1e9
+
+    stats = []
+    names = names or tuple(_stats)
+    for name in names:
+        if not (stat := _stats.pop(name, None)):
+            continue
+        if not (lines := stat.stat()):
+            continue
+        stats.append((*lines, name))
+
+    for busy, idle, tail, name in sorted(stats):
+        print(
+            f'{busy/all_busy:6.2%}',
+            f'{si(busy):>5s}s + {si(idle):>5s}s',
+            name,
+            tail,
+            sep=' - ')
+
+
+def time_this(fn=None, /, *, name: str | None = None):
+    """Log function and/or generator timings at program exit"""
+    if fn is None:
+        return partial(time_this, name=name)
 
-import torch
-from torch import nn
+    if name is None:
+        name = _to_fname(fn)
 
-from .modules import Activation
-
-
-class Nonlinear:  # TODO: deprecate and/or refactor
-    """`order` specifies order of blocks:
-        - `-`: weight
-        - `N`: normalization
-        - `A`: activation
-    """
-    order: str = '-NA'
-
-    @classmethod
-    def new(cls,
-            module: type,
-            cin: int,
-            cout: int = 0,
-            *,
-            order: str = '',
-            **kwargs: object) -> nn.Module:
-        order = order or cls.order
-        assert {*order} <= {*'AN-'}
-        cout = cout or cin
-
-        def _to_layer(char):
-            if char == 'N':
-                if order.index('N') < order.index('-'):
-                    return nn.BatchNorm2d(cin)
-                else:
-                    return nn.BatchNorm2d(cout)
-            elif char == 'A':
-                return Activation.new()
-
-            bias = order.index('-') < order.index('N')
-            return module(cin, cout, **kwargs, bias=bias)
-
-        if len(order) == 1:
-            return _to_layer(order)
-        return nn.Sequential(*(_to_layer(o) for o in order))
-
-
-def linear(cin, cout=0, **kwargs):
-    return Nonlinear.new(nn.Linear, cin, cout, **kwargs)
-
-
-def conv(cin, cout=0, stride=1, padding=1, **kwargs):
-    """
-    Convolution. Special cases:
-        - Channelwise: `padding` = 0, `stride` = 1
-
-    Kernel size equals to `stride + 2 * padding` for integer scaling
-    """
-    return Nonlinear.new(
-        nn.Conv2d,
-        cin,
-        cout,
-        kernel_size=(stride + 2 * padding),
-        stride=stride,
-        padding=padding,
-        **kwargs)
-
-
-class Cat(nn.Sequential):  # TODO: deprecate and/or refactor
-    """
-    Helper for U-Net-like modules
-
-    >>> conv = nn.Conv1d(4, 4, 1)
-    >>> cat = Cat(conv)
-    >>> x = torch.randn(1, 4, 16)
-    >>> torch.equal(cat(x), torch.cat([x, conv(x)], dim=1))
-    True
-    """
-    def forward(self, x):
-        return torch.cat([x, super().forward(x)], dim=1)
-
-
-class Sum(nn.Sequential):  # TODO: deprecate and/or refactor
-    """Helper for ResNet-like modules"""
-    kind = 'resnet'
-    expansion: float | None = None
-    groups: int | None = None
-    blending = False
-
-    def __init__(self,
-                 *children: nn.Module,
-                 tail: nn.Module = None,
-                 ident: nn.Module = None,
-                 skip: float = 0.0) -> None:
-        super().__init__(*children)
-        self.tail = tail
-        self.ident = ident
-        self.skip = skip
-
-    def forward(self, x):
-        y = self.ident(x) if self.ident else x
-        if not self.training or self.skip == 0 or self.skip < random.random():
-            y = super().forward(x).add_(y)
-        return self.tail(y) if self.tail else y
-
-    @classmethod
-    def _base_2_way(cls, cin):
-        children = [conv(cin), conv(cin, order='-N')]
-        return cls(*children, tail=Activation.new(inplace=False))
-
-    @classmethod
-    def _base_3_way(cls, cin, expansion, **kwargs):
-        mid = int(cin * expansion)
-        children = [
-            conv(cin, mid, padding=0),
-            conv(mid, mid, **kwargs),
-            conv(mid, cin, padding=0, order='-N'),
-        ]
-        if cls.blending:
-            children.append(SEBlock.new(cin))
-        return cls(*children, tail=Activation.new(inplace=False))
-
-    @classmethod
-    def new(cls, cin):
-        factory = {
-            'resnet': cls._resnet,
-            'resnext': cls._resnext,
-            'mobile': cls._mobile,
-        }.get(cls.kind)
-        if factory is None:
-            raise ValueError(f'Unsupported {cls.kind}')
-        return factory(cin)
-
-    @classmethod
-    def _resnet(cls, cin):
-        expansion = cls.expansion or (1 / 4)
-        return cls._base_3_way(cin, expansion=expansion)
-
-    @classmethod
-    def _resnext(cls, cin):
-        expansion = cls.expansion or (1 / 2)
-        groups = cls.groups or 32
-        return cls._base_3_way(cin, expansion=expansion, groups=groups)
-
-    @classmethod
-    def _mobile(cls, cin):
-        expansion = cls.expansion or 6
-        return cls._base_3_way(
-            cin, expansion=expansion, groups=cin * expansion)
-
-
-# -------------------------------- factories --------------------------------
-
-
-class DenseBlock(nn.Sequential):
-    def __init__(self, cin, depth=4, step=16, full=False):
-        super().__init__(*(conv(cin + step * i, step, order='NA-')
-                           for i in range(depth)))
-        self.full = full
-
-    def __repr__(self):
-        convs = [
-            c for m in self.children()
-            for c in m.children() if isinstance(c, nn.modules.conv._ConvNd)
-        ]
-        cin = convs[0].in_channels
-        cout = sum(c.out_channels for c in convs)
-        if self.full:
-            cout += cin
-        return f'{type(self).__name__}({cin}, {cout}, full={self.full})'
-
-    def forward(self, x):
-        ys = []
-        for module in self.children():
-            y = module(x)
-            ys.append(y)
-            x = torch.cat([x, y], dim=1)
-        return x if self.full else torch.cat(ys, dim=1)
-
-
-class SEBlock(nn.Sequential):
-    reduction = 16
-
-    @classmethod
-    def new(cls, cin):
-        return cls(
-            nn.AdaptiveAvgPool2d(1),
-            nn.Conv2d(cin, cin // cls.reduction, 1, bias=False),
-            Activation.new(),
-            nn.Conv2d(cin // cls.reduction, cin, 1, bias=False),
-            nn.Sigmoid(),
-        )
-
-    def forward(self, x):
-        return x * super().forward(x)
+    fn.log_timing = partial(_print_stats, name)
+    return _TimedCall(fn, _stats[name])
```

### Comparing `glow-0.11.3/glow/nn/optimizers.py` & `glow-0.12.7/src/glow/nn/optimizers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 __all__ = ['AdamW', 'RAdam', 'SGDW']
 
-from typing import Any, Tuple
-
 import torch
 from torch.optim import optimizer
 
 
 class _OptimizerBase(optimizer.Optimizer):
     _step = 0
 
@@ -24,17 +22,17 @@
                 if p.grad is None:
                     continue
                 if p.grad.is_sparse:
                     raise RuntimeError('Sparse grads are not supported')
                 with torch.no_grad():
                     self._do_step(p, group, self.state[p], *args)
 
-        return loss  # noqa: R504
+        return loss
 
-    def _update_group(self, group) -> Tuple[Any, ...]:
+    def _update_group(self, group) -> tuple:
         return ()
 
     def _do_step(self, p, group, state, *args):
         raise NotImplementedError
 
 
 class SGDW(_OptimizerBase):
@@ -74,15 +72,14 @@
     def _do_step(self, p, group, state):
         if group['weight_decay'] != 0:
             p.mul_(1 - group['lr'] * group['weight_decay'])
 
         momentum = group['momentum']
         grad = p.grad
         if momentum != 0:
-            state = self.state[p]
             if state:
                 grad = state['exp_avg']
                 grad.mul_(momentum).add_(p.grad, alpha=1 - group['dampening'])
             else:
                 grad = state['exp_avg'] = p.grad.clone().detach_()
 
             if group['nesterov']:
@@ -104,16 +101,16 @@
     def __init__(self,
                  params,
                  lr=1e-3,
                  betas=(0.9, 0.999),
                  eps=1e-8,
                  weight_decay=1e-2,
                  amsgrad=False) -> None:
-        assert 0.0 <= lr
-        assert 0.0 <= eps
+        assert lr >= 0.0
+        assert eps >= 0.0
         for i, beta in enumerate(betas):
             assert 0.0 <= beta < 1.0, f'Invalid beta at index {i}: {betas}'
         defaults = {
             'lr': lr,
             'betas': betas,
             'eps': eps,
             'weight_decay': weight_decay,
```

### Comparing `glow-0.11.3/glow/nn/plot.py` & `glow-0.12.7/src/glow/nn/plot.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,50 +1,65 @@
 __all__ = ['plot_model']
 
 import functools
+from collections.abc import Iterable, Iterator, Mapping
 from contextlib import ExitStack
-from typing import Any
 
 import graphviz
 import torch
 from torch import nn
 from torch.autograd import Function
 
 from .. import mangle, si
 
+# TODO: Still buggy, continue research/refactor
 
-def id_(x: Any) -> str:
+
+def id_(x) -> str:
     if hasattr(x, 'variable'):
         x = x.variable
-    return hex(x.storage().data_ptr() if torch.is_tensor(x) else id(x))
+    addr = x.storage().data_ptr() if isinstance(x, torch.Tensor) else id(x)
+    return hex(addr)
 
 
-def as_tuple(xs):
+def flatten(xs) -> Iterator[torch.Tensor]:
     if xs is None:
-        return ()
-    if isinstance(xs, tuple):
-        return tuple(x for x in xs if x is not None)
-    return (xs, )
+        return
+    if isinstance(xs, torch.Tensor):
+        yield xs
+        return
+    if isinstance(xs, Iterable):
+        if isinstance(xs, Mapping):
+            xs = xs.items()
+        for x in xs:
+            yield from flatten(x)
+        return
+    raise TypeError(f'Unsupported argument type: {type(xs)}')
 
 
 def sized(var: torch.Tensor):
     if max(var.shape) == var.numel():
         return f'{tuple(var.shape)}'
     return f'{tuple(var.shape)}\n{si(var.numel())}'
 
 
 class Builder:
-    flat = False
-
-    def __init__(self, inputs: set, params: dict):
+    def __init__(self,
+                 inputs: set[str],
+                 params: dict[str, str],
+                 *,
+                 nesting: bool = True,
+                 variables: bool = True):
         self.inputs = inputs
         self.params = params
+        self.nesting = nesting
+        self.variables = variables
 
         self._mangle = mangle()
-        self._seen: dict[str, str] = {}
+        self._memo: dict[str, str] = {}
         self._shapes: dict[Function, str] = {}
         root = graphviz.Digraph(
             name='root',
             graph_attr={
                 'rankdir': 'LR',
                 'newrank': 'true',
                 'color': 'lightgrey',
@@ -59,130 +74,143 @@
                 'fontsize': '12',
                 'height': '0.2',
                 'ranksep': '0.1',
             },
         )
         self.stack = [root]
 
-    def _add_node(self, grad):
-        root = self.stack[-1]
-        # doesn't have variable, so it's "operation"
-        if not hasattr(grad, 'variable'):
-            label = type(grad).__name__.replace('Backward', '')
-            if grad in self._shapes:
-                label = f'{label}\n=> {tuple(self._shapes[grad])}'
-            root.node(id_(grad), label)
-            return False
-
-        # have variable, so it's either Parameter or Variable
-        var, label = grad.variable, ''
-        try:
-            name = self.params[id(var)] + '\n'
-            label = (name.partition if self.flat else name.rpartition)('.')[-1]
-        except KeyError:
+    def _add_op_node(self, grad_id: str, grad: Function):
+        label = type(grad).__name__.replace('Backward', '')
+        if grad in self._shapes:
+            label = f'{label}\n=> {tuple(self._shapes[grad])}'
+        self.stack[-1].node(grad_id, label)
+
+    def _add_var_node(self, var_id: str, var: torch.Tensor):
+        label_ = []
+        if param_name := self.params.get(var_id):
+            root = self.stack[-1]
+            parts = param_name.split('.')
+            label_.append(parts[-1] if self.nesting else '.'.join(parts[1:]))
+        else:
             root = self.stack[0]  # unnamed, that's why external
-        label = f'{label}{var.storage().data_ptr():x}\n'
 
-        color = 'yellow' if id(var) in self.inputs else 'lightblue'
-        root.node(id_(grad), label + sized(var), fillcolor=color)
-        return True
-
-    def _traverse_saved(self, grad):
-        saved_tensors = grad.saved_tensors or ()
-        saved_tensors = [var for var in saved_tensors if torch.is_tensor(var)]
-        if not saved_tensors:
-            return
-        with self.stack[-1].subgraph() as s:
+        label = '\n'.join([*label_, var_id, sized(var)])
+        color = 'yellow' if var_id in self.inputs else 'lightblue'
+        root.node(var_id, label, fillcolor=color)
+
+    def _traverse_saved(self, grad_id: str, *tensors):
+        tensors = *(v for v in tensors if isinstance(v, torch.Tensor)),
+        if not tensors:
+            return
+        s_ctx = self.stack[-1].subgraph()
+        assert s_ctx is not None
+        with s_ctx as s:
             s.attr(rank='same')
-            for var in saved_tensors:
-                label = hex(var.storage().data_ptr()) + '\n' + sized(var)
-                # label = sized(var)
-                if id_(var) not in self._seen:
-                    s.node(id_(var), label, fillcolor='orange')
-                s.edge(id_(var), id_(grad))
+            for var in tensors:
+                var_id = id_(var)
+                if var_id not in self._memo:
+                    label = f'{var_id}\n{sized(var)}'
+                    s.node(var_id, label, fillcolor='orange')
+                s.edge(var_id, grad_id)
 
-    def _traverse(self, grad, depth=0):
-        if grad is None or id_(grad) in self._seen:
+    def _traverse(self, grad: Function, depth: int = 0):
+        if grad is None or (grad_id := id_(grad)) in self._memo:
             return
 
         root = self.stack[-1]
-        self._seen[id_(grad)] = head = root.name
-        if self._add_node(grad):
+        self._memo[grad_id] = head = root.name
+        if hasattr(grad, 'variable'):
+            # Has variable, so it's either Parameter or Variable
+            self._add_var_node(grad_id, grad.variable)
             yield (depth - 1, None, grad)
             return
 
+        # Doesn't have variable, so it's "operation"
+        self._add_op_node(grad_id, grad)
+
         # TODO : add merging of tensors with same data
-        if hasattr(grad, 'saved_tensors'):
-            self._traverse_saved(grad)
+        if self.variables and hasattr(grad, 'saved_tensors'):
+            self._traverse_saved(grad_id, *(grad.saved_tensors or ()))
 
-        for ch, _ in getattr(grad, 'next_functions', ()):
-            if ch is None:
+        for grad_next, _ in getattr(grad, 'next_functions', ()):
+            if grad_next is None:
                 continue
-            yield from self._traverse(ch, depth + 1)
+            yield from self._traverse(grad_next, depth + 1)
 
-            tail = self._seen.get(id_(ch))
+            next_id = id_(grad_next)
+            tail = self._memo.get(next_id)
             if tail is not None and head is not None and not (
                     head.startswith(tail) or tail.startswith(head)):
-                yield (depth, ch, grad)  # leafs, yield for depth-check
+                yield (depth, grad_next, grad)  # leafs, yield for depth-check
                 continue
 
-            name = self.params.get(id(getattr(ch, 'variable', None)))
-            if not self.flat and name and name.rpartition('.')[0] == head:
-                with root.subgraph() as s:  # type: ignore
+            name = self.params.get(next_id)
+            if self.nesting and name and name.rpartition('.')[0] == head:
+                s_ctx = root.subgraph()
+                assert s_ctx is not None
+                with s_ctx as s:
                     s.attr(rank='same')
-                    s.edge(id_(ch), id_(grad))  # same module, same rank
+                    s.edge(next_id, grad_id)  # same module, same rank
             else:
-                self.stack[0].edge(id_(ch), id_(grad))
+                self.stack[0].edge(next_id, grad_id)
 
     def _mark(self, ts):
         edges = []
-        for t in as_tuple(ts):
+        for t in flatten(ts):
             if t.grad_fn is not None:
-                self._shapes[t.grad_fn] = t.shape
-                edges.extend(self._traverse(t.grad_fn))
+                self._shapes[t.grad_fn] = t.shape  # type: ignore[assignment]
+                edges += self._traverse(t.grad_fn)
         if not edges:
             return
 
         max_depth = max(depth for depth, *_ in edges) + 1
         for depth, tail, head in edges:  # inter-module edges
             if tail is not None:
-                minlen = None if self.flat else f'{max_depth - depth}'
+                minlen = f'{max_depth - depth}' if self.nesting else None
                 self.stack[0].edge(id_(tail), id_(head), minlen=minlen)
 
     def forward_pre(self, name, module, xs):
         self._mark(xs)
         # -------- start node --------
-        if self.flat:
+        if not self.nesting:
             return
         scope = graphviz.Digraph(name=self._mangle(name))
         scope.attr(label=f'{name.split(".")[-1]}:{type(module).__name__}')
         self.stack.append(scope)
 
     def forward(self, module, _, ys):
         self._mark(ys)
-        if self.flat:
+        if not self.nesting:
             return
-        cluster = self.stack.pop(-1)
+        cluster = self.stack.pop()
         cluster.name = f'cluster_{cluster.name}'
         self.stack[-1].subgraph(cluster)
         # -------- end node --------
 
 
-def plot_model(model: nn.Module, *input_shapes: tuple[int, ...], device='cpu'):
+def plot_model(model: nn.Module,
+               *input_shapes: tuple[int, ...],
+               device='cpu',
+               nesting: bool = True,
+               variables: bool = False):
     """Produces Graphviz representation of PyTorch autograd graph
 
     Blue nodes are the Variables that require grad, orange are Tensors
     saved for backward in torch.autograd.Function
     """
-    inputs = [torch.zeros(1, *shape, device=device) for shape in input_shapes]
-    inputs = [inp.requires_grad_() for inp in inputs]
+    inputs = [
+        torch.zeros(1, *s, device=device, requires_grad=True)
+        for s in input_shapes
+    ]
     params = model.state_dict(prefix='root.', keep_vars=True)
     hk = Builder(
-        {id(var) for var in inputs},
-        {id(var): name for name, var in params.items()},
+        {id_(var) for var in inputs},
+        {id_(var): name for name, var in params.items()},
+        nesting=nesting,
+        variables=variables,
     )
     with ExitStack() as stack:
         for name, m in model.named_modules(prefix='root'):
             stack.callback(
                 m.register_forward_pre_hook(
                     functools.partial(hk.forward_pre, name)).remove)
             stack.callback(m.register_forward_hook(hk.forward).remove)
```

### Comparing `glow-0.11.3/glow/test/run_metrics.py` & `glow-0.12.7/test/run_metrics.py`

 * *Files identical despite different names*

### Comparing `glow-0.11.3/glow/test/test_api.py` & `glow-0.12.7/test/test_api.py`

 * *Files identical despite different names*

### Comparing `glow-0.11.3/glow/test/test_batch.py` & `glow-0.12.7/test/test_batch.py`

 * *Files identical despite different names*

### Comparing `glow-0.11.3/glow/test/test_buffered.py` & `glow-0.12.7/test/test_buffered.py`

 * *Files identical despite different names*

### Comparing `glow-0.11.3/glow/test/test_cli.py` & `glow-0.12.7/test/test_cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 @dataclass
 class Arg:
     arg: str
 
 
 @dataclass
-class List_:
+class List_:  # noqa: N801
     args: list[str]
 
 
 @dataclass
 class UntypedList:  # Forbidden, as list field should always be typed
     args: list
 
@@ -39,19 +39,19 @@
 @dataclass
 class Boolean:
     param: bool = False
 
 
 @dataclass
 class Nullable:
-    param: Optional[str] = None
+    param: Optional[str] = None  # noqa: UP007
 
 
 @dataclass
-class Optional_:
+class Optional_:  # noqa: N801
     param: str = 'hello'
 
 
 @dataclass
 class Nested:
     arg: str
     nested: Optional_
@@ -118,31 +118,31 @@
     return a
 
 
 def _kwarg(a: int = 4):
     return a
 
 
-def _kwarg_opt(a: int = None):
+def _kwarg_opt(a: int = None):  # type: ignore[assignment]
     return a
 
 
 def _kwarg_literal(a: Literal[1, 2] = 1):
     return a
 
 
 def _kwarg_bool(a: bool = False):
     return a
 
 
-def _kwarg_list(a: list[int] = []):
+def _kwarg_list(a: list[int] = []):  # noqa: B006
     return a
 
 
-def _kwarg_opt_list(a: list[int] = None):
+def _kwarg_opt_list(a: list[int] = None):  # type: ignore[assignment]
     return a
 
 
 def _arg_kwarg(a: int, b: str = 'hello'):
     return a, b
```

### Comparing `glow-0.11.3/glow/test/test_shm.py` & `glow-0.12.7/test/test_shm.py`

 * *Files identical despite different names*

### Comparing `glow-0.11.3/glow/test/test_thread_pool.py` & `glow-0.12.7/test/test_thread_pool.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-import os
-import sys
-from typing import NamedTuple
+from dataclasses import dataclass
 
 import numpy as np
+import pytest
 
 import glow
+from glow import eat
+from glow.core._parallel import max_cpu_count
 
 DEATH_RATE = 0
 SIZE = 100
 NUM_STEPS = 10
 DTYPE = np.dtype(np.float32)
 
-NUM_CPUS = os.cpu_count() or 1
-if sys.platform == 'win32':
-    NUM_CPUS = min(NUM_CPUS, 8)
+MAX_PROCS = 8
+NUM_PROCS = max_cpu_count(MAX_PROCS, mp=True)
 
 
 def _make_array(n):
     return np.arange(int(n), dtype=DTYPE)
 
 
 class AsInit:
@@ -27,15 +27,16 @@
     def args(self):
         return [[np.mean(self.data)]] * NUM_STEPS
 
     def __call__(self, mean):
         assert np.mean(self.data) == mean
 
 
-class AsArg(NamedTuple):
+@dataclass(frozen=True)
+class AsArg:
     n: int
 
     def args(self):
         for _ in range(NUM_STEPS):
             data = _make_array(self.n)
             yield data, np.mean(data)
 
@@ -45,15 +46,16 @@
 
 class AsArgRepeated(AsArg):
     def args(self):
         args, = super().args()
         return [[*args]] * NUM_STEPS
 
 
-class AsResult(NamedTuple):
+@dataclass(frozen=True)
+class AsResult:
     n: int
 
     def args(self):
         return np.arange(NUM_STEPS).reshape(-1, 1)
 
     def __call__(self, _):
         return _make_array(self.n)
@@ -78,34 +80,34 @@
 def bench_ipc_speed(order=25, steps=100):
     from matplotlib import pyplot as plt
 
     sizes = np.asarray([2 ** order, *np.logspace(order, 2, num=steps, base=2)])
     to_bytes = DTYPE.itemsize * 2  # x2, because copy+read
 
     fig = plt.figure(figsize=(10, 4))
-    workers = [AsInit, AsArgRepeated, AsArg, AsResult]
+    workers = (AsInit, AsArgRepeated, AsArg, AsResult)
     for i, worker in enumerate(workers, 1):
         ax = fig.add_subplot(
             1,
             len(workers),
             i,
             ylabel='bytes/s',
             xlabel='size',
             xscale='log',
             yscale='log',
             ylim=(1, 1e12),
             title=worker.__name__)
         for runner in [run_glow, run_joblib, run_joblib_mp]:
             label = f'{worker.__name__}-{runner.__name__}'
-            times = []
+            times: list[int] = []
             for size in sizes:
                 task = worker(size)
-                args = zip(*task.args())
+                args = zip(*task.args())  # type: ignore[attr-defined]
                 with glow.timer(times.append):
-                    [*runner(task, *args)]
+                    eat(runner(task, *args))
 
             bps = to_bytes * NUM_STEPS * sizes / np.asarray(times)
             print(f'max {glow.si_bin(bps.max())}/s - {label}')
 
             ax.plot(to_bytes * sizes, bps, label=runner.__name__)
             ax.legend()
 
@@ -136,33 +138,35 @@
 def _test_interrupt():
     """Should die gracefully on Ctrl-C"""
     sources = (
         source(SIZE),
         np.random.randint(2 ** 10, size=SIZE),
     )
     # sources = map(glow.buffered, sources)
-    res = glow.map_n(do_work, *sources, max_workers=NUM_CPUS, mp=True)
+    res = glow.map_n(do_work, *sources, max_workers=NUM_PROCS, mp=True)
     print('start main', end='')
     for r in res:
         print(end=f'\rmain {r} computes...')
         rg = np.random.default_rng(r)
         n = 10
         a = rg.random((2 ** n, 2 ** n), dtype='f4')
         b = rg.random((2 ** n, 2 ** n), dtype='f4')
         (a @ b).sum()
         yield r
         print(end=f'\rmain {r} waits...')
     print('\rmain done')
 
 
+@pytest.mark.skipif(NUM_PROCS < 2, reason='not enough memory')
 def test_interrupt():
     rs = _test_interrupt()
     assert [*rs] == [*range(SIZE)]
 
 
+@pytest.mark.skipif(NUM_PROCS < 2, reason='not enough memory')
 def test_interrupt_with_buffer():
     rs = glow.buffered(_test_interrupt())
     assert [*rs] == [*range(SIZE)]
 
 
 if __name__ == '__main__':
     bench_ipc_speed()
```

### Comparing `glow-0.11.3/glow/test/test_timed.py` & `glow-0.12.7/test/test_timed.py`

 * *Files identical despite different names*

### Comparing `glow-0.11.3/glow/test/test_uuid.py` & `glow-0.12.7/test/test_uuid.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,21 +38,18 @@
     assert u == Uid(str(Uid(u)))
 
     u = Uid.v4()
     assert isinstance(u, Uid)
     assert u == Uid(u)
     assert u == Uid(str(u))
 
-    with pytest.raises(ValueError):
-        Uid('0')
-
 
 def test_consistency():
     num_iterations = 1000
-    lengths = Counter()
+    lengths = Counter[int]()
 
     for _ in range(num_iterations):
         uid = Uid.v4()
 
         encoded = str(uid)
         lengths[len(encoded)] += 1
         uid_decoded = Uid(encoded)
@@ -61,14 +58,17 @@
 
     assert len(lengths) == 1
 
     (_, count), = lengths.most_common()
     assert count == num_iterations
 
 
-def test_edge_cases():
-    with pytest.raises(ValueError):
-        Uid([])
-    with pytest.raises(ValueError):
-        Uid({})
+@pytest.mark.parametrize('x', [[], {}, ()])
+def test_badtype(x):
+    with pytest.raises(TypeError):
+        Uid(x)
+
+
+@pytest.mark.parametrize('x', ['', '0'])
+def test_badvalue(x):
     with pytest.raises(ValueError):
-        Uid((2, ))
+        Uid(x)
```

### Comparing `glow-0.11.3/glow/transforms/__init__.py` & `glow-0.12.7/src/glow/transforms/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from .classes import (BitFlipNoise, ChannelMix, ChannelShuffle, CutOut,
                       DegradeJpeg, DegradeQuality, Elastic, FlipAxis, HsvShift,
                       LumaJitter, MaskDropout, MultiNoise, WarpAffine)
 from .core import Chain, Transform
 from .functional import grid_shuffle
 
 __all__ = [
-    'BitFlipNoise', 'ChannelMix', 'ChannelShuffle', 'Chain', 'CutOut',
+    'BitFlipNoise', 'Chain', 'ChannelMix', 'ChannelShuffle', 'CutOut',
     'DegradeJpeg', 'DegradeQuality', 'Elastic', 'FlipAxis', 'HsvShift',
     'LumaJitter', 'MaskDropout', 'MultiNoise', 'Transform', 'WarpAffine',
     'grid_shuffle'
 ]
```

### Comparing `glow-0.11.3/glow/transforms/classes.py` & `glow-0.12.7/src/glow/transforms/classes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 __all__ = [
-    'ChannelMix', 'ChannelShuffle', 'CutOut', 'BitFlipNoise', 'Elastic',
-    'LumaJitter', 'DegradeJpeg', 'DegradeQuality', 'FlipAxis', 'HsvShift',
+    'BitFlipNoise', 'ChannelMix', 'ChannelShuffle', 'CutOut', 'DegradeJpeg',
+    'DegradeQuality', 'Elastic', 'FlipAxis', 'HsvShift', 'LumaJitter',
     'MaskDropout', 'MultiNoise', 'WarpAffine'
 ]
 
 from dataclasses import InitVar, dataclass, field
 from typing import Any
 
 import cv2
@@ -121,15 +121,15 @@
         mat = ortho_group.rvs(num_channels, random_state=rng).astype('f4')
 
         mat *= rng.uniform(*self.intensity)
         lumat = np.full((num_channels, num_channels), 1 / num_channels)
 
         image = image @ ((np.eye(num_channels) - lumat) @ mat + lumat)
 
-        return image.clip(0, 255).astype('u1')  # type: ignore
+        return image.clip(0, 255).astype('u1')
 
 
 @dataclass
 class LumaJitter(_LutTransform):
     brightness: tuple[float, float] = (-0.2, 0.2)
     contrast: tuple[float, float] = (0.8, 1.2)
 
@@ -153,15 +153,15 @@
     def get_lut(self, rng: np.random.Generator) -> np.ndarray:
         lut = np.linspace(0, 1, num=256, dtype='f4')
 
         max_gamma = 1 + self.gamma
         lut **= rng.uniform(1 / max_gamma, max_gamma)
         lut *= 255
 
-        return lut.clip(0, 255).astype('u1')  # type: ignore
+        return lut.clip(0, 255).astype('u1')
 
 
 @dataclass
 class HsvShift(_LutTransform):
     max_shift: int = 20
 
     def get_lut(self, rng: np.random.Generator) -> list[np.ndarray]:
@@ -296,23 +296,28 @@
     sigma: float = 50
     inter: InitVar[str] = 'LINEAR'
     _inter: int = field(init=False)
 
     def __post_init__(self, inter: str):
         self._inter = getattr(cv2, f'INTER_{inter}')
 
-    def prepare(self, rng: np.random.Generator, /, image: np.ndarray,
-                **_) -> dict[str, Any]:
+    def prepare(self,
+                rng: np.random.Generator,
+                /,
+                image: np.ndarray | None = None,
+                **_) -> dict[str, Any] | None:
+        if image is None:
+            return None
         offsets = rng.random((2, *image.shape[:2]), dtype='f4')
         offsets *= self.scale * 2
         offsets -= self.scale
 
         for dim, (off, size) in enumerate(zip(offsets, image.shape[:2])):
             shape = np.where(np.arange(2) == dim, size, 1)
-            off += np.arange(size).reshape(shape)
+            off += np.arange(size).reshape(shape)  # noqa: PLW2901
             cv2.GaussianBlur(off, (17, 17), self.sigma, dst=off)
         return {'offsets': offsets[::-1]}
 
     def _apply(self, image: np.ndarray, inter: int, **params) -> np.ndarray:
         map_x, map_y = params['offsets']
         return cv2.remap(
             image, map_x, map_y, inter, borderMode=cv2.BORDER_REFLECT_101)
```

### Comparing `glow-0.11.3/glow/transforms/core.py` & `glow-0.12.7/src/glow/transforms/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,31 +62,34 @@
     _key = 'mask'
 
     def mask(self, mask: np.ndarray, rng: np.random.Generator) -> np.ndarray:
         raise NotImplementedError
 
 
 class DualStageTransform(Transform):
-    _keys: frozenset[str] = frozenset({'image', 'mask'})
+    _keys = frozenset[str]({'image', 'mask'})
 
-    def prepare(self, rng: np.random.Generator, /, **data) -> dict[str, Any]:
+    def prepare(self, rng: np.random.Generator, /,
+                **data) -> dict[str, Any] | None:
         return {}
 
     def image(self, image: np.ndarray, **params) -> np.ndarray:
         return image
 
     def mask(self, mask: np.ndarray, **params) -> np.ndarray:
         return mask
 
     @final
     def __call__(self, rng: np.random.Generator, /, **data) -> dict[str, Any]:
         if unknown_keys := {*data} - self._keys:
             raise ValueError(f'Got unknown keys in data: {unknown_keys}')
 
         params = self.prepare(rng, **data)
+        if params is None:
+            return data
         return {
             key: getattr(self, key)(value, **params)
             for key, value in data.items() if value is not None
         }
 
 
 @final
```

### Comparing `glow-0.11.3/glow/transforms/functional/core.py` & `glow-0.12.7/src/glow/transforms/functional/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+from __future__ import annotations
+
 __all__ = ['affine', 'flip', 'grid_shuffle', 'mask_dropout']
 
 import cv2
 import numpy as np
 
 
 def grid_shuffle(image: np.ndarray,
-                 mask: np.ndarray = None,
+                 mask: np.ndarray | None = None,
                  *,
                  rng: np.random.Generator,
                  grid=4) -> tuple[np.ndarray, ...]:
     axes = (
         np.linspace(0, size, grid + 1, dtype=np.int_)
         for size in image.shape[:2])
     mats = np.stack(np.meshgrid(*axes, indexing='ij'))
@@ -37,15 +39,15 @@
 
     results = []
     for v in sources:
         new_v = np.empty_like(v)
         for (y2, x2), (y1, x1), (ys, xs) in tiles:
             new_v[y2:y2 + ys, x2:x2 + xs] = v[y1:y1 + ys, x1:x1 + xs]
         results.append(new_v)
-    return tuple(results)
+    return *results,
 
 
 def affine(image: np.ndarray,
            skew: float,
            angle: float,
            scale: float,
            inter: int = cv2.INTER_LINEAR,
@@ -63,15 +65,15 @@
     mat[:, 2] += center  # restore center
 
     flags = inter + cv2.WARP_INVERSE_MAP
     return cv2.warpAffine(
         image, mat, image.shape[:2], flags=flags, borderMode=border)
 
 
-def flip(image: np.ndarray, ud: bool, lr: bool, rot90: bool) -> np.ndarray:
+def flip(image: np.ndarray, *, ud: bool, lr: bool, rot90: bool) -> np.ndarray:
     if ud:
         image = image[::-1, :]
     if lr:
         image = image[:, ::-1]
     if rot90:
         image = np.rot90(image, axes=(0, 1))
     return np.ascontiguousarray(image)
@@ -117,12 +119,12 @@
     assert 0 <= qbits < 8
     peak = 256 << qbits
 
     lut = np.linspace(0, 1, num=257, dtype='f4')
     lut **= y
     lut *= peak  # Increase precision
     lut = lut.astype('u2')
-    lut = lut.clip(0, peak - 1)  # type: ignore  # Remove overshoot
+    lut = lut.clip(0, peak - 1)  # Remove overshoot
 
     arr = rng.integers(lut[arr], lut[1:][arr], dtype='u2', endpoint=True)
     arr >>= qbits  # Round to 8 bits
     return arr.astype('u1')
```

### Comparing `glow-0.11.3/glow/transforms/functional/numba.py` & `glow-0.12.7/src/glow/transforms/functional/numba.py`

 * *Files 11% similar despite different names*

```diff
@@ -46,22 +46,22 @@
 def dither(image: np.ndarray,
            bits: int = 3,
            kind: _DitherKind = 'stucki') -> np.ndarray:
     mat = _MATRICES[kind]
     assert image.dtype == 'u1'
     if image.ndim == 3:
         mat = mat[..., None]
-        channel_pad = [(0, 0)]
+        channel_pad = [[0, 0]]
     else:
         channel_pad = []
-    image = np.pad(image, [(0, 2), (2, 2)] + channel_pad, mode='constant')
+    image = np.pad(image, [[0, 2], [2, 2], *channel_pad])
 
     dtype = image.dtype
     if dtype == 'uint8':
         max_value = 256
         image = image.astype('i2')
     else:
         max_value = 1
     quant = max_value / 2 ** bits
 
     image = _dither(image, mat, quant)
-    return image.clip(0, max_value - quant).astype(dtype)  # type: ignore
+    return image.clip(0, max_value - quant).astype(dtype)
```

