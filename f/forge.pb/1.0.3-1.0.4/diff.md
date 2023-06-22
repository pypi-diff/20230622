# Comparing `tmp/forge.pb-1.0.3.tar.gz` & `tmp/forge.pb-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forge.pb-1.0.3.tar", last modified: Wed Jan 26 17:59:33 2022, max compression
+gzip compressed data, was "forge.pb-1.0.4.tar", last modified: Thu Jun 22 17:25:20 2023, max compression
```

## Comparing `forge.pb-1.0.3.tar` & `forge.pb-1.0.4.tar`

### file list

```diff
@@ -1,27 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 17:59:33.134920 forge.pb-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (121)    11356 2022-01-26 17:59:10.000000 forge.pb-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2609 2022-01-26 17:59:33.134920 forge.pb-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2277 2022-01-26 17:59:10.000000 forge.pb-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 17:59:33.130920 forge.pb-1.0.3/forge.pb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2609 2022-01-26 17:59:33.000000 forge.pb-1.0.3/forge.pb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      474 2022-01-26 17:59:33.000000 forge.pb-1.0.3/forge.pb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-26 17:59:33.000000 forge.pb-1.0.3/forge.pb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-01-26 17:59:33.000000 forge.pb-1.0.3/forge.pb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      331 2022-01-26 17:59:33.000000 forge.pb-1.0.3/forge.pb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-01-26 17:59:33.000000 forge.pb-1.0.3/forge.pb.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 17:59:33.134920 forge.pb-1.0.3/forgepb/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 17:59:10.000000 forge.pb-1.0.3/forgepb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-01-26 17:59:10.000000 forge.pb-1.0.3/forgepb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12370 2022-01-26 17:59:10.000000 forge.pb-1.0.3/forgepb/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 17:59:33.134920 forge.pb-1.0.3/forgepb/cmd/
--rw-r--r--   0 runner    (1001) docker     (121)      742 2022-01-26 17:59:10.000000 forge.pb-1.0.3/forgepb/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      506 2022-01-26 17:59:10.000000 forge.pb-1.0.3/forgepb/cmd/config.py
--rw-r--r--   0 runner    (1001) docker     (121)    10406 2022-01-26 17:59:10.000000 forge.pb-1.0.3/forgepb/cmd/node.py
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-01-26 17:59:10.000000 forge.pb-1.0.3/forgepb/cmd/provenance.py
--rw-r--r--   0 runner    (1001) docker     (121)     1262 2022-01-26 17:59:10.000000 forge.pb-1.0.3/forgepb/command_line.py
--rw-r--r--   0 runner    (1001) docker     (121)     1432 2022-01-26 17:59:10.000000 forge.pb-1.0.3/forgepb/config_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)     1032 2022-01-26 17:59:10.000000 forge.pb-1.0.3/forgepb/forge.py
--rw-r--r--   0 runner    (1001) docker     (121)     1524 2022-01-26 17:59:10.000000 forge.pb-1.0.3/forgepb/global_.py
--rw-r--r--   0 runner    (1001) docker     (121)    16263 2022-01-26 17:59:10.000000 forge.pb-1.0.3/forgepb/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-26 17:59:33.134920 forge.pb-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      788 2022-01-26 17:59:10.000000 forge.pb-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:25:20.803397 forge.pb-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-06-22 17:25:15.000000 forge.pb-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-06-22 17:25:20.803397 forge.pb-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-06-22 17:25:15.000000 forge.pb-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:25:20.803397 forge.pb-1.0.4/forge.pb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-06-22 17:25:20.000000 forge.pb-1.0.4/forge.pb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-22 17:25:20.000000 forge.pb-1.0.4/forge.pb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 17:25:20.000000 forge.pb-1.0.4/forge.pb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-22 17:25:20.000000 forge.pb-1.0.4/forge.pb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-22 17:25:20.000000 forge.pb-1.0.4/forge.pb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-22 17:25:20.000000 forge.pb-1.0.4/forge.pb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:25:20.803397 forge.pb-1.0.4/forgepb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 17:25:15.000000 forge.pb-1.0.4/forgepb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-22 17:25:15.000000 forge.pb-1.0.4/forgepb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12370 2023-06-22 17:25:15.000000 forge.pb-1.0.4/forgepb/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:25:20.803397 forge.pb-1.0.4/forgepb/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-22 17:25:15.000000 forge.pb-1.0.4/forgepb/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-22 17:25:15.000000 forge.pb-1.0.4/forgepb/cmd/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10406 2023-06-22 17:25:15.000000 forge.pb-1.0.4/forgepb/cmd/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-22 17:25:15.000000 forge.pb-1.0.4/forgepb/cmd/provenance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-22 17:25:15.000000 forge.pb-1.0.4/forgepb/command_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-22 17:25:15.000000 forge.pb-1.0.4/forgepb/config_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-22 17:25:15.000000 forge.pb-1.0.4/forgepb/forge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-22 17:25:15.000000 forge.pb-1.0.4/forgepb/global_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16263 2023-06-22 17:25:15.000000 forge.pb-1.0.4/forgepb/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 17:25:20.803397 forge.pb-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-22 17:25:15.000000 forge.pb-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:25:20.803397 forge.pb-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    11090 2023-06-22 17:25:15.000000 forge.pb-1.0.4/tests/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-06-22 17:25:15.000000 forge.pb-1.0.4/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-06-22 17:25:15.000000 forge.pb-1.0.4/tests/test_variables.py
```

### Comparing `forge.pb-1.0.3/LICENSE` & `forge.pb-1.0.4/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2021 Provenance Blockchain, Inc
+   Copyright 2021 Figure Technologies, Inc
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `forge.pb-1.0.3/PKG-INFO` & `forge.pb-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: forge.pb
-Version: 1.0.3
+Version: 1.0.4
 Summary: Node manager for the Provenance Blockchain
 Home-page: https://github.com/provenance-io/forge.pb
 Author: Wyatt Baker
 Author-email: wbaker@figure.com
-License: UNKNOWN
-Platform: UNKNOWN
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Forge.pb - Provenance Blockchain Process Manager
 
 ## Description
 The Provenance Blockchain Manager is an application for automated startup of nodes on the [Provenance Blockchain](https://docs.provenance.io/) testnet, mainnet, or localnet which can be used for testing.
 
 ## Getting Started
-Forge is available on [Pypi](https://pypi.org/project/forge.pb/) and the repo is on [GitHub](https://github.com/provenance-io/forge.pb) and can be installed using pip.
+Forge is available on [Pypi](https://pypi.org/project/forge.pb/) and the repo is on [GitHub](https://github.com/FigureTechnologies/forge.pb) and can be installed using pip.
 ```
 pip install forge.pb
 ```
 or
 ```
 pip install forge.pb==1.0.2
 ```
@@ -62,10 +60,8 @@
 ```
 You can also drill into the individual commands for more help and additional commands:
 ```sh
 forge node --help
 ```
 
 ## Version Info
