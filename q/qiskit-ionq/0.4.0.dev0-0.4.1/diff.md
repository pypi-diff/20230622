# Comparing `tmp/qiskit-ionq-0.4.0.dev0.tar.gz` & `tmp/qiskit-ionq-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit-ionq-0.4.0.dev0.tar", last modified: Tue Apr 18 19:43:54 2023, max compression
+gzip compressed data, was "qiskit-ionq-0.4.1.tar", last modified: Thu Jun 22 04:34:28 2023, max compression
```

## Comparing `qiskit-ionq-0.4.0.dev0.tar` & `qiskit-ionq-0.4.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:43:54.583224 qiskit-ionq-0.4.0.dev0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:43:54.579224 qiskit-ionq-0.4.0.dev0/.eggs/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-18 19:43:53.000000 qiskit-ionq-0.4.0.dev0/.eggs/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:43:54.575224 qiskit-ionq-0.4.0.dev0/.eggs/pytest_runner-6.0.0-py3.9.egg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:43:54.579224 qiskit-ionq-0.4.0.dev0/.eggs/pytest_runner-6.0.0-py3.9.egg/EGG-INFO/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-18 19:43:54.000000 qiskit-ionq-0.4.0.dev0/.eggs/pytest_runner-6.0.0-py3.9.egg/EGG-INFO/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-18 19:43:54.000000 qiskit-ionq-0.4.0.dev0/.eggs/pytest_runner-6.0.0-py3.9.egg/EGG-INFO/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-18 19:43:54.000000 qiskit-ionq-0.4.0.dev0/.eggs/pytest_runner-6.0.0-py3.9.egg/EGG-INFO/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-04-18 19:43:45.000000 qiskit-ionq-0.4.0.dev0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-18 19:43:45.000000 qiskit-ionq-0.4.0.dev0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-04-18 19:43:54.583224 qiskit-ionq-0.4.0.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-04-18 19:43:45.000000 qiskit-ionq-0.4.0.dev0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-18 19:43:45.000000 qiskit-ionq-0.4.0.dev0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:43:54.579224 qiskit-ionq-0.4.0.dev0/qiskit_ionq/
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-18 19:43:45.000000 qiskit-ionq-0.4.0.dev0/qiskit_ionq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-04-18 19:43:45.000000 qiskit-ionq-0.4.0.dev0/qiskit_ionq/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     9123 2023-04-18 19:43:45.000000 qiskit-ionq-0.4.0.dev0/qiskit_ionq/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15179 2023-04-18 19:43:45.000000 qiskit-ionq-0.4.0.dev0/qiskit_ionq/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14014 2023-04-18 19:43:45.000000 qiskit-ionq-0.4.0.dev0/qiskit_ionq/ionq_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     7688 2023-04-18 19:43:45.000000 qiskit-ionq-0.4.0.dev0/qiskit_ionq/ionq_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-04-18 19:43:45.000000 qiskit-ionq-0.4.0.dev0/qiskit_ionq/ionq_gates.py
--rw-r--r--   0 runner    (1001) docker     (123)    16098 2023-04-18 19:43:45.000000 qiskit-ionq-0.4.0.dev0/qiskit_ionq/ionq_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-04-18 19:43:45.000000 qiskit-ionq-0.4.0.dev0/qiskit_ionq/ionq_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-04-18 19:43:45.000000 qiskit-ionq-0.4.0.dev0/qiskit_ionq/ionq_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-04-18 19:43:45.000000 qiskit-ionq-0.4.0.dev0/qiskit_ionq/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:43:54.583224 qiskit-ionq-0.4.0.dev0/qiskit_ionq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-04-18 19:43:54.000000 qiskit-ionq-0.4.0.dev0/qiskit_ionq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-18 19:43:54.000000 qiskit-ionq-0.4.0.dev0/qiskit_ionq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 19:43:54.000000 qiskit-ionq-0.4.0.dev0/qiskit_ionq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 19:43:54.000000 qiskit-ionq-0.4.0.dev0/qiskit_ionq.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-18 19:43:54.000000 qiskit-ionq-0.4.0.dev0/qiskit_ionq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 19:43:54.000000 qiskit-ionq-0.4.0.dev0/qiskit_ionq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-18 19:43:45.000000 qiskit-ionq-0.4.0.dev0/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-18 19:43:45.000000 qiskit-ionq-0.4.0.dev0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-18 19:43:45.000000 qiskit-ionq-0.4.0.dev0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-18 19:43:54.583224 qiskit-ionq-0.4.0.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-04-18 19:43:45.000000 qiskit-ionq-0.4.0.dev0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:43:54.583224 qiskit-ionq-0.4.0.dev0/test/
--rw-r--r--   0 runner    (1001) docker     (123)    10551 2023-04-18 19:43:45.000000 qiskit-ionq-0.4.0.dev0/test/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-04-18 19:43:45.000000 qiskit-ionq-0.4.0.dev0/test/test_mock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 04:34:28.551550 qiskit-ionq-0.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 04:34:28.547550 qiskit-ionq-0.4.1/.eggs/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-22 04:34:27.000000 qiskit-ionq-0.4.1/.eggs/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 04:34:28.547550 qiskit-ionq-0.4.1/.eggs/pytest_runner-6.0.0-py3.11.egg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 04:34:28.547550 qiskit-ionq-0.4.1/.eggs/pytest_runner-6.0.0-py3.11.egg/EGG-INFO/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-22 04:34:28.000000 qiskit-ionq-0.4.1/.eggs/pytest_runner-6.0.0-py3.11.egg/EGG-INFO/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-22 04:34:28.000000 qiskit-ionq-0.4.1/.eggs/pytest_runner-6.0.0-py3.11.egg/EGG-INFO/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-22 04:34:28.000000 qiskit-ionq-0.4.1/.eggs/pytest_runner-6.0.0-py3.11.egg/EGG-INFO/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-06-22 04:34:19.000000 qiskit-ionq-0.4.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-22 04:34:19.000000 qiskit-ionq-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-06-22 04:34:28.551550 qiskit-ionq-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-06-22 04:34:19.000000 qiskit-ionq-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-22 04:34:19.000000 qiskit-ionq-0.4.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 04:34:28.551550 qiskit-ionq-0.4.1/qiskit_ionq/
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-22 04:34:19.000000 qiskit-ionq-0.4.1/qiskit_ionq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-06-22 04:34:19.000000 qiskit-ionq-0.4.1/qiskit_ionq/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9123 2023-06-22 04:34:19.000000 qiskit-ionq-0.4.1/qiskit_ionq/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15693 2023-06-22 04:34:19.000000 qiskit-ionq-0.4.1/qiskit_ionq/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14234 2023-06-22 04:34:19.000000 qiskit-ionq-0.4.1/qiskit_ionq/ionq_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8403 2023-06-22 04:34:19.000000 qiskit-ionq-0.4.1/qiskit_ionq/ionq_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-06-22 04:34:19.000000 qiskit-ionq-0.4.1/qiskit_ionq/ionq_gates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16466 2023-06-22 04:34:19.000000 qiskit-ionq-0.4.1/qiskit_ionq/ionq_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-06-22 04:34:19.000000 qiskit-ionq-0.4.1/qiskit_ionq/ionq_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-06-22 04:34:19.000000 qiskit-ionq-0.4.1/qiskit_ionq/ionq_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-06-22 04:34:19.000000 qiskit-ionq-0.4.1/qiskit_ionq/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 04:34:28.551550 qiskit-ionq-0.4.1/qiskit_ionq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-06-22 04:34:28.000000 qiskit-ionq-0.4.1/qiskit_ionq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-22 04:34:28.000000 qiskit-ionq-0.4.1/qiskit_ionq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 04:34:28.000000 qiskit-ionq-0.4.1/qiskit_ionq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 04:34:28.000000 qiskit-ionq-0.4.1/qiskit_ionq.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-22 04:34:28.000000 qiskit-ionq-0.4.1/qiskit_ionq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-22 04:34:28.000000 qiskit-ionq-0.4.1/qiskit_ionq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-22 04:34:19.000000 qiskit-ionq-0.4.1/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-22 04:34:19.000000 qiskit-ionq-0.4.1/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-22 04:34:19.000000 qiskit-ionq-0.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-22 04:34:28.551550 qiskit-ionq-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-06-22 04:34:19.000000 qiskit-ionq-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 04:34:28.551550 qiskit-ionq-0.4.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    10551 2023-06-22 04:34:19.000000 qiskit-ionq-0.4.1/test/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-06-22 04:34:19.000000 qiskit-ionq-0.4.1/test/test_mock.py
```

### Comparing `qiskit-ionq-0.4.0.dev0/LICENSE.txt` & `qiskit-ionq-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qiskit-ionq-0.4.0.dev0/PKG-INFO` & `qiskit-ionq-0.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: qiskit-ionq
-Version: 0.4.0.dev0
+Version: 0.4.1
 Summary: Qiskit provider for IonQ backends
 Home-page: https://github.com/qiskit-partners/qiskit-ionq
 Author: IonQ
 Author-email: info@ionq.com
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/qiskit-partners/qiskit-ionq/issues
 Project-URL: Source Code, https://github.com/qiskit-partners/qiskit-ionq
 Keywords: qiskit sdk quantum
-Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
@@ -75,15 +74,15 @@
 ```bash
 export QISKIT_IONQ_API_TOKEN="token"
 ```
 
 Then invoke instantiate the provider without any arguments:
 
 ```python
-from qiskit_ionq import IonQProvider
+from qiskit_ionq import IonQProvider, ErrorMitigation
 
 provider = IonQProvider()
 ```
 
 Once the provider has been instantiated, it may be used to access supported backends:
 
 ```python
@@ -97,31 +96,30 @@
 ### Submitting a Circuit
 
 Once a backend has been specified, it may be used to submit circuits.
 For example, running a Bell State:
 
 ```python
 from qiskit import QuantumCircuit
-from qiskit_ionq.constants import AggregationType
 
 # Create a basic Bell State circuit:
 qc = QuantumCircuit(2, 2)
 qc.h(0)
 qc.cx(0, 1)
 qc.measure([0, 1], [0, 1])
 
-# Run the circuit on IonQ's platform:
-job = simulator_backend.run(qc)
+# Run the circuit on IonQ's platform with error mitigation:
+job = simulator_backend.run(qc, error_mitigation=ErrorMitigation.DEBIASING)
 
 # Print the results.
 print(job.result().get_counts())
 
-# Get results with a different aggregation method when symmetrization
+# Get results with a different aggregation method when debiasing
 # is applied as an error mitigation strategy
