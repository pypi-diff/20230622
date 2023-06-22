# Comparing `tmp/reticuler-1.0.tar.gz` & `tmp/reticuler-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reticuler-1.0.tar", last modified: Sun Apr 30 21:33:50 2023, max compression
+gzip compressed data, was "reticuler-1.1.tar", last modified: Thu Jun 22 12:11:00 2023, max compression
```

## Comparing `reticuler-1.0.tar` & `reticuler-1.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 21:33:50.827000 reticuler-1.0/
--rw-rw-rw-   0        0        0     1097 2022-11-09 13:08:57.000000 reticuler-1.0/LICENSE
--rw-rw-rw-   0        0        0     2396 2023-04-30 21:33:50.763000 reticuler-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1909 2022-11-28 08:05:01.000000 reticuler-1.0/README.md
--rw-rw-rw-   0        0        0     1112 2023-04-28 10:05:25.000000 reticuler-1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-30 21:33:50.802000 reticuler-1.0/setup.cfg
--rw-rw-rw-   0        0        0       91 2022-11-02 22:21:50.000000 reticuler-1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-30 21:33:48.399000 reticuler-1.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-30 21:33:49.036000 reticuler-1.0/src/reticuler/
--rw-rw-rw-   0        0        0      100 2023-04-28 10:12:46.000000 reticuler-1.0/src/reticuler/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-30 21:33:49.723000 reticuler-1.0/src/reticuler/backward_evolution/
--rw-rw-rw-   0        0        0       53 2023-04-28 10:06:15.000000 reticuler-1.0/src/reticuler/backward_evolution/__init__.py
--rw-rw-rw-   0        0        0    15255 2023-04-30 20:39:35.000000 reticuler-1.0/src/reticuler/backward_evolution/system_back.py
--rw-rw-rw-   0        0        0    13312 2023-04-30 20:39:49.000000 reticuler-1.0/src/reticuler/backward_evolution/trimmers.py
-drwxrwxrwx   0        0        0        0 2023-04-30 21:33:50.040000 reticuler-1.0/src/reticuler/extending_kernels/
--rw-rw-rw-   0        0        0       93 2022-11-23 12:02:56.000000 reticuler-1.0/src/reticuler/extending_kernels/__init__.py
--rw-rw-rw-   0        0        0     8831 2023-04-27 13:36:32.000000 reticuler-1.0/src/reticuler/extending_kernels/extenders.py
--rw-rw-rw-   0        0        0    16736 2023-04-27 13:33:53.000000 reticuler-1.0/src/reticuler/extending_kernels/pde_solvers.py
--rw-rw-rw-   0        0        0     4906 2023-04-27 14:20:25.000000 reticuler-1.0/src/reticuler/extending_kernels/trajectory_integrators.py
--rw-rw-rw-   0        0        0    26823 2023-04-28 16:01:04.000000 reticuler-1.0/src/reticuler/system.py
-drwxrwxrwx   0        0        0        0 2023-04-30 21:33:50.714000 reticuler-1.0/src/reticuler/user_interface/
--rw-rw-rw-   0        0        0       48 2023-04-28 09:54:46.000000 reticuler-1.0/src/reticuler/user_interface/__init__.py
--rw-rw-rw-   0        0        0     3070 2023-04-28 12:37:49.000000 reticuler-1.0/src/reticuler/user_interface/clip_ret.py
--rw-rw-rw-   0        0        0     2815 2023-04-28 09:44:01.000000 reticuler-1.0/src/reticuler/user_interface/clippers.py
--rw-rw-rw-   0        0        0     2313 2023-04-28 12:40:36.000000 reticuler-1.0/src/reticuler/user_interface/graphics.py
--rw-rw-rw-   0        0        0     3574 2023-04-28 13:16:15.000000 reticuler-1.0/src/reticuler/user_interface/plot_ret.py
--rw-rw-rw-   0        0        0     7618 2022-12-20 11:49:09.000000 reticuler-1.0/src/reticuler/user_interface/reticulate.py
--rw-rw-rw-   0        0        0     3755 2023-04-30 20:39:06.000000 reticuler-1.0/src/reticuler/user_interface/reticulate_back.py
-drwxrwxrwx   0        0        0        0 2023-04-30 21:33:49.479000 reticuler-1.0/src/reticuler.egg-info/
--rw-rw-rw-   0        0        0     2396 2023-04-30 21:33:47.000000 reticuler-1.0/src/reticuler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      943 2023-04-30 21:33:48.000000 reticuler-1.0/src/reticuler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 21:33:47.000000 reticuler-1.0/src/reticuler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      236 2023-04-30 21:33:48.000000 reticuler-1.0/src/reticuler.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       28 2023-04-30 21:33:48.000000 reticuler-1.0/src/reticuler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-30 21:33:48.000000 reticuler-1.0/src/reticuler.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-22 12:11:00.457000 reticuler-1.1/
+-rw-rw-rw-   0        0        0     1097 2022-11-09 13:08:57.000000 reticuler-1.1/LICENSE
+-rw-rw-rw-   0        0        0     2368 2023-06-22 12:11:00.402000 reticuler-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1883 2023-06-22 12:07:52.000000 reticuler-1.1/README.md
+-rw-rw-rw-   0        0        0     1112 2023-06-22 12:01:21.000000 reticuler-1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-22 12:11:00.438000 reticuler-1.1/setup.cfg
+-rw-rw-rw-   0        0        0       91 2022-11-02 22:21:50.000000 reticuler-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:10:58.601000 reticuler-1.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-22 12:10:58.916000 reticuler-1.1/src/reticuler/
+-rw-rw-rw-   0        0        0      100 2023-06-16 08:54:04.000000 reticuler-1.1/src/reticuler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:10:59.571000 reticuler-1.1/src/reticuler/backward_evolution/
+-rw-rw-rw-   0        0        0       53 2023-06-16 08:54:04.000000 reticuler-1.1/src/reticuler/backward_evolution/__init__.py
+-rw-rw-rw-   0        0        0    19689 2023-06-22 11:27:48.000000 reticuler-1.1/src/reticuler/backward_evolution/system_back.py
+-rw-rw-rw-   0        0        0    14065 2023-06-22 11:26:56.000000 reticuler-1.1/src/reticuler/backward_evolution/trimmers.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:10:59.864000 reticuler-1.1/src/reticuler/extending_kernels/
+-rw-rw-rw-   0        0        0       93 2022-11-23 12:02:56.000000 reticuler-1.1/src/reticuler/extending_kernels/__init__.py
+-rw-rw-rw-   0        0        0     8866 2023-06-16 08:54:04.000000 reticuler-1.1/src/reticuler/extending_kernels/extenders.py
+-rw-rw-rw-   0        0        0    17017 2023-06-22 11:23:41.000000 reticuler-1.1/src/reticuler/extending_kernels/pde_solvers.py
+-rw-rw-rw-   0        0        0     4980 2023-06-20 18:02:51.000000 reticuler-1.1/src/reticuler/extending_kernels/trajectory_integrators.py
+-rw-rw-rw-   0        0        0    26659 2023-06-16 08:54:05.000000 reticuler-1.1/src/reticuler/system.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:11:00.331000 reticuler-1.1/src/reticuler/user_interface/
+-rw-rw-rw-   0        0        0       50 2023-06-16 08:54:05.000000 reticuler-1.1/src/reticuler/user_interface/__init__.py
+-rw-rw-rw-   0        0        0     4573 2023-06-20 15:51:45.000000 reticuler-1.1/src/reticuler/user_interface/clip_ret.py
+-rw-rw-rw-   0        0        0     8719 2023-06-20 20:06:37.000000 reticuler-1.1/src/reticuler/user_interface/clippers.py
+-rw-rw-rw-   0        0        0     2313 2023-06-16 08:54:05.000000 reticuler-1.1/src/reticuler/user_interface/graphics.py
+-rw-rw-rw-   0        0        0     3574 2023-06-16 08:54:05.000000 reticuler-1.1/src/reticuler/user_interface/plot_ret.py
+-rw-rw-rw-   0        0        0     7726 2023-06-16 08:54:05.000000 reticuler-1.1/src/reticuler/user_interface/reticulate.py
+-rw-rw-rw-   0        0        0     4633 2023-06-21 10:39:10.000000 reticuler-1.1/src/reticuler/user_interface/reticulate_back.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:10:59.325000 reticuler-1.1/src/reticuler.egg-info/
+-rw-rw-rw-   0        0        0     2368 2023-06-22 12:10:58.000000 reticuler-1.1/src/reticuler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      943 2023-06-22 12:10:58.000000 reticuler-1.1/src/reticuler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 12:10:58.000000 reticuler-1.1/src/reticuler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      236 2023-06-22 12:10:58.000000 reticuler-1.1/src/reticuler.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       28 2023-06-22 12:10:58.000000 reticuler-1.1/src/reticuler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-22 12:10:58.000000 reticuler-1.1/src/reticuler.egg-info/top_level.txt
```

### Comparing `reticuler-1.0/LICENSE` & `reticuler-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `reticuler-1.0/PKG-INFO` & `reticuler-1.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reticuler
-Version: 1.0
+Version: 1.1
 Summary: Simulations of spatial networks growth
 Author: Stanisław Żukowski
 Author-email: zukowski.st@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/stzukowski/reticuler
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -33,33 +33,29 @@
 ### Package installation
 ```
 pip install reticuler
 ```
 
 ## Usage
 
-During installation two command line scripts are installed:
-- *reticulate* - runs the simulation
-- *plot_ret* - plots the network based on the *.json* file from the simulation
+During the installation four command line scripts are installed:
+   - *reticulate* - runs the simulation
+   - *reticulate_back* - runs the the Backward Evolution Algorithm
+   - *clip_ret* - clips the network to one of the growth thresholds (maximum forward evolution step, length, height, evolution time, or BEA step)
+   - *plot_ret* - plots the network based on the *.json* file from the simulation
 
 To use just type in the command line:
 `reticulate -h`
-or
-`plot_ret -h`
 
 Typical network growth simulation:
 - output file: *test*,
 - growth threshold type: maximum network height,
 - growth threshold: 2
 ```
 reticulate -out test --growth_params {\"growth_thresh_type\":1,\"growth_thresh\":2}
 ```
 
 ## How to cite
-*Through history to growth dynamics: backward evolution of spatial networks*, S. Żukowski, P. Morawiecki, H. Seybold, P. Szymczak, Sci Rep 12, 20407 (2022). https://doi.org/10.1038/s41598-022-24656-x
+*Through history to growth dynamics: backward evolution of spatial networks*, S. Żukowski, P. Morawiecki, H. Seybold, P. Szymczak, Sci. Rep. 12, 20407 (2022). https://doi.org/10.1038/s41598-022-24656-x
 
 ### References
-[1]: [P. Morawiecki, *Problem odwrotny do ewolucji sieci rzecznych* (2016)](http://www.fuw.edu.pl/~piotrek/theses/PMorawiecki.pdf).
-
-[2]: [S. Żukowski, *Związek między geometrią sieci rzecznych a prawami ich wzrostu* (2019)](http://www.fuw.edu.pl/~piotrek/theses/SZukowski.pdf).
-
-[3]: [S. Żukowski, *Backward evolution of river networks* (2021)](http://www.fuw.edu.pl/~piotrek/theses/SZukowski2.pdf).
+*Bifurcation dynamics of natural drainage networks*,  A. Petroff, O. Devauchelle, H. Seybold, and D. H. Rothman. Philos. Trans. Royal Soc. A 371, no. 2004 (2013): 20120365.
```

#### html2text {}

```diff
@@ -1,27 +1,26 @@
-Metadata-Version: 2.1 Name: reticuler Version: 1.0 Summary: Simulations of
+Metadata-Version: 2.1 Name: reticuler Version: 1.1 Summary: Simulations of
 spatial networks growth Author: StanisÅaw Å»ukowski Author-email:
 zukowski.st@gmail.com License: MIT Project-URL: Source, https://github.com/
 stzukowski/reticuler Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.9 Description-Content-Type: text/
 markdown License-File: LICENSE # Reticuler
                [PyPI] [Documentation_Status] [Code_style:_black]
 Python package to simulate the growth of spatial networks in nature.
 [Documentation](https://reticuler.readthedocs.io/en/latest/) ## Setup ###
 External dependencies: [__FreeFEM++__](https://freefem.org/) - PDE solver ###
-Package installation ``` pip install reticuler ``` ## Usage During installation
-two command line scripts are installed: - *reticulate* - runs the simulation -
-*plot_ret* - plots the network based on the *.json* file from the simulation To
-use just type in the command line: `reticulate -h` or `plot_ret -h` Typical
-network growth simulation: - output file: *test*, - growth threshold type:
-maximum network height, - growth threshold: 2 ``` reticulate -out test --
-growth_params {\"growth_thresh_type\":1,\"growth_thresh\":2} ``` ## How to cite
-*Through history to growth dynamics: backward evolution of spatial networks*,
-S. Å»ukowski, P. Morawiecki, H. Seybold, P. Szymczak, Sci Rep 12, 20407 (2022).
-https://doi.org/10.1038/s41598-022-24656-x ### References [1]: [P. Morawiecki,
-*Problem odwrotny do ewolucji sieci rzecznych* (2016)](http://www.fuw.edu.pl/
-~piotrek/theses/PMorawiecki.pdf). [2]: [S. Å»ukowski, *ZwiÄzek miÄdzy
-geometriÄ sieci rzecznych a prawami ich wzrostu* (2019)](http://
-www.fuw.edu.pl/~piotrek/theses/SZukowski.pdf). [3]: [S. Å»ukowski, *Backward
-evolution of river networks* (2021)](http://www.fuw.edu.pl/~piotrek/theses/
-SZukowski2.pdf).
+Package installation ``` pip install reticuler ``` ## Usage During the
+installation four command line scripts are installed: - *reticulate* - runs the
+simulation - *reticulate_back* - runs the the Backward Evolution Algorithm -
+*clip_ret* - clips the network to one of the growth thresholds (maximum forward
+evolution step, length, height, evolution time, or BEA step) - *plot_ret* -
+plots the network based on the *.json* file from the simulation To use just
+type in the command line: `reticulate -h` Typical network growth simulation: -
+output file: *test*, - growth threshold type: maximum network height, - growth
+threshold: 2 ``` reticulate -out test --growth_params {\"growth_thresh_type\":
+1,\"growth_thresh\":2} ``` ## How to cite *Through history to growth dynamics:
+backward evolution of spatial networks*, S. Å»ukowski, P. Morawiecki, H.
+Seybold, P. Szymczak, Sci. Rep. 12, 20407 (2022). https://doi.org/10.1038/
+s41598-022-24656-x ### References *Bifurcation dynamics of natural drainage
+networks*, A. Petroff, O. Devauchelle, H. Seybold, and D. H. Rothman. Philos.
+Trans. Royal Soc. A 371, no. 2004 (2013): 20120365.
```

### Comparing `reticuler-1.0/README.md` & `reticuler-1.1/src/reticuler.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: reticuler
+Version: 1.1
+Summary: Simulations of spatial networks growth
+Author: Stanisław Żukowski
+Author-email: zukowski.st@gmail.com
+License: MIT
+Project-URL: Source, https://github.com/stzukowski/reticuler
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Reticuler
 
 <p align="center">
 <a href="https://pypi.org/project/reticuler/"><img alt="PyPI" src="https://img.shields.io/pypi/v/reticuler"></a>
 <a href='https://reticuler.readthedocs.io/en/latest/?badge=latest'><img src='https://readthedocs.org/projects/reticuler/badge/?version=latest' alt='Documentation Status'/></a>
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 </p>
@@ -18,33 +33,29 @@
 ### Package installation
 ```
 pip install reticuler
 ```
 
 ## Usage
 
-During installation two command line scripts are installed:
-- *reticulate* - runs the simulation
-- *plot_ret* - plots the network based on the *.json* file from the simulation
+During the installation four command line scripts are installed:
+   - *reticulate* - runs the simulation
+   - *reticulate_back* - runs the the Backward Evolution Algorithm
+   - *clip_ret* - clips the network to one of the growth thresholds (maximum forward evolution step, length, height, evolution time, or BEA step)
+   - *plot_ret* - plots the network based on the *.json* file from the simulation
 
 To use just type in the command line:
 `reticulate -h`
-or
-`plot_ret -h`
 
 Typical network growth simulation:
 - output file: *test*,
 - growth threshold type: maximum network height,
 - growth threshold: 2
 ```
 reticulate -out test --growth_params {\"growth_thresh_type\":1,\"growth_thresh\":2}
 ```
 
 ## How to cite
-*Through history to growth dynamics: backward evolution of spatial networks*, S. Żukowski, P. Morawiecki, H. Seybold, P. Szymczak, Sci Rep 12, 20407 (2022). https://doi.org/10.1038/s41598-022-24656-x
+*Through history to growth dynamics: backward evolution of spatial networks*, S. Żukowski, P. Morawiecki, H. Seybold, P. Szymczak, Sci. Rep. 12, 20407 (2022). https://doi.org/10.1038/s41598-022-24656-x
 
 ### References
-[1]: [P. Morawiecki, *Problem odwrotny do ewolucji sieci rzecznych* (2016)](http://www.fuw.edu.pl/~piotrek/theses/PMorawiecki.pdf).
-
-[2]: [S. Żukowski, *Związek między geometrią sieci rzecznych a prawami ich wzrostu* (2019)](http://www.fuw.edu.pl/~piotrek/theses/SZukowski.pdf).
-
-[3]: [S. Żukowski, *Backward evolution of river networks* (2021)](http://www.fuw.edu.pl/~piotrek/theses/SZukowski2.pdf).
+*Bifurcation dynamics of natural drainage networks*,  A. Petroff, O. Devauchelle, H. Seybold, and D. H. Rothman. Philos. Trans. Royal Soc. A 371, no. 2004 (2013): 20120365.
```

#### html2text {}

```diff
@@ -1,21 +1,26 @@
-# Reticuler
+Metadata-Version: 2.1 Name: reticuler Version: 1.1 Summary: Simulations of
+spatial networks growth Author: StanisÅaw Å»ukowski Author-email:
+zukowski.st@gmail.com License: MIT Project-URL: Source, https://github.com/
+stzukowski/reticuler Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
+:: OS Independent Requires-Python: >=3.9 Description-Content-Type: text/
+markdown License-File: LICENSE # Reticuler
                [PyPI] [Documentation_Status] [Code_style:_black]
 Python package to simulate the growth of spatial networks in nature.
 [Documentation](https://reticuler.readthedocs.io/en/latest/) ## Setup ###
 External dependencies: [__FreeFEM++__](https://freefem.org/) - PDE solver ###
-Package installation ``` pip install reticuler ``` ## Usage During installation
-two command line scripts are installed: - *reticulate* - runs the simulation -
-*plot_ret* - plots the network based on the *.json* file from the simulation To
-use just type in the command line: `reticulate -h` or `plot_ret -h` Typical
-network growth simulation: - output file: *test*, - growth threshold type:
-maximum network height, - growth threshold: 2 ``` reticulate -out test --
-growth_params {\"growth_thresh_type\":1,\"growth_thresh\":2} ``` ## How to cite
-*Through history to growth dynamics: backward evolution of spatial networks*,
-S. Å»ukowski, P. Morawiecki, H. Seybold, P. Szymczak, Sci Rep 12, 20407 (2022).
-https://doi.org/10.1038/s41598-022-24656-x ### References [1]: [P. Morawiecki,
-*Problem odwrotny do ewolucji sieci rzecznych* (2016)](http://www.fuw.edu.pl/
-~piotrek/theses/PMorawiecki.pdf). [2]: [S. Å»ukowski, *ZwiÄzek miÄdzy
-geometriÄ sieci rzecznych a prawami ich wzrostu* (2019)](http://
-www.fuw.edu.pl/~piotrek/theses/SZukowski.pdf). [3]: [S. Å»ukowski, *Backward
-evolution of river networks* (2021)](http://www.fuw.edu.pl/~piotrek/theses/
-SZukowski2.pdf).
+Package installation ``` pip install reticuler ``` ## Usage During the
+installation four command line scripts are installed: - *reticulate* - runs the
+simulation - *reticulate_back* - runs the the Backward Evolution Algorithm -
+*clip_ret* - clips the network to one of the growth thresholds (maximum forward
+evolution step, length, height, evolution time, or BEA step) - *plot_ret* -
+plots the network based on the *.json* file from the simulation To use just
+type in the command line: `reticulate -h` Typical network growth simulation: -
+output file: *test*, - growth threshold type: maximum network height, - growth
+threshold: 2 ``` reticulate -out test --growth_params {\"growth_thresh_type\":
+1,\"growth_thresh\":2} ``` ## How to cite *Through history to growth dynamics:
+backward evolution of spatial networks*, S. Å»ukowski, P. Morawiecki, H.
+Seybold, P. Szymczak, Sci. Rep. 12, 20407 (2022). https://doi.org/10.1038/
+s41598-022-24656-x ### References *Bifurcation dynamics of natural drainage
+networks*, A. Petroff, O. Devauchelle, H. Seybold, and D. H. Rothman. Philos.
+Trans. Royal Soc. A 371, no. 2004 (2013): 20120365.
```

### Comparing `reticuler-1.0/pyproject.toml` & `reticuler-1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.setuptools.packages.find]
 where = ["src"]  # list of folders that contain the packages (["."] by default)
 include = ["reticuler*"]  # package names should match these glob patterns (["*"] by default)
 
 [project]
 name = "reticuler"
-version = "1.0"
+version = "1.1"
 authors = [
 	{name="Stanisław Żukowski"},
 	{email="zukowski.st@gmail.com"}
 ]
 description = "Simulations of spatial networks growth"
 readme = "README.md"
 license = { text = "MIT" }
```

### Comparing `reticuler-1.0/src/reticuler/backward_evolution/system_back.py` & `reticuler-1.1/src/reticuler/backward_evolution/system_back.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import time
 import datetime
 import numpy as np
 import importlib.metadata
 import json
 
 from reticuler.system import NumpyEncoder
+from reticuler.backward_evolution import trimmers
 
 
 class BackwardBranch:
     """A class of a single branch in a network used to collect BEA metrics.
 
     Attributes
     ----------
@@ -25,14 +26,17 @@
         Branch ID.
     mother_ID : int
         ID of the mother branch (branch from which `self` bifrucated). 
         If `self` is connected to the border mother_ID=-1.
     points : array
         A 2-n array with xy coordinates of the points composing the branch.
         Chronological order of growth (tip is the last point).
+    nums_left : array
+        A 1-n array with the number of points left in the forward branch at the current BEA step.
+        Used to clip reconstruct the state of the network during BEA.
     steps : array
         A 1-n array with BEA steps at which corresponding points were added.
     a1a2a3_coefficients : array
         A 3-n array with a1,a2,a3 coefficients in a point after backward step.
     overshoot : array
         A 1-n array with overshoot after virtual forward step.
     angular_deflection : array
@@ -54,30 +58,32 @@
         None.
 
         """
         self.ID = ID
         self.mother_ID = mother_ID
 
         self.points = np.empty((0,2), dtype=float)  # in order of trimming
+        self.nums_left = [] # how many points are left in the forward branch
         self.steps = [] # at which step of the BEA the point was reached
 
         # arrays with BEA metrics are two elements shorter than points/steps
         # we don't collect metrics at the first and the last point of the initial branch
         self.a1a2a3_coefficients = np.empty((0,3), dtype=float)
         self.overshoot = []
         self.angular_deflection = []
         
-    def add_point(self, point, BEA_step):
+    def add_point(self, point, ind, BEA_step):
         """Add a new point to ``self.points`` (position of the tip after trimming)."""
         self.points = np.vstack((self.points, point))
+        self.nums_left = np.append(self.nums_left, ind)
         self.steps = np.append(self.steps, BEA_step)
 
-    def points_steps(self):
-        """Return a 3-n array of points and BEA steps when they were added."""
-        return np.column_stack((self.points, self.steps))
+    def points_numsleft_steps(self):
+        """Return a 3-n array of points, number of points left in the forward branch and BEA steps when they were added."""
+        return np.column_stack((self.points, self.nums_left, self.steps))
 
 
 class BackwardBifurcations:
     """A class containing BEA metrics at all bifurcation points.
 
     Attributes
     ----------
@@ -181,14 +187,149 @@
         self.backward_branches, self.backward_bifurcations = self.import_branches(self.system.network)
         self.system.extender.eta = self.trimmer.eta
         self.system.extender.bifurcation_type = 0
         self.system.extender.inflow_thresh = 0
         
         self.dump_every = dump_every
         self.exp_name = system.exp_name+'_back'
+        
+    @classmethod
+    def import_json(cls, input_file, system):
+        """Construct an instance of class BackwardSystem based on the imported .json file.
+
+        Parameters
+        ----------
+        input_file : path
+            Name of the experiment location. Extension '.json' will be added.
+
+        Returns
+        -------
+        backward_system : object of class BackwardSystem
+
+        """
+        with open(input_file + ".json", "r") as f:
+            json_load = json.load(f)
+
+        # Backward branches
+        backward_branches = []
+        for i in reversed(list(json_load["backward_branches"].keys())):
+            json_branch = json_load["backward_branches"][i]
+            backward_branch = BackwardBranch(
+                ID=json_branch["ID"],
+                mother_ID=json_branch["mother_ID"],
+            )
+            
+            points_numsleft_steps = np.asarray(json_branch["points_numsleft_steps"])
+            if points_numsleft_steps.size:
+                backward_branch.points = points_numsleft_steps[:, :2]
+                backward_branch.nums_left = np.array(points_numsleft_steps[:, 2], dtype=int)
+                backward_branch.steps = np.array(points_numsleft_steps[:, 3], dtype=int)
+                backward_branch.a1a2a3_coefficients = np.asarray(json_branch["a1a2a3_coefficients"])
+                backward_branch.overshoot = np.asarray(json_branch["overshoot"])
+                backward_branch.angular_deflection = np.asarray(json_branch["angular_deflection"])
+
+            backward_branches.append(backward_branch)
+
+        # BackwardBifurcations
+        bif_info = np.asarray(json_load["backward_bifurcations"]["bif_info"])
+        backward_bifurcations = BackwardBifurcations(np.array(bif_info[:,0],dtype=int))
+        backward_bifurcations.a1a2a3_coefficients = bif_info[:, 1:4]
+        backward_bifurcations.length_mismatch = bif_info[:, 4]
+        backward_bifurcations.flags = np.array(bif_info[:,5], dtype=int)
+
+        # Trimmer
+        json_trimmer = json_load["trimmer"]
+        if json_trimmer["type"] == "BackwardModifiedEulerMethod":
+            trimmer = trimmers.BackwardModifiedEulerMethod(
+                pde_solver=system.extender.pde_solver,
+                eta=json_trimmer["eta"],
+                ds=json_trimmer["ds"],
+                max_approximation_step=json_trimmer["max_approximation_step"],
+                inflow_thresh=json_trimmer["inflow_thresh"],
+            )
+
+        # General
+        json_BEA_parameters = json_load["BEA_parameters"]
+        BEA_step = json_BEA_parameters["BEA_step"]
+        BEA_step_thresh = json_BEA_parameters["BEA_step_thresh"]
+        back_forth_steps_thresh = json_BEA_parameters["back_forth_steps_thresh"]
+        dump_every = json_BEA_parameters["dump_every"]
+
+        backward_system = cls(
+            system=system,
+            trimmer=trimmer,
+            BEA_step_thresh=BEA_step_thresh,
+            back_forth_steps_thresh=back_forth_steps_thresh,
+            dump_every=dump_every,
+        )
+        backward_system.BEA_step = BEA_step
+        backward_system.backward_branches = backward_branches
+        backward_system.backward_bifurcations = backward_bifurcations
+
+        return backward_system
+
+    def export_json(self):
+        """Export all the information to 'self.exp_name'+'.json'."""
+        
+        export_general = {
+            "reticuler_version": importlib.metadata.version("reticuler"),
+            "exp_name": self.exp_name,
+            "BEA_parameters": {
+                "back_forth_steps_thresh": self.back_forth_steps_thresh,
+                "BEA_step": self.BEA_step,
+                "BEA_step_thresh": self.BEA_step_thresh,
+                "dump_every": self.dump_every,
+            },
+        }
+        
+        if type(self.trimmer.pde_solver).__name__ == "FreeFEM":
+            equation_legend = ["Laplace", "Poisson"]
+            export_solver = {
+                "type": type(self.trimmer.pde_solver).__name__,
+                "equation": equation_legend[self.trimmer.pde_solver.equation],
+            }
+        
+        if type(self.trimmer).__name__ == "BackwardModifiedEulerMethod":
+            export_trimmer = {
+                    "trimmer": {
+                        "type": type(self.trimmer).__name__,
+                        "eta": self.trimmer.eta,
+                        "ds": self.trimmer.ds,
+                        "max_approximation_step": self.trimmer.max_approximation_step,
+                        "inflow_thresh": self.trimmer.inflow_thresh,
+                        "pde_solver": {**export_solver},
+                    }
+                }
+
+        export_backward_bifurcations = {
+            "backward_bifurcations": {
+                "description": "Information gathered in the bifurcation points: mother_ID, a1, a2, a3, length mismatch, flag",
+                "bif_info": self.backward_bifurcations.bif_info(),
+            }
+        }
+        
+        export_backward_branches = {}
+        for branch in self.backward_branches[::-1]:
+            branch_dict = {
+                branch.ID: {
+                    "ID": branch.ID,
+                    "mother_ID": branch.mother_ID,
+                    "points_numsleft_steps": branch.points_numsleft_steps(),
+                    "a1a2a3_coefficients": branch.a1a2a3_coefficients,
+                    "overshoot": branch.overshoot,
+                    "angular_deflection": branch.angular_deflection,
+                }
+            }
+            export_backward_branches = export_backward_branches | branch_dict
+        export_backward_branches = { "backward_branches": {**export_backward_branches} }
+        
+        to_export = export_general | export_trimmer | export_backward_bifurcations | export_backward_branches
+        with open(self.exp_name + ".json", "w", encoding="utf-8") as f:
+            json.dump(to_export, f, ensure_ascii=False,
+                      indent=4, cls=NumpyEncoder)
 
     def import_branches(self, network):
         """Reorganizing and importing branches from the networks.
         
         Parameters
         ----------
         network : Network
@@ -210,46 +351,103 @@
         for i, forward_branch in enumerate(network.branches):
             network.branch_connectivity[branch_connectivity_0 ==
                                         forward_branch.ID] = i
             network.box.seeds_connectivity[seeds_connectivity_0[:, 1]
                                            == forward_branch.ID, 1] = i
             forward_branch.ID = i
             
-            mother = network.branch_connectivity[
-                network.branch_connectivity[:,1]==i, 0]
-            if mother.size > 0:
-                mother_ID = mother[0]
-                mother_IDs.append(mother[0])
-            else:
+            if network.branch_connectivity.size==0:
                 mother_ID = -1
+                network.active_branches.append(forward_branch)
+            else:
+                mother = network.branch_connectivity[
+                    network.branch_connectivity[:,1]==i, 0]
+                if mother.size > 0:
+                    mother_ID = mother[0]
+                    mother_IDs.append(mother[0])
+                else:
+                    mother_ID = -1
                 
             # forward/backward branch ID is its index in backward_branches
             backward_branches.append(BackwardBranch(ID=i, mother_ID=mother_ID))
             
             # free node ==> active branch
-            if np.isin(forward_branch.ID, network.branch_connectivity[:,0], invert=True):
+            if network.branch_connectivity.size!=0 and \
+                np.isin(forward_branch.ID, network.branch_connectivity[:,0], invert=True):
                 network.active_branches.append(forward_branch)
 
         # above, we go over branches, so the mother_IDs are repeated; hence np.unique
         backward_bifurcations = BackwardBifurcations(np.unique(mother_IDs))
 
         return backward_branches, backward_bifurcations
 
+    def __compare_networks(self, initial_network, backward_network, test_network, a1a2a3_coefficients):
+        """Gathering BEA metrics.
+        
+        Parameters
+        ----------
+        initial_network : Network
+        backward_network : Network
+            Network after backward step.
+        test_network : Network
+            Network after backward-forward step.
+        a1a2a3_coefficients : array
+            A 3-n array with a1,a2,a3 coefficients after backward step.
+
+        Returns
+        -------
+        None.
+        
+        """
+
+        for i in range(len(initial_network.active_branches)):
+            backward_branch = self.backward_branches[initial_network.active_branches[i].ID]
+            bifurcation_ind = self.backward_bifurcations.mother_IDs == \
+                backward_branch.mother_ID
+                
+            # if we've reached the bifurcation point for the second time
+            if self.backward_bifurcations.flags[bifurcation_ind]==2:
+                self.backward_bifurcations.flags[bifurcation_ind] = 3
+                self.backward_bifurcations.a1a2a3_coefficients[bifurcation_ind] = a1a2a3_coefficients[i]
+                # length_mismatch is saved in the trimmer after first visit in the bifurcation point
+        
+            # if we haven't reached the bifurcation point
+            # (if we've reached it only once then the branched is popped from active_branches)
+            else:
+                initial_point = initial_network.active_branches[i].points[-1]
+                back_point = backward_network.active_branches[i].points[-1]
+                test_point = test_network.active_branches[i].points[-1]
+    
+                # for angular deflection
+                v1 = initial_point - back_point
+                real_angle = np.arctan2(v1[1], v1[0])
+                v2 = test_point - back_point
+                test_angle = np.arctan2(v2[1], v2[0])
+    
+                # overshoot
+                backward_branch.overshoot = np.append(backward_branch.overshoot, \
+                                                      np.linalg.norm(test_point - initial_point))
+                # angular deflection
+                backward_branch.angular_deflection = np.append(backward_branch.angular_deflection, \
+                                                               real_angle-test_angle)
+                # a1, a2, a3 coefficients
+                backward_branch.a1a2a3_coefficients = np.vstack((backward_branch.a1a2a3_coefficients, a1a2a3_coefficients[i]))
+                
     def run_BEA(self):
         """Run the Backward Evolution Algorithm.
 
         Returns
         -------
         None.
 
         """
         start_clock = time.time()
         backward_dts = np.empty(self.back_forth_steps_thresh)
         # while branches list is not empty
-        while not len(self.system.network.branches)==1 or self.BEA_step < self.BEA_step_thresh:
+        while not len(self.system.network.branches)==1 and self.BEA_step < self.BEA_step_thresh:
             self.BEA_step = self.BEA_step + 1
             print(
                 "\n-------------------   Backward Evolution Algorithm step: {step:.0f}   -------------------\n".format(
                     step=self.BEA_step
                 )
             )
             print("Date and time: ", datetime.datetime.now())
@@ -281,125 +479,17 @@
 
             # compare the network before and after the backward-forward steps
             self.__compare_networks(
                 initial_network, self.system.network, test_network, a1a2a3_coefficients)
 
             if not self.BEA_step % self.dump_every:
                 self.export_json()
-                self.system.export_json()
+                # self.system.export_json()
 
         self.export_json()
-        self.system.export_json()
+        # self.system.export_json()
 
         print(
             "\n End of the Backward Evolution Algorithm. Time: {clock:.2f}s".format(
                 clock=time.time() - start_clock
             )
         )        
-
-    def __compare_networks(self, initial_network, backward_network, test_network, a1a2a3_coefficients):
-        """Gathering BEA metrics.
-        
-        Parameters
-        ----------
-        initial_network : Network
-        backward_network : Network
-            Network after backward step.
-        test_network : Network
-            Network after backward-forward step.
-        a1a2a3_coefficients : array
-            A 3-n array with a1,a2,a3 coefficients after backward step.
-
-        Returns
-        -------
-        None.
-        
-        """
-
-        for i in range(len(initial_network.active_branches)):
-            backward_branch = self.backward_branches[initial_network.active_branches[i].ID]
-            bifurcation_ind = self.backward_bifurcations.mother_IDs == \
-                initial_network.active_branches[i].ID
-                
-            # if we've reached the bifurcation point for the second time
-            if self.backward_bifurcations.flags[bifurcation_ind]==2:
-                self.backward_bifurcations.flags[bifurcation_ind] = 3
-                self.backward_bifurcations.a1a2a3_coefficients[bifurcation_ind] = a1a2a3_coefficients[i]
-                # length_mismatch is saved in the trimmer after first visit in the bifurcation point
-        
-            # if we haven't reached the bifurcation point
-            # (if we've reached it only once then the branched is popped from active_branches)
-            else:
-                initial_point = initial_network.active_branches[i].points[-1]
-                back_point = backward_network.active_branches[i].points[-1]
-                test_point = test_network.active_branches[i].points[-1]
-    
-                # for angular deflection
-                v1 = initial_point - back_point
-                v1 = v1 / np.linalg.norm(v1)
-                v2 = test_point - back_point
-                v2 = v2 / np.linalg.norm(v2)
-    
-                # overshoot
-                backward_branch.overshoot.append(
-                    np.linalg.norm(test_point - initial_point))
-                # angular deflection
-                backward_branch.angular_deflection.append(
-                    np.arccos(np.clip(np.dot(v1, v2), -1.0, 1.0)))
-                # a1, a2, a3 coefficients
-                backward_branch.a1a2a3_coefficients = np.vstack((backward_branch.a1a2a3_coefficients, a1a2a3_coefficients[i]))
-                
-    def export_json(self):
-        """Export all the information to 'self.exp_name'+'.json'."""
-        
-        export_general = {
-            "reticuler_version": importlib.metadata.version("reticuler"),
-            "exp_name": self.exp_name,
-            "BEA_parameters": {
-                "back_forth_steps_thresh": self.back_forth_steps_thresh,
-                "BEA_step": self.BEA_step,
-                "BEA_step_thresh": self.BEA_step_thresh,
-                "dump_every": self.dump_every,
-            },
-        }
-        
-        if type(self.trimmer.pde_solver).__name__ == "FreeFEM":
-            equation_legend = ["Laplace", "Poisson"]
-            export_solver = {
-                "type": type(self.trimmer.pde_solver).__name__,
-                "equation": equation_legend[self.trimmer.pde_solver.equation],
-            }
-        
-        if type(self.trimmer).__name__ == "BackwardModifiedEulerMethod":
-            export_trimmer = {
-                "type": type(self.trimmer).__name__,
-                "eta": self.trimmer.eta,
-                "ds": self.trimmer.ds,
-                "max_approximation_step": self.trimmer.max_approximation_step,
-                "inflow_thresh": self.trimmer.inflow_thresh,
-                "pde_solver": {**export_solver},
-            }
-
-        export_backward_bifurcations = {
-            "description": "Information gathered in the bifurcation points: mother_ID, a1, a2, a3, length mismatch, flag",
-            "bif_info": self.backward_bifurcations.bif_info(),
-        }
-
-        export_backward_branches = {}
-        for branch in self.backward_branches[::-1]:
-            branch_dict = {
-                branch.ID: {
-                    "ID": branch.ID,
-                    "mother_ID": branch.mother_ID,
-                    "points_and_steps": branch.points_steps(),
-                    "a1a2a3_coefficients": branch.a1a2a3_coefficients,
-                    "overshoot": branch.overshoot,
-                    "angular_deflection": branch.angular_deflection,
-                }
-            }
-            export_backward_branches = export_backward_branches | branch_dict
-    
-        to_export = export_general | export_trimmer | export_backward_bifurcations | export_backward_branches
-        with open(self.exp_name + ".json", "w", encoding="utf-8") as f:
-            json.dump(to_export, f, ensure_ascii=False,
-                      indent=4, cls=NumpyEncoder)
-
```

### Comparing `reticuler-1.0/src/reticuler/backward_evolution/trimmers.py` & `reticuler-1.1/src/reticuler/backward_evolution/trimmers.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,15 +40,15 @@
             https://doi.org/10.1038/s41598-022-24656-x
     .. [Ref3] https://en.wikipedia.org/wiki/Trapezoidal_rule_(differential_equations)
 
     """
     def __init__(
         self,
         pde_solver,
-        eta=1.0,
+        eta=0.0,
         ds=0.01,
         max_approximation_step=3,
         inflow_thresh = 0.05,
     ):
         """Initialize BackwardModifiedEulerMethod.
 
         Parameters
@@ -70,14 +70,139 @@
         self.ds = ds
 
         self.max_approximation_step = max_approximation_step
         
         # less than `inflow_thresh` of max flux/velocity puts branches asleep
         self.inflow_thresh = inflow_thresh
         
+    def __check_moving_conditions(self, network):
+        """Check moving conditions."""
+        a1 = self.pde_solver.a1a2a3_coefficients[:, 0]
+        max_a1 = np.max(a1)
+        # (first condition for low eta, second for high)
+        are_moving = np.logical_and(a1/max_a1 > self.inflow_thresh,
+                                   (a1/max_a1)**self.eta > self.inflow_thresh)
+        # shallow copy of active_branches (creates new list instance, but the elements are still the same)
+        branches_to_iterate = network.active_branches.copy()
+        for i, branch in enumerate(branches_to_iterate):
+            if not are_moving[i]:
+                network.sleeping_branches.append(branch)
+                network.active_branches.remove(branch)
+                # print("! Branch {ID} is sleeping !".format(ID=branch.ID))                
+        return are_moving
+
+    def __explicit_network_trim(self, test_network, drs_0, backward_branches, backward_bifurcations, BEA_step):
+        """Trim branches with given ``drs``."""
+        min_distance = 0.0001  # avoid two nodes very close to each other after trimming
+
+        drs = drs_0.copy()
+        branches_to_iterate = test_network.active_branches.copy()
+        are_living_after_bif = np.ones(len(branches_to_iterate), dtype=bool)
+        for i, forward_branch in enumerate(branches_to_iterate):
+            
+            while drs[i] > 0:
+                backward_branch = backward_branches[forward_branch.ID]
+                # check the distances from the tip to bifurcation point
+                segment_lengths = np.linalg.norm(
+                    forward_branch.points[1:]-forward_branch.points[:-1], axis=1)
+                length_from_tip = np.cumsum(segment_lengths[::-1])
+                       
+                # bifurcation not reached
+                if drs[i]+min_distance < length_from_tip[-1]:
+                    are_living_after_bif[i] = True
+                    
+                    # how many points to remove
+                    to_remove = np.sum(drs[i]+min_distance > length_from_tip)
+                    
+                    if to_remove>0:
+                        forward_branch.points = forward_branch.points[:-to_remove]
+                        forward_branch.steps = forward_branch.steps[:-to_remove]
+                        drs[i] = drs[i] - length_from_tip[to_remove-1]
+                    
+                    # shifting the last point
+                    if drs[i]!=0:
+                        tip_versor = forward_branch.points[-1] - forward_branch.points[-2]
+                        tip_versor = tip_versor / np.linalg.norm(tip_versor)
+                        forward_branch.points[-1] = forward_branch.points[-1] - tip_versor * drs[i]
+                        backward_branch.add_point(forward_branch.points[-1], len(forward_branch.points)-1, BEA_step) 
+                        drs[i] = 0
+                # bifurcation reached
+                else:
+                    drs[i] = drs[i] - length_from_tip[-1]
+                    backward_branch.add_point(forward_branch.points[0], 0, BEA_step) 
+                                    
+                    mask = test_network.branch_connectivity[:,1]!=forward_branch.ID
+                    test_network.branch_connectivity = test_network.branch_connectivity[mask,...]
+                    test_network.branches.remove(forward_branch)
+                    ind_branch = test_network.active_branches.index(forward_branch)
+                    
+                    # if we reach the border
+                    if backward_branch.mother_ID==-1:
+                        mask = test_network.box.seeds_connectivity[:,1]!=forward_branch.ID
+                        test_network.box.seeds_connectivity = test_network.box.seeds_connectivity[mask,...]
+                        test_network.active_branches.pop(ind_branch)
+                    # bifurcation point
+                    else:
+                        ind_bifurcation = backward_bifurcations.mother_IDs==backward_branch.mother_ID
+                        if backward_bifurcations.flags[ind_bifurcation] == 0:
+                            print("! Branch {ID} reached bifurcation {bifID} ! (1st one)".format(ID=backward_branch.ID, bifID=backward_branch.mother_ID))
+                            backward_bifurcations.flags[ind_bifurcation] = 1
+                            are_living_after_bif[i] = False
+                            # branched is later poped from initial_network (back in the trim method)
+                            test_network.active_branches.pop(ind_branch)
+                            
+                            # total length of the remaining branches connected to the mother branch
+                            remaining_length, remaining_IDs = self.__calculate_remaining_length(test_network, backward_branch.mother_ID)
+                            inds_remaining = [i for i, b in enumerate(branches_to_iterate) if b.ID in remaining_IDs]
+                            
+                            # if drs[i]>0 when tip(i) reaches the bifPoint, then dt was too big;
+                            # we compansate the effect by adding the 'virtual length'
+                            virtual_length = drs[i] / drs_0[i] * np.sum(drs_0[inds_remaining])
+                            
+                            # if remaining branches weren't moved yet we have to subtract their drs
+                            length_mismatch = remaining_length + virtual_length - np.sum(drs[inds_remaining])
+                            
+                            # if length_mismatch < 0 then we have to reverse the above line and calculate virtual_length for the remaining tip
+                            if length_mismatch < 0:
+                                virtual_length = (np.sum(drs[inds_remaining])-remaining_length) / np.sum(drs_0[inds_remaining]) * drs_0[i]
+                                length_mismatch = virtual_length - drs[i]
+                            
+                            backward_bifurcations.length_mismatch[ind_bifurcation] = length_mismatch
+                            drs[i] = 0 # stops while loop
+                            
+                        elif backward_bifurcations.flags[ind_bifurcation] == 1:
+                            print("! Branch {ID} reached bifurcation {bifID} ! (2nd one)".format(ID=backward_branch.ID, bifID=backward_branch.mother_ID))
+                            backward_bifurcations.flags[ind_bifurcation] = 2
+                            are_living_after_bif[i] = True
+                            
+                            mother_branch = [b for b in test_network.branches if b.ID==backward_branch.mother_ID][0]
+                            forward_branch = mother_branch
+                            test_network.active_branches[ind_branch] = mother_branch
+                        
+        return are_living_after_bif
+    
+    
+    def __calculate_remaining_length(self, network, mother_ID):
+        to_check = network.branch_connectivity[network.branch_connectivity[:,0]==mother_ID,1]
+        branch_IDs = np.array([b.ID for b in network.branches])
+        remaining_length = 0
+        remaining_IDs = []
+        while to_check.size:
+            next_ID = to_check[0]
+            remaining_length = remaining_length + network.branches[np.where(branch_IDs==next_ID)[0][0]].length()
+            
+            to_add = network.branch_connectivity[network.branch_connectivity[:,0]==next_ID,1]
+            if to_add.size:
+                to_check = np.concatenate((to_check, to_add))
+                remaining_IDs.append(next_ID)
+            else:
+                remaining_IDs.append(next_ID)
+            to_check = to_check[1:]
+        return remaining_length, remaining_IDs
+    
     def trim(self, network, backward_branches_0, backward_bifurcations_0, BEA_step):
         """Perform backward step with the reversed modified Euler's method and the streamline algorithm.
     
         Parameters
         ----------
         network : Network
             An object of class Network.
@@ -103,15 +228,15 @@
         
         Returns
         -------
         None.
                 
         """
         # activate sleeping branches        
-        network.active_branches = network.active_branches + network.sleeping_branches
+        network.active_branches = network.sleeping_branches + network.active_branches
         network.sleeping_branches = []
         
         # v[x(n)]: finding velocity at the starting point
         self.pde_solver.solve_PDE(network)
         velocity_0 = self.pde_solver.a1a2a3_coefficients[:, 0]**self.eta
         dt_0 = self.ds / np.max(velocity_0)
         drs_0 = dt_0 * velocity_0
@@ -122,32 +247,31 @@
         initial_network = network.copy()
         
         # x(n-1): trimming drs_0 from test_network
         backward_branches = copy.deepcopy(backward_branches_0)
         backward_bifurcations = copy.deepcopy(backward_bifurcations_0)
         test_network = network.copy()
         are_living_after_bif = self.__explicit_network_trim(test_network, drs_0, backward_branches, backward_bifurcations, BEA_step)
-
         if test_network.active_branches:
             drs = np.zeros_like(drs_0)   
             approximation_step = 0
             # APPROXIMATION LOOP
             while approximation_step < self.max_approximation_step and not (~are_living_after_bif).all():
                 approximation_step = approximation_step + 1
 
                 # v[x(n-1)]: finding velocity at the x(n-1) point
                 self.pde_solver.solve_PDE(test_network)
                 velocity_1 = self.pde_solver.a1a2a3_coefficients[:, 0]**self.eta
                 drs_1 = dt_0 * velocity_1
 
                 # 0.5 * dt * (v[x(n)] + v[x(n-1)]): average drs
-                drs[np.logical_not(are_living_after_bif)] = drs_0[np.logical_not(are_living_after_bif)] / 2
+                # drs[np.logical_not(are_living_after_bif)] = drs_0[np.logical_not(are_living_after_bif)] / 2
                 # !!! dead tips after bif don't move, so dt*(v[x(n)] + v[x(n-1)])/2 = dt*v[x(n-1)]/2 - it was commented in matlab code?
                 drs[are_living_after_bif] = (drs_0[are_living_after_bif] + drs_1) / 2
-                velocity = drs/dt_0
+                velocity = drs / dt_0
                 dt = self.ds / np.max(velocity)
                 drs = dt * velocity
 
                 # improved x(n-1)
                 backward_branches = copy.deepcopy(backward_branches_0)
                 backward_bifurcations = copy.deepcopy(backward_bifurcations_0)
                 test_network = network.copy()
@@ -155,127 +279,7 @@
                 
             initial_network.active_branches = [b for i, b in enumerate(network.active_branches) if are_living_after_bif[i]]
         else:
             dt = 0
         
         return initial_network, test_network, backward_branches, backward_bifurcations, dt        
         
-    def __check_moving_conditions(self, network):
-        """Check moving conditions."""
-        a1 = self.pde_solver.a1a2a3_coefficients[:, 0]
-        max_a1 = np.max(a1)
-        # (first condition for low eta, second for high)
-        are_moving = np.logical_and(a1/max_a1 > self.inflow_thresh,
-                                   (a1/max_a1)**self.eta > self.inflow_thresh)
-        # shallow copy of active_branches (creates new list instance, but the elements are still the same)
-        branches_to_iterate = network.active_branches.copy()
-        for i, branch in enumerate(branches_to_iterate):
-            if not are_moving[i]:
-                network.sleeping_branches.append(branch)
-                network.active_branches.remove(branch)
-                # print("! Branch {ID} is sleeping !".format(ID=branch.ID))                
-        return are_moving
-
-    def __explicit_network_trim(self, test_network, drs, backward_branches, backward_bifurcations, BEA_step):
-        """Trim branches with given ``drs``."""
-        min_distance = 0.0001  # avoid two nodes very close to each other after trimming
-
-        drs_0 = drs.copy()
-        branches_to_iterate = test_network.active_branches.copy()
-        are_living_after_bif = np.ones(len(branches_to_iterate), dtype=bool)
-        for i, forward_branch in enumerate(branches_to_iterate):
-            backward_branch = backward_branches[forward_branch.ID]
-            # if len(backward_branch.steps)==0 or backward_branch.steps[-1]<BEA_step-1:
-            backward_branch.add_point(forward_branch.points[-1], BEA_step-1) 
-            
-            # check the distances from the tip to bifurcation point
-            segment_lengths = np.linalg.norm(
-                forward_branch.points[1:]-forward_branch.points[:-1], axis=1)
-            length_from_tip = np.cumsum(segment_lengths[::-1])
-            
-            # bifurcation not reached
-            if drs[i]+min_distance < length_from_tip[-1]:
-                are_living_after_bif[i] = True
-                
-                # how many points to remove
-                to_remove = np.sum(drs[i]+min_distance > length_from_tip)
-                
-                if to_remove:
-                    forward_branch.points = forward_branch.points[:-to_remove]
-                    forward_branch.steps = forward_branch.steps[:-to_remove]
-                    drs[i] = drs[i] - length_from_tip[to_remove-1]
-                
-                # shifting the last point
-                if drs[i] > 0:
-                    tip_versor = forward_branch.points[-1] - forward_branch.points[-2]
-                    tip_versor = tip_versor / np.linalg.norm(tip_versor)
-                    forward_branch.points[-1] = forward_branch.points[-1] - tip_versor * drs[i]
-                    
-            # bifurcation reached
-            else:
-                drs[i] = drs[i] - length_from_tip[-1]
-                # if backward_branch.steps[-1]<BEA_step:
-                backward_branch.add_point(forward_branch.points[-1], BEA_step)
-                                
-                mask = test_network.branch_connectivity[:,1]!=forward_branch.ID
-                test_network.branch_connectivity = test_network.branch_connectivity[mask,...]
-                test_network.branches.remove(forward_branch)
-                ind_branch = test_network.active_branches.index(forward_branch)
-                
-                # if we reach the border
-                if backward_branch.mother_ID==-1:
-                    mask = test_network.box.seeds_connectivity[:,1]!=forward_branch.ID
-                    test_network.box.seeds_connectivity = test_network.box.seeds_connectivity[mask,...]
-                    test_network.active_branches.pop(ind_branch)
-                # bifurcation point
-                else:
-                    ind_bifurcation = backward_bifurcations.mother_IDs==backward_branch.mother_ID
-                    if backward_bifurcations.flags[ind_bifurcation] == 0:
-                        backward_bifurcations.flags[ind_bifurcation] = 1
-                        # branched is later poped from initial_network (back in the trim method)
-                        test_network.active_branches.pop(ind_branch)
-                        are_living_after_bif[i] = False
-                        
-                        # total length of the remaining branches connected to the mother branch
-                        remaining_length, remaining_IDs = self.__calculate_remaining_length(test_network, backward_branch.mother_ID)
-                        inds_remaining = [i for i, b in enumerate(branches_to_iterate) if b.ID in remaining_IDs]
-                        
-                        # if drs[i]>0 when tip(i) reaches the bifPoint, then dt was too big;
-                        # we compansate the effect by adding the 'virtual length'
-                        virtual_length = drs[i] / drs_0[i] * np.sum(drs_0[inds_remaining])
-                        
-                        # if remaining branches weren't moved yet we have to subtract their drs
-                        length_mismatch = remaining_length + virtual_length - np.sum(drs[inds_remaining])
-                        
-                        # if length_mismatch < 0 then we have to reverse the above line and calculate virtual_length for the remaining tip
-                        if length_mismatch < 0:
-                            virtual_length = (np.sum(drs[inds_remaining])-remaining_length) / np.sum(drs_0[inds_remaining]) * drs_0[i]
-                            length_mismatch = virtual_length - drs[i]
-                        
-                        backward_bifurcations.length_mismatch[ind_bifurcation] = length_mismatch
-                        
-                    elif backward_bifurcations.flags[ind_bifurcation] == 1:
-                        backward_bifurcations.flags[ind_bifurcation] = 2
-                        
-                        mother_branch = [b for b in test_network.branches if b.ID==backward_branch.mother_ID][0]
-                        test_network.active_branches[ind_branch] = mother_branch
-                        are_living_after_bif[i] = True
-
-        return are_living_after_bif
-    
-    
-    def __calculate_remaining_length(self, network, mother_ID):
-        to_check = network.branch_connectivity[network.branch_connectivity[:,0]==mother_ID,1]
-        branch_IDs = np.array([b.ID for b in network.branches])
-        remaining_length = 0
-        remaining_IDs = []
-        while to_check:
-            next_ID = to_check[0]
-            remaining_length = remaining_length + network.branches[np.where(branch_IDs==next_ID)[0][0]].length()
-            
-            to_add = network.branch_connectivity[network.branch_connectivity[:,0]==next_ID,1]
-            if to_add:
-                to_check = np.concatenate((to_check, to_add))
-            else:
-                remaining_IDs.append(next_ID)
-            to_check = to_check[1:]
-        return remaining_length, remaining_IDs
```

### Comparing `reticuler-1.0/src/reticuler/extending_kernels/extenders.py` & `reticuler-1.1/src/reticuler/extending_kernels/extenders.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,29 +196,30 @@
             An n-2 array with dx and dy shifts for each tip.
 
         """
         # running PDE solver
         # self.pde_solver.a1a2a3_coefficients are updated in FreeFEM solver
         self.pde_solver.solve_PDE(network)
 
-        # dr_norm = 1, ds <=> dt
-        dr_norm = 1
         if is_BEA_off:
             # normalize dr, so that the fastest tip moves over ds
             dr_norm = np.max(self.pde_solver.a1a2a3_coefficients[..., 0] ** self.eta)
+        else:
+            # dr_norm = 1, ds <=> dt
+            dr_norm = 1
         dRs_test = np.empty((len(network.active_branches), 2))
         for i, branch in enumerate(network.active_branches):
             a1 = self.pde_solver.a1a2a3_coefficients[i, 0]
             a2 = self.pde_solver.a1a2a3_coefficients[i, 1]
             beta = a1 / a2
 
             # __streamline_extension formula is derived in the coordinate
             # system where the tip segment lies on a negative Y axis;
             # hence, we rotate obtained dR vector to that system
-            tip_angle = branch.tip_angle()
+            tip_angle = np.pi / 2 - branch.tip_angle()
             dr = self.ds * a1**self.eta / dr_norm
             dRs_test[i] = np.dot(
                 self.__rotation_matrix(
                     tip_angle), self.__streamline_extension(beta, dr)
             )
         return dRs_test
```

### Comparing `reticuler-1.0/src/reticuler/extending_kernels/pde_solvers.py` & `reticuler-1.1/src/reticuler/extending_kernels/pde_solvers.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     
 """
 
 import numpy as np
 import subprocess
 import os.path
 import os
+from platform import system
 from tempfile import NamedTemporaryFile
 import textwrap
 
 
 class FreeFEM:
     """PDE solver based on the finite element method implemented in FreeFEM [Ref2]_.
 
@@ -125,15 +126,15 @@
             x1 = network.box.points[triple[1], 0]
             y1 = network.box.points[triple[1], 1]
             boundary_condition = triple[2]
             n_points = np.max((1, int(np.sqrt((x0 - x1) ** 2 + (y0 - y1) ** 2) / 2)))
 
             border_box = (
                 border_box
-                + "border box{i}(t=0, 1){{x={x0}+t*({ax});y={y0}+t*({ay}); label={bc};}}\n".format(
+                + "border box{i}(t=0, 1){{x={x0:.12g}+t*({ax:.12g});y={y0:.12g}+t*({ay:.12g}); label={bc};}}\n".format(
                     i=i, x0=x0, ax=x1 - x0, y0=y0, ay=y1 - y0, bc=boundary_condition
                 )
             )
 
             inside_buildmesh = inside_buildmesh + " box{i}({n}) +".format(
                 i=i, n=n_points
             )
@@ -144,15 +145,15 @@
                 x0 = pair[0][0]
                 y0 = pair[0][1]
                 x1 = pair[1][0]
                 y1 = pair[1][1]
 
                 border_network = (
                     border_network
-                    + "border branch{i}connection{j}(t=0, 1){{x={x0}+t*({ax});y={y0}+t*({ay}); label=1;}}\n".format(
+                    + "border branch{i}connection{j}(t=0, 1){{x={x0:.12g}+t*({ax:.12g});y={y0:.12g}+t*({ay:.12g}); label=1;}}\n".format(
                         i=i, j=j, x0=x0, ax=x1 - x0, y0=y0, ay=y1 - y0
                     )
                 )
 
                 inside_buildmesh = (
                     inside_buildmesh + " branch{i}connection{j}(1) +".format(i=i, j=j)
                 )
@@ -187,18 +188,18 @@
             """.format(
                 n_tips=len(network.active_branches)
             )
         )
         for i, branch in enumerate(network.active_branches):
             tip_information = (
                 tip_information
-                + "\nX({j})={x};".format(j=i, x=branch.points[-1, 0])
-                + "\nY({j})={y};".format(j=i, y=branch.points[-1, 1])
-                + "\nangle({j})={angle};".format(
-                    j=i, angle=np.pi / 2 - branch.tip_angle()
+                + "\nX({j})={x:.12g};".format(j=i, x=branch.points[-1, 0])
+                + "\nY({j})={y:.12g};".format(j=i, y=branch.points[-1, 1])
+                + "\nangle({j})={angle:.12g};".format(
+                    j=i, angle=branch.tip_angle()
                 )
             )  # angle with X axis
         tip_information = tip_information + "\n"
 
         problem_Laplace = textwrap.dedent(
             """
             ///////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
@@ -296,40 +297,43 @@
             real coeffTime0=clock();
             // cout << endl << endl << "Finding the Tip coefficients..." << endl;
             
             mesh Ph;
             real[int] a(3); // list of coefficients of the expansion
             int exponant=2; // precision of the exponential
             // ofstream freefemOutput("{file_name}");
+            
+            cout.precision(12);
+            cout << "kopytko ";
             for(int i=0;i<nbTips;++i)
-            {{
+            {
                 // cout << "Processing Tip " << i << " ";   
                 x0=X(i);y0=Y(i);
                 // cout << "(x0, y0) = (" << x0 << ", " <<y0<< "), angle = " << angle(i) << endl;
                 
             	// cout << "Projecting... Th.nv = " << Th.nv;
                 Ph=trunc(Th,(sqrt((x-x0)^2+(y-y0)^2) < 3*R)); 
             	// cout << ", Ph.nv = " << Ph.nv << endl;
             	
-                for(int order=1; order<=a.n; ++order){{ 
+                for(int order=1; order<=a.n; ++order){ 
                     a[order-1]=
                     int2d(Ph)( u*exp(-(sqrt((x-x0)^2 + (y-y0)^2)/R)^exponant)
             		*BaseVector(order,exp(-angle(i)*1i)*( (x-x0) + (y-y0)*1i) ) ) /
                     (int2d(Ph)(exp(-(sqrt((x-x0)^2 + (y-y0)^2)/R)^exponant)
             		*square(BaseVector(order,exp(-angle(i)*1i)*( (x-x0) + (y-y0)*1i) ) )));
             		
             		cout << a[order-1] << ",";
                     // cout << "a(" << order << ") = " << a[order-1] << endl;
-                }}
+                }
             	// freefemOutput << Th.nv << " ";
             	// freefemOutput << Ph.nv << " ";
             	// freefemOutput << adaptCounter << " ";
             	
             	// cout << endl;
-            }};
+            };
             
             // cout << endl << endl << "Building mesh took: " << buildTime; 
             // cout << endl << "First adapt took: " << firstAdaptTime; 
             // cout << endl << "First run took: " << firstRunTime; 
             // cout << endl << "Adaptation took: " << adaptTime; 
             // cout << endl << "Calculating coefficients took: " << clock()- coeffTime0;
             // cout << endl << "Total time: " << clock()-time0 << endl << endl;
@@ -367,18 +371,17 @@
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
         )
         if result.returncode:
             print("\nFreeFem++ failed.\n")
             print("stdout:", result.stdout.decode())
             print("stderr:", result.stderr.decode())
-
-        ai_coeffs_flat = np.fromstring(result.stdout, sep=",")
+            
+        ai_coeffs_flat = np.fromstring(result.stdout[result.stdout.find(b'kopytko')+7:], sep=",")
         self.a1a2a3_coefficients = ai_coeffs_flat.reshape(len(ai_coeffs_flat) // 3, 3)
-        # print(self.a1a2a3_coefficients)
 
         # close temporary files
         for tmp_file in temporary_files:
             tmp_file.close()
             os.unlink(tmp_file.name)
 
     def __run_freefem(self, script):
@@ -398,22 +401,21 @@
         ]
         result = subprocess.run(
             args=cmd,
             stdin=subprocess.PIPE,
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
         )
-        print("stdout:", result.stdout.decode())
-        print("stderr:", result.stderr.decode())
+        # print("stdout:", result.stdout.decode())
+        # print("stderr:", result.stderr.decode())
         if result.returncode:
             print("\nFreeFem++ failed.\n")
 
-        ai_coeffs_flat = np.fromstring(result.stdout, sep=",")
+        ai_coeffs_flat = np.fromstring(result.stdout[result.stdout.find(b'kopytko')+7:], sep=",")
         self.a1a2a3_coefficients = ai_coeffs_flat.reshape(len(ai_coeffs_flat) // 3, 3)
-        # print(self.a1a2a3_coefficients)
 
     def solve_PDE(self, network):
         """Solve the PDE for the field around the network.
 
         Prepare a FreeFEM script, export it to a temporary file and run.
         Then, import the a1a2a3 coefficients to ``self.a1a2a3_coefficients``.
 
@@ -424,10 +426,13 @@
 
         Returns
         -------
         None.
 
         """
         script = self.__prepare_script(network)
-        self.__run_freefem_temp(script)
-        # self.__run_freefem(script) # useful for debugging
-        # print('a1a2a3: ', self.a1a2a3_coefficients)
+        if system() == 'Windows':
+            self.__run_freefem(script) # useful for debugging
+        else:
+            self.__run_freefem_temp(script)
+        # with np.printoptions(formatter={'float': '{:.6e}'.format}):
+            # print('a1a2a3: \n', self.a1a2a3_coefficients)
```

### Comparing `reticuler-1.0/src/reticuler/extending_kernels/trajectory_integrators.py` & `reticuler-1.1/src/reticuler/extending_kernels/trajectory_integrators.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     
         """
         # x[n + 1] = x[n] + dt * v[x(n)]: finding position n+1 with explicit Euler
         dRs_0 = extender.find_test_dRs(network, is_BEA_off)
         
         # in the BEA we want to move over dt as in the backward step,
         # so no normalization
-        a1a2a3_coefficients_0 = extender.pde_solver.a1a2a3_coefficients
+        a1a2a3_coefficients_0 = extender.pde_solver.a1a2a3_coefficients.copy()
             
         # checking if branches are_moving or each branch.is_bifurcating
         are_moving = extender.check_bifurcation_and_moving_conditions(network)
         dRs_0 = dRs_0[are_moving]
         # print('a1, a2, a3:\n',extender.pde_solver.a1a2a3_coefficients)
     
         # moving test_system by dRs_0
@@ -105,14 +105,15 @@
             # v[ x(n+1)] ]: finding velocity at the next point
             dRs_1 = extender.find_test_dRs(test_network, is_BEA_off)
             
             # calculating approximation error and average dR
             epsilon = np.sum(np.linalg.norm(dRs_test - \
                             (dRs_0 + dRs_1) / 2, axis=1)) / len(dRs_0)
             dRs_test = (dRs_0 + dRs_1) / 2
+            # print(dRs_test)
             if is_BEA_off:
                 dRs_test = dRs_test * extender.ds / np.max(np.linalg.norm(dRs_test, axis=1))
                 
             # moving test_system by dR
             test_network = network.copy()
             self.move_test_tips(test_network, dRs_test)
             
@@ -121,10 +122,11 @@
             # normally division dX/a1^eta would give single dt
             # due to the modified Euler's algorithm (dR = (dRs_0+dRs_1)/2 )
             # dt is not perfectly the same for different tips, so we take a mean
             dt = np.mean( np.linalg.norm(dRs_test, axis=1) / extender.pde_solver.a1a2a3_coefficients[...,0]**extender.eta)
         else: 
             dt = extender.ds
         
+        # print('dRs: ', dRs_test)
         extender.assign_dRs(network, dRs_test)
         
         return dt, a1a2a3_coefficients_0
```

### Comparing `reticuler-1.0/src/reticuler/system.py` & `reticuler-1.1/src/reticuler/system.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     ----------
     .. [1] https://stackoverflow.com/questions/26646362/numpy-array-is-not-json-serializable
     """
 
     def default(self, obj):
         if isinstance(obj, np.ndarray):
             return obj.tolist()
-        if isinstance(obj, np.int32): 
+        if isinstance(obj, np.int32) or isinstance(obj, np.int64): 
             return int(obj)
         return json.JSONEncoder.default(self, obj)
 
 
 class Branch:
     """A class of a single branch in a network.
 
@@ -81,20 +81,20 @@
         self.points = np.vstack((self.points, self.points[-1] + self.dR))
 
     def length(self):
         """Return length of the Branch."""
         return np.sum(np.linalg.norm(self.points[1:]-self.points[:-1], axis=1))
 
     def tip_angle(self):
-        """Return the angle between the tip segment (last and penultimate point) and Y axis."""
+        """Return the angle between the tip segment (last and penultimate point) and X axis."""
         point_penult = self.points[-2]
         point_last = self.points[-1]
         dx = point_last[0] - point_penult[0]
         dy = point_last[1] - point_penult[1]
-        return np.pi / 2 - np.arctan2(dy, dx)
+        return np.arctan2(dy, dx)
 
     def points_steps(self):
         """Return a 3-n array of points and evolution steps when they were added."""
         return np.column_stack((self.points, self.steps))
 
 
 class Box:
@@ -116,15 +116,15 @@
         A 2-n array of seeds connectivity.
             - 1st column: index in ``points``
             - 2nd column: outgoing branch ``ID`` 
 
     """
 
     def __init__(
-        self, points, connections, boundary_conditions, seeds_connectivity
+        self, points=None, connections=None, boundary_conditions=None, seeds_connectivity=None
     ):
         """Initialize Box.
 
         Parameters
         ----------
         points : array, default []
         connections : array, default []
@@ -132,40 +132,28 @@
         seeds_connectivity : array, default []
 
         Returns
         -------
         None.
 
         """
-        self.points = points # [] if points is None else points
-        self.connections = connections
-        self.boundary_conditions = boundary_conditions
+        self.points = np.empty((0,2),dtype=float) if points is None else points
+        self.connections = np.empty((0,2),dtype=int) if connections is None else connections
+        self.boundary_conditions = np.empty((0,1),dtype=int) if boundary_conditions is None else boundary_conditions
 
         # 1st column: index on border
         # 2nd column: branch_id
-        self.seeds_connectivity = seeds_connectivity
+        self.seeds_connectivity = [] if seeds_connectivity is None else seeds_connectivity
         
     def __add_points(self, points):
-        if not len(self.points):
-            self.points = points
-        else:
-            self.points = np.vstack((self.points, points))
+        self.points = np.vstack((self.points, points))
 
     def __add_connection(self, connections, boundary_conditions):
-        if not len(self.connections):
-            self.connections = connections
-        else:
-            self.connections = np.vstack((self.connections, connections))
-
-        if not len(self.boundary_conditions):
-            self.boundary_conditions = boundary_conditions
-        else:
-            self.boundary_conditions = np.concatenates(
-                (self.boundary_conditions, boundary_conditions)
-            )
+        self.connections = np.vstack((self.connections, connections))
+        self.boundary_conditions = np.append(self.boundary_conditions, boundary_conditions)
 
     def connections_bc(self):
         """Return a 3-n array of connections and boundary conditions corresponding to them.
         (1st/2nd column - point indices, 3rd column - BC)
         """
         return np.column_stack((self.connections, self.boundary_conditions))
 
@@ -404,21 +392,21 @@
         An object of class Network.
     extender : Extender
         An object of one of the classes from reticuler.extending_kernels.extenders.
     trajectory_integrator : TrajectoryIntegrator
         One of the classes from reticuler.extending_kernels.trajectory_integrators.
     growth_thresh_type : int, default 0
         Type of growth threshold.
-            - 0: number of steps
+            - 0: max step
             - 1: height
             - 2: network length
     growth_thresh : float, default 5
         A value of growth threshold. The simulation is stopped, when it's reached.
     growth_gauges : array, default array([0.,0.,0.])
-        A 1-3 array with growth gauges (number of steps, height, network length).
+        A 1-3 array with growth gauges (max step, height, network length).
     dump_every : int, default 1
         Dumps the results every ``dump_every`` steps.
     exp_name: str, default ''
         Path to a file, where the results will be stored.
 
     """
 
@@ -452,31 +440,31 @@
 
         """
         self.network = network
         self.extender = extender
         self.trajectory_integrator = trajectory_integrator
 
         # Growth limits:
-        # 0: number of steps, 1: max height
-        # 2: max tree length 3: max time
+        # 0: max step, 1: max height
+        # 2: max length 3: max time
         self.growth_gauges = np.zeros(4) if growth_gauges is None else growth_gauges
         self.growth_thresh_type = growth_thresh_type
         self.growth_thresh = growth_thresh
 
         self.dump_every = dump_every
         self.exp_name = exp_name
     
     def copy(self):
         """Return a deepcopy of the Network."""
         return copy.deepcopy(self)
 
     def export_json(self):
         """Export all the information to 'self.exp_name'+'.json'."""
-        growth_type_legend = ["number of steps",
-                              "max height", "max tree length", "max time"]
+        growth_type_legend = ["max step",
+                              "max height", "max length", "max time"]
         export_general = {
             "reticuler_version": importlib.metadata.version("reticuler"),
             "exp_name": self.exp_name,
             "growth": {
                 "threshold_type": growth_type_legend[self.growth_thresh_type],
                 "threshold": self.growth_thresh,
                 "growth_gauges": {
@@ -589,18 +577,18 @@
             branch = Branch(
                 ID=json_branch["ID"],
                 points=points_steps[:, :2],
                 steps=np.array(points_steps[:, 2], dtype=int),
             )
 
             branches.append(branch)
-            if json_branch["state"] == "active":
+            if json_branch["state"] == "active" or json_branch["state"] == "sleeping":
                 active_branches.append(branch)
-            elif json_branch["state"] == "sleeping":
-                sleeping_branches.append(branch)
+            # elif json_branch["state"] == "sleeping":
+            #     sleeping_branches.append(branch)
 
         # Box
         json_box = json_load["network"]["box"]
         connections_bc = np.asarray(json_box["connections_and_bc"])
         box = Box(
             points=np.asarray(json_box["points"]),
             connections=connections_bc[:, :2],
@@ -645,24 +633,24 @@
             extender = extenders.Streamline(
                 pde_solver=pde_solver,
                 eta=json_extender["eta"],
                 ds=json_extender["ds"],
                 bifurcation_type=bifurcation_type,
                 bifurcation_thresh=json_bifurcation["threshold"],
                 bifurcation_angle=json_bifurcation["angle"],
+                inflow_thresh=json_extender["inflow_thresh"],
             )
-            extender.inflow_thresh = json_extender["inflow_thresh"]
             extender.distance_from_bif_thresh = json_extender[
                 "distance_from_bif_thresh"
             ]
 
         # General
         json_growth = json_load["growth"]
-        growth_type_legend = ["number of steps",
-                              "max height", "max tree length", "max time"]
+        growth_type_legend = ["max step",
+                              "max height", "max length", "max time"]
         growth_thresh_type = growth_type_legend.index(
             json_growth["threshold_type"])
         growth_thresh = json_growth["threshold"]
         dump_every = json_growth["dump_every"]
 
         json_growth_gauges = json_growth["growth_gauges"]
         growth_gauges = np.array(
```

### Comparing `reticuler-1.0/src/reticuler/user_interface/clip_ret.py` & `reticuler-1.1/src/reticuler/user_interface/plot_ret.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-"""Command line script to clip a network"""
+"""Command line script to plot a network"""
 
 import argparse
 import json
 import textwrap
 import matplotlib.pyplot as plt
 
 from reticuler.system import System
-from reticuler.user_interface import graphics, clippers
+from reticuler.user_interface import graphics
 
 # %%
 def main():
     parser = argparse.ArgumentParser(
-        description="Clip a network.", formatter_class=argparse.RawTextHelpFormatter
+        description="Plot a network.", formatter_class=argparse.RawTextHelpFormatter
     )
 
     # defining arguments for parser object
     parser.add_argument(
         "input_file",
         type=str,
         nargs=1,
@@ -29,87 +29,102 @@
         "-out",
         "--output_file",
         type=str,
         nargs=1,
         metavar="file_name",
         help=textwrap.dedent(
             """\
-                            File to export. If None the same as input (+"_clipped" at the end).
+                            File to export. If None the same as input.
                             default = None """
         ),
         default=None,
     )
 
-    # Clipping type and limit
     parser.add_argument(
-        "-S",
-        "--step",
+        "-out_ext",
+        "--output_extension",
+        type=str,
+        nargs=1,
+        metavar="ext",
+        help=textwrap.dedent(
+            """\
+                            Output extension ('.pdf', '.svg', '.png', etc.)
+                            default = '.jpg' """
+        ),
+        default=[".jpg"],
+    )
+
+    # Plotting options
+    parser.add_argument(
+        "--ylim",
         type=float,
         nargs=1,
         metavar="num",
         help=textwrap.dedent(
             """\
-                            Maximum step in the network evolution. If filled trips to step.
+                            ylim of the plot. If None ylim=max height of the network.
                             default = None
                             """
         ),
-        default=None,
+        default=[None],
     )
     parser.add_argument(
-        "-L",
-        "--length",
+        "--xlim",
         type=float,
         nargs=1,
         metavar="num",
         help=textwrap.dedent(
             """\
-                            Maximum length of the network. If filled trips to length.
-                            default = None
+                            xlim of the plot.
+                            default = 2
                             """
         ),
-        default=None,
+        default=[2],
     )
     parser.add_argument(
-        "-H",
-        "--height",
-        type=float,
+        "--plot_params",
+        type=json.loads,
         nargs=1,
-        metavar="num",
+        metavar="dict",
         help=textwrap.dedent(
             """\
-                            Maximum height of the network. If filled trips to height.
-                            default = None
+                            Optional plotting parameters.
+                            
+                            Pass dictionary in a form (no spaces, 
+                            backslash before quotes around `value`): 
+                                "{\"value\":key}"
+                            default = {} (keeps default values as listed below)
+                            
                             """
+        )
+        + textwrap.dedent(
+            graphics.plot_tree.__doc__[
+                graphics.plot_tree.__doc__.find("kwargs_plots")
+                - 4 : graphics.plot_tree.__doc__.find("Returns")
+            ]
         ),
-        default=None,
+        default=[{}],
     )
 
     # parse the arguments from standard input
     args = parser.parse_args()
 
     # Import System from JSON file
     system = System.import_json(input_file=args.input_file[0])
 
     fig, ax = plt.subplots()
     graphics.plot_tree(
         ax,
         network=system.network,
+        ylim=args.ylim[0],
+        xlim=args.xlim[0],
+        **args.plot_params[0]
     )
-    
-    if args.step is not None:
-        clippers.clip_to_step(system, args.step)
-    elif args.length is not None:
-        clippers.clip_to_length(system, args.length)
-    elif args.height is not None:
-        clippers.clip_to_height(system, args.height)
-    else:
-        print("Network not clipped - you must choose one clipping limit!")
 
     if args.output_file is None:
-        system.exp_name = args.input_file[0] + "_clipped"
+        fig.savefig(args.input_file[0] + args.output_extension[0], bbox_inches="tight")
     else:
-        system.exp_name = args.output_file[0]
-    system.export_json()
+        fig.savefig(args.output_file[0] + args.output_extension[0], bbox_inches="tight")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `reticuler-1.0/src/reticuler/user_interface/graphics.py` & `reticuler-1.1/src/reticuler/user_interface/graphics.py`

 * *Files identical despite different names*

### Comparing `reticuler-1.0/src/reticuler/user_interface/plot_ret.py` & `reticuler-1.1/src/reticuler/user_interface/clip_ret.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,130 +1,157 @@
-"""Command line script to plot a network"""
+"""Command line script to clip a network"""
 
 import argparse
-import json
 import textwrap
-import matplotlib.pyplot as plt
 
 from reticuler.system import System
-from reticuler.user_interface import graphics
+from reticuler.backward_evolution.system_back import BackwardSystem
+from reticuler.user_interface import clippers
 
 # %%
 def main():
     parser = argparse.ArgumentParser(
-        description="Plot a network.", formatter_class=argparse.RawTextHelpFormatter
+        description="Clip a network.", formatter_class=argparse.RawTextHelpFormatter
     )
 
     # defining arguments for parser object
     parser.add_argument(
         "input_file",
         type=str,
         nargs=1,
         metavar="file_name",
         help=textwrap.dedent(
             """\
                             File to import"""
         ),
-    )
+    )       
     parser.add_argument(
         "-out",
         "--output_file",
         type=str,
         nargs=1,
         metavar="file_name",
         help=textwrap.dedent(
             """\
-                            File to export. If None the same as input.
+                            File to export. If None the same as input (+"_clipped" at the end).
                             default = None """
         ),
         default=None,
     )
-
+        
+    parser.add_argument(
+        "-in_BEA",
+        "--input_file_BEA",
+        type=str,
+        nargs=1,
+        metavar="file_name",
+        help=textwrap.dedent(
+            """\
+                            File with the BEA results to import"""
+        ),
+    ) 
     parser.add_argument(
-        "-out_ext",
-        "--output_extension",
+        "-out_BEA",
+        "--output_file_BEA",
         type=str,
         nargs=1,
-        metavar="ext",
+        metavar="file_name",
         help=textwrap.dedent(
             """\
-                            Output extension ('.pdf', '.svg', '.png', etc.)
-                            default = '.jpg' """
+                            The BEA file to export. If None the same as input (+"_clipped" at the end).
+                            default = None """
         ),
-        default=[".jpg"],
+        default=None,
     )
-
-    # Plotting options
+    # Clipping type and limit
     parser.add_argument(
-        "--ylim",
+        "-S",
+        "--step",
         type=float,
         nargs=1,
         metavar="num",
         help=textwrap.dedent(
             """\
-                            ylim of the plot. If None ylim=max height of the network.
+                            Maximum step in the network evolution. If filled clips to step.
                             default = None
                             """
         ),
-        default=[None],
+        default=None,
     )
     parser.add_argument(
-        "--xlim",
+        "-L",
+        "--length",
         type=float,
         nargs=1,
         metavar="num",
         help=textwrap.dedent(
             """\
-                            xlim of the plot.
-                            default = 2
+                            Maximum length of the network. If filled clips to length.
+                            default = None
                             """
         ),
-        default=[2],
+        default=None,
     )
     parser.add_argument(
-        "--plot_params",
-        type=json.loads,
+        "-H",
+        "--height",
+        type=float,
         nargs=1,
-        metavar="dict",
+        metavar="num",
         help=textwrap.dedent(
             """\
-                            Optional plotting parameters.
-                            
-                            Pass dictionary in a form (no spaces, 
-                            backslash before quotes around `value`): 
-                                "{\"value\":key}"
-                            default = {} (keeps default values as listed below)
-                            
+                            Maximum height of the network. If filled clips to height.
+                            default = None
                             """
-        )
-        + textwrap.dedent(
-            graphics.plot_tree.__doc__[
-                graphics.plot_tree.__doc__.find("kwargs_plots")
-                - 4 : graphics.plot_tree.__doc__.find("Returns")
-            ]
         ),
-        default=[{}],
+        default=None,
     )
+    parser.add_argument(
+        "-BEA",
+        "--BEA_step",
+        type=float,
+        nargs=1,
+        metavar="num",
+        help=textwrap.dedent(
+            """\
+                            Clipping Maximum height of the network. If filled clips to height.
+                            default = None
+                            """
+        ),
+        default=None,
+    )        
 
     # parse the arguments from standard input
     args = parser.parse_args()
 
     # Import System from JSON file
     system = System.import_json(input_file=args.input_file[0])
-
-    fig, ax = plt.subplots()
-    graphics.plot_tree(
-        ax,
-        network=system.network,
-        ylim=args.ylim[0],
-        xlim=args.xlim[0],
-        **args.plot_params[0]
-    )
-
+    
     if args.output_file is None:
-        fig.savefig(args.input_file[0] + args.output_extension[0], bbox_inches="tight")
+        system.exp_name = args.input_file[0] + "_clipped"
     else:
-        fig.savefig(args.output_file[0] + args.output_extension[0], bbox_inches="tight")
+        system.exp_name = args.output_file[0]
+    
+    if args.step is not None:
+        clippers.clip_to_step(system, args.step[0])
+    elif args.length is not None:
+        clippers.clip_to_length(system, args.length[0])
+    elif args.height is not None:
+        clippers.clip_to_height(system, args.height[0])
+    elif args.BEA_step is not None:
+        backward_system = BackwardSystem.import_json(input_file=args.input_file_BEA[0], system=system)
+        clippers.clip_to_BEA_step(system, backward_system, max_BEA_step=args.BEA_step[0])
+        
+        if args.output_file_BEA is None:
+            backward_system.exp_name = args.input_file_BEA[0]+"_clipped"
+        else:
+            backward_system.exp_name = args.output_file_BEA[0]
+              
+        backward_system.export_json()          
+    else:
+        print("Network not clipped - you must choose one clipping limit!")
+
+    system.export_json()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `reticuler-1.0/src/reticuler/user_interface/reticulate.py` & `reticuler-1.1/src/reticuler/user_interface/reticulate.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,16 @@
         "-out",
         "--output_file",
         type=str,
         nargs=1,
         metavar="exp_name",
         help=textwrap.dedent(
             """\
-            File to export.
+            File to export. If we import a file and leave this as default, 
+            `system.exp_name` will be set to `input_file`.
             default = '' """
         ),
         default=[""],
     )
 
     # Growth options
     parser.add_argument(
```

### Comparing `reticuler-1.0/src/reticuler/user_interface/reticulate_back.py` & `reticuler-1.1/src/reticuler/user_interface/reticulate_back.py`

 * *Files 22% similar despite different names*

```diff
@@ -36,18 +36,20 @@
         "-out",
         "--output_file",
         type=str,
         nargs=1,
         metavar="exp_name",
         help=textwrap.dedent(
             """\
-            File to export. 
-            Forward file: `exp_name`+`.json`.
-            BEA results: `exp_name`+`_back.json`
-            default = ``
+            File to export:
+            exp_name = `exp_name`+'_back.json'.
+            If left as default: 
+            exp_name = `input_file`+'_back.json'.
+            
+            default = ''
             """
         ),
         default=[""],
     )
 
     # BEA options
     parser.add_argument(
@@ -109,25 +111,50 @@
                trimmers.BackwardModifiedEulerMethod.__doc__.find("eta")
                 - 4 : trimmers.BackwardModifiedEulerMethod.__doc__.find("References")-6
             ]
         ),
         default=[{}],
     )       
 
+    # Continuation
+    parser.add_argument(
+        "-cont",
+        "--continuation_file",
+        type=str,
+        nargs=1,
+        metavar="file_name",
+        help=textwrap.dedent(
+            """\
+            Continuation of the previously commenced BEA.
+            System will be imported from `input_file` and backward system from 
+            `continuation_file`+'.json'.
+            """
+        ),
+        default=[""],
+    )
+    
     # parse the arguments from standard input
     args = parser.parse_args()
-
+    
     # Import System from JSON file
     system = System.import_json(input_file=args.input_file[0])
-    system.exp_name = args.output_file[0]
-
-    # Trimmer
-    if args.trimmer[0] == "BackwardModifiedEulerMethod":
-        trimmer = trimmers.BackwardModifiedEulerMethod(system.extender.pde_solver, **args.trimmer_params[0])
-        trimmer.eta = args.eta[0]
-    # General
-    backward_system = BackwardSystem(system, trimmer)
-    
+    if args.output_file[0]!="":
+        system.exp_name = args.output_file[0]
+    else:
+        system.exp_name = args.input_file[0]
+
+    # Create or import BackwardSystem
+    if args.continuation_file[0]!="":
+        backward_system = BackwardSystem.import_json(input_file=args.continuation_file[0], system=system)
+        backward_system.exp_name = backward_system.exp_name + "_cont"
+    else:
+        # Trimmer
+        if args.trimmer[0] == "BackwardModifiedEulerMethod":
+            trimmer = trimmers.BackwardModifiedEulerMethod(system.extender.pde_solver, **args.trimmer_params[0])
+        # All
+        backward_system = BackwardSystem(system, trimmer)
+        
+    # Running BEA
     backward_system.run_BEA()
 
 if __name__ == "__main__":
     main()
```

### Comparing `reticuler-1.0/src/reticuler.egg-info/SOURCES.txt` & `reticuler-1.1/src/reticuler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

