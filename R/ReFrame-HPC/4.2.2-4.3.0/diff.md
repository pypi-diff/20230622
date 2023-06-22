# Comparing `tmp/ReFrame-HPC-4.2.2.tar.gz` & `tmp/ReFrame-HPC-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ReFrame-HPC-4.2.2.tar", last modified: Fri Jun 16 16:23:46 2023, max compression
+gzip compressed data, was "ReFrame-HPC-4.3.0.tar", last modified: Thu Jun 22 19:29:37 2023, max compression
```

## Comparing `ReFrame-HPC-4.2.2.tar` & `ReFrame-HPC-4.3.0.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:23:46.365694 ReFrame-HPC-4.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-06-16 16:23:46.365694 ReFrame-HPC-4.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/README_minimal.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:23:46.341693 ReFrame-HPC-4.2.2/ReFrame_HPC.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-06-16 16:23:46.000000 ReFrame-HPC-4.2.2/ReFrame_HPC.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-06-16 16:23:46.000000 ReFrame-HPC-4.2.2/ReFrame_HPC.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 16:23:46.000000 ReFrame-HPC-4.2.2/ReFrame_HPC.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-16 16:23:46.000000 ReFrame-HPC-4.2.2/ReFrame_HPC.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-16 16:23:46.000000 ReFrame-HPC-4.2.2/ReFrame_HPC.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:23:46.341693 ReFrame-HPC-4.2.2/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      546 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/bin/reframe
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:23:46.341693 ReFrame-HPC-4.2.2/reframe/
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:23:46.353694 ReFrame-HPC-4.2.2/reframe/core/
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/backends.py
--rw-r--r--   0 runner    (1001) docker     (123)    31411 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/buildsystems.py
--rw-r--r--   0 runner    (1001) docker     (123)     7455 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)    23120 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8980 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     9592 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/deferrable.py
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/environments.py
--rw-r--r--   0 runner    (1001) docker     (123)    10627 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    44510 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:23:46.357694 ReFrame-HPC-4.2.2/reframe/core/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/launchers/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/launchers/mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/launchers/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)    32490 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    36789 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    37547 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/namespaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    16354 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    94662 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    14256 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:23:46.357694 ReFrame-HPC-4.2.2/reframe/core/schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)    19439 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/schedulers/flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/schedulers/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/schedulers/lsf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/schedulers/oar.py
--rw-r--r--   0 runner    (1001) docker     (123)     9805 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/schedulers/pbs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/schedulers/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/schedulers/sge.py
--rw-r--r--   0 runner    (1001) docker     (123)    25280 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/schedulers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/shell.py
--rw-r--r--   0 runner    (1001) docker     (123)    22673 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/systems.py
--rw-r--r--   0 runner    (1001) docker     (123)    29596 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/core/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:23:46.361694 ReFrame-HPC-4.2.2/reframe/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/frontend/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     8272 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/frontend/autodetect.py
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/frontend/ci.py
--rw-r--r--   0 runner    (1001) docker     (123)    55077 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/frontend/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/frontend/dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:23:46.361694 ReFrame-HPC-4.2.2/reframe/frontend/executors/
--rw-r--r--   0 runner    (1001) docker     (123)    21499 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/frontend/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22692 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/frontend/executors/policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/frontend/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/frontend/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/frontend/printer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8849 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/frontend/runreport.py
--rw-r--r--   0 runner    (1001) docker     (123)    16299 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/frontend/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/frontend/testgenerators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:23:46.365694 ReFrame-HPC-4.2.2/reframe/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)    25667 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/schemas/config.json
--rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/schemas/junit.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/schemas/runreport.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:23:46.365694 ReFrame-HPC-4.2.2/reframe/utility/
--rw-r--r--   0 runner    (1001) docker     (123)    49317 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/utility/color.py
--rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/utility/cpuinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/utility/jsonext.py
--rw-r--r--   0 runner    (1001) docker     (123)    21443 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/utility/osext.py
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/utility/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    32327 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/utility/sanity.py
--rw-r--r--   0 runner    (1001) docker     (123)    14330 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/utility/typecheck.py
--rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/utility/udeps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-06-16 16:23:33.000000 ReFrame-HPC-4.2.2/reframe/utility/versioning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-16 16:23:46.365694 ReFrame-HPC-4.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:29:37.689236 ReFrame-HPC-4.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-06-22 19:29:37.689236 ReFrame-HPC-4.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/README_minimal.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:29:37.681236 ReFrame-HPC-4.3.0/ReFrame_HPC.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-06-22 19:29:37.000000 ReFrame-HPC-4.3.0/ReFrame_HPC.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-06-22 19:29:37.000000 ReFrame-HPC-4.3.0/ReFrame_HPC.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 19:29:37.000000 ReFrame-HPC-4.3.0/ReFrame_HPC.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-22 19:29:37.000000 ReFrame-HPC-4.3.0/ReFrame_HPC.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-22 19:29:37.000000 ReFrame-HPC-4.3.0/ReFrame_HPC.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:29:37.681236 ReFrame-HPC-4.3.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      546 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/bin/reframe
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:29:37.681236 ReFrame-HPC-4.3.0/reframe/
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:29:37.685236 ReFrame-HPC-4.3.0/reframe/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/core/backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32121 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/core/buildsystems.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7455 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/core/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24489 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8980 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/core/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/core/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9592 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/core/deferrable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8686 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/core/environments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10627 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/core/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44510 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/core/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/core/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:29:37.685236 ReFrame-HPC-4.3.0/reframe/core/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/core/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/core/launchers/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/core/launchers/mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/core/launchers/rsh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34546 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/core/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36657 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/core/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37547 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/core/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/core/namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16354 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/core/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94662 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/core/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14317 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/core/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:29:37.685236 ReFrame-HPC-4.3.0/reframe/core/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)    19439 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/core/schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/core/schedulers/flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/core/schedulers/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/core/schedulers/lsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/core/schedulers/oar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9805 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/core/schedulers/pbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/core/schedulers/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/core/schedulers/sge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25280 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/core/schedulers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/core/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/core/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22804 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/core/systems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29596 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/core/variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/core/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:29:37.689236 ReFrame-HPC-4.3.0/reframe/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/frontend/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8272 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/frontend/autodetect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/frontend/ci.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56992 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/frontend/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/frontend/dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:29:37.689236 ReFrame-HPC-4.3.0/reframe/frontend/executors/
+-rw-r--r--   0 runner    (1001) docker     (123)    21499 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/frontend/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22692 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/frontend/executors/policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/frontend/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8306 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/frontend/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/frontend/printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8849 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/frontend/runreport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16299 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/frontend/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6240 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/frontend/testgenerators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:29:37.689236 ReFrame-HPC-4.3.0/reframe/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)    26220 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/schemas/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/schemas/junit.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/schemas/runreport.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:29:37.689236 ReFrame-HPC-4.3.0/reframe/utility/
+-rw-r--r--   0 runner    (1001) docker     (123)    49673 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/utility/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/utility/cpuinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/utility/jsonext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21443 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/utility/osext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/utility/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32327 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/utility/sanity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14330 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/utility/typecheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/utility/udeps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-06-22 19:29:24.000000 ReFrame-HPC-4.3.0/reframe/utility/versioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-22 19:29:37.689236 ReFrame-HPC-4.3.0/setup.cfg
```

### Comparing `ReFrame-HPC-4.2.2/LICENSE` & `ReFrame-HPC-4.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.2/PKG-INFO` & `ReFrame-HPC-4.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReFrame-HPC
-Version: 4.2.2
+Version: 4.3.0
 Summary: ReFrame is a powerful framework for writing system regression tests and benchmarks, specifically targeted to HPC systems
 Home-page: https://github.com/reframe-hpc/reframe
 Author: Swiss National Supercomputing Center (CSCS/ETH Zurich), ReFrame Project Developers
 License: BSD 3-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `ReFrame-HPC-4.2.2/README.md` & `ReFrame-HPC-4.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.2/README_minimal.md` & `ReFrame-HPC-4.3.0/README_minimal.md`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.2/ReFrame_HPC.egg-info/PKG-INFO` & `ReFrame-HPC-4.3.0/ReFrame_HPC.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReFrame-HPC
