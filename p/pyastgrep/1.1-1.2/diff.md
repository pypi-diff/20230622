# Comparing `tmp/pyastgrep-1.1.tar.gz` & `tmp/pyastgrep-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyastgrep-1.1.tar", last modified: Fri Jun  9 13:42:58 2023, max compression
+gzip compressed data, was "pyastgrep-1.2.tar", last modified: Wed Jun 21 20:24:35 2023, max compression
```

## Comparing `pyastgrep-1.1.tar` & `pyastgrep-1.2.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-06-09 13:42:58.005910 pyastgrep-1.1/
--rw-r--r--   0 luke      (1000) luke      (1000)      378 2022-10-17 13:09:58.000000 pyastgrep-1.1/.gitattributes
--rw-r--r--   0 luke      (1000) luke      (1000)     1771 2022-11-07 12:01:43.000000 pyastgrep-1.1/.gitignore
--rw-rw-rw-   0 luke      (1000) luke      (1000)    14968 2023-06-09 13:42:58.005910 pyastgrep-1.1/PKG-INFO
--rw-r--r--   0 luke      (1000) luke      (1000)    14121 2023-02-20 15:44:13.000000 pyastgrep-1.1/README.rst
--rw-r--r--   0 luke      (1000) luke      (1000)      755 2023-04-17 15:02:16.000000 pyastgrep-1.1/pyproject.toml
--rw-r--r--   0 luke      (1000) luke      (1000)     1135 2023-06-09 13:42:58.005910 pyastgrep-1.1/setup.cfg
--rw-r--r--   0 luke      (1000) luke      (1000)       38 2022-10-21 16:01:47.000000 pyastgrep-1.1/setup.py
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-06-09 13:42:57.997910 pyastgrep-1.1/src/
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-06-09 13:42:58.001910 pyastgrep-1.1/src/pyastgrep/
--rw-r--r--   0 luke      (1000) luke      (1000)       20 2023-06-09 13:42:38.000000 pyastgrep-1.1/src/pyastgrep/__init__.py
--rw-r--r--   0 luke      (1000) luke      (1000)     3158 2022-11-18 11:57:27.000000 pyastgrep-1.1/src/pyastgrep/asts.py
--rw-r--r--   0 luke      (1000) luke      (1000)     3930 2022-11-16 20:46:57.000000 pyastgrep-1.1/src/pyastgrep/cli.py
--rw-r--r--   0 luke      (1000) luke      (1000)      890 2022-11-25 07:36:32.000000 pyastgrep-1.1/src/pyastgrep/dump.py
--rw-r--r--   0 luke      (1000) luke      (1000)     3244 2023-02-20 15:43:43.000000 pyastgrep-1.1/src/pyastgrep/files.py
--rw-r--r--   0 luke      (1000) luke      (1000)     7934 2023-06-09 13:41:41.000000 pyastgrep-1.1/src/pyastgrep/ignores.py
--rw-r--r--   0 luke      (1000) luke      (1000)     4276 2023-04-17 14:55:13.000000 pyastgrep-1.1/src/pyastgrep/printer.py
--rw-r--r--   0 luke      (1000) luke      (1000)     4207 2023-04-17 14:55:57.000000 pyastgrep-1.1/src/pyastgrep/search.py
--rw-r--r--   0 luke      (1000) luke      (1000)      696 2022-11-14 14:54:35.000000 pyastgrep-1.1/src/pyastgrep/xml.py
--rw-r--r--   0 luke      (1000) luke      (1000)      366 2022-11-06 20:21:35.000000 pyastgrep-1.1/src/pyastgrep/xpath2.py
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-06-09 13:42:58.005910 pyastgrep-1.1/src/pyastgrep.egg-info/
--rw-r-----   0 luke      (1000) luke      (1000)    14968 2023-06-09 13:42:57.000000 pyastgrep-1.1/src/pyastgrep.egg-info/PKG-INFO
--rw-r-----   0 luke      (1000) luke      (1000)      698 2023-06-09 13:42:57.000000 pyastgrep-1.1/src/pyastgrep.egg-info/SOURCES.txt
--rw-r-----   0 luke      (1000) luke      (1000)        1 2023-06-09 13:42:57.000000 pyastgrep-1.1/src/pyastgrep.egg-info/dependency_links.txt
--rw-r-----   0 luke      (1000) luke      (1000)       81 2023-06-09 13:42:57.000000 pyastgrep-1.1/src/pyastgrep.egg-info/entry_points.txt
--rw-r-----   0 luke      (1000) luke      (1000)       58 2023-06-09 13:42:57.000000 pyastgrep-1.1/src/pyastgrep.egg-info/requires.txt
--rw-r-----   0 luke      (1000) luke      (1000)       10 2023-06-09 13:42:57.000000 pyastgrep-1.1/src/pyastgrep.egg-info/top_level.txt
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-06-09 13:42:58.005910 pyastgrep-1.1/tests/
--rw-r--r--   0 luke      (1000) luke      (1000)     6800 2022-11-25 07:33:14.000000 pyastgrep-1.1/tests/test_cli.py
--rw-r--r--   0 luke      (1000) luke      (1000)      733 2022-11-06 19:59:49.000000 pyastgrep-1.1/tests/test_encodings.py
--rw-r--r--   0 luke      (1000) luke      (1000)      648 2022-11-07 12:52:05.000000 pyastgrep-1.1/tests/test_errors.py
--rw-r--r--   0 luke      (1000) luke      (1000)     4093 2023-06-09 13:41:41.000000 pyastgrep-1.1/tests/test_ignores.py
--rw-r--r--   0 luke      (1000) luke      (1000)      449 2022-11-25 08:08:17.000000 pyastgrep-1.1/tests/test_parsing.py
--rw-r--r--   0 luke      (1000) luke      (1000)     2190 2022-11-07 12:01:43.000000 pyastgrep-1.1/tests/test_printing.py
--rw-r--r--   0 luke      (1000) luke      (1000)      410 2023-02-20 15:45:50.000000 pyastgrep-1.1/tests/test_symlinks.py
--rw-r--r--   0 luke      (1000) luke      (1000)     1682 2022-11-07 12:01:43.000000 pyastgrep-1.1/tests/test_xml.py
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-06-21 20:24:35.198377 pyastgrep-1.2/
+-rw-r--r--   0 luke      (1000) luke      (1000)      378 2022-10-17 13:09:58.000000 pyastgrep-1.2/.gitattributes
+-rw-r--r--   0 luke      (1000) luke      (1000)     1771 2022-11-07 12:01:43.000000 pyastgrep-1.2/.gitignore
+-rw-rw-rw-   0 luke      (1000) luke      (1000)    15391 2023-06-21 20:24:35.198377 pyastgrep-1.2/PKG-INFO
+-rw-r--r--   0 luke      (1000) luke      (1000)    14571 2023-06-21 20:21:15.000000 pyastgrep-1.2/README.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)      755 2023-04-17 15:02:16.000000 pyastgrep-1.2/pyproject.toml
+-rw-r--r--   0 luke      (1000) luke      (1000)     1120 2023-06-21 20:24:35.202377 pyastgrep-1.2/setup.cfg
+-rw-r--r--   0 luke      (1000) luke      (1000)       38 2022-10-21 16:01:47.000000 pyastgrep-1.2/setup.py
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-06-21 20:24:35.190377 pyastgrep-1.2/src/
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-06-21 20:24:35.194378 pyastgrep-1.2/src/pyastgrep/
+-rw-r--r--   0 luke      (1000) luke      (1000)       20 2023-06-21 20:24:04.000000 pyastgrep-1.2/src/pyastgrep/__init__.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     1188 2023-06-21 15:46:03.000000 pyastgrep-1.2/src/pyastgrep/ast_compat.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     3158 2022-11-18 11:57:27.000000 pyastgrep-1.2/src/pyastgrep/asts.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     6338 2023-06-21 18:07:13.000000 pyastgrep-1.2/src/pyastgrep/cli.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      890 2022-11-25 07:36:32.000000 pyastgrep-1.2/src/pyastgrep/dump.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     4097 2023-06-21 12:33:14.000000 pyastgrep-1.2/src/pyastgrep/files.py
+-rw-r--r--   0 luke      (1000) luke      (1000)    10840 2023-06-21 10:04:58.000000 pyastgrep-1.2/src/pyastgrep/ignores.py
+-rw-r--r--   0 luke      (1000) luke      (1000)    11507 2023-06-21 19:52:37.000000 pyastgrep-1.2/src/pyastgrep/printer.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     4801 2023-06-21 18:07:13.000000 pyastgrep-1.2/src/pyastgrep/search.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      696 2022-11-14 14:54:35.000000 pyastgrep-1.2/src/pyastgrep/xml.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      366 2022-11-06 20:21:35.000000 pyastgrep-1.2/src/pyastgrep/xpath2.py
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-06-21 20:24:35.194378 pyastgrep-1.2/src/pyastgrep.egg-info/
+-rw-r-----   0 luke      (1000) luke      (1000)    15391 2023-06-21 20:24:35.000000 pyastgrep-1.2/src/pyastgrep.egg-info/PKG-INFO
+-rw-r-----   0 luke      (1000) luke      (1000)      726 2023-06-21 20:24:35.000000 pyastgrep-1.2/src/pyastgrep.egg-info/SOURCES.txt
+-rw-r-----   0 luke      (1000) luke      (1000)        1 2023-06-21 20:24:35.000000 pyastgrep-1.2/src/pyastgrep.egg-info/dependency_links.txt
+-rw-r-----   0 luke      (1000) luke      (1000)       81 2023-06-21 20:24:35.000000 pyastgrep-1.2/src/pyastgrep.egg-info/entry_points.txt
+-rw-r-----   0 luke      (1000) luke      (1000)       58 2023-06-21 20:24:35.000000 pyastgrep-1.2/src/pyastgrep.egg-info/requires.txt
+-rw-r-----   0 luke      (1000) luke      (1000)       10 2023-06-21 20:24:35.000000 pyastgrep-1.2/src/pyastgrep.egg-info/top_level.txt
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-06-21 20:24:35.198377 pyastgrep-1.2/tests/
+-rw-r--r--   0 luke      (1000) luke      (1000)     6529 2023-06-21 08:40:28.000000 pyastgrep-1.2/tests/test_cli.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      733 2022-11-06 19:59:49.000000 pyastgrep-1.2/tests/test_encodings.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      648 2022-11-07 12:52:05.000000 pyastgrep-1.2/tests/test_errors.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     5325 2023-06-21 09:44:46.000000 pyastgrep-1.2/tests/test_ignores.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      449 2022-11-25 08:08:17.000000 pyastgrep-1.2/tests/test_parsing.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     4808 2023-06-21 20:13:30.000000 pyastgrep-1.2/tests/test_printing.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      410 2023-02-20 15:45:50.000000 pyastgrep-1.2/tests/test_symlinks.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     1560 2023-06-21 09:04:52.000000 pyastgrep-1.2/tests/test_xml.py
```

### Comparing `pyastgrep-1.1/.gitignore` & `pyastgrep-1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pyastgrep-1.1/PKG-INFO` & `pyastgrep-1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: pyastgrep
-Version: 1.1
+Version: 1.2
 Summary: A query tool for Python abstract syntax trees
 Home-page: https://github.com/spookylukey/pyastgrep
 Author: Luke Plant
 License: MIT
 Keywords: xpath xml ast asts syntax query css grep
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 
 pyastgrep
 =========
 
 
 .. image:: https://badge.fury.io/py/pyastgrep.svg