-print(job.result(AggregationType.AVERAGE).get_counts())
+print(job.result(sharpen=True).get_counts())
 
 # The simulator specifically provides the the ideal probabilities and creates
 # counts by sampling from these probabilities. The raw probabilities are also accessible:
 print(job.result().get_probabilities())
 ```
 
 ### Basis gates and transpilation
@@ -184,9 +182,7 @@
 
 [Apache License 2.0].
 
 The IonQ logo and Q mark are copyright IonQ, Inc. All rights reserved.
 
 [ionq]: https://www.ionq.com/
 [apache license 2.0]: https://github.com/qiskit-partners/qiskit-ionq/blob/master/LICENSE.txt
-
-
```

### Comparing `qiskit-ionq-0.4.0.dev0/README.md` & `qiskit-ionq-0.4.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 ```bash
 export QISKIT_IONQ_API_TOKEN="token"
 ```
 
 Then invoke instantiate the provider without any arguments:
 
 ```python
-from qiskit_ionq import IonQProvider
+from qiskit_ionq import IonQProvider, ErrorMitigation
 
 provider = IonQProvider()
 ```
 
 Once the provider has been instantiated, it may be used to access supported backends:
 
 ```python
@@ -70,31 +70,30 @@
 ### Submitting a Circuit
 
 Once a backend has been specified, it may be used to submit circuits.
 For example, running a Bell State:
 
 ```python
 from qiskit import QuantumCircuit
-from qiskit_ionq.constants import AggregationType
 
 # Create a basic Bell State circuit:
 qc = QuantumCircuit(2, 2)
 qc.h(0)
 qc.cx(0, 1)
 qc.measure([0, 1], [0, 1])
 
-# Run the circuit on IonQ's platform:
-job = simulator_backend.run(qc)
+# Run the circuit on IonQ's platform with error mitigation:
+job = simulator_backend.run(qc, error_mitigation=ErrorMitigation.DEBIASING)
 
 # Print the results.
 print(job.result().get_counts())
 
-# Get results with a different aggregation method when symmetrization
+# Get results with a different aggregation method when debiasing
 # is applied as an error mitigation strategy
-print(job.result(AggregationType.AVERAGE).get_counts())
+print(job.result(sharpen=True).get_counts())
 
 # The simulator specifically provides the the ideal probabilities and creates
 # counts by sampling from these probabilities. The raw probabilities are also accessible:
 print(job.result().get_probabilities())
 ```
 
 ### Basis gates and transpilation
```

### Comparing `qiskit-ionq-0.4.0.dev0/qiskit_ionq/__init__.py` & `qiskit-ionq-0.4.1/qiskit_ionq/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,8 +25,8 @@
 # limitations under the License.
 
 """Provider for IonQ backends"""
 
 from .ionq_provider import IonQProvider
 from .version import __version__
 from .ionq_gates import GPIGate, GPI2Gate, MSGate
-from .constants import AggregationType, ErrorMitigation
+from .constants import ErrorMitigation
```

### Comparing `qiskit-ionq-0.4.0.dev0/qiskit_ionq/constants.py` & `qiskit-ionq-0.4.1/qiskit_ionq/constants.py`

 * *Files 9% similar despite different names*

```diff
@@ -59,22 +59,15 @@
     READY = jobstatus.JobStatus.QUEUED.name
     RUNNING = jobstatus.JobStatus.RUNNING.name
     CANCELED = jobstatus.JobStatus.CANCELLED.name
     COMPLETED = jobstatus.JobStatus.DONE.name
     FAILED = jobstatus.JobStatus.ERROR.name
 
 
-class AggregationType(enum.Enum):
-    """Class for job results aggregation enumerated type."""
-
-    AVERAGE = "average"
-    PLURALITY = "plurality"
-
-
 class ErrorMitigation(enum.Enum):
     """Class for error mitigation settings enumerated type."""
 
-    SYMMETRIZATION = {"symmetrization": True}
-    NO_SYMMETRIZATION = {"symmetrization": False}
+    DEBIASING = {"debias": True}
+    NO_DEBIASING = {"debias": False}
 
 
 __all__ = ["APIJobStatus", "JobStatusMap"]
