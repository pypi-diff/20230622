# Comparing `tmp/superpathlib-1.0.1.tar.gz` & `tmp/superpathlib-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superpathlib-1.0.1.tar", last modified: Mon Apr 24 04:31:06 2023, max compression
+gzip compressed data, was "superpathlib-1.0.2.tar", last modified: Thu Jun 22 13:46:35 2023, max compression
```

## Comparing `superpathlib-1.0.1.tar` & `superpathlib-1.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-04-24 04:31:06.834797 superpathlib-1.0.1/
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     1069 2023-04-24 04:20:41.000000 superpathlib-1.0.1/LICENSE
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     2808 2023-04-24 04:31:06.834797 superpathlib-1.0.1/PKG-INFO
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     2511 2023-04-24 04:20:41.000000 superpathlib-1.0.1/README.md
-drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-04-24 04:31:06.834797 superpathlib-1.0.1/plib/
--rw-rw-r--   0 quinten   (1000) quinten   (1000)       23 2023-04-24 04:20:41.000000 superpathlib-1.0.1/plib/__init__.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)    15026 2023-04-24 04:25:02.000000 superpathlib-1.0.1/plib/plib.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     1152 2023-04-24 04:20:41.000000 superpathlib-1.0.1/plib/tags.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      808 2023-04-24 04:20:41.000000 superpathlib-1.0.1/plib/utils.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      549 2023-04-24 04:31:06.834797 superpathlib-1.0.1/setup.cfg
--rw-rw-r--   0 quinten   (1000) quinten   (1000)       69 2023-04-24 04:20:41.000000 superpathlib-1.0.1/setup.py
-drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-04-24 04:31:06.834797 superpathlib-1.0.1/superpathlib.egg-info/
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     2808 2023-04-24 04:31:06.000000 superpathlib-1.0.1/superpathlib.egg-info/PKG-INFO
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      353 2023-04-24 04:31:06.000000 superpathlib-1.0.1/superpathlib.egg-info/SOURCES.txt
--rw-rw-r--   0 quinten   (1000) quinten   (1000)        1 2023-04-24 04:31:06.000000 superpathlib-1.0.1/superpathlib.egg-info/dependency_links.txt
--rw-rw-r--   0 quinten   (1000) quinten   (1000)        7 2023-04-24 04:31:06.000000 superpathlib-1.0.1/superpathlib.egg-info/requires.txt
--rw-rw-r--   0 quinten   (1000) quinten   (1000)        5 2023-04-24 04:31:06.000000 superpathlib-1.0.1/superpathlib.egg-info/top_level.txt
-drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-04-24 04:31:06.834797 superpathlib-1.0.1/tests/
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     4150 2023-04-24 04:20:41.000000 superpathlib-1.0.1/tests/test_content.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     1532 2023-04-24 04:20:41.000000 superpathlib-1.0.1/tests/test_functionality.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     1271 2023-04-24 04:20:41.000000 superpathlib-1.0.1/tests/test_metadata.py
+drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-06-22 13:46:35.651064 superpathlib-1.0.2/
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     1069 2023-06-22 09:35:22.000000 superpathlib-1.0.2/LICENSE
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     2975 2023-06-22 13:46:35.647064 superpathlib-1.0.2/PKG-INFO
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     2630 2023-06-22 10:13:57.000000 superpathlib-1.0.2/README.md
+drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-06-22 13:46:35.647064 superpathlib-1.0.2/plib/
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)       23 2023-06-22 09:35:22.000000 superpathlib-1.0.2/plib/__init__.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)    15354 2023-06-22 13:45:28.000000 superpathlib-1.0.2/plib/plib.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     1152 2023-06-22 09:35:22.000000 superpathlib-1.0.2/plib/tags.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      857 2023-06-22 13:42:15.000000 superpathlib-1.0.2/plib/utils.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      559 2023-06-22 10:17:00.000000 superpathlib-1.0.2/pyproject.toml
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)       38 2023-06-22 13:46:35.651064 superpathlib-1.0.2/setup.cfg
+drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-06-22 13:46:35.647064 superpathlib-1.0.2/superpathlib.egg-info/
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     2975 2023-06-22 13:46:35.000000 superpathlib-1.0.2/superpathlib.egg-info/PKG-INFO
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      406 2023-06-22 13:46:35.000000 superpathlib-1.0.2/superpathlib.egg-info/SOURCES.txt
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)        1 2023-06-22 13:46:35.000000 superpathlib-1.0.2/superpathlib.egg-info/dependency_links.txt
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)       69 2023-06-22 13:46:35.000000 superpathlib-1.0.2/superpathlib.egg-info/requires.txt
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)        5 2023-06-22 13:46:35.000000 superpathlib-1.0.2/superpathlib.egg-info/top_level.txt
+drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-06-22 13:46:35.647064 superpathlib-1.0.2/tests/
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     4483 2023-06-22 09:59:18.000000 superpathlib-1.0.2/tests/test_content.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     1532 2023-06-22 09:35:22.000000 superpathlib-1.0.2/tests/test_functionality.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     1271 2023-06-22 09:35:22.000000 superpathlib-1.0.2/tests/test_metadata.py
```

### Comparing `superpathlib-1.0.1/LICENSE` & `superpathlib-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `superpathlib-1.0.1/PKG-INFO` & `superpathlib-1.0.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: superpathlib
-Version: 1.0.1
-Summary: extended pathlib
-Home-page: https://github.com/quintenroets/superpathlib
-Author: Quinten Roets
-Author-email: quinten.roets@gmail.com
-License: MIT
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Superpathlib
 Superpathlib offers Path objects with functionality extended from pathlib to maximize your productivity with a minimal amount of code.
 
 ## Usage
 
 ```shell
 from plib import Path
