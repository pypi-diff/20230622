# Comparing `tmp/cellfinder-core-0.4.0.tar.gz` & `tmp/cellfinder-core-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellfinder-core-0.4.0.tar", last modified: Wed May 17 09:39:26 2023, max compression
+gzip compressed data, was "cellfinder-core-0.4.1.tar", last modified: Thu Jun 22 14:26:27 2023, max compression
```

## Comparing `cellfinder-core-0.4.0.tar` & `cellfinder-core-0.4.1.tar`

### file list

```diff
@@ -1,107 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:26.741206 cellfinder-core-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/.codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:26.721206 cellfinder-core-0.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:26.729206 cellfinder-core-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/.github/workflows/test_numba_off.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12671 2023-05-17 09:39:26.741206 cellfinder-core-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11634 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:26.729206 cellfinder-core-0.4.0/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/benchmarks/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/benchmarks/detect_and_classify.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/benchmarks/filter_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/benchmarks/filter_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/cell_detection.md
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 09:39:26.741206 cellfinder-core-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:26.721206 cellfinder-core-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:26.729206 cellfinder-core-0.4.0/src/cellfinder_core/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:26.733206 cellfinder-core-0.4.0/src/cellfinder_core/classify/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/classify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/classify/augment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/classify/classify.py
--rw-r--r--   0 runner    (1001) docker     (123)    15384 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/classify/cube_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9862 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/classify/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/classify/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:26.733206 cellfinder-core-0.4.0/src/cellfinder_core/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/config/cellfinder.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:26.737206 cellfinder-core-0.4.0/src/cellfinder_core/detect/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/detect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/detect/detect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:26.737206 cellfinder-core-0.4.0/src/cellfinder_core/detect/filters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/detect/filters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:26.737206 cellfinder-core-0.4.0/src/cellfinder_core/detect/filters/plane/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/detect/filters/plane/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/detect/filters/plane/classical_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/detect/filters/plane/plane_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/detect/filters/plane/tile_walker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/detect/filters/setup_filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:26.737206 cellfinder-core-0.4.0/src/cellfinder_core/detect/filters/volume/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/detect/filters/volume/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11173 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/detect/filters/volume/ball_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9152 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/detect/filters/volume/structure_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/detect/filters/volume/structure_splitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6693 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/detect/filters/volume/volume_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:26.741206 cellfinder-core-0.4.0/src/cellfinder_core/download/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/download/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/download/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/download/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:26.741206 cellfinder-core-0.4.0/src/cellfinder_core/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/tools/IO.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/tools/array_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/tools/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/tools/image_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/tools/prep.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/tools/source_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/tools/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/tools/tf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/tools/tiff.py
--rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/tools/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:26.741206 cellfinder-core-0.4.0/src/cellfinder_core/train/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/train/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13029 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/train/train_yml.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/src/cellfinder_core/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:26.733206 cellfinder-core-0.4.0/src/cellfinder_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12671 2023-05-17 09:39:24.000000 cellfinder-core-0.4.0/src/cellfinder_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-05-17 09:39:26.000000 cellfinder-core-0.4.0/src/cellfinder_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 09:39:24.000000 cellfinder-core-0.4.0/src/cellfinder_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-17 09:39:24.000000 cellfinder-core-0.4.0/src/cellfinder_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-17 09:39:24.000000 cellfinder-core-0.4.0/src/cellfinder_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-17 09:39:24.000000 cellfinder-core-0.4.0/src/cellfinder_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:26.741206 cellfinder-core-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:10.000000 cellfinder-core-0.4.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:26.741206 cellfinder-core-0.4.0/tests/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:12.000000 cellfinder-core-0.4.0/tests/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-17 09:39:12.000000 cellfinder-core-0.4.0/tests/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:26.741206 cellfinder-core-0.4.0/tests/tests/test_integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:12.000000 cellfinder-core-0.4.0/tests/tests/test_integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-05-17 09:39:12.000000 cellfinder-core-0.4.0/tests/tests/test_integration/test_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-17 09:39:12.000000 cellfinder-core-0.4.0/tests/tests/test_integration/test_detection_structure_splitting.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-17 09:39:12.000000 cellfinder-core-0.4.0/tests/tests/test_integration/test_train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:26.741206 cellfinder-core-0.4.0/tests/tests/test_unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:12.000000 cellfinder-core-0.4.0/tests/tests/test_unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:26.741206 cellfinder-core-0.4.0/tests/tests/test_unit/test_detect/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:12.000000 cellfinder-core-0.4.0/tests/tests/test_unit/test_detect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-17 09:39:12.000000 cellfinder-core-0.4.0/tests/tests/test_unit/test_detect/test_detect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:26.725206 cellfinder-core-0.4.0/tests/tests/test_unit/test_detect/test_filters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:26.741206 cellfinder-core-0.4.0/tests/tests/test_unit/test_detect/test_filters/test_volume_filters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:12.000000 cellfinder-core-0.4.0/tests/tests/test_unit/test_detect/test_filters/test_volume_filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-05-17 09:39:12.000000 cellfinder-core-0.4.0/tests/tests/test_unit/test_detect/test_filters/test_volume_filters/test_structure_detection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:26.741206 cellfinder-core-0.4.0/tests/tests/test_unit/test_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:39:12.000000 cellfinder-core-0.4.0/tests/tests/test_unit/test_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-17 09:39:12.000000 cellfinder-core-0.4.0/tests/tests/test_unit/test_tools/test_IO.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-17 09:39:12.000000 cellfinder-core-0.4.0/tests/tests/test_unit/test_tools/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-17 09:39:12.000000 cellfinder-core-0.4.0/tests/tests/test_unit/test_tools/test_image_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-05-17 09:39:12.000000 cellfinder-core-0.4.0/tests/tests/test_unit/test_tools/test_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-17 09:39:12.000000 cellfinder-core-0.4.0/tests/tests/test_unit/test_tools/test_tools_general.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-17 09:39:12.000000 cellfinder-core-0.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:27.443091 cellfinder-core-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/.codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:27.415090 cellfinder-core-0.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:27.423091 cellfinder-core-0.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/.github/workflows/test_numba_off.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12358 2023-06-22 14:26:27.443091 cellfinder-core-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11321 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:27.427091 cellfinder-core-0.4.1/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/benchmarks/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/benchmarks/detect_and_classify.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/benchmarks/filter_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/benchmarks/filter_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 14:26:27.443091 cellfinder-core-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:27.415090 cellfinder-core-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:27.427091 cellfinder-core-0.4.1/src/cellfinder_core/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:27.431091 cellfinder-core-0.4.1/src/cellfinder_core/classify/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/classify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/classify/augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/classify/classify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15384 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/classify/cube_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9862 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/classify/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/classify/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:27.431091 cellfinder-core-0.4.1/src/cellfinder_core/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/config/cellfinder.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:27.431091 cellfinder-core-0.4.1/src/cellfinder_core/detect/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/detect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/detect/detect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:27.431091 cellfinder-core-0.4.1/src/cellfinder_core/detect/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/detect/filters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:27.435091 cellfinder-core-0.4.1/src/cellfinder_core/detect/filters/plane/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/detect/filters/plane/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/detect/filters/plane/classical_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/detect/filters/plane/plane_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/detect/filters/plane/tile_walker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/detect/filters/setup_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:27.435091 cellfinder-core-0.4.1/src/cellfinder_core/detect/filters/volume/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/detect/filters/volume/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11173 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/detect/filters/volume/ball_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9152 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/detect/filters/volume/structure_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/detect/filters/volume/structure_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6693 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/detect/filters/volume/volume_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:27.439091 cellfinder-core-0.4.1/src/cellfinder_core/download/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/download/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/download/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/download/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:27.443091 cellfinder-core-0.4.1/src/cellfinder_core/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/tools/IO.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/tools/array_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/tools/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/tools/image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/tools/prep.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/tools/source_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/tools/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/tools/tf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/tools/tiff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/tools/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:27.443091 cellfinder-core-0.4.1/src/cellfinder_core/train/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13029 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/train/train_yml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/src/cellfinder_core/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:27.427091 cellfinder-core-0.4.1/src/cellfinder_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12358 2023-06-22 14:26:25.000000 cellfinder-core-0.4.1/src/cellfinder_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-06-22 14:26:27.000000 cellfinder-core-0.4.1/src/cellfinder_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 14:26:25.000000 cellfinder-core-0.4.1/src/cellfinder_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-22 14:26:25.000000 cellfinder-core-0.4.1/src/cellfinder_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-22 14:26:25.000000 cellfinder-core-0.4.1/src/cellfinder_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-22 14:26:25.000000 cellfinder-core-0.4.1/src/cellfinder_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:27.443091 cellfinder-core-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:11.000000 cellfinder-core-0.4.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:27.443091 cellfinder-core-0.4.1/tests/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:13.000000 cellfinder-core-0.4.1/tests/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-06-22 14:26:13.000000 cellfinder-core-0.4.1/tests/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:27.443091 cellfinder-core-0.4.1/tests/tests/test_integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:13.000000 cellfinder-core-0.4.1/tests/tests/test_integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-06-22 14:26:13.000000 cellfinder-core-0.4.1/tests/tests/test_integration/test_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-22 14:26:13.000000 cellfinder-core-0.4.1/tests/tests/test_integration/test_detection_structure_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-22 14:26:13.000000 cellfinder-core-0.4.1/tests/tests/test_integration/test_train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:27.443091 cellfinder-core-0.4.1/tests/tests/test_unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:13.000000 cellfinder-core-0.4.1/tests/tests/test_unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:27.443091 cellfinder-core-0.4.1/tests/tests/test_unit/test_detect/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:13.000000 cellfinder-core-0.4.1/tests/tests/test_unit/test_detect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-22 14:26:13.000000 cellfinder-core-0.4.1/tests/tests/test_unit/test_detect/test_detect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:27.419091 cellfinder-core-0.4.1/tests/tests/test_unit/test_detect/test_filters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:27.443091 cellfinder-core-0.4.1/tests/tests/test_unit/test_detect/test_filters/test_volume_filters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:13.000000 cellfinder-core-0.4.1/tests/tests/test_unit/test_detect/test_filters/test_volume_filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-06-22 14:26:13.000000 cellfinder-core-0.4.1/tests/tests/test_unit/test_detect/test_filters/test_volume_filters/test_structure_detection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:27.443091 cellfinder-core-0.4.1/tests/tests/test_unit/test_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 14:26:13.000000 cellfinder-core-0.4.1/tests/tests/test_unit/test_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-22 14:26:13.000000 cellfinder-core-0.4.1/tests/tests/test_unit/test_tools/test_IO.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-22 14:26:13.000000 cellfinder-core-0.4.1/tests/tests/test_unit/test_tools/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-22 14:26:13.000000 cellfinder-core-0.4.1/tests/tests/test_unit/test_tools/test_image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-06-22 14:26:13.000000 cellfinder-core-0.4.1/tests/tests/test_unit/test_tools/test_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-22 14:26:13.000000 cellfinder-core-0.4.1/tests/tests/test_unit/test_tools/test_tools_general.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-22 14:26:13.000000 cellfinder-core-0.4.1/tox.ini
```

### Comparing `cellfinder-core-0.4.0/.codecov.yml` & `cellfinder-core-0.4.1/.codecov.yml`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.0/.github/workflows/test_and_deploy.yml` & `cellfinder-core-0.4.1/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.0/.github/workflows/test_numba_off.yml` & `cellfinder-core-0.4.1/.github/workflows/test_numba_off.yml`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.0/.gitignore` & `cellfinder-core-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.0/CHANGELOG.md` & `cellfinder-core-0.4.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.0/LICENSE` & `cellfinder-core-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.0/PKG-INFO` & `cellfinder-core-0.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellfinder-core
-Version: 0.4.0
+Version: 0.4.1
 Summary: Automated 3D cell detection in large microscopy images
 Author-email: "Adam Tyson, Christian Niedworok, Charly Rousseau" <code@adamltyson.com>
 Project-URL: Homepage, https://brainglobe.info/cellfinder
 Project-URL: Source Code, https://github.com/brainglobe/cellfinder-core
 Project-URL: Bug Tracker, https://github.com/brainglobe/cellfinder-core/issues
 Project-URL: Documentation, https://docs.brainglobe.info/cellfinder
 Classifier: Development Status :: 3 - Alpha
