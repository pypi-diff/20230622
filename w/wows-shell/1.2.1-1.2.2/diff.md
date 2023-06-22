# Comparing `tmp/wows_shell-1.2.1.tar.gz` & `tmp/wows_shell-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wows_shell-1.2.1.tar", last modified: Mon Jun 19 19:00:29 2023, max compression
+gzip compressed data, was "wows_shell-1.2.2.tar", last modified: Thu Jun 22 03:24:03 2023, max compression
```

## Comparing `wows_shell-1.2.1.tar` & `wows_shell-1.2.2.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 19:00:29.479077 wows_shell-1.2.1/
--rw-rw-rw-   0        0        0     1084 2020-07-28 13:49:29.000000 wows_shell-1.2.1/LICENSE
--rw-rw-rw-   0        0        0       31 2021-01-23 20:09:16.000000 wows_shell-1.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3257 2023-06-19 19:00:29.478082 wows_shell-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     3003 2020-12-29 19:40:43.000000 wows_shell-1.2.1/README.md
--rw-rw-rw-   0        0        0      131 2021-01-23 20:09:16.000000 wows_shell-1.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-19 19:00:29.480119 wows_shell-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1095 2023-06-19 14:50:35.000000 wows_shell-1.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 19:00:29.396871 wows_shell-1.2.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-19 19:00:29.399847 wows_shell-1.2.1/src/Python/
-drwxrwxrwx   0        0        0        0 2023-06-19 18:51:10.703243 wows_shell-1.2.1/src/Python/out/
-drwxrwxrwx   0        0        0        0 2023-06-19 19:00:29.366842 wows_shell-1.2.1/src/Python/out/build/
-drwxrwxrwx   0        0        0        0 2023-06-19 19:00:29.366842 wows_shell-1.2.1/src/Python/out/build/x64-Debug (default)/
-drwxrwxrwx   0        0        0        0 2023-06-19 19:00:29.366842 wows_shell-1.2.1/src/Python/out/build/x64-Debug (default)/CMakeFiles/
-drwxrwxrwx   0        0        0        0 2023-06-19 19:00:29.401618 wows_shell-1.2.1/src/Python/out/build/x64-Debug (default)/CMakeFiles/ShowIncludes/
--rw-rw-rw-   0        0        0        2 2021-01-23 06:11:54.000000 wows_shell-1.2.1/src/Python/out/build/x64-Debug (default)/CMakeFiles/ShowIncludes/foo.h
--rw-rw-rw-   0        0        0    24784 2023-06-19 14:50:35.000000 wows_shell-1.2.1/src/Python/wows_shell_python.cpp
--rw-rw-rw-   0        0        0     3197 2022-02-01 03:51:03.000000 wows_shell-1.2.1/src/controlEnums.hpp
-drwxrwxrwx   0        0        0        0 2023-06-19 19:00:29.368808 wows_shell-1.2.1/src/fitShell/
-drwxrwxrwx   0        0        0        0 2023-06-19 19:00:29.368808 wows_shell-1.2.1/src/fitShell/out/
-drwxrwxrwx   0        0        0        0 2023-06-19 19:00:29.370921 wows_shell-1.2.1/src/fitShell/out/build/
-drwxrwxrwx   0        0        0        0 2023-06-19 19:00:29.371919 wows_shell-1.2.1/src/fitShell/out/build/x64-Debug/
-drwxrwxrwx   0        0        0        0 2023-06-19 19:00:29.371919 wows_shell-1.2.1/src/fitShell/out/build/x64-Debug/CMakeFiles/
-drwxrwxrwx   0        0        0        0 2023-06-19 19:00:29.407608 wows_shell-1.2.1/src/fitShell/out/build/x64-Debug/CMakeFiles/ShowIncludes/
--rw-rw-rw-   0        0        0        2 2020-12-26 00:29:01.000000 wows_shell-1.2.1/src/fitShell/out/build/x64-Debug/CMakeFiles/ShowIncludes/foo.h
-drwxrwxrwx   0        0        0        0 2023-06-19 19:00:29.370921 wows_shell-1.2.1/src/fitShell/out/build/x64-Debug (default)/
-drwxrwxrwx   0        0        0        0 2023-06-19 19:00:29.370921 wows_shell-1.2.1/src/fitShell/out/build/x64-Debug (default)/CMakeFiles/
-drwxrwxrwx   0        0        0        0 2023-06-19 19:00:29.405621 wows_shell-1.2.1/src/fitShell/out/build/x64-Debug (default)/CMakeFiles/ShowIncludes/
--rw-rw-rw-   0        0        0        2 2021-01-23 06:11:50.000000 wows_shell-1.2.1/src/fitShell/out/build/x64-Debug (default)/CMakeFiles/ShowIncludes/foo.h
--rw-rw-rw-   0        0        0    24869 2023-06-19 14:50:35.000000 wows_shell-1.2.1/src/shell.hpp
--rw-rw-rw-   0        0        0    77483 2023-06-19 14:50:35.000000 wows_shell-1.2.1/src/shellCPP.hpp
-drwxrwxrwx   0        0        0        0 2023-06-19 19:00:29.373912 wows_shell-1.2.1/src/test/
-drwxrwxrwx   0        0        0        0 2023-06-19 19:00:29.373912 wows_shell-1.2.1/src/test/out/
-drwxrwxrwx   0        0        0        0 2023-06-19 19:00:29.375909 wows_shell-1.2.1/src/test/out/build/
-drwxrwxrwx   0        0        0        0 2023-06-19 19:00:29.374909 wows_shell-1.2.1/src/test/out/build/x64-Debug/
-drwxrwxrwx   0        0        0        0 2023-06-19 19:00:29.374909 wows_shell-1.2.1/src/test/out/build/x64-Debug/CMakeFiles/
-drwxrwxrwx   0        0        0        0 2023-06-19 19:00:29.409608 wows_shell-1.2.1/src/test/out/build/x64-Debug/CMakeFiles/ShowIncludes/
--rw-rw-rw-   0        0        0        2 2021-01-07 19:49:47.000000 wows_shell-1.2.1/src/test/out/build/x64-Debug/CMakeFiles/ShowIncludes/foo.h
-drwxrwxrwx   0        0        0        0 2023-06-19 19:00:29.375909 wows_shell-1.2.1/src/test/out/build/x64-Release/
-drwxrwxrwx   0        0        0        0 2023-06-19 19:00:29.376906 wows_shell-1.2.1/src/test/out/build/x64-Release/CMakeFiles/
-drwxrwxrwx   0        0        0        0 2023-06-19 19:00:29.411637 wows_shell-1.2.1/src/test/out/build/x64-Release/CMakeFiles/ShowIncludes/
--rw-rw-rw-   0        0        0        2 2021-01-07 19:53:01.000000 wows_shell-1.2.1/src/test/out/build/x64-Release/CMakeFiles/ShowIncludes/foo.h
--rw-rw-rw-   0        0        0     6534 2023-06-19 14:50:35.000000 wows_shell-1.2.1/src/utility.hpp
-drwxrwxrwx   0        0        0        0 2023-06-19 19:00:29.466108 wows_shell-1.2.1/src/version2/
--rw-rw-rw-   0        0        0    65564 2021-01-23 19:57:18.000000 wows_shell-1.2.1/src/version2/instrset.h
--rw-rw-rw-   0        0        0    16541 2021-01-23 19:57:18.000000 wows_shell-1.2.1/src/version2/vector_convert.h
--rw-rw-rw-   0        0        0     3357 2021-01-23 19:57:18.000000 wows_shell-1.2.1/src/version2/vectorclass.h
--rw-rw-rw-   0        0        0   103276 2021-01-23 19:57:18.000000 wows_shell-1.2.1/src/version2/vectorf128.h
--rw-rw-rw-   0        0        0   108363 2021-01-17 18:51:59.000000 wows_shell-1.2.1/src/version2/vectorf256.h
--rw-rw-rw-   0        0        0    65665 2021-01-17 18:51:59.000000 wows_shell-1.2.1/src/version2/vectorf256e.h
--rw-rw-rw-   0        0        0    78870 2021-01-17 18:51:59.000000 wows_shell-1.2.1/src/version2/vectorf512.h
--rw-rw-rw-   0        0        0    67972 2021-01-17 18:51:59.000000 wows_shell-1.2.1/src/version2/vectorf512e.h
--rw-rw-rw-   0        0        0   267691 2021-01-17 18:51:59.000000 wows_shell-1.2.1/src/version2/vectori128.h
--rw-rw-rw-   0        0        0   223226 2021-01-17 18:51:59.000000 wows_shell-1.2.1/src/version2/vectori256.h
--rw-rw-rw-   0        0        0   136921 2021-01-17 18:51:59.000000 wows_shell-1.2.1/src/version2/vectori256e.h
--rw-rw-rw-   0        0        0    85149 2021-01-17 18:51:59.000000 wows_shell-1.2.1/src/version2/vectori512.h
--rw-rw-rw-   0        0        0    79858 2021-01-17 18:51:59.000000 wows_shell-1.2.1/src/version2/vectori512e.h
--rw-rw-rw-   0        0        0    95406 2021-01-17 18:51:59.000000 wows_shell-1.2.1/src/version2/vectori512s.h
--rw-rw-rw-   0        0        0    74561 2021-01-17 18:51:59.000000 wows_shell-1.2.1/src/version2/vectori512se.h
--rw-rw-rw-   0        0        0    13288 2021-01-17 18:51:59.000000 wows_shell-1.2.1/src/version2/vectormath_common.h
--rw-rw-rw-   0        0        0    77691 2021-01-17 18:51:59.000000 wows_shell-1.2.1/src/version2/vectormath_exp.h
--rw-rw-rw-   0        0        0    22661 2021-01-17 18:51:59.000000 wows_shell-1.2.1/src/version2/vectormath_hyp.h
--rw-rw-rw-   0        0        0    77876 2021-01-17 18:51:59.000000 wows_shell-1.2.1/src/version2/vectormath_lib.h
--rw-rw-rw-   0        0        0    29775 2021-01-17 18:51:59.000000 wows_shell-1.2.1/src/version2/vectormath_trig.h
-drwxrwxrwx   0        0        0        0 2023-06-19 19:00:29.475083 wows_shell-1.2.1/wows_shell.egg-info/
--rw-rw-rw-   0        0        0     3257 2023-06-19 19:00:28.000000 wows_shell-1.2.1/wows_shell.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1204 2023-06-19 19:00:29.000000 wows_shell-1.2.1/wows_shell.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 19:00:28.000000 wows_shell-1.2.1/wows_shell.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-19 19:00:28.000000 wows_shell-1.2.1/wows_shell.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-22 03:24:03.894619 wows_shell-1.2.2/
+-rw-rw-rw-   0        0        0     1084 2020-07-28 13:49:29.000000 wows_shell-1.2.2/LICENSE
+-rw-rw-rw-   0        0        0       31 2021-01-23 20:09:16.000000 wows_shell-1.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3257 2023-06-22 03:24:03.894619 wows_shell-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3003 2020-12-29 19:40:43.000000 wows_shell-1.2.2/README.md
+-rw-rw-rw-   0        0        0      131 2021-01-23 20:09:16.000000 wows_shell-1.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-22 03:24:03.894619 wows_shell-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1095 2023-06-22 03:18:32.000000 wows_shell-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 03:24:03.853729 wows_shell-1.2.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-22 03:24:03.854726 wows_shell-1.2.2/src/Python/
+drwxrwxrwx   0        0        0        0 2023-06-22 03:24:03.837770 wows_shell-1.2.2/src/Python/out/
+drwxrwxrwx   0        0        0        0 2023-06-22 03:24:03.837770 wows_shell-1.2.2/src/Python/out/build/
+drwxrwxrwx   0        0        0        0 2023-06-22 03:24:03.838770 wows_shell-1.2.2/src/Python/out/build/x64-Debug (default)/
+drwxrwxrwx   0        0        0        0 2023-06-22 03:24:03.838770 wows_shell-1.2.2/src/Python/out/build/x64-Debug (default)/CMakeFiles/
+drwxrwxrwx   0        0        0        0 2023-06-22 03:24:03.855722 wows_shell-1.2.2/src/Python/out/build/x64-Debug (default)/CMakeFiles/ShowIncludes/
+-rw-rw-rw-   0        0        0        2 2021-01-23 06:11:54.000000 wows_shell-1.2.2/src/Python/out/build/x64-Debug (default)/CMakeFiles/ShowIncludes/foo.h
+-rw-rw-rw-   0        0        0    24784 2023-06-19 14:50:35.000000 wows_shell-1.2.2/src/Python/wows_shell_python.cpp
+-rw-rw-rw-   0        0        0     3197 2022-02-01 03:51:03.000000 wows_shell-1.2.2/src/controlEnums.hpp
+drwxrwxrwx   0        0        0        0 2023-06-22 03:24:03.838770 wows_shell-1.2.2/src/fitShell/
+drwxrwxrwx   0        0        0        0 2023-06-22 03:24:03.839765 wows_shell-1.2.2/src/fitShell/out/
+drwxrwxrwx   0        0        0        0 2023-06-22 03:24:03.840763 wows_shell-1.2.2/src/fitShell/out/build/
+drwxrwxrwx   0        0        0        0 2023-06-22 03:24:03.840763 wows_shell-1.2.2/src/fitShell/out/build/x64-Debug/
+drwxrwxrwx   0        0        0        0 2023-06-22 03:24:03.840763 wows_shell-1.2.2/src/fitShell/out/build/x64-Debug/CMakeFiles/
+drwxrwxrwx   0        0        0        0 2023-06-22 03:24:03.857717 wows_shell-1.2.2/src/fitShell/out/build/x64-Debug/CMakeFiles/ShowIncludes/
+-rw-rw-rw-   0        0        0        2 2020-12-26 00:29:01.000000 wows_shell-1.2.2/src/fitShell/out/build/x64-Debug/CMakeFiles/ShowIncludes/foo.h
+drwxrwxrwx   0        0        0        0 2023-06-22 03:24:03.839765 wows_shell-1.2.2/src/fitShell/out/build/x64-Debug (default)/
+drwxrwxrwx   0        0        0        0 2023-06-22 03:24:03.839765 wows_shell-1.2.2/src/fitShell/out/build/x64-Debug (default)/CMakeFiles/
+drwxrwxrwx   0        0        0        0 2023-06-22 03:24:03.856719 wows_shell-1.2.2/src/fitShell/out/build/x64-Debug (default)/CMakeFiles/ShowIncludes/
+-rw-rw-rw-   0        0        0        2 2021-01-23 06:11:50.000000 wows_shell-1.2.2/src/fitShell/out/build/x64-Debug (default)/CMakeFiles/ShowIncludes/foo.h
+-rw-rw-rw-   0        0        0    24869 2023-06-19 14:50:35.000000 wows_shell-1.2.2/src/shell.hpp
+-rw-rw-rw-   0        0        0    77537 2023-06-22 03:16:05.000000 wows_shell-1.2.2/src/shellCPP.hpp
+drwxrwxrwx   0        0        0        0 2023-06-22 03:24:03.841760 wows_shell-1.2.2/src/test/
+drwxrwxrwx   0        0        0        0 2023-06-22 03:24:03.841760 wows_shell-1.2.2/src/test/out/
+drwxrwxrwx   0        0        0        0 2023-06-22 03:24:03.842757 wows_shell-1.2.2/src/test/out/build/
+drwxrwxrwx   0        0        0        0 2023-06-22 03:24:03.842757 wows_shell-1.2.2/src/test/out/build/x64-Debug/
+drwxrwxrwx   0        0        0        0 2023-06-22 03:24:03.842757 wows_shell-1.2.2/src/test/out/build/x64-Debug/CMakeFiles/
+drwxrwxrwx   0        0        0        0 2023-06-22 03:24:03.857717 wows_shell-1.2.2/src/test/out/build/x64-Debug/CMakeFiles/ShowIncludes/
+-rw-rw-rw-   0        0        0        2 2021-01-07 19:49:47.000000 wows_shell-1.2.2/src/test/out/build/x64-Debug/CMakeFiles/ShowIncludes/foo.h
+drwxrwxrwx   0        0        0        0 2023-06-22 03:24:03.842757 wows_shell-1.2.2/src/test/out/build/x64-Release/
+drwxrwxrwx   0        0        0        0 2023-06-22 03:24:03.843754 wows_shell-1.2.2/src/test/out/build/x64-Release/CMakeFiles/
+drwxrwxrwx   0        0        0        0 2023-06-22 03:24:03.859714 wows_shell-1.2.2/src/test/out/build/x64-Release/CMakeFiles/ShowIncludes/
+-rw-rw-rw-   0        0        0        2 2021-01-07 19:53:01.000000 wows_shell-1.2.2/src/test/out/build/x64-Release/CMakeFiles/ShowIncludes/foo.h
+-rw-rw-rw-   0        0        0     6534 2023-06-19 14:50:35.000000 wows_shell-1.2.2/src/utility.hpp
+drwxrwxrwx   0        0        0        0 2023-06-22 03:24:03.888635 wows_shell-1.2.2/src/version2/
+-rw-rw-rw-   0        0        0    65564 2021-01-23 19:57:18.000000 wows_shell-1.2.2/src/version2/instrset.h
+-rw-rw-rw-   0        0        0    16541 2021-01-23 19:57:18.000000 wows_shell-1.2.2/src/version2/vector_convert.h
+-rw-rw-rw-   0        0        0     3357 2021-01-23 19:57:18.000000 wows_shell-1.2.2/src/version2/vectorclass.h
+-rw-rw-rw-   0        0        0   103276 2021-01-23 19:57:18.000000 wows_shell-1.2.2/src/version2/vectorf128.h
+-rw-rw-rw-   0        0        0   108363 2021-01-17 18:51:59.000000 wows_shell-1.2.2/src/version2/vectorf256.h
+-rw-rw-rw-   0        0        0    65665 2021-01-17 18:51:59.000000 wows_shell-1.2.2/src/version2/vectorf256e.h
+-rw-rw-rw-   0        0        0    78870 2021-01-17 18:51:59.000000 wows_shell-1.2.2/src/version2/vectorf512.h
+-rw-rw-rw-   0        0        0    67972 2021-01-17 18:51:59.000000 wows_shell-1.2.2/src/version2/vectorf512e.h
+-rw-rw-rw-   0        0        0   267691 2021-01-17 18:51:59.000000 wows_shell-1.2.2/src/version2/vectori128.h
+-rw-rw-rw-   0        0        0   223226 2021-01-17 18:51:59.000000 wows_shell-1.2.2/src/version2/vectori256.h
+-rw-rw-rw-   0        0        0   136921 2021-01-17 18:51:59.000000 wows_shell-1.2.2/src/version2/vectori256e.h
+-rw-rw-rw-   0        0        0    85149 2021-01-17 18:51:59.000000 wows_shell-1.2.2/src/version2/vectori512.h
+-rw-rw-rw-   0        0        0    79858 2021-01-17 18:51:59.000000 wows_shell-1.2.2/src/version2/vectori512e.h
+-rw-rw-rw-   0        0        0    95406 2021-01-17 18:51:59.000000 wows_shell-1.2.2/src/version2/vectori512s.h
+-rw-rw-rw-   0        0        0    74561 2021-01-17 18:51:59.000000 wows_shell-1.2.2/src/version2/vectori512se.h
+-rw-rw-rw-   0        0        0    13288 2021-01-17 18:51:59.000000 wows_shell-1.2.2/src/version2/vectormath_common.h
+-rw-rw-rw-   0        0        0    77691 2021-01-17 18:51:59.000000 wows_shell-1.2.2/src/version2/vectormath_exp.h
+-rw-rw-rw-   0        0        0    22661 2021-01-17 18:51:59.000000 wows_shell-1.2.2/src/version2/vectormath_hyp.h
+-rw-rw-rw-   0        0        0    77876 2021-01-17 18:51:59.000000 wows_shell-1.2.2/src/version2/vectormath_lib.h
+-rw-rw-rw-   0        0        0    29775 2021-01-17 18:51:59.000000 wows_shell-1.2.2/src/version2/vectormath_trig.h
+drwxrwxrwx   0        0        0        0 2023-06-22 03:24:03.892624 wows_shell-1.2.2/wows_shell.egg-info/
+-rw-rw-rw-   0        0        0     3257 2023-06-22 03:24:03.000000 wows_shell-1.2.2/wows_shell.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1204 2023-06-22 03:24:03.000000 wows_shell-1.2.2/wows_shell.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 03:24:03.000000 wows_shell-1.2.2/wows_shell.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-22 03:24:03.000000 wows_shell-1.2.2/wows_shell.egg-info/top_level.txt
```

### Comparing `wows_shell-1.2.1/LICENSE` & `wows_shell-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wows_shell-1.2.1/PKG-INFO` & `wows_shell-1.2.2/wows_shell.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: wows_shell
-Version: 1.2.1
+Name: wows-shell
+Version: 1.2.2
 Summary: Python extension of wows_shell
 Home-page: https://github.com/jcw780/wows_shell
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `wows_shell-1.2.1/README.md` & `wows_shell-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `wows_shell-1.2.1/setup.py` & `wows_shell-1.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     cxx_compile_args.append('-march=native')
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="wows_shell",
-    version="1.2.1",
+    version="1.2.2",
     description="Python extension of wows_shell",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jcw780/wows_shell",
     cmdclass={"build_ext": build_ext},
     ext_modules=ext_modules,
 )