@@ -42,15 +42,15 @@
 
 .. contents:: Contents
 
 
 Installation
 ------------
 
-Python 3.7+ required.
+Python 3.8+ required.
 
 We recommend `pipx <https://pipxproject.github.io/pipx/>`_ to install it
 conveniently in an isolated environment:
 
 ::
 
    pipx install pyastgrep
@@ -303,14 +303,30 @@
 do translations before passing to ``pyastgrep``. This tool also supports some
 things that our `cssselect (our dependency) does not yet support
 <https://github.com/scrapy/cssselect/issues>`_.
 
 Tips
 ----
 
+Command line flags
+~~~~~~~~~~~~~~~~~~
+
+There are a growing number of command line flags – see ``pyastgrep --help``
+
+Extracting code snippets
+~~~~~~~~~~~~~~~~~~~~~~~~
+
+If you want to extract standalone snippets of code, try ``--context=statement
+--heading`` which does automatic dedenting. e.g. to extract all functions and
+methods, with leading whitespace removed, do:
+
+.. code-block:: bash
+
+   $ pyastgrep --heading -C statement './/FunctionDef'
+
 Absolute paths
 ~~~~~~~~~~~~~~
 To get pyastgrep to print absolute paths in results, pass the current absolute
 path as the directory to search::
 
   pyastgrep "..." $(pwd)
