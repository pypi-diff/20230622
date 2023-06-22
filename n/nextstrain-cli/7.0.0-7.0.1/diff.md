# Comparing `tmp/nextstrain-cli-7.0.0.tar.gz` & `tmp/nextstrain-cli-7.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nextstrain-cli-7.0.0.tar", last modified: Fri May 26 20:34:09 2023, max compression
+gzip compressed data, was "nextstrain-cli-7.0.1.tar", last modified: Wed May 31 21:12:37 2023, max compression
```

## Comparing `nextstrain-cli-7.0.0.tar` & `nextstrain-cli-7.0.1.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:34:09.742600 nextstrain-cli-7.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11683 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/LICENSE.cognito-srp
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/LICENSE.sphinx
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-26 20:34:09.742600 nextstrain-cli-7.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:34:09.730600 nextstrain-cli-7.0.0/nextstrain/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:34:09.738600 nextstrain-cli-7.0.0/nextstrain/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7138 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/authn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:34:09.738600 nextstrain-cli-7.0.0/nextstrain/cli/aws/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:34:09.738600 nextstrain-cli-7.0.0/nextstrain/cli/aws/cognito/
--rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/aws/cognito/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11366 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/aws/cognito/srp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:34:09.738600 nextstrain-cli-7.0.0/nextstrain/cli/command/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/command/authorization.py
--rw-r--r--   0 runner    (1001) docker     (123)    10309 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/command/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/command/check_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/command/debugger.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/command/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/command/init_shell.py
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/command/login.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/command/logout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:34:09.738600 nextstrain-cli-7.0.0/nextstrain/cli/command/remote/
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/command/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/command/remote/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/command/remote/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/command/remote/ls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/command/remote/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/command/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/command/shell.py
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/command/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/command/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    15564 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/command/view.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/command/whoami.py
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/console.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/gzip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/hostenv.py
--rw-r--r--   0 runner    (1001) docker     (123)    15241 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:34:09.738600 nextstrain-cli-7.0.0/nextstrain/cli/remote/
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32844 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/remote/nextstrain_dot_org.py
--rw-r--r--   0 runner    (1001) docker     (123)    15474 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/remote/s3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:34:09.738600 nextstrain-cli-7.0.0/nextstrain/cli/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/resources/bashrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:34:09.742600 nextstrain-cli-7.0.0/nextstrain/cli/rst/
--rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/rst/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40176 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/rst/sphinx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:34:09.742600 nextstrain-cli-7.0.0/nextstrain/cli/runner/
--rw-r--r--   0 runner    (1001) docker     (123)     9210 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/runner/ambient.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:34:09.742600 nextstrain-cli-7.0.0/nextstrain/cli/runner/aws_batch/
--rw-r--r--   0 runner    (1001) docker     (123)    12636 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/runner/aws_batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11949 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/runner/aws_batch/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/runner/aws_batch/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6872 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/runner/aws_batch/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)    21276 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/runner/conda.py
--rw-r--r--   0 runner    (1001) docker     (123)    20536 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/runner/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)    17125 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/runner/singularity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    20164 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:34:09.742600 nextstrain-cli-7.0.0/nextstrain_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-26 20:34:09.000000 nextstrain-cli-7.0.0/nextstrain_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-05-26 20:34:09.000000 nextstrain-cli-7.0.0/nextstrain_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 20:34:09.000000 nextstrain-cli-7.0.0/nextstrain_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-26 20:34:09.000000 nextstrain-cli-7.0.0/nextstrain_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-26 20:34:09.000000 nextstrain-cli-7.0.0/nextstrain_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-26 20:34:09.000000 nextstrain-cli-7.0.0/nextstrain_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 20:34:09.742600 nextstrain-cli-7.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:12:37.457996 nextstrain-cli-7.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11683 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/LICENSE.cognito-srp
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/LICENSE.sphinx
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-31 21:12:37.457996 nextstrain-cli-7.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:12:37.437996 nextstrain-cli-7.0.1/nextstrain/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:12:37.445996 nextstrain-cli-7.0.1/nextstrain/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/nextstrain/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/nextstrain/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/nextstrain/cli/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7138 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/nextstrain/cli/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/nextstrain/cli/authn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:12:37.445996 nextstrain-cli-7.0.1/nextstrain/cli/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/nextstrain/cli/aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:12:37.445996 nextstrain-cli-7.0.1/nextstrain/cli/aws/cognito/
+-rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/nextstrain/cli/aws/cognito/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11366 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/nextstrain/cli/aws/cognito/srp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:12:37.449996 nextstrain-cli-7.0.1/nextstrain/cli/command/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/nextstrain/cli/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/nextstrain/cli/command/authorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10309 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/nextstrain/cli/command/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/nextstrain/cli/command/check_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/nextstrain/cli/command/debugger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/nextstrain/cli/command/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/nextstrain/cli/command/init_shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/nextstrain/cli/command/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/nextstrain/cli/command/logout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:12:37.449996 nextstrain-cli-7.0.1/nextstrain/cli/command/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/nextstrain/cli/command/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/nextstrain/cli/command/remote/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/nextstrain/cli/command/remote/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/nextstrain/cli/command/remote/ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/nextstrain/cli/command/remote/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/nextstrain/cli/command/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/nextstrain/cli/command/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/nextstrain/cli/command/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/nextstrain/cli/command/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15564 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/nextstrain/cli/command/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/nextstrain/cli/command/whoami.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/nextstrain/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/nextstrain/cli/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/nextstrain/cli/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/nextstrain/cli/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/nextstrain/cli/gzip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/nextstrain/cli/hostenv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15241 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/nextstrain/cli/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/nextstrain/cli/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:12:37.449996 nextstrain-cli-7.0.1/nextstrain/cli/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/nextstrain/cli/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32844 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/nextstrain/cli/remote/nextstrain_dot_org.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15474 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/nextstrain/cli/remote/s3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:12:37.453996 nextstrain-cli-7.0.1/nextstrain/cli/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/nextstrain/cli/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/nextstrain/cli/resources/bashrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:12:37.453996 nextstrain-cli-7.0.1/nextstrain/cli/rst/
+-rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/nextstrain/cli/rst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40176 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/nextstrain/cli/rst/sphinx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:12:37.453996 nextstrain-cli-7.0.1/nextstrain/cli/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)     9210 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/nextstrain/cli/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/nextstrain/cli/runner/ambient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:12:37.453996 nextstrain-cli-7.0.1/nextstrain/cli/runner/aws_batch/
+-rw-r--r--   0 runner    (1001) docker     (123)    12636 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/nextstrain/cli/runner/aws_batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11949 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/nextstrain/cli/runner/aws_batch/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/nextstrain/cli/runner/aws_batch/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6872 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/nextstrain/cli/runner/aws_batch/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23742 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/nextstrain/cli/runner/conda.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20536 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/nextstrain/cli/runner/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17125 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/nextstrain/cli/runner/singularity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/nextstrain/cli/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20164 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/nextstrain/cli/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/nextstrain/cli/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:12:37.457996 nextstrain-cli-7.0.1/nextstrain_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-31 21:12:37.000000 nextstrain-cli-7.0.1/nextstrain_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-05-31 21:12:37.000000 nextstrain-cli-7.0.1/nextstrain_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 21:12:37.000000 nextstrain-cli-7.0.1/nextstrain_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-31 21:12:37.000000 nextstrain-cli-7.0.1/nextstrain_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-31 21:12:37.000000 nextstrain-cli-7.0.1/nextstrain_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-31 21:12:37.000000 nextstrain-cli-7.0.1/nextstrain_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 21:12:37.457996 nextstrain-cli-7.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-05-31 21:12:20.000000 nextstrain-cli-7.0.1/setup.py
```

### Comparing `nextstrain-cli-7.0.0/LICENSE` & `nextstrain-cli-7.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-7.0.0/LICENSE.cognito-srp` & `nextstrain-cli-7.0.1/LICENSE.cognito-srp`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-7.0.0/LICENSE.sphinx` & `nextstrain-cli-7.0.1/LICENSE.sphinx`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-7.0.0/PKG-INFO` & `nextstrain-cli-7.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextstrain-cli
-Version: 7.0.0
+Version: 7.0.1
 Summary: Nextstrain command-line tool
 Home-page: https://docs.nextstrain.org/projects/cli/
 Author: Thomas Sibley
 Author-email: tsibley@fredhutch.org
 License: MIT
 Project-URL: Bug Reports, https://github.com/nextstrain/cli/issues
 Project-URL: Change Log, https://github.com/nextstrain/cli/blob/master/CHANGES.md
