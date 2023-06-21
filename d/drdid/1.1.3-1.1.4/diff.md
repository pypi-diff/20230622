# Comparing `tmp/drdid-1.1.3.tar.gz` & `tmp/drdid-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drdid-1.1.3.tar", last modified: Wed Jun 21 23:05:14 2023, max compression
+gzip compressed data, was "drdid-1.1.4.tar", last modified: Wed Jun 21 23:28:37 2023, max compression
```

## Comparing `drdid-1.1.3.tar` & `drdid-1.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:05:14.770010 drdid-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-21 23:05:06.000000 drdid-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-21 23:05:14.770010 drdid-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-21 23:05:06.000000 drdid-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:05:14.766009 drdid-1.1.3/drdid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 23:05:06.000000 drdid-1.1.3/drdid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 23:05:06.000000 drdid-1.1.3/drdid/_version_.py
--rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-06-21 23:05:06.000000 drdid-1.1.3/drdid/drdid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-06-21 23:05:06.000000 drdid-1.1.3/drdid/ipwd_did.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-06-21 23:05:06.000000 drdid-1.1.3/drdid/reg_did.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-21 23:05:06.000000 drdid-1.1.3/drdid/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:05:14.770010 drdid-1.1.3/drdid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-21 23:05:14.000000 drdid-1.1.3/drdid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-21 23:05:14.000000 drdid-1.1.3/drdid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 23:05:14.000000 drdid-1.1.3/drdid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-21 23:05:14.000000 drdid-1.1.3/drdid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 23:05:14.000000 drdid-1.1.3/drdid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 23:05:14.770010 drdid-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-21 23:05:06.000000 drdid-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:28:37.460778 drdid-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-21 23:28:27.000000 drdid-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-21 23:28:37.460778 drdid-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-21 23:28:27.000000 drdid-1.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:28:37.460778 drdid-1.1.4/drdid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 23:28:27.000000 drdid-1.1.4/drdid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 23:28:27.000000 drdid-1.1.4/drdid/_version_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-06-21 23:28:27.000000 drdid-1.1.4/drdid/drdid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-06-21 23:28:27.000000 drdid-1.1.4/drdid/ipwd_did.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-06-21 23:28:27.000000 drdid-1.1.4/drdid/reg_did.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-21 23:28:27.000000 drdid-1.1.4/drdid/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:28:37.460778 drdid-1.1.4/drdid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-21 23:28:37.000000 drdid-1.1.4/drdid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-21 23:28:37.000000 drdid-1.1.4/drdid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 23:28:37.000000 drdid-1.1.4/drdid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-21 23:28:37.000000 drdid-1.1.4/drdid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 23:28:37.000000 drdid-1.1.4/drdid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 23:28:37.460778 drdid-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-21 23:28:27.000000 drdid-1.1.4/setup.py
```

### Comparing `drdid-1.1.3/LICENSE` & `drdid-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `drdid-1.1.3/drdid/drdid.py` & `drdid-1.1.4/drdid/drdid.py`

 * *Files identical despite different names*

### Comparing `drdid-1.1.3/drdid/ipwd_did.py` & `drdid-1.1.4/drdid/ipwd_did.py`

 * *Files identical despite different names*

### Comparing `drdid-1.1.3/drdid/reg_did.py` & `drdid-1.1.4/drdid/reg_did.py`

 * *Files identical despite different names*

### Comparing `drdid-1.1.3/drdid/utils.py` & `drdid-1.1.4/drdid/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,8 +87,8 @@
 
   w_ps = w * (d - ps_fit)
   score_ps = w_ps[:, n_x] * x
   hessian = glm_fit.cov_params() * n
 
   asy_lin_ps = np.dot(score_ps, hessian)
 
-  return (ps_fit, w_cont_pre, w_cont, w_cont_post, asy_lin_ps)
+  return (ps_fit, w_cont_pre, w_cont, w_cont_post, 0, asy_lin_ps)
```

### Comparing `drdid-1.1.3/setup.py` & `drdid-1.1.4/setup.py`

 * *Files identical despite different names*