```

### Comparing `pyastgrep-1.1/README.rst` & `pyastgrep-1.2/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 .. contents:: Contents
 
 
 Installation
 ------------
 
-Python 3.7+ required.
+Python 3.8+ required.
 
 We recommend `pipx <https://pipxproject.github.io/pipx/>`_ to install it
 conveniently in an isolated environment:
 
 ::
 
    pipx install pyastgrep
@@ -281,14 +281,30 @@
 do translations before passing to ``pyastgrep``. This tool also supports some
 things that our `cssselect (our dependency) does not yet support
 <https://github.com/scrapy/cssselect/issues>`_.
 
 Tips
 ----
 
+Command line flags
+~~~~~~~~~~~~~~~~~~
+
+There are a growing number of command line flags – see ``pyastgrep --help``
+
+Extracting code snippets
+~~~~~~~~~~~~~~~~~~~~~~~~
+
+If you want to extract standalone snippets of code, try ``--context=statement
+--heading`` which does automatic dedenting. e.g. to extract all functions and
+methods, with leading whitespace removed, do:
+
+.. code-block:: bash
+
+   $ pyastgrep --heading -C statement './/FunctionDef'
+
 Absolute paths
 ~~~~~~~~~~~~~~
 To get pyastgrep to print absolute paths in results, pass the current absolute
 path as the directory to search::
 
   pyastgrep "..." $(pwd)
```

### Comparing `pyastgrep-1.1/pyproject.toml` & `pyastgrep-1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyastgrep-1.1/setup.cfg` & `pyastgrep-1.2/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 author = Luke Plant
 url = https://github.com/spookylukey/pyastgrep
 keywords = xpath xml ast asts syntax query css grep
 classifiers = 
 	Development Status :: 4 - Beta
 	Programming Language :: Python
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Intended Audience :: Developers
 	Operating System :: OS Independent
 	License :: OSI Approved :: MIT License
 	Natural Language :: English
 
 [options]
 packages = find:
 package_dir = =src
+python_requires = >=3.8
 install_requires = 
 	lxml>=3.3.5
 	elementpath
 	astpretty
 	pathspec
 	cssselect>=1.2
