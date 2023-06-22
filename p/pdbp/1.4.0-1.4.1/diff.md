# Comparing `tmp/pdbp-1.4.0.tar.gz` & `tmp/pdbp-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdbp-1.4.0.tar", last modified: Wed Apr 26 19:53:08 2023, max compression
+gzip compressed data, was "pdbp-1.4.1.tar", last modified: Thu Jun 22 15:50:46 2023, max compression
```

## Comparing `pdbp-1.4.0.tar` & `pdbp-1.4.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-26 19:53:08.885245 pdbp-1.4.0/
--rw-r--r--   0 michael    (501) staff       (20)      774 2022-11-28 00:12:24.000000 pdbp-1.4.0/.gitignore
--rwxr-xr-x   0 michael    (501) staff       (20)     1536 2022-11-28 00:30:19.000000 pdbp-1.4.0/CODE_OF_CONDUCT.md
--rwxr-xr-x   0 michael    (501) staff       (20)     1664 2022-11-28 00:28:34.000000 pdbp-1.4.0/CONTRIBUTING.md
--rw-r--r--   0 michael    (501) staff       (20)     1066 2022-11-28 00:19:16.000000 pdbp-1.4.0/LICENSE
--rw-rw-r--   0 michael    (501) staff       (20)       34 2022-11-28 00:19:28.000000 pdbp-1.4.0/MANIFEST.in
--rw-r--r--   0 michael    (501) staff       (20)     6298 2023-04-26 19:53:08.885299 pdbp-1.4.0/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)     4282 2023-04-26 19:51:46.000000 pdbp-1.4.0/README.md
--rwxr-xr-x   0 michael    (501) staff       (20)      303 2022-11-28 07:12:13.000000 pdbp-1.4.0/SECURITY.md
--rwxr-xr-x   0 michael    (501) staff       (20)       88 2023-04-26 19:53:08.885477 pdbp-1.4.0/setup.cfg
--rwxr-xr-x   0 michael    (501) staff       (20)     5324 2023-04-26 19:51:46.000000 pdbp-1.4.0/setup.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-26 19:53:08.884357 pdbp-1.4.0/src/
--rwxr-xr-x   0 michael    (501) staff       (20)       39 2022-11-28 05:30:45.000000 pdbp-1.4.0/src/__init__.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-26 19:53:08.885122 pdbp-1.4.0/src/pdbp.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)     6298 2023-04-26 19:53:08.000000 pdbp-1.4.0/src/pdbp.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      293 2023-04-26 19:53:08.000000 pdbp-1.4.0/src/pdbp.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-04-26 19:53:08.000000 pdbp-1.4.0/src/pdbp.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)      121 2023-04-26 19:53:08.000000 pdbp-1.4.0/src/pdbp.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)        5 2023-04-26 19:53:08.000000 pdbp-1.4.0/src/pdbp.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) staff       (20)    54036 2023-04-26 19:51:46.000000 pdbp-1.4.0/src/pdbp.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-22 15:50:46.460670 pdbp-1.4.1/
+-rw-r--r--   0 michael    (501) staff       (20)      774 2022-11-28 00:12:24.000000 pdbp-1.4.1/.gitignore
+-rwxr-xr-x   0 michael    (501) staff       (20)     1536 2022-11-28 00:30:19.000000 pdbp-1.4.1/CODE_OF_CONDUCT.md
+-rwxr-xr-x   0 michael    (501) staff       (20)     1664 2022-11-28 00:28:34.000000 pdbp-1.4.1/CONTRIBUTING.md
+-rw-r--r--   0 michael    (501) staff       (20)     1066 2022-11-28 00:19:16.000000 pdbp-1.4.1/LICENSE
+-rw-rw-r--   0 michael    (501) staff       (20)       34 2022-11-28 00:19:28.000000 pdbp-1.4.1/MANIFEST.in
+-rw-r--r--   0 michael    (501) staff       (20)     6821 2023-06-22 15:50:46.460728 pdbp-1.4.1/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)     4805 2023-06-22 15:48:47.000000 pdbp-1.4.1/README.md
+-rwxr-xr-x   0 michael    (501) staff       (20)      303 2022-11-28 07:12:13.000000 pdbp-1.4.1/SECURITY.md
+-rwxr-xr-x   0 michael    (501) staff       (20)       88 2023-06-22 15:50:46.460919 pdbp-1.4.1/setup.cfg
+-rwxr-xr-x   0 michael    (501) staff       (20)     5379 2023-06-22 15:48:47.000000 pdbp-1.4.1/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-22 15:50:46.460029 pdbp-1.4.1/src/
+-rwxr-xr-x   0 michael    (501) staff       (20)       39 2022-11-28 05:30:45.000000 pdbp-1.4.1/src/__init__.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-22 15:50:46.460562 pdbp-1.4.1/src/pdbp.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)     6821 2023-06-22 15:50:46.000000 pdbp-1.4.1/src/pdbp.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      293 2023-06-22 15:50:46.000000 pdbp-1.4.1/src/pdbp.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-06-22 15:50:46.000000 pdbp-1.4.1/src/pdbp.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)      109 2023-06-22 15:50:46.000000 pdbp-1.4.1/src/pdbp.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)        5 2023-06-22 15:50:46.000000 pdbp-1.4.1/src/pdbp.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) staff       (20)    53998 2023-06-22 15:48:47.000000 pdbp-1.4.1/src/pdbp.py
```

### Comparing `pdbp-1.4.0/.gitignore` & `pdbp-1.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pdbp-1.4.0/CODE_OF_CONDUCT.md` & `pdbp-1.4.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pdbp-1.4.0/CONTRIBUTING.md` & `pdbp-1.4.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pdbp-1.4.0/LICENSE` & `pdbp-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pdbp-1.4.0/PKG-INFO` & `pdbp-1.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdbp
-Version: 1.4.0
+Version: 1.4.1
 Summary: pdbp (Pdb+): A drop-in replacement for pdb and pdbpp.
 Home-page: https://github.com/mdmintz/pdbp
 Author: Michael Mintz
 Author-email: mdmintz@gmail.com
 Maintainer: Michael Mintz
 License: MIT
 Project-URL: Changelog, https://github.com/mdmintz/pdbp/releases
