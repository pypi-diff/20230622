# Comparing `tmp/dissect.contrib-1.4.dev1.tar.gz` & `tmp/dissect.contrib-1.4.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.contrib-1.4.dev1.tar", last modified: Fri Jun 16 12:48:49 2023, max compression
+gzip compressed data, was "dissect.contrib-1.4.dev2.tar", last modified: Thu Jun 22 14:33:33 2023, max compression
```

## Comparing `dissect.contrib-1.4.dev1.tar` & `dissect.contrib-1.4.dev2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:48:49.296563 dissect.contrib-1.4.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-16 12:48:35.000000 dissect.contrib-1.4.dev1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-16 12:48:35.000000 dissect.contrib-1.4.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-16 12:48:35.000000 dissect.contrib-1.4.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-06-16 12:48:49.296563 dissect.contrib-1.4.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-16 12:48:35.000000 dissect.contrib-1.4.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:48:49.292563 dissect.contrib-1.4.dev1/dissect.contrib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-06-16 12:48:49.000000 dissect.contrib-1.4.dev1/dissect.contrib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-16 12:48:49.000000 dissect.contrib-1.4.dev1/dissect.contrib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 12:48:49.000000 dissect.contrib-1.4.dev1/dissect.contrib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 12:48:49.000000 dissect.contrib-1.4.dev1/dissect.contrib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-16 12:48:39.000000 dissect.contrib-1.4.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 12:48:49.296563 dissect.contrib-1.4.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:48:49.292563 dissect.contrib-1.4.dev1/template/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-16 12:48:35.000000 dissect.contrib-1.4.dev1/template/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-16 12:48:35.000000 dissect.contrib-1.4.dev1/template/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:48:49.288563 dissect.contrib-1.4.dev1/template/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:48:49.288563 dissect.contrib-1.4.dev1/template/dissect/contrib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:48:49.296563 dissect.contrib-1.4.dev1/template/dissect/contrib/template/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 12:48:35.000000 dissect.contrib-1.4.dev1/template/dissect/contrib/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-16 12:48:35.000000 dissect.contrib-1.4.dev1/template/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-16 12:48:35.000000 dissect.contrib-1.4.dev1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:33:33.076774 dissect.contrib-1.4.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-22 14:33:16.000000 dissect.contrib-1.4.dev2/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-22 14:33:16.000000 dissect.contrib-1.4.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-22 14:33:16.000000 dissect.contrib-1.4.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-06-22 14:33:33.076774 dissect.contrib-1.4.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-22 14:33:16.000000 dissect.contrib-1.4.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:33:33.072774 dissect.contrib-1.4.dev2/dissect.contrib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-06-22 14:33:33.000000 dissect.contrib-1.4.dev2/dissect.contrib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-22 14:33:33.000000 dissect.contrib-1.4.dev2/dissect.contrib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 14:33:33.000000 dissect.contrib-1.4.dev2/dissect.contrib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 14:33:33.000000 dissect.contrib-1.4.dev2/dissect.contrib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-22 14:33:21.000000 dissect.contrib-1.4.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 14:33:33.076774 dissect.contrib-1.4.dev2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:33:33.072774 dissect.contrib-1.4.dev2/template/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-22 14:33:16.000000 dissect.contrib-1.4.dev2/template/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-22 14:33:16.000000 dissect.contrib-1.4.dev2/template/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:33:33.068773 dissect.contrib-1.4.dev2/template/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:33:33.068773 dissect.contrib-1.4.dev2/template/dissect/contrib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:33:33.076774 dissect.contrib-1.4.dev2/template/dissect/contrib/template/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-22 14:33:16.000000 dissect.contrib-1.4.dev2/template/dissect/contrib/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-22 14:33:16.000000 dissect.contrib-1.4.dev2/template/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-22 14:33:16.000000 dissect.contrib-1.4.dev2/tox.ini
```

### Comparing `dissect.contrib-1.4.dev1/LICENSE` & `dissect.contrib-1.4.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.contrib-1.4.dev1/PKG-INFO` & `dissect.contrib-1.4.dev2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.contrib
-Version: 1.4.dev1
+Version: 1.4.dev2
 Summary: This project is a meta package: it reserves the namespace for Dissect packages made by external contributors
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: repository, https://github.com/fox-it/dissect.contrib
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `dissect.contrib-1.4.dev1/README.md` & `dissect.contrib-1.4.dev2/README.md`

 * *Files identical despite different names*

### Comparing `dissect.contrib-1.4.dev1/dissect.contrib.egg-info/PKG-INFO` & `dissect.contrib-1.4.dev2/dissect.contrib.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.contrib
-Version: 1.4.dev1
+Version: 1.4.dev2
 Summary: This project is a meta package: it reserves the namespace for Dissect packages made by external contributors
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: repository, https://github.com/fox-it/dissect.contrib
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `dissect.contrib-1.4.dev1/pyproject.toml` & `dissect.contrib-1.4.dev2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.contrib-1.4.dev1/template/pyproject.toml` & `dissect.contrib-1.4.dev2/template/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 dynamic = ["version"]
 
 [project.urls]
 # Replace with the actual websites you use as homepage, documentation site and
 # repository, or remove if not used
 homepage = "https://homepage.for.your.project.example.com"
 documentation = "https://docs.for.your.project.example.com/"
-repository = "https://github.com/username/dissect.contrib.template
+repository = "https://github.com/username/dissect.contrib.template"
 
 [tool.black]
 line-length = 120
 
 [tool.isort]
 profile = "black"
 # Replace 'template' with the actual name of your project
```

### Comparing `dissect.contrib-1.4.dev1/tox.ini` & `dissect.contrib-1.4.dev2/tox.ini`

 * *Files identical despite different names*