```

### Comparing `pyastgrep-1.1/src/pyastgrep/asts.py` & `pyastgrep-1.2/src/pyastgrep/asts.py`

 * *Files identical despite different names*

### Comparing `pyastgrep-1.1/src/pyastgrep/dump.py` & `pyastgrep-1.2/src/pyastgrep/dump.py`

 * *Files identical despite different names*

### Comparing `pyastgrep-1.1/src/pyastgrep/files.py` & `pyastgrep-1.2/src/pyastgrep/files.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,21 +6,40 @@
 from dataclasses import dataclass
 from pathlib import Path
 from typing import BinaryIO, Generator, Sequence
 
 from .ignores import DirWalker
 
 
-@dataclass
+@dataclass(frozen=True)
 class MissingPath:
     path: Path
 
 
-def get_files_to_search(paths: Sequence[Path | BinaryIO]) -> Generator[Path | BinaryIO | MissingPath, None, None]:
-    walker = DirWalker(glob="*.py")
+def get_files_to_search(
+    paths: Sequence[Path | BinaryIO],
+    include_hidden: bool = False,
+    respect_global_ignores: bool = True,
+    respect_vcs_ignores: bool = True,
+) -> Generator[Path | BinaryIO | MissingPath, None, None]:
+    """
+    Entry-point function for finding files to search.
+
+    By default, POSIX hidden files (starting with `.`) will be skipped - pass
+    `include_hidden=True` to include them.
+
+    By default, global .gitignore file will be respected - pass
+    `respect_global_ignores=False` to ignore it
+    """
+    walker = DirWalker(
+        glob="*.py",
+        include_hidden=include_hidden,
+        respect_global_ignores=respect_global_ignores,
+        respect_vcs_ignores=respect_vcs_ignores,
+    )
     working_dir = Path(os.getcwd())
     for path in paths:
         if isinstance(path, Path):
             if not path.exists():
                 yield MissingPath(path)
             elif path.is_file():
                 yield path
@@ -53,19 +72,27 @@
         if linebreak_idx < 0:
             break
         else:
             current_idx = linebreak_idx + 1
     return "utf-8"
 
 
-def parse_python_file(contents: bytes, filename: str | Path, *, auto_dedent: bool) -> tuple[str, ast.AST]:
+def parse_python_file(
+    contents: bytes, filename: str | Path, *, auto_dedent: bool, add_ast_parent_nodes: bool = False
+) -> tuple[str, ast.AST]:
     if auto_dedent:
         contents = auto_dedent_code(contents)
 
     parsed_ast: ast.AST = ast.parse(contents, str(filename))
+    if add_ast_parent_nodes:
+        # Needed for StatementContext
+        for node in ast.walk(parsed_ast):
+            for child in ast.iter_child_nodes(node):
+                child.parent = node  # type: ignore
+
     # ast.parse does it's own encoding detection, which we have to replicate
     # here since we can't assume utf-8
     encoding = get_encoding(contents)
     str_contents = contents.decode(encoding)
     return str_contents, parsed_ast
```

### Comparing `pyastgrep-1.1/src/pyastgrep/ignores.py` & `pyastgrep-1.2/src/pyastgrep/ignores.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,37 @@
+"""
+Directory walker, with smart behaviour for ignoring files.
+
+This is based on ripgrep behaviour:
+
+- Automatically respect global and local `.gitignore` files
+- Automatically ignore hidden files
+
+With some known differences/unimplemented features/bugs:
+
+- doesn't yet support `.ignore` files
+- ripgrep does not respect `.gitignore` files if the starting directory is outside a git repo
+  https://github.com/BurntSushi/ripgrep/issues/1109 but we do
+- ripgrep considers Windows files with hidden attribute to be hidden, we do not yet.
+- if starting inside hidden folders, we return nothing by default because the parent is hidden,
+  but ripgrep doesn't do this.
+
+"""
 from __future__ import annotations
 
+import logging
 import subprocess
 from pathlib import Path
-from typing import Generator, Union, overload
+from typing import Any, Generator, Union, overload
 
 from pathspec import GitIgnoreSpec, PathSpec
 from pathspec.patterns.gitwildmatch import GitWildMatchPattern
 
+logger = logging.getLogger(__name__)
+
 
 class DirectoryPathSpec:
     """
     PathSpec object for a specific directory.
     """
 
     # We have to keep track of the location of a .gitignore file, as well as
@@ -33,18 +54,35 @@
             # .gitignore file correctly if we don't know where the file
             # is relative to it?
             # Rather than crash, we ignore the file
             return False
         else:
             return self.pathspec.match_file(relative)
 
+    def __repr__(self) -> str:
+        return f"<DirectoryPathSpec {self.location!r} {self.pathspec!r}>"
+
+
+class GlobalGitIgnoreSpec(GitIgnoreSpec):
+    # This subclass exists currently only for the sake of debugging
+    pass
+
 
 PathSpecLike = Union[PathSpec, DirectoryPathSpec]
 
 
+class _Default:
+    """
+    Sentinel for default values to function/method args
+    """
+
+
+DEFAULT: Any = _Default()
+
+
 @overload
 def add_negative_dir_pattern(pathspec: PathSpec, directory: Path) -> PathSpec:
     pass
 
 
 @overload
 def add_negative_dir_pattern(pathspec: DirectoryPathSpec, directory: Path) -> DirectoryPathSpec:
@@ -63,56 +101,68 @@
     while automatically respecting dot-ignore files
     """
 
     def __init__(
         self,
         *,
         glob: str,
-        pathspecs: list[PathSpecLike] | None = None,
+        pathspecs: list[PathSpecLike] = DEFAULT,
         init_global_pathspecs: bool = True,
         start_directory: Path | None = None,
         working_dir: Path | None = None,
         absolute_base: bool = False,
+        include_hidden: bool = False,
+        respect_global_ignores: bool = True,
+        respect_vcs_ignores: bool = True,
     ):
         # DirWalker is immutable outside __init__
         self.glob: str = glob
-        if pathspecs is None:
+        if pathspecs is DEFAULT:
             pathspecs = []
         if init_global_pathspecs:
-            global_gitignore = get_global_gitignore()
-            if global_gitignore and global_gitignore.exists():
-                pathspecs.append(pathspec_for_gitignore(global_gitignore, is_global_gitignore=True))
+            if respect_global_ignores:
+                if respect_vcs_ignores:
+                    global_gitignore = get_global_gitignore()
+                    if global_gitignore and global_gitignore.exists():
+                        pathspecs.append(pathspec_for_gitignore(global_gitignore, is_global_gitignore=True))
             # POSIX hidden files:
-            pathspecs.append(PathSpec([GitWildMatchPattern(".*")]))
+            if not include_hidden:
+                # TODO we should probably use a different mechanism for hidden
+                # files, this causes problems and doesn't cope with Windows
+                # hidden files.
+                pathspecs.append(PathSpec([GitWildMatchPattern(".*")]))
         self.pathspecs: list[PathSpecLike] = pathspecs
         self.start_directory: Path | None = start_directory
-        self.working_dir = working_dir
+        self.working_dir: Path | None = working_dir
         self.absolute_base: bool = absolute_base
+        self.respect_vcs_ignores: bool = respect_vcs_ignores
 
     def for_dir(self, directory: Path, working_dir: Path) -> DirWalker:
         """
         Return a new DirWalker, customised for the directory.
         """
         # Here we keep the already loaded global gitignore, and add any
         # more needed, up to and including the current directory.
         base_directory = directory.resolve()
-        pathspecs = self.pathspecs + [
-            pathspec_for_gitignore(ignorepath) for ignorepath in find_gitignore_files(base_directory, recurse_up=True)
-        ]
+        if self.respect_vcs_ignores:
+            pathspecs = self.pathspecs + [
+                pathspec_for_gitignore(ignorepath)
+                for ignorepath in find_gitignore_files(base_directory, recurse_up=True)
+            ]
+        else:
+            pathspecs = self.pathspecs
         # We also need to add a negative override to ensure that paths specified
         # directly are not ignored.
         if directory != Path("."):
             # TODO this doesn't work in all cases, e.g. if an exclude is specified
             # in a subdirectory `.gitignore` which matches the passed in directory.
             pathspecs = [add_negative_dir_pattern(pathspec, directory) for pathspec in pathspecs]
 
-        return DirWalker(
-            glob=self.glob,
+        return self._clone(
             pathspecs=pathspecs,
-            init_global_pathspecs=False,
             start_directory=base_directory,
             working_dir=working_dir,
             absolute_base=directory.is_absolute(),
         )
 
     def for_subdir(self, directory: Path) -> DirWalker:
         """