```

### Comparing `qiskit-ionq-0.4.0.dev0/qiskit_ionq/exceptions.py` & `qiskit-ionq-0.4.1/qiskit_ionq/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-ionq-0.4.0.dev0/qiskit_ionq/helpers.py` & `qiskit-ionq-0.4.1/qiskit_ionq/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 to IonQ REST API compatible values.
 """
 
 import json
 import gzip
 import base64
 import platform
+import warnings
 
 from qiskit import __version__ as qiskit_terra_version
 from qiskit.circuit import controlledgate as q_cgates
 from qiskit.circuit.library import standard_gates as q_gates
 
 # Use this to get version instead of __version__ to avoid circular dependency.
 from importlib_metadata import version
@@ -185,15 +186,15 @@
                     "rotation"
                     if gateset == "qis"
                     else "phase": float(instruction.params[0])
                 }
             else:
                 rotation = {
                     "phases": [float(t) for t in instruction.params[:2]],
-                    "angle": instruction.params[2]
+                    "angle": instruction.params[2],
                 }
 
         # Default conversion is simple, just gate & target(s).
         targets = [input_circuit.qubits.index(qargs[0])]
         if instruction_name == "ms":
             targets.append(input_circuit.qubits.index(qargs[1]))
 
@@ -227,16 +228,15 @@
             # If this is a multi-control, use more than one qubit.
             if instruction.num_ctrl_qubits > 1:
                 controls = [
                     input_circuit.qubits.index(qargs[i])
                     for i in range(instruction.num_ctrl_qubits)
                 ]
                 targets = [
-                    input_circuit.qubits.index(
-                        qargs[instruction.num_ctrl_qubits])
+                    input_circuit.qubits.index(qargs[instruction.num_ctrl_qubits])
                 ]
             if gate == "swap":
                 # If this is a cswap, we have two targets:
                 targets = [
                     input_circuit.qubits.index(qargs[-2]),
                     input_circuit.qubits.index(qargs[-1]),
                 ]
@@ -340,28 +340,28 @@
         return None
     encoded = input_string.encode()
     decoded = base64.b64decode(encoded)
     decompressed = gzip.decompress(decoded)
     return json.loads(decompressed)
 
 
-def qiskit_to_ionq(circuit, backend, passed_args=None):
+def qiskit_to_ionq(circuit, backend, passed_args=None, extra_query_params=None):
     """Convert a Qiskit circuit to a IonQ compatible dict.
 
     Parameters:
         circuit (:class:`qiskit.circuit.QuantumCircuit`): A Qiskit quantum circuit.
         backend (:class:`qiskit_ionq.IonQBackend`): The IonQ backend.
         passed_args (dict): Dictionary containing additional passed arguments, eg. shots.
+        extra_query_params (dict): Specify any parameters to include in the request
 
     Returns:
         str: A string / JSON-serialized dictionary with IonQ API compatible values.
     """
     passed_args = passed_args or {}
-    ionq_circ, _, meas_map = qiskit_circ_to_ionq_circ(
-        circuit, backend.gateset())
+    ionq_circ, _, meas_map = qiskit_circ_to_ionq_circ(circuit, backend.gateset())
     creg_sizes, clbit_labels = get_register_sizes_and_labels(circuit.cregs)
     qreg_sizes, qubit_labels = get_register_sizes_and_labels(circuit.qregs)
     qiskit_header = compress_dict_to_metadata_string(
         {
             "memory_slots": circuit.num_clbits,  # int
             "global_phase": circuit.global_phase,  # float
             "n_qubits": circuit.num_qubits,  # int
@@ -373,15 +373,22 @@
             # list of [str, int] tuples cardinality num_qubits
             "qreg_sizes": qreg_sizes,
             # list of [str, int] tuples cardinality num_qubits
             "qubit_labels": qubit_labels,
         }
     )
 
-    target = backend.name()[5:]
+    target = backend.name()[5:] if backend.name().startswith("ionq") else backend.name()
+    if target == "qpu":
+        target = "qpu.harmony"  # todo default to cheapest available option
+        warnings.warn(
+            "The ionq_qpu backend is deprecated. Defaulting to ionq_qpu.harmony.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
     ionq_json = {
         "target": target,
         "shots": passed_args.get("shots"),
         "name": circuit.name,
         "input": {
             "format": "ionq.circuit.v0",
             "gateset": backend.gateset(),
@@ -403,14 +410,16 @@
         }
     settings = passed_args.get("job_settings") or None
     if settings is not None:
         ionq_json["settings"] = settings
     error_mitigation = passed_args.get("error_mitigation")
     if error_mitigation and isinstance(error_mitigation, ErrorMitigation):
         ionq_json["error_mitigation"] = error_mitigation.value
+    if extra_query_params is not None:
+        ionq_json.update(extra_query_params)
     return json.dumps(ionq_json)
 
 
 def get_user_agent():
     """Generates the user agent string which is helpful in identifying
     different tools in the internet. Valid user-agent ionq_client header that
     indicates the request is from qiskit_ionq along with the system, os,
