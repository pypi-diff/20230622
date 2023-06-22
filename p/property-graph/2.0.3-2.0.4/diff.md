# Comparing `tmp/property-graph-2.0.3.tar.gz` & `tmp/property-graph-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "property-graph-2.0.3.tar", last modified: Wed Jun 21 20:25:57 2023, max compression
+gzip compressed data, was "property-graph-2.0.4.tar", last modified: Wed Jun 21 21:06:44 2023, max compression
```

## Comparing `property-graph-2.0.3.tar` & `property-graph-2.0.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:25:57.056223 property-graph-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-21 20:25:45.000000 property-graph-2.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18100 2023-06-21 20:25:57.056223 property-graph-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-06-21 20:25:45.000000 property-graph-2.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-21 20:25:45.000000 property-graph-2.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 20:25:57.056223 property-graph-2.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:25:57.052222 property-graph-2.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:25:57.052222 property-graph-2.0.3/src/property_graph.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18100 2023-06-21 20:25:57.000000 property-graph-2.0.3/src/property_graph.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-21 20:25:57.000000 property-graph-2.0.3/src/property_graph.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 20:25:57.000000 property-graph-2.0.3/src/property_graph.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-21 20:25:57.000000 property-graph-2.0.3/src/property_graph.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:25:57.052222 property-graph-2.0.3/src/pypg/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-21 20:25:45.000000 property-graph-2.0.3/src/pypg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-21 20:25:45.000000 property-graph-2.0.3/src/pypg/locator.py
--rw-r--r--   0 runner    (1001) docker     (123)    16865 2023-06-21 20:25:45.000000 property-graph-2.0.3/src/pypg/property.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-21 20:25:45.000000 property-graph-2.0.3/src/pypg/property_transcoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:25:57.056223 property-graph-2.0.3/src/pypg/traits/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-21 20:25:45.000000 property-graph-2.0.3/src/pypg/traits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-06-21 20:25:45.000000 property-graph-2.0.3/src/pypg/traits/allowed_range.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-21 20:25:45.000000 property-graph-2.0.3/src/pypg/traits/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-21 20:25:45.000000 property-graph-2.0.3/src/pypg/traits/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-21 20:25:45.000000 property-graph-2.0.3/src/pypg/traits/obligate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-06-21 20:25:45.000000 property-graph-2.0.3/src/pypg/traits/observable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-06-21 20:25:45.000000 property-graph-2.0.3/src/pypg/traits/overridable.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-21 20:25:45.000000 property-graph-2.0.3/src/pypg/traits/read_only.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-21 20:25:45.000000 property-graph-2.0.3/src/pypg/traits/unit.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-21 20:25:45.000000 property-graph-2.0.3/src/pypg/traits/validated.py
--rw-r--r--   0 runner    (1001) docker     (123)    11503 2023-06-21 20:25:45.000000 property-graph-2.0.3/src/pypg/transcode.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-21 20:25:45.000000 property-graph-2.0.3/src/pypg/type_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-21 20:25:45.000000 property-graph-2.0.3/src/pypg/type_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:25:57.056223 property-graph-2.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-06-21 20:25:45.000000 property-graph-2.0.3/tests/test_allowed_range.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-21 20:25:45.000000 property-graph-2.0.3/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-21 20:25:45.000000 property-graph-2.0.3/tests/test_locator.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-21 20:25:45.000000 property-graph-2.0.3/tests/test_obligate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-06-21 20:25:45.000000 property-graph-2.0.3/tests/test_observable.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-06-21 20:25:45.000000 property-graph-2.0.3/tests/test_overridable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-06-21 20:25:45.000000 property-graph-2.0.3/tests/test_property.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-21 20:25:45.000000 property-graph-2.0.3/tests/test_readonly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-21 20:25:45.000000 property-graph-2.0.3/tests/test_traits.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-06-21 20:25:45.000000 property-graph-2.0.3/tests/test_transcoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-21 20:25:45.000000 property-graph-2.0.3/tests/test_type_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-21 20:25:45.000000 property-graph-2.0.3/tests/test_type_schema_encoding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:06:44.975739 property-graph-2.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-21 21:06:36.000000 property-graph-2.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18100 2023-06-21 21:06:44.971739 property-graph-2.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-06-21 21:06:36.000000 property-graph-2.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-21 21:06:36.000000 property-graph-2.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 21:06:44.975739 property-graph-2.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:06:44.967739 property-graph-2.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:06:44.967739 property-graph-2.0.4/src/property_graph.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18100 2023-06-21 21:06:44.000000 property-graph-2.0.4/src/property_graph.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-21 21:06:44.000000 property-graph-2.0.4/src/property_graph.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 21:06:44.000000 property-graph-2.0.4/src/property_graph.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-21 21:06:44.000000 property-graph-2.0.4/src/property_graph.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:06:44.967739 property-graph-2.0.4/src/pypg/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-21 21:06:36.000000 property-graph-2.0.4/src/pypg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-21 21:06:36.000000 property-graph-2.0.4/src/pypg/locator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16865 2023-06-21 21:06:36.000000 property-graph-2.0.4/src/pypg/property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-21 21:06:36.000000 property-graph-2.0.4/src/pypg/property_transcoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:06:44.971739 property-graph-2.0.4/src/pypg/traits/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-21 21:06:36.000000 property-graph-2.0.4/src/pypg/traits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-06-21 21:06:36.000000 property-graph-2.0.4/src/pypg/traits/allowed_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-21 21:06:36.000000 property-graph-2.0.4/src/pypg/traits/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-21 21:06:36.000000 property-graph-2.0.4/src/pypg/traits/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-21 21:06:36.000000 property-graph-2.0.4/src/pypg/traits/obligate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-06-21 21:06:36.000000 property-graph-2.0.4/src/pypg/traits/observable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-06-21 21:06:36.000000 property-graph-2.0.4/src/pypg/traits/overridable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-21 21:06:36.000000 property-graph-2.0.4/src/pypg/traits/read_only.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-21 21:06:36.000000 property-graph-2.0.4/src/pypg/traits/unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-21 21:06:36.000000 property-graph-2.0.4/src/pypg/traits/validated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11503 2023-06-21 21:06:36.000000 property-graph-2.0.4/src/pypg/transcode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-21 21:06:36.000000 property-graph-2.0.4/src/pypg/type_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-21 21:06:36.000000 property-graph-2.0.4/src/pypg/type_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:06:44.971739 property-graph-2.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-06-21 21:06:36.000000 property-graph-2.0.4/tests/test_allowed_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-21 21:06:36.000000 property-graph-2.0.4/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-21 21:06:36.000000 property-graph-2.0.4/tests/test_locator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-21 21:06:36.000000 property-graph-2.0.4/tests/test_obligate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-06-21 21:06:36.000000 property-graph-2.0.4/tests/test_observable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-06-21 21:06:36.000000 property-graph-2.0.4/tests/test_overridable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-06-21 21:06:36.000000 property-graph-2.0.4/tests/test_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-21 21:06:36.000000 property-graph-2.0.4/tests/test_readonly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-21 21:06:36.000000 property-graph-2.0.4/tests/test_traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-06-21 21:06:36.000000 property-graph-2.0.4/tests/test_transcoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-21 21:06:36.000000 property-graph-2.0.4/tests/test_type_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-21 21:06:36.000000 property-graph-2.0.4/tests/test_type_schema_encoding.py
```

### Comparing `property-graph-2.0.3/LICENSE` & `property-graph-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `property-graph-2.0.3/PKG-INFO` & `property-graph-2.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: property-graph
-Version: 2.0.3
+Version: 2.0.4
 Summary: python library for working with objects as graphs of property data
 Author-email: Matt Fowler <mattefowler@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `property-graph-2.0.3/README.md` & `property-graph-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `property-graph-2.0.3/pyproject.toml` & `property-graph-2.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `property-graph-2.0.3/src/property_graph.egg-info/PKG-INFO` & `property-graph-2.0.4/src/property_graph.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: property-graph
