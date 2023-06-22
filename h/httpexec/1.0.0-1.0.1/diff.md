# Comparing `tmp/httpexec-1.0.0.tar.gz` & `tmp/httpexec-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "httpexec-1.0.0.tar", last modified: Thu May 25 16:35:26 2023, max compression
+gzip compressed data, was "httpexec-1.0.1.tar", last modified: Thu Jun 22 04:46:52 2023, max compression
```

## Comparing `httpexec-1.0.0.tar` & `httpexec-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:35:26.404433 httpexec-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-25 16:34:40.000000 httpexec-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13231 2023-05-25 16:35:26.404433 httpexec-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10905 2023-05-25 16:34:40.000000 httpexec-1.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-25 16:34:40.000000 httpexec-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 16:35:26.404433 httpexec-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:35:26.404433 httpexec-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:35:26.404433 httpexec-1.0.0/src/httpexec/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-25 16:34:40.000000 httpexec-1.0.0/src/httpexec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-25 16:34:40.000000 httpexec-1.0.0/src/httpexec/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-05-25 16:34:40.000000 httpexec-1.0.0/src/httpexec/asgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:35:26.404433 httpexec-1.0.0/src/httpexec/etc/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-25 16:34:40.000000 httpexec-1.0.0/src/httpexec/etc/defaults.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:35:26.404433 httpexec-1.0.0/src/httpexec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13231 2023-05-25 16:35:26.000000 httpexec-1.0.0/src/httpexec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-25 16:35:26.000000 httpexec-1.0.0/src/httpexec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 16:35:26.000000 httpexec-1.0.0/src/httpexec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-25 16:35:26.000000 httpexec-1.0.0/src/httpexec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-25 16:35:26.000000 httpexec-1.0.0/src/httpexec.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 04:46:52.054640 httpexec-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-22 04:46:25.000000 httpexec-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13810 2023-06-22 04:46:52.054640 httpexec-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11484 2023-06-22 04:46:25.000000 httpexec-1.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-06-22 04:46:25.000000 httpexec-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 04:46:52.054640 httpexec-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 04:46:52.054640 httpexec-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 04:46:52.054640 httpexec-1.0.1/src/httpexec/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-22 04:46:25.000000 httpexec-1.0.1/src/httpexec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-22 04:46:25.000000 httpexec-1.0.1/src/httpexec/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-06-22 04:46:25.000000 httpexec-1.0.1/src/httpexec/asgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 04:46:52.054640 httpexec-1.0.1/src/httpexec/etc/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-22 04:46:25.000000 httpexec-1.0.1/src/httpexec/etc/defaults.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 04:46:52.054640 httpexec-1.0.1/src/httpexec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13810 2023-06-22 04:46:52.000000 httpexec-1.0.1/src/httpexec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-22 04:46:52.000000 httpexec-1.0.1/src/httpexec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 04:46:52.000000 httpexec-1.0.1/src/httpexec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-22 04:46:52.000000 httpexec-1.0.1/src/httpexec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-22 04:46:52.000000 httpexec-1.0.1/src/httpexec.egg-info/top_level.txt
```

### Comparing `httpexec-1.0.0/LICENSE` & `httpexec-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `httpexec-1.0.0/PKG-INFO` & `httpexec-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httpexec
-Version: 1.0.0
+Version: 1.0.1
 Summary: Execute CLI commands via a REST API.
 Author-email: Michael Klatt <mdklatt@alumni.ou.edu>
 License: The MIT License (MIT)
         
         Copyright (c) 2022-2023, Michael Klatt
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -58,16 +58,16 @@
 |pypi|
 |tests|
 
 *httpexec* is an `Asynchronous Server Gateway Interface`_ (ASGI) application
 that allows remote clients to execute CLI commands on the local host via a
 REST API. An `ASGI-capable server`_ is also required.
 
-**There are critical security concerns when using this application.** See the
-`Security`_ section.
+**There are critical security considerations when using this application.** See
+the `Security`_ section.
 
 
 .. image:: docs/httpexec.png
   :alt: httpexec System Architecture
 
 
 ========
@@ -154,14 +154,25 @@
 Install the application, its runtime dependencies, and the `Hypercorn`_ web
 server:
 
 .. code-block:: console
 
     $ python -m pip install httpexec "hypercorn>=0.14.3,<1"
 
+Pinned Dependencies
++++++++++++++++++++
+
+Production applications should pin their dependencies to exact versions to
+avoid unexpected breaking changes. The downside of this is that it makes it
+more difficult to receive critical updates. This application relies on
+`Semantic Versioning`_ for its own dependencies to minimize breaking changes
+while allowing for routine updates (see *pyproject.toml*). Users should use
+their packaage manager to pin this package and its dependencies to exact
+versions in a production environment.
+
 
 Configuration
 -------------
 
 User-configurable options can be set using a `TOML`_ config file or an
 environment variable. Environment variable names must be prefixed with
 ``HTTPEXEC_``, *e.g.* ``HTTPEXEC_EXEC_ROOT`` sets ``EXEC_ROOT``. Environment
@@ -362,11 +373,12 @@
 .. _GitHub Actions: https://github.com/mdklatt/httpexec/actions/workflows/test.yml
 .. _Hypercorn: https://pgjones.gitlab.io/hypercorn
 .. _LXC: https://linuxcontainers.org/
 .. _MIT License: https://choosealicense.com/licenses/mit
 .. _OpenAPI: https://www.openapis.org/
 .. _PyPI: https://pypi.org/project/httpexec/
 .. _Python logging: https://docs.python.org/3/howto/logging.html
+.. _Semantic Versioning: https://semver.org/
 .. _Sphinx: https://www.sphinx-doc.org/en/master/
 .. _TOML: https://toml.io/en/
 .. _user-defined bridge network: https://docs.docker.com/network/network-tutorial-standalone/#use-user-defined-bridge-networks
 .. _wheel: https://peps.python.org/pep-0491/
```

