# Comparing `tmp/blspy-2.0.1.tar.gz` & `tmp/blspy-2.0.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blspy-2.0.1.tar", last modified: Thu Jun 22 21:31:57 2023, max compression
+gzip compressed data, was "blspy-2.0.1b1.tar", last modified: Thu Jun 22 19:07:45 2023, max compression
```

## Comparing `blspy-2.0.1.tar` & `blspy-2.0.1b1.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:31:57.899464 blspy-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-22 21:31:44.000000 blspy-2.0.1/.clang-format
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-22 21:31:44.000000 blspy-2.0.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:31:57.887463 blspy-2.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:31:57.891463 blspy-2.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-22 21:31:44.000000 blspy-2.0.1/.github/workflows/build-blst-nightly.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-06-22 21:31:44.000000 blspy-2.0.1/.github/workflows/build-test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-06-22 21:31:44.000000 blspy-2.0.1/.github/workflows/build-wheels.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-06-22 21:31:44.000000 blspy-2.0.1/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-22 21:31:44.000000 blspy-2.0.1/.github/workflows/js-bindings.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-22 21:31:44.000000 blspy-2.0.1/.github/workflows/stale-issue.yml
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-22 21:31:44.000000 blspy-2.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-22 21:31:44.000000 blspy-2.0.1/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-06-22 21:31:44.000000 blspy-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-22 21:31:44.000000 blspy-2.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-06-22 21:31:57.899464 blspy-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11118 2023-06-22 21:31:44.000000 blspy-2.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:31:57.891463 blspy-2.0.1/blspy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-06-22 21:31:57.000000 blspy-2.0.1/blspy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-06-22 21:31:57.000000 blspy-2.0.1/blspy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 21:31:57.000000 blspy-2.0.1/blspy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 21:31:57.000000 blspy-2.0.1/blspy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-22 21:31:57.000000 blspy-2.0.1/blspy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-22 21:31:57.000000 blspy-2.0.1/blspy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:31:57.891463 blspy-2.0.1/cmake_modules/
--rw-r--r--   0 runner    (1001) docker     (123)     9884 2023-06-22 21:31:44.000000 blspy-2.0.1/cmake_modules/Findsodium.cmake
--rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-06-22 21:31:44.000000 blspy-2.0.1/emsdk_build.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:31:57.891463 blspy-2.0.1/js-bindings/
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-22 21:31:44.000000 blspy-2.0.1/js-bindings/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-06-22 21:31:44.000000 blspy-2.0.1/js-bindings/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-22 21:31:44.000000 blspy-2.0.1/js-bindings/blsjs.d.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-22 21:31:44.000000 blspy-2.0.1/js-bindings/helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-22 21:31:44.000000 blspy-2.0.1/js-bindings/helpers.h
--rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-06-22 21:31:44.000000 blspy-2.0.1/js-bindings/jsbindings.cpp
--rw-r--r--   0 runner    (1001) docker     (123)   129248 2023-06-22 21:31:44.000000 blspy-2.0.1/js-bindings/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-06-22 21:31:44.000000 blspy-2.0.1/js-bindings/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:31:57.891463 blspy-2.0.1/js-bindings/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-06-22 21:31:44.000000 blspy-2.0.1/js-bindings/tests/PrivateKey.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-06-22 21:31:44.000000 blspy-2.0.1/js-bindings/tests/PublicKey.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-06-22 21:31:44.000000 blspy-2.0.1/js-bindings/tests/Signature.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-22 21:31:44.000000 blspy-2.0.1/js-bindings/tests/karma.conf.js
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-22 21:31:44.000000 blspy-2.0.1/js-bindings/tests/karma.test.js
--rw-r--r--   0 runner    (1001) docker     (123)    19006 2023-06-22 21:31:44.000000 blspy-2.0.1/js-bindings/tests/test.js
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-06-22 21:31:44.000000 blspy-2.0.1/js-bindings/tests/typings.spec.ts
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-22 21:31:44.000000 blspy-2.0.1/js-bindings/tests/webpack.config.js
--rw-r--r--   0 runner    (1001) docker     (123)    13186 2023-06-22 21:31:44.000000 blspy-2.0.1/js-bindings/tests/yarn.lock
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:31:57.895464 blspy-2.0.1/js-bindings/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-06-22 21:31:44.000000 blspy-2.0.1/js-bindings/wrappers/G1ElementWrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-22 21:31:44.000000 blspy-2.0.1/js-bindings/wrappers/G1ElementWrapper.h
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-22 21:31:44.000000 blspy-2.0.1/js-bindings/wrappers/G2ElementWrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-06-22 21:31:44.000000 blspy-2.0.1/js-bindings/wrappers/G2ElementWrapper.h
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-22 21:31:44.000000 blspy-2.0.1/js-bindings/wrappers/JSWrapper.h
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-06-22 21:31:44.000000 blspy-2.0.1/js-bindings/wrappers/PrivateKeyWrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-06-22 21:31:44.000000 blspy-2.0.1/js-bindings/wrappers/PrivateKeyWrapper.h
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-22 21:31:44.000000 blspy-2.0.1/js-bindings/wrappers/SchemeMPLWrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-06-22 21:31:44.000000 blspy-2.0.1/js-bindings/wrappers/SchemeMPLWrapper.h
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-22 21:31:44.000000 blspy-2.0.1/js-bindings/wrappers/UtilWrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-22 21:31:44.000000 blspy-2.0.1/js-bindings/wrappers/UtilWrapper.h
--rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-06-22 21:31:44.000000 blspy-2.0.1/js_build.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      272 2023-06-22 21:31:44.000000 blspy-2.0.1/js_test.sh
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-22 21:31:44.000000 blspy-2.0.1/lgtm.yml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-22 21:31:44.000000 blspy-2.0.1/mypi.ini
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-22 21:31:44.000000 blspy-2.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:31:57.895464 blspy-2.0.1/python-bindings/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-22 21:31:44.000000 blspy-2.0.1/python-bindings/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-06-22 21:31:44.000000 blspy-2.0.1/python-bindings/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-22 21:31:44.000000 blspy-2.0.1/python-bindings/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)    29858 2023-06-22 21:31:44.000000 blspy-2.0.1/python-bindings/pythonbindings.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    17701 2023-06-22 21:31:44.000000 blspy-2.0.1/python-bindings/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:31:57.895464 blspy-2.0.1/python-impl/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-22 21:31:44.000000 blspy-2.0.1/python-impl/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-06-22 21:31:44.000000 blspy-2.0.1/python-impl/bls12381.py
--rw-r--r--   0 runner    (1001) docker     (123)    17476 2023-06-22 21:31:44.000000 blspy-2.0.1/python-impl/ec.py
--rw-r--r--   0 runner    (1001) docker     (123)    21950 2023-06-22 21:31:44.000000 blspy-2.0.1/python-impl/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-06-22 21:31:44.000000 blspy-2.0.1/python-impl/hash_to_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-06-22 21:31:44.000000 blspy-2.0.1/python-impl/hd_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-22 21:31:44.000000 blspy-2.0.1/python-impl/hkdf.py
--rw-r--r--   0 runner    (1001) docker     (123)    26234 2023-06-22 21:31:44.000000 blspy-2.0.1/python-impl/impl-test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7389 2023-06-22 21:31:44.000000 blspy-2.0.1/python-impl/op_swu_g2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-06-22 21:31:44.000000 blspy-2.0.1/python-impl/pairing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-06-22 21:31:44.000000 blspy-2.0.1/python-impl/private_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-06-22 21:31:44.000000 blspy-2.0.1/python-impl/schemes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-22 21:31:44.000000 blspy-2.0.1/python-impl/util.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 21:31:57.899464 blspy-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-06-22 21:31:44.000000 blspy-2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:31:57.899464 blspy-2.0.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-22 21:31:44.000000 blspy-2.0.1/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-22 21:31:44.000000 blspy-2.0.1/src/bls.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-22 21:31:44.000000 blspy-2.0.1/src/bls.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11518 2023-06-22 21:31:44.000000 blspy-2.0.1/src/elements.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-06-22 21:31:44.000000 blspy-2.0.1/src/elements.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6310 2023-06-22 21:31:44.000000 blspy-2.0.1/src/hdkeys.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-06-22 21:31:44.000000 blspy-2.0.1/src/hkdf.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-06-22 21:31:44.000000 blspy-2.0.1/src/privatekey.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-06-22 21:31:44.000000 blspy-2.0.1/src/privatekey.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    17747 2023-06-22 21:31:44.000000 blspy-2.0.1/src/schemes.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7176 2023-06-22 21:31:44.000000 blspy-2.0.1/src/schemes.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-06-22 21:31:44.000000 blspy-2.0.1/src/test-bench.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-22 21:31:44.000000 blspy-2.0.1/src/test-utils.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    58076 2023-06-22 21:31:44.000000 blspy-2.0.1/src/test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-06-22 21:31:44.000000 blspy-2.0.1/src/util.hpp
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