```

### Comparing `nextstrain-cli-7.0.0/README.md` & `nextstrain-cli-7.0.1/README.md`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-7.0.0/nextstrain/cli/__init__.py` & `nextstrain-cli-7.0.1/nextstrain/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-7.0.0/nextstrain/cli/__main__.py` & `nextstrain-cli-7.0.1/nextstrain/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-7.0.0/nextstrain/cli/argparse.py` & `nextstrain-cli-7.0.1/nextstrain/cli/argparse.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-7.0.0/nextstrain/cli/authn.py` & `nextstrain-cli-7.0.1/nextstrain/cli/authn.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-7.0.0/nextstrain/cli/aws/__init__.py` & `nextstrain-cli-7.0.1/nextstrain/cli/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-7.0.0/nextstrain/cli/aws/cognito/__init__.py` & `nextstrain-cli-7.0.1/nextstrain/cli/aws/cognito/__init__.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-7.0.0/nextstrain/cli/aws/cognito/srp.py` & `nextstrain-cli-7.0.1/nextstrain/cli/aws/cognito/srp.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-7.0.0/nextstrain/cli/command/authorization.py` & `nextstrain-cli-7.0.1/nextstrain/cli/command/authorization.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-7.0.0/nextstrain/cli/command/build.py` & `nextstrain-cli-7.0.1/nextstrain/cli/command/build.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-7.0.0/nextstrain/cli/command/check_setup.py` & `nextstrain-cli-7.0.1/nextstrain/cli/command/check_setup.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-7.0.0/nextstrain/cli/command/deploy.py` & `nextstrain-cli-7.0.1/nextstrain/cli/command/deploy.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-7.0.0/nextstrain/cli/command/init_shell.py` & `nextstrain-cli-7.0.1/nextstrain/cli/command/init_shell.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-7.0.0/nextstrain/cli/command/login.py` & `nextstrain-cli-7.0.1/nextstrain/cli/command/login.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-7.0.0/nextstrain/cli/command/remote/__init__.py` & `nextstrain-cli-7.0.1/nextstrain/cli/command/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-7.0.0/nextstrain/cli/command/remote/delete.py` & `nextstrain-cli-7.0.1/nextstrain/cli/command/remote/delete.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-7.0.0/nextstrain/cli/command/remote/download.py` & `nextstrain-cli-7.0.1/nextstrain/cli/command/remote/download.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-7.0.0/nextstrain/cli/command/remote/ls.py` & `nextstrain-cli-7.0.1/nextstrain/cli/command/remote/ls.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-7.0.0/nextstrain/cli/command/remote/upload.py` & `nextstrain-cli-7.0.1/nextstrain/cli/command/remote/upload.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-7.0.0/nextstrain/cli/command/setup.py` & `nextstrain-cli-7.0.1/nextstrain/cli/command/setup.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-7.0.0/nextstrain/cli/command/shell.py` & `nextstrain-cli-7.0.1/nextstrain/cli/command/shell.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-7.0.0/nextstrain/cli/command/update.py` & `nextstrain-cli-7.0.1/nextstrain/cli/command/update.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-7.0.0/nextstrain/cli/command/version.py` & `nextstrain-cli-7.0.1/nextstrain/cli/command/version.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-7.0.0/nextstrain/cli/command/view.py` & `nextstrain-cli-7.0.1/nextstrain/cli/command/view.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-7.0.0/nextstrain/cli/command/whoami.py` & `nextstrain-cli-7.0.1/nextstrain/cli/command/whoami.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-7.0.0/nextstrain/cli/config.py` & `nextstrain-cli-7.0.1/nextstrain/cli/config.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-7.0.0/nextstrain/cli/console.py` & `nextstrain-cli-7.0.1/nextstrain/cli/console.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-7.0.0/nextstrain/cli/debug.py` & `nextstrain-cli-7.0.1/nextstrain/cli/debug.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-7.0.0/nextstrain/cli/errors.py` & `nextstrain-cli-7.0.1/nextstrain/cli/errors.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-7.0.0/nextstrain/cli/gzip.py` & `nextstrain-cli-7.0.1/nextstrain/cli/gzip.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-7.0.0/nextstrain/cli/hostenv.py` & `nextstrain-cli-7.0.1/nextstrain/cli/hostenv.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-7.0.0/nextstrain/cli/markdown.py` & `nextstrain-cli-7.0.1/nextstrain/cli/markdown.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-7.0.0/nextstrain/cli/paths.py` & `nextstrain-cli-7.0.1/nextstrain/cli/paths.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-7.0.0/nextstrain/cli/remote/__init__.py` & `nextstrain-cli-7.0.1/nextstrain/cli/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-7.0.0/nextstrain/cli/remote/nextstrain_dot_org.py` & `nextstrain-cli-7.0.1/nextstrain/cli/remote/nextstrain_dot_org.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-7.0.0/nextstrain/cli/remote/s3.py` & `nextstrain-cli-7.0.1/nextstrain/cli/remote/s3.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-7.0.0/nextstrain/cli/resources/__init__.py` & `nextstrain-cli-7.0.1/nextstrain/cli/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-7.0.0/nextstrain/cli/resources/bashrc` & `nextstrain-cli-7.0.1/nextstrain/cli/resources/bashrc`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-7.0.0/nextstrain/cli/rst/__init__.py` & `nextstrain-cli-7.0.1/nextstrain/cli/rst/__init__.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-7.0.0/nextstrain/cli/rst/sphinx.py` & `nextstrain-cli-7.0.1/nextstrain/cli/rst/sphinx.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-7.0.0/nextstrain/cli/runner/__init__.py` & `nextstrain-cli-7.0.1/nextstrain/cli/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-7.0.0/nextstrain/cli/runner/ambient.py` & `nextstrain-cli-7.0.1/nextstrain/cli/runner/ambient.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-7.0.0/nextstrain/cli/runner/aws_batch/__init__.py` & `nextstrain-cli-7.0.1/nextstrain/cli/runner/aws_batch/__init__.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-7.0.0/nextstrain/cli/runner/aws_batch/jobs.py` & `nextstrain-cli-7.0.1/nextstrain/cli/runner/aws_batch/jobs.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-7.0.0/nextstrain/cli/runner/aws_batch/logs.py` & `nextstrain-cli-7.0.1/nextstrain/cli/runner/aws_batch/logs.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-7.0.0/nextstrain/cli/runner/aws_batch/s3.py` & `nextstrain-cli-7.0.1/nextstrain/cli/runner/aws_batch/s3.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-7.0.0/nextstrain/cli/runner/conda.py` & `nextstrain-cli-7.0.1/nextstrain/cli/runner/conda.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,16 @@
 import platform
 import re
 import requests
 import shutil
 import subprocess
 import tarfile
 import traceback
