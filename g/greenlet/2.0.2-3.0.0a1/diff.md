# Comparing `tmp/greenlet-2.0.2.tar.gz` & `tmp/greenlet-3.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "greenlet-2.0.2.tar", last modified: Sat Jan 28 14:19:24 2023, max compression
+gzip compressed data, was "greenlet-3.0.0a1.tar", last modified: Wed Jun 21 22:01:39 2023, max compression
```

## Comparing `greenlet-2.0.2.tar` & `greenlet-3.0.0a1.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-01-28 14:19:24.823805 greenlet-2.0.2/
--rw-r--r--   0 jmadden    (501) staff       (20)      697 2023-01-28 14:19:23.000000 greenlet-2.0.2/.clang-format
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-01-28 14:19:24.788707 greenlet-2.0.2/.github/
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-01-28 14:19:24.795563 greenlet-2.0.2/.github/workflows/
--rw-r--r--   0 jmadden    (501) staff       (20)     7789 2023-01-28 14:19:23.000000 greenlet-2.0.2/.github/workflows/tests.yml
--rw-r--r--   0 jmadden    (501) staff       (20)      142 2023-01-28 14:19:23.000000 greenlet-2.0.2/.gitignore
--rw-r--r--   0 jmadden    (501) staff       (20)     5046 2023-01-28 14:19:23.000000 greenlet-2.0.2/.pylintrc
--rw-r--r--   0 jmadden    (501) staff       (20)      439 2023-01-28 14:19:23.000000 greenlet-2.0.2/.readthedocs.yml
--rw-r--r--   0 jmadden    (501) staff       (20)      849 2023-01-28 14:19:23.000000 greenlet-2.0.2/AUTHORS
--rw-r--r--   0 jmadden    (501) staff       (20)    15901 2023-01-28 14:19:23.000000 greenlet-2.0.2/CHANGES.rst
--rw-r--r--   0 jmadden    (501) staff       (20)     1434 2023-01-28 14:19:23.000000 greenlet-2.0.2/LICENSE
--rw-r--r--   0 jmadden    (501) staff       (20)     2424 2023-01-28 14:19:23.000000 greenlet-2.0.2/LICENSE.PSF
--rw-r--r--   0 jmadden    (501) staff       (20)      902 2023-01-28 14:19:23.000000 greenlet-2.0.2/MANIFEST.in
--rw-r--r--   0 jmadden    (501) staff       (20)     3895 2023-01-28 14:19:24.823978 greenlet-2.0.2/PKG-INFO
--rw-r--r--   0 jmadden    (501) staff       (20)     2211 2023-01-28 14:19:23.000000 greenlet-2.0.2/README.rst
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-01-28 14:19:24.796244 greenlet-2.0.2/appveyor/
--rw-r--r--   0 jmadden    (501) staff       (20)     7195 2023-01-28 14:19:23.000000 greenlet-2.0.2/appveyor/install.ps1
--rw-r--r--   0 jmadden    (501) staff       (20)     3366 2023-01-28 14:19:23.000000 greenlet-2.0.2/appveyor/run_with_env.cmd
--rw-r--r--   0 jmadden    (501) staff       (20)     7462 2023-01-28 14:19:23.000000 greenlet-2.0.2/appveyor.yml
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-01-28 14:19:24.796560 greenlet-2.0.2/benchmarks/
--rwxr-xr-x   0 jmadden    (501) staff       (20)     2589 2023-01-28 14:19:23.000000 greenlet-2.0.2/benchmarks/chain.py
--rw-r--r--   0 jmadden    (501) staff       (20)       17 2023-01-28 14:19:23.000000 greenlet-2.0.2/dev-requirements.txt
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-01-28 14:19:24.802382 greenlet-2.0.2/docs/
--rw-r--r--   0 jmadden    (501) staff       (20)     5572 2023-01-28 14:19:23.000000 greenlet-2.0.2/docs/Makefile
--rw-r--r--   0 jmadden    (501) staff       (20)     2437 2023-01-28 14:19:23.000000 greenlet-2.0.2/docs/api.rst
--rw-r--r--   0 jmadden    (501) staff       (20)     3377 2023-01-28 14:19:23.000000 greenlet-2.0.2/docs/c_api.rst
--rw-r--r--   0 jmadden    (501) staff       (20)     1137 2023-01-28 14:19:23.000000 greenlet-2.0.2/docs/caveats.rst
--rw-r--r--   0 jmadden    (501) staff       (20)       28 2023-01-28 14:19:23.000000 greenlet-2.0.2/docs/changes.rst
--rw-r--r--   0 jmadden    (501) staff       (20)     8899 2023-01-28 14:19:23.000000 greenlet-2.0.2/docs/conf.py
--rw-r--r--   0 jmadden    (501) staff       (20)     4876 2023-01-28 14:19:23.000000 greenlet-2.0.2/docs/contextvars.rst
--rw-r--r--   0 jmadden    (501) staff       (20)     4750 2023-01-28 14:19:23.000000 greenlet-2.0.2/docs/creating_executing_greenlets.rst
--rw-r--r--   0 jmadden    (501) staff       (20)      736 2023-01-28 14:19:23.000000 greenlet-2.0.2/docs/development.rst
--rw-r--r--   0 jmadden    (501) staff       (20)     5885 2023-01-28 14:19:23.000000 greenlet-2.0.2/docs/greenlet.rst
--rw-r--r--   0 jmadden    (501) staff       (20)     6217 2023-01-28 14:19:23.000000 greenlet-2.0.2/docs/greenlet_gc.rst
--rw-r--r--   0 jmadden    (501) staff       (20)     9267 2023-01-28 14:19:23.000000 greenlet-2.0.2/docs/gui_example.rst
--rw-r--r--   0 jmadden    (501) staff       (20)       87 2023-01-28 14:19:23.000000 greenlet-2.0.2/docs/history.rst
--rw-r--r--   0 jmadden    (501) staff       (20)     5431 2023-01-28 14:19:23.000000 greenlet-2.0.2/docs/index.rst
--rw-r--r--   0 jmadden    (501) staff       (20)     5100 2023-01-28 14:19:23.000000 greenlet-2.0.2/docs/make.bat
--rw-r--r--   0 jmadden    (501) staff       (20)     2398 2023-01-28 14:19:23.000000 greenlet-2.0.2/docs/python_threads.rst
--rw-r--r--   0 jmadden    (501) staff       (20)     6096 2023-01-28 14:19:23.000000 greenlet-2.0.2/docs/switching.rst
--rw-r--r--   0 jmadden    (501) staff       (20)     2960 2023-01-28 14:19:23.000000 greenlet-2.0.2/docs/tracing.rst
--rwxr-xr-x   0 jmadden    (501) staff       (20)     1990 2023-01-28 14:19:23.000000 greenlet-2.0.2/make-manylinux
--rw-r--r--   0 jmadden    (501) staff       (20)      125 2023-01-28 14:19:24.824500 greenlet-2.0.2/setup.cfg
--rwxr-xr-x   0 jmadden    (501) staff       (20)    10184 2023-01-28 14:19:23.000000 greenlet-2.0.2/setup.py
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-01-28 14:19:24.789756 greenlet-2.0.2/src/
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-01-28 14:19:24.807607 greenlet-2.0.2/src/greenlet/
--rw-r--r--   0 jmadden    (501) staff       (20)     1723 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/__init__.py
--rw-r--r--   0 jmadden    (501) staff       (20)   110159 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/greenlet.cpp
--rw-r--r--   0 jmadden    (501) staff       (20)     4755 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/greenlet.h
--rw-r--r--   0 jmadden    (501) staff       (20)     1582 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/greenlet_allocator.hpp
--rw-r--r--   0 jmadden    (501) staff       (20)     5446 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/greenlet_compiler_compat.hpp
--rw-r--r--   0 jmadden    (501) staff       (20)     4806 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/greenlet_cpython_compat.hpp
--rw-r--r--   0 jmadden    (501) staff       (20)     2307 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/greenlet_exceptions.hpp
--rw-r--r--   0 jmadden    (501) staff       (20)    41611 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/greenlet_greenlet.hpp
--rw-r--r--   0 jmadden    (501) staff       (20)     2707 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/greenlet_internal.hpp
--rw-r--r--   0 jmadden    (501) staff       (20)    32906 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/greenlet_refs.hpp
--rw-r--r--   0 jmadden    (501) staff       (20)     3987 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/greenlet_slp_switch.hpp
--rw-r--r--   0 jmadden    (501) staff       (20)    21075 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/greenlet_thread_state.hpp
--rw-r--r--   0 jmadden    (501) staff       (20)     3831 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/greenlet_thread_state_dict_cleanup.hpp
--rw-r--r--   0 jmadden    (501) staff       (20)     4126 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/greenlet_thread_support.hpp
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-01-28 14:19:24.817961 greenlet-2.0.2/src/greenlet/platform/
--rw-r--r--   0 jmadden    (501) staff       (20)        0 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/platform/__init__.py
--rw-r--r--   0 jmadden    (501) staff       (20)      143 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/platform/setup_switch_x64_masm.cmd
--rw-r--r--   0 jmadden    (501) staff       (20)     2683 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/platform/switch_aarch64_gcc.h
--rw-r--r--   0 jmadden    (501) staff       (20)      689 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/platform/switch_alpha_unix.h
--rw-r--r--   0 jmadden    (501) staff       (20)     2748 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/platform/switch_amd64_unix.h
--rw-r--r--   0 jmadden    (501) staff       (20)     2488 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/platform/switch_arm32_gcc.h
--rw-r--r--   0 jmadden    (501) staff       (20)     1901 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/platform/switch_arm32_ios.h
--rw-r--r--   0 jmadden    (501) staff       (20)     1245 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/platform/switch_arm64_masm.asm
--rw-r--r--   0 jmadden    (501) staff       (20)      746 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/platform/switch_arm64_masm.obj
--rw-r--r--   0 jmadden    (501) staff       (20)      398 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/platform/switch_arm64_msvc.h
--rw-r--r--   0 jmadden    (501) staff       (20)     1340 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/platform/switch_csky_gcc.h
--rw-r--r--   0 jmadden    (501) staff       (20)      928 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/platform/switch_m68k_gcc.h
--rw-r--r--   0 jmadden    (501) staff       (20)     1444 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/platform/switch_mips_unix.h
--rw-r--r--   0 jmadden    (501) staff       (20)     3878 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/platform/switch_ppc64_aix.h
--rw-r--r--   0 jmadden    (501) staff       (20)     3833 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/platform/switch_ppc64_linux.h
--rw-r--r--   0 jmadden    (501) staff       (20)     2959 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/platform/switch_ppc_aix.h
--rw-r--r--   0 jmadden    (501) staff       (20)     2777 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/platform/switch_ppc_linux.h
--rw-r--r--   0 jmadden    (501) staff       (20)     2642 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/platform/switch_ppc_macosx.h
--rw-r--r--   0 jmadden    (501) staff       (20)     2670 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/platform/switch_ppc_unix.h
--rw-r--r--   0 jmadden    (501) staff       (20)      740 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/platform/switch_riscv_unix.h
--rw-r--r--   0 jmadden    (501) staff       (20)     2781 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/platform/switch_s390_unix.h
--rw-r--r--   0 jmadden    (501) staff       (20)     2815 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/platform/switch_sparc_sun_gcc.h
--rw-r--r--   0 jmadden    (501) staff       (20)     1527 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/platform/switch_x32_unix.h
--rw-r--r--   0 jmadden    (501) staff       (20)     1841 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/platform/switch_x64_masm.asm
--rw-r--r--   0 jmadden    (501) staff       (20)     1078 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/platform/switch_x64_masm.obj
--rw-r--r--   0 jmadden    (501) staff       (20)     1805 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/platform/switch_x64_msvc.h
--rw-r--r--   0 jmadden    (501) staff       (20)    12838 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/platform/switch_x86_msvc.h
--rw-r--r--   0 jmadden    (501) staff       (20)     3068 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/platform/switch_x86_unix.h
--rw-r--r--   0 jmadden    (501) staff       (20)     3280 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/slp_platformselect.h
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-01-28 14:19:24.823559 greenlet-2.0.2/src/greenlet/tests/
--rw-r--r--   0 jmadden    (501) staff       (20)     4976 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/tests/__init__.py
--rw-r--r--   0 jmadden    (501) staff       (20)     6017 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/tests/_test_extension.c
--rw-r--r--   0 jmadden    (501) staff       (20)     5639 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/tests/_test_extension_cpp.cpp
--rw-r--r--   0 jmadden    (501) staff       (20)    11929 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/tests/leakcheck.py
--rw-r--r--   0 jmadden    (501) staff       (20)    10240 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/tests/test_contextvars.py
--rw-r--r--   0 jmadden    (501) staff       (20)     2963 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/tests/test_cpp.py
--rw-r--r--   0 jmadden    (501) staff       (20)     3829 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/tests/test_extension_interface.py
--rw-r--r--   0 jmadden    (501) staff       (20)     2916 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/tests/test_gc.py
--rw-r--r--   0 jmadden    (501) staff       (20)     1240 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/tests/test_generator.py
--rw-r--r--   0 jmadden    (501) staff       (20)     3720 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/tests/test_generator_nested.py
--rw-r--r--   0 jmadden    (501) staff       (20)    37747 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/tests/test_greenlet.py
--rw-r--r--   0 jmadden    (501) staff       (20)     7683 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/tests/test_greenlet_trash.py
--rw-r--r--   0 jmadden    (501) staff       (20)    17683 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/tests/test_leaks.py
--rw-r--r--   0 jmadden    (501) staff       (20)      446 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/tests/test_stack_saved.py
--rw-r--r--   0 jmadden    (501) staff       (20)     3734 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/tests/test_throw.py
--rw-r--r--   0 jmadden    (501) staff       (20)     7843 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/tests/test_tracing.py
--rwxr-xr-x   0 jmadden    (501) staff       (20)     1339 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/tests/test_version.py
--rw-r--r--   0 jmadden    (501) staff       (20)      898 2023-01-28 14:19:23.000000 greenlet-2.0.2/src/greenlet/tests/test_weakref.py
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-01-28 14:19:24.809431 greenlet-2.0.2/src/greenlet.egg-info/
--rw-r--r--   0 jmadden    (501) staff       (20)     3895 2023-01-28 14:19:24.000000 greenlet-2.0.2/src/greenlet.egg-info/PKG-INFO
--rw-r--r--   0 jmadden    (501) staff       (20)     3188 2023-01-28 14:19:24.000000 greenlet-2.0.2/src/greenlet.egg-info/SOURCES.txt
--rw-r--r--   0 jmadden    (501) staff       (20)        1 2023-01-28 14:19:24.000000 greenlet-2.0.2/src/greenlet.egg-info/dependency_links.txt
--rw-r--r--   0 jmadden    (501) staff       (20)        1 2023-01-28 14:19:24.000000 greenlet-2.0.2/src/greenlet.egg-info/not-zip-safe
--rw-r--r--   0 jmadden    (501) staff       (20)       82 2023-01-28 14:19:24.000000 greenlet-2.0.2/src/greenlet.egg-info/requires.txt
--rw-r--r--   0 jmadden    (501) staff       (20)        9 2023-01-28 14:19:24.000000 greenlet-2.0.2/src/greenlet.egg-info/top_level.txt
--rw-r--r--   0 jmadden    (501) staff       (20)      816 2023-01-28 14:19:23.000000 greenlet-2.0.2/tox.ini
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-06-21 22:01:39.731233 greenlet-3.0.0a1/
+-rw-r--r--   0 jmadden    (501) staff       (20)      697 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/.clang-format
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-06-21 22:01:39.719174 greenlet-3.0.0a1/.github/
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-06-21 22:01:39.721738 greenlet-3.0.0a1/.github/workflows/
+-rw-r--r--   0 jmadden    (501) staff       (20)     6584 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/.github/workflows/tests.yml
+-rw-r--r--   0 jmadden    (501) staff       (20)      142 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/.gitignore
+-rw-r--r--   0 jmadden    (501) staff       (20)     5046 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/.pylintrc
+-rw-r--r--   0 jmadden    (501) staff       (20)      439 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/.readthedocs.yml
+-rw-r--r--   0 jmadden    (501) staff       (20)      849 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/AUTHORS
+-rw-r--r--   0 jmadden    (501) staff       (20)    17230 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/CHANGES.rst
+-rw-r--r--   0 jmadden    (501) staff       (20)     1434 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/LICENSE
+-rw-r--r--   0 jmadden    (501) staff       (20)     2424 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/LICENSE.PSF
+-rw-r--r--   0 jmadden    (501) staff       (20)      902 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/MANIFEST.in
+-rw-r--r--   0 jmadden    (501) staff       (20)     3715 2023-06-21 22:01:39.731304 greenlet-3.0.0a1/PKG-INFO
+-rw-r--r--   0 jmadden    (501) staff       (20)     2211 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/README.rst
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-06-21 22:01:39.721986 greenlet-3.0.0a1/appveyor/
+-rw-r--r--   0 jmadden    (501) staff       (20)     7195 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/appveyor/install.ps1
+-rw-r--r--   0 jmadden    (501) staff       (20)     3366 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/appveyor/run_with_env.cmd
+-rw-r--r--   0 jmadden    (501) staff       (20)     6894 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/appveyor.yml
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-06-21 22:01:39.722098 greenlet-3.0.0a1/benchmarks/
+-rwxr-xr-x   0 jmadden    (501) staff       (20)     2589 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/benchmarks/chain.py
+-rw-r--r--   0 jmadden    (501) staff       (20)       17 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/dev-requirements.txt
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-06-21 22:01:39.723942 greenlet-3.0.0a1/docs/
+-rw-r--r--   0 jmadden    (501) staff       (20)     5572 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/docs/Makefile
+-rw-r--r--   0 jmadden    (501) staff       (20)     2437 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/docs/api.rst
+-rw-r--r--   0 jmadden    (501) staff       (20)     3377 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/docs/c_api.rst
+-rw-r--r--   0 jmadden    (501) staff       (20)     1137 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/docs/caveats.rst
+-rw-r--r--   0 jmadden    (501) staff       (20)       28 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/docs/changes.rst
+-rw-r--r--   0 jmadden    (501) staff       (20)     8899 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/docs/conf.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     4876 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/docs/contextvars.rst
+-rw-r--r--   0 jmadden    (501) staff       (20)     4750 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/docs/creating_executing_greenlets.rst
+-rw-r--r--   0 jmadden    (501) staff       (20)      736 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/docs/development.rst
+-rw-r--r--   0 jmadden    (501) staff       (20)     5885 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/docs/greenlet.rst
+-rw-r--r--   0 jmadden    (501) staff       (20)     6217 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/docs/greenlet_gc.rst
+-rw-r--r--   0 jmadden    (501) staff       (20)     9267 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/docs/gui_example.rst
+-rw-r--r--   0 jmadden    (501) staff       (20)       87 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/docs/history.rst
+-rw-r--r--   0 jmadden    (501) staff       (20)     5431 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/docs/index.rst
+-rw-r--r--   0 jmadden    (501) staff       (20)     5100 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/docs/make.bat
+-rw-r--r--   0 jmadden    (501) staff       (20)     2398 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/docs/python_threads.rst
+-rw-r--r--   0 jmadden    (501) staff       (20)     6096 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/docs/switching.rst
+-rw-r--r--   0 jmadden    (501) staff       (20)     2960 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/docs/tracing.rst
+-rwxr-xr-x   0 jmadden    (501) staff       (20)     1985 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/make-manylinux
+-rw-r--r--   0 jmadden    (501) staff       (20)      125 2023-06-21 22:01:39.731506 greenlet-3.0.0a1/setup.cfg
+-rwxr-xr-x   0 jmadden    (501) staff       (20)     9618 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/setup.py
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-06-21 22:01:39.719545 greenlet-3.0.0a1/src/
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-06-21 22:01:39.725692 greenlet-3.0.0a1/src/greenlet/
+-rw-r--r--   0 jmadden    (501) staff       (20)     1725 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/__init__.py
+-rw-r--r--   0 jmadden    (501) staff       (20)   106403 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/greenlet.cpp
+-rw-r--r--   0 jmadden    (501) staff       (20)     4755 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/greenlet.h
+-rw-r--r--   0 jmadden    (501) staff       (20)     1582 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/greenlet_allocator.hpp
+-rw-r--r--   0 jmadden    (501) staff       (20)     4140 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/greenlet_compiler_compat.hpp
+-rw-r--r--   0 jmadden    (501) staff       (20)     3414 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/greenlet_cpython_compat.hpp
+-rw-r--r--   0 jmadden    (501) staff       (20)     2307 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/greenlet_exceptions.hpp
+-rw-r--r--   0 jmadden    (501) staff       (20)    41744 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/greenlet_greenlet.hpp
+-rw-r--r--   0 jmadden    (501) staff       (20)     2703 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/greenlet_internal.hpp
+-rw-r--r--   0 jmadden    (501) staff       (20)    32762 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/greenlet_refs.hpp
+-rw-r--r--   0 jmadden    (501) staff       (20)     3198 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/greenlet_slp_switch.hpp
+-rw-r--r--   0 jmadden    (501) staff       (20)    20614 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/greenlet_thread_state.hpp
+-rw-r--r--   0 jmadden    (501) staff       (20)     3831 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/greenlet_thread_state_dict_cleanup.hpp
+-rw-r--r--   0 jmadden    (501) staff       (20)      867 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/greenlet_thread_support.hpp
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-06-21 22:01:39.729194 greenlet-3.0.0a1/src/greenlet/platform/
+-rw-r--r--   0 jmadden    (501) staff       (20)        0 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/platform/__init__.py
+-rw-r--r--   0 jmadden    (501) staff       (20)      143 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/platform/setup_switch_x64_masm.cmd
+-rw-r--r--   0 jmadden    (501) staff       (20)     4084 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/platform/switch_aarch64_gcc.h
+-rw-r--r--   0 jmadden    (501) staff       (20)      671 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/platform/switch_alpha_unix.h
+-rw-r--r--   0 jmadden    (501) staff       (20)     2748 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/platform/switch_amd64_unix.h
+-rw-r--r--   0 jmadden    (501) staff       (20)     2479 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/platform/switch_arm32_gcc.h
+-rw-r--r--   0 jmadden    (501) staff       (20)     1892 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/platform/switch_arm32_ios.h
+-rw-r--r--   0 jmadden    (501) staff       (20)     1245 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/platform/switch_arm64_masm.asm
+-rw-r--r--   0 jmadden    (501) staff       (20)      746 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/platform/switch_arm64_masm.obj
+-rw-r--r--   0 jmadden    (501) staff       (20)      398 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/platform/switch_arm64_msvc.h
+-rw-r--r--   0 jmadden    (501) staff       (20)     1331 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/platform/switch_csky_gcc.h
+-rw-r--r--   0 jmadden    (501) staff       (20)      928 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/platform/switch_m68k_gcc.h
+-rw-r--r--   0 jmadden    (501) staff       (20)     1426 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/platform/switch_mips_unix.h
+-rw-r--r--   0 jmadden    (501) staff       (20)     3860 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/platform/switch_ppc64_aix.h
+-rw-r--r--   0 jmadden    (501) staff       (20)     3815 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/platform/switch_ppc64_linux.h
+-rw-r--r--   0 jmadden    (501) staff       (20)     2941 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/platform/switch_ppc_aix.h
+-rw-r--r--   0 jmadden    (501) staff       (20)     2759 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/platform/switch_ppc_linux.h
+-rw-r--r--   0 jmadden    (501) staff       (20)     2624 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/platform/switch_ppc_macosx.h
+-rw-r--r--   0 jmadden    (501) staff       (20)     2652 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/platform/switch_ppc_unix.h
+-rw-r--r--   0 jmadden    (501) staff       (20)      740 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/platform/switch_riscv_unix.h
+-rw-r--r--   0 jmadden    (501) staff       (20)     2763 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/platform/switch_s390_unix.h
+-rw-r--r--   0 jmadden    (501) staff       (20)     2797 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/platform/switch_sparc_sun_gcc.h
+-rw-r--r--   0 jmadden    (501) staff       (20)     1509 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/platform/switch_x32_unix.h
+-rw-r--r--   0 jmadden    (501) staff       (20)     1841 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/platform/switch_x64_masm.asm
+-rw-r--r--   0 jmadden    (501) staff       (20)     1078 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/platform/switch_x64_masm.obj
+-rw-r--r--   0 jmadden    (501) staff       (20)     1805 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/platform/switch_x64_msvc.h
+-rw-r--r--   0 jmadden    (501) staff       (20)    12838 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/platform/switch_x86_msvc.h
+-rw-r--r--   0 jmadden    (501) staff       (20)     3059 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/platform/switch_x86_unix.h
+-rw-r--r--   0 jmadden    (501) staff       (20)     3280 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/slp_platformselect.h
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-06-21 22:01:39.731117 greenlet-3.0.0a1/src/greenlet/tests/
+-rw-r--r--   0 jmadden    (501) staff       (20)     4976 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/tests/__init__.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     5773 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/tests/_test_extension.c
+-rw-r--r--   0 jmadden    (501) staff       (20)     5344 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/tests/_test_extension_cpp.cpp
+-rw-r--r--   0 jmadden    (501) staff       (20)    11929 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/tests/leakcheck.py
+-rw-r--r--   0 jmadden    (501) staff       (20)    10240 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/tests/test_contextvars.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     2963 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/tests/test_cpp.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     3829 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/tests/test_extension_interface.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     2916 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/tests/test_gc.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     1240 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/tests/test_generator.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     3720 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/tests/test_generator_nested.py
+-rw-r--r--   0 jmadden    (501) staff       (20)    37546 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/tests/test_greenlet.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     7508 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/tests/test_greenlet_trash.py
+-rw-r--r--   0 jmadden    (501) staff       (20)    17623 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/tests/test_leaks.py
+-rw-r--r--   0 jmadden    (501) staff       (20)      446 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/tests/test_stack_saved.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     3734 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/tests/test_throw.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     7843 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/tests/test_tracing.py
+-rwxr-xr-x   0 jmadden    (501) staff       (20)     1339 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/tests/test_version.py
+-rw-r--r--   0 jmadden    (501) staff       (20)      898 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet/tests/test_weakref.py
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-06-21 22:01:39.726339 greenlet-3.0.0a1/src/greenlet.egg-info/
+-rw-r--r--   0 jmadden    (501) staff       (20)     3715 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet.egg-info/PKG-INFO
+-rw-r--r--   0 jmadden    (501) staff       (20)     3188 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet.egg-info/SOURCES.txt
+-rw-r--r--   0 jmadden    (501) staff       (20)        1 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet.egg-info/dependency_links.txt
+-rw-r--r--   0 jmadden    (501) staff       (20)        1 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet.egg-info/not-zip-safe
+-rw-r--r--   0 jmadden    (501) staff       (20)       39 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet.egg-info/requires.txt
+-rw-r--r--   0 jmadden    (501) staff       (20)        9 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/src/greenlet.egg-info/top_level.txt
+-rw-r--r--   0 jmadden    (501) staff       (20)      639 2023-06-21 22:01:39.000000 greenlet-3.0.0a1/tox.ini
```

### Comparing `greenlet-2.0.2/.clang-format` & `greenlet-3.0.0a1/.clang-format`

 * *Files identical despite different names*

### Comparing `greenlet-2.0.2/.github/workflows/tests.yml` & `greenlet-3.0.0a1/.github/workflows/tests.yml`

 * *Files 12% similar despite different names*

```diff
@@ -21,19 +21,19 @@
 
 
 jobs:
   test:
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        python-version: [2.7, 3.5, 3.6, 3.7, 3.8, 3.9, "3.10", "3.11"]
-        # Jan 2023: We have pinned back from ubuntu-latest (which is
-        # now ubuntu 22.04) because older Python versions like
-        # 3.5, 3.6 and presumably 2.7 are not available in it.
-        os: [ubuntu-20.04, macos-latest]
+        python-version: [3.7, 3.8, 3.9, "3.10", "3.11", "3.12-dev"]
+        os: [ubuntu-latest, macos-latest]
+        exclude:
+          - os: macos-latest
+            python-version: 3.12-dev
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
         cache: 'pip'
