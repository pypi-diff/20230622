# Comparing `tmp/MGSurvE-0.9.1.5.tar.gz` & `tmp/MGSurvE-1.0.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MGSurvE-0.9.1.5.tar", last modified: Fri Jun  9 00:18:16 2023, max compression
+gzip compressed data, was "MGSurvE-1.0.0.0.tar", last modified: Wed Jun 21 23:42:09 2023, max compression
```

## Comparing `MGSurvE-0.9.1.5.tar` & `MGSurvE-1.0.0.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-06-09 00:18:16.372396 MGSurvE-0.9.1.5/
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    35149 2023-05-11 16:34:41.000000 MGSurvE-0.9.1.5/LICENSE
-drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-06-09 00:18:16.370935 MGSurvE-0.9.1.5/MGSurvE/
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      275 2023-05-11 16:34:41.000000 MGSurvE-0.9.1.5/MGSurvE/__init__.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       23 2023-06-09 00:18:16.000000 MGSurvE-0.9.1.5/MGSurvE/_version.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6881 2023-05-11 16:34:41.000000 MGSurvE-0.9.1.5/MGSurvE/auxiliary.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      605 2023-06-01 22:38:54.000000 MGSurvE-0.9.1.5/MGSurvE/colors.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1665 2023-05-11 16:34:41.000000 MGSurvE-0.9.1.5/MGSurvE/constants.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     7191 2023-06-08 23:51:28.000000 MGSurvE-0.9.1.5/MGSurvE/kernels.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    21376 2023-06-08 23:51:28.000000 MGSurvE-0.9.1.5/MGSurvE/landscape.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4924 2023-05-11 16:34:41.000000 MGSurvE-0.9.1.5/MGSurvE/matrices.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1358 2023-05-11 16:34:41.000000 MGSurvE-0.9.1.5/MGSurvE/network.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    45037 2023-05-11 16:34:41.000000 MGSurvE-0.9.1.5/MGSurvE/optimization.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     9200 2023-05-11 16:34:41.000000 MGSurvE-0.9.1.5/MGSurvE/optimizationPSO.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    18219 2023-06-08 23:51:28.000000 MGSurvE-0.9.1.5/MGSurvE/plots.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6849 2023-05-11 16:34:41.000000 MGSurvE-0.9.1.5/MGSurvE/pointProcess.py
-drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-06-09 00:18:16.371961 MGSurvE-0.9.1.5/MGSurvE.egg-info/
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4596 2023-06-09 00:18:16.000000 MGSurvE-0.9.1.5/MGSurvE.egg-info/PKG-INFO
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      451 2023-06-09 00:18:16.000000 MGSurvE-0.9.1.5/MGSurvE.egg-info/SOURCES.txt
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)        1 2023-06-09 00:18:16.000000 MGSurvE-0.9.1.5/MGSurvE.egg-info/dependency_links.txt
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      221 2023-06-09 00:18:16.000000 MGSurvE-0.9.1.5/MGSurvE.egg-info/requires.txt
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)        8 2023-06-09 00:18:16.000000 MGSurvE-0.9.1.5/MGSurvE.egg-info/top_level.txt
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4596 2023-06-09 00:18:16.372220 MGSurvE-0.9.1.5/PKG-INFO
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4162 2023-05-11 16:34:41.000000 MGSurvE-0.9.1.5/README.md
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       38 2023-06-09 00:18:16.372469 MGSurvE-0.9.1.5/setup.cfg
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1428 2023-06-08 23:51:28.000000 MGSurvE-0.9.1.5/setup.py
+drwxrwxr-x   0 hector    (1002) hector    (1006)        0 2023-06-21 23:42:09.408160 MGSurvE-1.0.0.0/
+-rw-rw-r--   0 hector    (1002) hector    (1006)    35149 2022-05-16 15:12:26.000000 MGSurvE-1.0.0.0/LICENSE
+drwxrwxr-x   0 hector    (1002) hector    (1006)        0 2023-06-21 23:42:09.408160 MGSurvE-1.0.0.0/MGSurvE/
+-rw-rw-r--   0 hector    (1002) hector    (1006)      275 2022-05-16 15:12:26.000000 MGSurvE-1.0.0.0/MGSurvE/__init__.py
+-rw-rw-r--   0 hector    (1002) hector    (1006)       23 2023-06-21 23:42:09.000000 MGSurvE-1.0.0.0/MGSurvE/_version.py
+-rw-rw-r--   0 hector    (1002) hector    (1006)     6881 2022-05-16 15:12:26.000000 MGSurvE-1.0.0.0/MGSurvE/auxiliary.py
+-rw-rw-r--   0 hector    (1002) hector    (1006)      605 2023-06-02 17:57:12.000000 MGSurvE-1.0.0.0/MGSurvE/colors.py
+-rw-rw-r--   0 hector    (1002) hector    (1006)     1665 2022-05-16 15:12:26.000000 MGSurvE-1.0.0.0/MGSurvE/constants.py
+-rw-rw-r--   0 hector    (1002) hector    (1006)     7191 2023-06-08 23:47:04.000000 MGSurvE-1.0.0.0/MGSurvE/kernels.py
+-rw-rw-r--   0 hector    (1002) hector    (1006)    21376 2023-06-05 16:05:28.000000 MGSurvE-1.0.0.0/MGSurvE/landscape.py
+-rw-rw-r--   0 hector    (1002) hector    (1006)     4924 2022-03-15 21:24:52.000000 MGSurvE-1.0.0.0/MGSurvE/matrices.py
+-rw-rw-r--   0 hector    (1002) hector    (1006)     1358 2022-03-15 21:24:52.000000 MGSurvE-1.0.0.0/MGSurvE/network.py
+-rw-rw-r--   0 hector    (1002) hector    (1006)    45037 2023-04-05 15:58:13.000000 MGSurvE-1.0.0.0/MGSurvE/optimization.py
+-rw-rw-r--   0 hector    (1002) hector    (1006)     9200 2022-05-16 15:12:26.000000 MGSurvE-1.0.0.0/MGSurvE/optimizationPSO.py
+-rw-rw-r--   0 hector    (1002) hector    (1006)    18219 2023-06-02 19:31:52.000000 MGSurvE-1.0.0.0/MGSurvE/plots.py
+-rw-rw-r--   0 hector    (1002) hector    (1006)     6849 2023-03-04 15:56:03.000000 MGSurvE-1.0.0.0/MGSurvE/pointProcess.py
+drwxrwxr-x   0 hector    (1002) hector    (1006)        0 2023-06-21 23:42:09.408160 MGSurvE-1.0.0.0/MGSurvE.egg-info/
+-rw-rw-r--   0 hector    (1002) hector    (1006)     4611 2023-06-21 23:42:09.000000 MGSurvE-1.0.0.0/MGSurvE.egg-info/PKG-INFO
+-rw-rw-r--   0 hector    (1002) hector    (1006)      451 2023-06-21 23:42:09.000000 MGSurvE-1.0.0.0/MGSurvE.egg-info/SOURCES.txt
+-rw-rw-r--   0 hector    (1002) hector    (1006)        1 2023-06-21 23:42:09.000000 MGSurvE-1.0.0.0/MGSurvE.egg-info/dependency_links.txt
+-rw-rw-r--   0 hector    (1002) hector    (1006)      221 2023-06-21 23:42:09.000000 MGSurvE-1.0.0.0/MGSurvE.egg-info/requires.txt
+-rw-rw-r--   0 hector    (1002) hector    (1006)        8 2023-06-21 23:42:09.000000 MGSurvE-1.0.0.0/MGSurvE.egg-info/top_level.txt
+-rw-rw-r--   0 hector    (1002) hector    (1006)     4611 2023-06-21 23:42:09.408160 MGSurvE-1.0.0.0/PKG-INFO
+-rw-rw-r--   0 hector    (1002) hector    (1006)     4177 2023-06-12 15:17:24.000000 MGSurvE-1.0.0.0/README.md
+-rw-rw-r--   0 hector    (1002) hector    (1006)       38 2023-06-21 23:42:09.408160 MGSurvE-1.0.0.0/setup.cfg
+-rw-rw-r--   0 hector    (1002) hector    (1006)     1428 2023-06-08 23:48:37.000000 MGSurvE-1.0.0.0/setup.py
```

### Comparing `MGSurvE-0.9.1.5/LICENSE` & `MGSurvE-1.0.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.9.1.5/MGSurvE/auxiliary.py` & `MGSurvE-1.0.0.0/MGSurvE/auxiliary.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.9.1.5/MGSurvE/colors.py` & `MGSurvE-1.0.0.0/MGSurvE/colors.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.9.1.5/MGSurvE/constants.py` & `MGSurvE-1.0.0.0/MGSurvE/constants.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.9.1.5/MGSurvE/kernels.py` & `MGSurvE-1.0.0.0/MGSurvE/kernels.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.9.1.5/MGSurvE/landscape.py` & `MGSurvE-1.0.0.0/MGSurvE/landscape.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.9.1.5/MGSurvE/matrices.py` & `MGSurvE-1.0.0.0/MGSurvE/matrices.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.9.1.5/MGSurvE/network.py` & `MGSurvE-1.0.0.0/MGSurvE/network.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.9.1.5/MGSurvE/optimization.py` & `MGSurvE-1.0.0.0/MGSurvE/optimization.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.9.1.5/MGSurvE/optimizationPSO.py` & `MGSurvE-1.0.0.0/MGSurvE/optimizationPSO.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.9.1.5/MGSurvE/plots.py` & `MGSurvE-1.0.0.0/MGSurvE/plots.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.9.1.5/MGSurvE/pointProcess.py` & `MGSurvE-1.0.0.0/MGSurvE/pointProcess.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.9.1.5/MGSurvE.egg-info/PKG-INFO` & `MGSurvE-1.0.0.0/MGSurvE.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MGSurvE
-Version: 0.9.1.5
+Version: 1.0.0.0
 Summary: MGSurvE
 Home-page: https://github.com/Chipdelmal/MGSurvE
 Author: Hector M. Sanchez C.
 Author-email: sanchez.hmsc@berkeley.edu
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -31,15 +31,15 @@
 
 To install the package's latest stable version run (usage of [anaconda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/download.html) for environment management is strongly recommended):
 
 ```
 pip install MGSurvE
 ```
 
