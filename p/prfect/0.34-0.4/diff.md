# Comparing `tmp/prfect-0.34.tar.gz` & `tmp/prfect-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prfect-0.34.tar", last modified: Thu Jun 22 01:47:08 2023, max compression
+gzip compressed data, was "/Users/katelyn/develop/prfect/dist/tmp30oixgxt/prfect-0.4.tar", last modified: Thu May 19 16:53:09 2022, max compression
```

## Comparing `prfect-0.34.tar` & `prfect-0.4.tar`

### file list

```diff
@@ -1,31 +1,30 @@
-drwxr-xr-x   0 katelyn    (501) staff       (20)        0 2023-06-22 01:47:08.942836 prfect-0.34/
--rw-r--r--   0 katelyn    (501) staff       (20)    35149 2023-06-22 01:35:09.000000 prfect-0.34/LICENSE
--rw-r--r--   0 katelyn    (501) staff       (20)       95 2023-06-22 01:35:09.000000 prfect-0.34/MANIFEST.in
--rw-r--r--   0 katelyn    (501) staff       (20)     3126 2023-06-22 01:47:08.942580 prfect-0.34/PKG-INFO
--rw-r--r--   0 katelyn    (501) staff       (20)     2644 2023-06-22 01:35:09.000000 prfect-0.34/README.md
--rw-r--r--   0 katelyn    (501) staff       (20)        5 2023-06-22 01:44:01.000000 prfect-0.34/VERSION.md
-drwxr-xr-x   0 katelyn    (501) staff       (20)        0 2023-06-22 01:47:08.938424 prfect-0.34/prfect/
--rw-r--r--   0 katelyn    (501) staff       (20)        0 2023-06-22 01:35:11.000000 prfect-0.34/prfect/__init__.py
--rw-r--r--   0 katelyn    (501) staff       (20)  1056098 2023-06-22 01:35:11.000000 prfect-0.34/prfect/clf.0.24.2.pkl
--rw-r--r--   0 katelyn    (501) staff       (20)  1051706 2023-06-22 01:35:11.000000 prfect-0.34/prfect/clf.1.1.1.pkl
--rw-r--r--   0 katelyn    (501) staff       (20)     3097 2023-06-22 01:35:11.000000 prfect-0.34/prfect/codons.py
--rw-r--r--   0 katelyn    (501) staff       (20)     1883 2023-06-22 01:35:11.000000 prfect-0.34/prfect/feature.py
--rw-r--r--   0 katelyn    (501) staff       (20)       99 2023-06-22 01:35:11.000000 prfect-0.34/prfect/file.py
--rw-r--r--   0 katelyn    (501) staff       (20)     5338 2023-06-22 01:35:11.000000 prfect-0.34/prfect/functions.py
--rw-r--r--   0 katelyn    (501) staff       (20)     7207 2023-06-22 01:35:11.000000 prfect-0.34/prfect/locus.py
--rw-r--r--   0 katelyn    (501) staff       (20)     4150 2023-06-22 01:35:11.000000 prfect-0.34/prfect/prodigal.py
--rw-r--r--   0 katelyn    (501) staff       (20)      972 2023-06-22 01:35:11.000000 prfect-0.34/prfect/stats.py
-drwxr-xr-x   0 katelyn    (501) staff       (20)        0 2023-06-22 01:47:08.939657 prfect-0.34/prfect.egg-info/
--rw-r--r--   0 katelyn    (501) staff       (20)     3126 2023-06-22 01:47:08.000000 prfect-0.34/prfect.egg-info/PKG-INFO
--rw-r--r--   0 katelyn    (501) staff       (20)      455 2023-06-22 01:47:08.000000 prfect-0.34/prfect.egg-info/SOURCES.txt
--rw-r--r--   0 katelyn    (501) staff       (20)        1 2023-06-22 01:47:08.000000 prfect-0.34/prfect.egg-info/dependency_links.txt
--rw-r--r--   0 katelyn    (501) staff       (20)       90 2023-06-22 01:47:08.000000 prfect-0.34/prfect.egg-info/requires.txt
--rw-r--r--   0 katelyn    (501) staff       (20)        7 2023-06-22 01:47:08.000000 prfect-0.34/prfect.egg-info/top_level.txt
--rw-r--r--   0 katelyn    (501) staff       (20)     7212 2023-06-22 01:43:54.000000 prfect-0.34/prfect.py
--rw-r--r--   0 katelyn    (501) staff       (20)       38 2023-06-22 01:47:08.942906 prfect-0.34/setup.cfg
--rw-r--r--   0 katelyn    (501) staff       (20)     1562 2023-06-22 01:35:11.000000 prfect-0.34/setup.py
-drwxr-xr-x   0 katelyn    (501) staff       (20)        0 2023-06-22 01:47:08.942305 prfect-0.34/test/
--rw-r--r--   0 katelyn    (501) staff       (20)   124036 2023-06-22 01:35:11.000000 prfect-0.34/test/SPP1.gbk
--rw-r--r--   0 katelyn    (501) staff       (20)    68654 2023-06-22 01:35:11.000000 prfect-0.34/test/covid19.gbk
--rw-r--r--   0 katelyn    (501) staff       (20)   176792 2023-06-22 01:35:11.000000 prfect-0.34/test/lambda.gbk
--rw-r--r--   0 katelyn    (501) staff       (20)     7636 2023-06-22 01:35:11.000000 prfect-0.34/test/phiX174.gbk
+drwxr-xr-x   0 katelyn    (501) staff       (20)        0 2022-05-19 16:53:09.933264 prfect-0.4/
+-rw-r--r--   0 katelyn    (501) staff       (20)    35149 2022-02-15 21:45:34.000000 prfect-0.4/LICENSE
+-rw-r--r--   0 katelyn    (501) staff       (20)       95 2022-05-19 06:36:08.000000 prfect-0.4/MANIFEST.in
+-rw-r--r--   0 katelyn    (501) staff       (20)      872 2022-05-19 16:53:09.933047 prfect-0.4/PKG-INFO
+-rw-r--r--   0 katelyn    (501) staff       (20)      391 2022-03-02 22:17:37.000000 prfect-0.4/README.md
+-rw-r--r--   0 katelyn    (501) staff       (20)        4 2022-05-19 16:48:44.000000 prfect-0.4/VERSION
+drwxr-xr-x   0 katelyn    (501) staff       (20)        0 2022-05-19 16:53:09.927464 prfect-0.4/prfect/
+-rw-r--r--   0 katelyn    (501) staff       (20)        0 2022-03-02 22:14:51.000000 prfect-0.4/prfect/__init__.py
+-rw-r--r--   0 katelyn    (501) staff       (20)   458055 2022-05-18 03:20:38.000000 prfect-0.4/prfect/all.pkl
+-rw-r--r--   0 katelyn    (501) staff       (20)     3097 2022-02-15 21:32:22.000000 prfect-0.4/prfect/codons.py
+-rw-r--r--   0 katelyn    (501) staff       (20)     1883 2022-02-19 01:13:27.000000 prfect-0.4/prfect/feature.py
+-rw-r--r--   0 katelyn    (501) staff       (20)       99 2022-04-07 22:41:53.000000 prfect-0.4/prfect/file.py
+-rw-r--r--   0 katelyn    (501) staff       (20)    20322 2022-05-19 06:33:56.000000 prfect-0.4/prfect/locus.py
+-rw-r--r--   0 katelyn    (501) staff       (20)     6285 2022-05-19 06:24:30.000000 prfect-0.4/prfect/motif.py
+-rw-r--r--   0 katelyn    (501) staff       (20)     4150 2022-03-17 21:15:37.000000 prfect-0.4/prfect/prodigal.py
+-rw-r--r--   0 katelyn    (501) staff       (20)      972 2022-02-15 21:34:17.000000 prfect-0.4/prfect/stats.py
+drwxr-xr-x   0 katelyn    (501) staff       (20)        0 2022-05-19 16:53:09.928649 prfect-0.4/prfect.egg-info/
+-rw-r--r--   0 katelyn    (501) staff       (20)      872 2022-05-19 16:53:09.000000 prfect-0.4/prfect.egg-info/PKG-INFO
+-rw-r--r--   0 katelyn    (501) staff       (20)      420 2022-05-19 16:53:09.000000 prfect-0.4/prfect.egg-info/SOURCES.txt
+-rw-r--r--   0 katelyn    (501) staff       (20)        1 2022-05-19 16:53:09.000000 prfect-0.4/prfect.egg-info/dependency_links.txt
+-rw-r--r--   0 katelyn    (501) staff       (20)       59 2022-05-19 16:53:09.000000 prfect-0.4/prfect.egg-info/requires.txt
+-rw-r--r--   0 katelyn    (501) staff       (20)        7 2022-05-19 16:53:09.000000 prfect-0.4/prfect.egg-info/top_level.txt
+-rw-r--r--   0 katelyn    (501) staff       (20)     2685 2022-05-19 16:51:24.000000 prfect-0.4/prfect.py
+-rw-r--r--   0 katelyn    (501) staff       (20)       38 2022-05-19 16:53:09.933326 prfect-0.4/setup.cfg
+-rw-r--r--   0 katelyn    (501) staff       (20)     1523 2022-05-19 06:15:50.000000 prfect-0.4/setup.py
+drwxr-xr-x   0 katelyn    (501) staff       (20)        0 2022-05-19 16:53:09.932034 prfect-0.4/test/
+-rw-r--r--   0 katelyn    (501) staff       (20)   124036 2022-03-16 22:09:47.000000 prfect-0.4/test/SPP1.gbk
+-rw-r--r--   0 katelyn    (501) staff       (20)    68654 2022-05-18 18:52:54.000000 prfect-0.4/test/covid19.gbk
+-rw-r--r--   0 katelyn    (501) staff       (20)   176792 2022-05-18 19:06:26.000000 prfect-0.4/test/lambda.gbk
+-rw-r--r--   0 katelyn    (501) staff       (20)     7636 2022-02-28 21:49:57.000000 prfect-0.4/test/phiX174.gbk
```

### Comparing `prfect-0.34/LICENSE` & `prfect-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `prfect-0.34/prfect/codons.py` & `prfect-0.4/prfect/codons.py`

 * *Files identical despite different names*

