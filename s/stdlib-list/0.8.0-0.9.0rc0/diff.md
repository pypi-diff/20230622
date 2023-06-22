# Comparing `tmp/stdlib-list-0.8.0.tar.gz` & `tmp/stdlib_list-0.9.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/stdlib-list-0.8.0.tar", last modified: Thu Nov 19 14:10:49 2020, max compression
+gzip compressed data, was "stdlib_list-0.9.0rc0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `stdlib-list-0.8.0.tar` & `stdlib_list-0.9.0rc0.tar`

### file list

```diff
@@ -1,48 +1,21 @@
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2020-11-19 14:10:49.380721 stdlib-list-0.8.0/
--rw-r--r--   0 filipe    (1000) filipe    (1000)       37 2018-11-08 16:22:48.000000 stdlib-list-0.8.0/.gitattributes
--rw-r--r--   0 filipe    (1000) filipe    (1000)     3379 2018-11-08 14:29:17.000000 stdlib-list-0.8.0/.gitignore
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      675 2020-11-19 14:10:22.000000 stdlib-list-0.8.0/.travis.yml
--rw-r--r--   0 filipe    (1000) filipe    (1000)     1077 2018-11-08 14:29:17.000000 stdlib-list-0.8.0/LICENSE
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      160 2020-06-08 20:50:45.000000 stdlib-list-0.8.0/MANIFEST.in
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     2559 2020-11-19 14:10:49.380721 stdlib-list-0.8.0/PKG-INFO
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     2030 2020-06-08 20:50:45.000000 stdlib-list-0.8.0/README.md
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2020-11-19 14:10:49.352719 stdlib-list-0.8.0/docs/
--rw-r--r--   0 filipe    (1000) filipe    (1000)     6838 2018-11-08 14:29:17.000000 stdlib-list-0.8.0/docs/Makefile
--rw-r--r--   0 filipe    (1000) filipe    (1000)     8960 2019-11-26 17:04:22.000000 stdlib-list-0.8.0/docs/conf.py
--rw-r--r--   0 filipe    (1000) filipe    (1000)      397 2018-11-08 14:29:17.000000 stdlib-list-0.8.0/docs/fetch.rst
--rw-r--r--   0 filipe    (1000) filipe    (1000)     2100 2018-11-08 14:29:17.000000 stdlib-list-0.8.0/docs/index.rst
--rw-r--r--   0 filipe    (1000) filipe    (1000)      229 2018-11-08 14:29:17.000000 stdlib-list-0.8.0/docs/install.rst
--rw-r--r--   0 filipe    (1000) filipe    (1000)     6739 2018-11-08 14:29:17.000000 stdlib-list-0.8.0/docs/make.bat
--rw-r--r--   0 filipe    (1000) filipe    (1000)     1364 2019-11-26 14:27:21.000000 stdlib-list-0.8.0/docs/usage.rst
--rw-r--r--   0 filipe    (1000) filipe    (1000)       64 2019-11-27 11:35:37.000000 stdlib-list-0.8.0/requirements-dev.txt
--rw-r--r--   0 filipe    (1000) filipe    (1000)        7 2018-11-08 14:29:17.000000 stdlib-list-0.8.0/requirements.txt
--rw-r--r--   0 filipe    (1000) filipe    (1000)      264 2020-11-19 14:10:49.380721 stdlib-list-0.8.0/setup.cfg
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      832 2020-11-13 14:16:40.000000 stdlib-list-0.8.0/setup.py
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2020-11-19 14:10:49.384722 stdlib-list-0.8.0/stdlib_list/
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      298 2020-06-08 20:50:45.000000 stdlib-list-0.8.0/stdlib_list/__init__.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      498 2020-11-19 14:10:49.384722 stdlib-list-0.8.0/stdlib_list/_version.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     2963 2020-06-08 20:50:45.000000 stdlib-list-0.8.0/stdlib_list/base.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     2388 2020-11-15 00:04:46.000000 stdlib-list-0.8.0/stdlib_list/fetch.py
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2020-11-19 14:10:49.380721 stdlib-list-0.8.0/stdlib_list/lists/
--rw-r--r--   0 filipe    (1000) filipe    (1000)     4720 2018-11-08 14:29:17.000000 stdlib-list-0.8.0/stdlib_list/lists/2.6.txt
--rw-rw-r--   0 filipe    (1000) filipe    (1000)    27222 2020-06-08 20:50:45.000000 stdlib-list-0.8.0/stdlib_list/lists/2.7.txt
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     3514 2020-06-08 20:50:45.000000 stdlib-list-0.8.0/stdlib_list/lists/3.2.txt
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     3618 2020-06-08 20:50:45.000000 stdlib-list-0.8.0/stdlib_list/lists/3.3.txt
--rw-rw-r--   0 filipe    (1000) filipe    (1000)    31024 2020-06-08 20:50:45.000000 stdlib-list-0.8.0/stdlib_list/lists/3.4.txt
--rw-rw-r--   0 filipe    (1000) filipe    (1000)    32711 2020-06-08 20:50:45.000000 stdlib-list-0.8.0/stdlib_list/lists/3.5.txt
--rw-rw-r--   0 filipe    (1000) filipe    (1000)    34003 2020-06-08 20:50:45.000000 stdlib-list-0.8.0/stdlib_list/lists/3.6.txt
--rw-rw-r--   0 filipe    (1000) filipe    (1000)    35238 2020-06-08 20:50:45.000000 stdlib-list-0.8.0/stdlib_list/lists/3.7.txt
--rw-rw-r--   0 filipe    (1000) filipe    (1000)    36209 2020-06-08 20:50:45.000000 stdlib-list-0.8.0/stdlib_list/lists/3.8.txt
--rw-rw-r--   0 filipe    (1000) filipe    (1000)    16244 2020-11-18 17:15:08.000000 stdlib-list-0.8.0/stdlib_list/lists/3.9.txt
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2020-11-19 14:10:49.356720 stdlib-list-0.8.0/stdlib_list.egg-info/
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     2559 2020-11-19 14:10:49.000000 stdlib-list-0.8.0/stdlib_list.egg-info/PKG-INFO
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      843 2020-11-19 14:10:49.000000 stdlib-list-0.8.0/stdlib_list.egg-info/SOURCES.txt
--rw-rw-r--   0 filipe    (1000) filipe    (1000)        1 2020-11-19 14:10:49.000000 stdlib-list-0.8.0/stdlib_list.egg-info/dependency_links.txt
--rw-rw-r--   0 filipe    (1000) filipe    (1000)       57 2020-11-19 14:10:49.000000 stdlib-list-0.8.0/stdlib_list.egg-info/requires.txt
--rw-rw-r--   0 filipe    (1000) filipe    (1000)       12 2020-11-19 14:10:49.000000 stdlib-list-0.8.0/stdlib_list.egg-info/top_level.txt
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2020-11-19 14:10:49.380721 stdlib-list-0.8.0/tests/
--rw-rw-r--   0 filipe    (1000) filipe    (1000)        0 2020-06-08 20:50:45.000000 stdlib-list-0.8.0/tests/__init__.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      130 2020-06-08 20:50:45.000000 stdlib-list-0.8.0/tests/__main__.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     2957 2020-06-08 20:50:45.000000 stdlib-list-0.8.0/tests/test_basic.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     5295 2020-11-15 00:04:37.000000 stdlib-list-0.8.0/tests/test_platform.py
--rw-r--r--   0 filipe    (1000) filipe    (1000)    68611 2019-11-26 17:04:22.000000 stdlib-list-0.8.0/versioneer.py
+-rw-r--r--   0        0        0     1077 2023-06-22 03:57:34.675631 stdlib_list-0.9.0rc0/LICENSE
+-rw-r--r--   0        0        0     1928 2023-06-22 03:57:34.675631 stdlib_list-0.9.0rc0/README.md
+-rw-r--r--   0        0        0     1567 2023-06-22 03:57:34.675631 stdlib_list-0.9.0rc0/pyproject.toml
+-rw-r--r--   0        0        0      353 2023-06-22 03:57:34.675631 stdlib_list-0.9.0rc0/stdlib_list/__init__.py
+-rw-r--r--   0        0        0     2922 2023-06-22 03:57:34.675631 stdlib_list-0.9.0rc0/stdlib_list/base.py
+-rw-r--r--   0        0        0     4720 2023-06-22 03:57:34.675631 stdlib_list-0.9.0rc0/stdlib_list/lists/2.6.txt
+-rw-r--r--   0        0        0    27222 2023-06-22 03:57:34.675631 stdlib_list-0.9.0rc0/stdlib_list/lists/2.7.txt
+-rw-r--r--   0        0        0    18293 2023-06-22 03:57:34.675631 stdlib_list-0.9.0rc0/stdlib_list/lists/3.10.txt
+-rw-r--r--   0        0        0    18405 2023-06-22 03:57:34.675631 stdlib_list-0.9.0rc0/stdlib_list/lists/3.11.txt
+-rw-r--r--   0        0        0     3514 2023-06-22 03:57:34.675631 stdlib_list-0.9.0rc0/stdlib_list/lists/3.2.txt
+-rw-r--r--   0        0        0     3618 2023-06-22 03:57:34.675631 stdlib_list-0.9.0rc0/stdlib_list/lists/3.3.txt
+-rw-r--r--   0        0        0    31024 2023-06-22 03:57:34.675631 stdlib_list-0.9.0rc0/stdlib_list/lists/3.4.txt
+-rw-r--r--   0        0        0    32711 2023-06-22 03:57:34.675631 stdlib_list-0.9.0rc0/stdlib_list/lists/3.5.txt
+-rw-r--r--   0        0        0    34003 2023-06-22 03:57:34.679631 stdlib_list-0.9.0rc0/stdlib_list/lists/3.6.txt
+-rw-r--r--   0        0        0    35554 2023-06-22 03:57:34.679631 stdlib_list-0.9.0rc0/stdlib_list/lists/3.7.txt
+-rw-r--r--   0        0        0    36675 2023-06-22 03:57:34.679631 stdlib_list-0.9.0rc0/stdlib_list/lists/3.8.txt
+-rw-r--r--   0        0        0    34880 2023-06-22 03:57:34.679631 stdlib_list-0.9.0rc0/stdlib_list/lists/3.9.txt
+-rw-r--r--   0        0        0        0 2023-06-22 03:57:34.679631 stdlib_list-0.9.0rc0/stdlib_list/py.typed
+-rw-r--r--   0        0        0        0 2023-06-22 03:57:34.679631 stdlib_list-0.9.0rc0/tests/__init__.py
+-rw-r--r--   0        0        0      952 2023-06-22 03:57:34.679631 stdlib_list-0.9.0rc0/tests/test_base.py
+-rw-r--r--   0        0        0     2975 1970-01-01 00:00:00.000000 stdlib_list-0.9.0rc0/PKG-INFO
```

