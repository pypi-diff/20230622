# Comparing `tmp/fh_fablib-1.0.20230531.tar.gz` & `tmp/fh_fablib-1.0.20230622.tar.gz`

## Comparing `fh_fablib-1.0.20230531.tar` & `fh_fablib-1.0.20230622.tar`

### file list

```diff
@@ -1,18 +1,16 @@
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230531/.editorconfig
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230531/.pre-commit-config.yaml
--rw-r--r--   0        0        0    19496 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230531/CHANGELOG.rst
--rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230531/bumpversion.sh
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230531/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230531/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0    26558 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230531/fh_fablib/__init__.py
--rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230531/fh_fablib/extract_js_gettext_strings.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230531/fh_fablib/dotfiles/.editorconfig
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230531/fh_fablib/dotfiles/.eslintrc.js
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230531/fh_fablib/dotfiles/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230531/fh_fablib/dotfiles/pyproject.toml
--rw-r--r--   0        0        0     5820 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230531/fh_fablib/dotfiles/webpack.library.js
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230531/.gitignore
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230531/LICENSE
--rw-r--r--   0        0        0     7322 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230531/README.rst
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230531/pyproject.toml
--rw-r--r--   0        0        0     7724 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230531/PKG-INFO
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230622/.editorconfig
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230622/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    19712 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230622/CHANGELOG.rst
+-rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230622/bumpversion.sh
+-rw-r--r--   0        0        0    26616 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230622/fh_fablib/__init__.py
+-rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230622/fh_fablib/extract_js_gettext_strings.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230622/fh_fablib/dotfiles/.editorconfig
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230622/fh_fablib/dotfiles/.eslintrc.js
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230622/fh_fablib/dotfiles/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230622/fh_fablib/dotfiles/pyproject.toml
+-rw-r--r--   0        0        0     5820 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230622/fh_fablib/dotfiles/webpack.library.js
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230622/.gitignore
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230622/LICENSE
+-rw-r--r--   0        0        0     7322 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230622/README.rst
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230622/pyproject.toml
+-rw-r--r--   0        0        0     7724 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230622/PKG-INFO
```

### Comparing `fh_fablib-1.0.20230531/.pre-commit-config.yaml` & `fh_fablib-1.0.20230622/.pre-commit-config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -14,15 +14,15 @@
       - id: mixed-line-ending
       - id: trailing-whitespace
   - repo: https://github.com/MarcoGorelli/absolufy-imports
     rev: v0.3.1
     hooks:
       - id: absolufy-imports
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: "v0.0.270"
+    rev: "v0.0.274"
     hooks:
       - id: ruff
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/pre-commit/mirrors-prettier
```

### Comparing `fh_fablib-1.0.20230531/CHANGELOG.rst` & `fh_fablib-1.0.20230622/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 ==========
 Change log
 ==========
 
 Next version
 ~~~~~~~~~~~~
 
+1.0.20230622
+~~~~~~~~~~~~
+
+- Changed the JavaScript string extractor to strip trailing commas from
+  argument lists.
+- Switched to not deleting everything under ``static/`` when deploying, only
+  delete old files.
+
+
 1.0.20230531
 ~~~~~~~~~~~~
 
 - Updated the pre-commit hooks. Started ignoring the invalid module names
   generated by Django's database migration framework.
 - Changed ``nine-reinit-from`` to create more hardlinks when syncing media files.
 - Switched to hatchling.
```

### Comparing `fh_fablib-1.0.20230531/fh_fablib/__init__.py` & `fh_fablib-1.0.20230622/fh_fablib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from fabric import Connection, task
 from invoke import Collection  # noqa, re-export
 from speckenv_django import django_database_url
 
 from fh_fablib.extract_js_gettext_strings import generate_strings
 
 
-__version__ = "1.0.20230531"
+__version__ = "1.0.20230622"
 
 
 # I don't care, in this context.
 warnings.simplefilter("ignore", category=ResourceWarning)
 
 
 def ansi(code):
@@ -882,15 +882,16 @@
     if not fast:
         run_local(ctx, "NODE_ENV=production yarn run webpack --mode production --bail")
 
     with Connection(config.host) as conn, conn.cd(config.domain):
         _deploy_sync_origin_url(ctx, conn)
         _deploy_django(conn)
         if not fast:
-            _rsync_static(ctx, delete=True)
+            run(conn, "find static/ -mtime +60 -delete")
+            _rsync_static(ctx, delete=False)
         _deploy_staticfiles(conn)
         _nine_restart(conn)
 
     fetch(ctx)
     progress(f"Successfully deployed the {config.environment} environment.")
```

### Comparing `fh_fablib-1.0.20230531/fh_fablib/extract_js_gettext_strings.py` & `fh_fablib-1.0.20230622/fh_fablib/extract_js_gettext_strings.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     parens = 0
     quote = ""
     for idx, c in enumerate(part):
         if c == quote:
             quote = ""
         elif quote:
             pass
-        elif c in {"'", '"'}:
+        elif c in {"'", '"', "`"}:
             quote = c
         elif c == "(":
             parens += 1
         elif c == ")":
             parens -= 1
 
         if parens == 0:
@@ -57,32 +57,36 @@
     ["ngettext('singular', 'plural', someVar)"]
     >>> list(gettext_calls("abc def gettext ( ' abc ' ) xyz"))
     ["gettext(' abc ')"]
     >>> list(gettext_calls("gettext(':-/')"))
     ["gettext(':-/')"]
     >>> list(gettext_calls("gettext(':-)')"))
     ["gettext(':-)')"]
-    >>> list(gettext_calls("abc gettext('xyz' def pgettext('ctx', 'str') xzz"))
+    >>> list(gettext_calls("abc gettext('xyz' def pgettext('ctx', 'str', ) xzz"))
     ["pgettext('ctx', 'str')"]
