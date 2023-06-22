# Comparing `tmp/climate_categories-0.9.1.tar.gz` & `tmp/climate_categories-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climate_categories-0.9.1.tar", last modified: Thu Jun 15 13:50:35 2023, max compression
+gzip compressed data, was "climate_categories-0.9.2.tar", last modified: Thu Jun 22 11:11:18 2023, max compression
```

## Comparing `climate_categories-0.9.1.tar` & `climate_categories-0.9.2.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-06-15 13:50:35.933570 climate_categories-0.9.1/
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-06-15 13:50:35.929570 climate_categories-0.9.1/.github/
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-06-15 13:50:35.929570 climate_categories-0.9.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      671 2023-04-26 09:04:13.000000 climate_categories-0.9.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      548 2023-04-26 09:04:13.000000 climate_categories-0.9.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      571 2023-04-26 09:04:13.000000 climate_categories-0.9.1/.github/ISSUE_TEMPLATE/new_categorization.md
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      369 2023-04-26 13:19:45.000000 climate_categories-0.9.1/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-06-15 13:50:35.929570 climate_categories-0.9.1/.github/workflows/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      963 2023-04-26 11:23:54.000000 climate_categories-0.9.1/.github/workflows/ci.yml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1331 2023-04-26 11:23:54.000000 climate_categories-0.9.1/.gitignore
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1253 2023-06-13 09:03:12.000000 climate_categories-0.9.1/.pre-commit-config.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      297 2023-04-26 13:26:25.000000 climate_categories-0.9.1/.readthedocs.yml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       38 2023-04-26 09:04:13.000000 climate_categories-0.9.1/.sourcery.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      216 2023-04-26 14:19:11.000000 climate_categories-0.9.1/AUTHORS.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5357 2023-06-15 13:49:02.000000 climate_categories-0.9.1/CHANGELOG.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5446 2023-04-26 11:23:54.000000 climate_categories-0.9.1/CONTRIBUTING.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      696 2023-04-26 14:19:11.000000 climate_categories-0.9.1/LICENSE
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3280 2023-06-14 15:10:21.000000 climate_categories-0.9.1/Makefile
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     9834 2023-06-15 13:50:35.933570 climate_categories-0.9.1/PKG-INFO
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3460 2023-06-15 13:50:20.000000 climate_categories-0.9.1/README.rst
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-06-15 13:50:35.929570 climate_categories-0.9.1/climate_categories/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1978 2023-06-15 13:48:49.000000 climate_categories-0.9.1/climate_categories/__init__.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    43254 2023-05-23 15:38:02.000000 climate_categories-0.9.1/climate_categories/_categories.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    47235 2023-04-26 12:57:44.000000 climate_categories-0.9.1/climate_categories/_conversions.py
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-06-15 13:50:35.933570 climate_categories-0.9.1/climate_categories/data/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    48820 2023-04-26 13:51:54.000000 climate_categories-0.9.1/climate_categories/data/BURDI.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    39603 2023-04-26 13:51:50.000000 climate_categories-0.9.1/climate_categories/data/BURDI.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    91320 2023-04-26 13:52:03.000000 climate_categories-0.9.1/climate_categories/data/BURDI_class.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    64321 2023-04-26 13:51:56.000000 climate_categories-0.9.1/climate_categories/data/BURDI_class.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    84030 2023-04-26 13:49:12.000000 climate_categories-0.9.1/climate_categories/data/CRF1999.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    69834 2023-04-26 13:49:07.000000 climate_categories-0.9.1/climate_categories/data/CRF1999.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   172563 2023-04-26 13:59:42.000000 climate_categories-0.9.1/climate_categories/data/CRF2013.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   136709 2023-04-26 13:59:42.000000 climate_categories-0.9.1/climate_categories/data/CRF2013.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   213803 2023-04-26 13:59:42.000000 climate_categories-0.9.1/climate_categories/data/CRF2013_2021.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   165299 2023-04-26 13:59:42.000000 climate_categories-0.9.1/climate_categories/data/CRF2013_2021.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   214940 2023-04-26 13:59:42.000000 climate_categories-0.9.1/climate_categories/data/CRF2013_2022.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   165976 2023-04-26 13:59:42.000000 climate_categories-0.9.1/climate_categories/data/CRF2013_2022.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   215236 2023-04-26 13:59:42.000000 climate_categories-0.9.1/climate_categories/data/CRF2013_2023.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   166217 2023-04-26 13:59:42.000000 climate_categories-0.9.1/climate_categories/data/CRF2013_2023.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    85443 2023-04-26 13:51:04.000000 climate_categories-0.9.1/climate_categories/data/CRFDI.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    68686 2023-04-26 13:50:55.000000 climate_categories-0.9.1/climate_categories/data/CRFDI.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   252079 2023-04-26 13:51:45.000000 climate_categories-0.9.1/climate_categories/data/CRFDI_class.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   172924 2023-04-26 13:51:08.000000 climate_categories-0.9.1/climate_categories/data/CRFDI_class.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     2039 2023-04-26 13:48:45.000000 climate_categories-0.9.1/climate_categories/data/GCB.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1795 2023-04-26 09:04:13.000000 climate_categories-0.9.1/climate_categories/data/GCB.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    60150 2023-04-26 13:49:07.000000 climate_categories-0.9.1/climate_categories/data/IPCC1996.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    51928 2023-04-26 13:49:05.000000 climate_categories-0.9.1/climate_categories/data/IPCC1996.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   146256 2023-04-26 13:48:54.000000 climate_categories-0.9.1/climate_categories/data/IPCC2006.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   126862 2023-04-26 13:48:48.000000 climate_categories-0.9.1/climate_categories/data/IPCC2006.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   149225 2023-04-26 13:49:01.000000 climate_categories-0.9.1/climate_categories/data/IPCC2006_PRIMAP.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   128959 2023-04-26 13:48:55.000000 climate_categories-0.9.1/climate_categories/data/IPCC2006_PRIMAP.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    61742 2023-06-15 13:48:28.000000 climate_categories-0.9.1/climate_categories/data/ISO3.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    40093 2023-06-15 13:48:28.000000 climate_categories-0.9.1/climate_categories/data/ISO3.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    24803 2023-04-26 13:59:42.000000 climate_categories-0.9.1/climate_categories/data/RCMIP.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    18549 2023-04-26 13:59:42.000000 climate_categories-0.9.1/climate_categories/data/RCMIP.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-26 09:04:13.000000 climate_categories-0.9.1/climate_categories/data/__init__.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3761 2023-04-26 09:06:11.000000 climate_categories-0.9.1/climate_categories/data/conversion.IPCC1996.IPCC2006.csv
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    32498 2023-04-26 13:50:50.000000 climate_categories-0.9.1/climate_categories/data/gas.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    23635 2023-04-26 13:50:49.000000 climate_categories-0.9.1/climate_categories/data/gas.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-23 14:12:58.000000 climate_categories-0.9.1/climate_categories/py.typed
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      304 2023-04-26 11:23:54.000000 climate_categories-0.9.1/climate_categories/search.py
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-06-15 13:50:35.933570 climate_categories-0.9.1/climate_categories/tests/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       48 2023-04-26 09:04:13.000000 climate_categories-0.9.1/climate_categories/tests/__init__.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3795 2023-04-26 11:23:55.000000 climate_categories-0.9.1/climate_categories/tests/conftest.py
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-06-15 13:50:35.933570 climate_categories-0.9.1/climate_categories/tests/data/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-26 10:17:34.000000 climate_categories-0.9.1/climate_categories/tests/data/__init__.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      359 2023-04-26 09:06:11.000000 climate_categories-0.9.1/climate_categories/tests/data/broken_conversion_not_allowed.csv
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      359 2023-04-26 09:06:11.000000 climate_categories-0.9.1/climate_categories/tests/data/broken_conversion_not_existing.csv
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1387 2023-04-26 09:04:13.000000 climate_categories-0.9.1/climate_categories/tests/data/broken_hierarchical_categorization.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      705 2023-04-26 09:04:13.000000 climate_categories-0.9.1/climate_categories/tests/data/broken_simple_categorization.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      350 2023-04-26 09:06:11.000000 climate_categories-0.9.1/climate_categories/tests/data/good_conversion.csv
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      650 2023-04-26 09:04:13.000000 climate_categories-0.9.1/climate_categories/tests/data/good_conversion_A.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      341 2023-04-26 09:04:13.000000 climate_categories-0.9.1/climate_categories/tests/data/good_conversion_B.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      372 2023-04-26 09:04:13.000000 climate_categories-0.9.1/climate_categories/tests/data/good_conversion_aux1.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      349 2023-04-26 09:04:13.000000 climate_categories-0.9.1/climate_categories/tests/data/good_conversion_aux2.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      350 2023-04-26 09:06:11.000000 climate_categories-0.9.1/climate_categories/tests/data/good_conversion_reversed.csv
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1387 2023-04-26 09:04:13.000000 climate_categories-0.9.1/climate_categories/tests/data/hierarchical_categorization.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      702 2023-04-26 09:04:13.000000 climate_categories-0.9.1/climate_categories/tests/data/simple_categorization.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1665 2023-04-26 09:04:13.000000 climate_categories-0.9.1/climate_categories/tests/examples.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    21970 2023-05-15 16:28:37.000000 climate_categories-0.9.1/climate_categories/tests/test_climate_categories.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    14271 2023-04-26 11:23:55.000000 climate_categories-0.9.1/climate_categories/tests/test_conversions.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1205 2023-04-26 11:23:54.000000 climate_categories-0.9.1/climate_categories/tests/test_crf.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      769 2023-04-26 09:04:13.000000 climate_categories-0.9.1/climate_categories/tests/test_di.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      508 2023-04-26 09:04:13.000000 climate_categories-0.9.1/climate_categories/tests/test_gas.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1296 2023-04-26 09:04:13.000000 climate_categories-0.9.1/climate_categories/tests/test_ipcc.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1708 2023-06-15 13:48:28.000000 climate_categories-0.9.1/climate_categories/tests/test_iso3.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     7703 2023-04-26 09:04:13.000000 climate_categories-0.9.1/climate_categories/tests/test_overcounting.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      596 2023-04-26 09:04:13.000000 climate_categories-0.9.1/climate_categories/tests/test_primap.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      305 2023-04-26 09:06:11.000000 climate_categories-0.9.1/climate_categories/tests/test_rcmip.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      649 2023-04-26 11:23:54.000000 climate_categories-0.9.1/climate_categories/tests/test_search.py
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-06-15 13:50:35.929570 climate_categories-0.9.1/climate_categories.egg-info/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     9834 2023-06-15 13:50:35.000000 climate_categories-0.9.1/climate_categories.egg-info/PKG-INFO
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     4157 2023-06-15 13:50:35.000000 climate_categories-0.9.1/climate_categories.egg-info/SOURCES.txt
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        1 2023-06-15 13:50:35.000000 climate_categories-0.9.1/climate_categories.egg-info/dependency_links.txt
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      307 2023-06-15 13:50:35.000000 climate_categories-0.9.1/climate_categories.egg-info/requires.txt
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       19 2023-06-15 13:50:35.000000 climate_categories-0.9.1/climate_categories.egg-info/top_level.txt
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      130 2023-04-26 09:04:13.000000 climate_categories-0.9.1/codecov.yml
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-06-15 13:50:35.933570 climate_categories-0.9.1/data_generation/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       62 2023-04-26 09:06:11.000000 climate_categories-0.9.1/data_generation/.gitignore
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5819 2023-04-26 13:44:45.000000 climate_categories-0.9.1/data_generation/BURDI.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3177 2023-04-26 13:44:45.000000 climate_categories-0.9.1/data_generation/BURDI_class.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    17598 2023-04-26 13:44:45.000000 climate_categories-0.9.1/data_generation/CRF1999.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    65761 2023-04-26 13:44:45.000000 climate_categories-0.9.1/data_generation/CRF2013.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    30906 2023-04-26 13:44:45.000000 climate_categories-0.9.1/data_generation/CRF2013_2021.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    31721 2023-04-26 13:44:45.000000 climate_categories-0.9.1/data_generation/CRF2013_2022.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    32225 2023-04-26 13:44:45.000000 climate_categories-0.9.1/data_generation/CRF2013_2023.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5318 2023-04-26 13:44:45.000000 climate_categories-0.9.1/data_generation/CRFDI.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5232 2023-04-26 13:44:45.000000 climate_categories-0.9.1/data_generation/CRFDI_class.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    11562 2023-04-26 13:44:45.000000 climate_categories-0.9.1/data_generation/IPCC1996.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     8947 2023-04-26 13:44:45.000000 climate_categories-0.9.1/data_generation/IPCC2006.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     4254 2023-04-26 13:44:45.000000 climate_categories-0.9.1/data_generation/IPCC2006_PRIMAP.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    14792 2023-06-15 13:48:28.000000 climate_categories-0.9.1/data_generation/ISO3.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     8134 2023-04-26 13:44:45.000000 climate_categories-0.9.1/data_generation/RCMIP.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      272 2023-04-26 13:44:45.000000 climate_categories-0.9.1/data_generation/convert_yaml_to_python.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3318 2023-04-26 13:44:45.000000 climate_categories-0.9.1/data_generation/gas.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1082 2023-04-26 13:44:45.000000 climate_categories-0.9.1/data_generation/utils.py
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-06-15 13:50:35.933570 climate_categories-0.9.1/docs/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      631 2023-04-26 09:04:13.000000 climate_categories-0.9.1/docs/Makefile
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      241 2023-04-26 09:04:13.000000 climate_categories-0.9.1/docs/api.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       30 2023-04-26 09:04:13.000000 climate_categories-0.9.1/docs/changelog.rst
--rwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)     5232 2023-05-10 09:47:08.000000 climate_categories-0.9.1/docs/conf.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       33 2023-04-26 09:04:13.000000 climate_categories-0.9.1/docs/contributing.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      337 2023-04-26 09:04:13.000000 climate_categories-0.9.1/docs/credits.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     8179 2023-05-10 10:01:49.000000 climate_categories-0.9.1/docs/data.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      325 2023-04-26 09:04:13.000000 climate_categories-0.9.1/docs/index.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1209 2023-04-26 09:04:13.000000 climate_categories-0.9.1/docs/installation.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      780 2023-04-26 09:04:13.000000 climate_categories-0.9.1/docs/make.bat
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       27 2023-04-26 09:04:13.000000 climate_categories-0.9.1/docs/readme.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       21 2023-05-10 09:48:15.000000 climate_categories-0.9.1/docs/requirements.txt
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    18889 2023-05-15 16:28:37.000000 climate_categories-0.9.1/docs/usage.ipynb
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      328 2023-04-26 12:59:50.000000 climate_categories-0.9.1/pyproject.toml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        2 2023-04-26 09:04:13.000000 climate_categories-0.9.1/requirements.txt
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        7 2023-04-26 09:04:13.000000 climate_categories-0.9.1/requirements_dev.txt
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1658 2023-06-15 13:50:35.933570 climate_categories-0.9.1/setup.cfg
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       61 2023-04-26 09:08:24.000000 climate_categories-0.9.1/setup.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1381 2023-06-15 13:48:49.000000 climate_categories-0.9.1/tbump.toml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      379 2023-04-26 11:23:54.000000 climate_categories-0.9.1/tox.ini
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      773 2023-04-26 09:04:13.000000 climate_categories-0.9.1/update_changelog.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1181 2023-04-26 11:23:54.000000 climate_categories-0.9.1/update_citation_info.py
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-06-22 11:11:18.844593 climate_categories-0.9.2/
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-06-22 11:11:18.836593 climate_categories-0.9.2/.github/
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-06-22 11:11:18.836593 climate_categories-0.9.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      671 2023-04-26 09:04:13.000000 climate_categories-0.9.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      548 2023-04-26 09:04:13.000000 climate_categories-0.9.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      571 2023-04-26 09:04:13.000000 climate_categories-0.9.2/.github/ISSUE_TEMPLATE/new_categorization.md
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      369 2023-04-26 13:19:45.000000 climate_categories-0.9.2/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-06-22 11:11:18.836593 climate_categories-0.9.2/.github/workflows/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      963 2023-04-26 11:23:54.000000 climate_categories-0.9.2/.github/workflows/ci.yml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1331 2023-04-26 11:23:54.000000 climate_categories-0.9.2/.gitignore
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1253 2023-06-13 09:03:12.000000 climate_categories-0.9.2/.pre-commit-config.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      297 2023-04-26 13:26:25.000000 climate_categories-0.9.2/.readthedocs.yml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       38 2023-04-26 09:04:13.000000 climate_categories-0.9.2/.sourcery.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      216 2023-04-26 14:19:11.000000 climate_categories-0.9.2/AUTHORS.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5621 2023-06-22 11:08:17.000000 climate_categories-0.9.2/CHANGELOG.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5446 2023-04-26 11:23:54.000000 climate_categories-0.9.2/CONTRIBUTING.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      696 2023-04-26 14:19:11.000000 climate_categories-0.9.2/LICENSE
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3280 2023-06-14 15:10:21.000000 climate_categories-0.9.2/Makefile
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    10098 2023-06-22 11:11:18.844593 climate_categories-0.9.2/PKG-INFO
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3460 2023-06-22 11:10:56.000000 climate_categories-0.9.2/README.rst
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-06-22 11:11:18.836593 climate_categories-0.9.2/climate_categories/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1978 2023-06-22 11:08:05.000000 climate_categories-0.9.2/climate_categories/__init__.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    43254 2023-05-23 15:38:02.000000 climate_categories-0.9.2/climate_categories/_categories.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    47235 2023-04-26 12:57:44.000000 climate_categories-0.9.2/climate_categories/_conversions.py
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-06-22 11:11:18.840593 climate_categories-0.9.2/climate_categories/data/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    48820 2023-04-26 13:51:54.000000 climate_categories-0.9.2/climate_categories/data/BURDI.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    39603 2023-04-26 13:51:50.000000 climate_categories-0.9.2/climate_categories/data/BURDI.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    91320 2023-04-26 13:52:03.000000 climate_categories-0.9.2/climate_categories/data/BURDI_class.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    64321 2023-04-26 13:51:56.000000 climate_categories-0.9.2/climate_categories/data/BURDI_class.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    84030 2023-04-26 13:49:12.000000 climate_categories-0.9.2/climate_categories/data/CRF1999.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    69834 2023-04-26 13:49:07.000000 climate_categories-0.9.2/climate_categories/data/CRF1999.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   172563 2023-04-26 13:59:42.000000 climate_categories-0.9.2/climate_categories/data/CRF2013.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   136709 2023-04-26 13:59:42.000000 climate_categories-0.9.2/climate_categories/data/CRF2013.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   213803 2023-04-26 13:59:42.000000 climate_categories-0.9.2/climate_categories/data/CRF2013_2021.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   165299 2023-04-26 13:59:42.000000 climate_categories-0.9.2/climate_categories/data/CRF2013_2021.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   214940 2023-04-26 13:59:42.000000 climate_categories-0.9.2/climate_categories/data/CRF2013_2022.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   165976 2023-04-26 13:59:42.000000 climate_categories-0.9.2/climate_categories/data/CRF2013_2022.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   215236 2023-04-26 13:59:42.000000 climate_categories-0.9.2/climate_categories/data/CRF2013_2023.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   166217 2023-04-26 13:59:42.000000 climate_categories-0.9.2/climate_categories/data/CRF2013_2023.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    85443 2023-04-26 13:51:04.000000 climate_categories-0.9.2/climate_categories/data/CRFDI.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    68686 2023-04-26 13:50:55.000000 climate_categories-0.9.2/climate_categories/data/CRFDI.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   252079 2023-04-26 13:51:45.000000 climate_categories-0.9.2/climate_categories/data/CRFDI_class.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   172924 2023-04-26 13:51:08.000000 climate_categories-0.9.2/climate_categories/data/CRFDI_class.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     2039 2023-04-26 13:48:45.000000 climate_categories-0.9.2/climate_categories/data/GCB.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1795 2023-04-26 09:04:13.000000 climate_categories-0.9.2/climate_categories/data/GCB.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    60150 2023-04-26 13:49:07.000000 climate_categories-0.9.2/climate_categories/data/IPCC1996.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    51928 2023-04-26 13:49:05.000000 climate_categories-0.9.2/climate_categories/data/IPCC1996.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   146256 2023-04-26 13:48:54.000000 climate_categories-0.9.2/climate_categories/data/IPCC2006.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   126862 2023-04-26 13:48:48.000000 climate_categories-0.9.2/climate_categories/data/IPCC2006.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   149225 2023-04-26 13:49:01.000000 climate_categories-0.9.2/climate_categories/data/IPCC2006_PRIMAP.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   128959 2023-04-26 13:48:55.000000 climate_categories-0.9.2/climate_categories/data/IPCC2006_PRIMAP.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    67170 2023-06-22 11:02:00.000000 climate_categories-0.9.2/climate_categories/data/ISO3.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    42483 2023-06-22 11:01:56.000000 climate_categories-0.9.2/climate_categories/data/ISO3.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    24803 2023-04-26 13:59:42.000000 climate_categories-0.9.2/climate_categories/data/RCMIP.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    18549 2023-04-26 13:59:42.000000 climate_categories-0.9.2/climate_categories/data/RCMIP.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-26 09:04:13.000000 climate_categories-0.9.2/climate_categories/data/__init__.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3761 2023-04-26 09:06:11.000000 climate_categories-0.9.2/climate_categories/data/conversion.IPCC1996.IPCC2006.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    32498 2023-04-26 13:50:50.000000 climate_categories-0.9.2/climate_categories/data/gas.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    23635 2023-04-26 13:50:49.000000 climate_categories-0.9.2/climate_categories/data/gas.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-23 14:12:58.000000 climate_categories-0.9.2/climate_categories/py.typed
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      304 2023-04-26 11:23:54.000000 climate_categories-0.9.2/climate_categories/search.py
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-06-22 11:11:18.840593 climate_categories-0.9.2/climate_categories/tests/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       48 2023-04-26 09:04:13.000000 climate_categories-0.9.2/climate_categories/tests/__init__.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3795 2023-04-26 11:23:55.000000 climate_categories-0.9.2/climate_categories/tests/conftest.py
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-06-22 11:11:18.840593 climate_categories-0.9.2/climate_categories/tests/data/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-26 10:17:34.000000 climate_categories-0.9.2/climate_categories/tests/data/__init__.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      359 2023-04-26 09:06:11.000000 climate_categories-0.9.2/climate_categories/tests/data/broken_conversion_not_allowed.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      359 2023-04-26 09:06:11.000000 climate_categories-0.9.2/climate_categories/tests/data/broken_conversion_not_existing.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1387 2023-04-26 09:04:13.000000 climate_categories-0.9.2/climate_categories/tests/data/broken_hierarchical_categorization.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      705 2023-04-26 09:04:13.000000 climate_categories-0.9.2/climate_categories/tests/data/broken_simple_categorization.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      350 2023-04-26 09:06:11.000000 climate_categories-0.9.2/climate_categories/tests/data/good_conversion.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      650 2023-04-26 09:04:13.000000 climate_categories-0.9.2/climate_categories/tests/data/good_conversion_A.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      341 2023-04-26 09:04:13.000000 climate_categories-0.9.2/climate_categories/tests/data/good_conversion_B.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      372 2023-04-26 09:04:13.000000 climate_categories-0.9.2/climate_categories/tests/data/good_conversion_aux1.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      349 2023-04-26 09:04:13.000000 climate_categories-0.9.2/climate_categories/tests/data/good_conversion_aux2.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      350 2023-04-26 09:06:11.000000 climate_categories-0.9.2/climate_categories/tests/data/good_conversion_reversed.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1387 2023-04-26 09:04:13.000000 climate_categories-0.9.2/climate_categories/tests/data/hierarchical_categorization.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      702 2023-04-26 09:04:13.000000 climate_categories-0.9.2/climate_categories/tests/data/simple_categorization.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1665 2023-04-26 09:04:13.000000 climate_categories-0.9.2/climate_categories/tests/examples.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    21970 2023-05-15 16:28:37.000000 climate_categories-0.9.2/climate_categories/tests/test_climate_categories.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    14271 2023-04-26 11:23:55.000000 climate_categories-0.9.2/climate_categories/tests/test_conversions.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1205 2023-04-26 11:23:54.000000 climate_categories-0.9.2/climate_categories/tests/test_crf.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      769 2023-04-26 09:04:13.000000 climate_categories-0.9.2/climate_categories/tests/test_di.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      508 2023-04-26 09:04:13.000000 climate_categories-0.9.2/climate_categories/tests/test_gas.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1296 2023-04-26 09:04:13.000000 climate_categories-0.9.2/climate_categories/tests/test_ipcc.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1999 2023-06-22 10:58:07.000000 climate_categories-0.9.2/climate_categories/tests/test_iso3.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     7703 2023-04-26 09:04:13.000000 climate_categories-0.9.2/climate_categories/tests/test_overcounting.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      596 2023-04-26 09:04:13.000000 climate_categories-0.9.2/climate_categories/tests/test_primap.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      305 2023-04-26 09:06:11.000000 climate_categories-0.9.2/climate_categories/tests/test_rcmip.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      649 2023-04-26 11:23:54.000000 climate_categories-0.9.2/climate_categories/tests/test_search.py
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-06-22 11:11:18.836593 climate_categories-0.9.2/climate_categories.egg-info/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    10098 2023-06-22 11:11:18.000000 climate_categories-0.9.2/climate_categories.egg-info/PKG-INFO
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     4157 2023-06-22 11:11:18.000000 climate_categories-0.9.2/climate_categories.egg-info/SOURCES.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        1 2023-06-22 11:11:18.000000 climate_categories-0.9.2/climate_categories.egg-info/dependency_links.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      307 2023-06-22 11:11:18.000000 climate_categories-0.9.2/climate_categories.egg-info/requires.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       19 2023-06-22 11:11:18.000000 climate_categories-0.9.2/climate_categories.egg-info/top_level.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      130 2023-04-26 09:04:13.000000 climate_categories-0.9.2/codecov.yml
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-06-22 11:11:18.844593 climate_categories-0.9.2/data_generation/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       62 2023-04-26 09:06:11.000000 climate_categories-0.9.2/data_generation/.gitignore
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5819 2023-04-26 13:44:45.000000 climate_categories-0.9.2/data_generation/BURDI.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3177 2023-04-26 13:44:45.000000 climate_categories-0.9.2/data_generation/BURDI_class.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    17598 2023-04-26 13:44:45.000000 climate_categories-0.9.2/data_generation/CRF1999.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    65761 2023-04-26 13:44:45.000000 climate_categories-0.9.2/data_generation/CRF2013.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    30906 2023-04-26 13:44:45.000000 climate_categories-0.9.2/data_generation/CRF2013_2021.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    31721 2023-04-26 13:44:45.000000 climate_categories-0.9.2/data_generation/CRF2013_2022.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    32225 2023-04-26 13:44:45.000000 climate_categories-0.9.2/data_generation/CRF2013_2023.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5318 2023-04-26 13:44:45.000000 climate_categories-0.9.2/data_generation/CRFDI.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5232 2023-04-26 13:44:45.000000 climate_categories-0.9.2/data_generation/CRFDI_class.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    11562 2023-04-26 13:44:45.000000 climate_categories-0.9.2/data_generation/IPCC1996.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     8947 2023-04-26 13:44:45.000000 climate_categories-0.9.2/data_generation/IPCC2006.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     4254 2023-04-26 13:44:45.000000 climate_categories-0.9.2/data_generation/IPCC2006_PRIMAP.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    14920 2023-06-22 11:01:52.000000 climate_categories-0.9.2/data_generation/ISO3.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     8134 2023-04-26 13:44:45.000000 climate_categories-0.9.2/data_generation/RCMIP.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      272 2023-04-26 13:44:45.000000 climate_categories-0.9.2/data_generation/convert_yaml_to_python.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3318 2023-04-26 13:44:45.000000 climate_categories-0.9.2/data_generation/gas.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1082 2023-04-26 13:44:45.000000 climate_categories-0.9.2/data_generation/utils.py
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-06-22 11:11:18.844593 climate_categories-0.9.2/docs/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      631 2023-04-26 09:04:13.000000 climate_categories-0.9.2/docs/Makefile
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      241 2023-04-26 09:04:13.000000 climate_categories-0.9.2/docs/api.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       30 2023-04-26 09:04:13.000000 climate_categories-0.9.2/docs/changelog.rst
+-rwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)     5232 2023-05-10 09:47:08.000000 climate_categories-0.9.2/docs/conf.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       33 2023-04-26 09:04:13.000000 climate_categories-0.9.2/docs/contributing.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      337 2023-04-26 09:04:13.000000 climate_categories-0.9.2/docs/credits.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     8179 2023-05-10 10:01:49.000000 climate_categories-0.9.2/docs/data.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      325 2023-04-26 09:04:13.000000 climate_categories-0.9.2/docs/index.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1209 2023-04-26 09:04:13.000000 climate_categories-0.9.2/docs/installation.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      780 2023-04-26 09:04:13.000000 climate_categories-0.9.2/docs/make.bat
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       27 2023-04-26 09:04:13.000000 climate_categories-0.9.2/docs/readme.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       21 2023-05-10 09:48:15.000000 climate_categories-0.9.2/docs/requirements.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    18889 2023-05-15 16:28:37.000000 climate_categories-0.9.2/docs/usage.ipynb
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      328 2023-04-26 12:59:50.000000 climate_categories-0.9.2/pyproject.toml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        2 2023-04-26 09:04:13.000000 climate_categories-0.9.2/requirements.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        7 2023-04-26 09:04:13.000000 climate_categories-0.9.2/requirements_dev.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1658 2023-06-22 11:11:18.844593 climate_categories-0.9.2/setup.cfg
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       61 2023-04-26 09:08:24.000000 climate_categories-0.9.2/setup.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1381 2023-06-22 11:08:05.000000 climate_categories-0.9.2/tbump.toml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      379 2023-04-26 11:23:54.000000 climate_categories-0.9.2/tox.ini
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      773 2023-04-26 09:04:13.000000 climate_categories-0.9.2/update_changelog.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1181 2023-04-26 11:23:54.000000 climate_categories-0.9.2/update_citation_info.py
```

### Comparing `climate_categories-0.9.1/.github/ISSUE_TEMPLATE/bug_report.md` & `climate_categories-0.9.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/.github/ISSUE_TEMPLATE/feature_request.md` & `climate_categories-0.9.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/.github/ISSUE_TEMPLATE/new_categorization.md` & `climate_categories-0.9.2/.github/ISSUE_TEMPLATE/new_categorization.md`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/.github/workflows/ci.yml` & `climate_categories-0.9.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/.gitignore` & `climate_categories-0.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/.pre-commit-config.yaml` & `climate_categories-0.9.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/CHANGELOG.rst` & `climate_categories-0.9.2/CHANGELOG.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 =========
 Changelog
 =========
 
+0.9.2 (2023-06-22)
+------------------
+* ISO3: Add all parties to the UNFCCC as direct children of UNFCCC as first set of
+  children. That way, it is easy to ergonomically get all parties to the UNFCCC without
+  adding up Annex-I and Non-Annex-I parties manually.
+
 0.9.1 (2023-06-15)
 ------------------
 * Add AOSIS country group to ISO3 categorization.
 
 0.9.0 (2023-06-14)
 ------------------
 * Add ISO3 terminology for countries, areas, and country groups including UNFCCC
```

