# Comparing `tmp/numba_rvsdg-0.0.1.tar.gz` & `tmp/numba_rvsdg-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numba_rvsdg-0.0.1.tar", last modified: Mon Mar 27 15:13:15 2023, max compression
+gzip compressed data, was "numba_rvsdg-0.0.2.tar", last modified: Thu Jun 22 13:03:05 2023, max compression
```

## Comparing `numba_rvsdg-0.0.1.tar` & `numba_rvsdg-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,38 @@
-drwx------   0 vhaenel    (503) staff       (20)        0 2023-03-27 15:13:15.415098 numba_rvsdg-0.0.1/
--rw-------   0 vhaenel    (503) staff       (20)     1286 2023-02-24 09:45:24.000000 numba_rvsdg-0.0.1/LICENSE
--rw-------   0 vhaenel    (503) staff       (20)     5385 2023-03-27 15:13:15.414965 numba_rvsdg-0.0.1/PKG-INFO
--rw-------   0 vhaenel    (503) staff       (20)     5067 2023-03-27 11:55:12.000000 numba_rvsdg-0.0.1/README.md
-drwx------   0 vhaenel    (503) staff       (20)        0 2023-03-27 15:13:15.413926 numba_rvsdg-0.0.1/numba_rvsdg/
--rw-------   0 vhaenel    (503) staff       (20)        0 2023-03-15 20:09:13.000000 numba_rvsdg-0.0.1/numba_rvsdg/__init__.py
-drwx------   0 vhaenel    (503) staff       (20)        0 2023-03-27 15:13:15.414757 numba_rvsdg-0.0.1/numba_rvsdg.egg-info/
--rw-------   0 vhaenel    (503) staff       (20)     5385 2023-03-27 15:13:15.000000 numba_rvsdg-0.0.1/numba_rvsdg.egg-info/PKG-INFO
--rw-------   0 vhaenel    (503) staff       (20)      230 2023-03-27 15:13:15.000000 numba_rvsdg-0.0.1/numba_rvsdg.egg-info/SOURCES.txt
--rw-------   0 vhaenel    (503) staff       (20)        1 2023-03-27 15:13:15.000000 numba_rvsdg-0.0.1/numba_rvsdg.egg-info/dependency_links.txt
--rw-------   0 vhaenel    (503) staff       (20)       16 2023-03-27 15:13:15.000000 numba_rvsdg-0.0.1/numba_rvsdg.egg-info/requires.txt
--rw-------   0 vhaenel    (503) staff       (20)       12 2023-03-27 15:13:15.000000 numba_rvsdg-0.0.1/numba_rvsdg.egg-info/top_level.txt
--rw-------   0 vhaenel    (503) staff       (20)      511 2023-03-15 20:09:13.000000 numba_rvsdg-0.0.1/pyproject.toml
--rw-------   0 vhaenel    (503) staff       (20)       38 2023-03-27 15:13:15.415143 numba_rvsdg-0.0.1/setup.cfg
+drwx------   0 vhaenel    (503) staff       (20)        0 2023-06-22 13:03:05.677966 numba_rvsdg-0.0.2/
+-rw-------   0 vhaenel    (503) staff       (20)     1286 2023-02-24 09:45:24.000000 numba_rvsdg-0.0.2/LICENSE
+-rw-------   0 vhaenel    (503) staff       (20)     4990 2023-06-22 13:03:05.677793 numba_rvsdg-0.0.2/PKG-INFO
+-rw-------   0 vhaenel    (503) staff       (20)     4652 2023-06-22 12:38:52.000000 numba_rvsdg-0.0.2/README.md
+drwx------   0 vhaenel    (503) staff       (20)        0 2023-06-22 13:03:05.667810 numba_rvsdg-0.0.2/numba_rvsdg/
+-rw-------   0 vhaenel    (503) staff       (20)        0 2023-04-06 08:43:00.000000 numba_rvsdg-0.0.2/numba_rvsdg/__init__.py
+drwx------   0 vhaenel    (503) staff       (20)        0 2023-06-22 13:03:05.669000 numba_rvsdg-0.0.2/numba_rvsdg/core/
+drwx------   0 vhaenel    (503) staff       (20)        0 2023-06-22 13:03:05.674850 numba_rvsdg-0.0.2/numba_rvsdg/core/datastructures/
+-rw-------   0 vhaenel    (503) staff       (20)    11540 2023-06-22 12:38:52.000000 numba_rvsdg-0.0.2/numba_rvsdg/core/datastructures/basic_block.py
+-rw-------   0 vhaenel    (503) staff       (20)      285 2023-06-22 12:38:52.000000 numba_rvsdg-0.0.2/numba_rvsdg/core/datastructures/block_names.py
+-rw-------   0 vhaenel    (503) staff       (20)     4953 2023-06-22 12:38:52.000000 numba_rvsdg-0.0.2/numba_rvsdg/core/datastructures/byte_flow.py
+-rw-------   0 vhaenel    (503) staff       (20)     4832 2023-06-22 12:38:52.000000 numba_rvsdg-0.0.2/numba_rvsdg/core/datastructures/flow_info.py
+-rw-------   0 vhaenel    (503) staff       (20)    35123 2023-06-22 12:38:52.000000 numba_rvsdg-0.0.2/numba_rvsdg/core/datastructures/scfg.py
+-rw-------   0 vhaenel    (503) staff       (20)    23260 2023-06-22 12:57:56.000000 numba_rvsdg-0.0.2/numba_rvsdg/core/transformations.py
+-rw-------   0 vhaenel    (503) staff       (20)     1154 2023-06-22 12:38:52.000000 numba_rvsdg-0.0.2/numba_rvsdg/core/utils.py
+drwx------   0 vhaenel    (503) staff       (20)        0 2023-06-22 13:03:05.675087 numba_rvsdg-0.0.2/numba_rvsdg/networkx_vendored/
+-rw-------   0 vhaenel    (503) staff       (20)     2483 2023-06-22 12:38:52.000000 numba_rvsdg-0.0.2/numba_rvsdg/networkx_vendored/scc.py
+drwx------   0 vhaenel    (503) staff       (20)        0 2023-06-22 13:03:05.675274 numba_rvsdg-0.0.2/numba_rvsdg/rendering/
+-rw-------   0 vhaenel    (503) staff       (20)    11916 2023-06-22 12:38:52.000000 numba_rvsdg-0.0.2/numba_rvsdg/rendering/rendering.py
+drwx------   0 vhaenel    (503) staff       (20)        0 2023-06-22 13:03:05.677539 numba_rvsdg-0.0.2/numba_rvsdg/tests/
+-rw-------   0 vhaenel    (503) staff       (20)     6262 2023-06-22 12:38:52.000000 numba_rvsdg-0.0.2/numba_rvsdg/tests/mock_asm.py
+-rw-------   0 vhaenel    (503) staff       (20)    13374 2023-06-22 12:38:52.000000 numba_rvsdg-0.0.2/numba_rvsdg/tests/simulator.py
+-rw-------   0 vhaenel    (503) staff       (20)     8874 2023-06-22 12:38:52.000000 numba_rvsdg-0.0.2/numba_rvsdg/tests/test_byteflow.py
+-rw-------   0 vhaenel    (503) staff       (20)     1477 2023-06-22 12:38:52.000000 numba_rvsdg-0.0.2/numba_rvsdg/tests/test_fig3.py
+-rw-------   0 vhaenel    (503) staff       (20)     1396 2023-06-22 12:38:52.000000 numba_rvsdg-0.0.2/numba_rvsdg/tests/test_fig4.py
+-rw-------   0 vhaenel    (503) staff       (20)     1913 2023-06-22 12:38:52.000000 numba_rvsdg-0.0.2/numba_rvsdg/tests/test_mock_asm.py
+-rw-------   0 vhaenel    (503) staff       (20)     4129 2023-06-22 12:38:52.000000 numba_rvsdg-0.0.2/numba_rvsdg/tests/test_scfg.py
+-rw-------   0 vhaenel    (503) staff       (20)     5053 2023-05-03 16:50:18.000000 numba_rvsdg-0.0.2/numba_rvsdg/tests/test_simulate.py
+-rw-------   0 vhaenel    (503) staff       (20)    19260 2023-06-22 12:38:52.000000 numba_rvsdg-0.0.2/numba_rvsdg/tests/test_transforms.py
+-rw-------   0 vhaenel    (503) staff       (20)     3927 2023-06-22 12:38:52.000000 numba_rvsdg-0.0.2/numba_rvsdg/tests/test_utils.py
+drwx------   0 vhaenel    (503) staff       (20)        0 2023-06-22 13:03:05.668640 numba_rvsdg-0.0.2/numba_rvsdg.egg-info/
+-rw-------   0 vhaenel    (503) staff       (20)     4990 2023-06-22 13:03:05.000000 numba_rvsdg-0.0.2/numba_rvsdg.egg-info/PKG-INFO
+-rw-------   0 vhaenel    (503) staff       (20)      916 2023-06-22 13:03:05.000000 numba_rvsdg-0.0.2/numba_rvsdg.egg-info/SOURCES.txt
+-rw-------   0 vhaenel    (503) staff       (20)        1 2023-06-22 13:03:05.000000 numba_rvsdg-0.0.2/numba_rvsdg.egg-info/dependency_links.txt
+-rw-------   0 vhaenel    (503) staff       (20)       71 2023-06-22 13:03:05.000000 numba_rvsdg-0.0.2/numba_rvsdg.egg-info/requires.txt
+-rw-------   0 vhaenel    (503) staff       (20)       12 2023-06-22 13:03:05.000000 numba_rvsdg-0.0.2/numba_rvsdg.egg-info/top_level.txt
+-rw-------   0 vhaenel    (503) staff       (20)      636 2023-06-22 12:57:56.000000 numba_rvsdg-0.0.2/pyproject.toml
+-rw-------   0 vhaenel    (503) staff       (20)       38 2023-06-22 13:03:05.678018 numba_rvsdg-0.0.2/setup.cfg
```

### Comparing `numba_rvsdg-0.0.1/LICENSE` & `numba_rvsdg-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `numba_rvsdg-0.0.1/PKG-INFO` & `numba_rvsdg-0.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 Metadata-Version: 2.1
 Name: numba_rvsdg
-Version: 0.0.1
+Version: 0.0.2
 Summary: Numba Compatible RVSDG utilities
 Author-email: Numba Developers <none@none.none>
 License: BSD-2-Clause
 Keywords: numba
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 # numba-rvsdg
 
 Numba compatible RVSDG (Regionalized Value State Dependence Graph)  utilities.
 
 ## about
 
 This repository contains Numba compatible utilities for working with RVSDGs
 (Regionalized Value State Dependency Graphs). RVSDGs are a type of
 Intermediary Representation (IR) suitable for regularizing Python bytecode
 within Numba.
 
 The code in this repository is an implementation of the CFG restructuring
-algorithms in Bahmann2015, specifically those from section 4.1 and 4.2: namely
+algorithms in Bahmann 2015, specifically those from section 4.1 and 4.2: namely
 "loop restructuring" and "branch restructuring". These are interesting for
-Numba because they serve to clearly identify regions withing the Python
+Numba because they serve to clearly identify regions within the Python
 bytecode.
 
 ## dependencies
 
 * Python 3.11
 * graphviz
 * pyyaml
 
-As of 2023-03-06 you can create a conda env using the following:
+You can create a conda env using the following:
 
 ```
 conda env create -n numba-rvsdg python=3.11 python-graphviz
 conda activate numba-rvsdg
 pip install pyyaml
 ```
 
@@ -50,24 +51,23 @@
 
 ```
 numba_rvsdg
 ├── __init__.py
 ├── core
 │   ├── datastructures
 │   │   ├── basic_block.py  # BasicBlock implementation