### Comparing `blspy-2.0.1/.github/workflows/build-blst-nightly.yml` & `blspy-2.0.1b1/.github/workflows/build-blst-nightly.yml`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/.github/workflows/build-test.yaml` & `blspy-2.0.1b1/.github/workflows/build-test.yaml`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/.github/workflows/build-wheels.yml` & `blspy-2.0.1b1/.github/workflows/build-wheels.yml`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/.github/workflows/codeql.yml` & `blspy-2.0.1b1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/.github/workflows/js-bindings.yml` & `blspy-2.0.1b1/.github/workflows/js-bindings.yml`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/.github/workflows/stale-issue.yml` & `blspy-2.0.1b1/.github/workflows/stale-issue.yml`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/CMakeLists.txt` & `blspy-2.0.1b1/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/LICENSE` & `blspy-2.0.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/PKG-INFO` & `blspy-2.0.1b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blspy
-Version: 2.0.1
+Version: 2.0.1b1
 Summary: BLS signatures in c++ (python bindings)
 Home-page: https://github.com/Chia-Network/bls-signatures
 Author: Mariano Sorgente
 Author-email: mariano@chia.net
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `blspy-2.0.1/README.md` & `blspy-2.0.1b1/README.md`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/blspy.egg-info/PKG-INFO` & `blspy-2.0.1b1/blspy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blspy
-Version: 2.0.1
+Version: 2.0.1b1
 Summary: BLS signatures in c++ (python bindings)
 Home-page: https://github.com/Chia-Network/bls-signatures
 Author: Mariano Sorgente
 Author-email: mariano@chia.net
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `blspy-2.0.1/blspy.egg-info/SOURCES.txt` & `blspy-2.0.1b1/blspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/cmake_modules/Findsodium.cmake` & `blspy-2.0.1b1/cmake_modules/Findsodium.cmake`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/js-bindings/CMakeLists.txt` & `blspy-2.0.1b1/js-bindings/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/js-bindings/README.md` & `blspy-2.0.1b1/js-bindings/README.md`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/js-bindings/blsjs.d.ts` & `blspy-2.0.1b1/js-bindings/blsjs.d.ts`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/js-bindings/helpers.cpp` & `blspy-2.0.1b1/js-bindings/helpers.cpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/js-bindings/helpers.h` & `blspy-2.0.1b1/js-bindings/helpers.h`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/js-bindings/jsbindings.cpp` & `blspy-2.0.1b1/js-bindings/jsbindings.cpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/js-bindings/package-lock.json` & `blspy-2.0.1b1/js-bindings/package-lock.json`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/js-bindings/package.json` & `blspy-2.0.1b1/js-bindings/package.json`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/js-bindings/tests/PrivateKey.spec.js` & `blspy-2.0.1b1/js-bindings/tests/PrivateKey.spec.js`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/js-bindings/tests/PublicKey.spec.js` & `blspy-2.0.1b1/js-bindings/tests/PublicKey.spec.js`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/js-bindings/tests/Signature.spec.js` & `blspy-2.0.1b1/js-bindings/tests/Signature.spec.js`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/js-bindings/tests/karma.conf.js` & `blspy-2.0.1b1/js-bindings/tests/karma.conf.js`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/js-bindings/tests/test.js` & `blspy-2.0.1b1/js-bindings/tests/test.js`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/js-bindings/tests/typings.spec.ts` & `blspy-2.0.1b1/js-bindings/tests/typings.spec.ts`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/js-bindings/tests/yarn.lock` & `blspy-2.0.1b1/js-bindings/tests/yarn.lock`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/js-bindings/wrappers/G1ElementWrapper.cpp` & `blspy-2.0.1b1/js-bindings/wrappers/G1ElementWrapper.cpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/js-bindings/wrappers/G1ElementWrapper.h` & `blspy-2.0.1b1/js-bindings/wrappers/G1ElementWrapper.h`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/js-bindings/wrappers/G2ElementWrapper.cpp` & `blspy-2.0.1b1/js-bindings/wrappers/G2ElementWrapper.cpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/js-bindings/wrappers/G2ElementWrapper.h` & `blspy-2.0.1b1/js-bindings/wrappers/G2ElementWrapper.h`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/js-bindings/wrappers/JSWrapper.h` & `blspy-2.0.1b1/js-bindings/wrappers/JSWrapper.h`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/js-bindings/wrappers/PrivateKeyWrapper.cpp` & `blspy-2.0.1b1/js-bindings/wrappers/PrivateKeyWrapper.cpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/js-bindings/wrappers/PrivateKeyWrapper.h` & `blspy-2.0.1b1/js-bindings/wrappers/PrivateKeyWrapper.h`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/js-bindings/wrappers/SchemeMPLWrapper.cpp` & `blspy-2.0.1b1/js-bindings/wrappers/SchemeMPLWrapper.cpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/js-bindings/wrappers/SchemeMPLWrapper.h` & `blspy-2.0.1b1/js-bindings/wrappers/SchemeMPLWrapper.h`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/js-bindings/wrappers/UtilWrapper.cpp` & `blspy-2.0.1b1/js-bindings/wrappers/UtilWrapper.cpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/js-bindings/wrappers/UtilWrapper.h` & `blspy-2.0.1b1/js-bindings/wrappers/UtilWrapper.h`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/python-bindings/README.md` & `blspy-2.0.1b1/python-bindings/README.md`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/python-bindings/benchmark.py` & `blspy-2.0.1b1/python-bindings/benchmark.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/python-bindings/pythonbindings.cpp` & `blspy-2.0.1b1/python-bindings/pythonbindings.cpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/python-bindings/test.py` & `blspy-2.0.1b1/python-bindings/test.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/python-impl/README.md` & `blspy-2.0.1b1/python-impl/README.md`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/python-impl/bls12381.py` & `blspy-2.0.1b1/python-impl/bls12381.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/python-impl/ec.py` & `blspy-2.0.1b1/python-impl/ec.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/python-impl/fields.py` & `blspy-2.0.1b1/python-impl/fields.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/python-impl/hash_to_field.py` & `blspy-2.0.1b1/python-impl/hash_to_field.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/python-impl/hd_keys.py` & `blspy-2.0.1b1/python-impl/hd_keys.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/python-impl/hkdf.py` & `blspy-2.0.1b1/python-impl/hkdf.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/python-impl/impl-test.py` & `blspy-2.0.1b1/python-impl/impl-test.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/python-impl/op_swu_g2.py` & `blspy-2.0.1b1/python-impl/op_swu_g2.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/python-impl/pairing.py` & `blspy-2.0.1b1/python-impl/pairing.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/python-impl/private_key.py` & `blspy-2.0.1b1/python-impl/private_key.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/python-impl/schemes.py` & `blspy-2.0.1b1/python-impl/schemes.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/python-impl/util.py` & `blspy-2.0.1b1/python-impl/util.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/setup.py` & `blspy-2.0.1b1/setup.py`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/src/CMakeLists.txt` & `blspy-2.0.1b1/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/src/bls.cpp` & `blspy-2.0.1b1/src/bls.cpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/src/bls.hpp` & `blspy-2.0.1b1/src/bls.hpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/src/elements.cpp` & `blspy-2.0.1b1/src/elements.cpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/src/elements.hpp` & `blspy-2.0.1b1/src/elements.hpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/src/hdkeys.hpp` & `blspy-2.0.1b1/src/hdkeys.hpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/src/hkdf.hpp` & `blspy-2.0.1b1/src/hkdf.hpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/src/privatekey.cpp` & `blspy-2.0.1b1/src/privatekey.cpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/src/privatekey.hpp` & `blspy-2.0.1b1/src/privatekey.hpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/src/schemes.cpp` & `blspy-2.0.1b1/src/schemes.cpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/src/schemes.hpp` & `blspy-2.0.1b1/src/schemes.hpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/src/test-bench.cpp` & `blspy-2.0.1b1/src/test-bench.cpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/src/test-utils.hpp` & `blspy-2.0.1b1/src/test-utils.hpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/src/test.cpp` & `blspy-2.0.1b1/src/test.cpp`

 * *Files identical despite different names*

### Comparing `blspy-2.0.1/src/util.hpp` & `blspy-2.0.1b1/src/util.hpp`

 * *Files identical despite different names*