### Comparing `stdlib-list-0.8.0/LICENSE` & `stdlib_list-0.9.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `stdlib-list-0.8.0/stdlib_list/base.py` & `stdlib_list-0.9.0rc0/stdlib_list/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,84 +1,95 @@
-from __future__ import print_function, absolute_import
+from __future__ import annotations
 
 import os
 import pkgutil
 import sys
+from functools import lru_cache
 
-try:
-    from functools import lru_cache
-except ImportError:
-    from functools32 import lru_cache
-
-long_versions = ["2.6.9", "2.7.9", "3.2.6", "3.3.6", "3.4.3", "3.5", "3.6",
-                 "3.7", "3.8", "3.9"]
+long_versions = [
+    "2.6.9",
+    "2.7.9",
+    "3.2.6",
+    "3.3.6",
+    "3.4.3",
+    "3.5",
+    "3.6",
+    "3.7",
+    "3.8",
+    "3.9",
+    "3.10",
+    "3.11",
+]
 
 short_versions = [".".join(x.split(".")[:2]) for x in long_versions]
 
 
-def get_canonical_version(version):
-
+def get_canonical_version(version: str) -> str:
     if version in long_versions:
         version = ".".join(version.split(".")[:2])
     elif version not in short_versions:
-        raise ValueError("No such version: {}".format(version))
+        raise ValueError(f"No such version: {version}")
 
     return version
 
 
