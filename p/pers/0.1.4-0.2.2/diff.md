# Comparing `tmp/pers-0.1.4.tar.gz` & `tmp/pers-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pers-0.1.4.tar", last modified: Mon May 29 18:46:08 2023, max compression
+gzip compressed data, was "pers-0.2.2.tar", last modified: Thu Jun 22 08:46:48 2023, max compression
```

## Comparing `pers-0.1.4.tar` & `pers-0.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ok        (1000) ok        (1000)        0 2023-05-29 18:46:08.967730 pers-0.1.4/
--rw-r--r--   0 ok        (1000) ok        (1000)    35149 2023-05-02 13:14:10.000000 pers-0.1.4/LICENSE
--rw-r--r--   0 ok        (1000) ok        (1000)     3456 2023-05-29 18:46:08.967730 pers-0.1.4/PKG-INFO
--rw-r--r--   0 ok        (1000) ok        (1000)     2944 2023-05-28 20:32:01.000000 pers-0.1.4/README.md
-drwxr-xr-x   0 ok        (1000) ok        (1000)        0 2023-05-29 18:46:08.965730 pers-0.1.4/pers/
--rw-r--r--   0 ok        (1000) ok        (1000)       19 2023-05-02 13:13:28.000000 pers-0.1.4/pers/__init__.py
--rw-r--r--   0 ok        (1000) ok        (1000)     5665 2023-05-29 18:45:21.000000 pers-0.1.4/pers/pers.py
--rw-r--r--   0 ok        (1000) ok        (1000)       21 2023-05-29 18:45:23.000000 pers-0.1.4/pers/version.py
-drwxr-xr-x   0 ok        (1000) ok        (1000)        0 2023-05-29 18:46:08.966730 pers-0.1.4/pers.egg-info/
--rw-r--r--   0 ok        (1000) ok        (1000)     3456 2023-05-29 18:46:08.000000 pers-0.1.4/pers.egg-info/PKG-INFO
--rw-r--r--   0 ok        (1000) ok        (1000)      232 2023-05-29 18:46:08.000000 pers-0.1.4/pers.egg-info/SOURCES.txt
--rw-r--r--   0 ok        (1000) ok        (1000)        1 2023-05-29 18:46:08.000000 pers-0.1.4/pers.egg-info/dependency_links.txt
--rw-r--r--   0 ok        (1000) ok        (1000)       12 2023-05-29 18:46:08.000000 pers-0.1.4/pers.egg-info/requires.txt
--rw-r--r--   0 ok        (1000) ok        (1000)        5 2023-05-29 18:46:08.000000 pers-0.1.4/pers.egg-info/top_level.txt
--rw-r--r--   0 ok        (1000) ok        (1000)       38 2023-05-29 18:46:08.967730 pers-0.1.4/setup.cfg
--rw-r--r--   0 ok        (1000) ok        (1000)     1133 2023-05-15 19:49:22.000000 pers-0.1.4/setup.py
-drwxr-xr-x   0 ok        (1000) ok        (1000)        0 2023-05-29 18:46:08.967730 pers-0.1.4/tests/
--rw-r--r--   0 ok        (1000) ok        (1000)     3254 2023-05-28 09:19:46.000000 pers-0.1.4/tests/tests.py
+drwxr-xr-x   0 ok        (1000) ok        (1000)        0 2023-06-22 08:46:48.837724 pers-0.2.2/
+-rw-r--r--   0 ok        (1000) ok        (1000)    35149 2023-05-02 13:14:10.000000 pers-0.2.2/LICENSE
+-rw-r--r--   0 ok        (1000) ok        (1000)     3456 2023-06-22 08:46:48.836724 pers-0.2.2/PKG-INFO
+-rw-r--r--   0 ok        (1000) ok        (1000)     2944 2023-05-28 20:32:01.000000 pers-0.2.2/README.md
+drwxr-xr-x   0 ok        (1000) ok        (1000)        0 2023-06-22 08:46:48.830724 pers-0.2.2/pers/
+-rw-r--r--   0 ok        (1000) ok        (1000)       19 2023-05-02 13:13:28.000000 pers-0.2.2/pers/__init__.py
+-rw-r--r--   0 ok        (1000) ok        (1000)     6548 2023-06-22 08:40:31.000000 pers-0.2.2/pers/pers.py
+-rw-r--r--   0 ok        (1000) ok        (1000)       21 2023-06-22 08:40:38.000000 pers-0.2.2/pers/version.py
+drwxr-xr-x   0 ok        (1000) ok        (1000)        0 2023-06-22 08:46:48.834724 pers-0.2.2/pers.egg-info/
+-rw-r--r--   0 ok        (1000) ok        (1000)     3456 2023-06-22 08:46:48.000000 pers-0.2.2/pers.egg-info/PKG-INFO
+-rw-r--r--   0 ok        (1000) ok        (1000)      232 2023-06-22 08:46:48.000000 pers-0.2.2/pers.egg-info/SOURCES.txt
+-rw-r--r--   0 ok        (1000) ok        (1000)        1 2023-06-22 08:46:48.000000 pers-0.2.2/pers.egg-info/dependency_links.txt
+-rw-r--r--   0 ok        (1000) ok        (1000)       12 2023-06-22 08:46:48.000000 pers-0.2.2/pers.egg-info/requires.txt
+-rw-r--r--   0 ok        (1000) ok        (1000)        5 2023-06-22 08:46:48.000000 pers-0.2.2/pers.egg-info/top_level.txt
+-rw-r--r--   0 ok        (1000) ok        (1000)       38 2023-06-22 08:46:48.837724 pers-0.2.2/setup.cfg
+-rw-r--r--   0 ok        (1000) ok        (1000)     1133 2023-05-15 19:49:22.000000 pers-0.2.2/setup.py
+drwxr-xr-x   0 ok        (1000) ok        (1000)        0 2023-06-22 08:46:48.835724 pers-0.2.2/tests/
+-rw-r--r--   0 ok        (1000) ok        (1000)     3759 2023-06-22 08:39:19.000000 pers-0.2.2/tests/tests.py
```

### Comparing `pers-0.1.4/LICENSE` & `pers-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pers-0.1.4/PKG-INFO` & `pers-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pers
-Version: 0.1.4
+Version: 0.2.2
 Summary: Persistent results is a Python class that ensures the results of tests will be available even if interruptions during the tests occur.
 Home-page: https://github.com/rsusik/pers
 Author: Robert Susik
 Author-email: robert.susik@gmail.com
 License: GPLv3
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: Developers
```

### Comparing `pers-0.1.4/README.md` & `pers-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pers-0.1.4/pers/pers.py` & `pers-0.2.2/pers/pers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 from typing import Any, Callable, List, Tuple
 from itertools import product
