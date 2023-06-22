# Comparing `tmp/blspy-2.0.0b3.tar.gz` & `tmp/blspy-2.0.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blspy-2.0.0b3.tar", last modified: Tue Jun 13 16:43:59 2023, max compression
+gzip compressed data, was "blspy-2.0.1b1.tar", last modified: Thu Jun 22 19:07:45 2023, max compression
```

## Comparing `blspy-2.0.0b3.tar` & `blspy-2.0.1b1.tar`

### file list

```diff
@@ -1,100 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:43:59.431975 blspy-2.0.0b3/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-13 16:43:49.000000 blspy-2.0.0b3/.clang-format
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-13 16:43:49.000000 blspy-2.0.0b3/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:43:59.419975 blspy-2.0.0b3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:43:59.423975 blspy-2.0.0b3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-06-13 16:43:49.000000 blspy-2.0.0b3/.github/workflows/build-test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    10138 2023-06-13 16:43:49.000000 blspy-2.0.0b3/.github/workflows/build-wheels.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-06-13 16:43:49.000000 blspy-2.0.0b3/.github/workflows/js-bindings.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-13 16:43:49.000000 blspy-2.0.0b3/.github/workflows/stale-issue.yml
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-13 16:43:49.000000 blspy-2.0.0b3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-13 16:43:49.000000 blspy-2.0.0b3/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-06-13 16:43:49.000000 blspy-2.0.0b3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-13 16:43:49.000000 blspy-2.0.0b3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11844 2023-06-13 16:43:59.431975 blspy-2.0.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-06-13 16:43:49.000000 blspy-2.0.0b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:43:59.423975 blspy-2.0.0b3/blspy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11844 2023-06-13 16:43:59.000000 blspy-2.0.0b3/blspy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-06-13 16:43:59.000000 blspy-2.0.0b3/blspy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 16:43:59.000000 blspy-2.0.0b3/blspy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 16:43:59.000000 blspy-2.0.0b3/blspy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-13 16:43:59.000000 blspy-2.0.0b3/blspy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-13 16:43:59.000000 blspy-2.0.0b3/blspy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:43:59.423975 blspy-2.0.0b3/cmake_modules/
--rw-r--r--   0 runner    (1001) docker     (123)     9884 2023-06-13 16:43:49.000000 blspy-2.0.0b3/cmake_modules/Findsodium.cmake
--rwxr-xr-x   0 runner    (1001) docker     (123)      158 2023-06-13 16:43:49.000000 blspy-2.0.0b3/emsdk_build.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:43:59.423975 blspy-2.0.0b3/js-bindings/
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js-bindings/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js-bindings/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js-bindings/blsjs.d.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js-bindings/helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js-bindings/helpers.h
--rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js-bindings/jsbindings.cpp
--rw-r--r--   0 runner    (1001) docker     (123)   126728 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js-bindings/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js-bindings/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:43:59.427975 blspy-2.0.0b3/js-bindings/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js-bindings/tests/PrivateKey.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js-bindings/tests/PublicKey.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js-bindings/tests/Signature.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js-bindings/tests/karma.conf.js
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js-bindings/tests/karma.test.js
--rw-r--r--   0 runner    (1001) docker     (123)    19006 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js-bindings/tests/test.js
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js-bindings/tests/typings.spec.ts
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js-bindings/tests/webpack.config.js
--rw-r--r--   0 runner    (1001) docker     (123)    13186 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js-bindings/tests/yarn.lock
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:43:59.427975 blspy-2.0.0b3/js-bindings/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js-bindings/wrappers/G1ElementWrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js-bindings/wrappers/G1ElementWrapper.h
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js-bindings/wrappers/G2ElementWrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js-bindings/wrappers/G2ElementWrapper.h
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js-bindings/wrappers/JSWrapper.h
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js-bindings/wrappers/PrivateKeyWrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js-bindings/wrappers/PrivateKeyWrapper.h
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js-bindings/wrappers/SchemeMPLWrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js-bindings/wrappers/SchemeMPLWrapper.h
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js-bindings/wrappers/UtilWrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js-bindings/wrappers/UtilWrapper.h
--rwxr-xr-x   0 runner    (1001) docker     (123)      219 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js_build.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      272 2023-06-13 16:43:49.000000 blspy-2.0.0b3/js_test.sh
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-13 16:43:49.000000 blspy-2.0.0b3/lgtm.yml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-13 16:43:49.000000 blspy-2.0.0b3/mypi.ini
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-13 16:43:49.000000 blspy-2.0.0b3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:43:59.427975 blspy-2.0.0b3/python-bindings/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-13 16:43:49.000000 blspy-2.0.0b3/python-bindings/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-06-13 16:43:49.000000 blspy-2.0.0b3/python-bindings/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-13 16:43:49.000000 blspy-2.0.0b3/python-bindings/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)    29858 2023-06-13 16:43:49.000000 blspy-2.0.0b3/python-bindings/pythonbindings.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    17701 2023-06-13 16:43:49.000000 blspy-2.0.0b3/python-bindings/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:43:59.427975 blspy-2.0.0b3/python-impl/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-13 16:43:49.000000 blspy-2.0.0b3/python-impl/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-06-13 16:43:49.000000 blspy-2.0.0b3/python-impl/bls12381.py
--rw-r--r--   0 runner    (1001) docker     (123)    17476 2023-06-13 16:43:49.000000 blspy-2.0.0b3/python-impl/ec.py
--rw-r--r--   0 runner    (1001) docker     (123)    21950 2023-06-13 16:43:49.000000 blspy-2.0.0b3/python-impl/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-06-13 16:43:49.000000 blspy-2.0.0b3/python-impl/hash_to_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-06-13 16:43:49.000000 blspy-2.0.0b3/python-impl/hd_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-13 16:43:49.000000 blspy-2.0.0b3/python-impl/hkdf.py
--rw-r--r--   0 runner    (1001) docker     (123)    26234 2023-06-13 16:43:49.000000 blspy-2.0.0b3/python-impl/impl-test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7389 2023-06-13 16:43:49.000000 blspy-2.0.0b3/python-impl/op_swu_g2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-06-13 16:43:49.000000 blspy-2.0.0b3/python-impl/pairing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-06-13 16:43:49.000000 blspy-2.0.0b3/python-impl/private_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-06-13 16:43:49.000000 blspy-2.0.0b3/python-impl/schemes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-13 16:43:49.000000 blspy-2.0.0b3/python-impl/util.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 16:43:59.431975 blspy-2.0.0b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-06-13 16:43:49.000000 blspy-2.0.0b3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:43:59.431975 blspy-2.0.0b3/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-13 16:43:49.000000 blspy-2.0.0b3/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-13 16:43:49.000000 blspy-2.0.0b3/src/bls.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-13 16:43:49.000000 blspy-2.0.0b3/src/bls.hpp
--rw-r--r--   0 runner    (1001) docker     (123)   261840 2023-06-13 16:43:49.000000 blspy-2.0.0b3/src/blstasm.lib
--rw-r--r--   0 runner    (1001) docker     (123)    11614 2023-06-13 16:43:49.000000 blspy-2.0.0b3/src/elements.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-06-13 16:43:49.000000 blspy-2.0.0b3/src/elements.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-06-13 16:43:49.000000 blspy-2.0.0b3/src/hdkeys.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-06-13 16:43:49.000000 blspy-2.0.0b3/src/hkdf.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-06-13 16:43:49.000000 blspy-2.0.0b3/src/privatekey.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-06-13 16:43:49.000000 blspy-2.0.0b3/src/privatekey.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    19459 2023-06-13 16:43:49.000000 blspy-2.0.0b3/src/schemes.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7176 2023-06-13 16:43:49.000000 blspy-2.0.0b3/src/schemes.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-06-13 16:43:49.000000 blspy-2.0.0b3/src/test-bench.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-13 16:43:49.000000 blspy-2.0.0b3/src/test-utils.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    56462 2023-06-13 16:43:49.000000 blspy-2.0.0b3/src/test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-13 16:43:49.000000 blspy-2.0.0b3/src/util.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:07:45.697795 blspy-2.0.1b1/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-22 19:07:35.000000 blspy-2.0.1b1/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-22 19:07:35.000000 blspy-2.0.1b1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:07:45.685795 blspy-2.0.1b1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:07:45.689795 blspy-2.0.1b1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-22 19:07:35.000000 blspy-2.0.1b1/.github/workflows/build-blst-nightly.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-06-22 19:07:35.000000 blspy-2.0.1b1/.github/workflows/build-test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-06-22 19:07:35.000000 blspy-2.0.1b1/.github/workflows/build-wheels.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-06-22 19:07:35.000000 blspy-2.0.1b1/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-22 19:07:35.000000 blspy-2.0.1b1/.github/workflows/js-bindings.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-22 19:07:35.000000 blspy-2.0.1b1/.github/workflows/stale-issue.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-22 19:07:35.000000 blspy-2.0.1b1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-22 19:07:35.000000 blspy-2.0.1b1/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-06-22 19:07:35.000000 blspy-2.0.1b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-22 19:07:35.000000 blspy-2.0.1b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11418 2023-06-22 19:07:45.697795 blspy-2.0.1b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11118 2023-06-22 19:07:35.000000 blspy-2.0.1b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:07:45.689795 blspy-2.0.1b1/blspy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11418 2023-06-22 19:07:45.000000 blspy-2.0.1b1/blspy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-06-22 19:07:45.000000 blspy-2.0.1b1/blspy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 19:07:45.000000 blspy-2.0.1b1/blspy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 19:07:45.000000 blspy-2.0.1b1/blspy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-22 19:07:45.000000 blspy-2.0.1b1/blspy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-22 19:07:45.000000 blspy-2.0.1b1/blspy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:07:45.689795 blspy-2.0.1b1/cmake_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     9884 2023-06-22 19:07:35.000000 blspy-2.0.1b1/cmake_modules/Findsodium.cmake
+-rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-06-22 19:07:35.000000 blspy-2.0.1b1/emsdk_build.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:07:45.689795 blspy-2.0.1b1/js-bindings/
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-22 19:07:35.000000 blspy-2.0.1b1/js-bindings/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-06-22 19:07:35.000000 blspy-2.0.1b1/js-bindings/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-22 19:07:35.000000 blspy-2.0.1b1/js-bindings/blsjs.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-22 19:07:35.000000 blspy-2.0.1b1/js-bindings/helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-22 19:07:35.000000 blspy-2.0.1b1/js-bindings/helpers.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-06-22 19:07:35.000000 blspy-2.0.1b1/js-bindings/jsbindings.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)   129248 2023-06-22 19:07:35.000000 blspy-2.0.1b1/js-bindings/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-06-22 19:07:35.000000 blspy-2.0.1b1/js-bindings/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:07:45.689795 blspy-2.0.1b1/js-bindings/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-06-22 19:07:35.000000 blspy-2.0.1b1/js-bindings/tests/PrivateKey.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-06-22 19:07:35.000000 blspy-2.0.1b1/js-bindings/tests/PublicKey.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-06-22 19:07:35.000000 blspy-2.0.1b1/js-bindings/tests/Signature.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-22 19:07:35.000000 blspy-2.0.1b1/js-bindings/tests/karma.conf.js
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-22 19:07:35.000000 blspy-2.0.1b1/js-bindings/tests/karma.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19006 2023-06-22 19:07:35.000000 blspy-2.0.1b1/js-bindings/tests/test.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-06-22 19:07:35.000000 blspy-2.0.1b1/js-bindings/tests/typings.spec.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-22 19:07:35.000000 blspy-2.0.1b1/js-bindings/tests/webpack.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13186 2023-06-22 19:07:35.000000 blspy-2.0.1b1/js-bindings/tests/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:07:45.693795 blspy-2.0.1b1/js-bindings/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-06-22 19:07:35.000000 blspy-2.0.1b1/js-bindings/wrappers/G1ElementWrapper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-22 19:07:35.000000 blspy-2.0.1b1/js-bindings/wrappers/G1ElementWrapper.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-22 19:07:35.000000 blspy-2.0.1b1/js-bindings/wrappers/G2ElementWrapper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-06-22 19:07:35.000000 blspy-2.0.1b1/js-bindings/wrappers/G2ElementWrapper.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-22 19:07:35.000000 blspy-2.0.1b1/js-bindings/wrappers/JSWrapper.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-06-22 19:07:35.000000 blspy-2.0.1b1/js-bindings/wrappers/PrivateKeyWrapper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-06-22 19:07:35.000000 blspy-2.0.1b1/js-bindings/wrappers/PrivateKeyWrapper.h
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-22 19:07:35.000000 blspy-2.0.1b1/js-bindings/wrappers/SchemeMPLWrapper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-06-22 19:07:35.000000 blspy-2.0.1b1/js-bindings/wrappers/SchemeMPLWrapper.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-22 19:07:35.000000 blspy-2.0.1b1/js-bindings/wrappers/UtilWrapper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-22 19:07:35.000000 blspy-2.0.1b1/js-bindings/wrappers/UtilWrapper.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-06-22 19:07:35.000000 blspy-2.0.1b1/js_build.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      272 2023-06-22 19:07:35.000000 blspy-2.0.1b1/js_test.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-22 19:07:35.000000 blspy-2.0.1b1/lgtm.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-22 19:07:35.000000 blspy-2.0.1b1/mypi.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-22 19:07:35.000000 blspy-2.0.1b1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:07:45.693795 blspy-2.0.1b1/python-bindings/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-22 19:07:35.000000 blspy-2.0.1b1/python-bindings/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-06-22 19:07:35.000000 blspy-2.0.1b1/python-bindings/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-22 19:07:35.000000 blspy-2.0.1b1/python-bindings/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29858 2023-06-22 19:07:35.000000 blspy-2.0.1b1/python-bindings/pythonbindings.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17701 2023-06-22 19:07:35.000000 blspy-2.0.1b1/python-bindings/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:07:45.693795 blspy-2.0.1b1/python-impl/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-22 19:07:35.000000 blspy-2.0.1b1/python-impl/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-06-22 19:07:35.000000 blspy-2.0.1b1/python-impl/bls12381.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17476 2023-06-22 19:07:35.000000 blspy-2.0.1b1/python-impl/ec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21950 2023-06-22 19:07:35.000000 blspy-2.0.1b1/python-impl/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-06-22 19:07:35.000000 blspy-2.0.1b1/python-impl/hash_to_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-06-22 19:07:35.000000 blspy-2.0.1b1/python-impl/hd_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-22 19:07:35.000000 blspy-2.0.1b1/python-impl/hkdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26234 2023-06-22 19:07:35.000000 blspy-2.0.1b1/python-impl/impl-test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7389 2023-06-22 19:07:35.000000 blspy-2.0.1b1/python-impl/op_swu_g2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-06-22 19:07:35.000000 blspy-2.0.1b1/python-impl/pairing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-06-22 19:07:35.000000 blspy-2.0.1b1/python-impl/private_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-06-22 19:07:35.000000 blspy-2.0.1b1/python-impl/schemes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-22 19:07:35.000000 blspy-2.0.1b1/python-impl/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 19:07:45.697795 blspy-2.0.1b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-06-22 19:07:35.000000 blspy-2.0.1b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:07:45.697795 blspy-2.0.1b1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-22 19:07:35.000000 blspy-2.0.1b1/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-22 19:07:35.000000 blspy-2.0.1b1/src/bls.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-22 19:07:35.000000 blspy-2.0.1b1/src/bls.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11518 2023-06-22 19:07:35.000000 blspy-2.0.1b1/src/elements.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-06-22 19:07:35.000000 blspy-2.0.1b1/src/elements.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6310 2023-06-22 19:07:35.000000 blspy-2.0.1b1/src/hdkeys.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-06-22 19:07:35.000000 blspy-2.0.1b1/src/hkdf.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-06-22 19:07:35.000000 blspy-2.0.1b1/src/privatekey.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-06-22 19:07:35.000000 blspy-2.0.1b1/src/privatekey.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17747 2023-06-22 19:07:35.000000 blspy-2.0.1b1/src/schemes.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7176 2023-06-22 19:07:35.000000 blspy-2.0.1b1/src/schemes.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-06-22 19:07:35.000000 blspy-2.0.1b1/src/test-bench.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-22 19:07:35.000000 blspy-2.0.1b1/src/test-utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    58076 2023-06-22 19:07:35.000000 blspy-2.0.1b1/src/test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-06-22 19:07:35.000000 blspy-2.0.1b1/src/util.hpp
```

### Comparing `blspy-2.0.0b3/.github/workflows/build-test.yaml` & `blspy-2.0.1b1/.github/workflows/build-test.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -75,18 +75,16 @@
         echo "Running ./src/runtest"
         ./src/runtest
         valgrind --leak-check=full --show-leak-kinds=all --errors-for-leak-kinds=all  ./src/runtest
 
     - name: Mac OS build C++ and test
       if: startsWith(matrix.os, 'macos')
       run: |
-        ls -l
         export MACOSX_DEPLOYMENT_TARGET=10.14
         mkdir -p build
-        ls -l build
         cd build
         cmake ../
         cmake --build . -- -j 6
         echo "Running ./src/runtest"
         ./src/runtest
 
     - name: Test pure python implementation
```

### Comparing `blspy-2.0.0b3/.github/workflows/build-wheels.yml` & `blspy-2.0.1b1/.github/workflows/build-wheels.yml`

 * *Files 5% similar despite different names*

```diff
@@ -40,39 +40,39 @@
             matrix: windows
             runs-on:
               intel: [windows-latest]
         python:
           - major-dot-minor: '3.7'
             cibw-build: 'cp37-*'
             manylinux:
-              arch: manylinux2014
+              arm: manylinux2014
               intel: manylinux2014
             matrix: '3.7'
           - major-dot-minor: '3.8'
             cibw-build: 'cp38-*'
             manylinux:
-              arch: manylinux2014
+              arm: manylinux2014
               intel: manylinux2014
             matrix: '3.8'
           - major-dot-minor: '3.9'
             cibw-build: 'cp39-*'
             manylinux:
-              arch: manylinux2014
+              arm: manylinux2014
               intel: manylinux2014
             matrix: '3.9'
           - major-dot-minor: '3.10'
             cibw-build: 'cp310-*'
             manylinux:
-              arch: manylinux2014
+              arm: manylinux2014
               intel: manylinux2014
             matrix: '3.10'
           - major-dot-minor: '3.11'
             cibw-build: 'cp311-*'
             manylinux:
-              arch: manylinux2014
+              arm: manylinux2014
               intel: manylinux2014
             matrix: '3.11'
         arch:
           - name: ARM
             matrix: arm
           - name: Intel
             matrix: intel
@@ -109,15 +109,14 @@
 
     - name: Checkout code
       uses: actions/checkout@v3
       with:
         fetch-depth: 0
 
     - name: Set Env
-      if: env.RUNNER_ARCH != 'ARM64'
       uses: Chia-Network/actions/setjobenv@main
       env:
         GH_TOKEN: ${{ secrets.GITHUB_TOKEN }}
 
     - uses: chia-network/actions/setup-python@main
       with:
         python-version: ${{ matrix.python.major-dot-minor }}
@@ -147,25 +146,18 @@
           && rm -f /usr/bin/cmake
           && cmake --version
           && uname -a
         CIBW_BEFORE_BUILD_LINUX: >
           python -m pip install --upgrade pip
         CIBW_ARCHS_MACOS: ${{ matrix.os.cibw-archs-macos[matrix.arch.matrix] }}
         CIBW_BEFORE_ALL_MACOS: >
-          brew install boost cmake
+          brew install cmake
         CIBW_BEFORE_BUILD_MACOS: >
           python -m pip install --upgrade pip
         CIBW_ENVIRONMENT_MACOS: "MACOSX_DEPLOYMENT_TARGET=10.14"
-        CIBW_BEFORE_ALL_WINDOWS: >
-          curl -L https://download.libsodium.org/libsodium/releases/libsodium-1.0.18-stable-msvc.zip > libsodium-1.0.18-stable-msvc.zip
-          && 7z x libsodium-1.0.18-stable-msvc.zip
-          && git clone https://github.com/supranational/blst.git
-          && ls -l blst
-        CIBW_REPAIR_WHEEL_COMMAND_WINDOWS: >
-          cp {wheel} {dest_dir}
         CIBW_TEST_REQUIRES: pytest
         CIBW_TEST_COMMAND: py.test -v {project}/python-bindings/test.py
       run:
         pipx run --spec='cibuildwheel==2.9.0' cibuildwheel --output-dir dist 2>&1
 
     - name: Upload artifacts
       uses: actions/upload-artifact@v3
```

### Comparing `blspy-2.0.0b3/.github/workflows/js-bindings.yml` & `blspy-2.0.1b1/.github/workflows/js-bindings.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 name: Build & Publish JS Bindings
 
 on:
   push:
     branches:
       - main
