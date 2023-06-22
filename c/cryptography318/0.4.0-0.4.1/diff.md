# Comparing `tmp/cryptography318-0.4.0.tar.gz` & `tmp/cryptography318-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptography318-0.4.0.tar", last modified: Mon Jun 19 21:14:12 2023, max compression
+gzip compressed data, was "cryptography318-0.4.1.tar", last modified: Thu Jun 22 03:43:29 2023, max compression
```

## Comparing `cryptography318-0.4.0.tar` & `cryptography318-0.4.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-19 21:14:12.624491 cryptography318-0.4.0/
--rw-r--r--   0 andrew     (501) staff       (20)     1718 2023-06-19 21:14:12.624350 cryptography318-0.4.0/PKG-INFO
--rw-r--r--   0 andrew     (501) staff       (20)     1128 2023-03-15 02:24:32.000000 cryptography318-0.4.0/README.md
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-19 21:14:12.621548 cryptography318-0.4.0/cryptography318/
--rw-r--r--   0 andrew     (501) staff       (20)      987 2023-03-15 00:29:52.000000 cryptography318-0.4.0/cryptography318/__init__.py
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-19 21:14:12.622498 cryptography318-0.4.0/cryptography318/dlp/
--rw-r--r--   0 andrew     (501) staff       (20)      150 2023-03-15 00:26:39.000000 cryptography318-0.4.0/cryptography318/dlp/__init__.py
--rw-r--r--   0 andrew     (501) staff       (20)     5516 2023-03-15 01:53:10.000000 cryptography318-0.4.0/cryptography318/dlp/dlp.py
--rw-r--r--   0 andrew     (501) staff       (20)     2901 2023-03-15 01:50:49.000000 cryptography318-0.4.0/cryptography318/dlp/icm.py
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-19 21:14:12.623079 cryptography318-0.4.0/cryptography318/factor/
--rw-r--r--   0 andrew     (501) staff       (20)      370 2023-06-19 20:52:32.000000 cryptography318-0.4.0/cryptography318/factor/__init__.py
--rw-r--r--   0 andrew     (501) staff       (20)    10578 2023-03-15 00:26:39.000000 cryptography318-0.4.0/cryptography318/factor/curve.py
--rw-r--r--   0 andrew     (501) staff       (20)     8832 2023-03-15 00:26:39.000000 cryptography318-0.4.0/cryptography318/factor/elliptic.py
--rw-r--r--   0 andrew     (501) staff       (20)     7009 2023-06-19 20:52:32.000000 cryptography318-0.4.0/cryptography318/factor/factor.py
--rw-r--r--   0 andrew     (501) staff       (20)    10914 2023-03-15 02:17:46.000000 cryptography318-0.4.0/cryptography318/factor/siqs.py
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-19 21:14:12.623324 cryptography318-0.4.0/cryptography318/linalg/
--rw-r--r--   0 andrew     (501) staff       (20)      117 2023-03-15 00:26:39.000000 cryptography318-0.4.0/cryptography318/linalg/__init__.py
--rw-r--r--   0 andrew     (501) staff       (20)     7370 2023-03-15 00:27:38.000000 cryptography318-0.4.0/cryptography318/linalg/linalg.py
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-19 21:14:12.623776 cryptography318-0.4.0/cryptography318/prime/
--rw-r--r--   0 andrew     (501) staff       (20)      478 2023-06-19 20:52:32.000000 cryptography318-0.4.0/cryptography318/prime/__init__.py
--rw-r--r--   0 andrew     (501) staff       (20)     3531 2023-03-15 01:46:28.000000 cryptography318-0.4.0/cryptography318/prime/bailliepsw_helper.py
--rw-r--r--   0 andrew     (501) staff       (20)    24675 2023-06-19 20:52:32.000000 cryptography318-0.4.0/cryptography318/prime/prime.py
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-19 21:14:12.624166 cryptography318-0.4.0/cryptography318/utils/
--rw-r--r--   0 andrew     (501) staff       (20)       66 2022-03-18 04:48:41.000000 cryptography318-0.4.0/cryptography318/utils/__init__.py
--rw-r--r--   0 andrew     (501) staff       (20)     3640 2023-06-19 20:19:13.000000 cryptography318-0.4.0/cryptography318/utils/utils.py
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-19 21:14:12.622170 cryptography318-0.4.0/cryptography318.egg-info/
--rw-r--r--   0 andrew     (501) staff       (20)     1718 2023-06-19 21:14:12.000000 cryptography318-0.4.0/cryptography318.egg-info/PKG-INFO
--rw-r--r--   0 andrew     (501) staff       (20)      733 2023-06-19 21:14:12.000000 cryptography318-0.4.0/cryptography318.egg-info/SOURCES.txt
--rw-r--r--   0 andrew     (501) staff       (20)        1 2023-06-19 21:14:12.000000 cryptography318-0.4.0/cryptography318.egg-info/dependency_links.txt
--rw-r--r--   0 andrew     (501) staff       (20)       26 2023-06-19 21:14:12.000000 cryptography318-0.4.0/cryptography318.egg-info/requires.txt
--rw-r--r--   0 andrew     (501) staff       (20)       16 2023-06-19 21:14:12.000000 cryptography318-0.4.0/cryptography318.egg-info/top_level.txt
--rw-r--r--   0 andrew     (501) staff       (20)       38 2023-06-19 21:14:12.624534 cryptography318-0.4.0/setup.cfg
--rw-r--r--   0 andrew     (501) staff       (20)     1668 2022-09-09 15:43:03.000000 cryptography318-0.4.0/setup.py
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-22 03:43:29.192597 cryptography318-0.4.1/
+-rw-r--r--   0 andrew     (501) staff       (20)     1718 2023-06-22 03:43:29.192433 cryptography318-0.4.1/PKG-INFO
+-rw-r--r--   0 andrew     (501) staff       (20)     1128 2023-03-15 02:24:32.000000 cryptography318-0.4.1/README.md
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-22 03:43:29.186820 cryptography318-0.4.1/cryptography318/
+-rw-r--r--   0 andrew     (501) staff       (20)      987 2023-03-15 00:29:52.000000 cryptography318-0.4.1/cryptography318/__init__.py
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-22 03:43:29.188674 cryptography318-0.4.1/cryptography318/dlp/
+-rw-r--r--   0 andrew     (501) staff       (20)      150 2023-03-15 00:26:39.000000 cryptography318-0.4.1/cryptography318/dlp/__init__.py
+-rw-r--r--   0 andrew     (501) staff       (20)     5516 2023-03-15 01:53:10.000000 cryptography318-0.4.1/cryptography318/dlp/dlp.py
+-rw-r--r--   0 andrew     (501) staff       (20)     2901 2023-03-15 01:50:49.000000 cryptography318-0.4.1/cryptography318/dlp/icm.py
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-22 03:43:29.190171 cryptography318-0.4.1/cryptography318/factor/
+-rw-r--r--   0 andrew     (501) staff       (20)      370 2023-06-19 20:52:32.000000 cryptography318-0.4.1/cryptography318/factor/__init__.py
+-rw-r--r--   0 andrew     (501) staff       (20)    10578 2023-03-15 00:26:39.000000 cryptography318-0.4.1/cryptography318/factor/curve.py
+-rw-r--r--   0 andrew     (501) staff       (20)     8832 2023-03-15 00:26:39.000000 cryptography318-0.4.1/cryptography318/factor/elliptic.py
+-rw-r--r--   0 andrew     (501) staff       (20)     7006 2023-06-22 03:36:31.000000 cryptography318-0.4.1/cryptography318/factor/factor.py
+-rw-r--r--   0 andrew     (501) staff       (20)    10926 2023-06-22 03:42:30.000000 cryptography318-0.4.1/cryptography318/factor/siqs.py
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-22 03:43:29.190663 cryptography318-0.4.1/cryptography318/linalg/
+-rw-r--r--   0 andrew     (501) staff       (20)      117 2023-03-15 00:26:39.000000 cryptography318-0.4.1/cryptography318/linalg/__init__.py
+-rw-r--r--   0 andrew     (501) staff       (20)     7370 2023-03-15 00:27:38.000000 cryptography318-0.4.1/cryptography318/linalg/linalg.py
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-22 03:43:29.191504 cryptography318-0.4.1/cryptography318/prime/
+-rw-r--r--   0 andrew     (501) staff       (20)      478 2023-06-19 20:52:32.000000 cryptography318-0.4.1/cryptography318/prime/__init__.py
+-rw-r--r--   0 andrew     (501) staff       (20)     3531 2023-03-15 01:46:28.000000 cryptography318-0.4.1/cryptography318/prime/bailliepsw_helper.py
+-rw-r--r--   0 andrew     (501) staff       (20)    24741 2023-06-22 03:36:14.000000 cryptography318-0.4.1/cryptography318/prime/prime.py
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-22 03:43:29.192098 cryptography318-0.4.1/cryptography318/utils/
+-rw-r--r--   0 andrew     (501) staff       (20)       66 2022-03-18 04:48:41.000000 cryptography318-0.4.1/cryptography318/utils/__init__.py
+-rw-r--r--   0 andrew     (501) staff       (20)     3640 2023-06-19 20:19:13.000000 cryptography318-0.4.1/cryptography318/utils/utils.py
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2023-06-22 03:43:29.187861 cryptography318-0.4.1/cryptography318.egg-info/
+-rw-r--r--   0 andrew     (501) staff       (20)     1718 2023-06-22 03:43:29.000000 cryptography318-0.4.1/cryptography318.egg-info/PKG-INFO
+-rw-r--r--   0 andrew     (501) staff       (20)      733 2023-06-22 03:43:29.000000 cryptography318-0.4.1/cryptography318.egg-info/SOURCES.txt
+-rw-r--r--   0 andrew     (501) staff       (20)        1 2023-06-22 03:43:29.000000 cryptography318-0.4.1/cryptography318.egg-info/dependency_links.txt
+-rw-r--r--   0 andrew     (501) staff       (20)       26 2023-06-22 03:43:29.000000 cryptography318-0.4.1/cryptography318.egg-info/requires.txt
+-rw-r--r--   0 andrew     (501) staff       (20)       16 2023-06-22 03:43:29.000000 cryptography318-0.4.1/cryptography318.egg-info/top_level.txt
+-rw-r--r--   0 andrew     (501) staff       (20)       38 2023-06-22 03:43:29.192646 cryptography318-0.4.1/setup.cfg
+-rw-r--r--   0 andrew     (501) staff       (20)     1668 2022-09-09 15:43:03.000000 cryptography318-0.4.1/setup.py
```

### Comparing `cryptography318-0.4.0/PKG-INFO` & `cryptography318-0.4.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryptography318
-Version: 0.4.0
+Version: 0.4.1
 Summary: A set of functions useful in cryptography and linear algebra
 Home-page: https://github.com/aarpyy/Cryptography
 Author: Andrew Carpenter
 Author-email: andrewcarp00@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Education
 Classifier: License :: Public Domain
