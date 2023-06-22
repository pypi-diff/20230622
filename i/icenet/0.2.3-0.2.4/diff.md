# Comparing `tmp/icenet-0.2.3.tar.gz` & `tmp/icenet-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/jambyr/code/ai-lab/icenet/icenet/dist/.tmp-kcc0nawy/icenet-0.2.3.tar", last modified: Tue Mar  7 14:12:29 2023, max compression
+gzip compressed data, was "/home/jambyr/code/ai-lab/icenet/icenet/dist/.tmp-olhoky7y/icenet-0.2.4.tar", last modified: Thu Jun 22 07:43:10 2023, max compression
```

## Comparing `icenet-0.2.3.tar` & `icenet-0.2.4.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-03-07 14:12:29.456933 icenet-0.2.3/
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      291 2023-03-07 11:38:13.000000 icenet-0.2.3/AUTHORS.rst
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     3207 2022-11-22 16:24:34.000000 icenet-0.2.3/CONTRIBUTING.rst
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      458 2022-11-22 16:27:46.000000 icenet-0.2.3/HISTORY.rst
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     1083 2022-02-03 18:27:11.000000 icenet-0.2.3/LICENSE
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      261 2022-11-22 15:17:37.000000 icenet-0.2.3/MANIFEST.in
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     1418 2023-03-07 14:12:29.456933 icenet-0.2.3/PKG-INFO
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      545 2023-03-06 14:06:50.000000 icenet-0.2.3/README.md
-drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-03-07 14:12:29.441933 icenet-0.2.3/docs/
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      607 2022-11-22 16:40:49.000000 icenet-0.2.3/docs/Makefile
-drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-03-07 14:12:29.435933 icenet-0.2.3/docs/_build/
-drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-03-07 14:12:29.435933 icenet-0.2.3/docs/_build/html/
-drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-03-07 14:12:29.443934 icenet-0.2.3/docs/_build/html/_static/
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      673 2022-11-22 15:22:19.000000 icenet-0.2.3/docs/_build/html/_static/ajax-loader.gif
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      756 2022-11-22 15:22:19.000000 icenet-0.2.3/docs/_build/html/_static/comment-bright.png
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      829 2022-11-22 15:22:19.000000 icenet-0.2.3/docs/_build/html/_static/comment-close.png
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      641 2022-11-22 15:22:19.000000 icenet-0.2.3/docs/_build/html/_static/comment.png
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      222 2022-11-22 15:22:19.000000 icenet-0.2.3/docs/_build/html/_static/down-pressed.png
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      202 2022-11-22 15:22:19.000000 icenet-0.2.3/docs/_build/html/_static/down.png
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      286 2022-11-22 15:22:19.000000 icenet-0.2.3/docs/_build/html/_static/file.png
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)       90 2022-11-22 15:22:19.000000 icenet-0.2.3/docs/_build/html/_static/minus.png
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)       90 2022-11-22 15:22:19.000000 icenet-0.2.3/docs/_build/html/_static/plus.png
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      214 2022-11-22 15:22:19.000000 icenet-0.2.3/docs/_build/html/_static/up-pressed.png
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      203 2022-11-22 15:22:19.000000 icenet-0.2.3/docs/_build/html/_static/up.png
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)       28 2022-02-03 18:27:11.000000 icenet-0.2.3/docs/authors.rst
--rwxrwxr-x   0 jambyr    (1000) jambyr    (1000)     4893 2023-02-02 11:23:27.000000 icenet-0.2.3/docs/conf.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)       33 2022-02-03 18:27:11.000000 icenet-0.2.3/docs/contributing.rst
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)       28 2022-02-03 18:27:11.000000 icenet-0.2.3/docs/history.rst
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      380 2022-11-22 17:17:40.000000 icenet-0.2.3/docs/icenet.data.datasets.rst
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     1099 2022-11-22 16:36:53.000000 icenet-0.2.3/docs/icenet.data.interfaces.rst
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      872 2022-11-22 17:17:40.000000 icenet-0.2.3/docs/icenet.data.loaders.rst
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     1254 2022-11-22 16:36:53.000000 icenet-0.2.3/docs/icenet.data.processors.rst
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     1176 2022-11-22 16:42:51.000000 icenet-0.2.3/docs/icenet.data.rst
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      505 2022-11-22 16:37:49.000000 icenet-0.2.3/docs/icenet.data.sic.rst
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     1238 2022-11-22 16:38:22.000000 icenet-0.2.3/docs/icenet.model.rst
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      671 2022-11-22 16:38:41.000000 icenet-0.2.3/docs/icenet.plotting.rst
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     1122 2022-11-22 16:39:14.000000 icenet-0.2.3/docs/icenet.process.rst
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      168 2022-11-22 16:39:20.000000 icenet-0.2.3/docs/icenet.results.rst
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      444 2023-02-02 12:45:59.000000 icenet-0.2.3/docs/icenet.rst
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      343 2022-11-22 17:17:40.000000 icenet-0.2.3/docs/icenet.tests.rst
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      303 2022-11-22 16:39:50.000000 icenet-0.2.3/docs/index.rst
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     1110 2022-11-22 16:40:33.000000 icenet-0.2.3/docs/installation.rst
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      768 2022-11-22 16:40:49.000000 icenet-0.2.3/docs/make.bat
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)       55 2023-02-02 12:45:59.000000 icenet-0.2.3/docs/modules.rst
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)       55 2022-05-19 22:27:19.000000 icenet-0.2.3/docs/readme.rst
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)       67 2022-11-22 16:41:07.000000 icenet-0.2.3/docs/usage.rst
-drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-03-07 14:12:29.444934 icenet-0.2.3/icenet/
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      217 2023-03-07 14:11:43.000000 icenet-0.2.3/icenet/__init__.py
-drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-03-07 14:12:29.446934 icenet-0.2.3/icenet/data/
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)        0 2022-02-03 09:47:39.000000 icenet-0.2.3/icenet/data/__init__.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     7001 2023-03-07 11:38:13.000000 icenet-0.2.3/icenet/data/cli.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     9106 2023-02-02 11:23:27.000000 icenet-0.2.3/icenet/data/dataset.py
-drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-03-07 14:12:29.447934 icenet-0.2.3/icenet/data/datasets/
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)        0 2022-06-18 16:56:02.000000 icenet-0.2.3/icenet/data/datasets/__init__.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     8145 2023-03-07 11:38:13.000000 icenet-0.2.3/icenet/data/datasets/utils.py
-drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-03-07 14:12:29.448933 icenet-0.2.3/icenet/data/interfaces/
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)        0 2022-02-03 09:47:39.000000 icenet-0.2.3/icenet/data/interfaces/__init__.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)    10896 2023-03-07 11:38:13.000000 icenet-0.2.3/icenet/data/interfaces/cds.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     6830 2023-03-07 11:38:13.000000 icenet-0.2.3/icenet/data/interfaces/cmems.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)    23752 2023-03-07 11:38:13.000000 icenet-0.2.3/icenet/data/interfaces/downloader.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     9244 2023-03-07 11:38:13.000000 icenet-0.2.3/icenet/data/interfaces/esgf.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)    14765 2023-03-07 11:38:13.000000 icenet-0.2.3/icenet/data/interfaces/mars.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     7838 2022-11-22 15:28:41.000000 icenet-0.2.3/icenet/data/interfaces/utils.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     3044 2022-12-22 13:08:59.000000 icenet-0.2.3/icenet/data/loader.py
-drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-03-07 14:12:29.449933 icenet-0.2.3/icenet/data/loaders/
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     1454 2022-12-22 13:08:59.000000 icenet-0.2.3/icenet/data/loaders/__init__.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)    11461 2023-02-02 11:23:27.000000 icenet-0.2.3/icenet/data/loaders/base.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)    17301 2023-02-02 11:23:27.000000 icenet-0.2.3/icenet/data/loaders/dask.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      864 2022-11-22 15:29:16.000000 icenet-0.2.3/icenet/data/loaders/stdlib.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     1536 2022-09-29 11:27:40.000000 icenet-0.2.3/icenet/data/loaders/utils.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)    23424 2023-03-07 11:38:13.000000 icenet-0.2.3/icenet/data/process.py
-drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-03-07 14:12:29.450934 icenet-0.2.3/icenet/data/processors/
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)        0 2022-02-03 09:47:39.000000 icenet-0.2.3/icenet/data/processors/__init__.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     1703 2023-03-07 11:38:13.000000 icenet-0.2.3/icenet/data/processors/cmip.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      944 2022-11-22 15:29:37.000000 icenet-0.2.3/icenet/data/processors/era5.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      951 2023-02-02 11:23:27.000000 icenet-0.2.3/icenet/data/processors/hres.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     3534 2023-03-07 11:38:13.000000 icenet-0.2.3/icenet/data/processors/meta.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      940 2022-11-22 15:29:55.000000 icenet-0.2.3/icenet/data/processors/oras5.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     2034 2022-11-22 15:30:01.000000 icenet-0.2.3/icenet/data/processors/osi.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     6512 2023-03-07 11:38:13.000000 icenet-0.2.3/icenet/data/processors/utils.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)    10779 2023-03-07 11:38:13.000000 icenet-0.2.3/icenet/data/producers.py
-drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-03-07 14:12:29.451933 icenet-0.2.3/icenet/data/sic/
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)        0 2022-02-03 09:47:39.000000 icenet-0.2.3/icenet/data/sic/__init__.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)    10059 2023-02-02 11:23:27.000000 icenet-0.2.3/icenet/data/sic/mask.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)    20647 2023-03-07 11:38:13.000000 icenet-0.2.3/icenet/data/sic/osisaf.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)       64 2022-06-15 11:18:18.000000 icenet-0.2.3/icenet/data/sic/utils.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     7074 2023-03-07 11:38:13.000000 icenet-0.2.3/icenet/data/utils.py
-drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-03-07 14:12:29.453934 icenet-0.2.3/icenet/model/
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)        0 2022-02-03 09:47:39.000000 icenet-0.2.3/icenet/model/__init__.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     4118 2022-11-22 15:32:01.000000 icenet-0.2.3/icenet/model/callbacks.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     1029 2023-03-07 11:38:13.000000 icenet-0.2.3/icenet/model/losses.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     9515 2023-03-07 11:38:13.000000 icenet-0.2.3/icenet/model/metrics.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     7903 2023-03-07 11:38:13.000000 icenet-0.2.3/icenet/model/models.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     7211 2022-11-22 16:15:02.000000 icenet-0.2.3/icenet/model/predict.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)    16105 2022-12-22 13:08:59.000000 icenet-0.2.3/icenet/model/train.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     3921 2022-11-22 16:15:24.000000 icenet-0.2.3/icenet/model/utils.py
-drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-03-07 14:12:29.453934 icenet-0.2.3/icenet/plotting/
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)        0 2022-02-03 09:47:39.000000 icenet-0.2.3/icenet/plotting/__init__.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     2449 2022-11-22 16:15:33.000000 icenet-0.2.3/icenet/plotting/data.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)    62601 2023-03-07 14:11:35.000000 icenet-0.2.3/icenet/plotting/forecast.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      250 2022-11-22 16:15:42.000000 icenet-0.2.3/icenet/plotting/trend.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)    14158 2023-03-07 11:38:13.000000 icenet-0.2.3/icenet/plotting/utils.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)    12356 2023-03-07 11:38:13.000000 icenet-0.2.3/icenet/plotting/video.py
-drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-03-07 14:12:29.455933 icenet-0.2.3/icenet/process/
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)        0 2022-02-03 09:47:39.000000 icenet-0.2.3/icenet/process/__init__.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     2491 2022-11-22 16:15:59.000000 icenet-0.2.3/icenet/process/azure.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     5714 2023-03-07 11:38:13.000000 icenet-0.2.3/icenet/process/forecasts.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     1447 2022-11-22 16:16:07.000000 icenet-0.2.3/icenet/process/local.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)    11256 2023-03-07 11:38:13.000000 icenet-0.2.3/icenet/process/predict.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)        0 2022-02-03 09:47:39.000000 icenet-0.2.3/icenet/process/train.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      874 2022-08-11 12:13:43.000000 icenet-0.2.3/icenet/process/utils.py
-drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-03-07 14:12:29.455933 icenet-0.2.3/icenet/results/
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)        0 2022-02-03 09:47:39.000000 icenet-0.2.3/icenet/results/__init__.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     1674 2023-02-02 11:23:27.000000 icenet-0.2.3/icenet/results/threshold.py
-drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-03-07 14:12:29.456933 icenet-0.2.3/icenet/tests/
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)       36 2022-11-22 15:25:11.000000 icenet-0.2.3/icenet/tests/__init__.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      758 2023-03-07 11:38:13.000000 icenet-0.2.3/icenet/tests/test_entry_points.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      540 2023-03-07 11:38:13.000000 icenet-0.2.3/icenet/tests/test_mod.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     2580 2023-03-07 11:38:13.000000 icenet-0.2.3/icenet/utils.py
-drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-03-07 14:12:29.445933 icenet-0.2.3/icenet.egg-info/
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     1418 2023-03-07 14:12:29.000000 icenet-0.2.3/icenet.egg-info/PKG-INFO
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     2846 2023-03-07 14:12:29.000000 icenet-0.2.3/icenet.egg-info/SOURCES.txt
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)        1 2023-03-07 14:12:29.000000 icenet-0.2.3/icenet.egg-info/dependency_links.txt
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     2155 2023-03-07 14:12:29.000000 icenet-0.2.3/icenet.egg-info/entry_points.txt
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)        1 2023-03-07 14:12:29.000000 icenet-0.2.3/icenet.egg-info/not-zip-safe
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      421 2023-03-07 14:12:29.000000 icenet-0.2.3/icenet.egg-info/requires.txt
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)        7 2023-03-07 14:12:29.000000 icenet-0.2.3/icenet.egg-info/top_level.txt
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      173 2023-03-07 14:12:29.456933 icenet-0.2.3/setup.cfg
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     4415 2023-03-07 11:38:13.000000 icenet-0.2.3/setup.py
+drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-06-22 07:43:10.112728 icenet-0.2.4/
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      291 2023-03-07 11:38:13.000000 icenet-0.2.4/AUTHORS.rst
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     3207 2022-11-22 16:24:34.000000 icenet-0.2.4/CONTRIBUTING.rst
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      458 2022-11-22 16:27:46.000000 icenet-0.2.4/HISTORY.rst
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     1083 2022-02-03 18:27:11.000000 icenet-0.2.4/LICENSE
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      261 2022-11-22 15:17:37.000000 icenet-0.2.4/MANIFEST.in
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     3212 2023-06-22 07:43:10.112728 icenet-0.2.4/PKG-INFO
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     2339 2023-06-22 07:41:55.000000 icenet-0.2.4/README.md
+drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-06-22 07:43:10.066727 icenet-0.2.4/docs/
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      607 2022-11-22 16:40:49.000000 icenet-0.2.4/docs/Makefile
+drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-06-22 07:43:10.036726 icenet-0.2.4/docs/_build/
+drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-06-22 07:43:10.036726 icenet-0.2.4/docs/_build/html/
+drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-06-22 07:43:10.072727 icenet-0.2.4/docs/_build/html/_static/
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      673 2022-11-22 15:22:19.000000 icenet-0.2.4/docs/_build/html/_static/ajax-loader.gif
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      756 2022-11-22 15:22:19.000000 icenet-0.2.4/docs/_build/html/_static/comment-bright.png
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      829 2022-11-22 15:22:19.000000 icenet-0.2.4/docs/_build/html/_static/comment-close.png
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      641 2022-11-22 15:22:19.000000 icenet-0.2.4/docs/_build/html/_static/comment.png
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      222 2022-11-22 15:22:19.000000 icenet-0.2.4/docs/_build/html/_static/down-pressed.png
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      202 2022-11-22 15:22:19.000000 icenet-0.2.4/docs/_build/html/_static/down.png
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      286 2022-11-22 15:22:19.000000 icenet-0.2.4/docs/_build/html/_static/file.png
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)       90 2022-11-22 15:22:19.000000 icenet-0.2.4/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)       90 2022-11-22 15:22:19.000000 icenet-0.2.4/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      214 2022-11-22 15:22:19.000000 icenet-0.2.4/docs/_build/html/_static/up-pressed.png
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      203 2022-11-22 15:22:19.000000 icenet-0.2.4/docs/_build/html/_static/up.png
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)       28 2022-02-03 18:27:11.000000 icenet-0.2.4/docs/authors.rst
+-rwxrwxr-x   0 jambyr    (1000) jambyr    (1000)     4893 2023-02-02 11:23:27.000000 icenet-0.2.4/docs/conf.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)       33 2022-02-03 18:27:11.000000 icenet-0.2.4/docs/contributing.rst
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)       28 2022-02-03 18:27:11.000000 icenet-0.2.4/docs/history.rst
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      380 2022-11-22 17:17:40.000000 icenet-0.2.4/docs/icenet.data.datasets.rst
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     1099 2022-11-22 16:36:53.000000 icenet-0.2.4/docs/icenet.data.interfaces.rst
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      872 2022-11-22 17:17:40.000000 icenet-0.2.4/docs/icenet.data.loaders.rst
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     1254 2022-11-22 16:36:53.000000 icenet-0.2.4/docs/icenet.data.processors.rst
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     1176 2022-11-22 16:42:51.000000 icenet-0.2.4/docs/icenet.data.rst
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      505 2022-11-22 16:37:49.000000 icenet-0.2.4/docs/icenet.data.sic.rst
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     1238 2022-11-22 16:38:22.000000 icenet-0.2.4/docs/icenet.model.rst
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      671 2022-11-22 16:38:41.000000 icenet-0.2.4/docs/icenet.plotting.rst
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     1122 2022-11-22 16:39:14.000000 icenet-0.2.4/docs/icenet.process.rst
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      168 2022-11-22 16:39:20.000000 icenet-0.2.4/docs/icenet.results.rst
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      444 2023-02-02 12:45:59.000000 icenet-0.2.4/docs/icenet.rst
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      343 2022-11-22 17:17:40.000000 icenet-0.2.4/docs/icenet.tests.rst
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      303 2022-11-22 16:39:50.000000 icenet-0.2.4/docs/index.rst
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     1110 2022-11-22 16:40:33.000000 icenet-0.2.4/docs/installation.rst
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      768 2022-11-22 16:40:49.000000 icenet-0.2.4/docs/make.bat
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)       55 2023-02-02 12:45:59.000000 icenet-0.2.4/docs/modules.rst
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)       55 2022-05-19 22:27:19.000000 icenet-0.2.4/docs/readme.rst
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)       67 2022-11-22 16:41:07.000000 icenet-0.2.4/docs/usage.rst
+drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-06-22 07:43:10.072727 icenet-0.2.4/icenet/
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      217 2023-06-22 07:41:55.000000 icenet-0.2.4/icenet/__init__.py
+drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-06-22 07:43:10.076727 icenet-0.2.4/icenet/data/
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)        0 2022-02-03 09:47:39.000000 icenet-0.2.4/icenet/data/__init__.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     7193 2023-06-22 07:41:55.000000 icenet-0.2.4/icenet/data/cli.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     9106 2023-02-02 11:23:27.000000 icenet-0.2.4/icenet/data/dataset.py
+drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-06-22 07:43:10.077727 icenet-0.2.4/icenet/data/datasets/
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)        0 2022-06-18 16:56:02.000000 icenet-0.2.4/icenet/data/datasets/__init__.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     8145 2023-03-07 11:38:13.000000 icenet-0.2.4/icenet/data/datasets/utils.py
+drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-06-22 07:43:10.081728 icenet-0.2.4/icenet/data/interfaces/
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)        0 2022-02-03 09:47:39.000000 icenet-0.2.4/icenet/data/interfaces/__init__.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)    10896 2023-03-07 11:38:13.000000 icenet-0.2.4/icenet/data/interfaces/cds.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     6830 2023-03-07 11:38:13.000000 icenet-0.2.4/icenet/data/interfaces/cmems.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)    23972 2023-06-22 07:41:55.000000 icenet-0.2.4/icenet/data/interfaces/downloader.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     9244 2023-03-07 11:38:13.000000 icenet-0.2.4/icenet/data/interfaces/esgf.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)    14765 2023-03-07 11:38:13.000000 icenet-0.2.4/icenet/data/interfaces/mars.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     7838 2022-11-22 15:28:41.000000 icenet-0.2.4/icenet/data/interfaces/utils.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     4068 2023-06-22 07:41:55.000000 icenet-0.2.4/icenet/data/loader.py
+drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-06-22 07:43:10.085728 icenet-0.2.4/icenet/data/loaders/
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     1454 2022-12-22 13:08:59.000000 icenet-0.2.4/icenet/data/loaders/__init__.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)    11679 2023-06-22 07:41:55.000000 icenet-0.2.4/icenet/data/loaders/base.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)    17301 2023-06-14 13:21:26.000000 icenet-0.2.4/icenet/data/loaders/dask.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      864 2022-11-22 15:29:16.000000 icenet-0.2.4/icenet/data/loaders/stdlib.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     1536 2022-09-29 11:27:40.000000 icenet-0.2.4/icenet/data/loaders/utils.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)    23399 2023-06-22 07:41:55.000000 icenet-0.2.4/icenet/data/process.py
+drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-06-22 07:43:10.087728 icenet-0.2.4/icenet/data/processors/
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)        0 2022-02-03 09:47:39.000000 icenet-0.2.4/icenet/data/processors/__init__.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     1747 2023-06-22 07:41:55.000000 icenet-0.2.4/icenet/data/processors/cmip.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      988 2023-06-22 07:41:55.000000 icenet-0.2.4/icenet/data/processors/era5.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      995 2023-06-22 07:41:55.000000 icenet-0.2.4/icenet/data/processors/hres.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     3534 2023-03-07 11:38:13.000000 icenet-0.2.4/icenet/data/processors/meta.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      984 2023-06-22 07:41:55.000000 icenet-0.2.4/icenet/data/processors/oras5.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     2078 2023-06-22 07:41:55.000000 icenet-0.2.4/icenet/data/processors/osi.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     6512 2023-03-07 11:38:13.000000 icenet-0.2.4/icenet/data/processors/utils.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)    10779 2023-03-07 11:38:13.000000 icenet-0.2.4/icenet/data/producers.py
+drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-06-22 07:43:10.088728 icenet-0.2.4/icenet/data/sic/
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)        0 2022-02-03 09:47:39.000000 icenet-0.2.4/icenet/data/sic/__init__.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)    10059 2023-02-02 11:23:27.000000 icenet-0.2.4/icenet/data/sic/mask.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)    24591 2023-06-22 07:41:55.000000 icenet-0.2.4/icenet/data/sic/osisaf.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)       64 2022-06-15 11:18:18.000000 icenet-0.2.4/icenet/data/sic/utils.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     7074 2023-03-07 11:38:13.000000 icenet-0.2.4/icenet/data/utils.py
+drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-06-22 07:43:10.092728 icenet-0.2.4/icenet/model/
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)        0 2022-02-03 09:47:39.000000 icenet-0.2.4/icenet/model/__init__.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     4118 2022-11-22 15:32:01.000000 icenet-0.2.4/icenet/model/callbacks.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     1029 2023-03-07 11:38:13.000000 icenet-0.2.4/icenet/model/losses.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     9515 2023-03-07 11:38:13.000000 icenet-0.2.4/icenet/model/metrics.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     7903 2023-03-07 11:38:13.000000 icenet-0.2.4/icenet/model/models.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     7201 2023-06-22 07:41:55.000000 icenet-0.2.4/icenet/model/predict.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)    16918 2023-06-22 07:41:55.000000 icenet-0.2.4/icenet/model/train.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     3921 2022-11-22 16:15:24.000000 icenet-0.2.4/icenet/model/utils.py
+drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-06-22 07:43:10.099728 icenet-0.2.4/icenet/plotting/
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)        0 2022-02-03 09:47:39.000000 icenet-0.2.4/icenet/plotting/__init__.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     4593 2023-06-22 07:41:55.000000 icenet-0.2.4/icenet/plotting/data.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)    75295 2023-06-22 07:41:55.000000 icenet-0.2.4/icenet/plotting/forecast.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      250 2022-11-22 16:15:42.000000 icenet-0.2.4/icenet/plotting/trend.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)    15077 2023-06-22 07:41:55.000000 icenet-0.2.4/icenet/plotting/utils.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)    12356 2023-03-07 11:38:13.000000 icenet-0.2.4/icenet/plotting/video.py
+drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-06-22 07:43:10.106728 icenet-0.2.4/icenet/process/
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)        0 2022-02-03 09:47:39.000000 icenet-0.2.4/icenet/process/__init__.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     2491 2022-11-22 16:15:59.000000 icenet-0.2.4/icenet/process/azure.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     5714 2023-03-07 11:38:13.000000 icenet-0.2.4/icenet/process/forecasts.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     1447 2022-11-22 16:16:07.000000 icenet-0.2.4/icenet/process/local.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)    11256 2023-03-07 11:38:13.000000 icenet-0.2.4/icenet/process/predict.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)        0 2022-02-03 09:47:39.000000 icenet-0.2.4/icenet/process/train.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      874 2022-08-11 12:13:43.000000 icenet-0.2.4/icenet/process/utils.py
+drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-06-22 07:43:10.108728 icenet-0.2.4/icenet/results/
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)        0 2022-02-03 09:47:39.000000 icenet-0.2.4/icenet/results/__init__.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     1674 2023-02-02 11:23:27.000000 icenet-0.2.4/icenet/results/threshold.py
+drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-06-22 07:43:10.110728 icenet-0.2.4/icenet/tests/
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)       36 2022-11-22 15:25:11.000000 icenet-0.2.4/icenet/tests/__init__.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      758 2023-03-07 11:38:13.000000 icenet-0.2.4/icenet/tests/test_entry_points.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      540 2023-03-07 11:38:13.000000 icenet-0.2.4/icenet/tests/test_mod.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     2580 2023-03-07 11:38:13.000000 icenet-0.2.4/icenet/utils.py
+drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-06-22 07:43:10.074727 icenet-0.2.4/icenet.egg-info/
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     3212 2023-06-22 07:43:10.000000 icenet-0.2.4/icenet.egg-info/PKG-INFO
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     2846 2023-06-22 07:43:10.000000 icenet-0.2.4/icenet.egg-info/SOURCES.txt
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)        1 2023-06-22 07:43:10.000000 icenet-0.2.4/icenet.egg-info/dependency_links.txt
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     2159 2023-06-22 07:43:10.000000 icenet-0.2.4/icenet.egg-info/entry_points.txt
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)        1 2023-06-22 07:43:09.000000 icenet-0.2.4/icenet.egg-info/not-zip-safe
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      372 2023-06-22 07:43:10.000000 icenet-0.2.4/icenet.egg-info/requires.txt
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)        7 2023-06-22 07:43:10.000000 icenet-0.2.4/icenet.egg-info/top_level.txt
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      173 2023-06-22 07:43:10.114728 icenet-0.2.4/setup.cfg
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     4419 2023-06-22 07:41:55.000000 icenet-0.2.4/setup.py
```

### Comparing `icenet-0.2.3/CONTRIBUTING.rst` & `icenet-0.2.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `icenet-0.2.3/LICENSE` & `icenet-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `icenet-0.2.3/docs/Makefile` & `icenet-0.2.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `icenet-0.2.3/docs/_build/html/_static/ajax-loader.gif` & `icenet-0.2.4/docs/_build/html/_static/ajax-loader.gif`

 * *Files identical despite different names*

