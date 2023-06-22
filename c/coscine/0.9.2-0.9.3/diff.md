# Comparing `tmp/coscine-0.9.2.tar.gz` & `tmp/coscine-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/coscine-0.9.2.tar", last modified: Tue Apr 11 13:46:22 2023, max compression
+gzip compressed data, was "dist/coscine-0.9.3.tar", last modified: Thu Jun 22 14:08:05 2023, max compression
```

## Comparing `coscine-0.9.2.tar` & `coscine-0.9.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:46:22.000000 coscine-0.9.2/
--rw-rw-rw-   0 root         (0) root         (0)     1084 2023-04-11 13:11:08.000000 coscine-0.9.2/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     7001 2023-04-11 13:46:22.000000 coscine-0.9.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5471 2023-04-11 13:11:08.000000 coscine-0.9.2/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 13:46:22.000000 coscine-0.9.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3905 2023-04-11 13:11:08.000000 coscine-0.9.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:46:22.000000 coscine-0.9.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:46:22.000000 coscine-0.9.2/src/coscine/
--rw-rw-rw-   0 root         (0) root         (0)     2949 2023-04-11 13:46:13.000000 coscine-0.9.2/src/coscine/__about__.py
--rw-rw-rw-   0 root         (0) root         (0)     2231 2023-04-11 13:11:08.000000 coscine-0.9.2/src/coscine/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6267 2023-04-11 13:11:08.000000 coscine-0.9.2/src/coscine/cache.py
--rw-rw-rw-   0 root         (0) root         (0)    24288 2023-04-11 13:11:08.000000 coscine-0.9.2/src/coscine/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:46:22.000000 coscine-0.9.2/src/coscine/data/
--rw-rw-rw-   0 root         (0) root         (0)     1991 2023-04-11 13:11:08.000000 coscine-0.9.2/src/coscine/data/project.json
--rw-rw-rw-   0 root         (0) root         (0)     2029 2023-04-11 13:11:08.000000 coscine-0.9.2/src/coscine/data/resource.json
--rw-rw-rw-   0 root         (0) root         (0)     2276 2023-04-11 13:11:08.000000 coscine-0.9.2/src/coscine/defaults.py
--rw-rw-rw-   0 root         (0) root         (0)    28275 2023-04-11 13:11:08.000000 coscine-0.9.2/src/coscine/form.py
--rw-rw-rw-   0 root         (0) root         (0)     6910 2023-04-11 13:11:08.000000 coscine-0.9.2/src/coscine/graph.py
--rw-rw-rw-   0 root         (0) root         (0)    19225 2023-04-11 13:18:30.000000 coscine-0.9.2/src/coscine/object.py
--rw-rw-rw-   0 root         (0) root         (0)    21761 2023-04-11 13:11:08.000000 coscine-0.9.2/src/coscine/project.py
--rw-rw-rw-   0 root         (0) root         (0)    26362 2023-04-11 13:46:13.000000 coscine-0.9.2/src/coscine/resource.py
--rw-rw-rw-   0 root         (0) root         (0)     7402 2023-04-11 13:11:08.000000 coscine-0.9.2/src/coscine/s3.py
--rw-rw-rw-   0 root         (0) root         (0)    11884 2023-04-11 13:11:08.000000 coscine-0.9.2/src/coscine/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    14870 2023-04-11 13:11:08.000000 coscine-0.9.2/src/coscine/vocabulary.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:46:22.000000 coscine-0.9.2/src/coscine.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7001 2023-04-11 13:46:22.000000 coscine-0.9.2/src/coscine.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      556 2023-04-11 13:46:22.000000 coscine-0.9.2/src/coscine.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 13:46:22.000000 coscine-0.9.2/src/coscine.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       84 2023-04-11 13:46:22.000000 coscine-0.9.2/src/coscine.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-11 13:46:22.000000 coscine-0.9.2/src/coscine.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:08:05.000000 coscine-0.9.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1084 2023-04-11 13:11:08.000000 coscine-0.9.3/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     7630 2023-06-22 14:08:05.000000 coscine-0.9.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6100 2023-06-22 14:06:09.000000 coscine-0.9.3/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 14:08:05.000000 coscine-0.9.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3905 2023-04-11 13:11:08.000000 coscine-0.9.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:08:05.000000 coscine-0.9.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:08:05.000000 coscine-0.9.3/src/coscine/
+-rw-rw-rw-   0 root         (0) root         (0)     2954 2023-06-22 14:06:09.000000 coscine-0.9.3/src/coscine/__about__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2231 2023-04-11 13:11:08.000000 coscine-0.9.3/src/coscine/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6267 2023-04-11 13:11:08.000000 coscine-0.9.3/src/coscine/cache.py
+-rw-rw-rw-   0 root         (0) root         (0)    24288 2023-04-11 13:11:08.000000 coscine-0.9.3/src/coscine/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:08:05.000000 coscine-0.9.3/src/coscine/data/
+-rw-rw-rw-   0 root         (0) root         (0)     1991 2023-04-11 13:11:08.000000 coscine-0.9.3/src/coscine/data/project.json
+-rw-rw-rw-   0 root         (0) root         (0)     2029 2023-04-11 13:11:08.000000 coscine-0.9.3/src/coscine/data/resource.json
+-rw-rw-rw-   0 root         (0) root         (0)     2276 2023-04-11 13:11:08.000000 coscine-0.9.3/src/coscine/defaults.py
+-rw-rw-rw-   0 root         (0) root         (0)    28275 2023-04-11 13:11:08.000000 coscine-0.9.3/src/coscine/form.py
+-rw-rw-rw-   0 root         (0) root         (0)     6907 2023-06-22 14:06:09.000000 coscine-0.9.3/src/coscine/graph.py
+-rw-rw-rw-   0 root         (0) root         (0)    19265 2023-06-22 14:06:09.000000 coscine-0.9.3/src/coscine/object.py
+-rw-rw-rw-   0 root         (0) root         (0)    21761 2023-04-11 13:11:08.000000 coscine-0.9.3/src/coscine/project.py
+-rw-rw-rw-   0 root         (0) root         (0)    26362 2023-04-11 13:46:13.000000 coscine-0.9.3/src/coscine/resource.py
+-rw-rw-rw-   0 root         (0) root         (0)     7402 2023-04-11 13:11:08.000000 coscine-0.9.3/src/coscine/s3.py
+-rw-rw-rw-   0 root         (0) root         (0)    11884 2023-04-11 13:11:08.000000 coscine-0.9.3/src/coscine/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    14870 2023-04-11 13:11:08.000000 coscine-0.9.3/src/coscine/vocabulary.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:08:05.000000 coscine-0.9.3/src/coscine.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7630 2023-06-22 14:08:05.000000 coscine-0.9.3/src/coscine.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      556 2023-06-22 14:08:05.000000 coscine-0.9.3/src/coscine.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 14:08:05.000000 coscine-0.9.3/src/coscine.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       84 2023-06-22 14:08:05.000000 coscine-0.9.3/src/coscine.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-22 14:08:05.000000 coscine-0.9.3/src/coscine.egg-info/top_level.txt
```

### Comparing `coscine-0.9.2/LICENSE.txt` & `coscine-0.9.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `coscine-0.9.2/PKG-INFO` & `coscine-0.9.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coscine
-Version: 0.9.2
+Version: 0.9.3
 Summary: The Coscine Python SDK provides a pythonic interface to the Coscine REST API.
 Home-page: https://git.rwth-aachen.de/coscine/community-features/coscine-python-sdk/
 Author: RWTH Aachen University
 Author-email: coscine@itc.rwth-aachen.de
 License: MIT License
 Project-URL: Issues, https://git.rwth-aachen.de/coscine/community-features/coscine-python-sdk/-/issues
 Project-URL: Documentation, https://coscine.pages.rwth-aachen.de/community-features/coscine-python-sdk/
@@ -24,14 +24,23 @@
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
+## DISCLAIMER
+> Issues have been permanently disabled due to increasing amounts of spam.
+> If you have any questions or would like to report a bug, request a feature or
+> have any other business similar to that, you can send a good old-fashioned E-Mail
+> to the [Coscine Technical Adaption Mailing List](mailto:coscine-technical-adaptation@itc.rwth-aachen.de)
+> or contact me personally via my personal Mail (Click on my GitLab profile and copy the full name
+> in the browsers address bar including the dot between first and last name.
+> Then append (at) rwth-aachen.de). In either cases I'll get a Mail and am able to respond.
+
 # Coscine Python SDK
 ![Coscine] ![Python]  
 [Coscine](https://coscine.de/), short for **Co**llaborative **Sc**ientific
 **In**tegration **E**nvironment, is a platform for Research Data Management.  
 
 [Coscine]: https://git.rwth-aachen.de/coscine/community-features/coscine-python-sdk/-/raw/master/data/coscine_logo_rgb.png
 [Python]: https://git.rwth-aachen.de/coscine/community-features/coscine-python-sdk/-/raw/master/data/python-powered-w-200x80.png
```

