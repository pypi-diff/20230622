# Comparing `tmp/currentscape-1.0.6.tar.gz` & `tmp/currentscape-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "currentscape-1.0.6.tar", last modified: Wed Jun 21 10:47:19 2023, max compression
+gzip compressed data, was "currentscape-1.0.7.tar", last modified: Thu Jun 22 10:14:56 2023, max compression
```

## Comparing `currentscape-1.0.6.tar` & `currentscape-1.0.7.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:47:19.475717 currentscape-1.0.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:47:19.467717 currentscape-1.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:47:19.471717 currentscape-1.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-21 10:47:06.000000 currentscape-1.0.6/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-21 10:47:06.000000 currentscape-1.0.6/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-21 10:47:06.000000 currentscape-1.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-21 10:47:06.000000 currentscape-1.0.6/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-06-21 10:47:06.000000 currentscape-1.0.6/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-21 10:47:06.000000 currentscape-1.0.6/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-21 10:47:06.000000 currentscape-1.0.6/.zenodo.json
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-21 10:47:06.000000 currentscape-1.0.6/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-06-21 10:47:06.000000 currentscape-1.0.6/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-06-21 10:47:06.000000 currentscape-1.0.6/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-06-21 10:47:06.000000 currentscape-1.0.6/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-21 10:47:06.000000 currentscape-1.0.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-21 10:47:06.000000 currentscape-1.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-21 10:47:06.000000 currentscape-1.0.6/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    11485 2023-06-21 10:47:19.475717 currentscape-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10479 2023-06-21 10:47:06.000000 currentscape-1.0.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15155 2023-06-21 10:47:06.000000 currentscape-1.0.6/Tutorial.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:47:19.471717 currentscape-1.0.6/currentscape/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-21 10:47:06.000000 currentscape-1.0.6/currentscape/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-06-21 10:47:06.000000 currentscape-1.0.6/currentscape/config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    23209 2023-06-21 10:47:06.000000 currentscape-1.0.6/currentscape/currents.py
--rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-06-21 10:47:06.000000 currentscape-1.0.6/currentscape/currentscape.py
--rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-06-21 10:47:06.000000 currentscape-1.0.6/currentscape/data_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-06-21 10:47:06.000000 currentscape-1.0.6/currentscape/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-06-21 10:47:06.000000 currentscape-1.0.6/currentscape/ions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7699 2023-06-21 10:47:06.000000 currentscape-1.0.6/currentscape/legends.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-06-21 10:47:06.000000 currentscape-1.0.6/currentscape/mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    18165 2023-06-21 10:47:06.000000 currentscape-1.0.6/currentscape/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-06-21 10:47:06.000000 currentscape-1.0.6/currentscape/voltages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:47:19.471717 currentscape-1.0.6/currentscape.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11485 2023-06-21 10:47:19.000000 currentscape-1.0.6/currentscape.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-06-21 10:47:19.000000 currentscape-1.0.6/currentscape.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 10:47:19.000000 currentscape-1.0.6/currentscape.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-21 10:47:19.000000 currentscape-1.0.6/currentscape.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-21 10:47:19.000000 currentscape-1.0.6/currentscape.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:47:19.471717 currentscape-1.0.6/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-21 10:47:06.000000 currentscape-1.0.6/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:47:19.471717 currentscape-1.0.6/doc/source/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-21 10:47:06.000000 currentscape-1.0.6/doc/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-21 10:47:06.000000 currentscape-1.0.6/doc/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-21 10:47:06.000000 currentscape-1.0.6/doc/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:47:19.471717 currentscape-1.0.6/doc/source/images/
--rw-r--r--   0 runner    (1001) docker     (123)   183971 2023-06-21 10:47:06.000000 currentscape-1.0.6/doc/source/images/plot.png
--rw-r--r--   0 runner    (1001) docker     (123)    51976 2023-06-21 10:47:06.000000 currentscape-1.0.6/doc/source/images/quickstart_plot.png
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-21 10:47:06.000000 currentscape-1.0.6/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-21 10:47:06.000000 currentscape-1.0.6/doc/source/tutorial.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:47:19.467717 currentscape-1.0.6/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:47:19.471717 currentscape-1.0.6/examples/original_paper_plot/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-21 10:47:06.000000 currentscape-1.0.6/examples/original_paper_plot/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-06-21 10:47:06.000000 currentscape-1.0.6/examples/original_paper_plot/LICENSE_CC0-1.0
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 10:47:06.000000 currentscape-1.0.6/examples/original_paper_plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-21 10:47:06.000000 currentscape-1.0.6/examples/original_paper_plot/config.json
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-06-21 10:47:06.000000 currentscape-1.0.6/examples/original_paper_plot/get_currents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-21 10:47:06.000000 currentscape-1.0.6/examples/original_paper_plot/integrate_single_compartment_and_plot_currentscape.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:47:19.475717 currentscape-1.0.6/examples/original_paper_plot/parameters-and-initial-conditions/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-21 10:47:06.000000 currentscape-1.0.6/examples/original_paper_plot/parameters-and-initial-conditions/initial-conditions.txt
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-21 10:47:06.000000 currentscape-1.0.6/examples/original_paper_plot/parameters-and-initial-conditions/model-A-name-HZFTSB.txt
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-21 10:47:06.000000 currentscape-1.0.6/examples/original_paper_plot/parameters-and-initial-conditions/model-B-name-8XCUQE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-21 10:47:06.000000 currentscape-1.0.6/examples/original_paper_plot/parameters-and-initial-conditions/model-C-name-C1L1R0.txt
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-21 10:47:06.000000 currentscape-1.0.6/examples/original_paper_plot/parameters-and-initial-conditions/model-D-name-KI47XV.txt
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-21 10:47:06.000000 currentscape-1.0.6/examples/original_paper_plot/parameters-and-initial-conditions/model-E-name-OG1RE2.txt
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-21 10:47:06.000000 currentscape-1.0.6/examples/original_paper_plot/parameters-and-initial-conditions/model-F-name-B7S21N.txt
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-21 10:47:06.000000 currentscape-1.0.6/examples/original_paper_plot/parameters-and-initial-conditions/model-FIG2-name-1BLGMA.txt
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-21 10:47:06.000000 currentscape-1.0.6/examples/original_paper_plot/parameters-and-initial-conditions/model-FIG3-name-VVECT5.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-06-21 10:47:06.000000 currentscape-1.0.6/examples/original_paper_plot/single_compartment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:47:19.475717 currentscape-1.0.6/examples/use_case/
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-21 10:47:06.000000 currentscape-1.0.6/examples/use_case/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-06-21 10:47:06.000000 currentscape-1.0.6/examples/use_case/LICENSE_CC-BY-CA-SA-4.0
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 10:47:06.000000 currentscape-1.0.6/examples/use_case/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:47:19.467717 currentscape-1.0.6/examples/use_case/config/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:47:19.475717 currentscape-1.0.6/examples/use_case/config/params/
--rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-06-21 10:47:06.000000 currentscape-1.0.6/examples/use_case/config/params/final.json
--rw-r--r--   0 runner    (1001) docker     (123)    10218 2023-06-21 10:47:06.000000 currentscape-1.0.6/examples/use_case/config/params/pyr.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:47:19.475717 currentscape-1.0.6/examples/use_case/mechanisms/
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-21 10:47:06.000000 currentscape-1.0.6/examples/use_case/mechanisms/CaDynamics_DC0.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-21 10:47:06.000000 currentscape-1.0.6/examples/use_case/mechanisms/Ca_HVA2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-21 10:47:06.000000 currentscape-1.0.6/examples/use_case/mechanisms/Ca_LVAst.mod
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-21 10:47:06.000000 currentscape-1.0.6/examples/use_case/mechanisms/Ih.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-21 10:47:06.000000 currentscape-1.0.6/examples/use_case/mechanisms/K_Pst.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-21 10:47:06.000000 currentscape-1.0.6/examples/use_case/mechanisms/K_Tst.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-21 10:47:06.000000 currentscape-1.0.6/examples/use_case/mechanisms/NaTg.mod
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-06-21 10:47:06.000000 currentscape-1.0.6/examples/use_case/mechanisms/Nap_Et2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-21 10:47:06.000000 currentscape-1.0.6/examples/use_case/mechanisms/SK_E2.mod
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-21 10:47:06.000000 currentscape-1.0.6/examples/use_case/mechanisms/SKv3_1.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-21 10:47:06.000000 currentscape-1.0.6/examples/use_case/mechanisms/notes.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:47:19.475717 currentscape-1.0.6/examples/use_case/morphology/
--rw-r--r--   0 runner    (1001) docker     (123)   135189 2023-06-21 10:47:06.000000 currentscape-1.0.6/examples/use_case/morphology/dend-C231296A-P4B2_axon-C200897C-P2_-_Scale_x1.000_y0.975_z1.000.asc
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-06-21 10:47:06.000000 currentscape-1.0.6/examples/use_case/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:47:19.475717 currentscape-1.0.6/examples/use_case/python_recordings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 10:47:06.000000 currentscape-1.0.6/examples/use_case/python_recordings/.keep
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-06-21 10:47:06.000000 currentscape-1.0.6/examples/use_case/run.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      665 2023-06-21 10:47:06.000000 currentscape-1.0.6/examples/use_case/run_py.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:47:19.467717 currentscape-1.0.6/extra/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:47:19.475717 currentscape-1.0.6/extra/jjb-cells/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-21 10:47:06.000000 currentscape-1.0.6/extra/jjb-cells/cells.currentscape.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:47:19.467717 currentscape-1.0.6/extra/spack/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:47:19.467717 currentscape-1.0.6/extra/spack/var/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:47:19.467717 currentscape-1.0.6/extra/spack/var/spack/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:47:19.467717 currentscape-1.0.6/extra/spack/var/spack/repos/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:47:19.467717 currentscape-1.0.6/extra/spack/var/spack/repos/builtin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:47:19.467717 currentscape-1.0.6/extra/spack/var/spack/repos/builtin/packages/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:47:19.475717 currentscape-1.0.6/extra/spack/var/spack/repos/builtin/packages/py-currentscape/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-21 10:47:06.000000 currentscape-1.0.6/extra/spack/var/spack/repos/builtin/packages/py-currentscape/package.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-21 10:47:06.000000 currentscape-1.0.6/requirements_docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 10:47:19.475717 currentscape-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-06-21 10:47:06.000000 currentscape-1.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:47:19.475717 currentscape-1.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 10:47:06.000000 currentscape-1.0.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-21 10:47:06.000000 currentscape-1.0.6/tests/extract_bNAC_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-21 10:47:06.000000 currentscape-1.0.6/tests/test_currentscape_config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-21 10:47:06.000000 currentscape-1.0.6/tests/test_currentscape_currents.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-06-21 10:47:06.000000 currentscape-1.0.6/tests/test_currentscape_dataprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-06-21 10:47:06.000000 currentscape-1.0.6/tests/test_currentscape_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-21 10:47:06.000000 currentscape-1.0.6/tests/test_currentscape_from_paper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-21 10:47:06.000000 currentscape-1.0.6/tests/test_currentscape_ions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-06-21 10:47:06.000000 currentscape-1.0.6/tests/test_currentscape_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8340 2023-06-21 10:47:06.000000 currentscape-1.0.6/tests/test_currentscape_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-21 10:47:06.000000 currentscape-1.0.6/tests/test_use_case_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-21 10:47:06.000000 currentscape-1.0.6/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-21 10:47:06.000000 currentscape-1.0.6/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:14:56.734471 currentscape-1.0.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:14:56.726471 currentscape-1.0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:14:56.730471 currentscape-1.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-06-22 10:14:47.000000 currentscape-1.0.7/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-22 10:14:47.000000 currentscape-1.0.7/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-22 10:14:47.000000 currentscape-1.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-22 10:14:47.000000 currentscape-1.0.7/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-06-22 10:14:47.000000 currentscape-1.0.7/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-22 10:14:47.000000 currentscape-1.0.7/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-22 10:14:47.000000 currentscape-1.0.7/.zenodo.json
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-22 10:14:47.000000 currentscape-1.0.7/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-06-22 10:14:47.000000 currentscape-1.0.7/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-06-22 10:14:47.000000 currentscape-1.0.7/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-06-22 10:14:47.000000 currentscape-1.0.7/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-22 10:14:47.000000 currentscape-1.0.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-22 10:14:47.000000 currentscape-1.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-22 10:14:47.000000 currentscape-1.0.7/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    11485 2023-06-22 10:14:56.734471 currentscape-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10479 2023-06-22 10:14:47.000000 currentscape-1.0.7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15155 2023-06-22 10:14:47.000000 currentscape-1.0.7/Tutorial.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:14:56.730471 currentscape-1.0.7/currentscape/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-22 10:14:47.000000 currentscape-1.0.7/currentscape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-06-22 10:14:47.000000 currentscape-1.0.7/currentscape/config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23209 2023-06-22 10:14:47.000000 currentscape-1.0.7/currentscape/currents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-06-22 10:14:47.000000 currentscape-1.0.7/currentscape/currentscape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-06-22 10:14:47.000000 currentscape-1.0.7/currentscape/data_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-06-22 10:14:47.000000 currentscape-1.0.7/currentscape/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-06-22 10:14:47.000000 currentscape-1.0.7/currentscape/ions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7699 2023-06-22 10:14:47.000000 currentscape-1.0.7/currentscape/legends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-06-22 10:14:47.000000 currentscape-1.0.7/currentscape/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18165 2023-06-22 10:14:47.000000 currentscape-1.0.7/currentscape/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-06-22 10:14:47.000000 currentscape-1.0.7/currentscape/voltages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:14:56.730471 currentscape-1.0.7/currentscape.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11485 2023-06-22 10:14:56.000000 currentscape-1.0.7/currentscape.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-06-22 10:14:56.000000 currentscape-1.0.7/currentscape.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 10:14:56.000000 currentscape-1.0.7/currentscape.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-22 10:14:56.000000 currentscape-1.0.7/currentscape.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-22 10:14:56.000000 currentscape-1.0.7/currentscape.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:14:56.730471 currentscape-1.0.7/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-22 10:14:47.000000 currentscape-1.0.7/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:14:56.730471 currentscape-1.0.7/doc/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-22 10:14:47.000000 currentscape-1.0.7/doc/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-22 10:14:47.000000 currentscape-1.0.7/doc/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-22 10:14:47.000000 currentscape-1.0.7/doc/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:14:56.730471 currentscape-1.0.7/doc/source/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   183971 2023-06-22 10:14:47.000000 currentscape-1.0.7/doc/source/images/plot.png
+-rw-r--r--   0 runner    (1001) docker     (123)    51976 2023-06-22 10:14:47.000000 currentscape-1.0.7/doc/source/images/quickstart_plot.png
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-22 10:14:47.000000 currentscape-1.0.7/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-22 10:14:47.000000 currentscape-1.0.7/doc/source/tutorial.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:14:56.726471 currentscape-1.0.7/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:14:56.730471 currentscape-1.0.7/examples/original_paper_plot/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-22 10:14:47.000000 currentscape-1.0.7/examples/original_paper_plot/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-06-22 10:14:47.000000 currentscape-1.0.7/examples/original_paper_plot/LICENSE_CC0-1.0
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 10:14:47.000000 currentscape-1.0.7/examples/original_paper_plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-22 10:14:47.000000 currentscape-1.0.7/examples/original_paper_plot/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-06-22 10:14:47.000000 currentscape-1.0.7/examples/original_paper_plot/get_currents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-22 10:14:47.000000 currentscape-1.0.7/examples/original_paper_plot/integrate_single_compartment_and_plot_currentscape.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:14:56.730471 currentscape-1.0.7/examples/original_paper_plot/parameters-and-initial-conditions/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-22 10:14:47.000000 currentscape-1.0.7/examples/original_paper_plot/parameters-and-initial-conditions/initial-conditions.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-22 10:14:47.000000 currentscape-1.0.7/examples/original_paper_plot/parameters-and-initial-conditions/model-A-name-HZFTSB.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-22 10:14:47.000000 currentscape-1.0.7/examples/original_paper_plot/parameters-and-initial-conditions/model-B-name-8XCUQE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-22 10:14:47.000000 currentscape-1.0.7/examples/original_paper_plot/parameters-and-initial-conditions/model-C-name-C1L1R0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-22 10:14:47.000000 currentscape-1.0.7/examples/original_paper_plot/parameters-and-initial-conditions/model-D-name-KI47XV.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-22 10:14:47.000000 currentscape-1.0.7/examples/original_paper_plot/parameters-and-initial-conditions/model-E-name-OG1RE2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-22 10:14:47.000000 currentscape-1.0.7/examples/original_paper_plot/parameters-and-initial-conditions/model-F-name-B7S21N.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-22 10:14:47.000000 currentscape-1.0.7/examples/original_paper_plot/parameters-and-initial-conditions/model-FIG2-name-1BLGMA.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-22 10:14:47.000000 currentscape-1.0.7/examples/original_paper_plot/parameters-and-initial-conditions/model-FIG3-name-VVECT5.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-06-22 10:14:47.000000 currentscape-1.0.7/examples/original_paper_plot/single_compartment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:14:56.734471 currentscape-1.0.7/examples/use_case/
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-22 10:14:47.000000 currentscape-1.0.7/examples/use_case/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-06-22 10:14:47.000000 currentscape-1.0.7/examples/use_case/LICENSE_CC-BY-CA-SA-4.0
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 10:14:47.000000 currentscape-1.0.7/examples/use_case/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:14:56.726471 currentscape-1.0.7/examples/use_case/config/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:14:56.734471 currentscape-1.0.7/examples/use_case/config/params/
+-rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-06-22 10:14:47.000000 currentscape-1.0.7/examples/use_case/config/params/final.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10218 2023-06-22 10:14:47.000000 currentscape-1.0.7/examples/use_case/config/params/pyr.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:14:56.734471 currentscape-1.0.7/examples/use_case/mechanisms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-22 10:14:47.000000 currentscape-1.0.7/examples/use_case/mechanisms/CaDynamics_DC0.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-22 10:14:47.000000 currentscape-1.0.7/examples/use_case/mechanisms/Ca_HVA2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-22 10:14:47.000000 currentscape-1.0.7/examples/use_case/mechanisms/Ca_LVAst.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-22 10:14:47.000000 currentscape-1.0.7/examples/use_case/mechanisms/Ih.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-22 10:14:47.000000 currentscape-1.0.7/examples/use_case/mechanisms/K_Pst.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-22 10:14:47.000000 currentscape-1.0.7/examples/use_case/mechanisms/K_Tst.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-22 10:14:47.000000 currentscape-1.0.7/examples/use_case/mechanisms/NaTg.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-06-22 10:14:47.000000 currentscape-1.0.7/examples/use_case/mechanisms/Nap_Et2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-22 10:14:47.000000 currentscape-1.0.7/examples/use_case/mechanisms/SK_E2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-22 10:14:47.000000 currentscape-1.0.7/examples/use_case/mechanisms/SKv3_1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-22 10:14:47.000000 currentscape-1.0.7/examples/use_case/mechanisms/notes.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:14:56.734471 currentscape-1.0.7/examples/use_case/morphology/
+-rw-r--r--   0 runner    (1001) docker     (123)   135189 2023-06-22 10:14:47.000000 currentscape-1.0.7/examples/use_case/morphology/dend-C231296A-P4B2_axon-C200897C-P2_-_Scale_x1.000_y0.975_z1.000.asc
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-06-22 10:14:47.000000 currentscape-1.0.7/examples/use_case/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:14:56.734471 currentscape-1.0.7/examples/use_case/python_recordings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 10:14:47.000000 currentscape-1.0.7/examples/use_case/python_recordings/.keep
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-06-22 10:14:47.000000 currentscape-1.0.7/examples/use_case/run.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      665 2023-06-22 10:14:47.000000 currentscape-1.0.7/examples/use_case/run_py.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:14:56.726471 currentscape-1.0.7/extra/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:14:56.734471 currentscape-1.0.7/extra/jjb-cells/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-22 10:14:47.000000 currentscape-1.0.7/extra/jjb-cells/cells.currentscape.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:14:56.726471 currentscape-1.0.7/extra/spack/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:14:56.726471 currentscape-1.0.7/extra/spack/var/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:14:56.726471 currentscape-1.0.7/extra/spack/var/spack/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:14:56.726471 currentscape-1.0.7/extra/spack/var/spack/repos/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:14:56.726471 currentscape-1.0.7/extra/spack/var/spack/repos/builtin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:14:56.726471 currentscape-1.0.7/extra/spack/var/spack/repos/builtin/packages/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:14:56.734471 currentscape-1.0.7/extra/spack/var/spack/repos/builtin/packages/py-currentscape/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-22 10:14:47.000000 currentscape-1.0.7/extra/spack/var/spack/repos/builtin/packages/py-currentscape/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-22 10:14:47.000000 currentscape-1.0.7/requirements_docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 10:14:56.734471 currentscape-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-06-22 10:14:47.000000 currentscape-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:14:56.734471 currentscape-1.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 10:14:47.000000 currentscape-1.0.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-22 10:14:47.000000 currentscape-1.0.7/tests/extract_bNAC_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-22 10:14:47.000000 currentscape-1.0.7/tests/test_currentscape_config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-22 10:14:47.000000 currentscape-1.0.7/tests/test_currentscape_currents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-06-22 10:14:47.000000 currentscape-1.0.7/tests/test_currentscape_dataprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-06-22 10:14:47.000000 currentscape-1.0.7/tests/test_currentscape_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-22 10:14:47.000000 currentscape-1.0.7/tests/test_currentscape_from_paper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-22 10:14:47.000000 currentscape-1.0.7/tests/test_currentscape_ions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-06-22 10:14:47.000000 currentscape-1.0.7/tests/test_currentscape_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8340 2023-06-22 10:14:47.000000 currentscape-1.0.7/tests/test_currentscape_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-22 10:14:47.000000 currentscape-1.0.7/tests/test_use_case_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-22 10:14:47.000000 currentscape-1.0.7/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-22 10:14:47.000000 currentscape-1.0.7/tox.ini
```

### Comparing `currentscape-1.0.6/.github/workflows/test.yml` & `currentscape-1.0.7/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/.pylintrc` & `currentscape-1.0.7/.pylintrc`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/.zenodo.json` & `currentscape-1.0.7/.zenodo.json`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/CHANGELOG.rst` & `currentscape-1.0.7/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/CONTRIBUTING.md` & `currentscape-1.0.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/COPYING` & `currentscape-1.0.7/COPYING`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/LICENSE.txt` & `currentscape-1.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/PKG-INFO` & `currentscape-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: currentscape
-Version: 1.0.6
+Version: 1.0.7
 Summary: Module to easily plot currentscape.
 Home-page: https://github.com/BlueBrain/Currentscape
 Author: Blue Brain Project, EPFL
 License: Apache 2.0
 Project-URL: Tracker, https://github.com/BlueBrain/Currentscape
 Project-URL: Source, https://github.com/BlueBrain/Currentscape
 Classifier: Development Status :: 4 - Beta
```

