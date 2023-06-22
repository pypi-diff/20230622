# Comparing `tmp/nvidia-dali-nightly-cuda120-1.28.0.dev20230620.tar.gz` & `tmp/nvidia-dali-nightly-cuda120-1.28.0.dev20230621.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvidia-dali-nightly-cuda120-1.28.0.dev20230620.tar", last modified: Tue Jun 20 10:44:37 2023, max compression
+gzip compressed data, was "nvidia-dali-nightly-cuda120-1.28.0.dev20230621.tar", last modified: Thu Jun 22 15:24:32 2023, max compression
```

## Comparing `nvidia-dali-nightly-cuda120-1.28.0.dev20230620.tar` & `nvidia-dali-nightly-cuda120-1.28.0.dev20230621.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-20 10:44:37.855159 nvidia-dali-nightly-cuda120-1.28.0.dev20230620/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      459 2023-06-20 10:44:37.000000 nvidia-dali-nightly-cuda120-1.28.0.dev20230620/ERROR.txt
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-06-14 04:38:44.000000 nvidia-dali-nightly-cuda120-1.28.0.dev20230620/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       27 2023-06-20 10:44:37.000000 nvidia-dali-nightly-cuda120-1.28.0.dev20230620/PACKAGE_NAME
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1668 2023-06-20 10:44:37.855159 nvidia-dali-nightly-cuda120-1.28.0.dev20230620/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      286 2023-06-20 10:44:37.000000 nvidia-dali-nightly-cuda120-1.28.0.dev20230620/README.rst
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-20 10:44:37.855159 nvidia-dali-nightly-cuda120-1.28.0.dev20230620/nvidia_dali_nightly_cuda120.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1668 2023-06-20 10:44:37.000000 nvidia-dali-nightly-cuda120-1.28.0.dev20230620/nvidia_dali_nightly_cuda120.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      257 2023-06-20 10:44:37.000000 nvidia-dali-nightly-cuda120-1.28.0.dev20230620/nvidia_dali_nightly_cuda120.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-06-20 10:44:37.000000 nvidia-dali-nightly-cuda120-1.28.0.dev20230620/nvidia_dali_nightly_cuda120.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-06-20 10:44:37.000000 nvidia-dali-nightly-cuda120-1.28.0.dev20230620/nvidia_dali_nightly_cuda120.egg-info/top_level.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-06-20 10:44:37.855159 nvidia-dali-nightly-cuda120-1.28.0.dev20230620/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-06-14 04:38:44.000000 nvidia-dali-nightly-cuda120-1.28.0.dev20230620/setup.py
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-22 15:24:32.876755 nvidia-dali-nightly-cuda120-1.28.0.dev20230621/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      459 2023-06-22 15:24:32.000000 nvidia-dali-nightly-cuda120-1.28.0.dev20230621/ERROR.txt
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-06-14 04:38:44.000000 nvidia-dali-nightly-cuda120-1.28.0.dev20230621/LICENSE.md
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       27 2023-06-22 15:24:32.000000 nvidia-dali-nightly-cuda120-1.28.0.dev20230621/PACKAGE_NAME
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1668 2023-06-22 15:24:32.876755 nvidia-dali-nightly-cuda120-1.28.0.dev20230621/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      286 2023-06-22 15:24:32.000000 nvidia-dali-nightly-cuda120-1.28.0.dev20230621/README.rst
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-22 15:24:32.876755 nvidia-dali-nightly-cuda120-1.28.0.dev20230621/nvidia_dali_nightly_cuda120.egg-info/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1668 2023-06-22 15:24:32.000000 nvidia-dali-nightly-cuda120-1.28.0.dev20230621/nvidia_dali_nightly_cuda120.egg-info/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      257 2023-06-22 15:24:32.000000 nvidia-dali-nightly-cuda120-1.28.0.dev20230621/nvidia_dali_nightly_cuda120.egg-info/SOURCES.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-06-22 15:24:32.000000 nvidia-dali-nightly-cuda120-1.28.0.dev20230621/nvidia_dali_nightly_cuda120.egg-info/dependency_links.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-06-22 15:24:32.000000 nvidia-dali-nightly-cuda120-1.28.0.dev20230621/nvidia_dali_nightly_cuda120.egg-info/top_level.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-06-22 15:24:32.876755 nvidia-dali-nightly-cuda120-1.28.0.dev20230621/setup.cfg
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-06-14 04:38:44.000000 nvidia-dali-nightly-cuda120-1.28.0.dev20230621/setup.py
```

### Comparing `nvidia-dali-nightly-cuda120-1.28.0.dev20230620/LICENSE.md` & `nvidia-dali-nightly-cuda120-1.28.0.dev20230621/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nvidia-dali-nightly-cuda120-1.28.0.dev20230620/PKG-INFO` & `nvidia-dali-nightly-cuda120-1.28.0.dev20230621/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-nightly-cuda120
-Version: 1.28.0.dev20230620
+Version: 1.28.0.dev20230621
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `nvidia-dali-nightly-cuda120-1.28.0.dev20230620/nvidia_dali_nightly_cuda120.egg-info/PKG-INFO` & `nvidia-dali-nightly-cuda120-1.28.0.dev20230621/nvidia_dali_nightly_cuda120.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-nightly-cuda120
-Version: 1.28.0.dev20230620
+Version: 1.28.0.dev20230621
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `nvidia-dali-nightly-cuda120-1.28.0.dev20230620/setup.py` & `nvidia-dali-nightly-cuda120-1.28.0.dev20230621/setup.py`

 * *Files identical despite different names*

