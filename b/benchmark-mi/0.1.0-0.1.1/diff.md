# Comparing `tmp/benchmark_mi-0.1.0.tar.gz` & `tmp/benchmark_mi-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "benchmark_mi-0.1.0.tar", max compression
+gzip compressed data, was "benchmark_mi-0.1.1.tar", max compression
```

## Comparing `benchmark_mi-0.1.0.tar` & `benchmark_mi-0.1.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0     1069 2022-09-04 15:32:37.482599 benchmark_mi-0.1.0/LICENSE
--rw-r--r--   0        0        0     2863 2023-06-22 10:18:16.367190 benchmark_mi-0.1.0/README.md
--rw-r--r--   0        0        0     1686 2023-06-22 14:19:44.400892 benchmark_mi-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      855 2023-04-18 08:12:30.427657 benchmark_mi-0.1.0/src/bmi/__init__.py
--rw-r--r--   0        0        0      405 2023-04-26 08:58:26.068033 benchmark_mi-0.1.0/src/bmi/benchmark/__init__.py
--rw-r--r--   0        0        0     2511 2023-04-21 14:02:30.457371 benchmark_mi-0.1.0/src/bmi/benchmark/result.py
--rw-r--r--   0        0        0     2316 2023-04-25 06:41:03.254696 benchmark_mi-0.1.0/src/bmi/benchmark/task.py
--rw-r--r--   0        0        0     3426 2023-06-09 15:54:47.936482 benchmark_mi-0.1.0/src/bmi/benchmark/task_list.py
--rw-r--r--   0        0        0     1640 2023-05-11 08:40:52.316036 benchmark_mi-0.1.0/src/bmi/benchmark/tasks/__init__.py
--rw-r--r--   0        0        0      410 2023-04-18 08:12:30.427657 benchmark_mi-0.1.0/src/bmi/benchmark/tasks/additive_noise.py
--rw-r--r--   0        0        0      595 2023-04-21 14:02:30.457371 benchmark_mi-0.1.0/src/bmi/benchmark/tasks/asinh.py
--rw-r--r--   0        0        0     1079 2023-05-11 08:40:52.316036 benchmark_mi-0.1.0/src/bmi/benchmark/tasks/bimodal_gaussians.py
--rw-r--r--   0        0        0      458 2023-05-11 08:40:52.316036 benchmark_mi-0.1.0/src/bmi/benchmark/tasks/bivariate_normal.py
--rw-r--r--   0        0        0      570 2023-04-18 08:12:30.427657 benchmark_mi-0.1.0/src/bmi/benchmark/tasks/embeddings.py
--rw-r--r--   0        0        0      615 2023-04-18 08:12:30.427657 benchmark_mi-0.1.0/src/bmi/benchmark/tasks/half_cube.py
--rw-r--r--   0        0        0     2811 2023-05-11 08:40:52.316036 benchmark_mi-0.1.0/src/bmi/benchmark/tasks/multinormal.py
--rw-r--r--   0        0        0      621 2023-04-18 08:12:30.427657 benchmark_mi-0.1.0/src/bmi/benchmark/tasks/normal_cdf.py
--rw-r--r--   0        0        0      766 2023-04-25 06:41:03.254696 benchmark_mi-0.1.0/src/bmi/benchmark/tasks/power.py
--rw-r--r--   0        0        0     1400 2023-04-18 08:12:30.431657 benchmark_mi-0.1.0/src/bmi/benchmark/tasks/rotate.py
--rw-r--r--   0        0        0     2896 2023-05-11 08:40:52.316036 benchmark_mi-0.1.0/src/bmi/benchmark/tasks/scaling.py
--rw-r--r--   0        0        0     1318 2023-05-11 08:40:52.316036 benchmark_mi-0.1.0/src/bmi/benchmark/tasks/spiral.py
--rw-r--r--   0        0        0     2638 2023-05-11 12:42:03.244573 benchmark_mi-0.1.0/src/bmi/benchmark/tasks/student.py
--rw-r--r--   0        0        0      879 2023-04-18 08:12:30.431657 benchmark_mi-0.1.0/src/bmi/benchmark/tasks/wiggly.py
--rw-r--r--   0        0        0        0 2023-04-17 13:43:16.477119 benchmark_mi-0.1.0/src/bmi/benchmark/utils/__init__.py
--rw-r--r--   0        0        0      969 2023-04-17 13:43:16.481119 benchmark_mi-0.1.0/src/bmi/benchmark/utils/dict_dumper.py
--rw-r--r--   0        0        0     1263 2023-04-17 13:43:16.481119 benchmark_mi-0.1.0/src/bmi/benchmark/utils/timer.py
--rw-r--r--   0        0        0      982 2023-04-25 06:41:03.254696 benchmark_mi-0.1.0/src/bmi/estimators/__init__.py
--rw-r--r--   0        0        0     2724 2023-04-18 08:12:30.431657 benchmark_mi-0.1.0/src/bmi/estimators/_histogram.py
--rw-r--r--   0        0        0     5090 2023-04-18 08:12:30.431657 benchmark_mi-0.1.0/src/bmi/estimators/_kde.py
--rw-r--r--   0        0        0      193 2022-09-10 12:24:03.944146 benchmark_mi-0.1.0/src/bmi/estimators/base.py
--rw-r--r--   0        0        0      974 2023-01-11 13:17:48.363884 benchmark_mi-0.1.0/src/bmi/estimators/correlation.py
--rw-r--r--   0        0        0        0 2023-04-17 13:43:16.481119 benchmark_mi-0.1.0/src/bmi/estimators/external/__init__.py
--rw-r--r--   0        0        0     1421 2023-04-21 14:02:30.457371 benchmark_mi-0.1.0/src/bmi/estimators/external/external_estimator.py
--rw-r--r--   0        0        0     4595 2023-04-17 13:43:16.481119 benchmark_mi-0.1.0/src/bmi/estimators/external/julia_estimators.py
--rw-r--r--   0        0        0     3743 2023-04-17 13:43:16.481119 benchmark_mi-0.1.0/src/bmi/estimators/external/r_estimators.py
--rw-r--r--   0        0        0     1111 2023-01-11 13:17:48.363884 benchmark_mi-0.1.0/src/bmi/estimators/function_wrapper.py
--rw-r--r--   0        0        0    10065 2023-01-11 13:17:48.363884 benchmark_mi-0.1.0/src/bmi/estimators/ksg.py
--rw-r--r--   0        0        0      506 2023-04-20 06:38:31.092199 benchmark_mi-0.1.0/src/bmi/estimators/neural/__init__.py
--rw-r--r--   0        0        0     2528 2023-04-20 06:38:31.092199 benchmark_mi-0.1.0/src/bmi/estimators/neural/_backend_linear_memory.py
--rw-r--r--   0        0        0     1933 2023-04-20 06:38:31.092199 benchmark_mi-0.1.0/src/bmi/estimators/neural/_backend_quadratic_memory.py
--rw-r--r--   0        0        0     3057 2023-05-02 14:04:39.541203 benchmark_mi-0.1.0/src/bmi/estimators/neural/_basic_training.py
--rw-r--r--   0        0        0     1794 2023-04-28 10:29:27.556715 benchmark_mi-0.1.0/src/bmi/estimators/neural/_critics.py
--rw-r--r--   0        0        0    11078 2023-05-02 14:04:39.541203 benchmark_mi-0.1.0/src/bmi/estimators/neural/_estimators.py
--rw-r--r--   0        0        0    11527 2023-05-02 14:04:39.541203 benchmark_mi-0.1.0/src/bmi/estimators/neural/_mine_estimator.py
--rw-r--r--   0        0        0     6655 2023-05-02 14:04:39.541203 benchmark_mi-0.1.0/src/bmi/estimators/neural/_training_log.py
--rw-r--r--   0        0        0      469 2023-04-20 06:38:31.092199 benchmark_mi-0.1.0/src/bmi/estimators/neural/_types.py
--rw-r--r--   0        0        0     3258 2023-04-21 14:02:30.457371 benchmark_mi-0.1.0/src/bmi/interface.py
--rw-r--r--   0        0        0        0 2023-03-09 09:37:35.444801 benchmark_mi-0.1.0/src/bmi/plot_utils/__init__.py
--rw-r--r--   0        0        0     2813 2023-03-28 10:17:29.390563 benchmark_mi-0.1.0/src/bmi/plot_utils/subplots_from_axsize.py
--rw-r--r--   0        0        0      967 2023-04-26 08:58:26.068033 benchmark_mi-0.1.0/src/bmi/samplers/__init__.py
--rw-r--r--   0        0        0     1674 2023-04-18 08:12:30.431657 benchmark_mi-0.1.0/src/bmi/samplers/_additive_uniform.py
--rw-r--r--   0        0        0    12595 2023-04-26 08:58:26.068033 benchmark_mi-0.1.0/src/bmi/samplers/_matrix_utils.py
--rw-r--r--   0        0        0     5814 2023-04-18 08:12:30.431657 benchmark_mi-0.1.0/src/bmi/samplers/_split_student_t.py
--rw-r--r--   0        0        0     7280 2023-04-18 08:12:30.431657 benchmark_mi-0.1.0/src/bmi/samplers/_splitmultinormal.py
--rw-r--r--   0        0        0     3749 2023-04-18 08:12:30.431657 benchmark_mi-0.1.0/src/bmi/samplers/_transformed.py
--rw-r--r--   0        0        0     1187 2023-01-11 13:40:10.079266 benchmark_mi-0.1.0/src/bmi/samplers/base.py
--rw-r--r--   0        0        0      336 2023-04-18 08:12:30.431657 benchmark_mi-0.1.0/src/bmi/transforms/__init__.py
--rw-r--r--   0        0        0     1226 2023-04-18 08:12:30.431657 benchmark_mi-0.1.0/src/bmi/transforms/_invert_cdf.py
--rw-r--r--   0        0        0     3780 2023-04-18 08:12:30.431657 benchmark_mi-0.1.0/src/bmi/transforms/_rotate.py
--rw-r--r--   0        0        0      736 2023-04-17 13:43:16.481119 benchmark_mi-0.1.0/src/bmi/transforms/simple.py
--rw-r--r--   0        0        0     4542 2023-04-17 13:43:16.481119 benchmark_mi-0.1.0/src/bmi/utils.py
--rw-r--r--   0        0        0     3773 1970-01-01 00:00:00.000000 benchmark_mi-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-09-04 15:32:37.482599 benchmark_mi-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3122 2023-06-22 14:27:34.217361 benchmark_mi-0.1.1/README.md
+-rw-r--r--   0        0        0     1727 2023-06-22 14:42:16.606444 benchmark_mi-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      855 2023-04-18 08:12:30.427657 benchmark_mi-0.1.1/src/bmi/__init__.py
+-rw-r--r--   0        0        0      405 2023-04-26 08:58:26.068033 benchmark_mi-0.1.1/src/bmi/benchmark/__init__.py
+-rw-r--r--   0        0        0     2511 2023-04-21 14:02:30.457371 benchmark_mi-0.1.1/src/bmi/benchmark/result.py
+-rw-r--r--   0        0        0     2316 2023-04-25 06:41:03.254696 benchmark_mi-0.1.1/src/bmi/benchmark/task.py
+-rw-r--r--   0        0        0     3426 2023-06-09 15:54:47.936482 benchmark_mi-0.1.1/src/bmi/benchmark/task_list.py
+-rw-r--r--   0        0        0     1640 2023-05-11 08:40:52.316036 benchmark_mi-0.1.1/src/bmi/benchmark/tasks/__init__.py
+-rw-r--r--   0        0        0      410 2023-04-18 08:12:30.427657 benchmark_mi-0.1.1/src/bmi/benchmark/tasks/additive_noise.py
+-rw-r--r--   0        0        0      595 2023-04-21 14:02:30.457371 benchmark_mi-0.1.1/src/bmi/benchmark/tasks/asinh.py
+-rw-r--r--   0        0        0     1079 2023-05-11 08:40:52.316036 benchmark_mi-0.1.1/src/bmi/benchmark/tasks/bimodal_gaussians.py
+-rw-r--r--   0        0        0      458 2023-05-11 08:40:52.316036 benchmark_mi-0.1.1/src/bmi/benchmark/tasks/bivariate_normal.py
+-rw-r--r--   0        0        0      570 2023-04-18 08:12:30.427657 benchmark_mi-0.1.1/src/bmi/benchmark/tasks/embeddings.py
+-rw-r--r--   0        0        0      615 2023-04-18 08:12:30.427657 benchmark_mi-0.1.1/src/bmi/benchmark/tasks/half_cube.py
+-rw-r--r--   0        0        0     2811 2023-05-11 08:40:52.316036 benchmark_mi-0.1.1/src/bmi/benchmark/tasks/multinormal.py
+-rw-r--r--   0        0        0      621 2023-04-18 08:12:30.427657 benchmark_mi-0.1.1/src/bmi/benchmark/tasks/normal_cdf.py
+-rw-r--r--   0        0        0      766 2023-04-25 06:41:03.254696 benchmark_mi-0.1.1/src/bmi/benchmark/tasks/power.py
+-rw-r--r--   0        0        0     1400 2023-04-18 08:12:30.431657 benchmark_mi-0.1.1/src/bmi/benchmark/tasks/rotate.py
+-rw-r--r--   0        0        0     2896 2023-05-11 08:40:52.316036 benchmark_mi-0.1.1/src/bmi/benchmark/tasks/scaling.py
+-rw-r--r--   0        0        0     1318 2023-05-11 08:40:52.316036 benchmark_mi-0.1.1/src/bmi/benchmark/tasks/spiral.py
+-rw-r--r--   0        0        0     2638 2023-05-11 12:42:03.244573 benchmark_mi-0.1.1/src/bmi/benchmark/tasks/student.py
+-rw-r--r--   0        0        0      879 2023-04-18 08:12:30.431657 benchmark_mi-0.1.1/src/bmi/benchmark/tasks/wiggly.py
+-rw-r--r--   0        0        0        0 2023-04-17 13:43:16.477119 benchmark_mi-0.1.1/src/bmi/benchmark/utils/__init__.py
+-rw-r--r--   0        0        0      969 2023-04-17 13:43:16.481119 benchmark_mi-0.1.1/src/bmi/benchmark/utils/dict_dumper.py
+-rw-r--r--   0        0        0     1263 2023-04-17 13:43:16.481119 benchmark_mi-0.1.1/src/bmi/benchmark/utils/timer.py
+-rw-r--r--   0        0        0      982 2023-04-25 06:41:03.254696 benchmark_mi-0.1.1/src/bmi/estimators/__init__.py
+-rw-r--r--   0        0        0     2724 2023-04-18 08:12:30.431657 benchmark_mi-0.1.1/src/bmi/estimators/_histogram.py
+-rw-r--r--   0        0        0     5090 2023-04-18 08:12:30.431657 benchmark_mi-0.1.1/src/bmi/estimators/_kde.py
+-rw-r--r--   0        0        0      193 2022-09-10 12:24:03.944146 benchmark_mi-0.1.1/src/bmi/estimators/base.py
+-rw-r--r--   0        0        0      974 2023-01-11 13:17:48.363884 benchmark_mi-0.1.1/src/bmi/estimators/correlation.py
+-rw-r--r--   0        0        0        0 2023-04-17 13:43:16.481119 benchmark_mi-0.1.1/src/bmi/estimators/external/__init__.py
+-rw-r--r--   0        0        0     1421 2023-04-21 14:02:30.457371 benchmark_mi-0.1.1/src/bmi/estimators/external/external_estimator.py
+-rw-r--r--   0        0        0     4595 2023-04-17 13:43:16.481119 benchmark_mi-0.1.1/src/bmi/estimators/external/julia_estimators.py
+-rw-r--r--   0        0        0     3743 2023-04-17 13:43:16.481119 benchmark_mi-0.1.1/src/bmi/estimators/external/r_estimators.py
+-rw-r--r--   0        0        0     1111 2023-01-11 13:17:48.363884 benchmark_mi-0.1.1/src/bmi/estimators/function_wrapper.py
+-rw-r--r--   0        0        0    10065 2023-01-11 13:17:48.363884 benchmark_mi-0.1.1/src/bmi/estimators/ksg.py
+-rw-r--r--   0        0        0      506 2023-04-20 06:38:31.092199 benchmark_mi-0.1.1/src/bmi/estimators/neural/__init__.py
+-rw-r--r--   0        0        0     2528 2023-04-20 06:38:31.092199 benchmark_mi-0.1.1/src/bmi/estimators/neural/_backend_linear_memory.py
+-rw-r--r--   0        0        0     1933 2023-04-20 06:38:31.092199 benchmark_mi-0.1.1/src/bmi/estimators/neural/_backend_quadratic_memory.py
+-rw-r--r--   0        0        0     3057 2023-05-02 14:04:39.541203 benchmark_mi-0.1.1/src/bmi/estimators/neural/_basic_training.py
+-rw-r--r--   0        0        0     1794 2023-04-28 10:29:27.556715 benchmark_mi-0.1.1/src/bmi/estimators/neural/_critics.py
+-rw-r--r--   0        0        0    11078 2023-05-02 14:04:39.541203 benchmark_mi-0.1.1/src/bmi/estimators/neural/_estimators.py
+-rw-r--r--   0        0        0    11527 2023-05-02 14:04:39.541203 benchmark_mi-0.1.1/src/bmi/estimators/neural/_mine_estimator.py
+-rw-r--r--   0        0        0     6655 2023-05-02 14:04:39.541203 benchmark_mi-0.1.1/src/bmi/estimators/neural/_training_log.py
+-rw-r--r--   0        0        0      469 2023-04-20 06:38:31.092199 benchmark_mi-0.1.1/src/bmi/estimators/neural/_types.py
+-rw-r--r--   0        0        0     3258 2023-04-21 14:02:30.457371 benchmark_mi-0.1.1/src/bmi/interface.py
+-rw-r--r--   0        0        0        0 2023-03-09 09:37:35.444801 benchmark_mi-0.1.1/src/bmi/plot_utils/__init__.py
+-rw-r--r--   0        0        0     2813 2023-03-28 10:17:29.390563 benchmark_mi-0.1.1/src/bmi/plot_utils/subplots_from_axsize.py
+-rw-r--r--   0        0        0      967 2023-04-26 08:58:26.068033 benchmark_mi-0.1.1/src/bmi/samplers/__init__.py
+-rw-r--r--   0        0        0     1674 2023-04-18 08:12:30.431657 benchmark_mi-0.1.1/src/bmi/samplers/_additive_uniform.py
+-rw-r--r--   0        0        0    12595 2023-04-26 08:58:26.068033 benchmark_mi-0.1.1/src/bmi/samplers/_matrix_utils.py
+-rw-r--r--   0        0        0     5814 2023-04-18 08:12:30.431657 benchmark_mi-0.1.1/src/bmi/samplers/_split_student_t.py
+-rw-r--r--   0        0        0     7280 2023-04-18 08:12:30.431657 benchmark_mi-0.1.1/src/bmi/samplers/_splitmultinormal.py
+-rw-r--r--   0        0        0     3749 2023-04-18 08:12:30.431657 benchmark_mi-0.1.1/src/bmi/samplers/_transformed.py
+-rw-r--r--   0        0        0     1187 2023-01-11 13:40:10.079266 benchmark_mi-0.1.1/src/bmi/samplers/base.py
+-rw-r--r--   0        0        0      336 2023-04-18 08:12:30.431657 benchmark_mi-0.1.1/src/bmi/transforms/__init__.py
+-rw-r--r--   0        0        0     1226 2023-04-18 08:12:30.431657 benchmark_mi-0.1.1/src/bmi/transforms/_invert_cdf.py
+-rw-r--r--   0        0        0     3780 2023-04-18 08:12:30.431657 benchmark_mi-0.1.1/src/bmi/transforms/_rotate.py
+-rw-r--r--   0        0        0      736 2023-04-17 13:43:16.481119 benchmark_mi-0.1.1/src/bmi/transforms/simple.py
+-rw-r--r--   0        0        0     4542 2023-04-17 13:43:16.481119 benchmark_mi-0.1.1/src/bmi/utils.py
+-rw-r--r--   0        0        0     4032 1970-01-01 00:00:00.000000 benchmark_mi-0.1.1/PKG-INFO
```

### Comparing `benchmark_mi-0.1.0/LICENSE` & `benchmark_mi-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `benchmark_mi-0.1.0/README.md` & `benchmark_mi-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 [![arXiv](https://img.shields.io/badge/arXiv-2306.11078-b31b1b.svg)](https://arxiv.org/abs/2306.11078)
 [![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
+[![PyPI Latest Release](https://img.shields.io/pypi/v/benchmark-mi.svg)](https://pypi.org/project/benchmark-mi/)
 [![build](https://github.com/cbg-ethz/bmi/actions/workflows/build.yml/badge.svg?branch=main)](https://github.com/cbg-ethz/bmi/actions/workflows/build.yml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 # Benchmarking Mutual Information
 
 BMI is the package for estimation of mutual information between continuous random variables and testing new estimators.
 
 - **Documentation**: [https://cbg-ethz.github.io/bmi/](https://cbg-ethz.github.io/bmi/)
 - **Source code**: [https://github.com/cbg-ethz/bmi](https://github.com/cbg-ethz/bmi)
 - **Bug reports**: [https://github.com/cbg-ethz/bmi/issues](https://github.com/cbg-ethz/bmi/issues)
-
+- **PyPI package**: [https://pypi.org/project/benchmark-mi](https://pypi.org/project/benchmark-mi)
 
 ## Getting started
 While we recommend taking a look at the [documentation](https://cbg-ethz.github.io/bmi/) to learn about full package capabilities, below we present the main capabilities of the Python package.
 (Note that BMI can also be used to test non-Python mutual information estimators.)
 
 You can install the package using:
 
-**TODO:** Add installation instructions after we push to PyPI.
+```bash
+$ pip install benchmark-mi
+```
+
+Alternatively, you can use the development version from source using:
+
 ```bash
 $ pip install "bmi @ https://github.com/cbg-ethz/bmi"
 ```
 
 Note: BMI uses [JAX](https://github.com/google/jax) and by default installs the CPU version of it.
 If you have a device supporting CUDA, you can [install the CUDA version of JAX](https://github.com/google/jax#pip-installation-gpu-cuda-installed-via-pip-easier).
```

