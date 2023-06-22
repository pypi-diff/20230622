# Comparing `tmp/pmkoalas-0.0.1a2.tar.gz` & `tmp/pmkoalas-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pmkoalas-0.0.1a2.tar", last modified: Mon Apr 24 04:53:27 2023, max compression
+gzip compressed data, was "pmkoalas-0.2.tar", last modified: Thu Jun 22 03:23:17 2023, max compression
```

## Comparing `pmkoalas-0.0.1a2.tar` & `pmkoalas-0.2.tar`

### file list

```diff
@@ -1,34 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 04:53:27.933278 pmkoalas-0.0.1a2/
--rw-rw-rw-   0        0        0     1094 2022-08-18 07:14:37.000000 pmkoalas-0.0.1a2/LICENSE
--rw-rw-rw-   0        0        0     3152 2023-04-24 04:53:27.932280 pmkoalas-0.0.1a2/PKG-INFO
--rw-rw-rw-   0        0        0     1222 2023-04-24 04:48:17.000000 pmkoalas-0.0.1a2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 04:53:27.903964 pmkoalas-0.0.1a2/pmkoalas/
--rw-rw-rw-   0        0        0       29 2023-04-24 04:53:12.000000 pmkoalas-0.0.1a2/pmkoalas/__init__.py
--rw-rw-rw-   0        0        0     2705 2023-04-24 04:48:17.000000 pmkoalas-0.0.1a2/pmkoalas/_logging.py
--rw-rw-rw-   0        0        0    11208 2023-04-24 04:48:17.000000 pmkoalas-0.0.1a2/pmkoalas/complex.py
--rw-rw-rw-   0        0        0    17693 2023-04-24 04:48:17.000000 pmkoalas-0.0.1a2/pmkoalas/directly.py
--rw-rw-rw-   0        0        0      706 2023-04-24 04:48:17.000000 pmkoalas-0.0.1a2/pmkoalas/dtlog.py
--rw-rw-rw-   0        0        0        0 2023-04-24 04:48:17.000000 pmkoalas-0.0.1a2/pmkoalas/eventlog.py
--rw-rw-rw-   0        0        0     9574 2023-04-24 04:48:17.000000 pmkoalas-0.0.1a2/pmkoalas/export.py
--rw-rw-rw-   0        0        0    10090 2023-04-24 04:48:17.000000 pmkoalas-0.0.1a2/pmkoalas/read.py
--rw-rw-rw-   0        0        0     9240 2023-04-24 04:48:17.000000 pmkoalas-0.0.1a2/pmkoalas/simple.py
--rw-rw-rw-   0        0        0        0 2023-04-24 04:48:17.000000 pmkoalas-0.0.1a2/pmkoalas/work.py
--rw-rw-rw-   0        0        0      192 2023-04-24 04:48:17.000000 pmkoalas-0.0.1a2/pmkoalas/xes.py
--rw-rw-rw-   0        0        0     5221 2023-04-24 04:48:17.000000 pmkoalas-0.0.1a2/pmkoalas/xes_export.py
-drwxrwxrwx   0        0        0        0 2023-04-24 04:53:27.914328 pmkoalas-0.0.1a2/pmkoalas.egg-info/
--rw-rw-rw-   0        0        0     3152 2023-04-24 04:53:27.000000 pmkoalas-0.0.1a2/pmkoalas.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      620 2023-04-24 04:53:27.000000 pmkoalas-0.0.1a2/pmkoalas.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 04:53:27.000000 pmkoalas-0.0.1a2/pmkoalas.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-04-24 04:53:27.000000 pmkoalas-0.0.1a2/pmkoalas.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-24 04:53:27.000000 pmkoalas-0.0.1a2/pmkoalas.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      917 2023-04-24 04:53:04.000000 pmkoalas-0.0.1a2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-24 04:53:27.933278 pmkoalas-0.0.1a2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-24 04:53:27.930286 pmkoalas-0.0.1a2/tests/
--rw-rw-rw-   0        0        0     7858 2023-04-24 04:48:17.000000 pmkoalas-0.0.1a2/tests/test_alpha.py
--rw-rw-rw-   0        0        0     3819 2023-04-24 04:48:17.000000 pmkoalas-0.0.1a2/tests/test_drelations.py
--rw-rw-rw-   0        0        0     1214 2023-04-24 04:48:17.000000 pmkoalas-0.0.1a2/tests/test_dtlog.py
--rw-rw-rw-   0        0        0     3260 2023-04-24 04:48:17.000000 pmkoalas-0.0.1a2/tests/test_export_complex.py
--rw-rw-rw-   0        0        0     2278 2023-04-24 04:48:17.000000 pmkoalas-0.0.1a2/tests/test_export_simple.py
--rw-rw-rw-   0        0        0     4079 2023-04-24 04:48:17.000000 pmkoalas-0.0.1a2/tests/test_read_complex.py
--rw-rw-rw-   0        0        0     1976 2023-04-24 04:48:17.000000 pmkoalas-0.0.1a2/tests/test_read_simple.py
--rw-rw-rw-   0        0        0     1577 2023-04-24 04:48:17.000000 pmkoalas-0.0.1a2/tests/test_simple.py
+drwxrwxrwx   0        0        0        0 2023-06-22 03:23:17.334381 pmkoalas-0.2/
+-rw-rw-rw-   0        0        0     1095 2022-10-22 22:45:35.000000 pmkoalas-0.2/LICENSE
+-rw-rw-rw-   0        0        0     4040 2023-06-22 03:23:17.333383 pmkoalas-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2132 2023-06-22 02:19:40.000000 pmkoalas-0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 03:23:17.310191 pmkoalas-0.2/pmkoalas/
+-rw-rw-rw-   0        0        0       19 2023-06-22 02:19:40.000000 pmkoalas-0.2/pmkoalas/__init__.py
+-rw-rw-rw-   0        0        0     2705 2023-06-22 02:19:40.000000 pmkoalas-0.2/pmkoalas/_logging.py
+-rw-rw-rw-   0        0        0    11208 2023-06-22 02:19:40.000000 pmkoalas-0.2/pmkoalas/complex.py
+-rw-rw-rw-   0        0        0    17693 2023-06-22 02:19:40.000000 pmkoalas-0.2/pmkoalas/directly.py
+-rw-rw-rw-   0        0        0      706 2023-06-22 03:18:45.000000 pmkoalas-0.2/pmkoalas/dtlog.py
+-rw-rw-rw-   0        0        0        0 2023-06-22 02:19:40.000000 pmkoalas-0.2/pmkoalas/eventlog.py
+-rw-rw-rw-   0        0        0     9574 2023-06-22 02:19:40.000000 pmkoalas-0.2/pmkoalas/export.py
+-rw-rw-rw-   0        0        0    10090 2023-06-22 02:19:40.000000 pmkoalas-0.2/pmkoalas/read.py
+-rw-rw-rw-   0        0        0     9240 2023-06-22 02:19:40.000000 pmkoalas-0.2/pmkoalas/simple.py
+-rw-rw-rw-   0        0        0        0 2023-06-22 02:19:40.000000 pmkoalas-0.2/pmkoalas/work.py
+-rw-rw-rw-   0        0        0      192 2023-06-22 02:19:40.000000 pmkoalas-0.2/pmkoalas/xes.py
+-rw-rw-rw-   0        0        0     5221 2023-06-22 02:19:40.000000 pmkoalas-0.2/pmkoalas/xes_export.py
+drwxrwxrwx   0        0        0        0 2023-06-22 03:23:17.326193 pmkoalas-0.2/pmkoalas.egg-info/
+-rw-rw-rw-   0        0        0     4040 2023-06-22 03:23:17.000000 pmkoalas-0.2/pmkoalas.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      600 2023-06-22 03:23:17.000000 pmkoalas-0.2/pmkoalas.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 03:23:17.000000 pmkoalas-0.2/pmkoalas.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-06-22 03:23:17.000000 pmkoalas-0.2/pmkoalas.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-22 03:23:17.000000 pmkoalas-0.2/pmkoalas.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      874 2023-06-22 02:19:40.000000 pmkoalas-0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-22 03:23:17.334381 pmkoalas-0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-22 03:23:17.332381 pmkoalas-0.2/tests/
+-rw-rw-rw-   0        0        0     3819 2023-06-22 02:26:48.000000 pmkoalas-0.2/tests/test_drelations.py
+-rw-rw-rw-   0        0        0     1214 2023-06-22 03:18:45.000000 pmkoalas-0.2/tests/test_dtlog.py
+-rw-rw-rw-   0        0        0     3260 2023-06-22 02:19:40.000000 pmkoalas-0.2/tests/test_export_complex.py
+-rw-rw-rw-   0        0        0     2278 2023-06-22 02:19:40.000000 pmkoalas-0.2/tests/test_export_simple.py
+-rw-rw-rw-   0        0        0     4079 2023-06-22 02:19:40.000000 pmkoalas-0.2/tests/test_read_complex.py
+-rw-rw-rw-   0        0        0     1976 2023-06-22 02:19:40.000000 pmkoalas-0.2/tests/test_read_simple.py
+-rw-rw-rw-   0        0        0     1577 2023-06-22 02:25:48.000000 pmkoalas-0.2/tests/test_simple.py
```

### Comparing `pmkoalas-0.0.1a2/LICENSE` & `pmkoalas-0.2/LICENSE`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `pmkoalas-0.0.1a2/pmkoalas/_logging.py` & `pmkoalas-0.2/pmkoalas/_logging.py`

 * *Files identical despite different names*

### Comparing `pmkoalas-0.0.1a2/pmkoalas/complex.py` & `pmkoalas-0.2/pmkoalas/complex.py`

 * *Files identical despite different names*

### Comparing `pmkoalas-0.0.1a2/pmkoalas/directly.py` & `pmkoalas-0.2/pmkoalas/directly.py`

 * *Files identical despite different names*

### Comparing `pmkoalas-0.0.1a2/pmkoalas/dtlog.py` & `pmkoalas-0.2/pmkoalas/dtlog.py`

 * *Files identical despite different names*

### Comparing `pmkoalas-0.0.1a2/pmkoalas/export.py` & `pmkoalas-0.2/pmkoalas/export.py`

 * *Files identical despite different names*

### Comparing `pmkoalas-0.0.1a2/pmkoalas/read.py` & `pmkoalas-0.2/pmkoalas/read.py`

 * *Files identical despite different names*

### Comparing `pmkoalas-0.0.1a2/pmkoalas/simple.py` & `pmkoalas-0.2/pmkoalas/simple.py`

 * *Files identical despite different names*

### Comparing `pmkoalas-0.0.1a2/pmkoalas/xes_export.py` & `pmkoalas-0.2/pmkoalas/xes_export.py`

 * *Files identical despite different names*

### Comparing `pmkoalas-0.0.1a2/pmkoalas.egg-info/SOURCES.txt` & `pmkoalas-0.2/pmkoalas.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 pmkoalas/xes.py
 pmkoalas/xes_export.py
 pmkoalas.egg-info/PKG-INFO
 pmkoalas.egg-info/SOURCES.txt
 pmkoalas.egg-info/dependency_links.txt
 pmkoalas.egg-info/requires.txt
 pmkoalas.egg-info/top_level.txt
