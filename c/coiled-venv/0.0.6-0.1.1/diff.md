# Comparing `tmp/coiled-venv-0.0.6.tar.gz` & `tmp/coiled-venv-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coiled-venv-0.0.6.tar", last modified: Wed Feb  9 16:15:54 2022, max compression
+gzip compressed data, was "coiled-venv-0.1.1.tar", last modified: Wed Jun 21 23:11:40 2023, max compression
```

## Comparing `coiled-venv-0.0.6.tar` & `coiled-venv-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-09 16:15:54.659905 coiled-venv-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-02-09 16:15:43.000000 coiled-venv-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2407 2022-02-09 16:15:54.659905 coiled-venv-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1592 2022-02-09 16:15:43.000000 coiled-venv-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-09 16:15:54.659905 coiled-venv-0.0.6/coil/
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-02-09 16:15:43.000000 coiled-venv-0.0.6/coil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2253 2022-02-09 16:15:43.000000 coiled-venv-0.0.6/coil/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      436 2022-02-09 16:15:43.000000 coiled-venv-0.0.6/coil/config.py
--rw-r--r--   0 runner    (1001) docker     (121)      424 2022-02-09 16:15:43.000000 coiled-venv-0.0.6/coil/db.py
--rw-r--r--   0 runner    (1001) docker     (121)     1029 2022-02-09 16:15:43.000000 coiled-venv-0.0.6/coil/shell.py
--rw-r--r--   0 runner    (1001) docker     (121)     2034 2022-02-09 16:15:43.000000 coiled-venv-0.0.6/coil/venv.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-09 16:15:54.659905 coiled-venv-0.0.6/coiled_venv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2407 2022-02-09 16:15:54.000000 coiled-venv-0.0.6/coiled_venv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      291 2022-02-09 16:15:54.000000 coiled-venv-0.0.6/coiled_venv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-09 16:15:54.000000 coiled-venv-0.0.6/coiled_venv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-02-09 16:15:54.000000 coiled-venv-0.0.6/coiled_venv.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-02-09 16:15:54.000000 coiled-venv-0.0.6/coiled_venv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-09 16:15:54.659905 coiled-venv-0.0.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     1327 2022-02-09 16:15:43.000000 coiled-venv-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:11:40.587370 coiled-venv-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:11:40.583369 coiled-venv-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:11:40.583369 coiled-venv-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-21 23:11:15.000000 coiled-venv-0.1.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-21 23:11:15.000000 coiled-venv-0.1.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-21 23:11:15.000000 coiled-venv-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-21 23:11:15.000000 coiled-venv-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-21 23:11:40.587370 coiled-venv-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-06-21 23:11:15.000000 coiled-venv-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:11:40.587370 coiled-venv-0.1.1/coil/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-21 23:11:15.000000 coiled-venv-0.1.1/coil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-06-21 23:11:15.000000 coiled-venv-0.1.1/coil/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-21 23:11:15.000000 coiled-venv-0.1.1/coil/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-21 23:11:15.000000 coiled-venv-0.1.1/coil/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-21 23:11:15.000000 coiled-venv-0.1.1/coil/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-06-21 23:11:15.000000 coiled-venv-0.1.1/coil/venv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:11:40.587370 coiled-venv-0.1.1/coiled_venv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-21 23:11:40.000000 coiled-venv-0.1.1/coiled_venv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-21 23:11:40.000000 coiled-venv-0.1.1/coiled_venv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 23:11:40.000000 coiled-venv-0.1.1/coiled_venv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-21 23:11:40.000000 coiled-venv-0.1.1/coiled_venv.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-21 23:11:40.000000 coiled-venv-0.1.1/coiled_venv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-21 23:11:40.000000 coiled-venv-0.1.1/coiled_venv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-21 23:11:15.000000 coiled-venv-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 23:11:40.587370 coiled-venv-0.1.1/setup.cfg
```

### Comparing `coiled-venv-0.0.6/LICENSE` & `coiled-venv-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `coiled-venv-0.0.6/PKG-INFO` & `coiled-venv-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: coiled-venv
-Version: 0.0.6
+Version: 0.1.1
 Summary: Let it hatch, watch it coil (your python virtualenv)
-Home-page: https://github.com/fopina/coiled-venv
-Author: Filipe Pina
-Author-email: fopina@skmobi.com
+Author-email: Filipe Pina <fopina@skmobi.com>
 License: MIT
-Download-URL: https://github.com/fopina/coiled-venv/tarball/v0.0.6
 Keywords: productivity,virtual env,cleanup,cli
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 # coil
 Let it [hatch](https://github.com/ofek/hatch), watch it [coil](https://www.google.com/search?q=coiled+python&tbm=isch)
 
 [hatch](https://github.com/ofek/hatch) is a great virtualenv manager IMHO. But pure virtualenv management can be simpler!
 
@@ -66,9 +65,7 @@
 ➜ otherproject coil
 No env configured for /home/fopina/projects/otherproject
 ➜ myproject coil thisenv
 /home/fopina/.virtualenvs/thisenv assigned to /home/fopina/projects/otherproject
 /home/fopina/.virtualenvs/thisenv loaded
 (thisenv) ➜  otherproject 
 ```
