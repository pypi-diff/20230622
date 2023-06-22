# Comparing `tmp/uproot_browser-0.6.3.tar.gz` & `tmp/uproot_browser-0.6.4.tar.gz`

## Comparing `uproot_browser-0.6.3.tar` & `uproot_browser-0.6.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/noxfile.py
--rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/.github/dependabot.yml
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/.github/workflows/ci.yml
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/docs/make_logo.py
--rw-r--r--   0        0        0    71775 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/docs/_images/iterm.png
--rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/docs/_images/uproot-browser-logo.png
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/src/uproot_browser/__init__.py
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/src/uproot_browser/__main__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/src/uproot_browser/_version.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/src/uproot_browser/_version.pyi
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/src/uproot_browser/dirs.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/src/uproot_browser/exceptions.py
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/src/uproot_browser/plot.py
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/src/uproot_browser/plot_mpl.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/src/uproot_browser/py.typed
--rw-r--r--   0        0        0     5650 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/src/uproot_browser/tree.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/src/uproot_browser/_compat/__init__.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/src/uproot_browser/_compat/typing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/src/uproot_browser/_compat/importlib/__init__.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/src/uproot_browser/_compat/importlib/resources.py
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/src/uproot_browser/tui/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/src/uproot_browser/tui/__init__.py
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/src/uproot_browser/tui/browser.css
--rw-r--r--   0        0        0     5398 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/src/uproot_browser/tui/browser.py
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/src/uproot_browser/tui/header.py
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/src/uproot_browser/tui/help.py
--rw-r--r--   0        0        0     4232 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/src/uproot_browser/tui/left_panel.py
--rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/src/uproot_browser/tui/right_panel.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/tests/constraints.txt
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/tests/test_dirs.py
--rw-r--r--   0        0        0     4000 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/tests/test_printouts.py
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/tests/test_tui.py
--rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/.gitignore
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/LICENSE
--rw-r--r--   0        0        0    10628 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/README.md
--rw-r--r--   0        0        0     4248 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/pyproject.toml
--rw-r--r--   0        0        0    14323 2020-02-02 00:00:00.000000 uproot_browser-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 uproot_browser-0.6.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 uproot_browser-0.6.4/noxfile.py
+-rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 uproot_browser-0.6.4/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 uproot_browser-0.6.4/.github/dependabot.yml
+-rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 uproot_browser-0.6.4/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 uproot_browser-0.6.4/docs/make_logo.py
+-rw-r--r--   0        0        0    71775 2020-02-02 00:00:00.000000 uproot_browser-0.6.4/docs/_images/iterm.png
+-rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 uproot_browser-0.6.4/docs/_images/uproot-browser-logo.png
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 uproot_browser-0.6.4/src/uproot_browser/__init__.py
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 uproot_browser-0.6.4/src/uproot_browser/__main__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 uproot_browser-0.6.4/src/uproot_browser/_version.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 uproot_browser-0.6.4/src/uproot_browser/_version.pyi
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 uproot_browser-0.6.4/src/uproot_browser/dirs.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 uproot_browser-0.6.4/src/uproot_browser/exceptions.py
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 uproot_browser-0.6.4/src/uproot_browser/plot.py
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 uproot_browser-0.6.4/src/uproot_browser/plot_mpl.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uproot_browser-0.6.4/src/uproot_browser/py.typed
+-rw-r--r--   0        0        0     5650 2020-02-02 00:00:00.000000 uproot_browser-0.6.4/src/uproot_browser/tree.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uproot_browser-0.6.4/src/uproot_browser/_compat/__init__.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 uproot_browser-0.6.4/src/uproot_browser/_compat/typing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uproot_browser-0.6.4/src/uproot_browser/_compat/importlib/__init__.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 uproot_browser-0.6.4/src/uproot_browser/_compat/importlib/resources.py
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 uproot_browser-0.6.4/src/uproot_browser/tui/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uproot_browser-0.6.4/src/uproot_browser/tui/__init__.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 uproot_browser-0.6.4/src/uproot_browser/tui/browser.css
+-rw-r--r--   0        0        0     5400 2020-02-02 00:00:00.000000 uproot_browser-0.6.4/src/uproot_browser/tui/browser.py
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 uproot_browser-0.6.4/src/uproot_browser/tui/header.py
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 uproot_browser-0.6.4/src/uproot_browser/tui/help.py
+-rw-r--r--   0        0        0     4205 2020-02-02 00:00:00.000000 uproot_browser-0.6.4/src/uproot_browser/tui/left_panel.py
+-rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 uproot_browser-0.6.4/src/uproot_browser/tui/right_panel.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 uproot_browser-0.6.4/tests/constraints.txt
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 uproot_browser-0.6.4/tests/test_dirs.py
+-rw-r--r--   0        0        0     4000 2020-02-02 00:00:00.000000 uproot_browser-0.6.4/tests/test_printouts.py
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 uproot_browser-0.6.4/tests/test_tui.py
+-rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 uproot_browser-0.6.4/.gitignore
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 uproot_browser-0.6.4/LICENSE
+-rw-r--r--   0        0        0    10628 2020-02-02 00:00:00.000000 uproot_browser-0.6.4/README.md
+-rw-r--r--   0        0        0     4268 2020-02-02 00:00:00.000000 uproot_browser-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0    14369 2020-02-02 00:00:00.000000 uproot_browser-0.6.4/PKG-INFO
```

### Comparing `uproot_browser-0.6.3/.pre-commit-config.yaml` & `uproot_browser-0.6.4/.pre-commit-config.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -15,28 +15,33 @@
   - id: debug-statements
   - id: end-of-file-fixer
   - id: mixed-line-ending
   - id: requirements-txt-fixer
   - id: trailing-whitespace
 
 - repo: https://github.com/charliermarsh/ruff-pre-commit
