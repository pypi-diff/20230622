# Comparing `tmp/pyblock3-0.2.7.tar.gz` & `tmp/pyblock3-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyblock3-0.2.7.tar", last modified: Wed Jun 14 11:05:54 2023, max compression
+gzip compressed data, was "pyblock3-0.2.8.tar", last modified: Thu Jun 22 21:12:17 2023, max compression
```

## Comparing `pyblock3-0.2.7.tar` & `pyblock3-0.2.8.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:54.825503 pyblock3-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)    10859 2023-06-14 11:05:36.000000 pyblock3-0.2.7/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-14 11:05:36.000000 pyblock3-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-14 11:05:36.000000 pyblock3-0.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7294 2023-06-14 11:05:54.821503 pyblock3-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-06-14 11:05:36.000000 pyblock3-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:54.805503 pyblock3-0.2.7/pyblock3/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:54.809503 pyblock3-0.2.7/pyblock3/algebra/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:54.813503 pyblock3-0.2.7/pyblock3/algebra/ad/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/ad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    94198 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/ad/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    41261 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/ad/fermion.py
--rw-r--r--   0 runner    (1001) docker     (123)    18791 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/ad/fermion_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    58861 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/ad/flat.py
--rw-r--r--   0 runner    (1001) docker     (123)    25405 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/ad/flat_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)    24467 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/ad/mps.py
--rw-r--r--   0 runner    (1001) docker     (123)    87649 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     6539 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/einsum.py
--rw-r--r--   0 runner    (1001) docker     (123)    82436 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/fermion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/fermion_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)    33077 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/fermion_large.py
--rw-r--r--   0 runner    (1001) docker     (123)    18829 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/fermion_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/fermion_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     8371 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/fermion_symmetry.py
--rw-r--r--   0 runner    (1001) docker     (123)    58423 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/flat.py
--rw-r--r--   0 runner    (1001) docker     (123)    11178 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/flat_functor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:54.813503 pyblock3-0.2.7/pyblock3/algebra/impl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24602 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/impl/flat.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/integrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8113 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/linalg.py
--rw-r--r--   0 runner    (1001) docker     (123)    23715 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/mpe.py
--rw-r--r--   0 runner    (1001) docker     (123)    28783 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/mps.py
--rw-r--r--   0 runner    (1001) docker     (123)     8967 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/symmetry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:54.813503 pyblock3-0.2.7/pyblock3/algebra/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/tests/test_boson_cpp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7888 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/tests/test_boson_python.py
--rw-r--r--   0 runner    (1001) docker     (123)     7609 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/tests/test_fermion_cpp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7498 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/tests/test_fermion_large.py
--rw-r--r--   0 runner    (1001) docker     (123)    10548 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/tests/test_fermion_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     8829 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/tests/test_fermion_python.py
--rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/tests/test_symmetry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:54.813503 pyblock3-0.2.7/pyblock3/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7554 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algorithms/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7824 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algorithms/dmrg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algorithms/green.py
--rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algorithms/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algorithms/tddmrg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:54.817503 pyblock3-0.2.7/pyblock3/algorithms/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algorithms/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algorithms/tests/test_dmrg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algorithms/tests/test_ghf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algorithms/tests/test_sa.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algorithms/tests/test_soc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:54.817503 pyblock3-0.2.7/pyblock3/block2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/block2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11751 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/block2/hamil.py
--rw-r--r--   0 runner    (1001) docker     (123)    23824 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/block2/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    25632 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/fcidump.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:54.817503 pyblock3-0.2.7/pyblock3/gaussian/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/gaussian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45689 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/gaussian/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    16903 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/hamiltonian.py
--rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/heisenberg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:54.817503 pyblock3-0.2.7/pyblock3/symbolic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/symbolic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11748 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/symbolic/expr.py
--rw-r--r--   0 runner    (1001) docker     (123)    37662 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/symbolic/symbolic.py
--rw-r--r--   0 runner    (1001) docker     (123)    22316 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/symbolic/symbolic_mpo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:54.809503 pyblock3-0.2.7/pyblock3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7294 2023-06-14 11:05:54.000000 pyblock3-0.2.7/pyblock3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-06-14 11:05:54.000000 pyblock3-0.2.7/pyblock3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 11:05:54.000000 pyblock3-0.2.7/pyblock3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-14 11:05:54.000000 pyblock3-0.2.7/pyblock3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-14 11:05:54.000000 pyblock3-0.2.7/pyblock3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 11:05:54.825503 pyblock3-0.2.7/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3446 2023-06-14 11:05:36.000000 pyblock3-0.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:54.821503 pyblock3-0.2.7/src/
--rw-r--r--   0 runner    (1001) docker     (123)     8996 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/bond_info.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/bond_info.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/bond_info_tmpl.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10314 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/fermion_symmetry.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    35673 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/flat_fermion.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/flat_fermion.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/flat_fermion_tmpl.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    26561 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/flat_functor.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/flat_functor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/flat_functor_tmpl.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    74291 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/flat_sparse.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11959 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/flat_sparse.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10372 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/flat_sparse_tmpl.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:54.821503 pyblock3-0.2.7/src/gpu/
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/gpu/flat_fermion.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/gpu/flat_fermion_tmpl.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    39837 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/hamiltonian.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/hamiltonian.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    42218 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/hamiltonian_ptree.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/hamiltonian_ptree.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    59786 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/main.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/max_flow.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    36058 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/qc_expr.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    23892 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/qc_hamiltonian.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/qc_hamiltonian.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    26524 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/qc_mpo.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10579 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/qc_symbolic.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/symmetry_tmpl.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/sz.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7033 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/tensor.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/tensor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/tensor_einsum.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/tensor_einsum.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7495 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/tensor_impl.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    30167 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/tensor_impl.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:12:17.747842 pyblock3-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    10895 2023-06-22 21:12:01.000000 pyblock3-0.2.8/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-22 21:12:01.000000 pyblock3-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-22 21:12:01.000000 pyblock3-0.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7294 2023-06-22 21:12:17.743842 pyblock3-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-06-22 21:12:01.000000 pyblock3-0.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:12:17.731842 pyblock3-0.2.8/pyblock3/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:12:17.735842 pyblock3-0.2.8/pyblock3/algebra/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/algebra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:12:17.735842 pyblock3-0.2.8/pyblock3/algebra/ad/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/algebra/ad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94198 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/algebra/ad/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41261 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/algebra/ad/fermion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18791 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/algebra/ad/fermion_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58861 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/algebra/ad/flat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25405 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/algebra/ad/flat_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24467 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/algebra/ad/mps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87649 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/algebra/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6539 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/algebra/einsum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82436 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/algebra/fermion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/algebra/fermion_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33077 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/algebra/fermion_large.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18829 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/algebra/fermion_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/algebra/fermion_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8371 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/algebra/fermion_symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58423 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/algebra/flat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11178 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/algebra/flat_functor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/algebra/funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:12:17.735842 pyblock3-0.2.8/pyblock3/algebra/impl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/algebra/impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24602 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/algebra/impl/flat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/algebra/integrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8113 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/algebra/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23715 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/algebra/mpe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28783 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/algebra/mps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8967 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/algebra/symmetry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:12:17.735842 pyblock3-0.2.8/pyblock3/algebra/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/algebra/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/algebra/tests/test_boson_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7888 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/algebra/tests/test_boson_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7609 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/algebra/tests/test_fermion_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7498 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/algebra/tests/test_fermion_large.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10548 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/algebra/tests/test_fermion_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8829 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/algebra/tests/test_fermion_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/algebra/tests/test_symmetry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:12:17.739842 pyblock3-0.2.8/pyblock3/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7554 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/algorithms/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7824 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/algorithms/dmrg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/algorithms/green.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/algorithms/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/algorithms/tddmrg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:12:17.739842 pyblock3-0.2.8/pyblock3/algorithms/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/algorithms/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/algorithms/tests/test_dmrg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/algorithms/tests/test_ghf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/algorithms/tests/test_sa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/algorithms/tests/test_soc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:12:17.739842 pyblock3-0.2.8/pyblock3/block2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/block2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11751 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/block2/hamil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23824 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/block2/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25632 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/fcidump.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:12:17.739842 pyblock3-0.2.8/pyblock3/gaussian/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/gaussian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45689 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/gaussian/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16903 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/hamiltonian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/heisenberg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:12:17.739842 pyblock3-0.2.8/pyblock3/symbolic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/symbolic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11748 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/symbolic/expr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37662 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/symbolic/symbolic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22316 2023-06-22 21:12:01.000000 pyblock3-0.2.8/pyblock3/symbolic/symbolic_mpo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:12:17.731842 pyblock3-0.2.8/pyblock3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7294 2023-06-22 21:12:17.000000 pyblock3-0.2.8/pyblock3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-06-22 21:12:17.000000 pyblock3-0.2.8/pyblock3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 21:12:17.000000 pyblock3-0.2.8/pyblock3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-22 21:12:17.000000 pyblock3-0.2.8/pyblock3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-22 21:12:17.000000 pyblock3-0.2.8/pyblock3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 21:12:17.747842 pyblock3-0.2.8/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3446 2023-06-22 21:12:02.000000 pyblock3-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:12:17.743842 pyblock3-0.2.8/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     8996 2023-06-22 21:12:01.000000 pyblock3-0.2.8/src/bond_info.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-06-22 21:12:01.000000 pyblock3-0.2.8/src/bond_info.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-22 21:12:01.000000 pyblock3-0.2.8/src/bond_info_tmpl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10314 2023-06-22 21:12:01.000000 pyblock3-0.2.8/src/fermion_symmetry.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    35673 2023-06-22 21:12:01.000000 pyblock3-0.2.8/src/flat_fermion.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-22 21:12:01.000000 pyblock3-0.2.8/src/flat_fermion.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-06-22 21:12:01.000000 pyblock3-0.2.8/src/flat_fermion_tmpl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    26561 2023-06-22 21:12:01.000000 pyblock3-0.2.8/src/flat_functor.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-06-22 21:12:01.000000 pyblock3-0.2.8/src/flat_functor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-06-22 21:12:01.000000 pyblock3-0.2.8/src/flat_functor_tmpl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    74291 2023-06-22 21:12:01.000000 pyblock3-0.2.8/src/flat_sparse.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11959 2023-06-22 21:12:01.000000 pyblock3-0.2.8/src/flat_sparse.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10372 2023-06-22 21:12:01.000000 pyblock3-0.2.8/src/flat_sparse_tmpl.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:12:17.743842 pyblock3-0.2.8/src/gpu/
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-06-22 21:12:01.000000 pyblock3-0.2.8/src/gpu/flat_fermion.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-06-22 21:12:01.000000 pyblock3-0.2.8/src/gpu/flat_fermion_tmpl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    39837 2023-06-22 21:12:01.000000 pyblock3-0.2.8/src/hamiltonian.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-06-22 21:12:01.000000 pyblock3-0.2.8/src/hamiltonian.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    42218 2023-06-22 21:12:01.000000 pyblock3-0.2.8/src/hamiltonian_ptree.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-06-22 21:12:01.000000 pyblock3-0.2.8/src/hamiltonian_ptree.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    59786 2023-06-22 21:12:01.000000 pyblock3-0.2.8/src/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-06-22 21:12:01.000000 pyblock3-0.2.8/src/max_flow.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    36058 2023-06-22 21:12:01.000000 pyblock3-0.2.8/src/qc_expr.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    23892 2023-06-22 21:12:01.000000 pyblock3-0.2.8/src/qc_hamiltonian.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-22 21:12:01.000000 pyblock3-0.2.8/src/qc_hamiltonian.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    26524 2023-06-22 21:12:01.000000 pyblock3-0.2.8/src/qc_mpo.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10579 2023-06-22 21:12:01.000000 pyblock3-0.2.8/src/qc_symbolic.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-22 21:12:01.000000 pyblock3-0.2.8/src/symmetry_tmpl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-06-22 21:12:01.000000 pyblock3-0.2.8/src/sz.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7033 2023-06-22 21:12:01.000000 pyblock3-0.2.8/src/tensor.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-06-22 21:12:01.000000 pyblock3-0.2.8/src/tensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-06-22 21:12:01.000000 pyblock3-0.2.8/src/tensor_einsum.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-06-22 21:12:01.000000 pyblock3-0.2.8/src/tensor_einsum.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7495 2023-06-22 21:12:01.000000 pyblock3-0.2.8/src/tensor_impl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    30167 2023-06-22 21:12:01.000000 pyblock3-0.2.8/src/tensor_impl.hpp
```

### Comparing `pyblock3-0.2.7/CMakeLists.txt` & `pyblock3-0.2.8/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -153,15 +153,15 @@
         FIND_LIBRARY(OMP_LIB_NAME NAMES gomp PATHS ${OMP_LIB_HINT})
     ENDIF()
     SET(MKL_OMP_LIB_NAME mkl_gnu_thread)
 ENDIF()
 
 IF (${USE_MKL})
     SET(CMAKE_FIND_LIBRARY_SUFFIXES_BKP ${CMAKE_FIND_LIBRARY_SUFFIXES})