### Comparing `icenet-0.2.3/docs/_build/html/_static/comment-bright.png` & `icenet-0.2.4/docs/_build/html/_static/comment-bright.png`

 * *Files identical despite different names*

### Comparing `icenet-0.2.3/docs/_build/html/_static/comment-close.png` & `icenet-0.2.4/docs/_build/html/_static/comment-close.png`

 * *Files identical despite different names*

### Comparing `icenet-0.2.3/docs/_build/html/_static/comment.png` & `icenet-0.2.4/docs/_build/html/_static/comment.png`

 * *Files identical despite different names*

### Comparing `icenet-0.2.3/docs/conf.py` & `icenet-0.2.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.3/docs/icenet.data.interfaces.rst` & `icenet-0.2.4/docs/icenet.data.interfaces.rst`

 * *Files identical despite different names*

### Comparing `icenet-0.2.3/docs/icenet.data.loaders.rst` & `icenet-0.2.4/docs/icenet.data.loaders.rst`

 * *Files identical despite different names*

### Comparing `icenet-0.2.3/docs/icenet.data.processors.rst` & `icenet-0.2.4/docs/icenet.data.processors.rst`

 * *Files identical despite different names*

### Comparing `icenet-0.2.3/docs/icenet.data.rst` & `icenet-0.2.4/docs/icenet.data.rst`

 * *Files identical despite different names*

### Comparing `icenet-0.2.3/docs/icenet.model.rst` & `icenet-0.2.4/docs/icenet.model.rst`

 * *Files identical despite different names*

### Comparing `icenet-0.2.3/docs/icenet.plotting.rst` & `icenet-0.2.4/docs/icenet.plotting.rst`

 * *Files identical despite different names*

### Comparing `icenet-0.2.3/docs/icenet.process.rst` & `icenet-0.2.4/docs/icenet.process.rst`

 * *Files identical despite different names*

### Comparing `icenet-0.2.3/docs/installation.rst` & `icenet-0.2.4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `icenet-0.2.3/docs/make.bat` & `icenet-0.2.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `icenet-0.2.3/icenet/data/cli.py` & `icenet-0.2.4/icenet/data/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,14 +159,17 @@
     ap.add_argument("hemisphere", choices=("north", "south"))
 
     if dates:
         add_date_args(ap)
 
     ap.add_argument("-l", "--lag", type=int, default=2)
     ap.add_argument("-f", "--forecast", type=int, default=93)