-│   │   ├── block_map.py    # BlockMap implementation, maps labels to blocks
-│   │   ├── byte_flow.py    # ByteFlow implementation, BlockMap + bytecode
+│   │   ├── scfg.py         # SCFG implementation, maps names to blocks
+│   │   ├── byte_flow.py    # ByteFlow implementation, SCFG + bytecode
 │   │   ├── flow_info.py    # Converts program to ByteFlow
-│   │   └── labels.py       # Collection of Label classes
 │   ├── transformations.py  # Algorithms
 │   └── utils.py            # Miscellaneous utilities
 ├── networkx_vendored
 │   └── scc.py              # Strongly Connected Componets (loop detection)
 ├── rendering
-│   └── rendering.py        # Graphivz based rendering of BlockMaps
+│   └── rendering.py        # Graphivz based rendering of SCFGs
 ├── tests
 │   ├── simulator.py        # Simulator utility for running SCFGs
 │   ├── test_byteflow.py    # Testung ByteFlow and others
 │   ├── test_fig3.py        # Testing fig. 3 from Bahman2015
 │   ├── test_fig4.py        # Testing fig. 4 from Bahman2015
 │   ├── test_simulate.py    # Simulator based testing
 │   └── test_transforms.py  # Testing graph transformations
@@ -82,33 +82,27 @@
 restructuring" is the loop-restructured version and "branch-restructured" is
 the final form which includes closing, loop-restructuring and
 branch-restructuring.
 
 
 ```python
 # Example: for loop with branch and early exit
+
+from numba_rvsdg.rendering.rendering import render_func
+
 def foo(n):
     c = 0
     for i in range(n):
         c += 1
         if i == 100:
             break
     return c
 
-flow = ByteFlow.from_bytecode(foo)
-ByteFlowRenderer().render_byteflow(flow).view("initial")
-
-cflow = flow._join_returns()
-ByteFlowRenderer().render_byteflow(cflow).view("closed")
-
-lflow = cflow._restructure_loop()
-ByteFlowRenderer().render_byteflow(lflow).view("loop restructured")
+render_func(foo)
 
-bflow = lflow._restructure_branch()
-ByteFlowRenderer().render_byteflow(bflow).view("branch restructured")
 ```
 
 ![initial](docs/images/initial.png "initial")
 ![closed](docs/images/closed.png "closed")
 ![loop-restructured](docs/images/loop_restructured.png "loop-restructured")
 ![branch-restructured](docs/images/branch_restructured.png "branch-restructured")
