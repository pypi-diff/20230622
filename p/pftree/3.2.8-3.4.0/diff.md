# Comparing `tmp/pftree-3.2.8.tar.gz` & `tmp/pftree-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pftree-3.2.8.tar", last modified: Thu Oct  6 00:48:12 2022, max compression
+gzip compressed data, was "pftree-3.4.0.tar", last modified: Thu Jun 22 21:12:18 2023, max compression
```

## Comparing `pftree-3.2.8.tar` & `pftree-3.4.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2022-10-06 00:48:12.490965 pftree-3.2.8/
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     1069 2022-09-30 15:08:40.000000 pftree-3.2.8/LICENSE
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     9048 2022-10-06 00:48:12.490965 pftree-3.2.8/PKG-INFO
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     8783 2022-10-05 20:23:59.000000 pftree-3.2.8/README.rst
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2022-10-06 00:48:12.489965 pftree-3.2.8/pftree/
--rwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)      123 2022-10-05 20:59:00.000000 pftree-3.2.8/pftree/__init__.py
--rwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)    19194 2022-10-05 20:58:40.000000 pftree-3.2.8/pftree/__main__.py
--rwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)    58187 2022-10-06 00:44:38.000000 pftree-3.2.8/pftree/pftree.py
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2022-10-06 00:48:12.490965 pftree-3.2.8/pftree.egg-info/
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     9048 2022-10-06 00:48:11.000000 pftree-3.2.8/pftree.egg-info/PKG-INFO
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      293 2022-10-06 00:48:12.000000 pftree-3.2.8/pftree.egg-info/SOURCES.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)        1 2022-10-06 00:48:11.000000 pftree-3.2.8/pftree.egg-info/dependency_links.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       48 2022-10-06 00:48:12.000000 pftree-3.2.8/pftree.egg-info/entry_points.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)        1 2022-09-30 16:51:07.000000 pftree-3.2.8/pftree.egg-info/not-zip-safe
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       17 2022-10-06 00:48:12.000000 pftree-3.2.8/pftree.egg-info/requires.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)        7 2022-10-06 00:48:12.000000 pftree-3.2.8/pftree.egg-info/top_level.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       38 2022-10-06 00:48:12.490965 pftree-3.2.8/setup.cfg
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      901 2022-10-06 00:44:45.000000 pftree-3.2.8/setup.py
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2023-06-22 21:12:18.918562 pftree-3.4.0/
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     1069 2022-10-06 19:19:07.000000 pftree-3.4.0/LICENSE
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     9885 2023-06-22 21:12:18.918562 pftree-3.4.0/PKG-INFO
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     9639 2022-10-11 16:42:40.000000 pftree-3.4.0/README.rst
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2023-06-22 21:12:18.918562 pftree-3.4.0/pftree/
+-rwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)      123 2022-10-06 19:19:07.000000 pftree-3.4.0/pftree/__init__.py
+-rwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)    21572 2022-10-19 15:31:08.000000 pftree-3.4.0/pftree/__main__.py
+-rwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)    60593 2023-06-22 21:07:06.000000 pftree-3.4.0/pftree/pftree.py
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2023-06-22 21:12:18.918562 pftree-3.4.0/pftree.egg-info/
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     9885 2023-06-22 21:12:18.000000 pftree-3.4.0/pftree.egg-info/PKG-INFO
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      293 2023-06-22 21:12:18.000000 pftree-3.4.0/pftree.egg-info/SOURCES.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)        1 2023-06-22 21:12:18.000000 pftree-3.4.0/pftree.egg-info/dependency_links.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       48 2023-06-22 21:12:18.000000 pftree-3.4.0/pftree.egg-info/entry_points.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)        1 2022-10-11 15:48:34.000000 pftree-3.4.0/pftree.egg-info/not-zip-safe
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       17 2023-06-22 21:12:18.000000 pftree-3.4.0/pftree.egg-info/requires.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)        7 2023-06-22 21:12:18.000000 pftree-3.4.0/pftree.egg-info/top_level.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       38 2023-06-22 21:12:18.918562 pftree-3.4.0/setup.cfg
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      901 2023-06-22 21:09:51.000000 pftree-3.4.0/setup.py
```

### Comparing `pftree-3.2.8/LICENSE` & `pftree-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pftree-3.2.8/PKG-INFO` & `pftree-3.4.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: pftree
-Version: 3.2.8
-Summary: Utility to create dict representations of file system trees.
-Home-page: https://github.com/FNNDSC/pftree
-Author: FNNDSC
-Author-email: dev@babymri.org
-License: MIT
-Platform: UNKNOWN
-License-File: LICENSE
-
 pftree
 ======
 
 .. image:: https://badge.fury.io/py/pftree.svg
     :target: https://badge.fury.io/py/pftree
 
 .. image:: https://travis-ci.org/FNNDSC/pftree.svg?branch=master
@@ -162,17 +151,33 @@
         [--verbosity <level>]
         Set the app verbosity level. This ranges from 0...<N> where internal
         log messages with a level=<M> will only display if M <= N. In this
         manner increasing the level here can be used to show more and more
         debugging info, assuming that debug messages in the code have been
         tagged with a level.
 
-        [--stats | --statsReverse]
-        If specified, return some stats to caller -- summary list ordered
-        by directory size (--statsReverse does a reverse sort).
+        [--stats | --statsReverse | --du | --duf]
+        If specified, return some stats to caller. The amount of information
+        returned depends on the --verbosity.
+
+        For --stats (and --statsReverse):
+
+            * --verbosity 0: return only a final summary of group statistics
+            * --verbosity 1: in addition, return a sorted (by size) list of
+                             subdirectories in the search tree
+            * --verbosity >1: same as above, but provide probing status updates.
+                              NOTE: this incurs a significant performance penalty!
+
+        For --du | --duf
+
+            similar to '--stats' but return directory lists in a fashion similar
+            to the GNU 'du' tool. Both of these set default verbosity values so that
+
+            * --du : only provide a summary
+            * --duf: provide the (full) sorted list as well
 
         [--3D]
         A "toy" flag that simply shows the final stats report with an ASCII
         3D effect.
 
         [--jsonStats]
         If specified, do a JSON dump of the stats.
