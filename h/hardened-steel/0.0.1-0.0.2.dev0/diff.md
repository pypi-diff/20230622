# Comparing `tmp/hardened-steel-0.0.1.tar.gz` & `tmp/hardened-steel-0.0.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hardened-steel-0.0.1.tar", last modified: Wed Jun 21 20:32:51 2023, max compression
+gzip compressed data, was "hardened-steel-0.0.2.dev0.tar", last modified: Wed Jun 21 22:36:23 2023, max compression
```

## Comparing `hardened-steel-0.0.1.tar` & `hardened-steel-0.0.2.dev0.tar`

### file list

```diff
@@ -1,11 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:32:51.255900 hardened-steel-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-21 20:32:51.255900 hardened-steel-0.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:32:51.255900 hardened-steel-0.0.1/hardened_steel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-21 20:32:51.000000 hardened-steel-0.0.1/hardened_steel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-21 20:32:51.000000 hardened-steel-0.0.1/hardened_steel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 20:32:51.000000 hardened-steel-0.0.1/hardened_steel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 20:32:51.000000 hardened-steel-0.0.1/hardened_steel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-21 20:32:39.000000 hardened-steel-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 20:32:51.255900 hardened-steel-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:32:51.255900 hardened-steel-0.0.1/steel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 20:32:39.000000 hardened-steel-0.0.1/steel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:36:23.469661 hardened-steel-0.0.2.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-21 22:36:23.469661 hardened-steel-0.0.2.dev0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:36:23.469661 hardened-steel-0.0.2.dev0/hardened_steel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-21 22:36:23.000000 hardened-steel-0.0.2.dev0/hardened_steel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-21 22:36:23.000000 hardened-steel-0.0.2.dev0/hardened_steel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 22:36:23.000000 hardened-steel-0.0.2.dev0/hardened_steel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 22:36:23.000000 hardened-steel-0.0.2.dev0/hardened_steel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-21 22:36:11.000000 hardened-steel-0.0.2.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 22:36:23.469661 hardened-steel-0.0.2.dev0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:36:23.469661 hardened-steel-0.0.2.dev0/steel/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-21 22:36:11.000000 hardened-steel-0.0.2.dev0/steel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:36:23.469661 hardened-steel-0.0.2.dev0/steel/facades/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-21 22:36:11.000000 hardened-steel-0.0.2.dev0/steel/facades/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:36:23.469661 hardened-steel-0.0.2.dev0/steel/facades/texts/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-21 22:36:11.000000 hardened-steel-0.0.2.dev0/steel/facades/texts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:36:23.469661 hardened-steel-0.0.2.dev0/steel/facades/texts/characters/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-21 22:36:11.000000 hardened-steel-0.0.2.dev0/steel/facades/texts/characters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-21 22:36:11.000000 hardened-steel-0.0.2.dev0/steel/facades/texts/characters/ranges.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-21 22:36:11.000000 hardened-steel-0.0.2.dev0/steel/facades/texts/random_text_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:36:23.469661 hardened-steel-0.0.2.dev0/steel/globals/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-21 22:36:11.000000 hardened-steel-0.0.2.dev0/steel/globals/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:36:23.469661 hardened-steel-0.0.2.dev0/steel/globals/singletons/
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-21 22:36:11.000000 hardened-steel-0.0.2.dev0/steel/globals/singletons/SingletonSystenRandom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-21 22:36:11.000000 hardened-steel-0.0.2.dev0/steel/globals/singletons/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:36:23.469661 hardened-steel-0.0.2.dev0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-21 22:36:11.000000 hardened-steel-0.0.2.dev0/tests/test_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-21 22:36:11.000000 hardened-steel-0.0.2.dev0/tests/test_singleton.py
```

### Comparing `hardened-steel-0.0.1/PKG-INFO` & `hardened-steel-0.0.2.dev0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: hardened-steel
-Version: 0.0.1
-Summary: Framework for helping to test projects with the generation of data
+Version: 0.0.2.dev0
+Summary: Framework for helping to test projects with the generation of random data during TDD
 Author-email: IO Jægers <support@cloud.iojaegers.com>, Kent Madsen <kent.vejrup.madsen@outlook.com>
 Project-URL: Homepage, https://github.com/IO-Jaegers/Steel
 Project-URL: Issues, https://github.com/IO-Jaegers/Steel/issues
 Project-URL: Wiki, https://github.com/IO-Jaegers/Steel/wiki
+Project-URL: Releases, https://pypi.org/manage/project/hardened-steel/releases/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `hardened-steel-0.0.1/hardened_steel.egg-info/PKG-INFO` & `hardened-steel-0.0.2.dev0/hardened_steel.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: hardened-steel
-Version: 0.0.1
-Summary: Framework for helping to test projects with the generation of data
+Version: 0.0.2.dev0
+Summary: Framework for helping to test projects with the generation of random data during TDD
 Author-email: IO Jægers <support@cloud.iojaegers.com>, Kent Madsen <kent.vejrup.madsen@outlook.com>
 Project-URL: Homepage, https://github.com/IO-Jaegers/Steel
 Project-URL: Issues, https://github.com/IO-Jaegers/Steel/issues
 Project-URL: Wiki, https://github.com/IO-Jaegers/Steel/wiki
+Project-URL: Releases, https://pypi.org/manage/project/hardened-steel/releases/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `hardened-steel-0.0.1/pyproject.toml` & `hardened-steel-0.0.2.dev0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hardened-steel"
-version = "0.0.1"
+version = "0.0.2-dev"
 authors = [
   { name="IO Jægers", email="support@cloud.iojaegers.com" },
   { name="Kent Madsen", email="kent.vejrup.madsen@outlook.com" },
 ]
-description = "Framework for helping to test projects with the generation of data"
+description = "Framework for helping to test projects with the generation of random data during TDD"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/IO-Jaegers/Steel"
 "Issues" = "https://github.com/IO-Jaegers/Steel/issues"
 "Wiki" = "https://github.com/IO-Jaegers/Steel/wiki"
+"Releases" = "https://pypi.org/manage/project/hardened-steel/releases/"
```