@@ -73,14 +73,15 @@
     - name: Store greenlet wheel
       uses: actions/upload-artifact@v3
       with:
         name: greenlet-${{ runner.os }}-${{ matrix.python-version }}.whl
         path: dist/*whl
     - name: Test
       run: |
+        python -VV
         python -c 'import greenlet._greenlet as G; assert G.GREENLET_USE_STANDARD_THREADING'
         python -m unittest discover -v greenlet.tests
     - name: Doctest
       run: |
         sphinx-build -b doctest -d docs/_build/doctrees2 docs docs/_build/doctest2
     - name: Publish package to PyPI (mac)
       # We cannot 'uses: pypa/gh-action-pypi-publish@v1.4.1' because
@@ -88,43 +89,14 @@
       # the Mac.
       if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags') && startsWith(runner.os, 'Mac')
       env:
         TWINE_PASSWORD: ${{ secrets.TWINE_PASSWORD }}
       run: |
         twine upload --skip-existing dist/*
 
-  test_non_standard_thread:
-    runs-on: ${{ matrix.os }}
-    strategy:
-      matrix:
-        python-version: [2.7, 3.5, "3.11"]
-        os: [ubuntu-20.04, macos-latest]
-    steps:
-    - uses: actions/checkout@v3
-    - name: Set up Python
-      uses: actions/setup-python@v4
-      with:
-        python-version: ${{ matrix.python-version }}
-        cache: 'pip'
-        cache-dependency-path: setup.py
-    - name: Install dependencies
-      run: |
-        python -m pip install -U pip setuptools wheel
-        python -m pip install -U twine
-    - name: Install greenlet
-      env:
-        CPPFLAGS: "-DG_USE_STANDARD_THREADING=0 -UNDEBUG -Ofast"
-      run: |
-        python setup.py bdist_wheel
-        python -m pip install -U -v -e ".[test,docs]"
-    - name: Test
-      run: |
-        python -c 'import greenlet._greenlet as G; assert not G.GREENLET_USE_STANDARD_THREADING'
-        python -m unittest discover -v greenlet.tests
-
   CodeQL:
     runs-on: ubuntu-latest
     permissions:
       # required for all workflows
       security-events: write
     steps:
       - uses: actions/checkout@v3
@@ -164,33 +136,31 @@
     strategy:
       matrix:
         python-version: [3.9]
         image:
           - manylinux2010_x86_64
           - manylinux2014_aarch64
           - manylinux2014_ppc64le
+          - manylinux2014_s390x
           - manylinux2014_x86_64
           - musllinux_1_1_x86_64
           - musllinux_1_1_aarch64
     name: ${{ matrix.image }}
 
     steps:
       - name: checkout
         uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
-      - name: Enable emulation
-        run: |
-          docker run --rm --privileged hypriot/qemu-register
-        # This one was seen in pyca/bcrypt. What's the difference?
-        # (Other than this one not working.)
-        #run: |
-        #  docker run --rm --privileged multiarch/qemu-user-static:register --reset
+      - name: Set up QEMU
+        uses: docker/setup-qemu-action@v2
+        with:
+          platforms: all
       - name: Build and test greenlet
         if: matrix.image == 'manylinux2010_x86_64'
         # An alternate way to do this is to run the container directly with a uses:
         # and then the script runs inside it. That may work better with caching.
         # See https://github.com/pyca/bcrypt/blob/f6b5ee2eda76d077c531362ac65e16f045cf1f29/.github/workflows/wheel-builder.yml
         # The 2010 image is the last one that comes with Python 2.7,
         # and only up through the tag 2021-02-06-3d322a5
```

### Comparing `greenlet-2.0.2/.pylintrc` & `greenlet-3.0.0a1/.pylintrc`

 * *Files identical despite different names*

### Comparing `greenlet-2.0.2/AUTHORS` & `greenlet-3.0.0a1/AUTHORS`

 * *Files identical despite different names*

### Comparing `greenlet-2.0.2/CHANGES.rst` & `greenlet-3.0.0a1/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,40 @@
 =========
  Changes
 =========
 
+3.0.0a1 (2023-06-21)
+====================
+
+- Build binary wheels for S390x Linux. See `PR 358
+  <https://github.com/python-greenlet/greenlet/pull/358>`_ from Steven
+  Silvester.
+- Fix a rare crash on shutdown seen in uWSGI deployments. See `issue
+  330 <https://github.com/python-greenlet/greenlet/issues/330>`_ and `PR 356
+  <https://github.com/python-greenlet/greenlet/pull/356>`_ from Andrew
+  Wason.
+- Make the platform-specific low-level C/assembly snippets stop using
+  the ``register`` storage class. Newer versions of standards remove
+  this storage class, and it has been generally ignored by many
+  compilers for some time. See `PR 347
+  <https://github.com/python-greenlet/greenlet/pull/347>`_ from Khem
+  Raj.
+- Add initial support for Python 3.12. See `issue
+  <https://github.com/python-greenlet/greenlet/issues/323>`_ and `PR
+  <https://github.com/python-greenlet/greenlet/pull/327>`_; thanks go
+  to (at least) Michael Droettboom, Andreas Motl, Thomas A Caswell,
+  raphaelauv, Hugo van Kemenade, Mark Shannon, and Petr Viktorin.
+- Remove support for end-of-life Python versions, including Python
+  2.7, Python 3.5 and Python 3.6.
+- Require a compiler that supports ``noinline`` directives. See
+  `issue 271
+  <https://github.com/python-greenlet/greenlet/issues/266>`_.
+- Require a compiler that supports C++11.
+
+
 2.0.2 (2023-01-28)
 ==================
 
 - Fix calling ``greenlet.settrace()`` with the same tracer object that
   was currently active. See `issue 332
   <https://github.com/python-greenlet/greenlet/issues/332>`_.
 - Various compilation and standards conformance fixes. See #335, #336,
```

### Comparing `greenlet-2.0.2/LICENSE` & `greenlet-3.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `greenlet-2.0.2/LICENSE.PSF` & `greenlet-3.0.0a1/LICENSE.PSF`

 * *Files identical despite different names*

### Comparing `greenlet-2.0.2/MANIFEST.in` & `greenlet-3.0.0a1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `greenlet-2.0.2/PKG-INFO` & `greenlet-3.0.0a1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: greenlet
-Version: 2.0.2
+Version: 3.0.0a1
 Summary: Lightweight in-process concurrent programming
 Home-page: https://greenlet.readthedocs.io/
 Author: Alexey Borzenkov
 Author-email: snaury@gmail.com
 Maintainer: Jason Madden
 Maintainer-email: jason@seecoresoftware.com
 License: MIT License
@@ -15,27 +15,24 @@
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: test
 License-File: LICENSE
 License-File: LICENSE.PSF
 License-File: AUTHORS
```

### Comparing `greenlet-2.0.2/README.rst` & `greenlet-3.0.0a1/README.rst`

 * *Files identical despite different names*

### Comparing `greenlet-2.0.2/appveyor/install.ps1` & `greenlet-3.0.0a1/appveyor/install.ps1`

 * *Files identical despite different names*

### Comparing `greenlet-2.0.2/appveyor/run_with_env.cmd` & `greenlet-3.0.0a1/appveyor/run_with_env.cmd`

 * *Files identical despite different names*

### Comparing `greenlet-2.0.2/appveyor.yml` & `greenlet-3.0.0a1/appveyor.yml`

 * *Files 10% similar despite different names*

```diff
@@ -35,25 +35,31 @@
       secure: 9JKBIB2o2S18+REaEqzUrP/1g08eRdX3eEa7D/BBN5ae0XHTlrPqbvRTNJceiUa/o3r4bejFF3o0xA69ueMd+09PGKAAAfpQnwnQPInuLVkOq3mprNk4wW0GyWLFzI3WqZhYnWH7PZtmG4Kr7mNOyd6Qdi773kN3Hn7CNhvk+ik/K3zbsGerb2YYloM/KIQSJbgdEqNcIIItoqrZzg/cqiM/47Pz7ZzcGDvevD8Nx/0lVGqFVJnj8cMevwa9iDPYn7fB59Y1GEEbtBjenrWr1Q==
 
   matrix:
     # http://www.appveyor.com/docs/installed-software#python
 
     # Fully supported 64-bit versions, with testing. This should be
     # all the current (non EOL) versions.
+    - PYTHON: "C:\\Python312-x64"
+      PYTHON_VERSION: "3.12.0b3"
+      PYTHON_ARCH: "64"
+      PYTHON_EXE: python
+      APPVEYOR_BUILD_WORKER_IMAGE: Visual Studio 2022
+
     - PYTHON: "C:\\Python311-x64"
       PYTHON_VERSION: "3.11.0"
       PYTHON_ARCH: "64"
       PYTHON_EXE: python
-      APPVEYOR_BUILD_WORKER_IMAGE: Visual Studio 2019
+      APPVEYOR_BUILD_WORKER_IMAGE: Visual Studio 2022
 
     - PYTHON: "C:\\Python310-x64"
       PYTHON_VERSION: "3.10.0"
       PYTHON_ARCH: "64"
       PYTHON_EXE: python
-      APPVEYOR_BUILD_WORKER_IMAGE: Visual Studio 2019
+      APPVEYOR_BUILD_WORKER_IMAGE: Visual Studio 2022
 
     - PYTHON: "C:\\Python39-x64"
       PYTHON_ARCH: "64"
       PYTHON_VERSION: "3.9.x"
       PYTHON_EXE: python
       APPVEYOR_BUILD_WORKER_IMAGE: Visual Studio 2019
 
@@ -65,49 +71,29 @@
 
     - PYTHON: "C:\\Python37-x64"
       PYTHON_ARCH: "64"
       PYTHON_VERSION: "3.7.x"
       PYTHON_EXE: python
       APPVEYOR_BUILD_WORKER_IMAGE: Visual Studio 2019
 
-    - PYTHON: "C:\\Python27-x64"
-      PYTHON_ARCH: "64"
-      PYTHON_VERSION: "2.7.x"
-      PYTHON_EXE: python
-
     # Tested 32-bit versions. A small, hand-picked selection covering
     # important variations. No need to include newer versions of
     # cpython here, 32-bit x86 windows is on the way out.
 
     - PYTHON: "C:\\Python39"
       PYTHON_ARCH: "32"
       PYTHON_VERSION: "3.9.x"
       PYTHON_EXE: python
       APPVEYOR_BUILD_WORKER_IMAGE: Visual Studio 2019
 
-    - PYTHON: "C:\\Python27"
-      PYTHON_ARCH: "32"
-      PYTHON_VERSION: "2.7.x"
-      PYTHON_EXE: python
-
 
     # Untested 64-bit versions. We don't expect any variance here from
     # the other tested 64-bit versions, OR they are very EOL
 
-    - PYTHON: "C:\\Python36-x64"
-      PYTHON_ARCH: "64"
-      PYTHON_VERSION: "3.6.x"
-      PYTHON_EXE: python
-      GWHEEL_ONLY: true
-
-    - PYTHON: "C:\\Python35-x64"
-      PYTHON_ARCH: "64"
-      PYTHON_VERSION: "3.5.x"
-      PYTHON_EXE: python
-      GWHEEL_ONLY: true
+    # None right now.
 
     # Untested 32-bit versions. As above, we don't expect any variance
     # from the tested 32-bit versions, OR they are very EOL.
 
     - PYTHON: "C:\\Python38"
       PYTHON_ARCH: "32"
       PYTHON_VERSION: "3.8.x"
@@ -116,26 +102,14 @@
 
     - PYTHON: "C:\\Python37"
       PYTHON_ARCH: "32"
       PYTHON_VERSION: "3.7.x"
       PYTHON_EXE: python
       GWHEEL_ONLY: true
 
-    - PYTHON: "C:\\Python36"
-      PYTHON_ARCH: "32"
-      PYTHON_VERSION: "3.6.x"
-      PYTHON_EXE: python
-      GWHEEL_ONLY: true
-
-    - PYTHON: "C:\\Python35"
-      PYTHON_ARCH: "32"
-      PYTHON_VERSION: "3.5.x"
-      PYTHON_EXE: python
-      GWHEEL_ONLY: true
-
 
 
 cache:
   - "%TMP%\\py\\"
   - '%LOCALAPPDATA%\pip\Cache -> appveyor.yml,setup.py'
 
 install:
```

### Comparing `greenlet-2.0.2/benchmarks/chain.py` & `greenlet-3.0.0a1/benchmarks/chain.py`

 * *Files identical despite different names*

### Comparing `greenlet-2.0.2/docs/Makefile` & `greenlet-3.0.0a1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `greenlet-2.0.2/docs/api.rst` & `greenlet-3.0.0a1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `greenlet-2.0.2/docs/c_api.rst` & `greenlet-3.0.0a1/docs/c_api.rst`

 * *Files identical despite different names*

### Comparing `greenlet-2.0.2/docs/caveats.rst` & `greenlet-3.0.0a1/docs/caveats.rst`

 * *Files identical despite different names*

### Comparing `greenlet-2.0.2/docs/conf.py` & `greenlet-3.0.0a1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `greenlet-2.0.2/docs/contextvars.rst` & `greenlet-3.0.0a1/docs/contextvars.rst`

 * *Files identical despite different names*

### Comparing `greenlet-2.0.2/docs/creating_executing_greenlets.rst` & `greenlet-3.0.0a1/docs/creating_executing_greenlets.rst`

 * *Files identical despite different names*

### Comparing `greenlet-2.0.2/docs/development.rst` & `greenlet-3.0.0a1/docs/development.rst`

 * *Files identical despite different names*

### Comparing `greenlet-2.0.2/docs/greenlet.rst` & `greenlet-3.0.0a1/docs/greenlet.rst`

 * *Files identical despite different names*

### Comparing `greenlet-2.0.2/docs/greenlet_gc.rst` & `greenlet-3.0.0a1/docs/greenlet_gc.rst`

 * *Files identical despite different names*

### Comparing `greenlet-2.0.2/docs/gui_example.rst` & `greenlet-3.0.0a1/docs/gui_example.rst`

 * *Files identical despite different names*

### Comparing `greenlet-2.0.2/docs/index.rst` & `greenlet-3.0.0a1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `greenlet-2.0.2/docs/make.bat` & `greenlet-3.0.0a1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `greenlet-2.0.2/docs/python_threads.rst` & `greenlet-3.0.0a1/docs/python_threads.rst`

 * *Files identical despite different names*

### Comparing `greenlet-2.0.2/docs/switching.rst` & `greenlet-3.0.0a1/docs/switching.rst`

 * *Files identical despite different names*

### Comparing `greenlet-2.0.2/docs/tracing.rst` & `greenlet-3.0.0a1/docs/tracing.rst`

 * *Files identical despite different names*

### Comparing `greenlet-2.0.2/make-manylinux` & `greenlet-3.0.0a1/make-manylinux`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     cd /tmp/build
     git clone /greenlet greenlet
     cd greenlet
 
     mkdir -p /greenlet/wheelhouse
     OPATH="$PATH"
     which auditwheel
-    for variant in `ls -d /opt/python/cp{27,35,36,37,38,39,310,311}*`; do
+    for variant in `ls -d /opt/python/cp{37,38,39,310,311,312}*`; do
         export PATH="$variant/bin:$OPATH"
         echo "Building $variant $(python --version)"
 
         python -mpip install -U pip
         python setup.py bdist_wheel
         python -mpip install -U .[test]
         python -m unittest discover -v greenlet.tests
@@ -49,9 +49,9 @@
     done
 
     exit 0
 fi
 
 # Mount the current directory as /greenlet
 # Can't use -i on Travis with arm64, "input device not a tty"
-docker run --rm -v "$(pwd):/greenlet"  ${DOCKER_IMAGE:-quay.io/pypa/manylinux2010_x86_64} /greenlet/$(basename $0)
+docker run --rm -v "$(pwd):/greenlet"  ${DOCKER_IMAGE:-quay.io/pypa/manylinux2014_x86_64} /greenlet/$(basename $0)
 ls -l wheelhouse
```

### Comparing `greenlet-2.0.2/setup.py` & `greenlet-3.0.0a1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -224,37 +224,29 @@
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Programming Language :: C',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Operating System :: OS Independent',
         'Topic :: Software Development :: Libraries :: Python Modules'
     ],
     extras_require={
         'docs': [
             'Sphinx',
-            # 0.18b1 breaks sphinx 1.8.5 which is the latest version that runs
-            # on Python 2. The version pin sphinx itself contains isn't specific enough.
-            'docutils < 0.18; python_version < "3"',
         ],
         'test': [
             'objgraph',
-            # Sigh, all releases of this were yanked from PyPI.
-            #'faulthandler; python_version == "2.7" and platform_python_implementation == "CPython"',
             'psutil',
         ],
     },
-    python_requires=">=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*",
+    python_requires=">=3.7",
     zip_safe=False,
 )
```

### Comparing `greenlet-2.0.2/src/greenlet/__init__.py` & `greenlet-3.0.0a1/src/greenlet/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 ]
 
 # pylint:disable=no-name-in-module
 
 ###
 # Metadata
 ###
-__version__ = '2.0.2'
+__version__ = '3.0.0a1'
 from ._greenlet import _C_API # pylint:disable=no-name-in-module
 
 ###
 # Exceptions
 ###
 from ._greenlet import GreenletExit
 from ._greenlet import error
```

### Comparing `greenlet-2.0.2/src/greenlet/greenlet.cpp` & `greenlet-3.0.0a1/src/greenlet/greenlet.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -148,15 +148,15 @@
 greenlet::refs::_BorrowedGreenlet<T, TC>& greenlet::refs::_BorrowedGreenlet<T, TC>::operator=(const greenlet::refs::BorrowedObject& other)
 {
     this->_set_raw_pointer(static_cast<PyObject*>(other));
     return *this;
 }
 
 template <typename T, greenlet::refs::TypeChecker TC>
-inline greenlet::refs::_BorrowedGreenlet<T, TC>::operator Greenlet*() const G_NOEXCEPT
+inline greenlet::refs::_BorrowedGreenlet<T, TC>::operator Greenlet*() const noexcept
 {
     if (!this->p) {
         return nullptr;
     }
     return reinterpret_cast<PyGreenlet*>(this->p)->pimpl;
 }
 
@@ -165,15 +165,15 @@
     : BorrowedReference<T, TC>(nullptr)
 {
 
     this->_set_raw_pointer(p.borrow());
 }
 
 template <typename T, greenlet::refs::TypeChecker TC>
-inline greenlet::refs::_OwnedGreenlet<T, TC>::operator Greenlet*() const G_NOEXCEPT
+inline greenlet::refs::_OwnedGreenlet<T, TC>::operator Greenlet*() const noexcept
 {
     if (!this->p) {
         return nullptr;
     }
     return reinterpret_cast<PyGreenlet*>(this->p)->pimpl;
 }
 
@@ -295,41 +295,33 @@
 
 };
 
 // This encapsulates what were previously module global "constants"
 // established at init time.
 // This is a step towards Python3 style module state that allows
 // reloading.
-// We play some tricks with placement new to be able to allocate this
-// object statically still, so that references to its members don't
-// incur an extra pointer indirection.
+//
+// In an earlier iteration of this code, we used placement new to be
+// able to allocate this object statically still, so that references
+// to its members don't incur an extra pointer indirection.
+// But under some scenarios, that could result in crashes at
+// shutdown because apparently the destructor was getting run twice?
 class GreenletGlobals
 {
 public:
     const ImmortalEventName event_switch;
     const ImmortalEventName event_throw;
     const ImmortalException PyExc_GreenletError;
     const ImmortalException PyExc_GreenletExit;
     const ImmortalObject empty_tuple;
     const ImmortalObject empty_dict;
     const ImmortalString str_run;
     Mutex* const thread_states_to_destroy_lock;
     greenlet::cleanup_queue_t thread_states_to_destroy;
 
-    GreenletGlobals(const int UNUSED(dummy)) :
-        event_switch(0),
-        event_throw(0),
-        PyExc_GreenletError(0),
-        PyExc_GreenletExit(0),
-        empty_tuple(0),
-        empty_dict(0),
-        str_run(0),
-        thread_states_to_destroy_lock(0)
-    {}
-
     GreenletGlobals() :
         event_switch("switch"),
         event_throw("throw"),
         PyExc_GreenletError("greenlet.error"),
         PyExc_GreenletExit("greenlet.GreenletExit", PyExc_BaseException),
         empty_tuple(Require(PyTuple_New(0))),
         empty_dict(Require(PyDict_New())),
@@ -366,15 +358,15 @@
         greenlet::cleanup_queue_t& q = const_cast<greenlet::cleanup_queue_t&>(this->thread_states_to_destroy);
         ThreadState* result = q.back();
         q.pop_back();
         return result;
     }
 };
 
-static const GreenletGlobals mod_globs(0);
+static const GreenletGlobals* mod_globs;
 
 // Protected by the GIL. Incremented when we create a main greenlet,
 // in a new thread, decremented when it is destroyed.
 static Py_ssize_t total_main_greenlets;
 
 struct ThreadState_DestroyWithGIL
 {
@@ -642,28 +634,28 @@
         // Python thread could run and call ``os.fork()``, which would
         // be bad if that happenend while we are holding the cleanup
         // lock (it wouldn't function in the child process).
         // Make a best effort to try to keep the duration we hold the
         // lock short.
         // TODO: On platforms that support it, use ``pthread_atfork`` to
         // drop this lock.
-        LockGuard cleanup_lock(*mod_globs.thread_states_to_destroy_lock);
+        LockGuard cleanup_lock(*mod_globs->thread_states_to_destroy_lock);
 
         if (state && state->has_main_greenlet()) {
             // Because we don't have the GIL, this is a race condition.
             if (!PyInterpreterState_Head()) {
                 // We have to leak the thread state, if the
                 // interpreter has shut down when we're getting
                 // deallocated, we can't run the cleanup code that
                 // deleting it would imply.
                 return;
             }
 
-            mod_globs.queue_to_destroy(state);
-            if (mod_globs.thread_states_to_destroy.size() == 1) {
+            mod_globs->queue_to_destroy(state);
+            if (mod_globs->thread_states_to_destroy.size() == 1) {
                 // We added the first item to the queue. We need to schedule
                 // the cleanup.
                 int result = ThreadState_DestroyNoGIL::AddPendingCall(
                     ThreadState_DestroyNoGIL::DestroyQueueWithGIL,
                     NULL);
                 if (result < 0) {
                     // Hmm, what can we do here?
@@ -679,87 +671,38 @@
     DestroyQueueWithGIL(void* UNUSED(arg))
     {
         // We're holding the GIL here, so no Python code should be able to
         // run to call ``os.fork()``.
         while (1) {
             ThreadState* to_destroy;
             {
-                LockGuard cleanup_lock(*mod_globs.thread_states_to_destroy_lock);
-                if (mod_globs.thread_states_to_destroy.empty()) {
+                LockGuard cleanup_lock(*mod_globs->thread_states_to_destroy_lock);
+                if (mod_globs->thread_states_to_destroy.empty()) {
                     break;
                 }
-                to_destroy = mod_globs.take_next_to_destroy();
+                to_destroy = mod_globs->take_next_to_destroy();
             }
             // Drop the lock while we do the actual deletion.
             ThreadState_DestroyWithGIL::DestroyWithGIL(to_destroy);
         }
         return 0;
     }
 
 };
 
-// The intent when GET_THREAD_STATE() is used multiple times in a function is to
-// take a reference to it in a local variable, to avoid the
-// thread-local indirection. On some platforms (macOS),
-// accessing a thread-local involves a function call (plus an initial
-// function call in each function that uses a thread local); in
-// contrast, static volatile variables are at some pre-computed offset.
-
-#if G_USE_STANDARD_THREADING == 1
+// The intent when GET_THREAD_STATE() is needed multiple times in a
+// function is to take a reference to its return value in a local
+// variable, to avoid the thread-local indirection. On some platforms
+// (macOS), accessing a thread-local involves a function call (plus an
+// initial function call in each function that uses a thread local);
+// in contrast, static volatile variables are at some pre-computed
+// offset.
 typedef greenlet::ThreadStateCreator<ThreadState_DestroyNoGIL> ThreadStateCreator;
-static G_THREAD_LOCAL_VAR ThreadStateCreator g_thread_state_global;
+static thread_local ThreadStateCreator g_thread_state_global;
 #define GET_THREAD_STATE() g_thread_state_global
-#else
-// if we're not using standard threading, we're using
-// the Python thread-local dictionary to perform our cleanup,
-// which means we're deallocated when holding the GIL. The
-// thread state is valid enough still for us to destroy
-// stuff.
-typedef greenlet::ThreadStateCreator<ThreadState_DestroyWithGIL> ThreadStateCreator;
-#define G_THREAD_STATE_DICT_CLEANUP_TYPE
-#include "greenlet_thread_state_dict_cleanup.hpp"
-typedef greenlet::refs::OwnedReference<PyGreenletCleanup> OwnedGreenletCleanup;
-// RECALL: legacy thread-local objects (__thread on GCC, __declspec(thread) on
-// MSVC) can't have constructors or destructors, they have to be
-// constant. So we indirect through a pointer and a function.
-static G_THREAD_LOCAL_VAR ThreadStateCreator* _g_thread_state_global_ptr = nullptr;
-static ThreadStateCreator& GET_THREAD_STATE()
-{
-    if (!_g_thread_state_global_ptr) {
-        // NOTE: If any of this fails, we'll probably go on to hard
-        // crash the process, because we're returning a reference to a
-        // null pointer. we've called Py_FatalError(), but have no way
-        // to communicate that to the caller. Since these should
-        // essentially never fail unless the entire process is borked,
-        // a hard crash with a decent C++ backtrace from the exception
-        // is much more useful.
-        _g_thread_state_global_ptr = new ThreadStateCreator();
-        if (!_g_thread_state_global_ptr) {
-            throw PyFatalError("greenlet: Failed to create greenlet thread state.");
-        }
-
-        OwnedGreenletCleanup cleanup(OwnedGreenletCleanup::consuming(PyType_GenericAlloc(&PyGreenletCleanup_Type, 0)));
-        if (!cleanup) {
-            throw PyFatalError("greenlet: Failed to create greenlet thread state cleanup.");
-        }
-
-        cleanup->thread_state_creator = _g_thread_state_global_ptr;
-        assert(PyObject_GC_IsTracked(cleanup.borrow_o()));
-
-        PyObject* ts_dict_w = PyThreadState_GetDict();
-        if (!ts_dict_w) {
-            throw PyFatalError("greenlet: Failed to get Python thread state.");
-        }
-        if (PyDict_SetItemString(ts_dict_w, "__greenlet_cleanup", cleanup.borrow_o()) < 0) {
-            throw PyFatalError("greenlet: Failed to save cleanup key in Python thread state.");
-        }
-    }
-    return *_g_thread_state_global_ptr;
-}
-#endif
 
 
 Greenlet::Greenlet(PyGreenlet* p)
 {
     p ->pimpl = this;
 }
 
@@ -767,15 +710,15 @@
     : stack_state(initial_stack)
 {
     // can't use a delegating constructor because of
     // MSVC for Python 2.7
     p->pimpl = this;
 }
 
-UserGreenlet::UserGreenlet(PyGreenlet* p,BorrowedGreenlet the_parent)
+UserGreenlet::UserGreenlet(PyGreenlet* p, BorrowedGreenlet the_parent)
     : Greenlet(p), _parent(the_parent)
 {
     this->_self = p;
 }
 
 
 MainGreenlet::MainGreenlet(PyGreenlet* p, ThreadState* state)
@@ -783,34 +726,34 @@
       _self(p),
       _thread_state(state)
 {
     total_main_greenlets++;
 }
 
 ThreadState*
-MainGreenlet::thread_state() const G_NOEXCEPT
+MainGreenlet::thread_state() const noexcept
 {
     return this->_thread_state;
 }
 
 void
-MainGreenlet::thread_state(ThreadState* t) G_NOEXCEPT
+MainGreenlet::thread_state(ThreadState* t) noexcept
 {
     assert(!t);
     this->_thread_state = t;
 }
 
 BorrowedGreenlet
-UserGreenlet::self() const G_NOEXCEPT
+UserGreenlet::self() const noexcept
 {
     return this->_self;
 }
 
 BorrowedGreenlet
-MainGreenlet::self() const G_NOEXCEPT
+MainGreenlet::self() const noexcept
 {
     return BorrowedGreenlet(this->_self.borrow());
 }
 
 const BorrowedMainGreenlet
 UserGreenlet::main_greenlet() const
 {
@@ -909,15 +852,15 @@
  * should be and transfers ownership of it to the left-hand-side.
  *
  * If switch() was just passed an arg tuple, then we'll just return that.
  * If only keyword arguments were passed, then we'll pass the keyword
  * argument dict. Otherwise, we'll create a tuple of (args, kwargs) and
  * return both.
  */
