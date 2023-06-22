# Comparing `tmp/cici-tools-0.2.2.tar.gz` & `tmp/cici-tools-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cici-tools-0.2.2.tar", last modified: Tue Jun 20 10:42:41 2023, max compression
+gzip compressed data, was "cici-tools-0.2.3.tar", last modified: Thu Jun 22 06:18:09 2023, max compression
```

## Comparing `cici-tools-0.2.2.tar` & `cici-tools-0.2.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 10:42:41.809664 cici-tools-0.2.2/
--rw-rw-rw-   0 root         (0) root         (0)     1069 2023-06-20 10:42:39.000000 cici-tools-0.2.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-06-20 10:42:39.000000 cici-tools-0.2.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2047 2023-06-20 10:42:41.809664 cici-tools-0.2.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1214 2023-06-20 10:42:39.000000 cici-tools-0.2.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 10:42:41.805664 cici-tools-0.2.2/cici/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 10:42:39.000000 cici-tools-0.2.2/cici/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-06-20 10:42:39.000000 cici-tools-0.2.2/cici/__main__.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-20 10:42:39.000000 cici-tools-0.2.2/cici/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 10:42:41.806665 cici-tools-0.2.2/cici/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 10:42:39.000000 cici-tools-0.2.2/cici/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1510 2023-06-20 10:42:39.000000 cici-tools-0.2.2/cici/cli/build.py
--rwxrwxrwx   0 root         (0) root         (0)     3073 2023-06-20 10:42:39.000000 cici-tools-0.2.2/cici/cli/bundle.py
--rw-rw-rw-   0 root         (0) root         (0)      881 2023-06-20 10:42:39.000000 cici-tools-0.2.2/cici/cli/fmt.py
--rw-rw-rw-   0 root         (0) root         (0)     3140 2023-06-20 10:42:39.000000 cici-tools-0.2.2/cici/cli/update.py
--rw-rw-rw-   0 root         (0) root         (0)      588 2023-06-20 10:42:39.000000 cici-tools-0.2.2/cici/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      438 2023-06-20 10:42:39.000000 cici-tools-0.2.2/cici/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 10:42:41.806665 cici-tools-0.2.2/cici/providers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 10:42:39.000000 cici-tools-0.2.2/cici/providers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 10:42:41.807664 cici-tools-0.2.2/cici/providers/gitlab/
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-06-20 10:42:39.000000 cici-tools-0.2.2/cici/providers/gitlab/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1580 2023-06-20 10:42:39.000000 cici-tools-0.2.2/cici/providers/gitlab/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     5002 2023-06-20 10:42:39.000000 cici-tools-0.2.2/cici/providers/gitlab/converter.py
--rw-rw-rw-   0 root         (0) root         (0)     6415 2023-06-20 10:42:39.000000 cici-tools-0.2.2/cici/providers/gitlab/models.py
--rw-rw-rw-   0 root         (0) root         (0)     2973 2023-06-20 10:42:39.000000 cici-tools-0.2.2/cici/providers/gitlab/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)      563 2023-06-20 10:42:39.000000 cici-tools-0.2.2/cici/providers/gitlab/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 10:42:41.807664 cici-tools-0.2.2/cici/schema/
--rw-rw-rw-   0 root         (0) root         (0)     2001 2023-06-20 10:42:39.000000 cici-tools-0.2.2/cici/schema/LICENSE.gitlab
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 10:42:39.000000 cici-tools-0.2.2/cici/schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    70638 2023-06-20 10:42:39.000000 cici-tools-0.2.2/cici/schema/gitlab-ci.json
--rw-rw-rw-   0 root         (0) root         (0)     1755 2023-06-20 10:42:39.000000 cici-tools-0.2.2/cici/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 10:42:41.809664 cici-tools-0.2.2/cici_tools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2047 2023-06-20 10:42:41.000000 cici-tools-0.2.2/cici_tools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      752 2023-06-20 10:42:41.000000 cici-tools-0.2.2/cici_tools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 10:42:41.000000 cici-tools-0.2.2/cici_tools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-06-20 10:42:41.000000 cici-tools-0.2.2/cici_tools.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-06-20 10:42:41.000000 cici-tools-0.2.2/cici_tools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-20 10:42:41.000000 cici-tools-0.2.2/cici_tools.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-06-20 10:42:41.809664 cici-tools-0.2.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1360 2023-06-20 10:42:39.000000 cici-tools-0.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 06:18:09.149300 cici-tools-0.2.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-06-22 06:18:06.000000 cici-tools-0.2.3/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-06-22 06:18:06.000000 cici-tools-0.2.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2689 2023-06-22 06:18:09.150300 cici-tools-0.2.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1856 2023-06-22 06:18:06.000000 cici-tools-0.2.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 06:18:09.146300 cici-tools-0.2.3/cici/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 06:18:06.000000 cici-tools-0.2.3/cici/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-06-22 06:18:06.000000 cici-tools-0.2.3/cici/__main__.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-22 06:18:07.000000 cici-tools-0.2.3/cici/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 06:18:09.146300 cici-tools-0.2.3/cici/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 06:18:06.000000 cici-tools-0.2.3/cici/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1510 2023-06-22 06:18:06.000000 cici-tools-0.2.3/cici/cli/build.py
+-rwxrwxrwx   0 root         (0) root         (0)     3073 2023-06-22 06:18:06.000000 cici-tools-0.2.3/cici/cli/bundle.py
+-rw-rw-rw-   0 root         (0) root         (0)      881 2023-06-22 06:18:06.000000 cici-tools-0.2.3/cici/cli/fmt.py
+-rw-rw-rw-   0 root         (0) root         (0)     3140 2023-06-22 06:18:06.000000 cici-tools-0.2.3/cici/cli/update.py
+-rw-rw-rw-   0 root         (0) root         (0)      588 2023-06-22 06:18:06.000000 cici-tools-0.2.3/cici/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      438 2023-06-22 06:18:06.000000 cici-tools-0.2.3/cici/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 06:18:09.146300 cici-tools-0.2.3/cici/providers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 06:18:06.000000 cici-tools-0.2.3/cici/providers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 06:18:09.148300 cici-tools-0.2.3/cici/providers/gitlab/
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-06-22 06:18:06.000000 cici-tools-0.2.3/cici/providers/gitlab/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1580 2023-06-22 06:18:06.000000 cici-tools-0.2.3/cici/providers/gitlab/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     5641 2023-06-22 06:18:06.000000 cici-tools-0.2.3/cici/providers/gitlab/converter.py
+-rw-rw-rw-   0 root         (0) root         (0)     6415 2023-06-22 06:18:06.000000 cici-tools-0.2.3/cici/providers/gitlab/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     3091 2023-06-22 06:18:06.000000 cici-tools-0.2.3/cici/providers/gitlab/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)      563 2023-06-22 06:18:06.000000 cici-tools-0.2.3/cici/providers/gitlab/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 06:18:09.148300 cici-tools-0.2.3/cici/schema/
+-rw-rw-rw-   0 root         (0) root         (0)     2001 2023-06-22 06:18:06.000000 cici-tools-0.2.3/cici/schema/LICENSE.gitlab
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 06:18:06.000000 cici-tools-0.2.3/cici/schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    70638 2023-06-22 06:18:06.000000 cici-tools-0.2.3/cici/schema/gitlab-ci.json
+-rw-rw-rw-   0 root         (0) root         (0)     1755 2023-06-22 06:18:06.000000 cici-tools-0.2.3/cici/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 06:18:09.149300 cici-tools-0.2.3/cici_tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2689 2023-06-22 06:18:09.000000 cici-tools-0.2.3/cici_tools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      752 2023-06-22 06:18:09.000000 cici-tools-0.2.3/cici_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 06:18:09.000000 cici-tools-0.2.3/cici_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-06-22 06:18:09.000000 cici-tools-0.2.3/cici_tools.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-06-22 06:18:09.000000 cici-tools-0.2.3/cici_tools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-22 06:18:09.000000 cici-tools-0.2.3/cici_tools.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-06-22 06:18:09.150300 cici-tools-0.2.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1360 2023-06-22 06:18:07.000000 cici-tools-0.2.3/setup.py
```

### Comparing `cici-tools-0.2.2/LICENSE` & `cici-tools-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.2/PKG-INFO` & `cici-tools-0.2.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cici-tools
-Version: 0.2.2
+Version: 0.2.3
 Summary: Power tools for CI/CD.
 Home-page: https://gitlab.com/brettops/tools/cici
 Author: Brett Weir
 Author-email: brett@brettops.io
 License: MIT
 Keywords: ci pipeline python
 Platform: UNKNOWN
