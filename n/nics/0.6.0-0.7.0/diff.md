# Comparing `tmp/nics-0.6.0.tar.gz` & `tmp/nics-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nics-0.6.0.tar", last modified: Thu Jun 22 05:58:44 2023, max compression
+gzip compressed data, was "/home/runner/work/now-i-can-sleep/now-i-can-sleep/dist/.tmp-u1tj0hje/nics-0.7.0.tar", last modified: Thu Jun 22 06:22:35 2023, max compression
```

## Comparing `nics-0.6.0.tar` & `nics-0.7.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 05:58:44.710003 nics-0.6.0/
--rw-rw-rw-   0        0        0     1097 2023-06-21 04:57:10.000000 nics-0.6.0/LICENSE
--rw-rw-rw-   0        0        0     1351 2023-06-22 05:58:44.712004 nics-0.6.0/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-06-21 08:49:46.000000 nics-0.6.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 05:58:44.552965 nics-0.6.0/nics/
--rw-rw-rw-   0        0        0     2290 2023-06-21 15:56:17.000000 nics-0.6.0/nics/__init__.py
--rw-rw-rw-   0        0        0       65 2023-06-21 12:48:52.000000 nics-0.6.0/nics/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-22 05:58:44.647989 nics-0.6.0/nics/compile/
--rw-rw-rw-   0        0        0     1499 2023-06-22 05:06:14.000000 nics-0.6.0/nics/compile/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-22 05:58:44.706002 nics-0.6.0/nics/wizard/
--rw-rw-rw-   0        0        0      137 2023-06-21 05:37:43.000000 nics-0.6.0/nics/wizard/step1.py
--rw-rw-rw-   0        0        0      137 2023-06-21 05:37:43.000000 nics-0.6.0/nics/wizard/step2.py
--rw-rw-rw-   0        0        0      137 2023-06-21 05:37:43.000000 nics-0.6.0/nics/wizard/step3.py
-drwxrwxrwx   0        0        0        0 2023-06-22 05:58:44.642987 nics-0.6.0/nics.egg-info/
--rw-rw-rw-   0        0        0     1351 2023-06-22 05:58:44.000000 nics-0.6.0/nics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      343 2023-06-22 05:58:44.000000 nics-0.6.0/nics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 05:58:44.000000 nics-0.6.0/nics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-06-22 05:58:44.000000 nics-0.6.0/nics.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       13 2023-06-22 05:58:44.000000 nics-0.6.0/nics.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-22 05:58:44.000000 nics-0.6.0/nics.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1257 2023-06-22 05:06:52.000000 nics-0.6.0/pyproject.toml
--rw-rw-rw-   0        0        0      171 2023-06-22 05:58:44.718007 nics-0.6.0/setup.cfg
--rw-rw-rw-   0        0        0       37 2023-06-21 04:57:10.000000 nics-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:22:35.000000 nics-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-22 06:22:18.000000 nics-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-22 06:22:35.000000 nics-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-22 06:22:18.000000 nics-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:22:35.000000 nics-0.7.0/nics/
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-06-22 06:22:18.000000 nics-0.7.0/nics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-22 06:22:18.000000 nics-0.7.0/nics/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:22:35.000000 nics-0.7.0/nics/compile/
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-22 06:22:18.000000 nics-0.7.0/nics/compile/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:22:35.000000 nics-0.7.0/nics/wizard/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-22 06:22:18.000000 nics-0.7.0/nics/wizard/step1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-22 06:22:18.000000 nics-0.7.0/nics/wizard/step2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-22 06:22:18.000000 nics-0.7.0/nics/wizard/step3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:22:35.000000 nics-0.7.0/nics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-22 06:22:35.000000 nics-0.7.0/nics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-22 06:22:35.000000 nics-0.7.0/nics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 06:22:35.000000 nics-0.7.0/nics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-22 06:22:35.000000 nics-0.7.0/nics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-22 06:22:35.000000 nics-0.7.0/nics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-22 06:22:35.000000 nics-0.7.0/nics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-22 06:22:18.000000 nics-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-22 06:22:35.000000 nics-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-22 06:22:18.000000 nics-0.7.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `nics-0.6.0/LICENSE` & `nics-0.7.0/LICENSE`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Nicholas Valentinus
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Nicholas Valentinus
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `nics-0.6.0/PKG-INFO` & `nics-0.7.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-Metadata-Version: 2.1
-Name: nics
-Version: 0.6.0
-Summary: Automated docs repo generator
-Home-page: https://nvfp.github.io/now-i-can-sleep
-Author: Nicholas Valentinus
-Author-email: nvfastplease@gmail.com
-License: MIT
-Project-URL: documentation, https://nvfp.github.io/now-i-can-sleep/docs
-Project-URL: report bugs, https://github.com/nvfp/now-i-can-sleep/issues
-Project-URL: repo, https://github.com/nvfp/now-i-can-sleep
-Project-URL: changelog, https://nvfp.github.io/now-i-can-sleep/changelog
-Keywords: python,toolkit,mykit
-Classifier: Topic :: Scientific/Engineering
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Natural Language :: English
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
-
-# Now-I-Can-Sleep
-
-## Usage
-
-1. Install via pip:
-
-    ```sh
-    pip install nics
-    ```
-
-2. Navigate to your project root directory
-3. Run:
-
-    ```sh
-    nics start
-    ```
-4. Follow the wizard, and you all set!
+Metadata-Version: 2.1
+Name: nics
+Version: 0.7.0
+Summary: Automated docs repo generator
+Home-page: https://nvfp.github.io/now-i-can-sleep
+Author: Nicholas Valentinus
+Author-email: nvfastplease@gmail.com
+License: MIT
+Project-URL: documentation, https://nvfp.github.io/now-i-can-sleep/docs
+Project-URL: report bugs, https://github.com/nvfp/now-i-can-sleep/issues
+Project-URL: repo, https://github.com/nvfp/now-i-can-sleep
+Project-URL: changelog, https://nvfp.github.io/now-i-can-sleep/changelog
+Keywords: python,toolkit,mykit
+Classifier: Topic :: Scientific/Engineering
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Natural Language :: English
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+
+# Now-I-Can-Sleep
+
+## Usage
+
+1. Install via pip:
+
+    ```sh
+    pip install nics
+    ```
+
+2. Navigate to your project root directory
+3. Run:
+
+    ```sh
+    nics start
+    ```
+4. Follow the wizard, and you all set!
```

