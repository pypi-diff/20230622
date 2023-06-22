# Comparing `tmp/drf-serializer-prefetch-1.0.8.tar.gz` & `tmp/drf-serializer-prefetch-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-serializer-prefetch-1.0.8.tar", last modified: Wed Jun 21 19:04:53 2023, max compression
+gzip compressed data, was "drf-serializer-prefetch-1.0.9.tar", last modified: Thu Jun 22 20:25:03 2023, max compression
```

## Comparing `drf-serializer-prefetch-1.0.8.tar` & `drf-serializer-prefetch-1.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-21 19:04:53.209857 drf-serializer-prefetch-1.0.8/
--rw-rw-r--   0 max       (1000) max       (1000)     1073 2023-06-20 13:02:29.000000 drf-serializer-prefetch-1.0.8/LICENSE
--rw-rw-r--   0 max       (1000) max       (1000)     9342 2023-06-21 19:04:53.209857 drf-serializer-prefetch-1.0.8/PKG-INFO
--rw-rw-r--   0 max       (1000) max       (1000)     8990 2023-06-21 19:04:46.000000 drf-serializer-prefetch-1.0.8/README.md
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-21 19:04:53.209857 drf-serializer-prefetch-1.0.8/drf_serializer_prefetch.egg-info/
--rw-rw-r--   0 max       (1000) max       (1000)     9342 2023-06-21 19:04:53.000000 drf-serializer-prefetch-1.0.8/drf_serializer_prefetch.egg-info/PKG-INFO
--rw-rw-r--   0 max       (1000) max       (1000)      465 2023-06-21 19:04:53.000000 drf-serializer-prefetch-1.0.8/drf_serializer_prefetch.egg-info/SOURCES.txt
--rw-rw-r--   0 max       (1000) max       (1000)        1 2023-06-21 19:04:53.000000 drf-serializer-prefetch-1.0.8/drf_serializer_prefetch.egg-info/dependency_links.txt
--rw-rw-r--   0 max       (1000) max       (1000)       40 2023-06-21 19:04:53.000000 drf-serializer-prefetch-1.0.8/drf_serializer_prefetch.egg-info/requires.txt
--rw-rw-r--   0 max       (1000) max       (1000)       26 2023-06-21 19:04:53.000000 drf-serializer-prefetch-1.0.8/drf_serializer_prefetch.egg-info/top_level.txt
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-21 19:04:53.209857 drf-serializer-prefetch-1.0.8/serializer_prefetch/
--rw-rw-r--   0 max       (1000) max       (1000)      139 2023-06-20 14:41:43.000000 drf-serializer-prefetch-1.0.8/serializer_prefetch/__init__.py
--rw-rw-r--   0 max       (1000) max       (1000)    12459 2023-06-21 15:38:51.000000 drf-serializer-prefetch-1.0.8/serializer_prefetch/base.py
--rw-rw-r--   0 max       (1000) max       (1000)       38 2023-06-21 19:04:53.209857 drf-serializer-prefetch-1.0.8/setup.cfg
--rw-rw-r--   0 max       (1000) max       (1000)      679 2023-06-21 19:03:35.000000 drf-serializer-prefetch-1.0.8/setup.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-21 19:04:53.209857 drf-serializer-prefetch-1.0.8/tests/
--rw-rw-r--   0 max       (1000) max       (1000)        0 2023-06-20 15:59:03.000000 drf-serializer-prefetch-1.0.8/tests/__init__.py
--rw-rw-r--   0 max       (1000) max       (1000)      515 2023-06-21 13:57:02.000000 drf-serializer-prefetch-1.0.8/tests/models.py
--rw-rw-r--   0 max       (1000) max       (1000)      708 2023-06-21 14:24:52.000000 drf-serializer-prefetch-1.0.8/tests/serializers.py
--rw-rw-r--   0 max       (1000) max       (1000)      381 2023-06-20 18:58:38.000000 drf-serializer-prefetch-1.0.8/tests/settings.py
--rw-rw-r--   0 max       (1000) max       (1000)     4003 2023-06-21 15:25:58.000000 drf-serializer-prefetch-1.0.8/tests/test_conditions.py
--rw-rw-r--   0 max       (1000) max       (1000)     2404 2023-06-21 15:24:05.000000 drf-serializer-prefetch-1.0.8/tests/test_errors.py
--rw-rw-r--   0 max       (1000) max       (1000)    16527 2023-06-21 15:38:39.000000 drf-serializer-prefetch-1.0.8/tests/test_serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:03.977120 drf-serializer-prefetch-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-22 20:24:53.000000 drf-serializer-prefetch-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9305 2023-06-22 20:25:03.977120 drf-serializer-prefetch-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8990 2023-06-22 20:24:53.000000 drf-serializer-prefetch-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:03.973120 drf-serializer-prefetch-1.0.9/drf_serializer_prefetch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9305 2023-06-22 20:25:03.000000 drf-serializer-prefetch-1.0.9/drf_serializer_prefetch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-22 20:25:03.000000 drf-serializer-prefetch-1.0.9/drf_serializer_prefetch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 20:25:03.000000 drf-serializer-prefetch-1.0.9/drf_serializer_prefetch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-22 20:25:03.000000 drf-serializer-prefetch-1.0.9/drf_serializer_prefetch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-22 20:25:03.000000 drf-serializer-prefetch-1.0.9/drf_serializer_prefetch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:03.973120 drf-serializer-prefetch-1.0.9/serializer_prefetch/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-22 20:24:53.000000 drf-serializer-prefetch-1.0.9/serializer_prefetch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12465 2023-06-22 20:24:53.000000 drf-serializer-prefetch-1.0.9/serializer_prefetch/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 20:25:03.977120 drf-serializer-prefetch-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-22 20:24:53.000000 drf-serializer-prefetch-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:03.973120 drf-serializer-prefetch-1.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:24:53.000000 drf-serializer-prefetch-1.0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-22 20:24:53.000000 drf-serializer-prefetch-1.0.9/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-22 20:24:53.000000 drf-serializer-prefetch-1.0.9/tests/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-22 20:24:53.000000 drf-serializer-prefetch-1.0.9/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-06-22 20:24:53.000000 drf-serializer-prefetch-1.0.9/tests/test_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-06-22 20:24:53.000000 drf-serializer-prefetch-1.0.9/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16527 2023-06-22 20:24:53.000000 drf-serializer-prefetch-1.0.9/tests/test_serializers.py
```

### Comparing `drf-serializer-prefetch-1.0.8/LICENSE` & `drf-serializer-prefetch-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `drf-serializer-prefetch-1.0.8/PKG-INFO` & `drf-serializer-prefetch-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: drf-serializer-prefetch
-Version: 1.0.8
+Version: 1.0.9
 Summary: An automatic prefetcher for django-rest-framework.
 Home-page: https://github.com/MaxDude132/drf-serializer-prefetch
 Author: Maxime Toussaint
 Author-email: m.toussaint@mail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![codecov](https://codecov.io/gh/MaxDude132/drf-serializer-prefetch/branch/main/graph/badge.svg?token=MFI4E7L7SU)](https://codecov.io/gh/MaxDude132/drf-serializer-prefetch)
 
 # drf-serializer-prefetch
 
@@ -206,9 +204,7 @@
 ```
 
 The same logic can be applied to other libraries that could need to interact with the queryset between the time it is prefetched and the time it is split into models. Note that `queryset_after_prefetch` is only ever called if the instance passed to the ListSerializer is a Queryset, so you do not need to worry about checking for the type. Similarly, `call_to_representation` is only called if some prefetching was done. If none was done, either because it was not the furthermost parent or because auto_prefetch has been set to `False`, then this method will not be called. If you need a method to always be called, you can define a `to_representation` method in the new `PrefetchingListSerializer` you defined. Do not forget to call the super method!
 
 ## Important note
 
 While the Prefetching Serializer does work on regular django-rest-framework serializers, it is really intended to be used with their `ModelSerializer`. If you do use it with a regular Serializer, you will need to define `select_related` and `prefetch_related` for all the fields used. Note that this is still better than having the logic in `get_queryset` in the viewset, as it is kept with its own serializer and will be used properly if the serializer is nested.