### Comparing `prfect-0.34/prfect/feature.py` & `prfect-0.4/prfect/feature.py`

 * *Files identical despite different names*

### Comparing `prfect-0.34/prfect/prodigal.py` & `prfect-0.4/prfect/prodigal.py`

 * *Files identical despite different names*

### Comparing `prfect-0.34/prfect/stats.py` & `prfect-0.4/prfect/stats.py`

 * *Files identical despite different names*

### Comparing `prfect-0.34/setup.py` & `prfect-0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 def readme():
 	with open("README.md", "r") as fh:
 		long_desc = fh.read()
 	return long_desc
 
 def get_version():
-	with open("VERSION.md", 'r') as f:
+	with open("VERSION", 'r') as f:
 		v = f.readline().strip()
 		return v
 
 def main():
 	setup (
 		name = 'prfect',
 		version = get_version(),
@@ -49,14 +49,14 @@
 			"Programming Language :: Python :: 3",
 			"License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
 			"Operating System :: OS Independent",
 		],
 		python_requires='>3.5.2',
 		packages=find_packages(),
 		package_data = {'': ['*.pkl'],},
-		install_requires=['scikit-learn>=0.24.0','sklearn','numpy','pandas','genbank','LinearFold','hotknots','score_rbs', 'packaging'],
+		install_requires=['sklearn','numpy','pandas','genbank','LinearFold','hotknots','score_rbs'],
 		#ext_modules = [module],
 	)
 
 
 if __name__ == "__main__":
 	main()
```

### Comparing `prfect-0.34/test/SPP1.gbk` & `prfect-0.4/test/SPP1.gbk`

 * *Files identical despite different names*

### Comparing `prfect-0.34/test/covid19.gbk` & `prfect-0.4/test/covid19.gbk`

 * *Files identical despite different names*

### Comparing `prfect-0.34/test/lambda.gbk` & `prfect-0.4/test/lambda.gbk`

 * *Files identical despite different names*

### Comparing `prfect-0.34/test/phiX174.gbk` & `prfect-0.4/test/phiX174.gbk`

 * *Files identical despite different names*