-def stdlib_list(version=None):
+def stdlib_list(version: str | None = None) -> list[str]:
     """
     Given a ``version``, return a ``list`` of names of the Python Standard
-    Libraries for that version. These names are obtained from the Sphinx inventory
-    file (used in :py:mod:`sphinx.ext.intersphinx`).
+    Libraries for that version.
 
     :param str|None version: The version (as a string) whose list of libraries you want
-    (one of ``"2.6"``, ``"2.7"``, ``"3.2"``, ``"3.3"``, ``"3.4"``, or ``"3.5"``).
-    If not specified, the current version of Python will be used.
+        (formatted as ``X.Y``, e.g. ``"2.7"`` or ``"3.10"``).
+
+        If not specified, the current version of Python will be used.
 
     :return: A list of standard libraries from the specified version of Python
     :rtype: list
     """
 
-    version = get_canonical_version(version) if version is not None else '.'.join(
-        str(x) for x in sys.version_info[:2])
+    version = (
+        get_canonical_version(version)
+        if version is not None
+        else ".".join(str(x) for x in sys.version_info[:2])
+    )
 
-    module_list_file = os.path.join("lists", "{}.txt".format(version))
+    module_list_file = os.path.join("lists", f"{version}.txt")
 
-    data = pkgutil.get_data("stdlib_list", module_list_file).decode()
+    data = pkgutil.get_data("stdlib_list", module_list_file).decode()  # type: ignore[union-attr]
 
     result = [y for y in [x.strip() for x in data.splitlines()] if y]
 
     return result
 
 
 @lru_cache(maxsize=16)
-def _stdlib_list_with_cache(version=None):
+def _stdlib_list_with_cache(version: str | None = None) -> list[str]:
     """Internal cached version of `stdlib_list`"""
     return stdlib_list(version=version)
 
 
 @lru_cache(maxsize=256)
-def in_stdlib(module_name, version=None):
+def in_stdlib(module_name: str, version: str | None = None) -> bool:
     """
     Return a ``bool`` indicating if module ``module_name`` is in the list of stdlib
     symbols for python version ``version``. If ``version`` is ``None`` (default), the
     version of current python interpreter is used.
 
     Note that ``True`` will be returned for built-in modules too, since this project
     considers they are part of stdlib. See :issue:21.
 
     It relies on ``@lru_cache`` to cache the stdlib list and query results for similar
     calls. Therefore it is much more efficient than ``module_name in stdlib_list()``
     especially if you wish to perform multiple checks.
 
     :param str|None module_name: The module name (as a string) to query for.
     :param str|None version: The version (as a string) whose list of libraries you want
-    (one of ``"2.6"``, ``"2.7"``, ``"3.2"``, ``"3.3"``, ``"3.4"``, or ``"3.5"``).
-    If not specified, the current version of Python will be used.
+        (formatted as ``X.Y``, e.g. ``"2.7"`` or ``"3.10"``).
+
+        If not specified, the current version of Python will be used.
 
     :return: A bool indicating if the given module name is part of standard libraries
-    for the specified version of Python.
+        for the specified version of Python.
     :rtype: list
     """
     ref_list = _stdlib_list_with_cache(version=version)
     return module_name in ref_list