+import inspect
 from ncache import Cache
 
 class PersistentResults:
     def __init__(self, 
         filename:str, 
         tmpfilename:str=None, 
         interval:int=1, 
         load:bool=True,               # if False the results will be replaced
         exeption_on_duplicate:bool=False,
-        arg_prefix:str='_arg_',       # prefix for positional arguments (by default '_arg_': _arg_0, _arg_1, ..., _arg_n)
+        arg_prefix:str='_arg_',       # prefix for positional arguments that do not have corresponding names (by default '_arg_': _arg_0, _arg_1, ..., _arg_n). Case when *args is used in function
         result_key:str='result',      # key of the result if not flatten_result
         flatten_result:bool=True,     # flatten the results - return 2D table
         result_prefix:str='_result_', # prefix of result entries if flatten_result
+        skip_list:list[str]=None,     # list of arguments and results that shouldn't be added to output
     ):
         self.load           = load
         self.interval       = interval
         self.flatten_result = flatten_result
         self.arg_prefix     = arg_prefix
         self.result_prefix  = result_prefix
         self.result_key     = result_key
         self.exeption_on_duplicate = exeption_on_duplicate
+        if skip_list is not None:
+            self.skip_list = skip_list
+        else:
+            self.skip_list = []
 
         self.results = Cache(filename, tmpfilename=tmpfilename)
         self.counter = 0
         
         if self.load:
             self.results.load_cache()
     
