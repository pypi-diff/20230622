# Comparing `tmp/PyLEMS-0.6.2.tar.gz` & `tmp/PyLEMS-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyLEMS-0.6.2.tar", last modified: Wed May 10 09:50:37 2023, max compression
+gzip compressed data, was "PyLEMS-0.6.4.tar", last modified: Thu Jun 22 17:38:53 2023, max compression
```

## Comparing `PyLEMS-0.6.2.tar` & `PyLEMS-0.6.4.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:50:37.643511 PyLEMS-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-10 09:50:23.000000 PyLEMS-0.6.2/LICENSE.lesser
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-10 09:50:23.000000 PyLEMS-0.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-05-10 09:50:37.643511 PyLEMS-0.6.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:50:37.631511 PyLEMS-0.6.2/PyLEMS.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-05-10 09:50:37.000000 PyLEMS-0.6.2/PyLEMS.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-10 09:50:37.000000 PyLEMS-0.6.2/PyLEMS.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 09:50:37.000000 PyLEMS-0.6.2/PyLEMS.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-10 09:50:37.000000 PyLEMS-0.6.2/PyLEMS.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-10 09:50:37.000000 PyLEMS-0.6.2/PyLEMS.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:50:37.635511 PyLEMS-0.6.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/examples/MultiRunSimulation.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/examples/SimpleNetwork.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/examples/SimpleTest.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/examples/SingleSimulation.xml
--rwxr-xr-x   0 runner    (1001) docker     (123)      951 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/examples/apitest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/examples/apitest2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/examples/apitest3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/examples/bounce-conditional.xml
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/examples/elecdims.xml
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/examples/ex2dims.xml
--rw-r--r--   0 runner    (1001) docker     (123)    10891 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/examples/example1.xml
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/examples/example10_Q10.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/examples/example2.xml
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/examples/example3.xml
--rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/examples/example4.xml
--rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/examples/example5.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/examples/example6.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/examples/example7.xml
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/examples/example8.xml
--rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/examples/example9.xml
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/examples/hhaltgate.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/examples/hhcell.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/examples/hhchannel.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/examples/hhmodels.xml
--rwxr-xr-x   0 runner    (1001) docker     (123)      719 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/examples/loadtest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/examples/misciaf.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/examples/spikegenerators.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:50:37.635511 PyLEMS-0.6.2/lems/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/lems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/lems/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:50:37.639511 PyLEMS-0.6.2/lems/base/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/lems/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/lems/base/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/lems/base/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/lems/base/map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/lems/base/stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/lems/base/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:50:37.639511 PyLEMS-0.6.2/lems/dlems/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/lems/dlems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/lems/dlems/exportdlems.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:50:37.639511 PyLEMS-0.6.2/lems/model/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/lems/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35202 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/lems/model/component.py
--rw-r--r--   0 runner    (1001) docker     (123)    24275 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/lems/model/dynamics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/lems/model/fundamental.py
--rw-r--r--   0 runner    (1001) docker     (123)    49991 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/lems/model/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/lems/model/simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    14088 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/lems/model/structure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:50:37.639511 PyLEMS-0.6.2/lems/parser/
--rw-r--r--   0 runner    (1001) docker     (123)    57546 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/lems/parser/LEMS.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/lems/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17203 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/lems/parser/expr.py
--rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/lems/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:50:37.643511 PyLEMS-0.6.2/lems/sim/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/lems/sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46666 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/lems/sim/build.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/lems/sim/recording.py
--rw-r--r--   0 runner    (1001) docker     (123)    30369 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/lems/sim/runnable.py
--rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/lems/sim/sim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:50:37.627511 PyLEMS-0.6.2/man/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:50:37.643511 PyLEMS-0.6.2/man/man1/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/man/man1/pylems.1
--rwxr-xr-x   0 runner    (1001) docker     (123)      280 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/pylems
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-10 09:50:37.643511 PyLEMS-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-10 09:50:24.000000 PyLEMS-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:38:53.743073 PyLEMS-0.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/LICENSE.lesser
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-06-22 17:38:53.747073 PyLEMS-0.6.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:38:53.735073 PyLEMS-0.6.4/PyLEMS.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-06-22 17:38:53.000000 PyLEMS-0.6.4/PyLEMS.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-22 17:38:53.000000 PyLEMS-0.6.4/PyLEMS.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 17:38:53.000000 PyLEMS-0.6.4/PyLEMS.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-22 17:38:53.000000 PyLEMS-0.6.4/PyLEMS.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-22 17:38:53.000000 PyLEMS-0.6.4/PyLEMS.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-22 17:38:53.000000 PyLEMS-0.6.4/PyLEMS.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:38:53.739073 PyLEMS-0.6.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/examples/MultiRunSimulation.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/examples/SimpleNetwork.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/examples/SimpleTest.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/examples/SingleSimulation.xml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      951 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/examples/apitest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/examples/apitest2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/examples/apitest3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/examples/bounce-conditional.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/examples/elecdims.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/examples/ex2dims.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    10891 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/examples/example1.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/examples/example10_Q10.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/examples/example2.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/examples/example3.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/examples/example4.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/examples/example5.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/examples/example6.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/examples/example7.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/examples/example8.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/examples/example9.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/examples/hhaltgate.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/examples/hhcell.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/examples/hhchannel.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/examples/hhmodels.xml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      719 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/examples/loadtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/examples/misciaf.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/examples/spikegenerators.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:38:53.739073 PyLEMS-0.6.4/lems/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/lems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/lems/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:38:53.743073 PyLEMS-0.6.4/lems/base/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/lems/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/lems/base/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/lems/base/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/lems/base/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/lems/base/stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/lems/base/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:38:53.743073 PyLEMS-0.6.4/lems/dlems/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/lems/dlems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/lems/dlems/exportdlems.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:38:53.743073 PyLEMS-0.6.4/lems/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/lems/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35202 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/lems/model/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24275 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/lems/model/dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/lems/model/fundamental.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49991 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/lems/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/lems/model/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14088 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/lems/model/structure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:38:53.743073 PyLEMS-0.6.4/lems/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)    57546 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/lems/parser/LEMS.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/lems/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17203 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/lems/parser/expr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/lems/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:38:53.743073 PyLEMS-0.6.4/lems/sim/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/lems/sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46666 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/lems/sim/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/lems/sim/recording.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30369 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/lems/sim/runnable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/lems/sim/sim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:38:53.735073 PyLEMS-0.6.4/man/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:38:53.743073 PyLEMS-0.6.4/man/man1/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/man/man1/pylems.1
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-22 17:38:40.000000 PyLEMS-0.6.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-22 17:38:53.747073 PyLEMS-0.6.4/setup.cfg
```

### Comparing `PyLEMS-0.6.2/LICENSE.lesser` & `PyLEMS-0.6.4/LICENSE.lesser`

 * *Files identical despite different names*

### Comparing `PyLEMS-0.6.2/PKG-INFO` & `PyLEMS-0.6.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: PyLEMS
-Version: 0.6.2
+Version: 0.6.4
 Summary: A Python library for working with the Low Entropy Model Specification language (LEMS)
 Home-page: https://github.com/LEMS/pylems
 Author: PyLEMS authors and contributors
 Author-email: gautham@lisphacker.org, p.gleeson@gmail.com
