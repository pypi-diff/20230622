# Comparing `tmp/payload_tagger-0.1.1.tar.gz` & `tmp/payload_tagger-0.1.2.tar.gz`

## Comparing `payload_tagger-0.1.1.tar` & `payload_tagger-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 payload_tagger-0.1.1/.tool-versions
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 payload_tagger-0.1.1/.github/CODEOWNERS
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 payload_tagger-0.1.1/.github/workflows/release.yml
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 payload_tagger-0.1.1/.github/workflows/test.yml
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 payload_tagger-0.1.1/.vscode/settings.json
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 payload_tagger-0.1.1/payload_tagger/__init__.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 payload_tagger-0.1.1/payload_tagger/errors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 payload_tagger-0.1.1/payload_tagger/py.typed
--rw-r--r--   0        0        0     5331 2020-02-02 00:00:00.000000 payload_tagger-0.1.1/payload_tagger/whatsapp.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 payload_tagger-0.1.1/requirements/core.txt
--rw-r--r--   0        0        0     3801 2020-02-02 00:00:00.000000 payload_tagger-0.1.1/requirements/dev.txt
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 payload_tagger-0.1.1/scripts/release_github.py
--rw-r--r--   0        0        0    46092 2020-02-02 00:00:00.000000 payload_tagger-0.1.1/tests/unit/test_whastapp.py
--rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 payload_tagger-0.1.1/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 payload_tagger-0.1.1/LICENSE
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 payload_tagger-0.1.1/README.md
--rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 payload_tagger-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 payload_tagger-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 payload_tagger-0.1.2/.tool-versions
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 payload_tagger-0.1.2/.github/CODEOWNERS
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 payload_tagger-0.1.2/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 payload_tagger-0.1.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 payload_tagger-0.1.2/.vscode/settings.json
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 payload_tagger-0.1.2/payload_tagger/__init__.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 payload_tagger-0.1.2/payload_tagger/errors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 payload_tagger-0.1.2/payload_tagger/py.typed
+-rw-r--r--   0        0        0     5331 2020-02-02 00:00:00.000000 payload_tagger-0.1.2/payload_tagger/whatsapp.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 payload_tagger-0.1.2/requirements/core.txt
+-rw-r--r--   0        0        0     3801 2020-02-02 00:00:00.000000 payload_tagger-0.1.2/requirements/dev.txt
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 payload_tagger-0.1.2/scripts/release_github.py
+-rw-r--r--   0        0        0    46092 2020-02-02 00:00:00.000000 payload_tagger-0.1.2/tests/unit/test_whastapp.py
+-rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 payload_tagger-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 payload_tagger-0.1.2/LICENSE
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 payload_tagger-0.1.2/README.md
+-rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 payload_tagger-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 payload_tagger-0.1.2/PKG-INFO
```

### Comparing `payload_tagger-0.1.1/.github/workflows/release.yml` & `payload_tagger-0.1.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `payload_tagger-0.1.1/.github/workflows/test.yml` & `payload_tagger-0.1.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `payload_tagger-0.1.1/.vscode/settings.json` & `payload_tagger-0.1.2/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `payload_tagger-0.1.1/payload_tagger/whatsapp.py` & `payload_tagger-0.1.2/payload_tagger/whatsapp.py`

 * *Files identical despite different names*

### Comparing `payload_tagger-0.1.1/requirements/dev.txt` & `payload_tagger-0.1.2/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `payload_tagger-0.1.1/scripts/release_github.py` & `payload_tagger-0.1.2/scripts/release_github.py`

 * *Files identical despite different names*

### Comparing `payload_tagger-0.1.1/tests/unit/test_whastapp.py` & `payload_tagger-0.1.2/tests/unit/test_whastapp.py`

 * *Files identical despite different names*

### Comparing `payload_tagger-0.1.1/.gitignore` & `payload_tagger-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `payload_tagger-0.1.1/LICENSE` & `payload_tagger-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `payload_tagger-0.1.1/pyproject.toml` & `payload_tagger-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "payload_tagger"
-version = "0.1.1"
+version = "0.1.2"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
```

### Comparing `payload_tagger-0.1.1/PKG-INFO` & `payload_tagger-0.1.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: payload_tagger
-Version: 0.1.1
+Version: 0.1.2
 Project-URL: Documentation, https://github.com/Tomperez98/payload-tagger#readme
 Project-URL: Issues, https://github.com/Tomperez98/payload-tagger/issues
 Project-URL: Source, https://github.com/Tomperez98/payload-tagger
 License-File: LICENSE
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
```