-OwnedObject& operator<<=(OwnedObject& lhs, greenlet::SwitchingArgs& rhs) G_NOEXCEPT
+OwnedObject& operator<<=(OwnedObject& lhs, greenlet::SwitchingArgs& rhs) noexcept
 {
     // Because this may invoke arbitrary Python code, which could
     // result in switching back to us, we need to get the
     // arguments locally on the stack.
     assert(rhs);
     OwnedObject args = rhs.args();
     OwnedObject kwargs = rhs.kwargs();
@@ -976,15 +919,15 @@
 
 OwnedObject
 Greenlet::throw_GreenletExit_during_dealloc(const ThreadState& UNUSED(current_thread_state))
 {
     // If we're killed because we lost all references in the
     // middle of a switch, that's ok. Don't reset the args/kwargs,
     // we still want to pass them to the parent.
-    PyErr_SetString(mod_globs.PyExc_GreenletExit,
+    PyErr_SetString(mod_globs->PyExc_GreenletExit,
                     "Killing the greenlet because all references have vanished.");
     // To get here it had to have run before
     return this->g_switch();
 }
 
 OwnedObject
 UserGreenlet::throw_GreenletExit_during_dealloc(const ThreadState& current_thread_state)
@@ -998,53 +941,53 @@
     // exception happened. Whether or not an exception happens,
     // we need to restore the parent in case the greenlet gets
     // resurrected.
     return Greenlet::throw_GreenletExit_during_dealloc(current_thread_state);
 }
 
 ThreadState*
-UserGreenlet::thread_state() const G_NOEXCEPT
+UserGreenlet::thread_state() const noexcept
 {
     // TODO: maybe make this throw, if the thread state isn't there?
     // if (!this->main_greenlet) {
     //     throw std::runtime_error("No thread state"); // TODO: Better exception
     // }
     if (!this->_main_greenlet) {
         return nullptr;
     }
     return this->_main_greenlet->thread_state();
 }
 
 
 
 bool
-UserGreenlet::was_running_in_dead_thread() const G_NOEXCEPT
+UserGreenlet::was_running_in_dead_thread() const noexcept
 {
     return this->_main_greenlet && !this->thread_state();
 }
 
 bool
-MainGreenlet::was_running_in_dead_thread() const G_NOEXCEPT
+MainGreenlet::was_running_in_dead_thread() const noexcept
 {
     return !this->_thread_state;
 }
 
 inline void
-Greenlet::slp_restore_state() G_NOEXCEPT
+Greenlet::slp_restore_state() noexcept
 {
 #ifdef SLP_BEFORE_RESTORE_STATE
     SLP_BEFORE_RESTORE_STATE();
 #endif
     this->stack_state.copy_heap_to_stack(
            this->thread_state()->borrow_current()->stack_state);
 }
 
 
 inline int
-Greenlet::slp_save_state(char *const stackref) G_NOEXCEPT
+Greenlet::slp_save_state(char *const stackref) noexcept
 {
     // XXX: This used to happen in the middle, before saving, but
     // after finding the next owner. Does that matter? This is
     // only defined for Sparc/GCC where it flushes register
     // windows to the stack (I think)
 #ifdef SLP_BEFORE_SAVE_STATE
     SLP_BEFORE_SAVE_STATE();
@@ -1168,15 +1111,15 @@
     }
 
     return err.the_state_that_switched->g_switch_finish(err);
 }
 
 
 OwnedGreenlet
