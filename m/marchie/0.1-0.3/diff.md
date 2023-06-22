# Comparing `tmp/marchie-0.1.tar.gz` & `tmp/marchie-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marchie-0.1.tar", last modified: Thu Jun 22 08:45:18 2023, max compression
+gzip compressed data, was "marchie-0.3.tar", last modified: Thu Jun 22 09:07:51 2023, max compression
```

## Comparing `marchie-0.1.tar` & `marchie-0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 maxschmaltz   (501) staff       (20)        0 2023-06-22 08:45:18.426775 marchie-0.1/
--rw-r--r--   0 maxschmaltz   (501) staff       (20)    11356 2023-06-21 19:22:24.000000 marchie-0.1/LICENSE
--rw-r--r--   0 maxschmaltz   (501) staff       (20)     6722 2023-06-22 08:45:18.426535 marchie-0.1/PKG-INFO
--rw-r--r--   0 maxschmaltz   (501) staff       (20)     5838 2023-06-22 08:44:46.000000 marchie-0.1/README.md
-drwxr-xr-x   0 maxschmaltz   (501) staff       (20)        0 2023-06-22 08:45:18.424503 marchie-0.1/marchie/
--rw-r--r--   0 maxschmaltz   (501) staff       (20)     1877 2023-06-22 08:17:43.000000 marchie-0.1/marchie/__init__.py
--rw-r--r--   0 maxschmaltz   (501) staff       (20)    21932 2023-06-21 23:03:23.000000 marchie-0.1/marchie/end_behavior.py
--rw-r--r--   0 maxschmaltz   (501) staff       (20)    66511 2023-06-22 08:38:26.000000 marchie-0.1/marchie/marchie.py
--rw-r--r--   0 maxschmaltz   (501) staff       (20)    12275 2023-06-21 19:09:49.000000 marchie-0.1/marchie/structure.py
-drwxr-xr-x   0 maxschmaltz   (501) staff       (20)        0 2023-06-22 08:45:18.425711 marchie-0.1/marchie.egg-info/
--rw-r--r--   0 maxschmaltz   (501) staff       (20)     6722 2023-06-22 08:45:18.000000 marchie-0.1/marchie.egg-info/PKG-INFO
--rw-r--r--   0 maxschmaltz   (501) staff       (20)      278 2023-06-22 08:45:18.000000 marchie-0.1/marchie.egg-info/SOURCES.txt
--rw-r--r--   0 maxschmaltz   (501) staff       (20)        1 2023-06-22 08:45:18.000000 marchie-0.1/marchie.egg-info/dependency_links.txt
--rw-r--r--   0 maxschmaltz   (501) staff       (20)       15 2023-06-22 08:45:18.000000 marchie-0.1/marchie.egg-info/requires.txt
--rw-r--r--   0 maxschmaltz   (501) staff       (20)        8 2023-06-22 08:45:18.000000 marchie-0.1/marchie.egg-info/top_level.txt
--rw-r--r--   0 maxschmaltz   (501) staff       (20)       38 2023-06-22 08:45:18.426846 marchie-0.1/setup.cfg
--rw-r--r--   0 maxschmaltz   (501) staff       (20)     1238 2023-06-22 08:44:51.000000 marchie-0.1/setup.py
-drwxr-xr-x   0 maxschmaltz   (501) staff       (20)        0 2023-06-22 08:45:18.425975 marchie-0.1/tests/
--rw-r--r--   0 maxschmaltz   (501) staff       (20)    53045 2023-06-22 08:17:58.000000 marchie-0.1/tests/test.py
+drwxr-xr-x   0 maxschmaltz   (501) staff       (20)        0 2023-06-22 09:07:51.708512 marchie-0.3/
+-rw-r--r--   0 maxschmaltz   (501) staff       (20)    11356 2023-06-21 19:22:24.000000 marchie-0.3/LICENSE
+-rw-r--r--   0 maxschmaltz   (501) staff       (20)     6720 2023-06-22 09:07:51.708304 marchie-0.3/PKG-INFO
+-rw-r--r--   0 maxschmaltz   (501) staff       (20)     5836 2023-06-22 09:07:20.000000 marchie-0.3/README.md
+drwxr-xr-x   0 maxschmaltz   (501) staff       (20)        0 2023-06-22 09:07:51.706408 marchie-0.3/marchie/
+-rw-r--r--   0 maxschmaltz   (501) staff       (20)     1877 2023-06-22 08:17:43.000000 marchie-0.3/marchie/__init__.py
+-rw-r--r--   0 maxschmaltz   (501) staff       (20)    21932 2023-06-21 23:03:23.000000 marchie-0.3/marchie/end_behavior.py
+-rw-r--r--   0 maxschmaltz   (501) staff       (20)    66545 2023-06-22 08:59:56.000000 marchie-0.3/marchie/marchie.py
+-rw-r--r--   0 maxschmaltz   (501) staff       (20)    12275 2023-06-21 19:09:49.000000 marchie-0.3/marchie/structure.py
+drwxr-xr-x   0 maxschmaltz   (501) staff       (20)        0 2023-06-22 09:07:51.707574 marchie-0.3/marchie.egg-info/
+-rw-r--r--   0 maxschmaltz   (501) staff       (20)     6720 2023-06-22 09:07:51.000000 marchie-0.3/marchie.egg-info/PKG-INFO
+-rw-r--r--   0 maxschmaltz   (501) staff       (20)      278 2023-06-22 09:07:51.000000 marchie-0.3/marchie.egg-info/SOURCES.txt
+-rw-r--r--   0 maxschmaltz   (501) staff       (20)        1 2023-06-22 09:07:51.000000 marchie-0.3/marchie.egg-info/dependency_links.txt
+-rw-r--r--   0 maxschmaltz   (501) staff       (20)       15 2023-06-22 09:07:51.000000 marchie-0.3/marchie.egg-info/requires.txt
+-rw-r--r--   0 maxschmaltz   (501) staff       (20)        8 2023-06-22 09:07:51.000000 marchie-0.3/marchie.egg-info/top_level.txt
+-rw-r--r--   0 maxschmaltz   (501) staff       (20)       38 2023-06-22 09:07:51.708573 marchie-0.3/setup.cfg
+-rw-r--r--   0 maxschmaltz   (501) staff       (20)     1238 2023-06-22 09:06:56.000000 marchie-0.3/setup.py
+drwxr-xr-x   0 maxschmaltz   (501) staff       (20)        0 2023-06-22 09:07:51.707807 marchie-0.3/tests/
+-rw-r--r--   0 maxschmaltz   (501) staff       (20)    53045 2023-06-22 08:17:58.000000 marchie-0.3/tests/test.py
```

### Comparing `marchie-0.1/LICENSE` & `marchie-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `marchie-0.1/PKG-INFO` & `marchie-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marchie
-Version: 0.1
+Version: 0.3
 Summary: MarChie: a Compact Open Source Tool for Analyzing Discrete Markov Chains.
 Home-page: https://github.com/maxschmaltz/MarChie
 Author: Max Schmaltz
 Author-email: schmaltzmax@gmail.com
 License: Apache Software License
 Keywords: markov chain,mathematics
 Classifier: Development Status :: 4 - Beta
@@ -18,18 +18,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MarChie: a Compact Open Source Tool for Analyzing Discrete **Mar**kov **Ch**ains
 
-[![Generic badge](https://img.shields.io/badge/PyPI-0.1-green.svg)](https://pypi.org/project/MarChie/)
-[![Generic badge](https://img.shields.io/badge/GitHub-Source-red.svg)](https://github.com/maxschmaltz/MarChie)
-[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)
-[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
+[![Generic badge](https://img.shields.io/badge/PyPI-0.3-green.svg)](https://pypi.org/project/MarChie/) [![Generic badge](https://img.shields.io/badge/GitHub-Source-red.svg)](https://github.com/maxschmaltz/MarChie) [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0) [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
 
 
 ----------
 
 ### Contents:
 
 * [Intro](#intro)
@@ -88,26 +85,26 @@
 * defines properties of the chain;
 * classifies the chain (based on the properties);
 * defines end behavior of the chain (based on the classification).
 
 
 ## Quick Start
 
-`March` is a `pip`-installable package. You can access it directly from PyPI:
+`Marchie` is a `pip`-installable package. You can access it directly from PyPI:
 
 ```bash
