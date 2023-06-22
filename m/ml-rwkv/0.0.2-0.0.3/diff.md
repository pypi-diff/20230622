# Comparing `tmp/ml-rwkv-0.0.2.tar.gz` & `tmp/ml-rwkv-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-rwkv-0.0.2.tar", last modified: Wed Jun 21 19:27:35 2023, max compression
+gzip compressed data, was "ml-rwkv-0.0.3.tar", last modified: Thu Jun 22 04:49:19 2023, max compression
```

## Comparing `ml-rwkv-0.0.2.tar` & `ml-rwkv-0.0.3.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:27:35.292059 ml-rwkv-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-21 19:27:22.000000 ml-rwkv-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-21 19:27:22.000000 ml-rwkv-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-21 19:27:35.292059 ml-rwkv-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-21 19:27:22.000000 ml-rwkv-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:27:35.288059 ml-rwkv-0.0.2/ml_rwkv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-21 19:27:35.000000 ml-rwkv-0.0.2/ml_rwkv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-21 19:27:35.000000 ml-rwkv-0.0.2/ml_rwkv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 19:27:35.000000 ml-rwkv-0.0.2/ml_rwkv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-21 19:27:35.000000 ml-rwkv-0.0.2/ml_rwkv.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-21 19:27:35.000000 ml-rwkv-0.0.2/ml_rwkv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-21 19:27:35.000000 ml-rwkv-0.0.2/ml_rwkv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-21 19:27:22.000000 ml-rwkv-0.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:27:35.288059 ml-rwkv-0.0.2/rwkv/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 19:27:22.000000 ml-rwkv-0.0.2/rwkv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13227 2023-06-21 19:27:22.000000 ml-rwkv-0.0.2/rwkv/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-06-21 19:27:22.000000 ml-rwkv-0.0.2/rwkv/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:27:35.288059 ml-rwkv-0.0.2/rwkv/triton/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 19:27:22.000000 ml-rwkv-0.0.2/rwkv/triton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-21 19:27:22.000000 ml-rwkv-0.0.2/rwkv/triton/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:27:35.288059 ml-rwkv-0.0.2/rwkv/triton/wkv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 19:27:22.000000 ml-rwkv-0.0.2/rwkv/triton/wkv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11492 2023-06-21 19:27:22.000000 ml-rwkv-0.0.2/rwkv/triton/wkv/vanilla.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:27:35.288059 ml-rwkv-0.0.2/rwkv/wkv/
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-06-21 19:27:22.000000 ml-rwkv-0.0.2/rwkv/wkv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-06-21 19:27:22.000000 ml-rwkv-0.0.2/rwkv/wkv/eps.py
--rw-r--r--   0 runner    (1001) docker     (123)     7658 2023-06-21 19:27:22.000000 ml-rwkv-0.0.2/rwkv/wkv/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-06-21 19:27:22.000000 ml-rwkv-0.0.2/rwkv/wkv/vanilla.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-21 19:27:35.292059 ml-rwkv-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-21 19:27:22.000000 ml-rwkv-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:27:35.292059 ml-rwkv-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-06-21 19:27:22.000000 ml-rwkv-0.0.2/tests/test_eps_wkv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-21 19:27:22.000000 ml-rwkv-0.0.2/tests/test_log_wkv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-06-21 19:27:22.000000 ml-rwkv-0.0.2/tests/test_vanilla_wkv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-06-21 19:27:22.000000 ml-rwkv-0.0.2/tests/test_wkv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 04:49:19.699888 ml-rwkv-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-22 04:49:08.000000 ml-rwkv-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-22 04:49:08.000000 ml-rwkv-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-22 04:49:19.699888 ml-rwkv-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-22 04:49:08.000000 ml-rwkv-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 04:49:19.699888 ml-rwkv-0.0.3/ml_rwkv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-22 04:49:19.000000 ml-rwkv-0.0.3/ml_rwkv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-22 04:49:19.000000 ml-rwkv-0.0.3/ml_rwkv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 04:49:19.000000 ml-rwkv-0.0.3/ml_rwkv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-22 04:49:19.000000 ml-rwkv-0.0.3/ml_rwkv.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-22 04:49:19.000000 ml-rwkv-0.0.3/ml_rwkv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-22 04:49:19.000000 ml-rwkv-0.0.3/ml_rwkv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-22 04:49:08.000000 ml-rwkv-0.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 04:49:19.699888 ml-rwkv-0.0.3/rwkv/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-22 04:49:08.000000 ml-rwkv-0.0.3/rwkv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13227 2023-06-22 04:49:08.000000 ml-rwkv-0.0.3/rwkv/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-06-22 04:49:08.000000 ml-rwkv-0.0.3/rwkv/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 04:49:19.699888 ml-rwkv-0.0.3/rwkv/triton/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 04:49:08.000000 ml-rwkv-0.0.3/rwkv/triton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-22 04:49:08.000000 ml-rwkv-0.0.3/rwkv/triton/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 04:49:19.699888 ml-rwkv-0.0.3/rwkv/triton/wkv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 04:49:08.000000 ml-rwkv-0.0.3/rwkv/triton/wkv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13151 2023-06-22 04:49:08.000000 ml-rwkv-0.0.3/rwkv/triton/wkv/eps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14820 2023-06-22 04:49:08.000000 ml-rwkv-0.0.3/rwkv/triton/wkv/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-06-22 04:49:08.000000 ml-rwkv-0.0.3/rwkv/triton/wkv/vanilla.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 04:49:19.699888 ml-rwkv-0.0.3/rwkv/wkv/
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-06-22 04:49:08.000000 ml-rwkv-0.0.3/rwkv/wkv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-06-22 04:49:08.000000 ml-rwkv-0.0.3/rwkv/wkv/eps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-06-22 04:49:08.000000 ml-rwkv-0.0.3/rwkv/wkv/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-06-22 04:49:08.000000 ml-rwkv-0.0.3/rwkv/wkv/vanilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-22 04:49:19.703888 ml-rwkv-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-22 04:49:08.000000 ml-rwkv-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 04:49:19.699888 ml-rwkv-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-06-22 04:49:08.000000 ml-rwkv-0.0.3/tests/test_eps_wkv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-06-22 04:49:08.000000 ml-rwkv-0.0.3/tests/test_log_wkv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-06-22 04:49:08.000000 ml-rwkv-0.0.3/tests/test_vanilla_wkv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-06-22 04:49:08.000000 ml-rwkv-0.0.3/tests/test_wkv.py
```

### Comparing `ml-rwkv-0.0.2/LICENSE` & `ml-rwkv-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-rwkv-0.0.2/PKG-INFO` & `ml-rwkv-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-rwkv
-Version: 0.0.2
+Version: 0.0.3
 Summary: RWKV implementation that is friendly with `ml-starter`
 Home-page: https://github.com/codekansas/rwkv
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-rwkv-0.0.2/README.md` & `ml-rwkv-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ml-rwkv-0.0.2/ml_rwkv.egg-info/PKG-INFO` & `ml-rwkv-0.0.3/ml_rwkv.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-rwkv
-Version: 0.0.2
+Version: 0.0.3
 Summary: RWKV implementation that is friendly with `ml-starter`
 Home-page: https://github.com/codekansas/rwkv
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-rwkv-0.0.2/ml_rwkv.egg-info/SOURCES.txt` & `ml-rwkv-0.0.3/ml_rwkv.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 ml_rwkv.egg-info/top_level.txt
 rwkv/__init__.py
 rwkv/model.py
 rwkv/run.py
 rwkv/triton/__init__.py
 rwkv/triton/utils.py
 rwkv/triton/wkv/__init__.py
