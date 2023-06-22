# Comparing `tmp/proto-plus-1.9.0.tar.gz` & `tmp/proto-plus-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/proto-plus-1.9.0.tar", last modified: Wed Sep  2 23:47:45 2020, max compression
+gzip compressed data, was "dist/proto-plus-1.9.1.tar", last modified: Tue Sep  8 21:32:38 2020, max compression
```

## Comparing `proto-plus-1.9.0.tar` & `proto-plus-1.9.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-02 23:47:45.476204 proto-plus-1.9.0/
--rw-r--r--   0 root         (0) root         (0)     2431 2020-09-02 23:47:45.476204 proto-plus-1.9.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1318 2020-09-02 23:47:38.000000 proto-plus-1.9.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-02 23:47:45.472204 proto-plus-1.9.0/proto/
--rw-r--r--   0 root         (0) root         (0)     1660 2020-09-02 23:47:39.000000 proto-plus-1.9.0/proto/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7874 2020-09-02 23:47:39.000000 proto-plus-1.9.0/proto/_file_info.py
--rw-r--r--   0 root         (0) root         (0)     1484 2020-09-02 23:47:39.000000 proto-plus-1.9.0/proto/_package_info.py
--rw-r--r--   0 root         (0) root         (0)     7389 2020-09-02 23:47:39.000000 proto-plus-1.9.0/proto/datetime_helpers.py
--rw-r--r--   0 root         (0) root         (0)     3759 2020-09-02 23:47:39.000000 proto-plus-1.9.0/proto/enums.py
--rw-r--r--   0 root         (0) root         (0)     5023 2020-09-02 23:47:39.000000 proto-plus-1.9.0/proto/fields.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-02 23:47:45.472204 proto-plus-1.9.0/proto/marshal/
--rw-r--r--   0 root         (0) root         (0)      630 2020-09-02 23:47:39.000000 proto-plus-1.9.0/proto/marshal/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-02 23:47:45.472204 proto-plus-1.9.0/proto/marshal/collections/
--rw-r--r--   0 root         (0) root         (0)      755 2020-09-02 23:47:39.000000 proto-plus-1.9.0/proto/marshal/collections/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2878 2020-09-02 23:47:39.000000 proto-plus-1.9.0/proto/marshal/collections/maps.py
--rw-r--r--   0 root         (0) root         (0)     4469 2020-09-02 23:47:39.000000 proto-plus-1.9.0/proto/marshal/collections/repeated.py
--rw-r--r--   0 root         (0) root         (0)     1421 2020-09-02 23:47:39.000000 proto-plus-1.9.0/proto/marshal/compat.py
--rw-r--r--   0 root         (0) root         (0)    10442 2020-09-02 23:47:39.000000 proto-plus-1.9.0/proto/marshal/marshal.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-02 23:47:45.476204 proto-plus-1.9.0/proto/marshal/rules/
--rw-r--r--   0 root         (0) root         (0)      575 2020-09-02 23:47:39.000000 proto-plus-1.9.0/proto/marshal/rules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2760 2020-09-02 23:47:39.000000 proto-plus-1.9.0/proto/marshal/rules/dates.py
--rw-r--r--   0 root         (0) root         (0)     2189 2020-09-02 23:47:39.000000 proto-plus-1.9.0/proto/marshal/rules/enums.py
--rw-r--r--   0 root         (0) root         (0)     1433 2020-09-02 23:47:39.000000 proto-plus-1.9.0/proto/marshal/rules/message.py
--rw-r--r--   0 root         (0) root         (0)     4728 2020-09-02 23:47:39.000000 proto-plus-1.9.0/proto/marshal/rules/struct.py
--rw-r--r--   0 root         (0) root         (0)     2280 2020-09-02 23:47:39.000000 proto-plus-1.9.0/proto/marshal/rules/wrappers.py
--rw-r--r--   0 root         (0) root         (0)    23058 2020-09-02 23:47:39.000000 proto-plus-1.9.0/proto/message.py
--rw-r--r--   0 root         (0) root         (0)     1544 2020-09-02 23:47:39.000000 proto-plus-1.9.0/proto/modules.py
--rw-r--r--   0 root         (0) root         (0)     1000 2020-09-02 23:47:39.000000 proto-plus-1.9.0/proto/primitives.py
--rw-r--r--   0 root         (0) root         (0)     1460 2020-09-02 23:47:39.000000 proto-plus-1.9.0/proto/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-02 23:47:45.476204 proto-plus-1.9.0/proto_plus.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2431 2020-09-02 23:47:45.000000 proto-plus-1.9.0/proto_plus.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      776 2020-09-02 23:47:45.000000 proto-plus-1.9.0/proto_plus.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-09-02 23:47:45.000000 proto-plus-1.9.0/proto_plus.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-09-02 23:47:45.000000 proto-plus-1.9.0/proto_plus.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       17 2020-09-02 23:47:45.000000 proto-plus-1.9.0/proto_plus.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2020-09-02 23:47:45.000000 proto-plus-1.9.0/proto_plus.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2020-09-02 23:47:45.476204 proto-plus-1.9.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1890 2020-09-02 23:47:39.000000 proto-plus-1.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-08 21:32:38.033587 proto-plus-1.9.1/
+-rw-r--r--   0 root         (0) root         (0)     2479 2020-09-08 21:32:38.033587 proto-plus-1.9.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1318 2020-09-08 21:32:31.000000 proto-plus-1.9.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-08 21:32:38.029587 proto-plus-1.9.1/proto/
+-rw-r--r--   0 root         (0) root         (0)     1660 2020-09-08 21:32:31.000000 proto-plus-1.9.1/proto/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6581 2020-09-08 21:32:31.000000 proto-plus-1.9.1/proto/_file_info.py
+-rw-r--r--   0 root         (0) root         (0)     1484 2020-09-08 21:32:31.000000 proto-plus-1.9.1/proto/_package_info.py
+-rw-r--r--   0 root         (0) root         (0)     7389 2020-09-08 21:32:31.000000 proto-plus-1.9.1/proto/datetime_helpers.py
+-rw-r--r--   0 root         (0) root         (0)     1546 2020-09-08 21:32:31.000000 proto-plus-1.9.1/proto/enums.py
+-rw-r--r--   0 root         (0) root         (0)     5402 2020-09-08 21:32:31.000000 proto-plus-1.9.1/proto/fields.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-08 21:32:38.033587 proto-plus-1.9.1/proto/marshal/
+-rw-r--r--   0 root         (0) root         (0)      630 2020-09-08 21:32:31.000000 proto-plus-1.9.1/proto/marshal/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-08 21:32:38.033587 proto-plus-1.9.1/proto/marshal/collections/
+-rw-r--r--   0 root         (0) root         (0)      755 2020-09-08 21:32:31.000000 proto-plus-1.9.1/proto/marshal/collections/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2878 2020-09-08 21:32:31.000000 proto-plus-1.9.1/proto/marshal/collections/maps.py
+-rw-r--r--   0 root         (0) root         (0)     4469 2020-09-08 21:32:31.000000 proto-plus-1.9.1/proto/marshal/collections/repeated.py
+-rw-r--r--   0 root         (0) root         (0)     1421 2020-09-08 21:32:31.000000 proto-plus-1.9.1/proto/marshal/compat.py
+-rw-r--r--   0 root         (0) root         (0)    10442 2020-09-08 21:32:31.000000 proto-plus-1.9.1/proto/marshal/marshal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-08 21:32:38.033587 proto-plus-1.9.1/proto/marshal/rules/
+-rw-r--r--   0 root         (0) root         (0)      575 2020-09-08 21:32:31.000000 proto-plus-1.9.1/proto/marshal/rules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2760 2020-09-08 21:32:31.000000 proto-plus-1.9.1/proto/marshal/rules/dates.py
+-rw-r--r--   0 root         (0) root         (0)     2189 2020-09-08 21:32:31.000000 proto-plus-1.9.1/proto/marshal/rules/enums.py
+-rw-r--r--   0 root         (0) root         (0)     1433 2020-09-08 21:32:31.000000 proto-plus-1.9.1/proto/marshal/rules/message.py
+-rw-r--r--   0 root         (0) root         (0)     4728 2020-09-08 21:32:31.000000 proto-plus-1.9.1/proto/marshal/rules/struct.py
+-rw-r--r--   0 root         (0) root         (0)     2280 2020-09-08 21:32:31.000000 proto-plus-1.9.1/proto/marshal/rules/wrappers.py
+-rw-r--r--   0 root         (0) root         (0)    22638 2020-09-08 21:32:31.000000 proto-plus-1.9.1/proto/message.py
+-rw-r--r--   0 root         (0) root         (0)     1544 2020-09-08 21:32:31.000000 proto-plus-1.9.1/proto/modules.py
+-rw-r--r--   0 root         (0) root         (0)     1000 2020-09-08 21:32:31.000000 proto-plus-1.9.1/proto/primitives.py
+-rw-r--r--   0 root         (0) root         (0)     1460 2020-09-08 21:32:31.000000 proto-plus-1.9.1/proto/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-08 21:32:38.033587 proto-plus-1.9.1/proto_plus.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2479 2020-09-08 21:32:37.000000 proto-plus-1.9.1/proto_plus.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      776 2020-09-08 21:32:37.000000 proto-plus-1.9.1/proto_plus.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2020-09-08 21:32:37.000000 proto-plus-1.9.1/proto_plus.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2020-09-08 21:32:37.000000 proto-plus-1.9.1/proto_plus.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       17 2020-09-08 21:32:37.000000 proto-plus-1.9.1/proto_plus.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2020-09-08 21:32:37.000000 proto-plus-1.9.1/proto_plus.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2020-09-08 21:32:38.033587 proto-plus-1.9.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1937 2020-09-08 21:32:31.000000 proto-plus-1.9.1/setup.py
```

### Comparing `proto-plus-1.9.0/PKG-INFO` & `proto-plus-1.9.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: proto-plus
-Version: 1.9.0
+Version: 1.9.1
 Summary: Beautiful, Pythonic protocol buffers.
 Home-page: https://github.com/googleapis/proto-plus-python.git
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Description: Proto Plus for Python
         =====================