-  rev: "v0.0.265"
+  rev: "v0.0.272"
   hooks:
     - id: ruff
       args: ["--fix", "--show-fixes"]
 
 - repo: https://github.com/pre-commit/mirrors-mypy
-  rev: v1.2.0
+  rev: v1.3.0
   hooks:
   - id: mypy
     files: src
-    additional_dependencies: [rich>=12, click>=8.1.1, hist, numpy, textual>=0.24]
+    additional_dependencies:
+    - rich>=12
+    - click>=8.1.1
+    - hist
+    - numpy
+    - textual>=0.27
 
 - repo: https://github.com/codespell-project/codespell
-  rev: v2.2.4
+  rev: v2.2.5
   hooks:
   - id: codespell
     args: [-L, "hist,iterm"]
 
 - repo: local
   hooks:
   - id: disallow-caps
```

### Comparing `uproot_browser-0.6.3/noxfile.py` & `uproot_browser-0.6.4/noxfile.py`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.3/.github/CONTRIBUTING.md` & `uproot_browser-0.6.4/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.3/.github/workflows/ci.yml` & `uproot_browser-0.6.4/.github/workflows/ci.yml`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,14 @@
     - uses: pre-commit/action@v3.0.0
     - name: PyLint
       run: pipx run nox -s pylint
 
   checks:
     name: Check Python ${{ matrix.python-version }} on ${{ matrix.runs-on }}
     runs-on: ${{ matrix.runs-on }}
-    needs: [pre-commit]
     strategy:
       fail-fast: false
       matrix:
         python-version: ["3.7", "3.11"]
         runs-on: [ubuntu-latest, macos-latest, windows-latest]
 
         include:
```

### Comparing `uproot_browser-0.6.3/docs/make_logo.py` & `uproot_browser-0.6.4/docs/make_logo.py`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.3/docs/_images/iterm.png` & `uproot_browser-0.6.4/docs/_images/iterm.png`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.3/docs/_images/uproot-browser-logo.png` & `uproot_browser-0.6.4/docs/_images/uproot-browser-logo.png`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.3/src/uproot_browser/__main__.py` & `uproot_browser-0.6.4/src/uproot_browser/__main__.py`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.3/src/uproot_browser/dirs.py` & `uproot_browser-0.6.4/src/uproot_browser/dirs.py`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.3/src/uproot_browser/plot.py` & `uproot_browser-0.6.4/src/uproot_browser/plot.py`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.3/src/uproot_browser/plot_mpl.py` & `uproot_browser-0.6.4/src/uproot_browser/plot_mpl.py`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.3/src/uproot_browser/tree.py` & `uproot_browser-0.6.4/src/uproot_browser/tree.py`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.3/src/uproot_browser/tui/README.md` & `uproot_browser-0.6.4/src/uproot_browser/tui/README.md`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.3/src/uproot_browser/tui/browser.css` & `uproot_browser-0.6.4/src/uproot_browser/tui/browser.css`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.3/src/uproot_browser/tui/browser.py` & `uproot_browser-0.6.4/src/uproot_browser/tui/browser.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     LogoWidget,
     Plotext,
     PlotWidget,
     make_plot,
 )
 
 
