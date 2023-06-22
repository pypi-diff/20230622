# Comparing `tmp/ocp-freecad-cam-0.9.1.tar.gz` & `tmp/ocp-freecad-cam-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocp-freecad-cam-0.9.1.tar", last modified: Wed Jun 21 19:50:13 2023, max compression
+gzip compressed data, was "ocp-freecad-cam-0.9.2.tar", last modified: Thu Jun 22 06:40:27 2023, max compression
```

## Comparing `ocp-freecad-cam-0.9.1.tar` & `ocp-freecad-cam-0.9.2.tar`

### file list

```diff
@@ -1,63 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:50:13.267669 ocp-freecad-cam-0.9.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:50:13.263669 ocp-freecad-cam-0.9.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-21 19:49:55.000000 ocp-freecad-cam-0.9.1/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:50:13.263669 ocp-freecad-cam-0.9.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-06-21 19:49:55.000000 ocp-freecad-cam-0.9.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-21 19:49:55.000000 ocp-freecad-cam-0.9.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-21 19:49:55.000000 ocp-freecad-cam-0.9.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-21 19:49:55.000000 ocp-freecad-cam-0.9.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-06-21 19:49:55.000000 ocp-freecad-cam-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-06-21 19:50:13.267669 ocp-freecad-cam-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-06-21 19:49:55.000000 ocp-freecad-cam-0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:50:13.263669 ocp-freecad-cam-0.9.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-21 19:49:55.000000 ocp-freecad-cam-0.9.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-21 19:49:55.000000 ocp-freecad-cam-0.9.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-21 19:49:55.000000 ocp-freecad-cam-0.9.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:50:13.267669 ocp-freecad-cam-0.9.1/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-21 19:49:55.000000 ocp-freecad-cam-0.9.1/docs/examples/cq_adaptive.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-21 19:49:55.000000 ocp-freecad-cam-0.9.1/docs/examples/cq_drill.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-21 19:49:55.000000 ocp-freecad-cam-0.9.1/docs/examples/cq_helix.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-21 19:49:55.000000 ocp-freecad-cam-0.9.1/docs/examples/cq_pocket.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-21 19:49:55.000000 ocp-freecad-cam-0.9.1/docs/examples/cq_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-21 19:49:55.000000 ocp-freecad-cam-0.9.1/docs/examples/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-06-21 19:49:55.000000 ocp-freecad-cam-0.9.1/docs/examples/generate_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:50:13.267669 ocp-freecad-cam-0.9.1/docs/examples/images/
--rw-r--r--   0 runner    (1001) docker     (123)    22857 2023-06-21 19:49:55.000000 ocp-freecad-cam-0.9.1/docs/examples/images/cq_adaptive.png
--rw-r--r--   0 runner    (1001) docker     (123)    11373 2023-06-21 19:49:55.000000 ocp-freecad-cam-0.9.1/docs/examples/images/cq_drill.png
--rw-r--r--   0 runner    (1001) docker     (123)    19879 2023-06-21 19:49:55.000000 ocp-freecad-cam-0.9.1/docs/examples/images/cq_helix.png
--rw-r--r--   0 runner    (1001) docker     (123)    22366 2023-06-21 19:49:55.000000 ocp-freecad-cam-0.9.1/docs/examples/images/cq_pocket.png
--rw-r--r--   0 runner    (1001) docker     (123)    12271 2023-06-21 19:49:55.000000 ocp-freecad-cam-0.9.1/docs/examples/images/cq_profile.png
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-21 19:49:55.000000 ocp-freecad-cam-0.9.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-21 19:49:55.000000 ocp-freecad-cam-0.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-21 19:49:55.000000 ocp-freecad-cam-0.9.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-21 19:49:55.000000 ocp-freecad-cam-0.9.1/requirements-dev.in
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-06-21 19:49:55.000000 ocp-freecad-cam-0.9.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 19:49:55.000000 ocp-freecad-cam-0.9.1/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 19:49:55.000000 ocp-freecad-cam-0.9.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 19:50:13.267669 ocp-freecad-cam-0.9.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:50:13.263669 ocp-freecad-cam-0.9.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:50:13.267669 ocp-freecad-cam-0.9.1/src/ocp_freecad_cam/
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-21 19:49:55.000000 ocp-freecad-cam-0.9.1/src/ocp_freecad_cam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32305 2023-06-21 19:49:55.000000 ocp-freecad-cam-0.9.1/src/ocp_freecad_cam/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-06-21 19:49:55.000000 ocp-freecad-cam-0.9.1/src/ocp_freecad_cam/api_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-06-21 19:49:55.000000 ocp-freecad-cam-0.9.1/src/ocp_freecad_cam/api_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-21 19:49:55.000000 ocp-freecad-cam-0.9.1/src/ocp_freecad_cam/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    28457 2023-06-21 19:49:55.000000 ocp-freecad-cam-0.9.1/src/ocp_freecad_cam/fc_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-21 19:49:55.000000 ocp-freecad-cam-0.9.1/src/ocp_freecad_cam/fc_impl_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    16109 2023-06-21 19:49:55.000000 ocp-freecad-cam-0.9.1/src/ocp_freecad_cam/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:50:13.267669 ocp-freecad-cam-0.9.1/src/ocp_freecad_cam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-06-21 19:50:13.000000 ocp-freecad-cam-0.9.1/src/ocp_freecad_cam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-21 19:50:13.000000 ocp-freecad-cam-0.9.1/src/ocp_freecad_cam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 19:50:13.000000 ocp-freecad-cam-0.9.1/src/ocp_freecad_cam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-21 19:50:13.000000 ocp-freecad-cam-0.9.1/src/ocp_freecad_cam.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:50:13.263669 ocp-freecad-cam-0.9.1/stubs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:50:13.267669 ocp-freecad-cam-0.9.1/stubs/Part/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-21 19:49:55.000000 ocp-freecad-cam-0.9.1/stubs/Part/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:50:13.267669 ocp-freecad-cam-0.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-21 19:49:55.000000 ocp-freecad-cam-0.9.1/tests/test_adaptive.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-21 19:49:55.000000 ocp-freecad-cam-0.9.1/tests/test_drill.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-21 19:49:55.000000 ocp-freecad-cam-0.9.1/tests/test_engrave.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-21 19:49:55.000000 ocp-freecad-cam-0.9.1/tests/test_helix.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-21 19:49:55.000000 ocp-freecad-cam-0.9.1/tests/test_params.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-21 19:49:55.000000 ocp-freecad-cam-0.9.1/tests/test_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-21 19:49:55.000000 ocp-freecad-cam-0.9.1/tests/test_waterline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:40:27.790021 ocp-freecad-cam-0.9.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:40:27.786021 ocp-freecad-cam-0.9.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-22 06:40:08.000000 ocp-freecad-cam-0.9.2/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:40:27.786021 ocp-freecad-cam-0.9.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-06-22 06:40:08.000000 ocp-freecad-cam-0.9.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-22 06:40:08.000000 ocp-freecad-cam-0.9.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-22 06:40:08.000000 ocp-freecad-cam-0.9.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-22 06:40:08.000000 ocp-freecad-cam-0.9.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-06-22 06:40:08.000000 ocp-freecad-cam-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-06-22 06:40:27.790021 ocp-freecad-cam-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-06-22 06:40:08.000000 ocp-freecad-cam-0.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:40:27.786021 ocp-freecad-cam-0.9.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-22 06:40:08.000000 ocp-freecad-cam-0.9.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-22 06:40:08.000000 ocp-freecad-cam-0.9.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-22 06:40:08.000000 ocp-freecad-cam-0.9.2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:40:27.786021 ocp-freecad-cam-0.9.2/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-22 06:40:08.000000 ocp-freecad-cam-0.9.2/docs/examples/cq_adaptive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-22 06:40:08.000000 ocp-freecad-cam-0.9.2/docs/examples/cq_drill.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-22 06:40:08.000000 ocp-freecad-cam-0.9.2/docs/examples/cq_helix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-22 06:40:08.000000 ocp-freecad-cam-0.9.2/docs/examples/cq_pocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-22 06:40:08.000000 ocp-freecad-cam-0.9.2/docs/examples/cq_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-22 06:40:08.000000 ocp-freecad-cam-0.9.2/docs/examples/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-06-22 06:40:08.000000 ocp-freecad-cam-0.9.2/docs/examples/generate_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:40:27.786021 ocp-freecad-cam-0.9.2/docs/examples/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    22857 2023-06-22 06:40:08.000000 ocp-freecad-cam-0.9.2/docs/examples/images/cq_adaptive.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11373 2023-06-22 06:40:08.000000 ocp-freecad-cam-0.9.2/docs/examples/images/cq_drill.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19879 2023-06-22 06:40:08.000000 ocp-freecad-cam-0.9.2/docs/examples/images/cq_helix.png
+-rw-r--r--   0 runner    (1001) docker     (123)    22366 2023-06-22 06:40:08.000000 ocp-freecad-cam-0.9.2/docs/examples/images/cq_pocket.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12271 2023-06-22 06:40:08.000000 ocp-freecad-cam-0.9.2/docs/examples/images/cq_profile.png
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-22 06:40:08.000000 ocp-freecad-cam-0.9.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-22 06:40:08.000000 ocp-freecad-cam-0.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-22 06:40:08.000000 ocp-freecad-cam-0.9.2/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-22 06:40:08.000000 ocp-freecad-cam-0.9.2/requirements-dev.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-06-22 06:40:08.000000 ocp-freecad-cam-0.9.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 06:40:08.000000 ocp-freecad-cam-0.9.2/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 06:40:08.000000 ocp-freecad-cam-0.9.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 06:40:27.790021 ocp-freecad-cam-0.9.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:40:27.782021 ocp-freecad-cam-0.9.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:40:27.790021 ocp-freecad-cam-0.9.2/src/ocp_freecad_cam/
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-22 06:40:08.000000 ocp-freecad-cam-0.9.2/src/ocp_freecad_cam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32305 2023-06-22 06:40:08.000000 ocp-freecad-cam-0.9.2/src/ocp_freecad_cam/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-06-22 06:40:08.000000 ocp-freecad-cam-0.9.2/src/ocp_freecad_cam/api_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-06-22 06:40:08.000000 ocp-freecad-cam-0.9.2/src/ocp_freecad_cam/api_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-22 06:40:08.000000 ocp-freecad-cam-0.9.2/src/ocp_freecad_cam/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28457 2023-06-22 06:40:08.000000 ocp-freecad-cam-0.9.2/src/ocp_freecad_cam/fc_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-22 06:40:08.000000 ocp-freecad-cam-0.9.2/src/ocp_freecad_cam/fc_impl_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16109 2023-06-22 06:40:08.000000 ocp-freecad-cam-0.9.2/src/ocp_freecad_cam/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:40:27.790021 ocp-freecad-cam-0.9.2/src/ocp_freecad_cam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-06-22 06:40:27.000000 ocp-freecad-cam-0.9.2/src/ocp_freecad_cam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-22 06:40:27.000000 ocp-freecad-cam-0.9.2/src/ocp_freecad_cam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 06:40:27.000000 ocp-freecad-cam-0.9.2/src/ocp_freecad_cam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-22 06:40:27.000000 ocp-freecad-cam-0.9.2/src/ocp_freecad_cam.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:40:27.782021 ocp-freecad-cam-0.9.2/stubs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:40:27.790021 ocp-freecad-cam-0.9.2/stubs/Part/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-22 06:40:08.000000 ocp-freecad-cam-0.9.2/stubs/Part/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:40:27.790021 ocp-freecad-cam-0.9.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-22 06:40:08.000000 ocp-freecad-cam-0.9.2/tests/test_adaptive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-22 06:40:08.000000 ocp-freecad-cam-0.9.2/tests/test_drill.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-22 06:40:08.000000 ocp-freecad-cam-0.9.2/tests/test_engrave.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-22 06:40:08.000000 ocp-freecad-cam-0.9.2/tests/test_gcode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-22 06:40:08.000000 ocp-freecad-cam-0.9.2/tests/test_helix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-22 06:40:08.000000 ocp-freecad-cam-0.9.2/tests/test_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-22 06:40:08.000000 ocp-freecad-cam-0.9.2/tests/test_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-22 06:40:08.000000 ocp-freecad-cam-0.9.2/tests/test_waterline.py
```

### Comparing `ocp-freecad-cam-0.9.1/.github/workflows/ci.yml` & `ocp-freecad-cam-0.9.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.1/.github/workflows/release.yml` & `ocp-freecad-cam-0.9.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.1/.readthedocs.yaml` & `ocp-freecad-cam-0.9.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.1/LICENSE` & `ocp-freecad-cam-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.1/PKG-INFO` & `ocp-freecad-cam-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocp-freecad-cam
-Version: 0.9.1
+Version: 0.9.2
 Summary: OCP FreeCAD CAM
 Author-email: Matti Eiden <snaipperi@gmail.com>
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/voneiden/ocp-freecad-cam/issues/
 Project-URL: Documentation, https://github.com/voneiden/ocp-freecad-cam/
 Project-URL: Source Code, https://github.com/voneiden/ocp-freecad-cam/
 Keywords: cadquery,viewer
