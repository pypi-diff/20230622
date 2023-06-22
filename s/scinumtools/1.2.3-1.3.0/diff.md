# Comparing `tmp/scinumtools-1.2.3.tar.gz` & `tmp/scinumtools-1.3.0.tar.gz`

## Comparing `scinumtools-1.2.3.tar` & `scinumtools-1.3.0.tar`

### file list

```diff
@@ -1,29 +1,37 @@
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-1.2.3/requirements.txt
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 scinumtools-1.2.3/.github/workflows/pytest.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 scinumtools-1.2.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 scinumtools-1.2.3/src/scinumtools/__init__.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 scinumtools-1.2.3/src/scinumtools/data/CachingClass.py
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 scinumtools-1.2.3/src/scinumtools/data/ImageClass.py
--rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 scinumtools-1.2.3/src/scinumtools/data/PlottingClass.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 scinumtools-1.2.3/src/scinumtools/data/__init__.py
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 scinumtools-1.2.3/src/scinumtools/phys/ConstantsClass.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 scinumtools-1.2.3/src/scinumtools/phys/__init__.py
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 scinumtools-1.2.3/src/scinumtools/phys/units/DIP_Solver_Units.py
--rw-r--r--   0        0        0     9216 2020-02-02 00:00:00.000000 scinumtools-1.2.3/src/scinumtools/phys/units/QuantityClass.py
--rw-r--r--   0        0        0    10693 2020-02-02 00:00:00.000000 scinumtools-1.2.3/src/scinumtools/phys/units/UnitList.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-1.2.3/src/scinumtools/phys/units/__init__.py
--rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 scinumtools-1.2.3/src/scinumtools/stats/StopwatchClass.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 scinumtools-1.2.3/src/scinumtools/stats/__init__.py
--rw-r--r--   0        0        0     5397 2020-02-02 00:00:00.000000 scinumtools-1.2.3/src/scinumtools/structs/CollectorClass.py
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 scinumtools-1.2.3/src/scinumtools/structs/ParameterClass.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 scinumtools-1.2.3/src/scinumtools/structs/__init__.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 scinumtools-1.2.3/tests/cached_data.npy
--rw-r--r--   0        0        0     6211 2020-02-02 00:00:00.000000 scinumtools-1.2.3/tests/test_data.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 scinumtools-1.2.3/tests/test_physics.py
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 scinumtools-1.2.3/tests/test_stats.py
--rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 scinumtools-1.2.3/tests/test_struct.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 scinumtools-1.2.3/tests/test_units.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 scinumtools-1.2.3/.gitignore
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 scinumtools-1.2.3/README.md
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 scinumtools-1.2.3/pyproject.toml
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 scinumtools-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-1.3.0/requirements.txt
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 scinumtools-1.3.0/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 scinumtools-1.3.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 scinumtools-1.3.0/src/scinumtools/__init__.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 scinumtools-1.3.0/src/scinumtools/data/CachingClass.py
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 scinumtools-1.3.0/src/scinumtools/data/ImageClass.py
+-rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 scinumtools-1.3.0/src/scinumtools/data/PlottingClass.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 scinumtools-1.3.0/src/scinumtools/data/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scinumtools-1.3.0/src/scinumtools/math/__init__.py
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 scinumtools-1.3.0/src/scinumtools/math/solver/AtomClass.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 scinumtools-1.3.0/src/scinumtools/math/solver/ExpressionClass.py
+-rw-r--r--   0        0        0     7525 2020-02-02 00:00:00.000000 scinumtools-1.3.0/src/scinumtools/math/solver/OperatorClass.py
+-rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 scinumtools-1.3.0/src/scinumtools/math/solver/SolverClass.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 scinumtools-1.3.0/src/scinumtools/math/solver/TokensClass.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 scinumtools-1.3.0/src/scinumtools/math/solver/__init__.py
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 scinumtools-1.3.0/src/scinumtools/phys/ConstantsClass.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 scinumtools-1.3.0/src/scinumtools/phys/__init__.py
+-rw-r--r--   0        0        0     7312 2020-02-02 00:00:00.000000 scinumtools-1.3.0/src/scinumtools/phys/units/QuantityClass.py
+-rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 scinumtools-1.3.0/src/scinumtools/phys/units/UnitConverters.py
+-rw-r--r--   0        0        0    10140 2020-02-02 00:00:00.000000 scinumtools-1.3.0/src/scinumtools/phys/units/UnitList.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-1.3.0/src/scinumtools/phys/units/__init__.py
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 scinumtools-1.3.0/src/scinumtools/stats/StopwatchClass.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 scinumtools-1.3.0/src/scinumtools/stats/__init__.py
+-rw-r--r--   0        0        0     5397 2020-02-02 00:00:00.000000 scinumtools-1.3.0/src/scinumtools/structs/CollectorClass.py
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 scinumtools-1.3.0/src/scinumtools/structs/ParameterClass.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 scinumtools-1.3.0/src/scinumtools/structs/__init__.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 scinumtools-1.3.0/tests/cached_data.npy
+-rw-r--r--   0        0        0     6088 2020-02-02 00:00:00.000000 scinumtools-1.3.0/tests/test_data.py
+-rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 scinumtools-1.3.0/tests/test_math.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 scinumtools-1.3.0/tests/test_physics.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 scinumtools-1.3.0/tests/test_stats.py
+-rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 scinumtools-1.3.0/tests/test_struct.py
+-rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 scinumtools-1.3.0/tests/test_units.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 scinumtools-1.3.0/.gitignore
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 scinumtools-1.3.0/README.md
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 scinumtools-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 scinumtools-1.3.0/PKG-INFO
```

