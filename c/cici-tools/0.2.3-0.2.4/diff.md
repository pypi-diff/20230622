# Comparing `tmp/cici-tools-0.2.3.tar.gz` & `tmp/cici-tools-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cici-tools-0.2.3.tar", last modified: Thu Jun 22 06:18:09 2023, max compression
+gzip compressed data, was "cici-tools-0.2.4.tar", last modified: Thu Jun 22 06:23:12 2023, max compression
```

## Comparing `cici-tools-0.2.3.tar` & `cici-tools-0.2.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 06:18:09.149300 cici-tools-0.2.3/
--rw-rw-rw-   0 root         (0) root         (0)     1069 2023-06-22 06:18:06.000000 cici-tools-0.2.3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-06-22 06:18:06.000000 cici-tools-0.2.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2689 2023-06-22 06:18:09.150300 cici-tools-0.2.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1856 2023-06-22 06:18:06.000000 cici-tools-0.2.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 06:18:09.146300 cici-tools-0.2.3/cici/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 06:18:06.000000 cici-tools-0.2.3/cici/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-06-22 06:18:06.000000 cici-tools-0.2.3/cici/__main__.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-22 06:18:07.000000 cici-tools-0.2.3/cici/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 06:18:09.146300 cici-tools-0.2.3/cici/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 06:18:06.000000 cici-tools-0.2.3/cici/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1510 2023-06-22 06:18:06.000000 cici-tools-0.2.3/cici/cli/build.py
--rwxrwxrwx   0 root         (0) root         (0)     3073 2023-06-22 06:18:06.000000 cici-tools-0.2.3/cici/cli/bundle.py
--rw-rw-rw-   0 root         (0) root         (0)      881 2023-06-22 06:18:06.000000 cici-tools-0.2.3/cici/cli/fmt.py
--rw-rw-rw-   0 root         (0) root         (0)     3140 2023-06-22 06:18:06.000000 cici-tools-0.2.3/cici/cli/update.py
--rw-rw-rw-   0 root         (0) root         (0)      588 2023-06-22 06:18:06.000000 cici-tools-0.2.3/cici/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      438 2023-06-22 06:18:06.000000 cici-tools-0.2.3/cici/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 06:18:09.146300 cici-tools-0.2.3/cici/providers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 06:18:06.000000 cici-tools-0.2.3/cici/providers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 06:18:09.148300 cici-tools-0.2.3/cici/providers/gitlab/
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-06-22 06:18:06.000000 cici-tools-0.2.3/cici/providers/gitlab/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1580 2023-06-22 06:18:06.000000 cici-tools-0.2.3/cici/providers/gitlab/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     5641 2023-06-22 06:18:06.000000 cici-tools-0.2.3/cici/providers/gitlab/converter.py
--rw-rw-rw-   0 root         (0) root         (0)     6415 2023-06-22 06:18:06.000000 cici-tools-0.2.3/cici/providers/gitlab/models.py
--rw-rw-rw-   0 root         (0) root         (0)     3091 2023-06-22 06:18:06.000000 cici-tools-0.2.3/cici/providers/gitlab/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)      563 2023-06-22 06:18:06.000000 cici-tools-0.2.3/cici/providers/gitlab/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 06:18:09.148300 cici-tools-0.2.3/cici/schema/
--rw-rw-rw-   0 root         (0) root         (0)     2001 2023-06-22 06:18:06.000000 cici-tools-0.2.3/cici/schema/LICENSE.gitlab
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 06:18:06.000000 cici-tools-0.2.3/cici/schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    70638 2023-06-22 06:18:06.000000 cici-tools-0.2.3/cici/schema/gitlab-ci.json
--rw-rw-rw-   0 root         (0) root         (0)     1755 2023-06-22 06:18:06.000000 cici-tools-0.2.3/cici/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 06:18:09.149300 cici-tools-0.2.3/cici_tools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2689 2023-06-22 06:18:09.000000 cici-tools-0.2.3/cici_tools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      752 2023-06-22 06:18:09.000000 cici-tools-0.2.3/cici_tools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 06:18:09.000000 cici-tools-0.2.3/cici_tools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-06-22 06:18:09.000000 cici-tools-0.2.3/cici_tools.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-06-22 06:18:09.000000 cici-tools-0.2.3/cici_tools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-22 06:18:09.000000 cici-tools-0.2.3/cici_tools.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-06-22 06:18:09.150300 cici-tools-0.2.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1360 2023-06-22 06:18:07.000000 cici-tools-0.2.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 06:23:12.765753 cici-tools-0.2.4/
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-06-22 06:23:10.000000 cici-tools-0.2.4/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-06-22 06:23:10.000000 cici-tools-0.2.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2689 2023-06-22 06:23:12.765753 cici-tools-0.2.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1856 2023-06-22 06:23:10.000000 cici-tools-0.2.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 06:23:12.760753 cici-tools-0.2.4/cici/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 06:23:10.000000 cici-tools-0.2.4/cici/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-06-22 06:23:10.000000 cici-tools-0.2.4/cici/__main__.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-22 06:23:10.000000 cici-tools-0.2.4/cici/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 06:23:12.761753 cici-tools-0.2.4/cici/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 06:23:10.000000 cici-tools-0.2.4/cici/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1510 2023-06-22 06:23:10.000000 cici-tools-0.2.4/cici/cli/build.py
+-rwxrwxrwx   0 root         (0) root         (0)     3073 2023-06-22 06:23:10.000000 cici-tools-0.2.4/cici/cli/bundle.py
+-rw-rw-rw-   0 root         (0) root         (0)      881 2023-06-22 06:23:10.000000 cici-tools-0.2.4/cici/cli/fmt.py
+-rw-rw-rw-   0 root         (0) root         (0)     3140 2023-06-22 06:23:10.000000 cici-tools-0.2.4/cici/cli/update.py
+-rw-rw-rw-   0 root         (0) root         (0)      588 2023-06-22 06:23:10.000000 cici-tools-0.2.4/cici/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      438 2023-06-22 06:23:10.000000 cici-tools-0.2.4/cici/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 06:23:12.762753 cici-tools-0.2.4/cici/providers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 06:23:10.000000 cici-tools-0.2.4/cici/providers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 06:23:12.763753 cici-tools-0.2.4/cici/providers/gitlab/
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-06-22 06:23:10.000000 cici-tools-0.2.4/cici/providers/gitlab/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1580 2023-06-22 06:23:10.000000 cici-tools-0.2.4/cici/providers/gitlab/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     5760 2023-06-22 06:23:10.000000 cici-tools-0.2.4/cici/providers/gitlab/converter.py
+-rw-rw-rw-   0 root         (0) root         (0)     6415 2023-06-22 06:23:10.000000 cici-tools-0.2.4/cici/providers/gitlab/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     3091 2023-06-22 06:23:10.000000 cici-tools-0.2.4/cici/providers/gitlab/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)      563 2023-06-22 06:23:10.000000 cici-tools-0.2.4/cici/providers/gitlab/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 06:23:12.763753 cici-tools-0.2.4/cici/schema/
+-rw-rw-rw-   0 root         (0) root         (0)     2001 2023-06-22 06:23:10.000000 cici-tools-0.2.4/cici/schema/LICENSE.gitlab
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 06:23:10.000000 cici-tools-0.2.4/cici/schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    70638 2023-06-22 06:23:10.000000 cici-tools-0.2.4/cici/schema/gitlab-ci.json
+-rw-rw-rw-   0 root         (0) root         (0)     1829 2023-06-22 06:23:10.000000 cici-tools-0.2.4/cici/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 06:23:12.765753 cici-tools-0.2.4/cici_tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2689 2023-06-22 06:23:12.000000 cici-tools-0.2.4/cici_tools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      752 2023-06-22 06:23:12.000000 cici-tools-0.2.4/cici_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 06:23:12.000000 cici-tools-0.2.4/cici_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-06-22 06:23:12.000000 cici-tools-0.2.4/cici_tools.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-06-22 06:23:12.000000 cici-tools-0.2.4/cici_tools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-22 06:23:12.000000 cici-tools-0.2.4/cici_tools.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-06-22 06:23:12.765753 cici-tools-0.2.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1360 2023-06-22 06:23:10.000000 cici-tools-0.2.4/setup.py
```

### Comparing `cici-tools-0.2.3/LICENSE` & `cici-tools-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.3/PKG-INFO` & `cici-tools-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cici-tools
-Version: 0.2.3
+Version: 0.2.4
 Summary: Power tools for CI/CD.
 Home-page: https://gitlab.com/brettops/tools/cici
 Author: Brett Weir
 Author-email: brett@brettops.io
 License: MIT
 Keywords: ci pipeline python
 Platform: UNKNOWN