@@ -40,24 +40,63 @@
 
 ## Usage
 
 ### `bundle`
 
 Flatten `extends` keywords to make zero-dependency GitLab CI/CD files.
 
+```bash
+cici bundle
+```
+
+```console
+$ cici bundle
+pipeline name: python
+bundle names: ['black', 'isort', 'mypy', 'pyroma', 'pytest', 'setuptools', 'twine', 'vulture']
+created black.yml
+created isort.yml
+created mypy.yml
+created pyroma.yml
+created pytest.yml
+created setuptools.yml
+created twine.yml
+created vulture.yml
+```
+
+```yaml
+include:
+  - project: brettops/pipelines/python
+    ref: ""
+    file:
+      - black.yml
+      - isort.yml
+      - vulture.yml
+```
+
 ### `fmt`
 
 Normalize the style of your GitLab CI/CD files:
 
 ```bash
 cici fmt
 ```
 
+```console
+$ cici fmt
+.gitlab-ci.yml formatted
+```
+
 ### `update`
 
 Update to the latest GitLab CI/CD `include` versions available.
 
-```
+```bash
 cici update
 ```
 
+```console
+$ cici update
+brettops/pipelines/prettier has no releases
+brettops/pipelines/python is the latest at 0.5.0
+```
+
```

### Comparing `cici-tools-0.2.2/README.md` & `cici-tools-0.2.3/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -16,22 +16,61 @@
 
 ## Usage
 
 ### `bundle`
 
 Flatten `extends` keywords to make zero-dependency GitLab CI/CD files.
 