### Comparing `httpexec-1.0.0/README.rst` & `httpexec-1.0.1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 |pypi|
 |tests|
 
 *httpexec* is an `Asynchronous Server Gateway Interface`_ (ASGI) application
 that allows remote clients to execute CLI commands on the local host via a
 REST API. An `ASGI-capable server`_ is also required.
 
-**There are critical security concerns when using this application.** See the
-`Security`_ section.
+**There are critical security considerations when using this application.** See
+the `Security`_ section.
 
 
 .. image:: docs/httpexec.png
   :alt: httpexec System Architecture
 
 
 ========
@@ -106,14 +106,25 @@
 Install the application, its runtime dependencies, and the `Hypercorn`_ web
 server:
 
 .. code-block:: console
 
     $ python -m pip install httpexec "hypercorn>=0.14.3,<1"
 
+Pinned Dependencies
++++++++++++++++++++
+
+Production applications should pin their dependencies to exact versions to
+avoid unexpected breaking changes. The downside of this is that it makes it
+more difficult to receive critical updates. This application relies on
+`Semantic Versioning`_ for its own dependencies to minimize breaking changes
+while allowing for routine updates (see *pyproject.toml*). Users should use
+their packaage manager to pin this package and its dependencies to exact
+versions in a production environment.
+
 
 Configuration
 -------------
 
 User-configurable options can be set using a `TOML`_ config file or an
 environment variable. Environment variable names must be prefixed with
 ``HTTPEXEC_``, *e.g.* ``HTTPEXEC_EXEC_ROOT`` sets ``EXEC_ROOT``. Environment
@@ -314,11 +325,12 @@
 .. _GitHub Actions: https://github.com/mdklatt/httpexec/actions/workflows/test.yml
 .. _Hypercorn: https://pgjones.gitlab.io/hypercorn
 .. _LXC: https://linuxcontainers.org/
 .. _MIT License: https://choosealicense.com/licenses/mit
 .. _OpenAPI: https://www.openapis.org/
 .. _PyPI: https://pypi.org/project/httpexec/
 .. _Python logging: https://docs.python.org/3/howto/logging.html
+.. _Semantic Versioning: https://semver.org/
 .. _Sphinx: https://www.sphinx-doc.org/en/master/
 .. _TOML: https://toml.io/en/
 .. _user-defined bridge network: https://docs.docker.com/network/network-tutorial-standalone/#use-user-defined-bridge-networks
 .. _wheel: https://peps.python.org/pep-0491/
```

### Comparing `httpexec-1.0.0/pyproject.toml` & `httpexec-1.0.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -19,16 +19,19 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
     "Topic :: Software Development :: User Interfaces",
 ]
 requires-python = ">=3.9"
 dependencies = [
+    # Relying on Semantic Versioning instead of pinned versions to minimize
+    # breaking changes while making it easier to recieve critical updates.
+    # Add a rquirements.txt file for production deployments.
     "quart>=0.17.0,<1",
-    "toml>=0.10.2,<1",
+    "tomli>=2.0.1,<3; python_version<'3.11'"
 ]
 dynamic = ["version", "readme"]
 
 [project.urls]
 "Homepage" = "https://github.com/mdklatt/httpexec"
 "Repository" = "https://github.com/mdklatt/httpexec"