-Version: 4.2.2
+Version: 4.3.0
 Summary: ReFrame is a powerful framework for writing system regression tests and benchmarks, specifically targeted to HPC systems
 Home-page: https://github.com/reframe-hpc/reframe
 Author: Swiss National Supercomputing Center (CSCS/ETH Zurich), ReFrame Project Developers
 License: BSD 3-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `ReFrame-HPC-4.2.2/ReFrame_HPC.egg-info/SOURCES.txt` & `ReFrame-HPC-4.3.0/ReFrame_HPC.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 reframe/core/shell.py
 reframe/core/systems.py
 reframe/core/variables.py
 reframe/core/warnings.py
 reframe/core/launchers/__init__.py
 reframe/core/launchers/local.py
 reframe/core/launchers/mpi.py
-reframe/core/launchers/ssh.py
+reframe/core/launchers/rsh.py
 reframe/core/schedulers/__init__.py
 reframe/core/schedulers/flux.py
 reframe/core/schedulers/local.py
 reframe/core/schedulers/lsf.py
 reframe/core/schedulers/oar.py
 reframe/core/schedulers/pbs.py
 reframe/core/schedulers/registry.py
```

### Comparing `ReFrame-HPC-4.2.2/bin/reframe` & `ReFrame-HPC-4.3.0/bin/reframe`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.2/reframe/__init__.py` & `ReFrame-HPC-4.3.0/reframe/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # ReFrame Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: BSD-3-Clause
 
 import os
 import sys
 
-VERSION = '4.2.2'
+VERSION = '4.3.0'
 INSTALL_PREFIX = os.path.normpath(
     os.path.abspath(os.path.join(os.path.dirname(__file__), '..'))
 )
 MIN_PYTHON_VERSION = (3, 6, 0)
 
 # Check python version
 if sys.version_info[:3] < MIN_PYTHON_VERSION:
