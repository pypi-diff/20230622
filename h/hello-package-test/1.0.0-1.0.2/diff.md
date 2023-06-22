# Comparing `tmp/hello-package-test-1.0.0.tar.gz` & `tmp/hello-package-test-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hello-package-test-1.0.0.tar", last modified: Thu Jun 22 12:28:57 2023, max compression
+gzip compressed data, was "hello-package-test-1.0.2.tar", last modified: Thu Jun 22 12:44:59 2023, max compression
```

## Comparing `hello-package-test-1.0.0.tar` & `hello-package-test-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 tunji      (501) staff       (20)        0 2023-06-22 12:28:57.018920 hello-package-test-1.0.0/
--rw-r--r--   0 tunji      (501) staff       (20)      485 2023-06-22 12:28:57.019042 hello-package-test-1.0.0/PKG-INFO
--rw-r--r--   0 tunji      (501) staff       (20)       29 2023-06-22 09:27:57.000000 hello-package-test-1.0.0/README.md
--rw-r--r--   0 tunji      (501) staff       (20)      104 2023-06-22 09:28:11.000000 hello-package-test-1.0.0/pyproject.toml
--rw-r--r--   0 tunji      (501) staff       (20)      603 2023-06-22 12:28:57.019565 hello-package-test-1.0.0/setup.cfg
-drwxr-xr-x   0 tunji      (501) staff       (20)        0 2023-06-22 12:28:57.014948 hello-package-test-1.0.0/src/
-drwxr-xr-x   0 tunji      (501) staff       (20)        0 2023-06-22 12:28:57.015940 hello-package-test-1.0.0/src/hello_package_test/
--rw-r--r--   0 tunji      (501) staff       (20)       55 2023-06-22 11:46:42.000000 hello-package-test-1.0.0/src/hello_package_test/__init__.py
-drwxr-xr-x   0 tunji      (501) staff       (20)        0 2023-06-22 12:28:57.018479 hello-package-test-1.0.0/src/hello_package_test.egg-info/
--rw-r--r--   0 tunji      (501) staff       (20)      485 2023-06-22 12:28:57.000000 hello-package-test-1.0.0/src/hello_package_test.egg-info/PKG-INFO
--rw-r--r--   0 tunji      (501) staff       (20)      253 2023-06-22 12:28:57.000000 hello-package-test-1.0.0/src/hello_package_test.egg-info/SOURCES.txt
--rw-r--r--   0 tunji      (501) staff       (20)        1 2023-06-22 12:28:57.000000 hello-package-test-1.0.0/src/hello_package_test.egg-info/dependency_links.txt
--rw-r--r--   0 tunji      (501) staff       (20)       19 2023-06-22 12:28:57.000000 hello-package-test-1.0.0/src/hello_package_test.egg-info/top_level.txt
+drwxr-xr-x   0 tunji      (501) staff       (20)        0 2023-06-22 12:44:59.854799 hello-package-test-1.0.2/
+-rw-r--r--   0 tunji      (501) staff       (20)      485 2023-06-22 12:44:59.854919 hello-package-test-1.0.2/PKG-INFO
+-rw-r--r--   0 tunji      (501) staff       (20)       29 2023-06-22 09:27:57.000000 hello-package-test-1.0.2/README.md
+-rw-r--r--   0 tunji      (501) staff       (20)      104 2023-06-22 09:28:11.000000 hello-package-test-1.0.2/pyproject.toml
+-rw-r--r--   0 tunji      (501) staff       (20)      603 2023-06-22 12:44:59.855414 hello-package-test-1.0.2/setup.cfg
+drwxr-xr-x   0 tunji      (501) staff       (20)        0 2023-06-22 12:44:59.851264 hello-package-test-1.0.2/src/
+drwxr-xr-x   0 tunji      (501) staff       (20)        0 2023-06-22 12:44:59.852406 hello-package-test-1.0.2/src/hello_package_test/
+-rw-r--r--   0 tunji      (501) staff       (20)       70 2023-06-22 12:39:09.000000 hello-package-test-1.0.2/src/hello_package_test/__init__.py
+drwxr-xr-x   0 tunji      (501) staff       (20)        0 2023-06-22 12:44:59.854482 hello-package-test-1.0.2/src/hello_package_test.egg-info/
+-rw-r--r--   0 tunji      (501) staff       (20)      485 2023-06-22 12:44:59.000000 hello-package-test-1.0.2/src/hello_package_test.egg-info/PKG-INFO
+-rw-r--r--   0 tunji      (501) staff       (20)      253 2023-06-22 12:44:59.000000 hello-package-test-1.0.2/src/hello_package_test.egg-info/SOURCES.txt
+-rw-r--r--   0 tunji      (501) staff       (20)        1 2023-06-22 12:44:59.000000 hello-package-test-1.0.2/src/hello_package_test.egg-info/dependency_links.txt
+-rw-r--r--   0 tunji      (501) staff       (20)       19 2023-06-22 12:44:59.000000 hello-package-test-1.0.2/src/hello_package_test.egg-info/top_level.txt
```

### Comparing `hello-package-test-1.0.0/setup.cfg` & `hello-package-test-1.0.2/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hello-package-test
-version = 1.0.0
+version = 1.0.2
 author = Oyetunji Abioye
 author_email = oabioye@riskprotocol.io
 description = SDK for the Risk Simulator
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://riskprotocol.io
 project_urls =
```