```

### Comparing `stdlib-list-0.8.0/stdlib_list/lists/2.6.txt` & `stdlib_list-0.9.0rc0/stdlib_list/lists/2.6.txt`

 * *Files identical despite different names*

### Comparing `stdlib-list-0.8.0/stdlib_list/lists/2.7.txt` & `stdlib_list-0.9.0rc0/stdlib_list/lists/2.7.txt`

 * *Files identical despite different names*

### Comparing `stdlib-list-0.8.0/stdlib_list/lists/3.2.txt` & `stdlib_list-0.9.0rc0/stdlib_list/lists/3.2.txt`

 * *Files identical despite different names*

### Comparing `stdlib-list-0.8.0/stdlib_list/lists/3.3.txt` & `stdlib_list-0.9.0rc0/stdlib_list/lists/3.3.txt`

 * *Files identical despite different names*

### Comparing `stdlib-list-0.8.0/stdlib_list/lists/3.4.txt` & `stdlib_list-0.9.0rc0/stdlib_list/lists/3.4.txt`

 * *Files identical despite different names*

### Comparing `stdlib-list-0.8.0/stdlib_list/lists/3.5.txt` & `stdlib_list-0.9.0rc0/stdlib_list/lists/3.5.txt`

 * *Files identical despite different names*

### Comparing `stdlib-list-0.8.0/stdlib_list/lists/3.6.txt` & `stdlib_list-0.9.0rc0/stdlib_list/lists/3.6.txt`

 * *Files identical despite different names*

### Comparing `stdlib-list-0.8.0/stdlib_list/lists/3.7.txt` & `stdlib_list-0.9.0rc0/stdlib_list/lists/3.7.txt`

 * *Files 1% similar despite different names*

```diff
@@ -913,14 +913,15 @@
 test.bytecode_helper
 test.coding20731
 test.curses_tests
 test.dataclass_module_1
 test.dataclass_module_1_str
 test.dataclass_module_2
 test.dataclass_module_2_str
+test.dataclass_textanno
 test.datetimetester
 test.dis_module
 test.doctest_aliases
 test.double_const
 test.dtracedata.call_stack
 test.dtracedata.gc
 test.dtracedata.instance
@@ -944,14 +945,15 @@
 test.libregrtest.main
 test.libregrtest.refleak
 test.libregrtest.runtest
 test.libregrtest.runtest_mp
 test.libregrtest.save_env
 test.libregrtest.setup
 test.libregrtest.utils
+test.libregrtest.win_utils
 test.list_tests
 test.lock_tests
 test.make_ssl_certs
 test.mapping_tests
 test.memory_watchdog
 test.mock_socket
 test.mod_generics_cache
@@ -1483,14 +1485,15 @@
 test.test_tk
 test.test_tokenize
 test.test_tools
 test.test_tools.__main__
 test.test_tools.test_fixcid
 test.test_tools.test_gprof2html
 test.test_tools.test_i18n
+test.test_tools.test_lll
 test.test_tools.test_md5sum
 test.test_tools.test_pdeps
 test.test_tools.test_pindent
 test.test_tools.test_reindent
 test.test_tools.test_sundry
 test.test_tools.test_unparse
 test.test_trace
@@ -1709,15 +1712,23 @@
 xml.etree.ElementInclude
 xml.etree.ElementPath
 xml.etree.ElementTree
 xml.etree.cElementTree
 xml.parsers
 xml.parsers.expat
 xml.parsers.expat.errors
+xml.parsers.expat.errors.dom
+xml.parsers.expat.errors.etree
+xml.parsers.expat.errors.parsers
+xml.parsers.expat.errors.sax
 xml.parsers.expat.model
+xml.parsers.expat.model.dom
+xml.parsers.expat.model.etree
+xml.parsers.expat.model.parsers
+xml.parsers.expat.model.sax
 xml.sax
 xml.sax._exceptions
 xml.sax.expatreader
 xml.sax.handler
 xml.sax.saxutils
 xml.sax.xmlreader
 xmlrpc
```

### Comparing `stdlib-list-0.8.0/stdlib_list/lists/3.8.txt` & `stdlib_list-0.9.0rc0/stdlib_list/lists/3.8.txt`

 * *Files 1% similar despite different names*

```diff
@@ -895,14 +895,15 @@
 test
 test.__main__
 test._test_multiprocessing
 test.ann_module
 test.ann_module2
 test.ann_module3
 test.audiotests
+test.audit-tests
 test.autotest
 test.bad_coding
 test.bad_coding2
 test.bad_getattr
 test.bad_getattr2
 test.bad_getattr3
 test.badsyntax_3131
@@ -919,14 +920,15 @@
 test.bytecode_helper
 test.coding20731
 test.curses_tests
 test.dataclass_module_1
 test.dataclass_module_1_str
 test.dataclass_module_2
 test.dataclass_module_2_str
+test.dataclass_textanno
 test.datetimetester
 test.dis_module
 test.doctest_aliases
 test.double_const
 test.dtracedata.call_stack
 test.dtracedata.gc
 test.dtracedata.instance
@@ -1011,19 +1013,21 @@
 test.test_asynchat
 test.test_asyncio
 test.test_asyncio.__main__
 test.test_asyncio.echo
 test.test_asyncio.echo2
 test.test_asyncio.echo3
 test.test_asyncio.functional
+test.test_asyncio.test_asyncio_waitfor
 test.test_asyncio.test_base_events
 test.test_asyncio.test_buffered_proto
 test.test_asyncio.test_context
 test.test_asyncio.test_events
 test.test_asyncio.test_futures