-MGSurvE requires the installation of the [DEAP](https://deap.readthedocs.io/en/master/) optimization package, which should be installed automatically with our previous `pip` command. This package can also be installed with `conda install deap`, if needed; or by having a look at [DEAP's documentation](https://pypi.org/project/deap/) for additional methods. Please have a look at our [installation instructions](https://chipdelmal.github.io/MGSurvE/build/html/installation.html) for common issues with some of the dependencies. Alternatively, pre-build images from [our Dockerhub](https://hub.docker.com/repository/docker/chipdelmal/mgsurve) can be pulled and used to avoid dependencies issues. 
+MGSurvE requires the installation of the [DEAP](https://deap.readthedocs.io/en/master/) optimization package, which should be installed automatically with our previous `pip` command. This package can also be installed with `conda install -c conda-forge deap`, if needed; or by having a look at [DEAP's documentation](https://pypi.org/project/deap/) for additional methods. Please have a look at our [installation instructions](https://chipdelmal.github.io/MGSurvE/build/html/installation.html) for common issues with some of the dependencies. Alternatively, pre-build images from [our Dockerhub](https://hub.docker.com/repository/docker/chipdelmal/mgsurve) can be pulled and used to avoid dependencies issues. 
 
 
 
 <!-- Additionally, some of MGSurvE's map-plotting functions use [cartopy](https://scitools.org.uk/cartopy/). Even though the dependency's installation is not strictly required, the easiest way to install this package is with `conda install cartopy`, but in case there are errors in this process, have a look at the package's [installation instructions](https://scitools.org.uk/cartopy/docs/latest/installing.html). -->
 
 
 ![landscape](https://github.com/Chipdelmal/MGSurvE/raw/main/img/demo.jpg)
```

### Comparing `MGSurvE-0.9.1.5/PKG-INFO` & `MGSurvE-1.0.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MGSurvE
-Version: 0.9.1.5
+Version: 1.0.0.0
 Summary: MGSurvE
 Home-page: https://github.com/Chipdelmal/MGSurvE
 Author: Hector M. Sanchez C.
 Author-email: sanchez.hmsc@berkeley.edu
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -31,15 +31,15 @@
 
 To install the package's latest stable version run (usage of [anaconda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/download.html) for environment management is strongly recommended):
 
 ```
 pip install MGSurvE
 ```
 
-MGSurvE requires the installation of the [DEAP](https://deap.readthedocs.io/en/master/) optimization package, which should be installed automatically with our previous `pip` command. This package can also be installed with `conda install deap`, if needed; or by having a look at [DEAP's documentation](https://pypi.org/project/deap/) for additional methods. Please have a look at our [installation instructions](https://chipdelmal.github.io/MGSurvE/build/html/installation.html) for common issues with some of the dependencies. Alternatively, pre-build images from [our Dockerhub](https://hub.docker.com/repository/docker/chipdelmal/mgsurve) can be pulled and used to avoid dependencies issues. 
+MGSurvE requires the installation of the [DEAP](https://deap.readthedocs.io/en/master/) optimization package, which should be installed automatically with our previous `pip` command. This package can also be installed with `conda install -c conda-forge deap`, if needed; or by having a look at [DEAP's documentation](https://pypi.org/project/deap/) for additional methods. Please have a look at our [installation instructions](https://chipdelmal.github.io/MGSurvE/build/html/installation.html) for common issues with some of the dependencies. Alternatively, pre-build images from [our Dockerhub](https://hub.docker.com/repository/docker/chipdelmal/mgsurve) can be pulled and used to avoid dependencies issues. 
 
 
 
 <!-- Additionally, some of MGSurvE's map-plotting functions use [cartopy](https://scitools.org.uk/cartopy/). Even though the dependency's installation is not strictly required, the easiest way to install this package is with `conda install cartopy`, but in case there are errors in this process, have a look at the package's [installation instructions](https://scitools.org.uk/cartopy/docs/latest/installing.html). -->
 
 
 ![landscape](https://github.com/Chipdelmal/MGSurvE/raw/main/img/demo.jpg)
```

### Comparing `MGSurvE-0.9.1.5/README.md` & `MGSurvE-1.0.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 To install the package's latest stable version run (usage of [anaconda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/download.html) for environment management is strongly recommended):
 
 ```
 pip install MGSurvE
 ```
 
-MGSurvE requires the installation of the [DEAP](https://deap.readthedocs.io/en/master/) optimization package, which should be installed automatically with our previous `pip` command. This package can also be installed with `conda install deap`, if needed; or by having a look at [DEAP's documentation](https://pypi.org/project/deap/) for additional methods. Please have a look at our [installation instructions](https://chipdelmal.github.io/MGSurvE/build/html/installation.html) for common issues with some of the dependencies. Alternatively, pre-build images from [our Dockerhub](https://hub.docker.com/repository/docker/chipdelmal/mgsurve) can be pulled and used to avoid dependencies issues. 
+MGSurvE requires the installation of the [DEAP](https://deap.readthedocs.io/en/master/) optimization package, which should be installed automatically with our previous `pip` command. This package can also be installed with `conda install -c conda-forge deap`, if needed; or by having a look at [DEAP's documentation](https://pypi.org/project/deap/) for additional methods. Please have a look at our [installation instructions](https://chipdelmal.github.io/MGSurvE/build/html/installation.html) for common issues with some of the dependencies. Alternatively, pre-build images from [our Dockerhub](https://hub.docker.com/repository/docker/chipdelmal/mgsurve) can be pulled and used to avoid dependencies issues. 
 
 
 
 <!-- Additionally, some of MGSurvE's map-plotting functions use [cartopy](https://scitools.org.uk/cartopy/). Even though the dependency's installation is not strictly required, the easiest way to install this package is with `conda install cartopy`, but in case there are errors in this process, have a look at the package's [installation instructions](https://scitools.org.uk/cartopy/docs/latest/installing.html). -->
 
 
 ![landscape](https://github.com/Chipdelmal/MGSurvE/raw/main/img/demo.jpg)
```

### Comparing `MGSurvE-0.9.1.5/setup.py` & `MGSurvE-1.0.0.0/setup.py`

 * *Files identical despite different names*

