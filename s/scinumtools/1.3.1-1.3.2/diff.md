# Comparing `tmp/scinumtools-1.3.1.tar.gz` & `tmp/scinumtools-1.3.2.tar.gz`

## Comparing `scinumtools-1.3.1.tar` & `scinumtools-1.3.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-1.3.1/requirements.txt
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 scinumtools-1.3.1/.github/workflows/pytest.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 scinumtools-1.3.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 scinumtools-1.3.1/src/scinumtools/__init__.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 scinumtools-1.3.1/src/scinumtools/data/CachingClass.py
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 scinumtools-1.3.1/src/scinumtools/data/ImageClass.py
--rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 scinumtools-1.3.1/src/scinumtools/data/PlottingClass.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 scinumtools-1.3.1/src/scinumtools/data/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scinumtools-1.3.1/src/scinumtools/math/__init__.py
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 scinumtools-1.3.1/src/scinumtools/math/solver/AtomClass.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 scinumtools-1.3.1/src/scinumtools/math/solver/ExpressionClass.py
--rw-r--r--   0        0        0     7525 2020-02-02 00:00:00.000000 scinumtools-1.3.1/src/scinumtools/math/solver/OperatorClass.py
--rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 scinumtools-1.3.1/src/scinumtools/math/solver/SolverClass.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 scinumtools-1.3.1/src/scinumtools/math/solver/TokensClass.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 scinumtools-1.3.1/src/scinumtools/math/solver/__init__.py
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 scinumtools-1.3.1/src/scinumtools/phys/ConstantsClass.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 scinumtools-1.3.1/src/scinumtools/phys/__init__.py
--rw-r--r--   0        0        0     7501 2020-02-02 00:00:00.000000 scinumtools-1.3.1/src/scinumtools/phys/units/QuantityClass.py
--rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 scinumtools-1.3.1/src/scinumtools/phys/units/UnitConverters.py
--rw-r--r--   0        0        0    10140 2020-02-02 00:00:00.000000 scinumtools-1.3.1/src/scinumtools/phys/units/UnitList.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-1.3.1/src/scinumtools/phys/units/__init__.py
--rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 scinumtools-1.3.1/src/scinumtools/stats/StopwatchClass.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 scinumtools-1.3.1/src/scinumtools/stats/__init__.py
--rw-r--r--   0        0        0     5397 2020-02-02 00:00:00.000000 scinumtools-1.3.1/src/scinumtools/structs/CollectorClass.py
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 scinumtools-1.3.1/src/scinumtools/structs/ParameterClass.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 scinumtools-1.3.1/src/scinumtools/structs/__init__.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 scinumtools-1.3.1/tests/cached_data.npy
--rw-r--r--   0        0        0     6088 2020-02-02 00:00:00.000000 scinumtools-1.3.1/tests/test_data.py
--rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 scinumtools-1.3.1/tests/test_math.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 scinumtools-1.3.1/tests/test_physics.py
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 scinumtools-1.3.1/tests/test_stats.py
--rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 scinumtools-1.3.1/tests/test_struct.py
--rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 scinumtools-1.3.1/tests/test_units.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 scinumtools-1.3.1/.gitignore
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 scinumtools-1.3.1/README.md
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 scinumtools-1.3.1/pyproject.toml
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 scinumtools-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-1.3.2/requirements.txt
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 scinumtools-1.3.2/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 scinumtools-1.3.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 scinumtools-1.3.2/src/scinumtools/__init__.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 scinumtools-1.3.2/src/scinumtools/data/CachingClass.py
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 scinumtools-1.3.2/src/scinumtools/data/ImageClass.py
+-rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 scinumtools-1.3.2/src/scinumtools/data/PlottingClass.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 scinumtools-1.3.2/src/scinumtools/data/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scinumtools-1.3.2/src/scinumtools/math/__init__.py
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 scinumtools-1.3.2/src/scinumtools/math/solver/AtomClass.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 scinumtools-1.3.2/src/scinumtools/math/solver/ExpressionClass.py
+-rw-r--r--   0        0        0     7525 2020-02-02 00:00:00.000000 scinumtools-1.3.2/src/scinumtools/math/solver/OperatorClass.py
+-rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 scinumtools-1.3.2/src/scinumtools/math/solver/SolverClass.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 scinumtools-1.3.2/src/scinumtools/math/solver/TokensClass.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 scinumtools-1.3.2/src/scinumtools/math/solver/__init__.py
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 scinumtools-1.3.2/src/scinumtools/phys/ConstantsClass.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 scinumtools-1.3.2/src/scinumtools/phys/__init__.py
+-rw-r--r--   0        0        0     7821 2020-02-02 00:00:00.000000 scinumtools-1.3.2/src/scinumtools/phys/units/QuantityClass.py
+-rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 scinumtools-1.3.2/src/scinumtools/phys/units/UnitConverters.py
+-rw-r--r--   0        0        0    10140 2020-02-02 00:00:00.000000 scinumtools-1.3.2/src/scinumtools/phys/units/UnitList.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-1.3.2/src/scinumtools/phys/units/__init__.py
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 scinumtools-1.3.2/src/scinumtools/stats/StopwatchClass.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 scinumtools-1.3.2/src/scinumtools/stats/__init__.py
+-rw-r--r--   0        0        0     5397 2020-02-02 00:00:00.000000 scinumtools-1.3.2/src/scinumtools/structs/CollectorClass.py
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 scinumtools-1.3.2/src/scinumtools/structs/ParameterClass.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 scinumtools-1.3.2/src/scinumtools/structs/__init__.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 scinumtools-1.3.2/tests/cached_data.npy
+-rw-r--r--   0        0        0     6088 2020-02-02 00:00:00.000000 scinumtools-1.3.2/tests/test_data.py
+-rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 scinumtools-1.3.2/tests/test_math.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 scinumtools-1.3.2/tests/test_physics.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 scinumtools-1.3.2/tests/test_stats.py
+-rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 scinumtools-1.3.2/tests/test_struct.py
+-rw-r--r--   0        0        0     3357 2020-02-02 00:00:00.000000 scinumtools-1.3.2/tests/test_units.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 scinumtools-1.3.2/.gitignore
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 scinumtools-1.3.2/README.md
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 scinumtools-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 scinumtools-1.3.2/PKG-INFO
```

### Comparing `scinumtools-1.3.1/.github/workflows/python-publish.yml` & `scinumtools-1.3.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `scinumtools-1.3.1/src/scinumtools/data/ImageClass.py` & `scinumtools-1.3.2/src/scinumtools/data/ImageClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.3.1/src/scinumtools/data/PlottingClass.py` & `scinumtools-1.3.2/src/scinumtools/data/PlottingClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.3.1/src/scinumtools/math/solver/AtomClass.py` & `scinumtools-1.3.2/src/scinumtools/math/solver/AtomClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.3.1/src/scinumtools/math/solver/ExpressionClass.py` & `scinumtools-1.3.2/src/scinumtools/math/solver/ExpressionClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.3.1/src/scinumtools/math/solver/OperatorClass.py` & `scinumtools-1.3.2/src/scinumtools/math/solver/OperatorClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.3.1/src/scinumtools/math/solver/SolverClass.py` & `scinumtools-1.3.2/src/scinumtools/math/solver/SolverClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.3.1/src/scinumtools/math/solver/TokensClass.py` & `scinumtools-1.3.2/src/scinumtools/math/solver/TokensClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.3.1/src/scinumtools/phys/ConstantsClass.py` & `scinumtools-1.3.2/src/scinumtools/phys/ConstantsClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.3.1/src/scinumtools/phys/units/QuantityClass.py` & `scinumtools-1.3.2/src/scinumtools/phys/units/QuantityClass.py`

 * *Files 14% similar despite different names*