+rwkv/triton/wkv/eps.py
+rwkv/triton/wkv/log.py
 rwkv/triton/wkv/vanilla.py
 rwkv/wkv/__init__.py
 rwkv/wkv/eps.py
 rwkv/wkv/log.py
 rwkv/wkv/vanilla.py
 tests/test_eps_wkv.py
 tests/test_log_wkv.py
```

### Comparing `ml-rwkv-0.0.2/pyproject.toml` & `ml-rwkv-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ml-rwkv-0.0.2/rwkv/model.py` & `ml-rwkv-0.0.3/rwkv/model.py`

 * *Files identical despite different names*

### Comparing `ml-rwkv-0.0.2/rwkv/run.py` & `ml-rwkv-0.0.3/rwkv/run.py`

 * *Files identical despite different names*

### Comparing `ml-rwkv-0.0.2/rwkv/triton/wkv/vanilla.py` & `ml-rwkv-0.0.3/rwkv/triton/wkv/vanilla.py`

 * *Files 8% similar despite different names*

```diff
@@ -112,17 +112,14 @@
     assert w.shape == (chans,), f"{w.shape} != {(chans,)}"
     assert u.shape == (chans,), f"{u.shape} != {(chans,)}"
 
     # Checks tensor dtypes and devices.
     for t in (v, state, w, u):
         assert t.dtype == dtype and t.device == device, f"{t.dtype} != {dtype} or {t.device} != {device}"
 