-    SET(CMAKE_FIND_LIBRARY_SUFFIXES "${CMAKE_FIND_LIBRARY_SUFFIXES_BKP};.so.1;.so.2;.so.3;.so.4")
+    SET(CMAKE_FIND_LIBRARY_SUFFIXES "${CMAKE_FIND_LIBRARY_SUFFIXES_BKP};.so.1;.1.dylib;.so.2;.2.dylib;.so.3;.3.dylib;.so.4;.4.dylib")
     FIND_PATH(MKL_INCLUDE_DIR NAMES mkl.h HINTS $ENV{MKLROOT}/include /usr/local/include ${PYTHON_INCLUDE_PATH})
     FIND_LIBRARY(MKL_LIB_LP NAMES mkl_intel_lp64
         PATHS $ENV{MKLROOT}/lib $ENV{MKLROOT}/lib/intel64 /usr/local/lib ${PYTHON_LIB_PATH} NO_DEFAULT_PATH)
     FIND_LIBRARY(MKL_LIB_CORE NAMES mkl_core
         PATHS $ENV{MKLROOT}/lib $ENV{MKLROOT}/lib/intel64 /usr/local/lib ${PYTHON_LIB_PATH} NO_DEFAULT_PATH)
     FIND_LIBRARY(MKL_LIB_GT NAMES ${MKL_OMP_LIB_NAME}
         PATHS $ENV{MKLROOT}/lib $ENV{MKLROOT}/lib/intel64 /usr/local/lib ${PYTHON_LIB_PATH} NO_DEFAULT_PATH)