@@ -421,19 +430,21 @@
     """
     # from qiskit_ionq import __version__ as qiskit_ionq_version
 
     os_string = f"os/{platform.system()}"
     provider_version_string = f"qiskit-ionq/{version('qiskit_ionq')}"
     qiskit_terra_version_string = f"qiskit-terra/{qiskit_terra_version}"
     python_version_string = f"python/{platform.python_version()}"
-    return f"User-Agent: {provider_version_string} " \
-           f"({qiskit_terra_version_string}) {os_string} " \
-           f"({python_version_string})"
+    return (
+        f"User-Agent: {provider_version_string} "
+        f"({qiskit_terra_version_string}) {os_string} "
+        f"({python_version_string})"
+    )
 
 
 __all__ = [
     "qiskit_to_ionq",
     "qiskit_circ_to_ionq_circ",
     "compress_dict_to_metadata_string",
     "decompress_metadata_string_to_dict",
-    "get_user_agent"
+    "get_user_agent",
 ]
```

### Comparing `qiskit-ionq-0.4.0.dev0/qiskit_ionq/ionq_backend.py` & `qiskit-ionq-0.4.1/qiskit_ionq/ionq_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,15 +130,20 @@
 class IonQBackend(Backend):
     """IonQ Backend base class."""
 
     _client = None
 
     @classmethod
     def _default_options(cls):
-        return Options(shots=1024, job_settings=None, error_mitigation=None)
+        return Options(
+            shots=1024,
+            job_settings=None,
+            error_mitigation=None,
+            extra_query_params=None,
+        )
 
     @property
     def client(self):
         """A lazily populated IonQ API Client.
 
         Returns:
             IonQClient: An instance of a REST API client
@@ -176,16 +181,15 @@
             url = credentials["url"]
         except KeyError as ex:
             raise exceptions.IonQCredentialsError(
                 "Credentials `url` not present in provider."
             ) from ex
 
         if url is None:
-            raise exceptions.IonQCredentialsError(
-                "Credentials `url` may not be None!")
+            raise exceptions.IonQCredentialsError("Credentials `url` may not be None!")
 
         return ionq_client.IonQClient(token, url, self._provider.custom_headers)
 
     # pylint: disable=missing-type-doc,missing-param-doc,arguments-differ,arguments-renamed
     def run(self, circuit, **kwargs):
         """Create and run a job on an IonQ Backend.
 
@@ -226,16 +230,22 @@
                 )
         if "shots" not in kwargs:
             kwargs["shots"] = self.options.shots
         # TODO: Should we merge the two maps, or warn if both are set?
         if "job_settings" not in kwargs:
             kwargs["job_settings"] = self.options.job_settings
         elif self.options.job_settings is not None:
-            warnings.warn(("Option job_settings is set on the backend, and on the request. "
-                           "Ignoring the backend specified option."), UserWarning, stacklevel=2)
+            warnings.warn(
+                (
+                    "Option job_settings is set on the backend, and on the request. "
+                    "Ignoring the backend specified option."
+                ),
+                UserWarning,
+                stacklevel=2,
+            )
         passed_args = kwargs
 
         job = ionq_job.IonQJob(
             self,
             None,
             self.client,
             circuit=circuit,
@@ -334,15 +344,20 @@
         :meth:`get_counts <qiskit_ionq.ionq_job.IonQJob.get_counts>`
         on a job processed by this backend will return counts expressed as
         probabilites, rather than a multiple of shots.
     """
 
     @classmethod
     def _default_options(cls):
-        return Options(shots=1024, job_settings=None, sampler_seed=None, noise_model='ideal')
+        return Options(
+            shots=1024,
+            job_settings=None,
+            sampler_seed=None,
+            noise_model="ideal",
+        )
 
     # pylint: disable=missing-type-doc,missing-param-doc,arguments-differ,useless-super-delegation
     def run(self, circuit, **kwargs):
         """Create and run a job on IonQ's Simulator Backend.
 
         .. WARNING:
```

### Comparing `qiskit-ionq-0.4.0.dev0/qiskit_ionq/ionq_client.py` & `qiskit-ionq-0.4.1/qiskit_ionq/ionq_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Basic API Client for IonQ's REST API"""
 
+from typing import Optional
+from warnings import warn
 import requests
 
 from retry import retry
 
 from . import exceptions
 from .helpers import qiskit_to_ionq, get_user_agent
 from .exceptions import IonQRetriableError
@@ -87,18 +89,26 @@
         Raises:
             IonQAPIError: When the API returns a non-200 status code.
 
         Returns:
             dict: A :mod:`requests <requests>` response :meth:`json <requests.Response.json>` dict.
         """
         as_json = qiskit_to_ionq(
-                job.circuit, job.backend(), job._passed_args
+            job.circuit,
+            job.backend(),
+            job._passed_args,
+            job.extra_query_params,
         )
         req_path = self.make_path("jobs")
-        res = requests.post(req_path, data=as_json, headers=self.api_headers, timeout=30)
+        res = requests.post(
+            req_path,
+            data=as_json,
+            headers=self.api_headers,
+            timeout=30,
+        )
         exceptions.IonQAPIError.raise_for_status(res)
         return res.json()
 
     @retry(exceptions=IonQRetriableError, max_delay=60, backoff=2, jitter=1)
     def retrieve_job(self, job_id: str):
         """Retrieve job information from the IonQ API.
 
