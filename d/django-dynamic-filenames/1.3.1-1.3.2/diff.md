# Comparing `tmp/django-dynamic-filenames-1.3.1.tar.gz` & `tmp/django-dynamic-filenames-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-dynamic-filenames-1.3.1.tar", last modified: Wed Oct  5 19:24:30 2022, max compression
+gzip compressed data, was "django-dynamic-filenames-1.3.2.tar", last modified: Thu Jun 22 06:38:57 2023, max compression
```

## Comparing `django-dynamic-filenames-1.3.1.tar` & `django-dynamic-filenames-1.3.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 19:24:30.465863 django-dynamic-filenames-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-10-05 19:24:17.000000 django-dynamic-filenames-1.3.1/.bandit
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 19:24:30.461863 django-dynamic-filenames-1.3.1/.github/
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-10-05 19:24:17.000000 django-dynamic-filenames-1.3.1/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-10-05 19:24:17.000000 django-dynamic-filenames-1.3.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 19:24:30.461863 django-dynamic-filenames-1.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1945 2022-10-05 19:24:17.000000 django-dynamic-filenames-1.3.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)      598 2022-10-05 19:24:17.000000 django-dynamic-filenames-1.3.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1203 2022-10-05 19:24:17.000000 django-dynamic-filenames-1.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-10-05 19:24:17.000000 django-dynamic-filenames-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3882 2022-10-05 19:24:30.465863 django-dynamic-filenames-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2824 2022-10-05 19:24:17.000000 django-dynamic-filenames-1.3.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 19:24:30.465863 django-dynamic-filenames-1.3.1/django_dynamic_filenames.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3882 2022-10-05 19:24:30.000000 django-dynamic-filenames-1.3.1/django_dynamic_filenames.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      626 2022-10-05 19:24:30.000000 django-dynamic-filenames-1.3.1/django_dynamic_filenames.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-05 19:24:30.000000 django-dynamic-filenames-1.3.1/django_dynamic_filenames.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-10-05 19:24:30.000000 django-dynamic-filenames-1.3.1/django_dynamic_filenames.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-10-05 19:24:30.000000 django-dynamic-filenames-1.3.1/django_dynamic_filenames.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4401 2022-10-05 19:24:17.000000 django-dynamic-filenames-1.3.1/dynamic_filenames.py
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-10-05 19:24:17.000000 django-dynamic-filenames-1.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1786 2022-10-05 19:24:30.465863 django-dynamic-filenames-1.3.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)      163 2022-10-05 19:24:17.000000 django-dynamic-filenames-1.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 19:24:30.465863 django-dynamic-filenames-1.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-05 19:24:17.000000 django-dynamic-filenames-1.3.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8208 2022-10-05 19:24:17.000000 django-dynamic-filenames-1.3.1/tests/test_dynamic_filenames.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 19:24:30.465863 django-dynamic-filenames-1.3.1/tests/testapp/
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-10-05 19:24:17.000000 django-dynamic-filenames-1.3.1/tests/testapp/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-05 19:24:17.000000 django-dynamic-filenames-1.3.1/tests/testapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      327 2022-10-05 19:24:17.000000 django-dynamic-filenames-1.3.1/tests/testapp/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     3072 2022-10-05 19:24:17.000000 django-dynamic-filenames-1.3.1/tests/testapp/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)      749 2022-10-05 19:24:17.000000 django-dynamic-filenames-1.3.1/tests/testapp/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)      391 2022-10-05 19:24:17.000000 django-dynamic-filenames-1.3.1/tests/testapp/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:38:57.778305 django-dynamic-filenames-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-22 06:38:40.000000 django-dynamic-filenames-1.3.2/.bandit
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:38:57.778305 django-dynamic-filenames-1.3.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-22 06:38:40.000000 django-dynamic-filenames-1.3.2/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-22 06:38:40.000000 django-dynamic-filenames-1.3.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:38:57.778305 django-dynamic-filenames-1.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-22 06:38:40.000000 django-dynamic-filenames-1.3.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-22 06:38:40.000000 django-dynamic-filenames-1.3.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-22 06:38:40.000000 django-dynamic-filenames-1.3.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-22 06:38:40.000000 django-dynamic-filenames-1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-06-22 06:38:57.778305 django-dynamic-filenames-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-06-22 06:38:40.000000 django-dynamic-filenames-1.3.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:38:57.778305 django-dynamic-filenames-1.3.2/django_dynamic_filenames.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-06-22 06:38:57.000000 django-dynamic-filenames-1.3.2/django_dynamic_filenames.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-22 06:38:57.000000 django-dynamic-filenames-1.3.2/django_dynamic_filenames.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 06:38:57.000000 django-dynamic-filenames-1.3.2/django_dynamic_filenames.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-22 06:38:57.000000 django-dynamic-filenames-1.3.2/django_dynamic_filenames.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-22 06:38:57.000000 django-dynamic-filenames-1.3.2/django_dynamic_filenames.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-06-22 06:38:40.000000 django-dynamic-filenames-1.3.2/dynamic_filenames.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-22 06:38:40.000000 django-dynamic-filenames-1.3.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-06-22 06:38:57.782306 django-dynamic-filenames-1.3.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      163 2023-06-22 06:38:40.000000 django-dynamic-filenames-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:38:57.778305 django-dynamic-filenames-1.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 06:38:40.000000 django-dynamic-filenames-1.3.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-06-22 06:38:40.000000 django-dynamic-filenames-1.3.2/tests/test_dynamic_filenames.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:38:57.778305 django-dynamic-filenames-1.3.2/tests/testapp/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-22 06:38:40.000000 django-dynamic-filenames-1.3.2/tests/testapp/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 06:38:40.000000 django-dynamic-filenames-1.3.2/tests/testapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-22 06:38:40.000000 django-dynamic-filenames-1.3.2/tests/testapp/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-06-22 06:38:40.000000 django-dynamic-filenames-1.3.2/tests/testapp/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-22 06:38:40.000000 django-dynamic-filenames-1.3.2/tests/testapp/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-22 06:38:40.000000 django-dynamic-filenames-1.3.2/tests/testapp/wsgi.py
```

### Comparing `django-dynamic-filenames-1.3.1/.github/workflows/ci.yml` & `django-dynamic-filenames-1.3.2/.github/workflows/ci.yml`

 * *Files 20% similar despite different names*

```diff
@@ -53,24 +53,58 @@
       - lint
     strategy:
       matrix:
         python-version:
           - "3.8"
           - "3.9"
           - "3.10"
