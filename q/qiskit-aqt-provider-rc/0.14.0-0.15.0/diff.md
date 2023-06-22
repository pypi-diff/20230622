# Comparing `tmp/qiskit_aqt_provider_rc-0.14.0.tar.gz` & `tmp/qiskit_aqt_provider_rc-0.15.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit_aqt_provider_rc-0.14.0.tar", max compression
+gzip compressed data, was "qiskit_aqt_provider_rc-0.15.0.tar", max compression
```

## Comparing `qiskit_aqt_provider_rc-0.14.0.tar` & `qiskit_aqt_provider_rc-0.15.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     3214 2023-05-30 14:32:41.750526 qiskit_aqt_provider_rc-0.14.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0    14035 2023-05-30 14:32:41.750526 qiskit_aqt_provider_rc-0.14.0/CONTRIBUTING.md
--rw-r--r--   0        0        0    11416 2023-05-30 14:32:41.750526 qiskit_aqt_provider_rc-0.14.0/LICENSE.txt
--rw-r--r--   0        0        0     1467 2023-05-30 14:32:41.750526 qiskit_aqt_provider_rc-0.14.0/README.md
--rw-r--r--   0        0        0     6143 2023-05-30 14:32:41.754526 qiskit_aqt_provider_rc-0.14.0/pyproject.toml
--rw-r--r--   0        0        0      562 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/__init__.py
--rw-r--r--   0        0        0     8241 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/api_models.py
--rw-r--r--   0        0        0    12734 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/api_models_generated.py
--rw-r--r--   0        0        0    16481 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/aqt_job.py
--rw-r--r--   0        0        0     2704 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/aqt_options.py
--rw-r--r--   0        0        0     8826 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/aqt_provider.py
--rw-r--r--   0        0        0    12462 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/aqt_resource.py
--rw-r--r--   0        0        0     3425 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/circuit_to_aqt.py
--rw-r--r--   0        0        0      564 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/primitives/__init__.py
--rw-r--r--   0        0        0     2476 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/primitives/estimator.py
--rw-r--r--   0        0        0     2286 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/primitives/sampler.py
--rw-r--r--   0        0        0        0 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/py.typed
--rw-r--r--   0        0        0      587 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/test/__init__.py
--rw-r--r--   0        0        0     1884 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/test/circuits.py
--rw-r--r--   0        0        0     2703 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/test/fixtures.py
--rw-r--r--   0        0        0     6970 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/test/resources.py
--rw-r--r--   0        0        0     1259 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/test/timeout.py
--rw-r--r--   0        0        0     7323 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/transpiler_plugin.py
--rw-r--r--   0        0        0     1838 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/utils.py
--rw-r--r--   0        0        0     1040 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/versions.py
--rw-r--r--   0        0        0        0 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/test/__init__.py
--rw-r--r--   0        0        0     3822 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/test/test_api_models.py
--rw-r--r--   0        0        0     6142 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/test/test_circuit_to_aqt.py
--rw-r--r--   0        0        0    13208 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/test/test_execution.py
--rw-r--r--   0        0        0     2121 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/test/test_options.py
--rw-r--r--   0        0        0     6603 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/test/test_primitives.py
--rw-r--r--   0        0        0     5139 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/test/test_provider.py
--rw-r--r--   0        0        0    11103 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/test/test_resource.py
--rw-r--r--   0        0        0     8668 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/test/test_transpilation.py
--rw-r--r--   0        0        0     1063 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/test/test_utils.py
--rw-r--r--   0        0        0     3071 1970-01-01 00:00:00.000000 qiskit_aqt_provider_rc-0.14.0/PKG-INFO
+-rw-r--r--   0        0        0     3214 2023-06-22 14:50:37.327675 qiskit_aqt_provider_rc-0.15.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0    14035 2023-06-22 14:50:37.327675 qiskit_aqt_provider_rc-0.15.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11416 2023-06-22 14:50:37.327675 qiskit_aqt_provider_rc-0.15.0/LICENSE.txt
+-rw-r--r--   0        0        0     1467 2023-06-22 14:50:37.327675 qiskit_aqt_provider_rc-0.15.0/README.md
+-rw-r--r--   0        0        0     6144 2023-06-22 14:50:37.331675 qiskit_aqt_provider_rc-0.15.0/pyproject.toml
+-rw-r--r--   0        0        0      562 2023-06-22 14:50:37.331675 qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/__init__.py
+-rw-r--r--   0        0        0     8241 2023-06-22 14:50:37.331675 qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/api_models.py
+-rw-r--r--   0        0        0    12734 2023-06-22 14:50:37.331675 qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/api_models_generated.py
+-rw-r--r--   0        0        0    16481 2023-06-22 14:50:37.331675 qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/aqt_job.py
+-rw-r--r--   0        0        0     2704 2023-06-22 14:50:37.331675 qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/aqt_options.py
+-rw-r--r--   0        0        0     8824 2023-06-22 14:50:37.331675 qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/aqt_provider.py
+-rw-r--r--   0        0        0    12462 2023-06-22 14:50:37.331675 qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/aqt_resource.py
+-rw-r--r--   0        0        0     3425 2023-06-22 14:50:37.331675 qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/circuit_to_aqt.py
+-rw-r--r--   0        0        0      564 2023-06-22 14:50:37.331675 qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/primitives/__init__.py
+-rw-r--r--   0        0        0     2476 2023-06-22 14:50:37.331675 qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/primitives/estimator.py
+-rw-r--r--   0        0        0     2286 2023-06-22 14:50:37.331675 qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/primitives/sampler.py
+-rw-r--r--   0        0        0        0 2023-06-22 14:50:37.331675 qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/py.typed
+-rw-r--r--   0        0        0      587 2023-06-22 14:50:37.331675 qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/test/__init__.py
+-rw-r--r--   0        0        0     1884 2023-06-22 14:50:37.331675 qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/test/circuits.py
+-rw-r--r--   0        0        0     2703 2023-06-22 14:50:37.331675 qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/test/fixtures.py
+-rw-r--r--   0        0        0     6970 2023-06-22 14:50:37.331675 qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/test/resources.py
+-rw-r--r--   0        0        0     1259 2023-06-22 14:50:37.331675 qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/test/timeout.py
+-rw-r--r--   0        0        0     7323 2023-06-22 14:50:37.331675 qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/transpiler_plugin.py
+-rw-r--r--   0        0        0     1838 2023-06-22 14:50:37.331675 qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/utils.py
+-rw-r--r--   0        0        0     1040 2023-06-22 14:50:37.331675 qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/versions.py
+-rw-r--r--   0        0        0        0 2023-06-22 14:50:37.331675 qiskit_aqt_provider_rc-0.15.0/test/__init__.py
+-rw-r--r--   0        0        0     3822 2023-06-22 14:50:37.331675 qiskit_aqt_provider_rc-0.15.0/test/test_api_models.py
+-rw-r--r--   0        0        0     6142 2023-06-22 14:50:37.331675 qiskit_aqt_provider_rc-0.15.0/test/test_circuit_to_aqt.py
+-rw-r--r--   0        0        0    13208 2023-06-22 14:50:37.331675 qiskit_aqt_provider_rc-0.15.0/test/test_execution.py
+-rw-r--r--   0        0        0     2121 2023-06-22 14:50:37.331675 qiskit_aqt_provider_rc-0.15.0/test/test_options.py
+-rw-r--r--   0        0        0     6630 2023-06-22 14:50:37.331675 qiskit_aqt_provider_rc-0.15.0/test/test_primitives.py
+-rw-r--r--   0        0        0     5139 2023-06-22 14:50:37.331675 qiskit_aqt_provider_rc-0.15.0/test/test_provider.py
+-rw-r--r--   0        0        0    11103 2023-06-22 14:50:37.335675 qiskit_aqt_provider_rc-0.15.0/test/test_resource.py
+-rw-r--r--   0        0        0     8668 2023-06-22 14:50:37.335675 qiskit_aqt_provider_rc-0.15.0/test/test_transpilation.py
+-rw-r--r--   0        0        0     1063 2023-06-22 14:50:37.335675 qiskit_aqt_provider_rc-0.15.0/test/test_utils.py
+-rw-r--r--   0        0        0     2921 1970-01-01 00:00:00.000000 qiskit_aqt_provider_rc-0.15.0/PKG-INFO
```

### Comparing `qiskit_aqt_provider_rc-0.14.0/CODE_OF_CONDUCT.md` & `qiskit_aqt_provider_rc-0.15.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.14.0/CONTRIBUTING.md` & `qiskit_aqt_provider_rc-0.15.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.14.0/LICENSE.txt` & `qiskit_aqt_provider_rc-0.15.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.14.0/README.md` & `qiskit_aqt_provider_rc-0.15.0/README.md`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.14.0/pyproject.toml` & `qiskit_aqt_provider_rc-0.15.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qiskit-aqt-provider-rc"
-version = "0.14.0"
+version = "0.15.0"
 description = "Qiskit provider for AQT backends"
 authors = ["Qiskit Development Team", "Alpine Quantum Technologies GmbH"]
 repository = "https://github.com/alpine-quantum-technologies/qiskit-aqt-provider-rc/"
 readme = "README.md"
 license = "Apache-2.0"
 classifiers=[
         "Intended Audience :: Developers",
@@ -38,21 +38,21 @@
 [tool.poetry.plugins."qiskit.transpiler.translation"]
 aqt = "qiskit_aqt_provider.transpiler_plugin:AQTTranslationPlugin"
 
 [tool.poetry.plugins.pytest11]
 pytest_qiskit_aqt = "qiskit_aqt_provider.test.fixtures"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.11"
+python = ">=3.8,<3.12"
 
 httpx = ">=0.24.0"
 pydantic = ">=1.10.8,<2"
 python-dotenv = ">=1"
 qiskit-aer = ">=0.11"
-qiskit-terra = ">=0.23.3,<0.24.0"
+qiskit-terra = ">=0.23.3,!=0.24.0"
 tabulate = ">=0.9.0"
 tqdm = ">=4"
 tweedledum = { version = ">=1", optional = true }
 typing-extensions = ">=4.0.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
```