-tests/test_alpha.py
 tests/test_drelations.py
 tests/test_dtlog.py
 tests/test_export_complex.py
 tests/test_export_simple.py
 tests/test_read_complex.py
 tests/test_read_simple.py
 tests/test_simple.py
```

### Comparing `pmkoalas-0.0.1a2/pyproject.toml` & `pmkoalas-0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pmkoalas"
-version = "0.0.1-alpha.2"
+version = "0.2"
 authors = [
   { name="Adam Banham", email="adam_banham@hotmail.com" },
-  { name="Adam Burke", email="adam_burke_mail@yahoo.com" },
+  { name="Adam Burke" },
 ]
 description = "A process mining library that focuses on providing pythonic interactions with event logs and languages."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -30,8 +30,8 @@
 [tool.setuptools]
 packages = [
 "pmkoalas"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/AdamBanham/koalas"
-"Bug Tracker" = "https://github.com/AdamBanham/koalas/issues"
+"Bug Tracker" = "https://github.com/AdamBanham/koalas/issues"
```

### Comparing `pmkoalas-0.0.1a2/tests/test_drelations.py` & `pmkoalas-0.2/tests/test_drelations.py`

 * *Files identical despite different names*

### Comparing `pmkoalas-0.0.1a2/tests/test_dtlog.py` & `pmkoalas-0.2/tests/test_dtlog.py`

 * *Files identical despite different names*

### Comparing `pmkoalas-0.0.1a2/tests/test_export_complex.py` & `pmkoalas-0.2/tests/test_export_complex.py`

 * *Files identical despite different names*

### Comparing `pmkoalas-0.0.1a2/tests/test_export_simple.py` & `pmkoalas-0.2/tests/test_export_simple.py`

 * *Files identical despite different names*

### Comparing `pmkoalas-0.0.1a2/tests/test_read_complex.py` & `pmkoalas-0.2/tests/test_read_complex.py`

 * *Files identical despite different names*

### Comparing `pmkoalas-0.0.1a2/tests/test_read_simple.py` & `pmkoalas-0.2/tests/test_read_simple.py`

 * *Files identical despite different names*

### Comparing `pmkoalas-0.0.1a2/tests/test_simple.py` & `pmkoalas-0.2/tests/test_simple.py`

 * *Files identical despite different names*

