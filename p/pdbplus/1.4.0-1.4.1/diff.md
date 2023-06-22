# Comparing `tmp/pdbplus-1.4.0.tar.gz` & `tmp/pdbplus-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdbplus-1.4.0.tar", last modified: Wed Apr 26 19:54:14 2023, max compression
+gzip compressed data, was "pdbplus-1.4.1.tar", last modified: Thu Jun 22 15:56:45 2023, max compression
```

## Comparing `pdbplus-1.4.0.tar` & `pdbplus-1.4.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-26 19:54:14.325675 pdbplus-1.4.0/
--rw-r--r--   0 michael    (501) staff       (20)    10439 2023-04-26 19:54:14.325459 pdbplus-1.4.0/PKG-INFO
--rwxr-xr-x   0 michael    (501) staff       (20)     8486 2023-04-26 19:16:20.000000 pdbplus-1.4.0/README.md
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-26 19:54:14.325242 pdbplus-1.4.0/pdbplus.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)    10439 2023-04-26 19:54:14.000000 pdbplus-1.4.0/pdbplus.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      172 2023-04-26 19:54:14.000000 pdbplus-1.4.0/pdbplus.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-04-26 19:54:14.000000 pdbplus-1.4.0/pdbplus.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)       12 2023-04-26 19:54:14.000000 pdbplus-1.4.0/pdbplus.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-04-26 19:54:14.000000 pdbplus-1.4.0/pdbplus.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) staff       (20)       38 2023-04-26 19:54:14.325708 pdbplus-1.4.0/setup.cfg
--rwxr-xr-x   0 michael    (501) staff       (20)     4948 2023-04-26 16:43:02.000000 pdbplus-1.4.0/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-22 15:56:45.974635 pdbplus-1.4.1/
+-rw-r--r--   0 michael    (501) staff       (20)     7052 2023-06-22 15:56:45.974538 pdbplus-1.4.1/PKG-INFO
+-rwxr-xr-x   0 michael    (501) staff       (20)     5099 2023-06-22 14:53:13.000000 pdbplus-1.4.1/README.md
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-22 15:56:45.974405 pdbplus-1.4.1/pdbplus.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)     7052 2023-06-22 15:56:45.000000 pdbplus-1.4.1/pdbplus.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      172 2023-06-22 15:56:45.000000 pdbplus-1.4.1/pdbplus.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-06-22 15:56:45.000000 pdbplus-1.4.1/pdbplus.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)       12 2023-06-22 15:56:45.000000 pdbplus-1.4.1/pdbplus.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-06-22 15:56:45.000000 pdbplus-1.4.1/pdbplus.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) staff       (20)       38 2023-06-22 15:56:45.974664 pdbplus-1.4.1/setup.cfg
+-rwxr-xr-x   0 michael    (501) staff       (20)     5032 2023-06-22 15:22:19.000000 pdbplus-1.4.1/setup.py
```

### Comparing `pdbplus-1.4.0/PKG-INFO` & `pdbplus-1.4.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdbplus
-Version: 1.4.0
+Version: 1.4.1
 Summary: pdbp (Pdb+): A drop-in replacement for pdb and pdbpp.
 Home-page: https://github.com/mdmintz/pdbp
 Author: Michael Mintz
 Author-email: mdmintz@gmail.com
 Maintainer: Michael Mintz
 License: MIT
 Project-URL: Changelog, https://github.com/mdmintz/pdbp/releases
