# Comparing `tmp/drdid-1.1.4.tar.gz` & `tmp/drdid-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drdid-1.1.4.tar", last modified: Wed Jun 21 23:28:37 2023, max compression
+gzip compressed data, was "drdid-1.1.5.tar", last modified: Wed Jun 21 23:34:46 2023, max compression
```

## Comparing `drdid-1.1.4.tar` & `drdid-1.1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:28:37.460778 drdid-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-21 23:28:27.000000 drdid-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-21 23:28:37.460778 drdid-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-21 23:28:27.000000 drdid-1.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:28:37.460778 drdid-1.1.4/drdid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 23:28:27.000000 drdid-1.1.4/drdid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 23:28:27.000000 drdid-1.1.4/drdid/_version_.py
--rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-06-21 23:28:27.000000 drdid-1.1.4/drdid/drdid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-06-21 23:28:27.000000 drdid-1.1.4/drdid/ipwd_did.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-06-21 23:28:27.000000 drdid-1.1.4/drdid/reg_did.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-21 23:28:27.000000 drdid-1.1.4/drdid/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:28:37.460778 drdid-1.1.4/drdid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-21 23:28:37.000000 drdid-1.1.4/drdid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-21 23:28:37.000000 drdid-1.1.4/drdid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 23:28:37.000000 drdid-1.1.4/drdid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-21 23:28:37.000000 drdid-1.1.4/drdid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 23:28:37.000000 drdid-1.1.4/drdid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 23:28:37.460778 drdid-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-21 23:28:27.000000 drdid-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:34:46.046669 drdid-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-21 23:34:34.000000 drdid-1.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-21 23:34:46.046669 drdid-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-21 23:34:34.000000 drdid-1.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:34:46.046669 drdid-1.1.5/drdid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 23:34:34.000000 drdid-1.1.5/drdid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-21 23:34:34.000000 drdid-1.1.5/drdid/_version_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-06-21 23:34:34.000000 drdid-1.1.5/drdid/drdid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-06-21 23:34:34.000000 drdid-1.1.5/drdid/ipwd_did.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-06-21 23:34:34.000000 drdid-1.1.5/drdid/reg_did.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-21 23:34:34.000000 drdid-1.1.5/drdid/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:34:46.046669 drdid-1.1.5/drdid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-21 23:34:45.000000 drdid-1.1.5/drdid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-21 23:34:46.000000 drdid-1.1.5/drdid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 23:34:45.000000 drdid-1.1.5/drdid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-21 23:34:45.000000 drdid-1.1.5/drdid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 23:34:45.000000 drdid-1.1.5/drdid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 23:34:46.046669 drdid-1.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-21 23:34:34.000000 drdid-1.1.5/setup.py
```

### Comparing `drdid-1.1.4/LICENSE` & `drdid-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `drdid-1.1.4/drdid/drdid.py` & `drdid-1.1.5/drdid/drdid.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     if np.all(covariates[:, 0] == int_cov):
       int_cov = covariates
     else:
       int_cov = np.concatenate((np.ones((n, 1)), covariates), axis=1)
   pscore_tr = glm(D, int_cov, family=binomial, freq_weights=i_weights)\
     .fit()
 
-  _, w_cont_pre, _,\
+  ps_fit, w_cont_pre, _,\
     w_cont_post, _, asy_lin_rep_ps = fit_ps(D, int_cov, i_weights, post)
   
   def reg_out_y(d, p, y = y, int_cov = int_cov, wg = i_weights):
     rows_ = (D == d) & (post == p)
     reg_cont = lm(y[rows_], int_cov[rows_], weights=wg[rows_])\
       .fit().params
     out_y = np.dot(reg_cont, int_cov.T)
@@ -218,8 +218,8 @@
   dr_att_inf_func = inf_treat - inf_control
 
   if not boot:
     se_att = np.std(dr_att_inf_func) / np.sqrt(n)
 
   return (dr_att, dr_att_inf_func, se_att)
 
-  
+
```

### Comparing `drdid-1.1.4/drdid/ipwd_did.py` & `drdid-1.1.5/drdid/ipwd_did.py`

 * *Files identical despite different names*

### Comparing `drdid-1.1.4/drdid/reg_did.py` & `drdid-1.1.5/drdid/reg_did.py`

 * *Files identical despite different names*

### Comparing `drdid-1.1.4/drdid/utils.py` & `drdid-1.1.5/drdid/utils.py`

 * *Files identical despite different names*

### Comparing `drdid-1.1.4/setup.py` & `drdid-1.1.5/setup.py`

 * *Files identical despite different names*

