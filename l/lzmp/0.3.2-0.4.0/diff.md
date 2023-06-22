# Comparing `tmp/lzmp-0.3.2.tar.gz` & `tmp/lzmp-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lzmp-0.3.2.tar", last modified: Thu Jan 12 12:23:25 2023, max compression
+gzip compressed data, was "lzmp-0.4.0.tar", last modified: Thu Jun 22 08:56:06 2023, max compression
```

## Comparing `lzmp-0.3.2.tar` & `lzmp-0.4.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxr-x   0 stephane  (1000) stephane  (1000)        0 2023-01-12 12:23:25.347620 lzmp-0.3.2/
--rw-rw-r--   0 stephane  (1000) stephane  (1000)     1261 2023-01-12 12:23:25.347620 lzmp-0.3.2/PKG-INFO
--rw-rw-r--   0 stephane  (1000) stephane  (1000)      680 2023-01-12 11:09:48.000000 lzmp-0.3.2/README.md
-drwxrwxr-x   0 stephane  (1000) stephane  (1000)        0 2023-01-12 12:23:25.347620 lzmp-0.3.2/lzmp.egg-info/
--rw-rw-r--   0 stephane  (1000) stephane  (1000)     1261 2023-01-12 12:23:25.000000 lzmp-0.3.2/lzmp.egg-info/PKG-INFO
--rw-rw-r--   0 stephane  (1000) stephane  (1000)      188 2023-01-12 12:23:25.000000 lzmp-0.3.2/lzmp.egg-info/SOURCES.txt
--rw-rw-r--   0 stephane  (1000) stephane  (1000)        1 2023-01-12 12:23:25.000000 lzmp-0.3.2/lzmp.egg-info/dependency_links.txt
--rw-rw-r--   0 stephane  (1000) stephane  (1000)       45 2023-01-12 12:23:25.000000 lzmp-0.3.2/lzmp.egg-info/entry_points.txt
--rw-rw-r--   0 stephane  (1000) stephane  (1000)       15 2023-01-12 12:23:25.000000 lzmp-0.3.2/lzmp.egg-info/top_level.txt
--rw-rw-r--   0 stephane  (1000) stephane  (1000)     7699 2023-01-12 12:22:32.000000 lzmp-0.3.2/lzmp.py
--rw-r--r--   0 stephane  (1000) stephane  (1000)     2221 2023-01-12 12:22:10.000000 lzmp-0.3.2/lzmp_test.py
--rw-rw-r--   0 stephane  (1000) stephane  (1000)      779 2023-01-12 12:22:37.000000 lzmp-0.3.2/pyproject.toml
--rw-rw-r--   0 stephane  (1000) stephane  (1000)       38 2023-01-12 12:23:25.347620 lzmp-0.3.2/setup.cfg
+drwxr-xr-x   0 sdemita   (1000) sdemita   (1000)        0 2023-06-22 08:56:06.759531 lzmp-0.4.0/
+-rw-r--r--   0 sdemita   (1000) sdemita   (1000)    35149 2022-12-29 07:38:16.000000 lzmp-0.4.0/COPYING
+-rw-r--r--   0 sdemita   (1000) sdemita   (1000)     1283 2023-06-22 08:56:06.759531 lzmp-0.4.0/PKG-INFO
+-rw-rw-r--   0 sdemita   (1000) sdemita   (1000)      680 2023-01-12 11:09:48.000000 lzmp-0.4.0/README.md
+drwxr-xr-x   0 sdemita   (1000) sdemita   (1000)        0 2023-06-22 08:56:06.758531 lzmp-0.4.0/lzmp.egg-info/
+-rw-rw-r--   0 sdemita   (1000) sdemita   (1000)     1283 2023-06-22 08:56:06.000000 lzmp-0.4.0/lzmp.egg-info/PKG-INFO
+-rw-rw-r--   0 sdemita   (1000) sdemita   (1000)      196 2023-06-22 08:56:06.000000 lzmp-0.4.0/lzmp.egg-info/SOURCES.txt
+-rw-rw-r--   0 sdemita   (1000) sdemita   (1000)        1 2023-06-22 08:56:06.000000 lzmp-0.4.0/lzmp.egg-info/dependency_links.txt
+-rw-rw-r--   0 sdemita   (1000) sdemita   (1000)       45 2023-06-22 08:56:06.000000 lzmp-0.4.0/lzmp.egg-info/entry_points.txt
+-rw-rw-r--   0 sdemita   (1000) sdemita   (1000)       15 2023-06-22 08:56:06.000000 lzmp-0.4.0/lzmp.egg-info/top_level.txt
+-rw-rw-r--   0 sdemita   (1000) sdemita   (1000)     8129 2023-06-22 08:52:49.000000 lzmp-0.4.0/lzmp.py
+-rw-r--r--   0 sdemita   (1000) sdemita   (1000)     2221 2023-01-12 12:22:10.000000 lzmp-0.4.0/lzmp_test.py
+-rw-rw-r--   0 sdemita   (1000) sdemita   (1000)      779 2023-06-22 08:52:56.000000 lzmp-0.4.0/pyproject.toml
+-rw-r--r--   0 sdemita   (1000) sdemita   (1000)       38 2023-06-22 08:56:06.759531 lzmp-0.4.0/setup.cfg
```

### Comparing `lzmp-0.3.2/PKG-INFO` & `lzmp-0.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: lzmp
-Version: 0.3.2
+Version: 0.4.0
 Summary: simple wrapper around the multiprocessing module allowing the lazy programmer to run batches of processes
 Author-email: Stéphane De Mita <demita@gmail.com>
 Project-URL: Homepage, https://gitlab.com/demita/lzmp
 Project-URL: Documentation, https://lzmp.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: COPYING
 
 lzmp
 ----
 
 ``lzmp`` is a simple wrapper around the Python multiprocessing module,
 allowing the lazy programmer to run batches of processes.