```

### Comparing `ReFrame-HPC-4.2.2/reframe/core/backends.py` & `ReFrame-HPC-4.3.0/reframe/core/backends.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 import reframe.core.fields as fields
 from reframe.core.exceptions import ConfigError
 
 _launcher_backend_modules = [
     'reframe.core.launchers.local',
     'reframe.core.launchers.mpi',
-    'reframe.core.launchers.ssh'
+    'reframe.core.launchers.rsh'
 ]
 _launchers = {}
 _scheduler_backend_modules = [
     'reframe.core.schedulers.flux',
     'reframe.core.schedulers.local',
     'reframe.core.schedulers.lsf',
     'reframe.core.schedulers.pbs',
```

### Comparing `ReFrame-HPC-4.2.2/reframe/core/buildsystems.py` & `ReFrame-HPC-4.3.0/reframe/core/buildsystems.py`

 * *Files 1% similar despite different names*

```diff
@@ -859,28 +859,43 @@
 
     #: Emit the necessary ``spack load`` commands before running the test.
     #:
     #: :type: :class:`bool`
     #: :default: :obj:`True`
     emit_load_cmds = variable(bool, value=True)
 
-    #: Options to pass to ``spack install``
+    #: Options to pass to ``spack install``.
     #:
     #: :type: :class:`List[str]`
     #: :default: ``[]``
     install_opts = variable(typ.List[str], value=[])
 
     #: A list of Spack configurations in flattened YAML.
     #:
     #: :type: :class:`List[str]`
     #: :default: ``[]``
     #:
     #: .. versionadded:: 4.2
     config_opts = variable(typ.List[str], value=[])
 
+    #: Options to pass to ``spack env create``.
+    #:
+    #: :type: :class:`List[str]`
+    #: :default: ``[]``
+    env_create_opts = variable(typ.List[str], value=[])
+
+    #: A list of commands to run after a Spack environment
+    #: is created, but before it is installed.
+    #:
+    #: :type: :class:`List[str]`
+    #: :default: ``[]``
+    #:
+    preinstall_cmds = variable(typ.List[str], value=[])
+
+
     def __init__(self):
         # Set to True if the environment was auto-generated
         self._auto_env = False
 
     def emit_build_commands(self, environ):
         ret = self._create_env_cmds()
 
@@ -893,28 +908,37 @@
         for opt in config_opts:
             ret.append(f'spack -e {self.environment} config add "{opt}"')
 
         if self.specs:
             specs_str = ' '.join(self.specs)
             ret.append(f'spack -e {self.environment} add {specs_str}')
 
+        if self.preinstall_cmds:
+            for cmd in self.preinstall_cmds:
+                ret.append(cmd)
+
         install_cmd = f'spack -e {self.environment} install'
         if self.install_opts:
             install_cmd += ' ' + ' '.join(self.install_opts)
 
         ret.append(install_cmd)
         return ret
 
     def _create_env_cmds(self):
         if self.environment:
             return []
 
         self.environment = 'rfm_spack_env'
         self._auto_env = True
-        return [f'spack env create -d {self.environment}']
+
+        if self.env_create_opts:
+            env_create_opts = ' '.join(self.env_create_opts)
+            return [f'spack env create -d {self.environment} {env_create_opts}']
+        else:
+            return [f'spack env create -d {self.environment}']
 
     def prepare_cmds(self):
         cmds = self._create_env_cmds()
         if self.specs and self.emit_load_cmds:
             cmds.append(
                 f'eval `spack -e {self.environment} load '
                 f'--sh {" ".join(self.specs)}`'
```

### Comparing `ReFrame-HPC-4.2.2/reframe/core/builtins.py` & `ReFrame-HPC-4.3.0/reframe/core/builtins.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.2/reframe/core/config.py` & `ReFrame-HPC-4.3.0/reframe/core/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,27 +3,28 @@
 #
 # SPDX-License-Identifier: BSD-3-Clause
 
 import contextlib
 import copy
 import fnmatch
 import functools
+import importlib
 import itertools
 import json
 import jsonschema
 import os
 import re
-import socket
 
 import reframe
 import reframe.core.settings as settings
 import reframe.utility as util
 import reframe.utility.jsonext as jsonext
+import reframe.utility.osext as osext
 from reframe.core.environments import normalize_module_list
-from reframe.core.exceptions import ConfigError, ReframeFatalError
+from reframe.core.exceptions import (ConfigError, ReframeFatalError)
 from reframe.core.logging import getlogger
 from reframe.utility import ScopedDict
 
 
 def _match_option(opt, opt_map):
     if isinstance(opt, list):
         opt = '/'.join(opt)
@@ -57,48 +58,23 @@
             return ret
 
         return _get
 
     return _do_normalize
 
 
-def _hostname(use_fqdn, use_xthostname):
-    '''Return hostname'''
-    if use_xthostname:
-        try:
-            xthostname_file = '/etc/xthostname'
-            getlogger().debug(f'Trying {xthostname_file!r}...')
-            with open(xthostname_file) as fp:
-                return fp.read()
-        except OSError as e:
-            '''Log the error and continue to the next method'''
-            getlogger().debug(f'Failed to read {xthostname_file!r}')
-
-    if use_fqdn:
-        getlogger().debug('Using FQDN...')
-        return socket.getfqdn()
-
-    getlogger().debug('Using standard hostname...')
-    return socket.gethostname()
-
-
 class _SiteConfig:
     def __init__(self):
         self._site_config = None
+        self._config_modules = []
         self._sources = []
         self._subconfigs = {}
         self._local_system = None
         self._sticky_options = {}
-        self._autodetect_meth = 'hostname'
-        self._autodetect_opts = {
-            'hostname': {
-                'use_fqdn': False,
-                'use_xthostname': False,
-            }
-        }
+        self._autodetect_methods = []
         self._definitions = {
             'systems': {},
             'partitions': {},
             'environments': {},
             'modes': {}
         }
 
@@ -192,29 +168,30 @@
 
     def update_config(self, config, filename):
         self._sources.append(filename)
         self._update_defs(config, filename)
         nc = copy.deepcopy(config)
         if self._site_config is None:
             self._site_config = nc
-            return self
+            return
 
         mergeable_sections = ('general', 'logging', 'schedulers')
         for sec in nc.keys():
             if sec not in self._site_config:
                 self._site_config[sec] = nc[sec]
             elif sec in mergeable_sections:
                 self._site_config[sec] = self._merge_config_sections(
                     self._site_config[sec], nc[sec]
                 )
             else:
-                if sec == 'systems':
-                    # Systems have to be inserted in the beginning of the list,
-                    # since they are selected by the first matching entry in
-                    # `hostnames`.
+                if sec in ('systems', 'autodetect_methods'):
+                    # Systems have to be inserted in the beginning of the
+                    # list, since they are selected by the first matching
+                    # entry in `hostnames`. Similarly, the autodetection
+                    # methods are tried from left to right.
                     self._site_config[sec] = nc[sec] + self._site_config[sec]
                 else:
                     self._site_config[sec] += nc[sec]
 
     def _pick_config(self):
         if self._local_system:
             return self._subconfigs[self._local_system]
@@ -236,22 +213,16 @@
 
     def __getitem__(self, key):
         return self._pick_config()[key]
 
     def __getattr__(self, attr):
         return getattr(self._pick_config(), attr)
 
-    def set_autodetect_meth(self, method, **opts):
-        self._autodetect_meth = method
-        try:
-            self._autodetect_opts[method].update(opts)
-        except KeyError:
-            raise ConfigError(
-                f'unknown auto-detection method: {method!r}'
-            ) from None
+    def set_autodetect_methods(self, methods):
+        self._site_config['autodetect_methods'] = list(methods)
 
     @property
     def schema(self):
         '''Configuration schema'''
         return self._schema
 
     def add_sticky_option(self, option, value):
@@ -361,64 +332,118 @@
     def load_config_python(self, filename):
         try:
             mod = util.import_module_from_file(filename)
         except ImportError as e:
             # import_module_from_file() may raise an ImportError if the
             # configuration file is under ReFrame's top-level directory
             raise ConfigError(
-                f"could not load Python configuration file: '{filename}'"
+                f'could not load Python configuration file: {filename!r}'
             ) from e
 
-        if hasattr(mod, 'settings'):
-            # Looks like an old style config
-            raise ConfigError(
-                f"the syntax of the configuration file {filename!r} "
-                f"is no longer supported"
-            )
-
-        mod = util.import_module_from_file(filename)
         if not hasattr(mod, 'site_configuration'):
             raise ConfigError(
                 f"not a valid Python configuration file: '{filename}'"
             )
 
+        self._config_modules.append(mod)
         self.update_config(mod.site_configuration, filename)
 
     def load_config_json(self, filename):
         with open(filename) as fp:
             try:
                 config = json.loads(fp.read())
             except json.JSONDecodeError as e:
                 raise ConfigError(
                     f"invalid JSON syntax in configuration file '{filename}'"
                 ) from e
 
         self.update_config(config, filename)
 
-    def _detect_system(self):
-        getlogger().debug(
-            f'Detecting system using method: {self._autodetect_meth!r}'
-        )
-        hostname = _hostname(
-            self._autodetect_opts[self._autodetect_meth]['use_fqdn'],
-            self._autodetect_opts[self._autodetect_meth]['use_xthostname'],
+    def _setup_autodect_methods(self):
+        def _py_meth(m):
+            try:
+                module, symbol = m.rsplit('.', maxsplit=1)
+            except ValueError:
+                # Not enough values to unpack; we assume a single symbol
+                module, symbol = None, m
+
+            try:
+                if module:
+                    mod = importlib.import_module(module)
+                    return getattr(mod, symbol)
+
+                if not self._config_modules:
+                    raise ConfigError(
+                        f'no module context for requested symbol: {symbol!r}'
+                    )
+
+                # Symbol is local to one of the config files; try to resolve
+                # it in reverse order
+                for mod in reversed(self._config_modules):
+                    if hasattr(mod, symbol):
+                        return getattr(mod, symbol)
+
+                raise ConfigError(f'symbol {symbol!r} is not defined in '
+                                  f'any of the loaded configuration files')
+            except (AttributeError, ImportError, ConfigError) as e:
+                getlogger().warning(f"ignoring autodetection method 'py::{m}' "
+                                    f"due to errors: {e}")
+
+        def _sh_meth(m):
+            def _fn():
+                completed = osext.run_command(m, check=True)
+                return completed.stdout.strip()
+
+            return _fn
+
+        methods = self._site_config.get(
+            'autodetect_methods',
+            self._schema['defaults']['autodetect_methods']
         )
+        for m in methods:
+            if m.startswith('py::'):
+                fn = _py_meth(m.lstrip('py::'))
+                if fn is not None:
+                    self._autodetect_methods.append((m, fn))
+            else:
+                self._autodetect_methods.append((m, _sh_meth(m)))
+
+    def _detect_system(self):
+        getlogger().debug('Autodetecting system')
+        if not self._autodetect_methods:
+            self._setup_autodect_methods()
+
+        hostname = None
+        for meth, fn in self._autodetect_methods:
+            getlogger().debug(f'Trying autodetection method: {meth!r}')
+            try:
+                hostname = fn()
+            except Exception as e:
+                getlogger().debug(f'Autodetection method {meth!r} failed: {e}')
+            else:
+                break
+
+        if hostname is None:
+            raise ConfigError('all autodetection methods failed; '
+                              'try passing a system name explicitly using '
+                              'the `--system` option')
+
         getlogger().debug(f'Retrieved hostname: {hostname!r}')
         getlogger().debug(f'Looking for a matching configuration entry')
         for system in self._site_config['systems']:
             for patt in system['hostnames']:
                 if re.match(patt, hostname):
                     sysname = system['name']
                     getlogger().debug(
                         f'Configuration found: picking system {sysname!r}'
                     )
                     return sysname
 
-        raise ConfigError(f"could not find a configuration entry "
-                          f"for the current system: '{hostname}'")
+        raise ConfigError(f'could not find a configuration entry '
+                          f'for the current system: {hostname!r}')
 
     def validate(self):
         site_config = self._pick_config()
         try:
             jsonschema.validate(site_config, self._schema)
         except jsonschema.ValidationError as e:
             raise ConfigError(f"could not validate configuration files: "
@@ -506,16 +531,16 @@
                 f"for the requested system/partition combination: "
                 f"'{system_name}:{part_name}'"
             )
 
         # Create local configuration for the current or the requested system
         local_config['systems'] = systems
         for name, section in site_config.items():
-            if name == 'systems':
-                # The systems sections has already been treated
+            if name in ('systems', 'autodetect_methods'):
+                # These sections have already been treated
                 continue
 
             # Convert section to a scoped dict that will handle correctly and
             # transparently the system/partition resolution
             scoped_section = ScopedDict()
             unnamed_objects = False
             for obj in section:
@@ -622,18 +647,22 @@
                 res.append(f)
 
     return res
 
 
 def load_config(*filenames):
     ret = _SiteConfig()
-    getlogger().debug('Loading the generic configuration')
+    getlogger().debug('Loading the builtin configuration')
     ret.update_config(settings.site_configuration, '<builtin>')
     for f in filenames:
-        getlogger().debug(f'Loading configuration file: {filenames!r}')
+        if f == '<builtin>':
+            # The builtin configuration is always loaded at the beginning
+            continue
+
+        getlogger().debug(f'Loading configuration file: {f!r}')
         _, ext = os.path.splitext(f)
         if ext == '.py':
             ret.load_config_python(f)
         elif ext == '.json':
             ret.load_config_json(f)
         else:
             raise ConfigError(f"unknown configuration file type: '{f}'")
```

### Comparing `ReFrame-HPC-4.2.2/reframe/core/containers.py` & `ReFrame-HPC-4.3.0/reframe/core/containers.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.2/reframe/core/decorators.py` & `ReFrame-HPC-4.3.0/reframe/core/decorators.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.2/reframe/core/deferrable.py` & `ReFrame-HPC-4.3.0/reframe/core/deferrable.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.2/reframe/core/environments.py` & `ReFrame-HPC-4.3.0/reframe/core/environments.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     to be set when this environment is loaded by the framework.
 
     .. warning::
        Users may not create :class:`Environment` objects directly.
     '''
 
     def __init__(self, name, modules=None, env_vars=None,
-                 extras=None, features=None):
+                 extras=None, features=None, prepare_cmds=None):
         modules = modules or []
         env_vars = env_vars or []
         self._name = name
         self._modules = normalize_module_list(modules)
         self._module_names = [m['name'] for m in self._modules]
 
         # Convert values of env_vars to strings before storing
@@ -52,14 +52,15 @@
 
         self._env_vars = collections.OrderedDict()
         for k, v in env_vars:
             self._env_vars[k] = str(v)
 
         self._extras = extras or {}
         self._features = features or []
+        self._prepare_cmds = prepare_cmds or []
 
     @property
     def name(self):
         '''The name of this environment.
 
         :type: :class:`str`
         '''
@@ -131,14 +132,24 @@
 
         .. versionadded:: 3.11.0
 
         :type: :class:`List[str]`
         '''
         return self._features
 
+    @property
+    def prepare_cmds(self):
+        '''The prepare commands associated with this environment.
+
+        .. versionadded:: 4.3.0
+
+        :type: :class:`List[str]`
+        '''
+        return util.SequenceView(self._prepare_cmds)
+
     def __eq__(self, other):
         if not isinstance(other, type(self)):
             return NotImplemented
 
         if (self.name != other.name or
             set(self.modules) != set(other.modules)):
             return False
@@ -216,25 +227,27 @@
 
     def __init__(self,
                  name,
                  modules=None,
                  env_vars=None,
                  extras=None,
                  features=None,
+                 prepare_cmds=None,
                  cc='cc',
                  cxx='CC',
                  ftn='ftn',
                  nvcc='nvcc',
                  cppflags=None,
                  cflags=None,
                  cxxflags=None,
                  fflags=None,
                  ldflags=None,
                  **kwargs):
-        super().__init__(name, modules, env_vars, extras, features)
+        super().__init__(name, modules, env_vars, extras, features,
+                         prepare_cmds)
         self._cc = cc
         self._cxx = cxx
         self._ftn = ftn
         self._nvcc = nvcc
         self._cppflags = cppflags or []
         self._cflags   = cflags   or []
         self._cxxflags = cxxflags or []
```

### Comparing `ReFrame-HPC-4.2.2/reframe/core/exceptions.py` & `ReFrame-HPC-4.3.0/reframe/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.2/reframe/core/fields.py` & `ReFrame-HPC-4.3.0/reframe/core/fields.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.2/reframe/core/fixtures.py` & `ReFrame-HPC-4.3.0/reframe/core/fixtures.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.2/reframe/core/hooks.py` & `ReFrame-HPC-4.3.0/reframe/core/hooks.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.2/reframe/core/launchers/__init__.py` & `ReFrame-HPC-4.3.0/reframe/core/launchers/__init__.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.2/reframe/core/launchers/local.py` & `ReFrame-HPC-4.3.0/reframe/core/launchers/local.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.2/reframe/core/launchers/mpi.py` & `ReFrame-HPC-4.3.0/reframe/core/launchers/mpi.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.2/reframe/core/logging.py` & `ReFrame-HPC-4.3.0/reframe/core/logging.py`

 * *Files 4% similar despite different names*

```diff
@@ -124,36 +124,71 @@
 
     return ignore_brokenpipe
 
 
 logging.Handler.handleError = handleError(logging.Handler.handleError)
 
 
+def _expand_params(check):
+    cls = type(check)
+    return {
+        name: getattr(check, name) for name, param in cls.param_space.items
+        if param.is_loggable()
+    }
+
+
+def _guess_delim(s):
+    '''Guess the delimiter in the given logging format string'''
+    delims = set()
+    for m in re.finditer(r'\%\((.*?)\)s(.)?', s):
+        d = m.group(2)
+        if d:
+            delims.add(d)
+
+    if len(delims) == 1:
+        return delims.pop()
+    else:
+        return '|'
+
+
 class MultiFileHandler(logging.FileHandler):
     '''A file handler that allows writing on different log files based on
     information from the log record.
     '''
 
-    def __init__(self, prefix, mode='a', encoding=None, fmt=None, perffmt=None):
+    def __init__(self, prefix, mode='a', encoding=None, fmt=None,
+                 perffmt=None, ignore_keys=None):
         super().__init__(prefix, mode, encoding, delay=True)
 
         # Reset FileHandler's filename
         self.baseFilename = None
         self._prefix = prefix
 
         # Associates filenames with open streams
         self.__streams = {}
 
         # Format specifiers
         self.__fmt = fmt
         self.__perffmt = perffmt
         self.__attr_patt = re.compile(r'\%\((.*?)\)s(.)?')
+        self.__ignore_keys = set(ignore_keys) if ignore_keys else set()
 
     def __generate_header(self, record):
         # Generate the header from the record and fmt
+
+        # Expand the special check_#ALL specifier
+        if '%(check_#ALL)s' in self.__fmt:
+            delim = _guess_delim(self.__fmt)
+            self.__fmt = self.__fmt.replace(
+                '%(check_#ALL)s',
+                delim.join(f'%({x})s'
+                           for x in sorted(record.__rfm_loggable_attrs__)
+                           if x not in self.__ignore_keys)
+            )
+
         header = ''
         for m in self.__attr_patt.finditer(self.__fmt):
             attr = m.group(1)
             delim = m.group(2)
             if attr == 'check_perfvalues':
                 # Expand based on the perffmt
                 delim_p = ''
@@ -218,17 +253,16 @@
             os.makedirs(dirname, exist_ok=True)
         except KeyError as e:
             raise LoggingError(f'logging failed: unknown placeholder in '
                                f'filename pattern: {e}') from None
         except OSError as e:
             raise LoggingError('logging failed') from e
 
-        self.baseFilename = os.path.join(
-            dirname, f'{record.__rfm_check__.short_name}.log'
-        )
+        check_basename = type(record.__rfm_check__).variant_name()
+        self.baseFilename = os.path.join(dirname, f'{check_basename}.log')
         self._emit_header(record)
         self.stream = self.__streams[self.baseFilename]
         super().emit(record)
 
     def close(self):
         # Close all open streams
         for s in self.__streams.values():
@@ -259,21 +293,36 @@
 
 
 class CheckFieldFormatter(logging.Formatter):
     '''Log formatter that dynamically looks up format specifiers inside a
     regression test.'''
 
     # NOTE: This formatter will work only for the '%' style
-    def __init__(self, fmt=None, datefmt=None, perffmt=None, style='%'):
+    def __init__(self, fmt=None, datefmt=None, perffmt=None,
+                 ignore_keys=None, style='%'):
         super().__init__(fmt, datefmt, style)
 
         self.__fmt = fmt
         self.__fmtperf = perffmt[:-1] if perffmt else ''
         self.__specs = re.findall(r'\%\((\S+?)\)s', fmt)
         self.__delim = perffmt[-1] if perffmt else ''
+        self.__expand_vars = '%(check_#ALL)s' in self.__fmt
+        self.__expanded = False
+        self.__ignore_keys = set(ignore_keys) if ignore_keys else set()
+
+    def _expand_fmt(self, attrs):
+        if not self.__expand_vars or self.__expanded:
+            return self.__fmt
+
+        delim = _guess_delim(self.__fmt)
+        self.__fmt = self.__fmt.replace(
+            '%(check_#ALL)s', delim.join(f'%({x})s' for x in attrs
+                                         if x not in self.__ignore_keys)
+        )
+        self.__expanded = True
 
     def _format_perf(self, perfvars):
         chunks = []
         for var, info in perfvars.items():
             val, ref, lower, upper, unit = info
             record = {
                 'check_perf_var': var.split(':')[-1],
@@ -288,14 +337,15 @@
             except ValueError:
                 chunks.append("<error formatting the performance record: "
                               "please check the 'format_perfvars' string>")
 
         return self.__delim.join(chunks)
 
     def formatMessage(self, record):
+        self._expand_fmt(sorted(record.__rfm_loggable_attrs__))
         for s in self.__specs:
             if not hasattr(record, s):
                 setattr(record, s, None)
 
         record_proxy = dict(record.__dict__)
         for k, v in record_proxy.items():
             if k == 'check_perfvalues':
@@ -379,16 +429,18 @@
         osext.expandvars(site_config.get(f'{config_prefix}/basedir'))
     ))
     prefix  = osext.expandvars(site_config.get(f'{config_prefix}/prefix'))
     filename_patt = os.path.join(basedir, prefix)
     append = site_config.get(f'{config_prefix}/append')
     format = site_config.get(f'{config_prefix}/format')
     format_perf = site_config.get(f'{config_prefix}/format_perfvars')
+    ignore_keys = site_config.get(f'{config_prefix}/ignore_keys')
     return MultiFileHandler(filename_patt, mode='a+' if append else 'w+',
-                            fmt=format, perffmt=format_perf)
+                            fmt=format, perffmt=format_perf,
+                            ignore_keys=ignore_keys)
 
 
 def _create_syslog_handler(site_config, config_prefix):
     address = site_config.get(f'{config_prefix}/address')
 
     # Check if address is in `host:port` format
     try:
@@ -654,16 +706,18 @@
             # Should not enter here
             raise AssertionError(f'unknown handler type: {handler_type}')
 
         level = site_config.get(f'{handler_prefix}/{i}/level')
         fmt = site_config.get(f'{handler_prefix}/{i}/format')
         datefmt = site_config.get(f'{handler_prefix}/{i}/datefmt')
         perffmt = site_config.get(f'{handler_prefix}/{i}/format_perfvars')
+        ignore_keys = site_config.get(f'{handler_prefix}/{i}/ignore_keys')
         hdlr.setFormatter(RFC3339Formatter(fmt=fmt,
-                                           datefmt=datefmt, perffmt=perffmt))
+                                           datefmt=datefmt, perffmt=perffmt,
+                                           ignore_keys=ignore_keys))
         hdlr.setLevel(_check_level(level))
         hdlr._rfm_type = handler_type
         handlers.append(hdlr)
 
     return handlers
 
 