### Comparing `qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/__init__.py` & `qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/api_models.py` & `qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/api_models.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/api_models_generated.py` & `qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/api_models_generated.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/aqt_job.py` & `qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/aqt_job.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/aqt_options.py` & `qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/aqt_options.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/aqt_provider.py` & `qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/aqt_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,15 @@
 
     where `'MY_TOKEN'` is the access token provided by AQT.
 
     If no token is given, it is read from the `AQT_TOKEN` environment variable.
     """
 
     # Set AQT_PORTAL_URL environment variable to override
-    DEFAULT_PORTAL_URL: Final = "http://arnica.internal.aqt.eu"
+    DEFAULT_PORTAL_URL: Final = "https://arnica-stage.aqt.eu"
 
     def __init__(
         self,
         access_token: Optional[str] = None,
         *,
         load_dotenv: bool = True,
         dotenv_path: Optional[StrPath] = None,
```

### Comparing `qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/aqt_resource.py` & `qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/aqt_resource.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/circuit_to_aqt.py` & `qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/circuit_to_aqt.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/primitives/__init__.py` & `qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/primitives/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/primitives/estimator.py` & `qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/primitives/estimator.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/primitives/sampler.py` & `qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/primitives/sampler.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/test/__init__.py` & `qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/test/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/test/circuits.py` & `qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/test/circuits.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/test/fixtures.py` & `qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/test/fixtures.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/test/resources.py` & `qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/test/resources.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/test/timeout.py` & `qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/test/timeout.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/transpiler_plugin.py` & `qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/transpiler_plugin.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/utils.py` & `qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/versions.py` & `qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/versions.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.14.0/test/test_api_models.py` & `qiskit_aqt_provider_rc-0.15.0/test/test_api_models.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.14.0/test/test_circuit_to_aqt.py` & `qiskit_aqt_provider_rc-0.15.0/test/test_circuit_to_aqt.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.14.0/test/test_execution.py` & `qiskit_aqt_provider_rc-0.15.0/test/test_execution.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.14.0/test/test_options.py` & `qiskit_aqt_provider_rc-0.15.0/test/test_options.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.14.0/test/test_primitives.py` & `qiskit_aqt_provider_rc-0.15.0/test/test_primitives.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,17 @@
 from qiskit_aqt_provider.test.fixtures import MockSimulator
 
 
 @pytest.mark.skipif(
     importlib.metadata.version("qiskit-terra") >= "0.24.0",
     reason="qiskit.opflow is deprecated in qiskit-terra>=0.24",
 )
-def test_circuit_sampling_opflow(offline_simulator_no_noise: AQTResource) -> None:
+def test_circuit_sampling_opflow(
+    offline_simulator_no_noise: AQTResource,
+) -> None:  # pragma: no cover
     """Check that an `AQTResource` can be used as backend for the legacy
     `opflow.CircuitSampler` with parametric circuits.
     """
     from qiskit.opflow import CircuitSampler, StateFn
 
     theta = Parameter("θ")
```

### Comparing `qiskit_aqt_provider_rc-0.14.0/test/test_provider.py` & `qiskit_aqt_provider_rc-0.15.0/test/test_provider.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.14.0/test/test_resource.py` & `qiskit_aqt_provider_rc-0.15.0/test/test_resource.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.14.0/test/test_transpilation.py` & `qiskit_aqt_provider_rc-0.15.0/test/test_transpilation.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.14.0/test/test_utils.py` & `qiskit_aqt_provider_rc-0.15.0/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.14.0/PKG-INFO` & `qiskit_aqt_provider_rc-0.15.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 Metadata-Version: 2.1
 Name: qiskit-aqt-provider-rc
-Version: 0.14.0
+Version: 0.15.0
 Summary: Qiskit provider for AQT backends
 Home-page: https://github.com/alpine-quantum-technologies/qiskit-aqt-provider-rc/
 License: Apache-2.0
 Keywords: qiskit,sdk,quantum
 Author: Qiskit Development Team
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8,<3.12
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering
 Provides-Extra: examples
 Requires-Dist: httpx (>=0.24.0)
 Requires-Dist: pydantic (>=1.10.8,<2)
 Requires-Dist: python-dotenv (>=1)
 Requires-Dist: qiskit-aer (>=0.11)
-Requires-Dist: qiskit-terra (>=0.23.3,<0.24.0)
+Requires-Dist: qiskit-terra (>=0.23.3,!=0.24.0)
 Requires-Dist: tabulate (>=0.9.0)
 Requires-Dist: tqdm (>=4)
 Requires-Dist: tweedledum (>=1) ; extra == "examples"
 Requires-Dist: typing-extensions (>=4.0.0)
 Project-URL: Repository, https://github.com/alpine-quantum-technologies/qiskit-aqt-provider-rc/
 Description-Content-Type: text/markdown
```