@@ -41,13 +41,14 @@
         
 Platform: Posix; MacOS X
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `proto-plus-1.9.0/README.rst` & `proto-plus-1.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `proto-plus-1.9.0/proto/__init__.py` & `proto-plus-1.9.1/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `proto-plus-1.9.0/proto/_file_info.py` & `proto-plus-1.9.1/proto/_file_info.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,57 +8,34 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import collections
+import collections.abc
 import inspect
 import logging
 
-from google.protobuf import descriptor_pb2
 from google.protobuf import descriptor_pool
 from google.protobuf import message
 from google.protobuf import reflection
 
 from proto.marshal.rules.message import MessageRule
 
 log = logging.getLogger("_FileInfo")
 
 
 class _FileInfo(
     collections.namedtuple(
-        "_FileInfo",
-        ["descriptor", "messages", "enums", "name", "nested", "nested_enum"],
+        "_FileInfo", ["descriptor", "messages", "enums", "name", "nested"]
     )
 ):
     registry = {}  # Mapping[str, '_FileInfo']
 
-    @classmethod
-    def maybe_add_descriptor(cls, filename, package):
-        descriptor = cls.registry.get(filename)
-        if not descriptor:
-            descriptor = cls.registry[filename] = cls(
-                descriptor=descriptor_pb2.FileDescriptorProto(
-                    name=filename, package=package, syntax="proto3",
-                ),
-                enums=collections.OrderedDict(),
-                messages=collections.OrderedDict(),
-                name=filename,
-                nested={},
-                nested_enum={},
-            )
-
-        return descriptor
-
-    @staticmethod
-    def proto_file_name(name):
-        return "{0}.proto".format(name.replace(".", "/"))
-
     def _get_manifest(self, new_class):
         module = inspect.getmodule(new_class)
         if hasattr(module, "__protobuf__"):
             return frozenset(module.__protobuf__.manifest)
 
         return frozenset()
 
@@ -126,21 +103,14 @@
             )
 
             # Iterate over any fields on the message and, if their type
             # is a message still referenced as a string, resolve the reference.
             for field in proto_plus_message._meta.fields.values():
                 if field.message and isinstance(field.message, str):
                     field.message = self.messages[field.message]
-                elif field.enum and isinstance(field.enum, str):
-                    field.enum = self.enums[field.enum]
-
-        # Same thing for enums
-        for full_name, proto_plus_enum in self.enums.items():
-            descriptor = pool.FindEnumTypeByName(full_name)
-            proto_plus_enum._meta.pb = descriptor
 
         # We no longer need to track this file's info; remove it from
         # the module's registry and from this object.
         self.registry.pop(self.name)
 
     def ready(self, new_class):
         """Return True if a file descriptor may added, False otherwise.
@@ -156,24 +126,22 @@
 
         Args:
             new_class (~.MessageMeta): The new class currently undergoing
                 creation.
         """
         # If there are any nested descriptors that have not been assigned to
         # the descriptors that should contain them, then we are not ready.
-        if len(self.nested) or len(self.nested_enum):
+        if len(self.nested):
             return False
 
         # If there are any unresolved fields (fields with a composite message
         # declared as a string), ensure that the corresponding message is
         # declared.
         for field in self.unresolved_fields:
-            if (field.message and field.message not in self.messages) or (
-                field.enum and field.enum not in self.enums
-            ):
+            if field.message not in self.messages:
                 return False
 
         # If the module in which this class is defined provides a
         # __protobuf__ property, it may have a manifest.
         #
         # Do not generate the file descriptor until every member of the
         # manifest has been populated.
@@ -184,11 +152,9 @@
         return all(hasattr(module, i) for i in manifest)
 
     @property
     def unresolved_fields(self):
         """Return fields with referencing message types as strings."""
         for proto_plus_message in self.messages.values():
             for field in proto_plus_message._meta.fields.values():
-                if (field.message and isinstance(field.message, str)) or (
-                    field.enum and isinstance(field.enum, str)
-                ):
+                if field.message and isinstance(field.message, str):
                     yield field
```

