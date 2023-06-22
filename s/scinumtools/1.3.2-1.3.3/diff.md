# Comparing `tmp/scinumtools-1.3.2.tar.gz` & `tmp/scinumtools-1.3.3.tar.gz`

## Comparing `scinumtools-1.3.2.tar` & `scinumtools-1.3.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-1.3.2/requirements.txt
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 scinumtools-1.3.2/.github/workflows/pytest.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 scinumtools-1.3.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 scinumtools-1.3.2/src/scinumtools/__init__.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 scinumtools-1.3.2/src/scinumtools/data/CachingClass.py
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 scinumtools-1.3.2/src/scinumtools/data/ImageClass.py
--rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 scinumtools-1.3.2/src/scinumtools/data/PlottingClass.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 scinumtools-1.3.2/src/scinumtools/data/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scinumtools-1.3.2/src/scinumtools/math/__init__.py
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 scinumtools-1.3.2/src/scinumtools/math/solver/AtomClass.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 scinumtools-1.3.2/src/scinumtools/math/solver/ExpressionClass.py
--rw-r--r--   0        0        0     7525 2020-02-02 00:00:00.000000 scinumtools-1.3.2/src/scinumtools/math/solver/OperatorClass.py
--rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 scinumtools-1.3.2/src/scinumtools/math/solver/SolverClass.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 scinumtools-1.3.2/src/scinumtools/math/solver/TokensClass.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 scinumtools-1.3.2/src/scinumtools/math/solver/__init__.py
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 scinumtools-1.3.2/src/scinumtools/phys/ConstantsClass.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 scinumtools-1.3.2/src/scinumtools/phys/__init__.py
--rw-r--r--   0        0        0     7821 2020-02-02 00:00:00.000000 scinumtools-1.3.2/src/scinumtools/phys/units/QuantityClass.py
--rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 scinumtools-1.3.2/src/scinumtools/phys/units/UnitConverters.py
--rw-r--r--   0        0        0    10140 2020-02-02 00:00:00.000000 scinumtools-1.3.2/src/scinumtools/phys/units/UnitList.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-1.3.2/src/scinumtools/phys/units/__init__.py
--rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 scinumtools-1.3.2/src/scinumtools/stats/StopwatchClass.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 scinumtools-1.3.2/src/scinumtools/stats/__init__.py
--rw-r--r--   0        0        0     5397 2020-02-02 00:00:00.000000 scinumtools-1.3.2/src/scinumtools/structs/CollectorClass.py
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 scinumtools-1.3.2/src/scinumtools/structs/ParameterClass.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 scinumtools-1.3.2/src/scinumtools/structs/__init__.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 scinumtools-1.3.2/tests/cached_data.npy
--rw-r--r--   0        0        0     6088 2020-02-02 00:00:00.000000 scinumtools-1.3.2/tests/test_data.py
--rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 scinumtools-1.3.2/tests/test_math.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 scinumtools-1.3.2/tests/test_physics.py
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 scinumtools-1.3.2/tests/test_stats.py
--rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 scinumtools-1.3.2/tests/test_struct.py
--rw-r--r--   0        0        0     3357 2020-02-02 00:00:00.000000 scinumtools-1.3.2/tests/test_units.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 scinumtools-1.3.2/.gitignore
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 scinumtools-1.3.2/README.md
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 scinumtools-1.3.2/pyproject.toml
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 scinumtools-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-1.3.3/requirements.txt
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 scinumtools-1.3.3/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 scinumtools-1.3.3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 scinumtools-1.3.3/src/scinumtools/__init__.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 scinumtools-1.3.3/src/scinumtools/data/CachingClass.py
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 scinumtools-1.3.3/src/scinumtools/data/ImageClass.py
+-rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 scinumtools-1.3.3/src/scinumtools/data/PlottingClass.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 scinumtools-1.3.3/src/scinumtools/data/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scinumtools-1.3.3/src/scinumtools/math/__init__.py
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 scinumtools-1.3.3/src/scinumtools/math/solver/AtomClass.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 scinumtools-1.3.3/src/scinumtools/math/solver/ExpressionClass.py
+-rw-r--r--   0        0        0     7525 2020-02-02 00:00:00.000000 scinumtools-1.3.3/src/scinumtools/math/solver/OperatorClass.py
+-rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 scinumtools-1.3.3/src/scinumtools/math/solver/SolverClass.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 scinumtools-1.3.3/src/scinumtools/math/solver/TokensClass.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 scinumtools-1.3.3/src/scinumtools/math/solver/__init__.py
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 scinumtools-1.3.3/src/scinumtools/phys/ConstantsClass.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 scinumtools-1.3.3/src/scinumtools/phys/__init__.py
+-rw-r--r--   0        0        0     9181 2020-02-02 00:00:00.000000 scinumtools-1.3.3/src/scinumtools/phys/units/QuantityClass.py
+-rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 scinumtools-1.3.3/src/scinumtools/phys/units/UnitConverters.py
+-rw-r--r--   0        0        0    10140 2020-02-02 00:00:00.000000 scinumtools-1.3.3/src/scinumtools/phys/units/UnitList.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-1.3.3/src/scinumtools/phys/units/__init__.py
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 scinumtools-1.3.3/src/scinumtools/stats/StopwatchClass.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 scinumtools-1.3.3/src/scinumtools/stats/__init__.py
+-rw-r--r--   0        0        0     5397 2020-02-02 00:00:00.000000 scinumtools-1.3.3/src/scinumtools/structs/CollectorClass.py
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 scinumtools-1.3.3/src/scinumtools/structs/ParameterClass.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 scinumtools-1.3.3/src/scinumtools/structs/__init__.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 scinumtools-1.3.3/tests/cached_data.npy
+-rw-r--r--   0        0        0     6088 2020-02-02 00:00:00.000000 scinumtools-1.3.3/tests/test_data.py
+-rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 scinumtools-1.3.3/tests/test_math.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 scinumtools-1.3.3/tests/test_physics.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 scinumtools-1.3.3/tests/test_stats.py
+-rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 scinumtools-1.3.3/tests/test_struct.py
+-rw-r--r--   0        0        0     4313 2020-02-02 00:00:00.000000 scinumtools-1.3.3/tests/test_units.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 scinumtools-1.3.3/.gitignore
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 scinumtools-1.3.3/README.md
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 scinumtools-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 scinumtools-1.3.3/PKG-INFO
```

### Comparing `scinumtools-1.3.2/.github/workflows/python-publish.yml` & `scinumtools-1.3.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `scinumtools-1.3.2/src/scinumtools/data/ImageClass.py` & `scinumtools-1.3.3/src/scinumtools/data/ImageClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.3.2/src/scinumtools/data/PlottingClass.py` & `scinumtools-1.3.3/src/scinumtools/data/PlottingClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.3.2/src/scinumtools/math/solver/AtomClass.py` & `scinumtools-1.3.3/src/scinumtools/math/solver/AtomClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.3.2/src/scinumtools/math/solver/ExpressionClass.py` & `scinumtools-1.3.3/src/scinumtools/math/solver/ExpressionClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.3.2/src/scinumtools/math/solver/OperatorClass.py` & `scinumtools-1.3.3/src/scinumtools/math/solver/OperatorClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.3.2/src/scinumtools/math/solver/SolverClass.py` & `scinumtools-1.3.3/src/scinumtools/math/solver/SolverClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.3.2/src/scinumtools/math/solver/TokensClass.py` & `scinumtools-1.3.3/src/scinumtools/math/solver/TokensClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.3.2/src/scinumtools/phys/ConstantsClass.py` & `scinumtools-1.3.3/src/scinumtools/phys/ConstantsClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.3.2/src/scinumtools/phys/units/QuantityClass.py` & `scinumtools-1.3.3/src/scinumtools/phys/units/QuantityClass.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,23 +24,30 @@
             self, magnitude:float,
             dimensions = None,
             baseunits = {}
     ):
         # Initialize settings
         self.unitlist = ParameterDict(['magnitude','dimensions','definition','name'], UnitStandard)
         self.prefixes = ParameterDict(['magnitude','dimensions','definition','name'], UnitPrefixes)
-        self.magnitude = magnitude
+        if isinstance(magnitude, (int,float)):
+            self.magnitude = float(magnitude)
+        elif isinstance(magnitude, list):
+            self.magnitude = np.array(magnitude, dtype=float)
+        elif isinstance(magnitude, np.ndarray):
+            self.magnitude = magnitude.astype(float)
+        else:
+            raise Exception("Magnitude can be either a number or an list/array of numbers")
         # Set quantity
         if dimensions is None:
             self.dimensions = [0]*len(UnitBase)
             self.baseunits = {}
         elif isinstance(dimensions, str):
             with ExpressionSolver(self._atom_parser, [OperatorPar,OperatorMul,OperatorTruediv]) as es:
                 unit = es.solve(dimensions)
-            self.magnitude *= float(unit.magnitude)
+            self.magnitude *= unit.magnitude
             self.dimensions = list(unit.dimensions)
             self.baseunits = dict(unit.baseunits)
         elif isinstance(dimensions, (list, np.ndarray)):
             self.dimensions = list(dimensions)
             if baseunits:
                 self.baseunits = baseunits
             else:
@@ -49,38 +56,46 @@
             raise Exception("Insufficient quantity definition", magnitude, dimensions, baseunits)
         # Remove zero base units
         for unit in list(self.baseunits.keys()):
             if self.baseunits[unit]==0:
                 del self.baseunits[unit]
         
     def __add__(self, other):
+        if not isinstance(other, Quantity):
+            other = Quantity(other)
         if not self.dimensions==other.dimensions:
             raise Exception('Addition of two units with different dimensions:', self, other)
         magnitude = self.magnitude + other.magnitude
         dimensions = list(self.dimensions)
         baseunits = dict(self.baseunits)
         return Quantity(magnitude, dimensions, baseunits)
 
     def __sub__(self, other):
+        if not isinstance(other, Quantity):
+            other = Quantity(other)
         if not self.dimensions==other.dimensions:
             raise Exception('Substraction of two units with different dimensions:', self, other)
         magnitude = self.magnitude - other.magnitude
         dimensions = list(self.dimensions)
         baseunits = dict(self.baseunits)
         return Quantity(magnitude, dimensions, baseunits)
     
     def __mul__(self, other):
+        if not isinstance(other, Quantity):
+            other = Quantity(other)
         magnitude = self.magnitude * other.magnitude
         dimensions = [self.dimensions[i]+other.dimensions[i] for i in range(len(UnitBase))]
         baseunits = dict(self.baseunits)
         for unit,exp in other.baseunits.items():
             baseunits[unit] = baseunits[unit]+exp if unit in baseunits else exp
         return Quantity(magnitude, dimensions, baseunits)
 
     def __truediv__(self, other):
+        if not isinstance(other, Quantity):
+            other = Quantity(other)
         magnitude = self.magnitude / other.magnitude
         dimensions = [self.dimensions[i]-other.dimensions[i] for i in range(len(UnitBase))]
         baseunits = dict(self.baseunits)
         for unit,exp in other.baseunits.items():
             baseunits[unit] = baseunits[unit]-exp if unit in baseunits else -exp
         return Quantity(magnitude, dimensions, baseunits)
 
@@ -94,24 +109,42 @@
         if not isclose(self.magnitude, other.magnitude, rel_tol=self.precision):
             return False
         if self.dimensions!=other.dimensions:
             return False
         return True
     
     def __str__(self):
+        magnitude = self.value()
+        if isinstance(magnitude, np.ndarray):
+            with np.printoptions(precision=3, suppress=False, threshold=5):
+                magnitude = f"{str(magnitude):s}"
+        else:
+            magnitude = f"{magnitude:.03e}"
         if self.baseunits:
-            return f"Quantity({self.value():.03e} {self.units()})"
+            return f"Quantity({magnitude:s} {self.units()})"
         else:
-            return f"Quantity({self.value():.03e})"
+            return f"Quantity({magnitude:s})"
             
     def __repr__(self):
+        magnitude = self.value()
+        if isinstance(magnitude, np.ndarray):
+            with np.printoptions(precision=3, suppress=False, threshold=5):
+                magnitude = f"{str(magnitude):s}"
+        else:
+            magnitude = f"{magnitude:.03e}"
         if self.baseunits:
-            return f"Quantity({self.value():.03e} {self.units()})"
+            return f"Quantity({magnitude:s} {self.units()})"
         else:
-            return f"Quantity({self.value():.03e})"
+            return f"Quantity({magnitude:s})"
+
+    def __array__(self):
+        return self.magnitude
+
+    def __array_wrap__(self, out_arr, context=None):
+        return Quantity(out_arr, self.dimensions, self.baseunits)
     
     def _atom_parser(self, string=None):
         # parse number
         m = re.match(r'^[-]?([0-9.]+)(e([0-9+-]+)|)$', str(string))
         if m:
             magnitude = float(string)
             return Quantity(magnitude)
```

