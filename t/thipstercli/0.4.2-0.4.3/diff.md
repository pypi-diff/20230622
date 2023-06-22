# Comparing `tmp/thipstercli-0.4.2.tar.gz` & `tmp/thipstercli-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thipstercli-0.4.2.tar", last modified: Wed Jun 21 14:49:24 2023, max compression
+gzip compressed data, was "thipstercli-0.4.3.tar", last modified: Thu Jun 22 10:30:59 2023, max compression
```

## Comparing `thipstercli-0.4.2.tar` & `thipstercli-0.4.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 14:49:24.500550 thipstercli-0.4.2/
--rw-r--r--   0 root         (0) root         (0)     1052 2023-06-21 14:49:20.000000 thipstercli-0.4.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5204 2023-06-21 14:49:24.500550 thipstercli-0.4.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4516 2023-06-21 14:49:20.000000 thipstercli-0.4.2/README.md
--rw-r--r--   0 root         (0) root         (0)     1361 2023-06-21 14:49:20.000000 thipstercli-0.4.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-21 14:49:24.500550 thipstercli-0.4.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1823 2023-06-21 14:49:20.000000 thipstercli-0.4.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 14:49:24.500550 thipstercli-0.4.2/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 14:49:20.000000 thipstercli-0.4.2/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1730 2023-06-21 14:49:20.000000 thipstercli-0.4.2/tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)     3847 2023-06-21 14:49:20.000000 thipstercli-0.4.2/tests/test_cli.py
--rw-r--r--   0 root         (0) root         (0)     2874 2023-06-21 14:49:20.000000 thipstercli-0.4.2/tests/test_info.py
--rw-r--r--   0 root         (0) root         (0)     3155 2023-06-21 14:49:20.000000 thipstercli-0.4.2/tests/test_providers.py
--rw-r--r--   0 root         (0) root         (0)     1669 2023-06-21 14:49:20.000000 thipstercli-0.4.2/tests/test_repository.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 14:49:24.500550 thipstercli-0.4.2/thipstercli/
--rw-r--r--   0 root         (0) root         (0)      105 2023-06-21 14:49:20.000000 thipstercli-0.4.2/thipstercli/__init__.py
--rw-r--r--   0 root         (0) root         (0)      118 2023-06-21 14:49:20.000000 thipstercli-0.4.2/thipstercli/__main__.py
--rw-r--r--   0 root         (0) root         (0)     6315 2023-06-21 14:49:20.000000 thipstercli-0.4.2/thipstercli/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 14:49:24.500550 thipstercli-0.4.2/thipstercli/commands/
--rw-r--r--   0 root         (0) root         (0)      131 2023-06-21 14:49:20.000000 thipstercli-0.4.2/thipstercli/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8194 2023-06-21 14:49:20.000000 thipstercli-0.4.2/thipstercli/commands/info.py
--rw-r--r--   0 root         (0) root         (0)     2312 2023-06-21 14:49:20.000000 thipstercli-0.4.2/thipstercli/commands/providers.py
--rw-r--r--   0 root         (0) root         (0)     3471 2023-06-21 14:49:20.000000 thipstercli-0.4.2/thipstercli/commands/repository.py
--rw-r--r--   0 root         (0) root         (0)     1881 2023-06-21 14:49:20.000000 thipstercli-0.4.2/thipstercli/config.py
--rw-r--r--   0 root         (0) root         (0)      296 2023-06-21 14:49:20.000000 thipstercli-0.4.2/thipstercli/constants.py
--rw-r--r--   0 root         (0) root         (0)     1249 2023-06-21 14:49:20.000000 thipstercli-0.4.2/thipstercli/display.py
--rw-r--r--   0 root         (0) root         (0)     2686 2023-06-21 14:49:20.000000 thipstercli-0.4.2/thipstercli/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 14:49:24.500550 thipstercli-0.4.2/thipstercli.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5204 2023-06-21 14:49:24.000000 thipstercli-0.4.2/thipstercli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      666 2023-06-21 14:49:24.000000 thipstercli-0.4.2/thipstercli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 14:49:24.000000 thipstercli-0.4.2/thipstercli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       54 2023-06-21 14:49:24.000000 thipstercli-0.4.2/thipstercli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      284 2023-06-21 14:49:24.000000 thipstercli-0.4.2/thipstercli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-21 14:49:24.000000 thipstercli-0.4.2/thipstercli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 10:30:59.525079 thipstercli-0.4.3/
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-06-22 10:30:54.000000 thipstercli-0.4.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5204 2023-06-22 10:30:59.525079 thipstercli-0.4.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4516 2023-06-22 10:30:54.000000 thipstercli-0.4.3/README.md
+-rw-r--r--   0 root         (0) root         (0)     1372 2023-06-22 10:30:54.000000 thipstercli-0.4.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 10:30:59.525079 thipstercli-0.4.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1823 2023-06-22 10:30:55.000000 thipstercli-0.4.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 10:30:59.521079 thipstercli-0.4.3/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 10:30:54.000000 thipstercli-0.4.3/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1730 2023-06-22 10:30:54.000000 thipstercli-0.4.3/tests/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     3847 2023-06-22 10:30:54.000000 thipstercli-0.4.3/tests/test_cli.py
+-rw-r--r--   0 root         (0) root         (0)     2874 2023-06-22 10:30:54.000000 thipstercli-0.4.3/tests/test_info.py
+-rw-r--r--   0 root         (0) root         (0)     3155 2023-06-22 10:30:54.000000 thipstercli-0.4.3/tests/test_providers.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-06-22 10:30:54.000000 thipstercli-0.4.3/tests/test_repository.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 10:30:59.525079 thipstercli-0.4.3/thipstercli/
+-rw-r--r--   0 root         (0) root         (0)      105 2023-06-22 10:30:54.000000 thipstercli-0.4.3/thipstercli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      118 2023-06-22 10:30:54.000000 thipstercli-0.4.3/thipstercli/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     6309 2023-06-22 10:30:54.000000 thipstercli-0.4.3/thipstercli/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 10:30:59.525079 thipstercli-0.4.3/thipstercli/commands/
+-rw-r--r--   0 root         (0) root         (0)      131 2023-06-22 10:30:54.000000 thipstercli-0.4.3/thipstercli/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8194 2023-06-22 10:30:54.000000 thipstercli-0.4.3/thipstercli/commands/info.py
+-rw-r--r--   0 root         (0) root         (0)     2312 2023-06-22 10:30:54.000000 thipstercli-0.4.3/thipstercli/commands/providers.py
+-rw-r--r--   0 root         (0) root         (0)     3471 2023-06-22 10:30:54.000000 thipstercli-0.4.3/thipstercli/commands/repository.py
+-rw-r--r--   0 root         (0) root         (0)     1881 2023-06-22 10:30:54.000000 thipstercli-0.4.3/thipstercli/config.py
+-rw-r--r--   0 root         (0) root         (0)      296 2023-06-22 10:30:54.000000 thipstercli-0.4.3/thipstercli/constants.py
+-rw-r--r--   0 root         (0) root         (0)     1249 2023-06-22 10:30:54.000000 thipstercli-0.4.3/thipstercli/display.py
+-rw-r--r--   0 root         (0) root         (0)     2686 2023-06-22 10:30:54.000000 thipstercli-0.4.3/thipstercli/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 10:30:59.525079 thipstercli-0.4.3/thipstercli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5204 2023-06-22 10:30:59.000000 thipstercli-0.4.3/thipstercli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      666 2023-06-22 10:30:59.000000 thipstercli-0.4.3/thipstercli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 10:30:59.000000 thipstercli-0.4.3/thipstercli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       54 2023-06-22 10:30:59.000000 thipstercli-0.4.3/thipstercli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      284 2023-06-22 10:30:59.000000 thipstercli-0.4.3/thipstercli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-22 10:30:59.000000 thipstercli-0.4.3/thipstercli.egg-info/top_level.txt
```

### Comparing `thipstercli-0.4.2/LICENSE` & `thipstercli-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `thipstercli-0.4.2/PKG-INFO` & `thipstercli-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipstercli
-Version: 0.4.2
+Version: 0.4.3
 Summary: CLI interface build with typer, designed to use the thipster package
 Home-page: https://github.com/THipster/THipster-cli
 Download-URL: https://github.com/THipster/THipster-cli.git
 License: MIT
 Keywords: thipster,cli,generator,infrastructure as code,iac,terraform,typer
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thipstercli Version: 0.4.2 Summary: CLI interface
+Metadata-Version: 2.1 Name: thipstercli Version: 0.4.3 Summary: CLI interface
 build with typer, designed to use the thipster package Home-page: https://
 github.com/THipster/THipster-cli Download-URL: https://github.com/THipster/
 THipster-cli.git License: MIT Keywords: thipster,cli,generator,infrastructure
 as code,iac,terraform,typer Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console Classifier: Programming Language :: Python
 :: 3.11 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
```

