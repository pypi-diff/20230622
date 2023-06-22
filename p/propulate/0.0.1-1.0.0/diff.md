# Comparing `tmp/propulate-0.0.1.tar.gz` & `tmp/propulate-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "propulate-0.0.1.tar", last modified: Thu Sep 22 13:52:33 2022, max compression
+gzip compressed data, was "propulate-1.0.0.tar", last modified: Thu Jun 22 14:52:41 2023, max compression
```

## Comparing `propulate-0.0.1.tar` & `propulate-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 13:52:33.108970 propulate-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-09-22 13:52:23.000000 propulate-0.0.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1563 2022-09-22 13:52:23.000000 propulate-0.0.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)     2676 2022-09-22 13:52:33.108970 propulate-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2190 2022-09-22 13:52:23.000000 propulate-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 13:52:33.108970 propulate-0.0.1/propulate/
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-09-22 13:52:23.000000 propulate-0.0.1/propulate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-09-22 13:52:23.000000 propulate-0.0.1/propulate/_globals.py
--rw-r--r--   0 runner    (1001) docker     (121)     2682 2022-09-22 13:52:23.000000 propulate-0.0.1/propulate/population.py
--rw-r--r--   0 runner    (1001) docker     (121)    27182 2022-09-22 13:52:23.000000 propulate-0.0.1/propulate/propagators.py
--rw-r--r--   0 runner    (1001) docker     (121)    67915 2022-09-22 13:52:23.000000 propulate-0.0.1/propulate/propulator.py
--rw-r--r--   0 runner    (1001) docker     (121)     3180 2022-09-22 13:52:23.000000 propulate-0.0.1/propulate/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    10575 2022-09-22 13:52:23.000000 propulate-0.0.1/propulate/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 13:52:33.108970 propulate-0.0.1/propulate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2676 2022-09-22 13:52:33.000000 propulate-0.0.1/propulate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      418 2022-09-22 13:52:33.000000 propulate-0.0.1/propulate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-22 13:52:33.000000 propulate-0.0.1/propulate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-22 13:52:32.000000 propulate-0.0.1/propulate.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      122 2022-09-22 13:52:33.000000 propulate-0.0.1/propulate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-09-22 13:52:33.000000 propulate-0.0.1/propulate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1256 2022-09-22 13:52:33.108970 propulate-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      381 2022-09-22 13:52:23.000000 propulate-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:52:41.641328 propulate-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-22 14:52:32.000000 propulate-1.0.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-06-22 14:52:32.000000 propulate-1.0.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-06-22 14:52:41.641328 propulate-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-06-22 14:52:32.000000 propulate-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:52:41.637328 propulate-1.0.0/propulate/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-22 14:52:32.000000 propulate-1.0.0/propulate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-22 14:52:32.000000 propulate-1.0.0/propulate/_globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10164 2023-06-22 14:52:32.000000 propulate-1.0.0/propulate/islands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32944 2023-06-22 14:52:32.000000 propulate-1.0.0/propulate/pollinator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-06-22 14:52:32.000000 propulate-1.0.0/propulate/population.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26605 2023-06-22 14:52:32.000000 propulate-1.0.0/propulate/propagators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33894 2023-06-22 14:52:32.000000 propulate-1.0.0/propulate/propulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-22 14:52:32.000000 propulate-1.0.0/propulate/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:52:41.641328 propulate-1.0.0/propulate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-06-22 14:52:41.000000 propulate-1.0.0/propulate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-22 14:52:41.000000 propulate-1.0.0/propulate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 14:52:41.000000 propulate-1.0.0/propulate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 14:52:41.000000 propulate-1.0.0/propulate.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-22 14:52:41.000000 propulate-1.0.0/propulate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-22 14:52:41.000000 propulate-1.0.0/propulate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-22 14:52:41.641328 propulate-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-22 14:52:32.000000 propulate-1.0.0/setup.py
```

### Comparing `propulate-0.0.1/LICENSE.md` & `propulate-1.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `propulate-0.0.1/PKG-INFO` & `propulate-1.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 Metadata-Version: 2.1
 Name: propulate
-Version: 0.0.1
+Version: 1.0.0
 Summary: Massively parallel genetic optimization through asynchronous propagation of populations
 Author: Oskar Taubert, Marie Weiel, Helmholtz AI
 Author-email: oskar.taubert@kit.edu, marie.weiel@kit.edu
 License: mit
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: testing
 License-File: LICENSE.md
-License-File: AUTHORS.rst
+License-File: AUTHORS.md
 
 ![Propulate Logo](./LOGO.svg)
 
 # Parallel Propagator of Populations
 ## Project Status
 [![License: BSD-3](https://img.shields.io/badge/License-BSD--3-blue)](https://opensource.org/licenses/BSD-3-Clause)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/propulate)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-``Propulate`` is a massively parallel evolutionary hyperparameter optimizer based on the island model with asynchronous propagation of populations and asynchronous migration. 
-In contrast to classical GAs, ``Propulate`` maintains a continuous population of already evaluated individuals with a softened notion of the typically strictly separated, discrete generations. 
+``Propulate`` is a massively parallel evolutionary hyperparameter optimizer based on the island model with asynchronous propagation of populations and asynchronous migration.
+In contrast to classical GAs, ``Propulate`` maintains a continuous population of already evaluated individuals with a softened notion of the typically strictly separated, discrete generations.
 Our contributions include:
-- A novel parallel genetic algorithm based on a fully asynchronized island model with independently processing workers. 
+- A novel parallel genetic algorithm based on a fully asynchronized island model with independently processing workers.
 - Massive parallelism by asynchronous propagation of continuous populations and migration via efficient communication using the message passing interface.
 - Optimized use efficiency of parallel hardware by minimizing idle times in distributed computing environments.
 
 To be more efficient, the generations are less well separated than they usually are in evolutionary algorithms.
-New individuals are generated from a pool of currently active, already evaluated individuals that may be from any generation. 
+New individuals are generated from a pool of currently active, already evaluated individuals that may be from any generation.
 Individuals may be removed from the breeding population based on different criteria.
 
+You can find the corresponding publication here:  
+Taubert, O. *et al.* (2023). Massively Parallel Genetic Optimization Through Asynchronous Propagation of Populations. In: Bhatele, A., Hammond, J., Baboulin, M., Kruse, C. (eds) High Performance Computing. ISC High Performance 2023. Lecture Notes in Computer Science, vol 13948. Springer, Cham. [https://doi.org/10.1007/978-3-031-32041-5_6](https://doi.org/10.1007/978-3-031-32041-5_6)
+
 ## Documentation
 
 For usage example, see scripts.
 
 ## Installation
 
-Pull and run ``pip install -e .`` or ``python setup.py develop``.
+From PyPI: ``pip install propulate``  
+Alternatively, pull and run ``pip install -e .`` or ``python setup.py develop``.  
 Requires an MPI implementation (currently only tested with OpenMPI) and ``mpi4py``.
 
-## To Dos
-
-- weight/parameter succession from parents or hall of fame
-- more algorithms and operators, covariance matrix adaptation evolution strategy
-
 ## Acknowledgments
 *This work is supported by the Helmholtz AI platform grant.*
 <div align="center"; style="position:absolute;top:50%;left:50%;">
   <a href="http://www.kit.edu/english/index.php"><img src=./.figs/logo_KIT.svg height="50px" hspace="5%" vspace="0px"></a><a href="https://www.helmholtz.ai"><img src=./.figs/logo_HelmholtzAI.svg height="25px" hspace="5%" vspace="0px"></a>
 </div>
```

