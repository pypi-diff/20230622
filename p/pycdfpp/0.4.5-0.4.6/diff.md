# Comparing `tmp/pycdfpp-0.4.5.tar.gz` & `tmp/pycdfpp-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycdfpp-0.4.5.tar", last modified: Wed Jun 21 09:44:49 2023, max compression
+gzip compressed data, was "pycdfpp-0.4.6.tar", last modified: Thu Jun 22 13:56:07 2023, max compression
```

## Comparing `pycdfpp-0.4.5.tar` & `pycdfpp-0.4.6.tar`

### file list

```diff
@@ -1,73 +1,73 @@
--rw-r--r--   0        0        0      201 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/.bumpversion.cfg
--rw-r--r--   0        0        0     2445 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/.cirrus.yml
--rw-r--r--   0        0        0      613 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/.clang-format
--rw-r--r--   0        0        0     4926 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/.github/workflows/CI.yml
--rw-r--r--   0        0        0     1259 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/.github/workflows/tests-with-coverage.yml
--rw-r--r--   0        0        0      130 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/.gitignore
--rw-r--r--   0        0        0      378 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/.gitpod.Dockerfile
--rw-r--r--   0        0        0      279 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/.gitpod.yml
--rw-r--r--   0        0        0      309 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/.theia/settings.json
--rw-r--r--   0        0        0     1552 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/COPYING
--rw-r--r--   0        0        0     6390 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/README.md
--rw-r--r--   0        0        0      171 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/environment.yml
--rw-r--r--   0        0        0     1041 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/examples/basic_cpp/main.cpp
--rw-r--r--   0        0        0   550561 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/examples/notebooks/Demo.ipynb
--rw-r--r--   0        0        0     3735 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/include/cdfpp/attribute.hpp
--rw-r--r--   0        0        0     8709 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/include/cdfpp/cdf-data.hpp
--rw-r--r--   0        0        0     1797 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/include/cdfpp/cdf-debug.hpp
--rw-r--r--   0        0        0     4816 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/include/cdfpp/cdf-endianness.hpp
--rw-r--r--   0        0        0     7921 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/include/cdfpp/cdf-enums.hpp
--rw-r--r--   0        0        0     1996 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/include/cdfpp/cdf-file.hpp
--rw-r--r--   0        0        0     1553 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/include/cdfpp/cdf-helpers.hpp
--rw-r--r--   0        0        0     3302 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/include/cdfpp/cdf-io/cdf-io-attribute.hpp
--rw-r--r--   0        0        0     9295 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/include/cdfpp/cdf-io/cdf-io-buffers.hpp
--rw-r--r--   0        0        0     7420 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/include/cdfpp/cdf-io/cdf-io-common.hpp
--rw-r--r--   0        0        0    28550 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/include/cdfpp/cdf-io/cdf-io-desc-records.hpp
--rw-r--r--   0        0        0     1896 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/include/cdfpp/cdf-io/cdf-io-rle.hpp
--rw-r--r--   0        0        0    11871 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/include/cdfpp/cdf-io/cdf-io-variable.hpp
--rw-r--r--   0        0        0     7208 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/include/cdfpp/cdf-io/cdf-io-zlib.hpp
--rw-r--r--   0        0        0     7540 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/include/cdfpp/cdf-io/cdf-io.hpp
--rw-r--r--   0        0        0     6668 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/include/cdfpp/cdf-majority-swap.hpp
--rw-r--r--   0        0        0     8482 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/include/cdfpp/cdf-repr.hpp
--rw-r--r--   0        0        0     1319 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/include/cdfpp/cdf.hpp
--rw-r--r--   0        0        0     1419 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/include/cdfpp/chrono/cdf-chrono-constants.hpp
--rw-r--r--   0        0        0     4403 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/include/cdfpp/chrono/cdf-chrono.hpp
--rw-r--r--   0        0        0     5689 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/include/cdfpp/chrono/cdf-leap-seconds.h
--rw-r--r--   0        0        0     3512 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/include/cdfpp/variable.hpp
--rw-r--r--   0        0        0     6996 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/meson.build
--rw-r--r--   0        0        0      217 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/meson_options.txt
--rw-r--r--   0        0        0     8409 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/notebooks/Leap_seconds.ipynb
--rw-r--r--   0        0        0     2573 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/notebooks/chrono_test_table_gen.ipynb
--rw-r--r--   0        0        0      947 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/pyproject.toml
--rwxr-xr-x   0        0        0     1349 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/scripts/build_wheel.py
--rwxr-xr-x   0        0        0     1208 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/scripts/version.py
--rw-r--r--   0        0        0      432 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/subprojects/catch2.wrap
--rw-r--r--   0        0        0      446 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/subprojects/fmt.wrap
--rw-r--r--   0        0        0      451 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/subprojects/hedley.wrap
--rw-r--r--   0        0        0      616 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/subprojects/pybind11.wrap
--rw-r--r--   0        0        0      449 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/subprojects/zlib.wrap
--rw-r--r--   0        0        0     2084 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/tests/chrono/main.cpp
--rw-r--r--   0        0        0   124469 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/tests/chrono/test_values.hpp
--rw-r--r--   0        0        0      543 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/tests/endianness/main.cpp
--rw-r--r--   0        0        0     2478 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/tests/full_corpus/test_full_corpus.py
--rw-r--r--   0        0        0     1399 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/tests/majority/main.cpp
--rw-r--r--   0        0        0      965 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/tests/manual_load/main.cpp
--rwxr-xr-x   0        0        0     8834 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/tests/python_wrapper/test.py
--rwxr-xr-x   0        0        0     5626 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/tests/python_wrapper/test_corpus.py
--rw-r--r--   0        0        0      461 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/tests/python_wrapper_cpp/main.cpp
--rw-r--r--   0        0        0   113172 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/tests/resources/a_cdf.cdf
--rw-r--r--   0        0        0    41097 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/tests/resources/a_cdf_with_compressed_vars.cdf
--rw-r--r--   0        0        0   113172 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/tests/resources/a_col_major_cdf.cdf
--rw-r--r--   0        0        0     4936 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/tests/resources/a_compressed_cdf.cdf
--rw-r--r--   0        0        0     4936 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/tests/resources/a_rle_compressed_cdf.cdf
--rwxr-xr-x   0        0        0     4348 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/tests/resources/make_cdf.py
--rw-r--r--   0        0        0       20 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/tests/resources/not_a_cdf.cdf
--rw-r--r--   0        0        0   117066 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/tests/resources/testutf8.cdf
--rw-r--r--   0        0        0    55597 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/tests/resources/wi_l2-30min_sms-stics-afm-magnetosphere_00000000_v01.cdf
--rw-r--r--   0        0        0    19688 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/tests/simple_open/main.cpp
--rw-r--r--   0        0        0     2010 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/tests/zlib/main.cpp
--rw-r--r--   0        0        0        6 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/version.txt
--rw-r--r--   0        0        0     8660 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/wrapper/buffers.hpp
--rw-r--r--   0        0        0     7412 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/wrapper/chrono.hpp
--rw-r--r--   0        0        0    10477 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/wrapper/pycdfpp.cpp
--rw-r--r--   0        0        0     9050 1970-01-01 00:00:00.000000 pycdfpp-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0      201 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/.bumpversion.cfg
+-rw-r--r--   0        0        0     2445 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/.cirrus.yml
+-rw-r--r--   0        0        0      613 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/.clang-format
+-rw-r--r--   0        0        0     4926 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/.github/workflows/CI.yml
+-rw-r--r--   0        0        0     1259 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/.github/workflows/tests-with-coverage.yml
+-rw-r--r--   0        0        0      130 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/.gitignore
+-rw-r--r--   0        0        0      378 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/.gitpod.Dockerfile
+-rw-r--r--   0        0        0      279 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/.gitpod.yml
+-rw-r--r--   0        0        0      309 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/.theia/settings.json
+-rw-r--r--   0        0        0     1552 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/COPYING
+-rw-r--r--   0        0        0     6390 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/README.md
+-rw-r--r--   0        0        0      171 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/environment.yml
+-rw-r--r--   0        0        0     1041 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/examples/basic_cpp/main.cpp
+-rw-r--r--   0        0        0   550561 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/examples/notebooks/Demo.ipynb
+-rw-r--r--   0        0        0     3735 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/include/cdfpp/attribute.hpp
+-rw-r--r--   0        0        0     8709 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/include/cdfpp/cdf-data.hpp
+-rw-r--r--   0        0        0     1797 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/include/cdfpp/cdf-debug.hpp
+-rw-r--r--   0        0        0     4816 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/include/cdfpp/cdf-endianness.hpp
+-rw-r--r--   0        0        0     7921 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/include/cdfpp/cdf-enums.hpp
+-rw-r--r--   0        0        0     1996 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/include/cdfpp/cdf-file.hpp
+-rw-r--r--   0        0        0     1553 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/include/cdfpp/cdf-helpers.hpp
+-rw-r--r--   0        0        0     3302 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/include/cdfpp/cdf-io/cdf-io-attribute.hpp
+-rw-r--r--   0        0        0     9295 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/include/cdfpp/cdf-io/cdf-io-buffers.hpp
+-rw-r--r--   0        0        0     7420 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/include/cdfpp/cdf-io/cdf-io-common.hpp
+-rw-r--r--   0        0        0    28550 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/include/cdfpp/cdf-io/cdf-io-desc-records.hpp
+-rw-r--r--   0        0        0     1896 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/include/cdfpp/cdf-io/cdf-io-rle.hpp
+-rw-r--r--   0        0        0    11871 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/include/cdfpp/cdf-io/cdf-io-variable.hpp
+-rw-r--r--   0        0        0     7208 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/include/cdfpp/cdf-io/cdf-io-zlib.hpp
+-rw-r--r--   0        0        0     7540 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/include/cdfpp/cdf-io/cdf-io.hpp
+-rw-r--r--   0        0        0     6668 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/include/cdfpp/cdf-majority-swap.hpp
+-rw-r--r--   0        0        0     8571 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/include/cdfpp/cdf-repr.hpp
+-rw-r--r--   0        0        0     1319 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/include/cdfpp/cdf.hpp
+-rw-r--r--   0        0        0     1419 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/include/cdfpp/chrono/cdf-chrono-constants.hpp
+-rw-r--r--   0        0        0     4403 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/include/cdfpp/chrono/cdf-chrono.hpp
+-rw-r--r--   0        0        0     5689 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/include/cdfpp/chrono/cdf-leap-seconds.h
+-rw-r--r--   0        0        0     3512 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/include/cdfpp/variable.hpp
+-rw-r--r--   0        0        0     6996 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/meson.build
+-rw-r--r--   0        0        0      217 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/meson_options.txt
+-rw-r--r--   0        0        0     8409 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/notebooks/Leap_seconds.ipynb
+-rw-r--r--   0        0        0     2573 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/notebooks/chrono_test_table_gen.ipynb
+-rw-r--r--   0        0        0      947 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/pyproject.toml
+-rwxr-xr-x   0        0        0     1349 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/scripts/build_wheel.py
+-rwxr-xr-x   0        0        0     1208 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/scripts/version.py
+-rw-r--r--   0        0        0      432 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/subprojects/catch2.wrap
+-rw-r--r--   0        0        0      446 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/subprojects/fmt.wrap
+-rw-r--r--   0        0        0      451 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/subprojects/hedley.wrap
+-rw-r--r--   0        0        0      616 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/subprojects/pybind11.wrap
+-rw-r--r--   0        0        0      449 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/subprojects/zlib.wrap
+-rw-r--r--   0        0        0     2084 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/tests/chrono/main.cpp
+-rw-r--r--   0        0        0   124469 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/tests/chrono/test_values.hpp
+-rw-r--r--   0        0        0      543 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/tests/endianness/main.cpp
+-rw-r--r--   0        0        0     2478 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/tests/full_corpus/test_full_corpus.py
+-rw-r--r--   0        0        0     1399 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/tests/majority/main.cpp
+-rw-r--r--   0        0        0      965 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/tests/manual_load/main.cpp
+-rwxr-xr-x   0        0        0     8834 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/tests/python_wrapper/test.py
+-rwxr-xr-x   0        0        0     5626 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/tests/python_wrapper/test_corpus.py
+-rw-r--r--   0        0        0      461 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/tests/python_wrapper_cpp/main.cpp
+-rw-r--r--   0        0        0   113172 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/tests/resources/a_cdf.cdf
+-rw-r--r--   0        0        0    41097 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/tests/resources/a_cdf_with_compressed_vars.cdf
+-rw-r--r--   0        0        0   113172 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/tests/resources/a_col_major_cdf.cdf
+-rw-r--r--   0        0        0     4936 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/tests/resources/a_compressed_cdf.cdf
+-rw-r--r--   0        0        0     4936 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/tests/resources/a_rle_compressed_cdf.cdf
+-rwxr-xr-x   0        0        0     4348 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/tests/resources/make_cdf.py
+-rw-r--r--   0        0        0       20 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/tests/resources/not_a_cdf.cdf
+-rw-r--r--   0        0        0   117066 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/tests/resources/testutf8.cdf
+-rw-r--r--   0        0        0    55597 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/tests/resources/wi_l2-30min_sms-stics-afm-magnetosphere_00000000_v01.cdf
+-rw-r--r--   0        0        0    19688 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/tests/simple_open/main.cpp
+-rw-r--r--   0        0        0     2010 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/tests/zlib/main.cpp
+-rw-r--r--   0        0        0        6 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/version.txt
+-rw-r--r--   0        0        0     8660 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/wrapper/buffers.hpp
+-rw-r--r--   0        0        0     7412 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/wrapper/chrono.hpp
+-rw-r--r--   0        0        0    10477 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/wrapper/pycdfpp.cpp
+-rw-r--r--   0        0        0     9050 1970-01-01 00:00:00.000000 pycdfpp-0.4.6/PKG-INFO
```

### Comparing `pycdfpp-0.4.5/.cirrus.yml` & `pycdfpp-0.4.6/.cirrus.yml`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/.clang-format` & `pycdfpp-0.4.6/.clang-format`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/.github/workflows/CI.yml` & `pycdfpp-0.4.6/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/.github/workflows/tests-with-coverage.yml` & `pycdfpp-0.4.6/.github/workflows/tests-with-coverage.yml`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/COPYING` & `pycdfpp-0.4.6/COPYING`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/README.md` & `pycdfpp-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/examples/basic_cpp/main.cpp` & `pycdfpp-0.4.6/examples/basic_cpp/main.cpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/examples/notebooks/Demo.ipynb` & `pycdfpp-0.4.6/examples/notebooks/Demo.ipynb`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/include/cdfpp/attribute.hpp` & `pycdfpp-0.4.6/include/cdfpp/attribute.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/include/cdfpp/cdf-data.hpp` & `pycdfpp-0.4.6/include/cdfpp/cdf-data.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/include/cdfpp/cdf-debug.hpp` & `pycdfpp-0.4.6/include/cdfpp/cdf-debug.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/include/cdfpp/cdf-endianness.hpp` & `pycdfpp-0.4.6/include/cdfpp/cdf-endianness.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/include/cdfpp/cdf-enums.hpp` & `pycdfpp-0.4.6/include/cdfpp/cdf-enums.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/include/cdfpp/cdf-file.hpp` & `pycdfpp-0.4.6/include/cdfpp/cdf-file.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/include/cdfpp/cdf-helpers.hpp` & `pycdfpp-0.4.6/include/cdfpp/cdf-helpers.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/include/cdfpp/cdf-io/cdf-io-attribute.hpp` & `pycdfpp-0.4.6/include/cdfpp/cdf-io/cdf-io-attribute.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/include/cdfpp/cdf-io/cdf-io-buffers.hpp` & `pycdfpp-0.4.6/include/cdfpp/cdf-io/cdf-io-buffers.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/include/cdfpp/cdf-io/cdf-io-common.hpp` & `pycdfpp-0.4.6/include/cdfpp/cdf-io/cdf-io-common.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/include/cdfpp/cdf-io/cdf-io-desc-records.hpp` & `pycdfpp-0.4.6/include/cdfpp/cdf-io/cdf-io-desc-records.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/include/cdfpp/cdf-io/cdf-io-rle.hpp` & `pycdfpp-0.4.6/include/cdfpp/cdf-io/cdf-io-rle.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/include/cdfpp/cdf-io/cdf-io-variable.hpp` & `pycdfpp-0.4.6/include/cdfpp/cdf-io/cdf-io-variable.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/include/cdfpp/cdf-io/cdf-io-zlib.hpp` & `pycdfpp-0.4.6/include/cdfpp/cdf-io/cdf-io-zlib.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/include/cdfpp/cdf-io/cdf-io.hpp` & `pycdfpp-0.4.6/include/cdfpp/cdf-io/cdf-io.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/include/cdfpp/cdf-majority-swap.hpp` & `pycdfpp-0.4.6/include/cdfpp/cdf-majority-swap.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/include/cdfpp/cdf-repr.hpp` & `pycdfpp-0.4.6/include/cdfpp/cdf-repr.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -48,26 +48,31 @@
 };
 
 inline std::ostream& operator<<(
     std::ostream& os, const std::chrono::time_point<std::chrono::system_clock>& tp)
 {
     const auto time_t = std::chrono::system_clock::to_time_t(tp);
     const auto tt = std::gmtime(&time_t);
-    const auto us
-        = (std::chrono::duration_cast<std::chrono::microseconds>(tp.time_since_epoch()) % 1000000)
-              .count();
-    // clang-format off
-    os << fixed_width<4> << tt->tm_year + 1900 << '-'
-       << fixed_width<2> << tt->tm_mon + 1     << '-'
-       << fixed_width<2> << tt->tm_mday        << 'T'
-       << fixed_width<2> << tt->tm_hour        << ':'
-       << fixed_width<2> << tt->tm_min         << ':'
-       << fixed_width<2> << tt->tm_sec         << '.'
-       << fixed_width<6> << us;
-    // clang-format on
+    if (tt)
+    {
+        const auto us
+            = (std::chrono::duration_cast<std::chrono::microseconds>(tp.time_since_epoch())
+                % 1000000)
+                  .count();
+        // clang-format off
+        os << fixed_width<4> << tt->tm_year + 1900 << '-'
+           << fixed_width<2> << tt->tm_mon + 1     << '-'
+           << fixed_width<2> << tt->tm_mday        << 'T'
+           << fixed_width<2> << tt->tm_hour        << ':'
+           << fixed_width<2> << tt->tm_min         << ':'
+           << fixed_width<2> << tt->tm_sec         << '.'
+           << fixed_width<6> << us;
+        // clang-format on
+    }
+
     return os;
 }
 
 inline std::ostream& operator<<(std::ostream& os, const epoch& time)
 {
     os << cdf::to_time_point(time) << std::endl;
     return os;
```