```diff
@@ -172,18 +172,24 @@
         for unitid,exponent in baseunits.items():
             symbol = unitid.replace(':','')
             units.append(f"{symbol}" if exponent==1 else f"{symbol}{exponent}")
         return "*".join(units)
 
     def to(self, units):
         if isinstance(units,str):
-            other = Quantity(1,units)
-            if self.dimensions!=other.dimensions:
-                raise Exception("Converting units with different dimensions:",
-                                self.dimensions, other.dimensions)
-            with TemperatureConverter(self.baseunits, other.baseunits) as tc:
+            unit1 = self
+            unit2 = Quantity(1,units)
+            # Check if units can be directly converted
+            if unit1.dimensions!=unit2.dimensions:
+                # Check if inverted unit can be converted
+                if np.all([-unit1.dimensions[d]==unit2.dimensions[d] for d in range(len(UnitBase))]):
+                    unit1 = Quantity(1)/self
+                else:
+                    raise Exception("Converting units with different dimensions:",
+                                    unit1.dimensions, unit2.dimensions)
+            with TemperatureConverter(unit1.baseunits, unit2.baseunits) as tc:
                 if tc.convertable:
-                    return Quantity(tc.convert(self.magnitude, other.magnitude), units)
-            unit = self/other
+                    return Quantity(tc.convert(unit1.magnitude, unit2.magnitude), units)
+            unit = unit1/unit2
             return Quantity(unit.magnitude, units)
         else:
             raise Exception("Invalid units format:", units)
```

