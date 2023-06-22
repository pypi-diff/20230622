# Comparing `tmp/nn_tilde-1.5.5.tar.gz` & `tmp/nn_tilde-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nn_tilde-1.5.5.tar", last modified: Thu Jun 22 16:41:14 2023, max compression
+gzip compressed data, was "nn_tilde-1.5.6.tar", last modified: Thu Jun 22 16:37:11 2023, max compression
```

## Comparing `nn_tilde-1.5.5.tar` & `nn_tilde-1.5.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:41:14.409433 nn_tilde-1.5.5/
--rw-r--r--   0 runner    (1001) docker     (123)    19916 2023-06-22 16:38:56.000000 nn_tilde-1.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-22 16:38:56.000000 nn_tilde-1.5.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10235 2023-06-22 16:41:14.409433 nn_tilde-1.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10048 2023-06-22 16:38:56.000000 nn_tilde-1.5.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:41:14.405433 nn_tilde-1.5.5/nn_tilde.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10235 2023-06-22 16:41:14.000000 nn_tilde-1.5.5/nn_tilde.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-22 16:41:14.000000 nn_tilde-1.5.5/nn_tilde.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 16:41:14.000000 nn_tilde-1.5.5/nn_tilde.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-22 16:41:14.000000 nn_tilde-1.5.5/nn_tilde.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-22 16:41:14.000000 nn_tilde-1.5.5/nn_tilde.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:41:14.405433 nn_tilde-1.5.5/python_tools/
--rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-06-22 16:38:56.000000 nn_tilde-1.5.5/python_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-22 16:38:56.000000 nn_tilde-1.5.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 16:41:14.409433 nn_tilde-1.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-22 16:38:56.000000 nn_tilde-1.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:37:11.979371 nn_tilde-1.5.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    19916 2023-06-22 16:35:13.000000 nn_tilde-1.5.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-22 16:35:13.000000 nn_tilde-1.5.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10235 2023-06-22 16:37:11.979371 nn_tilde-1.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10048 2023-06-22 16:35:13.000000 nn_tilde-1.5.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:37:11.979371 nn_tilde-1.5.6/nn_tilde.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10235 2023-06-22 16:37:11.000000 nn_tilde-1.5.6/nn_tilde.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-22 16:37:11.000000 nn_tilde-1.5.6/nn_tilde.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 16:37:11.000000 nn_tilde-1.5.6/nn_tilde.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-22 16:37:11.000000 nn_tilde-1.5.6/nn_tilde.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-22 16:37:11.000000 nn_tilde-1.5.6/nn_tilde.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:37:11.979371 nn_tilde-1.5.6/python_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-06-22 16:35:13.000000 nn_tilde-1.5.6/python_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-22 16:35:13.000000 nn_tilde-1.5.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 16:37:11.979371 nn_tilde-1.5.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-22 16:35:13.000000 nn_tilde-1.5.6/setup.py
```

### Comparing `nn_tilde-1.5.5/LICENSE` & `nn_tilde-1.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nn_tilde-1.5.5/PKG-INFO` & `nn_tilde-1.5.6/nn_tilde.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nn_tilde
-Version: 1.5.5
+Name: nn-tilde
+Version: 1.5.6
 Summary: Set of tools to create nn_tilde compatible models.
 Author: Antoine CAILLON
 Author-email: caillon@ircam.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nn_tilde Version: 1.5.5 Summary: Set of tools to
+Metadata-Version: 2.1 Name: nn-tilde Version: 1.5.6 Summary: Set of tools to
 create nn_tilde compatible models. Author: Antoine CAILLON Author-email:
 caillon@ircam.fr Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
 License-File: LICENSE ![banner](https://github.com/acids-ircam/nn_tilde/raw/
 master/assets/banner.png) # Demonstration video [![RAVE x nn~](http://
 img.youtube.com/vi/dMZs04TzxUI/mqdefault.jpg)](https://www.youtube.com/
```

### Comparing `nn_tilde-1.5.5/README.md` & `nn_tilde-1.5.6/README.md`

 * *Files identical despite different names*

### Comparing `nn_tilde-1.5.5/nn_tilde.egg-info/PKG-INFO` & `nn_tilde-1.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nn-tilde
-Version: 1.5.5
+Name: nn_tilde
+Version: 1.5.6
 Summary: Set of tools to create nn_tilde compatible models.
 Author: Antoine CAILLON
 Author-email: caillon@ircam.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nn-tilde Version: 1.5.5 Summary: Set of tools to
+Metadata-Version: 2.1 Name: nn_tilde Version: 1.5.6 Summary: Set of tools to
 create nn_tilde compatible models. Author: Antoine CAILLON Author-email:
 caillon@ircam.fr Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
 License-File: LICENSE ![banner](https://github.com/acids-ircam/nn_tilde/raw/
 master/assets/banner.png) # Demonstration video [![RAVE x nn~](http://
 img.youtube.com/vi/dMZs04TzxUI/mqdefault.jpg)](https://www.youtube.com/
```

### Comparing `nn_tilde-1.5.5/python_tools/__init__.py` & `nn_tilde-1.5.6/python_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `nn_tilde-1.5.5/setup.py` & `nn_tilde-1.5.6/setup.py`

 * *Files identical despite different names*