-    tags:
-      - '**'
+  release:
+    types: [published]
   pull_request:
     branches:
       - '**'
 
 concurrency:
   # SHA is added to the end if on `main` to let all main workflows run
   group: ${{ github.ref }}-${{ github.workflow }}-${{ github.event_name }}-${{ (github.ref == 'refs/heads/main') && github.sha || '' }}
@@ -19,14 +19,19 @@
   js_bindings:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
 
+      - name: Set Env
+        uses: Chia-Network/actions/setjobenv@main
+        env:
+          GH_TOKEN: ${{ secrets.GITHUB_TOKEN }}
+
       - uses: actions/setup-node@v3
         with:
           node-version: 16
 
       - name: Install emsdk
         uses: mymindstorm/setup-emsdk@v12
 
@@ -42,15 +47,15 @@
         run: |
           jq --arg VER "$SOURCE_TAG" '.version=$VER' package.json > temp.json && mv temp.json package.json
 
       - name: Build JS
         run: ./js_build.sh
 
       - name: Publish
-        if: startsWith(github.ref, 'refs/tags/')
+        if: env.FULL_RELEASE == 'true'
         working-directory: ${{ github.workspace }}/js_build/js-bindings
         env:
           NPM_TOKEN: ${{ secrets.NPM_TOKEN }}
         run: |
           echo "//registry.npmjs.org/:_authToken=${NPM_TOKEN}" > .npmrc
           npm publish --access public
```

### Comparing `blspy-2.0.0b3/.github/workflows/stale-issue.yml` & `blspy-2.0.1b1/.github/workflows/stale-issue.yml`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b3/CMakeLists.txt` & `blspy-2.0.1b1/CMakeLists.txt`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,21 @@
 if(NOT CMAKE_BUILD_TYPE)
   set(CMAKE_BUILD_TYPE "Release"
     CACHE STRING "Possible values are empty, Debug, Release, RelWithDebInfo, MinSizeRel, ..."
     FORCE
   )
 endif()
 
-project(BLS C CXX ASM)
+project(BLS)
+
+if(MSVC)
+  enable_language(ASM_MASM)
+else()
+  enable_language(ASM)
+endif()
 
 set(BUILD_BLS_PYTHON_BINDINGS "1" CACHE STRING "")
 set(BUILD_BLS_TESTS "1" CACHE STRING "")
 set(BUILD_BLS_BENCHMARKS "1" CACHE STRING "")
 
 message(STATUS "Build python bindings: ${BUILD_BLS_PYTHON_BINDINGS}")
 message(STATUS "Build tests: ${BUILD_BLS_TESTS}")
@@ -29,34 +35,39 @@
   ${CMAKE_CURRENT_SOURCE_DIR}/cmake_modules
 )
 
 include(FetchContent)
 
 FetchContent_Declare(Sodium
   GIT_REPOSITORY https://github.com/AmineKhaldi/libsodium-cmake.git
+
   # Latest commit at the moment this was added here
   # Anchored to libsodium v1.0.18
   GIT_TAG f73a3fe1afdc4e37ac5fe0ddd401bf521f6bba65
 )
 set(SODIUM_PCH "on" CACHE STRING "")
 set(SODIUM_DISABLE_TESTS "on" CACHE STRING "")
 set(SODIUM_CHIA_MINIMAL "on" CACHE STRING "")
 FetchContent_MakeAvailable(Sodium)
 
-set(BLST_GIT_TAG "a8cd361c9f671577aeab3f074098443af92a53fc")
-set(BLST_REPOSITORY "https://github.com/supranational/blst")
+if (DEFINED ENV{BLST_MAIN})
+  set(BLST_GIT_TAG "origin/master")
+else ()
+  # This is currently anchored to upstream 6b837a0921cf41e501faaee1976a4035ae29d893 dated 2023-06-16
+  set(BLST_GIT_TAG "6b837a0921cf41e501faaee1976a4035ae29d893")
+endif ()
+set(BLST_REPOSITORY "https://github.com/supranational/blst.git")
 
 message(STATUS "blst will be built from: ${BLST_GIT_TAG} and repository ${BLST_REPOSITORY}")
 
 FetchContent_Declare(
   blst
   GIT_REPOSITORY ${BLST_REPOSITORY}
   GIT_TAG ${BLST_GIT_TAG}
 )
-
 FetchContent_MakeAvailable(blst)
 
 add_subdirectory(src)
 
 if(EMSCRIPTEN)
   add_subdirectory(js-bindings)
 else()