### Comparing `proto-plus-1.9.0/proto/_package_info.py` & `proto-plus-1.9.1/proto/_package_info.py`

 * *Files identical despite different names*

### Comparing `proto-plus-1.9.0/proto/datetime_helpers.py` & `proto-plus-1.9.1/proto/datetime_helpers.py`

 * *Files identical despite different names*

### Comparing `proto-plus-1.9.0/proto/fields.py` & `proto-plus-1.9.1/proto/fields.py`

 * *Files 9% similar despite different names*

```diff
@@ -68,43 +68,50 @@
         # types are written later.
         self._descriptor = None
 
     @property
     def descriptor(self):
         """Return the descriptor for the field."""
         if not self._descriptor:
+            proto_type = self.proto_type
             # Resolve the message type, if any, to a string.
             type_name = None
             if isinstance(self.message, str):
                 if not self.message.startswith(self.package):
                     self.message = "{package}.{name}".format(
                         package=self.package, name=self.message,
                     )
                 type_name = self.message
             elif self.message:
                 type_name = (
                     self.message.DESCRIPTOR.full_name
                     if hasattr(self.message, "DESCRIPTOR")
-                    else self.message._meta.full_name
+                    else self.message.meta.full_name
                 )
-            elif isinstance(self.enum, str):
-                if not self.enum.startswith(self.package):
-                    self.enum = "{package}.{name}".format(
-                        package=self.package, name=self.enum,
-                    )
-                type_name = self.enum
             elif self.enum:
-                type_name = self.enum._meta.full_name
+                # Nos decipiat.
+                #
+                # As far as the wire format is concerned, enums are int32s.
+                # Protocol buffers itself also only sends ints; the enum
+                # objects are simply helper classes for translating names
+                # and values and it is the user's job to resolve to an int.
+                #
+                # Therefore, the non-trivial effort of adding the actual
+                # enum descriptors seems to add little or no actual value.
+                #
+                # FIXME: Eventually, come back and put in the actual enum
+                # descriptors.
+                proto_type = ProtoType.INT32
 
             # Set the descriptor.
             self._descriptor = descriptor_pb2.FieldDescriptorProto(
                 name=self.name,
                 number=self.number,
                 label=3 if self.repeated else 1,
-                type=self.proto_type,
+                type=proto_type,
                 type_name=type_name,
                 json_name=self.json_name,
                 proto3_optional=self.optional,
             )
 
         # Return the descriptor.
         return self._descriptor
```