-from packaging.version import parse as parse_version
+from functools import partial
+from packaging.version import Version, InvalidVersion
 from pathlib import Path, PurePosixPath
 from typing import Iterable, NamedTuple, Optional
 from urllib.parse import urljoin, quote as urlquote
 from ..errors import InternalError
 from ..paths import RUNTIMES
 from ..types import RunnerSetupStatus, RunnerTestResults, RunnerUpdateStatus
 from ..util import capture_output, colored, exec_or_return, runner_tests_ok, warn
@@ -592,14 +593,74 @@
     label_files = (file for file in response.json() if label in file.get("labels", []))
     # Default '0-dev' should be the lowest version according to PEP440
     # See https://peps.python.org/pep-0440/#summary-of-permitted-suffixes-and-relative-ordering
     latest_file: dict = max(label_files, default={}, key=lambda file: parse_version(file.get('version', '0-dev')))
     return latest_file.get("version")
 
 
+def parse_version(version: str) -> Version:
+    """
+    Parse *version* into a PEP-440-compliant :cls:`Version` object, by hook or
+    by crook.
+
+    If *version* isn't already PEP-440 compliant, then it is parsed as a
+    PEP-440 local version label after replacing with ``.`` any characters not
+    matching ``a-z``, ``A-Z``, ``0-9``, ``.``, ``_``, or ``-``.  The comparison
+    semantics for local version labels amount to a string- and integer-based
+    comparison by parts ("segments"), which is super good enough for our
+    purposes here.  The full local version identifier produced for versions
+    parsed in this way always contains a public version identifier component of
+    ``0.dev0`` so it compares lowest against other public version identifiers.
+
+    >>> parse_version("1.2.3")
+    <Version('1.2.3')>
+    >>> parse_version("1.2.3-nope")
+    <Version('0.dev0+1.2.3.nope')>
+    >>> parse_version("20221019T172207Z")
+    <Version('0.dev0+20221019t172207z')>
+    >>> parse_version("@invalid+@")
+    <Version('0.dev0+invalid')>
+    >>> parse_version("not@@ok")
+    <Version('0.dev0+not.ok')>
+    >>> parse_version("20221019T172207Z") < parse_version("20230525T143814Z")
+    True
+    """
+    try:
+        return Version(version)
+    except InvalidVersion:
+        # Per PEP-440
+        #
+        # > …local version labels MUST be limited to the following set of
+        # > permitted characters:
+        # >
+        # >   ASCII letters ([a-zA-Z])
+        # >   ASCII digits ([0-9])
+        # >   periods (.)
+        # >
+        # > Local version labels MUST start and end with an ASCII letter or
+        # > digit.
+        #
+        # and
+        #
+        # > With a local version, in addition to the use of . as a separator of
+        # > segments, the use of - and _ is also acceptable. The normal form is
+        # > using the . character.
+        #
+        # and empty segments (x..z) aren't allowed either.
+        #
+        # c.f. <https://peps.python.org/pep-0440/#local-version-identifiers>
+        #      <https://peps.python.org/pep-0440/#local-version-segments>
+        remove_invalid_start_end_chars = partial(re.sub, r'^[^a-zA-Z0-9]+|[^a-zA-Z0-9]+$', '')
+        replace_invalid_with_separators = partial(re.sub, r'[^a-zA-Z0-9._-]+', '.')
+
+        as_local_segment = lambda v: replace_invalid_with_separators(remove_invalid_start_end_chars(v))
+
+        return Version(f"0.dev0+{as_local_segment(version)}")
+
+
 class PackageSpec(NamedTuple):
     name: str
     version_spec: Optional[str] = None
     build_id: Optional[str] = None
 
     @staticmethod
     def parse(spec):
