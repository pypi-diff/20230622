# Comparing `tmp/flufl.lock-7.1.1.tar.gz` & `tmp/flufl_lock-8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flufl.lock-7.1.1.tar", last modified: Mon Sep  5 00:26:23 2022, max compression
+gzip compressed data, was "flufl_lock-8.0.tar", last modified: Thu Jun 22 04:17:39 2023, max compression
```

## Comparing `flufl.lock-7.1.1.tar` & `flufl_lock-8.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-rw-rw-   0 root         (0) root         (0)      558 2022-09-05 00:25:49.266757 flufl.lock-7.1.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)     2131 2022-09-05 00:25:49.266757 flufl.lock-7.1.1/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     2961 2022-09-05 00:25:49.266757 flufl.lock-7.1.1/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     7107 2022-09-05 00:25:49.266757 flufl.lock-7.1.1/docs/NEWS.rst
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-05 00:25:49.266757 flufl.lock-7.1.1/docs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      273 2022-09-05 00:25:49.266757 flufl.lock-7.1.1/docs/_static/lock-dark.svg
--rw-rw-rw-   0 root         (0) root         (0)      337 2022-09-05 00:25:49.266757 flufl.lock-7.1.1/docs/_static/lock-light.svg
--rw-rw-rw-   0 root         (0) root         (0)     1634 2022-09-05 00:25:49.266757 flufl.lock-7.1.1/docs/_static/logo-dark.png
--rw-rw-rw-   0 root         (0) root         (0)     1273 2022-09-05 00:25:49.266757 flufl.lock-7.1.1/docs/_static/logo-dark.svg
--rw-rw-rw-   0 root         (0) root         (0)     1302 2022-09-05 00:25:49.266757 flufl.lock-7.1.1/docs/_static/logo-light.png
--rw-rw-rw-   0 root         (0) root         (0)     1308 2022-09-05 00:25:49.266757 flufl.lock-7.1.1/docs/_static/logo-light.svg
--rw-rw-rw-   0 root         (0) root         (0)      405 2022-09-05 00:25:49.266757 flufl.lock-7.1.1/docs/apiref.rst
--rw-rw-rw-   0 root         (0) root         (0)     6792 2022-09-05 00:25:49.266757 flufl.lock-7.1.1/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     1834 2022-09-05 00:25:49.266757 flufl.lock-7.1.1/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     9350 2022-09-05 00:25:49.267757 flufl.lock-7.1.1/docs/theory.rst
--rw-rw-rw-   0 root         (0) root         (0)     9188 2022-09-05 00:25:49.267757 flufl.lock-7.1.1/docs/using.rst
--rw-rw-rw-   0 root         (0) root         (0)     3072 2022-09-05 00:25:49.267757 flufl.lock-7.1.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      453 2022-09-05 00:25:49.268757 flufl.lock-7.1.1/src/flufl/lock/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    25499 2022-09-05 00:25:49.268757 flufl.lock-7.1.1/src/flufl/lock/_lockfile.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-05 00:25:49.268757 flufl.lock-7.1.1/src/flufl/lock/py.typed
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-05 00:25:49.268757 flufl.lock-7.1.1/test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      296 2022-09-05 00:25:49.268757 flufl.lock-7.1.1/test/test_api.py
--rw-rw-rw-   0 root         (0) root         (0)    16021 2022-09-05 00:25:49.268757 flufl.lock-7.1.1/test/test_lock.py
--rw-rw-rw-   0 root         (0) root         (0)      914 2022-09-05 00:25:49.268757 flufl.lock-7.1.1/tox.ini
--rw-------   0 runner    (1000) runner    (1000)     3231 2022-09-05 00:26:23.808209 flufl.lock-7.1.1/PKG-INFO
+-rw-r--r--   0        0        0      558 2023-06-22 04:17:13.047805 flufl_lock-8.0/LICENSE
+-rw-r--r--   0        0        0     2131 2023-06-22 04:17:13.047805 flufl_lock-8.0/README.rst
+-rw-r--r--   0        0        0     2961 2023-06-22 04:17:13.048805 flufl_lock-8.0/conftest.py
+-rw-r--r--   0        0        0     7447 2023-06-22 04:17:13.048805 flufl_lock-8.0/docs/NEWS.rst
+-rw-r--r--   0        0        0        0 2023-06-22 04:17:13.072805 flufl_lock-8.0/docs/__init__.py
+-rw-r--r--   0        0        0      273 2023-06-22 04:17:13.048805 flufl_lock-8.0/docs/_static/lock-dark.svg
+-rw-r--r--   0        0        0      337 2023-06-22 04:17:13.048805 flufl_lock-8.0/docs/_static/lock-light.svg
+-rw-r--r--   0        0        0     1634 2023-06-22 04:17:13.048805 flufl_lock-8.0/docs/_static/logo-dark.png
+-rw-r--r--   0        0        0     1273 2023-06-22 04:17:13.048805 flufl_lock-8.0/docs/_static/logo-dark.svg
+-rw-r--r--   0        0        0     1302 2023-06-22 04:17:13.048805 flufl_lock-8.0/docs/_static/logo-light.png
+-rw-r--r--   0        0        0     1308 2023-06-22 04:17:13.048805 flufl_lock-8.0/docs/_static/logo-light.svg
+-rw-r--r--   0        0        0      405 2023-06-22 04:17:13.048805 flufl_lock-8.0/docs/apiref.rst
+-rw-r--r--   0        0        0     6814 2023-06-22 04:17:13.048805 flufl_lock-8.0/docs/conf.py
+-rw-r--r--   0        0        0     1834 2023-06-22 04:17:13.048805 flufl_lock-8.0/docs/index.rst
+-rw-r--r--   0        0        0     9350 2023-06-22 04:17:13.048805 flufl_lock-8.0/docs/theory.rst
+-rw-r--r--   0        0        0     9430 2023-06-22 04:17:13.048805 flufl_lock-8.0/docs/using.rst
+-rw-r--r--   0        0        0     3185 2023-06-22 04:17:39.516602 flufl_lock-8.0/pyproject.toml
+-rw-r--r--   0        0        0      451 2023-06-22 04:17:13.049805 flufl_lock-8.0/src/flufl/lock/__init__.py
+-rw-r--r--   0        0        0    25626 2023-06-22 04:17:13.049805 flufl_lock-8.0/src/flufl/lock/_lockfile.py
+-rw-r--r--   0        0        0        0 2023-06-22 04:17:13.072805 flufl_lock-8.0/src/flufl/lock/py.typed
+-rw-r--r--   0        0        0        0 2023-06-22 04:17:13.072805 flufl_lock-8.0/test/__init__.py
+-rw-r--r--   0        0        0      296 2023-06-22 04:17:13.049805 flufl_lock-8.0/test/test_api.py
+-rw-r--r--   0        0        0    19924 2023-06-22 04:17:13.049805 flufl_lock-8.0/test/test_lock.py
+-rw-r--r--   0        0        0      772 2023-06-22 04:17:13.050805 flufl_lock-8.0/tox.ini
+-rw-r--r--   0        0        0     3274 1970-01-01 00:00:00.000000 flufl_lock-8.0/PKG-INFO
```

### Comparing `flufl.lock-7.1.1/LICENSE` & `flufl_lock-8.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright 2004-2022 Barry Warsaw
+Copyright 2004-2023 Barry Warsaw
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `flufl.lock-7.1.1/README.rst` & `flufl_lock-8.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 data.  In a distributed (NFS) environment, you also need to make sure that
 your clocks are properly synchronized.
 
 
 Author
 ======
 
-``flufl.lock`` is Copyright (C) 2007-2022 Barry Warsaw <barry@python.org>
+``flufl.lock`` is Copyright (C) 2007-2023 Barry Warsaw <barry@python.org>
 
 Licensed under the terms of the Apache License Version 2.0.  See the LICENSE
 file for details.
 
 
 Project details
 ===============
```