+test.test_asyncio.test_futures2
 test.test_asyncio.test_locks
 test.test_asyncio.test_pep492
 test.test_asyncio.test_proactor_events
 test.test_asyncio.test_protocols
 test.test_asyncio.test_queues
 test.test_asyncio.test_runners
 test.test_asyncio.test_selector_events
@@ -1292,14 +1296,15 @@
 test.test_importlib.source
 test.test_importlib.source.__main__
 test.test_importlib.source.test_case_sensitivity
 test.test_importlib.source.test_file_loader
 test.test_importlib.source.test_finder
 test.test_importlib.source.test_path_hook
 test.test_importlib.source.test_source_encoding
+test.test_importlib.stubs
 test.test_importlib.test_abc
 test.test_importlib.test_api
 test.test_importlib.test_lazy
 test.test_importlib.test_locks
 test.test_importlib.test_main
 test.test_importlib.test_metadata_api
 test.test_importlib.test_namespace_pkgs
@@ -1613,19 +1618,21 @@
 tkinter.messagebox
 tkinter.scrolledtext
 tkinter.simpledialog
 tkinter.test
 tkinter.test.runtktests
 tkinter.test.support
 tkinter.test.test_tkinter
+tkinter.test.test_tkinter.test_colorchooser
 tkinter.test.test_tkinter.test_font
 tkinter.test.test_tkinter.test_geometry_managers
 tkinter.test.test_tkinter.test_images
 tkinter.test.test_tkinter.test_loadtk
 tkinter.test.test_tkinter.test_misc
+tkinter.test.test_tkinter.test_simpledialog
 tkinter.test.test_tkinter.test_text
 tkinter.test.test_tkinter.test_variables
 tkinter.test.test_tkinter.test_widgets
 tkinter.test.test_ttk
 tkinter.test.test_ttk.test_extensions
 tkinter.test.test_ttk.test_functions
 tkinter.test.test_ttk.test_style
@@ -1744,15 +1751,23 @@
 xml.etree.ElementInclude
 xml.etree.ElementPath
 xml.etree.ElementTree
 xml.etree.cElementTree
 xml.parsers
 xml.parsers.expat
 xml.parsers.expat.errors
+xml.parsers.expat.errors.dom
+xml.parsers.expat.errors.etree
+xml.parsers.expat.errors.parsers
+xml.parsers.expat.errors.sax
 xml.parsers.expat.model
+xml.parsers.expat.model.dom
+xml.parsers.expat.model.etree
+xml.parsers.expat.model.parsers
+xml.parsers.expat.model.sax
 xml.sax
 xml.sax._exceptions
 xml.sax.expatreader
 xml.sax.handler
 xml.sax.saxutils
 xml.sax.xmlreader
 xmlrpc
```

### Comparing `stdlib-list-0.8.0/stdlib_list/lists/3.9.txt` & `stdlib_list-0.9.0rc0/stdlib_list/lists/3.11.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,71 +1,142 @@
 __future__
 __main__
-__phello__.foo
+_abc
 _aix_support
-_bootlocale
+_ast
+_asyncio
+_bisect
+_blake2
 _bootsubprocess
+_bz2
+_codecs
+_codecs_cn
+_codecs_hk
+_codecs_iso2022
+_codecs_jp
+_codecs_kr
+_codecs_tw
+_collections
 _collections_abc
 _compat_pickle
 _compression
+_contextvars
+_crypt
+_csv
+_ctypes
+_curses
+_curses_panel
+_datetime
+_dbm
+_decimal
+_elementtree
+_frozen_importlib
+_frozen_importlib_external
+_functools
+_gdbm
+_hashlib
+_heapq
+_imp
+_io
+_json
+_locale
+_lsprof
+_lzma
 _markupbase
+_md5
+_msi
+_multibytecodec
+_multiprocessing
+_opcode
+_operator
 _osx_support
+_overlapped
+_pickle
+_posixshmem
+_posixsubprocess
 _py_abc
 _pydecimal
 _pyio
+_queue
+_random
+_scproxy
+_sha1
+_sha256
+_sha3
+_sha512
+_signal
 _sitebuiltins
+_socket
+_sqlite3
+_sre
+_ssl
+_stat
+_statistics
+_string
 _strptime
-_sysconfigdata_x86_64_conda_cos6_linux_gnu
-_sysconfigdata_x86_64_conda_linux_gnu
+_struct
+_symtable
 _thread
 _threading_local
+_tkinter
+_tokenize
+_tracemalloc
+_typing
+_uuid
+_warnings
+_weakref
 _weakrefset
+_winapi
+_zoneinfo
 abc
 aifc
 antigravity
 argparse
 array
 ast
 asynchat
 asyncio
+asyncio.__main__
 asyncio.base_events
 asyncio.base_futures
 asyncio.base_subprocess
 asyncio.base_tasks
 asyncio.constants
 asyncio.coroutines
 asyncio.events
 asyncio.exceptions
 asyncio.format_helpers
 asyncio.futures
 asyncio.locks
 asyncio.log
+asyncio.mixins
 asyncio.proactor_events
 asyncio.protocols
 asyncio.queues
 asyncio.runners
 asyncio.selector_events
 asyncio.sslproto
 asyncio.staggered
 asyncio.streams
 asyncio.subprocess
+asyncio.taskgroups
 asyncio.tasks
 asyncio.threads
+asyncio.timeouts
 asyncio.transports
 asyncio.trsock
 asyncio.unix_events
 asyncio.windows_events
 asyncio.windows_utils
 asyncore
 atexit
 audioop
 base64
 bdb
 binascii