@@ -44,28 +44,28 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pdbp (Pdb+) [![](https://img.shields.io/pypi/v/pdbp.svg)](https://pypi.python.org/pypi/pdbp)
 
-<img width="650" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/234679015-b1daa50f-94a8-4ef2-b3f5-3157b7a3733b.png">
+<img width="660" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/247826485-d782911e-d817-4ea6-86dd-215991d7b8ea.png">
 
 --------
 
-**[pdbp (Pdb+)](https://github.com/mdmintz/pdbp)** is an advanced console debugger for Python. It can be used as a drop-in replacement for ``pdb`` and [pdbpp](https://github.com/pdbpp/pdbpp).
+**[pdbp (Pdb+)](https://github.com/mdmintz/pdbp)** is an advanced console debugger for Python. It can be used as a drop-in replacement for [pdb](https://docs.python.org/3/library/pdb.html) and [pdbpp](https://github.com/pdbpp/pdbpp).
 
 <p><b>pdbp (Pdb+)</b> makes Python debugging a lot easier (and more fun!)</p>
 
 --------
 
-<img width="650" alt="Pdb+" src="https://user-images.githubusercontent.com/6788579/234669562-30dae4ad-1207-47e4-8327-fbd5662c8b9c.png">
+<img width="650" alt="Pdb+" src="https://user-images.githubusercontent.com/6788579/234679015-b1daa50f-94a8-4ef2-b3f5-3157b7a3733b.png">
 
 
-## Installation & Usage:
+## Installation:
 
 ```bash
 pip install pdbp
 ```
 
 Then add ``import pdbp`` to an ``__init__.py`` of your project, which will automatically make **``Pdb+``** the default debugger at breakpoints:
 
@@ -75,16 +75,32 @@
 
 (If using ``flake8`` for code-linting, you may want to add ``# noqa`` to that line):
 
 ```python
 import pdbp  # noqa
 ```
 
+You can also make ``pdbp`` the default debugger by setting an environmental variable:
+
+```bash
+PYTHONBREAKPOINT=pdbp.set_trace
+```
+
+## Usage:
+
 To trigger a breakpoint in your code with ``pytest``, add ``--trace`` (to start tests with a breakpoint) or ``--pdb`` (to trigger a breakpoint if a test fails).
 
+To trigger a breakpoint from a pure ``python`` run, use:
+
+```bash
+python -m pdbp <script.py>
+```
+
+--------
+
 Basic **``Pdb+``** console commands: ``n``, ``c``, ``s`` => ``next``, ``continue``, ``step``.
 
 Use the ``u`` and ``d`` keys to travel ``up`` and ``down`` the stack!
 
 (To learn more **Pdb+** console commands, type ``help`` in the **Pdb+** console and press ``Enter/Return``.)
 
 --------
@@ -129,35 +145,42 @@
 <img width="640" alt="Pdb+ Post Mortem Debug Mode" src="https://user-images.githubusercontent.com/6788579/232537816-0b9e9048-724f-48cb-81e3-5cc403109de9.png">
 
 
 ### The ``where`` / ``w`` command, which displays the current stack:
 
 <img width="870" alt="Example of the 'where' command" src="https://user-images.githubusercontent.com/6788579/232962807-2d469603-a1d0-4891-8d0e-f03a4e1d0d00.png">
 
+--------
 
 ### Sticky Mode vs Non-Sticky Mode:
 
 The default mode (``sticky``) lets you see a lot more lines of code from the debugger when active. In Non-Sticky mode, only one line of code is shown at a time. You can switch between the two modes by typing ``sticky`` in the **Pdb+** console prompt and pressing ``Enter/Return``.
 
 > **Sticky Mode:**
 
 <img width="600" alt="Pdb+ Stick Mode" src="https://user-images.githubusercontent.com/6788579/204890148-53d2567b-9a56-4243-a7d7-66100a284312.png">
 
 > **Non-Sticky Mode:**
 
 <img width="600" alt="Pdb+ Non-Sticky Mode" src="https://user-images.githubusercontent.com/6788579/204890164-8465bc22-0f20-43f1-8ab7-b4316718a4c6.png">
 
+--------
+
+### Multi-layer highlighting in the same stack:
+
+<img width="536" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/207925754-4d4ffce5-be6c-44b6-b614-ae0e800a93d8.png">
+
 
 ### More examples:
 
 **``Pdb+``** is used by packages such as **``seleniumbase``**:
 
 * https://pypi.org/project/seleniumbase/
 * https://github.com/seleniumbase/SeleniumBase
 
 --------
 
-<img width="600" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/204896775-38d8551b-1d3c-4e95-9f5c-0e03c9de13da.png">
+<img width="650" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/234669562-30dae4ad-1207-47e4-8327-fbd5662c8b9c.png">
 
 --------
 
 (**Pdb+** is maintained by the [SeleniumBase Dev Team](https://github.com/seleniumbase/SeleniumBase))
```

### Comparing `pdbp-1.4.0/README.md` & `pdbp-1.4.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # pdbp (Pdb+) [![](https://img.shields.io/pypi/v/pdbp.svg)](https://pypi.python.org/pypi/pdbp)
 
-<img width="650" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/234679015-b1daa50f-94a8-4ef2-b3f5-3157b7a3733b.png">
+<img width="660" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/247826485-d782911e-d817-4ea6-86dd-215991d7b8ea.png">
 
 --------
 
-**[pdbp (Pdb+)](https://github.com/mdmintz/pdbp)** is an advanced console debugger for Python. It can be used as a drop-in replacement for ``pdb`` and [pdbpp](https://github.com/pdbpp/pdbpp).
+**[pdbp (Pdb+)](https://github.com/mdmintz/pdbp)** is an advanced console debugger for Python. It can be used as a drop-in replacement for [pdb](https://docs.python.org/3/library/pdb.html) and [pdbpp](https://github.com/pdbpp/pdbpp).
 
 <p><b>pdbp (Pdb+)</b> makes Python debugging a lot easier (and more fun!)</p>
 
 --------
 
-<img width="650" alt="Pdb+" src="https://user-images.githubusercontent.com/6788579/234669562-30dae4ad-1207-47e4-8327-fbd5662c8b9c.png">
+<img width="650" alt="Pdb+" src="https://user-images.githubusercontent.com/6788579/234679015-b1daa50f-94a8-4ef2-b3f5-3157b7a3733b.png">
 
 
-## Installation & Usage:
+## Installation:
 
 ```bash
 pip install pdbp
 ```
 
 Then add ``import pdbp`` to an ``__init__.py`` of your project, which will automatically make **``Pdb+``** the default debugger at breakpoints:
 
@@ -27,16 +27,32 @@
 
 (If using ``flake8`` for code-linting, you may want to add ``# noqa`` to that line):
 
 ```python
 import pdbp  # noqa
 ```
 
+You can also make ``pdbp`` the default debugger by setting an environmental variable:
+
+```bash
+PYTHONBREAKPOINT=pdbp.set_trace
+```
+
+## Usage:
+
 To trigger a breakpoint in your code with ``pytest``, add ``--trace`` (to start tests with a breakpoint) or ``--pdb`` (to trigger a breakpoint if a test fails).
 
+To trigger a breakpoint from a pure ``python`` run, use:
+
+```bash
+python -m pdbp <script.py>
+```
+
+--------
+
 Basic **``Pdb+``** console commands: ``n``, ``c``, ``s`` => ``next``, ``continue``, ``step``.
 
 Use the ``u`` and ``d`` keys to travel ``up`` and ``down`` the stack!
 
 (To learn more **Pdb+** console commands, type ``help`` in the **Pdb+** console and press ``Enter/Return``.)
 
 --------
@@ -81,35 +97,42 @@
 <img width="640" alt="Pdb+ Post Mortem Debug Mode" src="https://user-images.githubusercontent.com/6788579/232537816-0b9e9048-724f-48cb-81e3-5cc403109de9.png">
 
 
 ### The ``where`` / ``w`` command, which displays the current stack:
 
 <img width="870" alt="Example of the 'where' command" src="https://user-images.githubusercontent.com/6788579/232962807-2d469603-a1d0-4891-8d0e-f03a4e1d0d00.png">
 
+--------
 
 ### Sticky Mode vs Non-Sticky Mode:
 
 The default mode (``sticky``) lets you see a lot more lines of code from the debugger when active. In Non-Sticky mode, only one line of code is shown at a time. You can switch between the two modes by typing ``sticky`` in the **Pdb+** console prompt and pressing ``Enter/Return``.
 
 > **Sticky Mode:**
 
 <img width="600" alt="Pdb+ Stick Mode" src="https://user-images.githubusercontent.com/6788579/204890148-53d2567b-9a56-4243-a7d7-66100a284312.png">
 
 > **Non-Sticky Mode:**
 
 <img width="600" alt="Pdb+ Non-Sticky Mode" src="https://user-images.githubusercontent.com/6788579/204890164-8465bc22-0f20-43f1-8ab7-b4316718a4c6.png">
 
+--------
+
+### Multi-layer highlighting in the same stack:
+
+<img width="536" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/207925754-4d4ffce5-be6c-44b6-b614-ae0e800a93d8.png">
+
 
 ### More examples:
 
 **``Pdb+``** is used by packages such as **``seleniumbase``**:
 
 * https://pypi.org/project/seleniumbase/
 * https://github.com/seleniumbase/SeleniumBase
 
 --------
 
-<img width="600" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/204896775-38d8551b-1d3c-4e95-9f5c-0e03c9de13da.png">
+<img width="650" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/234669562-30dae4ad-1207-47e4-8327-fbd5662c8b9c.png">
 
 --------
 
 (**Pdb+** is maintained by the [SeleniumBase Dev Team](https://github.com/seleniumbase/SeleniumBase))
```

### Comparing `pdbp-1.4.0/setup.py` & `pdbp-1.4.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,37 +21,37 @@
     long_description = "\n".join(long_description_lines)
 except IOError:
     long_description = "pdbp (Pdb+): A drop-in replacement for pdb and pdbpp."
 
 if sys.argv[-1] == "publish":
     reply = None
     input_method = input
-    if not sys.version_info[0] >= 3:
-        input_method = raw_input  # noqa: F821
     confirm_text = ">>> Confirm release PUBLISH to PyPI? (yes/no): "
     reply = str(input_method(confirm_text)).lower().strip()
     if reply == "yes":
+        if sys.version_info < (3, 9):
+            print("\nERROR! Publishing to PyPI requires Python>=3.9")
+            sys.exit()
         print("\n*** Checking code health with flake8:\n")
-        if sys.version_info >= (3, 9):
-            os.system("python -m pip install 'flake8==6.0.0'")
-        else:
-            os.system("python -m pip install 'flake8==5.0.4'")
+        os.system("python -m pip install 'flake8==6.0.0'")
         flake8_status = os.system("flake8 --exclude=.eggs,temp")
         if flake8_status != 0:
-            print("\nWARNING! Fix flake8 issues before publishing to PyPI!\n")
+            print("\nERROR! Fix flake8 issues before publishing to PyPI!\n")
             sys.exit()
         else:
             print("*** No flake8 issues detected. Continuing...")
         print("\n*** Removing existing distribution packages: ***\n")
         os.system("rm -f dist/*.egg; rm -f dist/*.tar.gz; rm -f dist/*.whl")
         os.system("rm -rf build/bdist.*; rm -rf build/lib")
         print("\n*** Installing build: *** (Required for PyPI uploads)\n")
         os.system("python -m pip install --upgrade 'build>=0.10.0'")
         print("\n*** Installing pkginfo: *** (Required for PyPI uploads)\n")
         os.system("python -m pip install --upgrade 'pkginfo>=1.9.6'")
+        print("\n*** Installing readme-renderer: *** (For PyPI uploads)\n")
+        os.system("python -m pip install --upgrade 'readme-renderer>=40.0'")
         print("\n*** Installing twine: *** (Required for PyPI uploads)\n")
         os.system("python -m pip install --upgrade 'twine>=4.0.2'")
         print("\n*** Installing tqdm: *** (Required for PyPI uploads)\n")
         os.system("python -m pip install --upgrade tqdm")
         print("\n*** Rebuilding distribution packages: ***\n")
         os.system("python -m build")  # Create new tar/wheel
         print("\n*** Publishing The Release to PyPI: ***\n")
@@ -59,15 +59,15 @@
         print("\n*** The Release was PUBLISHED SUCCESSFULLY to PyPI! :) ***\n")
     else:
         print("\n>>> The Release was NOT PUBLISHED to PyPI! <<<\n")
     sys.exit()
 
 setup(
     name="pdbp",
-    version="1.4.0",
+    version="1.4.1",
     description="pdbp (Pdb+): A drop-in replacement for pdb and pdbpp.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="pdb debugger tab color completion",
     url="https://github.com/mdmintz/pdbp",
     project_urls={
         "Changelog": "https://github.com/mdmintz/pdbp/releases",
@@ -111,15 +111,14 @@
         "Topic :: Software Development :: Testing",
         "Topic :: Utilities",
     ],
     python_requires=">=3.6",
     install_requires=[
         'pygments>=2.14.0;python_version<"3.7"',
         'pygments>=2.15.1;python_version>="3.7"',
-        "tabcompleter>=1.2.0",
-        "six>=1.16.0",
+        "tabcompleter>=1.2.1",
     ],
     setup_requires=[],
     include_package_data=True,
 )
 
 print("\n*** pdbp (Pdb+) Installation Complete! ***\n")
```

### Comparing `pdbp-1.4.0/src/pdbp.egg-info/PKG-INFO` & `pdbp-1.4.1/src/pdbp.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdbp
-Version: 1.4.0
+Version: 1.4.1
 Summary: pdbp (Pdb+): A drop-in replacement for pdb and pdbpp.
 Home-page: https://github.com/mdmintz/pdbp
 Author: Michael Mintz
 Author-email: mdmintz@gmail.com
 Maintainer: Michael Mintz
 License: MIT
 Project-URL: Changelog, https://github.com/mdmintz/pdbp/releases
@@ -44,28 +44,28 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pdbp (Pdb+) [![](https://img.shields.io/pypi/v/pdbp.svg)](https://pypi.python.org/pypi/pdbp)
 
-<img width="650" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/234679015-b1daa50f-94a8-4ef2-b3f5-3157b7a3733b.png">
+<img width="660" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/247826485-d782911e-d817-4ea6-86dd-215991d7b8ea.png">
 
 --------
 
-**[pdbp (Pdb+)](https://github.com/mdmintz/pdbp)** is an advanced console debugger for Python. It can be used as a drop-in replacement for ``pdb`` and [pdbpp](https://github.com/pdbpp/pdbpp).
+**[pdbp (Pdb+)](https://github.com/mdmintz/pdbp)** is an advanced console debugger for Python. It can be used as a drop-in replacement for [pdb](https://docs.python.org/3/library/pdb.html) and [pdbpp](https://github.com/pdbpp/pdbpp).
 
 <p><b>pdbp (Pdb+)</b> makes Python debugging a lot easier (and more fun!)</p>
 
 --------
 
-<img width="650" alt="Pdb+" src="https://user-images.githubusercontent.com/6788579/234669562-30dae4ad-1207-47e4-8327-fbd5662c8b9c.png">
+<img width="650" alt="Pdb+" src="https://user-images.githubusercontent.com/6788579/234679015-b1daa50f-94a8-4ef2-b3f5-3157b7a3733b.png">
 
 
-## Installation & Usage:
+## Installation:
 
 ```bash
 pip install pdbp
 ```
 
 Then add ``import pdbp`` to an ``__init__.py`` of your project, which will automatically make **``Pdb+``** the default debugger at breakpoints:
 
@@ -75,16 +75,32 @@
 
 (If using ``flake8`` for code-linting, you may want to add ``# noqa`` to that line):
 
 ```python
 import pdbp  # noqa
 ```
 
+You can also make ``pdbp`` the default debugger by setting an environmental variable:
+
+```bash
+PYTHONBREAKPOINT=pdbp.set_trace
+```
+
+## Usage:
+
 To trigger a breakpoint in your code with ``pytest``, add ``--trace`` (to start tests with a breakpoint) or ``--pdb`` (to trigger a breakpoint if a test fails).
 
+To trigger a breakpoint from a pure ``python`` run, use:
+
+```bash
+python -m pdbp <script.py>
+```
+
+--------
+
 Basic **``Pdb+``** console commands: ``n``, ``c``, ``s`` => ``next``, ``continue``, ``step``.
 
 Use the ``u`` and ``d`` keys to travel ``up`` and ``down`` the stack!
 
 (To learn more **Pdb+** console commands, type ``help`` in the **Pdb+** console and press ``Enter/Return``.)
 
 --------
@@ -129,35 +145,42 @@
 <img width="640" alt="Pdb+ Post Mortem Debug Mode" src="https://user-images.githubusercontent.com/6788579/232537816-0b9e9048-724f-48cb-81e3-5cc403109de9.png">
 
 
 ### The ``where`` / ``w`` command, which displays the current stack:
 
 <img width="870" alt="Example of the 'where' command" src="https://user-images.githubusercontent.com/6788579/232962807-2d469603-a1d0-4891-8d0e-f03a4e1d0d00.png">
 
+--------
 
 ### Sticky Mode vs Non-Sticky Mode:
 
 The default mode (``sticky``) lets you see a lot more lines of code from the debugger when active. In Non-Sticky mode, only one line of code is shown at a time. You can switch between the two modes by typing ``sticky`` in the **Pdb+** console prompt and pressing ``Enter/Return``.
 
 > **Sticky Mode:**
 
 <img width="600" alt="Pdb+ Stick Mode" src="https://user-images.githubusercontent.com/6788579/204890148-53d2567b-9a56-4243-a7d7-66100a284312.png">
 
 > **Non-Sticky Mode:**
 
 <img width="600" alt="Pdb+ Non-Sticky Mode" src="https://user-images.githubusercontent.com/6788579/204890164-8465bc22-0f20-43f1-8ab7-b4316718a4c6.png">
 
+--------
+
+### Multi-layer highlighting in the same stack:
+
+<img width="536" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/207925754-4d4ffce5-be6c-44b6-b614-ae0e800a93d8.png">
+
 
 ### More examples:
 
 **``Pdb+``** is used by packages such as **``seleniumbase``**:
 
 * https://pypi.org/project/seleniumbase/
 * https://github.com/seleniumbase/SeleniumBase
 
 --------
 
-<img width="600" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/204896775-38d8551b-1d3c-4e95-9f5c-0e03c9de13da.png">
+<img width="650" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/234669562-30dae4ad-1207-47e4-8327-fbd5662c8b9c.png">
 
 --------
 
 (**Pdb+** is maintained by the [SeleniumBase Dev Team](https://github.com/seleniumbase/SeleniumBase))
```

### Comparing `pdbp-1.4.0/src/pdbp.py` & `pdbp-1.4.1/src/pdbp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """
 pdbp (Pdb+): A drop-in replacement for pdb and pdbpp.
 =====================================================
 """
-from __future__ import print_function
 import code
 import codecs
 import inspect
 import math
 import os.path
 import pprint
 import re
```

