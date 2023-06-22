# Comparing `tmp/myoktros-0.0.2.tar.gz` & `tmp/myoktros-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myoktros-0.0.2.tar", max compression
+gzip compressed data, was "myoktros-0.1.0.tar", max compression
```

## Comparing `myoktros-0.0.2.tar` & `myoktros-0.1.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1091 2023-06-14 23:53:33.677031 myoktros-0.0.2/LICENSE
--rw-r--r--   0        0        0     3769 2023-06-14 23:53:33.677031 myoktros-0.0.2/README.md
--rw-r--r--   0        0        0     3214 2023-06-14 23:54:22.933186 myoktros-0.0.2/pyproject.toml
--rwxr-xr-x   0        0        0     4374 2023-06-14 23:53:33.681031 myoktros-0.0.2/src/myoktros/__init__.py
--rw-r--r--   0        0        0     2054 2023-06-14 23:53:33.681031 myoktros-0.0.2/src/myoktros/gesture.py
--rw-r--r--   0        0        0      128 2023-06-14 23:53:33.681031 myoktros-0.0.2/src/myoktros/kt_mode.py
--rw-r--r--   0        0        0     6158 2023-06-14 23:53:33.681031 myoktros-0.0.2/src/myoktros/myo_manager.py
--rw-r--r--   0        0        0     4337 2023-06-14 23:53:33.681031 myoktros-0.0.2/src/myoktros/ros.py
--rw-r--r--   0        0        0     4437 1970-01-01 00:00:00.000000 myoktros-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-06-22 17:59:33.647998 myoktros-0.1.0/LICENSE
+-rw-r--r--   0        0        0     9765 2023-06-22 17:59:33.647998 myoktros-0.1.0/README.md
+-rw-r--r--   0        0        0     3334 2023-06-22 18:00:26.923932 myoktros-0.1.0/pyproject.toml
+-rwxr-xr-x   0        0        0     7016 2023-06-22 17:59:33.647998 myoktros-0.1.0/src/myoktros/__init__.py
+-rw-r--r--   0        0        0     8729 2023-06-22 17:59:33.647998 myoktros-0.1.0/src/myoktros/client.py
+-rw-r--r--   0        0        0     2134 2023-06-22 17:59:33.647998 myoktros-0.1.0/src/myoktros/command.py
+-rw-r--r--   0        0        0     6445 2023-06-22 17:59:33.647998 myoktros-0.1.0/src/myoktros/gesture.py
+-rw-r--r--   0        0        0     9298 2023-06-22 17:59:33.647998 myoktros-0.1.0/src/myoktros/robot.py
+-rw-r--r--   0        0        0    10473 1970-01-01 00:00:00.000000 myoktros-0.1.0/PKG-INFO
```

### Comparing `myoktros-0.0.2/LICENSE` & `myoktros-0.1.0/LICENSE`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Felix Wohlgemuth and Iori Mizutani
+Copyright (c) 2023 Iori Mizutani and Felix Wohlgemuth
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `myoktros-0.0.2/pyproject.toml` & `myoktros-0.1.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [project]
 name = "MyoKTROS"
 authors = [
-  { name="Iori Mizutani", email="iori.mizutani@gmail.com" },
+  { name="Iori Mizutani", email="iomz@sazanka.io" },
   { name="Felix Wohlgemuth", email="felixwohlgemuth@gmx.ch" },
 ]
 maintainers = [
-  { name="Iori Mizutani", email="iori.mizutani@gmail.com" },
+  { name="Iori Mizutani", email="iomz@sazanka.io" },
 ]
 description = "Myo EMG-based KT system for ROS"
 readme = "README.md"
 classifiers = [
     "Environment :: Console",
     "Framework :: AsyncIO",
     "Framework :: Robot Framework :: Tool",
     "Intended Audience :: Developers",
     "Intended Audience :: Education",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Topic :: Scientific/Engineering :: Human Machine Interfaces",
 ]
 dynamic = ["version"]
 
 [project.urls]
 "Homepage" = "https://github.com/Interactions-HSG/MyoKTROS"
@@ -90,33 +91,37 @@
   "no cov",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
 ]
 
 [tool.poetry]
 name = "MyoKTROS"
-version = "0.0.2"
+version = "0.1.0"
 description = "Myo EMG-based KT system for ROS"
-authors = ["Iori Mizutani <iori.mizutani@gmail.com>"]
+authors = ["Iori Mizutani <iomz@sazanka.io>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.11"
-dl-myo = ">=0.2.0"
+dl-myo = ">=1.0.3"
 joblib = "^1.2.0"
 numpy = "^1.24.3"
 pandas = "^2.0.2"
 scikit-learn = "^1.2.2"
-tensorflow = ">=2.12.0"
+tensorflow = ">=2.13.0rc1"
+transitions = "^0.9.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pytest = "^7.3.2"
 pytest-cov = "^4.1.0"
+pytest-asyncio = "^0.21.0"
+transitions-gui = "^0.1.0"
+tornado = "^6.3.2"
 
 [tool.poetry.scripts]
 myoktros = "myoktros:entrypoint"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
```

