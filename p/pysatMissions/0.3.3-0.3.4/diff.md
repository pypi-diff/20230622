# Comparing `tmp/pysatMissions-0.3.3.tar.gz` & `tmp/pysatMissions-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysatMissions-0.3.3.tar", last modified: Tue Sep  6 18:06:14 2022, max compression
+gzip compressed data, was "pysatMissions-0.3.4.tar", last modified: Thu Jun 22 14:07:13 2023, max compression
```

## Comparing `pysatMissions-0.3.3.tar` & `pysatMissions-0.3.4.tar`

### file list

```diff
@@ -1,35 +1,34 @@
-drwxr-xr-x   0 jklenzin   (502) staff       (20)        0 2022-09-06 18:06:14.417843 pysatMissions-0.3.3/
--rw-r--r--   0 jklenzin   (502) staff       (20)     2736 2022-09-06 18:02:20.000000 pysatMissions-0.3.3/CHANGELOG.md
--rw-r--r--   0 jklenzin   (502) staff       (20)     3358 2022-09-06 18:03:25.000000 pysatMissions-0.3.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 jklenzin   (502) staff       (20)     5434 2022-09-06 18:05:00.000000 pysatMissions-0.3.3/CONTRIBUTING.md
--rw-r--r--   0 jklenzin   (502) staff       (20)     1513 2022-09-06 18:03:15.000000 pysatMissions-0.3.3/LICENSE
--rw-r--r--   0 jklenzin   (502) staff       (20)      237 2020-06-18 14:38:11.000000 pysatMissions-0.3.3/MANIFEST.in
--rw-r--r--   0 jklenzin   (502) staff       (20)     5062 2022-09-06 18:06:14.418020 pysatMissions-0.3.3/PKG-INFO
--rw-r--r--   0 jklenzin   (502) staff       (20)     3987 2022-09-06 18:05:00.000000 pysatMissions-0.3.3/README.md
-drwxr-xr-x   0 jklenzin   (502) staff       (20)        0 2022-09-06 18:06:14.400728 pysatMissions-0.3.3/pysatMissions/
--rw-r--r--   0 jklenzin   (502) staff       (20)      755 2022-09-06 17:43:34.000000 pysatMissions-0.3.3/pysatMissions/__init__.py
-drwxr-xr-x   0 jklenzin   (502) staff       (20)        0 2022-09-06 18:06:14.415300 pysatMissions-0.3.3/pysatMissions/instruments/
--rw-r--r--   0 jklenzin   (502) staff       (20)      274 2022-05-13 20:42:30.000000 pysatMissions-0.3.3/pysatMissions/instruments/__init__.py
--rw-r--r--   0 jklenzin   (502) staff       (20)      224 2022-05-13 20:42:30.000000 pysatMissions-0.3.3/pysatMissions/instruments/_core.py
-drwxr-xr-x   0 jklenzin   (502) staff       (20)        0 2022-09-06 18:06:14.415930 pysatMissions-0.3.3/pysatMissions/instruments/methods/
--rw-r--r--   0 jklenzin   (502) staff       (20)      128 2022-05-13 20:42:30.000000 pysatMissions-0.3.3/pysatMissions/instruments/methods/__init__.py
--rw-r--r--   0 jklenzin   (502) staff       (20)     4242 2022-05-13 20:42:45.000000 pysatMissions-0.3.3/pysatMissions/instruments/methods/orbits.py
--rw-r--r--   0 jklenzin   (502) staff       (20)     9939 2022-09-06 17:43:34.000000 pysatMissions-0.3.3/pysatMissions/instruments/missions_ephem.py
--rw-r--r--   0 jklenzin   (502) staff       (20)    14445 2022-09-06 17:43:34.000000 pysatMissions-0.3.3/pysatMissions/instruments/missions_sgp4.py
-drwxr-xr-x   0 jklenzin   (502) staff       (20)        0 2022-09-06 18:06:14.416958 pysatMissions-0.3.3/pysatMissions/methods/
--rw-r--r--   0 jklenzin   (502) staff       (20)      207 2022-05-13 20:42:30.000000 pysatMissions-0.3.3/pysatMissions/methods/__init__.py
--rw-r--r--   0 jklenzin   (502) staff       (20)     5363 2022-09-06 17:43:34.000000 pysatMissions-0.3.3/pysatMissions/methods/magcoord.py
--rw-r--r--   0 jklenzin   (502) staff       (20)     7322 2022-09-06 17:43:34.000000 pysatMissions-0.3.3/pysatMissions/methods/spacecraft.py
-drwxr-xr-x   0 jklenzin   (502) staff       (20)        0 2022-09-06 18:06:14.417580 pysatMissions-0.3.3/pysatMissions/utils/
--rw-r--r--   0 jklenzin   (502) staff       (20)      108 2022-09-06 17:43:34.000000 pysatMissions-0.3.3/pysatMissions/utils/__init__.py
--rw-r--r--   0 jklenzin   (502) staff       (20)     1465 2022-09-06 17:43:34.000000 pysatMissions-0.3.3/pysatMissions/utils/_core.py
--rw-r--r--   0 jklenzin   (502) staff       (20)        6 2022-09-06 18:05:24.000000 pysatMissions-0.3.3/pysatMissions/version.txt
-drwxr-xr-x   0 jklenzin   (502) staff       (20)        0 2022-09-06 18:06:14.414097 pysatMissions-0.3.3/pysatMissions.egg-info/
--rw-r--r--   0 jklenzin   (502) staff       (20)     5062 2022-09-06 18:06:14.000000 pysatMissions-0.3.3/pysatMissions.egg-info/PKG-INFO
--rw-r--r--   0 jklenzin   (502) staff       (20)      783 2022-09-06 18:06:14.000000 pysatMissions-0.3.3/pysatMissions.egg-info/SOURCES.txt
--rw-r--r--   0 jklenzin   (502) staff       (20)        1 2022-09-06 18:06:14.000000 pysatMissions-0.3.3/pysatMissions.egg-info/dependency_links.txt
--rw-r--r--   0 jklenzin   (502) staff       (20)        1 2020-09-30 15:19:59.000000 pysatMissions-0.3.3/pysatMissions.egg-info/not-zip-safe
--rw-r--r--   0 jklenzin   (502) staff       (20)       94 2022-09-06 18:06:14.000000 pysatMissions-0.3.3/pysatMissions.egg-info/requires.txt
--rw-r--r--   0 jklenzin   (502) staff       (20)       14 2022-09-06 18:06:14.000000 pysatMissions-0.3.3/pysatMissions.egg-info/top_level.txt
--rw-r--r--   0 jklenzin   (502) staff       (20)     1625 2022-09-06 18:06:14.418823 pysatMissions-0.3.3/setup.cfg
--rw-r--r--   0 jklenzin   (502) staff       (20)      317 2022-05-13 20:42:30.000000 pysatMissions-0.3.3/setup.py
+drwxr-xr-x   0 jklenzin   (502) staff       (20)        0 2023-06-22 14:07:13.578247 pysatMissions-0.3.4/
+-rw-r--r--   0 jklenzin   (502) staff       (20)     3384 2023-06-13 17:48:23.000000 pysatMissions-0.3.4/CHANGELOG.md
+-rw-r--r--   0 jklenzin   (502) staff       (20)     3358 2022-09-06 18:03:25.000000 pysatMissions-0.3.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jklenzin   (502) staff       (20)     5927 2023-06-13 17:47:40.000000 pysatMissions-0.3.4/CONTRIBUTING.md
+-rw-r--r--   0 jklenzin   (502) staff       (20)     1513 2022-09-06 18:03:15.000000 pysatMissions-0.3.4/LICENSE
+-rw-r--r--   0 jklenzin   (502) staff       (20)      237 2022-10-26 17:19:38.000000 pysatMissions-0.3.4/MANIFEST.in
+-rw-r--r--   0 jklenzin   (502) staff       (20)     7071 2023-06-22 14:07:13.578404 pysatMissions-0.3.4/PKG-INFO
+-rw-r--r--   0 jklenzin   (502) staff       (20)     4035 2023-06-13 17:47:40.000000 pysatMissions-0.3.4/README.md
+-rw-r--r--   0 jklenzin   (502) staff       (20)     1896 2023-06-16 20:30:54.000000 pysatMissions-0.3.4/pyproject.toml
+drwxr-xr-x   0 jklenzin   (502) staff       (20)        0 2023-06-22 14:07:13.568467 pysatMissions-0.3.4/pysatMissions/
+-rw-r--r--   0 jklenzin   (502) staff       (20)      648 2023-06-07 18:23:29.000000 pysatMissions-0.3.4/pysatMissions/__init__.py
+drwxr-xr-x   0 jklenzin   (502) staff       (20)        0 2023-06-22 14:07:13.573879 pysatMissions-0.3.4/pysatMissions/instruments/
+-rw-r--r--   0 jklenzin   (502) staff       (20)      351 2023-06-13 17:47:40.000000 pysatMissions-0.3.4/pysatMissions/instruments/__init__.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)      224 2022-12-19 15:24:06.000000 pysatMissions-0.3.4/pysatMissions/instruments/_core.py
+drwxr-xr-x   0 jklenzin   (502) staff       (20)        0 2023-06-22 14:07:13.575158 pysatMissions-0.3.4/pysatMissions/instruments/methods/
+-rw-r--r--   0 jklenzin   (502) staff       (20)      128 2022-05-13 20:42:30.000000 pysatMissions-0.3.4/pysatMissions/instruments/methods/__init__.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)     4242 2022-05-13 20:42:45.000000 pysatMissions-0.3.4/pysatMissions/instruments/methods/orbits.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)     9939 2022-09-06 17:43:34.000000 pysatMissions-0.3.4/pysatMissions/instruments/missions_ephem.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)    14445 2023-03-06 18:39:51.000000 pysatMissions-0.3.4/pysatMissions/instruments/missions_sgp4.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)    12970 2023-06-15 14:28:17.000000 pysatMissions-0.3.4/pysatMissions/instruments/missions_skyfield.py
+drwxr-xr-x   0 jklenzin   (502) staff       (20)        0 2023-06-22 14:07:13.576811 pysatMissions-0.3.4/pysatMissions/methods/
+-rw-r--r--   0 jklenzin   (502) staff       (20)      207 2022-05-13 20:42:30.000000 pysatMissions-0.3.4/pysatMissions/methods/__init__.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)     5363 2022-09-06 17:43:34.000000 pysatMissions-0.3.4/pysatMissions/methods/magcoord.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)     7866 2023-06-07 18:23:29.000000 pysatMissions-0.3.4/pysatMissions/methods/spacecraft.py
+drwxr-xr-x   0 jklenzin   (502) staff       (20)        0 2023-06-22 14:07:13.577832 pysatMissions-0.3.4/pysatMissions/utils/
+-rw-r--r--   0 jklenzin   (502) staff       (20)      108 2022-09-06 17:43:34.000000 pysatMissions-0.3.4/pysatMissions/utils/__init__.py
+-rw-r--r--   0 jklenzin   (502) staff       (20)     1465 2022-09-06 17:43:34.000000 pysatMissions-0.3.4/pysatMissions/utils/_core.py
+drwxr-xr-x   0 jklenzin   (502) staff       (20)        0 2023-06-22 14:07:13.570744 pysatMissions-0.3.4/pysatMissions.egg-info/
+-rw-r--r--   0 jklenzin   (502) staff       (20)     7071 2023-06-22 14:07:13.000000 pysatMissions-0.3.4/pysatMissions.egg-info/PKG-INFO
+-rw-r--r--   0 jklenzin   (502) staff       (20)      774 2023-06-22 14:07:13.000000 pysatMissions-0.3.4/pysatMissions.egg-info/SOURCES.txt
+-rw-r--r--   0 jklenzin   (502) staff       (20)        1 2023-06-22 14:07:13.000000 pysatMissions-0.3.4/pysatMissions.egg-info/dependency_links.txt
+-rw-r--r--   0 jklenzin   (502) staff       (20)      294 2023-06-22 14:07:13.000000 pysatMissions-0.3.4/pysatMissions.egg-info/requires.txt
+-rw-r--r--   0 jklenzin   (502) staff       (20)       14 2023-06-22 14:07:13.000000 pysatMissions-0.3.4/pysatMissions.egg-info/top_level.txt
+-rw-r--r--   0 jklenzin   (502) staff       (20)       97 2023-06-22 14:07:13.578873 pysatMissions-0.3.4/setup.cfg
```

### Comparing `pysatMissions-0.3.3/CHANGELOG.md` & `pysatMissions-0.3.4/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,28 @@
 # Change Log
 All notable changes to this project will be documented in this file.
 This project adheres to [Semantic Versioning](https://semver.org/).
 
+## [0.3.4] - 2023-06-22
+* Add support for skyfield propagation
+* Maintenance
+  * Update pytest syntax
+  * Update Github Actions versions
+  * Add manual GitHub Actions tests for pysat RC
+  * Add manual GitHub Actions tests for optional dependencies
+  * Add manual GitHub Actions tests for pysatMissions RC
+  * Remove optional dependencies in readthedocs requirements
+  * Add tests for NEP 29 testing
+  * Add tests for Mac OS
+  * Deprecate `calculate_ecef_velocity` method
+  * Use pyproject.toml to handle metadata / installation
+  * Update GitHub Actions workflow standards
+* Testing
+  * Include checks on sc coordinate transformation calculations
+
 ## [0.3.3] - 2022-09-06
 * Documentation Updates
 
 ## [0.3.2] - 2022-09-06
 * Make fortran dependencies optional installs
   * aacgmv2
   * apexpy
```

### Comparing `pysatMissions-0.3.3/CODE_OF_CONDUCT.md` & `pysatMissions-0.3.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pysatMissions-0.3.3/CONTRIBUTING.md` & `pysatMissions-0.3.4/CONTRIBUTING.md`

 * *Files 5% similar despite different names*

```diff
@@ -9,36 +9,41 @@
 [pysat GitHub Repository.](https://github.com/pysat/pysat) Development meetings
 are generally held fortnightly.
 
 Short version
 -------------
 
 * Submit bug reports and feature requests at [GitHub](https://github.com/pysat/pysatMissions/issues)
+
 * Make pull requests to the ``develop`` branch
 
 Bug reports
 -----------
 
 When [reporting a bug](https://github.com/pysat/pysatMissions/issues) please
 include:
 
 * Your operating system name and version
+
 * Any details about your local setup that might be helpful in troubleshooting
+
 * Detailed steps to reproduce the bug
 
 Feature requests and feedback
 -----------------------------
 
 The best way to send feedback is to file an issue at
 [GitHub](https://github.com/pysat/pysatMissions/issues).
 
 If you are proposing a feature:
 
 * Explain in detail how it would work.
+
 * Keep the scope as narrow as possible, to make it easier to implement.
+
 * Remember that this is a volunteer-driven project, and that code contributions
   are welcome :)
 
 Development
 -----------
 
 To set up `pysatMissions` for local development:
@@ -51,70 +56,85 @@
    ```
 
 3. Create a branch for local development:
    ```
    git checkout -b name-of-your-bugfix-or-feature
    ```
 
-   Now you can make your changes locally. Tests for new instruments are
-   performed automatically.  Tests for custom functions should be added to
-   the appropriately named file in ``pysatMissions/tests``.  If no test
-   file exists, then you should create one.  This testing uses pytest, which
-   will run tests on any python file in the test directory that starts with
-   ``test_``.
+   Now you can make your changes locally.
+
+   Tests for new instruments are performed automatically.  Tests for custom
+   functions should be added to the appropriately named file in
+   ``pysatMissions/tests``.  If no test file exists, then you should create
+   one.  This testing uses pytest, which will run tests on any python file in
+   the test directory that starts with ``test_`` as well.
 
 4. When you're done making changes, run all the checks to ensure that nothing
    is broken on your local system:
    ```
    pytest -vs
    ```
 
-5. Update/add documentation (in ``docs``), if relevant
+   5. You should also check for flake8 style compliance:
 
-6. Add your name to the .zenodo.json file as an author
+      ```
+      flake8 . --count --select=D,E,F,H,W --show-source --statistics
+      ```
+
+      Note that pysat uses the `flake-docstrings` and `hacking` packages to ensure
+      standards in docstring formatting.
+
+
+   6. Update/add documentation (in ``docs``), if relevant
+
+   7. Add your name to the .zenodo.json file as an author
+
+   8. Commit your changes:
+      ```
+      git add .
+      git commit -m "AAA: Brief description of your changes"
+      ```
+      Where AAA is a standard shorthand for the type of change (eg, BUG or DOC).
+      `pysat` follows the [numpy development workflow](https://numpy.org/doc/stable/dev/development_workflow.html),
+      see the discussion there for a full list of this shorthand notation.  
+
+   9. Once you are happy with the local changes, push to GitHub:
+      ```
+      git push origin name-of-your-bugfix-or-feature
+      ```
+      Note that each push will trigger the Continuous Integration workflow.
+
+   10. Submit a pull request through the GitHub website. Pull requests should be
+       made to the ``develop`` branch.  Note that automated tests will be run on
+       GitHub Actions, but these must be initialized by a member of the pysat team.
 
-7. Commit your changes:
-   ```
-   git add .
-   git commit -m "AAA: Brief description of your changes"
-   ```
-   Where AAA is a standard shorthand for the type of change (eg, BUG or DOC).
-   `pysat` follows the [numpy development workflow](https://numpy.org/doc/stable/dev/development_workflow.html),
-   see the discussion there for a full list of this shorthand notation.  
-
-8. Once you are happy with the local changes, push to Github:
-   ```
-   git push origin name-of-your-bugfix-or-feature
-   ```
-   Note that each push will trigger the Continuous Integration workflow.
-
-9. Submit a pull request through the GitHub website. Pull requests should be
-   made to the ``develop`` branch.
 
 Pull Request Guidelines
 -----------------------
 
 If you need some code review or feedback while you're developing the code, just
 make a pull request. Pull requests should be made to the ``develop`` branch.
 
 For merging, you should:
 
 1. Include an example for use
 2. Add a note to ``CHANGELOG.md`` about the changes
-3. Ensure that all checks passed (current checks include GitHub Actions
-   and Coveralls)
+3. Update the author list in ``zenodo.json`` if applicable
+4. Ensure that all checks passed (current checks include Github Actions and
+   Coveralls)
 
 If you don't have all the necessary Python versions available locally or
 have trouble building all the testing environments, you can rely on
-the project's Continuous Integration (CI) service to run the tests for each change you add in the pull
+GitHub Actions to run the tests for each change you add in the pull
 request. Because testing here will delay tests by other developers,
 please ensure that the code passes all tests on your local system first.
 
+
 Project Style Guidelines
-^^^^^^^^^^^^^^^^^^^^^^^^
+------------------------
 
 In general, pysat follows PEP8 and numpydoc guidelines.  Pytest runs the unit
 and integration tests, flake8 checks for style, and sphinx-build performs
 documentation tests.  However, there are certain additional style elements that
 have been settled on to ensure the project maintains a consistent coding style.
 These include:
```

### Comparing `pysatMissions-0.3.3/LICENSE` & `pysatMissions-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pysatMissions-0.3.3/PKG-INFO` & `pysatMissions-0.3.4/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,7 @@
-Metadata-Version: 2.1
-Name: pysatMissions
-Version: 0.3.3
-Summary: 'Mission Planning toolkit for pysat'
-Home-page: https://github.com/pysat/pysatMissions
-Author: Jeff Klenzing, Russell Stoneback
-Author-email: pysat.developers@gmail.com
-Keywords: pysat,ionosphere,cubesat,satellite,ephemeris,orbit,mission-planning
-Classifier: Development Status :: 3 - Alpha
-Classifier: Topic :: Scientific/Engineering :: Physics
-Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-Provides-Extra: aacgmv2
-Provides-Extra: apexpy
-Provides-Extra: OMMBV
-License-File: LICENSE
-
 <div align="left">
         <img height="0" width="0px">
         <img width="20%" src="https://raw.githubusercontent.com/pysat/pysatMissions/main/docs/figures/missions-draft-logo.jpeg" alt="pysat Missions logo - the python snakes dreaming of a spaceship" title="pysatMissions"</img>
 </div>
 
 # pysatMissions
 [![Documentation Status](https://readthedocs.org/projects/pysatmissions/badge/?version=latest)](https://pysatmissions.readthedocs.io/en/latest/?badge=latest)
@@ -59,14 +32,15 @@
 Python 3.8+.  
 
 | Common modules | Community modules | Optional modules |
 | -------------- | ----------------- | ---------------- |
 | numpy          | pysat>=3.0.4      | aacgmv2          |
 | pandas         | pyEphem           | apexpy           |
 |                | sgp4>=2.7         | OMMBV            |
+|                | skyfield          |                  |
 
 
 One way to install is through pip.  Just type
 
 ```
 pip install pysatMissions
 ```
@@ -79,15 +53,15 @@
 ```
 
 Change directories into the repository folder and run the setup.py file.  For
 a local install use the "--user" flag after "install".
 
 ```
 cd pysatMissions/
-python setup.py install
+pip install .
 ```
 
 Note: pre-1.0.0 version
 -----------------------
 pysatMissions is currently in an initial development phase and requires pysat
 3.0.4.
```

### Comparing `pysatMissions-0.3.3/pysatMissions/instruments/methods/orbits.py` & `pysatMissions-0.3.4/pysatMissions/instruments/methods/orbits.py`

 * *Files identical despite different names*

### Comparing `pysatMissions-0.3.3/pysatMissions/instruments/missions_ephem.py` & `pysatMissions-0.3.4/pysatMissions/instruments/missions_ephem.py`

 * *Files identical despite different names*

### Comparing `pysatMissions-0.3.3/pysatMissions/instruments/missions_sgp4.py` & `pysatMissions-0.3.4/pysatMissions/instruments/missions_sgp4.py`

 * *Files identical despite different names*

### Comparing `pysatMissions-0.3.3/pysatMissions/methods/magcoord.py` & `pysatMissions-0.3.4/pysatMissions/methods/magcoord.py`

 * *Files identical despite different names*

### Comparing `pysatMissions-0.3.3/pysatMissions/methods/spacecraft.py` & `pysatMissions-0.3.4/pysatMissions/methods/spacecraft.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Default routines for projecting values onto vectors for pysat instruments."""
 
 import numpy as np
+import warnings
 
 
 def add_ram_pointing_sc_attitude_vectors(inst):
     """Add attitude vectors for spacecraft assuming ram pointing.
 
     Presumes spacecraft is pointed along the velocity vector (x), z is
     generally nadir pointing (positive towards Earth), and y completes the
@@ -88,14 +89,19 @@
 
     return
 
 
 def calculate_ecef_velocity(inst):
     """Calculate spacecraft velocity in ECEF frame.
 
+    .. deprecated:: 0.4.0
+      This function is no longer needed with the deprecation of `missions_ephem`.
+      Better calculations are available through geospacepy and skyfield.
+      `calculate_ecef_velocity` will be removed in versions 0.5.0+
+
     Presumes that the spacecraft velocity in ECEF is in
     the input instrument object as position_ecef_*. Uses a symmetric
     difference to calculate the velocity thus endpoints will be
     set to NaN. Routine should be run using pysat data padding feature
     to create valid end points.
 
     Parameters
@@ -107,14 +113,19 @@
     -------
     None
         Modifies pysat.Instrument object in place to include ECEF velocity
         using naming scheme velocity_ecef_* (*=x,y,z)
 
     """
 
+    warnings.warn(' '.join(("`calculate_ecef_velocity` has been deprecated and",
+                            "will be removed in pysatMissions 0.5.0+.",
+                            "Use `geospacepy` or `skyfield` instead.")),
+                  DeprecationWarning, stacklevel=2)
+
     def get_vel_from_pos(x):
         vel = (x.values[2:] - x.values[0:-2]) / 2.
         return vel
 
     vel_x = get_vel_from_pos(inst['position_ecef_x'])
     vel_y = get_vel_from_pos(inst['position_ecef_y'])
     vel_z = get_vel_from_pos(inst['position_ecef_z'])
```

### Comparing `pysatMissions-0.3.3/pysatMissions/utils/_core.py` & `pysatMissions-0.3.4/pysatMissions/utils/_core.py`

 * *Files identical despite different names*

### Comparing `pysatMissions-0.3.3/pysatMissions.egg-info/SOURCES.txt` & `pysatMissions-0.3.4/pysatMissions.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 CHANGELOG.md
 CODE_OF_CONDUCT.md
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 setup.cfg
-setup.py
 pysatMissions/__init__.py
-pysatMissions/version.txt
 pysatMissions.egg-info/PKG-INFO
 pysatMissions.egg-info/SOURCES.txt
 pysatMissions.egg-info/dependency_links.txt
-pysatMissions.egg-info/not-zip-safe
 pysatMissions.egg-info/requires.txt
 pysatMissions.egg-info/top_level.txt
 pysatMissions/instruments/__init__.py
 pysatMissions/instruments/_core.py
 pysatMissions/instruments/missions_ephem.py
 pysatMissions/instruments/missions_sgp4.py
+pysatMissions/instruments/missions_skyfield.py
 pysatMissions/instruments/methods/__init__.py
 pysatMissions/instruments/methods/orbits.py
 pysatMissions/methods/__init__.py
 pysatMissions/methods/magcoord.py
 pysatMissions/methods/spacecraft.py
 pysatMissions/utils/__init__.py
 pysatMissions/utils/_core.py
```