@@ -182,45 +192,59 @@
                     "reset": <int>
                 }
             }
 
         Returns:
             dict: A dictionary of an IonQ backend's calibration data.
         """
-        req_path = self.make_path("/".join([
-            "characterizations/backends",
-            backend_name[5:],
-            "current"
-        ]))
+        req_path = self.make_path(
+            "/".join(["characterizations/backends", backend_name[5:], "current"])
+        )
         res = requests.get(req_path, headers=self.api_headers, timeout=30)
         exceptions.IonQAPIError.raise_for_status(res)
 
         return res.json()
 
     @retry(exceptions=IonQRetriableError, max_delay=60, backoff=2, jitter=1)
-    def get_results(self, job_id: str, aggregation=None):
+    def get_results(
+        self,
+        job_id: str,
+        sharpen: Optional[bool] = None,
+        extra_query_params: Optional[dict] = None,
+    ):
         """Retrieve job results from the IonQ API.
 
         The returned JSON dict will only have data if job has completed.
 
         Args:
             job_id (str): The ID of a job to retrieve.
-            aggregation (str): type of results aggregation
+            sharpen (bool): Supported if the job is debiased,
+            allows you to filter out physical qubit bias from the results.
+            extra_query_params (dict): Specify any parameters to include in the request
 
         Raises:
             IonQAPIError: When the API returns a non-200 status code.
 
         Returns:
             dict: A :mod:`requests <requests>` response :meth:`json <requests.Response.json>` dict.
         """
 
         params = {}
 
-        if aggregation:
-            params["aggregation"] = aggregation
+        if sharpen is not None:
+            params["sharpen"] = sharpen
+
+        if extra_query_params is not None:
+            warn(
+                (
+                    f"The parameter(s): {extra_query_params} is not checked by default "
+                    "but will be submitted in the request."
+                )
+            )
+            params.update(extra_query_params)
 
         req_path = self.make_path("jobs", job_id, "results")
         res = requests.get(req_path, params, headers=self.api_headers, timeout=30)
         exceptions.IonQAPIError.raise_for_status(res)
         return res.json()
```

### Comparing `qiskit-ionq-0.4.0.dev0/qiskit_ionq/ionq_gates.py` & `qiskit-ionq-0.4.1/qiskit_ionq/ionq_gates.py`

 * *Files identical despite different names*

### Comparing `qiskit-ionq-0.4.0.dev0/qiskit_ionq/ionq_job.py` & `qiskit-ionq-0.4.1/qiskit_ionq/ionq_job.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 
 import warnings
 import numpy as np
 
 from qiskit.providers import JobV1, jobstatus
 from qiskit.providers.exceptions import JobTimeoutError
 from .ionq_result import IonQResult as Result
-from .constants import AggregationType
 from .helpers import decompress_metadata_string_to_dict
 
 
 from . import constants, exceptions
 
 
 def map_output(data, clbits, num_qubits):
@@ -55,27 +54,31 @@
         return {}
 
     mapped_output = {}
 
     def get_bitvalue(bitstring, bit):
         if bit is not None and 0 <= bit < len(bitstring):
             return bitstring[bit]
-        return '0'
+        return "0"
 
     for value, probability in data.items():
         bitstring = bin(int(value))[2:].rjust(num_qubits, "0")[::-1]
 
-        outvalue = int(''.join([get_bitvalue(bitstring, bit) for bit in clbits])[::-1], 2)
+        outvalue = int(
+            "".join([get_bitvalue(bitstring, bit) for bit in clbits])[::-1], 2
+        )
 
         mapped_output[outvalue] = mapped_output.get(outvalue, 0) + probability
 
     return mapped_output
 
 
-def _build_counts(data, num_qubits, clbits, shots, use_sampler=False, sampler_seed=None):
+def _build_counts(
+    data, num_qubits, clbits, shots, use_sampler=False, sampler_seed=None
+):
     """Map IonQ's ``counts`` onto qiskit's ``counts`` model.
 
     .. NOTE:: For simulator jobs, this method builds counts using a randomly
         generated sampling of the probabilities returned from the API. Because
         this is a random process, rebuilding the results object (by e.g.
         restarting the kernel and getting the job again) without providing a
         sampler_seed in the run method may result in slightly different counts.
@@ -146,33 +149,50 @@
 
     .. IMPORTANT::
        IonQ backends do not support multi-experiment jobs.  Attempting to
        submit a multi-experiment job will raise an exception.
 
     It is not recommended to create Job instances directly, but rather use the
     :meth:`run <IonQBackend.run>` and :meth:`retrieve_job <IonQBackend.retrieve_job>`