```

### Comparing `numba_rvsdg-0.0.1/README.md` & `numba_rvsdg-0.0.2/numba_rvsdg.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,44 @@
+Metadata-Version: 2.1
+Name: numba-rvsdg
+Version: 0.0.2
+Summary: Numba Compatible RVSDG utilities
+Author-email: Numba Developers <none@none.none>
+License: BSD-2-Clause
+Keywords: numba
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 # numba-rvsdg
 
 Numba compatible RVSDG (Regionalized Value State Dependence Graph)  utilities.
 
 ## about
 
 This repository contains Numba compatible utilities for working with RVSDGs
 (Regionalized Value State Dependency Graphs). RVSDGs are a type of
 Intermediary Representation (IR) suitable for regularizing Python bytecode
 within Numba.
 
 The code in this repository is an implementation of the CFG restructuring
-algorithms in Bahmann2015, specifically those from section 4.1 and 4.2: namely
+algorithms in Bahmann 2015, specifically those from section 4.1 and 4.2: namely
 "loop restructuring" and "branch restructuring". These are interesting for
-Numba because they serve to clearly identify regions withing the Python
+Numba because they serve to clearly identify regions within the Python
 bytecode.
 
 ## dependencies
 
 * Python 3.11
 * graphviz
 * pyyaml
 
