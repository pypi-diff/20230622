# Comparing `tmp/h5parm-1.0.3.tar.gz` & `tmp/h5parm-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "h5parm-1.0.3.tar", last modified: Thu May 18 12:01:34 2023, max compression
+gzip compressed data, was "h5parm-1.0.4.tar", last modified: Thu May 18 12:41:51 2023, max compression
```

## Comparing `h5parm-1.0.3.tar` & `h5parm-1.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-05-18 12:01:34.339587 h5parm-1.0.3/
--rw-rw-r--   0 albert    (1000) albert    (1000)    11357 2021-06-02 01:08:45.000000 h5parm-1.0.3/LICENSE
--rw-rw-r--   0 albert    (1000) albert    (1000)     1348 2023-05-18 12:01:34.339587 h5parm-1.0.3/PKG-INFO
--rw-rw-r--   0 albert    (1000) albert    (1000)      903 2022-05-21 17:50:27.000000 h5parm-1.0.3/README.md
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-05-18 12:01:34.335586 h5parm-1.0.3/h5parm/
--rw-rw-r--   0 albert    (1000) albert    (1000)      141 2021-06-02 01:08:45.000000 h5parm-1.0.3/h5parm/__init__.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-05-18 12:01:34.339587 h5parm-1.0.3/h5parm/arrays/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2021-06-02 01:08:45.000000 h5parm-1.0.3/h5parm/arrays/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)   134014 2022-05-21 17:50:27.000000 h5parm-1.0.3/h5parm/arrays/dsa2000.W.cfg
--rwxrwxr-x   0 albert    (1000) albert    (1000)     2455 2021-06-02 01:08:45.000000 h5parm-1.0.3/h5parm/arrays/gmrtPos.cfg
--rw-rw-r--   0 albert    (1000) albert    (1000)     6649 2021-06-02 01:08:45.000000 h5parm-1.0.3/h5parm/arrays/lofar.antenna.cfg
--rwxrwxr-x   0 albert    (1000) albert    (1000)     2844 2021-06-02 01:08:45.000000 h5parm-1.0.3/h5parm/arrays/lofar.hba.antenna.cfg
--rw-rw-r--   0 albert    (1000) albert    (1000)    33542 2023-05-18 11:59:57.000000 h5parm-1.0.3/h5parm/datapack.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     2271 2021-06-02 01:08:45.000000 h5parm-1.0.3/h5parm/maintenance.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    15652 2023-05-18 09:03:26.000000 h5parm-1.0.3/h5parm/utils.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-05-18 12:01:34.335586 h5parm-1.0.3/h5parm.egg-info/
--rw-rw-r--   0 albert    (1000) albert    (1000)     1348 2023-05-18 12:01:34.000000 h5parm-1.0.3/h5parm.egg-info/PKG-INFO
--rw-rw-r--   0 albert    (1000) albert    (1000)      396 2023-05-18 12:01:34.000000 h5parm-1.0.3/h5parm.egg-info/SOURCES.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)        1 2023-05-18 12:01:34.000000 h5parm-1.0.3/h5parm.egg-info/dependency_links.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)        7 2023-05-18 12:01:34.000000 h5parm-1.0.3/h5parm.egg-info/top_level.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)       38 2023-05-18 12:01:34.339587 h5parm-1.0.3/setup.cfg
--rwxrwxr-x   0 albert    (1000) albert    (1000)     1135 2023-05-18 12:01:23.000000 h5parm-1.0.3/setup.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-05-18 12:41:51.597006 h5parm-1.0.4/
+-rw-rw-r--   0 albert    (1000) albert    (1000)    11357 2021-06-02 01:08:45.000000 h5parm-1.0.4/LICENSE
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1348 2023-05-18 12:41:51.597006 h5parm-1.0.4/PKG-INFO
+-rw-rw-r--   0 albert    (1000) albert    (1000)      903 2022-05-21 17:50:27.000000 h5parm-1.0.4/README.md
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-05-18 12:41:51.593006 h5parm-1.0.4/h5parm/
+-rw-rw-r--   0 albert    (1000) albert    (1000)      141 2021-06-02 01:08:45.000000 h5parm-1.0.4/h5parm/__init__.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-05-18 12:41:51.597006 h5parm-1.0.4/h5parm/arrays/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2021-06-02 01:08:45.000000 h5parm-1.0.4/h5parm/arrays/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)   134014 2022-05-21 17:50:27.000000 h5parm-1.0.4/h5parm/arrays/dsa2000.W.cfg
+-rwxrwxr-x   0 albert    (1000) albert    (1000)     2455 2021-06-02 01:08:45.000000 h5parm-1.0.4/h5parm/arrays/gmrtPos.cfg
+-rw-rw-r--   0 albert    (1000) albert    (1000)     6649 2021-06-02 01:08:45.000000 h5parm-1.0.4/h5parm/arrays/lofar.antenna.cfg
+-rwxrwxr-x   0 albert    (1000) albert    (1000)     2844 2021-06-02 01:08:45.000000 h5parm-1.0.4/h5parm/arrays/lofar.hba.antenna.cfg
+-rw-rw-r--   0 albert    (1000) albert    (1000)    33533 2023-05-18 12:41:43.000000 h5parm-1.0.4/h5parm/datapack.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2271 2021-06-02 01:08:45.000000 h5parm-1.0.4/h5parm/maintenance.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    15652 2023-05-18 09:03:26.000000 h5parm-1.0.4/h5parm/utils.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-05-18 12:41:51.593006 h5parm-1.0.4/h5parm.egg-info/
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1348 2023-05-18 12:41:51.000000 h5parm-1.0.4/h5parm.egg-info/PKG-INFO
+-rw-rw-r--   0 albert    (1000) albert    (1000)      396 2023-05-18 12:41:51.000000 h5parm-1.0.4/h5parm.egg-info/SOURCES.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)        1 2023-05-18 12:41:51.000000 h5parm-1.0.4/h5parm.egg-info/dependency_links.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)        7 2023-05-18 12:41:51.000000 h5parm-1.0.4/h5parm.egg-info/top_level.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)       38 2023-05-18 12:41:51.597006 h5parm-1.0.4/setup.cfg
+-rwxrwxr-x   0 albert    (1000) albert    (1000)     1135 2023-05-18 12:41:43.000000 h5parm-1.0.4/setup.py
```

### Comparing `h5parm-1.0.3/LICENSE` & `h5parm-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `h5parm-1.0.3/PKG-INFO` & `h5parm-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h5parm
-Version: 1.0.3
+Version: 1.0.4
 Summary: H5Parm data pack interface
 Home-page: https://github.com/joshuaalbert/h5parm
 Author: Joshua G. Albert
 Author-email: albert@strw.leidenuniv.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `h5parm-1.0.3/README.md` & `h5parm-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `h5parm-1.0.3/h5parm/arrays/dsa2000.W.cfg` & `h5parm-1.0.4/h5parm/arrays/dsa2000.W.cfg`

 * *Files identical despite different names*