### Comparing `proto-plus-1.9.0/proto/marshal/__init__.py` & `proto-plus-1.9.1/proto/marshal/__init__.py`

 * *Files identical despite different names*

### Comparing `proto-plus-1.9.0/proto/marshal/collections/__init__.py` & `proto-plus-1.9.1/proto/marshal/collections/__init__.py`

 * *Files identical despite different names*

### Comparing `proto-plus-1.9.0/proto/marshal/collections/maps.py` & `proto-plus-1.9.1/proto/marshal/collections/maps.py`

 * *Files identical despite different names*

### Comparing `proto-plus-1.9.0/proto/marshal/collections/repeated.py` & `proto-plus-1.9.1/proto/marshal/collections/repeated.py`

 * *Files identical despite different names*

### Comparing `proto-plus-1.9.0/proto/marshal/compat.py` & `proto-plus-1.9.1/proto/marshal/compat.py`

 * *Files identical despite different names*

### Comparing `proto-plus-1.9.0/proto/marshal/marshal.py` & `proto-plus-1.9.1/proto/marshal/marshal.py`

 * *Files identical despite different names*

### Comparing `proto-plus-1.9.0/proto/marshal/rules/__init__.py` & `proto-plus-1.9.1/proto/marshal/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `proto-plus-1.9.0/proto/marshal/rules/dates.py` & `proto-plus-1.9.1/proto/marshal/rules/dates.py`

 * *Files identical despite different names*