-
-
```

### Comparing `drf-serializer-prefetch-1.0.8/README.md` & `drf-serializer-prefetch-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `drf-serializer-prefetch-1.0.8/drf_serializer_prefetch.egg-info/PKG-INFO` & `drf-serializer-prefetch-1.0.9/drf_serializer_prefetch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: drf-serializer-prefetch
-Version: 1.0.8
+Version: 1.0.9
 Summary: An automatic prefetcher for django-rest-framework.
 Home-page: https://github.com/MaxDude132/drf-serializer-prefetch
 Author: Maxime Toussaint
 Author-email: m.toussaint@mail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![codecov](https://codecov.io/gh/MaxDude132/drf-serializer-prefetch/branch/main/graph/badge.svg?token=MFI4E7L7SU)](https://codecov.io/gh/MaxDude132/drf-serializer-prefetch)
 
 # drf-serializer-prefetch
 
@@ -206,9 +204,7 @@
 ```
 
 The same logic can be applied to other libraries that could need to interact with the queryset between the time it is prefetched and the time it is split into models. Note that `queryset_after_prefetch` is only ever called if the instance passed to the ListSerializer is a Queryset, so you do not need to worry about checking for the type. Similarly, `call_to_representation` is only called if some prefetching was done. If none was done, either because it was not the furthermost parent or because auto_prefetch has been set to `False`, then this method will not be called. If you need a method to always be called, you can define a `to_representation` method in the new `PrefetchingListSerializer` you defined. Do not forget to call the super method!
 
 ## Important note
 
 While the Prefetching Serializer does work on regular django-rest-framework serializers, it is really intended to be used with their `ModelSerializer`. If you do use it with a regular Serializer, you will need to define `select_related` and `prefetch_related` for all the fields used. Note that this is still better than having the logic in `get_queryset` in the viewset, as it is kept with its own serializer and will be used properly if the serializer is nested.