```

### Comparing `ocp-freecad-cam-0.9.1/README.md` & `ocp-freecad-cam-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.1/docs/Makefile` & `ocp-freecad-cam-0.9.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.1/docs/conf.py` & `ocp-freecad-cam-0.9.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.1/docs/examples/examples.rst` & `ocp-freecad-cam-0.9.2/docs/examples/examples.rst`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.1/docs/examples/generate_image.py` & `ocp-freecad-cam-0.9.2/docs/examples/generate_image.py`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.1/docs/examples/images/cq_adaptive.png` & `ocp-freecad-cam-0.9.2/docs/examples/images/cq_adaptive.png`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.1/docs/examples/images/cq_drill.png` & `ocp-freecad-cam-0.9.2/docs/examples/images/cq_drill.png`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.1/docs/examples/images/cq_helix.png` & `ocp-freecad-cam-0.9.2/docs/examples/images/cq_helix.png`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.1/docs/examples/images/cq_pocket.png` & `ocp-freecad-cam-0.9.2/docs/examples/images/cq_pocket.png`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.1/docs/examples/images/cq_profile.png` & `ocp-freecad-cam-0.9.2/docs/examples/images/cq_profile.png`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.1/docs/index.rst` & `ocp-freecad-cam-0.9.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.1/pyproject.toml` & `ocp-freecad-cam-0.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.1/requirements-dev.txt` & `ocp-freecad-cam-0.9.2/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.1/src/ocp_freecad_cam/__init__.py` & `ocp-freecad-cam-0.9.2/src/ocp_freecad_cam/__init__.py`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.1/src/ocp_freecad_cam/api.py` & `ocp-freecad-cam-0.9.2/src/ocp_freecad_cam/api.py`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.1/src/ocp_freecad_cam/api_tool.py` & `ocp-freecad-cam-0.9.2/src/ocp_freecad_cam/api_tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     param_mapping: ClassVar[ParamMapping] = {
         "chip_load": "ChipLoad",
         "flutes": "Flutes",
         "material": "Material",
     }
 
     tc_param_mapping: ClassVar[ParamMapping] = {
+        "speed": "SpindleSpeed",
         "spindle_dir": (
             "SpindleDirection",
             {"forward": "Forward", "reverse": "Reverse", "none": "None"},
         ),
         "h_feed": AutoUnitKey("HorizFeed", mode="feed"),
         "v_feed": AutoUnitKey("VertFeed", mode="feed"),
     }
@@ -45,14 +46,15 @@
     chip_load: str = None
     flutes: int = None
     material: str = None
 
     # TC attributes
     h_feed: float | str = None
     v_feed: float | str = None
+    speed: float | str = None
     spindle_dir: Literal["forward", "reverse", "none"] = None
 
     def __post_init__(self):
         self._bit = None
         self._tool_controller = None
 
         self.params = map_params(
```