### Comparing `scinumtools-1.3.1/src/scinumtools/phys/units/UnitConverters.py` & `scinumtools-1.3.2/src/scinumtools/phys/units/UnitConverters.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.3.1/src/scinumtools/phys/units/UnitList.py` & `scinumtools-1.3.2/src/scinumtools/phys/units/UnitList.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.3.1/src/scinumtools/stats/StopwatchClass.py` & `scinumtools-1.3.2/src/scinumtools/stats/StopwatchClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.3.1/src/scinumtools/structs/CollectorClass.py` & `scinumtools-1.3.2/src/scinumtools/structs/CollectorClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.3.1/src/scinumtools/structs/ParameterClass.py` & `scinumtools-1.3.2/src/scinumtools/structs/ParameterClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.3.1/tests/test_data.py` & `scinumtools-1.3.2/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.3.1/tests/test_math.py` & `scinumtools-1.3.2/tests/test_math.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.3.1/tests/test_stats.py` & `scinumtools-1.3.2/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.3.1/tests/test_struct.py` & `scinumtools-1.3.2/tests/test_struct.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.3.1/tests/test_units.py` & `scinumtools-1.3.2/tests/test_units.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,7 +73,13 @@
     assert str(q) == "Quantity(1.340e-32)"
     
     with pytest.raises(Exception) as excinfo:
         q = q.to("kg3*s/cm3")
     assert excinfo.value.args[0]=="Converting units with different dimensions:"
     assert excinfo.value.args[1]==[0, 0, 0, 0, 0, 0, 0, 0]
     assert excinfo.value.args[2]==[-3, 3, 1, 0, 0, 0, 0, 0]
+
+def test_inversion():
+
+    assert str(Quantity(23, 'Hz').to('s'))     == "Quantity(4.348e-02 s)"
+    assert str(Quantity(34, 'Ohm').to('S'))    == "Quantity(2.941e-02 S)"
+    assert str(Quantity(102, 'J').to('erg-1')) == "Quantity(9.804e-10 erg-1)"
```

### Comparing `scinumtools-1.3.1/.gitignore` & `scinumtools-1.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `scinumtools-1.3.1/pyproject.toml` & `scinumtools-1.3.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "scinumtools"
-version = "1.3.1"
+version = "1.3.2"
 authors = [
   { name="Ondrej Pego Jaura", email="vrtulka23@pm.me" },
 ]
 description = "Set of most frequently used tools for a rapid numerical code development in Python."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `scinumtools-1.3.1/PKG-INFO` & `scinumtools-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scinumtools
-Version: 1.3.1
+Version: 1.3.2
 Summary: Set of most frequently used tools for a rapid numerical code development in Python.
 Project-URL: Homepage, https://github.com/vrtulka23/scinumtools
 Project-URL: Bug Tracker, https://github.com/vrtulka23/scinumtools/issues
 Author-email: Ondrej Pego Jaura <vrtulka23@pm.me>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