```

### Comparing `httpexec-1.0.0/src/httpexec/__version__.py` & `httpexec-1.0.1/src/httpexec/__version__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 internal code changes that do not affect the API. Development versions are
 incomplete states of a release .
 
 Version 0.x should be considered a development version with an unstable API,
 and backwards compatibility is not guaranteed for minor versions.
 
 """
-__version__ = "1.0.0"
+__version__ = "1.0.1"
```

### Comparing `httpexec-1.0.0/src/httpexec/asgi.py` & `httpexec-1.0.1/src/httpexec/asgi.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,18 @@
 from asyncio.subprocess import create_subprocess_exec, DEVNULL, PIPE
 from base64 import a85decode, a85encode, b64decode, b64encode
 from http.client import NOT_FOUND
 from importlib import resources
 from os import environ
 from pathlib import Path
 from quart import Quart, jsonify, request
-from toml import loads  # TODO: tomllib in Python 3.11+
+try:
+    import tomllib  # Python 3.11+
+except ModuleNotFoundError:
+    import tomli as tomllib
 from typing import Sequence
 
 
 __all__ = "app",
 
 
 app = Quart(__name__)
@@ -39,21 +42,21 @@
     # This should not need to be marked async, but doing so causes no harm,
     # and, anecdotally, eliminates some reliability issues when `httpexec` is
     # running inside a Docker container that is being accessed by another
     # Docker container. Circumstantially, this is related to the use of the
     # `quart.utils.run_sync()` adapter to run a synchronous function.
     # See <https://github.com/mdklatt/httpexec/issues/1>.
     defaults = resources.files("httpexec").joinpath("etc/defaults.toml")
-    config = loads(defaults.read_text())
+    config = tomllib.loads(defaults.read_text())
     try:
         path = Path(environ["HTTPEXEC_CONFIG_PATH"])
     except KeyError:
         pass
     else:
-        config |= loads(path.read_text())
+        config |= tomllib.loads(path.read_text())
     app.config.from_mapping(config)
     app.config.from_prefixed_env("HTTPEXEC")
     app.logger.setLevel(app.config.get("LOGGING_LEVEL"))
     return
 
 
 @app.route("/<path:command>", methods=["POST"])
```

### Comparing `httpexec-1.0.0/src/httpexec.egg-info/PKG-INFO` & `httpexec-1.0.1/src/httpexec.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httpexec
-Version: 1.0.0
+Version: 1.0.1
 Summary: Execute CLI commands via a REST API.
 Author-email: Michael Klatt <mdklatt@alumni.ou.edu>
 License: The MIT License (MIT)
         
         Copyright (c) 2022-2023, Michael Klatt
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -58,16 +58,16 @@
 |pypi|
 |tests|
 
 *httpexec* is an `Asynchronous Server Gateway Interface`_ (ASGI) application
 that allows remote clients to execute CLI commands on the local host via a
 REST API. An `ASGI-capable server`_ is also required.
 
-**There are critical security concerns when using this application.** See the
-`Security`_ section.
+**There are critical security considerations when using this application.** See
+the `Security`_ section.
 
 
 .. image:: docs/httpexec.png
   :alt: httpexec System Architecture
 
 
 ========
@@ -154,14 +154,25 @@
 Install the application, its runtime dependencies, and the `Hypercorn`_ web
 server:
 
 .. code-block:: console
 
     $ python -m pip install httpexec "hypercorn>=0.14.3,<1"
 
+Pinned Dependencies
++++++++++++++++++++
+
+Production applications should pin their dependencies to exact versions to
+avoid unexpected breaking changes. The downside of this is that it makes it
+more difficult to receive critical updates. This application relies on
+`Semantic Versioning`_ for its own dependencies to minimize breaking changes
+while allowing for routine updates (see *pyproject.toml*). Users should use
+their packaage manager to pin this package and its dependencies to exact
+versions in a production environment.
+
 
 Configuration
 -------------
 
 User-configurable options can be set using a `TOML`_ config file or an
 environment variable. Environment variable names must be prefixed with
 ``HTTPEXEC_``, *e.g.* ``HTTPEXEC_EXEC_ROOT`` sets ``EXEC_ROOT``. Environment
@@ -362,11 +373,12 @@
 .. _GitHub Actions: https://github.com/mdklatt/httpexec/actions/workflows/test.yml
 .. _Hypercorn: https://pgjones.gitlab.io/hypercorn
 .. _LXC: https://linuxcontainers.org/
 .. _MIT License: https://choosealicense.com/licenses/mit
 .. _OpenAPI: https://www.openapis.org/
 .. _PyPI: https://pypi.org/project/httpexec/
 .. _Python logging: https://docs.python.org/3/howto/logging.html
+.. _Semantic Versioning: https://semver.org/
 .. _Sphinx: https://www.sphinx-doc.org/en/master/
 .. _TOML: https://toml.io/en/
 .. _user-defined bridge network: https://docs.docker.com/network/network-tutorial-standalone/#use-user-defined-bridge-networks
 .. _wheel: https://peps.python.org/pep-0491/
```

