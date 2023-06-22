# Comparing `tmp/seqchromloader-0.6.0.tar.gz` & `tmp/seqchromloader-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seqchromloader-0.6.0.tar", last modified: Tue Jun 20 15:14:13 2023, max compression
+gzip compressed data, was "seqchromloader-0.6.1.tar", last modified: Thu Jun 22 02:00:20 2023, max compression
```

## Comparing `seqchromloader-0.6.0.tar` & `seqchromloader-0.6.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-06-20 15:14:13.169778 seqchromloader-0.6.0/
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     1086 2023-06-20 15:14:13.169450 seqchromloader-0.6.0/PKG-INFO
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      649 2023-03-27 19:08:58.000000 seqchromloader-0.6.0/README.md
-drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-06-20 15:14:13.152544 seqchromloader-0.6.0/seqchromloader/
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      313 2023-05-30 03:38:50.000000 seqchromloader-0.6.0/seqchromloader/__init__.py
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)    12423 2023-06-20 14:51:56.000000 seqchromloader-0.6.0/seqchromloader/loader.py
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)    14272 2023-06-20 14:56:57.000000 seqchromloader-0.6.0/seqchromloader/utils.py
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     7280 2023-06-20 14:39:51.000000 seqchromloader-0.6.0/seqchromloader/writer.py
-drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-06-20 15:14:13.162922 seqchromloader-0.6.0/seqchromloader.egg-info/
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     1086 2023-06-20 15:14:13.000000 seqchromloader-0.6.0/seqchromloader.egg-info/PKG-INFO
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      336 2023-06-20 15:14:13.000000 seqchromloader-0.6.0/seqchromloader.egg-info/SOURCES.txt
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)        1 2023-06-20 15:14:13.000000 seqchromloader-0.6.0/seqchromloader.egg-info/dependency_links.txt
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      126 2023-06-20 15:14:13.000000 seqchromloader-0.6.0/seqchromloader.egg-info/requires.txt
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)       15 2023-06-20 15:14:13.000000 seqchromloader-0.6.0/seqchromloader.egg-info/top_level.txt
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)       38 2023-06-20 15:14:13.169876 seqchromloader-0.6.0/setup.cfg
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     3368 2023-06-20 14:48:49.000000 seqchromloader-0.6.0/setup.py
-drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-06-20 15:14:13.168493 seqchromloader-0.6.0/tests/
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)    12376 2023-06-20 15:03:21.000000 seqchromloader-0.6.0/tests/test_writer_loader.py
+drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-06-22 02:00:20.853333 seqchromloader-0.6.1/
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     1086 2023-06-22 02:00:20.852929 seqchromloader-0.6.1/PKG-INFO
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      649 2023-03-27 19:08:58.000000 seqchromloader-0.6.1/README.md
+drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-06-22 02:00:20.837029 seqchromloader-0.6.1/seqchromloader/
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      313 2023-05-30 03:38:50.000000 seqchromloader-0.6.1/seqchromloader/__init__.py
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)    12423 2023-06-20 14:51:56.000000 seqchromloader-0.6.1/seqchromloader/loader.py
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)    14608 2023-06-22 01:59:36.000000 seqchromloader-0.6.1/seqchromloader/utils.py
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     7280 2023-06-20 14:39:51.000000 seqchromloader-0.6.1/seqchromloader/writer.py
+drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-06-22 02:00:20.846891 seqchromloader-0.6.1/seqchromloader.egg-info/
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     1086 2023-06-22 02:00:20.000000 seqchromloader-0.6.1/seqchromloader.egg-info/PKG-INFO
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      336 2023-06-22 02:00:20.000000 seqchromloader-0.6.1/seqchromloader.egg-info/SOURCES.txt
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)        1 2023-06-22 02:00:20.000000 seqchromloader-0.6.1/seqchromloader.egg-info/dependency_links.txt
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      126 2023-06-22 02:00:20.000000 seqchromloader-0.6.1/seqchromloader.egg-info/requires.txt
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)       15 2023-06-22 02:00:20.000000 seqchromloader-0.6.1/seqchromloader.egg-info/top_level.txt
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)       38 2023-06-22 02:00:20.853455 seqchromloader-0.6.1/setup.cfg
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     3368 2023-06-22 01:59:49.000000 seqchromloader-0.6.1/setup.py
+drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-06-22 02:00:20.852012 seqchromloader-0.6.1/tests/
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)    12376 2023-06-20 15:03:21.000000 seqchromloader-0.6.1/tests/test_writer_loader.py
```

### Comparing `seqchromloader-0.6.0/PKG-INFO` & `seqchromloader-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seqchromloader
-Version: 0.6.0
+Version: 0.6.1
 Summary: Sequence and chromatin dataloader for deep learning
 Home-page: https://github.com/yztxwd/seqchromloader
 Author-email: yztxwd@gmail.com
 Keywords: dataloder,pytorch,webdataset
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `seqchromloader-0.6.0/README.md` & `seqchromloader-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `seqchromloader-0.6.0/seqchromloader/loader.py` & `seqchromloader-0.6.1/seqchromloader/loader.py`

 * *Files identical despite different names*

### Comparing `seqchromloader-0.6.0/seqchromloader/utils.py` & `seqchromloader-0.6.1/seqchromloader/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -350,17 +350,22 @@
     
     return seq_array
 
 def extract_target(chrom, start, end, strand, target):
     if isinstance(target, pysam.AlignmentFile):
         target_array = np.array(target.count(chrom, start, end), dtype=np.float32)[np.newaxis]
     elif isinstance(target, pyBigWig.pyBigWig):