```

### Comparing `cryptography318-0.4.0/README.md` & `cryptography318-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `cryptography318-0.4.0/cryptography318/__init__.py` & `cryptography318-0.4.1/cryptography318/__init__.py`

 * *Files identical despite different names*

### Comparing `cryptography318-0.4.0/cryptography318/dlp/dlp.py` & `cryptography318-0.4.1/cryptography318/dlp/dlp.py`

 * *Files identical despite different names*

### Comparing `cryptography318-0.4.0/cryptography318/dlp/icm.py` & `cryptography318-0.4.1/cryptography318/dlp/icm.py`

 * *Files identical despite different names*

### Comparing `cryptography318-0.4.0/cryptography318/factor/curve.py` & `cryptography318-0.4.1/cryptography318/factor/curve.py`

 * *Files identical despite different names*

### Comparing `cryptography318-0.4.0/cryptography318/factor/elliptic.py` & `cryptography318-0.4.1/cryptography318/factor/elliptic.py`

 * *Files identical despite different names*

### Comparing `cryptography318-0.4.0/cryptography318/factor/factor.py` & `cryptography318-0.4.1/cryptography318/factor/factor.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import os
 from math import gcd, log, sqrt
 from random import randrange
+from typing import Any
 
 from cryptography318.factor import lenstra_ecm
 from cryptography318.factor import siqs
 from cryptography318.prime.prime import isprime, next_prime, primesieve