### Comparing `scinumtools-1.2.3/.github/workflows/python-publish.yml` & `scinumtools-1.3.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `scinumtools-1.2.3/src/scinumtools/data/ImageClass.py` & `scinumtools-1.3.0/src/scinumtools/data/ImageClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.2.3/src/scinumtools/data/PlottingClass.py` & `scinumtools-1.3.0/src/scinumtools/data/PlottingClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.2.3/src/scinumtools/phys/ConstantsClass.py` & `scinumtools-1.3.0/src/scinumtools/phys/ConstantsClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.2.3/src/scinumtools/phys/units/UnitList.py` & `scinumtools-1.3.0/src/scinumtools/phys/units/UnitList.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,124 +1,104 @@
-import numpy as np
-
-def convert_celsius(unit1, unit2):
-    pass
-
+import numpy as np        
+        
 UnitPrefixes = {
-    'Y':        (1.0,        [ 24, 0, 0, 0, 0, 0, 0, 0, 0],  '1e24',                   'yotta'            ), 
-    'Z':        (1.0,        [ 21, 0, 0, 0, 0, 0, 0, 0, 0],  '1e21',                   'zetta'            ), 
-    'E':        (1.0,        [ 18, 0, 0, 0, 0, 0, 0, 0, 0],  '1e18',                   'exa'              ), 
-    'P':        (1.0,        [ 15, 0, 0, 0, 0, 0, 0, 0, 0],  '1e15',                   'peta'             ), 
-    'T':        (1.0,        [ 12, 0, 0, 0, 0, 0, 0, 0, 0],  '1e12',                   'tera'             ), 
-    'G':        (1.0,        [  9, 0, 0, 0, 0, 0, 0, 0, 0],  '1e9',                    'giga'             ), 
-    'M':        (1.0,        [  6, 0, 0, 0, 0, 0, 0, 0, 0],  '1e6',                    'mega'             ), 
-    'k':        (1.0,        [  3, 0, 0, 0, 0, 0, 0, 0, 0],  '1e3',                    'kilo'             ), 
-    'h':        (1.0,        [  2, 0, 0, 0, 0, 0, 0, 0, 0],  '1e2',                    'hecto'            ), 
-    'da':       (1.0,        [  1, 0, 0, 0, 0, 0, 0, 0, 0],  '1e1',                    'deka'             ), 
-    'd':        (1.0,        [ -1, 0, 0, 0, 0, 0, 0, 0, 0],  '1e-1',                   'deci'             ), 
-    'c':        (1.0,        [ -2, 0, 0, 0, 0, 0, 0, 0, 0],  '1e-2',                   'centi'            ), 
-    'm':        (1.0,        [ -3, 0, 0, 0, 0, 0, 0, 0, 0],  '1e-3',                   'milli'            ), 
-    'u':        (1.0,        [ -6, 0, 0, 0, 0, 0, 0, 0, 0],  '1e-6',                   'micro'            ), 
-    'n':        (1.0,        [ -9, 0, 0, 0, 0, 0, 0, 0, 0],  '1e-9',                   'nano'             ), 
-    'p':        (1.0,        [-12, 0, 0, 0, 0, 0, 0, 0, 0],  '1e-12',                  'pico'             ), 
-    'f':        (1.0,        [-15, 0, 0, 0, 0, 0, 0, 0, 0],  '1e-15',                  'femto'            ), 
-    'a':        (1.0,        [-18, 0, 0, 0, 0, 0, 0, 0, 0],  '1e-18',                  'atto'             ), 
-    'z':        (1.0,        [-21, 0, 0, 0, 0, 0, 0, 0, 0],  '1e-21',                  'zepto'            ), 
-    'y':        (1.0,        [-24, 0, 0, 0, 0, 0, 0, 0, 0],  '1e-24',                  'yocto'            ), 
+    'Y':        (1.0e24,         [ 0, 0, 0, 0, 0, 0, 0, 0],  '1e24',                   'yotta'            ), 
+    'Z':        (1.0e21,         [ 0, 0, 0, 0, 0, 0, 0, 0],  '1e21',                   'zetta'            ), 
+    'E':        (1.0e18,         [ 0, 0, 0, 0, 0, 0, 0, 0],  '1e18',                   'exa'              ), 
+    'P':        (1.0e15,         [ 0, 0, 0, 0, 0, 0, 0, 0],  '1e15',                   'peta'             ), 
+    'T':        (1.0e12,         [ 0, 0, 0, 0, 0, 0, 0, 0],  '1e12',                   'tera'             ), 
+    'G':        (1.0e9,          [ 0, 0, 0, 0, 0, 0, 0, 0],  '1e9',                    'giga'             ), 
+    'M':        (1.0e6,          [ 0, 0, 0, 0, 0, 0, 0, 0],  '1e6',                    'mega'             ), 
+    'k':        (1.0e3,          [ 0, 0, 0, 0, 0, 0, 0, 0],  '1e3',                    'kilo'             ), 
+    'h':        (1.0e2,          [ 0, 0, 0, 0, 0, 0, 0, 0],  '1e2',                    'hecto'            ), 
+    'da':       (1.0e1,          [ 0, 0, 0, 0, 0, 0, 0, 0],  '1e1',                    'deka'             ), 
+    'd':        (1.0e-1,         [ 0, 0, 0, 0, 0, 0, 0, 0],  '1e-1',                   'deci'             ), 
+    'c':        (1.0e-2,         [ 0, 0, 0, 0, 0, 0, 0, 0],  '1e-2',                   'centi'            ), 
+    'm':        (1.0e-3,         [ 0, 0, 0, 0, 0, 0, 0, 0],  '1e-3',                   'milli'            ), 
+    'u':        (1.0e-6,         [ 0, 0, 0, 0, 0, 0, 0, 0],  '1e-6',                   'micro'            ), 
+    'n':        (1.0e-9,         [ 0, 0, 0, 0, 0, 0, 0, 0],  '1e-9',                   'nano'             ), 
+    'p':        (1.0e-12,        [ 0, 0, 0, 0, 0, 0, 0, 0],  '1e-12',                  'pico'             ), 
+    'f':        (1.0e-15,        [ 0, 0, 0, 0, 0, 0, 0, 0],  '1e-15',                  'femto'            ), 
+    'a':        (1.0e-18,        [ 0, 0, 0, 0, 0, 0, 0, 0],  '1e-18',                  'atto'             ), 
+    'z':        (1.0e-21,        [ 0, 0, 0, 0, 0, 0, 0, 0],  '1e-21',                  'zepto'            ), 
+    'y':        (1.0e-24,        [ 0, 0, 0, 0, 0, 0, 0, 0],  '1e-24',                  'yocto'            ), 
 }                                                                                        
             