-    methods on sub-classe instances of IonQBackend to create and retrieve jobs
+    methods on sub-class instances of IonQBackend to create and retrieve jobs
     (both methods return a job instance).
 
     Attributes:
         circuit(:mod:`QuantumCircuit <qiskit.QuantumCircuit>`): A possibly ``None``
             Qiskit quantum circuit.
         _result(:class:`Result <qiskit.result.Result>`):
             The actual Qiskit Result of this job when done.
     """
 
-    def __init__(self, backend, job_id, client=None, circuit=None, passed_args=None):
+    def __init__(
+        self,
+        backend,
+        job_id,
+        client=None,
+        circuit=None,
+        passed_args=None,
+    ):
         super().__init__(backend, job_id)
         self._client = client or backend.client
-        self._passed_args = passed_args or {"shots": 1024, "sampler_seed": None}
         self._result = None
         self._status = None
         self._execution_time = None
         self._metadata = {}
 
+        if passed_args is not None:
+            self.extra_query_params = (
+                passed_args.pop("extra_query_params")
+                if "extra_query_params" in passed_args
+                else None
+            )
+            self._passed_args = passed_args
+        else:
+            self.extra_query_params = None
+            self._passed_args = {"shots": 1024, "sampler_seed": None}
+
         if circuit is not None:
             self.circuit = circuit
             self._status = jobstatus.JobStatus.INITIALIZING
         else:  # retrieve existing job
             self.circuit = None
             self._status = jobstatus.JobStatus.INITIALIZING
             self._job_id = job_id
@@ -229,15 +249,15 @@
             circuit (str or QuantumCircuit or int or None): Optional.
 
         Returns:
             tuple(dict[str, float], dict[str, float]): A tuple counts, probabilities.
         """
         return self.result().get_probabilities()
 
-    def result(self, aggregation: AggregationType = None):
+    def result(self, sharpen: bool = None, extra_query_params: dict = None):
         """Retrieve job result data.
 
         .. NOTE::
            :attr:`_result` is populated by :meth:`status`, when the job
            status has reached a "final" state.
 
         This method calls the
@@ -251,34 +271,33 @@
             IonQJobError: If the job has reached a final state but
                 the job itself was never converted to a
                 :class:`Result <qiskit.result.Result>`.
 
         Returns:
             Result: A Qiskit :class:`Result <qiskit.result.Result>` representation of this job.
         """
-        # TODO: cache results by aggregation type
+        # TODO: cache results by sharpen
 
-        if aggregation is not None and not isinstance(aggregation, AggregationType):
-            warnings.warn("Invalid aggregation type")
+        if sharpen is not None and not isinstance(sharpen, bool):
+            warnings.warn("Invalid sharpen type")
 
         # Wait for the job to complete.
         try:
             self.wait_for_final_state()
         except JobTimeoutError as ex:
             raise exceptions.IonQJobTimeoutError(
                 "Timed out waiting for job to complete."
             ) from ex
 
         if self._status is jobstatus.JobStatus.DONE:
