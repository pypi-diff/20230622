# Comparing `tmp/testkafkainitialcleint-1.0.0.tar.gz` & `tmp/testkafkainitialcleint-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testkafkainitialcleint-1.0.0.tar", last modified: Thu Jun 22 09:15:57 2023, max compression
+gzip compressed data, was "testkafkainitialcleint-1.0.1.tar", last modified: Thu Jun 22 09:17:36 2023, max compression
```

## Comparing `testkafkainitialcleint-1.0.0.tar` & `testkafkainitialcleint-1.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-06-22 09:15:57.530115 testkafkainitialcleint-1.0.0/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      185 2023-06-22 09:15:57.529999 testkafkainitialcleint-1.0.0/PKG-INFO
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       85 2023-06-22 09:15:02.000000 testkafkainitialcleint-1.0.0/my_pip_package.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       38 2023-06-22 09:15:57.530148 testkafkainitialcleint-1.0.0/setup.cfg
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      306 2023-06-22 09:15:37.000000 testkafkainitialcleint-1.0.0/setup.py
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-06-22 09:15:57.529855 testkafkainitialcleint-1.0.0/testkafkainitialcleint.egg-info/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      185 2023-06-22 09:15:57.000000 testkafkainitialcleint-1.0.0/testkafkainitialcleint.egg-info/PKG-INFO
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      210 2023-06-22 09:15:57.000000 testkafkainitialcleint-1.0.0/testkafkainitialcleint.egg-info/SOURCES.txt
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        1 2023-06-22 09:15:57.000000 testkafkainitialcleint-1.0.0/testkafkainitialcleint.egg-info/dependency_links.txt
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       15 2023-06-22 09:15:57.000000 testkafkainitialcleint-1.0.0/testkafkainitialcleint.egg-info/top_level.txt
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-06-22 09:17:36.542853 testkafkainitialcleint-1.0.1/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      185 2023-06-22 09:17:36.542749 testkafkainitialcleint-1.0.1/PKG-INFO
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       85 2023-06-22 09:17:21.000000 testkafkainitialcleint-1.0.1/my_pip_package.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       38 2023-06-22 09:17:36.542887 testkafkainitialcleint-1.0.1/setup.cfg
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      306 2023-06-22 09:15:37.000000 testkafkainitialcleint-1.0.1/setup.py
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-06-22 09:17:36.542611 testkafkainitialcleint-1.0.1/testkafkainitialcleint.egg-info/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      185 2023-06-22 09:17:36.000000 testkafkainitialcleint-1.0.1/testkafkainitialcleint.egg-info/PKG-INFO
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      210 2023-06-22 09:17:36.000000 testkafkainitialcleint-1.0.1/testkafkainitialcleint.egg-info/SOURCES.txt
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        1 2023-06-22 09:17:36.000000 testkafkainitialcleint-1.0.1/testkafkainitialcleint.egg-info/dependency_links.txt
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       15 2023-06-22 09:17:36.000000 testkafkainitialcleint-1.0.1/testkafkainitialcleint.egg-info/top_level.txt
```