-
-
```

### Comparing `drf-serializer-prefetch-1.0.8/serializer_prefetch/base.py` & `drf-serializer-prefetch-1.0.9/serializer_prefetch/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -221,24 +221,24 @@
     def _build_computed_related(self, related_attr, current_relation):
         return [
             self._get_joined_prefetch(current_relation, item) for item in related_attr
         ]
 
 
 class List(list):
-    _braindate_prefetch_done = False
+    _serializer_prefetch_done = False
 
 
 class PrefetchingListSerializer(PrefetchingLogicMixin, serializers.ListSerializer):
     def __init__(self, *args, auto_prefetch=True, **kwargs):
         self._auto_prefetch = auto_prefetch
         super().__init__(*args, **kwargs)
 
     def to_representation(self, instance, *args, **kwargs):
-        prefetch_done = getattr(instance, "_braindate_prefetch_done", False)
+        prefetch_done = getattr(instance, "_serializer_prefetch_done", False)
         if prefetch_done or self.parent is not None or not self._auto_prefetch:
             return super().to_representation(instance)
 
         child = self.child
         select_items, prefetch_items = self.get_prefetch(child)
 
         if isinstance(instance, QuerySet):
@@ -257,30 +257,30 @@
 
             for related_lookup in set(select_items + prefetch_items):
                 prefetch_related_objects(instance, related_lookup)
 
         if isinstance(instance, list):
             instance = List(instance)
 
-        instance._braindate_prefetch_done = True
+        instance._serializer_prefetch_done = True
 
         self.call_other_prefetching_methods()
 
         return self.call_to_representation(instance)
 
 
 class Dict(dict):
-    _braindate_prefetch_done = False
+    _serializer_prefetch_done = False
 
 
 class PrefetchingSerializerMixin(PrefetchingLogicMixin):
     default_list_serializer_class = PrefetchingListSerializer
 
     def to_representation(self, instance, *args, **kwargs):
-        prefetch_done = getattr(instance, "_braindate_prefetch_done", False)
+        prefetch_done = getattr(instance, "_serializer_prefetch_done", False)
         if (
             not prefetch_done
             and self._auto_prefetch
             and not self.parent
             and not getattr(instance, "_prefetched_objects_cache", None)
         ):
             select_items, prefetch_items = self.get_prefetch(self)
@@ -294,15 +294,15 @@
                             "Got an AttributeError. You might have forgotten to "
                             "add `many=True` on the serializer."
                         )
                     ) from exc
 
             if isinstance(instance, dict):
                 instance = Dict(instance)
-            instance._braindate_prefetch_done = True
+            instance._serializer_prefetch_done = True
 
             self.call_other_prefetching_methods()
 
             if isinstance(instance, Model):
                 return self.call_to_representation(instance)
 
         return super().to_representation(instance)
```

### Comparing `drf-serializer-prefetch-1.0.8/setup.py` & `drf-serializer-prefetch-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
 from setuptools import setup, find_packages
 
 
-VERSION = "1.0.8"
+VERSION = "1.0.9"
 DESCRIPTION = "An automatic prefetcher for django-rest-framework."
 this_directory = Path(__file__).parent
 LONG_DESCRIPTION = (this_directory / "README.md").read_text()
 
 setup(
     name="drf-serializer-prefetch",
     version=VERSION,
```

### Comparing `drf-serializer-prefetch-1.0.8/tests/models.py` & `drf-serializer-prefetch-1.0.9/tests/models.py`

 * *Files identical despite different names*

### Comparing `drf-serializer-prefetch-1.0.8/tests/serializers.py` & `drf-serializer-prefetch-1.0.9/tests/serializers.py`

 * *Files identical despite different names*

### Comparing `drf-serializer-prefetch-1.0.8/tests/test_conditions.py` & `drf-serializer-prefetch-1.0.9/tests/test_conditions.py`

 * *Files identical despite different names*

### Comparing `drf-serializer-prefetch-1.0.8/tests/test_errors.py` & `drf-serializer-prefetch-1.0.9/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `drf-serializer-prefetch-1.0.8/tests/test_serializers.py` & `drf-serializer-prefetch-1.0.9/tests/test_serializers.py`

 * *Files identical despite different names*