@@ -22,16 +22,15 @@
 License-File: LICENSE
 
 [![Python Version](https://img.shields.io/pypi/pyversions/cellfinder-core.svg)](https://pypi.org/project/cellfinder-core)
 [![PyPI](https://img.shields.io/pypi/v/cellfinder-core.svg)](https://pypi.org/project/cellfinder-core)
 [![Downloads](https://pepy.tech/badge/cellfinder-core)](https://pepy.tech/project/cellfinder-core)
 [![Wheel](https://img.shields.io/pypi/wheel/cellfinder-core.svg)](https://pypi.org/project/cellfinder-core)
 [![Development Status](https://img.shields.io/pypi/status/cellfinder-core.svg)](https://github.com/brainglobe/cellfinder-core)
-[![Tests](https://img.shields.io/github/workflow/status/brainglobe/cellfinder-core/tests)](
-    https://github.com/brainglobe/cellfinder-core/actions)
+[![Tests](https://img.shields.io/github/workflow/status/brainglobe/cellfinder-core/tests)](https://github.com/brainglobe/cellfinder-core/actions)
 [![codecov](https://codecov.io/gh/brainglobe/cellfinder-core/branch/main/graph/badge.svg?token=nx1lhNI7ox)](https://codecov.io/gh/brainglobe/cellfinder-core)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Contributions](https://img.shields.io/badge/Contributions-Welcome-brightgreen.svg)](https://docs.brainglobe.info/cellfinder/contributing)
 [![Twitter](https://img.shields.io/twitter/follow/brain_globe?style=social)](https://twitter.com/brain_globe)
 
@@ -48,46 +47,45 @@
 whole-brain microscopy analysis, and the algorithm can also be implemented in
 [napari](https://napari.org/index.html) using the
 [cellfinder napari plugin](https://github.com/brainglobe/cellfinder-napari).
 
 ---
 
 ## Instructions
-
 ### Installation
-`cellfinder-core` supports Python >=3.7,
+`cellfinder-core` supports Python >=3.9,
 and works across Linux, Windows, and should work on most versions of macOS
 (although this is not tested).
 
 Assuming you have a Python environment set up
-(e.g. [using conda](https://docs.brainglobe.info/cellfinder/using-conda)),
+(e.g. [using conda](https://brainglobe.info/documentation/general/conda.html)),
 you can install `cellfinder-core` with:
 ```bash
 pip install cellfinder-core
 ```
 
 Once you have [installed napari](https://napari.org/index.html#installation).
 You can install napari either through the napari plugin installation tool, or
 directly from PyPI with:
 ```bash
 pip install cellfinder-napari
 ```
 
 N.B. To speed up cellfinder, you need CUDA & cuDNN installed. Instructions
-[here](https://docs.brainglobe.info/cellfinder/installation/using-gpu).
+[here](https://brainglobe.info/documentation/general/gpu.html).
 
 ### Usage
 Before using cellfinder-core, it may be useful to take a look at the
 [paper](https://doi.org/10.1371/journal.pcbi.1009074) which
 outlines the algorithm.
 
 The API is not yet fully documented. For an idea of what the parameters do,
 see the documentation for the cellfinder whole-brain microscopy image analysis
-command-line tool ([cell candidate detection](https://docs.brainglobe.info/cellfinder/user-guide/command-line/candidate-detection),
-[cell candidate classification](https://docs.brainglobe.info/cellfinder/user-guide/command-line/classification)).
+command-line tool ([cell candidate detection](https://brainglobe.info/documentation/cellfinder/user-guide/command-line/candidate-detection.html),
+[cell candidate classification](https://brainglobe.info/documentation/cellfinder/user-guide/command-line/classification.html)).
 It may also be useful to try the
 [cellfinder napari plugin](https://github.com/brainglobe/cellfinder-napari)
 so you can adjust the parameters in a GUI.
 
 #### To run the full pipeline (cell candidate detection and classification)
 ```python
 from cellfinder_core.main import main as cellfinder_run
@@ -238,16 +236,16 @@
 [Napari plugin](https://docs.brainglobe.info/cellfinder-napari/user-guide/training-data-generation).
 
 `cellfinder-core` comes with a 50-layer ResNet trained on ~100,000 data points
 from serial two-photon microscopy images of mouse brains
 (available [here](https://gin.g-node.org/cellfinder/training_data)).
 
 Training the network is likely simpler using the
-[command-line interface](https://docs.brainglobe.info/cellfinder/user-guide/training#start-training)
-or the [Napari plugin](https://docs.brainglobe.info/cellfinder-napari/user-guide/training-the-network),
+[command-line interface](https://brainglobe.info/documentation/cellfinder/user-guide/command-line/training/index.html)
+or the [Napari plugin](https://brainglobe.info/documentation/cellfinder/user-guide/napari-plugin/training-the-network.html),
 but it is possible through the Python API.
 
 ```python
 from pathlib import Path
 from cellfinder_core.train.train_yml import run as run_training
 
 # list of training yml files
@@ -272,15 +270,15 @@
 )
 ```
 
 ---
 ### More info
 
 More documentation about cellfinder and other BrainGlobe tools can be
-found [here](https://docs.brainglobe.info).
+found [here](https://brainglobe.info).
 
 This software is at a very early stage, and was written with our data in mind.
 Over time we hope to support other data types/formats. If you have any
 questions or issues, please get in touch [on the forum](https://forum.image.sc/tag/brainglobe) or by
 [raising an issue](https://github.com/brainglobe/cellfinder-core/issues).
 
 ---
@@ -308,24 +306,18 @@
 A deep-learning network (ResNet) is used to classify cell candidates as true
 cells or artefacts:
 
 ![raw](https://raw.githubusercontent.com/brainglobe/cellfinder/master/resources/classify.png)
 **Cassified cell candidates. Yellow - cells, Blue - artefacts**
 
 ## Contributing
-Contributions to cellfinder-core are more than welcome. Please see the [contributing guide](https://github.com/brainglobe/.github/blob/main/CONTRIBUTING.md).
+Contributions to cellfinder-core are more than welcome. Please see the [developers guide](https://brainglobe.info/developers/index.html).
 
 ---
 ## Citing cellfinder
 If you find this plugin useful, and use it in your research, please cite the paper outlining the cell detection algorithm:
 > Tyson, A. L., Rousseau, C. V., Niedworok, C. J., Keshavarzi, S., Tsitoura, C., Cossell, L., Strom, M. and Margrie, T. W. (2021) “A deep learning algorithm for 3D cell detection in whole mouse brain image datasets’ PLOS Computational Biology, 17(5), e1009074
 [https://doi.org/10.1371/journal.pcbi.1009074](https://doi.org/10.1371/journal.pcbi.1009074)
 
 **If you use this, or any other tools in the brainglobe suite, please
  [let us know](mailto:code@adamltyson.com?subject=cellfinder-core), and
  we'd be happy to promote your paper/talk etc.**
-
-
- ---
-The BrainGlobe project is generously supported by the Sainsbury Wellcome Centre and the Institute of Neuroscience, Technical University of Munich, with funding from Wellcome, the Gatsby Charitable Foundation and the Munich Cluster for Systems Neurology - Synergy.
-
-<img src='https://brainglobe.info/images/logos_combined.png' width="550">
```

### Comparing `cellfinder-core-0.4.0/README.md` & `cellfinder-core-0.4.1/src/cellfinder_core.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,36 @@
+Metadata-Version: 2.1
+Name: cellfinder-core
+Version: 0.4.1
+Summary: Automated 3D cell detection in large microscopy images
+Author-email: "Adam Tyson, Christian Niedworok, Charly Rousseau" <code@adamltyson.com>
+Project-URL: Homepage, https://brainglobe.info/cellfinder
+Project-URL: Source Code, https://github.com/brainglobe/cellfinder-core
+Project-URL: Bug Tracker, https://github.com/brainglobe/cellfinder-core/issues
+Project-URL: Documentation, https://docs.brainglobe.info/cellfinder
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering :: Image Recognition
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 [![Python Version](https://img.shields.io/pypi/pyversions/cellfinder-core.svg)](https://pypi.org/project/cellfinder-core)
 [![PyPI](https://img.shields.io/pypi/v/cellfinder-core.svg)](https://pypi.org/project/cellfinder-core)
 [![Downloads](https://pepy.tech/badge/cellfinder-core)](https://pepy.tech/project/cellfinder-core)
 [![Wheel](https://img.shields.io/pypi/wheel/cellfinder-core.svg)](https://pypi.org/project/cellfinder-core)
 [![Development Status](https://img.shields.io/pypi/status/cellfinder-core.svg)](https://github.com/brainglobe/cellfinder-core)
-[![Tests](https://img.shields.io/github/workflow/status/brainglobe/cellfinder-core/tests)](
-    https://github.com/brainglobe/cellfinder-core/actions)
+[![Tests](https://img.shields.io/github/workflow/status/brainglobe/cellfinder-core/tests)](https://github.com/brainglobe/cellfinder-core/actions)
 [![codecov](https://codecov.io/gh/brainglobe/cellfinder-core/branch/main/graph/badge.svg?token=nx1lhNI7ox)](https://codecov.io/gh/brainglobe/cellfinder-core)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Contributions](https://img.shields.io/badge/Contributions-Welcome-brightgreen.svg)](https://docs.brainglobe.info/cellfinder/contributing)
 [![Twitter](https://img.shields.io/twitter/follow/brain_globe?style=social)](https://twitter.com/brain_globe)
 
@@ -25,46 +47,45 @@
 whole-brain microscopy analysis, and the algorithm can also be implemented in
 [napari](https://napari.org/index.html) using the
 [cellfinder napari plugin](https://github.com/brainglobe/cellfinder-napari).
 
 ---
 
 ## Instructions
-
 ### Installation
-`cellfinder-core` supports Python >=3.7,
+`cellfinder-core` supports Python >=3.9,
 and works across Linux, Windows, and should work on most versions of macOS
 (although this is not tested).
 
 Assuming you have a Python environment set up
-(e.g. [using conda](https://docs.brainglobe.info/cellfinder/using-conda)),
+(e.g. [using conda](https://brainglobe.info/documentation/general/conda.html)),
 you can install `cellfinder-core` with:
 ```bash
 pip install cellfinder-core
 ```
 
 Once you have [installed napari](https://napari.org/index.html#installation).
 You can install napari either through the napari plugin installation tool, or
 directly from PyPI with:
 ```bash
 pip install cellfinder-napari
 ```
 
 N.B. To speed up cellfinder, you need CUDA & cuDNN installed. Instructions
-[here](https://docs.brainglobe.info/cellfinder/installation/using-gpu).
+[here](https://brainglobe.info/documentation/general/gpu.html).
 
 ### Usage
 Before using cellfinder-core, it may be useful to take a look at the
 [paper](https://doi.org/10.1371/journal.pcbi.1009074) which
 outlines the algorithm.
 
 The API is not yet fully documented. For an idea of what the parameters do,
 see the documentation for the cellfinder whole-brain microscopy image analysis
-command-line tool ([cell candidate detection](https://docs.brainglobe.info/cellfinder/user-guide/command-line/candidate-detection),
-[cell candidate classification](https://docs.brainglobe.info/cellfinder/user-guide/command-line/classification)).
+command-line tool ([cell candidate detection](https://brainglobe.info/documentation/cellfinder/user-guide/command-line/candidate-detection.html),
+[cell candidate classification](https://brainglobe.info/documentation/cellfinder/user-guide/command-line/classification.html)).
 It may also be useful to try the
 [cellfinder napari plugin](https://github.com/brainglobe/cellfinder-napari)
 so you can adjust the parameters in a GUI.
 
 #### To run the full pipeline (cell candidate detection and classification)
 ```python
 from cellfinder_core.main import main as cellfinder_run
@@ -215,16 +236,16 @@
 [Napari plugin](https://docs.brainglobe.info/cellfinder-napari/user-guide/training-data-generation).
 
 `cellfinder-core` comes with a 50-layer ResNet trained on ~100,000 data points
 from serial two-photon microscopy images of mouse brains
 (available [here](https://gin.g-node.org/cellfinder/training_data)).
 
 Training the network is likely simpler using the
-[command-line interface](https://docs.brainglobe.info/cellfinder/user-guide/training#start-training)
-or the [Napari plugin](https://docs.brainglobe.info/cellfinder-napari/user-guide/training-the-network),
+[command-line interface](https://brainglobe.info/documentation/cellfinder/user-guide/command-line/training/index.html)
+or the [Napari plugin](https://brainglobe.info/documentation/cellfinder/user-guide/napari-plugin/training-the-network.html),
 but it is possible through the Python API.
 
 ```python
 from pathlib import Path
 from cellfinder_core.train.train_yml import run as run_training
 
 # list of training yml files
@@ -249,15 +270,15 @@
 )
 ```
 
 ---
 ### More info
 
 More documentation about cellfinder and other BrainGlobe tools can be
-found [here](https://docs.brainglobe.info).
+found [here](https://brainglobe.info).
 
 This software is at a very early stage, and was written with our data in mind.
 Over time we hope to support other data types/formats. If you have any
 questions or issues, please get in touch [on the forum](https://forum.image.sc/tag/brainglobe) or by
 [raising an issue](https://github.com/brainglobe/cellfinder-core/issues).
 
 ---
@@ -285,24 +306,18 @@
 A deep-learning network (ResNet) is used to classify cell candidates as true
 cells or artefacts:
 
 ![raw](https://raw.githubusercontent.com/brainglobe/cellfinder/master/resources/classify.png)
 **Cassified cell candidates. Yellow - cells, Blue - artefacts**
 
 ## Contributing
-Contributions to cellfinder-core are more than welcome. Please see the [contributing guide](https://github.com/brainglobe/.github/blob/main/CONTRIBUTING.md).
+Contributions to cellfinder-core are more than welcome. Please see the [developers guide](https://brainglobe.info/developers/index.html).
 
 ---
 ## Citing cellfinder
 If you find this plugin useful, and use it in your research, please cite the paper outlining the cell detection algorithm:
 > Tyson, A. L., Rousseau, C. V., Niedworok, C. J., Keshavarzi, S., Tsitoura, C., Cossell, L., Strom, M. and Margrie, T. W. (2021) “A deep learning algorithm for 3D cell detection in whole mouse brain image datasets’ PLOS Computational Biology, 17(5), e1009074
 [https://doi.org/10.1371/journal.pcbi.1009074](https://doi.org/10.1371/journal.pcbi.1009074)
 
 **If you use this, or any other tools in the brainglobe suite, please
  [let us know](mailto:code@adamltyson.com?subject=cellfinder-core), and
  we'd be happy to promote your paper/talk etc.**
-
-
- ---
-The BrainGlobe project is generously supported by the Sainsbury Wellcome Centre and the Institute of Neuroscience, Technical University of Munich, with funding from Wellcome, the Gatsby Charitable Foundation and the Munich Cluster for Systems Neurology - Synergy.
-
-<img src='https://brainglobe.info/images/logos_combined.png' width="550">
```

### Comparing `cellfinder-core-0.4.0/benchmarks/README.md` & `cellfinder-core-0.4.1/benchmarks/README.md`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.0/benchmarks/detect_and_classify.py` & `cellfinder-core-0.4.1/benchmarks/detect_and_classify.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.0/benchmarks/filter_2d.py` & `cellfinder-core-0.4.1/benchmarks/filter_2d.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.0/benchmarks/filter_3d.py` & `cellfinder-core-0.4.1/benchmarks/filter_3d.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.0/pyproject.toml` & `cellfinder-core-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.0/src/cellfinder_core/classify/augment.py` & `cellfinder-core-0.4.1/src/cellfinder_core/classify/augment.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.0/src/cellfinder_core/classify/classify.py` & `cellfinder-core-0.4.1/src/cellfinder_core/classify/classify.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.0/src/cellfinder_core/classify/cube_generator.py` & `cellfinder-core-0.4.1/src/cellfinder_core/classify/cube_generator.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.0/src/cellfinder_core/classify/resnet.py` & `cellfinder-core-0.4.1/src/cellfinder_core/classify/resnet.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.0/src/cellfinder_core/classify/tools.py` & `cellfinder-core-0.4.1/src/cellfinder_core/classify/tools.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.0/src/cellfinder_core/detect/detect.py` & `cellfinder-core-0.4.1/src/cellfinder_core/detect/detect.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.0/src/cellfinder_core/detect/filters/plane/classical_filter.py` & `cellfinder-core-0.4.1/src/cellfinder_core/detect/filters/plane/classical_filter.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.0/src/cellfinder_core/detect/filters/plane/plane_filter.py` & `cellfinder-core-0.4.1/src/cellfinder_core/detect/filters/plane/plane_filter.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.0/src/cellfinder_core/detect/filters/plane/tile_walker.py` & `cellfinder-core-0.4.1/src/cellfinder_core/detect/filters/plane/tile_walker.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.0/src/cellfinder_core/detect/filters/setup_filters.py` & `cellfinder-core-0.4.1/src/cellfinder_core/detect/filters/setup_filters.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.0/src/cellfinder_core/detect/filters/volume/ball_filter.py` & `cellfinder-core-0.4.1/src/cellfinder_core/detect/filters/volume/ball_filter.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.0/src/cellfinder_core/detect/filters/volume/structure_detection.py` & `cellfinder-core-0.4.1/src/cellfinder_core/detect/filters/volume/structure_detection.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.0/src/cellfinder_core/detect/filters/volume/structure_splitting.py` & `cellfinder-core-0.4.1/src/cellfinder_core/detect/filters/volume/structure_splitting.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.0/src/cellfinder_core/detect/filters/volume/volume_filter.py` & `cellfinder-core-0.4.1/src/cellfinder_core/detect/filters/volume/volume_filter.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.0/src/cellfinder_core/download/cli.py` & `cellfinder-core-0.4.1/src/cellfinder_core/download/cli.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.0/src/cellfinder_core/download/download.py` & `cellfinder-core-0.4.1/src/cellfinder_core/download/download.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.0/src/cellfinder_core/download/models.py` & `cellfinder-core-0.4.1/src/cellfinder_core/download/models.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.0/src/cellfinder_core/main.py` & `cellfinder-core-0.4.1/src/cellfinder_core/main.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.0/src/cellfinder_core/tools/IO.py` & `cellfinder-core-0.4.1/src/cellfinder_core/tools/IO.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.0/src/cellfinder_core/tools/array_operations.py` & `cellfinder-core-0.4.1/src/cellfinder_core/tools/array_operations.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.0/src/cellfinder_core/tools/geometry.py` & `cellfinder-core-0.4.1/src/cellfinder_core/tools/geometry.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.0/src/cellfinder_core/tools/image_processing.py` & `cellfinder-core-0.4.1/src/cellfinder_core/tools/image_processing.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.0/src/cellfinder_core/tools/prep.py` & `cellfinder-core-0.4.1/src/cellfinder_core/tools/prep.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.0/src/cellfinder_core/tools/system.py` & `cellfinder-core-0.4.1/src/cellfinder_core/tools/system.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.0/src/cellfinder_core/tools/tf.py` & `cellfinder-core-0.4.1/src/cellfinder_core/tools/tf.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.0/src/cellfinder_core/tools/tiff.py` & `cellfinder-core-0.4.1/src/cellfinder_core/tools/tiff.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.0/src/cellfinder_core/tools/tools.py` & `cellfinder-core-0.4.1/src/cellfinder_core/tools/tools.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.0/src/cellfinder_core/train/train_yml.py` & `cellfinder-core-0.4.1/src/cellfinder_core/train/train_yml.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.0/src/cellfinder_core.egg-info/PKG-INFO` & `cellfinder-core-0.4.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,13 @@
-Metadata-Version: 2.1
-Name: cellfinder-core
-Version: 0.4.0
-Summary: Automated 3D cell detection in large microscopy images
-Author-email: "Adam Tyson, Christian Niedworok, Charly Rousseau" <code@adamltyson.com>
-Project-URL: Homepage, https://brainglobe.info/cellfinder
-Project-URL: Source Code, https://github.com/brainglobe/cellfinder-core
-Project-URL: Bug Tracker, https://github.com/brainglobe/cellfinder-core/issues
-Project-URL: Documentation, https://docs.brainglobe.info/cellfinder
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Image Recognition
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 [![Python Version](https://img.shields.io/pypi/pyversions/cellfinder-core.svg)](https://pypi.org/project/cellfinder-core)
 [![PyPI](https://img.shields.io/pypi/v/cellfinder-core.svg)](https://pypi.org/project/cellfinder-core)
 [![Downloads](https://pepy.tech/badge/cellfinder-core)](https://pepy.tech/project/cellfinder-core)
 [![Wheel](https://img.shields.io/pypi/wheel/cellfinder-core.svg)](https://pypi.org/project/cellfinder-core)
 [![Development Status](https://img.shields.io/pypi/status/cellfinder-core.svg)](https://github.com/brainglobe/cellfinder-core)
-[![Tests](https://img.shields.io/github/workflow/status/brainglobe/cellfinder-core/tests)](
-    https://github.com/brainglobe/cellfinder-core/actions)
+[![Tests](https://img.shields.io/github/workflow/status/brainglobe/cellfinder-core/tests)](https://github.com/brainglobe/cellfinder-core/actions)
 [![codecov](https://codecov.io/gh/brainglobe/cellfinder-core/branch/main/graph/badge.svg?token=nx1lhNI7ox)](https://codecov.io/gh/brainglobe/cellfinder-core)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Contributions](https://img.shields.io/badge/Contributions-Welcome-brightgreen.svg)](https://docs.brainglobe.info/cellfinder/contributing)
 [![Twitter](https://img.shields.io/twitter/follow/brain_globe?style=social)](https://twitter.com/brain_globe)
 
@@ -48,46 +24,45 @@
 whole-brain microscopy analysis, and the algorithm can also be implemented in
 [napari](https://napari.org/index.html) using the
 [cellfinder napari plugin](https://github.com/brainglobe/cellfinder-napari).
 
 ---
 
 ## Instructions
-
 ### Installation
-`cellfinder-core` supports Python >=3.7,
+`cellfinder-core` supports Python >=3.9,
 and works across Linux, Windows, and should work on most versions of macOS
 (although this is not tested).
 
 Assuming you have a Python environment set up
-(e.g. [using conda](https://docs.brainglobe.info/cellfinder/using-conda)),
+(e.g. [using conda](https://brainglobe.info/documentation/general/conda.html)),
 you can install `cellfinder-core` with:
 ```bash
 pip install cellfinder-core
 ```
 
 Once you have [installed napari](https://napari.org/index.html#installation).
 You can install napari either through the napari plugin installation tool, or
 directly from PyPI with:
 ```bash
 pip install cellfinder-napari
 ```
 
 N.B. To speed up cellfinder, you need CUDA & cuDNN installed. Instructions
-[here](https://docs.brainglobe.info/cellfinder/installation/using-gpu).
+[here](https://brainglobe.info/documentation/general/gpu.html).
 
 ### Usage
 Before using cellfinder-core, it may be useful to take a look at the
 [paper](https://doi.org/10.1371/journal.pcbi.1009074) which
 outlines the algorithm.
 
 The API is not yet fully documented. For an idea of what the parameters do,
 see the documentation for the cellfinder whole-brain microscopy image analysis
-command-line tool ([cell candidate detection](https://docs.brainglobe.info/cellfinder/user-guide/command-line/candidate-detection),
-[cell candidate classification](https://docs.brainglobe.info/cellfinder/user-guide/command-line/classification)).
+command-line tool ([cell candidate detection](https://brainglobe.info/documentation/cellfinder/user-guide/command-line/candidate-detection.html),
+[cell candidate classification](https://brainglobe.info/documentation/cellfinder/user-guide/command-line/classification.html)).
 It may also be useful to try the
 [cellfinder napari plugin](https://github.com/brainglobe/cellfinder-napari)
 so you can adjust the parameters in a GUI.
 
 #### To run the full pipeline (cell candidate detection and classification)
 ```python
 from cellfinder_core.main import main as cellfinder_run
@@ -238,16 +213,16 @@
 [Napari plugin](https://docs.brainglobe.info/cellfinder-napari/user-guide/training-data-generation).
 
 `cellfinder-core` comes with a 50-layer ResNet trained on ~100,000 data points
 from serial two-photon microscopy images of mouse brains
 (available [here](https://gin.g-node.org/cellfinder/training_data)).
 
 Training the network is likely simpler using the
-[command-line interface](https://docs.brainglobe.info/cellfinder/user-guide/training#start-training)
-or the [Napari plugin](https://docs.brainglobe.info/cellfinder-napari/user-guide/training-the-network),
+[command-line interface](https://brainglobe.info/documentation/cellfinder/user-guide/command-line/training/index.html)
+or the [Napari plugin](https://brainglobe.info/documentation/cellfinder/user-guide/napari-plugin/training-the-network.html),
 but it is possible through the Python API.
 
 ```python
 from pathlib import Path
 from cellfinder_core.train.train_yml import run as run_training
 
 # list of training yml files
@@ -272,15 +247,15 @@
 )
 ```
 
 ---
 ### More info
 
 More documentation about cellfinder and other BrainGlobe tools can be
-found [here](https://docs.brainglobe.info).
+found [here](https://brainglobe.info).
 
 This software is at a very early stage, and was written with our data in mind.
 Over time we hope to support other data types/formats. If you have any
 questions or issues, please get in touch [on the forum](https://forum.image.sc/tag/brainglobe) or by
 [raising an issue](https://github.com/brainglobe/cellfinder-core/issues).
 
 ---
@@ -308,24 +283,18 @@
 A deep-learning network (ResNet) is used to classify cell candidates as true
 cells or artefacts:
 
 ![raw](https://raw.githubusercontent.com/brainglobe/cellfinder/master/resources/classify.png)
 **Cassified cell candidates. Yellow - cells, Blue - artefacts**
 
 ## Contributing
-Contributions to cellfinder-core are more than welcome. Please see the [contributing guide](https://github.com/brainglobe/.github/blob/main/CONTRIBUTING.md).
+Contributions to cellfinder-core are more than welcome. Please see the [developers guide](https://brainglobe.info/developers/index.html).
 
 ---
 ## Citing cellfinder
 If you find this plugin useful, and use it in your research, please cite the paper outlining the cell detection algorithm:
 > Tyson, A. L., Rousseau, C. V., Niedworok, C. J., Keshavarzi, S., Tsitoura, C., Cossell, L., Strom, M. and Margrie, T. W. (2021) “A deep learning algorithm for 3D cell detection in whole mouse brain image datasets’ PLOS Computational Biology, 17(5), e1009074
 [https://doi.org/10.1371/journal.pcbi.1009074](https://doi.org/10.1371/journal.pcbi.1009074)
 
 **If you use this, or any other tools in the brainglobe suite, please
  [let us know](mailto:code@adamltyson.com?subject=cellfinder-core), and
  we'd be happy to promote your paper/talk etc.**
-
-
- ---
-The BrainGlobe project is generously supported by the Sainsbury Wellcome Centre and the Institute of Neuroscience, Technical University of Munich, with funding from Wellcome, the Gatsby Charitable Foundation and the Munich Cluster for Systems Neurology - Synergy.
-
-<img src='https://brainglobe.info/images/logos_combined.png' width="550">
```

### Comparing `cellfinder-core-0.4.0/src/cellfinder_core.egg-info/SOURCES.txt` & `cellfinder-core-0.4.1/src/cellfinder_core.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 .codecov.yml
 .gitignore
 .pre-commit-config.yaml
 CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.md
-cell_detection.md
 pyproject.toml
 tox.ini
 .github/workflows/test_and_deploy.yml
 .github/workflows/test_numba_off.yml
 benchmarks/README.md
 benchmarks/detect_and_classify.py
 benchmarks/filter_2d.py
```

### Comparing `cellfinder-core-0.4.0/tests/tests/conftest.py` & `cellfinder-core-0.4.1/tests/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.0/tests/tests/test_integration/test_detection.py` & `cellfinder-core-0.4.1/tests/tests/test_integration/test_detection.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.0/tests/tests/test_integration/test_detection_structure_splitting.py` & `cellfinder-core-0.4.1/tests/tests/test_integration/test_detection_structure_splitting.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.0/tests/tests/test_integration/test_train.py` & `cellfinder-core-0.4.1/tests/tests/test_integration/test_train.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.0/tests/tests/test_unit/test_detect/test_detect.py` & `cellfinder-core-0.4.1/tests/tests/test_unit/test_detect/test_detect.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.0/tests/tests/test_unit/test_detect/test_filters/test_volume_filters/test_structure_detection.py` & `cellfinder-core-0.4.1/tests/tests/test_unit/test_detect/test_filters/test_volume_filters/test_structure_detection.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.0/tests/tests/test_unit/test_tools/test_image_processing.py` & `cellfinder-core-0.4.1/tests/tests/test_unit/test_tools/test_image_processing.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.0/tests/tests/test_unit/test_tools/test_system.py` & `cellfinder-core-0.4.1/tests/tests/test_unit/test_tools/test_system.py`

 * *Files identical despite different names*

### Comparing `cellfinder-core-0.4.0/tests/tests/test_unit/test_tools/test_tools_general.py` & `cellfinder-core-0.4.1/tests/tests/test_unit/test_tools/test_tools_general.py`

 * *Files identical despite different names*