-As of 2023-03-06 you can create a conda env using the following:
+You can create a conda env using the following:
 
 ```
 conda env create -n numba-rvsdg python=3.11 python-graphviz
 conda activate numba-rvsdg
 pip install pyyaml
 ```
 
@@ -38,24 +51,23 @@
 
 ```
 numba_rvsdg
 ├── __init__.py
 ├── core
 │   ├── datastructures
 │   │   ├── basic_block.py  # BasicBlock implementation
-│   │   ├── block_map.py    # BlockMap implementation, maps labels to blocks
-│   │   ├── byte_flow.py    # ByteFlow implementation, BlockMap + bytecode
+│   │   ├── scfg.py         # SCFG implementation, maps names to blocks
+│   │   ├── byte_flow.py    # ByteFlow implementation, SCFG + bytecode
 │   │   ├── flow_info.py    # Converts program to ByteFlow
-│   │   └── labels.py       # Collection of Label classes
 │   ├── transformations.py  # Algorithms
 │   └── utils.py            # Miscellaneous utilities
 ├── networkx_vendored
 │   └── scc.py              # Strongly Connected Componets (loop detection)
 ├── rendering
-│   └── rendering.py        # Graphivz based rendering of BlockMaps
+│   └── rendering.py        # Graphivz based rendering of SCFGs
 ├── tests
 │   ├── simulator.py        # Simulator utility for running SCFGs
 │   ├── test_byteflow.py    # Testung ByteFlow and others
 │   ├── test_fig3.py        # Testing fig. 3 from Bahman2015
 │   ├── test_fig4.py        # Testing fig. 4 from Bahman2015
 │   ├── test_simulate.py    # Simulator based testing
 │   └── test_transforms.py  # Testing graph transformations
@@ -70,33 +82,27 @@
 restructuring" is the loop-restructured version and "branch-restructured" is
 the final form which includes closing, loop-restructuring and
 branch-restructuring.
 
 
 ```python
 # Example: for loop with branch and early exit
+
+from numba_rvsdg.rendering.rendering import render_func
+
 def foo(n):
     c = 0
     for i in range(n):
         c += 1
         if i == 100:
             break
     return c
 
-flow = ByteFlow.from_bytecode(foo)
-ByteFlowRenderer().render_byteflow(flow).view("initial")
-
-cflow = flow._join_returns()
-ByteFlowRenderer().render_byteflow(cflow).view("closed")
-
-lflow = cflow._restructure_loop()
-ByteFlowRenderer().render_byteflow(lflow).view("loop restructured")
+render_func(foo)
 