### Comparing `h5parm-1.0.3/h5parm/arrays/gmrtPos.cfg` & `h5parm-1.0.4/h5parm/arrays/gmrtPos.cfg`

 * *Files identical despite different names*

### Comparing `h5parm-1.0.3/h5parm/arrays/lofar.antenna.cfg` & `h5parm-1.0.4/h5parm/arrays/lofar.antenna.cfg`

 * *Files identical despite different names*

### Comparing `h5parm-1.0.3/h5parm/arrays/lofar.hba.antenna.cfg` & `h5parm-1.0.4/h5parm/arrays/lofar.hba.antenna.cfg`

 * *Files identical despite different names*

### Comparing `h5parm-1.0.3/h5parm/datapack.py` & `h5parm-1.0.4/h5parm/datapack.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         f.write('# Created on {0} by Joshua G. Albert\n'.format(time.strftime("%a %c", time.localtime())))
         f.write('#ITRS(m)\n')
         f.write('#station\tX\tY\tZ\n')
         i = 0
         while i < Na:
             f.write(
                 '{3},{0:1.9e},{1:1.9e},{2:1.9e}'.format(antennas[i, 0], antennas[i, 1], antennas[i, 2],
-                                                        labels[i].decode()))
+                                                        labels[i]))
             if i < Na - 1:
                 f.write('\n')
             i += 1
 
 
 def update_h5parm(old_h5parm, new_h5parm):
     """
```

### Comparing `h5parm-1.0.3/h5parm/maintenance.py` & `h5parm-1.0.4/h5parm/maintenance.py`

 * *Files identical despite different names*

### Comparing `h5parm-1.0.3/h5parm/utils.py` & `h5parm-1.0.4/h5parm/utils.py`

 * *Files identical despite different names*

### Comparing `h5parm-1.0.3/h5parm.egg-info/PKG-INFO` & `h5parm-1.0.4/h5parm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h5parm
-Version: 1.0.3
+Version: 1.0.4
 Summary: H5Parm data pack interface
 Home-page: https://github.com/joshuaalbert/h5parm
 Author: Joshua G. Albert
 Author-email: albert@strw.leidenuniv.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `h5parm-1.0.3/setup.py` & `h5parm-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
                   'tables>=' + __minimum_tables_version__,
                   'astropy>=' + __minimum_astropy_version__]
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='h5parm',
-      version='1.0.3',
+      version='1.0.4',
       description='H5Parm data pack interface',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/joshuaalbert/h5parm",
       author='Joshua G. Albert',
       author_email='albert@strw.leidenuniv.nl',
       setup_requires=setup_requires,
```