#### html2text {}

```diff
@@ -1,34 +1,39 @@
-Metadata-Version: 2.1 Name: propulate Version: 0.0.1 Summary: Massively
+Metadata-Version: 2.1 Name: propulate Version: 1.0.0 Summary: Massively
 parallel genetic optimization through asynchronous propagation of populations
 Author: Oskar Taubert, Marie Weiel, Helmholtz AI Author-email:
 oskar.taubert@kit.edu, marie.weiel@kit.edu License: mit Classifier: Development
 Status :: 4 - Beta Classifier: Programming Language :: Python Description-
 Content-Type: text/markdown; charset=UTF-8 Provides-Extra: testing License-
-File: LICENSE.md License-File: AUTHORS.rst ![Propulate Logo](./LOGO.svg) #
+File: LICENSE.md License-File: AUTHORS.md ![Propulate Logo](./LOGO.svg) #
 Parallel Propagator of Populations ## Project Status [![License: BSD-3](https:/
 /img.shields.io/badge/License-BSD--3-blue)](https://opensource.org/licenses/
-BSD-3-Clause) [![Code style: black](https://img.shields.io/badge/code%20style-
-black-000000.svg)](https://github.com/psf/black) ``Propulate`` is a massively
+BSD-3-Clause) ![PyPI - Downloads](https://img.shields.io/pypi/dm/propulate) [!
+[Code style: black](https://img.shields.io/badge/code%20style-black-
+000000.svg)](https://github.com/psf/black) ``Propulate`` is a massively
 parallel evolutionary hyperparameter optimizer based on the island model with
 asynchronous propagation of populations and asynchronous migration. In contrast
 to classical GAs, ``Propulate`` maintains a continuous population of already
 evaluated individuals with a softened notion of the typically strictly
 separated, discrete generations. Our contributions include: - A novel parallel
 genetic algorithm based on a fully asynchronized island model with
 independently processing workers. - Massive parallelism by asynchronous
 propagation of continuous populations and migration via efficient communication
 using the message passing interface. - Optimized use efficiency of parallel
 hardware by minimizing idle times in distributed computing environments. To be
 more efficient, the generations are less well separated than they usually are
 in evolutionary algorithms. New individuals are generated from a pool of
 currently active, already evaluated individuals that may be from any
 generation. Individuals may be removed from the breeding population based on
-different criteria. ## Documentation For usage example, see scripts. ##
-Installation Pull and run ``pip install -e .`` or ``python setup.py develop``.
-Requires an MPI implementation (currently only tested with OpenMPI) and
-``mpi4py``. ## To Dos - weight/parameter succession from parents or hall of
-fame - more algorithms and operators, covariance matrix adaptation evolution
-strategy ## Acknowledgments *This work is supported by the Helmholtz AI
-platform grant.*
+different criteria. You can find the corresponding publication here: Taubert,
+O. *et al.* (2023). Massively Parallel Genetic Optimization Through
+Asynchronous Propagation of Populations. In: Bhatele, A., Hammond, J.,
+Baboulin, M., Kruse, C. (eds) High Performance Computing. ISC High Performance
+2023. Lecture Notes in Computer Science, vol 13948. Springer, Cham. [https://
+doi.org/10.1007/978-3-031-32041-5_6](https://doi.org/10.1007/978-3-031-32041-
+5_6) ## Documentation For usage example, see scripts. ## Installation From
+PyPI: ``pip install propulate`` Alternatively, pull and run ``pip install -
+e .`` or ``python setup.py develop``. Requires an MPI implementation (currently
+only tested with OpenMPI) and ``mpi4py``. ## Acknowledgments *This work is
+supported by the Helmholtz AI platform grant.*
  style="position:absolute;top:50%;left:50%;"> [./.figs/logo_KIT.svg][./.figs/
 logo_HelmholtzAI.svg]
```