### Comparing `pycdfpp-0.4.5/include/cdfpp/cdf.hpp` & `pycdfpp-0.4.6/include/cdfpp/cdf.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/include/cdfpp/chrono/cdf-chrono-constants.hpp` & `pycdfpp-0.4.6/include/cdfpp/chrono/cdf-chrono-constants.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/include/cdfpp/chrono/cdf-chrono.hpp` & `pycdfpp-0.4.6/include/cdfpp/chrono/cdf-chrono.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/include/cdfpp/chrono/cdf-leap-seconds.h` & `pycdfpp-0.4.6/include/cdfpp/chrono/cdf-leap-seconds.h`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/include/cdfpp/variable.hpp` & `pycdfpp-0.4.6/include/cdfpp/variable.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/meson.build` & `pycdfpp-0.4.6/meson.build`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/notebooks/Leap_seconds.ipynb` & `pycdfpp-0.4.6/notebooks/Leap_seconds.ipynb`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/notebooks/chrono_test_table_gen.ipynb` & `pycdfpp-0.4.6/notebooks/chrono_test_table_gen.ipynb`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/pyproject.toml` & `pycdfpp-0.4.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/scripts/build_wheel.py` & `pycdfpp-0.4.6/scripts/build_wheel.py`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/scripts/version.py` & `pycdfpp-0.4.6/scripts/version.py`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/subprojects/pybind11.wrap` & `pycdfpp-0.4.6/subprojects/pybind11.wrap`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/tests/chrono/main.cpp` & `pycdfpp-0.4.6/tests/chrono/main.cpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/tests/chrono/test_values.hpp` & `pycdfpp-0.4.6/tests/chrono/test_values.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/tests/endianness/main.cpp` & `pycdfpp-0.4.6/tests/endianness/main.cpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/tests/full_corpus/test_full_corpus.py` & `pycdfpp-0.4.6/tests/full_corpus/test_full_corpus.py`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/tests/majority/main.cpp` & `pycdfpp-0.4.6/tests/majority/main.cpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/tests/manual_load/main.cpp` & `pycdfpp-0.4.6/tests/manual_load/main.cpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/tests/python_wrapper/test.py` & `pycdfpp-0.4.6/tests/python_wrapper/test.py`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/tests/python_wrapper/test_corpus.py` & `pycdfpp-0.4.6/tests/python_wrapper/test_corpus.py`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/tests/resources/a_cdf.cdf` & `pycdfpp-0.4.6/tests/resources/a_cdf.cdf`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/tests/resources/a_cdf_with_compressed_vars.cdf` & `pycdfpp-0.4.6/tests/resources/a_cdf_with_compressed_vars.cdf`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/tests/resources/a_col_major_cdf.cdf` & `pycdfpp-0.4.6/tests/resources/a_col_major_cdf.cdf`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/tests/resources/a_compressed_cdf.cdf` & `pycdfpp-0.4.6/tests/resources/a_compressed_cdf.cdf`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/tests/resources/a_rle_compressed_cdf.cdf` & `pycdfpp-0.4.6/tests/resources/a_rle_compressed_cdf.cdf`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/tests/resources/make_cdf.py` & `pycdfpp-0.4.6/tests/resources/make_cdf.py`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/tests/resources/testutf8.cdf` & `pycdfpp-0.4.6/tests/resources/testutf8.cdf`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/tests/resources/wi_l2-30min_sms-stics-afm-magnetosphere_00000000_v01.cdf` & `pycdfpp-0.4.6/tests/resources/wi_l2-30min_sms-stics-afm-magnetosphere_00000000_v01.cdf`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/tests/simple_open/main.cpp` & `pycdfpp-0.4.6/tests/simple_open/main.cpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/tests/zlib/main.cpp` & `pycdfpp-0.4.6/tests/zlib/main.cpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/wrapper/buffers.hpp` & `pycdfpp-0.4.6/wrapper/buffers.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/wrapper/chrono.hpp` & `pycdfpp-0.4.6/wrapper/chrono.hpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/wrapper/pycdfpp.cpp` & `pycdfpp-0.4.6/wrapper/pycdfpp.cpp`

 * *Files identical despite different names*

### Comparing `pycdfpp-0.4.5/PKG-INFO` & `pycdfpp-0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycdfpp
-Version: 0.4.5
+Version: 0.4.6
 Summary: A modern C++ header only cdf library
 Home-page: https://github.com/SciQLop/CDFpp
 Author-Email: Alexis Jeandet <alexis.jeandet@member.fsf.org>
 License: GNU GENERAL PUBLIC LICENSE
                               Version 3, 29 June 2007
         
             An easy to use ISTP loader package.
```

