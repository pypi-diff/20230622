# Comparing `tmp/plone.releaser-2.0.0.tar.gz` & `tmp/plone.releaser-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.releaser-2.0.0.tar", last modified: Thu Feb 23 13:30:32 2023, max compression
+gzip compressed data, was "plone.releaser-2.0.1.tar", last modified: Thu Jun 22 19:10:32 2023, max compression
```

## Comparing `plone.releaser-2.0.0.tar` & `plone.releaser-2.0.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-23 13:30:32.141592 plone.releaser-2.0.0/
--rw-r--r--   0 maurits    (501) staff       (20)     3287 2023-02-23 13:30:31.000000 plone.releaser-2.0.0/ADD-A-NEWS-ITEM.rst
--rw-r--r--   0 maurits    (501) staff       (20)     6471 2023-02-23 13:30:31.000000 plone.releaser-2.0.0/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-02-23 13:30:31.000000 plone.releaser-2.0.0/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      109 2023-02-23 13:30:31.000000 plone.releaser-2.0.0/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)     8050 2023-02-23 13:30:32.141711 plone.releaser-2.0.0/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      871 2023-02-23 13:30:31.000000 plone.releaser-2.0.0/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)      108 2023-02-23 13:30:31.000000 plone.releaser-2.0.0/buildout.cfg
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-23 13:30:32.136664 plone.releaser-2.0.0/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-02-23 13:30:31.000000 plone.releaser-2.0.0/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-23 13:30:32.141348 plone.releaser-2.0.0/plone/releaser/
--rw-r--r--   0 maurits    (501) staff       (20)      940 2023-02-23 13:30:31.000000 plone.releaser-2.0.0/plone/releaser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     7359 2023-02-23 13:30:31.000000 plone.releaser-2.0.0/plone/releaser/buildout.py
--rw-r--r--   0 maurits    (501) staff       (20)     8635 2023-02-23 13:30:31.000000 plone.releaser-2.0.0/plone/releaser/changelog.py
--rw-r--r--   0 maurits    (501) staff       (20)      772 2023-02-23 13:30:31.000000 plone.releaser-2.0.0/plone/releaser/db.py
--rw-r--r--   0 maurits    (501) staff       (20)     4618 2023-02-23 13:30:31.000000 plone.releaser-2.0.0/plone/releaser/manage.py
--rw-r--r--   0 maurits    (501) staff       (20)    10900 2023-02-23 13:30:31.000000 plone.releaser-2.0.0/plone/releaser/package.py
--rw-r--r--   0 maurits    (501) staff       (20)      371 2023-02-23 13:30:31.000000 plone.releaser-2.0.0/plone/releaser/pypi.py
--rw-r--r--   0 maurits    (501) staff       (20)     8796 2023-02-23 13:30:31.000000 plone.releaser-2.0.0/plone/releaser/release.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-23 13:30:32.139022 plone.releaser-2.0.0/plone.releaser.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)     8050 2023-02-23 13:30:32.000000 plone.releaser-2.0.0/plone.releaser.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      653 2023-02-23 13:30:32.000000 plone.releaser-2.0.0/plone.releaser.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-02-23 13:30:32.000000 plone.releaser-2.0.0/plone.releaser.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)      706 2023-02-23 13:30:32.000000 plone.releaser-2.0.0/plone.releaser.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-02-23 13:30:32.000000 plone.releaser-2.0.0/plone.releaser.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-02-23 13:30:32.000000 plone.releaser-2.0.0/plone.releaser.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      145 2023-02-23 13:30:32.000000 plone.releaser-2.0.0/plone.releaser.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-02-23 13:30:32.000000 plone.releaser-2.0.0/plone.releaser.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)      920 2023-02-23 13:30:31.000000 plone.releaser-2.0.0/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      215 2023-02-23 13:30:32.142309 plone.releaser-2.0.0/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2556 2023-02-23 13:30:31.000000 plone.releaser-2.0.0/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:10:32.813255 plone.releaser-2.0.1/
+-rw-r--r--   0 maurits    (501) staff       (20)     3287 2023-06-22 19:10:32.000000 plone.releaser-2.0.1/ADD-A-NEWS-ITEM.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     6795 2023-06-22 19:10:32.000000 plone.releaser-2.0.1/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-06-22 19:10:32.000000 plone.releaser-2.0.1/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      109 2023-06-22 19:10:32.000000 plone.releaser-2.0.1/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)     8216 2023-06-22 19:10:32.813485 plone.releaser-2.0.1/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      713 2023-06-22 19:10:32.000000 plone.releaser-2.0.1/README.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      108 2023-06-22 19:10:32.000000 plone.releaser-2.0.1/buildout.cfg
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:10:32.807848 plone.releaser-2.0.1/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-06-22 19:10:32.000000 plone.releaser-2.0.1/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:10:32.812904 plone.releaser-2.0.1/plone/releaser/
+-rw-r--r--   0 maurits    (501) staff       (20)      940 2023-06-22 19:10:32.000000 plone.releaser-2.0.1/plone/releaser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7359 2023-06-22 19:10:32.000000 plone.releaser-2.0.1/plone/releaser/buildout.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8635 2023-06-22 19:10:32.000000 plone.releaser-2.0.1/plone/releaser/changelog.py
+-rw-r--r--   0 maurits    (501) staff       (20)      772 2023-06-22 19:10:32.000000 plone.releaser-2.0.1/plone/releaser/db.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4618 2023-06-22 19:10:32.000000 plone.releaser-2.0.1/plone/releaser/manage.py
+-rw-r--r--   0 maurits    (501) staff       (20)    10900 2023-06-22 19:10:32.000000 plone.releaser-2.0.1/plone/releaser/package.py
+-rw-r--r--   0 maurits    (501) staff       (20)      701 2023-06-22 19:10:32.000000 plone.releaser-2.0.1/plone/releaser/pypi.py
+-rw-r--r--   0 maurits    (501) staff       (20)     9378 2023-06-22 19:10:32.000000 plone.releaser-2.0.1/plone/releaser/release.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:10:32.810051 plone.releaser-2.0.1/plone.releaser.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)     8216 2023-06-22 19:10:32.000000 plone.releaser-2.0.1/plone.releaser.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      653 2023-06-22 19:10:32.000000 plone.releaser-2.0.1/plone.releaser.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-06-22 19:10:32.000000 plone.releaser-2.0.1/plone.releaser.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      706 2023-06-22 19:10:32.000000 plone.releaser-2.0.1/plone.releaser.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-06-22 19:10:32.000000 plone.releaser-2.0.1/plone.releaser.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-06-22 19:10:32.000000 plone.releaser-2.0.1/plone.releaser.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      145 2023-06-22 19:10:32.000000 plone.releaser-2.0.1/plone.releaser.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-06-22 19:10:32.000000 plone.releaser-2.0.1/plone.releaser.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      920 2023-06-22 19:10:32.000000 plone.releaser-2.0.1/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      215 2023-06-22 19:10:32.814025 plone.releaser-2.0.1/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2556 2023-06-22 19:10:32.000000 plone.releaser-2.0.1/setup.py
```

### Comparing `plone.releaser-2.0.0/ADD-A-NEWS-ITEM.rst` & `plone.releaser-2.0.1/ADD-A-NEWS-ITEM.rst`

 * *Files identical despite different names*

### Comparing `plone.releaser-2.0.0/CHANGES.rst` & `plone.releaser-2.0.1/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,26 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.0.1 (2023-06-22)
+------------------
+
+Bug fixes:
+
+
+- Allow disabling PyPI rights check, as this does not know how to check organisations.
+  Set env variable ``PLONE_RELEASER_CHECK_PYPI_ACCESS=0`` if you want to disable it.
+  Also, we do not check PyPI if the user is `__token__`, so using an API token.
+  [maurits] (#50)
+
+
 2.0.0 (2023-02-23)
 ------------------
 
 Breaking changes:
 
 
 - Require Python 3.8+.
```

### Comparing `plone.releaser-2.0.0/PKG-INFO` & `plone.releaser-2.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.releaser
-Version: 2.0.0
+Version: 2.0.1
 Summary: Plone release management utilities
 Home-page: https://github.com/plone/plone.releaser
 Author: Eric Steele
 Author-email: eric@esteele.net
 License: GPL
 Keywords: plone release
 Classifier: Development Status :: 5 - Production/Stable
@@ -59,32 +59,36 @@
 
   $ bin/manage changelog
 
 Check checkout::
 
   $ bin/manage check-checkout
 
-Append Jenkins build number to package version::
-
-  $ bin/append-jenkins-build-number-to-package-version
-
-Set package version::
-
-  $ bin/set-package-version
-
 Changelog
 =========
 
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.0.1 (2023-06-22)
+------------------
+
+Bug fixes:
+
+
+- Allow disabling PyPI rights check, as this does not know how to check organisations.
+  Set env variable ``PLONE_RELEASER_CHECK_PYPI_ACCESS=0`` if you want to disable it.
+  Also, we do not check PyPI if the user is `__token__`, so using an API token.
+  [maurits] (#50)
+
+
 2.0.0 (2023-02-23)
 ------------------
 
 Breaking changes:
 
 
 - Require Python 3.8+.
```

### Comparing `plone.releaser-2.0.0/README.rst` & `plone.releaser-2.0.1/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -38,15 +38,7 @@
 Changelog::
 
   $ bin/manage changelog
 
 Check checkout::
 
   $ bin/manage check-checkout
-
-Append Jenkins build number to package version::
-
-  $ bin/append-jenkins-build-number-to-package-version
-
-Set package version::
-
-  $ bin/set-package-version
```

### Comparing `plone.releaser-2.0.0/plone/releaser/__init__.py` & `plone.releaser-2.0.1/plone/releaser/__init__.py`

 * *Files identical despite different names*

### Comparing `plone.releaser-2.0.0/plone/releaser/buildout.py` & `plone.releaser-2.0.1/plone/releaser/buildout.py`

 * *Files identical despite different names*

### Comparing `plone.releaser-2.0.0/plone/releaser/changelog.py` & `plone.releaser-2.0.1/plone/releaser/changelog.py`

 * *Files identical despite different names*

### Comparing `plone.releaser-2.0.0/plone/releaser/db.py` & `plone.releaser-2.0.1/plone/releaser/db.py`

 * *Files identical despite different names*

### Comparing `plone.releaser-2.0.0/plone/releaser/manage.py` & `plone.releaser-2.0.1/plone/releaser/manage.py`

 * *Files identical despite different names*

### Comparing `plone.releaser-2.0.0/plone/releaser/package.py` & `plone.releaser-2.0.1/plone/releaser/package.py`

 * *Files identical despite different names*

### Comparing `plone.releaser-2.0.0/plone/releaser/release.py` & `plone.releaser-2.0.1/plone/releaser/release.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,15 +167,31 @@
         sys.exit()
     print("Committing changes.")
     print(g.add(history_file))
     print(g.commit(message=message))
 
 
 def check_pypi_access(data):
-    pypi_user = pypi.PypiConfig().config.get("pypi", "username")
+    env_var = "PLONE_RELEASER_CHECK_PYPI_ACCESS"
+    try:
+        if int(os.getenv(env_var, 1)) == 0:
+            print(
+                f"{env_var} variable set to zero: not checking pypi release rights."
+            )
+            return
+    except (TypeError, ValueError, AttributeError):
+        print(
+            f"ERROR: could not parse {env_var} env var. Ignoring it."
+        )
+
+    section = os.getenv("TWINE_REPOSITORY", "pypi")
+    pypi_user = pypi.PypiConfig().config.get(section, "username")
+    if pypi_user == "__token__":
+        print("Using token for PyPI upload: cannot check if you have release rights.")
+        return
     if not can_user_release_package_to_pypi(pypi_user, data["name"]):
         msg = "User {0} does not have pypi release rights to {1}. Continue?"
         if not ask(msg.format(pypi_user, data["name"]), default=False):
             sys.exit()
 
 
 def update_core(data, branch=None):
@@ -221,15 +237,15 @@
             msg = f"Ok to push coredev {branch}?"
         if ask(msg, default=True):
             print("Pushing changes to server.")
             g.push()
 
 
 def update_other_core_branches(data):
-    CORE_BRANCHES = ["5.2", "6.0"]
+    CORE_BRANCHES = ["5.2", "6.0", "6.1"]
     package_name = data["name"]
     root_path = os.path.join(os.getcwd(), "../../")
 
     def _get_current_core_branch():
         g = git.Repo(root_path)
         return g.head.reference.name
```

### Comparing `plone.releaser-2.0.0/plone.releaser.egg-info/PKG-INFO` & `plone.releaser-2.0.1/plone.releaser.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.releaser
-Version: 2.0.0
+Version: 2.0.1
 Summary: Plone release management utilities
 Home-page: https://github.com/plone/plone.releaser
 Author: Eric Steele
 Author-email: eric@esteele.net
 License: GPL
 Keywords: plone release
 Classifier: Development Status :: 5 - Production/Stable
@@ -59,32 +59,36 @@
 
   $ bin/manage changelog
 
 Check checkout::
 
   $ bin/manage check-checkout
 
-Append Jenkins build number to package version::
-
-  $ bin/append-jenkins-build-number-to-package-version
-
-Set package version::
-
-  $ bin/set-package-version
-
 Changelog
 =========
 
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.0.1 (2023-06-22)
+------------------
+
+Bug fixes:
+
+
+- Allow disabling PyPI rights check, as this does not know how to check organisations.
+  Set env variable ``PLONE_RELEASER_CHECK_PYPI_ACCESS=0`` if you want to disable it.
+  Also, we do not check PyPI if the user is `__token__`, so using an API token.
+  [maurits] (#50)
+
+
 2.0.0 (2023-02-23)
 ------------------
 
 Breaking changes:
 
 
 - Require Python 3.8+.
```

### Comparing `plone.releaser-2.0.0/plone.releaser.egg-info/SOURCES.txt` & `plone.releaser-2.0.1/plone.releaser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.releaser-2.0.0/plone.releaser.egg-info/entry_points.txt` & `plone.releaser-2.0.1/plone.releaser.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `plone.releaser-2.0.0/pyproject.toml` & `plone.releaser-2.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone.releaser-2.0.0/setup.py` & `plone.releaser-2.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "2.0.0"
+version = "2.0.1"
 
 long_description = "{}\n{}".format(
     open("README.rst").read(), open("CHANGES.rst").read()
 )
 
 setup(
     name="plone.releaser",
```