-pip install MarChie
+pip install marchie
 ```
 
-The main object that is really intended to be used is `class marchie.marchie.March`. The class requires only transition probability matrix and (optionally) initial state probability distribution vector as arguments; if you provide no initial distribution vector, it will be generated.
+The main object that is really intended to be used is `class marchie.marchie.Marchie`. The class requires only transition probability matrix and (optionally) initial state probability distribution vector as arguments; if you provide no initial distribution vector, it will be generated.
 
 ```python
 
 >>> import numpy as np
->>> from marchie.marchie import March
+>>> from marchie import Marchie
 
 >>> trans_mat = np.array([
     [1,     0,     0  ],
     [0.8,   0.2,   0  ],
     [0.3,   0.5,   0.2]
 ])
 >>> init_distr = np.array(
```

### Comparing `marchie-0.1/README.md` & `marchie-0.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 # MarChie: a Compact Open Source Tool for Analyzing Discrete **Mar**kov **Ch**ains
 
-[![Generic badge](https://img.shields.io/badge/PyPI-0.1-green.svg)](https://pypi.org/project/MarChie/)
-[![Generic badge](https://img.shields.io/badge/GitHub-Source-red.svg)](https://github.com/maxschmaltz/MarChie)
-[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)
-[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
+[![Generic badge](https://img.shields.io/badge/PyPI-0.3-green.svg)](https://pypi.org/project/MarChie/) [![Generic badge](https://img.shields.io/badge/GitHub-Source-red.svg)](https://github.com/maxschmaltz/MarChie) [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0) [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
 
 
 ----------
 
 ### Contents:
 
 * [Intro](#intro)
@@ -66,26 +63,26 @@
 * defines properties of the chain;
 * classifies the chain (based on the properties);
 * defines end behavior of the chain (based on the classification).
 
 
 ## Quick Start
 
-`March` is a `pip`-installable package. You can access it directly from PyPI:
+`Marchie` is a `pip`-installable package. You can access it directly from PyPI:
 
 ```bash
-pip install MarChie
+pip install marchie
 ```
 
-The main object that is really intended to be used is `class marchie.marchie.March`. The class requires only transition probability matrix and (optionally) initial state probability distribution vector as arguments; if you provide no initial distribution vector, it will be generated.
+The main object that is really intended to be used is `class marchie.marchie.Marchie`. The class requires only transition probability matrix and (optionally) initial state probability distribution vector as arguments; if you provide no initial distribution vector, it will be generated.
 
 ```python
 
 >>> import numpy as np
->>> from marchie.marchie import March
+>>> from marchie import Marchie
 
 >>> trans_mat = np.array([
     [1,     0,     0  ],
     [0.8,   0.2,   0  ],
     [0.3,   0.5,   0.2]
 ])
 >>> init_distr = np.array(
```

### Comparing `marchie-0.1/marchie/__init__.py` & `marchie-0.3/marchie/__init__.py`

 * *Files identical despite different names*

### Comparing `marchie-0.1/marchie/end_behavior.py` & `marchie-0.3/marchie/end_behavior.py`

 * *Files identical despite different names*

### Comparing `marchie-0.1/marchie/marchie.py` & `marchie-0.3/marchie/marchie.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,40 +156,40 @@
     '''
     ### Initial state distribution vector.
     Vector \(\pi = (\pi_0, \pi_1, ..., \pi_n)\), where \(n\) is the number 
     of states in the system, and \(\pi_i\) is the probability that the system starts in the state \(i\).
 
     Returns
     -------
-    init_distr : `March._matrix` of shape (`n_states`, )
+    init_distr : `Marchie._matrix` of shape (`n_states`, )
         distribution vector
     '''
 
     trans_mat: _matrix
     '''
     ### Transition probability matrix
     Matrix \(P = (p_{ij})\) where \(p_{ij}\) is the probability to go
     to the state \(j\) from the state \(i\) in one step.
 
     Returns
     -------
-    trans_mat : `March._matrix` of shape (`n_states`, `n_states`)
+    trans_mat : `Marchie._matrix` of shape (`n_states`, `n_states`)
         transition matrix
     '''
 
     adjacency_mat: _matrix
     '''
     ### Adjacency matrix of the chain.
     Adjacency matrix is a matrix that indicates existence of one-step paths between states,
     where a one-step path from the state \(i\) to the state \(j\) exists 
     if there a non-zero probability transition between them.
 
     Returns
     -------
-    adjacency_mat : `March._matrix` of shape (`n_states`, `n_states`)
+    adjacency_mat : `Marchie._matrix` of shape (`n_states`, `n_states`)
         boolean-like matrix indicating one-step paths between states,
         where `adjacency_mat[i, j]` is \(1\) if the probability of tranition 
         from the state `i` to the state `j` is not zero, else \(0\)
 
     Notes
     -----
     Adjacency matrix is calculated as shown below:
@@ -211,15 +211,15 @@
     Reachability matrix is a matrix that indicates existence of paths between states,
     where a path from the state \(i\) to the state \(j\) exists if there a sequence 
     of non-zero probability transitions between states such that it leads from \(i\) to \(j\)
     (e.g. \(i\) → \(h\) → \(k\) → ... → \(j\)).
 
     Returns
     -------
-    reachability_mat : `March._matrix` of shape (`n_states`, `n_states`)
+    reachability_mat : `Marchie._matrix` of shape (`n_states`, `n_states`)
         boolean-like matrix indicating paths between states,
         where `reachability_mat[i, j]` is \(1\) if there is a path 
         from the state `i` to the state `j`, else \(0\)
 
     Notes
     -----
     Reachability matrix is calculated as shown below:
@@ -241,15 +241,15 @@
     Reachability matrix is a matrix that indicates existence of inverse paths between states,
     where a path from the state \(i\) to the state \(j\) exists if there a sequence 
     of non-zero probability transitions between states such that it leads from \(i\) to \(j\)
     (e.g. \(i\) → \(h\) → \(k\) → ... → \(j\)).
 
     Returns
     -------
-    reachability_mat_tr : `March._matrix` of shape (`n_states`, `n_states`)
+    reachability_mat_tr : `Marchie._matrix` of shape (`n_states`, `n_states`)
         boolean-like matrix indicating paths between states,
         where `reachability_mat_tr[i, j]` is \(1\) if there is a path 
         from the state `j` to the state `i`, else \(0\)
 
     Notes
     -----
     Transposed reachability matrix is calculated as shown below:
@@ -271,15 +271,15 @@
     Communication matrix is a matrix that indicates existence of bidirectional paths between states,
     where a bidirectional path between the states \(i\) and \(j\) exists if there a sequence 
     of non-zero probability transitions from \(i\) to \(j\) (e.g. \(i\) → \(h\) → \(k\) → ... → \(j\))
     and from \(j\) to \(i\) (not exactly the same way back).
 
     Returns
     -------
-    communication_mat : `March._matrix` of shape (`n_states`, `n_states`)
+    communication_mat : `Marchie._matrix` of shape (`n_states`, `n_states`)
         boolean-like matrix indicating bidirectional paths between states,
         where `communication_mat[i, j]` is \(1\) if there is a path 
         from the state `j` to the state `i` and from `j` to `i`, else \(0\)
 
     Notes
     -----
     Communication matrix is calculated as shown below:
@@ -302,15 +302,15 @@
     Communication matrix complement is a matrix that indicates nonexistence of bidirectional paths between states,
     where a bidirectional path between the states \(i\) and \(j\) exists if there a sequence 
     of non-zero probability transitions from \(i\) to \(j\) (e.g. \(i\) → \(h\) → \(k\) → ... → \(j\))
     and from \(j\) to \(i\) (not exactly the same way back).
 
     Returns
     -------
-    communication_mat_comp : `March._matrix` of shape (`n_states`, `n_states`)
+    communication_mat_comp : `Marchie._matrix` of shape (`n_states`, `n_states`)
         boolean-like matrix indicating absence of bidirectional paths between states,
         where `communication_mat[i, j]` is \(1\) if there is no path 
         from the state `j` to the state `i` and from `j` to `i`, else 0
 
     Notes
     -----
     Communication matrix complement is calculated as follows:
@@ -329,15 +329,15 @@
     classification_mat: _matrix
     '''
     ### Classification matrix of the chain.
     Classification matrix is a step for building extended classification matrix.
 
     Returns
     -------
-    classification_mat : `March._matrix` of shape (`n_states`, `n_states`)
+    classification_mat : `Marchie._matrix` of shape (`n_states`, `n_states`)
         boolean-like matrix where `classification_mat[i, j]` is \(1\) if there is a path 
         from the state `i` to the state `j` but states `j` and `i` do not communicate, 0 otherwise
 
     Notes
     -----
     Classification matrix is calculated as follows:
 
@@ -358,15 +358,15 @@
     ### Classification matrix extension. 
     Classification matrix extension indicates essential and inessential states.
     Essential states are the ones that communicate with each (!) state they have a path to;
     respectively, the ineccential are the ones for which this statement is not true.
 
     Returns
     -------
-    classification_mat_ext : `March._matrix` of shape (`n_states`, `n_states` + 1)
+    classification_mat_ext : `Marchie._matrix` of shape (`n_states`, `n_states` + 1)
         boolean-like matrix where the last column indicates essentiality of states:
         if classification_mat_ext[`i`, `n_states` + 1] equals 1, the state `i`
         is inessential, if 0, is essential
 
     Notes
     -----
     Classification matrix extention is defined below:
@@ -385,15 +385,15 @@
 
     equivalency_cls_mat: _matrix
     '''
     ### Equivalency matrix of the chain.
 
     Returns
     -------
-    equivalency_cls_mat : `March._matrix` of shape (`n_classes`, `n_essential`)
+    equivalency_cls_mat : `Marchie._matrix` of shape (`n_classes`, `n_essential`)
         matrix showing belonging of each essential (!) state to its equivalence class;
         `equivalency_cls_mat[i, j]` indicates that the state `j` is in `i`th equivalence class
 
     Notes
     -----
     Matrix of equivalency classes is defined as follows:
 
@@ -1079,15 +1079,15 @@
         ### Builds adjacency matrix of the chain.
         Adjacency matrix is a matrix that indicates existence of one-step paths between states,
         where a one-step path from the state \(i\) to the state \(j\) exists 
         if there a non-zero probability transition between them.
 
         Returns
         -------
-        adjacency_mat : `March._matrix` of shape (`n_states`, `n_states`)
+        adjacency_mat : `Marchie._matrix` of shape (`n_states`, `n_states`)
             boolean-like matrix indicating one-step paths between states,
             where `adjacency_mat[i, j]` is \(1\) if the probability of tranition 
             from the state `i` to the state `j` is not zero, else \(0\)
 
         Notes
         -----
         Adjacency matrix is calculated as shown below:
@@ -1114,15 +1114,15 @@
         Reachability matrix is a matrix that indicates existence of paths between states,
         where a path from the state \(i\) to the state \(j\) exists if there a sequence 
         of non-zero probability transitions between states such that it leads from \(i\) to \(j\)
         (e.g. \(i\) → \(h\) → \(k\) → ... → \(j\)).
 
         Returns
         -------
-        reachability_mat : `March._matrix` of shape (`n_states`, `n_states`)
+        reachability_mat : `Marchie._matrix` of shape (`n_states`, `n_states`)
             boolean-like matrix indicating paths between states,
             where `reachability_mat[i, j]` is \(1\) if there is a path 
             from the state `i` to the state `j`, else \(0\)
 
         Notes
         -----
         Reachability matrix is calculated as shown below:
@@ -1156,15 +1156,15 @@
         Reachability matrix is a matrix that indicates existence of inverse paths between states,
         where a path from the state \(i\) to the state \(j\) exists if there a sequence 
         of non-zero probability transitions between states such that it leads from \(i\) to \(j\)
         (e.g. \(i\) → \(h\) → \(k\) → ... → \(j\)).
 
         Returns
         -------
-        reachability_mat_tr : `March._matrix` of shape (`n_states`, `n_states`)
+        reachability_mat_tr : `Marchie._matrix` of shape (`n_states`, `n_states`)
             boolean-like matrix indicating paths between states,
             where `reachability_mat_tr[i, j]` is \(1\) if there is a path 
             from the state `j` to the state `i`, else \(0\)
 
         Notes
         -----
         Transposed reachability matrix is calculated as shown below:
@@ -1190,15 +1190,15 @@
         Communication matrix is a matrix that indicates existence of bidirectional paths between states,
         where a bidirectional path between the states \(i\) and \(j\) exists if there a sequence 
         of non-zero probability transitions from \(i\) to \(j\) (e.g. \(i\) → \(h\) → \(k\) → ... → \(j\))
         and from \(j\) to \(i\) (not exactly the same way back).
 
         Returns
         -------
-        communication_mat : `March._matrix` of shape (`n_states`, `n_states`)
+        communication_mat : `Marchie._matrix` of shape (`n_states`, `n_states`)
             boolean-like matrix indicating bidirectional paths between states,
             where `communication_mat[i, j]` is \(1\) if there is a path 
             from the state `j` to the state `i` and from `j` to `i`, else \(0\)
 
         Notes
         -----
         Communication matrix is calculated as shown below:
@@ -1225,15 +1225,15 @@
         Communication matrix complement is a matrix that indicates nonexistence of bidirectional paths between states,
         where a bidirectional path between the states \(i\) and \(j\) exists if there a sequence 
         of non-zero probability transitions from \(i\) to \(j\) (e.g. \(i\) → \(h\) → \(k\) → ... → \(j\))
         and from \(j\) to \(i\) (not exactly the same way back).
 
         Returns
         -------
-        communication_mat_comp : `March._matrix` of shape (`n_states`, `n_states`)
+        communication_mat_comp : `Marchie._matrix` of shape (`n_states`, `n_states`)
             boolean-like matrix indicating absence of bidirectional paths between states,
             where `communication_mat[i, j]` is \(1\) if there is no path 
             from the state `j` to the state `i` and from `j` to `i`, else 0
 
         Notes
         -----
         Communication matrix complement is calculated as follows:
@@ -1257,15 +1257,15 @@
 
         '''
         ### Builds classification matrix. 
         Classification matrix is a step for building extended classification matrix.
 
         Returns
         -------
-        classification_mat : `March._matrix` of shape (`n_states`, `n_states`)
+        classification_mat : `Marchie._matrix` of shape (`n_states`, `n_states`)
             boolean-like matrix where `classification_mat[i, j]` is \(1\) if there is a path 
             from the state `i` to the state `j` but states `j` and `i` do not communicate, 0 otherwise
 
         Notes
         -----
         Classification matrix is calculated as follows:
 
@@ -1290,15 +1290,15 @@
         ### Builds classification matrix extension. 
         Classification matrix extension indicates essential and inessential states.
         Essential states are the ones that communicate with each (!) state they have a path to;
         respectively, the ineccential are the ones for which this statement is not true.
 
         Returns
         -------
-        classification_mat_ext : `March._matrix` of shape (`n_states`, `n_states` + 1)
+        classification_mat_ext : `Marchie._matrix` of shape (`n_states`, `n_states` + 1)
             boolean-like matrix where the last column indicates essentiality of states:
             if classification_mat_ext[`i`, `n_states` + 1] equals 1, the state `i`
             is inessential, if 0, is essential
 
         Notes
         -----
         Classification matrix extention is defined below:
```

### Comparing `marchie-0.1/marchie/structure.py` & `marchie-0.3/marchie/structure.py`

 * *Files identical despite different names*

### Comparing `marchie-0.1/marchie.egg-info/PKG-INFO` & `marchie-0.3/marchie.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marchie
-Version: 0.1
+Version: 0.3
 Summary: MarChie: a Compact Open Source Tool for Analyzing Discrete Markov Chains.
 Home-page: https://github.com/maxschmaltz/MarChie
 Author: Max Schmaltz
 Author-email: schmaltzmax@gmail.com
 License: Apache Software License
 Keywords: markov chain,mathematics
 Classifier: Development Status :: 4 - Beta
@@ -18,18 +18,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MarChie: a Compact Open Source Tool for Analyzing Discrete **Mar**kov **Ch**ains
 
-[![Generic badge](https://img.shields.io/badge/PyPI-0.1-green.svg)](https://pypi.org/project/MarChie/)
-[![Generic badge](https://img.shields.io/badge/GitHub-Source-red.svg)](https://github.com/maxschmaltz/MarChie)
-[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)
-[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
+[![Generic badge](https://img.shields.io/badge/PyPI-0.3-green.svg)](https://pypi.org/project/MarChie/) [![Generic badge](https://img.shields.io/badge/GitHub-Source-red.svg)](https://github.com/maxschmaltz/MarChie) [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0) [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
 
 
 ----------
 
 ### Contents:
 
 * [Intro](#intro)
@@ -88,26 +85,26 @@
 * defines properties of the chain;
 * classifies the chain (based on the properties);
 * defines end behavior of the chain (based on the classification).
 
 
 ## Quick Start
 
-`March` is a `pip`-installable package. You can access it directly from PyPI:
+`Marchie` is a `pip`-installable package. You can access it directly from PyPI:
 
 ```bash
-pip install MarChie
+pip install marchie
 ```
 
-The main object that is really intended to be used is `class marchie.marchie.March`. The class requires only transition probability matrix and (optionally) initial state probability distribution vector as arguments; if you provide no initial distribution vector, it will be generated.
+The main object that is really intended to be used is `class marchie.marchie.Marchie`. The class requires only transition probability matrix and (optionally) initial state probability distribution vector as arguments; if you provide no initial distribution vector, it will be generated.
 
 ```python
 
 >>> import numpy as np
->>> from marchie.marchie import March
+>>> from marchie import Marchie
 
 >>> trans_mat = np.array([
     [1,     0,     0  ],
     [0.8,   0.2,   0  ],
     [0.3,   0.5,   0.2]
 ])
 >>> init_distr = np.array(
```

### Comparing `marchie-0.1/setup.py` & `marchie-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 desc = '''
     MarChie: a Compact Open Source Tool for Analyzing Discrete Markov Chains.
     '''
 with open('./README.md') as readme: long_description = readme.read()
 
 setuptools.setup(
     name='marchie',
-    version='0.1',
+    version='0.3',
     author='Max Schmaltz',
     author_email='schmaltzmax@gmail.com',
     description=desc,
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/maxschmaltz/MarChie',
     # packages=[
```

### Comparing `marchie-0.1/tests/test.py` & `marchie-0.3/tests/test.py`

 * *Files identical despite different names*