### Comparing `thipstercli-0.4.2/README.md` & `thipstercli-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `thipstercli-0.4.2/pyproject.toml` & `thipstercli-0.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     "INP",
     "PYI",
     "PTH",
     "Q",
     "RSE",
     "RET",
     "SIM",
+    "SLF",
     "TID",
     "ARG",
     "RUF",
 ]
 
 [tool.ruff.pydocstyle]
 # Use Google-style docstrings.
```

### Comparing `thipstercli-0.4.2/setup.py` & `thipstercli-0.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     for req_file in Path('.').glob('requirements-*.txt'):
         extras_require[
             req_file.stem.removeprefix('requirements-')
         ] = req_file.read_text().splitlines()
     return extras_require
 
 
-__version__ = '0.4.2'
+__version__ = '0.4.3'
 
 with Path('requirements.txt').open() as f:
     required = f.read().splitlines()
 
 with Path('README.md').open() as f:
     long_description = f.read()
```

### Comparing `thipstercli-0.4.2/tests/conftest.py` & `thipstercli-0.4.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.4.2/tests/test_cli.py` & `thipstercli-0.4.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.4.2/tests/test_info.py` & `thipstercli-0.4.3/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.4.2/tests/test_providers.py` & `thipstercli-0.4.3/tests/test_providers.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.4.2/tests/test_repository.py` & `thipstercli-0.4.3/tests/test_repository.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.4.2/thipstercli/cli.py` & `thipstercli-0.4.3/thipstercli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,35 +126,35 @@
         authentification_provider,
         Terraform(),
     )
     print_if_verbose('Engine start-up successful! :rocket:')
 
     try:
         print_start_if_verbose('Parsing files')
