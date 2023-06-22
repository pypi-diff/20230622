# Comparing `tmp/python-dataschema-0.1.4.tar.gz` & `tmp/python-dataschema-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python-dataschema-0.1.4.tar", last modified: Tue Jan  4 23:03:34 2022, max compression
+gzip compressed data, was "python-dataschema-0.1.5.tar", last modified: Thu Jun 22 19:33:38 2023, max compression
```

## Comparing `python-dataschema-0.1.4.tar` & `python-dataschema-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-01-04 23:03:34.000000 python-dataschema-0.1.4/
--rw-r--r--   0 alex       (501) staff       (20)      359 2022-01-04 23:03:34.000000 python-dataschema-0.1.4/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)     5231 2019-12-07 02:17:46.000000 python-dataschema-0.1.4/README.md
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-01-04 23:03:34.000000 python-dataschema-0.1.4/dataschema/
--rw-r--r--   0 alex       (501) staff       (20)      389 2021-03-19 04:29:08.000000 python-dataschema-0.1.4/dataschema/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     1264 2021-03-11 21:00:12.000000 python-dataschema-0.1.4/dataschema/_utils.py
--rw-r--r--   0 alex       (501) staff       (20)     7672 2021-07-03 01:35:03.000000 python-dataschema-0.1.4/dataschema/base.py
--rw-r--r--   0 alex       (501) staff       (20)     1360 2021-07-03 01:35:03.000000 python-dataschema-0.1.4/dataschema/common.py
--rw-r--r--   0 alex       (501) staff       (20)    25992 2022-01-04 22:47:18.000000 python-dataschema-0.1.4/dataschema/specs.py
--rw-r--r--   0 alex       (501) staff       (20)     1836 2021-03-19 04:28:46.000000 python-dataschema-0.1.4/dataschema/utils.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-01-04 23:03:34.000000 python-dataschema-0.1.4/python_dataschema.egg-info/
--rw-r--r--   0 alex       (501) staff       (20)      359 2022-01-04 23:03:34.000000 python-dataschema-0.1.4/python_dataschema.egg-info/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)      306 2022-01-04 23:03:34.000000 python-dataschema-0.1.4/python_dataschema.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2022-01-04 23:03:34.000000 python-dataschema-0.1.4/python_dataschema.egg-info/dependency_links.txt
--rw-r--r--   0 alex       (501) staff       (20)       11 2022-01-04 23:03:34.000000 python-dataschema-0.1.4/python_dataschema.egg-info/top_level.txt
--rw-r--r--   0 alex       (501) staff       (20)       38 2022-01-04 23:03:34.000000 python-dataschema-0.1.4/setup.cfg
--rw-r--r--   0 alex       (501) staff       (20)      438 2022-01-04 22:49:30.000000 python-dataschema-0.1.4/setup.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-06-22 19:33:38.816706 python-dataschema-0.1.5/
+-rw-r--r--   0 alex       (501) staff       (20)      359 2023-06-22 19:33:38.816295 python-dataschema-0.1.5/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)     5231 2023-06-22 19:33:07.000000 python-dataschema-0.1.5/README.md
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-06-22 19:33:38.813434 python-dataschema-0.1.5/dataschema/
+-rw-r--r--   0 alex       (501) staff       (20)      479 2023-06-22 19:33:07.000000 python-dataschema-0.1.5/dataschema/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     1264 2023-06-22 19:33:07.000000 python-dataschema-0.1.5/dataschema/_utils.py
+-rw-r--r--   0 alex       (501) staff       (20)     7672 2023-06-22 19:33:07.000000 python-dataschema-0.1.5/dataschema/base.py
+-rw-r--r--   0 alex       (501) staff       (20)     1360 2023-06-22 19:33:07.000000 python-dataschema-0.1.5/dataschema/common.py
+-rw-r--r--   0 alex       (501) staff       (20)    28112 2023-06-22 19:33:07.000000 python-dataschema-0.1.5/dataschema/specs.py
+-rw-r--r--   0 alex       (501) staff       (20)     1836 2023-06-22 19:33:07.000000 python-dataschema-0.1.5/dataschema/utils.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-06-22 19:33:38.815733 python-dataschema-0.1.5/python_dataschema.egg-info/
+-rw-r--r--   0 alex       (501) staff       (20)      359 2023-06-22 19:33:38.000000 python-dataschema-0.1.5/python_dataschema.egg-info/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)      306 2023-06-22 19:33:38.000000 python-dataschema-0.1.5/python_dataschema.egg-info/SOURCES.txt
+-rw-r--r--   0 alex       (501) staff       (20)        1 2023-06-22 19:33:38.000000 python-dataschema-0.1.5/python_dataschema.egg-info/dependency_links.txt
+-rw-r--r--   0 alex       (501) staff       (20)       11 2023-06-22 19:33:38.000000 python-dataschema-0.1.5/python_dataschema.egg-info/top_level.txt
+-rw-r--r--   0 alex       (501) staff       (20)       38 2023-06-22 19:33:38.816831 python-dataschema-0.1.5/setup.cfg
+-rw-r--r--   0 alex       (501) staff       (20)      438 2023-06-22 19:33:07.000000 python-dataschema-0.1.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `python-dataschema-0.1.4/README.md` & `python-dataschema-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `python-dataschema-0.1.4/dataschema/_utils.py` & `python-dataschema-0.1.5/dataschema/_utils.py`

 * *Files identical despite different names*

### Comparing `python-dataschema-0.1.4/dataschema/base.py` & `python-dataschema-0.1.5/dataschema/base.py`

 * *Files identical despite different names*

### Comparing `python-dataschema-0.1.4/dataschema/common.py` & `python-dataschema-0.1.5/dataschema/common.py`

 * *Files identical despite different names*

### Comparing `python-dataschema-0.1.4/dataschema/specs.py` & `python-dataschema-0.1.5/dataschema/specs.py`

 * *Files 4% similar despite different names*

```diff
@@ -301,19 +301,42 @@
 
     def __init__(self,
                  type_sequence: Sequence[BaseType],
                  c_type: IterableType = tuple,
                  optional: bool = False,
                  default: Any = list,
                  is_unset: Validator = simple_is_unset,
-                 constraints: Constraints = None):
+                 constraints: Constraints = None,
+                 auto_optional: bool = False):
         self.type_sequence = type_sequence
         self.c_type = c_type