```

### Comparing `pyblock3-0.2.7/LICENSE` & `pyblock3-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/PKG-INFO` & `pyblock3-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyblock3
-Version: 0.2.7
+Version: 0.2.8
 Summary: An efficient python block-sparse tensor and MPS/DMRG library.
 Home-page: https://github.com/block-hczhai/pyblock3-preview
 Author: Huanchen Zhai, Yang Gao, and Garnet K.-L. Chan
 Author-email: hczhai@ucla.edu
 License: LICENSE
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyblock3-0.2.7/README.md` & `pyblock3-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/pyblock3/algebra/ad/core.py` & `pyblock3-0.2.8/pyblock3/algebra/ad/core.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/pyblock3/algebra/ad/fermion.py` & `pyblock3-0.2.8/pyblock3/algebra/ad/fermion.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/pyblock3/algebra/ad/fermion_ops.py` & `pyblock3-0.2.8/pyblock3/algebra/ad/fermion_ops.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/pyblock3/algebra/ad/flat.py` & `pyblock3-0.2.8/pyblock3/algebra/ad/flat.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/pyblock3/algebra/ad/flat_impl.py` & `pyblock3-0.2.8/pyblock3/algebra/ad/flat_impl.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/pyblock3/algebra/ad/mps.py` & `pyblock3-0.2.8/pyblock3/algebra/ad/mps.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/pyblock3/algebra/core.py` & `pyblock3-0.2.8/pyblock3/algebra/core.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/pyblock3/algebra/einsum.py` & `pyblock3-0.2.8/pyblock3/algebra/einsum.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/pyblock3/algebra/fermion.py` & `pyblock3-0.2.8/pyblock3/algebra/fermion.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/pyblock3/algebra/fermion_encoding.py` & `pyblock3-0.2.8/pyblock3/algebra/fermion_encoding.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/pyblock3/algebra/fermion_large.py` & `pyblock3-0.2.8/pyblock3/algebra/fermion_large.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/pyblock3/algebra/fermion_ops.py` & `pyblock3-0.2.8/pyblock3/algebra/fermion_ops.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/pyblock3/algebra/fermion_setting.py` & `pyblock3-0.2.8/pyblock3/algebra/fermion_setting.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/pyblock3/algebra/fermion_symmetry.py` & `pyblock3-0.2.8/pyblock3/algebra/fermion_symmetry.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/pyblock3/algebra/flat.py` & `pyblock3-0.2.8/pyblock3/algebra/flat.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/pyblock3/algebra/flat_functor.py` & `pyblock3-0.2.8/pyblock3/algebra/flat_functor.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/pyblock3/algebra/funcs.py` & `pyblock3-0.2.8/pyblock3/algebra/funcs.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/pyblock3/algebra/impl/flat.py` & `pyblock3-0.2.8/pyblock3/algebra/impl/flat.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/pyblock3/algebra/integrate.py` & `pyblock3-0.2.8/pyblock3/algebra/integrate.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/pyblock3/algebra/linalg.py` & `pyblock3-0.2.8/pyblock3/algebra/linalg.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/pyblock3/algebra/mpe.py` & `pyblock3-0.2.8/pyblock3/algebra/mpe.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/pyblock3/algebra/mps.py` & `pyblock3-0.2.8/pyblock3/algebra/mps.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/pyblock3/algebra/symmetry.py` & `pyblock3-0.2.8/pyblock3/algebra/symmetry.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/pyblock3/algebra/tests/test_boson_cpp.py` & `pyblock3-0.2.8/pyblock3/algebra/tests/test_boson_cpp.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/pyblock3/algebra/tests/test_boson_python.py` & `pyblock3-0.2.8/pyblock3/algebra/tests/test_boson_python.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/pyblock3/algebra/tests/test_fermion_cpp.py` & `pyblock3-0.2.8/pyblock3/algebra/tests/test_fermion_cpp.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/pyblock3/algebra/tests/test_fermion_large.py` & `pyblock3-0.2.8/pyblock3/algebra/tests/test_fermion_large.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/pyblock3/algebra/tests/test_fermion_ops.py` & `pyblock3-0.2.8/pyblock3/algebra/tests/test_fermion_ops.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/pyblock3/algebra/tests/test_fermion_python.py` & `pyblock3-0.2.8/pyblock3/algebra/tests/test_fermion_python.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/pyblock3/algebra/tests/test_symmetry.py` & `pyblock3-0.2.8/pyblock3/algebra/tests/test_symmetry.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/pyblock3/algorithms/core.py` & `pyblock3-0.2.8/pyblock3/algorithms/core.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/pyblock3/algorithms/dmrg.py` & `pyblock3-0.2.8/pyblock3/algorithms/dmrg.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/pyblock3/algorithms/green.py` & `pyblock3-0.2.8/pyblock3/algorithms/green.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/pyblock3/algorithms/linear.py` & `pyblock3-0.2.8/pyblock3/algorithms/linear.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/pyblock3/algorithms/tddmrg.py` & `pyblock3-0.2.8/pyblock3/algorithms/tddmrg.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/pyblock3/algorithms/tests/test_dmrg.py` & `pyblock3-0.2.8/pyblock3/algorithms/tests/test_dmrg.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/pyblock3/algorithms/tests/test_ghf.py` & `pyblock3-0.2.8/pyblock3/algorithms/tests/test_ghf.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/pyblock3/algorithms/tests/test_sa.py` & `pyblock3-0.2.8/pyblock3/algorithms/tests/test_sa.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/pyblock3/algorithms/tests/test_soc.py` & `pyblock3-0.2.8/pyblock3/algorithms/tests/test_soc.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/pyblock3/block2/hamil.py` & `pyblock3-0.2.8/pyblock3/block2/hamil.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/pyblock3/block2/io.py` & `pyblock3-0.2.8/pyblock3/block2/io.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/pyblock3/fcidump.py` & `pyblock3-0.2.8/pyblock3/fcidump.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/pyblock3/gaussian/core.py` & `pyblock3-0.2.8/pyblock3/gaussian/core.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/pyblock3/hamiltonian.py` & `pyblock3-0.2.8/pyblock3/hamiltonian.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/pyblock3/heisenberg.py` & `pyblock3-0.2.8/pyblock3/heisenberg.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/pyblock3/symbolic/expr.py` & `pyblock3-0.2.8/pyblock3/symbolic/expr.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/pyblock3/symbolic/symbolic.py` & `pyblock3-0.2.8/pyblock3/symbolic/symbolic.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/pyblock3/symbolic/symbolic_mpo.py` & `pyblock3-0.2.8/pyblock3/symbolic/symbolic_mpo.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/pyblock3.egg-info/PKG-INFO` & `pyblock3-0.2.8/pyblock3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyblock3
-Version: 0.2.7
+Version: 0.2.8
 Summary: An efficient python block-sparse tensor and MPS/DMRG library.
 Home-page: https://github.com/block-hczhai/pyblock3-preview
 Author: Huanchen Zhai, Yang Gao, and Garnet K.-L. Chan
 Author-email: hczhai@ucla.edu
 License: LICENSE
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyblock3-0.2.7/pyblock3.egg-info/SOURCES.txt` & `pyblock3-0.2.8/pyblock3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/setup.py` & `pyblock3-0.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
             subprocess.check_call(['cmake', '--build', '.', '--config', cfg, '--', '--jobs=4'],
                                   cwd=self.build_temp)
 
 
 setup_options = dict(
     name='pyblock3',
-    version='0.2.7',
+    version='0.2.8',
     packages=find_packages(),
     license='LICENSE',
     description='An efficient python block-sparse tensor and MPS/DMRG library.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Huanchen Zhai, Yang Gao, and Garnet K.-L. Chan',
     author_email='hczhai@ucla.edu',
```

### Comparing `pyblock3-0.2.7/src/bond_info.cpp` & `pyblock3-0.2.8/src/bond_info.cpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/src/bond_info.hpp` & `pyblock3-0.2.8/src/bond_info.hpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/src/bond_info_tmpl.hpp` & `pyblock3-0.2.8/src/bond_info_tmpl.hpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/src/fermion_symmetry.hpp` & `pyblock3-0.2.8/src/fermion_symmetry.hpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/src/flat_fermion.cpp` & `pyblock3-0.2.8/src/flat_fermion.cpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/src/flat_fermion.hpp` & `pyblock3-0.2.8/src/flat_fermion.hpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/src/flat_fermion_tmpl.hpp` & `pyblock3-0.2.8/src/flat_fermion_tmpl.hpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/src/flat_functor.cpp` & `pyblock3-0.2.8/src/flat_functor.cpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/src/flat_functor.hpp` & `pyblock3-0.2.8/src/flat_functor.hpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/src/flat_functor_tmpl.hpp` & `pyblock3-0.2.8/src/flat_functor_tmpl.hpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/src/flat_sparse.cpp` & `pyblock3-0.2.8/src/flat_sparse.cpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/src/flat_sparse.hpp` & `pyblock3-0.2.8/src/flat_sparse.hpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/src/flat_sparse_tmpl.hpp` & `pyblock3-0.2.8/src/flat_sparse_tmpl.hpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/src/gpu/flat_fermion.hpp` & `pyblock3-0.2.8/src/gpu/flat_fermion.hpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/src/gpu/flat_fermion_tmpl.hpp` & `pyblock3-0.2.8/src/gpu/flat_fermion_tmpl.hpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/src/hamiltonian.cpp` & `pyblock3-0.2.8/src/hamiltonian.cpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/src/hamiltonian.hpp` & `pyblock3-0.2.8/src/hamiltonian.hpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/src/hamiltonian_ptree.cpp` & `pyblock3-0.2.8/src/hamiltonian_ptree.cpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/src/hamiltonian_ptree.hpp` & `pyblock3-0.2.8/src/hamiltonian_ptree.hpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/src/main.cpp` & `pyblock3-0.2.8/src/main.cpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/src/max_flow.hpp` & `pyblock3-0.2.8/src/max_flow.hpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/src/qc_expr.hpp` & `pyblock3-0.2.8/src/qc_expr.hpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/src/qc_hamiltonian.cpp` & `pyblock3-0.2.8/src/qc_hamiltonian.cpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/src/qc_hamiltonian.hpp` & `pyblock3-0.2.8/src/qc_hamiltonian.hpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/src/qc_mpo.hpp` & `pyblock3-0.2.8/src/qc_mpo.hpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/src/qc_symbolic.hpp` & `pyblock3-0.2.8/src/qc_symbolic.hpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/src/symmetry_tmpl.hpp` & `pyblock3-0.2.8/src/symmetry_tmpl.hpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/src/sz.hpp` & `pyblock3-0.2.8/src/sz.hpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/src/tensor.cpp` & `pyblock3-0.2.8/src/tensor.cpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/src/tensor.hpp` & `pyblock3-0.2.8/src/tensor.hpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/src/tensor_einsum.cpp` & `pyblock3-0.2.8/src/tensor_einsum.cpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/src/tensor_einsum.hpp` & `pyblock3-0.2.8/src/tensor_einsum.hpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/src/tensor_impl.cpp` & `pyblock3-0.2.8/src/tensor_impl.cpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.7/src/tensor_impl.hpp` & `pyblock3-0.2.8/src/tensor_impl.hpp`

 * *Files identical despite different names*