@@ -216,14 +221,20 @@
                         --stats --verbosity 0
 
 Increasing the ``verbosity`` will produce increasing output on the console. Passing
 a ``--json`` will return a highly detailed JSON payload with considerable information.
 Passing a ``--jsonStats`` will only return a summary of the final stats on the
 filesystem probed. Note that the ``--verbosity`` flag is ignored if ``--json`` or ``--jsonStats`` are also present.
 
+.. code:: bash
+
+    pftree          --duf --inputDir /var/www/html
+
+Simpler CLI for a less "progress displaying" but faster response.
+
 test
 ~~~~
 
 Run a test down a target tree:
 
 .. code:: bash
 
@@ -231,9 +242,8 @@
                         --outputDir /tmp/test                                   \
                         --verbosity 1 --relativeDir                             \
                         --outputLeafDir 'preview-%%s'                           \
                         --test 0
 
 which will "copy" the input tree to the output, and save a file-ls.txt in each directory where necessary. Note the ``-r`` for 'relative' directory specification and the ``--outputLeafDir`` spec.
 
-_-30-_
-
+_-30-_
```

### Comparing `pftree-3.2.8/README.rst` & `pftree-3.4.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: pftree
+Version: 3.4.0
+Summary: Utility to create dict representations of file system trees.
+Home-page: https://github.com/FNNDSC/pftree
+Author: FNNDSC
+Author-email: dev@babymri.org
+License: MIT
+License-File: LICENSE
+
 pftree
 ======
 
 .. image:: https://badge.fury.io/py/pftree.svg
     :target: https://badge.fury.io/py/pftree
 
 .. image:: https://travis-ci.org/FNNDSC/pftree.svg?branch=master
@@ -151,17 +161,33 @@
         [--verbosity <level>]
         Set the app verbosity level. This ranges from 0...<N> where internal
         log messages with a level=<M> will only display if M <= N. In this
         manner increasing the level here can be used to show more and more
         debugging info, assuming that debug messages in the code have been
         tagged with a level.
 
-        [--stats | --statsReverse]
-        If specified, return some stats to caller -- summary list ordered
-        by directory size (--statsReverse does a reverse sort).
+        [--stats | --statsReverse | --du | --duf]
+        If specified, return some stats to caller. The amount of information
+        returned depends on the --verbosity.
+
+        For --stats (and --statsReverse):
+
+            * --verbosity 0: return only a final summary of group statistics
+            * --verbosity 1: in addition, return a sorted (by size) list of
+                             subdirectories in the search tree
+            * --verbosity >1: same as above, but provide probing status updates.
+                              NOTE: this incurs a significant performance penalty!
+
+        For --du | --duf
+
+            similar to '--stats' but return directory lists in a fashion similar
+            to the GNU 'du' tool. Both of these set default verbosity values so that
+
+            * --du : only provide a summary
+            * --duf: provide the (full) sorted list as well
 
         [--3D]
         A "toy" flag that simply shows the final stats report with an ASCII
         3D effect.
 
         [--jsonStats]
         If specified, do a JSON dump of the stats.
@@ -205,14 +231,20 @@
                         --stats --verbosity 0
 
 Increasing the ``verbosity`` will produce increasing output on the console. Passing
 a ``--json`` will return a highly detailed JSON payload with considerable information.
 Passing a ``--jsonStats`` will only return a summary of the final stats on the
 filesystem probed. Note that the ``--verbosity`` flag is ignored if ``--json`` or ``--jsonStats`` are also present.
 
+.. code:: bash
+
+    pftree          --duf --inputDir /var/www/html
+
+Simpler CLI for a less "progress displaying" but faster response.
+
 test
 ~~~~
 
 Run a test down a target tree:
 
 .. code:: bash
 
@@ -220,8 +252,8 @@
                         --outputDir /tmp/test                                   \
                         --verbosity 1 --relativeDir                             \
                         --outputLeafDir 'preview-%%s'                           \
                         --test 0
 
 which will "copy" the input tree to the output, and save a file-ls.txt in each directory where necessary. Note the ``-r`` for 'relative' directory specification and the ``--outputLeafDir`` spec.
 
-_-30-_
+_-30-_
```

### Comparing `pftree-3.2.8/pftree/__main__.py` & `pftree-3.4.0/pftree/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -63,14 +63,18 @@
 
 ''' + Colors.NO_COLOUR
 
 package_IOcore  = """
         --inputDir <inputDir>                                                   \\
         [--outputDir <outputDir>]                                               \\"""
 
+package_DSIO  = """
+        <inputDir>                                                              \\
+        <outputDir>                                                             \\"""
+
 package_CLIcore = """
         [--fileFilter <someFilter1,someFilter2,...>]                            \\
         [--filteFilterLogic AND|OR]                                             \\
         [--dirFilter <someFilter1,someFilter2,...>]                             \\
         [--dirFilterLogic AND|OR]                                               \\
         [--maxdepth <dirDepth>]                                                 \\
         [--inputFile <inputFile>]                                               \\
@@ -84,24 +88,40 @@
         [--verbosity <verbosity>]                                               \\
         [--version]                                                             \\
         [--threads <numThreads>]                                                \\
         [--json]
 """
 
 package_CLIself     = '''