### Comparing `currentscape-1.0.6/README.rst` & `currentscape-1.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/Tutorial.rst` & `currentscape-1.0.7/Tutorial.rst`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/currentscape/__init__.py` & `currentscape-1.0.7/currentscape/__init__.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/currentscape/config_parser.py` & `currentscape-1.0.7/currentscape/config_parser.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/currentscape/currents.py` & `currentscape-1.0.7/currentscape/currents.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/currentscape/currentscape.py` & `currentscape-1.0.7/currentscape/currentscape.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/currentscape/data_processing.py` & `currentscape-1.0.7/currentscape/data_processing.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/currentscape/datasets.py` & `currentscape-1.0.7/currentscape/datasets.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/currentscape/ions.py` & `currentscape-1.0.7/currentscape/ions.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/currentscape/legends.py` & `currentscape-1.0.7/currentscape/legends.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/currentscape/mapper.py` & `currentscape-1.0.7/currentscape/mapper.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/currentscape/plotting.py` & `currentscape-1.0.7/currentscape/plotting.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/currentscape/voltages.py` & `currentscape-1.0.7/currentscape/voltages.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/currentscape.egg-info/PKG-INFO` & `currentscape-1.0.7/currentscape.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: currentscape
-Version: 1.0.6
+Version: 1.0.7
 Summary: Module to easily plot currentscape.
 Home-page: https://github.com/BlueBrain/Currentscape
 Author: Blue Brain Project, EPFL
 License: Apache 2.0
 Project-URL: Tracker, https://github.com/BlueBrain/Currentscape
 Project-URL: Source, https://github.com/BlueBrain/Currentscape
 Classifier: Development Status :: 4 - Beta