+    >>> list(gettext_calls("gettext( 'Blub', )"))
+    ["gettext('Blub')"]
+    >>> list(gettext_calls("gettext(`Blub'`)"))
+    ["gettext(`Blub'`)"]
     """
 
     parts = deque(part.strip() for part in re.split(r"\b(\w*gettext)\b", source))
 
     while parts:
         top = parts.popleft()
         if not top.endswith("gettext"):
             continue
 
         if parts and (args := extract_args(parts.popleft())):
-            yield f"{top}({args.strip()})"
+            yield f"{top}({args.strip().rstrip(',')})"
 
 
 def generate_strings():
     calls = set()
     for file in js_files():
         with open(file, encoding="utf-8") as f:
             calls |= set(gettext_calls(f.read()))
-    return sorted(calls, key=lambda c: c.lower())
+    return sorted(calls, key=lambda c: (c.lower(), c))
 
 
 if __name__ == "__main__":
     print(generate_strings())
```

### Comparing `fh_fablib-1.0.20230531/fh_fablib/dotfiles/.pre-commit-config.yaml` & `fh_fablib-1.0.20230622/fh_fablib/dotfiles/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -20,32 +20,32 @@
       - id: django-check
         name: django check
         entry: venv/bin/python manage.py check
         pass_filenames: false
         language: system
         always_run: true
   - repo: https://github.com/adamchainz/django-upgrade
-    rev: 1.13.0
+    rev: 1.14.0
     hooks:
       - id: django-upgrade
         args: [--target-version, "4.0"]
   - repo: https://github.com/MarcoGorelli/absolufy-imports
     rev: v0.3.1
     hooks:
       - id: absolufy-imports
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: "v0.0.270"
+    rev: "v0.0.274"
     hooks:
       - id: ruff
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/pre-commit/mirrors-eslint
-    rev: v8.41.0
+    rev: v8.43.0
     hooks:
       - id: eslint
         args: [--fix]
         types_or: [css, scss, javascript]
         verbose: true
         additional_dependencies:
           - eslint
@@ -66,14 +66,14 @@
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: v3.0.0-alpha.9-for-vscode
     hooks:
       - id: prettier
         args: [--list-different, --no-semi]
         exclude: "^conf/|.*\\.html$|.*\\.json$"
   - repo: https://github.com/tox-dev/pyproject-fmt
-    rev: 0.11.2
+    rev: 0.12.1
     hooks:
       - id: pyproject-fmt
   - repo: https://github.com/abravalheri/validate-pyproject
     rev: v0.13
     hooks:
       - id: validate-pyproject
```

### Comparing `fh_fablib-1.0.20230531/fh_fablib/dotfiles/webpack.library.js` & `fh_fablib-1.0.20230622/fh_fablib/dotfiles/webpack.library.js`

 * *Files identical despite different names*

### Comparing `fh_fablib-1.0.20230531/LICENSE` & `fh_fablib-1.0.20230622/LICENSE`

 * *Files identical despite different names*

### Comparing `fh_fablib-1.0.20230531/README.rst` & `fh_fablib-1.0.20230622/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 3. Add a ``fabfile.py`` to your project. A minimal example follows:
 
    .. code-block:: python
 
        import fh_fablib as fl
 
-       fl.require("1.0.20230531")
+       fl.require("1.0.20230622")
        fl.config.update(host="www-data@feinheit06.nine.ch")
 
        environments = [
            fl.environment(
                "production",
                {
                    "domain": "example.com",
@@ -90,15 +90,15 @@
 
 If you need multiple environments, add environment tasks as follows:
 
 .. code-block:: python
 
     import fh_fablib as fl
 
-    fl.require("1.0.20230531")
+    fl.require("1.0.20230622")
     fl.config.update(host="www-data@feinheit06.nine.ch")
 
     environments = [
         fl.environment(
             "production",
             {
                 "domain": "example.com",
```

### Comparing `fh_fablib-1.0.20230531/pyproject.toml` & `fh_fablib-1.0.20230622/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -43,16 +43,14 @@
   "UP",
   # flake8-2020
   "YTT",
   # flake8-boolean-trap
   "FBT",
   # flake8-bugbear
   "B",
-  # flake8-builtins
-  "A",
   # flake8-comprehensions
   "C4",
   # flake8-django
   "DJ",
   # flake8-logging-format
   "G",
   # flake8-pie
```

### Comparing `fh_fablib-1.0.20230531/PKG-INFO` & `fh_fablib-1.0.20230622/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fh-fablib
-Version: 1.0.20230531
+Version: 1.0.20230622
 Summary: fh-fablib
 Project-URL: Homepage, https://github.com/feinheit/fh-fablib/
 Author-email: Matthias Kestenholz <mk@feinheit.ch>
 License: BSD-3-Clause
 License-File: LICENSE
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.9
@@ -28,15 +28,15 @@
 
 3. Add a ``fabfile.py`` to your project. A minimal example follows:
 
    .. code-block:: python
 
        import fh_fablib as fl
 
-       fl.require("1.0.20230531")
+       fl.require("1.0.20230622")
        fl.config.update(host="www-data@feinheit06.nine.ch")
 
        environments = [
            fl.environment(
                "production",
                {
                    "domain": "example.com",
@@ -104,15 +104,15 @@
 
 If you need multiple environments, add environment tasks as follows:
 
 .. code-block:: python
 
     import fh_fablib as fl
 
-    fl.require("1.0.20230531")
+    fl.require("1.0.20230622")
     fl.config.update(host="www-data@feinheit06.nine.ch")
 
     environments = [
         fl.environment(
             "production",
             {
                 "domain": "example.com",
```

