# Comparing `tmp/cryptography318-0.4.1.tar.gz` & `tmp/cryptography318-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptography318-0.4.1.tar", last modified: Thu Jun 22 03:43:29 2023, max compression
+gzip compressed data, was "cryptography318-0.4.2.tar", last modified: Thu Jun 22 03:47:31 2023, max compression
```

## Comparing `cryptography318-0.4.1.tar` & `cryptography318-0.4.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-22 03:43:29.192597 cryptography318-0.4.1/
--rw-r--r--   0 andrew     (501) staff       (20)     1718 2023-06-22 03:43:29.192433 cryptography318-0.4.1/PKG-INFO
--rw-r--r--   0 andrew     (501) staff       (20)     1128 2023-03-15 02:24:32.000000 cryptography318-0.4.1/README.md
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-22 03:43:29.186820 cryptography318-0.4.1/cryptography318/
--rw-r--r--   0 andrew     (501) staff       (20)      987 2023-03-15 00:29:52.000000 cryptography318-0.4.1/cryptography318/__init__.py
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-22 03:43:29.188674 cryptography318-0.4.1/cryptography318/dlp/
--rw-r--r--   0 andrew     (501) staff       (20)      150 2023-03-15 00:26:39.000000 cryptography318-0.4.1/cryptography318/dlp/__init__.py
--rw-r--r--   0 andrew     (501) staff       (20)     5516 2023-03-15 01:53:10.000000 cryptography318-0.4.1/cryptography318/dlp/dlp.py
--rw-r--r--   0 andrew     (501) staff       (20)     2901 2023-03-15 01:50:49.000000 cryptography318-0.4.1/cryptography318/dlp/icm.py
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-22 03:43:29.190171 cryptography318-0.4.1/cryptography318/factor/
--rw-r--r--   0 andrew     (501) staff       (20)      370 2023-06-19 20:52:32.000000 cryptography318-0.4.1/cryptography318/factor/__init__.py
--rw-r--r--   0 andrew     (501) staff       (20)    10578 2023-03-15 00:26:39.000000 cryptography318-0.4.1/cryptography318/factor/curve.py
--rw-r--r--   0 andrew     (501) staff       (20)     8832 2023-03-15 00:26:39.000000 cryptography318-0.4.1/cryptography318/factor/elliptic.py
--rw-r--r--   0 andrew     (501) staff       (20)     7006 2023-06-22 03:36:31.000000 cryptography318-0.4.1/cryptography318/factor/factor.py
--rw-r--r--   0 andrew     (501) staff       (20)    10926 2023-06-22 03:42:30.000000 cryptography318-0.4.1/cryptography318/factor/siqs.py
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-22 03:43:29.190663 cryptography318-0.4.1/cryptography318/linalg/
--rw-r--r--   0 andrew     (501) staff       (20)      117 2023-03-15 00:26:39.000000 cryptography318-0.4.1/cryptography318/linalg/__init__.py
--rw-r--r--   0 andrew     (501) staff       (20)     7370 2023-03-15 00:27:38.000000 cryptography318-0.4.1/cryptography318/linalg/linalg.py
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-22 03:43:29.191504 cryptography318-0.4.1/cryptography318/prime/
--rw-r--r--   0 andrew     (501) staff       (20)      478 2023-06-19 20:52:32.000000 cryptography318-0.4.1/cryptography318/prime/__init__.py
--rw-r--r--   0 andrew     (501) staff       (20)     3531 2023-03-15 01:46:28.000000 cryptography318-0.4.1/cryptography318/prime/bailliepsw_helper.py
--rw-r--r--   0 andrew     (501) staff       (20)    24741 2023-06-22 03:36:14.000000 cryptography318-0.4.1/cryptography318/prime/prime.py
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-22 03:43:29.192098 cryptography318-0.4.1/cryptography318/utils/
--rw-r--r--   0 andrew     (501) staff       (20)       66 2022-03-18 04:48:41.000000 cryptography318-0.4.1/cryptography318/utils/__init__.py
--rw-r--r--   0 andrew     (501) staff       (20)     3640 2023-06-19 20:19:13.000000 cryptography318-0.4.1/cryptography318/utils/utils.py
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-22 03:43:29.187861 cryptography318-0.4.1/cryptography318.egg-info/
--rw-r--r--   0 andrew     (501) staff       (20)     1718 2023-06-22 03:43:29.000000 cryptography318-0.4.1/cryptography318.egg-info/PKG-INFO
--rw-r--r--   0 andrew     (501) staff       (20)      733 2023-06-22 03:43:29.000000 cryptography318-0.4.1/cryptography318.egg-info/SOURCES.txt
--rw-r--r--   0 andrew     (501) staff       (20)        1 2023-06-22 03:43:29.000000 cryptography318-0.4.1/cryptography318.egg-info/dependency_links.txt
--rw-r--r--   0 andrew     (501) staff       (20)       26 2023-06-22 03:43:29.000000 cryptography318-0.4.1/cryptography318.egg-info/requires.txt
--rw-r--r--   0 andrew     (501) staff       (20)       16 2023-06-22 03:43:29.000000 cryptography318-0.4.1/cryptography318.egg-info/top_level.txt
--rw-r--r--   0 andrew     (501) staff       (20)       38 2023-06-22 03:43:29.192646 cryptography318-0.4.1/setup.cfg
--rw-r--r--   0 andrew     (501) staff       (20)     1668 2022-09-09 15:43:03.000000 cryptography318-0.4.1/setup.py
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-22 03:47:31.335463 cryptography318-0.4.2/
+-rw-r--r--   0 andrew     (501) staff       (20)     1718 2023-06-22 03:47:31.335290 cryptography318-0.4.2/PKG-INFO
+-rw-r--r--   0 andrew     (501) staff       (20)     1128 2023-03-15 02:24:32.000000 cryptography318-0.4.2/README.md
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-22 03:47:31.331561 cryptography318-0.4.2/cryptography318/
+-rw-r--r--   0 andrew     (501) staff       (20)      987 2023-03-15 00:29:52.000000 cryptography318-0.4.2/cryptography318/__init__.py
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-22 03:47:31.332934 cryptography318-0.4.2/cryptography318/dlp/
+-rw-r--r--   0 andrew     (501) staff       (20)      150 2023-03-15 00:26:39.000000 cryptography318-0.4.2/cryptography318/dlp/__init__.py
+-rw-r--r--   0 andrew     (501) staff       (20)     5516 2023-03-15 01:53:10.000000 cryptography318-0.4.2/cryptography318/dlp/dlp.py
+-rw-r--r--   0 andrew     (501) staff       (20)     2901 2023-03-15 01:50:49.000000 cryptography318-0.4.2/cryptography318/dlp/icm.py
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-22 03:47:31.333818 cryptography318-0.4.2/cryptography318/factor/
+-rw-r--r--   0 andrew     (501) staff       (20)      370 2023-06-19 20:52:32.000000 cryptography318-0.4.2/cryptography318/factor/__init__.py
+-rw-r--r--   0 andrew     (501) staff       (20)    10578 2023-03-15 00:26:39.000000 cryptography318-0.4.2/cryptography318/factor/curve.py
+-rw-r--r--   0 andrew     (501) staff       (20)     8832 2023-03-15 00:26:39.000000 cryptography318-0.4.2/cryptography318/factor/elliptic.py
+-rw-r--r--   0 andrew     (501) staff       (20)     7006 2023-06-22 03:36:31.000000 cryptography318-0.4.2/cryptography318/factor/factor.py
+-rw-r--r--   0 andrew     (501) staff       (20)    10906 2023-06-22 03:47:16.000000 cryptography318-0.4.2/cryptography318/factor/siqs.py
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-22 03:47:31.334139 cryptography318-0.4.2/cryptography318/linalg/
+-rw-r--r--   0 andrew     (501) staff       (20)      117 2023-03-15 00:26:39.000000 cryptography318-0.4.2/cryptography318/linalg/__init__.py
+-rw-r--r--   0 andrew     (501) staff       (20)     7370 2023-03-15 00:27:38.000000 cryptography318-0.4.2/cryptography318/linalg/linalg.py
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-22 03:47:31.334675 cryptography318-0.4.2/cryptography318/prime/
+-rw-r--r--   0 andrew     (501) staff       (20)      478 2023-06-19 20:52:32.000000 cryptography318-0.4.2/cryptography318/prime/__init__.py
+-rw-r--r--   0 andrew     (501) staff       (20)     3531 2023-03-15 01:46:28.000000 cryptography318-0.4.2/cryptography318/prime/bailliepsw_helper.py
+-rw-r--r--   0 andrew     (501) staff       (20)    24741 2023-06-22 03:36:14.000000 cryptography318-0.4.2/cryptography318/prime/prime.py
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-22 03:47:31.335074 cryptography318-0.4.2/cryptography318/utils/
+-rw-r--r--   0 andrew     (501) staff       (20)       66 2022-03-18 04:48:41.000000 cryptography318-0.4.2/cryptography318/utils/__init__.py
+-rw-r--r--   0 andrew     (501) staff       (20)     3640 2023-06-19 20:19:13.000000 cryptography318-0.4.2/cryptography318/utils/utils.py
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-22 03:47:31.332420 cryptography318-0.4.2/cryptography318.egg-info/
+-rw-r--r--   0 andrew     (501) staff       (20)     1718 2023-06-22 03:47:31.000000 cryptography318-0.4.2/cryptography318.egg-info/PKG-INFO
+-rw-r--r--   0 andrew     (501) staff       (20)      733 2023-06-22 03:47:31.000000 cryptography318-0.4.2/cryptography318.egg-info/SOURCES.txt
+-rw-r--r--   0 andrew     (501) staff       (20)        1 2023-06-22 03:47:31.000000 cryptography318-0.4.2/cryptography318.egg-info/dependency_links.txt
+-rw-r--r--   0 andrew     (501) staff       (20)       26 2023-06-22 03:47:31.000000 cryptography318-0.4.2/cryptography318.egg-info/requires.txt
+-rw-r--r--   0 andrew     (501) staff       (20)       16 2023-06-22 03:47:31.000000 cryptography318-0.4.2/cryptography318.egg-info/top_level.txt
+-rw-r--r--   0 andrew     (501) staff       (20)       38 2023-06-22 03:47:31.335510 cryptography318-0.4.2/setup.cfg
+-rw-r--r--   0 andrew     (501) staff       (20)     1668 2022-09-09 15:43:03.000000 cryptography318-0.4.2/setup.py
```

### Comparing `cryptography318-0.4.1/PKG-INFO` & `cryptography318-0.4.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryptography318
-Version: 0.4.1
+Version: 0.4.2
 Summary: A set of functions useful in cryptography and linear algebra
 Home-page: https://github.com/aarpyy/Cryptography
 Author: Andrew Carpenter
 Author-email: andrewcarp00@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Education
 Classifier: License :: Public Domain