### Comparing `proto-plus-1.9.0/proto/marshal/rules/enums.py` & `proto-plus-1.9.1/proto/marshal/rules/enums.py`

 * *Files identical despite different names*

### Comparing `proto-plus-1.9.0/proto/marshal/rules/message.py` & `proto-plus-1.9.1/proto/marshal/rules/message.py`

 * *Files identical despite different names*

### Comparing `proto-plus-1.9.0/proto/marshal/rules/struct.py` & `proto-plus-1.9.1/proto/marshal/rules/struct.py`

 * *Files identical despite different names*

### Comparing `proto-plus-1.9.0/proto/marshal/rules/wrappers.py` & `proto-plus-1.9.1/proto/marshal/rules/wrappers.py`

 * *Files identical despite different names*

### Comparing `proto-plus-1.9.0/proto/message.py` & `proto-plus-1.9.1/proto/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,29 +141,24 @@
             # If this field references a message, it may be from another
             # proto file; ensure we know about the import (to faithfully
             # construct our file descriptor proto).
             if field.message and not isinstance(field.message, str):
                 field_msg = field.message
                 if hasattr(field_msg, "pb") and callable(field_msg.pb):
                     field_msg = field_msg.pb()
+
                 # Sanity check: The field's message may not yet be defined if
                 # it was a Message defined in the same file, and the file
                 # descriptor proto has not yet been generated.
                 #
                 # We do nothing in this situation; everything will be handled
                 # correctly when the file descriptor is created later.
                 if field_msg:
                     proto_imports.add(field_msg.DESCRIPTOR.file.name)
-
-            # Same thing, but for enums.
-            elif field.enum and not isinstance(field.enum, str):
-                field_enum = field.enum._meta.pb
-
-                if field_enum:
-                    proto_imports.add(field_enum.file.name)
+                    symbol_database.Default().RegisterMessage(field_msg)
 
             # Increment the field index counter.
             index += 1
 
         # As per descriptor.proto, all synthetic oneofs must be ordered after
         # 'real' oneofs.
         opt_attrs = {}
@@ -184,21 +179,32 @@
         # MyMessage.field in m
         if opt_attrs:
             mcls = type("AttrsMeta", (mcls,), opt_attrs)
 
         # Determine the filename.
         # We determine an appropriate proto filename based on the
         # Python module.