-        parsed_file = engine._parse_files(path)
+        parsed_file = engine.parse_files(path)
         print_success_if_verbose('Parsing successful!')
 
         print_start_if_verbose('Retrieving models')
-        models = engine._get_models(parsed_file)
+        models = engine.get_models(parsed_file)
         print_success_if_verbose('Models retrieved!')
 
         print_start_if_verbose('Generating Terraform files')
-        engine._generate_tf_files(parsed_file, models)
+        engine.generate_tf_files(parsed_file, models)
         print_success_if_verbose('Terraform files generated!')
 
         print_start_if_verbose('Initializing Terraform')
-        engine._init_terraform()
+        engine.init_terraform()
         print_success_if_verbose('Terraform initialized!')
 
         print_start_if_verbose('Creating Terraform plan')
-        print(engine._plan_terraform())
+        print(engine.plan_terraform())
 
         if apply:
             print("Type 'yes' to apply the changes : ")
-            print(engine._apply_terraform())
+            print(engine.apply_terraform())
 
         print_if_verbose('Done! :tada:')
 
     except THipsterError as e:
         error(e.message)
     except FileNotFoundError as e:
         error(
```

### Comparing `thipstercli-0.4.2/thipstercli/commands/info.py` & `thipstercli-0.4.3/thipstercli/commands/info.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.4.2/thipstercli/commands/providers.py` & `thipstercli-0.4.3/thipstercli/commands/providers.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.4.2/thipstercli/commands/repository.py` & `thipstercli-0.4.3/thipstercli/commands/repository.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.4.2/thipstercli/config.py` & `thipstercli-0.4.3/thipstercli/config.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.4.2/thipstercli/display.py` & `thipstercli-0.4.3/thipstercli/display.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.4.2/thipstercli/helpers.py` & `thipstercli-0.4.3/thipstercli/helpers.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.4.2/thipstercli.egg-info/PKG-INFO` & `thipstercli-0.4.3/thipstercli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipstercli
-Version: 0.4.2
+Version: 0.4.3
 Summary: CLI interface build with typer, designed to use the thipster package
 Home-page: https://github.com/THipster/THipster-cli
 Download-URL: https://github.com/THipster/THipster-cli.git
 License: MIT
 Keywords: thipster,cli,generator,infrastructure as code,iac,terraform,typer
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thipstercli Version: 0.4.2 Summary: CLI interface
+Metadata-Version: 2.1 Name: thipstercli Version: 0.4.3 Summary: CLI interface
 build with typer, designed to use the thipster package Home-page: https://
 github.com/THipster/THipster-cli Download-URL: https://github.com/THipster/
 THipster-cli.git License: MIT Keywords: thipster,cli,generator,infrastructure
 as code,iac,terraform,typer Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console Classifier: Programming Language :: Python
 :: 3.11 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
```

### Comparing `thipstercli-0.4.2/thipstercli.egg-info/SOURCES.txt` & `thipstercli-0.4.3/thipstercli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