-Greenlet::g_switchstack_success() G_NOEXCEPT
+Greenlet::g_switchstack_success() noexcept
 {
     PyThreadState* tstate = PyThreadState_GET();
     // restore the saved state
     this->python_state >> tstate;
     this->exception_state >> tstate;
 
     // The thread state hasn't been changed yet.
@@ -1204,15 +1147,15 @@
         /* save exception in case getattr clears it */
         PyErrPieces saved;
 
         /*
           self.run is the object to call in the new greenlet.
           This could run arbitrary python code and switch greenlets!
         */
-        run = this->_self.PyRequireAttr(mod_globs.str_run);
+        run = this->_self.PyRequireAttr(mod_globs->str_run);
 
         /* restore saved exception */
         saved.PyErrRestore();
 
 
         /* recheck that it's safe to switch in case greenlet reparented anywhere above */
         this->check_switch_allowed();
@@ -1345,15 +1288,15 @@
     // The first switch we need to manually call the trace
     // function here instead of in g_switch_finish, because we
     // never return there.
 
     if (OwnedObject tracefunc = this->thread_state()->get_tracefunc()) {
         try {
             g_calltrace(tracefunc,
-                        args ? mod_globs.event_switch : mod_globs.event_throw,
+                        args ? mod_globs->event_switch : mod_globs->event_throw,
                         origin_greenlet,
                         this->_self);
         }
         catch (const PyErrOccurred&) {
             /* Turn trace errors into switch throws */
             args.CLEAR();
         }
@@ -1406,15 +1349,15 @@
             //
             // Hopefully the basic C stdlib is still functional enough
             // for us to at least print an error.
             //
             // It gets more complicated than that, though, on some
             // platforms, specifically at least Linux/gcc/libstdc++. They use
             // an exception to unwind the stack when a background
-            // thread exits. (See comments about G_NOEXCEPT.) So this
+            // thread exits. (See comments about noexcept.) So this
             // may not actually represent anything untoward. On those
             // platforms we allow throws of this to propagate, or
             // attempt to anyway.
 # if defined(WIN32) || defined(_WIN32)
             Py_FatalError(
                 "greenlet: Unhandled C++ exception from a greenlet run function. "
                 "Because memory is likely corrupted, terminating process.");
@@ -1424,15 +1367,15 @@
 #endif
         }
     }
     args.CLEAR();
     Py_CLEAR(run);
 
     if (!result
-        && mod_globs.PyExc_GreenletExit.PyExceptionMatches()
+        && mod_globs->PyExc_GreenletExit.PyExceptionMatches()
         && (this->switch_args)) {
         // This can happen, for example, if our only reference
         // goes away after we switch back to the parent.
         // See test_dealloc_switch_args_not_lost
         PyErrPieces clear_error;
         result <<= this->switch_args;
         result = single_result(result);
@@ -1554,20 +1497,20 @@
     // thread state pointer we have is bogus.
     // TODO: Give the objects an API to determine if they belong
     // to a dead thread.
 
     const BorrowedMainGreenlet main_greenlet = this->find_main_greenlet_in_lineage();
 
     if (!main_greenlet) {
-        throw PyErrOccurred(mod_globs.PyExc_GreenletError,
+        throw PyErrOccurred(mod_globs->PyExc_GreenletError,
                             "cannot switch to a garbage collected greenlet");
     }
 
     if (!main_greenlet->thread_state()) {
-        throw PyErrOccurred(mod_globs.PyExc_GreenletError,
+        throw PyErrOccurred(mod_globs->PyExc_GreenletError,
                             "cannot switch to a different thread (which happens to have exited)");
     }
 
     // The main greenlet we found was from the .parent lineage.
     // That may or may not have any relationship to the main
     // greenlet of the running thread. We can't actually access
     // our this->thread_state members to try to check that,
@@ -1586,15 +1529,15 @@
             // XXX: Same condition as above. Was this supposed to be
             // this->main_greenlet()?
             && current_main_greenlet != main_greenlet)
         // switching into a known dead thread (XXX: which, if we get here,
         // is bad, because we just accessed the thread state, which is
         // gone!)
         || (!current_main_greenlet->thread_state())) {
-        throw PyErrOccurred(mod_globs.PyExc_GreenletError,
+        throw PyErrOccurred(mod_globs->PyExc_GreenletError,
                             "cannot switch to a different thread");
     }
 }
 
 
 OwnedObject
 Greenlet::g_switch_finish(const switchstack_result_t& err)
@@ -1604,15 +1547,15 @@
     try {
         // Our only caller handles the bad error case
         assert(err.status >= 0);
         assert(state.borrow_current() == this->self());
 
         if (OwnedObject tracefunc = state.get_tracefunc()) {
             g_calltrace(tracefunc,
-                        this->args() ? mod_globs.event_switch : mod_globs.event_throw,
+                        this->args() ? mod_globs->event_switch : mod_globs->event_throw,
                         err.origin_greenlet,
                         this->self());
         }
         // The above could have invoked arbitrary Python code, but
         // it couldn't switch back to this object and *also*
         // throw an exception, so the args won't have changed.
 
@@ -1726,15 +1669,15 @@
 }
 
 
 
 static OwnedObject
 g_handle_exit(const OwnedObject& greenlet_result)
 {
-    if (!greenlet_result && mod_globs.PyExc_GreenletExit.PyExceptionMatches()) {
+    if (!greenlet_result && mod_globs->PyExc_GreenletExit.PyExceptionMatches()) {
         /* catch and ignore GreenletExit */
         PyErrFetchParam val;
         PyErr_Fetch(PyErrFetchParam(), val, PyErrFetchParam());
         if (!val) {
             return OwnedObject::None();
         }
         return OwnedObject(val);
@@ -1755,15 +1698,15 @@
 
 /***********************************************************/
 
 static PyGreenlet*
 green_new(PyTypeObject* type, PyObject* UNUSED(args), PyObject* UNUSED(kwds))
 {
     PyGreenlet* o =
-        (PyGreenlet*)PyBaseObject_Type.tp_new(type, mod_globs.empty_tuple, mod_globs.empty_dict);
+        (PyGreenlet*)PyBaseObject_Type.tp_new(type, mod_globs->empty_tuple, mod_globs->empty_dict);
     if (o) {
         new UserGreenlet(o, GET_THREAD_STATE().state().borrow_current());
         assert(Py_REFCNT(o) == 1);
     }
     return o;
 }
 
@@ -2288,15 +2231,15 @@
     "except that this trick does not work for the\n"
     "`greenlet.GreenletExit` exception, which would not propagate\n"
     "from ``g_raiser`` to ``g``.\n");
 
 static PyObject*
 green_throw(PyGreenlet* self, PyObject* args)
 {
-    PyArgParseParam typ(mod_globs.PyExc_GreenletExit);
+    PyArgParseParam typ(mod_globs->PyExc_GreenletExit);
     PyArgParseParam val;
     PyArgParseParam tb;
 
     if (!PyArg_ParseTuple(args, "|OOO:throw", &typ, &val, &tb)) {
         return NULL;
     }
 
@@ -2496,35 +2439,29 @@
     }
     catch(const PyErrOccurred&) {
         return -1;
     }
     return 0;
 }
 
-#ifdef Py_CONTEXT_H
-#    define GREENLET_NO_CONTEXTVARS_REASON "This build of greenlet"
-#else
-#    define GREENLET_NO_CONTEXTVARS_REASON "This Python interpreter"
-#endif
-
 namespace greenlet
 {
 
-template<>
+
 const OwnedObject
-Greenlet::context<GREENLET_WHEN_PY37>(GREENLET_WHEN_PY37::Yes) const
+Greenlet::context() const
 {
     using greenlet::PythonStateContext;
     OwnedObject result;
 
     if (this->is_currently_running_in_some_thread()) {
         /* Currently running greenlet: context is stored in the thread state,
            not the greenlet object. */
         if (GET_THREAD_STATE().state().is_current(this->self())) {
-            result = PythonStateContext<G_IS_PY37>::context(PyThreadState_GET());
+            result = PythonStateContext::context(PyThreadState_GET());
         }
         else {
             throw ValueError(
                             "cannot get context of a "
                             "greenlet that is running in a different thread");
         }
     }
@@ -2534,26 +2471,16 @@
     }
     if (!result) {
         result = OwnedObject::None();
     }
     return result;
 }
 
-template<>
-const OwnedObject
-Greenlet::context<GREENLET_WHEN_NOT_PY37>(GREENLET_WHEN_NOT_PY37::No) const
-{
-    throw AttributeError(
-                         GREENLET_NO_CONTEXTVARS_REASON
-                         "does not support context variables"
-    );
-}
 
-template<>
-void Greenlet::context<GREENLET_WHEN_PY37>(BorrowedObject given, GREENLET_WHEN_PY37::Yes)
+void Greenlet::context(BorrowedObject given)
 {
     using greenlet::PythonStateContext;
     if (!given) {
         throw AttributeError("can't delete context attribute");
     }
     if (given.is_None()) {
         /* "Empty context" is stored as NULL, not None. */
@@ -2568,62 +2495,51 @@
         if (!GET_THREAD_STATE().state().is_current(this->self())) {
             throw ValueError("cannot set context of a greenlet"
                              " that is running in a different thread");
         }
 
         /* Currently running greenlet: context is stored in the thread state,
            not the greenlet object. */
-        OwnedObject octx = OwnedObject::consuming(PythonStateContext<G_IS_PY37>::context(tstate));
-        PythonStateContext<G_IS_PY37>::context(tstate, context.relinquish_ownership());
+        OwnedObject octx = OwnedObject::consuming(PythonStateContext::context(tstate));
+        PythonStateContext::context(tstate, context.relinquish_ownership());
     }
     else {
         /* Greenlet is not running: just set context. Note that the
            greenlet may be dead.*/
         this->python_state.context() = context;
     }
 }
 
-template<>
-void
-Greenlet::context<GREENLET_WHEN_NOT_PY37>(BorrowedObject UNUSED(given), GREENLET_WHEN_NOT_PY37::No)
-{
-    throw AttributeError(
-                         GREENLET_NO_CONTEXTVARS_REASON
-                         "does not support context variables"
-    );
-}
-
-};
+}; //namespace greenlet
 
 static PyObject*
 green_getcontext(const PyGreenlet* self, void* UNUSED(context))
 {
     const Greenlet *const g = self->pimpl;
     try {
-        OwnedObject result(g->context<G_IS_PY37>());
+        OwnedObject result(g->context());
         return result.relinquish_ownership();
     }
     catch(const PyErrOccurred&) {
         return nullptr;
     }
 }
 
 static int
 green_setcontext(BorrowedGreenlet self, PyObject* nctx, void* UNUSED(context))
 {
     try {
-        self->context<G_IS_PY37>(nctx, G_IS_PY37::IsIt());
+        self->context(nctx);
         return 0;
     }
     catch(const PyErrOccurred&) {
         return -1;
     }
 }
 
-#undef GREENLET_NO_CONTEXTVARS_REASON
 
 static PyObject*
 green_getframe(BorrowedGreenlet self, void* UNUSED(context))
 {
     const PythonState::OwnedFrame& top_frame = self->top_frame();
     return top_frame.acquire_or_None();
 }
@@ -2671,27 +2587,27 @@
             state_in_thread = " (thread exited)";
         }
         else {
             state_in_thread = GET_THREAD_STATE().state().is_current(self)
                 ? " current"
                 : (self->started() ? " suspended" : "");
         }
-        result = GNative_FromFormat(
+        result = PyUnicode_FromFormat(
             "<%s object at %p (otid=%p)%s%s%s%s>",
             tp_name,
             self.borrow_o(),
             self->thread_state(),
             state_in_thread,
             self->active() ? " active" : "",
             never_started ? " pending" : " started",
             self->main() ? " main" : ""
         );
     }
     else {
-        result = GNative_FromFormat(
+        result = PyUnicode_FromFormat(
             "<%s object at %p (otid=%p) %sdead>",
             tp_name,
             self.borrow_o(),
             self->thread_state(),
             self->was_running_in_dead_thread()
             ? "(thread exited) "
             : ""
@@ -2731,21 +2647,21 @@
     if (!g) {
         return NULL;
     }
 
     try {
         NewDictReference kwargs;
         if (run) {
-            kwargs.SetItem(mod_globs.str_run, run);
+            kwargs.SetItem(mod_globs->str_run, run);
         }
         if (parent) {
             kwargs.SetItem("parent", (PyObject*)parent);
         }
 
-        Require(green_init(g, mod_globs.empty_tuple, kwargs));
+        Require(green_init(g, mod_globs->empty_tuple, kwargs));
     }
     catch (const PyErrOccurred&) {
         return nullptr;
     }
 
     return g.relinquish_ownership();
 }
@@ -2757,15 +2673,15 @@
 
     if (!PyGreenlet_Check(self)) {
         PyErr_BadArgument();
         return NULL;
     }
 
     if (args == NULL) {
-        args = mod_globs.empty_tuple;
+        args = mod_globs->empty_tuple;
     }
 
     if (kwargs == NULL || !PyDict_Check(kwargs)) {
         kwargs = NULL;
     }
 
     return green_switch(g, args, kwargs);
@@ -2857,17 +2773,14 @@
     {NULL}
 };
 
 static PyNumberMethods green_as_number = {
     NULL, /* nb_add */
     NULL, /* nb_subtract */
     NULL, /* nb_multiply */
-#if PY_MAJOR_VERSION < 3
-    NULL, /* nb_divide */
-#endif
     NULL,                /* nb_remainder */
     NULL,                /* nb_divmod */
     NULL,                /* nb_power */
     NULL,                /* nb_negative */
     NULL,                /* nb_positive */
     NULL,                /* nb_absolute */
     (inquiry)green_bool, /* nb_bool */
@@ -3003,16 +2916,16 @@
              "\n"
              "Get the number of greenlet cleanup operations pending. Testing only.\n");
 
 
 static PyObject*
 mod_get_pending_cleanup_count(PyObject* UNUSED(module))
 {
-    LockGuard cleanup_lock(*mod_globs.thread_states_to_destroy_lock);
-    return PyLong_FromSize_t(mod_globs.thread_states_to_destroy.size());
+    LockGuard cleanup_lock(*mod_globs->thread_states_to_destroy_lock);
+    return PyLong_FromSize_t(mod_globs->thread_states_to_destroy.size());
 }
 
 PyDoc_STRVAR(mod_get_total_main_greenlets_doc,
              "get_total_main_greenlets() -> Integer\n"
              "\n"
              "Quickly return the number of main greenlets that exist. Testing only.\n");
 
@@ -3088,15 +3001,20 @@
              "get_tstate_trash_delete_nesting() -> Integer\n"
              "\n"
              "Return the 'trash can' nesting level. Testing only.\n");
 static PyObject*
 mod_get_tstate_trash_delete_nesting(PyObject* UNUSED(module))
 {
     PyThreadState* tstate = PyThreadState_GET();
+
+#if GREENLET_PY312
+    return PyLong_FromLong(tstate->trash.delete_nesting);
+#else
     return PyLong_FromLong(tstate->trash_delete_nesting);
+#endif
 }
 
 static PyMethodDef GreenMethods[] = {
     {"getcurrent",
      (PyCFunction)mod_getcurrent,
      METH_NOARGS,
      mod_getcurrent_doc},
@@ -3127,41 +3045,34 @@
     -1,
     GreenMethods,
 };
 
 
 
 static PyObject*
-greenlet_internal_mod_init() G_NOEXCEPT
+greenlet_internal_mod_init() noexcept
 {
     static void* _PyGreenlet_API[PyGreenlet_API_pointers];
-    GREENLET_NOINLINE_INIT();
 
     try {
         CreatedModule m(greenlet_module_def);
 
         Require(PyType_Ready(&PyGreenlet_Type));
 
-#if G_USE_STANDARD_THREADING == 0
-        Require(PyType_Ready(&PyGreenletCleanup_Type));
-#endif
-
-        new((void*)&mod_globs) GreenletGlobals;
+        mod_globs = new GreenletGlobals;
         ThreadState::init();
 
         m.PyAddObject("greenlet", PyGreenlet_Type);
-        m.PyAddObject("error", mod_globs.PyExc_GreenletError);
-        m.PyAddObject("GreenletExit", mod_globs.PyExc_GreenletExit);
+        m.PyAddObject("error", mod_globs->PyExc_GreenletError);
+        m.PyAddObject("GreenletExit", mod_globs->PyExc_GreenletExit);
 
         m.PyAddObject("GREENLET_USE_GC", 1);
         m.PyAddObject("GREENLET_USE_TRACING", 1);
-        // The macros are eithre 0 or 1; the 0 case can be interpreted
-        // the same as NULL, which is ambiguous with a pointer.
-        m.PyAddObject("GREENLET_USE_CONTEXT_VARS", (long)GREENLET_PY37);
-        m.PyAddObject("GREENLET_USE_STANDARD_THREADING", (long)G_USE_STANDARD_THREADING);
+        m.PyAddObject("GREENLET_USE_CONTEXT_VARS", 1L);
+        m.PyAddObject("GREENLET_USE_STANDARD_THREADING", 1L);
 
         OwnedObject clocks_per_sec = OwnedObject::consuming(PyLong_FromSsize_t(CLOCKS_PER_SEC));
         m.PyAddObject("CLOCKS_PER_SEC", clocks_per_sec);
 
         /* also publish module-level data as attributes of the greentype. */
         // XXX: This is weird, and enables a strange pattern of
         // confusing the class greenlet with the module greenlet; with
@@ -3176,16 +3087,16 @@
          * Expose C API
          */
 
         /* types */
         _PyGreenlet_API[PyGreenlet_Type_NUM] = (void*)&PyGreenlet_Type;
 
         /* exceptions */
-        _PyGreenlet_API[PyExc_GreenletError_NUM] = (void*)mod_globs.PyExc_GreenletError;
-        _PyGreenlet_API[PyExc_GreenletExit_NUM] = (void*)mod_globs.PyExc_GreenletExit;
+        _PyGreenlet_API[PyExc_GreenletError_NUM] = (void*)mod_globs->PyExc_GreenletError;
+        _PyGreenlet_API[PyExc_GreenletExit_NUM] = (void*)mod_globs->PyExc_GreenletExit;
 
         /* methods */
         _PyGreenlet_API[PyGreenlet_New_NUM] = (void*)PyGreenlet_New;
         _PyGreenlet_API[PyGreenlet_GetCurrent_NUM] = (void*)PyGreenlet_GetCurrent;
         _PyGreenlet_API[PyGreenlet_Throw_NUM] = (void*)PyGreenlet_Throw;
         _PyGreenlet_API[PyGreenlet_Switch_NUM] = (void*)PyGreenlet_Switch;
         _PyGreenlet_API[PyGreenlet_SetParent_NUM] = (void*)PyGreenlet_SetParent;
@@ -3230,27 +3141,21 @@
     catch (const PyErrOccurred&) {
         return NULL;
     }
 
 }
 
 extern "C" {
-#if PY_MAJOR_VERSION >= 3
+
 PyMODINIT_FUNC
 PyInit__greenlet(void)
 {
     return greenlet_internal_mod_init();
 }
-#else
-PyMODINIT_FUNC
-init_greenlet(void)
-{
-    greenlet_internal_mod_init();
-}
-#endif
-};
+
+}; // extern C
 
 #ifdef __clang__
 #    pragma clang diagnostic pop
 #elif defined(__GNUC__)
 #    pragma GCC diagnostic pop
 #endif
```

### Comparing `greenlet-2.0.2/src/greenlet/greenlet.h` & `greenlet-3.0.0a1/src/greenlet/greenlet.h`

 * *Files identical despite different names*

### Comparing `greenlet-2.0.2/src/greenlet/greenlet_allocator.hpp` & `greenlet-3.0.0a1/src/greenlet/greenlet_allocator.hpp`

 * *Files identical despite different names*

### Comparing `greenlet-2.0.2/src/greenlet/greenlet_compiler_compat.hpp` & `greenlet-3.0.0a1/src/greenlet/greenlet_compiler_compat.hpp`

 * *Files 19% similar despite different names*

```diff
@@ -1,132 +1,95 @@
 /* -*- indent-tabs-mode: nil; tab-width: 4; -*- */
 #ifndef GREENLET_COMPILER_COMPAT_HPP
 #define GREENLET_COMPILER_COMPAT_HPP
 
 /**
  * Definitions to aid with compatibility with different compilers.
  *
- * .. caution:: Use extreme care with G_NOEXCEPT.
+ * .. caution:: Use extreme care with noexcept.
  * Some compilers and runtimes, specifically gcc/libgcc/libstdc++ on
  * Linux, implement stack unwinding by throwing an uncatchable
  * exception, one that specifically does not appear to be an active
- * exception to the rest of the runtime. If this happens while we're in a G_NOEXCEPT function,
+ * exception to the rest of the runtime. If this happens while we're in a noexcept function,
  * we have violated our dynamic exception contract, and so the runtime
  * will call std::terminate(), which kills the process with the
  * unhelpful message "terminate called without an active exception".
  *
  * This has happened in this scenario: A background thread is running
  * a greenlet that has made a native call and released the GIL.
  * Meanwhile, the main thread finishes and starts shutting down the
  * interpreter. When the background thread is scheduled again and
  * attempts to obtain the  GIL, it notices that the interpreter is
  * exiting and calls ``pthread_exit()``. This in turn starts to unwind
  * the stack by throwing that exception. But we had the ``PyCall``
- * functions annotated as G_NOEXCEPT, so the runtime terminated us.
+ * functions annotated as noexcept, so the runtime terminated us.
  *
  * #2  0x00007fab26fec2b7 in std::terminate() () from /lib/x86_64-linux-gnu/libstdc++.so.6
  * #3  0x00007fab26febb3c in __gxx_personality_v0 () from /lib/x86_64-linux-gnu/libstdc++.so.6
  * #4  0x00007fab26f34de6 in ?? () from /lib/x86_64-linux-gnu/libgcc_s.so.1
  * #6  0x00007fab276a34c6 in __GI___pthread_unwind  at ./nptl/unwind.c:130
  * #7  0x00007fab2769bd3a in __do_cancel () at ../sysdeps/nptl/pthreadP.h:280
  * #8  __GI___pthread_exit (value=value@entry=0x0) at ./nptl/pthread_exit.c:36
  * #9  0x000000000052e567 in PyThread_exit_thread () at ../Python/thread_pthread.h:370
  * #10 0x00000000004d60b5 in take_gil at ../Python/ceval_gil.h:224
  * #11 0x00000000004d65f9 in PyEval_RestoreThread  at ../Python/ceval.c:467
  * #12 0x000000000060cce3 in setipaddr  at ../Modules/socketmodule.c:1203
  * #13 0x00000000006101cd in socket_gethostbyname
  */
 