-License: LGPL
+Maintainer-email: p.gleeson@gmail.com
+License: LGPL-3.0-only
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,15 +23,14 @@
 
 ## PyLEMS
 
 [![Build](https://github.com/LEMS/pylems/actions/workflows/ci.yml/badge.svg)](https://github.com/LEMS/pylems/actions/workflows/ci.yml)
 [![Check LEMS examples](https://github.com/LEMS/pylems/actions/workflows/examples.yml/badge.svg)](https://github.com/LEMS/pylems/actions/workflows/examples.yml)
 [![Documentation Status](https://readthedocs.org/projects/pylems/badge/?version=latest)](https://pylems.readthedocs.io/en/latest/?badge=latest)
 
-
 A LEMS (http://lems.github.io/LEMS) simulator written in Python which can be used to run NeuroML2  models (see [here](https://docs.neuroml.org/Userdocs/Software/pyLEMS.html)).
 
 For more about PyLEMS see:
 
 Michael Vella, Robert C. Cannon, Sharon Crook, Andrew P. Davison, Gautham Ganapathy, Hugh P. C. Robinson, R. Angus Silver and Padraig Gleeson,
 **libNeuroML and PyLEMS: using Python to combine procedural and declarative modeling approaches in computational neuroscience**
 [Frontiers in Neuroinformatics 2014](http://journal.frontiersin.org/Journal/10.3389/fninf.2014.00038/abstract), doi: 10.3389/fninf.2014.00038
@@ -39,44 +39,43 @@
 
 For more details on LEMS see:
 
 Robert C. Cannon, Padraig Gleeson, Sharon Crook, Gautham Ganapathy, Boris Marin, Eugenio Piasini and R. Angus Silver,
 **LEMS: A language for expressing complex biological models in concise and hierarchical form and its use in underpinning NeuroML 2**,
 [Frontiers in Neuroinformatics 2014](http://journal.frontiersin.org/Journal/10.3389/fninf.2014.00079/abstract), doi: 10.3389/fninf.2014.00079
 
-
 ### Installation
 
 A stable version of PyLEMS is [available on PyPI](https://pypi.python.org/pypi/PyLEMS) using [pip](https://pip.pypa.io/en/latest/installing.html):
 
-    pip install pylems
-
-To install as root:
-
-    sudo pip install pylems
+```
+pip install pylems
+```
 
 Alternatively, you can obtain the latest version with
 
-    git clone https://github.com/LEMS/pylems.git
-    cd pylems
-    git checkout development   # optional
-    sudo python setup.py install
+```
+git clone https://github.com/LEMS/pylems.git
+cd pylems
+git checkout development   # optional
+pip install .
+```
 
 ### Usage as a LEMS model simulator
 
-    pylems [options] LEMS_file
+```
+pylems [options] LEMS_file
+```
 
 **Options**
 
 - -I/-include path - Adds a directory to the model file include search path
 
-
 ### Examples
 
-
 **NeuroML examples (from https://github.com/NeuroML/NeuroML2/tree/development/NeuroML2CoreTypes)**
 
 - Example 0 --  Working
 - Example 1 --  Working
 - Example 2 --  Working
 - Example 3 --  Working
 - Example 4 --  Not working (Unsupported in PyLEMS: KSChannel)
@@ -91,26 +90,24 @@
 - Example 13 -- Working
 - Example 14 -- Not working (Unsupported in PyLEMS: Property)
 - Example 15 -- Working
 - Example 16 -- Working (apart from spikeArray)
 - Example 17 -- Working
 - Example 18 -- Working
 
-
 **LEMS examples (in directory examples)**
 
 - example1.xml --  Working
 - example2.xml --  Working
 - example3.xml --  Working
 - example4.xml --  Not working (Unsupported in PyLEMS: KSChannel)
 - example5.xml --  Not working (Unsupported in PyLEMS: KSChannel)
 - example6.xml --  Working
--- TODO: Rest of examples require an update to the `<Simulation>` element,
-   i.e. use `<Simulation...>` not `<SimulationSet...>`, to work in PyLEMS
 
+TODO: Rest of examples require an update to the `<Simulation>` element, i.e. use `<Simulation...>` not `<SimulationSet...>`, to work in PyLEMS
 
 **LEMS elements that do not work**
 
 - KSChannel
 - Property
 - XPath based parameters - PathParameter
 - Assertions
```

### Comparing `PyLEMS-0.6.2/PyLEMS.egg-info/PKG-INFO` & `PyLEMS-0.6.4/PyLEMS.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: PyLEMS
-Version: 0.6.2
+Version: 0.6.4
 Summary: A Python library for working with the Low Entropy Model Specification language (LEMS)
 Home-page: https://github.com/LEMS/pylems
 Author: PyLEMS authors and contributors
 Author-email: gautham@lisphacker.org, p.gleeson@gmail.com
-License: LGPL
+Maintainer-email: p.gleeson@gmail.com
+License: LGPL-3.0-only
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,15 +23,14 @@
 
 ## PyLEMS
 
 [![Build](https://github.com/LEMS/pylems/actions/workflows/ci.yml/badge.svg)](https://github.com/LEMS/pylems/actions/workflows/ci.yml)
 [![Check LEMS examples](https://github.com/LEMS/pylems/actions/workflows/examples.yml/badge.svg)](https://github.com/LEMS/pylems/actions/workflows/examples.yml)
 [![Documentation Status](https://readthedocs.org/projects/pylems/badge/?version=latest)](https://pylems.readthedocs.io/en/latest/?badge=latest)
 
-
 A LEMS (http://lems.github.io/LEMS) simulator written in Python which can be used to run NeuroML2  models (see [here](https://docs.neuroml.org/Userdocs/Software/pyLEMS.html)).
 
 For more about PyLEMS see:
 
 Michael Vella, Robert C. Cannon, Sharon Crook, Andrew P. Davison, Gautham Ganapathy, Hugh P. C. Robinson, R. Angus Silver and Padraig Gleeson,
 **libNeuroML and PyLEMS: using Python to combine procedural and declarative modeling approaches in computational neuroscience**
 [Frontiers in Neuroinformatics 2014](http://journal.frontiersin.org/Journal/10.3389/fninf.2014.00038/abstract), doi: 10.3389/fninf.2014.00038
@@ -39,44 +39,43 @@
 
 For more details on LEMS see:
 
 Robert C. Cannon, Padraig Gleeson, Sharon Crook, Gautham Ganapathy, Boris Marin, Eugenio Piasini and R. Angus Silver,
 **LEMS: A language for expressing complex biological models in concise and hierarchical form and its use in underpinning NeuroML 2**,
 [Frontiers in Neuroinformatics 2014](http://journal.frontiersin.org/Journal/10.3389/fninf.2014.00079/abstract), doi: 10.3389/fninf.2014.00079
 
-
 ### Installation
 
 A stable version of PyLEMS is [available on PyPI](https://pypi.python.org/pypi/PyLEMS) using [pip](https://pip.pypa.io/en/latest/installing.html):
 
-    pip install pylems
-
-To install as root:
-
-    sudo pip install pylems
+```
+pip install pylems
+```
 
 Alternatively, you can obtain the latest version with
 
-    git clone https://github.com/LEMS/pylems.git
-    cd pylems
-    git checkout development   # optional
-    sudo python setup.py install
+```
+git clone https://github.com/LEMS/pylems.git
+cd pylems
+git checkout development   # optional
+pip install .
+```
 
 ### Usage as a LEMS model simulator
 
-    pylems [options] LEMS_file
+```
+pylems [options] LEMS_file
+```
 
 **Options**
 
 - -I/-include path - Adds a directory to the model file include search path
 
-
 ### Examples
 
-
 **NeuroML examples (from https://github.com/NeuroML/NeuroML2/tree/development/NeuroML2CoreTypes)**
 
 - Example 0 --  Working
 - Example 1 --  Working
 - Example 2 --  Working
 - Example 3 --  Working
 - Example 4 --  Not working (Unsupported in PyLEMS: KSChannel)
@@ -91,26 +90,24 @@
 - Example 13 -- Working
 - Example 14 -- Not working (Unsupported in PyLEMS: Property)
 - Example 15 -- Working
 - Example 16 -- Working (apart from spikeArray)
 - Example 17 -- Working
 - Example 18 -- Working
 
-
 **LEMS examples (in directory examples)**
 
 - example1.xml --  Working
 - example2.xml --  Working
 - example3.xml --  Working
 - example4.xml --  Not working (Unsupported in PyLEMS: KSChannel)
 - example5.xml --  Not working (Unsupported in PyLEMS: KSChannel)
 - example6.xml --  Working
--- TODO: Rest of examples require an update to the `<Simulation>` element,
-   i.e. use `<Simulation...>` not `<SimulationSet...>`, to work in PyLEMS
 
+TODO: Rest of examples require an update to the `<Simulation>` element, i.e. use `<Simulation...>` not `<SimulationSet...>`, to work in PyLEMS
 
 **LEMS elements that do not work**
 
 - KSChannel
 - Property
 - XPath based parameters - PathParameter
 - Assertions
```

### Comparing `PyLEMS-0.6.2/PyLEMS.egg-info/SOURCES.txt` & `PyLEMS-0.6.4/PyLEMS.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 LICENSE.lesser
 MANIFEST.in
 README.md
-pylems
+pyproject.toml
 setup.cfg
-setup.py
 PyLEMS.egg-info/PKG-INFO
 PyLEMS.egg-info/SOURCES.txt
 PyLEMS.egg-info/dependency_links.txt
+PyLEMS.egg-info/entry_points.txt
 PyLEMS.egg-info/requires.txt
 PyLEMS.egg-info/top_level.txt
 examples/MultiRunSimulation.xml
 examples/SimpleNetwork.xml
 examples/SimpleTest.xml
 examples/SingleSimulation.xml
 examples/apitest.py
```

### Comparing `PyLEMS-0.6.2/README.md` & `PyLEMS-0.6.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 ## PyLEMS
 
 [![Build](https://github.com/LEMS/pylems/actions/workflows/ci.yml/badge.svg)](https://github.com/LEMS/pylems/actions/workflows/ci.yml)
 [![Check LEMS examples](https://github.com/LEMS/pylems/actions/workflows/examples.yml/badge.svg)](https://github.com/LEMS/pylems/actions/workflows/examples.yml)
 [![Documentation Status](https://readthedocs.org/projects/pylems/badge/?version=latest)](https://pylems.readthedocs.io/en/latest/?badge=latest)
 
-
 A LEMS (http://lems.github.io/LEMS) simulator written in Python which can be used to run NeuroML2  models (see [here](https://docs.neuroml.org/Userdocs/Software/pyLEMS.html)).
 
 For more about PyLEMS see:
 
 Michael Vella, Robert C. Cannon, Sharon Crook, Andrew P. Davison, Gautham Ganapathy, Hugh P. C. Robinson, R. Angus Silver and Padraig Gleeson,
 **libNeuroML and PyLEMS: using Python to combine procedural and declarative modeling approaches in computational neuroscience**
 [Frontiers in Neuroinformatics 2014](http://journal.frontiersin.org/Journal/10.3389/fninf.2014.00038/abstract), doi: 10.3389/fninf.2014.00038
@@ -17,44 +16,43 @@
 
 For more details on LEMS see:
 
 Robert C. Cannon, Padraig Gleeson, Sharon Crook, Gautham Ganapathy, Boris Marin, Eugenio Piasini and R. Angus Silver,
 **LEMS: A language for expressing complex biological models in concise and hierarchical form and its use in underpinning NeuroML 2**,
 [Frontiers in Neuroinformatics 2014](http://journal.frontiersin.org/Journal/10.3389/fninf.2014.00079/abstract), doi: 10.3389/fninf.2014.00079
 
-
 ### Installation
 
 A stable version of PyLEMS is [available on PyPI](https://pypi.python.org/pypi/PyLEMS) using [pip](https://pip.pypa.io/en/latest/installing.html):
 
-    pip install pylems
-
-To install as root:
-
-    sudo pip install pylems
+```
+pip install pylems
+```
 
 Alternatively, you can obtain the latest version with
 
-    git clone https://github.com/LEMS/pylems.git
-    cd pylems
-    git checkout development   # optional
-    sudo python setup.py install
+```
+git clone https://github.com/LEMS/pylems.git
+cd pylems
+git checkout development   # optional
+pip install .
+```
 
 ### Usage as a LEMS model simulator
 
-    pylems [options] LEMS_file
+```
+pylems [options] LEMS_file
+```
 
 **Options**
 
 - -I/-include path - Adds a directory to the model file include search path
 
-
 ### Examples
 
-
 **NeuroML examples (from https://github.com/NeuroML/NeuroML2/tree/development/NeuroML2CoreTypes)**
 
 - Example 0 --  Working
 - Example 1 --  Working
 - Example 2 --  Working
 - Example 3 --  Working
 - Example 4 --  Not working (Unsupported in PyLEMS: KSChannel)
@@ -69,26 +67,24 @@
 - Example 13 -- Working
 - Example 14 -- Not working (Unsupported in PyLEMS: Property)
 - Example 15 -- Working
 - Example 16 -- Working (apart from spikeArray)
 - Example 17 -- Working
 - Example 18 -- Working
 
-
 **LEMS examples (in directory examples)**
 
 - example1.xml --  Working
 - example2.xml --  Working
 - example3.xml --  Working
 - example4.xml --  Not working (Unsupported in PyLEMS: KSChannel)
 - example5.xml --  Not working (Unsupported in PyLEMS: KSChannel)
 - example6.xml --  Working
--- TODO: Rest of examples require an update to the `<Simulation>` element,
-   i.e. use `<Simulation...>` not `<SimulationSet...>`, to work in PyLEMS
 
+TODO: Rest of examples require an update to the `<Simulation>` element, i.e. use `<Simulation...>` not `<SimulationSet...>`, to work in PyLEMS
 
 **LEMS elements that do not work**
 
 - KSChannel
 - Property
 - XPath based parameters - PathParameter
 - Assertions
```

### Comparing `PyLEMS-0.6.2/examples/MultiRunSimulation.xml` & `PyLEMS-0.6.4/examples/MultiRunSimulation.xml`

 * *Files identical despite different names*

### Comparing `PyLEMS-0.6.2/examples/SimpleNetwork.xml` & `PyLEMS-0.6.4/examples/SimpleNetwork.xml`

 * *Files identical despite different names*

### Comparing `PyLEMS-0.6.2/examples/SimpleTest.xml` & `PyLEMS-0.6.4/examples/SimpleTest.xml`

 * *Files identical despite different names*

### Comparing `PyLEMS-0.6.2/examples/SingleSimulation.xml` & `PyLEMS-0.6.4/examples/SingleSimulation.xml`

 * *Files identical despite different names*

### Comparing `PyLEMS-0.6.2/examples/apitest.py` & `PyLEMS-0.6.4/examples/apitest.py`

 * *Files identical despite different names*

### Comparing `PyLEMS-0.6.2/examples/apitest2.py` & `PyLEMS-0.6.4/examples/apitest2.py`

 * *Files identical despite different names*

### Comparing `PyLEMS-0.6.2/examples/apitest3.py` & `PyLEMS-0.6.4/examples/apitest3.py`

 * *Files identical despite different names*

### Comparing `PyLEMS-0.6.2/examples/bounce-conditional.xml` & `PyLEMS-0.6.4/examples/bounce-conditional.xml`

 * *Files identical despite different names*

### Comparing `PyLEMS-0.6.2/examples/ex2dims.xml` & `PyLEMS-0.6.4/examples/ex2dims.xml`

 * *Files identical despite different names*

### Comparing `PyLEMS-0.6.2/examples/example1.xml` & `PyLEMS-0.6.4/examples/example1.xml`

 * *Files identical despite different names*

### Comparing `PyLEMS-0.6.2/examples/example10_Q10.xml` & `PyLEMS-0.6.4/examples/example10_Q10.xml`

 * *Files identical despite different names*

### Comparing `PyLEMS-0.6.2/examples/example2.xml` & `PyLEMS-0.6.4/examples/example2.xml`

 * *Files identical despite different names*

### Comparing `PyLEMS-0.6.2/examples/example3.xml` & `PyLEMS-0.6.4/examples/example3.xml`

 * *Files identical despite different names*

### Comparing `PyLEMS-0.6.2/examples/example4.xml` & `PyLEMS-0.6.4/examples/example4.xml`

 * *Files identical despite different names*

### Comparing `PyLEMS-0.6.2/examples/example5.xml` & `PyLEMS-0.6.4/examples/example5.xml`

 * *Files identical despite different names*

### Comparing `PyLEMS-0.6.2/examples/example6.xml` & `PyLEMS-0.6.4/examples/example6.xml`

 * *Files identical despite different names*

### Comparing `PyLEMS-0.6.2/examples/example7.xml` & `PyLEMS-0.6.4/examples/example7.xml`

 * *Files identical despite different names*

### Comparing `PyLEMS-0.6.2/examples/example8.xml` & `PyLEMS-0.6.4/examples/example8.xml`

 * *Files identical despite different names*

### Comparing `PyLEMS-0.6.2/examples/example9.xml` & `PyLEMS-0.6.4/examples/example9.xml`

 * *Files identical despite different names*

### Comparing `PyLEMS-0.6.2/examples/hhaltgate.xml` & `PyLEMS-0.6.4/examples/hhaltgate.xml`

 * *Files identical despite different names*

### Comparing `PyLEMS-0.6.2/examples/hhcell.xml` & `PyLEMS-0.6.4/examples/hhcell.xml`

 * *Files identical despite different names*

### Comparing `PyLEMS-0.6.2/examples/hhchannel.xml` & `PyLEMS-0.6.4/examples/hhchannel.xml`

 * *Files identical despite different names*

### Comparing `PyLEMS-0.6.2/examples/hhmodels.xml` & `PyLEMS-0.6.4/examples/hhmodels.xml`

 * *Files identical despite different names*

### Comparing `PyLEMS-0.6.2/examples/loadtest.py` & `PyLEMS-0.6.4/examples/loadtest.py`

 * *Files identical despite different names*

### Comparing `PyLEMS-0.6.2/examples/misciaf.xml` & `PyLEMS-0.6.4/examples/misciaf.xml`

 * *Files identical despite different names*

### Comparing `PyLEMS-0.6.2/examples/spikegenerators.xml` & `PyLEMS-0.6.4/examples/spikegenerators.xml`

 * *Files identical despite different names*

### Comparing `PyLEMS-0.6.2/lems/base/errors.py` & `PyLEMS-0.6.4/lems/base/errors.py`

 * *Files identical despite different names*

### Comparing `PyLEMS-0.6.2/lems/base/stack.py` & `PyLEMS-0.6.4/lems/base/stack.py`

 * *Files identical despite different names*

### Comparing `PyLEMS-0.6.2/lems/base/util.py` & `PyLEMS-0.6.4/lems/base/util.py`

 * *Files identical despite different names*

### Comparing `PyLEMS-0.6.2/lems/dlems/exportdlems.py` & `PyLEMS-0.6.4/lems/dlems/exportdlems.py`

 * *Files identical despite different names*

### Comparing `PyLEMS-0.6.2/lems/model/component.py` & `PyLEMS-0.6.4/lems/model/component.py`

 * *Files identical despite different names*

### Comparing `PyLEMS-0.6.2/lems/model/dynamics.py` & `PyLEMS-0.6.4/lems/model/dynamics.py`

 * *Files identical despite different names*

### Comparing `PyLEMS-0.6.2/lems/model/fundamental.py` & `PyLEMS-0.6.4/lems/model/fundamental.py`

 * *Files identical despite different names*

### Comparing `PyLEMS-0.6.2/lems/model/model.py` & `PyLEMS-0.6.4/lems/model/model.py`

 * *Files identical despite different names*

### Comparing `PyLEMS-0.6.2/lems/model/simulation.py` & `PyLEMS-0.6.4/lems/model/simulation.py`

 * *Files identical despite different names*

### Comparing `PyLEMS-0.6.2/lems/model/structure.py` & `PyLEMS-0.6.4/lems/model/structure.py`

 * *Files identical despite different names*

### Comparing `PyLEMS-0.6.2/lems/parser/LEMS.py` & `PyLEMS-0.6.4/lems/parser/LEMS.py`

 * *Files identical despite different names*

### Comparing `PyLEMS-0.6.2/lems/parser/expr.py` & `PyLEMS-0.6.4/lems/parser/expr.py`

 * *Files identical despite different names*

### Comparing `PyLEMS-0.6.2/lems/run.py` & `PyLEMS-0.6.4/lems/run.py`

 * *Files identical despite different names*

### Comparing `PyLEMS-0.6.2/lems/sim/build.py` & `PyLEMS-0.6.4/lems/sim/build.py`

 * *Files identical despite different names*

### Comparing `PyLEMS-0.6.2/lems/sim/recording.py` & `PyLEMS-0.6.4/lems/sim/recording.py`

 * *Files identical despite different names*

### Comparing `PyLEMS-0.6.2/lems/sim/runnable.py` & `PyLEMS-0.6.4/lems/sim/runnable.py`

 * *Files identical despite different names*

### Comparing `PyLEMS-0.6.2/lems/sim/sim.py` & `PyLEMS-0.6.4/lems/sim/sim.py`

 * *Files identical despite different names*

### Comparing `PyLEMS-0.6.2/man/man1/pylems.1` & `PyLEMS-0.6.4/man/man1/pylems.1`

 * *Files identical despite different names*