```

### Comparing `lzmp-0.3.2/README.md` & `lzmp-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `lzmp-0.3.2/lzmp.egg-info/PKG-INFO` & `lzmp-0.4.0/lzmp.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: lzmp
-Version: 0.3.2
+Version: 0.4.0
 Summary: simple wrapper around the multiprocessing module allowing the lazy programmer to run batches of processes
 Author-email: Stéphane De Mita <demita@gmail.com>
 Project-URL: Homepage, https://gitlab.com/demita/lzmp
 Project-URL: Documentation, https://lzmp.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: COPYING
 
 lzmp
 ----
 
 ``lzmp`` is a simple wrapper around the Python multiprocessing module,
 allowing the lazy programmer to run batches of processes.
```

### Comparing `lzmp-0.3.2/lzmp.py` & `lzmp-0.4.0/lzmp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-    Copyright 2022 Stéphane De Mita
+    Copyright 2022-2023 Stéphane De Mita
 
     lzmp is a simple wrapper around the multiprocessing module,
     allowing the lazy programmer to run batches of processes.
 
     lzmp contains the class Pool which lets the user specify one or more
     callable objects (such as functions) along with lists of arguments
     to process. lzmp collects the return value of each call and return
@@ -21,15 +21,15 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with lzmp.  If not, see <http://www.gnu.org/licenses/>.
 """
 
-__version__ = '0.3.2'
+__version__ = '0.4.0'
 
 import multiprocessing, random, queue
 
 class Pool:
     """
     Class to run tasks in parallel. Can be used to run different
     functions at once.
@@ -78,34 +78,40 @@
             p = self._waiting.pop(0)
             p.start()
             self._started.append(p)
             return True
         else:
             return False
 