-bflow = lflow._restructure_branch()
-ByteFlowRenderer().render_byteflow(bflow).view("branch restructured")
 ```
 
 ![initial](docs/images/initial.png "initial")
 ![closed](docs/images/closed.png "closed")
 ![loop-restructured](docs/images/loop_restructured.png "loop-restructured")
 ![branch-restructured](docs/images/branch_restructured.png "branch-restructured")
```

### Comparing `numba_rvsdg-0.0.1/numba_rvsdg.egg-info/PKG-INFO` & `numba_rvsdg-0.0.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,43 +1,31 @@
-Metadata-Version: 2.1
-Name: numba-rvsdg
-Version: 0.0.1
-Summary: Numba Compatible RVSDG utilities
-Author-email: Numba Developers <none@none.none>
-License: BSD-2-Clause
-Keywords: numba
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # numba-rvsdg
 
 Numba compatible RVSDG (Regionalized Value State Dependence Graph)  utilities.
 
 ## about
 
 This repository contains Numba compatible utilities for working with RVSDGs
 (Regionalized Value State Dependency Graphs). RVSDGs are a type of
 Intermediary Representation (IR) suitable for regularizing Python bytecode
 within Numba.
 
 The code in this repository is an implementation of the CFG restructuring
-algorithms in Bahmann2015, specifically those from section 4.1 and 4.2: namely
+algorithms in Bahmann 2015, specifically those from section 4.1 and 4.2: namely
 "loop restructuring" and "branch restructuring". These are interesting for
-Numba because they serve to clearly identify regions withing the Python
+Numba because they serve to clearly identify regions within the Python
 bytecode.
 
 ## dependencies
 
 * Python 3.11
 * graphviz
 * pyyaml
 
-As of 2023-03-06 you can create a conda env using the following:
+You can create a conda env using the following:
 
 ```
 conda env create -n numba-rvsdg python=3.11 python-graphviz
 conda activate numba-rvsdg
 pip install pyyaml
 ```
 
@@ -50,24 +38,23 @@
 
 ```
 numba_rvsdg
 ├── __init__.py
 ├── core
 │   ├── datastructures
 │   │   ├── basic_block.py  # BasicBlock implementation
-│   │   ├── block_map.py    # BlockMap implementation, maps labels to blocks
-│   │   ├── byte_flow.py    # ByteFlow implementation, BlockMap + bytecode
+│   │   ├── scfg.py         # SCFG implementation, maps names to blocks
+│   │   ├── byte_flow.py    # ByteFlow implementation, SCFG + bytecode
 │   │   ├── flow_info.py    # Converts program to ByteFlow
-│   │   └── labels.py       # Collection of Label classes
 │   ├── transformations.py  # Algorithms
 │   └── utils.py            # Miscellaneous utilities
 ├── networkx_vendored
 │   └── scc.py              # Strongly Connected Componets (loop detection)
 ├── rendering
-│   └── rendering.py        # Graphivz based rendering of BlockMaps
+│   └── rendering.py        # Graphivz based rendering of SCFGs
 ├── tests
 │   ├── simulator.py        # Simulator utility for running SCFGs
 │   ├── test_byteflow.py    # Testung ByteFlow and others
 │   ├── test_fig3.py        # Testing fig. 3 from Bahman2015
 │   ├── test_fig4.py        # Testing fig. 4 from Bahman2015
 │   ├── test_simulate.py    # Simulator based testing
 │   └── test_transforms.py  # Testing graph transformations
@@ -82,33 +69,27 @@
 restructuring" is the loop-restructured version and "branch-restructured" is
 the final form which includes closing, loop-restructuring and
 branch-restructuring.
 
 
 ```python
 # Example: for loop with branch and early exit
+
+from numba_rvsdg.rendering.rendering import render_func
+
 def foo(n):
     c = 0
     for i in range(n):
         c += 1
         if i == 100:
             break
     return c
 
-flow = ByteFlow.from_bytecode(foo)
-ByteFlowRenderer().render_byteflow(flow).view("initial")
-
-cflow = flow._join_returns()
-ByteFlowRenderer().render_byteflow(cflow).view("closed")
-
-lflow = cflow._restructure_loop()
-ByteFlowRenderer().render_byteflow(lflow).view("loop restructured")
+render_func(foo)
 
-bflow = lflow._restructure_branch()
-ByteFlowRenderer().render_byteflow(bflow).view("branch restructured")
 ```
 
 ![initial](docs/images/initial.png "initial")
 ![closed](docs/images/closed.png "closed")
 ![loop-restructured](docs/images/loop_restructured.png "loop-restructured")
 ![branch-restructured](docs/images/branch_restructured.png "branch-restructured")
```