-binhex
 bisect
 builtins
 bz2
 cProfile
 calendar
 cgi
 cgitb
@@ -94,14 +165,67 @@
 ctypes
 ctypes._aix
 ctypes._endian
 ctypes.macholib
 ctypes.macholib.dyld
 ctypes.macholib.dylib
 ctypes.macholib.framework
+ctypes.test
+ctypes.test.__main__
+ctypes.test.test_anon
+ctypes.test.test_array_in_pointer
+ctypes.test.test_arrays
+ctypes.test.test_as_parameter
+ctypes.test.test_bitfields
+ctypes.test.test_buffers
+ctypes.test.test_bytes
+ctypes.test.test_byteswap
+ctypes.test.test_callbacks
+ctypes.test.test_cast
+ctypes.test.test_cfuncs
+ctypes.test.test_checkretval
+ctypes.test.test_delattr
+ctypes.test.test_errno
+ctypes.test.test_find
+ctypes.test.test_frombuffer
+ctypes.test.test_funcptr
+ctypes.test.test_functions
+ctypes.test.test_incomplete
+ctypes.test.test_init
+ctypes.test.test_internals
+ctypes.test.test_keeprefs
+ctypes.test.test_libc
+ctypes.test.test_loading
+ctypes.test.test_macholib
+ctypes.test.test_memfunctions
+ctypes.test.test_numbers
+ctypes.test.test_objects
+ctypes.test.test_parameters
+ctypes.test.test_pep3118
+ctypes.test.test_pickling
+ctypes.test.test_pointers
+ctypes.test.test_prototypes
+ctypes.test.test_python_api
+ctypes.test.test_random_things
+ctypes.test.test_refcounts
+ctypes.test.test_repr
+ctypes.test.test_returnfuncptrs
+ctypes.test.test_simplesubclasses
+ctypes.test.test_sizes
+ctypes.test.test_slicing
+ctypes.test.test_stringptr
+ctypes.test.test_strings
+ctypes.test.test_struct_fields
+ctypes.test.test_structures
+ctypes.test.test_unaligned_structures
+ctypes.test.test_unicode
+ctypes.test.test_values
+ctypes.test.test_varsize_struct
+ctypes.test.test_win32
+ctypes.test.test_wintypes
 ctypes.util
 ctypes.wintypes
 curses
 curses.ascii
 curses.has_key
 curses.panel
 curses.textpad
@@ -111,40 +235,42 @@
 dbm.dumb
 dbm.gnu
 dbm.ndbm
 decimal
 difflib
 dis
 distutils
+distutils._collections
+distutils._functools
+distutils._macos_compat
 distutils._msvccompiler
 distutils.archive_util
 distutils.bcppcompiler
 distutils.ccompiler
 distutils.cmd
 distutils.command
+distutils.command._framework_compat
 distutils.command.bdist
 distutils.command.bdist_dumb
-distutils.command.bdist_msi
-distutils.command.bdist_packager
 distutils.command.bdist_rpm
-distutils.command.bdist_wininst
 distutils.command.build
 distutils.command.build_clib
 distutils.command.build_ext
 distutils.command.build_py
 distutils.command.build_scripts
 distutils.command.check
 distutils.command.clean
 distutils.command.config
 distutils.command.install
 distutils.command.install_data
 distutils.command.install_egg_info
 distutils.command.install_headers
 distutils.command.install_lib
 distutils.command.install_scripts
+distutils.command.py37compat
 distutils.command.register
 distutils.command.sdist
 distutils.command.upload
 distutils.config
 distutils.core
 distutils.cygwinccompiler
 distutils.debug
@@ -155,60 +281,18 @@
 distutils.extension
 distutils.fancy_getopt
 distutils.file_util
 distutils.filelist
 distutils.log
 distutils.msvc9compiler
 distutils.msvccompiler
+distutils.py38compat
+distutils.py39compat
 distutils.spawn
 distutils.sysconfig
-distutils.tests
-distutils.tests.support
-distutils.tests.test_archive_util
-distutils.tests.test_bdist
-distutils.tests.test_bdist_dumb
-distutils.tests.test_bdist_msi
-distutils.tests.test_bdist_rpm
-distutils.tests.test_bdist_wininst
-distutils.tests.test_build
-distutils.tests.test_build_clib
-distutils.tests.test_build_ext
-distutils.tests.test_build_py
-distutils.tests.test_build_scripts
-distutils.tests.test_check
-distutils.tests.test_clean
-distutils.tests.test_cmd
-distutils.tests.test_config
-distutils.tests.test_config_cmd
-distutils.tests.test_core
-distutils.tests.test_cygwinccompiler
-distutils.tests.test_dep_util
-distutils.tests.test_dir_util
-distutils.tests.test_dist
-distutils.tests.test_extension
-distutils.tests.test_file_util
-distutils.tests.test_filelist
-distutils.tests.test_install
-distutils.tests.test_install_data
-distutils.tests.test_install_headers
-distutils.tests.test_install_lib
-distutils.tests.test_install_scripts
-distutils.tests.test_log
-distutils.tests.test_msvc9compiler
-distutils.tests.test_msvccompiler
-distutils.tests.test_register
-distutils.tests.test_sdist
-distutils.tests.test_spawn
-distutils.tests.test_sysconfig
-distutils.tests.test_text_file
-distutils.tests.test_unixccompiler
-distutils.tests.test_upload
-distutils.tests.test_util
-distutils.tests.test_version
-distutils.tests.test_versionpredicate
 distutils.text_file
 distutils.unixccompiler
 distutils.util
 distutils.version
 distutils.versionpredicate
 doctest
 email
