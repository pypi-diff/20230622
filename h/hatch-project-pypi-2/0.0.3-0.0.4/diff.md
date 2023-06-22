# Comparing `tmp/hatch_project_pypi_2-0.0.3.tar.gz` & `tmp/hatch_project_pypi_2-0.0.4.tar.gz`

## Comparing `hatch_project_pypi_2-0.0.3.tar` & `hatch_project_pypi_2-0.0.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rwxr-xr-x   0        0        0      131 2020-02-02 00:00:00.000000 hatch_project_pypi_2-0.0.3/src/hatch_project_pypi_2/__about__.py
--rwxr-xr-x   0        0        0      109 2020-02-02 00:00:00.000000 hatch_project_pypi_2-0.0.3/src/hatch_project_pypi_2/__init__.py
--rwxr-xr-x   0        0        0       43 2020-02-02 00:00:00.000000 hatch_project_pypi_2-0.0.3/src/hatch_project_pypi_2/hello.py
--rwxr-xr-x   0        0        0      109 2020-02-02 00:00:00.000000 hatch_project_pypi_2-0.0.3/tests/__init__.py
--rwxr-xr-x   0        0        0     1101 2020-02-02 00:00:00.000000 hatch_project_pypi_2-0.0.3/LICENSE.txt
--rwxr-xr-x   0        0        0      562 2020-02-02 00:00:00.000000 hatch_project_pypi_2-0.0.3/README.md
--rwxr-xr-x   0        0        0     3258 2020-02-02 00:00:00.000000 hatch_project_pypi_2-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 hatch_project_pypi_2-0.0.3/PKG-INFO
+-rwxr-xr-x   0        0        0      131 2020-02-02 00:00:00.000000 hatch_project_pypi_2-0.0.4/src/hatch_project_pypi_2/__about__.py
+-rwxr-xr-x   0        0        0      109 2020-02-02 00:00:00.000000 hatch_project_pypi_2-0.0.4/src/hatch_project_pypi_2/__init__.py
+-rwxr-xr-x   0        0        0       43 2020-02-02 00:00:00.000000 hatch_project_pypi_2-0.0.4/src/hatch_project_pypi_2/hello.py
+-rwxr-xr-x   0        0        0      109 2020-02-02 00:00:00.000000 hatch_project_pypi_2-0.0.4/tests/__init__.py
+-rwxr-xr-x   0        0        0     1101 2020-02-02 00:00:00.000000 hatch_project_pypi_2-0.0.4/LICENSE.txt
+-rwxr-xr-x   0        0        0      562 2020-02-02 00:00:00.000000 hatch_project_pypi_2-0.0.4/README.md
+-rwxr-xr-x   0        0        0     3285 2020-02-02 00:00:00.000000 hatch_project_pypi_2-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 hatch_project_pypi_2-0.0.4/PKG-INFO
```

### Comparing `hatch_project_pypi_2-0.0.3/LICENSE.txt` & `hatch_project_pypi_2-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hatch_project_pypi_2-0.0.3/README.md` & `hatch_project_pypi_2-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `hatch_project_pypi_2-0.0.3/pyproject.toml` & `hatch_project_pypi_2-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "hatch-project-pypi-2"
 dynamic = ["version"]
-description = ''
+description = "ハッチプロのテスト"
 readme = "README.md"
 requires-python = ">=3.7"
 license = "MIT"
 keywords = []
 authors = [
   { name = "Kenno-Warise", email = "wariken0523@gmail.com" },
 ]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hatch_project_pypi_2-0.0.3/PKG-INFO` & `hatch_project_pypi_2-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: hatch-project-pypi-2
-Version: 0.0.3
+Version: 0.0.4
+Summary: ハッチプロのテスト
 Project-URL: Documentation, https://github.com/unknown/hatch-project-pypi-2#readme
 Project-URL: Issues, https://github.com/unknown/hatch-project-pypi-2/issues
 Project-URL: Source, https://github.com/unknown/hatch-project-pypi-2
 Author-email: Kenno-Warise <wariken0523@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