-
-
```

### Comparing `coiled-venv-0.0.6/README.md` & `coiled-venv-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `coiled-venv-0.0.6/coil/shell.py` & `coiled-venv-0.1.1/coil/shell.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import os
 from pathlib import Path
 
 from . import config as C
 
+
 def zsh_shell(exe_dir, shell_path):
     rcfile = exe_dir / '.coil.zsh' / '.zshrc'
     rcfile.parent.mkdir(exist_ok=True)
     with open(rcfile, 'w') as f:
-        f.write(f'''\
+        f.write(
+            f'''\
 . ~/.zshrc
 . {exe_dir / 'activate'}
-''')
+'''
+        )
     os.environ['ZDOTDIR'] = str(rcfile.parent)
     os.execlp(shell_path or 'zsh', '-i')
 
 
 def bash_shell(exe_dir, shell_path):
     """
     TODO: windows support
@@ -43,8 +46,8 @@
 #     'csh': csh_shell,
 # }
 
 
 SHELL_COMMANDS = {
     'zsh': zsh_shell,
     'bash': bash_shell,
-}
+}
```

### Comparing `coiled-venv-0.0.6/coil/venv.py` & `coiled-venv-0.1.1/coil/venv.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,56 @@
 from pathlib import Path
+from typing import Optional
 import venv as pyvenv
 import random
 import shutil
 import subprocess
 
 from . import config as C, db, shell
 
 
 class VenvError(Exception):
     """
     errors managing virtualenvs
     """
 
 
-def bindir(path):
+def bindir(path) -> Optional[Path]:
     d = path / 'bin'
     if d.is_dir():
         return d
     if C.ON_WINDOWS:
         d = path / 'Scripts'
         if d.is_dir():
             return d
     return None
 
 
 def check(path):
     return bindir(path) is not None
 
 
+def fix_broken(name):
+    v = C.VENV_DIR / name
+    bin = bindir(v)
+    try:
+        subprocess.check_output([bin / 'python', '--version'], stderr=subprocess.PIPE)
+        return False
+    except subprocess.CalledProcessError:
+        pass
+
+    for pe in bin.glob('python*'):
+        if pe.is_file():
+            pe.unlink()
+    for pe in bin.glob('pip*'):
+        if pe.is_file():
+            pe.unlink()
+    return new(name=name)
+
+
 def list_available():
     for l in C.VENV_DIR.glob('*'):
         if check(l):
             yield l.name
 
 
 def load(path):
```

### Comparing `coiled-venv-0.0.6/coiled_venv.egg-info/PKG-INFO` & `coiled-venv-0.1.1/coiled_venv.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: coiled-venv
-Version: 0.0.6
+Version: 0.1.1
 Summary: Let it hatch, watch it coil (your python virtualenv)
-Home-page: https://github.com/fopina/coiled-venv
-Author: Filipe Pina
-Author-email: fopina@skmobi.com
+Author-email: Filipe Pina <fopina@skmobi.com>
 License: MIT
-Download-URL: https://github.com/fopina/coiled-venv/tarball/v0.0.6
 Keywords: productivity,virtual env,cleanup,cli
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 # coil
 Let it [hatch](https://github.com/ofek/hatch), watch it [coil](https://www.google.com/search?q=coiled+python&tbm=isch)
 
 [hatch](https://github.com/ofek/hatch) is a great virtualenv manager IMHO. But pure virtualenv management can be simpler!
 
@@ -66,9 +65,7 @@
 ➜ otherproject coil
 No env configured for /home/fopina/projects/otherproject
 ➜ myproject coil thisenv
 /home/fopina/.virtualenvs/thisenv assigned to /home/fopina/projects/otherproject
 /home/fopina/.virtualenvs/thisenv loaded
 (thisenv) ➜  otherproject 
 ```
-
-
```