@@ -122,22 +128,34 @@
             if self.flatten_result:
                 res = self._flatten_result(res)
                 # jeżeli w wyniku zostaly zwrocone argumenty funkcji to zignoruj te z identycznymi wartosciami
                 for k, v in kwargs.items():
                     if k in res:
                         if v != res[k]:
                             # TODO: poprawic komunikat
-                            raise Exception(f'Conflict!\nThere is argument with key {k}:{v} which is different than result with the same name {k}:{res[k]}\nYou can change the prefix or turn off flatten result')
+                            raise Exception(f'Conflict!\nThere is argument with key {k}:{v} which is different than result with the same name {k}:{res[k]}\nYou can change the prefix or turn off flattening result')
             else:
                 res = {self.result_key: res}
 
+            arg_names = [k for k, param in inspect.signature(fun).parameters.items() if param.kind not in [
+                inspect.Parameter.VAR_POSITIONAL, 
+                inspect.Parameter.VAR_KEYWORD,
+                inspect.Parameter.KEYWORD_ONLY
+            ]]
+
+            arg_names_count = len(arg_names)
+            if arg_names_count < len(args):
+                for idx in range(arg_names_count, len(args)):
+                    arg_names.append(f'{self.arg_prefix}{idx}')
+
+            args_dict = {arg_names[idx]: el for idx, el in enumerate(args)}
+            all_args = {**args_dict, **kwargs, **res}
+
             val = {
-                **res,
-                **{f'{self.arg_prefix}{idx}':x for idx, x in enumerate(args)},
-                **kwargs,
+                **{k:v for k, v in all_args.items() if k not in self.skip_list}
             }
             self.results.set_value(_hash, val)
             self.counter += 1
             if self.counter % self.interval == 0:
                 self.results.save_cache()
             return val
```

### Comparing `pers-0.1.4/pers.egg-info/PKG-INFO` & `pers-0.2.2/pers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pers
-Version: 0.1.4
+Version: 0.2.2
 Summary: Persistent results is a Python class that ensures the results of tests will be available even if interruptions during the tests occur.
 Home-page: https://github.com/rsusik/pers
 Author: Robert Susik
 Author-email: robert.susik@gmail.com
 License: GPLv3
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: Developers
```

### Comparing `pers-0.1.4/setup.py` & `pers-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `pers-0.1.4/tests/tests.py` & `pers-0.2.2/tests/tests.py`

 * *Files 14% similar despite different names*

```diff
@@ -95,12 +95,29 @@
         for x in range(10):
             for y in range(11):
                 results.append(fun, x, y, a=x, b=y)
         # It means there should be no records with 'DUPLICATE' value
         self.assertEqual(len([x for x in results.data if 'DUPLICATE' in x.values()]), 0)
 
 
+    def test_skip_list(self):
+        skip_list=['b', 'c', 'tmp']
+        results = PersistentResults(
+            'test_skip_list.pickle',
+            interval=1,
+            load=False,
+            skip_list=skip_list,
+            result_prefix=''
+        )
+        f = lambda a, b, *args, c=5, d=10: {'res': a+b+c+d, 'tmp': 123}
+        v = results.append(f, 2, 4, 6, d=5, c=3)
+        for k in skip_list:
+            self.assertNotIn(k, v.keys())
+        os.remove('test_skip_list.pickle')
+        
+
+
 if __name__ == '__main__':
     unittest.main()
```