@@ -22,14 +10,15 @@
 
 ### 1) Use properties to read & write path content in different formats
 * text
 * byte_content
 * lines
 * yaml
 * json
+* numpy
 
 examples: 
 
 ```shell
 path.json = {key: value}
 
 for line in path.lines:
@@ -106,9 +95,12 @@
 This only works if you inherit from plib and not from the builtin pathlib
 
 
 ## Installation
 
 ```shell
 pip install superpathlib
-requires python version >= 3.9
 ```
+
+Install the packages corresponding with the properties you want to use
+* e.g. PyYaml for yaml property
+* Packages listed in requirements.txt
```

### Comparing `superpathlib-1.0.1/README.md` & `superpathlib-1.0.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: superpathlib
+Version: 1.0.2
+Summary: Extended Pathlib
+Author-email: Quinten Roets <qdr2104@columbia.edu>
+License: MIT
+Project-URL: Source Code, https://github.com/quintenroets/superpathlib
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: test
+License-File: LICENSE
+
 # Superpathlib
 Superpathlib offers Path objects with functionality extended from pathlib to maximize your productivity with a minimal amount of code.
 
 ## Usage
 
 ```shell
 from plib import Path
@@ -10,14 +23,15 @@
 
 ### 1) Use properties to read & write path content in different formats
 * text
 * byte_content
 * lines
 * yaml
 * json
+* numpy
 
 examples: 
 
 ```shell
 path.json = {key: value}
 
 for line in path.lines:
@@ -94,9 +108,12 @@
 This only works if you inherit from plib and not from the builtin pathlib
 
 
 ## Installation
 
 ```shell
 pip install superpathlib
-requires python version >= 3.9
 ```
+
+Install the packages corresponding with the properties you want to use
+* e.g. PyYaml for yaml property
+* Packages listed in requirements.txt
```

### Comparing `superpathlib-1.0.1/plib/plib.py` & `superpathlib-1.0.2/plib/plib.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from functools import cached_property, wraps
 from typing import Any
 
 from .utils import find_first_match
 
 # Long import times relative to their usage frequency: lazily imported
 # import yaml
-# from datatime import datetime
+# from datetime import datetime
 # from .tags import XDGTags
 
 
 def catch_missing(default=None):
     def wrap_function(func):
         @wraps(func)
         def wrap_args(*args, **kwargs):
@@ -64,17 +64,16 @@
     """Extend pathlib functionality and enable further extensions by
     inheriting.
     """
 
     _flavour = (
         pathlib._windows_flavour if os.name == "nt" else pathlib._posix_flavour
     )  # _flavour attribute needs to inherited explicitely from pathlib
