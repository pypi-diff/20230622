# Comparing `tmp/ProjectAssessment-0.3.1.tar.gz` & `tmp/projectassessment-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ProjectAssessment-0.3.1.tar", last modified: Wed Jun 14 20:53:27 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `ProjectAssessment-0.3.1.tar` & `projectassessment-0.3.2.tar`

### file list

```diff
@@ -1,17 +1,15 @@
-drwxr-xr-x   0 tazz       (501) staff       (20)        0 2023-06-14 20:53:27.735282 ProjectAssessment-0.3.1/
--rw-r--r--   0 tazz       (501) staff       (20)     1066 2022-06-04 12:11:30.000000 ProjectAssessment-0.3.1/LICENSE
--rw-r--r--   0 tazz       (501) staff       (20)      831 2023-06-14 20:53:27.735189 ProjectAssessment-0.3.1/PKG-INFO
-drwxr-xr-x   0 tazz       (501) staff       (20)        0 2023-06-14 20:53:27.734521 ProjectAssessment-0.3.1/ProjectAssessment/
--rw-r--r--   0 tazz       (501) staff       (20)       99 2022-06-29 18:35:17.000000 ProjectAssessment-0.3.1/ProjectAssessment/MakeTable.py
--rw-r--r--   0 tazz       (501) staff       (20)     4659 2023-06-14 19:59:55.000000 ProjectAssessment-0.3.1/ProjectAssessment/Marginal.py
--rw-r--r--   0 tazz       (501) staff       (20)    21282 2023-06-14 19:59:55.000000 ProjectAssessment-0.3.1/ProjectAssessment/Solver.py
--rw-r--r--   0 tazz       (501) staff       (20)       83 2023-06-14 20:49:14.000000 ProjectAssessment-0.3.1/ProjectAssessment/__init__.py
-drwxr-xr-x   0 tazz       (501) staff       (20)        0 2023-06-14 20:53:27.735042 ProjectAssessment-0.3.1/ProjectAssessment.egg-info/
--rw-r--r--   0 tazz       (501) staff       (20)      831 2023-06-14 20:53:27.000000 ProjectAssessment-0.3.1/ProjectAssessment.egg-info/PKG-INFO
--rw-r--r--   0 tazz       (501) staff       (20)      349 2023-06-14 20:53:27.000000 ProjectAssessment-0.3.1/ProjectAssessment.egg-info/SOURCES.txt
--rw-r--r--   0 tazz       (501) staff       (20)        1 2023-06-14 20:53:27.000000 ProjectAssessment-0.3.1/ProjectAssessment.egg-info/dependency_links.txt
--rw-r--r--   0 tazz       (501) staff       (20)       60 2023-06-14 20:53:27.000000 ProjectAssessment-0.3.1/ProjectAssessment.egg-info/requires.txt
--rw-r--r--   0 tazz       (501) staff       (20)       18 2023-06-14 20:53:27.000000 ProjectAssessment-0.3.1/ProjectAssessment.egg-info/top_level.txt
--rw-r--r--   0 tazz       (501) staff       (20)     6770 2023-06-14 19:59:55.000000 ProjectAssessment-0.3.1/README.md
--rw-r--r--   0 tazz       (501) staff       (20)       38 2023-06-14 20:53:27.735317 ProjectAssessment-0.3.1/setup.cfg
--rw-r--r--   0 tazz       (501) staff       (20)     1082 2023-06-14 20:49:28.000000 ProjectAssessment-0.3.1/setup.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 projectassessment-0.3.2/.gitattributes
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 projectassessment-0.3.2/.pylintrc
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 projectassessment-0.3.2/SECURITY.md
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 projectassessment-0.3.2/data.csv
+-rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 projectassessment-0.3.2/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 projectassessment-0.3.2/.vscode/settings.json
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 projectassessment-0.3.2/src/ProjectAssessment/MakeTable.py
+-rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 projectassessment-0.3.2/src/ProjectAssessment/Marginal.py
+-rw-r--r--   0        0        0    21282 2020-02-02 00:00:00.000000 projectassessment-0.3.2/src/ProjectAssessment/Solver.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 projectassessment-0.3.2/src/ProjectAssessment/__init__.py
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 projectassessment-0.3.2/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 projectassessment-0.3.2/LICENSE
+-rw-r--r--   0        0        0     6770 2020-02-02 00:00:00.000000 projectassessment-0.3.2/README.md
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 projectassessment-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     7862 2020-02-02 00:00:00.000000 projectassessment-0.3.2/PKG-INFO
```