-from cryptography318.utils.utils import Details
 
-factor_details = Details(**{
+__factor_details: dict[str, Any] = {
     "Pollard's Rho": None,
     "ECM": None,
     "Pollard's P-1": None,
     "Quadratic Sieve": None,
-    "Direct": None
-})
+    "Trial Division": None
+}
 
 
 def get_details():
-    global factor_details
-    return str(factor_details)
+    global __factor_details
+    return __factor_details
 
 
 def factor(n, rho=True, ecm=True, p1=True, qs=True, limit=None, *, details=False):
     """
     Attempts to factor given integer with four methods, returning None if un-factorable.
     Function first checks if number is prime then finds all small factors if any exist.
     Then (assuming no specific methods were set to False) Pollard's Rho, Lenstra's ECM,
@@ -36,73 +36,74 @@
     :param ecm: bool determining if Lenstra's ECM algorithm should be used
     :param p1: bool determining if Pollard's P-1 algorithm should be used
     :param qs: bool determining if Quadratic Sieve algorithm should be used
     :param limit: integer limit of factors to be found using small_factors()
     :param details: bool determining if factor details should be updated
     :return: dictionary of all primes factors and their powers, or None if not factorable
     """
-    global factor_details
+    global __factor_details
     if details:
-        factor_details.clear_details()
+        for key, value in __factor_details.items():
+            __factor_details[key] = None
 
     if n == 1:
         if details:
-            factor_details.add_details("Direct", True)
+            __factor_details["Trial Division"] = True
         return {}
     elif isprime(n):
         if details:
-            factor_details.add_details("Direct", True)
+            __factor_details["Trial Division"] = True
         return {n: 1}
 
     if limit is None:
         limit = 32768
 
     factors = {}
-    k, p = factor_small(factors, n, limit)
+    k, _ = factor_small(factors, n, limit)
     # If we factored it completely with small factors, return factors
     if k == 1:
         if details:
-            factor_details.add_details("Direct", True)
+            __factor_details["Trial Division"] = True
         return factors
     # If we factored it partially with small factors, recursively factor the rest
     elif k != n:
+        if details:
+            __factor_details["Trial Division"] = True
         # If remaining factor is prime, we are done factoring
         if isprime(k):
             factors[k] = factors.get(k, 0) + 1
-            if details:
-                factor_details.add_details("Direct", True)
             return factors
         n = k
 
     factor_kwargs = {"rho": rho, "ecm": ecm, "p1": p1, "qs": qs, "limit": limit}
 
     if rho:
         if details:
-            factor_details.add_details("Pollard's Rho", True)
+            __factor_details["Pollard's Rho"] = True
         n = _factor_further(n, pollard_rho_factor(n), factors, **factor_kwargs)
         if n == 1:
             return factors
 
     if ecm:
         if details:
-            factor_details.add_details("ECM", True)
+            __factor_details["ECM"] = True
         n = _factor_further(n, lenstra_ecm(n), factors, **factor_kwargs)
         if n == 1:
             return factors
 
     if p1:
         if details:
-            factor_details.add_details("Pollard's P-1", True)
+            __factor_details["Pollard's P-1"] = True
         n = _factor_further(n, pollard_p1(n), factors, **factor_kwargs)
         if n == 1:
             return factors
 
     if qs:
         if details:
-            factor_details.add_details("Quadratic Sieve", True)
+            __factor_details["Quadratic Sieve"] = True
 
         # Use local primes.txt if we can find it, otherwise don't use a file (slow)
         fp = "primes.txt" if os.path.exists("../prime/primes.txt") else None
 
         # Nothing left after quadratic sieve, so just return factors
         n = _factor_further(n, siqs(n, fp=fp, loud=False), factors, **factor_kwargs)
         if n != 1:
```

### Comparing `cryptography318-0.4.0/cryptography318/factor/siqs.py` & `cryptography318-0.4.1/cryptography318/factor/siqs.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,15 +222,15 @@
 
     _b = a - b if b + b > a else b
 
     assert (_b * _b - n) % a == 0
 
     n_factors = len(a_factors)
     size_fb = len(factor_base)
-    B_ainv_2 = []
+    B_ainv_2: list[list] = []
     for _ in range(n_factors):
         B_ainv_2.append([None] * size_fb)
 
     for p in a_non_factors:
         prime = factor_base[p]
         a_inv = pow(a, -1, prime)
         for j in range(n_factors):
```

### Comparing `cryptography318-0.4.0/cryptography318/linalg/linalg.py` & `cryptography318-0.4.1/cryptography318/linalg/linalg.py`

 * *Files identical despite different names*

### Comparing `cryptography318-0.4.0/cryptography318/prime/bailliepsw_helper.py` & `cryptography318-0.4.1/cryptography318/prime/bailliepsw_helper.py`

 * *Files identical despite different names*

### Comparing `cryptography318-0.4.0/cryptography318/prime/prime.py` & `cryptography318-0.4.1/cryptography318/prime/prime.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from collections import UserList
 from itertools import islice
 from math import isqrt, prod
 from pathlib import Path
 from random import choice, randrange
+from typing import Any
 
 from cryptography318.prime.bailliepsw_helper import D_chooser, LucasPseudoPrime
-from cryptography318.utils.utils import binary_search, Details
+from cryptography318.utils.utils import binary_search
 
-
-isprime_details = Details(**{
+__isprime_details: dict[str, Any] = {
     "Miller-Rabin": None,
     "Baillie-PSW": None,
-    "Direct": None,
-})
+    "Trial Division": None,
+}
 
 
 def get_details():
-    global isprime_details
-    return str(isprime_details)
+    global __isprime_details
+    return __isprime_details
 
 
 class Sieve(UserList[int]):
     """
     Unbound list of primes starting at 2. Object is iterable, index-able, print-able, searchable,
     and extendable. Unless another specific use is required, import primesieve object as a global
     variable for use. Intended to help with primality tests and factoring integers.
@@ -296,16 +296,16 @@
     while not d & 1:
         r += 1
         d >>= 1
 
     for _ in range(k):
         if not _mr_test(d, n):
             if details:
-                global isprime_details
-                isprime_details.add_details("Miller-Rabin", f"{d} is a witness to {n}'s composite-ness")
+                global __isprime_details
+                __isprime_details["Miller-Rabin"] = f"{d} is a witness to {n}'s composite-ness"
             return False
 
     return True
 
 
 def _mr_test(d, n):
     """Helper function for miller_rabin which uses previously found d to
@@ -358,23 +358,23 @@
 
     return False
 
 
 def miller_rabin_bases(bases, n, *, details=False):
     """Helper function that allows for a list of witnesses to be tested
     using MillerRabin_base_a function"""
-    global isprime_details
+    global __isprime_details
 
     for a in bases:
         if not _miller_rabin_base_a(a, n):
             if details:
-                isprime_details.add_details("Miller-Rabin", f"{a} is witness to {n}'s compositeness")
+                __isprime_details["Miller-Rabin"] = f"{a} is witness to {n}'s compositeness"
             return False
     if details:
-        isprime_details.add_details("Miller-Rabin", f"{n} is probably prime")
+        __isprime_details["Miller-Rabin"] = f"{n} is probably prime"
     return True
 
 
 def baillie_psw(n, mr=True):
     """
     Perform the Baillie-PSW probabilistic primality test on candidate.
 
@@ -431,46 +431,47 @@
     candidate is prime for n < 3317044064679887385961981. For all larger n,
     there is no  known set of bases that makes the MR test deterministic. Thus, a
     SPRP-test consisting of a Strong Lucas Pseudo-prime test and a Miller-Rabin
     test with 20 random bases `a`, s.t. 1 < a < n is used to determine if candidate is
     probably prime.
     """
 
-    global isprime_details
+    global __isprime_details
     if details:
-        isprime_details.clear_details()
+        for key in __isprime_details:
+            __isprime_details[key] = None
 
     if n < 2:
         if details:
-            isprime_details.add_details("Direct", f"{n} < 2")
+            __isprime_details["Trial Division"] = f"{n} < 2"
         return False
 
     elif n < 10:
         if details:
-            isprime_details.add_details("Direct", f"{n} < 10")
+            __isprime_details["Trial Division"] = f"{n} < 10"
         return bool([0, 0, 1, 1, 0, 1, 0, 1, 0, 0, 0][n])
 
     # check for odds
     elif not n & 1:
         if details:
-            isprime_details.add_details("Direct", f"{n} is even")
+            __isprime_details["Trial Division"] = f"{n} is even"
         return False
 
     # check for all other instances n != 6k +/- 1
     elif not n % 3:
         if details:
-            isprime_details.add_details("Direct", f"{n} is divisible by 3")
+            __isprime_details["Trial Division"] = f"{n} is divisible by 3"
         return False
 
     # This step is pretty useless unless primesieve is being used for something else or is
     # being purposefully generated, since it is constructed only with first 6 primes
     global primesieve
     if n in primesieve:
         if details:
-            isprime_details.add_details("Direct", f"{n} is known prime")
+            __isprime_details["Trial Division"] = f"{n} is known prime"
         return True
     elif n < 2047:
         return miller_rabin_bases([2], n, details=details)
     elif n < 1373653:
         return miller_rabin_bases([2, 3], n, details=details)
     elif n < 9080191:
         return miller_rabin_bases([31, 73], n, details=details)
@@ -481,29 +482,30 @@
     elif n < 4759123141:
         return miller_rabin_bases([2, 7, 61], n, details=details)
     elif n < 1122004669633:
         return miller_rabin_bases([2, 13, 23, 1662803], n, details=details)
     elif n < 55245642489451:
         return miller_rabin_bases([2, 141889084524735, 1199124725622454117, 11096072698276303650], n, details=details)
     elif n < 7999252175582851:
-        return miller_rabin_bases([2, 4130806001517, 149795463772692060, 186635894390467037, 3967304179347715805], n, details=details)
+        return miller_rabin_bases([2, 4130806001517, 149795463772692060, 186635894390467037, 3967304179347715805], n,
+                                  details=details)
     elif n < 18446744073709551616:
         return miller_rabin_bases([2, 325, 9375, 28178, 450775, 9780504, 1795265022], n, details=details)
     elif n < 318665857834031151167461:
         return miller_rabin_bases([2, 3, 5, 7, 11, 13, 17, 19, 23, 29, 31, 37], n, details=details)
     elif n < 3317044064679887385961981:
         return miller_rabin_bases([2, 3, 5, 7, 11, 13, 17, 19, 23, 29, 31, 37, 41], n, details=details)
     else:
         res = miller_rabin(n, k=40, details=details)
         if not res:
             return False
 
         # If miller rabin didn't say it was composite, then we should note that we used Baillie-PSW
         if details:
-            isprime_details.add_details("Baillie-PSW", True)
+            __isprime_details["Baillie-PSW"] = True
         return baillie_psw(n, mr=False)
 
 
 def randprime(a: int, b: int = None):
     """Uses combination of Miller-Rabin and Baillie-PSW primality tests to generate random prime
 
     Note
```

### Comparing `cryptography318-0.4.0/cryptography318/utils/utils.py` & `cryptography318-0.4.1/cryptography318/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cryptography318-0.4.0/cryptography318.egg-info/PKG-INFO` & `cryptography318-0.4.1/cryptography318.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryptography318
-Version: 0.4.0
+Version: 0.4.1
 Summary: A set of functions useful in cryptography and linear algebra
 Home-page: https://github.com/aarpyy/Cryptography
 Author: Andrew Carpenter
 Author-email: andrewcarp00@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Education
 Classifier: License :: Public Domain
```

### Comparing `cryptography318-0.4.0/cryptography318.egg-info/SOURCES.txt` & `cryptography318-0.4.1/cryptography318.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cryptography318-0.4.0/setup.py` & `cryptography318-0.4.1/setup.py`

 * *Files identical despite different names*