-class Browser(textual.app.App[None]):
+class Browser(textual.app.App[object]):
     """A basic implementation of the uproot-browser TUI"""
 
     CSS_PATH = "browser.css"
     BINDINGS = [
         textual.binding.Binding("b", "toggle_files", "Navbar"),
         textual.binding.Binding("q", "quit", "Quit"),
         textual.binding.Binding("d", "quit_with_dump", "Dump & Quit"),
```

### Comparing `uproot_browser-0.6.3/src/uproot_browser/tui/header.py` & `uproot_browser-0.6.4/src/uproot_browser/tui/header.py`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.3/src/uproot_browser/tui/help.py` & `uproot_browser-0.6.4/src/uproot_browser/tui/help.py`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.3/src/uproot_browser/tui/left_panel.py` & `uproot_browser-0.6.4/src/uproot_browser/tui/left_panel.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,23 +53,22 @@
 
         label = rich.text.Text.assemble(label_icon, meta["label_text"])
         label.stylize(style)
         return label
 
     def on_mount(self) -> None:
         self.load_directory(self.root)
+        self.root.expand()
 
     def load_directory(self, node: textual.widgets.tree.TreeNode[UprootEntry]) -> None:
         assert node.data
         if not node.children:
             children = node.data.children
             for child in children:
                 node.add(child.path, child)
-        node.expand()
-        self.refresh(layout=True)
 
     def on_tree_node_selected(
         self, event: textual.widgets.Tree.NodeSelected[UprootEntry]
     ) -> None:
         event.stop()
         item = event.node.data
         assert item
@@ -85,27 +84,27 @@
         if item.is_dir:
             self.load_directory(event.node)
 
     def _node_expanded(
         self, node: textual.widgets.tree.TreeNode[UprootEntry]
     ) -> textual.widgets.Tree.NodeExpanded[UprootEntry]:
         try:
-            return self.NodeExpanded(self, node)
-        except TypeError:  # textual < 0.24
-            # pylint: disable-next=(no-value-for-parameter)
-            return self.NodeExpanded(node)  # type:ignore[call-arg,arg-type]
+            return self.NodeExpanded(node)
+        except TypeError:  # textual 0.24-0.26
+            # pylint: disable-next=too-many-function-args
+            return self.NodeExpanded(self, node)  # type:ignore[call-arg,arg-type]
 
     def _node_collapsed(
         self, node: textual.widgets.tree.TreeNode[UprootEntry]
     ) -> textual.widgets.Tree.NodeCollapsed[UprootEntry]:
         try:
-            return self.NodeCollapsed(self, node)
-        except TypeError:  # textual < 0.24
-            # pylint: disable-next=(no-value-for-parameter)
-            return self.NodeCollapsed(node)  # type:ignore[call-arg,arg-type]
+            return self.NodeCollapsed(node)
+        except TypeError:  # textual 0.24-0.26
+            # pylint: disable-next=too-many-function-args
+            return self.NodeCollapsed(self, node)  # type:ignore[call-arg,arg-type]
 
     def action_cursor_in(self) -> None:
         node = self.cursor_node
         if node is None:
             return
         if node.allow_expand and not node.is_expanded:
             node.expand()
```

### Comparing `uproot_browser-0.6.3/src/uproot_browser/tui/right_panel.py` & `uproot_browser-0.6.4/src/uproot_browser/tui/right_panel.py`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.3/tests/test_printouts.py` & `uproot_browser-0.6.4/tests/test_printouts.py`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.3/tests/test_tui.py` & `uproot_browser-0.6.4/tests/test_tui.py`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.3/.gitignore` & `uproot_browser-0.6.4/.gitignore`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.3/LICENSE` & `uproot_browser-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.3/README.md` & `uproot_browser-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.3/pyproject.toml` & `uproot_browser-0.6.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -60,14 +60,15 @@
   "matplotlib",
   "itermplot==0.5",
   "mplhep",
 ]
 dev = [
   "ipython >=6",
   "pytest >=6",
+  "pytest-asyncio",
   "scikit-hep-testdata",
 ]
 
 [project.urls]
 homepage = "https://github.com/scikit-hep/uproot-browser"
 repository = "https://github.com/scikit-hep/uproot-browser"
 
@@ -125,15 +126,15 @@
   "unused-argument",  # Handled by Ruff
   "wrong-import-position",  # Handled by Ruff
 ]
 
 [tool.ruff]
 select = [
   "E", "F", "W", # flake8
-  "B", "B904",   # flake8-bugbear
+  "B",           # flake8-bugbear
   "I",           # isort
   "ARG",         # flake8-unused-arguments
   "C4",          # flake8-comprehensions
   "EM",          # flake8-errmsg
   "ICN",         # flake8-import-conventions
   "ISC",         # flake8-implicit-str-concat
   "PGH",         # pygrep-hooks
```

### Comparing `uproot_browser-0.6.3/PKG-INFO` & `uproot_browser-0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uproot_browser
-Version: 0.6.3
+Version: 0.6.4
 Summary: Tools to inspect ROOT files with uproot
 Project-URL: homepage, https://github.com/scikit-hep/uproot-browser
 Project-URL: repository, https://github.com/scikit-hep/uproot-browser
 Author-email: Henry Schreiner <henryfs@princeton.edu>
 Maintainer-email: The Scikit-HEP admins <scikit-hep-admins@googlegroups.com>
 License: BSD 3-Clause License
         
@@ -60,14 +60,15 @@
 Requires-Dist: plotext>=5.2.7
 Requires-Dist: rich>=13.3.3
 Requires-Dist: textual>=0.18.0
 Requires-Dist: typing-extensions; python_version < '3.8'
 Requires-Dist: uproot>=4.2.1
 Provides-Extra: dev
 Requires-Dist: ipython>=6; extra == 'dev'
+Requires-Dist: pytest-asyncio; extra == 'dev'
 Requires-Dist: pytest>=6; extra == 'dev'
 Requires-Dist: scikit-hep-testdata; extra == 'dev'
 Provides-Extra: iterm
 Requires-Dist: itermplot==0.5; extra == 'iterm'
 Requires-Dist: matplotlib; extra == 'iterm'
 Requires-Dist: mplhep; extra == 'iterm'
 Provides-Extra: test
```