```

### Comparing `blspy-2.0.0b3/LICENSE` & `blspy-2.0.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b3/PKG-INFO` & `blspy-2.0.1b1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blspy
-Version: 2.0.0b3
+Version: 2.0.1b1
 Summary: BLS signatures in c++ (python bindings)
 Home-page: https://github.com/Chia-Network/bls-signatures
 Author: Mariano Sorgente
 Author-email: mariano@chia.net
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -12,18 +12,17 @@
 # BLS Signatures implementation
 
 [![Build and Test C++, Javascript, and Python](https://github.com/Chia-Network/bls-signatures/actions/workflows/build-test.yaml/badge.svg)](https://github.com/Chia-Network/bls-signatures/actions/workflows/build-test.yaml)
 ![PyPI](https://img.shields.io/pypi/v/blspy?logo=pypi)
 ![PyPI - Format](https://img.shields.io/pypi/format/blspy?logo=pypi)
 ![GitHub](https://img.shields.io/github/license/Chia-Network/bls-signatures?logo=Github)
 
-[![Total alerts](https://img.shields.io/lgtm/alerts/g/Chia-Network/bls-signatures.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/Chia-Network/bls-signatures/alerts/)
-[![Language grade: JavaScript](https://img.shields.io/lgtm/grade/javascript/g/Chia-Network/bls-signatures.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/Chia-Network/bls-signatures/context:javascript)
-[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/Chia-Network/bls-signatures.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/Chia-Network/bls-signatures/context:python)
-[![Language grade: C/C++](https://img.shields.io/lgtm/grade/cpp/g/Chia-Network/bls-signatures.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/Chia-Network/bls-signatures/context:cpp)
+[![CodeQL](https://github.com/Chia-Network/bls-signatures/actions/workflows/codeql.yml/badge.svg)](https://github.com/Chia-Network/bls-signatures/actions/workflows/codeql.yml)
+
+[![Coverage Status](https://coveralls.io/repos/github/Chia-Network/bls-signatures/badge.svg?branch=main)](https://coveralls.io/github/Chia-Network/bls-signatures?branch=main)
 
 NOTE: THIS LIBRARY IS NOT YET FORMALLY REVIEWED FOR SECURITY
 
 NOTE: THIS LIBRARY WAS SHIFTED TO THE IETF BLS SPECIFICATION ON 7/16/20
 
 Implements BLS signatures with aggregation using [blst library](https://github.com/supranational/blst.git)
 for cryptographic primitives (pairings, EC, hashing) according to the
```

### Comparing `blspy-2.0.0b3/README.md` & `blspy-2.0.1b1/blspy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,28 @@
+Metadata-Version: 2.1
+Name: blspy
+Version: 2.0.1b1
+Summary: BLS signatures in c++ (python bindings)
+Home-page: https://github.com/Chia-Network/bls-signatures
+Author: Mariano Sorgente
+Author-email: mariano@chia.net
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # BLS Signatures implementation
 
 [![Build and Test C++, Javascript, and Python](https://github.com/Chia-Network/bls-signatures/actions/workflows/build-test.yaml/badge.svg)](https://github.com/Chia-Network/bls-signatures/actions/workflows/build-test.yaml)
 ![PyPI](https://img.shields.io/pypi/v/blspy?logo=pypi)
 ![PyPI - Format](https://img.shields.io/pypi/format/blspy?logo=pypi)
 ![GitHub](https://img.shields.io/github/license/Chia-Network/bls-signatures?logo=Github)
 
-[![Total alerts](https://img.shields.io/lgtm/alerts/g/Chia-Network/bls-signatures.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/Chia-Network/bls-signatures/alerts/)
-[![Language grade: JavaScript](https://img.shields.io/lgtm/grade/javascript/g/Chia-Network/bls-signatures.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/Chia-Network/bls-signatures/context:javascript)
-[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/Chia-Network/bls-signatures.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/Chia-Network/bls-signatures/context:python)
-[![Language grade: C/C++](https://img.shields.io/lgtm/grade/cpp/g/Chia-Network/bls-signatures.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/Chia-Network/bls-signatures/context:cpp)
+[![CodeQL](https://github.com/Chia-Network/bls-signatures/actions/workflows/codeql.yml/badge.svg)](https://github.com/Chia-Network/bls-signatures/actions/workflows/codeql.yml)
+
+[![Coverage Status](https://coveralls.io/repos/github/Chia-Network/bls-signatures/badge.svg?branch=main)](https://coveralls.io/github/Chia-Network/bls-signatures?branch=main)
 
 NOTE: THIS LIBRARY IS NOT YET FORMALLY REVIEWED FOR SECURITY
 
 NOTE: THIS LIBRARY WAS SHIFTED TO THE IETF BLS SPECIFICATION ON 7/16/20
 
 Implements BLS signatures with aggregation using [blst library](https://github.com/supranational/blst.git)
 for cryptographic primitives (pairings, EC, hashing) according to the
```

### Comparing `blspy-2.0.0b3/blspy.egg-info/PKG-INFO` & `blspy-2.0.1b1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,17 @@
-Metadata-Version: 2.1
-Name: blspy
-Version: 2.0.0b3
-Summary: BLS signatures in c++ (python bindings)
-Home-page: https://github.com/Chia-Network/bls-signatures
-Author: Mariano Sorgente
-Author-email: mariano@chia.net
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # BLS Signatures implementation
 
 [![Build and Test C++, Javascript, and Python](https://github.com/Chia-Network/bls-signatures/actions/workflows/build-test.yaml/badge.svg)](https://github.com/Chia-Network/bls-signatures/actions/workflows/build-test.yaml)
 ![PyPI](https://img.shields.io/pypi/v/blspy?logo=pypi)
 ![PyPI - Format](https://img.shields.io/pypi/format/blspy?logo=pypi)
 ![GitHub](https://img.shields.io/github/license/Chia-Network/bls-signatures?logo=Github)
 
-[![Total alerts](https://img.shields.io/lgtm/alerts/g/Chia-Network/bls-signatures.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/Chia-Network/bls-signatures/alerts/)
-[![Language grade: JavaScript](https://img.shields.io/lgtm/grade/javascript/g/Chia-Network/bls-signatures.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/Chia-Network/bls-signatures/context:javascript)
-[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/Chia-Network/bls-signatures.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/Chia-Network/bls-signatures/context:python)
-[![Language grade: C/C++](https://img.shields.io/lgtm/grade/cpp/g/Chia-Network/bls-signatures.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/Chia-Network/bls-signatures/context:cpp)
+[![CodeQL](https://github.com/Chia-Network/bls-signatures/actions/workflows/codeql.yml/badge.svg)](https://github.com/Chia-Network/bls-signatures/actions/workflows/codeql.yml)
+
+[![Coverage Status](https://coveralls.io/repos/github/Chia-Network/bls-signatures/badge.svg?branch=main)](https://coveralls.io/github/Chia-Network/bls-signatures?branch=main)
 
 NOTE: THIS LIBRARY IS NOT YET FORMALLY REVIEWED FOR SECURITY
 
 NOTE: THIS LIBRARY WAS SHIFTED TO THE IETF BLS SPECIFICATION ON 7/16/20
 
 Implements BLS signatures with aggregation using [blst library](https://github.com/supranational/blst.git)
 for cryptographic primitives (pairings, EC, hashing) according to the
```

### Comparing `blspy-2.0.0b3/blspy.egg-info/SOURCES.txt` & `blspy-2.0.1b1/blspy.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -9,16 +9,18 @@
 js_build.sh
 js_test.sh
 lgtm.yml
 mypi.ini
 pyproject.toml
 setup.py
 ./
+.github/workflows/build-blst-nightly.yml
 .github/workflows/build-test.yaml
 .github/workflows/build-wheels.yml
+.github/workflows/codeql.yml
 .github/workflows/js-bindings.yml
 .github/workflows/stale-issue.yml
 blspy.egg-info/PKG-INFO
 blspy.egg-info/SOURCES.txt
 blspy.egg-info/dependency_links.txt
 blspy.egg-info/not-zip-safe
 blspy.egg-info/requires.txt
@@ -69,15 +71,14 @@
 python-impl/pairing.py
 python-impl/private_key.py
 python-impl/schemes.py
 python-impl/util.py
 src/CMakeLists.txt
 src/bls.cpp
 src/bls.hpp
-src/blstasm.lib
 src/elements.cpp
 src/elements.hpp
 src/hdkeys.hpp
 src/hkdf.hpp
 src/privatekey.cpp
 src/privatekey.hpp
 src/schemes.cpp
```

### Comparing `blspy-2.0.0b3/cmake_modules/Findsodium.cmake` & `blspy-2.0.1b1/cmake_modules/Findsodium.cmake`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b3/js-bindings/CMakeLists.txt` & `blspy-2.0.1b1/js-bindings/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b3/js-bindings/README.md` & `blspy-2.0.1b1/js-bindings/README.md`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b3/js-bindings/blsjs.d.ts` & `blspy-2.0.1b1/js-bindings/blsjs.d.ts`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b3/js-bindings/helpers.cpp` & `blspy-2.0.1b1/js-bindings/helpers.cpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b3/js-bindings/helpers.h` & `blspy-2.0.1b1/js-bindings/helpers.h`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b3/js-bindings/jsbindings.cpp` & `blspy-2.0.1b1/js-bindings/jsbindings.cpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b3/js-bindings/package-lock.json` & `blspy-2.0.1b1/js-bindings/package-lock.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9936420727142158%*

 * *Differences: {"'dependencies'": "{'@types/cors': {'version': '2.8.13', 'resolved': "*

 * *                   "'https://registry.npmjs.org/@types/cors/-/cors-2.8.13.tgz', 'integrity': "*

 * *                   "'sha512-RG8AStHlUiV5ysZQKq97copd2UmVYw3/pRMLefISZ3S1hK104Cwm7iLQ3fTKx+lsUH2CE8FlLaYeEA2LSeqYUA==', "*

 * *                   "'requires': OrderedDict([('@types/node', '*')])}, '@types/eslint': {'version': "*

 * *                   "'8.40.0', 'resolved': "*

 * *                   "'https://registry.npmjs.org/@types/eslint/-/eslint-8.40.0.t […]*

```diff
@@ -1,9 +1,15 @@
 {
     "dependencies": {
+        "@colors/colors": {
+            "dev": true,
+            "integrity": "sha512-ooWCrlZP11i8GImSjTHYHLkvFDP48nS4+204nGb1RiX/WXYHmJA2III9/e2DWVabCESdW7hBAEzHRqUn9OUVvQ==",
+            "resolved": "https://registry.npmjs.org/@colors/colors/-/colors-1.5.0.tgz",
+            "version": "1.5.0"
+        },
         "@jridgewell/gen-mapping": {
             "dev": true,
             "integrity": "sha512-HLhSWOLRi875zjjMG/r+Nv0oCW8umGb0BgEhyX3dDX3egwZtB8PqLnjz3yedt8R5StBrzcg4aBpnh8UA9D1BoQ==",
             "requires": {
                 "@jridgewell/set-array": "^1.0.1",
                 "@jridgewell/sourcemap-codec": "^1.4.10",
                 "@jridgewell/trace-mapping": "^0.3.9"
@@ -45,227 +51,224 @@
             "requires": {
                 "@jridgewell/resolve-uri": "3.1.0",
                 "@jridgewell/sourcemap-codec": "1.4.14"
             },
             "resolved": "https://registry.npmjs.org/@jridgewell/trace-mapping/-/trace-mapping-0.3.18.tgz",
             "version": "0.3.18"
         },
-        "@socket.io/base64-arraybuffer": {
-            "dev": true,
-            "integrity": "sha512-dOlCBKnDw4iShaIsH/bxujKTM18+2TOAsYz+KSc11Am38H4q5Xw8Bbz97ZYdrVNM+um3p7w86Bvvmcn9q+5+eQ==",
-            "resolved": "https://registry.npmjs.org/@socket.io/base64-arraybuffer/-/base64-arraybuffer-1.0.2.tgz",
-            "version": "1.0.2"
-        },
         "@socket.io/component-emitter": {
             "dev": true,
             "integrity": "sha512-+9jVqKhRSpsc591z5vX+X5Yyw+he/HCB4iQ/RYxw35CEPaY1gnsNE43nf9n9AaYjAQrTiI/mOwKUKdUs9vf7Xg==",
             "resolved": "https://registry.npmjs.org/@socket.io/component-emitter/-/component-emitter-3.1.0.tgz",
             "version": "3.1.0"
         },
         "@types/cookie": {
             "dev": true,
             "integrity": "sha512-XW/Aa8APYr6jSVVA1y/DEIZX0/GMKLEVekNG727R8cs56ahETkRAy/3DR7+fJyh7oUgGwNQaRfXCun0+KbWY7Q==",
             "resolved": "https://registry.npmjs.org/@types/cookie/-/cookie-0.4.1.tgz",
             "version": "0.4.1"
         },
         "@types/cors": {
             "dev": true,
-            "integrity": "sha512-vt+kDhq/M2ayberEtJcIN/hxXy1Pk+59g2FV/ZQceeaTyCtCucjL2Q7FXlFjtWn4n15KCr1NE2lNNFhp0lEThw==",
-            "resolved": "https://registry.npmjs.org/@types/cors/-/cors-2.8.12.tgz",
-            "version": "2.8.12"
+            "integrity": "sha512-RG8AStHlUiV5ysZQKq97copd2UmVYw3/pRMLefISZ3S1hK104Cwm7iLQ3fTKx+lsUH2CE8FlLaYeEA2LSeqYUA==",
+            "requires": {
+                "@types/node": "*"
+            },
+            "resolved": "https://registry.npmjs.org/@types/cors/-/cors-2.8.13.tgz",
+            "version": "2.8.13"
         },
         "@types/eslint": {
             "dev": true,
-            "integrity": "sha512-Piet7dG2JBuDIfohBngQ3rCt7MgO9xCO4xIMKxBThCq5PNRB91IjlJ10eJVwfoNtvTErmxLzwBZ7rHZtbOMmFQ==",
+            "integrity": "sha512-nbq2mvc/tBrK9zQQuItvjJl++GTN5j06DaPtp3hZCpngmG6Q3xoyEmd0TwZI0gAy/G1X0zhGBbr2imsGFdFV0g==",
             "requires": {
                 "@types/estree": "*",
                 "@types/json-schema": "*"
             },
-            "resolved": "https://registry.npmjs.org/@types/eslint/-/eslint-8.37.0.tgz",
-            "version": "8.37.0"
+            "resolved": "https://registry.npmjs.org/@types/eslint/-/eslint-8.40.0.tgz",
+            "version": "8.40.0"
         },
         "@types/eslint-scope": {
             "dev": true,
             "integrity": "sha512-9K4zoImiZc3HlIp6AVUDE4CWYx22a+lhSZMYNpbjW04+YF0KWj4pJXnEMjdnFTiQibFFmElcsasJXDbdI/EPhA==",
             "requires": {
                 "@types/eslint": "*",
                 "@types/estree": "*"
             },
             "resolved": "https://registry.npmjs.org/@types/eslint-scope/-/eslint-scope-3.7.4.tgz",
             "version": "3.7.4"
         },
         "@types/estree": {
             "dev": true,
-            "integrity": "sha512-CuPgU6f3eT/XgKKPqKd/gLZV1Xmvf1a2R5POBOGQa6uv82xpls89HU5zKeVoyR8XzHd1RGNOlQlvUe3CFkjWNQ==",
-            "resolved": "https://registry.npmjs.org/@types/estree/-/estree-0.0.51.tgz",
-            "version": "0.0.51"
+            "integrity": "sha512-LG4opVs2ANWZ1TJoKc937iMmNstM/d0ae1vNbnBvBhqCSezgVUOzcLCqbI5elV8Vy6WKwKjaqR+zO9VKirBBCA==",
+            "resolved": "https://registry.npmjs.org/@types/estree/-/estree-1.0.1.tgz",
+            "version": "1.0.1"
         },
         "@types/json-schema": {
             "dev": true,
-            "integrity": "sha512-wOuvG1SN4Us4rez+tylwwwCV1psiNVOkJeM3AUWUNWg/jDQY2+HE/444y5gc+jBmRqASOm2Oeh5c1axHobwRKQ==",
-            "resolved": "https://registry.npmjs.org/@types/json-schema/-/json-schema-7.0.11.tgz",
-            "version": "7.0.11"
+            "integrity": "sha512-Hr5Jfhc9eYOQNPYO5WLDq/n4jqijdHNlDXjuAQkkt+mWdQR+XJToOHrsD4cPaMXpn6KO7y2+wM8AZEs8VpBLVA==",
+            "resolved": "https://registry.npmjs.org/@types/json-schema/-/json-schema-7.0.12.tgz",
+            "version": "7.0.12"
         },
         "@types/mocha": {
             "dev": true,
-            "integrity": "sha512-NYrtPht0wGzhwe9+/idPaBB+TqkY9AhTvOLMkThm0IoEfLaiVQZwBwyJ5puCkO3AUCWrmcoePjp2mbFocKy4SQ==",
-            "resolved": "https://registry.npmjs.org/@types/mocha/-/mocha-5.2.7.tgz",
-            "version": "5.2.7"
+            "integrity": "sha512-/fvYntiO1GeICvqbQ3doGDIP97vWmvFt83GKguJ6prmQM2iXZfFcq6YE8KteFyRtX2/h5Hf91BYvPodJKFYv5Q==",
+            "resolved": "https://registry.npmjs.org/@types/mocha/-/mocha-10.0.1.tgz",
+            "version": "10.0.1"
         },
         "@types/node": {
             "dev": true,
-            "integrity": "sha512-3p2M6moxwdDFyPia2ROI8CCkRa9ZzYjvCys2TOE1xgwYDQmY49Cj0cvkdBkzh/rY9gkvzgzYOeECYtB4f0/fDA==",
-            "resolved": "https://registry.npmjs.org/@types/node/-/node-11.15.18.tgz",
-            "version": "11.15.18"
+            "integrity": "sha512-IvGD1CD/nego63ySR7vrAKEX3AJTcmrAN2kn+/sDNLi1Ff5kBzDeEdqWDplK+0HAEoLYej137Sk0cUU8OLOlMg==",
+            "resolved": "https://registry.npmjs.org/@types/node/-/node-20.1.5.tgz",
+            "version": "20.1.5"
         },
         "@webassemblyjs/ast": {
             "dev": true,
-            "integrity": "sha512-ukBh14qFLjxTQNTXocdyksN5QdM28S1CxHt2rdskFyL+xFV7VremuBLVbmCePj+URalXBENx/9Lm7lnhihtCSw==",
+            "integrity": "sha512-IN1xI7PwOvLPgjcf180gC1bqn3q/QaOCwYUahIOhbYUu8KA/3tw2RT/T0Gidi1l7Hhj5D/INhJxiICObqpMu4Q==",
             "requires": {
-                "@webassemblyjs/helper-numbers": "1.11.1",
-                "@webassemblyjs/helper-wasm-bytecode": "1.11.1"
+                "@webassemblyjs/helper-numbers": "1.11.6",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.6"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/ast/-/ast-1.11.1.tgz",
-            "version": "1.11.1"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/ast/-/ast-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "@webassemblyjs/floating-point-hex-parser": {
             "dev": true,
-            "integrity": "sha512-iGRfyc5Bq+NnNuX8b5hwBrRjzf0ocrJPI6GWFodBFzmFnyvrQ83SHKhmilCU/8Jv67i4GJZBMhEzltxzcNagtQ==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/floating-point-hex-parser/-/floating-point-hex-parser-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-ejAj9hfRJ2XMsNHk/v6Fu2dGS+i4UaXBXGemOfQ/JfQ6mdQg/WXtwleQRLLS4OvfDhv8rYnVwH27YJLMyYsxhw==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/floating-point-hex-parser/-/floating-point-hex-parser-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "@webassemblyjs/helper-api-error": {
             "dev": true,
-            "integrity": "sha512-RlhS8CBCXfRUR/cwo2ho9bkheSXG0+NwooXcc3PAILALf2QLdFyj7KGsKRbVc95hZnhnERon4kW/D3SZpp6Tcg==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-api-error/-/helper-api-error-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-o0YkoP4pVu4rN8aTJgAyj9hC2Sv5UlkzCHhxqWj8butaLvnpdc2jOwh4ewE6CX0txSfLn/UYaV/pheS2Txg//Q==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-api-error/-/helper-api-error-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "@webassemblyjs/helper-buffer": {
             "dev": true,
-            "integrity": "sha512-gwikF65aDNeeXa8JxXa2BAk+REjSyhrNC9ZwdT0f8jc4dQQeDQ7G4m0f2QCLPJiMTTO6wfDmRmj/pW0PsUvIcA==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-buffer/-/helper-buffer-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-z3nFzdcp1mb8nEOFFk8DrYLpHvhKC3grJD2ardfKOzmbmJvEf/tPIqCY+sNcwZIY8ZD7IkB2l7/pqhUhqm7hLA==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-buffer/-/helper-buffer-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "@webassemblyjs/helper-numbers": {
             "dev": true,
-            "integrity": "sha512-vDkbxiB8zfnPdNK9Rajcey5C0w+QJugEglN0of+kmO8l7lDb77AnlKYQF7aarZuCrv+l0UvqL+68gSDr3k9LPQ==",
+            "integrity": "sha512-vUIhZ8LZoIWHBohiEObxVm6hwP034jwmc9kuq5GdHZH0wiLVLIPcMCdpJzG4C11cHoQ25TFIQj9kaVADVX7N3g==",
             "requires": {
-                "@webassemblyjs/floating-point-hex-parser": "1.11.1",
-                "@webassemblyjs/helper-api-error": "1.11.1",
+                "@webassemblyjs/floating-point-hex-parser": "1.11.6",
+                "@webassemblyjs/helper-api-error": "1.11.6",
                 "@xtuc/long": "4.2.2"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-numbers/-/helper-numbers-1.11.1.tgz",
-            "version": "1.11.1"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-numbers/-/helper-numbers-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "@webassemblyjs/helper-wasm-bytecode": {
             "dev": true,
-            "integrity": "sha512-PvpoOGiJwXeTrSf/qfudJhwlvDQxFgelbMqtq52WWiXC6Xgg1IREdngmPN3bs4RoO83PnL/nFrxucXj1+BX62Q==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-wasm-bytecode/-/helper-wasm-bytecode-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-sFFHKwcmBprO9e7Icf0+gddyWYDViL8bpPjJJl0WHxCdETktXdmtWLGVzoHbqUcY4Be1LkNfwTmXOJUFZYSJdA==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-wasm-bytecode/-/helper-wasm-bytecode-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "@webassemblyjs/helper-wasm-section": {
             "dev": true,
-            "integrity": "sha512-10P9No29rYX1j7F3EVPX3JvGPQPae+AomuSTPiF9eBQeChHI6iqjMIwR9JmOJXwpnn/oVGDk7I5IlskuMwU/pg==",
+            "integrity": "sha512-LPpZbSOwTpEC2cgn4hTydySy1Ke+XEu+ETXuoyvuyezHO3Kjdu90KK95Sh9xTbmjrCsUwvWwCOQQNta37VrS9g==",
             "requires": {
-                "@webassemblyjs/ast": "1.11.1",
-                "@webassemblyjs/helper-buffer": "1.11.1",
-                "@webassemblyjs/helper-wasm-bytecode": "1.11.1",
-                "@webassemblyjs/wasm-gen": "1.11.1"
+                "@webassemblyjs/ast": "1.11.6",
+                "@webassemblyjs/helper-buffer": "1.11.6",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.6",
+                "@webassemblyjs/wasm-gen": "1.11.6"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-wasm-section/-/helper-wasm-section-1.11.1.tgz",
-            "version": "1.11.1"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-wasm-section/-/helper-wasm-section-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "@webassemblyjs/ieee754": {
             "dev": true,
-            "integrity": "sha512-hJ87QIPtAMKbFq6CGTkZYJivEwZDbQUgYd3qKSadTNOhVY7p+gfP6Sr0lLRVTaG1JjFj+r3YchoqRYxNH3M0GQ==",
+            "integrity": "sha512-LM4p2csPNvbij6U1f19v6WR56QZ8JcHg3QIJTlSwzFcmx6WSORicYj6I63f9yU1kEUtrpG+kjkiIAkevHpDXrg==",
             "requires": {
                 "@xtuc/ieee754": "^1.2.0"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/ieee754/-/ieee754-1.11.1.tgz",
-            "version": "1.11.1"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/ieee754/-/ieee754-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "@webassemblyjs/leb128": {
             "dev": true,
-            "integrity": "sha512-BJ2P0hNZ0u+Th1YZXJpzW6miwqQUGcIHT1G/sf72gLVD9DZ5AdYTqPNbHZh6K1M5VmKvFXwGSWZADz+qBWxeRw==",
+            "integrity": "sha512-m7a0FhE67DQXgouf1tbN5XQcdWoNgaAuoULHIfGFIEVKA6tu/edls6XnIlkmS6FrXAquJRPni3ZZKjw6FSPjPQ==",
             "requires": {
                 "@xtuc/long": "4.2.2"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/leb128/-/leb128-1.11.1.tgz",
-            "version": "1.11.1"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/leb128/-/leb128-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "@webassemblyjs/utf8": {
             "dev": true,
-            "integrity": "sha512-9kqcxAEdMhiwQkHpkNiorZzqpGrodQQ2IGrHHxCy+Ozng0ofyMA0lTqiLkVs1uzTRejX+/O0EOT7KxqVPuXosQ==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/utf8/-/utf8-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-vtXf2wTQ3+up9Zsg8sa2yWiQpzSsMyXj0qViVP6xKGCUT8p8YJ6HqI7l5eCnWx1T/FYdsv07HQs2wTFbbof/RA==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/utf8/-/utf8-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "@webassemblyjs/wasm-edit": {
             "dev": true,
-            "integrity": "sha512-g+RsupUC1aTHfR8CDgnsVRVZFJqdkFHpsHMfJuWQzWU3tvnLC07UqHICfP+4XyL2tnr1amvl1Sdp06TnYCmVkA==",
+            "integrity": "sha512-Ybn2I6fnfIGuCR+Faaz7YcvtBKxvoLV3Lebn1tM4o/IAJzmi9AWYIPWpyBfU8cC+JxAO57bk4+zdsTjJR+VTOw==",
             "requires": {
-                "@webassemblyjs/ast": "1.11.1",
-                "@webassemblyjs/helper-buffer": "1.11.1",
-                "@webassemblyjs/helper-wasm-bytecode": "1.11.1",
-                "@webassemblyjs/helper-wasm-section": "1.11.1",
-                "@webassemblyjs/wasm-gen": "1.11.1",
-                "@webassemblyjs/wasm-opt": "1.11.1",
-                "@webassemblyjs/wasm-parser": "1.11.1",
-                "@webassemblyjs/wast-printer": "1.11.1"
+                "@webassemblyjs/ast": "1.11.6",
+                "@webassemblyjs/helper-buffer": "1.11.6",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.6",
+                "@webassemblyjs/helper-wasm-section": "1.11.6",
+                "@webassemblyjs/wasm-gen": "1.11.6",
+                "@webassemblyjs/wasm-opt": "1.11.6",
+                "@webassemblyjs/wasm-parser": "1.11.6",
+                "@webassemblyjs/wast-printer": "1.11.6"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-edit/-/wasm-edit-1.11.1.tgz",
-            "version": "1.11.1"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-edit/-/wasm-edit-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "@webassemblyjs/wasm-gen": {
             "dev": true,
-            "integrity": "sha512-F7QqKXwwNlMmsulj6+O7r4mmtAlCWfO/0HdgOxSklZfQcDu0TpLiD1mRt/zF25Bk59FIjEuGAIyn5ei4yMfLhA==",
+            "integrity": "sha512-3XOqkZP/y6B4F0PBAXvI1/bky7GryoogUtfwExeP/v7Nzwo1QLcq5oQmpKlftZLbT+ERUOAZVQjuNVak6UXjPA==",
             "requires": {
-                "@webassemblyjs/ast": "1.11.1",
-                "@webassemblyjs/helper-wasm-bytecode": "1.11.1",
-                "@webassemblyjs/ieee754": "1.11.1",
-                "@webassemblyjs/leb128": "1.11.1",
-                "@webassemblyjs/utf8": "1.11.1"
+                "@webassemblyjs/ast": "1.11.6",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.6",
+                "@webassemblyjs/ieee754": "1.11.6",
+                "@webassemblyjs/leb128": "1.11.6",
+                "@webassemblyjs/utf8": "1.11.6"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-gen/-/wasm-gen-1.11.1.tgz",
-            "version": "1.11.1"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-gen/-/wasm-gen-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "@webassemblyjs/wasm-opt": {
             "dev": true,
-            "integrity": "sha512-VqnkNqnZlU5EB64pp1l7hdm3hmQw7Vgqa0KF/KCNO9sIpI6Fk6brDEiX+iCOYrvMuBWDws0NkTOxYEb85XQHHw==",
+            "integrity": "sha512-cOrKuLRE7PCe6AsOVl7WasYf3wbSo4CeOk6PkrjS7g57MFfVUF9u6ysQBBODX0LdgSvQqRiGz3CXvIDKcPNy4g==",
             "requires": {
-                "@webassemblyjs/ast": "1.11.1",
-                "@webassemblyjs/helper-buffer": "1.11.1",
-                "@webassemblyjs/wasm-gen": "1.11.1",
-                "@webassemblyjs/wasm-parser": "1.11.1"
+                "@webassemblyjs/ast": "1.11.6",
+                "@webassemblyjs/helper-buffer": "1.11.6",
+                "@webassemblyjs/wasm-gen": "1.11.6",
+                "@webassemblyjs/wasm-parser": "1.11.6"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-opt/-/wasm-opt-1.11.1.tgz",
-            "version": "1.11.1"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-opt/-/wasm-opt-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "@webassemblyjs/wasm-parser": {
             "dev": true,
-            "integrity": "sha512-rrBujw+dJu32gYB7/Lup6UhdkPx9S9SnobZzRVL7VcBH9Bt9bCBLEuX/YXOOtBsOZ4NQrRykKhffRWHvigQvOA==",
+            "integrity": "sha512-6ZwPeGzMJM3Dqp3hCsLgESxBGtT/OeCvCZ4TA1JUPYgmhAx38tTPR9JaKy0S5H3evQpO/h2uWs2j6Yc/fjkpTQ==",
             "requires": {
-                "@webassemblyjs/ast": "1.11.1",
-                "@webassemblyjs/helper-api-error": "1.11.1",
-                "@webassemblyjs/helper-wasm-bytecode": "1.11.1",
-                "@webassemblyjs/ieee754": "1.11.1",
-                "@webassemblyjs/leb128": "1.11.1",
-                "@webassemblyjs/utf8": "1.11.1"
+                "@webassemblyjs/ast": "1.11.6",
+                "@webassemblyjs/helper-api-error": "1.11.6",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.6",
+                "@webassemblyjs/ieee754": "1.11.6",
+                "@webassemblyjs/leb128": "1.11.6",
+                "@webassemblyjs/utf8": "1.11.6"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-parser/-/wasm-parser-1.11.1.tgz",
-            "version": "1.11.1"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-parser/-/wasm-parser-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "@webassemblyjs/wast-printer": {
             "dev": true,
-            "integrity": "sha512-IQboUWM4eKzWW+N/jij2sRatKMh99QEelo3Eb2q0qXkvPRISAj8Qxtmw5itwqK+TTkBuUIE45AxYPToqPtL5gg==",
+            "integrity": "sha512-JM7AhRcE+yW2GWYaKeHL5vt4xqee5N2WcezptmgyhNS+ScggqcT1OtXykhAb13Sn5Yas0j2uv9tHgrjwvzAP4A==",
             "requires": {
-                "@webassemblyjs/ast": "1.11.1",
+                "@webassemblyjs/ast": "1.11.6",
                 "@xtuc/long": "4.2.2"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wast-printer/-/wast-printer-1.11.1.tgz",
-            "version": "1.11.1"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wast-printer/-/wast-printer-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "@xtuc/ieee754": {
             "dev": true,
             "integrity": "sha512-DX8nKgqcGwsc0eJSqYt5lwP4DH5FlHnmuWWBRy7X0NcaGR0ZtuyeESgMwTYVEtxmsNGY+qit4QYT/MIYTOTPeA==",
             "resolved": "https://registry.npmjs.org/@xtuc/ieee754/-/ieee754-1.2.0.tgz",
             "version": "1.2.0"
         },
@@ -275,26 +278,26 @@
             "resolved": "https://registry.npmjs.org/@xtuc/long/-/long-4.2.2.tgz",
             "version": "4.2.2"
         },
         "accepts": {
             "dependencies": {
                 "mime-db": {
                     "dev": true,
-                    "integrity": "sha512-5y8A56jg7XVQx2mbv1lu49NR4dokRnhZYTtL+KGfaa27uq4pSTXkwQkFJl4pkRMyNFz/EtYDSkiiEHx3F7UN6g==",
-                    "resolved": "https://registry.npmjs.org/mime-db/-/mime-db-1.51.0.tgz",
-                    "version": "1.51.0"
+                    "integrity": "sha512-sPU4uV7dYlvtWJxwwxHD0PuihVNiE7TyAbQ5SWxDCB9mUYvOgroQOwYQQOKPJ8CIbE+1ETVlOoK1UC2nU3gYvg==",
+                    "resolved": "https://registry.npmjs.org/mime-db/-/mime-db-1.52.0.tgz",
+                    "version": "1.52.0"
                 },
                 "mime-types": {
                     "dev": true,
-                    "integrity": "sha512-6cP692WwGIs9XXdOO4++N+7qjqv0rqxxVvJ3VHPh/Sc9mVZcQP+ZGhkKiTvWMQRr2tbHkJP/Yn7Y0npb3ZBs4A==",
+                    "integrity": "sha512-ZDY+bPm5zTTF+YpCrAU9nK0UgICYPT0QtT1NZWFv4s++TNkcgVaT0g6+4R2uI4MjQjzysHB1zxuWL50hzaeXiw==",
                     "requires": {
-                        "mime-db": "1.51.0"
+                        "mime-db": "1.52.0"
                     },
-                    "resolved": "https://registry.npmjs.org/mime-types/-/mime-types-2.1.34.tgz",
-                    "version": "2.1.34"
+                    "resolved": "https://registry.npmjs.org/mime-types/-/mime-types-2.1.35.tgz",
+                    "version": "2.1.35"
                 }
             },
             "dev": true,
             "integrity": "sha512-PYAthTa2m2VKxuvSD3DPC/Gy+U+sOA1LAuT8mkmRuvw+NACSaeXEQ+NHcVF7rONl6qcaxV3Uuemwawk+7+SJLw==",
             "requires": {
                 "mime-types": "~2.1.34",
                 "negotiator": "0.6.3"
@@ -306,17 +309,17 @@
             "dev": true,
             "integrity": "sha512-xjIYgE8HBrkpd/sJqOGNspf8uHG+NOHGOw6a/Urj8taM2EXfdNAH2oFcPeIFfsv3+kz/mJrS5VuMqbNLjCa2vw==",
             "resolved": "https://registry.npmjs.org/acorn/-/acorn-8.8.2.tgz",
             "version": "8.8.2"
         },
         "acorn-import-assertions": {
             "dev": true,
-            "integrity": "sha512-m7VZ3jwz4eK6A4Vtt8Ew1/mNbP24u0FhdyfA7fSvnJR6LMdfOYnmuIrrJAgrYfYJ10F/otaHTtrtrtmHdMNzEw==",
-            "resolved": "https://registry.npmjs.org/acorn-import-assertions/-/acorn-import-assertions-1.8.0.tgz",
-            "version": "1.8.0"
+            "integrity": "sha512-cmMwop9x+8KFhxvKrKfPYmN6/pKTYYHBqLa0DfvVZcKMJWNyWLnaqND7dx/qn66R7ewM1UX5XMaDVP5wlVTaVA==",
+            "resolved": "https://registry.npmjs.org/acorn-import-assertions/-/acorn-import-assertions-1.9.0.tgz",
+            "version": "1.9.0"
         },
         "ajv": {
             "dev": true,
             "integrity": "sha512-j3fVLgvTo527anyYyJOGTYJbG+vnnQYvE0m5mmkc1TK+nxAppkCLMIL0aZ4dblVCNoGShhm+kzE4ZUykBoMg4g==",
             "requires": {
                 "fast-deep-equal": "^3.1.1",
                 "fast-json-stable-stringify": "^2.0.0",
@@ -459,29 +462,31 @@
             "dev": true,
             "integrity": "sha512-D7iWRBvnZE8ecXiLj/9wbxH7Tk79fAh8IHaTNq1RWRixsS02W+5qS+iE9yq6RYl0asXx5tw0bLhmT5pIfbSquw==",
             "resolved": "https://registry.npmjs.org/bn.js/-/bn.js-5.2.0.tgz",
             "version": "5.2.0"
         },
         "body-parser": {
             "dev": true,
-            "integrity": "sha512-SAAwOxgoCKMGs9uUAUFHygfLAyaniaoun6I8mFY9pRAJL9+Kec34aU+oIjDhTycub1jozEfEwx1W1IuOYxVSFw==",
+            "integrity": "sha512-ml9pReCu3M61kGlqoTm2umSXTlRTuGTx0bfYj+uIUKKYycG5NtSbeetV3faSU6R7ajOPw0g/J1PvK4qNy7s5bA==",
             "requires": {
                 "bytes": "3.1.2",
-                "content-type": "~1.0.4",
+                "content-type": "~1.0.5",
                 "debug": "2.6.9",
-                "depd": "~1.1.2",
-                "http-errors": "1.8.1",
+                "depd": "2.0.0",
+                "destroy": "1.2.0",
+                "http-errors": "2.0.0",
                 "iconv-lite": "0.4.24",
-                "on-finished": "~2.3.0",
-                "qs": "6.9.7",
-                "raw-body": "2.4.3",
-                "type-is": "~1.6.18"
+                "on-finished": "2.4.1",
+                "qs": "6.11.0",
+                "raw-body": "2.5.2",
+                "type-is": "~1.6.18",
+                "unpipe": "1.0.0"
             },
-            "resolved": "https://registry.npmjs.org/body-parser/-/body-parser-1.19.2.tgz",
-            "version": "1.19.2"
+            "resolved": "https://registry.npmjs.org/body-parser/-/body-parser-1.20.2.tgz",
+            "version": "1.20.2"
         },
         "brace-expansion": {
             "dev": true,
             "integrity": "sha512-iCuPHDFgrHX7H2vEI/5xpz07zSHB00TpugqhmYtVmMO6518mCuRMoOYFldEBl0g187ufozdaHgWKcYFb61qGiA==",
             "requires": {
                 "balanced-match": "^1.0.0",
                 "concat-map": "0.0.1"
@@ -586,23 +591,23 @@
                 "safe-buffer": "^5.2.0"
             },
             "resolved": "https://registry.npmjs.org/browserify-sign/-/browserify-sign-4.2.1.tgz",
             "version": "4.2.1"
         },
         "browserslist": {
             "dev": true,
-            "integrity": "sha512-tUkiguQGW7S3IhB7N+c2MV/HZPSCPAAiYBZXLsBhFB/PCy6ZKKsZrmBayHV9fdGV/ARIfJ14NkxKzRDjvp7L6w==",
+            "integrity": "sha512-BauCXrQ7I2ftSqd2mvKHGo85XR0u7Ru3C/Hxsy/0TkfCtjrmAbPdzLGasmoiBxplpDXlPvdjX9u7srIMfgasNA==",
             "requires": {
-                "caniuse-lite": "^1.0.30001449",
-                "electron-to-chromium": "^1.4.284",
-                "node-releases": "^2.0.8",
-                "update-browserslist-db": "^1.0.10"
+                "caniuse-lite": "^1.0.30001489",
+                "electron-to-chromium": "^1.4.411",
+                "node-releases": "^2.0.12",
+                "update-browserslist-db": "^1.0.11"
             },
-            "resolved": "https://registry.npmjs.org/browserslist/-/browserslist-4.21.5.tgz",
-            "version": "4.21.5"
+            "resolved": "https://registry.npmjs.org/browserslist/-/browserslist-4.21.7.tgz",
+            "version": "4.21.7"
         },
         "buffer": {
             "dev": true,
             "integrity": "sha512-FTiCpNxtwiZZHEZbcbTIcZjERVICn9yq/pDFkTl95/AxzD1naBctN7YO68riM/gLSDY7sdrMby8hofADYuuqOA==",
             "requires": {
                 "base64-js": "^1.3.1",
                 "ieee754": "^1.2.1"
@@ -642,17 +647,17 @@
             "dev": true,
             "integrity": "sha512-Gmy6FhYlCY7uOElZUSbxo2UCDH8owEk996gkbrpsgGtrJLM3J7jGxl9Ic7Qwwj4ivOE5AWZWRMecDdF7hqGjFA==",
             "resolved": "https://registry.npmjs.org/camelcase/-/camelcase-6.3.0.tgz",
             "version": "6.3.0"
         },
         "caniuse-lite": {
             "dev": true,
-            "integrity": "sha512-KCqHwRnaa1InZBtqXzP98LPg0ajCVujMKjqKDhZEthIpAsJl/YEIa3YvXjGXPVqzZVguccuu7ga9KOE1J9rKPQ==",
-            "resolved": "https://registry.npmjs.org/caniuse-lite/-/caniuse-lite-1.0.30001481.tgz",
-            "version": "1.0.30001481"
+            "integrity": "sha512-F6x5IEuigtUfU5ZMQK2jsy5JqUUlEFRVZq8bO2a+ysq5K7jD6PPc9YXZj78xDNS3uNchesp1Jw47YXEqr+Viyg==",
+            "resolved": "https://registry.npmjs.org/caniuse-lite/-/caniuse-lite-1.0.30001495.tgz",
+            "version": "1.0.30001495"
         },
         "chalk": {
             "dependencies": {
                 "supports-color": {
                     "dev": true,
                     "integrity": "sha512-QjVjwdXIt408MIiAqCX4oUKsgU2EqAGzs2Ppkm4aQYbjm+ZEWEcW4SfFNTr4uMNZma0ey4f5lgLrkB0aX0QMow==",
                     "requires": {
@@ -766,20 +771,14 @@
         },
         "color-name": {
             "dev": true,
             "integrity": "sha1-p9BVi9icQveV3UIyj3QIMcpTvCU=",
             "resolved": "https://registry.npmjs.org/color-name/-/color-name-1.1.3.tgz",
             "version": "1.1.3"
         },
-        "colors": {
-            "dev": true,
-            "integrity": "sha512-a+UqTh4kgZg/SlGvfbzDHpgRu7AAQOmmqRHJnxhRZICKFUT91brVhNNt58CMWU9PsBbv3PDCZUHbVxuDiH2mtA==",
-            "resolved": "https://registry.npmjs.org/colors/-/colors-1.4.0.tgz",
-            "version": "1.4.0"
-        },
         "commander": {
             "dev": true,
             "integrity": "sha512-GpVkmM8vF2vQUkj2LvZmD35JxeJOLCwJ9cUkugyk2nuhbv3+mJvpLYYt+0+USMxE+oj+ey/lJEnhZw75x/OMcQ==",
             "resolved": "https://registry.npmjs.org/commander/-/commander-2.20.3.tgz",
             "version": "2.20.3"
         },
         "concat-map": {
@@ -798,17 +797,17 @@
                 "utils-merge": "1.0.1"
             },
             "resolved": "https://registry.npmjs.org/connect/-/connect-3.7.0.tgz",
             "version": "3.7.0"
         },
         "content-type": {
             "dev": true,
-            "integrity": "sha512-hIP3EEPs8tB9AT1L+NUqtwOAps4mk2Zob89MWXMHjHWg9milF/j4osnnQLXBCBFBk/tvIG/tUc9mOUJiPBhPXA==",
-            "resolved": "https://registry.npmjs.org/content-type/-/content-type-1.0.4.tgz",
-            "version": "1.0.4"
+            "integrity": "sha512-nTjqfcBFEipKdXCv4YDQWCfmcLZKm81ldF0pAopTvyrFGVbcR6P/VAAd5G7N+0tTr8QqiU0tFadD6FK4NtJwOA==",
+            "resolved": "https://registry.npmjs.org/content-type/-/content-type-1.0.5.tgz",
+            "version": "1.0.5"
         },
         "cookie": {
             "dev": true,
             "integrity": "sha512-aSWTXFzaKWkvHO1Ny/s+ePFpvKsPnjc551iI41v3ny/ow6tBG5Vd+FuqGNhh1LxOmVzOlGUriIlOaokOvhaStA==",
             "resolved": "https://registry.npmjs.org/cookie/-/cookie-0.4.2.tgz",
             "version": "0.4.2"
         },
@@ -890,23 +889,23 @@
                 "randomfill": "^1.0.3"
             },
             "resolved": "https://registry.npmjs.org/crypto-browserify/-/crypto-browserify-3.12.0.tgz",
             "version": "3.12.0"
         },
         "custom-event": {
             "dev": true,
-            "integrity": "sha1-XQKkaFCt8bSjF5RqOSj8y1v9BCU=",
+            "integrity": "sha512-GAj5FOq0Hd+RsCGVJxZuKaIDXDf3h6GQoNEjFgbLLI/trgtavwUbSnZ5pVfg27DVCaWjIohryS0JFwIJyT2cMg==",
             "resolved": "https://registry.npmjs.org/custom-event/-/custom-event-1.0.1.tgz",
             "version": "1.0.1"
         },
         "date-format": {
             "dev": true,
-            "integrity": "sha512-7P3FyqDcfeznLZp2b+OMitV9Sz2lUnsT87WaTat9nVwqsBkTzPG3lPLNwW3en6F4pHUiWzr6vb8CLhjdK9bcxQ==",
-            "resolved": "https://registry.npmjs.org/date-format/-/date-format-4.0.3.tgz",
-            "version": "4.0.3"
+            "integrity": "sha512-39BOQLs9ZjKh0/patS9nrT8wc3ioX3/eA/zgbKNopnF2wCqJEoxywwwElATYvRsXdnOxA/OQeQoFZ3rFjVajhg==",
+            "resolved": "https://registry.npmjs.org/date-format/-/date-format-4.0.14.tgz",
+            "version": "4.0.14"
         },
         "debug": {
             "dev": true,
             "integrity": "sha512-bC7ElrdJaJnPbAP+1EotYvqZsb3ecl5wi6Bfi6BJTUcNowp6cvspg0jXznRTKDjm/E7AdgFBVeAPVMNcKGsHMA==",
             "requires": {
                 "ms": "2.0.0"
             },
@@ -926,31 +925,37 @@
                 "object-keys": "^1.0.12"
             },
             "resolved": "https://registry.npmjs.org/define-properties/-/define-properties-1.1.3.tgz",
             "version": "1.1.3"
         },
         "depd": {
             "dev": true,
-            "integrity": "sha1-m81S4UwJd2PnSbJ0xDRu0uVgtak=",
-            "resolved": "https://registry.npmjs.org/depd/-/depd-1.1.2.tgz",
-            "version": "1.1.2"
+            "integrity": "sha512-g7nH6P6dyDioJogAAGprGpCtVImJhpPk/roCzdb3fIh61/s/nPsfR6onyMwkCAR/OlC3yBC0lESvUoQEAssIrw==",
+            "resolved": "https://registry.npmjs.org/depd/-/depd-2.0.0.tgz",
+            "version": "2.0.0"
         },
         "des.js": {
             "dev": true,
             "integrity": "sha512-Q0I4pfFrv2VPd34/vfLrFOoRmlYj3OV50i7fskps1jZWK1kApMWWT9G6RRUeYedLcBDIhnSDaUvJMb3AhUlaEA==",
             "requires": {
                 "inherits": "^2.0.1",
                 "minimalistic-assert": "^1.0.0"
             },
             "resolved": "https://registry.npmjs.org/des.js/-/des.js-1.0.1.tgz",
             "version": "1.0.1"
         },
+        "destroy": {
+            "dev": true,
+            "integrity": "sha512-2sJGJTaXIIaR1w4iJSNoN0hnMY7Gpc/n8D4qSCJw8QqFWXf7cuAgnEHxBpweaVcPevC2l3KpjYCx3NypQQgaJg==",
+            "resolved": "https://registry.npmjs.org/destroy/-/destroy-1.2.0.tgz",
+            "version": "1.2.0"
+        },
         "di": {
             "dev": true,
-            "integrity": "sha1-gGZJMmzqp8qjMG112YXqJ0i6kTw=",
+            "integrity": "sha512-uJaamHkagcZtHPqCIHZxnFrXlunQXgBOsZSUOWwFw31QJCAbyTBoHMW75YOTur5ZNx8pIeAKgf6GWIgaqqiLhA==",
             "resolved": "https://registry.npmjs.org/di/-/di-0.0.1.tgz",
             "version": "0.0.1"
         },
         "diff": {
             "dev": true,
             "integrity": "sha512-/VTCrvm5Z0JGty/BWHljh+BAiw3IK+2j87NGMu8Nwc/f48WoDAC395uomO9ZD117ZOBaHmkX1oyLvkVM/aIT3w==",
             "resolved": "https://registry.npmjs.org/diff/-/diff-5.0.0.tgz",
@@ -973,35 +978,35 @@
                 "randombytes": "^2.0.0"
             },
             "resolved": "https://registry.npmjs.org/diffie-hellman/-/diffie-hellman-5.0.3.tgz",
             "version": "5.0.3"
         },
         "dom-serialize": {
             "dev": true,
-            "integrity": "sha1-ViromZ9Evl6jB29UGdzVnrQ6yVs=",
+            "integrity": "sha512-Yra4DbvoW7/Z6LBN560ZwXMjoNOSAN2wRsKFGc4iBeso+mpIA6qj1vfdf9HpMaKAqG6wXTy+1SYEzmNpKXOSsQ==",
             "requires": {
                 "custom-event": "~1.0.0",
                 "ent": "~2.2.0",
                 "extend": "^3.0.0",
                 "void-elements": "^2.0.0"
             },
             "resolved": "https://registry.npmjs.org/dom-serialize/-/dom-serialize-2.2.1.tgz",
             "version": "2.2.1"
         },
         "ee-first": {
             "dev": true,
-            "integrity": "sha1-WQxhFWsK4vTwJVcyoViyZrxWsh0=",
+            "integrity": "sha512-WMwm9LhRUo+WUaRN+vRuETqG89IgZphVSNkdFgeb6sS/E4OrDIN7t48CAewSHXc6C8lefD8KKfr5vY61brQlow==",
             "resolved": "https://registry.npmjs.org/ee-first/-/ee-first-1.1.1.tgz",
             "version": "1.1.1"
         },
         "electron-to-chromium": {
             "dev": true,
-            "integrity": "sha512-LfxbHXdA/S+qyoTEA4EbhxGjrxx7WK2h6yb5K2v0UCOufUKX+VZaHbl3svlzZfv9sGseym/g3Ne4DpsgRULmqg==",
-            "resolved": "https://registry.npmjs.org/electron-to-chromium/-/electron-to-chromium-1.4.369.tgz",
-            "version": "1.4.369"
+            "integrity": "sha512-wZOyn3s/aQOtLGAwXMZfteQPN68kgls2wDAnYOA8kCjBvKVrW5RwmWVspxJYTqrcN7Y263XJVsC66VCIGzDO3g==",
+            "resolved": "https://registry.npmjs.org/electron-to-chromium/-/electron-to-chromium-1.4.421.tgz",
+            "version": "1.4.421"
         },
         "elliptic": {
             "dependencies": {
                 "bn.js": {
                     "dev": true,
                     "integrity": "sha512-c98Bf3tPniI+scsdk237ku1Dc3ujXQTSgyiPUDEOe7tRkhrqridvh8klBv0HCEso1OLOYcHuCv/cS6DNxKH+ZA==",
                     "resolved": "https://registry.npmjs.org/bn.js/-/bn.js-4.12.0.tgz",
@@ -1032,15 +1037,15 @@
             "dev": true,
             "integrity": "sha512-MSjYzcWNOA0ewAHpz0MxpYFvwg6yjy1NG3xteoqz644VCo/RPgnr1/GGt+ic3iJTzQ8Eu3TdM14SawnVUmGE6A==",
             "resolved": "https://registry.npmjs.org/emoji-regex/-/emoji-regex-8.0.0.tgz",
             "version": "8.0.0"
         },
         "encodeurl": {
             "dev": true,
-            "integrity": "sha1-rT/0yG7C0CkyL1oCw6mmBslbP1k=",
+            "integrity": "sha512-TPJXq8JqFaVYm2CWmPvnP2Iyo4ZSM7/QKcSmuMLDObfpH5fi7RUGmd/rTDf+rut/saiDiQEeVTNgAmJEdAOx0w==",
             "resolved": "https://registry.npmjs.org/encodeurl/-/encodeurl-1.0.2.tgz",
             "version": "1.0.2"
         },
         "engine.io": {
             "dependencies": {
                 "debug": {
                     "dev": true,
@@ -1073,34 +1078,31 @@
                 "ws": "~8.11.0"
             },
             "resolved": "https://registry.npmjs.org/engine.io/-/engine.io-6.4.2.tgz",
             "version": "6.4.2"
         },
         "engine.io-parser": {
             "dev": true,
-            "integrity": "sha512-BtQxwF27XUNnSafQLvDi0dQ8s3i6VgzSoQMJacpIcGNrlUdfHSKbgm3jmjCVvQluGzqwujQMPAoMai3oYSTurg==",
-            "requires": {
-                "@socket.io/base64-arraybuffer": "~1.0.2"
-            },
-            "resolved": "https://registry.npmjs.org/engine.io-parser/-/engine.io-parser-5.0.3.tgz",
-            "version": "5.0.3"
+            "integrity": "sha512-P+jDFbvK6lE3n1OL+q9KuzdOFWkkZ/cMV9gol/SbVfpyqfvrfrFTOFJ6fQm2VC3PZHlU3QPhVwmbsCnauHF2MQ==",
+            "resolved": "https://registry.npmjs.org/engine.io-parser/-/engine.io-parser-5.0.7.tgz",
+            "version": "5.0.7"
         },
         "enhanced-resolve": {
             "dev": true,
-            "integrity": "sha512-eyV8f0y1+bzyfh8xAwW/WTSZpLbjhqc4ne9eGSH4Zo2ejdyiNG9pU6mf9DG8a7+Auk6MFTlNOT4Y2y/9k8GKVg==",
+            "integrity": "sha512-Vklwq2vDKtl0y/vtwjSesgJ5MYS7Etuk5txS8VdKL4AOS1aUlD96zqIfsOSLQsdv3xgMRbtkWM8eG9XDfKUPow==",
             "requires": {
                 "graceful-fs": "^4.2.4",
                 "tapable": "^2.2.0"
             },
-            "resolved": "https://registry.npmjs.org/enhanced-resolve/-/enhanced-resolve-5.13.0.tgz",
-            "version": "5.13.0"
+            "resolved": "https://registry.npmjs.org/enhanced-resolve/-/enhanced-resolve-5.14.1.tgz",
+            "version": "5.14.1"
         },
         "ent": {
             "dev": true,
-            "integrity": "sha1-6WQhkyWiHQX0RGai9obtbOX13R0=",
+            "integrity": "sha512-GHrMyVZQWvTIdDtpiEXdHZnFQKzeO09apj8Cbl4pKWy4i0Oprcq17usfDt5aO63swf0JOeMWjWQE/LzgSRuWpA==",
             "resolved": "https://registry.npmjs.org/ent/-/ent-2.2.0.tgz",
             "version": "2.2.0"
         },
         "es-abstract": {
             "dependencies": {
                 "has-symbols": {
                     "dev": true,
@@ -1148,17 +1150,17 @@
                 "unbox-primitive": "^1.0.1"
             },
             "resolved": "https://registry.npmjs.org/es-abstract/-/es-abstract-1.18.3.tgz",
             "version": "1.18.3"
         },
         "es-module-lexer": {
             "dev": true,
-            "integrity": "sha512-1HQ2M2sPtxwnvOvT1ZClHyQDiggdNjURWpY2we6aMKCQiUVxTmVs2UYPLIrD84sS+kMdUwfBSylbJPwNnBrnHQ==",
-            "resolved": "https://registry.npmjs.org/es-module-lexer/-/es-module-lexer-0.9.3.tgz",
-            "version": "0.9.3"
+            "integrity": "sha512-9978wrXM50Y4rTMmW5kXIC09ZdXQZqkE4mxhwkd8VbzsGkXGPgV4zWuqQJgCEzYngdo2dYDa0l8xhX4fkSwJSg==",
+            "resolved": "https://registry.npmjs.org/es-module-lexer/-/es-module-lexer-1.2.1.tgz",
+            "version": "1.2.1"
         },
         "es-to-primitive": {
             "dev": true,
             "integrity": "sha512-QCOllgZJtaUo9miYBcLChTUaHNjJF3PYs1VidD7AwiEj1kYxKeQTctLAezAOH5ZKRH0g2IgPn6KwB4IT8iRpvA==",
             "requires": {
                 "is-callable": "^1.1.4",
                 "is-date-object": "^1.0.1",
@@ -1177,15 +1179,15 @@
             "dev": true,
             "integrity": "sha512-k0er2gUkLf8O0zKJiAhmkTnJlTvINGv7ygDNPbeIsX/TJjGJZHuh9B2UxbsaEkmlEo9MfhrSzmhIlhRlI2GXnw==",
             "resolved": "https://registry.npmjs.org/escalade/-/escalade-3.1.1.tgz",
             "version": "3.1.1"
         },
         "escape-html": {
             "dev": true,
-            "integrity": "sha1-Aljq5NPQwJdN4cFpGI7wBR0dGYg=",
+            "integrity": "sha512-NiSupZ4OeuGwr68lGIeym/ksIZMJodUGOSCZ/FSnTxcrekbvqrgdUxlJOMpijaKZVjAJrWrGs/6Jy8OMuyj9ow==",
             "resolved": "https://registry.npmjs.org/escape-html/-/escape-html-1.0.3.tgz",
             "version": "1.0.3"
         },
         "escape-string-regexp": {
             "dev": true,
             "integrity": "sha1-G2HAViGQqN/2rjuyzwIAyhMLhtQ=",
             "resolved": "https://registry.npmjs.org/escape-string-regexp/-/escape-string-regexp-1.0.5.tgz",
@@ -1270,14 +1272,31 @@
             "requires": {
                 "to-regex-range": "^5.0.1"
             },
             "resolved": "https://registry.npmjs.org/fill-range/-/fill-range-7.0.1.tgz",
             "version": "7.0.1"
         },
         "finalhandler": {
+            "dependencies": {
+                "on-finished": {
+                    "dev": true,
+                    "integrity": "sha512-ikqdkGAAyf/X/gPhXGvfgAytDZtDbr+bkNUJ0N9h5MI/dmdgCs3l6hoHrcUv41sRKew3jIwrp4qQDXiK99Utww==",
+                    "requires": {
+                        "ee-first": "1.1.1"
+                    },
+                    "resolved": "https://registry.npmjs.org/on-finished/-/on-finished-2.3.0.tgz",
+                    "version": "2.3.0"
+                },
+                "statuses": {
+                    "dev": true,
+                    "integrity": "sha512-OpZ3zP+jT1PI7I8nemJX4AKmAX070ZkYPVWV/AaKTJl+tXCTGyVdC1a4SL8RUQYEwk/f34ZX8UTykN68FwrqAA==",
+                    "resolved": "https://registry.npmjs.org/statuses/-/statuses-1.5.0.tgz",
+                    "version": "1.5.0"
+                }
+            },
             "dev": true,
             "integrity": "sha512-aAWcW57uxVNrQZqFXjITpW3sIUQmHGG3qSb9mUah9MgMC4NeWhNOlNjXEYq3HjRAvL6arUviZGGJsBg6z0zsWA==",
             "requires": {
                 "debug": "2.6.9",
                 "encodeurl": "~1.0.2",
                 "escape-html": "~1.0.3",
                 "on-finished": "~2.3.0",
@@ -1302,40 +1321,40 @@
             "dev": true,
             "integrity": "sha512-b6suED+5/3rTpUBdG1gupIl8MPFCAMA0QXwmljLhvCUKcUvdE4gWky9zpuGCcXHOsz4J9wPGNWq6OKpmIzz3hQ==",
             "resolved": "https://registry.npmjs.org/flat/-/flat-5.0.2.tgz",
             "version": "5.0.2"
         },
         "flatted": {
             "dev": true,
-            "integrity": "sha512-WIWGi2L3DyTUvUrwRKgGi9TwxQMUEqPOPQBVi71R96jZXJdFskXEmf54BoZaS1kknGODoIGASGEzBUYdyMCBJg==",
-            "resolved": "https://registry.npmjs.org/flatted/-/flatted-3.2.5.tgz",
-            "version": "3.2.5"
+            "integrity": "sha512-5nqDSxl8nn5BSNxyR3n4I6eDmbolI6WT+QqR547RwxQapgjQBmtktdP+HTBb/a/zLsbzERTONyUB5pefh5TtjQ==",
+            "resolved": "https://registry.npmjs.org/flatted/-/flatted-3.2.7.tgz",
+            "version": "3.2.7"
         },
         "follow-redirects": {
             "dev": true,
-            "integrity": "sha512-MQDfihBQYMcyy5dhRDJUHcw7lb2Pv/TuE6xP1vyraLukNDHKbDxDNaOE3NbCAdKQApno+GPRyo1YAp89yCjK4w==",
-            "resolved": "https://registry.npmjs.org/follow-redirects/-/follow-redirects-1.14.9.tgz",
-            "version": "1.14.9"
+            "integrity": "sha512-VQLG33o04KaQ8uYi2tVNbdrWp1QWxNNea+nmIB4EVM28v0hmP17z7aG1+wAkNzVq4KeXTq3221ye5qTJP91JwA==",
+            "resolved": "https://registry.npmjs.org/follow-redirects/-/follow-redirects-1.15.2.tgz",
+            "version": "1.15.2"
         },
         "foreach": {
             "dev": true,
             "integrity": "sha1-C+4AUBiusmDQo6865ljdATbsG5k=",
             "resolved": "https://registry.npmjs.org/foreach/-/foreach-2.0.5.tgz",
             "version": "2.0.5"
         },
         "fs-extra": {
             "dev": true,
-            "integrity": "sha512-NbdoVMZso2Lsrn/QwLXOy6rm0ufY2zEOKCDzJR/0kBsb0E6qed0P3iYK+Ath3BfvXEeu4JhEtXLgILx5psUfag==",
+            "integrity": "sha512-yhlQgA6mnOJUKOsRUFsgJdQCvkKhcz8tlZG5HBQfReYZy46OwLcY+Zia0mtdHsOo9y/hP+CxMN0TU9QxoOtG4g==",
             "requires": {
                 "graceful-fs": "^4.2.0",
-                "jsonfile": "^6.0.1",
-                "universalify": "^2.0.0"
+                "jsonfile": "^4.0.0",
+                "universalify": "^0.1.0"
             },
-            "resolved": "https://registry.npmjs.org/fs-extra/-/fs-extra-10.0.1.tgz",
-            "version": "10.0.1"
+            "resolved": "https://registry.npmjs.org/fs-extra/-/fs-extra-8.1.0.tgz",
+            "version": "8.1.0"
         },
         "fs.realpath": {
             "dev": true,
             "integrity": "sha1-FQStJSMVjKpA20onh8sBQRmU6k8=",
             "resolved": "https://registry.npmjs.org/fs.realpath/-/fs.realpath-1.0.0.tgz",
             "version": "1.0.0"
         },
@@ -1491,24 +1510,24 @@
                     "dev": true,
                     "integrity": "sha512-k/vGaX4/Yla3WzyMCvTQOXYeIHvqOKtnqBduzTHpzpQZzAskKMhZ2K+EnBiSM9zGSoIFeMpXKxa4dYeZIQqewQ==",
                     "resolved": "https://registry.npmjs.org/inherits/-/inherits-2.0.4.tgz",
                     "version": "2.0.4"
                 }
             },
             "dev": true,
-            "integrity": "sha512-Kpk9Sm7NmI+RHhnj6OIWDI1d6fIoFAtFt9RLaTMRlg/8w49juAStsrBgp0Dp4OdxdVbRIeKhtCUvoi/RuAhO4g==",
+            "integrity": "sha512-FtwrG/euBzaEjYeRqOgly7G0qviiXoJWnvEH2Z1plBdXgbyjv34pHTSb9zoeHMyDy33+DWy5Wt9Wo+TURtOYSQ==",
             "requires": {
-                "depd": "~1.1.2",
+                "depd": "2.0.0",
                 "inherits": "2.0.4",
                 "setprototypeof": "1.2.0",
-                "statuses": ">= 1.5.0 < 2",
+                "statuses": "2.0.1",
                 "toidentifier": "1.0.1"
             },
-            "resolved": "https://registry.npmjs.org/http-errors/-/http-errors-1.8.1.tgz",
-            "version": "1.8.1"
+            "resolved": "https://registry.npmjs.org/http-errors/-/http-errors-2.0.0.tgz",
+            "version": "2.0.0"
         },
         "http-proxy": {
             "dev": true,
             "integrity": "sha512-7mz/721AbnJwIVbnaSv1Cz3Am0ZLT/UBwkC92VlxhXv/k/BBQfM2fXElQNC27BVGr0uwUpplYPQM9LnaBMR5NQ==",
             "requires": {
                 "eventemitter3": "^4.0.0",
                 "follow-redirects": "^1.0.0",
@@ -1591,17 +1610,17 @@
             "dev": true,
             "integrity": "sha512-/b4ZVsG7Z5XVtIxs/h9W8nvfLgSAyKYdtGWQLbqy6jA1icmgjf8WCoTKgeS4wy5tYaPePouzFMANbnj94c2Z+A==",
             "resolved": "https://registry.npmjs.org/is-date-object/-/is-date-object-1.0.4.tgz",
             "version": "1.0.4"
         },
         "is-docker": {
             "dev": true,
-            "integrity": "sha512-pJEdRugimx4fBMra5z2/5iRdZ63OhYV0vr0Dwm5+xtW4D1FvRkB8hamMIhnWfyJeDdyr/aa7BDyNbtG38VxgoQ==",
-            "resolved": "https://registry.npmjs.org/is-docker/-/is-docker-2.0.0.tgz",
-            "version": "2.0.0"
+            "integrity": "sha512-F+i2BKsFrH66iaUFc0woD8sLy8getkwTwtOBjvs56Cx4CgJDeKQeqfz8wAYiSb8JOprWhHH5p77PbmYCvvUuXQ==",
+            "resolved": "https://registry.npmjs.org/is-docker/-/is-docker-2.2.1.tgz",
+            "version": "2.2.1"
         },
         "is-extglob": {
             "dev": true,
             "integrity": "sha1-qIwCU1eR8C7TfHahueqXc8gz+MI=",
             "resolved": "https://registry.npmjs.org/is-extglob/-/is-extglob-2.1.1.tgz",
             "version": "2.1.1"
         },
@@ -1729,17 +1748,23 @@
                 "is-docker": "^2.0.0"
             },
             "resolved": "https://registry.npmjs.org/is-wsl/-/is-wsl-2.2.0.tgz",
             "version": "2.2.0"
         },
         "isbinaryfile": {
             "dev": true,
-            "integrity": "sha512-53h6XFniq77YdW+spoRrebh0mnmTxRPTlcuIArO57lmMdq4uBKFKaeTjnb92oYWrSn/LVL+LT+Hap2tFQj8V+w==",
-            "resolved": "https://registry.npmjs.org/isbinaryfile/-/isbinaryfile-4.0.8.tgz",
-            "version": "4.0.8"
+            "integrity": "sha512-iHrqe5shvBUcFbmZq9zOQHBoeOhZJu6RQGrDpBgenUm/Am+F3JM2MgQj+rK3Z601fzrL5gLZWtAPH2OBaSVcyw==",
+            "resolved": "https://registry.npmjs.org/isbinaryfile/-/isbinaryfile-4.0.10.tgz",
+            "version": "4.0.10"
+        },
+        "isexe": {
+            "dev": true,
+            "integrity": "sha512-RHxMLp9lnKHGHRng9QFhRCMbYAcVpn69smSGcq3f36xjgVVWThj4qqLbTLlq7Ssj8B+fIQ1EuCEGI2lKsyQeIw==",
+            "resolved": "https://registry.npmjs.org/isexe/-/isexe-2.0.0.tgz",
+            "version": "2.0.0"
         },
         "jest-worker": {
             "dev": true,
             "integrity": "sha512-7vuh85V5cdDofPyxn58nrPjBktZo0u9x1g8WtjQol+jZDaE+fhN+cIvTj11GndBnMnyfrUOG1sZQxCdjKh+DKg==",
             "requires": {
                 "@types/node": "*",
                 "merge-stream": "^2.0.0",
@@ -1767,58 +1792,57 @@
             "dev": true,
             "integrity": "sha512-xbbCH5dCYU5T8LcEhhuh7HJ88HXuW3qsI3Y0zOZFKfZEHcpWiHU/Jxzk629Brsab/mMiHQti9wMP+845RPe3Vg==",
             "resolved": "https://registry.npmjs.org/json-schema-traverse/-/json-schema-traverse-0.4.1.tgz",
             "version": "0.4.1"
         },
         "jsonfile": {
             "dev": true,
-            "integrity": "sha512-5dgndWOriYSm5cnYaJNhalLNDKOqFwyDB/rr1E9ZsGciGvKPs8R2xYGCacuf3z6K1YKDz182fd+fY3cn3pMqXQ==",
+            "integrity": "sha512-m6F1R3z8jjlf2imQHS2Qez5sjKWQzbuuhuJ/FKYFRZvPE3PuHcSMVZzfsLhGVOkfd20obL5SWEBew5ShlquNxg==",
             "requires": {
-                "graceful-fs": "^4.1.6",
-                "universalify": "^2.0.0"
+                "graceful-fs": "^4.1.6"
             },
-            "resolved": "https://registry.npmjs.org/jsonfile/-/jsonfile-6.1.0.tgz",
-            "version": "6.1.0"
+            "resolved": "https://registry.npmjs.org/jsonfile/-/jsonfile-4.0.0.tgz",
+            "version": "4.0.0"
         },
         "karma": {
             "dependencies": {
                 "glob": {
                     "dev": true,
-                    "integrity": "sha512-lmLf6gtyrPq8tTjSmrO94wBeQbFR3HbLHbuyD69wuyQkImp2hWqMGB47OX65FBkPffO641IP9jWa1z4ivqG26Q==",
+                    "integrity": "sha512-nFR0zLpU2YCaRxwoCJvL6UvCH2JFyFVIvwTLsIf21AuHlMskA1hhTdk+LlYJtOlYt9v6dvszD2BGRqBL+iQK9Q==",
                     "requires": {
                         "fs.realpath": "^1.0.0",
                         "inflight": "^1.0.4",
                         "inherits": "2",
-                        "minimatch": "^3.0.4",
+                        "minimatch": "^3.1.1",
                         "once": "^1.3.0",
                         "path-is-absolute": "^1.0.0"
                     },
-                    "resolved": "https://registry.npmjs.org/glob/-/glob-7.2.0.tgz",
-                    "version": "7.2.0"
+                    "resolved": "https://registry.npmjs.org/glob/-/glob-7.2.3.tgz",
+                    "version": "7.2.3"
                 },
                 "graceful-fs": {
                     "dev": true,
-                    "integrity": "sha512-NtNxqUcXgpW2iMrfqSfR73Glt39K+BLwWsPs94yR63v45T0Wbej7eRmL5cWfwEgqXnmjQp3zaJTshdRW/qC2ZQ==",
-                    "resolved": "https://registry.npmjs.org/graceful-fs/-/graceful-fs-4.2.9.tgz",
-                    "version": "4.2.9"
+                    "integrity": "sha512-RbJ5/jmFcNNCcDV5o9eTnBLJ/HszWV0P73bc+Ff4nS/rJj+YaS6IGyiOL0VoBYX+l1Wrl3k63h/KrH+nhJ0XvQ==",
+                    "resolved": "https://registry.npmjs.org/graceful-fs/-/graceful-fs-4.2.11.tgz",
+                    "version": "4.2.11"
                 },
                 "mime": {
                     "dev": true,
                     "integrity": "sha512-USPkMeET31rOMiarsBNIHZKLGgvKc/LrjofAnBlOttf5ajRvqiRA8QsenbcooctK6d6Ts6aqZXBA+XbkKthiQg==",
                     "resolved": "https://registry.npmjs.org/mime/-/mime-2.6.0.tgz",
                     "version": "2.6.0"
                 }
             },
             "dev": true,
-            "integrity": "sha512-nEU50jLvDe5yvXqkEJRf8IuvddUkOY2x5Xc4WXHz6dxINgGDrgD2uqQWeVrJs4hbfNaotn+HQ1LZJ4yOXrL7xQ==",
+            "integrity": "sha512-C6SU/53LB31BEgRg+omznBEMY4SjHU3ricV6zBcAe1EeILKkeScr+fZXtaI5WyDbkVowJxxAI6h73NcFPmXolQ==",
             "requires": {
+                "@colors/colors": "1.5.0",
                 "body-parser": "^1.19.0",
                 "braces": "^3.0.2",
                 "chokidar": "^3.5.1",
-                "colors": "1.4.0",
                 "connect": "^3.7.0",
                 "di": "^0.0.1",
                 "dom-serialize": "^2.2.1",
                 "glob": "^7.1.7",
                 "graceful-fs": "^4.2.6",
                 "http-proxy": "^1.18.1",
                 "isbinaryfile": "^4.0.8",
@@ -1826,31 +1850,32 @@
                 "log4js": "^6.4.1",
                 "mime": "^2.5.2",
                 "minimatch": "^3.0.4",
                 "mkdirp": "^0.5.5",
                 "qjobs": "^1.2.0",
                 "range-parser": "^1.2.1",
                 "rimraf": "^3.0.2",
-                "socket.io": "^4.2.0",
+                "socket.io": "^4.4.1",
                 "source-map": "^0.6.1",
                 "tmp": "^0.2.1",
                 "ua-parser-js": "^0.7.30",
                 "yargs": "^16.1.1"
             },
-            "resolved": "https://registry.npmjs.org/karma/-/karma-6.3.16.tgz",
-            "version": "6.3.16"
+            "resolved": "https://registry.npmjs.org/karma/-/karma-6.4.2.tgz",
+            "version": "6.4.2"
         },
         "karma-firefox-launcher": {
             "dev": true,
-            "integrity": "sha512-Fi7xPhwrRgr+94BnHX0F5dCl1miIW4RHnzjIGxF8GaIEp7rNqX7LSi7ok63VXs3PS/5MQaQMhGxw+bvD+pibBQ==",
+            "integrity": "sha512-VV9xDQU1QIboTrjtGVD4NCfzIH7n01ZXqy/qpBhnOeGVOkG5JYPEm8kuSd7psHE6WouZaQ9Ool92g8LFweSNMA==",
             "requires": {
-                "is-wsl": "^2.1.0"
+                "is-wsl": "^2.2.0",
+                "which": "^2.0.1"
             },
-            "resolved": "https://registry.npmjs.org/karma-firefox-launcher/-/karma-firefox-launcher-1.3.0.tgz",
-            "version": "1.3.0"
+            "resolved": "https://registry.npmjs.org/karma-firefox-launcher/-/karma-firefox-launcher-2.1.2.tgz",
+            "version": "2.1.2"
         },
         "karma-mocha": {
             "dev": true,
             "integrity": "sha512-Tzd5HBjm8his2OA4bouAsATYEpZrp9vC7z5E5j4C5Of5Rrs1jY67RAwXNcVmd/Bnk1wgvQRou0zGVLey44G4tQ==",
             "requires": {
                 "minimist": "^1.2.3"
             },
@@ -1909,54 +1934,54 @@
             "resolved": "https://registry.npmjs.org/log-symbols/-/log-symbols-2.2.0.tgz",
             "version": "2.2.0"
         },
         "log4js": {
             "dependencies": {
                 "debug": {
                     "dev": true,
-                    "integrity": "sha512-/zxw5+vh1Tfv+4Qn7a5nsbcJKPaSvCDhojn6FEl9vupwK2VCSDtEiEtqr8DFtzYFOdz63LBkxec7DYuc2jon6Q==",
+                    "integrity": "sha512-PRWFHuSU3eDtQJPvnNY7Jcket1j0t5OuOsFzPPzsekD52Zl8qUfFIPEiswXqIvHWGVHOgX+7G/vCNNhehwxfkQ==",
                     "requires": {
                         "ms": "2.1.2"
                     },
-                    "resolved": "https://registry.npmjs.org/debug/-/debug-4.3.3.tgz",
-                    "version": "4.3.3"
+                    "resolved": "https://registry.npmjs.org/debug/-/debug-4.3.4.tgz",
+                    "version": "4.3.4"
                 },
                 "ms": {
                     "dev": true,
                     "integrity": "sha512-sGkPx+VjMtmA6MX27oA4FBFELFCZZ4S4XqeGOXCv68tT+jb3vk/RyaKWP0PTKyWtmLSM0b+adUTEvbs1PEaH2w==",
                     "resolved": "https://registry.npmjs.org/ms/-/ms-2.1.2.tgz",
                     "version": "2.1.2"
                 }
             },
             "dev": true,
-            "integrity": "sha512-iUiYnXqAmNKiIZ1XSAitQ4TmNs8CdZYTAWINARF3LjnsLN8tY5m0vRwd6uuWj/yNY0YHxeZodnbmxKFUOM2rMg==",
+            "integrity": "sha512-1somDdy9sChrr9/f4UlzhdaGfDR2c/SaD2a4T7qEkG4jTS57/B3qmnjLYePwQ8cqWnUHZI0iAKxMBpCZICiZ2g==",
             "requires": {
-                "date-format": "^4.0.3",
-                "debug": "^4.3.3",
-                "flatted": "^3.2.4",
+                "date-format": "^4.0.14",
+                "debug": "^4.3.4",
+                "flatted": "^3.2.7",
                 "rfdc": "^1.3.0",
-                "streamroller": "^3.0.2"
+                "streamroller": "^3.1.5"
             },
-            "resolved": "https://registry.npmjs.org/log4js/-/log4js-6.4.1.tgz",
-            "version": "6.4.1"
+            "resolved": "https://registry.npmjs.org/log4js/-/log4js-6.9.1.tgz",
+            "version": "6.9.1"
         },
         "md5.js": {
             "dev": true,
             "integrity": "sha512-xitP+WxNPcTTOgnTJcrhM0xvdPepipPSf3I8EIpGKeFLjt3PlJLIDG3u8EX53ZIubkb+5U2+3rELYpEhHhzdkg==",
             "requires": {
                 "hash-base": "^3.0.0",
                 "inherits": "^2.0.1",
                 "safe-buffer": "^5.1.2"
             },
             "resolved": "https://registry.npmjs.org/md5.js/-/md5.js-1.3.5.tgz",
             "version": "1.3.5"
         },
         "media-typer": {
             "dev": true,
-            "integrity": "sha1-hxDXrwqmJvj/+hzgAWhUUmMlV0g=",
+            "integrity": "sha512-dq+qelQ9akHpcOl/gUVRTxVIOkAJ1wR3QAvb4RsVjS8oVoFjDGTc679wJYmUmknUF5HwMLOgb5O+a3KxfWapPQ==",
             "resolved": "https://registry.npmjs.org/media-typer/-/media-typer-0.3.0.tgz",
             "version": "0.3.0"
         },
         "merge-stream": {
             "dev": true,
             "integrity": "sha512-abv/qOcuPfk3URPfDzmZU1LKmuw8kT+0nIHvKrKgFrwifol/doWcdA4ZqsWQ8ENrFKkd67Mfpo/LovbIUsbt3w==",
             "resolved": "https://registry.npmjs.org/merge-stream/-/merge-stream-2.0.0.tgz",
@@ -1978,17 +2003,17 @@
                 "brorand": "^1.0.1"
             },
             "resolved": "https://registry.npmjs.org/miller-rabin/-/miller-rabin-4.0.1.tgz",
             "version": "4.0.1"
         },
         "mime": {
             "dev": true,
-            "integrity": "sha512-KI1+qOZu5DcW6wayYHSzR/tXKCDC5Om4s1z2QJjDULzLcmf3DvzS7oluY4HCTrc+9FiKmWUgeNLg7W3uIQvxtQ==",
-            "resolved": "https://registry.npmjs.org/mime/-/mime-1.4.1.tgz",
-            "version": "1.4.1"
+            "integrity": "sha512-jSCU7/VB1loIWBZe14aEYHU/+1UMEHoaO7qxCOVJOw9GgH72VAWppxNcjU+x9a2k3GSIBXNKxXQFqRvvZ7vr3A==",
+            "resolved": "https://registry.npmjs.org/mime/-/mime-3.0.0.tgz",
+            "version": "3.0.0"
         },
         "mime-db": {
             "dev": true,
             "integrity": "sha512-QBmA/G2y+IfeS4oktet3qRZ+P5kPhCKRXxXnQEudYqUaEioAU1/Lq2us3D/t1Jfo4hE9REQPrbB7K5sOczJVIw==",
             "resolved": "https://registry.npmjs.org/mime-db/-/mime-db-1.47.0.tgz",
             "version": "1.47.0"
         },
@@ -2026,20 +2051,20 @@
             "dev": true,
             "integrity": "sha512-Jsjnk4bw3YJqYzbdyBiNsPWHPfO++UGG749Cxs6peCu5Xg4nrena6OVxOYxrQTqww0Jmwt+Ref8rggumkTLz9Q==",
             "resolved": "https://registry.npmjs.org/minimist/-/minimist-1.2.6.tgz",
             "version": "1.2.6"
         },
         "mkdirp": {
             "dev": true,
-            "integrity": "sha512-NKmAlESf6jMGym1++R0Ra7wvhV+wFW63FaSOFPwRahvea0gMUcGUhVeAg/0BC0wiv9ih5NYPB1Wn1UEI1/L+xQ==",
+            "integrity": "sha512-FP+p8RB8OWpF3YZBCrP5gtADmtXApB5AMLn+vdyA+PyxCjrCs00mjyUozssO33cwDeT3wNGdLxJ5M//YqtHAJw==",
             "requires": {
-                "minimist": "^1.2.5"
+                "minimist": "^1.2.6"
             },
-            "resolved": "https://registry.npmjs.org/mkdirp/-/mkdirp-0.5.5.tgz",
-            "version": "0.5.5"
+            "resolved": "https://registry.npmjs.org/mkdirp/-/mkdirp-0.5.6.tgz",
+            "version": "0.5.6"
         },
         "mocha": {
             "dependencies": {
                 "ansi-styles": {
                     "dev": true,
                     "integrity": "sha512-zbB9rCJAT1rbjiVDb2hqKFHNYLxgtk8NURxZ3IZwD3F6NtxbXZQCnnSi1Lkx+IDohdPlFp222wVALIheZJQSEg==",
                     "requires": {
@@ -2210,15 +2235,15 @@
                 "yargs-unparser": "2.0.0"
             },
             "resolved": "https://registry.npmjs.org/mocha/-/mocha-10.2.0.tgz",
             "version": "10.2.0"
         },
         "ms": {
             "dev": true,
-            "integrity": "sha1-VgiurfwAvmwpAd9fmGF4jeDVl8g=",
+            "integrity": "sha512-Tpp60P6IUJDTuOq/5Z8cdskzJujfwqfOTkrwIwj7IRISpnkJnT6SyJ4PCPnGMoFjC9ddhal5KVIYtAt97ix05A==",
             "resolved": "https://registry.npmjs.org/ms/-/ms-2.0.0.tgz",
             "version": "2.0.0"
         },
         "nanoid": {
             "dev": true,
             "integrity": "sha512-p1sjXuopFs0xg+fPASzQ28agW1oHD7xDsd9Xkf3T15H3c/cifrFHVwrh74PdoklAPi+i7MdRsE47vm2r6JoB+w==",
             "resolved": "https://registry.npmjs.org/nanoid/-/nanoid-3.3.3.tgz",
@@ -2234,27 +2259,27 @@
             "dev": true,
             "integrity": "sha512-Yd3UES5mWCSqR+qNT93S3UoYUkqAZ9lLg8a7g9rimsWmYGK8cVToA4/sF3RrshdyV3sAGMXVUmpMYOw+dLpOuw==",
             "resolved": "https://registry.npmjs.org/neo-async/-/neo-async-2.6.2.tgz",
             "version": "2.6.2"
         },
         "node-releases": {
             "dev": true,
-            "integrity": "sha512-5GFldHPXVG/YZmFzJvKK2zDSzPKhEp0+ZR5SVaoSag9fsL5YgHbUHDfnG5494ISANDcK4KwPXAx2xqVEydmd7w==",
-            "resolved": "https://registry.npmjs.org/node-releases/-/node-releases-2.0.10.tgz",
-            "version": "2.0.10"
+            "integrity": "sha512-QzsYKWhXTWx8h1kIvqfnC++o0pEmpRQA/aenALsL2F4pqNVr7YzcdMlDij5WBnwftRbJCNJL/O7zdKaxKPHqgQ==",
+            "resolved": "https://registry.npmjs.org/node-releases/-/node-releases-2.0.12.tgz",
+            "version": "2.0.12"
         },
         "normalize-path": {
             "dev": true,
             "integrity": "sha512-6eZs5Ls3WtCisHWp9S2GUy8dqkpGi4BVSz3GaqiE6ezub0512ESztXUwUB6C6IKbQkY2Pnb/mD4WYojCRwcwLA==",
             "resolved": "https://registry.npmjs.org/normalize-path/-/normalize-path-3.0.0.tgz",
             "version": "3.0.0"
         },
         "object-assign": {
             "dev": true,
-            "integrity": "sha1-IQmtx5ZYh8/AXLvUQsrIv7s2CGM=",
+            "integrity": "sha512-rJgTQnkUnH1sFw8yT6VSU3zD3sWmu6sZhIseY8VX+GRu3P6F7Fu+JNDoXfklElbLJSnc3FUQHVe4cU5hj+BcUg==",
             "resolved": "https://registry.npmjs.org/object-assign/-/object-assign-4.1.1.tgz",
             "version": "4.1.1"
         },
         "object-inspect": {
             "dev": true,
             "integrity": "sha512-jp7ikS6Sd3GxQfZJPyH3cjcbJF6GZPClgdV+EFygjFLQ5FmW/dRUnTd9PQ9k0JhoNDabWFbpF1yCdSWCC6gexg==",
             "resolved": "https://registry.npmjs.org/object-inspect/-/object-inspect-1.11.0.tgz",
@@ -2274,20 +2299,20 @@
             "dev": true,
             "integrity": "sha512-6OO5X1+2tYkNyNEx6TsCxEqFfRWaqx6EtMiSbGrw8Ob8v9Ne+Hl8rBAgLBZn5wjEz3s/s6U1WXFUFOcxxAwUpg==",
             "resolved": "https://registry.npmjs.org/object-keys/-/object-keys-1.1.0.tgz",
             "version": "1.1.0"
         },
         "on-finished": {
             "dev": true,
-            "integrity": "sha1-IPEzZIGwg811M3mSoWlxqi2QaUc=",
+            "integrity": "sha512-oVlzkg3ENAhCk2zdv7IJwd/QUD4z2RxRwpkcGY8psCVcCYZNq4wYnVWALHM+brtuJjePWiYF/ClmuDr8Ch5+kg==",
             "requires": {
                 "ee-first": "1.1.1"
             },
-            "resolved": "https://registry.npmjs.org/on-finished/-/on-finished-2.3.0.tgz",
-            "version": "2.3.0"
+            "resolved": "https://registry.npmjs.org/on-finished/-/on-finished-2.4.1.tgz",
+            "version": "2.4.1"
         },
         "once": {
             "dev": true,
             "integrity": "sha1-WDsap3WWHUsROsF9nFC6753Xa9E=",
             "requires": {
                 "wrappy": "1"
             },
@@ -2412,17 +2437,20 @@
             "dev": true,
             "integrity": "sha512-8YOJEHtxpySA3fFDyCRxA+UUV+fA+rTWnuWvylOK/NCjhY+b4ocCtmu8TtsWb+mYeU+GCHf/S66KZF/AsteKHg==",
             "resolved": "https://registry.npmjs.org/qjobs/-/qjobs-1.2.0.tgz",
             "version": "1.2.0"
         },
         "qs": {
             "dev": true,
-            "integrity": "sha512-IhMFgUmuNpyRfxA90umL7ByLlgRXu6tIfKPpF5TmcfRLlLCckfP/g3IQmju6jjpu+Hh8rA+2p6A27ZSPOOHdKw==",
-            "resolved": "https://registry.npmjs.org/qs/-/qs-6.9.7.tgz",
-            "version": "6.9.7"
+            "integrity": "sha512-MvjoMCJwEarSbUYk5O+nmoSzSutSsTwF85zcHPQ9OrlFoZOYIjaqBAJIqIXjptyD5vThxGq52Xu/MaJzRkIk4Q==",
+            "requires": {
+                "side-channel": "^1.0.4"
+            },
+            "resolved": "https://registry.npmjs.org/qs/-/qs-6.11.0.tgz",
+            "version": "6.11.0"
         },
         "randombytes": {
             "dev": true,
             "integrity": "sha512-vYl3iOX+4CKUWuxGi9Ukhie6fsqXqS9FE2Zaic4tNFD2N2QQaXOMFbuKK4QmDHC0JO6B1Zp41J0LpT0oR68amQ==",
             "requires": {
                 "safe-buffer": "^5.1.0"
             },
@@ -2443,23 +2471,23 @@
             "dev": true,
             "integrity": "sha512-Hrgsx+orqoygnmhFbKaHE6c296J+HTAQXoxEF6gNupROmmGJRoyzfG3ccAveqCBrwr/2yxQ5BVd/GTl5agOwSg==",
             "resolved": "https://registry.npmjs.org/range-parser/-/range-parser-1.2.1.tgz",
             "version": "1.2.1"
         },
         "raw-body": {
             "dev": true,
-            "integrity": "sha512-UlTNLIcu0uzb4D2f4WltY6cVjLi+/jEN4lgEUj3E04tpMDpUlkBo/eSn6zou9hum2VMNpCCUone0O0WeJim07g==",
+            "integrity": "sha512-8zGqypfENjCIqGhgXToC8aB2r7YrBX+AQAfIPs/Mlk+BtPTztOvTS01NRW/3Eh60J+a48lt8qsCzirQ6loCVfA==",
             "requires": {
                 "bytes": "3.1.2",
-                "http-errors": "1.8.1",
+                "http-errors": "2.0.0",
                 "iconv-lite": "0.4.24",
                 "unpipe": "1.0.0"
             },
-            "resolved": "https://registry.npmjs.org/raw-body/-/raw-body-2.4.3.tgz",
-            "version": "2.4.3"
+            "resolved": "https://registry.npmjs.org/raw-body/-/raw-body-2.5.2.tgz",
+            "version": "2.5.2"
         },
         "readable-stream": {
             "dev": true,
             "integrity": "sha512-BViHy7LKeTz4oNnkcLJ+lVSL6vpiFeX6/d3oSH8zCW7UxP2onchk+vTGB143xuFjHS3deTgkKoXXymXqymiIdA==",
             "requires": {
                 "inherits": "^2.0.3",
                 "string_decoder": "^1.1.1",
@@ -2487,15 +2515,15 @@
             "dev": true,
             "integrity": "sha1-jGStX9MNqxyXbiNE/+f3kqam30I=",
             "resolved": "https://registry.npmjs.org/require-directory/-/require-directory-2.1.1.tgz",
             "version": "2.1.1"
         },
         "requires-port": {
             "dev": true,
-            "integrity": "sha1-kl0mAdOaxIXgkc8NpcbmlNw9yv8=",
+            "integrity": "sha512-KigOCHcocU3XODJxsu8i/j8T9tzT4adHiecwORRQ0ZZFcp7ahwXuRU1m+yuO90C5ZUyGeGfocHDI14M3L3yDAQ==",
             "resolved": "https://registry.npmjs.org/requires-port/-/requires-port-1.0.0.tgz",
             "version": "1.0.0"
         },
         "rfdc": {
             "dev": true,
             "integrity": "sha512-V2hovdzFbOi77/WajaSMXk2OLm+xNIeQdMMuB7icj7bk6zi2F8GGAxigcnDFpJHbNyNcgyJDiP+8nOrY5cZGrA==",
             "resolved": "https://registry.npmjs.org/rfdc/-/rfdc-1.3.0.tgz",
@@ -2564,14 +2592,25 @@
             "requires": {
                 "inherits": "^2.0.1",
                 "safe-buffer": "^5.0.1"
             },
             "resolved": "https://registry.npmjs.org/sha.js/-/sha.js-2.4.11.tgz",
             "version": "2.4.11"
         },
+        "side-channel": {
+            "dev": true,
+            "integrity": "sha512-q5XPytqFEIKHkGdiMIrY10mvLRvnQh42/+GoBlFW3b2LXLE2xxJpZFdm94we0BaoV3RwJyGqg5wS7epxTv0Zvw==",
+            "requires": {
+                "call-bind": "^1.0.0",
+                "get-intrinsic": "^1.0.2",
+                "object-inspect": "^1.9.0"
+            },
+            "resolved": "https://registry.npmjs.org/side-channel/-/side-channel-1.0.4.tgz",
+            "version": "1.0.4"
+        },
         "socket.io": {
             "dependencies": {
                 "debug": {
                     "dev": true,
                     "integrity": "sha512-PRWFHuSU3eDtQJPvnNY7Jcket1j0t5OuOsFzPPzsekD52Zl8qUfFIPEiswXqIvHWGVHOgX+7G/vCNNhehwxfkQ==",
                     "requires": {
                         "ms": "2.1.2"
@@ -2580,43 +2619,37 @@
                     "version": "4.3.4"
                 },
                 "ms": {
                     "dev": true,
                     "integrity": "sha512-sGkPx+VjMtmA6MX27oA4FBFELFCZZ4S4XqeGOXCv68tT+jb3vk/RyaKWP0PTKyWtmLSM0b+adUTEvbs1PEaH2w==",
                     "resolved": "https://registry.npmjs.org/ms/-/ms-2.1.2.tgz",
                     "version": "2.1.2"
-                },
-                "socket.io-adapter": {
-                    "dev": true,
-                    "integrity": "sha512-87C3LO/NOMc+eMcpcxUBebGjkpMDkNBS9tf7KJqcDsmL936EChtVva71Dw2q4tQcuVC+hAUy4an2NO/sYXmwRA==",
-                    "requires": {
-                        "ws": "~8.11.0"
-                    },
-                    "resolved": "https://registry.npmjs.org/socket.io-adapter/-/socket.io-adapter-2.5.2.tgz",
-                    "version": "2.5.2"
-                },
-                "ws": {
-                    "dev": true,
-                    "integrity": "sha512-HPG3wQd9sNQoT9xHyNCXoDUa+Xw/VevmY9FoHyQ+g+rrMn4j6FB4np7Z0OhdTgjx6MgQLK7jwSy1YecU1+4Asg==",
-                    "resolved": "https://registry.npmjs.org/ws/-/ws-8.11.0.tgz",
-                    "version": "8.11.0"
                 }
             },
             "dev": true,
-            "integrity": "sha512-KMcaAi4l/8+xEjkRICl6ak8ySoxsYG+gG6/XfRCPJPQ/haCRIJBTL4wIl8YCsmtaBovcAXGLOShyVWQ/FG8GZA==",
+            "integrity": "sha512-Vp+lSks5k0dewYTfwgPT9UeGGd+ht7sCpB7p0e83VgO4X/AHYWhXITMrNk/pg8syY2bpx23ptClCQuHhqi2BgQ==",
             "requires": {
                 "accepts": "~1.3.4",
                 "base64id": "~2.0.0",
                 "debug": "~4.3.2",
-                "engine.io": "~6.4.1",
+                "engine.io": "~6.4.2",
                 "socket.io-adapter": "~2.5.2",
-                "socket.io-parser": "~4.2.1"
+                "socket.io-parser": "~4.2.4"
             },
-            "resolved": "https://registry.npmjs.org/socket.io/-/socket.io-4.6.1.tgz",
-            "version": "4.6.1"
+            "resolved": "https://registry.npmjs.org/socket.io/-/socket.io-4.6.2.tgz",
+            "version": "4.6.2"
+        },
+        "socket.io-adapter": {
+            "dev": true,
+            "integrity": "sha512-87C3LO/NOMc+eMcpcxUBebGjkpMDkNBS9tf7KJqcDsmL936EChtVva71Dw2q4tQcuVC+hAUy4an2NO/sYXmwRA==",
+            "requires": {
+                "ws": "~8.11.0"
+            },
+            "resolved": "https://registry.npmjs.org/socket.io-adapter/-/socket.io-adapter-2.5.2.tgz",
+            "version": "2.5.2"
         },
         "socket.io-parser": {
             "dependencies": {
                 "debug": {
                     "dev": true,
                     "integrity": "sha512-PRWFHuSU3eDtQJPvnNY7Jcket1j0t5OuOsFzPPzsekD52Zl8qUfFIPEiswXqIvHWGVHOgX+7G/vCNNhehwxfkQ==",
                     "requires": {
@@ -2629,21 +2662,21 @@
                     "dev": true,
                     "integrity": "sha512-sGkPx+VjMtmA6MX27oA4FBFELFCZZ4S4XqeGOXCv68tT+jb3vk/RyaKWP0PTKyWtmLSM0b+adUTEvbs1PEaH2w==",
                     "resolved": "https://registry.npmjs.org/ms/-/ms-2.1.2.tgz",
                     "version": "2.1.2"
                 }
             },
             "dev": true,
-            "integrity": "sha512-JMafRntWVO2DCJimKsRTh/wnqVvO4hrfwOqtO7f+uzwsQMuxO6VwImtYxaQ+ieoyshWOTJyV0fA21lccEXRPpQ==",
+            "integrity": "sha512-/GbIKmo8ioc+NIWIhwdecY0ge+qVBSMdgxGygevmdHj24bsfgtCmcUUcQ5ZzcylGFHsN3k4HB4Cgkl96KVnuew==",
             "requires": {
                 "@socket.io/component-emitter": "~3.1.0",
                 "debug": "~4.3.1"
             },
-            "resolved": "https://registry.npmjs.org/socket.io-parser/-/socket.io-parser-4.2.3.tgz",
-            "version": "4.2.3"
+            "resolved": "https://registry.npmjs.org/socket.io-parser/-/socket.io-parser-4.2.4.tgz",
+            "version": "4.2.4"
         },
         "source-map": {
             "dev": true,
             "integrity": "sha512-UjgapumWlbMhkBgzT7Ykc5YXUT46F0iKu8SGXq0bcwP5dz/h0Plj6enJqjz1Zbq2l5WaqYnrVbwWOWMyF3F47g==",
             "resolved": "https://registry.npmjs.org/source-map/-/source-map-0.6.1.tgz",
             "version": "0.6.1"
         },
@@ -2655,17 +2688,17 @@
                 "source-map": "^0.6.0"
             },
             "resolved": "https://registry.npmjs.org/source-map-support/-/source-map-support-0.5.21.tgz",
             "version": "0.5.21"
         },
         "statuses": {
             "dev": true,
-            "integrity": "sha1-Fhx9rBd2Wf2YEfQ3cfqZOBR4Yow=",
-            "resolved": "https://registry.npmjs.org/statuses/-/statuses-1.5.0.tgz",
-            "version": "1.5.0"
+            "integrity": "sha512-RwNA9Z/7PrK06rYLIzFMlaF+l73iwpzsqRIFgbMLbTcLD6cOao82TaWefPXQvB2fOC4AjuYSEndS7N/mTCbkdQ==",
+            "resolved": "https://registry.npmjs.org/statuses/-/statuses-2.0.1.tgz",
+            "version": "2.0.1"
         },
         "stream-browserify": {
             "dependencies": {
                 "inherits": {
                     "dev": true,
                     "integrity": "sha512-k/vGaX4/Yla3WzyMCvTQOXYeIHvqOKtnqBduzTHpzpQZzAskKMhZ2K+EnBiSM9zGSoIFeMpXKxa4dYeZIQqewQ==",
                     "resolved": "https://registry.npmjs.org/inherits/-/inherits-2.0.4.tgz",
@@ -2681,37 +2714,37 @@
             "resolved": "https://registry.npmjs.org/stream-browserify/-/stream-browserify-3.0.0.tgz",
             "version": "3.0.0"
         },
         "streamroller": {
             "dependencies": {
                 "debug": {
                     "dev": true,
-                    "integrity": "sha512-/zxw5+vh1Tfv+4Qn7a5nsbcJKPaSvCDhojn6FEl9vupwK2VCSDtEiEtqr8DFtzYFOdz63LBkxec7DYuc2jon6Q==",
+                    "integrity": "sha512-PRWFHuSU3eDtQJPvnNY7Jcket1j0t5OuOsFzPPzsekD52Zl8qUfFIPEiswXqIvHWGVHOgX+7G/vCNNhehwxfkQ==",
                     "requires": {
                         "ms": "2.1.2"
                     },
-                    "resolved": "https://registry.npmjs.org/debug/-/debug-4.3.3.tgz",
-                    "version": "4.3.3"
+                    "resolved": "https://registry.npmjs.org/debug/-/debug-4.3.4.tgz",
+                    "version": "4.3.4"
                 },
                 "ms": {
                     "dev": true,
                     "integrity": "sha512-sGkPx+VjMtmA6MX27oA4FBFELFCZZ4S4XqeGOXCv68tT+jb3vk/RyaKWP0PTKyWtmLSM0b+adUTEvbs1PEaH2w==",
                     "resolved": "https://registry.npmjs.org/ms/-/ms-2.1.2.tgz",
                     "version": "2.1.2"
                 }
             },
             "dev": true,
-            "integrity": "sha512-ur6y5S5dopOaRXBuRIZ1u6GC5bcEXHRZKgfBjfCglMhmIf+roVCECjvkEYzNQOXIN2/JPnkMPW/8B3CZoKaEPA==",
+            "integrity": "sha512-KFxaM7XT+irxvdqSP1LGLgNWbYN7ay5owZ3r/8t77p+EtSUAfUgtl7be3xtqtOmGUl9K9YPO2ca8133RlTjvKw==",
             "requires": {
-                "date-format": "^4.0.3",
-                "debug": "^4.1.1",
-                "fs-extra": "^10.0.0"
+                "date-format": "^4.0.14",
+                "debug": "^4.3.4",
+                "fs-extra": "^8.1.0"
             },
-            "resolved": "https://registry.npmjs.org/streamroller/-/streamroller-3.0.2.tgz",
-            "version": "3.0.2"
+            "resolved": "https://registry.npmjs.org/streamroller/-/streamroller-3.1.5.tgz",
+            "version": "3.1.5"
         },
         "string.prototype.trimend": {
             "dev": true,
             "integrity": "sha512-y9xCjw1P23Awk8EvTpcyL2NIr1j7wJ39f+k6lvRnSMz+mz9CGz9NYPelDk42kOz6+ql8xjfK8oYzy3jAP5QU5A==",
             "requires": {
                 "call-bind": "^1.0.2",
                 "define-properties": "^1.1.3"
@@ -2790,36 +2823,36 @@
             "dev": true,
             "integrity": "sha512-GNzQvQTOIP6RyTfE2Qxb8ZVlNmw0n88vp1szwWRimP02mnTsx3Wtn5qRdqY9w2XduFNUgvOwhNnQsjwCp+kqaQ==",
             "resolved": "https://registry.npmjs.org/tapable/-/tapable-2.2.1.tgz",
             "version": "2.2.1"
         },
         "terser": {
             "dev": true,
-            "integrity": "sha512-hVl35zClmpisy6oaoKALOpS0rDYLxRFLHhRuDlEGTKey9qHjS1w9GMORjuwIMt70Wan4lwsLYyWDVnWgF+KUEw==",
+            "integrity": "sha512-/bi0Zm2C6VAexlGgLlVxA0P2lru/sdLyfCVaRMfKVo9nWxbmz7f/sD8VPybPeSUJaJcwmCJis9pBIhcVcG1QcQ==",
             "requires": {
-                "@jridgewell/source-map": "^0.3.2",
-                "acorn": "^8.5.0",
+                "@jridgewell/source-map": "^0.3.3",
+                "acorn": "^8.8.2",
                 "commander": "^2.20.0",
                 "source-map-support": "~0.5.20"
             },
-            "resolved": "https://registry.npmjs.org/terser/-/terser-5.17.1.tgz",
-            "version": "5.17.1"
+            "resolved": "https://registry.npmjs.org/terser/-/terser-5.17.7.tgz",
+            "version": "5.17.7"
         },
         "terser-webpack-plugin": {
             "dev": true,
-            "integrity": "sha512-AfKwIktyP7Cu50xNjXF/6Qb5lBNzYaWpU6YfoX3uZicTx0zTy0stDDCsvjDapKsSDvOeWo5MEq4TmdBy2cNoHw==",
+            "integrity": "sha512-ZuXsqE07EcggTWQjXUj+Aot/OMcD0bMKGgF63f7UxYcu5/AJF53aIpK1YoP5xR9l6s/Hy2b+t1AM0bLNPRuhwA==",
             "requires": {
                 "@jridgewell/trace-mapping": "^0.3.17",
                 "jest-worker": "^27.4.5",
                 "schema-utils": "^3.1.1",
                 "serialize-javascript": "^6.0.1",
-                "terser": "^5.16.5"
+                "terser": "^5.16.8"
             },
-            "resolved": "https://registry.npmjs.org/terser-webpack-plugin/-/terser-webpack-plugin-5.3.7.tgz",
-            "version": "5.3.7"
+            "resolved": "https://registry.npmjs.org/terser-webpack-plugin/-/terser-webpack-plugin-5.3.9.tgz",
+            "version": "5.3.9"
         },
         "tmp": {
             "dev": true,
             "integrity": "sha512-76SUhtfqR2Ijn+xllcI5P1oyannHNHByD80W1q447gU3mp9G9PSpGdWmjUOHRDPiHYacIk66W7ubDTuPF3BEtQ==",
             "requires": {
                 "rimraf": "^3.0.0"
             },
@@ -2849,23 +2882,23 @@
                 "mime-types": "~2.1.24"
             },
             "resolved": "https://registry.npmjs.org/type-is/-/type-is-1.6.18.tgz",
             "version": "1.6.18"
         },
         "typescript": {
             "dev": true,
-            "integrity": "sha512-BLbiRkiBzAwsjut4x/dsibSTB6yWpwT5qWmC2OfuCg3GgVQCSgMs4vEctYPhsaGtd0AeuuHMkjZ2h2WG8MSzRw==",
-            "resolved": "https://registry.npmjs.org/typescript/-/typescript-3.9.7.tgz",
-            "version": "3.9.7"
+            "integrity": "sha512-cW9T5W9xY37cc+jfEnaUvX91foxtHkza3Nw3wkoF4sSlKn0MONdkdEndig/qPBWXNkmplh3NzayQzCiHM4/hqw==",
+            "resolved": "https://registry.npmjs.org/typescript/-/typescript-5.0.4.tgz",
+            "version": "5.0.4"
         },
         "ua-parser-js": {
             "dev": true,
-            "integrity": "sha512-s8ax/CeZdK9R/56Sui0WM6y9OFREJarMRHqLB2EwkovemBxNQ+Bqu8GAsUnVcXKgphb++ghr/B2BZx4mahujPw==",
-            "resolved": "https://registry.npmjs.org/ua-parser-js/-/ua-parser-js-0.7.33.tgz",
-            "version": "0.7.33"
+            "integrity": "sha512-veRf7dawaj9xaWEu9HoTVn5Pggtc/qj+kqTOFvNiN1l0YdxwC1kvel57UCjThjGa3BHBihE8/UJAHI+uQHmd/g==",
+            "resolved": "https://registry.npmjs.org/ua-parser-js/-/ua-parser-js-0.7.35.tgz",
+            "version": "0.7.35"
         },
         "unbox-primitive": {
             "dependencies": {
                 "has-symbols": {
                     "dev": true,
                     "integrity": "sha512-chXa79rL/UC2KlX17jo3vRGz0azaWEx5tGqZg5pO3NUyEJVB17dMruQlzCCOfUvElghKcm5194+BCRvi2Rv/Gw==",
                     "resolved": "https://registry.npmjs.org/has-symbols/-/has-symbols-1.0.2.tgz",
@@ -2881,21 +2914,21 @@
                 "which-boxed-primitive": "^1.0.2"
             },
             "resolved": "https://registry.npmjs.org/unbox-primitive/-/unbox-primitive-1.0.1.tgz",
             "version": "1.0.1"
         },
         "universalify": {
             "dev": true,
-            "integrity": "sha512-hAZsKq7Yy11Zu1DE0OzWjw7nnLZmJZYTDZZyEFHZdUhV8FkH5MCfoU1XMaxXovpyW5nq5scPqq0ZDP9Zyl04oQ==",
-            "resolved": "https://registry.npmjs.org/universalify/-/universalify-2.0.0.tgz",
-            "version": "2.0.0"
+            "integrity": "sha512-rBJeI5CXAlmy1pV+617WB9J63U6XcazHHF2f2dbJix4XzpUF0RS3Zbj0FGIOCAva5P/d/GBOYaACQ1w+0azUkg==",
+            "resolved": "https://registry.npmjs.org/universalify/-/universalify-0.1.2.tgz",
+            "version": "0.1.2"
         },
         "unpipe": {
             "dev": true,
-            "integrity": "sha1-sr9O6FFKrmFltIF4KdIbLvSZBOw=",
+            "integrity": "sha512-pjy2bYhSsufwWlKwPc+l3cN7+wuJlK6uz0YdJEOlQDbl6jo/YlPi4mb8agUkVC8BF7V8NuzeyPNqRksA3hztKQ==",
             "resolved": "https://registry.npmjs.org/unpipe/-/unpipe-1.0.0.tgz",
             "version": "1.0.0"
         },
         "update-browserslist-db": {
             "dev": true,
             "integrity": "sha512-dCwEFf0/oT85M1fHBg4F0jtLwJrutGoHSQXCh7u4o2t1drG+c0a9Flnqww6XUKSfQMPpJBRjU8d4RXB09qtvaA==",
             "requires": {
@@ -2932,27 +2965,27 @@
             "dev": true,
             "integrity": "sha1-RQ1Nyfpw3nMnYvvS1KKJgUGaDM8=",
             "resolved": "https://registry.npmjs.org/util-deprecate/-/util-deprecate-1.0.2.tgz",
             "version": "1.0.2"
         },
         "utils-merge": {
             "dev": true,
-            "integrity": "sha1-n5VxD1CiZ5R7LMwSR0HBAoQn5xM=",
+            "integrity": "sha512-pMZTvIkT1d+TFGvDOqodOclx0QWkkgi6Tdoa8gC8ffGAAqz9pzPTZWAybbsHHoED/ztMtkv/VoYTYyShUn81hA==",
             "resolved": "https://registry.npmjs.org/utils-merge/-/utils-merge-1.0.1.tgz",
             "version": "1.0.1"
         },
         "vary": {
             "dev": true,
-            "integrity": "sha1-IpnwLG3tMNSllhsLn3RSShj2NPw=",
+            "integrity": "sha512-BNGbWLfd0eUPabhkXUVm0j8uuvREyTh5ovRa/dyow/BqAbZJyC+5fU+IzQOzmAKzYqYRAISoRhdQr3eIZ/PXqg==",
             "resolved": "https://registry.npmjs.org/vary/-/vary-1.1.2.tgz",
             "version": "1.1.2"
         },
         "void-elements": {
             "dev": true,
-            "integrity": "sha1-wGavtYK7HLQSjWDqkjkulNXp2+w=",
+            "integrity": "sha512-qZKX4RnBzH2ugr8Lxa7x+0V6XD9Sb/ouARtiasEQCHB1EVU4NXtmHsDDrx1dO4ne5fc3J6EW05BP1Dl0z0iung==",
             "resolved": "https://registry.npmjs.org/void-elements/-/void-elements-2.0.1.tgz",
             "version": "2.0.1"
         },
         "watchpack": {
             "dev": true,
             "integrity": "sha512-Lcvm7MGST/4fup+ifyKi2hjyIAwcdI4HRgtvTpIUxBRhB+RFtUh8XtDOxUfctVCnhVi+QQj49i91OyvzkJl6cg==",
             "requires": {
@@ -2968,43 +3001,43 @@
                     "dev": true,
                     "integrity": "sha512-RbJ5/jmFcNNCcDV5o9eTnBLJ/HszWV0P73bc+Ff4nS/rJj+YaS6IGyiOL0VoBYX+l1Wrl3k63h/KrH+nhJ0XvQ==",
                     "resolved": "https://registry.npmjs.org/graceful-fs/-/graceful-fs-4.2.11.tgz",
                     "version": "4.2.11"
                 }
             },
             "dev": true,
-            "integrity": "sha512-l5sOdYBDunyf72HW8dF23rFtWq/7Zgvt/9ftMof71E/yUb1YLOBmTgA2K4vQthB3kotMrSj609txVE0dnr2fjA==",
+            "integrity": "sha512-C6uiGQJ+Gt4RyHXXYt+v9f+SN1v83x68URwgxNQ98cvH8kxiuywWGP4XeNZ1paOzZ63aY3cTciCEQJNFUljlLw==",
             "requires": {
                 "@types/eslint-scope": "^3.7.3",
-                "@types/estree": "^0.0.51",
-                "@webassemblyjs/ast": "1.11.1",
-                "@webassemblyjs/wasm-edit": "1.11.1",
-                "@webassemblyjs/wasm-parser": "1.11.1",
+                "@types/estree": "^1.0.0",
+                "@webassemblyjs/ast": "^1.11.5",
+                "@webassemblyjs/wasm-edit": "^1.11.5",
+                "@webassemblyjs/wasm-parser": "^1.11.5",
                 "acorn": "^8.7.1",
                 "acorn-import-assertions": "^1.7.6",
                 "browserslist": "^4.14.5",
                 "chrome-trace-event": "^1.0.2",
-                "enhanced-resolve": "^5.10.0",
-                "es-module-lexer": "^0.9.0",
+                "enhanced-resolve": "^5.14.0",
+                "es-module-lexer": "^1.2.1",
                 "eslint-scope": "5.1.1",
                 "events": "^3.2.0",
                 "glob-to-regexp": "^0.4.1",
                 "graceful-fs": "^4.2.9",
                 "json-parse-even-better-errors": "^2.3.1",
                 "loader-runner": "^4.2.0",
                 "mime-types": "^2.1.27",
                 "neo-async": "^2.6.2",
-                "schema-utils": "^3.1.0",
+                "schema-utils": "^3.1.2",
                 "tapable": "^2.1.1",
-                "terser-webpack-plugin": "^5.1.3",
+                "terser-webpack-plugin": "^5.3.7",
                 "watchpack": "^2.4.0",
                 "webpack-sources": "^3.2.3"
             },
-            "resolved": "https://registry.npmjs.org/webpack/-/webpack-5.76.0.tgz",
-            "version": "5.76.0"
+            "resolved": "https://registry.npmjs.org/webpack/-/webpack-5.82.1.tgz",
+            "version": "5.82.1"
         },
         "webpack-merge": {
             "dev": true,
             "integrity": "sha512-TUE1UGoTX2Cd42j3krGYqObZbOD+xF7u28WB7tfUordytSjbWTIjK/8V0amkBfTYN4/pB/GIDlJZZ657BGG19g==",
             "requires": {
                 "lodash": "^4.17.15"
             },
@@ -3013,14 +3046,23 @@
         },
         "webpack-sources": {
             "dev": true,
             "integrity": "sha512-/DyMEOrDgLKKIG0fmvtz+4dUX/3Ghozwgm6iPp8KRhvn+eQf9+Q7GWxVNMk3+uCPWfdXYC4ExGBckIXdFEfH1w==",
             "resolved": "https://registry.npmjs.org/webpack-sources/-/webpack-sources-3.2.3.tgz",
             "version": "3.2.3"
         },
+        "which": {
+            "dev": true,
+            "integrity": "sha512-BLI3Tl1TW3Pvl70l3yq3Y64i+awpwXqsGBYWkkqMtnbXgrMD+yj7rhW0kuEDxzJaYXGjEW5ogapKNMEKNMjibA==",
+            "requires": {
+                "isexe": "^2.0.0"
+            },
+            "resolved": "https://registry.npmjs.org/which/-/which-2.0.2.tgz",
+            "version": "2.0.2"
+        },
         "which-boxed-primitive": {
             "dev": true,
             "integrity": "sha512-bwZdv0AKLpplFY2KZRX6TvyuN7ojjr7lwkg6ml0roIy9YeuSr7JS372qlNW18UQYzgYK9ziGcerWqZOmEn9VNg==",
             "requires": {
                 "is-bigint": "^1.0.1",
                 "is-boolean-object": "^1.1.0",
                 "is-number-object": "^1.0.4",
```

### Comparing `blspy-2.0.0b3/js-bindings/package.json` & `blspy-2.0.1b1/js-bindings/package.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9930555555555556%*

 * *Differences: {"'devDependencies'": "{'@types/mocha': '^10.0.1', '@types/node': '^20.1.5', 'karma': '^6.4.2', "*

 * *                      "'karma-firefox-launcher': '^2.1.2', 'mime': '3.0.0', 'typescript': "*

 * *                      "'^5.0.4', 'webpack': '^5.82.1'}"}*

```diff
@@ -5,32 +5,32 @@
         "url": "https://github.com/antouhou"
     },
     "dependencies": {
         "binascii": "0.0.2"
     },
     "description": "The most advanced BLS library for JavaScript",
     "devDependencies": {
-        "@types/mocha": "^5.2.7",
-        "@types/node": "^11.15.18",
+        "@types/mocha": "^10.0.1",
+        "@types/node": "^20.1.5",
         "assert": "^2.0.0",
         "babel-polyfill": "^6.26.0",
         "buffer": "^6.0.3",
         "crypto-browserify": "^3.12.0",
-        "karma": "^6.3.4",
-        "karma-firefox-launcher": "^1.3.0",
+        "karma": "^6.4.2",
+        "karma-firefox-launcher": "^2.1.2",
         "karma-mocha": "^2.0.1",
         "karma-mocha-reporter": "^2.2.5",
         "karma-webpack": "^5.0.0",
-        "mime": "1.4.1",
+        "mime": "3.0.0",
         "mocha": "^10.2.0",
         "path-browserify": "^1.0.1",
         "process": "^0.11.10",
         "stream-browserify": "^3.0.0",
-        "typescript": "^3.6.5",
-        "webpack": "^5.39.0"
+        "typescript": "^5.0.4",
+        "webpack": "^5.82.1"
     },
     "directories": {
         "test": "tests"
     },
     "files": [
         "blsjs.js",
         "blsjs.wasm",
```

### Comparing `blspy-2.0.0b3/js-bindings/tests/PrivateKey.spec.js` & `blspy-2.0.1b1/js-bindings/tests/PrivateKey.spec.js`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b3/js-bindings/tests/PublicKey.spec.js` & `blspy-2.0.1b1/js-bindings/tests/PublicKey.spec.js`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b3/js-bindings/tests/Signature.spec.js` & `blspy-2.0.1b1/js-bindings/tests/Signature.spec.js`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b3/js-bindings/tests/karma.conf.js` & `blspy-2.0.1b1/js-bindings/tests/karma.conf.js`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b3/js-bindings/tests/test.js` & `blspy-2.0.1b1/js-bindings/tests/test.js`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b3/js-bindings/tests/typings.spec.ts` & `blspy-2.0.1b1/js-bindings/tests/typings.spec.ts`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b3/js-bindings/tests/yarn.lock` & `blspy-2.0.1b1/js-bindings/tests/yarn.lock`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b3/js-bindings/wrappers/G1ElementWrapper.cpp` & `blspy-2.0.1b1/js-bindings/wrappers/G1ElementWrapper.cpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b3/js-bindings/wrappers/G1ElementWrapper.h` & `blspy-2.0.1b1/js-bindings/wrappers/G1ElementWrapper.h`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b3/js-bindings/wrappers/G2ElementWrapper.cpp` & `blspy-2.0.1b1/js-bindings/wrappers/G2ElementWrapper.cpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b3/js-bindings/wrappers/G2ElementWrapper.h` & `blspy-2.0.1b1/js-bindings/wrappers/G2ElementWrapper.h`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b3/js-bindings/wrappers/JSWrapper.h` & `blspy-2.0.1b1/js-bindings/wrappers/JSWrapper.h`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b3/js-bindings/wrappers/PrivateKeyWrapper.cpp` & `blspy-2.0.1b1/js-bindings/wrappers/PrivateKeyWrapper.cpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b3/js-bindings/wrappers/PrivateKeyWrapper.h` & `blspy-2.0.1b1/js-bindings/wrappers/PrivateKeyWrapper.h`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b3/js-bindings/wrappers/SchemeMPLWrapper.cpp` & `blspy-2.0.1b1/js-bindings/wrappers/SchemeMPLWrapper.cpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b3/js-bindings/wrappers/SchemeMPLWrapper.h` & `blspy-2.0.1b1/js-bindings/wrappers/SchemeMPLWrapper.h`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b3/js-bindings/wrappers/UtilWrapper.cpp` & `blspy-2.0.1b1/js-bindings/wrappers/UtilWrapper.cpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b3/js-bindings/wrappers/UtilWrapper.h` & `blspy-2.0.1b1/js-bindings/wrappers/UtilWrapper.h`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b3/python-bindings/README.md` & `blspy-2.0.1b1/python-bindings/README.md`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b3/python-bindings/benchmark.py` & `blspy-2.0.1b1/python-bindings/benchmark.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b3/python-bindings/pythonbindings.cpp` & `blspy-2.0.1b1/python-bindings/pythonbindings.cpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b3/python-bindings/test.py` & `blspy-2.0.1b1/python-bindings/test.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b3/python-impl/README.md` & `blspy-2.0.1b1/python-impl/README.md`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b3/python-impl/bls12381.py` & `blspy-2.0.1b1/python-impl/bls12381.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b3/python-impl/ec.py` & `blspy-2.0.1b1/python-impl/ec.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b3/python-impl/fields.py` & `blspy-2.0.1b1/python-impl/fields.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b3/python-impl/hash_to_field.py` & `blspy-2.0.1b1/python-impl/hash_to_field.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b3/python-impl/hd_keys.py` & `blspy-2.0.1b1/python-impl/hd_keys.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b3/python-impl/hkdf.py` & `blspy-2.0.1b1/python-impl/hkdf.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b3/python-impl/impl-test.py` & `blspy-2.0.1b1/python-impl/impl-test.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b3/python-impl/op_swu_g2.py` & `blspy-2.0.1b1/python-impl/op_swu_g2.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b3/python-impl/pairing.py` & `blspy-2.0.1b1/python-impl/pairing.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b3/python-impl/private_key.py` & `blspy-2.0.1b1/python-impl/private_key.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b3/python-impl/schemes.py` & `blspy-2.0.1b1/python-impl/schemes.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b3/python-impl/util.py` & `blspy-2.0.1b1/python-impl/util.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b3/src/bls.cpp` & `blspy-2.0.1b1/src/bls.cpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b3/src/bls.hpp` & `blspy-2.0.1b1/src/bls.hpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b3/src/elements.cpp` & `blspy-2.0.1b1/src/elements.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -120,20 +120,17 @@
     G1Element ele;
     ele.p = *(blst_p1_generator());
     return ele;
 }
 
 bool G1Element::IsValid() const
 {
-    // Infinity no longer valid in Relic
-    // https://github.com/relic-toolkit/relic/commit/f3be2babb955cf9f82743e0ae5ef265d3da6c02b
-    // if (blst_p1_is_inf(&p) == 1)
-    //     return true;
-
-    // return blst_p1_on_curve((blst_p1*)&p);
+    // Infinity was considered a valid G1Element in older Relic versions
+    // on which this library was previously based.
+    // For historical compatibililty this behavior is maintained.
 
     if (blst_p1_is_inf(&p))
         return true;
 
     return blst_p1_in_g1(&p);
 }
 
@@ -151,16 +148,15 @@
 void G1Element::ToAffine(blst_p1_affine* output) const
 {
     blst_p1_to_affine(output, &p);
 }
 
 G1Element G1Element::Negate() const
 {
-    G1Element ans;
-    ans.FromNative(p);
+    G1Element ans = G1Element::FromNative(p);
     blst_p1_cneg(&(ans.p), true);
     return ans;
 }
 
 GTElement G1Element::Pair(const G2Element& b) const { return (*this) & b; }
 
 uint32_t G1Element::GetFingerprint() const
@@ -296,20 +292,17 @@
     G2Element ele;
     ele.q = (*blst_p2_generator());
     return ele;
 }
 
 bool G2Element::IsValid() const
 {
-    // Infinity no longer valid in Relic
-    // https://github.com/relic-toolkit/relic/commit/f3be2babb955cf9f82743e0ae5ef265d3da6c02b
-    // if (blst_p2_is_inf(&q) == 1)
-    //     return true;
-
-    // return blst_p2_on_curve((blst_p2*)&q);
+    // Infinity was considered a valid G2Element in older Relic versions
+    // on which this library was previously based.
+    // For historical compatibililty this behavior is maintained.
 
     if (blst_p2_is_inf(&q))
         return true;
 
     return blst_p2_in_g2(&q);
 }
 
@@ -327,16 +320,15 @@
 void G2Element::ToAffine(blst_p2_affine* output) const
 {
     blst_p2_to_affine(output, &q);
 }
 
 G2Element G2Element::Negate() const
 {
-    G2Element ans;
-    ans.FromNative(q);
+    G2Element ans = G2Element::FromNative(q);
     blst_p2_cneg(&(ans.q), true);
     return ans;
 }
 
 GTElement G2Element::Pair(const G1Element& a) const { return a & (*this); }
 
 std::vector<uint8_t> G2Element::Serialize() const
```

### Comparing `blspy-2.0.0b3/src/elements.hpp` & `blspy-2.0.1b1/src/elements.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 
 private:
     blst_p2 q;
 };
 
 class GTElement {
 public:
-    static const size_t SIZE = 576;
+    static const size_t SIZE = sizeof(blst_fp12);
 
     static GTElement FromBytes(Bytes bytes);
     static GTElement FromBytesUnchecked(Bytes bytes);
     static GTElement FromByteVector(const std::vector<uint8_t> &bytevec);
     static GTElement FromNative(const blst_fp12 *element);
     static GTElement FromAffine(const blst_p1_affine &element);
     static GTElement FromAffine(const blst_p2_affine &element);
```

### Comparing `blspy-2.0.0b3/src/hdkeys.hpp` & `blspy-2.0.1b1/src/hdkeys.hpp`

 * *Files 14% similar despite different names*

```diff
@@ -47,24 +47,19 @@
         const size_t infoLen = 0;
 
         // Required by the ietf spec to be at least 32 bytes
         if (seed.size() < 32) {
             throw std::invalid_argument("Seed size must be at least 32 bytes");
         }
 
-        // std::cout << "seed: "<< Util::HexStr(seed.begin(),seed.size()) <<
-        // std::endl;
-
         blst_scalar* skBn = Util::SecAlloc<blst_scalar>(1);
         blst_keygen_v3(skBn, seed.begin(), seed.size(), info, infoLen);
         uint8_t* skBytes = Util::SecAlloc<uint8_t>(32);
         blst_bendian_from_scalar(skBytes, skBn);
 
-        // std::cout << "skBytes: "<< Util::HexStr(skBytes,32) << std::endl;
-
         PrivateKey k = PrivateKey::FromBytes(Bytes(skBytes, 32));
 
         Util::SecFree(skBn);
         Util::SecFree(skBytes);
 
         return k;
     }
```

### Comparing `blspy-2.0.0b3/src/hkdf.hpp` & `blspy-2.0.1b1/src/hkdf.hpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b3/src/privatekey.cpp` & `blspy-2.0.1b1/src/privatekey.cpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b3/src/privatekey.hpp` & `blspy-2.0.1b1/src/privatekey.hpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b3/src/schemes.cpp` & `blspy-2.0.1b1/src/schemes.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -260,47 +260,14 @@
 
     blst_pairing_commit(ctx);
     auto ret = blst_pairing_finalverify(ctx, &gtsig);
     free(ctx);
     return ret;
 }
 
-// bool CoreMPL::NativeVerify(
-//     blst_p1* pubkeys,
-//     blst_p2* mappedHashes,
-//     size_t length)
-// {
-//     blst_fp12 target, candidate, tmpPairing;
-//     memcpy(&target, blst_fp12_one(), sizeof(blst_fp12));
-//     memcpy(&candidate, blst_fp12_one(), sizeof(blst_fp12));
-
-//     // prod e(pubkey[i], hash[i]) * e(-g1, aggSig)
-//     // Performs pubKeys.size() pairings, 250 at a time
-
-//     blst_p1_affine Ps[length];
-//     blst_p2_affine Qs[length];
-//     const blst_p1* ppoints[2] = {pubkeys, NULL};
-//     const blst_p2* pqoints[2] = {mappedHashes, NULL};
-
-//     blst_p1s_to_affine(Ps, ppoints, length);
-//     blst_p2s_to_affine(Qs, pqoints, length);
-//     for (size_t i = 0; i < length; i += 250) {
-//         size_t numPairings = std::min((length - i), (size_t)250);
-//         const blst_p1_affine* const pP = &(Ps[i]);
-//         const blst_p2_affine* const pQ = &(Qs[i]);
-//         blst_miller_loop_n(&tmpPairing, &pQ, &pP, numPairings);
-//         blst_fp12_mul(&candidate, &candidate, &tmpPairing);
-//     }
-//     // 1 =? prod e(pubkey[i], hash[i]) * e(-g1, aggSig)
-//     if (memcmp(&target, &candidate, sizeof(blst_fp12)) != 0) {
-//         return false;
-//     }
-//     return true;
-// }
-
 PrivateKey CoreMPL::DeriveChildSk(const PrivateKey& sk, uint32_t index)
 {
     return HDKeys::DeriveChildSk(sk, index);
 }
 
 PrivateKey CoreMPL::DeriveChildSkUnhardened(
     const PrivateKey& sk,
@@ -580,29 +547,14 @@
     return PopSchemeMPL::PopVerify(Bytes(pubkey), Bytes(proof));
 }
 
 bool PopSchemeMPL::PopVerify(const Bytes& pubkey, const Bytes& proof)
 {
     return PopSchemeMPL::PopVerify(
         G1Element::FromBytes(pubkey), G2Element::FromBytes(proof));
-
-    // const G2Element hashedPoint = G2Element::FromMessage(
-    //     pubkey,
-    //     (const uint8_t*)POP_CIPHERSUITE_ID.c_str(),
-    //     POP_CIPHERSUITE_ID.length());
-
-    // blst_p1 g1s[2];
-    // blst_p2 g2s[2];
-
-    // G1Element::Generator().Negate().ToNative(&(g1s[0]));
-    // G1Element::FromBytes(pubkey).ToNative(&(g1s[1]));
-    // G2Element::FromBytes(proof).ToNative(&(g2s[0]));
-    // hashedPoint.ToNative(&(g2s[1]));
-
-    // return CoreMPL::NativeVerify(g1s, g2s, 2);
 }
 
 bool PopSchemeMPL::FastAggregateVerify(
     const vector<G1Element>& pubkeys,
     const vector<uint8_t>& message,
     const G2Element& signature)
 {
```

### Comparing `blspy-2.0.0b3/src/schemes.hpp` & `blspy-2.0.1b1/src/schemes.hpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b3/src/test-bench.cpp` & `blspy-2.0.1b1/src/test-bench.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,14 @@
 // limitations under the License.
 
 #include <chrono>
 
 #include "bls.hpp"
 #include "test-utils.hpp"
 
-using std::cout;
-using std::endl;
 using std::string;
 using std::vector;
 
 using namespace bls;
 
 std::vector<uint8_t> wjbgetRandomSeed()
 {
```

### Comparing `blspy-2.0.0b3/src/test-utils.hpp` & `blspy-2.0.1b1/src/test-utils.hpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.0b3/src/test.cpp` & `blspy-2.0.1b1/src/test.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,14 @@
 
 #include <catch2/catch_session.hpp>
 #include <catch2/catch_test_macros.hpp>
 #include <thread>
 
 #include "bls.hpp"
 #include "test-utils.hpp"
-using std::cout;
-using std::endl;
 using std::string;
 using std::vector;
 
 using namespace bls;
 
 void TestHKDF(
     string ikm_hex,
@@ -108,14 +106,15 @@
         REQUIRE(pk1 != pk2);
         REQUIRE(pk1 != pk3);
         REQUIRE(pk2 == pk3);
     }
     SECTION("(De)Serialization")
     {
         PrivateKey pk1 = PrivateKey::FromByteVector(getRandomSeed(), true);
+        REQUIRE_THROWS_AS(pk1.Serialize(nullptr), std::runtime_error);
         pk1.Serialize(buffer);
         REQUIRE(
             memcmp(
                 buffer, pk1.Serialize().data(), PrivateKey::PRIVATE_KEY_SIZE) ==
             0);
         PrivateKey pk2 = PrivateKey::FromBytes(
             Bytes(buffer, PrivateKey::PRIVATE_KEY_SIZE), true);
@@ -398,24 +397,28 @@
         PrivateKey sk2 = BasicSchemeMPL().KeyGen(seed2);
         G1Element pk2 = sk2.GetG1Element();
         G2Element sig2 = BasicSchemeMPL().Sign(sk2, message2);
 
         REQUIRE(pk1.GetFingerprint() == 0xb40dd58a);
         REQUIRE(pk2.GetFingerprint() == 0xb839add1);
 
+        std::stringstream out;
+        out << sig1;  // operator<< tests Serialize()
         REQUIRE(
-            Util::HexStr(sig1.Serialize()) ==
+            out.str() ==
             "b8faa6d6a3881c9fdbad803b170d70ca5cbf1e6ba5a586262df368c75acd1d1f"
             "fa3ab6ee21c71f844494659878f5eb230c958dd576b08b8564aad2ee0992e85a"
             "1e565f299cd53a285de729937f70dc176a1f01432129bb2b94d3d5031f8065a1");
         REQUIRE(
             Util::HexStr(sk1.Serialize()) ==
             "4a353be3dac091a0a7e640620372f5e1e2e4401717c1e79cac6ffba8f6905604");
+        out.str("");
+        out << pk1;
         REQUIRE(
-            Util::HexStr(pk1.Serialize()) ==
+            out.str() ==
             "85695fcbc06cc4c4c9451f4dce21cbf8de3e5a13bf48f44cdbb18e2038ba7b8bb1"
             "632d7911e"
             "f1e2e08749bddbf165352");
 
         REQUIRE(
             Util::HexStr(sig2.Serialize()) ==
             "a9c4d3e689b82c7ec7e838dac2380cb014f9a08f6cd6ba044c263746e39a8f7a60"
@@ -1337,14 +1340,17 @@
 
     SECTION("Invalid G1 points should not succeed")
     {
         string badPointHex =
             "8d5d0fb73b9c92df4eab4216e48c3e358578b4cc30f82c268bd6fef3bd34b55862"
             "8daf1afef798d4c3b0fcd8b28c8973";
 
+        REQUIRE_THROWS_AS(
+            G1Element::FromBytesUnchecked(vector<uint8_t>(100, 0x05)),
+            std::invalid_argument);
         // FromBytes throws
         REQUIRE_THROWS(
             G1Element::FromBytes(Bytes(Util::HexToBytes(badPointHex))));
 
         // FromBytesUnchecked does not throw
         G1Element bad_pk =
             G1Element::FromBytesUnchecked(Bytes(Util::HexToBytes(badPointHex)));
@@ -1374,14 +1380,58 @@
         G2Element point = G2Element::FromNative(point_native);
         REQUIRE(point.IsValid() == false);
         REQUIRE_THROWS(point.CheckValid());
 
         auto badSer = point.Serialize();
 
         REQUIRE_THROWS(G2Element::FromByteVector(badSer));
+
+        REQUIRE_THROWS_AS(
+            G2Element::FromBytesUnchecked(vector<uint8_t>(100, 0x04)),
+            std::invalid_argument);
+    }
+}
+
+TEST_CASE("Element operations")
+{
+    SECTION("G1Element")
+    {
+        auto pk1 =
+            PrivateKey::FromByteVector(getRandomSeed(), true).GetG1Element();
+        auto pk2 =
+            PrivateKey::FromByteVector(getRandomSeed(), true).GetG1Element();
+        auto res = pk1 + G1Element();
+        REQUIRE(res == pk1);
+        REQUIRE(pk1 + G1Element() == pk1);
+
+        REQUIRE(pk1 + pk2 == pk2 + pk1);
+        pk1 += pk1.Negate();
+        REQUIRE(pk1 == G1Element());
+
+        auto g = G1Element::Generator();
+        REQUIRE(g.IsValid() == true);
+        // assert g.is_on_curve()
+        // assert 2 * g == g + g
+        // assert (3 * g).is_on_curve()
+        // assert 3 * g == g + g + g
+    }
+    SECTION("G2Element")
+    {
+        auto sig1 =
+            PrivateKey::FromByteVector(getRandomSeed(), true).GetG2Element();
+        auto sig2 =
+            PrivateKey::FromByteVector(getRandomSeed(), true).GetG2Element();
+        auto res = sig1 + G2Element();
+        REQUIRE(res == sig1);
+        REQUIRE(sig1 + G2Element() == sig1);
+
+        REQUIRE(sig1 + sig2 == sig2 + sig1);
+        sig1 += sig1.Negate();
+        REQUIRE(sig1 == G2Element());
+        REQUIRE(G2Element::Generator().IsValid());
     }
 }
 
 TEST_CASE("GTElement")
 {
     SECTION("GTElement serialization")
     {
```

### Comparing `blspy-2.0.0b3/src/util.hpp` & `blspy-2.0.1b1/src/util.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -66,38 +66,36 @@
 
 static void md_hmac(uint8_t *mac, const uint8_t *in, int in_len, const uint8_t *key,
     int key_len) {
   #define block_size 64
   #define RLC_MD_LEN 32
     uint8_t opad[block_size + RLC_MD_LEN];
     uint8_t *ipad = (uint8_t *)malloc(block_size + in_len);
-        uint8_t _key[block_size];
+    uint8_t _key[block_size];
 
-/*    if (ipad == NULL) {
-        RLC_THROW(ERR_NO_MEMORY);
-                return;
+    if (ipad == NULL)
+        throw std::runtime_error("out of memory");
+
+    if (key_len > block_size) {
+        Hash256(_key, key, key_len);
+        key = _key;
+        key_len = RLC_MD_LEN;
+    }
+
+    memcpy(_key, key, key_len);
+    memset(_key + key_len, 0, block_size - key_len);
+    key = _key;
+
+    for (int i = 0; i < block_size; i++) {
+        opad[i] = 0x5C ^ key[i];
+        ipad[i] = 0x36 ^ key[i];
     }
-*/
-        if (key_len > block_size) {
-                Hash256(_key, key, key_len);
-                key = _key;
-                key_len = RLC_MD_LEN;
-        }
-        if (key_len <= block_size) {
-                memcpy(_key, key, key_len);
-                memset(_key + key_len, 0, block_size - key_len);
-                key = _key;
-        }
-        for (int i = 0; i < block_size; i++) {
-                opad[i] = 0x5C ^ key[i];
-                ipad[i] = 0x36 ^ key[i];
-        }
-        memcpy(ipad + block_size, in, in_len);
-        Hash256(opad + block_size, ipad, block_size + in_len);
-        Hash256(mac, opad, block_size + RLC_MD_LEN);
+    memcpy(ipad + block_size, in, in_len);
+    Hash256(opad + block_size, ipad, block_size + in_len);
+    Hash256(mac, opad, block_size + RLC_MD_LEN);
 
     free(ipad);
 }
 
     static std::string HexStr(const uint8_t* data, size_t len) {
         std::stringstream s;
         s << std::hex;
```