### Comparing `climate_categories-0.9.1/CONTRIBUTING.rst` & `climate_categories-0.9.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/LICENSE` & `climate_categories-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/Makefile` & `climate_categories-0.9.2/Makefile`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/PKG-INFO` & `climate_categories-0.9.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climate_categories
-Version: 0.9.1
+Version: 0.9.2
 Summary: Commonly used codes, categories, terminologies, and nomenclatures used in climate policy analysis as a Python package.
 Home-page: https://github.com/pik-primap/climate_categories
 Author: Mika Pflüger
 Author-email: mika.pflueger@climate-resource.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://climate-categories.readthedocs.io/
 Classifier: Development Status :: 4 - Beta
@@ -96,22 +96,28 @@
 KIND, either express or implied. See the License for the specific language governing
 permissions and limitations under the License.
 
 Citation
 --------
 If you use this library and want to cite it, please cite it as:
 
-Mika Pflüger, Annika Günther, Johannes Gütschow, and Robert Gieseke. (2023-06-15).
-pik-primap/climate_categories: climate_categories Version 0.9.1.
-Zenodo. https://doi.org/10.5281/zenodo.8043234
+Mika Pflüger, Annika Günther, Johannes Gütschow, and Robert Gieseke. (2023-06-22).
+pik-primap/climate_categories: climate_categories Version 0.9.2.
+Zenodo. https://doi.org/10.5281/zenodo.8069963
 
 =========
 Changelog
 =========
 