@@ -120,58 +170,88 @@
         the directory the parent current walker is for.
         """
         # This is distinct from `for_dir`, so that we can re-use the work
         # that has already been done in checking parent dirs for .gitignore files,
         # and just check the new current dir.
         if self.start_directory is None:
             raise AssertionError("Must use `for_dir` before `for_subdir`")
-        extra_pathspecs: list[PathSpecLike] = [
-            pathspec_for_gitignore(ignorepath) for ignorepath in find_gitignore_files(directory, recurse_up=False)
-        ]
+        if self.respect_vcs_ignores:
+            extra_pathspecs: list[PathSpecLike] = [
+                pathspec_for_gitignore(ignorepath) for ignorepath in find_gitignore_files(directory, recurse_up=False)
+            ]
+        else:
+            extra_pathspecs = []
 
-        return DirWalker(
-            glob=self.glob,
+        return self._clone(
             pathspecs=self.pathspecs + extra_pathspecs,
-            init_global_pathspecs=False,
             start_directory=directory,
-            working_dir=self.working_dir,
-            absolute_base=self.absolute_base,
         )
 
     def walk(self) -> Generator[Path, None, None]:
         if self.start_directory is None or self.working_dir is None:
             raise AssertionError("Must use `for_dir` before `walk`")
         for filepath in self.start_directory.glob(self.glob):
             if filepath.is_symlink():
                 # Follow default behaviour of ripgrep, and avoid issues with
                 # `resolve().relative_to(working_dir)
+                logger.debug("Ignoring symlink %s", filepath)
                 continue
             if filepath.is_file():
-                if any(pathspec.match_file(filepath) for pathspec in self.pathspecs):
+                pathspec_matched = False
+                for pathspec in self.pathspecs:
+                    if pathspec.match_file(filepath):
+                        pathspec_matched = True
+                        logger.debug("Ignoring path %s because it matches pathspec %s", filepath, pathspec)
+                        break
+                if pathspec_matched:
                     continue
                 if self.absolute_base:
                     yield filepath
                 else:
                     yield filepath.resolve().relative_to(self.working_dir)
         for subdir in self.start_directory.iterdir():
             if subdir.is_symlink():
+                logger.debug("Ignoring symlink %s", subdir)
                 continue
             if subdir.is_dir():
-                if any(pathspec.match_file(subdir) for pathspec in self.pathspecs):
+                pathspec_matched = False
+                for pathspec in self.pathspecs:
+                    if pathspec.match_file(subdir):
+                        pathspec_matched = True
+                        logger.debug("Ignoring path %s because it matches pathspec %s", subdir, pathspec)
+                        break
+                if pathspec_matched:
                     continue
                 yield from self.for_subdir(subdir).walk()
 
+    def _clone(
+        self,
+        *,
+        pathspecs: list[PathSpecLike],
+        start_directory: Path,
+        working_dir: Path = DEFAULT,
+        absolute_base: bool = DEFAULT,
+    ) -> DirWalker:
+        return DirWalker(
+            glob=self.glob,
+            pathspecs=pathspecs,
+            init_global_pathspecs=False,
+            start_directory=start_directory,
+            working_dir=self.working_dir if working_dir is DEFAULT else working_dir,
+            absolute_base=self.absolute_base if absolute_base is DEFAULT else absolute_base,
+            respect_vcs_ignores=self.respect_vcs_ignores,
+        )
+
 
 def pathspec_for_gitignore(gitignore_file: Path, is_global_gitignore: bool = False) -> PathSpec | DirectoryPathSpec:
     with open(gitignore_file) as fp:
-        spec = GitIgnoreSpec.from_lines(fp)
         if is_global_gitignore:
-            return spec
+            return GlobalGitIgnoreSpec.from_lines(fp)
         else:
-            return DirectoryPathSpec(gitignore_file.parent, spec)
+            return DirectoryPathSpec(gitignore_file.parent, GitIgnoreSpec.from_lines(fp))
 
 
 def find_gitignore_files(starting_path: Path, *, recurse_up: bool = True) -> list[Path]:
     """
     For a given working dir, returns a list of .gitignore files
     that apply to it.
     """
```

### Comparing `pyastgrep-1.1/src/pyastgrep/search.py` & `pyastgrep-1.2/src/pyastgrep/search.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,43 +18,52 @@
     Pathlike = Path | Literal["<stdin>"]
 else:
     # `|` not supported on older Python versions we support,
     # and Literal is only available in Python 3.8+
     Pathlike = Path
 
 
-@dataclass
+@dataclass(frozen=True)
 class Match:
     path: Pathlike
     file_lines: list[str]
     xml_element: _Element
     position: Position
     ast_node: ast.AST
 
     @property
     def matching_line(self) -> str:
         return self.file_lines[self.position.lineno - 1]
 
 
-@dataclass
+@dataclass(frozen=True)
 class Position:
     lineno: int  # 1-indexed, as per AST
     col_offset: int  # 0-indexed, as per AST
 
 
-@dataclass
+@dataclass(frozen=True)
 class ReadError:
     path: str
     exception: Exception
 
 
 class NonElementReturned(ValueError):
     pass
 
 
+@dataclass(frozen=True)
+class FileFinished:
+    """
+    Sentinel used for flushing output
+    """
+
+    path: Pathlike
+
+
 def position_from_xml(element: _Element, node_mappings: dict[_Element, ast.AST] | None = None) -> Position | None:
     if not hasattr(element, "xpath"):
         # Most likely an _ElementUnicodeResult, the result of a query that terminated in
         # an attribute rather than a node. We have no way of getting from here to
         # something representing an AST node.
         raise NonElementReturned(element)
     try:
@@ -76,25 +85,34 @@
         return xml.lxml_query
 
 
 def search_python_files(
     paths: Sequence[Path | BinaryIO],
     expression: str,
     xpath2: bool = False,
-) -> Generator[Match | MissingPath | ReadError | NonElementReturned, None, None]:
+    include_hidden: bool = False,
+    respect_global_ignores: bool = True,
+    respect_vcs_ignores: bool = True,
+    add_ast_parent_nodes: bool = False,
+) -> Generator[Match | MissingPath | ReadError | NonElementReturned | FileFinished, None, None]:
     """
     Perform a recursive search through Python files.
 
     Paths may include directories, e.g "." for the current directory.
     .gitignore rules will be applied automatically.
 
     """
     query_func = get_query_func(xpath2=xpath2)
 
-    for path in get_files_to_search(paths):
+    for path in get_files_to_search(
+        paths,
+        include_hidden=include_hidden,
+        respect_global_ignores=respect_global_ignores,
+        respect_vcs_ignores=respect_vcs_ignores,
+    ):
         node_mappings: dict[_Element, ast.AST] = {}
         source: Pathlike
         auto_dedent = False
         if isinstance(path, MissingPath):
             yield path
             continue
         elif isinstance(path, Path):
@@ -106,15 +124,17 @@
                 continue
         else:
             source = "<stdin>"
             contents = path.read()
             auto_dedent = True
 
         try:
-            str_contents, parsed_ast = parse_python_file(contents, source, auto_dedent=auto_dedent)
+            str_contents, parsed_ast = parse_python_file(
+                contents, source, auto_dedent=auto_dedent, add_ast_parent_nodes=add_ast_parent_nodes
+            )
         except SyntaxError as ex:
             yield ReadError(str(source), ex)
             continue
 
         file_lines = str_contents.splitlines()
         xml_ast = ast_to_xml(
             parsed_ast,
@@ -134,7 +154,9 @@
             try:
                 position = position_from_xml(element, node_mappings=node_mappings)
             except NonElementReturned as ex:
                 position = None
                 yield ex
             if position is not None and ast_node is not None:
                 yield Match(source, file_lines, element, position, ast_node)
+
+        yield FileFinished(source)
```

### Comparing `pyastgrep-1.1/src/pyastgrep/xml.py` & `pyastgrep-1.2/src/pyastgrep/xml.py`

 * *Files identical despite different names*

### Comparing `pyastgrep-1.1/src/pyastgrep.egg-info/PKG-INFO` & `pyastgrep-1.2/src/pyastgrep.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: pyastgrep
-Version: 1.1
+Version: 1.2
 Summary: A query tool for Python abstract syntax trees
 Home-page: https://github.com/spookylukey/pyastgrep
 Author: Luke Plant
 License: MIT
 Keywords: xpath xml ast asts syntax query css grep
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 
 pyastgrep
 =========
 
 
 .. image:: https://badge.fury.io/py/pyastgrep.svg
@@ -42,15 +42,15 @@
 
 .. contents:: Contents
 
 
 Installation
 ------------
 
-Python 3.7+ required.
+Python 3.8+ required.
 
 We recommend `pipx <https://pipxproject.github.io/pipx/>`_ to install it
 conveniently in an isolated environment:
 
 ::
 
    pipx install pyastgrep
@@ -303,14 +303,30 @@
 do translations before passing to ``pyastgrep``. This tool also supports some
 things that our `cssselect (our dependency) does not yet support
 <https://github.com/scrapy/cssselect/issues>`_.
 
 Tips
 ----
 
+Command line flags
+~~~~~~~~~~~~~~~~~~
+
+There are a growing number of command line flags – see ``pyastgrep --help``
+
+Extracting code snippets
+~~~~~~~~~~~~~~~~~~~~~~~~
+
+If you want to extract standalone snippets of code, try ``--context=statement
+--heading`` which does automatic dedenting. e.g. to extract all functions and
+methods, with leading whitespace removed, do:
+
+.. code-block:: bash
+
+   $ pyastgrep --heading -C statement './/FunctionDef'
+
 Absolute paths
 ~~~~~~~~~~~~~~
 To get pyastgrep to print absolute paths in results, pass the current absolute
 path as the directory to search::
 
   pyastgrep "..." $(pwd)
```

### Comparing `pyastgrep-1.1/src/pyastgrep.egg-info/SOURCES.txt` & `pyastgrep-1.2/src/pyastgrep.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 .gitattributes
 .gitignore
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
 src/pyastgrep/__init__.py
+src/pyastgrep/ast_compat.py
 src/pyastgrep/asts.py
 src/pyastgrep/cli.py
 src/pyastgrep/dump.py
 src/pyastgrep/files.py
 src/pyastgrep/ignores.py
 src/pyastgrep/printer.py
 src/pyastgrep/search.py
```

### Comparing `pyastgrep-1.1/tests/test_cli.py` & `pyastgrep-1.2/tests/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from __future__ import annotations
 
 import io
-import re
 import subprocess
-import sys
 from pathlib import Path
 
 import pytest
 
 from pyastgrep.cli import main
 from tests.utils import chdir
 
@@ -134,17 +132,14 @@
         end_col_offset=5,
         left=Name(lineno=1, col_offset=0, end_lineno=1, end_col_offset=1, id='a', ctx=Load()),
         op=Add(),
         right=Name(lineno=1, col_offset=4, end_lineno=1, end_col_offset=5, id='b', ctx=Load()),
     ),
 )
 """