-        [--stats | --statsReverse]                                              \\
+        [--stats | --statsReverse | --du | --duf]                               \\
         [--3D]                                                                  \\
         [--jsonStats]                                                           \\
         [--syslog]                                                              \\
         [--test <analysisDelayLength[:<type>]>]                                 \\'''
 
 package_argSynopsisSelf = """
-        [--stats | --statsReverse]
-        If specified, return some stats to caller -- summary list ordered
-        by directory size (--statsReverse does a reverse sort).
+        [--stats | --statsReverse | --du | --duf]
+        If specified, return some stats to caller. The amount of information
+        returned depends on the --verbosity.
+
+        For --stats (and --statsReverse):
+
+            * --verbosity 0: return only a final summary of group statistics
+            * --verbosity 1: in addition, return a sorted (by size) list of
+                             subdirectories in the search tree
+            * --verbosity >1: same as above, but provide probing status updates.
+                              NOTE: this incurs a significant performance penalty!
+
+        For --du | --duf
+
+            similar to '--stats' but return directory lists in a fashion similar
+            to the GNU 'du' tool. Both of these set default verbosity values so that
+
+            * --du : only provide a summary
+            * --duf: provide the (full) sorted list as well
 
         [--3D]
         A "toy" flag that simply shows the final stats report with an ASCII
         3D effect.
 
         [--jsonStats]
         If specified, do a JSON dump of the stats.
@@ -139,14 +159,29 @@
 
         [--outputDir <outputDir>]
         The directory to contain a tree structure identical to the input
         tree structure, and which contains all output files from the
         per-input-dir processing.
 """
 
+package_argSynopsisDS = """
+
+        <inputDir>
+        A _required_ positional argument for ChRIS DS plugins denoting the
+        input directory to examine. The downstream nested structure of this
+        directory is examined and recreated in the <outputDir>.
+
+        <outputDir>
+        A _required_ positional argument for ChRIS DS plugins denoting the
+        output directory to store data. The structure of this tree mimics
+        that of the <inputDir>, with correspondant directory nodes containing
+        the results of corresponding <inputDir> processing.
+"""
+
+
 package_argSynopsisCore = """
 
         [--maxdepth <dirDepth>]
         The maximum depth to descend relative to the <inputDir>. Note, that
         this counts from zero! Default of '-1' implies transverse the entire
         directory tree.
 
@@ -292,15 +327,17 @@
     * Run on a target tree and output some detail and stats
 
         pftree          --inputDir /var/www/html                                \\
                         --printElapsedTime                                      \\
                         --stats --verbosity 0 --json
 
     which will output only at script conclusion and will log a JSON formatted
-    string.
+    string. Similarly
+
+        pftree          --du --inputDir /var/www/html
 
     * Run a test down a target tree:
 
         pftree          --inputDir /etc                                         \\
                         --outputDir /tmp/test                                   \\
                         --verbosity 1 --relativeDir                             \\
                         --outputLeafDir 'preview-%%s'                           \\
@@ -324,19 +361,19 @@
                              formatter_class    = RawTextHelpFormatter,
                              add_help           = False)
 parserSelf  = ArgumentParser(description        = 'Self specific',
                              formatter_class    = RawTextHelpFormatter,
                              add_help           = False)
 
 
-parserIO.add_argument("--inputDir",
+parserIO.add_argument("--inputDir", '--inputdir',
                     help    = "input dir",
                     dest    = 'inputDir',
                     default = '')
-parserIO.add_argument("--outputDir",
+parserIO.add_argument("--outputDir", '--outputdir',
                     help    = "output image directory",
                     dest    = 'outputDir',
                     default = '.')
 
 parserCore.add_argument("--maxDepth",
                     help    = "max depth, counting from zero, to descend",
                     dest    = 'maxDepth',
@@ -409,65 +446,85 @@
                     help    = "a list of comma separated string filters to apply across the input dir space",
                     dest    = 'dirFilter',
                     default = '')
 parserCore.add_argument("--dirFilterLogic",
                     help    = "the logic to apply across the dir filter",
                     dest    = 'dirFilterLogic',
                     default = 'OR')
+parserCore.add_argument("--syslog",
+                    help    = "show outputs in syslog style",
+                    dest    = 'syslog',
+                    action  = 'store_true',
+                    default = False)
 
 parserSelf.add_argument("--stats",
                     help    = "show some quick stats",
                     dest    = 'stats',
                     action  = 'store_true',
                     default = False)
 parserSelf.add_argument("--statsReverse",
                     help    = "show some quick stats (reverse order)",
                     dest    = 'statsReverse',
                     action  = 'store_true',
                     default = False)
+parserSelf.add_argument("--du",
+                    help    = "show disk usage in the GNU du style",
+                    dest    = 'du',
+                    action  = 'store_true',
+                    default = False)
+parserSelf.add_argument("--duf",
+                    help    = "show disk usage in the GNU du style (no console updating)",
+                    dest    = 'duf',
+                    action  = 'store_true',
+                    default = False)
 parserSelf.add_argument("--3D",
                     help    = "show table in ASCII 3D",
                     dest    = 'table3D',
                     action  = 'store_true',
                     default = False)
-parserSelf.add_argument("--syslog",
-                    help    = "show outputs in syslog style",
-                    dest    = 'syslog',
-                    action  = 'store_true',
-                    default = False)
 parserSelf.add_argument("--jsonStats",
                     help    = "JSON dump stats",
                     dest    = 'jsonStats',
                     action  = 'store_true',
                     default = False)
 parserSelf.add_argument("--test",
                     help    = "perform a test run of the read/analyze/write loop -- arg indicates sleep length in analyze",
                     dest    = 'test',
                     default = '')
 
-def main(argv = None):
-
-    parser  = ArgumentParser(description        = str_desc,
+# Stand alone parser
+parserSA     = ArgumentParser(description       = str_desc,
                              formatter_class    = RawTextHelpFormatter,
                              parents            = [parserIO, parserCore, parserSelf])
-    args = parser.parse_args()
+
+# DS conformant parser
+parserDS     = ArgumentParser(description       = str_desc,
+                             formatter_class    = RawTextHelpFormatter,
+                             parents            = [parserCore, parserSelf])
+
+def main(argv = None):
+
+    args = parserSA.parse_args()
 
     if args.man or args.synopsis:
         print(str_desc)
         if args.man:
             str_help     = synopsis(False)
         else:
             str_help     = synopsis(True)
         print(str_help)
         return 1
 
     if args.b_version:
         print("Name:    %s\nVersion: %s" % (__pkg.name, __version__))
         return 1
 
+    args.str_version    = __version__
+    args.str_desc       = synopsis(True)
+
     try:
         pf_tree             = pftree.pftree(vars(args))
     except:
         pf_tree             = pftree(vars(args))
 
     # And now run it!
     d_pftree = pf_tree.run(timerStart = True)
```

### Comparing `pftree-3.2.8/pftree/pftree.py` & `pftree-3.4.0/pftree/pftree.py`

 * *Files 3% similar despite different names*

```diff
@@ -175,15 +175,14 @@
                 'error'         : 'no boolean "status" was found. This is a *required* return key',
                 'exitCode'      : 4}
             }
 
         #
         # Object desc block
         #
-        self.str_desc                   = ''
         self.__name__                   = __name__
         self.str_version                = __version__
 
         # Object containing this class
         self.within                     = None
 
         # Thread number
@@ -213,14 +212,15 @@
         self.testType                   = 0
 
         self.dp                         = None
         self.log                        = None
         self.tic_start                  = 0.0
         self.pp                         = pprint.PrettyPrinter(indent=4)
         self.verbosityLevel             = 1
+        self.debugLevel                 = 0
 
     def checkFor_tests(self) -> bool:
         """Checks the internal self.str_sleepLength value
         that is used to trigger tests. The CLI `--test` flag
         might be set by a descendent or sibling module and
         hence cause issues if interpreted by this class.
 
@@ -246,46 +246,81 @@
         return b_status
 
     def __init__(self, *args, **kwargs):
 
         # pudb.set_trace()
         self.declare_selfvars()
         self.args                       = args[0]
+        self.str_desc                   = self.args['str_desc']
         if len(self.args):
             kwargs  = {**self.args, **kwargs}
 
+        for pkey in ['du', 'duf']:
+            if pkey not in self.args.keys(): self.args[pkey] = False
+        if self.args['du']:
+            self.verbosityLevel = 2
+            self.debugLevel     = 2
+        if self.args['duf']:
+            self.verbosityLevel = 0
+            self.debugLevel     = 0
+
         for key, value in kwargs.items():
-            if key == 'inputDir':       self.str_inputDir       = value
-            if key == 'maxDepth':       self.maxdepth           = int(value)
-            if key == 'inputFile':      self.str_inputFile      = value
-            if key == 'outputDir':      self.str_outputDir      = value
-            if key == 'verbosity':      self.verbosityLevel     = int(value)
-            if key == 'threads':        self.numThreads         = int(value)
-            if key == 'relativeDir':    self.b_relativeDir      = bool(value)
-            if key == 'stats':          self.b_stats            = bool(value)
-            if key == 'statsReverse':   self.b_statsReverse     = bool(value)
-            if key == 'jsonStats':      self.b_jsonStats        = bool(value)
-            if key == 'json':           self.b_json             = bool(value)
-            if key == 'followLinks':    self.b_followLinks      = bool(value)
-            if key == 'test':           self.str_sleepLength    = value
-            if key == 'outputLeafDir':  self.str_outputLeafDir  = value
+            if key.lower() == 'inputdir':   self.str_inputDir       = value
+            if key == 'maxDepth':           self.maxdepth           = int(value)
+            if key == 'inputFile':          self.str_inputFile      = value
+            if key.lower() == 'outputdir':  self.str_outputDir      = value
+            if key == 'verbosity':          self.verbosityLevel     = int(value)
+            if key == 'threads':            self.numThreads         = int(value)
+            if key == 'relativeDir':        self.b_relativeDir      = bool(value)
+            if key == 'stats':              self.b_stats            = bool(value)
+            if key == 'statsReverse':       self.b_statsReverse     = bool(value)
+            if key == 'jsonStats':          self.b_jsonStats        = bool(value)
+            if key == 'json':               self.b_json             = bool(value)
+            if key == 'followLinks':        self.b_followLinks      = bool(value)
+            if key == 'test':               self.str_sleepLength    = value
+            if key == 'outputLeafDir':      self.str_outputLeafDir  = value
 
         self.checkFor_tests()
 
         # Set logging
         self.dp                        = pfmisc.debug(
                                             verbosity   = self.verbosityLevel,
                                             within      = self.__name__,
                                             syslog      = self.args['syslog']
                                             )
         self.log                       = pfmisc.Message()
         self.log.syslog(True)
 
         if not len(self.str_inputDir): self.str_inputDir = '.'
 
+    def toConsole(self) -> bool:
+        """A simple check on CLI flag patterning to resolve whether or not
+        to actually generate console output. This output needs to return
+        false if any json related flag has been indicated since any non-
+        json "noise" could corrupt any app that wants to only consume
+        json data from this module.
+
+        Essentially, the method will return True, unless either a
+        --json or --jsonStats has been specified
+
+        Returns:
+            bool: True if OK to print to console
+        """
+
+        b_toConsole :   bool    = True
+
+        if self.verbosityLevel:
+            for noConsole in ['jsonStats', 'json']:
+                if noConsole in self.args.keys():
+                    b_toConsole     = b_toConsole and not self.args[noConsole]
+        else:
+            b_toConsole = False
+
+        return b_toConsole
+
     def simpleProgress_show(self, index, total, *args):
         str_pretext = ""
         if len(args):
             str_pretext = args[0] + ":"
         f_percent   = index/total*100
         str_num     = "[%3d/%3d: %6.2f%%] " % (index, total, f_percent)
         str_bar     = "*" * int(f_percent)
@@ -341,15 +376,15 @@
                 inner : inner function
             """
             spinner = '\\|/-'
             pos     = 0
             def inner(b_cursorToNextLine):
                 nonlocal pos, spinner
                 if pos>=len(spinner): pos = 0
-                if not self.args['json'] and not self.args['jsonStats']:
+                if self.toConsole():
                     self.dp.qprint('Probing filesystem... {}'.format(spinner[pos]), end = '')
                     if not b_cursorToNextLine:
                         self.dp.qprint('\r', end = '', syslog = self.args['syslog'])
                     else:
                         self.dp.qprint('\n', end = '', syslog = self.args['syslog'])
                 pos += 1
                 return inner
@@ -377,15 +412,15 @@
                     str_path    = str(pathlib.PurePath(*l_copy))
             return str_path
 
         def elements_flash(l_el, debugLevel):
             """
             Flash elements in the passed list at the debugLevel
             """
-            if not self.args['json'] and not self.args['jsonStats']:
+            if self.toConsole():
                 for el in l_el:
                     self.dp.qprint('%s (%d)\033[K\r' % \
                             (path_shorten(el, - len(str(len(l_el))) - 4), len(l_el)),
                             level   = debugLevel,
                             end     = '',
                             syslog  = self.args['syslog'])
 
@@ -398,40 +433,45 @@
         l_dirsHere          = []
         l_filesHere         = []
         b_cursorToNextLine  = False
 
         for k, v in kwargs.items():
             if k == 'root':  str_topDir  = v
 
-        if int(self.args['verbosity']) >= 2:
+        if int(self.verbosityLevel) >= 2:
             b_cursorToNextLine = True
         spinner             = nextSpinner(b_cursorToNextLine)
+        index:int       = 0
         for root, dirs, files in pftree.walklevel(str_topDir,
                                                   self.maxdepth,
                                                   followlinks = self.b_followLinks):
             b_status = True
-            spinner(b_cursorToNextLine)
+            if self.verbosityLevel >= 2: spinner(b_cursorToNextLine)
             str_path = root.split(os.sep)
-            if dirs:
-                l_dirsHere = [root + '/' + x for x in dirs]
-                l_dirs.append(l_dirsHere)
-                elements_flash(l_dirsHere, 2)
-            if files:
+            l_dirs.append(root)
+            if self.verbosityLevel >= 2: elements_flash(l_dirs, 2)
+            if index:
                 l_filesHere = [root + '/' + y for y in files]
-                if len(self.str_inputFile):
-                    l_hit = [s for s in l_filesHere if self.str_inputFile in s]
-                    if l_hit:
-                        l_filesHere = l_hit
-                    else:
-                        l_filesHere = []
-                if l_filesHere:
-                    l_files.append(l_filesHere)
-                    elements_flash(l_filesHere, 3)
-            self.dp.qprint("\033[A" * 1, end = '', syslog = self.args['syslog'], level =2)
-        if not self.args['json'] and not self.args['jsonStats']:
+            else:
+                l_filesHere = [root + '/' + y for y in dirs]
+            if len(self.str_inputFile):
+                l_hit = [s for s in l_filesHere if self.str_inputFile in s]
+                if l_hit:
+                    l_filesHere = l_hit
+                else:
+                    l_filesHere = []
+            l_files.append(l_filesHere)
+            if self.verbosityLevel >= 3: elements_flash(l_filesHere, 3)
+            if self.toConsole() and self.verbosityLevel >=2:
+                self.dp.qprint("\033[A" * 1,
+                                end     = '',
+                                syslog  = self.args['syslog'],
+                                level   = 2 )
+            index += 1
+        if self.toConsole() and self.verbosityLevel >= 2:
             self.dp.qprint('Probing complete!              ', level = 1)
         return {
             'status':   b_status,
             'l_dir':    l_dirs,
             'l_files':  l_files
         }
 
@@ -451,23 +491,24 @@
 
         for k, v in kwargs.items():
             if k == 'l_files':           l_files                 = v
             if k == 'constructCallback': fn_constructCallback    = v
             if k == 'd_probe':           d_probe                 = v
 
         if d_probe: l_files     = d_probe['l_files']
-        index   = 1
+        index   = 0
         total   = len(l_files)
-        if int(self.args['verbosity']) and not self.args['json'] and not self.args['jsonStats']:
+        if int(self.verbosityLevel) and self.toConsole():
             l_range     = tqdm(l_files, desc = ' Constructing tree')
         else:
             l_range     = l_files
         for l_series in l_range:
-            str_path    = os.path.dirname(l_series[0])
-            l_series    = [ os.path.basename(i) for i in l_series]
+            if len(l_series):
+                str_path    = os.path.dirname(l_series[0])
+                l_series    = [ os.path.basename(i) for i in l_series]
             # self.simpleProgress_show(index, total)
             self.d_inputTree[str_path]  = l_series
             if fn_constructCallback:
                 kwargs['path']          = str_path
                 d_constructCallback     = fn_constructCallback(l_series, **kwargs)
                 self.d_inputTreeCallback[str_path]  = d_constructCallback
             self.d_outputTree[str_path] = ""
@@ -537,16 +578,19 @@
                     al_file = [x for x in al_file if y in x]
 
         if len(self.args['dirFilter']):
             l_dirHits   = [str_path                                         \
                             for y in self.args['dirFilter'].split(',')      \
                                 if y in str_path]
             if self.args['dirFilterLogic'].upper()  == 'AND':
-                for y in self.args['dirFilter'].split(','):
-                    l_dirHits = [x for x in l_dirHits if y in x]
+                if len(l_dirHits) == len(self.args['dirFilter'].split(',')):
+                    for y in self.args['dirFilter'].split(','):
+                        l_dirHits = [x for x in l_dirHits if y in x]
+                else:
+                    l_dirHits = []
             if len(l_dirHits):
                 # Remove any duplicates in the l_dirHits: duplicates can occur
                 # if the tokens in the filter expression map more than once
                 # into the leaf node in the <str_path>, as a path that is
                 #
                 #               /some/dir/in/the/space/1234567
                 #
@@ -589,15 +633,15 @@
         self.d_inputTreeCallback = {k :self.d_inputTreeCallback[k]
                                         for k in self.d_inputTree}
 
         return d_filterFileHitList
 
     @staticmethod
     def sizeof_fmt(num, suffix='B'):
-        for unit in ['','Ki','Mi','Gi','Ti','Pi','Ei','Zi']:
+        for unit in ['','k','M','G','T','P','E','Z']:
             if abs(num) < 1024.0:
                 return "%3.1f%s%s" % (num, unit, suffix)
             num /= 1024.0
         return "%.1f%s%s" % (num, 'Yi', suffix)
 
     @staticmethod
     def dirsize_get(l_filesWithoutPath, **kwargs):
@@ -760,22 +804,15 @@
             from specific "leaf" nodes in the <inputDir>.
             """
             nonlocal    filesRead
             nonlocal    index
             nonlocal    d_tree
             nonlocal    fn_inputReadCallback
 
-            # self.simpleProgress_show(index, total, '%s:%s' %
-            #     ('%25s' %threading.currentThread().getName(),
-            #      '%25s' % fn_inputReadCallback.__name__)
-            # )
-
-            d_read = fn_inputReadCallback(
-                ('%s/%s' % (self.str_inputDir, path), data), **kwargs
-            )
+            d_read = fn_inputReadCallback((path, data), **kwargs)
 
             if 'status' in d_read.keys():
                 d_tree[path]    = d_read
                 if 'filesRead' in d_read.keys():
                     filesRead   += d_read['filesRead']
             else:
                 self.dp.qprint(
@@ -787,22 +824,15 @@
             return d_read
 
         def analysis_do(path, data, index, **kwargs):
             nonlocal    filesAnalyzed
             nonlocal    d_tree
             nonlocal    fn_analysisCallback
 
-            # self.simpleProgress_show(index, total, '%s:%s' %
-            #     ('%25s' % threading.currentThread().getName(),
-            #      '%25s' % fn_analysisCallback.__name__)
-            # )
-
-            d_analysis          = fn_analysisCallback(
-                ('%s/%s' % (self.str_inputDir, path), d_tree[path]), **kwargs
-            )
+            d_analysis          = fn_analysisCallback((path, d_tree[path]), **kwargs)
 
             if 'status' in d_analysis.keys():
                 if d_analysis['status']:
                     # Analysis was successful
                     if len(str_applyKey):
                         d_tree[path]    = d_analysis[str_applyKey]
                     else:
@@ -936,15 +966,21 @@
             nonlocal dret_outputSet
             nonlocal str_desc
 
             b_analyzeStatusHist:    bool = False
             b_inputStatusHist:      bool = False
             b_outputStatusHist:     bool = False
 
-            for path, data in tqdm(self.d_inputTree.items(), desc = str_desc):
+            if int(self.verbosityLevel) and self.toConsole():
+                iterator        = tqdm( self.d_inputTree.items(),
+                                    desc = str_desc)
+            else:
+                iterator        = self.d_inputTree.items()
+
+            for path, data in iterator:
                 dret_inputSet   = {}
                 dret_analyze    = {}
                 dret_outputSet  = {}
                 # Read (is sometimes skipped) / Analyze / Write (also sometimes skipped)
                 if fn_inputReadCallback:
                     dret_inputSet       = inputSet_read(path, data)
                     try:
@@ -1025,29 +1061,33 @@
                                         0)
                 nextRunCount    =  thread_batch(
                                         l_threadAnalysis,
                                         1,
                                         threadRem,
                                         alreadyRunCount)
 
+            if int(self.verbosityLevel) and self.toConsole():
+                iterator        = tqdm( self.d_inputTree.items(),
+                                    desc = str_desc)
+            else:
+                iterator        = self.d_inputTree.items()
+
             # Read
             if fn_inputReadCallback:
                 index = 1
-                for path, data in tqdm( self.d_inputTree.items(),
-                                        desc = ' Reading      tree'):
+                for path, data in iterator:
                     dret_inputSet   = inputSet_read(path, data)
                     # filesRead       += dret_inputSet['filesRead']
                     index += 1
 
             # Analyze
             if fn_analysisCallback:
                 index               = 1
                 l_threadAnalysis    = []
-                for path, data in tqdm( self.d_inputTree.items(),
-                                        desc = ' Analyzing    tree'):
+                for path, data in iterator:
                     l_threadAnalysis.append(thread_createOnFunction(
                                                     path, data,
                                                     'analysisThread',
                                                     # t_analyze
                                                     analysis_do
                                             )
                     )
@@ -1055,16 +1095,15 @@
 
                 # And now batch them in groups
                 threadsInBatches_run(l_threadAnalysis)
                 tree_removeDeadBranches()
             # Write
             if fn_outputWriteCallback:
                 index   = 1
-                for path, data in tqdm( self.d_inputTree.items(),
-                                        ' Saving  new  tree'):
+                for path, data in iterator:
                     dret_outputSet  = outputSet_write(path, d_tree[path])
                     # filesSaved      += dret_outputSet['filesSaved']
                     index += 1
 
         for k, v in kwargs.items():
             if k == 'inputReadCallback':        fn_inputReadCallback        = v
             if k == 'analysisCallback':         fn_analysisCallback         = v
@@ -1143,40 +1182,54 @@
         of files).
         """
         totalElements   = 0
         totalKeys       = 0
         totalSize       = 0
         l_stats         = []
         d_report        = {}
+        str_report      = ""
+        l_range         = []
 
-        for k, v in sorted(self.d_inputTreeCallback.items(),
+        if int(self.verbosityLevel) and self.toConsole():
+            l_range     = tqdm(sorted(self.d_inputTreeCallback.items(),
+                            key         = lambda kv: (kv[1]['diskUsage_raw']),
+                            reverse     = self.b_statsReverse),
+                            desc = ' Processing  stats')
+        else:
+            l_range     = sorted(self.d_inputTreeCallback.items(),
                             key         = lambda kv: (kv[1]['diskUsage_raw']),
-                            reverse     = self.b_statsReverse):
+                            reverse     = self.b_statsReverse)
+
+        for k, v in l_range:
             try:
-                str_report  = "files: %5d│ raw_size: %12d│ human_size: %8s│ dir: %s" % (\
-                        len(self.d_inputTree[k]),
-                        self.d_inputTreeCallback[k]['diskUsage_raw'],
-                        self.d_inputTreeCallback[k]['diskUsage_human'],
-                        k)
+                if not self.args['du'] and not self.args['duf']:
+                    str_report  += "files: %5d│ raw_size: %12d│ human_size: %8s│ dir: %s\n" % (\
+                            len(self.d_inputTree[k]),
+                            self.d_inputTreeCallback[k]['diskUsage_raw'],
+                            self.d_inputTreeCallback[k]['diskUsage_human'],
+                            k)
+                else:
+                    str_report += '%-10s%s\n' % (
+                        self.d_inputTreeCallback[k]['diskUsage_human'], k)
             except:
                 pass
             d_report = {
                 'files':            len(self.d_inputTree[k]),
                 'diskUsage_raw':    self.d_inputTreeCallback[k]['diskUsage_raw'],
                 'diskUsage_human':  self.d_inputTreeCallback[k]['diskUsage_human'],
                 'path':             k
             }
-            self.dp.qprint(str_report, level =2)
             l_stats.append(d_report)
             totalElements   += len(v)
             totalKeys       += 1
             totalSize       += self.d_inputTreeCallback[k]['diskUsage_raw']
         str_totalSize_human = self.sizeof_fmt(totalSize)
         return {
             'status':           True,
+            'report':           str_report,
             'dirs':             totalKeys,
             'files':            totalElements,
             'totalSize':        totalSize,
             'totalSize_human':  str_totalSize_human,
             'l_stats':          l_stats,
             'runTime':          other.toc()
         }
@@ -1305,15 +1358,15 @@
         """
         Simple environment check routine.
         """
         b_status    :   bool    = True
         str_error   :   str     = "no error"
         if not os.path.exists(self.str_inputDir):
             b_status    = False
-            if not self.args['json'] and not self.args['jsonStats']:
+            if self.toConsole():
                 error.warn(self, 'inputDirFail', exitToOS = True, drawBox = True)
             str_error   = 'error captured while accessing input directory'
         return {
             'status'    : b_status,
             'error'     : str_error
         }
 
@@ -1348,22 +1401,25 @@
         def stats_process():
             """
             Call the dir/files stats processing
             """
             nonlocal d_stats, b_status
             log         = slog()
             d_stats     = self.stats_compute()
+            if self.toConsole() or self.args['duf'] or self.args['du']:
+                self.dp.qprint(d_stats['report'], level = self.debugLevel)
             slog_filter = filters_show()
             log.title_set('Size statistics')
             if self.args['table3D']: log.render3D()
-            log('Total size (raw):        %d\n' % d_stats['totalSize']      )
-            log('Total size (friendly):   {:,}\n'.format(d_stats['totalSize']))
-            log('Total size (human):      %s\n' % d_stats['totalSize_human'])
-            log('Total files:             %s\n' % d_stats['files']          )
-            log('Total dirs:              %s' % d_stats['dirs']           )
+            log('Total size (raw):        %d\n' % d_stats['totalSize']          )
+            log('Total size (friendly):   {:,}\n'.format(d_stats['totalSize'])  )
+            log('Total size (human):      %s\n' % d_stats['totalSize_human']    )
+            log('Total files:             %s\n' % d_stats['files']              )
+            log('Total dirs:              %s\n' % d_stats['dirs']               )
+            log('Total runtime:           %5.3f s' % other.toc()                )
             b_status    = b_status and d_stats['status']
             return {
                 'status':       b_status,
                 'filterLog':    slog_filter,
                 'bodyLog':      log
             }
 
@@ -1388,32 +1444,37 @@
             for k, v in kwargs.items():
                 if k == 'timerStart':   b_timerStart    = bool(v)
             if b_timerStart:
                 other.tic()
 
         def postProcess_check() -> dict:
             """
-            Once a tree has been constructed, run some in-line
-            post processing operations if desired.
+            Once a tree has been constructed, run some
+            in-line post processing filtering and other
+            operations as desired.
             """
             nonlocal d_test, b_status, d_filter, d_stats
 
             if len(self.args['fileFilter']) or len(self.args['dirFilter']):
                 d_filter    = self.filterFileHitList()
                 b_status    = d_filter['status']
             if self.b_test:
                 d_test      = self.test_run(*args, **kwargs)
                 b_status    = b_status and d_test['status']
-            if self.b_stats or self.b_statsReverse:
+            if  self.b_stats or self.b_statsReverse or \
+                self.b_jsonStats or self.args['du'] or self.args['duf']:
                 d_stats     = stats_process()
                 b_status    = b_status and d_stats['status']
-                # pudb.set_trace()
-                if not self.args['json'] and not self.args['jsonStats']:
-                    print(d_stats['filterLog'].border_draw())
-                    print(d_stats['bodyLog'].border_draw())
+                self.verbosityLevel = 1
+                if self.toConsole():
+                    if not self.args['du'] and not self.args['duf']:
+                        print(d_stats['filterLog'].border_draw())
+                        print(d_stats['bodyLog'].border_draw())
+                    elif self.args['du'] or self.args['duf']:
+                        print(d_stats['bodyLog'])
                 else:
                     d_stats['filterLog']    = d_stats['filterLog'].json_dump()
                     d_stats['bodyLog']      = d_stats['bodyLog'].json_dump()
 
             return {
                 'status':   b_status,
                 'filter':   d_filter,
@@ -1435,21 +1496,19 @@
 
         timer_startIfNeeded()
         b_status, str_error = self.unpack(self.env_check(), 'status', 'error')
 
         if b_status:
             str_origDir = os.getcwd()
             d_tree      = self.tree_construct(
-                d_probe             = self.tree_probe(root= tree_resolveRoot()),
+                d_probe             = self.tree_probe(root = tree_resolveRoot()),
                 constructCallback   = self.dirsize_get
             )
             b_status    = d_tree['status']
-
             d_post      = postProcess_check()
-
             if self.b_jsonStats:
                 print(json.dumps(d_post['stats'], indent = 4, sort_keys = True))
 
             if self.b_relativeDir:
                 os.chdir(str_origDir)
 
         d_ret = {
```

### Comparing `pftree-3.2.8/pftree.egg-info/PKG-INFO` & `pftree-3.4.0/pftree.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pftree
-Version: 3.2.8
+Version: 3.4.0
 Summary: Utility to create dict representations of file system trees.
 Home-page: https://github.com/FNNDSC/pftree
 Author: FNNDSC
 Author-email: dev@babymri.org
 License: MIT
-Platform: UNKNOWN
 License-File: LICENSE
 
 pftree
 ======
 
 .. image:: https://badge.fury.io/py/pftree.svg
     :target: https://badge.fury.io/py/pftree
@@ -162,17 +161,33 @@
         [--verbosity <level>]
         Set the app verbosity level. This ranges from 0...<N> where internal
         log messages with a level=<M> will only display if M <= N. In this
         manner increasing the level here can be used to show more and more
         debugging info, assuming that debug messages in the code have been
         tagged with a level.
 
-        [--stats | --statsReverse]
-        If specified, return some stats to caller -- summary list ordered
-        by directory size (--statsReverse does a reverse sort).
+        [--stats | --statsReverse | --du | --duf]
+        If specified, return some stats to caller. The amount of information
+        returned depends on the --verbosity.
+
+        For --stats (and --statsReverse):
+
+            * --verbosity 0: return only a final summary of group statistics
+            * --verbosity 1: in addition, return a sorted (by size) list of
+                             subdirectories in the search tree
+            * --verbosity >1: same as above, but provide probing status updates.
+                              NOTE: this incurs a significant performance penalty!
+
+        For --du | --duf
+
+            similar to '--stats' but return directory lists in a fashion similar
+            to the GNU 'du' tool. Both of these set default verbosity values so that
+
+            * --du : only provide a summary
+            * --duf: provide the (full) sorted list as well
 
         [--3D]
         A "toy" flag that simply shows the final stats report with an ASCII
         3D effect.
 
         [--jsonStats]
         If specified, do a JSON dump of the stats.
@@ -216,14 +231,20 @@
                         --stats --verbosity 0
 
 Increasing the ``verbosity`` will produce increasing output on the console. Passing
 a ``--json`` will return a highly detailed JSON payload with considerable information.
 Passing a ``--jsonStats`` will only return a summary of the final stats on the
 filesystem probed. Note that the ``--verbosity`` flag is ignored if ``--json`` or ``--jsonStats`` are also present.
 
+.. code:: bash
+
+    pftree          --duf --inputDir /var/www/html
+
+Simpler CLI for a less "progress displaying" but faster response.
+
 test
 ~~~~
 
 Run a test down a target tree:
 
 .. code:: bash
 
@@ -232,8 +253,7 @@
                         --verbosity 1 --relativeDir                             \
                         --outputLeafDir 'preview-%%s'                           \
                         --test 0
 
 which will "copy" the input tree to the output, and save a file-ls.txt in each directory where necessary. Note the ``-r`` for 'relative' directory specification and the ``--outputLeafDir`` spec.
 
 _-30-_
-
```

### Comparing `pftree-3.2.8/setup.py` & `pftree-3.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 def readme():
     with open('README.rst') as f:
         return f.read()
 
 setup(
       name             =   'pftree',
-      version          =   '3.2.8',
+      version          =   '3.4.0',
       description      =   'Utility to create dict representations of file system trees.',
       long_description =   readme(),
       author           =   'FNNDSC',
       author_email     =   'dev@babymri.org',
       url              =   'https://github.com/FNNDSC/pftree',
       packages         =   ['pftree'],
       install_requires =   ['tqdm', 'pfmisc', 'pudb'],
```

