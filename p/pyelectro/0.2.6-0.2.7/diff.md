# Comparing `tmp/pyelectro-0.2.6.tar.gz` & `tmp/pyelectro-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyelectro-0.2.6.tar", last modified: Thu Jun 22 16:45:47 2023, max compression
+gzip compressed data, was "pyelectro-0.2.7.tar", last modified: Thu Jun 22 16:51:41 2023, max compression
```

## Comparing `pyelectro-0.2.6.tar` & `pyelectro-0.2.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 padraig   (1000) padraig   (1000)        0 2023-06-22 16:45:47.165955 pyelectro-0.2.6/
--rw-rw-r--   0 padraig   (1000) padraig   (1000)     1502 2023-06-22 16:45:12.000000 pyelectro-0.2.6/LICENSE
--rw-rw-r--   0 padraig   (1000) padraig   (1000)     3986 2023-06-22 16:45:47.165955 pyelectro-0.2.6/PKG-INFO
--rw-------   0 padraig   (1000) padraig   (1000)     1624 2023-06-22 16:43:34.000000 pyelectro-0.2.6/README.md
-drwxrwxr-x   0 padraig   (1000) padraig   (1000)        0 2023-06-22 16:45:47.165955 pyelectro-0.2.6/pyelectro/
--rw-rw-r--   0 padraig   (1000) padraig   (1000)      269 2023-06-22 16:35:51.000000 pyelectro-0.2.6/pyelectro/__init__.py
--rw-rw-r--   0 padraig   (1000) padraig   (1000)    54334 2021-12-02 17:14:22.000000 pyelectro-0.2.6/pyelectro/analysis.py
--rw-rw-r--   0 padraig   (1000) padraig   (1000)     1907 2021-12-02 17:14:22.000000 pyelectro-0.2.6/pyelectro/io.py
--rw-rw-r--   0 padraig   (1000) padraig   (1000)     6191 2021-12-02 17:14:22.000000 pyelectro-0.2.6/pyelectro/utils.py
-drwxrwxr-x   0 padraig   (1000) padraig   (1000)        0 2023-06-22 16:45:47.165955 pyelectro-0.2.6/pyelectro.egg-info/
--rw-rw-r--   0 padraig   (1000) padraig   (1000)     3986 2023-06-22 16:45:47.000000 pyelectro-0.2.6/pyelectro.egg-info/PKG-INFO
--rw-rw-r--   0 padraig   (1000) padraig   (1000)      307 2023-06-22 16:45:47.000000 pyelectro-0.2.6/pyelectro.egg-info/SOURCES.txt
--rw-rw-r--   0 padraig   (1000) padraig   (1000)        1 2023-06-22 16:45:47.000000 pyelectro-0.2.6/pyelectro.egg-info/dependency_links.txt
--rw-rw-r--   0 padraig   (1000) padraig   (1000)       48 2023-06-22 16:45:47.000000 pyelectro-0.2.6/pyelectro.egg-info/requires.txt
--rw-rw-r--   0 padraig   (1000) padraig   (1000)       10 2023-06-22 16:45:47.000000 pyelectro-0.2.6/pyelectro.egg-info/top_level.txt
--rw-rw-r--   0 padraig   (1000) padraig   (1000)       81 2023-06-22 16:35:51.000000 pyelectro-0.2.6/pyproject.toml
--rw-rw-r--   0 padraig   (1000) padraig   (1000)     1095 2023-06-22 16:45:47.165955 pyelectro-0.2.6/setup.cfg
-drwxrwxr-x   0 padraig   (1000) padraig   (1000)        0 2023-06-22 16:45:47.165955 pyelectro-0.2.6/test/
--rw-rw-r--   0 padraig   (1000) padraig   (1000)     9098 2021-11-25 09:49:14.000000 pyelectro-0.2.6/test/test_analysis.py
+drwxrwxr-x   0 padraig   (1000) padraig   (1000)        0 2023-06-22 16:51:41.039121 pyelectro-0.2.7/
+-rw-rw-r--   0 padraig   (1000) padraig   (1000)     1501 2023-06-22 16:46:32.000000 pyelectro-0.2.7/LICENSE
+-rw-rw-r--   0 padraig   (1000) padraig   (1000)     2523 2023-06-22 16:51:41.039121 pyelectro-0.2.7/PKG-INFO
+-rw-------   0 padraig   (1000) padraig   (1000)     1624 2023-06-22 16:43:34.000000 pyelectro-0.2.7/README.md
+drwxrwxr-x   0 padraig   (1000) padraig   (1000)        0 2023-06-22 16:51:41.039121 pyelectro-0.2.7/pyelectro/
+-rw-rw-r--   0 padraig   (1000) padraig   (1000)      269 2023-06-22 16:35:51.000000 pyelectro-0.2.7/pyelectro/__init__.py
+-rw-rw-r--   0 padraig   (1000) padraig   (1000)    54334 2021-12-02 17:14:22.000000 pyelectro-0.2.7/pyelectro/analysis.py
+-rw-rw-r--   0 padraig   (1000) padraig   (1000)     1907 2021-12-02 17:14:22.000000 pyelectro-0.2.7/pyelectro/io.py
+-rw-rw-r--   0 padraig   (1000) padraig   (1000)     6191 2021-12-02 17:14:22.000000 pyelectro-0.2.7/pyelectro/utils.py
+drwxrwxr-x   0 padraig   (1000) padraig   (1000)        0 2023-06-22 16:51:41.039121 pyelectro-0.2.7/pyelectro.egg-info/
+-rw-rw-r--   0 padraig   (1000) padraig   (1000)     2523 2023-06-22 16:51:41.000000 pyelectro-0.2.7/pyelectro.egg-info/PKG-INFO
+-rw-rw-r--   0 padraig   (1000) padraig   (1000)      307 2023-06-22 16:51:41.000000 pyelectro-0.2.7/pyelectro.egg-info/SOURCES.txt
+-rw-rw-r--   0 padraig   (1000) padraig   (1000)        1 2023-06-22 16:51:41.000000 pyelectro-0.2.7/pyelectro.egg-info/dependency_links.txt
+-rw-rw-r--   0 padraig   (1000) padraig   (1000)       48 2023-06-22 16:51:41.000000 pyelectro-0.2.7/pyelectro.egg-info/requires.txt
+-rw-rw-r--   0 padraig   (1000) padraig   (1000)       10 2023-06-22 16:51:41.000000 pyelectro-0.2.7/pyelectro.egg-info/top_level.txt
+-rw-rw-r--   0 padraig   (1000) padraig   (1000)       81 2023-06-22 16:35:51.000000 pyelectro-0.2.7/pyproject.toml
+-rw-rw-r--   0 padraig   (1000) padraig   (1000)     1132 2023-06-22 16:51:41.039121 pyelectro-0.2.7/setup.cfg
+drwxrwxr-x   0 padraig   (1000) padraig   (1000)        0 2023-06-22 16:51:41.039121 pyelectro-0.2.7/test/
+-rw-rw-r--   0 padraig   (1000) padraig   (1000)     9098 2021-11-25 09:49:14.000000 pyelectro-0.2.7/test/test_analysis.py
```

### Comparing `pyelectro-0.2.6/LICENSE` & `pyelectro-0.2.7/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 Copyright (c) 2023, libNeuroML authors and contributors
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 * Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
-
 Neither the names of the copyright holders nor the names of the contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 
 THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `pyelectro-0.2.6/README.md` & `pyelectro-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `pyelectro-0.2.6/pyelectro/analysis.py` & `pyelectro-0.2.7/pyelectro/analysis.py`

 * *Files identical despite different names*

### Comparing `pyelectro-0.2.6/pyelectro/io.py` & `pyelectro-0.2.7/pyelectro/io.py`

 * *Files identical despite different names*

### Comparing `pyelectro-0.2.6/pyelectro/utils.py` & `pyelectro-0.2.7/pyelectro/utils.py`

 * *Files identical despite different names*

### Comparing `pyelectro-0.2.6/setup.cfg` & `pyelectro-0.2.7/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [metadata]
 name = pyelectro
-version = 0.2.6
+version = 0.2.7
 author = Michael Vella, Padraig Gleeson
 author_email = mv333@cam.ac.uk, p.gleeson@gmail.com
 url = https://github.com/NeuralEnsemble/pyelectro
 license = BSD-2-clause
 description = A Python library for analysis of electrophysiological data
-long_description = file: README.md, LICENSE
+long_description = file: README.md
+long_description_content_type = text/markdown
 classifiers = 
 	License :: OSI Approved :: BSD License
 	Development Status :: 3 - Alpha
 	Intended Audience :: Science/Research
 	Natural Language :: English
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3.7
```

### Comparing `pyelectro-0.2.6/test/test_analysis.py` & `pyelectro-0.2.7/test/test_analysis.py`

 * *Files identical despite different names*