### Comparing `ProjectAssessment-0.3.1/LICENSE` & `projectassessment-0.3.2/LICENSE`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Ben Smith
+Copyright (c) 2023 Ben Smith
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `ProjectAssessment-0.3.1/ProjectAssessment/Marginal.py` & `projectassessment-0.3.2/src/ProjectAssessment/Marginal.py`

 * *Files identical despite different names*

### Comparing `ProjectAssessment-0.3.1/ProjectAssessment/Solver.py` & `projectassessment-0.3.2/src/ProjectAssessment/Solver.py`

 * *Files identical despite different names*

### Comparing `ProjectAssessment-0.3.1/README.md` & `projectassessment-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `ProjectAssessment-0.3.1/setup.py` & `projectassessment-0.3.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,40 @@
-from distutils.core import setup
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
 
-setup(
-    name='ProjectAssessment',
-    version='0.3.1',
-    packages=['ProjectAssessment',],
-    python_requires='>3.7.0',
-    license='MIT',
-    install_requires=[
-        'numpy>=1.21.0',
-        'pandas>=1.3.0',
-        'tqdm',
-        'numba>=0.54.0',
-        'scipy>=1.4.0',
-    ],
-    author='Ben Smith',
-    author_email='bosmith@unomaha.edu',
-    classifiers=[
-    'Development Status :: 4 - Beta',
-    'Intended Audience :: Science/Research',
-    'License :: OSI Approved :: MIT License',
-    'Programming Language :: Python :: 3.10',
-    'Programming Language :: Python :: 3.9',
-    'Programming Language :: Python :: 3.8',
-    'Programming Language :: Python :: 3.7',
-    ],
-    keywords = ['Assessment', 'Projects', 'Statistics', 'Education', 'Bootstrap'],
-    url = 'https://github.com/tazzben/project-based-assessment',
-    download_url = 'https://github.com/tazzben/project-based-assessment/archive/v0.3.1.tar.gz',
-    description = 'Package to compute the Project-Based Assessment estimates of student and rubric proficiency.',
-)
+[project]
+name = "ProjectAssessment"
+version = "0.3.2"
+description = "Package to compute the Project-Based Assessment estimates of student and rubric proficiency."
+license = "MIT"
+authors = [
+  { name="Ben Smith", email="bosmith@unomaha.edu" },
+]
+maintainers = [
+  { name="Ben Smith", email="bosmith@unomaha.edu" },
+]
+readme = "README.md"
+homepage = "https://github.com/tazzben/project-based-assessment"
+repository = "https://github.com/tazzben/project-based-assessment"
+keywords = ["Assessment", "Projects", "Statistics", "Education", "Bootstrap"]
+classifiers = [
+    "Development Status :: 5 - Production/Stable",
+    "Intended Audience :: Science/Research",
+    "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.8",
+]
+requires-python = ">=3.8"
+dependencies = [
+    "numpy>=1.21.0",
+    "pandas>=1.3.0",
+    "tqdm>=4.26.0",
+    "numba>=0.54.0",
+    "scipy>=1.4.0",
+]
+
+[project.urls]
+"Homepage" = "https://github.com/tazzben/project-based-assessment"
+"Bug Tracker" = "https://github.com/tazzben/project-based-assessment/issues"
```