### Comparing `flufl.lock-7.1.1/conftest.py` & `flufl_lock-8.0/conftest.py`

 * *Files identical despite different names*

### Comparing `flufl.lock-7.1.1/docs/NEWS.rst` & `flufl_lock-8.0/docs/NEWS.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 =====================
 flufl.lock change log
 =====================
 
+8.0 (2023-06-21)
+================
+* Drop Python 3.7 support (GL#34)
+* Added a ``claimfile`` property to ``Lock`` objects (GL#30)
+* Switch to ``pdm-backend`` (GL#33)
+* Use ``ruff`` for linting, since its much faster. (GL#17)
+* Bump dependencies.
+* More GitLab CI integration improvements.
+* Make ``tox.ini`` consistent with flufl defaults.
+
 7.1.1 (2022-09-03)
 ==================
 * Improvements to the GitLab CI integration.
 
 7.1 (2022-08-27)
 ================
 * Add support for Python 3.11.
```

### Comparing `flufl.lock-7.1.1/docs/_static/logo-dark.png` & `flufl_lock-8.0/docs/_static/logo-dark.png`

 * *Files identical despite different names*

### Comparing `flufl.lock-7.1.1/docs/_static/logo-dark.svg` & `flufl_lock-8.0/docs/_static/logo-dark.svg`

 * *Files identical despite different names*

### Comparing `flufl.lock-7.1.1/docs/_static/logo-light.png` & `flufl_lock-8.0/docs/_static/logo-light.png`

 * *Files identical despite different names*

### Comparing `flufl.lock-7.1.1/docs/_static/logo-light.svg` & `flufl_lock-8.0/docs/_static/logo-light.svg`

 * *Files identical despite different names*

### Comparing `flufl.lock-7.1.1/docs/conf.py` & `flufl_lock-8.0/docs/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,30 +15,32 @@
 from datetime import date
 import importlib.metadata
 
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
-#sys.path.append(os.path.abspath('.'))
+sys.path.append(os.path.abspath('.'))
 
 # -- General configuration -----------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be extensions
 # coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
 extensions = [
     'sphinx.ext.autodoc',
     'sphinx.ext.intersphinx',
-    'sphinx_autodoc_typehints',
     ]
 
 intersphinx_mapping = {
     'python': ('https://docs.python.org/', None),
     }
 
+autodoc_typehints = 'both'
+autoclass_content = 'both'
+
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['../../_templates']
 
 # The suffix of source filenames.
 source_suffix = '.rst'
 
 # The encoding of source files.
```

### Comparing `flufl.lock-7.1.1/docs/index.rst` & `flufl_lock-8.0/docs/index.rst`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 You can contact the author via barry@python.org.
 
 
 Copyright
 =========
 
-Copyright (C) 2004-2022 Barry A. Warsaw
+Copyright (C) 2004-2023 Barry A. Warsaw
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `flufl.lock-7.1.1/docs/theory.rst` & `flufl_lock-8.0/docs/theory.rst`

 * *Files identical despite different names*

### Comparing `flufl.lock-7.1.1/docs/using.rst` & `flufl_lock-8.0/docs/using.rst`

 * *Files 3% similar despite different names*

```diff
@@ -312,21 +312,30 @@
 * It cannot appear in the lock's file name (the argument passed to the
   :class:`Lock` constructor)
 
 It may also be helpful to avoid `any reserved characters
 <https://en.wikipedia.org/wiki/Filename#Reserved_characters_and_words>`_ on
 the file systems where you intend to run the code.
 
+You can also get both the lock file and claim file names from the lock object.
+
     >>> lock = Lock(filename, separator='+')
     >>> lock.lock()
     >>> hostname, pid, lockfile = lock.details
     >>> hostname == lock.hostname
     True
     >>> pid == os.getpid()
     True
     >>> lockfile == filename
     True
+    >>> lock.lockfile == lockfile
+    True
+
+The claim file name is also stored in the contents of any acquired lock file.
+
     >>> with open(filename) as fp:
-    ...     claim_file = fp.read().strip()
-    ...     '+' in claim_file
+    ...     claimfile = fp.read().strip()
+    >>> lock.claimfile == claimfile
+    True
+    >>> '+' in claimfile
     True
     >>> lock.unlock()
```

### Comparing `flufl.lock-7.1.1/pyproject.toml` & `flufl_lock-8.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "flufl.lock"
 authors = [
     { name = "Barry Warsaw", email = "barry@python.org" },
 ]
 description = "NFS-safe file locking with timeouts for POSIX and Windows"
 readme = "README.rst"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 keywords = [
     "locking",
     "locks",
     "lock",
 ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
@@ -21,34 +21,32 @@
     "Operating System :: Microsoft :: Windows",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dependencies = [
-    "typing_extensions; python_version<'3.8'",
-    "atpublic>=2.3",
-    "psutil>=5.9.0",
+    "atpublic",
+    "psutil",
 ]
 dynamic = []
-version = "7.1.1"
+version = "8.0"
 
 [project.license]
 text = "Apache-2.0"
 
 [project.urls]
 "Home Page" = "https://flufllock.readthedocs.io"
 Documentation = "https://flufllock.readthedocs.io"
 "Source Code" = "https://gitlab.com/warsaw/flufl.lock.git"
 "Bug Tracker" = "https://gitlab.com/warsaw/flufl.lock/issues"
 
-[project.optional-dependencies]
-
 [tool.pdm.version]
-from = "src/flufl/lock/__init__.py"
+source = "file"
+path = "src/flufl/lock/__init__.py"
 
 [tool.pdm.build]
 includes = [
     "src/flufl",
 ]
 excludes = [
     "**/.mypy_cache",
@@ -65,53 +63,78 @@
     "coverage[toml]",
     "diff-cover",
     "pytest",
     "pytest-cov",
     "sybil",
 ]
 qa = [
-    "flake8",
-    "isort",
-    "mypy",
     "blue",
+    "mypy",
+    "ruff",
 ]
 docs = [
     "sphinx",
-    "sphinx-autodoc-typehints",
     "furo",
 ]
 
 [tool.pytest.ini_options]
 addopts = "--cov=flufl --cov-report=term --cov-report=xml"
 testpaths = "test docs"
 
-[tool.coverage.report]
-fail_under = 100
-show_missing = true
-
 [tool.coverage.run]
 branch = true
 parallel = true
 
+[tool.coverage.report]
+fail_under = 100
+show_missing = true
+
 [tool.coverage.paths]
 source = [
     "flufl/lock",
 ]
 
-[tool.isort]
-include_trailing_comma = true
-known_first_party = "flufl"
-length_sort_straight = true
-lines_after_imports = 2
-lines_between_types = 1
-multi_line_output = 3
-order_by_type = false
-skip = [
-    "conf.py",
-]
+[tool.ruff]
+line-length = 79
+src = [
+    "src",
+]
+select = [
+    "B",
+    "D",
+    "E",
+    "F",
+    "I",
+    "RUF100",
+    "UP",
+    "W",
+]
+ignore = [
+    "D100",
+    "D104",
+]
+
+[tool.ruff.per-file-ignores]
+"src/flufl/lock/_lockfile.py" = [
+    "I001",
+]
+
+[tool.ruff.pydocstyle]
+convention = "pep257"
+
+[tool.ruff.isort]
+classes = [
+    "SEP",
+]
+known-first-party = [
+    "flufl.lock",
+]
+lines-after-imports = 2
+lines-between-types = 1
+order-by-type = true
 
 [tool.mypy]
 mypy_path = "src"
 namespace_packages = true
 disallow_any_generics = true
 disallow_subclassing_any = true
 disallow_untyped_calls = false
@@ -142,10 +165,10 @@
     "sybil.*",
     "psutil",
 ]
 ignore_missing_imports = true
 
 [build-system]
 requires = [
-    "pdm-pep517",
+    "pdm-backend",
 ]
-build-backend = "pdm.pep517.api"
+build-backend = "pdm.backend"
```

### Comparing `flufl.lock-7.1.1/src/flufl/lock/_lockfile.py` & `flufl_lock-8.0/src/flufl/lock/_lockfile.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,26 +7,20 @@
 import logging
 
 from contextlib import suppress
 from datetime import datetime, timedelta
 from enum import Enum
 from logging import NullHandler
 from types import TracebackType
-from typing import cast, List, Optional, Tuple, Type, Union
+from typing import cast, List, Literal, Optional, Tuple, Type, Union
 
 from psutil import pid_exists
 from public import public
 
 
-try:
-    from typing import Literal
-except ImportError:                                 # pragma: nocover
-    from typing_extensions import Literal  # type: ignore
-
-
 Interval = Union[timedelta, int]
 
 # 2020-06-26(bwarsaw): Once Python 3.8 is the minimum, we could annotatey some
 # of these module globals as typing.Final.
 
 
 DEFAULT_LOCK_LIFETIME = timedelta(seconds=15)
@@ -196,15 +190,15 @@
         self._separator = separator
         self._claimfile: str
         self._set_claimfile()
         # For extending the set of NFS errnos that are retried in _read().
         self._retry_errnos: List[int] = []
 
     def __repr__(self) -> str:
-        return '<%s %s [%s: %s] pid=%s at %#xx>' % (
+        return '<{} {} [{}: {}] pid={} at {:#x}>'.format(
             self.__class__.__name__,
             self._lockfile,
             ('locked' if self._is_locked_no_refresh() else 'unlocked'),
             self._lifetime,
             os.getpid(),
             id(self),
         )
@@ -280,17 +274,17 @@
         else:
             self._lifetime = timedelta(seconds=lifetime)
 
     def refresh(
         self,
         lifetime: Optional[Interval] = None,
         *,
-        unconditionally: bool = False
+        unconditionally: bool = False,
     ) -> None:
-        """Refreshes the lifetime of a locked file.
+        """Refresh the lifetime of a locked file.
 
         Use this if you realize that you need to keep a resource locked longer
         than you thought.
 
         :param lifetime: If given, this sets the lock's new lifetime.  It
             represents the number of seconds into the future that the
             lock's lifetime will expire, relative to now, or whenever it is
@@ -302,15 +296,15 @@
             ``unconditionally`` flag is set to True.
         """
         if lifetime is not None:
             # https://github.com/python/mypy/issues/3004
             self.lifetime = lifetime                # type: ignore
         # Do we have the lock?  As a side effect, this refreshes the lock!
         if not self.is_locked and not unconditionally:
-            raise NotLockedError('{}: {}'.format(repr(self), self._read()))
+            raise NotLockedError(f'{self!r}: {self._read()}')
 
     def lock(self, timeout: Optional[Interval] = None) -> None:
         """Acquire the lock.
 
         This blocks until the lock is acquired unless optional timeout is not
         None, in which case a ``TimeOutError`` is raised when the timeout
         expires without lock acquisition.
@@ -327,27 +321,27 @@
         # Make sure the claim file exists, and that its contents are current.
         self._write()
         # XXX This next call can fail with an EPERM.  I have no idea why, but
         # I'm nervous about ignoring it.  It seems to be a very rare
         # occurrence, only happens from cron, and has only(?) been observed on
         # Solaris 2.6.
         self._touch()
-        log.debug('laying claim: {}'.format(self._lockfile))
+        log.debug(f'laying claim: {self._lockfile}')
         # For quieting the logging output.
         loopcount = -1
         while True:
             loopcount += 1
             # Create the hard link from the claim file to the lock file and
             # test for a hard count of exactly 2 links.
             try:
                 os.link(self._claimfile, self._lockfile)
                 # If we got here, we know we got the lock, and never
                 # had it before, so we're done.  Just touch it again for the
                 # fun of it.
-                log.debug('got the lock: {}'.format(self._lockfile))
+                log.debug(f'got the lock: {self._lockfile}')
                 self._touch()
                 break
             except OSError as error:
                 # The link failed for some reason, possibly because someone
                 # else already has the lock (i.e. we got an EEXIST), or for
                 # some other bizarre reason.
                 if error.errno in ERRORS:
@@ -365,21 +359,21 @@
                     # pass the error on up.
                     log.exception('unexpected link')
                     os.unlink(self._claimfile)
                     raise
                 elif self._linkcount != 2:
                     # Somebody's messin' with us!  Log this, and try again
                     # later.  XXX should we raise an exception?
-                    log.error(
-                        'unexpected linkcount: {0:d}'.format(self._linkcount)
-                    )
+                    log.error(f'unexpected linkcount: {self._linkcount:d}')
                 elif self._read() == self._claimfile:
                     # It was us that already had the link.
-                    log.debug('already locked: {}'.format(self._lockfile))
-                    raise AlreadyLockedError('We already had the lock')
+                    log.debug(f'already locked: {self._lockfile}')
+                    raise AlreadyLockedError(
+                        'We already had the lock'
+                    ) from None
                 # Otherwise, someone else has the lock
                 pass
             # We did not acquire the lock, because someone else already has
             # it.  Have we timed out in our quest for the lock?
             if timeout_time is not None and timeout_time < datetime.now():
                 os.unlink(self._claimfile)
                 log.error('timed out')
@@ -395,29 +389,32 @@
                     # Yes, so break the lock.
                     log.error('lifetime has expired, breaking')
                     self._break()
             # Okay, someone else has the lock, our claim hasn't timed out yet,
             # and the expected lock lifetime hasn't expired yet either.  So
             # let's wait a while for the owner of the lock to give it up.
             elif not loopcount % 100:
-                log.debug('waiting for claim: {}'.format(self._lockfile))
+                log.debug(f'waiting for claim: {self._lockfile}')
             self._sleep()
 
     # 2020-06-27(bwarsaw): `unconditionally` should really be a keyword-only
     # argument, but those didn't exist when this library was originally
     # written, and changing that now would be a needless backward incompatible
     # API break.
     def unlock(self, *, unconditionally: bool = False) -> None:
         """Release the lock.
 
         :param unconditionally: When False (the default), a ``NotLockedError``
             is raised if this is called on an unlocked lock.
         :raises NotLockedError: if we don't own the lock, either because of
             unbalanced unlock calls, or because the lock was stolen out from
             under us, unless optional ``unconditionally`` is True.
+
+        Note that successfully unlocking the lock also unlinks the claim file,
+        even if it is already unlocked and ``unconditionally`` is True.
         """
         is_locked = self.is_locked
         if not is_locked and not unconditionally:
             raise NotLockedError('Already unlocked')
         # If we owned the lock, remove the lockfile, relinquishing the lock.
         if is_locked:
             try:
@@ -427,15 +424,15 @@
                     raise
         # Remove our claim file.
         try:
             os.unlink(self._claimfile)
         except OSError as error:
             if error.errno not in ERRORS:
                 raise
-        log.debug('unlocked: {}'.format(self._lockfile))
+        log.debug(f'unlocked: {self._lockfile}')
 
     def _is_locked_no_refresh(self) -> bool:
         """Don't refresh the lock, just return the status."""
         # XXX Can the link count ever be > 2?
         if self._linkcount != 2:
             return False
         return self._read() == self._claimfile
@@ -512,25 +509,30 @@
         return datetime.fromtimestamp(os.stat(self._lockfile).st_mtime)
 
     @property
     def lockfile(self) -> str:
         """Return the lock file name."""
         return self._lockfile
 
+    @property
+    def claimfile(self) -> str:
+        """Return the claim file name."""
+        return self._claimfile
+
     def _read(self) -> Optional[str]:
         """Read the contents of our lock file.
 
         :return: The contents of the lock file or None if the lock file does
             not exist.
         """
         while True:
             try:
                 with open(self._lockfile) as fp:
                     return fp.read()
-            except EnvironmentError as error:
+            except OSError as error:
                 if error.errno in self._retry_errnos:
                     self._sleep()
                 elif error.errno not in ERRORS:
                     raise
                 else:
                     return None
 
@@ -583,15 +585,15 @@
         # contents have the details expected of any lock file.  If not, then
         # this probably isn't a lock that needs breaking, it's a Lock with a
         # lock file pointing to an existing, unrelated file.  Refuse to break
         # that lock.  All we really need to do is to log and return.  If a
         # timeout was given, eventually the .lock() call will timeout.
         # However if no timeout was given, the .lock() will block forever.
         try:
-            self.details
+            self.details                            # noqa: B018
         except NotLockedError:
             log.error(
                 "lockfile exists but isn't safe to break: {}".format(
                     self._lockfile
                 )
             )
             return
@@ -602,15 +604,15 @@
         # they'll do in that function is delete the lock files, not claim the
         # lock, and we can be defensive for ENOENTs here.
         #
         # Touching the lock could fail if the process breaking the lock and
         # the process that claimed the lock have different owners.  Don't do
         # that.
         with suppress(PermissionError):
-            self._touch(self._lockfile)
+            self._touch(self._lockfile)             # pragma: nocover
         # Get the name of the old winner's claim file.
         winner = self._read()
         # Remove the global lockfile, which actually breaks the lock.
         try:
             os.unlink(self._lockfile)
         except OSError as error:                    # pragma: nocover
             if error.errno not in ERRORS:
```

### Comparing `flufl.lock-7.1.1/test/test_lock.py` & `flufl_lock-8.0/test/test_lock.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,43 +2,56 @@
 
 import os
 import re
 import sys
 import time
 import errno
 import builtins
+import platform
 
 from contextlib import contextmanager, ExitStack, suppress
 from datetime import timedelta
 from io import StringIO
 from multiprocessing import Process, Queue
 from pathlib import Path
 from random import randint
 from tempfile import TemporaryDirectory
 from unittest.mock import patch
 
 import pytest
 
 from flufl.lock import Lock, LockState, NotLockedError, SEP, TimeOutError
-from flufl.lock._lockfile import CLOCK_SLOP
+from flufl.lock._lockfile import CLOCK_SLOP, ERRORS
 
 
 EMOCKEDFAILURE = 99
 EOTHERMOCKEDFAILURE = 98
+ENINES = 999
 
 
 @pytest.fixture
 def lock():
     with TemporaryDirectory() as lock_dir:
         lock = Lock(os.path.join(lock_dir, 'test.lck'))
         yield lock
         with suppress(NotLockedError):
             lock.unlock()
 
 
+def child_locker(filename, queue, *, sleep=3, lifetime=15, keep=False):
+    with suppress(NotLockedError):
+        with Lock(filename, lifetime=lifetime):
+            queue.put(True)
+            time.sleep(sleep)
+            queue.put(True)
+            # The test wants us to keep the lock a little bit longer.
+            if keep:
+                queue.get()
+
+
 def test_retry_errno_property(lock):
     assert lock.retry_errnos == []
     lock.retry_errnos = [EMOCKEDFAILURE, EOTHERMOCKEDFAILURE]
     assert lock.retry_errnos == [EMOCKEDFAILURE, EOTHERMOCKEDFAILURE]
     del lock.retry_errnos
     assert lock.retry_errnos == []
 
@@ -69,19 +82,19 @@
     assert retry_open.retry_count == 3
 
 
 def test_read_unexpected_errors(lock):
     # Test that _read() will raise when an unexpected errno is encountered.
     lock.lock()
     retry_open = RetryOpen(failure_countdown=3)
-    retry_open.errno = 999
+    retry_open.errno = ENINES
     with patch('builtins.open', retry_open):
         with pytest.raises(OSError) as excinfo:
             lock.is_locked
-        assert excinfo.value.errno == 999
+        assert excinfo.value.errno == ENINES
 
 
 def test_is_locked_permission_error(lock):
     with ExitStack() as resources:
         resources.enter_context(patch('os.utime', side_effect=PermissionError))
         log_mock = resources.enter_context(patch('flufl.lock._lockfile.log'))
         assert not lock.is_locked
@@ -185,21 +198,14 @@
     assert lock.lifetime.seconds == 31
     # No exception is raised when we try to refresh an unlocked lock
     # unconditionally.
     lock.unlock()
     lock.refresh(unconditionally=True)
 
 
-def child_locker(filename, queue, sleep=3, lifetime=15):
-    with suppress(NotLockedError):
-        with Lock(filename, lifetime=lifetime):
-            queue.put(True)
-            time.sleep(sleep)
-
-
 def test_lock_with_explicit_timeout(lock):
     queue = Queue()
     Process(target=child_locker, args=(lock.lockfile, queue)).start()
     # Wait for the child process to acquire the lock.
     queue.get()
     with pytest.raises(TimeOutError):
         lock.lock(timeout=1)
@@ -259,18 +265,18 @@
 class SymlinkErrorRaiser(SymlinkErrorRaiserBase):
     def __init__(self, errnos):
         super().__init__(errnos)
         self._os_function = os.link
 
 
 def test_os_link_expected_OSError(lock):
-    with patch('os.link', SymlinkErrorRaiser([999])):
+    with patch('os.link', SymlinkErrorRaiser([ENINES])):
         with pytest.raises(OSError) as excinfo:
             lock.lock()
-        assert excinfo.value.errno == 999
+        assert excinfo.value.errno == ENINES
 
 
 def test_os_link_unexpected_OSError(lock):
     raiser = SymlinkErrorRaiser([errno.ENOENT, errno.ESTALE])
     with patch('os.link', raiser):
         lock.lock()
     # os.link() will be called 3 time; the first two will raise exceptions
@@ -336,19 +342,19 @@
     # os.unlink() gets called twice.  The first one unlinks the lock file, but
     # that results in an expected errno.  The second one unlinks the claimfile.
     assert unlinker.call_count == 2
 
 
 def test_unlock_with_unexpected_OSError(lock):
     lock.lock()
-    unlinker = SymUnlinkErrorRaiser([999])
+    unlinker = SymUnlinkErrorRaiser([ENINES])
     with patch('os.unlink', unlinker):
         with pytest.raises(OSError) as excinfo:
             lock.unlock()
-        assert excinfo.value.errno == 999
+        assert excinfo.value.errno == ENINES
     # os.unlink() gets called once, since the unlinking of the lockfile
     # results in an unexpected errno.
     assert unlinker.call_count == 1
 
 
 def test_unlock_unconditionally_with_expected_OSError(lock):
     unlinker = SymUnlinkErrorRaiser([errno.ESTALE])
@@ -356,31 +362,31 @@
         lock.unlock(unconditionally=True)
     # Since the lock was not acquired, os.unlink() should have been called
     # exactly once to remove the claim file.
     assert unlinker.call_count == 1
 
 
 def test_unlock_unconditionally_with_unexpected_OSError(lock):
-    unlinker = SymUnlinkErrorRaiser([999])
+    unlinker = SymUnlinkErrorRaiser([ENINES])
     with patch('os.unlink', unlinker):
         with pytest.raises(OSError) as excinfo:
             lock.unlock(unconditionally=True)
-        assert excinfo.value.errno == 999
+        assert excinfo.value.errno == ENINES
     # Since the lock was not acquired, os.unlink() should have been called
     # exactly once to remove the claim file.
     assert unlinker.call_count == 1
 
 
 class MtimeFailure:
     def __init__(self, stat_results):
         self._stat_results = stat_results
 
     def __getattr__(self, name):
         if name == 'st_mtime':
-            raise OSError(999, 'st_mtime failure')
+            raise OSError(ENINES, 'st_mtime failure')
         return getattr(self._stat_results, name)
 
 
 class StatMtimeFailure:
     def __init__(self):
         self._os_stat = os.stat
 
@@ -390,31 +396,31 @@
 
 def test_releasetime_weird_failure(lock):
     # _releasetime() is an internal function that returns the expiration of
     # the lock, but handles error conditions.  We have to basically fail to
     # acquire a lock, don't time out, and the os_stat() of the lock file must
     # fail with an unexpected error.
     queue = Queue()
-    Process(target=child_locker, args=(lock.lockfile, queue, 3)).start()
+    Process(target=child_locker, args=(lock.lockfile, queue)).start()
     # Wait for the child process to acquire the lock.
     queue.get()
     # Now we try to acquire the lock, which will fail.
     with patch('os.stat', StatMtimeFailure()):
         with pytest.raises(OSError) as excinfo:
             lock.lock()
-    assert excinfo.value.errno == 999
+    assert excinfo.value.errno == ENINES
 
 
 class NlinkFailure:
     def __init__(self, stat_results):
         self._stat_results = stat_results
 
     def __getattr__(self, name):
         if name == 'st_nlink':
-            raise OSError(999, 'st_nlink failure')
+            raise OSError(ENINES, 'st_nlink failure')
         return getattr(self._stat_results, name)
 
 
 class StatNlinkFailure:
     def __init__(self):
         self._os_stat = os.stat
 
@@ -424,22 +430,22 @@
 
 def test_linkcount_weird_failure(lock):
     # _releasetime() is an internal function that returns the expiration of
     # the lock, but handles error conditions.  We have to basically fail to
     # acquire a lock, don't time out, and the os_stat() of the lock file must
     # fail with an unexpected error.
     queue = Queue()
-    Process(target=child_locker, args=(lock.lockfile, queue, 3)).start()
+    Process(target=child_locker, args=(lock.lockfile, queue)).start()
     # Wait for the child process to acquire the lock.
     queue.get()
     # Now we try to acquire the lock, which will fail.
     with patch('os.stat', StatNlinkFailure()):
         with pytest.raises(OSError) as excinfo:
             lock.is_locked
-    assert excinfo.value.errno == 999
+    assert excinfo.value.errno == ENINES
 
 
 def test_lock_constructor_with_timeout(lock):
     # Pass an optional timeout value to the constructor.
     queue = Queue()
     Process(target=child_locker, args=(lock.lockfile, queue)).start()
     # Wait for the child process to acquire the lock.
@@ -453,15 +459,15 @@
     # Explicit timeout in the lock() call overrides constructor timeout.
     queue = Queue()
     Process(target=child_locker,
             # Give the child lock a lifetime of 5 seconds.  We'll provide a
             # shorter timeout in the constructor, which should time out, but a
             # longer time in the lock() call which will result in acquiring
             # the lock when the lifetime of the child expires.
-            args=(lock.lockfile, queue, 3, 5)
+            args=(lock.lockfile, queue), kwargs=dict(sleep=3, lifetime=5),
             ).start()
     # Wait for the child process to acquire the lock.
     queue.get()
     my_lock = Lock(lock.lockfile, default_timeout=1)
     try:
         my_lock.lock(timeout=10)
         assert my_lock.is_locked
@@ -488,7 +494,95 @@
     # clock slop factor.
     past = time.time() - lifetime - CLOCK_SLOP.seconds
     os.utime(lock.lockfile, (past, past))
     with pytest.raises(TimeOutError):
         lock.lock(timeout=3)
     with open(lock.lockfile) as fp:
         assert fp.read() == 'save me'
+
+
+# 2023-06-20(warsaw): On CI in Windows, we sometimes see PermissionError when
+# unlocking the lock on context manager __exit__(), but only in the lock
+# breaking tests.  It appears to happen when we attempt to unlink the lock
+# file.
+#
+# [WinError 32] The process cannot access the file because it is being used
+# by another process
+#
+# Despite the '32' there, by trial and error, it seems that the errno that
+# occurs is actually 13.  I have no idea why the original error occurs, nor
+# why we get this mysterious value 13, but at least on Windows, this allows CI
+# to pass.
+WINDOWS_CI_ERRNO = 13
+
+
+def test_break_lock(lock, monkeypatch, capsys):
+    queue = Queue()
+    proc = Process(target=child_locker,
+            # The child will acquire the lock and sleep for 5 seconds, which
+            # is longer than lock's lifetime.  Once the second boolean is
+            # placed in the queue, we know that the sleep has completed and
+            # the lock should be ready for breakage in the parent.
+            args=(lock.lockfile, queue),
+            kwargs=dict(sleep=5, lifetime=3, keep=True),
+            ).start()
+    # Wait for the child process to acquire the lock.
+    queue.get()
+    child_details = lock.details
+    # Wait for the child to finish sleeping.
+    queue.get()
+    # Now acquire the lock in the parent.  This should break the lock. See
+    # above for an explanation of why we have to monkeypatch ERRORS on
+    # Windows.
+    if platform.system() == 'Windows':
+        monkeypatch.setattr(
+            'flufl.lock._lockfile.ERRORS',
+            list(ERRORS) + [WINDOWS_CI_ERRNO])
+    with lock:
+        assert lock.is_locked
+        # The child no longer has the lock.
+        assert child_details != lock.details
+        # Let the child exit.
+        queue.put(True)
+
+
+def test_break_lock_with_ununlinkable_winner(lock, monkeypatch):
+    queue = Queue()
+    proc = Process(target=child_locker,
+            # The child will acquire the lock and sleep for 5 seconds, which
+            # is longer than lock's lifetime.  Once the second boolean is
+            # placed in the queue, we know that the sleep has completed and
+            # the lock should be ready for breakage in the parent.
+            args=(lock.lockfile, queue),
+            kwargs=dict(sleep=5, lifetime=3, keep=True),
+            ).start()
+    # Wait for the child process to acquire the lock.
+    queue.get()
+    child_details = lock.details
+    # Wait for the child to finish sleeping.
+    queue.get()
+    # Now acquire the lock in the parent.  This should break the lock.
+    #
+    # Count how many times os.unlink() gets called when breaking the lock.
+    # The fourth call (found by trial and error) should be the attempt to
+    # unlink the winner file in Lock._break().
+    unlink_count = 2
+    os_unlink = os.unlink
+    def unlink_counter(*args, **kws):
+        nonlocal unlink_count
+        unlink_count -= 1
+        if unlink_count > 0:
+            return os_unlink(*args, **kws)
+        raise OSError(ENINES, 'Bad Unlink')
+    if platform.system() == 'Windows':
+        monkeypatch.setattr(
+            'flufl.lock._lockfile.ERRORS',
+            list(ERRORS) + [WINDOWS_CI_ERRNO])
+    with patch('os.unlink', unlink_counter):
+        # This lock attempt will technically succeed, but it will raise an
+        # exception (EMOCKEDFAILURE) during the attempt to os.unlink(winner).
+        # It's coverage of that call that this test is actually after.
+        with pytest.raises(OSError) as excinfo:
+            lock.lock()
+        assert excinfo.value.errno == ENINES
+        # We still need to let the child exit.
+        queue.put(True)
```

### Comparing `flufl.lock-7.1.1/PKG-INFO` & `flufl_lock-8.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
-Name: flufl.lock
-Version: 7.1.1
+Name: flufl-lock
+Version: 8.0
 Summary: NFS-safe file locking with timeouts for POSIX and Windows
+Keywords: locking locks lock
+Author-Email: Barry Warsaw <barry@python.org>
 License: Apache-2.0
-Keywords: locking,locks,lock
-Author-email: Barry Warsaw <barry@python.org>
-Requires-Python: >=3.7
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Project-URL: Bug Tracker, https://gitlab.com/warsaw/flufl.lock/issues
+Project-URL: Home page, https://flufllock.readthedocs.io
 Project-URL: Documentation, https://flufllock.readthedocs.io
-Project-URL: Home Page, https://flufllock.readthedocs.io
-Project-URL: Source Code, https://gitlab.com/warsaw/flufl.lock.git
+Project-URL: Source code, https://gitlab.com/warsaw/flufl.lock.git
+Project-URL: Bug tracker, https://gitlab.com/warsaw/flufl.lock/issues
+Requires-Python: >=3.8
+Requires-Dist: atpublic
+Requires-Dist: psutil
 Description-Content-Type: text/x-rst
 
 ==========
 flufl.lock
 ==========
 
 NFS-safe file locking with timeouts for POSIX and Windows.
@@ -58,22 +60,21 @@
 data.  In a distributed (NFS) environment, you also need to make sure that
 your clocks are properly synchronized.
 
 
 Author
 ======
 
-``flufl.lock`` is Copyright (C) 2007-2022 Barry Warsaw <barry@python.org>
+``flufl.lock`` is Copyright (C) 2007-2023 Barry Warsaw <barry@python.org>
 
 Licensed under the terms of the Apache License Version 2.0.  See the LICENSE
 file for details.
 
 
 Project details
 ===============
 
  * Project home: https://gitlab.com/warsaw/flufl.lock
  * Report bugs at: https://gitlab.com/warsaw/flufl.lock/issues
  * Code hosting: https://gitlab.com/warsaw/flufl.lock.git
  * Documentation: https://flufllock.readthedocs.io/
  * PyPI: https://pypi.python.org/pypi/flufl.lock
-
```

