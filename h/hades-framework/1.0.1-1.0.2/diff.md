# Comparing `tmp/hades_framework-1.0.1.tar.gz` & `tmp/hades_framework-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hades_framework-1.0.1.tar", max compression
+gzip compressed data, was "hades_framework-1.0.2.tar", max compression
```

## Comparing `hades_framework-1.0.1.tar` & `hades_framework-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    11358 2023-06-22 17:21:12.746112 hades_framework-1.0.1/LICENSE.md
--rw-r--r--   0        0        0     7815 2023-06-22 17:21:12.746112 hades_framework-1.0.1/README.pypi.md
--rw-r--r--   0        0        0     1034 2023-06-22 17:21:12.814116 hades_framework-1.0.1/hades/__init__.py
--rw-r--r--   0        0        0      589 2023-06-22 17:21:12.814116 hades_framework-1.0.1/hades/core/__init__.py
--rw-r--r--   0        0        0     2516 2023-06-22 17:21:12.814116 hades_framework-1.0.1/hades/core/event.py
--rw-r--r--   0        0        0    12228 2023-06-22 17:21:12.814116 hades_framework-1.0.1/hades/core/hades.py
--rw-r--r--   0        0        0     7341 2023-06-22 17:21:12.814116 hades_framework-1.0.1/hades/core/process.py
--rw-r--r--   0        0        0     1255 2023-06-22 17:21:12.814116 hades_framework-1.0.1/hades/logging.py
--rw-r--r--   0        0        0     1222 2023-06-22 17:21:12.814116 hades_framework-1.0.1/hades/time/__init__.py
--rw-r--r--   0        0        0     1493 2023-06-22 17:21:12.814116 hades_framework-1.0.1/hades/time/day_steps.py
--rw-r--r--   0        0        0     1307 2023-06-22 17:21:12.814116 hades_framework-1.0.1/hades/time/event.py
--rw-r--r--   0        0        0     1086 2023-06-22 17:21:12.814116 hades_framework-1.0.1/hades/time/logging.py
--rw-r--r--   0        0        0     3866 2023-06-22 17:21:12.814116 hades_framework-1.0.1/hades/time/process.py
--rw-r--r--   0        0        0      589 2023-06-22 17:21:12.814116 hades_framework-1.0.1/hades/visualisation/__init__.py
--rw-r--r--   0        0        0     2284 2023-06-22 17:21:12.814116 hades_framework-1.0.1/hades/visualisation/networkx.py
--rw-r--r--   0        0        0     6344 2023-06-22 17:21:12.814116 hades_framework-1.0.1/hades/visualisation/websockets.py
--rw-r--r--   0        0        0     1807 2023-06-22 17:21:12.814116 hades_framework-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     8540 1970-01-01 00:00:00.000000 hades_framework-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-06-22 17:37:29.033846 hades_framework-1.0.2/LICENSE.md
+-rw-r--r--   0        0        0     7815 2023-06-22 17:37:29.033846 hades_framework-1.0.2/README.pypi.md
+-rw-r--r--   0        0        0     1034 2023-06-22 17:37:29.105846 hades_framework-1.0.2/hades/__init__.py
+-rw-r--r--   0        0        0      589 2023-06-22 17:37:29.105846 hades_framework-1.0.2/hades/core/__init__.py
+-rw-r--r--   0        0        0     2516 2023-06-22 17:37:29.105846 hades_framework-1.0.2/hades/core/event.py
+-rw-r--r--   0        0        0    12228 2023-06-22 17:37:29.105846 hades_framework-1.0.2/hades/core/hades.py
+-rw-r--r--   0        0        0     7341 2023-06-22 17:37:29.105846 hades_framework-1.0.2/hades/core/process.py
+-rw-r--r--   0        0        0     1255 2023-06-22 17:37:29.105846 hades_framework-1.0.2/hades/logging.py
+-rw-r--r--   0        0        0     1222 2023-06-22 17:37:29.105846 hades_framework-1.0.2/hades/time/__init__.py
+-rw-r--r--   0        0        0     1493 2023-06-22 17:37:29.105846 hades_framework-1.0.2/hades/time/day_steps.py
+-rw-r--r--   0        0        0     1307 2023-06-22 17:37:29.105846 hades_framework-1.0.2/hades/time/event.py
+-rw-r--r--   0        0        0     1086 2023-06-22 17:37:29.105846 hades_framework-1.0.2/hades/time/logging.py
+-rw-r--r--   0        0        0     3866 2023-06-22 17:37:29.105846 hades_framework-1.0.2/hades/time/process.py
+-rw-r--r--   0        0        0      589 2023-06-22 17:37:29.105846 hades_framework-1.0.2/hades/visualisation/__init__.py
+-rw-r--r--   0        0        0     2284 2023-06-22 17:37:29.105846 hades_framework-1.0.2/hades/visualisation/networkx.py
+-rw-r--r--   0        0        0     6344 2023-06-22 17:37:29.105846 hades_framework-1.0.2/hades/visualisation/websockets.py
+-rw-r--r--   0        0        0     1807 2023-06-22 17:37:29.105846 hades_framework-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     8540 1970-01-01 00:00:00.000000 hades_framework-1.0.2/PKG-INFO
```

### Comparing `hades_framework-1.0.1/LICENSE.md` & `hades_framework-1.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hades_framework-1.0.1/README.pypi.md` & `hades_framework-1.0.2/README.pypi.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <p align="center">
 
 <img src="https://raw.githubusercontent.com/ki-oss/hades/main/docs/img/hades_black.png" alt="Hades Logo">
 
 </p>
 <p align="center">