-UnitBase = ['1e','m','g','s','K','C','cd','mol','rad']
+UnitBase = ['m','g','s','K','C','cd','mol','rad']
             
 UnitStandard = {
-    # order
-    '1e':       (1.0,        [  1, 0, 0, 0, 0, 0, 0, 0, 0],  None,                     'power of ten'     ),
-    # physical units                            
-    'm':        (1.0,        [  0, 1, 0, 0, 0, 0, 0, 0, 0],  None,                     'meter'            ),
-    'g':        (1.0,        [  0, 0, 1, 0, 0, 0, 0, 0, 0],  None,                     'gram'             ),
-    's':        (1.0,        [  0, 0, 0, 1, 0, 0, 0, 0, 0],  None,                     'second'           ),
-    'K':        (1.0,        [  0, 0, 0, 0, 1, 0, 0, 0, 0],  None,                     'kelvin'           ),
-    'C':        (1.0,        [  0, 0, 0, 0, 0, 1, 0, 0, 0],  None,                     'coulomb'          ),
-    'cd':       (1.0,        [  0, 0, 0, 0, 0, 0, 1, 0, 0],  None,                     'candela'          ),
-    # numerical units
-    'mol':      (1.0,        [  0, 0, 0, 0, 0, 0, 0, 1, 0],  None,                     'mole'             ),
-    'rad':      (1.0,        [  0, 0, 0, 0, 0, 0, 0, 0, 1],  None,                     'radian'           ),
-    # Derived units
-    # SI units                                                                                
-    'sr':       (1.0,        [  0, 0, 0, 0, 0, 0, 0, 0, 2],  'rad2',                   'steradian'        ),
-    'Hz':       (1.0,        [  0, 0, 0,-1, 0, 0, 0, 0, 0],  's-1',                    'hertz'            ),
-    'N':        (1.0,        [  3, 1, 1,-2, 0, 0, 0, 0, 0],  'kg*m/s2',                'newton'           ),
-    'Pa':       (1.0,        [  3,-1, 1,-2, 0, 0, 0, 0, 0],  'N/m2',                   'pascal'           ),
-    'J':        (1.0,        [  3, 2, 1,-2, 0, 0, 0, 0, 0],  'N*m',                    'joule'            ),
-    'W':        (1.0,        [  3, 2, 1,-3, 0, 0, 0, 0, 0],  'J/s',                    'watt'             ),
-    'A':        (1.0,        [  0, 0, 0,-1, 0, 1, 0, 0, 0],  'C/s',                    'ampere'           ),
-    'V':        (1.0,        [  3, 2, 1,-2, 0,-1, 0, 0, 0],  'J/C',                    'volt'             ),
-    'F':        (1.0,        [ -3,-2,-1, 2, 0, 2, 0, 0, 0],  'C/V',                    'farad'            ),
-    'Ohm':      (1.0,        [  3, 2, 1,-1, 0,-2, 0, 0, 0],  'V/A',                    'ohm'              ),
-    'S':        (1.0,        [ -3,-2,-1, 1, 0, 2, 0, 0, 0],  'Ohm-1',                  'siemens'          ),
-    'Wb':       (1.0,        [  3, 2, 1,-1, 0,-1, 0, 0, 0],  'V*s',                    'weber'            ),
-    'T':        (1.0,        [  3, 0, 1,-1, 0,-1, 0, 0, 0],  'Wb/m2',                  'tesla'            ),
-    'H':        (1.0,        [  3, 2, 1, 0, 0,-2, 0, 0, 0],  'Wb/A',                   'henry'            ),
-    'lm':       (1.0,        [  0, 0, 0, 0, 0, 0, 1, 0, 2],  'cd*sr',                  'lumen'            ),
-    'lx':       (1.0,        [  0,-2, 0, 0, 0, 0, 1, 0, 2],  'lm/m2',                  'lux'              ),
-    'Bq':       (1.0,        [  0, 0, 0,-1, 0, 0, 0, 0, 0],  's-1',                    'becquerel'        ),
-    'Gy':       (1.0,        [  0, 2, 0,-2, 0, 0, 0, 0, 0],  'J/kg',                   'gray'             ),
-    'Sv':       (1.0,        [  0, 2, 0,-2, 0, 0, 0, 0, 0],  'J/kg',                   'sivert'           ),
+    # physical units                        
+    'm':        (1.0,            [ 1, 0, 0, 0, 0, 0, 0, 0],  None,                     'meter'            ),
+    'g':        (1.0,            [ 0, 1, 0, 0, 0, 0, 0, 0],  None,                     'gram'             ),
+    's':        (1.0,            [ 0, 0, 1, 0, 0, 0, 0, 0],  None,                     'second'           ),
+    'K':        (1.0,            [ 0, 0, 0, 1, 0, 0, 0, 0],  None,                     'kelvin'           ),
+    'C':        (1.0,            [ 0, 0, 0, 0, 1, 0, 0, 0],  None,                     'coulomb'          ),
+    'cd':       (1.0,            [ 0, 0, 0, 0, 0, 1, 0, 0],  None,                     'candela'          ),
+    # numerical units            
+    'mol':      (1.0,            [ 0, 0, 0, 0, 0, 0, 1, 0],  None,                     'mole'             ),
+    'rad':      (1.0,            [ 0, 0, 0, 0, 0, 0, 0, 1],  None,                     'radian'           ),
+    # Derived units              
+    # SI units                                                                                    
+    'sr':       (1.0e0,          [ 0, 0, 0, 0, 0, 0, 0, 2],  'rad2',                   'steradian'        ),
+    'Hz':       (1.0e0,          [ 0, 0,-1, 0, 0, 0, 0, 0],  's-1',                    'hertz'            ),
+    'N':        (1.0e3,          [ 1, 1,-2, 0, 0, 0, 0, 0],  'kg*m/s2',                'newton'           ),
+    'Pa':       (1.0e3,          [-1, 1,-2, 0, 0, 0, 0, 0],  'N/m2',                   'pascal'           ),
+    'J':        (1.0e3,          [ 2, 1,-2, 0, 0, 0, 0, 0],  'N*m',                    'joule'            ),
+    'W':        (1.0e3,          [ 2, 1,-3, 0, 0, 0, 0, 0],  'J/s',                    'watt'             ),
+    'A':        (1.0e0,          [ 0, 0,-1, 0, 1, 0, 0, 0],  'C/s',                    'ampere'           ),
+    'V':        (1.0e3,          [ 2, 1,-2, 0,-1, 0, 0, 0],  'J/C',                    'volt'             ),
+    'F':        (1.0e-3,         [-2,-1, 2, 0, 2, 0, 0, 0],  'C/V',                    'farad'            ),
+    'Ohm':      (1.0e3,          [ 2, 1,-1, 0,-2, 0, 0, 0],  'V/A',                    'ohm'              ),
+    'S':        (1.0e-3,         [-2,-1, 1, 0, 2, 0, 0, 0],  'Ohm-1',                  'siemens'          ),
+    'Wb':       (1.0e3,          [ 2, 1,-1, 0,-1, 0, 0, 0],  'V*s',                    'weber'            ),
+    'T':        (1.0e3,          [ 0, 1,-1, 0,-1, 0, 0, 0],  'Wb/m2',                  'tesla'            ),
+    'H':        (1.0e3,          [ 2, 1, 0, 0,-2, 0, 0, 0],  'Wb/A',                   'henry'            ),
+    'lm':       (1.0e0,          [ 0, 0, 0, 0, 0, 1, 0, 2],  'cd*sr',                  'lumen'            ),
+    'lx':       (1.0e0,          [-2, 0, 0, 0, 0, 1, 0, 2],  'lm/m2',                  'lux'              ),
+    'Bq':       (1.0e0,          [ 0, 0,-1, 0, 0, 0, 0, 0],  's-1',                    'becquerel'        ),
+    'Gy':       (1.0e0,          [ 2, 0,-2, 0, 0, 0, 0, 0],  'J/kg',                   'gray'             ),
+    'Sv':       (1.0e0,          [ 2, 0,-2, 0, 0, 0, 0, 0],  'J/kg',                   'sivert'           ),
     # CGS units                                                                               
-    'dyn':      (1.0,        [ -2, 1, 1,-2, 0, 0, 0, 0, 0],  'g*cm/s2',                'dyne'             ),
-    'erg':      (1.0,        [ -4, 2, 1,-2, 0, 0, 0, 0, 0],  'dyn*cm',                 'erg'              ),
-    'G':        (1.0,        [ -1, 0, 1,-1, 0,-1, 0, 0, 0],  '1e-4*T',                 'Gauss'            ),
-    # other derived units                                                                     
-    'deg':      (1.745329,   [ -2, 0, 0, 0, 0, 0, 0, 0, 1],  '2*[pi]*rad/360',         'angle degree'     ),
-    "'":        (2.908882,   [ -4, 0, 0, 0, 0, 0, 0, 0, 1],  'deg/60',                 'angle minute'     ),
-    "''":       (4.848137,   [ -6, 0, 0, 0, 0, 0, 0, 0, 1],  "'/60",                   'angle second'     ),
-    'l':        (1,          [ -3, 3, 0, 0, 0, 0, 0, 0, 0],  'dm3',                    'liter'            ),
-    'L':        (1,          [ -3, 3, 0, 0, 0, 0, 0, 0, 0],  'l',                      'liter'            ),
-    'ar':       (1,          [  2, 2, 0, 0, 0, 0, 0, 0, 0],  '100*m2',                 'are'              ),
-    'min':      (6.0,        [  1, 0, 0, 1, 0, 0, 0, 0, 0],  '60*s',                   'minute'           ),
-    'h':        (3.6,        [  3, 0, 0, 1, 0, 0, 0, 0, 0],  '60*min',                 'hour'             ),
-    'd':        (8.64,       [  4, 0, 0, 1, 0, 0, 0, 0, 0],  '24*h',                   'day'              ),
-    'a_t':      (3.155693,   [  7, 0, 0, 1, 0, 0, 0, 0, 0],  '365.24219*d',            'tropical year'    ),
-    'a_j':      (3.155760,   [  7, 0, 0, 1, 0, 0, 0, 0, 0],  '365.25*d',               'Julian year'      ),
-    'a_g':      (3.155695,   [  7, 0, 0, 1, 0, 0, 0, 0, 0],  '365.2425*d',             'Gregorian year'   ),
-    'a':        (3.155760,   [  7, 0, 0, 1, 0, 0, 0, 0, 0],  'a_j',                    'year'             ),
-    'eV':       (1.60217733, [-16, 2, 1,-2, 0, 0, 0, 0, 0],  '[e]*V',                  'electronvolt'     ),
-    'au':       (1.49597870, [ 11, 1, 0, 0, 0, 0, 0, 0, 0],  '149597.870691*Mm',       'astr. unit'       ),
-    'AU':       (1.49597870, [ 11, 1, 0, 0, 0, 0, 0, 0, 0],  'au',                     'astr. unit'       ),
-    # natural units
-    '[c]':      (2.99792458, [  8, 1, 0,-1, 0, 0, 0, 0, 0],  '299792458*m/s',          'velocity of light'),
-    '[h]':      (6.626076,   [-31, 2, 1,-1, 0, 0, 0, 0, 0],  '6.6260755e-34*J*s',      'Planck const.'    ),
-    '[k]':      (1.380658,   [-20, 2, 1,-2,-1, 0, 0, 0, 0],  '1.380658e-23*J/K',       'Boltzmann const.' ),
-    '[eps_0]':  (8.854188,   [-15,-3,-1, 2, 0, 2, 0, 0, 0],  '8.854187817e-12*F/m',    'permit. of vac.'  ),
-    '[mu_0]':   (1.256637,   [ -3, 1, 1, 0, 0,-2, 0, 0, 0],  '4*[pi]*1e-7*N/A2',       'permeab. of vac.' ),
-    '[e]':      (1.60217733, [-19, 0, 0, 0, 0, 1, 0, 0, 0],  '1.60217733e-19*C',       'elem. charge'     ),
-    '[m_e]':    (9.109390,   [-28, 0, 1, 0, 0, 0, 0, 0, 0],  '9.1093897e-28*g',        'electron mass'    ),
-    '[m_p]':    (1.672623,   [-24, 0, 1, 0, 0, 0, 0, 0, 0],  '1.6726231e-24*g',        'proton mass'      ),
-    '[G]':      (6.672590,   [-14, 3,-1,-2, 0, 0, 0, 0, 0],  '6.67259e-11*m3/(kg*s2)', 'grav. const.'     ),
-    '[g]':      (9.806650,   [  0, 1, 0,-2, 0, 0, 0, 0, 0],  '9.80665*m/s2',           'grav. accel.'     ),
-    'atm':      (1.013250,   [  8,-1, 1,-2, 0, 0, 0, 0, 0],  '101325*Pa',              'atm. pressure'    ),
-    'ly':       (9.460730,   [ 15, 1, 0, 0, 0, 0, 0, 0, 0],  '[c]*a_j',                'light-year'       ),
+    'dyn':      (1.0e-2,         [ 1, 1,-2, 0, 0, 0, 0, 0],  'g*cm/s2',                'dyne'             ),
+    'erg':      (1.0e-4,         [ 2, 1,-2, 0, 0, 0, 0, 0],  'dyn*cm',                 'erg'              ),
+    'G':        (1.0e-1,         [ 0, 1,-1, 0,-1, 0, 0, 0],  '1e-4*T',                 'Gauss'            ),
+    # other derived units                                                                        
+    'deg':      (1.7453292e-2,   [ 0, 0, 0, 0, 0, 0, 0, 1],  '2*[pi]*rad/360',         'angle degree'     ),
+    "'":        (2.908882e-4,    [ 0, 0, 0, 0, 0, 0, 0, 1],  'deg/60',                 'angle minute'     ),
+    "''":       (4.848137e-6,    [ 0, 0, 0, 0, 0, 0, 0, 1],  "'/60",                   'angle second'     ),
+    'l':        (1e-3,           [ 3, 0, 0, 0, 0, 0, 0, 0],  'dm3',                    'liter'            ),
+    'L':        (1e-3,           [ 3, 0, 0, 0, 0, 0, 0, 0],  'l',                      'liter'            ),
+    'ar':       (1e2,            [ 2, 0, 0, 0, 0, 0, 0, 0],  '100*m2',                 'are'              ),
+    'min':      (6.0e1,          [ 0, 0, 1, 0, 0, 0, 0, 0],  '60*s',                   'minute'           ),
+    'h':        (3.6e3,          [ 0, 0, 1, 0, 0, 0, 0, 0],  '60*min',                 'hour'             ),
+    'd':        (8.64e4,         [ 0, 0, 1, 0, 0, 0, 0, 0],  '24*h',                   'day'              ),
+    'a_t':      (3.1556925e7,    [ 0, 0, 1, 0, 0, 0, 0, 0],  '365.24219*d',            'tropical year'    ),
+    'a_j':      (3.1557600e7,    [ 0, 0, 1, 0, 0, 0, 0, 0],  '365.25*d',               'Julian year'      ),
+    'a_g':      (3.155695e7,     [ 0, 0, 1, 0, 0, 0, 0, 0],  '365.2425*d',             'Gregorian year'   ),
+    'a':        (3.155760e7,     [ 0, 0, 1, 0, 0, 0, 0, 0],  'a_j',                    'year'             ),
+    'eV':       (1.60217733e-16, [ 2, 1,-2, 0, 0, 0, 0, 0],  '[e]*V',                  'electronvolt'     ),
+    'au':       (1.49597870e11,  [ 1, 0, 0, 0, 0, 0, 0, 0],  '149597.870691*Mm',       'astr. unit'       ),
+    'AU':       (1.49597870e11,  [ 1, 0, 0, 0, 0, 0, 0, 0],  'au',                     'astr. unit'       ),
+    # natural units             
+    '[c]':      (2.99792458e8,   [ 1, 0,-1, 0, 0, 0, 0, 0],  '299792458*m/s',          'velocity of light'),
+    '[h]':      (6.626076e-31,   [ 2, 1,-1, 0, 0, 0, 0, 0],  '6.6260755e-34*J*s',      'Planck const.'    ),
+    '[k]':      (1.380658e-20,   [ 2, 1,-2,-1, 0, 0, 0, 0],  '1.380658e-23*J/K',       'Boltzmann const.' ),
+    '[eps_0]':  (8.854188e-15,   [-3,-1, 2, 0, 2, 0, 0, 0],  '8.854187817e-12*F/m',    'permit. of vac.'  ),
+    '[mu_0]':   (1.256637e-3,    [ 1, 1, 0, 0,-2, 0, 0, 0],  '4*[pi]*1e-7*N/A2',       'permeab. of vac.' ),
+    '[e]':      (1.60217733e-19, [ 0, 0, 0, 0, 1, 0, 0, 0],  '1.60217733e-19*C',       'elem. charge'     ),
+    '[m_e]':    (9.109390e-28,   [ 0, 1, 0, 0, 0, 0, 0, 0],  '9.1093897e-28*g',        'electron mass'    ),
+    '[m_p]':    (1.672623e-24,   [ 0, 1, 0, 0, 0, 0, 0, 0],  '1.6726231e-24*g',        'proton mass'      ),
+    '[G]':      (6.672590e-14,   [ 3,-1,-2, 0, 0, 0, 0, 0],  '6.67259e-11*m3/(kg*s2)', 'grav. const.'     ),
+    '[g]':      (9.806650e0,     [ 1, 0,-2, 0, 0, 0, 0, 0],  '9.80665*m/s2',           'grav. accel.'     ),
+    'atm':      (1.013250e8,     [-1, 1,-2, 0, 0, 0, 0, 0],  '101325*Pa',              'atm. pressure'    ),
+    'ly':       (9.460730e15,    [ 1, 0, 0, 0, 0, 0, 0, 0],  '[c]*a_j',                'light-year'       ),
     # dimensionless units
-    '[pi]':     (np.pi,      [  0, 0, 0, 0, 0, 0, 0, 0, 0],  '3.141593',               'pi'               ),
-    '[euler]':  (np.e,       [  0, 0, 0, 0, 0, 0, 0, 0, 0],  '2.718282',               "Euler's num."     ),
-    '[N_A]':    (6.0221367,  [ 23, 0, 0, 0, 0, 0, 0, 0, 0],  '6.022137e23',            "Avogadro's num."  ),
-    '%':        (1,          [ -2, 0, 0, 0, 0, 0, 0, 0, 0],  '1e-2',                   'percent'          ),
-    '[ppth]':   (1,          [ -3, 0, 0, 0, 0, 0, 0, 0, 0],  '1e-3',                   'promile'          ),
+    '[pi]':     (np.pi,          [ 0, 0, 0, 0, 0, 0, 0, 0],  '3.1415926',              'pi'               ),
+    '[euler]':  (np.e,           [ 0, 0, 0, 0, 0, 0, 0, 0],  '2.718282',               "Euler's num."     ),
+    '[N_A]':    (6.0221367e23,   [ 0, 0, 0, 0, 0, 0, 0, 0],  '6.022137e23',            "Avogadro's num."  ),
+    '%':        (1e-2,           [ 0, 0, 0, 0, 0, 0, 0, 0],  '1e-2',                   'percent'          ),
+    '[ppth]':   (1e-3,           [ 0, 0, 0, 0, 0, 0, 0, 0],  '1e-3',                   'promile'          ),
+    '[degR]':   (5/9,            [ 0, 0, 0, 1, 0, 0, 0, 0],  '5/9*K',                  'Degree Rankine'   ),
     # units defined by a nonlinear function
-    'Cel':      (1,          [  0, 0, 0, 0, 1, 0, 0, 0, 0],  convert_celsius,          'Degree Celsius'   ),
+    'Cel':      (1,              [ 0, 0, 0, 1, 0, 0, 0, 0],  None,                     'Degree Celsius'   ),
+    '[degF]':   (1,              [ 0, 0, 0, 1, 0, 0, 0, 0],  None,                     'Degree Fahrenheit'),
 }