-    if sys.version_info < (3, 8):
-        # Python 3.7 doesn't return end info
-        expected, _ = re.subn(r" *end_(lineno|col_offset)=\d+,\n?", "", expected)
     assert_output(
         capsys,
         ["--ast", "./*/*", "-"],
         stdin="a + b",
         equals=expected,
     )
 
@@ -200,15 +195,14 @@
 for item in items:
     pass
 """.strip(),
         error_equals="Invalid CSS selector: .//For/Name\n",
     )
 
 
-@pytest.mark.skipif(sys.version_info < (3, 8), reason="Python 3.7 has different output")
 def test_pyastdump_stdin():
     result = subprocess.run("echo 'x = 1' | pyastdump -", shell=True, capture_output=True)
     assert result.returncode == 0
     assert result.stderr == b""
     assert result.stdout == (
         b"<Module>\n"
         b"  <body>\n"
```

### Comparing `pyastgrep-1.1/tests/test_encodings.py` & `pyastgrep-1.2/tests/test_encodings.py`

 * *Files identical despite different names*

### Comparing `pyastgrep-1.1/tests/test_errors.py` & `pyastgrep-1.2/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `pyastgrep-1.1/tests/test_ignores.py` & `pyastgrep-1.2/tests/test_ignores.py`

 * *Files 22% similar despite different names*

```diff
@@ -44,43 +44,70 @@
         "node_modules/subdir/should_be_ignored.py",
         # custom_gitignored is in this subdir's .gitignore
         "custom_gitignored/__init__.py",
         "custom_gitignored/should_be_ignored2.py",
         "custom_gitignored/subdir/should_be_ignored2.py",
         # /subsubdir is in this subdir's .gitignore
         "subsubdir/not_ignored.py",
+        # should_be_ignored.py is in subsubdir's .gitignore
+        "subdir/subsubdir/should_be_ignored.py",
+        # globalignored is in our 'global' .gitgnore (global_gitignore_file, monkeypatched below)
+        "global_ignored/should_be_ignored.py",
     ]
 
+    with patch("pyastgrep.ignores.get_global_gitignore", lambda: DIR / "global_gitignore_file"):
+        with chdir(DIR):
+            files = list(get_files_to_search([Path(".")]))
+
+        for p in FOUND:
+            assert Path(p) in files
+
+        for p in IGNORED:
+            # Sanity check:
+            assert (DIR / Path(p)).exists()
+            # Test:
+            assert Path(p) not in files
+
+        # We should get the same results if we start the search higher up.
+        # This is important for testing whether we are discovering .gitignore
+        # files as we walk sub directories
+
+        with chdir(REPO_ROOT):
+            files2 = list(get_files_to_search([Path(".")]))
+
+        for p in FOUND:
+            assert (DIR_FROM_ROOT / Path(p)) in files2
+
+        for p in IGNORED:
+            # Sanity check:
+            assert (DIR / Path(p)).exists()
+            # Test:
+            assert (DIR_FROM_ROOT / Path(p)) not in files2
+
+
+def test_include_hidden():
     with chdir(DIR):
-        files = list(get_files_to_search([Path(".")]))
+        assert Path(".custom_hidden/should_be_ignored.py") in list(
+            get_files_to_search([Path(".")], include_hidden=True)
+        )
+
 
-    for p in FOUND:
-        assert Path(p) in files
+def test_respect_global_ignores():
+    with patch("pyastgrep.ignores.get_global_gitignore", lambda: DIR / "global_gitignore_file"):
+        with chdir(DIR):
+            assert Path("global_ignored/should_be_ignored.py") in list(
+                get_files_to_search([Path(".")], respect_global_ignores=False)
+            )
 
-    for p in IGNORED:
-        # Sanity check:
-        assert (DIR / Path(p)).exists()
-        # Test:
-        assert Path(p) not in files
-
-    # We should get the same results if we start the search higher up.
-    # This is important for testing whether we are discovering .gitignore
-    # files as we walk sub directories
-
-    with chdir(REPO_ROOT):
-        files2 = list(get_files_to_search([Path(".")]))
-
-    for p in FOUND:
-        assert (DIR_FROM_ROOT / Path(p)) in files2
-
-    for p in IGNORED:
-        # Sanity check:
-        assert (DIR / Path(p)).exists()
-        # Test:
-        assert (DIR_FROM_ROOT / Path(p)) not in files2
+
+def test_respect_vcs_ignores():
+    with chdir(DIR):
+        files = list(get_files_to_search([Path(".")], respect_vcs_ignores=False))
+        assert Path("custom_gitignored/should_be_ignored2.py") in files
+        assert Path("subdir/subsubdir/should_be_ignored.py") in files
 
 
 def test_override_on_cli():
     """
     Directories specified on command line should always be searched.
     """
     with chdir(DIR):
```

### Comparing `pyastgrep-1.1/tests/test_xml.py` & `pyastgrep-1.2/tests/test_xml.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,18 @@
-import sys
 from pathlib import Path
 
 from tests.utils import run_print
 
 DIR = Path(__file__).parent / "examples" / "test_xml"
 
 
 def test_literals():
     # We need a way to distinguish between different literals
-    if sys.version_info < (3, 8):
-        expr_int = ".//Num"
-        expr_string = ".//Str"
-    else:
-        expr_int = './/Constant[@type="int"]'
-        expr_string = './/Constant[@type="str"]'
+    expr_int = './/Constant[@type="int"]'
+    expr_string = './/Constant[@type="str"]'
 
     output_int = run_print(DIR, expr_int, print_xml=True).stdout
     output_string = run_print(DIR, expr_string, print_xml=True).stdout
     assert "assigned_int" in output_int
     assert "assigned_string" not in output_int
 
     assert "assigned_int" not in output_string
```

