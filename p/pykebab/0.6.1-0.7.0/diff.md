# Comparing `tmp/pykebab-0.6.1.tar.gz` & `tmp/pykebab-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykebab-0.6.1.tar", max compression
+gzip compressed data, was "pykebab-0.7.0.tar", max compression
```

## Comparing `pykebab-0.6.1.tar` & `pykebab-0.7.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      821 2022-11-06 03:32:21.214628 pykebab-0.6.1/kebab/__init__.py
--rw-r--r--   0        0        0     3920 2022-11-06 03:32:21.214802 pykebab-0.6.1/kebab/aws.py
--rw-r--r--   0        0        0       40 2022-11-06 03:32:21.214897 pykebab-0.6.1/kebab/cli/__init__.py
--rw-r--r--   0        0        0     1801 2023-01-05 03:45:44.147407 pykebab-0.6.1/kebab/cli/cli.py
--rw-r--r--   0        0        0      798 2023-02-03 08:02:22.409418 pykebab-0.6.1/kebab/constants.py
--rw-r--r--   0        0        0       42 2022-11-06 03:32:21.215088 pykebab-0.6.1/kebab/exceptions.py
--rw-r--r--   0        0        0     2587 2023-01-05 03:45:44.147717 pykebab-0.6.1/kebab/k8s.py
--rw-r--r--   0        0        0      773 2023-03-28 07:51:19.037015 pykebab-0.6.1/kebab/loader.py
--rw-r--r--   0        0        0     2368 2022-11-06 03:32:21.215294 pykebab-0.6.1/kebab/magic.py
--rw-r--r--   0        0        0     2108 2023-03-25 11:13:55.662982 pykebab-0.6.1/kebab/openers.py
--rw-r--r--   0        0        0    19971 2023-05-16 19:08:58.975736 pykebab-0.6.1/kebab/sources.py
--rw-r--r--   0        0        0     4825 2023-01-05 03:45:44.148106 pykebab-0.6.1/kebab/utils.py
--rw-r--r--   0        0        0     1025 2023-05-16 19:10:07.348057 pykebab-0.6.1/pyproject.toml
--rw-r--r--   0        0        0      889 1970-01-01 00:00:00.000000 pykebab-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0      821 2022-11-06 03:32:21.214628 pykebab-0.7.0/kebab/__init__.py
+-rw-r--r--   0        0        0     3920 2022-11-06 03:32:21.214802 pykebab-0.7.0/kebab/aws.py
+-rw-r--r--   0        0        0       40 2022-11-06 03:32:21.214897 pykebab-0.7.0/kebab/cli/__init__.py
+-rw-r--r--   0        0        0     1801 2023-01-05 03:45:44.147407 pykebab-0.7.0/kebab/cli/cli.py
+-rw-r--r--   0        0        0      798 2023-02-03 08:02:22.409418 pykebab-0.7.0/kebab/constants.py
+-rw-r--r--   0        0        0       42 2022-11-06 03:32:21.215088 pykebab-0.7.0/kebab/exceptions.py
+-rw-r--r--   0        0        0     2587 2023-01-05 03:45:44.147717 pykebab-0.7.0/kebab/k8s.py
+-rw-r--r--   0        0        0      773 2023-03-28 07:51:19.037015 pykebab-0.7.0/kebab/loader.py
+-rw-r--r--   0        0        0     2381 2023-06-21 14:37:29.161728 pykebab-0.7.0/kebab/magic.py
+-rw-r--r--   0        0        0     2108 2023-03-25 11:13:55.662982 pykebab-0.7.0/kebab/openers.py
+-rw-r--r--   0        0        0    21897 2023-06-22 18:44:40.594527 pykebab-0.7.0/kebab/sources.py
+-rw-r--r--   0        0        0     4825 2023-01-05 03:45:44.148106 pykebab-0.7.0/kebab/utils.py
+-rw-r--r--   0        0        0     1025 2023-06-22 18:48:02.725805 pykebab-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      889 1970-01-01 00:00:00.000000 pykebab-0.7.0/PKG-INFO
```

### Comparing `pykebab-0.6.1/kebab/__init__.py` & `pykebab-0.7.0/kebab/__init__.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.6.1/kebab/aws.py` & `pykebab-0.7.0/kebab/aws.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.6.1/kebab/cli/cli.py` & `pykebab-0.7.0/kebab/cli/cli.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.6.1/kebab/constants.py` & `pykebab-0.7.0/kebab/constants.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.6.1/kebab/k8s.py` & `pykebab-0.7.0/kebab/k8s.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.6.1/kebab/loader.py` & `pykebab-0.7.0/kebab/loader.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.6.1/kebab/magic.py` & `pykebab-0.7.0/kebab/magic.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import time
+
 from kebab.sources import KebabSource, literal
 
 
 class Field:
     def __init__(
         self,
         config_name=None,
```

### Comparing `pykebab-0.6.1/kebab/openers.py` & `pykebab-0.7.0/kebab/openers.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.6.1/kebab/sources.py` & `pykebab-0.7.0/kebab/sources.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import abc
 import copy
+import dataclasses
 import logging
 import os
 import queue  # using python-future for 2/3 compatibility
 import threading
 import time
-from typing import Any, List, Dict
+from typing import Any, List, Dict, get_type_hints, Type, TypeVar
 from urllib.request import OpenerDirector
 
 import deprecation
 # noinspection PyPackageRequirements
 from pydantic import BaseModel
 
 from kebab.constants import DEFAULT_URL_ENVVAR, DISABLE_RELOAD
@@ -187,27 +188,34 @@
     def get(
         self,
         config_name=".",
         default=None,
         required=False,
         expected_type=None,
         masked=False,
+        update_after_reload=False
     ):
         """
         :param str config_name: The key to retrieve the config value. If '.', return the
                         whole context
         :param object default: The default value to fall back to if config_name not
                         found
         :param bool required: When the required value is not found, throw exception if
                         set True, return None otherwise.
                         Default is False.
         :param type expected_type: Expected type of the value, ignored if default
                         presents.
         :param bool masked: The value will be logged as "*" if set True. This is useful
                         when a value is a secret.
+        :param bool update_after_reload: If True, the config value will be updated to
+                        the latest after the source reload periodically. Be careful:
+                        1. this could cause performance issue if the config value is
+                        retrieved frequently.
+                        2. for primitive types, the value will not be updated.
+
         :rtype str|int|bool|list[str]:
 
         Function to get a config value. This is a facade function which will retrieve
         all sources, with the following precedence:
             1. environment variable
             2. sources (a list of sources)
             3. default, if specified
@@ -219,22 +227,18 @@
         Otherwise, it could return None.
 
         Note that the type of the default becomes the expected_type if presents,
         the original expected_type will be ignored in that case.
 
         The parameter `default_value` is deprecated, use `default` instead
         """
-
-        if not config_name:
-            raise ValueError("Please specify a config_name")
-
         if default is not None:
             # set expected type based on default value (and ignore the original
             # expected_type
-            if expected_type is not None and type(default) != expected_type:
+            if expected_type is not None and not isinstance(default, expected_type):
                 raise ValueError(
                     "You specified default of type {}, but expected_type={}".format(
                         type(default), expected_type
                     )
                 )
             expected_type = type(default)
 
@@ -254,14 +258,36 @@
                 raise KeyError(f"Missing value for {config_name}")
 
         config_value = self._cast(config_value, expected_type)
 
         printed_value = "*" * len(str(config_value)) if masked else config_value
         _logger.debug(f"read config: {config_name} = {printed_value}")
 
+        if update_after_reload:
+            class KebabProxy(expected_type):
+                def __init__(self2, value):
+                    self2._value = value
+                    self2._last_eval_timestamp = time.time()
+
+                def __getattr__(self2, name):
+                    # noinspection PyProtectedMember
+                    if (
+                        name != "_last_eval_timestamp"
+                        and self2._last_eval_timestamp < self.last_reload_timestamp
+                    ):
+                        self2._value = self.get(
+                            config_name=config_name,
+                            default=default,
+                            required=required,
+                            expected_type=expected_type,
+                            masked=masked)
+                        self._last_eval_timestamp = time.time()
+                    return getattr(self2._value, name)
+            return KebabProxy(config_value)
+
         return config_value
 
     @staticmethod
     def _cast_bool(config_value: Any) -> bool:
         if isinstance(config_value, str):
             v = config_value.lower()
             if v in ("1", "true", "yes", "on", "enable"):
@@ -303,34 +329,46 @@
             elif not isinstance(config_value, expected_type):
                 if expected_type == bool:
                     return KebabSource._cast_bool(config_value)
                 elif hasattr(expected_type, "__kebab_config__"):
                     return expected_type(literal(**config_value))
                 elif issubclass(expected_type, BaseModel):
                     return expected_type(**config_value)
+                elif dataclasses.is_dataclass(expected_type):
+                    # noinspection PyTypeChecker
+                    return KebabSource._to_dataclass(expected_type, config_value)
                 else:
                     return expected_type(config_value)
         return config_value
 
-    def subsource(self, config_name, reload_interval_in_secs=DISABLE_RELOAD):
+    T = TypeVar('T')
+
+    @staticmethod
+    def _to_dataclass(data_class_type: Type[T], data: Dict[str, Any]) -> T:
+        field_types = get_type_hints(data_class_type)
+        return data_class_type(**{
+            field: KebabSource._to_dataclass(field_types[field], data[field])
+            if dataclasses.is_dataclass(field_types[field])
+            else data[field]
+            for field in data
+        })
+
+    def subsource(self, config_name):
         """
         Caveats:
 
         When parent KebabSource reloads, SubSource is not effected the updated values in
             KebabSource.
         In another word, reload in SubSource is limited and is not encouraged to use at
             the moment.
 
         :param str config_name: config_name
-        :param int|float reload_interval_in_secs: same as parent param
         :rtype: KebabSource
         """
-        source = SubSource(self, config_name)
-        source.reload(reload_interval_in_secs=reload_interval_in_secs)
-        return source
+        return SubSource(self, config_name)
 
     @deprecation.deprecated(
         deprecated_in="0.4.0",
         removed_in="0.5.0",
         details="Use the get function instead (with expected_type=config_class)",
     )
     def cast(self, config_name, config_class, *args, **kwargs):
@@ -526,14 +564,21 @@
         return f"{self.__class__.__name__}({repr(self._parent_source)})"
 
     def _load_context(self):
         return self._parent_source.get(
             self._source_name, required=True, expected_type=dict
         )
 
+    def _get_context(self):
+        return self._load_context()
+
+    @property
+    def last_reload_timestamp(self):
+        return self._parent_source.last_reload_timestamp
+
 
 def union(*sources, **kwargs):
     # """
     # The shortcut to create UnionSource
     # :param sources: a list of source to be union
     # :rtype: UnionSource
     # """
```

### Comparing `pykebab-0.6.1/kebab/utils.py` & `pykebab-0.7.0/kebab/utils.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.6.1/pyproject.toml` & `pykebab-0.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pykebab"
-version = "0.6.1"
+version = "0.7.0"
 description = ""
 authors = ["Yangming Huang <leonmax@gmail.com>"]
 packages = [
     { include = "kebab" },
 ]
 
 [tool.poetry.dependencies]
```

### Comparing `pykebab-0.6.1/PKG-INFO` & `pykebab-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykebab
-Version: 0.6.1
+Version: 0.7.0
 Summary: 
 Author: Yangming Huang
 Author-email: leonmax@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

