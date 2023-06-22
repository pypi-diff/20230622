# Comparing `tmp/jwave-0.1.1.tar.gz` & `tmp/jwave-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jwave-0.1.1.tar", max compression
+gzip compressed data, was "jwave-0.1.2.tar", max compression
```

## Comparing `jwave-0.1.1.tar` & `jwave-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rwxr-xr-x   0        0        0     7652 2023-06-22 13:51:00.238868 jwave-0.1.1/LICENSE
--rwxr-xr-x   0        0        0     4552 2023-06-22 13:51:00.238868 jwave-0.1.1/README.md
--rwxr-xr-x   0        0        0       19 2023-06-22 13:51:00.282869 jwave-0.1.1/jwave/__about__.py
--rwxr-xr-x   0        0        0      885 2023-06-22 13:51:00.282869 jwave-0.1.1/jwave/__init__.py
--rw-r--r--   0        0        0      768 2023-06-22 13:51:00.282869 jwave-0.1.1/jwave/acoustics/__init__.py
--rw-r--r--   0        0        0     1951 2023-06-22 13:51:00.282869 jwave-0.1.1/jwave/acoustics/conversion.py
--rw-r--r--   0        0        0    10119 2023-06-22 13:51:00.282869 jwave-0.1.1/jwave/acoustics/operators.py
--rw-r--r--   0        0        0     4561 2023-06-22 13:51:00.282869 jwave-0.1.1/jwave/acoustics/pml.py
--rwxr-xr-x   0        0        0     1186 2023-06-22 13:51:00.282869 jwave-0.1.1/jwave/acoustics/spectral.py
--rw-r--r--   0        0        0    20569 2023-06-22 13:51:00.282869 jwave-0.1.1/jwave/acoustics/time_harmonic.py
--rwxr-xr-x   0        0        0    19105 2023-06-22 13:51:00.282869 jwave-0.1.1/jwave/acoustics/time_varying.py
--rw-r--r--   0        0        0       85 2023-06-22 13:51:00.282869 jwave-0.1.1/jwave/extras/__init__.py
--rw-r--r--   0        0        0     2899 2023-06-22 13:51:00.282869 jwave-0.1.1/jwave/extras/export.py
--rwxr-xr-x   0        0        0    15953 2023-06-22 13:51:00.282869 jwave-0.1.1/jwave/geometry.py
--rwxr-xr-x   0        0        0     1423 2023-06-22 13:51:00.282869 jwave-0.1.1/jwave/phantoms.py
--rwxr-xr-x   0        0        0     8798 2023-06-22 13:51:00.282869 jwave-0.1.1/jwave/signal_processing.py
--rw-r--r--   0        0        0      835 2023-06-22 13:51:00.282869 jwave-0.1.1/jwave/transformations.py
--rwxr-xr-x   0        0        0     6265 2023-06-22 13:51:00.282869 jwave-0.1.1/jwave/utils.py
--rw-r--r--   0        0        0     2988 2023-06-22 13:51:00.282869 jwave-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     6331 1970-01-01 00:00:00.000000 jwave-0.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0     7652 2023-06-22 15:50:58.991539 jwave-0.1.2/LICENSE
+-rwxr-xr-x   0        0        0     4467 2023-06-22 15:50:58.991539 jwave-0.1.2/README.md
+-rwxr-xr-x   0        0        0       19 2023-06-22 15:50:59.027540 jwave-0.1.2/jwave/__about__.py
+-rwxr-xr-x   0        0        0      885 2023-06-22 15:50:59.027540 jwave-0.1.2/jwave/__init__.py
+-rw-r--r--   0        0        0      768 2023-06-22 15:50:59.027540 jwave-0.1.2/jwave/acoustics/__init__.py
+-rw-r--r--   0        0        0     1951 2023-06-22 15:50:59.027540 jwave-0.1.2/jwave/acoustics/conversion.py
+-rw-r--r--   0        0        0    10119 2023-06-22 15:50:59.027540 jwave-0.1.2/jwave/acoustics/operators.py
+-rw-r--r--   0        0        0     4561 2023-06-22 15:50:59.027540 jwave-0.1.2/jwave/acoustics/pml.py
+-rwxr-xr-x   0        0        0     1186 2023-06-22 15:50:59.027540 jwave-0.1.2/jwave/acoustics/spectral.py
+-rw-r--r--   0        0        0    20569 2023-06-22 15:50:59.027540 jwave-0.1.2/jwave/acoustics/time_harmonic.py
+-rwxr-xr-x   0        0        0    19105 2023-06-22 15:50:59.027540 jwave-0.1.2/jwave/acoustics/time_varying.py
+-rw-r--r--   0        0        0       85 2023-06-22 15:50:59.027540 jwave-0.1.2/jwave/extras/__init__.py
+-rw-r--r--   0        0        0     3029 2023-06-22 15:50:59.027540 jwave-0.1.2/jwave/extras/export.py
+-rwxr-xr-x   0        0        0    15953 2023-06-22 15:50:59.027540 jwave-0.1.2/jwave/geometry.py
+-rwxr-xr-x   0        0        0     1423 2023-06-22 15:50:59.027540 jwave-0.1.2/jwave/phantoms.py
+-rwxr-xr-x   0        0        0     8798 2023-06-22 15:50:59.027540 jwave-0.1.2/jwave/signal_processing.py
+-rw-r--r--   0        0        0      835 2023-06-22 15:50:59.027540 jwave-0.1.2/jwave/transformations.py
+-rwxr-xr-x   0        0        0     6265 2023-06-22 15:50:59.027540 jwave-0.1.2/jwave/utils.py
+-rw-r--r--   0        0        0     2944 2023-06-22 15:50:59.027540 jwave-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     6246 1970-01-01 00:00:00.000000 jwave-0.1.2/PKG-INFO
```

### Comparing `jwave-0.1.1/LICENSE` & `jwave-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jwave-0.1.1/README.md` & `jwave-0.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -4,44 +4,44 @@
 
 # j-Wave: Differentiable acoustic simulations in JAX
 
 [![Support](https://dcbadge.vercel.app/api/server/VtUb4fFznt?style=flat)](https://discord.gg/VtUb4fFznt)
 [![License: LGPL v3](https://img.shields.io/badge/License-LGPL_v3-blue.svg)](LICENSE)
 [![Continous Integration](https://github.com/ucl-bug/jwave/actions/workflows/tests.yml/badge.svg)](https://github.com/ucl-bug/jwave/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/gh/ucl-bug/jwave/branch/main/graph/badge.svg?token=6J03OMVJS1)](https://codecov.io/gh/ucl-bug/jwave)
-[![Documentation](https://github.com/ucl-bug/jwave/actions/workflows/build_docs.yml/badge.svg)](https://ucl-bug.github.io/jwave)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ucl-bug/jwave/main?labpath=docs%2Fnotebooks%2Fivp%2Fhomogeneous_medium.ipynb)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1xAHAognF1v9un6GNvaGPSfdVeCDK8l9z?usp=sharing)
 
 [Install](#install) | [Tutorials](https://ucl-bug.github.io/jwave/notebooks/ivp/homogeneous_medium.html) | [Documentation](https://ucl-bug.github.io/jwave) | [Changelog](HISTORY.md)
 
-j-Wave is a library of simulators for acoustic applications. Is heavily inspired by [k-Wave](http://www.k-wave.org/) (a big portion of j-Wave is a port of k-Wave in JAX), and its intented to be used as a collection of modular blocks that can be easily included into any machine learning pipeline.
+j-Wave is a library of simulators for acoustic applications. It is heavily inspired by [k-Wave](http://www.k-wave.org/)—a substantial portion of j-Wave is a port of k-Wave in JAX—and it's intended to be used as a collection of modular blocks that can be easily incorporated into any machine learning pipeline.
 
-Following the phylosophy of [JAX](https://jax.readthedocs.io/en/stable/), j-Wave is developed with the following principles in mind
+Embracing the philosophy of [JAX](https://jax.readthedocs.io/en/stable/), j-Wave is developed with the following principles in mind:
+
+1. To be differentiable
+2. To be efficient through `jit` compilation
+3. To be easily run on GPUs
+4. To be easily customizable
 
-1. To be differntiable
-2. To be fast via `jit` compilation
-3. Easy to run on GPUs
-4. Easy to customize
 
 <br/>
 
 ## Install
 
-Follow the instructions to install [Jax with CUDA support](https://github.com/google/jax#installation) if you want to use your GPU.
+Follow the instructions to install [Jax with CUDA support](https://github.com/google/jax#installation) if you wish to use your GPU.
 
-Then, simply install `jwave` using pip
+Next, simply install `jwave` using pip:
 
 ```bash
-pip install git+https://github.com/ucl-bug/jwave.git
+pip install jwave
 ```
 
-For more details, see the [Linux install guide](docs/install/on_linux.md).
+For more information, refer to the [Linux installation guide](docs/install/on_linux.md).
 
-Because JAX has limited support on Windows, j-Wave can be run on Windows machines only using the Windows Subsystem for Linux. See the [Install on Windows](docs/install/on_win.md) guide for more details.
+Due to JAX's limited support on Windows, j-Wave can only be run on Windows machines using the Windows Subsystem for Linux. Please refer to the [Installation on Windows guide](docs/install/on_win.md) for more details.
 
 <br/>
 
 ## Example
 
 This example simulates an acoustic initial value problem, which is often used as a simple model for photoacoustic acquisitions:
 
@@ -74,15 +74,15 @@
 ![Simulated pressure field](docs/assets/images/readme_example_reconimage.png)
 
 
 ## Support
 
 [![Support](https://dcbadge.vercel.app/api/server/VtUb4fFznt?style=flat)](https://discord.gg/VtUb4fFznt)
 
-If you find some problems in the code or want to propose some new features, feel free to open an issue. If you generally would like to have some guidance, discuss something, or just say hi, feel free to write a message in the [Discord channel](https://discord.gg/VtUb4fFznt).
+If you encounter any problems with the code or wish to propose new features, please feel free to open an issue. If you need general guidance, wish to discuss something, or just want to say hi, don't hesitate to leave a message in our [Discord channel](https://discord.gg/VtUb4fFznt).
 
 <br/>
 
 ## Citation
 
 [![arXiv](https://img.shields.io/badge/arXiv-2207.01499-b31b1b.svg?style=flat)](https://arxiv.org/abs/2207.01499)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `jwave-0.1.1/jwave/__init__.py` & `jwave-0.1.2/jwave/__init__.py`

 * *Files identical despite different names*

### Comparing `jwave-0.1.1/jwave/acoustics/__init__.py` & `jwave-0.1.2/jwave/acoustics/__init__.py`

 * *Files identical despite different names*

### Comparing `jwave-0.1.1/jwave/acoustics/conversion.py` & `jwave-0.1.2/jwave/acoustics/conversion.py`

 * *Files identical despite different names*

### Comparing `jwave-0.1.1/jwave/acoustics/operators.py` & `jwave-0.1.2/jwave/acoustics/operators.py`

 * *Files identical despite different names*

### Comparing `jwave-0.1.1/jwave/acoustics/pml.py` & `jwave-0.1.2/jwave/acoustics/pml.py`

 * *Files identical despite different names*

### Comparing `jwave-0.1.1/jwave/acoustics/spectral.py` & `jwave-0.1.2/jwave/acoustics/spectral.py`

 * *Files identical despite different names*

### Comparing `jwave-0.1.1/jwave/acoustics/time_harmonic.py` & `jwave-0.1.2/jwave/acoustics/time_harmonic.py`

 * *Files identical despite different names*

### Comparing `jwave-0.1.1/jwave/acoustics/time_varying.py` & `jwave-0.1.2/jwave/acoustics/time_varying.py`

 * *Files identical despite different names*

### Comparing `jwave-0.1.1/jwave/extras/export.py` & `jwave-0.1.2/jwave/extras/export.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,18 +11,23 @@
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with j-Wave. If not, see <https://www.gnu.org/licenses/>.
 
 import os
 
-import imageio
+try:
+    import imageio
+    from tqdm import trange
+except ImportError:
+    raise ImportError(
+        "Please install imageio and tqdm to use use the extras module.")
+
 import matplotlib.pyplot as plt
 from jaxdf import Field
-from tqdm import trange
 
 
 def save_video(
     fields: Field,
     filename: str,
     fps=30,
     vmin=None,
```

### Comparing `jwave-0.1.1/jwave/geometry.py` & `jwave-0.1.2/jwave/geometry.py`

 * *Files identical despite different names*

### Comparing `jwave-0.1.1/jwave/phantoms.py` & `jwave-0.1.2/jwave/phantoms.py`

 * *Files identical despite different names*

### Comparing `jwave-0.1.1/jwave/signal_processing.py` & `jwave-0.1.2/jwave/signal_processing.py`

 * *Files identical despite different names*

### Comparing `jwave-0.1.1/jwave/transformations.py` & `jwave-0.1.2/jwave/transformations.py`

 * *Files identical despite different names*

### Comparing `jwave-0.1.1/jwave/utils.py` & `jwave-0.1.2/jwave/utils.py`

 * *Files identical despite different names*

### Comparing `jwave-0.1.1/pyproject.toml` & `jwave-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jwave"
-version = "0.1.1"
+version = "0.1.2"
 description = "Fast and differentiable acoustic simulations in JAX."
 authors = [
   "Antonio Stanziola <a.stanziola@ucl.ac.uk>",
   "Simon Arridge",
   "Ben T. Cox",
   "Bradley E. Treeby",
 ]
@@ -52,29 +52,31 @@
 [tool.poetry.dependencies]
 python = "^3.9"
 jaxdf = "^0.2.4"
 matplotlib = "^3.0.0"
 
 [tool.poetry.group.dev.dependencies]
 coverage = "7.0.4"
-flake8 = "5.0.4"
 pytest = "^7.2.0"
 pre-commit = "^2.20.0"
-pycln = "2.1.1"
+pycln = "^2.1.5"
 isort = "^5.12.0"
-griffe = "^0.24.0"
+griffe = "^0.29.1"
 mkdocs-material = "^9.1.16"
 mkdocstrings = "^0.22.0"
 mkdocs-jupyter = "^0.24.1"
 mkdocs-macros-plugin = "^0.7.0"
 mkdocs-mermaid2-plugin = "^0.6.0"
 mkdocstrings-python = "^0.8.0"
 python-kacl = "^0.4.6"
 pymdown-extensions = "^10.0.1"
 plumkdocs = "0.0.2"
+imageio = "^2.31.1"
+tqdm = "^4.65.0"
+imageio-ffmpeg = "^0.4.8"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tools.isort]
 src_paths = ["jwave", "tests"]
@@ -103,18 +105,14 @@
 [tool.yapf]
 based_on_style = "pep8"
 spaces_before_comment = 4
 split_before_logical_operator = true
 
 [tool.pytest.ini_options]
 addopts = """\
-    --cov jwave \
-    --cov tests \
-    --cov-report term-missing \
-    --no-cov-on-fail \
     --doctest-modules \
 """
 
 [tool.coverage.report]
 exclude_lines = [
     'if TYPE_CHECKING:',
     'pragma: no cover'
```

### Comparing `jwave-0.1.1/PKG-INFO` & `jwave-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jwave
-Version: 0.1.1
+Version: 0.1.2
 Summary: Fast and differentiable acoustic simulations in JAX.
 License: LGPL-3.0-only
 Keywords: jax,acoustics,simulation,ultrasound,differentiable-programming
 Author: Antonio Stanziola
 Author-email: a.stanziola@ucl.ac.uk
 Requires-Python: >=3.9,<4.0
 Classifier: Environment :: GPU
@@ -42,44 +42,44 @@
 
 # j-Wave: Differentiable acoustic simulations in JAX
 
 [![Support](https://dcbadge.vercel.app/api/server/VtUb4fFznt?style=flat)](https://discord.gg/VtUb4fFznt)
 [![License: LGPL v3](https://img.shields.io/badge/License-LGPL_v3-blue.svg)](LICENSE)
 [![Continous Integration](https://github.com/ucl-bug/jwave/actions/workflows/tests.yml/badge.svg)](https://github.com/ucl-bug/jwave/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/gh/ucl-bug/jwave/branch/main/graph/badge.svg?token=6J03OMVJS1)](https://codecov.io/gh/ucl-bug/jwave)
-[![Documentation](https://github.com/ucl-bug/jwave/actions/workflows/build_docs.yml/badge.svg)](https://ucl-bug.github.io/jwave)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ucl-bug/jwave/main?labpath=docs%2Fnotebooks%2Fivp%2Fhomogeneous_medium.ipynb)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1xAHAognF1v9un6GNvaGPSfdVeCDK8l9z?usp=sharing)
 
 [Install](#install) | [Tutorials](https://ucl-bug.github.io/jwave/notebooks/ivp/homogeneous_medium.html) | [Documentation](https://ucl-bug.github.io/jwave) | [Changelog](HISTORY.md)
 
-j-Wave is a library of simulators for acoustic applications. Is heavily inspired by [k-Wave](http://www.k-wave.org/) (a big portion of j-Wave is a port of k-Wave in JAX), and its intented to be used as a collection of modular blocks that can be easily included into any machine learning pipeline.
+j-Wave is a library of simulators for acoustic applications. It is heavily inspired by [k-Wave](http://www.k-wave.org/)—a substantial portion of j-Wave is a port of k-Wave in JAX—and it's intended to be used as a collection of modular blocks that can be easily incorporated into any machine learning pipeline.
 
-Following the phylosophy of [JAX](https://jax.readthedocs.io/en/stable/), j-Wave is developed with the following principles in mind
+Embracing the philosophy of [JAX](https://jax.readthedocs.io/en/stable/), j-Wave is developed with the following principles in mind:
+
+1. To be differentiable
+2. To be efficient through `jit` compilation
+3. To be easily run on GPUs
+4. To be easily customizable
 
-1. To be differntiable
-2. To be fast via `jit` compilation
-3. Easy to run on GPUs
-4. Easy to customize
 
 <br/>
 
 ## Install
 
-Follow the instructions to install [Jax with CUDA support](https://github.com/google/jax#installation) if you want to use your GPU.
+Follow the instructions to install [Jax with CUDA support](https://github.com/google/jax#installation) if you wish to use your GPU.
 
-Then, simply install `jwave` using pip
+Next, simply install `jwave` using pip:
 
 ```bash
-pip install git+https://github.com/ucl-bug/jwave.git
+pip install jwave
 ```
 
-For more details, see the [Linux install guide](docs/install/on_linux.md).
+For more information, refer to the [Linux installation guide](docs/install/on_linux.md).
 
-Because JAX has limited support on Windows, j-Wave can be run on Windows machines only using the Windows Subsystem for Linux. See the [Install on Windows](docs/install/on_win.md) guide for more details.
+Due to JAX's limited support on Windows, j-Wave can only be run on Windows machines using the Windows Subsystem for Linux. Please refer to the [Installation on Windows guide](docs/install/on_win.md) for more details.
 
 <br/>
 
 ## Example
 
 This example simulates an acoustic initial value problem, which is often used as a simple model for photoacoustic acquisitions:
 
@@ -112,15 +112,15 @@
 ![Simulated pressure field](docs/assets/images/readme_example_reconimage.png)
 
 
 ## Support
 
 [![Support](https://dcbadge.vercel.app/api/server/VtUb4fFznt?style=flat)](https://discord.gg/VtUb4fFznt)
 
-If you find some problems in the code or want to propose some new features, feel free to open an issue. If you generally would like to have some guidance, discuss something, or just say hi, feel free to write a message in the [Discord channel](https://discord.gg/VtUb4fFznt).
+If you encounter any problems with the code or wish to propose new features, please feel free to open an issue. If you need general guidance, wish to discuss something, or just want to say hi, don't hesitate to leave a message in our [Discord channel](https://discord.gg/VtUb4fFznt).
 
 <br/>
 
 ## Citation
 
 [![arXiv](https://img.shields.io/badge/arXiv-2207.01499-b31b1b.svg?style=flat)](https://arxiv.org/abs/2207.01499)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

