# Comparing `tmp/reswarm-0.0.8.tar.gz` & `tmp/reswarm-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reswarm-0.0.8.tar", last modified: Thu Jun 23 08:03:37 2022, max compression
+gzip compressed data, was "reswarm-0.0.9.tar", last modified: Thu Jun 23 08:33:41 2022, max compression
```

## Comparing `reswarm-0.0.8.tar` & `reswarm-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 ruben      (501) staff       (20)        0 2022-06-23 08:03:37.575952 reswarm-0.0.8/
--rw-r--r--   0 ruben      (501) staff       (20)     1073 2022-03-16 19:54:31.000000 reswarm-0.0.8/LICENSE
--rw-r--r--   0 ruben      (501) staff       (20)      103 2022-03-16 19:54:31.000000 reswarm-0.0.8/MANIFEST.in
--rw-r--r--   0 ruben      (501) staff       (20)     1151 2022-06-23 08:03:37.575648 reswarm-0.0.8/PKG-INFO
--rw-r--r--   0 ruben      (501) staff       (20)      773 2022-03-16 20:29:58.000000 reswarm-0.0.8/README.md
--rw-r--r--   0 ruben      (501) staff       (20)      103 2022-03-16 19:54:31.000000 reswarm-0.0.8/pyproject.toml
--rw-r--r--   0 ruben      (501) staff       (20)       25 2022-06-22 13:25:41.000000 reswarm-0.0.8/requirements.txt
-drwxr-xr-x   0 ruben      (501) staff       (20)        0 2022-06-23 08:03:37.573454 reswarm-0.0.8/reswarm/
--rw-r--r--   0 ruben      (501) staff       (20)       29 2022-03-16 19:54:31.000000 reswarm-0.0.8/reswarm/__init__.py
--rw-r--r--   0 ruben      (501) staff       (20)     3023 2022-06-23 08:02:00.000000 reswarm-0.0.8/reswarm/crossbar.py
--rw-r--r--   0 ruben      (501) staff       (20)     1186 2022-06-23 06:21:17.000000 reswarm-0.0.8/reswarm/reswarm.py
-drwxr-xr-x   0 ruben      (501) staff       (20)        0 2022-06-23 08:03:37.575126 reswarm-0.0.8/reswarm.egg-info/
--rw-r--r--   0 ruben      (501) staff       (20)     1151 2022-06-23 08:03:37.000000 reswarm-0.0.8/reswarm.egg-info/PKG-INFO
--rw-r--r--   0 ruben      (501) staff       (20)      283 2022-06-23 08:03:37.000000 reswarm-0.0.8/reswarm.egg-info/SOURCES.txt
--rw-r--r--   0 ruben      (501) staff       (20)        1 2022-06-23 08:03:37.000000 reswarm-0.0.8/reswarm.egg-info/dependency_links.txt
--rw-r--r--   0 ruben      (501) staff       (20)       26 2022-06-23 08:03:37.000000 reswarm-0.0.8/reswarm.egg-info/requires.txt
--rw-r--r--   0 ruben      (501) staff       (20)        8 2022-06-23 08:03:37.000000 reswarm-0.0.8/reswarm.egg-info/top_level.txt
--rw-r--r--   0 ruben      (501) staff       (20)       38 2022-06-23 08:03:37.576094 reswarm-0.0.8/setup.cfg
--rw-r--r--   0 ruben      (501) staff       (20)      757 2022-06-23 08:03:00.000000 reswarm-0.0.8/setup.py
+drwxr-xr-x   0 ruben      (501) staff       (20)        0 2022-06-23 08:33:41.432631 reswarm-0.0.9/
+-rw-r--r--   0 ruben      (501) staff       (20)     1073 2022-03-16 19:54:31.000000 reswarm-0.0.9/LICENSE
+-rw-r--r--   0 ruben      (501) staff       (20)      103 2022-03-16 19:54:31.000000 reswarm-0.0.9/MANIFEST.in
+-rw-r--r--   0 ruben      (501) staff       (20)     1151 2022-06-23 08:33:41.432345 reswarm-0.0.9/PKG-INFO
+-rw-r--r--   0 ruben      (501) staff       (20)      773 2022-03-16 20:29:58.000000 reswarm-0.0.9/README.md
+-rw-r--r--   0 ruben      (501) staff       (20)      103 2022-03-16 19:54:31.000000 reswarm-0.0.9/pyproject.toml
+-rw-r--r--   0 ruben      (501) staff       (20)       25 2022-06-22 13:25:41.000000 reswarm-0.0.9/requirements.txt
+drwxr-xr-x   0 ruben      (501) staff       (20)        0 2022-06-23 08:33:41.429867 reswarm-0.0.9/reswarm/
+-rw-r--r--   0 ruben      (501) staff       (20)       29 2022-03-16 19:54:31.000000 reswarm-0.0.9/reswarm/__init__.py
+-rw-r--r--   0 ruben      (501) staff       (20)     3006 2022-06-23 08:32:48.000000 reswarm-0.0.9/reswarm/crossbar.py
+-rw-r--r--   0 ruben      (501) staff       (20)     1186 2022-06-23 06:21:17.000000 reswarm-0.0.9/reswarm/reswarm.py
+drwxr-xr-x   0 ruben      (501) staff       (20)        0 2022-06-23 08:33:41.431927 reswarm-0.0.9/reswarm.egg-info/
+-rw-r--r--   0 ruben      (501) staff       (20)     1151 2022-06-23 08:33:41.000000 reswarm-0.0.9/reswarm.egg-info/PKG-INFO
+-rw-r--r--   0 ruben      (501) staff       (20)      283 2022-06-23 08:33:41.000000 reswarm-0.0.9/reswarm.egg-info/SOURCES.txt
+-rw-r--r--   0 ruben      (501) staff       (20)        1 2022-06-23 08:33:41.000000 reswarm-0.0.9/reswarm.egg-info/dependency_links.txt
+-rw-r--r--   0 ruben      (501) staff       (20)       26 2022-06-23 08:33:41.000000 reswarm-0.0.9/reswarm.egg-info/requires.txt
+-rw-r--r--   0 ruben      (501) staff       (20)        8 2022-06-23 08:33:41.000000 reswarm-0.0.9/reswarm.egg-info/top_level.txt
+-rw-r--r--   0 ruben      (501) staff       (20)       38 2022-06-23 08:33:41.432728 reswarm-0.0.9/setup.cfg
+-rw-r--r--   0 ruben      (501) staff       (20)      757 2022-06-23 08:33:30.000000 reswarm-0.0.9/setup.py
```

### Comparing `reswarm-0.0.8/LICENSE` & `reswarm-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `reswarm-0.0.8/PKG-INFO` & `reswarm-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reswarm
-Version: 0.0.8
+Version: 0.0.9
 Summary: Aids users in publishing data to a Record Evolution Datapod
 Home-page: https://github.com/RecordEvolution/reswarm-python
 Author: Record Evolution GmbH
 Author-email: marko.petzold@record-evolution.de
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `reswarm-0.0.8/README.md` & `reswarm-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `reswarm-0.0.8/reswarm/crossbar.py` & `reswarm-0.0.9/reswarm/crossbar.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,14 @@
         self.loop = None
         self.quiet = quiet
         self.serial_number = serial_number
 
     def start(self):
         t = threading.Thread(target=self._initSessionLoop)
         t.start()
-        t.join()
 
     def _setSession(self, session):
         self.session = session
 
     def getEventLoop(self):
         while self.loop == None:
             continue
```

### Comparing `reswarm-0.0.8/reswarm/reswarm.py` & `reswarm-0.0.9/reswarm/reswarm.py`

 * *Files identical despite different names*

### Comparing `reswarm-0.0.8/reswarm.egg-info/PKG-INFO` & `reswarm-0.0.9/reswarm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reswarm
-Version: 0.0.8
+Version: 0.0.9
 Summary: Aids users in publishing data to a Record Evolution Datapod
 Home-page: https://github.com/RecordEvolution/reswarm-python
 Author: Record Evolution GmbH
 Author-email: marko.petzold@record-evolution.de
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `reswarm-0.0.8/setup.py` & `reswarm-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         requirements.append(line.strip())
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='reswarm',
-    version='0.0.8',
+    version='0.0.9',
     description='Aids users in publishing data to a Record Evolution Datapod',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/RecordEvolution/reswarm-python',
     author='Record Evolution GmbH',
     author_email='marko.petzold@record-evolution.de',
     packages=find_packages(),
```