+0.9.2 (2023-06-22)
+------------------
+* ISO3: Add all parties to the UNFCCC as direct children of UNFCCC as first set of
+  children. That way, it is easy to ergonomically get all parties to the UNFCCC without
+  adding up Annex-I and Non-Annex-I parties manually.
+
 0.9.1 (2023-06-15)
 ------------------
 * Add AOSIS country group to ISO3 categorization.
 
 0.9.0 (2023-06-14)
 ------------------
 * Add ISO3 terminology for countries, areas, and country groups including UNFCCC
```

### Comparing `climate_categories-0.9.1/README.rst` & `climate_categories-0.9.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -72,10 +72,10 @@
 KIND, either express or implied. See the License for the specific language governing
 permissions and limitations under the License.
 
 Citation
 --------
 If you use this library and want to cite it, please cite it as:
 
-Mika Pflüger, Annika Günther, Johannes Gütschow, and Robert Gieseke. (2023-06-15).
-pik-primap/climate_categories: climate_categories Version 0.9.1.
-Zenodo. https://doi.org/10.5281/zenodo.8043234
+Mika Pflüger, Annika Günther, Johannes Gütschow, and Robert Gieseke. (2023-06-22).
+pik-primap/climate_categories: climate_categories Version 0.9.2.
+Zenodo. https://doi.org/10.5281/zenodo.8069963
```

### Comparing `climate_categories-0.9.1/climate_categories/__init__.py` & `climate_categories-0.9.2/climate_categories/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Access to all categorizations is provided directly at the module level, using the
 names of categorizations. To access the example categorization `Excat`, simply use
 `climate_categories.Excat` .
 """
 
 __author__ = """Mika Pflüger"""
 __email__ = "mika.pflueger@climate-resource.com"
-__version__ = "0.9.1"
+__version__ = "0.9.2"
 
 import importlib
 import importlib.resources
 
 from . import (
     search,
 )
```

### Comparing `climate_categories-0.9.1/climate_categories/_categories.py` & `climate_categories-0.9.2/climate_categories/_categories.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/climate_categories/_conversions.py` & `climate_categories-0.9.2/climate_categories/_conversions.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/climate_categories/data/BURDI.py` & `climate_categories-0.9.2/climate_categories/data/BURDI.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/climate_categories/data/BURDI.yaml` & `climate_categories-0.9.2/climate_categories/data/BURDI.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/climate_categories/data/BURDI_class.py` & `climate_categories-0.9.2/climate_categories/data/BURDI_class.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/climate_categories/data/BURDI_class.yaml` & `climate_categories-0.9.2/climate_categories/data/BURDI_class.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/climate_categories/data/CRF1999.py` & `climate_categories-0.9.2/climate_categories/data/CRF1999.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/climate_categories/data/CRF1999.yaml` & `climate_categories-0.9.2/climate_categories/data/CRF1999.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/climate_categories/data/CRF2013.py` & `climate_categories-0.9.2/climate_categories/data/CRF2013.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/climate_categories/data/CRF2013.yaml` & `climate_categories-0.9.2/climate_categories/data/CRF2013.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/climate_categories/data/CRF2013_2021.py` & `climate_categories-0.9.2/climate_categories/data/CRF2013_2021.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/climate_categories/data/CRF2013_2021.yaml` & `climate_categories-0.9.2/climate_categories/data/CRF2013_2021.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/climate_categories/data/CRF2013_2022.py` & `climate_categories-0.9.2/climate_categories/data/CRF2013_2022.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/climate_categories/data/CRF2013_2022.yaml` & `climate_categories-0.9.2/climate_categories/data/CRF2013_2022.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/climate_categories/data/CRF2013_2023.py` & `climate_categories-0.9.2/climate_categories/data/CRF2013_2023.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/climate_categories/data/CRF2013_2023.yaml` & `climate_categories-0.9.2/climate_categories/data/CRF2013_2023.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/climate_categories/data/CRFDI.py` & `climate_categories-0.9.2/climate_categories/data/CRFDI.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/climate_categories/data/CRFDI.yaml` & `climate_categories-0.9.2/climate_categories/data/CRFDI.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/climate_categories/data/CRFDI_class.py` & `climate_categories-0.9.2/climate_categories/data/CRFDI_class.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/climate_categories/data/CRFDI_class.yaml` & `climate_categories-0.9.2/climate_categories/data/CRFDI_class.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/climate_categories/data/GCB.py` & `climate_categories-0.9.2/climate_categories/data/GCB.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/climate_categories/data/GCB.yaml` & `climate_categories-0.9.2/climate_categories/data/GCB.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/climate_categories/data/IPCC1996.py` & `climate_categories-0.9.2/climate_categories/data/IPCC1996.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/climate_categories/data/IPCC1996.yaml` & `climate_categories-0.9.2/climate_categories/data/IPCC1996.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/climate_categories/data/IPCC2006.py` & `climate_categories-0.9.2/climate_categories/data/IPCC2006.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/climate_categories/data/IPCC2006.yaml` & `climate_categories-0.9.2/climate_categories/data/IPCC2006.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/climate_categories/data/IPCC2006_PRIMAP.py` & `climate_categories-0.9.2/climate_categories/data/IPCC2006_PRIMAP.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/climate_categories/data/IPCC2006_PRIMAP.yaml` & `climate_categories-0.9.2/climate_categories/data/IPCC2006_PRIMAP.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/climate_categories/data/ISO3.py` & `climate_categories-0.9.2/climate_categories/data/ISO3.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # Do not edit this file. It was auto-generated from the
 # corresponding YAML file.
 spec = {
     "name": "ISO3",
     "title": "ISO 3166-1 countries with climate-relevant groupings",
     "comment": "Countries, regions, and other areas. Also includes information on groups like being included in Annex I of the UN Framework Convention on Climate Change.",
-    "references": "ISO 3166, https://www.iso.org/iso-3166-country-codes.html; iso-codes package, https://salsa.debian.org/iso-codes-team/iso-codes; UNFCCC Parties & Observers, https://unfccc.int/parties-observers; EU members, https://ec.europa.eu/eurostat/statistics-explained/index.php?title=Glossary:EU_enlargements; G7 and G20, https://www.bmuv.de/themen/europa-internationales/internationales/g7-und-g20; OECD members, https://www.oecd.org/about/document/ratification-oecd-convention.htm; AOSIS members, https://www.aosis.org/about/member-states/",
+    "references": "ISO 3166, https://www.iso.org/iso-3166-country-codes.html;\niso-codes package, https://salsa.debian.org/iso-codes-team/iso-codes;\nUNFCCC Parties & Observers, https://unfccc.int/parties-observers;\nEU members,\nhttps://ec.europa.eu/eurostat/statistics-explained/index.php?title=Glossary:EU_enlargements;\n G7 and G20, https://www.bmuv.de/themen/europa-internationales/internationales/g7-und-g20;\n OECD members, https://www.oecd.org/about/document/ratification-oecd-convention.htm;\n AOSIS members, https://www.aosis.org/about/member-states/",
     "institution": "UN",
     "hierarchical": True,
-    "last_update": "2023-04-27",
-    "version": "2023-04-27",
+    "last_update": "2023-06-22",
+    "version": "2023-06-22",
     "total_sum": False,
     "canonical_top_level_category": "World",
     "categories": {
         "ABW": {"title": "Aruba", "alternative_codes": ["AW", "533"]},
         "AFG": {
             "title": "Afghanistan",
             "alternative_codes": ["AF", "004"],
@@ -1706,15 +1706,217 @@
                     "ZWE",
                 ]
             ],
         },
         "UNFCCC": {
             "title": "Parties to the UNFCCC",
             "comment": "Parties to the UN Framework Convention on Climate Change.",
-            "children": [["Annex-I", "Non-Annex-I"]],
+            "children": [
+                [
+                    "AFG",
+                    "AGO",
+                    "ALB",
+                    "AND",
+                    "ARE",
+                    "ARG",
+                    "ARM",
+                    "ATG",
+                    "AUS",
+                    "AUT",
+                    "AZE",
+                    "BDI",
+                    "BEL",
+                    "BEN",
+                    "BFA",
+                    "BGD",
+                    "BGR",
+                    "BHR",
+                    "BHS",
+                    "BIH",
+                    "BLR",
+                    "BLZ",
+                    "BOL",
+                    "BRA",
+                    "BRB",
+                    "BRN",
+                    "BTN",
+                    "BWA",
+                    "CAF",
+                    "CAN",
+                    "CHE",
+                    "CHL",
+                    "CHN",
+                    "CIV",
+                    "CMR",
+                    "COD",
+                    "COG",
+                    "COK",
+                    "COL",
+                    "COM",
+                    "CPV",
+                    "CRI",
+                    "CUB",
+                    "CYP",
+                    "CZE",
+                    "DEU",
+                    "DJI",
+                    "DMA",
+                    "DNK",
+                    "DOM",
+                    "DZA",
+                    "ECU",
+                    "EGY",
+                    "ERI",
+                    "ESP",
+                    "EST",
+                    "ETH",
+                    "EU_2020",
+                    "FIN",
+                    "FJI",
+                    "FRA",
+                    "FSM",
+                    "GAB",
+                    "GBR",
+                    "GEO",
+                    "GHA",
+                    "GIN",
+                    "GMB",
+                    "GNB",
+                    "GNQ",
+                    "GRC",
+                    "GRD",
+                    "GTM",
+                    "GUY",
+                    "HND",
+                    "HRV",
+                    "HTI",
+                    "HUN",
+                    "IDN",
+                    "IND",
+                    "IRL",
+                    "IRN",
+                    "IRQ",
+                    "ISL",
+                    "ISR",
+                    "ITA",
+                    "JAM",
+                    "JOR",
+                    "JPN",
+                    "KAZ",
+                    "KEN",
+                    "KGZ",
+                    "KHM",
+                    "KIR",
+                    "KNA",
+                    "KOR",
+                    "KWT",
+                    "LAO",
+                    "LBN",
+                    "LBR",
+                    "LBY",
+                    "LCA",
+                    "LIE",
+                    "LKA",
+                    "LSO",
+                    "LTU",
+                    "LUX",
+                    "LVA",
+                    "MAR",
+                    "MCO",
+                    "MDA",
+                    "MDG",
+                    "MDV",
+                    "MEX",
+                    "MHL",
+                    "MKD",
+                    "MLI",
+                    "MLT",
+                    "MMR",
+                    "MNE",
+                    "MNG",
+                    "MOZ",
+                    "MRT",
+                    "MUS",
+                    "MWI",
+                    "MYS",
+                    "NAM",
+                    "NER",
+                    "NGA",
+                    "NIC",
+                    "NIU",
+                    "NLD",
+                    "NOR",
+                    "NPL",
+                    "NRU",
+                    "NZL",
+                    "OMN",
+                    "PAK",
+                    "PAN",
+                    "PER",
+                    "PHL",
+                    "PLW",
+                    "PNG",
+                    "POL",
+                    "PRK",
+                    "PRT",
+                    "PRY",
+                    "PSE",
+                    "QAT",
+                    "ROU",
+                    "RUS",
+                    "RWA",
+                    "SAU",
+                    "SDN",
+                    "SEN",
+                    "SGP",
+                    "SLB",
+                    "SLE",
+                    "SLV",
+                    "SMR",
+                    "SOM",
+                    "SRB",
+                    "SSD",
+                    "STP",
+                    "SUR",
+                    "SVK",
+                    "SVN",
+                    "SWE",
+                    "SWZ",
+                    "SYC",
+                    "SYR",
+                    "TCD",
+                    "TGO",
+                    "THA",
+                    "TJK",
+                    "TKM",
+                    "TLS",
+                    "TON",
+                    "TTO",
+                    "TUN",
+                    "TUR",
+                    "TUV",
+                    "TZA",
+                    "UGA",
+                    "UKR",
+                    "URY",
+                    "USA",
+                    "UZB",
+                    "VAT",
+                    "VCT",
+                    "VEN",
+                    "VNM",
+                    "VUT",
+                    "WSM",
+                    "YEM",
+                    "ZAF",
+                    "ZMB",
+                    "ZWE",
+                ],
+                ["Annex-I", "Non-Annex-I"],
+            ],
         },
         "AOSIS": {
             "title": "Alliance of Small Island States",
             "children": [
                 [
                     "ATG",
                     "BHS",
```

### Comparing `climate_categories-0.9.1/climate_categories/data/ISO3.yaml` & `climate_categories-0.9.2/climate_categories/data/ISO3.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 name: ISO3
 title: ISO 3166-1 countries with climate-relevant groupings
 comment: Countries, regions, and other areas. Also includes information on groups
   like being included in Annex I of the UN Framework Convention on Climate Change.
-references: ISO 3166, https://www.iso.org/iso-3166-country-codes.html; iso-codes package,
-  https://salsa.debian.org/iso-codes-team/iso-codes; UNFCCC Parties & Observers, https://unfccc.int/parties-observers;
-  EU members,
-  https://ec.europa.eu/eurostat/statistics-explained/index.php?title=Glossary:EU_enlargements;
-  G7 and G20, https://www.bmuv.de/themen/europa-internationales/internationales/g7-und-g20;
-  OECD members, https://www.oecd.org/about/document/ratification-oecd-convention.htm;
-  AOSIS members, https://www.aosis.org/about/member-states/
+references: "ISO 3166, https://www.iso.org/iso-3166-country-codes.html;\niso-codes
+  package, https://salsa.debian.org/iso-codes-team/iso-codes;\nUNFCCC Parties & Observers,
+  https://unfccc.int/parties-observers;\nEU members,\nhttps://ec.europa.eu/eurostat/statistics-explained/index.php?title=Glossary:EU_enlargements;\n
+  G7 and G20, https://www.bmuv.de/themen/europa-internationales/internationales/g7-und-g20;\n
+  OECD members, https://www.oecd.org/about/document/ratification-oecd-convention.htm;\n
+  AOSIS members, https://www.aosis.org/about/member-states/"
 institution: UN
 hierarchical: true
-last_update: '2023-04-27'
-version: '2023-04-27'
+last_update: '2023-06-22'
+version: '2023-06-22'
 total_sum: false
 canonical_top_level_category: World
 categories:
   ABW:
     title: Aruba
     alternative_codes:
     - AW
@@ -2281,14 +2280,212 @@
       - ZAF
       - ZMB
       - ZWE
   UNFCCC:
     title: Parties to the UNFCCC
     comment: Parties to the UN Framework Convention on Climate Change.
     children:
+    - - AFG
+      - AGO
+      - ALB
+      - AND
+      - ARE
+      - ARG
+      - ARM
+      - ATG
+      - AUS
+      - AUT
+      - AZE
+      - BDI
+      - BEL
+      - BEN
+      - BFA
+      - BGD
+      - BGR
+      - BHR
+      - BHS
+      - BIH
+      - BLR
+      - BLZ
+      - BOL
+      - BRA
+      - BRB
+      - BRN
+      - BTN
+      - BWA
+      - CAF
+      - CAN
+      - CHE
+      - CHL
+      - CHN
+      - CIV
+      - CMR
+      - COD
+      - COG
+      - COK
+      - COL
+      - COM
+      - CPV
+      - CRI
+      - CUB
+      - CYP
+      - CZE
+      - DEU
+      - DJI
+      - DMA
+      - DNK
+      - DOM
+      - DZA
+      - ECU
+      - EGY
+      - ERI
+      - ESP
+      - EST
+      - ETH
+      - EU_2020
+      - FIN
+      - FJI
+      - FRA
+      - FSM
+      - GAB
+      - GBR
+      - GEO
+      - GHA
+      - GIN
+      - GMB
+      - GNB
+      - GNQ
+      - GRC
+      - GRD
+      - GTM
+      - GUY
+      - HND
+      - HRV
+      - HTI
+      - HUN
+      - IDN
+      - IND
+      - IRL
+      - IRN
+      - IRQ
+      - ISL
+      - ISR
+      - ITA
+      - JAM
+      - JOR
+      - JPN
+      - KAZ
+      - KEN
+      - KGZ
+      - KHM
+      - KIR
+      - KNA
+      - KOR
+      - KWT
+      - LAO
+      - LBN
+      - LBR
+      - LBY
+      - LCA
+      - LIE
+      - LKA
+      - LSO
+      - LTU
+      - LUX
+      - LVA
+      - MAR
+      - MCO
+      - MDA
+      - MDG
+      - MDV
+      - MEX
+      - MHL
+      - MKD
+      - MLI
+      - MLT
+      - MMR
+      - MNE
+      - MNG
+      - MOZ
+      - MRT
+      - MUS
+      - MWI
+      - MYS
+      - NAM
+      - NER
+      - NGA
+      - NIC
+      - NIU
+      - NLD
+      - NOR
+      - NPL
+      - NRU
+      - NZL
+      - OMN
+      - PAK
+      - PAN
+      - PER
+      - PHL
+      - PLW
+      - PNG
+      - POL
+      - PRK
+      - PRT
+      - PRY
+      - PSE
+      - QAT
+      - ROU
+      - RUS
+      - RWA
+      - SAU
+      - SDN
+      - SEN
+      - SGP
+      - SLB
+      - SLE
+      - SLV
+      - SMR
+      - SOM
+      - SRB
+      - SSD
+      - STP
+      - SUR
+      - SVK
+      - SVN
+      - SWE
+      - SWZ
+      - SYC
+      - SYR
+      - TCD
+      - TGO
+      - THA
+      - TJK
+      - TKM
+      - TLS
+      - TON
+      - TTO
+      - TUN
+      - TUR
+      - TUV
+      - TZA
+      - UGA
+      - UKR
+      - URY
+      - USA
+      - UZB
+      - VAT
+      - VCT
+      - VEN
+      - VNM
+      - VUT
+      - WSM
+      - YEM
+      - ZAF
+      - ZMB
+      - ZWE
     - - Annex-I
       - Non-Annex-I
   AOSIS:
     title: Alliance of Small Island States
     children:
     - - ATG
       - BHS
```

### Comparing `climate_categories-0.9.1/climate_categories/data/RCMIP.py` & `climate_categories-0.9.2/climate_categories/data/RCMIP.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/climate_categories/data/RCMIP.yaml` & `climate_categories-0.9.2/climate_categories/data/RCMIP.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/climate_categories/data/conversion.IPCC1996.IPCC2006.csv` & `climate_categories-0.9.2/climate_categories/data/conversion.IPCC1996.IPCC2006.csv`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/climate_categories/data/gas.py` & `climate_categories-0.9.2/climate_categories/data/gas.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/climate_categories/data/gas.yaml` & `climate_categories-0.9.2/climate_categories/data/gas.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/climate_categories/tests/conftest.py` & `climate_categories-0.9.2/climate_categories/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/climate_categories/tests/data/broken_hierarchical_categorization.yaml` & `climate_categories-0.9.2/climate_categories/tests/data/broken_hierarchical_categorization.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/climate_categories/tests/data/broken_simple_categorization.yaml` & `climate_categories-0.9.2/climate_categories/tests/data/broken_simple_categorization.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/climate_categories/tests/data/good_conversion_A.yaml` & `climate_categories-0.9.2/climate_categories/tests/data/good_conversion_A.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/climate_categories/tests/data/hierarchical_categorization.yaml` & `climate_categories-0.9.2/climate_categories/tests/data/hierarchical_categorization.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/climate_categories/tests/data/simple_categorization.yaml` & `climate_categories-0.9.2/climate_categories/tests/data/simple_categorization.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/climate_categories/tests/examples.py` & `climate_categories-0.9.2/climate_categories/tests/examples.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/climate_categories/tests/test_climate_categories.py` & `climate_categories-0.9.2/climate_categories/tests/test_climate_categories.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/climate_categories/tests/test_conversions.py` & `climate_categories-0.9.2/climate_categories/tests/test_conversions.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/climate_categories/tests/test_crf.py` & `climate_categories-0.9.2/climate_categories/tests/test_crf.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/climate_categories/tests/test_di.py` & `climate_categories-0.9.2/climate_categories/tests/test_di.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/climate_categories/tests/test_ipcc.py` & `climate_categories-0.9.2/climate_categories/tests/test_ipcc.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/climate_categories/tests/test_iso3.py` & `climate_categories-0.9.2/climate_categories/tests/test_iso3.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,17 +23,24 @@
 
 
 def test_unfccc():
     assert len(climate_categories.ISO3["Annex-I"].children[0]) == 43
     assert len(climate_categories.ISO3["Non-Annex-I"].children[0]) == 155
     # leaf children excludes EU, because EU is not a leaf
     assert len(climate_categories.ISO3["UNFCCC"].leaf_children[0]) == 197
+    assert len(climate_categories.ISO3["UNFCCC"].children[0]) == 198
     assert (
-        climate_categories.ISO3["EU"] in climate_categories.ISO3["UNFCCC"].descendants
+        climate_categories.ISO3["EU"] in climate_categories.ISO3["UNFCCC"].children[0]
     )
+    assert climate_categories.ISO3["Annex-I"] in climate_categories.ISO3.descendants(
+        "UNFCCC"
+    )
+    assert climate_categories.ISO3[
+        "Non-Annex-I"
+    ] in climate_categories.ISO3.descendants("UNFCCC")
 
 
 def test_g7g20():
     # since the EU is a non-enumerated member, G7 has 8 members, G8 has 9.
     assert len(climate_categories.ISO3["G7"].children[0]) == 8
     assert len(climate_categories.ISO3["G8"].children[0]) == 9
     # in the G20, the EU is enumerated
```

### Comparing `climate_categories-0.9.1/climate_categories/tests/test_overcounting.py` & `climate_categories-0.9.2/climate_categories/tests/test_overcounting.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/climate_categories/tests/test_primap.py` & `climate_categories-0.9.2/climate_categories/tests/test_primap.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/climate_categories/tests/test_search.py` & `climate_categories-0.9.2/climate_categories/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/climate_categories.egg-info/PKG-INFO` & `climate_categories-0.9.2/climate_categories.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climate-categories
-Version: 0.9.1
+Version: 0.9.2
 Summary: Commonly used codes, categories, terminologies, and nomenclatures used in climate policy analysis as a Python package.
 Home-page: https://github.com/pik-primap/climate_categories
 Author: Mika Pflüger
 Author-email: mika.pflueger@climate-resource.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://climate-categories.readthedocs.io/
 Classifier: Development Status :: 4 - Beta
@@ -96,22 +96,28 @@
 KIND, either express or implied. See the License for the specific language governing
 permissions and limitations under the License.
 
 Citation
 --------
 If you use this library and want to cite it, please cite it as:
 
-Mika Pflüger, Annika Günther, Johannes Gütschow, and Robert Gieseke. (2023-06-15).
-pik-primap/climate_categories: climate_categories Version 0.9.1.
-Zenodo. https://doi.org/10.5281/zenodo.8043234
+Mika Pflüger, Annika Günther, Johannes Gütschow, and Robert Gieseke. (2023-06-22).
+pik-primap/climate_categories: climate_categories Version 0.9.2.
+Zenodo. https://doi.org/10.5281/zenodo.8069963
 
 =========
 Changelog
 =========
 
+0.9.2 (2023-06-22)
+------------------
+* ISO3: Add all parties to the UNFCCC as direct children of UNFCCC as first set of
+  children. That way, it is easy to ergonomically get all parties to the UNFCCC without
+  adding up Annex-I and Non-Annex-I parties manually.
+
 0.9.1 (2023-06-15)
 ------------------
 * Add AOSIS country group to ISO3 categorization.
 
 0.9.0 (2023-06-14)
 ------------------
 * Add ISO3 terminology for countries, areas, and country groups including UNFCCC
```

### Comparing `climate_categories-0.9.1/climate_categories.egg-info/SOURCES.txt` & `climate_categories-0.9.2/climate_categories.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/data_generation/BURDI.py` & `climate_categories-0.9.2/data_generation/BURDI.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/data_generation/BURDI_class.py` & `climate_categories-0.9.2/data_generation/BURDI_class.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/data_generation/CRF1999.py` & `climate_categories-0.9.2/data_generation/CRF1999.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/data_generation/CRF2013.py` & `climate_categories-0.9.2/data_generation/CRF2013.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/data_generation/CRF2013_2021.py` & `climate_categories-0.9.2/data_generation/CRF2013_2021.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/data_generation/CRF2013_2022.py` & `climate_categories-0.9.2/data_generation/CRF2013_2022.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/data_generation/CRF2013_2023.py` & `climate_categories-0.9.2/data_generation/CRF2013_2023.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/data_generation/CRFDI.py` & `climate_categories-0.9.2/data_generation/CRFDI.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/data_generation/CRFDI_class.py` & `climate_categories-0.9.2/data_generation/CRFDI_class.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/data_generation/IPCC1996.py` & `climate_categories-0.9.2/data_generation/IPCC1996.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/data_generation/IPCC2006.py` & `climate_categories-0.9.2/data_generation/IPCC2006.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/data_generation/IPCC2006_PRIMAP.py` & `climate_categories-0.9.2/data_generation/IPCC2006_PRIMAP.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/data_generation/ISO3.py` & `climate_categories-0.9.2/data_generation/ISO3.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,17 +43,17 @@
 UNFCCC Parties & Observers, https://unfccc.int/parties-observers;
 EU members,
 https://ec.europa.eu/eurostat/statistics-explained/index.php?title=Glossary:EU_enlargements;
 G7 and G20, https://www.bmuv.de/themen/europa-internationales/internationales/g7-und-g20;
 OECD members, https://www.oecd.org/about/document/ratification-oecd-convention.htm;
 AOSIS members, https://www.aosis.org/about/member-states/""",
         "institution": "UN",