-* Python 3.6
-
-
+* Python 3.7
```

### Comparing `forge.pb-1.0.3/README.md` & `forge.pb-1.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Forge.pb - Provenance Blockchain Process Manager
 
 ## Description
 The Provenance Blockchain Manager is an application for automated startup of nodes on the [Provenance Blockchain](https://docs.provenance.io/) testnet, mainnet, or localnet which can be used for testing.
 
 ## Getting Started
-Forge is available on [Pypi](https://pypi.org/project/forge.pb/) and the repo is on [GitHub](https://github.com/provenance-io/forge.pb) and can be installed using pip.
+Forge is available on [Pypi](https://pypi.org/project/forge.pb/) and the repo is on [GitHub](https://github.com/FigureTechnologies/forge.pb) and can be installed using pip.
 ```
 pip install forge.pb
 ```
 or
 ```
 pip install forge.pb==1.0.2
 ```
@@ -49,8 +49,8 @@
 ```
 You can also drill into the individual commands for more help and additional commands:
 ```sh
 forge node --help
 ```
 
 ## Version Info
-* Python 3.6
+* Python 3.7
```

### Comparing `forge.pb-1.0.3/forge.pb.egg-info/PKG-INFO` & `forge.pb-1.0.4/forge.pb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: forge.pb
-Version: 1.0.3
+Version: 1.0.4
 Summary: Node manager for the Provenance Blockchain
 Home-page: https://github.com/provenance-io/forge.pb
 Author: Wyatt Baker
 Author-email: wbaker@figure.com
-License: UNKNOWN
-Platform: UNKNOWN
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Forge.pb - Provenance Blockchain Process Manager
 
 ## Description
 The Provenance Blockchain Manager is an application for automated startup of nodes on the [Provenance Blockchain](https://docs.provenance.io/) testnet, mainnet, or localnet which can be used for testing.
 
 ## Getting Started
-Forge is available on [Pypi](https://pypi.org/project/forge.pb/) and the repo is on [GitHub](https://github.com/provenance-io/forge.pb) and can be installed using pip.
+Forge is available on [Pypi](https://pypi.org/project/forge.pb/) and the repo is on [GitHub](https://github.com/FigureTechnologies/forge.pb) and can be installed using pip.
 ```
 pip install forge.pb
 ```
 or
 ```
 pip install forge.pb==1.0.2
 ```
@@ -62,10 +60,8 @@
 ```
 You can also drill into the individual commands for more help and additional commands:
 ```sh
 forge node --help
 ```
 
 ## Version Info
-* Python 3.6
-
-
+* Python 3.7
```

### Comparing `forge.pb-1.0.3/forgepb/builder.py` & `forge.pb-1.0.4/forgepb/builder.py`

 * *Files identical despite different names*

### Comparing `forge.pb-1.0.3/forgepb/cmd/__init__.py` & `forge.pb-1.0.4/forgepb/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `forge.pb-1.0.3/forgepb/cmd/node.py` & `forge.pb-1.0.4/forgepb/cmd/node.py`

 * *Files identical despite different names*

### Comparing `forge.pb-1.0.3/forgepb/command_line.py` & `forge.pb-1.0.4/forgepb/command_line.py`

 * *Files identical despite different names*

### Comparing `forge.pb-1.0.3/forgepb/config_handler.py` & `forge.pb-1.0.4/forgepb/config_handler.py`

 * *Files identical despite different names*

### Comparing `forge.pb-1.0.3/forgepb/forge.py` & `forge.pb-1.0.4/forgepb/forge.py`

 * *Files identical despite different names*

### Comparing `forge.pb-1.0.3/forgepb/global_.py` & `forge.pb-1.0.4/forgepb/global_.py`

 * *Files identical despite different names*

### Comparing `forge.pb-1.0.3/forgepb/utils.py` & `forge.pb-1.0.4/forgepb/utils.py`

 * *Files identical despite different names*

### Comparing `forge.pb-1.0.3/setup.py` & `forge.pb-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.read()
 
 setup(
     name="forge.pb",
-    version="1.0.3",
+    version="1.0.4",
     url='https://github.com/provenance-io/forge.pb',
     author='Wyatt Baker',
     author_email='wbaker@figure.com',
     packages=['forgepb','forgepb.cmd'],
     install_requires = [requirements],
-    python_requires='>=3.6',
+    python_requires='>=3.7',
     entry_points={
         'console_scripts': [
             'forge=forgepb.command_line:start'
         ]
     },
     keyword="provenance, node, bootstrap",
     description="Node manager for the Provenance Blockchain",
```

