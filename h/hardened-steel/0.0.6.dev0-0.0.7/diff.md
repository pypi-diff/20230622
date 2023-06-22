# Comparing `tmp/hardened-steel-0.0.6.dev0.tar.gz` & `tmp/hardened-steel-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hardened-steel-0.0.6.dev0.tar", last modified: Thu Jun 22 11:58:35 2023, max compression
+gzip compressed data, was "hardened-steel-0.0.7.tar", last modified: Thu Jun 22 12:13:32 2023, max compression
```

## Comparing `hardened-steel-0.0.6.dev0.tar` & `hardened-steel-0.0.7.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:58:35.051432 hardened-steel-0.0.6.dev0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:58:35.047432 hardened-steel-0.0.6.dev0/HardenedSteel/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-22 11:58:15.000000 hardened-steel-0.0.6.dev0/HardenedSteel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:58:35.047432 hardened-steel-0.0.6.dev0/HardenedSteel/facades/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-22 11:58:15.000000 hardened-steel-0.0.6.dev0/HardenedSteel/facades/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:58:35.047432 hardened-steel-0.0.6.dev0/HardenedSteel/facades/booleans/
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-22 11:58:15.000000 hardened-steel-0.0.6.dev0/HardenedSteel/facades/booleans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-22 11:58:15.000000 hardened-steel-0.0.6.dev0/HardenedSteel/facades/booleans/random_boolean_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:58:35.047432 hardened-steel-0.0.6.dev0/HardenedSteel/facades/integers/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-22 11:58:15.000000 hardened-steel-0.0.6.dev0/HardenedSteel/facades/integers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-22 11:58:15.000000 hardened-steel-0.0.6.dev0/HardenedSteel/facades/integers/random_number_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:58:35.047432 hardened-steel-0.0.6.dev0/HardenedSteel/facades/texts/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-22 11:58:15.000000 hardened-steel-0.0.6.dev0/HardenedSteel/facades/texts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:58:35.051432 hardened-steel-0.0.6.dev0/HardenedSteel/facades/texts/characters/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-22 11:58:15.000000 hardened-steel-0.0.6.dev0/HardenedSteel/facades/texts/characters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-22 11:58:15.000000 hardened-steel-0.0.6.dev0/HardenedSteel/facades/texts/characters/ranges.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-22 11:58:15.000000 hardened-steel-0.0.6.dev0/HardenedSteel/facades/texts/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-06-22 11:58:15.000000 hardened-steel-0.0.6.dev0/HardenedSteel/facades/texts/random_text_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:58:35.051432 hardened-steel-0.0.6.dev0/HardenedSteel/globals/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-22 11:58:15.000000 hardened-steel-0.0.6.dev0/HardenedSteel/globals/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:58:35.051432 hardened-steel-0.0.6.dev0/HardenedSteel/globals/singletons/
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-22 11:58:15.000000 hardened-steel-0.0.6.dev0/HardenedSteel/globals/singletons/SingletonSystenRandom.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-22 11:58:15.000000 hardened-steel-0.0.6.dev0/HardenedSteel/globals/singletons/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:58:35.051432 hardened-steel-0.0.6.dev0/HardenedSteel/globals/vars/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-22 11:58:15.000000 hardened-steel-0.0.6.dev0/HardenedSteel/globals/vars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-22 11:58:15.000000 hardened-steel-0.0.6.dev0/HardenedSteel/globals/vars/integer.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-22 11:58:35.051432 hardened-steel-0.0.6.dev0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:58:35.051432 hardened-steel-0.0.6.dev0/hardened_steel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-22 11:58:35.000000 hardened-steel-0.0.6.dev0/hardened_steel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-22 11:58:35.000000 hardened-steel-0.0.6.dev0/hardened_steel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 11:58:35.000000 hardened-steel-0.0.6.dev0/hardened_steel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-22 11:58:35.000000 hardened-steel-0.0.6.dev0/hardened_steel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-22 11:58:15.000000 hardened-steel-0.0.6.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 11:58:35.051432 hardened-steel-0.0.6.dev0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:58:35.051432 hardened-steel-0.0.6.dev0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-22 11:58:15.000000 hardened-steel-0.0.6.dev0/tests/test_default.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-22 11:58:15.000000 hardened-steel-0.0.6.dev0/tests/test_singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:13:32.261771 hardened-steel-0.0.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:13:32.257771 hardened-steel-0.0.7/HardenedSteel/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-22 12:13:08.000000 hardened-steel-0.0.7/HardenedSteel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:13:32.257771 hardened-steel-0.0.7/HardenedSteel/facades/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-22 12:13:08.000000 hardened-steel-0.0.7/HardenedSteel/facades/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:13:32.257771 hardened-steel-0.0.7/HardenedSteel/facades/booleans/
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-22 12:13:08.000000 hardened-steel-0.0.7/HardenedSteel/facades/booleans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-22 12:13:08.000000 hardened-steel-0.0.7/HardenedSteel/facades/booleans/random_boolean_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:13:32.257771 hardened-steel-0.0.7/HardenedSteel/facades/integers/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-22 12:13:08.000000 hardened-steel-0.0.7/HardenedSteel/facades/integers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-22 12:13:08.000000 hardened-steel-0.0.7/HardenedSteel/facades/integers/random_number_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:13:32.257771 hardened-steel-0.0.7/HardenedSteel/facades/texts/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-22 12:13:08.000000 hardened-steel-0.0.7/HardenedSteel/facades/texts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:13:32.261771 hardened-steel-0.0.7/HardenedSteel/facades/texts/characters/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-22 12:13:08.000000 hardened-steel-0.0.7/HardenedSteel/facades/texts/characters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-22 12:13:08.000000 hardened-steel-0.0.7/HardenedSteel/facades/texts/characters/ranges.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-22 12:13:08.000000 hardened-steel-0.0.7/HardenedSteel/facades/texts/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-06-22 12:13:08.000000 hardened-steel-0.0.7/HardenedSteel/facades/texts/random_text_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:13:32.261771 hardened-steel-0.0.7/HardenedSteel/globals/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-22 12:13:08.000000 hardened-steel-0.0.7/HardenedSteel/globals/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:13:32.261771 hardened-steel-0.0.7/HardenedSteel/globals/singletons/
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-22 12:13:08.000000 hardened-steel-0.0.7/HardenedSteel/globals/singletons/SingletonSystenRandom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-22 12:13:08.000000 hardened-steel-0.0.7/HardenedSteel/globals/singletons/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:13:32.261771 hardened-steel-0.0.7/HardenedSteel/globals/vars/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-22 12:13:08.000000 hardened-steel-0.0.7/HardenedSteel/globals/vars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-22 12:13:08.000000 hardened-steel-0.0.7/HardenedSteel/globals/vars/integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-22 12:13:08.000000 hardened-steel-0.0.7/License.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-06-22 12:13:32.261771 hardened-steel-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-22 12:13:08.000000 hardened-steel-0.0.7/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:13:32.261771 hardened-steel-0.0.7/hardened_steel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-06-22 12:13:32.000000 hardened-steel-0.0.7/hardened_steel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-22 12:13:32.000000 hardened-steel-0.0.7/hardened_steel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 12:13:32.000000 hardened-steel-0.0.7/hardened_steel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-22 12:13:32.000000 hardened-steel-0.0.7/hardened_steel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-22 12:13:08.000000 hardened-steel-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 12:13:32.261771 hardened-steel-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:13:32.261771 hardened-steel-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-22 12:13:08.000000 hardened-steel-0.0.7/tests/test_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-22 12:13:08.000000 hardened-steel-0.0.7/tests/test_singleton.py
```

### Comparing `hardened-steel-0.0.6.dev0/HardenedSteel/facades/integers/random_number_generation.py` & `hardened-steel-0.0.7/HardenedSteel/facades/integers/random_number_generation.py`

 * *Files identical despite different names*

### Comparing `hardened-steel-0.0.6.dev0/HardenedSteel/facades/texts/characters/ranges.py` & `hardened-steel-0.0.7/HardenedSteel/facades/texts/characters/ranges.py`

 * *Files identical despite different names*

### Comparing `hardened-steel-0.0.6.dev0/HardenedSteel/facades/texts/random_text_generation.py` & `hardened-steel-0.0.7/HardenedSteel/facades/texts/random_text_generation.py`

 * *Files identical despite different names*

### Comparing `hardened-steel-0.0.6.dev0/HardenedSteel/globals/__init__.py` & `hardened-steel-0.0.7/HardenedSteel/globals/__init__.py`

 * *Files identical despite different names*

### Comparing `hardened-steel-0.0.6.dev0/HardenedSteel/globals/singletons/SingletonSystenRandom.py` & `hardened-steel-0.0.7/HardenedSteel/globals/singletons/SingletonSystenRandom.py`

 * *Files identical despite different names*

### Comparing `hardened-steel-0.0.6.dev0/HardenedSteel/globals/vars/integer.py` & `hardened-steel-0.0.7/HardenedSteel/globals/vars/integer.py`

 * *Files identical despite different names*

### Comparing `hardened-steel-0.0.6.dev0/hardened_steel.egg-info/SOURCES.txt` & `hardened-steel-0.0.7/hardened_steel.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+License.md
+Readme.md
 pyproject.toml
 HardenedSteel/__init__.py
 HardenedSteel/facades/__init__.py
 HardenedSteel/facades/booleans/__init__.py
 HardenedSteel/facades/booleans/random_boolean_generation.py
 HardenedSteel/facades/integers/__init__.py
 HardenedSteel/facades/integers/random_number_generation.py
```

### Comparing `hardened-steel-0.0.6.dev0/pyproject.toml` & `hardened-steel-0.0.7/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
+requires-python = ">=3.10"
+
 name = "hardened-steel"
-version = "0.0.6-dev"
+version = "0.0.7"
+
 authors = [
   { name="IO Jægers", email="support@cloud.iojaegers.com" },
   { name="Kent Madsen", email="kent.vejrup.madsen@outlook.com" },
 ]
+
 description = "Framework for helping to test projects with the generation of random data during TDD"
-readme = "README.md"
-requires-python = ">=3.10"
+
+readme = "Readme.md"
+license = {file='License.md'}
+
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
@@ -25,8 +31,8 @@
 "Releases" = "https://pypi.org/manage/project/hardened-steel/releases/"
 
 [tool.setuptools]
 include-package-data = false
 
 [tool.setuptools.packages.find]
 include = ["HardenedSteel*"]
-exclude = ["docs*", "tests*"]
+exclude = ["docs*", "tests*"]
```