```

### Comparing `wows_shell-1.2.1/src/Python/wows_shell_python.cpp` & `wows_shell-1.2.2/src/Python/wows_shell_python.cpp`

 * *Files identical despite different names*

### Comparing `wows_shell-1.2.1/src/controlEnums.hpp` & `wows_shell-1.2.2/src/controlEnums.hpp`

 * *Files identical despite different names*

### Comparing `wows_shell-1.2.1/src/shell.hpp` & `wows_shell-1.2.2/src/shell.hpp`

 * *Files identical despite different names*

### Comparing `wows_shell-1.2.1/src/shellCPP.hpp` & `wows_shell-1.2.2/src/shellCPP.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     // TODO: Static Constexpr these
     // Physical Constants     Description                  | Units
     static constexpr double g = 9.8;  // Gravitational Constant       | m/(s^2)
     static constexpr double t0 = 288.15;  // Temperature at Sea Level     | K
     static constexpr double L = 0.0065;   // Atmospheric Lapse Rate       | C/m
     static constexpr double p0 = 101325;  // Pressure at Sea Level        | Pa
     static constexpr double R =
-        8.31447;  // Ideal Gas Constant           | J/(mol K)
+        8.31447;    // Ideal Gas Constant           | J/(mol K)
     static constexpr double M =
         0.0289644;  // Molarity of Air at Sea Level | kg/mol
     static constexpr double cw_1 = 1;
 
     static constexpr double gMRL = (g * M) / (R * L);
     // Calculation Parameters
     double maxA = 25;       // Max Angle                    | degrees