```

### Comparing `cryptography318-0.4.1/README.md` & `cryptography318-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `cryptography318-0.4.1/cryptography318/__init__.py` & `cryptography318-0.4.2/cryptography318/__init__.py`

 * *Files identical despite different names*

### Comparing `cryptography318-0.4.1/cryptography318/dlp/dlp.py` & `cryptography318-0.4.2/cryptography318/dlp/dlp.py`

 * *Files identical despite different names*

### Comparing `cryptography318-0.4.1/cryptography318/dlp/icm.py` & `cryptography318-0.4.2/cryptography318/dlp/icm.py`

 * *Files identical despite different names*

### Comparing `cryptography318-0.4.1/cryptography318/factor/curve.py` & `cryptography318-0.4.2/cryptography318/factor/curve.py`

 * *Files identical despite different names*

### Comparing `cryptography318-0.4.1/cryptography318/factor/elliptic.py` & `cryptography318-0.4.2/cryptography318/factor/elliptic.py`

 * *Files identical despite different names*

### Comparing `cryptography318-0.4.1/cryptography318/factor/factor.py` & `cryptography318-0.4.2/cryptography318/factor/factor.py`

 * *Files identical despite different names*

### Comparing `cryptography318-0.4.1/cryptography318/factor/siqs.py` & `cryptography318-0.4.2/cryptography318/factor/siqs.py`

 * *Files 2% similar despite different names*