-            agg_type = (
-                aggregation.value
-                if isinstance(aggregation, AggregationType)
-                else aggregation
+            response = self._client.get_results(
+                job_id=self._job_id,
+                sharpen=sharpen,
+                extra_query_params=extra_query_params,
             )
-            response = self._client.get_results(self._job_id, agg_type)
             self._result = self._format_result(response)
 
         return self._result
 
     def status(self):
         """Retrieve the status of a job
 
@@ -327,15 +346,17 @@
 
         if self._status in jobstatus.JOB_FINAL_STATES:
             self._metadata = response.get("metadata") or {}
 
         if self._status == jobstatus.JobStatus.DONE:
             self._num_qubits = response.get("qubits")
             default_map = list(range(self._num_qubits))
-            self._clbits = (response.get("registers") or {}).get("meas_mapped", default_map)
+            self._clbits = (response.get("registers") or {}).get(
+                "meas_mapped", default_map
+            )
             self._execution_time = response.get("execution_time") / 1000
 
         if self._status == jobstatus.JobStatus.ERROR:
             failure = response.get("failure") or {}
             failure_type = failure.get("code", "")
             failure_message = failure.get("error", "")
             error_message = (
@@ -388,27 +409,29 @@
             if metadata.get("sampler_seed", "").isdigit()
             else None
         )
         qiskit_header = decompress_metadata_string_to_dict(
             metadata.get("qiskit_header", None)
         )
 
-        shots = int(
-            metadata.get("shots") if metadata.get("shots").isdigit() else 1024
-        )
+        shots = int(metadata.get("shots") if metadata.get("shots").isdigit() else 1024)
         job_result = {
             "data": {},
             "shots": shots,
             "header": qiskit_header or {},
             "success": success,
         }
         if self._status == jobstatus.JobStatus.DONE:
             (counts, probabilities) = _build_counts(
-                data, self._num_qubits, self._clbits, shots,
-                use_sampler=is_ideal_simulator, sampler_seed=sampler_seed
+                data,
+                self._num_qubits,
+                self._clbits,
+                shots,
+                use_sampler=is_ideal_simulator,
+                sampler_seed=sampler_seed,
             )
             job_result["data"] = {
                 "counts": counts,
                 "probabilities": probabilities,
                 # Qiskit/experiments relies on this being present in this location in the
                 # ExperimentData class.
                 "metadata": qiskit_header or {},
```

### Comparing `qiskit-ionq-0.4.0.dev0/qiskit_ionq/ionq_provider.py` & `qiskit-ionq-0.4.1/qiskit_ionq/ionq_provider.py`

 * *Files identical despite different names*

### Comparing `qiskit-ionq-0.4.0.dev0/qiskit_ionq/ionq_result.py` & `qiskit-ionq-0.4.1/qiskit_ionq/ionq_result.py`

 * *Files identical despite different names*

### Comparing `qiskit-ionq-0.4.0.dev0/qiskit_ionq/version.py` & `qiskit-ionq-0.4.1/qiskit_ionq/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 import pathlib
 import subprocess
 from typing import List
 
 pkg_parent = pathlib.Path(__file__).parent.parent.absolute()
 
 # major, minor, micro
-VERSION_INFO = ".".join(map(str, (0, 4, 0, "dev0")))
+VERSION_INFO = ".".join(map(str, (0, 4, 1)))
 
 
 def _minimal_ext_cmd(cmd: List[str]) -> bytes:
     # construct minimal environment
     env = {
         "LANGUAGE": "C",  # LANGUAGE is used on win32
         "LANG": "C",
```

### Comparing `qiskit-ionq-0.4.0.dev0/qiskit_ionq.egg-info/PKG-INFO` & `qiskit-ionq-0.4.1/qiskit_ionq.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: qiskit-ionq
-Version: 0.4.0.dev0
+Version: 0.4.1
 Summary: Qiskit provider for IonQ backends
 Home-page: https://github.com/qiskit-partners/qiskit-ionq
 Author: IonQ
 Author-email: info@ionq.com
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/qiskit-partners/qiskit-ionq/issues
 Project-URL: Source Code, https://github.com/qiskit-partners/qiskit-ionq
 Keywords: qiskit sdk quantum
-Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
@@ -75,15 +74,15 @@
 ```bash
 export QISKIT_IONQ_API_TOKEN="token"
 ```
 
 Then invoke instantiate the provider without any arguments:
 
 ```python
-from qiskit_ionq import IonQProvider
+from qiskit_ionq import IonQProvider, ErrorMitigation
 
 provider = IonQProvider()
 ```
 
 Once the provider has been instantiated, it may be used to access supported backends:
 
 ```python
@@ -97,31 +96,30 @@
 ### Submitting a Circuit
 
 Once a backend has been specified, it may be used to submit circuits.
 For example, running a Bell State:
 
 ```python
 from qiskit import QuantumCircuit
-from qiskit_ionq.constants import AggregationType
 
 # Create a basic Bell State circuit:
 qc = QuantumCircuit(2, 2)
 qc.h(0)
 qc.cx(0, 1)
 qc.measure([0, 1], [0, 1])
 
-# Run the circuit on IonQ's platform:
-job = simulator_backend.run(qc)
+# Run the circuit on IonQ's platform with error mitigation:
+job = simulator_backend.run(qc, error_mitigation=ErrorMitigation.DEBIASING)
 
 # Print the results.
 print(job.result().get_counts())
 
-# Get results with a different aggregation method when symmetrization
+# Get results with a different aggregation method when debiasing
 # is applied as an error mitigation strategy
-print(job.result(AggregationType.AVERAGE).get_counts())
+print(job.result(sharpen=True).get_counts())
 
 # The simulator specifically provides the the ideal probabilities and creates
 # counts by sampling from these probabilities. The raw probabilities are also accessible:
 print(job.result().get_probabilities())
 ```
 
 ### Basis gates and transpilation
@@ -184,9 +182,7 @@
 
 [Apache License 2.0].
 
 The IonQ logo and Q mark are copyright IonQ, Inc. All rights reserved.
 
 [ionq]: https://www.ionq.com/
 [apache license 2.0]: https://github.com/qiskit-partners/qiskit-ionq/blob/master/LICENSE.txt
-
-
```

### Comparing `qiskit-ionq-0.4.0.dev0/qiskit_ionq.egg-info/SOURCES.txt` & `qiskit-ionq-0.4.1/qiskit_ionq.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 setup.cfg
 setup.py
 ./LICENSE.txt
 ./requirements-docs.txt
 ./requirements-test.txt
 ./requirements.txt
 ./.eggs/README.txt
-./.eggs/pytest_runner-6.0.0-py3.9.egg/EGG-INFO/entry_points.txt
-./.eggs/pytest_runner-6.0.0-py3.9.egg/EGG-INFO/requires.txt
-./.eggs/pytest_runner-6.0.0-py3.9.egg/EGG-INFO/top_level.txt
+./.eggs/pytest_runner-6.0.0-py3.11.egg/EGG-INFO/entry_points.txt
+./.eggs/pytest_runner-6.0.0-py3.11.egg/EGG-INFO/requires.txt
+./.eggs/pytest_runner-6.0.0-py3.11.egg/EGG-INFO/top_level.txt
 ./qiskit_ionq.egg-info/SOURCES.txt
 ./qiskit_ionq.egg-info/dependency_links.txt
 ./qiskit_ionq.egg-info/requires.txt
 ./qiskit_ionq.egg-info/top_level.txt
 qiskit_ionq/__init__.py
 qiskit_ionq/constants.py
 qiskit_ionq/exceptions.py
```

### Comparing `qiskit-ionq-0.4.0.dev0/setup.py` & `qiskit-ionq-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `qiskit-ionq-0.4.0.dev0/test/test_exceptions.py` & `qiskit-ionq-0.4.1/test/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-ionq-0.4.0.dev0/test/test_mock.py` & `qiskit-ionq-0.4.1/test/test_mock.py`

 * *Files identical despite different names*