-
-/* The compiler used for Python 2.7 on Windows doesn't include
-   either stdint.h or cstdint.h. Nor does it understand nullptr or have
-   std::shared_ptr. = delete, etc Sigh. */
-#if defined(_MSC_VER) &&  _MSC_VER <= 1500
-typedef unsigned long long uint64_t;
-typedef signed long long int64_t;
-typedef unsigned int uint32_t;
-// C++ defines NULL to be 0, which is ambiguous
-// with an integer in certain cases, and won't autoconvert to a
-// pointer in other cases.
-#define nullptr NULL
-#define G_HAS_METHOD_DELETE 0
-// Use G_EXPLICIT_OP as the prefix for operator methods
-// that should be explicit. Old MSVC doesn't support explicit operator
-// methods.
-#define G_EXPLICIT_OP
-#define G_NOEXCEPT throw()
-// This version doesn't support "objects with internal linkage"
-// in non-type template arguments. Translation: function pointer
-// template arguments cannot be for static functions.
-#define G_FP_TMPL_STATIC
-#else
-// Newer, reasonable compilers implementing C++11 or so.
 #include <cstdint>
-#define G_HAS_METHOD_DELETE 1
-#define G_EXPLICIT_OP explicit
-#define G_NOEXCEPT noexcept
+
 # if defined(__clang__)
 #  define G_FP_TMPL_STATIC static
 # else
 // GCC has no problem allowing static function pointers, but emits
 // tons of warnings about "whose type uses the anonymous namespace [-Wsubobject-linkage]"
 #  define G_FP_TMPL_STATIC
 # endif
 
-#endif
-
-#if G_HAS_METHOD_DELETE == 1
 #    define G_NO_COPIES_OF_CLS(Cls) private:     \
     Cls(const Cls& other) = delete; \
     Cls& operator=(const Cls& other) = delete
 
 #    define G_NO_ASSIGNMENT_OF_CLS(Cls) private:  \
     Cls& operator=(const Cls& other) = delete
 
 #    define G_NO_COPY_CONSTRUCTOR_OF_CLS(Cls) private: \
     Cls(const Cls& other) = delete;
-#else
-#    define G_NO_COPIES_OF_CLS(Cls) private: \
-    Cls(const Cls& other); \
-    Cls& operator=(const Cls& other)
 
-#    define G_NO_ASSIGNMENT_OF_CLS(Cls) private: \
-        Cls& operator=(const Cls& other)
-
-#    define G_NO_COPY_CONSTRUCTOR_OF_CLS(Cls) private: \
-    Cls(const Cls& other);
-#endif
 
 // CAUTION: MSVC is stupidly picky:
 //
 // "The compiler ignores, without warning, any __declspec keywords
 // placed after * or & and in front of the variable identifier in a
 // declaration."
 // (https://docs.microsoft.com/en-us/cpp/cpp/declspec?view=msvc-160)
 //
 // So pointer return types must be handled differently (because of the
 // trailing *), or you get inscrutable compiler warnings like "error
 // C2059: syntax error: ''"
+//
+// In C++ 11, there is a standard syntax for attributes, and
+// GCC defines an attribute to use with this: [[gnu:noinline]].
+// In the future, this is expected to become standard.
 
 #if defined(__GNUC__) || defined(__clang__)
 /* We used to check for GCC 4+ or 3.4+, but those compilers are
    laughably out of date. Just assume they support it. */
-#    define GREENLET_NOINLINE_SUPPORTED
 #    define GREENLET_NOINLINE(name) __attribute__((noinline)) name
 #    define GREENLET_NOINLINE_P(rtype, name) rtype __attribute__((noinline)) name
 #    define UNUSED(x) UNUSED_ ## x __attribute__((__unused__))
 #elif defined(_MSC_VER)
 /* We used to check for  && (_MSC_VER >= 1300) but that's also out of date. */
-#    define GREENLET_NOINLINE_SUPPORTED
 #    define GREENLET_NOINLINE(name) __declspec(noinline) name
 #    define GREENLET_NOINLINE_P(rtype, name) __declspec(noinline) rtype name
 #    define UNUSED(x) UNUSED_ ## x
 #endif
 
 #if defined(_MSC_VER)
-#    define G_NOEXCEPT_WIN32 G_NOEXCEPT
+#    define G_NOEXCEPT_WIN32 noexcept
 #else
 #    define G_NOEXCEPT_WIN32
 #endif
 
 
 #endif
```

### Comparing `greenlet-2.0.2/src/greenlet/greenlet_exceptions.hpp` & `greenlet-3.0.0a1/src/greenlet/greenlet_exceptions.hpp`

 * *Files identical despite different names*

### Comparing `greenlet-2.0.2/src/greenlet/greenlet_greenlet.hpp` & `greenlet-3.0.0a1/src/greenlet/greenlet_greenlet.hpp`

 * *Files 10% similar despite different names*

```diff
@@ -28,47 +28,34 @@
 namespace greenlet
 {
     class ExceptionState
     {
     private:
         G_NO_COPIES_OF_CLS(ExceptionState);
 
-#if PY_VERSION_HEX >= 0x030700A3
         // Even though these are borrowed objects, we actually own
         // them, when they're not null.
         // XXX: Express that in the API.
     private:
         _PyErr_StackItem* exc_info;
         _PyErr_StackItem exc_state;
-#else
-        OwnedObject exc_value;
-#if !GREENLET_PY311
-        OwnedObject exc_type;
-        OwnedObject exc_traceback;
-#endif
-#endif
     public:
         ExceptionState();
-        void operator<<(const PyThreadState *const tstate) G_NOEXCEPT;
-        void operator>>(PyThreadState* tstate) G_NOEXCEPT;
-        void clear() G_NOEXCEPT;
+        void operator<<(const PyThreadState *const tstate) noexcept;
+        void operator>>(PyThreadState* tstate) noexcept;
+        void clear() noexcept;
 
-        int tp_traverse(visitproc visit, void* arg) G_NOEXCEPT;
-        void tp_clear() G_NOEXCEPT;
+        int tp_traverse(visitproc visit, void* arg) noexcept;
+        void tp_clear() noexcept;
     };
 
     template<typename T>
     void operator<<(const PyThreadState *const tstate, T& exc);
 
-    template<typename IsPy37>
     class PythonStateContext
-    {};
-
-    template<>
-    class PythonStateContext<GREENLET_WHEN_PY37>
     {
     protected:
         greenlet::refs::OwnedContext _context;
     public:
         inline const greenlet::refs::OwnedContext& context() const
         {
             return this->_context;
@@ -93,45 +80,15 @@
         inline static void context(T* tstate, PyObject* new_context)
         {
             tstate->context = new_context;
             tstate->context_ver++;
         }
     };
 
-
-    template<>
-    class PythonStateContext<GREENLET_WHEN_NOT_PY37>
-    {
-    public:
-        inline const greenlet::refs::OwnedContext& context() const
-        {
-            throw AttributeError("no context");
-        }
-
-        inline greenlet::refs::OwnedContext& context()
-        {
-            throw AttributeError("no context");
-        }
-
-        inline void tp_clear(){};
-
-        template<typename T>
-        inline static PyObject* context(T* UNUSED(tstate))
-        {
-            throw PyFatalError("This should never be called.");
-        }
-
-        template<typename T>
-        inline static void context(T* UNUSED(tstate), PyObject* UNUSED(new_context))
-        {
-            throw PyFatalError("This should never be called.");
-        }
-    };
-
-    class PythonState : public PythonStateContext<G_IS_PY37>
+    class PythonState : public PythonStateContext
     {
     public:
         typedef greenlet::refs::OwnedReference<struct _frame> OwnedFrame;
     private:
         G_NO_COPIES_OF_CLS(PythonState);
         // We own this if we're suspended (although currently we don't
         // tp_traverse into it; that's a TODO). If we're running, it's
@@ -139,42 +96,47 @@
         // won't be reachable from the place that normally decref's
         // it, so we need to do it (hence owning it).
         OwnedFrame _top_frame;
 #if GREENLET_USE_CFRAME
         _PyCFrame* cframe;
         int use_tracing;
 #endif
+#if GREENLET_PY312
+        int py_recursion_depth;
+        int c_recursion_depth;
+#else
         int recursion_depth;
+#endif
         int trash_delete_nesting;
 #if GREENLET_PY311
         _PyInterpreterFrame* current_frame;
         _PyStackChunk* datastack_chunk;
         PyObject** datastack_top;
         PyObject** datastack_limit;
 #endif
 
     public:
         PythonState();
         // You can use this for testing whether we have a frame
         // or not. It returns const so they can't modify it.
-        const OwnedFrame& top_frame() const G_NOEXCEPT;
+        const OwnedFrame& top_frame() const noexcept;
 
 
-        void operator<<(const PyThreadState *const tstate) G_NOEXCEPT;
-        void operator>>(PyThreadState* tstate) G_NOEXCEPT;
-        void clear() G_NOEXCEPT;
+        void operator<<(const PyThreadState *const tstate) noexcept;
+        void operator>>(PyThreadState* tstate) noexcept;
+        void clear() noexcept;
 
-        int tp_traverse(visitproc visit, void* arg, bool visit_top_frame) G_NOEXCEPT;
-        void tp_clear(bool own_top_frame) G_NOEXCEPT;
-        void set_initial_state(const PyThreadState* const tstate) G_NOEXCEPT;
+        int tp_traverse(visitproc visit, void* arg, bool visit_top_frame) noexcept;
+        void tp_clear(bool own_top_frame) noexcept;
+        void set_initial_state(const PyThreadState* const tstate) noexcept;
 #if GREENLET_USE_CFRAME
-        void set_new_cframe(_PyCFrame& frame) G_NOEXCEPT;
+        void set_new_cframe(_PyCFrame& frame) noexcept;
 #endif
-        void will_switch_from(PyThreadState *const origin_tstate) G_NOEXCEPT;
-        void did_finish(PyThreadState* tstate) G_NOEXCEPT;
+        void will_switch_from(PyThreadState *const origin_tstate) noexcept;
+        void did_finish(PyThreadState* tstate) noexcept;
     };
 
     class StackState
     {
         // By having only plain C (POD) members, no virtual functions
         // or bases, we get a trivial assignment operator generated
         // for us. However, that's not safe since we do manage memory.
@@ -184,40 +146,40 @@
         // object small)
     private:
         char* _stack_start;
         char* stack_stop;
         char* stack_copy;
         intptr_t _stack_saved;
         StackState* stack_prev;
-        inline int copy_stack_to_heap_up_to(const char* const stop) G_NOEXCEPT;
-        inline void free_stack_copy() G_NOEXCEPT;
+        inline int copy_stack_to_heap_up_to(const char* const stop) noexcept;
+        inline void free_stack_copy() noexcept;
 
     public:
         /**
          * Creates a started, but inactive, state, using *current*
          * as the previous.
          */
         StackState(void* mark, StackState& current);
         /**
          * Creates an inactive, unstarted, state.
          */
         StackState();
         ~StackState();
         StackState(const StackState& other);
         StackState& operator=(const StackState& other);
-        inline void copy_heap_to_stack(const StackState& current) G_NOEXCEPT;
-        inline int copy_stack_to_heap(char* const stackref, const StackState& current) G_NOEXCEPT;
-        inline bool started() const G_NOEXCEPT;
-        inline bool main() const G_NOEXCEPT;
-        inline bool active() const G_NOEXCEPT;
-        inline void set_active() G_NOEXCEPT;
-        inline void set_inactive() G_NOEXCEPT;
-        inline intptr_t stack_saved() const G_NOEXCEPT;
-        inline char* stack_start() const G_NOEXCEPT;
-        static inline StackState make_main() G_NOEXCEPT;
+        inline void copy_heap_to_stack(const StackState& current) noexcept;
+        inline int copy_stack_to_heap(char* const stackref, const StackState& current) noexcept;
+        inline bool started() const noexcept;
+        inline bool main() const noexcept;
+        inline bool active() const noexcept;
+        inline void set_active() noexcept;
+        inline void set_inactive() noexcept;
+        inline intptr_t stack_saved() const noexcept;
+        inline char* stack_start() const noexcept;
+        static inline StackState make_main() noexcept;
 #ifdef GREENLET_USE_STDIO
         friend std::ostream& operator<<(std::ostream& os, const StackState& s);
 #endif
     };
 #ifdef GREENLET_USE_STDIO
     std::ostream& operator<<(std::ostream& os, const StackState& s);
 #endif
@@ -289,15 +251,15 @@
             this->_args = args;
             this->_kwargs.CLEAR();
             args.CLEAR();
 
             return *this;
         }
 
-        G_EXPLICIT_OP operator bool() const G_NOEXCEPT
+        explicit operator bool() const noexcept
         {
             return this->_args || this->_kwargs;
         }
 
         inline void CLEAR()
         {
             this->_args.CLEAR();
@@ -325,38 +287,36 @@
         StackState stack_state;
         PythonState python_state;
         Greenlet(PyGreenlet* p, const StackState& initial_state);
     public:
         Greenlet(PyGreenlet* p);
         virtual ~Greenlet();
 
-        template <typename IsPy37> // maybe we can use a value here?
-        const OwnedObject context(const typename IsPy37::IsIt=nullptr) const;
+        const OwnedObject context() const;
 
-        template <typename IsPy37>
-        inline void context(refs::BorrowedObject new_context, typename IsPy37::IsIt=nullptr);
+        inline void context(refs::BorrowedObject new_context);
 
         inline SwitchingArgs& args()
         {
             return this->switch_args;
         }
 
         virtual const refs::BorrowedMainGreenlet main_greenlet() const = 0;
 
-        inline intptr_t stack_saved() const G_NOEXCEPT
+        inline intptr_t stack_saved() const noexcept
         {
             return this->stack_state.stack_saved();
         }
 
         // This is used by the macro SLP_SAVE_STATE to compute the
         // difference in stack sizes. It might be nice to handle the
         // computation ourself, but the type of the result
         // varies by platform, so doing it in the macro is the
         // simplest way.
-        inline const char* stack_start() const G_NOEXCEPT
+        inline const char* stack_start() const noexcept
         {
             return this->stack_state.stack_start();
         }
 
         virtual OwnedObject throw_GreenletExit_during_dealloc(const ThreadState& current_thread_state);
         virtual OwnedObject g_switch() = 0;
         /**
@@ -382,16 +342,16 @@
         // The thread may or may not be the same thread the greenlet
         // was running in.
         // The thread state will be null if the thread the greenlet
         // was running in was known to have exited.
         void deallocing_greenlet_in_thread(const ThreadState* current_state);
 
         // TODO: Figure out how to make these non-public.
-        inline void slp_restore_state() G_NOEXCEPT;
-        inline int slp_save_state(char *const stackref) G_NOEXCEPT;
+        inline void slp_restore_state() noexcept;
+        inline int slp_save_state(char *const stackref) noexcept;
 
         inline bool is_currently_running_in_some_thread() const;
         virtual bool belongs_to_thread(const ThreadState* state) const;
 
         inline bool started() const
         {
             return this->stack_state.started();
@@ -421,23 +381,23 @@
         virtual int tp_traverse(visitproc visit, void* arg);
         virtual int tp_clear();
 
 
         // Return the thread state that the greenlet is running in, or
         // null if the greenlet is not running or the thread is known
         // to have exited.
-        virtual ThreadState* thread_state() const G_NOEXCEPT = 0;
+        virtual ThreadState* thread_state() const noexcept = 0;
 
         // Return true if the greenlet is known to have been running
         // (active) in a thread that has now exited.
-        virtual bool was_running_in_dead_thread() const G_NOEXCEPT = 0;
+        virtual bool was_running_in_dead_thread() const noexcept = 0;
 
         // Return a borrowed greenlet that is the Python object
         // this object represents.
-        virtual BorrowedGreenlet self() const G_NOEXCEPT = 0;
+        virtual BorrowedGreenlet self() const noexcept = 0;
 
     protected:
         inline void release_args();
 
         // The functions that must not be inlined are declared virtual.
         // We also mark them as protected, not private, so that the
         // compiler is forced to call them through a function pointer.
@@ -483,15 +443,15 @@
                 this->the_state_that_switched = other.the_state_that_switched;
                 this->origin_greenlet = other.origin_greenlet;
                 return *this;
             }
         };
 
         // Returns the previous greenlet we just switched away from.
-        virtual OwnedGreenlet g_switchstack_success() G_NOEXCEPT;
+        virtual OwnedGreenlet g_switchstack_success() noexcept;
 
 
         // Check the preconditions for switching to this greenlet; if they
         // aren't met, throws PyErrOccurred. Most callers will want to
         // catch this and clear the arguments
         inline void check_switch_allowed() const;
         class GreenletStartedWhileInPython : public std::runtime_error
@@ -554,16 +514,16 @@
         static void* operator new(size_t UNUSED(count));
         static void operator delete(void* ptr);
 
         UserGreenlet(PyGreenlet* p, BorrowedGreenlet the_parent);
         virtual ~UserGreenlet();
 
         virtual refs::BorrowedMainGreenlet find_main_greenlet_in_lineage() const;
-        virtual bool was_running_in_dead_thread() const G_NOEXCEPT;
-        virtual ThreadState* thread_state() const G_NOEXCEPT;
+        virtual bool was_running_in_dead_thread() const noexcept;
+        virtual ThreadState* thread_state() const noexcept;
         virtual OwnedObject g_switch();
         virtual const OwnedObject& run() const
         {
             if (this->started() || !this->_run_callable) {
                 throw AttributeError("run");
             }
             return this->_run_callable;
@@ -571,15 +531,15 @@
         virtual void run(const refs::BorrowedObject nrun);
 
         virtual const OwnedGreenlet parent() const;
         virtual void parent(const refs::BorrowedObject new_parent);
 
         virtual const refs::BorrowedMainGreenlet main_greenlet() const;
 
-        virtual BorrowedGreenlet self() const G_NOEXCEPT;
+        virtual BorrowedGreenlet self() const noexcept;
         virtual void murder_in_place();
         virtual bool belongs_to_thread(const ThreadState* state) const;
         virtual int tp_traverse(visitproc visit, void* arg);
         virtual int tp_clear();
         class ParentIsCurrentGuard
         {
         private:
@@ -617,19 +577,19 @@
 
         virtual const OwnedGreenlet parent() const;
         virtual void parent(const refs::BorrowedObject new_parent);
 
         virtual const refs::BorrowedMainGreenlet main_greenlet() const;
 
         virtual refs::BorrowedMainGreenlet find_main_greenlet_in_lineage() const;
-        virtual bool was_running_in_dead_thread() const G_NOEXCEPT;
-        virtual ThreadState* thread_state() const G_NOEXCEPT;
-        void thread_state(ThreadState*) G_NOEXCEPT;
+        virtual bool was_running_in_dead_thread() const noexcept;
+        virtual ThreadState* thread_state() const noexcept;
+        void thread_state(ThreadState*) noexcept;
         virtual OwnedObject g_switch();
-        virtual BorrowedGreenlet self() const G_NOEXCEPT;
+        virtual BorrowedGreenlet self() const noexcept;
         virtual int tp_traverse(visitproc visit, void* arg);
     };
 
 };
 
 template<typename T>
 void greenlet::operator<<(const PyThreadState *const lhs, T& rhs)
@@ -642,98 +602,98 @@
 ExceptionState::ExceptionState()
 {
     this->clear();
 }
 
 #if PY_VERSION_HEX >= 0x030700A3
 // ******** Python 3.7 and above *********
-void ExceptionState::operator<<(const PyThreadState *const tstate) G_NOEXCEPT
+void ExceptionState::operator<<(const PyThreadState *const tstate) noexcept
 {
     this->exc_info = tstate->exc_info;
     this->exc_state = tstate->exc_state;
 }
 
-void ExceptionState::operator>>(PyThreadState *const tstate) G_NOEXCEPT
+void ExceptionState::operator>>(PyThreadState *const tstate) noexcept
 {
     tstate->exc_state = this->exc_state;
     tstate->exc_info =
         this->exc_info ? this->exc_info : &tstate->exc_state;
     this->clear();
 }
 
-void ExceptionState::clear() G_NOEXCEPT
+void ExceptionState::clear() noexcept
 {
     this->exc_info = nullptr;
     this->exc_state.exc_value = nullptr;
 #if !GREENLET_PY311
     this->exc_state.exc_type = nullptr;
     this->exc_state.exc_traceback = nullptr;
 #endif
     this->exc_state.previous_item = nullptr;
 }
 
-int ExceptionState::tp_traverse(visitproc visit, void* arg) G_NOEXCEPT
+int ExceptionState::tp_traverse(visitproc visit, void* arg) noexcept
 {
     Py_VISIT(this->exc_state.exc_value);
 #if !GREENLET_PY311
     Py_VISIT(this->exc_state.exc_type);
     Py_VISIT(this->exc_state.exc_traceback);
 #endif
     return 0;
 }
 
-void ExceptionState::tp_clear() G_NOEXCEPT
+void ExceptionState::tp_clear() noexcept
 {
     Py_CLEAR(this->exc_state.exc_value);
 #if !GREENLET_PY311
     Py_CLEAR(this->exc_state.exc_type);
     Py_CLEAR(this->exc_state.exc_traceback);
 #endif
 }
 #else
 // ********** Python 3.6 and below ********
-void ExceptionState::operator<<(const PyThreadState *const tstate) G_NOEXCEPT
+void ExceptionState::operator<<(const PyThreadState *const tstate) noexcept
 {
     this->exc_value.steal(tstate->exc_value);
 #if !GREENLET_PY311
     this->exc_type.steal(tstate->exc_type);
     this->exc_traceback.steal(tstate->exc_traceback);
 #endif
 }
 
-void ExceptionState::operator>>(PyThreadState *const tstate) G_NOEXCEPT
+void ExceptionState::operator>>(PyThreadState *const tstate) noexcept
 {
     tstate->exc_value <<= this->exc_value;
 #if !GREENLET_PY311
     tstate->exc_type <<= this->exc_type;
     tstate->exc_traceback <<= this->exc_traceback;
 #endif
     this->clear();
 }
 
-void ExceptionState::clear() G_NOEXCEPT
+void ExceptionState::clear() noexcept
 {
     this->exc_value = nullptr;
 #if !GREENLET_PY311
     this->exc_type = nullptr;
     this->exc_traceback = nullptr;
 #endif
 }
 
-int ExceptionState::tp_traverse(visitproc visit, void* arg) G_NOEXCEPT
+int ExceptionState::tp_traverse(visitproc visit, void* arg) noexcept
 {
     Py_VISIT(this->exc_value.borrow());
 #if !GREENLET_PY311
     Py_VISIT(this->exc_type.borrow());
     Py_VISIT(this->exc_traceback.borrow());
 #endif
     return 0;
 }
 
-void ExceptionState::tp_clear() G_NOEXCEPT
+void ExceptionState::tp_clear() noexcept
 {
     this->exc_value.CLEAR();
 #if !GREENLET_PY311
     this->exc_type.CLEAR();
     this->exc_traceback.CLEAR();
 #endif
 }
@@ -744,15 +704,20 @@
 
 PythonState::PythonState()
     : _top_frame()
 #if GREENLET_USE_CFRAME
     ,cframe(nullptr)
     ,use_tracing(0)
 #endif
+#if GREENLET_PY312
+    ,py_recursion_depth(0)
+    ,c_recursion_depth(0)
+#else
     ,recursion_depth(0)
+#endif
     ,trash_delete_nesting(0)
 #if GREENLET_PY311
     ,current_frame(nullptr)
     ,datastack_chunk(nullptr)
     ,datastack_top(nullptr)
     ,datastack_limit(nullptr)
 #endif
@@ -807,147 +772,169 @@
       dealloc in another thread? (Is that even possible if we're still
       running and haven't returned from g_initialstub?)
     */
     this->cframe = &PyThreadState_GET()->root_cframe;
 #endif
 }
 
-void PythonState::operator<<(const PyThreadState *const tstate) G_NOEXCEPT
+void PythonState::operator<<(const PyThreadState *const tstate) noexcept
 {
-#if GREENLET_PY37
     this->_context.steal(tstate->context);
-#endif
 #if GREENLET_USE_CFRAME
     /*
       IMPORTANT: ``cframe`` is a pointer into the STACK. Thus, because
       the call to ``slp_switch()`` changes the contents of the stack,
       you cannot read from ``ts_current->cframe`` after that call and
       necessarily get the same values you get from reading it here.
       Anything you need to restore from now to then must be saved in a
       global/threadlocal variable (because we can't use stack
       variables here either). For things that need to persist across
       the switch, use `will_switch_from`.
     */
     this->cframe = tstate->cframe;
+  #if !GREENLET_PY312
     this->use_tracing = tstate->cframe->use_tracing;
-#endif
+  #endif
+#endif // GREENLET_USE_CFRAME
 #if GREENLET_PY311
+  #if GREENLET_PY312
+    this->py_recursion_depth = tstate->py_recursion_limit - tstate->py_recursion_remaining;
+    this->c_recursion_depth = C_RECURSION_LIMIT - tstate->c_recursion_remaining;
+  #else // not 312
     this->recursion_depth = tstate->recursion_limit - tstate->recursion_remaining;
+  #endif // GREENLET_PY312
     this->current_frame = tstate->cframe->current_frame;
     this->datastack_chunk = tstate->datastack_chunk;
     this->datastack_top = tstate->datastack_top;
     this->datastack_limit = tstate->datastack_limit;
     PyFrameObject *frame = PyThreadState_GetFrame((PyThreadState *)tstate);
     Py_XDECREF(frame);  // PyThreadState_GetFrame gives us a new reference.
     this->_top_frame.steal(frame);
-#else
+  #if GREENLET_PY312
+    this->trash_delete_nesting = tstate->trash.delete_nesting;
+  #else // not 312
+    this->trash_delete_nesting = tstate->trash_delete_nesting;
+  #endif // GREENLET_PY312
+#else // Not 311
     this->recursion_depth = tstate->recursion_depth;
     this->_top_frame.steal(tstate->frame);
-#endif
-
-    // All versions of Python.
     this->trash_delete_nesting = tstate->trash_delete_nesting;
+#endif // GREENLET_PY311
 }
 
-void PythonState::operator>>(PyThreadState *const tstate) G_NOEXCEPT
+void PythonState::operator>>(PyThreadState *const tstate) noexcept
 {
-#if GREENLET_PY37
     tstate->context = this->_context.relinquish_ownership();
     /* Incrementing this value invalidates the contextvars cache,
        which would otherwise remain valid across switches */
     tstate->context_ver++;
-#endif
 #if GREENLET_USE_CFRAME
     tstate->cframe = this->cframe;
     /*
       If we were tracing, we need to keep tracing.
       There should never be the possibility of hitting the
       root_cframe here. See note above about why we can't
       just copy this from ``origin->cframe->use_tracing``.
     */
+  #if !GREENLET_PY312
     tstate->cframe->use_tracing = this->use_tracing;
-#endif
+  #endif
+#endif // GREENLET_USE_CFRAME
 #if GREENLET_PY311
+  #if GREENLET_PY312
+    tstate->py_recursion_remaining = tstate->py_recursion_limit - this->py_recursion_depth;
+    tstate->c_recursion_remaining = C_RECURSION_LIMIT - this->c_recursion_depth;
+  #else // not 3.12
     tstate->recursion_remaining = tstate->recursion_limit - this->recursion_depth;
+  #endif
     tstate->cframe->current_frame = this->current_frame;
     tstate->datastack_chunk = this->datastack_chunk;
     tstate->datastack_top = this->datastack_top;
     tstate->datastack_limit = this->datastack_limit;
     this->_top_frame.relinquish_ownership();
-#else
+  #if GREENLET_PY312
+    tstate->trash.delete_nesting = this->trash_delete_nesting;
+  #else // not 3.12
+    tstate->trash_delete_nesting = this->trash_delete_nesting;
+  #endif // GREENLET_PY312
+#else // not 3.11
     tstate->frame = this->_top_frame.relinquish_ownership();
     tstate->recursion_depth = this->recursion_depth;
-#endif
-    // All versions of Python.
     tstate->trash_delete_nesting = this->trash_delete_nesting;
+#endif // GREENLET_PY311
 }
 
-void PythonState::will_switch_from(PyThreadState *const origin_tstate) G_NOEXCEPT
+void PythonState::will_switch_from(PyThreadState *const origin_tstate) noexcept
 {
-#if GREENLET_USE_CFRAME
+#if GREENLET_USE_CFRAME && !GREENLET_PY312
     // The weird thing is, we don't actually save this for an
     // effect on the current greenlet, it's saved for an
     // effect on the target greenlet. That is, we want
     // continuity of this setting across the greenlet switch.
     this->use_tracing = origin_tstate->cframe->use_tracing;
 #endif
 }
 
-void PythonState::set_initial_state(const PyThreadState* const tstate) G_NOEXCEPT
+void PythonState::set_initial_state(const PyThreadState* const tstate) noexcept
 {
     this->_top_frame = nullptr;
-#if GREENLET_PY311
+#if GREENLET_PY312
+    this->py_recursion_depth = tstate->py_recursion_limit - tstate->py_recursion_remaining;
+    // XXX: TODO: Comment from a reviewer:
+    //     Should this be ``C_RECURSION_LIMIT - tstate->c_recursion_remaining``?
+    // But to me it looks more like that might not be the right
+    // initialization either?
+    this->c_recursion_depth = tstate->py_recursion_limit - tstate->py_recursion_remaining;
+#elif GREENLET_PY311
     this->recursion_depth = tstate->recursion_limit - tstate->recursion_remaining;
 #else
     this->recursion_depth = tstate->recursion_depth;
 #endif
 }
 // TODO: Better state management about when we own the top frame.
-int PythonState::tp_traverse(visitproc visit, void* arg, bool own_top_frame) G_NOEXCEPT
+int PythonState::tp_traverse(visitproc visit, void* arg, bool own_top_frame) noexcept
 {
-#if GREENLET_PY37
     Py_VISIT(this->_context.borrow());
-#endif
     if (own_top_frame) {
         Py_VISIT(this->_top_frame.borrow());
     }
     return 0;
 }
 
-void PythonState::tp_clear(bool own_top_frame) G_NOEXCEPT
+void PythonState::tp_clear(bool own_top_frame) noexcept
 {
     PythonStateContext::tp_clear();
     // If we get here owning a frame,
     // we got dealloc'd without being finished. We may or may not be
     // in the same thread.
     if (own_top_frame) {
         this->_top_frame.CLEAR();
     }
 }
 
 #if GREENLET_USE_CFRAME
-void PythonState::set_new_cframe(_PyCFrame& frame) G_NOEXCEPT
+void PythonState::set_new_cframe(_PyCFrame& frame) noexcept
 {
     frame = *PyThreadState_GET()->cframe;
     /* Make the target greenlet refer to the stack value. */
     this->cframe = &frame;
     /*
       And restore the link to the previous frame so this one gets
       unliked appropriately.
     */
     this->cframe->previous = &PyThreadState_GET()->root_cframe;
 }
 #endif
 
-const PythonState::OwnedFrame& PythonState::top_frame() const G_NOEXCEPT
+const PythonState::OwnedFrame& PythonState::top_frame() const noexcept
 {
     return this->_top_frame;
 }
 
-void PythonState::did_finish(PyThreadState* tstate) G_NOEXCEPT
+void PythonState::did_finish(PyThreadState* tstate) noexcept
 {
 #if GREENLET_PY311
     // See https://github.com/gevent/gevent/issues/1924 and
     // https://github.com/python-greenlet/greenlet/issues/328. In
     // short, Python 3.11 allocates memory for frames as a sort of
     // linked list that's kept as part of PyThreadState in the
     // ``datastack_chunk`` member and friends. These are saved and
@@ -1096,22 +1083,22 @@
     this->stack_stop = other.stack_stop;
     this->stack_copy = other.stack_copy;
     this->_stack_saved = other._stack_saved;
     this->stack_prev = other.stack_prev;
     return *this;
 }
 
-inline void StackState::free_stack_copy() G_NOEXCEPT
+inline void StackState::free_stack_copy() noexcept
 {
     PyMem_Free(this->stack_copy);
     this->stack_copy = nullptr;
     this->_stack_saved = 0;
 }
 
-inline void StackState::copy_heap_to_stack(const StackState& current) G_NOEXCEPT
+inline void StackState::copy_heap_to_stack(const StackState& current) noexcept
 {
     // cerr << "copy_heap_to_stack" << endl
     //      << "\tFrom    : " << *this << endl
     //      << "\tCurrent:" << current
     //      << endl;
     /* Restore the heap copy back into the C stack */
     if (this->_stack_saved != 0) {
@@ -1126,15 +1113,15 @@
         // cerr << "\tOwner: " << owner << endl;
         owner = owner->stack_prev; /* find greenlet with more stack */
     }
     this->stack_prev = owner;
     // cerr << "\tFinished with: " << *this << endl;
 }
 
-inline int StackState::copy_stack_to_heap_up_to(const char* const stop) G_NOEXCEPT
+inline int StackState::copy_stack_to_heap_up_to(const char* const stop) noexcept
 {
     /* Save more of g's stack into the heap -- at least up to 'stop'
        g->stack_stop |________|
                      |        |
                      |    __ stop       . . . . .
                      |        |    ==>  .       .
                      |________|          _______
@@ -1155,15 +1142,15 @@
         this->stack_copy = c;
         this->_stack_saved = sz2;
     }
     return 0;
 }
 
 inline int StackState::copy_stack_to_heap(char* const stackref,
-                                          const StackState& current) G_NOEXCEPT
+                                          const StackState& current) noexcept
 {
     // cerr << "copy_stack_to_heap: " << endl
     //      << "\tstackref: " << (void*)stackref << endl
     //      << "\tthis: " << *this << endl
     //      << "\tcurrent: " << current
     //      << endl;
     /* must free all the C stack up to target_stop */
@@ -1191,36 +1178,36 @@
         if (owner->copy_stack_to_heap_up_to(target_stop)) {
             return -1; /* XXX */
         }
     }
     return 0;
 }
 
