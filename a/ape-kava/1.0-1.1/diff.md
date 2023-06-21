# Comparing `tmp/ape-kava-1.0.tar.gz` & `tmp/ape-kava-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-kava-1.0.tar", last modified: Wed Jun 21 21:24:04 2023, max compression
+gzip compressed data, was "ape-kava-1.1.tar", last modified: Wed Jun 21 21:30:19 2023, max compression
```

## Comparing `ape-kava-1.0.tar` & `ape-kava-1.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 raghu      (501) staff       (20)        0 2023-06-21 21:24:04.034883 ape-kava-1.0/
-drwxr-xr-x   0 raghu      (501) staff       (20)        0 2023-06-21 21:24:04.030576 ape-kava-1.0/.github/
-drwxr-xr-x   0 raghu      (501) staff       (20)        0 2023-06-21 21:24:04.031221 ape-kava-1.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 raghu      (501) staff       (20)      701 2023-06-21 14:35:39.000000 ape-kava-1.0/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 raghu      (501) staff       (20)      668 2023-06-21 14:35:39.000000 ape-kava-1.0/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 raghu      (501) staff       (20)     1268 2023-06-21 14:35:39.000000 ape-kava-1.0/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 raghu      (501) staff       (20)      474 2023-06-21 14:35:39.000000 ape-kava-1.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 raghu      (501) staff       (20)      651 2023-06-21 14:35:39.000000 ape-kava-1.0/.github/release-drafter.yml
-drwxr-xr-x   0 raghu      (501) staff       (20)        0 2023-06-21 21:24:04.032303 ape-kava-1.0/.github/workflows/
--rw-r--r--   0 raghu      (501) staff       (20)      618 2023-06-21 14:35:39.000000 ape-kava-1.0/.github/workflows/codeql.yaml
--rw-r--r--   0 raghu      (501) staff       (20)      624 2023-06-21 14:35:39.000000 ape-kava-1.0/.github/workflows/commitlint.yaml
--rw-r--r--   0 raghu      (501) staff       (20)      366 2023-06-21 14:35:39.000000 ape-kava-1.0/.github/workflows/draft.yaml
--rw-r--r--   0 raghu      (501) staff       (20)      554 2023-06-21 14:35:39.000000 ape-kava-1.0/.github/workflows/prtitle.yaml
--rw-r--r--   0 raghu      (501) staff       (20)      623 2023-06-21 14:35:39.000000 ape-kava-1.0/.github/workflows/publish.yaml
--rw-r--r--   0 raghu      (501) staff       (20)     2496 2023-06-21 14:35:39.000000 ape-kava-1.0/.github/workflows/test.yaml
--rw-r--r--   0 raghu      (501) staff       (20)     1719 2023-06-21 14:35:39.000000 ape-kava-1.0/.gitignore
--rw-r--r--   0 raghu      (501) staff       (20)       14 2023-06-21 14:35:39.000000 ape-kava-1.0/.mdformat.toml
--rw-r--r--   0 raghu      (501) staff       (20)      788 2023-06-21 14:35:39.000000 ape-kava-1.0/.pre-commit-config.yaml
--rw-r--r--   0 raghu      (501) staff       (20)     1662 2023-06-21 14:35:39.000000 ape-kava-1.0/CONTRIBUTING.md
--rw-r--r--   0 raghu      (501) staff       (20)    11342 2023-06-21 14:35:39.000000 ape-kava-1.0/LICENSE
--rw-r--r--   0 raghu      (501) staff       (20)     2003 2023-06-21 21:24:04.034979 ape-kava-1.0/PKG-INFO
--rw-r--r--   0 raghu      (501) staff       (20)     1048 2023-06-21 14:35:39.000000 ape-kava-1.0/README.md
-drwxr-xr-x   0 raghu      (501) staff       (20)        0 2023-06-21 21:24:04.033000 ape-kava-1.0/ape-kava/
--rw-r--r--   0 raghu      (501) staff       (20)      980 2023-06-21 20:30:13.000000 ape-kava-1.0/ape-kava/__init__.py
--rw-r--r--   0 raghu      (501) staff       (20)     1274 2023-06-21 20:36:15.000000 ape-kava-1.0/ape-kava/ecosystem.py
--rw-r--r--   0 raghu      (501) staff       (20)        0 2023-06-21 14:35:39.000000 ape-kava-1.0/ape-kava/py.typed
--rw-r--r--   0 raghu      (501) staff       (20)      155 2023-06-21 21:24:03.000000 ape-kava-1.0/ape-kava/version.py
-drwxr-xr-x   0 raghu      (501) staff       (20)        0 2023-06-21 21:24:04.033840 ape-kava-1.0/ape_kava.egg-info/
--rw-r--r--   0 raghu      (501) staff       (20)     2003 2023-06-21 21:24:03.000000 ape-kava-1.0/ape_kava.egg-info/PKG-INFO
--rw-r--r--   0 raghu      (501) staff       (20)      817 2023-06-21 21:24:04.000000 ape-kava-1.0/ape_kava.egg-info/SOURCES.txt
--rw-r--r--   0 raghu      (501) staff       (20)        1 2023-06-21 21:24:03.000000 ape-kava-1.0/ape_kava.egg-info/dependency_links.txt
--rw-r--r--   0 raghu      (501) staff       (20)        1 2023-06-21 21:11:11.000000 ape-kava-1.0/ape_kava.egg-info/not-zip-safe
--rw-r--r--   0 raghu      (501) staff       (20)      558 2023-06-21 21:24:03.000000 ape-kava-1.0/ape_kava.egg-info/requires.txt
--rw-r--r--   0 raghu      (501) staff       (20)       18 2023-06-21 21:24:03.000000 ape-kava-1.0/ape_kava.egg-info/top_level.txt
--rw-r--r--   0 raghu      (501) staff       (20)      949 2023-06-21 20:56:52.000000 ape-kava-1.0/pyproject.toml
--rw-r--r--   0 raghu      (501) staff       (20)      108 2023-06-21 21:24:04.035238 ape-kava-1.0/setup.cfg
--rw-r--r--   0 raghu      (501) staff       (20)     2963 2023-06-21 20:46:03.000000 ape-kava-1.0/setup.py
-drwxr-xr-x   0 raghu      (501) staff       (20)        0 2023-06-21 21:24:04.034665 ape-kava-1.0/tests/
--rw-r--r--   0 raghu      (501) staff       (20)        0 2023-06-21 14:35:39.000000 ape-kava-1.0/tests/__init__.py
--rw-r--r--   0 raghu      (501) staff       (20)      430 2023-06-21 20:58:37.000000 ape-kava-1.0/tests/conftest.py
--rw-r--r--   0 raghu      (501) staff       (20)      907 2023-06-21 20:52:18.000000 ape-kava-1.0/tests/test_integration.py
--rw-r--r--   0 raghu      (501) staff       (20)      508 2023-06-21 20:56:35.000000 ape-kava-1.0/tests/test_provider.py
+drwxr-xr-x   0 raghu      (501) staff       (20)        0 2023-06-21 21:30:19.561425 ape-kava-1.1/
+drwxr-xr-x   0 raghu      (501) staff       (20)        0 2023-06-21 21:30:19.556685 ape-kava-1.1/.github/
+drwxr-xr-x   0 raghu      (501) staff       (20)        0 2023-06-21 21:30:19.557363 ape-kava-1.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 raghu      (501) staff       (20)      701 2023-06-21 14:35:39.000000 ape-kava-1.1/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 raghu      (501) staff       (20)      668 2023-06-21 14:35:39.000000 ape-kava-1.1/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 raghu      (501) staff       (20)     1268 2023-06-21 14:35:39.000000 ape-kava-1.1/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 raghu      (501) staff       (20)      474 2023-06-21 14:35:39.000000 ape-kava-1.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 raghu      (501) staff       (20)      651 2023-06-21 14:35:39.000000 ape-kava-1.1/.github/release-drafter.yml
+drwxr-xr-x   0 raghu      (501) staff       (20)        0 2023-06-21 21:30:19.558415 ape-kava-1.1/.github/workflows/
+-rw-r--r--   0 raghu      (501) staff       (20)      618 2023-06-21 14:35:39.000000 ape-kava-1.1/.github/workflows/codeql.yaml
+-rw-r--r--   0 raghu      (501) staff       (20)      624 2023-06-21 14:35:39.000000 ape-kava-1.1/.github/workflows/commitlint.yaml
+-rw-r--r--   0 raghu      (501) staff       (20)      366 2023-06-21 14:35:39.000000 ape-kava-1.1/.github/workflows/draft.yaml
+-rw-r--r--   0 raghu      (501) staff       (20)      554 2023-06-21 14:35:39.000000 ape-kava-1.1/.github/workflows/prtitle.yaml
+-rw-r--r--   0 raghu      (501) staff       (20)      623 2023-06-21 14:35:39.000000 ape-kava-1.1/.github/workflows/publish.yaml
+-rw-r--r--   0 raghu      (501) staff       (20)     2496 2023-06-21 14:35:39.000000 ape-kava-1.1/.github/workflows/test.yaml
+-rw-r--r--   0 raghu      (501) staff       (20)     1719 2023-06-21 14:35:39.000000 ape-kava-1.1/.gitignore
+-rw-r--r--   0 raghu      (501) staff       (20)       14 2023-06-21 14:35:39.000000 ape-kava-1.1/.mdformat.toml
+-rw-r--r--   0 raghu      (501) staff       (20)      788 2023-06-21 14:35:39.000000 ape-kava-1.1/.pre-commit-config.yaml
+-rw-r--r--   0 raghu      (501) staff       (20)     1662 2023-06-21 14:35:39.000000 ape-kava-1.1/CONTRIBUTING.md
+-rw-r--r--   0 raghu      (501) staff       (20)    11342 2023-06-21 14:35:39.000000 ape-kava-1.1/LICENSE
+-rw-r--r--   0 raghu      (501) staff       (20)     2003 2023-06-21 21:30:19.561518 ape-kava-1.1/PKG-INFO
+-rw-r--r--   0 raghu      (501) staff       (20)     1048 2023-06-21 14:35:39.000000 ape-kava-1.1/README.md
+drwxr-xr-x   0 raghu      (501) staff       (20)        0 2023-06-21 21:30:19.559093 ape-kava-1.1/ape-kava/
+-rw-r--r--   0 raghu      (501) staff       (20)      980 2023-06-21 20:30:13.000000 ape-kava-1.1/ape-kava/__init__.py
+-rw-r--r--   0 raghu      (501) staff       (20)     1274 2023-06-21 20:36:15.000000 ape-kava-1.1/ape-kava/ecosystem.py
+-rw-r--r--   0 raghu      (501) staff       (20)        0 2023-06-21 14:35:39.000000 ape-kava-1.1/ape-kava/py.typed
+-rw-r--r--   0 raghu      (501) staff       (20)      155 2023-06-21 21:30:19.000000 ape-kava-1.1/ape-kava/version.py
+drwxr-xr-x   0 raghu      (501) staff       (20)        0 2023-06-21 21:30:19.560317 ape-kava-1.1/ape_kava.egg-info/
+-rw-r--r--   0 raghu      (501) staff       (20)     2003 2023-06-21 21:30:19.000000 ape-kava-1.1/ape_kava.egg-info/PKG-INFO
+-rw-r--r--   0 raghu      (501) staff       (20)      817 2023-06-21 21:30:19.000000 ape-kava-1.1/ape_kava.egg-info/SOURCES.txt
+-rw-r--r--   0 raghu      (501) staff       (20)        1 2023-06-21 21:30:19.000000 ape-kava-1.1/ape_kava.egg-info/dependency_links.txt
+-rw-r--r--   0 raghu      (501) staff       (20)        1 2023-06-21 21:11:11.000000 ape-kava-1.1/ape_kava.egg-info/not-zip-safe
+-rw-r--r--   0 raghu      (501) staff       (20)      558 2023-06-21 21:30:19.000000 ape-kava-1.1/ape_kava.egg-info/requires.txt
+-rw-r--r--   0 raghu      (501) staff       (20)        9 2023-06-21 21:30:19.000000 ape-kava-1.1/ape_kava.egg-info/top_level.txt
+-rw-r--r--   0 raghu      (501) staff       (20)      949 2023-06-21 20:56:52.000000 ape-kava-1.1/pyproject.toml
+-rw-r--r--   0 raghu      (501) staff       (20)      108 2023-06-21 21:30:19.561771 ape-kava-1.1/setup.cfg
+-rw-r--r--   0 raghu      (501) staff       (20)     2963 2023-06-21 21:28:23.000000 ape-kava-1.1/setup.py
+drwxr-xr-x   0 raghu      (501) staff       (20)        0 2023-06-21 21:30:19.561229 ape-kava-1.1/tests/
+-rw-r--r--   0 raghu      (501) staff       (20)        0 2023-06-21 14:35:39.000000 ape-kava-1.1/tests/__init__.py
+-rw-r--r--   0 raghu      (501) staff       (20)      430 2023-06-21 20:58:37.000000 ape-kava-1.1/tests/conftest.py
+-rw-r--r--   0 raghu      (501) staff       (20)      907 2023-06-21 20:52:18.000000 ape-kava-1.1/tests/test_integration.py
+-rw-r--r--   0 raghu      (501) staff       (20)      508 2023-06-21 20:56:35.000000 ape-kava-1.1/tests/test_provider.py
```

### Comparing `ape-kava-1.0/.github/ISSUE_TEMPLATE/bug.md` & `ape-kava-1.1/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-kava-1.0/.github/ISSUE_TEMPLATE/feature.md` & `ape-kava-1.1/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-kava-1.0/.github/ISSUE_TEMPLATE/work-item.md` & `ape-kava-1.1/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-kava-1.0/.github/release-drafter.yml` & `ape-kava-1.1/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-kava-1.0/.github/workflows/codeql.yaml` & `ape-kava-1.1/.github/workflows/codeql.yaml`

 * *Files identical despite different names*

### Comparing `ape-kava-1.0/.github/workflows/commitlint.yaml` & `ape-kava-1.1/.github/workflows/commitlint.yaml`

 * *Files identical despite different names*

### Comparing `ape-kava-1.0/.github/workflows/prtitle.yaml` & `ape-kava-1.1/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `ape-kava-1.0/.github/workflows/publish.yaml` & `ape-kava-1.1/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ape-kava-1.0/.github/workflows/test.yaml` & `ape-kava-1.1/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `ape-kava-1.0/.gitignore` & `ape-kava-1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-kava-1.0/.pre-commit-config.yaml` & `ape-kava-1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ape-kava-1.0/CONTRIBUTING.md` & `ape-kava-1.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-kava-1.0/LICENSE` & `ape-kava-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-kava-1.0/PKG-INFO` & `ape-kava-1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-kava
-Version: 1.0
+Version: 1.1
 Summary: ape-kava: Ecosystem plugin for Kava
 Home-page: https://github.com/0xRaghu/ape-kava
 Author: ApeWorX Ltd. | Kava
 Author-email: raghu.thiyagharajan@kava.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ape-kava-1.0/README.md` & `ape-kava-1.1/README.md`

 * *Files identical despite different names*

### Comparing `ape-kava-1.0/ape-kava/__init__.py` & `ape-kava-1.1/ape-kava/__init__.py`

 * *Files identical despite different names*

### Comparing `ape-kava-1.0/ape-kava/ecosystem.py` & `ape-kava-1.1/ape-kava/ecosystem.py`

 * *Files identical despite different names*

### Comparing `ape-kava-1.0/ape_kava.egg-info/PKG-INFO` & `ape-kava-1.1/ape_kava.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-kava
-Version: 1.0
+Version: 1.1
 Summary: ape-kava: Ecosystem plugin for Kava
 Home-page: https://github.com/0xRaghu/ape-kava
 Author: ApeWorX Ltd. | Kava
 Author-email: raghu.thiyagharajan@kava.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ape-kava-1.0/ape_kava.egg-info/SOURCES.txt` & `ape-kava-1.1/ape_kava.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ape-kava-1.0/ape_kava.egg-info/requires.txt` & `ape-kava-1.1/ape_kava.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ape-kava-1.0/pyproject.toml` & `ape-kava-1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ape-kava-1.0/setup.py` & `ape-kava-1.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,20 +57,20 @@
     url="https://github.com/0xRaghu/ape-kava",
     include_package_data=True,
     install_requires=[
         "eth-ape>=0.6.0,<0.7",
     ],
     python_requires=">=3.8,<4",
     extras_require=extras_require,
-    py_modules=["ape_kava"],
+    py_modules=["ape-kava"],
     license="Apache-2.0",
     zip_safe=False,
     keywords="ethereum",
     packages=find_packages(exclude=["tests", "tests.*"]),
-    package_data={"ape_kava": ["py.typed"]},
+    package_data={"ape-kava": ["py.typed"]},
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Natural Language :: English",
         "Operating System :: MacOS",
         "Operating System :: POSIX",
```

### Comparing `ape-kava-1.0/tests/test_integration.py` & `ape-kava-1.1/tests/test_integration.py`

 * *Files identical despite different names*