+```bash
+cici bundle
+```
+
+```console
+$ cici bundle
+pipeline name: python
+bundle names: ['black', 'isort', 'mypy', 'pyroma', 'pytest', 'setuptools', 'twine', 'vulture']
+created black.yml
+created isort.yml
+created mypy.yml
+created pyroma.yml
+created pytest.yml
+created setuptools.yml
+created twine.yml
+created vulture.yml
+```
+
+```yaml
+include:
+  - project: brettops/pipelines/python
+    ref: ""
+    file:
+      - black.yml
+      - isort.yml
+      - vulture.yml
+```
+
 ### `fmt`
 
 Normalize the style of your GitLab CI/CD files:
 
 ```bash
 cici fmt
 ```
 
+```console
+$ cici fmt
+.gitlab-ci.yml formatted
+```
+
 ### `update`
 
 Update to the latest GitLab CI/CD `include` versions available.
 
-```
+```bash
 cici update
 ```
+
+```console
+$ cici update
+brettops/pipelines/prettier has no releases
+brettops/pipelines/python is the latest at 0.5.0
+```
```

### Comparing `cici-tools-0.2.2/cici/cli/build.py` & `cici-tools-0.2.3/cici/cli/build.py`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.2/cici/cli/bundle.py` & `cici-tools-0.2.3/cici/cli/bundle.py`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.2/cici/cli/fmt.py` & `cici-tools-0.2.3/cici/cli/fmt.py`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.2/cici/cli/update.py` & `cici-tools-0.2.3/cici/cli/update.py`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.2/cici/constants.py` & `cici-tools-0.2.3/cici/constants.py`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.2/cici/providers/gitlab/constants.py` & `cici-tools-0.2.3/cici/providers/gitlab/constants.py`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.2/cici/providers/gitlab/converter.py` & `cici-tools-0.2.3/cici/providers/gitlab/converter.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Union
 
 import cattrs
 from cattrs.gen import make_dict_structure_fn, make_dict_unstructure_fn, override
 
 from ...utils import (
     make_quoted_dict,
+    make_quoted_list,
     make_quoted_list_or_string,
     make_quoted_string,
     make_scalar_list,
 )
 from . import models
 
 CONVERTER = cattrs.Converter(omit_if_default=True, forbid_extra_keys=True)
@@ -24,14 +25,18 @@
 make_dict_unstruct = functools.partial(
     make_dict_unstructure_fn,
     _cattrs_forbid_extra_keys=True,
     _cattrs_omit_if_default=True,
 )
 
 
+def quoted_list_struct_hook(object, __):
+    return make_quoted_list(object)
+
+
 def quoted_string_struct_hook(object, __):
     return make_quoted_string(object)
 
 
 def quoted_list_or_string_struct_hook(object, __):
     return make_quoted_list_or_string(object)
 
@@ -80,15 +85,21 @@
 def structure_service(object, __):
     if isinstance(object, str):
         return make_quoted_string(CONVERTER.structure(object, str))
     return CONVERTER.structure(object, models.Service)
 
 
 def structure_variables(object, __):