### Comparing `scinumtools-1.3.2/src/scinumtools/phys/units/UnitConverters.py` & `scinumtools-1.3.3/src/scinumtools/phys/units/UnitConverters.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.3.2/src/scinumtools/phys/units/UnitList.py` & `scinumtools-1.3.3/src/scinumtools/phys/units/UnitList.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.3.2/src/scinumtools/stats/StopwatchClass.py` & `scinumtools-1.3.3/src/scinumtools/stats/StopwatchClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.3.2/src/scinumtools/structs/CollectorClass.py` & `scinumtools-1.3.3/src/scinumtools/structs/CollectorClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.3.2/src/scinumtools/structs/ParameterClass.py` & `scinumtools-1.3.3/src/scinumtools/structs/ParameterClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.3.2/tests/test_data.py` & `scinumtools-1.3.3/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.3.2/tests/test_math.py` & `scinumtools-1.3.3/tests/test_math.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.3.2/tests/test_stats.py` & `scinumtools-1.3.3/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.3.2/tests/test_struct.py` & `scinumtools-1.3.3/tests/test_struct.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.3.2/tests/test_units.py` & `scinumtools-1.3.3/tests/test_units.py`

 * *Files 20% similar despite different names*

```diff
@@ -33,53 +33,73 @@
     assert str(Quantity(23,'[degF]').to('Cel'))     == "Quantity(-5.000e+00 Cel)"
     assert str(Quantity(23,'[degF]').to('[degR]'))  == "Quantity(4.827e+02 [degR])"
     assert str(Quantity(23,'[degR]').to('K'))       == "Quantity(1.278e+01 K)"
     assert str(Quantity(23,'[degR]').to('Cel'))     == "Quantity(-2.604e+02 Cel)"
     assert str(Quantity(23,'[degR]').to('[degF]'))  == "Quantity(-4.367e+02 [degF])"
     assert str(Quantity(2300,'Cel').to('kK'))       == "Quantity(2.573e+00 kK)"
     
-def test_units():
+def test_inversion():
+
+    assert str(Quantity(23, 'Hz').to('s'))     == "Quantity(4.348e-02 s)"
+    assert str(Quantity(34, 'Ohm').to('S'))    == "Quantity(2.941e-02 S)"
+    assert str(Quantity(102, 'J').to('erg-1')) == "Quantity(9.804e-10 erg-1)"
+
+def test_scalar_arithmetics():
     
     q = Quantity(123e2, [3,3,0,0,1,0,0,0])
-    assert str(q) == "Quantity(1.230e+04 m3*g3*C)"
-    
-    q = q / Quantity(123, 'C')
+    assert str(q) == "Quantity(1.230e+04 m3*g3*C)"    
+    q /= Quantity(123, 'C')
     assert str(q) == "Quantity(1.000e+02 m3*g3)"
-
-    q = q * Quantity(2, 's2')
+    q *= Quantity(2, 's2')
     assert str(q) == "Quantity(2.000e+02 m3*g3*s2)"
-    
     q = Quantity(123, "kg3*cm-2*s")
     assert str(q) == "Quantity(1.230e+02 kg3*cm-2*s)"
-    
     q = Quantity(123e34, "J")
     assert str(q) == "Quantity(1.230e+36 J)"
-    
-    q = q / Quantity(123, 's')
+    q /= Quantity(123, 's')
     assert str(q) == "Quantity(1.000e+34 J*s-1)"
-    
     q = q ** 2
     assert str(q) == "Quantity(1.000e+68 J2*s-2)"
-    
     q = q.to('kg2*m4/s6')
     assert str(q) == "Quantity(1.000e+68 kg2*m4*s-6)"
-    
     q = Quantity(123, "kg3*s/(cm2*m)")
     assert str(q) == "Quantity(1.230e+02 kg3*s*cm-2*m-1)"
-
     q = q.to("kg3*s/cm3")
     assert str(q) == "Quantity(1.230e+00 kg3*s*cm-3)"
-
     q = Quantity(134e-34)
     assert str(q) == "Quantity(1.340e-32)"
     
     with pytest.raises(Exception) as excinfo:
         q = q.to("kg3*s/cm3")
     assert excinfo.value.args[0]=="Converting units with different dimensions:"
     assert excinfo.value.args[1]==[0, 0, 0, 0, 0, 0, 0, 0]
     assert excinfo.value.args[2]==[-3, 3, 1, 0, 0, 0, 0, 0]
 
-def test_inversion():
+def test_array_arithmetics():
 
-    assert str(Quantity(23, 'Hz').to('s'))     == "Quantity(4.348e-02 s)"
-    assert str(Quantity(34, 'Ohm').to('S'))    == "Quantity(2.941e-02 S)"
-    assert str(Quantity(102, 'J').to('erg-1')) == "Quantity(9.804e-10 erg-1)"
+    # Test basic arithmetics
+    q = Quantity([2,3,4], 'm')
+    assert str(q) == "Quantity([2. 3. 4.] m)"
+    q += Quantity(2, 'm')
+    assert str(q) == "Quantity([4. 5. 6.] m)"
+    q -= Quantity(2, 'm')
+    assert str(q) == "Quantity([2. 3. 4.] m)"
+    q /= Quantity(2)
+    assert str(q) == "Quantity([1.  1.5 2. ] m)"
+    q *= Quantity(2)
+    assert str(q) == "Quantity([2. 3. 4.] m)"
+    q /= 2
+    assert str(q) == "Quantity([1.  1.5 2. ] m)"
+    q *= 2
+    assert str(q) == "Quantity([2. 3. 4.] m)"
+    q /= [1, 1.5, 2]
+    assert str(q) == "Quantity([2. 2. 2.] m)"
+    q *= [1, 1.5, 2]
+    assert str(q) == "Quantity([2. 3. 4.] m)"
+    q = q ** 10
+    assert str(q) == "Quantity([1.024e+03 5.905e+04 1.049e+06] m10)"
+
+    # Test unit conversion on arrays
+    assert str(Quantity([1,2,3], 'm').to('km')) == "Quantity([0.001 0.002 0.003] km)"
+
+    # Test numpy functions
+    assert str(np.sqrt(Quantity([4, 9, 16], 'm'))) == "Quantity([2. 3. 4.] m)"
```

### Comparing `scinumtools-1.3.2/.gitignore` & `scinumtools-1.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `scinumtools-1.3.2/pyproject.toml` & `scinumtools-1.3.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "scinumtools"
-version = "1.3.2"
+version = "1.3.3"
 authors = [
   { name="Ondrej Pego Jaura", email="vrtulka23@pm.me" },
 ]
 description = "Set of most frequently used tools for a rapid numerical code development in Python."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `scinumtools-1.3.2/PKG-INFO` & `scinumtools-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scinumtools
-Version: 1.3.2
+Version: 1.3.3
 Summary: Set of most frequently used tools for a rapid numerical code development in Python.
 Project-URL: Homepage, https://github.com/vrtulka23/scinumtools
 Project-URL: Bug Tracker, https://github.com/vrtulka23/scinumtools/issues
 Author-email: Ondrej Pego Jaura <vrtulka23@pm.me>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