-        target_array = np.nan_to_num(target.values(chrom, start, end)).astype(np.float32)
-        if strand=="-":
-            target_array = target_array[::-1]
+        try:
+            target_array = np.nan_to_num(target.values(chrom, start, end)).astype(np.float32)
+            if strand=="-":
+                target_array = target_array[::-1]
+        except RuntimeError as e:
+            logging.warning(e)
+            logging.warning(f"RuntimeError happened when accessing {chrom}:{start}-{end}, it's probably due to at least one chromatin track bigwig doesn't have information in this region")
+            raise BigWigInaccessible(chrom, start, end)
     else:
         target_array = None
     return target_array
 
 def extract_info(chrom, start, end, label, genome_pyfaidx, bigwigs, target, strand="+", transforms:dict=None):
     seq_array = extract_dnaOneHot(chrom, start, end, strand, genome_pyfaidx)
 
@@ -381,8 +386,8 @@
         'label': label_array
     }
 
     if transforms is not None:
         for k,t in transforms.items(): 
             feature[k] = t(feature[k])
     
-    return feature
+    return feature
```

### Comparing `seqchromloader-0.6.0/seqchromloader/writer.py` & `seqchromloader-0.6.1/seqchromloader/writer.py`

 * *Files identical despite different names*

### Comparing `seqchromloader-0.6.0/seqchromloader.egg-info/PKG-INFO` & `seqchromloader-0.6.1/seqchromloader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seqchromloader
-Version: 0.6.0
+Version: 0.6.1
 Summary: Sequence and chromatin dataloader for deep learning
 Home-page: https://github.com/yztxwd/seqchromloader
 Author-email: yztxwd@gmail.com
 Keywords: dataloder,pytorch,webdataset
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `seqchromloader-0.6.0/setup.py` & `seqchromloader-0.6.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     # The version of your project.
     # Usually, it would be in the form of:
     # major.minor.patch
     # eg: 1.0.0, 1.0.1, 3.0.2, 5.0-beta, etc.
     # You CANNOT upload two versions of your package with the same version number
     # This field is REQUIRED
-    version="0.6.0",
+    version="0.6.1",
 
     # The packages that constitute your project.
     # For my project, I have only one - "pydash".
     # Either you could write the name of the package, or
     # alternatively use setuptools.findpackages()
     #
     # If you only have one file, instead of a package,
```

### Comparing `seqchromloader-0.6.0/tests/test_writer_loader.py` & `seqchromloader-0.6.1/tests/test_writer_loader.py`

 * *Files identical despite different names*