-        "last_update": "2023-04-27",
+        "last_update": "2023-06-22",
         "hierarchical": True,
-        "version": "2023-04-27",
+        "version": "2023-06-22",
         "total_sum": False,
         "categories": categories,
         "canonical_top_level_category": "WORLD",
     }
 
     return climate_categories.HierarchicalCategorization.from_spec(spec)
 
@@ -423,15 +423,19 @@
                 "BOL",
             ]
         ],
     }
     categories["UNFCCC"] = {
         "title": "Parties to the UNFCCC",
         "comment": "Parties to the UN Framework Convention on Climate Change.",
-        "children": [["Annex-I", "Non-Annex-I"]],
+        "children": [
+            categories["Annex-I"]["children"][0]
+            + categories["Non-Annex-I"]["children"][0],
+            ["Annex-I", "Non-Annex-I"],
+        ],
     }
 
     return categories
 
 
 def add_eu_categories(categories):
     categories["EU_1993"] = {
```

### Comparing `climate_categories-0.9.1/data_generation/RCMIP.py` & `climate_categories-0.9.2/data_generation/RCMIP.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/data_generation/gas.py` & `climate_categories-0.9.2/data_generation/gas.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/data_generation/utils.py` & `climate_categories-0.9.2/data_generation/utils.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/docs/Makefile` & `climate_categories-0.9.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/docs/conf.py` & `climate_categories-0.9.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/docs/data.rst` & `climate_categories-0.9.2/docs/data.rst`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/docs/installation.rst` & `climate_categories-0.9.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/docs/make.bat` & `climate_categories-0.9.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/docs/usage.ipynb` & `climate_categories-0.9.2/docs/usage.ipynb`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/setup.cfg` & `climate_categories-0.9.2/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = climate_categories
-version = 0.9.1
+version = 0.9.2
 author = Mika Pflüger
 author_email = mika.pflueger@climate-resource.com
 description = Commonly used codes, categories, terminologies, and nomenclatures used in climate policy analysis as a Python package.
 long_description = file: README.rst, CHANGELOG.rst
 long_description_content_type = text/x-rst
 url = https://github.com/pik-primap/climate_categories
 project_urls =
```

### Comparing `climate_categories-0.9.1/tbump.toml` & `climate_categories-0.9.2/tbump.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Uncomment this if your project is hosted on GitHub:
 github_url = "https://github.com/pik-primap/climate_categories/"
 
 [version]
-current = "0.9.1"
+current = "0.9.2"
 
 # Example of a semver regexp.
 # Make sure this matches current_version before
 # using tbump
 regex = '''
   (?P<major>\d+)
   \.
```

### Comparing `climate_categories-0.9.1/update_changelog.py` & `climate_categories-0.9.2/update_changelog.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.9.1/update_citation_info.py` & `climate_categories-0.9.2/update_citation_info.py`

 * *Files identical despite different names*