-Version: 2.0.3
+Version: 2.0.4
 Summary: python library for working with objects as graphs of property data
 Author-email: Matt Fowler <mattefowler@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `property-graph-2.0.3/src/property_graph.egg-info/SOURCES.txt` & `property-graph-2.0.4/src/property_graph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `property-graph-2.0.3/src/pypg/locator.py` & `property-graph-2.0.4/src/pypg/locator.py`

 * *Files identical despite different names*

### Comparing `property-graph-2.0.3/src/pypg/property.py` & `property-graph-2.0.4/src/pypg/property.py`

 * *Files identical despite different names*

### Comparing `property-graph-2.0.3/src/pypg/property_transcoder.py` & `property-graph-2.0.4/src/pypg/property_transcoder.py`

 * *Files identical despite different names*

### Comparing `property-graph-2.0.3/src/pypg/traits/allowed_range.py` & `property-graph-2.0.4/src/pypg/traits/allowed_range.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 
 
 class AllowedRange(Validated, metaclass=_AllowedRangeMeta):
     def __init__(
         self,
         minimum: LimitProvider,
         maximum: LimitProvider,
-        min_cmp: Comparator = gt,
-        max_cmp: Comparator = lt,
+        min_cmp: Comparator = ge,
+        max_cmp: Comparator = le,
     ):
         super().__init__(self.check_range)
         self.minimum, self.maximum = (
             bound if callable(bound) else self._constant(bound)
             for bound in (minimum, maximum)
         )
         self.min_cmp = min_cmp
