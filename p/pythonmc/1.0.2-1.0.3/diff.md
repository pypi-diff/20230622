# Comparing `tmp/pythonmc-1.0.2.tar.gz` & `tmp/pythonmc-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonmc-1.0.2.tar", last modified: Tue Jun 20 01:31:13 2023, max compression
+gzip compressed data, was "pythonmc-1.0.3.tar", last modified: Thu Jun 22 20:18:50 2023, max compression
```

## Comparing `pythonmc-1.0.2.tar` & `pythonmc-1.0.3.tar`

### file list

```diff
@@ -1,11 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 01:31:13.642351 pythonmc-1.0.2/
--rw-rw-rw-   0        0        0     4674 2023-06-20 01:31:13.642351 pythonmc-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4161 2023-06-19 22:16:33.000000 pythonmc-1.0.2/README.md
--rw-rw-rw-   0        0        0      108 2023-06-20 00:42:26.000000 pythonmc-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      675 2023-06-20 01:31:13.643351 pythonmc-1.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-20 01:31:13.634533 pythonmc-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-20 01:31:13.641347 pythonmc-1.0.2/src/pythonmc.egg-info/
--rw-rw-rw-   0        0        0     4674 2023-06-20 01:31:13.000000 pythonmc-1.0.2/src/pythonmc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-06-20 01:31:13.000000 pythonmc-1.0.2/src/pythonmc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 01:31:13.000000 pythonmc-1.0.2/src/pythonmc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 01:31:13.000000 pythonmc-1.0.2/src/pythonmc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-22 20:18:50.620172 pythonmc-1.0.3/
+-rw-rw-rw-   0        0        0     4694 2023-06-22 20:18:50.620172 pythonmc-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4181 2023-06-22 18:13:59.000000 pythonmc-1.0.3/README.md
+-rw-rw-rw-   0        0        0      108 2023-06-22 18:13:59.000000 pythonmc-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      675 2023-06-22 20:18:50.621168 pythonmc-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-22 20:18:50.614107 pythonmc-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-06-22 20:18:50.616167 pythonmc-1.0.3/src/pythonmc/
+-rw-rw-rw-   0        0        0   155553 2023-06-22 19:37:55.000000 pythonmc-1.0.3/src/pythonmc/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 20:18:50.619167 pythonmc-1.0.3/src/pythonmc.egg-info/
+-rw-rw-rw-   0        0        0     4694 2023-06-22 20:18:50.000000 pythonmc-1.0.3/src/pythonmc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2023-06-22 20:18:50.000000 pythonmc-1.0.3/src/pythonmc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 20:18:50.000000 pythonmc-1.0.3/src/pythonmc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-22 20:18:50.000000 pythonmc-1.0.3/src/pythonmc.egg-info/top_level.txt
```

### Comparing `pythonmc-1.0.2/PKG-INFO` & `pythonmc-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythonmc
-Version: 1.0.2
+Version: 1.0.3
 Summary: The python library for PythonMC
 Home-page: https://github.com/RevolvingMadness/PythonMC
 Author: RevolvingMadness
 Author-email: revolvingmad@gmail.com
 Project-URL: Bug Tracker, https://github.com/RevolvingMadness/PythonMC/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -23,15 +23,15 @@
 
 <!--suppress ALL -->
 
 <br />
 <div align="center">
   <a href="https://github.com/RevolvingMadness/PythonMC">
     <!--suppress CheckImageSize, CheckImageSize -->
-<img src="images/logo.png" alt="PythonMC Logo" width="80" height="80">
+<img src="https://raw.githubusercontent.com/RevolvingMadness/PythonMC/master/images/logo.png" alt="PythonMC Logo" width="80" height="80">
   </a>
 
 <h3 align="center">PythonMC</h3>
 
   <p align="center">
     PythonMC is a Fabric mod that allows datapacks to be written in Python. Minecraft datapacks have some big limitations but, PythonMC has very little. Like for loops, functions, if statements, and modules. 
     <br />