### Comparing `benchmark_mi-0.1.0/pyproject.toml` & `benchmark_mi-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "benchmark-mi"
-version = "0.1.0"
+version = "0.1.1"
 description = "Estimators of mutual information and distributions used to benchmark them."
 authors = ["Paweł Czyż <pawelpiotr.czyz@ai.ethz.ch>", "Frederic Grabowski <grabowski.frederic@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "bmi", from = "src"}]
 
 [tool.poetry.dependencies]
@@ -21,14 +21,17 @@
 pandas = "<2.0.0"
 pydantic = "^1.10.7"
 pyyaml = "^6.0"
 scipy = "^1.10.1"
 tqdm = "^4.64.1"
 
 
+[tool.poetry.group.dev]
+optional = true
+
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 flake8 = "^6.0.0"
 isort = "^5.12.0"
 pre-commit = "^3.2.2"
 pytype = "^2023.4.11"
 pytest = "^7.3.1"
```

### Comparing `benchmark_mi-0.1.0/src/bmi/__init__.py` & `benchmark_mi-0.1.1/src/bmi/__init__.py`

 * *Files identical despite different names*

### Comparing `benchmark_mi-0.1.0/src/bmi/benchmark/result.py` & `benchmark_mi-0.1.1/src/bmi/benchmark/result.py`

 * *Files identical despite different names*

### Comparing `benchmark_mi-0.1.0/src/bmi/benchmark/task.py` & `benchmark_mi-0.1.1/src/bmi/benchmark/task.py`

 * *Files identical despite different names*

### Comparing `benchmark_mi-0.1.0/src/bmi/benchmark/task_list.py` & `benchmark_mi-0.1.1/src/bmi/benchmark/task_list.py`

 * *Files identical despite different names*

### Comparing `benchmark_mi-0.1.0/src/bmi/benchmark/tasks/__init__.py` & `benchmark_mi-0.1.1/src/bmi/benchmark/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `benchmark_mi-0.1.0/src/bmi/benchmark/tasks/asinh.py` & `benchmark_mi-0.1.1/src/bmi/benchmark/tasks/asinh.py`

 * *Files identical despite different names*

### Comparing `benchmark_mi-0.1.0/src/bmi/benchmark/tasks/bimodal_gaussians.py` & `benchmark_mi-0.1.1/src/bmi/benchmark/tasks/bimodal_gaussians.py`

 * *Files identical despite different names*

### Comparing `benchmark_mi-0.1.0/src/bmi/benchmark/tasks/embeddings.py` & `benchmark_mi-0.1.1/src/bmi/benchmark/tasks/embeddings.py`

 * *Files identical despite different names*

### Comparing `benchmark_mi-0.1.0/src/bmi/benchmark/tasks/half_cube.py` & `benchmark_mi-0.1.1/src/bmi/benchmark/tasks/half_cube.py`

 * *Files identical despite different names*

### Comparing `benchmark_mi-0.1.0/src/bmi/benchmark/tasks/multinormal.py` & `benchmark_mi-0.1.1/src/bmi/benchmark/tasks/multinormal.py`

 * *Files identical despite different names*

### Comparing `benchmark_mi-0.1.0/src/bmi/benchmark/tasks/normal_cdf.py` & `benchmark_mi-0.1.1/src/bmi/benchmark/tasks/normal_cdf.py`

 * *Files identical despite different names*

### Comparing `benchmark_mi-0.1.0/src/bmi/benchmark/tasks/power.py` & `benchmark_mi-0.1.1/src/bmi/benchmark/tasks/power.py`

 * *Files identical despite different names*

### Comparing `benchmark_mi-0.1.0/src/bmi/benchmark/tasks/rotate.py` & `benchmark_mi-0.1.1/src/bmi/benchmark/tasks/rotate.py`

 * *Files identical despite different names*

### Comparing `benchmark_mi-0.1.0/src/bmi/benchmark/tasks/scaling.py` & `benchmark_mi-0.1.1/src/bmi/benchmark/tasks/scaling.py`

 * *Files identical despite different names*

### Comparing `benchmark_mi-0.1.0/src/bmi/benchmark/tasks/spiral.py` & `benchmark_mi-0.1.1/src/bmi/benchmark/tasks/spiral.py`

 * *Files identical despite different names*

### Comparing `benchmark_mi-0.1.0/src/bmi/benchmark/tasks/student.py` & `benchmark_mi-0.1.1/src/bmi/benchmark/tasks/student.py`

 * *Files identical despite different names*

### Comparing `benchmark_mi-0.1.0/src/bmi/benchmark/tasks/wiggly.py` & `benchmark_mi-0.1.1/src/bmi/benchmark/tasks/wiggly.py`

 * *Files identical despite different names*

### Comparing `benchmark_mi-0.1.0/src/bmi/benchmark/utils/dict_dumper.py` & `benchmark_mi-0.1.1/src/bmi/benchmark/utils/dict_dumper.py`

 * *Files identical despite different names*

### Comparing `benchmark_mi-0.1.0/src/bmi/benchmark/utils/timer.py` & `benchmark_mi-0.1.1/src/bmi/benchmark/utils/timer.py`

 * *Files identical despite different names*

### Comparing `benchmark_mi-0.1.0/src/bmi/estimators/__init__.py` & `benchmark_mi-0.1.1/src/bmi/estimators/__init__.py`

 * *Files identical despite different names*

### Comparing `benchmark_mi-0.1.0/src/bmi/estimators/_histogram.py` & `benchmark_mi-0.1.1/src/bmi/estimators/_histogram.py`

 * *Files identical despite different names*

### Comparing `benchmark_mi-0.1.0/src/bmi/estimators/_kde.py` & `benchmark_mi-0.1.1/src/bmi/estimators/_kde.py`

 * *Files identical despite different names*

### Comparing `benchmark_mi-0.1.0/src/bmi/estimators/correlation.py` & `benchmark_mi-0.1.1/src/bmi/estimators/correlation.py`

 * *Files identical despite different names*

### Comparing `benchmark_mi-0.1.0/src/bmi/estimators/external/external_estimator.py` & `benchmark_mi-0.1.1/src/bmi/estimators/external/external_estimator.py`

 * *Files identical despite different names*

### Comparing `benchmark_mi-0.1.0/src/bmi/estimators/external/julia_estimators.py` & `benchmark_mi-0.1.1/src/bmi/estimators/external/julia_estimators.py`

 * *Files identical despite different names*

### Comparing `benchmark_mi-0.1.0/src/bmi/estimators/external/r_estimators.py` & `benchmark_mi-0.1.1/src/bmi/estimators/external/r_estimators.py`

 * *Files identical despite different names*

### Comparing `benchmark_mi-0.1.0/src/bmi/estimators/function_wrapper.py` & `benchmark_mi-0.1.1/src/bmi/estimators/function_wrapper.py`

 * *Files identical despite different names*

### Comparing `benchmark_mi-0.1.0/src/bmi/estimators/ksg.py` & `benchmark_mi-0.1.1/src/bmi/estimators/ksg.py`

 * *Files identical despite different names*

### Comparing `benchmark_mi-0.1.0/src/bmi/estimators/neural/_backend_linear_memory.py` & `benchmark_mi-0.1.1/src/bmi/estimators/neural/_backend_linear_memory.py`

 * *Files identical despite different names*

### Comparing `benchmark_mi-0.1.0/src/bmi/estimators/neural/_backend_quadratic_memory.py` & `benchmark_mi-0.1.1/src/bmi/estimators/neural/_backend_quadratic_memory.py`

 * *Files identical despite different names*

### Comparing `benchmark_mi-0.1.0/src/bmi/estimators/neural/_basic_training.py` & `benchmark_mi-0.1.1/src/bmi/estimators/neural/_basic_training.py`

 * *Files identical despite different names*

### Comparing `benchmark_mi-0.1.0/src/bmi/estimators/neural/_critics.py` & `benchmark_mi-0.1.1/src/bmi/estimators/neural/_critics.py`

 * *Files identical despite different names*

### Comparing `benchmark_mi-0.1.0/src/bmi/estimators/neural/_estimators.py` & `benchmark_mi-0.1.1/src/bmi/estimators/neural/_estimators.py`

 * *Files identical despite different names*

### Comparing `benchmark_mi-0.1.0/src/bmi/estimators/neural/_mine_estimator.py` & `benchmark_mi-0.1.1/src/bmi/estimators/neural/_mine_estimator.py`

 * *Files identical despite different names*

### Comparing `benchmark_mi-0.1.0/src/bmi/estimators/neural/_training_log.py` & `benchmark_mi-0.1.1/src/bmi/estimators/neural/_training_log.py`

 * *Files identical despite different names*

### Comparing `benchmark_mi-0.1.0/src/bmi/interface.py` & `benchmark_mi-0.1.1/src/bmi/interface.py`

 * *Files identical despite different names*

### Comparing `benchmark_mi-0.1.0/src/bmi/plot_utils/subplots_from_axsize.py` & `benchmark_mi-0.1.1/src/bmi/plot_utils/subplots_from_axsize.py`

 * *Files identical despite different names*

### Comparing `benchmark_mi-0.1.0/src/bmi/samplers/__init__.py` & `benchmark_mi-0.1.1/src/bmi/samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `benchmark_mi-0.1.0/src/bmi/samplers/_additive_uniform.py` & `benchmark_mi-0.1.1/src/bmi/samplers/_additive_uniform.py`

 * *Files identical despite different names*

### Comparing `benchmark_mi-0.1.0/src/bmi/samplers/_matrix_utils.py` & `benchmark_mi-0.1.1/src/bmi/samplers/_matrix_utils.py`

 * *Files identical despite different names*

### Comparing `benchmark_mi-0.1.0/src/bmi/samplers/_split_student_t.py` & `benchmark_mi-0.1.1/src/bmi/samplers/_split_student_t.py`

 * *Files identical despite different names*

### Comparing `benchmark_mi-0.1.0/src/bmi/samplers/_splitmultinormal.py` & `benchmark_mi-0.1.1/src/bmi/samplers/_splitmultinormal.py`

 * *Files identical despite different names*

### Comparing `benchmark_mi-0.1.0/src/bmi/samplers/_transformed.py` & `benchmark_mi-0.1.1/src/bmi/samplers/_transformed.py`

 * *Files identical despite different names*

### Comparing `benchmark_mi-0.1.0/src/bmi/samplers/base.py` & `benchmark_mi-0.1.1/src/bmi/samplers/base.py`

 * *Files identical despite different names*

### Comparing `benchmark_mi-0.1.0/src/bmi/transforms/_invert_cdf.py` & `benchmark_mi-0.1.1/src/bmi/transforms/_invert_cdf.py`

 * *Files identical despite different names*

### Comparing `benchmark_mi-0.1.0/src/bmi/transforms/_rotate.py` & `benchmark_mi-0.1.1/src/bmi/transforms/_rotate.py`

 * *Files identical despite different names*

### Comparing `benchmark_mi-0.1.0/src/bmi/transforms/simple.py` & `benchmark_mi-0.1.1/src/bmi/transforms/simple.py`

 * *Files identical despite different names*

### Comparing `benchmark_mi-0.1.0/src/bmi/utils.py` & `benchmark_mi-0.1.1/src/bmi/utils.py`

 * *Files identical despite different names*

### Comparing `benchmark_mi-0.1.0/PKG-INFO` & `benchmark_mi-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: benchmark-mi
-Version: 0.1.0
+Version: 0.1.1
 Summary: Estimators of mutual information and distributions used to benchmark them.
 License: MIT
 Author: Paweł Czyż
 Author-email: pawelpiotr.czyz@ai.ethz.ch
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -21,33 +21,39 @@
 Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
 Description-Content-Type: text/markdown
 
 [![arXiv](https://img.shields.io/badge/arXiv-2306.11078-b31b1b.svg)](https://arxiv.org/abs/2306.11078)
 [![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
+[![PyPI Latest Release](https://img.shields.io/pypi/v/benchmark-mi.svg)](https://pypi.org/project/benchmark-mi/)
 [![build](https://github.com/cbg-ethz/bmi/actions/workflows/build.yml/badge.svg?branch=main)](https://github.com/cbg-ethz/bmi/actions/workflows/build.yml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 # Benchmarking Mutual Information
 
 BMI is the package for estimation of mutual information between continuous random variables and testing new estimators.
 
 - **Documentation**: [https://cbg-ethz.github.io/bmi/](https://cbg-ethz.github.io/bmi/)
 - **Source code**: [https://github.com/cbg-ethz/bmi](https://github.com/cbg-ethz/bmi)
 - **Bug reports**: [https://github.com/cbg-ethz/bmi/issues](https://github.com/cbg-ethz/bmi/issues)
-
+- **PyPI package**: [https://pypi.org/project/benchmark-mi](https://pypi.org/project/benchmark-mi)
 
 ## Getting started
 While we recommend taking a look at the [documentation](https://cbg-ethz.github.io/bmi/) to learn about full package capabilities, below we present the main capabilities of the Python package.
 (Note that BMI can also be used to test non-Python mutual information estimators.)
 
 You can install the package using:
 
-**TODO:** Add installation instructions after we push to PyPI.
+```bash
+$ pip install benchmark-mi
+```
+
+Alternatively, you can use the development version from source using:
+
 ```bash
 $ pip install "bmi @ https://github.com/cbg-ethz/bmi"
 ```
 
 Note: BMI uses [JAX](https://github.com/google/jax) and by default installs the CPU version of it.
 If you have a device supporting CUDA, you can [install the CUDA version of JAX](https://github.com/google/jax#pip-installation-gpu-cuda-installed-via-pip-easier).
```