```

### Comparing `nextstrain-cli-7.0.0/nextstrain/cli/runner/docker.py` & `nextstrain-cli-7.0.1/nextstrain/cli/runner/docker.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-7.0.0/nextstrain/cli/runner/singularity.py` & `nextstrain-cli-7.0.1/nextstrain/cli/runner/singularity.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-7.0.0/nextstrain/cli/types.py` & `nextstrain-cli-7.0.1/nextstrain/cli/types.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-7.0.0/nextstrain/cli/util.py` & `nextstrain-cli-7.0.1/nextstrain/cli/util.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-7.0.0/nextstrain/cli/volume.py` & `nextstrain-cli-7.0.1/nextstrain/cli/volume.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-7.0.0/nextstrain_cli.egg-info/PKG-INFO` & `nextstrain-cli-7.0.1/nextstrain_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextstrain-cli
-Version: 7.0.0
+Version: 7.0.1
 Summary: Nextstrain command-line tool
 Home-page: https://docs.nextstrain.org/projects/cli/
 Author: Thomas Sibley
 Author-email: tsibley@fredhutch.org
 License: MIT
 Project-URL: Bug Reports, https://github.com/nextstrain/cli/issues
 Project-URL: Change Log, https://github.com/nextstrain/cli/blob/master/CHANGES.md
```

### Comparing `nextstrain-cli-7.0.0/nextstrain_cli.egg-info/SOURCES.txt` & `nextstrain-cli-7.0.1/nextstrain_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-7.0.0/nextstrain_cli.egg-info/requires.txt` & `nextstrain-cli-7.0.1/nextstrain_cli.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-7.0.0/setup.py` & `nextstrain-cli-7.0.1/setup.py`

 * *Files identical despite different names*