### Comparing `ocp-freecad-cam-0.9.1/src/ocp_freecad_cam/api_util.py` & `ocp-freecad-cam-0.9.2/src/ocp_freecad_cam/api_util.py`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.1/src/ocp_freecad_cam/common.py` & `ocp-freecad-cam-0.9.2/src/ocp_freecad_cam/common.py`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.1/src/ocp_freecad_cam/fc_impl.py` & `ocp-freecad-cam-0.9.2/src/ocp_freecad_cam/fc_impl.py`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.1/src/ocp_freecad_cam/fc_impl_util.py` & `ocp-freecad-cam-0.9.2/src/ocp_freecad_cam/fc_impl_util.py`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.1/src/ocp_freecad_cam/visualizer.py` & `ocp-freecad-cam-0.9.2/src/ocp_freecad_cam/visualizer.py`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.1/src/ocp_freecad_cam.egg-info/PKG-INFO` & `ocp-freecad-cam-0.9.2/src/ocp_freecad_cam.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocp-freecad-cam
-Version: 0.9.1
+Version: 0.9.2
 Summary: OCP FreeCAD CAM
 Author-email: Matti Eiden <snaipperi@gmail.com>
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/voneiden/ocp-freecad-cam/issues/
 Project-URL: Documentation, https://github.com/voneiden/ocp-freecad-cam/
 Project-URL: Source Code, https://github.com/voneiden/ocp-freecad-cam/
 Keywords: cadquery,viewer