```

### Comparing `property-graph-2.0.3/src/pypg/traits/config.py` & `property-graph-2.0.4/src/pypg/traits/config.py`

 * *Files identical despite different names*

### Comparing `property-graph-2.0.3/src/pypg/traits/obligate.py` & `property-graph-2.0.4/src/pypg/traits/obligate.py`

 * *Files identical despite different names*

### Comparing `property-graph-2.0.3/src/pypg/traits/observable.py` & `property-graph-2.0.4/src/pypg/traits/observable.py`

 * *Files identical despite different names*

### Comparing `property-graph-2.0.3/src/pypg/traits/overridable.py` & `property-graph-2.0.4/src/pypg/traits/overridable.py`

 * *Files identical despite different names*

### Comparing `property-graph-2.0.3/src/pypg/traits/read_only.py` & `property-graph-2.0.4/src/pypg/traits/read_only.py`

 * *Files identical despite different names*

### Comparing `property-graph-2.0.3/src/pypg/traits/validated.py` & `property-graph-2.0.4/src/pypg/traits/validated.py`

 * *Files identical despite different names*

### Comparing `property-graph-2.0.3/src/pypg/transcode.py` & `property-graph-2.0.4/src/pypg/transcode.py`

 * *Files identical despite different names*

### Comparing `property-graph-2.0.3/src/pypg/type_registry.py` & `property-graph-2.0.4/src/pypg/type_registry.py`

 * *Files identical despite different names*

### Comparing `property-graph-2.0.3/src/pypg/type_utils.py` & `property-graph-2.0.4/src/pypg/type_utils.py`

 * *Files identical despite different names*

### Comparing `property-graph-2.0.3/tests/test_allowed_range.py` & `property-graph-2.0.4/tests/test_allowed_range.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 from unittest import TestCase
-from operator import ge, le
+from operator import ge, le, lt, gt
 
 from pypg import PreSet, Property, PropertyClass
 from pypg.traits.allowed_range import AllowedRange
 
 
 class TestAllowedRange(TestCase):
     def test_exclusive_bounds(self):
         class Bounded(PropertyClass):
             ar = AllowedRange[PreSet](0, 1)
             p = Property[float](0.5, traits=[ar])
 
         b = Bounded()
         b.p = 0.5  # within range
-        with self.assertRaises(ValueError):
-            b.p = 0  # boundaries are exlcusive by default
-        with self.assertRaises(ValueError):
-            b.p = 1  # boundaries are exlcusive by default
+        b.p = 0  # boundaries are inclusive by default
+        b.p = 1  # boundaries are inclusive by default
         with self.assertRaises(ValueError):
             b.p = -1  # below minimum
         with self.assertRaises(ValueError):
             b.p = 2  # above maximum
 
-    def test_inclusive_bounds(self):
+    def test_exclusive_bounds(self):
         class Bounded(PropertyClass):
-            ar = AllowedRange[PreSet](0, 1, min_cmp=ge, max_cmp=le)
-            p = Property[float](0, traits=[ar])
+            ar = AllowedRange[PreSet](0, 1, min_cmp=gt, max_cmp=lt)
+            p = Property[float](0.5, traits=[ar])
 
         b = Bounded()
         b.p = 0.5  # within range
-        b.p = 0  # bounds have been explicitly declared inclusive
-        b.p = 1  # bounds have been explicitly declared inclusive
+        with self.assertRaises(ValueError):
+            b.p = 0  # bounds have been explicitly declared exclusive
+        with self.assertRaises(ValueError):
+            b.p = 1  # bounds have been explicitly declared exclusive
         with self.assertRaises(ValueError):
             b.p = -1  # below minimum
         with self.assertRaises(ValueError):
             b.p = 2  # above maximum
 
     def test_operators_exclusive(self):
         class Bounded(PropertyClass):
```

### Comparing `property-graph-2.0.3/tests/test_config.py` & `property-graph-2.0.4/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `property-graph-2.0.3/tests/test_locator.py` & `property-graph-2.0.4/tests/test_locator.py`

 * *Files identical despite different names*

### Comparing `property-graph-2.0.3/tests/test_obligate.py` & `property-graph-2.0.4/tests/test_obligate.py`

 * *Files identical despite different names*

### Comparing `property-graph-2.0.3/tests/test_observable.py` & `property-graph-2.0.4/tests/test_observable.py`

 * *Files identical despite different names*

### Comparing `property-graph-2.0.3/tests/test_overridable.py` & `property-graph-2.0.4/tests/test_overridable.py`

 * *Files identical despite different names*

### Comparing `property-graph-2.0.3/tests/test_property.py` & `property-graph-2.0.4/tests/test_property.py`

 * *Files identical despite different names*

### Comparing `property-graph-2.0.3/tests/test_readonly.py` & `property-graph-2.0.4/tests/test_readonly.py`

 * *Files identical despite different names*

### Comparing `property-graph-2.0.3/tests/test_traits.py` & `property-graph-2.0.4/tests/test_traits.py`

 * *Files identical despite different names*

### Comparing `property-graph-2.0.3/tests/test_transcoder.py` & `property-graph-2.0.4/tests/test_transcoder.py`

 * *Files identical despite different names*

### Comparing `property-graph-2.0.3/tests/test_type_registry.py` & `property-graph-2.0.4/tests/test_type_registry.py`

 * *Files identical despite different names*

### Comparing `property-graph-2.0.3/tests/test_type_schema_encoding.py` & `property-graph-2.0.4/tests/test_type_schema_encoding.py`

 * *Files identical despite different names*