@@ -118,12 +118,10 @@
 
 [license-url]: https://github.com/RevolvingMadness/PythonMC/blob/master/LICENSE.txt
 
 [linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
 
 [linkedin-url]: https://linkedin.com/in/linkedin_username
 
-[product-screenshot]: images/screenshot.png
-
 [fabricmc.net]: https://img.shields.io/badge/Fabric%20-1.19.4%20-blue?style=for-the-badge
 
 [Fabric-url]: https://fabricmc.net
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pythonmc Version: 1.0.2 Summary: The python library
+Metadata-Version: 2.1 Name: pythonmc Version: 1.0.3 Summary: The python library
 for PythonMC Home-page: https://github.com/RevolvingMadness/PythonMC Author:
 RevolvingMadness Author-email: revolvingmad@gmail.com Project-URL: Bug Tracker,
 https://github.com/RevolvingMadness/PythonMC/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.9
 Description-Content-Type: text/markdown  [![Contributors][contributors-shield]]
 [contributors-url] [![Forks][forks-shield]][forks-url] [![Stargazers][stars-
@@ -50,10 +50,9 @@
 RevolvingMadness/PythonMC/stargazers [issues-shield]: https://img.shields.io/
 github/issues/RevolvingMadness/PythonMC.svg?style=for-the-badge [issues-url]:
 https://github.com/RevolvingMadness/PythonMC/issues [license-shield]: https://
 img.shields.io/github/license/RevolvingMadness/PythonMC.svg?style=for-the-badge
 [license-url]: https://github.com/RevolvingMadness/PythonMC/blob/master/
 LICENSE.txt [linkedin-shield]: https://img.shields.io/badge/-LinkedIn-
 black.svg?style=for-the-badge&logo=linkedin&colorB=555 [linkedin-url]: https://
-linkedin.com/in/linkedin_username [product-screenshot]: images/screenshot.png
-[fabricmc.net]: https://img.shields.io/badge/Fabric%20-1.19.4%20-
-blue?style=for-the-badge [Fabric-url]: https://fabricmc.net
+linkedin.com/in/linkedin_username [fabricmc.net]: https://img.shields.io/badge/
+Fabric%20-1.19.4%20-blue?style=for-the-badge [Fabric-url]: https://fabricmc.net
```

### Comparing `pythonmc-1.0.2/README.md` & `pythonmc-1.0.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 <!--suppress ALL -->
 
 <br />
 <div align="center">
   <a href="https://github.com/RevolvingMadness/PythonMC">
     <!--suppress CheckImageSize, CheckImageSize -->
-<img src="images/logo.png" alt="PythonMC Logo" width="80" height="80">
+<img src="https://raw.githubusercontent.com/RevolvingMadness/PythonMC/master/images/logo.png" alt="PythonMC Logo" width="80" height="80">
   </a>
 
 <h3 align="center">PythonMC</h3>
 
   <p align="center">
     PythonMC is a Fabric mod that allows datapacks to be written in Python. Minecraft datapacks have some big limitations but, PythonMC has very little. Like for loops, functions, if statements, and modules. 
     <br />
@@ -104,12 +104,10 @@
 
 [license-url]: https://github.com/RevolvingMadness/PythonMC/blob/master/LICENSE.txt
 
 [linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
 
 [linkedin-url]: https://linkedin.com/in/linkedin_username
 
-[product-screenshot]: images/screenshot.png
-
 [fabricmc.net]: https://img.shields.io/badge/Fabric%20-1.19.4%20-blue?style=for-the-badge
 
 [Fabric-url]: https://fabricmc.net
```

#### html2text {}

```diff
@@ -43,10 +43,9 @@
 RevolvingMadness/PythonMC/stargazers [issues-shield]: https://img.shields.io/
 github/issues/RevolvingMadness/PythonMC.svg?style=for-the-badge [issues-url]:
 https://github.com/RevolvingMadness/PythonMC/issues [license-shield]: https://
 img.shields.io/github/license/RevolvingMadness/PythonMC.svg?style=for-the-badge
 [license-url]: https://github.com/RevolvingMadness/PythonMC/blob/master/
 LICENSE.txt [linkedin-shield]: https://img.shields.io/badge/-LinkedIn-
 black.svg?style=for-the-badge&logo=linkedin&colorB=555 [linkedin-url]: https://
-linkedin.com/in/linkedin_username [product-screenshot]: images/screenshot.png
-[fabricmc.net]: https://img.shields.io/badge/Fabric%20-1.19.4%20-
-blue?style=for-the-badge [Fabric-url]: https://fabricmc.net
+linkedin.com/in/linkedin_username [fabricmc.net]: https://img.shields.io/badge/
+Fabric%20-1.19.4%20-blue?style=for-the-badge [Fabric-url]: https://fabricmc.net
```

### Comparing `pythonmc-1.0.2/setup.cfg` & `pythonmc-1.0.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7974 686f 6e6d 630d 0a76 6572   = pythonmc..ver
-00000020: 7369 6f6e 203d 2031 2e30 2e32 0d0a 6175  sion = 1.0.2..au
+00000020: 7369 6f6e 203d 2031 2e30 2e33 0d0a 6175  sion = 1.0.3..au
 00000030: 7468 6f72 203d 2052 6576 6f6c 7669 6e67  thor = Revolving
 00000040: 4d61 646e 6573 730d 0a61 7574 686f 725f  Madness..author_
 00000050: 656d 6169 6c20 3d20 7265 766f 6c76 696e  email = revolvin
 00000060: 676d 6164 4067 6d61 696c 2e63 6f6d 0d0a  gmad@gmail.com..
 00000070: 6465 7363 7269 7074 696f 6e20 3d20 5468  description = Th
 00000080: 6520 7079 7468 6f6e 206c 6962 7261 7279  e python library
 00000090: 2066 6f72 2050 7974 686f 6e4d 430d 0a6c   for PythonMC..l
```

### Comparing `pythonmc-1.0.2/src/pythonmc.egg-info/PKG-INFO` & `pythonmc-1.0.3/src/pythonmc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythonmc
-Version: 1.0.2
+Version: 1.0.3
 Summary: The python library for PythonMC
 Home-page: https://github.com/RevolvingMadness/PythonMC
 Author: RevolvingMadness
 Author-email: revolvingmad@gmail.com
 Project-URL: Bug Tracker, https://github.com/RevolvingMadness/PythonMC/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -23,15 +23,15 @@
 
 <!--suppress ALL -->
 
 <br />
 <div align="center">
   <a href="https://github.com/RevolvingMadness/PythonMC">
     <!--suppress CheckImageSize, CheckImageSize -->
-<img src="images/logo.png" alt="PythonMC Logo" width="80" height="80">
+<img src="https://raw.githubusercontent.com/RevolvingMadness/PythonMC/master/images/logo.png" alt="PythonMC Logo" width="80" height="80">
   </a>
 
 <h3 align="center">PythonMC</h3>
 
   <p align="center">
     PythonMC is a Fabric mod that allows datapacks to be written in Python. Minecraft datapacks have some big limitations but, PythonMC has very little. Like for loops, functions, if statements, and modules. 
     <br />
@@ -118,12 +118,10 @@
 
 [license-url]: https://github.com/RevolvingMadness/PythonMC/blob/master/LICENSE.txt
 
 [linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
 
 [linkedin-url]: https://linkedin.com/in/linkedin_username
 
-[product-screenshot]: images/screenshot.png
-
 [fabricmc.net]: https://img.shields.io/badge/Fabric%20-1.19.4%20-blue?style=for-the-badge
 
 [Fabric-url]: https://fabricmc.net
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pythonmc Version: 1.0.2 Summary: The python library
+Metadata-Version: 2.1 Name: pythonmc Version: 1.0.3 Summary: The python library
 for PythonMC Home-page: https://github.com/RevolvingMadness/PythonMC Author:
 RevolvingMadness Author-email: revolvingmad@gmail.com Project-URL: Bug Tracker,
 https://github.com/RevolvingMadness/PythonMC/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.9
 Description-Content-Type: text/markdown  [![Contributors][contributors-shield]]
 [contributors-url] [![Forks][forks-shield]][forks-url] [![Stargazers][stars-
@@ -50,10 +50,9 @@
 RevolvingMadness/PythonMC/stargazers [issues-shield]: https://img.shields.io/
 github/issues/RevolvingMadness/PythonMC.svg?style=for-the-badge [issues-url]:
 https://github.com/RevolvingMadness/PythonMC/issues [license-shield]: https://
 img.shields.io/github/license/RevolvingMadness/PythonMC.svg?style=for-the-badge
 [license-url]: https://github.com/RevolvingMadness/PythonMC/blob/master/
 LICENSE.txt [linkedin-shield]: https://img.shields.io/badge/-LinkedIn-
 black.svg?style=for-the-badge&logo=linkedin&colorB=555 [linkedin-url]: https://
-linkedin.com/in/linkedin_username [product-screenshot]: images/screenshot.png
-[fabricmc.net]: https://img.shields.io/badge/Fabric%20-1.19.4%20-
-blue?style=for-the-badge [Fabric-url]: https://fabricmc.net
+linkedin.com/in/linkedin_username [fabricmc.net]: https://img.shields.io/badge/
+Fabric%20-1.19.4%20-blue?style=for-the-badge [Fabric-url]: https://fabricmc.net
```