```diff
@@ -222,17 +222,15 @@
 
     _b = a - b if b + b > a else b
 
     assert (_b * _b - n) % a == 0
 
     n_factors = len(a_factors)
     size_fb = len(factor_base)
-    B_ainv_2: list[list] = []
-    for _ in range(n_factors):
-        B_ainv_2.append([None] * size_fb)
+    B_ainv_2 = [[None] * size_fb for _ in range(n_factors)]     # type: list[list]
 
     for p in a_non_factors:
         prime = factor_base[p]
         a_inv = pow(a, -1, prime)
         for j in range(n_factors):
             B_ainv_2[j][p] = ((B[j] + B[j]) * a_inv) % prime
```

### Comparing `cryptography318-0.4.1/cryptography318/linalg/linalg.py` & `cryptography318-0.4.2/cryptography318/linalg/linalg.py`

 * *Files identical despite different names*

### Comparing `cryptography318-0.4.1/cryptography318/prime/bailliepsw_helper.py` & `cryptography318-0.4.2/cryptography318/prime/bailliepsw_helper.py`

 * *Files identical despite different names*

### Comparing `cryptography318-0.4.1/cryptography318/prime/prime.py` & `cryptography318-0.4.2/cryptography318/prime/prime.py`

 * *Files identical despite different names*

### Comparing `cryptography318-0.4.1/cryptography318/utils/utils.py` & `cryptography318-0.4.2/cryptography318/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cryptography318-0.4.1/cryptography318.egg-info/PKG-INFO` & `cryptography318-0.4.2/cryptography318.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryptography318
-Version: 0.4.1
+Version: 0.4.2
 Summary: A set of functions useful in cryptography and linear algebra
 Home-page: https://github.com/aarpyy/Cryptography
 Author: Andrew Carpenter
 Author-email: andrewcarp00@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Education
 Classifier: License :: Public Domain
```

### Comparing `cryptography318-0.4.1/cryptography318.egg-info/SOURCES.txt` & `cryptography318-0.4.2/cryptography318.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cryptography318-0.4.1/setup.py` & `cryptography318-0.4.2/setup.py`

 * *Files identical despite different names*