-<img src="https://img.shields.io/badge/version-1.0.0-blue" alt="version">
+<img src="https://img.shields.io/badge/version-1.0.2-blue" alt="version">
 <img src="https://img.shields.io/badge/License-Apache 2.0-blue.svg" alt="version">
 
 </p>
 <p align="center">
     <b>HADES</b> <i>(HADES Asynchronous Discrete-Event Simulation)</i> is a small, user friendly framework for creating simulations in python!
 </p>
 
@@ -28,20 +28,20 @@
 ```
 
 ## Usage
 Using the Hades Framework is as simple as creating your custom `Process`es and `Event`s, registering them in the simulation, and letting Hades take care of the rest.
 
 Here are some of the fun things you might do with it:
 
-* [Boids and Websockets](https://github.io/ki-oss/hades/examples/boids) - The classic Boids simulation with canvas and d3.js visualisation via websockets.
+* [Boids and Websockets](https://ki-oss.github.io/hades/examples/boids) - The classic Boids simulation with canvas and d3.js visualisation via websockets.
     ![boids example](https://raw.githubusercontent.com/ki-oss/hades/main/docs/img/boids.gif)
-* [Multi Agent LLM Storytelling](https://github.io/ki-oss/hades/examples/multi) -  Retelling the Odyssey with LLMs - demonstrates the highly IO bound stuff hades is good at. Some output:
+* [Multi Agent LLM Storytelling](https://ki-oss.github.io/hades/examples/multi) -  Retelling the Odyssey with LLMs - demonstrates the highly IO bound stuff hades is good at. Some output:
     >   "He remembered the sea nymph who had helped him before and realized that having allies like her was crucial to his success. 
         He also continued to use his technological knowledge to stay ahead of Poseidon's wrath, utilizing his drone and sonar to navigate the waters safely."
-* [Battery charging station](https://github.io/ki-oss/hades/examples/battery-charging-station) - to help compare what building a simulation looks with `simpy` vs `hades`
+* [Battery charging station](https://ki-oss.github.io/hades/examples/battery-charging-station) - to help compare what building a simulation looks with `simpy` vs `hades`
 
 Here is a very simple example where we simulate Zeus sending lightning bolts and Poseidon creating storms, both potentially affecting the life of Odysseus:
 
 ```python
 import asyncio
 from enum import Enum