### Comparing `propulate-0.0.1/README.md` & `propulate-1.0.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 ![Propulate Logo](./LOGO.svg)
 
 # Parallel Propagator of Populations
 ## Project Status
 [![License: BSD-3](https://img.shields.io/badge/License-BSD--3-blue)](https://opensource.org/licenses/BSD-3-Clause)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/propulate)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-``Propulate`` is a massively parallel evolutionary hyperparameter optimizer based on the island model with asynchronous propagation of populations and asynchronous migration. 
-In contrast to classical GAs, ``Propulate`` maintains a continuous population of already evaluated individuals with a softened notion of the typically strictly separated, discrete generations. 
+``Propulate`` is a massively parallel evolutionary hyperparameter optimizer based on the island model with asynchronous propagation of populations and asynchronous migration.
+In contrast to classical GAs, ``Propulate`` maintains a continuous population of already evaluated individuals with a softened notion of the typically strictly separated, discrete generations.
 Our contributions include:
-- A novel parallel genetic algorithm based on a fully asynchronized island model with independently processing workers. 
+- A novel parallel genetic algorithm based on a fully asynchronized island model with independently processing workers.
 - Massive parallelism by asynchronous propagation of continuous populations and migration via efficient communication using the message passing interface.
 - Optimized use efficiency of parallel hardware by minimizing idle times in distributed computing environments.
 
 To be more efficient, the generations are less well separated than they usually are in evolutionary algorithms.
-New individuals are generated from a pool of currently active, already evaluated individuals that may be from any generation. 
+New individuals are generated from a pool of currently active, already evaluated individuals that may be from any generation.
 Individuals may be removed from the breeding population based on different criteria.
 
+You can find the corresponding publication here:  
+Taubert, O. *et al.* (2023). Massively Parallel Genetic Optimization Through Asynchronous Propagation of Populations. In: Bhatele, A., Hammond, J., Baboulin, M., Kruse, C. (eds) High Performance Computing. ISC High Performance 2023. Lecture Notes in Computer Science, vol 13948. Springer, Cham. [https://doi.org/10.1007/978-3-031-32041-5_6](https://doi.org/10.1007/978-3-031-32041-5_6)
+
 ## Documentation
 
 For usage example, see scripts.
 
 ## Installation
 
-Pull and run ``pip install -e .`` or ``python setup.py develop``.
+From PyPI: ``pip install propulate``  
+Alternatively, pull and run ``pip install -e .`` or ``python setup.py develop``.  
 Requires an MPI implementation (currently only tested with OpenMPI) and ``mpi4py``.
 
-## To Dos
-
-- weight/parameter succession from parents or hall of fame
-- more algorithms and operators, covariance matrix adaptation evolution strategy
-
 ## Acknowledgments
 *This work is supported by the Helmholtz AI platform grant.*
 <div align="center"; style="position:absolute;top:50%;left:50%;">
   <a href="http://www.kit.edu/english/index.php"><img src=./.figs/logo_KIT.svg height="50px" hspace="5%" vspace="0px"></a><a href="https://www.helmholtz.ai"><img src=./.figs/logo_HelmholtzAI.svg height="25px" hspace="5%" vspace="0px"></a>
 </div>
```

#### html2text {}

```diff
@@ -1,27 +1,32 @@
 ![Propulate Logo](./LOGO.svg) # Parallel Propagator of Populations ## Project
 Status [![License: BSD-3](https://img.shields.io/badge/License-BSD--3-blue)]
-(https://opensource.org/licenses/BSD-3-Clause) [![Code style: black](https://
-img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/
-black) ``Propulate`` is a massively parallel evolutionary hyperparameter
-optimizer based on the island model with asynchronous propagation of
-populations and asynchronous migration. In contrast to classical GAs,
-``Propulate`` maintains a continuous population of already evaluated
-individuals with a softened notion of the typically strictly separated,
-discrete generations. Our contributions include: - A novel parallel genetic
-algorithm based on a fully asynchronized island model with independently
-processing workers. - Massive parallelism by asynchronous propagation of
-continuous populations and migration via efficient communication using the
-message passing interface. - Optimized use efficiency of parallel hardware by
-minimizing idle times in distributed computing environments. To be more
-efficient, the generations are less well separated than they usually are in
-evolutionary algorithms. New individuals are generated from a pool of currently
-active, already evaluated individuals that may be from any generation.
-Individuals may be removed from the breeding population based on different
-criteria. ## Documentation For usage example, see scripts. ## Installation Pull
-and run ``pip install -e .`` or ``python setup.py develop``. Requires an MPI
-implementation (currently only tested with OpenMPI) and ``mpi4py``. ## To Dos -
-weight/parameter succession from parents or hall of fame - more algorithms and
-operators, covariance matrix adaptation evolution strategy ## Acknowledgments
-*This work is supported by the Helmholtz AI platform grant.*
+(https://opensource.org/licenses/BSD-3-Clause) ![PyPI - Downloads](https://
+img.shields.io/pypi/dm/propulate) [![Code style: black](https://img.shields.io/
+badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+``Propulate`` is a massively parallel evolutionary hyperparameter optimizer
+based on the island model with asynchronous propagation of populations and
+asynchronous migration. In contrast to classical GAs, ``Propulate`` maintains a
+continuous population of already evaluated individuals with a softened notion
+of the typically strictly separated, discrete generations. Our contributions
+include: - A novel parallel genetic algorithm based on a fully asynchronized
+island model with independently processing workers. - Massive parallelism by
+asynchronous propagation of continuous populations and migration via efficient
+communication using the message passing interface. - Optimized use efficiency
+of parallel hardware by minimizing idle times in distributed computing
+environments. To be more efficient, the generations are less well separated
+than they usually are in evolutionary algorithms. New individuals are generated
+from a pool of currently active, already evaluated individuals that may be from
+any generation. Individuals may be removed from the breeding population based
+on different criteria. You can find the corresponding publication here:
+Taubert, O. *et al.* (2023). Massively Parallel Genetic Optimization Through
+Asynchronous Propagation of Populations. In: Bhatele, A., Hammond, J.,
+Baboulin, M., Kruse, C. (eds) High Performance Computing. ISC High Performance
+2023. Lecture Notes in Computer Science, vol 13948. Springer, Cham. [https://
+doi.org/10.1007/978-3-031-32041-5_6](https://doi.org/10.1007/978-3-031-32041-
+5_6) ## Documentation For usage example, see scripts. ## Installation From
+PyPI: ``pip install propulate`` Alternatively, pull and run ``pip install -
+e .`` or ``python setup.py develop``. Requires an MPI implementation (currently
+only tested with OpenMPI) and ``mpi4py``. ## Acknowledgments *This work is
+supported by the Helmholtz AI platform grant.*
  style="position:absolute;top:50%;left:50%;"> [./.figs/logo_KIT.svg][./.figs/
 logo_HelmholtzAI.svg]
```

### Comparing `propulate-0.0.1/propulate/population.py` & `propulate-1.0.0/propulate/population.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # TODO invalidate loss, when entry is modified so this does not have to be done by the propagator
 # TODO genealogy
 # TODO have ordinal vs categorical inferred from list vs set
 
 from decimal import Decimal
-import time
 
 
 class Individual(dict):
     def __init__(self, generation=None, rank=None):
         super(Individual, self).__init__(list())
         self.generation = generation  # Equals each worker's iteration for continuous population in propulate.
         self.rank = rank
@@ -25,16 +24,20 @@
         rep = {
             key: (
                 f"{Decimal(self[key]):.2E}" if type(self[key]) == float else self[key]
             )
             for key in self
         }
         Active = "active" if self.active else "deactivated"
+        if self.loss is None:
+            loss_str = f"{self.loss}"
+        else:
+            loss_str = f"{Decimal(float(self.loss)):.2E}"
         return (
-            f"[{rep}, loss {Decimal(float(self.loss)):.2E}, I{self.isle}, W{self.rank}, "
+            f"[{rep}, loss " + loss_str + f", I{self.isle}, W{self.rank}, "
             f"G{self.generation}, {self.evaltime}, w{self.current}, m{self.migration_steps}, {Active}]"
         )
 
     def __eq__(self, other):
         # Check if object to compare to is of the same class.
         assert isinstance(other, self.__class__)
         # Check equivalence of actual traits, i.e., hyperparameter values.
@@ -62,11 +65,8 @@
         compare_traits = True
         for key in self.keys():
             if self[key] == other[key]:
                 continue
             else:
                 compare_traits = False
                 break
-        return (
-            compare_traits
-            and self.loss == other.loss
-        )
+        return compare_traits and self.loss == other.loss
```

### Comparing `propulate-0.0.1/propulate/propagators.py` & `propulate-1.0.0/propulate/propagators.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-import random
 import copy
+
 import numpy
 
 from .population import Individual
 
 
 def _check_compatible(out1, in2):
     """
-    Check compability of two propagators for stacking them together sequentially with Cascade().
+    Check compability of two propagators for stacking them together sequentially with Compose().
     """
     return out1 == in2 or in2 == -1
 
 
 class Propagator:
     """
     Abstract base class for all propagators, i.e., evolutionary operators, in Propulate.
@@ -73,25 +73,14 @@
               random number generator
         """
         super(Stochastic, self).__init__(parents, offspring, rng)
         self.probability = probability
         if offspring == 0:
             raise ValueError("Propagator has to sire more than 0 offspring.")
 
-    def __call__(self, inds):
-        """
-        Apply stochastic propagator (not implemented!).
-
-        Parameters
-        ----------
-        inds: propulate.population.Individual
-              individuals the propagator is applied to
-        """
-        raise NotImplementedError()
-
 
 class Conditional(Propagator):
     """
     Apply different propagators depending on whether breeding population is complete or not.
 
     If population consists of less than the specified number of individuals required for breeding,
     a different propagator is applied than if this condition is fulfilled.
@@ -132,51 +121,49 @@
             len(inds) >= self.pop_size
         ):  # If number of evaluated individuals >= pop_size apply true_prop.
             return self.true_prop(inds)
         else:  # Else apply false_prop.
             return self.false_prop(inds)
 
 
-class Cascade(Propagator):
+class Compose(Propagator):
     """
     Stack propagators together sequentially for successive application.
     """
 
     def __init__(self, propagators):
         """
-        Constructor of Cascade class.
+        Constructor of Compose class.
 
         Parameters
         ----------
         propagators : list of propulate.propagators.Propagator objects
                       propagators to be stacked together sequentially
         """
-        super(Cascade, self).__init__(propagators[0].parents, propagators[-1].offspring)
+        super(Compose, self).__init__(propagators[0].parents, propagators[-1].offspring)
         self.propagators = propagators
         for i in range(len(propagators) - 1):
             # Check compability of consecutive propagators in terms of number of parents + offsprings.
             if not _check_compatible(
                 propagators[i].offspring, propagators[i + 1].parents
             ):
                 outp = propagators[i]
                 inp = propagators[i + 1]
                 outd = outp.offspring
-                ind = indp.parents
+                ind = inp.parents
 
                 raise ValueError(
-                    "Incompatible combination of {} output individuals of {} and {} input individuals of {}".format(
-                        outd, outp, ind, inp
-                    )
+                    f"Incompatible combination of {outd} output individuals of {outp} and {ind} input individuals of {inp}."
                 )
 
     def __call__(
         self, inds
-    ):  # Apply propagators sequentially as requested in Cascade(...)
+    ):  # Apply propagators sequentially as requested in Compose(...)
         """
-        Apply Cascade propagator.
+        Apply Compose propagator.
 
         Parameters
         ----------
         inds: list of propulate.population.Individual objects
               individuals the propagator is applied to
 
         Returns
@@ -210,17 +197,15 @@
               random number generator
         """
         super(PointMutation, self).__init__(1, 1, probability, rng)
         self.points = points
         self.limits = limits
         if len(limits) < points:
             raise ValueError(
-                "Too many points to mutate for individual with {} traits".format(
-                    len(limits)
-                )
+                f"Too many points to mutate for individual with {len(limits)} traits."
             )
 
     def __call__(self, ind):
         """
         Apply point-mutation propagator.
 
         Parameters
@@ -237,15 +222,15 @@
             self.rng.random() < self.probability
         ):  # Apply propagator only with specified `probability`
             ind = copy.deepcopy(ind)
             ind.loss = None  # Initialize individual's loss attribute.
             # Determine traits to mutate via random sampling.
             # Return `self.points` length list of unique elements chosen from `ind.keys()`.
             # Used for random sampling without replacement.
-            to_mutate = self.rng.sample(ind.keys(), self.points)
+            to_mutate = self.rng.sample(sorted(ind.keys()), self.points)
             # Point-mutate `self.points` randomly chosen traits of individual `ind`.
             for i in to_mutate:
                 if type(ind[i]) == int:
                     # Return randomly selected element from int range(start, stop, step).
                     ind[i] = self.rng.randrange(*self.limits[i])
                 elif type(ind[i]) == float:
                     # Return random floating point number N within limits.
@@ -278,29 +263,23 @@
                       probability of application
         rng : random.Random()
               random number generator
         """
         super(RandomPointMutation, self).__init__(1, 1, probability, rng)
         if min_points <= 0:
             raise ValueError(
-                "Minimum number of points to mutate must be > 0 but was {}.".format(
-                    min_points
-                )
+                f"Minimum number of points to mutate must be > 0 but was {min_points}."
             )
         if len(limits) < max_points:
             raise ValueError(
-                "Too many points to mutate for individual with {} traits.".format(
-                    len(limits)
-                )
+                f"Too many points to mutate for individual with {len(limits)} traits."
             )
         if min_points > max_points:
             raise ValueError(
-                "Minimum number of traits to mutate must be <= respective maximum number but min_points = {} > {} = max_points.".format(
-                    min_points, max_points
-                )
+                f"Minimum number of traits to mutate must be <= respective maximum number but min_points = {min_points} > {max_points} = max_points."
             )
         self.min_points = int(min_points)
         self.max_points = int(max_points)
         self.limits = limits
 
     def __call__(self, ind):
         """
@@ -321,15 +300,15 @@
         ):  # Apply propagator only with specified `probability`
             ind = copy.deepcopy(ind)
             ind.loss = None  # Initialize individual's loss attribute.
             # Determine traits to mutate via random sampling.
             # Return `self.points` length list of unique elements chosen from `ind.keys()`.
             # Used for random sampling without replacement.
             points = self.rng.randint(self.min_points, self.max_points)
-            to_mutate = self.rng.sample(ind.keys(), points)
+            to_mutate = self.rng.sample(sorted(ind.keys()), points)
             # Point-mutate `points` randomly chosen traits of individual `ind`.
             for i in to_mutate:
                 if type(ind[i]) == int:
                     # Return randomly selected element from int range(start, stop, step).
                     ind[i] = self.rng.randrange(*self.limits[i])
                 elif type(ind[i]) == float:
                     # Return random floating point number N within limits.
@@ -366,17 +345,15 @@
         super(IntervalMutationNormal, self).__init__(1, 1, probability, rng)
         self.points = points  # number of traits to point-mutate
         self.limits = limits
         self.sigma_factor = sigma_factor
         n_interval_traits = len([x for x in limits if type(limits[x][0]) == float])
         if n_interval_traits < points:
             raise ValueError(
-                "Too many points to mutate for individual with {} interval traits".format(
-                    n_interval_traits
-                )
+                f"Too many points to mutate for individual with {n_interval_traits} interval traits"
             )
 
     def __call__(self, ind):
         """
         Apply interval-mutation propagator.
 
         Parameters
@@ -436,17 +413,15 @@
               random number generator
         """
         super(MateUniform, self).__init__(
             2, 1, probability, rng
         )  # Breed 1 offspring from 2 parents.
         if rel_parent_contrib <= 0 or rel_parent_contrib >= 1:
             raise ValueError(
-                "Relative parent contribution must be within (0, 1) but was {}.".format(
-                    rel_parent_contrib
-                )
+                f"Relative parent contribution must be within (0, 1) but was {rel_parent_contrib}."
             )
         self.rel_parent_contrib = rel_parent_contrib
 
     def __call__(self, inds):
         """
         Apply uniform-crossover propagator.
 
@@ -543,14 +518,15 @@
                       probability of application
         rng : random.Random()
               random number generator
         """
         super(MateSigmoid, self).__init__(
             2, 1, probability, rng
         )  # Breed 1 offspring from 2 parents.
+        self.temperature = temperature
 
     def __call__(self, inds):
         """
         Apply sigmoid-crossover propagator.
 
         Parameters
         ----------
@@ -561,45 +537,46 @@
         -------
         ind : propulate.population.Individual
               possibly cross-bred individual after application of propagator
         """
         ind = copy.deepcopy(inds[0])  # Consider 1st parent.
         if inds[0].loss <= inds[1].loss:
             delta = inds[0].loss - inds[1].loss
-            fraction = 1 / (1 + numpy.exp(-delta / temperature))
+            fraction = 1 / (1 + numpy.exp(-delta / self.temperature))
         else:
             delta = inds[1].loss - inds[0].loss
-            fraction = 1 - 1 / (1 + numpy.exp(-delta / temperature))
+            fraction = 1 - 1 / (1 + numpy.exp(-delta / self.temperature))
 
         if (
             self.rng.random() < self.probability
         ):  # Apply propagator only with specified `probability`.
             ind.loss = None  # Initialize individual's loss attribute.
             # Replace traits in 1st parent with values of 2nd parent with Boltzmann probability.
             for k in inds[1].keys():
                 if self.rng.random() > fraction:
                     ind[k] = inds[1][k]
         return ind  # Return offspring.
 
 
-class SelectBest(Propagator):
+class SelectMin(Propagator):
     """
     Select specified number of best performing individuals as evaluated by their losses.
+    i.e., those individuals with minimum losses.
     """
 
     def __init__(self, offspring, rng=None):
         """
-        Constructor of SelectBest class.
+        Constructor of SelectMin class.
 
         Parameters
         ----------
         offspring : int
                     number of offsprings (individuals to be selected)
         """
-        super(SelectBest, self).__init__(-1, offspring)
+        super(SelectMin, self).__init__(-1, offspring)
 
     def __call__(self, inds):
         """
         Apply elitist-selection propagator.
 
         Parameters
         ----------
@@ -609,39 +586,38 @@
         Returns
         -------
         ind : propulate.population.Individual
               list of selected individuals after application of propagator
         """
         if len(inds) < self.offspring:
             raise ValueError(
-                "Has to have at least {} individuals to select the {} best ones.".format(
-                    self.offspring, self.offspring
-                )
+                f"Has to have at least {self.offspring} individuals to select the {self.offspring} best ones."
             )
         # Sort elements of given iterable in specific order + return as list.
         return sorted(inds, key=lambda ind: ind.loss)[
             : self.offspring
         ]  # Return `self.offspring` best individuals in terms of loss.
 
 
-class SelectWorst(Propagator):
+class SelectMax(Propagator):
     """
-    Select specified number of worst performing individuals as evaluated by their losses.
+    Select specified number of worst performing individuals as evaluated by their losses,
+    i.e., those individuals with maximum losses.
     """
 
     def __init__(self, offspring, rng=None):
         """
-        Constructor of SelectBest class.
+        Constructor of SelectMax class.
 
         Parameters
         ----------
         offspring : int
                     number of offsprings (individuals to be selected)
         """
-        super(SelectWorst, self).__init__(-1, offspring)
+        super(SelectMax, self).__init__(-1, offspring)
 
     def __call__(self, inds):
         """
         Apply anti-elitist-selection propagator.
 
         Parameters
         ----------
@@ -651,32 +627,30 @@
         Returns
         -------
         ind : propulate.population.Individual
               list of selected individuals after application of propagator
         """
         if len(inds) < self.offspring:
             raise ValueError(
-                "Has to have at least {} individuals to select the {} worst ones.".format(
-                    self.offspring, self.offspring
-                )
+                f"Has to have at least {self.offspring} individuals to select the {self.offspring} worst ones."
             )
         # Sort elements of given iterable in specific order + return as list.
         return sorted(inds, key=lambda ind: -ind.loss)[
             : self.offspring
         ]  # Return `self.offspring` worst individuals in terms of loss.
 
 
 class SelectUniform(Propagator):
     """
     Select specified number of individuals randomly.
     """
 
     def __init__(self, offspring, rng=None):
         """
-        Constructor of SelectRandom class.
+        Constructor of SelectUniform class.
 
         Parameters
         ----------
         offspring : int
                     number of offsprings (individuals to be selected)
         rng : random.Random()
               random number generator
```

### Comparing `propulate-0.0.1/propulate/utils.py` & `propulate-1.0.0/propulate/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from .propagators import (
+    Compose,
     Conditional,
-    Cascade,
-    PointMutation,
-    MateUniform,
-    SelectBest,
-    SelectUniform,
     InitUniform,
     IntervalMutationNormal,
+    MateUniform,
+    PointMutation,
+    SelectMin,
+    SelectUniform,
 )
-from .population import Individual
 
 
 def get_default_propagator(
     pop_size, limits, mate_prob, mut_prob, random_prob, sigma_factor=0.05, rng=None
 ):
     """
     Get propulate's default propagator.
@@ -30,69 +29,39 @@
     random_prob : float
                   random-initialization probability
     sigma_factor : float
                    scaling factor for obtaining std from search-space boundaries for interval mutation
     rng : random.Random()
           random number generator
     """
-    propagator = Cascade(  # Compose propagator out of basic evolutionary operators with Cascade(...).
-        [
-            SelectBest(pop_size),
-            SelectUniform(2, rng=rng),
-            MateUniform(mate_prob, rng=rng),
-            PointMutation(limits, probability=mut_prob, rng=rng),
-            IntervalMutationNormal(limits, sigma_factor=sigma_factor, probability=1, rng=rng),
-            InitUniform(
-                limits, parents=1, probability=random_prob, rng=rng
-            ),  # TODO this should be put in a "forked" propagator?
-        ]
-    )
-
-    init = InitUniform(limits, rng=rng)
-
-    propagator = Conditional(
-        pop_size, propagator, init
-    )  # Initialize random if current population size < specified `pop_size`.
-    return propagator
-
-
-def get_default_propagator_select_random(
-    pop_size, limits, mate_prob, mut_prob, random_prob, sigma_factor=0.1, rng=None):
-    """
-    Get propulate's default propagator.
-
-
-    Parameters
-    ----------
-    pop_size : int
-               number of individuals in breeding population
-    limits : dict
-    mate_prob : float
-                uniform-crossover probability
-    mut_prob : float
-               point-mutation probability
-    random_prob : float
-                  random-initialization probability
-    sigma_factor : float
-                   scaling factor for obtaining std from search-space boundaries for interval mutation
-    rng : random.Random()
-          random number generator
-    """
-    propagator = Cascade(  # Compose propagator out of basic evolutionary operators with Cascade(...).
-        [
-            SelectUniform(pop_size, rng=rng),
-            SelectUniform(2, rng=rng),
-            MateUniform(mate_prob, rng=rng),
-            PointMutation(limits, probability=mut_prob, rng=rng),
-            IntervalMutationNormal(limits, sigma_factor=sigma_factor, probability=1, rng=rng),
-            InitUniform(
-                limits, parents=1, probability=random_prob, rng=rng
-            ),  # TODO this should be put in a "forked" propagator?
-        ]
-    )
+    if (
+        len([x for x in limits if type(limits[x][0]) == float]) > 0
+    ):  # Check for existence of at least one continuous trait.
+        propagator = Compose(  # Compose propagator out of basic evolutionary operators with Compose(...).
+            [
+                SelectMin(pop_size),
+                SelectUniform(2, rng=rng),
+                MateUniform(mate_prob, rng=rng),
+                PointMutation(limits, probability=mut_prob, rng=rng),
+                IntervalMutationNormal(
+                    limits, sigma_factor=sigma_factor, probability=1, rng=rng
+                ),
+                InitUniform(limits, parents=1, probability=random_prob, rng=rng),
+            ]
+        )
+    else:
+        propagator = Compose(  # Compose propagator out of basic evolutionary operators with Compose(...).
+            [
+                SelectMin(pop_size),
+                SelectUniform(2, rng=rng),
+                MateUniform(mate_prob, rng=rng),
+                PointMutation(limits, probability=mut_prob, rng=rng),
+                InitUniform(limits, parents=1, probability=random_prob, rng=rng),
+            ]
+        )
 
     init = InitUniform(limits, rng=rng)
 
     propagator = Conditional(
         pop_size, propagator, init
     )  # Initialize random if current population size < specified `pop_size`.
     return propagator
```

### Comparing `propulate-0.0.1/propulate/wrapper.py` & `propulate-1.0.0/propulate/islands.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,36 @@
-import os
-import pickle
-from operator import attrgetter
-from mpi4py import MPI
+from pathlib import Path
 import numpy as np
 
-from .population import Individual
-from .propulator import Propulator, PolliPropulator
-from .propagators import SelectBest, SelectUniform, SelectWorst
+from mpi4py import MPI
+
+from .propagators import SelectMin, SelectMax
+from .propulator import Propulator
+from .pollinator import PolliPropulator
 
 
 class Islands:
     """
     Wrapper class for propulate optimization runs with multiple separate evolutionary isles.
     """
 
     def __init__(
         self,
         loss_fn,
         propagator,
-        rng, 
+        rng,
         generations=0,
         num_isles=1,
         isle_sizes=None,
         migration_topology=None,
         migration_probability=0.0,
-        emigration_propagator=SelectBest,
-        immigration_propagator=SelectWorst,
+        emigration_propagator=SelectMin,
+        immigration_propagator=SelectMax,
         pollination=False,
-        load_checkpoint="pop_cpt.p",
-        save_checkpoint="pop_cpt.p",
+        checkpoint_path=Path('./'),
     ):
         """
         Constructor of Islands() class.
 
         Parameters
         ----------
         loss_fn : callable
@@ -59,18 +57,16 @@
         immigration_propagator : propulate.propagators.Propagator
                                  immigration propagator, i.e., how to choose individuals on target isle
                                  to be replaced by immigrants.
                                  Should be some kind of selection operator.
         pollination : bool
                       If True, copies of emigrants are sent, otherwise, emigrants are removed from
                       original isle.
-        load_checkpoint : str
-                          checkpoint file to resume optimization from
-        save_checkpoint : str
-                          checkpoint file to write checkpoints to
+        checkpoint_path : Union[Path, str]
+                          Path where checkpoints are loaded from and stored.
         """
         # Set attributes.
         self.loss_fn = loss_fn  # callable loss function
         self.propagator = propagator  # propagator
         self.generations = int(
             generations
         )  # number of generations, i.e., evaluations per individual
@@ -95,15 +91,15 @@
             remainder = int(
                 size % num_isles
             )  # remaining workers to be distributed equally for load balancing
 
             isle_sizes = []
             for i in range(num_isles):
                 if i < remainder:
-                    temp = isle_sizes.append(base_size + 1)
+                    isle_sizes.append(base_size + 1)
                 else:
                     isle_sizes.append(base_size)
 
         isle_sizes = np.array(isle_sizes)
 
         # Heterogeneous case with user-defined isle sizes.
         if np.sum(isle_sizes) != size:
@@ -162,67 +158,63 @@
             print(
                 f"Migration topology {migration_topology} has shape {migration_topology.shape}."
             )
 
         if migration_topology.shape != (num_isles, num_isles):
             raise ValueError(
                 f"Migration topology must be a quadratic matrix of size "
-                f"{unique.size} x {unique.size} but has shape {migration_topology.shape}."
+                f"{unique_ind.size} x {unique_ind.size} but has shape {migration_topology.shape}."
             )
 
         if migration_probability > 1.0:
             raise ValueError(
                 f"Migration probability must be in [0, 1] but was set to {migration_probability}."
             )
         migration_prob = float(migration_probability) / comm_intra.size
 
         if rank == 0:
             print(
                 f"NOTE: Isle migration probability of {migration_probability} "
                 f"results in per-rank migration probability of {migration_prob}."
             )
-        load_rank_cpt = "isle_" + str(isle_idx) + "_" + load_checkpoint
-        save_rank_cpt = "isle_" + str(isle_idx) + "_" + save_checkpoint
 
         self.emigration_propagator = emigration_propagator
 
         if rank == 0:
             print("Starting parallel optimization process...")
         MPI.COMM_WORLD.barrier()
         # Set up Propulator objects, one for each isle.
-        if pollination == False:
+        if pollination is False:
             if MPI.COMM_WORLD.rank == 0:
                 print("No pollination.")
             self.propulator = Propulator(
                 loss_fn,
                 propagator,
                 comm=comm_intra,
                 generations=generations,
                 isle_idx=isle_idx,
-                load_checkpoint=load_rank_cpt,
-                save_checkpoint=save_rank_cpt,
+                checkpoint_path=checkpoint_path,
                 comm_inter=comm_inter,
                 migration_topology=migration_topology,
                 migration_prob=migration_prob,
                 emigration_propagator=emigration_propagator,
                 unique_ind=unique_ind,
                 unique_counts=isle_sizes,
                 rng=rng,
             )
-        elif pollination == True:
+        elif pollination is True:
             if MPI.COMM_WORLD.rank == 0:
                 print("Pollination.")
             self.propulator = PolliPropulator(
                 loss_fn,
                 propagator,
                 comm=comm_intra,
                 generations=generations,
                 isle_idx=isle_idx,
-                load_checkpoint=load_rank_cpt,
-                save_checkpoint=save_rank_cpt,
+                checkpoint_path=checkpoint_path,
                 comm_inter=comm_inter,
                 migration_topology=migration_topology,
                 migration_prob=migration_prob,
                 emigration_propagator=emigration_propagator,
                 immigration_propagator=immigration_propagator,
                 unique_ind=unique_ind,
                 unique_counts=isle_sizes,
```

### Comparing `propulate-0.0.1/propulate.egg-info/PKG-INFO` & `propulate-1.0.0/propulate.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 Metadata-Version: 2.1
 Name: propulate
-Version: 0.0.1
+Version: 1.0.0
 Summary: Massively parallel genetic optimization through asynchronous propagation of populations
 Author: Oskar Taubert, Marie Weiel, Helmholtz AI
 Author-email: oskar.taubert@kit.edu, marie.weiel@kit.edu
 License: mit
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: testing
 License-File: LICENSE.md
-License-File: AUTHORS.rst
+License-File: AUTHORS.md
 
 ![Propulate Logo](./LOGO.svg)
 
 # Parallel Propagator of Populations
 ## Project Status
 [![License: BSD-3](https://img.shields.io/badge/License-BSD--3-blue)](https://opensource.org/licenses/BSD-3-Clause)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/propulate)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-``Propulate`` is a massively parallel evolutionary hyperparameter optimizer based on the island model with asynchronous propagation of populations and asynchronous migration. 
-In contrast to classical GAs, ``Propulate`` maintains a continuous population of already evaluated individuals with a softened notion of the typically strictly separated, discrete generations. 
+``Propulate`` is a massively parallel evolutionary hyperparameter optimizer based on the island model with asynchronous propagation of populations and asynchronous migration.
+In contrast to classical GAs, ``Propulate`` maintains a continuous population of already evaluated individuals with a softened notion of the typically strictly separated, discrete generations.
 Our contributions include:
-- A novel parallel genetic algorithm based on a fully asynchronized island model with independently processing workers. 
+- A novel parallel genetic algorithm based on a fully asynchronized island model with independently processing workers.
 - Massive parallelism by asynchronous propagation of continuous populations and migration via efficient communication using the message passing interface.
 - Optimized use efficiency of parallel hardware by minimizing idle times in distributed computing environments.
 
 To be more efficient, the generations are less well separated than they usually are in evolutionary algorithms.
-New individuals are generated from a pool of currently active, already evaluated individuals that may be from any generation. 
+New individuals are generated from a pool of currently active, already evaluated individuals that may be from any generation.
 Individuals may be removed from the breeding population based on different criteria.
 
+You can find the corresponding publication here:  
+Taubert, O. *et al.* (2023). Massively Parallel Genetic Optimization Through Asynchronous Propagation of Populations. In: Bhatele, A., Hammond, J., Baboulin, M., Kruse, C. (eds) High Performance Computing. ISC High Performance 2023. Lecture Notes in Computer Science, vol 13948. Springer, Cham. [https://doi.org/10.1007/978-3-031-32041-5_6](https://doi.org/10.1007/978-3-031-32041-5_6)
+
 ## Documentation
 
 For usage example, see scripts.
 
 ## Installation
 
-Pull and run ``pip install -e .`` or ``python setup.py develop``.
+From PyPI: ``pip install propulate``  
+Alternatively, pull and run ``pip install -e .`` or ``python setup.py develop``.  
 Requires an MPI implementation (currently only tested with OpenMPI) and ``mpi4py``.
 
-## To Dos
-
-- weight/parameter succession from parents or hall of fame
-- more algorithms and operators, covariance matrix adaptation evolution strategy
-
 ## Acknowledgments
 *This work is supported by the Helmholtz AI platform grant.*
 <div align="center"; style="position:absolute;top:50%;left:50%;">
   <a href="http://www.kit.edu/english/index.php"><img src=./.figs/logo_KIT.svg height="50px" hspace="5%" vspace="0px"></a><a href="https://www.helmholtz.ai"><img src=./.figs/logo_HelmholtzAI.svg height="25px" hspace="5%" vspace="0px"></a>
 </div>
```

#### html2text {}

```diff
@@ -1,34 +1,39 @@
-Metadata-Version: 2.1 Name: propulate Version: 0.0.1 Summary: Massively
+Metadata-Version: 2.1 Name: propulate Version: 1.0.0 Summary: Massively
 parallel genetic optimization through asynchronous propagation of populations
 Author: Oskar Taubert, Marie Weiel, Helmholtz AI Author-email:
 oskar.taubert@kit.edu, marie.weiel@kit.edu License: mit Classifier: Development
 Status :: 4 - Beta Classifier: Programming Language :: Python Description-
 Content-Type: text/markdown; charset=UTF-8 Provides-Extra: testing License-
-File: LICENSE.md License-File: AUTHORS.rst ![Propulate Logo](./LOGO.svg) #
+File: LICENSE.md License-File: AUTHORS.md ![Propulate Logo](./LOGO.svg) #
 Parallel Propagator of Populations ## Project Status [![License: BSD-3](https:/
 /img.shields.io/badge/License-BSD--3-blue)](https://opensource.org/licenses/
-BSD-3-Clause) [![Code style: black](https://img.shields.io/badge/code%20style-
-black-000000.svg)](https://github.com/psf/black) ``Propulate`` is a massively
+BSD-3-Clause) ![PyPI - Downloads](https://img.shields.io/pypi/dm/propulate) [!
+[Code style: black](https://img.shields.io/badge/code%20style-black-
+000000.svg)](https://github.com/psf/black) ``Propulate`` is a massively
 parallel evolutionary hyperparameter optimizer based on the island model with
 asynchronous propagation of populations and asynchronous migration. In contrast
 to classical GAs, ``Propulate`` maintains a continuous population of already
 evaluated individuals with a softened notion of the typically strictly
 separated, discrete generations. Our contributions include: - A novel parallel
 genetic algorithm based on a fully asynchronized island model with
 independently processing workers. - Massive parallelism by asynchronous
 propagation of continuous populations and migration via efficient communication
 using the message passing interface. - Optimized use efficiency of parallel
 hardware by minimizing idle times in distributed computing environments. To be
 more efficient, the generations are less well separated than they usually are
 in evolutionary algorithms. New individuals are generated from a pool of
 currently active, already evaluated individuals that may be from any
 generation. Individuals may be removed from the breeding population based on
-different criteria. ## Documentation For usage example, see scripts. ##
-Installation Pull and run ``pip install -e .`` or ``python setup.py develop``.
-Requires an MPI implementation (currently only tested with OpenMPI) and
-``mpi4py``. ## To Dos - weight/parameter succession from parents or hall of
-fame - more algorithms and operators, covariance matrix adaptation evolution
-strategy ## Acknowledgments *This work is supported by the Helmholtz AI
-platform grant.*
+different criteria. You can find the corresponding publication here: Taubert,
+O. *et al.* (2023). Massively Parallel Genetic Optimization Through
+Asynchronous Propagation of Populations. In: Bhatele, A., Hammond, J.,
+Baboulin, M., Kruse, C. (eds) High Performance Computing. ISC High Performance
+2023. Lecture Notes in Computer Science, vol 13948. Springer, Cham. [https://
+doi.org/10.1007/978-3-031-32041-5_6](https://doi.org/10.1007/978-3-031-32041-
+5_6) ## Documentation For usage example, see scripts. ## Installation From
+PyPI: ``pip install propulate`` Alternatively, pull and run ``pip install -
+e .`` or ``python setup.py develop``. Requires an MPI implementation (currently
+only tested with OpenMPI) and ``mpi4py``. ## Acknowledgments *This work is
+supported by the Helmholtz AI platform grant.*
  style="position:absolute;top:50%;left:50%;"> [./.figs/logo_KIT.svg][./.figs/
 logo_HelmholtzAI.svg]
```

### Comparing `propulate-0.0.1/setup.cfg` & `propulate-1.0.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = propulate
-version = 0.0.1
+version = 1.0.0
 description = Massively parallel genetic optimization through asynchronous propagation of populations
 author = Oskar Taubert, Marie Weiel, Helmholtz AI
 author_email = oskar.taubert@kit.edu, marie.weiel@kit.edu
 license = mit
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8
 classifiers = 
@@ -36,21 +36,14 @@
 
 [options.entry_points]
 
 [test]
 extras = True
 
 [tool:pytest]
-addopts = 
-	--cov propulate --cov-report term-missing
-	--verbose
-norecursedirs = 
-	dist
-	build
-	.tox
 testpaths = tests
 
 [aliases]
 dists = bdist_wheel
 
 [bdist_wheel]
 universal = 1
@@ -66,12 +59,13 @@
 [flake8]
 exclude = 
 	.tox
 	build
 	dist
 	.eggs
 	docs/conf.py
+max-line-length = 250
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