-inline bool StackState::started() const G_NOEXCEPT
+inline bool StackState::started() const noexcept
 {
     return this->stack_stop != nullptr;
 }
 
-inline bool StackState::main() const G_NOEXCEPT
+inline bool StackState::main() const noexcept
 {
     return this->stack_stop == (char*)-1;
 }
 
-inline bool StackState::active() const G_NOEXCEPT
+inline bool StackState::active() const noexcept
 {
     return this->_stack_start != nullptr;
 }
 
-inline void StackState::set_active() G_NOEXCEPT
+inline void StackState::set_active() noexcept
 {
     assert(this->_stack_start == nullptr);
     this->_stack_start = (char*)1;
 }
 
-inline void StackState::set_inactive() G_NOEXCEPT
+inline void StackState::set_inactive() noexcept
 {
     this->_stack_start = nullptr;
     // XXX: What if we still have memory out there?
     // That case is actually triggered by
     // test_issue251_issue252_explicit_reference_not_collectable (greenlet.tests.test_leaks.TestLeaks)
     // and
     // test_issue251_issue252_need_to_collect_in_background
@@ -1230,26 +1217,26 @@
     // runs.
     // It *seems* safe to clean up the memory here?
     if (this->_stack_saved) {
         this->free_stack_copy();
     }
 }
 
-inline intptr_t StackState::stack_saved() const G_NOEXCEPT
+inline intptr_t StackState::stack_saved() const noexcept
 {
     return this->_stack_saved;
 }
 
-inline char* StackState::stack_start() const G_NOEXCEPT
+inline char* StackState::stack_start() const noexcept
 {
     return this->_stack_start;
 }
 
 
-inline StackState StackState::make_main() G_NOEXCEPT
+inline StackState StackState::make_main() noexcept
 {
     StackState s;
     s._stack_start = (char*)1;
     s.stack_stop = (char*)-1;
     return s;
 }
```

### Comparing `greenlet-2.0.2/src/greenlet/greenlet_internal.hpp` & `greenlet-3.0.0a1/src/greenlet/greenlet_internal.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -64,21 +64,21 @@
         throw greenlet::TypeError(err);
     }
 }
 
 
 
 template <typename T, greenlet::refs::TypeChecker TC>
-inline greenlet::Greenlet* greenlet::refs::_OwnedGreenlet<T, TC>::operator->() const G_NOEXCEPT
+inline greenlet::Greenlet* greenlet::refs::_OwnedGreenlet<T, TC>::operator->() const noexcept
 {
     return reinterpret_cast<PyGreenlet*>(this->p)->pimpl;
 }
 
 template <typename T, greenlet::refs::TypeChecker TC>
-inline greenlet::Greenlet* greenlet::refs::_BorrowedGreenlet<T, TC>::operator->() const G_NOEXCEPT
+inline greenlet::Greenlet* greenlet::refs::_BorrowedGreenlet<T, TC>::operator->() const noexcept
 {
     return reinterpret_cast<PyGreenlet*>(this->p)->pimpl;
 }
 
 #include <memory>
 #include <stdexcept>
```

### Comparing `greenlet-2.0.2/src/greenlet/greenlet_refs.hpp` & `greenlet-3.0.0a1/src/greenlet/greenlet_refs.hpp`

 * *Files 10% similar despite different names*

```diff
@@ -94,21 +94,19 @@
 
         G_FP_TMPL_STATIC inline void
         ContextExactChecker(void *p)
         {
             if (!p) {
                 return;
             }
-#if GREENLET_PY37
             if (!PyContext_CheckExact(p)) {
                 throw TypeError(
                     "greenlet context must be a contextvars.Context or None"
                 );
             }
-#endif
         }
 
         typedef OwnedReference<PyObject, ContextExactChecker> OwnedContext;
     }
 }
 
 namespace greenlet {
@@ -174,59 +172,59 @@
         // know better, then you can use the get() method, like on a
         // std::shared_ptr. Except we name it borrow() to clarify that
         // if this is a reference-tracked object, the pointer you get
         // back will go away when the object does.
         // TODO: This should probably not exist here, but be moved
         // down to relevant sub-types.
 
-        inline T* borrow() const G_NOEXCEPT
+        inline T* borrow() const noexcept
         {
             return this->p;
         }
 
-        PyObject* borrow_o() const G_NOEXCEPT
+        PyObject* borrow_o() const noexcept
         {
             return reinterpret_cast<PyObject*>(this->p);
         }
 
-        inline T* operator->() const G_NOEXCEPT
+        inline T* operator->() const noexcept
         {
             return this->p;
         }
 
-        bool is_None() const G_NOEXCEPT
+        bool is_None() const noexcept
         {
             return this->p == Py_None;
         }
 
-        inline PyObject* acquire_or_None() const G_NOEXCEPT
+        inline PyObject* acquire_or_None() const noexcept
         {
             PyObject* result = this->p ? reinterpret_cast<PyObject*>(this->p) : Py_None;
             Py_INCREF(result);
             return result;
         }
 
-        G_EXPLICIT_OP operator bool() const G_NOEXCEPT
+        explicit operator bool() const noexcept
         {
             return p != nullptr;
         }
 
-        inline Py_ssize_t REFCNT() const G_NOEXCEPT
+        inline Py_ssize_t REFCNT() const noexcept
         {
             return p ? Py_REFCNT(p) : -42;
         }
 
-        inline PyTypeObject* TYPE() const G_NOEXCEPT
+        inline PyTypeObject* TYPE() const noexcept
         {
             return p ? Py_TYPE(p) : nullptr;
         }
 
-        inline OwnedObject PyStr() const G_NOEXCEPT;
-        inline const std::string as_str() const G_NOEXCEPT;
-        inline OwnedObject PyGetAttr(const ImmortalObject& name) const G_NOEXCEPT;
+        inline OwnedObject PyStr() const noexcept;
+        inline const std::string as_str() const noexcept;
+        inline OwnedObject PyGetAttr(const ImmortalObject& name) const noexcept;
         inline OwnedObject PyRequireAttr(const char* const name) const;
         inline OwnedObject PyRequireAttr(const ImmortalObject& name) const;
         inline OwnedObject PyCall(const BorrowedObject& arg) const;
         inline OwnedObject PyCall(PyGreenlet* arg) const ;
         inline OwnedObject PyCall(PyObject* arg) const ;
         // PyObject_Call(this, args, kwargs);
         inline OwnedObject PyCall(const BorrowedObject args,
@@ -258,28 +256,28 @@
                << ")";
 
             return os;
         }
 #endif
 
     template<typename T, TypeChecker TC>
-    inline bool operator==(const PyObjectPointer<T, TC>& lhs, const void* const rhs) G_NOEXCEPT
+    inline bool operator==(const PyObjectPointer<T, TC>& lhs, const void* const rhs) noexcept
     {
         return lhs.borrow_o() == rhs;
     }
 
     template<typename T, TypeChecker TC, typename X, TypeChecker XC>
-    inline bool operator==(const PyObjectPointer<T, TC>& lhs, const PyObjectPointer<X, XC>& rhs) G_NOEXCEPT
+    inline bool operator==(const PyObjectPointer<T, TC>& lhs, const PyObjectPointer<X, XC>& rhs) noexcept
     {
         return lhs.borrow_o() == rhs.borrow_o();
     }
 
     template<typename T, TypeChecker TC, typename X, TypeChecker XC>
     inline bool operator!=(const PyObjectPointer<T, TC>& lhs,
-                           const PyObjectPointer<X, XC>& rhs) G_NOEXCEPT
+                           const PyObjectPointer<X, XC>& rhs) noexcept
     {
         return lhs.borrow_o() != rhs.borrow_o();
     }
 
     template<typename T=PyObject, TypeChecker TC=NoOpChecker>
     class OwnedReference : public PyObjectPointer<T, TC>
     {
@@ -504,16 +502,16 @@
         }
 
         PyObject* relinquish_ownership_o()
         {
             return reinterpret_cast<PyObject*>(relinquish_ownership());
         }
 