-
-    """
-    Overwrite existing methods with exception handling and default values
+    """Overwrite existing methods with exception handling and default
+    values.
     """
 
     @create_parent_on_missing
     def touch(self, mode=0o666, exist_ok=True, mtime=None):
         super().touch(mode=mode, exist_ok=exist_ok)
         if mtime is not None:
             self.mtime = mtime  # set time after touch or it is immediately overwritten
@@ -192,14 +191,28 @@
         import yaml  # noqa: autoimport
 
         # C implementation much faster but only supported on Linux
         Dumper = yaml.CDumper if hasattr(yaml, "CDumper") else yaml.Dumper
         self.text = yaml.dump(value, Dumper=Dumper, width=1024)
 
     @property
+    def numpy(self):
+        import numpy as np  # noqa: autoimport
+
+        with self.open("rb") as fp:
+            return np.load(fp)  # noqa
+
+    @numpy.setter
+    def numpy(self, value):
+        import numpy as np  # noqa: autoimport
+
+        with self.open("wb") as fp:
+            np.save(fp, value)  # noqa
+
+    @property
     def encrypted(self):
         path = self
         encryption_suffix = ".gpg"
         if path.suffix != encryption_suffix:
             path = path.with_suffix(path.suffix + encryption_suffix)
         return EncryptedPath(path)
```

### Comparing `superpathlib-1.0.1/plib/tags.py` & `superpathlib-1.0.2/plib/tags.py`

 * *Files identical despite different names*

### Comparing `superpathlib-1.0.1/plib/utils.py` & `superpathlib-1.0.2/plib/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,25 @@
-from typing import Callable
+from collections.abc import Callable
 
 
 def find_first_match(condition: Callable) -> int:
     """
     :param condition: Condition that number needs to match.
-                      The condition is assumed to be valid for all integers staring from an initial value.
+                      The condition is assumed to be valid for all integers staring
+                      from an initial value.
     :return: First integer for which condition is valid.
     """
 
     # exponential increase for logarithmic search
     upper_bound = 1
     while not condition(upper_bound):
         upper_bound *= 2
 
-    # narrow down range of first match = [lower_bound + 1, upper_bound] until one value left
+    # first match = [lower_bound + 1, upper_bound]
+    # narrow down range of first match until one value left
     lower_bound = upper_bound // 2
     while lower_bound + 1 < upper_bound:
         middle = (upper_bound + lower_bound) // 2
         if condition(middle):
             upper_bound = middle
         else:
             lower_bound = middle
```

### Comparing `superpathlib-1.0.1/superpathlib.egg-info/PKG-INFO` & `superpathlib-1.0.2/superpathlib.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: superpathlib
-Version: 1.0.1
-Summary: extended pathlib
-Home-page: https://github.com/quintenroets/superpathlib
-Author: Quinten Roets
-Author-email: quinten.roets@gmail.com
+Version: 1.0.2
+Summary: Extended Pathlib
+Author-email: Quinten Roets <qdr2104@columbia.edu>
 License: MIT
-Requires-Python: >=3.9
+Project-URL: Source Code, https://github.com/quintenroets/superpathlib
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: test
 License-File: LICENSE
 
 # Superpathlib
 Superpathlib offers Path objects with functionality extended from pathlib to maximize your productivity with a minimal amount of code.
 
 ## Usage
 
@@ -22,14 +23,15 @@
 
 ### 1) Use properties to read & write path content in different formats
 * text
 * byte_content
 * lines
 * yaml
 * json
+* numpy
 
 examples: 
 
 ```shell
 path.json = {key: value}
 
 for line in path.lines:
@@ -106,9 +108,12 @@
 This only works if you inherit from plib and not from the builtin pathlib
 
 
 ## Installation
 
 ```shell
 pip install superpathlib
-requires python version >= 3.9
 ```
+
+Install the packages corresponding with the properties you want to use
+* e.g. PyYaml for yaml property
+* Packages listed in requirements.txt
```

### Comparing `superpathlib-1.0.1/tests/test_content.py` & `superpathlib-1.0.2/tests/test_content.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import numpy as np
 import pytest
 from hypothesis import HealthCheck, given, settings, strategies
 
 from plib import Path
 
 
 def dictionary_strategy():
@@ -85,14 +86,22 @@
 @dictionary_content
 @settings(suppress_health_check=(HealthCheck.function_scoped_fixture,), max_examples=10)
 def test_yaml(path, content):
     path.yaml = content
     assert path.yaml == content
 
 
+@given(content=strategies.lists(strategies.floats()))
+@settings(suppress_health_check=(HealthCheck.function_scoped_fixture,), max_examples=10)
+def test_numpy(path, content):
+    numpy_content = np.array(content)
+    path.numpy = numpy_content
+    assert np.array_equal(path.numpy, numpy_content, equal_nan=True)
+
+
 @settings(
     max_examples=2,
     deadline=2000,
     suppress_health_check=(HealthCheck.function_scoped_fixture,),
 )
 @given(byte_content=strategies.binary())
 def test_encrypted_bytes(encryption_path, byte_content):
```

### Comparing `superpathlib-1.0.1/tests/test_functionality.py` & `superpathlib-1.0.2/tests/test_functionality.py`

 * *Files identical despite different names*

### Comparing `superpathlib-1.0.1/tests/test_metadata.py` & `superpathlib-1.0.2/tests/test_metadata.py`

 * *Files identical despite different names*

