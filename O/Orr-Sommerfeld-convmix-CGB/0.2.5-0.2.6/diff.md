# Comparing `tmp/orr_sommerfeld_convmix_cgb-0.2.5.tar.gz` & `tmp/orr_sommerfeld_convmix_cgb-0.2.6.tar.gz`

## Comparing `orr_sommerfeld_convmix_cgb-0.2.5.tar` & `orr_sommerfeld_convmix_cgb-0.2.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    12028 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.5/src/Orr_Sommerfeld_convmix_CGB/OS_CM.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.5/src/Orr_Sommerfeld_convmix_CGB/__init__.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.5/LICENSE
--rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.5/README.md
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     4190 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0    12028 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.6/src/Orr_Sommerfeld_convmix_CGB/OS_CM.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.6/src/Orr_Sommerfeld_convmix_CGB/__init__.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.6/LICENSE
+-rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.6/README.md
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.6/PKG-INFO
```

### Comparing `orr_sommerfeld_convmix_cgb-0.2.5/src/Orr_Sommerfeld_convmix_CGB/OS_CM.py` & `orr_sommerfeld_convmix_cgb-0.2.6/src/Orr_Sommerfeld_convmix_CGB/OS_CM.py`

 * *Files identical despite different names*

### Comparing `orr_sommerfeld_convmix_cgb-0.2.5/LICENSE` & `orr_sommerfeld_convmix_cgb-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `orr_sommerfeld_convmix_cgb-0.2.5/README.md` & `orr_sommerfeld_convmix_cgb-0.2.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # Orr-Sommerfeld-convmix-CGB Package
 It is a python package developed in order to solve the Orr Sommerfeld equations. It is free for the community and allows to calculate disturbances for one flow of interest: Mixed convection in vertical rectangular channels. These perturbations can be used to analyze the phenomenon of the laminar-turbulent transition. 
+
 ## Table of contents
 * [General info](#general-info)
 * [Technologies](#technologies)
 * [Installation](#installation)
 * [Examples](#examples)
 
 ## General info
```

### Comparing `orr_sommerfeld_convmix_cgb-0.2.5/pyproject.toml` & `orr_sommerfeld_convmix_cgb-0.2.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "Orr_Sommerfeld_convmix_CGB"
-version = "0.2.5"
+version = "0.2.6"
 authors = [
   { name="Pablo Szuban", email="pablo.szuban@ib.edu.ar" },
 ]
 description = "Paquete para cálculo de autovalores y autofunciones."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `orr_sommerfeld_convmix_cgb-0.2.5/PKG-INFO` & `orr_sommerfeld_convmix_cgb-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: Orr_Sommerfeld_convmix_CGB
-Version: 0.2.5
+Version: 0.2.6
 Summary: Paquete para cálculo de autovalores y autofunciones.
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Project-URL: Source Code, https://gitlab.com/mecom-cnea-os/orr-sommerfeld-convmix-cgb
 Author-email: Pablo Szuban <pablo.szuban@ib.edu.ar>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Orr-Sommerfeld-convmix-CGB Package
 It is a python package developed in order to solve the Orr Sommerfeld equations. It is free for the community and allows to calculate disturbances for one flow of interest: Mixed convection in vertical rectangular channels. These perturbations can be used to analyze the phenomenon of the laminar-turbulent transition. 
+
 ## Table of contents
 * [General info](#general-info)
 * [Technologies](#technologies)
 * [Installation](#installation)
 * [Examples](#examples)
 
 ## General info
```