-        inline Greenlet* operator->() const G_NOEXCEPT;
-        inline operator Greenlet*() const G_NOEXCEPT;
+        inline Greenlet* operator->() const noexcept;
+        inline operator Greenlet*() const noexcept;
     };
 
     template <typename T=PyObject, TypeChecker TC=NoOpChecker>
     class BorrowedReference : public PyObjectPointer<T, TC>
     {
     public:
         // Allow implicit creation from PyObject* pointers as we
@@ -560,16 +558,16 @@
 
         // We get one of these for PyGreenlet, but one for PyObject
         // is handy as well
         operator PyObject*() const
         {
             return reinterpret_cast<PyObject*>(this->p);
         }
-        inline Greenlet* operator->() const G_NOEXCEPT;
-        inline operator Greenlet*() const G_NOEXCEPT;
+        inline Greenlet* operator->() const noexcept;
+        inline operator Greenlet*() const noexcept;
     };
 
     typedef _BorrowedGreenlet<PyGreenlet> BorrowedGreenlet;
 
     template<typename T, TypeChecker TC>
     _OwnedGreenlet<T, TC>::_OwnedGreenlet(const BorrowedGreenlet& other)
         : OwnedReference<T, TC>(reinterpret_cast<T*>(other.borrow()))
@@ -631,65 +629,61 @@
     class ImmortalString : public ImmortalObject
     {
     private:
         G_NO_COPIES_OF_CLS(ImmortalString);
         const char* str;
     public:
         ImmortalString(const char* const str) :
-            ImmortalObject(str ? Require(Greenlet_Intern(str)) : nullptr)
+            ImmortalObject(str ? Require(PyUnicode_InternFromString(str)) : nullptr)
         {
             this->str = str;
         }
 
         inline ImmortalString& operator=(const char* const str)
         {
             if (!this->p) {
-                this->p = Require(Greenlet_Intern(str));
+                this->p = Require(PyUnicode_InternFromString(str));
                 this->str = str;
             }
             else {
                 assert(this->str == str);
             }
             return *this;
         }
 
     };
 
     template<typename T, TypeChecker TC>
-    inline OwnedObject PyObjectPointer<T, TC>::PyStr() const G_NOEXCEPT
+    inline OwnedObject PyObjectPointer<T, TC>::PyStr() const noexcept
     {
         if (!this->p) {
             return OwnedObject();
         }
         return OwnedObject::consuming(PyObject_Str(reinterpret_cast<PyObject*>(this->p)));
     }
 
     template<typename T, TypeChecker TC>
-    inline const std::string PyObjectPointer<T, TC>::as_str() const G_NOEXCEPT
+    inline const std::string PyObjectPointer<T, TC>::as_str() const noexcept
     {
         // NOTE: This is not Python exception safe.
         if (this->p) {
             // The Python APIs return a cached char* value that's only valid
             // as long as the original object stays around, and we're
             // about to (probably) toss it. Hence the copy to std::string.
             OwnedObject py_str = this->PyStr();
             if (!py_str) {
                 return "(nil)";
             }
-#if PY_MAJOR_VERSION >= 3
             return PyUnicode_AsUTF8(py_str.borrow());
-#else
-            return PyString_AsString(py_str.borrow());
-#endif
         }
         return "(nil)";
     }
 
     template<typename T, TypeChecker TC>
-    inline OwnedObject PyObjectPointer<T, TC>::PyGetAttr(const ImmortalObject& name) const G_NOEXCEPT
+    inline OwnedObject PyObjectPointer<T, TC>::PyGetAttr(const ImmortalObject& name) const noexcept
     {
         assert(this->p);
         return OwnedObject::consuming(PyObject_GetAttr(reinterpret_cast<PyObject*>(this->p), name));
     }
 
     template<typename T, TypeChecker TC>
     inline OwnedObject PyObjectPointer<T, TC>::PyRequireAttr(const char* const name) const
```

### Comparing `greenlet-2.0.2/src/greenlet/greenlet_slp_switch.hpp` & `greenlet-3.0.0a1/src/greenlet/greenlet_slp_switch.hpp`

 * *Files 22% similar despite different names*

```diff
@@ -35,37 +35,19 @@
 // This is safe because we're protected by the GIL, and if we're
 // running this code, the thread isn't exiting. This also nets us a
 // 10-12% speed improvement.
 
 static greenlet::Greenlet* volatile switching_thread_state = nullptr;
 
 
-#ifdef GREENLET_NOINLINE_SUPPORTED
 extern "C" {
 static int GREENLET_NOINLINE(slp_save_state_trampoline)(char* stackref);
 static void GREENLET_NOINLINE(slp_restore_state_trampoline)();
 }
-#define GREENLET_NOINLINE_INIT() \
-    do {                         \
-    } while (0)
-#else
-/* force compiler to call functions via pointers */
-/* XXX: Do we even want/need to support such compilers? This code path
-   is untested on CI. */
-extern "C" {
-static int (slp_save_state_trampoline)(char* stackref);
-static void (slp_restore_state_trampoline)();
-}
-#define GREENLET_NOINLINE(name) cannot_inline_##name
-#define GREENLET_NOINLINE_INIT()                                  \
-    do {                                                              \
-            slp_save_state_trampoline = GREENLET_NOINLINE(slp_save_state_trampoline); \
-            slp_restore_state_trampoline = GREENLET_NOINLINE(slp_restore_state_trampoline); \
-    } while (0)
-#endif
+
 
 #define SLP_SAVE_STATE(stackref, stsizediff) \
 do {                                                    \
     assert(switching_thread_state);  \
     stackref += STACK_MAGIC;                 \
     if (slp_save_state_trampoline((char*)stackref))    \
         return -1;                                     \
```

### Comparing `greenlet-2.0.2/src/greenlet/greenlet_thread_state.hpp` & `greenlet-3.0.0a1/src/greenlet/greenlet_thread_state.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -528,34 +528,16 @@
             return this->_state->tp_traverse(visit, arg);
         }
         return 0;
     }
 
 };
 
-#if G_USE_STANDARD_THREADING == 1
+
 // We can't use the PythonAllocator for this, because we push to it
 // from the thread state destructor, which doesn't have the GIL,
 // and Python's allocators can only be called with the GIL.
 typedef std::vector<ThreadState*> cleanup_queue_t;
-#else
-class cleanup_queue_t {
-public:
-    inline ssize_t size() const { return 0; };
-    inline bool empty() const { return true; };
-    inline void pop_back()
-    {
-        throw std::out_of_range("empty queue.");
-    };
-    inline ThreadState* back()
-    {
-        throw std::out_of_range("empty queue.");
-    };
-    inline void push_back(ThreadState* g)
-    {
-        throw std::out_of_range("empty queue.");
-    };
-};
-#endif
+
 }; // namespace greenlet
 
 #endif
```

### Comparing `greenlet-2.0.2/src/greenlet/greenlet_thread_state_dict_cleanup.hpp` & `greenlet-3.0.0a1/src/greenlet/greenlet_thread_state_dict_cleanup.hpp`

 * *Files identical despite different names*

### Comparing `greenlet-2.0.2/src/greenlet/platform/switch_alpha_unix.h` & `greenlet-3.0.0a1/src/greenlet/platform/switch_alpha_unix.h`

 * *Files 16% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 #define REGS_TO_SAVE "$9", "$10", "$11", "$12", "$13", "$14", "$15", \
 		     "$f2", "$f3", "$f4", "$f5", "$f6", "$f7", "$f8", "$f9"
 
 static int
 slp_switch(void)
 {
-  register int ret;
-  register long *stackref, stsizediff;
+  int ret;
+  long *stackref, stsizediff;
   __asm__ volatile ("" : : : REGS_TO_SAVE);
   __asm__ volatile ("mov $30, %0" : "=r" (stackref) : );
   {
       SLP_SAVE_STATE(stackref, stsizediff);
       __asm__ volatile (
 	  "addq $30, %0, $30\n\t"
 	  : /* no outputs */
```

### Comparing `greenlet-2.0.2/src/greenlet/platform/switch_amd64_unix.h` & `greenlet-3.0.0a1/src/greenlet/platform/switch_amd64_unix.h`

 * *Files identical despite different names*