### Comparing `coscine-0.9.2/README.md` & `coscine-0.9.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+## DISCLAIMER
+> Issues have been permanently disabled due to increasing amounts of spam.
+> If you have any questions or would like to report a bug, request a feature or
+> have any other business similar to that, you can send a good old-fashioned E-Mail
+> to the [Coscine Technical Adaption Mailing List](mailto:coscine-technical-adaptation@itc.rwth-aachen.de)
+> or contact me personally via my personal Mail (Click on my GitLab profile and copy the full name
+> in the browsers address bar including the dot between first and last name.
+> Then append (at) rwth-aachen.de). In either cases I'll get a Mail and am able to respond.
+
 # Coscine Python SDK
 ![Coscine] ![Python]  
 [Coscine](https://coscine.de/), short for **Co**llaborative **Sc**ientific
 **In**tegration **E**nvironment, is a platform for Research Data Management.  
 
 [Coscine]: ./data/coscine_logo_rgb.png
 [Python]: ./data/python-powered-w-200x80.png
```

### Comparing `coscine-0.9.2/setup.py` & `coscine-0.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `coscine-0.9.2/src/coscine/__about__.py` & `coscine-0.9.3/src/coscine/__about__.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 # Module globals / Constants
 ###############################################################################
 
 # Package title/name as it would appear in PyPi
 __title__ = "coscine"
 
 # Current package version
-# Do not set version to 1.0.0 before Coscine end of pilot phase
-__version__ = "0.9.2"
+# Do not set version to 1.0.0 before update to Coscine API version 2
+__version__ = "0.9.3"
 
 # Short package description
 __summary__ = (
     "The Coscine Python SDK provides a pythonic interface to "
     "the Coscine REST API."
 )
```

### Comparing `coscine-0.9.2/src/coscine/__init__.py` & `coscine-0.9.3/src/coscine/__init__.py`

 * *Files identical despite different names*

### Comparing `coscine-0.9.2/src/coscine/cache.py` & `coscine-0.9.3/src/coscine/cache.py`

 * *Files identical despite different names*

### Comparing `coscine-0.9.2/src/coscine/client.py` & `coscine-0.9.3/src/coscine/client.py`

 * *Files identical despite different names*

### Comparing `coscine-0.9.2/src/coscine/data/project.json` & `coscine-0.9.3/src/coscine/data/project.json`

 * *Files identical despite different names*

### Comparing `coscine-0.9.2/src/coscine/data/resource.json` & `coscine-0.9.3/src/coscine/data/resource.json`

 * *Files identical despite different names*

### Comparing `coscine-0.9.2/src/coscine/defaults.py` & `coscine-0.9.3/src/coscine/defaults.py`

 * *Files identical despite different names*

### Comparing `coscine-0.9.2/src/coscine/form.py` & `coscine-0.9.3/src/coscine/form.py`

 * *Files identical despite different names*

### Comparing `coscine-0.9.2/src/coscine/graph.py` & `coscine-0.9.3/src/coscine/graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         Returns a str indicating the target class of the application profile.
         This may for example be "engmeta" in case of an engmeta profile.
         """
 
         query = \
             """
             SELECT ?target WHERE {
-                ?_ sh:targetClass ?target .
+                ?target a sh:NodeShape .
             }
             """
         result = self.query(query)
         return str(result[0][0])  # Force string
 
 ###############################################################################
```

### Comparing `coscine-0.9.2/src/coscine/object.py` & `coscine-0.9.3/src/coscine/object.py`

 * *Files 2% similar despite different names*

```diff
@@ -534,18 +534,18 @@
         if self.is_folder:
             fullpath = posixpath.join(self.path, path)
             return self.resource.object(fullpath)
         raise TypeError(f"FileObject '{self.path}' is not a directory!")
 
 ###############################################################################
 
-    def form(self) -> MetadataForm:
+    def form(self, force_update: bool = False) -> MetadataForm:
         """
         Returns a MetadataForm to interact with the metadata of the FileObject.
         """
 
         graph = self.resource.application_profile()
         form = MetadataForm(self.client, graph)
-        form.parse(self.metadata())
+        form.parse(self.metadata(force_update))
         return form
 
 ###############################################################################
```

### Comparing `coscine-0.9.2/src/coscine/project.py` & `coscine-0.9.3/src/coscine/project.py`

 * *Files identical despite different names*

### Comparing `coscine-0.9.2/src/coscine/resource.py` & `coscine-0.9.3/src/coscine/resource.py`

 * *Files identical despite different names*

### Comparing `coscine-0.9.2/src/coscine/s3.py` & `coscine-0.9.3/src/coscine/s3.py`

 * *Files identical despite different names*

### Comparing `coscine-0.9.2/src/coscine/utils.py` & `coscine-0.9.3/src/coscine/utils.py`

 * *Files identical despite different names*

### Comparing `coscine-0.9.2/src/coscine/vocabulary.py` & `coscine-0.9.3/src/coscine/vocabulary.py`

 * *Files identical despite different names*

### Comparing `coscine-0.9.2/src/coscine.egg-info/PKG-INFO` & `coscine-0.9.3/src/coscine.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coscine
-Version: 0.9.2
+Version: 0.9.3
 Summary: The Coscine Python SDK provides a pythonic interface to the Coscine REST API.
 Home-page: https://git.rwth-aachen.de/coscine/community-features/coscine-python-sdk/
 Author: RWTH Aachen University
 Author-email: coscine@itc.rwth-aachen.de
 License: MIT License
 Project-URL: Issues, https://git.rwth-aachen.de/coscine/community-features/coscine-python-sdk/-/issues
 Project-URL: Documentation, https://coscine.pages.rwth-aachen.de/community-features/coscine-python-sdk/
@@ -24,14 +24,23 @@
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
+## DISCLAIMER
+> Issues have been permanently disabled due to increasing amounts of spam.
+> If you have any questions or would like to report a bug, request a feature or
+> have any other business similar to that, you can send a good old-fashioned E-Mail
+> to the [Coscine Technical Adaption Mailing List](mailto:coscine-technical-adaptation@itc.rwth-aachen.de)
+> or contact me personally via my personal Mail (Click on my GitLab profile and copy the full name
+> in the browsers address bar including the dot between first and last name.
+> Then append (at) rwth-aachen.de). In either cases I'll get a Mail and am able to respond.
+
 # Coscine Python SDK
 ![Coscine] ![Python]  
 [Coscine](https://coscine.de/), short for **Co**llaborative **Sc**ientific
 **In**tegration **E**nvironment, is a platform for Research Data Management.  
 
 [Coscine]: https://git.rwth-aachen.de/coscine/community-features/coscine-python-sdk/-/raw/master/data/coscine_logo_rgb.png
 [Python]: https://git.rwth-aachen.de/coscine/community-features/coscine-python-sdk/-/raw/master/data/python-powered-w-200x80.png
```

### Comparing `coscine-0.9.2/src/coscine.egg-info/SOURCES.txt` & `coscine-0.9.3/src/coscine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

