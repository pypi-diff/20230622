# Comparing `tmp/bubble_api-0.3.1.tar.gz` & `tmp/bubble_api-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "bubble_api-0.4.0.tar", last modified: Thu Jun 22 10:25:13 2023, max compression
```

## Comparing `bubble_api-0.3.1.tar` & `bubble_api-0.4.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 bubble_api-0.3.1/requirements.txt
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 bubble_api-0.3.1/.idea/.gitignore
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 bubble_api-0.3.1/.idea/bubble-api.iml
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 bubble_api-0.3.1/.idea/misc.xml
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 bubble_api-0.3.1/.idea/modules.xml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 bubble_api-0.3.1/.idea/vcs.xml
--rw-r--r--   0        0        0    10516 2020-02-02 00:00:00.000000 bubble_api-0.3.1/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 bubble_api-0.3.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bubble_api-0.3.1/src/bubble_api/__init__.py
--rw-r--r--   0        0        0    56334 2020-02-02 00:00:00.000000 bubble_api-0.3.1/src/bubble_api/bubble.py
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 bubble_api-0.3.1/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 bubble_api-0.3.1/LICENSE
--rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 bubble_api-0.3.1/README.md
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 bubble_api-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 bubble_api-0.3.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-22 10:25:13.530379 bubble_api-0.4.0/
+-rw-rw-rw-   0        0        0     1105 2023-06-22 10:19:29.000000 bubble_api-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0     3422 2023-06-22 10:25:13.530379 bubble_api-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2575 2023-06-22 10:19:29.000000 bubble_api-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 10:25:13.505137 bubble_api-0.4.0/bubble_api/
+-rw-rw-rw-   0        0        0       98 2023-06-22 10:19:29.000000 bubble_api-0.4.0/bubble_api/__init__.py
+-rw-rw-rw-   0        0        0     1230 2023-06-22 10:19:29.000000 bubble_api-0.4.0/bubble_api/constraint.py
+-rw-rw-rw-   0        0        0     2438 2023-06-22 10:19:29.000000 bubble_api-0.4.0/bubble_api/field.py
+-rw-rw-rw-   0        0        0     9600 2023-06-22 10:19:29.000000 bubble_api-0.4.0/bubble_api/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-06-22 10:25:13.517645 bubble_api-0.4.0/bubble_api.egg-info/
+-rw-rw-rw-   0        0        0     3422 2023-06-22 10:25:13.000000 bubble_api-0.4.0/bubble_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      301 2023-06-22 10:25:13.000000 bubble_api-0.4.0/bubble_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 10:25:13.000000 bubble_api-0.4.0/bubble_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-22 10:25:13.000000 bubble_api-0.4.0/bubble_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-22 10:25:13.000000 bubble_api-0.4.0/bubble_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1015 2023-06-22 10:19:29.000000 bubble_api-0.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0      100 2023-06-22 10:25:13.530379 bubble_api-0.4.0/setup.cfg
```

### Comparing `bubble_api-0.3.1/LICENSE` & `bubble_api-0.4.0/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 settorac-nina
+Copyright (c) 2023 Dylan Nina & Mathis Bourdin
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

