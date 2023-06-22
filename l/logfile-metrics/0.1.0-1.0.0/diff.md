# Comparing `tmp/logfile_metrics-0.1.0.tar.gz` & `tmp/logfile_metrics-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logfile_metrics-0.1.0.tar", max compression
+gzip compressed data, was "logfile_metrics-1.0.0.tar", max compression
```

## Comparing `logfile_metrics-0.1.0.tar` & `logfile_metrics-1.0.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-06-21 07:08:03.639407 logfile_metrics-0.1.0/logfile_metrics/__init__.py
--rw-r--r--   0        0        0     1827 2023-06-21 08:54:44.273953 logfile_metrics-0.1.0/logfile_metrics/__main__.py
--rw-r--r--   0        0        0    15100 2023-06-21 10:13:17.886193 logfile_metrics-0.1.0/logfile_metrics/logfile_metrics.py
--rw-r--r--   0        0        0     1020 2023-06-21 09:59:14.938210 logfile_metrics-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      356 2023-06-21 05:07:43.426524 logfile_metrics-0.1.0/README.md
--rw-r--r--   0        0        0      995 1970-01-01 00:00:00.000000 logfile_metrics-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-21 07:08:03.639407 logfile_metrics-1.0.0/logfile_metrics/__init__.py
+-rw-r--r--   0        0        0     1827 2023-06-21 08:54:44.273953 logfile_metrics-1.0.0/logfile_metrics/__main__.py
+-rw-r--r--   0        0        0    15178 2023-06-22 04:30:28.875744 logfile_metrics-1.0.0/logfile_metrics/logfile_metrics.py
+-rw-r--r--   0        0        0     1020 2023-06-22 06:30:52.853133 logfile_metrics-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      356 2023-06-21 05:07:43.426524 logfile_metrics-1.0.0/README.md
+-rw-r--r--   0        0        0      995 1970-01-01 00:00:00.000000 logfile_metrics-1.0.0/PKG-INFO
```

### Comparing `logfile_metrics-0.1.0/logfile_metrics/__main__.py` & `logfile_metrics-1.0.0/logfile_metrics/__main__.py`

 * *Files identical despite different names*

### Comparing `logfile_metrics-0.1.0/logfile_metrics/logfile_metrics.py` & `logfile_metrics-1.0.0/logfile_metrics/logfile_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,17 @@
                 except Exception:  # pylint: disable=broad-exception-caught
                     pass
 
         if match is not None:
             # Update fields from match object
             fields.update(match)
             # Add new fields if given
-            fields.update({dest: fields[src] for dest, src in rule.get("add", [])})
+            for assignment in rule.get("add", []):
+                dest, src = [s.strip() for s in assignment.split("=")]
+                fields[dest] = fields[src]
         else:
             if rule.get("mismatch_break", False):
                 break
 
     return fields
 
 
@@ -273,16 +275,16 @@
             opt=["opt", "mismatch_break", "add"],
             where="rule configuration",
         )
         addlist = rule.get("add", [])
         assert isinstance(addlist, list), "'add' is expected to be an array"
         for a in addlist:
             assert (
-                isinstance(a, list) and len(cast(List[str], a)) == 2
-            ), "'add' items are expected to be [dest, src] pair ('dest' and 'src' are field names)"
+                isinstance(a, str) and len(a.split("=")) == 2
+            ), "'add' items must be strings of 'dest = src' format ('dest' and 'src' are fields names)"
 
     metrics = job["metrics"]
     assert isinstance(metrics, list), "job 'metrics' is expected to be an array"
     metrics = cast(
         List[Dict[str, Any]], metrics
     )  # Do nothing at runtime, for type checker only.
     for metric in metrics:
```

### Comparing `logfile_metrics-0.1.0/pyproject.toml` & `logfile_metrics-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "logfile_metrics"
-version = "0.1.0"
+version = "1.0.0"
 description = "Parse the logfile(s) and output the results in metrics file format for Prometheus."
 authors = ["Evgeny Klunko <eklunko@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 toml = "^0.10.2"
```

### Comparing `logfile_metrics-0.1.0/PKG-INFO` & `logfile_metrics-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logfile-metrics
-Version: 0.1.0
+Version: 1.0.0
 Summary: Parse the logfile(s) and output the results in metrics file format for Prometheus.
 Author: Evgeny Klunko
 Author-email: eklunko@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