-
-def Convert_Arbitrary(quantity1, quantity2):
-    conv = "_".join([quantity1.symbol_base, quantity2.symbol_base])
-    if conv=="Cel_K":
-        magnitude1 = quantity1.magnitude()
-        magnitude2 = (magnitude1 + 273.15) / quantity2.magnitude()
-    elif conv=="K_Cel":
-        magnitude1 = quantity1.magnitude()
-        magnitude2 = (magnitude1 - 273.15) / quantity2.magnitude()
-    if magnitude2:
-        quantity2.magnitude = magnitude2
-        quantity2.base[0] = 0
-        quantity2._rebase()
-        return quantity2
-    else:
-        raise Exception(f"No conversion of arbitrary unit '{quantity1.symbol}' to '{quantity2.symbol}' was found.")
-
```

### Comparing `scinumtools-1.2.3/src/scinumtools/stats/StopwatchClass.py` & `scinumtools-1.3.0/src/scinumtools/stats/StopwatchClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.2.3/src/scinumtools/structs/CollectorClass.py` & `scinumtools-1.3.0/src/scinumtools/structs/CollectorClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.2.3/src/scinumtools/structs/ParameterClass.py` & `scinumtools-1.3.0/src/scinumtools/structs/ParameterClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.2.3/tests/test_data.py` & `scinumtools-1.3.0/tests/test_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,38 +88,31 @@
         (3, 1, 1, 3),
         (4, 2, 0, 4),
     ]
     for r,row in enumerate(ListToGrid(data,ncols)):
         assert grid[r] == row
 
     # List all missing grid points