```

### Comparing `ocp-freecad-cam-0.9.1/src/ocp_freecad_cam.egg-info/SOURCES.txt` & `ocp-freecad-cam-0.9.2/src/ocp_freecad_cam.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -39,11 +39,12 @@
 src/ocp_freecad_cam.egg-info/SOURCES.txt
 src/ocp_freecad_cam.egg-info/dependency_links.txt
 src/ocp_freecad_cam.egg-info/top_level.txt
 stubs/Part/__init__.pyi
 tests/test_adaptive.py
 tests/test_drill.py
 tests/test_engrave.py
+tests/test_gcode.py
 tests/test_helix.py
 tests/test_params.py
 tests/test_profile.py
 tests/test_waterline.py
```

### Comparing `ocp-freecad-cam-0.9.1/tests/test_adaptive.py` & `ocp-freecad-cam-0.9.2/tests/test_adaptive.py`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.1/tests/test_drill.py` & `ocp-freecad-cam-0.9.2/tests/test_drill.py`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.1/tests/test_engrave.py` & `ocp-freecad-cam-0.9.2/tests/test_engrave.py`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.1/tests/test_helix.py` & `ocp-freecad-cam-0.9.2/tests/test_helix.py`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.1/tests/test_params.py` & `ocp-freecad-cam-0.9.2/tests/test_params.py`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.1/tests/test_profile.py` & `ocp-freecad-cam-0.9.2/tests/test_profile.py`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.1/tests/test_waterline.py` & `ocp-freecad-cam-0.9.2/tests/test_waterline.py`

 * *Files identical despite different names*