### Comparing `greenlet-2.0.2/src/greenlet/platform/switch_arm32_gcc.h` & `greenlet-3.0.0a1/src/greenlet/platform/switch_arm32_gcc.h`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 static int
 #ifdef __GNUC__
 __attribute__((optimize("no-omit-frame-pointer")))
 #endif
 slp_switch(void)
 {
         void *fp;
-        register int *stackref, stsizediff;
+        int *stackref, stsizediff;
         int result;
         __asm__ volatile ("" : : : REGS_TO_SAVE);
         __asm__ volatile ("mov r0," REG_FP "\n\tstr r0,%0" : "=m" (fp) : : "r0");
         __asm__ ("mov %0," REG_SP : "=r" (stackref));
         {
                 SLP_SAVE_STATE(stackref, stsizediff);
                 __asm__ volatile (
```

### Comparing `greenlet-2.0.2/src/greenlet/platform/switch_arm32_ios.h` & `greenlet-3.0.0a1/src/greenlet/platform/switch_arm32_ios.h`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 static int
 #ifdef __GNUC__
 __attribute__((optimize("no-omit-frame-pointer")))
 #endif
 slp_switch(void)
 {
         void *fp;
-        register int *stackref, stsizediff, result;
+        int *stackref, stsizediff, result;
         __asm__ volatile ("" : : : REGS_TO_SAVE);
         __asm__ volatile ("str " REG_FP ",%0" : "=m" (fp));
         __asm__ ("mov %0," REG_SP : "=r" (stackref));
         {
                 SLP_SAVE_STATE(stackref, stsizediff);
                 __asm__ volatile (
                     "add " REG_SPSP ",%0\n"
```

### Comparing `greenlet-2.0.2/src/greenlet/platform/switch_arm64_masm.asm` & `greenlet-3.0.0a1/src/greenlet/platform/switch_arm64_masm.asm`

 * *Files identical despite different names*

### Comparing `greenlet-2.0.2/src/greenlet/platform/switch_arm64_masm.obj` & `greenlet-3.0.0a1/src/greenlet/platform/switch_arm64_masm.obj`

 * *Files identical despite different names*

### Comparing `greenlet-2.0.2/src/greenlet/platform/switch_csky_gcc.h` & `greenlet-3.0.0a1/src/greenlet/platform/switch_csky_gcc.h`

 * *Files 10% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 static int
 #ifdef __GNUC__
 __attribute__((optimize("no-omit-frame-pointer")))
 #endif
 slp_switch(void)
 {
-        register int *stackref, stsizediff;
+        int *stackref, stsizediff;
         int result;
 
         __asm__ volatile ("" : : : REGS_TO_SAVE);
         __asm__ ("mov %0, sp" : "=r" (stackref));
         {
                 SLP_SAVE_STATE(stackref, stsizediff);
                 __asm__ volatile (
```

### Comparing `greenlet-2.0.2/src/greenlet/platform/switch_m68k_gcc.h` & `greenlet-3.0.0a1/src/greenlet/platform/switch_m68k_gcc.h`

 * *Files identical despite different names*

### Comparing `greenlet-2.0.2/src/greenlet/platform/switch_mips_unix.h` & `greenlet-3.0.0a1/src/greenlet/platform/switch_mips_unix.h`

 * *Files 10% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 #define STACK_MAGIC 0
 
 #define REGS_TO_SAVE "$16", "$17", "$18", "$19", "$20", "$21", "$22", \
        "$23", "$30"
 static int
 slp_switch(void)
 {
-    register int err;
-    register int *stackref, stsizediff;
+    int err;
+    int *stackref, stsizediff;
 #ifdef __mips64
     uint64_t gpsave;
 #endif
     __asm__ __volatile__ ("" : : : REGS_TO_SAVE);
 #ifdef __mips64
     __asm__ __volatile__ ("sd $28,%0" : "=m" (gpsave) : : );
 #endif
```

### Comparing `greenlet-2.0.2/src/greenlet/platform/switch_ppc64_aix.h` & `greenlet-3.0.0a1/src/greenlet/platform/switch_ppc64_aix.h`

 * *Files 2% similar despite different names*

```diff
@@ -70,16 +70,16 @@
        "fr30", "fr31", \
        ALTIVEC_REGS \
        "cr2", "cr3", "cr4"
 
 static int
 slp_switch(void)
 {
-    register int err;
-    register long *stackref, stsizediff;
+    int err;
+    long *stackref, stsizediff;
     void * toc;
     void * r30;
     __asm__ volatile ("" : : : REGS_TO_SAVE);
     __asm__ volatile ("std 2, %0" : "=m" (toc));
     __asm__ volatile ("std 30, %0" : "=m" (r30));
     __asm__ ("mr %0, 1" : "=r" (stackref) : );
     {
```

### Comparing `greenlet-2.0.2/src/greenlet/platform/switch_ppc64_linux.h` & `greenlet-3.0.0a1/src/greenlet/platform/switch_ppc64_linux.h`

 * *Files 3% similar despite different names*

```diff
@@ -72,16 +72,16 @@
        "fr30", "fr31", \
        ALTIVEC_REGS \
        "cr2", "cr3", "cr4"
 
 static int
 slp_switch(void)
 {
-    register int err;
-    register long *stackref, stsizediff;
+    int err;
+    long *stackref, stsizediff;
     void * toc;
     void * r30;
     __asm__ volatile ("" : : : REGS_TO_SAVE);
     __asm__ volatile ("std 2, %0" : "=m" (toc));
     __asm__ volatile ("std 30, %0" : "=m" (r30));
     __asm__ ("mr %0, 1" : "=r" (stackref) : );
     {
```

### Comparing `greenlet-2.0.2/src/greenlet/platform/switch_ppc_aix.h` & `greenlet-3.0.0a1/src/greenlet/platform/switch_ppc_aix.h`

 * *Files 5% similar despite different names*

```diff
@@ -49,16 +49,16 @@
  */
 #define REGS_TO_SAVE "r13", "r14", "r15", "r16", "r17", "r18", "r19", "r20", \
        "r21", "r22", "r23", "r24", "r25", "r26", "r27", "r28", "r29", \
        "cr2", "cr3", "cr4"
 static int
 slp_switch(void)
 {
-    register int err;
-    register int *stackref, stsizediff;
+    int err;
+    int *stackref, stsizediff;
     __asm__ volatile ("" : : : REGS_TO_SAVE);
     __asm__ ("mr %0, 1" : "=r" (stackref) : );
     {
         SLP_SAVE_STATE(stackref, stsizediff);
         __asm__ volatile (
             "mr 11, %0\n"
             "add 1, 1, 11\n"
```

### Comparing `greenlet-2.0.2/src/greenlet/platform/switch_ppc_linux.h` & `greenlet-3.0.0a1/src/greenlet/platform/switch_ppc_unix.h`

 * *Files 4% similar despite different names*

```diff
@@ -26,16 +26,14 @@
  *      slightly changed framework for sparc
  * 29-Jun-02  Christian Tismer  <tismer@tismer.com>
  *      Added register 13-29, 31 saves. The same way as
  *      Armin Rigo did for the x86_unix version.
  *      This seems to be now fully functional!
  * 04-Mar-02  Hye-Shik Chang  <perky@fallin.lv>
  *      Ported from i386.
- * 31-Jul-12  Trevor Bowen    <trevorbowen@gmail.com>
- *      Changed memory constraints to register only.
  */
 
 #define STACK_REFPLUS 1
 
 #ifdef SLP_EVAL
 
 #define STACK_MAGIC 3
@@ -45,26 +43,26 @@
  */
 #define REGS_TO_SAVE "r13", "r14", "r15", "r16", "r17", "r18", "r19", "r20", \
        "r21", "r22", "r23", "r24", "r25", "r26", "r27", "r28", "r29", \
        "cr2", "cr3", "cr4"
 static int
 slp_switch(void)
 {
-    register int err;
-    register int *stackref, stsizediff;
+    int err;
+    int *stackref, stsizediff;
     __asm__ volatile ("" : : : REGS_TO_SAVE);
-    __asm__ ("mr %0, 1" : "=r" (stackref) : );
+    __asm__ ("mr %0, 1" : "=g" (stackref) : );
     {
         SLP_SAVE_STATE(stackref, stsizediff);
         __asm__ volatile (
             "mr 11, %0\n"
             "add 1, 1, 11\n"
             "add 30, 30, 11\n"
             : /* no outputs */
-            : "r" (stsizediff)
+            : "g" (stsizediff)
             : "11"
             );
         SLP_RESTORE_STATE();
     }
     __asm__ volatile ("" : : : REGS_TO_SAVE);
     __asm__ volatile ("li %0, 0" : "=r" (err));
     return err;
```

### Comparing `greenlet-2.0.2/src/greenlet/platform/switch_ppc_macosx.h` & `greenlet-3.0.0a1/src/greenlet/platform/switch_ppc_linux.h`

 * *Files 10% similar despite different names*

```diff
@@ -12,58 +12,60 @@
  *      What about vector registers?
  *      Differences between darwin and unix?
  * 24-Nov-02  Christian Tismer  <tismer@tismer.com>
  *      needed to add another magic constant to insure
  *      that f in slp_eval_frame(PyFrameObject *f)
  *      STACK_REFPLUS will probably be 1 in most cases.
  *      gets included into the saved stack area.
+ * 04-Oct-02  Gustavo Niemeyer <niemeyer@conectiva.com>
+ *      Ported from MacOS version.
  * 17-Sep-02  Christian Tismer  <tismer@tismer.com>
  *      after virtualizing stack save/restore, the
  *      stack size shrunk a bit. Needed to introduce
  *      an adjustment STACK_MAGIC per platform.
  * 15-Sep-02  Gerd Woetzel       <gerd.woetzel@GMD.DE>
  *      slightly changed framework for sparc
  * 29-Jun-02  Christian Tismer  <tismer@tismer.com>
  *      Added register 13-29, 31 saves. The same way as
  *      Armin Rigo did for the x86_unix version.
  *      This seems to be now fully functional!
  * 04-Mar-02  Hye-Shik Chang  <perky@fallin.lv>
  *      Ported from i386.
+ * 31-Jul-12  Trevor Bowen    <trevorbowen@gmail.com>
+ *      Changed memory constraints to register only.
  */
 
 #define STACK_REFPLUS 1
 
 #ifdef SLP_EVAL
 
 #define STACK_MAGIC 3
 
 /* !!!!WARNING!!!! need to add "r31" in the next line if this header file
  * is meant to be compiled non-dynamically!
  */
 #define REGS_TO_SAVE "r13", "r14", "r15", "r16", "r17", "r18", "r19", "r20", \
        "r21", "r22", "r23", "r24", "r25", "r26", "r27", "r28", "r29", \
        "cr2", "cr3", "cr4"
-
 static int
 slp_switch(void)
 {
-    register int err;
-    register int *stackref, stsizediff;
+    int err;
+    int *stackref, stsizediff;
     __asm__ volatile ("" : : : REGS_TO_SAVE);
-    __asm__ ("; asm block 2\n\tmr %0, r1" : "=g" (stackref) : );
+    __asm__ ("mr %0, 1" : "=r" (stackref) : );
     {
         SLP_SAVE_STATE(stackref, stsizediff);
         __asm__ volatile (
-            "; asm block 3\n"
-            "\tmr r11, %0\n"
-            "\tadd r1, r1, r11\n"
-            "\tadd r30, r30, r11\n"
+            "mr 11, %0\n"
+            "add 1, 1, 11\n"
+            "add 30, 30, 11\n"
             : /* no outputs */
-            : "g" (stsizediff)
-            : "r11"
+            : "r" (stsizediff)
+            : "11"
             );
         SLP_RESTORE_STATE();
     }
     __asm__ volatile ("" : : : REGS_TO_SAVE);
     __asm__ volatile ("li %0, 0" : "=r" (err));
     return err;
 }
```

### Comparing `greenlet-2.0.2/src/greenlet/platform/switch_ppc_unix.h` & `greenlet-3.0.0a1/src/greenlet/platform/switch_ppc_macosx.h`

 * *Files 11% similar despite different names*

```diff
@@ -12,16 +12,14 @@
  *      What about vector registers?
  *      Differences between darwin and unix?
  * 24-Nov-02  Christian Tismer  <tismer@tismer.com>
  *      needed to add another magic constant to insure
  *      that f in slp_eval_frame(PyFrameObject *f)
  *      STACK_REFPLUS will probably be 1 in most cases.
  *      gets included into the saved stack area.
- * 04-Oct-02  Gustavo Niemeyer <niemeyer@conectiva.com>
- *      Ported from MacOS version.
  * 17-Sep-02  Christian Tismer  <tismer@tismer.com>
  *      after virtualizing stack save/restore, the
  *      stack size shrunk a bit. Needed to introduce
  *      an adjustment STACK_MAGIC per platform.
  * 15-Sep-02  Gerd Woetzel       <gerd.woetzel@GMD.DE>
  *      slightly changed framework for sparc
  * 29-Jun-02  Christian Tismer  <tismer@tismer.com>
@@ -40,30 +38,32 @@
 
 /* !!!!WARNING!!!! need to add "r31" in the next line if this header file
  * is meant to be compiled non-dynamically!
  */
 #define REGS_TO_SAVE "r13", "r14", "r15", "r16", "r17", "r18", "r19", "r20", \
        "r21", "r22", "r23", "r24", "r25", "r26", "r27", "r28", "r29", \
        "cr2", "cr3", "cr4"
+
 static int
 slp_switch(void)
 {
-    register int err;
-    register int *stackref, stsizediff;
+    int err;
+    int *stackref, stsizediff;
     __asm__ volatile ("" : : : REGS_TO_SAVE);
-    __asm__ ("mr %0, 1" : "=g" (stackref) : );
+    __asm__ ("; asm block 2\n\tmr %0, r1" : "=g" (stackref) : );
     {
         SLP_SAVE_STATE(stackref, stsizediff);
         __asm__ volatile (
-            "mr 11, %0\n"
-            "add 1, 1, 11\n"
-            "add 30, 30, 11\n"
+            "; asm block 3\n"
+            "\tmr r11, %0\n"
+            "\tadd r1, r1, r11\n"
+            "\tadd r30, r30, r11\n"
             : /* no outputs */
             : "g" (stsizediff)
-            : "11"
+            : "r11"
             );
         SLP_RESTORE_STATE();
     }
     __asm__ volatile ("" : : : REGS_TO_SAVE);
     __asm__ volatile ("li %0, 0" : "=r" (err));
     return err;
 }
```

### Comparing `greenlet-2.0.2/src/greenlet/platform/switch_riscv_unix.h` & `greenlet-3.0.0a1/src/greenlet/platform/switch_riscv_unix.h`

 * *Files identical despite different names*

### Comparing `greenlet-2.0.2/src/greenlet/platform/switch_s390_unix.h` & `greenlet-3.0.0a1/src/greenlet/platform/switch_s390_unix.h`

 * *Files 6% similar despite different names*

```diff
@@ -32,16 +32,16 @@
 #define REGS_TO_SAVE "r6", "r7", "r8", "r9", "r10", "r14", \
 		     "f0", "f1", "f2", "f3", "f4", "f5", "f6", "f7", \
 		     "f8", "f9", "f10", "f11", "f12", "f13", "f14", "f15"
 
 static int
 slp_switch(void)
 {
-    register int ret;
-    register long *stackref, stsizediff;
+    int ret;
+    long *stackref, stsizediff;
     __asm__ volatile ("" : : : REGS_TO_SAVE);
 #ifdef __s390x__
     __asm__ volatile ("lgr %0, 15" : "=r" (stackref) : );
 #else
     __asm__ volatile ("lr %0, 15" : "=r" (stackref) : );
 #endif
     {
```

### Comparing `greenlet-2.0.2/src/greenlet/platform/switch_sparc_sun_gcc.h` & `greenlet-3.0.0a1/src/greenlet/platform/switch_sparc_sun_gcc.h`

 * *Files 2% similar despite different names*

```diff
@@ -47,16 +47,16 @@
 #define SLP_BEFORE_SAVE_STATE() SLP_FLUSHW
 #define SLP_BEFORE_RESTORE_STATE() SLP_FLUSHW
 
 
 static int
 slp_switch(void)
 {
-    register int err;
-    register int *stackref, stsizediff;
+    int err;
+    int *stackref, stsizediff;
 
     /* Put current stack pointer into stackref.
      * Register spilling is done in save/restore.
      */
     __asm__ volatile ("mov %%sp, %0" : "=r" (stackref));
 
     {
```

### Comparing `greenlet-2.0.2/src/greenlet/platform/switch_x32_unix.h` & `greenlet-3.0.0a1/src/greenlet/platform/switch_x32_unix.h`

 * *Files 6% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 static int
 slp_switch(void)
 {
     void* ebp;
     void* ebx;
     unsigned int csr;
     unsigned short cw;
-    register int err;
-    register int *stackref, stsizediff;
+    int err;
+    int *stackref, stsizediff;
     __asm__ volatile ("" : : : REGS_TO_SAVE);
     __asm__ volatile ("fstcw %0" : "=m" (cw));
     __asm__ volatile ("stmxcsr %0" : "=m" (csr));
     __asm__ volatile ("movl %%ebp, %0" : "=m" (ebp));
     __asm__ volatile ("movl %%ebx, %0" : "=m" (ebx));
     __asm__ ("movl %%esp, %0" : "=g" (stackref));
     {
```

### Comparing `greenlet-2.0.2/src/greenlet/platform/switch_x64_masm.asm` & `greenlet-3.0.0a1/src/greenlet/platform/switch_x64_masm.asm`

 * *Files identical despite different names*

### Comparing `greenlet-2.0.2/src/greenlet/platform/switch_x64_masm.obj` & `greenlet-3.0.0a1/src/greenlet/platform/switch_x64_masm.obj`

 * *Files identical despite different names*

### Comparing `greenlet-2.0.2/src/greenlet/platform/switch_x64_msvc.h` & `greenlet-3.0.0a1/src/greenlet/platform/switch_x64_msvc.h`

 * *Files identical despite different names*

### Comparing `greenlet-2.0.2/src/greenlet/platform/switch_x86_msvc.h` & `greenlet-3.0.0a1/src/greenlet/platform/switch_x86_msvc.h`

 * *Files identical despite different names*

### Comparing `greenlet-2.0.2/src/greenlet/platform/switch_x86_unix.h` & `greenlet-3.0.0a1/src/greenlet/platform/switch_x86_unix.h`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 {
     int err;
 #ifdef _WIN32
     void *seh;
 #endif
     void *ebp, *ebx;
     unsigned short cw;
-    register int *stackref, stsizediff;
+    int *stackref, stsizediff;
     __asm__ volatile ("" : : : "esi", "edi");
     __asm__ volatile ("fstcw %0" : "=m" (cw));
     __asm__ volatile ("movl %%ebp, %0" : "=m" (ebp));
     __asm__ volatile ("movl %%ebx, %0" : "=m" (ebx));
 #ifdef _WIN32
     __asm__ volatile (
         "movl %%fs:0x0, %%eax\n"
```

### Comparing `greenlet-2.0.2/src/greenlet/slp_platformselect.h` & `greenlet-3.0.0a1/src/greenlet/slp_platformselect.h`

 * *Files identical despite different names*

### Comparing `greenlet-2.0.2/src/greenlet/tests/__init__.py` & `greenlet-3.0.0a1/src/greenlet/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `greenlet-2.0.2/src/greenlet/tests/_test_extension.c` & `greenlet-3.0.0a1/src/greenlet/tests/_test_extension.c`

 * *Files 2% similar despite different names*

```diff
@@ -199,46 +199,33 @@
     {"test_throw_exact",
      (PyCFunction)test_throw_exact,
      METH_VARARGS,
      "Throw exactly the arguments given at the provided greenlet"},
     {NULL, NULL, 0, NULL}
 };
 
-#if PY_MAJOR_VERSION >= 3
-#    define INITERROR return NULL
+
+#define INITERROR return NULL
 
 static struct PyModuleDef moduledef = {PyModuleDef_HEAD_INIT,
                                        TEST_MODULE_NAME,
                                        NULL,
                                        0,
                                        test_methods,
                                        NULL,
                                        NULL,
                                        NULL,
                                        NULL};
 
 PyMODINIT_FUNC
 PyInit__test_extension(void)
-#else
-#    define INITERROR return
-PyMODINIT_FUNC
-init_test_extension(void)
-#endif
 {
     PyObject* module = NULL;
-
-#if PY_MAJOR_VERSION >= 3
     module = PyModule_Create(&moduledef);
-#else
-    module = Py_InitModule(TEST_MODULE_NAME, test_methods);
-#endif
 
     if (module == NULL) {
-        INITERROR;
+        return NULL;
     }
 
     PyGreenlet_Import();
-
-#if PY_MAJOR_VERSION >= 3
     return module;
-#endif
 }
```

### Comparing `greenlet-2.0.2/src/greenlet/tests/_test_extension_cpp.cpp` & `greenlet-3.0.0a1/src/greenlet/tests/_test_extension_cpp.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -145,52 +145,39 @@
      "C++ exceptions thrown in a greenlet doe not corrupt memory."},
     {"test_exception_throw",
      (PyCFunction)&py_test_exception_throw,
      METH_VARARGS,
      "Throws C++ exception. Calling this function directly should abort the process."},
     {NULL, NULL, 0, NULL}};
 
-#if PY_MAJOR_VERSION >= 3
-#    define INITERROR return NULL
 
 static struct PyModuleDef moduledef = {PyModuleDef_HEAD_INIT,
                                        "greenlet.tests._test_extension_cpp",
                                        NULL,
                                        0,
                                        test_methods,
                                        NULL,
                                        NULL,
                                        NULL,
                                        NULL};
 
 PyMODINIT_FUNC
 PyInit__test_extension_cpp(void)
-#else
-#    define INITERROR return
-PyMODINIT_FUNC
-init_test_extension_cpp(void)
-#endif
 {
     PyObject* module = NULL;
 
-#if PY_MAJOR_VERSION >= 3
     module = PyModule_Create(&moduledef);
-#else
-    module = Py_InitModule("greenlet.tests._test_extension_cpp", test_methods);
-#endif
 
     if (module == NULL) {
-        INITERROR;
+        return NULL;
     }
 
     PyGreenlet_Import();
     if (_PyGreenlet_API == NULL) {
-        INITERROR;
+        return NULL;
     }
 
     p_test_exception_throw = test_exception_throw;
     p_test_exception_switch_recurse = test_exception_switch_recurse;
 
-#if PY_MAJOR_VERSION >= 3
     return module;
-#endif
 }
```

### Comparing `greenlet-2.0.2/src/greenlet/tests/leakcheck.py` & `greenlet-3.0.0a1/src/greenlet/tests/leakcheck.py`

 * *Files identical despite different names*

### Comparing `greenlet-2.0.2/src/greenlet/tests/test_contextvars.py` & `greenlet-3.0.0a1/src/greenlet/tests/test_contextvars.py`

 * *Files identical despite different names*

### Comparing `greenlet-2.0.2/src/greenlet/tests/test_cpp.py` & `greenlet-3.0.0a1/src/greenlet/tests/test_cpp.py`

 * *Files identical despite different names*

### Comparing `greenlet-2.0.2/src/greenlet/tests/test_extension_interface.py` & `greenlet-3.0.0a1/src/greenlet/tests/test_extension_interface.py`

 * *Files identical despite different names*

### Comparing `greenlet-2.0.2/src/greenlet/tests/test_gc.py` & `greenlet-3.0.0a1/src/greenlet/tests/test_gc.py`

 * *Files identical despite different names*

### Comparing `greenlet-2.0.2/src/greenlet/tests/test_generator.py` & `greenlet-3.0.0a1/src/greenlet/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `greenlet-2.0.2/src/greenlet/tests/test_generator_nested.py` & `greenlet-3.0.0a1/src/greenlet/tests/test_generator_nested.py`

 * *Files identical despite different names*

### Comparing `greenlet-2.0.2/src/greenlet/tests/test_greenlet.py` & `greenlet-3.0.0a1/src/greenlet/tests/test_greenlet.py`

 * *Files 2% similar despite different names*

```diff
@@ -574,34 +574,29 @@
         worker[0].switch() # prime worker
         initiator = greenlet(initiator, worker[0])
         value = initiator.switch()
         self.assertTrue(seen)
         self.assertEqual(value, 42)
 
     def test_tuple_subclass(self):
-        # XXX: This is failing on Python 2 with a SystemError: error return without exception set
-
         # The point of this test is to see what happens when a custom
         # tuple subclass is used as an object passed directly to the C
         # function ``green_switch``; part of ``green_switch`` checks
         # the ``len()`` of the ``args`` tuple, and that can call back
         # into Python. Here, when it calls back into Python, we
         # recursively enter ``green_switch`` again.
 
         # This test is really only relevant on Python 2. The builtin
         # `apply` function directly passes the given args tuple object
         # to the underlying function, whereas the Python 3 version
         # unpacks and repacks into an actual tuple. This could still
-        # happen using the C API on Python 3 though.
-        if sys.version_info[0] > 2:
-            # There's no apply in Python 3.x
-            def _apply(func, a, k):
-                func(*a, **k)
-        else:
-            _apply = apply # pylint:disable=undefined-variable
+        # happen using the C API on Python 3 though. We should write a
+        # builtin version of apply() ourself.
+        def _apply(func, a, k):
+            func(*a, **k)
 
         class mytuple(tuple):
             def __len__(self):
                 greenlet.getcurrent().switch()
                 return tuple.__len__(self)
         args = mytuple()
         kwargs = dict(a=42)
```

### Comparing `greenlet-2.0.2/src/greenlet/tests/test_greenlet_trash.py` & `greenlet-3.0.0a1/src/greenlet/tests/test_greenlet_trash.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,25 +23,18 @@
     - The test fails by hitting an ``assert()`` in object.c; if the
       build didn't enable assert, then we don't catch this.
 
     - If the test fails in that way, the interpreter crashes.
 """
 from __future__ import print_function, absolute_import, division
 
-import sys
 import unittest
 
-
-
 class TestTrashCanReEnter(unittest.TestCase):
 
-    @unittest.skipUnless(
-        sys.version_info[0] > 2,
-        "Python 2 tracks this slightly differently, so our test doesn't catch a problem there. "
-    )
     def test_it(self):
         # Try several times to trigger it, because it isn't 100%
         # reliable.
         for _ in range(10):
             self.check_it()
 
     def check_it(self): # pylint:disable=too-many-statements
```

### Comparing `greenlet-2.0.2/src/greenlet/tests/test_leaks.py` & `greenlet-3.0.0a1/src/greenlet/tests/test_leaks.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 import psutil
 
 import greenlet
 from . import TestCase
 from .leakcheck import fails_leakcheck
 from .leakcheck import ignores_leakcheck
-from .leakcheck import RUNNING_ON_GITHUB_ACTIONS
 from .leakcheck import RUNNING_ON_MANYLINUX
 
 try:
     from sys import intern
 except ImportError:
     # Python 2
     pass
@@ -305,19 +304,19 @@
     UNTRACK_ATTEMPTS = 100
 
     def _only_test_some_versions(self):
         # We're only looking for this problem specifically on 3.11,
         # and this set of tests is relatively fragile, depending on
         # OS and memory management details. So we want to run it on 3.11+
         # (obviously) but not every older 3.x version in order to reduce
-        # false negatives.
-        if sys.version_info[0] >= 3 and sys.version_info[:2] < (3, 8):
+        # false negatives. At the moment, those false results seem to have
+        # resolved, so we are actually running this on 3.8+
+        assert sys.version_info[0] >= 3
+        if sys.version_info[:2] < (3, 8):
             self.skipTest('Only observed on 3.11')
-        if sys.version_info[0] == 2 and RUNNING_ON_GITHUB_ACTIONS:
-            self.skipTest('Hard to get a stable pattern here')
         if RUNNING_ON_MANYLINUX:
             self.skipTest("Slow and not worth repeating here")
 
     @ignores_leakcheck
     # Because we're just trying to track raw memory, not objects, and running
     # the leakcheck makes an already slow test slower.
     def test_untracked_memory_doesnt_increase(self):
```

### Comparing `greenlet-2.0.2/src/greenlet/tests/test_throw.py` & `greenlet-3.0.0a1/src/greenlet/tests/test_throw.py`

 * *Files identical despite different names*

### Comparing `greenlet-2.0.2/src/greenlet/tests/test_tracing.py` & `greenlet-3.0.0a1/src/greenlet/tests/test_tracing.py`

 * *Files identical despite different names*

### Comparing `greenlet-2.0.2/src/greenlet/tests/test_version.py` & `greenlet-3.0.0a1/src/greenlet/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `greenlet-2.0.2/src/greenlet/tests/test_weakref.py` & `greenlet-3.0.0a1/src/greenlet/tests/test_weakref.py`

 * *Files identical despite different names*

### Comparing `greenlet-2.0.2/src/greenlet.egg-info/PKG-INFO` & `greenlet-3.0.0a1/src/greenlet.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: greenlet
-Version: 2.0.2
+Version: 3.0.0a1
 Summary: Lightweight in-process concurrent programming
 Home-page: https://greenlet.readthedocs.io/
 Author: Alexey Borzenkov
 Author-email: snaury@gmail.com
 Maintainer: Jason Madden
 Maintainer-email: jason@seecoresoftware.com
 License: MIT License
@@ -15,27 +15,24 @@
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: test
 License-File: LICENSE
 License-File: LICENSE.PSF
 License-File: AUTHORS
```

### Comparing `greenlet-2.0.2/src/greenlet.egg-info/SOURCES.txt` & `greenlet-3.0.0a1/src/greenlet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `greenlet-2.0.2/tox.ini` & `greenlet-3.0.0a1/tox.ini`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 [tox]
 envlist =
-    py27,py35,py36,py37,py38,py39,py310,py27-ns,py310-ns,py311,py311-ns,docs
+    py37,py38,py39,py310,py27-ns,py310-ns,py311,py311-ns,docs
 
 [testenv]
-setenv =
-    ns: CPPFLAGS=-DG_USE_STANDARD_THREADING=0
 commands =
-    ns: python -c 'import greenlet._greenlet as G; assert not G.GREENLET_USE_STANDARD_THREADING'
-    !ns: python -c 'import greenlet._greenlet as G; assert G.GREENLET_USE_STANDARD_THREADING'
+    python -c 'import greenlet._greenlet as G; assert G.GREENLET_USE_STANDARD_THREADING'
     python -m unittest discover -v greenlet.tests
-    !ns: sphinx-build -b doctest -d docs/_build/doctrees-{envname} docs docs/_build/doctest-{envname}
+    sphinx-build -b doctest -d docs/_build/doctrees-{envname} docs docs/_build/doctest-{envname}
 sitepackages = False
 extras =
     test
     docs
```

