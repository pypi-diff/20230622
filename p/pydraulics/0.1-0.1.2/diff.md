# Comparing `tmp/pydraulics-0.1.tar.gz` & `tmp/pydraulics-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydraulics-0.1.tar", last modified: Thu Jun 22 10:56:09 2023, max compression
+gzip compressed data, was "pydraulics-0.1.2.tar", last modified: Thu Jun 22 11:04:26 2023, max compression
```

## Comparing `pydraulics-0.1.tar` & `pydraulics-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 10:56:09.276732 pydraulics-0.1/
--rw-rw-rw-   0        0        0     3392 2023-06-22 10:56:09.275731 pydraulics-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-22 10:56:09.244768 pydraulics-0.1/pydraulics/
-drwxrwxrwx   0        0        0        0 2023-06-22 10:56:09.273736 pydraulics-0.1/pydraulics/pydraulics.egg-info/
--rw-rw-rw-   0        0        0     3392 2023-06-22 10:56:09.000000 pydraulics-0.1/pydraulics/pydraulics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2023-06-22 10:56:09.000000 pydraulics-0.1/pydraulics/pydraulics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 10:56:09.000000 pydraulics-0.1/pydraulics/pydraulics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-22 10:50:58.000000 pydraulics-0.1/pydraulics/pydraulics.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        1 2023-06-22 10:56:09.000000 pydraulics-0.1/pydraulics/pydraulics.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-22 10:56:09.276732 pydraulics-0.1/setup.cfg
--rw-rw-rw-   0        0        0      859 2023-06-22 10:54:50.000000 pydraulics-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 11:04:26.607571 pydraulics-0.1.2/
+-rw-rw-rw-   0        0        0      480 2023-06-22 11:04:26.606632 pydraulics-0.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-22 11:04:26.576836 pydraulics-0.1.2/pydraulics/
+drwxrwxrwx   0        0        0        0 2023-06-22 11:04:26.604620 pydraulics-0.1.2/pydraulics/pydraulics.egg-info/
+-rw-rw-rw-   0        0        0      480 2023-06-22 11:04:26.000000 pydraulics-0.1.2/pydraulics/pydraulics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2023-06-22 11:04:26.000000 pydraulics-0.1.2/pydraulics/pydraulics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 11:04:26.000000 pydraulics-0.1.2/pydraulics/pydraulics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-22 10:50:58.000000 pydraulics-0.1.2/pydraulics/pydraulics.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        1 2023-06-22 11:04:26.000000 pydraulics-0.1.2/pydraulics/pydraulics.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-22 11:04:26.608651 pydraulics-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      867 2023-06-22 11:04:23.000000 pydraulics-0.1.2/setup.py
```

### Comparing `pydraulics-0.1/setup.py` & `pydraulics-0.1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import setuptools
 
-with open("./pydraulics/README.md", "r", encoding = "utf-8") as fh:
-    long_description = fh.read()
+# with open("./pydraulics/README.md", "r", encoding = "utf-8") as fh:
+#     long_description = fh.read()
 
 setuptools.setup(
     name = "pydraulics",
-    version = "0.1",
+    version = "0.1.2",
     author = "Juan David Guerrero",
     author_email = "juanguerrero09mc@gmail.com",
     description = "A simple package for open and pipe flow in hydraulics created at IDOM.",
-    long_description = long_description,
+    # long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/JuanGuerrero09/pydraulics",
     classifiers = [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