@@ -47,15 +47,15 @@
     double precision = .1;  // Angle Step                   | degrees
     double x0 = 0, y0 = 0;  // Starting x0, y0              | m
     double dt_min = .02;    // Time step                    | s
 
     static constexpr double timeMultiplier = 2.75;
     // For some reason the game has a different shell multiplier than the
     // global speed multiplier of 2.61 used for everything else.
-    static constexpr double velocityPower = 2*0.69;
+    static constexpr double velocityPower = 2 * 0.69;
     // Effect of impact velocity on penetration: P = K * v ^ velocity power
 
     // delta t (dtf) for fusing needs to be smaller than the delta t (dt) used
     // for trajectories due to the shorter distances. Otherwise results become
     // jagged - precision suffers.
     double dtf = 0.0001;
     double xf0 = 0, yf0 = 0;
@@ -86,16 +86,17 @@
     mutable std::atomic<std::size_t> counter{0};
 
    public:
 #if defined(__SSE4_1__) || defined(__AVX__)
     VT calcNormalizationR(
         const VT angle,
         const double normalizationR) const noexcept {  // Input in radians
-        auto gt = angle > VT(normalizationR);
-        return select(gt, angle - VT(normalizationR), VT(0));
+        auto abs_angle = abs(angle);
+        auto gt = abs_angle > VT(normalizationR);
+        return select(gt, abs_angle - VT(normalizationR), VT(0));
         // Don't worry this branch goes away
     }
 #endif
     double calcNormalizationR(
         const double angle,
         const double normalizationR) const noexcept {  // Input in radians
         return fabs(angle) > normalizationR ? fabs(angle) - normalizationR : 0;
@@ -1563,15 +1564,15 @@
             vSize, penetrationV.data());
         std::copy_n(
             s.get_impactPtr(distIndex, impact::impactIndices::impactVelocity),
             vSize, v0V.data());
 
         for (uint32_t l = 0; l < vSize; l++) {
             const double HA_R =
-                hAngleV[l] * M_PI / 180;  // lateral  angle radians
+                hAngleV[l] * M_PI / 180;     // lateral  angle radians
             const double VA_R =
                 vAngleV[l] + inclination_R;  // vertical angle radians
             const double cAngle = acos(cos(HA_R) * cos(VA_R));
             const double nCAngle =
                 calcNormalizationR(cAngle, s.get_normalizationR());
             const double eThickness = thickness / cos(nCAngle);
             const double pPV =
@@ -1595,15 +1596,15 @@
                 v_z[l] = pPV * cos(VA_R) * sin(HA_R);
                 v_y[l] = pPV * sin(VA_R);
             }
             eThicknessV[l] = eThickness;
         }
 #endif
 
