# Comparing `tmp/byu_pytest_utils-0.7.0.tar.gz` & `tmp/byu_pytest_utils-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byu_pytest_utils-0.7.0.tar", max compression
+gzip compressed data, was "byu_pytest_utils-0.7.1.tar", max compression
```

## Comparing `byu_pytest_utils-0.7.0.tar` & `byu_pytest_utils-0.7.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1195 2023-06-16 19:58:44.944894 byu_pytest_utils-0.7.0/byu_pytest_utils/__init__.py
--rw-r--r--   0        0        0      611 2023-06-16 19:58:44.958391 byu_pytest_utils-0.7.0/byu_pytest_utils/cpp_utils.py
--rw-r--r--   0        0        0     1168 2023-06-16 19:58:44.971739 byu_pytest_utils-0.7.0/byu_pytest_utils/decorators.py
--rw-r--r--   0        0        0    17831 2023-06-16 19:58:44.991847 byu_pytest_utils-0.7.0/byu_pytest_utils/dialog.py
--rw-r--r--   0        0        0     3088 2023-03-04 23:37:17.852701 byu_pytest_utils-0.7.0/byu_pytest_utils/edit_dist.py
--rw-r--r--   0        0        0     3595 2023-03-06 23:42:26.126776 byu_pytest_utils-0.7.0/byu_pytest_utils/pytest_plugin.py
--rw-r--r--   0        0        0     3474 2023-04-21 21:39:00.608118 byu_pytest_utils-0.7.0/byu_pytest_utils/utils.py
--rw-r--r--   0        0        0      562 2023-06-16 19:58:45.006438 byu_pytest_utils-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      601 1970-01-01 00:00:00.000000 byu_pytest_utils-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1195 2023-06-16 19:58:44.944894 byu_pytest_utils-0.7.1/byu_pytest_utils/__init__.py
+-rw-r--r--   0        0        0      611 2023-06-16 19:58:44.958391 byu_pytest_utils-0.7.1/byu_pytest_utils/cpp_utils.py
+-rw-r--r--   0        0        0     1168 2023-06-16 19:58:44.971739 byu_pytest_utils-0.7.1/byu_pytest_utils/decorators.py
+-rw-r--r--   0        0        0    17927 2023-06-22 20:04:44.736000 byu_pytest_utils-0.7.1/byu_pytest_utils/dialog.py
+-rw-r--r--   0        0        0     3088 2023-03-04 23:37:17.852701 byu_pytest_utils-0.7.1/byu_pytest_utils/edit_dist.py
+-rw-r--r--   0        0        0     3636 2023-06-22 20:04:44.765627 byu_pytest_utils-0.7.1/byu_pytest_utils/pytest_plugin.py
+-rw-r--r--   0        0        0     3474 2023-04-21 21:39:00.608118 byu_pytest_utils-0.7.1/byu_pytest_utils/utils.py
+-rw-r--r--   0        0        0      562 2023-06-22 20:04:44.774571 byu_pytest_utils-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0      601 1970-01-01 00:00:00.000000 byu_pytest_utils-0.7.1/PKG-INFO
```

### Comparing `byu_pytest_utils-0.7.0/byu_pytest_utils/__init__.py` & `byu_pytest_utils-0.7.1/byu_pytest_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `byu_pytest_utils-0.7.0/byu_pytest_utils/cpp_utils.py` & `byu_pytest_utils-0.7.1/byu_pytest_utils/cpp_utils.py`

 * *Files identical despite different names*

### Comparing `byu_pytest_utils-0.7.0/byu_pytest_utils/decorators.py` & `byu_pytest_utils-0.7.1/byu_pytest_utils/decorators.py`

 * *Files identical despite different names*

### Comparing `byu_pytest_utils-0.7.0/byu_pytest_utils/dialog.py` & `byu_pytest_utils-0.7.1/byu_pytest_utils/dialog.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,15 @@
         def new_func(group_name):
             group_stat = group_stats[group_name]
             if not group_stat['passed']:
                 assert group_stat['observed'] == group_stat['expected']
 
         new_func._group_stats = group_stats
         new_func.__name__ = func.__name__
+        new_func.__module__ = func.__module__
         return new_func
 
     return decorator
 
 
 def _ensure_absent(output_file):
     if output_file is not None:
@@ -321,15 +322,16 @@
             runpy.run_path(script_name, _globals, module)
 
             if output_file is not None:
                 if os.path.exists(output_file):
                     with open(output_file) as output:
                         group_stats = self._score_output(output.read())
                 else:
-                    group_stats = self._score_output(f"File not found: {output_file}. Did you write it?")
+                    group_stats = self._score_output(
+                        f"File not found: {output_file}. Did you write it?")
             else:
                 group_stats = self._score_output(self.observed_output)
 
         except Exception as ex:
             # get stack trace as string
             exception = f"Exception: {ex}\n{traceback.format_exc()}"
             group_stats = self._score_output(exception)
@@ -388,15 +390,16 @@
                     process.stdin, close_stdin_after_all_inputs_given, max_output_len)
 
             if output_file is not None:
                 if os.path.exists(output_file):
                     with open(output_file) as file:
                         group_stats = self._score_output(file.read())
                 else:
-                    group_stats = self._score_output(f'File not found: {output_file}. Did you write it?')
+                    group_stats = self._score_output(
+                        f'File not found: {output_file}. Did you write it?')
             else:
                 group_stats = self._score_output(self.observed_output)
 
         except Exception as ex:
             exception = f'Exception: {ex}\n{traceback.format_exc()}'
             group_stats = self._score_output(exception)
             process.terminate()
```

### Comparing `byu_pytest_utils-0.7.0/byu_pytest_utils/edit_dist.py` & `byu_pytest_utils-0.7.1/byu_pytest_utils/edit_dist.py`

 * *Files identical despite different names*

### Comparing `byu_pytest_utils-0.7.0/byu_pytest_utils/pytest_plugin.py` & `byu_pytest_utils-0.7.1/byu_pytest_utils/pytest_plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 def pytest_generate_tests(metafunc):
     if hasattr(metafunc.function, '_group_stats'):
         group_stats = metafunc.function._group_stats
 
         for group_name, stats in group_stats.items():
             stats['max_score'] *= getattr(metafunc.function, 'max_score', 0)
             stats['score'] *= getattr(metafunc.function, 'max_score', 0)
-            test_name = f'{metafunc.function.__name__}[{group_name}]'
+            test_name = f'{metafunc.function.__module__}.py::{metafunc.function.__name__}[{group_name}]'
             test_group_stats[test_name] = stats
 
         metafunc.parametrize('group_name', group_stats.keys())
     else:
         test_group_stats[metafunc.definition.name] = {
             'max_score': getattr(metafunc.function, 'max_score', 0)
         }
@@ -51,15 +51,16 @@
 
 @pytest.hookimpl(hookwrapper=True)
 def pytest_runtest_makereport(item):
     x = yield
     if item._obj not in metadata:
         metadata[item._obj] = {}
     metadata[item._obj]['max_score'] = getattr(item._obj, 'max_score', 0)
-    metadata[item._obj]['visibility'] = getattr(item._obj, 'visibility', 'visible')
+    metadata[item._obj]['visibility'] = getattr(
+        item._obj, 'visibility', 'visible')
     x._result.metadata_key = item._obj
 
 
 @pytest.hookimpl(hookwrapper=True)
 def pytest_pyfunc_call(pyfuncitem):
     # Deprecated function - remove with CheckIO stuff
     outcome = yield
@@ -77,15 +78,15 @@
     if 'passed' in terminalreporter.stats:
         all_tests = all_tests + terminalreporter.stats['passed']
     if 'failed' in terminalreporter.stats:
         all_tests = all_tests + terminalreporter.stats['failed']
 
     for s in all_tests:
         output = s.capstdout + '\n' + s.capstderr
-        group_stats = test_group_stats[s.head_line]
+        group_stats = test_group_stats[s.nodeid]
 
         max_score = group_stats['max_score']
         score = group_stats.get('score', max_score if s.passed else 0)
 
         output += s.longreprtext
 
         json_results["tests"].append(
```

### Comparing `byu_pytest_utils-0.7.0/byu_pytest_utils/utils.py` & `byu_pytest_utils-0.7.1/byu_pytest_utils/utils.py`

 * *Files identical despite different names*

### Comparing `byu_pytest_utils-0.7.0/pyproject.toml` & `byu_pytest_utils-0.7.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "byu_pytest_utils"
-version = "0.7.0"
+version = "0.7.1"
 description = "A few utilities for pytest to help with integration into gradescope"
 authors = ["Gordon Bean <gbean@cs.byu.edu>", "Daniel Zappala <daniel.zappala@gmail.com>"]
 license = "MIT"
 classifiers = [
     "Framework :: Pytest"
 ]
```

### Comparing `byu_pytest_utils-0.7.0/PKG-INFO` & `byu_pytest_utils-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: byu-pytest-utils
-Version: 0.7.0
+Version: 0.7.1
 Summary: A few utilities for pytest to help with integration into gradescope
 License: MIT
 Author: Gordon Bean
 Author-email: gbean@cs.byu.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Framework :: Pytest
 Classifier: License :: OSI Approved :: MIT License
```