-        filename = _file_info._FileInfo.proto_file_name(
-            new_attrs.get("__module__", name.lower())
+        filename = "{0}.proto".format(
+            new_attrs.get("__module__", name.lower()).replace(".", "/")
         )
 
         # Get or create the information about the file, including the
         # descriptor to which the new message descriptor shall be added.
-        file_info = _file_info._FileInfo.maybe_add_descriptor(filename, package)
+        file_info = _file_info._FileInfo.registry.setdefault(
+            filename,
+            _file_info._FileInfo(
+                descriptor=descriptor_pb2.FileDescriptorProto(
+                    name=filename, package=package, syntax="proto3",
+                ),
+                enums=collections.OrderedDict(),
+                messages=collections.OrderedDict(),
+                name=filename,
+                nested={},
+            ),
+        )
 
         # Ensure any imports that would be necessary are assigned to the file
         # descriptor proto being created.
         for proto_import in proto_imports:
             if proto_import not in file_info.descriptor.dependency:
                 file_info.descriptor.dependency.append(proto_import)
 
@@ -217,19 +223,14 @@
 
         # If any descriptors were nested under this one, they need to be
         # attached as nested types here.
         child_paths = [p for p in file_info.nested.keys() if local_path == p[:-1]]
         for child_path in child_paths:
             desc.nested_type.add().MergeFrom(file_info.nested.pop(child_path))
 
-        # Same thing, but for enums
-        child_paths = [p for p in file_info.nested_enum.keys() if local_path == p[:-1]]
-        for child_path in child_paths:
-            desc.enum_type.add().MergeFrom(file_info.nested_enum.pop(child_path))
-
         # Add the descriptor to the file if it is a top-level descriptor,
         # or to a "holding area" for nested messages otherwise.
         if len(local_path) == 1:
             file_info.descriptor.message_type.add().MergeFrom(desc)
         else:
             file_info.nested[local_path] = desc
 
@@ -320,32 +321,25 @@
 
         Returns:
             ~.Message: An instance of the message class against which this
             method was called.
         """
         return cls.wrap(cls.pb().FromString(payload))
 
-    def to_json(cls, instance, *, use_integers_for_enums=True) -> str:
+    def to_json(cls, instance) -> str:
         """Given a message instance, serialize it to json
 
         Args:
             instance: An instance of this message type, or something
                 compatible (accepted by the type's constructor).
-            use_integers_for_enums (Optional(bool)): An option that determines whether enum
-                values should be represented by strings (False) or integers (True).
-                Default is True.
 
         Returns:
             str: The json string representation of the protocol buffer.
         """
-        return MessageToJson(
-            cls.pb(instance),
-            use_integers_for_enums=use_integers_for_enums,
-            including_default_value_fields=True,
-        )
+        return MessageToJson(cls.pb(instance))
 
     def from_json(cls, payload) -> "Message":
         """Given a json string representing an instance,
         parse it into a message.
 
         Args:
             paylod: A json string representing a message.
```

### Comparing `proto-plus-1.9.0/proto/modules.py` & `proto-plus-1.9.1/proto/modules.py`

 * *Files identical despite different names*

### Comparing `proto-plus-1.9.0/proto/primitives.py` & `proto-plus-1.9.1/proto/primitives.py`

 * *Files identical despite different names*

### Comparing `proto-plus-1.9.0/proto/utils.py` & `proto-plus-1.9.1/proto/utils.py`

 * *Files identical despite different names*

### Comparing `proto-plus-1.9.0/proto_plus.egg-info/PKG-INFO` & `proto-plus-1.9.1/proto_plus.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: proto-plus
-Version: 1.9.0
+Version: 1.9.1
 Summary: Beautiful, Pythonic protocol buffers.
 Home-page: https://github.com/googleapis/proto-plus-python.git
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Description: Proto Plus for Python
         =====================
@@ -41,13 +41,14 @@
         
 Platform: Posix; MacOS X
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `proto-plus-1.9.0/proto_plus.egg-info/SOURCES.txt` & `proto-plus-1.9.1/proto_plus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `proto-plus-1.9.0/setup.py` & `proto-plus-1.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 import io
 import os
 
 from setuptools import find_packages, setup
 
-version = "1.9.0"
+version = "1.9.1"
 
 PACKAGE_ROOT = os.path.abspath(os.path.dirname(__file__))
 
 with io.open(os.path.join(PACKAGE_ROOT, "README.rst")) as file_obj:
     README = file_obj.read()
 
 setup(
@@ -39,14 +39,15 @@
     install_requires=("protobuf >= 3.12.0",),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: POSIX",
+        "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Topic :: Software Development :: Code Generators",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
```