+    ap.add_argument("-p", "--parallel-opens",
+                    type=bool, default=False, action="store_true",
+                    help="Allow xarray mfdataset to work with parallel opens")
 
     ap.add_argument("--abs",
                     help="Comma separated list of abs vars",
                     type=csv_arg,
                     default=[])
     ap.add_argument("--anom",
                     help="Comma separated list of abs vars",
```

### Comparing `icenet-0.2.3/icenet/data/dataset.py` & `icenet-0.2.4/icenet/data/dataset.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.3/icenet/data/datasets/utils.py` & `icenet-0.2.4/icenet/data/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.3/icenet/data/interfaces/cds.py` & `icenet-0.2.4/icenet/data/interfaces/cds.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.3/icenet/data/interfaces/cmems.py` & `icenet-0.2.4/icenet/data/interfaces/cmems.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.3/icenet/data/interfaces/downloader.py` & `icenet-0.2.4/icenet/data/interfaces/downloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,25 +60,25 @@
     regridded_dates = list()
     drop_vars = list() if drop_vars is None else drop_vars
 
     # Latlon files should in theory be aggregated and singular arrays
     # meaning we can naively open and interrogate the dates
     if check_latlon and os.path.exists(latlon_path):
         try:
-            latlon_dates = xr.open_dataarray(
+            latlon_dates = xr.open_dataset(
                 latlon_path,
                 drop_variables=drop_vars).time.values
             logging.debug("{} latlon dates already available in {}".format(
                 len(latlon_dates), latlon_path
             ))
         except ValueError:
             logging.warning("Latlon {} dates not readable, ignoring file")
 
     if check_regridded and os.path.exists(regridded_name):
-        regridded_dates = xr.open_dataarray(
+        regridded_dates = xr.open_dataset(
             regridded_name,
             drop_variables=drop_vars).time.values
         logging.debug("{} regridded dates already available in {}".format(
             len(regridded_dates), regridded_name
         ))
 
     exclude_dates = list(set(latlon_dates).union(set(regridded_dates)))
@@ -101,23 +101,25 @@
     drop_variables = list() if drop_variables is None else drop_variables
 
     if other_datafile is not None:
         (datafile_path, new_filename) = os.path.split(new_datafile)
         moved_new_datafile = \
             os.path.join(datafile_path, "new.{}".format(new_filename))
         os.rename(new_datafile, moved_new_datafile)
-        d1 = xr.open_dataset(moved_new_datafile,
-                             drop_variables=drop_variables)
+        d1 = xr.open_dataarray(moved_new_datafile,
+                               drop_variables=drop_variables)
 
         logging.info("Concatenating with previous data {}".format(
             other_datafile
         ))
-        d2 = xr.open_dataset(other_datafile,
-                             drop_variables=drop_variables)
-        new_ds = xr.concat([d1, d2], dim="time").sortby("time")
+        d2 = xr.open_dataarray(other_datafile,
+                               drop_variables=drop_variables)
+        new_ds = xr.concat([d1, d2], dim="time").\
+            sortby("time").\
+            drop_duplicates("time", keep="first")
 
         logging.info("Saving merged data to {}... ".
                      format(new_datafile))
         new_ds.to_netcdf(new_datafile)
         os.unlink(other_datafile)
         os.unlink(moved_new_datafile)
 
@@ -255,15 +257,18 @@
         var = var_prefix if not level else \
             "{}{}".format(var_prefix, level)
         var_folder = self.get_data_var_folder(var)
 
         latlon_path, regridded_name = \
             self.get_req_filenames(var_folder, req_dates[0])
 
-        req_dates = filter_dates_on_data(latlon_path, regridded_name, req_dates)
+        req_dates = filter_dates_on_data(latlon_path,
+                                         regridded_name,
+                                         req_dates,
+                                         drop_vars=self._drop_vars)
 
         if len(req_dates):
             if self._download:
                 with tempfile.TemporaryDirectory() as tmpdir:
                     tmp_latlon_path = os.path.join(tmpdir, os.path.basename("{}.download".format(latlon_path)))
 
                     self.download_method(var,
```

### Comparing `icenet-0.2.3/icenet/data/interfaces/esgf.py` & `icenet-0.2.4/icenet/data/interfaces/esgf.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.3/icenet/data/interfaces/mars.py` & `icenet-0.2.4/icenet/data/interfaces/mars.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.3/icenet/data/interfaces/utils.py` & `icenet-0.2.4/icenet/data/interfaces/utils.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.3/icenet/data/loaders/__init__.py` & `icenet-0.2.4/icenet/data/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.3/icenet/data/loaders/base.py` & `icenet-0.2.4/icenet/data/loaders/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -314,14 +314,20 @@
 
         logging.info("Writing configuration to {}".format(output_path))
 
         with open(output_path, "w") as fh:
             json.dump(configuration, fh, indent=4, default=_serialize)
 
     @property
+    def channel_names(self):
+        return ["{}_{}".format(nom, idx) if idx_qty > 1 else nom
+                for nom, idx_qty in self._channels.items()
+                for idx in range(1, idx_qty + 1)]
+
+    @property
     def config(self):
         return self._config
 
     @property
     def dates_override(self):
         return self._dates_override
```

### Comparing `icenet-0.2.3/icenet/data/loaders/dask.py` & `icenet-0.2.4/icenet/data/loaders/dask.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.3/icenet/data/loaders/stdlib.py` & `icenet-0.2.4/icenet/data/loaders/stdlib.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.3/icenet/data/loaders/utils.py` & `icenet-0.2.4/icenet/data/loaders/utils.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.3/icenet/data/process.py` & `icenet-0.2.4/icenet/data/process.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,16 @@
     :param linear_trends: 
     :param linear_trend_days: 
     :param meta_vars:
     :param missing_dates:
     :param minmax:
     :param no_normalise: 
     :param path:
-    :param ref_procdir: 
+    :param parallel_opens:
+    :param ref_procdir:
     :param source_data:
     :param update_key:
     :param update_loader: 
     """
 
     DATE_FORMAT = "%Y_%m_%d"
 
@@ -67,14 +68,15 @@
                  linear_trends=tuple(["siconca"]),
                  linear_trend_steps=7,
                  meta_vars=tuple(),
                  missing_dates=tuple(),
                  minmax=True,
                  no_normalise=tuple(["siconca"]),
                  path=os.path.join(".", "processed"),
+                 parallel_opens=False,
                  ref_procdir=None,
                  source_data=os.path.join(".", "data"),
                  update_key=None,
                  update_loader=True,
                  **kwargs):
         super().__init__(identifier,
                          source_data,
@@ -97,14 +99,15 @@
         self._dtype = dtype
         self._exclude_vars = exclude_vars
         self._linear_trends = linear_trends
         self._missing_dates = list(missing_dates)
         self._no_normalise = no_normalise
         self._normalise = self._normalise_array_mean \
             if not minmax else self._normalise_array_scaling
+        self._parallel = parallel_opens
         self._refdir = ref_procdir
         self._update_key = self.identifier if not update_key else update_key
         self._update_loader = os.path.join(".",
                                            "loader.{}.json".format(name)) \
             if update_loader else None
 
         if type(linear_trend_steps) == int:
@@ -340,17 +343,15 @@
                                # Solves issue with inheriting files without
                                # time dimension (only having coordinate)
                                combine="nested",
                                concat_dim="time",
                                coords="minimal",
                                compat="override",
                                drop_variables=("lat", "lon"),
-                               # TODO: Wasteful on small sets, but much faster
-                               #  on big sets: make optional
-                               parallel=True)
+                               parallel=self._parallel)
 
         # For processing one file, we're going to assume a single non-lambert
         # variable exists at the start and rename all of them
         var_names = [name for name in list(ds.data_vars.keys())
                      if not name.startswith("lambert_")]
 
         var_names = set(var_names)
```

### Comparing `icenet-0.2.3/icenet/data/processors/cmip.py` & `icenet-0.2.4/icenet/data/processors/cmip.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,14 +56,15 @@
         args.name,
         dates["train"],
         dates["val"],
         dates["test"],
         linear_trends=args.trends,
         linear_trend_days=args.trend_lead,
         north=args.hemisphere == "north",
+        parallel_opens=args.parallel_opens,
         ref_procdir=args.ref,
         south=args.hemisphere == "south",
         update_key=args.update_key,
     )
     cmip.init_source_data(
         lag_days=args.lag,
     )
```

### Comparing `icenet-0.2.3/icenet/data/processors/era5.py` & `icenet-0.2.4/icenet/data/processors/hres.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,41 +2,43 @@
 from icenet.data.process import IceNetPreProcessor
 
 """
 
 """
 
 
-class IceNetERA5PreProcessor(IceNetPreProcessor):
+class IceNetHRESPreProcessor(IceNetPreProcessor):
     """
 
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args,
                          file_filters=["latlon_"],
-                         identifier="era5",
+                         identifier="mars.hres",
                          **kwargs)
 
 
 def main():
     args = process_args()
     dates = process_date_args(args)
 
-    era5 = IceNetERA5PreProcessor(
+    hres = IceNetHRESPreProcessor(
         args.abs,
         args.anom,
         args.name,
         dates["train"],
         dates["val"],
         dates["test"],
         linear_trends=args.trends,
-        linear_trend_days=args.trend_lead,
+        linear_trend_steps=args.trend_lead,
         north=args.hemisphere == "north",
+        parallel_opens=args.parallel_opens,
         ref_procdir=args.ref,
         south=args.hemisphere == "south",
         update_key=args.update_key,
     )
-    era5.init_source_data(
+    hres.init_source_data(
         lag_days=args.lag,
     )
-    era5.process()
+    hres.process()
+
```

### Comparing `icenet-0.2.3/icenet/data/processors/hres.py` & `icenet-0.2.4/icenet/data/processors/era5.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,42 +2,42 @@
 from icenet.data.process import IceNetPreProcessor
 
 """
 
 """
 
 
-class IceNetHRESPreProcessor(IceNetPreProcessor):
+class IceNetERA5PreProcessor(IceNetPreProcessor):
     """
 
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args,
                          file_filters=["latlon_"],
-                         identifier="mars.hres",
+                         identifier="era5",
                          **kwargs)
 
 
 def main():
     args = process_args()
     dates = process_date_args(args)
 
-    hres = IceNetHRESPreProcessor(
+    era5 = IceNetERA5PreProcessor(
         args.abs,
         args.anom,
         args.name,
         dates["train"],
         dates["val"],
         dates["test"],
         linear_trends=args.trends,
-        linear_trend_steps=args.trend_lead,
+        linear_trend_days=args.trend_lead,
         north=args.hemisphere == "north",
+        parallel_opens=args.parallel_opens,
         ref_procdir=args.ref,
         south=args.hemisphere == "south",
         update_key=args.update_key,
     )
-    hres.init_source_data(
+    era5.init_source_data(
         lag_days=args.lag,
     )
-    hres.process()
-
+    era5.process()
```

### Comparing `icenet-0.2.3/icenet/data/processors/meta.py` & `icenet-0.2.4/icenet/data/processors/meta.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.3/icenet/data/processors/oras5.py` & `icenet-0.2.4/icenet/data/processors/oras5.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,14 +24,15 @@
         args.name,
         dates["train"],
         dates["val"],
         dates["test"],
         linear_trends=args.trends,
         linear_trend_days=args.trend_lead,
         north=args.hemisphere == "north",
+        parallel_opens=args.parallel_opens,
         ref_procdir=args.ref,
         south=args.hemisphere == "south",
         update_key=args.update_key,
     )
     oras5.init_source_data(
         lag_days=args.lag,
     )
```

### Comparing `icenet-0.2.3/icenet/data/processors/osi.py` & `icenet-0.2.4/icenet/data/processors/osi.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,14 +62,15 @@
         args.name,
         dates["train"],
         dates["val"],
         dates["test"],
         linear_trends=args.trends,
         linear_trend_steps=args.trend_lead,
         north=args.hemisphere == "north",
+        parallel_opens=args.parallel_opens,
         ref_procdir=args.ref,
         south=args.hemisphere == "south"
     )
     osi.init_source_data(
         lag_days=args.lag,
     )
     osi.process()
```

### Comparing `icenet-0.2.3/icenet/data/processors/utils.py` & `icenet-0.2.4/icenet/data/processors/utils.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.3/icenet/data/producers.py` & `icenet-0.2.4/icenet/data/producers.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.3/icenet/data/sic/mask.py` & `icenet-0.2.4/icenet/data/sic/mask.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.3/icenet/data/utils.py` & `icenet-0.2.4/icenet/data/utils.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.3/icenet/model/callbacks.py` & `icenet-0.2.4/icenet/model/callbacks.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.3/icenet/model/losses.py` & `icenet-0.2.4/icenet/model/losses.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.3/icenet/model/metrics.py` & `icenet-0.2.4/icenet/model/metrics.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.3/icenet/model/models.py` & `icenet-0.2.4/icenet/model/models.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.3/icenet/model/predict.py` & `icenet-0.2.4/icenet/model/predict.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 import numpy as np
 import pandas as pd
 import tensorflow as tf
 
 import icenet.model.models as models
 
+from icenet.data.loader import save_sample
 from icenet.data.dataset import IceNetDataSet
 from icenet.utils import setup_logging
 
 """
 
 """
 
@@ -22,27 +23,29 @@
     dataset_config: object,
     network_name: object,
     dataset_name: object = None,
     model_func: callable = models.unet_batchnorm,
     n_filters_factor: float = 1 / 8,
     network_folder: object = None,
     output_folder: object = None,
+    save_args: bool = False,
     seed: int = 42,
     start_dates: object = tuple([dt.datetime.now().date()]),
     test_set: bool = False,
 ) -> object:
     """
 
     :param dataset_config:
     :param network_name:
     :param dataset_name:
     :param model_func:
     :param n_filters_factor:
     :param network_folder:
     :param output_folder:
+    :param save_args:
     :param seed:
     :param start_dates:
     :param test_set:
     :return:
     """
     # TODO: going to need to be able to handle merged datasets
     ds = IceNetDataSet(dataset_config)
@@ -68,18 +71,20 @@
     )
     network.load_weights(network_path)
 
     if not test_set:
         logging.info("Generating forecast inputs from processed/ files")
 
         for date in start_dates:
-            run_prediction(network,
-                           date,
-                           output_folder,
-                           *dl.generate_sample(date, prediction=True))
+            data_sample = dl.generate_sample(date, prediction=True)
+            run_prediction(network=network,
+                           date=date,
+                           output_folder=output_folder,
+                           sample=data_sample,
+                           save_args=save_args)
     else:
         # TODO: This is horrible behaviour, rethink and refactor: we should
         #  be able to pull from the test set in a nicer and more efficient
         #  fashion
         _, _, test_inputs = ds.get_split_datasets()
 
         source_key = [k for k in dl.config['sources'].keys() if k != "meta"][0]
@@ -108,49 +113,44 @@
                 data = next(data_iter)
                 x, y, sw = data
                 batch += 1
             arr_idx = idx % ds.batch_size
             logging.info("Processing test batch {}, item {} (date {})".format(
                 batch + 1, arr_idx, test_dates[idx]))
 
-            run_prediction(network,
-                           test_dates[idx],
-                           output_folder,
-                           x[arr_idx, ...],
-                           y[arr_idx, ...],
-                           sw[arr_idx, ...])
+            run_prediction(network=network,
+                           date=test_dates[idx],
+                           output_folder=output_folder,
+                           data_sample=(x[arr_idx, ...],
+                                        y[arr_idx, ...],
+                                        sw[arr_idx, ...]),
+                           save_args=save_args)
 
 
-def run_prediction(network, date, output_folder,
-                   net_input, net_output, sample_weights):
+def run_prediction(network,
+                   date,
+                   output_folder,
+                   data_sample,
+                   save_args):
+    net_input, net_output, sample_weights = data_sample
+
     logging.info("Running prediction {}".format(date))
     pred = network(tf.convert_to_tensor([net_input]), training=False)
 
     if os.path.exists(output_folder):
         logging.warning("{} output already exists".format(output_folder))
     os.makedirs(output_folder, exist_ok=output_folder)
     output_path = os.path.join(output_folder, date.strftime("%Y_%m_%d.npy"))
 
     logging.info("Saving {} - forecast output {}".format(date, pred.shape))
     np.save(output_path, pred)
 
-    logging.debug("Saving loader generated data for reference...")
-
-    for date, output, directory in \
-            ((date, net_input, "input"),
-             (date, net_output, "outputs"),
-             (date, sample_weights, "weights")):
-        output_directory = os.path.join(output_folder, "loader", directory)
-        os.makedirs(output_directory, exist_ok=True)
-        loader_output_path = os.path.join(output_directory,
-                                          date.strftime("%Y_%m_%d.npy"))
-
-        logging.info("Saving {} - generated {} {}".
-                     format(date, directory, output.shape))
-        np.save(loader_output_path, output)
+    if save_args:
+        logging.debug("Saving loader generated data for reference...")
+        save_sample(output_path, date, data_sample)
 
     return output_path
 
 
 def date_arg(string: str) -> object:
     """
 
@@ -173,16 +173,17 @@
     ap.add_argument("output_name")
     ap.add_argument("seed", type=int, default=42)
     ap.add_argument("datefile", type=argparse.FileType("r"))
 
     ap.add_argument("-i", "--train-identifier", dest="ident",
                     help="Train dataset identifier", type=str, default=None)
     ap.add_argument("-n", "--n-filters-factor", type=float, default=1.)
-    ap.add_argument("-t", "--testset", default=False, action="store_true")
+    ap.add_argument("-t", "--testset", action="store_true", default=False)
     ap.add_argument("-v", "--verbose", action="store_true", default=False)
+    ap.add_argument("-s", "--save_args", action="store_true", default=False)
 
     return ap.parse_args()
 
 
 def main():
     args = get_args()
 
@@ -199,16 +200,15 @@
                                  "{}.{}".format(args.network_name, args.seed))
 
     predict_forecast(dataset_config,
                      args.network_name,
                      # FIXME: this is turning into a mapping mess,
                      #  do we need to retain the train SD name in the
                      #  network?
-                     dataset_name=
-                     args.ident if args.ident else args.dataset,
-                     n_filters_factor=
-                     args.n_filters_factor,
+                     dataset_name=args.ident if args.ident else args.dataset,
+                     n_filters_factor=args.n_filters_factor,
                      output_folder=output_folder,
+                     save_args=args.save_args,
                      seed=args.seed,
                      start_dates=dates,
                      test_set=args.testset)
```

### Comparing `icenet-0.2.3/icenet/model/train.py` & `icenet-0.2.4/icenet/model/train.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 import argparse
 import datetime as dt
 import json
 import logging
 import os
+import pkg_resources
 import random
 import time
 
 from pprint import pformat
 
 import numpy as np
 import pandas as pd
 import tensorflow as tf
-import wandb
 
 from tensorflow.keras.callbacks import \
     EarlyStopping, ModelCheckpoint, LearningRateScheduler
 from tensorflow.keras.models import load_model, save_model
-from wandb.keras import WandbCallback
 
 from icenet.data.dataset import IceNetDataSet, MergedIceNetDataSet
 import icenet.model.losses as losses
 import icenet.model.metrics as metrics
 from icenet.model.utils import make_exp_decay_lr_schedule
 import icenet.model.models as models
 from icenet.utils import setup_logging
 
 
 def train_model(
         run_name: object,
         dataset: object,
-        batch_size: int = 4,
+        callback_objects: list = None,
         checkpoint_monitor: str = 'val_rmse',
         checkpoint_mode: str = 'min',
         dataset_ratio: float = 1.0,
         early_stopping_patience: int = 30,
         epochs: int = 2,
         filter_size: float = 3,
         learning_rate: float = 1e-4,
@@ -49,24 +48,20 @@
         pre_load_network: bool = False,
         pre_load_path: object = None,
         seed: int = 42,
         strategy: object = tf.distribute.get_strategy(),
         training_verbosity: int = 1,
         workers: int = 5,
         use_multiprocessing: bool = True,
-        use_tensorboard: bool = True,
-        use_wandb: bool = True,
-        wandb_offline: bool = False,
-        wandb_project: str = os.environ.get("ICENET_ENVIRONMENT"),
-        wandb_user: str = os.environ.get("USER")) -> object:
+        use_tensorboard: bool = True) -> object:
     """
 
     :param run_name:
     :param dataset:
-    :param batch_size:
+    :param callback_objects:
     :param checkpoint_monitor:
     :param checkpoint_mode:
     :param dataset_ratio:
     :param early_stopping_patience:
     :param epochs:
     :param filter_size:
     :param learning_rate:
@@ -83,52 +78,18 @@
     :param pre_load_path:
     :param seed:
     :param strategy:
     :param training_verbosity:
     :param workers:
     :param use_multiprocessing:
     :param use_tensorboard:
-    :param use_wandb:
-    :param wandb_offline:
-    :param wandb_project:
-    :param wandb_user:
     :return:
     """
 
     lr_decay = -0.1 * np.log(lr_10e_decay_fac)
-    wandb.init(
-        project=wandb_project,
-        name="{}.{}".format(run_name, seed),
-        notes="{}: run at {}{}".format(run_name,
-                                       dt.datetime.now().strftime("%D %T"),
-                                       "" if
-                                       not pre_load_network else
-                                       " preload {}".format(pre_load_path)),
-        entity=wandb_user,
-        config=dict(
-            seed=seed,
-            learning_rate=learning_rate,
-            filter_size=filter_size,
-            n_filters_factor=n_filters_factor,
-            lr_10e_decay_fac=lr_10e_decay_fac,
-            lr_decay=lr_decay,
-            lr_decay_start=lr_decay_start,
-            lr_decay_end=lr_decay_end,
-            batch_size=batch_size,
-        ),
-        allow_val_change=True,
-        mode='disabled' if not use_wandb else 'offline' if wandb_offline else 'online',
-        settings=wandb.Settings(
-            start_method="fork",
-            _disable_stats=True,
-        ),
-        group=run_name,
-    )
-
-    logging.info("Hyperparameters: {}".format(pformat(wandb.config)))
 
     input_shape = (*dataset.shape, dataset.num_channels)
 
     if pre_load_network and not os.path.exists(pre_load_path):
         raise RuntimeError("{} is not available, so you cannot preload the "
                            "network with it!".format(pre_load_path))
 
@@ -184,25 +145,14 @@
 
     if use_tensorboard:
         logging.info("Adding tensorboard callback")
         log_dir = "logs/" + dt.datetime.now().strftime("%d-%m-%y-%H%M%S")
         callbacks_list.append(tf.keras.callbacks.TensorBoard(log_dir=log_dir,
                                                              histogram_freq=1))
 
-    if use_wandb:
-        # Log training metrics to wandb each epoch
-        logging.info("Adding wandb callback")
-        callbacks_list.append(
-            WandbCallback(
-                monitor=checkpoint_monitor,
-                mode=checkpoint_mode,
-                save_model=False,
-                save_graph=False,
-            ))
-
     ############################################################################
     #                              TRAINING MODEL
     ############################################################################
 
     with strategy.scope():
         loss = losses.WeightedMSE()
         metrics_list = [
@@ -236,18 +186,18 @@
     ratio = dataset_ratio if dataset_ratio else 1.0
     train_ds, val_ds, test_ds = dataset.get_split_datasets(ratio=ratio)
 
     model_history = network.fit(
         train_ds,
         epochs=epochs,
         verbose=training_verbosity,
-        callbacks=callbacks_list,
+        callbacks=callbacks_list + callback_objects,
         validation_data=val_ds,
         max_queue_size=max_queue_size,
-        # TODO: not useful for tf.data usage according to docs
+        # not useful for tf.data usage according to docs, but useful in dev
         workers=workers,
         use_multiprocessing=use_multiprocessing
     )
 
     if network_save:
         logging.info("Saving network to: {}".format(weights_path))
         network.save_weights(weights_path)
@@ -314,57 +264,54 @@
     results_path = "{}.results.json".format(model_path)
     with open(results_path, "w") as fh:
         json.dump(results, fh)
 
     logging.debug(results)
     logging.info("Done in {:.1f}s".format(time.time() - tic))
 
-    metric_vals = [[results[f'{name}{lt}']
-                    for lt in lead_times] for name in metric_names]
-    table_data = list(zip(lead_times, *metric_vals))
-    table = wandb.Table(data=table_data, columns=['leadtime', *metric_names])
-
-    # Log each metric vs. leadtime as a plot to wandb
-    for name in metric_names:
-        wandb.log(
-            {f'{name}_plot': wandb.plot.line(table, x='leadtime', y=name)})
+    return results, metric_names, lead_times
 
 
 @setup_logging
 def get_args():
     """
 
     :return:
     """
     ap = argparse.ArgumentParser()
     ap.add_argument("dataset", type=str)
     ap.add_argument("run_name", type=str)
     ap.add_argument("seed", type=int)
 
     ap.add_argument("-b", "--batch-size", type=int, default=4)
+    ap.add_argument("-ca", "--checkpoint-mode", default="min", type=str)
+    ap.add_argument("-cm", "--checkpoint-monitor", default="val_rmse", type=str)
     ap.add_argument("-ds", "--additional-dataset",
                     dest="additional", nargs="*", default=[])
     ap.add_argument("-e", "--epochs", type=int, default=4)
+    ap.add_argument("-f", "--filter-size", type=int, default=3)
     ap.add_argument("--early-stopping", type=int, default=50)
     ap.add_argument("-m", "--multiprocessing",
                     action="store_true", default=False)
     ap.add_argument("-n", "--n-filters-factor", type=float, default=1.)
-    ap.add_argument("-nw", "--no-wandb", default=False, action="store_true")
     ap.add_argument("-p", "--preload", type=str)
     ap.add_argument("-pw", "--pickup-weights",
                     action="store_true", default=False)
     ap.add_argument("-qs", "--max-queue-size", default=10, type=int)
     ap.add_argument("-r", "--ratio", default=1.0, type=float)
     ap.add_argument("-s", "--strategy", default="default",
                     choices=("default", "mirrored", "central"))
     ap.add_argument("--shuffle-train", default=False,
                     action="store_true", help="Shuffle the training set")
     ap.add_argument("--gpus", default=None)
     ap.add_argument("-v", "--verbose", action="store_true", default=False)
     ap.add_argument("-w", "--workers", type=int, default=4)
+
+    # WandB additional arguments
+    ap.add_argument("-nw", "--no-wandb", default=False, action="store_true")
     ap.add_argument("-wo", "--wandb-offline", default=False, action="store_true")
     ap.add_argument("-wp", "--wandb-project",
                     default=os.environ.get("ICENET_ENVIRONMENT"), type=str)
     ap.add_argument("-wu", "--wandb-user",
                     default=os.environ.get("USER"), type=str)
 
     ap.add_argument("--lr", default=1e-4, type=float)
@@ -410,39 +357,103 @@
 
     strategy = tf.distribute.MirroredStrategy() \
         if args.strategy == "mirrored" \
         else tf.distribute.experimental.CentralStorageStrategy() \
         if args.strategy == "central" \
         else tf.distribute.get_strategy()
 
+    # There is a better way of doing this by passing off to a dynamic factory
+    # for other integrations, but for the moment I have no shame
+    callback_objects = list()
+    using_wandb = False
+
+    if not args.no_wandb:
+        logging.warning("Initialising WANDB for this run at user request")
+
+        try:
+            import wandb
+            import wandb.keras
+        except ModuleNotFoundError:
+            logging.info("WandB is not available, we will never use it")
+        else:
+            wandb.init(
+                project=args.wandb_project,
+                name="{}.{}".format(args.run_name, args.seed),
+                notes="{}: run at {}{}".format(args.run_name,
+                                               dt.datetime.now().strftime("%D %T"),
+                                               "" if
+                                               not args.preload is not None else
+                                               " preload {}".format(args.preload)),
+                entity=args.wandb_user,
+                config=dict(
+                    seed=args.seed,
+                    learning_rate=args.lr,
+                    filter_size=args.filter_size,
+                    n_filters_factor=args.n_filters_factor,
+                    lr_10e_decay_fac=args.lr_10e_decay_fac,
+                    lr_decay_start=args.lr_decay_start,
+                    lr_decay_end=args.lr_decay_end,
+                    batch_size=args.batch_size,
+                ),
+                allow_val_change=True,
+                mode='offline' if args.wandb_offline else 'online',
+                settings=wandb.Settings(
+                    start_method="fork",
+                    _disable_stats=True,
+                ),
+                group=args.run_name,
+            )
+            using_wandb = True
+
+            # Log training metrics to wandb each epoch
+            logging.info("Adding wandb callback")
+            callback_objects.append(
+                wandb.keras.WandbCallback(
+                    monitor=args.checkpoint_monitor,
+                    mode=args.checkpoint_mode,
+                    save_model=False,
+                    save_graph=False,
+                ))
+
     weights_path, model_path = \
         train_model(args.run_name,
                     dataset,
-                    batch_size=args.batch_size,
+                    callback_objects=callback_objects,
+                    checkpoint_mode=args.checkpoint_mode,
+                    checkpoint_monitor=args.checkpoint_monitor,
                     dataset_ratio=args.ratio,
                     early_stopping_patience=args.early_stopping,
                     epochs=args.epochs,
+                    filter_size=args.filter_size,
                     learning_rate=args.lr,
                     lr_10e_decay_fac=args.lr_10e_decay_fac,
                     lr_decay_start=args.lr_decay_start,
                     lr_decay_end=args.lr_decay_end,
                     pickup_weights=args.pickup_weights,
                     pre_load_network=args.preload is not None,
                     pre_load_path=args.preload,
                     max_queue_size=args.max_queue_size,
                     n_filters_factor=args.n_filters_factor,
                     seed=args.seed,
                     strategy=strategy,
                     training_verbosity=1 if args.verbose else 2,
                     use_multiprocessing=args.multiprocessing,
-                    use_wandb=not args.no_wandb,
-                    wandb_offline=args.wandb_offline,
-                    wandb_project=args.wandb_project,
-                    wandb_user=args.wandb_user,
                     workers=args.workers)
 
-    evaluate_model(model_path,
-                   dataset,
-                   dataset_ratio=args.ratio,
-                   max_queue_size=args.max_queue_size,
-                   use_multiprocessing=args.multiprocessing,
-                   workers=args.workers)
+    results, metric_names, leads = \
+        evaluate_model(model_path,
+                       dataset,
+                       dataset_ratio=args.ratio,
+                       max_queue_size=args.max_queue_size,
+                       use_multiprocessing=args.multiprocessing,
+                       workers=args.workers)
+
+    if using_wandb:
+        metric_vals = [[results[f'{name}{lt}']
+                        for lt in leads] for name in metrics]
+        table_data = list(zip(leads, *metric_vals))
+        table = wandb.Table(data=table_data, columns=['leadtime', *metrics])
+
+        # Log each metric vs. leadtime as a plot to wandb
+        for name in metrics:
+            wandb.log(
+                {f'{name}_plot': wandb.plot.line(table, x='leadtime', y=name)})
```

### Comparing `icenet-0.2.3/icenet/model/utils.py` & `icenet-0.2.4/icenet/model/utils.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.3/icenet/plotting/data.py` & `icenet-0.2.4/icenet/process/azure.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,82 +1,85 @@
 import argparse
-import json
+import configparser
 import logging
 import os
-import subprocess
+import shutil
+import tempfile
 
-import numpy as np
-import tensorflow as tf
+import xarray as xr
 
-from icenet.data.datasets.utils import get_decoder
+from icenet.process.utils import date_arg, destination_filename
 from icenet.utils import setup_logging
 
-import matplotlib.pyplot as plt
+from azure.storage.blob import ContainerClient
+
+# https://docs.microsoft.com/en-us/azure/developer/python/sdk/storage/storage-blob-readme?view=storage-py-v12#next-steps
 
 
 @setup_logging
-def tfrecord_args():
+def upload_parse_args():
     """
 
     :return:
     """
-    ap = argparse.ArgumentParser()
-    ap.add_argument("file")
-    ap.add_argument("configuration", type=argparse.FileType("r"))
-    ap.add_argument("-i", "--index", default=1, type=int)
-    ap.add_argument("-l", "--levels", default=100, type=int)
-    ap.add_argument("-o", "--output", default="plot")
-
-    return ap.parse_args()
-
-
-def plot_tfrecord():
-    args = tfrecord_args()
-
-    ds = tf.data.TFRecordDataset([args.file])
-    config = json.load(args.configuration)
-    args.configuration.close()
-
-    decoder = get_decoder(tuple(config['shape']),
-                          config['num_channels'],
-                          config['n_forecast_days'])
-
-    ds = ds.map(decoder).batch(1)
-    it = ds.as_numpy_iterator()
-
-    for _ in range(0, args.index):
-        data = next(it)
-
-    x, y, sample_weights = data
-    logging.debug("x {}".format(x.shape))
-    logging.debug("y {}".format(y.shape))
-    logging.debug("sample_weights {}".format(sample_weights.shape))
-
-    output_dir = os.path.join(args.output, "plot_set")
-    os.makedirs(output_dir, exist_ok=True)
-    subprocess.run("rm -v {}/{}.*.png".format(
-        output_dir, config["identifier"]), shell=True)
-
-    for i, channel in enumerate(config['channels']):
-        output_path = os.path.join(output_dir, "{}.{:03d}_{}.png".
-                                   format(config["identifier"], i, channel))
-        logging.info("Producing {}".format(output_path))
-
-        fig, ax = plt.subplots()
-        ax.contourf(x[0, ..., i], levels=args.levels)
-        plt.savefig(output_path)
-        plt.close()
-
-    for i in range(config['n_forecast_days']):
-        output_path = os.path.join(output_dir, "{}.y.{:03d}.png".
-                                   format(config["identifier"], i + 1))
-        y_out = y[0, ..., i, 0]
+    a = argparse.ArgumentParser()
+
+    a.add_argument("filename")
+    a.add_argument("date", default=None, type=date_arg, nargs="?")
+
+    a.add_argument("-c", "--container", default="input", type=str)
+    a.add_argument("-l", "--leave", default=False, action="store_true")
+    a.add_argument("-o", "--overwrite", default=False, action="store_true")
+    a.add_argument("-v", "--verbose", default=False, action="store_true")
 
-        logging.info("Producing {}".format(output_path))
+    return a.parse_args()
+
+
+def upload():
+    """
 
-        if len(y_out.flatten()) == np.isnan(y_out).sum():
-            logging.warning("Skipping {} due to fully nan".format(output_path))
+    """
+    args = upload_parse_args()
+    logging.info("Azure upload facility")
+
+    url = os.getenv("AZURE_STORAGE_CONNECTION_STRING")
+
+    if not url:
+        try:
+            ini = configparser.RawConfigParser()
+            ini.read(os.path.expandvars("$HOME/.icenet.conf"))
+            url = ini.get("azure", "connection_string")
+        except configparser.Error as e:
+            logging.exception("Configuration is not correctly set up")
+            raise e
+
+    try:
+        if args.date:
+            tmpdir = tempfile.mkdtemp(dir=".")
+            ds = xr.open_dataset(args.filename)
+            ds = ds.sel(time=slice(args.date, args.date))
+
+            if len(ds.time) < 1:
+                raise ValueError("No elements in {} for {}".format(
+                    args.filename, args.date
+                ))
+
+            filename = destination_filename(tmpdir, args.filename, args.date)
+            ds.to_netcdf(filename)
+            ds.close()
         else:
-            fig, ax = plt.subplots()
-            ax.contourf(y_out, levels=args.levels)
-            plt.savefig(output_path)
-            plt.close()
+            filename = args.filename
+
+        with open(filename, "rb") as data:
+            logging.info("Uploading {}".format(filename))
+            logging.info("Connecting client")
+
+            container_client = \
+                ContainerClient.\
+                from_connection_string(url, container_name=args.container)
+            container_client.upload_blob(
+                os.path.basename(filename), data, overwrite=args.overwrite)
+    finally:
+        if args.date and not args.leave:
+            logging.info("Removing {}".format(tmpdir))
+            shutil.rmtree(tmpdir)
+
```

### Comparing `icenet-0.2.3/icenet/plotting/forecast.py` & `icenet-0.2.4/icenet/plotting/forecast.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,15 +26,17 @@
 from icenet.plotting.utils import (
     filter_ds_by_obs,
     get_forecast_ds,
     get_obs_da,
     get_seas_forecast_da,
     get_seas_forecast_init_dates,
     show_img,
-    get_plot_axes
+    get_plot_axes,
+    process_probes,
+    process_regions
 )
 from icenet.plotting.video import xarray_to_video
 
 
 def parse_location_or_region(argument: str):
     separator = ','
     # Allow ValueError to propagate if not given sequence of integers
@@ -64,57 +66,14 @@
         assert x2 > x1 and y2 > y1, "Region is not valid"
         return x1, y1, x2, y2
     except TypeError:
         raise argparse.ArgumentTypeError(
             "Region argument must be list of four integers")
 
 
-def process_regions(region: tuple,
-                    data: tuple) -> tuple:
-    """
-
-    :param region:
-    :param data:
-    
-    :return:
-    """
-
-    assert len(region) == 4, "Region needs to be a list of four integers"
-    x1, y1, x2, y2 = region
-    assert x2 > x1 and y2 > y1, "Region is not valid"
-
-    for idx, arr in enumerate(data):
-        if arr is not None:
-            data[idx] = arr[..., y1:y2, x1:x2]
-    return data
-
-
-def process_probes(probes, data) -> tuple:
-    """
-    :param probes: A sequence of locations (pairs)
-    :param data: A sequence of xr.DataArray
-    """
-
-    # index into each element of data with a xr.DataArray, for pointwise
-    # selection.  Construct the indexing DataArray as follows:
-
-    probes_da = xr.DataArray(probes, dims=('probe', 'coord'))
-    xcs, ycs = probes_da.sel(coord=0), probes_da.sel(coord=1)
-
-    for idx, arr in enumerate(data):
-        arr = arr.assign_coords({
-            "xi": ("xc", np.arange(len(arr.xc))),
-            "yi": ("yc", np.arange(len(arr.yc))),
-        })
-        if arr is not None:
-            data[idx] = arr.isel(xc=xcs, yc=ycs)
-
-    return data
-
-
 def compute_binary_accuracy(masks: object,
                             fc_da: object,
                             obs_da: object,
                             threshold: float) -> object:
     """
     Compute the binary class accuracy of a forecast,
     where we consider a binary class prediction of ice with SIC > 15%.
@@ -192,18 +151,20 @@
                                              fc_da=cmp_da,
                                              obs_da=obs_da,
                                              threshold=threshold)
         ax.plot(binacc_cmp.time, binacc_cmp.values, label="SEAS")
     else:
         binacc_cmp = None
 
+    ax.set_ylabel("Binary accuracy (%)")
     ax.xaxis.set_major_formatter(
         mdates.ConciseDateFormatter(ax.xaxis.get_major_locator()))
     ax.xaxis.set_major_locator(mdates.MonthLocator())
     ax.xaxis.set_minor_locator(mdates.DayLocator())
+    ax.set_xlabel("Date")
     ax.legend(loc='lower right')
 
     output_path = os.path.join("plot", "binacc.png") \
         if not output_path else output_path
     logging.info(f"Saving to {output_path}")
     plt.savefig(output_path)
 
@@ -212,28 +173,28 @@
 
 def compute_sea_ice_extent_error(masks: object,
                                  fc_da: object,
                                  obs_da: object,
                                  grid_area_size: int,
                                  threshold: float) -> object:
     """
-    Compute sea ice extent (SIE) error of a forecast, where SIE is
+    Compute sea ice extent (SIE) error of a forecast, where SIE error is
     defined as the total area covered by grid cells with SIC > (threshold*100)%.
 
     :param masks: an icenet Masks object
     :param fc_da: the forecasts given as an xarray.DataArray object 
                   with time, xc, yc coordinates
     :param obs_da: the "ground truth" given as an xarray.DataArray object
                    with time, xc, yc coordinates
     :param grid_area_size: the length of the sides of the grid (in km),
                            by default set to 25 (so area of grid is 25*25)
     :param threshold: the SIC threshold of interest (in percentage as a fraction),
                       i.e. threshold is between 0 and 1
 
-    :return: SIE for forecast as xarray.DataArray object
+    :return: SIE error for forecast as xarray.DataArray object
     """
     grid_area_size = 25 if grid_area_size is None else grid_area_size
     threshold = 0.15 if threshold is None else threshold
     if (threshold < 0) or (threshold > 1):
         raise ValueError("threshold must be a float between 0 and 1")
     
     # obtain mask
@@ -260,15 +221,15 @@
                               fc_da: object,
                               cmp_da: object,
                               obs_da: object,
                               output_path: object,
                               grid_area_size: int = 25,
                               threshold: float = 0.15) -> object:
     """
-    Compute and plot sea ice extent (SIE) error of a forecast, where SIE is
+    Compute and plot sea ice extent (SIE) error of a forecast, where SIE error is
     defined as the total area covered by grid cells with SIC > (threshold*100)%.
     
     :param masks: an icenet Masks object
     :param fc_da: the forecasts given as an xarray.DataArray object 
                   with time, xc, yc coordinates
     :param cmp_da: a comparison forecast / sea ice data given as an 
                    xarray.DataArray object with time, xc, yc coordinates.
@@ -277,41 +238,43 @@
                    with time, xc, yc coordinates
     :param output_path: string specifying the path to store the plot
     :param grid_area_size: the length of the sides of the grid (in km),
                            by default set to 25 (so area of grid is 25*25)
     :param threshold: the SIC threshold of interest (in percentage as a fraction),
                       i.e. threshold is between 0 and 1
     
-    :return: tuple of (SIE for forecast (fc_da), SIE for comparison (cmp_da))
+    :return: tuple of (SIE error for forecast (fc_da), SIE error for comparison (cmp_da))
     """
     forecast_sie_error = compute_sea_ice_extent_error(masks=masks,
                                                       fc_da=fc_da,
                                                       obs_da=obs_da,
                                                       grid_area_size=grid_area_size,
                                                       threshold=threshold)
     
     fig, ax = plt.subplots(figsize=(12, 6))
-    ax.set_title(f"SIE comparison ({grid_area_size} km grid resolution) "
+    ax.set_title(f"SIE error comparison ({grid_area_size} km grid resolution) "
                  f"(threshold SIC = {threshold*100}%)")
     ax.plot(forecast_sie_error.time, forecast_sie_error.values, label="IceNet")
 
     if cmp_da is not None:
         cmp_sie_error = compute_sea_ice_extent_error(masks=masks,
                                                      fc_da=cmp_da,
                                                      obs_da=obs_da,
                                                      grid_area_size=grid_area_size,
                                                      threshold=threshold)
         ax.plot(cmp_sie_error.time, cmp_sie_error.values, label="SEAS")
     else:
         cmp_sie_error = None
 
+    ax.set_ylabel("Sea ice extent error (km)")
     ax.xaxis.set_major_formatter(
         mdates.ConciseDateFormatter(ax.xaxis.get_major_locator()))
     ax.xaxis.set_major_locator(mdates.MonthLocator())
     ax.xaxis.set_minor_locator(mdates.DayLocator())
+    ax.set_xlabel("Date")
     ax.legend(loc='lower right')
 
     output_path = os.path.join("plot", "sie_error.png") \
         if not output_path else output_path
     logging.info(f"Saving to {output_path}")
     plt.savefig(output_path)
 
@@ -332,47 +295,47 @@
     :param fc_da: an xarray.DataArray object with time, xc, yc coordinates
     :param obs_da: an xarray.DataArray object with time, xc, yc coordinates
     
     :return: dictionary with keys as metric names and values as 
              xarray.DataArray's storing the computed metrics for each forecast
     """
     # check requested metrics have been implemented
-    implemented_metrics = ['MAE', 'MSE', 'RMSE']
+    implemented_metrics = ["mae", "mse", "rmse"]
     for metric in metrics:
         if metric not in implemented_metrics:
             raise NotImplementedError(f"{metric} metric has not been implemented. "
                                       f"Please only choose out of {implemented_metrics}.")
     
     # obtain mask
     mask_da = masks.get_active_cell_da(obs_da)
     
     metric_dict = {}
     # compute raw error
     err_da = (fc_da-obs_da)*100
-    if "MAE" in metrics:
+    if "mae" in metrics:
         # compute absolute SIC errors
         abs_err_da = da.fabs(err_da)
         abs_weighted_da = abs_err_da.weighted(mask_da)
-    if "MSE" in metrics or "RMSE" in metrics:
+    if "mse" in metrics or "rmse" in metrics:
         # compute squared SIC errors
         square_err_da = err_da**2
         square_weighted_da = square_err_da.weighted(mask_da)
         
     for metric in metrics:
-        if metric == "MAE":
+        if metric == "mae":
             metric_dict[metric] = abs_weighted_da.mean(dim=['yc', 'xc'])
-        elif metric == "MSE":
-            if "MSE" not in metric_dict.keys():
+        elif metric == "mse":
+            if "mse" not in metric_dict.keys():
                 # might've already been computed if RMSE came first
-                metric_dict["MSE"] = square_weighted_da.mean(dim=['yc', 'xc'])
-        elif metric == "RMSE":
-            if "MSE" not in metric_dict.keys():
+                metric_dict["mse"] = square_weighted_da.mean(dim=['yc', 'xc'])
+        elif metric == "rmse":
+            if "mse" not in metric_dict.keys():
                 # check if MSE already been computed
-                metric_dict["MSE"] = square_weighted_da.mean(dim=['yc', 'xc'])
-            metric_dict[metric] = da.sqrt(metric_dict["MSE"])
+                metric_dict["mse"] = square_weighted_da.mean(dim=['yc', 'xc'])
+            metric_dict[metric] = da.sqrt(metric_dict["mse"])
 
     # only return metrics requested (might've computed MSE when computing RMSE)
     return {k: metric_dict[k] for k in metrics}
     
     
 def plot_metrics(metrics: object,
                  masks: object,
@@ -392,15 +355,15 @@
     :param fc_da: an xarray.DataArray object with time, xc, yc coordinates
     :param cmp_da: a comparison forecast / sea ice data given as an 
                    xarray.DataArray object with time, xc, yc coordinates.
                    If None, will ignore plotting a comparison forecast
     :param obs_da: an xarray.DataArray object with time, xc, yc coordinates
     :param output_path: string specifying the path to store the plot(s).
                         If separate=True, this should be a directory
-    :param separate: logical value specifying whether there is a plot created for
+    :param separate: bool specifying whether there is a plot created for
                      each metric (True) or not (False), default is False
     
     :return: dictionary with keys as metric names and values as 
              xarray.DataArray's storing the computed metrics for each forecast
     """
     # compute metrics
     fc_metric_dict = compute_metrics(metrics=metrics,
@@ -415,15 +378,15 @@
     else:
         cmp_metric_dict = None
     
     if separate:
         # produce separate plots for each metric
         for metric in metrics:
             fig, ax = plt.subplots(figsize=(12, 6))
-            ax.set_title(f"{metric} comparison")
+            ax.set_title(f"{metric.upper()} comparison")
             ax.plot(fc_metric_dict[metric].time,
                     fc_metric_dict[metric].values,
                     label="IceNet")
             if cmp_metric_dict is not None:
                 ax.plot(cmp_metric_dict[metric].time,
                         cmp_metric_dict[metric].values,
                         label="SEAS")
@@ -441,114 +404,128 @@
     else:
         # produce one plot for all metrics
         fig, ax = plt.subplots(figsize=(12, 6))
         ax.set_title("Metric comparison")
         for metric in metrics:
             ax.plot(fc_metric_dict[metric].time,
                     fc_metric_dict[metric].values,
-                    label=f"IceNet {metric}")
+                    label=f"IceNet {metric.upper()}")
             if cmp_metric_dict is not None:
                 ax.plot(cmp_metric_dict[metric].time,
                         cmp_metric_dict[metric].values,
-                        label=f"SEAS {metric}",
+                        label=f"SEAS {metric.upper()}",
                         linestyle="dotted")
         
+        ax.set_ylabel("SIC (%)")
         ax.xaxis.set_major_formatter(
             mdates.ConciseDateFormatter(ax.xaxis.get_major_locator()))
         ax.xaxis.set_major_locator(mdates.MonthLocator())
         ax.xaxis.set_minor_locator(mdates.DayLocator())
+        ax.set_xlabel("Date")
         ax.legend(loc='lower right')
         
         output_path = os.path.join("plot", "metrics.png") \
             if not output_path else output_path
         logging.info(f"Saving to {output_path}")
         plt.savefig(output_path)
     
     return fc_metric_dict, cmp_metric_dict
 
 
-def compute_metric_as_dataframe(metric: str,
+def compute_metric_as_dataframe(metric: object,
                                 masks: object,
                                 init_date: object,
                                 fc_da: object,
                                 obs_da: object,
                                 **kwargs) -> pd.DataFrame:
     """
     Computes a metric for each leadtime in a forecast and stores the
     results in a pandas dataframe with columns 'date' (which is the
-    initialisation date passed in), 'leadtime' and the metric name.
+    initialisation date passed in), 'leadtime' and the metric name(s).
     
-    :param metric: string specifying which metric to compute
+    :param metric: string, or list of strings, specifying which metric(s) to compute
     :param masks: an icenet Masks object
     :param init_date: forecast initialisation date which gets
                       added to pandas dataframe (as string, or datetime object)
     :param fc_da: an xarray.DataArray object with time, xc, yc coordinates
     :param obs_da: an xarray.DataArray object with time, xc, yc coordinates
     :param kwargs: any keyword arguments that are required for the computation
-                   of the metric, e.g. 'threshold' for SIE and binary accuracy
-                   metrics, or 'grid_area_size' for SIE metric
+                   of the metric, e.g. 'threshold' for SIE error and binary accuracy
+                   metrics, or 'grid_area_size' for SIE error metric
     
     :return: computed metric in a pandas dataframe with columns 'date',
-             'leadtime' and 'metric'
+             'leadtime' and 'met' for each metric, met, in metric
     """
-    if metric in ["MAE", "MSE", "RMSE"]:
-        met = compute_metrics(metrics=[metric],
-                              masks=masks,
-                              fc_da=fc_da,
-                              obs_da=obs_da)[metric]
-    elif metric == "binacc":
-        if "threshold" not in kwargs.keys():
-            raise KeyError("if metric = 'binacc', must pass in argument for threshold")
-        met = compute_binary_accuracy(masks=masks,
-                                      fc_da=fc_da,
-                                      obs_da=obs_da,
-                                      threshold=kwargs["threshold"])
-    elif metric == "SIE":
-        if "grid_area_size" not in kwargs.keys():
-            raise KeyError("if metric = 'SIE', must pass in argument for grid_area_size")
-        if "threshold" not in kwargs.keys():
-            raise KeyError("if metric = 'SIE', must pass in argument for threshold")
-        met = compute_sea_ice_extent_error(masks=masks,
-                                           fc_da=fc_da,
-                                           obs_da=obs_da,
-                                           grid_area_size=kwargs["grid_area_size"],
-                                           threshold=kwargs["threshold"])
-    else:
-        raise NotImplementedError(f"{metric} is not implemented")
+    if isinstance(metric, str):
+        metric = [metric]
+    metric_dict = {}
+    for met in metric:
+        if met in ["mae", "mse", "rmse"]:
+            metric_dict[met] = compute_metrics(metrics=[met],
+                                               masks=masks,
+                                               fc_da=fc_da,
+                                               obs_da=obs_da)[met].values
+        elif met == "binacc":
+            if "threshold" not in kwargs.keys():
+                raise KeyError("if met = 'binacc', must pass in argument for threshold")
+            metric_dict[met] = compute_binary_accuracy(masks=masks,
+                                                       fc_da=fc_da,
+                                                       obs_da=obs_da,
+                                                       threshold=kwargs["threshold"]).values
+        elif met == "sie":
+            if "grid_area_size" not in kwargs.keys():
+                raise KeyError("if met = 'sie', must pass in argument for grid_area_size")
+            if "threshold" not in kwargs.keys():
+                raise KeyError("if met = 'sie', must pass in argument for threshold")
+            metric_dict[met] = compute_sea_ice_extent_error(masks=masks,
+                                                            fc_da=fc_da,
+                                                            obs_da=obs_da,
+                                                            grid_area_size=kwargs["grid_area_size"],
+                                                            threshold=kwargs["threshold"]).values
+        else:
+            raise NotImplementedError(f"{met} is not implemented")
+    
+    # create dataframe from metric_dict
+    metric_df = pd.DataFrame(metric_dict)
     
     init_date = pd.to_datetime(init_date)
     # compute day of year after first converting year to a non-leap year
     # avoids issue where 2016-03-31 is different to 2015-03-31
     if init_date.strftime("%m-%d") == "02-29":
         # if date is 29th Feb on a leap year, use dayofyear 59
         # (corresponds to 28th Feb in non-leap years)
         dayofyear = 59
     else:
         dayofyear = init_date.replace(year=2001).dayofyear
     month = init_date.month
     # get target dates
-    leadtime = list(range(1, len(met.values)+1, 1))
+    leadtime = list(range(1, len(metric_df.index)+1, 1))
     target_date = pd.Series([init_date + timedelta(days=d) for d in leadtime])
     target_dayofyear = target_date.dt.dayofyear
+    # obtain day of year using same method above to avoid any leap-year issues
+    target_dayofyear = pd.Series([59 if d.strftime("%m-%d")=="02-29"
+                                  else d.replace(year=2001).dayofyear
+                                  for d in target_date])
     target_month = target_date.dt.month
-    return pd.DataFrame({"date": init_date,
-                         "dayofyear": dayofyear,
-                         "month": month,
-                         "target_date": target_date,
-                         "target_dayofyear": target_dayofyear,
-                         "target_month": target_month,
-                         "leadtime": leadtime,
-                         f"{metric}": met.values})
+    return pd.concat([pd.DataFrame({"date": init_date,
+                                    "dayofyear": dayofyear,
+                                    "month": month,
+                                    "target_date": target_date,
+                                    "target_dayofyear": target_dayofyear,
+                                    "target_month": target_month,
+                                    "leadtime": leadtime}),
+                      metric_df],
+                      axis=1)
 
 
 def compute_metrics_leadtime_avg(metric: str,
                                  masks: object,
                                  hemisphere: str,
                                  forecast_file: str,
-                                 emcwf: bool,
+                                 ecmwf: bool,
                                  data_path: str,
                                  bias_correct: bool = False,
                                  region: tuple = None,
                                  **kwargs) -> object:
     """
     Given forecast file, for each initialisation date in the xarrray.DataArray
     we compute the metric for each leadtime and store the results
@@ -556,56 +533,56 @@
     'leadtime' and the metric name. This pandas dataframe can then be used
     to average over leadtime to obtain leadtime averaged metrics.
     
     :param metric: string specifying which metric to compute
     :param masks: an icenet Masks object
     :param hemisphere: string, typically either 'north' or 'south'
     :param forecast_file: string specifying a path to a .nc file
-    :param emcwf: logical value to indicate whether or not to compare
-                  with EMCWF SEAS forecast. If True, will only average
+    :param ecmwf: bool to indicate whether or not to compare
+                  with ECMWF SEAS forecast. If True, will only average
                   over forecasts where the initialisation dates between IceNet
                   and SEAS are the same
     :param data_path: string specifying where to save the metrics dataframe.
                       If None, dataframe is not saved
-    :param bias_correct: logical value to indicate whether or not to
+    :param bias_correct: bool to indicate whether or not to
                          perform a bias correction on SEAS forecast,
-                         by default False. Ignored if emcwf=False
+                         by default False. Ignored if ecmwf=False
     :param region: region to zoom in to
     :param kwargs: any keyword arguments that are required for the computation
-                   of the metric, e.g. 'threshold' for SIE and binary accuracy
-                   metrics, or 'grid_area_size' for SIE metric
+                   of the metric, e.g. 'threshold' for SIE error and binary accuracy
+                   metrics, or 'grid_area_size' for SIE error metric
     
     :return: pandas dataframe with columns 'date', 'leadtime' and the metric name.
     """
     # open forecast file
     fc_ds = xr.open_dataset(forecast_file)
     
-    if emcwf:
+    if ecmwf:
         # find out what dates cross over with the SEAS5 predictions
         (fc_start_date, fc_end_date) = (fc_ds.time.values.min(), fc_ds.time.values.max())
         dates = get_seas_forecast_init_dates(hemisphere)
         dates = dates[(dates > fc_start_date) & (dates <= fc_end_date)]
         times = [x for x in fc_ds.time.values if x in dates]
         fc_ds = fc_ds.sel(time=times)
     
     logging.info(f"Computing {metric} for {len(fc_ds.time.values)} forecasts")
     # obtain metric for each leadtime at each initialised date in the forecast file
     
     fc_metrics_list = []
-    if emcwf:
+    if ecmwf:
         seas_metrics_list = []
     for time in fc_ds.time.values:
         # obtain forecast
         fc = fc_ds.sel(time=slice(time, time))["sic_mean"]
         obs = get_obs_da(hemisphere=hemisphere,
                          start_date=pd.to_datetime(time) + timedelta(days=1),
                          end_date=pd.to_datetime(time) + timedelta(days=int(fc.leadtime.max())))
         fc = filter_ds_by_obs(fc, obs, time)
         
-        if emcwf:
+        if ecmwf:
             # obtain SEAS forecast
             seas = get_seas_forecast_da(hemisphere=hemisphere,
                                         date=pd.to_datetime(time),
                                         bias_correct=bias_correct)
             # remove the initialisation date from dataarray
             seas = seas.assign_coords(dict(xc=seas.xc / 1e3, yc=seas.yc / 1e3))
             seas = seas.isel(time=slice(1, None))
@@ -630,15 +607,15 @@
                                                                  fc_da=seas,
                                                                  obs_da=obs,
                                                                  **kwargs))
     
     # groupby the leadtime and compute the mean average of the metric
     fc_metric_df = pd.concat(fc_metrics_list)
     fc_metric_df["forecast_name"] = "IceNet"
-    if emcwf:
+    if ecmwf:
         seas_metric_df = pd.concat(seas_metrics_list)
         seas_metric_df["forecast_name"] = "SEAS"
         fc_metric_df = pd.concat([fc_metric_df, seas_metric_df])
     
     if data_path is not None:
         logging.info(f"Saving the metric dataframe in {data_path}")
         try:
@@ -646,79 +623,251 @@
         except OSError:
             # don't break if not successful, still return dataframe
             logging.info("Save not successful! Make sure the data_path directory exists")
         
     return fc_metric_df.reset_index(drop=True)
 
 
-def _parse_day_of_year(dayofyear, leapyear=False):
+def _parse_day_of_year(dayofyear: int, leapyear: bool = False) -> int:
+    """
+    Private function which takes in a day of year (integer or float) and returns
+    the integer day of year. Useful for ensuring consistency over leap years,
+    as dates after March could have different day of years due to leap years.
+    For example, 01/03/00 is 60th day in 2000 but 01/03/01 is the 59th day in 2001.
+    
+    :param dayofyear: integer as int or float type
+    :param leapyear: bool to indicate if we want to convert a leapyear dayofyear to
+                     non-leapyear
+    
+    :return: int dayofyear
+    """
     if leapyear:
         return (pd.Timestamp("2000-01-01") + timedelta(days=int(dayofyear) - 1)).strftime("%m-%d")
     else:
         return (pd.Timestamp("2001-01-01") + timedelta(days=int(dayofyear) - 1)).strftime("%m-%d")
 
 
+def _heatmap_ylabels(metrics_df: pd.DataFrame, average_over: str, groupby_col: str) -> object:
+    """
+    Private function to return the labels for the y-axis in heatmap plots.
+
+    :param metrics_df: pandas dataframe with columns 'date', 'leadtime' and the metric name
+    :param average_over: string to specify how to average the metrics.
+                         If average_over="all", averages over all possible
+                         forecasts and produces line plot.
+                         If average_over="month" or "day", averages
+                         over the month or day respectively and produces
+                         heat map plot.
+    :param groupby_col: string to specify how we are grouping the data.
+                        If average_over="all", this is typically "dayofyear"
+                        or "target_dayofyear".
+                        If average_over="month" or "day", this is typically
+                        "month" or "target_month".
+    
+    :return: list of labels for the y-axis
+    """
+    if average_over == "day":
+        # only add labels to the start, end dates
+        # and any days that represent the start of months
+        days_of_interest = np.array([metrics_df[groupby_col].min(),
+                                     1, 32, 60, 91, 121, 152,
+                                     182, 213, 244, 274, 305, 335,
+                                     metrics_df[groupby_col].max()])
+        labels = [_parse_day_of_year(day)
+                    if day in days_of_interest else ""
+                    for day in sorted(metrics_df[groupby_col].unique())]
+    else:
+        # find out what months have been plotted and add their names
+        month_names = np.array(["Jan", "Feb", "Mar", "Apr", "May", "Jun",
+                                "Jul", "Aug", "Sept", "Oct", "Nov", "Dec"])
+        labels = [month_names[month-1]
+                    for month in sorted(metrics_df[groupby_col].unique())]
+
+    return labels
+
+
+def standard_deviation_heatmap(metric: str,
+                               model_name: str,
+                               metrics_df: pd.DataFrame,
+                               average_over: str,
+                               target_date_avg: bool = False,
+                               output_path: str = None,
+                               fc_std_metric: pd.DataFrame = None,
+                               vmax: float = None,
+                               **kwargs) -> object:
+    """
+    Produces a heatmap plot of the leadtime standard deviation of a metric.
+
+    :param metric: string specifying which metric to compute
+    :param model_name: string specifying the name of the model or forecast
+    :param metrics_df: pandas dataframe with columns 'date', 'leadtime' and the metric name
+    :param average_over: string to specify how to average the metrics.
+                         If average_over="all", averages over all possible
+                         forecasts and produces line plot.
+                         If average_over="month" or "day", averages
+                         over the month or day respectively and produces
+                         heat map plot.
+    :param target_date_avg: bool to indiciate whether or not to average over
+                            the target date of forecast (as opposed to averaging
+                            over the initialisation date), by default False
+    :param output_path: string specifying the path to store the plot, default None
+    :param fc_std_metric: pandas dataframe of the standard deviation of the metric over leadtime.
+                          If None, this will be computed here
+    :param vmax: float specifying maximum to anchor the colourmap. If None,
+                 this is inferred from the data
+    
+    :return: dataframe of the standard deviation of the metric over leadtime
+    """
+    logging.info(f"Creating standard deviation over leadtime plot for "
+                 f"{metric} metric for {model_name} forecasts")
+    if average_over == "day":
+        groupby_col = "dayofyear"
+    else:
+        groupby_col = "month"
+    if target_date_avg:
+        groupby_col = "target_" + groupby_col
+    
+    if fc_std_metric is None:
+        # compute standard deviation of metric
+        fc_std_metric = metrics_df.groupby([groupby_col, "leadtime"]).std(numeric_only=True).\
+            reset_index().pivot(index=groupby_col, columns="leadtime", values=metric).\
+                sort_values(groupby_col, ascending=True)
+    n_forecast_days = fc_std_metric.shape[1]
+    
+    # set ylabel (if average_over == "all"), or legend label (otherwise)
+    if metric in ["mae", "mse", "rmse"]:
+        ylabel = f"SIC {metric.upper()} (%)"
+    elif metric == "binacc":
+        ylabel = f"Binary accuracy (%)"
+    elif metric == "sie":
+        ylabel = f"SIE error (km)"
+        
+    # plot heatmap of standard deviation for IceNet
+    fig, ax = plt.subplots(figsize=(12, 6))
+    sns.heatmap(data=fc_std_metric,
+                ax=ax,
+                vmin=0,
+                vmax=vmax,
+                cmap="mako_r",
+                cbar_kws=dict(label=f"Standard deviation of {ylabel}"))
+    
+    # y-axis
+    labels = _heatmap_ylabels(metrics_df=metrics_df,
+                              average_over=average_over,
+                              groupby_col=groupby_col)
+    ax.set_yticks(np.arange(len(metrics_df[groupby_col].unique()))+0.5)
+    ax.set_yticklabels(labels)
+    plt.yticks(rotation=0)
+    if target_date_avg:
+        ax.set_ylabel("Target date of forecast")
+    else:
+        ax.set_ylabel("Initialisation date of forecast")
+    
+    # x-axis
+    ax.set_xticks(np.arange(30, n_forecast_days, 30))
+    ax.set_xticklabels(np.arange(30, n_forecast_days, 30))
+    plt.xticks(rotation=0)
+    ax.set_xlabel("Lead time (days)")
+    
+    # add plot title
+    (start_date, end_date) = (metrics_df["date"].min().strftime('%d/%m/%Y'),
+                              metrics_df["date"].max().strftime('%d/%m/%Y'))
+    time_coverage = "\nStandard deviation over a minimum of " + \
+        f"{round((metrics_df[groupby_col].value_counts()/n_forecast_days).min())} " + \
+        f"forecasts between {start_date} - {end_date}"
+    if metric in ["mae", "mse", "rmse"]:
+        title = f"{metric.upper()} comparison"
+    elif metric == "binacc":
+        title = f"Binary accuracy comparison (threshold SIC = {kwargs['threshold'] * 100}%)"
+    elif metric == "sie":
+        title = f"SIE error comparison ({kwargs['grid_area_size']} km grid resolution, " +\
+            f"threshold SIC = {kwargs['threshold'] * 100}%)"
+    ax.set_title(title + f" ({model_name})" + time_coverage)
+
+    # save plot
+    targ = "target" if target_date_avg and average_over != "all" else "init"
+    filename = f"leadtime_averaged_{targ}_{average_over}_{metric}_{model_name}_std.png"
+    output_path = os.path.join("plot", filename) \
+        if not output_path else output_path
+    logging.info(f"Saving to {output_path}")
+    plt.savefig(output_path)
+    
+    return fc_std_metric
+
+
 def plot_metrics_leadtime_avg(metric: str,
                               masks: object,
                               hemisphere: str,
                               forecast_file: str,
-                              emcwf: bool,
+                              ecmwf: bool,
                               output_path: str,
                               average_over: str,
+                              plot_std: bool = False,
+                              std_mult: float = 1.0,
                               data_path: str = None,
-                              target_date_avg: bool = True,
+                              target_date_avg: bool = False,
                               bias_correct: bool = False,
                               region: tuple = None,
                               **kwargs) -> object:
     """
     Plots leadtime averaged metrics either using all the forecasts
     in the forecast file, or averaging them over by month or day.
     
     :param metric: string specifying which metric to compute
     :param masks: an icenet Masks object
     :param hemisphere: string, typically either 'north' or 'south'
     :param forecast_file: a path to a .nc file
-    :param emcwf: logical value to indicate whether or not to compare
-                  with EMCWF SEAS forecast. If True, will only average
+    :param ecmwf: bool to indicate whether or not to compare
+                  with ECMWF SEAS forecast. If True, will only average
                   over forecasts where the initialisation dates between IceNet
                   and SEAS are the same
     :param output_path: string specifying the path to store the plot
     :param average_over: string to specify how to average the metrics.
                          If average_over="all", averages over all possible
                          forecasts and produces line plot.
                          If average_over="month" or "day", averages
                          over the month or day respectively and produces
                          heat map plot.
-    :param target_date_avg:
+    :param target_date_avg: bool to indiciate whether or not to average over
+                            the target date of forecast (as opposed to averaging
+                            over the initialisation date), by default False
     :param data_path: string specifying a CSV file where metrics dataframe
                       could be loaded from. If loading in the dataframe is
                       not possible, it will compute the metrics dataframe
                       and try to save the dataframe
-    :param bias_correct: logical value to indicate whether or not to
+    :param bias_correct: bool to indicate whether or not to
                          perform a bias correction on SEAS forecast,
-                         by default False. Ignored if emcwf=False
+                         by default False. Ignored if ecmwf=False
     :param region: region to zoom in to
     :param kwargs: any keyword arguments that are required for the computation
-                   of the metric, e.g. 'threshold' for SIE and binary accuracy
-                   metrics, or 'grid_area_size' for SIE metric
+                   of the metric, e.g. 'threshold' for SIE error and binary accuracy
+                   metrics, or 'grid_area_size' for SIE error metric
     
-    :return: pandas dataframe with columns 'date', 'leadtime' and the metric name.
+    :return: pandas dataframe with columns 'date', 'leadtime' and the metric name
     """
-    implemented_metrics = ["binacc", "SIE", "MAE", "MSE", "RMSE"]
+    implemented_metrics = ["binacc", "sie", "mae", "mse", "rmse"]
     if metric not in implemented_metrics:
         raise NotImplementedError(f"{metric} metric has not been implemented. "
                                   f"Please only choose out of {implemented_metrics}.")
     if metric == "binacc":
+        # add default kwargs
         if "threshold" not in kwargs.keys():
             kwargs["threshold"] = 0.15
-    elif metric == "SIE":
+    elif metric == "sie":
+        # add default kwargs
         if "grid_area_size" not in kwargs.keys():
             kwargs["grid_area_size"] = 25
         if "threshold" not in kwargs.keys():
             kwargs["threshold"] = 0.15
+    elif metric in ["mae", "mse", "rmse"]:
+        # remove grid_area_size and threshold kwargs if passed
+        if "grid_area_size" in kwargs.keys():
+            del kwargs["grid_area_size"]
+        if "threshold" in kwargs.keys():
+            del kwargs["threshold"]
     
     do_compute_metrics = True
     if data_path is not None:
         # loading in precomputed dataframes for the metrics
         logging.info(f"Attempting to read in metrics dataframe from {data_path}")
         try:
             metric_df = pd.read_csv(data_path)
@@ -730,137 +879,197 @@
 
     if do_compute_metrics:
         # computing the dataframes for the metrics
         # will save dataframe in data_path if data_path is not None
         metric_df = compute_metrics_leadtime_avg(metric=metric,
                                                  hemisphere=hemisphere,
                                                  forecast_file=forecast_file,
-                                                 emcwf=emcwf,
+                                                 ecmwf=ecmwf,
                                                  masks=masks,
                                                  data_path=data_path,
                                                  bias_correct=bias_correct,
                                                  region=region,
                                                  **kwargs)
 
     fc_metric_df = metric_df[metric_df["forecast_name"] == "IceNet"]
     seas_metric_df = metric_df[metric_df["forecast_name"] == "SEAS"]
-    seas_metric_df = seas_metric_df if len(seas_metric_df) != 0 else None
+    seas_metric_df = seas_metric_df if (len(seas_metric_df) != 0) and ecmwf else None
 
     logging.info(f"Creating leadtime averaged plot for {metric} metric")
     fig, ax = plt.subplots(figsize=(12, 6))
     (start_date, end_date) = (fc_metric_df["date"].min().strftime('%d/%m/%Y'),
                               fc_metric_df["date"].max().strftime('%d/%m/%Y'))
     
+    # set ylabel (if average_over == "all"), or legend label (otherwise)
+    if metric in ["mae", "mse", "rmse"]:
+        ylabel = f"SIC {metric.upper()} (%)"
+    elif metric == "binacc":
+        ylabel = f"Binary accuracy (%)"
+    elif metric == "sie":
+        ylabel = f"SIE error (km)"
+    
     if average_over == "all":
         # averaging metric over leadtime for all forecasts
-        fc_avg_metric = fc_metric_df.groupby("leadtime")[metric].mean()
+        fc_avg_metric = fc_metric_df.groupby("leadtime").mean(metric).\
+            sort_values("leadtime", ascending=True)[metric]
         n_forecast_days = fc_avg_metric.index.max()
         
         # plot leadtime averaged metrics
-        ax.plot(fc_avg_metric.index, fc_avg_metric, label="IceNet")
+        ax.plot(fc_avg_metric.index, fc_avg_metric, label="IceNet", color="blue")
+        if plot_std:
+            # obtaining the standard deviation of the metric
+            fc_std_metric = fc_metric_df.groupby("leadtime")[metric].std().\
+                sort_index(ascending=True)
+            ci = std_mult * fc_std_metric
+            ax.fill_between(x=fc_avg_metric.index,
+                            y1=fc_avg_metric - ci,
+                            y2=fc_avg_metric + ci,
+                            color="blue",
+                            alpha=0.1)
         if seas_metric_df is not None:
-            seas_avg_metric = seas_metric_df.groupby("leadtime")[metric].mean()
-            ax.plot(seas_avg_metric.index, seas_avg_metric, label="SEAS")
+            seas_avg_metric = seas_metric_df.groupby("leadtime").mean(metric).\
+                sort_values("leadtime", ascending=True)[metric]
+            ax.plot(seas_avg_metric.index, seas_avg_metric, label="SEAS", color="darkorange")
+            if plot_std:
+                # obtaining the standard deviation of the metric
+                seas_std_metric = seas_metric_df.groupby("leadtime")[metric].std().\
+                    sort_index(ascending=True)
+                ci = std_mult * seas_std_metric
+                ax.fill_between(x=seas_avg_metric.index,
+                                y1=seas_avg_metric - ci,
+                                y2=seas_avg_metric + ci,
+                                color="darkorange",
+                                alpha=0.1)
 
         # string to add in plot title
-        time_coverage = f"\n Averaged over {len(fc_metric_df['date'].unique())} " + \
+        time_coverage = f"\nAveraged over {len(fc_metric_df['date'].unique())} " + \
             f"forecasts between {start_date} - {end_date}"
-        
-        ax.set_ylabel(metric)
+        if plot_std:
+            time_coverage += f"\n(with +/-{std_mult} standard deviations)"
+        ax.set_ylabel(ylabel)
         ax.legend(loc='lower right')
     elif average_over in ["day", "month"]:
         if average_over == "day":
             groupby_col = "dayofyear"
         else:
             groupby_col = "month"
         if target_date_avg:
             groupby_col = "target_" + groupby_col
         
         # compute metric by first grouping the dataframe by groupby_col and leadtime
         fc_avg_metric = fc_metric_df.groupby([groupby_col, "leadtime"]).mean(metric).\
-            reset_index().pivot(index=groupby_col, columns="leadtime", values=metric)
+            reset_index().pivot(index=groupby_col, columns="leadtime", values=metric).\
+                sort_values(groupby_col, ascending=True)
         n_forecast_days = fc_avg_metric.shape[1]
         
         if seas_metric_df is not None:
             # compute the difference in leadtime average to SEAS forecast
             seas_avg_metric = seas_metric_df.groupby([groupby_col, "leadtime"]).mean(metric).\
-                reset_index().pivot(index=groupby_col, columns="leadtime", values=metric)
+                reset_index().pivot(index=groupby_col, columns="leadtime", values=metric).\
+                    sort_values(groupby_col, ascending=True)
             heatmap_df_diff = fc_avg_metric - seas_avg_metric
             max = np.nanmax(np.abs(heatmap_df_diff.values))
             
             # plot heatmap of the difference between IceNet and SEAS
-            sns.heatmap(data=heatmap_df_diff, 
+            sns.heatmap(data=heatmap_df_diff,
                         ax=ax,
                         vmax=max,
                         vmin=-max,
-                        cmap='seismic_r',
-                        cbar_kws=dict(label=f"{metric} difference between IceNet and SEAS"))
+                        cmap="seismic_r" if metric in ["binacc", "sie"] else "seismic",
+                        cbar_kws=dict(label=f"{ylabel} difference between IceNet and SEAS"))
+
         else:
             # plot heatmap of the leadtime averaged metric when grouped by groupby_col
             sns.heatmap(data=fc_avg_metric, 
                         ax=ax,
-                        cmap='inferno',
-                        cbar_kws=dict(label=metric))
+                        cmap="inferno" if metric in ["binacc", "sie"] else "inferno_r",
+                        cbar_kws=dict(label=ylabel))
 
         # string to add in plot title
-        time_coverage = "\n Averaged over a minimum of " + \
+        time_coverage = "\nAveraged over a minimum of " + \
             f"{round((fc_metric_df[groupby_col].value_counts()/n_forecast_days).min())} " + \
             f"forecasts between {start_date} - {end_date}"
 
         # y-axis
+        labels = _heatmap_ylabels(metrics_df=fc_metric_df,
+                                  average_over=average_over,
+                                  groupby_col=groupby_col)
         ax.set_yticks(np.arange(len(fc_metric_df[groupby_col].unique()))+0.5)
-        if average_over == "day":
-            # only add labels to the start, end dates
-            # and any days that represent the start of months
-            days_of_interest = np.array([fc_metric_df[groupby_col].min(),
-                                         1, 32, 60, 91, 121, 152,
-                                         182, 213, 244, 274, 305, 335,
-                                         fc_metric_df[groupby_col].max()])
-            labels = [_parse_day_of_year(day)
-                      if day in days_of_interest else ""
-                      for day in fc_metric_df[groupby_col].unique()]
-        else:
-            # find out what months have been plotted and add their names
-            month_names = np.array(['Jan', 'Feb', 'Mar', 'Apr', 'May', 'Jun',
-                                    'Jul', 'Aug', 'Sept', 'Oct', 'Nov', 'Dec'])
-            labels = [month_names[month-1]
-                      for month in fc_metric_df[groupby_col].unique()]
         ax.set_yticklabels(labels)
+                
         plt.yticks(rotation=0)
         if target_date_avg:
             ax.set_ylabel("Target date of forecast")
         else:
             ax.set_ylabel("Initialisation date of forecast")
     else:
         raise NotImplementedError(f"averaging over {average_over} not a valid option.")
     
     # add plot title
-    if metric in ["MAE", "MSE", "RMSE"]:
-        ax.set_title(f"{metric} comparison" + time_coverage)
+    if metric in ["mae", "mse", "rmse"]:
+        title = f"{metric.upper()} comparison"
     elif metric == "binacc":
-        ax.set_title("Binary accuracy comparison (threshold SIC = "
-                     f"{kwargs['threshold'] * 100}%)" + time_coverage)
-    elif metric == "SIE":
-        ax.set_title(f"SIE comparison ({kwargs['grid_area_size']} km grid resolution, "
-                     f"threshold SIC = {kwargs['threshold'] * 100}%)" + time_coverage)
+        title = f"Binary accuracy comparison (threshold SIC = {kwargs['threshold'] * 100}%)"
+    elif metric == "sie":
+        title = f"SIE error comparison ({kwargs['grid_area_size']} km grid resolution, " +\
+            f"threshold SIC = {kwargs['threshold'] * 100}%)"
+    ax.set_title(title + time_coverage)
         
     # x-axis
     ax.set_xticks(np.arange(30, n_forecast_days, 30))
     ax.set_xticklabels(np.arange(30, n_forecast_days, 30))
     plt.xticks(rotation=0)
-    ax.set_xlabel('Lead time (days)')
+    ax.set_xlabel("Lead time (days)")
     
     # save plot
-    targ = "target" if target_date_avg else "init"
-    output_path = os.path.join("plot",
-                               f"leadtime_averaged_{targ}_{average_over}_{metric}.png") \
-        if not output_path else output_path    
+    targ = "target" if target_date_avg and average_over != "all" else "init"
+    filename = f"leadtime_averaged_{targ}_{average_over}_{metric}" + \
+        ("_comp" if seas_metric_df is not None else "") + ".png"
+    output_path = os.path.join("plot", filename) \
+        if not output_path else output_path
     logging.info(f"Saving to {output_path}")
     plt.savefig(output_path)
     
+    if plot_std and average_over in ["day", "month"]:
+        # create heapmap for the standard deviation
+        if seas_metric_df is not None:
+            # compute the standard deviation of the metric for both the forecast and SEAS5
+            fc_std_metric = fc_metric_df.groupby([groupby_col, "leadtime"]).std(numeric_only=True).\
+                reset_index().pivot(index=groupby_col, columns="leadtime", values=metric).\
+                    sort_values(groupby_col, ascending=True)
+            seas_std_metric = seas_metric_df.groupby([groupby_col, "leadtime"]).std(numeric_only=True).\
+                reset_index().pivot(index=groupby_col, columns="leadtime", values=metric).\
+                    sort_values(groupby_col, ascending=True)
+            # compute the maximum standard deviation to obtain a common scale
+            vmax = np.nanmax([np.nanmax(fc_std_metric.values), np.nanmax(seas_std_metric.values)])
+            # create heapmap for the standard deviation
+            standard_deviation_heatmap(metric=metric,
+                                       model_name="SEAS",
+                                       metrics_df=seas_metric_df,
+                                       average_over=average_over,
+                                       output_path=output_path.replace(".png", "_SEAS_std.png"),
+                                       target_date_avg=target_date_avg,
+                                       fc_std_metric=seas_std_metric,
+                                       vmax=vmax,
+                                       **kwargs)
+        else:
+            # no need to pre-compute the scale for the heatmap, hence
+            # pre-computing the standard deviation of the metric is not required
+            fc_std_metric = None
+            vmax = None
+        standard_deviation_heatmap(metric=metric,
+                                   model_name="IceNet",
+                                   metrics_df=fc_metric_df,
+                                   average_over=average_over,
+                                   output_path=output_path.replace(".png", "_IceNet_std.png"),
+                                   target_date_avg=target_date_avg,
+                                   fc_std_metric=fc_std_metric,
+                                   vmax=vmax,
+                                   **kwargs)
+
     return fc_metric_df, seas_metric_df
 
 
 def sic_error_video(fc_da: object,
                     obs_da: object,
                     land_mask: object,
                     output_path: object) -> object:
@@ -1039,19 +1248,18 @@
 
             ax.set_title(
                 f"Sea ice concentration at location {i_probe + 1}\n"
                 f"{lat:.3f}° {lat_h}, {lon:.3f}° {lon_h}"
             )
 
             ax.set_xlabel("Date")
-            ax.set_ylabel("Concentration (fraction)")
-            ax.set_ylim([0.0, 1.0])
+            ax.set_ylabel("SIC (%)")
 
             # dims: (obs_kind, time, probe)
-            ax.plot(plot_series.loc[OBS_KIND_FC, :, i_probe], label="Icenet forecast")
+            ax.plot(plot_series.loc[OBS_KIND_FC, :, i_probe], label="IceNet")
             ax.plot(plot_series.loc[OBS_KIND_OBS, :, i_probe], label="Observed")
             ax.legend()
 
             plt.setp(ax.get_xticklabels(), rotation=45, ha='right')
             output_pdf.savefig(fig, bbox_inches='tight')
 
             #### Error plot ####
@@ -1060,15 +1268,15 @@
 
             ax2.set_title(
                 f"Sea ice concentration error at location {i_probe + 1}\n"
                 f"{lat:.3f}° {lat_h}, {lon:.3f}° {lon_h}"
             )
 
             ax2.set_xlabel("Date")
-            ax2.set_ylabel("Sea ice concentration error (signed difference)")
+            ax2.set_ylabel("SIC error (%)")
 
             ax2.axhline(color='k', lw=0.5, ls='--')
             ax2.plot(plot_series.loc[OBS_KIND_ERR, :, i_probe], color='C2')
 
             plt.setp(ax2.get_xticklabels(), rotation=45, ha='right')
             output_pdf.savefig(fig2, bbox_inches='tight')
 
@@ -1081,17 +1289,20 @@
                           as_command: bool = False):
 
     """
     :param fc_da: a DataArray with dims ('time', 'probe')
     :param obs_da: a DataArray with dims ('time', 'probe')
     """
 
-    error_da = fc_da - obs_da
+    # convert SIC to percentages (ranging from 0% to 100%) rather than a fraction
+    fc_da = fc_da*100
+    obs_da = obs_da*100
+    err_da = (fc_da-obs_da)
     combined_da = xr.concat(
-        [fc_da, obs_da, error_da],
+        [fc_da, obs_da, err_da],
         dim="obs_kind", coords="minimal"
     )
 
     # convert to a dataframe for csv output
     df = (
         combined_da
         .to_dataframe(name="SIC")
@@ -1182,15 +1393,15 @@
         return self
 
     def allow_metrics(self):
         self.add_argument("-m", 
                           "--metrics",
                           help="Which metrics to compute and plot",
                           type=str,
-                          default="MAE,MSE,RMSE")
+                          default="mae,mse,rmse")
         self.add_argument("-s",
                           "--separate",
                           help="Whether or not to produce separate plots for each metric",
                           action="store_true",
                           default=False)
         return self
 
@@ -1250,26 +1461,26 @@
             seas = seas.isel(time=slice(1, None))
     else:
         seas = None
 
     if args.region:
         seas, fc, obs, masks = process_regions(args.region,
                                                [seas, fc, obs, masks])
-
+    
     plot_binary_accuracy(masks=masks,
                          fc_da=fc,
                          cmp_da=seas,
                          obs_da=obs,
                          output_path=args.output_path,
                          threshold=args.threshold)
 
 
 def sie_error():
     """
-    Produces plot of the sea-ice extent (SIE) error of forecasts.
+    Produces plot of the sea ice extent (SIE) error of forecasts.
     """
     ap = (
         ForecastPlotArgParser()
         .allow_ecmwf()
         .allow_threshold()
         .allow_sie()
     )
@@ -1329,44 +1540,50 @@
     ap.add_argument("-c", "--no-coastlines",
                     help="Turn off cartopy integration",
                     action="store_true", default=False)
     ap.add_argument("-f", "--format",
                     help="Format to output in",
                     choices=("mp4", "png", "svg", "tiff"),
                     default="png")
+    ap.add_argument("-n", "--cmap-name",
+                    help="Color map name if not wanting to use default",
+                    default=None)
     ap.add_argument("-s", "--stddev",
                     help="Plot the standard deviation from the ensemble",
                     action="store_true",
                     default=False)
     args = ap.parse_args()
 
     fc = get_forecast_ds(args.forecast_file,
                          args.forecast_date,
                          stddev=args.stddev)
     fc = fc.transpose(..., "yc", "xc")
 
-    if not os.path.isdir(args.output_path):
-        logging.warning("No directory at: {}".format(args.output_path))
-        os.makedirs(args.output_path)
-    elif os.path.isfile(args.output_path):
+    output_path = "." if args.output_path is None else args.output_path
+
+    if not os.path.isdir(output_path):
+        logging.warning("No directory at: {}".format(output_path))
+        os.makedirs(output_path)
+    elif os.path.isfile(output_path):
         raise RuntimeError("{} should be a directory and not existent...".
-                           format(args.output_path))
+                           format(output_path))
 
     forecast_name = "{}.{}".format(
         os.path.splitext(os.path.basename(args.forecast_file))[0],
         args.forecast_date)
 
-    cmap = cm.get_cmap("BuPu_r")
+    cmap_name = "BuPu_r" if args.stddev else "Blues_r"
+    if args.cmap_name is not None:
+        cmap_name = args.cmap_name
+
+    logging.info("Using cmap {}".format(cmap_name))
+    cmap = cm.get_cmap(cmap_name)
     cmap.set_bad("dimgrey")
 
     if args.region is not None:
-        if not args.stddev:
-            cmap = cm.get_cmap("tab20")
-            cmap.set_bad("dimgrey")
-
         fc = process_regions(args.region, [fc])[0]
 
     vmax = 1.
 
     if args.stddev:
         vmax = float(fc.max())
         logging.info("Calculated vmax to be: {}".format(vmax))
@@ -1391,29 +1608,30 @@
         anim_args = dict(
             figsize=5
         )
         if not args.no_coastlines:
             logging.warning("Coastlines will not work with the current "
                             "implementation of xarray_to_video")
 
-        output_filename = os.path.join(args.output_path, "{}.{}.{}{}".format(
+        output_filename = os.path.join(output_path, "{}.{}.{}{}".format(
             forecast_name,
             args.forecast_date.strftime("%Y%m%d"),
             "" if not args.stddev else "stddev.",
             args.format
         ))
         xarray_to_video(pred_da, fps=1, cmap=cmap,
                         imshow_kwargs=dict(vmin=0., vmax=vmax)
                         if not args.stddev else None,
                         video_path=output_filename,
                         **anim_args)
     else:
         for leadtime in leadtimes:
             pred_da = fc.sel(leadtime=leadtime).isel(time=0)
-            bound_args = dict()
+            bound_args = dict(north=args.hemisphere == "north",
+                              south=args.hemisphere == "south")
 
             if args.region is not None:
                 bound_args.update(x1=args.region[0],
                                   x2=args.region[2],
                                   y1=args.region[1],
                                   y2=args.region[3])
 
@@ -1426,15 +1644,15 @@
                           do_coastlines=not args.no_coastlines)
 
             plt.colorbar(im, ax=ax)
             plot_date = args.forecast_date + dt.timedelta(leadtime)
             ax.set_title("{:04d}/{:02d}/{:02d}".format(plot_date.year,
                                                        plot_date.month,
                                                        plot_date.day))
-            output_filename = os.path.join(args.output_path, "{}.{}.{}{}".format(
+            output_filename = os.path.join(output_path, "{}.{}.{}{}".format(
                 forecast_name,
                 (args.forecast_date + dt.timedelta(
                     days=leadtime)).strftime("%Y%m%d"),
                 "" if not args.stddev else "stddev.",
                 args.format
             ))
 
@@ -1510,14 +1728,16 @@
 def leadtime_avg_plots():
     """
     Produces plot of leadtime averaged metrics for forecasts.
     """
     ap = (
         ForecastPlotArgParser(forecast_date=False)
         .allow_ecmwf()
+        .allow_threshold()
+        .allow_sie()
     )
     ap.add_argument("-m",
                     "--metric",
                     help="Which metric to compute and plot",
                     type=str)
     ap.add_argument("-dp",
                     "--data_path",
@@ -1525,34 +1745,48 @@
                     type=str,
                     default=None)
     ap.add_argument("-ao",
                     "--average_over",
                     help="How to average the forecast metrics",
                     type=str,
                     choices=["all", "month", "day"])
+    ap.add_argument("-s",
+                    "--std",
+                    help="If flagged, standard deviation is plotted",
+                    action="store_true",
+                    default=False)
+    ap.add_argument("-sm",
+                    "--std_mult",
+                    help="What multiple of the standard deviation to plot",
+                    type=float,
+                    default=1.0)
     ap.add_argument("-td",
                     "--target_date_average",
                     help="Averages metric over target date instead of init date",
                     action="store_true",
                     default=False)
     args = ap.parse_args()
     masks = Masks(north=args.hemisphere == "north",
                   south=args.hemisphere == "south")
     
     plot_metrics_leadtime_avg(metric=args.metric,
                               masks=masks,
                               hemisphere=args.hemisphere,
                               forecast_file=args.forecast_file,
-                              emcwf=args.ecmwf,
+                              ecmwf=args.ecmwf,
                               output_path=args.output_path,
                               average_over=args.average_over,
+                              plot_std=args.std,
+                              std_mult=args.std_mult,
                               data_path=args.data_path,
                               target_date_avg=args.target_date_average,
                               bias_correct=args.bias_correct,
-                              region=args.region)
+                              region=args.region,
+                              threshold=args.threshold,
+                              grid_area_size=args.grid_area)
 
 
 def sic_error():
     """
     Produces video visualisation of SIC of forecast and ground truth.
     """
     ap = ForecastPlotArgParser()
```

### Comparing `icenet-0.2.3/icenet/plotting/utils.py` & `icenet-0.2.4/icenet/plotting/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -307,117 +307,155 @@
     logging.info("Got files: {}".format(obs_dfs))
     obs_ds = xr.open_mfdataset(obs_dfs)
     obs_ds = obs_ds.sel(time=slice(start_date, end_date))
 
     return obs_ds.ice_conc
 
 
-def calculate_data_extents(x1: int,
-                           x2: int,
-                           y1: int,
-                           y2: int):
+def calculate_extents(x1: int,
+                      x2: int,
+                      y1: int,
+                      y2: int):
     """
 
     :param x1:
     :param x2:
     :param y1:
     :param y2:
     :return:
     """
-    data_extent_estimate = 5400000.0    # 216 * 25000
+    data_extent_base = 5387500
 
-    return [-(data_extent_estimate) + (x1 * 25000),
-            data_extent_estimate - ((432 - x2) * 25000),
-            -(data_extent_estimate) + ((432 - y2) * 25000),
-            data_extent_estimate - (y1 * 25000)]
+    extents = [
+        -data_extent_base + (x1 * 25000),
+        data_extent_base - ((432 - x2) * 25000),
+        -data_extent_base + (y1 * 25000),
+        data_extent_base - ((432 - y2) * 25000),
+    ]
 
-
-def calculate_proj_extents(x1: int,
-                           x2: int,
-                           y1: int,
-                           y2: int):
-    """
-
-    :param x1:
-    :param x2:
-    :param y1:
-    :param y2:
-    :return:
-    """
-    data_extent_estimate = 5400000.0    # 216 * 25000
-
-    return [-(data_extent_estimate) + (y1 * 25000),
-            data_extent_estimate - ((432 - y2) * 25000),
-            -(data_extent_estimate) + (x1 * 25000),
-            data_extent_estimate - ((432 - x2) * 25000)]
+    logging.debug("Data extents: {}".format(extents))
+    return extents
 
 
 def get_plot_axes(x1: int = 0,
                   x2: int = 432,
                   y1: int = 0,
                   y2: int = 432,
-                  do_coastlines: bool = True):
+                  do_coastlines: bool = True,
+                  north: bool = True,
+                  south: bool = False):
     """
 
     :param x1:
     :param x2:
     :param y1:
     :param y2:
     :param do_coastlines:
+    :param north:
+    :param south:
     :return:
     """
+    assert north ^ south, "One hemisphere only must be selected"
+
     fig = plt.figure(figsize=(10, 8), dpi=150, layout='tight')
 
     if do_coastlines:
-        proj = ccrs.LambertAzimuthalEqualArea(-90, 90)
+        pole = 1 if north else -1
+        proj = ccrs.LambertAzimuthalEqualArea(0, pole * 90)
         ax = fig.add_subplot(1, 1, 1, projection=proj)
-        bounds = calculate_proj_extents(x1, x2, y1, y2)
-        ax.set_extent(bounds, crs=proj)
+        extents = calculate_extents(x1, x2, y1, y2)
+        ax.set_extent(extents, crs=proj)
     else:
         ax = fig.add_subplot(1, 1, 1)
 
     return ax
 
 
 def show_img(ax,
              arr,
              x1: int = 0,
              x2: int = 432,
              y1: int = 0,
              y2: int = 432,
              cmap: object = None,
              do_coastlines: bool = True,
-             vmin = 0.,
-             vmax = 1.):
+             vmin: float = 0.,
+             vmax: float = 1.,
+             north: bool = True,
+             south: bool = False):
     """
 
     :param ax:
     :param arr:
     :param x1:
     :param x2:
     :param y1:
     :param y2:
     :param cmap:
     :param do_coastlines:
     :param vmin:
     :param vmax:
+    :param north:
+    :param south:
     :return:
     """
 
-    if do_coastlines:
-        data_globe = ccrs.Globe(datum="WGS84",
-                                inverse_flattening=298.257223563,
-                                semimajor_axis=6378137.0)
-        data_crs = ccrs.LambertAzimuthalEqualArea(0, 90, globe=data_globe)
+    assert north ^ south, "One hemisphere only must be selected"
 
+    if do_coastlines:
+        pole = 1 if north else -1
+        data_crs = ccrs.LambertAzimuthalEqualArea(0, pole * 90)
+        extents = calculate_extents(x1, x2, y1, y2)
         im = ax.imshow(arr,
                        vmin=vmin,
                        vmax=vmax,
                        cmap=cmap,
                        transform=data_crs,
-                       extent=calculate_data_extents(x1, x2, y1, y2))
+                       extent=extents)
         ax.coastlines()
     else:
         im = ax.imshow(arr, cmap=cmap, vmin=vmin, vmax=vmax)
 
     return im
 
+
+def process_probes(probes, data) -> tuple:
+    """
+    :param probes: A sequence of locations (pairs)
+    :param data: A sequence of xr.DataArray
+    """
+
+    # index into each element of data with a xr.DataArray, for pointwise
+    # selection.  Construct the indexing DataArray as follows:
+
+    probes_da = xr.DataArray(probes, dims=('probe', 'coord'))
+    xcs, ycs = probes_da.sel(coord=0), probes_da.sel(coord=1)
+
+    for idx, arr in enumerate(data):
+        arr = arr.assign_coords({
+            "xi": ("xc", np.arange(len(arr.xc))),
+            "yi": ("yc", np.arange(len(arr.yc))),
+        })
+        if arr is not None:
+            data[idx] = arr.isel(xc=xcs, yc=ycs)
+
+    return data
+
+
+def process_regions(region: tuple,
+                    data: tuple) -> tuple:
+    """
+
+    :param region:
+    :param data:
+
+    :return:
+    """
+
+    assert len(region) == 4, "Region needs to be a list of four integers"
+    x1, y1, x2, y2 = region
+    assert x2 > x1 and y2 > y1, "Region is not valid"
+
+    for idx, arr in enumerate(data):
+        if arr is not None:
+            data[idx] = arr[..., (432 - y2):(432 - y1), x1:x2]
+    return data
```

### Comparing `icenet-0.2.3/icenet/plotting/video.py` & `icenet-0.2.4/icenet/plotting/video.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.3/icenet/process/forecasts.py` & `icenet-0.2.4/icenet/process/forecasts.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.3/icenet/process/local.py` & `icenet-0.2.4/icenet/process/local.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.3/icenet/process/predict.py` & `icenet-0.2.4/icenet/process/predict.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.3/icenet/process/utils.py` & `icenet-0.2.4/icenet/process/utils.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.3/icenet/results/threshold.py` & `icenet-0.2.4/icenet/results/threshold.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.3/icenet/tests/test_entry_points.py` & `icenet-0.2.4/icenet/tests/test_entry_points.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.3/icenet/tests/test_mod.py` & `icenet-0.2.4/icenet/tests/test_mod.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.3/icenet/utils.py` & `icenet-0.2.4/icenet/utils.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.3/icenet.egg-info/SOURCES.txt` & `icenet-0.2.4/icenet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `icenet-0.2.3/icenet.egg-info/entry_points.txt` & `icenet-0.2.4/icenet.egg-info/entry_points.txt`

 * *Files 6% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 icenet_data_masks = icenet.data.sic.mask:main
 icenet_data_oras5 = icenet.data.interfaces.cmems:main
 icenet_data_reproc_monthly = icenet.data.interfaces.utils:reprocess_main
 icenet_data_seas = icenet.data.interfaces.mars:seas_main
 icenet_data_sic = icenet.data.sic.osisaf:main
 icenet_dataset_check = icenet.data.dataset:check_dataset
 icenet_dataset_create = icenet.data.loader:create
-icenet_loader_sample = icenet.data.loader:get_sample
 icenet_output = icenet.process.predict:create_cf_output
 icenet_output_broadcast = icenet.process.forecasts:broadcast_main
 icenet_output_geotiff = icenet.process.forecasts:create_geotiff_output
 icenet_output_reproject = icenet.process.forecasts:reproject_main
 icenet_plot_bin_accuracy = icenet.plotting.forecast:binary_accuracy
 icenet_plot_forecast = icenet.plotting.forecast:plot_forecast
+icenet_plot_input = icenet.plotting.data:plot_sample_cli
 icenet_plot_leadtime_avg = icenet.plotting.forecast:leadtime_avg_plots
 icenet_plot_metrics = icenet.plotting.forecast:metric_plots
 icenet_plot_record = icenet.plotting.data:plot_tfrecord
 icenet_plot_sic_error = icenet.plotting.forecast:sic_error
 icenet_plot_sic_error_local = icenet.plotting.forecast:sic_error_local
 icenet_plot_sie_error = icenet.plotting.forecast:sie_error
 icenet_predict = icenet.model.predict:main
```

### Comparing `icenet-0.2.3/setup.py` & `icenet-0.2.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,24 +62,24 @@
             "icenet_process_metadata = icenet.data.processors.meta:main",
 
             "icenet_process_condense = "
             "icenet.data.processors.utils:condense_main",
 
             "icenet_dataset_check = icenet.data.dataset:check_dataset",
             "icenet_dataset_create = icenet.data.loader:create",
-            "icenet_loader_sample = icenet.data.loader:get_sample",
 
             "icenet_train = icenet.model.train:main",
             "icenet_predict = icenet.model.predict:main",
             "icenet_upload_azure = icenet.process.azure:upload",
             "icenet_upload_local = icenet.process.local:upload",
 
             "icenet_plot_record = icenet.plotting.data:plot_tfrecord",
 
             "icenet_plot_forecast = icenet.plotting.forecast:plot_forecast",
+            "icenet_plot_input = icenet.plotting.data:plot_sample_cli",
             "icenet_plot_sic_error = icenet.plotting.forecast:sic_error",
             "icenet_plot_sic_error_local = icenet.plotting.forecast:sic_error_local",
             "icenet_plot_bin_accuracy = "
             "icenet.plotting.forecast:binary_accuracy",
             "icenet_plot_sie_error = icenet.plotting.forecast:sie_error",
             "icenet_plot_metrics = icenet.plotting.forecast:metric_plots",
             "icenet_plot_leadtime_avg = icenet.plotting.forecast:leadtime_avg_plots",
```