### Comparing `nics-0.6.0/nics/__init__.py` & `nics-0.7.0/nics/__init__.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,80 +1,80 @@
-import argparse
-import os
-import pkg_resources
-
-from mykit.kit.utils import printer
-
-from nics.compile import run as run_compile
-
-
-try:
-    __version__ = pkg_resources.get_distribution('nics').version
-except pkg_resources.DistributionNotFound:
-    ## this exception occurred during development (before the software installed via pip)
-    __version__ = 'dev'
-
-
-SOFTWARE_REPO = 'https://github.com/nvfp/now-i-can-sleep'
-SOFTWARE_NAME = 'Now I Can Sleep'
-SOFTWARE_DIST_NAME = 'nics'  # distribution name
-
-ROOT_DIR_PTH = os.path.dirname(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
-DIST_DIR_PTH = os.path.join(ROOT_DIR_PTH, SOFTWARE_DIST_NAME)
-
-
-def main():
-
-    parser = argparse.ArgumentParser(
-        prog=SOFTWARE_DIST_NAME,
-        usage=(
-            '\n'
-            '├─ %(prog)s start\n'
-            '├─ %(prog)s start step2\n'
-            '├─ %(prog)s start step3\n'
-            '└─ %(prog)s downl\n'
-        ),
-        formatter_class=argparse.RawTextHelpFormatter  # to use line breaks (\n) in the help message
-    )
-
-    ## version
-    parser.add_argument(
-        '-v', '--version', action='version', version=f'%(prog)s-{__version__}',
-        help='show app\'s version then exit'
-    )
-
-    ## command parser
-    subparsers = parser.add_subparsers(dest='cmd')
-
-    ## start command
-    start_parser = subparsers.add_parser('start', help='')
-    start_parser.add_argument('arg1', type=int, help='')
-
-    ## compile command (that users shouldn't run)
-    compile_parser = subparsers.add_parser('_compile', help='')
-    compile_parser.add_argument('input')
-    compile_parser.add_argument('output')
-
-
-    ## positional args
-    # parser.add_argument(
-    #     'cmd',
-    #     choices=['start', 'update', '_compile'],
-    #     help=argparse.SUPPRESS  # to hide the help message
-    # )
-    # parser.add_argument(
-    #     'arg2',
-    #     choices=[
-    #         'step2', 'step3',
-    #         ''
-    #     ],
-    #     nargs='?',
-    #     help=argparse.SUPPRESS  # to hide the help message
-    # )
-
-
-    args = parser.parse_args()
-
-    printer(f'INFO: running command {repr(args.cmd)}.')
-
-    if args.cmd == '_compile':
+import argparse
+import os
+import pkg_resources
+
+from mykit.kit.utils import printer
+
+from nics.compile import run as run_compile
+
+
+try:
+    __version__ = pkg_resources.get_distribution('nics').version
+except pkg_resources.DistributionNotFound:
+    ## this exception occurred during development (before the software installed via pip)
+    __version__ = 'dev'
+
+
+SOFTWARE_REPO = 'https://github.com/nvfp/now-i-can-sleep'
+SOFTWARE_NAME = 'Now I Can Sleep'
+SOFTWARE_DIST_NAME = 'nics'  # distribution name
+
+ROOT_DIR_PTH = os.path.dirname(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
+DIST_DIR_PTH = os.path.join(ROOT_DIR_PTH, SOFTWARE_DIST_NAME)
+
+
+def main():
+
+    parser = argparse.ArgumentParser(
+        prog=SOFTWARE_DIST_NAME,
+        usage=(
+            '\n'
+            '├─ %(prog)s start\n'
+            '├─ %(prog)s start step2\n'
+            '├─ %(prog)s start step3\n'
+            '└─ %(prog)s downl\n'
+        ),
+        formatter_class=argparse.RawTextHelpFormatter  # to use line breaks (\n) in the help message
+    )
+
+    ## version
+    parser.add_argument(
+        '-v', '--version', action='version', version=f'%(prog)s-{__version__}',
+        help='show app\'s version then exit'
+    )
+
+    ## command parser
+    subparsers = parser.add_subparsers(dest='cmd')
+
+    ## start command
+    start_parser = subparsers.add_parser('start', help='')
+    start_parser.add_argument('arg1', type=int, help='')
+
+    ## compile command (that users shouldn't run)
+    compile_parser = subparsers.add_parser('_compile', help='')
+    compile_parser.add_argument('input')
+    compile_parser.add_argument('output')
+
+
+    ## positional args
+    # parser.add_argument(
+    #     'cmd',
+    #     choices=['start', 'update', '_compile'],
+    #     help=argparse.SUPPRESS  # to hide the help message
+    # )
+    # parser.add_argument(
+    #     'arg2',
+    #     choices=[
+    #         'step2', 'step3',
+    #         ''
+    #     ],
+    #     nargs='?',
+    #     help=argparse.SUPPRESS  # to hide the help message
+    # )
+
+
+    args = parser.parse_args()
+
+    printer(f'INFO: running command {repr(args.cmd)}.')
+
+    if args.cmd == '_compile':
         run_compile(args.input, args.output)
```

### Comparing `nics-0.6.0/nics/compile/__init__.py` & `nics-0.7.0/nics/compile/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-import os
-
-from mykit.kit.keycrate import KeyCrate
-from mykit.kit.utils import printer
-
-
-def header_writer(docs) -> str:
-    
-    header = (
-        '<header>'
-
-            '<h1>{{ page.title }}</h1>'
-
-            '<div class="wrap">'
-
-                '<button id="_root__nav">v Navigation</button>'
-                '<div class="main" id="_root__nav-div">'
-    )
-
-    for pth, dirs, files in os.walk(docs):
-
-        printer(f'DEBUG: pth: {pth}')
-        printer(f'DEBUG: dirs: {dirs}')
-        printer(f'DEBUG: files: {files}')
-        printer(f'DEBUG: ---------')
-
-    header += (
-                '</div>'
-            
-            '</div>'
-
-        '</header>'
-    )
-    
-    return header
-
-
-def run(docs, target):
-    """
-    ## Params
-    - `docs`: the docs/ bundle
-    - `target`: the branch
-    """
-
-    printer(f'DEBUG: docs: {repr(docs)}.')
-    printer(f'DEBUG: target: {repr(target)}.')
-
-    printer(f'DEBUG: os.path.isdir(docs): {os.path.isdir(docs)}.')
-    printer(f'DEBUG: os.path.isdir(target): {os.path.isdir(target)}.')
-
-    printer(f'DEBUG: os.listdir(docs): {os.listdir(docs)}.')
-    printer(f'DEBUG: os.listdir(target): {os.listdir(target)}.')
-
-    settings = KeyCrate(
-        file_pth=os.path.join(docs, '_nics', 'settings.txt'),
-        key_is_var=True, eval_value=True
-    )
-    
-    printer(f'DEBUG: settings.export(): {settings.export()}')
-
-    header = header_writer(docs)
-
+import os
+
+from mykit.kit.keycrate import KeyCrate
+from mykit.kit.utils import printer
+
+
+def header_writer(docs) -> str:
+    
+    header = (
+        '<header>'
+
+            '<h1>{{ page.title }}</h1>'
+
+            '<div class="wrap">'
+
+                '<button id="_root__nav">v Navigation</button>'
+                '<div class="main" id="_root__nav-div">'
+    )
+
+    for pth, dirs, files in os.walk(docs):
+
+        printer(f'DEBUG: pth: {pth}')
+        printer(f'DEBUG: dirs: {dirs}')
+        printer(f'DEBUG: files: {files}')
+        printer(f'DEBUG: ---------')
+
+    header += (
+                '</div>'
+            
+            '</div>'
+
+        '</header>'
+    )
+    
+    return header
+
+
+def run(docs, target):
+    """
+    ## Params
+    - `docs`: the docs/ bundle
+    - `target`: the branch
+    """
+
+    printer(f'DEBUG: docs: {repr(docs)}.')
+    printer(f'DEBUG: target: {repr(target)}.')
+
+    printer(f'DEBUG: os.path.isdir(docs): {os.path.isdir(docs)}.')
+    printer(f'DEBUG: os.path.isdir(target): {os.path.isdir(target)}.')
+
+    printer(f'DEBUG: os.listdir(docs): {os.listdir(docs)}.')
+    printer(f'DEBUG: os.listdir(target): {os.listdir(target)}.')
+
+    settings = KeyCrate(
+        os.path.join(docs, '_nics', 'settings.txt'),
+        key_is_var=True, eval_value=True
+    )
+    
+    printer(f'DEBUG: settings.export(): {settings.export()}')
+
+    header = header_writer(docs)
+
     printer(f'DEBUG: header: {header}')
```

### Comparing `nics-0.6.0/nics.egg-info/PKG-INFO` & `nics-0.7.0/nics.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-Metadata-Version: 2.1
-Name: nics
-Version: 0.6.0
-Summary: Automated docs repo generator
-Home-page: https://nvfp.github.io/now-i-can-sleep
-Author: Nicholas Valentinus
-Author-email: nvfastplease@gmail.com
-License: MIT
-Project-URL: documentation, https://nvfp.github.io/now-i-can-sleep/docs
-Project-URL: report bugs, https://github.com/nvfp/now-i-can-sleep/issues
-Project-URL: repo, https://github.com/nvfp/now-i-can-sleep
-Project-URL: changelog, https://nvfp.github.io/now-i-can-sleep/changelog
-Keywords: python,toolkit,mykit
-Classifier: Topic :: Scientific/Engineering
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Natural Language :: English
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
-
-# Now-I-Can-Sleep
-
-## Usage
-
-1. Install via pip:
-
-    ```sh
-    pip install nics
-    ```
-
-2. Navigate to your project root directory
-3. Run:
-
-    ```sh
-    nics start
-    ```
-4. Follow the wizard, and you all set!
+Metadata-Version: 2.1
+Name: nics
+Version: 0.7.0
+Summary: Automated docs repo generator
+Home-page: https://nvfp.github.io/now-i-can-sleep
+Author: Nicholas Valentinus
+Author-email: nvfastplease@gmail.com
+License: MIT
+Project-URL: documentation, https://nvfp.github.io/now-i-can-sleep/docs
+Project-URL: report bugs, https://github.com/nvfp/now-i-can-sleep/issues
+Project-URL: repo, https://github.com/nvfp/now-i-can-sleep
+Project-URL: changelog, https://nvfp.github.io/now-i-can-sleep/changelog
+Keywords: python,toolkit,mykit
+Classifier: Topic :: Scientific/Engineering
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Natural Language :: English
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+
+# Now-I-Can-Sleep
+
+## Usage
+
+1. Install via pip:
+
+    ```sh
+    pip install nics
+    ```
+
+2. Navigate to your project root directory
+3. Run:
+
+    ```sh
+    nics start
+    ```
+4. Follow the wizard, and you all set!
```

### Comparing `nics-0.6.0/pyproject.toml` & `nics-0.7.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-[build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
-
-
-[project]
-name = "nics"
-version = "0.6.0"
-description = "Automated docs repo generator"
-readme = "README.md"
-requires-python = ">=3.8"
-license = {text = "MIT"}
-authors = [
-  	{email = "nvfastplease@gmail.com"},
-]
-keywords = ["python", "toolkit", "mykit"]
-classifiers = [
-	"Topic :: Scientific/Engineering",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3 :: Only",
-    "Natural Language :: English"
-]
-dependencies = [
-    "mykit==4.1.0",
-]
-
-
-[tool.setuptools.packages.find]
-exclude = [
-    "archive*",
-    "docs*",
-]
-
-
-[project.urls]
-documentation = "https://nvfp.github.io/now-i-can-sleep/docs"
-"report bugs" = "https://github.com/nvfp/now-i-can-sleep/issues"
-repo = "https://github.com/nvfp/now-i-can-sleep"
-changelog = "https://nvfp.github.io/now-i-can-sleep/changelog"
-
-
-[project.scripts]
-nics = "nics.__main__:main"
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
+
+
+[project]
+name = "nics"
+version = "0.7.0"
+description = "Automated docs repo generator"
+readme = "README.md"
+requires-python = ">=3.8"
+license = {text = "MIT"}
+authors = [
+  	{email = "nvfastplease@gmail.com"},
+]
+keywords = ["python", "toolkit", "mykit"]
+classifiers = [
+	"Topic :: Scientific/Engineering",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3 :: Only",
+    "Natural Language :: English"
+]
+dependencies = [
+    "mykit==4.1.0",
+]
+
+
+[tool.setuptools.packages.find]
+exclude = [
+    "archive*",
+    "docs*",
+]
+
+
+[project.urls]
+documentation = "https://nvfp.github.io/now-i-can-sleep/docs"
+"report bugs" = "https://github.com/nvfp/now-i-can-sleep/issues"
+repo = "https://github.com/nvfp/now-i-can-sleep"
+changelog = "https://nvfp.github.io/now-i-can-sleep/changelog"
+
+
+[project.scripts]
+nics = "nics.__main__:main"
```