@@ -729,14 +783,15 @@
     def __init__(self, logger=None, check=None):
         super().__init__(
             logger,
             {
                 # Here we only set the format specifiers that do not
                 # correspond directly to check attributes
                 '__rfm_check__': check,
+                '__rfm_loggable_attrs__': [],
                 'check_name': 'reframe',
                 'check_jobid': None,
                 'check_job_completion_time': None,
                 'check_job_completion_time_unix': None,
                 'check_info': 'reframe',
                 'check_system': None,
                 'check_partition': None,
@@ -782,15 +837,17 @@
                 # we set the value to None
                 val = getattr(self.check, attr, None)
 
             if attr in check_type.raw_params:
                 # Attribute is parameter, so format it
                 val = check_type.raw_params[attr].format(val)
 
-            self.extra[f'check_{extra_name}'] = val
+            key = f'check_{extra_name}'
+            self.extra['__rfm_loggable_attrs__'].append(key)
+            self.extra[key] = val
 
         # Add special extras
         self.extra['check_info'] = self.check.info()
         self.extra['check_job_completion_time'] = _format_time_rfc3339(
             time.localtime(self.extra['check_job_completion_time_unix']),
             '%FT%T%:z'
         )
```

### Comparing `ReFrame-HPC-4.2.2/reframe/core/meta.py` & `ReFrame-HPC-4.3.0/reframe/core/meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -932,28 +932,26 @@
     .. versionadded:: 4.2
        Added the ``module`` argument.
 
     '''
     namespace = RegressionTestMeta.__prepare__(name, bases, **kwargs)
     methods = methods or []
 
-    # Add methods to the body
-    for m in methods:
-        body[m.__name__] = m
+    # Update the namespace with the body elements
+    #
+    # NOTE: We do not use `update()` here so as to force the `__setitem__`
+    # logic
+    for k, v in body.items():
+        namespace[k] = v
 
-    # We update the namespace with the body of the class and we explicitly
-    # call reset on each namespace key to trigger the functionality of
-    # `__setitem__()` as if the body elements were actually being typed in the
-    # class definition
-    namespace.update(body)
-    for k in list(namespace.keys()):
-        namespace.reset(k)
+    # Add methods to the namespace
+    for m in methods:
+        namespace[m.__name__] = m
 
     cls = RegressionTestMeta(name, bases, namespace, **kwargs)
-
     if not module:
         # Set the test's module to be that of our callers
         caller = inspect.currentframe().f_back
         module = caller.f_globals['__name__']
 
     cls.__module__ = module
     return cls
```

### Comparing `ReFrame-HPC-4.2.2/reframe/core/modules.py` & `ReFrame-HPC-4.3.0/reframe/core/modules.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.2/reframe/core/namespaces.py` & `ReFrame-HPC-4.3.0/reframe/core/namespaces.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.2/reframe/core/parameters.py` & `ReFrame-HPC-4.3.0/reframe/core/parameters.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.2/reframe/core/pipeline.py` & `ReFrame-HPC-4.3.0/reframe/core/pipeline.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.2/reframe/core/runtime.py` & `ReFrame-HPC-4.3.0/reframe/core/runtime.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 #
 # Handling of the current host context
 #
 
 import os
 import functools
-from datetime import datetime
+import time
 
 import reframe.core.config as config
 import reframe.utility.osext as osext
 from reframe.core.environments import (Environment, snapshot)
 from reframe.core.exceptions import ReframeFatalError
 from reframe.core.logging import getlogger
 from reframe.core.systems import System
@@ -27,15 +27,15 @@
     .. versionadded:: 2.13
     '''
 
     def __init__(self, site_config):
         self._site_config = site_config
         self._system = System.create(site_config)
         self._current_run = 0
-        self._timestamp = datetime.now()
+        self._timestamp = time.localtime()
 
     def _makedir(self, *dirs, wipeout=False):
         ret = os.path.join(*dirs)
         if wipeout:
             osext.rmtree(ret, ignore_errors=True)
 
         os.makedirs(ret, exist_ok=True)
@@ -107,15 +107,15 @@
         return osext.expandvars(
             self.site_config.get(f'logging/0/handlers_perflog/{i}/basedir')
         )
 
     @property
     def timestamp(self):
         timefmt = self.site_config.get('general/0/timestamp_dirs')
-        return self._timestamp.strftime(timefmt)
+        return time.strftime(timefmt, self._timestamp)
 
     @property
     def output_prefix(self):
         '''The output directory prefix.
 
         :type: :class:`str`
         '''
@@ -238,14 +238,17 @@
 
         return commands
 
     modules_system = runtime().modules_system
     env_snapshot = snapshot()
     commands = []
     for env in environs:
+        for cmd in env.prepare_cmds:
+            commands.append(cmd)
+
         for mod in env.modules_detailed:
             if runtime().get_option('general/0/resolve_module_conflicts'):
                 commands += _load_cmds_tracked(**mod)
             else:
                 commands += modules_system.emit_load_commands(**mod)
 
         for k, v in env.env_vars.items():
```

### Comparing `ReFrame-HPC-4.2.2/reframe/core/schedulers/__init__.py` & `ReFrame-HPC-4.3.0/reframe/core/schedulers/__init__.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.2/reframe/core/schedulers/flux.py` & `ReFrame-HPC-4.3.0/reframe/core/schedulers/flux.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.2/reframe/core/schedulers/local.py` & `ReFrame-HPC-4.3.0/reframe/core/schedulers/local.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import signal
 import socket
 import time
 
 import reframe.core.schedulers as sched
 import reframe.utility.osext as osext
 from reframe.core.backends import register_scheduler
-from reframe.core.exceptions import ReframeError
+from reframe.core.exceptions import JobError, ReframeError
 
 
 class _TimeoutExpired(ReframeError):
     pass
 
 
 class _LocalJob(sched.Job):
@@ -183,17 +183,20 @@
             self._kill_all(job)
             return
 
         if not pid:
             # Job has not finished; check if we have reached a timeout
             t_elapsed = time.time() - job.submit_time
             if job.time_limit and t_elapsed > job.time_limit:
-                self.log(f'Job {job.jobid} timed out; kill it')
                 self._kill_all(job)
                 job._state = 'TIMEOUT'
+                job._exception = JobError(
+                    f'job timed out ({t_elapsed:.6f}s > {job.time_limit}s)',
+                    job.jobid
+                )
 
             return
 
         # Job has finished; kill the whole session
         self._kill_all(job)
 
         # Retrieve the status of the job and return
```

### Comparing `ReFrame-HPC-4.2.2/reframe/core/schedulers/lsf.py` & `ReFrame-HPC-4.3.0/reframe/core/schedulers/lsf.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.2/reframe/core/schedulers/oar.py` & `ReFrame-HPC-4.3.0/reframe/core/schedulers/oar.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.2/reframe/core/schedulers/pbs.py` & `ReFrame-HPC-4.3.0/reframe/core/schedulers/pbs.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.2/reframe/core/schedulers/registry.py` & `ReFrame-HPC-4.3.0/reframe/core/schedulers/registry.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.2/reframe/core/schedulers/sge.py` & `ReFrame-HPC-4.3.0/reframe/core/schedulers/sge.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.2/reframe/core/schedulers/slurm.py` & `ReFrame-HPC-4.3.0/reframe/core/schedulers/slurm.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.2/reframe/core/shell.py` & `ReFrame-HPC-4.3.0/reframe/core/shell.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.2/reframe/core/systems.py` & `ReFrame-HPC-4.3.0/reframe/core/systems.py`

 * *Files 1% similar despite different names*

```diff
@@ -527,14 +527,17 @@
             part_environs = [
                 ProgEnvironment(
                     name=e,
                     modules=site_config.get(f'environments/@{e}/modules'),
                     env_vars=site_config.get(f'environments/@{e}/env_vars'),
                     extras=site_config.get(f'environments/@{e}/extras'),
                     features=site_config.get(f'environments/@{e}/features'),
+                    prepare_cmds=site_config.get(
+                        f'environments/@{e}/prepare_cmds'
+                    ),
                     cc=site_config.get(f'environments/@{e}/cc'),
                     cxx=site_config.get(f'environments/@{e}/cxx'),
                     ftn=site_config.get(f'environments/@{e}/ftn'),
                     cppflags=site_config.get(f'environments/@{e}/cppflags'),
                     cflags=site_config.get(f'environments/@{e}/cflags'),
                     cxxflags=site_config.get(f'environments/@{e}/cxxflags'),
                     fflags=site_config.get(f'environments/@{e}/fflags'),
```

### Comparing `ReFrame-HPC-4.2.2/reframe/core/variables.py` & `ReFrame-HPC-4.3.0/reframe/core/variables.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.2/reframe/core/warnings.py` & `ReFrame-HPC-4.3.0/reframe/core/warnings.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.2/reframe/frontend/argparse.py` & `ReFrame-HPC-4.3.0/reframe/frontend/argparse.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.2/reframe/frontend/autodetect.py` & `ReFrame-HPC-4.3.0/reframe/frontend/autodetect.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.2/reframe/frontend/ci.py` & `ReFrame-HPC-4.3.0/reframe/frontend/ci.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.2/reframe/frontend/cli.py` & `ReFrame-HPC-4.3.0/reframe/frontend/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 import random
 import shlex
 import socket
 import sys
 import time
 import traceback
 
-import reframe
 import reframe.core.config as config
 import reframe.core.exceptions as errors
 import reframe.core.logging as logging
 import reframe.core.runtime as runtime
 import reframe.frontend.argparse as argparse
 import reframe.frontend.autodetect as autodetect
 import reframe.frontend.ci as ci
@@ -27,15 +26,16 @@
 import reframe.frontend.runreport as runreport
 import reframe.utility as util
 import reframe.utility.jsonext as jsonext
 import reframe.utility.osext as osext
 import reframe.utility.typecheck as typ
 
 from reframe.frontend.testgenerators import (distribute_tests,
-                                             getallnodes, repeat_tests)
+                                             getallnodes, repeat_tests,
+                                             parameterize_tests)
 from reframe.frontend.executors.policies import (SerialExecutionPolicy,
                                                  AsynchronousExecutionPolicy)
 from reframe.frontend.executors import Runner, generate_testcases
 from reframe.frontend.loader import RegressionCheckLoader
 from reframe.frontend.printer import PrettyPrinter
 
 
@@ -282,15 +282,15 @@
     )
     output_options.add_argument(
         '--save-log-files', action='store_true', default=False,
         help='Save ReFrame log files to the output directory',
         envvar='RFM_SAVE_LOG_FILES', configvar='general/save_log_files'
     )
     output_options.add_argument(
-        '--timestamp', action='store', nargs='?', const='%FT%T',
+        '--timestamp', action='store', nargs='?', const='%y%m%dT%H%M%S%z',
         metavar='TIMEFMT',
         help=('Append a timestamp to the output and stage directory prefixes '
               '(default: "%%FT%%T")'),
         envvar='RFM_TIMESTAMP_DIRS', configvar='general/timestamp_dirs'
     )
 
     # Check discovery options
@@ -434,14 +434,18 @@
         '--maxfail', metavar='NUM', action='store', default=sys.maxsize,
         help='Exit after first NUM failures', type=int
     )
     run_options.add_argument(
         '--mode', action='store', help='Execution mode to use'
     )
     run_options.add_argument(
+        '-P', '--parameterize', action='append', metavar='VAR:VAL0,VAL1,...',
+        default=[], help='Parameterize a test on a set of variables'
+    )
+    run_options.add_argument(
         '--repeat', action='store', metavar='N',
         help='Repeat selected tests N times'
     )
     run_options.add_argument(
         '--reruns', action='store', metavar='N', default=0,
         help='Rerun the whole test session N times', type=int
     )
@@ -570,32 +574,37 @@
         type=typ.Bool,
         help='Use the full qualified domain name as host name'
     )
     argparser.add_argument(
         dest='autodetect_method',
         envvar='RFM_AUTODETECT_METHOD',
         action='store',
-        default='hostname',
         help='Method to detect the system'
     )
     argparser.add_argument(
-        dest='config_path',
-        envvar='RFM_CONFIG_PATH :',
-        action='append',
-        help='Directories where ReFrame will look for base configuration'
+        dest='autodetect_methods',
+        envvar='RFM_AUTODETECT_METHODS',
+        action='store',
+        help='List of methods for detecting the current system'
     )
     argparser.add_argument(
         dest='autodetect_xthostname',
         envvar='RFM_AUTODETECT_XTHOSTNAME',
         action='store',
         default=False,
         type=typ.Bool,
         help="Use Cray's xthostname file to retrieve the host name"
     )
     argparser.add_argument(
+        dest='config_path',
+        envvar='RFM_CONFIG_PATH :',
+        action='append',
+        help='Directories where ReFrame will look for base configuration'
+    )
+    argparser.add_argument(
         dest='git_timeout',
         envvar='RFM_GIT_TIMEOUT',
         configvar='general/git_timeout',
         action='store',
         help=('Timeout in seconds when checking if the url is a '
               'valid repository.'),
         type=float
@@ -703,17 +712,15 @@
     if len(sys.argv) == 1:
         argparser.print_help()
         sys.exit(1)
 
     # First configure logging with our generic configuration so as to be able
     # to print pretty messages; logging will be reconfigured by user's
     # configuration later
-    site_config = config.load_config(
-        os.path.join(reframe.INSTALL_PREFIX, 'reframe/core/settings.py')
-    )
+    site_config = config.load_config('<builtin>')
     site_config.select_subconfig('generic')
     options.update_config(site_config)
     logging.configure_logging(site_config)
     printer = PrettyPrinter()
     printer.colorize = site_config.get('general/0/colorize')
     if not restrict_logging():
         printer.adjust_verbosity(calc_verbosity(site_config, options.quiet))
@@ -735,19 +742,41 @@
 
         printer.debug('Loading user configuration')
         conf_files = config.find_config_files(
             options.config_path, options.config_files
         )
         site_config = config.load_config(*conf_files)
         site_config.validate()
-        site_config.set_autodetect_meth(
-            options.autodetect_method,
-            use_fqdn=options.autodetect_fqdn,
-            use_xthostname=options.autodetect_xthostname
-        )
+
+        if options.autodetect_method:
+            printer.warning('RFM_AUTODETECT_METHOD is deprecated; '
+                            'please use RFM_AUTODETECT_METHODS instead')
+
+        autodetect_methods = []
+        if options.autodetect_methods:
+            autodetect_methods = options.autodetect_methods.split(',')
+        else:
+            if options.autodetect_fqdn:
+                printer.warning(
+                    'RFM_AUTODETECT_FQDN is deprecated; '
+                    'please use RFM_AUTODETECT_METHODS=py::socket.getfqdn '
+                    'instead'
+                )
+                autodetect_methods = ['py::socket.getfqdn']
+            elif options.autodetect_xthostname:
+                printer.warning(
+                    "RFM_AUTODETECT_XTHOSTNAME is deprecated; "
+                    "please use RFM_AUTODETECT_METHODS='cat /etc/xthostname,hostname' "  # noqa: E501
+                    "instead"
+                )
+                autodetect_methods = ['cat /etc/xthostname',
+                                      'py::socket.gethostname']
+
+        if autodetect_methods:
+            site_config.set_autodetect_methods(autodetect_methods)
 
         # We ignore errors about unresolved sections or configuration
         # parameters here, because they might be defined at the individual
         # partition level and will be caught when we will instantiating
         # internally the system and partitions later on.
         site_config.select_subconfig(options.system,
                                      ignore_resolve_errors=True)
@@ -1068,14 +1097,30 @@
 
             testcases = list(filter(_case_failed, testcases))
             printer.verbose(
                 f'Filtering successful test case(s): '
                 f'{len(testcases)} remaining'
             )
 
+        if options.parameterize:
+            # Prepare parameters
+            params = {}
+            for param_spec in options.parameterize:
+                try:
+                    var, values_spec = param_spec.split('=')
+                except ValueError:
+                    raise errors.CommandLineError(
+                        f'invalid parameter spec: {param_spec}'
+                    ) from None
+                else:
+                    params[var] = values_spec.split(',')
+
+            testcases_all = parameterize_tests(testcases, params)
+            testcases = testcases_all
+
         if options.repeat is not None:
             try:
                 num_repeats = int(options.repeat)
                 if num_repeats <= 0:
                     raise ValueError
             except ValueError:
                 raise errors.CommandLineError(
```

### Comparing `ReFrame-HPC-4.2.2/reframe/frontend/dependencies.py` & `ReFrame-HPC-4.3.0/reframe/frontend/dependencies.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.2/reframe/frontend/executors/__init__.py` & `ReFrame-HPC-4.3.0/reframe/frontend/executors/__init__.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.2/reframe/frontend/executors/policies.py` & `ReFrame-HPC-4.3.0/reframe/frontend/executors/policies.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.2/reframe/frontend/filters.py` & `ReFrame-HPC-4.3.0/reframe/frontend/filters.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.2/reframe/frontend/loader.py` & `ReFrame-HPC-4.3.0/reframe/frontend/loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,27 +16,14 @@
 
 import reframe.utility as util
 import reframe.utility.osext as osext
 from reframe.core.exceptions import NameConflictError, is_severe, what
 from reframe.core.logging import getlogger, time_function
 
 
-class temp_sys_path:
-    def __init__(self, path):
-        self._path = path
-        self._pos = None
-
-    def __enter__(self):
-        self._pos = len(sys.path)
-        sys.path.append(self._path)
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        sys.path.pop(self._pos)
-
-
 class no_op:
     def __enter__(self):
         pass
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         pass
 
@@ -202,15 +189,15 @@
         filename = os.path.abspath(filename)
         if not self._validate_source(filename):
             return []
 
         try:
             dirname = os.path.dirname(filename)
             with osext.change_dir(dirname):
-                with temp_sys_path(dirname):
+                with util.temp_sys_path(dirname):
                     return self.load_from_module(
                         util.import_module_from_file(filename, force)
                     )
         except Exception:
             exc_info = sys.exc_info()
             if not is_severe(*exc_info):
                 # Simply skip the file in this case
```

### Comparing `ReFrame-HPC-4.2.2/reframe/frontend/printer.py` & `ReFrame-HPC-4.3.0/reframe/frontend/printer.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.2/reframe/frontend/runreport.py` & `ReFrame-HPC-4.3.0/reframe/frontend/runreport.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.2/reframe/frontend/statistics.py` & `ReFrame-HPC-4.3.0/reframe/frontend/statistics.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.2/reframe/frontend/testgenerators.py` & `ReFrame-HPC-4.3.0/reframe/frontend/testgenerators.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 
 import reframe.core.builtins as builtins
 import reframe.core.runtime as runtime
 import reframe.utility as util
 
 from reframe.core.decorators import TestRegistry
+from reframe.core.fields import make_convertible
 from reframe.core.logging import getlogger, time_function
 from reframe.core.meta import make_test
 from reframe.core.schedulers import Job
 from reframe.frontend.executors import generate_testcases
 
 
 @time_function
@@ -44,44 +45,15 @@
             )
 
         nodes[part.fullname] = [n.name for n in available_nodes]
 
     return nodes
 
 
-def _rfm_pin_run_nodes(obj):
-    nodelist = getattr(obj, '$nid')
-    if not obj.local:
-        obj.job.pin_nodes = nodelist
-
-
-def _rfm_pin_build_nodes(obj):
-    pin_nodes = getattr(obj, '$nid')
-    if not obj.local and not obj.build_locally:
-        obj.build_job.pin_nodes = pin_nodes
-
-
-def make_valid_systems_hook(systems):
-    '''Returns a function to be used as a hook that sets the
-    valid systems.
-
-    Since valid_systems change for each generated test, we need to
-    generate different post-init hooks for each one of them.
-    '''
-    def _rfm_set_valid_systems(obj):
-        obj.valid_systems = systems
-
-    return _rfm_set_valid_systems
-
-
-@time_function
-def distribute_tests(testcases, node_map):
-    '''Returns new testcases that will be parameterized to run in node of
-    their partitions based on the nodemap
-    '''
+def _generate_tests(testcases, gen_fn):
     tmp_registry = TestRegistry()
 
     # We don't want to register the same check for every environment
     # per partition
     check_part_combs = set()
     for tc in testcases:
         check, partition, _ = tc
@@ -90,73 +62,122 @@
             continue
 
         check_part_combs.add(candidate_comb)
         cls = type(check)
         variant_info = cls.get_variant_info(
             check.variant_num, recurse=True
         )
-        nc = make_test(
+        nc, params = gen_fn(tc)
+        nc._rfm_custom_prefix = check.prefix
+        for i in range(nc.num_variants):
+            # Check if this variant should be instantiated
+            vinfo = nc.get_variant_info(i, recurse=True)
+            for p in params:
+                vinfo['params'].pop(p)
+
+            if vinfo == variant_info:
+                tmp_registry.add(nc, variant_num=i)
+
+    new_checks = tmp_registry.instantiate_all()
+    return generate_testcases(new_checks)
+
+
+@time_function
+def distribute_tests(testcases, node_map):
+    def _rfm_pin_run_nodes(obj):
+        nodelist = getattr(obj, '$nid')
+        if not obj.local:
+            obj.job.pin_nodes = nodelist
+
+    def _rfm_pin_build_nodes(obj):
+        pin_nodes = getattr(obj, '$nid')
+        if not obj.local and not obj.build_locally:
+            obj.build_job.pin_nodes = pin_nodes
+
+    def _make_dist_test(testcase):
+        check, partition, _ = testcase
+        cls = type(check)
+
+        def _rfm_set_valid_systems(obj):
+            obj.valid_systems = [partition.fullname]
+
+        return make_test(
             f'{cls.__name__}_{partition.fullname.replace(":", "_")}',
             (cls,),
             {
                 'valid_systems': [partition.fullname],
                 '$nid': builtins.parameter(
                     [[n] for n in node_map[partition.fullname]],
                     fmt=util.nodelist_abbrev
                 )
             },
             methods=[
                 builtins.run_before('run')(_rfm_pin_run_nodes),
                 builtins.run_before('compile')(_rfm_pin_build_nodes),
                 # We re-set the valid system in a hook to make sure that it
-                # will not be overwriten by a parent post-init hook
-                builtins.run_after('init')(
-                    make_valid_systems_hook([partition.fullname])
-                ),
+                # will not be overwritten by a parent post-init hook
+                builtins.run_after('init')(_rfm_set_valid_systems),
             ]
-        )
+        ), ['$nid']
 
-        # We have to set the prefix manually
-        nc._rfm_custom_prefix = check.prefix
-        for i in range(nc.num_variants):
-            # Check if this variant should be instantiated
-            vinfo = nc.get_variant_info(i, recurse=True)
-            vinfo['params'].pop('$nid')
-            if vinfo == variant_info:
-                tmp_registry.add(nc, variant_num=i)
-
-    new_checks = tmp_registry.instantiate_all()
-    return generate_testcases(new_checks)
+    return _generate_tests(testcases, _make_dist_test)
 
 
 @time_function
 def repeat_tests(testcases, num_repeats):
     '''Returns new test cases parameterized over their repetition number'''
 
-    tmp_registry = TestRegistry()
-    unique_checks = set()
-    for tc in testcases:
-        check = tc.check
-        if check.is_fixture() or check in unique_checks:
-            continue
-
-        unique_checks.add(check)
-        cls = type(check)
-        variant_info = cls.get_variant_info(
-            check.variant_num, recurse=True
-        )
-        nc = make_test(
+    def _make_repeat_test(testcase):
+        cls = type(testcase.check)
+        return make_test(
             f'{cls.__name__}', (cls,),
             {
                 '$repeat_no': builtins.parameter(range(num_repeats))
             }
-        )
-        nc._rfm_custom_prefix = check.prefix
-        for i in range(nc.num_variants):
-            # Check if this variant should be instantiated
-            vinfo = nc.get_variant_info(i, recurse=True)
-            vinfo['params'].pop('$repeat_no')
-            if vinfo == variant_info:
-                tmp_registry.add(nc, variant_num=i)
+        ), ['$repeat_no']
 
-    new_checks = tmp_registry.instantiate_all()
-    return generate_testcases(new_checks)
+    return _generate_tests(testcases, _make_repeat_test)
+
+
+@time_function
+def parameterize_tests(testcases, paramvars):
+    '''Returns new test cases parameterized over specific variables.'''
+
+    def _make_parameterized_test(testcase):
+        check = testcase.check
+        cls = type(check)
+
+        # Check that all the requested variables exist
+        body = {}
+        for var, values in paramvars.items():
+            var_parts = var.split('.')
+            if len(var_parts) == 1:
+                var = var_parts[0]
+            elif len(var_parts) == 2:
+                var_check, var = var_parts
+                if var_check != cls.__name__:
+                    continue
+            else:
+                getlogger().warning(f'cannot set a variable in a fixture')
+                continue
+
+            if not var in cls.var_space:
+                getlogger().warning(
+                    f'variable {var!r} not defined for test '
+                    f'{check.display_name!r}; ignoring parameterization'
+                )
+                continue
+
+            body[f'${var}'] = builtins.parameter(values)
+
+        def _set_vars(self):
+            for var in body.keys():
+                setattr(self, var[1:],
+                        make_convertible(getattr(self, f'{var}')))
+
+        return make_test(
+            f'{cls.__name__}', (cls,),
+            body=body,
+            methods=[builtins.run_after('init')(_set_vars)]
+        ), body.keys()
+
+    return _generate_tests(testcases, _make_parameterized_test)
```

### Comparing `ReFrame-HPC-4.2.2/reframe/schemas/config.json` & `ReFrame-HPC-4.3.0/reframe/schemas/config.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.989618261222313%*

 * *Differences: {"'defaults'": "{'autodetect_methods': ['py::socket.gethostname'], "*

 * *               "'logging/handlers_perflog/filelog_ignore_keys': []}",*

 * * "'defs'": "{'filelog_handler': {'allOf': {1: {'properties': {'ignore_keys': OrderedDict([('type', "*

 * *           "'array'), ('items', OrderedDict([('type', 'string')]))])}}}}}",*

 * * "'properties'": "{'environments': {'items': {'properties': {'prepare_cmds': OrderedDict([('type', "*

 * *                 "'array'), ('items', OrderedDict([('type', 'string')]))])}}}, "*

 * *               […]*

```diff
@@ -1,12 +1,15 @@
 {
     "$id": "https://raw.githubusercontent.com/reframe-hpc/reframe/master/reframe/schemas/config.json",
     "$schema": "http://json-schema.org/draft-07/schema#",
     "additionalProperties": false,
     "defaults": {
+        "autodetect_methods": [
+            "py::socket.gethostname"
+        ],
         "environments/cc": "cc",
         "environments/cflags": [],
         "environments/cppflags": [],
         "environments/cxx": "CC",
         "environments/cxxflags": [],
         "environments/env_vars": [],
         "environments/extras": {},
@@ -60,14 +63,15 @@
         "logging/handlers*/file_timestamp": false,
         "logging/handlers*/stream_name": "stdout",
         "logging/handlers*/syslog_facility": "user",
         "logging/handlers*/syslog_socktype": "udp",
         "logging/handlers_perflog": [],
         "logging/handlers_perflog/filelog_append": true,
         "logging/handlers_perflog/filelog_basedir": "./perflogs",
+        "logging/handlers_perflog/filelog_ignore_keys": [],
         "logging/handlers_perflog/graylog_extras": {},
         "logging/handlers_perflog/httpjson_debug": false,
         "logging/handlers_perflog/httpjson_extra_headers": {},
         "logging/handlers_perflog/httpjson_extras": {},
         "logging/handlers_perflog/httpjson_ignore_keys": [],
         "logging/handlers_perflog/httpjson_json_formatter": null,
         "logging/level": "undefined",
@@ -191,14 +195,20 @@
                     "properties": {
                         "append": {
                             "type": "boolean"
                         },
                         "basedir": {
                             "type": "string"
                         },
+                        "ignore_keys": {
+                            "items": {
+                                "type": "string"
+                            },
+                            "type": "array"
+                        },
                         "prefix": {
                             "type": "string"
                         }
                     },
                     "required": [
                         "prefix"
                     ]
@@ -501,14 +511,20 @@
                     "type": "array"
                 }
             },
             "type": "object"
         }
     },
     "properties": {
+        "autodetect_methods": {
+            "items": {
+                "type": "string"
+            },
+            "type": "array"
+        },
         "environments": {
             "items": {
                 "additionalProperties": false,
                 "properties": {
                     "cc": {
                         "type": "string"
                     },
@@ -565,14 +581,20 @@
                     },
                     "modules": {
                         "$ref": "#/defs/modules_list"
                     },
                     "name": {
                         "$ref": "#/defs/alphanum_ext_string"
                     },
+                    "prepare_cmds": {
+                        "items": {
+                            "type": "string"
+                        },
+                        "type": "array"
+                    },
                     "target_systems": {
                         "$ref": "#/defs/system_ref"
                     },
                     "variables": {
                         "$ref": "#/defs/envvar_list"
                     }
                 },
```

### Comparing `ReFrame-HPC-4.2.2/reframe/schemas/junit.xsd` & `ReFrame-HPC-4.3.0/reframe/schemas/junit.xsd`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.2/reframe/schemas/runreport.json` & `ReFrame-HPC-4.3.0/reframe/schemas/runreport.json`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.2/reframe/utility/__init__.py` & `ReFrame-HPC-4.3.0/reframe/utility/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1058,14 +1058,29 @@
     def __enter__(self):
         setattr(self._obj, self._attr, self._newval)
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         setattr(self._obj, self._attr, self._saved)
 
 
+class temp_sys_path:
+    '''Context manager to temporarily change the py:obj:`sys.path`.'''
+
+    def __init__(self, path):
+        self._path = path
+        self._pos = None
+
+    def __enter__(self):
+        self._pos = len(sys.path)
+        sys.path.append(self._path)
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        sys.path.pop(self._pos)
+
+
 class ScopedDict(UserDict):
     '''This is a special dictionary that imposes scopes on its keys.
 
     When a key is not found, it will be searched up in the scope hierarchy.
     If not found even at the global scope, a :class:`KeyError` will be raised.
 
     A scoped dictionary is initialized using a two-level normal dictionary
```

### Comparing `ReFrame-HPC-4.2.2/reframe/utility/color.py` & `ReFrame-HPC-4.3.0/reframe/utility/color.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.2/reframe/utility/cpuinfo.py` & `ReFrame-HPC-4.3.0/reframe/utility/cpuinfo.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.2/reframe/utility/jsonext.py` & `ReFrame-HPC-4.3.0/reframe/utility/jsonext.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.2/reframe/utility/osext.py` & `ReFrame-HPC-4.3.0/reframe/utility/osext.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.2/reframe/utility/profile.py` & `ReFrame-HPC-4.3.0/reframe/utility/profile.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.2/reframe/utility/sanity.py` & `ReFrame-HPC-4.3.0/reframe/utility/sanity.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.2/reframe/utility/typecheck.py` & `ReFrame-HPC-4.3.0/reframe/utility/typecheck.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.2/reframe/utility/udeps.py` & `ReFrame-HPC-4.3.0/reframe/utility/udeps.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.2/reframe/utility/versioning.py` & `ReFrame-HPC-4.3.0/reframe/utility/versioning.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.2/setup.cfg` & `ReFrame-HPC-4.3.0/setup.cfg`

 * *Files identical despite different names*