-    alpha, beta = state[:, :, -1].chunk(2, dim=1)  # (B, 1, D), (B, 1, D)
-    alpha, beta = alpha.contiguous(), beta.contiguous()
-
     # New tensors to output.
     wkvs = k.new_empty(bsz, tsz, chans)
     state_out = k.new_empty(bsz, 2, tsz, chans)
 
     wkv_triton_vanilla_forward_kernel[(bsz, chans)](
         # W
         w,
@@ -271,22 +268,19 @@
         ek = tl.exp(kt)
 
         denom = beta_prev + euk
         denom_sq = denom * denom
 
         gwkvt = tl.load(gwkv_ptr + tc * gwkv_s_t + gwkv_s_c * cs, mask=cmask)
 
-        gk = tl.zeros_like(kt)
-        gv = tl.zeros_like(vt)
-
         # Backpropagates wkv gradients.
         guk = gwkvt * euk * (beta_prev * vt - alpha_prev) / denom_sq
         gu += guk
-        gk += guk
-        gv += gwkvt * euk / denom
+        gk = guk
+        gv = gwkvt * euk / denom
 
         galpha_wkv = gwkvt / denom
         gbeta_wkv = -gwkvt * (euk * vt + alpha_prev) / denom_sq
 
         # Backpropagates alpha gradients.
         gw += galpha * ew * alpha_prev
         gk += galpha * ek * vt
@@ -301,16 +295,18 @@
         tl.store(gv_ptr + tc * gv_s_t + gv_s_c * cs, gv, mask=cmask)
 
         # Computes new gradients for alpha and beta.
         galpha = galpha * ew + galpha_wkv
         gbeta = gbeta * ew + gbeta_wkv
 
     # Stores final gradients for alpha and beta.
-    tl.store(gstate_ptr + b_idx * gstate_s_b + gstate_s_c * cs, galpha, mask=cmask)
-    tl.store(gstate_ptr + b_idx * gstate_s_b + gstate_s_ab + gstate_s_c * cs, gbeta, mask=cmask)
+    galpha_ptr = gstate_ptr + b_idx * gstate_s_b
+    gbeta_ptr = gstate_ptr + b_idx * gstate_s_b + gstate_s_ab
+    tl.store(galpha_ptr + gstate_s_c * cs, galpha, mask=cmask)
+    tl.store(gbeta_ptr + gstate_s_c * cs, gbeta, mask=cmask)
 
     # Stores final gradients for w and u.
     tl.atomic_add(gw_ptr + gw_s_c * cs, gw, mask=cmask)
     tl.atomic_add(gu_ptr + gu_s_c * cs, gu, mask=cmask)
 
 
 def wkv_triton_vanilla_backward(
```

### Comparing `ml-rwkv-0.0.2/rwkv/wkv/__init__.py` & `ml-rwkv-0.0.3/rwkv/wkv/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,12 +58,16 @@
         case "eps":
             return wkv_with_eps, initial_state_with_eps(emb_dim)
         case "triton-vanilla":
             from rwkv.triton.wkv.vanilla import wkv_triton_vanilla
 
             return wkv_triton_vanilla, initial_state_vanilla(emb_dim)
         case "triton-log":
-            raise NotImplementedError
+            from rwkv.triton.wkv.log import wkv_triton_log_space
+
+            return wkv_triton_log_space, initial_state_log_space(emb_dim)
         case "triton-eps":
-            raise NotImplementedError
+            from rwkv.triton.wkv.eps import wkv_triton_with_eps
+
+            return wkv_triton_with_eps, initial_state_with_eps(emb_dim)
         case _:
             raise ValueError(f"Unknown implementation: {impl}")
```

### Comparing `ml-rwkv-0.0.2/rwkv/wkv/eps.py` & `ml-rwkv-0.0.3/rwkv/wkv/eps.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # mypy: disable-error-code="override"
 """Provides a numerically-stable implementation of the WKV computation.
 
 This implementation follows the official implementation.
 """
 
+from typing import cast
+
 import torch
 from torch import Tensor
 from torch.autograd.function import Function, FunctionCtx, once_differentiable
 
 
 @torch.jit.script
 def wkv_with_eps_forward(w: Tensor, u: Tensor, k: Tensor, v: Tensor, state: Tensor) -> tuple[Tensor, Tensor]:
@@ -88,15 +90,15 @@
         tau = torch.maximum(ukt, eps_prev)
         e1 = torch.exp(eps_prev - tau)
         e2 = torch.exp(ukt - tau)
 
         euke = torch.exp(ukt + eps_prev - 2 * tau)
 
         denom = e1 * beta_prev + e2
-        denom_sq = denom**2
+        denom_sq = denom * denom
 
         grad_wkvt = grad_wkv[:, t : t + 1]
 
         # Backpropagates wkv gradients.
         grad_uk = grad_wkvt * e2 * (e1 * beta_prev * vt - e1 * alpha_prev) / denom_sq
         grad_u += grad_uk.flatten(0, -2).sum(0)
         grad_k[:, t : t + 1] += grad_uk
@@ -153,15 +155,15 @@
     @staticmethod
     @once_differentiable
     def backward(
         ctx: FunctionCtx,
         grad_wkv: Tensor,
         grad_state: Tensor,
     ) -> tuple[Tensor, Tensor, Tensor, Tensor, Tensor]:
-        w, u, k, v, state = ctx.saved_tensors
+        w, u, k, v, state = cast(tuple[Tensor, ...], ctx.saved_tensors)
         return wkv_with_eps_backward(w, u, k, v, state, grad_wkv, grad_state)
 
 
 def initial_state_with_eps(emb_dim: int) -> Tensor:
     return torch.zeros(1, 3, 1, emb_dim)
```

### Comparing `ml-rwkv-0.0.2/rwkv/wkv/log.py` & `ml-rwkv-0.0.3/rwkv/wkv/log.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,33 +2,33 @@
 """Provides a numerically-stable implementation of the WKV computation.
 
 This implementation uses log-space state variables, verses the original
 implementation which offsets the exponents.
 """
 
 import math
+from typing import cast
 
 import torch
 from torch import Tensor
 from torch.autograd.function import Function, FunctionCtx, once_differentiable
 
 EPS = 1e-9
 
 
 @torch.jit.script
 def logaddexp(a: Tensor, b: Tensor) -> Tensor:
-    # max_av = torch.maximum(a, b)
-    # return max_av + torch.log(torch.exp(a - max_av) + torch.exp(b - max_av))
-    return torch.logaddexp(a, b)
+    max_ab = torch.maximum(a, b)
+    return max_ab + torch.log(torch.exp(a - max_ab) + torch.exp(b - max_ab))
 
 
 @torch.jit.script
 def logsubexp(a: Tensor, b: Tensor, log_eps: float) -> Tensor:
-    max_av = torch.maximum(torch.maximum(a, b), torch.full_like(a, log_eps))
-    return max_av + torch.log(torch.exp(a - max_av) - torch.exp(b - max_av))
+    max_ab = torch.clamp_min(torch.maximum(a, b), log_eps)
+    return max_ab + torch.log(torch.exp(a - max_ab) - torch.exp(b - max_ab))
 
 
 @torch.jit.script
 def wkv_log_space_forward(
     w: Tensor,
     u: Tensor,
     k: Tensor,
@@ -182,15 +182,15 @@
     @staticmethod
     @once_differentiable
     def backward(
         ctx: FunctionCtx,
         grad_wkv: Tensor,
         grad_state: Tensor,
     ) -> tuple[Tensor, Tensor, Tensor, Tensor, Tensor]:
-        w, u, k, v, state = ctx.saved_tensors
+        w, u, k, v, state = cast(tuple[Tensor, ...], ctx.saved_tensors)
         return wkv_log_space_backward(w, u, k, v, state, grad_wkv, grad_state)
 
 
 def initial_state_log_space(emb_dim: int) -> Tensor:
     return torch.full((1, 3, 1, emb_dim), float("-inf"))
```

### Comparing `ml-rwkv-0.0.2/rwkv/wkv/vanilla.py` & `ml-rwkv-0.0.3/rwkv/wkv/vanilla.py`

 * *Files identical despite different names*

### Comparing `ml-rwkv-0.0.2/setup.py` & `ml-rwkv-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `ml-rwkv-0.0.2/tests/test_eps_wkv.py` & `ml-rwkv-0.0.3/tests/test_eps_wkv.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 def _get_grads(*t: Tensor) -> tuple[Tensor | None, ...]:
     return tuple(cast(Tensor, t_i.grad) for t_i in t)
 
 
 def test_eps_wkv() -> None:
     bsz, tsz, chans = 2, 7, 16
-    device, dtype = torch.device("cpu"), torch.float32
+    device, dtype = torch.device("cpu"), torch.float64
 
     w, u, k, v = _get_dummy_tensors(bsz, tsz, chans, device, dtype)
     state = initial_state_with_eps(chans).repeat_interleave(bsz, dim=0).to(device, dtype)
 
     # Runs in full mode.
     out_full, _ = wkv_with_eps(w, u, k, v, state)
 
@@ -43,15 +43,15 @@
         out_parts.append(out_part)
     out_partial = torch.cat(out_parts, dim=1)
 
     assert torch.allclose(out_full, out_partial)
 
 
 @pytest.mark.parametrize("mode", ["state", "wkv", "both"])
-def test_eps_wkv_gradients(mode: str) -> None:
+def test_gradients_eps_wkv(mode: str) -> None:
     bsz, tsz, chans = 2, 7, 16
     device, dtype = torch.device("cpu"), torch.float64
 
     w, u, k, v = _get_dummy_tensors(bsz, tsz, chans, device, dtype)
     state = initial_state_with_eps(chans).repeat_interleave(bsz, dim=0).to(device, dtype)
 
     def backprop(wkv_out: Tensor, state_out: Tensor) -> None:
```

### Comparing `ml-rwkv-0.0.2/tests/test_log_wkv.py` & `ml-rwkv-0.0.3/tests/test_log_wkv.py`

 * *Files 9% similar despite different names*

```diff
@@ -50,39 +50,32 @@
 def test_log_wkv_gradients(mode: str) -> None:
     bsz, tsz, chans = 2, 7, 16
     device, dtype = torch.device("cpu"), torch.float64
 
     w, u, k, v = _get_dummy_tensors(bsz, tsz, chans, device, dtype)
     state = initial_state_log_space(chans).repeat_interleave(bsz, dim=0).to(device, dtype)
 
-    def backprop(wkv_out: Tensor, state_out: Tensor, wkv_grad: Tensor, state_out_grad: Tensor) -> None:
-        if mode == "both":
-            torch.autograd.backward((wkv_out, state_out), (wkv_grad, state_out_grad))
-        elif mode == "wkv":
-            wkv_out.backward(wkv_grad)
-        elif mode == "state":
-            state_out.backward(state_out_grad)
-        else:
-            raise ValueError(f"Invalid mode: {mode}")
-
     # Uses autograd to compute the gradients.
     wt, ut, kt, vt, statet = _copy_with_grad(w, u, k, v, state)
     wkv_ref, state_out_ref = wkv_log_space_forward(wt, ut, kt, vt, statet)
     state_out_ref = state_out_ref[:, :, -1:]
-    wkv_grad, state_out_grad = torch.rand_like(wkv_ref), torch.rand_like(state_out_ref)
-    backprop(wkv_ref, state_out_ref, wkv_grad, state_out_grad)
+    wkv_grad = torch.zeros_like(wkv_ref) if mode == "state" else torch.rand_like(wkv_ref)
+    state_out_grad = torch.zeros_like(state_out_ref) if mode == "wkv" else torch.rand_like(state_out_ref)
+    torch.autograd.backward((wkv_ref, state_out_ref), (wkv_grad, state_out_grad))
     wgr, ugr, kgr, vgr, stategr = _get_grads(wt, ut, kt, vt, statet)
 
     # Uses the manual gradient computation to compute the gradients.
     wt, ut, kt, vt, statet = _copy_with_grad(w, u, k, v, state)
     wkv_man, state_out_man = wkv_log_space(wt, ut, kt, vt, statet)
-    backprop(wkv_man, state_out_man, wkv_grad, state_out_grad)
+    torch.autograd.backward((wkv_man, state_out_man), (wkv_grad, state_out_grad))
     wgm, ugm, kgm, vgm, stategm = _get_grads(wt, ut, kt, vt, statet)
 
-    for gr, gm in zip((wgr, ugr, kgr, vgr, stategr), (wgm, ugm, kgm, vgm, stategm)):
-        if gr is not None and gm is not None:
-            assert torch.allclose(gr, gm)
-
-
-if __name__ == "__main__":
-    # python -m tests.test_log_wkv
-    test_log_wkv_gradients("wkv")
+    for gr, gm, gname in [
+        (wgr, wgm, "w"),
+        (ugr, ugm, "u"),
+        (kgr, kgm, "k"),
+        (vgr, vgm, "v"),
+        (stategr, stategm, "state"),
+    ]:
+        if gr is None or gm is None:
+            continue
+        assert torch.allclose(gr, gm), f"Gradient {gname} mismatch"
```

### Comparing `ml-rwkv-0.0.2/tests/test_vanilla_wkv.py` & `ml-rwkv-0.0.3/tests/test_vanilla_wkv.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 def _get_grads(*t: Tensor) -> tuple[Tensor | None, ...]:
     return tuple(cast(Tensor, t_i.grad) for t_i in t)
 
 
 def test_vanilla_wkv() -> None:
     bsz, tsz, chans = 2, 7, 16
-    device, dtype = torch.device("cpu"), torch.float32
+    device, dtype = torch.device("cpu"), torch.float64
 
     w, u, k, v = _get_dummy_tensors(bsz, tsz, chans, device, dtype)
     state = initial_state_vanilla(chans).repeat_interleave(bsz, dim=0).to(device, dtype)
 
     # Runs in full mode.
     out_full, _ = wkv_vanilla(w, u, k, v, state)
 
@@ -47,15 +47,15 @@
         out_parts.append(out_part)
     out_partial = torch.cat(out_parts, dim=1)
 
     assert torch.allclose(out_full, out_partial)
 
 
 @pytest.mark.parametrize("mode", ["state", "wkv", "both"])
-def test_vanilla_wkv_gradients(mode: str) -> None:
+def test_gradients_vanilla_wkv(mode: str) -> None:
     bsz, tsz, chans = 2, 7, 16
     device, dtype = torch.device("cpu"), torch.float64
 
     w, u, k, v = _get_dummy_tensors(bsz, tsz, chans, device, dtype)
     state = initial_state_vanilla(chans).repeat_interleave(bsz, dim=0).to(device, dtype)
 
     def backprop(wkv_out: Tensor, state_out: Tensor) -> None:
@@ -80,12 +80,7 @@
     wkv_man, state_out_man = wkv_vanilla(wt, ut, kt, vt, statet)
     backprop(wkv_man, state_out_man)
     wgm, ugm, kgm, vgm, stategm = _get_grads(wt, ut, kt, vt, statet)
 
     for gr, gm in zip((wgr, ugr, kgr, vgr, stategr), (wgm, ugm, kgm, vgm, stategm)):
         if gr is not None and gm is not None:
             assert torch.allclose(gr, gm)
-
-
-if __name__ == "__main__":
-    # python -m tests.test_vanilla_wkv
-    test_vanilla_wkv_gradients("wkv")
```

### Comparing `ml-rwkv-0.0.2/tests/test_wkv.py` & `ml-rwkv-0.0.3/tests/test_wkv.py`

 * *Files identical despite different names*