+
+        if auto_optional:
+            if optional or default is not list:
+                raise BadSchemaError('cannot pass auto_optional=True with optional or default')
+            if not type_sequence:
+                raise BadSchemaError('cannot pass auto_optional=True with empty type_sequence')
+            auto_default = self._auto_optional()
+            if auto_default:
+                optional = True
+                default = auto_default
+
         Spec.__init__(self, optional, default, is_unset, constraints)
 
+    def _auto_optional(self):
+        default_seq = []
+        for spec in self.type_sequence:
+            if isinstance(spec, Spec) and spec.optional:
+                d_value = spec.default()
+                default_seq.append(spec.check_value(d_value))
+            else:
+                default_seq.clear()
+                break
+        return self.c_type(default_seq)
+
     def type_name(self):
         return 'sequence(' + ', '.join(get_types_names(self.type_sequence)) + ')'
 
     def _check_value(self, value):
         if not isinstance(value, abc.Sequence):
             raise InvalidValueNoTypeMatch(f'Must be Sequence type')
 
@@ -492,15 +515,16 @@
                  type_key_specs: IterableSchema = None,
                  post: PostProcessing = None,
                  name: str = 'dict',
                  unhandled_ok: bool = False,
                  optional: bool = False,
                  default: Any = dict,
                  is_unset: Validator = simple_is_unset,
-                 constraints: Constraints = None):
+                 constraints: Constraints = None,
+                 auto_optional: bool = False):
         """
         ---
         schema: |
             This is mainly a convenience parameter to allow defining the DictSpec using a dict, such that the spec looks
             a lot like a valid value. Keys may either be specific values (see `value_key_specs`) as well as types
             or Specs (see `type_key_specs`). Values must always be a type or Spec.
         value_key_specs: |
@@ -529,14 +553,17 @@
         post: |
             An iterable of instances of the `Post` ABC, currently `Update` and `Test`. After the dict is considered
             "type-valid" by passing the requirements defined in the schema, additional post-processing steps can be
             applied, typically be associated with cross-references between dict keys. See `Update` and `Test` for more
             details.
         name: A string containing a canonical name for this `DictSpec`. Primarily used in error messages.
         unhandled_ok: Set to True to consider the dict valid if it contains unhandled keys after processing the schema
+        auto_optional: |
+            Set to True to make the `DictSpec` optional if all value keys are optional or if there are only
+            type keys, and auto-generate a default dict where all value keys are set to their default value.
         """
 
         if schema:
             if value_key_specs or type_key_specs:
                 raise BadSchemaError('May not specify both schema and value_key_specs/type_key_specs')
             value_key_specs, type_key_specs = self._dict_schema_to_sequences(schema)
         else:
@@ -551,16 +578,41 @@
             self.value_key_specs = tuple(value_key_specs)
         if type_key_specs:
             self.type_key_specs = tuple(type_key_specs)
         if post:
             self.post = tuple(post)
         self.name = name
         self.unhandled_ok = unhandled_ok
+
+        if auto_optional:
+            if optional or default is not dict:
+                raise BadSchemaError('cannot pass auto_optional=True with optional or default')
+            if self.value_key_specs:
+                auto_default = self._auto_optional()
+                if auto_default:
+                    optional = True
+                    default = auto_default
+            elif self.type_key_specs:
+                optional = True
+            else:
+                raise BadSchemaError('cannot pass auto_optional=True with empty schema/value_key_specs/type_key_specs')
+
         Spec.__init__(self, optional, default, is_unset, constraints)
 
+    def _auto_optional(self):
+        default_dict = {}
+        for value_key, spec in self.value_key_specs:
+            if isinstance(spec, Spec) and spec.optional:
+                d_value = spec.default()
+                default_dict[value_key] = spec.check_value(d_value)
+            else:
+                default_dict.clear()
+                break
+        return default_dict
+
     @staticmethod
     def _dict_schema_to_sequences(schema: DictSchema):
         value_key_specs = []
         type_key_specs = []
         for key, spec in schema.items():
             try:
                 type_key = canonicalize_base_type(key)
```

### Comparing `python-dataschema-0.1.4/dataschema/utils.py` & `python-dataschema-0.1.5/dataschema/utils.py`

 * *Files identical despite different names*