-    return make_quoted_dict(object)
+    variables = {}
+    for key, value in object.items():
+        if isinstance(value, str):
+            variables[key] = make_quoted_string(value)
+        else:
+            variables[key] = CONVERTER.structure(value, models.Variable)
+    return variables
 
 
 CONVERTER.register_structure_hook(
     Union[
         str,
         list[
             Union[
@@ -144,14 +155,25 @@
         CONVERTER,
         name=override(struct_hook=quoted_string_struct_hook),
         command=override(struct_hook=quoted_list_or_string_struct_hook),
         entrypoint=override(struct_hook=quoted_list_or_string_struct_hook),
     ),
 )
 
+CONVERTER.register_structure_hook(
+    models.Variable,
+    make_dict_struct(
+        models.Variable,
+        CONVERTER,
+        description=override(struct_hook=quoted_string_struct_hook),
+        value=override(struct_hook=quoted_string_struct_hook),
+        options=override(struct_hook=quoted_list_struct_hook),
+    ),
+)
+
 
 def unstructure_script(cls):
     object = CONVERTER.unstructure(cls, str if isinstance(cls, str) else list[str])
     if isinstance(object, str):
         return object  # make_quoted_scalar_string(object)
     return make_scalar_list(object)
 
@@ -185,19 +207,19 @@
 
 
 CONVERTER.register_structure_hook(
     models.Job,
     make_dict_struct(
         models.Job,
         CONVERTER,
-        variables=override(struct_hook=quoted_dict_struct_hook),
+        variables=override(struct_hook=structure_variables),
     ),
 )
 
 CONVERTER.register_structure_hook(
     models.File,
     make_dict_struct(
         models.File,
         CONVERTER,
-        variables=override(struct_hook=quoted_dict_struct_hook),
+        variables=override(struct_hook=structure_variables),
     ),
 )
```

### Comparing `cici-tools-0.2.2/cici/providers/gitlab/models.py` & `cici-tools-0.2.3/cici/providers/gitlab/models.py`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.2/cici/providers/gitlab/serializers.py` & `cici-tools-0.2.3/cici/providers/gitlab/serializers.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,18 +48,21 @@
         if job_name.startswith("."):
             try:
                 CONVERTER.structure(data[job_name], models.Job)
                 jobs[job_name] = data[job_name]
             except (
                 cattrs.errors.ClassValidationError,
                 cattrs.errors.ForbiddenExtraKeysError,
-                AttributeError,
             ):
-                # monkey patch for YAML anchors in GitLab CI
                 logging.warning(f"job {job_name} skipped")
+            except (AttributeError,) as excinfo:
+                if "CommentedSeq" in str(excinfo):
+                    logging.warning(f"job {job_name} skipped")
+                else:
+                    raise
                 # extras[job_name] = data[job_name]
         else:
             jobs[job_name] = data[job_name]
 
         del data[job_name]
     data["jobs"] = jobs
     data["extras"] = extras
```

### Comparing `cici-tools-0.2.2/cici/providers/gitlab/utils.py` & `cici-tools-0.2.3/cici/providers/gitlab/utils.py`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.2/cici/schema/LICENSE.gitlab` & `cici-tools-0.2.3/cici/schema/LICENSE.gitlab`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.2/cici/schema/gitlab-ci.json` & `cici-tools-0.2.3/cici/schema/gitlab-ci.json`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.2/cici/utils.py` & `cici-tools-0.2.3/cici/utils.py`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.2/cici_tools.egg-info/PKG-INFO` & `cici-tools-0.2.3/cici_tools.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cici-tools
-Version: 0.2.2
+Version: 0.2.3
 Summary: Power tools for CI/CD.
 Home-page: https://gitlab.com/brettops/tools/cici
 Author: Brett Weir
 Author-email: brett@brettops.io
 License: MIT
 Keywords: ci pipeline python
 Platform: UNKNOWN
@@ -40,24 +40,63 @@
 
 ## Usage
 
 ### `bundle`
 
 Flatten `extends` keywords to make zero-dependency GitLab CI/CD files.
 
+```bash
+cici bundle
+```
+
+```console
+$ cici bundle
+pipeline name: python
+bundle names: ['black', 'isort', 'mypy', 'pyroma', 'pytest', 'setuptools', 'twine', 'vulture']
+created black.yml
+created isort.yml
+created mypy.yml
+created pyroma.yml
+created pytest.yml
+created setuptools.yml
+created twine.yml
+created vulture.yml
+```
+
+```yaml
+include:
+  - project: brettops/pipelines/python
+    ref: ""
+    file:
+      - black.yml
+      - isort.yml
+      - vulture.yml
+```
+
 ### `fmt`
 
 Normalize the style of your GitLab CI/CD files:
 
 ```bash
 cici fmt
 ```
 
+```console
+$ cici fmt
+.gitlab-ci.yml formatted
+```
+
 ### `update`
 
 Update to the latest GitLab CI/CD `include` versions available.
 
-```
+```bash
 cici update
 ```
 
+```console
+$ cici update
+brettops/pipelines/prettier has no releases
+brettops/pipelines/python is the latest at 0.5.0
+```
+
```

### Comparing `cici-tools-0.2.2/cici_tools.egg-info/SOURCES.txt` & `cici-tools-0.2.3/cici_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.2/setup.py` & `cici-tools-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_packages, setup
 
 # injected version
-__version__ = "0.2.2"
+__version__ = "0.2.3"
 
 # markdown readme
 long_description = open("README.md").read()
 
 # read requirements from requirements.in
 install_requires = open("requirements.in").read().splitlines()
```