@@ -47,28 +47,28 @@
 **[<img src="https://img.shields.io/badge/pypi-pdbplus-22AAEE.svg" alt="pypi" />](https://pypi.python.org/pypi/pdbplus) is a proxy for installing [<img src="https://img.shields.io/badge/pypi-pdbp-22AAEE.svg" alt="pypi" />](https://pypi.python.org/pypi/pdbp) (Pdb+).**
 ****
 
 <!-- Pdb+ Docs -->
 
 # pdbp (Pdb+) [![](https://img.shields.io/pypi/v/pdbp.svg)](https://pypi.python.org/pypi/pdbp)
 
-<img width="600" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/234679015-b1daa50f-94a8-4ef2-b3f5-3157b7a3733b.png">
+<img width="660" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/247826485-d782911e-d817-4ea6-86dd-215991d7b8ea.png">
 
 --------
 
-**[pdbp (Pdb+)](https://github.com/mdmintz/pdbp)** is an advanced console debugger for Python. It can be used as a drop-in replacement for ``pdb`` and [pdbpp](https://github.com/pdbpp/pdbpp).
+**[pdbp (Pdb+)](https://github.com/mdmintz/pdbp)** is an advanced console debugger for Python. It can be used as a drop-in replacement for [pdb](https://docs.python.org/3/library/pdb.html) and [pdbpp](https://github.com/pdbpp/pdbpp).
 
 <p><b>pdbp (Pdb+)</b> makes Python debugging a lot easier (and more fun!)</p>
 
 --------
 
-<img width="600" alt="Pdb+" src="https://user-images.githubusercontent.com/6788579/234669562-30dae4ad-1207-47e4-8327-fbd5662c8b9c.png">
+<img width="650" alt="Pdb+" src="https://user-images.githubusercontent.com/6788579/234679015-b1daa50f-94a8-4ef2-b3f5-3157b7a3733b.png">
 
 
-## Installation & Usage:
+## Installation:
 
 ```bash
 pip install pdbp
 ```
 
 Then add ``import pdbp`` to an ``__init__.py`` of your project, which will automatically make **``Pdb+``** the default debugger at breakpoints:
 
@@ -78,118 +78,31 @@
 
 (If using ``flake8`` for code-linting, you may want to add ``# noqa`` to that line):
 
 ```python
 import pdbp  # noqa
 ```
 
-To trigger a breakpoint in your code with ``pytest``, add ``--trace`` (to start tests with a breakpoint) or ``--pdb`` (to trigger a breakpoint if a test fails).
-
-Basic **``Pdb+``** console commands: ``n``, ``c``, ``s`` => ``next``, ``continue``, ``step``.
-
-(To learn more **Pdb+** console commands, type ``help`` in the **Pdb+** console and press ``Enter/Return``.)
-
---------
-
-**``pdbp`` (Pdb+)** makes improvements to ``pdbpp`` so that it works in all environments. It also includes other bug-fixes. "Sticky" mode is the default option, which shows multiple lines of code while letting you see where you're going (while typing ``n`` + ``Enter``).
-
-If you somehow reset ``pdb`` to Python's built-in version, you can always replace ``pdb`` with **``pdbp``** again as the default debugger by running this:
-
-```python
-import pdb
-import pdbp
-for key in pdbp.__dict__.keys():
-    pdb.__dict__[key] = pdbp.__dict__[key]
-```
-
-Here's how to customize **``pdbp``**/``pdb`` options if you don't like the default settings: (<i>Shown below are the default settings.</i>)
-
-```python
-import pdb
-if hasattr(pdb, "DefaultConfig"):
-    pdb.DefaultConfig.filename_color = pdb.Color.fuchsia
-    pdb.DefaultConfig.line_number_color = pdb.Color.turquoise
-    pdb.DefaultConfig.truncate_long_lines = False
-    pdb.DefaultConfig.sticky_by_default = True
-```
-
-You can also trigger **``Pdb+``** activation like this:
-
-```python
-import pdbp
-pdbp.set_trace()
-```
-
-
-### pdbp (Pdb+) commands:
-
-<img width="550" alt="Pdb+ Commands" src="https://user-images.githubusercontent.com/6788579/204386211-5fc44f73-e29f-4e87-b0ca-bb8ea69217af.png">
-
-
-### Sticky Mode vs Non-Sticky Mode:
-
-The default mode (``sticky``) lets you see a lot more lines of code from the debugger when active. In Non-Sticky mode, only one line of code is shown at a time. You can switch between the two modes by typing ``sticky`` in the **Pdb+** console prompt and pressing ``Enter/Return``.
-
-> **Sticky Mode:**
-
-<img width="550" alt="Pdb+ Stick Mode" src="https://user-images.githubusercontent.com/6788579/204890148-53d2567b-9a56-4243-a7d7-66100a284312.png">
-
-> **Non-Sticky Mode:**
-
-<img width="550" alt="Pdb+ Non-Sticky Mode" src="https://user-images.githubusercontent.com/6788579/204890164-8465bc22-0f20-43f1-8ab7-b4316718a4c6.png">
-
-
-### More examples:
-
-**``Pdb+``** is used by packages such as **``seleniumbase``**:
-
-* https://pypi.org/project/seleniumbase/
-* https://github.com/seleniumbase/SeleniumBase
-
---------
-
-<img width="550" alt="Pdb+" src="https://user-images.githubusercontent.com/6788579/204359676-137cf541-12ef-469a-9d29-99709608ede0.png">
-
---------
-
-(**Pdb+** is maintained by the [SeleniumBase Dev Team](https://github.com/seleniumbase/SeleniumBase))
-# pdbp (Pdb+) [![](https://img.shields.io/pypi/v/pdbp.svg)](https://pypi.python.org/pypi/pdbp)
-
-<img width="650" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/207774790-fb63af65-5f98-4d92-afe3-12c2733d4db6.png">
-
---------
-
-**[pdbp (Pdb+)](https://github.com/mdmintz/pdbp)** is an advanced console debugger for Python. It can be used as a drop-in replacement for ``pdb`` and [pdbpp](https://github.com/pdbpp/pdbpp).
-
-<p><b>pdbp (Pdb+)</b> makes Python debugging a lot easier (and more fun!)</p>
-
---------
-
-<img width="650" alt="Pdb+" src="https://user-images.githubusercontent.com/6788579/232536483-9236c513-c5ba-4444-8faa-e8ea64eb5ce2.png">
-
-
-## Installation & Usage:
+You can also make ``pdbp`` the default debugger by setting an environmental variable:
 
 ```bash
-pip install pdbp
+PYTHONBREAKPOINT=pdbp.set_trace
 ```
 
-Then add ``import pdbp`` to an ``__init__.py`` of your project, which will automatically make **``Pdb+``** the default debugger at breakpoints:
+## Usage:
 
-```python
-import pdbp
-```
+To trigger a breakpoint in your code with ``pytest``, add ``--trace`` (to start tests with a breakpoint) or ``--pdb`` (to trigger a breakpoint if a test fails).
 
-(If using ``flake8`` for code-linting, you may want to add ``# noqa`` to that line):
+To trigger a breakpoint from a pure ``python`` run, use:
 
-```python
-import pdbp  # noqa
+```bash
+python -m pdbp <script.py>
 ```
 
-To trigger a breakpoint in your code with ``pytest``, add ``--trace`` (to start tests with a breakpoint) or ``--pdb`` (to trigger a breakpoint if a test fails).
+--------
 
 Basic **``Pdb+``** console commands: ``n``, ``c``, ``s`` => ``next``, ``continue``, ``step``.
 
 Use the ``u`` and ``d`` keys to travel ``up`` and ``down`` the stack!
 
 (To learn more **Pdb+** console commands, type ``help`` in the **Pdb+** console and press ``Enter/Return``.)
 
@@ -207,20 +120,17 @@
 ```
 
 Here's how to customize **``pdbp``**/``pdb`` options if you don't like the default settings: (<i>Shown below are the default settings.</i>)
 
 ```python
 import pdb
 if hasattr(pdb, "DefaultConfig"):
-    pdb.DefaultConfig.filename_color = pdb.Color.blue
+    pdb.DefaultConfig.filename_color = pdb.Color.fuchsia
     pdb.DefaultConfig.line_number_color = pdb.Color.turquoise
-    pdb.DefaultConfig.show_hidden_frames_count = False
-    pdb.DefaultConfig.disable_pytest_capturing = True
-    pdb.DefaultConfig.enable_hidden_frames = False
-    pdb.DefaultConfig.truncate_long_lines = True
+    pdb.DefaultConfig.truncate_long_lines = False
     pdb.DefaultConfig.sticky_by_default = True
 ```
 
 You can also trigger **``Pdb+``** activation like this:
 
 ```python
 import pdbp
@@ -238,35 +148,42 @@
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

### Comparing `pdbplus-1.4.0/README.md` & `pdbplus-1.4.1/pdbplus.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,74 @@
+Metadata-Version: 2.1
+Name: pdbplus
+Version: 1.4.1
+Summary: pdbp (Pdb+): A drop-in replacement for pdb and pdbpp.
+Home-page: https://github.com/mdmintz/pdbp
+Author: Michael Mintz
+Author-email: mdmintz@gmail.com
+Maintainer: Michael Mintz
+License: MIT
+Project-URL: Changelog, https://github.com/mdmintz/pdbp/releases
+Project-URL: Download, https://pypi.org/project/pdbp/#files
+Project-URL: Bug Tracker, https://github.com/mdmintz/pdbp/issues
+Project-URL: PyPI, https://pypi.org/project/pdbp/
+Project-URL: Source, https://github.com/mdmintz/pdbp
+Platform: Windows
+Platform: Linux
+Platform: Mac OS-X
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Environment :: MacOS X
+Classifier: Environment :: Win32 (MS Windows)
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Debuggers
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Quality Assurance
+Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: Utilities
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
 **[<img src="https://img.shields.io/badge/pypi-pdbplus-22AAEE.svg" alt="pypi" />](https://pypi.python.org/pypi/pdbplus) is a proxy for installing [<img src="https://img.shields.io/badge/pypi-pdbp-22AAEE.svg" alt="pypi" />](https://pypi.python.org/pypi/pdbp) (Pdb+).**
 ****
 
 <!-- Pdb+ Docs -->
 
 # pdbp (Pdb+) [![](https://img.shields.io/pypi/v/pdbp.svg)](https://pypi.python.org/pypi/pdbp)
 
-<img width="600" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/234679015-b1daa50f-94a8-4ef2-b3f5-3157b7a3733b.png">
+<img width="660" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/247826485-d782911e-d817-4ea6-86dd-215991d7b8ea.png">
 
 --------
 
-**[pdbp (Pdb+)](https://github.com/mdmintz/pdbp)** is an advanced console debugger for Python. It can be used as a drop-in replacement for ``pdb`` and [pdbpp](https://github.com/pdbpp/pdbpp).
+**[pdbp (Pdb+)](https://github.com/mdmintz/pdbp)** is an advanced console debugger for Python. It can be used as a drop-in replacement for [pdb](https://docs.python.org/3/library/pdb.html) and [pdbpp](https://github.com/pdbpp/pdbpp).
 
 <p><b>pdbp (Pdb+)</b> makes Python debugging a lot easier (and more fun!)</p>
 
 --------
 
-<img width="600" alt="Pdb+" src="https://user-images.githubusercontent.com/6788579/234669562-30dae4ad-1207-47e4-8327-fbd5662c8b9c.png">
+<img width="650" alt="Pdb+" src="https://user-images.githubusercontent.com/6788579/234679015-b1daa50f-94a8-4ef2-b3f5-3157b7a3733b.png">
 
 
-## Installation & Usage:
+## Installation:
 
 ```bash
 pip install pdbp
 ```
 
 Then add ``import pdbp`` to an ``__init__.py`` of your project, which will automatically make **``Pdb+``** the default debugger at breakpoints:
 
@@ -32,118 +78,31 @@
 
 (If using ``flake8`` for code-linting, you may want to add ``# noqa`` to that line):
 
 ```python
 import pdbp  # noqa
 ```
 
-To trigger a breakpoint in your code with ``pytest``, add ``--trace`` (to start tests with a breakpoint) or ``--pdb`` (to trigger a breakpoint if a test fails).
-
-Basic **``Pdb+``** console commands: ``n``, ``c``, ``s`` => ``next``, ``continue``, ``step``.
-
-(To learn more **Pdb+** console commands, type ``help`` in the **Pdb+** console and press ``Enter/Return``.)
-
---------
-
-**``pdbp`` (Pdb+)** makes improvements to ``pdbpp`` so that it works in all environments. It also includes other bug-fixes. "Sticky" mode is the default option, which shows multiple lines of code while letting you see where you're going (while typing ``n`` + ``Enter``).
-
-If you somehow reset ``pdb`` to Python's built-in version, you can always replace ``pdb`` with **``pdbp``** again as the default debugger by running this:
-
-```python
-import pdb
-import pdbp
-for key in pdbp.__dict__.keys():
-    pdb.__dict__[key] = pdbp.__dict__[key]
-```
-
-Here's how to customize **``pdbp``**/``pdb`` options if you don't like the default settings: (<i>Shown below are the default settings.</i>)
-
-```python
-import pdb
-if hasattr(pdb, "DefaultConfig"):
-    pdb.DefaultConfig.filename_color = pdb.Color.fuchsia
-    pdb.DefaultConfig.line_number_color = pdb.Color.turquoise
-    pdb.DefaultConfig.truncate_long_lines = False
-    pdb.DefaultConfig.sticky_by_default = True
-```
-
-You can also trigger **``Pdb+``** activation like this:
-
-```python
-import pdbp
-pdbp.set_trace()
-```
-
-
-### pdbp (Pdb+) commands:
-
-<img width="550" alt="Pdb+ Commands" src="https://user-images.githubusercontent.com/6788579/204386211-5fc44f73-e29f-4e87-b0ca-bb8ea69217af.png">
-
-
-### Sticky Mode vs Non-Sticky Mode:
-
-The default mode (``sticky``) lets you see a lot more lines of code from the debugger when active. In Non-Sticky mode, only one line of code is shown at a time. You can switch between the two modes by typing ``sticky`` in the **Pdb+** console prompt and pressing ``Enter/Return``.
-
-> **Sticky Mode:**
-
-<img width="550" alt="Pdb+ Stick Mode" src="https://user-images.githubusercontent.com/6788579/204890148-53d2567b-9a56-4243-a7d7-66100a284312.png">
-
-> **Non-Sticky Mode:**
-
-<img width="550" alt="Pdb+ Non-Sticky Mode" src="https://user-images.githubusercontent.com/6788579/204890164-8465bc22-0f20-43f1-8ab7-b4316718a4c6.png">
-
-
-### More examples:
-
-**``Pdb+``** is used by packages such as **``seleniumbase``**:
-
-* https://pypi.org/project/seleniumbase/
-* https://github.com/seleniumbase/SeleniumBase
-
---------
-
-<img width="550" alt="Pdb+" src="https://user-images.githubusercontent.com/6788579/204359676-137cf541-12ef-469a-9d29-99709608ede0.png">
-
---------
-
-(**Pdb+** is maintained by the [SeleniumBase Dev Team](https://github.com/seleniumbase/SeleniumBase))
-# pdbp (Pdb+) [![](https://img.shields.io/pypi/v/pdbp.svg)](https://pypi.python.org/pypi/pdbp)
-
-<img width="650" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/207774790-fb63af65-5f98-4d92-afe3-12c2733d4db6.png">
-
---------
-
-**[pdbp (Pdb+)](https://github.com/mdmintz/pdbp)** is an advanced console debugger for Python. It can be used as a drop-in replacement for ``pdb`` and [pdbpp](https://github.com/pdbpp/pdbpp).
-
-<p><b>pdbp (Pdb+)</b> makes Python debugging a lot easier (and more fun!)</p>
-
---------
-
-<img width="650" alt="Pdb+" src="https://user-images.githubusercontent.com/6788579/232536483-9236c513-c5ba-4444-8faa-e8ea64eb5ce2.png">
-
-
-## Installation & Usage:
+You can also make ``pdbp`` the default debugger by setting an environmental variable:
 
 ```bash
-pip install pdbp
+PYTHONBREAKPOINT=pdbp.set_trace
 ```
 
-Then add ``import pdbp`` to an ``__init__.py`` of your project, which will automatically make **``Pdb+``** the default debugger at breakpoints:
+## Usage:
 
-```python
-import pdbp
-```
+To trigger a breakpoint in your code with ``pytest``, add ``--trace`` (to start tests with a breakpoint) or ``--pdb`` (to trigger a breakpoint if a test fails).
 
-(If using ``flake8`` for code-linting, you may want to add ``# noqa`` to that line):
+To trigger a breakpoint from a pure ``python`` run, use:
 
-```python
-import pdbp  # noqa
+```bash
+python -m pdbp <script.py>
 ```
 
-To trigger a breakpoint in your code with ``pytest``, add ``--trace`` (to start tests with a breakpoint) or ``--pdb`` (to trigger a breakpoint if a test fails).
+--------
 
 Basic **``Pdb+``** console commands: ``n``, ``c``, ``s`` => ``next``, ``continue``, ``step``.
 
 Use the ``u`` and ``d`` keys to travel ``up`` and ``down`` the stack!
 
 (To learn more **Pdb+** console commands, type ``help`` in the **Pdb+** console and press ``Enter/Return``.)
 
@@ -161,20 +120,17 @@
 ```
 
 Here's how to customize **``pdbp``**/``pdb`` options if you don't like the default settings: (<i>Shown below are the default settings.</i>)
 
 ```python
 import pdb
 if hasattr(pdb, "DefaultConfig"):
-    pdb.DefaultConfig.filename_color = pdb.Color.blue
+    pdb.DefaultConfig.filename_color = pdb.Color.fuchsia
     pdb.DefaultConfig.line_number_color = pdb.Color.turquoise
-    pdb.DefaultConfig.show_hidden_frames_count = False
-    pdb.DefaultConfig.disable_pytest_capturing = True
-    pdb.DefaultConfig.enable_hidden_frames = False
-    pdb.DefaultConfig.truncate_long_lines = True
+    pdb.DefaultConfig.truncate_long_lines = False
     pdb.DefaultConfig.sticky_by_default = True
 ```
 
 You can also trigger **``Pdb+``** activation like this:
 
 ```python
 import pdbp
@@ -192,35 +148,42 @@
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

### Comparing `pdbplus-1.4.0/setup.py` & `pdbplus-1.4.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,37 +18,37 @@
     long_description = "\n".join(long_description_lines)
 except IOError:
     long_description = "pdbp (Pdb+): A drop-in replacement for pdb and pdbpp."
 
 if sys.argv[-1] == 'publish':
     reply = None
     input_method = input
-    if not sys.version_info[0] >= 3:
-        input_method = raw_input  # noqa
     reply = str(input_method(
         '>>> Confirm release PUBLISH to PyPI? (yes/no): ')).lower().strip()
     if reply == 'yes':
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
@@ -56,15 +56,15 @@
         print("\n*** The Release was PUBLISHED SUCCESSFULLY to PyPI! :) ***\n")
     else:
         print("\n>>> The Release was NOT PUBLISHED to PyPI! <<<\n")
     sys.exit()
 
 setup(
     name='pdbplus',
-    version='1.4.0',
+    version='1.4.1',
     description="pdbp (Pdb+): A drop-in replacement for pdb and pdbpp.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/mdmintz/pdbp",
     project_urls={
         "Changelog": "https://github.com/mdmintz/pdbp/releases",
         "Download": "https://pypi.org/project/pdbp/#files",
@@ -103,14 +103,14 @@
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Quality Assurance",
         "Topic :: Software Development :: Testing",
         "Topic :: Utilities",
     ],
     python_requires=">=3.6",
     install_requires=[
-        'pdbp>=1.4.0',
+        'pdbp>=1.4.1',
     ],
     setup_requires=[],
     packages=[],
 )
 
 print("\n*** pdbplus Installation Complete! ***\n")
```