@@ -359,24 +443,23 @@
 encodings.utf_32_le
 encodings.utf_7
 encodings.utf_8
 encodings.utf_8_sig
 encodings.uu_codec
 encodings.zlib_codec
 ensurepip
-ensurepip._bundled
+ensurepip.__main__
 ensurepip._uninstall
 enum
 errno
 faulthandler
 fcntl
 filecmp
 fileinput
 fnmatch
-formatter
 fractions
 ftplib
 functools
 gc
 genericpath
 getopt
 getpass
@@ -393,14 +476,15 @@
 html.parser
 http
 http.client
 http.cookiejar
 http.cookies
 http.server
 idlelib
+idlelib.__main__
 idlelib.autocomplete
 idlelib.autocomplete_w
 idlelib.autoexpand
 idlelib.browser
 idlelib.calltip
 idlelib.calltip_w
 idlelib.codecontext
@@ -478,17 +562,20 @@
 idlelib.idle_test.test_stackviewer
 idlelib.idle_test.test_statusbar
 idlelib.idle_test.test_text
 idlelib.idle_test.test_textview
 idlelib.idle_test.test_tooltip
 idlelib.idle_test.test_tree
 idlelib.idle_test.test_undo
+idlelib.idle_test.test_util
 idlelib.idle_test.test_warning
 idlelib.idle_test.test_window
 idlelib.idle_test.test_zoomheight
+idlelib.idle_test.test_zzdummy
+idlelib.idle_test.tkinter_testing_utils
 idlelib.iomenu
 idlelib.macosx
 idlelib.mainmenu
 idlelib.multicall
 idlelib.outwin
 idlelib.parenmatch
 idlelib.pathbrowser
@@ -509,41 +596,57 @@
 idlelib.squeezer
 idlelib.stackviewer
 idlelib.statusbar
 idlelib.textview
 idlelib.tooltip
 idlelib.tree
 idlelib.undo
+idlelib.util
 idlelib.window
 idlelib.zoomheight
 idlelib.zzdummy
 imaplib
 imghdr
 imp
 importlib
+importlib._abc
 importlib._bootstrap
 importlib._bootstrap_external
-importlib._common
 importlib.abc
 importlib.machinery
 importlib.metadata
+importlib.metadata._adapters
+importlib.metadata._collections
+importlib.metadata._functools
+importlib.metadata._itertools
+importlib.metadata._meta
+importlib.metadata._text
+importlib.readers
 importlib.resources
+importlib.resources._adapters
+importlib.resources._common
+importlib.resources._itertools
+importlib.resources._legacy
+importlib.resources.abc
+importlib.resources.readers
+importlib.resources.simple
+importlib.simple
 importlib.util
 inspect
 io
 ipaddress
 itertools
 json
 json.decoder
 json.encoder
 json.scanner
 json.tool
 keyword
-lib.libpython3
 lib2to3
+lib2to3.__main__
 lib2to3.btm_matcher
 lib2to3.btm_utils
 lib2to3.fixer_base
 lib2to3.fixer_util
 lib2to3.fixes
 lib2to3.fixes.fix_apply
 lib2to3.fixes.fix_asserts
@@ -608,30 +711,15 @@
 lib2to3.pgen2.pgen
 lib2to3.pgen2.token
 lib2to3.pgen2.tokenize
 lib2to3.pygram
 lib2to3.pytree
 lib2to3.refactor
 lib2to3.tests
-lib2to3.tests.data.bom
-lib2to3.tests.data.crlf
-lib2to3.tests.data.different_encoding
-lib2to3.tests.data.false_encoding
-lib2to3.tests.data.fixers.bad_order
-lib2to3.tests.data.fixers.myfixes
-lib2to3.tests.data.fixers.myfixes.fix_explicit
-lib2to3.tests.data.fixers.myfixes.fix_first
-lib2to3.tests.data.fixers.myfixes.fix_last
-lib2to3.tests.data.fixers.myfixes.fix_parrot
-lib2to3.tests.data.fixers.myfixes.fix_preorder
-lib2to3.tests.data.fixers.no_fixer_cls
-lib2to3.tests.data.fixers.parrot_example
-lib2to3.tests.data.infinite_recursion
-lib2to3.tests.data.py2_test_grammar
-lib2to3.tests.data.py3_test_grammar
+lib2to3.tests.__main__
 lib2to3.tests.pytree_idempotency
 lib2to3.tests.support
 lib2to3.tests.test_all_fixers
 lib2to3.tests.test_fixers
 lib2to3.tests.test_main
 lib2to3.tests.test_parser
 lib2to3.tests.test_pytree
@@ -674,24 +762,24 @@
 multiprocessing.sharedctypes
 multiprocessing.spawn
 multiprocessing.synchronize
 multiprocessing.util
 netrc
 nis
 nntplib
+nt
 ntpath
 nturl2path
 numbers
 opcode
 operator
 optparse
 os
 os.path
 ossaudiodev