-    def run(self, final=None, final_args=None, shuffle=False, echo=False):
+    def run(self, final=None, final_args=None, post=None, shuffle=False, echo=False):
         """
         Run the requested tasks. If *shuffle* is true, the order of
         tasks is randomized. Return a list of return values of the
         called function (order is not altered by shuffling). If *final*
         is not ``None``, call this function on this list and return the
         result. The callable passed as *final* will receive the combined
-        return values of the callable passed to :meth:`.Pool.add` as
+        return values of all jobs as
         first argument and, if specified, *final_args* as second
-        argument. If *echo* is set, the arguments (but not the callable)
+        argument. If *post* is set, this callable is called with the
+        return value of each job in a tuple with the job index,
+        on the main thread, after it finishes.
+        If *echo* is set, the arguments (but not the callable)
         are returned along with the corresponding results, wrapped in
         two-item tuples ``(args, res)``. If arguments are all one-item
         tuples, they are unwrapped automatically. It is not possible to
         set both *final* and *echo*.
 
         .. versionchanged:: 0.2
             *echo* argument
         
         .. versionchanged:: 0.3
             close automatically terminated processes upon completion
+
+        .. versionchanged:: 0.4
+            added *post* argument
         """
         if final and echo: raise ValueError("cannot set both final and echo arguments")
         if not len(self._tasks): return []
         self._waiting = [multiprocessing.Process(target=f, args=args) for (f, args) in self._tasks]
         if shuffle: random.shuffle(self._waiting)
         n = len(self._waiting)
         results = [None] * self._idx
@@ -117,14 +123,15 @@
                 break
         c = 0
         err = 0
         returncodes = set()
         while c < n:
             try:
                 res, idx = self._queue.get(timeout=1)
+                if post: post(res, idx)
                 c += 1
             except queue.Empty as e:
                 if not returncodes <= {0}:
                     for p in self._started:
                         if p.exitcode is None: p.terminate()
                     err = 1
                     break
@@ -147,24 +154,27 @@
         elif echo:
             args = [args for f, args in self._tasks]
             if set(map(len, args)) == {1}: return [(arg[0], res) for arg, res in zip(args, results)]
             else: return list(zip(args, results))
         else:
             return results
 
-def run(f, args, final=None, final_args=None, max_threads=None, shuffle=False, echo=False):
+def run(f, args, final=None, final_args=None, post=None, max_threads=None, shuffle=False, echo=False):
     """
     Convenience function to parallelise a single type of tasks.
 
     :param f: callable (typically a function) to execute
     :param args: iterable of arguments (each one must be a sequence).
         :func:`.wrap` can generate a proper iterable out of a
         single-item iterable.
     :param final: optional callable (function) to apply to the list of
         results. See :meth:`.Pool.run` for details.
+    :param post: optional callable (function) to apply to the return
+        value of each job immediately as it finishes (in the main
+        thread).
     :param final_args: arguments to pass to *final* if specified.
     :param max_threads: maximum number of process to run
         simultaneously.
     :param shuffle: randomly shuffle tasks. Will not affect the order
         or returned items.
     :param echo: return the arguments (but not the callable) along with
         the corresponding results, wrapped in two-item tuples
@@ -175,15 +185,15 @@
         return value of *final*, if specified.
 
     .. versionchanged:: 0.2
         *echo* argument
     """
     p = Pool(max_threads)
     p.add(f, args)
-    return p.run(final, final_args, shuffle, echo)
+    return p.run(final, final_args, post, shuffle, echo)
 
 def wrap(iterable, *extra):
     """
     Return a generator wherein each item yields by *iterable* is
     included as a single-item tuple. Constant *extra* arguments are
     appended to the tuple at each iteration round.
```

### Comparing `lzmp-0.3.2/lzmp_test.py` & `lzmp-0.4.0/lzmp_test.py`

 * *Files identical despite different names*

### Comparing `lzmp-0.3.2/pyproject.toml` & `lzmp-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lzmp"
-version = "0.3.2"
+version = "0.4.0"
 authors = [
   { name="Stéphane De Mita", email="demita@gmail.com" },
 ]
 description = "simple wrapper around the multiprocessing module allowing the lazy programmer to run batches of processes"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