+          - "3.11"
         django-version:
-          - "3.2a"
-          - "4.0a"
+          - "3.2"
+          - "4.1"
+          - "4.2"
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
     - name: Upgrade Python setuptools
       run: python -m pip install --upgrade pip setuptools wheel codecov
     - run: python setup.py develop
     - name: Install Django ${{ matrix.django-version }}
-      run: python -m pip install "django~=${{ matrix.django-version }}"
+      run: python -m pip install "django~=${{ matrix.django-version }}.0"
     - name: Run tests
       run: python setup.py test
     - run: codecov
+
+  analyze:
+    name: CodeQL Analyze
+    needs: [ pytest ]
+    runs-on: ubuntu-latest
+    permissions:
+      actions: read
+      contents: read
+      security-events: write
+
+    strategy:
+      fail-fast: false
+      matrix:
+        language: [ python ]
+
+    steps:
+      - name: Checkout
+        uses: actions/checkout@v3
+
+      - name: Initialize CodeQL
+        uses: github/codeql-action/init@v2
+        with:
+          languages: ${{ matrix.language }}
+          queries: +security-and-quality
+
+      - name: Autobuild
+        uses: github/codeql-action/autobuild@v2
+
+      - name: Perform CodeQL Analysis
+        uses: github/codeql-action/analyze@v2
+        with:
+          category: "/language:${{ matrix.language }}"
```

### Comparing `django-dynamic-filenames-1.3.1/.github/workflows/release.yml` & `django-dynamic-filenames-1.3.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `django-dynamic-filenames-1.3.1/.gitignore` & `django-dynamic-filenames-1.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `django-dynamic-filenames-1.3.1/LICENSE` & `django-dynamic-filenames-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-dynamic-filenames-1.3.1/PKG-INFO` & `django-dynamic-filenames-1.3.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: django-dynamic-filenames
-Version: 1.3.1
+Version: 1.3.2
 Summary: Write advanced filename patterns using the Format String Syntax.
 Home-page: https://github.com/codingjoe/django-dynamic-filenames
 Author: Johannes Maron
 Author-email: johannes@maron.family
 License: MIT License
 Keywords: django,django-storages,file
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/x-rst
 Provides-Extra: slugify
 License-File: LICENSE
 
 ========================
 Django Dynamic Filenames
 ========================
```

### Comparing `django-dynamic-filenames-1.3.1/README.rst` & `django-dynamic-filenames-1.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `django-dynamic-filenames-1.3.1/django_dynamic_filenames.egg-info/PKG-INFO` & `django-dynamic-filenames-1.3.2/django_dynamic_filenames.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: django-dynamic-filenames
-Version: 1.3.1
+Version: 1.3.2
 Summary: Write advanced filename patterns using the Format String Syntax.
 Home-page: https://github.com/codingjoe/django-dynamic-filenames
 Author: Johannes Maron
 Author-email: johannes@maron.family
 License: MIT License
 Keywords: django,django-storages,file
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/x-rst
 Provides-Extra: slugify
 License-File: LICENSE
 
 ========================
 Django Dynamic Filenames
 ========================
```

### Comparing `django-dynamic-filenames-1.3.1/django_dynamic_filenames.egg-info/SOURCES.txt` & `django-dynamic-filenames-1.3.2/django_dynamic_filenames.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-dynamic-filenames-1.3.1/dynamic_filenames.py` & `django-dynamic-filenames-1.3.2/dynamic_filenames.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import base64
 import os
 import re
 import uuid
 from string import Formatter
+
 from django.utils.text import slugify
 
 
 class SlugFormatter(Formatter):
     format_spec_pattern = re.compile(r"(\.\d+)?([\d\w]+)?")
 
     def format_field(self, value, format_spec):
```

### Comparing `django-dynamic-filenames-1.3.1/setup.cfg` & `django-dynamic-filenames-1.3.2/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -12,21 +12,23 @@
 	Development Status :: 5 - Production/Stable
 	Environment :: Web Environment
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Framework :: Django
 	Framework :: Django :: 3.2
-	Framework :: Django :: 4.0
+	Framework :: Django :: 4.1
+	Framework :: Django :: 4.2
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 keywords = 
 	django
 	django-storages
 	file
 
 [options]
 install_requires =
```

### Comparing `django-dynamic-filenames-1.3.1/tests/test_dynamic_filenames.py` & `django-dynamic-filenames-1.3.2/tests/test_dynamic_filenames.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-filenames-1.3.1/tests/testapp/settings.py` & `django-dynamic-filenames-1.3.2/tests/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-filenames-1.3.1/tests/testapp/urls.py` & `django-dynamic-filenames-1.3.2/tests/testapp/urls.py`

 * *Files identical despite different names*