-        //#pragma clang loop vectorize(enable)
+        // #pragma clang loop vectorize(enable)
         const std::size_t loopSize =
             std::min<std::size_t>(vSize, s.postPenSize - i);
         for (std::size_t j = 0; j < loopSize; j++) {
             postPenTraj<fast>(i + j, s, v_x[j], v_y[j], v_z[j], eThicknessV[j]);
         }
         // std::cout<<index<<" Completed\n";
     }
```

### Comparing `wows_shell-1.2.1/src/utility.hpp` & `wows_shell-1.2.2/src/utility.hpp`

 * *Files identical despite different names*

### Comparing `wows_shell-1.2.1/src/version2/instrset.h` & `wows_shell-1.2.2/src/version2/instrset.h`

 * *Files identical despite different names*

### Comparing `wows_shell-1.2.1/src/version2/vector_convert.h` & `wows_shell-1.2.2/src/version2/vector_convert.h`

 * *Files identical despite different names*

### Comparing `wows_shell-1.2.1/src/version2/vectorclass.h` & `wows_shell-1.2.2/src/version2/vectorclass.h`

 * *Files identical despite different names*

### Comparing `wows_shell-1.2.1/src/version2/vectorf128.h` & `wows_shell-1.2.2/src/version2/vectorf128.h`

 * *Files identical despite different names*

### Comparing `wows_shell-1.2.1/src/version2/vectorf256.h` & `wows_shell-1.2.2/src/version2/vectorf256.h`

 * *Files identical despite different names*

### Comparing `wows_shell-1.2.1/src/version2/vectorf256e.h` & `wows_shell-1.2.2/src/version2/vectorf256e.h`

 * *Files identical despite different names*

### Comparing `wows_shell-1.2.1/src/version2/vectorf512.h` & `wows_shell-1.2.2/src/version2/vectorf512.h`

 * *Files identical despite different names*

### Comparing `wows_shell-1.2.1/src/version2/vectorf512e.h` & `wows_shell-1.2.2/src/version2/vectorf512e.h`

 * *Files identical despite different names*

### Comparing `wows_shell-1.2.1/src/version2/vectori128.h` & `wows_shell-1.2.2/src/version2/vectori128.h`

 * *Files identical despite different names*

### Comparing `wows_shell-1.2.1/src/version2/vectori256.h` & `wows_shell-1.2.2/src/version2/vectori256.h`

 * *Files identical despite different names*

### Comparing `wows_shell-1.2.1/src/version2/vectori256e.h` & `wows_shell-1.2.2/src/version2/vectori256e.h`

 * *Files identical despite different names*

### Comparing `wows_shell-1.2.1/src/version2/vectori512.h` & `wows_shell-1.2.2/src/version2/vectori512.h`

 * *Files identical despite different names*

### Comparing `wows_shell-1.2.1/src/version2/vectori512e.h` & `wows_shell-1.2.2/src/version2/vectori512e.h`

 * *Files identical despite different names*

### Comparing `wows_shell-1.2.1/src/version2/vectori512s.h` & `wows_shell-1.2.2/src/version2/vectori512s.h`

 * *Files identical despite different names*

### Comparing `wows_shell-1.2.1/src/version2/vectori512se.h` & `wows_shell-1.2.2/src/version2/vectori512se.h`

 * *Files identical despite different names*

### Comparing `wows_shell-1.2.1/src/version2/vectormath_common.h` & `wows_shell-1.2.2/src/version2/vectormath_common.h`

 * *Files identical despite different names*

### Comparing `wows_shell-1.2.1/src/version2/vectormath_exp.h` & `wows_shell-1.2.2/src/version2/vectormath_exp.h`

 * *Files identical despite different names*

### Comparing `wows_shell-1.2.1/src/version2/vectormath_hyp.h` & `wows_shell-1.2.2/src/version2/vectormath_hyp.h`

 * *Files identical despite different names*

### Comparing `wows_shell-1.2.1/src/version2/vectormath_lib.h` & `wows_shell-1.2.2/src/version2/vectormath_lib.h`

 * *Files identical despite different names*

### Comparing `wows_shell-1.2.1/src/version2/vectormath_trig.h` & `wows_shell-1.2.2/src/version2/vectormath_trig.h`

 * *Files identical despite different names*

### Comparing `wows_shell-1.2.1/wows_shell.egg-info/PKG-INFO` & `wows_shell-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: wows-shell
-Version: 1.2.1
+Name: wows_shell
+Version: 1.2.2
 Summary: Python extension of wows_shell
 Home-page: https://github.com/jcw780/wows_shell
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `wows_shell-1.2.1/wows_shell.egg-info/SOURCES.txt` & `wows_shell-1.2.2/wows_shell.egg-info/SOURCES.txt`

 * *Files identical despite different names*