```

### Comparing `cici-tools-0.2.3/README.md` & `cici-tools-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.3/cici/cli/build.py` & `cici-tools-0.2.4/cici/cli/build.py`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.3/cici/cli/bundle.py` & `cici-tools-0.2.4/cici/cli/bundle.py`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.3/cici/cli/fmt.py` & `cici-tools-0.2.4/cici/cli/fmt.py`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.3/cici/cli/update.py` & `cici-tools-0.2.4/cici/cli/update.py`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.3/cici/constants.py` & `cici-tools-0.2.4/cici/constants.py`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.3/cici/providers/gitlab/constants.py` & `cici-tools-0.2.4/cici/providers/gitlab/constants.py`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.3/cici/providers/gitlab/converter.py` & `cici-tools-0.2.4/cici/providers/gitlab/converter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import functools
 from typing import Union
 
 import cattrs
 from cattrs.gen import make_dict_structure_fn, make_dict_unstructure_fn, override
 
 from ...utils import (
+    make_multiline_string,
     make_quoted_dict,
     make_quoted_list,
     make_quoted_list_or_string,
     make_quoted_string,
     make_scalar_list,
 )
 from . import models
@@ -33,14 +34,18 @@
     return make_quoted_list(object)
 
 
 def quoted_string_struct_hook(object, __):
     return make_quoted_string(object)
 
 
