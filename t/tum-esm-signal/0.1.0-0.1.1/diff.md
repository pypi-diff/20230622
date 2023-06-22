# Comparing `tmp/tum_esm_signal-0.1.0.tar.gz` & `tmp/tum_esm_signal-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tum_esm_signal-0.1.0.tar", max compression
+gzip compressed data, was "tum_esm_signal-0.1.1.tar", max compression
```

## Comparing `tum_esm_signal-0.1.0.tar` & `tum_esm_signal-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       83 2023-06-22 10:19:18.781597 tum_esm_signal-0.1.0/README.md
--rw-r--r--   0        0        0      940 2023-06-22 11:38:50.127953 tum_esm_signal-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       85 2023-06-22 10:42:21.174903 tum_esm_signal-0.1.0/tum_esm_signal/__init__.py
--rw-r--r--   0        0        0     1469 2023-06-22 11:32:52.786253 tum_esm_signal-0.1.0/tum_esm_signal/client.py
--rw-r--r--   0        0        0     3872 2023-06-22 11:33:36.395624 tum_esm_signal-0.1.0/tum_esm_signal/pocketbase.py
--rw-r--r--   0        0        0        0 2023-06-22 11:37:33.577931 tum_esm_signal-0.1.0/tum_esm_signal/py.typed
--rw-r--r--   0        0        0      861 1970-01-01 00:00:00.000000 tum_esm_signal-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      607 2023-06-22 11:48:10.894351 tum_esm_signal-0.1.1/README.md
+-rw-r--r--   0        0        0      940 2023-06-22 11:48:49.022738 tum_esm_signal-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       85 2023-06-22 10:42:21.174903 tum_esm_signal-0.1.1/tum_esm_signal/__init__.py
+-rw-r--r--   0        0        0     1469 2023-06-22 11:32:52.786253 tum_esm_signal-0.1.1/tum_esm_signal/client.py
+-rw-r--r--   0        0        0     3872 2023-06-22 11:33:36.395624 tum_esm_signal-0.1.1/tum_esm_signal/pocketbase.py
+-rw-r--r--   0        0        0        0 2023-06-22 11:37:33.577931 tum_esm_signal-0.1.1/tum_esm_signal/py.typed
+-rw-r--r--   0        0        0     1385 1970-01-01 00:00:00.000000 tum_esm_signal-0.1.1/PKG-INFO
```

### Comparing `tum_esm_signal-0.1.0/pyproject.toml` & `tum_esm_signal-0.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tum_esm_signal"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Moritz Makowski <moritz@dostuffthatmatters.dev>"]
 readme = "README.md"
 packages = [
     {include = "tum_esm_signal"},
     {include = "tum_esm_signal/py.typed"}
 ]
```

### Comparing `tum_esm_signal-0.1.0/tum_esm_signal/client.py` & `tum_esm_signal-0.1.1/tum_esm_signal/client.py`

 * *Files identical despite different names*

### Comparing `tum_esm_signal-0.1.0/tum_esm_signal/pocketbase.py` & `tum_esm_signal-0.1.1/tum_esm_signal/pocketbase.py`

 * *Files identical despite different names*

### Comparing `tum_esm_signal-0.1.0/PKG-INFO` & `tum_esm_signal-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tum-esm-signal
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Home-page: https://github.com/tum-esm/signal
 License: AGPL-3.0-only
 Keywords: python,library,utilities,plotting
 Author: Moritz Makowski
 Author-email: moritz@dostuffthatmatters.dev
 Requires-Python: >=3.9,<4.0
@@ -16,12 +16,41 @@
 Requires-Dist: pendulum (>=2.1.2,<3.0.0)
 Requires-Dist: pydantic (>=1.10.9,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Repository, https://github.com/tum-esm/signal
 Description-Content-Type: text/markdown
 
 
-## TUM ESM Signal
+# TUM ESM Signal
 
 Replaces the `shareable-timeseries-visualization` repository.
 
+**Installation:**
 
+```bash
+poetry add tum-esm-signal
+# or
+pip install tum-esm-signal
+```
+
+**Usage:**
+
+```python
+signal_client = TUM_ESM_SignalClient(
+    cms_identity=cms_identity,
+    cms_password=cms_password,
+    collection_name="test",
+    table_name="test",
+    column_name="test",
+    sensor_id="test",
+    unit="test",
+    description="test",
+    minimum=0,
+    maximum=10,
+    decimal_places=0,
+)
+
+while True:
+    print("Sending datapoint")
+    signal_client.add_datapoint(random.randint(0, 10))
+    time.sleep(2)
+```
```