-parser
 pathlib
 pdb
 pickle
 pickletools
 pipes
 pkgutil
 platform
@@ -705,18 +793,25 @@
 pty
 pwd
 py_compile
 pyclbr
 pydoc
 pydoc_data
 pydoc_data.topics
+pyexpat
+pyexpat.errors
+pyexpat.model
 queue
 quopri
 random
 re
+re._casefix
+re._compiler
+re._constants
+re._parser
 readline
 reprlib
 resource
 rlcompleter
 runpy
 sched
 secrets
@@ -743,60 +838,74 @@
 stat
 statistics
 string
 stringprep
 struct
 subprocess
 sunau
-symbol
 symtable
 sys
 sysconfig
 syslog
 tabnanny
 tarfile
 telnetlib
 tempfile
 termios
-test
-test.support
-test.support.bytecode_helper
-test.support.hashlib_helper
-test.support.logging_helper
-test.support.script_helper
-test.support.socket_helper
-test.support.testresult
-test.test_script_helper
-test.test_support
 textwrap
 this
 threading
 time
 timeit
 tkinter
+tkinter.__main__
 tkinter.colorchooser
 tkinter.commondialog
 tkinter.constants
 tkinter.dialog
 tkinter.dnd
 tkinter.filedialog
 tkinter.font
 tkinter.messagebox
 tkinter.scrolledtext
 tkinter.simpledialog
+tkinter.test
+tkinter.test.support
+tkinter.test.test_tkinter
+tkinter.test.test_tkinter.test_colorchooser
+tkinter.test.test_tkinter.test_font
+tkinter.test.test_tkinter.test_geometry_managers
+tkinter.test.test_tkinter.test_images
+tkinter.test.test_tkinter.test_loadtk
+tkinter.test.test_tkinter.test_messagebox
+tkinter.test.test_tkinter.test_misc
+tkinter.test.test_tkinter.test_simpledialog
+tkinter.test.test_tkinter.test_text
+tkinter.test.test_tkinter.test_variables
+tkinter.test.test_tkinter.test_widgets
+tkinter.test.test_ttk
+tkinter.test.test_ttk.test_extensions
+tkinter.test.test_ttk.test_style
+tkinter.test.test_ttk.test_widgets
+tkinter.test.widget_tests
 tkinter.tix
 tkinter.ttk
 token
 tokenize
+tomllib
+tomllib._parser
+tomllib._re
+tomllib._types
 trace
 traceback
 tracemalloc
 tty
 turtle
 turtledemo
+turtledemo.__main__
 turtledemo.bytedesign
 turtledemo.chaos
 turtledemo.clock
 turtledemo.colormixer
 turtledemo.forest
 turtledemo.fractalcurves
 turtledemo.lindenmayer
@@ -812,44 +921,77 @@
 turtledemo.tree
 turtledemo.two_canvases
 turtledemo.yinyang
 types
 typing
 unicodedata
 unittest
+unittest.__main__
 unittest._log
 unittest.async_case
 unittest.case
 unittest.loader
 unittest.main
 unittest.mock
 unittest.result
 unittest.runner
 unittest.signals
 unittest.suite
+unittest.test
+unittest.test.__main__
+unittest.test._test_warnings
+unittest.test.dummy
+unittest.test.support
+unittest.test.test_assertions
+unittest.test.test_async_case
+unittest.test.test_break
+unittest.test.test_case
+unittest.test.test_discovery
+unittest.test.test_functiontestcase
+unittest.test.test_loader
+unittest.test.test_program
+unittest.test.test_result
+unittest.test.test_runner
+unittest.test.test_setups
+unittest.test.test_skipping
+unittest.test.test_suite
+unittest.test.testmock
+unittest.test.testmock.__main__
+unittest.test.testmock.support
+unittest.test.testmock.testasync
+unittest.test.testmock.testcallable
+unittest.test.testmock.testhelpers
+unittest.test.testmock.testmagicmethods
+unittest.test.testmock.testmock
+unittest.test.testmock.testpatch
+unittest.test.testmock.testsealable
+unittest.test.testmock.testsentinel
+unittest.test.testmock.testwith
 unittest.util
 urllib
 urllib.error
 urllib.parse
 urllib.request
 urllib.response
 urllib.robotparser
 uu
 uuid
 venv
+venv.__main__
 warnings
 wave
 weakref
 webbrowser
 winreg
 winsound
 wsgiref
 wsgiref.handlers
 wsgiref.headers
 wsgiref.simple_server
+wsgiref.types
 wsgiref.util
 wsgiref.validate
 xdrlib
 xml
 xml.dom
 xml.dom.NodeFilter
 xml.dom.domreg
@@ -861,25 +1003,24 @@
 xml.etree
 xml.etree.ElementInclude
 xml.etree.ElementPath
 xml.etree.ElementTree
 xml.etree.cElementTree
 xml.parsers
 xml.parsers.expat
-xml.parsers.expat.errors
-xml.parsers.expat.model
 xml.sax
 xml.sax._exceptions
 xml.sax.expatreader
 xml.sax.handler
 xml.sax.saxutils
 xml.sax.xmlreader
 xmlrpc
 xmlrpc.client
 xmlrpc.server
+xxsubtype
 zipapp
 zipfile
 zipimport
 zlib
 zoneinfo
 zoneinfo._common
 zoneinfo._tzpath
```