```

### Comparing `currentscape-1.0.6/currentscape.egg-info/SOURCES.txt` & `currentscape-1.0.7/currentscape.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/doc/Makefile` & `currentscape-1.0.7/doc/Makefile`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/doc/source/conf.py` & `currentscape-1.0.7/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/doc/source/images/plot.png` & `currentscape-1.0.7/doc/source/images/plot.png`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/doc/source/images/quickstart_plot.png` & `currentscape-1.0.7/doc/source/images/quickstart_plot.png`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/examples/original_paper_plot/LICENSE_CC0-1.0` & `currentscape-1.0.7/examples/original_paper_plot/LICENSE_CC0-1.0`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/examples/original_paper_plot/config.json` & `currentscape-1.0.7/examples/original_paper_plot/config.json`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/examples/original_paper_plot/get_currents.py` & `currentscape-1.0.7/examples/original_paper_plot/get_currents.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/examples/original_paper_plot/integrate_single_compartment_and_plot_currentscape.py` & `currentscape-1.0.7/examples/original_paper_plot/integrate_single_compartment_and_plot_currentscape.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/examples/original_paper_plot/parameters-and-initial-conditions/model-A-name-HZFTSB.txt` & `currentscape-1.0.7/examples/original_paper_plot/parameters-and-initial-conditions/model-A-name-HZFTSB.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/examples/original_paper_plot/parameters-and-initial-conditions/model-B-name-8XCUQE.txt` & `currentscape-1.0.7/examples/original_paper_plot/parameters-and-initial-conditions/model-B-name-8XCUQE.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/examples/original_paper_plot/parameters-and-initial-conditions/model-C-name-C1L1R0.txt` & `currentscape-1.0.7/examples/original_paper_plot/parameters-and-initial-conditions/model-C-name-C1L1R0.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/examples/original_paper_plot/parameters-and-initial-conditions/model-D-name-KI47XV.txt` & `currentscape-1.0.7/examples/original_paper_plot/parameters-and-initial-conditions/model-D-name-KI47XV.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/examples/original_paper_plot/parameters-and-initial-conditions/model-E-name-OG1RE2.txt` & `currentscape-1.0.7/examples/original_paper_plot/parameters-and-initial-conditions/model-E-name-OG1RE2.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/examples/original_paper_plot/parameters-and-initial-conditions/model-F-name-B7S21N.txt` & `currentscape-1.0.7/examples/original_paper_plot/parameters-and-initial-conditions/model-F-name-B7S21N.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/examples/original_paper_plot/parameters-and-initial-conditions/model-FIG2-name-1BLGMA.txt` & `currentscape-1.0.7/examples/original_paper_plot/parameters-and-initial-conditions/model-FIG2-name-1BLGMA.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/examples/original_paper_plot/parameters-and-initial-conditions/model-FIG3-name-VVECT5.txt` & `currentscape-1.0.7/examples/original_paper_plot/parameters-and-initial-conditions/model-FIG3-name-VVECT5.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/examples/original_paper_plot/single_compartment.py` & `currentscape-1.0.7/examples/original_paper_plot/single_compartment.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/examples/use_case/LICENSE.txt` & `currentscape-1.0.7/examples/use_case/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/examples/use_case/LICENSE_CC-BY-CA-SA-4.0` & `currentscape-1.0.7/examples/use_case/LICENSE_CC-BY-CA-SA-4.0`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/examples/use_case/config/params/final.json` & `currentscape-1.0.7/examples/use_case/config/params/final.json`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/examples/use_case/config/params/pyr.json` & `currentscape-1.0.7/examples/use_case/config/params/pyr.json`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/examples/use_case/mechanisms/CaDynamics_DC0.mod` & `currentscape-1.0.7/examples/use_case/mechanisms/CaDynamics_DC0.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/examples/use_case/mechanisms/Ca_HVA2.mod` & `currentscape-1.0.7/examples/use_case/mechanisms/Ca_HVA2.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/examples/use_case/mechanisms/Ca_LVAst.mod` & `currentscape-1.0.7/examples/use_case/mechanisms/Ca_LVAst.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/examples/use_case/mechanisms/Ih.mod` & `currentscape-1.0.7/examples/use_case/mechanisms/Ih.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/examples/use_case/mechanisms/K_Pst.mod` & `currentscape-1.0.7/examples/use_case/mechanisms/K_Pst.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/examples/use_case/mechanisms/K_Tst.mod` & `currentscape-1.0.7/examples/use_case/mechanisms/K_Tst.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/examples/use_case/mechanisms/NaTg.mod` & `currentscape-1.0.7/examples/use_case/mechanisms/NaTg.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/examples/use_case/mechanisms/Nap_Et2.mod` & `currentscape-1.0.7/examples/use_case/mechanisms/Nap_Et2.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/examples/use_case/mechanisms/SK_E2.mod` & `currentscape-1.0.7/examples/use_case/mechanisms/SK_E2.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/examples/use_case/mechanisms/SKv3_1.mod` & `currentscape-1.0.7/examples/use_case/mechanisms/SKv3_1.mod`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/examples/use_case/mechanisms/notes.txt` & `currentscape-1.0.7/examples/use_case/mechanisms/notes.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/examples/use_case/morphology/dend-C231296A-P4B2_axon-C200897C-P2_-_Scale_x1.000_y0.975_z1.000.asc` & `currentscape-1.0.7/examples/use_case/morphology/dend-C231296A-P4B2_axon-C200897C-P2_-_Scale_x1.000_y0.975_z1.000.asc`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/examples/use_case/plot.py` & `currentscape-1.0.7/examples/use_case/plot.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/examples/use_case/run.py` & `currentscape-1.0.7/examples/use_case/run.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/examples/use_case/run_py.sh` & `currentscape-1.0.7/examples/use_case/run_py.sh`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/extra/spack/var/spack/repos/builtin/packages/py-currentscape/package.py` & `currentscape-1.0.7/extra/spack/var/spack/repos/builtin/packages/py-currentscape/package.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/requirements_docs.txt` & `currentscape-1.0.7/requirements_docs.txt`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/setup.py` & `currentscape-1.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/tests/extract_bNAC_config.json` & `currentscape-1.0.7/tests/extract_bNAC_config.json`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/tests/test_currentscape_config_parser.py` & `currentscape-1.0.7/tests/test_currentscape_config_parser.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/tests/test_currentscape_currents.py` & `currentscape-1.0.7/tests/test_currentscape_currents.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/tests/test_currentscape_dataprocessing.py` & `currentscape-1.0.7/tests/test_currentscape_dataprocessing.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/tests/test_currentscape_datasets.py` & `currentscape-1.0.7/tests/test_currentscape_datasets.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/tests/test_currentscape_from_paper.py` & `currentscape-1.0.7/tests/test_currentscape_from_paper.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/tests/test_currentscape_ions.py` & `currentscape-1.0.7/tests/test_currentscape_ions.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/tests/test_currentscape_mapper.py` & `currentscape-1.0.7/tests/test_currentscape_mapper.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/tests/test_currentscape_plotting.py` & `currentscape-1.0.7/tests/test_currentscape_plotting.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/tests/test_use_case_example.py` & `currentscape-1.0.7/tests/test_use_case_example.py`

 * *Files identical despite different names*

### Comparing `currentscape-1.0.6/tox.ini` & `currentscape-1.0.7/tox.ini`

 * *Files identical despite different names*