+def multiline_string_struct_hook(object, __):
+    return make_multiline_string(object)
+
+
 def quoted_list_or_string_struct_hook(object, __):
     return make_quoted_list_or_string(object)
 
 
 def quoted_dict_struct_hook(object, __):
     return make_quoted_dict(object)
 
@@ -160,15 +165,15 @@
 )
 
 CONVERTER.register_structure_hook(
     models.Variable,
     make_dict_struct(
         models.Variable,
         CONVERTER,
-        description=override(struct_hook=quoted_string_struct_hook),
+        description=override(struct_hook=multiline_string_struct_hook),
         value=override(struct_hook=quoted_string_struct_hook),
         options=override(struct_hook=quoted_list_struct_hook),
     ),
 )
 
 
 def unstructure_script(cls):
```

### Comparing `cici-tools-0.2.3/cici/providers/gitlab/models.py` & `cici-tools-0.2.4/cici/providers/gitlab/models.py`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.3/cici/providers/gitlab/serializers.py` & `cici-tools-0.2.4/cici/providers/gitlab/serializers.py`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.3/cici/providers/gitlab/utils.py` & `cici-tools-0.2.4/cici/providers/gitlab/utils.py`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.3/cici/schema/LICENSE.gitlab` & `cici-tools-0.2.4/cici/schema/LICENSE.gitlab`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.3/cici/schema/gitlab-ci.json` & `cici-tools-0.2.4/cici/schema/gitlab-ci.json`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.3/cici/utils.py` & `cici-tools-0.2.4/cici/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -24,14 +24,18 @@
         elif key in new:
             final[key] = new[key]
         else:
             raise NotImplementedError("This should not possible")
     return final
 
 
+def make_multiline_string(line):
+    return PreservedScalarString(line)
+
+
 def make_scalar_string(line, quote=False):
     if "\n" in line.strip():
         return PreservedScalarString(line)
     elif len(line) >= 80:
         return FoldedScalarString(line)
     elif quote:
         return DoubleQuotedScalarString(line)
```

### Comparing `cici-tools-0.2.3/cici_tools.egg-info/PKG-INFO` & `cici-tools-0.2.4/cici_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cici-tools
-Version: 0.2.3
+Version: 0.2.4
 Summary: Power tools for CI/CD.
 Home-page: https://gitlab.com/brettops/tools/cici
 Author: Brett Weir
 Author-email: brett@brettops.io
 License: MIT
 Keywords: ci pipeline python
 Platform: UNKNOWN
```

### Comparing `cici-tools-0.2.3/cici_tools.egg-info/SOURCES.txt` & `cici-tools-0.2.4/cici_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.3/setup.py` & `cici-tools-0.2.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_packages, setup
 
 # injected version
-__version__ = "0.2.3"
+__version__ = "0.2.4"
 
 # markdown readme
 long_description = open("README.md").read()
 
 # read requirements from requirements.in
 install_requires = open("requirements.in").read().splitlines()
```