```

### Comparing `hades_framework-1.0.1/hades/__init__.py` & `hades_framework-1.0.2/hades/__init__.py`

 * *Files identical despite different names*

### Comparing `hades_framework-1.0.1/hades/core/__init__.py` & `hades_framework-1.0.2/hades/core/__init__.py`

 * *Files identical despite different names*

### Comparing `hades_framework-1.0.1/hades/core/event.py` & `hades_framework-1.0.2/hades/core/event.py`

 * *Files identical despite different names*

### Comparing `hades_framework-1.0.1/hades/core/hades.py` & `hades_framework-1.0.2/hades/core/hades.py`

 * *Files identical despite different names*

### Comparing `hades_framework-1.0.1/hades/core/process.py` & `hades_framework-1.0.2/hades/core/process.py`

 * *Files identical despite different names*

### Comparing `hades_framework-1.0.1/hades/logging.py` & `hades_framework-1.0.2/hades/logging.py`

 * *Files identical despite different names*

### Comparing `hades_framework-1.0.1/hades/time/__init__.py` & `hades_framework-1.0.2/hades/time/__init__.py`

 * *Files identical despite different names*

### Comparing `hades_framework-1.0.1/hades/time/day_steps.py` & `hades_framework-1.0.2/hades/time/day_steps.py`

 * *Files identical despite different names*

### Comparing `hades_framework-1.0.1/hades/time/event.py` & `hades_framework-1.0.2/hades/time/event.py`

 * *Files identical despite different names*

### Comparing `hades_framework-1.0.1/hades/time/logging.py` & `hades_framework-1.0.2/hades/time/logging.py`

 * *Files identical despite different names*

### Comparing `hades_framework-1.0.1/hades/time/process.py` & `hades_framework-1.0.2/hades/time/process.py`

 * *Files identical despite different names*

### Comparing `hades_framework-1.0.1/hades/visualisation/__init__.py` & `hades_framework-1.0.2/hades/visualisation/__init__.py`

 * *Files identical despite different names*

### Comparing `hades_framework-1.0.1/hades/visualisation/networkx.py` & `hades_framework-1.0.2/hades/visualisation/networkx.py`

 * *Files identical despite different names*

### Comparing `hades_framework-1.0.1/hades/visualisation/websockets.py` & `hades_framework-1.0.2/hades/visualisation/websockets.py`

 * *Files identical despite different names*

### Comparing `hades_framework-1.0.1/pyproject.toml` & `hades_framework-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hades-framework"
-version = "1.0.1"
+version = "1.0.2"
 description = "Hades Asynchronous Discrete-Event Simulation"
 authors = ["Ki Insurance Team", "Reuben Thomas-Davis <Reuben.Thomas-Davis@ki-insurance.com>", "Keith Kam <keith.kam@accenture.com>"]
 license = "Apache License 2.0"
 readme = "README.pypi.md"
 packages = [
     {include="hades"}
 ]
```

### Comparing `hades_framework-1.0.1/PKG-INFO` & `hades_framework-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hades-framework
-Version: 1.0.1
+Version: 1.0.2
 Summary: Hades Asynchronous Discrete-Event Simulation
 License: Apache-2.0
 Author: Ki Insurance Team
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -19,15 +19,15 @@
 
 <p align="center">
 
 <img src="https://raw.githubusercontent.com/ki-oss/hades/main/docs/img/hades_black.png" alt="Hades Logo">
 
 </p>
 <p align="center">
-<img src="https://img.shields.io/badge/version-1.0.0-blue" alt="version">
+<img src="https://img.shields.io/badge/version-1.0.2-blue" alt="version">
 <img src="https://img.shields.io/badge/License-Apache 2.0-blue.svg" alt="version">
 
 </p>
 <p align="center">
     <b>HADES</b> <i>(HADES Asynchronous Discrete-Event Simulation)</i> is a small, user friendly framework for creating simulations in python!
 </p>
 
@@ -46,20 +46,20 @@
 ```
 
 ## Usage
 Using the Hades Framework is as simple as creating your custom `Process`es and `Event`s, registering them in the simulation, and letting Hades take care of the rest.
 
 Here are some of the fun things you might do with it:
 
-* [Boids and Websockets](https://github.io/ki-oss/hades/examples/boids) - The classic Boids simulation with canvas and d3.js visualisation via websockets.
+* [Boids and Websockets](https://ki-oss.github.io/hades/examples/boids) - The classic Boids simulation with canvas and d3.js visualisation via websockets.
     ![boids example](https://raw.githubusercontent.com/ki-oss/hades/main/docs/img/boids.gif)
-* [Multi Agent LLM Storytelling](https://github.io/ki-oss/hades/examples/multi) -  Retelling the Odyssey with LLMs - demonstrates the highly IO bound stuff hades is good at. Some output:
+* [Multi Agent LLM Storytelling](https://ki-oss.github.io/hades/examples/multi) -  Retelling the Odyssey with LLMs - demonstrates the highly IO bound stuff hades is good at. Some output:
     >   "He remembered the sea nymph who had helped him before and realized that having allies like her was crucial to his success. 
         He also continued to use his technological knowledge to stay ahead of Poseidon's wrath, utilizing his drone and sonar to navigate the waters safely."
-* [Battery charging station](https://github.io/ki-oss/hades/examples/battery-charging-station) - to help compare what building a simulation looks with `simpy` vs `hades`
+* [Battery charging station](https://ki-oss.github.io/hades/examples/battery-charging-station) - to help compare what building a simulation looks with `simpy` vs `hades`
 
 Here is a very simple example where we simulate Zeus sending lightning bolts and Poseidon creating storms, both potentially affecting the life of Odysseus:
 
 ```python
 import asyncio
 from enum import Enum
```

