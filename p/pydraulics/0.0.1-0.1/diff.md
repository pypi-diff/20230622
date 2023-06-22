# Comparing `tmp/pydraulics-0.0.1.tar.gz` & `tmp/pydraulics-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydraulics-0.0.1.tar", last modified: Thu Jun 22 10:17:02 2023, max compression
+gzip compressed data, was "pydraulics-0.1.tar", last modified: Thu Jun 22 10:56:09 2023, max compression
```

## Comparing `pydraulics-0.0.1.tar` & `pydraulics-0.1.tar`

### file list

```diff
@@ -1,13 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 10:17:02.781892 pydraulics-0.0.1/
--rw-rw-rw-   0        0        0     1088 2023-06-21 08:15:13.000000 pydraulics-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     3417 2023-06-22 10:17:02.781892 pydraulics-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2910 2023-06-22 10:05:56.000000 pydraulics-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 10:17:02.739046 pydraulics-0.0.1/pydraulics/
-drwxrwxrwx   0        0        0        0 2023-06-22 10:17:02.780892 pydraulics-0.0.1/pydraulics/pydraulics.egg-info/
--rw-rw-rw-   0        0        0     3417 2023-06-22 10:17:02.000000 pydraulics-0.0.1/pydraulics/pydraulics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      260 2023-06-22 10:17:02.000000 pydraulics-0.0.1/pydraulics/pydraulics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 10:17:02.000000 pydraulics-0.0.1/pydraulics/pydraulics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-22 09:53:20.000000 pydraulics-0.0.1/pydraulics/pydraulics.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        1 2023-06-22 10:17:02.000000 pydraulics-0.0.1/pydraulics/pydraulics.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-22 10:17:02.784892 pydraulics-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      848 2023-06-22 10:16:42.000000 pydraulics-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 10:56:09.276732 pydraulics-0.1/
+-rw-rw-rw-   0        0        0     3392 2023-06-22 10:56:09.275731 pydraulics-0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-22 10:56:09.244768 pydraulics-0.1/pydraulics/
+drwxrwxrwx   0        0        0        0 2023-06-22 10:56:09.273736 pydraulics-0.1/pydraulics/pydraulics.egg-info/
+-rw-rw-rw-   0        0        0     3392 2023-06-22 10:56:09.000000 pydraulics-0.1/pydraulics/pydraulics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2023-06-22 10:56:09.000000 pydraulics-0.1/pydraulics/pydraulics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 10:56:09.000000 pydraulics-0.1/pydraulics/pydraulics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-22 10:50:58.000000 pydraulics-0.1/pydraulics/pydraulics.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        1 2023-06-22 10:56:09.000000 pydraulics-0.1/pydraulics/pydraulics.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-22 10:56:09.276732 pydraulics-0.1/setup.cfg
+-rw-rw-rw-   0        0        0      859 2023-06-22 10:54:50.000000 pydraulics-0.1/setup.py
```

### Comparing `pydraulics-0.0.1/PKG-INFO` & `pydraulics-0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: pydraulics
-Version: 0.0.1
+Version: 0.1
 Summary: A simple package for open and pipe flow in hydraulics created at IDOM.
 Home-page: https://github.com/JuanGuerrero09/pydraulics
 Author: Juan David Guerrero
 Author-email: juanguerrero09mc@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # pydraulics
 
 pydraulics is a Python package designed to facilitate hydraulic calculations and analysis. It provides a range of functionalities for open channel flow and pipe flow calculations.
 
 ## Features
```

### Comparing `pydraulics-0.0.1/README.md` & `pydraulics-0.1/pydraulics/pydraulics.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: pydraulics
+Version: 0.1
+Summary: A simple package for open and pipe flow in hydraulics created at IDOM.
+Home-page: https://github.com/JuanGuerrero09/pydraulics
+Author: Juan David Guerrero
+Author-email: juanguerrero09mc@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
 # pydraulics
 
 pydraulics is a Python package designed to facilitate hydraulic calculations and analysis. It provides a range of functionalities for open channel flow and pipe flow calculations.
 
 ## Features
 
 ### Open Channel Flow
@@ -56,8 +69,8 @@
 
 Contributions to pydraulics are welcome! If you have any ideas, bug fixes, or new features, feel free to open an issue or submit a pull request on GitHub.
 
 ## License
 
 pydraulics is licensed under the MIT License. See the [LICENSE](https://github.com/your-username/pydraulics/blob/main/LICENSE) file for more information.
 
-We hope pydraulics proves to be a valuable tool for your hydraulic analysis and calculations. Happy coding!
+We hope pydraulics proves to be a valuable tool for your hydraulic analysis and calculations. Happy coding!
```

### Comparing `pydraulics-0.0.1/setup.py` & `pydraulics-0.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
-with open("README.md", "r", encoding = "utf-8") as fh:
+with open("./pydraulics/README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "pydraulics",
-    version = "0.0.1",
+    version = "0.1",
     author = "Juan David Guerrero",
     author_email = "juanguerrero09mc@gmail.com",
     description = "A simple package for open and pipe flow in hydraulics created at IDOM.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/JuanGuerrero09/pydraulics",
     classifiers = [
```