-    grid = [
-        (5, 2, 1)
-    ]
     for r,row in enumerate(ListToGrid(data,ncols,missing=True)):
-        print(r,row)
-        assert grid[r] == row
+        assert (5, 2, 1) == row
 
     # List transposed grid points
     grid = [
         (0, 0, 0, 0),
         (1, 1, 0, 1),
         (2, 2, 0, 2),
         (3, 0, 1, 3),
         (4, 1, 1, 4),
     ]
     for r,row in enumerate(ListToGrid(data,ncols,transpose=True)):
         assert grid[r] == row
         
     # List all missing transposed grid points
-    grid = [
-        (5, 2, 1)
-    ]
     for r,row in enumerate(ListToGrid(data,ncols,transpose=True,missing=True)):
-        assert grid[r] == row
+        assert (5, 2, 1) == row
         
 def test_dict_to_grid():
 
     data = dict(
         a = 0,
         b = 1,
         c = 2,
@@ -228,10 +221,9 @@
         [[73, 73, 73],
          [85, 85, 85],
          [72, 72, 72],
          [85, 85, 85],
          [71, 71, 71]],
     ]
     imnew = imold.resize((-35,35,-25,25), (5,5))
-    print(np.asarray(imnew.im))
     np.testing.assert_equal(np.asarray(imnew.im), data_resized)
```

### Comparing `scinumtools-1.2.3/tests/test_stats.py` & `scinumtools-1.3.0/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.2.3/tests/test_struct.py` & `scinumtools-1.3.0/tests/test_struct.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.2.3/.gitignore` & `scinumtools-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `scinumtools-1.2.3/pyproject.toml` & `scinumtools-1.3.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "scinumtools"
-version = "1.2.3"
+version = "1.3.0"
 authors = [
   { name="Ondrej Pego Jaura", email="vrtulka23@pm.me" },
 ]
 description = "Set of most frequently used tools for a rapid numerical code development in Python."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `scinumtools-1.2.3/PKG-INFO` & `scinumtools-1.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scinumtools
-Version: 1.2.3
+Version: 1.3.0
 Summary: Set of most frequently used tools for a rapid numerical code development in Python.
 Project-URL: Homepage, https://github.com/vrtulka23/scinumtools
 Project-URL: Bug Tracker, https://github.com/vrtulka23/scinumtools/issues
 Author-email: Ondrej Pego Jaura <vrtulka23@pm.me>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

